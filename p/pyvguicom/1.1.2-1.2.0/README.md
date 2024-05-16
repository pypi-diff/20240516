# Comparing `tmp/pyvguicom-1.1.2.tar.gz` & `tmp/pyvguicom-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvguicom-1.1.2.tar", last modified: Sun May  5 17:54:38 2024, max compression
+gzip compressed data, was "pyvguicom-1.2.0.tar", last modified: Thu May 16 13:05:14 2024, max compression
```

## Comparing `pyvguicom-1.1.2.tar` & `pyvguicom-1.2.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-05 17:54:38.843153 pyvguicom-1.1.2/
--rw-r--r--   0 peterglen  (1000) users      (100)     3062 2024-05-05 17:54:38.843153 pyvguicom-1.1.2/PKG-INFO
--rw-rw-r--   0 peterglen  (1000) users      (100)     2330 2024-05-05 17:40:57.000000 pyvguicom-1.1.2/README.md
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-05 17:54:38.839153 pyvguicom-1.1.2/pyvguicom/
--rw-rw-r--   0 peterglen  (1000) users      (100)       13 2024-04-24 07:51:41.000000 pyvguicom-1.1.2/pyvguicom/__init__.py
--rw-r--r--   0 peterglen  (1000) users      (100)     7590 2024-05-05 17:19:18.000000 pyvguicom-1.1.2/pyvguicom/browsewin.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     3693 2024-04-24 07:55:00.000000 pyvguicom-1.1.2/pyvguicom/custwidg.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-05 17:54:38.843153 pyvguicom-1.1.2/pyvguicom/docs/
--rw-r--r--   0 peterglen  (1000) users      (100)        0 2024-05-05 17:51:13.000000 pyvguicom-1.1.2/pyvguicom/docs/__index__.py
--rw-r--r--   0 peterglen  (1000) users      (100)    35939 2024-05-05 17:53:16.000000 pyvguicom-1.1.2/pyvguicom/docs/browsewin.html
--rw-r--r--   0 peterglen  (1000) users      (100)    44251 2024-05-05 17:53:18.000000 pyvguicom-1.1.2/pyvguicom/docs/htmledit.html
--rw-r--r--   0 peterglen  (1000) users      (100)    81647 2024-05-05 17:53:25.000000 pyvguicom-1.1.2/pyvguicom/docs/pgbox.html
--rw-r--r--   0 peterglen  (1000) users      (100)    27700 2024-05-05 17:53:17.000000 pyvguicom-1.1.2/pyvguicom/docs/pgbutt.html
--rw-r--r--   0 peterglen  (1000) users      (100)    39527 2024-05-05 17:53:19.000000 pyvguicom-1.1.2/pyvguicom/docs/pgentry.html
--rw-r--r--   0 peterglen  (1000) users      (100)   181257 2024-05-05 17:53:24.000000 pyvguicom-1.1.2/pyvguicom/docs/pggui.html
--rw-r--r--   0 peterglen  (1000) users      (100)    54919 2024-05-05 17:53:16.000000 pyvguicom-1.1.2/pyvguicom/docs/pgsel.html
--rw-r--r--   0 peterglen  (1000) users      (100)    38344 2024-05-05 17:53:22.000000 pyvguicom-1.1.2/pyvguicom/docs/pgsimp.html
--rw-r--r--   0 peterglen  (1000) users      (100)    95560 2024-05-05 17:53:26.000000 pyvguicom-1.1.2/pyvguicom/docs/pgtextview.html
--rw-r--r--   0 peterglen  (1000) users      (100)    89497 2024-05-05 17:53:18.000000 pyvguicom-1.1.2/pyvguicom/docs/pgutils.html
--rw-r--r--   0 peterglen  (1000) users      (100)    93952 2024-05-05 17:53:20.000000 pyvguicom-1.1.2/pyvguicom/docs/pgwkit.html
--rw-r--r--   0 peterglen  (1000) users      (100)    32044 2024-04-23 13:57:10.000000 pyvguicom-1.1.2/pyvguicom/docs/sutil.html
--rw-r--r--   0 peterglen  (1000) users      (100)    10064 2023-09-14 20:07:28.000000 pyvguicom-1.1.2/pyvguicom/htmledit.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    20271 2024-04-24 11:20:12.000000 pyvguicom-1.1.2/pyvguicom/pgbox.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     6723 2024-04-24 06:56:13.000000 pyvguicom-1.1.2/pyvguicom/pgbutt.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    10486 2024-05-01 13:23:40.000000 pyvguicom-1.1.2/pyvguicom/pgentry.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    46488 2024-05-05 17:54:16.000000 pyvguicom-1.1.2/pyvguicom/pggui.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    13350 2024-05-05 17:10:41.000000 pyvguicom-1.1.2/pyvguicom/pgsel.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     7628 2024-04-24 13:25:59.000000 pyvguicom-1.1.2/pyvguicom/pgsimp.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     3228 2024-05-05 16:33:55.000000 pyvguicom-1.1.2/pyvguicom/pgtests.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    29341 2024-04-24 07:00:30.000000 pyvguicom-1.1.2/pyvguicom/pgtextview.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    31329 2024-05-05 16:33:34.000000 pyvguicom-1.1.2/pyvguicom/pgutils.py
--rw-r--r--   0 peterglen  (1000) users      (100)    26237 2024-05-05 17:19:38.000000 pyvguicom-1.1.2/pyvguicom/pgwkit.py
--rw-r--r--   0 peterglen  (1000) users      (100)     1017 2023-09-14 20:07:28.000000 pyvguicom-1.1.2/pyvguicom/plug.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     2902 2024-05-03 05:29:54.000000 pyvguicom-1.1.2/pyvguicom/testbutt.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     1150 2024-05-03 05:29:54.000000 pyvguicom-1.1.2/pyvguicom/testcust.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3091 2024-05-03 05:30:04.000000 pyvguicom-1.1.2/pyvguicom/testentry.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3624 2024-05-05 16:37:37.000000 pyvguicom-1.1.2/pyvguicom/testgui.py
--rwxr-xr-x   0 peterglen  (1000) users      (100)     8947 2023-09-14 20:07:28.000000 pyvguicom-1.1.2/pyvguicom/testicons.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3019 2024-05-03 05:32:33.000000 pyvguicom-1.1.2/pyvguicom/testlettsel.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     4067 2024-05-03 07:57:22.000000 pyvguicom-1.1.2/pyvguicom/testmsgs.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3214 2024-05-03 05:32:55.000000 pyvguicom-1.1.2/pyvguicom/testnums.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     4082 2024-04-24 11:12:22.000000 pyvguicom-1.1.2/pyvguicom/testroot.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     2371 2024-05-05 16:30:56.000000 pyvguicom-1.1.2/pyvguicom/testsimple.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     1883 2024-05-03 05:33:21.000000 pyvguicom-1.1.2/pyvguicom/testtests.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     7126 2024-05-03 05:34:29.000000 pyvguicom-1.1.2/pyvguicom/testtextv.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3965 2024-05-03 05:52:44.000000 pyvguicom-1.1.2/pyvguicom/testutils.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-05 17:54:38.843153 pyvguicom-1.1.2/pyvguicom.egg-info/
--rw-r--r--   0 peterglen  (1000) users      (100)     3062 2024-05-05 17:54:38.000000 pyvguicom-1.1.2/pyvguicom.egg-info/PKG-INFO
--rw-r--r--   0 peterglen  (1000) users      (100)     1115 2024-05-05 17:54:38.000000 pyvguicom-1.1.2/pyvguicom.egg-info/SOURCES.txt
--rw-r--r--   0 peterglen  (1000) users      (100)        1 2024-05-05 17:54:38.000000 pyvguicom-1.1.2/pyvguicom.egg-info/dependency_links.txt
--rw-r--r--   0 peterglen  (1000) users      (100)       10 2024-05-05 17:54:38.000000 pyvguicom-1.1.2/pyvguicom.egg-info/top_level.txt
--rw-r--r--   0 peterglen  (1000) users      (100)       38 2024-05-05 17:54:38.843153 pyvguicom-1.1.2/setup.cfg
--rw-rw-r--   0 peterglen  (1000) users      (100)     2054 2024-05-05 17:51:51.000000 pyvguicom-1.1.2/setup.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-16 13:05:14.592770 pyvguicom-1.2.0/
+-rw-r--r--   0 peterglen  (1000) users      (100)     3062 2024-05-16 13:05:14.592770 pyvguicom-1.2.0/PKG-INFO
+-rw-rw-r--   0 peterglen  (1000) users      (100)     2330 2024-05-05 17:40:57.000000 pyvguicom-1.2.0/README.md
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-16 13:05:14.588770 pyvguicom-1.2.0/pyvguicom/
+-rw-rw-r--   0 peterglen  (1000) users      (100)       13 2024-04-24 07:51:41.000000 pyvguicom-1.2.0/pyvguicom/__init__.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     7590 2024-05-05 17:19:18.000000 pyvguicom-1.2.0/pyvguicom/browsewin.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     3693 2024-04-24 07:55:00.000000 pyvguicom-1.2.0/pyvguicom/custwidg.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-16 13:05:14.592770 pyvguicom-1.2.0/pyvguicom/docs/
+-rw-r--r--   0 peterglen  (1000) users      (100)        0 2024-05-05 17:51:13.000000 pyvguicom-1.2.0/pyvguicom/docs/__index__.py
+-rw-r--r--   0 peterglen  (1000) users      (100)    35939 2024-05-05 17:53:16.000000 pyvguicom-1.2.0/pyvguicom/docs/browsewin.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    44251 2024-05-05 17:53:18.000000 pyvguicom-1.2.0/pyvguicom/docs/htmledit.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    81647 2024-05-05 17:53:25.000000 pyvguicom-1.2.0/pyvguicom/docs/pgbox.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    27700 2024-05-05 17:53:17.000000 pyvguicom-1.2.0/pyvguicom/docs/pgbutt.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    39527 2024-05-05 17:53:19.000000 pyvguicom-1.2.0/pyvguicom/docs/pgentry.html
+-rw-r--r--   0 peterglen  (1000) users      (100)   181257 2024-05-05 17:53:24.000000 pyvguicom-1.2.0/pyvguicom/docs/pggui.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    54919 2024-05-05 17:53:16.000000 pyvguicom-1.2.0/pyvguicom/docs/pgsel.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    38344 2024-05-05 17:53:22.000000 pyvguicom-1.2.0/pyvguicom/docs/pgsimp.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    95560 2024-05-05 17:53:26.000000 pyvguicom-1.2.0/pyvguicom/docs/pgtextview.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    89497 2024-05-05 17:53:18.000000 pyvguicom-1.2.0/pyvguicom/docs/pgutils.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    93952 2024-05-05 17:53:20.000000 pyvguicom-1.2.0/pyvguicom/docs/pgwkit.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    32044 2024-04-23 13:57:10.000000 pyvguicom-1.2.0/pyvguicom/docs/sutil.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    10064 2023-09-14 20:07:28.000000 pyvguicom-1.2.0/pyvguicom/htmledit.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    20271 2024-04-24 11:20:12.000000 pyvguicom-1.2.0/pyvguicom/pgbox.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     6723 2024-04-24 06:56:13.000000 pyvguicom-1.2.0/pyvguicom/pgbutt.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    10486 2024-05-01 13:23:40.000000 pyvguicom-1.2.0/pyvguicom/pgentry.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    46488 2024-05-16 13:05:00.000000 pyvguicom-1.2.0/pyvguicom/pggui.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    13350 2024-05-05 17:10:41.000000 pyvguicom-1.2.0/pyvguicom/pgsel.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     7628 2024-04-24 13:25:59.000000 pyvguicom-1.2.0/pyvguicom/pgsimp.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     3461 2024-05-13 01:26:36.000000 pyvguicom-1.2.0/pyvguicom/pgtests.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    29341 2024-04-24 07:00:30.000000 pyvguicom-1.2.0/pyvguicom/pgtextview.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    31329 2024-05-05 16:33:34.000000 pyvguicom-1.2.0/pyvguicom/pgutils.py
+-rw-r--r--   0 peterglen  (1000) users      (100)    26237 2024-05-05 17:19:38.000000 pyvguicom-1.2.0/pyvguicom/pgwkit.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     1017 2023-09-14 20:07:28.000000 pyvguicom-1.2.0/pyvguicom/plug.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     2902 2024-05-03 05:29:54.000000 pyvguicom-1.2.0/pyvguicom/testbutt.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     1150 2024-05-03 05:29:54.000000 pyvguicom-1.2.0/pyvguicom/testcust.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3091 2024-05-03 05:30:04.000000 pyvguicom-1.2.0/pyvguicom/testentry.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3624 2024-05-05 16:37:37.000000 pyvguicom-1.2.0/pyvguicom/testgui.py
+-rwxr-xr-x   0 peterglen  (1000) users      (100)     8947 2023-09-14 20:07:28.000000 pyvguicom-1.2.0/pyvguicom/testicons.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3019 2024-05-03 05:32:33.000000 pyvguicom-1.2.0/pyvguicom/testlettsel.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     4067 2024-05-03 07:57:22.000000 pyvguicom-1.2.0/pyvguicom/testmsgs.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3214 2024-05-03 05:32:55.000000 pyvguicom-1.2.0/pyvguicom/testnums.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     4082 2024-04-24 11:12:22.000000 pyvguicom-1.2.0/pyvguicom/testroot.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     2371 2024-05-05 16:30:56.000000 pyvguicom-1.2.0/pyvguicom/testsimple.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     2379 2024-05-13 01:30:02.000000 pyvguicom-1.2.0/pyvguicom/testtests.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     7126 2024-05-03 05:34:29.000000 pyvguicom-1.2.0/pyvguicom/testtextv.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3965 2024-05-03 05:52:44.000000 pyvguicom-1.2.0/pyvguicom/testutils.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-16 13:05:14.592770 pyvguicom-1.2.0/pyvguicom.egg-info/
+-rw-r--r--   0 peterglen  (1000) users      (100)     3062 2024-05-16 13:05:14.000000 pyvguicom-1.2.0/pyvguicom.egg-info/PKG-INFO
+-rw-r--r--   0 peterglen  (1000) users      (100)     1115 2024-05-16 13:05:14.000000 pyvguicom-1.2.0/pyvguicom.egg-info/SOURCES.txt
+-rw-r--r--   0 peterglen  (1000) users      (100)        1 2024-05-16 13:05:14.000000 pyvguicom-1.2.0/pyvguicom.egg-info/dependency_links.txt
+-rw-r--r--   0 peterglen  (1000) users      (100)       10 2024-05-16 13:05:14.000000 pyvguicom-1.2.0/pyvguicom.egg-info/top_level.txt
+-rw-r--r--   0 peterglen  (1000) users      (100)       38 2024-05-16 13:05:14.592770 pyvguicom-1.2.0/setup.cfg
+-rw-rw-r--   0 peterglen  (1000) users      (100)     2054 2024-05-05 17:51:51.000000 pyvguicom-1.2.0/setup.py
```

### Comparing `pyvguicom-1.1.2/PKG-INFO` & `pyvguicom-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvguicom
-Version: 1.1.2
+Version: 1.2.0
 Summary: High power secure server GUI utility helpers.
 Home-page: https://github.com/pglen/pyguicom.git
 Author: Peter Glen
 Author-email: peterglen99@gmail.com
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
```

### Comparing `pyvguicom-1.1.2/README.md` & `pyvguicom-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.1.2/pyvguicom/browsewin.py` & `pyvguicom-1.2.0/pyvguicom/browsewin.py`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.1.2/pyvguicom/custwidg.py` & `pyvguicom-1.2.0/pyvguicom/custwidg.py`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.1.2/pyvguicom/docs/browsewin.html` & `pyvguicom-1.2.0/pyvguicom/docs/browsewin.html`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.1.2/pyvguicom/docs/htmledit.html` & `pyvguicom-1.2.0/pyvguicom/docs/htmledit.html`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.1.2/pyvguicom/docs/pgbox.html` & `pyvguicom-1.2.0/pyvguicom/docs/pgbox.html`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.1.2/pyvguicom/docs/pgbutt.html` & `pyvguicom-1.2.0/pyvguicom/docs/pgbutt.html`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.1.2/pyvguicom/docs/pgentry.html` & `pyvguicom-1.2.0/pyvguicom/docs/pgentry.html`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.1.2/pyvguicom/docs/pggui.html` & `pyvguicom-1.2.0/pyvguicom/docs/pggui.html`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.1.2/pyvguicom/docs/pgsel.html` & `pyvguicom-1.2.0/pyvguicom/docs/pgsel.html`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.1.2/pyvguicom/docs/pgsimp.html` & `pyvguicom-1.2.0/pyvguicom/docs/pgsimp.html`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.1.2/pyvguicom/docs/pgtextview.html` & `pyvguicom-1.2.0/pyvguicom/docs/pgtextview.html`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.1.2/pyvguicom/docs/pgutils.html` & `pyvguicom-1.2.0/pyvguicom/docs/pgutils.html`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.1.2/pyvguicom/docs/pgwkit.html` & `pyvguicom-1.2.0/pyvguicom/docs/pgwkit.html`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.1.2/pyvguicom/docs/sutil.html` & `pyvguicom-1.2.0/pyvguicom/docs/sutil.html`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.1.2/pyvguicom/htmledit.py` & `pyvguicom-1.2.0/pyvguicom/htmledit.py`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.1.2/pyvguicom/pgbox.py` & `pyvguicom-1.2.0/pyvguicom/pgbox.py`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.1.2/pyvguicom/pgbutt.py` & `pyvguicom-1.2.0/pyvguicom/pgbutt.py`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.1.2/pyvguicom/pgentry.py` & `pyvguicom-1.2.0/pyvguicom/pgentry.py`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.1.2/pyvguicom/pggui.py` & `pyvguicom-1.2.0/pyvguicom/pggui.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 sys.path.append(realinc)
 
 import pgutils
 import pgsimp
 
 IDXERR = "Index is larger than the available number of controls."
 
