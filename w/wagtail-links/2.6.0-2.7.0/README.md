# Comparing `tmp/wagtail-links-2.6.0.tar.gz` & `tmp/wagtail_links-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-links-2.6.0.tar", last modified: Wed Oct 11 16:19:43 2023, max compression
+gzip compressed data, was "wagtail_links-2.7.0.tar", max compression
```

## Comparing `wagtail-links-2.6.0.tar` & `wagtail_links-2.7.0.tar`

### file list

```diff
@@ -1,37 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-11 16:19:43.064596 wagtail-links-2.6.0/
--rw-rw-rw-   0 root         (0) root         (0)      740 2023-10-11 16:19:32.000000 wagtail-links-2.6.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       98 2023-10-11 16:19:32.000000 wagtail-links-2.6.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2643 2023-10-11 16:19:43.064596 wagtail-links-2.6.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1746 2023-10-11 16:19:32.000000 wagtail-links-2.6.0/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      126 2023-10-11 16:19:43.065596 wagtail-links-2.6.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1585 2023-10-11 16:19:32.000000 wagtail-links-2.6.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-11 16:19:43.057596 wagtail-links-2.6.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-11 16:19:43.060596 wagtail-links-2.6.0/src/wagtail_links/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-11 16:19:32.000000 wagtail-links-2.6.0/src/wagtail_links/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      233 2023-10-11 16:19:32.000000 wagtail-links-2.6.0/src/wagtail_links/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     1173 2023-10-11 16:19:32.000000 wagtail-links-2.6.0/src/wagtail_links/fields.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-11 16:19:43.057596 wagtail-links-2.6.0/src/wagtail_links/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-11 16:19:43.057596 wagtail-links-2.6.0/src/wagtail_links/locale/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-11 16:19:43.061596 wagtail-links-2.6.0/src/wagtail_links/locale/es/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      380 2023-10-11 16:19:32.000000 wagtail-links-2.6.0/src/wagtail_links/locale/es/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)     2630 2023-10-11 16:19:32.000000 wagtail-links-2.6.0/src/wagtail_links/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-11 16:19:43.063596 wagtail-links-2.6.0/src/wagtail_links/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1721 2023-10-11 16:19:32.000000 wagtail-links-2.6.0/src/wagtail_links/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      856 2023-10-11 16:19:32.000000 wagtail-links-2.6.0/src/wagtail_links/migrations/0002_auto_20170522_1552.py
--rw-rw-rw-   0 root         (0) root         (0)      696 2023-10-11 16:19:32.000000 wagtail-links-2.6.0/src/wagtail_links/migrations/0003_auto_20170522_2015.py
--rw-rw-rw-   0 root         (0) root         (0)     2236 2023-10-11 16:19:32.000000 wagtail-links-2.6.0/src/wagtail_links/migrations/0004_auto_20190411_2102.py
--rw-rw-rw-   0 root         (0) root         (0)     2939 2023-10-11 16:19:32.000000 wagtail-links-2.6.0/src/wagtail_links/migrations/0005_auto_20191203_1908_squashed_0006_auto_20191204_2129.py
--rw-rw-rw-   0 root         (0) root         (0)      596 2023-10-11 16:19:32.000000 wagtail-links-2.6.0/src/wagtail_links/migrations/0006_auto_20200101_1646.py
--rw-rw-rw-   0 root         (0) root         (0)      578 2023-10-11 16:19:32.000000 wagtail-links-2.6.0/src/wagtail_links/migrations/0007_auto_20200101_1658.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-11 16:19:32.000000 wagtail-links-2.6.0/src/wagtail_links/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4938 2023-10-11 16:19:32.000000 wagtail-links-2.6.0/src/wagtail_links/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-11 16:19:43.063596 wagtail-links-2.6.0/src/wagtail_links/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-11 16:19:32.000000 wagtail-links-2.6.0/src/wagtail_links/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      565 2023-10-11 16:19:32.000000 wagtail-links-2.6.0/src/wagtail_links/templatetags/wagtail_links.py
--rw-rw-rw-   0 root         (0) root         (0)     3903 2023-10-11 16:19:32.000000 wagtail-links-2.6.0/src/wagtail_links/tests.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-11 16:19:43.061596 wagtail-links-2.6.0/src/wagtail_links.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2643 2023-10-11 16:19:43.000000 wagtail-links-2.6.0/src/wagtail_links.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1038 2023-10-11 16:19:43.000000 wagtail-links-2.6.0/src/wagtail_links.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-11 16:19:43.000000 wagtail-links-2.6.0/src/wagtail_links.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       76 2023-10-11 16:19:43.000000 wagtail-links-2.6.0/src/wagtail_links.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-10-11 16:19:43.000000 wagtail-links-2.6.0/src/wagtail_links.egg-info/top_level.txt
+-rw-r--r--   0        0        0      747 2024-02-27 15:04:54.895588 wagtail_links-2.7.0/LICENSE
+-rw-r--r--   0        0        0     1746 2024-02-27 15:04:54.895588 wagtail_links-2.7.0/README.rst
+-rw-r--r--   0        0        0      652 2024-02-27 15:04:54.896588 wagtail_links-2.7.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-27 15:04:54.921588 wagtail_links-2.7.0/src/wagtail_links/__init__.py
+-rw-r--r--   0        0        0      233 2024-02-27 15:04:54.896588 wagtail_links-2.7.0/src/wagtail_links/apps.py
+-rw-r--r--   0        0        0     1173 2024-02-27 15:04:54.897589 wagtail_links-2.7.0/src/wagtail_links/fields.py
+-rw-r--r--   0        0        0      380 2024-02-27 15:04:54.897589 wagtail_links-2.7.0/src/wagtail_links/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2630 2024-02-27 15:04:54.897589 wagtail_links-2.7.0/src/wagtail_links/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1720 2024-02-27 15:04:54.897589 wagtail_links-2.7.0/src/wagtail_links/migrations/0001_initial.py
+-rw-r--r--   0        0        0      855 2024-02-27 15:04:54.897589 wagtail_links-2.7.0/src/wagtail_links/migrations/0002_auto_20170522_1552.py
+-rw-r--r--   0        0        0      695 2024-02-27 15:04:54.897589 wagtail_links-2.7.0/src/wagtail_links/migrations/0003_auto_20170522_2015.py
+-rw-r--r--   0        0        0     2235 2024-02-27 15:04:54.897589 wagtail_links-2.7.0/src/wagtail_links/migrations/0004_auto_20190411_2102.py
+-rw-r--r--   0        0        0     2938 2024-02-27 15:04:54.897589 wagtail_links-2.7.0/src/wagtail_links/migrations/0005_auto_20191203_1908_squashed_0006_auto_20191204_2129.py
+-rw-r--r--   0        0        0      595 2024-02-27 15:04:54.897589 wagtail_links-2.7.0/src/wagtail_links/migrations/0006_auto_20200101_1646.py
+-rw-r--r--   0        0        0      577 2024-02-27 15:04:54.897589 wagtail_links-2.7.0/src/wagtail_links/migrations/0007_auto_20200101_1658.py
+-rw-r--r--   0        0        0        0 2024-02-27 15:04:54.924588 wagtail_links-2.7.0/src/wagtail_links/migrations/__init__.py
+-rw-r--r--   0        0        0     4888 2024-02-27 15:04:54.897589 wagtail_links-2.7.0/src/wagtail_links/models.py
+-rw-r--r--   0        0        0        0 2024-02-27 15:04:54.924588 wagtail_links-2.7.0/src/wagtail_links/templatetags/__init__.py
+-rw-r--r--   0        0        0      565 2024-02-27 15:04:54.897589 wagtail_links-2.7.0/src/wagtail_links/templatetags/wagtail_links.py
+-rw-r--r--   0        0        0     3903 2024-02-27 15:04:54.897589 wagtail_links-2.7.0/src/wagtail_links/tests.py
+-rw-r--r--   0        0        0     2370 1970-01-01 00:00:00.000000 wagtail_links-2.7.0/PKG-INFO
```

### Comparing `wagtail-links-2.6.0/LICENSE` & `wagtail_links-2.7.0/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ISC License
 
