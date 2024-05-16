# Comparing `tmp/dfapp-0.0.1a0.tar.gz` & `tmp/dfapp-0.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfapp-0.0.1a0.tar", last modified: Tue May 14 06:17:21 2024, max compression
+gzip compressed data, was "dfapp-0.0.1a1.tar", max compression
```

## Comparing `dfapp-0.0.1a0.tar` & `dfapp-0.0.1a1.tar`

### file list

```diff
@@ -1,12 +1,8 @@
-drwxrwxr-x   0 avatar    (1000) avatar    (1000)        0 2024-05-14 06:17:21.872175 dfapp-0.0.1a0/
--rw-rw-r--   0 avatar    (1000) avatar    (1000)      231 2024-05-14 06:17:21.872175 dfapp-0.0.1a0/PKG-INFO
-drwxrwxr-x   0 avatar    (1000) avatar    (1000)        0 2024-05-14 06:17:21.872175 dfapp-0.0.1a0/dfapp/
--rw-rw-r--   0 avatar    (1000) avatar    (1000)        0 2024-04-28 10:55:59.000000 dfapp-0.0.1a0/dfapp/__init__.py
--rw-rw-r--   0 avatar    (1000) avatar    (1000)       39 2024-04-28 10:56:20.000000 dfapp-0.0.1a0/dfapp/hello.py
-drwxrwxr-x   0 avatar    (1000) avatar    (1000)        0 2024-05-14 06:17:21.872175 dfapp-0.0.1a0/dfapp.egg-info/
--rw-rw-r--   0 avatar    (1000) avatar    (1000)      231 2024-05-14 06:17:21.000000 dfapp-0.0.1a0/dfapp.egg-info/PKG-INFO
--rw-rw-r--   0 avatar    (1000) avatar    (1000)      157 2024-05-14 06:17:21.000000 dfapp-0.0.1a0/dfapp.egg-info/SOURCES.txt
--rw-rw-r--   0 avatar    (1000) avatar    (1000)        1 2024-05-14 06:17:21.000000 dfapp-0.0.1a0/dfapp.egg-info/dependency_links.txt
--rw-rw-r--   0 avatar    (1000) avatar    (1000)        6 2024-05-14 06:17:21.000000 dfapp-0.0.1a0/dfapp.egg-info/top_level.txt
--rw-rw-r--   0 avatar    (1000) avatar    (1000)       38 2024-05-14 06:17:21.872175 dfapp-0.0.1a0/setup.cfg
--rw-rw-r--   0 avatar    (1000) avatar    (1000)      387 2024-05-14 06:17:04.000000 dfapp-0.0.1a0/setup.py
+-rw-r--r--   0        0        0    11357 2024-05-16 06:33:06.956856 dfapp-0.0.1a1/LICENSE
+-rw-r--r--   0        0        0      330 2024-05-16 08:31:47.115008 dfapp-0.0.1a1/README.md
+-rw-r--r--   0        0        0     4031 2024-05-16 09:00:46.702570 dfapp-0.0.1a1/pyproject.toml
+-rw-r--r--   0        0        0       63 2024-05-16 06:04:00.296073 dfapp-0.0.1a1/src/backend/dfapp/version/__init__.py
+-rw-r--r--   0        0        0      261 2024-05-16 06:06:17.973384 dfapp-0.0.1a1/src/backend/dfapp/version/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      731 2024-05-16 06:06:17.973384 dfapp-0.0.1a1/src/backend/dfapp/version/__pycache__/version.cpython-311.pyc
+-rw-r--r--   0        0        0      324 2024-05-16 06:04:00.296073 dfapp-0.0.1a1/src/backend/dfapp/version/version.py
+-rw-r--r--   0        0        0     4004 1970-01-01 00:00:00.000000 dfapp-0.0.1a1/PKG-INFO
```

