# Comparing `tmp/django-easyjwt-0.4.3.tar.gz` & `tmp/django_easyjwt-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-easyjwt-0.4.3.tar", last modified: Tue Mar 19 09:07:03 2024, max compression
+gzip compressed data, was "django_easyjwt-0.4.4.tar", last modified: Wed May 15 22:40:18 2024, max compression
```

## Comparing `django-easyjwt-0.4.3.tar` & `django_easyjwt-0.4.4.tar`

### file list

```diff
@@ -1,86 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:07:03.867037 django-easyjwt-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    24259 2024-03-19 09:07:03.867037 django-easyjwt-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22744 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:07:03.863037 django-easyjwt-0.4.3/django_easyjwt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    24259 2024-03-19 09:07:03.000000 django-easyjwt-0.4.3/django_easyjwt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-03-19 09:07:03.000000 django-easyjwt-0.4.3/django_easyjwt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 09:07:03.000000 django-easyjwt-0.4.3/django_easyjwt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-19 09:07:03.000000 django-easyjwt-0.4.3/django_easyjwt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-19 09:07:03.000000 django-easyjwt-0.4.3/django_easyjwt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:07:03.855037 django-easyjwt-0.4.3/remotejwt_auth/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_auth/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     4933 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_auth/backends.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_auth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_auth/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_auth/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5438 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_auth/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_auth/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_auth/state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:07:03.855037 django-easyjwt-0.4.3/remotejwt_auth/token_blacklist/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_auth/token_blacklist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_auth/token_blacklist/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_auth/token_blacklist/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:07:03.855037 django-easyjwt-0.4.3/remotejwt_auth/token_blacklist/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_auth/token_blacklist/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:07:03.855037 django-easyjwt-0.4.3/remotejwt_auth/token_blacklist/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_auth/token_blacklist/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_auth/token_blacklist/management/commands/flushexpiredtokens.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:07:03.859037 django-easyjwt-0.4.3/remotejwt_auth/token_blacklist/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_auth/token_blacklist/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_auth/token_blacklist/migrations/0002_outstandingtoken_jti_hex.py
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_auth/token_blacklist/migrations/0003_auto_20171017_2007.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_auth/token_blacklist/migrations/0004_auto_20171017_2013.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_auth/token_blacklist/migrations/0005_remove_outstandingtoken_jti.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_auth/token_blacklist/migrations/0006_auto_20171017_2113.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_auth/token_blacklist/migrations/0007_auto_20171017_2214.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_auth/token_blacklist/migrations/0008_migrate_to_bigautofield.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_auth/token_blacklist/migrations/0010_fix_migrate_to_bigautofield.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_auth/token_blacklist/migrations/0011_linearizes_history.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_auth/token_blacklist/migrations/0012_alter_outstandingtoken_user.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_auth/token_blacklist/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_auth/token_blacklist/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    12181 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_auth/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_auth/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_auth/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_auth/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:07:03.859037 django-easyjwt-0.4.3/remotejwt_client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_client/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_client/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     7361 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_client/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_client/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_client/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_client/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_client/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:07:03.863037 django-easyjwt-0.4.3/remotejwt_client/tmp/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_client/tmp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_client/tmp/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_client/tmp/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_client/tmp/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_client/tmp/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_client/tmp/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_client/tmp/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_client/tmp/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_client/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_client/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_client/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:07:03.863037 django-easyjwt-0.4.3/remotejwt_user/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_user/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_user/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:07:03.863037 django-easyjwt-0.4.3/remotejwt_user/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_user/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_user/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9110 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_user/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_user/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_user/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_user/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_user/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_user/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/remotejwt_user/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-03-19 09:07:03.867037 django-easyjwt-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-19 09:06:59.000000 django-easyjwt-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:40:18.184773 django_easyjwt-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    24259 2024-05-15 22:40:18.184773 django_easyjwt-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22744 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:40:18.184773 django_easyjwt-0.4.4/django_easyjwt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    24259 2024-05-15 22:40:18.000000 django_easyjwt-0.4.4/django_easyjwt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-15 22:40:18.000000 django_easyjwt-0.4.4/django_easyjwt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 22:40:18.000000 django_easyjwt-0.4.4/django_easyjwt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-15 22:40:18.000000 django_easyjwt-0.4.4/django_easyjwt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-15 22:40:18.000000 django_easyjwt-0.4.4/django_easyjwt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:40:18.176772 django_easyjwt-0.4.4/remotejwt_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_auth/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4933 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_auth/backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_auth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_auth/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_auth/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5438 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_auth/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_auth/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_auth/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:40:18.176772 django_easyjwt-0.4.4/remotejwt_auth/token_blacklist/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_auth/token_blacklist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_auth/token_blacklist/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_auth/token_blacklist/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:40:18.176772 django_easyjwt-0.4.4/remotejwt_auth/token_blacklist/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_auth/token_blacklist/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:40:18.176772 django_easyjwt-0.4.4/remotejwt_auth/token_blacklist/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_auth/token_blacklist/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_auth/token_blacklist/management/commands/flushexpiredtokens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:40:18.180772 django_easyjwt-0.4.4/remotejwt_auth/token_blacklist/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_auth/token_blacklist/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_auth/token_blacklist/migrations/0002_outstandingtoken_jti_hex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_auth/token_blacklist/migrations/0003_auto_20171017_2007.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_auth/token_blacklist/migrations/0004_auto_20171017_2013.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_auth/token_blacklist/migrations/0005_remove_outstandingtoken_jti.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_auth/token_blacklist/migrations/0006_auto_20171017_2113.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_auth/token_blacklist/migrations/0007_auto_20171017_2214.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_auth/token_blacklist/migrations/0008_migrate_to_bigautofield.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_auth/token_blacklist/migrations/0010_fix_migrate_to_bigautofield.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_auth/token_blacklist/migrations/0011_linearizes_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_auth/token_blacklist/migrations/0012_alter_outstandingtoken_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_auth/token_blacklist/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_auth/token_blacklist/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12181 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_auth/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_auth/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_auth/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_auth/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:40:18.180772 django_easyjwt-0.4.4/remotejwt_client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_client/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_client/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7361 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_client/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_client/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_client/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_client/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_client/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:40:18.184773 django_easyjwt-0.4.4/remotejwt_client/tmp/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_client/tmp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_client/tmp/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_client/tmp/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_client/tmp/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_client/tmp/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_client/tmp/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_client/tmp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_client/tmp/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_client/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_client/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/remotejwt_client/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-15 22:40:18.184773 django_easyjwt-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-15 22:40:14.000000 django_easyjwt-0.4.4/setup.py
```

### Comparing `django-easyjwt-0.4.3/LICENCE` & `django_easyjwt-0.4.4/LICENCE`

 * *Files identical despite different names*

### Comparing `django-easyjwt-0.4.3/PKG-INFO` & `django_easyjwt-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-easyjwt
-Version: 0.4.3
+Version: 0.4.4
 Summary: A convenient package for building both client and server implementations for JWTs or Json Web Tokens. It allows you to build either side by only including the module you need and includes an optional custom user model.
 Home-page: https://github.com/garrethcain/django-easyjwt
 Author: Garreth Cain
 Author-email: garrethccain@gmail.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE
 Requires-Dist: Django>=3.2
 Requires-Dist: djangorestframework>=3.12.4
 Requires-Dist: requests>=2.24.0
 Requires-Dist: PyJWT>=2.8.0
 Requires-Dist: jwt>=1.3.1
