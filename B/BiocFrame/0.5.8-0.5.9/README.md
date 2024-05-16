# Comparing `tmp/BiocFrame-0.5.8.tar.gz` & `tmp/BiocFrame-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BiocFrame-0.5.8.tar", last modified: Tue Jan 23 22:08:28 2024, max compression
+gzip compressed data, was "BiocFrame-0.5.9.tar", last modified: Fri Jan 26 18:46:56 2024, max compression
```

## Comparing `BiocFrame-0.5.8.tar` & `BiocFrame-0.5.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 22:08:28.031408 BiocFrame-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-01-23 22:07:29.000000 BiocFrame-0.5.8/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 22:08:28.019408 BiocFrame-0.5.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 22:08:28.023408 BiocFrame-0.5.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-01-23 22:07:29.000000 BiocFrame-0.5.8/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-01-23 22:07:29.000000 BiocFrame-0.5.8/.github/workflows/pypi-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-01-23 22:07:29.000000 BiocFrame-0.5.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-01-23 22:07:29.000000 BiocFrame-0.5.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-01-23 22:07:29.000000 BiocFrame-0.5.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-01-23 22:07:29.000000 BiocFrame-0.5.8/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-01-23 22:07:29.000000 BiocFrame-0.5.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    13503 2024-01-23 22:07:29.000000 BiocFrame-0.5.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-01-23 22:07:29.000000 BiocFrame-0.5.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12353 2024-01-23 22:08:28.031408 BiocFrame-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-01-23 22:07:29.000000 BiocFrame-0.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 22:08:28.023408 BiocFrame-0.5.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-01-23 22:07:29.000000 BiocFrame-0.5.8/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 22:08:28.023408 BiocFrame-0.5.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-23 22:07:29.000000 BiocFrame-0.5.8/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-01-23 22:07:29.000000 BiocFrame-0.5.8/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-01-23 22:07:29.000000 BiocFrame-0.5.8/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)    10400 2024-01-23 22:07:29.000000 BiocFrame-0.5.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-01-23 22:07:29.000000 BiocFrame-0.5.8/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-01-23 22:07:29.000000 BiocFrame-0.5.8/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-01-23 22:07:29.000000 BiocFrame-0.5.8/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-01-23 22:07:29.000000 BiocFrame-0.5.8/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-01-23 22:07:29.000000 BiocFrame-0.5.8/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-01-23 22:07:29.000000 BiocFrame-0.5.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-01-23 22:08:28.031408 BiocFrame-0.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-01-23 22:07:29.000000 BiocFrame-0.5.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 22:08:28.019408 BiocFrame-0.5.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 22:08:28.027408 BiocFrame-0.5.8/src/BiocFrame.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12353 2024-01-23 22:08:27.000000 BiocFrame-0.5.8/src/BiocFrame.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-01-23 22:08:28.000000 BiocFrame-0.5.8/src/BiocFrame.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-23 22:08:27.000000 BiocFrame-0.5.8/src/BiocFrame.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-23 22:08:27.000000 BiocFrame-0.5.8/src/BiocFrame.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-01-23 22:08:27.000000 BiocFrame-0.5.8/src/BiocFrame.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-23 22:08:27.000000 BiocFrame-0.5.8/src/BiocFrame.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 22:08:28.027408 BiocFrame-0.5.8/src/biocframe/
--rw-r--r--   0 runner    (1001) docker     (127)    56279 2024-01-23 22:07:29.000000 BiocFrame-0.5.8/src/biocframe/BiocFrame.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-01-23 22:07:29.000000 BiocFrame-0.5.8/src/biocframe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 22:08:28.027408 BiocFrame-0.5.8/src/biocframe/io/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-01-23 22:07:29.000000 BiocFrame-0.5.8/src/biocframe/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-01-23 22:07:29.000000 BiocFrame-0.5.8/src/biocframe/io/from_pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 22:08:28.027408 BiocFrame-0.5.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-01-23 22:07:29.000000 BiocFrame-0.5.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-01-23 22:07:29.000000 BiocFrame-0.5.8/tests/test_combine.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-01-23 22:07:29.000000 BiocFrame-0.5.8/tests/test_copy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-01-23 22:07:29.000000 BiocFrame-0.5.8/tests/test_initialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-01-23 22:07:29.000000 BiocFrame-0.5.8/tests/test_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)    17953 2024-01-23 22:07:29.000000 BiocFrame-0.5.8/tests/test_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-01-23 22:07:29.000000 BiocFrame-0.5.8/tests/test_readme.py
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-01-23 22:07:29.000000 BiocFrame-0.5.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 18:46:56.717800 BiocFrame-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-01-26 18:45:55.000000 BiocFrame-0.5.9/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 18:46:56.705800 BiocFrame-0.5.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 18:46:56.709800 BiocFrame-0.5.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-01-26 18:45:55.000000 BiocFrame-0.5.9/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-01-26 18:45:55.000000 BiocFrame-0.5.9/.github/workflows/pypi-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-01-26 18:45:55.000000 BiocFrame-0.5.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-01-26 18:45:55.000000 BiocFrame-0.5.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-01-26 18:45:55.000000 BiocFrame-0.5.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-01-26 18:45:55.000000 BiocFrame-0.5.9/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-01-26 18:45:55.000000 BiocFrame-0.5.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13503 2024-01-26 18:45:55.000000 BiocFrame-0.5.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-01-26 18:45:55.000000 BiocFrame-0.5.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12353 2024-01-26 18:46:56.717800 BiocFrame-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-01-26 18:45:55.000000 BiocFrame-0.5.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 18:46:56.713800 BiocFrame-0.5.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-01-26 18:45:55.000000 BiocFrame-0.5.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 18:46:56.713800 BiocFrame-0.5.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-26 18:45:55.000000 BiocFrame-0.5.9/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-01-26 18:45:55.000000 BiocFrame-0.5.9/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-01-26 18:45:55.000000 BiocFrame-0.5.9/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10400 2024-01-26 18:45:55.000000 BiocFrame-0.5.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-01-26 18:45:55.000000 BiocFrame-0.5.9/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-01-26 18:45:55.000000 BiocFrame-0.5.9/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-01-26 18:45:55.000000 BiocFrame-0.5.9/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-01-26 18:45:55.000000 BiocFrame-0.5.9/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-01-26 18:45:55.000000 BiocFrame-0.5.9/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-01-26 18:45:55.000000 BiocFrame-0.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-01-26 18:46:56.717800 BiocFrame-0.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-01-26 18:45:55.000000 BiocFrame-0.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 18:46:56.705800 BiocFrame-0.5.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 18:46:56.717800 BiocFrame-0.5.9/src/BiocFrame.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12353 2024-01-26 18:46:56.000000 BiocFrame-0.5.9/src/BiocFrame.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-01-26 18:46:56.000000 BiocFrame-0.5.9/src/BiocFrame.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-26 18:46:56.000000 BiocFrame-0.5.9/src/BiocFrame.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-26 18:46:56.000000 BiocFrame-0.5.9/src/BiocFrame.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-01-26 18:46:56.000000 BiocFrame-0.5.9/src/BiocFrame.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-26 18:46:56.000000 BiocFrame-0.5.9/src/BiocFrame.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 18:46:56.713800 BiocFrame-0.5.9/src/biocframe/
+-rw-r--r--   0 runner    (1001) docker     (127)    56659 2024-01-26 18:45:55.000000 BiocFrame-0.5.9/src/biocframe/BiocFrame.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-01-26 18:45:55.000000 BiocFrame-0.5.9/src/biocframe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 18:46:56.713800 BiocFrame-0.5.9/src/biocframe/io/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-01-26 18:45:55.000000 BiocFrame-0.5.9/src/biocframe/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-01-26 18:45:55.000000 BiocFrame-0.5.9/src/biocframe/io/from_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 18:46:56.717800 BiocFrame-0.5.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-01-26 18:45:55.000000 BiocFrame-0.5.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-01-26 18:45:55.000000 BiocFrame-0.5.9/tests/test_combine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-01-26 18:45:55.000000 BiocFrame-0.5.9/tests/test_copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-01-26 18:45:55.000000 BiocFrame-0.5.9/tests/test_initialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-01-26 18:45:55.000000 BiocFrame-0.5.9/tests/test_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17953 2024-01-26 18:45:55.000000 BiocFrame-0.5.9/tests/test_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-01-26 18:45:55.000000 BiocFrame-0.5.9/tests/test_readme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-01-26 18:45:55.000000 BiocFrame-0.5.9/tox.ini
```

### Comparing `BiocFrame-0.5.8/.coveragerc` & `BiocFrame-0.5.9/.coveragerc`

 * *Files identical despite different names*

### Comparing `BiocFrame-0.5.8/.github/workflows/pypi-publish.yml` & `BiocFrame-0.5.9/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `BiocFrame-0.5.8/.github/workflows/pypi-test.yml` & `BiocFrame-0.5.9/.github/workflows/pypi-test.yml`

 * *Files identical despite different names*

