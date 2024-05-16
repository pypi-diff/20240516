# Comparing `tmp/wagtail_links-2.7.0.tar.gz` & `tmp/wagtail_links-2.8.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_links-2.7.0.tar", max compression
+gzip compressed data, was "wagtail_links-2.8.0b1.tar", max compression
```

## Comparing `wagtail_links-2.7.0.tar` & `wagtail_links-2.8.0b1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      747 2024-02-27 15:04:54.895588 wagtail_links-2.7.0/LICENSE
--rw-r--r--   0        0        0     1746 2024-02-27 15:04:54.895588 wagtail_links-2.7.0/README.rst
--rw-r--r--   0        0        0      652 2024-02-27 15:04:54.896588 wagtail_links-2.7.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-27 15:04:54.921588 wagtail_links-2.7.0/src/wagtail_links/__init__.py
--rw-r--r--   0        0        0      233 2024-02-27 15:04:54.896588 wagtail_links-2.7.0/src/wagtail_links/apps.py
--rw-r--r--   0        0        0     1173 2024-02-27 15:04:54.897589 wagtail_links-2.7.0/src/wagtail_links/fields.py
--rw-r--r--   0        0        0      380 2024-02-27 15:04:54.897589 wagtail_links-2.7.0/src/wagtail_links/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2630 2024-02-27 15:04:54.897589 wagtail_links-2.7.0/src/wagtail_links/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1720 2024-02-27 15:04:54.897589 wagtail_links-2.7.0/src/wagtail_links/migrations/0001_initial.py
--rw-r--r--   0        0        0      855 2024-02-27 15:04:54.897589 wagtail_links-2.7.0/src/wagtail_links/migrations/0002_auto_20170522_1552.py
--rw-r--r--   0        0        0      695 2024-02-27 15:04:54.897589 wagtail_links-2.7.0/src/wagtail_links/migrations/0003_auto_20170522_2015.py
--rw-r--r--   0        0        0     2235 2024-02-27 15:04:54.897589 wagtail_links-2.7.0/src/wagtail_links/migrations/0004_auto_20190411_2102.py
--rw-r--r--   0        0        0     2938 2024-02-27 15:04:54.897589 wagtail_links-2.7.0/src/wagtail_links/migrations/0005_auto_20191203_1908_squashed_0006_auto_20191204_2129.py
--rw-r--r--   0        0        0      595 2024-02-27 15:04:54.897589 wagtail_links-2.7.0/src/wagtail_links/migrations/0006_auto_20200101_1646.py
--rw-r--r--   0        0        0      577 2024-02-27 15:04:54.897589 wagtail_links-2.7.0/src/wagtail_links/migrations/0007_auto_20200101_1658.py
--rw-r--r--   0        0        0        0 2024-02-27 15:04:54.924588 wagtail_links-2.7.0/src/wagtail_links/migrations/__init__.py
--rw-r--r--   0        0        0     4888 2024-02-27 15:04:54.897589 wagtail_links-2.7.0/src/wagtail_links/models.py
--rw-r--r--   0        0        0        0 2024-02-27 15:04:54.924588 wagtail_links-2.7.0/src/wagtail_links/templatetags/__init__.py
--rw-r--r--   0        0        0      565 2024-02-27 15:04:54.897589 wagtail_links-2.7.0/src/wagtail_links/templatetags/wagtail_links.py
--rw-r--r--   0        0        0     3903 2024-02-27 15:04:54.897589 wagtail_links-2.7.0/src/wagtail_links/tests.py
--rw-r--r--   0        0        0     2370 1970-01-01 00:00:00.000000 wagtail_links-2.7.0/PKG-INFO
+-rw-r--r--   0        0        0      744 2024-05-16 15:55:49.042207 wagtail_links-2.8.0b1/LICENSE
+-rw-r--r--   0        0        0     1602 2024-05-16 15:55:49.043207 wagtail_links-2.8.0b1/README.md
+-rw-r--r--   0        0        0      645 2024-05-16 15:55:49.044207 wagtail_links-2.8.0b1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-16 15:55:49.078206 wagtail_links-2.8.0b1/src/wagtail_links/__init__.py
+-rw-r--r--   0        0        0      233 2024-05-16 15:55:49.045207 wagtail_links-2.8.0b1/src/wagtail_links/apps.py
+-rw-r--r--   0        0        0     1173 2024-05-16 15:55:49.045207 wagtail_links-2.8.0b1/src/wagtail_links/fields.py
+-rw-r--r--   0        0        0      380 2024-05-16 15:55:49.045207 wagtail_links-2.8.0b1/src/wagtail_links/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2630 2024-05-16 15:55:49.045207 wagtail_links-2.8.0b1/src/wagtail_links/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1720 2024-05-16 15:55:49.045207 wagtail_links-2.8.0b1/src/wagtail_links/migrations/0001_initial.py
+-rw-r--r--   0        0        0      855 2024-05-16 15:55:49.045207 wagtail_links-2.8.0b1/src/wagtail_links/migrations/0002_auto_20170522_1552.py
+-rw-r--r--   0        0        0      695 2024-05-16 15:55:49.045207 wagtail_links-2.8.0b1/src/wagtail_links/migrations/0003_auto_20170522_2015.py
+-rw-r--r--   0        0        0     2235 2024-05-16 15:55:49.046207 wagtail_links-2.8.0b1/src/wagtail_links/migrations/0004_auto_20190411_2102.py
+-rw-r--r--   0        0        0     2938 2024-05-16 15:55:49.046207 wagtail_links-2.8.0b1/src/wagtail_links/migrations/0005_auto_20191203_1908_squashed_0006_auto_20191204_2129.py
+-rw-r--r--   0        0        0      595 2024-05-16 15:55:49.046207 wagtail_links-2.8.0b1/src/wagtail_links/migrations/0006_auto_20200101_1646.py
+-rw-r--r--   0        0        0      577 2024-05-16 15:55:49.046207 wagtail_links-2.8.0b1/src/wagtail_links/migrations/0007_auto_20200101_1658.py
+-rw-r--r--   0        0        0        0 2024-05-16 15:55:49.080206 wagtail_links-2.8.0b1/src/wagtail_links/migrations/__init__.py
+-rw-r--r--   0        0        0     4888 2024-05-16 15:55:49.046207 wagtail_links-2.8.0b1/src/wagtail_links/models.py
+-rw-r--r--   0        0        0        0 2024-05-16 15:55:49.080206 wagtail_links-2.8.0b1/src/wagtail_links/templatetags/__init__.py
+-rw-r--r--   0        0        0      565 2024-05-16 15:55:49.046207 wagtail_links-2.8.0b1/src/wagtail_links/templatetags/wagtail_links.py
+-rw-r--r--   0        0        0     3903 2024-05-16 15:55:49.046207 wagtail_links-2.8.0b1/src/wagtail_links/tests.py
+-rw-r--r--   0        0        0     2275 1970-01-01 00:00:00.000000 wagtail_links-2.8.0b1/PKG-INFO
```

### Comparing `wagtail_links-2.7.0/LICENSE` & `wagtail_links-2.8.0b1/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ISC License
 
