# Comparing `tmp/testflows.github.hetzner.runners-1.7.240318.1205504.tar.gz` & `tmp/testflows.github.hetzner.runners-1.7.240319.1151947.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.hetzner.runners-1.7.240318.1205504.tar", last modified: Mon Mar 18 20:55:04 2024, max compression
+gzip compressed data, was "testflows.github.hetzner.runners-1.7.240319.1151947.tar", last modified: Tue Mar 19 15:19:47 2024, max compression
```

## Comparing `testflows.github.hetzner.runners-1.7.240318.1205504.tar` & `testflows.github.hetzner.runners-1.7.240319.1151947.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-18 20:55:04.524890 testflows.github.hetzner.runners-1.7.240318.1205504/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2024-03-14 16:48:24.000000 testflows.github.hetzner.runners-1.7.240318.1205504/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    19385 2024-03-18 20:55:04.524890 testflows.github.hetzner.runners-1.7.240318.1205504/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    18747 2024-03-18 11:17:58.000000 testflows.github.hetzner.runners-1.7.240318.1205504/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2024-03-18 20:55:04.524890 testflows.github.hetzner.runners-1.7.240318.1205504/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2317 2024-03-18 20:55:04.000000 testflows.github.hetzner.runners-1.7.240318.1205504/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-18 20:55:04.524890 testflows.github.hetzner.runners-1.7.240318.1205504/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-18 20:55:04.524890 testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-18 20:55:04.524890 testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-18 20:55:04.524890 testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2024-03-18 20:55:04.000000 testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2520 2024-03-14 16:48:24.000000 testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     1995 2024-03-14 16:48:24.000000 testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/api_watch.py
--rw-rw-r--   0 user      (1000) user      (1000)     4319 2024-03-14 16:48:24.000000 testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-18 20:55:04.524890 testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    33497 2024-03-16 23:20:07.000000 testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/bin/github-hetzner-runners
--rw-rw-r--   0 user      (1000) user      (1000)    15625 2024-03-14 16:48:24.000000 testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/cloud.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-18 20:55:04.524890 testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/config/
--rw-rw-r--   0 user      (1000) user      (1000)      993 2024-03-14 16:48:24.000000 testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/config/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    24278 2024-03-14 16:48:24.000000 testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/config/config.py
--rw-rw-r--   0 user      (1000) user      (1000)    13636 2024-03-14 16:48:24.000000 testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/config/schema.json
--rw-rw-r--   0 user      (1000) user      (1000)     2574 2024-03-14 16:48:24.000000 testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/delete.py
--rw-rw-r--   0 user      (1000) user      (1000)    12025 2024-03-18 20:51:22.000000 testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/estimate.py
--rw-rw-r--   0 user      (1000) user      (1000)     6743 2024-03-14 16:48:24.000000 testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/logger.py
--rw-rw-r--   0 user      (1000) user      (1000)     1926 2024-03-14 16:48:24.000000 testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)    26796 2024-03-16 19:51:24.000000 testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)    35850 2024-03-18 16:00:18.000000 testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-18 20:55:04.524890 testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2024-03-14 16:48:24.000000 testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-18 20:55:04.524890 testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2024-03-14 16:48:24.000000 testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      535 2024-03-14 16:48:24.000000 testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)        0 2024-03-14 16:48:24.000000 testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/scripts/none.sh
--rw-rw-r--   0 user      (1000) user      (1000)     1148 2024-03-14 16:48:24.000000 testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/scripts/setup-docker.sh
--rw-rw-r--   0 user      (1000) user      (1000)      260 2024-03-14 16:48:24.000000 testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      767 2024-03-17 13:54:38.000000 testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/scripts/startup-arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      759 2024-03-17 13:54:45.000000 testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/scripts/startup-x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     3206 2024-03-14 16:48:24.000000 testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     2722 2024-03-14 16:48:24.000000 testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/servers.py
--rw-rw-r--   0 user      (1000) user      (1000)     9056 2024-03-14 16:48:24.000000 testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1695 2024-03-14 16:48:24.000000 testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/shell.py
--rw-rw-r--   0 user      (1000) user      (1000)     2683 2024-03-16 20:04:55.000000 testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/streamingyaml.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-18 20:55:04.524890 testflows.github.hetzner.runners-1.7.240318.1205504/testflows.github.hetzner.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    19385 2024-03-18 20:55:04.000000 testflows.github.hetzner.runners-1.7.240318.1205504/testflows.github.hetzner.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1723 2024-03-18 20:55:04.000000 testflows.github.hetzner.runners-1.7.240318.1205504/testflows.github.hetzner.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-03-18 20:55:04.000000 testflows.github.hetzner.runners-1.7.240318.1205504/testflows.github.hetzner.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-03-15 23:34:11.000000 testflows.github.hetzner.runners-1.7.240318.1205504/testflows.github.hetzner.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       73 2024-03-18 20:55:04.000000 testflows.github.hetzner.runners-1.7.240318.1205504/testflows.github.hetzner.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2024-03-18 20:55:04.000000 testflows.github.hetzner.runners-1.7.240318.1205504/testflows.github.hetzner.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-19 15:19:47.324334 testflows.github.hetzner.runners-1.7.240319.1151947/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2024-03-14 16:48:24.000000 testflows.github.hetzner.runners-1.7.240319.1151947/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    19385 2024-03-19 15:19:47.324334 testflows.github.hetzner.runners-1.7.240319.1151947/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    18747 2024-03-18 11:17:58.000000 testflows.github.hetzner.runners-1.7.240319.1151947/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2024-03-19 15:19:47.324334 testflows.github.hetzner.runners-1.7.240319.1151947/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2317 2024-03-19 15:19:47.000000 testflows.github.hetzner.runners-1.7.240319.1151947/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-19 15:19:47.324334 testflows.github.hetzner.runners-1.7.240319.1151947/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-19 15:19:47.324334 testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-19 15:19:47.324334 testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-19 15:19:47.324334 testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2024-03-19 15:19:47.000000 testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2520 2024-03-14 16:48:24.000000 testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1995 2024-03-14 16:48:24.000000 testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/api_watch.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4319 2024-03-14 16:48:24.000000 testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-19 15:19:47.324334 testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    33497 2024-03-16 23:20:07.000000 testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/bin/github-hetzner-runners
+-rw-rw-r--   0 user      (1000) user      (1000)    15625 2024-03-14 16:48:24.000000 testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/cloud.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-19 15:19:47.324334 testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/config/
+-rw-rw-r--   0 user      (1000) user      (1000)      993 2024-03-14 16:48:24.000000 testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/config/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    24278 2024-03-14 16:48:24.000000 testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/config/config.py
+-rw-rw-r--   0 user      (1000) user      (1000)    13636 2024-03-14 16:48:24.000000 testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/config/schema.json
+-rw-rw-r--   0 user      (1000) user      (1000)     2574 2024-03-14 16:48:24.000000 testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/delete.py
+-rw-rw-r--   0 user      (1000) user      (1000)    14121 2024-03-19 14:55:14.000000 testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/estimate.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6743 2024-03-14 16:48:24.000000 testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/logger.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1926 2024-03-14 16:48:24.000000 testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)    26796 2024-03-16 19:51:24.000000 testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)    35850 2024-03-18 16:00:18.000000 testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-19 15:19:47.324334 testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2024-03-14 16:48:24.000000 testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-19 15:19:47.324334 testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2024-03-14 16:48:24.000000 testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      535 2024-03-14 16:48:24.000000 testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2024-03-14 16:48:24.000000 testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/scripts/none.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     1148 2024-03-14 16:48:24.000000 testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/scripts/setup-docker.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      260 2024-03-14 16:48:24.000000 testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      767 2024-03-17 13:54:38.000000 testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/scripts/startup-arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      759 2024-03-17 13:54:45.000000 testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/scripts/startup-x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     3206 2024-03-14 16:48:24.000000 testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2722 2024-03-14 16:48:24.000000 testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/servers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9056 2024-03-14 16:48:24.000000 testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1695 2024-03-14 16:48:24.000000 testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/shell.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2683 2024-03-16 20:04:55.000000 testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/streamingyaml.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-19 15:19:47.324334 testflows.github.hetzner.runners-1.7.240319.1151947/testflows.github.hetzner.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    19385 2024-03-19 15:19:47.000000 testflows.github.hetzner.runners-1.7.240319.1151947/testflows.github.hetzner.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1723 2024-03-19 15:19:47.000000 testflows.github.hetzner.runners-1.7.240319.1151947/testflows.github.hetzner.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-03-19 15:19:47.000000 testflows.github.hetzner.runners-1.7.240319.1151947/testflows.github.hetzner.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-03-15 23:34:11.000000 testflows.github.hetzner.runners-1.7.240319.1151947/testflows.github.hetzner.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       73 2024-03-19 15:19:47.000000 testflows.github.hetzner.runners-1.7.240319.1151947/testflows.github.hetzner.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2024-03-19 15:19:47.000000 testflows.github.hetzner.runners-1.7.240319.1151947/testflows.github.hetzner.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.hetzner.runners-1.7.240318.1205504/LICENSE` & `testflows.github.hetzner.runners-1.7.240319.1151947/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.hetzner.runners-1.7.240318.1205504/PKG-INFO` & `testflows.github.hetzner.runners-1.7.240319.1151947/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.hetzner.runners
-Version: 1.7.240318.1205504
+Version: 1.7.240319.1151947
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/testflows-github-hetzner-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `testflows.github.hetzner.runners-1.7.240318.1205504/README.rst` & `testflows.github.hetzner.runners-1.7.240319.1151947/README.rst`

 * *Files identical despite different names*

