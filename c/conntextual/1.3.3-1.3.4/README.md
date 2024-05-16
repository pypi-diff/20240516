# Comparing `tmp/conntextual-1.3.3.tar.gz` & `tmp/conntextual-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conntextual-1.3.3.tar", last modified: Thu Apr 11 07:02:55 2024, max compression
+gzip compressed data, was "conntextual-1.3.4.tar", last modified: Thu May 16 03:04:02 2024, max compression
```

## Comparing `conntextual-1.3.3.tar` & `conntextual-1.3.4.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:02:55.922390 conntextual-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-11 07:01:07.000000 conntextual-1.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-04-11 07:02:55.922390 conntextual-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-11 07:01:07.000000 conntextual-1.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:02:55.918390 conntextual-1.3.3/conntextual/
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-11 07:01:07.000000 conntextual-1.3.3/conntextual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-11 07:01:07.000000 conntextual-1.3.3/conntextual/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-11 07:01:07.000000 conntextual-1.3.3/conntextual/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-11 07:01:07.000000 conntextual-1.3.3/conntextual/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:02:55.918390 conntextual-1.3.3/conntextual/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 07:01:07.000000 conntextual-1.3.3/conntextual/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-11 07:01:07.000000 conntextual-1.3.3/conntextual/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-11 07:01:07.000000 conntextual-1.3.3/conntextual/commands/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-11 07:01:07.000000 conntextual-1.3.3/conntextual/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-11 07:01:07.000000 conntextual-1.3.3/conntextual/commands/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:02:55.918390 conntextual-1.3.3/conntextual/curses/
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-11 07:01:07.000000 conntextual-1.3.3/conntextual/curses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-11 07:01:07.000000 conntextual-1.3.3/conntextual/curses/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-11 07:01:07.000000 conntextual-1.3.3/conntextual/curses/tui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:02:55.918390 conntextual-1.3.3/conntextual/data/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-11 07:01:07.000000 conntextual-1.3.3/conntextual/data/app.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-11 07:01:07.000000 conntextual-1.3.3/conntextual/data/curses.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-11 07:01:07.000000 conntextual-1.3.3/conntextual/data/headless.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-11 07:01:07.000000 conntextual-1.3.3/conntextual/data/json.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-11 07:01:07.000000 conntextual-1.3.3/conntextual/data/sample.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:02:55.918390 conntextual-1.3.3/conntextual/data/tcss/
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-11 07:01:07.000000 conntextual-1.3.3/conntextual/data/tcss/base.tcss
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-11 07:01:07.000000 conntextual-1.3.3/conntextual/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-11 07:01:07.000000 conntextual-1.3.3/conntextual/entry.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 07:01:07.000000 conntextual-1.3.3/conntextual/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-11 07:01:07.000000 conntextual-1.3.3/conntextual/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-04-11 07:01:07.000000 conntextual-1.3.3/conntextual/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:02:55.922390 conntextual-1.3.3/conntextual/ui/
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-04-11 07:01:07.000000 conntextual-1.3.3/conntextual/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7739 2024-04-11 07:01:07.000000 conntextual-1.3.3/conntextual/ui/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:02:55.922390 conntextual-1.3.3/conntextual/ui/channel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 07:01:07.000000 conntextual-1.3.3/conntextual/ui/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-11 07:01:07.000000 conntextual-1.3.3/conntextual/ui/channel/color.py
--rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-04-11 07:01:07.000000 conntextual-1.3.3/conntextual/ui/channel/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-11 07:01:07.000000 conntextual-1.3.3/conntextual/ui/channel/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-11 07:01:07.000000 conntextual-1.3.3/conntextual/ui/channel/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-11 07:01:07.000000 conntextual-1.3.3/conntextual/ui/channel/pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-11 07:01:07.000000 conntextual-1.3.3/conntextual/ui/channel/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-11 07:01:07.000000 conntextual-1.3.3/conntextual/ui/channel/selected.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-11 07:01:07.000000 conntextual-1.3.3/conntextual/ui/channel/suggester.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-11 07:01:07.000000 conntextual-1.3.3/conntextual/ui/footer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-11 07:01:07.000000 conntextual-1.3.3/conntextual/ui/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-04-11 07:01:07.000000 conntextual-1.3.3/conntextual/ui/task.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-11 07:01:07.000000 conntextual-1.3.3/conntextual/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:02:55.922390 conntextual-1.3.3/conntextual.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-04-11 07:02:55.000000 conntextual-1.3.3/conntextual.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-11 07:02:55.000000 conntextual-1.3.3/conntextual.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 07:02:55.000000 conntextual-1.3.3/conntextual.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-11 07:02:55.000000 conntextual-1.3.3/conntextual.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-11 07:02:55.000000 conntextual-1.3.3/conntextual.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-11 07:02:55.000000 conntextual-1.3.3/conntextual.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-11 07:01:07.000000 conntextual-1.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 07:02:55.922390 conntextual-1.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-11 07:01:07.000000 conntextual-1.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:02:55.922390 conntextual-1.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-11 07:01:07.000000 conntextual-1.3.3/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-11 07:01:07.000000 conntextual-1.3.3/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:04:02.539195 conntextual-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-16 03:02:19.000000 conntextual-1.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-05-16 03:04:02.539195 conntextual-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-05-16 03:02:19.000000 conntextual-1.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:04:02.531195 conntextual-1.3.4/conntextual/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-16 03:02:19.000000 conntextual-1.3.4/conntextual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-16 03:02:19.000000 conntextual-1.3.4/conntextual/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-16 03:02:19.000000 conntextual-1.3.4/conntextual/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-16 03:02:19.000000 conntextual-1.3.4/conntextual/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:04:02.535195 conntextual-1.3.4/conntextual/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 03:02:19.000000 conntextual-1.3.4/conntextual/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-16 03:02:19.000000 conntextual-1.3.4/conntextual/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-16 03:02:19.000000 conntextual-1.3.4/conntextual/commands/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-16 03:02:19.000000 conntextual-1.3.4/conntextual/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-16 03:02:19.000000 conntextual-1.3.4/conntextual/commands/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:04:02.535195 conntextual-1.3.4/conntextual/curses/
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-16 03:02:19.000000 conntextual-1.3.4/conntextual/curses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-16 03:02:19.000000 conntextual-1.3.4/conntextual/curses/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-16 03:02:19.000000 conntextual-1.3.4/conntextual/curses/tui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:04:02.535195 conntextual-1.3.4/conntextual/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-16 03:02:19.000000 conntextual-1.3.4/conntextual/data/app.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-16 03:02:19.000000 conntextual-1.3.4/conntextual/data/curses.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-16 03:02:19.000000 conntextual-1.3.4/conntextual/data/headless.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-16 03:02:19.000000 conntextual-1.3.4/conntextual/data/json.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-16 03:02:19.000000 conntextual-1.3.4/conntextual/data/sample.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:04:02.535195 conntextual-1.3.4/conntextual/data/tcss/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-16 03:02:19.000000 conntextual-1.3.4/conntextual/data/tcss/base.tcss
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-16 03:02:19.000000 conntextual-1.3.4/conntextual/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-16 03:02:19.000000 conntextual-1.3.4/conntextual/entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 03:02:19.000000 conntextual-1.3.4/conntextual/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-16 03:02:19.000000 conntextual-1.3.4/conntextual/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-16 03:02:19.000000 conntextual-1.3.4/conntextual/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:04:02.535195 conntextual-1.3.4/conntextual/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-16 03:02:19.000000 conntextual-1.3.4/conntextual/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7739 2024-05-16 03:02:19.000000 conntextual-1.3.4/conntextual/ui/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:04:02.539195 conntextual-1.3.4/conntextual/ui/channel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 03:02:19.000000 conntextual-1.3.4/conntextual/ui/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-16 03:02:19.000000 conntextual-1.3.4/conntextual/ui/channel/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-05-16 03:02:19.000000 conntextual-1.3.4/conntextual/ui/channel/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-05-16 03:02:19.000000 conntextual-1.3.4/conntextual/ui/channel/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-16 03:02:19.000000 conntextual-1.3.4/conntextual/ui/channel/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-16 03:02:19.000000 conntextual-1.3.4/conntextual/ui/channel/pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-16 03:02:19.000000 conntextual-1.3.4/conntextual/ui/channel/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-16 03:02:19.000000 conntextual-1.3.4/conntextual/ui/channel/selected.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-16 03:02:19.000000 conntextual-1.3.4/conntextual/ui/channel/suggester.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-16 03:02:19.000000 conntextual-1.3.4/conntextual/ui/footer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-16 03:02:19.000000 conntextual-1.3.4/conntextual/ui/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-05-16 03:02:19.000000 conntextual-1.3.4/conntextual/ui/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-16 03:02:19.000000 conntextual-1.3.4/conntextual/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:04:02.539195 conntextual-1.3.4/conntextual.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-05-16 03:04:02.000000 conntextual-1.3.4/conntextual.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-16 03:04:02.000000 conntextual-1.3.4/conntextual.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 03:04:02.000000 conntextual-1.3.4/conntextual.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-16 03:04:02.000000 conntextual-1.3.4/conntextual.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-16 03:04:02.000000 conntextual-1.3.4/conntextual.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-16 03:04:02.000000 conntextual-1.3.4/conntextual.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-16 03:02:19.000000 conntextual-1.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 03:04:02.539195 conntextual-1.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-16 03:02:19.000000 conntextual-1.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:04:02.539195 conntextual-1.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-16 03:02:19.000000 conntextual-1.3.4/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-16 03:02:19.000000 conntextual-1.3.4/tests/test_resources.py
```

### Comparing `conntextual-1.3.3/LICENSE` & `conntextual-1.3.4/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vaughn Kottler
+Copyright (c) 2024 Vaughn Kottler
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `conntextual-1.3.3/PKG-INFO` & `conntextual-1.3.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conntextual
-Version: 1.3.3
+Version: 1.3.4
 Summary: A network-application TUI using textual.
 Home-page: https://github.com/vkottler/conntextual
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -13,20 +13,20 @@
 Classifier: Operating System :: Unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: textual
-Requires-Dist: runtimepy>=2.12.3
-Requires-Dist: uvloop
-Requires-Dist: aiohttp>=3.9.0b0
-Requires-Dist: textual-plotext
 Requires-Dist: numpy
 Requires-Dist: psutil
+Requires-Dist: textual-plotext
+Requires-Dist: runtimepy>=4.4.3
+Requires-Dist: aiohttp>=3.9.0b0
+Requires-Dist: uvloop
 Provides-Extra: test
 Requires-Dist: pylint; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: isort; extra == "test"
@@ -39,19 +39,19 @@
 Requires-Dist: types-psutil; extra == "test"
 Requires-Dist: types-setuptools; extra == "test"
 
 <!--
     =====================================
     generator=datazen
     version=3.1.4
-    hash=8b302ab6c9f0ef6558a1aeb77a875edb
+    hash=1c09a2d5cb8a5fe2b20a06aef6ff1564
     =====================================
 -->
 
-# conntextual ([1.3.3](https://pypi.org/project/conntextual/))
+# conntextual ([1.3.4](https://pypi.org/project/conntextual/))
 
 [![python](https://img.shields.io/pypi/pyversions/conntextual.svg)](https://pypi.org/project/conntextual/)
 ![Build Status](https://github.com/vkottler/conntextual/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/conntextual/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/conntextual)
 ![PyPI - Status](https://img.shields.io/pypi/status/conntextual)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/conntextual)
```