-Copyright (c) 2017 - 2024 thelabnyc
+Copyright (c) 2017 - 2024 thelab
 
 Permission to use, copy, modify, and/or distribute this software for any
 purpose with or without fee is hereby granted, provided that the above
 copyright notice and this permission notice appear in all copies.
 
 THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
 REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY
```

### Comparing `wagtail_links-2.7.0/README.rst` & `wagtail_links-2.8.0b1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,80 +1,71 @@
-=============
-Wagtail Links
-=============
+# wagtail-links
 
-Purpose
-=======
+## Purpose
 
 Wagtail links has two goals:
 
 - Provide a consistent way to refer to links, which may be of different types, so as to reduce decision fatigue
 - Minimize broken links as much as possible.
 
 
 
-Install
-=======
+## Install
 
 Install wagtail-links via Pip.
 
-.. code:: bash
+```sh
+pip install wagtail-links
+```
 
-    pip install wagtail-links
-
-Add ``wagtail_links`` to your Django project's INSTALLED_APPS setting.
+Add `wagtail_links` to your Django project's `INSTALLED_APPS` setting.
 
 Run database migrations.
 
-.. code:: bash
-
-    python manage.py migrate
+```sh
+python manage.py migrate
+```
 
 
-
-Usage
-=====
+## Usage
 
 Add a foreign key to the page you wish to add links to.
 
-.. code:: python
-
-    my_link = models.ForeignKey(
-        'wagtail_links.Link',
-        null=True,
-        blank=True,
-        on_delete=models.SET_NULL,
-        related_name='+'
-    )
+```py
+my_link = models.ForeignKey(
+    'wagtail_links.Link',
+    null=True,
+    blank=True,
+    on_delete=models.SET_NULL,
+    related_name='+'
+)
+```
 
 Neat:
 
