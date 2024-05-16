# Comparing `tmp/django_markdowns-0.1.3.tar.gz` & `tmp/django_markdowns-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_markdowns-0.1.3.tar", last modified: Tue Jun 27 14:03:28 2023, max compression
+gzip compressed data, was "django_markdowns-0.2.0.tar", last modified: Thu May 16 14:30:54 2024, max compression
```

## Comparing `django_markdowns-0.1.3.tar` & `django_markdowns-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 jnphilipp  (1000) jnphilipp  (1000)        0 2023-06-27 14:03:28.309754 django_markdowns-0.1.3/
--rw-r--r--   0 jnphilipp  (1000) jnphilipp  (1000)    35149 2021-06-15 15:56:07.000000 django_markdowns-0.1.3/LICENSE
--rw-r--r--   0 jnphilipp  (1000) jnphilipp  (1000)     1665 2023-06-27 14:03:28.309754 django_markdowns-0.1.3/PKG-INFO
--rw-r--r--   0 jnphilipp  (1000) jnphilipp  (1000)      425 2023-06-27 11:30:50.000000 django_markdowns-0.1.3/README.md
-drwxr-xr-x   0 jnphilipp  (1000) jnphilipp  (1000)        0 2023-06-27 14:03:28.309754 django_markdowns-0.1.3/django_markdowns/
--rw-r--r--   0 jnphilipp  (1000) jnphilipp  (1000)     1252 2023-06-27 13:46:36.000000 django_markdowns-0.1.3/django_markdowns/__init__.py
--rw-r--r--   0 jnphilipp  (1000) jnphilipp  (1000)     1077 2023-06-27 11:51:20.000000 django_markdowns-0.1.3/django_markdowns/apps.py
--rw-r--r--   0 jnphilipp  (1000) jnphilipp  (1000)     4814 2023-06-27 11:50:42.000000 django_markdowns-0.1.3/django_markdowns/extensions.py
--rw-r--r--   0 jnphilipp  (1000) jnphilipp  (1000)     1459 2023-06-27 11:51:28.000000 django_markdowns-0.1.3/django_markdowns/settings.py
-drwxr-xr-x   0 jnphilipp  (1000) jnphilipp  (1000)        0 2023-06-27 14:03:28.309754 django_markdowns-0.1.3/django_markdowns/templatetags/
--rw-r--r--   0 jnphilipp  (1000) jnphilipp  (1000)       88 2021-07-07 21:46:06.000000 django_markdowns-0.1.3/django_markdowns/templatetags/__init__.py
--rw-r--r--   0 jnphilipp  (1000) jnphilipp  (1000)     1362 2023-06-27 11:49:01.000000 django_markdowns-0.1.3/django_markdowns/templatetags/markdowns.py
--rw-r--r--   0 jnphilipp  (1000) jnphilipp  (1000)     1327 2023-06-27 13:16:28.000000 django_markdowns-0.1.3/django_markdowns/tests.py
-drwxr-xr-x   0 jnphilipp  (1000) jnphilipp  (1000)        0 2023-06-27 14:03:28.309754 django_markdowns-0.1.3/django_markdowns.egg-info/
--rw-r--r--   0 jnphilipp  (1000) jnphilipp  (1000)     1665 2023-06-27 14:03:28.000000 django_markdowns-0.1.3/django_markdowns.egg-info/PKG-INFO
--rw-r--r--   0 jnphilipp  (1000) jnphilipp  (1000)      473 2023-06-27 14:03:28.000000 django_markdowns-0.1.3/django_markdowns.egg-info/SOURCES.txt
--rw-r--r--   0 jnphilipp  (1000) jnphilipp  (1000)        1 2023-06-27 14:03:28.000000 django_markdowns-0.1.3/django_markdowns.egg-info/dependency_links.txt
--rw-r--r--   0 jnphilipp  (1000) jnphilipp  (1000)       30 2023-06-27 14:03:28.000000 django_markdowns-0.1.3/django_markdowns.egg-info/requires.txt
--rw-r--r--   0 jnphilipp  (1000) jnphilipp  (1000)       17 2023-06-27 14:03:28.000000 django_markdowns-0.1.3/django_markdowns.egg-info/top_level.txt
--rw-r--r--   0 jnphilipp  (1000) jnphilipp  (1000)     1370 2023-06-27 13:45:56.000000 django_markdowns-0.1.3/pyproject.toml
--rw-r--r--   0 jnphilipp  (1000) jnphilipp  (1000)       30 2023-06-27 11:07:41.000000 django_markdowns-0.1.3/requirements.txt
--rw-r--r--   0 jnphilipp  (1000) jnphilipp  (1000)       38 2023-06-27 14:03:28.309754 django_markdowns-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:30:54.929328 django_markdowns-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-16 14:30:35.000000 django_markdowns-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-16 14:30:54.929328 django_markdowns-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-16 14:30:35.000000 django_markdowns-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:30:54.925328 django_markdowns-0.2.0/django_markdowns/
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-16 14:30:35.000000 django_markdowns-0.2.0/django_markdowns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-16 14:30:35.000000 django_markdowns-0.2.0/django_markdowns/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-05-16 14:30:35.000000 django_markdowns-0.2.0/django_markdowns/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-16 14:30:35.000000 django_markdowns-0.2.0/django_markdowns/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:30:54.929328 django_markdowns-0.2.0/django_markdowns/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-16 14:30:35.000000 django_markdowns-0.2.0/django_markdowns/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-16 14:30:35.000000 django_markdowns-0.2.0/django_markdowns/templatetags/markdowns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-16 14:30:35.000000 django_markdowns-0.2.0/django_markdowns/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:30:54.929328 django_markdowns-0.2.0/django_markdowns.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-16 14:30:54.000000 django_markdowns-0.2.0/django_markdowns.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-16 14:30:54.000000 django_markdowns-0.2.0/django_markdowns.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 14:30:54.000000 django_markdowns-0.2.0/django_markdowns.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-16 14:30:54.000000 django_markdowns-0.2.0/django_markdowns.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-16 14:30:54.000000 django_markdowns-0.2.0/django_markdowns.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-16 14:30:35.000000 django_markdowns-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-16 14:30:35.000000 django_markdowns-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 14:30:54.929328 django_markdowns-0.2.0/setup.cfg
```

### Comparing `django_markdowns-0.1.3/LICENSE` & `django_markdowns-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_markdowns-0.1.3/django_markdowns/__init__.py` & `django_markdowns-0.2.0/django_markdowns/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-# -*- coding: utf-8 -*-
-# vim: ft=python fileencoding=utf-8 sts=4 sw=4 et:
-# Copyright (C) 2021-2023 J. Nathanael Philipp (jnphilipp) <nathanael@philipp.land>
+# Copyright (C) 2021-2024 J. Nathanael Philipp (jnphilipp) <nathanael@philipp.land>
 #
 # This file is part of django_markdowns.
 #
 # django_markdowns is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -16,15 +14,15 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with django_markdowns.  If not, see <http://www.gnu.org/licenses/>.
 """Django markdowns."""
 
 
 __author__ = "J. Nathanael Philipp"
