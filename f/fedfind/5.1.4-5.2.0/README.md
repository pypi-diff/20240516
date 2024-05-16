# Comparing `tmp/fedfind-5.1.4.tar.gz` & `tmp/fedfind-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedfind-5.1.4.tar", last modified: Mon Apr 29 22:21:24 2024, max compression
+gzip compressed data, was "fedfind-5.2.0.tar", last modified: Thu May 16 21:19:56 2024, max compression
```

## Comparing `fedfind-5.1.4.tar` & `fedfind-5.2.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-04-29 22:21:24.606799 fedfind-5.1.4/
--rw-rw-r--   0 adamw     (1000) adamw     (1000)       86 2019-06-18 21:22:51.000000 fedfind-5.1.4/.gitignore
--rw-rw-r--   0 adamw     (1000) adamw     (1000)       29 2019-06-18 21:22:51.000000 fedfind-5.1.4/.pylintrc
--rw-r--r--   0 adamw     (1000) adamw     (1000)      143 2023-10-19 16:24:10.000000 fedfind-5.1.4/.zuul.yaml
--rw-r--r--   0 adamw     (1000) adamw     (1000)    39960 2024-04-29 22:20:45.000000 fedfind-5.1.4/CHANGELOG.md
--rw-rw-r--   0 adamw     (1000) adamw     (1000)    35147 2015-02-09 17:48:14.000000 fedfind-5.1.4/COPYING
--rw-rw-r--   0 adamw     (1000) adamw     (1000)       37 2019-06-18 21:22:51.000000 fedfind-5.1.4/MANIFEST.in
--rw-r--r--   0 adamw     (1000) adamw     (1000)    27819 2024-04-29 22:21:24.606799 fedfind-5.1.4/PKG-INFO
--rw-r--r--   0 adamw     (1000) adamw     (1000)    27184 2023-10-19 16:24:10.000000 fedfind-5.1.4/README.md
-drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-04-29 22:21:24.579800 fedfind-5.1.4/ci/
--rw-r--r--   0 adamw     (1000) adamw     (1000)      397 2023-10-19 16:24:10.000000 fedfind-5.1.4/ci/tox.yaml
--rwxr-xr-x   0 adamw     (1000) adamw     (1000)      251 2023-10-19 16:24:10.000000 fedfind-5.1.4/fedfindlocal.py
--rwxr-xr-x   0 adamw     (1000) adamw     (1000)     3811 2024-04-23 22:13:33.000000 fedfind-5.1.4/gen-allstable
--rw-r--r--   0 adamw     (1000) adamw     (1000)       62 2023-10-19 16:24:10.000000 fedfind-5.1.4/install.requires
--rw-r--r--   0 adamw     (1000) adamw     (1000)      334 2023-10-19 16:24:10.000000 fedfind-5.1.4/pyproject.toml
--rwxr-xr-x   0 adamw     (1000) adamw     (1000)      658 2023-10-19 16:24:10.000000 fedfind-5.1.4/release.sh
--rw-r--r--   0 adamw     (1000) adamw     (1000)       38 2024-04-29 22:21:24.606799 fedfind-5.1.4/setup.cfg
--rw-r--r--   0 adamw     (1000) adamw     (1000)     1899 2024-04-29 22:21:00.000000 fedfind-5.1.4/setup.py
-drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-04-29 22:21:24.578800 fedfind-5.1.4/src/
-drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-04-29 22:21:24.581800 fedfind-5.1.4/src/fedfind/
--rw-r--r--   0 adamw     (1000) adamw     (1000)      934 2024-04-29 22:21:00.000000 fedfind-5.1.4/src/fedfind/__init__.py
--rwxr-xr-x   0 adamw     (1000) adamw     (1000)    10744 2023-10-19 16:24:10.000000 fedfind-5.1.4/src/fedfind/cli.py
--rw-r--r--   0 adamw     (1000) adamw     (1000)     7151 2024-04-23 21:43:29.000000 fedfind-5.1.4/src/fedfind/const.py
--rw-r--r--   0 adamw     (1000) adamw     (1000)     2502 2023-10-19 16:24:10.000000 fedfind-5.1.4/src/fedfind/exceptions.py
--rw-r--r--   0 adamw     (1000) adamw     (1000)    32037 2024-04-23 22:42:03.000000 fedfind-5.1.4/src/fedfind/helpers.py
--rw-r--r--   0 adamw     (1000) adamw     (1000)    95897 2024-04-23 21:44:41.000000 fedfind-5.1.4/src/fedfind/release.py
-drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-04-29 22:21:24.606799 fedfind-5.1.4/src/fedfind.egg-info/
--rw-r--r--   0 adamw     (1000) adamw     (1000)    27819 2024-04-29 22:21:24.000000 fedfind-5.1.4/src/fedfind.egg-info/PKG-INFO
--rw-rw-r--   0 adamw     (1000) adamw     (1000)     1715 2024-04-29 22:21:24.000000 fedfind-5.1.4/src/fedfind.egg-info/SOURCES.txt
--rw-rw-r--   0 adamw     (1000) adamw     (1000)        1 2024-04-29 22:21:24.000000 fedfind-5.1.4/src/fedfind.egg-info/dependency_links.txt
--rw-rw-r--   0 adamw     (1000) adamw     (1000)       45 2024-04-29 22:21:24.000000 fedfind-5.1.4/src/fedfind.egg-info/entry_points.txt
--rw-rw-r--   0 adamw     (1000) adamw     (1000)       68 2024-04-29 22:21:24.000000 fedfind-5.1.4/src/fedfind.egg-info/requires.txt
--rw-rw-r--   0 adamw     (1000) adamw     (1000)        8 2024-04-29 22:21:24.000000 fedfind-5.1.4/src/fedfind.egg-info/top_level.txt
-drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-04-29 22:21:24.583799 fedfind-5.1.4/tests/
--rw-r--r--   0 adamw     (1000) adamw     (1000)     7488 2024-04-23 22:30:37.000000 fedfind-5.1.4/tests/conftest.py
-drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-04-29 22:21:24.601799 fedfind-5.1.4/tests/data/
--rw-r--r--   0 adamw     (1000) adamw     (1000)  1035277 2024-04-23 21:30:59.000000 fedfind-5.1.4/tests/data/allstable.json
--rw-r--r--   0 adamw     (1000) adamw     (1000)   293981 2024-04-23 22:34:02.000000 fedfind-5.1.4/tests/data/compose-urls-20240423.json
--rwxr-xr-x   0 adamw     (1000) adamw     (1000)     1437 2023-10-19 16:24:10.000000 fedfind-5.1.4/tests/data/fedfindloc.py
-drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-04-29 22:21:24.578800 fedfind-5.1.4/tests/data/http/
-drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-04-29 22:21:24.578800 fedfind-5.1.4/tests/data/http/pub/
-drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-04-29 22:21:24.602799 fedfind-5.1.4/tests/data/http/pub/alt/
--rw-r--r--   0 adamw     (1000) adamw     (1000)   215056 2024-04-23 22:42:42.000000 fedfind-5.1.4/tests/data/http/pub/alt/imagelist-alt
-drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-04-29 22:21:24.603799 fedfind-5.1.4/tests/data/http/pub/archive/
--rw-r--r--   0 adamw     (1000) adamw     (1000)   146475 2024-04-23 22:42:42.000000 fedfind-5.1.4/tests/data/http/pub/archive/imagelist-archive
-drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-04-29 22:21:24.605799 fedfind-5.1.4/tests/data/http/pub/fedora/
--rw-r--r--   0 adamw     (1000) adamw     (1000)    33469 2024-04-23 22:42:42.000000 fedfind-5.1.4/tests/data/http/pub/fedora/imagelist-fedora
--rw-rw-r--   0 adamw     (1000) adamw     (1000)    38788 2019-06-18 21:22:51.000000 fedfind-5.1.4/tests/data/pdc-compimages-Fedora-24-20160614.0.json
--rw-rw-r--   0 adamw     (1000) adamw     (1000)    43446 2019-06-18 21:22:51.000000 fedfind-5.1.4/tests/data/pdc-compimages-Fedora-25-20161115.0.json
--rw-rw-r--   0 adamw     (1000) adamw     (1000)    73734 2019-06-18 21:22:51.000000 fedfind-5.1.4/tests/data/pdc-compimages-Fedora-26-20170705.0.json
--rw-rw-r--   0 adamw     (1000) adamw     (1000)    70323 2019-06-18 21:22:51.000000 fedfind-5.1.4/tests/data/pdc-compimages-Fedora-27-20171105.0.json
--rw-r--r--   0 adamw     (1000) adamw     (1000)    81069 2023-10-19 16:24:10.000000 fedfind-5.1.4/tests/data/pdc-compimages-Fedora-28-20180425.0.json
--rw-r--r--   0 adamw     (1000) adamw     (1000)    59560 2023-10-19 16:24:10.000000 fedfind-5.1.4/tests/data/pdc-compimages-Fedora-29-20181024.1.json
--rw-r--r--   0 adamw     (1000) adamw     (1000)    61551 2023-10-19 16:24:10.000000 fedfind-5.1.4/tests/data/pdc-compimages-Fedora-30-20190425.0.json
--rw-r--r--   0 adamw     (1000) adamw     (1000)    57550 2023-10-19 16:24:10.000000 fedfind-5.1.4/tests/data/pdc-compimages-Fedora-31-20191023.0.json
--rw-r--r--   0 adamw     (1000) adamw     (1000)    59948 2023-10-19 16:24:10.000000 fedfind-5.1.4/tests/data/pdc-compimages-Fedora-32-20200422.0.json
--rw-r--r--   0 adamw     (1000) adamw     (1000)    65722 2023-10-19 16:24:10.000000 fedfind-5.1.4/tests/data/pdc-compimages-Fedora-33-20201019.0.json
--rw-r--r--   0 adamw     (1000) adamw     (1000)    63265 2023-10-19 16:24:10.000000 fedfind-5.1.4/tests/data/pdc-compimages-Fedora-34-20210423.0.json
--rw-r--r--   0 adamw     (1000) adamw     (1000)    66775 2023-10-19 16:24:10.000000 fedfind-5.1.4/tests/data/pdc-compimages-Fedora-35-20211026.0.json
--rw-r--r--   0 adamw     (1000) adamw     (1000)    65980 2023-10-19 16:24:10.000000 fedfind-5.1.4/tests/data/pdc-compimages-Fedora-36-20220504.1.json
--rw-r--r--   0 adamw     (1000) adamw     (1000)    27726 2023-10-19 16:24:10.000000 fedfind-5.1.4/tests/data/pdc-compimages-Fedora-37-20221105.0.json
--rw-r--r--   0 adamw     (1000) adamw     (1000)    29444 2023-10-19 16:24:10.000000 fedfind-5.1.4/tests/data/pdc-compimages-Fedora-38-20230413.1.json
--rw-r--r--   0 adamw     (1000) adamw     (1000)    64647 2024-04-23 22:28:11.000000 fedfind-5.1.4/tests/data/pdc-compimages-Fedora-39-20231031.1.json
--rw-r--r--   0 adamw     (1000) adamw     (1000)    70999 2024-04-23 22:26:25.000000 fedfind-5.1.4/tests/data/pdc-compimages-Fedora-40-20240414.0.json
--rw-r--r--   0 adamw     (1000) adamw     (1000)    29635 2023-10-19 16:24:10.000000 fedfind-5.1.4/tests/test_helpers.py
--rw-r--r--   0 adamw     (1000) adamw     (1000)    52324 2024-04-23 22:35:22.000000 fedfind-5.1.4/tests/test_release.py
--rw-r--r--   0 adamw     (1000) adamw     (1000)       58 2023-10-19 16:24:10.000000 fedfind-5.1.4/tests.requires
--rw-r--r--   0 adamw     (1000) adamw     (1000)      549 2023-10-19 16:24:10.000000 fedfind-5.1.4/tox.ini
--rw-r--r--   0 adamw     (1000) adamw     (1000)       39 2023-10-19 16:24:10.000000 fedfind-5.1.4/tox.requires
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-05-16 21:19:56.833216 fedfind-5.2.0/
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)       86 2019-06-18 21:22:51.000000 fedfind-5.2.0/.gitignore
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)       29 2019-06-18 21:22:51.000000 fedfind-5.2.0/.pylintrc
+-rw-r--r--   0 adamw     (1000) adamw     (1000)      143 2023-10-19 16:24:10.000000 fedfind-5.2.0/.zuul.yaml
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    40810 2024-05-16 21:18:41.000000 fedfind-5.2.0/CHANGELOG.md
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)    35147 2015-02-09 17:48:14.000000 fedfind-5.2.0/COPYING
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)       37 2019-06-18 21:22:51.000000 fedfind-5.2.0/MANIFEST.in
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    27819 2024-05-16 21:19:56.832216 fedfind-5.2.0/PKG-INFO
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    27184 2023-10-19 16:24:10.000000 fedfind-5.2.0/README.md
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-05-16 21:19:56.829216 fedfind-5.2.0/ci/
+-rw-r--r--   0 adamw     (1000) adamw     (1000)      397 2023-10-19 16:24:10.000000 fedfind-5.2.0/ci/tox.yaml
+-rwxr-xr-x   0 adamw     (1000) adamw     (1000)      251 2023-10-19 16:24:10.000000 fedfind-5.2.0/fedfindlocal.py
+-rwxr-xr-x   0 adamw     (1000) adamw     (1000)     3811 2024-04-23 22:13:33.000000 fedfind-5.2.0/gen-allstable
+-rw-r--r--   0 adamw     (1000) adamw     (1000)       62 2023-10-19 16:24:10.000000 fedfind-5.2.0/install.requires
+-rw-r--r--   0 adamw     (1000) adamw     (1000)      334 2023-10-19 16:24:10.000000 fedfind-5.2.0/pyproject.toml
+-rwxr-xr-x   0 adamw     (1000) adamw     (1000)      658 2023-10-19 16:24:10.000000 fedfind-5.2.0/release.sh
+-rw-r--r--   0 adamw     (1000) adamw     (1000)       38 2024-05-16 21:19:56.833216 fedfind-5.2.0/setup.cfg
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     1899 2024-05-16 21:19:34.000000 fedfind-5.2.0/setup.py
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-05-16 21:19:56.828216 fedfind-5.2.0/src/
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-05-16 21:19:56.829216 fedfind-5.2.0/src/fedfind/
+-rw-r--r--   0 adamw     (1000) adamw     (1000)      934 2024-05-16 21:19:34.000000 fedfind-5.2.0/src/fedfind/__init__.py
+-rwxr-xr-x   0 adamw     (1000) adamw     (1000)    10798 2024-05-16 20:33:22.000000 fedfind-5.2.0/src/fedfind/cli.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     7151 2024-04-23 21:43:29.000000 fedfind-5.2.0/src/fedfind/const.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     2502 2023-10-19 16:24:10.000000 fedfind-5.2.0/src/fedfind/exceptions.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    32015 2024-05-15 17:51:07.000000 fedfind-5.2.0/src/fedfind/helpers.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)   100735 2024-05-16 21:10:04.000000 fedfind-5.2.0/src/fedfind/release.py
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-05-16 21:19:56.832216 fedfind-5.2.0/src/fedfind.egg-info/
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    27819 2024-05-16 21:19:56.000000 fedfind-5.2.0/src/fedfind.egg-info/PKG-INFO
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)     1715 2024-05-16 21:19:56.000000 fedfind-5.2.0/src/fedfind.egg-info/SOURCES.txt
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)        1 2024-05-16 21:19:56.000000 fedfind-5.2.0/src/fedfind.egg-info/dependency_links.txt
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)       45 2024-05-16 21:19:56.000000 fedfind-5.2.0/src/fedfind.egg-info/entry_points.txt
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)       68 2024-05-16 21:19:56.000000 fedfind-5.2.0/src/fedfind.egg-info/requires.txt
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)        8 2024-05-16 21:19:56.000000 fedfind-5.2.0/src/fedfind.egg-info/top_level.txt
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-05-16 21:19:56.830216 fedfind-5.2.0/tests/
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     7601 2024-05-15 18:18:27.000000 fedfind-5.2.0/tests/conftest.py
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-05-16 21:19:56.832216 fedfind-5.2.0/tests/data/
+-rw-r--r--   0 adamw     (1000) adamw     (1000)  1035277 2024-04-23 21:30:59.000000 fedfind-5.2.0/tests/data/allstable.json
+-rw-r--r--   0 adamw     (1000) adamw     (1000)   293981 2024-04-23 22:34:02.000000 fedfind-5.2.0/tests/data/compose-urls-20240423.json
+-rwxr-xr-x   0 adamw     (1000) adamw     (1000)     1437 2023-10-19 16:24:10.000000 fedfind-5.2.0/tests/data/fedfindloc.py
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-05-16 21:19:56.828216 fedfind-5.2.0/tests/data/http/
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-05-16 21:19:56.828216 fedfind-5.2.0/tests/data/http/pub/
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-05-16 21:19:56.832216 fedfind-5.2.0/tests/data/http/pub/alt/
+-rw-r--r--   0 adamw     (1000) adamw     (1000)   215056 2024-05-16 21:15:20.000000 fedfind-5.2.0/tests/data/http/pub/alt/imagelist-alt
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-05-16 21:19:56.832216 fedfind-5.2.0/tests/data/http/pub/archive/
+-rw-r--r--   0 adamw     (1000) adamw     (1000)   146475 2024-05-16 21:15:21.000000 fedfind-5.2.0/tests/data/http/pub/archive/imagelist-archive
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-05-16 21:19:56.832216 fedfind-5.2.0/tests/data/http/pub/fedora/
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    33469 2024-05-16 21:15:20.000000 fedfind-5.2.0/tests/data/http/pub/fedora/imagelist-fedora
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)    38788 2019-06-18 21:22:51.000000 fedfind-5.2.0/tests/data/pdc-compimages-Fedora-24-20160614.0.json
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)    43446 2019-06-18 21:22:51.000000 fedfind-5.2.0/tests/data/pdc-compimages-Fedora-25-20161115.0.json
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)    73734 2019-06-18 21:22:51.000000 fedfind-5.2.0/tests/data/pdc-compimages-Fedora-26-20170705.0.json
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)    70323 2019-06-18 21:22:51.000000 fedfind-5.2.0/tests/data/pdc-compimages-Fedora-27-20171105.0.json
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    81069 2023-10-19 16:24:10.000000 fedfind-5.2.0/tests/data/pdc-compimages-Fedora-28-20180425.0.json
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    59560 2023-10-19 16:24:10.000000 fedfind-5.2.0/tests/data/pdc-compimages-Fedora-29-20181024.1.json
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    61551 2023-10-19 16:24:10.000000 fedfind-5.2.0/tests/data/pdc-compimages-Fedora-30-20190425.0.json
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    57550 2023-10-19 16:24:10.000000 fedfind-5.2.0/tests/data/pdc-compimages-Fedora-31-20191023.0.json
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    59948 2023-10-19 16:24:10.000000 fedfind-5.2.0/tests/data/pdc-compimages-Fedora-32-20200422.0.json
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    65722 2023-10-19 16:24:10.000000 fedfind-5.2.0/tests/data/pdc-compimages-Fedora-33-20201019.0.json
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    63265 2023-10-19 16:24:10.000000 fedfind-5.2.0/tests/data/pdc-compimages-Fedora-34-20210423.0.json
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    66775 2023-10-19 16:24:10.000000 fedfind-5.2.0/tests/data/pdc-compimages-Fedora-35-20211026.0.json
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    65980 2023-10-19 16:24:10.000000 fedfind-5.2.0/tests/data/pdc-compimages-Fedora-36-20220504.1.json
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    27726 2023-10-19 16:24:10.000000 fedfind-5.2.0/tests/data/pdc-compimages-Fedora-37-20221105.0.json
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    29444 2023-10-19 16:24:10.000000 fedfind-5.2.0/tests/data/pdc-compimages-Fedora-38-20230413.1.json
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    64647 2024-04-23 22:28:11.000000 fedfind-5.2.0/tests/data/pdc-compimages-Fedora-39-20231031.1.json
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    70999 2024-04-23 22:26:25.000000 fedfind-5.2.0/tests/data/pdc-compimages-Fedora-40-20240414.0.json
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    29635 2023-10-19 16:24:10.000000 fedfind-5.2.0/tests/test_helpers.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    56539 2024-05-16 21:14:46.000000 fedfind-5.2.0/tests/test_release.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)       58 2023-10-19 16:24:10.000000 fedfind-5.2.0/tests.requires
+-rw-r--r--   0 adamw     (1000) adamw     (1000)      549 2023-10-19 16:24:10.000000 fedfind-5.2.0/tox.ini
+-rw-r--r--   0 adamw     (1000) adamw     (1000)       39 2023-10-19 16:24:10.000000 fedfind-5.2.0/tox.requires
```

### Comparing `fedfind-5.1.4/CHANGELOG.md` & `fedfind-5.2.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,23 @@
 ## Changelog
 
