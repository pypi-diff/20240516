# Comparing `tmp/smdb_web_server-0.3.2.tar.gz` & `tmp/smdb_web_server-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smdb_web_server-0.3.2.tar", last modified: Sat Mar 30 20:53:03 2024, max compression
+gzip compressed data, was "smdb_web_server-0.3.3.tar", last modified: Thu May 16 14:30:52 2024, max compression
```

## Comparing `smdb_web_server-0.3.2.tar` & `smdb_web_server-0.3.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-03-30 20:53:03.848125 smdb_web_server-0.3.2/
--rw-rw-rw-   0        0        0     1086 2023-06-18 19:13:59.000000 smdb_web_server-0.3.2/LICENSE
--rw-rw-rw-   0        0        0     7131 2024-03-30 20:53:03.847601 smdb_web_server-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     6568 2024-03-14 18:44:00.000000 smdb_web_server-0.3.2/README.md
--rw-rw-rw-   0        0        0      128 2023-07-04 05:55:03.000000 smdb_web_server-0.3.2/pyproject.toml
--rw-rw-rw-   0        0        0      627 2024-03-30 20:53:03.849675 smdb_web_server-0.3.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-30 20:53:03.833583 smdb_web_server-0.3.2/smdb_web_server/
--rw-rw-rw-   0        0        0    13233 2024-03-30 20:52:16.000000 smdb_web_server-0.3.2/smdb_web_server/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-30 20:53:03.846557 smdb_web_server-0.3.2/smdb_web_server.egg-info/
--rw-rw-rw-   0        0        0     7131 2024-03-30 20:53:03.000000 smdb_web_server-0.3.2/smdb_web_server.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2024-03-30 20:53:03.000000 smdb_web_server-0.3.2/smdb_web_server.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-30 20:53:03.000000 smdb_web_server-0.3.2/smdb_web_server.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-03-30 20:53:03.000000 smdb_web_server-0.3.2/smdb_web_server.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 14:30:52.384110 smdb_web_server-0.3.3/
+-rw-rw-rw-   0        0        0     1086 2023-06-18 19:13:59.000000 smdb_web_server-0.3.3/LICENSE
+-rw-rw-rw-   0        0        0     7317 2024-05-16 14:30:52.383595 smdb_web_server-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6754 2024-05-16 14:30:31.000000 smdb_web_server-0.3.3/README.md
+-rw-rw-rw-   0        0        0      128 2023-07-04 05:55:03.000000 smdb_web_server-0.3.3/pyproject.toml
+-rw-rw-rw-   0        0        0      627 2024-05-16 14:30:52.385661 smdb_web_server-0.3.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-16 14:30:52.338579 smdb_web_server-0.3.3/smdb_web_server/
+-rw-rw-rw-   0        0        0    13457 2024-05-16 14:28:38.000000 smdb_web_server-0.3.3/smdb_web_server/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 14:30:52.383077 smdb_web_server-0.3.3/smdb_web_server.egg-info/
+-rw-rw-rw-   0        0        0     7317 2024-05-16 14:30:52.000000 smdb_web_server-0.3.3/smdb_web_server.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2024-05-16 14:30:52.000000 smdb_web_server-0.3.3/smdb_web_server.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 14:30:52.000000 smdb_web_server-0.3.3/smdb_web_server.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-16 14:30:52.000000 smdb_web_server-0.3.3/smdb_web_server.egg-info/top_level.txt
```

### Comparing `smdb_web_server-0.3.2/LICENSE` & `smdb_web_server-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `smdb_web_server-0.3.2/PKG-INFO` & `smdb_web_server-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smdb_web_server
-Version: 0.3.2
+Version: 0.3.3
 Summary: A really basic, not so safe web server.
 Home-page: https://github.com/NightKey/smdb-server
 Author: Janthó Dávid
 Author-email: davidjantho@gmail.com
 Project-URL: Bug Tracker, https://github.com/NightKey/smdb-server/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -176,9 +176,9 @@
 Values: `Get`, `Put`
 
 ### UrlData
 
 This dataclass contains the following fields, either filled or containing `None`:
 
  - fragment: `String` object (Data following the `#` in the URL)
- - query: `Dictionary` with string keys and values (Data following the `?` in the URL)
+ - query: `Dictionary` with string keys and values (Data following the `?` in the URL). The key will be the part following the `?` or `&` characters, and the value will be the part after the `=` sign. If there is no value, `None` will be used as a value in the dictionary.
  - data: `Bytes` object (Payload of the request, if available)
