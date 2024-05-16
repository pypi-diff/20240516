# Comparing `tmp/naimco-0.1.0.tar.gz` & `tmp/naimco-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naimco-0.1.0.tar", max compression
+gzip compressed data, was "naimco-0.1.1.tar", max compression
```

## Comparing `naimco-0.1.0.tar` & `naimco-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1082 2024-05-02 14:22:16.396847 naimco-0.1.0/LICENSE
--rw-r--r--   0        0        0     1604 2024-05-02 14:22:16.396847 naimco-0.1.0/README.rst
--rw-r--r--   0        0        0      357 2024-05-02 14:22:16.396847 naimco-0.1.0/naimco/__init__.py
--rw-r--r--   0        0        0     2116 2024-05-02 14:22:16.396847 naimco-0.1.0/naimco/connection.py
--rw-r--r--   0        0        0    16178 2024-05-02 14:22:16.396847 naimco-0.1.0/naimco/controllers.py
--rw-r--r--   0        0        0     9378 2024-05-02 14:22:16.396847 naimco-0.1.0/naimco/core.py
--rw-r--r--   0        0        0     3995 2024-05-02 14:22:16.400847 naimco-0.1.0/naimco/msg_processing.py
--rw-r--r--   0        0        0     1580 2024-05-02 14:22:16.400847 naimco-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2540 1970-01-01 00:00:00.000000 naimco-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-05-16 15:49:46.600011 naimco-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1604 2024-05-16 15:49:46.600011 naimco-0.1.1/README.rst
+-rw-r--r--   0        0        0      357 2024-05-16 15:49:46.600011 naimco-0.1.1/naimco/__init__.py
+-rw-r--r--   0        0        0     2116 2024-05-16 15:49:46.600011 naimco-0.1.1/naimco/connection.py
+-rw-r--r--   0        0        0    16178 2024-05-16 15:49:46.600011 naimco-0.1.1/naimco/controllers.py
+-rw-r--r--   0        0        0     9378 2024-05-16 15:49:46.600011 naimco-0.1.1/naimco/core.py
+-rw-r--r--   0        0        0     3995 2024-05-16 15:49:46.600011 naimco-0.1.1/naimco/msg_processing.py
+-rw-r--r--   0        0        0     1559 2024-05-16 15:49:46.600011 naimco-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2420 1970-01-01 00:00:00.000000 naimco-0.1.1/PKG-INFO
```

### Comparing `naimco-0.1.0/LICENSE` & `naimco-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `naimco-0.1.0/README.rst` & `naimco-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `naimco-0.1.0/naimco/connection.py` & `naimco-0.1.1/naimco/connection.py`

 * *Files identical despite different names*

### Comparing `naimco-0.1.0/naimco/controllers.py` & `naimco-0.1.1/naimco/controllers.py`

 * *Files identical despite different names*

### Comparing `naimco-0.1.0/naimco/core.py` & `naimco-0.1.1/naimco/core.py`

 * *Files identical despite different names*

### Comparing `naimco-0.1.0/naimco/msg_processing.py` & `naimco-0.1.1/naimco/msg_processing.py`

 * *Files identical despite different names*

### Comparing `naimco-0.1.0/pyproject.toml` & `naimco-0.1.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "naimco"
-version = "0.1.0"
+version = "0.1.1"
 description = "Package to control Naim Mu-so sound systems"
 authors = ["Yngvi Þór Sigurjónsson <blitzkopf@gmail.com>"]
 readme = "README.rst"
 license = "MIT"
 homepage = "https://github.com/blitzkopf/NaimCo"
 repository = "https://github.com/blitzkopf/NaimCo"
 keywords = ["naim", "mu-so", "homeassistant"]
@@ -13,24 +13,23 @@
     "Topic :: Home Automation",
     "Topic :: Multimedia :: Sound/Audio :: Players",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 asyncio = "^3.4.3"
-ruff = ">=0.3.4,<0.5.0"
-logging = "^0.4.9.6"
 argparse = "^1.4.0"
-pytest = "^8.2.0"
 
 [tool.poetry.scripts]
 naim_control = "scripts.naim_control:main"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.7.0"
+ruff = ">=0.3.4,<0.5.0"
+pytest = "^8.2.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 skip-string-normalization = true
```

### Comparing `naimco-0.1.0/PKG-INFO` & `naimco-0.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naimco
-Version: 0.1.0
+Version: 0.1.1
 Summary: Package to control Naim Mu-so sound systems
 Home-page: https://github.com/blitzkopf/NaimCo
 License: MIT
 Keywords: naim,mu-so,homeassistant
 Author: Yngvi Þór Sigurjónsson
 Author-email: blitzkopf@gmail.com
 Requires-Python: >=3.11,<4.0
@@ -13,17 +13,14 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Home Automation
 Classifier: Topic :: Multimedia :: Sound/Audio :: Players
 Requires-Dist: argparse (>=1.4.0,<2.0.0)
 Requires-Dist: asyncio (>=3.4.3,<4.0.0)
-Requires-Dist: logging (>=0.4.9.6,<0.5.0.0)
-Requires-Dist: pytest (>=8.2.0,<9.0.0)
-Requires-Dist: ruff (>=0.3.4,<0.5.0)
 Project-URL: Repository, https://github.com/blitzkopf/NaimCo
 Description-Content-Type: text/x-rst
 
 
 NaimCo
 ======
 NaimCo (NaimController) is package to control Naim Mu-so sound systems.
```