+### 5.2.0 - 2024-05-16
+
+*   [fedfind-5.2.0.tar.gz](https://files.pythonhosted.org/packages/source/f/fedfind/fedfind-5.2.0.tar.gz)
+
+1.  **NEW**: add `relnum` property to `Release` instances, representing the release number
+2.  **NEW**: add `eol` property to `Release` instances, indicating EOL date
+3.  **NEW**: re-introduce ``Updates`` and ``UpdatesTesting`` classes and support
+
+The updates and updates-testing composes have images again now, so we need to bring back support
+for them. The eol property is useful for fedora-cloud-image-uploader, so it seems reasonable to
+implement it here rather than making that project do the work. relnum is similarly useful there
+but also in various other places, it gives you a guaranteed integer which will be the "most
+correct-ish" one for Rawhide and ELN - the number of the next release that will branch.
+
 ### 5.1.4 - 2024-04-29
 
 *   [fedfind-5.1.4.tar.gz](https://files.pythonhosted.org/packages/source/f/fedfind/fedfind-5.1.4.tar.gz)
 
 1.  Handle a few new subvariants
 2.  Update test data etc. for Fedora 40 release
```

### Comparing `fedfind-5.1.4/COPYING` & `fedfind-5.2.0/COPYING`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.4/PKG-INFO` & `fedfind-5.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedfind
-Version: 5.1.4
+Version: 5.2.0
 Summary: Fedora Finder finds Fedora - images, more to come?
 Home-page: https://pagure.io/fedora-qa/fedfind
 Author: Adam Williamson
 Author-email: awilliam@redhat.com
 License: GPLv3+
 Keywords: fedora release image media iso
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fedfind-5.1.4/README.md` & `fedfind-5.2.0/README.md`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.4/gen-allstable` & `fedfind-5.2.0/gen-allstable`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.4/release.sh` & `fedfind-5.2.0/release.sh`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.4/setup.py` & `fedfind-5.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         LONGDESC = f.read()
 except TypeError:
     with open(path.join(HERE, 'README.md')) as f:
         LONGDESC = f.read()
 
 setup(
     name="fedfind",
-    version="5.1.4",
+    version="5.2.0",
     entry_points={'console_scripts': ['fedfind = fedfind.cli:main'],},
     author="Adam Williamson",
     author_email="awilliam@redhat.com",
     description="Fedora Finder finds Fedora - images, more to come?",
     license="GPLv3+",
     keywords="fedora release image media iso",
     url="https://pagure.io/fedora-qa/fedfind",
```

### Comparing `fedfind-5.1.4/src/fedfind/__init__.py` & `fedfind-5.2.0/src/fedfind/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,10 +18,10 @@
 """Library and CLI tool for locating and getting information about
 Fedora composes.
 """
 
 from __future__ import unicode_literals
 from __future__ import print_function
 
-__version__ = "5.1.4"
+__version__ = "5.2.0"
 
 # vim: set textwidth=100 ts=8 et sw=4:
```

### Comparing `fedfind-5.1.4/src/fedfind/cli.py` & `fedfind-5.2.0/src/fedfind/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,14 +191,16 @@
             "Final",
             "RC",
             "Cloud",
             "Branched",
             "Rawhide",
             "Production",
             "Respin",
+            "Updates",
+            "Updates-testing",
         ],
     )
     parser_images.add_argument(
         "-c",
         "--compose",
         "--date",
         help="A compose or date to search, e.g. 1 or 20160314. You "
```

### Comparing `fedfind-5.1.4/src/fedfind/const.py` & `fedfind-5.2.0/src/fedfind/const.py`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.4/src/fedfind/exceptions.py` & `fedfind-5.2.0/src/fedfind/exceptions.py`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.4/src/fedfind/helpers.py` & `fedfind-5.2.0/src/fedfind/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,20 +212,20 @@
         gotjson = download_json("https://fedorapeople.org/groups/qa/metadata/release.json")
         RELEASES = [int(time.time()), gotjson]
 
     # only return the actual data, not the timestamp...
     return RELEASES[1]
 
 
-def get_current_release(branched=False):
-    """Find out what the 'current' Fedora release is, according to
-    the Bodhi 'releases' API. If 'branched' is truth-y, will return
-    the Branched release number if there is one.
+def get_current_release(branched=False, dist="fedora"):
+    """Find out what the 'current' Fedora or EL release is. If
+    'branched' is truth-y, will return the Branched release number if
+    there is one.
     """
-    releases = _get_releases()["fedora"]
+    releases = _get_releases()[dist]
     # find current releases
     rels = list(releases["stable"])
     if branched:
         rels.extend(releases["branched"])
     return max(rels)
```

### Comparing `fedfind-5.1.4/src/fedfind/release.py` & `fedfind-5.2.0/src/fedfind/release.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         ciddic["date"],
         ciddic["compose_type"],
         ciddic["respin"],
     )
     release = release.capitalize()
 
     if ciddic["version_type"] in ("updates", "updates-testing"):
-        if dist != "FedoraRespin":
+        if dist not in ("FedoraRespin", "Fedora"):
             raise fedfind.exceptions.UnsupportedComposeError(
                 "get_release(): fedfind does not support composes "
                 "like {} as they contain no images".format(cid)
             )
 
     # Reject EPEL composes, we do not handle these
     if "-epel-" in dist.lower():
@@ -124,14 +124,20 @@
     if typ == "nightly":
         if release == "Rawhide":
             milestone = ""
         else:
             milestone = "Branched"
         return (dist, release, milestone, date, int(respin))
     elif typ == "production":
+        if ciddic["version_type"] == "updates":
+            # 'updates' compose
+            return (dist, release, "Updates", date, int(respin))
+        elif ciddic["version_type"] == "updates-testing":
+            # 'updates-testing' compose
+            return (dist, release, "Updates-testing", date, int(respin))
         # date 19700101 indicates a fedfind fake CID, most likely
         # for a stable release, so just return the release number
         # so we get a stable release class
         if date == "19700101":
             return (dist, release, "", "", 0)
         return (dist, release, "Production", date, int(respin))
     else:
@@ -174,14 +180,16 @@
     snaps = (
         "rawhide",
         "branched",
         "Fedora-Cloud",
         "Fedora-Container",
         "Fedora-IoT",
         "production",
+        "updates",
+        "updates-testing",
     )
     # we also don't want to guess for FedoraRespin even if release
     # and milestone are not set
     if compose or dist.lower() == "fedorarespin":
         return compose
     if (not release and not milestone) or _val_in_str(snaps, (dist, release, milestone)):
         logger.debug("Guessing date")
@@ -211,14 +219,16 @@
             err = "Release {} must be a number, ELN, or Rawhide!".format(str(release))
             raise ValueError("get_release(): {}".format(err))
 
     # If we were specifically asked for a valid milestone, return
     # appropriate release.
     if milestone.lower() in ("branched", "production"):
         return fedfind.helpers.get_current_release() + 1
+    elif milestone.lower() in ("updates", "updates-testing"):
+        return fedfind.helpers.get_current_release()
     elif dist.lower() in (
         "fedora-cloud",
         "fedora-container",
         "fedora-iot",
     ):
         # Note: these are often composed for both
         # current and prev, but we gotta guess something...
@@ -294,27 +304,31 @@
     milestone. If respin is not specified, handles guessing that.
     """
     if milestone.lower() == "production":
         if respin is None:
             raise ValueError("Cannot guess respin for a production candidate compose!")
         return Production(release, date, respin)
 
-    # The only other milestone that's "valid" is Branched
-    if milestone and milestone.lower() != "branched":
+    # The only expected valid milestones
+    if milestone and milestone.lower() not in ("branched", "updates", "updates-testing"):
         logger.warning("Invalid milestone %s for nightly! Ignoring.", milestone)
 
+    # map of milestones to classes
+    updatesmap = {"updates": Updates, "updates-testing": UpdatesTesting}
     # map of dist strings to classes
     nightlymap = {
         "fedora-cloud": CloudNightly,
         "fedora-container": ContainerNightly,
         "fedora-iot": IoTNightly,
     }
-    # if the dist isn't any of the recognized ones, we'll just go with
-    # Branched
-    klass = nightlymap.get(dist.lower(), BranchedNightly)
+    klass = updatesmap.get(milestone.lower())
+    if not klass:
+        # if the dist isn't any of the recognized ones, we'll just go
+        # with Branched
+        klass = nightlymap.get(dist.lower(), BranchedNightly)
     if respin is None:
         partrel = partial(klass, release=release, compose=date)
         return _guess_nightly_respin(partrel)
     return klass(release=release, compose=date, respin=respin)
 
 
 def _legacy_milestones(dist, milestone):
@@ -487,22 +501,22 @@
     ensure compatibility with wikitcms, where Rawhide compose events
     are versioned as e.g. 23 Rawhide 20150304. Wikitcms similarly
     tries to handle fedfind release values (by guessing a release
     number for a version like Rawhide '' 20150304 0), so usually,
     fedfind and wikitcms versions are transparently interchangeable.
 
     For nightlies, pass compose as 'YYYYMMDD'. You'll wind up with
-    either a Rawhide, Branched, Cloud, Container or IoT nightly,
-    depending on dist, release and milestone. If you set "Fedora"
-    dist and a valid release number and leave milestone unset,
-    you'll get BranchedNightly. You can never get anything else by
-    nightly detection, you must specify it via dist, milestone, cid
-    or url. If you set a valid release number and a valid nightly
-    milestone or dist, you'll get what you asked for. For any other
-    case you'll wind up with RawhideNightly.
+    either a Rawhide, Branched, Cloud, Container, IoT, Updates or
+    Updates-testing nightly, depending on dist, release and milestone.
+    If you set "Fedora" dist and a valid release number and leave
+    milestone unset, you'll get BranchedNightly. You can never get
+    anything else by nightly detection, you must specify it via dist,
+    milestone, cid or url. If you set a valid release number and a
+    valid nightly milestone or dist, you'll get what you asked for.
+    For any other case you'll wind up with RawhideNightly.
 
     At present the interesting values for dist are 'Fedora' (the
     default), 'Fedora-Cloud', 'Fedora-Container' and 'Fedora-IoT'.
     Fedora' is the default and will give you 'mainstream' composes.
     The other dists give you the Container and IoT nightly composes
     respectively.
 
@@ -777,49 +791,49 @@
         Fedora key deliverables for the future.
         """
         imgs = list()
         intels = (arch.name for arch in fedfind.const.ARCHES if arch.group == "intel")
         # i386 stopped being primary in f26, fedfind doesn't currently
         # handle secondary arches (and we stopped building ix86 images
         # entirely after F30)
-        if self._relnum > 25:
+        if self._fake_relnum > 25:
             intels = (intel for intel in intels if intel != "i386")
         for arch in intels:
-            if self._relnum > 20:
+            if self._fake_relnum > 20:
                 imgs.append(("kde", "live", arch))
                 imgs.append(("workstation", "live", arch))
                 imgs.append(("server", "boot", arch))
                 imgs.append(("server", "dvd", arch))
                 # per dgilmore, we stopped doing 32-bit Cloud with F24
-                if arch == "x86_64" or self._relnum < 24:
+                if arch == "x86_64" or self._fake_relnum < 24:
                     imgs.append(("cloud_base", "raw-xz", arch))
                     imgs.append(("cloud_base", "qcow2", arch))
-            elif self._relnum > 1:
+            elif self._fake_relnum > 1:
                 imgs.append(("everything", "boot", arch))
-                if self._relnum > 2:
+                if self._fake_relnum > 2:
                     imgs.append(("everything", "dvd", arch))
-                if self._relnum > 6:
+                if self._fake_relnum > 6:
                     imgs.append(("kde", "live", arch))
                     imgs.append(("desktop", "live", arch))
                 # 7 and 8 had no installer CDs, for...some reason?
-                if self._relnum < 15 and self._relnum not in (7, 8):
+                if self._fake_relnum < 15 and self._fake_relnum not in (7, 8):
                     imgs.append(("everything", "cd", arch))
 
         # 32-bit arm images became primary in f20, were removed in f37
-        if self._relnum > 19 and self._relnum < 37:
+        if self._fake_relnum > 19 and self._fake_relnum < 37:
             imgs.append(("minimal", "raw-xz", "armhfp"))
-            if self._relnum > 31:
+            if self._fake_relnum > 31:
                 # we don't block on 32-bit ARM desktop after 31
                 pass
-            elif self._relnum > 22:
+            elif self._fake_relnum > 22:
                 imgs.append(("xfce", "raw-xz", "armhfp"))
             else:
                 imgs.append(("kde", "raw-xz", "armhfp"))
 
-        if self._relnum > 31:
+        if self._fake_relnum > 31:
             imgs.append(("cloud_base", "raw-xz", "aarch64"))
             imgs.append(("server", "dvd", "aarch64"))
             imgs.append(("server", "boot", "aarch64"))
             imgs.append(("workstation", "raw-xz", "aarch64"))
 
         return imgs
 
@@ -854,30 +868,54 @@
                         )
                     else:
                         imgdict["direct_url"] = imgdict["url"]
                     images.append(imgdict)
         return images
 
     @cached_property
-    def _relnum(self):
+    def _fake_relnum(self):
         """Having to deal with 'rawhide' when checking self.release is
         really annoying; this is a silly hack to help with that. It's
-        a property because self.release can actually involve a round
+        appropriate for cases where you just need an int, and for the
+        number for Rawhide to be higher than anything else. It's a
+        property because self.release can actually involve a network
         trip, for bare Pungi4Release instances, so we don't want to
         set it up in __init__.
         """
         try:
             if self.release.lower() == "rawhide":
                 return 999
             else:
                 return int(self.release)
         except AttributeError:
             # this happens in an odd path used in RespinRelease init
             return 999
 
+    @cached_property
+    def relnum(self):
+        """For non-Rawhide releases, this is just the release number
+        as an integer. For Rawhide, it is the number of the next
+        release that will branch. This is useful for doing comparisons
+        and for various cases where we do associate this number with
+        Rawhide, e.g. in Bodhi. This involves a network trip to get
+        the release metadata.
+        """
+        if self.release.lower() == "rawhide":
+            return fedfind.helpers.get_current_release(branched=True) + 1
+        else:
+            return int(self.release)
+
+    @cached_property
+    def eol(self):
+        """The EOL date for the release (from Bodhi data)."""
+        # this assumes we're a Fedora release, which is safe enough
+        # for now. Rawhide and ELN override this
+        url = "https://bodhi.fedoraproject.org/releases/F{}".format(self.relnum)
+        return fedfind.helpers.download_json(url).get("eol")
+
     def check_expected(self):
         """This checks whether all expected images are included in the
         release. If the release doesn't exist, it will raise an
         exception. If any expected images are missing, it will return
         a set of (subvariant, imagetype, arch) tuples identifying the
         missing images. If nothing is missing, it will return an empty
         set.
@@ -916,21 +954,21 @@
         # Grab the directory indexes we need. This is a bit different
         # for older releases; it's awkward to express this via the
         # classes so just conditionalize it here. Before F17, package
         # directories like this one are not split into subdirectories
         # by first character. Before F7, there was no /Everything.
         # Before F5, there was no /source.
         split = True
-        if self._relnum < 17:
+        if self._fake_relnum < 17:
             split = False
-        if self._relnum > 23:
+        if self._fake_relnum > 23:
             url = "{}/source/tree/Packages/".format(self.https_url_generic)
-        elif self._relnum > 6:
+        elif self._fake_relnum > 6:
             url = "{}/Everything/source/SRPMS/".format(self.location)
-        elif self._relnum > 4:
+        elif self._fake_relnum > 4:
             url = "{}/source/SRPMS/".format(self.location)
         else:
             url = "{}/SRPMS/".format(self.location)
         if split:
             for i in initials:
                 suburl = "{}{}/".format(url, i)
                 index = fedfind.helpers.urlopen_retries(suburl)
@@ -1466,14 +1504,19 @@
             milestone="",
             compose=compose,
             respin=respin,
             typ="nightly",
             cid=cid,
         )
 
+    @cached_property
+    def eol(self):
+        """Rawhide never has an EOL."""
+        return None
+
 
 class BranchedNightly(OldPreviousReleaseMixin, Pungi4ReleaseFull):
     """Branched "nightly" (bit of a misnomer, now) composes."""
 
     def __init__(self, release, compose, respin=0, cid=None):
         release = str(release)
         compose = str(compose)
@@ -1600,14 +1643,82 @@
             ("iot", "raw-xz", "x86_64"),
             ("iot", "dvd", "aarch64"),
             ("iot", "dvd-ostree", "aarch64"),
             ("iot", "raw-xz", "aarch64"),
         )
 
 