```

### Comparing `smdb_web_server-0.3.2/README.md` & `smdb_web_server-0.3.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -160,9 +160,9 @@
 Values: `Get`, `Put`
 
 ### UrlData
 
 This dataclass contains the following fields, either filled or containing `None`:
 
  - fragment: `String` object (Data following the `#` in the URL)
- - query: `Dictionary` with string keys and values (Data following the `?` in the URL)
+ - query: `Dictionary` with string keys and values (Data following the `?` in the URL). The key will be the part following the `?` or `&` characters, and the value will be the part after the `=` sign. If there is no value, `None` will be used as a value in the dictionary.
  - data: `Bytes` object (Payload of the request, if available)
```

### Comparing `smdb_web_server-0.3.2/setup.cfg` & `smdb_web_server-0.3.3/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 6d64 625f 7765 625f 7365 7276   = smdb_web_serv
 00000020: 6572 0d0a 7665 7273 696f 6e20 3d20 302e  er..version = 0.
-00000030: 332e 320d 0a61 7574 686f 7220 3d20 4a61  3.2..author = Ja
+00000030: 332e 330d 0a61 7574 686f 7220 3d20 4a61  3.3..author = Ja
 00000040: 6e74 68c3 b320 44c3 a176 6964 0d0a 6175  nth.. D..vid..au
 00000050: 7468 6f72 5f65 6d61 696c 203d 2064 6176  thor_email = dav
 00000060: 6964 6a61 6e74 686f 4067 6d61 696c 2e63  idjantho@gmail.c
 00000070: 6f6d 0d0a 6465 7363 7269 7074 696f 6e20  om..description 
 00000080: 3d20 4120 7265 616c 6c79 2062 6173 6963  = A really basic
 00000090: 2c20 6e6f 7420 736f 2073 6166 6520 7765  , not so safe we
 000000a0: 6220 7365 7276 6572 2e0d 0a6c 6f6e 675f  b server...long_
```

### Comparing `smdb_web_server-0.3.2/smdb_web_server/__init__.py` & `smdb_web_server-0.3.3/smdb_web_server/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
             fragment = None
             if (len(tmp_path) > 1):
                 fragment = tmp_path[-1]
             tmp_path = tmp_path[0]
             tmp_path = tmp_path.split("?")
             query = None
             if (len(tmp_path) > 1):
-                query = {item.split("=")[0]: item.split("=")[1] for item in tmp_path[-1].split("&") if len(item.split("=")) == 2}
+                query = self.getQueryItems(tmp_path[-1])
             self.path = tmp_path[0]
             self.headers = {head.split(": ")[0]: head.split(": ")[1] for head in tmp[1:] if head != ''}
             if (self.logger):
                 self.logger.debug(f"Headers retrived: {self.headers}")
             data = None
             if ("Content-Length" in self.headers):
                 data = await self.reader.read(int(self.headers["Content-Length"]))
@@ -110,14 +110,23 @@
             self.close_event.set()
         except Exception as ex :
             self.logger.error(f"Exception: {ex}")
             html_file = html_template.format(title=pageTitle, content=ex)
             response_code = InternalServerError
             self.send_message(response_code, html_file)
 
+    def getQueryItems(self, items: str) -> Dict[str, Any]:
+        ret = {}
+        for item in items.split("&"):
+            if len(item.split("=")) == 2:
+                ret[item.split("=")[0]] = item.split("=")[1]
+            else:
+                ret[item] = None
+        return ret
+
     def __404__(self, do_get: Timer) -> None:
         if (self.logger):
             self.logger.debug("Sending 404 page.")
         _404_time = Timer()
         _404_file = ""
         if ("404" in TEMPLATES):
             _404_file = TEMPLATES["404"].format(title=pageTitle)
```

### Comparing `smdb_web_server-0.3.2/smdb_web_server.egg-info/PKG-INFO` & `smdb_web_server-0.3.3/smdb_web_server.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smdb_web_server
-Version: 0.3.2
+Version: 0.3.3
 Summary: A really basic, not so safe web server.
 Home-page: https://github.com/NightKey/smdb-server
 Author: Janthó Dávid
 Author-email: davidjantho@gmail.com
 Project-URL: Bug Tracker, https://github.com/NightKey/smdb-server/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -176,9 +176,9 @@
 Values: `Get`, `Put`
 
 ### UrlData
 
 This dataclass contains the following fields, either filled or containing `None`:
 
  - fragment: `String` object (Data following the `#` in the URL)
- - query: `Dictionary` with string keys and values (Data following the `?` in the URL)
+ - query: `Dictionary` with string keys and values (Data following the `?` in the URL). The key will be the part following the `?` or `&` characters, and the value will be the part after the `=` sign. If there is no value, `None` will be used as a value in the dictionary.
  - data: `Bytes` object (Payload of the request, if available)
```