### Comparing `BiocFrame-0.5.8/.gitignore` & `BiocFrame-0.5.9/.gitignore`

 * *Files identical despite different names*

### Comparing `BiocFrame-0.5.8/.pre-commit-config.yaml` & `BiocFrame-0.5.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `BiocFrame-0.5.8/CHANGELOG.md` & `BiocFrame-0.5.9/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `BiocFrame-0.5.8/CONTRIBUTING.md` & `BiocFrame-0.5.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `BiocFrame-0.5.8/LICENSE.txt` & `BiocFrame-0.5.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `BiocFrame-0.5.8/PKG-INFO` & `BiocFrame-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BiocFrame
-Version: 0.5.8
+Version: 0.5.9
 Summary: Flexible dataframe representation to support nested structures.
 Home-page: https://github.com/BiocPy/biocframe
 Author: Jayaram Kancherla
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/BiocPy/biocframe
 Project-URL: Source, https://github.com/BiocPy/biocframe
```

### Comparing `BiocFrame-0.5.8/README.md` & `BiocFrame-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `BiocFrame-0.5.8/docs/Makefile` & `BiocFrame-0.5.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `BiocFrame-0.5.8/docs/conf.py` & `BiocFrame-0.5.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `BiocFrame-0.5.8/docs/index.md` & `BiocFrame-0.5.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `BiocFrame-0.5.8/pyproject.toml` & `BiocFrame-0.5.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `BiocFrame-0.5.8/setup.cfg` & `BiocFrame-0.5.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `BiocFrame-0.5.8/setup.py` & `BiocFrame-0.5.9/setup.py`

 * *Files identical despite different names*

### Comparing `BiocFrame-0.5.8/src/BiocFrame.egg-info/PKG-INFO` & `BiocFrame-0.5.9/src/BiocFrame.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BiocFrame
-Version: 0.5.8
+Version: 0.5.9
 Summary: Flexible dataframe representation to support nested structures.
 Home-page: https://github.com/BiocPy/biocframe
 Author: Jayaram Kancherla
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/BiocPy/biocframe
 Project-URL: Source, https://github.com/BiocPy/biocframe
