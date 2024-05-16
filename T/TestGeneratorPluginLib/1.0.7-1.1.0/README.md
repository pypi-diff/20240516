# Comparing `tmp/TestGeneratorPluginLib-1.0.7.tar.gz` & `tmp/TestGeneratorPluginLib-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TestGeneratorPluginLib-1.0.7.tar", last modified: Wed May 15 15:35:07 2024, max compression
+gzip compressed data, was "TestGeneratorPluginLib-1.1.0.tar", last modified: Thu May 16 12:31:35 2024, max compression
```

## Comparing `TestGeneratorPluginLib-1.0.7.tar` & `TestGeneratorPluginLib-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 15:35:07.142835 TestGeneratorPluginLib-1.0.7/
--rw-rw-rw-   0        0        0     1090 2024-05-15 15:34:08.000000 TestGeneratorPluginLib-1.0.7/LICENSE
--rw-rw-rw-   0        0        0     1569 2024-05-15 15:35:07.142835 TestGeneratorPluginLib-1.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-15 15:35:07.142835 TestGeneratorPluginLib-1.0.7/TestGeneratorPluginLib/
--rw-rw-rw-   0        0        0      288 2024-05-15 15:34:08.000000 TestGeneratorPluginLib-1.0.7/TestGeneratorPluginLib/__init__.py
--rw-rw-rw-   0        0        0     1707 2024-05-15 15:34:08.000000 TestGeneratorPluginLib-1.0.7/TestGeneratorPluginLib/_built_plugin.py
--rw-rw-rw-   0        0        0       19 2024-05-15 15:34:08.000000 TestGeneratorPluginLib-1.0.7/TestGeneratorPluginLib/_config.py
--rw-rw-rw-   0        0        0     1780 2024-05-15 15:34:08.000000 TestGeneratorPluginLib-1.0.7/TestGeneratorPluginLib/_language.py
--rw-rw-rw-   0        0        0     1219 2024-05-15 15:34:08.000000 TestGeneratorPluginLib-1.0.7/TestGeneratorPluginLib/_managers.py
--rw-rw-rw-   0        0        0     3227 2024-05-15 15:34:08.000000 TestGeneratorPluginLib-1.0.7/TestGeneratorPluginLib/_plugin.py
--rw-rw-rw-   0        0        0     3344 2024-05-15 15:34:08.000000 TestGeneratorPluginLib-1.0.7/TestGeneratorPluginLib/_widgets.py
-drwxrwxrwx   0        0        0        0 2024-05-15 15:35:07.142835 TestGeneratorPluginLib-1.0.7/TestGeneratorPluginLib.egg-info/
--rw-rw-rw-   0        0        0     1569 2024-05-15 15:35:07.000000 TestGeneratorPluginLib-1.0.7/TestGeneratorPluginLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      495 2024-05-15 15:35:07.000000 TestGeneratorPluginLib-1.0.7/TestGeneratorPluginLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 15:35:07.000000 TestGeneratorPluginLib-1.0.7/TestGeneratorPluginLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-15 15:35:07.000000 TestGeneratorPluginLib-1.0.7/TestGeneratorPluginLib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-05-15 15:35:07.000000 TestGeneratorPluginLib-1.0.7/TestGeneratorPluginLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 15:35:07.142835 TestGeneratorPluginLib-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1288 2024-05-15 15:34:08.000000 TestGeneratorPluginLib-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:31:35.612756 TestGeneratorPluginLib-1.1.0/
+-rw-rw-rw-   0        0        0     1090 2024-05-16 12:30:30.000000 TestGeneratorPluginLib-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1569 2024-05-16 12:31:35.612756 TestGeneratorPluginLib-1.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-16 12:31:35.612756 TestGeneratorPluginLib-1.1.0/TestGeneratorPluginLib/
+-rw-rw-rw-   0        0        0      350 2024-05-16 12:30:30.000000 TestGeneratorPluginLib-1.1.0/TestGeneratorPluginLib/__init__.py
+-rw-rw-rw-   0        0        0     2357 2024-05-16 12:30:30.000000 TestGeneratorPluginLib-1.1.0/TestGeneratorPluginLib/_built_plugin.py
+-rw-rw-rw-   0        0        0       19 2024-05-16 12:30:30.000000 TestGeneratorPluginLib-1.1.0/TestGeneratorPluginLib/_config.py
+-rw-rw-rw-   0        0        0     1780 2024-05-16 12:30:30.000000 TestGeneratorPluginLib-1.1.0/TestGeneratorPluginLib/_language.py
+-rw-rw-rw-   0        0        0     1219 2024-05-16 12:30:30.000000 TestGeneratorPluginLib-1.1.0/TestGeneratorPluginLib/_managers.py
+-rw-rw-rw-   0        0        0      533 2024-05-16 12:30:30.000000 TestGeneratorPluginLib-1.1.0/TestGeneratorPluginLib/_plugin.py
+-rw-rw-rw-   0        0        0     2834 2024-05-16 12:30:30.000000 TestGeneratorPluginLib-1.1.0/TestGeneratorPluginLib/_plugin_setup.py
+-rw-rw-rw-   0        0        0     3344 2024-05-16 12:30:30.000000 TestGeneratorPluginLib-1.1.0/TestGeneratorPluginLib/_widgets.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:31:35.612756 TestGeneratorPluginLib-1.1.0/TestGeneratorPluginLib.egg-info/
+-rw-rw-rw-   0        0        0     1569 2024-05-16 12:31:35.000000 TestGeneratorPluginLib-1.1.0/TestGeneratorPluginLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      535 2024-05-16 12:31:35.000000 TestGeneratorPluginLib-1.1.0/TestGeneratorPluginLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 12:31:35.000000 TestGeneratorPluginLib-1.1.0/TestGeneratorPluginLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-16 12:31:35.000000 TestGeneratorPluginLib-1.1.0/TestGeneratorPluginLib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-05-16 12:31:35.000000 TestGeneratorPluginLib-1.1.0/TestGeneratorPluginLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 12:31:35.612756 TestGeneratorPluginLib-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1288 2024-05-16 12:30:30.000000 TestGeneratorPluginLib-1.1.0/setup.py
```

### Comparing `TestGeneratorPluginLib-1.0.7/LICENSE` & `TestGeneratorPluginLib-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.0.7/PKG-INFO` & `TestGeneratorPluginLib-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TestGeneratorPluginLib
-Version: 1.0.7
+Version: 1.1.0
 Summary: A TestGeneratorPluginLib package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `TestGeneratorPluginLib-1.0.7/TestGeneratorPluginLib/_built_plugin.py` & `TestGeneratorPluginLib-1.1.0/TestGeneratorPluginLib/_built_plugin.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,63 +1,84 @@
-from typing import Callable
+from typing import Callable, Iterable, Type
 
 from TestGeneratorPluginLib._language import _FastRunOption
 from TestGeneratorPluginLib._plugin import Plugin
 from TestGeneratorPluginLib._managers import BackendManager, Manager
 from TestGeneratorPluginLib._widgets import MainTab, SideTab
 
 
 class BuiltPlugin:
     def __init__(self,
-                 plugin: Plugin,
-                 platform: str):
-        self._plugin = plugin
-        self._platform = platform if plugin.platform_specific else ''
+                 plugin: Type,
+                 name: str,
+                 description: str,
+                 version: str,
+                 author: str,
+                 url='',
+                 dependencies: Iterable[str] = tuple(),
+                 conflicts: Iterable[str] = tuple(),
+                 platform_specific=False,
+
+                 platform: str = ''):
+        self._name = name
+        self._description = description
+        self._version = version
+        self._author = author
+        self._url = url
+        self._dependencies = dependencies
+        self._conflicts = conflicts
+
+        self._plugin_class = plugin
+        self._plugin: Plugin | None = None
+        self._platform = platform if platform_specific else ''
+
+    def init(self, bm):
+        self._plugin = self._plugin_class(bm)
 
     @property
     def name(self) -> str:
-        return self._plugin.name
+        return self._name
 
     @property
     def description(self) -> str:
-        return self._plugin.description
+        return self._description
 
     @property
     def version(self) -> str:
-        return self._plugin.version
+        return self._version
 
     @property
     def author(self) -> str:
-        return self._plugin.author
+        return self._author
 
     @property
     def url(self) -> str:
-        return self._plugin.url
+        return self._url
 
     @property
     def platform(self) -> str:
         return self._platform
 
     @property
-    def dependencies(self) -> list[str]:
-        return self._plugin.dependencies
+    def dependencies(self) -> Iterable[str]:
+        return self._dependencies
 
     @property
-    def conflicts(self) -> list[str]:
-        return self._plugin.conflicts
+    def conflicts(self) -> Iterable[str]:
+        return self._conflicts
 
     @property
     def main_tabs(self) -> dict[str: Callable[[BackendManager], MainTab]]:
         return self._plugin.main_tabs
 
     @property
     def side_tabs(self) -> dict[str: Callable[[BackendManager], SideTab]]:
         return self._plugin.side_tabs
 
     @property
     def managers(self) -> dict[str: Callable[[BackendManager], Manager]]:
         return self._plugin.managers
 
     @property
-    def fast_run_options(self) -> dict[str, _FastRunOption]:
+    def fast_run_options(self) -> dict[str, list[_FastRunOption]]:
         return self._plugin.fast_run_options
```

### Comparing `TestGeneratorPluginLib-1.0.7/TestGeneratorPluginLib/_language.py` & `TestGeneratorPluginLib-1.1.0/TestGeneratorPluginLib/_language.py`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.0.7/TestGeneratorPluginLib/_managers.py` & `TestGeneratorPluginLib-1.1.0/TestGeneratorPluginLib/_managers.py`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.0.7/TestGeneratorPluginLib/_widgets.py` & `TestGeneratorPluginLib-1.1.0/TestGeneratorPluginLib/_widgets.py`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.0.7/TestGeneratorPluginLib.egg-info/PKG-INFO` & `TestGeneratorPluginLib-1.1.0/TestGeneratorPluginLib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TestGeneratorPluginLib
-Version: 1.0.7
+Version: 1.1.0
 Summary: A TestGeneratorPluginLib package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `TestGeneratorPluginLib-1.0.7/setup.py` & `TestGeneratorPluginLib-1.1.0/setup.py`

 * *Files identical despite different names*

