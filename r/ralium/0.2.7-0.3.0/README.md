# Comparing `tmp/ralium-0.2.7.tar.gz` & `tmp/ralium-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ralium-0.2.7.tar", last modified: Thu May 16 15:28:10 2024, max compression
+gzip compressed data, was "ralium-0.3.0.tar", last modified: Thu May 16 17:45:32 2024, max compression
```

## Comparing `ralium-0.2.7.tar` & `ralium-0.3.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 15:28:10.001352 ralium-0.2.7/
--rw-rw-rw-   0        0        0    35823 2024-04-24 23:35:07.000000 ralium-0.2.7/LICENSE
--rw-rw-rw-   0        0        0    41876 2024-05-16 15:28:09.999773 ralium-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0       52 2024-04-24 23:35:07.000000 ralium-0.2.7/README.md
--rw-rw-rw-   0        0        0     1018 2024-05-16 15:25:54.000000 ralium-0.2.7/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-16 15:28:09.982814 ralium-0.2.7/ralium/
--rw-rw-rw-   0        0        0      185 2024-05-13 23:24:25.000000 ralium-0.2.7/ralium/__init__.py
--rw-rw-rw-   0        0        0     1816 2024-05-14 21:40:48.000000 ralium-0.2.7/ralium/_util.py
--rw-rw-rw-   0        0        0      634 2024-05-14 21:32:03.000000 ralium-0.2.7/ralium/_util.pyi
--rw-rw-rw-   0        0        0     6356 2024-05-14 21:39:34.000000 ralium-0.2.7/ralium/api.py
--rw-rw-rw-   0        0        0     1066 2024-05-13 23:23:35.000000 ralium-0.2.7/ralium/api.pyi
--rw-rw-rw-   0        0        0      680 2024-05-02 17:00:29.000000 ralium-0.2.7/ralium/builtins.py
--rw-rw-rw-   0        0        0      541 2024-05-13 23:23:27.000000 ralium-0.2.7/ralium/builtins.pyi
--rw-rw-rw-   0        0        0     3332 2024-05-13 22:21:52.000000 ralium-0.2.7/ralium/config.py
--rw-rw-rw-   0        0        0      467 2024-05-01 22:26:47.000000 ralium-0.2.7/ralium/config.pyi
--rw-rw-rw-   0        0        0     6194 2024-05-14 05:14:25.000000 ralium-0.2.7/ralium/element.py
--rw-rw-rw-   0        0        0     1376 2024-05-14 05:14:09.000000 ralium-0.2.7/ralium/element.pyi
--rw-rw-rw-   0        0        0     4401 2024-05-13 21:17:30.000000 ralium-0.2.7/ralium/engine.py
--rw-rw-rw-   0        0        0     1389 2024-05-13 23:23:13.000000 ralium-0.2.7/ralium/engine.pyi
--rw-rw-rw-   0        0        0     1040 2024-05-13 22:41:14.000000 ralium-0.2.7/ralium/errors.py
--rw-rw-rw-   0        0        0     2387 2024-05-16 15:25:16.000000 ralium-0.2.7/ralium/listener.py
--rw-rw-rw-   0        0        0      890 2024-05-16 14:59:59.000000 ralium-0.2.7/ralium/listener.pyi
--rw-rw-rw-   0        0        0      804 2024-05-14 21:31:14.000000 ralium-0.2.7/ralium/navigation.py
--rw-rw-rw-   0        0        0      376 2024-04-29 20:44:02.000000 ralium-0.2.7/ralium/navigation.pyi
--rw-rw-rw-   0        0        0     3952 2024-05-13 23:29:31.000000 ralium-0.2.7/ralium/setup.py
--rw-rw-rw-   0        0        0      559 2024-05-13 23:23:01.000000 ralium-0.2.7/ralium/setup.pyi
--rw-rw-rw-   0        0        0     5738 2024-05-14 21:32:26.000000 ralium-0.2.7/ralium/webpage.py
--rw-rw-rw-   0        0        0     1250 2024-05-13 23:22:49.000000 ralium-0.2.7/ralium/webpage.pyi
--rw-rw-rw-   0        0        0     5198 2024-05-15 21:49:35.000000 ralium-0.2.7/ralium/window.py
--rw-rw-rw-   0        0        0      613 2024-05-14 05:14:09.000000 ralium-0.2.7/ralium/window.pyi
-drwxrwxrwx   0        0        0        0 2024-05-16 15:28:09.998766 ralium-0.2.7/ralium.egg-info/
--rw-rw-rw-   0        0        0    41876 2024-05-16 15:28:09.000000 ralium-0.2.7/ralium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      612 2024-05-16 15:28:09.000000 ralium-0.2.7/ralium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 15:28:09.000000 ralium-0.2.7/ralium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-05-16 15:28:09.000000 ralium-0.2.7/ralium.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-16 15:28:09.000000 ralium-0.2.7/ralium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 15:28:10.001352 ralium-0.2.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-16 17:45:32.570947 ralium-0.3.0/
+-rw-rw-rw-   0        0        0    35823 2024-04-24 23:35:07.000000 ralium-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0    41876 2024-05-16 17:45:32.569326 ralium-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0       52 2024-04-24 23:35:07.000000 ralium-0.3.0/README.md
+-rw-rw-rw-   0        0        0     1018 2024-05-16 17:44:45.000000 ralium-0.3.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-16 17:45:32.550027 ralium-0.3.0/ralium/
+-rw-rw-rw-   0        0        0      185 2024-05-13 23:24:25.000000 ralium-0.3.0/ralium/__init__.py
+-rw-rw-rw-   0        0        0     1816 2024-05-14 21:40:48.000000 ralium-0.3.0/ralium/_util.py
+-rw-rw-rw-   0        0        0      634 2024-05-14 21:32:03.000000 ralium-0.3.0/ralium/_util.pyi
+-rw-rw-rw-   0        0        0     6356 2024-05-14 21:39:34.000000 ralium-0.3.0/ralium/api.py
+-rw-rw-rw-   0        0        0     1066 2024-05-13 23:23:35.000000 ralium-0.3.0/ralium/api.pyi
+-rw-rw-rw-   0        0        0      680 2024-05-02 17:00:29.000000 ralium-0.3.0/ralium/builtins.py
+-rw-rw-rw-   0        0        0      541 2024-05-13 23:23:27.000000 ralium-0.3.0/ralium/builtins.pyi
+-rw-rw-rw-   0        0        0     3332 2024-05-13 22:21:52.000000 ralium-0.3.0/ralium/config.py
+-rw-rw-rw-   0        0        0      467 2024-05-01 22:26:47.000000 ralium-0.3.0/ralium/config.pyi
+-rw-rw-rw-   0        0        0     6194 2024-05-14 05:14:25.000000 ralium-0.3.0/ralium/element.py
+-rw-rw-rw-   0        0        0     1376 2024-05-14 05:14:09.000000 ralium-0.3.0/ralium/element.pyi
+-rw-rw-rw-   0        0        0     4401 2024-05-13 21:17:30.000000 ralium-0.3.0/ralium/engine.py
+-rw-rw-rw-   0        0        0     1389 2024-05-13 23:23:13.000000 ralium-0.3.0/ralium/engine.pyi
+-rw-rw-rw-   0        0        0     1086 2024-05-16 17:41:03.000000 ralium-0.3.0/ralium/errors.py
+-rw-rw-rw-   0        0        0     2387 2024-05-16 15:25:16.000000 ralium-0.3.0/ralium/listener.py
+-rw-rw-rw-   0        0        0      890 2024-05-16 14:59:59.000000 ralium-0.3.0/ralium/listener.pyi
+-rw-rw-rw-   0        0        0      804 2024-05-14 21:31:14.000000 ralium-0.3.0/ralium/navigation.py
+-rw-rw-rw-   0        0        0      376 2024-04-29 20:44:02.000000 ralium-0.3.0/ralium/navigation.pyi
+-rw-rw-rw-   0        0        0     3952 2024-05-13 23:29:31.000000 ralium-0.3.0/ralium/setup.py
+-rw-rw-rw-   0        0        0      559 2024-05-13 23:23:01.000000 ralium-0.3.0/ralium/setup.pyi
+-rw-rw-rw-   0        0        0     5738 2024-05-14 21:32:26.000000 ralium-0.3.0/ralium/webpage.py
+-rw-rw-rw-   0        0        0     1250 2024-05-13 23:22:49.000000 ralium-0.3.0/ralium/webpage.pyi
+-rw-rw-rw-   0        0        0     6022 2024-05-16 17:41:38.000000 ralium-0.3.0/ralium/window.py
+-rw-rw-rw-   0        0        0      693 2024-05-16 17:42:01.000000 ralium-0.3.0/ralium/window.pyi
+drwxrwxrwx   0        0        0        0 2024-05-16 17:45:32.568313 ralium-0.3.0/ralium.egg-info/
+-rw-rw-rw-   0        0        0    41876 2024-05-16 17:45:32.000000 ralium-0.3.0/ralium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      612 2024-05-16 17:45:32.000000 ralium-0.3.0/ralium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 17:45:32.000000 ralium-0.3.0/ralium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-05-16 17:45:32.000000 ralium-0.3.0/ralium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-16 17:45:32.000000 ralium-0.3.0/ralium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 17:45:32.570947 ralium-0.3.0/setup.cfg
```

### Comparing `ralium-0.2.7/LICENSE` & `ralium-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ralium-0.2.7/PKG-INFO` & `ralium-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ralium
-Version: 0.2.7
+Version: 0.3.0
 Summary: An easy to use wrapper for pywebview.
 Author-email: Isaiah Coroama <coroamaisaiah@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ralium-0.2.7/pyproject.toml` & `ralium-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools >= 69.5.0", "wheel >= 0.43.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ralium"