-.. image:: admin.png
+![](admin.png)
 
 You may use it like:
 
-.. code:: html
-
-    <a href="{{ self.link.url }}">Link here</a>
-
+```html
+<a href="{{ self.link.url }}">Link here</a>
+```
 
 From a template, you can also load a link by its name:
 
-.. code:: html
+```html
+{% load get_wagtail_link_url from wagtail_links %}
 
-    {% load get_wagtail_link_url from wagtail_links %}
-
-    <a href="{% get_wagtail_link_url 'my-link' %}">Link here</a>
+<a href="{% get_wagtail_link_url 'my-link' %}">Link here</a>
+```
 
 This is useful for global page links, navigation, etc.
 
 
-
-Validation and logging
-======================
+## Validation and logging
 
 The Link model will validate that one and only one field is set.
 It will also disallow invalid Django reverse view names.
 
 If a URL cannot be determined, we'll log the issue as a warning. We won't throw an exception as that would be bad for users. You are responsible for capturing this log warning, perhaps using Sentry.
 
 For example - let's say you make a Django view name called admin:index. This would typically give you `/admin/`. Later the admin application is removed from the program, now this link fails. It will now display "" and generate a warning in your server logs.
```

#### html2text {}

```diff
@@ -1,21 +1,20 @@
-============= Wagtail Links ============= Purpose ======= Wagtail links has two
-goals: - Provide a consistent way to refer to links, which may be of different
-types, so as to reduce decision fatigue - Minimize broken links as much as
-possible. Install ======= Install wagtail-links via Pip. .. code:: bash pip
-install wagtail-links Add ``wagtail_links`` to your Django project's
-INSTALLED_APPS setting. Run database migrations. .. code:: bash python
-manage.py migrate Usage ===== Add a foreign key to the page you wish to add
-links to. .. code:: python my_link = models.ForeignKey( 'wagtail_links.Link',
-null=True, blank=True, on_delete=models.SET_NULL, related_name='+' ) Neat: ..
-image:: admin.png You may use it like: .. code:: html _L_i_n_k_ _h_e_r_e From a
-template, you can also load a link by its name: .. code:: html {% load
-get_wagtail_link_url from wagtail_links %} _L_i_n_k_ _h_e_r_e This is useful for global
-page links, navigation, etc. Validation and logging ====================== The
-Link model will validate that one and only one field is set. It will also
-disallow invalid Django reverse view names. If a URL cannot be determined,
-we'll log the issue as a warning. We won't throw an exception as that would be
-bad for users. You are responsible for capturing this log warning, perhaps
-using Sentry. For example - let's say you make a Django view name called admin:
-index. This would typically give you `/admin/`. Later the admin application is
-removed from the program, now this link fails. It will now display "" and
-generate a warning in your server logs.
+# wagtail-links ## Purpose Wagtail links has two goals: - Provide a consistent
+way to refer to links, which may be of different types, so as to reduce
+decision fatigue - Minimize broken links as much as possible. ## Install
+Install wagtail-links via Pip. ```sh pip install wagtail-links ``` Add
+`wagtail_links` to your Django project's `INSTALLED_APPS` setting. Run database
+migrations. ```sh python manage.py migrate ``` ## Usage Add a foreign key to
+the page you wish to add links to. ```py my_link = models.ForeignKey
+( 'wagtail_links.Link', null=True, blank=True, on_delete=models.SET_NULL,
+related_name='+' ) ``` Neat: ![](admin.png) You may use it like: ```html _L_i_n_k
+_h_e_r_e ``` From a template, you can also load a link by its name: ```html {% load
+get_wagtail_link_url from wagtail_links %} _L_i_n_k_ _h_e_r_e ``` This is useful for
+global page links, navigation, etc. ## Validation and logging The Link model
+will validate that one and only one field is set. It will also disallow invalid
+Django reverse view names. If a URL cannot be determined, we'll log the issue
+as a warning. We won't throw an exception as that would be bad for users. You
+are responsible for capturing this log warning, perhaps using Sentry. For
+example - let's say you make a Django view name called admin:index. This would
+typically give you `/admin/`. Later the admin application is removed from the
+program, now this link fails. It will now display "" and generate a warning in
+your server logs.
```

### Comparing `wagtail_links-2.7.0/pyproject.toml` & `wagtail_links-2.8.0b1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-[build-system]
-requires = [ "poetry-core>=1.0.0",]
-build-backend = "poetry.core.masonry.api"
-
 [tool.poetry]
 name = "wagtail-links"
