# Comparing `tmp/tg_signer-0.1.2.tar.gz` & `tmp/tg_signer-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tg_signer-0.1.2.tar", last modified: Thu May 16 07:50:07 2024, max compression
+gzip compressed data, was "tg_signer-0.1.3.tar", last modified: Thu May 16 09:35:34 2024, max compression
```

## Comparing `tg_signer-0.1.2.tar` & `tg_signer-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 luming     (501) staff       (20)        0 2024-05-16 07:50:07.963207 tg_signer-0.1.2/
--rw-r--r--   0 luming     (501) staff       (20)     1493 2024-01-07 10:02:22.000000 tg_signer-0.1.2/LICENSE
--rw-r--r--   0 luming     (501) staff       (20)     1160 2024-05-16 07:50:07.963153 tg_signer-0.1.2/PKG-INFO
--rw-r--r--   0 luming     (501) staff       (20)      607 2024-05-16 07:49:00.000000 tg_signer-0.1.2/README.md
--rw-r--r--   0 luming     (501) staff       (20)      979 2024-05-16 07:50:07.965231 tg_signer-0.1.2/setup.cfg
--rw-r--r--   0 luming     (501) staff       (20)       38 2024-01-07 10:02:22.000000 tg_signer-0.1.2/setup.py
-drwxr-xr-x   0 luming     (501) staff       (20)        0 2024-05-16 07:50:07.961618 tg_signer-0.1.2/tg_signer/
--rw-r--r--   0 luming     (501) staff       (20)       22 2024-05-16 07:49:56.000000 tg_signer-0.1.2/tg_signer/__init__.py
--rw-r--r--   0 luming     (501) staff       (20)       66 2024-05-16 07:03:40.000000 tg_signer-0.1.2/tg_signer/__main__.py
--rw-r--r--   0 luming     (501) staff       (20)     8557 2024-05-16 07:49:00.000000 tg_signer-0.1.2/tg_signer/signer.py
-drwxr-xr-x   0 luming     (501) staff       (20)        0 2024-05-16 07:50:07.962982 tg_signer-0.1.2/tg_signer.egg-info/
--rw-r--r--   0 luming     (501) staff       (20)     1160 2024-05-16 07:50:07.000000 tg_signer-0.1.2/tg_signer.egg-info/PKG-INFO
--rw-r--r--   0 luming     (501) staff       (20)      300 2024-05-16 07:50:07.000000 tg_signer-0.1.2/tg_signer.egg-info/SOURCES.txt
--rw-r--r--   0 luming     (501) staff       (20)        1 2024-05-16 07:50:07.000000 tg_signer-0.1.2/tg_signer.egg-info/dependency_links.txt
--rw-r--r--   0 luming     (501) staff       (20)       53 2024-05-16 07:50:07.000000 tg_signer-0.1.2/tg_signer.egg-info/entry_points.txt
--rw-r--r--   0 luming     (501) staff       (20)       18 2024-05-16 07:50:07.000000 tg_signer-0.1.2/tg_signer.egg-info/requires.txt
--rw-r--r--   0 luming     (501) staff       (20)       10 2024-05-16 07:50:07.000000 tg_signer-0.1.2/tg_signer.egg-info/top_level.txt
+drwxr-xr-x   0 luming     (501) staff       (20)        0 2024-05-16 09:35:34.973740 tg_signer-0.1.3/
+-rw-r--r--   0 luming     (501) staff       (20)     1493 2024-01-07 10:02:22.000000 tg_signer-0.1.3/LICENSE
+-rw-r--r--   0 luming     (501) staff       (20)     1206 2024-05-16 09:35:34.973678 tg_signer-0.1.3/PKG-INFO
+-rw-r--r--   0 luming     (501) staff       (20)      607 2024-05-16 07:49:00.000000 tg_signer-0.1.3/README.md
+-rw-r--r--   0 luming     (501) staff       (20)     1017 2024-05-16 09:35:34.974450 tg_signer-0.1.3/setup.cfg
+-rw-r--r--   0 luming     (501) staff       (20)       38 2024-01-07 10:02:22.000000 tg_signer-0.1.3/setup.py
+drwxr-xr-x   0 luming     (501) staff       (20)        0 2024-05-16 09:35:34.972322 tg_signer-0.1.3/tg_signer/
+-rw-r--r--   0 luming     (501) staff       (20)       22 2024-05-16 08:34:11.000000 tg_signer-0.1.3/tg_signer/__init__.py
+-rw-r--r--   0 luming     (501) staff       (20)       66 2024-05-16 07:03:40.000000 tg_signer-0.1.3/tg_signer/__main__.py
+-rw-r--r--   0 luming     (501) staff       (20)     8896 2024-05-16 08:48:02.000000 tg_signer-0.1.3/tg_signer/signer.py
+drwxr-xr-x   0 luming     (501) staff       (20)        0 2024-05-16 09:35:34.973405 tg_signer-0.1.3/tg_signer.egg-info/
+-rw-r--r--   0 luming     (501) staff       (20)     1206 2024-05-16 09:35:34.000000 tg_signer-0.1.3/tg_signer.egg-info/PKG-INFO
+-rw-r--r--   0 luming     (501) staff       (20)      300 2024-05-16 09:35:34.000000 tg_signer-0.1.3/tg_signer.egg-info/SOURCES.txt
+-rw-r--r--   0 luming     (501) staff       (20)        1 2024-05-16 09:35:34.000000 tg_signer-0.1.3/tg_signer.egg-info/dependency_links.txt
+-rw-r--r--   0 luming     (501) staff       (20)       53 2024-05-16 09:35:34.000000 tg_signer-0.1.3/tg_signer.egg-info/entry_points.txt
+-rw-r--r--   0 luming     (501) staff       (20)       30 2024-05-16 09:35:34.000000 tg_signer-0.1.3/tg_signer.egg-info/requires.txt
+-rw-r--r--   0 luming     (501) staff       (20)       10 2024-05-16 09:35:34.000000 tg_signer-0.1.3/tg_signer.egg-info/top_level.txt
```

### Comparing `tg_signer-0.1.2/LICENSE` & `tg_signer-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tg_signer-0.1.2/PKG-INFO` & `tg_signer-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: tg-signer
-Version: 0.1.2
+Version: 0.1.3
 Summary: Telegram signer
 Home-page: https://github.com/amchii/tg-signer
 Author: Amchii
 Author-email: finethankuandyou@gmail.com
 License: BSD 3-Clause License
 Project-URL: Source, https://github.com/amchii/tg-signer
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyrogram
-Requires-Dist: tgcrypto
+Provides-Extra: tgcrypto
+Requires-Dist: tgcrypto; extra == "tgcrypto"
 
 # Telegram Signer - Telegram每日自动签到
 
 ## Install
 ```
 pip install -U tg-signer
 ```
