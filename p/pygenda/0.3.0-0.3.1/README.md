# Comparing `tmp/pygenda-0.3.0.tar.gz` & `tmp/pygenda-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygenda-0.3.0.tar", last modified: Tue Oct 31 22:15:32 2023, max compression
+gzip compressed data, was "pygenda-0.3.1.tar", last modified: Sun Dec 31 08:43:17 2023, max compression
```

## Comparing `pygenda-0.3.0.tar` & `pygenda-0.3.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwx------   0 matt      (1000) users      (100)        0 2023-10-31 22:15:32.977042 pygenda-0.3.0/
--rw-------   0 matt      (1000) users      (100)    35149 2022-01-30 22:37:16.000000 pygenda-0.3.0/COPYING
--rw-------   0 matt      (1000) users      (100)      275 2023-07-10 13:51:19.000000 pygenda-0.3.0/MANIFEST.in
--rw-------   0 matt      (1000) users      (100)     1015 2023-10-31 22:15:32.977042 pygenda-0.3.0/PKG-INFO
--rw-------   0 matt      (1000) users      (100)     6363 2023-10-31 22:04:55.000000 pygenda-0.3.0/README.md
-drwx------   0 matt      (1000) users      (100)        0 2023-10-31 22:15:32.962042 pygenda-0.3.0/csrc/
--rw-------   0 matt      (1000) users      (100)      814 2023-10-31 12:46:41.000000 pygenda-0.3.0/csrc/CMakeLists.txt
--rw-------   0 matt      (1000) users      (100)     3043 2023-07-10 13:51:19.000000 pygenda-0.3.0/csrc/pygenda_clipboard.c
-drwx------   0 matt      (1000) users      (100)        0 2023-10-31 22:15:32.968042 pygenda-0.3.0/pygenda/
--rwx------   0 matt      (1000) users      (100)      823 2023-06-10 21:22:42.000000 pygenda-0.3.0/pygenda/__main__.py
-drwx------   0 matt      (1000) users      (100)        0 2023-10-31 22:15:32.970042 pygenda-0.3.0/pygenda/app/
--rw-------   0 matt      (1000) users      (100)      369 2023-07-10 13:51:19.000000 pygenda-0.3.0/pygenda/app/pygenda.desktop
-drwx------   0 matt      (1000) users      (100)        0 2023-10-31 22:15:32.974042 pygenda-0.3.0/pygenda/css/
--rw-------   0 matt      (1000) users      (100)      288 2022-01-30 22:37:16.000000 pygenda-0.3.0/pygenda/css/disc+loop+star.svg
--rw-------   0 matt      (1000) users      (100)      215 2022-01-30 22:37:16.000000 pygenda-0.3.0/pygenda/css/disc+loop.svg
--rw-------   0 matt      (1000) users      (100)      208 2022-01-30 22:37:16.000000 pygenda-0.3.0/pygenda/css/disc+star.svg
--rw-------   0 matt      (1000) users      (100)      135 2022-01-30 22:37:16.000000 pygenda-0.3.0/pygenda/css/disc.svg
--rw-------   0 matt      (1000) users      (100)     3876 2023-10-31 12:46:41.000000 pygenda-0.3.0/pygenda/css/gemini.css
--rw-------   0 matt      (1000) users      (100)      223 2022-01-30 22:37:16.000000 pygenda-0.3.0/pygenda/css/loop+star.svg
--rw-------   0 matt      (1000) users      (100)      150 2022-01-30 22:37:16.000000 pygenda-0.3.0/pygenda/css/loop.svg
--rw-------   0 matt      (1000) users      (100)    16321 2023-10-31 12:46:41.000000 pygenda-0.3.0/pygenda/css/pygenda.css
--rw-------   0 matt      (1000) users      (100)      103 2023-10-06 15:06:24.000000 pygenda-0.3.0/pygenda/css/raspberrypi.css
--rw-------   0 matt      (1000) users      (100)      150 2022-01-30 22:37:16.000000 pygenda-0.3.0/pygenda/css/star.svg
-drwx------   0 matt      (1000) users      (100)        0 2023-10-31 22:15:32.976042 pygenda-0.3.0/pygenda/glade/
--rw-------   0 matt      (1000) users      (100)    45187 2023-10-31 12:46:41.000000 pygenda-0.3.0/pygenda/glade/dialog_event.glade
--rw-------   0 matt      (1000) users      (100)     5150 2023-06-10 21:22:42.000000 pygenda-0.3.0/pygenda/glade/dialog_find.glade
--rw-------   0 matt      (1000) users      (100)    14668 2023-10-31 12:46:41.000000 pygenda-0.3.0/pygenda/glade/dialog_todo.glade
--rw-------   0 matt      (1000) users      (100)    33318 2023-10-31 12:46:41.000000 pygenda-0.3.0/pygenda/glade/main.glade
--rw-------   0 matt      (1000) users      (100)    28347 2023-10-25 11:06:47.000000 pygenda-0.3.0/pygenda/glade/main2.glade
--rw-------   0 matt      (1000) users      (100)     3892 2023-06-10 21:22:42.000000 pygenda-0.3.0/pygenda/glade/view_week.glade
--rw-------   0 matt      (1000) users      (100)     5931 2023-07-10 13:51:19.000000 pygenda-0.3.0/pygenda/glade/view_year.glade
-drwx------   0 matt      (1000) users      (100)        0 2023-10-31 22:15:32.960042 pygenda-0.3.0/pygenda/locale/
-drwx------   0 matt      (1000) users      (100)        0 2023-10-31 22:15:32.960042 pygenda-0.3.0/pygenda/locale/en_US/
-drwx------   0 matt      (1000) users      (100)        0 2023-10-31 22:15:32.976042 pygenda-0.3.0/pygenda/locale/en_US/LC_MESSAGES/
--rw-------   0 matt      (1000) users      (100)      536 2023-10-31 20:22:54.000000 pygenda-0.3.0/pygenda/locale/en_US/LC_MESSAGES/pygenda.mo
-drwx------   0 matt      (1000) users      (100)        0 2023-10-31 22:15:32.960042 pygenda-0.3.0/pygenda/locale/fr/
-drwx------   0 matt      (1000) users      (100)        0 2023-10-31 22:15:32.976042 pygenda-0.3.0/pygenda/locale/fr/LC_MESSAGES/
--rw-------   0 matt      (1000) users      (100)     9564 2023-10-31 20:22:54.000000 pygenda-0.3.0/pygenda/locale/fr/LC_MESSAGES/pygenda.mo
--rw-------   0 matt      (1000) users      (100)    73649 2023-10-31 20:22:54.000000 pygenda-0.3.0/pygenda/pygenda_calendar.py
--rw-------   0 matt      (1000) users      (100)     5767 2023-10-31 20:22:54.000000 pygenda-0.3.0/pygenda/pygenda_config.py
--rw-------   0 matt      (1000) users      (100)    10344 2023-10-31 12:46:41.000000 pygenda-0.3.0/pygenda/pygenda_dialog_entryprops.py
--rw-------   0 matt      (1000) users      (100)    75156 2023-10-31 12:46:41.000000 pygenda-0.3.0/pygenda/pygenda_dialog_event.py
--rw-------   0 matt      (1000) users      (100)     3538 2023-06-10 21:22:42.000000 pygenda-0.3.0/pygenda/pygenda_dialog_find.py
--rw-------   0 matt      (1000) users      (100)    15356 2023-10-31 12:46:41.000000 pygenda-0.3.0/pygenda/pygenda_dialog_todo.py
--rw-------   0 matt      (1000) users      (100)     4610 2023-10-31 12:46:41.000000 pygenda-0.3.0/pygenda/pygenda_entryinfo.py
--rw-------   0 matt      (1000) users      (100)    45368 2023-10-31 20:22:54.000000 pygenda-0.3.0/pygenda/pygenda_gui.py
--rw-------   0 matt      (1000) users      (100)    10419 2023-10-31 20:22:54.000000 pygenda-0.3.0/pygenda/pygenda_util.py
--rw-------   0 matt      (1000) users      (100)      300 2023-10-31 22:08:32.000000 pygenda-0.3.0/pygenda/pygenda_version.py
--rw-------   0 matt      (1000) users      (100)    15867 2023-10-31 20:22:54.000000 pygenda-0.3.0/pygenda/pygenda_view.py
--rw-------   0 matt      (1000) users      (100)    27380 2023-10-31 12:46:41.000000 pygenda-0.3.0/pygenda/pygenda_view_todo.py
--rw-------   0 matt      (1000) users      (100)    22867 2023-10-31 20:22:54.000000 pygenda-0.3.0/pygenda/pygenda_view_week.py
--rw-------   0 matt      (1000) users      (100)    28863 2023-10-31 12:46:41.000000 pygenda-0.3.0/pygenda/pygenda_view_year.py
--rw-------   0 matt      (1000) users      (100)    22195 2023-08-08 20:56:45.000000 pygenda-0.3.0/pygenda/pygenda_widgets.py
-drwx------   0 matt      (1000) users      (100)        0 2023-10-31 22:15:32.970042 pygenda-0.3.0/pygenda.egg-info/
--rw-------   0 matt      (1000) users      (100)     1015 2023-10-31 22:15:32.000000 pygenda-0.3.0/pygenda.egg-info/PKG-INFO
--rw-------   0 matt      (1000) users      (100)     1251 2023-10-31 22:15:32.000000 pygenda-0.3.0/pygenda.egg-info/SOURCES.txt
--rw-------   0 matt      (1000) users      (100)        1 2023-10-31 22:15:32.000000 pygenda-0.3.0/pygenda.egg-info/dependency_links.txt
--rw-------   0 matt      (1000) users      (100)       67 2023-10-31 22:15:32.000000 pygenda-0.3.0/pygenda.egg-info/requires.txt
--rw-------   0 matt      (1000) users      (100)        8 2023-10-31 22:15:32.000000 pygenda-0.3.0/pygenda.egg-info/top_level.txt
--rw-------   0 matt      (1000) users      (100)       38 2023-10-31 22:15:32.977042 pygenda-0.3.0/setup.cfg
--rwx------   0 matt      (1000) users      (100)     3898 2023-10-31 12:46:41.000000 pygenda-0.3.0/setup.py
+drwx------   0 matt      (1000) users      (100)        0 2023-12-31 08:43:17.774070 pygenda-0.3.1/
+-rw-------   0 matt      (1000) users      (100)    35149 2022-01-30 22:37:16.000000 pygenda-0.3.1/COPYING
+-rw-------   0 matt      (1000) users      (100)      275 2023-12-30 00:19:21.000000 pygenda-0.3.1/MANIFEST.in
+-rw-------   0 matt      (1000) users      (100)     1015 2023-12-31 08:43:17.774070 pygenda-0.3.1/PKG-INFO
+-rw-------   0 matt      (1000) users      (100)     6363 2023-12-30 00:19:21.000000 pygenda-0.3.1/README.md
+drwx------   0 matt      (1000) users      (100)        0 2023-12-31 08:43:17.767070 pygenda-0.3.1/csrc/
+-rw-------   0 matt      (1000) users      (100)      814 2023-12-30 00:19:21.000000 pygenda-0.3.1/csrc/CMakeLists.txt
+-rw-------   0 matt      (1000) users      (100)     3043 2023-12-30 00:19:21.000000 pygenda-0.3.1/csrc/pygenda_clipboard.c
+drwx------   0 matt      (1000) users      (100)        0 2023-12-31 08:43:17.769070 pygenda-0.3.1/pygenda/
+-rwx------   0 matt      (1000) users      (100)      823 2023-12-30 00:19:21.000000 pygenda-0.3.1/pygenda/__main__.py
+drwx------   0 matt      (1000) users      (100)        0 2023-12-31 08:43:17.769070 pygenda-0.3.1/pygenda/app/
+-rw-------   0 matt      (1000) users      (100)      369 2023-12-30 00:19:21.000000 pygenda-0.3.1/pygenda/app/pygenda.desktop
+drwx------   0 matt      (1000) users      (100)        0 2023-12-31 08:43:17.772070 pygenda-0.3.1/pygenda/css/
+-rw-------   0 matt      (1000) users      (100)      288 2022-01-30 22:37:16.000000 pygenda-0.3.1/pygenda/css/disc+loop+star.svg
+-rw-------   0 matt      (1000) users      (100)      215 2022-01-30 22:37:16.000000 pygenda-0.3.1/pygenda/css/disc+loop.svg
+-rw-------   0 matt      (1000) users      (100)      208 2022-01-30 22:37:16.000000 pygenda-0.3.1/pygenda/css/disc+star.svg
+-rw-------   0 matt      (1000) users      (100)      135 2022-01-30 22:37:16.000000 pygenda-0.3.1/pygenda/css/disc.svg
+-rw-------   0 matt      (1000) users      (100)     3876 2023-12-30 00:19:21.000000 pygenda-0.3.1/pygenda/css/gemini.css
+-rw-------   0 matt      (1000) users      (100)      223 2022-01-30 22:37:16.000000 pygenda-0.3.1/pygenda/css/loop+star.svg
+-rw-------   0 matt      (1000) users      (100)      150 2022-01-30 22:37:16.000000 pygenda-0.3.1/pygenda/css/loop.svg
+-rw-------   0 matt      (1000) users      (100)    16321 2023-12-30 00:19:21.000000 pygenda-0.3.1/pygenda/css/pygenda.css
+-rw-------   0 matt      (1000) users      (100)      103 2023-10-06 15:06:24.000000 pygenda-0.3.1/pygenda/css/raspberrypi.css
+-rw-------   0 matt      (1000) users      (100)      150 2022-01-30 22:37:16.000000 pygenda-0.3.1/pygenda/css/star.svg
+drwx------   0 matt      (1000) users      (100)        0 2023-12-31 08:43:17.773070 pygenda-0.3.1/pygenda/locale/
+drwx------   0 matt      (1000) users      (100)        0 2023-12-31 08:43:17.765070 pygenda-0.3.1/pygenda/locale/en_US/
+drwx------   0 matt      (1000) users      (100)        0 2023-12-31 08:43:17.773070 pygenda-0.3.1/pygenda/locale/en_US/LC_MESSAGES/
+-rw-------   0 matt      (1000) users      (100)      536 2023-12-30 00:19:21.000000 pygenda-0.3.1/pygenda/locale/en_US/LC_MESSAGES/pygenda.mo
+drwx------   0 matt      (1000) users      (100)        0 2023-12-31 08:43:17.765070 pygenda-0.3.1/pygenda/locale/fr/
+drwx------   0 matt      (1000) users      (100)        0 2023-12-31 08:43:17.773070 pygenda-0.3.1/pygenda/locale/fr/LC_MESSAGES/
+-rw-------   0 matt      (1000) users      (100)     9680 2023-12-31 08:09:04.000000 pygenda-0.3.1/pygenda/locale/fr/LC_MESSAGES/pygenda.mo
+-rw-------   0 matt      (1000) users      (100)    12440 2023-12-31 08:09:04.000000 pygenda-0.3.1/pygenda/locale/pygenda.pot
+-rw-------   0 matt      (1000) users      (100)    77874 2023-12-30 00:19:21.000000 pygenda-0.3.1/pygenda/pygenda_calendar.py
+-rw-------   0 matt      (1000) users      (100)     5805 2023-12-30 00:19:21.000000 pygenda-0.3.1/pygenda/pygenda_config.py
+-rw-------   0 matt      (1000) users      (100)    11741 2023-12-31 08:09:04.000000 pygenda-0.3.1/pygenda/pygenda_dialog_entryprops.py
+-rw-------   0 matt      (1000) users      (100)    75600 2023-12-31 08:09:04.000000 pygenda-0.3.1/pygenda/pygenda_dialog_event.py
+-rw-------   0 matt      (1000) users      (100)     3447 2023-12-31 08:09:04.000000 pygenda-0.3.1/pygenda/pygenda_dialog_find.py
+-rw-------   0 matt      (1000) users      (100)    15266 2023-12-31 08:09:04.000000 pygenda-0.3.1/pygenda/pygenda_dialog_todo.py
+-rw-------   0 matt      (1000) users      (100)     4656 2023-12-30 00:19:21.000000 pygenda-0.3.1/pygenda/pygenda_entryinfo.py
+-rw-------   0 matt      (1000) users      (100)    45678 2023-12-31 08:09:04.000000 pygenda-0.3.1/pygenda/pygenda_gui.py
+-rw-------   0 matt      (1000) users      (100)    11411 2023-12-30 00:19:21.000000 pygenda-0.3.1/pygenda/pygenda_util.py
+-rw-------   0 matt      (1000) users      (100)      300 2023-12-31 08:30:33.000000 pygenda-0.3.1/pygenda/pygenda_version.py
+-rw-------   0 matt      (1000) users      (100)    16180 2023-12-31 08:09:04.000000 pygenda-0.3.1/pygenda/pygenda_view.py
+-rw-------   0 matt      (1000) users      (100)    27370 2023-12-31 08:09:04.000000 pygenda-0.3.1/pygenda/pygenda_view_todo.py
+-rw-------   0 matt      (1000) users      (100)    22946 2023-12-31 08:09:04.000000 pygenda-0.3.1/pygenda/pygenda_view_week.py
+-rw-------   0 matt      (1000) users      (100)    28954 2023-12-31 08:09:04.000000 pygenda-0.3.1/pygenda/pygenda_view_year.py
+-rw-------   0 matt      (1000) users      (100)    22109 2023-12-30 00:19:21.000000 pygenda-0.3.1/pygenda/pygenda_widgets.py
+drwx------   0 matt      (1000) users      (100)        0 2023-12-31 08:43:17.773070 pygenda-0.3.1/pygenda/ui/
+-rw-------   0 matt      (1000) users      (100)    45184 2023-12-31 08:09:04.000000 pygenda-0.3.1/pygenda/ui/dialog_event.ui
+-rw-------   0 matt      (1000) users      (100)     5147 2023-12-31 08:09:04.000000 pygenda-0.3.1/pygenda/ui/dialog_find.ui
+-rw-------   0 matt      (1000) users      (100)    14665 2023-12-31 08:09:04.000000 pygenda-0.3.1/pygenda/ui/dialog_todo.ui
+-rw-------   0 matt      (1000) users      (100)    33315 2023-12-31 08:09:04.000000 pygenda-0.3.1/pygenda/ui/main.ui
+-rw-------   0 matt      (1000) users      (100)     3889 2023-12-31 08:09:04.000000 pygenda-0.3.1/pygenda/ui/view_week.ui
+-rw-------   0 matt      (1000) users      (100)     5928 2023-12-31 08:09:04.000000 pygenda-0.3.1/pygenda/ui/view_year.ui
+drwx------   0 matt      (1000) users      (100)        0 2023-12-31 08:43:17.769070 pygenda-0.3.1/pygenda.egg-info/
+-rw-------   0 matt      (1000) users      (100)     1015 2023-12-31 08:43:17.000000 pygenda-0.3.1/pygenda.egg-info/PKG-INFO
+-rw-------   0 matt      (1000) users      (100)     1216 2023-12-31 08:43:17.000000 pygenda-0.3.1/pygenda.egg-info/SOURCES.txt
+-rw-------   0 matt      (1000) users      (100)        1 2023-12-31 08:43:17.000000 pygenda-0.3.1/pygenda.egg-info/dependency_links.txt
+-rw-------   0 matt      (1000) users      (100)       67 2023-12-31 08:43:17.000000 pygenda-0.3.1/pygenda.egg-info/requires.txt
+-rw-------   0 matt      (1000) users      (100)        8 2023-12-31 08:43:17.000000 pygenda-0.3.1/pygenda.egg-info/top_level.txt
+-rw-------   0 matt      (1000) users      (100)       38 2023-12-31 08:43:17.774070 pygenda-0.3.1/setup.cfg
+-rwx------   0 matt      (1000) users      (100)     3892 2023-12-31 08:09:04.000000 pygenda-0.3.1/setup.py
```

### Comparing `pygenda-0.3.0/COPYING` & `pygenda-0.3.1/COPYING`

 * *Files identical despite different names*

### Comparing `pygenda-0.3.0/PKG-INFO` & `pygenda-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygenda
-Version: 0.3.0
+Version: 0.3.1
 Summary: An agenda application inspired by Agenda programs on Psion PDAs.
 Home-page: https://github.com/semiprime/pygenda
 Author: Matthew Lewis
 Author-email: pygenda@semiprime.com
 License: GPLv3 only
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pygenda-0.3.0/README.md` & `pygenda-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pygenda-0.3.0/csrc/CMakeLists.txt` & `pygenda-0.3.1/csrc/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pygenda-0.3.0/csrc/pygenda_clipboard.c` & `pygenda-0.3.1/csrc/pygenda_clipboard.c`

 * *Files identical despite different names*

### Comparing `pygenda-0.3.0/pygenda/__main__.py` & `pygenda-0.3.1/pygenda/__main__.py`

 * *Files identical despite different names*

### Comparing `pygenda-0.3.0/pygenda/css/gemini.css` & `pygenda-0.3.1/pygenda/css/gemini.css`

 * *Files identical despite different names*

### Comparing `pygenda-0.3.0/pygenda/css/pygenda.css` & `pygenda-0.3.1/pygenda/css/pygenda.css`

 * *Files identical despite different names*

### Comparing `pygenda-0.3.0/pygenda/glade/dialog_event.glade` & `pygenda-0.3.1/pygenda/ui/dialog_event.ui`

 * *Files 0% similar despite different names*

#### Comparing `pygenda-0.3.0/pygenda/glade/dialog_event.glade` & `pygenda-0.3.1/pygenda/ui/dialog_event.ui`

```diff
@@ -1,10 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!--
-	dialog_event.glade
+	dialog_event.ui
 	Copyright (C) 2022,2023 Matthew Lewis
 	Based on a file generated with glade 3.38.2
 
 	This file is part of Pygenda.
 
 	Pygenda is free software: you can redistribute it and/or modify
 	it under the terms of the GNU General Public License as published by
