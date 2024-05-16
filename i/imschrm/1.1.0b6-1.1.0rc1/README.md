# Comparing `tmp/imschrm-1.1.0b6.tar.gz` & `tmp/imschrm-1.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imschrm-1.1.0b6.tar", last modified: Tue Dec 12 22:38:34 2023, max compression
+gzip compressed data, was "Z:\projects\imsc-hrm\imschrm-repo\dist\.tmp-_77kfgcr\imschrm-1.1.0rc1.tar", last modified: Thu Feb 29 18:58:10 2024, max compression
```

## Comparing `imschrm-1.1.0b6.tar` & `imschrm-1.1.0rc1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-12-12 22:38:34.031264 imschrm-1.1.0b6/
--rw-rw-rw-   0        0        0     1260 2021-06-02 18:29:36.000000 imschrm-1.1.0b6/LICENSE.txt
--rw-rw-rw-   0        0        0     3167 2023-12-12 22:38:34.015658 imschrm-1.1.0b6/PKG-INFO
--rw-rw-rw-   0        0        0     2221 2023-12-12 22:36:04.000000 imschrm-1.1.0b6/README.md
--rw-rw-rw-   0        0        0       42 2023-12-12 22:38:34.031264 imschrm-1.1.0b6/setup.cfg
--rw-rw-rw-   0        0        0     1330 2023-12-12 22:36:58.000000 imschrm-1.1.0b6/setup.py
-drwxrwxrwx   0        0        0        0 2023-12-12 22:38:33.312432 imschrm-1.1.0b6/src/
-drwxrwxrwx   0        0        0        0 2023-12-12 22:38:33.312432 imschrm-1.1.0b6/src/main/
-drwxrwxrwx   0        0        0        0 2023-12-12 22:38:33.312432 imschrm-1.1.0b6/src/main/python/
-drwxrwxrwx   0        0        0        0 2023-12-12 22:38:33.703112 imschrm-1.1.0b6/src/main/python/imschrm/
--rw-rw-rw-   0        0        0        0 2021-06-02 18:29:28.000000 imschrm-1.1.0b6/src/main/python/imschrm/__init__.py
--rw-rw-rw-   0        0        0     3643 2023-12-12 22:36:04.000000 imschrm-1.1.0b6/src/main/python/imschrm/cli.py
--rw-rw-rw-   0        0        0   366016 2023-12-12 22:36:04.000000 imschrm-1.1.0b6/src/main/python/imschrm/codepoint_sets.py
--rw-rw-rw-   0        0        0     3394 2023-12-08 01:40:13.000000 imschrm-1.1.0b6/src/main/python/imschrm/doc_sequence.py
--rw-rw-rw-   0        0        0    12174 2023-12-12 22:36:04.000000 imschrm-1.1.0b6/src/main/python/imschrm/hrm.py
-drwxrwxrwx   0        0        0        0 2023-12-12 22:38:34.000007 imschrm-1.1.0b6/src/main/python/imschrm.egg-info/
--rw-rw-rw-   0        0        0     3167 2023-12-12 22:38:32.000000 imschrm-1.1.0b6/src/main/python/imschrm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      778 2023-12-12 22:38:33.000000 imschrm-1.1.0b6/src/main/python/imschrm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-12 22:38:32.000000 imschrm-1.1.0b6/src/main/python/imschrm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-12-12 22:38:32.000000 imschrm-1.1.0b6/src/main/python/imschrm.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-12-12 22:38:32.000000 imschrm-1.1.0b6/src/main/python/imschrm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-12-12 22:38:32.000000 imschrm-1.1.0b6/src/main/python/imschrm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-02-29 18:58:10.472740 imschrm-1.1.0rc1/
+-rw-rw-rw-   0        0        0     1260 2021-06-02 18:29:36.000000 imschrm-1.1.0rc1/LICENSE.txt
+-rw-rw-rw-   0        0        0     3168 2024-02-29 18:58:10.472740 imschrm-1.1.0rc1/PKG-INFO
+-rw-rw-rw-   0        0        0     2221 2023-12-12 22:36:04.000000 imschrm-1.1.0rc1/README.md
+-rw-rw-rw-   0        0        0       42 2024-02-29 18:58:10.488362 imschrm-1.1.0rc1/setup.cfg
+-rw-rw-rw-   0        0        0     1333 2024-02-29 18:57:03.000000 imschrm-1.1.0rc1/setup.py
+drwxrwxrwx   0        0        0        0 2024-02-29 18:58:10.175932 imschrm-1.1.0rc1/src/
+drwxrwxrwx   0        0        0        0 2024-02-29 18:58:10.175932 imschrm-1.1.0rc1/src/main/
+drwxrwxrwx   0        0        0        0 2024-02-29 18:58:10.175932 imschrm-1.1.0rc1/src/main/python/
+drwxrwxrwx   0        0        0        0 2024-02-29 18:58:10.285282 imschrm-1.1.0rc1/src/main/python/imschrm/
+-rw-rw-rw-   0        0        0        0 2021-06-02 18:29:28.000000 imschrm-1.1.0rc1/src/main/python/imschrm/__init__.py
+-rw-rw-rw-   0        0        0     3643 2023-12-12 22:36:04.000000 imschrm-1.1.0rc1/src/main/python/imschrm/cli.py
+-rw-rw-rw-   0        0        0   366016 2023-12-12 22:36:04.000000 imschrm-1.1.0rc1/src/main/python/imschrm/codepoint_sets.py
+-rw-rw-rw-   0        0        0     3394 2023-12-08 01:40:13.000000 imschrm-1.1.0rc1/src/main/python/imschrm/doc_sequence.py
+-rw-rw-rw-   0        0        0    12174 2023-12-12 22:36:04.000000 imschrm-1.1.0rc1/src/main/python/imschrm/hrm.py
+drwxrwxrwx   0        0        0        0 2024-02-29 18:58:10.207175 imschrm-1.1.0rc1/src/main/python/imschrm.egg-info/
+-rw-rw-rw-   0        0        0     3168 2024-02-29 18:58:10.000000 imschrm-1.1.0rc1/src/main/python/imschrm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      778 2024-02-29 18:58:10.000000 imschrm-1.1.0rc1/src/main/python/imschrm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-02-29 18:58:10.000000 imschrm-1.1.0rc1/src/main/python/imschrm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-02-29 18:58:10.000000 imschrm-1.1.0rc1/src/main/python/imschrm.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-02-29 18:58:10.000000 imschrm-1.1.0rc1/src/main/python/imschrm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-02-29 18:58:10.000000 imschrm-1.1.0rc1/src/main/python/imschrm.egg-info/top_level.txt
```

### Comparing `imschrm-1.1.0b6/LICENSE.txt` & `imschrm-1.1.0rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `imschrm-1.1.0b6/PKG-INFO` & `imschrm-1.1.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imschrm
-Version: 1.1.0b6
+Version: 1.1.0rc1
 Summary: Validates IMSC documents against the IMSC HRM
 Home-page: https://www.sandflow.com
 Author: Sandflow Consulting LLC
 Author-email: info@sandflow.com
 Project-URL: Bug Reports, https://github.com/sandflow/imscHRM/issues
 Project-URL: Source, https://github.com/sandflow/imscHRM
 Keywords: ttml,imsc,smpte-tt,hrm,complexity
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Multimedia
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: ttconv>=1.0.8-a2
+Requires-Dist: ttconv>=1.1.0rc1
 
 # IMSC Hypothetical Render Model (HRM) Validator
 
      __  _  _  ____   ___  _  _  ____  _  _ 
     (  )( \/ )/ ___) / __)/ )( \(  _ \( \/ )
      )( / \/ \\___ \( (__ ) __ ( )   // \/ \
     (__)\_)(_/(____/ \___)\_)(_/(__\_)\_)(_/
```

