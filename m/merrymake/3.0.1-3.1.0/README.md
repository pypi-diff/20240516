# Comparing `tmp/merrymake-3.0.1.tar.gz` & `tmp/merrymake-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merrymake-3.0.1.tar", max compression
+gzip compressed data, was "merrymake-3.1.0.tar", max compression
```

## Comparing `merrymake-3.0.1.tar` & `merrymake-3.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      930 2024-02-16 16:29:03.616348 merrymake-3.0.1/README.md
--rw-r--r--   0        0        0      229 2023-10-12 10:23:09.487463 merrymake-3.0.1/merrymake/__init__.py
--rw-r--r--   0        0        0      129 2024-02-16 16:25:47.738906 merrymake-3.0.1/merrymake/envelope.py
--rw-r--r--   0        0        0      887 2024-02-16 16:25:47.738906 merrymake-3.0.1/merrymake/imerrymake.py
--rw-r--r--   0        0        0     5122 2024-02-16 16:25:47.738906 merrymake-3.0.1/merrymake/merrymake.py
--rw-r--r--   0        0        0     4712 2024-02-16 16:25:47.738906 merrymake-3.0.1/merrymake/merrymimetypes.py
--rw-r--r--   0        0        0      183 2023-11-21 15:12:20.039750 merrymake-3.0.1/merrymake/nullmerrymake.py
--rw-r--r--   0        0        0      191 2023-11-21 15:12:20.049750 merrymake-3.0.1/merrymake/streamhelper.py
--rw-r--r--   0        0        0      456 2024-02-16 16:29:03.616348 merrymake-3.0.1/pyproject.toml
--rw-r--r--   0        0        0     1300 1970-01-01 00:00:00.000000 merrymake-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0      899 2024-02-23 09:46:31.847480 merrymake-3.1.0/README.md
+-rw-r--r--   0        0        0      229 2023-10-12 10:23:09.487463 merrymake-3.1.0/merrymake/__init__.py
+-rw-r--r--   0        0        0      142 2024-02-23 09:46:31.847480 merrymake-3.1.0/merrymake/envelope.py
+-rw-r--r--   0        0        0      887 2024-02-16 16:25:47.738906 merrymake-3.1.0/merrymake/imerrymake.py
+-rw-r--r--   0        0        0     5087 2024-02-23 09:46:31.847480 merrymake-3.1.0/merrymake/merrymake.py
+-rw-r--r--   0        0        0     6959 2024-02-23 09:46:31.847480 merrymake-3.1.0/merrymake/merrymimetypes.py
+-rw-r--r--   0        0        0      183 2023-11-21 15:12:20.039750 merrymake-3.1.0/merrymake/nullmerrymake.py
+-rw-r--r--   0        0        0      191 2023-11-21 15:12:20.049750 merrymake-3.1.0/merrymake/streamhelper.py
+-rw-r--r--   0        0        0      456 2024-02-23 09:46:31.847480 merrymake-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1269 1970-01-01 00:00:00.000000 merrymake-3.1.0/PKG-INFO
```

### Comparing `merrymake-3.0.1/README.md` & `merrymake-3.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -3,27 +3,25 @@
 This is the official Python service library for Merrymake. It defines all the basic functions needed to work with Merrymake.
 
 ## Usage
 
 Here is the most basic example of how to use this library:
 
 ```python
-import sys
-
 from merrymake import Merrymake
 from merrymake.merrymimetypes import MerryMimetypes
 from merrymake.envelope import Envelope
 
 def handle_hello(payloadBytes: bytearray, envelope: Envelope):
     payload = bytes(payloadBytes).decode('utf-8')
-    Merrymake.reply_to_origin(f"Hello, {payload}!", MerryMimetypes.get_mime_type("txt"));
+    Merrymake.reply_to_origin(f"Hello, {payload}!", MerryMimetypes.txt)
 
 def main():
     (Merrymake.service()
-        .handle("handle_hello", handle_hello));
+        .handle("handle_hello", handle_hello))
 
 if __name__ == "__main__":
     main()
 ```
 
 ## Tutorials and templates
```

### Comparing `merrymake-3.0.1/merrymake/imerrymake.py` & `merrymake-3.1.0/merrymake/imerrymake.py`

 * *Files identical despite different names*

### Comparing `merrymake-3.0.1/merrymake/merrymake.py` & `merrymake-3.1.0/merrymake/merrymake.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         args = sys.argv[1:]
         return Merrymake(args)
 
     def __init__(self, args):
 
         try:
             self.action = args[-2]
-            buf = json.loads(args[-1]);
+            buf = json.loads(args[-1])
             self.envelope = Envelope(buf.get("messageId"), buf.get("traceId"), buf.get("sessionId"))
             self.payloadBytes = read_to_end(sys.stdin.buffer)
         except ValueError:  # includes simplejson.decoder.JSONDecodeError
             print('Decoding JSON has failed')
             raise Exception("Decoding JSON has failed")
         except:
             print("Could not read from stdin")
@@ -145,15 +145,15 @@
 
         Parameters
         ----------
         channel : string
             The channel to join
         """
 
-        Merrymake.post_to_rapids("$join", channel, MerryMimetypes.get_mime_type("txt"))
+        Merrymake.post_to_rapids("$join", channel, MerryMimetypes.txt)
 
     @staticmethod
     def broadcast_to_channel(to: str, event: str, payload: str):
         """Broadcast a message (event and payload) to all listeners in a channel.
 
         Parameters
         ----------
@@ -161,8 +161,8 @@
             The channel to broadcast to
         event : string
             The event-type of the message
         payload : string
             The payload of the message
         """
 
-        Merrymake.post_to_rapids("$broadcast", json.dumps({"to": to, "event": event, "payload": payload}), MerryMimetypes.get_mime_type("json"))
+        Merrymake.post_to_rapids("$broadcast", json.dumps({"to": to, "event": event, "payload": payload}), MerryMimetypes.json)
```

### Comparing `merrymake-3.0.1/PKG-INFO` & `merrymake-3.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merrymake
-Version: 3.0.1
+Version: 3.1.0
 Summary: Service library for the Merrymake platform
 Author: Nicolaj Græsholt
 Author-email: ng@merrymake.eu
 Requires-Python: >=3.11.2,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: requests (==2.31.0)
@@ -15,27 +15,25 @@
 This is the official Python service library for Merrymake. It defines all the basic functions needed to work with Merrymake.
 
 ## Usage
 
 Here is the most basic example of how to use this library:
 
 ```python
-import sys
-
 from merrymake import Merrymake
 from merrymake.merrymimetypes import MerryMimetypes
 from merrymake.envelope import Envelope
 
 def handle_hello(payloadBytes: bytearray, envelope: Envelope):
     payload = bytes(payloadBytes).decode('utf-8')
-    Merrymake.reply_to_origin(f"Hello, {payload}!", MerryMimetypes.get_mime_type("txt"));
+    Merrymake.reply_to_origin(f"Hello, {payload}!", MerryMimetypes.txt)
 
 def main():
     (Merrymake.service()
-        .handle("handle_hello", handle_hello));
+        .handle("handle_hello", handle_hello))
 
 if __name__ == "__main__":
     main()
 ```
 
 ## Tutorials and templates
```