-version = "2.7.0"
+version = "2.8.0-b1"
 description = "Wagtail links provides a consistent way to refer to links in a wagtail page."
-authors = [ "thelabnyc <thelabdev@thelabnyc.com>",]
-readme = "README.rst"
+authors = ["thelab <thelabdev@thelab.co>"]
+readme = "README.md"
 homepage = "https://gitlab.com/thelabnyc/wagtail-links"
 repository = "https://gitlab.com/thelabnyc/wagtail-links"
 license = "ISC"
 
 [[tool.poetry.packages]]
 include = "wagtail_links"
 from = "src"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-wagtail = ">=5.2,<6.0"
+wagtail = ">=5.2,<6.2"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = ">=3.3.0"
 tox = ">=2.7.0"
+
+[build-system]
+requires = [ "poetry-core>=1.0.0",]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `wagtail_links-2.7.0/src/wagtail_links/fields.py` & `wagtail_links-2.8.0b1/src/wagtail_links/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_links-2.7.0/src/wagtail_links/locale/es/LC_MESSAGES/django.po` & `wagtail_links-2.8.0b1/src/wagtail_links/locale/es/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-09-15 20:05+0000\n"
+"POT-Creation-Date: 2024-02-27 15:05+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -69,52 +69,52 @@
 msgstr ""
 
 #: wagtail_links/models.py:74
 msgid "Name of Django view for reverse lookup"
 msgstr ""
 
 #. Translators: Internal Model Name (singular)
-#: wagtail_links/models.py:97
+#: wagtail_links/models.py:95
 msgid "Link"
 msgstr ""
 
 #. Translators: Internal Model Name (plural)
-#: wagtail_links/models.py:99
+#: wagtail_links/models.py:97
 msgid "Links"
 msgstr ""
 
-#: wagtail_links/models.py:107
+#: wagtail_links/models.py:105
 msgid "No Link URL"
 msgstr ""
 
-#: wagtail_links/models.py:117
+#: wagtail_links/models.py:115
 #, python-format
 msgid "Link[name=%(name)s]: %(url)s"
 msgstr ""
 
-#: wagtail_links/models.py:119
+#: wagtail_links/models.py:117
 #, python-format
 msgid "Link[link_external=%(link_external)s]: %(url)s"
 msgstr ""
 
-#: wagtail_links/models.py:121
+#: wagtail_links/models.py:119
 #, python-format
 msgid "Link[link_relative=%(link_relative)s]: %(url)s"
 msgstr ""
 
-#: wagtail_links/models.py:123
+#: wagtail_links/models.py:121
 #, python-format
 msgid "Link[link_page=%(link_page)s]: %(url)s"
 msgstr ""
 
-#: wagtail_links/models.py:124
+#: wagtail_links/models.py:122
 #, python-format
 msgid "Link[django_view_name=%(django_view_name)s]: %(url)s"
 msgstr ""
 
-#: wagtail_links/models.py:158
+#: wagtail_links/models.py:156
 msgid "You may only use one link type"
 msgstr ""
 
-#: wagtail_links/models.py:160
+#: wagtail_links/models.py:158
 msgid "You must use exactly one link type"
 msgstr ""
```

### Comparing `wagtail_links-2.7.0/src/wagtail_links/migrations/0001_initial.py` & `wagtail_links-2.8.0b1/src/wagtail_links/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_links-2.7.0/src/wagtail_links/migrations/0002_auto_20170522_1552.py` & `wagtail_links-2.8.0b1/src/wagtail_links/migrations/0002_auto_20170522_1552.py`

 * *Files identical despite different names*

### Comparing `wagtail_links-2.7.0/src/wagtail_links/migrations/0003_auto_20170522_2015.py` & `wagtail_links-2.8.0b1/src/wagtail_links/migrations/0003_auto_20170522_2015.py`

 * *Files identical despite different names*

### Comparing `wagtail_links-2.7.0/src/wagtail_links/migrations/0004_auto_20190411_2102.py` & `wagtail_links-2.8.0b1/src/wagtail_links/migrations/0004_auto_20190411_2102.py`

 * *Files identical despite different names*

