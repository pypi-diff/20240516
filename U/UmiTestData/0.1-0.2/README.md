# Comparing `tmp/UmiTestData-0.1.tar.gz` & `tmp/UmiTestData-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UmiTestData-0.1.tar", last modified: Wed May 15 21:39:20 2024, max compression
+gzip compressed data, was "UmiTestData-0.2.tar", last modified: Wed May 15 22:10:56 2024, max compression
```

## Comparing `UmiTestData-0.1.tar` & `UmiTestData-0.2.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 21:39:20.379163 UmiTestData-0.1/
--rw-rw-rw-   0        0        0      605 2024-05-15 21:39:20.378163 UmiTestData-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-15 21:39:20.346430 UmiTestData-0.1/UmiTD/
--rw-rw-rw-   0        0        0     5597 2024-05-15 21:26:35.000000 UmiTestData-0.1/UmiTD/UmiTD.py
--rw-rw-rw-   0        0        0       15 2024-05-15 21:38:07.000000 UmiTestData-0.1/UmiTD/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 21:39:20.376165 UmiTestData-0.1/UmiTestData.egg-info/
--rw-rw-rw-   0        0        0      605 2024-05-15 21:39:20.000000 UmiTestData-0.1/UmiTestData.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2024-05-15 21:39:20.000000 UmiTestData-0.1/UmiTestData.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 21:39:20.000000 UmiTestData-0.1/UmiTestData.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-05-15 21:39:20.000000 UmiTestData-0.1/UmiTestData.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-15 21:39:20.000000 UmiTestData-0.1/UmiTestData.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 21:39:20.379163 UmiTestData-0.1/setup.cfg
--rw-rw-rw-   0        0        0      736 2024-05-15 21:33:44.000000 UmiTestData-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 22:10:56.397957 UmiTestData-0.2/
+-rw-rw-rw-   0        0        0      492 2024-05-15 22:10:56.396954 UmiTestData-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-15 22:10:56.372566 UmiTestData-0.2/UmiTD/
+-rw-rw-rw-   0        0        0     5597 2024-05-15 21:26:35.000000 UmiTestData-0.2/UmiTD/UmiTD.py
+-rw-rw-rw-   0        0        0       15 2024-05-15 21:38:07.000000 UmiTestData-0.2/UmiTD/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 22:10:56.395677 UmiTestData-0.2/UmiTestData.egg-info/
+-rw-rw-rw-   0        0        0      492 2024-05-15 22:10:56.000000 UmiTestData-0.2/UmiTestData.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      181 2024-05-15 22:10:56.000000 UmiTestData-0.2/UmiTestData.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 22:10:56.000000 UmiTestData-0.2/UmiTestData.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-15 22:10:56.000000 UmiTestData-0.2/UmiTestData.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 22:10:56.397957 UmiTestData-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      611 2024-05-15 22:09:55.000000 UmiTestData-0.2/setup.py
```

### Comparing `UmiTestData-0.1/UmiTD/UmiTD.py` & `UmiTestData-0.2/UmiTD/UmiTD.py`

 * *Files identical despite different names*

### Comparing `UmiTestData-0.1/setup.py` & `UmiTestData-0.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name='UmiTestData',
-    version='0.1',
+    version='0.2',
     packages=find_packages(),
     description='A simple tool to generate random test data',
     author='UmiCore - Kazuya',
     url='https://github.com/kazuya-2006-26',
     license='MIT',
-    install_requires=[
-        'random',
-        'time',
-        'json',
-        'string',
-        'datetime',
-    ],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
```