-version = "0.2.7"
+version = "0.3.0"
 description = "An easy to use wrapper for pywebview."
 readme = "README.md"
 authors = [{ name = "Isaiah Coroama", email = "coroamaisaiah@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
```

### Comparing `ralium-0.2.7/ralium/_util.py` & `ralium-0.3.0/ralium/_util.py`

 * *Files identical despite different names*

### Comparing `ralium-0.2.7/ralium/_util.pyi` & `ralium-0.3.0/ralium/_util.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.2.7/ralium/api.py` & `ralium-0.3.0/ralium/api.py`

 * *Files identical despite different names*

### Comparing `ralium-0.2.7/ralium/api.pyi` & `ralium-0.3.0/ralium/api.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.2.7/ralium/builtins.py` & `ralium-0.3.0/ralium/builtins.py`

 * *Files identical despite different names*

### Comparing `ralium-0.2.7/ralium/builtins.pyi` & `ralium-0.3.0/ralium/builtins.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.2.7/ralium/config.py` & `ralium-0.3.0/ralium/config.py`

 * *Files identical despite different names*

### Comparing `ralium-0.2.7/ralium/element.py` & `ralium-0.3.0/ralium/element.py`

 * *Files identical despite different names*

### Comparing `ralium-0.2.7/ralium/element.pyi` & `ralium-0.3.0/ralium/element.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.2.7/ralium/engine.py` & `ralium-0.3.0/ralium/engine.py`

 * *Files identical despite different names*

### Comparing `ralium-0.2.7/ralium/engine.pyi` & `ralium-0.3.0/ralium/engine.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.2.7/ralium/errors.py` & `ralium-0.3.0/ralium/errors.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 global __RALIUM_WARNING_MESSAGES__
 __RALIUM_WARNING_MESSAGES__ = True
 
 class WindowLoadError(Exception): pass
 class BridgeEventError(Exception): pass
 class FilePathLimitError(Exception): pass
 class RegistryNotFoundError(Exception): pass
+class WindowNotRunningError(Exception): pass
 
 class WebFunctionApiError(Exception): pass
 class WebFolderNotFoundError(Exception): pass
 class WebRoutesNotFoundError(Exception): pass
 class WebFolderDirectoryError(Exception): pass
 class WebRoutesDirectoryError(Exception): pass
```

### Comparing `ralium-0.2.7/ralium/listener.py` & `ralium-0.3.0/ralium/listener.py`

 * *Files identical despite different names*

### Comparing `ralium-0.2.7/ralium/listener.pyi` & `ralium-0.3.0/ralium/listener.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.2.7/ralium/navigation.py` & `ralium-0.3.0/ralium/navigation.py`

 * *Files identical despite different names*

### Comparing `ralium-0.2.7/ralium/setup.py` & `ralium-0.3.0/ralium/setup.py`

 * *Files identical despite different names*

### Comparing `ralium-0.2.7/ralium/setup.pyi` & `ralium-0.3.0/ralium/setup.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.2.7/ralium/webpage.py` & `ralium-0.3.0/ralium/webpage.py`

 * *Files identical despite different names*

### Comparing `ralium-0.2.7/ralium/webpage.pyi` & `ralium-0.3.0/ralium/webpage.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.2.7/ralium/window.py` & `ralium-0.3.0/ralium/window.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from ralium.navigation import WindowNavigation
 from ralium.listener import ClassListener
 from ralium.webpage import WebHookDict, HTML_TEMPLATE
-from ralium.errors import WebHookHomepageError
 from ralium.config import WindowConfig
 from ralium.engine import WebEngine
 import ralium.builtins
 
+from ralium.errors import (
+    WebHookHomepageError, 
+    WindowNotRunningError
+)
+
 from ralium.element import (
     HTMLElement,
     create_element, 
     create_ralium_id, 
     RALIUM_ID_IDENTIFIER_PREFIX
 )
 
@@ -55,14 +59,31 @@
 
             webhook.set_window(self)
             webhook._wrap_functions()
             webhook._wrap_namespaces()
         
         self.engine.start()
     
+    def getElementsByClassName(self, className):
+        """
+        Gets all elements with a specific Class Name.
+
+        :param className: The HTML Class to look for.
+
+        :raises WindowNotRunningError: If you call this method before starting it, an error will be raised.
+
+        :returns: A list of `HTMLElement` Objects. Returns an empty list if no elements are found.
+        """
+
+        if not self.running:
+            raise WindowNotRunningError("Window must be running before calling the 'getElementsByClassName' method.")
+
+        element_classes = self.webview.evaluate_js(f"Array.from(document.getElementsByClassName('{className}')).map((e) => e.classList);")
+        return [HTMLElement(self, classList[0]) for classList in element_classes]
+    
     def getElementById(self, id):
         """
         Gets an element with a specific Id.
 
         :param id: The HTML element Id.
         
         :returns: `HTMLElement` Object if found or `None`.
```

### Comparing `ralium-0.2.7/ralium.egg-info/PKG-INFO` & `ralium-0.3.0/ralium.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ralium
-Version: 0.2.7
+Version: 0.3.0
 Summary: An easy to use wrapper for pywebview.
 Author-email: Isaiah Coroama <coroamaisaiah@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ralium-0.2.7/ralium.egg-info/SOURCES.txt` & `ralium-0.3.0/ralium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

