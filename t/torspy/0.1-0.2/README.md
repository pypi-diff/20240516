# Comparing `tmp/torspy-0.1.tar.gz` & `tmp/torspy-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torspy-0.1.tar", last modified: Thu May 16 15:26:31 2024, max compression
+gzip compressed data, was "torspy-0.2.tar", last modified: Thu May 16 15:44:22 2024, max compression
```

## Comparing `torspy-0.1.tar` & `torspy-0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 15:26:31.198900 torspy-0.1/
--rw-rw-rw-   0        0        0     1065 2024-05-16 15:23:00.000000 torspy-0.1/LICENSE
--rw-rw-rw-   0        0        0     4266 2024-05-16 15:26:31.198900 torspy-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3727 2024-05-16 15:23:00.000000 torspy-0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-16 15:26:31.198900 torspy-0.1/setup.cfg
--rw-rw-rw-   0        0        0      827 2024-05-16 15:23:03.000000 torspy-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 15:26:31.152035 torspy-0.1/torspy/
--rw-rw-rw-   0        0        0       78 2024-05-16 15:22:59.000000 torspy-0.1/torspy/__init__.py
--rw-rw-rw-   0        0        0      905 2024-05-16 15:22:59.000000 torspy-0.1/torspy/cli.py
--rw-rw-rw-   0        0        0     2630 2024-05-16 15:22:59.000000 torspy-0.1/torspy/scraper.py
--rw-rw-rw-   0        0        0      102 2024-05-16 15:23:00.000000 torspy-0.1/torspy/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-16 15:26:31.198900 torspy-0.1/torspy.egg-info/
--rw-rw-rw-   0        0        0     4266 2024-05-16 15:26:30.000000 torspy-0.1/torspy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2024-05-16 15:26:30.000000 torspy-0.1/torspy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 15:26:30.000000 torspy-0.1/torspy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-05-16 15:26:30.000000 torspy-0.1/torspy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       24 2024-05-16 15:26:30.000000 torspy-0.1/torspy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-16 15:26:30.000000 torspy-0.1/torspy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 15:44:22.093960 torspy-0.2/
+-rw-rw-rw-   0        0        0     1065 2024-05-16 15:23:00.000000 torspy-0.2/LICENSE
+-rw-rw-rw-   0        0        0     4266 2024-05-16 15:44:22.093960 torspy-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3727 2024-05-16 15:23:00.000000 torspy-0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-16 15:44:22.093960 torspy-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      827 2024-05-16 15:43:42.000000 torspy-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 15:44:22.062718 torspy-0.2/torspy/
+-rw-rw-rw-   0        0        0       78 2024-05-16 15:22:59.000000 torspy-0.2/torspy/__init__.py
+-rw-rw-rw-   0        0        0      914 2024-05-16 15:37:35.000000 torspy-0.2/torspy/cli.py
+-rw-rw-rw-   0        0        0     2630 2024-05-16 15:22:59.000000 torspy-0.2/torspy/scraper.py
+-rw-rw-rw-   0        0        0      102 2024-05-16 15:23:00.000000 torspy-0.2/torspy/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-16 15:44:22.093960 torspy-0.2/torspy.egg-info/
+-rw-rw-rw-   0        0        0     4266 2024-05-16 15:44:21.000000 torspy-0.2/torspy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2024-05-16 15:44:21.000000 torspy-0.2/torspy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 15:44:21.000000 torspy-0.2/torspy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-05-16 15:44:21.000000 torspy-0.2/torspy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       24 2024-05-16 15:44:21.000000 torspy-0.2/torspy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-16 15:44:21.000000 torspy-0.2/torspy.egg-info/top_level.txt
```

### Comparing `torspy-0.1/LICENSE` & `torspy-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `torspy-0.1/PKG-INFO` & `torspy-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torspy
-Version: 0.1
+Version: 0.2
 Summary: Tor onion site scraping tool
 Home-page: https://github.com/mr-fidal/torspy
 Author: Fidal
 Author-email: mrfidal@proton.me
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `torspy-0.1/README.md` & `torspy-0.2/README.md`

 * *Files identical despite different names*

### Comparing `torspy-0.1/setup.py` & `torspy-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='torspy',
-    version='0.1',
+    version='0.2',
     author='Fidal',
     author_email='mrfidal@proton.me',
     description='Tor onion site scraping tool',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/mr-fidal/torspy',
     packages=find_packages(),
```

### Comparing `torspy-0.1/torspy/cli.py` & `torspy-0.2/torspy/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 #!/usr/bin/python3
 # copyright ©️ 2024 author Fidal
 
 import argparse
 from .scraper import scrape_onion_site
 
 def main():
-   epilog_text = '''
+    epilog_text = '''
 Copyright (©️) 2024 author: Fidal
 Issue: https://GitHub.com/mr-fidal/torspy
 '''
     parser = argparse.ArgumentParser(description='Scrape a .onion site.', epilog=epilog_text,
-                                 formatter_class=argparse.RawDescriptionHelpFormatter)
+                                     formatter_class=argparse.RawDescriptionHelpFormatter)
     parser.add_argument('url', type=str, help='The .onion site URL to scrape')
     parser.add_argument('--find', type=str, help='The text to search for within the site')
     parser.add_argument('-s', '--save', type=str, help='The file name to save the content')
     parser.add_argument('-d', '--directory', type=str, help='The directory to save the file')
     args = parser.parse_args()
     scrape_onion_site(args.url, args.find, args.save, args.directory)
 
 if __name__ == "__main__":
     main()
+
```

### Comparing `torspy-0.1/torspy/scraper.py` & `torspy-0.2/torspy/scraper.py`

 * *Files identical despite different names*

### Comparing `torspy-0.1/torspy.egg-info/PKG-INFO` & `torspy-0.2/torspy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torspy
-Version: 0.1
+Version: 0.2
 Summary: Tor onion site scraping tool
 Home-page: https://github.com/mr-fidal/torspy
 Author: Fidal
 Author-email: mrfidal@proton.me
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