-__copyright__ = "Copyright 2021-2023 J. Nathanael Philipp (jnphilipp)"
+__copyright__ = "Copyright 2021-2024 J. Nathanael Philipp (jnphilipp)"
 __license__ = "GPLv3+"
 __maintainer__ = __author__
 __email__ = "nathanael@philipp.land"
 __app_name__ = "django_markdowns"
-__version_info__ = (0, 1, 3)
+__version_info__ = (0, 2, 0)
 __version__ = ".".join(str(e) for e in __version_info__)
 __github__ = "https://github.com/jnphilipp/django-markdowns"
```

### Comparing `django_markdowns-0.1.3/django_markdowns/apps.py` & `django_markdowns-0.2.0/django_markdowns/apps.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-# -*- coding: utf-8 -*-
-# vim: ft=python fileencoding=utf-8 sts=4 sw=4 et:
-# Copyright (C) 2021-2023 J. Nathanael Philipp (jnphilipp) <nathanael@philipp.land>
+# Copyright (C) 2021-2024 J. Nathanael Philipp (jnphilipp) <nathanael@philipp.land>
 #
 # This file is part of django_markdowns.
 #
 # django_markdowns is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `django_markdowns-0.1.3/django_markdowns/extensions.py` & `django_markdowns-0.2.0/django_markdowns/extensions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-# -*- coding: utf-8 -*-
