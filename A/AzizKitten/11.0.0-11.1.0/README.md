# Comparing `tmp/AzizKitten-11.0.0.tar.gz` & `tmp/azizkitten-11.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AzizKitten-11.0.0.tar", last modified: Thu Feb  8 10:28:52 2024, max compression
+gzip compressed data, was "azizkitten-11.1.0.tar", last modified: Thu May 16 17:30:29 2024, max compression
```

## Comparing `AzizKitten-11.0.0.tar` & `azizkitten-11.1.0.tar`

### file list

```diff
@@ -1,42 +1,53 @@
-drwxrwxrwx   0        0        0        0 2024-02-08 10:28:52.161981 AzizKitten-11.0.0/
-drwxrwxrwx   0        0        0        0 2024-02-08 10:28:52.146347 AzizKitten-11.0.0/AzizKitten/
--rw-rw-rw-   0        0        0      654 2024-02-06 13:41:08.000000 AzizKitten-11.0.0/AzizKitten/__init__.py
--rw-rw-rw-   0        0        0      199 2024-02-06 13:32:20.000000 AzizKitten-11.0.0/AzizKitten/acos.py
--rw-rw-rw-   0        0        0       64 2024-02-06 13:34:15.000000 AzizKitten-11.0.0/AzizKitten/acot.py
--rw-rw-rw-   0        0        0       64 2024-02-06 13:33:55.000000 AzizKitten-11.0.0/AzizKitten/acsc.py
--rw-rw-rw-   0        0        0    19953 2024-02-06 12:37:23.000000 AzizKitten-11.0.0/AzizKitten/among_us.py
--rw-rw-rw-   0        0        0       64 2024-02-06 13:33:33.000000 AzizKitten-11.0.0/AzizKitten/asec.py
--rw-rw-rw-   0        0        0      406 2024-02-06 13:31:30.000000 AzizKitten-11.0.0/AzizKitten/asin.py
--rw-rw-rw-   0        0        0      141 2024-02-06 13:33:07.000000 AzizKitten-11.0.0/AzizKitten/atan.py
--rw-rw-rw-   0        0        0      409 2024-02-06 12:37:23.000000 AzizKitten-11.0.0/AzizKitten/bin_rep.py
--rw-rw-rw-   0        0        0      137 2024-02-06 13:45:33.000000 AzizKitten-11.0.0/AzizKitten/constants.py
--rw-rw-rw-   0        0        0      159 2024-02-06 13:28:54.000000 AzizKitten-11.0.0/AzizKitten/cos.py
--rw-rw-rw-   0        0        0      139 2024-02-06 13:30:41.000000 AzizKitten-11.0.0/AzizKitten/cot.py
--rw-rw-rw-   0        0        0      139 2024-02-06 13:26:25.000000 AzizKitten-11.0.0/AzizKitten/csc.py
--rw-rw-rw-   0        0        0       60 2024-02-06 13:34:42.000000 AzizKitten-11.0.0/AzizKitten/exp.py
--rw-rw-rw-   0        0        0      203 2024-02-07 12:41:40.000000 AzizKitten-11.0.0/AzizKitten/factorial.py
--rw-rw-rw-   0        0        0       81 2024-02-07 12:42:22.000000 AzizKitten-11.0.0/AzizKitten/gcd.py
--rw-rw-rw-   0        0        0      339 2024-02-06 13:20:04.000000 AzizKitten-11.0.0/AzizKitten/integrate.py
--rw-rw-rw-   0        0        0       82 2024-02-07 12:42:13.000000 AzizKitten-11.0.0/AzizKitten/lcm.py
--rw-rw-rw-   0        0        0      856 2024-02-07 12:53:36.000000 AzizKitten-11.0.0/AzizKitten/limit.py
--rw-rw-rw-   0        0        0      132 2024-02-06 14:20:00.000000 AzizKitten-11.0.0/AzizKitten/ln.py
--rw-rw-rw-   0        0        0       74 2024-02-06 13:22:15.000000 AzizKitten-11.0.0/AzizKitten/log.py
--rw-rw-rw-   0        0        0     2249 2024-02-06 12:37:23.000000 AzizKitten-11.0.0/AzizKitten/ment_calc.py
--rw-rw-rw-   0        0        0     6268 2024-02-06 12:37:23.000000 AzizKitten-11.0.0/AzizKitten/mystery.py
--rw-rw-rw-   0        0        0     5358 2024-02-06 13:18:37.000000 AzizKitten-11.0.0/AzizKitten/quad.py
--rw-rw-rw-   0        0        0      171 2024-02-06 13:19:07.000000 AzizKitten-11.0.0/AzizKitten/root.py
--rw-rw-rw-   0        0        0      139 2024-02-06 13:30:00.000000 AzizKitten-11.0.0/AzizKitten/sec.py
--rw-rw-rw-   0        0        0      295 2024-02-06 13:29:02.000000 AzizKitten-11.0.0/AzizKitten/sin.py
--rw-rw-rw-   0        0        0      169 2024-02-06 13:30:05.000000 AzizKitten-11.0.0/AzizKitten/tan.py
-drwxrwxrwx   0        0        0        0 2024-02-08 10:28:52.158019 AzizKitten-11.0.0/AzizKitten.egg-info/
--rw-rw-rw-   0        0        0      785 2024-02-08 10:28:52.000000 AzizKitten-11.0.0/AzizKitten.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      744 2024-02-08 10:28:52.000000 AzizKitten-11.0.0/AzizKitten.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-08 10:28:52.000000 AzizKitten-11.0.0/AzizKitten.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-02-08 10:28:52.000000 AzizKitten-11.0.0/AzizKitten.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1055 2024-02-06 12:37:22.000000 AzizKitten-11.0.0/LICENSE
--rw-rw-rw-   0        0        0       84 2024-02-06 12:37:22.000000 AzizKitten-11.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0      785 2024-02-08 10:28:52.160452 AzizKitten-11.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      173 2024-02-06 12:37:22.000000 AzizKitten-11.0.0/README.md
--rw-rw-rw-   0        0        0      673 2024-02-08 10:27:48.000000 AzizKitten-11.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-08 10:28:52.161981 AzizKitten-11.0.0/setup.cfg
--rw-rw-rw-   0        0        0      708 2024-02-08 10:28:04.000000 AzizKitten-11.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 17:30:29.411253 azizkitten-11.1.0/
+drwxrwxrwx   0        0        0        0 2024-05-16 17:30:29.400687 azizkitten-11.1.0/AzizKitten/
+-rw-rw-rw-   0        0        0      952 2024-05-16 17:24:43.000000 azizkitten-11.1.0/AzizKitten/__init__.py
+-rw-rw-rw-   0        0        0      199 2024-02-06 13:32:20.000000 azizkitten-11.1.0/AzizKitten/acos.py
+-rw-rw-rw-   0        0        0       64 2024-02-06 13:34:15.000000 azizkitten-11.1.0/AzizKitten/acot.py
+-rw-rw-rw-   0        0        0       64 2024-02-06 13:33:55.000000 azizkitten-11.1.0/AzizKitten/acsc.py
+-rw-rw-rw-   0        0        0    19953 2024-02-06 12:37:23.000000 azizkitten-11.1.0/AzizKitten/among_us.py
+-rw-rw-rw-   0        0        0       64 2024-02-06 13:33:33.000000 azizkitten-11.1.0/AzizKitten/asec.py
+-rw-rw-rw-   0        0        0      406 2024-02-06 13:31:30.000000 azizkitten-11.1.0/AzizKitten/asin.py
+-rw-rw-rw-   0        0        0      141 2024-05-16 17:14:01.000000 azizkitten-11.1.0/AzizKitten/atan.py
+-rw-rw-rw-   0        0        0      409 2024-02-06 12:37:23.000000 azizkitten-11.1.0/AzizKitten/bin_rep.py
+-rw-rw-rw-   0        0        0     2128 2024-05-16 17:14:20.000000 azizkitten-11.1.0/AzizKitten/cbrt.py
+-rw-rw-rw-   0        0        0      199 2024-05-16 17:28:31.000000 azizkitten-11.1.0/AzizKitten/constants.py
+-rw-rw-rw-   0        0        0      306 2024-05-16 17:14:09.000000 azizkitten-11.1.0/AzizKitten/cos.py
+-rw-rw-rw-   0        0        0       71 2024-02-09 14:35:45.000000 azizkitten-11.1.0/AzizKitten/cosh.py
+-rw-rw-rw-   0        0        0      168 2024-02-24 15:38:52.000000 azizkitten-11.1.0/AzizKitten/cot.py
+-rw-rw-rw-   0        0        0       96 2024-02-24 15:39:19.000000 azizkitten-11.1.0/AzizKitten/coth.py
+-rw-rw-rw-   0        0        0      139 2024-02-06 13:26:25.000000 azizkitten-11.1.0/AzizKitten/csc.py
+-rw-rw-rw-   0        0        0       62 2024-02-09 14:42:18.000000 azizkitten-11.1.0/AzizKitten/csch.py
+-rw-rw-rw-   0        0        0     2224 2024-05-16 17:14:30.000000 azizkitten-11.1.0/AzizKitten/cubic.py
+-rw-rw-rw-   0        0        0       66 2024-02-24 15:36:56.000000 azizkitten-11.1.0/AzizKitten/degree.py
+-rw-rw-rw-   0        0        0       60 2024-02-06 13:34:42.000000 azizkitten-11.1.0/AzizKitten/exp.py
+-rw-rw-rw-   0        0        0      506 2024-05-14 18:00:41.000000 azizkitten-11.1.0/AzizKitten/factorial.py
+-rw-rw-rw-   0        0        0      135 2024-02-10 09:32:39.000000 azizkitten-11.1.0/AzizKitten/floor.py
+-rw-rw-rw-   0        0        0       81 2024-02-07 12:42:22.000000 azizkitten-11.1.0/AzizKitten/gcd.py
+-rw-rw-rw-   0        0        0      605 2024-05-14 17:51:40.000000 azizkitten-11.1.0/AzizKitten/integrate.py
+-rw-rw-rw-   0        0        0       82 2024-02-07 12:42:13.000000 azizkitten-11.1.0/AzizKitten/lcm.py
+-rw-rw-rw-   0        0        0     1485 2024-02-10 11:22:50.000000 azizkitten-11.1.0/AzizKitten/limit.py
+-rw-rw-rw-   0        0        0      516 2024-05-14 17:38:20.000000 azizkitten-11.1.0/AzizKitten/ln.py
+-rw-rw-rw-   0        0        0       74 2024-02-06 13:22:15.000000 azizkitten-11.1.0/AzizKitten/log.py
+-rw-rw-rw-   0        0        0     2249 2024-02-06 12:37:23.000000 azizkitten-11.1.0/AzizKitten/ment_calc.py
+-rw-rw-rw-   0        0        0     6268 2024-02-06 12:37:23.000000 azizkitten-11.1.0/AzizKitten/mystery.py
+-rw-rw-rw-   0        0        0      560 2024-05-16 17:14:04.000000 azizkitten-11.1.0/AzizKitten/quad.py
+-rw-rw-rw-   0        0        0       68 2024-02-24 15:35:25.000000 azizkitten-11.1.0/AzizKitten/radian.py
+-rw-rw-rw-   0        0        0      139 2024-02-06 13:30:00.000000 azizkitten-11.1.0/AzizKitten/sec.py
+-rw-rw-rw-   0        0        0       62 2024-02-09 14:41:44.000000 azizkitten-11.1.0/AzizKitten/sech.py
+-rw-rw-rw-   0        0        0      310 2024-05-16 17:14:11.000000 azizkitten-11.1.0/AzizKitten/sin.py
+-rw-rw-rw-   0        0        0       71 2024-02-10 11:23:11.000000 azizkitten-11.1.0/AzizKitten/sinh.py
+-rw-rw-rw-   0        0        0      114 2024-05-14 17:41:04.000000 azizkitten-11.1.0/AzizKitten/sqrt.py
+-rw-rw-rw-   0        0        0      169 2024-02-06 13:30:05.000000 azizkitten-11.1.0/AzizKitten/tan.py
+-rw-rw-rw-   0        0        0       96 2024-02-09 14:36:37.000000 azizkitten-11.1.0/AzizKitten/tanh.py
+drwxrwxrwx   0        0        0        0 2024-05-16 17:30:29.409249 azizkitten-11.1.0/AzizKitten.egg-info/
+-rw-rw-rw-   0        0        0      785 2024-05-16 17:30:29.000000 azizkitten-11.1.0/AzizKitten.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      959 2024-05-16 17:30:29.000000 azizkitten-11.1.0/AzizKitten.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 17:30:29.000000 azizkitten-11.1.0/AzizKitten.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-16 17:30:29.000000 azizkitten-11.1.0/AzizKitten.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1055 2024-02-06 12:37:22.000000 azizkitten-11.1.0/LICENSE
+-rw-rw-rw-   0        0        0       84 2024-02-06 12:37:22.000000 azizkitten-11.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      785 2024-05-16 17:30:29.410252 azizkitten-11.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2024-02-06 12:37:22.000000 azizkitten-11.1.0/README.md
+-rw-rw-rw-   0        0        0      673 2024-05-16 17:29:10.000000 azizkitten-11.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-16 17:30:29.412251 azizkitten-11.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      708 2024-05-16 17:29:19.000000 azizkitten-11.1.0/setup.py
```

### Comparing `AzizKitten-11.0.0/AzizKitten/among_us.py` & `azizkitten-11.1.0/AzizKitten/among_us.py`

 * *Files identical despite different names*

### Comparing `AzizKitten-11.0.0/AzizKitten/ment_calc.py` & `azizkitten-11.1.0/AzizKitten/ment_calc.py`

 * *Files identical despite different names*

### Comparing `AzizKitten-11.0.0/AzizKitten/mystery.py` & `azizkitten-11.1.0/AzizKitten/mystery.py`

 * *Files identical despite different names*

### Comparing `AzizKitten-11.0.0/AzizKitten.egg-info/PKG-INFO` & `azizkitten-11.1.0/AzizKitten.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AzizKitten
-Version: 11.0.0
+Version: 11.1.0
 Summary: AzizOmrane's own Python package
 Author: AzizKitten
 Author-email: AzizKitten <azizprv43@gmail.com>
 Project-URL: AboutMe, https://azizkitten.github.io
 Project-URL: Documentation, https://azizkitten.github.io/python
 Project-URL: Bug Tracker, https://github.com/AzizKitten/azizkitten.github.io/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `AzizKitten-11.0.0/AzizKitten.egg-info/SOURCES.txt` & `azizkitten-11.1.0/AzizKitten.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -8,30 +8,41 @@
 AzizKitten/acot.py
 AzizKitten/acsc.py
 AzizKitten/among_us.py
 AzizKitten/asec.py
 AzizKitten/asin.py
 AzizKitten/atan.py
 AzizKitten/bin_rep.py