-VERSION = "1.1.2"
+VERSION = "1.2.0"
 
 gui_testmode = 0
 
 def randcol():
     return random.randint(0, 255)
 
 def randcolstr(start = 0, endd = 255):
```

### Comparing `pyvguicom-1.1.2/pyvguicom/pgsel.py` & `pyvguicom-1.2.0/pyvguicom/pgsel.py`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.1.2/pyvguicom/pgsimp.py` & `pyvguicom-1.2.0/pyvguicom/pgsimp.py`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.1.2/pyvguicom/pgtests.py` & `pyvguicom-1.2.0/pyvguicom/pgtests.py`

 * *Files 9% similar despite different names*

```diff
@@ -86,14 +86,25 @@
     for aa in range(lenx):
         ridx = random.randint(0, len(allstr)-1)
         rr = allstr[ridx]
         strx += str(rr)
 
     return strx
 
+def randstrrand(lenmin, lenmax):
+
+    lenx = random.randint(lenmin, lenmax)
+    strx = ""
+    for aa in range(lenx):
+        ridx = random.randint(0, len(allstr)-1)
+        rr = allstr[ridx]
+        strx += str(rr)
+
+    return strx
+
 def randasc(lenx):
 
     strx = ""
     for aa in range(lenx):
         ridx = random.randint(0, len(allasc)-1)
         rr = allasc[ridx]
         strx += str(rr)
