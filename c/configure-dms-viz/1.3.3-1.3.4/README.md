# Comparing `tmp/configure_dms_viz-1.3.3.tar.gz` & `tmp/configure_dms_viz-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configure_dms_viz-1.3.3.tar", max compression
+gzip compressed data, was "configure_dms_viz-1.3.4.tar", max compression
```

## Comparing `configure_dms_viz-1.3.3.tar` & `configure_dms_viz-1.3.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1095 2024-04-24 21:35:20.863707 configure_dms_viz-1.3.3/LICENSE
--rw-r--r--   0        0        0     9172 2024-04-24 21:35:20.863707 configure_dms_viz-1.3.3/README.md
--rw-r--r--   0        0        0        0 2024-04-24 21:35:20.863707 configure_dms_viz-1.3.3/configure_dms_viz/__init__.py
--rwxr-xr-x   0        0        0    38948 2024-04-24 21:35:20.863707 configure_dms_viz-1.3.3/configure_dms_viz/configure_dms_viz.py
--rw-r--r--   0        0        0     8500 2024-04-24 21:35:20.863707 configure_dms_viz-1.3.3/configure_dms_viz/pdb_utils.py
--rw-r--r--   0        0        0     1454 2024-04-24 21:35:20.867707 configure_dms_viz-1.3.3/pyproject.toml
--rw-r--r--   0        0        0    10199 1970-01-01 00:00:00.000000 configure_dms_viz-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1095 2024-05-15 22:23:18.834303 configure_dms_viz-1.3.4/LICENSE
+-rw-r--r--   0        0        0     9172 2024-05-15 22:23:18.834303 configure_dms_viz-1.3.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-15 22:23:18.834303 configure_dms_viz-1.3.4/configure_dms_viz/__init__.py
+-rwxr-xr-x   0        0        0    38915 2024-05-15 22:23:18.834303 configure_dms_viz-1.3.4/configure_dms_viz/configure_dms_viz.py
+-rw-r--r--   0        0        0     8500 2024-05-15 22:23:18.834303 configure_dms_viz-1.3.4/configure_dms_viz/pdb_utils.py
+-rw-r--r--   0        0        0     1454 2024-05-15 22:23:18.834303 configure_dms_viz-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0    10199 1970-01-01 00:00:00.000000 configure_dms_viz-1.3.4/PKG-INFO
```

### Comparing `configure_dms_viz-1.3.3/LICENSE` & `configure_dms_viz-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `configure_dms_viz-1.3.3/README.md` & `configure_dms_viz-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `configure_dms_viz-1.3.3/configure_dms_viz/configure_dms_viz.py` & `configure_dms_viz-1.3.4/configure_dms_viz/configure_dms_viz.py`

 * *Files 1% similar despite different names*

```diff
@@ -983,21 +983,18 @@
                 combined_data.update(data)
         except Exception as e:
             click.secho(
                 f"Failed to process file {file_path}. Error: {str(e)}", fg="red"
             )
             return
 
-    # Raise an error if the keys in the input files are not unique
-    if len(combined_data) != len(input):
-        click.secho(
-            "The keys in the input files are not unique. Please ensure that the keys are unique.",
-            fg="red",
-        )
-        return
+    # Raise an error if names of the datasets aren't unique
+    combined_data_keys = list(combined_data.keys())
+    if len(combined_data_keys) != len(set(combined_data_keys)):
+        raise ValueError("Names of the datasets are not unique.")
 
     try:
         # Write the combined data to the specified output file
         with open(output, "w") as f:
             json.dump(combined_data, f)
     except Exception as e:
         click.secho(f"Failed to write to output file. Error: {str(e)}", fg="red")
```

### Comparing `configure_dms_viz-1.3.3/configure_dms_viz/pdb_utils.py` & `configure_dms_viz-1.3.4/configure_dms_viz/pdb_utils.py`

 * *Files identical despite different names*

### Comparing `configure_dms_viz-1.3.3/pyproject.toml` & `configure_dms_viz-1.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configure-dms-viz"
-version = "1.3.3"
+version = "1.3.4"
 description = "Configure your data for visualization with dms-viz.github.io"
 authors = ["Will Hannon <hannonww@gmail.com>"]
 maintainers = ["Will Hannon <hannonww@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/dms-viz"
 repository = "https://github.com/dms-viz/configure_dms_viz"
```

### Comparing `configure_dms_viz-1.3.3/PKG-INFO` & `configure_dms_viz-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configure-dms-viz
-Version: 1.3.3
+Version: 1.3.4
 Summary: Configure your data for visualization with dms-viz.github.io
 Home-page: https://github.com/dms-viz
 License: MIT
 Keywords: deep mutational scanning,interactive protein structure,dms-viz,dms,protein
 Author: Will Hannon
 Author-email: hannonww@gmail.com
 Maintainer: Will Hannon
```