```

### Comparing `pygenda-0.3.0/pygenda/glade/dialog_find.glade` & `pygenda-0.3.1/pygenda/ui/dialog_find.ui`

 * *Files 1% similar despite different names*

#### Comparing `pygenda-0.3.0/pygenda/glade/dialog_find.glade` & `pygenda-0.3.1/pygenda/ui/dialog_find.ui`

```diff
@@ -1,10 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!--
-	dialog_find.glade
+	dialog_find.ui
 	Copyright (C) 2022,2023 Matthew Lewis
 	Based on a file generated with glade 3.38.2
 
 	This file is part of Pygenda.
 
 	Pygenda is free software: you can redistribute it and/or modify
 	it under the terms of the GNU General Public License as published by
```

### Comparing `pygenda-0.3.0/pygenda/glade/dialog_todo.glade` & `pygenda-0.3.1/pygenda/ui/dialog_todo.ui`

 * *Files 0% similar despite different names*

#### Comparing `pygenda-0.3.0/pygenda/glade/dialog_todo.glade` & `pygenda-0.3.1/pygenda/ui/dialog_todo.ui`

```diff
@@ -1,10 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!--
-	dialog_todo.glade
+	dialog_todo.ui
 	Copyright (C) 2022,2023 Matthew Lewis
 	Based on a file generated with glade 3.38.2
 
 	This file is part of Pygenda.
 
 	Pygenda is free software: you can redistribute it and/or modify
 	it under the terms of the GNU General Public License as published by
```

### Comparing `pygenda-0.3.0/pygenda/glade/main.glade` & `pygenda-0.3.1/pygenda/ui/main.ui`

 * *Files 1% similar despite different names*

#### Comparing `pygenda-0.3.0/pygenda/glade/main.glade` & `pygenda-0.3.1/pygenda/ui/main.ui`

```diff
@@ -1,10 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!--
-	main.glade
+	main.ui
 	Copyright (C) 2022,2023 Matthew Lewis
 	Based on a file generated with glade 3.38.2
 
 	This file is part of Pygenda.
 
 	Pygenda is free software: you can redistribute it and/or modify
 	it under the terms of the GNU General Public License as published by