```

### Comparing `tg_signer-0.1.2/README.md` & `tg_signer-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `tg_signer-0.1.2/setup.cfg` & `tg_signer-0.1.3/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 
 [options]
 python_requires = >=3.8
 include_package_data = True
 packages = find:
 install_requires = 
 	pyrogram
+
+[options.extras_require]
+tgcrypto = 
 	tgcrypto
 
 [options.entry_points]
 console_scripts = 
 	tg-signer = tg_signer.__main__:cli
 
 [flake8]
```

### Comparing `tg_signer-0.1.2/tg_signer/signer.py` & `tg_signer-0.1.3/tg_signer/signer.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,20 +52,15 @@
             "password": r.password,
         }
 
 
 def get_client(name: str = "my_account", proxy=None):
     proxy = proxy or get_proxy()
     api_id, api_hash = get_api_config()
-    return Client(
-        name,
-        api_id,
-        api_hash,
-        proxy=proxy,
-    )
+    return Client(name, api_id, api_hash, proxy=proxy, workdir=".")
 
 
 app = get_client()
 
 
 def get_now():
     return datetime.now(tz=timezone(timedelta(hours=8)))
@@ -132,67 +127,70 @@
     @property
     def config_file(self):
         return self.sign_dir.joinpath("config.json")
 
     def get_me(self):
         file = self.base_dir.joinpath("me.json")
         if file.is_file():
-            with open(file, "r") as f:
+            with open(file, "r", encoding="utf-8") as f:
                 data = json.load(f)
             data.pop("_")
             user = User(
                 id=data["id"],
                 is_self=True,
                 first_name=data.get("first_name"),
                 last_name=data.get("last_name"),
             )
             return user
 
     def set_me(self, user: User):
         self.user = user
-        with open(self.base_dir.joinpath("me.json"), "w") as fp:
+        with open(self.base_dir.joinpath("me.json"), "w", encoding="utf-8") as fp:
             fp.write(str(user))
 
     def ask_for_config(self) -> "SignConfig":
