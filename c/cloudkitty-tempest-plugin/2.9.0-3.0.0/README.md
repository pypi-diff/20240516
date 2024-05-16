# Comparing `tmp/cloudkitty_tempest_plugin-2.9.0.tar.gz` & `tmp/cloudkitty_tempest_plugin-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudkitty_tempest_plugin-2.9.0.tar", last modified: Thu Mar 21 10:06:18 2024, max compression
+gzip compressed data, was "cloudkitty_tempest_plugin-3.0.0.tar", last modified: Thu May 16 12:46:21 2024, max compression
```

## Comparing `cloudkitty_tempest_plugin-2.9.0.tar` & `cloudkitty_tempest_plugin-3.0.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:06:18.639623 cloudkitty_tempest_plugin-2.9.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2024-03-21 10:05:49.000000 cloudkitty_tempest_plugin-2.9.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2024-03-21 10:05:49.000000 cloudkitty_tempest_plugin-2.9.0/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2024-03-21 10:05:49.000000 cloudkitty_tempest_plugin-2.9.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1228 2024-03-21 10:05:49.000000 cloudkitty_tempest_plugin-2.9.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      975 2024-03-21 10:06:18.000000 cloudkitty_tempest_plugin-2.9.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      673 2024-03-21 10:05:49.000000 cloudkitty_tempest_plugin-2.9.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2129 2024-03-21 10:06:18.000000 cloudkitty_tempest_plugin-2.9.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2024-03-21 10:05:49.000000 cloudkitty_tempest_plugin-2.9.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-03-21 10:05:49.000000 cloudkitty_tempest_plugin-2.9.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2580 2024-03-21 10:06:18.639623 cloudkitty_tempest_plugin-2.9.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1328 2024-03-21 10:05:49.000000 cloudkitty_tempest_plugin-2.9.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2024-03-21 10:05:49.000000 cloudkitty_tempest_plugin-2.9.0/babel.cfg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:06:18.635623 cloudkitty_tempest_plugin-2.9.0/cloudkitty_tempest_plugin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2024-03-21 10:05:49.000000 cloudkitty_tempest_plugin-2.9.0/cloudkitty_tempest_plugin/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:05:49.000000 cloudkitty_tempest_plugin-2.9.0/cloudkitty_tempest_plugin/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1296 2024-03-21 10:05:49.000000 cloudkitty_tempest_plugin-2.9.0/cloudkitty_tempest_plugin/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1449 2024-03-21 10:05:49.000000 cloudkitty_tempest_plugin-2.9.0/cloudkitty_tempest_plugin/plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:06:18.635623 cloudkitty_tempest_plugin-2.9.0/cloudkitty_tempest_plugin/services/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:05:49.000000 cloudkitty_tempest_plugin-2.9.0/cloudkitty_tempest_plugin/services/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18329 2024-03-21 10:05:49.000000 cloudkitty_tempest_plugin-2.9.0/cloudkitty_tempest_plugin/services/client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:06:18.635623 cloudkitty_tempest_plugin-2.9.0/cloudkitty_tempest_plugin/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:05:49.000000 cloudkitty_tempest_plugin-2.9.0/cloudkitty_tempest_plugin/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:06:18.635623 cloudkitty_tempest_plugin-2.9.0/cloudkitty_tempest_plugin/tests/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:05:49.000000 cloudkitty_tempest_plugin-2.9.0/cloudkitty_tempest_plugin/tests/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2859 2024-03-21 10:05:49.000000 cloudkitty_tempest_plugin-2.9.0/cloudkitty_tempest_plugin/tests/api/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:06:18.635623 cloudkitty_tempest_plugin-2.9.0/cloudkitty_tempest_plugin/tests/api/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:05:49.000000 cloudkitty_tempest_plugin-2.9.0/cloudkitty_tempest_plugin/tests/api/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6097 2024-03-21 10:05:49.000000 cloudkitty_tempest_plugin-2.9.0/cloudkitty_tempest_plugin/tests/api/v1/test_cloudkitty_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13357 2024-03-21 10:05:49.000000 cloudkitty_tempest_plugin-2.9.0/cloudkitty_tempest_plugin/tests/api/v1/test_hashmap_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3142 2024-03-21 10:05:49.000000 cloudkitty_tempest_plugin-2.9.0/cloudkitty_tempest_plugin/tests/api/v1/test_pyscript_api.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:06:18.635623 cloudkitty_tempest_plugin-2.9.0/cloudkitty_tempest_plugin/tests/api/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:05:49.000000 cloudkitty_tempest_plugin-2.9.0/cloudkitty_tempest_plugin/tests/api/v2/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:06:18.635623 cloudkitty_tempest_plugin-2.9.0/cloudkitty_tempest_plugin/tests/scenario/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:05:49.000000 cloudkitty_tempest_plugin-2.9.0/cloudkitty_tempest_plugin/tests/scenario/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:06:18.635623 cloudkitty_tempest_plugin-2.9.0/cloudkitty_tempest_plugin.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2580 2024-03-21 10:06:18.000000 cloudkitty_tempest_plugin-2.9.0/cloudkitty_tempest_plugin.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1346 2024-03-21 10:06:18.000000 cloudkitty_tempest_plugin-2.9.0/cloudkitty_tempest_plugin.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-21 10:06:18.000000 cloudkitty_tempest_plugin-2.9.0/cloudkitty_tempest_plugin.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2024-03-21 10:06:18.000000 cloudkitty_tempest_plugin-2.9.0/cloudkitty_tempest_plugin.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-21 10:06:18.000000 cloudkitty_tempest_plugin-2.9.0/cloudkitty_tempest_plugin.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-03-21 10:06:18.000000 cloudkitty_tempest_plugin-2.9.0/cloudkitty_tempest_plugin.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2024-03-21 10:06:18.000000 cloudkitty_tempest_plugin-2.9.0/cloudkitty_tempest_plugin.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       26 2024-03-21 10:06:18.000000 cloudkitty_tempest_plugin-2.9.0/cloudkitty_tempest_plugin.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:06:18.639623 cloudkitty_tempest_plugin-2.9.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2024-03-21 10:05:49.000000 cloudkitty_tempest_plugin-2.9.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:06:18.631623 cloudkitty_tempest_plugin-2.9.0/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:06:18.639623 cloudkitty_tempest_plugin-2.9.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1957 2024-03-21 10:05:49.000000 cloudkitty_tempest_plugin-2.9.0/doc/source/contributor/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      412 2024-03-21 10:05:49.000000 cloudkitty_tempest_plugin-2.9.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      902 2024-03-21 10:06:18.639623 cloudkitty_tempest_plugin-2.9.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2024-03-21 10:05:49.000000 cloudkitty_tempest_plugin-2.9.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      563 2024-03-21 10:05:49.000000 cloudkitty_tempest_plugin-2.9.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1058 2024-03-21 10:05:49.000000 cloudkitty_tempest_plugin-2.9.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:46:21.059832 cloudkitty_tempest_plugin-3.0.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2024-05-16 12:45:16.000000 cloudkitty_tempest_plugin-3.0.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2024-05-16 12:45:16.000000 cloudkitty_tempest_plugin-3.0.0/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2024-05-16 12:45:16.000000 cloudkitty_tempest_plugin-3.0.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1492 2024-05-16 12:45:16.000000 cloudkitty_tempest_plugin-3.0.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      975 2024-05-16 12:46:20.000000 cloudkitty_tempest_plugin-3.0.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      673 2024-05-16 12:45:16.000000 cloudkitty_tempest_plugin-3.0.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2223 2024-05-16 12:46:20.000000 cloudkitty_tempest_plugin-3.0.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2024-05-16 12:45:16.000000 cloudkitty_tempest_plugin-3.0.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-05-16 12:45:16.000000 cloudkitty_tempest_plugin-3.0.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2582 2024-05-16 12:46:21.059832 cloudkitty_tempest_plugin-3.0.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1328 2024-05-16 12:45:16.000000 cloudkitty_tempest_plugin-3.0.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2024-05-16 12:45:16.000000 cloudkitty_tempest_plugin-3.0.0/babel.cfg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:46:21.055832 cloudkitty_tempest_plugin-3.0.0/cloudkitty_tempest_plugin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2024-05-16 12:45:16.000000 cloudkitty_tempest_plugin-3.0.0/cloudkitty_tempest_plugin/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:45:16.000000 cloudkitty_tempest_plugin-3.0.0/cloudkitty_tempest_plugin/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1296 2024-05-16 12:45:16.000000 cloudkitty_tempest_plugin-3.0.0/cloudkitty_tempest_plugin/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1449 2024-05-16 12:45:16.000000 cloudkitty_tempest_plugin-3.0.0/cloudkitty_tempest_plugin/plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:46:21.055832 cloudkitty_tempest_plugin-3.0.0/cloudkitty_tempest_plugin/services/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:45:16.000000 cloudkitty_tempest_plugin-3.0.0/cloudkitty_tempest_plugin/services/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18329 2024-05-16 12:45:16.000000 cloudkitty_tempest_plugin-3.0.0/cloudkitty_tempest_plugin/services/client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:46:21.055832 cloudkitty_tempest_plugin-3.0.0/cloudkitty_tempest_plugin/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:45:16.000000 cloudkitty_tempest_plugin-3.0.0/cloudkitty_tempest_plugin/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:46:21.059832 cloudkitty_tempest_plugin-3.0.0/cloudkitty_tempest_plugin/tests/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:45:16.000000 cloudkitty_tempest_plugin-3.0.0/cloudkitty_tempest_plugin/tests/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2859 2024-05-16 12:45:16.000000 cloudkitty_tempest_plugin-3.0.0/cloudkitty_tempest_plugin/tests/api/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:46:21.059832 cloudkitty_tempest_plugin-3.0.0/cloudkitty_tempest_plugin/tests/api/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:45:16.000000 cloudkitty_tempest_plugin-3.0.0/cloudkitty_tempest_plugin/tests/api/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6097 2024-05-16 12:45:16.000000 cloudkitty_tempest_plugin-3.0.0/cloudkitty_tempest_plugin/tests/api/v1/test_cloudkitty_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13357 2024-05-16 12:45:16.000000 cloudkitty_tempest_plugin-3.0.0/cloudkitty_tempest_plugin/tests/api/v1/test_hashmap_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3142 2024-05-16 12:45:16.000000 cloudkitty_tempest_plugin-3.0.0/cloudkitty_tempest_plugin/tests/api/v1/test_pyscript_api.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:46:21.059832 cloudkitty_tempest_plugin-3.0.0/cloudkitty_tempest_plugin/tests/api/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:45:16.000000 cloudkitty_tempest_plugin-3.0.0/cloudkitty_tempest_plugin/tests/api/v2/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:46:21.059832 cloudkitty_tempest_plugin-3.0.0/cloudkitty_tempest_plugin/tests/scenario/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:45:16.000000 cloudkitty_tempest_plugin-3.0.0/cloudkitty_tempest_plugin/tests/scenario/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:46:21.055832 cloudkitty_tempest_plugin-3.0.0/cloudkitty_tempest_plugin.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2582 2024-05-16 12:46:20.000000 cloudkitty_tempest_plugin-3.0.0/cloudkitty_tempest_plugin.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1346 2024-05-16 12:46:21.000000 cloudkitty_tempest_plugin-3.0.0/cloudkitty_tempest_plugin.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-16 12:46:20.000000 cloudkitty_tempest_plugin-3.0.0/cloudkitty_tempest_plugin.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2024-05-16 12:46:20.000000 cloudkitty_tempest_plugin-3.0.0/cloudkitty_tempest_plugin.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-16 12:46:20.000000 cloudkitty_tempest_plugin-3.0.0/cloudkitty_tempest_plugin.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2024-05-16 12:46:20.000000 cloudkitty_tempest_plugin-3.0.0/cloudkitty_tempest_plugin.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2024-05-16 12:46:20.000000 cloudkitty_tempest_plugin-3.0.0/cloudkitty_tempest_plugin.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       26 2024-05-16 12:46:20.000000 cloudkitty_tempest_plugin-3.0.0/cloudkitty_tempest_plugin.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:46:21.059832 cloudkitty_tempest_plugin-3.0.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2024-05-16 12:45:16.000000 cloudkitty_tempest_plugin-3.0.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:46:21.051832 cloudkitty_tempest_plugin-3.0.0/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:46:21.059832 cloudkitty_tempest_plugin-3.0.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1957 2024-05-16 12:45:16.000000 cloudkitty_tempest_plugin-3.0.0/doc/source/contributor/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      412 2024-05-16 12:45:16.000000 cloudkitty_tempest_plugin-3.0.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      904 2024-05-16 12:46:21.059832 cloudkitty_tempest_plugin-3.0.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2024-05-16 12:45:16.000000 cloudkitty_tempest_plugin-3.0.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      563 2024-05-16 12:45:16.000000 cloudkitty_tempest_plugin-3.0.0/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1058 2024-05-16 12:45:16.000000 cloudkitty_tempest_plugin-3.0.0/tox.ini
```

### Comparing `cloudkitty_tempest_plugin-2.9.0/.zuul.yaml` & `cloudkitty_tempest_plugin-3.0.0/.zuul.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -7,25 +7,32 @@
       jobs: &cloudkitty_tempest_jobs
         - cloudkitty-tempest-full-v2-storage-influxdb:
             voting: true
         - cloudkitty-tempest-full-v1-storage-sqlalchemy:
             voting: true
         - cloudkitty-tempest-full-v2-storage-elasticsearch:
             voting: true
