# Comparing `tmp/hfutils-0.2.5.tar.gz` & `tmp/hfutils-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hfutils-0.2.5.tar", last modified: Mon May  6 15:38:51 2024, max compression
+gzip compressed data, was "hfutils-0.2.6.tar", last modified: Thu May 16 13:09:49 2024, max compression
```

## Comparing `hfutils-0.2.5.tar` & `hfutils-0.2.6.tar`

### file list

```diff
@@ -1,63 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:38:51.514883 hfutils-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-06 15:38:32.000000 hfutils-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-06 15:38:32.000000 hfutils-0.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10172 2024-05-06 15:38:51.514883 hfutils-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7166 2024-05-06 15:38:32.000000 hfutils-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:38:51.506883 hfutils-0.2.5/hfutils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:38:51.506883 hfutils-0.2.5/hfutils/archive/
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/archive/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/archive/rar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/archive/sevenz.py
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/archive/tar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/archive/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:38:51.506883 hfutils-0.2.5/hfutils/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/config/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:38:51.506883 hfutils-0.2.5/hfutils/entry/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/entry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/entry/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/entry/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/entry/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/entry/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/entry/ls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/entry/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/entry/whoami.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:38:51.510883 hfutils-0.2.5/hfutils/index/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11377 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/index/fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/index/hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/index/make.py
--rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/index/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:38:51.510883 hfutils-0.2.5/hfutils/operate/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/operate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/operate/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7528 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/operate/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/operate/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/operate/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:38:51.510883 hfutils-0.2.5/hfutils/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/utils/binary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (127)    15309 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/utils/irregular_repo.json
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/utils/temp.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/utils/tqdm_.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/utils/walk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:38:51.510883 hfutils-0.2.5/hfutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10172 2024-05-06 15:38:51.000000 hfutils-0.2.5/hfutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-06 15:38:51.000000 hfutils-0.2.5/hfutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 15:38:51.000000 hfutils-0.2.5/hfutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-06 15:38:51.000000 hfutils-0.2.5/hfutils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-06 15:38:51.000000 hfutils-0.2.5/hfutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-06 15:38:51.000000 hfutils-0.2.5/hfutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-06 15:38:32.000000 hfutils-0.2.5/requirements-7z.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-06 15:38:32.000000 hfutils-0.2.5/requirements-build.txt
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-06 15:38:32.000000 hfutils-0.2.5/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-06 15:38:32.000000 hfutils-0.2.5/requirements-rar.txt
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-06 15:38:32.000000 hfutils-0.2.5/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-06 15:38:32.000000 hfutils-0.2.5/requirements-transfer.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-06 15:38:32.000000 hfutils-0.2.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 15:38:51.514883 hfutils-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-06 15:38:32.000000 hfutils-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:09:49.808173 hfutils-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-16 13:09:28.000000 hfutils-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-16 13:09:28.000000 hfutils-0.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10172 2024-05-16 13:09:49.808173 hfutils-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7166 2024-05-16 13:09:28.000000 hfutils-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:09:49.796173 hfutils-0.2.6/hfutils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:09:49.800173 hfutils-0.2.6/hfutils/archive/
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/archive/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/archive/rar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/archive/sevenz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/archive/tar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/archive/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:09:49.800173 hfutils-0.2.6/hfutils/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/config/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:09:49.800173 hfutils-0.2.6/hfutils/entry/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/entry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/entry/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/entry/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/entry/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/entry/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/entry/ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/entry/ls_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/entry/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/entry/whoami.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:09:49.800173 hfutils-0.2.6/hfutils/index/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11377 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/index/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/index/hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/index/make.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/index/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:09:49.800173 hfutils-0.2.6/hfutils/operate/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/operate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/operate/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7528 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/operate/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/operate/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/operate/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:09:49.804173 hfutils-0.2.6/hfutils/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/utils/binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15309 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/utils/irregular_repo.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/utils/temp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/utils/tqdm_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-16 13:09:28.000000 hfutils-0.2.6/hfutils/utils/walk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:09:49.804173 hfutils-0.2.6/hfutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10172 2024-05-16 13:09:49.000000 hfutils-0.2.6/hfutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-16 13:09:49.000000 hfutils-0.2.6/hfutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 13:09:49.000000 hfutils-0.2.6/hfutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-16 13:09:49.000000 hfutils-0.2.6/hfutils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-16 13:09:49.000000 hfutils-0.2.6/hfutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-16 13:09:49.000000 hfutils-0.2.6/hfutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-16 13:09:28.000000 hfutils-0.2.6/requirements-7z.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-16 13:09:28.000000 hfutils-0.2.6/requirements-build.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-16 13:09:28.000000 hfutils-0.2.6/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-16 13:09:28.000000 hfutils-0.2.6/requirements-rar.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-16 13:09:28.000000 hfutils-0.2.6/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-16 13:09:28.000000 hfutils-0.2.6/requirements-transfer.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-16 13:09:28.000000 hfutils-0.2.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 13:09:49.808173 hfutils-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-16 13:09:28.000000 hfutils-0.2.6/setup.py
```

### Comparing `hfutils-0.2.5/LICENSE` & `hfutils-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.5/PKG-INFO` & `hfutils-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hfutils
-Version: 0.2.5
+Version: 0.2.6
 Summary: Useful utilities for huggingface
 Home-page: https://github.com/deepghs/hfutils
 Author: narugo1992
 Author-email: narugo992@gmail.com
 License: Apache License, Version 2.0
 Keywords: Utilities of images.
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,33 +23,16 @@
 Requires-Dist: hbutils>=0.9.0
 Requires-Dist: huggingface_hub>=0.22
 Requires-Dist: tqdm
 Requires-Dist: requests
 Requires-Dist: click>=7
 Requires-Dist: tzlocal
 Requires-Dist: natsort
