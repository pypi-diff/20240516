# Comparing `tmp/dash_pydantic_form-0.1.2.tar.gz` & `tmp/dash_pydantic_form-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_pydantic_form-0.1.2.tar", last modified: Thu May 16 10:53:08 2024, max compression
+gzip compressed data, was "dash_pydantic_form-0.1.3.tar", last modified: Thu May 16 13:13:21 2024, max compression
```

## Comparing `dash_pydantic_form-0.1.2.tar` & `dash_pydantic_form-0.1.3.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 renaud    (1000) renaud    (1000)        0 2024-05-16 10:53:08.824334 dash_pydantic_form-0.1.2/
--rw-r--r--   0 renaud    (1000) renaud    (1000)     3231 2024-04-25 01:57:38.000000 dash_pydantic_form-0.1.2/.gitignore
--rw-r--r--   0 renaud    (1000) renaud    (1000)      406 2024-05-11 12:42:14.000000 dash_pydantic_form-0.1.2/.pre-commit-config.yaml
-drwxr-xr-x   0 renaud    (1000) renaud    (1000)        0 2024-05-16 10:53:08.804334 dash_pydantic_form-0.1.2/.vscode/
--rw-r--r--   0 renaud    (1000) renaud    (1000)      834 2024-05-12 04:37:36.000000 dash_pydantic_form-0.1.2/.vscode/launch.json
--rw-r--r--   0 renaud    (1000) renaud    (1000)      454 2024-05-16 10:52:16.000000 dash_pydantic_form-0.1.2/CHANGELOG.md
--rw-r--r--   0 renaud    (1000) renaud    (1000)     7487 2024-05-16 10:53:08.824334 dash_pydantic_form-0.1.2/PKG-INFO
--rw-r--r--   0 renaud    (1000) renaud    (1000)     6784 2024-05-13 22:03:05.000000 dash_pydantic_form-0.1.2/README.md
-drwxr-xr-x   0 renaud    (1000) renaud    (1000)        0 2024-05-16 10:53:08.804334 dash_pydantic_form-0.1.2/dash_pydantic_form/
--rw-r--r--   0 renaud    (1000) renaud    (1000)      749 2024-05-14 12:37:15.000000 dash_pydantic_form-0.1.2/dash_pydantic_form/__init__.py
-drwxr-xr-x   0 renaud    (1000) renaud    (1000)        0 2024-05-16 10:53:08.814334 dash_pydantic_form-0.1.2/dash_pydantic_form/fields/
--rw-r--r--   0 renaud    (1000) renaud    (1000)     1972 2024-05-16 10:50:49.000000 dash_pydantic_form-0.1.2/dash_pydantic_form/fields/__init__.py
--rw-r--r--   0 renaud    (1000) renaud    (1000)     1399 2024-05-16 10:50:49.000000 dash_pydantic_form-0.1.2/dash_pydantic_form/fields/all_fields.py
--rw-r--r--   0 renaud    (1000) renaud    (1000)    21730 2024-05-14 12:37:15.000000 dash_pydantic_form-0.1.2/dash_pydantic_form/fields/base_fields.py
--rw-r--r--   0 renaud    (1000) renaud    (1000)    18943 2024-05-14 13:01:55.000000 dash_pydantic_form-0.1.2/dash_pydantic_form/fields/editabletable_field.py
--rw-r--r--   0 renaud    (1000) renaud    (1000)     1994 2024-05-14 12:37:15.000000 dash_pydantic_form-0.1.2/dash_pydantic_form/fields/markdown_field.py
--rw-r--r--   0 renaud    (1000) renaud    (1000)     8218 2024-05-16 10:50:49.000000 dash_pydantic_form-0.1.2/dash_pydantic_form/fields/model_field.py
--rw-r--r--   0 renaud    (1000) renaud    (1000)    21436 2024-05-14 13:16:15.000000 dash_pydantic_form-0.1.2/dash_pydantic_form/fields/model_list_field.py
--rw-r--r--   0 renaud    (1000) renaud    (1000)     2145 2024-05-14 12:37:15.000000 dash_pydantic_form-0.1.2/dash_pydantic_form/form_section.py
--rw-r--r--   0 renaud    (1000) renaud    (1000)      944 2024-05-11 12:54:05.000000 dash_pydantic_form-0.1.2/dash_pydantic_form/ids.py
--rw-r--r--   0 renaud    (1000) renaud    (1000)    13585 2024-05-16 10:50:49.000000 dash_pydantic_form-0.1.2/dash_pydantic_form/model_form.py
--rw-r--r--   0 renaud    (1000) renaud    (1000)     8201 2024-05-14 12:37:15.000000 dash_pydantic_form-0.1.2/dash_pydantic_form/pydantic_form_scripts.js
--rw-r--r--   0 renaud    (1000) renaud    (1000)     2102 2024-05-14 12:37:15.000000 dash_pydantic_form-0.1.2/dash_pydantic_form/pydantic_form_styles.css
--rw-r--r--   0 renaud    (1000) renaud    (1000)     4834 2024-05-16 10:50:49.000000 dash_pydantic_form-0.1.2/dash_pydantic_form/utils.py
-drwxr-xr-x   0 renaud    (1000) renaud    (1000)        0 2024-05-16 10:53:08.824334 dash_pydantic_form-0.1.2/dash_pydantic_form.egg-info/
--rw-r--r--   0 renaud    (1000) renaud    (1000)     7487 2024-05-16 10:53:08.000000 dash_pydantic_form-0.1.2/dash_pydantic_form.egg-info/PKG-INFO
--rw-r--r--   0 renaud    (1000) renaud    (1000)     1041 2024-05-16 10:53:08.000000 dash_pydantic_form-0.1.2/dash_pydantic_form.egg-info/SOURCES.txt
--rw-r--r--   0 renaud    (1000) renaud    (1000)        1 2024-05-16 10:53:08.000000 dash_pydantic_form-0.1.2/dash_pydantic_form.egg-info/dependency_links.txt
--rw-r--r--   0 renaud    (1000) renaud    (1000)      116 2024-05-16 10:53:08.000000 dash_pydantic_form-0.1.2/dash_pydantic_form.egg-info/requires.txt
--rw-r--r--   0 renaud    (1000) renaud    (1000)       36 2024-05-16 10:53:08.000000 dash_pydantic_form-0.1.2/dash_pydantic_form.egg-info/top_level.txt
-drwxr-xr-x   0 renaud    (1000) renaud    (1000)        0 2024-05-16 10:53:08.814334 dash_pydantic_form-0.1.2/docs/
--rw-r--r--   0 renaud    (1000) renaud    (1000)       87 2024-05-12 09:51:29.000000 dash_pydantic_form-0.1.2/docs/_config.yml
--rw-r--r--   0 renaud    (1000) renaud    (1000)       21 2024-05-12 09:47:47.000000 dash_pydantic_form-0.1.2/docs/index.md
-drwxr-xr-x   0 renaud    (1000) renaud    (1000)        0 2024-05-16 10:53:08.824334 dash_pydantic_form-0.1.2/images/
--rwxr-xr-x   0 renaud    (1000) renaud    (1000)    47789 2024-05-13 11:27:16.000000 dash_pydantic_form-0.1.2/images/conditionnally-visible-field.gif
--rwxr-xr-x   0 renaud    (1000) renaud    (1000)    15290 2024-05-13 11:17:07.000000 dash_pydantic_form-0.1.2/images/editable-table.png
--rwxr-xr-x   0 renaud    (1000) renaud    (1000)     4506 2024-05-13 11:00:42.000000 dash_pydantic_form-0.1.2/images/form-sections.png
--rwxr-xr-x   0 renaud    (1000) renaud    (1000)    12406 2024-05-13 11:12:08.000000 dash_pydantic_form-0.1.2/images/model-list.png
--rwxr-xr-x   0 renaud    (1000) renaud    (1000)     8028 2024-05-13 11:00:37.000000 dash_pydantic_form-0.1.2/images/nested-model.png
--rwxr-xr-x   0 renaud    (1000) renaud    (1000)    16764 2024-05-13 10:21:46.000000 dash_pydantic_form-0.1.2/images/simple-form.png
--rw-r--r--   0 renaud    (1000) renaud    (1000)     1186 2024-05-16 10:51:16.000000 dash_pydantic_form-0.1.2/pyproject.toml
--rw-r--r--   0 renaud    (1000) renaud    (1000)       38 2024-05-16 10:53:08.824334 dash_pydantic_form-0.1.2/setup.cfg
--rw-r--r--   0 renaud    (1000) renaud    (1000)     6424 2024-05-16 10:50:49.000000 dash_pydantic_form-0.1.2/usage.py
+drwxr-xr-x   0 renaud    (1000) renaud    (1000)        0 2024-05-16 13:13:21.093371 dash_pydantic_form-0.1.3/
+-rw-r--r--   0 renaud    (1000) renaud    (1000)     3231 2024-04-25 01:57:38.000000 dash_pydantic_form-0.1.3/.gitignore
+-rw-r--r--   0 renaud    (1000) renaud    (1000)      406 2024-05-11 12:42:14.000000 dash_pydantic_form-0.1.3/.pre-commit-config.yaml
+drwxr-xr-x   0 renaud    (1000) renaud    (1000)        0 2024-05-16 13:13:21.083371 dash_pydantic_form-0.1.3/.vscode/
+-rw-r--r--   0 renaud    (1000) renaud    (1000)      834 2024-05-12 04:37:36.000000 dash_pydantic_form-0.1.3/.vscode/launch.json
+-rw-r--r--   0 renaud    (1000) renaud    (1000)      523 2024-05-16 13:12:46.000000 dash_pydantic_form-0.1.3/CHANGELOG.md
+-rw-r--r--   0 renaud    (1000) renaud    (1000)     8673 2024-05-16 13:13:21.093371 dash_pydantic_form-0.1.3/PKG-INFO
+-rw-r--r--   0 renaud    (1000) renaud    (1000)     7970 2024-05-16 13:12:27.000000 dash_pydantic_form-0.1.3/README.md
+drwxr-xr-x   0 renaud    (1000) renaud    (1000)        0 2024-05-16 13:13:21.083371 dash_pydantic_form-0.1.3/dash_pydantic_form/
+-rw-r--r--   0 renaud    (1000) renaud    (1000)      749 2024-05-14 12:37:15.000000 dash_pydantic_form-0.1.3/dash_pydantic_form/__init__.py
+drwxr-xr-x   0 renaud    (1000) renaud    (1000)        0 2024-05-16 13:13:21.093371 dash_pydantic_form-0.1.3/dash_pydantic_form/fields/
+-rw-r--r--   0 renaud    (1000) renaud    (1000)     1609 2024-05-16 13:12:27.000000 dash_pydantic_form-0.1.3/dash_pydantic_form/fields/__init__.py
+-rw-r--r--   0 renaud    (1000) renaud    (1000)     1399 2024-05-16 13:02:52.000000 dash_pydantic_form-0.1.3/dash_pydantic_form/fields/all_fields.py
+-rw-r--r--   0 renaud    (1000) renaud    (1000)    21910 2024-05-16 13:12:27.000000 dash_pydantic_form-0.1.3/dash_pydantic_form/fields/base_fields.py
+-rw-r--r--   0 renaud    (1000) renaud    (1000)    18943 2024-05-14 13:01:55.000000 dash_pydantic_form-0.1.3/dash_pydantic_form/fields/editabletable_field.py
+-rw-r--r--   0 renaud    (1000) renaud    (1000)     1994 2024-05-14 12:37:15.000000 dash_pydantic_form-0.1.3/dash_pydantic_form/fields/markdown_field.py
+-rw-r--r--   0 renaud    (1000) renaud    (1000)     8536 2024-05-16 13:12:27.000000 dash_pydantic_form-0.1.3/dash_pydantic_form/fields/model_field.py
+-rw-r--r--   0 renaud    (1000) renaud    (1000)    21436 2024-05-14 13:16:15.000000 dash_pydantic_form-0.1.3/dash_pydantic_form/fields/model_list_field.py
+-rw-r--r--   0 renaud    (1000) renaud    (1000)     2145 2024-05-14 12:37:15.000000 dash_pydantic_form-0.1.3/dash_pydantic_form/form_section.py
+-rw-r--r--   0 renaud    (1000) renaud    (1000)      944 2024-05-11 12:54:05.000000 dash_pydantic_form-0.1.3/dash_pydantic_form/ids.py
+-rw-r--r--   0 renaud    (1000) renaud    (1000)    17989 2024-05-16 13:12:27.000000 dash_pydantic_form-0.1.3/dash_pydantic_form/model_form.py
+-rw-r--r--   0 renaud    (1000) renaud    (1000)     8201 2024-05-14 12:37:15.000000 dash_pydantic_form-0.1.3/dash_pydantic_form/pydantic_form_scripts.js
+-rw-r--r--   0 renaud    (1000) renaud    (1000)     2102 2024-05-14 12:37:15.000000 dash_pydantic_form-0.1.3/dash_pydantic_form/pydantic_form_styles.css
+-rw-r--r--   0 renaud    (1000) renaud    (1000)     8782 2024-05-16 13:12:27.000000 dash_pydantic_form-0.1.3/dash_pydantic_form/utils.py
+drwxr-xr-x   0 renaud    (1000) renaud    (1000)        0 2024-05-16 13:13:21.093371 dash_pydantic_form-0.1.3/dash_pydantic_form.egg-info/
+-rw-r--r--   0 renaud    (1000) renaud    (1000)     8673 2024-05-16 13:13:21.000000 dash_pydantic_form-0.1.3/dash_pydantic_form.egg-info/PKG-INFO
+-rw-r--r--   0 renaud    (1000) renaud    (1000)     1072 2024-05-16 13:13:21.000000 dash_pydantic_form-0.1.3/dash_pydantic_form.egg-info/SOURCES.txt
+-rw-r--r--   0 renaud    (1000) renaud    (1000)        1 2024-05-16 13:13:21.000000 dash_pydantic_form-0.1.3/dash_pydantic_form.egg-info/dependency_links.txt
+-rw-r--r--   0 renaud    (1000) renaud    (1000)      116 2024-05-16 13:13:21.000000 dash_pydantic_form-0.1.3/dash_pydantic_form.egg-info/requires.txt
+-rw-r--r--   0 renaud    (1000) renaud    (1000)       36 2024-05-16 13:13:21.000000 dash_pydantic_form-0.1.3/dash_pydantic_form.egg-info/top_level.txt
+drwxr-xr-x   0 renaud    (1000) renaud    (1000)        0 2024-05-16 13:13:21.093371 dash_pydantic_form-0.1.3/docs/
+-rw-r--r--   0 renaud    (1000) renaud    (1000)       87 2024-05-12 09:51:29.000000 dash_pydantic_form-0.1.3/docs/_config.yml
+-rw-r--r--   0 renaud    (1000) renaud    (1000)       21 2024-05-12 09:47:47.000000 dash_pydantic_form-0.1.3/docs/index.md
+drwxr-xr-x   0 renaud    (1000) renaud    (1000)        0 2024-05-16 13:13:21.093371 dash_pydantic_form-0.1.3/images/
+-rwxr-xr-x   0 renaud    (1000) renaud    (1000)    47789 2024-05-13 11:27:16.000000 dash_pydantic_form-0.1.3/images/conditionnally-visible-field.gif
+-rwxr-xr-x   0 renaud    (1000) renaud    (1000)    55763 2024-05-16 13:12:27.000000 dash_pydantic_form-0.1.3/images/discriminated-union.gif
+-rwxr-xr-x   0 renaud    (1000) renaud    (1000)    15290 2024-05-13 11:17:07.000000 dash_pydantic_form-0.1.3/images/editable-table.png
+-rwxr-xr-x   0 renaud    (1000) renaud    (1000)     4506 2024-05-13 11:00:42.000000 dash_pydantic_form-0.1.3/images/form-sections.png
+-rwxr-xr-x   0 renaud    (1000) renaud    (1000)    12406 2024-05-13 11:12:08.000000 dash_pydantic_form-0.1.3/images/model-list.png
+-rwxr-xr-x   0 renaud    (1000) renaud    (1000)     8028 2024-05-13 11:00:37.000000 dash_pydantic_form-0.1.3/images/nested-model.png
+-rwxr-xr-x   0 renaud    (1000) renaud    (1000)    16764 2024-05-13 10:21:46.000000 dash_pydantic_form-0.1.3/images/simple-form.png
+-rw-r--r--   0 renaud    (1000) renaud    (1000)     1186 2024-05-16 13:00:11.000000 dash_pydantic_form-0.1.3/pyproject.toml
+-rw-r--r--   0 renaud    (1000) renaud    (1000)       38 2024-05-16 13:13:21.093371 dash_pydantic_form-0.1.3/setup.cfg
+-rw-r--r--   0 renaud    (1000) renaud    (1000)     7517 2024-05-16 13:12:27.000000 dash_pydantic_form-0.1.3/usage.py
```

### Comparing `dash_pydantic_form-0.1.2/.gitignore` & `dash_pydantic_form-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.2/.vscode/launch.json` & `dash_pydantic_form-0.1.3/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.2/PKG-INFO` & `dash_pydantic_form-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-pydantic-form
-Version: 0.1.2
+Version: 0.1.3
 Summary: Create Dash forms from pydantic objects
 Author-email: Renaud Lainé <renaud.laine@enea-consulting.com>
 License: Copyright ENEA Australia Pty Ltd - All Rights Reserved. Proprietary and confidential
 Project-URL: Source, https://github.com/RenaudLN/dash-pydantic-form
 Requires-Python: <3.13,>=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: dash