+class Updates(Pungi4Release):
+    """'updates' compose. These are mainly intended to produce the
+    'updates' repository for a release, but they also produce Atomic
+    Desktop container images, and may be extended to replace the
+    separate Cloud and Container nightly composes. Like other
+    post-release nightlies, these are of type 'production'.
+    """
+
+    def __init__(self, release, compose, respin=0, cid=None):
+        release = str(release)
+        compose = str(compose)
+        respin = str(respin)
+        path = "updates/Fedora-{}-updates-{}.{}/compose".format(release, compose, respin)
+        url = "/".join((fedfind.const.NIGHTLY_BASE, path))
+        super(Updates, self).__init__(
+            url,
+            release=release,
+            milestone="Updates",
+            compose=compose,
+            respin=respin,
+            typ="production",
+            cid=cid,
+        )
+        self._release = release
+
+    @property
+    def expected_images(self):
+        """See abstract class docstring for information on what this
+        is. I hate this interface and want to get rid of it, so I'm
+        not bothering to implement it properly here.
+        """
+        return tuple()
+
+
+class UpdatesTesting(Pungi4Release):
+    """'updates-testing' compose. These are mainly intended to produce
+    the 'updates-testing' repository for a release, but they also
+    produce Atomic Desktop container images, and may be extended to
+    replace the separate Cloud and Container nightly composes. Like
+    other post-release nightlies, these are of type 'production'.
+    """
+
+    def __init__(self, release, compose, respin=0, cid=None):
+        release = str(release)
+        compose = str(compose)
+        respin = str(respin)
+        path = "updates/Fedora-{}-updates-testing-{}.{}/compose".format(release, compose, respin)
+        url = "/".join((fedfind.const.NIGHTLY_BASE, path))
+        super(UpdatesTesting, self).__init__(
+            url,
+            release=release,
+            milestone="Updates-testing",
+            compose=compose,
+            respin=respin,
+            typ="production",
+            cid=cid,
+        )
+        self._release = release
+
+    @property
+    def expected_images(self):
+        """See abstract class docstring for information on what this
+        is. I hate this interface and want to get rid of it, so I'm
+        not bothering to implement it properly here.
+        """
+        return tuple()
+
+
 ## PUNGI 4 CANDIDATE COMPOSES ##
 
 
 class Production(Pungi4ReleaseFull):
     """A Pungi 4 'production' compose, on kojipkgs, identified by date
     and respin (not label). 'compose' is the date. e.g. 24, 20160314,
     1 for
@@ -1803,15 +1914,15 @@
                         size = int(size)
                     # in the file list, paths start with './'. But our
                     # base paths start with the folder name. So sub
                     # ./ with the folder name for comparison
                     path = path.split("/")
                     # along the way, let's check for boot.iso and
                     # throw it out if we're > 8
-                    if self._relnum > 8:
+                    if self._fake_relnum > 8:
                         fname = path[-1].strip()
                         if fname == "boot.iso":
                             continue
                     path[0] = flist
                     path = "/".join(path)
 
                     # Next three lines check if path starts with
@@ -1896,19 +2007,19 @@
     @property
     def https_url_generic(self):
         """HTTPS URL for the 'generic' tree for this release (whose
         subdirectories are named for primary arches and contain
         .treeinfo files, and where the 'generic' network install
         image for the release was built from).
         """
-        if self._relnum < 7:
+        if self._fake_relnum < 7:
             return self.location
-        elif self._relnum < 21:
+        elif self._fake_relnum < 21:
             return "{}/Fedora".format(self.location)
-        elif self._relnum <= 23:
+        elif self._fake_relnum <= 23:
             return "{}/Server".format(self.location)
         else:
             return "{}/Everything".format(self.location)
 
     @property
     def metadata(self):
         """Pungi 4 / productmd-style metadata for the compose. If we
