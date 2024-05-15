# Comparing `tmp/com_castsoftware_uc_oneclick-1.0.4.tar.gz` & `tmp/com_castsoftware_uc_oneclick-1.0.4b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "com_castsoftware_uc_oneclick-1.0.4.tar", last modified: Wed May 15 22:22:59 2024, max compression
+gzip compressed data, was "com_castsoftware_uc_oneclick-1.0.4b1.tar", last modified: Mon May  6 15:56:57 2024, max compression
```

## Comparing `com_castsoftware_uc_oneclick-1.0.4.tar` & `com_castsoftware_uc_oneclick-1.0.4b1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 22:22:59.901246 com_castsoftware_uc_oneclick-1.0.4/
--rw-rw-rw-   0        0        0      982 2024-05-15 22:22:59.824519 com_castsoftware_uc_oneclick-1.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-15 22:22:59.812351 com_castsoftware_uc_oneclick-1.0.4/com.castsoftware.uc.oneclick.egg-info/
--rw-rw-rw-   0        0        0      982 2024-05-15 22:22:59.000000 com_castsoftware_uc_oneclick-1.0.4/com.castsoftware.uc.oneclick.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      867 2024-05-15 22:22:59.000000 com_castsoftware_uc_oneclick-1.0.4/com.castsoftware.uc.oneclick.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 22:22:59.000000 com_castsoftware_uc_oneclick-1.0.4/com.castsoftware.uc.oneclick.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      227 2024-05-15 22:22:59.000000 com_castsoftware_uc_oneclick-1.0.4/com.castsoftware.uc.oneclick.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-15 22:22:59.000000 com_castsoftware_uc_oneclick-1.0.4/com.castsoftware.uc.oneclick.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-15 22:22:59.576663 com_castsoftware_uc_oneclick-1.0.4/oneclick/
--rw-rw-rw-   0        0        0        2 2024-02-13 17:42:06.000000 com_castsoftware_uc_oneclick-1.0.4/oneclick/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 22:22:59.679802 com_castsoftware_uc_oneclick-1.0.4/oneclick/analysis/
--rw-rw-rw-   0        0        0        0 2024-02-13 17:42:06.000000 com_castsoftware_uc_oneclick-1.0.4/oneclick/analysis/__init__.py
--rw-rw-rw-   0        0        0     2970 2024-04-24 18:58:40.000000 com_castsoftware_uc_oneclick-1.0.4/oneclick/analysis/aip_analysis.py
--rw-rw-rw-   0        0        0     1308 2024-02-22 13:23:04.000000 com_castsoftware_uc_oneclick-1.0.4/oneclick/analysis/analysis.py
--rw-rw-rw-   0        0        0     4288 2024-04-24 18:58:40.000000 com_castsoftware_uc_oneclick-1.0.4/oneclick/analysis/highlight_analysis.py
--rw-rw-rw-   0        0        0     4964 2024-04-24 18:58:40.000000 com_castsoftware_uc_oneclick-1.0.4/oneclick/analysis/trackAnalysis.py
--rw-rw-rw-   0        0        0    26252 2024-04-24 21:10:55.000000 com_castsoftware_uc_oneclick-1.0.4/oneclick/config.py
-drwxrwxrwx   0        0        0        0 2024-05-15 22:22:59.796122 com_castsoftware_uc_oneclick-1.0.4/oneclick/discovery/
--rw-rw-rw-   0        0        0        0 2024-02-13 17:42:06.000000 com_castsoftware_uc_oneclick-1.0.4/oneclick/discovery/__init__.py
--rw-rw-rw-   0        0        0     4907 2024-04-24 18:58:40.000000 com_castsoftware_uc_oneclick-1.0.4/oneclick/discovery/cleanup.py
--rw-rw-rw-   0        0        0    10901 2024-04-24 18:58:40.000000 com_castsoftware_uc_oneclick-1.0.4/oneclick/discovery/cloc.py
--rw-rw-rw-   0        0        0     9689 2024-04-24 18:58:40.000000 com_castsoftware_uc_oneclick-1.0.4/oneclick/discovery/discoveryReport.py
--rw-rw-rw-   0        0        0     3853 2024-04-24 21:29:48.000000 com_castsoftware_uc_oneclick-1.0.4/oneclick/discovery/prep.py
--rw-rw-rw-   0        0        0     4746 2024-02-13 17:42:06.000000 com_castsoftware_uc_oneclick-1.0.4/oneclick/discovery/profiler.py
--rw-rw-rw-   0        0        0      498 2024-02-22 13:23:04.000000 com_castsoftware_uc_oneclick-1.0.4/oneclick/discovery/sourceValidation.py
--rw-rw-rw-   0        0        0     7069 2024-04-24 18:58:40.000000 com_castsoftware_uc_oneclick-1.0.4/oneclick/discovery/sqlDiscovery.py
--rw-rw-rw-   0        0        0     5765 2024-05-06 16:53:45.000000 com_castsoftware_uc_oneclick-1.0.4/oneclick/discovery/unzip.py
--rw-rw-rw-   0        0        0      305 2024-02-13 17:42:07.000000 com_castsoftware_uc_oneclick-1.0.4/oneclick/exceptions.py
--rw-rw-rw-   0        0        0    11405 2024-04-24 21:36:38.000000 com_castsoftware_uc_oneclick-1.0.4/oneclick/main.py
--rw-rw-rw-   0        0        0     2225 2024-02-22 13:23:04.000000 com_castsoftware_uc_oneclick-1.0.4/oneclick/runArg.py
--rw-rw-rw-   0        0        0     2098 2024-02-13 17:42:07.000000 com_castsoftware_uc_oneclick-1.0.4/oneclick/sendEmail.py
--rw-rw-rw-   0        0        0     4251 2024-02-13 17:42:07.000000 com_castsoftware_uc_oneclick-1.0.4/oneclick/setup.py
--rw-rw-rw-   0        0        0      832 2024-05-15 22:22:22.000000 com_castsoftware_uc_oneclick-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-15 22:22:59.901246 com_castsoftware_uc_oneclick-1.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-06 15:56:57.189332 com_castsoftware_uc_oneclick-1.0.4b1/
+-rw-rw-rw-   0        0        0      984 2024-05-06 15:56:57.169062 com_castsoftware_uc_oneclick-1.0.4b1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-06 15:56:57.151024 com_castsoftware_uc_oneclick-1.0.4b1/com.castsoftware.uc.oneclick.egg-info/
+-rw-rw-rw-   0        0        0      984 2024-05-06 15:56:56.000000 com_castsoftware_uc_oneclick-1.0.4b1/com.castsoftware.uc.oneclick.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      867 2024-05-06 15:56:56.000000 com_castsoftware_uc_oneclick-1.0.4b1/com.castsoftware.uc.oneclick.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 15:56:56.000000 com_castsoftware_uc_oneclick-1.0.4b1/com.castsoftware.uc.oneclick.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      227 2024-05-06 15:56:56.000000 com_castsoftware_uc_oneclick-1.0.4b1/com.castsoftware.uc.oneclick.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-06 15:56:56.000000 com_castsoftware_uc_oneclick-1.0.4b1/com.castsoftware.uc.oneclick.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 15:56:56.881462 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/
+-rw-rw-rw-   0        0        0        2 2024-02-13 17:42:06.000000 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 15:56:56.949232 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/analysis/
+-rw-rw-rw-   0        0        0        0 2024-02-13 17:42:06.000000 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/analysis/__init__.py
+-rw-rw-rw-   0        0        0     2970 2024-04-24 18:58:40.000000 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/analysis/aip_analysis.py
+-rw-rw-rw-   0        0        0     1308 2024-02-22 13:23:04.000000 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/analysis/analysis.py
+-rw-rw-rw-   0        0        0     4288 2024-04-24 18:58:40.000000 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/analysis/highlight_analysis.py
+-rw-rw-rw-   0        0        0     4964 2024-04-24 18:58:40.000000 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/analysis/trackAnalysis.py
+-rw-rw-rw-   0        0        0    26252 2024-04-24 21:10:55.000000 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/config.py
+drwxrwxrwx   0        0        0        0 2024-05-06 15:56:57.131412 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/discovery/
+-rw-rw-rw-   0        0        0        0 2024-02-13 17:42:06.000000 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/discovery/__init__.py
+-rw-rw-rw-   0        0        0     4907 2024-04-24 18:58:40.000000 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/discovery/cleanup.py
+-rw-rw-rw-   0        0        0    10901 2024-04-24 18:58:40.000000 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/discovery/cloc.py
+-rw-rw-rw-   0        0        0     9689 2024-04-24 18:58:40.000000 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/discovery/discoveryReport.py
+-rw-rw-rw-   0        0        0     3853 2024-04-24 21:29:48.000000 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/discovery/prep.py
+-rw-rw-rw-   0        0        0     4746 2024-02-13 17:42:06.000000 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/discovery/profiler.py
+-rw-rw-rw-   0        0        0      498 2024-02-22 13:23:04.000000 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/discovery/sourceValidation.py
+-rw-rw-rw-   0        0        0     7069 2024-04-24 18:58:40.000000 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/discovery/sqlDiscovery.py
+-rw-rw-rw-   0        0        0     5753 2024-04-24 18:58:40.000000 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/discovery/unzip.py
+-rw-rw-rw-   0        0        0      305 2024-02-13 17:42:07.000000 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/exceptions.py
+-rw-rw-rw-   0        0        0    11405 2024-04-24 21:36:38.000000 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/main.py
+-rw-rw-rw-   0        0        0     2225 2024-02-22 13:23:04.000000 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/runArg.py
+-rw-rw-rw-   0        0        0     2098 2024-02-13 17:42:07.000000 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/sendEmail.py
+-rw-rw-rw-   0        0        0     4251 2024-02-13 17:42:07.000000 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/setup.py
+-rw-rw-rw-   0        0        0      839 2024-05-06 15:51:04.000000 com_castsoftware_uc_oneclick-1.0.4b1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-06 15:56:57.189332 com_castsoftware_uc_oneclick-1.0.4b1/setup.cfg
```

### Comparing `com_castsoftware_uc_oneclick-1.0.4/PKG-INFO` & `com_castsoftware_uc_oneclick-1.0.4b1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.oneclick
-Version: 1.0.4
+Version: 1.0.4b1
 Summary: Assessment Generator
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.arg
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.arg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -17,10 +17,10 @@
 Requires-Dist: pyunpack
 Requires-Dist: tqdm
 Requires-Dist: patool
 Requires-Dist: archive
 Requires-Dist: pypiwin32
 Requires-Dist: psycopg2
 Requires-Dist: openpyxl
