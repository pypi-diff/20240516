# Comparing `tmp/lollms_client-0.5.6.tar.gz` & `tmp/lollms_client-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lollms_client-0.5.6.tar", last modified: Wed May 15 22:33:18 2024, max compression
+gzip compressed data, was "lollms_client-0.5.7.tar", last modified: Wed May 15 22:41:34 2024, max compression
```

## Comparing `lollms_client-0.5.6.tar` & `lollms_client-0.5.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 22:33:18.692263 lollms_client-0.5.6/
--rw-rw-rw-   0        0        0    11558 2024-03-30 19:02:48.000000 lollms_client-0.5.6/LICENSE
--rw-rw-rw-   0        0        0     3258 2024-05-15 22:33:18.691263 lollms_client-0.5.6/PKG-INFO
--rw-rw-rw-   0        0        0     2780 2024-04-08 23:28:01.000000 lollms_client-0.5.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 22:33:18.667729 lollms_client-0.5.6/lollms_client/
--rw-rw-rw-   0        0        0      341 2024-04-27 17:10:22.000000 lollms_client-0.5.6/lollms_client/__init__.py
--rw-rw-rw-   0        0        0    21876 2024-03-20 22:06:25.000000 lollms_client-0.5.6/lollms_client/lollms_config.py
--rw-rw-rw-   0        0        0    20023 2024-05-07 23:05:45.000000 lollms_client-0.5.6/lollms_client/lollms_core.py
--rw-rw-rw-   0        0        0     2073 2024-04-27 17:07:34.000000 lollms_client-0.5.6/lollms_client/lollms_discussion.py
--rw-rw-rw-   0        0        0    20548 2024-04-27 23:24:03.000000 lollms_client-0.5.6/lollms_client/lollms_personality.py
--rw-rw-rw-   0        0        0    65331 2024-04-27 15:52:23.000000 lollms_client-0.5.6/lollms_client/lollms_personality_worker.py
--rw-rw-rw-   0        0        0    18863 2024-04-29 23:43:11.000000 lollms_client-0.5.6/lollms_client/lollms_tasks.py
--rw-rw-rw-   0        0        0     2170 2024-04-29 23:40:27.000000 lollms_client-0.5.6/lollms_client/lollms_types.py
--rw-rw-rw-   0        0        0     2087 2024-04-27 16:48:27.000000 lollms_client-0.5.6/lollms_client/lollms_utilities.py
--rw-rw-rw-   0        0        0      900 2024-05-15 22:32:42.000000 lollms_client-0.5.6/lollms_client/lollms_xtts.py
-drwxrwxrwx   0        0        0        0 2024-05-15 22:33:18.690261 lollms_client-0.5.6/lollms_client.egg-info/
--rw-rw-rw-   0        0        0     3258 2024-05-15 22:33:18.000000 lollms_client-0.5.6/lollms_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      533 2024-05-15 22:33:18.000000 lollms_client-0.5.6/lollms_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 22:33:18.000000 lollms_client-0.5.6/lollms_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-15 22:33:18.000000 lollms_client-0.5.6/lollms_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-15 22:33:18.000000 lollms_client-0.5.6/lollms_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 22:33:18.692263 lollms_client-0.5.6/setup.cfg
--rw-rw-rw-   0        0        0      814 2024-05-15 22:33:06.000000 lollms_client-0.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 22:41:34.374712 lollms_client-0.5.7/
+-rw-rw-rw-   0        0        0    11558 2024-03-30 19:02:48.000000 lollms_client-0.5.7/LICENSE
+-rw-rw-rw-   0        0        0     3258 2024-05-15 22:41:34.374174 lollms_client-0.5.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2780 2024-04-08 23:28:01.000000 lollms_client-0.5.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 22:41:34.358157 lollms_client-0.5.7/lollms_client/
+-rw-rw-rw-   0        0        0      341 2024-04-27 17:10:22.000000 lollms_client-0.5.7/lollms_client/__init__.py
+-rw-rw-rw-   0        0        0    21876 2024-03-20 22:06:25.000000 lollms_client-0.5.7/lollms_client/lollms_config.py
+-rw-rw-rw-   0        0        0    20023 2024-05-07 23:05:45.000000 lollms_client-0.5.7/lollms_client/lollms_core.py
+-rw-rw-rw-   0        0        0     2073 2024-04-27 17:07:34.000000 lollms_client-0.5.7/lollms_client/lollms_discussion.py
+-rw-rw-rw-   0        0        0    20548 2024-04-27 23:24:03.000000 lollms_client-0.5.7/lollms_client/lollms_personality.py
+-rw-rw-rw-   0        0        0    65331 2024-04-27 15:52:23.000000 lollms_client-0.5.7/lollms_client/lollms_personality_worker.py
+-rw-rw-rw-   0        0        0    18863 2024-04-29 23:43:11.000000 lollms_client-0.5.7/lollms_client/lollms_tasks.py
+-rw-rw-rw-   0        0        0     2170 2024-04-29 23:40:27.000000 lollms_client-0.5.7/lollms_client/lollms_types.py
+-rw-rw-rw-   0        0        0     2087 2024-04-27 16:48:27.000000 lollms_client-0.5.7/lollms_client/lollms_utilities.py
+-rw-rw-rw-   0        0        0      984 2024-05-15 22:35:06.000000 lollms_client-0.5.7/lollms_client/lollms_xtts.py
+drwxrwxrwx   0        0        0        0 2024-05-15 22:41:34.373174 lollms_client-0.5.7/lollms_client.egg-info/
+-rw-rw-rw-   0        0        0     3258 2024-05-15 22:41:34.000000 lollms_client-0.5.7/lollms_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      533 2024-05-15 22:41:34.000000 lollms_client-0.5.7/lollms_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 22:41:34.000000 lollms_client-0.5.7/lollms_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-15 22:41:34.000000 lollms_client-0.5.7/lollms_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-15 22:41:34.000000 lollms_client-0.5.7/lollms_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 22:41:34.374712 lollms_client-0.5.7/setup.cfg
+-rw-rw-rw-   0        0        0      814 2024-05-15 22:41:32.000000 lollms_client-0.5.7/setup.py
```

### Comparing `lollms_client-0.5.6/LICENSE` & `lollms_client-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lollms_client-0.5.6/PKG-INFO` & `lollms_client-0.5.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lollms_client
-Version: 0.5.6
+Version: 0.5.7
 Summary: A client library for LoLLMs generate endpoint
 Home-page: https://github.com/ParisNeo/lollms_client
 Author: ParisNeo
 Author-email: parisneoai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `lollms_client-0.5.6/README.md` & `lollms_client-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `lollms_client-0.5.6/lollms_client/lollms_config.py` & `lollms_client-0.5.7/lollms_client/lollms_config.py`

 * *Files identical despite different names*

### Comparing `lollms_client-0.5.6/lollms_client/lollms_core.py` & `lollms_client-0.5.7/lollms_client/lollms_core.py`

 * *Files identical despite different names*

### Comparing `lollms_client-0.5.6/lollms_client/lollms_discussion.py` & `lollms_client-0.5.7/lollms_client/lollms_discussion.py`

 * *Files identical despite different names*

### Comparing `lollms_client-0.5.6/lollms_client/lollms_personality.py` & `lollms_client-0.5.7/lollms_client/lollms_personality.py`

 * *Files identical despite different names*

### Comparing `lollms_client-0.5.6/lollms_client/lollms_personality_worker.py` & `lollms_client-0.5.7/lollms_client/lollms_personality_worker.py`

 * *Files identical despite different names*

### Comparing `lollms_client-0.5.6/lollms_client/lollms_tasks.py` & `lollms_client-0.5.7/lollms_client/lollms_tasks.py`

 * *Files identical despite different names*

### Comparing `lollms_client-0.5.6/lollms_client/lollms_types.py` & `lollms_client-0.5.7/lollms_client/lollms_types.py`

 * *Files identical despite different names*

### Comparing `lollms_client-0.5.6/lollms_client/lollms_utilities.py` & `lollms_client-0.5.7/lollms_client/lollms_utilities.py`

 * *Files identical despite different names*

### Comparing `lollms_client-0.5.6/lollms_client.egg-info/PKG-INFO` & `lollms_client-0.5.7/lollms_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lollms_client
-Version: 0.5.6
+Version: 0.5.7
 Summary: A client library for LoLLMs generate endpoint
 Home-page: https://github.com/ParisNeo/lollms_client
 Author: ParisNeo
 Author-email: parisneoai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `lollms_client-0.5.6/lollms_client.egg-info/SOURCES.txt` & `lollms_client-0.5.7/lollms_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lollms_client-0.5.6/setup.py` & `lollms_client-0.5.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open('requirements.txt', 'r') as f:
     install_requires = f.read().splitlines()
     
 setuptools.setup(
     name="lollms_client",
-    version="0.5.6",
+    version="0.5.7",
     author="ParisNeo",
     author_email="parisneoai@gmail.com",
     description="A client library for LoLLMs generate endpoint",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ParisNeo/lollms_client",
     packages=setuptools.find_packages(),
```