### Comparing `testflows.github.hetzner.runners-1.7.240318.1205504/setup.py` & `testflows.github.hetzner.runners-1.7.240319.1151947/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.hetzner.runners",
-    version="1.7.240318.1205504",
+    version="1.7.240319.1151947",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/testflows-github-hetzner-runners",
     classifiers=[
```

### Comparing `testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/__init__.py` & `testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 __author__ = "Vitaliy Zakaznikov"
-__version__ = "1.7.240318.1205504"
+__version__ = "1.7.240319.1151947"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/actions.py` & `testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/actions.py`

 * *Files identical despite different names*

### Comparing `testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/api_watch.py` & `testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/api_watch.py`

 * *Files identical despite different names*

### Comparing `testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/args.py` & `testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/args.py`

 * *Files identical despite different names*

### Comparing `testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/bin/github-hetzner-runners` & `testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/bin/github-hetzner-runners`

 * *Files identical despite different names*

### Comparing `testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/cloud.py` & `testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/cloud.py`

 * *Files identical despite different names*

### Comparing `testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/config/__init__.py` & `testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/config/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/config/config.py` & `testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/config/config.py`

 * *Files identical despite different names*

### Comparing `testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/config/schema.json` & `testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/config/schema.json`

 * *Files identical despite different names*

### Comparing `testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/delete.py` & `testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/delete.py`

 * *Files identical despite different names*

### Comparing `testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/estimate.py` & `testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/estimate.py`

 * *Files 6% similar despite different names*

```diff
@@ -176,14 +176,15 @@
     jobs: list[WorkflowJob],
     server_prices: dict[str, dict[str, float]],
     ipv4_price: float,
     ipv6_price: float,
 ):
     """Collect estimate for the given jobs."""
 