@@ -541,15 +541,15 @@
                             <property name="position">0</property>
                           </packing>
                         </child>
                         <child>
                           <object class="GtkLabel">
                             <property name="visible">True</property>
                             <property name="can-focus">False</property>
-                            <property name="label" translatable="yes">New Event</property>
+                            <property name="label" translatable="yes">New Entry</property>
                             <property name="justify">center</property>
                             <property name="wrap">True</property>
                             <property name="max-width-chars">9</property>
                           </object>
                           <packing>
                             <property name="expand">False</property>
                             <property name="fill">True</property>
```

### Comparing `pygenda-0.3.0/pygenda/glade/view_week.glade` & `pygenda-0.3.1/pygenda/ui/view_week.ui`

 * *Files 0% similar despite different names*

#### Comparing `pygenda-0.3.0/pygenda/glade/view_week.glade` & `pygenda-0.3.1/pygenda/ui/view_week.ui`

```diff
@@ -1,10 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!--
-	view_week.glade
+	view_week.ui
 	Copyright (C) 2022,2023 Matthew Lewis
 	Based on a file generated with glade 3.38.2
 
 	This file is part of Pygenda.
 
 	Pygenda is free software: you can redistribute it and/or modify
 	it under the terms of the GNU General Public License as published by
```

### Comparing `pygenda-0.3.0/pygenda/glade/view_year.glade` & `pygenda-0.3.1/pygenda/ui/view_year.ui`

 * *Files 0% similar despite different names*

#### Comparing `pygenda-0.3.0/pygenda/glade/view_year.glade` & `pygenda-0.3.1/pygenda/ui/view_year.ui`

```diff
@@ -1,10 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!--
-	view_year.glade
+	view_year.ui
 	Copyright (C) 2022,2023 Matthew Lewis
 	Based on a file generated with glade 3.38.2
 
 	This file is part of Pygenda.
 
 	Pygenda is free software: you can redistribute it and/or modify
 	it under the terms of the GNU General Public License as published by
```

### Comparing `pygenda-0.3.0/pygenda/locale/en_US/LC_MESSAGES/pygenda.mo` & `pygenda-0.3.1/pygenda/locale/en_US/LC_MESSAGES/pygenda.mo`

 * *Files identical despite different names*

### Comparing `pygenda-0.3.0/pygenda/locale/fr/LC_MESSAGES/pygenda.mo` & `pygenda-0.3.1/pygenda/locale/fr/LC_MESSAGES/pygenda.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Pygenda\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2023-10-22 23:04+0200\n"
+"PO-Revision-Date: 2023-12-28 09:46+0100\n"
 "Last-Translator: Matthew Lewis <pygenda@semiprime.com>\n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
@@ -107,14 +107,17 @@
 
 msgid "Cance_lled"
 msgstr "_Annulé"
 
 msgid "Cancelled"
 msgstr "Annulé"
 
+msgid "Categories:"
+msgstr "Catégories :"
+
 msgid "Completed"
 msgstr "Achevé"
 
 msgid "Completed date (noncompliant):"
 msgstr "Date d’achèvement (non-conforme) :"
 
 msgid "Completed date/time:"
@@ -268,14 +271,17 @@
 
 msgid "Location:"
 msgstr "Lieu :"
 
 msgid "Monthly"
 msgstr "Mensuelle"
 
+msgid "New Entry"
+msgstr "Nouvelle entrée"
+
 msgid "New Event"
 msgstr "Nouvel évènement"
 
 msgid "New To-do"
 msgstr "Nouvelle tâche"
 
 msgid "New _To-do…"
@@ -367,14 +373,17 @@
 
 msgid "Todo"
 msgstr "Tâche"
 
 msgid "Type:"
 msgstr "Type :"
 
+msgid "URL:"
+msgstr "URL :"
+
 msgid "Understood"
 msgstr "Je comprends"
 
 msgid "Until:"
 msgstr "Jusqu’à :"
 
 msgid "View"
```

### Comparing `pygenda-0.3.0/pygenda/pygenda_calendar.py` & `pygenda-0.3.1/pygenda/pygenda_calendar.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 from typing import Optional, Union, Tuple, List
 from copy import deepcopy
 from math import ceil
 from calendar import monthrange
 
 # Pygenda components
 from .pygenda_config import Config
-from .pygenda_util import dt_lt, dt_lte, datetime_to_date, date_to_datetime, LOCAL_TZ
+from .pygenda_util import dt_lt, dt_lte, datetime_to_date, date_to_datetime, get_local_tz, dt_add_delta
 from .pygenda_entryinfo import EntryInfo
 
 
 # Interface base class to connect to different data sources.
 # Used by Calendar class (below).
 class CalendarConnector:
     cal = None # type:iCalendar
@@ -84,19 +84,20 @@
 
 
 # Singleton class for calendar data access/manipulation
 class Calendar:
     STATUS_LIST_EVENT = ('TENTATIVE','CONFIRMED','CANCELLED')
     STATUS_LIST_TODO = ('NEEDS-ACTION','IN-PROCESS','COMPLETED','CANCELLED')
 
-    calConnectors = [] # type:List[CalendarConnector]
+    calConnectors = None # type:List[CalendarConnector]
     _default_connector_event = None # type:int
     _default_connector_todo = None # type:int
     _entry_norep_list_sorted = None
     _entry_rep_list = None
+    _entry_norep_xover_list_sorted = None # type:Optional[list]
     _todo_list = None
 
     @classmethod
     def init(cls) -> None:
         # Calendar connector initialisation.
         # Can take a long time, since it loads/sorts calendar data.
         # Best called in background after GUI is started, or startup can be slow.
@@ -131,31 +132,44 @@
                 flags |= ETMAP[entype]
 
             # Create new connector
             conn = CTMAP[caltype](sect, flags)
             if conn.cal.is_broken:
                 print('Warning: Non-conformant ical data, '+sect, file=stderr)
 
-            # Set display name
+            # Set display name (might already be set by constructor)
             dn = Config.get(sect, 'display_name')
-            conn.displayname = sect if dn is None else dn
+            if dn is not None:
+                conn.displayname = dn
+            elif not conn.displayname: # Don't want empty display name
+                conn.displayname = sect
 
             # Add _cal_idx attribute so we can find calendar from entry
             calidx = len(cls.calConnectors)
             if conn.stores_events():
                 for ev in conn.cal.walk('VEVENT'):
                     ev._cal_idx = calidx
             if conn.stores_todos():
                 for td in conn.cal.walk('VTODO'):
                     td._cal_idx = calidx
 
             # Finally, append our new connector to the list
             cls.calConnectors.append(conn)
 
 
+        # Re-initialise connections and saved lists so init()
+        # can be called more tn once if necessary
+        cls.calConnectors = []
+        cls._default_connector_event = None # type:ignore[assignment]
+        cls._default_connector_todo = None # type:ignore[assignment]
+        cls._entry_norep_list_sorted = None
+        cls._entry_rep_list = None
+        cls._entry_norep_xover_list_sorted = None
+        cls._todo_list = None
+
         caltype = Config.get('calendar','type')
         if caltype is not None:
             do_parse('calendar', caltype)
 
         # look for 'calendar1', 'calendar2' etc.
         i = len(cls.calConnectors) # if no 'calendar' start at 'calendar0'
         while True:
@@ -271,29 +285,28 @@
             if not cls.calConnectors[e_inf.cal_idx].stores_todos():
                 raise ValueError('Tried to add todo to calendar that doesn\'t store todos')
             en = iTodo()
             cls._todo_list = None # Clear todo cache as modified
         else:
             raise ValueError('Unrecognized entry type')
         en.add('UID', Calendar.gen_uid()) # Required
-        # DateTime utcnow() function doesn't include TZ, so use now(tz.utc)
-        utcnow = dt_datetime.now(timezone.utc)
-        en.add('DTSTAMP', utcnow) # Required
-        en.add('CREATED', utcnow) # Optional
+        cls._update_timestamps(en, is_new=True)
         en.add('SUMMARY', e_inf.desc)
 
         if e_inf.start_dt is not None:
             en.add('DTSTART', e_inf.start_dt)
             cls._event_add_end_dur_from_info(en, e_inf)
             # Repeats - only add these if entry has a date(time)
             if e_inf.rep_type is not None and e_inf.rep_inter>0:
                 cls._event_add_repeat_from_info(en, e_inf)
                 cls._entry_rep_list = None # Clear rep cache as modified
             else:
                 cls._entry_norep_list_sorted = None # Clear norep cache, mod'd
+                if cls._is_xover_entry(en):
+                    cls._entry_norep_xover_list_sorted = None
 
         cls._entry_set_status_from_info(en, e_inf)
         cls._event_set_location_from_info(en, e_inf)
         if e_inf.categories:
             # Convert to list - to work around bug passing set to old icalendar
             en.add('CATEGORIES', list(e_inf.categories))
         if e_inf.priority:
@@ -338,18 +351,16 @@
         else:
             raise ValueError('Unrecognized iCal entry type')
 
         if cls.calConnectors[cal_idx].is_readonly():
             raise ValueError('Tried to add entry to calendar set as read-only')
 
         en.add('UID', Calendar.gen_uid()) # Required
-        utcnow = dt_datetime.now(timezone.utc)
-        en.add('DTSTAMP', utcnow) # Required
-        # Since it has a new UID, we consider it a new entry
-        en.add('CREATED', utcnow) # Optional
+        cls._update_timestamps(en, is_new=True)
+
         summ = exen['SUMMARY'] if 'SUMMARY' in exen else None
         if not summ:
             summ = 'New entry' # fallback summary
         en.add('SUMMARY', summ)
         new_dt_start = None
         if en_is_event:
             # Some entry elements only relevant if an event (may change later)
@@ -397,14 +408,16 @@
             en.add('DESCRIPTION', exen['DESCRIPTION'])
 
         en = cls.calConnectors[cal_idx].add_entry(en) # Write to store
         en._cal_idx = cal_idx
 
         if new_dt_start is not None:
             cls._entry_norep_list_sorted = None # Clear norep cache as modified
+            if cls._is_xover_entry(en):
+                cls._entry_norep_xover_list_sorted = None
         if not en_is_event: # is Todo
             cls._todo_list = None # Clear todo cache as modified
         return en
 
 
     @classmethod
     def update_entry(cls, en:Union[iEvent,iTodo], e_inf:EntryInfo) -> None:
@@ -427,18 +440,15 @@
 
         clear_rep = False
         clear_norep = False
 
         if 'UID' not in en:
             en.add('UID', Calendar.gen_uid()) # Should be present
 
-        # DateTime utcnow() function doesn't include TZ, so use now(tz.utc)
-        utcnow =  dt_datetime.now(timezone.utc)
-        cls._update_entry_field(en, 'DTSTAMP', utcnow)
-        cls._update_entry_field(en, 'LAST-MODIFIED', utcnow)
+        cls._update_timestamps(en, is_new=False)
         cls._update_entry_field(en, 'SUMMARY', e_inf.desc)
         cls._update_entry_field(en, 'PRIORITY', e_inf.priority)
         cls._update_entry_field(en, 'DUE', e_inf.duedate)
         cls._update_entry_field(en, 'DESCRIPTION', e_inf.longdesc)
 
         # For Categories, we need to convert to a list,
         # to work around bug passing set to old icalendar.
@@ -482,14 +492,15 @@
         for alm in alms:
             en.subcomponents.remove(alm)
         cls._entry_set_alarms_from_info(en, e_inf)
 
         # This needs optimising - some cases cause too much cache flushing !!
         if clear_norep:
             cls._entry_norep_list_sorted = None