### Comparing `wagtail_links-2.7.0/src/wagtail_links/migrations/0005_auto_20191203_1908_squashed_0006_auto_20191204_2129.py` & `wagtail_links-2.8.0b1/src/wagtail_links/migrations/0005_auto_20191203_1908_squashed_0006_auto_20191204_2129.py`

 * *Files identical despite different names*

### Comparing `wagtail_links-2.7.0/src/wagtail_links/migrations/0006_auto_20200101_1646.py` & `wagtail_links-2.8.0b1/src/wagtail_links/migrations/0006_auto_20200101_1646.py`

 * *Files identical despite different names*

### Comparing `wagtail_links-2.7.0/src/wagtail_links/migrations/0007_auto_20200101_1658.py` & `wagtail_links-2.8.0b1/src/wagtail_links/migrations/0007_auto_20200101_1658.py`

 * *Files identical despite different names*

### Comparing `wagtail_links-2.7.0/src/wagtail_links/models.py` & `wagtail_links-2.8.0b1/src/wagtail_links/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_links-2.7.0/src/wagtail_links/templatetags/wagtail_links.py` & `wagtail_links-2.8.0b1/src/wagtail_links/templatetags/wagtail_links.py`

 * *Files identical despite different names*

### Comparing `wagtail_links-2.7.0/src/wagtail_links/tests.py` & `wagtail_links-2.8.0b1/src/wagtail_links/tests.py`

 * *Files identical despite different names*

### Comparing `wagtail_links-2.7.0/PKG-INFO` & `wagtail_links-2.8.0b1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,97 +1,89 @@
 Metadata-Version: 2.1
 Name: wagtail-links
-Version: 2.7.0
+Version: 2.8.0b1
 Summary: Wagtail links provides a consistent way to refer to links in a wagtail page.
 Home-page: https://gitlab.com/thelabnyc/wagtail-links
 License: ISC
