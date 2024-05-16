# Comparing `tmp/dooth-1.1.1-py3-none-any.whl.zip` & `tmp/dooth-1.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,14 @@
-Zip file size: 5511 bytes, number of entries: 11
+Zip file size: 6034 bytes, number of entries: 12
 -rw-r--r--  2.0 unx        0 b- defN 24-May-10 18:16 doot/__init__.py
--rw-r--r--  2.0 unx     8110 b- defN 24-May-12 16:21 doot/bot.py
--rw-r--r--  2.0 unx      454 b- defN 24-May-12 14:37 doot/command_handler.py
+-rw-r--r--  2.0 unx     8510 b- defN 24-May-16 06:02 doot/bot.py
+-rw-r--r--  2.0 unx      329 b- defN 24-May-16 05:53 doot/callback.py
+-rw-r--r--  2.0 unx      728 b- defN 24-May-16 06:02 doot/command_handler.py
 -rw-r--r--  2.0 unx      232 b- defN 24-May-12 12:24 doot/exception.py
 -rw-r--r--  2.0 unx     4255 b- defN 24-May-11 09:22 doot/message.py
--rw-r--r--  2.0 unx      444 b- defN 24-May-12 14:37 doot/message_handler.py
+-rw-r--r--  2.0 unx      702 b- defN 24-May-16 06:02 doot/message_handler.py
 -rw-r--r--  2.0 unx     2527 b- defN 24-May-12 15:15 doot/response.py
--rw-r--r--  2.0 unx       74 b- defN 24-May-12 16:22 dooth-1.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-12 16:22 dooth-1.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 24-May-12 16:22 dooth-1.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      801 b- defN 24-May-12 16:22 dooth-1.1.1.dist-info/RECORD
-11 files, 16994 bytes uncompressed, 4171 bytes compressed:  75.5%
+-rw-r--r--  2.0 unx       74 b- defN 24-May-16 06:47 dooth-1.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-16 06:47 dooth-1.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 24-May-16 06:47 dooth-1.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      873 b- defN 24-May-16 06:47 dooth-1.1.2.dist-info/RECORD
+12 files, 18327 bytes uncompressed, 4586 bytes compressed:  75.0%
```

## zipnote {}

```diff
@@ -1,13 +1,16 @@
 Filename: doot/__init__.py
 Comment: 
 
 Filename: doot/bot.py
 Comment: 
 
+Filename: doot/callback.py
+Comment: 
+
 Filename: doot/command_handler.py
 Comment: 
 
 Filename: doot/exception.py
 Comment: 
 
 Filename: doot/message.py
@@ -15,20 +18,20 @@
 
 Filename: doot/message_handler.py
 Comment: 
 
 Filename: doot/response.py
 Comment: 
 
-Filename: dooth-1.1.1.dist-info/METADATA
+Filename: dooth-1.1.2.dist-info/METADATA
 Comment: 
 
-Filename: dooth-1.1.1.dist-info/WHEEL
+Filename: dooth-1.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: dooth-1.1.1.dist-info/top_level.txt
+Filename: dooth-1.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: dooth-1.1.1.dist-info/RECORD
+Filename: dooth-1.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## doot/bot.py

```diff
@@ -1,38 +1,36 @@
-import asyncio
-import datetime
 import json
 import logging
 import os
 import threading
 import time
 
 import requests
-from urllib.parse import quote
 
+from doot.callback import BotCallback
 from doot.command_handler import CommandHandler, DefaultCommandHandler
 from doot.exception import CommandProcessingError, MessageProcessingError
 from doot.message import Mapper, Update
 from doot.message_handler import MessageHandler, DefaultMessageHandler
 from doot.response import HandlerResponse
 
 
-class Bot:
+class Bot(BotCallback):
 
     def __init__(self, token: str):
         self.__logger = logging.getLogger(self.__class__.__name__)
         self.__base_url = f'https://api.telegram.org/bot{token}'
         self.__send_msg_url = f'{self.__base_url}/sendMessage'
         self.__get_updates_url = f'{self.__base_url}/getUpdates'
         self.__send_photo_url = f'{self.__base_url}/sendPhoto'
         self.__send_doc_url = f'{self.__base_url}/sendDocument'
         self.__next_update_id = -1
 
-        self.command_handler: CommandHandler = DefaultCommandHandler()
-        self.message_handler: MessageHandler = DefaultMessageHandler()
+        self.command_handler: CommandHandler = DefaultCommandHandler(self)
+        self.message_handler: MessageHandler = DefaultMessageHandler(self)
 
     def send_notification(self, response: HandlerResponse, chat_id: int, disable_web_page_preview: bool = False):
 
         params = {
             'chat_id': chat_id,
             'text': response.get_message(),
             'parse_mode': response.get_message_parse_mode(),
@@ -127,39 +125,47 @@
         for e in update.message.text.split(' '):
             if e != '':
                 args.append(e)
         command = args.pop(0)
 
         response = None
         try:
-            response = self.command_handler.handle_command(command, args)
+            response = self.command_handler.handle_command(command, args, update.message.chat.id)
             self.respond(response, update)
         except Exception as e:
             raise CommandProcessingError(e)
         finally:
             self._delete_files_in_response(response)
 
     def _process_message(self, update: Update):
         response = None
         try:
-            response = self.message_handler.handle_message(update.message.text)
+            response = self.message_handler.handle_message(update.message.text, update.message.chat.id)
             self.respond(response, update)
         except Exception as e:
             raise MessageProcessingError(e)
         finally:
             self._delete_files_in_response(response)
 
     def respond(self, response: HandlerResponse, update: Update):
         if response.get_type() == 'text':
             self.send_notification(response, update.message.chat.id)
         elif response.get_type() == 'photo':
             self.send_photo(response, update.message.chat.id)
         elif response.get_type() == 'document':
             self.send_doc(response, update.message.chat.id)
 
+    def interim_response(self, response: HandlerResponse, chat_id: int):
+        if response.get_type() == 'text':
+            self.send_notification(response, chat_id)
+        elif response.get_type() == 'photo':
+            self.send_photo(response, chat_id)
+        elif response.get_type() == 'document':
+            self.send_doc(response, chat_id)
+
     def _delete_files_in_response(self, response: HandlerResponse):
         if response is None:
             return
 
         if response.get_photo_path() is not None:
             try:
                 os.remove(response.get_photo_path())
```