-Copyright (c) 2023 thelabnyc
+Copyright (c) 2017 - 2024 thelabnyc
 
 Permission to use, copy, modify, and/or distribute this software for any
 purpose with or without fee is hereby granted, provided that the above
 copyright notice and this permission notice appear in all copies.
 
 THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
 REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY
```

### Comparing `wagtail-links-2.6.0/PKG-INFO` & `wagtail_links-2.7.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,23 @@
 Metadata-Version: 2.1
 Name: wagtail-links
-Version: 2.6.0
+Version: 2.7.0
 Summary: Wagtail links provides a consistent way to refer to links in a wagtail page.
 Home-page: https://gitlab.com/thelabnyc/wagtail-links
+License: ISC
 Author: thelabnyc
 Author-email: thelabdev@thelabnyc.com
-License: ISC
-Keywords: django wagtail
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Framework :: Wagtail
-Classifier: Programming Language :: Python
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-License-File: LICENSE
-Requires-Dist: wagtail<6.0,>=4.1
-Provides-Extra: development
-Requires-Dist: flake8>=3.3.0; extra == "development"
-Requires-Dist: tox>=2.7.0; extra == "development"
-Requires-Dist: versiontag>=1.2.0; extra == "development"
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: wagtail (>=5.2,<6.0)
+Project-URL: Repository, https://gitlab.com/thelabnyc/wagtail-links
+Description-Content-Type: text/x-rst
 
 =============
 Wagtail Links
 =============
 
 Purpose
 =======
