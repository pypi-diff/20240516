# Comparing `tmp/bambot-0.4.4.tar.gz` & `tmp/bambot-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bambot-0.4.4.tar", last modified: Wed May 15 07:02:49 2024, max compression
+gzip compressed data, was "bambot-0.4.5.tar", last modified: Thu May 16 19:57:38 2024, max compression
```

## Comparing `bambot-0.4.4.tar` & `bambot-0.4.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-05-15 07:02:49.799245 bambot-0.4.4/
--rw-r--r--   0 spencerkinney   (501) staff       (20)     2248 2024-05-15 07:02:49.799015 bambot-0.4.4/PKG-INFO
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1331 2024-05-15 06:59:48.000000 bambot-0.4.4/README.md
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-05-15 07:02:49.796078 bambot-0.4.4/bambot/
--rw-r--r--   0 spencerkinney   (501) staff       (20)        0 2024-05-01 04:48:56.000000 bambot-0.4.4/bambot/__init__.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)      468 2024-05-15 06:26:45.000000 bambot-0.4.4/bambot/app.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1869 2024-05-15 06:54:28.000000 bambot-0.4.4/bambot/build.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1325 2024-05-15 06:26:34.000000 bambot-0.4.4/bambot/cli.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1666 2024-05-15 06:40:42.000000 bambot-0.4.4/bambot/docker_utils.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1609 2024-05-03 06:10:47.000000 bambot-0.4.4/bambot/project.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1457 2024-05-03 05:03:21.000000 bambot-0.4.4/bambot/run.py
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-05-15 07:02:49.798386 bambot-0.4.4/bambot/templates/
--rw-r--r--   0 spencerkinney   (501) staff       (20)      329 2024-05-15 06:38:26.000000 bambot-0.4.4/bambot/templates/Dockerfile
--rw-r--r--   0 spencerkinney   (501) staff       (20)      171 2024-05-02 22:06:34.000000 bambot-0.4.4/bambot/templates/agent_runner.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)      942 2024-05-03 01:32:06.000000 bambot-0.4.4/bambot/templates/agent_template.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)      528 2024-05-02 21:29:55.000000 bambot-0.4.4/bambot/templates/langchain_template.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)       49 2024-05-15 06:30:42.000000 bambot-0.4.4/bambot/templates/requirements.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)     3920 2024-05-15 06:31:49.000000 bambot-0.4.4/bambot/templates/server.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)     3326 2024-05-15 06:58:09.000000 bambot-0.4.4/bambot/utils.py
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-05-15 07:02:49.798783 bambot-0.4.4/bambot.egg-info/
--rw-r--r--   0 spencerkinney   (501) staff       (20)     2248 2024-05-15 07:02:49.000000 bambot-0.4.4/bambot.egg-info/PKG-INFO
--rw-r--r--   0 spencerkinney   (501) staff       (20)      530 2024-05-15 07:02:49.000000 bambot-0.4.4/bambot.egg-info/SOURCES.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)        1 2024-05-15 07:02:49.000000 bambot-0.4.4/bambot.egg-info/dependency_links.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)       40 2024-05-15 07:02:49.000000 bambot-0.4.4/bambot.egg-info/entry_points.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)       46 2024-05-15 07:02:49.000000 bambot-0.4.4/bambot.egg-info/requires.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)        7 2024-05-15 07:02:49.000000 bambot-0.4.4/bambot.egg-info/top_level.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)       38 2024-05-15 07:02:49.799278 bambot-0.4.4/setup.cfg
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1234 2024-05-15 07:02:09.000000 bambot-0.4.4/setup.py
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-05-16 19:57:38.688370 bambot-0.4.5/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     2339 2024-05-16 19:57:38.688131 bambot-0.4.5/PKG-INFO
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1422 2024-05-16 19:56:42.000000 bambot-0.4.5/README.md
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-05-16 19:57:38.683685 bambot-0.4.5/bambot/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)        0 2024-05-01 04:48:56.000000 bambot-0.4.5/bambot/__init__.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      468 2024-05-15 06:26:45.000000 bambot-0.4.5/bambot/app.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1869 2024-05-15 06:54:28.000000 bambot-0.4.5/bambot/build.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1325 2024-05-15 06:26:34.000000 bambot-0.4.5/bambot/cli.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1666 2024-05-15 06:40:42.000000 bambot-0.4.5/bambot/docker_utils.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1609 2024-05-03 06:10:47.000000 bambot-0.4.5/bambot/project.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1457 2024-05-03 05:03:21.000000 bambot-0.4.5/bambot/run.py
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-05-16 19:57:38.687204 bambot-0.4.5/bambot/templates/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      329 2024-05-15 06:38:26.000000 bambot-0.4.5/bambot/templates/Dockerfile
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      171 2024-05-02 22:06:34.000000 bambot-0.4.5/bambot/templates/agent_runner.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      942 2024-05-03 01:32:06.000000 bambot-0.4.5/bambot/templates/agent_template.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      528 2024-05-02 21:29:55.000000 bambot-0.4.5/bambot/templates/langchain_template.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)       49 2024-05-15 06:30:42.000000 bambot-0.4.5/bambot/templates/requirements.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     3920 2024-05-15 06:31:49.000000 bambot-0.4.5/bambot/templates/server.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     3326 2024-05-15 06:58:09.000000 bambot-0.4.5/bambot/utils.py
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-05-16 19:57:38.687703 bambot-0.4.5/bambot.egg-info/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     2339 2024-05-16 19:57:38.000000 bambot-0.4.5/bambot.egg-info/PKG-INFO
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      530 2024-05-16 19:57:38.000000 bambot-0.4.5/bambot.egg-info/SOURCES.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)        1 2024-05-16 19:57:38.000000 bambot-0.4.5/bambot.egg-info/dependency_links.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)       40 2024-05-16 19:57:38.000000 bambot-0.4.5/bambot.egg-info/entry_points.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)       46 2024-05-16 19:57:38.000000 bambot-0.4.5/bambot.egg-info/requires.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)        7 2024-05-16 19:57:38.000000 bambot-0.4.5/bambot.egg-info/top_level.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)       38 2024-05-16 19:57:38.688608 bambot-0.4.5/setup.cfg
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1234 2024-05-16 19:57:14.000000 bambot-0.4.5/setup.py
```

### Comparing `bambot-0.4.4/PKG-INFO` & `bambot-0.4.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bambot
-Version: 0.4.4
+Version: 0.4.5
 Summary: Containers for AI agents
 Home-page: https://github.com/Bam-Corp/bambot
 Author: Bam Corp
 Author-email: spencer@bam.bot
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -23,16 +23,17 @@
 Requires-Dist: tqdm
 Requires-Dist: python-dotenv
 Requires-Dist: halo
 Requires-Dist: colorama
 
 # Bam
 
