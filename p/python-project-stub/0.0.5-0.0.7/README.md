# Comparing `tmp/python_project_stub-0.0.5.tar.gz` & `tmp/python_project_stub-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_project_stub-0.0.5.tar", last modified: Tue May 14 19:32:16 2024, max compression
+gzip compressed data, was "python_project_stub-0.0.7.tar", last modified: Thu May 16 05:48:43 2024, max compression
```

## Comparing `python_project_stub-0.0.5.tar` & `python_project_stub-0.0.7.tar`

### file list

```diff
@@ -1,34 +1,19 @@
-drwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-14 19:32:16.715027 python_project_stub-0.0.5/
--rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)     1544 2024-05-14 19:30:51.000000 python_project_stub-0.0.5/LICENSE
--rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)       43 2024-05-14 19:30:51.000000 python_project_stub-0.0.5/MANIFEST.in
--rw-r--r--   0 jstrieb   (1012) jstrieb   (1012)    17037 2024-05-14 19:32:16.715027 python_project_stub-0.0.5/PKG-INFO
--rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)    16523 2024-05-14 19:30:51.000000 python_project_stub-0.0.5/README.md
--rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)     1530 2024-05-14 19:31:52.000000 python_project_stub-0.0.5/pyproject.toml
-drwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-14 19:32:16.715027 python_project_stub-0.0.5/python_project_stub/
--rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)       82 2024-05-14 19:30:51.000000 python_project_stub-0.0.5/python_project_stub/__init__.py
--rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)     1660 2024-05-14 19:30:51.000000 python_project_stub-0.0.5/python_project_stub/__main__.py
-drwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-14 19:32:16.715027 python_project_stub-0.0.5/python_project_stub/data/
--rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-14 19:30:51.000000 python_project_stub-0.0.5/python_project_stub/data/__init__.py
--rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)       82 2024-05-14 19:30:51.000000 python_project_stub-0.0.5/python_project_stub/data/quote.txt
-drwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-14 19:32:16.715027 python_project_stub-0.0.5/python_project_stub.egg-info/
--rw-r--r--   0 jstrieb   (1012) jstrieb   (1012)    17037 2024-05-14 19:32:16.000000 python_project_stub-0.0.5/python_project_stub.egg-info/PKG-INFO
--rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)      959 2024-05-14 19:32:16.000000 python_project_stub-0.0.5/python_project_stub.egg-info/SOURCES.txt
--rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)        1 2024-05-14 19:32:16.000000 python_project_stub-0.0.5/python_project_stub.egg-info/dependency_links.txt
--rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)       74 2024-05-14 19:32:16.000000 python_project_stub-0.0.5/python_project_stub.egg-info/entry_points.txt
--rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)       41 2024-05-14 19:32:16.000000 python_project_stub-0.0.5/python_project_stub.egg-info/requires.txt
--rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)       59 2024-05-14 19:32:16.000000 python_project_stub-0.0.5/python_project_stub.egg-info/top_level.txt
--rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)      161 2024-05-14 19:32:16.715027 python_project_stub-0.0.5/setup.cfg
-drwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-14 19:32:16.715027 python_project_stub-0.0.5/venv-python-project-stub/
-drwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-14 19:32:16.715027 python_project_stub-0.0.5/venv-python-project-stub/bin/
--rwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)      655 2024-05-12 21:27:02.000000 python_project_stub-0.0.5/venv-python-project-stub/bin/rst2html.py
--rwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)      777 2024-05-12 21:27:02.000000 python_project_stub-0.0.5/venv-python-project-stub/bin/rst2html4.py
--rwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)     1112 2024-05-12 21:27:02.000000 python_project_stub-0.0.5/venv-python-project-stub/bin/rst2html5.py
--rwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)      854 2024-05-12 21:27:02.000000 python_project_stub-0.0.5/venv-python-project-stub/bin/rst2latex.py
--rwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)      677 2024-05-12 21:27:02.000000 python_project_stub-0.0.5/venv-python-project-stub/bin/rst2man.py
--rwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)      843 2024-05-12 21:27:02.000000 python_project_stub-0.0.5/venv-python-project-stub/bin/rst2odt.py
--rwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)      649 2024-05-12 21:27:02.000000 python_project_stub-0.0.5/venv-python-project-stub/bin/rst2odt_prepstyles.py
--rwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)      662 2024-05-12 21:27:02.000000 python_project_stub-0.0.5/venv-python-project-stub/bin/rst2pseudoxml.py
--rwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)      698 2024-05-12 21:27:02.000000 python_project_stub-0.0.5/venv-python-project-stub/bin/rst2s5.py
--rwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)      934 2024-05-12 21:27:02.000000 python_project_stub-0.0.5/venv-python-project-stub/bin/rst2xetex.py
--rwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)      663 2024-05-12 21:27:02.000000 python_project_stub-0.0.5/venv-python-project-stub/bin/rst2xml.py
--rwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)      731 2024-05-12 21:27:02.000000 python_project_stub-0.0.5/venv-python-project-stub/bin/rstpep2html.py
+drwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-16 05:48:43.065907 python_project_stub-0.0.7/
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)     1544 2024-05-15 20:25:30.000000 python_project_stub-0.0.7/LICENSE
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)       43 2024-05-15 20:25:30.000000 python_project_stub-0.0.7/MANIFEST.in
+-rw-r--r--   0 jstrieb   (1012) jstrieb   (1012)    16958 2024-05-16 05:48:43.065907 python_project_stub-0.0.7/PKG-INFO
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)    16523 2024-05-15 20:25:30.000000 python_project_stub-0.0.7/README.md
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)      603 2024-05-16 05:48:41.000000 python_project_stub-0.0.7/pyproject.toml
+drwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-16 05:48:43.065907 python_project_stub-0.0.7/python_project_stub/
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)       82 2024-05-15 20:25:30.000000 python_project_stub-0.0.7/python_project_stub/__init__.py
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)     1660 2024-05-15 20:25:30.000000 python_project_stub-0.0.7/python_project_stub/__main__.py
+drwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-16 05:48:43.065907 python_project_stub-0.0.7/python_project_stub/data/
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-15 20:25:30.000000 python_project_stub-0.0.7/python_project_stub/data/__init__.py
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)       82 2024-05-15 20:25:30.000000 python_project_stub-0.0.7/python_project_stub/data/quote.txt
+drwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-16 05:48:43.065907 python_project_stub-0.0.7/python_project_stub.egg-info/
+-rw-r--r--   0 jstrieb   (1012) jstrieb   (1012)    16958 2024-05-16 05:48:43.000000 python_project_stub-0.0.7/python_project_stub.egg-info/PKG-INFO
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)      408 2024-05-16 05:48:43.000000 python_project_stub-0.0.7/python_project_stub.egg-info/SOURCES.txt
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)        1 2024-05-16 05:48:43.000000 python_project_stub-0.0.7/python_project_stub.egg-info/dependency_links.txt
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)       74 2024-05-16 05:48:43.000000 python_project_stub-0.0.7/python_project_stub.egg-info/entry_points.txt
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)       20 2024-05-16 05:48:43.000000 python_project_stub-0.0.7/python_project_stub.egg-info/top_level.txt
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)      170 2024-05-16 05:48:43.065907 python_project_stub-0.0.7/setup.cfg
```

### Comparing `python_project_stub-0.0.5/LICENSE` & `python_project_stub-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `python_project_stub-0.0.5/PKG-INFO` & `python_project_stub-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: python-project-stub
-Version: 0.0.5
+Version: 0.0.7
 Summary: Stub files to use as the basis of a Python project that can be packaged and uploaded to PyPI
 Home-page: https://github.com/striebel/python-project-stub
 Author: Jacob Striebel
-Author-email: jacob@example.com
-License: BSD 3-Clause License
+Author-email: jacob.striebel@example.com
+License: MIT
 Project-URL: Homepage, https://github.com/striebel/python-project-stub
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy<2.0.0,>=1.0.0
-Requires-Dist: pandas<3.0.0,>=2.0.0
 
 # `python-project-stub`
 
 <a href="https://pypi.org/project/python-project-stub/">
     <img alt="PyPI" src="https://img.shields.io/pypi/v/python-project-stub">
 </a>
 <a href="https://pepy.tech/project/python-project-stub">
```