### Comparing `conntextual-1.3.3/README.md` & `conntextual-1.3.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.4
-    hash=8b302ab6c9f0ef6558a1aeb77a875edb
+    hash=1c09a2d5cb8a5fe2b20a06aef6ff1564
     =====================================
 -->
 
-# conntextual ([1.3.3](https://pypi.org/project/conntextual/))
+# conntextual ([1.3.4](https://pypi.org/project/conntextual/))
 
 [![python](https://img.shields.io/pypi/pyversions/conntextual.svg)](https://pypi.org/project/conntextual/)
 ![Build Status](https://github.com/vkottler/conntextual/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/conntextual/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/conntextual)
 ![PyPI - Status](https://img.shields.io/pypi/status/conntextual)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/conntextual)
```

### Comparing `conntextual-1.3.3/conntextual/app.py` & `conntextual-1.3.4/conntextual/app.py`

 * *Files identical despite different names*

### Comparing `conntextual-1.3.3/conntextual/client.py` & `conntextual-1.3.4/conntextual/client.py`

 * *Files identical despite different names*

### Comparing `conntextual-1.3.3/conntextual/commands/all.py` & `conntextual-1.3.4/conntextual/commands/all.py`

 * *Files identical despite different names*

### Comparing `conntextual-1.3.3/conntextual/commands/client.py` & `conntextual-1.3.4/conntextual/commands/client.py`

 * *Files identical despite different names*

### Comparing `conntextual-1.3.3/conntextual/commands/common.py` & `conntextual-1.3.4/conntextual/commands/common.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,16 @@
 
     if not args.verbose and not is_headless:
         flags.add("--quiet")
 
     cli_args.extend(flags)
 
     cli_args.append(args.cmd)
-    cli_args.extend(list(forward_flags(args, ["init_only"])))
+
+    cli_args.extend(list(forward_flags(args, ["init_only", "no_poller"])))
 
     # Ensure that the application continues to run when running the user
     # interface.
     if not is_headless or args.wait_for_stop:
         cli_args.append("--wait-for-stop")
 
     cli_args.extend(args.configs)
```

### Comparing `conntextual-1.3.3/conntextual/commands/ui.py` & `conntextual-1.3.4/conntextual/commands/ui.py`

 * *Files identical despite different names*

### Comparing `conntextual-1.3.3/conntextual/curses/base.py` & `conntextual-1.3.4/conntextual/curses/base.py`

 * *Files identical despite different names*

### Comparing `conntextual-1.3.3/conntextual/curses/tui.py` & `conntextual-1.3.4/conntextual/curses/tui.py`

 * *Files identical despite different names*

### Comparing `conntextual-1.3.3/conntextual/data/tcss/base.tcss` & `conntextual-1.3.4/conntextual/data/tcss/base.tcss`

 * *Files identical despite different names*

### Comparing `conntextual-1.3.3/conntextual/entry.py` & `conntextual-1.3.4/conntextual/entry.py`

 * *Files identical despite different names*

### Comparing `conntextual-1.3.3/conntextual/server.py` & `conntextual-1.3.4/conntextual/server.py`

 * *Files identical despite different names*

### Comparing `conntextual-1.3.3/conntextual/ui/__init__.py` & `conntextual-1.3.4/conntextual/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `conntextual-1.3.3/conntextual/ui/base.py` & `conntextual-1.3.4/conntextual/ui/base.py`

 * *Files identical despite different names*

### Comparing `conntextual-1.3.3/conntextual/ui/channel/color.py` & `conntextual-1.3.4/conntextual/ui/channel/color.py`

 * *Files identical despite different names*

### Comparing `conntextual-1.3.3/conntextual/ui/channel/environment.py` & `conntextual-1.3.4/conntextual/ui/channel/environment.py`

 * *Files identical despite different names*

### Comparing `conntextual-1.3.3/conntextual/ui/channel/log.py` & `conntextual-1.3.4/conntextual/ui/channel/log.py`

 * *Files identical despite different names*

### Comparing `conntextual-1.3.3/conntextual/ui/channel/model.py` & `conntextual-1.3.4/conntextual/ui/channel/model.py`

 * *Files identical despite different names*

### Comparing `conntextual-1.3.3/conntextual/ui/channel/pattern.py` & `conntextual-1.3.4/conntextual/ui/channel/pattern.py`

 * *Files identical despite different names*

### Comparing `conntextual-1.3.3/conntextual/ui/channel/plot.py` & `conntextual-1.3.4/conntextual/ui/channel/plot.py`

 * *Files identical despite different names*

### Comparing `conntextual-1.3.3/conntextual/ui/channel/selected.py` & `conntextual-1.3.4/conntextual/ui/channel/selected.py`

 * *Files identical despite different names*

### Comparing `conntextual-1.3.3/conntextual/ui/channel/suggester.py` & `conntextual-1.3.4/conntextual/ui/channel/suggester.py`

 * *Files identical despite different names*

### Comparing `conntextual-1.3.3/conntextual/ui/footer.py` & `conntextual-1.3.4/conntextual/ui/footer.py`

 * *Files identical despite different names*

### Comparing `conntextual-1.3.3/conntextual/ui/model.py` & `conntextual-1.3.4/conntextual/ui/model.py`

 * *Files identical despite different names*

### Comparing `conntextual-1.3.3/conntextual/ui/task.py` & `conntextual-1.3.4/conntextual/ui/task.py`

 * *Files identical despite different names*

### Comparing `conntextual-1.3.3/conntextual.egg-info/PKG-INFO` & `conntextual-1.3.4/conntextual.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conntextual
-Version: 1.3.3
+Version: 1.3.4
 Summary: A network-application TUI using textual.
 Home-page: https://github.com/vkottler/conntextual
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -13,20 +13,20 @@
 Classifier: Operating System :: Unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: textual
-Requires-Dist: runtimepy>=2.12.3
-Requires-Dist: uvloop
-Requires-Dist: aiohttp>=3.9.0b0
-Requires-Dist: textual-plotext
 Requires-Dist: numpy
 Requires-Dist: psutil
+Requires-Dist: textual-plotext
+Requires-Dist: runtimepy>=4.4.3
+Requires-Dist: aiohttp>=3.9.0b0
+Requires-Dist: uvloop
 Provides-Extra: test
 Requires-Dist: pylint; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: isort; extra == "test"
@@ -39,19 +39,19 @@
 Requires-Dist: types-psutil; extra == "test"
 Requires-Dist: types-setuptools; extra == "test"
 
 <!--
     =====================================
     generator=datazen
     version=3.1.4
-    hash=8b302ab6c9f0ef6558a1aeb77a875edb
+    hash=1c09a2d5cb8a5fe2b20a06aef6ff1564
     =====================================
 -->
 
-# conntextual ([1.3.3](https://pypi.org/project/conntextual/))
+# conntextual ([1.3.4](https://pypi.org/project/conntextual/))
 
 [![python](https://img.shields.io/pypi/pyversions/conntextual.svg)](https://pypi.org/project/conntextual/)
 ![Build Status](https://github.com/vkottler/conntextual/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/conntextual/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/conntextual)
 ![PyPI - Status](https://img.shields.io/pypi/status/conntextual)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/conntextual)
```

### Comparing `conntextual-1.3.3/conntextual.egg-info/SOURCES.txt` & `conntextual-1.3.4/conntextual.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `conntextual-1.3.3/pyproject.toml` & `conntextual-1.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "conntextual"
-version = "1.3.3"
+version = "1.3.4"
 description = "A network-application TUI using textual."
 readme = "README.md"
 requires-python = ">=3.11"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `conntextual-1.3.3/setup.py` & `conntextual-1.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `conntextual-1.3.3/tests/test_entry.py` & `conntextual-1.3.4/tests/test_entry.py`

 * *Files identical despite different names*

