# Comparing `tmp/txt2udp-0.1.0.tar.gz` & `tmp/txt2udp-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "txt2udp-0.1.0.tar", last modified: Wed May 15 13:06:32 2024, max compression
+gzip compressed data, was "txt2udp-0.1.1.tar", last modified: Wed May 15 13:56:39 2024, max compression
```

## Comparing `txt2udp-0.1.0.tar` & `txt2udp-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 13:06:32.535065 txt2udp-0.1.0/
--rw-rw-rw-   0        0        0    11560 2024-05-15 12:52:07.000000 txt2udp-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     3069 2024-05-15 13:06:32.533091 txt2udp-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2218 2024-05-15 12:46:37.000000 txt2udp-0.1.0/README.md
--rw-rw-rw-   0        0        0      634 2024-05-15 12:32:57.000000 txt2udp-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-15 13:06:32.536060 txt2udp-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      917 2024-05-15 13:02:53.000000 txt2udp-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-15 13:06:32.500760 txt2udp-0.1.0/txt2udp/
--rw-rw-rw-   0        0        0        0 2024-05-13 01:53:18.000000 txt2udp-0.1.0/txt2udp/__init__.py
--rw-rw-rw-   0        0        0     2218 2024-05-15 12:12:05.000000 txt2udp-0.1.0/txt2udp/cli.py
--rw-rw-rw-   0        0        0     3169 2024-05-15 12:12:05.000000 txt2udp-0.1.0/txt2udp/client.py
--rw-rw-rw-   0        0        0     1127 2024-05-15 12:12:05.000000 txt2udp-0.1.0/txt2udp/config.py
--rw-rw-rw-   0        0        0     1844 2024-05-15 12:12:05.000000 txt2udp-0.1.0/txt2udp/conn.py
--rw-rw-rw-   0        0        0      977 2024-05-15 12:12:05.000000 txt2udp-0.1.0/txt2udp/datagram.py
--rw-rw-rw-   0        0        0     1579 2024-05-15 12:12:05.000000 txt2udp-0.1.0/txt2udp/main.py
--rw-rw-rw-   0        0        0      330 2024-05-13 07:34:38.000000 txt2udp-0.1.0/txt2udp/messages.py
-drwxrwxrwx   0        0        0        0 2024-05-15 13:06:32.526835 txt2udp-0.1.0/txt2udp/plugins/
--rw-rw-rw-   0        0        0      621 2024-05-13 10:51:17.000000 txt2udp-0.1.0/txt2udp/plugins/__init__.py
--rw-rw-rw-   0        0        0     3783 2024-05-15 12:12:05.000000 txt2udp-0.1.0/txt2udp/plugins/mitm.py
--rw-rw-rw-   0        0        0      761 2024-05-15 12:12:05.000000 txt2udp-0.1.0/txt2udp/plugins/stdio.py
--rw-rw-rw-   0        0        0     3032 2024-05-15 12:12:05.000000 txt2udp-0.1.0/txt2udp/server.py
-drwxrwxrwx   0        0        0        0 2024-05-15 13:06:32.529864 txt2udp-0.1.0/txt2udp.egg-info/
--rw-rw-rw-   0        0        0     3069 2024-05-15 13:06:32.000000 txt2udp-0.1.0/txt2udp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      433 2024-05-15 13:06:32.000000 txt2udp-0.1.0/txt2udp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 13:06:32.000000 txt2udp-0.1.0/txt2udp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-05-15 13:06:32.000000 txt2udp-0.1.0/txt2udp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-15 13:06:32.000000 txt2udp-0.1.0/txt2udp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 13:56:39.473701 txt2udp-0.1.1/
+-rw-rw-rw-   0        0        0    11560 2024-05-15 12:52:07.000000 txt2udp-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     2861 2024-05-15 13:56:39.473701 txt2udp-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2218 2024-05-15 12:46:37.000000 txt2udp-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-15 13:56:39.473701 txt2udp-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      944 2024-05-15 13:56:25.000000 txt2udp-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:56:39.453660 txt2udp-0.1.1/txt2udp/
+-rw-rw-rw-   0        0        0        0 2024-05-13 01:53:18.000000 txt2udp-0.1.1/txt2udp/__init__.py
+-rw-rw-rw-   0        0        0     2218 2024-05-15 12:12:05.000000 txt2udp-0.1.1/txt2udp/cli.py
+-rw-rw-rw-   0        0        0     3169 2024-05-15 12:12:05.000000 txt2udp-0.1.1/txt2udp/client.py
+-rw-rw-rw-   0        0        0     1127 2024-05-15 12:12:05.000000 txt2udp-0.1.1/txt2udp/config.py
+-rw-rw-rw-   0        0        0     1844 2024-05-15 12:12:05.000000 txt2udp-0.1.1/txt2udp/conn.py
+-rw-rw-rw-   0        0        0      977 2024-05-15 12:12:05.000000 txt2udp-0.1.1/txt2udp/datagram.py
+-rw-rw-rw-   0        0        0     1579 2024-05-15 12:12:05.000000 txt2udp-0.1.1/txt2udp/main.py
+-rw-rw-rw-   0        0        0      330 2024-05-13 07:34:38.000000 txt2udp-0.1.1/txt2udp/messages.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:56:39.467623 txt2udp-0.1.1/txt2udp/plugins/
+-rw-rw-rw-   0        0        0      621 2024-05-13 10:51:17.000000 txt2udp-0.1.1/txt2udp/plugins/__init__.py
+-rw-rw-rw-   0        0        0     3783 2024-05-15 12:12:05.000000 txt2udp-0.1.1/txt2udp/plugins/mitm.py
+-rw-rw-rw-   0        0        0      761 2024-05-15 12:12:05.000000 txt2udp-0.1.1/txt2udp/plugins/stdio.py
+-rw-rw-rw-   0        0        0     3032 2024-05-15 12:12:05.000000 txt2udp-0.1.1/txt2udp/server.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:56:39.473701 txt2udp-0.1.1/txt2udp.egg-info/
+-rw-rw-rw-   0        0        0     2861 2024-05-15 13:56:39.000000 txt2udp-0.1.1/txt2udp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      452 2024-05-15 13:56:39.000000 txt2udp-0.1.1/txt2udp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 13:56:39.000000 txt2udp-0.1.1/txt2udp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2024-05-15 13:56:39.000000 txt2udp-0.1.1/txt2udp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       88 2024-05-15 13:56:39.000000 txt2udp-0.1.1/txt2udp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-15 13:56:39.000000 txt2udp-0.1.1/txt2udp.egg-info/top_level.txt
```

### Comparing `txt2udp-0.1.0/LICENSE` & `txt2udp-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `txt2udp-0.1.0/PKG-INFO` & `txt2udp-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: txt2udp
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple tool for forwarding UDP datagrams through a text-only protocol/interface.
 Home-page: https://github.com/mirrorange/TXT2UDP
 Author: Orange
-Author-email: Orange <orange@icedeer.net>
-Project-URL: Homepage, https://github.com/mirrorange/TXT2UDP
-Project-URL: Issues, https://github.com/mirrorange/TXT2UDP/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Author-email: orange@icedeer.net
+License: Apache-2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pydantic
+Requires-Dist: pydantic-settings
+Requires-Dist: loguru
 Provides-Extra: mitm
 Requires-Dist: mitmproxy; extra == "mitm"
 Provides-Extra: cli
 Requires-Dist: typer; extra == "cli"
 Provides-Extra: all
 Requires-Dist: mitmproxy; extra == "all"
 Requires-Dist: typer; extra == "all"
```

