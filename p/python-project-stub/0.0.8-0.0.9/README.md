# Comparing `tmp/python_project_stub-0.0.8.tar.gz` & `tmp/python_project_stub-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_project_stub-0.0.8.tar", last modified: Thu May 16 06:18:20 2024, max compression
+gzip compressed data, was "python_project_stub-0.0.9.tar", last modified: Thu May 16 06:59:10 2024, max compression
```

## Comparing `python_project_stub-0.0.8.tar` & `python_project_stub-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-16 06:18:20.562386 python_project_stub-0.0.8/
--rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)     1076 2024-05-16 06:15:52.000000 python_project_stub-0.0.8/LICENSE
--rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)       43 2024-05-15 20:25:30.000000 python_project_stub-0.0.8/MANIFEST.in
--rw-r--r--   0 jstrieb   (1012) jstrieb   (1012)    16958 2024-05-16 06:18:20.562386 python_project_stub-0.0.8/PKG-INFO
--rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)    16523 2024-05-15 20:25:30.000000 python_project_stub-0.0.8/README.md
--rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)      603 2024-05-16 06:18:18.000000 python_project_stub-0.0.8/pyproject.toml
-drwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-16 06:18:20.558386 python_project_stub-0.0.8/python_project_stub/
--rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)       82 2024-05-15 20:25:30.000000 python_project_stub-0.0.8/python_project_stub/__init__.py
--rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)     1660 2024-05-15 20:25:30.000000 python_project_stub-0.0.8/python_project_stub/__main__.py
-drwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-16 06:18:20.562386 python_project_stub-0.0.8/python_project_stub/data/
--rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-15 20:25:30.000000 python_project_stub-0.0.8/python_project_stub/data/__init__.py
--rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)       82 2024-05-15 20:25:30.000000 python_project_stub-0.0.8/python_project_stub/data/quote.txt
-drwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-16 06:18:20.562386 python_project_stub-0.0.8/python_project_stub.egg-info/
--rw-r--r--   0 jstrieb   (1012) jstrieb   (1012)    16958 2024-05-16 06:18:20.000000 python_project_stub-0.0.8/python_project_stub.egg-info/PKG-INFO
--rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)      408 2024-05-16 06:18:20.000000 python_project_stub-0.0.8/python_project_stub.egg-info/SOURCES.txt
--rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)        1 2024-05-16 06:18:20.000000 python_project_stub-0.0.8/python_project_stub.egg-info/dependency_links.txt
--rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)       74 2024-05-16 06:18:20.000000 python_project_stub-0.0.8/python_project_stub.egg-info/entry_points.txt
--rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)       20 2024-05-16 06:18:20.000000 python_project_stub-0.0.8/python_project_stub.egg-info/top_level.txt
--rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)      170 2024-05-16 06:18:20.562386 python_project_stub-0.0.8/setup.cfg
+drwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-16 06:59:10.042792 python_project_stub-0.0.9/
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)     1076 2024-05-16 06:15:52.000000 python_project_stub-0.0.9/LICENSE
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)       45 2024-05-16 06:59:08.000000 python_project_stub-0.0.9/MANIFEST.in
+-rw-r--r--   0 jstrieb   (1012) jstrieb   (1012)    16958 2024-05-16 06:59:10.042792 python_project_stub-0.0.9/PKG-INFO
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)    16523 2024-05-15 20:25:30.000000 python_project_stub-0.0.9/README.md
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)      603 2024-05-16 06:59:08.000000 python_project_stub-0.0.9/pyproject.toml
+drwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-16 06:59:10.042792 python_project_stub-0.0.9/python_project_stub/
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)       82 2024-05-15 20:25:30.000000 python_project_stub-0.0.9/python_project_stub/__init__.py
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)     1660 2024-05-15 20:25:30.000000 python_project_stub-0.0.9/python_project_stub/__main__.py
+drwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-16 06:59:10.042792 python_project_stub-0.0.9/python_project_stub/data/
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-15 20:25:30.000000 python_project_stub-0.0.9/python_project_stub/data/__init__.py
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)       82 2024-05-15 20:25:30.000000 python_project_stub-0.0.9/python_project_stub/data/quote.txt
+drwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-16 06:59:10.042792 python_project_stub-0.0.9/python_project_stub.egg-info/
+-rw-r--r--   0 jstrieb   (1012) jstrieb   (1012)    16958 2024-05-16 06:59:10.000000 python_project_stub-0.0.9/python_project_stub.egg-info/PKG-INFO
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)      445 2024-05-16 06:59:10.000000 python_project_stub-0.0.9/python_project_stub.egg-info/SOURCES.txt
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)        1 2024-05-16 06:59:10.000000 python_project_stub-0.0.9/python_project_stub.egg-info/dependency_links.txt
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)       74 2024-05-16 06:59:10.000000 python_project_stub-0.0.9/python_project_stub.egg-info/entry_points.txt
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)       20 2024-05-16 06:59:10.000000 python_project_stub-0.0.9/python_project_stub.egg-info/top_level.txt
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)      170 2024-05-16 06:59:10.042792 python_project_stub-0.0.9/setup.cfg
```

### Comparing `python_project_stub-0.0.8/LICENSE` & `python_project_stub-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `python_project_stub-0.0.8/PKG-INFO` & `python_project_stub-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-project-stub
-Version: 0.0.8
+Version: 0.0.9
 Summary: Stub files to use as the basis of a Python project that can be packaged and uploaded to PyPI
 Home-page: https://github.com/striebel/python-project-stub
 Author: Jacob Striebel
 Author-email: jacob.striebel@example.com
 License: MIT
 Project-URL: Homepage, https://github.com/striebel/python-project-stub
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-project-stub Version: 0.0.8 Summary: Stub
+Metadata-Version: 2.1 Name: python-project-stub Version: 0.0.9 Summary: Stub
 files to use as the basis of a Python project that can be packaged and uploaded
 to PyPI Home-page: https://github.com/striebel/python-project-stub Author:
 Jacob Striebel Author-email: jacob.striebel@example.com License: MIT Project-
 URL: Homepage, https://github.com/striebel/python-project-stub Description-
 Content-Type: text/markdown License-File: LICENSE # `python-project-stub`_[_P_y_P_I_]
 _[_D_o_w_n_l_o_a_d_s_]_[_L_i_c_e_n_s_e_]
```

