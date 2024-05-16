# Comparing `tmp/django_xlsx_serializer-0.1.0.tar.gz` & `tmp/django_xlsx_serializer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_xlsx_serializer-0.1.0.tar", last modified: Thu May 16 14:11:17 2024, max compression
+gzip compressed data, was "django_xlsx_serializer-0.2.0.tar", last modified: Thu May 16 20:33:29 2024, max compression
```

## Comparing `django_xlsx_serializer-0.1.0.tar` & `django_xlsx_serializer-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:11:17.907904 django_xlsx_serializer-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-16 14:11:12.000000 django_xlsx_serializer-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-16 14:11:17.907904 django_xlsx_serializer-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-16 14:11:12.000000 django_xlsx_serializer-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-16 14:11:12.000000 django_xlsx_serializer-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 14:11:17.907904 django_xlsx_serializer-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:11:17.903904 django_xlsx_serializer-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:11:17.907904 django_xlsx_serializer-0.1.0/src/django_xlsx_serializer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-16 14:11:17.000000 django_xlsx_serializer-0.1.0/src/django_xlsx_serializer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-16 14:11:17.000000 django_xlsx_serializer-0.1.0/src/django_xlsx_serializer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 14:11:17.000000 django_xlsx_serializer-0.1.0/src/django_xlsx_serializer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-16 14:11:17.000000 django_xlsx_serializer-0.1.0/src/django_xlsx_serializer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-16 14:11:17.000000 django_xlsx_serializer-0.1.0/src/django_xlsx_serializer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:11:17.907904 django_xlsx_serializer-0.1.0/src/xlsx_serializer/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-16 14:11:12.000000 django_xlsx_serializer-0.1.0/src/xlsx_serializer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:33:29.594145 django_xlsx_serializer-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-16 20:33:20.000000 django_xlsx_serializer-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-16 20:33:29.594145 django_xlsx_serializer-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-16 20:33:20.000000 django_xlsx_serializer-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-05-16 20:33:20.000000 django_xlsx_serializer-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 20:33:29.594145 django_xlsx_serializer-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:33:29.590145 django_xlsx_serializer-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:33:29.590145 django_xlsx_serializer-0.2.0/src/django_xlsx_serializer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-16 20:33:29.000000 django_xlsx_serializer-0.2.0/src/django_xlsx_serializer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-16 20:33:29.000000 django_xlsx_serializer-0.2.0/src/django_xlsx_serializer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 20:33:29.000000 django_xlsx_serializer-0.2.0/src/django_xlsx_serializer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-16 20:33:29.000000 django_xlsx_serializer-0.2.0/src/django_xlsx_serializer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-16 20:33:29.000000 django_xlsx_serializer-0.2.0/src/django_xlsx_serializer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:33:29.590145 django_xlsx_serializer-0.2.0/src/xlsx_serializer/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-16 20:33:20.000000 django_xlsx_serializer-0.2.0/src/xlsx_serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 20:33:20.000000 django_xlsx_serializer-0.2.0/src/xlsx_serializer/py.typed
```

### Comparing `django_xlsx_serializer-0.1.0/LICENSE` & `django_xlsx_serializer-0.2.0/LICENSE`

 * *Files identical despite different names*

