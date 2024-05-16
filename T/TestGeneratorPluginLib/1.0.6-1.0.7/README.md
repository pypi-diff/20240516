# Comparing `tmp/TestGeneratorPluginLib-1.0.6.tar.gz` & `tmp/TestGeneratorPluginLib-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TestGeneratorPluginLib-1.0.6.tar", last modified: Wed May 15 14:21:11 2024, max compression
+gzip compressed data, was "TestGeneratorPluginLib-1.0.7.tar", last modified: Wed May 15 15:35:07 2024, max compression
```

## Comparing `TestGeneratorPluginLib-1.0.6.tar` & `TestGeneratorPluginLib-1.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 14:21:11.670509 TestGeneratorPluginLib-1.0.6/
--rw-rw-rw-   0        0        0     1090 2024-05-15 14:20:37.000000 TestGeneratorPluginLib-1.0.6/LICENSE
--rw-rw-rw-   0        0        0     1569 2024-05-15 14:21:11.670509 TestGeneratorPluginLib-1.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-15 14:21:11.670509 TestGeneratorPluginLib-1.0.6/TestGeneratorPluginLib/
--rw-rw-rw-   0        0        0      288 2024-05-15 14:20:37.000000 TestGeneratorPluginLib-1.0.6/TestGeneratorPluginLib/__init__.py
--rw-rw-rw-   0        0        0     1707 2024-05-15 14:20:37.000000 TestGeneratorPluginLib-1.0.6/TestGeneratorPluginLib/_built_plugin.py
--rw-rw-rw-   0        0        0       19 2024-05-15 14:20:37.000000 TestGeneratorPluginLib-1.0.6/TestGeneratorPluginLib/_config.py
--rw-rw-rw-   0        0        0     1780 2024-05-15 14:20:37.000000 TestGeneratorPluginLib-1.0.6/TestGeneratorPluginLib/_language.py
--rw-rw-rw-   0        0        0     1219 2024-05-15 14:20:37.000000 TestGeneratorPluginLib-1.0.6/TestGeneratorPluginLib/_managers.py
--rw-rw-rw-   0        0        0     3101 2024-05-15 14:20:37.000000 TestGeneratorPluginLib-1.0.6/TestGeneratorPluginLib/_plugin.py
--rw-rw-rw-   0        0        0     3344 2024-05-15 14:20:37.000000 TestGeneratorPluginLib-1.0.6/TestGeneratorPluginLib/_widgets.py
-drwxrwxrwx   0        0        0        0 2024-05-15 14:21:11.670509 TestGeneratorPluginLib-1.0.6/TestGeneratorPluginLib.egg-info/
--rw-rw-rw-   0        0        0     1569 2024-05-15 14:21:11.000000 TestGeneratorPluginLib-1.0.6/TestGeneratorPluginLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      495 2024-05-15 14:21:11.000000 TestGeneratorPluginLib-1.0.6/TestGeneratorPluginLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 14:21:11.000000 TestGeneratorPluginLib-1.0.6/TestGeneratorPluginLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-15 14:21:11.000000 TestGeneratorPluginLib-1.0.6/TestGeneratorPluginLib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-05-15 14:21:11.000000 TestGeneratorPluginLib-1.0.6/TestGeneratorPluginLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 14:21:11.670509 TestGeneratorPluginLib-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1288 2024-05-15 14:20:37.000000 TestGeneratorPluginLib-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 15:35:07.142835 TestGeneratorPluginLib-1.0.7/
+-rw-rw-rw-   0        0        0     1090 2024-05-15 15:34:08.000000 TestGeneratorPluginLib-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0     1569 2024-05-15 15:35:07.142835 TestGeneratorPluginLib-1.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-15 15:35:07.142835 TestGeneratorPluginLib-1.0.7/TestGeneratorPluginLib/
+-rw-rw-rw-   0        0        0      288 2024-05-15 15:34:08.000000 TestGeneratorPluginLib-1.0.7/TestGeneratorPluginLib/__init__.py
+-rw-rw-rw-   0        0        0     1707 2024-05-15 15:34:08.000000 TestGeneratorPluginLib-1.0.7/TestGeneratorPluginLib/_built_plugin.py
+-rw-rw-rw-   0        0        0       19 2024-05-15 15:34:08.000000 TestGeneratorPluginLib-1.0.7/TestGeneratorPluginLib/_config.py
+-rw-rw-rw-   0        0        0     1780 2024-05-15 15:34:08.000000 TestGeneratorPluginLib-1.0.7/TestGeneratorPluginLib/_language.py
+-rw-rw-rw-   0        0        0     1219 2024-05-15 15:34:08.000000 TestGeneratorPluginLib-1.0.7/TestGeneratorPluginLib/_managers.py
+-rw-rw-rw-   0        0        0     3227 2024-05-15 15:34:08.000000 TestGeneratorPluginLib-1.0.7/TestGeneratorPluginLib/_plugin.py
+-rw-rw-rw-   0        0        0     3344 2024-05-15 15:34:08.000000 TestGeneratorPluginLib-1.0.7/TestGeneratorPluginLib/_widgets.py
+drwxrwxrwx   0        0        0        0 2024-05-15 15:35:07.142835 TestGeneratorPluginLib-1.0.7/TestGeneratorPluginLib.egg-info/
+-rw-rw-rw-   0        0        0     1569 2024-05-15 15:35:07.000000 TestGeneratorPluginLib-1.0.7/TestGeneratorPluginLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      495 2024-05-15 15:35:07.000000 TestGeneratorPluginLib-1.0.7/TestGeneratorPluginLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 15:35:07.000000 TestGeneratorPluginLib-1.0.7/TestGeneratorPluginLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-15 15:35:07.000000 TestGeneratorPluginLib-1.0.7/TestGeneratorPluginLib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-05-15 15:35:07.000000 TestGeneratorPluginLib-1.0.7/TestGeneratorPluginLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 15:35:07.142835 TestGeneratorPluginLib-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1288 2024-05-15 15:34:08.000000 TestGeneratorPluginLib-1.0.7/setup.py
```

### Comparing `TestGeneratorPluginLib-1.0.6/LICENSE` & `TestGeneratorPluginLib-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.0.6/PKG-INFO` & `TestGeneratorPluginLib-1.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TestGeneratorPluginLib
-Version: 1.0.6
+Version: 1.0.7
 Summary: A TestGeneratorPluginLib package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `TestGeneratorPluginLib-1.0.6/TestGeneratorPluginLib/_built_plugin.py` & `TestGeneratorPluginLib-1.0.7/TestGeneratorPluginLib/_built_plugin.py`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.0.6/TestGeneratorPluginLib/_language.py` & `TestGeneratorPluginLib-1.0.7/TestGeneratorPluginLib/_language.py`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.0.6/TestGeneratorPluginLib/_managers.py` & `TestGeneratorPluginLib-1.0.7/TestGeneratorPluginLib/_managers.py`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.0.6/TestGeneratorPluginLib/_plugin.py` & `TestGeneratorPluginLib-1.0.7/TestGeneratorPluginLib/_plugin.py`

 * *Files 7% similar despite different names*

```diff
@@ -48,27 +48,29 @@
         self.fast_run_options = fast_run_options or dict()
 
         self._parse_args()
 
     def _parse_args(self):
         _parser = argparse.ArgumentParser()
         _parser.add_argument('-b', '--build', action='store_true')
