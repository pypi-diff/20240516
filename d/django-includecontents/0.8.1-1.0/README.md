# Comparing `tmp/django_includecontents-0.8.1.tar.gz` & `tmp/django_includecontents-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_includecontents-0.8.1.tar", last modified: Thu May  9 03:01:47 2024, max compression
+gzip compressed data, was "django_includecontents-1.0.tar", last modified: Thu May 16 04:23:13 2024, max compression
```

## Comparing `django_includecontents-0.8.1.tar` & `django_includecontents-1.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     8211 2024-05-09 02:46:25.109484 django_includecontents-0.8.1/README.md
--rw-r--r--   0        0        0        0 2024-04-09 04:42:05.196722 django_includecontents-0.8.1/includecontents/__init__.py
--rw-r--r--   0        0        0     1000 2024-04-19 05:13:37.190112 django_includecontents-0.8.1/includecontents/backend.py
--rw-r--r--   0        0        0     4797 2024-05-09 01:00:11.649227 django_includecontents-0.8.1/includecontents/base.py
--rw-r--r--   0        0        0     1401 2024-04-09 04:42:05.196722 django_includecontents-0.8.1/includecontents/engine.py
--rw-r--r--   0        0        0     1663 2024-04-18 05:37:15.283141 django_includecontents-0.8.1/includecontents/loaders.py
--rw-r--r--   0        0        0        0 2024-04-09 04:42:05.196722 django_includecontents-0.8.1/includecontents/templatetags/__init__.py
--rw-r--r--   0        0        0    17988 2024-05-09 02:59:02.223711 django_includecontents-0.8.1/includecontents/templatetags/includecontents.py
--rw-r--r--   0        0        0     1238 2024-05-09 03:01:47.950565 django_includecontents-0.8.1/pyproject.toml
--rw-r--r--   0        0        0      144 2024-04-19 05:31:17.752738 django_includecontents-0.8.1/tests/settings.py
--rw-r--r--   0        0        0      163 2024-04-21 20:37:00.117665 django_includecontents-0.8.1/tests/templates/components/card-extend.html
--rw-r--r--   0        0        0      168 2024-04-18 05:37:15.283141 django_includecontents-0.8.1/tests/templates/components/card.html
--rw-r--r--   0        0        0       11 2024-05-09 01:17:58.916937 django_includecontents-0.8.1/tests/templates/components/context.html
--rw-r--r--   0        0        0       42 2024-04-21 22:40:07.372787 django_includecontents-0.8.1/tests/templates/components/empty-props.html
--rw-r--r--   0        0        0       35 2024-05-01 04:25:18.356900 django_includecontents-0.8.1/tests/templates/components/escape-props.html
--rw-r--r--   0        0        0        5 2024-05-02 20:42:55.088146 django_includecontents-0.8.1/tests/templates/components/inside/cat.html
--rw-r--r--   0        0        0       97 2024-04-21 23:11:42.498021 django_includecontents-0.8.1/tests/templates/components/nested-attrs.html
--rw-r--r--   0        0        0       81 2024-04-30 04:36:00.000113 django_includecontents-0.8.1/tests/templates/multiline.html
--rw-r--r--   0        0        0      115 2024-04-09 21:50:46.125635 django_includecontents-0.8.1/tests/templates/test_component/attrs.html
--rw-r--r--   0        0        0      162 2024-05-01 00:06:23.461690 django_includecontents-0.8.1/tests/templates/test_component/extend_class.html
--rw-r--r--   0        0        0       73 2024-04-09 21:50:46.125635 django_includecontents-0.8.1/tests/templates/test_component/index.html
--rw-r--r--   0        0        0       34 2024-04-09 21:51:49.385743 django_includecontents-0.8.1/tests/templates/test_component/missing_attr.html
--rw-r--r--   0        0        0       24 2024-04-30 04:36:02.466786 django_includecontents-0.8.1/tests/templates/test_component/missing_closing_tag.html
--rw-r--r--   0        0        0      118 2024-04-09 21:50:46.115635 django_includecontents-0.8.1/tests/templates/test_tag/basic.html
--rw-r--r--   0        0        0      123 2024-05-09 01:24:20.757096 django_includecontents-0.8.1/tests/templates/test_tag/basic_only.html
--rw-r--r--   0        0        0       54 2024-04-21 20:37:00.117665 django_includecontents-0.8.1/tests/templates/test_tag/inner.html
--rw-r--r--   0        0        0      135 2024-04-09 21:50:46.115635 django_includecontents-0.8.1/tests/templates/test_tag/with_attr.html
--rw-r--r--   0        0        0     4399 2024-05-09 02:47:53.176259 django_includecontents-0.8.1/tests/test_component.py
--rw-r--r--   0        0        0      130 2024-04-09 04:52:09.297567 django_includecontents-0.8.1/tests/test_multiline.py
--rw-r--r--   0        0        0     1336 2024-05-09 01:24:42.027110 django_includecontents-0.8.1/tests/test_tag.py
--rw-r--r--   0        0        0     9270 1970-01-01 00:00:00.000000 django_includecontents-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     8552 2024-05-16 04:18:50.873093 django_includecontents-1.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 04:42:05.196722 django_includecontents-1.0/includecontents/__init__.py
+-rw-r--r--   0        0        0     1006 2024-05-16 04:16:45.636328 django_includecontents-1.0/includecontents/django/__init__.py
+-rw-r--r--   0        0        0     4797 2024-05-09 01:00:11.649227 django_includecontents-1.0/includecontents/django/base.py
+-rw-r--r--   0        0        0     1422 2024-05-16 04:21:18.886568 django_includecontents-1.0/includecontents/django/engine.py
+-rw-r--r--   0        0        0     1662 2024-05-16 04:20:38.116526 django_includecontents-1.0/includecontents/django/loaders.py
+-rw-r--r--   0        0        0        0 2024-04-09 04:42:05.196722 django_includecontents-1.0/includecontents/templatetags/__init__.py
+-rw-r--r--   0        0        0    17995 2024-05-16 04:20:38.119860 django_includecontents-1.0/includecontents/templatetags/includecontents.py
+-rw-r--r--   0        0        0     1236 2024-05-16 04:23:13.530027 django_includecontents-1.0/pyproject.toml
+-rw-r--r--   0        0        0      149 2024-05-16 04:16:52.346333 django_includecontents-1.0/tests/settings.py
+-rw-r--r--   0        0        0      163 2024-04-21 20:37:00.117665 django_includecontents-1.0/tests/templates/components/card-extend.html
+-rw-r--r--   0        0        0      168 2024-05-16 04:12:52.522811 django_includecontents-1.0/tests/templates/components/card.html
+-rw-r--r--   0        0        0       11 2024-05-09 01:17:58.916937 django_includecontents-1.0/tests/templates/components/context.html
+-rw-r--r--   0        0        0       42 2024-04-21 22:40:07.372787 django_includecontents-1.0/tests/templates/components/empty-props.html
+-rw-r--r--   0        0        0       35 2024-05-01 04:25:18.356900 django_includecontents-1.0/tests/templates/components/escape-props.html
+-rw-r--r--   0        0        0        5 2024-05-02 20:42:55.088146 django_includecontents-1.0/tests/templates/components/inside/cat.html
+-rw-r--r--   0        0        0       97 2024-04-21 23:11:42.498021 django_includecontents-1.0/tests/templates/components/nested-attrs.html
+-rw-r--r--   0        0        0       81 2024-04-30 04:36:00.000113 django_includecontents-1.0/tests/templates/multiline.html
+-rw-r--r--   0        0        0      115 2024-04-09 21:50:46.125635 django_includecontents-1.0/tests/templates/test_component/attrs.html
+-rw-r--r--   0        0        0      162 2024-05-12 22:22:26.017117 django_includecontents-1.0/tests/templates/test_component/extend_class.html
+-rw-r--r--   0        0        0       73 2024-04-09 21:50:46.125635 django_includecontents-1.0/tests/templates/test_component/index.html
+-rw-r--r--   0        0        0       34 2024-04-09 21:51:49.385743 django_includecontents-1.0/tests/templates/test_component/missing_attr.html
+-rw-r--r--   0        0        0       24 2024-04-30 04:36:02.466786 django_includecontents-1.0/tests/templates/test_component/missing_closing_tag.html
+-rw-r--r--   0        0        0      118 2024-04-09 21:50:46.115635 django_includecontents-1.0/tests/templates/test_tag/basic.html
+-rw-r--r--   0        0        0      123 2024-05-09 01:24:20.757096 django_includecontents-1.0/tests/templates/test_tag/basic_only.html
+-rw-r--r--   0        0        0       54 2024-04-21 20:37:00.117665 django_includecontents-1.0/tests/templates/test_tag/inner.html
+-rw-r--r--   0        0        0      135 2024-04-09 21:50:46.115635 django_includecontents-1.0/tests/templates/test_tag/with_attr.html
+-rw-r--r--   0        0        0     4406 2024-05-16 04:20:38.116526 django_includecontents-1.0/tests/test_component.py
+-rw-r--r--   0        0        0      130 2024-04-09 04:52:09.297567 django_includecontents-1.0/tests/test_multiline.py
+-rw-r--r--   0        0        0     1336 2024-05-09 01:24:42.027110 django_includecontents-1.0/tests/test_tag.py
+-rw-r--r--   0        0        0     9609 1970-01-01 00:00:00.000000 django_includecontents-1.0/PKG-INFO
```

### Comparing `django_includecontents-0.8.1/README.md` & `django_includecontents-1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -37,30 +37,30 @@
 
 ```bash
 pip install django-includecontents
 ```
 
 Either install the custom template engine or just add this app to your `INSTALLED_APPS`.
 