+    servers = {}
     best_estimate, worst_estimate = None, None
     total_duration, unknown_duration = None, None
     unknown_jobs = 0
 
     for i, job in enumerate(jobs, 1):
         duration = None
 
@@ -210,43 +211,81 @@
         }
 
         price, server_type, server_location = get_runner_server_price_per_second(
             server_prices, runner_name, ipv4_price, ipv6_price
         )
 
         job_entry["estimate"] = {
-            "server_type": server_type,
-            "server_location": server_location,
-            "server_price": (price * 3600) if price is not None else price,
+            "servers": [
+                {
+                    "type": server_type,
+                    "location": server_location,
+                    "price": (price * 3600) if price is not None else price,
+                    "duration": None,
+                    "worst": None,
+                    "best": None,
+                }
+            ],
             "worst": None,
             "best": None,
         }
 
+        if not (server_type, server_location) in servers:
+            servers[(server_type, server_location)] = {
+                "price": job_entry["estimate"]["servers"][0]["price"],
+                "duration": None,
+                "worst": None,
+                "best": None,
+            }
+
+        server = servers[(server_type, server_location)]
+
         if duration is not None:
             if unknown_duration is None:
                 unknown_duration = timedelta()
             if total_duration is None:
                 total_duration = timedelta()
 
+            server["duration"] = (
+                server["duration"] if server["duration"] is not None else timedelta()
+            ) + duration
+
+            job_entry["estimate"]["servers"][0]["duration"] = duration_str(
+                server["duration"]
+            )
+
         if price is not None and duration is not None:
             job_best_estimate = duration.total_seconds() * price
             job_worst_estimate = (
                 math.ceil(duration.total_seconds() / 3600) * 3600 * price
             )
             # update total
             best_estimate = (
                 best_estimate if best_estimate is not None else 0
             ) + job_best_estimate
             worst_estimate = (
                 worst_estimate if worst_estimate is not None else 0
             ) + job_worst_estimate
 
+            job_entry["estimate"]["servers"][0]["worst"] = job_worst_estimate
+            job_entry["estimate"]["servers"][0]["best"] = job_best_estimate
+
+            # estimates for the server are the same as the whole job
+            # as only 1 server is used per job
             job_entry["estimate"]["worst"] = job_worst_estimate
             job_entry["estimate"]["best"] = job_best_estimate
 
+            # update server["worst"] and server["best"] total estimates
+            server["best"] = (
+                server["best"] if server["best"] is not None else 0
+            ) + job_best_estimate
+            server["worst"] = (
+                server["worst"] if server["worst"] is not None else 0
+            ) + job_worst_estimate
+
         else:
             unknown_jobs += 1
             if duration is not None:
                 unknown_duration += duration
 
         if duration is not None:
             total_duration += duration