-        chat_id = int(input("Chat ID: "))
-        sign_text = input("签到文本: ")
-        sign_at_str = input("每日签到时间（如 06:00:00）: ")
+        chat_id = int(input("Chat ID（登录时最近对话输出中的ID）: "))
+        sign_text = input("签到文本（如 /sign）: ") or "/sign"
+        sign_at_str = input("每日签到时间（如 06:00:00）: ") or "06:00:00"
         sign_at_str = sign_at_str.replace("：", ":").strip()
         sign_at = time.fromisoformat(sign_at_str)
         random_seconds_str = input("签到时间误差随机秒数（默认为0）: ") or "0"
         random_seconds = int(float(random_seconds_str))
         return SignConfig(chat_id, sign_text, sign_at, random_seconds)
 
     def reconfig(self):
         config = self.ask_for_config()
-        with open(self.config_file, "w") as fp:
+        with open(self.config_file, "w", encoding="utf-8") as fp:
             json.dump(config.to_jsonable(), fp)
         return config
 
     def load_config(self) -> "SignConfig":
         if not self.config_file.exists():
             config = self.reconfig()
         else:
-            with open(self.config_file, "r") as fp:
+            with open(self.config_file, "r", encoding="utf-8") as fp:
                 config = SignConfig.from_json(json.load(fp))
         return config
 
     def load_sign_record(self):
         sign_record = {}
         if not self.sign_record_file.is_file():
-            with open(self.sign_record_file, "w") as fp:
+            with open(self.sign_record_file, "w", encoding="utf-8") as fp:
                 json.dump(sign_record, fp)
         else:
-            with open(self.sign_record_file, "r") as fp:
+            with open(self.sign_record_file, "r", encoding="utf-8") as fp:
                 sign_record = json.load(fp)
         return sign_record
 
     async def login(self, num_of_dialogs=20):
         num_of_dialogs = int(
-            input(f"获取最近N个对话（默认{num_of_dialogs}）：") or num_of_dialogs
+            input(
+                f"获取最近N个对话（默认{num_of_dialogs}，请确保想要签到的对话在最近N个对话内）："
+            )
+            or num_of_dialogs
         )
         async with app:
             me = await app.get_me()
             self.set_me(me)
             latest_chats = []
             async for dialog in app.get_dialogs(num_of_dialogs):
                 chat = dialog.chat
@@ -204,15 +202,17 @@
                         "username": chat.username,
                         "first_name": chat.first_name,
                         "last_name": chat.last_name,
                     }
                 )
                 print(latest_chats[-1])
 
-            with open(self.base_dir.joinpath("latest_chats.json"), "w") as fp:
+            with open(
+                self.base_dir.joinpath("latest_chats.json"), "w", encoding="utf-8"
+            ) as fp:
                 json.dump(
                     latest_chats,
                     fp,
                     indent=4,
                     default=Object.default,
                     ensure_ascii=False,
                 )
@@ -239,15 +239,15 @@
             try:
                 async with app:
                     now = get_now()
                     logger.info(f"当前时间: {now}")
                     if str(now.date()) not in sign_record:
                         await self.sign(config.chat_id, config.sign_text)
                         sign_record[str(now.date())] = now.isoformat()
-                        with open(self.sign_record_file, "w") as fp:
+                        with open(self.sign_record_file, "w", encoding="utf-8") as fp:
                             json.dump(sign_record, fp)
 
                     next_run = (now + timedelta(days=1)).replace(
                         hour=sign_at.hour,
                         minute=sign_at.minute,
                         second=sign_at.second,
                         microsecond=sign_at.microsecond,
@@ -270,15 +270,15 @@
         sys.exit(1)
     command = sys.argv[1].strip().lower()
     signer = UserSigner()
     if command == "login":
         return await signer.login()
     elif command == "list":
         return signer.list()
-    name = input("签到任务名（e.g. mojie）：")
+    name = input("签到任务名（e.g. mojie）：") or "my_sign"
     signer.sign_name = name
     if command == "run":
         return await signer.run()
     elif command == "reconfig":
         return signer.reconfig()
     print(help_text)
     sys.exit(1)
```

### Comparing `tg_signer-0.1.2/tg_signer.egg-info/PKG-INFO` & `tg_signer-0.1.3/tg_signer.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: tg-signer
-Version: 0.1.2
+Version: 0.1.3
 Summary: Telegram signer
 Home-page: https://github.com/amchii/tg-signer
 Author: Amchii
 Author-email: finethankuandyou@gmail.com
 License: BSD 3-Clause License
 Project-URL: Source, https://github.com/amchii/tg-signer
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyrogram
-Requires-Dist: tgcrypto
+Provides-Extra: tgcrypto
+Requires-Dist: tgcrypto; extra == "tgcrypto"
 
 # Telegram Signer - Telegram每日自动签到
 
 ## Install
 ```
 pip install -U tg-signer
 ```
```