#### html2text {}

```diff
@@ -1,15 +1,14 @@
-Metadata-Version: 2.1 Name: python-project-stub Version: 0.0.5 Summary: Stub
+Metadata-Version: 2.1 Name: python-project-stub Version: 0.0.7 Summary: Stub
 files to use as the basis of a Python project that can be packaged and uploaded
 to PyPI Home-page: https://github.com/striebel/python-project-stub Author:
-Jacob Striebel Author-email: jacob@example.com License: BSD 3-Clause License
-Project-URL: Homepage, https://github.com/striebel/python-project-stub
-Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-numpy<2.0.0,>=1.0.0 Requires-Dist: pandas<3.0.0,>=2.0.0 # `python-project-stub`
-_[_P_y_P_I_]_[_D_o_w_n_l_o_a_d_s_]_[_L_i_c_e_n_s_e_]
+Jacob Striebel Author-email: jacob.striebel@example.com License: MIT Project-
+URL: Homepage, https://github.com/striebel/python-project-stub Description-
+Content-Type: text/markdown License-File: LICENSE # `python-project-stub`_[_P_y_P_I_]
+_[_D_o_w_n_l_o_a_d_s_]_[_L_i_c_e_n_s_e_]
 
 This repository contains stub files that can be used to create a Python project
 that is able to be packaged and uploaded to the _P_y_t_h_o_n_ _P_a_c_k_a_g_e_ _I_n_d_e_x and hence
 can be conveniently installed with `pip install my-project-name`.
 This README describes how to modify the stub files, using them as the base of a
 new Python project. Requirements are a recent installation of Python 3 on
 Linux.
```