+        - cloudkitty-tempest-full-v2-storage-influxdb-2024-1
         - cloudkitty-tempest-full-v2-storage-influxdb-2023-2
         - cloudkitty-tempest-full-v2-storage-influxdb-2023-1
         - cloudkitty-tempest-full-v2-storage-influxdb-zed
     gate:
       jobs: *cloudkitty_tempest_jobs
 
 - job:
+    name: cloudkitty-tempest-full-v2-storage-influxdb-2024-1
+    parent: cloudkitty-tempest-full-v2-storage-influxdb
+    nodeset: openstack-single-node-jammy
+    override-checkout: stable/2024.1
+
+- job:
     name: cloudkitty-tempest-full-v2-storage-influxdb-2023-2
     parent: cloudkitty-tempest-full-v2-storage-influxdb
     nodeset: openstack-single-node-jammy
-    override-checkout: stable/2023.1
+    override-checkout: stable/2023.2
 
 - job:
     name: cloudkitty-tempest-full-v2-storage-influxdb-2023-1
     parent: cloudkitty-tempest-full-v2-storage-influxdb
     nodeset: openstack-single-node-jammy
     override-checkout: stable/2023.1
```

### Comparing `cloudkitty_tempest_plugin-2.9.0/AUTHORS` & `cloudkitty_tempest_plugin-3.0.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `cloudkitty_tempest_plugin-2.9.0/CONTRIBUTING.rst` & `cloudkitty_tempest_plugin-3.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cloudkitty_tempest_plugin-2.9.0/ChangeLog` & `cloudkitty_tempest_plugin-3.0.0/ChangeLog`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 CHANGES
 =======
 
