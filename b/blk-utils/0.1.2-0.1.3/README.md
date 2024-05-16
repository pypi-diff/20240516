# Comparing `tmp/blk-utils-0.1.2.tar.gz` & `tmp/blk_utils-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blk-utils-0.1.2.tar", last modified: Sun Oct  1 15:29:31 2023, max compression
+gzip compressed data, was "blk_utils-0.1.3.tar", last modified: Thu May 16 16:57:00 2024, max compression
```

## Comparing `blk-utils-0.1.2.tar` & `blk_utils-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-10-01 15:29:31.267664 blk-utils-0.1.2/
--rw-rw-rw-   0        0        0     4073 2023-04-14 17:28:18.000000 blk-utils-0.1.2/.gitignore
--rw-rw-rw-   0        0        0     1266 2023-10-01 15:29:31.266664 blk-utils-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      472 2023-04-14 17:36:30.000000 blk-utils-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-10-01 15:29:31.137081 blk-utils-0.1.2/blk_utils/
--rw-rw-rw-   0        0        0      130 2023-10-01 15:29:18.000000 blk-utils-0.1.2/blk_utils/__init__.py
--rw-rw-rw-   0        0        0     3969 2023-10-01 13:38:59.000000 blk-utils-0.1.2/blk_utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-10-01 15:29:31.261664 blk-utils-0.1.2/blk_utils.egg-info/
--rw-rw-rw-   0        0        0     1266 2023-10-01 15:29:30.000000 blk-utils-0.1.2/blk_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      289 2023-10-01 15:29:30.000000 blk-utils-0.1.2/blk_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-01 15:29:30.000000 blk-utils-0.1.2/blk_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-10-01 15:29:30.000000 blk-utils-0.1.2/blk_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-10-01 15:29:30.000000 blk-utils-0.1.2/blk_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       53 2023-04-14 17:24:44.000000 blk-utils-0.1.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-10-01 15:29:31.267664 blk-utils-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1359 2023-10-01 15:29:17.000000 blk-utils-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-10-01 15:29:31.264665 blk-utils-0.1.2/tests/
--rw-rw-rw-   0        0        0        0 2023-04-12 13:18:07.000000 blk-utils-0.1.2/tests/__init__.py
--rw-rw-rw-   0        0        0      322 2023-04-14 16:44:44.000000 blk-utils-0.1.2/tests/utils_test.py
+drwxrwxrwx   0        0        0        0 2024-05-16 16:57:00.449557 blk_utils-0.1.3/
+-rw-rw-rw-   0        0        0     4073 2023-04-14 17:28:18.000000 blk_utils-0.1.3/.gitignore
+-rw-rw-rw-   0        0        0     1370 2024-05-16 16:57:00.448556 blk_utils-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      472 2023-04-14 17:36:30.000000 blk_utils-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 16:57:00.437250 blk_utils-0.1.3/blk_utils/
+-rw-rw-rw-   0        0        0      137 2023-11-13 22:11:07.000000 blk_utils-0.1.3/blk_utils/__init__.py
+-rw-rw-rw-   0        0        0     4226 2024-05-16 16:52:07.000000 blk_utils-0.1.3/blk_utils/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-16 16:57:00.447556 blk_utils-0.1.3/blk_utils.egg-info/
+-rw-rw-rw-   0        0        0     1370 2024-05-16 16:57:00.000000 blk_utils-0.1.3/blk_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2024-05-16 16:57:00.000000 blk_utils-0.1.3/blk_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 16:57:00.000000 blk_utils-0.1.3/blk_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-05-16 16:57:00.000000 blk_utils-0.1.3/blk_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-16 16:57:00.000000 blk_utils-0.1.3/blk_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       53 2023-04-14 17:24:44.000000 blk_utils-0.1.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 16:57:00.449557 blk_utils-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1461 2024-05-16 16:52:07.000000 blk_utils-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 16:57:00.446557 blk_utils-0.1.3/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-12 13:18:07.000000 blk_utils-0.1.3/tests/__init__.py
+-rw-rw-rw-   0        0        0      322 2023-04-14 16:44:44.000000 blk_utils-0.1.3/tests/utils_test.py
```

### Comparing `blk-utils-0.1.2/.gitignore` & `blk_utils-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `blk-utils-0.1.2/PKG-INFO` & `blk_utils-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: blk-utils
-Version: 0.1.2
+Version: 0.1.3
 Summary: Small Utility Library
 Home-page: https://blk-utils.readthedocs.io/
 Author: Brian Christopher
 Author-email: bcr@blackarbs.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
 Requires-Dist: hypothesis
 Requires-Dist: timeutils
 
 <H1>BLK UTILS</H1>
```

