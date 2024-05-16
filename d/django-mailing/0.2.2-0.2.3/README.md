# Comparing `tmp/django_mailing-0.2.2.tar.gz` & `tmp/django_mailing-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_mailing-0.2.2.tar", last modified: Fri May  3 13:23:43 2024, max compression
+gzip compressed data, was "django_mailing-0.2.3.tar", last modified: Thu May 16 19:23:05 2024, max compression
```

## Comparing `django_mailing-0.2.2.tar` & `django_mailing-0.2.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jparadis   (501) staff       (20)        0 2024-05-03 13:23:43.735675 django_mailing-0.2.2/
--rwxr-xr-x   0 jparadis   (501) staff       (20)      178 2023-05-05 14:19:38.000000 django_mailing-0.2.2/AUTHORS.txt
--rwxr-xr-x   0 jparadis   (501) staff       (20)       41 2023-05-05 14:19:38.000000 django_mailing-0.2.2/CHANGES.txt
--rwxr-xr-x   0 jparadis   (501) staff       (20)     1113 2023-05-05 14:19:38.000000 django_mailing-0.2.2/LICENSE.txt
--rwxr-xr-x   0 jparadis   (501) staff       (20)      134 2023-05-05 14:19:38.000000 django_mailing-0.2.2/MANIFEST.in
--rw-r--r--   0 jparadis   (501) staff       (20)     8957 2024-05-03 13:23:43.735099 django_mailing-0.2.2/PKG-INFO
--rwxr-xr-x   0 jparadis   (501) staff       (20)     8415 2023-05-05 14:19:38.000000 django_mailing-0.2.2/README.txt
-drwxr-xr-x   0 jparadis   (501) staff       (20)        0 2024-05-03 13:23:43.734588 django_mailing-0.2.2/django_mailing.egg-info/
--rw-r--r--   0 jparadis   (501) staff       (20)     8957 2024-05-03 13:23:43.000000 django_mailing-0.2.2/django_mailing.egg-info/PKG-INFO
--rw-r--r--   0 jparadis   (501) staff       (20)      687 2024-05-03 13:23:43.000000 django_mailing-0.2.2/django_mailing.egg-info/SOURCES.txt
--rw-r--r--   0 jparadis   (501) staff       (20)        1 2024-05-03 13:23:43.000000 django_mailing-0.2.2/django_mailing.egg-info/dependency_links.txt
--rw-r--r--   0 jparadis   (501) staff       (20)       49 2024-05-03 13:23:43.000000 django_mailing-0.2.2/django_mailing.egg-info/requires.txt
--rw-r--r--   0 jparadis   (501) staff       (20)        8 2024-05-03 13:23:43.000000 django_mailing-0.2.2/django_mailing.egg-info/top_level.txt
-drwxr-xr-x   0 jparadis   (501) staff       (20)        0 2024-05-03 13:23:43.727230 django_mailing-0.2.2/docs/
--rwxr-xr-x   0 jparadis   (501) staff       (20)     8415 2023-05-05 14:19:38.000000 django_mailing-0.2.2/docs/usage.txt
-drwxr-xr-x   0 jparadis   (501) staff       (20)        0 2024-05-03 13:23:43.730758 django_mailing-0.2.2/mailing/
--rwxr-xr-x   0 jparadis   (501) staff       (20)      525 2024-05-03 13:09:42.000000 django_mailing-0.2.2/mailing/__init__.py
--rwxr-xr-x   0 jparadis   (501) staff       (20)     5074 2024-05-03 13:12:14.000000 django_mailing-0.2.2/mailing/mail.py
--rwxr-xr-x   0 jparadis   (501) staff       (20)        0 2023-05-05 14:19:38.000000 django_mailing-0.2.2/mailing/models.py
--rwxr-xr-x   0 jparadis   (501) staff       (20)     2307 2024-05-03 13:13:32.000000 django_mailing-0.2.2/mailing/shortcuts.py
--rwxr-xr-x   0 jparadis   (501) staff       (20)     1938 2024-05-03 13:13:16.000000 django_mailing-0.2.2/mailing/tasks.py
-drwxr-xr-x   0 jparadis   (501) staff       (20)        0 2024-05-03 13:23:43.721063 django_mailing-0.2.2/mailing/templates/
-drwxr-xr-x   0 jparadis   (501) staff       (20)        0 2024-05-03 13:23:43.731653 django_mailing-0.2.2/mailing/templates/mailing/
--rwxr-xr-x   0 jparadis   (501) staff       (20)     3245 2023-05-05 14:19:38.000000 django_mailing-0.2.2/mailing/templates/mailing/base.html
--rwxr-xr-x   0 jparadis   (501) staff       (20)      150 2023-05-05 14:19:38.000000 django_mailing-0.2.2/mailing/templates/mailing/base.txt
-drwxr-xr-x   0 jparadis   (501) staff       (20)        0 2024-05-03 13:23:43.733917 django_mailing-0.2.2/mailing/templates/mailing/email_boiletplate/
--rw-r--r--   0 jparadis   (501) staff       (20)     2555 2023-05-05 14:19:38.000000 django_mailing-0.2.2/mailing/templates/mailing/email_boiletplate/README.markdown
--rw-r--r--   0 jparadis   (501) staff       (20)      352 2023-05-05 14:19:38.000000 django_mailing-0.2.2/mailing/templates/mailing/email_boiletplate/contributors.txt
--rw-r--r--   0 jparadis   (501) staff       (20)    12246 2023-05-05 14:19:38.000000 django_mailing-0.2.2/mailing/templates/mailing/email_boiletplate/email.html
--rw-r--r--   0 jparadis   (501) staff       (20)     6542 2023-05-05 14:19:38.000000 django_mailing-0.2.2/mailing/templates/mailing/email_boiletplate/email_lite.html
--rwxr-xr-x   0 jparadis   (501) staff       (20)       26 2023-05-05 14:19:38.000000 django_mailing-0.2.2/mailing/views.py
--rw-r--r--   0 jparadis   (501) staff       (20)       38 2024-05-03 13:23:43.735773 django_mailing-0.2.2/setup.cfg
--rwxr-xr-x   0 jparadis   (501) staff       (20)     1099 2023-05-05 14:19:38.000000 django_mailing-0.2.2/setup.py
+drwxr-xr-x   0 jparadis   (501) staff       (20)        0 2024-05-16 19:23:05.072550 django_mailing-0.2.3/
+-rwxr-xr-x   0 jparadis   (501) staff       (20)      178 2023-05-05 14:19:38.000000 django_mailing-0.2.3/AUTHORS.txt
+-rwxr-xr-x   0 jparadis   (501) staff       (20)       41 2023-05-05 14:19:38.000000 django_mailing-0.2.3/CHANGES.txt
+-rwxr-xr-x   0 jparadis   (501) staff       (20)     1113 2023-05-05 14:19:38.000000 django_mailing-0.2.3/LICENSE.txt
+-rwxr-xr-x   0 jparadis   (501) staff       (20)      134 2023-05-05 14:19:38.000000 django_mailing-0.2.3/MANIFEST.in
+-rw-r--r--   0 jparadis   (501) staff       (20)     8957 2024-05-16 19:23:05.072117 django_mailing-0.2.3/PKG-INFO
+-rwxr-xr-x   0 jparadis   (501) staff       (20)     8415 2023-05-05 14:19:38.000000 django_mailing-0.2.3/README.txt
+drwxr-xr-x   0 jparadis   (501) staff       (20)        0 2024-05-16 19:23:05.071553 django_mailing-0.2.3/django_mailing.egg-info/
+-rw-r--r--   0 jparadis   (501) staff       (20)     8957 2024-05-16 19:23:05.000000 django_mailing-0.2.3/django_mailing.egg-info/PKG-INFO
+-rw-r--r--   0 jparadis   (501) staff       (20)      687 2024-05-16 19:23:05.000000 django_mailing-0.2.3/django_mailing.egg-info/SOURCES.txt
+-rw-r--r--   0 jparadis   (501) staff       (20)        1 2024-05-16 19:23:05.000000 django_mailing-0.2.3/django_mailing.egg-info/dependency_links.txt
+-rw-r--r--   0 jparadis   (501) staff       (20)       49 2024-05-16 19:23:05.000000 django_mailing-0.2.3/django_mailing.egg-info/requires.txt
+-rw-r--r--   0 jparadis   (501) staff       (20)        8 2024-05-16 19:23:05.000000 django_mailing-0.2.3/django_mailing.egg-info/top_level.txt
+drwxr-xr-x   0 jparadis   (501) staff       (20)        0 2024-05-16 19:23:05.065151 django_mailing-0.2.3/docs/
+-rwxr-xr-x   0 jparadis   (501) staff       (20)     8415 2023-05-05 14:19:38.000000 django_mailing-0.2.3/docs/usage.txt
+drwxr-xr-x   0 jparadis   (501) staff       (20)        0 2024-05-16 19:23:05.068071 django_mailing-0.2.3/mailing/
+-rwxr-xr-x   0 jparadis   (501) staff       (20)      525 2024-05-16 19:18:24.000000 django_mailing-0.2.3/mailing/__init__.py
+-rwxr-xr-x   0 jparadis   (501) staff       (20)     5372 2024-05-16 19:14:13.000000 django_mailing-0.2.3/mailing/mail.py
+-rwxr-xr-x   0 jparadis   (501) staff       (20)        0 2023-05-05 14:19:38.000000 django_mailing-0.2.3/mailing/models.py
+-rwxr-xr-x   0 jparadis   (501) staff       (20)     2307 2024-05-03 13:13:32.000000 django_mailing-0.2.3/mailing/shortcuts.py
+-rwxr-xr-x   0 jparadis   (501) staff       (20)     1938 2024-05-03 13:13:16.000000 django_mailing-0.2.3/mailing/tasks.py
+drwxr-xr-x   0 jparadis   (501) staff       (20)        0 2024-05-16 19:23:05.059106 django_mailing-0.2.3/mailing/templates/
+drwxr-xr-x   0 jparadis   (501) staff       (20)        0 2024-05-16 19:23:05.069004 django_mailing-0.2.3/mailing/templates/mailing/
+-rwxr-xr-x   0 jparadis   (501) staff       (20)     3245 2023-05-05 14:19:38.000000 django_mailing-0.2.3/mailing/templates/mailing/base.html
+-rwxr-xr-x   0 jparadis   (501) staff       (20)      150 2023-05-05 14:19:38.000000 django_mailing-0.2.3/mailing/templates/mailing/base.txt
+drwxr-xr-x   0 jparadis   (501) staff       (20)        0 2024-05-16 19:23:05.070993 django_mailing-0.2.3/mailing/templates/mailing/email_boiletplate/
+-rw-r--r--   0 jparadis   (501) staff       (20)     2555 2023-05-05 14:19:38.000000 django_mailing-0.2.3/mailing/templates/mailing/email_boiletplate/README.markdown
+-rw-r--r--   0 jparadis   (501) staff       (20)      352 2023-05-05 14:19:38.000000 django_mailing-0.2.3/mailing/templates/mailing/email_boiletplate/contributors.txt
+-rw-r--r--   0 jparadis   (501) staff       (20)    12246 2023-05-05 14:19:38.000000 django_mailing-0.2.3/mailing/templates/mailing/email_boiletplate/email.html
+-rw-r--r--   0 jparadis   (501) staff       (20)     6542 2023-05-05 14:19:38.000000 django_mailing-0.2.3/mailing/templates/mailing/email_boiletplate/email_lite.html
+-rwxr-xr-x   0 jparadis   (501) staff       (20)       26 2023-05-05 14:19:38.000000 django_mailing-0.2.3/mailing/views.py
+-rw-r--r--   0 jparadis   (501) staff       (20)       38 2024-05-16 19:23:05.072638 django_mailing-0.2.3/setup.cfg
+-rwxr-xr-x   0 jparadis   (501) staff       (20)     1099 2023-05-05 14:19:38.000000 django_mailing-0.2.3/setup.py
```

### Comparing `django_mailing-0.2.2/LICENSE.txt` & `django_mailing-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django_mailing-0.2.2/PKG-INFO` & `django_mailing-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mailing
-Version: 0.2.2
+Version: 0.2.3
 Summary: A flexible Django app for templated mailings with support for celery queuing, SendGrid and more.
 Home-page: http://github.com/JeromeParadis/django-mailing
 Author: Jerome Paradis
 Author-email: jparadis@paradivision.com
 License: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `django_mailing-0.2.2/README.txt` & `django_mailing-0.2.3/README.txt`

 * *Files identical despite different names*