-Requires-Dist: com.castsoftware.uc.python.common>=1.1.12
+Requires-Dist: com.castsoftware.uc.python.common>=1.1.11
 Requires-Dist: com.castsoftware.uc.action-plan
-Requires-Dist: com.castsoftware.uc.arg>=1.7.4
+Requires-Dist: com.castsoftware.uc.arg>=1.6.2
```

### Comparing `com_castsoftware_uc_oneclick-1.0.4/com.castsoftware.uc.oneclick.egg-info/PKG-INFO` & `com_castsoftware_uc_oneclick-1.0.4b1/com.castsoftware.uc.oneclick.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.oneclick
-Version: 1.0.4
+Version: 1.0.4b1
 Summary: Assessment Generator
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.arg
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.arg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -17,10 +17,10 @@
 Requires-Dist: pyunpack
 Requires-Dist: tqdm
 Requires-Dist: patool
 Requires-Dist: archive
 Requires-Dist: pypiwin32
 Requires-Dist: psycopg2
 Requires-Dist: openpyxl
-Requires-Dist: com.castsoftware.uc.python.common>=1.1.12
+Requires-Dist: com.castsoftware.uc.python.common>=1.1.11
 Requires-Dist: com.castsoftware.uc.action-plan
-Requires-Dist: com.castsoftware.uc.arg>=1.7.4
+Requires-Dist: com.castsoftware.uc.arg>=1.6.2
```

### Comparing `com_castsoftware_uc_oneclick-1.0.4/com.castsoftware.uc.oneclick.egg-info/SOURCES.txt` & `com_castsoftware_uc_oneclick-1.0.4b1/com.castsoftware.uc.oneclick.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_oneclick-1.0.4/oneclick/analysis/aip_analysis.py` & `com_castsoftware_uc_oneclick-1.0.4b1/oneclick/analysis/aip_analysis.py`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_oneclick-1.0.4/oneclick/analysis/analysis.py` & `com_castsoftware_uc_oneclick-1.0.4b1/oneclick/analysis/analysis.py`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_oneclick-1.0.4/oneclick/analysis/highlight_analysis.py` & `com_castsoftware_uc_oneclick-1.0.4b1/oneclick/analysis/highlight_analysis.py`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_oneclick-1.0.4/oneclick/analysis/trackAnalysis.py` & `com_castsoftware_uc_oneclick-1.0.4b1/oneclick/analysis/trackAnalysis.py`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_oneclick-1.0.4/oneclick/config.py` & `com_castsoftware_uc_oneclick-1.0.4b1/oneclick/config.py`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_oneclick-1.0.4/oneclick/discovery/cleanup.py` & `com_castsoftware_uc_oneclick-1.0.4b1/oneclick/discovery/cleanup.py`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_oneclick-1.0.4/oneclick/discovery/cloc.py` & `com_castsoftware_uc_oneclick-1.0.4b1/oneclick/discovery/cloc.py`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_oneclick-1.0.4/oneclick/discovery/discoveryReport.py` & `com_castsoftware_uc_oneclick-1.0.4b1/oneclick/discovery/discoveryReport.py`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_oneclick-1.0.4/oneclick/discovery/prep.py` & `com_castsoftware_uc_oneclick-1.0.4b1/oneclick/discovery/prep.py`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_oneclick-1.0.4/oneclick/discovery/profiler.py` & `com_castsoftware_uc_oneclick-1.0.4b1/oneclick/discovery/profiler.py`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_oneclick-1.0.4/oneclick/discovery/sqlDiscovery.py` & `com_castsoftware_uc_oneclick-1.0.4b1/oneclick/discovery/sqlDiscovery.py`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_oneclick-1.0.4/oneclick/discovery/unzip.py` & `com_castsoftware_uc_oneclick-1.0.4b1/oneclick/discovery/unzip.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
                   elif file.endswith(".7z") or file.endswith(".zip") :
                      archived_files += 1
                      found = True
                      full_name = abspath(f'{root.strip()}\\{file}')
                      create_folder(dest)
                      with ZipFile(full_name) as zf:
-                        for member in tqdm(zf.infolist(), desc=f'Extracting {full_name}',position=0,leave=False):
+                        for member in tqdm(zf.infolist(), desc='Extracting ',position=0,leave=False):
                            zf.extract(member, dest)
                      #Archive(full_name).extractall(dest,auto_create_dir=True)
 
                   else:
                      unarchived_files += 1
 
                   if found:
```