+            cls._entry_norep_xover_list_sorted = None
         if clear_rep:
             cls._entry_rep_list = None
         if e_inf.type==EntryInfo.TYPE_TODO or isinstance(en, iTodo):
             cls._todo_list = None
 
         if en._cal_idx == e_inf.cal_idx:
             cls.calConnectors[e_inf.cal_idx].update_entry(en) # Write to store
@@ -519,14 +530,28 @@
         if fname in en:
             del(en[fname])
         if val is not None:
             en.add(fname, val)
 
 
     @staticmethod
+    def _update_timestamps(en:Union[iEvent,iTodo], is_new:bool) -> None:
+        # Update entry fields recording modified time: DTSTAMP.
+        # if is_new, add CREATED; if not new, update LAST-MODIFIED.
+        # All these fields use UTC.
+        # DateTime utcnow() function doesn't include TZ, so use now(tz.utc)
+        utcnow =  dt_datetime.now(timezone.utc)
+        Calendar._update_entry_field(en, 'DTSTAMP', utcnow) # Required elt
+        if is_new:
+            en.add('CREATED', utcnow) # Optional elt
+        else:
+            Calendar._update_entry_field(en, 'LAST-MODIFIED', utcnow) # Opt
+
+
+    @staticmethod
     def _event_add_end_dur_from_info(ev:iEvent, e_inf:EntryInfo) -> None:
         # Adds end time or duration to an event from EntryInfo.
         # How it does this depends on whether event is timed or not
 
         # If entry is timed, check for an end-time/duration & add if present
         # Note: don't add both an end-time & duration - at most one
         if isinstance(e_inf.start_dt, dt_datetime):
@@ -539,18 +564,23 @@
                     if end_dttm != e_inf.start_dt: # require end time to be after start time
                         if end_dttm < e_inf.start_dt:
                             end_dttm += timedelta(days=1)
                         ev.add('DTEND', end_dttm)
             elif e_inf.duration is not None and isinstance(e_inf.duration, timedelta):
                 if e_inf.duration.total_seconds()>0: # require duration > 0
                     ev.add('DURATION', e_inf.duration)
-        elif isinstance(e_inf.start_dt, dt_date) and isinstance(e_inf.end_dt, dt_date):
-            # start & end are both dates (not times) => this is a day entry
-            if e_inf.end_dt > e_inf.start_dt: # sanity check
-                ev.add('DTEND', e_inf.end_dt)
+        elif isinstance(e_inf.start_dt, dt_date):
+            # start is a date (not time) => this might be a day entry
+            if isinstance(e_inf.end_dt, dt_date):
+                if e_inf.end_dt >= e_inf.start_dt: # sanity check
+                    ev.add('DTEND', e_inf.end_dt)
+            elif isinstance(e_inf.duration, timedelta):
+                # RFC 5545 Sect 3.8.2.5 says duration must be whole no of days
+                if e_inf.duration.seconds == e_inf.duration.microseconds == 0:
+                    ev.add('DURATION', e_inf.duration)
 
 
     @staticmethod
     def _event_add_repeat_from_info(ev:iEvent, e_inf:EntryInfo) -> None:
         # Adds FREQ and EXDATE fields to event.
         # Assume these fields are empty (so either it's a
         # new entry or the delete happens elsewhere).
@@ -637,14 +667,16 @@
                     attee = ''
             if desc is not None:
                 v_alm.add('DESCRIPTION', desc)
             if summ is not None:
                 v_alm.add('SUMMARY', summ)
             if attee is not None:
                 v_alm.add('ATTENDEE', attee)
+            if al.attach is not None:
+                v_alm.add('ATTACH', al.attach)
             en.add_component(v_alm)
 
 
     @classmethod
     def delete_entry(cls, entry:Union[iEvent,iTodo]) -> None:
         # Delete given entry.
         if cls.calendar_readonly(entry):
@@ -652,14 +684,15 @@
 
         # Need to clear cache containing the entry...
         if 'DTSTART' in entry:
             if 'RRULE' in entry:
                 cls._entry_rep_list = None
             else:
                 cls._entry_norep_list_sorted = None
+                cls._entry_norep_xover_list_sorted = None
         if type(entry)==iTodo:
             cls._todo_list = None
 
         cls.calConnectors[entry._cal_idx].delete_entry(entry)
 
 
     @classmethod
@@ -668,32 +701,36 @@
         # If STATUS is set and equals stat, toggle it off.
         if cls.calendar_readonly(entry):
             raise ValueError('Tried to update status of entry in read-only calendar')
         if 'STATUS' in entry:
             if stat==entry['STATUS']:
                 stat = None # If on, we toggle it off
             del(entry['STATUS'])
+        elif stat is None:
+            # No existing status & requesting set to none, so do nothing
+            return
         cls._add_status_entry(entry, stat)
+        cls._update_timestamps(entry, is_new=False)
         cls.calConnectors[entry._cal_idx].update_entry(entry) # Write to store
 
 
     @staticmethod
     def _add_status_entry(entry:Union[iEvent,iTodo], stat:Optional[str]) -> None:
         # Set entry STATUS to stat.
         # Assumes entry['STATUS'] does not exist.
-        # Only allows spec'ed values.
+        # Only allows spec'ed values (o/w leaves unchanged).
         if stat=='COMPLETED':
             # PERCENT-COMPLETE automatically set to 100, so can delete
             Calendar._del_entry_field(entry, 'PERCENT-COMPLETE')
         else:
             if 'PERCENT-COMPLETE' in entry and entry['PERCENT-COMPLETE']==100:
                 entry['PERCENT-COMPLETE'] = 99 # Stop it being == 100
             Calendar._del_entry_field(entry, 'COMPLETED')
-        if (isinstance(entry,iEvent) and stat in Calendar.STATUS_LIST_EVENT) or (
-            isinstance(entry,iTodo) and stat in Calendar.STATUS_LIST_TODO):
+        if (isinstance(entry,iEvent) and stat in Calendar.STATUS_LIST_EVENT) \
+           or (isinstance(entry,iTodo) and stat in Calendar.STATUS_LIST_TODO):
                 entry.add('STATUS', stat)
 
 
     @classmethod
     def _update_entry_norep_list(cls) -> None:
         # Re-build _entry_norep_list_sorted, if it has been cleared (==None)
         if cls._entry_norep_list_sorted is None:
@@ -716,14 +753,48 @@
             for conn in cls.calConnectors:
                 if conn.stores_events():
                     evs = conn.cal.walk('VEVENT')
                     cls._entry_rep_list.extend([e for e in evs if 'RRULE' in e and e['RRULE'] is not None])
 
 
     @classmethod
+    def _update_entry_norep_xover_list_sorted(cls) -> None:
+        # Re-build _entry_norep_xover_list_sorted, if it is cleared (==None)
+        if cls._entry_norep_xover_list_sorted is None:
+            cls._entry_norep_xover_list_sorted = []
+            for conn in cls.calConnectors:
+                evs = conn.cal.walk('vEvent')
+                cls._entry_norep_xover_list_sorted.extend([e for e in evs if 'RRULE' not in e and cls._is_xover_entry(e)])
+            cls._entry_norep_xover_list_sorted.sort()
+
+
+    @staticmethod
+    def _is_xover_entry(e:iEvent) -> bool:
+        # Helper function to determine if simple/non-repeating entry
+        # crosses over from one (localtime) day to the next
+        if 'DTEND' in e:
+            st = e['DTSTART'].dt
+            end = e['DTEND'].dt
+            if isinstance(st, dt_datetime):
+                st = date_to_datetime(st, True).astimezone(get_local_tz())
+                end = date_to_datetime(end, True).astimezone(get_local_tz())
+        elif 'DURATION' in e:
+            st = e['DTSTART'].dt
+            if isinstance(st, dt_datetime):
+                st = date_to_datetime(st, True).astimezone(get_local_tz())
+            end = dt_add_delta(st, e['DURATION'].dt)
+        else:
+            return False
+        enddate = datetime_to_date(end)
+        if not isinstance(end,dt_datetime) or end.time()==dt_time(hour=0,minute=0,second=0):
+            enddate -= timedelta(days=1)
+        return datetime_to_date(st) < enddate # type:ignore[no-any-return]
+
+
+    @classmethod
     def occurrence_list(cls, start:dt_date, stop:dt_date, include_single:bool=True, include_repeated:bool=True) -> list:
         # Return list of occurences in range start <= . < stop.
         # Designed to be called by View classes to get events in range.
         # An "occurrence" is a pair: (event,datetime)
         #  for repeating entries, datetime may not be the DTSTART entry
         # Needs to also return events that last/end over range??
         ret_list = []
@@ -751,14 +822,34 @@
             cls._update_entry_rep_list()
             for e in cls._entry_rep_list:
                 merge_repeating_entries_sort(ret_list,e,start,stop)
         return ret_list
 
 
     @classmethod
+    def ongoing_list(cls, dt:dt_date, include_single:bool=True, include_repeated:bool=True) -> list:
+        # Return list of events that are ongoing at datetime 'dt'
+        ret_list = []
+        if include_single:
+            # Naive implementation - scope for optimisation here!!
+            cls._update_entry_norep_xover_list_sorted()
+            for e in cls._entry_norep_xover_list_sorted:#type:ignore[union-attr]
+                e_st = e['DTSTART'].dt
+                if dt_lte(dt, e_st):
+                    break # List is sorted, so we can stop search here
+                if 'DTEND' in e:
+                    e_end = e['DTEND'].dt
+                else: # 'DURATION' in e
+                    e_end = dt_add_delta(e_st, e['DURATION'].dt)
+                if dt_lt(dt, e_end):
+                    ret_list.append((e,e_st))
+        return ret_list
+
+
+    @classmethod
     def _update_todo_list(cls) -> None:
         # Re-build _todo_list, if it has been cleared (==None)
         if cls._todo_list is None:
             # Get events with no repeat rule & sort
             cls._todo_list = []
             for conn in cls.calConnectors:
                 if conn.stores_todos():
@@ -1048,14 +1139,16 @@
         if not EDataServer.SourceRegistry.check_enabled(registry, src):
             raise ValueError('EDS calendar uid "{:s}" not enabled'.format(uid))
 
         self.__eds_client = ECal.Client().connect_sync(source=src, source_type=src_type, wait_for_connected_seconds=self.CONNECTION_TIMEOUT) # type:ignore[name-defined]
         if self.__eds_client is None:
             raise ValueError('Error connecting to EDS calendar uid "{:s}"'.format(uid))
 
+        # Read source properties to set some connector properties
+        self.displayname = src.get_display_name()
         if not src.get_writable():
             self.flags |= CalendarConnector.READONLY
 
         suc,comps = self.__eds_client.get_object_list_sync('#t')# Search #t=True
         if not suc:
             raise ValueError('Failed getting components from EDS calendar')
 
@@ -1511,15 +1604,15 @@
             raise StopIteration
         r = self.dt
         while True:
             self.dt += self.rinfo.delta
             if not self.rinfo.is_exdate(self.dt):
                 break
         if self.rinfo.subday_rpt:
-            r = r.astimezone(LOCAL_TZ)
+            r = r.astimezone(get_local_tz())
         return r
 
 
 class RepeatIter_multidelta(RepeatIter_simpledelta):
     # Iterator class for RepeatInfo where we have different deltas
     # (e.g. we may have different gaps between occurences, such as
     # a weekly repeat that occurs on Mondays and Wednesdays).
@@ -1537,15 +1630,15 @@
         r = self.dt
         while True:
             self.dt += self.rinfo.delta[self.i]
             self.i = (self.i+1)%len(self.rinfo.delta)
             if not self.rinfo.is_exdate(self.dt):
                 break
         if self.rinfo.subday_rpt:
-            r = r.astimezone(LOCAL_TZ)
+            r = r.astimezone(get_local_tz())
         return r
 
 
 class RepeatIter_byweekdayinmonth(RepeatIter_simpledelta):
     # Iterator class for RepeatInfo where the repeat is by weekday in month.
     # E.g. first Saturday of every month; or last Friday in October.
 