@@ -2091,15 +2202,15 @@
     @cached_property
     def label(self):
         """Try to figure out the compose label, if we can (i.e. if the
         compose was done with Pungi 4 but had its metadata stripped).
         We do this by parsing the image file names, looking for an
         expected pattern.
         """
-        if self._relnum < 24:
+        if self._fake_relnum < 24:
             # These composes cannot be said to have a label.
             return ""
 
         if self.milestone:
             relname = "_".join((self.release, self.milestone))
         else:
             relname = self.release
@@ -2121,15 +2232,15 @@
 
     @cached_property
     def cid(self):
         """If we can, try to figure out the true compose ID by first
         getting the label (see above) and then getting the CID from
         it. If we can't, just return something fake.
         """
-        if self._relnum < 24:
+        if self._fake_relnum < 24:
             # No chance.
             return self._fakecid
 
         if self.label:
             cid = fedfind.helpers.cid_from_label(self.release, self.label)
             if cid:
                 return cid
@@ -2221,15 +2332,15 @@
 
     @property
     def _basepath(self):
         return "archive/fedora/linux/releases/{}".format(self.release)
 
     @property
     def _altbasepath(self):
-        if self._relnum > 14:
+        if self._fake_relnum > 14:
             return "alt/releases/{}".format(self.release)
         else:
             # there were no 'alt' bits prior to F15
             return None
 
 
 class CoreRelease(MirrorRelease):
