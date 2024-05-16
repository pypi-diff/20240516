# Comparing `tmp/django_utilsds-0.5.2.tar.gz` & `tmp/django_utilsds-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_utilsds-0.5.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_utilsds-0.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_utilsds-0.5.2.tar` & `django_utilsds-0.6.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     6148 2024-03-20 03:28:32.696016 django_utilsds-0.5.2/.DS_Store
--rw-r--r--   0        0        0       66 2024-03-19 12:18:20.163079 django_utilsds-0.5.2/.gitattributes
--rw-r--r--   0        0        0        7 2024-03-19 12:37:16.850744 django_utilsds-0.5.2/.gitignore
--rw-r--r--   0        0        0       52 2024-03-19 12:19:45.020079 django_utilsds-0.5.2/.idea/.gitignore
--rw-r--r--   0        0        0      404 2024-03-19 12:19:44.945056 django_utilsds-0.5.2/.idea/django-utilsds.iml
--rw-r--r--   0        0        0      174 2024-03-19 12:19:44.955607 django_utilsds-0.5.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      419 2024-03-19 12:29:45.901640 django_utilsds-0.5.2/.idea/misc.xml
--rw-r--r--   0        0        0      280 2024-03-19 12:19:44.950172 django_utilsds-0.5.2/.idea/modules.xml
--rw-r--r--   0        0        0      167 2024-03-19 12:19:44.957383 django_utilsds-0.5.2/.idea/vcs.xml
--rw-r--r--   0        0        0     1079 2024-03-17 02:01:04.369747 django_utilsds-0.5.2/LICENSE
--rw-r--r--   0        0        0     1068 2024-04-21 07:20:18.847459 django_utilsds-0.5.2/README.md
--rw-r--r--   0        0        0        0 2024-03-19 12:26:04.845135 django_utilsds-0.5.2/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 12:26:04.845135 django_utilsds-0.5.2/django_utilsds/__init__.py
--rw-r--r--   0        0        0       63 2024-03-19 12:26:04.845706 django_utilsds-0.5.2/django_utilsds/admin.py
--rw-r--r--   0        0        0      159 2024-03-19 12:29:42.988859 django_utilsds-0.5.2/django_utilsds/apps.py
--rw-r--r--   0        0        0        0 2024-03-19 12:26:04.847399 django_utilsds-0.5.2/django_utilsds/migrations/__init__.py
--rw-r--r--   0        0        0       57 2024-03-19 12:26:04.847124 django_utilsds-0.5.2/django_utilsds/models.py
--rw-r--r--   0        0        0      520 2024-04-21 04:44:19.962450 django_utilsds-0.5.2/django_utilsds/templatetags/django_utilsds_tags.py
--rw-r--r--   0        0        0       60 2024-03-19 12:26:04.847256 django_utilsds-0.5.2/django_utilsds/tests.py
--rw-r--r--   0        0        0     1824 2024-03-19 06:52:37.021339 django_utilsds-0.5.2/django_utilsds/utils.py
--rw-r--r--   0        0        0       63 2024-03-19 12:26:04.845433 django_utilsds-0.5.2/django_utilsds/views.py
--rw-r--r--   0        0        0      581 2024-04-24 01:51:50.905059 django_utilsds-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     1382 1970-01-01 00:00:00.000000 django_utilsds-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     8196 2024-05-04 12:17:20.255320 django_utilsds-0.6.0/.DS_Store
+-rw-r--r--   0        0        0       66 2024-03-19 12:18:20.163079 django_utilsds-0.6.0/.gitattributes
+-rw-r--r--   0        0        0       18 2024-05-07 00:28:42.970789 django_utilsds-0.6.0/.gitignore
+-rw-r--r--   0        0        0       52 2024-03-19 12:19:45.020079 django_utilsds-0.6.0/.idea/.gitignore
+-rw-r--r--   0        0        0      404 2024-03-19 12:19:44.945056 django_utilsds-0.6.0/.idea/django-utilsds.iml
+-rw-r--r--   0        0        0      174 2024-03-19 12:19:44.955607 django_utilsds-0.6.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      419 2024-03-19 12:29:45.901640 django_utilsds-0.6.0/.idea/misc.xml
+-rw-r--r--   0        0        0      280 2024-03-19 12:19:44.950172 django_utilsds-0.6.0/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2024-03-19 12:19:44.957383 django_utilsds-0.6.0/.idea/vcs.xml
+-rw-r--r--   0        0        0     1079 2024-03-17 02:01:04.369747 django_utilsds-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1198 2024-05-16 02:44:33.500539 django_utilsds-0.6.0/README.md
+-rw-r--r--   0        0        0        0 2024-03-19 12:26:04.845135 django_utilsds-0.6.0/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-19 12:26:04.845135 django_utilsds-0.6.0/django_utilsds/__init__.py
+-rw-r--r--   0        0        0       63 2024-03-19 12:26:04.845706 django_utilsds-0.6.0/django_utilsds/admin.py
+-rw-r--r--   0        0        0      159 2024-03-19 12:29:42.988859 django_utilsds-0.6.0/django_utilsds/apps.py
+-rw-r--r--   0        0        0        0 2024-03-19 12:26:04.847399 django_utilsds-0.6.0/django_utilsds/migrations/__init__.py
+-rw-r--r--   0        0        0       57 2024-03-19 12:26:04.847124 django_utilsds-0.6.0/django_utilsds/models.py
+-rw-r--r--   0        0        0     1370 2024-05-16 03:10:43.224733 django_utilsds-0.6.0/django_utilsds/templatetags/django_utilsds_tags.py
+-rw-r--r--   0        0        0       60 2024-03-19 12:26:04.847256 django_utilsds-0.6.0/django_utilsds/tests.py
+-rw-r--r--   0        0        0     1824 2024-03-19 06:52:37.021339 django_utilsds-0.6.0/django_utilsds/utils.py
+-rw-r--r--   0        0        0       63 2024-03-19 12:26:04.845433 django_utilsds-0.6.0/django_utilsds/views.py
+-rw-r--r--   0        0        0      581 2024-05-16 03:11:59.330835 django_utilsds-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1512 1970-01-01 00:00:00.000000 django_utilsds-0.6.0/PKG-INFO
```

### Comparing `django_utilsds-0.5.2/LICENSE` & `django_utilsds-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_utilsds-0.5.2/README.md` & `django_utilsds-0.6.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -34,14 +34,20 @@
 html 파일 내에서 다음 코드를 삽입하여 사용한다.  
 ```html  
 {% load django_utilsds_tags %}
 {{ "test/utils/app"|split:"/" }}
 -> ['test', 'utils', 'app']
 ```
 
