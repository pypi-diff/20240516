# Comparing `tmp/inception_reports-0.3.tar.gz` & `tmp/inception_reports-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inception_reports-0.3.tar", last modified: Wed May 15 12:08:50 2024, max compression
+gzip compressed data, was "inception_reports-0.3.1.tar", last modified: Thu May 16 09:44:35 2024, max compression
```

## Comparing `inception_reports-0.3.tar` & `inception_reports-0.3.1.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 basch    (1060118464) domänen-benutzer (1060110849)        0 2024-05-15 12:08:50.084482 inception_reports-0.3/
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)    11357 2023-09-25 12:56:28.000000 inception_reports-0.3/LICENSE
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)      752 2023-11-07 13:15:00.000000 inception_reports-0.3/NOTICE.txt
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     2063 2024-05-15 12:08:50.084482 inception_reports-0.3/PKG-INFO
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     1376 2024-04-30 00:10:18.000000 inception_reports-0.3/README.md
-drwxr-xr-x   0 basch    (1060118464) domänen-benutzer (1060110849)        0 2024-05-15 12:08:50.080482 inception_reports-0.3/inception_reports/
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)      769 2024-04-02 01:14:36.000000 inception_reports-0.3/inception_reports/__init__.py
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     1704 2024-04-29 23:24:38.000000 inception_reports-0.3/inception_reports/__main__.py
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     6889 2024-05-15 10:52:10.000000 inception_reports-0.3/inception_reports/generate_reports_lead.py
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)    17113 2024-05-15 10:59:21.000000 inception_reports-0.3/inception_reports/generate_reports_manager.py
-drwxr-xr-x   0 basch    (1060118464) domänen-benutzer (1060110849)        0 2024-05-15 12:08:50.084482 inception_reports-0.3/inception_reports.egg-info/
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     2063 2024-05-15 12:08:50.000000 inception_reports-0.3/inception_reports.egg-info/PKG-INFO
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)      515 2024-05-15 12:08:50.000000 inception_reports-0.3/inception_reports.egg-info/SOURCES.txt
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)        1 2024-05-15 12:08:50.000000 inception_reports-0.3/inception_reports.egg-info/dependency_links.txt
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)       70 2024-05-15 12:08:50.000000 inception_reports-0.3/inception_reports.egg-info/entry_points.txt
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)       52 2024-05-15 12:08:50.000000 inception_reports-0.3/inception_reports.egg-info/requires.txt
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)       18 2024-05-15 12:08:50.000000 inception_reports-0.3/inception_reports.egg-info/top_level.txt
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)      792 2024-05-15 12:08:08.000000 inception_reports-0.3/pyproject.toml
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)       38 2024-05-15 12:08:50.084482 inception_reports-0.3/setup.cfg
-drwxr-xr-x   0 basch    (1060118464) domänen-benutzer (1060110849)        0 2024-05-15 12:08:50.084482 inception_reports-0.3/tests/
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     3565 2024-05-15 09:37:35.000000 inception_reports-0.3/tests/test_generate_reports_lead.py
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     4262 2024-05-07 01:00:49.000000 inception_reports-0.3/tests/test_generate_reports_manager.py
+drwxr-xr-x   0 basch    (1060118464) domänen-benutzer (1060110849)        0 2024-05-16 09:44:35.994131 inception_reports-0.3.1/
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)    11357 2023-09-25 12:56:28.000000 inception_reports-0.3.1/LICENSE
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)      752 2023-11-07 13:15:00.000000 inception_reports-0.3.1/NOTICE.txt
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     2065 2024-05-16 09:44:35.994131 inception_reports-0.3.1/PKG-INFO
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     1376 2024-04-30 00:10:18.000000 inception_reports-0.3.1/README.md
+drwxr-xr-x   0 basch    (1060118464) domänen-benutzer (1060110849)        0 2024-05-16 09:44:35.994131 inception_reports-0.3.1/inception_reports/
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)      769 2024-04-02 01:14:36.000000 inception_reports-0.3.1/inception_reports/__init__.py
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     1704 2024-04-29 23:24:38.000000 inception_reports-0.3.1/inception_reports/__main__.py
+drwxr-xr-x   0 basch    (1060118464) domänen-benutzer (1060110849)        0 2024-05-16 09:44:35.994131 inception_reports-0.3.1/inception_reports/data/
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)      769 2024-05-16 09:38:16.000000 inception_reports-0.3.1/inception_reports/data/__init__.py
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     6443 2024-05-16 09:44:28.000000 inception_reports-0.3.1/inception_reports/generate_reports_lead.py
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)    16666 2024-05-16 09:44:22.000000 inception_reports-0.3.1/inception_reports/generate_reports_manager.py
+drwxr-xr-x   0 basch    (1060118464) domänen-benutzer (1060110849)        0 2024-05-16 09:44:35.994131 inception_reports-0.3.1/inception_reports.egg-info/
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     2065 2024-05-16 09:44:35.000000 inception_reports-0.3.1/inception_reports.egg-info/PKG-INFO
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)      550 2024-05-16 09:44:35.000000 inception_reports-0.3.1/inception_reports.egg-info/SOURCES.txt
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)        1 2024-05-16 09:44:35.000000 inception_reports-0.3.1/inception_reports.egg-info/dependency_links.txt
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)       70 2024-05-16 09:44:35.000000 inception_reports-0.3.1/inception_reports.egg-info/entry_points.txt
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)       52 2024-05-16 09:44:35.000000 inception_reports-0.3.1/inception_reports.egg-info/requires.txt
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)       18 2024-05-16 09:44:35.000000 inception_reports-0.3.1/inception_reports.egg-info/top_level.txt
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)      794 2024-05-16 09:43:16.000000 inception_reports-0.3.1/pyproject.toml
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)       38 2024-05-16 09:44:35.994131 inception_reports-0.3.1/setup.cfg
+drwxr-xr-x   0 basch    (1060118464) domänen-benutzer (1060110849)        0 2024-05-16 09:44:35.994131 inception_reports-0.3.1/tests/
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     3565 2024-05-15 09:37:35.000000 inception_reports-0.3.1/tests/test_generate_reports_lead.py
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     4262 2024-05-07 01:00:49.000000 inception_reports-0.3.1/tests/test_generate_reports_manager.py
```

### Comparing `inception_reports-0.3/LICENSE` & `inception_reports-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `inception_reports-0.3/NOTICE.txt` & `inception_reports-0.3.1/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `inception_reports-0.3/PKG-INFO` & `inception_reports-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inception_reports
-Version: 0.3
+Version: 0.3.1
 Summary: Generate plots that report the progress of an INCEpTION project.
 Author-email: Serwar <serwar.basch@tu-darmstadt.de>
 Project-URL: Homepage, https://github.com/inception-project/inception-reporting-dashboard
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `inception_reports-0.3/README.md` & `inception_reports-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `inception_reports-0.3/inception_reports/__init__.py` & `inception_reports-0.3.1/inception_reports/__init__.py`

 * *Files identical despite different names*

### Comparing `inception_reports-0.3/inception_reports/__main__.py` & `inception_reports-0.3.1/inception_reports/__main__.py`

 * *Files identical despite different names*

### Comparing `inception_reports-0.3/inception_reports/generate_reports_lead.py` & `inception_reports-0.3.1/inception_reports/generate_reports_lead.py`

 * *Files 20% similar despite different names*

```diff
@@ -37,27 +37,14 @@
     st.rerun()
 
 
 def startup():
 
     st.markdown(
         """
-        <style>
-        body {
-            cursor: url('https://cdn-icons-png.flaticon.com/64/5198/5198523.png'), auto !important;
-        }
-
-        rect.legendtoggle {
-            cursor: url('https://cdn-icons-png.flaticon.com/32/12179/12179477.png'), pointer !important;
-        }
-
-        rect.nsewdrag.drag {
-            cursor: url('https://cdn-icons-png.flaticon.com/32/10263/10263093.png'), pointer !important;
-        }
-        </style>
 
         <style>
         .block-container {
             padding-top: 0rem;
             padding-bottom: 5rem;
             padding-left: 5rem;
             padding-right: 5rem;
@@ -201,15 +188,15 @@
     """
 
     st.sidebar.write(
         "Please input the path to the folder containing the INCEpTION projects."
     )
     projects_folder = st.sidebar.text_input(
         "Projects Folder:",
-        value="/home/basch/Documents/projects/exported_data_2024_05_13/",
+        value="/home/basch/Documents/projects/gemtex_demo_exported_data/",
     )
     button = st.sidebar.button("Generate Reports")
     if button:
         st.session_state["initialized"] = True
         st.session_state["projects"] = read_dir(projects_folder)
         button = False
         set_sidebar_state("collapsed")
```

### Comparing `inception_reports-0.3/inception_reports/generate_reports_manager.py` & `inception_reports-0.3.1/inception_reports/generate_reports_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,27 +43,14 @@
     st.rerun()
 
 
 def startup():
 
     st.markdown(
         """
-        <style>
-        body {
-            cursor: url('https://cdn-icons-png.flaticon.com/64/5198/5198523.png'), auto !important;
-        }
-
-        rect.legendtoggle {
-            cursor: url('https://cdn-icons-png.flaticon.com/32/12179/12179477.png'), pointer !important;
-        }
-
-        rect.nsewdrag.drag {
-            cursor: url('https://cdn-icons-png.flaticon.com/32/10263/10263093.png'), pointer !important;
-        }
-        </style>
 
         <style>
         .block-container {
             padding-top: 0rem;
             padding-bottom: 5rem;
             padding-left: 5rem;
             padding-right: 5rem;
```

### Comparing `inception_reports-0.3/inception_reports.egg-info/PKG-INFO` & `inception_reports-0.3.1/inception_reports.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inception_reports
-Version: 0.3
+Version: 0.3.1
 Summary: Generate plots that report the progress of an INCEpTION project.
 Author-email: Serwar <serwar.basch@tu-darmstadt.de>
 Project-URL: Homepage, https://github.com/inception-project/inception-reporting-dashboard
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `inception_reports-0.3/inception_reports.egg-info/SOURCES.txt` & `inception_reports-0.3.1/inception_reports.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,9 +8,10 @@
 inception_reports/generate_reports_manager.py
 inception_reports.egg-info/PKG-INFO
 inception_reports.egg-info/SOURCES.txt
 inception_reports.egg-info/dependency_links.txt
 inception_reports.egg-info/entry_points.txt
 inception_reports.egg-info/requires.txt
 inception_reports.egg-info/top_level.txt
+inception_reports/data/__init__.py
 tests/test_generate_reports_lead.py
 tests/test_generate_reports_manager.py
```

### Comparing `inception_reports-0.3/pyproject.toml` & `inception_reports-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "inception_reports"
 description = "Generate plots that report the progress of an INCEpTION project."
-version = "0.3"
+version = "0.3.1"
 authors = [
     { name = "Serwar", email = "serwar.basch@tu-darmstadt.de" }
 ]
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = [
     "streamlit",
```

### Comparing `inception_reports-0.3/tests/test_generate_reports_lead.py` & `inception_reports-0.3.1/tests/test_generate_reports_lead.py`

 * *Files identical despite different names*

### Comparing `inception_reports-0.3/tests/test_generate_reports_manager.py` & `inception_reports-0.3.1/tests/test_generate_reports_manager.py`

 * *Files identical despite different names*