-# vim: ft=python fileencoding=utf-8 sts=4 sw=4 et:
-# Copyright (C) 2021-2023 J. Nathanael Philipp (jnphilipp) <nathanael@philipp.land>
+# Copyright (C) 2021-2024 J. Nathanael Philipp (jnphilipp) <nathanael@philipp.land>
 #
 # This file is part of django_markdowns.
 #
 # django_markdowns is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -26,30 +24,37 @@
 import markdown
 
 from django.conf import settings
 from django.core.exceptions import ValidationError
 from django.core.validators import EmailValidator
 from django.urls import reverse, resolve, Resolver404, NoReverseMatch
 from markdown.inlinepatterns import (
-    ImageInlineProcessor,
-    LinkInlineProcessor,
     IMAGE_LINK_RE,
+    ImageInlineProcessor,
     LINK_RE,
+    LinkInlineProcessor,
+    SimpleTagInlineProcessor,
 )
 from typing import Optional, Tuple
 from urllib.parse import urlparse
 from xml.etree.ElementTree import Element
 
 from .settings import IMG_CLASS
 
 
+SUP_RE = r"()\^(.*?)\^"
+SUB_RE = r"()~(.*?)~"
+
+
 class DjangoLinkInlineProcessor(LinkInlineProcessor):
     """Django link inline processor."""
 
-    def getLink(self, data: str, index: int) -> Tuple[str, Optional[str], int, bool]:
+    def getLink(  # noqa, N802
+        self, data: str, index: int
+    ) -> Tuple[str, Optional[str], int, bool]:
         """Get link, with django specifix stuff."""
         href, title, index, handled = super().getLink(data, index)
         return self._clean_link(href), title, index, handled
 
     def _clean_link(self, href: str) -> str:
         if href == "":
             return ""
@@ -113,25 +118,36 @@
 
         return href
 
 
 class DjangoImageInlineProcessor(DjangoLinkInlineProcessor, ImageInlineProcessor):
     """Django link inline processor."""
 
-    def handleMatch(self, m: re.Match, data: str) -> Tuple[Element, int, int]:
+    def handleMatch(  # noqa, N802
+        self, m: re.Match[str], data: str
+    ) -> tuple[Element | None, int | None, int | None]:
         """Handle Match."""
         el, start, end = super().handleMatch(m, data)
 
-        if IMG_CLASS:
+        if IMG_CLASS and el:
             el.set("class", IMG_CLASS)
         return el, start, end
 
 
+class SubSupExtension(markdown.Extension):
+    """Subscript/superscript markdown extension."""
+
+    def extendMarkdown(self, md: markdown.Markdown):  # noqa, N802
+        """Extend markdown."""
+        md.inlinePatterns.register(SimpleTagInlineProcessor(SUB_RE, "sub"), "sub", 65)
+        md.inlinePatterns.register(SimpleTagInlineProcessor(SUP_RE, "sup"), "sup", 65)
+
+
 class DjangoExtension(markdown.Extension):
     """Django markdown extension."""
 
-    def extendMarkdown(self, md: markdown.Markdown, *args, **kwrags):
+    def extendMarkdown(self, md: markdown.Markdown):  # noqa, N802
         """Extend markdown."""
         md.inlinePatterns.register(DjangoLinkInlineProcessor(LINK_RE, md), "link", 160)
         md.inlinePatterns.register(
             DjangoImageInlineProcessor(IMAGE_LINK_RE, md), "image_link", 150
         )
```

### Comparing `django_markdowns-0.1.3/django_markdowns/settings.py` & `django_markdowns-0.2.0/django_markdowns/settings.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-# -*- coding: utf-8 -*-
-# vim: ft=python fileencoding=utf-8 sts=4 sw=4 et:
-# Copyright (C) 2021-2023 J. Nathanael Philipp (jnphilipp) <nathanael@philipp.land>
+# Copyright (C) 2021-2024 J. Nathanael Philipp (jnphilipp) <nathanael@philipp.land>
 #
 # This file is part of django_markdowns.
 #
 # django_markdowns is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `django_markdowns-0.1.3/django_markdowns/templatetags/markdowns.py` & `django_markdowns-0.2.0/django_markdowns/templatetags/markdowns.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-# -*- coding: utf-8 -*-
