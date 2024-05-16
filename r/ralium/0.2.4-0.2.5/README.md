# Comparing `tmp/ralium-0.2.4.tar.gz` & `tmp/ralium-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ralium-0.2.4.tar", last modified: Wed May 15 21:53:09 2024, max compression
+gzip compressed data, was "ralium-0.2.5.tar", last modified: Thu May 16 15:01:57 2024, max compression
```

## Comparing `ralium-0.2.4.tar` & `ralium-0.2.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 21:53:09.214575 ralium-0.2.4/
--rw-rw-rw-   0        0        0    35823 2024-04-24 23:35:07.000000 ralium-0.2.4/LICENSE
--rw-rw-rw-   0        0        0    41876 2024-05-15 21:53:09.212387 ralium-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0       52 2024-04-24 23:35:07.000000 ralium-0.2.4/README.md
--rw-rw-rw-   0        0        0     1018 2024-05-15 21:52:12.000000 ralium-0.2.4/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-15 21:53:09.177616 ralium-0.2.4/ralium/
--rw-rw-rw-   0        0        0      185 2024-05-13 23:24:25.000000 ralium-0.2.4/ralium/__init__.py
--rw-rw-rw-   0        0        0     1816 2024-05-14 21:40:48.000000 ralium-0.2.4/ralium/_util.py
--rw-rw-rw-   0        0        0      634 2024-05-14 21:32:03.000000 ralium-0.2.4/ralium/_util.pyi
--rw-rw-rw-   0        0        0     6356 2024-05-14 21:39:34.000000 ralium-0.2.4/ralium/api.py
--rw-rw-rw-   0        0        0     1066 2024-05-13 23:23:35.000000 ralium-0.2.4/ralium/api.pyi
--rw-rw-rw-   0        0        0      680 2024-05-02 17:00:29.000000 ralium-0.2.4/ralium/builtins.py
--rw-rw-rw-   0        0        0      541 2024-05-13 23:23:27.000000 ralium-0.2.4/ralium/builtins.pyi
--rw-rw-rw-   0        0        0     3332 2024-05-13 22:21:52.000000 ralium-0.2.4/ralium/config.py
--rw-rw-rw-   0        0        0      467 2024-05-01 22:26:47.000000 ralium-0.2.4/ralium/config.pyi
--rw-rw-rw-   0        0        0     6194 2024-05-14 05:14:25.000000 ralium-0.2.4/ralium/element.py
--rw-rw-rw-   0        0        0     1376 2024-05-14 05:14:09.000000 ralium-0.2.4/ralium/element.pyi
--rw-rw-rw-   0        0        0     4401 2024-05-13 21:17:30.000000 ralium-0.2.4/ralium/engine.py
--rw-rw-rw-   0        0        0     1389 2024-05-13 23:23:13.000000 ralium-0.2.4/ralium/engine.pyi
--rw-rw-rw-   0        0        0     1040 2024-05-13 22:41:14.000000 ralium-0.2.4/ralium/errors.py
--rw-rw-rw-   0        0        0     2142 2024-05-15 21:45:00.000000 ralium-0.2.4/ralium/listener.py
--rw-rw-rw-   0        0        0      772 2024-05-15 21:48:01.000000 ralium-0.2.4/ralium/listener.pyi
--rw-rw-rw-   0        0        0      804 2024-05-14 21:31:14.000000 ralium-0.2.4/ralium/navigation.py
--rw-rw-rw-   0        0        0      376 2024-04-29 20:44:02.000000 ralium-0.2.4/ralium/navigation.pyi
--rw-rw-rw-   0        0        0     3952 2024-05-13 23:29:31.000000 ralium-0.2.4/ralium/setup.py
--rw-rw-rw-   0        0        0      559 2024-05-13 23:23:01.000000 ralium-0.2.4/ralium/setup.pyi
--rw-rw-rw-   0        0        0     5738 2024-05-14 21:32:26.000000 ralium-0.2.4/ralium/webpage.py
--rw-rw-rw-   0        0        0     1250 2024-05-13 23:22:49.000000 ralium-0.2.4/ralium/webpage.pyi
--rw-rw-rw-   0        0        0     5198 2024-05-15 21:49:35.000000 ralium-0.2.4/ralium/window.py
--rw-rw-rw-   0        0        0      613 2024-05-14 05:14:09.000000 ralium-0.2.4/ralium/window.pyi
-drwxrwxrwx   0        0        0        0 2024-05-15 21:53:09.210952 ralium-0.2.4/ralium.egg-info/
--rw-rw-rw-   0        0        0    41876 2024-05-15 21:53:09.000000 ralium-0.2.4/ralium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      612 2024-05-15 21:53:09.000000 ralium-0.2.4/ralium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 21:53:09.000000 ralium-0.2.4/ralium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-05-15 21:53:09.000000 ralium-0.2.4/ralium.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-15 21:53:09.000000 ralium-0.2.4/ralium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 21:53:09.214575 ralium-0.2.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-16 15:01:57.501863 ralium-0.2.5/
+-rw-rw-rw-   0        0        0    35823 2024-04-24 23:35:07.000000 ralium-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0    41876 2024-05-16 15:01:57.498804 ralium-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0       52 2024-04-24 23:35:07.000000 ralium-0.2.5/README.md
+-rw-rw-rw-   0        0        0     1018 2024-05-16 15:01:14.000000 ralium-0.2.5/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-16 15:01:57.480457 ralium-0.2.5/ralium/
+-rw-rw-rw-   0        0        0      185 2024-05-13 23:24:25.000000 ralium-0.2.5/ralium/__init__.py
+-rw-rw-rw-   0        0        0     1816 2024-05-14 21:40:48.000000 ralium-0.2.5/ralium/_util.py
+-rw-rw-rw-   0        0        0      634 2024-05-14 21:32:03.000000 ralium-0.2.5/ralium/_util.pyi
+-rw-rw-rw-   0        0        0     6356 2024-05-14 21:39:34.000000 ralium-0.2.5/ralium/api.py
+-rw-rw-rw-   0        0        0     1066 2024-05-13 23:23:35.000000 ralium-0.2.5/ralium/api.pyi
+-rw-rw-rw-   0        0        0      680 2024-05-02 17:00:29.000000 ralium-0.2.5/ralium/builtins.py
+-rw-rw-rw-   0        0        0      541 2024-05-13 23:23:27.000000 ralium-0.2.5/ralium/builtins.pyi
+-rw-rw-rw-   0        0        0     3332 2024-05-13 22:21:52.000000 ralium-0.2.5/ralium/config.py
+-rw-rw-rw-   0        0        0      467 2024-05-01 22:26:47.000000 ralium-0.2.5/ralium/config.pyi
+-rw-rw-rw-   0        0        0     6194 2024-05-14 05:14:25.000000 ralium-0.2.5/ralium/element.py
+-rw-rw-rw-   0        0        0     1376 2024-05-14 05:14:09.000000 ralium-0.2.5/ralium/element.pyi
+-rw-rw-rw-   0        0        0     4401 2024-05-13 21:17:30.000000 ralium-0.2.5/ralium/engine.py
+-rw-rw-rw-   0        0        0     1389 2024-05-13 23:23:13.000000 ralium-0.2.5/ralium/engine.pyi
+-rw-rw-rw-   0        0        0     1040 2024-05-13 22:41:14.000000 ralium-0.2.5/ralium/errors.py
+-rw-rw-rw-   0        0        0     2365 2024-05-16 14:59:48.000000 ralium-0.2.5/ralium/listener.py
+-rw-rw-rw-   0        0        0      890 2024-05-16 14:59:59.000000 ralium-0.2.5/ralium/listener.pyi
+-rw-rw-rw-   0        0        0      804 2024-05-14 21:31:14.000000 ralium-0.2.5/ralium/navigation.py
+-rw-rw-rw-   0        0        0      376 2024-04-29 20:44:02.000000 ralium-0.2.5/ralium/navigation.pyi
+-rw-rw-rw-   0        0        0     3952 2024-05-13 23:29:31.000000 ralium-0.2.5/ralium/setup.py
+-rw-rw-rw-   0        0        0      559 2024-05-13 23:23:01.000000 ralium-0.2.5/ralium/setup.pyi
+-rw-rw-rw-   0        0        0     5738 2024-05-14 21:32:26.000000 ralium-0.2.5/ralium/webpage.py
+-rw-rw-rw-   0        0        0     1250 2024-05-13 23:22:49.000000 ralium-0.2.5/ralium/webpage.pyi
+-rw-rw-rw-   0        0        0     5198 2024-05-15 21:49:35.000000 ralium-0.2.5/ralium/window.py
+-rw-rw-rw-   0        0        0      613 2024-05-14 05:14:09.000000 ralium-0.2.5/ralium/window.pyi
+drwxrwxrwx   0        0        0        0 2024-05-16 15:01:57.498804 ralium-0.2.5/ralium.egg-info/
+-rw-rw-rw-   0        0        0    41876 2024-05-16 15:01:57.000000 ralium-0.2.5/ralium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      612 2024-05-16 15:01:57.000000 ralium-0.2.5/ralium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 15:01:57.000000 ralium-0.2.5/ralium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-05-16 15:01:57.000000 ralium-0.2.5/ralium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-16 15:01:57.000000 ralium-0.2.5/ralium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 15:01:57.501863 ralium-0.2.5/setup.cfg
```

### Comparing `ralium-0.2.4/LICENSE` & `ralium-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ralium-0.2.4/PKG-INFO` & `ralium-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ralium
-Version: 0.2.4
+Version: 0.2.5
 Summary: An easy to use wrapper for pywebview.
 Author-email: Isaiah Coroama <coroamaisaiah@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ralium-0.2.4/pyproject.toml` & `ralium-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools >= 69.5.0", "wheel >= 0.43.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ralium"