+3.0.0
+-----
+
+* Add stable/2024.1 jobs on master gate
+
 2.9.0
 -----
 
 * Remove six
 * Update stable branch testing
+* Update python classifier in setup.cfg
 
 2.8.0
 -----
 
 * Add stable/2023.1 jobs on master gate
 * Cleanup py27 support
```

### Comparing `cloudkitty_tempest_plugin-2.9.0/LICENSE` & `cloudkitty_tempest_plugin-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudkitty_tempest_plugin-2.9.0/PKG-INFO` & `cloudkitty_tempest_plugin-3.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cloudkitty_tempest_plugin
-Version: 2.9.0
+Version: 3.0.0
 Summary: Tempest plugin for CloudKitty
 Home-page: https://opendev.org/openstack/cloudkitty-tempest-plugin
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: =================================
         Tempest integration of CloudKitty
@@ -62,11 +62,11 @@
 Classifier: Environment :: OpenStack
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
```

### Comparing `cloudkitty_tempest_plugin-2.9.0/README.rst` & `cloudkitty_tempest_plugin-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `cloudkitty_tempest_plugin-2.9.0/cloudkitty_tempest_plugin/config.py` & `cloudkitty_tempest_plugin-3.0.0/cloudkitty_tempest_plugin/config.py`

 * *Files identical despite different names*