```

### Comparing `django-easyjwt-0.4.3/README.md` & `django_easyjwt-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `django-easyjwt-0.4.3/django_easyjwt.egg-info/PKG-INFO` & `django_easyjwt-0.4.4/django_easyjwt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-easyjwt
-Version: 0.4.3
+Version: 0.4.4
 Summary: A convenient package for building both client and server implementations for JWTs or Json Web Tokens. It allows you to build either side by only including the module you need and includes an optional custom user model.
 Home-page: https://github.com/garrethcain/django-easyjwt
 Author: Garreth Cain
 Author-email: garrethccain@gmail.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE
 Requires-Dist: Django>=3.2
 Requires-Dist: djangorestframework>=3.12.4
 Requires-Dist: requests>=2.24.0
 Requires-Dist: PyJWT>=2.8.0
 Requires-Dist: jwt>=1.3.1
```

### Comparing `django-easyjwt-0.4.3/django_easyjwt.egg-info/SOURCES.txt` & `django_easyjwt-0.4.4/django_easyjwt.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -55,20 +55,8 @@
 remotejwt_client/tmp/__init__.py
 remotejwt_client/tmp/authentication.py
 remotejwt_client/tmp/py.typed
 remotejwt_client/tmp/serializers.py
 remotejwt_client/tmp/settings.py
 remotejwt_client/tmp/state.py
 remotejwt_client/tmp/utils.py