+```html 
+{% load django_utilsds_tags %}
+{{ "서울시 구로구 새말로"|add_br:"2" }}
+-> 서울시 구로구<br>새말로
+```
+
 ```html
 {% load django_utilsds_tags %}
 {{ "test_utils_app"|underscore_to_hypen }}
 -> test-utils-app
 ```  
 
 value 값을 / 을 단위로 나눠서 리스트 형식으로 반환한다.
```

### Comparing `django_utilsds-0.5.2/django_utilsds/utils.py` & `django_utilsds-0.6.0/django_utilsds/utils.py`

 * *Files identical despite different names*

### Comparing `django_utilsds-0.5.2/pyproject.toml` & `django_utilsds-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "django-utilsds"
-version = "0.5.2"
+version = "0.6.0"
 description = "One of the my demiansoft apps"
 authors = [{name = "Hyungjin Kim", email = "hj3415@gmail.com"}]
 license = {file = "LICENSE"}
 readme = "README.md"
 classifiers = ["License :: OSI Approved :: MIT License"]
 dependencies = [
     "Django >= 4.2.11",
```

### Comparing `django_utilsds-0.5.2/PKG-INFO` & `django_utilsds-0.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-utilsds
-Version: 0.5.2
+Version: 0.6.0
 Summary: One of the my demiansoft apps
 Author-email: Hyungjin Kim <hj3415@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: Django >= 4.2.11
 Project-URL: Home, https://www.demiansoft.com
 
@@ -44,14 +44,20 @@
 html 파일 내에서 다음 코드를 삽입하여 사용한다.  
 ```html  
 {% load django_utilsds_tags %}
 {{ "test/utils/app"|split:"/" }}
 -> ['test', 'utils', 'app']
 ```
 
+```html 
+{% load django_utilsds_tags %}
+{{ "서울시 구로구 새말로"|add_br:"2" }}
+-> 서울시 구로구<br>새말로
+```
+
 ```html
 {% load django_utilsds_tags %}
 {{ "test_utils_app"|underscore_to_hypen }}
 -> test-utils-app
 ```  
 
 value 값을 / 을 단위로 나눠서 리스트 형식으로 반환한다.
```