### Comparing `cloudkitty_tempest_plugin-2.9.0/cloudkitty_tempest_plugin/plugin.py` & `cloudkitty_tempest_plugin-3.0.0/cloudkitty_tempest_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `cloudkitty_tempest_plugin-2.9.0/cloudkitty_tempest_plugin/services/client.py` & `cloudkitty_tempest_plugin-3.0.0/cloudkitty_tempest_plugin/services/client.py`

 * *Files identical despite different names*

### Comparing `cloudkitty_tempest_plugin-2.9.0/cloudkitty_tempest_plugin/tests/api/base.py` & `cloudkitty_tempest_plugin-3.0.0/cloudkitty_tempest_plugin/tests/api/base.py`

 * *Files identical despite different names*

### Comparing `cloudkitty_tempest_plugin-2.9.0/cloudkitty_tempest_plugin/tests/api/v1/test_cloudkitty_api.py` & `cloudkitty_tempest_plugin-3.0.0/cloudkitty_tempest_plugin/tests/api/v1/test_cloudkitty_api.py`

 * *Files identical despite different names*

### Comparing `cloudkitty_tempest_plugin-2.9.0/cloudkitty_tempest_plugin/tests/api/v1/test_hashmap_api.py` & `cloudkitty_tempest_plugin-3.0.0/cloudkitty_tempest_plugin/tests/api/v1/test_hashmap_api.py`

 * *Files identical despite different names*