```

### Comparing `pyvguicom-1.1.2/pyvguicom/pgtextview.py` & `pyvguicom-1.2.0/pyvguicom/pgtextview.py`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.1.2/pyvguicom/pgutils.py` & `pyvguicom-1.2.0/pyvguicom/pgutils.py`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.1.2/pyvguicom/pgwkit.py` & `pyvguicom-1.2.0/pyvguicom/pgwkit.py`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.1.2/pyvguicom/plug.py` & `pyvguicom-1.2.0/pyvguicom/plug.py`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.1.2/pyvguicom/testbutt.py` & `pyvguicom-1.2.0/pyvguicom/testbutt.py`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.1.2/pyvguicom/testcust.py` & `pyvguicom-1.2.0/pyvguicom/testcust.py`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.1.2/pyvguicom/testentry.py` & `pyvguicom-1.2.0/pyvguicom/testentry.py`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.1.2/pyvguicom/testgui.py` & `pyvguicom-1.2.0/pyvguicom/testgui.py`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.1.2/pyvguicom/testicons.py` & `pyvguicom-1.2.0/pyvguicom/testicons.py`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.1.2/pyvguicom/testlettsel.py` & `pyvguicom-1.2.0/pyvguicom/testlettsel.py`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.1.2/pyvguicom/testmsgs.py` & `pyvguicom-1.2.0/pyvguicom/testmsgs.py`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.1.2/pyvguicom/testnums.py` & `pyvguicom-1.2.0/pyvguicom/testnums.py`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.1.2/pyvguicom/testroot.py` & `pyvguicom-1.2.0/pyvguicom/testroot.py`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.1.2/pyvguicom/testsimple.py` & `pyvguicom-1.2.0/pyvguicom/testsimple.py`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.1.2/pyvguicom/testtests.py` & `pyvguicom-1.2.0/pyvguicom/testtests.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,24 @@
 from gi.repository import Pango
 
 gi.require_version('PangoCairo', '1.0')
 from gi.repository import PangoCairo
 
 import pgtests
 