### Comparing `django_mailing-0.2.2/django_mailing.egg-info/PKG-INFO` & `django_mailing-0.2.3/django_mailing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mailing
-Version: 0.2.2
+Version: 0.2.3
 Summary: A flexible Django app for templated mailings with support for celery queuing, SendGrid and more.
 Home-page: http://github.com/JeromeParadis/django-mailing
 Author: Jerome Paradis
 Author-email: jparadis@paradivision.com
 License: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `django_mailing-0.2.2/django_mailing.egg-info/SOURCES.txt` & `django_mailing-0.2.3/django_mailing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_mailing-0.2.2/docs/usage.txt` & `django_mailing-0.2.3/docs/usage.txt`

 * *Files identical despite different names*

### Comparing `django_mailing-0.2.2/mailing/__init__.py` & `django_mailing-0.2.3/mailing/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Versioning
 # --------------------------------
 #VERSION = (0, 1, 0, "beta", 11) # following PEP 386
-VERSION = (0, 2, 2, "f") # following PEP 386
+VERSION = (0, 2, 3, "f") # following PEP 386
 DEV_N = None
 
 def get_version():
     version = "%s.%s" % (VERSION[0], VERSION[1])
     if VERSION[2]:
         version = "%s.%s" % (version, VERSION[2])
     if VERSION[3] != "f":