-version = "0.2.4"
+version = "0.2.5"
 description = "An easy to use wrapper for pywebview."
 readme = "README.md"
 authors = [{ name = "Isaiah Coroama", email = "coroamaisaiah@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
```

### Comparing `ralium-0.2.4/ralium/_util.py` & `ralium-0.2.5/ralium/_util.py`

 * *Files identical despite different names*

### Comparing `ralium-0.2.4/ralium/_util.pyi` & `ralium-0.2.5/ralium/_util.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.2.4/ralium/api.py` & `ralium-0.2.5/ralium/api.py`

 * *Files identical despite different names*

### Comparing `ralium-0.2.4/ralium/api.pyi` & `ralium-0.2.5/ralium/api.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.2.4/ralium/builtins.py` & `ralium-0.2.5/ralium/builtins.py`

 * *Files identical despite different names*

### Comparing `ralium-0.2.4/ralium/builtins.pyi` & `ralium-0.2.5/ralium/builtins.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.2.4/ralium/config.py` & `ralium-0.2.5/ralium/config.py`

 * *Files identical despite different names*

### Comparing `ralium-0.2.4/ralium/element.py` & `ralium-0.2.5/ralium/element.py`

 * *Files identical despite different names*

### Comparing `ralium-0.2.4/ralium/element.pyi` & `ralium-0.2.5/ralium/element.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.2.4/ralium/engine.py` & `ralium-0.2.5/ralium/engine.py`

 * *Files identical despite different names*

### Comparing `ralium-0.2.4/ralium/engine.pyi` & `ralium-0.2.5/ralium/engine.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.2.4/ralium/errors.py` & `ralium-0.2.5/ralium/errors.py`

 * *Files identical despite different names*

### Comparing `ralium-0.2.4/ralium/listener.pyi` & `ralium-0.2.5/ralium/listener.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-from ralium._util import Self, FunctionType, ClassType, Any
-
-class SubscriptionService:
-    def __init__(self) -> None: ...
-    def subscribe(self, function: FunctionType, after: bool = False) -> None: ...
-    def unsubscribe(self, function: FunctionType, after: bool = False) -> None: ...
+from ralium._util import FunctionType, ClassType, Any
 
 class FunctionCallInfo:
     def __init__(self, 
         cls: ClassType, 
         function: FunctionType, 
         result: Any | None = None, 
         *args: tuple[Any], 
         **kwargs: dict[str, Any]
     ) -> None: ...
+    def __repr__(self) -> str: ...
 
 class ClassListener:
+    class BroadcastFunction:
+        def __init__(self) -> None: ...
+        def __call__(self, *args, **kwargs) -> ClassType: ...
+        def subscribe(self, function: FunctionType, is_after: bool = False) -> None: ...
+        def unsubscribe(self, function: FunctionType, is_after: bool = False) -> None: ...
+
     def __init__(self, cls: ClassType) -> None: ...
     def __call__(self, *args: tuple[Any], **kwargs: dict[str, Any]) -> ClassType: ...
     
-    def listen(this: Self, name: str, function: FunctionType) -> None: ...
+    def create_listener(self, function: FunctionType) -> BroadcastFunction: ...
```

### Comparing `ralium-0.2.4/ralium/navigation.py` & `ralium-0.2.5/ralium/navigation.py`

 * *Files identical despite different names*

### Comparing `ralium-0.2.4/ralium/setup.py` & `ralium-0.2.5/ralium/setup.py`

 * *Files identical despite different names*

### Comparing `ralium-0.2.4/ralium/setup.pyi` & `ralium-0.2.5/ralium/setup.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.2.4/ralium/webpage.py` & `ralium-0.2.5/ralium/webpage.py`

 * *Files identical despite different names*

### Comparing `ralium-0.2.4/ralium/webpage.pyi` & `ralium-0.2.5/ralium/webpage.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.2.4/ralium/window.py` & `ralium-0.2.5/ralium/window.py`

 * *Files identical despite different names*

### Comparing `ralium-0.2.4/ralium/window.pyi` & `ralium-0.2.5/ralium/window.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.2.4/ralium.egg-info/PKG-INFO` & `ralium-0.2.5/ralium.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ralium
-Version: 0.2.4
+Version: 0.2.5
 Summary: An easy to use wrapper for pywebview.
 Author-email: Isaiah Coroama <coroamaisaiah@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ralium-0.2.4/ralium.egg-info/SOURCES.txt` & `ralium-0.2.5/ralium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

