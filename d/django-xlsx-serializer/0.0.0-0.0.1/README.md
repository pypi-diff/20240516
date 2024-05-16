# Comparing `tmp/django_xlsx_serializer-0.0.0.tar.gz` & `tmp/django_xlsx_serializer-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_xlsx_serializer-0.0.0.tar", last modified: Thu May 16 12:33:29 2024, max compression
+gzip compressed data, was "django_xlsx_serializer-0.0.1.tar", last modified: Thu May 16 12:44:20 2024, max compression
```

## Comparing `django_xlsx_serializer-0.0.0.tar` & `django_xlsx_serializer-0.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:33:29.261730 django_xlsx_serializer-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-16 12:33:18.000000 django_xlsx_serializer-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-16 12:33:29.261730 django_xlsx_serializer-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-16 12:33:18.000000 django_xlsx_serializer-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-16 12:33:18.000000 django_xlsx_serializer-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 12:33:29.261730 django_xlsx_serializer-0.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:33:29.257730 django_xlsx_serializer-0.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:33:29.261730 django_xlsx_serializer-0.0.0/src/django_xlsx_serializer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-16 12:33:29.000000 django_xlsx_serializer-0.0.0/src/django_xlsx_serializer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-16 12:33:29.000000 django_xlsx_serializer-0.0.0/src/django_xlsx_serializer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 12:33:29.000000 django_xlsx_serializer-0.0.0/src/django_xlsx_serializer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-16 12:33:29.000000 django_xlsx_serializer-0.0.0/src/django_xlsx_serializer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-16 12:33:29.000000 django_xlsx_serializer-0.0.0/src/django_xlsx_serializer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:33:29.261730 django_xlsx_serializer-0.0.0/src/xlsx_serializer/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-16 12:33:18.000000 django_xlsx_serializer-0.0.0/src/xlsx_serializer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:44:20.871017 django_xlsx_serializer-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-16 12:44:04.000000 django_xlsx_serializer-0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-16 12:44:20.871017 django_xlsx_serializer-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-16 12:44:04.000000 django_xlsx_serializer-0.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-16 12:44:04.000000 django_xlsx_serializer-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 12:44:20.871017 django_xlsx_serializer-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:44:20.867017 django_xlsx_serializer-0.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:44:20.871017 django_xlsx_serializer-0.0.1/src/django_xlsx_serializer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-16 12:44:20.000000 django_xlsx_serializer-0.0.1/src/django_xlsx_serializer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-16 12:44:20.000000 django_xlsx_serializer-0.0.1/src/django_xlsx_serializer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 12:44:20.000000 django_xlsx_serializer-0.0.1/src/django_xlsx_serializer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-16 12:44:20.000000 django_xlsx_serializer-0.0.1/src/django_xlsx_serializer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-16 12:44:20.000000 django_xlsx_serializer-0.0.1/src/django_xlsx_serializer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:44:20.871017 django_xlsx_serializer-0.0.1/src/xlsx_serializer/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-16 12:44:04.000000 django_xlsx_serializer-0.0.1/src/xlsx_serializer/__init__.py
```

### Comparing `django_xlsx_serializer-0.0.0/LICENSE` & `django_xlsx_serializer-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_xlsx_serializer-0.0.0/PKG-INFO` & `django_xlsx_serializer-0.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: django-xlsx-serializer
-Version: 0.0.0
+Version: 0.0.1
 Summary: Load/dump Django models from/to Excel 2003+ workbooks
 Author-email: Kamil Paduszyński <92403542+paduszyk@users.noreply.github.com>
-License: MIT License
 Project-URL: Repository, https://github.com/paduszyk/django-xlsx-serializer
 Project-URL: Documentation, https://github.com/paduszyk/django-xlsx-serializer#readme
 Project-URL: Issue tracker, https://github.com/paduszyk/django-xlsx-serializer/issues
 Keywords: django,django-application,excel,excel-export,excel-import,openpyxl,xlsx
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -42,8 +41,8 @@
 
 Released under the [MIT license][license].
 
 [conventional-commits]: https://www.conventionalcommits.org/en/v1.0.0/
 [license]: https://github.com/paduszyk/django-xlsx-serializer/blob/main/LICENSE
 [paduszyk]: https://github.com/paduszyk
 [prettier]: https://prettier.io
-[pypi]: https://pypi.org/project/python-gitmojis/
+[pypi]: https://pypi.org/project/django-xlsx-serializer/
```

### Comparing `django_xlsx_serializer-0.0.0/README.md` & `django_xlsx_serializer-0.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 
 Released under the [MIT license][license].
 
 [conventional-commits]: https://www.conventionalcommits.org/en/v1.0.0/
 [license]: https://github.com/paduszyk/django-xlsx-serializer/blob/main/LICENSE
 [paduszyk]: https://github.com/paduszyk
 [prettier]: https://prettier.io
-[pypi]: https://pypi.org/project/python-gitmojis/
+[pypi]: https://pypi.org/project/django-xlsx-serializer/
```

### Comparing `django_xlsx_serializer-0.0.0/pyproject.toml` & `django_xlsx_serializer-0.0.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 dependencies = []
 requires-python = ">= 3.9"
 authors = [
   { name = "Kamil Paduszyński", email = "92403542+paduszyk@users.noreply.github.com" },
 ]
 description = "Load/dump Django models from/to Excel 2003+ workbooks"
 readme = "README.md"
-license = { text = "MIT License" }
 keywords = [
   "django",
   "django-application",
   "excel",
   "excel-export",
   "excel-import",
   "openpyxl",
```

### Comparing `django_xlsx_serializer-0.0.0/src/django_xlsx_serializer.egg-info/PKG-INFO` & `django_xlsx_serializer-0.0.1/src/django_xlsx_serializer.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: django-xlsx-serializer
-Version: 0.0.0
+Version: 0.0.1
 Summary: Load/dump Django models from/to Excel 2003+ workbooks
 Author-email: Kamil Paduszyński <92403542+paduszyk@users.noreply.github.com>
-License: MIT License
 Project-URL: Repository, https://github.com/paduszyk/django-xlsx-serializer
 Project-URL: Documentation, https://github.com/paduszyk/django-xlsx-serializer#readme
 Project-URL: Issue tracker, https://github.com/paduszyk/django-xlsx-serializer/issues
 Keywords: django,django-application,excel,excel-export,excel-import,openpyxl,xlsx
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -42,8 +41,8 @@
 
 Released under the [MIT license][license].
 
 [conventional-commits]: https://www.conventionalcommits.org/en/v1.0.0/
 [license]: https://github.com/paduszyk/django-xlsx-serializer/blob/main/LICENSE
 [paduszyk]: https://github.com/paduszyk
 [prettier]: https://prettier.io
-[pypi]: https://pypi.org/project/python-gitmojis/
+[pypi]: https://pypi.org/project/django-xlsx-serializer/
```