@@ -1563,15 +1656,15 @@
         ret = self.dt_toret
         while True:
             self.dt_ref += self.rinfo.delta
             self.dt_toret = self.rinfo.firstday_to_byweekdayinmonth(self.dt_ref)
             if not self.rinfo.is_exdate(self.dt_toret):
                 break
         if self.rinfo.subday_rpt:
-            ret = ret.astimezone(LOCAL_TZ)
+            ret = ret.astimezone(get_local_tz())
         return ret
 
 
 def merge_repeating_entries_sort(target:list, ev:iEvent, start:dt_date, stop:dt_date) -> None:
     # Given a sorted list of occurrences, 'target', and a single
     # repeating event 'ev', splice the repeats of ev from 'start'
     # to 'stop' into 'target', keeping it sorted.
@@ -1651,15 +1744,15 @@
     sp = date_to_datetime(stop, is_timed)
     sp -= timedelta(milliseconds=1)
     ret = rr.between(after=st,before=sp,inc=True)
     if not is_timed:
         ret = [d.date() for d in ret]
     elif is_hr_min_sec:
         # After doing calculations in UTC, convert results to local time
-        ret = [d.astimezone(LOCAL_TZ) for d in ret]
+        ret = [d.astimezone(get_local_tz()) for d in ret]
     if has_exd:
         exdate_list = Calendar.caldatetime_tree_to_dt_list(ev['EXDATE'])
         for exdt in exdate_list:
             if is_timed:
                 if isinstance(exdt, dt_datetime):
                     exdt = date_to_datetime(exdt, True)
                     ret = [d for d in ret if d!=exdt]
```

### Comparing `pygenda-0.3.0/pygenda/pygenda_config.py` & `pygenda-0.3.1/pygenda/pygenda_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
                 cls._cparser.set(sect,key,value_list[key])
 
 
     @staticmethod
     def _read_arguments() -> argparse.Namespace:
         # Helper function to parse & return command-line arguments.
         parser = argparse.ArgumentParser(description=__doc__)
-        parser.add_argument('-c', '--config', metavar='FILE', type=str, default=None, help='Config file. Default: {:s}'.format(Config.DEFAULT_CONFIG_FILE))
+        parser.add_argument('-c', '--config', metavar='FILE', type=str, default=None, help='Config file. Default: {:s}, {:s}'.format(Config.DEFAULT_CONFIG_FILE,Config.DEFAULT_CONFIG_FILE_USER))
         parser.add_argument('-d', '--date', metavar='DATE', type=str, default=None, help='Cursor startup date (YYYY-MM-DD)')
         parser.add_argument('-f', '--file', metavar='FILE', type=str, default=None, help='Calendar file. Default: {:s} in config directory'.format(Config.DEFAULT_ICAL_FILENAME))
         parser.add_argument('-v', '--view', metavar='VIEW', type=str, default=None, help='Opening view')
         return parser.parse_args()
 
 
     @classmethod
```

### Comparing `pygenda-0.3.0/pygenda/pygenda_dialog_entryprops.py` & `pygenda-0.3.1/pygenda/pygenda_dialog_entryprops.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,16 +16,14 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
 # General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Pygenda. If not, see <https://www.gnu.org/licenses/>.
 
 
-from gi import require_version as gi_require_version
-gi_require_version('Gtk', '3.0')
 from gi.repository import Gtk
 from gi.repository.Pango import WrapMode as PWrapMode
 
 from datetime import datetime as dt_datetime, timedelta
 from icalendar import Event as iEvent, Todo as iTodo, vDDDTypes
 from locale import gettext as _
 from typing import Union
@@ -79,33 +77,42 @@
         self._add_datetime_rows()
         self._add_rrule_row()
         self._add_property_row('PRIORITY')
         self._add_status_row()
         self._add_property_row('LOCATION')
         self._add_alarm_rows()
         self._add_description_rows()
+        self._add_url_row()
+        self._add_categories_row()
 
 
-    def _add_row(self, label:str, cont:str, wrap:bool=False) -> None:
-        # Add text to bottom of grid in the form "label cont"
+    def _add_row(self, label:str, cont:Union[str,Gtk.Widget], wrap:bool=False) -> None:
+        # Add text to bottom of grid in the form "label cont".
+        # If `cont` is a Widget, add it to grid; if a str convert to label.
         propnm_lab = Gtk.Label(label)
         propnm_lab.set_halign(Gtk.Align.END)
         propnm_lab.set_yalign(0)
         propnm_lab.get_style_context().add_class(GUI.STYLE_TXTLABEL)
-        cont_lab = Gtk.Label(cont)
-        cont_lab.set_halign(Gtk.Align.START)
-        cont_lab.set_yalign(0)
-        cont_lab.set_xalign(0)
-        cont_lab.get_style_context().add_class(GUI.STYLE_TXTPROP)
-        if wrap:
-            cont_lab.set_line_wrap(True)
-            cont_lab.set_line_wrap_mode(PWrapMode.WORD_CHAR)
-            cont_lab.set_max_width_chars(50) # otherwise it fills screen
         self.grid.attach(propnm_lab, 0,self.grid_y, 1,1)
-        self.grid.attach(cont_lab, 1,self.grid_y, 1,1)
+
+        if isinstance(cont, Gtk.Widget):
+            # Assume caller has set any styling etc.
+            self.grid.attach(cont, 1,self.grid_y, 1,1)
+        else:
+            cont_lab = Gtk.Label(cont)
+            cont_lab.set_halign(Gtk.Align.START)
+            cont_lab.set_yalign(0)
+            cont_lab.set_xalign(0)
+            cont_lab.get_style_context().add_class(GUI.STYLE_TXTPROP)
+            if wrap:
+                cont_lab.set_line_wrap(True)
+                cont_lab.set_line_wrap_mode(PWrapMode.WORD_CHAR)
+                cont_lab.set_max_width_chars(50) # otherwise it fills screen
+            self.grid.attach(cont_lab, 1,self.grid_y, 1,1)
+
         self.grid_y += 1
 
 
     def _add_property_row(self, propnm:str) -> None:
         # Add simple property in a single row to bottom of grid
         if propnm in self.entry:
             self._add_row(_(propnm.capitalize()+':'), self.entry[propnm])
@@ -233,14 +240,17 @@
                                     a_info += attee
                                 a_info += ')'
                         if act in ('Display','Email'):
                             if 'DESCRIPTION' in a:
                                 # Spec says only one description
                                 a_info += '\n'
                                 a_info += _(u'“{:s}”').format(a['DESCRIPTION'])
+                        if act=='Audio' and 'ATTACH' in a:
+                            a_info += '\n'
+                            a_info += a['ATTACH']
                 else:
                     # No Trigger (so breaks specs)
                     a_info += 'Unspecified'
             self._add_row(_('Alarms:'), a_info)
 
 
     def _add_description_rows(self) -> None:
@@ -257,14 +267,39 @@
                     else:
                         self._add_row(_('Description:'), d, wrap=True)
             else:
                 # !! Not sure how to access LANGUAGE parameter for single desc
                 self._add_row(_('Description:'), edesc, wrap=True)
 
 
+    def _add_url_row(self) -> None:
+        # Add URL property to bottom of grid.
+        # Use a Gtk.LinkButton so the URL is clickable.
+        # Maybe security implications here if people import entries.
+        if 'URL' in self.entry:
+            url = self.entry['URL']
+            link = Gtk.LinkButton.new(url)
+            link.set_halign(Gtk.Align.START)
+            link.get_style_context().add_class(GUI.STYLE_TXTPROP)
+            self._add_row(_('URL:'), link)
+
+
+    def _add_categories_row(self) -> None:
+        # Add categories property to bottom of grid.
+        if 'CATEGORIES' in self.entry:
+            catgs = self.entry['CATEGORIES']
+            # If entry has multiple CATEGORIES lines, catgs will be a list
+            if isinstance(catgs, list):
+                ctmp = [ ', '.join(c.cats) for c in catgs ]
+            else:
+                ctmp = catgs.cats
+            cstr = ', '.join(ctmp)
+            self._add_row(_('Categories:'), cstr)
+
+
     def run(self) -> Gtk.ResponseType:
         # run the dialog
         self._write_dialog_content()
         self.dialog.show_all()
         return self.dialog.run()
```

### Comparing `pygenda-0.3.0/pygenda/pygenda_dialog_event.py` & `pygenda-0.3.1/pygenda/pygenda_dialog_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,16 +16,14 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
 # General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Pygenda. If not, see <https://www.gnu.org/licenses/>.
 
 
-from gi import require_version as gi_require_version
-gi_require_version('Gtk', '3.0')
 from gi.repository import Gtk, Gdk
 
 from datetime import date as dt_date, time as dt_time, datetime as dt_datetime, timedelta
 from dateutil import rrule as du_rrule
 from dateutil.relativedelta import relativedelta
 from icalendar import Event as iEvent, vRecur
 from sys import stderr
@@ -121,23 +119,24 @@
     buf_notes_scroller = None # type: Gtk.ScrolledWindow
 
     # Set defaults for config
     Config.set_defaults('new_event',{
         'show_alarm_warning': True,
         'timed_default_alarm_before': '15m',
         'default_alarm_emailaddr': None,
+        'default_alarm_audiofile': None,
         })
 
     @classmethod
     def init(cls) -> None:
         # Initialiser for singleton class.
         # Called from GUI init_stage2().
 
-        # Load glade file
-        GUI.load_glade_file('dialog_event.glade')
+        # Load UI file
+        GUI.load_ui_file('dialog_event.ui')
 
         # Connect signal handlers
         HANDLERS = {
             'timed_toggled': cls._do_timed_toggle,
             'allday_toggled': cls._do_allday_toggle,
             'reptype_changed': cls._reptype_changed,
             'repforever_toggled': cls._do_repeatforever_toggle,
@@ -148,15 +147,15 @@
             'alarmlist_keypress': cls._alarmlist_keypress,
             'notes_focusin': cls._notes_focus,
             'notes_focusout': cls._notes_focusloss,
             'notes_keypress': cls._notes_keypress,
             }
         GUI._builder.connect_signals(HANDLERS)
 
-        # Get some references to dialog elements in glade
+        # Get some references to dialog elements from UI file
         cls.dialog = GUI._builder.get_object('dialog_event')
         if (not cls.dialog): # Sanity check
             raise NameError('Dialog Event not found')
 
         cls.wid_desc = GUI._builder.get_object('entry_dialogevent_desc')
         cls._wid_desc_changed_handler = cls.wid_desc.connect('changed', cls._desc_changed)
         wid_grid = GUI._builder.get_object('dialogevent_grid')
@@ -292,15 +291,15 @@
         # radio buttons. This sets up a custom handler.
         for i in range(3):
             cls.wid_timed_buttons[i].connect('key-press-event', cls._radiobutton_keypress)
 
 
     @classmethod
     def _revealers_from_ids(cls, *idlist) -> list:
-        # Given a list of id strings, in glade file, make a list of revealers
+        # Given a list of id strings from UI file, make a list of revealers
         revs = []
         for id in idlist:
             obj = GUI._builder.get_object(id)
             if obj is not None:
                 revs.append(obj)
                 # Reduce transition time, o/w devices like Gemini feel sluggish.
                 # Tried to do this with CSS, so could be set per device,
@@ -397,15 +396,15 @@
 
     @classmethod
     def _do_alarmset_toggle(cls, wid:Gtk.Widget, state:bool) -> bool:
         # Callback. Called when alarm set state is changed.
         # Reveals/hides alarm list.
         if state and len(cls.alarmlist_model)==0:
             # User just enabled alarms, so if no alarms, create default ones
-            cls._add_alarm(AlarmInfo(-cls._default_alarm_before,action='AUDIO'))
+            cls._add_alarm(AlarmInfo(-cls._default_alarm_before,action='AUDIO',attach=Config.get('new_event','default_alarm_audiofile')))
             cls._add_alarm(AlarmInfo(-cls._default_alarm_before,action='DISPLAY',desc=cls.wid_desc.get_text()))
         cls._revealer_alarmlist.set_reveal_child(state)
         return False # must propagate event for active CSS selector to apply
 
 
     @classmethod
     def _add_alarm(cls, a_info:AlarmInfo) -> None:
