# Comparing `tmp/mikoblocks-0.1.0.tar.gz` & `tmp/mikoblocks-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mikoblocks-0.1.0.tar", last modified: Thu May 16 05:18:48 2024, max compression
+gzip compressed data, was "mikoblocks-0.1.1.tar", last modified: Thu May 16 05:40:42 2024, max compression
```

## Comparing `mikoblocks-0.1.0.tar` & `mikoblocks-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 05:18:48.961105 mikoblocks-0.1.0/
--rw-rw-rw-   0        0        0     1115 2024-05-16 04:50:54.000000 mikoblocks-0.1.0/LICENSE.md
--rw-rw-rw-   0        0        0     3275 2024-05-16 05:18:48.960104 mikoblocks-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2322 2024-05-16 05:04:48.000000 mikoblocks-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 05:18:48.946592 mikoblocks-0.1.0/mikoblocks/
--rw-rw-rw-   0        0        0     2215 2024-04-23 03:42:37.000000 mikoblocks-0.1.0/mikoblocks/__init__.py
--rw-rw-rw-   0        0        0      329 2024-05-16 04:53:31.000000 mikoblocks-0.1.0/mikoblocks/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-16 05:18:48.959108 mikoblocks-0.1.0/mikoblocks.egg-info/
--rw-rw-rw-   0        0        0     3275 2024-05-16 05:18:48.000000 mikoblocks-0.1.0/mikoblocks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2024-05-16 05:18:48.000000 mikoblocks-0.1.0/mikoblocks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 05:18:48.000000 mikoblocks-0.1.0/mikoblocks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-16 05:18:48.000000 mikoblocks-0.1.0/mikoblocks.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1094 2024-05-16 05:18:42.000000 mikoblocks-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-16 05:18:48.961105 mikoblocks-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-16 05:40:42.130952 mikoblocks-0.1.1/
+-rw-rw-rw-   0        0        0     1115 2024-05-16 04:50:54.000000 mikoblocks-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     4470 2024-05-16 05:40:42.127956 mikoblocks-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2322 2024-05-16 05:04:48.000000 mikoblocks-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 05:40:42.111923 mikoblocks-0.1.1/mikoblocks/
+-rw-rw-rw-   0        0        0     2215 2024-04-23 03:42:37.000000 mikoblocks-0.1.1/mikoblocks/__init__.py
+-rw-rw-rw-   0        0        0      329 2024-05-16 04:53:31.000000 mikoblocks-0.1.1/mikoblocks/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-16 05:40:42.126944 mikoblocks-0.1.1/mikoblocks.egg-info/
+-rw-rw-rw-   0        0        0     4470 2024-05-16 05:40:42.000000 mikoblocks-0.1.1/mikoblocks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      211 2024-05-16 05:40:42.000000 mikoblocks-0.1.1/mikoblocks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 05:40:42.000000 mikoblocks-0.1.1/mikoblocks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-16 05:40:42.000000 mikoblocks-0.1.1/mikoblocks.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1094 2024-05-16 05:40:31.000000 mikoblocks-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-16 05:40:42.130952 mikoblocks-0.1.1/setup.cfg
```

### Comparing `mikoblocks-0.1.0/LICENSE.md` & `mikoblocks-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mikoblocks-0.1.0/PKG-INFO` & `mikoblocks-0.1.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: mikoblocks
-Version: 0.1.0
-Summary: Mikoblocks is a minimal library to programmatically generate html. It is unopinionated and outputs pure html code. Do to a small simple syntax the programming is much easier and clearer to type compared to html. It allows assembling of component -blocks- which can nest further components within, allowing complex reusable pieces to be shared across pages and projects.
-Author-email: Alex Stevovich <alex.stevovich@gmail.com>
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: Other/Proprietary License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 Mikoblocks is a minimal library to programmatically generate html. It is unopinionated and outputs pure html code and due to a small simple syntax the programming is much easier and clearer to type compared to html. It allows assembling of component "blocks" which can nest further components within, allowing complex reusable pieces to be shared across pages and projects.
 
 ``` javascript
 const { Block } = import('mikoblocks');
 
 class MikoblocksExamplePage extends Block {
```

### Comparing `mikoblocks-0.1.0/mikoblocks/__init__.py` & `mikoblocks-0.1.1/mikoblocks/__init__.py`

 * *Files identical despite different names*

### Comparing `mikoblocks-0.1.0/pyproject.toml` & `mikoblocks-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mikoblocks"
-version = "0.1.0"
+version = "0.1.1"
 description = "Mikoblocks is a minimal library to programmatically generate html. It is unopinionated and outputs pure html code. Do to a small simple syntax the programming is much easier and clearer to type compared to html. It allows assembling of component -blocks- which can nest further components within, allowing complex reusable pieces to be shared across pages and projects."
 authors = [{ name = "Alex Stevovich", email = "alex.stevovich@gmail.com" }]
 license = {file = "LICENSE"}
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
```