@@ -98,7 +91,8 @@
 
 The Link model will validate that one and only one field is set.
 It will also disallow invalid Django reverse view names.
 
 If a URL cannot be determined, we'll log the issue as a warning. We won't throw an exception as that would be bad for users. You are responsible for capturing this log warning, perhaps using Sentry.
 
 For example - let's say you make a Django view name called admin:index. This would typically give you `/admin/`. Later the admin application is removed from the program, now this link fails. It will now display "" and generate a warning in your server logs.
+
```

#### html2text {}

```diff
@@ -1,33 +1,29 @@
-Metadata-Version: 2.1 Name: wagtail-links Version: 2.6.0 Summary: Wagtail links
+Metadata-Version: 2.1 Name: wagtail-links Version: 2.7.0 Summary: Wagtail links
 provides a consistent way to refer to links in a wagtail page. Home-page:
-https://gitlab.com/thelabnyc/wagtail-links Author: thelabnyc Author-email:
-thelabdev@thelabnyc.com License: ISC Keywords: django wagtail Classifier:
-Development Status :: 5 - Production/Stable Classifier: Environment :: Web
-Environment Classifier: Framework :: Django Classifier: Framework :: Wagtail
-Classifier: Programming Language :: Python Classifier: Programming Language ::
-Python :: 3 Classifier: Intended Audience :: Developers Classifier: License ::
-OSI Approved :: Apache Software License License-File: LICENSE Requires-Dist:
-wagtail<6.0,>=4.1 Provides-Extra: development Requires-Dist: flake8>=3.3.0;
-extra == "development" Requires-Dist: tox>=2.7.0; extra == "development"
-Requires-Dist: versiontag>=1.2.0; extra == "development" ============= Wagtail
-Links ============= Purpose ======= Wagtail links has two goals: - Provide a
-consistent way to refer to links, which may be of different types, so as to
-reduce decision fatigue - Minimize broken links as much as possible. Install
-======= Install wagtail-links via Pip. .. code:: bash pip install wagtail-links
-Add ``wagtail_links`` to your Django project's INSTALLED_APPS setting. Run
-database migrations. .. code:: bash python manage.py migrate Usage ===== Add a
-foreign key to the page you wish to add links to. .. code:: python my_link =
-models.ForeignKey( 'wagtail_links.Link', null=True, blank=True,
-on_delete=models.SET_NULL, related_name='+' ) Neat: .. image:: admin.png You
-may use it like: .. code:: html _L_i_n_k_ _h_e_r_e From a template, you can also load a
-link by its name: .. code:: html {% load get_wagtail_link_url from
-wagtail_links %} _L_i_n_k_ _h_e_r_e This is useful for global page links, navigation,
-etc. Validation and logging ====================== The Link model will validate
-that one and only one field is set. It will also disallow invalid Django
-reverse view names. If a URL cannot be determined, we'll log the issue as a
-warning. We won't throw an exception as that would be bad for users. You are
-responsible for capturing this log warning, perhaps using Sentry. For example -
-let's say you make a Django view name called admin:index. This would typically
-give you `/admin/`. Later the admin application is removed from the program,
-now this link fails. It will now display "" and generate a warning in your
-server logs.
+https://gitlab.com/thelabnyc/wagtail-links License: ISC Author: thelabnyc
+Author-email: thelabdev@thelabnyc.com Requires-Python: >=3.10,<4.0 Classifier:
+License :: OSI Approved Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Requires-Dist: wagtail (>=5.2,<6.0) Project-URL:
+Repository, https://gitlab.com/thelabnyc/wagtail-links Description-Content-
+Type: text/x-rst ============= Wagtail Links ============= Purpose =======
+Wagtail links has two goals: - Provide a consistent way to refer to links,
+which may be of different types, so as to reduce decision fatigue - Minimize
+broken links as much as possible. Install ======= Install wagtail-links via
+Pip. .. code:: bash pip install wagtail-links Add ``wagtail_links`` to your
+Django project's INSTALLED_APPS setting. Run database migrations. .. code::
+bash python manage.py migrate Usage ===== Add a foreign key to the page you
+wish to add links to. .. code:: python my_link = models.ForeignKey
+( 'wagtail_links.Link', null=True, blank=True, on_delete=models.SET_NULL,
+related_name='+' ) Neat: .. image:: admin.png You may use it like: .. code::
+html _L_i_n_k_ _h_e_r_e From a template, you can also load a link by its name: .. code::
+html {% load get_wagtail_link_url from wagtail_links %} _L_i_n_k_ _h_e_r_e This is
+useful for global page links, navigation, etc. Validation and logging
+====================== The Link model will validate that one and only one field
+is set. It will also disallow invalid Django reverse view names. If a URL
+cannot be determined, we'll log the issue as a warning. We won't throw an
+exception as that would be bad for users. You are responsible for capturing
+this log warning, perhaps using Sentry. For example - let's say you make a
+Django view name called admin:index. This would typically give you `/admin/`.
+Later the admin application is removed from the program, now this link fails.
+It will now display "" and generate a warning in your server logs.
```

### Comparing `wagtail-links-2.6.0/README.rst` & `wagtail_links-2.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `wagtail-links-2.6.0/src/wagtail_links/fields.py` & `wagtail_links-2.7.0/src/wagtail_links/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail-links-2.6.0/src/wagtail_links/locale/es/LC_MESSAGES/django.po` & `wagtail_links-2.7.0/src/wagtail_links/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail-links-2.6.0/src/wagtail_links/migrations/0001_initial.py` & `wagtail_links-2.7.0/src/wagtail_links/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from __future__ import unicode_literals
 
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = [
         ("wagtailcore", "0033_remove_golive_expiry_help_text"),
     ]
 
     operations = [
```

