# Comparing `tmp/gdriveresolver-0.0.5.tar.gz` & `tmp/gdriveresolver-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdriveresolver-0.0.5.tar", last modified: Tue May 14 21:12:46 2024, max compression
+gzip compressed data, was "gdriveresolver-0.0.6.tar", last modified: Wed May 15 20:04:16 2024, max compression
```

## Comparing `gdriveresolver-0.0.5.tar` & `gdriveresolver-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 harman     (501) staff       (20)        0 2024-05-14 21:12:46.576372 gdriveresolver-0.0.5/
--rw-r--r--   0 harman     (501) staff       (20)     1069 2024-05-14 18:58:35.000000 gdriveresolver-0.0.5/LICENSE
--rw-r--r--   0 harman     (501) staff       (20)     1583 2024-05-14 21:12:46.576218 gdriveresolver-0.0.5/PKG-INFO
--rw-r--r--   0 harman     (501) staff       (20)      972 2024-05-14 21:11:01.000000 gdriveresolver-0.0.5/README.md
-drwxr-xr-x   0 harman     (501) staff       (20)        0 2024-05-14 21:12:46.575278 gdriveresolver-0.0.5/gdriveresolver/
--rw-r--r--   0 harman     (501) staff       (20)       37 2024-05-14 21:11:01.000000 gdriveresolver-0.0.5/gdriveresolver/__init__.py
--rw-r--r--   0 harman     (501) staff       (20)      105 2024-05-14 17:29:08.000000 gdriveresolver-0.0.5/gdriveresolver/exceptions.py
--rw-r--r--   0 harman     (501) staff       (20)     1053 2024-05-14 18:17:17.000000 gdriveresolver-0.0.5/gdriveresolver/model.py
--rw-r--r--   0 harman     (501) staff       (20)      863 2024-05-14 21:12:27.000000 gdriveresolver-0.0.5/gdriveresolver/resolver.py
--rw-r--r--   0 harman     (501) staff       (20)     2805 2024-05-14 19:26:42.000000 gdriveresolver-0.0.5/gdriveresolver/system_operations.py
-drwxr-xr-x   0 harman     (501) staff       (20)        0 2024-05-14 21:12:46.576057 gdriveresolver-0.0.5/gdriveresolver.egg-info/
--rw-r--r--   0 harman     (501) staff       (20)     1583 2024-05-14 21:12:46.000000 gdriveresolver-0.0.5/gdriveresolver.egg-info/PKG-INFO
--rw-r--r--   0 harman     (501) staff       (20)      327 2024-05-14 21:12:46.000000 gdriveresolver-0.0.5/gdriveresolver.egg-info/SOURCES.txt
--rw-r--r--   0 harman     (501) staff       (20)        1 2024-05-14 21:12:46.000000 gdriveresolver-0.0.5/gdriveresolver.egg-info/dependency_links.txt
--rw-r--r--   0 harman     (501) staff       (20)       15 2024-05-14 21:12:46.000000 gdriveresolver-0.0.5/gdriveresolver.egg-info/top_level.txt
--rw-r--r--   0 harman     (501) staff       (20)      683 2024-05-14 21:11:01.000000 gdriveresolver-0.0.5/pyproject.toml
--rw-r--r--   0 harman     (501) staff       (20)       38 2024-05-14 21:12:46.576405 gdriveresolver-0.0.5/setup.cfg
+drwxr-xr-x   0 harman     (501) staff       (20)        0 2024-05-15 20:04:16.867810 gdriveresolver-0.0.6/
+-rw-r--r--   0 harman     (501) staff       (20)     1069 2024-05-14 18:58:35.000000 gdriveresolver-0.0.6/LICENSE
+-rw-r--r--   0 harman     (501) staff       (20)     1583 2024-05-15 20:04:16.867661 gdriveresolver-0.0.6/PKG-INFO
+-rw-r--r--   0 harman     (501) staff       (20)      972 2024-05-14 21:11:01.000000 gdriveresolver-0.0.6/README.md
+drwxr-xr-x   0 harman     (501) staff       (20)        0 2024-05-15 20:04:16.866924 gdriveresolver-0.0.6/gdriveresolver/
+-rw-r--r--   0 harman     (501) staff       (20)       37 2024-05-14 21:11:01.000000 gdriveresolver-0.0.6/gdriveresolver/__init__.py
+-rw-r--r--   0 harman     (501) staff       (20)      105 2024-05-14 17:29:08.000000 gdriveresolver-0.0.6/gdriveresolver/exceptions.py
+-rw-r--r--   0 harman     (501) staff       (20)     1053 2024-05-15 16:16:16.000000 gdriveresolver-0.0.6/gdriveresolver/model.py
+-rw-r--r--   0 harman     (501) staff       (20)     2042 2024-05-15 18:42:59.000000 gdriveresolver-0.0.6/gdriveresolver/resolver.py
+-rw-r--r--   0 harman     (501) staff       (20)     2897 2024-05-15 16:16:16.000000 gdriveresolver-0.0.6/gdriveresolver/system_operations.py
+drwxr-xr-x   0 harman     (501) staff       (20)        0 2024-05-15 20:04:16.867512 gdriveresolver-0.0.6/gdriveresolver.egg-info/
+-rw-r--r--   0 harman     (501) staff       (20)     1583 2024-05-15 20:04:16.000000 gdriveresolver-0.0.6/gdriveresolver.egg-info/PKG-INFO
+-rw-r--r--   0 harman     (501) staff       (20)      357 2024-05-15 20:04:16.000000 gdriveresolver-0.0.6/gdriveresolver.egg-info/SOURCES.txt
+-rw-r--r--   0 harman     (501) staff       (20)        1 2024-05-15 20:04:16.000000 gdriveresolver-0.0.6/gdriveresolver.egg-info/dependency_links.txt
+-rw-r--r--   0 harman     (501) staff       (20)       15 2024-05-15 20:04:16.000000 gdriveresolver-0.0.6/gdriveresolver.egg-info/top_level.txt
+-rw-r--r--   0 harman     (501) staff       (20)      683 2024-05-15 20:04:04.000000 gdriveresolver-0.0.6/pyproject.toml
+-rw-r--r--   0 harman     (501) staff       (20)       38 2024-05-15 20:04:16.867855 gdriveresolver-0.0.6/setup.cfg
+drwxr-xr-x   0 harman     (501) staff       (20)        0 2024-05-15 20:04:16.867366 gdriveresolver-0.0.6/tests/
+-rw-r--r--   0 harman     (501) staff       (20)     4547 2024-05-15 20:03:13.000000 gdriveresolver-0.0.6/tests/test_gdrive_resolver.py
```

### Comparing `gdriveresolver-0.0.5/LICENSE` & `gdriveresolver-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gdriveresolver-0.0.5/PKG-INFO` & `gdriveresolver-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdriveresolver
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package that helps resolve relative Google Drive paths to absolute system paths that refer to the Google drive mount location.
 Author-email: C Harman <charman@netrias.com>
 Project-URL: Homepage, https://github.com/netrias/gdrive_resolver
 Project-URL: Issues, https://github.com/netrias/gdrive_resolver/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gdriveresolver-0.0.5/README.md` & `gdriveresolver-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `gdriveresolver-0.0.5/gdriveresolver/model.py` & `gdriveresolver-0.0.6/gdriveresolver/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     root_search_paths: list[Path]
     platform_name: str
 
 
 windows_definition = OSDefinition(
     name='Windows',
     sanitize_path=lambda file_path: file_path.replace('/', '\\'),
-    root_search_paths=[Path(f"{drive}:\\") for drive in "ABCDEFGHIJKLMNOPQRSTUVWXYZ"],
+    root_search_paths=[Path(f"{drive}:\\") for drive in "CDEFGHIJKLMNOPQRSTUVWXYZAB"],
     platform_name='win'
 )
 
 mac_definition = OSDefinition(
     name='Mac',
     sanitize_path=lambda file_path: file_path.replace('\\', '/'),
     root_search_paths=[Path('/')],
```

### Comparing `gdriveresolver-0.0.5/gdriveresolver/system_operations.py` & `gdriveresolver-0.0.6/gdriveresolver/system_operations.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         return mac_definition
     elif platform.startswith(linux_definition.platform_name):
         return linux_definition
     else:
         raise GDriveNotFoundError("Unsupported operating system.")
 
 
-def locate_google_drive(os_type: OSDefinition, max_depth: int, max_workers: int) -> Path:
+def locate_google_drive(os_type: OSDefinition, max_depth: int, max_workers: int) -> Optional[Path]:
     """
     Locate the Google Drive path by searching the filesystem.
     @param os_type: OSDefinition, the operating system of the current environment.
     @param max_depth: int, maximum depth to search for the Google Drive folder (to avoid long search times).
     @param max_workers: int, maximum number of threads to use for parallel search (to avoid overloading the system).
     """
     search_roots = os_type.root_search_paths
@@ -44,15 +44,17 @@
             try:
                 result = future.result()
                 if result:
                     return result
             except PermissionError:
                 # Skip locations where permission is denied
                 continue
-    raise GDriveNotFoundError(f"Google Drive not found. Searched in {search_roots} up to depth {max_depth}.")
+    print(f"Warning: Google Drive not found. Searched in {search_roots} up to depth {max_depth}.")
+    print("Warning: Paths will be resolved relative to the root directory.")
+    return None
 
 
 def _search_directory_for_drive(search_root: Path, common_names: list, max_depth: int) -> Optional[Path]:
     """Search for Google Drive folder in the specified directory up to a certain depth."""
     for root, dirs, _ in os.walk(search_root):
         depth = len(Path(root).relative_to(search_root).parts)
         if depth > max_depth:
```

### Comparing `gdriveresolver-0.0.5/gdriveresolver.egg-info/PKG-INFO` & `gdriveresolver-0.0.6/gdriveresolver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdriveresolver
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package that helps resolve relative Google Drive paths to absolute system paths that refer to the Google drive mount location.
 Author-email: C Harman <charman@netrias.com>
 Project-URL: Homepage, https://github.com/netrias/gdrive_resolver
 Project-URL: Issues, https://github.com/netrias/gdrive_resolver/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gdriveresolver-0.0.5/pyproject.toml` & `gdriveresolver-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "gdriveresolver"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="C Harman", email="charman@netrias.com" },
 ]
 description = "A package that helps resolve relative Google Drive paths to absolute system paths that refer to the Google drive mount location."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

