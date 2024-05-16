# Comparing `tmp/ssec-2.0.0.tar.gz` & `tmp/ssec-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssec-2.0.0.tar", last modified: Thu Apr  7 12:07:05 2022, max compression
+gzip compressed data, was "ssec-3.0.0.tar", last modified: Thu May 16 10:04:25 2024, max compression
```

## Comparing `ssec-2.0.0.tar` & `ssec-3.0.0.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxrwxrwx   0        0        0        0 2022-04-07 12:07:05.775104 ssec-2.0.0/
--rw-rw-rw-   0        0        0     1093 2022-03-29 11:46:20.000000 ssec-2.0.0/LICENSE
--rw-rw-rw-   0        0        0     1969 2022-04-07 12:07:05.775104 ssec-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1179 2022-04-06 07:59:48.000000 ssec-2.0.0/README.md
--rw-rw-rw-   0        0        0       98 2022-03-29 12:37:18.000000 ssec-2.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-04-07 12:07:05.775476 ssec-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1255 2022-04-03 12:20:24.000000 ssec-2.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-04-07 12:07:05.743521 ssec-2.0.0/ssec/
--rw-rw-rw-   0        0        0    14920 2022-04-07 12:05:20.000000 ssec-2.0.0/ssec/__init__.py
--rw-rw-rw-   0        0        0      295 2022-04-07 12:00:12.000000 ssec-2.0.0/ssec/__metadata__.py
--rw-rw-rw-   0        0        0      550 2022-04-01 13:14:13.000000 ssec-2.0.0/ssec/utilities.py
-drwxrwxrwx   0        0        0        0 2022-04-07 12:07:05.774327 ssec-2.0.0/ssec.egg-info/
--rw-rw-rw-   0        0        0     1969 2022-04-07 12:07:05.000000 ssec-2.0.0/ssec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2022-04-07 12:07:05.000000 ssec-2.0.0/ssec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-07 12:07:05.000000 ssec-2.0.0/ssec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2022-04-07 12:07:05.000000 ssec-2.0.0/ssec.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2022-04-07 12:07:05.000000 ssec-2.0.0/ssec.egg-info/top_level.txt
+drwxr-xr-x   0 jbaudisch  (1000) jbaudisch  (1000)        0 2024-05-16 10:04:25.381546 ssec-3.0.0/
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)     1063 2024-05-06 10:30:34.000000 ssec-3.0.0/LICENSE
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)     7168 2024-05-16 10:04:25.381546 ssec-3.0.0/PKG-INFO
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)     5929 2024-05-15 12:02:38.000000 ssec-3.0.0/README.md
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)     3651 2024-05-16 09:57:32.000000 ssec-3.0.0/pyproject.toml
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)       38 2024-05-16 10:04:25.381546 ssec-3.0.0/setup.cfg
+drwxr-xr-x   0 jbaudisch  (1000) jbaudisch  (1000)        0 2024-05-16 10:04:25.381546 ssec-3.0.0/src/
+drwxr-xr-x   0 jbaudisch  (1000) jbaudisch  (1000)        0 2024-05-16 10:04:25.381546 ssec-3.0.0/src/ssec/
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)      117 2024-05-15 12:02:38.000000 ssec-3.0.0/src/ssec/__init__.py
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)     5292 2024-05-16 09:42:47.000000 ssec-3.0.0/src/ssec/common.py
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)     1187 2024-05-16 09:37:29.000000 ssec-3.0.0/src/ssec/constants.py
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)      384 2024-05-16 09:40:43.000000 ssec-3.0.0/src/ssec/event.py
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)       57 2024-05-15 12:02:38.000000 ssec-3.0.0/src/ssec/py.typed
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)     7115 2024-05-16 09:48:02.000000 ssec-3.0.0/src/ssec/stream.py
+drwxr-xr-x   0 jbaudisch  (1000) jbaudisch  (1000)        0 2024-05-16 10:04:25.381546 ssec-3.0.0/src/ssec.egg-info/
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)     7168 2024-05-16 10:04:25.000000 ssec-3.0.0/src/ssec.egg-info/PKG-INFO
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)      308 2024-05-16 10:04:25.000000 ssec-3.0.0/src/ssec.egg-info/SOURCES.txt
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)        1 2024-05-16 10:04:25.000000 ssec-3.0.0/src/ssec.egg-info/dependency_links.txt
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)      112 2024-05-16 10:04:25.000000 ssec-3.0.0/src/ssec.egg-info/requires.txt
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)        5 2024-05-16 10:04:25.000000 ssec-3.0.0/src/ssec.egg-info/top_level.txt
```