### Comparing `blk-utils-0.1.2/blk_utils/utils.py` & `blk_utils-0.1.3/blk_utils/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,134 +1,143 @@
-import pandas as pd
-from decimal import Decimal, ROUND_HALF_DOWN
-from pathlib import Path
-from timeutils import Stopwatch
-
-
-# =============================================================================
-# general utils
-
-
-def quantize_number(number, precision=2, rounding=ROUND_HALF_DOWN):
-    """Quantizes a number to a given precision and returns a float.
-
-    Args:
-      number: The number to quantize.
-      precision: The precision to quantize to.
-
-    Returns:
-      A float.
-    """
-    # Convert the input number to a Decimal object
-    try:
-        number_decimal = Decimal(str(number))
-    except Exception as e:
-        print(e)
-    # Set the precision to the desired number of decimal places
-    precision_decimal = Decimal("0." + "0" * precision)
-
-    # Quantize the number using ROUND_HALF_DOWN rounding mode
-    quantized_decimal = number_decimal.quantize(precision_decimal, rounding=rounding)
-
-    # Convert the quantized Decimal back to a float
-    quantized_float = float(quantized_decimal)
-
-    return quantized_float
-
-
-def timer(func):
-    """
-    this is a decorator that shows the execution time of the
-    function passed in human readable format
-
-    :param func: function
-    :return: function output
-    """
-
-    def wrap_func(*args, **kwargs):
-        sw = Stopwatch(start=True)
-        result = func(*args, **kwargs)
-        sw.stop()
-        print(f"Function {func.__name__!r} executed in {sw.elapsed.human_str()}")
-        return result
-
-    return wrap_func
-
-
-def create_output_path(filepath):
-    """
-    create output path
-
-    :param filepath: str or path object
-    :return: path
-    """
-    p = Path(filepath)
-    if p.is_dir():
-        print("directory exists...")
-    else:
-        p.mkdir(parents=True, exist_ok=False)
-        print("creating directory...")
-        print("directory created [complete]")
-    return p
-
-
-def get_relative_project_dir(project_repo_name=None, partial=True):
-    """
-    helper function to get top level project directory path using exact or
-    partial name matching.
-
-    :param project_repo_name: str
-    :param partial: bool, default=True
-    :return: path obj
-    """
-    current_working_directory = Path.cwd()
-    cwd_parts = current_working_directory.parts
-    if partial:
-        while project_repo_name not in cwd_parts[-1]:
-            current_working_directory = current_working_directory.parent
-            cwd_parts = current_working_directory.parts
-            if len(cwd_parts) == 1:
-                if project_repo_name not in cwd_parts[0]:
-                    raise ValueError(
-                        f"{project_repo_name} not found in directory tree!"
-                    )
-    else:
-        while cwd_parts[-1] != project_repo_name:
-            current_working_directory = current_working_directory.parent
-            cwd_parts = current_working_directory.parts
-            if len(cwd_parts) == 1:
-                if project_repo_name not in cwd_parts[0]:
-                    raise ValueError(
-                        f"{project_repo_name} not found in directory tree!"
-                    )
-    return current_working_directory
-
-
-def cprint(df, nrows=None):
-    """
-    custom print function to output series or dataframe information
-
-    :param df: pandas series or dataframe
-    :param nrows: int
-    :return: None
-    """
-    if not isinstance(df, (pd.DataFrame,)):
-        try:
-            df = df.to_frame()
-        except:
-            raise ValueError("object cannot be coerced to df")
-
-    if not nrows:
-        nrows = 5
-    print("-" * 79)
-    print("dataframe information")
-    print("-" * 79)
-    print(f"HEAD num rows: {nrows}")
-    print(df.head(nrows))
-    print("-" * 25)
-    print(f"TAIL num rows: {nrows}")
-    print(df.tail(nrows))
-    print("-" * 50)
-    print(df.info(verbose=True))
-    print("-" * 79)
-    print()
-    return
+import pandas as pd
+from decimal import Decimal, ROUND_HALF_DOWN
+from pathlib import Path
+from timeutils import Stopwatch
+
+
+# =============================================================================
+# general utils
+
+
+def quantize_number(number, precision=2, rounding=ROUND_HALF_DOWN):
+    """Quantizes a number to a given precision and returns a float.
+
+    Args:
+      number: The number to quantize.
+      precision: The precision to quantize to.
+
+    Returns:
+      A float.
+    """
+    # Convert the input number to a Decimal object
+    try:
+        number_decimal = Decimal(str(number))
+    except Exception as e:
+        print(e)
+    # Set the precision to the desired number of decimal places
+    precision_decimal = Decimal("0." + "0" * precision)
+
+    # Quantize the number using ROUND_HALF_DOWN rounding mode
+    quantized_decimal = number_decimal.quantize(precision_decimal, rounding=rounding)
+
+    # Convert the quantized Decimal back to a float
+    quantized_float = float(quantized_decimal)
+
+    return quantized_float
+
+
+def timer(human_str=False, significant_digits=None):
+    """
+    this is a decorator that shows the execution time of the
+    function passed in human readable format if desired
+
+    :param human_str: bool
+    :param significant_digits: int, pass to human_str of timeutils package
+    :return: function output
+    """
+
+    def Inner(func):
+        def wrap_func(*args, **kwargs):
+            sw = Stopwatch(start=True)
+            result = func(*args, **kwargs)
+            sw.stop()
+            if human_str:
+                print(
+                    f"Function {func.__name__!r} executed in {sw.elapsed.human_str(significant_digits=significant_digits)}"
+                )
+            else:
+                print(f"Function {func.__name__!r} executed in {sw.elapsed}")
+            return result
+
+        return wrap_func
+
+    return Inner
+
+
+def create_output_path(filepath):
+    """
+    create output path
+
+    :param filepath: str or path object
+    :return: path
+    """
+    p = Path(filepath)
+    if p.is_dir():
+        print("directory exists...")
+    else:
+        p.mkdir(parents=True, exist_ok=False)
+        print("creating directory...")
+        print("directory created [complete]")
+    return p
+
+
+def get_relative_project_dir(project_repo_name=None, partial=True):
+    """
+    helper function to get top level project directory path using exact or
+    partial name matching.
+
+    :param project_repo_name: str
+    :param partial: bool, default=True
+    :return: path obj
+    """
+    current_working_directory = Path.cwd()
+    cwd_parts = current_working_directory.parts
+    if partial:
+        while project_repo_name not in cwd_parts[-1]:
+            current_working_directory = current_working_directory.parent
+            cwd_parts = current_working_directory.parts
+            if len(cwd_parts) == 1:
+                if project_repo_name not in cwd_parts[0]:
+                    raise ValueError(
+                        f"{project_repo_name} not found in directory tree!"
+                    )
+    else:
+        while cwd_parts[-1] != project_repo_name:
+            current_working_directory = current_working_directory.parent
+            cwd_parts = current_working_directory.parts
+            if len(cwd_parts) == 1:
+                if project_repo_name not in cwd_parts[0]:
+                    raise ValueError(
+                        f"{project_repo_name} not found in directory tree!"
+                    )
+    return current_working_directory
+
+
+def cprint(df, nrows=None):
+    """
+    custom print function to output series or dataframe information
+
+    :param df: pandas series or dataframe
+    :param nrows: int
+    :return: None
+    """
+    if not isinstance(df, (pd.DataFrame,)):
+        try:
+            df = df.to_frame()
+        except:
+            raise ValueError("object cannot be coerced to df")
+
+    if not nrows:
+        nrows = 5
+    print("-" * 79)
+    print("dataframe information")
+    print("-" * 79)
+    print(f"HEAD num rows: {nrows}")
+    print(df.head(nrows))
+    print("-" * 25)
+    print(f"TAIL num rows: {nrows}")
+    print(df.tail(nrows))
+    print("-" * 50)
+    print(df.info(verbose=True))
+    print("-" * 79)
+    print()
+    return
```

### Comparing `blk-utils-0.1.2/blk_utils.egg-info/PKG-INFO` & `blk_utils-0.1.3/blk_utils.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: blk-utils
-Version: 0.1.2
+Version: 0.1.3
 Summary: Small Utility Library
 Home-page: https://blk-utils.readthedocs.io/
 Author: Brian Christopher
 Author-email: bcr@blackarbs.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
 Requires-Dist: hypothesis
 Requires-Dist: timeutils
 
 <H1>BLK UTILS</H1>
```

### Comparing `blk-utils-0.1.2/setup.py` & `blk_utils-0.1.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="blk-utils",
-    version="0.1.2",
+    version="0.1.3",
     description="Small Utility Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://blk-utils.readthedocs.io/",
     author="Brian Christopher",
     author_email="bcr@blackarbs.com",
     license="MIT",
@@ -28,13 +28,15 @@
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Operating System :: OS Independent",
     ],
     packages=["blk_utils"],
     include_package_data=True,
     install_requires=["pandas", "hypothesis", "timeutils"],
 )
```