@@ -415,15 +414,18 @@
 
 
     @classmethod
     def _set_alarm_row(cls, itr:Gtk.TreeIter, a_info:AlarmInfo) -> None:
         # Sets alarm in alarm list for row given by itr
         act = a_info.action.capitalize()
         desc = _(act)
-        if act=='Email':
+        if act=='Audio':
+            if a_info.attach is not None: # sound file
+                desc += ' (' + a_info.attach.split('/')[-1] + ')'
+        elif act=='Email':
             desc += ' (' + a_info.attendee + ')'
         elif act=='Display' and a_info.desc is not None:
             desc += ' '
             desc += _(u'“{:s}”').format(a_info.desc)
         cls.alarmlist_model.set(itr, 0,a_info, 1,str(-a_info.tdelta), 2,desc)
 
 
@@ -1208,17 +1210,18 @@
         for valarm in valarms:
             if 'TRIGGER' in valarm and 'ACTION' in valarm:
                 pretime = valarm['TRIGGER'].dt
                 act = str(valarm['ACTION'])
                 desc = valarm['DESCRIPTION'] if 'DESCRIPTION' in valarm else None
                 summ = valarm['SUMMARY'] if 'SUMMARY' in valarm else None
                 attee = valarm['ATTENDEE'] if 'ATTENDEE' in valarm else None
+                attach = valarm['ATTACH'] if 'ATTACH' in valarm else None
                 if isinstance(attee, list):
                     raise EventPropertyBeyondEditDialog('Can\'t edit alarm with >1 email addresses')
-                a_info = AlarmInfo(pretime, action=act, desc=desc, summary=summ, attendee=attee)
+                a_info = AlarmInfo(pretime, action=act, desc=desc, summary=summ, attendee=attee, attach=attach)
                 cls._add_alarm(a_info)
         if len(cls.alarmlist_model):
             cls.wid_alarmset.set_active(True)
 
 
     @classmethod
     def _fields_are_defaults(cls) -> bool:
@@ -1545,16 +1548,18 @@
             # Change selected alarm to Audio/Display/Email
             store,row = wid.get_selection().get_selected()
             if store and row:
                 a_info = cls.alarmlist_model.get_value(row,0)
                 a_info.desc = None
                 a_info.summary = None
                 a_info.attendee = None
+                a_info.attach = None
                 if ev.keyval==Gdk.KEY_a:
                     a_info.action = 'AUDIO'
+                    a_info.attach = Config.get('new_event','default_alarm_audiofile')
                 elif ev.keyval==Gdk.KEY_d:
                     a_info.action = 'DISPLAY'
                     a_info.desc = cls.wid_desc.get_text()
                 elif ev.keyval==Gdk.KEY_e:
                     a_info.action = 'EMAIL'
                     a_info.attendee = Config.get('new_event','default_alarm_emailaddr')
                     a_info.summary = cls.wid_desc.get_text() # email subject
@@ -1566,15 +1571,16 @@
                         # If no default address, for now can't set email alarms
                         print('Error: No email address available', file=stderr)
                         return True
                 cls._set_alarm_row(row, a_info)
             return True # Don't propagate event
         elif ev.keyval==Gdk.KEY_n:
             # Add new alarm to list, Audio since it's the most basic type
-            cls._add_alarm(AlarmInfo(-cls._default_alarm_before,action='AUDIO'))
+            al = AlarmInfo(-cls._default_alarm_before, action='AUDIO', attach=Config.get('new_event','default_alarm_audiofile'))
+            cls._add_alarm(al)
             wid.set_cursor(len(cls.alarmlist_model)-1) # Move cursor to new row
             return True # Don't propagate event
         elif ev.keyval==Gdk.KEY_Return:
             # Manually trigger default event on dialog box
             cls.dialog.response(Gtk.ResponseType.OK)
             return True # Don't propagate event
```

### Comparing `pygenda-0.3.0/pygenda/pygenda_dialog_find.py` & `pygenda-0.3.1/pygenda/pygenda_dialog_find.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,16 +16,14 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
 # General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Pygenda. If not, see <https://www.gnu.org/licenses/>.
 
 
-from gi import require_version as gi_require_version
-gi_require_version('Gtk', '3.0')
 from gi.repository import Gtk
 
 from icalendar import Todo as iTodo
 from locale import gettext as _
 
 # pygenda components
 from .pygenda_gui import GUI
@@ -38,18 +36,18 @@
     find_text = None # type: Gtk.Entry
 
     @classmethod
     def init(cls) -> None:
         # Initialiser for FindController singleton class.
         # Called from GUI init_stage2().
 
-        # Load glade file
-        GUI.load_glade_file('dialog_find.glade')
+        # Load UI file
+        GUI.load_ui_file('dialog_find.ui')
 
-        # Get some references to dialog elements in glade
+        # Get some references to dialog elements from UI file
         cls.dialog = GUI._builder.get_object('dialog_find')
         cls.find_text = GUI._builder.get_object('dialog_find_text')
         if (not cls.dialog or not cls.find_text): # Sanity check
             raise NameError('Dialog Find not found')
 
     @classmethod
     def find(cls) -> None:
```

### Comparing `pygenda-0.3.0/pygenda/pygenda_dialog_todo.py` & `pygenda-0.3.1/pygenda/pygenda_dialog_todo.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,14 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
 # General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Pygenda. If not, see <https://www.gnu.org/licenses/>.
 
 
-from gi import require_version as gi_require_version
-gi_require_version('Gtk', '3.0')
 from gi.repository import Gtk, Gdk
 
 from icalendar import Todo as iTodo
 from locale import gettext as _
 from datetime import datetime as dt_datetime
 from typing import Optional, Tuple
 
@@ -65,26 +63,26 @@
     list_default_cats = None # type: list
 
     @classmethod
     def init(cls) -> None:
         # Initialiser for TodoDialogController singleton class.
         # Called from GUI init_stage2().
 
-        # Load glade file
-        GUI.load_glade_file('dialog_todo.glade')
+        # Load UI file
+        GUI.load_ui_file('dialog_todo.ui')
 
         # Connect signal handlers
         HANDLERS = {
             'notes_focusin': cls._notes_focus,
             'notes_focusout': cls._notes_focusloss,
             'notes_keypress': cls._notes_keypress,
             }
         GUI._builder.connect_signals(HANDLERS)
 
-        # Get some references to dialog elements in glade
+        # Get some references to dialog elements from UI file
         cls.dialog = GUI._builder.get_object('dialog_todo')
         if (not cls.dialog): # Sanity check
             raise NameError('Dialog Todo not found')
 
         cls.wid_desc = GUI._builder.get_object('entry_dialogtodo_desc')
         cls.wid_desc.connect('changed', cls._validated_field_changed)
         cls._init_todolists()
@@ -267,15 +265,15 @@
                 cls.wid_priority.set_active(p)
         if 'DUE' in todo:
             due = todo['DUE'].dt
             if isinstance(due,dt_datetime):
                 raise TodoPropertyBeyondEditDialog('Editing todo with date+time DUE not supported')
             cls.wid_duedate_switch.set_active(True)
             cls.wid_duedate.set_date(due)
-        if 'DTSTART' in todo or 'DTEND' in todo or 'COMPETED' in todo:
+        if 'DTSTART' in todo or 'DTEND' in todo or 'COMPLETED' in todo:
             raise TodoPropertyBeyondEditDialog('Editing todo with unsupported date property')
         if 'STATUS' in todo:
             s = todo['STATUS']
             if s in Calendar.STATUS_LIST_TODO:
                 cls.wid_status.set_active_id(s)
         if 'DESCRIPTION' in todo:
             cls.buf_notes.set_text(todo['DESCRIPTION'])
```

### Comparing `pygenda-0.3.0/pygenda/pygenda_entryinfo.py` & `pygenda-0.3.1/pygenda/pygenda_entryinfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,13 +118,14 @@
 
     def set_longdesc(self, ldesc:Optional[str]) -> None:
         # Set long description for this entry
         self.longdesc = ldesc
 
 
 class AlarmInfo:
-    def __init__(self, tdelta:timedelta, action:str, desc:str=None, summary:str=None, attendee:str=None):
+    def __init__(self, tdelta:timedelta, action:str, desc:str=None, summary:str=None, attendee:str=None, attach:str=None):
         self.tdelta = tdelta # Note: -ve -> before entry; +ve -> after entry
         self.action = action
         self.desc = desc
         self.summary = summary
         self.attendee = attendee
+        self.attach = attach
```

### Comparing `pygenda-0.3.0/pygenda/pygenda_gui.py` & `pygenda-0.3.1/pygenda/pygenda_gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,16 +137,16 @@
     def init(cls) -> None:
         # First stage initialisation to bring up the UI.
         # See init_stage2() below for init done after gtk_main loop started.
 
         # First set the locale, so UI language (e.g. in menu) is correct
         cls._init_locale()
 
-        # Construct GUI from GTK Builder XML glade file
-        cls.load_glade_file('main.glade')
+        # Construct GUI from GTK Builder XML UI file
+        cls.load_ui_file('main.ui')
 
         cls._window = cls._builder.get_object('window_main')
         if (not cls._window): # Sanity check
             raise NameError('Main window not found')
         cls._window.set_default_icon_name('x-office-calendar')
 
         cls._window.set_hide_titlebar_when_maximized(Config.get_bool('global','hide_titlebar_when_maximized'))
@@ -194,15 +194,15 @@
             'menuitem_switchview': cls.switch_view,
             'menuitem_zoomin': lambda a: cls.zoom(+1),
             'menuitem_zoomout': lambda a: cls.zoom(-1),
             'menuitem_fullscreen': cls.toggle_fullscreen,
             'menuitem_goto': cls.dialog_goto,
             'menuitem_find': cls.handler_find,
             'menuitem_about': cls.dialog_about,
-            'button0_clicked': cls.handler_newevent,
+            'button0_clicked': cls.handler_newentry,
             'button1_clicked': cls.switch_view,
             'button2_clicked': cls.dialog_goto,
             'button3_clicked': cls.zoom_button,
             }
         cls._builder.connect_signals(HANDLERS)
 
         cls._box_view_cont = cls._builder.get_object('box_view_cont')
@@ -250,20 +250,20 @@
     @classmethod
     def _get_objs_by_id(cls, id_list:Tuple[str,...]) -> Tuple[Gtk.Widget,...]:
         # Helper function to get a tuple of widgets by id
         return tuple((cls._builder.get_object(id) for id in id_list))
 
 
     @classmethod
-    def load_glade_file(cls, gfile:str) -> None:
-        # Load GUI elements from GTK Builder XML glade file in glade directory
-        fullname = ospath.dirname(__file__) + '/glade/' + gfile
+    def load_ui_file(cls, gfile:str) -> None:
+        # Load GUI elements from GTK Builder XML UI file in ui directory
+        fullname = ospath.dirname(__file__) + '/ui/' + gfile
         r = cls._builder.add_from_file(fullname)
         if not r:
-            print('Error loading glade file '+gfile, file=stderr)
+            print('Error loading UI file '+gfile, file=stderr)
             Gtk.main_quit()
 
 
     @staticmethod
     def init_cal(task:Gio.Task, src_obj, t_data, cancel:Gio.Cancellable)->None:
         # Wrapper around Calendar.init(), so we can call it in a GTask thread.
         try:
@@ -375,15 +375,15 @@
         cls._init_dialogs()
 
         # Add functionality to spinbuttons not provided by GTK
         cls._init_spinbuttons()
         cls._init_comboboxes()
         cls._init_entryboxes()
 
