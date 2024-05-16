# Comparing `tmp/gpt-repository-loader-0.1.7.tar.gz` & `tmp/gpt-repository-loader-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-repository-loader-0.1.7.tar", last modified: Sun Mar 19 08:43:32 2023, max compression
+gzip compressed data, was "gpt-repository-loader-0.9.0.tar", last modified: Thu May 16 17:53:09 2024, max compression
```

## Comparing `gpt-repository-loader-0.1.7.tar` & `gpt-repository-loader-0.9.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 harshwork   (502) staff       (20)        0 2023-03-19 08:43:32.410559 gpt-repository-loader-0.1.7/
--rw-r--r--   0 harshwork   (502) staff       (20)     1066 2023-03-17 08:40:06.000000 gpt-repository-loader-0.1.7/LICENSE
--rw-r--r--   0 harshwork   (502) staff       (20)     3288 2023-03-19 08:43:32.410411 gpt-repository-loader-0.1.7/PKG-INFO
--rw-r--r--   0 harshwork   (502) staff       (20)     2517 2023-03-19 08:30:02.000000 gpt-repository-loader-0.1.7/README.md
-drwxr-xr-x   0 harshwork   (502) staff       (20)        0 2023-03-19 08:43:32.409551 gpt-repository-loader-0.1.7/gpt_repository_loader/
--rw-r--r--   0 harshwork   (502) staff       (20)       57 2023-03-19 08:30:02.000000 gpt-repository-loader-0.1.7/gpt_repository_loader/__init__.py
--rwxr-xr-x   0 harshwork   (502) staff       (20)     3030 2023-03-19 08:41:54.000000 gpt-repository-loader-0.1.7/gpt_repository_loader/gpt_repository_loader.py
-drwxr-xr-x   0 harshwork   (502) staff       (20)        0 2023-03-19 08:43:32.410241 gpt-repository-loader-0.1.7/gpt_repository_loader.egg-info/
--rw-r--r--   0 harshwork   (502) staff       (20)     3288 2023-03-19 08:43:32.000000 gpt-repository-loader-0.1.7/gpt_repository_loader.egg-info/PKG-INFO
--rw-r--r--   0 harshwork   (502) staff       (20)      379 2023-03-19 08:43:32.000000 gpt-repository-loader-0.1.7/gpt_repository_loader.egg-info/SOURCES.txt
--rw-r--r--   0 harshwork   (502) staff       (20)        1 2023-03-19 08:43:32.000000 gpt-repository-loader-0.1.7/gpt_repository_loader.egg-info/dependency_links.txt
--rw-r--r--   0 harshwork   (502) staff       (20)       69 2023-03-19 08:43:32.000000 gpt-repository-loader-0.1.7/gpt_repository_loader.egg-info/entry_points.txt
--rw-r--r--   0 harshwork   (502) staff       (20)       10 2023-03-19 08:43:32.000000 gpt-repository-loader-0.1.7/gpt_repository_loader.egg-info/requires.txt
--rw-r--r--   0 harshwork   (502) staff       (20)       22 2023-03-19 08:43:32.000000 gpt-repository-loader-0.1.7/gpt_repository_loader.egg-info/top_level.txt
--rw-r--r--   0 harshwork   (502) staff       (20)       38 2023-03-19 08:43:32.410603 gpt-repository-loader-0.1.7/setup.cfg
--rwxr-xr-x   0 harshwork   (502) staff       (20)     1176 2023-03-19 08:42:46.000000 gpt-repository-loader-0.1.7/setup.py
+drwxr-xr-x   0 harshwork   (502) staff       (20)        0 2024-05-16 17:53:09.172155 gpt-repository-loader-0.9.0/
+-rw-r--r--   0 harshwork   (502) staff       (20)     1066 2023-03-17 08:40:06.000000 gpt-repository-loader-0.9.0/LICENSE
+-rw-r--r--   0 harshwork   (502) staff       (20)     3313 2024-05-16 17:53:09.171867 gpt-repository-loader-0.9.0/PKG-INFO
+-rw-r--r--   0 harshwork   (502) staff       (20)     2517 2023-03-23 06:58:13.000000 gpt-repository-loader-0.9.0/README.md
+drwxr-xr-x   0 harshwork   (502) staff       (20)        0 2024-05-16 17:53:09.170168 gpt-repository-loader-0.9.0/gpt_repository_loader/
+-rw-r--r--   0 harshwork   (502) staff       (20)      100 2023-03-21 06:32:35.000000 gpt-repository-loader-0.9.0/gpt_repository_loader/__init__.py
+-rwxr-xr-x   0 harshwork   (502) staff       (20)     4337 2024-05-16 17:46:08.000000 gpt-repository-loader-0.9.0/gpt_repository_loader/gpt_repository_loader.py
+drwxr-xr-x   0 harshwork   (502) staff       (20)        0 2024-05-16 17:53:09.171566 gpt-repository-loader-0.9.0/gpt_repository_loader.egg-info/
+-rw-r--r--   0 harshwork   (502) staff       (20)     3313 2024-05-16 17:53:09.000000 gpt-repository-loader-0.9.0/gpt_repository_loader.egg-info/PKG-INFO
+-rw-r--r--   0 harshwork   (502) staff       (20)      379 2024-05-16 17:53:09.000000 gpt-repository-loader-0.9.0/gpt_repository_loader.egg-info/SOURCES.txt
+-rw-r--r--   0 harshwork   (502) staff       (20)        1 2024-05-16 17:53:09.000000 gpt-repository-loader-0.9.0/gpt_repository_loader.egg-info/dependency_links.txt
+-rw-r--r--   0 harshwork   (502) staff       (20)       69 2024-05-16 17:53:09.000000 gpt-repository-loader-0.9.0/gpt_repository_loader.egg-info/entry_points.txt
+-rw-r--r--   0 harshwork   (502) staff       (20)       10 2024-05-16 17:53:09.000000 gpt-repository-loader-0.9.0/gpt_repository_loader.egg-info/requires.txt
+-rw-r--r--   0 harshwork   (502) staff       (20)       22 2024-05-16 17:53:09.000000 gpt-repository-loader-0.9.0/gpt_repository_loader.egg-info/top_level.txt
+-rw-r--r--   0 harshwork   (502) staff       (20)       38 2024-05-16 17:53:09.172209 gpt-repository-loader-0.9.0/setup.cfg
+-rwxr-xr-x   0 harshwork   (502) staff       (20)     1176 2024-05-16 17:49:31.000000 gpt-repository-loader-0.9.0/setup.py
```

### Comparing `gpt-repository-loader-0.1.7/LICENSE` & `gpt-repository-loader-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-repository-loader-0.1.7/PKG-INFO` & `gpt-repository-loader-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-repository-loader
-Version: 0.1.7
+Version: 0.9.0
 Summary: A utility to convert a Git repository into a text representation.
 Home-page: https://github.com/felvin-search/gpt-repository-loader
 Author: Felvin
 Author-email: team@felvin.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pyperclip
 
 # gpt-repository-loader
 
 `gpt-repository-loader` is a command-line tool that converts the contents of a Git repository into a text format, preserving the structure of the files and file contents. The generated output can be interpreted by AI language models, allowing them to process the repository's contents for various tasks, such as code review or documentation generation.
 
 ## Installation & Usage
 `pip install gpt-repository-loader` install the project locally.