@@ -2393,13 +2504,25 @@
         raise NotImplementedError
 
     def get_package_nevras_pdc(self, packages):
         """These aren't in PDC."""
         raise NotImplementedError
 
     @cached_property
-    def _relnum(self):
+    def _fake_relnum(self):
         """Let's treat ELN like Rawhide here."""
         return 999
 
+    @cached_property
+    def relnum(self):
+        """ELN's associated release number should always be the next
+        EL release to branch.
+        """
+        return fedfind.helpers.get_current_release(branched=True, dist="el") + 1
+
+    @cached_property
+    def eol(self):
+        """ELN never has an EOL."""
+        return None
+
 
 # vim: set textwidth=100 ts=8 et sw=4:
```

### Comparing `fedfind-5.1.4/src/fedfind.egg-info/PKG-INFO` & `fedfind-5.2.0/src/fedfind.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedfind
-Version: 5.1.4
+Version: 5.2.0
 Summary: Fedora Finder finds Fedora - images, more to come?
 Home-page: https://pagure.io/fedora-qa/fedfind
 Author: Adam Williamson
 Author-email: awilliam@redhat.com
 License: GPLv3+
 Keywords: fedora release image media iso
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fedfind-5.1.4/src/fedfind.egg-info/SOURCES.txt` & `fedfind-5.2.0/src/fedfind.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.4/tests/conftest.py` & `fedfind-5.2.0/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,18 +46,24 @@
 from six.moves.urllib.request import urlopen
 
 import fedfind.const
 import fedfind.helpers
 
 # Fake data for the releases fixtures. This is what real data would
 # have looked like as of 2020-02-21.
