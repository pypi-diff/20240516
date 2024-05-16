# Comparing `tmp/TestGeneratorPluginLib-1.1.0.tar.gz` & `tmp/TestGeneratorPluginLib-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TestGeneratorPluginLib-1.1.0.tar", last modified: Thu May 16 12:31:35 2024, max compression
+gzip compressed data, was "TestGeneratorPluginLib-1.1.1.tar", last modified: Thu May 16 12:38:52 2024, max compression
```

## Comparing `TestGeneratorPluginLib-1.1.0.tar` & `TestGeneratorPluginLib-1.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 12:31:35.612756 TestGeneratorPluginLib-1.1.0/
--rw-rw-rw-   0        0        0     1090 2024-05-16 12:30:30.000000 TestGeneratorPluginLib-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     1569 2024-05-16 12:31:35.612756 TestGeneratorPluginLib-1.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-16 12:31:35.612756 TestGeneratorPluginLib-1.1.0/TestGeneratorPluginLib/
--rw-rw-rw-   0        0        0      350 2024-05-16 12:30:30.000000 TestGeneratorPluginLib-1.1.0/TestGeneratorPluginLib/__init__.py
--rw-rw-rw-   0        0        0     2357 2024-05-16 12:30:30.000000 TestGeneratorPluginLib-1.1.0/TestGeneratorPluginLib/_built_plugin.py
--rw-rw-rw-   0        0        0       19 2024-05-16 12:30:30.000000 TestGeneratorPluginLib-1.1.0/TestGeneratorPluginLib/_config.py
--rw-rw-rw-   0        0        0     1780 2024-05-16 12:30:30.000000 TestGeneratorPluginLib-1.1.0/TestGeneratorPluginLib/_language.py
--rw-rw-rw-   0        0        0     1219 2024-05-16 12:30:30.000000 TestGeneratorPluginLib-1.1.0/TestGeneratorPluginLib/_managers.py
--rw-rw-rw-   0        0        0      533 2024-05-16 12:30:30.000000 TestGeneratorPluginLib-1.1.0/TestGeneratorPluginLib/_plugin.py
--rw-rw-rw-   0        0        0     2834 2024-05-16 12:30:30.000000 TestGeneratorPluginLib-1.1.0/TestGeneratorPluginLib/_plugin_setup.py
--rw-rw-rw-   0        0        0     3344 2024-05-16 12:30:30.000000 TestGeneratorPluginLib-1.1.0/TestGeneratorPluginLib/_widgets.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:31:35.612756 TestGeneratorPluginLib-1.1.0/TestGeneratorPluginLib.egg-info/
--rw-rw-rw-   0        0        0     1569 2024-05-16 12:31:35.000000 TestGeneratorPluginLib-1.1.0/TestGeneratorPluginLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      535 2024-05-16 12:31:35.000000 TestGeneratorPluginLib-1.1.0/TestGeneratorPluginLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 12:31:35.000000 TestGeneratorPluginLib-1.1.0/TestGeneratorPluginLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-16 12:31:35.000000 TestGeneratorPluginLib-1.1.0/TestGeneratorPluginLib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-05-16 12:31:35.000000 TestGeneratorPluginLib-1.1.0/TestGeneratorPluginLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 12:31:35.612756 TestGeneratorPluginLib-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1288 2024-05-16 12:30:30.000000 TestGeneratorPluginLib-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:38:52.501874 TestGeneratorPluginLib-1.1.1/
+-rw-rw-rw-   0        0        0     1090 2024-05-16 12:37:59.000000 TestGeneratorPluginLib-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1569 2024-05-16 12:38:52.501874 TestGeneratorPluginLib-1.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-16 12:38:52.501874 TestGeneratorPluginLib-1.1.1/TestGeneratorPluginLib/
+-rw-rw-rw-   0        0        0      350 2024-05-16 12:37:59.000000 TestGeneratorPluginLib-1.1.1/TestGeneratorPluginLib/__init__.py
+-rw-rw-rw-   0        0        0     2357 2024-05-16 12:37:59.000000 TestGeneratorPluginLib-1.1.1/TestGeneratorPluginLib/_built_plugin.py
+-rw-rw-rw-   0        0        0       19 2024-05-16 12:37:59.000000 TestGeneratorPluginLib-1.1.1/TestGeneratorPluginLib/_config.py
+-rw-rw-rw-   0        0        0     1780 2024-05-16 12:37:59.000000 TestGeneratorPluginLib-1.1.1/TestGeneratorPluginLib/_language.py
+-rw-rw-rw-   0        0        0     1219 2024-05-16 12:37:59.000000 TestGeneratorPluginLib-1.1.1/TestGeneratorPluginLib/_managers.py
+-rw-rw-rw-   0        0        0      533 2024-05-16 12:37:59.000000 TestGeneratorPluginLib-1.1.1/TestGeneratorPluginLib/_plugin.py
+-rw-rw-rw-   0        0        0     2854 2024-05-16 12:37:59.000000 TestGeneratorPluginLib-1.1.1/TestGeneratorPluginLib/_plugin_setup.py
+-rw-rw-rw-   0        0        0     3344 2024-05-16 12:37:59.000000 TestGeneratorPluginLib-1.1.1/TestGeneratorPluginLib/_widgets.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:38:52.501874 TestGeneratorPluginLib-1.1.1/TestGeneratorPluginLib.egg-info/
+-rw-rw-rw-   0        0        0     1569 2024-05-16 12:38:52.000000 TestGeneratorPluginLib-1.1.1/TestGeneratorPluginLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      535 2024-05-16 12:38:52.000000 TestGeneratorPluginLib-1.1.1/TestGeneratorPluginLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 12:38:52.000000 TestGeneratorPluginLib-1.1.1/TestGeneratorPluginLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-16 12:38:52.000000 TestGeneratorPluginLib-1.1.1/TestGeneratorPluginLib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-05-16 12:38:52.000000 TestGeneratorPluginLib-1.1.1/TestGeneratorPluginLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 12:38:52.501874 TestGeneratorPluginLib-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1288 2024-05-16 12:37:59.000000 TestGeneratorPluginLib-1.1.1/setup.py
```

### Comparing `TestGeneratorPluginLib-1.1.0/LICENSE` & `TestGeneratorPluginLib-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.1.0/PKG-INFO` & `TestGeneratorPluginLib-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TestGeneratorPluginLib
-Version: 1.1.0
+Version: 1.1.1
 Summary: A TestGeneratorPluginLib package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `TestGeneratorPluginLib-1.1.0/TestGeneratorPluginLib/_built_plugin.py` & `TestGeneratorPluginLib-1.1.1/TestGeneratorPluginLib/_built_plugin.py`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.1.0/TestGeneratorPluginLib/_language.py` & `TestGeneratorPluginLib-1.1.1/TestGeneratorPluginLib/_language.py`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.1.0/TestGeneratorPluginLib/_managers.py` & `TestGeneratorPluginLib-1.1.1/TestGeneratorPluginLib/_managers.py`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.1.0/TestGeneratorPluginLib/_plugin.py` & `TestGeneratorPluginLib-1.1.1/TestGeneratorPluginLib/_plugin.py`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.1.0/TestGeneratorPluginLib/_plugin_setup.py` & `TestGeneratorPluginLib-1.1.1/TestGeneratorPluginLib/_plugin_setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -63,13 +63,13 @@
         if self._requirements:
             subprocess.run(['pip', 'install', *self._requirements, '-t', os.path.join(build_path, '__packages__')])
 
         with open(os.path.join(build_path, '__plugin__.py'), 'w', encoding='utf-8') as f:
             f.write(f"""from TestGeneratorPluginLib._built_plugin import BuiltPlugin
 from {self._plugin[:self._plugin.rindex('.')]} import {self._plugin[self._plugin.rindex('.') + 1:]} as Plugin
 
-__plugin__ = BuiltPlugin(Plugin, '{self.name}', '{self.description}', '{self.version}', '{self.author}',
-                         '{self.url}', {self.dependencies}, {self.conflicts}, {self.platform_specific}, 
+__plugin__ = BuiltPlugin(Plugin, {repr(self.name)}, {repr(self.description)}, {repr(self.version)}, {repr(self.author)},
+                         {repr(self.url)}, {self.dependencies}, {self.conflicts}, {self.platform_specific}, 
                          '{sys.platform}')
 """)
 
         shutil.make_archive(dist_path, 'zip', build_path)
```

### Comparing `TestGeneratorPluginLib-1.1.0/TestGeneratorPluginLib/_widgets.py` & `TestGeneratorPluginLib-1.1.1/TestGeneratorPluginLib/_widgets.py`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.1.0/TestGeneratorPluginLib.egg-info/PKG-INFO` & `TestGeneratorPluginLib-1.1.1/TestGeneratorPluginLib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TestGeneratorPluginLib
-Version: 1.1.0
+Version: 1.1.1
 Summary: A TestGeneratorPluginLib package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `TestGeneratorPluginLib-1.1.0/TestGeneratorPluginLib.egg-info/SOURCES.txt` & `TestGeneratorPluginLib-1.1.1/TestGeneratorPluginLib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.1.0/setup.py` & `TestGeneratorPluginLib-1.1.1/setup.py`

 * *Files identical despite different names*