### Comparing `python_project_stub-0.0.8/README.md` & `python_project_stub-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `python_project_stub-0.0.8/pyproject.toml` & `python_project_stub-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
     requires      = ["setuptools>=61.0.0"]
     build-backend = "setuptools.build_meta"
 
 [project]
     name         = "python-project-stub"
-    version      = "0.0.8"
+    version      = "0.0.9"
     dynamic      = ["authors"] # specified in setup.cfg
     description  = "Stub files to use as the basis of a Python project that can be packaged and uploaded to PyPI"
     license      = {text = "MIT"}
     dependencies = [] # TODO
     readme = "README.md"
 
 [project.scripts]
```

### Comparing `python_project_stub-0.0.8/python_project_stub/__main__.py` & `python_project_stub-0.0.9/python_project_stub/__main__.py`

 * *Files identical despite different names*

### Comparing `python_project_stub-0.0.8/python_project_stub.egg-info/PKG-INFO` & `python_project_stub-0.0.9/python_project_stub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-project-stub
-Version: 0.0.8
+Version: 0.0.9
 Summary: Stub files to use as the basis of a Python project that can be packaged and uploaded to PyPI
 Home-page: https://github.com/striebel/python-project-stub
 Author: Jacob Striebel
 Author-email: jacob.striebel@example.com
 License: MIT
 Project-URL: Homepage, https://github.com/striebel/python-project-stub
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-project-stub Version: 0.0.8 Summary: Stub
+Metadata-Version: 2.1 Name: python-project-stub Version: 0.0.9 Summary: Stub
 files to use as the basis of a Python project that can be packaged and uploaded
 to PyPI Home-page: https://github.com/striebel/python-project-stub Author:
 Jacob Striebel Author-email: jacob.striebel@example.com License: MIT Project-
 URL: Homepage, https://github.com/striebel/python-project-stub Description-
 Content-Type: text/markdown License-File: LICENSE # `python-project-stub`_[_P_y_P_I_]
 _[_D_o_w_n_l_o_a_d_s_]_[_L_i_c_e_n_s_e_]
```

