# Comparing `tmp/mloggers-1.3.1.tar.gz` & `tmp/mloggers-1.3.2.tar.gz`

## Comparing `mloggers-1.3.1.tar` & `mloggers-1.3.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 mloggers-1.3.1/.taplo.toml
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 mloggers-1.3.1/log.json
--rw-r--r--   0        0        0    23530 2020-02-02 00:00:00.000000 mloggers-1.3.1/test.ipynb
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 mloggers-1.3.1/test.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 mloggers-1.3.1/mloggers/__init__.py
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 mloggers-1.3.1/mloggers/_log_levels.py
--rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 mloggers-1.3.1/mloggers/console_logger.py
--rw-r--r--   0        0        0     4939 2020-02-02 00:00:00.000000 mloggers-1.3.1/mloggers/file_logger.py
--rw-r--r--   0        0        0     9649 2020-02-02 00:00:00.000000 mloggers-1.3.1/mloggers/logger.py
--rw-r--r--   0        0        0     8703 2020-02-02 00:00:00.000000 mloggers-1.3.1/mloggers/multi_logger.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 mloggers-1.3.1/mloggers/optional_logger.py
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 mloggers-1.3.1/mloggers/progress.py
--rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 mloggers-1.3.1/mloggers/wandb_logger.py
--rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 mloggers-1.3.1/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mloggers-1.3.1/LICENSE
--rw-r--r--   0        0        0     5588 2020-02-02 00:00:00.000000 mloggers-1.3.1/README.md
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 mloggers-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     6324 2020-02-02 00:00:00.000000 mloggers-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 mloggers-1.3.2/.taplo.toml
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 mloggers-1.3.2/log.json
+-rw-r--r--   0        0        0    23530 2020-02-02 00:00:00.000000 mloggers-1.3.2/test.ipynb
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 mloggers-1.3.2/test.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 mloggers-1.3.2/mloggers/__init__.py
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 mloggers-1.3.2/mloggers/_log_levels.py
+-rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 mloggers-1.3.2/mloggers/console_logger.py
+-rw-r--r--   0        0        0     4876 2020-02-02 00:00:00.000000 mloggers-1.3.2/mloggers/file_logger.py
+-rw-r--r--   0        0        0     9649 2020-02-02 00:00:00.000000 mloggers-1.3.2/mloggers/logger.py
+-rw-r--r--   0        0        0     8703 2020-02-02 00:00:00.000000 mloggers-1.3.2/mloggers/multi_logger.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 mloggers-1.3.2/mloggers/optional_logger.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 mloggers-1.3.2/mloggers/progress.py
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 mloggers-1.3.2/mloggers/utils.py
+-rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 mloggers-1.3.2/mloggers/wandb_logger.py
+-rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 mloggers-1.3.2/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mloggers-1.3.2/LICENSE
+-rw-r--r--   0        0        0     5588 2020-02-02 00:00:00.000000 mloggers-1.3.2/README.md
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 mloggers-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     6350 2020-02-02 00:00:00.000000 mloggers-1.3.2/PKG-INFO
```

### Comparing `mloggers-1.3.1/log.json` & `mloggers-1.3.2/log.json`

 * *Files identical despite different names*

### Comparing `mloggers-1.3.1/test.ipynb` & `mloggers-1.3.2/test.ipynb`

 * *Files identical despite different names*

### Comparing `mloggers-1.3.1/mloggers/_log_levels.py` & `mloggers-1.3.2/mloggers/_log_levels.py`

 * *Files identical despite different names*

### Comparing `mloggers-1.3.1/mloggers/console_logger.py` & `mloggers-1.3.2/mloggers/console_logger.py`

 * *Files identical despite different names*

### Comparing `mloggers-1.3.1/mloggers/file_logger.py` & `mloggers-1.3.2/mloggers/file_logger.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import json
 import os
 from datetime import datetime
 from typing import Any
 
-import numpy as np
 import numpy.typing as npt
 from termcolor import colored
 
 from mloggers._log_levels import LogLevel
 from mloggers.logger import Logger
