# Comparing `tmp/cpimerge-0.0.4.tar.gz` & `tmp/cpimerge-0.0.5.tar.gz`

## Comparing `cpimerge-0.0.4.tar` & `cpimerge-0.0.5.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpimerge-0.0.4/src/cpimerge/__init__.py
--rw-r--r--   0        0        0    15463 2020-02-02 00:00:00.000000 cpimerge-0.0.4/src/cpimerge/cpimerge.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 cpimerge-0.0.4/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 cpimerge-0.0.4/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpimerge-0.0.4/README.md
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 cpimerge-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 cpimerge-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpimerge-0.0.5/src/cpimerge/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpimerge-0.0.5/src/cpimerge/__main__.py
+-rw-r--r--   0        0        0    15416 2020-02-02 00:00:00.000000 cpimerge-0.0.5/src/cpimerge/cpimerge.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 cpimerge-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 cpimerge-0.0.5/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpimerge-0.0.5/README.md
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 cpimerge-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 cpimerge-0.0.5/PKG-INFO
```

### Comparing `cpimerge-0.0.4/src/cpimerge/cpimerge.py` & `cpimerge-0.0.5/src/cpimerge/cpimerge.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import shutil
 import json
 from datetime import datetime
 from icalendar import Calendar, Event
 import tkinter as tk
 from tkinter import filedialog, messagebox
 from appdirs import user_data_dir
-import __main__
 
 # Define application name and author for appdirs
 APP_NAME = "cpimerge"
 APP_AUTHOR = "Kirk Coombs"
 
 # Get the path to the configuration directory
 config_dir = user_data_dir(APP_NAME, APP_AUTHOR)
@@ -360,9 +359,8 @@
 
 output_text.config(yscrollcommand=scrollbar.set)
 
 # Make the grid cells expand with window resizing
 frame.grid_rowconfigure(6, weight=1)
 frame.grid_columnconfigure(1, weight=1)
 
-if __name__ == '__main__':
-    root.mainloop()
+root.mainloop()
```

### Comparing `cpimerge-0.0.4/.gitignore` & `cpimerge-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `cpimerge-0.0.4/LICENSE` & `cpimerge-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cpimerge-0.0.4/pyproject.toml` & `cpimerge-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cpimerge"
 
-version = "0.0.4"
+version = "0.0.5"
 
 dependencies = [
   "icalendar",
   "appdirs",
 ]
 
 authors = [
```