-[![PyPI version](https://badge.fury.io/py/bam.svg)](https://badge.fury.io/py/bam)
+[![PyPI version](https://badge.fury.io/py/bam.svg)](https://badge.fury.io/py/bambot)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![Downloads](https://static.pepy.tech/badge/bambot)](https://pepy.tech/project/bambot)
 
 Bam is a lightweight and easy-to-use command-line interface (CLI) tool for creating and running AI agent containers. It is currently Docker-based.
 
 ## Installation
 
 You can install Bam using pip:
```

### Comparing `bambot-0.4.4/README.md` & `bambot-0.4.5/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Bam
 
-[![PyPI version](https://badge.fury.io/py/bam.svg)](https://badge.fury.io/py/bam)
+[![PyPI version](https://badge.fury.io/py/bam.svg)](https://badge.fury.io/py/bambot)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![Downloads](https://static.pepy.tech/badge/bambot)](https://pepy.tech/project/bambot)
 
 Bam is a lightweight and easy-to-use command-line interface (CLI) tool for creating and running AI agent containers. It is currently Docker-based.
 
 ## Installation
 
 You can install Bam using pip:
```

### Comparing `bambot-0.4.4/bambot/build.py` & `bambot-0.4.5/bambot/build.py`

 * *Files identical despite different names*

### Comparing `bambot-0.4.4/bambot/cli.py` & `bambot-0.4.5/bambot/cli.py`

 * *Files identical despite different names*

### Comparing `bambot-0.4.4/bambot/docker_utils.py` & `bambot-0.4.5/bambot/docker_utils.py`

 * *Files identical despite different names*

### Comparing `bambot-0.4.4/bambot/project.py` & `bambot-0.4.5/bambot/project.py`

 * *Files identical despite different names*

### Comparing `bambot-0.4.4/bambot/run.py` & `bambot-0.4.5/bambot/run.py`

 * *Files identical despite different names*

### Comparing `bambot-0.4.4/bambot/templates/agent_template.py` & `bambot-0.4.5/bambot/templates/agent_template.py`

 * *Files identical despite different names*

### Comparing `bambot-0.4.4/bambot/templates/langchain_template.py` & `bambot-0.4.5/bambot/templates/langchain_template.py`

 * *Files identical despite different names*

### Comparing `bambot-0.4.4/bambot/templates/server.py` & `bambot-0.4.5/bambot/templates/server.py`

 * *Files identical despite different names*

### Comparing `bambot-0.4.4/bambot/utils.py` & `bambot-0.4.5/bambot/utils.py`

 * *Files identical despite different names*

### Comparing `bambot-0.4.4/bambot.egg-info/PKG-INFO` & `bambot-0.4.5/bambot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bambot
-Version: 0.4.4
+Version: 0.4.5
 Summary: Containers for AI agents
 Home-page: https://github.com/Bam-Corp/bambot
 Author: Bam Corp
 Author-email: spencer@bam.bot
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -23,16 +23,17 @@
 Requires-Dist: tqdm
 Requires-Dist: python-dotenv
 Requires-Dist: halo
 Requires-Dist: colorama
 
 # Bam
 
-[![PyPI version](https://badge.fury.io/py/bam.svg)](https://badge.fury.io/py/bam)
+[![PyPI version](https://badge.fury.io/py/bam.svg)](https://badge.fury.io/py/bambot)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![Downloads](https://static.pepy.tech/badge/bambot)](https://pepy.tech/project/bambot)
 
 Bam is a lightweight and easy-to-use command-line interface (CLI) tool for creating and running AI agent containers. It is currently Docker-based.
 
 ## Installation
 
 You can install Bam using pip:
```

### Comparing `bambot-0.4.4/bambot.egg-info/SOURCES.txt` & `bambot-0.4.5/bambot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bambot-0.4.4/setup.py` & `bambot-0.4.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="bambot",
-    version="0.4.4",
+    version="0.4.5",
     author="Bam Corp",
     author_email="spencer@bam.bot",
     description="Containers for AI agents",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Bam-Corp/bambot",
     packages=find_packages(),
```

