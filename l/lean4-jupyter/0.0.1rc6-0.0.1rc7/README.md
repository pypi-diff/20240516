# Comparing `tmp/lean4_jupyter-0.0.1rc6.tar.gz` & `tmp/lean4_jupyter-0.0.1rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lean4_jupyter-0.0.1rc6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lean4_jupyter-0.0.1rc7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lean4_jupyter-0.0.1rc6.tar` & `lean4_jupyter-0.0.1rc7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0       30 2024-05-16 10:21:08.557007 lean4_jupyter-0.0.1rc6/.flake8
--rw-r--r--   0        0        0     2031 2024-05-16 10:21:08.557007 lean4_jupyter-0.0.1rc6/.github/workflows/ci.yml
--rw-r--r--   0        0        0     3096 2024-05-16 10:21:08.557007 lean4_jupyter-0.0.1rc6/.gitignore
--rw-r--r--   0        0        0     1064 2024-05-16 10:21:08.557007 lean4_jupyter-0.0.1rc6/LICENSE
--rw-r--r--   0        0        0     4350 2024-05-16 10:21:08.557007 lean4_jupyter-0.0.1rc6/README.md
--rw-r--r--   0        0        0    67337 2024-05-16 10:21:08.557007 lean4_jupyter-0.0.1rc6/examples/00_tutorial.ipynb
--rw-r--r--   0        0        0    11782 2024-05-16 10:21:08.557007 lean4_jupyter-0.0.1rc6/examples/01_cd.ipynb
--rw-r--r--   0        0        0    19404 2024-05-16 10:21:08.557007 lean4_jupyter-0.0.1rc6/examples/02_load.ipynb
--rw-r--r--   0        0        0    35042 2024-05-16 10:21:08.557007 lean4_jupyter-0.0.1rc6/examples/03_import.ipynb
--rw-r--r--   0        0        0        7 2024-05-16 10:21:08.557007 lean4_jupyter-0.0.1rc6/examples/demo_proj/.gitignore
--rw-r--r--   0        0        0      154 2024-05-16 10:21:08.557007 lean4_jupyter-0.0.1rc6/examples/demo_proj/DemoProj.lean
--rw-r--r--   0        0        0       37 2024-05-16 10:21:08.557007 lean4_jupyter-0.0.1rc6/examples/demo_proj/DemoProj/Basic.lean
--rw-r--r--   0        0        0       70 2024-05-16 10:21:08.557007 lean4_jupyter-0.0.1rc6/examples/demo_proj/DemoProj/Standalone.lean
--rw-r--r--   0        0        0     2171 2024-05-16 10:21:08.557007 lean4_jupyter-0.0.1rc6/examples/demo_proj/lake-manifest.json
--rw-r--r--   0        0        0      505 2024-05-16 10:21:08.557007 lean4_jupyter-0.0.1rc6/examples/demo_proj/lakefile.lean
--rw-r--r--   0        0        0       28 2024-05-16 10:21:08.557007 lean4_jupyter-0.0.1rc6/examples/demo_proj/lean-toolchain
--rw-r--r--   0        0        0    11222 2024-05-16 10:21:08.561007 lean4_jupyter-0.0.1rc6/examples/repl-issue-40-dup-msg.ipynb
--rw-r--r--   0        0        0    10532 2024-05-16 10:21:08.561007 lean4_jupyter-0.0.1rc6/examples/repl-issue-40-dup-sorries.ipynb
--rw-r--r--   0        0        0       91 2024-05-16 10:21:08.561007 lean4_jupyter-0.0.1rc6/lean4_jupyter/__init__.py
--rw-r--r--   0        0        0      129 2024-05-16 10:21:08.561007 lean4_jupyter-0.0.1rc6/lean4_jupyter/__main__.py
--rw-r--r--   0        0        0     9058 2024-05-16 10:21:08.561007 lean4_jupyter-0.0.1rc6/lean4_jupyter/display.py
--rw-r--r--   0        0        0     2134 2024-05-16 10:21:08.561007 lean4_jupyter-0.0.1rc6/lean4_jupyter/install.py
--rw-r--r--   0        0        0     3251 2024-05-16 10:21:08.561007 lean4_jupyter-0.0.1rc6/lean4_jupyter/kernel.py
--rw-r--r--   0        0        0     7359 2024-05-16 10:21:08.561007 lean4_jupyter-0.0.1rc6/lean4_jupyter/repl.py
--rw-r--r--   0        0        0       86 2024-05-16 10:21:08.561007 lean4_jupyter-0.0.1rc6/lean4_jupyter/resources/__init__.py
--rw-r--r--   0        0        0    11263 2024-05-16 10:21:08.561007 lean4_jupyter-0.0.1rc6/lean4_jupyter/resources/lean_logo.svg
--rw-r--r--   0        0        0      657 2024-05-16 10:21:08.561007 lean4_jupyter-0.0.1rc6/pyproject.toml
--rw-r--r--   0        0        0      602 1970-01-01 00:00:00.000000 lean4_jupyter-0.0.1rc6/setup.py
--rw-r--r--   0        0        0     4922 1970-01-01 00:00:00.000000 lean4_jupyter-0.0.1rc6/PKG-INFO
+-rw-r--r--   0        0        0       30 2024-05-16 10:37:33.849804 lean4_jupyter-0.0.1rc7/.flake8
+-rw-r--r--   0        0        0     2031 2024-05-16 10:37:33.849804 lean4_jupyter-0.0.1rc7/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     3096 2024-05-16 10:37:33.849804 lean4_jupyter-0.0.1rc7/.gitignore
+-rw-r--r--   0        0        0     1069 2024-05-16 10:37:33.849804 lean4_jupyter-0.0.1rc7/LICENSE
+-rw-r--r--   0        0        0     5034 2024-05-16 10:37:33.849804 lean4_jupyter-0.0.1rc7/README.md
+-rw-r--r--   0        0        0    67337 2024-05-16 10:37:33.853804 lean4_jupyter-0.0.1rc7/examples/00_tutorial.ipynb
+-rw-r--r--   0        0        0    11782 2024-05-16 10:37:33.853804 lean4_jupyter-0.0.1rc7/examples/01_cd.ipynb
+-rw-r--r--   0        0        0    19404 2024-05-16 10:37:33.853804 lean4_jupyter-0.0.1rc7/examples/02_load.ipynb
+-rw-r--r--   0        0        0    35042 2024-05-16 10:37:33.853804 lean4_jupyter-0.0.1rc7/examples/03_import.ipynb
+-rw-r--r--   0        0        0        7 2024-05-16 10:37:33.853804 lean4_jupyter-0.0.1rc7/examples/demo_proj/.gitignore
+-rw-r--r--   0        0        0      154 2024-05-16 10:37:33.853804 lean4_jupyter-0.0.1rc7/examples/demo_proj/DemoProj.lean
+-rw-r--r--   0        0        0       37 2024-05-16 10:37:33.853804 lean4_jupyter-0.0.1rc7/examples/demo_proj/DemoProj/Basic.lean
+-rw-r--r--   0        0        0       70 2024-05-16 10:37:33.853804 lean4_jupyter-0.0.1rc7/examples/demo_proj/DemoProj/Standalone.lean
+-rw-r--r--   0        0        0     2171 2024-05-16 10:37:33.853804 lean4_jupyter-0.0.1rc7/examples/demo_proj/lake-manifest.json
+-rw-r--r--   0        0        0      505 2024-05-16 10:37:33.853804 lean4_jupyter-0.0.1rc7/examples/demo_proj/lakefile.lean
+-rw-r--r--   0        0        0       28 2024-05-16 10:37:33.853804 lean4_jupyter-0.0.1rc7/examples/demo_proj/lean-toolchain
+-rw-r--r--   0        0        0    11222 2024-05-16 10:37:33.853804 lean4_jupyter-0.0.1rc7/examples/repl-issue-40-dup-msg.ipynb
+-rw-r--r--   0        0        0    10532 2024-05-16 10:37:33.853804 lean4_jupyter-0.0.1rc7/examples/repl-issue-40-dup-sorries.ipynb
+-rw-r--r--   0        0        0       91 2024-05-16 10:37:33.853804 lean4_jupyter-0.0.1rc7/lean4_jupyter/__init__.py
+-rw-r--r--   0        0        0      129 2024-05-16 10:37:33.853804 lean4_jupyter-0.0.1rc7/lean4_jupyter/__main__.py
+-rw-r--r--   0        0        0     9058 2024-05-16 10:37:33.853804 lean4_jupyter-0.0.1rc7/lean4_jupyter/display.py
+-rw-r--r--   0        0        0     2134 2024-05-16 10:37:33.853804 lean4_jupyter-0.0.1rc7/lean4_jupyter/install.py
+-rw-r--r--   0        0        0     3251 2024-05-16 10:37:33.853804 lean4_jupyter-0.0.1rc7/lean4_jupyter/kernel.py
+-rw-r--r--   0        0        0     7359 2024-05-16 10:37:33.853804 lean4_jupyter-0.0.1rc7/lean4_jupyter/repl.py
+-rw-r--r--   0        0        0       86 2024-05-16 10:37:33.853804 lean4_jupyter-0.0.1rc7/lean4_jupyter/resources/__init__.py
+-rw-r--r--   0        0        0    11263 2024-05-16 10:37:33.853804 lean4_jupyter-0.0.1rc7/lean4_jupyter/resources/lean_logo.svg
+-rw-r--r--   0        0        0      728 2024-05-16 10:37:33.853804 lean4_jupyter-0.0.1rc7/pyproject.toml
+-rw-r--r--   0        0        0      602 1970-01-01 00:00:00.000000 lean4_jupyter-0.0.1rc7/setup.py
+-rw-r--r--   0        0        0     5650 1970-01-01 00:00:00.000000 lean4_jupyter-0.0.1rc7/PKG-INFO
```

### Comparing `lean4_jupyter-0.0.1rc6/.github/workflows/ci.yml` & `lean4_jupyter-0.0.1rc7/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `lean4_jupyter-0.0.1rc6/.gitignore` & `lean4_jupyter-0.0.1rc7/.gitignore`

 * *Files identical despite different names*