```

### Comparing `gpt-repository-loader-0.1.7/README.md` & `gpt-repository-loader-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `gpt-repository-loader-0.1.7/gpt_repository_loader.egg-info/PKG-INFO` & `gpt-repository-loader-0.9.0/gpt_repository_loader.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-repository-loader
-Version: 0.1.7
+Version: 0.9.0
 Summary: A utility to convert a Git repository into a text representation.
 Home-page: https://github.com/felvin-search/gpt-repository-loader
 Author: Felvin
 Author-email: team@felvin.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pyperclip
 
 # gpt-repository-loader
 
 `gpt-repository-loader` is a command-line tool that converts the contents of a Git repository into a text format, preserving the structure of the files and file contents. The generated output can be interpreted by AI language models, allowing them to process the repository's contents for various tasks, such as code review or documentation generation.
 
 ## Installation & Usage
 `pip install gpt-repository-loader` install the project locally.
```

### Comparing `gpt-repository-loader-0.1.7/setup.py` & `gpt-repository-loader-0.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="gpt-repository-loader",
-    version="0.1.7",
+    version="0.9.0",
     author="Felvin",
     author_email="team@felvin.com",
     description="A utility to convert a Git repository into a text representation.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/felvin-search/gpt-repository-loader",
     packages=find_packages(),
```