+from mloggers.utils import serialize
 
 
 class FileLogger(Logger):
     """Logs to a file."""
 
     def __init__(
         self,
@@ -71,24 +71,24 @@
             else:
                 for message in messages:
                     self.log(message, level=level)
                 return
         else:
             message = messages[0]
 
-        # Convert numpy's ndarrays to lists so that they are JSON serializable
-        if isinstance(message, np.ndarray):
-            message = message.tolist()
-        if isinstance(message, dict):
-            for key, value in message.items():
-                if isinstance(value, np.ndarray):
-                    message[key] = value.tolist()
-        elif hasattr(message, "__str__") and callable(getattr(message, "__str__")):
-            message = str(message)
+        # JSON-serialize the message
+        try:
+            message = serialize(message)
+        except TypeError as e:
+            print(
+                f'{colored("[ERROR]", "red")} [FileLogger] Could not convert the message to a JSON serializable format: {e}'
+            )
+            return
 
+        # Read the existing logs
         try:
             with open(self._file_path, "r") as file:
                 existing_content = file.read()
                 if (
                     existing_content == ""
                     or existing_content.isspace()
                     or existing_content == "[]"
@@ -105,16 +105,16 @@
                         return
         except Exception as e:
             print(
                 f'{colored("[ERROR]", "red")} [FileLogger] Exception thrown while reading from the logging file: {e}'
             )
             return
 
+        # Create the new log and write it to the file
         new_logs = prev_logs.copy()
-
         try:
             log: dict[str, Any] = {
                 "timestamp": datetime.now().strftime("%d/%m/%Y %H:%M:%S"),
             }
             if level is not None:
                 log["level"] = (
                     level.name if isinstance(level, LogLevel) else str(level).upper()
```

### Comparing `mloggers-1.3.1/mloggers/logger.py` & `mloggers-1.3.2/mloggers/logger.py`

 * *Files identical despite different names*

### Comparing `mloggers-1.3.1/mloggers/multi_logger.py` & `mloggers-1.3.2/mloggers/multi_logger.py`

 * *Files identical despite different names*

### Comparing `mloggers-1.3.1/mloggers/optional_logger.py` & `mloggers-1.3.2/mloggers/optional_logger.py`

 * *Files identical despite different names*

### Comparing `mloggers-1.3.1/mloggers/progress.py` & `mloggers-1.3.2/mloggers/progress.py`

 * *Files identical despite different names*

### Comparing `mloggers-1.3.1/mloggers/wandb_logger.py` & `mloggers-1.3.2/mloggers/wandb_logger.py`

 * *Files identical despite different names*

### Comparing `mloggers-1.3.1/.gitignore` & `mloggers-1.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `mloggers-1.3.1/LICENSE` & `mloggers-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mloggers-1.3.1/README.md` & `mloggers-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `mloggers-1.3.1/pyproject.toml` & `mloggers-1.3.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mloggers"
-version = "1.3.1"
+version = "1.3.2"
 authors = [
     { name = "Sergio Hernandez Gutierrez", email = "contact.sergiohernandez@gmail.com" },
     { name = "Matteo Merler", email = "matteo.merler@gmail.com" },
 ]
 description = "A collection of loggers well-suited for machine learning experiments."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-dependencies = ["aenum", "numpy", "omegaconf", "termcolor", "wandb", "rich"]
+dependencies = [
+    "aenum",
+    "jsonpickle",
+    "numpy",
+    "omegaconf",
+    "termcolor",
+    "wandb",
+    "rich",
+]
 
 [project.urls]
 Homepage = "https://github.com/serhez/mloggers"
 Issues = "https://github.com/serhez/mloggers/issues"
```

### Comparing `mloggers-1.3.1/PKG-INFO` & `mloggers-1.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.3
 Name: mloggers
-Version: 1.3.1
+Version: 1.3.2
 Summary: A collection of loggers well-suited for machine learning experiments.
 Project-URL: Homepage, https://github.com/serhez/mloggers
 Project-URL: Issues, https://github.com/serhez/mloggers/issues
 Author-email: Sergio Hernandez Gutierrez <contact.sergiohernandez@gmail.com>, Matteo Merler <matteo.merler@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: aenum
+Requires-Dist: jsonpickle
 Requires-Dist: numpy
 Requires-Dist: omegaconf
 Requires-Dist: rich
 Requires-Dist: termcolor
 Requires-Dist: wandb
 Description-Content-Type: text/markdown
```