### Comparing `imschrm-1.1.0b6/README.md` & `imschrm-1.1.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `imschrm-1.1.0b6/setup.py` & `imschrm-1.1.0rc1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
   long_description = fh.read()
 
 setup(
   name='imschrm',
-  version='1.1.0b6',
+  version='1.1.0-rc.1',
   description='Validates IMSC documents against the IMSC HRM',
   long_description=long_description,
   long_description_content_type="text/markdown",
   author='Sandflow Consulting LLC',
   author_email='info@sandflow.com',
   url='https://www.sandflow.com',
   project_urls={
     'Bug Reports': 'https://github.com/sandflow/imscHRM/issues',
     'Source': 'https://github.com/sandflow/imscHRM',
   },
-  install_requires = ["ttconv>=1.0.8-a2"],
+  install_requires = ["ttconv>=1.1.0rc1"],
   classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'Environment :: Console',
         'License :: OSI Approved :: BSD License',
         'Programming Language :: Python :: 3.7',
```

### Comparing `imschrm-1.1.0b6/src/main/python/imschrm/cli.py` & `imschrm-1.1.0rc1/src/main/python/imschrm/cli.py`

 * *Files identical despite different names*

### Comparing `imschrm-1.1.0b6/src/main/python/imschrm/codepoint_sets.py` & `imschrm-1.1.0rc1/src/main/python/imschrm/codepoint_sets.py`

 * *Files identical despite different names*

### Comparing `imschrm-1.1.0b6/src/main/python/imschrm/doc_sequence.py` & `imschrm-1.1.0rc1/src/main/python/imschrm/doc_sequence.py`

 * *Files identical despite different names*

### Comparing `imschrm-1.1.0b6/src/main/python/imschrm/hrm.py` & `imschrm-1.1.0rc1/src/main/python/imschrm/hrm.py`

 * *Files identical despite different names*

### Comparing `imschrm-1.1.0b6/src/main/python/imschrm.egg-info/PKG-INFO` & `imschrm-1.1.0rc1/src/main/python/imschrm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imschrm
-Version: 1.1.0b6
+Version: 1.1.0rc1
 Summary: Validates IMSC documents against the IMSC HRM
 Home-page: https://www.sandflow.com
 Author: Sandflow Consulting LLC
 Author-email: info@sandflow.com
 Project-URL: Bug Reports, https://github.com/sandflow/imscHRM/issues
 Project-URL: Source, https://github.com/sandflow/imscHRM
 Keywords: ttml,imsc,smpte-tt,hrm,complexity
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Multimedia
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: ttconv>=1.0.8-a2
+Requires-Dist: ttconv>=1.1.0rc1
 
 # IMSC Hypothetical Render Model (HRM) Validator
 
      __  _  _  ____   ___  _  _  ____  _  _ 
     (  )( \/ )/ ___) / __)/ )( \(  _ \( \/ )
      )( / \/ \\___ \( (__ ) __ ( )   // \/ \
     (__)\_)(_/(____/ \___)\_)(_/(__\_)\_)(_/
```

### Comparing `imschrm-1.1.0b6/src/main/python/imschrm.egg-info/SOURCES.txt` & `imschrm-1.1.0rc1/src/main/python/imschrm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