+def test_randstr(arg2, arg3):
+    rrr = pgtests.randstr(12)
+    print(rrr)
+    arg3.set_text(rrr)
+
+def test_randstrrand(arg2, arg3):
+    rrr = pgtests.randstrrand(6, 18)
+    print(rrr)
+    arg3.set_text(rrr)
+
 def test_rand(arg2, arg3):
     rrr = pgtests.randascii(12)
     print(rrr)
     arg3.set_text(rrr)
 
 def test_rand2(arg2, arg3):
     rrr = pgtests.randisodate()
@@ -45,14 +55,22 @@
     vbox = Gtk.VBox()
     hbox = Gtk.HBox()
 
     lab1 = Gtk.Label(label="Test Label")
     hbox.pack_start(lab1, 1, 1, 0)
     vbox.pack_start(hbox, 1, 1, 0)
 
+    butt = Gtk.Button.new_with_mnemonic("Test Rand Str")
+    butt.connect("clicked", test_randstr, lab1)
+    vbox.pack_start(butt, 0, 0, 2)
+
+    butt = Gtk.Button.new_with_mnemonic("Test Rand Rand")
+    butt.connect("clicked", test_randstrrand, lab1)
+    vbox.pack_start(butt, 0, 0, 2)
+
     butt = Gtk.Button.new_with_mnemonic("Test Rand")
     butt.connect("clicked", test_rand, lab1)
     vbox.pack_start(butt, 0, 0, 2)
 
     butt = Gtk.Button.new_with_mnemonic("Test randisodate")
     butt.connect("clicked", test_rand2, lab1)
     vbox.pack_start(butt, 0, 0, 2)
```

### Comparing `pyvguicom-1.1.2/pyvguicom/testtextv.py` & `pyvguicom-1.2.0/pyvguicom/testtextv.py`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.1.2/pyvguicom/testutils.py` & `pyvguicom-1.2.0/pyvguicom/testutils.py`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.1.2/pyvguicom.egg-info/PKG-INFO` & `pyvguicom-1.2.0/pyvguicom.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvguicom
-Version: 1.1.2
+Version: 1.2.0
 Summary: High power secure server GUI utility helpers.
 Home-page: https://github.com/pglen/pyguicom.git
 Author: Peter Glen
 Author-email: peterglen99@gmail.com
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
```

### Comparing `pyvguicom-1.1.2/pyvguicom.egg-info/SOURCES.txt` & `pyvguicom-1.2.0/pyvguicom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.1.2/setup.py` & `pyvguicom-1.2.0/setup.py`

 * *Files identical despite different names*