### Comparing `lean4_jupyter-0.0.1rc6/README.md` & `lean4_jupyter-0.0.1rc7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,35 @@
+Metadata-Version: 2.1
+Name: lean4_jupyter
+Version: 0.0.1rc7
+Summary: lean4_jupyter: A Lean 4 Jupyter kernel via REPL
+Author-email: Utensil Song <utensilcandel@gmail.com>
+Description-Content-Type: text/markdown
+Classifier: Framework :: Jupyter
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Development Status :: 3 - Alpha
+Requires-Dist: pexpect (>=4.0)
+Requires-Dist: ipykernel
+Requires-Dist: alectryon
+Project-URL: Source, https://github.com/utensil/lean4_jupyter
+
 # lean4_jupyter
 
 A Lean 4 Jupyter kernel via [repl](https://github.com/leanprover-community/repl).
 
+[![PyPI](https://img.shields.io/pypi/v/lean4_jupyter.svg)](https://pypi.org/project/lean4_jupyter/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/lean4_jupyter.svg)](https://pypi.org/project/lean4_jupyter/)
+![PyPI - License](https://img.shields.io/pypi/l/lean4_jupyter)
+![PyPI - Status](https://img.shields.io/pypi/status/lean4_jupyter)
+[![Python CI](https://github.com/utensil/lean4_jupyter/actions/workflows/ci.yml/badge.svg)](https://github.com/utensil/lean4_jupyter/actions/workflows/ci.yml)
+[![Maintainability](https://api.codeclimate.com/v1/badges/666a7d45d436a598df2b/maintainability)](https://codeclimate.com/github/utensil/lean4_jupyter/maintainability) 
+
 ## Status
 
 Alpha.
 
 ## What's already working
 
 🔥 See it in action: [Tutorial notebook](https://nbviewer.org/github/utensil/lean4_jupyter/blob/main/examples/00_tutorial.ipynb?flush_cache=true).
@@ -115,7 +139,8 @@
 - [Making simple Python wrapper kernels](https://jupyter-client.readthedocs.io/en/stable/wrapperkernels.html)
 - [bash_kernel](https://github.com/takluyver/bash_kernel)
 - [pySagredo](https://github.com/zhangir-azerbayev/pySagredo) (see also [repl#5](https://github.com/leanprover-community/repl/pull/5))
 - [LeanDojo](https://github.com/lean-dojo/LeanDojo)
 - [alectryon](https://github.com/cpitclaudel/alectryon?tab=readme-ov-file#as-a-library)
 - [codespan](https://github.com/brendanzab/codespan)
 - [lean-lsp](https://github.com/utensil/lean-lsp) (My previous attempt to make a Lean 4 Jupyter kernel using Lean 4 LSP server)
+
```

### Comparing `lean4_jupyter-0.0.1rc6/examples/00_tutorial.ipynb` & `lean4_jupyter-0.0.1rc7/examples/00_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `lean4_jupyter-0.0.1rc6/examples/01_cd.ipynb` & `lean4_jupyter-0.0.1rc7/examples/01_cd.ipynb`

 * *Files identical despite different names*

### Comparing `lean4_jupyter-0.0.1rc6/examples/02_load.ipynb` & `lean4_jupyter-0.0.1rc7/examples/02_load.ipynb`

 * *Files identical despite different names*

### Comparing `lean4_jupyter-0.0.1rc6/examples/03_import.ipynb` & `lean4_jupyter-0.0.1rc7/examples/03_import.ipynb`

 * *Files identical despite different names*

### Comparing `lean4_jupyter-0.0.1rc6/examples/demo_proj/lake-manifest.json` & `lean4_jupyter-0.0.1rc7/examples/demo_proj/lake-manifest.json`

 * *Files identical despite different names*

### Comparing `lean4_jupyter-0.0.1rc6/examples/repl-issue-40-dup-msg.ipynb` & `lean4_jupyter-0.0.1rc7/examples/repl-issue-40-dup-msg.ipynb`

 * *Files identical despite different names*

### Comparing `lean4_jupyter-0.0.1rc6/examples/repl-issue-40-dup-sorries.ipynb` & `lean4_jupyter-0.0.1rc7/examples/repl-issue-40-dup-sorries.ipynb`

 * *Files identical despite different names*

### Comparing `lean4_jupyter-0.0.1rc6/lean4_jupyter/display.py` & `lean4_jupyter-0.0.1rc7/lean4_jupyter/display.py`

 * *Files identical despite different names*

### Comparing `lean4_jupyter-0.0.1rc6/lean4_jupyter/install.py` & `lean4_jupyter-0.0.1rc7/lean4_jupyter/install.py`

 * *Files identical despite different names*

### Comparing `lean4_jupyter-0.0.1rc6/lean4_jupyter/kernel.py` & `lean4_jupyter-0.0.1rc7/lean4_jupyter/kernel.py`

 * *Files identical despite different names*

### Comparing `lean4_jupyter-0.0.1rc6/lean4_jupyter/repl.py` & `lean4_jupyter-0.0.1rc7/lean4_jupyter/repl.py`

 * *Files identical despite different names*

### Comparing `lean4_jupyter-0.0.1rc6/lean4_jupyter/resources/lean_logo.svg` & `lean4_jupyter-0.0.1rc7/lean4_jupyter/resources/lean_logo.svg`

 * *Files identical despite different names*

### Comparing `lean4_jupyter-0.0.1rc6/pyproject.toml` & `lean4_jupyter-0.0.1rc7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -10,18 +10,20 @@
 description = "lean4_jupyter: A Lean 4 Jupyter kernel via REPL"
 readme = "README.md"
 dependencies = [
     "pexpect (>=4.0)",
     "ipykernel",
     "alectryon"
 ]
+# https://pypi.org/classifiers/
 classifiers = [
     "Framework :: Jupyter",
-    "License :: OSI Approved :: BSD License",
+    "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Operating System :: MacOS",
-    "Operating System :: POSIX :: Linux"
+    "Operating System :: POSIX :: Linux",
+    "Development Status :: 3 - Alpha"
 ]
 dynamic = ["version"]
 
 [project.urls]
 Source = "https://github.com/utensil/lean4_jupyter"
```

### Comparing `lean4_jupyter-0.0.1rc6/setup.py` & `lean4_jupyter-0.0.1rc7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['pexpect>=4.0', 'ipykernel', 'alectryon']
 
 setup(name='lean4_jupyter',
-      version='0.0.1rc6',
+      version='0.0.1rc7',
       description='lean4_jupyter: A Lean 4 Jupyter kernel via REPL',
       author=None,
       author_email='Utensil Song <utensilcandel@gmail.com>',
       url=None,
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