-RELEASES_BRANCHED_JSON = {"fedora": {"stable": [30, 31], "branched": [32]}}
+RELEASES_BRANCHED_JSON = {
+    "fedora": {"stable": [30, 31], "branched": [32]},
+    "el": {"stable": [6, 7, 8], "branched": [9]},
+}
 
 # This removes Branched, to check behaviour when there isn't one.
-RELEASES_NOBRANCHED_JSON = {"fedora": {"stable": [30, 31], "branched": []}}
+RELEASES_NOBRANCHED_JSON = {
+    "fedora": {"stable": [30, 31], "branched": []},
+    "el": {"stable": [6, 7, 8], "branched": []},
+}
 
 
 @pytest.yield_fixture(scope="session")
 def http(request):
     """Run a SimpleHTTPServer that we can use as a fake dl.fp.o. Serve
     the contents of tests/data/http, for the entire test session. We
     just do this with subprocess as we need it to run parallel to the
```

### Comparing `fedfind-5.1.4/tests/data/allstable.json` & `fedfind-5.2.0/tests/data/allstable.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.4/tests/data/compose-urls-20240423.json` & `fedfind-5.2.0/tests/data/compose-urls-20240423.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.4/tests/data/fedfindloc.py` & `fedfind-5.2.0/tests/data/fedfindloc.py`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.4/tests/data/http/pub/alt/imagelist-alt` & `fedfind-5.2.0/tests/data/http/pub/alt/imagelist-alt`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.4/tests/data/http/pub/archive/imagelist-archive` & `fedfind-5.2.0/tests/data/http/pub/archive/imagelist-archive`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.4/tests/data/http/pub/fedora/imagelist-fedora` & `fedfind-5.2.0/tests/data/http/pub/fedora/imagelist-fedora`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.4/tests/data/pdc-compimages-Fedora-24-20160614.0.json` & `fedfind-5.2.0/tests/data/pdc-compimages-Fedora-24-20160614.0.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.4/tests/data/pdc-compimages-Fedora-25-20161115.0.json` & `fedfind-5.2.0/tests/data/pdc-compimages-Fedora-25-20161115.0.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.4/tests/data/pdc-compimages-Fedora-26-20170705.0.json` & `fedfind-5.2.0/tests/data/pdc-compimages-Fedora-26-20170705.0.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.4/tests/data/pdc-compimages-Fedora-27-20171105.0.json` & `fedfind-5.2.0/tests/data/pdc-compimages-Fedora-27-20171105.0.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.4/tests/data/pdc-compimages-Fedora-28-20180425.0.json` & `fedfind-5.2.0/tests/data/pdc-compimages-Fedora-28-20180425.0.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.4/tests/data/pdc-compimages-Fedora-29-20181024.1.json` & `fedfind-5.2.0/tests/data/pdc-compimages-Fedora-29-20181024.1.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.4/tests/data/pdc-compimages-Fedora-30-20190425.0.json` & `fedfind-5.2.0/tests/data/pdc-compimages-Fedora-30-20190425.0.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.4/tests/data/pdc-compimages-Fedora-31-20191023.0.json` & `fedfind-5.2.0/tests/data/pdc-compimages-Fedora-31-20191023.0.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.4/tests/data/pdc-compimages-Fedora-32-20200422.0.json` & `fedfind-5.2.0/tests/data/pdc-compimages-Fedora-32-20200422.0.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.4/tests/data/pdc-compimages-Fedora-33-20201019.0.json` & `fedfind-5.2.0/tests/data/pdc-compimages-Fedora-33-20201019.0.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.4/tests/data/pdc-compimages-Fedora-34-20210423.0.json` & `fedfind-5.2.0/tests/data/pdc-compimages-Fedora-34-20210423.0.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.4/tests/data/pdc-compimages-Fedora-35-20211026.0.json` & `fedfind-5.2.0/tests/data/pdc-compimages-Fedora-35-20211026.0.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.4/tests/data/pdc-compimages-Fedora-36-20220504.1.json` & `fedfind-5.2.0/tests/data/pdc-compimages-Fedora-36-20220504.1.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.4/tests/data/pdc-compimages-Fedora-37-20221105.0.json` & `fedfind-5.2.0/tests/data/pdc-compimages-Fedora-37-20221105.0.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.4/tests/data/pdc-compimages-Fedora-38-20230413.1.json` & `fedfind-5.2.0/tests/data/pdc-compimages-Fedora-38-20230413.1.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.4/tests/data/pdc-compimages-Fedora-39-20231031.1.json` & `fedfind-5.2.0/tests/data/pdc-compimages-Fedora-39-20231031.1.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.4/tests/data/pdc-compimages-Fedora-40-20240414.0.json` & `fedfind-5.2.0/tests/data/pdc-compimages-Fedora-40-20240414.0.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.4/tests/test_helpers.py` & `fedfind-5.2.0/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.4/tests/test_release.py` & `fedfind-5.2.0/tests/test_release.py`

 * *Files 5% similar despite different names*

```diff
@@ -353,14 +353,40 @@
                 "Fedora-IoT",
                 fedfind.release.IoTNightly,
                 "28",
                 "Nightly",
                 "datestr",
                 "0",
             ),
+            # Updates nightly.
+            (
+                28,
+                "Updates",
+                "datestr",
+                0,
+                "Fedora",
+                fedfind.release.Updates,
+                "28",
+                "Updates",
+                "datestr",
+                "0",
+            ),
+            # Updates-testing nightly.
+            (
+                28,
+                "Updates-testing",
+                "datestr",
+                0,
+                "Fedora",
+                fedfind.release.UpdatesTesting,
+                "28",
+                "Updates-testing",
+                "datestr",
+                "0",
+            ),
             # Wikitcms format Rawhide.
             (
                 "24",
                 "Rawhide",
                 "datestr.n.0",
                 None,
                 "Fedora",
@@ -590,14 +616,42 @@
         )
         ret = fedfind.release.get_release(url=url)
         assert isinstance(ret, fedfind.release.BranchedNightly)
         assert ret.release == "27"
         assert ret.compose == "20170816"
         assert ret.respin == "0"
 
+    def test_get_release_url_cid_updates(self):
+        """Getting a release based on a correct updates compose
+        URL should work.
+        """
+        url = (
+            "https://kojipkgs.fedoraproject.org/"
+            "compose/updates/Fedora-28-updates-20180605.0/compose/"
+        )
+        ret = fedfind.release.get_release(url=url)
+        assert isinstance(ret, fedfind.release.Updates)
+        assert ret.release == "28"
+        assert ret.compose == "20180605"
+        assert ret.respin == "0"
+
+    def test_get_release_url_cid_updates_testing(self):
+        """Getting a release based on a correct updates-testing
+        compose URL should work.
+        """
+        url = (
+            "https://kojipkgs.fedoraproject.org/"
+            "compose/updates/Fedora-28-updates-testing-20180605.0/compose/"
+        )
+        ret = fedfind.release.get_release(url=url)
+        assert isinstance(ret, fedfind.release.UpdatesTesting)
+        assert ret.release == "28"
+        assert ret.compose == "20180605"
+        assert ret.respin == "0"
+
     def test_get_release_url_cid_unknown(self):
         """Getting a release based on an unknown URL should return
         a generic Pungi4Release instance, so long as the URL starts
         with an acceptable string (to avoid puiterwijk's 'evil URL
         input' scenario).
         """
         ret = fedfind.release.get_release(
@@ -751,19 +805,33 @@
         assert got.release == "23"
 
         got = fedfind.release.get_release("", "", "", 0, dist="Fedora-IoT")
         assert isinstance(got, fedfind.release.IoTNightly)
         assert got.compose == datestr
         assert got.release == "23"
 
+        # updates
+        got = fedfind.release.get_release("", "Updates", "", 0)
+        assert isinstance(got, fedfind.release.Updates)
+        assert got.compose == datestr
+        assert got.release == "23"
+
+        # updates-testing
+        got = fedfind.release.get_release("", "Updates-testing", "", 0)
+        assert isinstance(got, fedfind.release.UpdatesTesting)
+        assert got.compose == datestr
+        assert got.release == "23"
+
     @mock.patch("fedfind.release.RawhideNightly", FakeRelease)
     @mock.patch("fedfind.release.BranchedNightly", FakeRelease)
     @mock.patch("fedfind.release.CloudNightly", FakeRelease)
     @mock.patch("fedfind.release.ContainerNightly", FakeRelease)
     @mock.patch("fedfind.release.IoTNightly", FakeRelease)
+    @mock.patch("fedfind.release.Updates", FakeRelease)
+    @mock.patch("fedfind.release.UpdatesTesting", FakeRelease)
     def test_get_release_guess_respin(self):
         """Test the 'respin guessing' code works (when you request a
         nightly but don't provide a respin number). Uses the fake
         release class's feature of 'existing' when the respin is 3.
         """
         got = fedfind.release.get_release(24, "Branched", "20160314")
         assert isinstance(got, fedfind.release.BranchedNightly)
@@ -781,14 +849,22 @@
         assert got.respin == 3
         got = fedfind.release.get_release(24, "", "20160628", dist="Fedora-Container")
         assert isinstance(got, fedfind.release.ContainerNightly)
         assert got.respin == 3
         got = fedfind.release.get_release(24, "", "20160628", dist="Fedora-IoT")
         assert isinstance(got, fedfind.release.IoTNightly)
         assert got.respin == 3
+        # updates
+        got = fedfind.release.get_release(24, "Updates", "20160628")
+        assert isinstance(got, fedfind.release.Updates)
+        assert got.respin == 3
+        # updates-testing
+        got = fedfind.release.get_release(24, "UpdatesTesting", "20160628")
+        assert isinstance(got, fedfind.release.UpdatesTesting)
+        assert got.respin == 3
 
     @mock.patch.object(fedfind.release.BranchedNightly, "exists", True)
     @mock.patch.object(fedfind.release.BranchedNightly, "status", "FINISHED")
     def test_get_release_no_milestone_branched(self):
         """If we specify a date and a release number, but no milestone,
         fedfind should return BranchedNightly.
         """
@@ -840,15 +916,15 @@
         to bother mocking it here.
         """
         got = fedfind.release.get_release("ELN", "", "12345")
         assert isinstance(got, fedfind.release.ElnCompose)
         assert got.location == "https://odcs.fedoraproject.org/composes/odcs-12345/compose"
         expgen = "https://odcs.fedoraproject.org/composes/odcs-12345/compose/BaseOS"
         assert got.https_url_generic == expgen
-        assert got._relnum == 999
+        assert got._fake_relnum == 999
         with pytest.raises(NotImplementedError):
             _ = got.previous_release
         with pytest.raises(NotImplementedError):
             got.get_package_nevras_pdc(["somepackage"])
         got = fedfind.release.get_release(url="https://odcs.fedoraproject.org/composes/odcs-28282")
         assert isinstance(got, fedfind.release.ElnCompose)
         with pytest.raises(ValueError):
@@ -1101,9 +1177,42 @@
             assert fakeerror.call_count == 1 * multiplier
         if composeinfo and not images:
             # if composeinfo but no images, an info once per attempt
             assert fakeinfo.call_count == 1 * multiplier
         else:
             assert fakeinfo.call_count == 0
 
+    def test_relnum_branched(self, releases_branched):
+        """Check relnum property across Fedora and ELN (when branched
+        releases exist).
+        """
+        rawrel = fedfind.release.RawhideNightly("20230831", 0, "Fedora-Rawhide-20230831.n.0")
+        assert rawrel.relnum == 33
+        brel = fedfind.release.BranchedNightly("32", "20230831", 0, "Fedora-32-20230831.n.0")
+        assert brel.relnum == 32
+        elnrel = fedfind.release.ElnCompose("123")
+        assert elnrel.relnum == 10
+
+    def test_relnum_nobranched(self, releases_nobranched):
+        """Check relnum property across Fedora and ELN (when no
+        branched releases exist).
+        """
+        rawrel = fedfind.release.RawhideNightly("20230831", 0, "Fedora-Rawhide-20230831.n.0")
+        assert rawrel.relnum == 32
+        elnrel = fedfind.release.ElnCompose("123")
+        assert elnrel.relnum == 9
+
+    @mock.patch("fedfind.helpers.download_json", autospec=True, return_value={"eol": "2024-05-16"})
+    def test_eol(self, fakedljson):
+        """Test eol property works as expected."""
+        rawrel = fedfind.release.RawhideNightly("20230831", 0, "Fedora-Rawhide-20230831.n.0")
+        elnrel = fedfind.release.ElnCompose("123")
+        crel = fedfind.release.CurrentRelease("40")
+        assert rawrel.eol is None
+        assert elnrel.eol is None
+        assert fakedljson.call_count == 0
+        assert crel.eol == "2024-05-16"
+        assert fakedljson.call_count == 1
+        assert fakedljson.call_args == (("https://bodhi.fedoraproject.org/releases/F40",),)
+
 
 # vim: set textwidth=100 ts=8 et sw=4:
```

### Comparing `fedfind-5.1.4/tox.ini` & `fedfind-5.2.0/tox.ini`

 * *Files identical despite different names*