@@ -254,14 +293,15 @@
         writer.add_list_element(value=job_entry)
 
     return (
         i,
         total_duration,
         unknown_jobs,
         unknown_duration,
+        servers,
         worst_estimate,
         best_estimate,
     )
 
 
 def workflow_run(
     args,
@@ -304,31 +344,57 @@
         jobs_writer = list_value_writer.add_key("jobs")
 
         (
             count,
             total_duration,
             unknown_jobs,
             unknown_duration,
+            servers,
             worst_estimate,
             best_estimate,
         ) = get_estimate_for_jobs(
             jobs_writer, jobs, server_prices, args.ipv4_price, args.ipv6_price
         )
 
         workflow_totals = {}
-        workflow_totals["total_jobs"] = count
-        workflow_totals["total_duration"] = duration_str(total_duration)
-        workflow_totals["known_jobs"] = count - unknown_jobs
-        workflow_totals["known_duration"] = duration_str(
-            (total_duration - unknown_duration) if total_duration is not None else None
-        )
-        workflow_totals["unknown_jobs"] = unknown_jobs
-        workflow_totals["unknown_duration"] = duration_str(unknown_duration)
-        workflow_totals["worst_estimate"] = worst_estimate
-        workflow_totals["best_estimate"] = best_estimate
+
+        workflow_totals["total"] = {
+            "jobs": count,
+            "duration": duration_str(total_duration),
+        }
+        workflow_totals["known"] = {
+            "jobs": count - unknown_jobs,
+            "duration": duration_str(
+                (total_duration - unknown_duration)
+                if total_duration is not None
+                else None
+            ),
+        }
+        workflow_totals["unknown"] = {
+            "jobs": unknown_jobs,
+            "duration": duration_str(unknown_duration),
+        }
+        workflow_totals["estimate"] = {
+            "servers": [],
+            "worst": worst_estimate,
+            "best": best_estimate,
+        }
+
+        for server_type, server_location in servers:
+            server = servers[(server_type, server_location)]
+            workflow_totals["estimate"]["servers"].append(
+                {
+                    "type": server_type,
+                    "location": server_location,
+                    "price": server["price"],
+                    "duration": duration_str(server["duration"]),
+                    "worst": server["worst"],
+                    "best": server["best"],
+                }
+            )
 
         list_value_writer.add_value(workflow_totals)
 
 
 def workflow_runs(args, config: Config):
     """Estimate cost for different workflow runs."""
     repo, server_prices = login_and_get_prices(args, config)
```

### Comparing `testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/logger.py` & `testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/logger.py`

 * *Files identical despite different names*

### Comparing `testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/request.py` & `testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/scale_down.py` & `testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/scale_down.py`

 * *Files identical despite different names*

### Comparing `testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/scale_up.py` & `testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/scale_up.py`

 * *Files identical despite different names*

### Comparing `testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/scripts/__init__.py` & `testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/scripts/deploy/__init__.py` & `testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/scripts/deploy/setup.sh` & `testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/scripts/deploy/setup.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/scripts/setup-docker.sh` & `testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/scripts/setup-docker.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/scripts/startup-arm64.sh` & `testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/scripts/startup-arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/scripts/startup-x64.sh` & `testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/scripts/startup-x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/server.py` & `testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/server.py`

 * *Files identical despite different names*

### Comparing `testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/servers.py` & `testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/servers.py`

 * *Files identical despite different names*

### Comparing `testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/service.py` & `testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/service.py`

 * *Files identical despite different names*

### Comparing `testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/shell.py` & `testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.hetzner.runners-1.7.240318.1205504/testflows/github/hetzner/runners/streamingyaml.py` & `testflows.github.hetzner.runners-1.7.240319.1151947/testflows/github/hetzner/runners/streamingyaml.py`

 * *Files identical despite different names*

### Comparing `testflows.github.hetzner.runners-1.7.240318.1205504/testflows.github.hetzner.runners.egg-info/PKG-INFO` & `testflows.github.hetzner.runners-1.7.240319.1151947/testflows.github.hetzner.runners.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.hetzner.runners
-Version: 1.7.240318.1205504
+Version: 1.7.240319.1151947
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/testflows-github-hetzner-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `testflows.github.hetzner.runners-1.7.240318.1205504/testflows.github.hetzner.runners.egg-info/SOURCES.txt` & `testflows.github.hetzner.runners-1.7.240319.1151947/testflows.github.hetzner.runners.egg-info/SOURCES.txt`

 * *Files identical despite different names*