### Comparing `wagtail-links-2.6.0/src/wagtail_links/migrations/0002_auto_20170522_1552.py` & `wagtail_links-2.7.0/src/wagtail_links/migrations/0002_auto_20170522_1552.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from __future__ import unicode_literals
 
 import django.core.validators
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("wagtail_links", "0001_initial"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="link",
```

### Comparing `wagtail-links-2.6.0/src/wagtail_links/migrations/0003_auto_20170522_2015.py` & `wagtail_links-2.7.0/src/wagtail_links/migrations/0003_auto_20170522_2015.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from __future__ import unicode_literals
 
 from django.db import migrations, models
 import wagtail_links.models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("wagtail_links", "0002_auto_20170522_1552"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="link",
```

### Comparing `wagtail-links-2.6.0/src/wagtail_links/migrations/0004_auto_20190411_2102.py` & `wagtail_links-2.7.0/src/wagtail_links/migrations/0004_auto_20190411_2102.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import django.core.validators
 from django.db import migrations, models
 import django.db.models.deletion
 import wagtail_links.models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("wagtail_links", "0003_auto_20170522_2015"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="link",
```

### Comparing `wagtail-links-2.6.0/src/wagtail_links/migrations/0005_auto_20191203_1908_squashed_0006_auto_20191204_2129.py` & `wagtail_links-2.7.0/src/wagtail_links/migrations/0005_auto_20191203_1908_squashed_0006_auto_20191204_2129.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import django.core.validators
 from django.db import migrations, models
 import django.db.models.deletion
 import wagtail_links.models
 
 
 class Migration(migrations.Migration):
-
     replaces = [
         ("wagtail_links", "0005_auto_20191203_1908"),
         ("wagtail_links", "0006_auto_20191204_2129"),
     ]
 
     dependencies = [
         ("wagtail_links", "0004_auto_20190411_2102"),
```

### Comparing `wagtail-links-2.6.0/src/wagtail_links/migrations/0006_auto_20200101_1646.py` & `wagtail_links-2.7.0/src/wagtail_links/migrations/0006_auto_20200101_1646.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 2.2.9 on 2020-01-01 16:46
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("wagtail_links", "0005_auto_20191203_1908_squashed_0006_auto_20191204_2129"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="link",
```

### Comparing `wagtail-links-2.6.0/src/wagtail_links/migrations/0007_auto_20200101_1658.py` & `wagtail_links-2.7.0/src/wagtail_links/migrations/0007_auto_20200101_1658.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 2.2.9 on 2020-01-01 16:58
 
 from django.db import migrations
 import wagtail_links.fields
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("wagtail_links", "0006_auto_20200101_1646"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="link",
```

### Comparing `wagtail-links-2.6.0/src/wagtail_links/models.py` & `wagtail_links-2.7.0/src/wagtail_links/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,18 +82,16 @@
         FieldPanel("link_external"),
         FieldPanel("link_relative"),
         PageChooserPanel("link_page"),
         FieldPanel("django_view_name"),
     ]
 
     search_fields = [
-        index.RelatedFields(
-            "link_page", [index.SearchField("title", partial_match=True)]
-        ),
-        index.SearchField("title", partial_match=True),
+        index.RelatedFields("link_page", [index.AutocompleteField("title")]),
+        index.AutocompleteField("title"),
     ]
 
     class Meta:
         # Translators: Internal Model Name (singular)
         verbose_name = _("Link")
         # Translators: Internal Model Name (plural)
         verbose_name_plural = _("Links")
```

### Comparing `wagtail-links-2.6.0/src/wagtail_links/templatetags/wagtail_links.py` & `wagtail_links-2.7.0/src/wagtail_links/templatetags/wagtail_links.py`

 * *Files identical despite different names*

### Comparing `wagtail-links-2.6.0/src/wagtail_links/tests.py` & `wagtail_links-2.7.0/src/wagtail_links/tests.py`

 * *Files identical despite different names*