-### Template engine installation
+### Install with template engine
 
-Replace the default `DjangoTemplates` backend in your settings:
+Replace the default `django.template.backends.django.DjangoTemplates` backend in your settings:
 
 ```python
 TEMPLATES = [
     {
-        'BACKEND': 'includecontents.backend.Templates',
+        'BACKEND': 'includecontents.django.DjangoTemplates',
         ...
     },
 ]
 ```
 
 This engine also adds `includecontents` to the built-in tag libraries so there is no need to load it in your templates.
 
-### Basic installation
+### Install without template engine
 
 Alternatively, add this app to your `INSTALLED_APPS` and use `{% load includecontents %}` in your templates:
 
 ```python
 INSTALLED_APPS = [
     ...
     'includecontents',
@@ -285,14 +285,17 @@
         "quoteAttributes": false
       }
     }
   ]
 }
 ```
 
+`quoteAttributes` is set to `false` to avoid quoting HTML attribute values that are template variables (e.g. `title={mytitle}`).
+The workaround to keep the quotes when using the alpineJS `x-data` directive is to simply put a space between the quote and the curly brace: `x-data=" {...} "`.
+
 ### VScode formatting
 
 To use this Prettier formatting within VScode, use the following two extensions:
 
 * [Django](https://marketplace.visualstudio.com/items?itemName=batisteo.vscode-django)
 * [Prettier - Code formatter](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)
```

### Comparing `django_includecontents-0.8.1/includecontents/backend.py` & `django_includecontents-1.0/includecontents/django/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import django.template.backends.django
 from django.conf import settings
 
 from .engine import Engine
 
 
-class Templates(django.template.backends.django.DjangoTemplates):
+class DjangoTemplates(django.template.backends.django.DjangoTemplates):
     def __init__(self, params):
         # Copy parent init code.
         params = params.copy()
         options = params["OPTIONS"].copy()
         options.setdefault("autoescape", True)
         options.setdefault("debug", settings.DEBUG)
         options.setdefault("file_charset", "utf-8")
```

### Comparing `django_includecontents-0.8.1/includecontents/base.py` & `django_includecontents-1.0/includecontents/django/base.py`

 * *Files identical despite different names*

### Comparing `django_includecontents-0.8.1/includecontents/engine.py` & `django_includecontents-1.0/includecontents/django/engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,18 +17,18 @@
         context_processors=None,
         debug=False,
         loaders=None,
         *args,
         **kwargs,
     ):
         if loaders is None:
-            loaders = ["includecontents.loaders.FilesystemLoader"]
+            loaders = ["includecontents.django.loaders.FilesystemLoader"]
             if app_dirs:
-                loaders += ["includecontents.loaders.AppDirectoriesLoader"]
-            loaders = [("includecontents.loaders.CachedLoader", loaders)]
+                loaders += ["includecontents.django.loaders.AppDirectoriesLoader"]
+            loaders = [("includecontents.django.loaders.CachedLoader", loaders)]
         else:
             if app_dirs:
                 raise ImproperlyConfigured(
                     "app_dirs must not be set when loaders is defined."
                 )
         super().__init__(
             dirs=dirs,
```

### Comparing `django_includecontents-0.8.1/includecontents/loaders.py` & `django_includecontents-1.0/includecontents/django/loaders.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import django.template.loaders.filesystem
 from django.template import TemplateDoesNotExist
 
 from .base import Template
 
 
 class CustomTemplateMixin(django.template.loaders.base.Loader):
-
     def get_template(self, template_name, skip=None):
         """
         Call self.get_template_sources() and return a Template object for
         the first template matching template_name. If skip is provided, ignore
         template origins in skip. This is used to avoid recursion during
         template extending.
         """
```

### Comparing `django_includecontents-0.8.1/includecontents/templatetags/includecontents.py` & `django_includecontents-1.0/includecontents/templatetags/includecontents.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from django.template.base import FilterExpression, NodeList, Parser, TokenType
 from django.template.context import Context
 from django.template.loader_tags import construct_relative_path, do_include
 from django.utils.html import conditional_escape
 from django.utils.safestring import mark_safe
 from django.utils.text import smart_split
 
-from includecontents.base import Template
+from includecontents.django.base import Template
 
 register = template.Library()
 
 re_camel_case = re.compile(r"(?<=.)([A-Z])")
 
 
 @register.tag
```

### Comparing `django_includecontents-0.8.1/pyproject.toml` & `django_includecontents-1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "django-includecontents"
-version = "0.8.1"
+version = "1.0"
 description = "Django includecontents component-like tag"
 authors = [
     { name = "Chris Beaven", email = "smileychris@gmail.com" },
 ]
 dependencies = [
     "django",
 ]
```

### Comparing `django_includecontents-0.8.1/tests/test_component.py` & `django_includecontents-1.0/tests/test_component.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 
 import pytest
 from django.template import Context, TemplateSyntaxError
 from django.template.loader import render_to_string
 from django.test import override_settings
 
-from includecontents.base import Template
+from includecontents.django.base import Template
 
 
 def test_basic():
     assert render_to_string("test_component/index.html") == (
         """<main>
   <section class="card">
   <h3 >hello</h3>
```

### Comparing `django_includecontents-0.8.1/tests/test_tag.py` & `django_includecontents-1.0/tests/test_tag.py`

 * *Files identical despite different names*

### Comparing `django_includecontents-0.8.1/PKG-INFO` & `django_includecontents-1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-includecontents
-Version: 0.8.1
+Version: 1.0
 Summary: Django includecontents component-like tag
 Author-Email: Chris Beaven <smileychris@gmail.com>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -64,30 +64,30 @@
 
 ```bash
 pip install django-includecontents
 ```
 
 Either install the custom template engine or just add this app to your `INSTALLED_APPS`.
 
-### Template engine installation
+### Install with template engine
 
-Replace the default `DjangoTemplates` backend in your settings:
+Replace the default `django.template.backends.django.DjangoTemplates` backend in your settings:
 
 ```python
 TEMPLATES = [
     {
-        'BACKEND': 'includecontents.backend.Templates',
+        'BACKEND': 'includecontents.django.DjangoTemplates',
         ...
     },
 ]
 ```
 
 This engine also adds `includecontents` to the built-in tag libraries so there is no need to load it in your templates.
 
-### Basic installation
+### Install without template engine
 
 Alternatively, add this app to your `INSTALLED_APPS` and use `{% load includecontents %}` in your templates:
 
 ```python
 INSTALLED_APPS = [
     ...
     'includecontents',
@@ -312,14 +312,17 @@
         "quoteAttributes": false
       }
     }
   ]
 }
 ```
 
+`quoteAttributes` is set to `false` to avoid quoting HTML attribute values that are template variables (e.g. `title={mytitle}`).
+The workaround to keep the quotes when using the alpineJS `x-data` directive is to simply put a space between the quote and the curly brace: `x-data=" {...} "`.
+
 ### VScode formatting
 
 To use this Prettier formatting within VScode, use the following two extensions:
 
 * [Django](https://marketplace.visualstudio.com/items?itemName=batisteo.vscode-django)
 * [Prettier - Code formatter](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)
```