-# vim: ft=python fileencoding=utf-8 sts=4 sw=4 et:
-# Copyright (C) 2021-2023 J. Nathanael Philipp (jnphilipp) <nathanael@philipp.land>
+# Copyright (C) 2021-2024 J. Nathanael Philipp (jnphilipp) <nathanael@philipp.land>
 #
 # This file is part of django_markdowns.
 #
 # django_markdowns is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -20,21 +18,26 @@
 
 import markdown
 
 from django.template import Library
 from django.utils.safestring import mark_safe
 from django.template.defaultfilters import stringfilter
 
-from ..extensions import DjangoExtension
+from ..extensions import DjangoExtension, SubSupExtension
 
 register = Library()
 
 
 @register.filter()
 @stringfilter
 def md(text: str) -> str:
     """Convert markdown to html."""
     return mark_safe(
         markdown.markdown(
-            text, extensions=["markdown.extensions.fenced_code", DjangoExtension()]
+            text,
+            extensions=[
+                "markdown.extensions.fenced_code",
+                DjangoExtension(),
+                SubSupExtension(),
+            ],
         )
     )
```

### Comparing `django_markdowns-0.1.3/django_markdowns/tests.py` & `django_markdowns-0.2.0/django_markdowns/tests.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-# -*- coding: utf-8 -*-
-# vim: ft=python fileencoding=utf-8 sts=4 sw=4 et:
-# Copyright (C) 2021-2023 J. Nathanael Philipp (jnphilipp) <nathanael@philipp.land>
+# Copyright (C) 2021-2024 J. Nathanael Philipp (jnphilipp) <nathanael@philipp.land>
 #
 # This file is part of django_markdowns.
 #
 # django_markdowns is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -21,15 +19,24 @@
 
 from django.test import TestCase
 
 from .templatetags import markdowns
 
 
 class MarkdownsTestCase(TestCase):
+    """Markdown test case."""
+
     def test_templatefilter(self):
+        """Simple test for template filter."""
         html = markdowns.md("This is a simple paragraph.")
         self.assertEqual(html, "<p>This is a simple paragraph.</p>")
 
         html = markdowns.md("* this\n* is\n* a\n* list")
         self.assertEqual(
-            html, "<ul><li>this</li><li>is</li><li>a</li><li>list</li></ul>"
+            html,
+            "<ul>\n<li>this</li>\n<li>is</li>\n<li>a</li>\n<li>list</li>\n</ul>",
+        )
+
+        self.assertEqual(
+            markdowns.md("This is ^superscript^ and ~subscript~."),
+            "<p>This is <sup>superscript</sup> and <sub>subscript</sub>.</p>",
         )
```

### Comparing `django_markdowns-0.1.3/pyproject.toml` & `django_markdowns-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 [build-system]
-requires = ["setuptools>=65.5"]
+requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "django_markdowns"
-version = "0.1.3"
+version = "0.2.0"
 authors = [
     {name = "J. Nathanael Philipp", email = "nathanael@philipp.land"}
 ]
 description="Bring markdown functionality to Django."
 readme = "README.md"
 license = {text = "GPLv3+"}
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: OS Independent",
     "Framework :: Django",
-    "Framework :: Django :: 3.2",
     "Framework :: Django :: 4.1",
     "Framework :: Django :: 4.2",
     "Programming Language :: Python",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dynamic = ["dependencies"]
 keywords = ["django", "markdown"]
@@ -38,7 +35,10 @@
 [project.urls]
 "Homepage" = "http://github.com/jnphilipp/django-markdowns"
 "Bug Tracker" = "http://github.com/jnphilipp/django-markdowns/issues"
 
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
+
+[tool.setuptools.package-data]
+transkribus_rest_api = ["py.typed"]
```