### Comparing `cloudkitty_tempest_plugin-2.9.0/cloudkitty_tempest_plugin/tests/api/v1/test_pyscript_api.py` & `cloudkitty_tempest_plugin-3.0.0/cloudkitty_tempest_plugin/tests/api/v1/test_pyscript_api.py`

 * *Files identical despite different names*

### Comparing `cloudkitty_tempest_plugin-2.9.0/cloudkitty_tempest_plugin.egg-info/PKG-INFO` & `cloudkitty_tempest_plugin-3.0.0/cloudkitty_tempest_plugin.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cloudkitty-tempest-plugin
-Version: 2.9.0
+Version: 3.0.0
 Summary: Tempest plugin for CloudKitty
 Home-page: https://opendev.org/openstack/cloudkitty-tempest-plugin
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: =================================
         Tempest integration of CloudKitty
@@ -62,11 +62,11 @@
 Classifier: Environment :: OpenStack
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
```

### Comparing `cloudkitty_tempest_plugin-2.9.0/cloudkitty_tempest_plugin.egg-info/SOURCES.txt` & `cloudkitty_tempest_plugin-3.0.0/cloudkitty_tempest_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudkitty_tempest_plugin-2.9.0/doc/source/contributor/contributing.rst` & `cloudkitty_tempest_plugin-3.0.0/doc/source/contributor/contributing.rst`

 * *Files identical despite different names*

### Comparing `cloudkitty_tempest_plugin-2.9.0/setup.cfg` & `cloudkitty_tempest_plugin-3.0.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 	Environment :: OpenStack
 	Intended Audience :: Information Technology
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: Apache Software License
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [files]
 packages = 
 	cloudkitty_tempest_plugin
 
 [entry_points]
 tempest.test_plugins =
```

### Comparing `cloudkitty_tempest_plugin-2.9.0/setup.py` & `cloudkitty_tempest_plugin-3.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `cloudkitty_tempest_plugin-2.9.0/test-requirements.txt` & `cloudkitty_tempest_plugin-3.0.0/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `cloudkitty_tempest_plugin-2.9.0/tox.ini` & `cloudkitty_tempest_plugin-3.0.0/tox.ini`

 * *Files identical despite different names*