### Comparing `com_castsoftware_uc_oneclick-1.0.4/oneclick/main.py` & `com_castsoftware_uc_oneclick-1.0.4b1/oneclick/main.py`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_oneclick-1.0.4/oneclick/runArg.py` & `com_castsoftware_uc_oneclick-1.0.4b1/oneclick/runArg.py`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_oneclick-1.0.4/oneclick/sendEmail.py` & `com_castsoftware_uc_oneclick-1.0.4b1/oneclick/sendEmail.py`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_oneclick-1.0.4/oneclick/setup.py` & `com_castsoftware_uc_oneclick-1.0.4b1/oneclick/setup.py`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_oneclick-1.0.4/pyproject.toml` & `com_castsoftware_uc_oneclick-1.0.4b1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [project]
 name='com.castsoftware.uc.oneclick'
 description="Assessment Generator"
-version='1.0.4' #prod version
+version='1.0.4-beta-1' #prod version
 dependencies = [
     'pandas','python-pptx==0.6.18','python-docx',
     'argparse_formatter','django','pyunpack','tqdm',
     'patool','archive','pypiwin32','psycopg2','openpyxl',
-    'com.castsoftware.uc.python.common>=1.1.12',
+    'com.castsoftware.uc.python.common>=1.1.11',
     'com.castsoftware.uc.action-plan',
-    'com.castsoftware.uc.arg>=1.7.4'    
+    'com.castsoftware.uc.arg>=1.6.2'    
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
```

