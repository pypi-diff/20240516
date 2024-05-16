# Comparing `tmp/pynamodb_utils-1.3.7.tar.gz` & `tmp/pynamodb_utils-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynamodb_utils-1.3.7.tar", last modified: Tue Jan 30 17:29:54 2024, max compression
+gzip compressed data, was "pynamodb_utils-1.4.0.tar", last modified: Tue Jan 30 17:28:38 2024, max compression
```

## Comparing `pynamodb_utils-1.3.7.tar` & `pynamodb_utils-1.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 micmur     (501) staff       (20)        0 2024-01-30 17:29:54.426204 pynamodb_utils-1.3.7/
--rw-r--r--   0 micmur     (501) staff       (20)     1073 2022-04-01 12:23:02.000000 pynamodb_utils-1.3.7/LICENSE
--rw-r--r--   0 micmur     (501) staff       (20)     3681 2024-01-30 17:29:54.426270 pynamodb_utils-1.3.7/PKG-INFO
--rw-r--r--   0 micmur     (501) staff       (20)     3115 2024-01-26 16:01:00.000000 pynamodb_utils-1.3.7/README.md
--rw-r--r--   0 micmur     (501) staff       (20)      147 2024-01-30 17:29:54.426493 pynamodb_utils-1.3.7/setup.cfg
--rw-r--r--   0 micmur     (501) staff       (20)     1094 2024-01-30 17:29:24.000000 pynamodb_utils-1.3.7/setup.py
-drwxr-xr-x   0 micmur     (501) staff       (20)        0 2024-01-30 17:29:54.423843 pynamodb_utils-1.3.7/src/
-drwxr-xr-x   0 micmur     (501) staff       (20)        0 2024-01-30 17:29:54.425458 pynamodb_utils-1.3.7/src/pynamodb_utils/
--rw-r--r--   0 micmur     (501) staff       (20)      169 2023-04-19 15:08:53.000000 pynamodb_utils-1.3.7/src/pynamodb_utils/__init__.py
--rw-r--r--   0 micmur     (501) staff       (20)     4111 2024-01-30 17:29:24.000000 pynamodb_utils-1.3.7/src/pynamodb_utils/attributes.py
--rw-r--r--   0 micmur     (501) staff       (20)     3314 2024-01-30 17:19:07.000000 pynamodb_utils-1.3.7/src/pynamodb_utils/conditions.py
--rw-r--r--   0 micmur     (501) staff       (20)      318 2024-01-30 17:19:07.000000 pynamodb_utils-1.3.7/src/pynamodb_utils/exceptions.py
--rw-r--r--   0 micmur     (501) staff       (20)     3751 2024-01-30 17:19:07.000000 pynamodb_utils-1.3.7/src/pynamodb_utils/models.py
--rw-r--r--   0 micmur     (501) staff       (20)     6984 2024-01-30 17:19:07.000000 pynamodb_utils-1.3.7/src/pynamodb_utils/parsers.py
--rw-r--r--   0 micmur     (501) staff       (20)     4836 2023-08-11 10:47:24.000000 pynamodb_utils-1.3.7/src/pynamodb_utils/serializers.py
--rw-r--r--   0 micmur     (501) staff       (20)     3853 2024-01-30 17:19:07.000000 pynamodb_utils-1.3.7/src/pynamodb_utils/utils.py
-drwxr-xr-x   0 micmur     (501) staff       (20)        0 2024-01-30 17:29:54.426088 pynamodb_utils-1.3.7/src/pynamodb_utils.egg-info/
--rw-r--r--   0 micmur     (501) staff       (20)     3681 2024-01-30 17:29:54.000000 pynamodb_utils-1.3.7/src/pynamodb_utils.egg-info/PKG-INFO
--rw-r--r--   0 micmur     (501) staff       (20)      496 2024-01-30 17:29:54.000000 pynamodb_utils-1.3.7/src/pynamodb_utils.egg-info/SOURCES.txt
--rw-r--r--   0 micmur     (501) staff       (20)        1 2024-01-30 17:29:54.000000 pynamodb_utils-1.3.7/src/pynamodb_utils.egg-info/dependency_links.txt
--rw-r--r--   0 micmur     (501) staff       (20)       23 2024-01-30 17:29:54.000000 pynamodb_utils-1.3.7/src/pynamodb_utils.egg-info/requires.txt
--rw-r--r--   0 micmur     (501) staff       (20)       15 2024-01-30 17:29:54.000000 pynamodb_utils-1.3.7/src/pynamodb_utils.egg-info/top_level.txt
+drwxr-xr-x   0 micmur     (501) staff       (20)        0 2024-01-30 17:28:38.980183 pynamodb_utils-1.4.0/
+-rw-r--r--   0 micmur     (501) staff       (20)     1073 2022-04-01 12:23:02.000000 pynamodb_utils-1.4.0/LICENSE
+-rw-r--r--   0 micmur     (501) staff       (20)     3681 2024-01-30 17:28:38.980260 pynamodb_utils-1.4.0/PKG-INFO
+-rw-r--r--   0 micmur     (501) staff       (20)     3115 2024-01-26 16:01:00.000000 pynamodb_utils-1.4.0/README.md
+-rw-r--r--   0 micmur     (501) staff       (20)      147 2024-01-30 17:28:38.980490 pynamodb_utils-1.4.0/setup.cfg
+-rw-r--r--   0 micmur     (501) staff       (20)     1094 2024-01-30 17:22:35.000000 pynamodb_utils-1.4.0/setup.py
+drwxr-xr-x   0 micmur     (501) staff       (20)        0 2024-01-30 17:28:38.977721 pynamodb_utils-1.4.0/src/
+drwxr-xr-x   0 micmur     (501) staff       (20)        0 2024-01-30 17:28:38.979411 pynamodb_utils-1.4.0/src/pynamodb_utils/
+-rw-r--r--   0 micmur     (501) staff       (20)      169 2023-04-19 15:08:53.000000 pynamodb_utils-1.4.0/src/pynamodb_utils/__init__.py
+-rw-r--r--   0 micmur     (501) staff       (20)     5153 2024-01-30 17:21:13.000000 pynamodb_utils-1.4.0/src/pynamodb_utils/attributes.py
+-rw-r--r--   0 micmur     (501) staff       (20)     3314 2024-01-30 17:19:07.000000 pynamodb_utils-1.4.0/src/pynamodb_utils/conditions.py
+-rw-r--r--   0 micmur     (501) staff       (20)      318 2024-01-30 17:19:07.000000 pynamodb_utils-1.4.0/src/pynamodb_utils/exceptions.py
+-rw-r--r--   0 micmur     (501) staff       (20)     3751 2024-01-30 17:19:07.000000 pynamodb_utils-1.4.0/src/pynamodb_utils/models.py
+-rw-r--r--   0 micmur     (501) staff       (20)     6984 2024-01-30 17:19:07.000000 pynamodb_utils-1.4.0/src/pynamodb_utils/parsers.py
+-rw-r--r--   0 micmur     (501) staff       (20)     4836 2023-08-11 10:47:24.000000 pynamodb_utils-1.4.0/src/pynamodb_utils/serializers.py
+-rw-r--r--   0 micmur     (501) staff       (20)     3853 2024-01-30 17:19:07.000000 pynamodb_utils-1.4.0/src/pynamodb_utils/utils.py
+drwxr-xr-x   0 micmur     (501) staff       (20)        0 2024-01-30 17:28:38.980053 pynamodb_utils-1.4.0/src/pynamodb_utils.egg-info/
+-rw-r--r--   0 micmur     (501) staff       (20)     3681 2024-01-30 17:28:38.000000 pynamodb_utils-1.4.0/src/pynamodb_utils.egg-info/PKG-INFO
+-rw-r--r--   0 micmur     (501) staff       (20)      496 2024-01-30 17:28:38.000000 pynamodb_utils-1.4.0/src/pynamodb_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 micmur     (501) staff       (20)        1 2024-01-30 17:28:38.000000 pynamodb_utils-1.4.0/src/pynamodb_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 micmur     (501) staff       (20)       23 2024-01-30 17:28:38.000000 pynamodb_utils-1.4.0/src/pynamodb_utils.egg-info/requires.txt
+-rw-r--r--   0 micmur     (501) staff       (20)       15 2024-01-30 17:28:38.000000 pynamodb_utils-1.4.0/src/pynamodb_utils.egg-info/top_level.txt
```

### Comparing `pynamodb_utils-1.3.7/LICENSE` & `pynamodb_utils-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynamodb_utils-1.3.7/PKG-INFO` & `pynamodb_utils-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynamodb_utils
-Version: 1.3.7
+Version: 1.4.0
 Summary: Utilities package for pynamodb.
 Home-page: https://github.com/micmurawski/pynamodb-utils/
 Author: Michal Murawski
 Author-email: mmurawski777@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pynamodb_utils-1.3.7/README.md` & `pynamodb_utils-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pynamodb_utils-1.3.7/setup.py` & `pynamodb_utils-1.4.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,30 +8,30 @@
 
 def read(*parts):
     return codecs.open(os.path.join(HERE, *parts), "r").read()
 
 
 setup(
     name="pynamodb_utils",
-    version="1.3.7",
+    version="1.4.0",
     author="Michal Murawski",
     author_email="mmurawski777@gmail.com",
     description="Utilities package for pynamodb.",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     url="https://github.com/micmurawski/pynamodb-utils/",
     package_dir={"": "src"},
     packages=find_packages(
         where="./src",
         exclude=(
             'build',
             'tests',
         )
     ),
-    install_requires=["pynamodb>=5.0.0,<6.0.0"],
+    install_requires=["pynamodb>=6.0.0,<7.0.0"],
     include_package_data=True,
     python_requires=">=3.6",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
```

### Comparing `pynamodb_utils-1.3.7/src/pynamodb_utils/conditions.py` & `pynamodb_utils-1.4.0/src/pynamodb_utils/conditions.py`

 * *Files identical despite different names*

### Comparing `pynamodb_utils-1.3.7/src/pynamodb_utils/models.py` & `pynamodb_utils-1.4.0/src/pynamodb_utils/models.py`

 * *Files identical despite different names*

### Comparing `pynamodb_utils-1.3.7/src/pynamodb_utils/parsers.py` & `pynamodb_utils-1.4.0/src/pynamodb_utils/parsers.py`

 * *Files identical despite different names*

### Comparing `pynamodb_utils-1.3.7/src/pynamodb_utils/serializers.py` & `pynamodb_utils-1.4.0/src/pynamodb_utils/serializers.py`

 * *Files identical despite different names*

### Comparing `pynamodb_utils-1.3.7/src/pynamodb_utils/utils.py` & `pynamodb_utils-1.4.0/src/pynamodb_utils/utils.py`

 * *Files identical despite different names*

### Comparing `pynamodb_utils-1.3.7/src/pynamodb_utils.egg-info/PKG-INFO` & `pynamodb_utils-1.4.0/src/pynamodb_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynamodb-utils
-Version: 1.3.7
+Version: 1.4.0
 Summary: Utilities package for pynamodb.
 Home-page: https://github.com/micmurawski/pynamodb-utils/
 Author: Michal Murawski
 Author-email: mmurawski777@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

