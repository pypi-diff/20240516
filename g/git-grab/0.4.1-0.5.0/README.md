# Comparing `tmp/git-grab-0.4.1.tar.gz` & `tmp/git_grab-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/git-grab-0.4.1.tar", last modified: Sat Nov  7 17:31:54 2020, max compression
+gzip compressed data, was "git_grab-0.5.0.tar", max compression
```

## Comparing `git-grab-0.4.1.tar` & `git_grab-0.5.0.tar`

### file list

```diff
@@ -1,23 +1,6 @@
-drwxr-xr-x   0 boomatang  (1000) boomatang  (1000)        0 2020-11-07 17:31:54.160365 git-grab-0.4.1/
--rw-r--r--   0 boomatang  (1000) boomatang  (1000)     1070 2019-09-18 17:59:19.000000 git-grab-0.4.1/LICENSE
--rw-r--r--   0 boomatang  (1000) boomatang  (1000)      197 2019-09-18 17:59:19.000000 git-grab-0.4.1/MANIFEST.in
--rw-r--r--   0 boomatang  (1000) boomatang  (1000)     4411 2020-11-07 17:31:54.160365 git-grab-0.4.1/PKG-INFO
--rw-r--r--   0 boomatang  (1000) boomatang  (1000)     2759 2020-10-06 19:46:00.000000 git-grab-0.4.1/README.md
--rw-r--r--   0 boomatang  (1000) boomatang  (1000)      114 2020-11-07 17:31:54.160365 git-grab-0.4.1/setup.cfg
--rw-r--r--   0 boomatang  (1000) boomatang  (1000)     1640 2020-11-07 17:03:20.000000 git-grab-0.4.1/setup.py
-drwxr-xr-x   0 boomatang  (1000) boomatang  (1000)        0 2020-11-07 17:31:54.160365 git-grab-0.4.1/src/
-drwxr-xr-x   0 boomatang  (1000) boomatang  (1000)        0 2020-11-07 17:31:54.160365 git-grab-0.4.1/src/git_grab.egg-info/
--rw-r--r--   0 boomatang  (1000) boomatang  (1000)     4411 2020-11-07 17:31:54.000000 git-grab-0.4.1/src/git_grab.egg-info/PKG-INFO
--rw-r--r--   0 boomatang  (1000) boomatang  (1000)      360 2020-11-07 17:31:54.000000 git-grab-0.4.1/src/git_grab.egg-info/SOURCES.txt
--rw-r--r--   0 boomatang  (1000) boomatang  (1000)        1 2020-11-07 17:31:54.000000 git-grab-0.4.1/src/git_grab.egg-info/dependency_links.txt
--rw-r--r--   0 boomatang  (1000) boomatang  (1000)       44 2020-11-07 17:31:54.000000 git-grab-0.4.1/src/git_grab.egg-info/entry_points.txt
--rw-r--r--   0 boomatang  (1000) boomatang  (1000)       63 2020-11-07 17:31:54.000000 git-grab-0.4.1/src/git_grab.egg-info/requires.txt
--rw-r--r--   0 boomatang  (1000) boomatang  (1000)        5 2020-11-07 17:31:54.000000 git-grab-0.4.1/src/git_grab.egg-info/top_level.txt
-drwxr-xr-x   0 boomatang  (1000) boomatang  (1000)        0 2020-11-07 17:31:54.160365 git-grab-0.4.1/src/grab/
--rw-r--r--   0 boomatang  (1000) boomatang  (1000)      180 2020-11-07 17:28:13.000000 git-grab-0.4.1/src/grab/__init__.py
--rw-r--r--   0 boomatang  (1000) boomatang  (1000)    18457 2020-11-07 17:30:54.000000 git-grab-0.4.1/src/grab/api.py
--rw-r--r--   0 boomatang  (1000) boomatang  (1000)     3428 2020-10-06 19:49:55.000000 git-grab-0.4.1/src/grab/cli.py
--rw-r--r--   0 boomatang  (1000) boomatang  (1000)      859 2019-11-10 16:21:27.000000 git-grab-0.4.1/src/grab/helper.py
-drwxr-xr-x   0 boomatang  (1000) boomatang  (1000)        0 2020-11-07 17:31:54.160365 git-grab-0.4.1/tests/
-drwxr-xr-x   0 boomatang  (1000) boomatang  (1000)        0 2020-11-07 17:31:54.160365 git-grab-0.4.1/tests/api/
--rw-r--r--   0 boomatang  (1000) boomatang  (1000)     2886 2019-12-19 21:15:55.000000 git-grab-0.4.1/tests/api/test_api.py
+-rw-r--r--   0        0        0     1070 2023-07-01 11:42:16.859119 git_grab-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1621 2024-05-16 20:11:19.151203 git_grab-0.5.0/README.md
+-rw-r--r--   0        0        0      161 2024-05-16 20:11:19.153203 git_grab-0.5.0/git_grab/__init__.py
+-rw-r--r--   0        0        0     6365 2024-05-16 20:11:19.154203 git_grab-0.5.0/git_grab/cli.py
+-rw-r--r--   0        0        0     1011 2024-05-16 20:11:19.156203 git_grab-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2308 1970-01-01 00:00:00.000000 git_grab-0.5.0/PKG-INFO
```

### Comparing `git-grab-0.4.1/LICENSE` & `git_grab-0.5.0/LICENSE`

 * *Files identical despite different names*