-Provides-Extra: rar
-Requires-Dist: rarfile; extra == "rar"
-Provides-Extra: test
-Requires-Dist: coverage>=5; extra == "test"
-Requires-Dist: mock>=4.0.3; extra == "test"
-Requires-Dist: flake8~=3.5; extra == "test"
-Requires-Dist: testfixtures>=6.18.5; extra == "test"
-Requires-Dist: pytest~=6.2.5; extra == "test"
-Requires-Dist: pytest-cov~=3.0.0; extra == "test"
-Requires-Dist: pytest-mock~=3.6.1; extra == "test"
-Requires-Dist: pytest-xdist>=1.34.0; extra == "test"
-Requires-Dist: pytest-rerunfailures~=10.2; extra == "test"
-Requires-Dist: pytest-timeout~=2.0.2; extra == "test"
-Requires-Dist: pytest-benchmark~=3.4.0; extra == "test"
-Requires-Dist: easydict<2,>=1.7; extra == "test"
-Requires-Dist: testtools>=2; extra == "test"
-Requires-Dist: where>=1.0.2; extra == "test"
-Requires-Dist: responses>=0.20.0; extra == "test"
-Requires-Dist: natsort; extra == "test"
+Provides-Extra: build
+Requires-Dist: pyinstaller<5,>=4.7; extra == "build"
 Provides-Extra: doc
 Requires-Dist: Jinja2>=3.0.0; extra == "doc"
 Requires-Dist: sphinx>=3.2.0; extra == "doc"
 Requires-Dist: sphinx_rtd_theme>=0.4.3; extra == "doc"
 Requires-Dist: enum_tools>=0.9.0; extra == "doc"
 Requires-Dist: sphinx-toolbox; extra == "doc"
 Requires-Dist: plantumlcli>=0.0.2; extra == "doc"
@@ -62,20 +45,37 @@
 Requires-Dist: nbsphinx>=0.8.8; extra == "doc"
 Requires-Dist: ipython>=7.16.3; extra == "doc"
 Requires-Dist: psutil>=5.8.0; extra == "doc"
 Requires-Dist: ipykernel>=6.15; extra == "doc"
 Requires-Dist: py-cpuinfo>=8.0.0; extra == "doc"
 Requires-Dist: click>=7.0.0; extra == "doc"
 Requires-Dist: pandas; extra == "doc"
