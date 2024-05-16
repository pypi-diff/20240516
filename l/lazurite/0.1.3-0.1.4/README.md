# Comparing `tmp/lazurite-0.1.3.tar.gz` & `tmp/lazurite-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazurite-0.1.3.tar", last modified: Thu May  9 21:50:50 2024, max compression
+gzip compressed data, was "lazurite-0.1.4.tar", last modified: Thu May 16 12:09:08 2024, max compression
```

## Comparing `lazurite-0.1.3.tar` & `lazurite-0.1.4.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 21:50:50.817446 lazurite-0.1.3/
--rw-rw-rw-   0        0        0    35823 2024-05-03 11:00:28.000000 lazurite-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     1749 2024-05-09 21:50:50.817446 lazurite-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      659 2024-05-05 13:52:03.000000 lazurite-0.1.3/README.md
--rw-rw-rw-   0        0        0     1216 2024-05-09 21:49:44.000000 lazurite-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-09 21:50:50.817446 lazurite-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-09 21:50:50.750797 lazurite-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-09 21:50:50.772056 lazurite-0.1.3/src/lazurite/
--rw-rw-rw-   0        0        0        0 2024-02-13 20:06:38.000000 lazurite-0.1.3/src/lazurite/__init__.py
--rw-rw-rw-   0        0        0       73 2024-05-03 09:54:14.000000 lazurite-0.1.3/src/lazurite/__main__.py
--rw-rw-rw-   0        0        0    12806 2024-05-09 21:47:12.000000 lazurite-0.1.3/src/lazurite/cli.py
-drwxrwxrwx   0        0        0        0 2024-05-09 21:50:50.793267 lazurite-0.1.3/src/lazurite/compiler/
--rw-rw-rw-   0        0        0       68 2024-02-13 21:47:08.000000 lazurite-0.1.3/src/lazurite/compiler/__init__.py
--rw-rw-rw-   0        0        0     2645 2024-04-30 10:45:06.000000 lazurite-0.1.3/src/lazurite/compiler/dxc.py
--rw-rw-rw-   0        0        0      766 2024-04-01 13:25:10.000000 lazurite-0.1.3/src/lazurite/compiler/macro_define.py
--rw-rw-rw-   0        0        0     6461 2024-05-03 11:38:02.000000 lazurite-0.1.3/src/lazurite/compiler/shaderc.py
-drwxrwxrwx   0        0        0        0 2024-05-09 21:50:50.797227 lazurite-0.1.3/src/lazurite/decompiler/
--rw-rw-rw-   0        0        0        0 2023-07-31 21:03:18.000000 lazurite-0.1.3/src/lazurite/decompiler/__init__.py
--rw-rw-rw-   0        0        0    25267 2024-03-31 20:06:22.000000 lazurite-0.1.3/src/lazurite/decompiler/macro_decompiler.py
--rw-rw-rw-   0        0        0     3448 2024-03-31 20:05:52.000000 lazurite-0.1.3/src/lazurite/decompiler/varying_decompiler.py
-drwxrwxrwx   0        0        0        0 2024-05-09 21:50:50.804877 lazurite-0.1.3/src/lazurite/material/
--rw-rw-rw-   0        0        0       32 2024-02-13 21:47:22.000000 lazurite-0.1.3/src/lazurite/material/__init__.py
--rw-rw-rw-   0        0        0     6210 2024-05-08 16:14:47.000000 lazurite-0.1.3/src/lazurite/material/buffer.py
--rw-rw-rw-   0        0        0      359 2024-03-20 14:54:26.000000 lazurite-0.1.3/src/lazurite/material/encryption.py
--rw-rw-rw-   0        0        0    21695 2024-04-29 14:03:32.000000 lazurite-0.1.3/src/lazurite/material/material.py
--rw-rw-rw-   0        0        0      750 2024-02-13 20:38:24.000000 lazurite-0.1.3/src/lazurite/material/platform.py
--rw-rw-rw-   0        0        0      114 2023-10-07 14:20:58.000000 lazurite-0.1.3/src/lazurite/material/precision.py
-drwxrwxrwx   0        0        0        0 2024-05-09 21:50:50.811391 lazurite-0.1.3/src/lazurite/material/shader_pass/
--rw-rw-rw-   0        0        0       28 2024-02-13 21:07:36.000000 lazurite-0.1.3/src/lazurite/material/shader_pass/__init__.py
--rw-rw-rw-   0        0        0     5398 2024-04-06 20:22:04.000000 lazurite-0.1.3/src/lazurite/material/shader_pass/bgfx_shader.py
--rw-rw-rw-   0        0        0      377 2024-02-18 16:33:18.000000 lazurite-0.1.3/src/lazurite/material/shader_pass/blend_mode.py
--rw-rw-rw-   0        0        0     4192 2024-04-06 20:22:08.000000 lazurite-0.1.3/src/lazurite/material/shader_pass/shader_definition.py
--rw-rw-rw-   0        0        0     5119 2024-04-29 18:12:28.000000 lazurite-0.1.3/src/lazurite/material/shader_pass/shader_input.py
--rw-rw-rw-   0        0        0     6354 2024-05-05 22:06:01.000000 lazurite-0.1.3/src/lazurite/material/shader_pass/shader_pass.py
--rw-rw-rw-   0        0        0     1595 2024-03-01 01:21:50.000000 lazurite-0.1.3/src/lazurite/material/shader_pass/supported_platforms.py
--rw-rw-rw-   0        0        0     3871 2024-04-06 20:22:20.000000 lazurite-0.1.3/src/lazurite/material/shader_pass/variant.py
--rw-rw-rw-   0        0        0      121 2023-09-24 16:30:26.000000 lazurite-0.1.3/src/lazurite/material/stage.py
--rw-rw-rw-   0        0        0     2502 2024-04-13 17:47:30.000000 lazurite-0.1.3/src/lazurite/material/uniform.py
-drwxrwxrwx   0        0        0        0 2024-05-09 21:50:50.817446 lazurite-0.1.3/src/lazurite/project/
--rw-rw-rw-   0        0        0        0 2024-02-13 20:05:48.000000 lazurite-0.1.3/src/lazurite/project/__init__.py
--rw-rw-rw-   0        0        0      273 2024-04-01 22:39:38.000000 lazurite-0.1.3/src/lazurite/project/compiler_type.py
--rw-rw-rw-   0        0        0     3067 2024-04-06 20:35:26.000000 lazurite-0.1.3/src/lazurite/project/material_config.py
--rw-rw-rw-   0        0        0    13430 2024-05-09 21:47:01.000000 lazurite-0.1.3/src/lazurite/project/project.py
--rw-rw-rw-   0        0        0     5513 2024-04-06 20:35:26.000000 lazurite-0.1.3/src/lazurite/project/project_config.py
--rw-rw-rw-   0        0        0     1271 2024-04-01 22:38:14.000000 lazurite-0.1.3/src/lazurite/project/shader_file_overwrite.py
--rw-rw-rw-   0        0        0      838 2024-04-29 18:29:54.000000 lazurite-0.1.3/src/lazurite/tempfile.py
--rw-rw-rw-   0        0        0     2260 2024-02-24 14:42:42.000000 lazurite-0.1.3/src/lazurite/util.py
-drwxrwxrwx   0        0        0        0 2024-05-09 21:50:50.817446 lazurite-0.1.3/src/lazurite.egg-info/
--rw-rw-rw-   0        0        0     1749 2024-05-09 21:50:50.000000 lazurite-0.1.3/src/lazurite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1522 2024-05-09 21:50:50.000000 lazurite-0.1.3/src/lazurite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 21:50:50.000000 lazurite-0.1.3/src/lazurite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-05-09 21:50:50.000000 lazurite-0.1.3/src/lazurite.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       38 2024-05-09 21:50:50.000000 lazurite-0.1.3/src/lazurite.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-09 21:50:50.000000 lazurite-0.1.3/src/lazurite.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 12:09:08.627611 lazurite-0.1.4/
+-rw-rw-rw-   0        0        0    35823 2024-05-03 11:00:28.000000 lazurite-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     1820 2024-05-16 12:09:08.626612 lazurite-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      730 2024-05-16 12:03:06.000000 lazurite-0.1.4/README.md
+-rw-rw-rw-   0        0        0     1216 2024-05-16 12:07:15.000000 lazurite-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-16 12:09:08.627611 lazurite-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-16 12:09:08.574102 lazurite-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-16 12:09:08.583100 lazurite-0.1.4/src/lazurite/
+-rw-rw-rw-   0        0        0        0 2024-02-13 20:06:38.000000 lazurite-0.1.4/src/lazurite/__init__.py
+-rw-rw-rw-   0        0        0       73 2024-05-03 09:54:14.000000 lazurite-0.1.4/src/lazurite/__main__.py
+-rw-rw-rw-   0        0        0    12806 2024-05-09 21:47:12.000000 lazurite-0.1.4/src/lazurite/cli.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:09:08.603126 lazurite-0.1.4/src/lazurite/compiler/
+-rw-rw-rw-   0        0        0       68 2024-02-13 21:47:08.000000 lazurite-0.1.4/src/lazurite/compiler/__init__.py
+-rw-rw-rw-   0        0        0     2645 2024-04-30 10:45:06.000000 lazurite-0.1.4/src/lazurite/compiler/dxc.py
+-rw-rw-rw-   0        0        0      766 2024-04-01 13:25:10.000000 lazurite-0.1.4/src/lazurite/compiler/macro_define.py
+-rw-rw-rw-   0        0        0     6461 2024-05-03 11:38:02.000000 lazurite-0.1.4/src/lazurite/compiler/shaderc.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:09:08.605147 lazurite-0.1.4/src/lazurite/decompiler/
+-rw-rw-rw-   0        0        0        0 2023-07-31 21:03:18.000000 lazurite-0.1.4/src/lazurite/decompiler/__init__.py
+-rw-rw-rw-   0        0        0    25267 2024-03-31 20:06:22.000000 lazurite-0.1.4/src/lazurite/decompiler/macro_decompiler.py
+-rw-rw-rw-   0        0        0     3448 2024-03-31 20:05:52.000000 lazurite-0.1.4/src/lazurite/decompiler/varying_decompiler.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:09:08.613095 lazurite-0.1.4/src/lazurite/material/
+-rw-rw-rw-   0        0        0       32 2024-02-13 21:47:22.000000 lazurite-0.1.4/src/lazurite/material/__init__.py
+-rw-rw-rw-   0        0        0     6210 2024-05-15 17:13:46.000000 lazurite-0.1.4/src/lazurite/material/buffer.py
+-rw-rw-rw-   0        0        0      359 2024-03-20 14:54:26.000000 lazurite-0.1.4/src/lazurite/material/encryption.py
+-rw-rw-rw-   0        0        0    21695 2024-04-29 14:03:32.000000 lazurite-0.1.4/src/lazurite/material/material.py
+-rw-rw-rw-   0        0        0      750 2024-02-13 20:38:24.000000 lazurite-0.1.4/src/lazurite/material/platform.py
+-rw-rw-rw-   0        0        0      114 2023-10-07 14:20:58.000000 lazurite-0.1.4/src/lazurite/material/precision.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:09:08.619611 lazurite-0.1.4/src/lazurite/material/shader_pass/
+-rw-rw-rw-   0        0        0       28 2024-02-13 21:07:36.000000 lazurite-0.1.4/src/lazurite/material/shader_pass/__init__.py
+-rw-rw-rw-   0        0        0     5398 2024-04-06 20:22:04.000000 lazurite-0.1.4/src/lazurite/material/shader_pass/bgfx_shader.py
+-rw-rw-rw-   0        0        0      377 2024-02-18 16:33:18.000000 lazurite-0.1.4/src/lazurite/material/shader_pass/blend_mode.py
+-rw-rw-rw-   0        0        0     4192 2024-04-06 20:22:08.000000 lazurite-0.1.4/src/lazurite/material/shader_pass/shader_definition.py
+-rw-rw-rw-   0        0        0     5119 2024-04-29 18:12:28.000000 lazurite-0.1.4/src/lazurite/material/shader_pass/shader_input.py
+-rw-rw-rw-   0        0        0     6354 2024-05-05 22:06:01.000000 lazurite-0.1.4/src/lazurite/material/shader_pass/shader_pass.py
+-rw-rw-rw-   0        0        0     1595 2024-03-01 01:21:50.000000 lazurite-0.1.4/src/lazurite/material/shader_pass/supported_platforms.py
+-rw-rw-rw-   0        0        0     3871 2024-04-06 20:22:20.000000 lazurite-0.1.4/src/lazurite/material/shader_pass/variant.py
+-rw-rw-rw-   0        0        0      121 2023-09-24 16:30:26.000000 lazurite-0.1.4/src/lazurite/material/stage.py
+-rw-rw-rw-   0        0        0     2502 2024-04-13 17:47:30.000000 lazurite-0.1.4/src/lazurite/material/uniform.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:09:08.624611 lazurite-0.1.4/src/lazurite/project/
+-rw-rw-rw-   0        0        0        0 2024-02-13 20:05:48.000000 lazurite-0.1.4/src/lazurite/project/__init__.py
+-rw-rw-rw-   0        0        0      273 2024-04-01 22:39:38.000000 lazurite-0.1.4/src/lazurite/project/compiler_type.py
+-rw-rw-rw-   0        0        0     3067 2024-04-06 20:35:26.000000 lazurite-0.1.4/src/lazurite/project/material_config.py
+-rw-rw-rw-   0        0        0    13693 2024-05-16 11:55:24.000000 lazurite-0.1.4/src/lazurite/project/project.py
+-rw-rw-rw-   0        0        0     5513 2024-04-06 20:35:26.000000 lazurite-0.1.4/src/lazurite/project/project_config.py
+-rw-rw-rw-   0        0        0     1271 2024-04-01 22:38:14.000000 lazurite-0.1.4/src/lazurite/project/shader_file_overwrite.py
+-rw-rw-rw-   0        0        0      838 2024-04-29 18:29:54.000000 lazurite-0.1.4/src/lazurite/tempfile.py
+-rw-rw-rw-   0        0        0     2260 2024-02-24 14:42:42.000000 lazurite-0.1.4/src/lazurite/util.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:09:08.625612 lazurite-0.1.4/src/lazurite.egg-info/
+-rw-rw-rw-   0        0        0     1820 2024-05-16 12:09:08.000000 lazurite-0.1.4/src/lazurite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1522 2024-05-16 12:09:08.000000 lazurite-0.1.4/src/lazurite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 12:09:08.000000 lazurite-0.1.4/src/lazurite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-05-16 12:09:08.000000 lazurite-0.1.4/src/lazurite.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       38 2024-05-16 12:09:08.000000 lazurite-0.1.4/src/lazurite.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-16 12:09:08.000000 lazurite-0.1.4/src/lazurite.egg-info/top_level.txt
```

### Comparing `lazurite-0.1.3/LICENSE` & `lazurite-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lazurite-0.1.3/PKG-INFO` & `lazurite-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazurite
-Version: 0.1.3
+Version: 0.1.4
 Summary: Unofficial shader development tool for Minecraft: Bedrock Edition with RenderDragon graphics engine
 Author: veka0
 Project-URL: Documentation, https://veka0.github.io/lazurite
 Project-URL: Repository, https://github.com/veka0/lazurite
 Keywords: shader,minecraft,bedrock,renderdragon
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
@@ -33,15 +33,16 @@
 
 PyPi page: <https://pypi.org/project/lazurite>
 
 ## Installation
 
 Lazurite requires to have Python 3.10+ installed, but 3.12 is recommended.
 