-remotejwt_client/tmp/views.py
-remotejwt_user/__init__.py
-remotejwt_user/admin.py
-remotejwt_user/apps.py
-remotejwt_user/models.py
-remotejwt_user/permissions.py
-remotejwt_user/serializers.py
-remotejwt_user/settings.py
-remotejwt_user/tests.py
-remotejwt_user/urls.py
-remotejwt_user/views.py
-remotejwt_user/migrations/0001_initial.py
-remotejwt_user/migrations/__init__.py
+remotejwt_client/tmp/views.py
```

### Comparing `django-easyjwt-0.4.3/remotejwt_auth/authentication.py` & `django_easyjwt-0.4.4/remotejwt_auth/authentication.py`

 * *Files identical despite different names*

### Comparing `django-easyjwt-0.4.3/remotejwt_auth/backends.py` & `django_easyjwt-0.4.4/remotejwt_auth/backends.py`

 * *Files identical despite different names*

### Comparing `django-easyjwt-0.4.3/remotejwt_auth/exceptions.py` & `django_easyjwt-0.4.4/remotejwt_auth/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-easyjwt-0.4.3/remotejwt_auth/models.py` & `django_easyjwt-0.4.4/remotejwt_auth/models.py`

 * *Files identical despite different names*

### Comparing `django-easyjwt-0.4.3/remotejwt_auth/serializers.py` & `django_easyjwt-0.4.4/remotejwt_auth/serializers.py`

 * *Files identical despite different names*

### Comparing `django-easyjwt-0.4.3/remotejwt_auth/settings.py` & `django_easyjwt-0.4.4/remotejwt_auth/settings.py`

 * *Files identical despite different names*

### Comparing `django-easyjwt-0.4.3/remotejwt_auth/token_blacklist/admin.py` & `django_easyjwt-0.4.4/remotejwt_auth/token_blacklist/admin.py`

 * *Files identical despite different names*

### Comparing `django-easyjwt-0.4.3/remotejwt_auth/token_blacklist/migrations/0001_initial.py` & `django_easyjwt-0.4.4/remotejwt_auth/token_blacklist/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-easyjwt-0.4.3/remotejwt_auth/token_blacklist/migrations/0003_auto_20171017_2007.py` & `django_easyjwt-0.4.4/remotejwt_auth/token_blacklist/migrations/0003_auto_20171017_2007.py`

 * *Files identical despite different names*

### Comparing `django-easyjwt-0.4.3/remotejwt_auth/token_blacklist/migrations/0007_auto_20171017_2214.py` & `django_easyjwt-0.4.4/remotejwt_auth/token_blacklist/migrations/0007_auto_20171017_2214.py`

 * *Files identical despite different names*

### Comparing `django-easyjwt-0.4.3/remotejwt_auth/token_blacklist/migrations/0008_migrate_to_bigautofield.py` & `django_easyjwt-0.4.4/remotejwt_auth/token_blacklist/migrations/0008_migrate_to_bigautofield.py`

 * *Files identical despite different names*

### Comparing `django-easyjwt-0.4.3/remotejwt_auth/token_blacklist/migrations/0010_fix_migrate_to_bigautofield.py` & `django_easyjwt-0.4.4/remotejwt_auth/token_blacklist/migrations/0010_fix_migrate_to_bigautofield.py`

 * *Files identical despite different names*

### Comparing `django-easyjwt-0.4.3/remotejwt_auth/token_blacklist/migrations/0011_linearizes_history.py` & `django_easyjwt-0.4.4/remotejwt_auth/token_blacklist/migrations/0011_linearizes_history.py`

 * *Files identical despite different names*

### Comparing `django-easyjwt-0.4.3/remotejwt_auth/token_blacklist/migrations/0012_alter_outstandingtoken_user.py` & `django_easyjwt-0.4.4/remotejwt_auth/token_blacklist/migrations/0012_alter_outstandingtoken_user.py`

 * *Files identical despite different names*

### Comparing `django-easyjwt-0.4.3/remotejwt_auth/token_blacklist/models.py` & `django_easyjwt-0.4.4/remotejwt_auth/token_blacklist/models.py`

 * *Files identical despite different names*

### Comparing `django-easyjwt-0.4.3/remotejwt_auth/tokens.py` & `django_easyjwt-0.4.4/remotejwt_auth/tokens.py`

 * *Files identical despite different names*

### Comparing `django-easyjwt-0.4.3/remotejwt_auth/utils.py` & `django_easyjwt-0.4.4/remotejwt_auth/utils.py`

 * *Files identical despite different names*

### Comparing `django-easyjwt-0.4.3/remotejwt_auth/views.py` & `django_easyjwt-0.4.4/remotejwt_auth/views.py`

 * *Files identical despite different names*

### Comparing `django-easyjwt-0.4.3/remotejwt_client/authentication.py` & `django_easyjwt-0.4.4/remotejwt_client/authentication.py`

 * *Files identical despite different names*

### Comparing `django-easyjwt-0.4.3/remotejwt_client/serializers.py` & `django_easyjwt-0.4.4/remotejwt_client/serializers.py`

 * *Files identical despite different names*

### Comparing `django-easyjwt-0.4.3/remotejwt_client/settings.py` & `django_easyjwt-0.4.4/remotejwt_client/settings.py`

 * *Files identical despite different names*

### Comparing `django-easyjwt-0.4.3/remotejwt_client/tmp/authentication.py` & `django_easyjwt-0.4.4/remotejwt_client/tmp/authentication.py`

 * *Files identical despite different names*

### Comparing `django-easyjwt-0.4.3/remotejwt_client/tmp/serializers.py` & `django_easyjwt-0.4.4/remotejwt_client/tmp/serializers.py`

 * *Files identical despite different names*

### Comparing `django-easyjwt-0.4.3/remotejwt_client/tmp/settings.py` & `django_easyjwt-0.4.4/remotejwt_client/tmp/settings.py`

 * *Files identical despite different names*

### Comparing `django-easyjwt-0.4.3/remotejwt_client/tmp/utils.py` & `django_easyjwt-0.4.4/remotejwt_client/tmp/utils.py`

 * *Files identical despite different names*

### Comparing `django-easyjwt-0.4.3/remotejwt_client/tmp/views.py` & `django_easyjwt-0.4.4/remotejwt_client/tmp/views.py`

 * *Files identical despite different names*

### Comparing `django-easyjwt-0.4.3/remotejwt_client/utils.py` & `django_easyjwt-0.4.4/remotejwt_client/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,14 @@
             raise exceptions.AuthenticationFailed(response.text)
 
         user_dict = response.json()
         user_id = user_dict.pop("id")
         try:
             # Use a custom serializer?
             try:
-                print("&&&&&")
                 serializer = import_string(api_settings.USER_MODEL_SERIALIZER)
                 s = serializer(
                     data=user_dict,
                     context={
                         "user_id_field": settings.REMOTE_JWT["USER_ID_CLAIM"],
                         "raw_data": user_dict,
                     },
```

### Comparing `django-easyjwt-0.4.3/remotejwt_client/views.py` & `django_easyjwt-0.4.4/remotejwt_client/views.py`

 * *Files identical despite different names*

### Comparing `django-easyjwt-0.4.3/setup.cfg` & `django_easyjwt-0.4.4/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-easyjwt
-version = 0.4.3
+version = 0.4.4
 description = A convenient package for building both client and server implementations for JWTs or Json Web Tokens. It allows you to build either side by only including the module you need and includes an optional custom user model.
 long_description = file: README.md
 long_description_content_type = text/markdown
 readme = "README.md"
 url = https://github.com/garrethcain/django-easyjwt
 author = Garreth Cain
 author_email = garrethccain@gmail.com
@@ -28,15 +28,15 @@
 	Programming Language :: Python :: 3.12
 	Topic :: Internet :: WWW/HTTP
 	Topic :: Internet :: WWW/HTTP :: Dynamic Content
 
 [options]
 include_package_data = true
 packages = find:
-python_requires = >=3.6
+python_requires = >=3.8
 install_requires = 
 	Django >= 3.2
 	djangorestframework >= 3.12.4
 	requests >= 2.24.0
 	PyJWT >= 2.8.0
 	jwt >= 1.3.1
```