```

### Comparing `BiocFrame-0.5.8/src/BiocFrame.egg-info/SOURCES.txt` & `BiocFrame-0.5.9/src/BiocFrame.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BiocFrame-0.5.8/src/biocframe/BiocFrame.py` & `BiocFrame-0.5.9/src/biocframe/BiocFrame.py`

 * *Files 0% similar despite different names*

```diff
@@ -616,18 +616,30 @@
 
                 Alternatively, the integer index of the column of interest.
 
         Returns:
             The contents of the specified column.
         """
         if isinstance(column, int):
-            column = self._column_names[column]
-        elif not isinstance(column, str):
-            raise TypeError("`column` must be either an integer index or column name.")
-        return self._data[column]
+            if column < 0:
+                raise IndexError("Index cannot be negative.")
+
+            if column > len(self._column_names):
+                raise IndexError("Index greater than the number of columns.")
+
+            return self._data[self._column_names[column]]
+        elif isinstance(column, str):
+            if column not in self._column_names:
+                raise AttributeError(f"Column: {column} does not exist.")
+
+            return self._data[column]
+
+        raise TypeError(
+            f"'column' must be a string or integer, provided '{type(column)}'."
+        )
 
     def column(self, column: Union[str, int]) -> Any:
         """Alias for :py:meth:`~get_column`, provided for back-compatibility only."""
         warn(
             "Method 'column' is deprecated, use 'get_column' instead",
             DeprecationWarning,
         )
```

### Comparing `BiocFrame-0.5.8/src/biocframe/__init__.py` & `BiocFrame-0.5.9/src/biocframe/__init__.py`

 * *Files identical despite different names*

### Comparing `BiocFrame-0.5.8/tests/test_combine.py` & `BiocFrame-0.5.9/tests/test_combine.py`

 * *Files identical despite different names*

### Comparing `BiocFrame-0.5.8/tests/test_copy.py` & `BiocFrame-0.5.9/tests/test_copy.py`

 * *Files identical despite different names*

### Comparing `BiocFrame-0.5.8/tests/test_initialize.py` & `BiocFrame-0.5.9/tests/test_initialize.py`

 * *Files identical despite different names*

### Comparing `BiocFrame-0.5.8/tests/test_merge.py` & `BiocFrame-0.5.9/tests/test_merge.py`

 * *Files identical despite different names*

### Comparing `BiocFrame-0.5.8/tests/test_methods.py` & `BiocFrame-0.5.9/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `BiocFrame-0.5.8/tests/test_readme.py` & `BiocFrame-0.5.9/tests/test_readme.py`

 * *Files identical despite different names*

### Comparing `BiocFrame-0.5.8/tox.ini` & `BiocFrame-0.5.9/tox.ini`

 * *Files identical despite different names*