-Author: thelabnyc
-Author-email: thelabdev@thelabnyc.com
+Author: thelab
+Author-email: thelabdev@thelab.co
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: wagtail (>=5.2,<6.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: wagtail (>=5.2,<6.2)
 Project-URL: Repository, https://gitlab.com/thelabnyc/wagtail-links
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 
-=============
-Wagtail Links
-=============
+# wagtail-links
 
-Purpose
-=======
+## Purpose
 
 Wagtail links has two goals:
 
 - Provide a consistent way to refer to links, which may be of different types, so as to reduce decision fatigue
 - Minimize broken links as much as possible.
 
 
 
-Install
-=======
+## Install
 
 Install wagtail-links via Pip.
 
-.. code:: bash
+```sh
+pip install wagtail-links
+```
 
-    pip install wagtail-links
-
-Add ``wagtail_links`` to your Django project's INSTALLED_APPS setting.
+Add `wagtail_links` to your Django project's `INSTALLED_APPS` setting.
 
 Run database migrations.
 
-.. code:: bash
-
-    python manage.py migrate
+```sh
+python manage.py migrate
+```
 
 
-
-Usage
-=====
+## Usage
 
 Add a foreign key to the page you wish to add links to.
 
-.. code:: python
-
-    my_link = models.ForeignKey(
-        'wagtail_links.Link',
-        null=True,
-        blank=True,
-        on_delete=models.SET_NULL,
-        related_name='+'
-    )
+```py
+my_link = models.ForeignKey(
+    'wagtail_links.Link',
+    null=True,
+    blank=True,
+    on_delete=models.SET_NULL,
+    related_name='+'
+)
+```
 
 Neat:
 
-.. image:: admin.png
+![](admin.png)
 
 You may use it like:
 
-.. code:: html
-
-    <a href="{{ self.link.url }}">Link here</a>
-
+```html
+<a href="{{ self.link.url }}">Link here</a>
+```
 
 From a template, you can also load a link by its name:
 
-.. code:: html
+```html
+{% load get_wagtail_link_url from wagtail_links %}
 
-    {% load get_wagtail_link_url from wagtail_links %}
-
-    <a href="{% get_wagtail_link_url 'my-link' %}">Link here</a>
+<a href="{% get_wagtail_link_url 'my-link' %}">Link here</a>
+```
 
 This is useful for global page links, navigation, etc.
 
 
-
-Validation and logging
-======================
+## Validation and logging
 
 The Link model will validate that one and only one field is set.
 It will also disallow invalid Django reverse view names.
 
 If a URL cannot be determined, we'll log the issue as a warning. We won't throw an exception as that would be bad for users. You are responsible for capturing this log warning, perhaps using Sentry.
 
 For example - let's say you make a Django view name called admin:index. This would typically give you `/admin/`. Later the admin application is removed from the program, now this link fails. It will now display "" and generate a warning in your server logs.
```

#### html2text {}

```diff
@@ -1,29 +1,28 @@
-Metadata-Version: 2.1 Name: wagtail-links Version: 2.7.0 Summary: Wagtail links
-provides a consistent way to refer to links in a wagtail page. Home-page:
-https://gitlab.com/thelabnyc/wagtail-links License: ISC Author: thelabnyc
-Author-email: thelabdev@thelabnyc.com Requires-Python: >=3.10,<4.0 Classifier:
-License :: OSI Approved Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Dist: wagtail (>=5.2,<6.0) Project-URL:
-Repository, https://gitlab.com/thelabnyc/wagtail-links Description-Content-
-Type: text/x-rst ============= Wagtail Links ============= Purpose =======
-Wagtail links has two goals: - Provide a consistent way to refer to links,
-which may be of different types, so as to reduce decision fatigue - Minimize
-broken links as much as possible. Install ======= Install wagtail-links via
-Pip. .. code:: bash pip install wagtail-links Add ``wagtail_links`` to your
-Django project's INSTALLED_APPS setting. Run database migrations. .. code::
-bash python manage.py migrate Usage ===== Add a foreign key to the page you
-wish to add links to. .. code:: python my_link = models.ForeignKey
-( 'wagtail_links.Link', null=True, blank=True, on_delete=models.SET_NULL,
-related_name='+' ) Neat: .. image:: admin.png You may use it like: .. code::
-html _L_i_n_k_ _h_e_r_e From a template, you can also load a link by its name: .. code::
-html {% load get_wagtail_link_url from wagtail_links %} _L_i_n_k_ _h_e_r_e This is
-useful for global page links, navigation, etc. Validation and logging
-====================== The Link model will validate that one and only one field
-is set. It will also disallow invalid Django reverse view names. If a URL
-cannot be determined, we'll log the issue as a warning. We won't throw an
-exception as that would be bad for users. You are responsible for capturing
-this log warning, perhaps using Sentry. For example - let's say you make a
-Django view name called admin:index. This would typically give you `/admin/`.
-Later the admin application is removed from the program, now this link fails.
-It will now display "" and generate a warning in your server logs.
+Metadata-Version: 2.1 Name: wagtail-links Version: 2.8.0b1 Summary: Wagtail
+links provides a consistent way to refer to links in a wagtail page. Home-page:
+https://gitlab.com/thelabnyc/wagtail-links License: ISC Author: thelab Author-
+email: thelabdev@thelab.co Requires-Python: >=3.10,<4.0 Classifier: License ::
+OSI Approved Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
+Dist: wagtail (>=5.2,<6.2) Project-URL: Repository, https://gitlab.com/
+thelabnyc/wagtail-links Description-Content-Type: text/markdown # wagtail-links
+## Purpose Wagtail links has two goals: - Provide a consistent way to refer to
+links, which may be of different types, so as to reduce decision fatigue -
+Minimize broken links as much as possible. ## Install Install wagtail-links via
+Pip. ```sh pip install wagtail-links ``` Add `wagtail_links` to your Django
+project's `INSTALLED_APPS` setting. Run database migrations. ```sh python
+manage.py migrate ``` ## Usage Add a foreign key to the page you wish to add
+links to. ```py my_link = models.ForeignKey( 'wagtail_links.Link', null=True,
+blank=True, on_delete=models.SET_NULL, related_name='+' ) ``` Neat: ![]
+(admin.png) You may use it like: ```html _L_i_n_k_ _h_e_r_e ``` From a template, you can
+also load a link by its name: ```html {% load get_wagtail_link_url from
+wagtail_links %} _L_i_n_k_ _h_e_r_e ``` This is useful for global page links,
+navigation, etc. ## Validation and logging The Link model will validate that
+one and only one field is set. It will also disallow invalid Django reverse
+view names. If a URL cannot be determined, we'll log the issue as a warning. We
+won't throw an exception as that would be bad for users. You are responsible
+for capturing this log warning, perhaps using Sentry. For example - let's say
+you make a Django view name called admin:index. This would typically give you
+`/admin/`. Later the admin application is removed from the program, now this
+link fails. It will now display "" and generate a warning in your server logs.
```

