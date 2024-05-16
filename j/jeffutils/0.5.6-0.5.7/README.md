# Comparing `tmp/jeffutils-0.5.6.tar.gz` & `tmp/jeffutils-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeffutils-0.5.6.tar", last modified: Wed May 15 19:00:20 2024, max compression
+gzip compressed data, was "jeffutils-0.5.7.tar", last modified: Thu May 16 17:40:44 2024, max compression
```

## Comparing `jeffutils-0.5.6.tar` & `jeffutils-0.5.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-15 19:00:20.659960 jeffutils-0.5.6/
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     1070 2024-03-16 21:55:37.000000 jeffutils-0.5.6/LICENSE.txt
--rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-05-15 19:00:20.659960 jeffutils-0.5.6/PKG-INFO
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       12 2024-03-16 21:29:21.000000 jeffutils-0.5.6/README.md
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       84 2024-03-16 21:54:38.000000 jeffutils-0.5.6/pyproject.toml
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       38 2024-05-15 19:00:20.659960 jeffutils-0.5.6/setup.cfg
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      559 2024-05-15 19:00:16.000000 jeffutils-0.5.6/setup.py
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-15 19:00:20.659960 jeffutils-0.5.6/src/
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-15 19:00:20.659960 jeffutils-0.5.6/src/jeffutils/
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        0 2024-03-16 21:50:41.000000 jeffutils-0.5.6/src/jeffutils/__init__.py
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)    22577 2024-05-15 18:59:55.000000 jeffutils-0.5.6/src/jeffutils/utils.py
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-15 19:00:20.659960 jeffutils-0.5.6/src/jeffutils.egg-info/
--rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-05-15 19:00:20.000000 jeffutils-0.5.6/src/jeffutils.egg-info/PKG-INFO
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      242 2024-05-15 19:00:20.000000 jeffutils-0.5.6/src/jeffutils.egg-info/SOURCES.txt
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        1 2024-05-15 19:00:20.000000 jeffutils-0.5.6/src/jeffutils.egg-info/dependency_links.txt
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       10 2024-05-15 19:00:20.000000 jeffutils-0.5.6/src/jeffutils.egg-info/top_level.txt
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-16 17:40:44.930596 jeffutils-0.5.7/
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     1070 2024-03-16 21:55:37.000000 jeffutils-0.5.7/LICENSE.txt
+-rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-05-16 17:40:44.930596 jeffutils-0.5.7/PKG-INFO
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       12 2024-03-16 21:29:21.000000 jeffutils-0.5.7/README.md
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       84 2024-03-16 21:54:38.000000 jeffutils-0.5.7/pyproject.toml
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       38 2024-05-16 17:40:44.930596 jeffutils-0.5.7/setup.cfg
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      559 2024-05-16 17:40:39.000000 jeffutils-0.5.7/setup.py
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-16 17:40:44.926596 jeffutils-0.5.7/src/
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-16 17:40:44.926596 jeffutils-0.5.7/src/jeffutils/
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        0 2024-03-16 21:50:41.000000 jeffutils-0.5.7/src/jeffutils/__init__.py
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)    22668 2024-05-16 17:40:15.000000 jeffutils-0.5.7/src/jeffutils/utils.py
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-16 17:40:44.930596 jeffutils-0.5.7/src/jeffutils.egg-info/
+-rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-05-16 17:40:44.000000 jeffutils-0.5.7/src/jeffutils.egg-info/PKG-INFO
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      242 2024-05-16 17:40:44.000000 jeffutils-0.5.7/src/jeffutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        1 2024-05-16 17:40:44.000000 jeffutils-0.5.7/src/jeffutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       10 2024-05-16 17:40:44.000000 jeffutils-0.5.7/src/jeffutils.egg-info/top_level.txt
```

### Comparing `jeffutils-0.5.6/LICENSE.txt` & `jeffutils-0.5.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jeffutils-0.5.6/setup.py` & `jeffutils-0.5.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='jeffutils',
-    version='0.5.6',
+    version='0.5.7',
     author='Jeff Hansen',
     author_email='jeffxhansen@gmail.com',
     description='A series of useful functions and decorators I use in most of my projects. Feel free to use them as well :)',
     package_dir={"": "src"},
     packages = find_packages(where="src"),
     classifiers=[
         'Programming Language :: Python :: 3',
```

### Comparing `jeffutils-0.5.6/src/jeffutils/utils.py` & `jeffutils-0.5.7/src/jeffutils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,18 @@
     with open(filepath, "a+") as file:
         if header:
             file.write(current_time(string=True, utc=utc, timestamp=False, seconds=seconds))
             file.write("\n" + "-"*3 + "\n")
         file.write(string)
         file.write(end)
         if header:
-            file.write("\n" + "-"*3 + "\n")
+            if end == "\n":
+                file.write("-"*3 + "\n")
+            else:
+                file.write("\n" + "-"*3 + "\n")
             
 def format_perc(perc):
     """takes in a percentage as a decimal and formats it
     in the form of +x.xx% or -x.xx%
     """
     perc *= 100
```

