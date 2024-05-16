# Comparing `tmp/dash_pydantic_form-0.1.1.tar.gz` & `tmp/dash_pydantic_form-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_pydantic_form-0.1.1.tar", last modified: Mon May 13 11:49:33 2024, max compression
+gzip compressed data, was "dash_pydantic_form-0.1.2.tar", last modified: Thu May 16 10:53:08 2024, max compression
```

## Comparing `dash_pydantic_form-0.1.1.tar` & `dash_pydantic_form-0.1.2.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxr-xr-x   0 renaud    (1000) renaud    (1000)        0 2024-05-13 11:49:33.194478 dash_pydantic_form-0.1.1/
--rw-r--r--   0 renaud    (1000) renaud    (1000)     3231 2024-04-25 01:57:38.000000 dash_pydantic_form-0.1.1/.gitignore
--rw-r--r--   0 renaud    (1000) renaud    (1000)      406 2024-05-11 12:42:14.000000 dash_pydantic_form-0.1.1/.pre-commit-config.yaml
-drwxr-xr-x   0 renaud    (1000) renaud    (1000)        0 2024-05-13 11:49:33.194478 dash_pydantic_form-0.1.1/.vscode/
--rw-r--r--   0 renaud    (1000) renaud    (1000)      834 2024-05-12 04:37:36.000000 dash_pydantic_form-0.1.1/.vscode/launch.json
--rw-r--r--   0 renaud    (1000) renaud    (1000)      313 2024-05-13 11:40:57.000000 dash_pydantic_form-0.1.1/CHANGELOG.md
--rw-r--r--   0 renaud    (1000) renaud    (1000)     7104 2024-05-13 11:49:33.194478 dash_pydantic_form-0.1.1/PKG-INFO
--rw-r--r--   0 renaud    (1000) renaud    (1000)     6401 2024-05-13 11:34:53.000000 dash_pydantic_form-0.1.1/README.md
-drwxr-xr-x   0 renaud    (1000) renaud    (1000)        0 2024-05-13 11:49:33.194478 dash_pydantic_form-0.1.1/dash_pydantic_form/
--rw-r--r--   0 renaud    (1000) renaud    (1000)      680 2024-05-12 00:26:29.000000 dash_pydantic_form-0.1.1/dash_pydantic_form/__init__.py
-drwxr-xr-x   0 renaud    (1000) renaud    (1000)        0 2024-05-13 11:49:33.194478 dash_pydantic_form-0.1.1/dash_pydantic_form/fields/
--rw-r--r--   0 renaud    (1000) renaud    (1000)     1496 2024-05-12 05:06:05.000000 dash_pydantic_form-0.1.1/dash_pydantic_form/fields/__init__.py
--rw-r--r--   0 renaud    (1000) renaud    (1000)     1416 2024-05-11 12:46:28.000000 dash_pydantic_form-0.1.1/dash_pydantic_form/fields/all_fields.py
--rw-r--r--   0 renaud    (1000) renaud    (1000)    19394 2024-05-12 05:54:58.000000 dash_pydantic_form-0.1.1/dash_pydantic_form/fields/base_fields.py
--rw-r--r--   0 renaud    (1000) renaud    (1000)    18563 2024-05-12 06:44:14.000000 dash_pydantic_form-0.1.1/dash_pydantic_form/fields/editabletable_field.py
--rw-r--r--   0 renaud    (1000) renaud    (1000)    28331 2024-05-12 06:04:25.000000 dash_pydantic_form-0.1.1/dash_pydantic_form/fields/model_fields.py
--rw-r--r--   0 renaud    (1000) renaud    (1000)      913 2024-05-11 12:52:58.000000 dash_pydantic_form-0.1.1/dash_pydantic_form/form_section.py
--rw-r--r--   0 renaud    (1000) renaud    (1000)      944 2024-05-11 12:54:05.000000 dash_pydantic_form-0.1.1/dash_pydantic_form/ids.py
--rw-r--r--   0 renaud    (1000) renaud    (1000)    12561 2024-05-12 06:55:01.000000 dash_pydantic_form-0.1.1/dash_pydantic_form/model_form.py
--rw-r--r--   0 renaud    (1000) renaud    (1000)     8185 2024-05-12 06:25:19.000000 dash_pydantic_form-0.1.1/dash_pydantic_form/pydantic_form_scripts.js
--rw-r--r--   0 renaud    (1000) renaud    (1000)     1768 2024-05-11 12:58:15.000000 dash_pydantic_form-0.1.1/dash_pydantic_form/pydantic_form_styles.css
--rw-r--r--   0 renaud    (1000) renaud    (1000)     4506 2024-05-12 00:24:12.000000 dash_pydantic_form-0.1.1/dash_pydantic_form/utils.py
-drwxr-xr-x   0 renaud    (1000) renaud    (1000)        0 2024-05-13 11:49:33.194478 dash_pydantic_form-0.1.1/dash_pydantic_form.egg-info/
--rw-r--r--   0 renaud    (1000) renaud    (1000)     7104 2024-05-13 11:49:33.000000 dash_pydantic_form-0.1.1/dash_pydantic_form.egg-info/PKG-INFO
--rw-r--r--   0 renaud    (1000) renaud    (1000)      952 2024-05-13 11:49:33.000000 dash_pydantic_form-0.1.1/dash_pydantic_form.egg-info/SOURCES.txt
--rw-r--r--   0 renaud    (1000) renaud    (1000)        1 2024-05-13 11:49:33.000000 dash_pydantic_form-0.1.1/dash_pydantic_form.egg-info/dependency_links.txt
--rw-r--r--   0 renaud    (1000) renaud    (1000)      116 2024-05-13 11:49:33.000000 dash_pydantic_form-0.1.1/dash_pydantic_form.egg-info/requires.txt
--rw-r--r--   0 renaud    (1000) renaud    (1000)       36 2024-05-13 11:49:33.000000 dash_pydantic_form-0.1.1/dash_pydantic_form.egg-info/top_level.txt
-drwxr-xr-x   0 renaud    (1000) renaud    (1000)        0 2024-05-13 11:49:33.194478 dash_pydantic_form-0.1.1/docs/
--rw-r--r--   0 renaud    (1000) renaud    (1000)       87 2024-05-12 09:51:29.000000 dash_pydantic_form-0.1.1/docs/_config.yml
--rw-r--r--   0 renaud    (1000) renaud    (1000)       21 2024-05-12 09:47:47.000000 dash_pydantic_form-0.1.1/docs/index.md
-drwxr-xr-x   0 renaud    (1000) renaud    (1000)        0 2024-05-13 11:49:33.194478 dash_pydantic_form-0.1.1/images/
--rwxr-xr-x   0 renaud    (1000) renaud    (1000)    47789 2024-05-13 11:27:16.000000 dash_pydantic_form-0.1.1/images/conditionnally-visible-field.gif
--rwxr-xr-x   0 renaud    (1000) renaud    (1000)    15290 2024-05-13 11:17:07.000000 dash_pydantic_form-0.1.1/images/editable-table.png
--rwxr-xr-x   0 renaud    (1000) renaud    (1000)     4506 2024-05-13 11:00:42.000000 dash_pydantic_form-0.1.1/images/form-sections.png
--rwxr-xr-x   0 renaud    (1000) renaud    (1000)    12406 2024-05-13 11:12:08.000000 dash_pydantic_form-0.1.1/images/model-list.png
--rwxr-xr-x   0 renaud    (1000) renaud    (1000)     8028 2024-05-13 11:00:37.000000 dash_pydantic_form-0.1.1/images/nested-model.png
--rwxr-xr-x   0 renaud    (1000) renaud    (1000)    16764 2024-05-13 10:21:46.000000 dash_pydantic_form-0.1.1/images/simple-form.png
--rw-r--r--   0 renaud    (1000) renaud    (1000)     1186 2024-05-13 11:44:44.000000 dash_pydantic_form-0.1.1/pyproject.toml
--rw-r--r--   0 renaud    (1000) renaud    (1000)       38 2024-05-13 11:49:33.194478 dash_pydantic_form-0.1.1/setup.cfg
--rw-r--r--   0 renaud    (1000) renaud    (1000)     6243 2024-05-13 11:37:42.000000 dash_pydantic_form-0.1.1/usage.py
+drwxr-xr-x   0 renaud    (1000) renaud    (1000)        0 2024-05-16 10:53:08.824334 dash_pydantic_form-0.1.2/
+-rw-r--r--   0 renaud    (1000) renaud    (1000)     3231 2024-04-25 01:57:38.000000 dash_pydantic_form-0.1.2/.gitignore
+-rw-r--r--   0 renaud    (1000) renaud    (1000)      406 2024-05-11 12:42:14.000000 dash_pydantic_form-0.1.2/.pre-commit-config.yaml
+drwxr-xr-x   0 renaud    (1000) renaud    (1000)        0 2024-05-16 10:53:08.804334 dash_pydantic_form-0.1.2/.vscode/
+-rw-r--r--   0 renaud    (1000) renaud    (1000)      834 2024-05-12 04:37:36.000000 dash_pydantic_form-0.1.2/.vscode/launch.json
+-rw-r--r--   0 renaud    (1000) renaud    (1000)      454 2024-05-16 10:52:16.000000 dash_pydantic_form-0.1.2/CHANGELOG.md
+-rw-r--r--   0 renaud    (1000) renaud    (1000)     7487 2024-05-16 10:53:08.824334 dash_pydantic_form-0.1.2/PKG-INFO
+-rw-r--r--   0 renaud    (1000) renaud    (1000)     6784 2024-05-13 22:03:05.000000 dash_pydantic_form-0.1.2/README.md
+drwxr-xr-x   0 renaud    (1000) renaud    (1000)        0 2024-05-16 10:53:08.804334 dash_pydantic_form-0.1.2/dash_pydantic_form/
+-rw-r--r--   0 renaud    (1000) renaud    (1000)      749 2024-05-14 12:37:15.000000 dash_pydantic_form-0.1.2/dash_pydantic_form/__init__.py
+drwxr-xr-x   0 renaud    (1000) renaud    (1000)        0 2024-05-16 10:53:08.814334 dash_pydantic_form-0.1.2/dash_pydantic_form/fields/
+-rw-r--r--   0 renaud    (1000) renaud    (1000)     1972 2024-05-16 10:50:49.000000 dash_pydantic_form-0.1.2/dash_pydantic_form/fields/__init__.py
+-rw-r--r--   0 renaud    (1000) renaud    (1000)     1399 2024-05-16 10:50:49.000000 dash_pydantic_form-0.1.2/dash_pydantic_form/fields/all_fields.py
+-rw-r--r--   0 renaud    (1000) renaud    (1000)    21730 2024-05-14 12:37:15.000000 dash_pydantic_form-0.1.2/dash_pydantic_form/fields/base_fields.py
+-rw-r--r--   0 renaud    (1000) renaud    (1000)    18943 2024-05-14 13:01:55.000000 dash_pydantic_form-0.1.2/dash_pydantic_form/fields/editabletable_field.py
+-rw-r--r--   0 renaud    (1000) renaud    (1000)     1994 2024-05-14 12:37:15.000000 dash_pydantic_form-0.1.2/dash_pydantic_form/fields/markdown_field.py
+-rw-r--r--   0 renaud    (1000) renaud    (1000)     8218 2024-05-16 10:50:49.000000 dash_pydantic_form-0.1.2/dash_pydantic_form/fields/model_field.py
+-rw-r--r--   0 renaud    (1000) renaud    (1000)    21436 2024-05-14 13:16:15.000000 dash_pydantic_form-0.1.2/dash_pydantic_form/fields/model_list_field.py
+-rw-r--r--   0 renaud    (1000) renaud    (1000)     2145 2024-05-14 12:37:15.000000 dash_pydantic_form-0.1.2/dash_pydantic_form/form_section.py
+-rw-r--r--   0 renaud    (1000) renaud    (1000)      944 2024-05-11 12:54:05.000000 dash_pydantic_form-0.1.2/dash_pydantic_form/ids.py
+-rw-r--r--   0 renaud    (1000) renaud    (1000)    13585 2024-05-16 10:50:49.000000 dash_pydantic_form-0.1.2/dash_pydantic_form/model_form.py
+-rw-r--r--   0 renaud    (1000) renaud    (1000)     8201 2024-05-14 12:37:15.000000 dash_pydantic_form-0.1.2/dash_pydantic_form/pydantic_form_scripts.js
+-rw-r--r--   0 renaud    (1000) renaud    (1000)     2102 2024-05-14 12:37:15.000000 dash_pydantic_form-0.1.2/dash_pydantic_form/pydantic_form_styles.css
+-rw-r--r--   0 renaud    (1000) renaud    (1000)     4834 2024-05-16 10:50:49.000000 dash_pydantic_form-0.1.2/dash_pydantic_form/utils.py
+drwxr-xr-x   0 renaud    (1000) renaud    (1000)        0 2024-05-16 10:53:08.824334 dash_pydantic_form-0.1.2/dash_pydantic_form.egg-info/
+-rw-r--r--   0 renaud    (1000) renaud    (1000)     7487 2024-05-16 10:53:08.000000 dash_pydantic_form-0.1.2/dash_pydantic_form.egg-info/PKG-INFO
+-rw-r--r--   0 renaud    (1000) renaud    (1000)     1041 2024-05-16 10:53:08.000000 dash_pydantic_form-0.1.2/dash_pydantic_form.egg-info/SOURCES.txt
+-rw-r--r--   0 renaud    (1000) renaud    (1000)        1 2024-05-16 10:53:08.000000 dash_pydantic_form-0.1.2/dash_pydantic_form.egg-info/dependency_links.txt
+-rw-r--r--   0 renaud    (1000) renaud    (1000)      116 2024-05-16 10:53:08.000000 dash_pydantic_form-0.1.2/dash_pydantic_form.egg-info/requires.txt
+-rw-r--r--   0 renaud    (1000) renaud    (1000)       36 2024-05-16 10:53:08.000000 dash_pydantic_form-0.1.2/dash_pydantic_form.egg-info/top_level.txt
+drwxr-xr-x   0 renaud    (1000) renaud    (1000)        0 2024-05-16 10:53:08.814334 dash_pydantic_form-0.1.2/docs/
+-rw-r--r--   0 renaud    (1000) renaud    (1000)       87 2024-05-12 09:51:29.000000 dash_pydantic_form-0.1.2/docs/_config.yml
+-rw-r--r--   0 renaud    (1000) renaud    (1000)       21 2024-05-12 09:47:47.000000 dash_pydantic_form-0.1.2/docs/index.md
+drwxr-xr-x   0 renaud    (1000) renaud    (1000)        0 2024-05-16 10:53:08.824334 dash_pydantic_form-0.1.2/images/
+-rwxr-xr-x   0 renaud    (1000) renaud    (1000)    47789 2024-05-13 11:27:16.000000 dash_pydantic_form-0.1.2/images/conditionnally-visible-field.gif
+-rwxr-xr-x   0 renaud    (1000) renaud    (1000)    15290 2024-05-13 11:17:07.000000 dash_pydantic_form-0.1.2/images/editable-table.png
+-rwxr-xr-x   0 renaud    (1000) renaud    (1000)     4506 2024-05-13 11:00:42.000000 dash_pydantic_form-0.1.2/images/form-sections.png
+-rwxr-xr-x   0 renaud    (1000) renaud    (1000)    12406 2024-05-13 11:12:08.000000 dash_pydantic_form-0.1.2/images/model-list.png
+-rwxr-xr-x   0 renaud    (1000) renaud    (1000)     8028 2024-05-13 11:00:37.000000 dash_pydantic_form-0.1.2/images/nested-model.png
+-rwxr-xr-x   0 renaud    (1000) renaud    (1000)    16764 2024-05-13 10:21:46.000000 dash_pydantic_form-0.1.2/images/simple-form.png
+-rw-r--r--   0 renaud    (1000) renaud    (1000)     1186 2024-05-16 10:51:16.000000 dash_pydantic_form-0.1.2/pyproject.toml
+-rw-r--r--   0 renaud    (1000) renaud    (1000)       38 2024-05-16 10:53:08.824334 dash_pydantic_form-0.1.2/setup.cfg
+-rw-r--r--   0 renaud    (1000) renaud    (1000)     6424 2024-05-16 10:50:49.000000 dash_pydantic_form-0.1.2/usage.py
```

### Comparing `dash_pydantic_form-0.1.1/.gitignore` & `dash_pydantic_form-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.1/.vscode/launch.json` & `dash_pydantic_form-0.1.2/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.1/PKG-INFO` & `dash_pydantic_form-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: dash-pydantic-form
-Version: 0.1.1
+Version: 0.1.2
 Summary: Create Dash forms from pydantic objects
 Author-email: Renaud Lainé <renaud.laine@enea-consulting.com>
 License: Copyright ENEA Australia Pty Ltd - All Rights Reserved. Proprietary and confidential
 Project-URL: Source, https://github.com/RenaudLN/dash-pydantic-form
