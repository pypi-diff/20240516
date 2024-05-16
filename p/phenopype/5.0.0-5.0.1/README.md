# Comparing `tmp/phenopype-5.0.0.tar.gz` & `tmp/phenopype-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phenopype-5.0.0.tar", last modified: Wed May 15 04:00:57 2024, max compression
+gzip compressed data, was "phenopype-5.0.1.tar", last modified: Thu May 16 15:37:32 2024, max compression
```

## Comparing `phenopype-5.0.0.tar` & `phenopype-5.0.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 04:00:57.216616 phenopype-5.0.0/
--rw-rw-rw-   0        0        0     7815 2022-11-18 08:20:39.000000 phenopype-5.0.0/LICENSE
--rw-rw-rw-   0        0        0       28 2022-11-18 08:20:39.000000 phenopype-5.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0    15259 2024-05-15 04:00:57.214621 phenopype-5.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     4998 2023-11-15 10:03:26.000000 phenopype-5.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 04:00:57.078007 phenopype-5.0.0/_temp/
-drwxrwxrwx   0        0        0        0 2024-05-15 04:00:57.107318 phenopype-5.0.0/_temp/docs/
--rw-rw-rw-   0        0        0     3201 2022-05-03 09:06:29.000000 phenopype-5.0.0/_temp/docs/conf.py
-drwxrwxrwx   0        0        0        0 2024-05-15 04:00:57.078007 phenopype-5.0.0/_temp/tests/
-drwxrwxrwx   0        0        0        0 2024-05-15 04:00:57.110956 phenopype-5.0.0/_temp/tests/phenopype-tutorials-main/
--rw-rw-rw-   0        0        0     3104 2024-05-15 03:58:58.000000 phenopype-5.0.0/_temp/tests/phenopype-tutorials-main/conf.py
-drwxrwxrwx   0        0        0        0 2024-05-15 04:00:57.112913 phenopype-5.0.0/docs_source/
--rw-rw-rw-   0        0        0     1617 2024-05-15 03:58:09.000000 phenopype-5.0.0/docs_source/conf.py
-drwxrwxrwx   0        0        0        0 2024-05-15 04:00:57.127305 phenopype-5.0.0/phenopype/
--rw-rw-rw-   0        0        0      471 2024-05-15 03:58:09.000000 phenopype-5.0.0/phenopype/__init__.py
--rw-rw-rw-   0        0        0     5795 2024-05-15 03:58:09.000000 phenopype-5.0.0/phenopype/_vars.py
--rw-rw-rw-   0        0        0       23 2024-05-15 03:57:51.000000 phenopype-5.0.0/phenopype/_version.py
-drwxrwxrwx   0        0        0        0 2024-05-15 04:00:57.153538 phenopype-5.0.0/phenopype/assets/
--rw-rw-rw-   0        0        0    53700 2022-11-18 08:20:40.000000 phenopype-5.0.0/phenopype/assets/wc3_colours.html
--rw-rw-rw-   0        0        0      425 2024-05-15 03:58:09.000000 phenopype-5.0.0/phenopype/config.py
-drwxrwxrwx   0        0        0        0 2024-05-15 04:00:57.162573 phenopype-5.0.0/phenopype/core/
--rw-rw-rw-   0        0        0       79 2022-11-18 08:20:40.000000 phenopype-5.0.0/phenopype/core/__init__.py
--rw-rw-rw-   0        0        0    33750 2024-05-15 03:58:09.000000 phenopype-5.0.0/phenopype/core/export.py
--rw-rw-rw-   0        0        0    21663 2024-05-15 03:58:09.000000 phenopype-5.0.0/phenopype/core/measurement.py
--rw-rw-rw-   0        0        0    35877 2024-05-15 03:58:09.000000 phenopype-5.0.0/phenopype/core/preprocessing.py
--rw-rw-rw-   0        0        0    39405 2024-05-15 03:58:09.000000 phenopype-5.0.0/phenopype/core/segmentation.py
--rw-rw-rw-   0        0        0    31067 2024-05-15 03:58:09.000000 phenopype-5.0.0/phenopype/core/visualization.py
--rw-rw-rw-   0        0        0     2626 2024-05-15 03:58:09.000000 phenopype-5.0.0/phenopype/decorators.py
--rw-rw-rw-   0        0        0   129220 2024-05-15 03:58:09.000000 phenopype-5.0.0/phenopype/main.py
--rw-rw-rw-   0        0        0    32999 2024-05-15 03:58:09.000000 phenopype-5.0.0/phenopype/tracking.py
--rw-rw-rw-   0        0        0    14267 2024-05-15 03:58:09.000000 phenopype-5.0.0/phenopype/utils.py
--rw-rw-rw-   0        0        0   108585 2024-05-15 03:58:09.000000 phenopype-5.0.0/phenopype/utils_lowlevel.py
-drwxrwxrwx   0        0        0        0 2024-05-15 04:00:57.209634 phenopype-5.0.0/phenopype.egg-info/
--rw-rw-rw-   0        0        0    15259 2024-05-15 04:00:56.000000 phenopype-5.0.0/phenopype.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1031 2024-05-15 04:00:57.000000 phenopype-5.0.0/phenopype.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 04:00:56.000000 phenopype-5.0.0/phenopype.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      187 2024-05-15 04:00:56.000000 phenopype-5.0.0/phenopype.egg-info/requires.txt
--rw-rw-rw-   0        0        0       59 2024-05-15 04:00:56.000000 phenopype-5.0.0/phenopype.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1172 2024-05-15 03:58:09.000000 phenopype-5.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-15 04:00:57.217125 phenopype-5.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-15 04:00:57.207199 phenopype-5.0.0/tests/
--rw-rw-rw-   0        0        0        0 2022-11-18 08:20:40.000000 phenopype-5.0.0/tests/__init__.py
--rw-rw-rw-   0        0        0     7326 2024-05-15 03:58:09.000000 phenopype-5.0.0/tests/conftest.py
--rw-rw-rw-   0        0        0     3044 2024-05-15 03:58:09.000000 phenopype-5.0.0/tests/test_01_project.py
--rw-rw-rw-   0        0        0     3603 2024-05-15 03:58:09.000000 phenopype-5.0.0/tests/test_02_core_preprocessing.py
--rw-rw-rw-   0        0        0     2495 2024-05-15 03:58:09.000000 phenopype-5.0.0/tests/test_03_core_segmentation.py
--rw-rw-rw-   0        0        0     1577 2024-05-15 03:58:09.000000 phenopype-5.0.0/tests/test_04_core_measurement.py
--rw-rw-rw-   0        0        0     3867 2024-05-15 03:58:09.000000 phenopype-5.0.0/tests/test_05_core_visualization.py
--rw-rw-rw-   0        0        0     3640 2024-05-15 03:58:09.000000 phenopype-5.0.0/tests/test_06_core_export.py
--rw-rw-rw-   0        0        0     1609 2024-05-15 03:58:09.000000 phenopype-5.0.0/tests/test_07_pype.py
--rw-rw-rw-   0        0        0     3654 2023-11-15 10:03:26.000000 phenopype-5.0.0/tests/test_08_tracking.py
--rw-rw-rw-   0        0        0     2295 2023-11-15 10:03:26.000000 phenopype-5.0.0/tests/test_09_utils.py
--rw-rw-rw-   0        0        0      312 2022-11-18 08:20:40.000000 phenopype-5.0.0/tests/test_10_utils_lowlevel.py
+drwxrwxrwx   0        0        0        0 2024-05-16 15:37:32.463414 phenopype-5.0.1/
+-rw-rw-rw-   0        0        0     7815 2022-04-25 22:33:40.000000 phenopype-5.0.1/LICENSE
+-rw-rw-rw-   0        0        0       28 2023-10-10 22:30:43.000000 phenopype-5.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    15259 2024-05-16 15:37:32.462413 phenopype-5.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4998 2023-10-10 22:30:43.000000 phenopype-5.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 15:37:32.409891 phenopype-5.0.1/_temp/
+drwxrwxrwx   0        0        0        0 2024-05-16 15:37:32.416041 phenopype-5.0.1/_temp/docs/
+-rw-rw-rw-   0        0        0     3201 2023-04-29 09:38:39.000000 phenopype-5.0.1/_temp/docs/conf.py
+drwxrwxrwx   0        0        0        0 2024-05-16 15:37:32.410754 phenopype-5.0.1/_temp/tests/
+drwxrwxrwx   0        0        0        0 2024-05-16 15:37:32.418553 phenopype-5.0.1/_temp/tests/phenopype-tutorials-main/
+-rw-rw-rw-   0        0        0     3104 2024-05-16 15:33:43.000000 phenopype-5.0.1/_temp/tests/phenopype-tutorials-main/conf.py
+drwxrwxrwx   0        0        0        0 2024-05-16 15:37:32.419641 phenopype-5.0.1/docs_source/
+-rw-rw-rw-   0        0        0     1617 2024-05-15 15:11:34.000000 phenopype-5.0.1/docs_source/conf.py
+drwxrwxrwx   0        0        0        0 2024-05-16 15:37:32.427642 phenopype-5.0.1/phenopype/
+-rw-rw-rw-   0        0        0      471 2024-05-15 15:11:34.000000 phenopype-5.0.1/phenopype/__init__.py
+-rw-rw-rw-   0        0        0     5795 2024-05-15 15:10:11.000000 phenopype-5.0.1/phenopype/_vars.py
+-rw-rw-rw-   0        0        0       23 2023-11-20 09:20:30.000000 phenopype-5.0.1/phenopype/_version.py
+drwxrwxrwx   0        0        0        0 2024-05-16 15:37:32.442311 phenopype-5.0.1/phenopype/assets/
+-rw-rw-rw-   0        0        0    53700 2023-10-10 22:30:43.000000 phenopype-5.0.1/phenopype/assets/wc3_colours.html
+-rw-rw-rw-   0        0        0      425 2024-05-15 15:11:34.000000 phenopype-5.0.1/phenopype/config.py
+drwxrwxrwx   0        0        0        0 2024-05-16 15:37:32.448343 phenopype-5.0.1/phenopype/core/
+-rw-rw-rw-   0        0        0       79 2024-04-14 20:07:18.000000 phenopype-5.0.1/phenopype/core/__init__.py
+-rw-rw-rw-   0        0        0    33750 2024-05-15 15:11:34.000000 phenopype-5.0.1/phenopype/core/export.py
+-rw-rw-rw-   0        0        0    21663 2024-05-15 15:10:11.000000 phenopype-5.0.1/phenopype/core/measurement.py
+-rw-rw-rw-   0        0        0    35877 2024-05-15 15:11:34.000000 phenopype-5.0.1/phenopype/core/preprocessing.py
+-rw-rw-rw-   0        0        0    39404 2024-05-16 15:29:59.000000 phenopype-5.0.1/phenopype/core/segmentation.py
+-rw-rw-rw-   0        0        0    31067 2024-05-15 15:10:11.000000 phenopype-5.0.1/phenopype/core/visualization.py
+-rw-rw-rw-   0        0        0     2626 2024-05-15 15:10:11.000000 phenopype-5.0.1/phenopype/decorators.py
+-rw-rw-rw-   0        0        0   129220 2024-05-15 15:11:34.000000 phenopype-5.0.1/phenopype/main.py
+-rw-rw-rw-   0        0        0    32999 2024-05-15 15:10:11.000000 phenopype-5.0.1/phenopype/tracking.py
+-rw-rw-rw-   0        0        0    14327 2024-05-16 15:29:17.000000 phenopype-5.0.1/phenopype/utils.py
+-rw-rw-rw-   0        0        0   108584 2024-05-16 15:30:13.000000 phenopype-5.0.1/phenopype/utils_lowlevel.py
+drwxrwxrwx   0        0        0        0 2024-05-16 15:37:32.460414 phenopype-5.0.1/phenopype.egg-info/
+-rw-rw-rw-   0        0        0    15259 2024-05-16 15:37:32.000000 phenopype-5.0.1/phenopype.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1031 2024-05-16 15:37:32.000000 phenopype-5.0.1/phenopype.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 15:37:32.000000 phenopype-5.0.1/phenopype.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      187 2024-05-16 15:37:32.000000 phenopype-5.0.1/phenopype.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       65 2024-05-16 15:37:32.000000 phenopype-5.0.1/phenopype.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1172 2024-05-16 15:31:28.000000 phenopype-5.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-16 15:37:32.463414 phenopype-5.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-16 15:37:32.459414 phenopype-5.0.1/tests/
+-rw-rw-rw-   0        0        0        0 2022-04-25 22:33:41.000000 phenopype-5.0.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     7326 2024-05-15 15:10:11.000000 phenopype-5.0.1/tests/conftest.py
+-rw-rw-rw-   0        0        0     3044 2024-05-15 15:10:11.000000 phenopype-5.0.1/tests/test_01_project.py
+-rw-rw-rw-   0        0        0     3603 2024-05-15 15:10:11.000000 phenopype-5.0.1/tests/test_02_core_preprocessing.py
+-rw-rw-rw-   0        0        0     2495 2024-05-15 15:10:11.000000 phenopype-5.0.1/tests/test_03_core_segmentation.py
+-rw-rw-rw-   0        0        0     1577 2024-05-15 15:10:11.000000 phenopype-5.0.1/tests/test_04_core_measurement.py
+-rw-rw-rw-   0        0        0     3867 2024-05-15 15:10:11.000000 phenopype-5.0.1/tests/test_05_core_visualization.py
+-rw-rw-rw-   0        0        0     3640 2024-05-15 15:10:11.000000 phenopype-5.0.1/tests/test_06_core_export.py
+-rw-rw-rw-   0        0        0     1609 2024-05-15 15:10:11.000000 phenopype-5.0.1/tests/test_07_pype.py
+-rw-rw-rw-   0        0        0     3654 2023-10-10 22:30:43.000000 phenopype-5.0.1/tests/test_08_tracking.py
+-rw-rw-rw-   0        0        0     2295 2023-11-06 19:00:53.000000 phenopype-5.0.1/tests/test_09_utils.py
+-rw-rw-rw-   0        0        0      312 2022-04-25 22:33:41.000000 phenopype-5.0.1/tests/test_10_utils_lowlevel.py
```

### Comparing `phenopype-5.0.0/LICENSE` & `phenopype-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `phenopype-5.0.0/PKG-INFO` & `phenopype-5.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phenopype
-Version: 5.0.0
+Version: 5.0.1
 Summary: A phenotyping pipeline for python
 Author-email: Moritz Luerig <moritz.luerig@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `phenopype-5.0.0/README.md` & `phenopype-5.0.1/README.md`

 * *Files identical despite different names*

### Comparing `phenopype-5.0.0/_temp/docs/conf.py` & `phenopype-5.0.1/_temp/docs/conf.py`

 * *Files identical despite different names*

### Comparing `phenopype-5.0.0/_temp/tests/phenopype-tutorials-main/conf.py` & `phenopype-5.0.1/_temp/tests/phenopype-tutorials-main/conf.py`

 * *Files identical despite different names*

### Comparing `phenopype-5.0.0/docs_source/conf.py` & `phenopype-5.0.1/docs_source/conf.py`

 * *Files identical despite different names*

### Comparing `phenopype-5.0.0/phenopype/_vars.py` & `phenopype-5.0.1/phenopype/_vars.py`

 * *Files identical despite different names*

### Comparing `phenopype-5.0.0/phenopype/assets/wc3_colours.html` & `phenopype-5.0.1/phenopype/assets/wc3_colours.html`

 * *Files identical despite different names*

### Comparing `phenopype-5.0.0/phenopype/core/export.py` & `phenopype-5.0.1/phenopype/core/export.py`

 * *Files identical despite different names*

### Comparing `phenopype-5.0.0/phenopype/core/measurement.py` & `phenopype-5.0.1/phenopype/core/measurement.py`

 * *Files identical despite different names*

### Comparing `phenopype-5.0.0/phenopype/core/preprocessing.py` & `phenopype-5.0.1/phenopype/core/preprocessing.py`

 * *Files identical despite different names*

### Comparing `phenopype-5.0.0/phenopype/core/segmentation.py` & `phenopype-5.0.1/phenopype/core/segmentation.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
 def detect_contour(
     image,
     approximation="simple",
     retrieval="ext",
     match_against=None,
     apply_drawing=False,
     offset_coords=[0, 0],
-    stats_mode="moments",
+    stats_mode="circle",
     min_nodes=3,
     max_nodes=inf,
     min_area=0,
     max_area=inf,
     min_diameter=0,
     max_diameter=inf,
     **kwargs,
```

### Comparing `phenopype-5.0.0/phenopype/core/visualization.py` & `phenopype-5.0.1/phenopype/core/visualization.py`

 * *Files identical despite different names*

### Comparing `phenopype-5.0.0/phenopype/decorators.py` & `phenopype-5.0.1/phenopype/decorators.py`

 * *Files identical despite different names*

### Comparing `phenopype-5.0.0/phenopype/main.py` & `phenopype-5.0.1/phenopype/main.py`

 * *Files identical despite different names*

### Comparing `phenopype-5.0.0/phenopype/tracking.py` & `phenopype-5.0.1/phenopype/tracking.py`

 * *Files identical despite different names*

### Comparing `phenopype-5.0.0/phenopype/utils.py` & `phenopype-5.0.1/phenopype/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,27 +62,27 @@
                     image = cv2.imread(path, cv2.IMREAD_COLOR)
                 elif flags.mode == "gray":
                     image = cv2.imread(path, cv2.IMREAD_GRAYSCALE)
                 elif flags.mode == "rgb":
                     image = cv2.imread(path)
                     image = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
             else:
-                print(
+                ul._print(
                     'Invalid file extension "{}" - could not load image:\n'.format(ext)
                 )
                 return
         elif os.path.isdir(path):
             image = ul._load_project_image_directory(
                 path, as_container=False
             )
         else:
-            print("Invalid image path - could not load image.")
+            ul._print("Invalid image path - could not load image.")
             return
     else:
-        print("Invalid input format - could not load image.")
+        ul._print("Invalid input format - could not load image.")
         return
 
     return image
 
 
 def load_template(
     template_path,
@@ -127,38 +127,38 @@
         if template_path.__class__.__name__ == "str":
             if os.path.isfile(template_path):
                 template_loaded = ul._load_yaml(template_path)
                 config.template_path_current = template_path
                 config.template_loaded_current = ul._load_yaml(template_path)
 
             else:
-                print("Could not find template_path")
+                ul._print("Could not find template_path")
                 return
         else:
-            print("Wrong input format for template_path")
+            ul._print("Wrong input format for template_path")
             return
     else:
         template_loaded =  config.template_loaded_current
 
     ## construct config-name
     if (
         dir_path.__class__.__name__ == "NoneType"
         and image_path.__class__.__name__ == "NoneType"
     ):
-        print("Need to specify image_path or dir_path")
+        ul._print("Need to specify image_path or dir_path")
         return
 
     elif (
         dir_path.__class__.__name__ == "str"
         and image_path.__class__.__name__ == "NoneType"
     ):
         if os.path.isdir(dir_path):
             prepend = ""
         else:
-            print("Could not find dir_path")
+            ul._print("Could not find dir_path")
             return
 
     elif dir_path.__class__.__name__ == "NoneType":
         dir_path = os.path.dirname(image_path)
         image_name_root = os.path.splitext(os.path.basename(image_path))[0]
         prepend = image_name_root + "_"
 
@@ -335,21 +335,21 @@
     if original_ext:
         file_name = base_name  # Remove original extension if it exists
     file_name_new = f"{file_name}{suffix}{ext}"
     file_path = os.path.join(dir_path, file_name_new)
 
     # Check if file exists and handle overwrite logic
     if os.path.isfile(file_path) and not overwrite:
-        print(f"Image not saved - file already exists (overwrite=False): {file_path}")
+        ul._print(f"Image not saved - file already exists (overwrite=False): {file_path}")
         return False
     else:
         if overwrite and os.path.isfile(file_path):
-            print(f"Image saved and overwritten at: {file_path}")
+            ul._print(f"Image saved and overwritten at: {file_path}")
         else:
-            print(f"Image saved at: {file_path}")
+            ul._print(f"Image saved at: {file_path}")
 
         # Save the image
         success = cv2.imwrite(file_path, image)
         return success
 
 
 
@@ -391,38 +391,38 @@
 
     ## load image
     if image.__class__.__name__ == "ndarray":
         pass
     elif image.__class__.__name__ == "list":
         pass
     else:
-        print("wrong input format.")
+        ul._print("wrong input format.")
         return
 
     ## open images list or single images
     while True:
         if isinstance(image, list):
             if len(image) > 10 and flag_check == True:
                 warning_string = (
                     "WARNING: trying to open "
                     + str(len(image))
                     + " images - proceed (y/n)?"
                 )
                 check = input(warning_string)
                 if check in ["y", "Y", "yes", "Yes"]:
-                    print("Proceed - Opening images ...")
+                    ul._print("Proceed - Opening images ...")
                     pass
                 else:
-                    print("Aborting")
+                    ul._print("Aborting")
                     break
             idx = 0
             for i in image:
                 idx += 1
                 if i.__class__.__name__ == "ndarray":
-                    print("phenopype" + " - " + str(idx))
+                    ul._print("phenopype" + " - " + str(idx))
                     ul._GUI(
                         i,
                         mode="",
                         window_aspect=window_aspect,
                         window_name="phenopype" + " - " + str(idx),
                         window_control="external",
                         **kwargs,
@@ -430,15 +430,15 @@
                     if position_reset == True:
                         cv2.moveWindow(
                             "phenopype" + " - " + str(idx),
                             int(idx + idx * position_offset),
                             int(idx + idx * position_offset),
                         )
                 else:
-                    print("skipped showing list item of type " + i.__class__.__name__)
+                    ul._print("skipped showing list item of type " + i.__class__.__name__)
             cv2.waitKey(0)
             cv2.destroyAllWindows()
             break
         else:
             out = ul._GUI(
                 image=image,
                 mode="",
```

### Comparing `phenopype-5.0.0/phenopype/utils_lowlevel.py` & `phenopype-5.0.1/phenopype/utils_lowlevel.py`

 * *Files 1% similar despite different names*

```diff
@@ -2299,15 +2299,15 @@
         start_x = max(end_x - dim_final, 0)
     if end_y - start_y < dim_final:
         start_y = max(end_y - dim_final, 0)
     
     return image[start_y:end_y, start_x:end_x], (start_y, end_y,start_x,end_x)
 
 
-def _calc_contour_stats(contour, mode="moments"):
+def _calc_contour_stats(contour, mode="circle"):
     if mode=="moments":
         M = cv2.moments(contour)
         cx = int(M["m10"] / M["m00"])
         cy = int(M["m01"] / M["m00"])
         center = [cx, cy]
         # Calculate maximum distance from centroid to contour points for an approximated diameter
         max_dist = max(np.linalg.norm(np.array([px, py]) - np.array(center)) for px, py in contour[:, 0, :])
```

### Comparing `phenopype-5.0.0/phenopype.egg-info/PKG-INFO` & `phenopype-5.0.1/phenopype.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phenopype
-Version: 5.0.0
+Version: 5.0.1
 Summary: A phenotyping pipeline for python
 Author-email: Moritz Luerig <moritz.luerig@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `phenopype-5.0.0/phenopype.egg-info/SOURCES.txt` & `phenopype-5.0.1/phenopype.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phenopype-5.0.0/pyproject.toml` & `phenopype-5.0.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 00000010: 7265 7175 6972 6573 203d 205b 2273 6574  requires = ["set
 00000020: 7570 746f 6f6c 7322 5d0d 0a62 7569 6c64  uptools"]..build
 00000030: 2d62 6163 6b65 6e64 203d 2022 7365 7475  -backend = "setu
 00000040: 7074 6f6f 6c73 2e62 7569 6c64 5f6d 6574  ptools.build_met
 00000050: 6122 0d0a 0d0a 5b70 726f 6a65 6374 5d0d  a"....[project].
 00000060: 0a6e 616d 6520 3d20 2270 6865 6e6f 7079  .name = "phenopy
 00000070: 7065 220d 0a76 6572 7369 6f6e 203d 2022  pe"..version = "
-00000080: 352e 302e 3022 2020 0d0a 6465 7363 7269  5.0.0"  ..descri
+00000080: 352e 302e 3122 2020 0d0a 6465 7363 7269  5.0.1"  ..descri
 00000090: 7074 696f 6e20 3d20 2241 2070 6865 6e6f  ption = "A pheno
 000000a0: 7479 7069 6e67 2070 6970 656c 696e 6520  typing pipeline 
 000000b0: 666f 7220 7079 7468 6f6e 220d 0a72 6561  for python"..rea
 000000c0: 646d 6520 3d20 2252 4541 444d 452e 6d64  dme = "README.md
 000000d0: 220d 0a61 7574 686f 7273 203d 205b 0d0a  "..authors = [..
 000000e0: 2020 2020 7b6e 616d 6520 3d20 224d 6f72      {name = "Mor
 000000f0: 6974 7a20 4c75 6572 6967 222c 2065 6d61  itz Luerig", ema
```

### Comparing `phenopype-5.0.0/tests/conftest.py` & `phenopype-5.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `phenopype-5.0.0/tests/test_01_project.py` & `phenopype-5.0.1/tests/test_01_project.py`

 * *Files identical despite different names*

### Comparing `phenopype-5.0.0/tests/test_02_core_preprocessing.py` & `phenopype-5.0.1/tests/test_02_core_preprocessing.py`

 * *Files identical despite different names*

### Comparing `phenopype-5.0.0/tests/test_03_core_segmentation.py` & `phenopype-5.0.1/tests/test_03_core_segmentation.py`

 * *Files identical despite different names*

### Comparing `phenopype-5.0.0/tests/test_04_core_measurement.py` & `phenopype-5.0.1/tests/test_04_core_measurement.py`

 * *Files identical despite different names*

### Comparing `phenopype-5.0.0/tests/test_05_core_visualization.py` & `phenopype-5.0.1/tests/test_05_core_visualization.py`

 * *Files identical despite different names*

### Comparing `phenopype-5.0.0/tests/test_06_core_export.py` & `phenopype-5.0.1/tests/test_06_core_export.py`

 * *Files identical despite different names*

### Comparing `phenopype-5.0.0/tests/test_07_pype.py` & `phenopype-5.0.1/tests/test_07_pype.py`

 * *Files identical despite different names*

### Comparing `phenopype-5.0.0/tests/test_08_tracking.py` & `phenopype-5.0.1/tests/test_08_tracking.py`

 * *Files identical despite different names*

### Comparing `phenopype-5.0.0/tests/test_09_utils.py` & `phenopype-5.0.1/tests/test_09_utils.py`

 * *Files identical despite different names*