### Comparing `python_project_stub-0.0.5/README.md` & `python_project_stub-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `python_project_stub-0.0.5/python_project_stub/__main__.py` & `python_project_stub-0.0.7/python_project_stub/__main__.py`

 * *Files identical despite different names*

### Comparing `python_project_stub-0.0.5/python_project_stub.egg-info/PKG-INFO` & `python_project_stub-0.0.7/python_project_stub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: python-project-stub
-Version: 0.0.5
+Version: 0.0.7
 Summary: Stub files to use as the basis of a Python project that can be packaged and uploaded to PyPI
 Home-page: https://github.com/striebel/python-project-stub
 Author: Jacob Striebel
-Author-email: jacob@example.com
-License: BSD 3-Clause License
+Author-email: jacob.striebel@example.com
+License: MIT
 Project-URL: Homepage, https://github.com/striebel/python-project-stub
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy<2.0.0,>=1.0.0
-Requires-Dist: pandas<3.0.0,>=2.0.0
 
 # `python-project-stub`
 
 <a href="https://pypi.org/project/python-project-stub/">
     <img alt="PyPI" src="https://img.shields.io/pypi/v/python-project-stub">
 </a>
 <a href="https://pepy.tech/project/python-project-stub">
```

#### html2text {}

```diff
@@ -1,15 +1,14 @@
-Metadata-Version: 2.1 Name: python-project-stub Version: 0.0.5 Summary: Stub
+Metadata-Version: 2.1 Name: python-project-stub Version: 0.0.7 Summary: Stub
 files to use as the basis of a Python project that can be packaged and uploaded
 to PyPI Home-page: https://github.com/striebel/python-project-stub Author:
-Jacob Striebel Author-email: jacob@example.com License: BSD 3-Clause License
-Project-URL: Homepage, https://github.com/striebel/python-project-stub
-Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-numpy<2.0.0,>=1.0.0 Requires-Dist: pandas<3.0.0,>=2.0.0 # `python-project-stub`
-_[_P_y_P_I_]_[_D_o_w_n_l_o_a_d_s_]_[_L_i_c_e_n_s_e_]
+Jacob Striebel Author-email: jacob.striebel@example.com License: MIT Project-
+URL: Homepage, https://github.com/striebel/python-project-stub Description-
+Content-Type: text/markdown License-File: LICENSE # `python-project-stub`_[_P_y_P_I_]
+_[_D_o_w_n_l_o_a_d_s_]_[_L_i_c_e_n_s_e_]
 
 This repository contains stub files that can be used to create a Python project
 that is able to be packaged and uploaded to the _P_y_t_h_o_n_ _P_a_c_k_a_g_e_ _I_n_d_e_x and hence
 can be conveniently installed with `pip install my-project-name`.
 This README describes how to modify the stub files, using them as the base of a
 new Python project. Requirements are a recent installation of Python 3 on
 Linux.
```

