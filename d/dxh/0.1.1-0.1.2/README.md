# Comparing `tmp/dxh-0.1.1.tar.gz` & `tmp/dxh-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxh-0.1.1.tar", last modified: Thu May 16 15:22:56 2024, max compression
+gzip compressed data, was "dxh-0.1.2.tar", last modified: Thu May 16 15:35:39 2024, max compression
```

## Comparing `dxh-0.1.1.tar` & `dxh-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 foysal    (1000) foysal    (1000)        0 2024-05-16 15:22:56.680933 dxh-0.1.1/
--rwxrwxrwx   0 foysal    (1000) foysal    (1000)     1515 2024-05-16 15:22:56.679968 dxh-0.1.1/PKG-INFO
--rwxrwxrwx   0 foysal    (1000) foysal    (1000)      534 2023-10-10 17:48:20.000000 dxh-0.1.1/README.md
-drwxrwxrwx   0 foysal    (1000) foysal    (1000)        0 2024-05-16 15:22:56.666455 dxh-0.1.1/dxh/
--rwxrwxrwx   0 foysal    (1000) foysal    (1000)      287 2023-10-10 17:54:41.000000 dxh-0.1.1/dxh/__init__.py
--rwxrwxrwx   0 foysal    (1000) foysal    (1000)      351 2024-05-16 15:22:06.000000 dxh-0.1.1/dxh/__version__.py
--rwxrwxrwx   0 foysal    (1000) foysal    (1000)     1371 2023-10-10 19:24:00.000000 dxh-0.1.1/dxh/obj_converter.py
-drwxrwxrwx   0 foysal    (1000) foysal    (1000)        0 2024-05-16 15:22:56.676591 dxh-0.1.1/dxh.egg-info/
--rwxrwxrwx   0 foysal    (1000) foysal    (1000)     1515 2024-05-16 15:22:56.000000 dxh-0.1.1/dxh.egg-info/PKG-INFO
--rwxrwxrwx   0 foysal    (1000) foysal    (1000)      208 2024-05-16 15:22:56.000000 dxh-0.1.1/dxh.egg-info/SOURCES.txt
--rwxrwxrwx   0 foysal    (1000) foysal    (1000)        1 2024-05-16 15:22:56.000000 dxh-0.1.1/dxh.egg-info/dependency_links.txt
--rwxrwxrwx   0 foysal    (1000) foysal    (1000)       23 2024-05-16 15:22:56.000000 dxh-0.1.1/dxh.egg-info/requires.txt
--rwxrwxrwx   0 foysal    (1000) foysal    (1000)        4 2024-05-16 15:22:56.000000 dxh-0.1.1/dxh.egg-info/top_level.txt
--rwxrwxrwx   0 foysal    (1000) foysal    (1000)       38 2024-05-16 15:22:56.681463 dxh-0.1.1/setup.cfg
--rwxrwxrwx   0 foysal    (1000) foysal    (1000)     1345 2024-05-16 15:22:22.000000 dxh-0.1.1/setup.py
+drwxrwxrwx   0 foysal    (1000) foysal    (1000)        0 2024-05-16 15:35:39.243059 dxh-0.1.2/
+-rwxrwxrwx   0 foysal    (1000) foysal    (1000)     1515 2024-05-16 15:35:39.209489 dxh-0.1.2/PKG-INFO
+-rwxrwxrwx   0 foysal    (1000) foysal    (1000)      534 2023-10-10 17:48:20.000000 dxh-0.1.2/README.md
+drwxrwxrwx   0 foysal    (1000) foysal    (1000)        0 2024-05-16 15:35:39.067695 dxh-0.1.2/dxh/
+-rwxrwxrwx   0 foysal    (1000) foysal    (1000)      287 2023-10-10 17:54:41.000000 dxh-0.1.2/dxh/__init__.py
+-rwxrwxrwx   0 foysal    (1000) foysal    (1000)      351 2024-05-16 15:35:33.000000 dxh-0.1.2/dxh/__version__.py
+-rwxrwxrwx   0 foysal    (1000) foysal    (1000)     1371 2023-10-10 19:24:00.000000 dxh-0.1.2/dxh/obj_converter.py
+drwxrwxrwx   0 foysal    (1000) foysal    (1000)        0 2024-05-16 15:35:39.165994 dxh-0.1.2/dxh.egg-info/
+-rwxrwxrwx   0 foysal    (1000) foysal    (1000)     1515 2024-05-16 15:35:38.000000 dxh-0.1.2/dxh.egg-info/PKG-INFO
+-rwxrwxrwx   0 foysal    (1000) foysal    (1000)      208 2024-05-16 15:35:38.000000 dxh-0.1.2/dxh.egg-info/SOURCES.txt
+-rwxrwxrwx   0 foysal    (1000) foysal    (1000)        1 2024-05-16 15:35:38.000000 dxh-0.1.2/dxh.egg-info/dependency_links.txt
+-rwxrwxrwx   0 foysal    (1000) foysal    (1000)       23 2024-05-16 15:35:38.000000 dxh-0.1.2/dxh.egg-info/requires.txt
+-rwxrwxrwx   0 foysal    (1000) foysal    (1000)        4 2024-05-16 15:35:38.000000 dxh-0.1.2/dxh.egg-info/top_level.txt
+-rwxrwxrwx   0 foysal    (1000) foysal    (1000)       38 2024-05-16 15:35:39.257516 dxh-0.1.2/setup.cfg
+-rwxrwxrwx   0 foysal    (1000) foysal    (1000)     1350 2024-05-16 15:34:00.000000 dxh-0.1.2/setup.py
```

### Comparing `dxh-0.1.1/PKG-INFO` & `dxh-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxh
-Version: 0.1.1
+Version: 0.1.2
 Summary: dxh is Convert python objects to camel case and snake case keys using this library.
 Home-page: https://github.com/iamfoysal/dxh
 Author: Mohammad Foysal
 License: MIT
 Project-URL: Source, https://github.com/iamfoysal/dxh
 Keywords: python,object,convert,camel,snake,case,keys,to,camel,case
 Platform: UNKNOWN
```

### Comparing `dxh-0.1.1/README.md` & `dxh-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `dxh-0.1.1/dxh/obj_converter.py` & `dxh-0.1.2/dxh/obj_converter.py`

 * *Files identical despite different names*

### Comparing `dxh-0.1.1/dxh.egg-info/PKG-INFO` & `dxh-0.1.2/dxh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxh
-Version: 0.1.1
+Version: 0.1.2
 Summary: dxh is Convert python objects to camel case and snake case keys using this library.
 Home-page: https://github.com/iamfoysal/dxh
 Author: Mohammad Foysal
 License: MIT
 Project-URL: Source, https://github.com/iamfoysal/dxh
 Keywords: python,object,convert,camel,snake,case,keys,to,camel,case
 Platform: UNKNOWN
```

### Comparing `dxh-0.1.1/setup.py` & `dxh-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with open("dxh/__version__.py", "r") as f:
     exec(f.read(), about)
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 with open("requirements.txt", "r") as f:
-    install_requires = f.readlines()
+    install_requires = f.read().splitlines()
 
 setuptools.setup(
     name=about["__title__"],
     version=about["__version__"],
     description=about["__description__"],
     long_description=long_description,
     long_description_content_type="text/markdown",
@@ -31,14 +31,11 @@
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Topic :: Software Development",
         "Topic :: Software Development :: Libraries :: Python Modules",
-
-
     ],
     python_requires=">=3.9",
     project_urls={"Source": about["__url__"]},
-
 )
```

