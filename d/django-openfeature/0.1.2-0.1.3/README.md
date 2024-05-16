# Comparing `tmp/django-openfeature-0.1.2.tar.gz` & `tmp/django_openfeature-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-openfeature-0.1.2.tar", last modified: Wed Mar 20 06:05:27 2024, max compression
+gzip compressed data, was "django_openfeature-0.1.3.tar", last modified: Thu May 16 05:05:26 2024, max compression
```

## Comparing `django-openfeature-0.1.2.tar` & `django_openfeature-0.1.3.tar`

### file list

```diff
@@ -1,33 +1,36 @@
-drwxr-xr-x   0 federicobond   (501) staff       (20)        0 2024-03-20 06:05:27.085648 django-openfeature-0.1.2/
--rw-r--r--   0 federicobond   (501) staff       (20)     1074 2024-03-19 03:41:11.000000 django-openfeature-0.1.2/LICENSE
--rw-r--r--   0 federicobond   (501) staff       (20)       87 2024-03-19 07:27:46.000000 django-openfeature-0.1.2/MANIFEST.in
--rw-r--r--   0 federicobond   (501) staff       (20)     7418 2024-03-20 06:05:27.085413 django-openfeature-0.1.2/PKG-INFO
--rw-r--r--   0 federicobond   (501) staff       (20)     5315 2024-03-20 01:39:20.000000 django-openfeature-0.1.2/README.md
--rw-r--r--   0 federicobond   (501) staff       (20)     1417 2024-03-20 06:04:58.000000 django-openfeature-0.1.2/pyproject.toml
--rw-r--r--   0 federicobond   (501) staff       (20)       38 2024-03-20 06:05:27.085694 django-openfeature-0.1.2/setup.cfg
--rw-r--r--   0 federicobond   (501) staff       (20)       38 2024-03-19 07:26:59.000000 django-openfeature-0.1.2/setup.py
-drwxr-xr-x   0 federicobond   (501) staff       (20)        0 2024-03-20 06:05:27.080063 django-openfeature-0.1.2/src/
-drwxr-xr-x   0 federicobond   (501) staff       (20)        0 2024-03-20 06:05:27.082540 django-openfeature-0.1.2/src/django_openfeature/
--rw-r--r--   0 federicobond   (501) staff       (20)      988 2024-03-19 07:52:35.000000 django-openfeature-0.1.2/src/django_openfeature/__init__.py
--rw-r--r--   0 federicobond   (501) staff       (20)      889 2024-03-19 03:41:11.000000 django-openfeature-0.1.2/src/django_openfeature/context.py
-drwxr-xr-x   0 federicobond   (501) staff       (20)        0 2024-03-20 06:05:27.083728 django-openfeature-0.1.2/src/django_openfeature/debug_toolbar/
--rw-r--r--   0 federicobond   (501) staff       (20)        0 2024-03-19 03:41:11.000000 django-openfeature-0.1.2/src/django_openfeature/debug_toolbar/__init__.py
--rw-r--r--   0 federicobond   (501) staff       (20)     1678 2024-03-19 06:53:47.000000 django-openfeature-0.1.2/src/django_openfeature/debug_toolbar/panels.py
--rw-r--r--   0 federicobond   (501) staff       (20)     4539 2024-03-19 03:41:11.000000 django-openfeature-0.1.2/src/django_openfeature/provider.py
--rw-r--r--   0 federicobond   (501) staff       (20)      883 2024-03-19 07:52:35.000000 django-openfeature-0.1.2/src/django_openfeature/settings.py
-drwxr-xr-x   0 federicobond   (501) staff       (20)        0 2024-03-20 06:05:27.080259 django-openfeature-0.1.2/src/django_openfeature/templates/
-drwxr-xr-x   0 federicobond   (501) staff       (20)        0 2024-03-20 06:05:27.080308 django-openfeature-0.1.2/src/django_openfeature/templates/debug_toolbar/
-drwxr-xr-x   0 federicobond   (501) staff       (20)        0 2024-03-20 06:05:27.083993 django-openfeature-0.1.2/src/django_openfeature/templates/debug_toolbar/panels/
--rw-r--r--   0 federicobond   (501) staff       (20)     1393 2024-03-19 03:41:11.000000 django-openfeature-0.1.2/src/django_openfeature/templates/debug_toolbar/panels/feature_flags.html
-drwxr-xr-x   0 federicobond   (501) staff       (20)        0 2024-03-20 06:05:27.084410 django-openfeature-0.1.2/src/django_openfeature/templatetags/
--rw-r--r--   0 federicobond   (501) staff       (20)        0 2024-03-19 03:41:11.000000 django-openfeature-0.1.2/src/django_openfeature/templatetags/__init__.py
--rw-r--r--   0 federicobond   (501) staff       (20)     2393 2024-03-20 06:04:15.000000 django-openfeature-0.1.2/src/django_openfeature/templatetags/openfeature.py
--rw-r--r--   0 federicobond   (501) staff       (20)      610 2024-03-19 04:55:29.000000 django-openfeature-0.1.2/src/django_openfeature/test.py
-drwxr-xr-x   0 federicobond   (501) staff       (20)        0 2024-03-20 06:05:27.085039 django-openfeature-0.1.2/src/django_openfeature.egg-info/
--rw-r--r--   0 federicobond   (501) staff       (20)     7418 2024-03-20 06:05:27.000000 django-openfeature-0.1.2/src/django_openfeature.egg-info/PKG-INFO
--rw-r--r--   0 federicobond   (501) staff       (20)      734 2024-03-20 06:05:27.000000 django-openfeature-0.1.2/src/django_openfeature.egg-info/SOURCES.txt
--rw-r--r--   0 federicobond   (501) staff       (20)        1 2024-03-20 06:05:27.000000 django-openfeature-0.1.2/src/django_openfeature.egg-info/dependency_links.txt
--rw-r--r--   0 federicobond   (501) staff       (20)       73 2024-03-20 06:05:27.000000 django-openfeature-0.1.2/src/django_openfeature.egg-info/requires.txt
--rw-r--r--   0 federicobond   (501) staff       (20)       19 2024-03-20 06:05:27.000000 django-openfeature-0.1.2/src/django_openfeature.egg-info/top_level.txt
-drwxr-xr-x   0 federicobond   (501) staff       (20)        0 2024-03-20 06:05:27.084682 django-openfeature-0.1.2/tests/
--rw-r--r--   0 federicobond   (501) staff       (20)     1427 2024-03-19 07:08:18.000000 django-openfeature-0.1.2/tests/test.py
+drwxr-xr-x   0 federicobond   (501) staff       (20)        0 2024-05-16 05:05:26.322485 django_openfeature-0.1.3/
+-rw-r--r--   0 federicobond   (501) staff       (20)     1074 2024-03-19 03:41:11.000000 django_openfeature-0.1.3/LICENSE
+-rw-r--r--   0 federicobond   (501) staff       (20)       87 2024-03-19 07:27:46.000000 django_openfeature-0.1.3/MANIFEST.in
+-rw-r--r--   0 federicobond   (501) staff       (20)     7588 2024-05-16 05:05:26.322255 django_openfeature-0.1.3/PKG-INFO
+-rw-r--r--   0 federicobond   (501) staff       (20)     5485 2024-03-26 02:22:08.000000 django_openfeature-0.1.3/README.md
+-rw-r--r--   0 federicobond   (501) staff       (20)     1764 2024-05-16 05:04:37.000000 django_openfeature-0.1.3/pyproject.toml
+-rw-r--r--   0 federicobond   (501) staff       (20)       38 2024-05-16 05:05:26.322531 django_openfeature-0.1.3/setup.cfg
+-rw-r--r--   0 federicobond   (501) staff       (20)       38 2024-05-16 04:07:25.000000 django_openfeature-0.1.3/setup.py
+drwxr-xr-x   0 federicobond   (501) staff       (20)        0 2024-05-16 05:05:26.314605 django_openfeature-0.1.3/src/
+drwxr-xr-x   0 federicobond   (501) staff       (20)        0 2024-05-16 05:05:26.317875 django_openfeature-0.1.3/src/django_openfeature/
+-rw-r--r--   0 federicobond   (501) staff       (20)      988 2024-03-19 07:52:35.000000 django_openfeature-0.1.3/src/django_openfeature/__init__.py
+-rw-r--r--   0 federicobond   (501) staff       (20)      952 2024-05-16 04:15:24.000000 django_openfeature-0.1.3/src/django_openfeature/context.py
+drwxr-xr-x   0 federicobond   (501) staff       (20)        0 2024-05-16 05:05:26.319202 django_openfeature-0.1.3/src/django_openfeature/debug_toolbar/
+-rw-r--r--   0 federicobond   (501) staff       (20)        0 2024-03-19 03:41:11.000000 django_openfeature-0.1.3/src/django_openfeature/debug_toolbar/__init__.py
+-rw-r--r--   0 federicobond   (501) staff       (20)     1703 2024-03-27 02:00:18.000000 django_openfeature-0.1.3/src/django_openfeature/debug_toolbar/panels.py
+-rw-r--r--   0 federicobond   (501) staff       (20)     4687 2024-05-16 05:03:26.000000 django_openfeature-0.1.3/src/django_openfeature/provider.py
+-rw-r--r--   0 federicobond   (501) staff       (20)        0 2024-05-16 04:08:51.000000 django_openfeature-0.1.3/src/django_openfeature/py.typed
+-rw-r--r--   0 federicobond   (501) staff       (20)      883 2024-03-19 07:52:35.000000 django_openfeature-0.1.3/src/django_openfeature/settings.py
+drwxr-xr-x   0 federicobond   (501) staff       (20)        0 2024-05-16 05:05:26.314964 django_openfeature-0.1.3/src/django_openfeature/templates/
+drwxr-xr-x   0 federicobond   (501) staff       (20)        0 2024-05-16 05:05:26.315019 django_openfeature-0.1.3/src/django_openfeature/templates/debug_toolbar/
+drwxr-xr-x   0 federicobond   (501) staff       (20)        0 2024-05-16 05:05:26.319684 django_openfeature-0.1.3/src/django_openfeature/templates/debug_toolbar/panels/
+-rw-r--r--   0 federicobond   (501) staff       (20)     1393 2024-03-19 03:41:11.000000 django_openfeature-0.1.3/src/django_openfeature/templates/debug_toolbar/panels/feature_flags.html
+drwxr-xr-x   0 federicobond   (501) staff       (20)        0 2024-05-16 05:05:26.320118 django_openfeature-0.1.3/src/django_openfeature/templatetags/
+-rw-r--r--   0 federicobond   (501) staff       (20)        0 2024-03-19 03:41:11.000000 django_openfeature-0.1.3/src/django_openfeature/templatetags/__init__.py
+-rw-r--r--   0 federicobond   (501) staff       (20)     2391 2024-05-16 04:20:16.000000 django_openfeature-0.1.3/src/django_openfeature/templatetags/openfeature.py
+-rw-r--r--   0 federicobond   (501) staff       (20)      694 2024-05-16 04:16:56.000000 django_openfeature-0.1.3/src/django_openfeature/test.py
+drwxr-xr-x   0 federicobond   (501) staff       (20)        0 2024-05-16 05:05:26.321881 django_openfeature-0.1.3/src/django_openfeature.egg-info/
+-rw-r--r--   0 federicobond   (501) staff       (20)     7588 2024-05-16 05:05:26.000000 django_openfeature-0.1.3/src/django_openfeature.egg-info/PKG-INFO
+-rw-r--r--   0 federicobond   (501) staff       (20)      833 2024-05-16 05:05:26.000000 django_openfeature-0.1.3/src/django_openfeature.egg-info/SOURCES.txt
+-rw-r--r--   0 federicobond   (501) staff       (20)        1 2024-05-16 05:05:26.000000 django_openfeature-0.1.3/src/django_openfeature.egg-info/dependency_links.txt
+-rw-r--r--   0 federicobond   (501) staff       (20)       73 2024-05-16 05:05:26.000000 django_openfeature-0.1.3/src/django_openfeature.egg-info/requires.txt
+-rw-r--r--   0 federicobond   (501) staff       (20)       19 2024-05-16 05:05:26.000000 django_openfeature-0.1.3/src/django_openfeature.egg-info/top_level.txt
+drwxr-xr-x   0 federicobond   (501) staff       (20)        0 2024-05-16 05:05:26.321475 django_openfeature-0.1.3/tests/
+-rw-r--r--   0 federicobond   (501) staff       (20)     1529 2024-03-24 13:43:31.000000 django_openfeature-0.1.3/tests/test_debug_toolbar.py
+-rw-r--r--   0 federicobond   (501) staff       (20)     1721 2024-03-24 12:56:40.000000 django_openfeature-0.1.3/tests/test_feature.py
+-rw-r--r--   0 federicobond   (501) staff       (20)     1442 2024-03-24 12:29:48.000000 django_openfeature-0.1.3/tests/test_override_feature.py
```

### Comparing `django-openfeature-0.1.2/LICENSE` & `django_openfeature-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-openfeature-0.1.2/PKG-INFO` & `django_openfeature-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-openfeature
-Version: 0.1.2
+Version: 0.1.3
 Summary: OpenFeature integration for Django
 Author-email: Federico Bond <federicobond@gmail.com>
 License: MIT License
         
         Copyright 2024 Federico Bond
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -39,14 +39,21 @@
 ![release](https://img.shields.io/pypi/v/django-openfeature)
 ![python versions](https://img.shields.io/pypi/pyversions/django-openfeature)
 
 > ⚠️ Caution: this repository is a work-in-progress. ⚠️
 
 Django OpenFeature is a set of utilities to use OpenFeature in your Django applications.
 
+## Features
+
+ * Django Debug Toolbar integration
+ * Templatetags for flag evaluation
+ * Automatic evaluation context from request
+ * Flag override mechanism for testing
+
 ## Installation
 
 ```
 pip install django-openfeature
 ```
 
 Add `django_openfeature` to your `INSTALLED_APPS` setting.
```

### Comparing `django-openfeature-0.1.2/README.md` & `django_openfeature-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,21 @@
 ![release](https://img.shields.io/pypi/v/django-openfeature)
 ![python versions](https://img.shields.io/pypi/pyversions/django-openfeature)
 
 > ⚠️ Caution: this repository is a work-in-progress. ⚠️
 
 Django OpenFeature is a set of utilities to use OpenFeature in your Django applications.
 
+## Features
+
+ * Django Debug Toolbar integration
+ * Templatetags for flag evaluation
+ * Automatic evaluation context from request
+ * Flag override mechanism for testing
+
 ## Installation
 
 ```
 pip install django-openfeature
 ```
 
 Add `django_openfeature` to your `INSTALLED_APPS` setting.
```

### Comparing `django-openfeature-0.1.2/pyproject.toml` & `django_openfeature-0.1.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "django-openfeature"
-version = "0.1.2"
+version = "0.1.3"
 description = "OpenFeature integration for Django"
 readme = "README.md"
 authors = [{ name = "Federico Bond", email = "federicobond@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: MIT License",
@@ -30,14 +30,32 @@
 [project.urls]
 Homepage = "https://github.com/federicobond/django-openfeature"
 
 [build-system]
 requires = ['setuptools>=40.8.0']
 build-backend = 'setuptools.build_meta'
 
+[tool.setuptools.package-data]
+"django_openfeature" = ["py.typed"]
+
+[tool.setuptools.packages.find]
+where = ["src"]
+
+[tool.hatch.envs.default]
+dependencies = [
+    "django-debug-toolbar"
+]
+
+[tool.hatch.envs.default.scripts]
+test = "django-admin test"
+
+[tool.hatch.envs.default.env-vars]
+DJANGO_SETTINGS_MODULE = "tests.settings"
+PYTHONPATH = "."
+
 [tool.ruff]
 target-version = "py38"
 
 [tool.ruff.lint]
 select = [
     "A",
     "B",
```

### Comparing `django-openfeature-0.1.2/src/django_openfeature/__init__.py` & `django_openfeature-0.1.3/src/django_openfeature/__init__.py`

 * *Files identical despite different names*

### Comparing `django-openfeature-0.1.2/src/django_openfeature/context.py` & `django_openfeature-0.1.3/src/django_openfeature/context.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 
 
 class OpenFeatureContext:
     targeting_key = "id"
     targeting_key_anonymous = "unknown"
     user_attributes = ("username", "email")
 
-    def get_context(self, request):
+    def get_context(self, request) -> EvaluationContext:
         user = request.user
         if not user or user.is_anonymous:
             return EvaluationContext(self.targeting_key_anonymous)
         return self.get_user_context(user)
 
-    def get_user_context(self, user):
+    def get_user_context(self, user) -> EvaluationContext:
         attributes = {}
         for attr in self.user_attributes:
             if not hasattr(user, attr):
                 raise ValueError(f"User model does not have attribute: {attr}")
             attributes[attr] = getattr(user, attr)
         targeting_key = str(getattr(user, self.targeting_key))
         return EvaluationContext(targeting_key, attributes)
 
-    def __call__(self, request):
+    def __call__(self, request) -> EvaluationContext:
         return self.get_context(request)
```

### Comparing `django-openfeature-0.1.2/src/django_openfeature/debug_toolbar/panels.py` & `django_openfeature-0.1.3/src/django_openfeature/debug_toolbar/panels.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import List
+
 from debug_toolbar.panels import Panel
 from django.utils.translation import gettext_lazy as _
 from django.utils.translation import ngettext
 from openfeature.api import add_hooks, get_provider_metadata
 from openfeature.flag_evaluation import FlagEvaluationDetails
 from openfeature.hook import Hook, HookContext
 
@@ -13,15 +15,15 @@
         self.evaluations = []
 
     def after(
         self, hook_context: HookContext, details: FlagEvaluationDetails, hints: dict
     ):
         self.evaluations.append(details)
 
-    def extract_evaluations(self) -> list[FlagEvaluationDetails]:
+    def extract_evaluations(self) -> List[FlagEvaluationDetails]:
         evaluations = self.evaluations
         self.evaluations = []
         return evaluations
 
 
 hook = DebugToolbarHook()
 add_hooks([hook])
```

### Comparing `django-openfeature-0.1.2/src/django_openfeature/provider.py` & `django_openfeature-0.1.3/src/django_openfeature/provider.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,125 +1,129 @@
 from collections import ChainMap
 from typing import Any, Dict, List, Optional, Union
 
 from openfeature.evaluation_context import EvaluationContext
 from openfeature.exception import TypeMismatchError
 from openfeature.flag_evaluation import FlagResolutionDetails, Reason
 from openfeature.hook import Hook
+from openfeature.provider import FeatureProvider
 from openfeature.provider.metadata import Metadata
 from openfeature.provider.no_op_provider import NoOpProvider
 from openfeature.provider.provider import AbstractProvider
 
 
 class DjangoTestProvider(AbstractProvider):
-    def __init__(self):
-        self.chained = NoOpProvider()
-        self.overrides = ChainMap()
+    _chained: FeatureProvider
+    _overrides: ChainMap
+
+    def __init__(self) -> None:
+        self._chained = NoOpProvider()
+        self._overrides = ChainMap()
 
     def get_metadata(self) -> Metadata:
         return Metadata(name="Django Test Provider")
 
     def get_provider_hooks(self) -> List[Hook]:
         return []
 
-    def push_overrides(self, overrides: Dict[str, Any]):
-        self.overrides.maps.insert(0, overrides)
+    def push_overrides(self, overrides: Dict[str, Any]) -> None:
+        self._overrides.maps.insert(0, overrides)
 
-    def pop_overrides(self):
-        self.overrides.maps.pop(0)
+    def pop_overrides(self) -> None:
+        self._overrides.maps.pop(0)
 
     def resolve_boolean_details(
         self,
         flag_key: str,
         default_value: bool,
         evaluation_context: Optional[EvaluationContext] = None,
     ) -> FlagResolutionDetails[bool]:
-        if flag_key in self.overrides:
-            value = self.overrides[flag_key]
+        if flag_key in self._overrides:
+            value = self._overrides[flag_key]
             if not isinstance(value, bool):
                 raise TypeMismatchError(f"Expected type bool but got {type(value)}")
             return FlagResolutionDetails(
                 value=value,
                 reason=Reason.STATIC,
                 variant="Overridden for test",
             )
-        return self.chained.resolve_boolean_details(
+        return self._chained.resolve_boolean_details(
             flag_key, default_value, evaluation_context
         )
 
     def resolve_string_details(
         self,
         flag_key: str,
         default_value: str,
         evaluation_context: Optional[EvaluationContext] = None,
     ) -> FlagResolutionDetails[str]:
-        if flag_key in self.overrides:
-            value = self.overrides[flag_key]
+        if flag_key in self._overrides:
+            value = self._overrides[flag_key]
             if not isinstance(value, str):
                 raise TypeMismatchError(f"Expected type str but got {type(value)}")
             return FlagResolutionDetails(
                 value=value,
                 reason=Reason.STATIC,
                 variant="Overridden for test",
             )
-        return self.chained.resolve_string_details(
+        return self._chained.resolve_string_details(
             flag_key, default_value, evaluation_context
         )
 
     def resolve_integer_details(
         self,
         flag_key: str,
         default_value: int,
         evaluation_context: Optional[EvaluationContext] = None,
     ) -> FlagResolutionDetails[int]:
-        if flag_key in self.overrides:
-            value = self.overrides[flag_key]
+        if flag_key in self._overrides:
+            value = self._overrides[flag_key]
             if not isinstance(value, int):
                 raise TypeMismatchError(f"Expected type int but got {type(value)}")
             return FlagResolutionDetails(
                 value=value,
                 reason=Reason.STATIC,
                 variant="Overridden for test",
             )
-        return self.chained.resolve_integer_details(
+        return self._chained.resolve_integer_details(
             flag_key, default_value, evaluation_context
         )
 
     def resolve_float_details(
         self,
         flag_key: str,
         default_value: float,
         evaluation_context: Optional[EvaluationContext] = None,
     ) -> FlagResolutionDetails[float]:
-        if flag_key in self.overrides:
-            value = self.overrides[flag_key]
+        if flag_key in self._overrides:
+            value = self._overrides[flag_key]
             if not isinstance(value, float):
                 raise TypeMismatchError(f"Expected type float but got {type(value)}")
             return FlagResolutionDetails(
                 value=value,
                 reason=Reason.STATIC,
                 variant="Overridden for test",
             )
-        return self.chained.resolve_float_details(
+        return self._chained.resolve_float_details(
             flag_key, default_value, evaluation_context
         )
 
     def resolve_object_details(
         self,
         flag_key: str,
         default_value: Union[dict, list],
         evaluation_context: Optional[EvaluationContext] = None,
     ) -> FlagResolutionDetails[Union[dict, list]]:
-        if flag_key in self.overrides:
-            value = self.overrides[flag_key]
+        if flag_key in self._overrides:
+            value = self._overrides[flag_key]
             if not isinstance(value, (dict, list)):
                 raise TypeMismatchError(
                     f"Expected type dict or list but got {type(value)}"
                 )
             return FlagResolutionDetails(
                 value=value,
                 reason=Reason.STATIC,
                 variant="Overridden for test",
             )
-        return self.chained.resolve_object_details(
+        return self._chained.resolve_object_details(
             flag_key, default_value, evaluation_context
         )
```

### Comparing `django-openfeature-0.1.2/src/django_openfeature/settings.py` & `django_openfeature-0.1.3/src/django_openfeature/settings.py`

 * *Files identical despite different names*

### Comparing `django-openfeature-0.1.2/src/django_openfeature/templates/debug_toolbar/panels/feature_flags.html` & `django_openfeature-0.1.3/src/django_openfeature/templates/debug_toolbar/panels/feature_flags.html`

 * *Files identical despite different names*

### Comparing `django-openfeature-0.1.2/src/django_openfeature/templatetags/openfeature.py` & `django_openfeature-0.1.3/src/django_openfeature/templatetags/openfeature.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
 
 class IfFeatureNode(Node):
     def __init__(self, conditions_nodelists):
         self.conditions_nodelists = conditions_nodelists
 
     def __repr__(self):
-        return "<%s>" % self.__class__.__name__
+        return f"<{self.__class__.__name__}>"
 
     def __iter__(self):
         for _, nodelist in self.conditions_nodelists:
             yield from nodelist
 
     @property
     def nodelist(self):
```

### Comparing `django-openfeature-0.1.2/src/django_openfeature/test.py` & `django_openfeature-0.1.3/src/django_openfeature/test.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from contextlib import contextmanager
+from typing import Dict, List, Union
 
 from openfeature import api
 
 from django_openfeature.provider import DjangoTestProvider
 
 __all__ = ["override_feature"]
 
 
 @contextmanager
-def override_feature(name, value):
+def override_feature(name: str, value: Union[bool, str, int, float, Dict, List]):
     # NOTE: using undocumented client property to access the provider
     provider = api.get_client().provider
     if not isinstance(provider, DjangoTestProvider):
         raise ValueError(
             "The override_feature decorator requires a DjangoTestProvider to be set."
         )
     provider.push_overrides({name: value})
```

### Comparing `django-openfeature-0.1.2/src/django_openfeature.egg-info/PKG-INFO` & `django_openfeature-0.1.3/src/django_openfeature.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-openfeature
-Version: 0.1.2
+Version: 0.1.3
 Summary: OpenFeature integration for Django
 Author-email: Federico Bond <federicobond@gmail.com>
 License: MIT License
         
         Copyright 2024 Federico Bond
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -39,14 +39,21 @@
 ![release](https://img.shields.io/pypi/v/django-openfeature)
 ![python versions](https://img.shields.io/pypi/pyversions/django-openfeature)
 
 > ⚠️ Caution: this repository is a work-in-progress. ⚠️
 
 Django OpenFeature is a set of utilities to use OpenFeature in your Django applications.
 
+## Features
+
+ * Django Debug Toolbar integration
+ * Templatetags for flag evaluation
+ * Automatic evaluation context from request
+ * Flag override mechanism for testing
+
 ## Installation
 
 ```
 pip install django-openfeature
 ```
 
 Add `django_openfeature` to your `INSTALLED_APPS` setting.
```

### Comparing `django-openfeature-0.1.2/src/django_openfeature.egg-info/SOURCES.txt` & `django_openfeature-0.1.3/src/django_openfeature.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -2,20 +2,23 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 src/django_openfeature/__init__.py
 src/django_openfeature/context.py
 src/django_openfeature/provider.py
+src/django_openfeature/py.typed
 src/django_openfeature/settings.py
 src/django_openfeature/test.py
 src/django_openfeature.egg-info/PKG-INFO
 src/django_openfeature.egg-info/SOURCES.txt
 src/django_openfeature.egg-info/dependency_links.txt
 src/django_openfeature.egg-info/requires.txt
 src/django_openfeature.egg-info/top_level.txt
 src/django_openfeature/debug_toolbar/__init__.py
 src/django_openfeature/debug_toolbar/panels.py
 src/django_openfeature/templates/debug_toolbar/panels/feature_flags.html
 src/django_openfeature/templatetags/__init__.py
 src/django_openfeature/templatetags/openfeature.py
-tests/test.py
+tests/test_debug_toolbar.py
+tests/test_feature.py
+tests/test_override_feature.py
```

### Comparing `django-openfeature-0.1.2/tests/test.py` & `django_openfeature-0.1.3/tests/test_override_feature.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from django_openfeature.provider import DjangoTestProvider
 from django_openfeature.test import override_feature
 from openfeature.api import get_client, set_provider
 from openfeature.provider.no_op_provider import NoOpProvider
 
 
-class Tests(TestCase):
+class OverrideFeatureTests(TestCase):
     def test_override_feature_requires_django_test_provider(self):
         set_provider(NoOpProvider())
 
         @override_feature("foo", True)
         def function():
             pass
```