-Requires-Python: <3.11,>=3.10
+Requires-Python: <3.13,>=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: dash
 Requires-Dist: dash_mantine_components>=0.14
 Requires-Dist: dash_iconify
 Requires-Dist: dash_ag_grid
 Requires-Dist: pandas
 Requires-Dist: pydantic==2.*
@@ -20,14 +20,20 @@
 
 # Dash pydantic form
 
 This package allows users to quickly create forms with Plotly Dash based on pydantic models.
 
 ## Getting started
 
+Install with pip
+
+```sh
+pip install dash-pydantic-form
+```
+
 Create a pydantic model you would like to display a form for.
 
 *Note: This package uses pydantic 2.*
 
 ```py
 from datetime import date
 from typing import Literal
@@ -36,29 +42,42 @@
 class Employee(BaseModel):
     first_name: str = Field(title="First name")
     last_name: str = Field(title="Last name")
     office: Literal["au", "uk", "us", "fr"] = Field(title="Office")
     joined: date = Field(title="Employment date")
 ```
 
-Then you can get an auto-generated form with `ModelForm`, leveraging [dash-mantine-components](https://dash-mantine-components.com) for form inputs.
+Then you can get an auto-generated form with `ModelForm`, leveraging [dash-mantine-components](https://dash-mantine-components.com) (vercion 0.14) for form inputs.
 
 ```py
 from dash_pydantic_form import ModelForm
 
 # somewhere in your layout:
 form = ModelForm(
     Employee,
     aio_id="employees",
     form_id="new_employee",
 )
 ```
 
 ![Simple form](images/simple-form.png)
 
+You can also render a pre-filled form by passing an instance of the data model rather than the class
+
+```py
+# NOTE: This could come from a database
+bob = Employee(first_name="Bob", last_name="K", office="au", joined="2020-05-20")
+
+form = ModelForm(
+    bob,
+    aio_id="employees",
+    form_id="bob",
+)
+```
+
 You can then retrieve the contents of the whole form at once in a callback as follows
 
 ```py
 from dash import Input, Output, callback
 
 @callback(
     Output("some-output-id", "some-output-attribute"),
```

### Comparing `dash_pydantic_form-0.1.1/README.md` & `dash_pydantic_form-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # Dash pydantic form
 
 This package allows users to quickly create forms with Plotly Dash based on pydantic models.
 
 ## Getting started
 
+Install with pip
+
+```sh
+pip install dash-pydantic-form
+```
+
 Create a pydantic model you would like to display a form for.
 
 *Note: This package uses pydantic 2.*
 
 ```py
 from datetime import date
 from typing import Literal
@@ -16,29 +22,42 @@
 class Employee(BaseModel):
     first_name: str = Field(title="First name")
     last_name: str = Field(title="Last name")
     office: Literal["au", "uk", "us", "fr"] = Field(title="Office")
     joined: date = Field(title="Employment date")
 ```
 
-Then you can get an auto-generated form with `ModelForm`, leveraging [dash-mantine-components](https://dash-mantine-components.com) for form inputs.
+Then you can get an auto-generated form with `ModelForm`, leveraging [dash-mantine-components](https://dash-mantine-components.com) (vercion 0.14) for form inputs.
 
 ```py
 from dash_pydantic_form import ModelForm
 
 # somewhere in your layout:
 form = ModelForm(
     Employee,
     aio_id="employees",
     form_id="new_employee",
 )
 ```
 
 ![Simple form](images/simple-form.png)
 
+You can also render a pre-filled form by passing an instance of the data model rather than the class
+
+```py
+# NOTE: This could come from a database
+bob = Employee(first_name="Bob", last_name="K", office="au", joined="2020-05-20")
+
+form = ModelForm(
+    bob,
+    aio_id="employees",
+    form_id="bob",
+)
+```
+
 You can then retrieve the contents of the whole form at once in a callback as follows
 
 ```py
 from dash import Input, Output, callback
 
 @callback(
     Output("some-output-id", "some-output-attribute"),
```

### Comparing `dash_pydantic_form-0.1.1/dash_pydantic_form/fields/__init__.py` & `dash_pydantic_form-0.1.2/dash_pydantic_form/fields/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-import contextlib
+import logging
 from datetime import date, time
 from enum import Enum
-from typing import Literal, get_args, get_origin
+from types import UnionType
+from typing import Literal, Union, get_args, get_origin
 
 from pydantic import BaseModel
+from pydantic.fields import FieldInfo
 
-from dash_pydantic_form.utils import get_non_null_annotation
+from dash_pydantic_form.utils import get_non_null_annotation, is_subclass
 
 from . import all_fields as fields
 from .base_fields import BaseField, VisibilityFilter
 
 DEFAULT_FIELDS_REPR: dict[type, BaseField] = {
     str: fields.Text,
     int: fields.Number,
@@ -21,31 +23,44 @@
     Literal: fields.Select,
     Enum: fields.Select,
     BaseModel: fields.Model,
 }
 DEFAULT_REPR = fields.Json
 
 
-def get_default_repr(ann: type, **kwargs) -> BaseField:
+def get_default_repr(field_info: FieldInfo, **kwargs) -> BaseField:
     """Get default field representation."""
-    ann = get_non_null_annotation(ann)
-    with contextlib.suppress(Exception):
-        if get_origin(ann) == list and issubclass(get_args(ann)[0], BaseModel):
-            return fields.ModelList(**kwargs)
+    ann = get_non_null_annotation(field_info.annotation)
 
+    # Test for model list
+    if get_origin(ann) == list and is_subclass(get_args(ann)[0], BaseModel):
+        return fields.ModelList(**kwargs)
+
+    # Test for discriminated model
+    if field_info.discriminator:
+        if get_origin(ann) in [Union, UnionType] and all(is_subclass(x, BaseModel) for x in get_args(ann)):
+            # return fields.DiscriminatedModel(**kwargs)
+            logging.info("Discriminated model fields not yet supported.")
+        else:
+            logging.info(f"Discriminator not supported for {field_info.annotation}")
+
+    # Test for simple types
     if ann in DEFAULT_FIELDS_REPR:
         return DEFAULT_FIELDS_REPR[ann](**kwargs)
-    with contextlib.suppress(Exception):
-        origin = get_origin(ann)
-        if origin in DEFAULT_FIELDS_REPR:
-            return DEFAULT_FIELDS_REPR[origin](**kwargs)
+
+    # Test for type origin
+    origin = get_origin(ann)
+    if origin in DEFAULT_FIELDS_REPR:
+        return DEFAULT_FIELDS_REPR[origin](**kwargs)
+
+    # Test for subclass
     for type_, field_repr in DEFAULT_FIELDS_REPR.items():
-        with contextlib.suppress(Exception):
-            if issubclass(ann, type_):
-                return field_repr(**kwargs)
+        if is_subclass(ann, type_):
+            return field_repr(**kwargs)
+
     return DEFAULT_REPR(**kwargs)
 
 
 __all__ = [
     "BaseField",
     "VisibilityFilter",
     "fields",
```

### Comparing `dash_pydantic_form-0.1.1/dash_pydantic_form/fields/all_fields.py` & `dash_pydantic_form-0.1.2/dash_pydantic_form/fields/all_fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,28 +12,26 @@
 from .base_fields import SelectField as Select
 from .base_fields import SliderField as Slider
 from .base_fields import SwitchField as Switch
 from .base_fields import TextareaField as Textarea
 from .base_fields import TextField as Text
 from .base_fields import TimeField as Time
 from .editabletable_field import EditableTableField as EditableTable
-
-# from .markdown_field import MarkdownField as Markdown
-from .model_fields import ModelField as Model
-from .model_fields import ModelListField as ModelList
+from .markdown_field import MarkdownField as Markdown
+from .model_field import ModelField as Model
+from .model_list_field import ModelListField as ModelList
 
 __all__ = [
     "Checkbox",
     "Checklist",
     "Color",
     "Date",
     "EditableTable",
-    # "Image",
     "Json",
-    # "Markdown",
+    "Markdown",
     "Model",
     "ModelList",
     "MultiSelect",
     "Number",
     "Password",
     "RadioItems",
     "Range",
```

### Comparing `dash_pydantic_form-0.1.1/dash_pydantic_form/fields/base_fields.py` & `dash_pydantic_form-0.1.2/dash_pydantic_form/fields/base_fields.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import json
 import os
 from collections.abc import Callable
 from datetime import time
 from enum import Enum, EnumMeta
 from functools import partial
+from textwrap import TextWrapper
 from types import UnionType
 from typing import Any, ClassVar, Literal, Union, get_args, get_origin
 
 import dash_mantine_components as dmc
 from dash import ALL, MATCH, ClientsideFunction, Input, Output, State, clientside_callback, html
 from dash.development.base_component import Component
-from pydantic import BaseModel, field_serializer, field_validator
+from pydantic import BaseModel, Field, field_serializer, field_validator
 from pydantic.fields import FieldInfo
 from pydantic.types import annotated_types
 
 from dash_pydantic_form import ids as common_ids
 from dash_pydantic_form.utils import SEP, get_all_subclasses, get_fullpath, get_model_value, get_non_null_annotation
 
 CHECKED_COMPONENTS = [
@@ -31,27 +32,68 @@
 MAX_OPTIONS_INLINE = 4
 
 FilterOperator = Literal["==", "!=", "in", "not in", "array_contains", "array_contains_any"]
 VisibilityFilter = tuple[str, FilterOperator, Any]
 
 
 class BaseField(BaseModel):
-    """Base repr class."""
+    """Base field representation class."""
 
     base_component: ClassVar[type[Component] | None] = None
     reserved_attributes: ClassVar = ("value", "label", "description", "id", "required")
     full_width: ClassVar[bool] = False
 
-    title: str | None = None
-    description: str | None = None
-    required: bool | None = None
-    n_cols: int | None = None
-    visible: bool | VisibilityFilter | list[VisibilityFilter] | None = None
-    input_kwargs: dict | None = None
-    field_id_meta: str | None = None
+    title: str | None = Field(
+        default=None, description="Field label, overrides the title defined in the pydantic Field."
+    )
+    description: str | None = Field(
+        default=None, description="Field helper text, overrides the description defined in the pydantic Field."
+    )
+    required: bool | None = Field(
+        default=None,
+        description="Whether to display a required asterisk. If not provided, uses pydantic's field `is_required`.",
+    )
+    n_cols: int | None = Field(default=None, description="Number of columns in the form, out of 4. Default 2.")
+    visible: bool | VisibilityFilter | list[VisibilityFilter] | None = Field(
+        default=None,
+        description=(
+            "Define visibility conditions based on other form fields.\n"
+            "Accepts a boolean, a 3-tuple or list of 3-tuples with format: (field, operator, value).\n"
+            "The available operators are:\n"
+            "* '=='\n"
+            "* '!='\n"
+            "* 'in'\n"
+            "* 'not in'\n"
+            "* 'array_contains'\n"
+            "* 'array_contains_any'\n"
+            "NOTE: The field in the 3-tuples is a ':' separated path relative to the current field's "
+            "level of nesting.\n"
+            "If you need to reference a field from a parent or the root "
+            "use the special values `_parent_` or `_root_`.\n"
+            "E.g. visible=('_root_:first_name', '==', 'Bob')"
+            ""
+        ),
+    )
+    input_kwargs: dict | None = Field(
+        default=None,
+        description="Arguments to be passed to the underlying rendered component.",
+    )
+    field_id_meta: str | None = Field(default=None, description="Optional str to be set in the field id's 'meta' key.")
+
+    @classmethod
+    def __pydantic_init_subclass__(cls):
+        """Add docstring in subclasses."""
+        tw = TextWrapper(width=89, initial_indent="    ", subsequent_indent="    ")
+        result = (cls.__doc__ or "") + "\n\nParameters\n----------\n"
+        for field_name, field_info in cls.model_fields.items():
+            annotation = str(field_info.annotation)
+            description = tw.fill(field_info.description) if field_info.description else "    (missing description)"
+            result += f"{field_name}: {annotation}\n{description}\n"
+
+        cls.__doc__ = result
 
     def model_post_init(self, _context):
         """Model post init."""
         if self.n_cols is None:
             self.n_cols = 4 if self.full_width else 2
         if self.input_kwargs is None:
             self.input_kwargs = {}
@@ -400,18 +442,22 @@
 
         return value
 
 
 class SelectField(BaseField):
     """Select field."""
 
-    data_getter: Callable[[], list] | None = None
-    options_labels: dict | None = None
-    base_component = dmc.Select
+    data_getter: Callable[[], list] | None = Field(
+        default=None, description="Function to retrieve a list of options. This function takes no argument."
+    )
+    options_labels: dict | None = Field(
+        default=None, description="Mapper from option to label. Especially useful for Literals and Enums."
+    )
 
+    base_component = dmc.Select
     getters: ClassVar[dict[str, Callable]] = {}
 
     def model_post_init(self, _context):
         """Convert data_getter from serialised version to function."""
         super().model_post_init(_context)
         if self.data_getter is not None:
             self.getters[str(self.data_getter)] = self.data_getter
```

### Comparing `dash_pydantic_form-0.1.1/dash_pydantic_form/fields/editabletable_field.py` & `dash_pydantic_form-0.1.2/dash_pydantic_form/fields/editabletable_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,42 +6,44 @@
 from typing import get_args
 
 import dash_ag_grid as dag
 import dash_mantine_components as dmc
 import pandas as pd
 from dash import MATCH, ClientsideFunction, Input, Output, State, callback, clientside_callback, dcc, html, no_update
 from dash.development.base_component import Component
-from pydantic import BaseModel
+from pydantic import BaseModel, Field
 from pydantic.fields import FieldInfo
 from pydantic_core import PydanticUndefined
 
 from dash_pydantic_form import ids as common_ids
 from dash_pydantic_form.fields.base_fields import (
     BaseField,
     CheckboxField,
     RadioItemsField,
     SegmentedControlField,
     SelectField,
     TextareaField,
     TextField,
 )
+from dash_pydantic_form.fields.markdown_field import MarkdownField
 from dash_pydantic_form.ids import field_dependent_id
-
-# from dash_pydantic_form.form_helpers.markdown_field import MarkdownField
 from dash_pydantic_form.utils import get_fullpath, get_non_null_annotation
 
 
 class EditableTableField(BaseField):
     """Editable table input field attributes and rendering."""
 
-    fields_repr: dict[str, dict | BaseField] | None = None
-    with_upload: bool = True
-    rows_editable: bool = True
-    table_height: int = 300
-    column_defs_overrides: dict | None = None
+    fields_repr: dict[str, dict | BaseField] | None = Field(
+        default=None,
+        description="Fields representation, mapping between field name and field representation for the nested fields.",
+    )
+    with_upload: bool = Field(default=True, description="Whether to allow uploading a CSV file.")
+    rows_editable: bool = Field(default=True, description="Whether to allow editing rows.")
+    table_height: int = Field(default=300, description="Table rows height in pixels.")
+    column_defs_overrides: dict[str, dict] | None = Field(default=None, description="Ag-grid column_defs overrides.")
 
     full_width = True
 
     def model_post_init(self, _context):
         """Model post init."""
         super().model_post_init(_context)
         if self.fields_repr is None:
@@ -183,15 +185,15 @@
             ]
 
         def get_field_repr(field: str) -> BaseField | dict:
             from dash_pydantic_form.fields import get_default_repr
 
             if field in self.fields_repr:
                 return self.fields_repr[field]
-            return get_default_repr(template.model_fields[field].annotation)
+            return get_default_repr(template.model_fields[field])
 
         title = self.get_title(field_info, field_name=field)
         description = self.get_description(field_info)
         return html.Div(
             [
                 html.Div(
                     (title is not None)
@@ -280,15 +282,15 @@
         required_field: bool,
         editable: bool = True,
     ):
         """Takes a field and generates the 'columnDefs' dictionary for said field based on its type."""
         from dash_pydantic_form.fields import get_default_repr
 
         if isinstance(field_repr, dict):
-            field_repr = get_default_repr(field_info.annotation, **field_repr)
+            field_repr = get_default_repr(field_info, **field_repr)
         # Column_def no matter the type
         column_def = {
             "editable": editable,
             "field": field_name,
             "headerName": field_repr.get_title(field_info, field_name=field_name),
             "required": required_field,
             "cellClass": {
@@ -334,24 +336,24 @@
                         "function": "selectRequiredCell(params)",
                     }
                     if required_field
                     else None,
                 }
             )
 
-        if isinstance(field_info, TextareaField):  # MarkdownField)):
+        if isinstance(field_info, TextareaField | MarkdownField):
             column_def.update(
                 {
                     "cellEditor": "agLargeTextCellEditor",
                     "cellEditorPopup": True,
                     "cellEditorParams": {"maxLength": 100, "rows": 10, "cols": 50},
                 }
             )
 
-        if isinstance(field_info, TextField | TextareaField):  # MarkdownField)):
+        if isinstance(field_info, TextField | TextareaField | MarkdownField):
             column_def.update({"dtype": "str"})
 
         if isinstance(field_info, CheckboxField):
             column_def.update({"cellRenderer": "PydfCheckbox", "editable": False})
 
         if get_non_null_annotation(field_info.annotation) == date:
             column_def.update(
```

### Comparing `dash_pydantic_form-0.1.1/dash_pydantic_form/fields/model_fields.py` & `dash_pydantic_form-0.1.2/dash_pydantic_form/fields/model_list_field.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,236 +16,50 @@
     ctx,
     dcc,
     html,
     no_update,
 )
 from dash.development.base_component import Component
 from dash_iconify import DashIconify
-from pydantic import BaseModel
+from pydantic import BaseModel, Field
 from pydantic.fields import FieldInfo
 
 from dash_pydantic_form import ids as common_ids
 from dash_pydantic_form.fields.base_fields import BaseField
 from dash_pydantic_form.form_section import Sections
 from dash_pydantic_form.utils import (
     get_fullpath,
     get_model_cls,
     get_subitem_cls,
 )
 
 
-class ModelField(BaseField):
-    """Model field, used for nested BaseModel.
-
-    Optional attributes:
-    * render_type (one of 'accordion', 'modal', default 'accordion')
-    * fields_repr, mapping between field name and field representation
-    * sections, list of FormSection for the NestedModel form
-    """
-
-    render_type: Literal["accordion", "modal"] = "accordion"
-    fields_repr: dict[str, dict | BaseField] | None = None
-    sections: Sections = None
-
-    full_width = True
-
-    def model_post_init(self, _context):
-        """Model post init."""
-        super().model_post_init(_context)
-        if self.fields_repr is None:
-            self.fields_repr = {}
-
-    class ids(BaseField.ids):
-        """Model field ids."""
-
-        form_wrapper = partial(common_ids.field_dependent_id, "_pydf-model-form-wrapper")
-        edit = partial(common_ids.field_dependent_id, "_pydf-model-field-edit")
-        modal = partial(common_ids.field_dependent_id, "_pydf-model-field-modal")
-        modal_save = partial(common_ids.field_dependent_id, "_pydf-model-field-modal-save")
-
-    def modal_item(  # noqa: PLR0913
-        self,
-        item: BaseModel,
-        aio_id: str,
-        form_id: str,
-        field: str,
-        parent: str = "",
-        field_info: FieldInfo | None = None,
-    ) -> Component:
-        """Model field modal render."""
-        from dash_pydantic_form import ModelForm
-
-        title = self.get_title(field_info, field_name=field)
-        new_parent = get_fullpath(parent, field)
-        return dmc.Paper(
-            dmc.Group(
-                [
-                    dmc.Text(
-                        title,
-                        style={
-                            "flex": 1,
-                            "overflow": "hidden",
-                            "textOverflow": "ellipsis",
-                            "whiteSpace": "nowrap",
-                        },
-                    ),
-                    dmc.Group(
-                        [
-                            dmc.ActionIcon(
-                                DashIconify(icon="carbon:edit", height=16),
-                                variant="light",
-                                size="sm",
-                                id=self.ids.edit(aio_id, form_id, field, parent=parent),
-                            ),
-                        ],
-                        gap="0.25rem",
-                    ),
-                    dmc.Modal(
-                        [
-                            ModelForm(
-                                item=item,
-                                aio_id=aio_id,
-                                form_id=form_id,
-                                path=new_parent,
-                                fields_repr=self.fields_repr,
-                                sections=self.sections,
-                            ),
-                            dmc.Group(
-                                dmc.Button(
-                                    "Save",
-                                    leftSection=DashIconify(icon="carbon:save"),
-                                    id=self.ids.modal_save(aio_id, form_id, field, parent=parent),
-                                ),
-                                justify="right",
-                                mt="sm",
-                            ),
-                        ],
-                        title=title,
-                        id=self.ids.modal(aio_id, form_id, field, parent=parent),
-                        style={"--modal-size": "min(calc(100vw - 4rem), 1150px)"},
-                    ),
-                ],
-                gap="sm",
-                align="top",
-            ),
-            withBorder=True,
-            radius="sm",
-            p="xs",
-            className="pydf-model-list-modal-item",
-        )
-
-    def accordion_item(  # noqa: PLR0913
-        self,
-        item: BaseModel,
-        aio_id: str,
-        form_id: str,
-        field: str,
-        parent: str = "",
-        field_info: FieldInfo | None = None,
-    ) -> Component:
-        """Model field accordion item render."""
-        from dash_pydantic_form import ModelForm
-
-        title = self.get_title(field_info, field_name=field)
-        description = self.get_description(field_info)
-        return dmc.Accordion(
-            dmc.AccordionItem(
-                value="item",
-                children=[
-                    dmc.AccordionControl(dmc.Text(title)),
-                    dmc.AccordionPanel(
-                        [
-                            *([dmc.Text(description, size="xs", c="dimmed")] * bool(title) * bool(description)),
-                            ModelForm(
-                                item=item,
-                                aio_id=aio_id,
-                                form_id=form_id,
-                                path=get_fullpath(parent, field),
-                                fields_repr=self.fields_repr,
-                                sections=self.sections,
-                            ),
-                        ],
-                        id=self.ids.form_wrapper(aio_id, form_id, field, parent=parent),
-                    ),
-                ],
-            ),
-            value="item",
-            styles={
-                "control": {"padding": "0.5rem"},
-                "label": {"padding": 0},
-                "item": {
-                    "border": "1px solid color-mix(in srgb, var(--mantine-color-gray-light), transparent 40%)",
-                    "background": "color-mix(in srgb, var(--mantine-color-gray-light), transparent 80%)",
-                    "marginBottom": "0.5rem",
-                    "borderRadius": "0.25rem",
-                },
-                "content": {
-                    "display": "flex",
-                    "flexDirection": "column",
-                    "gap": "0.375rem",
-                    "padding": "0.125rem 0.5rem 0.5rem",
-                },
-            },
-            style={"gridColumn": "span var(--col-4-4)"},
-        )
-
-    def _render(  # noqa: PLR0913
-        self,
-        *,
-        item: BaseModel,
-        aio_id: str,
-        form_id: str,
-        field: str,
-        parent: str = "",
-        field_info: FieldInfo | None = None,
-    ) -> Component:
-        """Create a form field of type checklist to interact with the model field."""
-        if self.render_type == "accordion":
-            input_ = self.accordion_item(item, aio_id, form_id, field, parent, field_info)
-        elif self.render_type == "modal":
-            input_ = self.modal_item(item, aio_id, form_id, field, parent, field_info)
-        else:
-            raise ValueError("Unknown render type.")
-        return input_
-
-    # Open a model modal when editing an item
-    clientside_callback(
-        ClientsideFunction(namespace="pydf", function_name="syncTrue"),
-        Output(ids.modal(MATCH, MATCH, MATCH, MATCH, MATCH), "opened", allow_duplicate=True),
-        Input(ids.edit(MATCH, MATCH, MATCH, MATCH, MATCH), "n_clicks"),
-        prevent_initial_call=True,
-    )
-
-    # Close a model modal when saving an item
-    clientside_callback(
-        ClientsideFunction(namespace="pydf", function_name="syncFalse"),
-        Output(ids.modal(MATCH, MATCH, MATCH, MATCH, MATCH), "opened", allow_duplicate=True),
-        Input(ids.modal_save(MATCH, MATCH, MATCH, MATCH, MATCH), "n_clicks"),
-        prevent_initial_call=True,
-    )
-
-
 class ModelListField(BaseField):
     """Model list field, used for list of nested BaseModel.
 
     Optional attributes:
     * render_type (one of 'accordion', 'modal', 'list', default 'accordion')
         new render types can be defined by extending this class and overriding
         the following methods: _contents_renderer and render_type_item_mapper
     * fields_repr, mapping between field name and field representation
     * sections, list of FormSection for the NestedModel form
     * items_deletable, whether the items can be deleted (bool, default True)
     * items_creatable, whether new items can be created (bool, default True)
     """
 
-    render_type: Literal["accordion", "modal", "list"] = "accordion"
-    fields_repr: dict[str, dict | BaseField] | None = None
-    sections: Sections | None = None
-    items_deletable: bool = True
-    items_creatable: bool = True
+    render_type: Literal["accordion", "modal", "list"] = Field(
+        default="accordion", description="How to render the list of items, one  of 'accordion', 'modal', 'list'."
+    )
+    fields_repr: dict[str, dict | BaseField] | None = Field(
+        default=None,
+        description="Fields representation, mapping between field name and field representation for the nested fields.",
+    )
+    sections: Sections | None = Field(default=None, description="Sub-form sections.")
+    items_deletable: bool = Field(default=True, description="Whether the items can be deleted.")
+    items_creatable: bool = Field(default=True, description="Whether new items can be created.")
 
     full_width = True
 
     def model_post_init(self, _context):
         """Model post init."""
         super().model_post_init(_context)
         if self.fields_repr is None:
@@ -567,15 +381,15 @@
         title = self.get_title(field_info, field_name=field)
         description = self.get_description(field_info)
 
         subitem_cls = get_subitem_cls(item, get_fullpath(parent, field, "0"))
         fields_repr_dicts = (
             {
                 field_name: (
-                    get_default_repr(subitem_cls.model_fields[field_name].annotation, **field_repr)
+                    get_default_repr(subitem_cls.model_fields[field_name], **field_repr)
                     if isinstance(field_repr, dict)
                     else field_repr
                 ).to_dict()
                 for field_name, field_repr in self.fields_repr.items()
             }
             if self.fields_repr
             else None
```

### Comparing `dash_pydantic_form-0.1.1/dash_pydantic_form/ids.py` & `dash_pydantic_form-0.1.2/dash_pydantic_form/ids.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.1/dash_pydantic_form/model_form.py` & `dash_pydantic_form-0.1.2/dash_pydantic_form/model_form.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,20 +18,41 @@
 
 
 def form_base_id(part: str, aio_id: str, form_id: str):
     """Form parts id."""
     return {"part": part, "aio_id": aio_id, "form_id": form_id}
 
 
+Children_ = Component | str | int | float
+Children = Children_ | list[Children_]
 SectionRender = Literal["accordion", "tabs", "steps"]
 Position = Literal["top", "bottom", "none"]
 
 
 class ModelForm(html.Div):
-    """Model form."""
+    """Create a Dash form from a pydantic model.
+
+    Parameters
+    ----------
+    item: BaseModel | type[BaseModel]
+        The model to create the form from, can be the model class or an instance of the class.
+        If the class is passed, the form will be empty. If an instance is passed, the form will be pre-filled
+        with existing values.
+    aio_id: str
+        All-in-one component ID
+    form_id: str
+        Form ID, can be used to create multiple forms on the same page. When working with databases
+        this could be the document / record ID.
+    fields_repr: dict[str, dict | BaseField] | None
+        Mapping between field name and field representation. If not provided, default field
+        representations will be used based on the field annotation.
+        See :meth:`dash_pydantic_form.fields.get_default_repr`.
+    sections: Sections | None
+        List of form sections (optional). See :class:`dash_pydantic_form.form_section.Sections`.
+    """
 
     class ids:
         """Model form ids."""
 
         main = partial(form_base_id, "_pydantic-form-main")
         accordion = partial(form_base_id, "_pydantic-form-accordion")
         tabs = partial(form_base_id, "_pydantic-form-tabs")
@@ -60,19 +81,19 @@
         field_inputs = {}
         subitem_cls = get_subitem_cls(item.__class__, path)
         for field_name, field_info in subitem_cls.model_fields.items():
             if sections and field_name in sections.excluded_fields:
                 continue
             if field_name in fields_repr:
                 if isinstance(fields_repr[field_name], dict):
-                    field_repr = get_default_repr(field_info.annotation, **fields_repr[field_name])
+                    field_repr = get_default_repr(field_info, **fields_repr[field_name])
                 else:
                     field_repr = fields_repr[field_name]
             else:
-                field_repr = get_default_repr(field_info.annotation)
+                field_repr = get_default_repr(field_info)
 
             field_inputs[field_name] = field_repr.render(
                 item=item,
                 aio_id=aio_id,
                 form_id=form_id,
                 field=field_name,
                 parent=path,
@@ -116,15 +137,15 @@
 
         if not path:
             children.append(dcc.Store(id=self.ids.main(aio_id, form_id)))
 
         super().__init__(children=children)
 
     @classmethod
-    def grid(cls, children, **kwargs):
+    def grid(cls, children: Children, **kwargs):
         """Create the responsive grid for a field."""
         return dmc.SimpleGrid(children, cols={"base": 1, "sm": 4}, className="pydantic-form-grid", **kwargs)
 
     @classmethod
     def render_accordion_sections(
         cls,
         *,
```

### Comparing `dash_pydantic_form-0.1.1/dash_pydantic_form/pydantic_form_scripts.js` & `dash_pydantic_form-0.1.2/dash_pydantic_form/pydantic_form_scripts.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -234,14 +234,15 @@
                 ...state.value,
                 display: checkVisibility(actualValue, operator, expectedValue) ? null : "none",
             })
         })
 
         return newStyles
     },
+    sync: x => x,
     syncTrue: x => !!x,
     syncFalse: x => !x,
     updateModalTitle: (val) => {
         return val != null ? Array(2).fill(String(val)) : Array(2).fill(dash_clientside.no_update)
     },
     updateAccordionTitle: (val) => {
         return val != null ? String(val) : dash_clientside.no_update
```

### Comparing `dash_pydantic_form-0.1.1/dash_pydantic_form/utils.py` & `dash_pydantic_form-0.1.2/dash_pydantic_form/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -33,29 +33,35 @@
 
 
 def get_non_null_annotation(annotation: type[Any]) -> type[Any]:
     """Get a non-null annotation.
 
     e.g., get_non_null_annotation(Optional[str]) = str
     """
-    if (
-        get_origin(annotation) in [Union, UnionType]
-        and len(non_null_ann := list(set(get_args(annotation)) - {type(None)})) == 1
-    ):
-        return non_null_ann[0]
+    if get_origin(annotation) in [Union, UnionType]:
+        args = tuple(x for x in get_args(annotation) if x != type(None))
+        if len(args) == 1:
+            return args[0]
+        return Union[args]  # noqa: UP007
     return annotation
 
 
 def get_model_value(item: BaseModel, field: str, parent: str, allow_default: bool = True):
     """Get the value of a model (parent, field) pair.
 
-    :param item: The object to get the value from
-    :param parent: The parent of the field (for nested fields), in dot notation
-    :param field: The field name
-    :param allow_default: Allow to return the default value, when the object has been created with model_construct.
+    Parameters
+    ----------
+    item: BaseModel
+        The object to get the value from
+    field: str
+        The field name
+    parent: str
+        The parent of the field (for nested fields), in dot notation
+    allow_default: bool
+        Allow to return the default value, when the object has been created with model_construct.
     """
     try:
         return get_subitem(item, parent)[field]
     except:
         if allow_default:
             field_info = get_subitem_cls(item, parent).model_fields[field]
             if field_info.default is not PydanticUndefined:
@@ -132,7 +138,15 @@
 
     return all_subclasses
 
 
 def get_model_cls(str_repr: str) -> type[BaseModel]:
     """Get the model class from a string representation."""
     return next(cls for cls in get_all_subclasses(BaseModel) if str(cls) == str_repr)
+
+
+def is_subclass(cls: type, base_cls: type) -> bool:
+    """Check if a class is a subclass of another class, handling issubclass errors."""
+    try:
+        return issubclass(cls, base_cls)
+    except TypeError:
+        return False
```

### Comparing `dash_pydantic_form-0.1.1/dash_pydantic_form.egg-info/PKG-INFO` & `dash_pydantic_form-0.1.2/dash_pydantic_form.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: dash-pydantic-form
-Version: 0.1.1
+Version: 0.1.2
 Summary: Create Dash forms from pydantic objects
 Author-email: Renaud Lainé <renaud.laine@enea-consulting.com>
 License: Copyright ENEA Australia Pty Ltd - All Rights Reserved. Proprietary and confidential
 Project-URL: Source, https://github.com/RenaudLN/dash-pydantic-form
-Requires-Python: <3.11,>=3.10
+Requires-Python: <3.13,>=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: dash
 Requires-Dist: dash_mantine_components>=0.14
 Requires-Dist: dash_iconify
 Requires-Dist: dash_ag_grid
 Requires-Dist: pandas
 Requires-Dist: pydantic==2.*
@@ -20,14 +20,20 @@
 
 # Dash pydantic form
 
 This package allows users to quickly create forms with Plotly Dash based on pydantic models.
 
 ## Getting started
 
+Install with pip
+
+```sh
+pip install dash-pydantic-form
+```
+
 Create a pydantic model you would like to display a form for.
 
 *Note: This package uses pydantic 2.*
 
 ```py
 from datetime import date
 from typing import Literal
@@ -36,29 +42,42 @@
 class Employee(BaseModel):
     first_name: str = Field(title="First name")
     last_name: str = Field(title="Last name")
     office: Literal["au", "uk", "us", "fr"] = Field(title="Office")
     joined: date = Field(title="Employment date")
 ```
 
-Then you can get an auto-generated form with `ModelForm`, leveraging [dash-mantine-components](https://dash-mantine-components.com) for form inputs.
+Then you can get an auto-generated form with `ModelForm`, leveraging [dash-mantine-components](https://dash-mantine-components.com) (vercion 0.14) for form inputs.
 
 ```py
 from dash_pydantic_form import ModelForm
 
 # somewhere in your layout:
 form = ModelForm(
     Employee,
     aio_id="employees",
     form_id="new_employee",
 )
 ```
 
 ![Simple form](images/simple-form.png)
 
+You can also render a pre-filled form by passing an instance of the data model rather than the class
+
+```py
+# NOTE: This could come from a database
+bob = Employee(first_name="Bob", last_name="K", office="au", joined="2020-05-20")
+
+form = ModelForm(
+    bob,
+    aio_id="employees",
+    form_id="bob",
+)
+```
+
 You can then retrieve the contents of the whole form at once in a callback as follows
 
 ```py
 from dash import Input, Output, callback
 
 @callback(
     Output("some-output-id", "some-output-attribute"),
```

### Comparing `dash_pydantic_form-0.1.1/dash_pydantic_form.egg-info/SOURCES.txt` & `dash_pydantic_form-0.1.2/dash_pydantic_form.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 dash_pydantic_form.egg-info/dependency_links.txt
 dash_pydantic_form.egg-info/requires.txt
 dash_pydantic_form.egg-info/top_level.txt
 dash_pydantic_form/fields/__init__.py
 dash_pydantic_form/fields/all_fields.py
 dash_pydantic_form/fields/base_fields.py
 dash_pydantic_form/fields/editabletable_field.py
-dash_pydantic_form/fields/model_fields.py
+dash_pydantic_form/fields/markdown_field.py
+dash_pydantic_form/fields/model_field.py
+dash_pydantic_form/fields/model_list_field.py
 docs/_config.yml
 docs/index.md
 images/conditionnally-visible-field.gif
 images/editable-table.png
 images/form-sections.png
 images/model-list.png
 images/nested-model.png
```

### Comparing `dash_pydantic_form-0.1.1/images/conditionnally-visible-field.gif` & `dash_pydantic_form-0.1.2/images/conditionnally-visible-field.gif`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.1/images/editable-table.png` & `dash_pydantic_form-0.1.2/images/editable-table.png`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.1/images/form-sections.png` & `dash_pydantic_form-0.1.2/images/form-sections.png`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.1/images/model-list.png` & `dash_pydantic_form-0.1.2/images/model-list.png`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.1/images/nested-model.png` & `dash_pydantic_form-0.1.2/images/nested-model.png`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.1/images/simple-form.png` & `dash_pydantic_form-0.1.2/images/simple-form.png`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.1/pyproject.toml` & `dash_pydantic_form-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = "dash-pydantic-form"
 dynamic = ["version"]
 description = "Create Dash forms from pydantic objects"
 authors = [
     {name = "Renaud Lainé", email = "renaud.laine@enea-consulting.com"},
 ]
 readme = "README.md"
-requires-python =  ">=3.10,<3.11"
+requires-python =  ">=3.10,<3.13"
 license = {text = "Copyright ENEA Australia Pty Ltd - All Rights Reserved. Proprietary and confidential"}
 dependencies = [
     "dash",
     "dash_mantine_components>=0.14",
     "dash_iconify",
     "dash_ag_grid",
     "pandas",
```

### Comparing `dash_pydantic_form-0.1.1/usage.py` & `dash_pydantic_form-0.1.2/usage.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 
 
 class Employee(BaseModel):
     """Employee model."""
 
     name: str = Field(title="Name", description="Name of the employee")
     age: int = Field(title="Age", description="Age of the employee, starting from their birth")
+    mini_bio: str | None = Field(title="Mini bio", description="Short bio of the employee", default=None)
     joined: date = Field(title="Joined", description="Date when the employee joined the company")
     office: Office = Field(title="Office", description="Office of the employee")
     metadata: Metadata | None = Field(title="Employee metadata", default=None)
     pets: list[Pet] = Field(title="Pets", description="Employee pets", default_factory=list)
 
 
 bob = Employee(name="Bob", age=30, joined="2020-01-01", office="au", pets=[{"name": "Rex", "species": "dog"}])
@@ -82,14 +83,15 @@
                     [
                         dmc.Title("Dash Pydantic form", mb="1rem", order=3),
                         ModelForm(
                             Employee,
                             AIO_ID,
                             FORM_ID,
                             fields_repr={
+                                "mini_bio": fields.Markdown(),
                                 "office": fields.RadioItems(
                                     options_labels={"au": "Australia", "fr": "France"},
                                 ),
                                 "metadata": {
                                     "render_type": "accordion",
                                     "fields_repr": {
                                         "languages": fields.Checklist(
@@ -108,15 +110,15 @@
                                         "species": {"options_labels": {"dog": "Dog", "cat": "Cat"}},
                                     },
                                     table_height=200,
                                 ),
                             },
                             sections=Sections(
                                 sections=[
-                                    FormSection(name="General", fields=["name", "age"], default_open=True),
+                                    FormSection(name="General", fields=["name", "age", "mini_bio"], default_open=True),
                                     FormSection(name="HR", fields=["office", "joined", "metadata"], default_open=True),
                                     FormSection(name="Other", fields=["pets"], default_open=True),
                                 ],
                                 render="accordion",
                             ),
                         ),
                     ],
```