+AzizKitten/cbrt.py
 AzizKitten/constants.py
 AzizKitten/cos.py
+AzizKitten/cosh.py
 AzizKitten/cot.py
+AzizKitten/coth.py
 AzizKitten/csc.py
+AzizKitten/csch.py
+AzizKitten/cubic.py
+AzizKitten/degree.py
 AzizKitten/exp.py
 AzizKitten/factorial.py
+AzizKitten/floor.py
 AzizKitten/gcd.py
 AzizKitten/integrate.py
 AzizKitten/lcm.py
 AzizKitten/limit.py
 AzizKitten/ln.py
 AzizKitten/log.py
 AzizKitten/ment_calc.py
 AzizKitten/mystery.py
 AzizKitten/quad.py
-AzizKitten/root.py
+AzizKitten/radian.py
 AzizKitten/sec.py
+AzizKitten/sech.py
 AzizKitten/sin.py
+AzizKitten/sinh.py
+AzizKitten/sqrt.py
 AzizKitten/tan.py
+AzizKitten/tanh.py
 AzizKitten.egg-info/PKG-INFO
 AzizKitten.egg-info/SOURCES.txt
 AzizKitten.egg-info/dependency_links.txt
 AzizKitten.egg-info/top_level.txt
```

### Comparing `AzizKitten-11.0.0/LICENSE` & `azizkitten-11.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `AzizKitten-11.0.0/PKG-INFO` & `azizkitten-11.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AzizKitten
-Version: 11.0.0
+Version: 11.1.0
 Summary: AzizOmrane's own Python package
 Author: AzizKitten
 Author-email: AzizKitten <azizprv43@gmail.com>
 Project-URL: AboutMe, https://azizkitten.github.io
 Project-URL: Documentation, https://azizkitten.github.io/python
 Project-URL: Bug Tracker, https://github.com/AzizKitten/azizkitten.github.io/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `AzizKitten-11.0.0/pyproject.toml` & `azizkitten-11.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "AzizKitten"
-version = "11.0.0"
+version = "11.1.0"
 authors = [
   { name="AzizKitten", email="azizprv43@gmail.com" },
 ]
 description = "AzizOmrane's own Python package"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `AzizKitten-11.0.0/setup.py` & `azizkitten-11.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="AzizKitten",
-    version="11.0.0",
+    version="11.1.0",
     packages=find_packages(),
     include_package_data=True,
     author="AzizKitten",
     author_email="azizprv43@gmail.com",
     description="AzizOmrane's own python library",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