@@ -278,10 +278,50 @@
 * "array_contains"
 * "array_contains_any"
 
 NOTE: The field in the 3-tuples is a ":" separated path relative to the current field's level of nesting. If you need to reference a field from a parent or the root use the special values `_parent_` or `_root_`.
 
 E.g., `visible=("_root_:first_name", "==", "Bob")`
 
+## Discriminated unions
+
+Dash pydantic form supports Pydantic [discriminated unions with str discriminator](https://docs.pydantic.dev/latest/concepts/unions/#discriminated-unions-with-str-discriminators)
+
+```py
+class HomeOffice(BaseModel):
+    """Home office model."""
+
+    type: Literal["home_office"]
+    has_workstation: bool = Field(title="Has workstation", description="Does the employee have a suitable workstation")
+
+
+class WorkOffice(BaseModel):
+    """Work office model."""
+
+    type: Literal["work_office"]
+    commute_time: int = Field(title="Commute time", description="Commute time in minutes", ge=0)
+
+class Employee(BaseModel):
+    name: str = Field(title="Name")
+    work_location: HomeOffice | WorkOffice | None = Field("Work location", default=None, discriminator="type")
+
+form = ModelForm(
+    Employee,
+    aio_id="employees",
+    form_id="new_employee",
+    fields_repr={
+        "work_location": {
+            "fields_repr": {
+                "type": fields.RadioItems(
+                    options_labels={"home_office": "Home", "work_office": "Work"}
+                )
+            },
+        },
+    }
+)
+```
+
+![Discriminated union](images/discriminated-union.gif)
+
 ## Creating custom fields
 
 *To be written*
```

### Comparing `dash_pydantic_form-0.1.2/README.md` & `dash_pydantic_form-0.1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -258,10 +258,50 @@
 * "array_contains"
 * "array_contains_any"
 
 NOTE: The field in the 3-tuples is a ":" separated path relative to the current field's level of nesting. If you need to reference a field from a parent or the root use the special values `_parent_` or `_root_`.
 
 E.g., `visible=("_root_:first_name", "==", "Bob")`
 
+## Discriminated unions
+
+Dash pydantic form supports Pydantic [discriminated unions with str discriminator](https://docs.pydantic.dev/latest/concepts/unions/#discriminated-unions-with-str-discriminators)
+
+```py
+class HomeOffice(BaseModel):
+    """Home office model."""
+
+    type: Literal["home_office"]
+    has_workstation: bool = Field(title="Has workstation", description="Does the employee have a suitable workstation")
+
+
+class WorkOffice(BaseModel):
+    """Work office model."""
+
+    type: Literal["work_office"]
+    commute_time: int = Field(title="Commute time", description="Commute time in minutes", ge=0)
+
+class Employee(BaseModel):
+    name: str = Field(title="Name")
+    work_location: HomeOffice | WorkOffice | None = Field("Work location", default=None, discriminator="type")
+
+form = ModelForm(
+    Employee,
+    aio_id="employees",
+    form_id="new_employee",
+    fields_repr={
+        "work_location": {
+            "fields_repr": {
+                "type": fields.RadioItems(
+                    options_labels={"home_office": "Home", "work_office": "Work"}
+                )
+            },
+        },
+    }
+)
+```
+
+![Discriminated union](images/discriminated-union.gif)
+
 ## Creating custom fields
 
 *To be written*
```

### Comparing `dash_pydantic_form-0.1.2/dash_pydantic_form/__init__.py` & `dash_pydantic_form-0.1.3/dash_pydantic_form/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.2/dash_pydantic_form/fields/__init__.py` & `dash_pydantic_form-0.1.3/dash_pydantic_form/fields/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-import logging
 from datetime import date, time
 from enum import Enum
-from types import UnionType
-from typing import Literal, Union, get_args, get_origin
+from typing import Literal, get_origin
 
 from pydantic import BaseModel
 from pydantic.fields import FieldInfo
 
-from dash_pydantic_form.utils import get_non_null_annotation, is_subclass
+from dash_pydantic_form.utils import Type, get_non_null_annotation, is_subclass
 
 from . import all_fields as fields
 from .base_fields import BaseField, VisibilityFilter
 
 DEFAULT_FIELDS_REPR: dict[type, BaseField] = {
     str: fields.Text,
     int: fields.Number,
@@ -26,30 +24,24 @@
 }
 DEFAULT_REPR = fields.Json
 
 
 def get_default_repr(field_info: FieldInfo, **kwargs) -> BaseField:
     """Get default field representation."""
     ann = get_non_null_annotation(field_info.annotation)
+    type_ = Type.classify(field_info.annotation, discriminator=field_info.discriminator)
 
-    # Test for model list
-    if get_origin(ann) == list and is_subclass(get_args(ann)[0], BaseModel):
-        return fields.ModelList(**kwargs)
+    if type_ == Type.SCALAR:
+        return DEFAULT_FIELDS_REPR.get(ann, DEFAULT_REPR)(**kwargs)
+
+    if type_ in [Type.MODEL, Type.DISCRIMINATED_MODEL]:
+        return fields.Model(**kwargs)
 
-    # Test for discriminated model
-    if field_info.discriminator:
-        if get_origin(ann) in [Union, UnionType] and all(is_subclass(x, BaseModel) for x in get_args(ann)):
-            # return fields.DiscriminatedModel(**kwargs)
-            logging.info("Discriminated model fields not yet supported.")
-        else:
-            logging.info(f"Discriminator not supported for {field_info.annotation}")
-
-    # Test for simple types
-    if ann in DEFAULT_FIELDS_REPR:
-        return DEFAULT_FIELDS_REPR[ann](**kwargs)
+    if type_ == Type.MODEL_LIST:
+        return fields.ModelList(**kwargs)
 
     # Test for type origin
     origin = get_origin(ann)
     if origin in DEFAULT_FIELDS_REPR:
         return DEFAULT_FIELDS_REPR[origin](**kwargs)
 
     # Test for subclass
```

### Comparing `dash_pydantic_form-0.1.2/dash_pydantic_form/fields/all_fields.py` & `dash_pydantic_form-0.1.3/dash_pydantic_form/fields/all_fields.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.2/dash_pydantic_form/fields/base_fields.py` & `dash_pydantic_form-0.1.3/dash_pydantic_form/fields/base_fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,21 @@
 from dash import ALL, MATCH, ClientsideFunction, Input, Output, State, clientside_callback, html
 from dash.development.base_component import Component
 from pydantic import BaseModel, Field, field_serializer, field_validator
 from pydantic.fields import FieldInfo
 from pydantic.types import annotated_types
 
 from dash_pydantic_form import ids as common_ids
-from dash_pydantic_form.utils import SEP, get_all_subclasses, get_fullpath, get_model_value, get_non_null_annotation
+from dash_pydantic_form.utils import (
+    SEP,
+    get_all_subclasses,
+    get_fullpath,
+    get_model_value,
+    get_non_null_annotation,
+)
 
 CHECKED_COMPONENTS = [
     dmc.Checkbox,
     dmc.Switch,
 ]
 NO_LABEL_COMPONENTS = [
     dmc.SegmentedControl,
@@ -503,15 +509,15 @@
         data = self._get_data_list_recursive(non_null_annotation, item=item, field=field, parent=parent, **kwargs)
         return data
 
     def _get_data_list_recursive(self, non_null_annotation: type, **_kwargs) -> list:
         """Get list of possible values from annotation recursively."""
         data = []
         # if the annotation is a union of types, recursively calls this function on each type.
-        if get_origin(non_null_annotation) is Union or get_origin(non_null_annotation) is UnionType:
+        if get_origin(non_null_annotation) in [Union, UnionType]:
             data.extend(
                 sum(
                     [self._get_data_list_recursive(sub_annotation) for sub_annotation in get_args(non_null_annotation)],
                     [],
                 )
             )
 
@@ -594,14 +600,19 @@
 
 
 class SegmentedControlField(SelectField):
     """Segmented control field."""
 
     base_component = dmc.SegmentedControl
 
+    def model_post_init(self, _context):
+        """Add default style."""
+        super().model_post_init(_context)
+        self.input_kwargs.setdefault("style", {"alignSelf": "baseline"})
+
 
 clientside_callback(
     ClientsideFunction(namespace="pydf", function_name="updateFieldVisibility"),
     Output(BaseField.ids.visibility_wrapper(MATCH, MATCH, MATCH, MATCH, ALL), "style"),
     Input(common_ids.value_field(MATCH, MATCH, MATCH, MATCH, ALL), "value"),
     Input(common_ids.checked_field(MATCH, MATCH, MATCH, MATCH, ALL), "checked"),
     State(BaseField.ids.visibility_wrapper(MATCH, MATCH, MATCH, MATCH, ALL), "style"),
```

### Comparing `dash_pydantic_form-0.1.2/dash_pydantic_form/fields/editabletable_field.py` & `dash_pydantic_form-0.1.3/dash_pydantic_form/fields/editabletable_field.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.2/dash_pydantic_form/fields/markdown_field.py` & `dash_pydantic_form-0.1.3/dash_pydantic_form/fields/markdown_field.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.2/dash_pydantic_form/fields/model_field.py` & `dash_pydantic_form-0.1.3/dash_pydantic_form/fields/model_field.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import dash_mantine_components as dmc
 from dash import (
     MATCH,
     ClientsideFunction,
     Input,
     Output,
     clientside_callback,
+    html,
 )
 from dash.development.base_component import Component
 from dash_iconify import DashIconify
 from pydantic import BaseModel, Field
 from pydantic.fields import FieldInfo
 
 from dash_pydantic_form import ids as common_ids
@@ -32,15 +33,15 @@
     render_type: Literal["accordion", "modal"] = Field(
         default="accordion", description="How to render the model field, one of 'accordion', 'modal'."
     )
     fields_repr: dict[str, dict | BaseField] | None = Field(
         default=None,
         description="Fields representation, mapping between field name and field representation for the nested fields.",
     )
-    sections: Sections = Field(default=None, description="Sub-form sections.")
+    sections: Sections | None = Field(default=None, description="Sub-form sections.")
 
     full_width = True
 
     def model_post_init(self, _context):
         """Model post init."""
         super().model_post_init(_context)
         if self.fields_repr is None:
@@ -143,24 +144,29 @@
             dmc.AccordionItem(
                 value="item",
                 children=[
                     dmc.AccordionControl(dmc.Text(title)),
                     dmc.AccordionPanel(
                         [
                             *([dmc.Text(description, size="xs", c="dimmed")] * bool(title) * bool(description)),
-                            ModelForm(
-                                item=item,
-                                aio_id=aio_id,
-                                form_id=form_id,
-                                path=get_fullpath(parent, field),
-                                fields_repr=self.fields_repr,
-                                sections=self.sections,
+                            html.Div(
+                                ModelForm(
+                                    item=item,
+                                    aio_id=aio_id,
+                                    form_id=form_id,
+                                    path=get_fullpath(parent, field),
+                                    fields_repr=self.fields_repr,
+                                    sections=self.sections,
+                                    discriminator=field_info.discriminator,
+                                ),
+                                id=self.ids.form_wrapper(
+                                    aio_id, form_id, field_info.discriminator or "", parent=get_fullpath(parent, field)
+                                ),
                             ),
                         ],
-                        id=self.ids.form_wrapper(aio_id, form_id, field, parent=parent),
                     ),
                 ],
             ),
             value="item",
             styles={
                 "control": {"padding": "0.5rem"},
                 "label": {"padding": 0},
```

### Comparing `dash_pydantic_form-0.1.2/dash_pydantic_form/fields/model_list_field.py` & `dash_pydantic_form-0.1.3/dash_pydantic_form/fields/model_list_field.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.2/dash_pydantic_form/form_section.py` & `dash_pydantic_form-0.1.3/dash_pydantic_form/form_section.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.2/dash_pydantic_form/ids.py` & `dash_pydantic_form-0.1.3/dash_pydantic_form/ids.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.2/dash_pydantic_form/model_form.py` & `dash_pydantic_form-0.1.3/dash_pydantic_form/model_form.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,50 @@
 import contextlib
 import itertools
+from copy import deepcopy
 from functools import partial
-from typing import TYPE_CHECKING, Literal, Union
+from typing import Literal, Union
 
 import dash_mantine_components as dmc
-from dash import ALL, MATCH, ClientsideFunction, Input, Output, State, clientside_callback, dcc, html
+from dash import (
+    ALL,
+    MATCH,
+    ClientsideFunction,
+    Input,
+    Output,
+    State,
+    callback,
+    clientside_callback,
+    ctx,
+    dcc,
+    html,
+)
 from dash.development.base_component import Component
 from dash_iconify import DashIconify
 from pydantic import BaseModel
 
 from . import ids as common_ids
+from .fields import BaseField, fields
 from .form_section import Sections
-from .utils import deep_merge, get_subitem_cls
-
-if TYPE_CHECKING:
-    from .fields import BaseField
+from .utils import (
+    SEP,
+    Type,
+    deep_merge,
+    get_fullpath,
+    get_model_cls,
+    get_subitem,
+    get_subitem_cls,
+    handle_discriminated,
+    model_construct_recursive,
+)
 
 
-def form_base_id(part: str, aio_id: str, form_id: str):
+def form_base_id(part: str, aio_id: str, form_id: str, parent: str = ""):
     """Form parts id."""
-    return {"part": part, "aio_id": aio_id, "form_id": form_id}
+    return {"part": part, "aio_id": aio_id, "form_id": form_id, "parent": parent}
 
 
 Children_ = Component | str | int | float
 Children = Children_ | list[Children_]
 SectionRender = Literal["accordion", "tabs", "steps"]
 Position = Literal["top", "bottom", "none"]
 
@@ -49,62 +70,85 @@
     sections: Sections | None
         List of form sections (optional). See :class:`dash_pydantic_form.form_section.Sections`.
     """
 
     class ids:
         """Model form ids."""
 
-        main = partial(form_base_id, "_pydantic-form-main")
-        accordion = partial(form_base_id, "_pydantic-form-accordion")
-        tabs = partial(form_base_id, "_pydantic-form-tabs")
-        steps = partial(form_base_id, "_pydantic-form-steps")
-        steps_save = partial(form_base_id, "_pydantic-form-steps-save")
-        steps_next = partial(form_base_id, "_pydantic-form-steps-next")
-        steps_previous = partial(form_base_id, "_pydantic-form-steps-previous")
-        steps_nsteps = partial(form_base_id, "_pydantic-form-steps-nsteps")
+        main = partial(form_base_id, "_pydf-main")
+        accordion = partial(form_base_id, "_pydf-accordion")
+        tabs = partial(form_base_id, "_pydf-tabs")
+        steps = partial(form_base_id, "_pydf-steps")
+        steps_save = partial(form_base_id, "_pydf-steps-save")
+        steps_next = partial(form_base_id, "_pydf-steps-next")
+        steps_previous = partial(form_base_id, "_pydf-steps-previous")
+        steps_nsteps = partial(form_base_id, "_pydf-steps-nsteps")
+        model_store = partial(form_base_id, "_pydf-model-store")
+        form_specs_store = partial(form_base_id, "_pydf-form-specs-store")
 
-    def __init__(  # noqa: PLR0912, PLR0913
+    def __init__(  # noqa: PLR0912, PLR0913, PLR0915
         self,
         item: BaseModel | type[BaseModel],
         aio_id: str,
         form_id: str,
         path: str = "",
         fields_repr: dict[str, Union["BaseField", dict]] | None = None,
         sections: Sections | None = None,
+        discriminator: str | None = None,
     ) -> None:
         from dash_pydantic_form.fields import get_default_repr
 
         with contextlib.suppress(Exception):
             if issubclass(item, BaseModel):
                 item = item.model_construct()
 
         fields_repr = fields_repr or {}
         field_inputs = {}
         subitem_cls = get_subitem_cls(item.__class__, path)
+
+        # Handle type unions
+        disc_vals = None
+        discriminator_value = None
+        if Type.classify(subitem_cls, discriminator) == Type.DISCRIMINATED_MODEL:
+            subitem = get_subitem(item, path)
+            discriminator_value = None if subitem is None else getattr(subitem, discriminator, None)
+            subitem_cls, disc_vals = handle_discriminated(
+                item.__class__, path, subitem_cls, discriminator, discriminator_value
+            )
+
+        more_kwargs = {}
         for field_name, field_info in subitem_cls.model_fields.items():
             if sections and field_name in sections.excluded_fields:
                 continue
+            # If discriminating field, ensure all discriminator values are shown
+            # Also add required metadata for discriminator callback
+            if disc_vals and field_name == discriminator:
+                field_info = deepcopy(field_info)  # noqa: PLW2901
+                field_info.annotation = Literal[disc_vals]
+                more_kwargs |= {"n_cols": 4, "field_id_meta": "discriminator"}
             if field_name in fields_repr:
                 if isinstance(fields_repr[field_name], dict):
-                    field_repr = get_default_repr(field_info, **fields_repr[field_name])
+                    field_repr = get_default_repr(field_info, **fields_repr[field_name], **more_kwargs)
                 else:
                     field_repr = fields_repr[field_name]
+                    for key, val in more_kwargs.items():
+                        setattr(field_repr, key, val)
             else:
-                field_repr = get_default_repr(field_info)
+                field_repr = get_default_repr(field_info, **more_kwargs)
 
             field_inputs[field_name] = field_repr.render(
                 item=item,
                 aio_id=aio_id,
                 form_id=form_id,
                 field=field_name,
                 parent=path,
                 field_info=field_info,
             )
 
-        if not sections:
+        if not sections or not any([f for f in field_inputs if f in s.fields] for s in sections.sections if s.fields):
             children = [self.grid(list(field_inputs.values()))]
         else:
             fields_not_in_sections = set(field_inputs) - set(
                 itertools.chain.from_iterable(s.fields for s in sections.sections)
             )
 
             if sections.render == "accordion":
@@ -115,14 +159,15 @@
                 render_function = self.render_steps_sections
             else:
                 raise ValueError("Only 'accordion', 'tabs' and 'steps' are supported for `section_render_type`.")
 
             sections_render = render_function(
                 aio_id=aio_id,
                 form_id=form_id,
+                path=path,
                 field_inputs=field_inputs,
                 sections=sections,
                 **sections.render_kwargs,
             )
 
             if sections.remaining_fields_position == "none" or not fields_not_in_sections:
                 children = sections_render
@@ -131,30 +176,55 @@
                     self.grid([v for k, v in field_inputs.items() if k in fields_not_in_sections], mb="sm")
                 ] + sections_render
             else:
                 children = sections_render + [
                     self.grid([v for k, v in field_inputs.items() if k in fields_not_in_sections], mb="sm")
                 ]
 
+        fields_repr_dicts = (
+            {
+                field_name: (
+                    get_default_repr(subitem_cls.model_fields[field_name], **field_repr)
+                    if isinstance(field_repr, dict)
+                    else field_repr
+                ).to_dict()
+                for field_name, field_repr in fields_repr.items()
+            }
+            if fields_repr
+            else None
+        )
         if not path:
             children.append(dcc.Store(id=self.ids.main(aio_id, form_id)))
+            children.append(dcc.Store(data=str(item.__class__), id=self.ids.model_store(aio_id, form_id)))
+
+        if discriminator:
+            children.append(
+                dcc.Store(
+                    data={
+                        "sections": sections.model_dump(mode="json") if sections else None,
+                        "fields_repr": fields_repr_dicts,
+                    },
+                    id=self.ids.form_specs_store(aio_id, form_id, path),
+                )
+            )
 
         super().__init__(children=children)
 
     @classmethod
     def grid(cls, children: Children, **kwargs):
         """Create the responsive grid for a field."""
         return dmc.SimpleGrid(children, cols={"base": 1, "sm": 4}, className="pydantic-form-grid", **kwargs)
 
     @classmethod
-    def render_accordion_sections(
+    def render_accordion_sections(  # noqa: PLR0913
         cls,
         *,
         aio_id: str,
         form_id: str,
+        path: str,
         field_inputs: dict[str, Component],
         sections: Sections,
         **_kwargs,
     ):
         """Render the form sections as accordion."""
         return [
             dmc.Accordion(
@@ -189,25 +259,26 @@
                     "content": {
                         "display": "flex",
                         "flexDirection": "column",
                         "gap": "0.375rem",
                         "padding": "0.125rem 0.5rem 0.5rem",
                     },
                 },
-                id=cls.ids.accordion(aio_id, form_id),
+                id=cls.ids.accordion(aio_id, form_id, path),
                 multiple=True,
             )
         ]
 
     @classmethod
-    def render_tabs_sections(
+    def render_tabs_sections(  # noqa: PLR0913
         cls,
         *,
         aio_id: str,
         form_id: str,
+        path: str,
         field_inputs: dict[str, Component],
         sections: Sections,
         **_kwargs,
     ):
         """Render the form sections as tabs."""
         value = sections.sections[0].name
         for section in sections.sections:
@@ -238,24 +309,25 @@
                         for section in sections.sections
                     ],
                 ],
                 value=value,
                 styles={
                     "panel": {"padding": "1rem 0.5rem 0"},
                 },
-                id=cls.ids.tabs(aio_id, form_id),
+                id=cls.ids.tabs(aio_id, form_id, path),
             )
         ]
 
     @classmethod
     def render_steps_sections(  # noqa: PLR0913
         cls,
         *,
         aio_id: str,
         form_id: str,
+        path: str,
         field_inputs: dict[str, Component],
         sections: Sections,
         additional_steps: list = None,
         **kwargs,
     ):
         """Render the form sections as steps."""
         stepper_styles = deep_merge(
@@ -266,15 +338,15 @@
                 "step": {"cursor": "pointer"},
                 "stepBody": {"padding-top": "0.6875rem"},
                 "stepCompletedIcon": {"&>svg": {"width": 12}},
             },
             kwargs.get("styles", {}),
         )
         stepper = dmc.Stepper(
-            id=cls.ids.steps(aio_id, form_id),
+            id=cls.ids.steps(aio_id, form_id, path),
             active=0,
             orientation="vertical",
             size="sm",
             styles=stepper_styles,
             children=[
                 dmc.StepperStep(
                     label=section.name,
@@ -290,61 +362,102 @@
             html.Div(
                 [
                     stepper,
                     dmc.Group(
                         [
                             dmc.Button(
                                 "Back",
-                                id=cls.ids.steps_previous(aio_id, form_id),
+                                id=cls.ids.steps_previous(aio_id, form_id, path),
                                 disabled=True,
                                 size="compact-md",
                                 leftSection=DashIconify(icon="carbon:arrow-left", height=16),
                             ),
                             dmc.Button(
                                 "Next",
-                                id=cls.ids.steps_next(aio_id, form_id),
+                                id=cls.ids.steps_next(aio_id, form_id, path),
                                 size="compact-md",
                                 rightSection=DashIconify(icon="carbon:arrow-right", height=16),
                             ),
                         ],
                         style={
                             "position": "absolute",
                             "top": f"calc({70 * (len(sections.sections) + len(additional_steps or []))}px + 1rem)",
                         },
                     ),
-                    dcc.Store(data=len(sections.sections), id=cls.ids.steps_nsteps(aio_id, form_id)),
+                    dcc.Store(data=len(sections.sections), id=cls.ids.steps_nsteps(aio_id, form_id, path)),
                 ],
                 style={"position": "relative"},
             )
         ]
 
 
 clientside_callback(
     ClientsideFunction(namespace="pydf", function_name="stepsPreviousNext"),
-    Output(ModelForm.ids.steps(MATCH, MATCH), "active"),
-    Input(ModelForm.ids.steps_previous(MATCH, MATCH), "n_clicks"),
-    Input(ModelForm.ids.steps_next(MATCH, MATCH), "n_clicks"),
-    State(ModelForm.ids.steps(MATCH, MATCH), "active"),
-    State(ModelForm.ids.steps_nsteps(MATCH, MATCH), "data"),
+    Output(ModelForm.ids.steps(MATCH, MATCH, MATCH), "active"),
+    Input(ModelForm.ids.steps_previous(MATCH, MATCH, MATCH), "n_clicks"),
+    Input(ModelForm.ids.steps_next(MATCH, MATCH, MATCH), "n_clicks"),
+    State(ModelForm.ids.steps(MATCH, MATCH, MATCH), "active"),
+    State(ModelForm.ids.steps_nsteps(MATCH, MATCH, MATCH), "data"),
     prevent_inital_call=True,
 )
 
 clientside_callback(
     ClientsideFunction(namespace="pydf", function_name="stepsDisable"),
-    Output(ModelForm.ids.steps_previous(MATCH, MATCH), "disabled"),
-    Output(ModelForm.ids.steps_next(MATCH, MATCH), "disabled"),
-    Input(ModelForm.ids.steps(MATCH, MATCH), "active"),
-    State(ModelForm.ids.steps_nsteps(MATCH, MATCH), "data"),
+    Output(ModelForm.ids.steps_previous(MATCH, MATCH, MATCH), "disabled"),
+    Output(ModelForm.ids.steps_next(MATCH, MATCH, MATCH), "disabled"),
+    Input(ModelForm.ids.steps(MATCH, MATCH, MATCH), "active"),
+    State(ModelForm.ids.steps_nsteps(MATCH, MATCH, MATCH), "data"),
 )
 
 clientside_callback(
     ClientsideFunction(namespace="pydf", function_name="stepsClickListener"),
-    Output(ModelForm.ids.steps(MATCH, MATCH), "id"),
-    Input(ModelForm.ids.steps(MATCH, MATCH), "id"),
+    Output(ModelForm.ids.steps(MATCH, MATCH, MATCH), "id"),
+    Input(ModelForm.ids.steps(MATCH, MATCH, MATCH), "id"),
 )
 
 clientside_callback(
     ClientsideFunction(namespace="pydf", function_name="getValues"),
     Output(ModelForm.ids.main(MATCH, MATCH), "data"),
-    Input(common_ids.value_field(MATCH, MATCH, ALL, ALL), "value"),
-    Input(common_ids.checked_field(MATCH, MATCH, ALL, ALL), "checked"),
+    Input(common_ids.value_field(MATCH, MATCH, ALL, ALL, ALL), "value"),
+    Input(common_ids.checked_field(MATCH, MATCH, ALL, ALL, ALL), "checked"),
+)
+
+
+@callback(
+    Output(fields.Model.ids.form_wrapper(MATCH, MATCH, MATCH, MATCH), "children"),
+    Input(common_ids.value_field(MATCH, MATCH, MATCH, MATCH, "discriminator"), "value"),
+    State(ModelForm.ids.main(MATCH, MATCH), "data"),
+    State(ModelForm.ids.model_store(MATCH, MATCH), "data"),
+    State(ModelForm.ids.form_specs_store(MATCH, MATCH, MATCH), "data"),
+    prevent_initial_call=True,
 )
+def update_discriminated(val, form_data: dict, model_name: str, form_specs: dict):
+    """Update discriminated form."""
+    path: str = get_fullpath(ctx.triggered_id["parent"], ctx.triggered_id["field"])
+    parts = path.split(SEP)
+    # Update the form data with the new value as it wouldn't have been updated yet
+    pointer = form_data
+    for i, part in enumerate(parts):
+        if i == len(parts) - 1:
+            pointer[part] = val
+        pointer = pointer[int(part) if part.isdigit() else part]
+
+    # Create an instance of the model sith the form data using model_construct_recursive
+    # to build it out as much as possible without failing on validation
+    model_cls = get_model_cls(model_name)
+    item = model_construct_recursive(form_data, model_cls)
+
+    # Retrieve fields-repr and sections from the stored data
+    fields_repr: dict[str, BaseField] = {
+        k: BaseField.from_dict(v) for k, v in (form_specs["fields_repr"] or {}).items()
+    }
+    sections = Sections(**form_specs["sections"]) if form_specs["sections"] else None
+
+    return ModelForm(
+        item=item,
+        aio_id=ctx.triggered_id["aio_id"],
+        form_id=ctx.triggered_id["form_id"],
+        path=ctx.triggered_id["parent"],
+        discriminator=ctx.triggered_id["field"],
+        sections=sections,
+        fields_repr=fields_repr,
+    )
```

### Comparing `dash_pydantic_form-0.1.2/dash_pydantic_form/pydantic_form_scripts.js` & `dash_pydantic_form-0.1.3/dash_pydantic_form/pydantic_form_scripts.js`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.2/dash_pydantic_form/pydantic_form_styles.css` & `dash_pydantic_form-0.1.3/dash_pydantic_form/pydantic_form_styles.css`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.2/dash_pydantic_form/utils.py` & `dash_pydantic_form-0.1.3/dash_pydantic_form/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,60 @@
 from copy import deepcopy
+from datetime import date, time
+from enum import Enum
+from numbers import Number
 from types import UnionType
-from typing import Any, Union, get_args, get_origin
+from typing import Any, Literal, Union, get_args, get_origin
 
-from pydantic import BaseModel
+from pydantic import BaseModel, create_model
 from pydantic_core import PydanticUndefined
 
 SEP = ":"
 
 
+class Type(Enum):
+    """Types of fields."""
+
+    SCALAR = "scalar"
+    MODEL = "model"
+    DISCRIMINATED_MODEL = "discriminated_model"
+    MODEL_LIST = "model_list"
+    SCALAR_LIST = "scalar_list"
+    UNKNOWN = "unknown"
+
+    @classmethod
+    def classify(cls, annotation: type, discriminator: str | None = None, depth: int = 0) -> bool:  # noqa: PLR0911
+        """Classify a value as a field type."""
+        annotation = get_non_null_annotation(annotation)
+
+        if is_subclass(annotation, str | Number | bool | date | time):
+            return cls.SCALAR
+
+        if is_subclass(annotation, BaseModel):
+            return cls.MODEL
+
+        if get_origin(annotation) in [Union, UnionType]:
+            if discriminator and all(is_subclass(x, BaseModel) for x in get_args(annotation)):
+                return cls.DISCRIMINATED_MODEL
+            if all(is_subclass(x, str | Number) for x in get_args(annotation)):
+                return cls.SCALAR
+
+        if get_origin(annotation) == list and not depth:
+            ann_args = get_args(annotation)
+            if not ann_args:
+                return cls.SCALAR_LIST
+            args_type = Type.classify(ann_args[0], depth=1)
+            if args_type == Type.SCALAR:
+                return cls.SCALAR_LIST
+            if args_type == Type.MODEL:
+                return cls.MODEL_LIST
+
+        return cls.UNKNOWN
+
+
 def deep_merge(dict1: dict, dict2: dict) -> dict:
     """Deep merge two dictionaries, the second input is given priority."""
     dict_final = deepcopy(dict1)
     for key, val in dict2.items():
         if isinstance(val, dict):
             dict_final[key] = deep_merge(dict_final.get(key, {}), val)
         else:
@@ -59,15 +102,18 @@
     allow_default: bool
         Allow to return the default value, when the object has been created with model_construct.
     """
     try:
         return get_subitem(item, parent)[field]
     except:
         if allow_default:
-            field_info = get_subitem_cls(item, parent).model_fields[field]
+            subitem_cls = get_subitem_cls(item.__class__, parent)
+            if not is_subclass(subitem_cls, BaseModel):
+                return None
+            field_info = subitem_cls.model_fields[field]
             if field_info.default is not PydanticUndefined:
                 return field_info.default
             if field_info.default_factory:
                 return field_info.default_factory()
             return None
         raise
 
@@ -104,29 +150,57 @@
 
     path = parent.split(SEP)
 
     first_part = path[0]
     second_part = None
 
     if len(path) == 1:
-        return get_non_null_annotation(model.model_fields[first_part].annotation)
+        ann = get_non_null_annotation(model.model_fields[first_part].annotation)
+        return ann
 
     second_part = path[1]
     if isinstance(second_part, str) and second_part.isdigit():
         second_part = int(second_part)
 
     first_annotation = get_non_null_annotation(model.model_fields[first_part].annotation)
     if get_non_null_annotation(get_origin(first_annotation)) == list and isinstance(second_part, int):
         return get_subitem_cls(
             get_non_null_annotation(get_args(first_annotation)[0]),
             SEP.join(path[2:]),
         )
     return get_subitem_cls(first_annotation, SEP.join(path[1:]))
 
 
+def handle_discriminated(model: type[BaseModel], parent: str, annotation: type, disc_field: str, disc_val: Any):
+    """Handle a discriminated model."""
+    all_vals = set()
+    out = None
+    for possible in get_args(annotation):
+        if not get_origin(possible.model_fields[disc_field].annotation) == Literal:
+            raise ValueError("Discriminator must be a Literal")
+
+        vals = get_args(possible.model_fields[disc_field].annotation)
+        all_vals = all_vals.union(vals)
+        if disc_val is not None and disc_val in vals:
+            out = possible
+
+    all_vals = tuple(all_vals)
+
+    if disc_val is None:
+        return create_model(
+            f"{model.__name__}{parent.replace(SEP, ' ').title().replace(' ', '')}Discriminator",
+            **{disc_field: (Literal[tuple(all_vals)], ...)},
+        ), all_vals
+
+    if out is None:
+        raise ValueError(f"Invalid discriminator value: {disc_val}")
+
+    return out, all_vals
+
+
 def get_fullpath(*parts):
     """Creates the full path of a field from its name and parent."""
     return SEP.join([str(p) for p in parts]).strip(SEP)
 
 
 def get_all_subclasses(cls: type):
     """Get all subclasses of a class."""
@@ -146,7 +220,37 @@
 
 def is_subclass(cls: type, base_cls: type) -> bool:
     """Check if a class is a subclass of another class, handling issubclass errors."""
     try:
         return issubclass(cls, base_cls)
     except TypeError:
         return False
+
+
+def model_construct_recursive(data: dict, data_model: type[BaseModel]):
+    """Construct a model recursively."""
+    updated = deepcopy(data)
+    for key, val in data.items():
+        if key not in data_model.model_fields:
+            continue
+
+        field_info = data_model.model_fields[key]
+        ann = get_non_null_annotation(field_info.annotation)
+        type_ = Type.classify(ann, field_info.discriminator)
+        if type_ == Type.MODEL:
+            updated[key] = model_construct_recursive(val, ann)
+        elif type_ == Type.DISCRIMINATED_MODEL and field_info.discriminator in val:
+            disc_val = val[field_info.discriminator]
+            out = None
+            for possible in get_args(ann):
+                if not get_origin(possible.model_fields[field_info.discriminator].annotation) == Literal:
+                    raise ValueError("Discriminator must be a Literal")
+
+                if disc_val in get_args(possible.model_fields[field_info.discriminator].annotation):
+                    out = possible
+                    break
+            if out is not None:
+                updated[key] = model_construct_recursive(val, possible)
+        elif type_ == Type.MODEL_LIST and isinstance(val, list):
+            updated[key] = [model_construct_recursive(vv, get_args(ann)[0]) for vv in val]
+
+    return data_model.model_construct(**updated)
```

### Comparing `dash_pydantic_form-0.1.2/dash_pydantic_form.egg-info/PKG-INFO` & `dash_pydantic_form-0.1.3/dash_pydantic_form.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-pydantic-form
-Version: 0.1.2
+Version: 0.1.3
 Summary: Create Dash forms from pydantic objects
 Author-email: Renaud Lainé <renaud.laine@enea-consulting.com>
 License: Copyright ENEA Australia Pty Ltd - All Rights Reserved. Proprietary and confidential
 Project-URL: Source, https://github.com/RenaudLN/dash-pydantic-form
 Requires-Python: <3.13,>=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: dash
@@ -278,10 +278,50 @@
 * "array_contains"
 * "array_contains_any"
 
 NOTE: The field in the 3-tuples is a ":" separated path relative to the current field's level of nesting. If you need to reference a field from a parent or the root use the special values `_parent_` or `_root_`.
 
 E.g., `visible=("_root_:first_name", "==", "Bob")`
 
+## Discriminated unions
+
+Dash pydantic form supports Pydantic [discriminated unions with str discriminator](https://docs.pydantic.dev/latest/concepts/unions/#discriminated-unions-with-str-discriminators)
+
+```py
+class HomeOffice(BaseModel):
+    """Home office model."""
+
+    type: Literal["home_office"]
+    has_workstation: bool = Field(title="Has workstation", description="Does the employee have a suitable workstation")
+
+
+class WorkOffice(BaseModel):
+    """Work office model."""
+
+    type: Literal["work_office"]
+    commute_time: int = Field(title="Commute time", description="Commute time in minutes", ge=0)
+
+class Employee(BaseModel):
+    name: str = Field(title="Name")
+    work_location: HomeOffice | WorkOffice | None = Field("Work location", default=None, discriminator="type")
+
+form = ModelForm(
+    Employee,
+    aio_id="employees",
+    form_id="new_employee",
+    fields_repr={
+        "work_location": {
+            "fields_repr": {
+                "type": fields.RadioItems(
+                    options_labels={"home_office": "Home", "work_office": "Work"}
+                )
+            },
+        },
+    }
+)
+```
+
+![Discriminated union](images/discriminated-union.gif)
+
 ## Creating custom fields
 
 *To be written*
```

### Comparing `dash_pydantic_form-0.1.2/dash_pydantic_form.egg-info/SOURCES.txt` & `dash_pydantic_form-0.1.3/dash_pydantic_form.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -23,12 +23,13 @@
 dash_pydantic_form/fields/editabletable_field.py
 dash_pydantic_form/fields/markdown_field.py
 dash_pydantic_form/fields/model_field.py
 dash_pydantic_form/fields/model_list_field.py
 docs/_config.yml
 docs/index.md
 images/conditionnally-visible-field.gif
+images/discriminated-union.gif
 images/editable-table.png
 images/form-sections.png
 images/model-list.png
 images/nested-model.png
 images/simple-form.png
```

### Comparing `dash_pydantic_form-0.1.2/images/conditionnally-visible-field.gif` & `dash_pydantic_form-0.1.3/images/conditionnally-visible-field.gif`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.2/images/editable-table.png` & `dash_pydantic_form-0.1.3/images/editable-table.png`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.2/images/form-sections.png` & `dash_pydantic_form-0.1.3/images/form-sections.png`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.2/images/model-list.png` & `dash_pydantic_form-0.1.3/images/model-list.png`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.2/images/nested-model.png` & `dash_pydantic_form-0.1.3/images/nested-model.png`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.2/images/simple-form.png` & `dash_pydantic_form-0.1.3/images/simple-form.png`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.2/pyproject.toml` & `dash_pydantic_form-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.2/usage.py` & `dash_pydantic_form-0.1.3/usage.py`

 * *Files 18% similar despite different names*

```diff
@@ -52,27 +52,42 @@
 
     name: str = Field(title="Name", description="Name of the pet")
     species: Species = Field(title="Species", description="Species of the pet")
     dob: date | None = Field(title="Date of birth", description="Date of birth of the pet", default=None)
     alive: bool = Field(title="Alive", description="Is the pet alive", default=True)
 
 
+class HomeOffice(BaseModel):
+    """Home office model."""
+
+    type: Literal["home_office"]
+    has_workstation: bool = Field(title="Has workstation", description="Does the employee have a suitable workstation")
+
+
+class WorkOffice(BaseModel):
+    """Work office model."""
+
+    type: Literal["work_office"]
+    commute_time: int = Field(title="Commute time", description="Commute time in minutes", ge=0)
+
+
 class Employee(BaseModel):
     """Employee model."""
 
     name: str = Field(title="Name", description="Name of the employee")
     age: int = Field(title="Age", description="Age of the employee, starting from their birth")
     mini_bio: str | None = Field(title="Mini bio", description="Short bio of the employee", default=None)
     joined: date = Field(title="Joined", description="Date when the employee joined the company")
     office: Office = Field(title="Office", description="Office of the employee")
     metadata: Metadata | None = Field(title="Employee metadata", default=None)
+    location: HomeOffice | WorkOffice | None = Field(title="Work location", default=None, discriminator="type")
     pets: list[Pet] = Field(title="Pets", description="Employee pets", default_factory=list)
 
 
-bob = Employee(name="Bob", age=30, joined="2020-01-01", office="au", pets=[{"name": "Rex", "species": "dog"}])
+bob = Employee(name="Bob", age=30, joined="2020-01-01", office="au", pet={"species": "cat"})
 
 
 AIO_ID = "home"
 FORM_ID = "Bob"
 
 app.layout = dmc.MantineProvider(
     # defaultColorScheme="dark",
@@ -80,14 +95,15 @@
         [
             dmc.AppShellMain(
                 dmc.Container(
                     [
                         dmc.Title("Dash Pydantic form", mb="1rem", order=3),
                         ModelForm(
                             Employee,
+                            # bob,
                             AIO_ID,
                             FORM_ID,
                             fields_repr={
                                 "mini_bio": fields.Markdown(),
                                 "office": fields.RadioItems(
                                     options_labels={"au": "Australia", "fr": "France"},
                                 ),
@@ -107,19 +123,30 @@
                                 },
                                 "pets": fields.EditableTable(
                                     fields_repr={
                                         "species": {"options_labels": {"dog": "Dog", "cat": "Cat"}},
                                     },
                                     table_height=200,
                                 ),
+                                "location": {
+                                    "fields_repr": {
+                                        "type": fields.RadioItems(
+                                            options_labels={"home_office": "Home", "work_office": "Work"}
+                                        )
+                                    },
+                                },
                             },
                             sections=Sections(
                                 sections=[
                                     FormSection(name="General", fields=["name", "age", "mini_bio"], default_open=True),
-                                    FormSection(name="HR", fields=["office", "joined", "metadata"], default_open=True),
+                                    FormSection(
+                                        name="HR",
+                                        fields=["office", "joined", "location", "metadata"],
+                                        default_open=True,
+                                    ),
                                     FormSection(name="Other", fields=["pets"], default_open=True),
                                 ],
                                 render="accordion",
                             ),
                         ),
                     ],
                     pt="1rem",
```