-        # Menu bar & softkey bar made insensitive in .glade for startup.
+        # Menu bar & softkey bar made insensitive in .ui for startup.
         # We make them sensitive here before activating view.
         cls._builder.get_object('menu_bar').set_sensitive(True)
         cls._builder.get_object('box_buttons').set_sensitive(True)
 
         cls.view_redraw(True) # Draw active view, including entries
         cls._eventbox.show_all()
 
@@ -743,27 +743,35 @@
     def exit(cls, *args) -> bool:
         # Callback for various types of exit signal (command line, menus...)
         Gtk.main_quit()
         return True # don't propagate event
 
     @classmethod
     def handler_newevent(cls, *args) -> bool:
-        # Callback for "Create new event" signal (menu, softkey)
+        # Callback for "Create new event" signal (menu)
         date = cls.views[cls._view_idx].cursor_date()
         EventDialogController.new_event(date=date)
         return True # don't propagate event
 
     @classmethod
     def handler_newtodo(cls, *args) -> bool:
         # Callback for "Create new todo" signal (menu)
         lst = cls.views[cls._view_idx].cursor_todo_list()
         TodoDialogController.new_todo(list_idx=lst)
         return True # don't propagate event
 
     @classmethod
+    def handler_newentry(cls, *args) -> bool:
+        # Callback for "Create new entry" signal (softkey)
+        # Create new event or new todo, depending on the View.
+        if cls.views[cls._view_idx].default_entry_is_todo():
+            return cls.handler_newtodo(cls, *args)
+        return cls.handler_newevent(cls, *args)
+
+    @classmethod
     def handler_find(cls, *args) -> bool:
         # Callback for find signal (menu)
         FindDialogController.find()
         return True # don't propagate event
 
     @classmethod
     def handler_showentryprops(cls, *args) -> bool:
```

### Comparing `pygenda-0.3.0/pygenda/pygenda_util.py` & `pygenda-0.3.1/pygenda/pygenda_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,19 +18,19 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with Pygenda. If not, see <https://www.gnu.org/licenses/>.
 
 
 from calendar import day_abbr,month_abbr
 from icalendar import cal as iCal
-from datetime import date, time, datetime, timedelta, tzinfo
+from datetime import date, time, datetime, timedelta, tzinfo, timezone
 from dateutil import tz as du_tz
 from tzlocal import get_localzone
 import locale
-from typing import Tuple
+from typing import Tuple, Any, Union
 
 from .pygenda_config import Config
 
 
 def datetime_to_date(dt:date) -> date:
     # Extract date from datetime object (which might be a date)
     try:
@@ -44,31 +44,41 @@
     # Return False if no time component.
     try:
         return dt.time()
     except AttributeError:
         return False
 
 
-# For many repeat types, we need to have a timezone that is "aware" of
+# For some calculations, we need to have a timezone that is "aware" of
 # summer time changes to make correct, e.g. hourly, calculations
-LOCAL_TZ = get_localzone()
-if not hasattr(LOCAL_TZ,'unwrap_shim') and hasattr(LOCAL_TZ,'zone'):
+_local_tz = get_localzone()
+if not hasattr(_local_tz,'unwrap_shim') and hasattr(_local_tz,'zone'):
     # Old tzlocal API, so need to create tzinfo object
-    LOCAL_TZ = du_tz.gettz(LOCAL_TZ.zone)
+    _local_tz = du_tz.gettz(_local_tz.zone)
 # Alternative for Linuxes:
-#LOCAL_TZ = du_tz.tzfile('/etc/localtime')
+#_local_tz = du_tz.tzfile('/etc/localtime')
 
+def get_local_tz() -> Any:
+    # Getter. Can be assumed to return a zoneinfo object.
+    return _local_tz
 
-def date_to_datetime(dt:date, tz:tzinfo=None) -> datetime:
+def _set_local_tz(zinfo:Any) -> None:
+    # Setter for test code - so we can run tests in different time zones.
+    # Users should set time from the system, not an agenda app!
+    global _local_tz
+    _local_tz = zinfo
+
+
+def date_to_datetime(dt:date, tz:Union[tzinfo,bool]=None) -> datetime:
     # Return datetime from dt argument. Set time to midnight if no time.
     # If tz parameter is not None/False, and dt has no timezone, add tz (True -> add local timezone)
     # Hence this function can be used to guarantee we have datetime with a timezone
     dt_ret= dt if isinstance(dt,datetime) else datetime(dt.year,dt.month,dt.day)
     if tz and dt_ret.tzinfo is None:
-        dt_ret = dt_ret.replace(tzinfo=LOCAL_TZ if tz is True else tz)
+        dt_ret = dt_ret.replace(tzinfo=_local_tz if tz is True else tz)
     return dt_ret
 
 
 def start_end_dts_event(event:iCal.Event) -> Tuple[date,date]:
     # Return start & end time of an event.
     # End time calculated from duration if needed; is None if no end/duration.
     start = event['DTSTART'].dt
@@ -157,15 +167,15 @@
     # Return the day number of dt in the week
     # Depends on config setting global/start_week_day
     day = dt.weekday()
     start_day = Config.get_int('global', 'start_week_day')
     return (day-start_day)%7
 
 
-def start_of_week(dt:date) -> int:
+def start_of_week(dt:date) -> date:
     # Return first day of week containing dt
     # Depends on config setting global/start_week_day
     return dt - timedelta(days=day_in_week(dt))
 
 
 def dt_lte(dt_a:date, dt_b:date) -> bool:
     # Return True if dt_a <= dt_b
@@ -195,14 +205,30 @@
     return dt_lt(self['DTSTART'].dt,other['DTSTART'].dt)
 
 # Attach method to classes so it can be used to sort
 iCal.Event.__lt__ = _entry_lt
 iCal.Todo.__lt__ = _entry_lt
 
 
+def dt_add_delta(dt:date, delta:timedelta) -> datetime:
+    # Return dt+delta, taking into account things like daylight savings
+    # changeover etc.
+    r = date_to_datetime(dt, True)
+    if delta.days:
+        # Add days with timezone - at DST crossover days can have 23/25 hours
+        r += timedelta(days=delta.days)
+        delta = timedelta(seconds=delta.seconds,microseconds=delta.microseconds)
+    # Add seconds in UTC because then there's no DST to worry about
+    r_utc = r.astimezone(timezone.utc)
+    r_utc += delta
+    # Convert back to localtime for return
+    r = r_utc.astimezone(_local_tz)
+    return r
+
+
 def guess_date_ord_from_locale() -> str:
     # Try to divine order of date (day/mon/yr mon/day/yr etc.) from locale.
     # Return a string like 'DMY' 'MDY' etc.
     dfmt = locale.nl_langinfo(locale.D_FMT) # E.g. '%x', '%m/%d/%Y'
     # To cope with dfmt=='%x': format a time & look at result
     st = date(year=3333,month=11,day=22).strftime(dfmt)
     ret = ''
```

### Comparing `pygenda-0.3.0/pygenda/pygenda_view.py` & `pygenda-0.3.1/pygenda/pygenda_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,14 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
 # General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Pygenda. If not, see <https://www.gnu.org/licenses/>.
 
 
-from gi import require_version as gi_require_version
-gi_require_version('Gtk', '3.0')
 from gi.repository import Gtk, Gdk, GLib
 from gi.repository.Pango import WrapMode as PWrapMode
 
 from icalendar import cal as iCal, Event as iEvent, Todo as iTodo
 from datetime import date as dt_date, datetime as dt_datetime, timedelta
 from typing import Optional, Union
 
@@ -104,14 +102,22 @@
     def keyrelease(cls, wid:Gtk.Widget, ev:Gdk.Event) -> None:
         # Called (from GUI.keypress()) on key release event
         # Default does nothing. Derived views may override.
         pass
 
 
     @classmethod
+    def default_entry_is_todo(cls) -> bool:
+        # Returns True if creating an "entry" in this view would
+        # mean creating a Todo item.
+        # Default is False - an "entry" would be an Event.
+        return False
+
+
+    @classmethod
     def new_entry_from_example(cls, en:Union[iEvent,iTodo]) -> None:
         # Creates new entry based on entry en. Used for pasting entries.
         # Type of entry should depend on View (e.g. Todo View -> to-do item).
         # Default implementation does nothing.
         pass
 
 
@@ -153,15 +159,15 @@
         # Default implementation: cursor not on todo list.
         return None
 
 
     @classmethod
     def cursor_goto_event(cls, ev:iEvent) -> bool:
         # Move cursor to given event.
-        # Return True if can (False if can't) jump to todo in this view.
+        # Return True if can (False if can't) jump to event in this view.
         # Default implementation does nothing & returns False.
         return False
 
 
     @classmethod
     def cursor_goto_todo(cls, todo:iTodo, list_idx:int) -> bool:
         # Move cursor to given todo in given list.
@@ -178,27 +184,30 @@
         # !! Note: might be better if it kept the cursor visible
         cls.zoom_ctx.remove_class('zoom'+str(cls.zoom_lvl)) # type:ignore
         cls.zoom_lvl = (cls.zoom_lvl+inc)%cls.zoom_lvls # type:ignore
         cls.zoom_ctx.add_class('zoom'+str(cls.zoom_lvl)) # type:ignore
 
 
     @staticmethod
-    def entry_text_label(ev:iCal.Event, dt_st:dt_date, dt_end:dt_date, add_location:bool=False) -> Gtk.Label:
+    def entry_text_label(ev:iCal.Event, dt_st:dt_date, dt_end:dt_date, add_location:bool=False, loc_max_chars:int=0) -> Gtk.Label:
         # Returns a GtkLabel with entry summary + icons as content.
         # Used by Week & Year views to display entries.
         lab = Gtk.Label()
         lab.set_line_wrap(True)
         lab.set_line_wrap_mode(PWrapMode.WORD_CHAR)
         lab.set_xalign(0)
         lab.set_yalign(0)
         endtm = View.entry_endtime(dt_st,dt_end,True)
         icons = View.entry_icons(ev,True)
         d_txt = ev['SUMMARY'] if 'SUMMARY' in ev else ''
         if add_location and 'LOCATION' in ev:
-            l_txt = ' (@{:s})'.format(ev['LOCATION'])
+            loc = ev['LOCATION']
+            if loc_max_chars>0 and len(loc)>loc_max_chars:
+                loc = loc[:loc_max_chars] + u'…'
+            l_txt = ' (@{:s})'.format(loc)
         else:
             l_txt = ''
         lab.set_text(u'{:s}{:s}{:s}{:s}'.format(d_txt,endtm,l_txt,icons))
         View.add_event_styles(lab, ev)
         return lab
```

### Comparing `pygenda-0.3.0/pygenda/pygenda_view_todo.py` & `pygenda-0.3.1/pygenda/pygenda_view_todo.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,14 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
 # General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Pygenda. If not, see <https://www.gnu.org/licenses/>.
 
 
-from gi import require_version as gi_require_version
-gi_require_version('Gtk', '3.0')
 from gi.repository import Gtk, Gdk, GLib
 from gi.repository.Pango import WrapMode as PWrapMode
 
 from icalendar import cal as iCal, Event as iEvent, Todo as iTodo
 from locale import gettext as _
 from typing import Optional, List, Tuple, Union
 
@@ -68,15 +66,14 @@
         k = _('todo_view_accel')
         return ord(k[0]) if len(k)>0 else 0
 
 
     @classmethod
     def init(cls) -> Gtk.Widget:
         # Called on startup.
-        # Gets view framework from glade file & tweaks/adds a few elements.
         # Returns widget containing view.
         cls._init_parse_list_config()
         cls._init_todo_widgets()
         cls._init_keymap()
         cls.init_zoom('todo_view', cls._topboxscroll.get_style_context())
         return cls._topboxscroll
 
@@ -179,14 +176,20 @@
         # Called from cursor_edit_entry() & delete_request().
         if len(cls._list_items[cls._cursor_list]) == 0:
             return None
         return cls._list_items[cls._cursor_list][cls._cursor_idx_in_list]
 
 
     @classmethod