-Official python installation page: <https://www.python.org/downloads/>
+Official python installation page: <https://www.python.org/downloads>.
+Windows users are recommended to install Python from Microsoft Store.
 
 After installing python, you can install lazurite package from pypi repository, with a command
 
 ```sh
 pip install lazurite
 ```
```

### Comparing `lazurite-0.1.3/README.md` & `lazurite-0.1.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 
 PyPi page: <https://pypi.org/project/lazurite>
 
 ## Installation
 
 Lazurite requires to have Python 3.10+ installed, but 3.12 is recommended.
 
-Official python installation page: <https://www.python.org/downloads/>
+Official python installation page: <https://www.python.org/downloads>.
+Windows users are recommended to install Python from Microsoft Store.
 
 After installing python, you can install lazurite package from pypi repository, with a command
 
 ```sh
 pip install lazurite
 ```
```

### Comparing `lazurite-0.1.3/pyproject.toml` & `lazurite-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "lazurite"
 description = "Unofficial shader development tool for Minecraft: Bedrock Edition with RenderDragon graphics engine"
 keywords = ["shader", "minecraft", "bedrock", "renderdragon"]
-version = "0.1.3"
+version = "0.1.4"
 readme = "README.md"
 requires-python = ">=3.10"
 authors = [{ name = "veka0" }]
 
 classifiers = [
     # General
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `lazurite-0.1.3/src/lazurite/cli.py` & `lazurite-0.1.4/src/lazurite/cli.py`

 * *Files identical despite different names*

### Comparing `lazurite-0.1.3/src/lazurite/compiler/dxc.py` & `lazurite-0.1.4/src/lazurite/compiler/dxc.py`

 * *Files identical despite different names*

### Comparing `lazurite-0.1.3/src/lazurite/compiler/macro_define.py` & `lazurite-0.1.4/src/lazurite/compiler/macro_define.py`

 * *Files identical despite different names*

### Comparing `lazurite-0.1.3/src/lazurite/compiler/shaderc.py` & `lazurite-0.1.4/src/lazurite/compiler/shaderc.py`

 * *Files identical despite different names*

### Comparing `lazurite-0.1.3/src/lazurite/decompiler/macro_decompiler.py` & `lazurite-0.1.4/src/lazurite/decompiler/macro_decompiler.py`

 * *Files identical despite different names*

### Comparing `lazurite-0.1.3/src/lazurite/decompiler/varying_decompiler.py` & `lazurite-0.1.4/src/lazurite/decompiler/varying_decompiler.py`

 * *Files identical despite different names*

### Comparing `lazurite-0.1.3/src/lazurite/material/buffer.py` & `lazurite-0.1.4/src/lazurite/material/buffer.py`

 * *Files identical despite different names*

### Comparing `lazurite-0.1.3/src/lazurite/material/material.py` & `lazurite-0.1.4/src/lazurite/material/material.py`

 * *Files identical despite different names*

### Comparing `lazurite-0.1.3/src/lazurite/material/platform.py` & `lazurite-0.1.4/src/lazurite/material/platform.py`

 * *Files identical despite different names*

### Comparing `lazurite-0.1.3/src/lazurite/material/shader_pass/bgfx_shader.py` & `lazurite-0.1.4/src/lazurite/material/shader_pass/bgfx_shader.py`

 * *Files identical despite different names*

### Comparing `lazurite-0.1.3/src/lazurite/material/shader_pass/shader_definition.py` & `lazurite-0.1.4/src/lazurite/material/shader_pass/shader_definition.py`

 * *Files identical despite different names*

### Comparing `lazurite-0.1.3/src/lazurite/material/shader_pass/shader_input.py` & `lazurite-0.1.4/src/lazurite/material/shader_pass/shader_input.py`

 * *Files identical despite different names*

### Comparing `lazurite-0.1.3/src/lazurite/material/shader_pass/shader_pass.py` & `lazurite-0.1.4/src/lazurite/material/shader_pass/shader_pass.py`

 * *Files identical despite different names*

### Comparing `lazurite-0.1.3/src/lazurite/material/shader_pass/supported_platforms.py` & `lazurite-0.1.4/src/lazurite/material/shader_pass/supported_platforms.py`

 * *Files identical despite different names*

### Comparing `lazurite-0.1.3/src/lazurite/material/shader_pass/variant.py` & `lazurite-0.1.4/src/lazurite/material/shader_pass/variant.py`

 * *Files identical despite different names*

### Comparing `lazurite-0.1.3/src/lazurite/material/uniform.py` & `lazurite-0.1.4/src/lazurite/material/uniform.py`

 * *Files identical despite different names*

### Comparing `lazurite-0.1.3/src/lazurite/project/material_config.py` & `lazurite-0.1.4/src/lazurite/project/material_config.py`

 * *Files identical despite different names*

### Comparing `lazurite-0.1.3/src/lazurite/project/project.py` & `lazurite-0.1.4/src/lazurite/project/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     platforms: list[ShaderPlatform],
     merge_source: list[str],
     cache: dict[str, tuple[str, set[ShaderPlatform]]],
 ):
     mat = None
     for platform in platforms:
         for path in merge_source:
-            if not path.endswith(name):
+            if os.path.basename(path) != name:
                 continue
             found_platform = False
             if path in cache:
                 if platform in cache[path][1]:
                     found_platform = True
                     temp_mat = Material.load_bin_file(path)
                     if mat is None:
@@ -246,23 +246,28 @@
             )
             or Material()
         )
 
         # If it failed to load any source materials.
         if not material.get_platforms():
             # Load and merge vanilla materials with any platforms.
-            material = (
-                _merge_source_materials(
-                    mat_dir,
-                    set(ShaderPlatform),
-                    proj_config.merge_source,
-                    material_cache,
-                )
-                or material
+            temp_mat = _merge_source_materials(
+                mat_dir,
+                set(ShaderPlatform),
+                proj_config.merge_source,
+                material_cache,
             )
+
+            if temp_mat:
+                material = temp_mat
+            elif proj_config.merge_source:
+                # Display a warning if no valid merge source was ever found
+                # but merge_source in project config is not empty.
+                print(f"Warning! Failed to find merge source for {mat_dir.name}")
+
             # Add necessary platforms.
             material.add_platforms(compilable_platforms)
             # Remove other unwanted platforms.
             material.remove_platforms(
                 set(ShaderPlatform).difference(compilable_platforms)
             )
         else:
```

### Comparing `lazurite-0.1.3/src/lazurite/project/project_config.py` & `lazurite-0.1.4/src/lazurite/project/project_config.py`

 * *Files identical despite different names*

### Comparing `lazurite-0.1.3/src/lazurite/project/shader_file_overwrite.py` & `lazurite-0.1.4/src/lazurite/project/shader_file_overwrite.py`

 * *Files identical despite different names*

### Comparing `lazurite-0.1.3/src/lazurite/tempfile.py` & `lazurite-0.1.4/src/lazurite/tempfile.py`

 * *Files identical despite different names*

### Comparing `lazurite-0.1.3/src/lazurite/util.py` & `lazurite-0.1.4/src/lazurite/util.py`

 * *Files identical despite different names*

### Comparing `lazurite-0.1.3/src/lazurite.egg-info/PKG-INFO` & `lazurite-0.1.4/src/lazurite.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazurite
-Version: 0.1.3
+Version: 0.1.4
 Summary: Unofficial shader development tool for Minecraft: Bedrock Edition with RenderDragon graphics engine
 Author: veka0
 Project-URL: Documentation, https://veka0.github.io/lazurite
 Project-URL: Repository, https://github.com/veka0/lazurite
 Keywords: shader,minecraft,bedrock,renderdragon
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
@@ -33,15 +33,16 @@
 
 PyPi page: <https://pypi.org/project/lazurite>
 
 ## Installation
 
 Lazurite requires to have Python 3.10+ installed, but 3.12 is recommended.
 
-Official python installation page: <https://www.python.org/downloads/>
+Official python installation page: <https://www.python.org/downloads>.
+Windows users are recommended to install Python from Microsoft Store.
 
 After installing python, you can install lazurite package from pypi repository, with a command
 
 ```sh
 pip install lazurite
 ```
```

### Comparing `lazurite-0.1.3/src/lazurite.egg-info/SOURCES.txt` & `lazurite-0.1.4/src/lazurite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