+        _parser.add_argument('-o', '--output')
         _parser.add_argument('-u', '--upload', action='store_true')
         args = _parser.parse_args()
 
         if args.build:
-            self._build()
+            self._build(args.output)
 
-    def _build(self):
+    def _build(self, output=None):
         build_path = f'build/{self.name}'
-        dist_path = f'dist/{self.name}.TGPlugin'
+        dist_path = output or f'dist/{self.name}.TGPlugin'
         if os.path.isdir(build_path):
             shutil.rmtree(build_path)
         os.makedirs(build_path)
-        os.makedirs(os.path.dirname(dist_path), exist_ok=True)
+        if os.path.dirname(dist_path):
+            os.makedirs(os.path.dirname(dist_path), exist_ok=True)
 
         for el in self._directories:
             shutil.copytree(el, os.path.join(build_path, el))
         shutil.copy(argv[0], os.path.join(build_path, os.path.basename(argv[0])))
 
         if self._requirements:
             subprocess.run(['pip', 'install', *self._requirements, '-t', os.path.join(build_path, '__packages__')])
```

### Comparing `TestGeneratorPluginLib-1.0.6/TestGeneratorPluginLib/_widgets.py` & `TestGeneratorPluginLib-1.0.7/TestGeneratorPluginLib/_widgets.py`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.0.6/TestGeneratorPluginLib.egg-info/PKG-INFO` & `TestGeneratorPluginLib-1.0.7/TestGeneratorPluginLib.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TestGeneratorPluginLib
-Version: 1.0.6
+Version: 1.0.7
 Summary: A TestGeneratorPluginLib package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `TestGeneratorPluginLib-1.0.6/setup.py` & `TestGeneratorPluginLib-1.0.7/setup.py`

 * *Files identical despite different names*