+    def default_entry_is_todo(cls) -> bool:
+        # Returns True: creating an "entry" in Todo View -> new Todo
+        return True
+
+
+    @classmethod
     def new_entry_from_example(cls, en:Union[iEvent,iTodo]) -> None:
         # Creates new entry based on entry en. Used for pasting entries.
         # Type of entry depends on View (e.g. Todo View -> to-do item).
         cats = cls._list_default_cats[cls._cursor_list]
         new_en = Calendar.new_entry_from_example(en, e_type=EntryInfo.TYPE_TODO, e_cats=cats)
         cls.cursor_goto_todo(new_en, cls._cursor_list)
```

### Comparing `pygenda-0.3.0/pygenda/pygenda_view_week.py` & `pygenda-0.3.1/pygenda/pygenda_view_week.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,14 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
 # General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Pygenda. If not, see <https://www.gnu.org/licenses/>.
 
 
-from gi import require_version as gi_require_version
-gi_require_version('Gtk', '3.0')
 from gi.repository import Gtk, Gdk, GLib
 
 from calendar import day_abbr,month_name
 from datetime import time as dt_time, date as dt_date, datetime as dt_datetime, timedelta
 from icalendar import cal as iCal
 from locale import gettext as _
 from typing import Optional
@@ -53,16 +51,16 @@
     _day_ent_count = [0]*7 # entry count for each day
     _day_entries = [[], [], [], [], [], [], []]
     _week_viewed = None # So view will be fully redrawn when needed
     _last_cursor = None
     _scroll_to_cursor_in_day = None
     _target_entry = None
     _is_repeat_key = False
-    CURSOR_STYLE = 'weekview_cursor'
 
+    CURSOR_STYLE = 'weekview_cursor'
     SHOW_LOC_ALWAYS = 1 # constant 'enum' for _show_location flag
 
     @staticmethod
     def view_name() -> str:
         # Return (localised) string to use in menu
         return _('_Week View')
 
@@ -72,17 +70,17 @@
         k = _('week_view_accel')
         return ord(k[0]) if len(k)>0 else 0
 
 
     @classmethod
     def init(cls) -> Gtk.Widget:
         # Called on startup.
-        # Gets view framework from glade file & tweaks/adds a few elements.
+        # Gets view framework from UI file & tweaks/adds a few elements.
         # Returns widget containing view.
-        GUI.load_glade_file('view_week.glade')
+        GUI.load_ui_file('view_week.ui')
         cls._topbox = GUI._builder.get_object('view_week')
         cls._month_label = GUI._builder.get_object('week_label_month')
         cls._weekno_label = GUI._builder.get_object('week_label_weekno')
         cls._init_week_widgets()
         cls._init_keymap()
         cls._init_config()
         cls.init_zoom('week_view', cls._topbox.get_style_context())
@@ -172,14 +170,17 @@
         map = {'every_day':1, 'first_day':0}
         cls._show_ongoing = map[show_ongoing] if show_ongoing in map else 0
 
         # Set _show_location flag from config.
         show_loc = Config.get('week_view','show_event_location')
         map = {'always':cls.SHOW_LOC_ALWAYS, 'never':0}
         cls._show_location = map[show_loc] if show_loc in map else 0
+        cls._loc_max_chars = Config.get_int('week_view','location_max_chars')
+        if cls._loc_max_chars is None:
+            cls._loc_max_chars = 0
 
 
     @classmethod
     def _init_gestures(cls) -> None:
         # Initialise swipe gesture. Called from init().
         cls.gest_swipe = Gtk.GestureSwipe(widget=cls._topbox)
         cls.gest_swipe.set_propagation_phase(Gtk.PropagationPhase.CAPTURE)
@@ -259,15 +260,15 @@
         sorted_occurrences = Calendar.occurrence_list(dt, dt+timedelta(days=7))
         itr = iter(sorted_occurrences)
         try:
             occ = next(itr)
         except StopIteration:
             occ = None
         if cls._show_ongoing:
-            ongoing = [] # !! Replace with call to calendar
+            ongoing = Calendar.ongoing_list(dt)
             rollover_dt = dt # Might want this to be 2am or something
         oneday = timedelta(days=1)
         for i in range(7):
             dt_nxt = dt + oneday
             # Delete anything previously written to day v-box
             cls._day_rows[i].foreach(Gtk.Widget.destroy)
             if cls._show_ongoing:
@@ -324,15 +325,15 @@
         row = Gtk.Box()
         # Create entry mark (bullet or time) & add to row
         mark_label = cls.marker_label(ev, dt_st, is_ongoing)
         ctx = mark_label.get_style_context()
         ctx.add_class('weekview_marker') # add style for CSS
         row.add(mark_label)
         # Create entry content label & add to row
-        cont_label = cls.entry_text_label(ev, dt_st, dt_end, add_location=show_loc)
+        cont_label = cls.entry_text_label(ev, dt_st, dt_end, add_location=show_loc, loc_max_chars=cls._loc_max_chars)
         cont_label.set_hexpand(True) # Also sets hexpand_set to True
         row.add(cont_label)
         cls._day_rows[dayidx].add(row)
         cls._day_entries[dayidx].append(ev)
         cls._day_ent_count[dayidx] += 1
```

### Comparing `pygenda-0.3.0/pygenda/pygenda_view_year.py` & `pygenda-0.3.1/pygenda/pygenda_view_year.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,14 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
 # General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Pygenda. If not, see <https://www.gnu.org/licenses/>.
 
 
-from gi import require_version as gi_require_version
-gi_require_version('Gtk', '3.0')
 from gi.repository import Gtk, Gdk, GLib
 
 import calendar
 from datetime import date as dt_date, datetime as dt_datetime, timedelta
 from locale import gettext as _
 from icalendar import cal as iCal
 from typing import Tuple
@@ -74,17 +72,17 @@
         k = _('year_view_accel')
         return ord(k[0]) if len(k)>0 else 0
 
 
     @classmethod
     def init(cls) -> Gtk.Widget:
         # Called on startup.
-        # Gets view framework from glade file & tweaks/adds a few elements.
+        # Gets view framework from UI file & tweaks/adds a few elements.
         # Returns widget containing view.
-        GUI.load_glade_file('view_year.glade')
+        GUI.load_ui_file('view_year.ui')
         cls._topbox = GUI._builder.get_object('view_year')
         cls._grid_cells = GUI._builder.get_object('year_grid_days')
         cls._date_label = GUI._builder.get_object('year_datelabel')
         cls._date_content_scroll = GUI._builder.get_object('year_datecontent_scroll')
         cls._date_content = GUI._builder.get_object('year_datecontent')
         cls._draw_day_month_labels()
         cls._init_keymap()
@@ -165,14 +163,17 @@
     @classmethod
     def _init_config(cls) -> None:
         # Initialisation from config settings.
         # Set _show_location flag from config.
         show_loc = Config.get('year_view','show_event_location')
         map = {'always':cls.SHOW_LOC_ALWAYS, 'never':0}
         cls._show_location = map[show_loc] if show_loc in map else 0
+        cls._loc_max_chars = Config.get_int('year_view','location_max_chars')
+        if cls._loc_max_chars is None:
+            cls._loc_max_chars = 0
 
 
     @classmethod
     def _init_gestures(cls) -> None:
         # Initialise swipe gesture. Called from init().
         yge = GUI._builder.get_object('year_grid_events')
         cls.gest_swipe = Gtk.GestureSwipe(widget=yge)
@@ -327,15 +328,15 @@
             row = Gtk.Box()
             # Create entry mark (bullet or time) & add to row
             mark_label = cls.marker_label(occ[0], occ_dt_sta)
             ctx = mark_label.get_style_context()
             ctx.add_class('yearview_marker') # add style for CSS
             row.add(mark_label)
             # Create entry content label & add to row
-            cont_label = cls.entry_text_label(occ[0], occ_dt_sta, occ_dt_end, add_location=cls._show_location)
+            cont_label = cls.entry_text_label(occ[0], occ_dt_sta, occ_dt_end, add_location=cls._show_location, loc_max_chars=cls._loc_max_chars)
             cont_label.set_hexpand(True) # Also sets hexpand_set to True
             row.add(cont_label)
             cls._date_content.add(row)
             # See if we've hit the cursor target entry
             if cls._target_entry is not None and cls._target_entry is occ[0]:
                 View._cursor_idx_in_date = r
                 cls._target_entry = None
```

### Comparing `pygenda-0.3.0/pygenda/pygenda_widgets.py` & `pygenda-0.3.1/pygenda/pygenda_widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,14 @@
 # !! Possible addition: ctrl+tab in WidgetDate brings up a calendar
 #    (a GtkCalendar) to allow choice with touchscreen (maybe also add
 #    a button to WidgetDate).
 #    Maybe similar in WidgetTime if can find/make a graphical time
 #    picker widget.
 
 
-from gi import require_version as gi_require_version
-gi_require_version('Gtk', '3.0')
 from gi.repository import Gtk, Gdk, GLib, GObject
 
 from datetime import date as dt_date, time as dt_time, timedelta
 from calendar import monthrange
 from typing import Optional
 
 # for internationalisation/localisation
```

### Comparing `pygenda-0.3.0/pygenda.egg-info/PKG-INFO` & `pygenda-0.3.1/pygenda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygenda
-Version: 0.3.0
+Version: 0.3.1
 Summary: An agenda application inspired by Agenda programs on Psion PDAs.
 Home-page: https://github.com/semiprime/pygenda
 Author: Matthew Lewis
 Author-email: pygenda@semiprime.com
 License: GPLv3 only
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pygenda-0.3.0/pygenda.egg-info/SOURCES.txt` & `pygenda-0.3.1/pygenda.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 pygenda/css/disc.svg
 pygenda/css/gemini.css
 pygenda/css/loop+star.svg
 pygenda/css/loop.svg
 pygenda/css/pygenda.css
 pygenda/css/raspberrypi.css
 pygenda/css/star.svg
-pygenda/glade/dialog_event.glade
-pygenda/glade/dialog_find.glade
-pygenda/glade/dialog_todo.glade
-pygenda/glade/main.glade
-pygenda/glade/main2.glade
-pygenda/glade/view_week.glade
-pygenda/glade/view_year.glade
+pygenda/locale/pygenda.pot
 pygenda/locale/en_US/LC_MESSAGES/pygenda.mo
-pygenda/locale/fr/LC_MESSAGES/pygenda.mo
+pygenda/locale/fr/LC_MESSAGES/pygenda.mo
+pygenda/ui/dialog_event.ui
+pygenda/ui/dialog_find.ui
+pygenda/ui/dialog_todo.ui
+pygenda/ui/main.ui
+pygenda/ui/view_week.ui
+pygenda/ui/view_year.ui
```

### Comparing `pygenda-0.3.0/setup.py` & `pygenda-0.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     url = "https://github.com/semiprime/pygenda",
     author = "Matthew Lewis",
     author_email = "pygenda@semiprime.com",
     description = "An agenda application inspired by Agenda programs on Psion PDAs.",
     long_description = "Pygenda is a calendar/agenda application written in Python3/GTK3. The UI is inspired by the Agenda programs on the Psion Series 3 and Series 5 range of keyboard PDAs, with the aim of being suitable for devices such as Planet Computers' Gemini (running Linux).\n\nFor more information/latest source, see https://github.com/semiprime/pygenda",
     packages = ["pygenda"],
     cmdclass = {'bdist_egg': PygendaEggInstall}, # use custom install above
-    package_data = {'': ['glade/*.glade', 'css/*.css', 'css/*.svg', 'libpygenda_clipboard.so', 'locale/*/LC_MESSAGES/pygenda.mo', 'app/pygenda.desktop']}, # files for bdists
+    package_data = {'': ['ui/*.ui', 'css/*.css', 'css/*.svg', 'libpygenda_clipboard.so', 'locale/*/LC_MESSAGES/pygenda.mo', 'app/pygenda.desktop']}, # files for bdists
     license = "GPLv3 only",
     python_requires = ">=3.5",
     install_requires = [
         "PyGObject",
         "pycairo",
         "python-dateutil",
         "icalendar",
```