```

### Comparing `django_mailing-0.2.2/mailing/mail.py` & `django_mailing-0.2.3/mailing/mail.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import absolute_import
 from django.conf import settings
 from django.core.mail import EmailMultiAlternatives, EmailMessage
 from django.template.loader import render_to_string
 from django.utils import translation
 import six
+import json 
 
 # Define exception classes
 # --------------------------------
 class MailerInvalidBodyError(Exception):
     def __init__(self, value):
         self.value = value
     def __str__(self):
@@ -39,15 +40,21 @@
             send_grid_support = settings.MAILING_USE_SENDGRID
         else:
             send_grid_support = False
 
         if not headers:
             headers = dict()        
         if send_grid_support and category:
-            headers['X-SMTPAPI'] = '{"category": "%s"}' % header_category_value
+            if 'X-SMTPAPI' not in headers:
+                headers['X-SMTPAPI'] = '{"category": "%s"}' % header_category_value
+            else:
+                xsmtpapi = headers['X-SMTPAPI']
+                if type(xsmtpapi) == dict:
+                    xsmtpapi['category'] = header_category_value
+                    headers['X-SMTPAPI'] = json.dumps(xsmtpapi)
 
         # Check for Mailgun support and add label header
         # --------------------------------
         if hasattr(settings, 'MAILING_USE_MAILGUN'):
             mailgun_support = settings.MAILING_USE_MAILGUN
         else:
             mailgun_support = False