### Comparing `txt2udp-0.1.0/README.md` & `txt2udp-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `txt2udp-0.1.0/setup.py` & `txt2udp-0.1.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="txt2udp",
-    version="0.1.0",
+    version="0.1.1",
     description="A simple tool for forwarding UDP datagrams through a text-only protocol/interface.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mirrorange/TXT2UDP",
     packages=find_packages(),
     entry_points={
         "console_scripts": [
@@ -25,8 +25,9 @@
     extras_require={
         "mitm": ["mitmproxy"],
         "cli": ["typer"],
         "all": ["mitmproxy", "typer"],
     },
     author="Orange",
     author_email="orange@icedeer.net",
+    license="Apache-2.0",
 )
```

### Comparing `txt2udp-0.1.0/txt2udp/cli.py` & `txt2udp-0.1.1/txt2udp/cli.py`

 * *Files identical despite different names*

### Comparing `txt2udp-0.1.0/txt2udp/client.py` & `txt2udp-0.1.1/txt2udp/client.py`

 * *Files identical despite different names*

### Comparing `txt2udp-0.1.0/txt2udp/config.py` & `txt2udp-0.1.1/txt2udp/config.py`

 * *Files identical despite different names*

### Comparing `txt2udp-0.1.0/txt2udp/conn.py` & `txt2udp-0.1.1/txt2udp/conn.py`

 * *Files identical despite different names*

### Comparing `txt2udp-0.1.0/txt2udp/datagram.py` & `txt2udp-0.1.1/txt2udp/datagram.py`

 * *Files identical despite different names*

### Comparing `txt2udp-0.1.0/txt2udp/main.py` & `txt2udp-0.1.1/txt2udp/main.py`

 * *Files identical despite different names*

### Comparing `txt2udp-0.1.0/txt2udp/plugins/__init__.py` & `txt2udp-0.1.1/txt2udp/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `txt2udp-0.1.0/txt2udp/plugins/mitm.py` & `txt2udp-0.1.1/txt2udp/plugins/mitm.py`

 * *Files identical despite different names*

### Comparing `txt2udp-0.1.0/txt2udp/plugins/stdio.py` & `txt2udp-0.1.1/txt2udp/plugins/stdio.py`

 * *Files identical despite different names*

### Comparing `txt2udp-0.1.0/txt2udp/server.py` & `txt2udp-0.1.1/txt2udp/server.py`

 * *Files identical despite different names*

### Comparing `txt2udp-0.1.0/txt2udp.egg-info/PKG-INFO` & `txt2udp-0.1.1/txt2udp.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: txt2udp
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple tool for forwarding UDP datagrams through a text-only protocol/interface.
 Home-page: https://github.com/mirrorange/TXT2UDP
 Author: Orange
-Author-email: Orange <orange@icedeer.net>
-Project-URL: Homepage, https://github.com/mirrorange/TXT2UDP
-Project-URL: Issues, https://github.com/mirrorange/TXT2UDP/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Author-email: orange@icedeer.net
+License: Apache-2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pydantic
+Requires-Dist: pydantic-settings
+Requires-Dist: loguru
 Provides-Extra: mitm
 Requires-Dist: mitmproxy; extra == "mitm"
 Provides-Extra: cli
 Requires-Dist: typer; extra == "cli"
 Provides-Extra: all
 Requires-Dist: mitmproxy; extra == "all"
 Requires-Dist: typer; extra == "all"
```