-Provides-Extra: build
-Requires-Dist: pyinstaller<5,>=4.7; extra == "build"
 Provides-Extra: 7z
 Requires-Dist: py7zr; extra == "7z"
 Provides-Extra: transfer
 Requires-Dist: hf-transfer; extra == "transfer"
+Provides-Extra: test
+Requires-Dist: coverage>=5; extra == "test"
+Requires-Dist: mock>=4.0.3; extra == "test"
+Requires-Dist: flake8~=3.5; extra == "test"
+Requires-Dist: testfixtures>=6.18.5; extra == "test"
+Requires-Dist: pytest~=6.2.5; extra == "test"
+Requires-Dist: pytest-cov~=3.0.0; extra == "test"
+Requires-Dist: pytest-mock~=3.6.1; extra == "test"
+Requires-Dist: pytest-xdist>=1.34.0; extra == "test"
+Requires-Dist: pytest-rerunfailures~=10.2; extra == "test"
+Requires-Dist: pytest-timeout~=2.0.2; extra == "test"
+Requires-Dist: pytest-benchmark~=3.4.0; extra == "test"
+Requires-Dist: easydict<2,>=1.7; extra == "test"
+Requires-Dist: testtools>=2; extra == "test"
+Requires-Dist: where>=1.0.2; extra == "test"
+Requires-Dist: responses>=0.20.0; extra == "test"
+Requires-Dist: natsort; extra == "test"
+Provides-Extra: rar
+Requires-Dist: rarfile; extra == "rar"
 
 # hfutils
 
 [![PyPI](https://img.shields.io/pypi/v/hfutils)](https://pypi.org/project/hfutils/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hfutils)
 ![Loc](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/narugo1992/b98a0fd1468c4858abf2a355bc9b4039/raw/loc.json)
 ![Comments](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/narugo1992/b98a0fd1468c4858abf2a355bc9b4039/raw/comments.json)
```

### Comparing `hfutils-0.2.5/README.md` & `hfutils-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.5/hfutils/archive/__init__.py` & `hfutils-0.2.6/hfutils/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.5/hfutils/archive/base.py` & `hfutils-0.2.6/hfutils/archive/base.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.5/hfutils/archive/rar.py` & `hfutils-0.2.6/hfutils/archive/rar.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.5/hfutils/archive/sevenz.py` & `hfutils-0.2.6/hfutils/archive/sevenz.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.5/hfutils/archive/tar.py` & `hfutils-0.2.6/hfutils/archive/tar.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.5/hfutils/archive/zip.py` & `hfutils-0.2.6/hfutils/archive/zip.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.5/hfutils/entry/base.py` & `hfutils-0.2.6/hfutils/entry/base.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.5/hfutils/entry/dispatch.py` & `hfutils-0.2.6/hfutils/entry/dispatch.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.5/hfutils/entry/download.py` & `hfutils-0.2.6/hfutils/entry/download.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.5/hfutils/entry/ls.py` & `hfutils-0.2.6/hfutils/entry/ls.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.5/hfutils/entry/upload.py` & `hfutils-0.2.6/hfutils/entry/upload.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.5/hfutils/entry/whoami.py` & `hfutils-0.2.6/hfutils/entry/whoami.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.5/hfutils/index/fetch.py` & `hfutils-0.2.6/hfutils/index/fetch.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.5/hfutils/index/hash.py` & `hfutils-0.2.6/hfutils/index/hash.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.5/hfutils/index/make.py` & `hfutils-0.2.6/hfutils/index/make.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.5/hfutils/index/validate.py` & `hfutils-0.2.6/hfutils/index/validate.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.5/hfutils/operate/base.py` & `hfutils-0.2.6/hfutils/operate/base.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.5/hfutils/operate/download.py` & `hfutils-0.2.6/hfutils/operate/download.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.5/hfutils/operate/upload.py` & `hfutils-0.2.6/hfutils/operate/upload.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.5/hfutils/operate/validate.py` & `hfutils-0.2.6/hfutils/operate/validate.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.5/hfutils/utils/binary.py` & `hfutils-0.2.6/hfutils/utils/binary.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.5/hfutils/utils/download.py` & `hfutils-0.2.6/hfutils/utils/download.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.5/hfutils/utils/irregular_repo.json` & `hfutils-0.2.6/hfutils/utils/irregular_repo.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9882352941176471%*

 * *Differences: {"'datasets'": "{insert: [(2, 'adv_glue'), (43, 'bigbench'), (48, 'biwi_kinect_head_pose'), (108, "*

 * *               "'conceptual_12m'), (109, 'conceptual_captions'), (113, 'conll2012_ontonotesv5'), "*

 * *               "(169, 'elkarhizketak'), (175, 'enwik8'), (180, 'ett'), (218, 'gsm8k'), (264, "*

 * *               "'imagenet-1k'), (265, 'imagenet_sketch'), (302, 'lccc'), (332, 'metashift'), (342, "*

 * *               "'monash_tsf'), (412, 'paws-x'), (445, 'quickdraw'), (461, "*

 * *               "'roman_urdu_hate_speech') […]*

```diff
@@ -1,11 +1,12 @@
 {
     "datasets": [
         "acronym_identification",
         "ade_corpus_v2",
+        "adv_glue",
         "aeslc",
         "afrikaans_ner_corpus",
         "ag_news",
         "air_dialogue",
         "ajgt_twitter_ar",
         "allegro_reviews",
         "allocine",
@@ -38,18 +39,20 @@
         "banking77",
         "bbaw_egyptian",
         "bbc_hindi_nli",
         "bc2gm_corpus",
         "best2009",
         "bible_para",
         "big_patent",
+        "bigbench",
         "billsum",
         "bing_coronavirus_query_set",
         "biomrc",
         "biosses",
+        "biwi_kinect_head_pose",
         "blended_skill_talk",
         "blog_authorship_corpus",
         "bn_hate_speech",
         "bnl_newspapers",
         "bookcorpus",
         "bookcorpusopen",
         "bprec",
@@ -101,17 +104,20 @@
         "code_x_glue_tc_text_to_code",
         "code_x_glue_tt_text_to_text",
         "com_qa",
         "common_language",
         "common_voice",
         "compguesswhat",
         "conceptnet5",
+        "conceptual_12m",
+        "conceptual_captions",
         "conll2000",
         "conll2002",
         "conll2003",
+        "conll2012_ontonotesv5",
         "conllpp",
         "consumer-finance-complaints",
         "conv_ai",
         "conv_ai_2",
         "conv_ai_3",
         "conv_questions",
         "cornell_movie_dialog",
@@ -159,23 +165,26 @@
         "ecb",
         "ecthr_cases",
         "eduge",
         "ehealth_kd",
         "electricity_load_diagrams",
         "eli5",
         "eli5_category",
+        "elkarhizketak",
         "emea",
         "emo",
         "emotone_ar",
         "empathetic_dialogues",
         "enriched_web_nlg",
+        "enwik8",
         "eraser_multi_rc",
         "esnli",
         "eth_py150_open",
         "ethos",
+        "ett",
         "eu_regulatory_ir",
         "eurlex",
         "euronews",
         "europa_eac_tm",
         "europa_ecdc_tm",
         "event2Mind",
         "evidence_infer_treatment",
@@ -205,14 +214,15 @@
         "glucose",
         "gnad10",
         "go_emotions",
         "gooaq",
         "google_wellformed_query",
         "grail_qa",
         "great_code",
+        "gsm8k",
         "guardian_authorship",
         "gutenberg_time",
         "hans",
         "hansards",
         "hard",
         "harem",
         "has_part",
@@ -250,14 +260,16 @@
         "id_newspapers_2018",
         "id_panl_bppt",
         "id_puisi",
         "igbo_english_machine_translation",
         "igbo_monolingual",
         "igbo_ner",
         "ilist",
+        "imagenet-1k",
+        "imagenet_sketch",
         "imdb_urdu_reviews",
         "imppres",
         "indic_glue",
         "indonli",
         "inquisitive_qg",
         "interpress_news_category_tr",
         "interpress_news_category_tr_lite",
@@ -286,14 +298,15 @@
         "kor_sae",
         "kor_sarcasm",
         "labr",
         "lama",
         "large_spanish_corpus",
         "laroseda",
         "lc_quad",
+        "lccc",
         "lener_br",
         "liar",
         "librispeech_asr",
         "librispeech_lm",
         "limit",
         "lince",
         "linnaeus",
@@ -315,23 +328,25 @@
         "mdd",
         "med_hop",
         "medal",
         "medical_dialog",
         "medical_questions_pairs",
         "menyo20k_mt",
         "meta_woz",
+        "metashift",
         "metooma",
         "metrec",
         "miam",
         "mkb",
         "mkqa",
         "mlqa",
         "mlsum",
         "mnist",
         "mocha",
+        "monash_tsf",
         "moroco",
         "movie_rationales",
         "mrqa",
         "ms_marco",
         "ms_terms",
         "msr_genomics_kbcomp",
         "msr_sqa",
@@ -392,16 +407,16 @@
         "opinosis",
         "orange_sum",
         "oscar",
         "para_crawl",
         "para_pat",
         "parsinlu_reading_comprehension",
         "pass",
-        "paws-x",
         "paws",
+        "paws-x",
         "pec",
         "peoples_daily_ner",
         "per_sent",
         "persian_ner",
         "pg19",
         "php",
         "pib",
@@ -426,14 +441,15 @@
         "qangaroo",
         "qanta",
         "qed",
         "qed_amara",
         "quac",
         "quail",
         "quarel",
+        "quickdraw",
         "quora",
         "quoref",
         "re_dial",
         "reasoning_bg",
         "recipe_nlg",
         "reclor",
         "red_caps",
@@ -441,20 +457,22 @@
         "refresd",
         "reuters21578",
         "riddle_sense",
         "ro_sent",
         "ro_sts",
         "ro_sts_parallel",
         "roman_urdu",
+        "roman_urdu_hate_speech",
         "ronec",
         "rotten_tomatoes",
         "samsum",
         "sanskrit_classic",
         "saudinewsnet",
         "sberquad",
+        "sbu_captions",
         "scan",
         "scb_mt_enth_2020",
         "scene_parse_150",
         "schema_guided_dstc8",
         "scielo",
         "scientific_papers",
         "search_qa",
@@ -526,30 +544,33 @@
         "ted_iwlst2013",
         "ted_multi",
         "ted_talks_iwslt",
         "telugu_books",
         "telugu_news",
         "tep_en_fa_para",
         "text2log",
+        "textvqa",
         "thai_toxicity_tweet",
         "thainer",
         "thaiqa_squad",
         "thaisum",
         "the_pile_books3",
         "the_pile_openwebtext2",
         "the_pile_stack_exchange",
         "tilde_model",
         "time_dial",
         "times_of_india_news_headlines",
         "timit_asr",
         "tlc",
         "tmu_gfm_dataset",
+        "tne",
         "told-br",
         "totto",
         "trec",
+        "truthful_qa",
         "tsac",
         "ttc4900",
         "tunizi",
         "tuple_ie",
         "turk",
         "turkic_xwmt",
         "turkish_movie_sentiment",
@@ -568,14 +589,15 @@
         "udhr",
         "um005",
         "universal_dependencies",
         "universal_morphologies",
         "urdu_fake_news",
         "urdu_sentiment_corpus",
         "vctk",
+        "visual_genome",
         "vivos",
         "web_nlg",
         "web_of_science",
         "web_questions",
         "weibo_ner",
         "wi_locness",
         "wider_face",
@@ -595,14 +617,15 @@
         "wiki_split",
         "wiki_summary",
         "wikiann",
         "wikicorpus",
         "wikihow",
         "wikipedia",
         "wikisql",
+        "wikitablequestions",
         "wikitext",
         "wikitext_tl39",
         "wili_2018",
         "wino_bias",
         "winograd_wsc",
         "winogrande",
         "wiqa",
@@ -628,35 +651,12 @@
         "yelp_polarity",
         "yelp_review_full",
         "yoruba_bbc_topics",
         "yoruba_gv_ner",
         "yoruba_text_c3",
         "yoruba_wordsim353",
         "youtube_caption_corrections",
-        "zest",
-        "elkarhizketak",
-        "wikitablequestions",
-        "conll2012_ontonotesv5",
-        "monash_tsf",
-        "roman_urdu_hate_speech",
-        "adv_glue",
-        "metashift",
-        "gsm8k",
-        "sbu_captions",
-        "conceptual_captions",
-        "conceptual_12m",
-        "visual_genome",
-        "imagenet-1k",
-        "tne",
-        "textvqa",
-        "ett",
-        "imagenet_sketch",
-        "biwi_kinect_head_pose",
-        "enwik8",
-        "truthful_qa",
-        "bigbench",
-        "quickdraw",
-        "lccc"
+        "zest"
     ],
     "models": [],
     "spaces": []
 }
```

### Comparing `hfutils-0.2.5/hfutils/utils/path.py` & `hfutils-0.2.6/hfutils/utils/path.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.5/hfutils/utils/temp.py` & `hfutils-0.2.6/hfutils/utils/temp.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.5/hfutils/utils/tqdm_.py` & `hfutils-0.2.6/hfutils/utils/tqdm_.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.5/hfutils/utils/walk.py` & `hfutils-0.2.6/hfutils/utils/walk.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.5/hfutils.egg-info/PKG-INFO` & `hfutils-0.2.6/hfutils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hfutils
-Version: 0.2.5
+Version: 0.2.6
 Summary: Useful utilities for huggingface
 Home-page: https://github.com/deepghs/hfutils
 Author: narugo1992
 Author-email: narugo992@gmail.com
 License: Apache License, Version 2.0
 Keywords: Utilities of images.
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,33 +23,16 @@
 Requires-Dist: hbutils>=0.9.0
 Requires-Dist: huggingface_hub>=0.22
 Requires-Dist: tqdm
 Requires-Dist: requests
 Requires-Dist: click>=7
 Requires-Dist: tzlocal
 Requires-Dist: natsort
-Provides-Extra: rar
-Requires-Dist: rarfile; extra == "rar"
-Provides-Extra: test
-Requires-Dist: coverage>=5; extra == "test"
-Requires-Dist: mock>=4.0.3; extra == "test"
-Requires-Dist: flake8~=3.5; extra == "test"
-Requires-Dist: testfixtures>=6.18.5; extra == "test"
-Requires-Dist: pytest~=6.2.5; extra == "test"
-Requires-Dist: pytest-cov~=3.0.0; extra == "test"
-Requires-Dist: pytest-mock~=3.6.1; extra == "test"
-Requires-Dist: pytest-xdist>=1.34.0; extra == "test"
-Requires-Dist: pytest-rerunfailures~=10.2; extra == "test"
-Requires-Dist: pytest-timeout~=2.0.2; extra == "test"
-Requires-Dist: pytest-benchmark~=3.4.0; extra == "test"
-Requires-Dist: easydict<2,>=1.7; extra == "test"
-Requires-Dist: testtools>=2; extra == "test"
-Requires-Dist: where>=1.0.2; extra == "test"
-Requires-Dist: responses>=0.20.0; extra == "test"
-Requires-Dist: natsort; extra == "test"
+Provides-Extra: build
+Requires-Dist: pyinstaller<5,>=4.7; extra == "build"
 Provides-Extra: doc
 Requires-Dist: Jinja2>=3.0.0; extra == "doc"
 Requires-Dist: sphinx>=3.2.0; extra == "doc"
 Requires-Dist: sphinx_rtd_theme>=0.4.3; extra == "doc"
 Requires-Dist: enum_tools>=0.9.0; extra == "doc"
 Requires-Dist: sphinx-toolbox; extra == "doc"
 Requires-Dist: plantumlcli>=0.0.2; extra == "doc"
@@ -62,20 +45,37 @@
 Requires-Dist: nbsphinx>=0.8.8; extra == "doc"
 Requires-Dist: ipython>=7.16.3; extra == "doc"
 Requires-Dist: psutil>=5.8.0; extra == "doc"
 Requires-Dist: ipykernel>=6.15; extra == "doc"
 Requires-Dist: py-cpuinfo>=8.0.0; extra == "doc"
 Requires-Dist: click>=7.0.0; extra == "doc"
 Requires-Dist: pandas; extra == "doc"
-Provides-Extra: build
-Requires-Dist: pyinstaller<5,>=4.7; extra == "build"
 Provides-Extra: 7z
 Requires-Dist: py7zr; extra == "7z"
 Provides-Extra: transfer
 Requires-Dist: hf-transfer; extra == "transfer"
+Provides-Extra: test
+Requires-Dist: coverage>=5; extra == "test"
+Requires-Dist: mock>=4.0.3; extra == "test"
+Requires-Dist: flake8~=3.5; extra == "test"
+Requires-Dist: testfixtures>=6.18.5; extra == "test"
+Requires-Dist: pytest~=6.2.5; extra == "test"
+Requires-Dist: pytest-cov~=3.0.0; extra == "test"
+Requires-Dist: pytest-mock~=3.6.1; extra == "test"
+Requires-Dist: pytest-xdist>=1.34.0; extra == "test"
+Requires-Dist: pytest-rerunfailures~=10.2; extra == "test"
+Requires-Dist: pytest-timeout~=2.0.2; extra == "test"
+Requires-Dist: pytest-benchmark~=3.4.0; extra == "test"
+Requires-Dist: easydict<2,>=1.7; extra == "test"
+Requires-Dist: testtools>=2; extra == "test"
+Requires-Dist: where>=1.0.2; extra == "test"
+Requires-Dist: responses>=0.20.0; extra == "test"
+Requires-Dist: natsort; extra == "test"
+Provides-Extra: rar
+Requires-Dist: rarfile; extra == "rar"
 
 # hfutils
 
 [![PyPI](https://img.shields.io/pypi/v/hfutils)](https://pypi.org/project/hfutils/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hfutils)
 ![Loc](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/narugo1992/b98a0fd1468c4858abf2a355bc9b4039/raw/loc.json)
 ![Comments](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/narugo1992/b98a0fd1468c4858abf2a355bc9b4039/raw/comments.json)
```

### Comparing `hfutils-0.2.5/hfutils.egg-info/SOURCES.txt` & `hfutils-0.2.6/hfutils.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 requirements-doc.txt
 requirements-rar.txt
 requirements-test.txt
 requirements-transfer.txt
 requirements.txt
 setup.py
 hfutils/__init__.py
+hfutils/__main__.py
 hfutils.egg-info/PKG-INFO
 hfutils.egg-info/SOURCES.txt
 hfutils.egg-info/dependency_links.txt
 hfutils.egg-info/entry_points.txt
 hfutils.egg-info/requires.txt
 hfutils.egg-info/top_level.txt
 hfutils/archive/__init__.py
@@ -26,14 +27,15 @@
 hfutils/config/meta.py
 hfutils/entry/__init__.py
 hfutils/entry/base.py
 hfutils/entry/cli.py
 hfutils/entry/dispatch.py
 hfutils/entry/download.py
 hfutils/entry/ls.py
+hfutils/entry/ls_repo.py
 hfutils/entry/upload.py
 hfutils/entry/whoami.py
 hfutils/index/__init__.py
 hfutils/index/fetch.py
 hfutils/index/hash.py
 hfutils/index/make.py
 hfutils/index/validate.py
```

### Comparing `hfutils-0.2.5/hfutils.egg-info/requires.txt` & `hfutils-0.2.6/hfutils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.5/setup.py` & `hfutils-0.2.6/setup.py`

 * *Files identical despite different names*