```

### Comparing `django_mailing-0.2.2/mailing/shortcuts.py` & `django_mailing-0.2.3/mailing/shortcuts.py`

 * *Files identical despite different names*

### Comparing `django_mailing-0.2.2/mailing/tasks.py` & `django_mailing-0.2.3/mailing/tasks.py`

 * *Files identical despite different names*

### Comparing `django_mailing-0.2.2/mailing/templates/mailing/base.html` & `django_mailing-0.2.3/mailing/templates/mailing/base.html`

 * *Files identical despite different names*

### Comparing `django_mailing-0.2.2/mailing/templates/mailing/email_boiletplate/README.markdown` & `django_mailing-0.2.3/mailing/templates/mailing/email_boiletplate/README.markdown`

 * *Files identical despite different names*

### Comparing `django_mailing-0.2.2/mailing/templates/mailing/email_boiletplate/email.html` & `django_mailing-0.2.3/mailing/templates/mailing/email_boiletplate/email.html`

 * *Files identical despite different names*

### Comparing `django_mailing-0.2.2/mailing/templates/mailing/email_boiletplate/email_lite.html` & `django_mailing-0.2.3/mailing/templates/mailing/email_boiletplate/email_lite.html`

 * *Files identical despite different names*

### Comparing `django_mailing-0.2.2/setup.py` & `django_mailing-0.2.3/setup.py`

 * *Files identical despite different names*