## doot/command_handler.py

```diff
@@ -1,19 +1,25 @@
+import logging
 from abc import ABC, abstractmethod
 
+from doot.callback import BotCallback
 from doot.response import HandlerResponse
 
 
 class CommandHandler(ABC):
 
-    def __init__(self):
-        pass
+    def __init__(self, callback: BotCallback):
+        self._logger = logging.getLogger(self.__class__.__name__)
+        self._callback = callback
 
     @abstractmethod
-    def handle_command(self, command: str, args: list) -> HandlerResponse:
+    def handle_command(self, command: str, args: list, chat_id: int) -> HandlerResponse:
         pass
 
 
 class DefaultCommandHandler(CommandHandler):
 
-    def handle_command(self, command: str, args: list) -> HandlerResponse:
+    def __init__(self, callback: BotCallback):
+        super().__init__(callback)
+
+    def handle_command(self, command: str, args: list, chat_id: int) -> HandlerResponse:
         return HandlerResponse(message=f'Command: {command}\nArgs: {args}')
```

## doot/message_handler.py

```diff
@@ -1,20 +1,25 @@
-import datetime
+import logging
 from abc import ABC, abstractmethod
 
+from doot.callback import BotCallback
 from doot.response import HandlerResponse
 
 
 class MessageHandler(ABC):
 
-    def __init__(self):
-        pass
+    def __init__(self, callback: BotCallback):
+        self._logger = logging.getLogger(self.__class__.__name__)
+        self._callback = callback
 
     @abstractmethod
-    def handle_message(self, message_text: str) -> HandlerResponse:
+    def handle_message(self, message_text: str, chat_id: int) -> HandlerResponse:
         pass
 
 
 class DefaultMessageHandler(MessageHandler):
 
-    def handle_message(self, message_text: str) -> HandlerResponse:
+    def __init__(self, callback: BotCallback):
+        super().__init__(callback)
+
+    def handle_message(self, message_text: str, chat_id: int) -> HandlerResponse:
         return HandlerResponse(message=f'Echo: {message_text}')
```

## Comparing `dooth-1.1.1.dist-info/RECORD` & `dooth-1.1.2.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 doot/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-doot/bot.py,sha256=D9ZgoE2cVaHx40SWUkeJiIzZEI1ynyd55j7agRHTPLg,8110
-doot/command_handler.py,sha256=euFeDZeJPHBgMR8EzAzGbyPJCitdIVVtapcIrut38pI,454
+doot/bot.py,sha256=gIw8Ah7OBJpUhWRB7DcTdV_nBO2ePKf4Wex8rWbz0Sk,8510
+doot/callback.py,sha256=Yyxw7P994bus6CCdc43G8enYdArwZc8qgnXICkp_JaY,329
+doot/command_handler.py,sha256=39fV4bk2XP21z6D4MBTNqqk-5hxGSauf0K9v1Q0nGrM,728
 doot/exception.py,sha256=Ys10w9WqxYIyzn6QPbkxoX_ykgMf_fTUDIH7UsRAWyQ,232
 doot/message.py,sha256=hiXeJ7TOTMvF2TGXj0fqbo3LTAxPi_lW6H1bMeG6UEI,4255
-doot/message_handler.py,sha256=KwDN7B0ig7GUXjeo6PJ-1RLehz4ilyiBHA_dSXC9zFw,444
+doot/message_handler.py,sha256=vA_HPP31iHUF-L4OmW4_oSPeXWegYhfJmN1zURYnpi0,702
 doot/response.py,sha256=iAFsgMb3nEJ_gRizDFG7xv-euzIbqRZYVpL6KfsnLX0,2527
-dooth-1.1.1.dist-info/METADATA,sha256=9q3P3DuWZ2WMLn35Z2kBR0wbT92qGARdfwA6OLZdHvQ,74
-dooth-1.1.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-dooth-1.1.1.dist-info/top_level.txt,sha256=259wJJXfvmJdcDJ_Bs4a1f9A0kyxtMNUn1hzSoaHU94,5
-dooth-1.1.1.dist-info/RECORD,,
+dooth-1.1.2.dist-info/METADATA,sha256=GiptRYWOA4z6ukn7KPpyE9rMRCjyFPrt9sQXO12sHp8,74
+dooth-1.1.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+dooth-1.1.2.dist-info/top_level.txt,sha256=259wJJXfvmJdcDJ_Bs4a1f9A0kyxtMNUn1hzSoaHU94,5
+dooth-1.1.2.dist-info/RECORD,,
```

