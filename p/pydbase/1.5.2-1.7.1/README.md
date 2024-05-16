# Comparing `tmp/pydbase-1.5.2.tar.gz` & `tmp/pydbase-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydbase-1.5.2.tar", last modified: Wed Apr 10 07:28:05 2024, max compression
+gzip compressed data, was "pydbase-1.7.1.tar", last modified: Thu May 16 13:00:44 2024, max compression
```

## Comparing `pydbase-1.5.2.tar` & `pydbase-1.7.1.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-10 07:28:05.782636 pydbase-1.5.2/
--rw-r--r--   0 peterglen  (1000) users      (100)    15090 2024-04-10 07:28:05.778636 pydbase-1.5.2/PKG-INFO
--rw-rw-r--   0 peterglen  (1000) users      (100)    14676 2024-04-10 04:30:09.000000 pydbase-1.5.2/README.md
--rwxrwxr-x   0 peterglen  (1000) users      (100)     7868 2024-04-10 04:06:28.000000 pydbase-1.5.2/chainadm.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)    10564 2024-04-10 05:43:45.000000 pydbase-1.5.2/dbaseadm.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-10 07:28:05.762635 pydbase-1.5.2/man/
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-10 07:28:05.766635 pydbase-1.5.2/man/man1/
--rwxrwxr--   0 peterglen  (1000) users      (100)     4965 2024-04-10 05:42:53.000000 pydbase-1.5.2/man/man1/pydbase.1
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-10 07:28:05.766635 pydbase-1.5.2/pydbase/
--rwxr-xr-x   0 peterglen  (1000) users      (100)        9 2023-09-25 19:38:11.000000 pydbase-1.5.2/pydbase/__init__.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     5225 2024-04-10 04:19:06.000000 pydbase-1.5.2/pydbase/dbutils.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-10 07:28:05.766635 pydbase-1.5.2/pydbase/docs/
--rw-r--r--   0 peterglen  (1000) users      (100)    30197 2024-04-09 10:03:09.000000 pydbase-1.5.2/pydbase/docs/twinbase.html
--rw-r--r--   0 peterglen  (1000) users      (100)    47882 2024-04-09 10:03:08.000000 pydbase-1.5.2/pydbase/docs/twinchain.html
--rw-r--r--   0 peterglen  (1000) users      (100)   143863 2024-04-09 10:03:09.000000 pydbase-1.5.2/pydbase/docs/twincore.html
--rw-rw-r--   0 peterglen  (1000) users      (100)     3453 2024-04-01 01:42:37.000000 pydbase-1.5.2/pydbase/portalocker.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     6514 2024-04-09 09:24:34.000000 pydbase-1.5.2/pydbase/twinbase.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    12981 2024-04-07 03:32:50.000000 pydbase-1.5.2/pydbase/twinchain.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    47418 2024-04-10 04:19:44.000000 pydbase-1.5.2/pydbase/twincore.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-10 07:28:05.778636 pydbase-1.5.2/pydbase.egg-info/
--rw-r--r--   0 peterglen  (1000) users      (100)    15090 2024-04-10 07:28:05.000000 pydbase-1.5.2/pydbase.egg-info/PKG-INFO
--rw-r--r--   0 peterglen  (1000) users      (100)      895 2024-04-10 07:28:05.000000 pydbase-1.5.2/pydbase.egg-info/SOURCES.txt
--rw-r--r--   0 peterglen  (1000) users      (100)        1 2024-04-10 07:28:05.000000 pydbase-1.5.2/pydbase.egg-info/dependency_links.txt
--rw-r--r--   0 peterglen  (1000) users      (100)       76 2024-04-10 07:28:05.000000 pydbase-1.5.2/pydbase.egg-info/entry_points.txt
--rw-r--r--   0 peterglen  (1000) users      (100)       18 2024-04-10 07:28:05.000000 pydbase-1.5.2/pydbase.egg-info/top_level.txt
--rw-r--r--   0 peterglen  (1000) users      (100)       38 2024-04-10 07:28:05.782636 pydbase-1.5.2/setup.cfg
--rw-rw-r--   0 peterglen  (1000) users      (100)     2335 2024-04-09 10:17:21.000000 pydbase-1.5.2/setup.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-10 07:28:05.778636 pydbase-1.5.2/tests/
--rw-rw-r--   0 peterglen  (1000) users      (100)     1436 2024-04-01 04:09:23.000000 pydbase-1.5.2/tests/test_acreate.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1470 2024-04-01 08:57:38.000000 pydbase-1.5.2/tests/test_bigdata.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1399 2024-04-01 07:47:06.000000 pydbase-1.5.2/tests/test_bindata.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1497 2024-03-07 15:25:35.000000 pydbase-1.5.2/tests/test_chain.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     2045 2024-04-10 04:00:21.000000 pydbase-1.5.2/tests/test_chain_data.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     2350 2024-04-10 04:12:19.000000 pydbase-1.5.2/tests/test_chain_link.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1189 2024-02-28 03:53:28.000000 pydbase-1.5.2/tests/test_del.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1273 2024-02-28 03:53:43.000000 pydbase-1.5.2/tests/test_dump.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1305 2024-04-01 04:15:24.000000 pydbase-1.5.2/tests/test_find.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1310 2024-04-01 04:09:03.000000 pydbase-1.5.2/tests/test_findrec.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1385 2024-04-01 04:21:29.000000 pydbase-1.5.2/tests/test_getoffs.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1567 2024-02-28 04:02:31.000000 pydbase-1.5.2/tests/test_getrec.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1931 2024-04-01 04:17:37.000000 pydbase-1.5.2/tests/test_handles.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1471 2024-04-01 04:18:57.000000 pydbase-1.5.2/tests/test_inplace.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1108 2024-04-01 04:23:28.000000 pydbase-1.5.2/tests/test_integrity.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1574 2024-04-01 04:20:53.000000 pydbase-1.5.2/tests/test_list.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1541 2024-03-10 04:45:43.000000 pydbase-1.5.2/tests/test_lockrel.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1799 2024-04-02 05:26:52.000000 pydbase-1.5.2/tests/test_multi.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1927 2024-02-28 04:05:14.000000 pydbase-1.5.2/tests/test_packer.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1654 2024-04-01 09:10:20.000000 pydbase-1.5.2/tests/test_reindex.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1503 2024-04-01 04:22:41.000000 pydbase-1.5.2/tests/test_search.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1676 2024-04-01 03:36:26.000000 pydbase-1.5.2/tests/test_vacuum.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-16 13:00:44.414285 pydbase-1.7.1/
+-rw-r--r--   0 peterglen  (1000) users      (100)    15215 2024-05-16 13:00:44.414285 pydbase-1.7.1/PKG-INFO
+-rw-rw-r--   0 peterglen  (1000) users      (100)    14801 2024-04-30 03:23:54.000000 pydbase-1.7.1/README.md
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     8244 2024-04-14 08:12:31.000000 pydbase-1.7.1/chainadm.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)    12237 2024-05-06 07:53:45.000000 pydbase-1.7.1/dbaseadm.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-16 13:00:44.390277 pydbase-1.7.1/man/
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-16 13:00:44.390277 pydbase-1.7.1/man/man1/
+-rwxrwxr--   0 peterglen  (1000) users      (100)     4965 2024-04-10 05:42:53.000000 pydbase-1.7.1/man/man1/pydbase.1
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-16 13:00:44.394278 pydbase-1.7.1/pydbase/
+-rwxr-xr-x   0 peterglen  (1000) users      (100)        9 2023-09-25 19:38:11.000000 pydbase-1.7.1/pydbase/__init__.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     5260 2024-04-11 01:37:17.000000 pydbase-1.7.1/pydbase/dbutils.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-16 13:00:44.398279 pydbase-1.7.1/pydbase/docs/
+-rw-r--r--   0 peterglen  (1000) users      (100)    30956 2024-04-13 02:31:39.000000 pydbase-1.7.1/pydbase/docs/twinbase.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    48509 2024-04-13 02:31:38.000000 pydbase-1.7.1/pydbase/docs/twinchain.html
+-rw-r--r--   0 peterglen  (1000) users      (100)   143433 2024-04-13 02:31:39.000000 pydbase-1.7.1/pydbase/docs/twincore.html
+-rw-rw-r--   0 peterglen  (1000) users      (100)     3453 2024-04-01 01:42:37.000000 pydbase-1.7.1/pydbase/portalocker.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     6552 2024-05-15 04:21:18.000000 pydbase-1.7.1/pydbase/twinbase.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    13276 2024-04-13 01:22:50.000000 pydbase-1.7.1/pydbase/twinchain.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    47764 2024-05-15 04:20:53.000000 pydbase-1.7.1/pydbase/twincore.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-16 13:00:44.414285 pydbase-1.7.1/pydbase.egg-info/
+-rw-r--r--   0 peterglen  (1000) users      (100)    15215 2024-05-16 13:00:44.000000 pydbase-1.7.1/pydbase.egg-info/PKG-INFO
+-rw-r--r--   0 peterglen  (1000) users      (100)      918 2024-05-16 13:00:44.000000 pydbase-1.7.1/pydbase.egg-info/SOURCES.txt
+-rw-r--r--   0 peterglen  (1000) users      (100)        1 2024-05-16 13:00:44.000000 pydbase-1.7.1/pydbase.egg-info/dependency_links.txt
+-rw-r--r--   0 peterglen  (1000) users      (100)       76 2024-05-16 13:00:44.000000 pydbase-1.7.1/pydbase.egg-info/entry_points.txt
+-rw-r--r--   0 peterglen  (1000) users      (100)       18 2024-05-16 13:00:44.000000 pydbase-1.7.1/pydbase.egg-info/top_level.txt
+-rw-r--r--   0 peterglen  (1000) users      (100)       38 2024-05-16 13:00:44.414285 pydbase-1.7.1/setup.cfg
+-rw-rw-r--   0 peterglen  (1000) users      (100)     2334 2024-04-25 10:51:40.000000 pydbase-1.7.1/setup.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-16 13:00:44.414285 pydbase-1.7.1/tests/
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1436 2024-04-01 04:09:23.000000 pydbase-1.7.1/tests/test_acreate.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1470 2024-04-01 08:57:38.000000 pydbase-1.7.1/tests/test_bigdata.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1399 2024-04-01 07:47:06.000000 pydbase-1.7.1/tests/test_bindata.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1694 2024-04-25 11:08:36.000000 pydbase-1.7.1/tests/test_callback.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1497 2024-03-07 15:25:35.000000 pydbase-1.7.1/tests/test_chain.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     2045 2024-04-10 04:00:21.000000 pydbase-1.7.1/tests/test_chain_data.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     2350 2024-04-10 04:12:19.000000 pydbase-1.7.1/tests/test_chain_link.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1189 2024-02-28 03:53:28.000000 pydbase-1.7.1/tests/test_del.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1273 2024-02-28 03:53:43.000000 pydbase-1.7.1/tests/test_dump.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1322 2024-04-13 04:52:03.000000 pydbase-1.7.1/tests/test_find.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1310 2024-04-01 04:09:03.000000 pydbase-1.7.1/tests/test_findrec.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1751 2024-04-13 05:16:03.000000 pydbase-1.7.1/tests/test_getoffs.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1567 2024-02-28 04:02:31.000000 pydbase-1.7.1/tests/test_getrec.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1931 2024-04-01 04:17:37.000000 pydbase-1.7.1/tests/test_handles.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     2002 2024-04-13 00:14:22.000000 pydbase-1.7.1/tests/test_inplace.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1108 2024-04-01 04:23:28.000000 pydbase-1.7.1/tests/test_integrity.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1574 2024-04-01 04:20:53.000000 pydbase-1.7.1/tests/test_list.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1541 2024-03-10 04:45:43.000000 pydbase-1.7.1/tests/test_lockrel.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1799 2024-04-02 05:26:52.000000 pydbase-1.7.1/tests/test_multi.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1927 2024-02-28 04:05:14.000000 pydbase-1.7.1/tests/test_packer.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1654 2024-04-01 09:10:20.000000 pydbase-1.7.1/tests/test_reindex.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1503 2024-04-01 04:22:41.000000 pydbase-1.7.1/tests/test_search.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1676 2024-04-01 03:36:26.000000 pydbase-1.7.1/tests/test_vacuum.py
```

### Comparing `pydbase-1.5.2/PKG-INFO` & `pydbase-1.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydbase
-Version: 1.5.2
+Version: 1.7.1
 Summary: High speed database with key / data in python.
 Home-page: https://github.com/pglen/pydbase
 Author: Peter Glen
 Author-email: peterglen99@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -347,9 +347,11 @@
     1.4.5       Fri 01.Mar.2024     Misc fixes
     1.4.6       Mon 04.Mar.2024     Vacuum count on vacuumed records
     1.4.7       Tue 05.Mar.2024     In place record update
     1.4.8       Sat 09.Mar.2024     Added new locking mechanism
     1.4.9       Mon 01.Apr.2024     Updated to run on MSYS2, new locking
     1.5.0       Tue 02.Apr.2024     Cleaned, pip upload
     1.5.1       Wed 10.Apr.2024     Dangling lock .. fixed
+    1.6.0       Thu 25.Apr.2024     Added IDX pre and post callbacks
+    1.6.1       Mon 29.Apr.2024     D: option corrected
 
 // EOF
```

### Comparing `pydbase-1.5.2/README.md` & `pydbase-1.7.1/pydbase.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: pydbase
+Version: 1.7.1
+Summary: High speed database with key / data in python.
+Home-page: https://github.com/pglen/pydbase
+Author: Peter Glen
+Author-email: peterglen99@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3
+Description-Content-Type: text/markdown
+
 # pydbase
 
 ## High speed database with key / data
 
 #### see: blockchain functions at the end
 
  &nbsp; The motivation was to create a no frills way of saving / retrieving data.
@@ -334,9 +347,11 @@
     1.4.5       Fri 01.Mar.2024     Misc fixes
     1.4.6       Mon 04.Mar.2024     Vacuum count on vacuumed records
     1.4.7       Tue 05.Mar.2024     In place record update
     1.4.8       Sat 09.Mar.2024     Added new locking mechanism
     1.4.9       Mon 01.Apr.2024     Updated to run on MSYS2, new locking
     1.5.0       Tue 02.Apr.2024     Cleaned, pip upload
     1.5.1       Wed 10.Apr.2024     Dangling lock .. fixed
+    1.6.0       Thu 25.Apr.2024     Added IDX pre and post callbacks
+    1.6.1       Mon 29.Apr.2024     D: option corrected
 
 // EOF
```

### Comparing `pydbase-1.5.2/chainadm.py` & `pydbase-1.7.1/chainadm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,46 @@
 #!/usr/bin/env python3
 
-import  os, sys, getopt, signal, select, socket, time, struct
-import  random, stat, os.path, datetime, threading, warnings
-import  string, hashlib, uuid
-
-import pyvpacker
+# pylint: disable=C0321
+# pylint: disable=C0209
+# pylint: disable=C0103
+
+''' Drive chain database '''
+
+import  os
+import  sys
+import  getopt
+import  socket
+import  random
+import  string
+import  uuid
 
 import gettext
 gettext.bindtextdomain('thisapp', './locale/')
 gettext.textdomain('thisapp')
 _ = gettext.gettext
 
 from pydbase import twinchain
+from pydbase import twincore
 from pydbase import dbutils
 
-version = "0.0.1"
+INT_MAX = 0xffffffff
+
+version = "1.0.0"
 
-#print("hashes", hashlib.algorithms_guaranteed)
+allstr  =    " " + \
+                string.ascii_lowercase +  string.ascii_uppercase +  \
+                    string.digits
 
 # Module variables (pushed to a class)
 
 class _c():
     deffile = "pydbchain.pydb"
     maxx    = 0xffffffff
-    lcount  = twinchain.INT_MAX
+    lcount  = INT_MAX
     quiet   = 0;    writex  = 0
     randx   = 0;    skipx   = 0
     offsx   = 0;    delx    = 0
     delrx   = 0;    delrx2  = 0
     backx   = 0;    sdelx   = 0
     vacx    = 0;    recx    = 0
     integx  = 0;    checkx  = 0
@@ -39,35 +52,56 @@
     keyx    = "";   datax  = ""
     dkeyx   = "";   dumpx  = 0
     findrec = "";   getrec = -1
     datex = 0   ;   cntx = 1
     headx = ""  ;   gethead = -1
     getby = ""  ;   getoffs = ""
 
-def help():
+pname = os.path.split(__file__)[1]
+
+chelp = '''\
+Administer pydbase chain data.
+Usage: %s [options]
+   options: -a  data     append data to the end of chain
+            -z           randomize data
+            -g recnum    get record
+            -k reckey    get record by key/header
+            -G recnum    get record offset by key
+            -r recnum    get record header buy position
+            -n           append / show / get number of records
+            -e           override header (checked for valid UUID)
+            -t           print record's UUID date)
+            -s           skip count
+            -x           max record count to list
+            -m           dump chain data
+            -c           check data integrity
+            -i           check link integrity
+            -S           get db size
+            -v           increase verbosity
+            -h           help (this screen) '''  % (pname)
+
+__doc__ = "<pre>" + chelp + "</pre>"
+
+def phelp():
 
     ''' Deliver program usage information '''
+    print(chelp)
+    sys.exit()
 
-    print("Usage: %s [options]" % os.path.split(sys.argv[0])[1])
-    print("   Options: -a  data   append data to the end of chain")
-    print("            -g recnum  get record")
-    print("            -k reckey  get record by key/header")
-    print("            -G recnum  get record offset by key")
-    print("            -r recnum  get record header")
-    print("            -n         append / show / get number of records")
-    print("            -e         override header (checked for UUID)")
-    print("            -t         print record's UUID date)")
-    print("            -s         skip count")
-    print("            -x         max record count to list")
-    print("            -m         dump chain data")
-    print("            -c         check data integrity")
-    print("            -i         check link integrity")
-    print("            -S         get db size")
-    print("            -v         increase verbosity")
-    print("            -h         help (this screen)")
+# Return a random string based upon length
+
+def randstr(lenx):
+
+    ''' Deliver a random string for testing '''
+    strx = ""
+    for aa in range(lenx):
+        ridx = random.randint(0, len(allstr)-1)
+        rr = allstr[ridx]
+        strx += str(rr)
+    return strx
 
 def mainfunc():
 
     ''' Exersize funtions of the twinchain library. '''
 
     opts = []; args = []
 
@@ -79,20 +113,21 @@
     except getopt.GetoptError as err:
         print(_("Invalid option(s) on command line:"), err)
         sys.exit(1)
 
     # Scan twice so verbose shows up early
     for aa in opts:
         if aa[0] == "-h" or aa[0] == "-?":
-            help(); exit(1)
+            phelp()
+            sys.exit(1)
 
         if aa[0] == "-V":
-            print("Script Version:", version);
-            print("Engine Version:", twincore.version);
-            exit(0)
+            print("Script Version:", version)
+            print("Engine Version:", twincore.version)
+            sys.exit(0)
 
         if aa[0] == "-f":
             _c.deffile = aa[1]
 
         if aa[0] == "-a":
             _c.append = aa[1]
 
@@ -152,18 +187,16 @@
 
     ''' Execute individual function from command line '''
 
     # Create our database
     core = twinchain.TwinChain(_c.deffile, _c.pgdebug, _c.verbose)
 
     core.base_quiet     = _c.quiet
-    core.base_pgdebug   = _c.pgdebug
-    core.base_showdel   = _c.sdelx
-    core.base_integrity = _c.checkx
-    core.base_pgdebug   = _c.pgdebug
+    core.showdel        = _c.sdelx
+    core.integrity      = _c.checkx
 
     if _c.integx:
         #print("Integrity", _c.integx)
         errx = False; cnt = []
         sss = core.getdbsize()
         # Remember record zero is the anchor
         for aa in range(0, sss):
@@ -200,26 +233,28 @@
         #print("Checking", _c.checkx)
         errx = False; cnt = -1
         sss = core.getdbsize()
         for aa in range(sss):
             ppp = core.checkdata(aa)
             if _c.verbose:
                 print(aa, ppp)
-            if not ppp: errx = True; cnt = aa
+            if not ppp:
+                errx = True
+                cnt = aa
         if errx:
             print("error on rec", cnt)
         else:
             print("DB checks out OK")
 
     elif _c.dumpx:
         #print("Dumping", _c.dumpx)
         sss = core.getdbsize()
         cnt = _c.skipcnt
         if cnt >= sss:
-            print("Passed EOF")
+            #print("Passed EOF")
             sys.exit(0)
         end = min(sss, _c.maxx + cnt)
         while True:
             if cnt >= end:
                 break
             hhh = core.get_header(cnt)
             ppp = core.get_payload(cnt)
@@ -228,34 +263,33 @@
                 ddd = dbutils.uuid2date(uuid.UUID(ppp[0]))
             if hhh:
                 print(cnt, hhh, ddd, ppp)
             cnt = cnt + 1
 
     elif _c.append:
         #print("Appending", _c.append)
-        dicx = {}; arrx = []
-        arrx = _c.append.split()
-        if len(arrx) % 2:
-            dicx['unkown'] = _c.append
-        else:
-            for aa in arrx:
-                arrz = aa.split(":")
-                if len(arrz) == 1:
-                    arrx = aa
-                else:
-                    dicx[arrz[0]] = arrz[1]
-        # Array or dic?
-        if len(arrx):
-            dicx =  arrx
-        #print("Appending", dicx)
+        #dicx = {}; arrx = []
+        #arrx = _c.append.split()
+        #if len(arrx) % 2:
+        #    dicx['unkown'] = _c.append
+        #else:
+        #    for aa in arrx:
+        #        arrz = aa.split(":")
+        #        if len(arrz) == 1:
+        #            arrx = aa
+        #        else:
+        #            dicx[arrz[0]] = arrz[1]
+
+        if _c.verbose:
+            print("Appending", _c.append)
         for aaa in range(_c.cntx):
             if _c.headx:
-                core.appendwith(_c.headx, dicx)
+                core.appendwith(_c.headx, _c.append)
             else:
-                core.append(dicx)
+                core.append(_c.append)
 
     elif _c.getby:
         #print("get bykey getby")
         #rec = core.retrieve(_c.getby, _c.ncount)
         rec = core.get_data_bykey(_c.getby, _c.ncount)
         if not rec:
             print("Record:", "'" + _c.getby + "'", "not found")
```

### Comparing `pydbase-1.5.2/dbaseadm.py` & `pydbase-1.7.1/dbaseadm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,59 @@
 #!/usr/bin/env python3
 
-import  os, sys, getopt, signal, select, socket, time, struct
-import  random, stat, os.path, datetime, threading, warnings
+''' Module pydb '''
+
+import  os
+import  sys
+import  random
 import  string
+import  getopt
+
+base = os.path.dirname(os.path.realpath(__file__))
+sys.path.append(os.path.join(base, 'pydbase'))
+
+from pydbase import twincore
+from pydbase import dbutils
 
 import pyvpacker
 
 import gettext
 gettext.bindtextdomain('thisapp', './locale/')
 gettext.textdomain('thisapp')
 _ = gettext.gettext
 
-base = os.path.dirname(os.path.realpath(__file__))
-sys.path.append(os.path.join(base, 'pydbase'))
-
-from pydbase import twincore
-
 #print(sys.prefix)
 
+# pylint: disable=C0321
+# pylint: disable=C0103
+
 # ------------------------------------------------------------------------
 
 gl_lockname = "pydbase.main.lock"
 
 # Module variables (pushed to a class)
 
 class _m():
     pgdebug = 0;  verbose = 0
     keyonly = 0;  ncount  = 1
-    skipcnt = 0;  maxdel = 0xffffffff
-    lcount  = twincore.INT_MAX
+    maxdel = 0xffffffff
+    findoff = ""; lcount  = twincore.INT_MAX
     quiet   = 0; writex  = 0;   randx   = 0; skipx   = 0
     offsx   = 0; delx    = 0;   delrx   = 0; delrx2  = 0
-    backx   = 0; sdelx   = 0;   vacx    = 0; recx    = 0
-    integx  = 0; checkx  = 0;   sizex   = 0; findx   = ""
-    retrx   = ""; getit  = "";  keyx    = ""; datax  = ""
+    revx   = 0; showdelx = 0;   vacx    = 0; recx    = 0
+    integx  = 0; checkf  = 0;   sizex   = 0; findx   = ""
+    retrx   = ""; keyx    = ""; datax  = ""
     dkeyx   = ""; dumpx  = 0;   findrec = ""; getrec = 0
-    replace = 0 ; recpos = 0;   inplace = 0
+    replace = 0 ; recpos = 0;    decode = 0
+
     deffile = "pydbase.pydb"
 
-version = "0.4.1"
-vdate   = "Fri 01.Mar.2024"
+VERSION = "1.1.0"
+VDATE   = "Fri 26.Apr.2024"
+
 allstr  =    " " + \
                 string.ascii_lowercase +  string.ascii_uppercase +  \
                     string.digits
 
 # ------------------------------------------------------------------------
 
 # Return a random string based upon length
@@ -54,111 +64,115 @@
     strx = ""
     for aa in range(lenx):
         ridx = random.randint(0, len(allstr)-1)
         rr = allstr[ridx]
         strx += str(rr)
     return strx
 
-pname = os.path.split(sys.argv[0])[1]
+pname = os.path.split(__file__)[1]
 
-__doc__ = ''' \
-Usage: %s [options] [arg_key arg_data]
+chelp = '''\
+Administer pydbase data.  Version: %s
+Usage: %s [options] [newkey newdata]
    -h         Help (this screen)   -|-  -E         Replace record in place
    -V         Print version        -|-  -q         Quiet on, less printing
    -d         Debug level (0-10)   -|-  -v         Increment verbosity level
    -r         Randomize (with -w)  -|-  -w         Write random record(s)
    -z         Dump backwards(s)    -|-  -i         Show deleted record(s)
    -U         Vacuum DB            -|-  -R         Re-index / recover DB
    -I         DB Integrity check   -|-  -c         Set check integrity flag
-   -s         Skip to count recs   -|-  -K         List keys only
-   -S         Print num recs       -|-  -m         Dump data to console
-   -n  num    Num of recs (with -w)-|-  -t  keyval Retrieve by key
-   -o  offs   Get data from offset -|-  -G  num    Get record by number
-   -F  subkey Find by sub str      -|-  -g  num    Get number of recs.
+   -S         Print dbase size     -|-  -m         Dump data to console
+   -K         List all, keys only  -|-  -F  subkey Find rec. by subkey
+   -O         Decode pyvpacker     -|-  -s  subkey Find file offsets
+   -n  num    Num of recs (with -w)-|-  -t  keyval Retrieve by key value
+   -o  offs   Get data at offset   -|-  -g         Get records. skip/lim/dec
    -k  keyval Key to save          -|-  -a  str    Data to save
-   -y  keyval Find by key          -|-  -D  keyval Delete by key
+   -y  keyval Get rec offset       -|-  -D  keyval Delete by key skip/rev/lim
    -p  num    Skip number of recs  -|-  -u  recnum Delete at recnum
    -l  lim    Limit get records    -|-  -e  offs   Delete at offset
    -Z  keyval Get record position  -|-  -X  max    Limit recs on delete
    -f  file   DB file for save/retrieve default: 'pydbase.pydb')
-The verbosity / debug  level influences the amount of printout presented.
-Use quotes for multi word arguments.''' \
-     % (pname)
+The verbosity / debug  level influences the amount of printout presented.\
+'''  % (VERSION, pname, )
 
-def help():
+#   -C  num    Get and print num of records. Skip aware, decode aware
+
+__doc__ = "<pre>" + chelp + "</pre>"
+
+def phelp():
 
     ''' Program usage information '''
-    print(__doc__)
+    print(chelp)
     sys.exit(0)
 
 def mainfunc():
 
     ''' Exercise most / all functions of the twincore library '''
 
-    opts = []; args = []
+    opts = []
+    args = []
 
     # Old fashioned parsing
-    opts_args   = "a:d:e:f:g:k:l:n:o:s:t:u:x:y:p:D:F:G:X:Z:"
-    opts_normal = "mchiVrwzvqURIK?SE"
+    opts_args   = "a:d:e:f:k:l:n:o:s:t:u:x:y:p:D:F:G:X:Z:"
+    opts_normal = "mchiVrwzvgqURIK?SECO"
     try:
-        opts, args = getopt.getopt(sys.argv[1:],  opts_normal + opts_args)
+        opts, args = getopt.getopt(sys.argv[1:],  opts_args + opts_normal )
     except getopt.GetoptError as err:
         print(_("Invalid option(s) on command line:"), err)
         sys.exit(1)
 
     # Scan twice so verbose shows up early
     for aa in opts:
         if aa[0] == "-h" or aa[0] == "-?":
-            help(); exit(1)
+            phelp()
+            sys.exit(1)
         if aa[0] == "-v":
             _m.verbose += 1
         if aa[0] == "-d":
             try:
                 _m.pgdebug = int(aa[1])
                 #print( sys.argv[0], _("Running at debug level"),  pgdebug)
             except:
                 _m.pgdebug = 0
 
     for aa in opts:
         if aa[0] == "-V":
-            print("Script Version:", version);
-            print("Engine Version:", twincore.version);
+            core = twincore.TwinCore(_m.deffile, _m.pgdebug)
+            print("Script Version:", VERSION)
+            print("Engine Version:", twincore.VERSION)
+            print("Vers.from  API:", core.version())
 
             if _m.verbose > 0:
-                print("Compiled:", vdate);
-            exit(1)
+                print("Compiled:", VDATE)
+            sys.exit(1)
 
         # Action flags, one at a time
         if aa[0] == "-z":
-            _m.backx = True
+            _m.revx = True
         if aa[0] == "-u":
             _m.delrx2 = 1
             _m.delrx = int(aa[1])
         if aa[0] == "-w":
             _m.writex = True
         if aa[0] == "-i":
-            _m.sdelx = True
+            _m.showdelx = True
         if aa[0] == "-q":
             _m.quiet = True
         if aa[0] == "-n":
             _m.ncount = int(aa[1])
         if aa[0] == "-t":
             _m.retrx = aa[1]
         if aa[0] == "-l":
             _m.lcount = int(aa[1])
         if aa[0] == "-X":
             _m.maxdel = int(aa[1])
-        if aa[0] == "-s":
-            _m.skipcnt = int(aa[1])
         if aa[0] == "-f":
             _m.deffile = aa[1]
         if aa[0] == "-g":
-            _m.getit = aa[1]
-        if aa[0] == "-G":
-            _m.getrec = aa[1]
+            _m.getrec = True
         if aa[0] == "-k":
             _m.keyx = aa[1]
         if aa[0] == "-D":
             _m.dkeyx = aa[1]
         if aa[0] == "-a":
             _m.datax = aa[1]
         if aa[0] == "-r":
@@ -178,49 +192,56 @@
         if aa[0] == "-o":
             _m.offsx = aa[1]
         if aa[0] == "-e":
             _m.delx = aa[1]
         if aa[0] == "-E":
             _m.replace = True
         if aa[0] == "-c":
-            _m.checkx = True
+            _m.checkf = True
         if aa[0] == "-S":
             _m.sizex = True
+        if aa[0] == "-s":
+            _m.findoff = aa[1]
         if aa[0] == "-I":
             _m.integx = True
         if aa[0] == "-m":
             _m.dumpx = True
+        if aa[0] == "-O":
+            _m.decode = True
+            global packer
+            packer = pyvpacker.packbin()
         if aa[0] == "-F":
             _m.findrec = aa[1]
         if aa[0] == "-Z":
             _m.recpos = aa[1]
 
     #print("args", len(args), args)
 
     if len(args) == 1:
         print("Must have zero or two arguments. Use -h for help.")
         sys.exit(1)
 
     # Set some flags
     twincore.base_quiet     = _m.quiet
     twincore.base_pgdebug   = _m.pgdebug
-    twincore.base_showdel   = _m.sdelx
-    twincore.base_integrity = _m.checkx
     twincore.base_pgdebug   = _m.pgdebug
 
     # Create our database
     core = twincore.TwinCore(_m.deffile, _m.pgdebug)
-    core.base_verbose   = _m.verbose
+    core.verbose   = _m.verbose
+    core.showdel   = _m.showdelx
+    core.integrity = _m.checkf
 
     # See if we have two arguments, save it as data
     if len(args) == 2:
         #print("args", args)
         curr = core.save_data(args[0], args[1])
         sys.exit(0)
 
+    #print("version", core.get_version())
     #print(dir(core))
 
     dbsize = core.getdbsize()
     #print("DBsize", dbsize)
 
     if _m.keyx and _m.datax:
         curr = 0
@@ -234,60 +255,88 @@
         data = randstr(random.randint(4, 24))
         if _m.verbose:
             print("adding", _m.keyx, data)
         for aa in range(_m.ncount):
             curr = core.save_data(_m.keyx, data, _m.replace)
         #print("curr", curr)
     elif _m.writex:
-        curr = 0;
+        curr = 0
         if _m.randx:
             for aa in range(_m.ncount):
                 curr = core.save_data(
                     randstr(random.randint(2, 10)),
                         randstr(random.randint(10, 20)))
         else:
             for aa in range(_m.ncount):
                 curr = core.save_data("111 222", "333 444")
         #print("curr", curr)
     elif _m.findx:
         if _m.lcount == 0: _m.lcount = 1
         ddd = core.find_key(_m.findx, _m.lcount)
-        print("Found records:", ddd)
-    elif _m.getrec:
-        ddd = core.get_rec(int(_m.getrec))
-        print(_m.getrec, "Got:", ddd)
-
+        print("Found record offsets:", ddd)
     elif _m.keyonly:
         cnt = 0
         if _m.lcount + _m.skipx > dbsize:
             _m.lcount = dbsize - _m.skipx
-        for aa in range(_m.skipx, _m.lcount):
+        for aa in range( _m.lcount-1, _m.skipx-1, -1):
             ddd = core.get_rec(aa)
             print(aa, ddd)
             cnt += 1
 
-    elif _m.getit:
-        getx = int(_m.getit)
-        #skipx = dbsize - skipx
+    elif _m.getrec:
+        getx = 0xffff
         if getx + _m.skipx > dbsize:
             getx = dbsize - _m.skipx
+        if getx < 0:
+            getx = 0
+            #print("Clipping getx to dbsize of", dbsize)
         if _m.skipx < 0:
             _m.skipx = 0
-            print("Clipping to dbsize of", dbsize)
+            #print("Clipping to dbsize of", dbsize)
+
         if _m.verbose:
-            print("Getting %d records" % getx);
-            if _m.skipx:
-                print("With skipping %d records" % skipx);
+            print("Getting %d records, skipping %d " % (getx, _m.skipx))
 
-        for aa in range(_m.skipx, getx + _m.skipx):
+        cnt = 0
+        for aa in range(dbsize - 1 - _m.skipx, dbsize - 1 - getx - _m.skipx, -1):
+            #_m.skipx, getx + _m.skipx):
             ddd = core.get_rec(aa)
-            print(aa, ddd)
+            if not ddd:
+                continue
+            if cnt >= _m.lcount:
+                break
+            #print("ddd", ddd)
+            if _m.decode:
+                try:
+                    dec = packer.decode_data(ddd[1])[0]
+                    # attempt to do second level
+                except:
+                    # Cannot decode, Just show record
+                    if _m.verbose:
+                        print("cannot decode:", sys.exc_info())
+                    if _m.pgdebug > 2:
+                            dbutils.put_exception("pyvpacker")
+                    dec = ddd
+                try:
+                    if type(dec) == type({}):
+                        for aa in dec.keys():
+                            if str(dec[aa])[:2] == "pg":
+                                dec[aa] = packer.decode_data(dec[aa])[0]
+                except:
+                    # Cannot decode second level
+                    if _m.verbose:
+                        print("cannot decode second level:", sys.exc_info())
+                    if _m.pgdebug > 2:
+                        dbutils.put_exception("second level")
+                print(dec)
+            else:
+                print(ddd)
+            cnt += 1
 
     elif _m.retrx != "":
-        if _m.ncount == 0: _m.ncount = 1
         ddd = core.retrieve(_m.retrx, _m.ncount)
         if not ddd:
             print("Record:", "'" + _m.retrx + "'", "is not found.")
         else:
             print(ddd)
     elif _m.sizex:
         print("Database size:", core.getdbsize())
@@ -297,38 +346,43 @@
     elif _m.delx:
         ddd = core.del_rec_offs(int(_m.delx))
         print(ddd)
     elif _m.delrx2:
         ddd = core.del_rec(int(_m.delrx))
         print(ddd)
     elif _m.dkeyx:
-        ddd = core.del_rec_bykey(_m.dkeyx, maxdelrec = _m.maxdel)
+        ddd = core.del_rec_bykey(_m.dkeyx, _m.maxdel, _m.skipx, _m.revx)
         print("Deleted:", ddd, "records.")
     elif _m.recx:
         ddd = core.reindex()
         print("Reindexed:", ddd, "record(s)")
     elif _m.vacx:
         ddd = core.vacuum()
         print("Vacuumed:", ddd[0], "saved", ddd[1], "record(s)")
     elif _m.integx:
         ddd = core.integrity_check()
         print("Integrity check found good:", ddd[0], "of", ddd[1], "record(s)")
     elif _m.dumpx:
-        if _m.backx:
+        if _m.revx:
             core.dump_data(_m.lcount, _m.skipx)
         else:
             core.revdump_data(_m.lcount, _m.skipx)
     elif _m.findrec:
-            ret = core.findrec(_m.findrec, _m.lcount, _m.skipx)
-            if _m.verbose:
-                print("Found:", end = "")
-            print(ret)
+        ret = core.findrec(_m.findrec, _m.lcount, _m.skipx)
+        if _m.verbose:
+            print("Found:", end = "")
+        print(ret)
+    elif _m.findoff:
+        ret = core.findrecoffs(_m.findoff, _m.lcount, _m.skipx)
+        if _m.verbose:
+            print("Found:", end = "")
+        print(ret)
     elif _m.recpos:
-            ret = core.findrecpos(_m.recpos, _m.lcount, _m.skipx)
-            print(ret)
+        ret = core.findrecpos(_m.recpos, _m.lcount, _m.skipx)
+        print(ret)
     else:
         print("Use:", os.path.split(sys.argv[0])[1], "-h to see options and help")
 
 if __name__ == "__main__":
 
     # Tested with process based lock (OK)
     #twincore.waitlock(gl_lockname)
```

### Comparing `pydbase-1.5.2/man/man1/pydbase.1` & `pydbase-1.7.1/man/man1/pydbase.1`

 * *Files identical despite different names*

### Comparing `pydbase-1.5.2/pydbase/dbutils.py` & `pydbase-1.7.1/pydbase/dbutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,17 @@
             # Always remove file
             try:
                 os.remove(self.lockname)
             except:
                 pass
                 #print("cannot delete lock", self.lockname, sys.exc_info())
         except:
-            print("exc on del (ignored)", self.lockname, sys.exc_info())
+
+            if utils_pgdebug:
+                print("exc on del (ignored)", self.lockname, sys.exc_info())
             pass
 
 def truncs(strx, num = 8):
 
     ''' Truncate a string for printing nicely. Add '..' if truncated'''
 
     if len(strx) > num:
```

### Comparing `pydbase-1.5.2/pydbase/docs/twinbase.html` & `pydbase-1.7.1/pydbase/docs/twinbase.html`

 * *Files 3% similar despite different names*

```diff
@@ -62,23 +62,21 @@
 FILESIG     = b&#34;PYDB&#34;
 IDXSIG      = b&#34;PYIX&#34;
 RECSIG      = b&#34;RECB&#34;
 RECDEL      = b&#34;RECX&#34;
 RECSEP      = b&#34;RECS&#34;
 RECEND      = b&#34;RECE&#34;
 
-version = &#34;1.5.2&#34;
+version = &#34;1.5.3&#34;
 
 # Accessed from the main file as well
 
 base_locktout   = LOCK_TIMEOUT   # Settable from ...
 base_pgdebug    = 0
 base_quiet      = 0
-base_integrity  = 0
-base_showdel    = 0
 
 class TwinCoreBase():
 
     &#39;&#39;&#39; This class provides basic services to twincore  &#39;&#39;&#39;
 
     INTSIZE     = 4
 
@@ -98,14 +96,18 @@
         self.ifp = None
         self.cnt = 0
 
         #self.fname = &#34;&#34; ;        self.idxname = &#34;&#34;
         #self.lckname = &#34;&#34;;
         self.lasterr = &#34;&#34;
 
+    def get_version(self):
+        &#39;&#39;&#39; Return version sting. &#39;&#39;&#39;
+        return version
+
     #def __del__(self):
     #    print(&#34;Flushing&#34;)
 
     def getsize(self, buffio):
 
         &#39;&#39;&#39; get the dabase file size &#39;&#39;&#39;
 
@@ -312,14 +314,18 @@
         self.ifp = None
         self.cnt = 0
 
         #self.fname = &#34;&#34; ;        self.idxname = &#34;&#34;
         #self.lckname = &#34;&#34;;
         self.lasterr = &#34;&#34;
 
+    def get_version(self):
+        &#39;&#39;&#39; Return version sting. &#39;&#39;&#39;
+        return version
+
     #def __del__(self):
     #    print(&#34;Flushing&#34;)
 
     def getsize(self, buffio):
 
         &#39;&#39;&#39; get the dabase file size &#39;&#39;&#39;
 
@@ -550,14 +556,28 @@
     ifp.write(outx)
 
     #pp = struct.pack(&#34;I&#34;, HEADSIZE)
     #ifp.seek(CURROFFS, io.SEEK_SET)
     #ifp.write(pp)</code></pre>
 </details>
 </dd>
+<dt id="twinbase.TwinCoreBase.get_version"><code class="name flex">
+<span>def <span class="ident">get_version</span></span>(<span>self)</span>
+</code></dt>
+<dd>
+<div class="desc"><p>Return version sting.</p></div>
+<details class="source">
+<summary>
+<span>Expand source code</span>
+</summary>
+<pre><code class="python">def get_version(self):
+    &#39;&#39;&#39; Return version sting. &#39;&#39;&#39;
+    return version</code></pre>
+</details>
+</dd>
 <dt id="twinbase.TwinCoreBase.getbuffint"><code class="name flex">
 <span>def <span class="ident">getbuffint</span></span>(<span>self, offs)</span>
 </code></dt>
 <dd>
 <div class="desc"><p>get an integer value from offset</p></div>
 <details class="source">
 <summary>
@@ -759,14 +779,15 @@
 <ul>
 <li>
 <h4><code><a title="twinbase.TwinCoreBase" href="#twinbase.TwinCoreBase">TwinCoreBase</a></code></h4>
 <ul class="two-column">
 <li><code><a title="twinbase.TwinCoreBase.INTSIZE" href="#twinbase.TwinCoreBase.INTSIZE">INTSIZE</a></code></li>
 <li><code><a title="twinbase.TwinCoreBase.create_data" href="#twinbase.TwinCoreBase.create_data">create_data</a></code></li>
 <li><code><a title="twinbase.TwinCoreBase.create_idx" href="#twinbase.TwinCoreBase.create_idx">create_idx</a></code></li>
+<li><code><a title="twinbase.TwinCoreBase.get_version" href="#twinbase.TwinCoreBase.get_version">get_version</a></code></li>
 <li><code><a title="twinbase.TwinCoreBase.getbuffint" href="#twinbase.TwinCoreBase.getbuffint">getbuffint</a></code></li>
 <li><code><a title="twinbase.TwinCoreBase.getbuffstr" href="#twinbase.TwinCoreBase.getbuffstr">getbuffstr</a></code></li>
 <li><code><a title="twinbase.TwinCoreBase.getidxint" href="#twinbase.TwinCoreBase.getidxint">getidxint</a></code></li>
 <li><code><a title="twinbase.TwinCoreBase.getsize" href="#twinbase.TwinCoreBase.getsize">getsize</a></code></li>
 <li><code><a title="twinbase.TwinCoreBase.hash32" href="#twinbase.TwinCoreBase.hash32">hash32</a></code></li>
 <li><code><a title="twinbase.TwinCoreBase.putbuffint" href="#twinbase.TwinCoreBase.putbuffint">putbuffint</a></code></li>
 <li><code><a title="twinbase.TwinCoreBase.putbuffstr" href="#twinbase.TwinCoreBase.putbuffstr">putbuffstr</a></code></li>
```

#### html2text {}

```diff
@@ -34,23 +34,21 @@
 FILESIG     = b"PYDB"
 IDXSIG      = b"PYIX"
 RECSIG      = b"RECB"
 RECDEL      = b"RECX"
 RECSEP      = b"RECS"
 RECEND      = b"RECE"
 
-version = "1.5.2"
+version = "1.5.3"
 
 # Accessed from the main file as well
 
 base_locktout   = LOCK_TIMEOUT   # Settable from ...
 base_pgdebug    = 0
 base_quiet      = 0
-base_integrity  = 0
-base_showdel    = 0
 
 class TwinCoreBase():
 
     ''' This class provides basic services to twincore  '''
 
     INTSIZE     = 4
 
@@ -70,14 +68,18 @@
         self.ifp = None
         self.cnt = 0
 
         #self.fname = "" ;        self.idxname = ""
         #self.lckname = "";
         self.lasterr = ""
 
+    def get_version(self):
+        ''' Return version sting. '''
+        return version
+
     #def __del__(self):
     #    print("Flushing")
 
     def getsize(self, buffio):
 
         ''' get the dabase file size '''
 
@@ -268,14 +270,18 @@
               self.ifp = None
               self.cnt = 0
 
               #self.fname = "" ;        self.idxname = ""
               #self.lckname = "";
               self.lasterr = ""
 
+          def get_version(self):
+              ''' Return version sting. '''
+              return version
+
           #def __del__(self):
           #    print("Flushing")
 
           def getsize(self, buffio):
 
               ''' get the dabase file size '''
 
@@ -485,14 +491,20 @@
                 outx = b"".join(arrx)
                 ifp.seek(0)
                 ifp.write(outx)
 
                 #pp = struct.pack("I", HEADSIZE)
                 #ifp.seek(CURROFFS, io.SEEK_SET)
                 #ifp.write(pp)
+        def get_version(self)
+            Return version sting.
+            Expand source code
+            def get_version(self):
+                ''' Return version sting. '''
+                return version
         def getbuffint(self, offs)
             get an integer value from offset
             Expand source code
             def getbuffint(self, offs):
                 ''' get an integer value from offset '''
                 self.fp.seek(offs, io.SEEK_SET)
                 val = self.fp.read(4)
@@ -610,14 +622,15 @@
                 return fp
 ************ IInnddeexx ************
     * ******** _CC_ll_aa_ss_ss_ee_ss ********
           o ****** _TT_ww_ii_nn_CC_oo_rr_ee_BB_aa_ss_ee ******
                 # _I_N_T_S_I_Z_E
                 # _c_r_e_a_t_e___d_a_t_a
                 # _c_r_e_a_t_e___i_d_x
+                # _g_e_t___v_e_r_s_i_o_n
                 # _g_e_t_b_u_f_f_i_n_t
                 # _g_e_t_b_u_f_f_s_t_r
                 # _g_e_t_i_d_x_i_n_t
                 # _g_e_t_s_i_z_e
                 # _h_a_s_h_3_2
                 # _p_u_t_b_u_f_f_i_n_t
                 # _p_u_t_b_u_f_f_s_t_r
```

### Comparing `pydbase-1.5.2/pydbase/docs/twinchain.html` & `pydbase-1.7.1/pydbase/docs/twinchain.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 <!doctype html>
 <html lang="en">
 <head>
 <meta charset="utf-8">
 <meta name="viewport" content="width=device-width, initial-scale=1, minimum-scale=1" />
 <meta name="generator" content="pdoc 0.10.0" />
 <title>twinchain API documentation</title>
-<meta name="description" content="!
-@mainpage …" />
+<meta name="description" content="&lt;pre&gt; …" />
 <link rel="preload stylesheet" as="style" href="https://cdnjs.cloudflare.com/ajax/libs/10up-sanitize.css/11.0.1/sanitize.min.css" integrity="sha256-PK9q560IAAa6WVRRh76LtCaI8pjTJ2z11v0miyNNjrs=" crossorigin>
 <link rel="preload stylesheet" as="style" href="https://cdnjs.cloudflare.com/ajax/libs/10up-sanitize.css/11.0.1/typography.min.css" integrity="sha256-7l/o7C8jubJiy74VsKTidCy1yBkRtiUGbVkYBylBqUg=" crossorigin>
 <link rel="stylesheet preload" as="style" href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.1.1/styles/github.min.css" crossorigin>
 <style>:root{--highlight-color:#fe9}.flex{display:flex !important}body{line-height:1.5em}#content{padding:20px}#sidebar{padding:30px;overflow:hidden}#sidebar > *:last-child{margin-bottom:2cm}.http-server-breadcrumbs{font-size:130%;margin:0 0 15px 0}#footer{font-size:.75em;padding:5px 30px;border-top:1px solid #ddd;text-align:right}#footer p{margin:0 0 0 1em;display:inline-block}#footer p:last-child{margin-right:30px}h1,h2,h3,h4,h5{font-weight:300}h1{font-size:2.5em;line-height:1.1em}h2{font-size:1.75em;margin:1em 0 .50em 0}h3{font-size:1.4em;margin:25px 0 10px 0}h4{margin:0;font-size:105%}h1:target,h2:target,h3:target,h4:target,h5:target,h6:target{background:var(--highlight-color);padding:.2em 0}a{color:#058;text-decoration:none;transition:color .3s ease-in-out}a:hover{color:#e82}.title code{font-weight:bold}h2[id^="header-"]{margin-top:2em}.ident{color:#900}pre code{background:#f8f8f8;font-size:.8em;line-height:1.4em}code{background:#f2f2f1;padding:1px 4px;overflow-wrap:break-word}h1 code{background:transparent}pre{background:#f8f8f8;border:0;border-top:1px solid #ccc;border-bottom:1px solid #ccc;margin:1em 0;padding:1ex}#http-server-module-list{display:flex;flex-flow:column}#http-server-module-list div{display:flex}#http-server-module-list dt{min-width:10%}#http-server-module-list p{margin-top:0}.toc ul,#index{list-style-type:none;margin:0;padding:0}#index code{background:transparent}#index h3{border-bottom:1px solid #ddd}#index ul{padding:0}#index h4{margin-top:.6em;font-weight:bold}@media (min-width:200ex){#index .two-column{column-count:2}}@media (min-width:300ex){#index .two-column{column-count:3}}dl{margin-bottom:2em}dl dl:last-child{margin-bottom:4em}dd{margin:0 0 1em 3em}#header-classes + dl > dd{margin-bottom:3em}dd dd{margin-left:2em}dd p{margin:10px 0}.name{background:#eee;font-weight:bold;font-size:.85em;padding:5px 10px;display:inline-block;min-width:40%}.name:hover{background:#e0e0e0}dt:target .name{background:var(--highlight-color)}.name > span:first-child{white-space:nowrap}.name.class > span:nth-child(2){margin-left:.4em}.inherited{color:#999;border-left:5px solid #eee;padding-left:1em}.inheritance em{font-style:normal;font-weight:bold}.desc h2{font-weight:400;font-size:1.25em}.desc h3{font-size:1em}.desc dt code{background:inherit}.source summary,.git-link-div{color:#666;text-align:right;font-weight:400;font-size:.8em;text-transform:uppercase}.source summary > *{white-space:nowrap;cursor:pointer}.git-link{color:inherit;margin-left:1em}.source pre{max-height:500px;overflow:auto;margin:0}.source pre code{font-size:12px;overflow:visible}.hlist{list-style:none}.hlist li{display:inline}.hlist li:after{content:',\2002'}.hlist li:last-child:after{content:none}.hlist .hlist{display:inline;padding-left:1em}img{max-width:100%}td{padding:0 .5em}.admonition{padding:.1em .5em;margin-bottom:1em}.admonition-title{font-weight:bold}.admonition.note,.admonition.info,.admonition.important{background:#aef}.admonition.todo,.admonition.versionadded,.admonition.tip,.admonition.hint{background:#dfd}.admonition.warning,.admonition.versionchanged,.admonition.deprecated{background:#fd4}.admonition.error,.admonition.danger,.admonition.caution{background:lightpink}</style>
 <style media="screen and (min-width: 700px)">@media screen and (min-width:700px){#sidebar{width:30%;height:100vh;overflow:auto;position:sticky;top:0}#content{width:70%;max-width:100ch;padding:3em 4em;border-left:1px solid #ddd}pre code{font-size:1em}.item .name{font-size:1em}main{display:flex;flex-direction:row-reverse;justify-content:flex-end}.toc ul ul,#index ul{padding-left:1.5em}.toc > ul > li{margin-top:.5em}}</style>
 <style media="print">@media print{#sidebar h1{page-break-before:always}.source{display:none}}@media print{*{background:transparent !important;color:#000 !important;box-shadow:none !important;text-shadow:none !important}a[href]:after{content:" (" attr(href) ")";font-size:90%}a[href][title]:after{content:none}abbr[title]:after{content:" (" attr(title) ")"}.ir a:after,a[href^="javascript:"]:after,a[href^="#"]:after{content:""}pre,blockquote{border:1px solid #999;page-break-inside:avoid}thead{display:table-header-group}tr,img{page-break-inside:avoid}img{max-width:100% !important}@page{margin:0.5cm}p,h2,h3{orphans:3;widows:3}h1,h2,h3,h4,h5,h6{page-break-after:avoid}}</style>
 <script defer src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.1.1/highlight.min.js" integrity="sha256-Uv3H6lx7dJmRfRvH8TH6kJD1TSK1aFcwgx+mdg3epi8=" crossorigin></script>
@@ -19,72 +18,81 @@
 <body>
 <main>
 <article id="content">
 <header>
 <h1 class="title">Module <code>twinchain</code></h1>
 </header>
 <section id="section-intro">
-<p>!
-@mainpage</p>
-<h1 id="twinchain">Twinchain</h1>
-<pre><code>Block chain layer on top of twincore.
-
-    prev     curr
-        record
-|   Time Now    |   Time  Now    |  Time Now     |
-|   hash256   | |    hash256   | |   hash256   | |
-|   Header    | |    Header    | |   Header    | |
-|   Payload   | |    Payload   | |   Payload   | |
-|   Backlink  | |    Backlink  | |   Backlink  | |
-              |-----&gt;---|      |----&gt;---|     |------ ...
+<pre>
 
-The sum of fields saved to the next backlink.
+Block chain layer on top of twincore.
 
-History:
+   |   Time Now    |   Time  Now    |  Time Now     |
+   |   hash256   | |    hash256   | |   hash256   | |
+   |   Header    | |    Header    | |   Header    | |
+   |   Payload   | |    Payload   | |   Payload   | |
+   |   Backlink  | |    Backlink  | |   Backlink  | |
+                 |----->---|      |---->---|     |------
+
+   The sum of fields saved to the next backlink.
+
+   History:
+
+   1.1         Tue 20.Feb.2024     Initial release
+   1.2.0       Mon 26.Feb.2024     Moved pip home to pydbase/
+   1.4.0       Tue 27.Feb.2024     Addedd pgdebug
+   1.4.2       Wed 28.Feb.2024     Fixed multiple instances
+   1.4.3       Wed 28.Feb.2024     ChainAdm added
+   1.4.4       Fri 01.Mar.2024     Tests for chain functions
+   1.4.5       Fri 01.Mar.2024     Misc fixes
+   1.4.6       Mon 04.Mar.2024     Vacuum count on vacuumed records
+   1.4.7       Tue 05.Mar.2024     In place record update
+   1.4.8       Sat 09.Mar.2024     Added new locking mechanism
+   1.4.9       Mon 01.Apr.2024     Updated to run on MSYS2, new locking
+   1.5.0       Tue 02.Apr.2024     Cleaned, pip upload
+   1.5.1       Wed 10.Apr.2024     Dangling lock .. fixed
 
-    0.0.0       Tue 20.Feb.2024     Initial release
-    0.0.0       Sun 26.Mar.2023     More features
-    1.2.0       Mon 26.Feb.2024     Moved pip home to pydbase/
-    1.4.0       Tue 27.Feb.2024     Addedd pgdebug
-    1.4.2       Wed 28.Feb.2024     Fixed multiple instances
-    1.4.3       Wed 28.Feb.2024     ChainAdm added
-</code></pre>
+   </pre>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
 <pre><code class="python">#!/usr/bin/env python3
 
-&#39;&#39;&#39;!
-    @mainpage
+&#39;&#39;&#39;
+    &lt;pre&gt;
+
+ Block chain layer on top of twincore.
 
-    # Twinchain
+    |   Time Now    |   Time  Now    |  Time Now     |
+    |   hash256   | |    hash256   | |   hash256   | |
+    |   Header    | |    Header    | |   Header    | |
+    |   Payload   | |    Payload   | |   Payload   | |
+    |   Backlink  | |    Backlink  | |   Backlink  | |
+                  |-----&gt;---|      |----&gt;---|     |------
 
-        Block chain layer on top of twincore.
+    The sum of fields saved to the next backlink.
 
-            prev     curr
-                record
-        |   Time Now    |   Time  Now    |  Time Now     |
-        |   hash256   | |    hash256   | |   hash256   | |
-        |   Header    | |    Header    | |   Header    | |
-        |   Payload   | |    Payload   | |   Payload   | |
-        |   Backlink  | |    Backlink  | |   Backlink  | |
-                      |-----&gt;---|      |----&gt;---|     |------ ...
-
-        The sum of fields saved to the next backlink.
-
-        History:
-
-            0.0.0       Tue 20.Feb.2024     Initial release
-            0.0.0       Sun 26.Mar.2023     More features
-            1.2.0       Mon 26.Feb.2024     Moved pip home to pydbase/
-            1.4.0       Tue 27.Feb.2024     Addedd pgdebug
-            1.4.2       Wed 28.Feb.2024     Fixed multiple instances
-            1.4.3       Wed 28.Feb.2024     ChainAdm added
+    History:
 
+    1.1         Tue 20.Feb.2024     Initial release
+    1.2.0       Mon 26.Feb.2024     Moved pip home to pydbase/
+    1.4.0       Tue 27.Feb.2024     Addedd pgdebug
+    1.4.2       Wed 28.Feb.2024     Fixed multiple instances
+    1.4.3       Wed 28.Feb.2024     ChainAdm added
+    1.4.4       Fri 01.Mar.2024     Tests for chain functions
+    1.4.5       Fri 01.Mar.2024     Misc fixes
+    1.4.6       Mon 04.Mar.2024     Vacuum count on vacuumed records
+    1.4.7       Tue 05.Mar.2024     In place record update
+    1.4.8       Sat 09.Mar.2024     Added new locking mechanism
+    1.4.9       Mon 01.Apr.2024     Updated to run on MSYS2, new locking
+    1.5.0       Tue 02.Apr.2024     Cleaned, pip upload
+    1.5.1       Wed 10.Apr.2024     Dangling lock .. fixed
+
+    &lt;/pre&gt;
 &#39;&#39;&#39;
 
 import  os, sys, getopt, signal, select, socket, time, struct
 import  random, stat, os.path, datetime, threading, uuid
 import  struct, io, hashlib
 
 import pyvpacker
@@ -114,17 +122,17 @@
 
 class TwinChain(TwinCore):
 
     &#39;&#39;&#39;
         Derive from database to accomodate block chain.
     &#39;&#39;&#39;
 
-    def __init__(self, fname = &#34;pydbchain.pydb&#34;, pgdebug = 0, core_verbose = 0):
+    def __init__(self, fname = &#34;pydbchain.pydb&#34;, pgdebug = 0, verbose = 0):
 
-        self.core_verbose = core_verbose
+        self.chain_verbose = verbose
 
         # Upper lock name
         ulockname = os.path.splitext(fname)[0] + &#34;.ulock&#34;
         self.ulock = FileLock(ulockname)
         self.ulock.waitlock()    #(self.ulockname)
 
         super(TwinChain, self).__init__(fname, pgdebug)
@@ -252,17 +260,17 @@
             decoded = self.packer.decode_data(arr[1])
             #print(&#34;decoded&#34;, decoded)
         except:
             print(&#34;Cannot decode record at&#34;, recnum, recnum, sys.exc_info())
             raise
         dic = self._get_fields(decoded[0])
 
-        if self.core_verbose &gt; 2:
+        if self.chain_verbose &gt; 2:
             print(dic)
-        if self.core_verbose &gt; 0:
+        if self.chain_verbose &gt; 0:
             print(dic[&#39;header&#39;] + &#34; &#34; + dic[&#39;now&#39;], dic[&#39;payload&#39;])
 
         return arr[0].decode(), dic[&#39;payload&#39;]
 
     def get_payoffs_bykey(self, keyval, maxrec = 1):
         &#34; get payload offset by key&#34;
         arr = []
@@ -295,15 +303,15 @@
         rrr = self.getdbsize()
         for aa in range(rrr -1, -1, -1):
             head = self.get_header(aa)
             if head == keyval:
                 ch = self.checkdata(aa)
                 li = self.linkintegrity(aa)
 
-                if self.core_verbose:
+                if self.chain_verbose:
                     print(&#34;li&#34;, li, &#34;ch&#34;, ch)
 
                 if not ch:
                     raise  DBCheckError(&#34;Check failed at rec %a&#34; % aa);
                 if not li:
                     raise  DBLinkError(&#34;Link checl failed at rec %a&#34; % aa);
 
@@ -320,99 +328,99 @@
         if self.pgdebug &gt; 5:
             print(&#34;get_header()&#34;, recnum)
         arr = self.get_rec(recnum)
         if not arr:
             if self.pgdebug &gt; 5:
                 print(&#34;get_header(): empty/deleted record&#34;, recnum)
 
-            if self.core_verbose &gt; 1:
+            if self.chain_verbose &gt; 1:
                 print(&#34;get_header(): empty/deleted record&#34;, recnum)
             return []
 
-        if self.core_verbose &gt; 1:
+        if self.chain_verbose &gt; 1:
             print(&#34;arr&#34;, arr)
             uuu = uuid.UUID(arr[0].decode())
             ddd = str(uuid2date(uuu))
             print(&#34;header&#34;, arr[0])
         return arr[0].decode()
 
     def linkintegrity(self, recnum):
 
         &#39;&#39;&#39; Scan one record an its integrity based on the previous one &#39;&#39;&#39;
 
         if recnum &lt; 1:
-            if self.core_verbose:
+            if self.chain_verbose:
                 print(&#34;Cannot check initial record.&#34;)
             return True
 
-        if self.core_verbose &gt; 4:
+        if self.chain_verbose &gt; 4:
             print(&#34;Checking link ...&#34;, recnum)
 
         arr = self.get_rec(recnum-1)
         try:
             decoded = self.packer.decode_data(arr[1])
         except:
             print(&#34;Cannot decode prev:&#34;, recnum, sys.exc_info())
             return
         dicold = self._get_fields(decoded[0])
         arr2 = self.get_rec(recnum)
         try:
             decoded2 = self.packer.decode_data(arr2[1])
         except:
-            if self.core_verbose &gt; 2:
+            if self.chain_verbose &gt; 2:
                 print(&#34;Cannot decode curr:&#34;, recnum, sys.exc_info())
             return
         dic = self._get_fields(decoded2[0])
         backlink = self._build_backlink(dicold)
         hhh = self._hashtohex(backlink)
-        if self.core_verbose &gt; 2:
+        if self.chain_verbose &gt; 2:
             print(&#34;calc      &#34;, hhh)
             print(&#34;backlink  &#34;, dic[&#39;backlink&#39;])
         return hhh == dic[&#39;backlink&#39;]
 
     def checkdata(self, recnum):
 
         &#39;&#39;&#39; Integrity check of record. &#39;&#39;&#39;
 
         arr = self.get_rec(recnum)
         try:
             decoded = self.packer.decode_data(arr[1])
         except:
-            if self.core_verbose &gt; 2:
+            if self.chain_verbose &gt; 2:
                 print(&#34;Cannot decode:&#34;, recnum, sys.exc_info())
             return
 
         aaa = self._get_fields(decoded[0])
         sumstr = self._build_sumstr(aaa)
         hhh = self._hashtohex(sumstr)
-        if self.core_verbose &gt; 1:
+        if self.chain_verbose &gt; 1:
             print(&#34;data&#34;, hhh)
-        if self.core_verbose &gt; 2:
+        if self.chain_verbose &gt; 2:
             print(&#34;hash&#34;, aaa[&#39;hash256&#39;])
         return hhh == aaa[&#39;hash256&#39;]
 
     def appendwith(self, header, datax):
 
         &#39;&#39;&#39; Append data and header to the end of database &#39;&#39;&#39;
 
         #if type(header) != type(b&#34;&#34;):
         #    header = header.encode() #errors=&#39;strict&#39;)
 
         #if type(datax) != type(b&#34;&#34;):
         #    datax = datax.encode() #errors=&#39;strict&#39;)
 
-        if self.core_verbose &gt; 0:
+        if self.chain_verbose &gt; 0:
             print(&#34;Appendwith&#34;, header, datax)
 
         self.ulock.waitlock()    #self.ulockname)
 
         try:
             uuu = uuid.UUID(header)
         except:
-            if self.core_verbose:
+            if self.chain_verbose:
                 print(&#34;Header override must be a valid UUID string.&#34;)
 
             self.ulock.unlock() #self.ulockname)
             raise ValueError(&#34;Header override must be a valid UUID string.&#34;)
 
         old_dicx = {}
         # Get last data from db
@@ -440,26 +448,26 @@
         encoded = self.packer.encode_data(&#34;&#34;, aaa)
 
         #print(&#34;save&#34;, header, &#34;-&#34;, encoded)
         #print(&#34;bbb&#34;, self.getdbsize())
         self.save_data(header, encoded)
         #print(&#34;eee&#34;, self.getdbsize())
 
-        if self.core_verbose &gt; 1:
+        if self.chain_verbose &gt; 1:
             bbb = self.packer.decode_data(encoded)
             print(&#34;Rec&#34;, bbb[0])
 
         self.ulock.unlock() #self.ulockname)
         return True
 
     def append(self, datax):
 
         &#39;&#39;&#39; Append data to the end of database &#39;&#39;&#39;
 
-        if self.core_verbose &gt; 0:
+        if self.chain_verbose &gt; 0:
             print(&#34;Append&#34;, datax)
 
         # Get last data from db
         #sss = self.getdbsize()
         #if not sss:
         #    #raise ValueError(&#34;Invalid database, must have at least one record.&#34;)
         #    pass
@@ -541,31 +549,31 @@
 <ul class="hlist">
 <li>builtins.Exception</li>
 <li>builtins.BaseException</li>
 </ul>
 </dd>
 <dt id="twinchain.TwinChain"><code class="flex name class">
 <span>class <span class="ident">TwinChain</span></span>
-<span>(</span><span>fname='pydbchain.pydb', pgdebug=0, core_verbose=0)</span>
+<span>(</span><span>fname='pydbchain.pydb', pgdebug=0, verbose=0)</span>
 </code></dt>
 <dd>
 <div class="desc"><p>Derive from database to accomodate block chain.</p></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
 <pre><code class="python">class TwinChain(TwinCore):
 
     &#39;&#39;&#39;
         Derive from database to accomodate block chain.
     &#39;&#39;&#39;
 
-    def __init__(self, fname = &#34;pydbchain.pydb&#34;, pgdebug = 0, core_verbose = 0):
+    def __init__(self, fname = &#34;pydbchain.pydb&#34;, pgdebug = 0, verbose = 0):
 
-        self.core_verbose = core_verbose
+        self.chain_verbose = verbose
 
         # Upper lock name
         ulockname = os.path.splitext(fname)[0] + &#34;.ulock&#34;
         self.ulock = FileLock(ulockname)
         self.ulock.waitlock()    #(self.ulockname)
 
         super(TwinChain, self).__init__(fname, pgdebug)
@@ -693,17 +701,17 @@
             decoded = self.packer.decode_data(arr[1])
             #print(&#34;decoded&#34;, decoded)
         except:
             print(&#34;Cannot decode record at&#34;, recnum, recnum, sys.exc_info())
             raise
         dic = self._get_fields(decoded[0])
 
-        if self.core_verbose &gt; 2:
+        if self.chain_verbose &gt; 2:
             print(dic)
-        if self.core_verbose &gt; 0:
+        if self.chain_verbose &gt; 0:
             print(dic[&#39;header&#39;] + &#34; &#34; + dic[&#39;now&#39;], dic[&#39;payload&#39;])
 
         return arr[0].decode(), dic[&#39;payload&#39;]
 
     def get_payoffs_bykey(self, keyval, maxrec = 1):
         &#34; get payload offset by key&#34;
         arr = []
@@ -736,15 +744,15 @@
         rrr = self.getdbsize()
         for aa in range(rrr -1, -1, -1):
             head = self.get_header(aa)
             if head == keyval:
                 ch = self.checkdata(aa)
                 li = self.linkintegrity(aa)
 
-                if self.core_verbose:
+                if self.chain_verbose:
                     print(&#34;li&#34;, li, &#34;ch&#34;, ch)
 
                 if not ch:
                     raise  DBCheckError(&#34;Check failed at rec %a&#34; % aa);
                 if not li:
                     raise  DBLinkError(&#34;Link checl failed at rec %a&#34; % aa);
 
@@ -761,99 +769,99 @@
         if self.pgdebug &gt; 5:
             print(&#34;get_header()&#34;, recnum)
         arr = self.get_rec(recnum)
         if not arr:
             if self.pgdebug &gt; 5:
                 print(&#34;get_header(): empty/deleted record&#34;, recnum)
 
-            if self.core_verbose &gt; 1:
+            if self.chain_verbose &gt; 1:
                 print(&#34;get_header(): empty/deleted record&#34;, recnum)
             return []
 
-        if self.core_verbose &gt; 1:
+        if self.chain_verbose &gt; 1:
             print(&#34;arr&#34;, arr)
             uuu = uuid.UUID(arr[0].decode())
             ddd = str(uuid2date(uuu))
             print(&#34;header&#34;, arr[0])
         return arr[0].decode()
 
     def linkintegrity(self, recnum):
 
         &#39;&#39;&#39; Scan one record an its integrity based on the previous one &#39;&#39;&#39;
 
         if recnum &lt; 1:
-            if self.core_verbose:
+            if self.chain_verbose:
                 print(&#34;Cannot check initial record.&#34;)
             return True
 
-        if self.core_verbose &gt; 4:
+        if self.chain_verbose &gt; 4:
             print(&#34;Checking link ...&#34;, recnum)
 
         arr = self.get_rec(recnum-1)
         try:
             decoded = self.packer.decode_data(arr[1])
         except:
             print(&#34;Cannot decode prev:&#34;, recnum, sys.exc_info())
             return
         dicold = self._get_fields(decoded[0])
         arr2 = self.get_rec(recnum)
         try:
             decoded2 = self.packer.decode_data(arr2[1])
         except:
-            if self.core_verbose &gt; 2:
+            if self.chain_verbose &gt; 2:
                 print(&#34;Cannot decode curr:&#34;, recnum, sys.exc_info())
             return
         dic = self._get_fields(decoded2[0])
         backlink = self._build_backlink(dicold)
         hhh = self._hashtohex(backlink)
-        if self.core_verbose &gt; 2:
+        if self.chain_verbose &gt; 2:
             print(&#34;calc      &#34;, hhh)
             print(&#34;backlink  &#34;, dic[&#39;backlink&#39;])
         return hhh == dic[&#39;backlink&#39;]
 
     def checkdata(self, recnum):
 
         &#39;&#39;&#39; Integrity check of record. &#39;&#39;&#39;
 
         arr = self.get_rec(recnum)
         try:
             decoded = self.packer.decode_data(arr[1])
         except:
-            if self.core_verbose &gt; 2:
+            if self.chain_verbose &gt; 2:
                 print(&#34;Cannot decode:&#34;, recnum, sys.exc_info())
             return
 
         aaa = self._get_fields(decoded[0])
         sumstr = self._build_sumstr(aaa)
         hhh = self._hashtohex(sumstr)
-        if self.core_verbose &gt; 1:
+        if self.chain_verbose &gt; 1:
             print(&#34;data&#34;, hhh)
-        if self.core_verbose &gt; 2:
+        if self.chain_verbose &gt; 2:
             print(&#34;hash&#34;, aaa[&#39;hash256&#39;])
         return hhh == aaa[&#39;hash256&#39;]
 
     def appendwith(self, header, datax):
 
         &#39;&#39;&#39; Append data and header to the end of database &#39;&#39;&#39;
 
         #if type(header) != type(b&#34;&#34;):
         #    header = header.encode() #errors=&#39;strict&#39;)
 
         #if type(datax) != type(b&#34;&#34;):
         #    datax = datax.encode() #errors=&#39;strict&#39;)
 
-        if self.core_verbose &gt; 0:
+        if self.chain_verbose &gt; 0:
             print(&#34;Appendwith&#34;, header, datax)
 
         self.ulock.waitlock()    #self.ulockname)
 
         try:
             uuu = uuid.UUID(header)
         except:
-            if self.core_verbose:
+            if self.chain_verbose:
                 print(&#34;Header override must be a valid UUID string.&#34;)
 
             self.ulock.unlock() #self.ulockname)
             raise ValueError(&#34;Header override must be a valid UUID string.&#34;)
 
         old_dicx = {}
         # Get last data from db
@@ -881,26 +889,26 @@
         encoded = self.packer.encode_data(&#34;&#34;, aaa)
 
         #print(&#34;save&#34;, header, &#34;-&#34;, encoded)
         #print(&#34;bbb&#34;, self.getdbsize())
         self.save_data(header, encoded)
         #print(&#34;eee&#34;, self.getdbsize())
 
-        if self.core_verbose &gt; 1:
+        if self.chain_verbose &gt; 1:
             bbb = self.packer.decode_data(encoded)
             print(&#34;Rec&#34;, bbb[0])
 
         self.ulock.unlock() #self.ulockname)
         return True
 
     def append(self, datax):
 
         &#39;&#39;&#39; Append data to the end of database &#39;&#39;&#39;
 
-        if self.core_verbose &gt; 0:
+        if self.chain_verbose &gt; 0:
             print(&#34;Append&#34;, datax)
 
         # Get last data from db
         #sss = self.getdbsize()
         #if not sss:
         #    #raise ValueError(&#34;Invalid database, must have at least one record.&#34;)
         #    pass
@@ -946,15 +954,15 @@
 <summary>
 <span>Expand source code</span>
 </summary>
 <pre><code class="python">def append(self, datax):
 
     &#39;&#39;&#39; Append data to the end of database &#39;&#39;&#39;
 
-    if self.core_verbose &gt; 0:
+    if self.chain_verbose &gt; 0:
         print(&#34;Append&#34;, datax)
 
     # Get last data from db
     #sss = self.getdbsize()
     #if not sss:
     #    #raise ValueError(&#34;Invalid database, must have at least one record.&#34;)
     #    pass
@@ -984,23 +992,23 @@
 
     #if type(header) != type(b&#34;&#34;):
     #    header = header.encode() #errors=&#39;strict&#39;)
 
     #if type(datax) != type(b&#34;&#34;):
     #    datax = datax.encode() #errors=&#39;strict&#39;)
 
-    if self.core_verbose &gt; 0:
+    if self.chain_verbose &gt; 0:
         print(&#34;Appendwith&#34;, header, datax)
 
     self.ulock.waitlock()    #self.ulockname)
 
     try:
         uuu = uuid.UUID(header)
     except:
-        if self.core_verbose:
+        if self.chain_verbose:
             print(&#34;Header override must be a valid UUID string.&#34;)
 
         self.ulock.unlock() #self.ulockname)
         raise ValueError(&#34;Header override must be a valid UUID string.&#34;)
 
     old_dicx = {}
     # Get last data from db
@@ -1028,15 +1036,15 @@
     encoded = self.packer.encode_data(&#34;&#34;, aaa)
 
     #print(&#34;save&#34;, header, &#34;-&#34;, encoded)
     #print(&#34;bbb&#34;, self.getdbsize())
     self.save_data(header, encoded)
     #print(&#34;eee&#34;, self.getdbsize())
 
-    if self.core_verbose &gt; 1:
+    if self.chain_verbose &gt; 1:
         bbb = self.packer.decode_data(encoded)
         print(&#34;Rec&#34;, bbb[0])
 
     self.ulock.unlock() #self.ulockname)
     return True</code></pre>
 </details>
 </dd>
@@ -1053,24 +1061,24 @@
 
     &#39;&#39;&#39; Integrity check of record. &#39;&#39;&#39;
 
     arr = self.get_rec(recnum)
     try:
         decoded = self.packer.decode_data(arr[1])
     except:
-        if self.core_verbose &gt; 2:
+        if self.chain_verbose &gt; 2:
             print(&#34;Cannot decode:&#34;, recnum, sys.exc_info())
         return
 
     aaa = self._get_fields(decoded[0])
     sumstr = self._build_sumstr(aaa)
     hhh = self._hashtohex(sumstr)
-    if self.core_verbose &gt; 1:
+    if self.chain_verbose &gt; 1:
         print(&#34;data&#34;, hhh)
-    if self.core_verbose &gt; 2:
+    if self.chain_verbose &gt; 2:
         print(&#34;hash&#34;, aaa[&#39;hash256&#39;])
     return hhh == aaa[&#39;hash256&#39;]</code></pre>
 </details>
 </dd>
 <dt id="twinchain.TwinChain.dump_rec"><code class="name flex">
 <span>def <span class="ident">dump_rec</span></span>(<span>self, bbb)</span>
 </code></dt>
@@ -1130,15 +1138,15 @@
     rrr = self.getdbsize()
     for aa in range(rrr -1, -1, -1):
         head = self.get_header(aa)
         if head == keyval:
             ch = self.checkdata(aa)
             li = self.linkintegrity(aa)
 
-            if self.core_verbose:
+            if self.chain_verbose:
                 print(&#34;li&#34;, li, &#34;ch&#34;, ch)
 
             if not ch:
                 raise  DBCheckError(&#34;Check failed at rec %a&#34; % aa);
             if not li:
                 raise  DBLinkError(&#34;Link checl failed at rec %a&#34; % aa);
 
@@ -1165,19 +1173,19 @@
     if self.pgdebug &gt; 5:
         print(&#34;get_header()&#34;, recnum)
     arr = self.get_rec(recnum)
     if not arr:
         if self.pgdebug &gt; 5:
             print(&#34;get_header(): empty/deleted record&#34;, recnum)
 
-        if self.core_verbose &gt; 1:
+        if self.chain_verbose &gt; 1:
             print(&#34;get_header(): empty/deleted record&#34;, recnum)
         return []
 
-    if self.core_verbose &gt; 1:
+    if self.chain_verbose &gt; 1:
         print(&#34;arr&#34;, arr)
         uuu = uuid.UUID(arr[0].decode())
         ddd = str(uuid2date(uuu))
         print(&#34;header&#34;, arr[0])
     return arr[0].decode()</code></pre>
 </details>
 </dd>
@@ -1201,17 +1209,17 @@
         decoded = self.packer.decode_data(arr[1])
         #print(&#34;decoded&#34;, decoded)
     except:
         print(&#34;Cannot decode record at&#34;, recnum, recnum, sys.exc_info())
         raise
     dic = self._get_fields(decoded[0])
 
-    if self.core_verbose &gt; 2:
+    if self.chain_verbose &gt; 2:
         print(dic)
-    if self.core_verbose &gt; 0:
+    if self.chain_verbose &gt; 0:
         print(dic[&#39;header&#39;] + &#34; &#34; + dic[&#39;now&#39;], dic[&#39;payload&#39;])
 
     return arr[0].decode(), dic[&#39;payload&#39;]</code></pre>
 </details>
 </dd>
 <dt id="twinchain.TwinChain.get_payoffs_bykey"><code class="name flex">
 <span>def <span class="ident">get_payoffs_bykey</span></span>(<span>self, keyval, maxrec=1)</span>
@@ -1245,55 +1253,53 @@
 <span>Expand source code</span>
 </summary>
 <pre><code class="python">def linkintegrity(self, recnum):
 
     &#39;&#39;&#39; Scan one record an its integrity based on the previous one &#39;&#39;&#39;
 
     if recnum &lt; 1:
-        if self.core_verbose:
+        if self.chain_verbose:
             print(&#34;Cannot check initial record.&#34;)
         return True
 
-    if self.core_verbose &gt; 4:
+    if self.chain_verbose &gt; 4:
         print(&#34;Checking link ...&#34;, recnum)
 
     arr = self.get_rec(recnum-1)
     try:
         decoded = self.packer.decode_data(arr[1])
     except:
         print(&#34;Cannot decode prev:&#34;, recnum, sys.exc_info())
         return
     dicold = self._get_fields(decoded[0])
     arr2 = self.get_rec(recnum)
     try:
         decoded2 = self.packer.decode_data(arr2[1])
     except:
-        if self.core_verbose &gt; 2:
+        if self.chain_verbose &gt; 2:
             print(&#34;Cannot decode curr:&#34;, recnum, sys.exc_info())
         return
     dic = self._get_fields(decoded2[0])
     backlink = self._build_backlink(dicold)
     hhh = self._hashtohex(backlink)
-    if self.core_verbose &gt; 2:
+    if self.chain_verbose &gt; 2:
         print(&#34;calc      &#34;, hhh)
         print(&#34;backlink  &#34;, dic[&#39;backlink&#39;])
     return hhh == dic[&#39;backlink&#39;]</code></pre>
 </details>
 </dd>
 </dl>
 </dd>
 </dl>
 </section>
 </article>
 <nav id="sidebar">
 <h1>Index</h1>
 <div class="toc">
-<ul>
-<li><a href="#twinchain">Twinchain</a></li>
-</ul>
+<ul></ul>
 </div>
 <ul id="index">
 <li><h3><a href="#header-classes">Classes</a></h3>
 <ul>
 <li>
 <h4><code><a title="twinchain.DBCheckError" href="#twinchain.DBCheckError">DBCheckError</a></code></h4>
 </li>
```

#### html2text {}

```diff
@@ -1,61 +1,69 @@
 ************ MMoodduullee ttwwiinncchhaaiinn ************
-! @mainpage
-************ TTwwiinncchhaaiinn ************
+
 Block chain layer on top of twincore.
 
-    prev     curr
-        record
-|   Time Now    |   Time  Now    |  Time Now     |
-|   hash256   | |    hash256   | |   hash256   | |
-|   Header    | |    Header    | |   Header    | |
-|   Payload   | |    Payload   | |   Payload   | |
-|   Backlink  | |    Backlink  | |   Backlink  | |
-              |----->---|      |---->---|     |------ ...
+   |   Time Now    |   Time  Now    |  Time Now     |
+   |   hash256   | |    hash256   | |   hash256   | |
+   |   Header    | |    Header    | |   Header    | |
+   |   Payload   | |    Payload   | |   Payload   | |
+   |   Backlink  | |    Backlink  | |   Backlink  | |
+                 |----->---|      |---->---|     |------
+
+   The sum of fields saved to the next backlink.
+
+   History:
+
+   1.1         Tue 20.Feb.2024     Initial release
+   1.2.0       Mon 26.Feb.2024     Moved pip home to pydbase/
+   1.4.0       Tue 27.Feb.2024     Addedd pgdebug
+   1.4.2       Wed 28.Feb.2024     Fixed multiple instances
+   1.4.3       Wed 28.Feb.2024     ChainAdm added
+   1.4.4       Fri 01.Mar.2024     Tests for chain functions
+   1.4.5       Fri 01.Mar.2024     Misc fixes
+   1.4.6       Mon 04.Mar.2024     Vacuum count on vacuumed records
+   1.4.7       Tue 05.Mar.2024     In place record update
+   1.4.8       Sat 09.Mar.2024     Added new locking mechanism
+   1.4.9       Mon 01.Apr.2024     Updated to run on MSYS2, new locking
+   1.5.0       Tue 02.Apr.2024     Cleaned, pip upload
+   1.5.1       Wed 10.Apr.2024     Dangling lock .. fixed
+Expand source code
+#!/usr/bin/env python3
+
+'''
+    <pre>
+
+ Block chain layer on top of twincore.
+
+    |   Time Now    |   Time  Now    |  Time Now     |
+    |   hash256   | |    hash256   | |   hash256   | |
+    |   Header    | |    Header    | |   Header    | |
+    |   Payload   | |    Payload   | |   Payload   | |
+    |   Backlink  | |    Backlink  | |   Backlink  | |
+                  |----->---|      |---->---|     |------
 
-The sum of fields saved to the next backlink.
+    The sum of fields saved to the next backlink.
 
-History:
+    History:
 
-    0.0.0       Tue 20.Feb.2024     Initial release
-    0.0.0       Sun 26.Mar.2023     More features
+    1.1         Tue 20.Feb.2024     Initial release
     1.2.0       Mon 26.Feb.2024     Moved pip home to pydbase/
     1.4.0       Tue 27.Feb.2024     Addedd pgdebug
     1.4.2       Wed 28.Feb.2024     Fixed multiple instances
     1.4.3       Wed 28.Feb.2024     ChainAdm added
-Expand source code
-#!/usr/bin/env python3
-
-'''!
-    @mainpage
-
-    # Twinchain
-
-        Block chain layer on top of twincore.
-
-            prev     curr
-                record
-        |   Time Now    |   Time  Now    |  Time Now     |
-        |   hash256   | |    hash256   | |   hash256   | |
-        |   Header    | |    Header    | |   Header    | |
-        |   Payload   | |    Payload   | |   Payload   | |
-        |   Backlink  | |    Backlink  | |   Backlink  | |
-                      |----->---|      |---->---|     |------ ...
-
-        The sum of fields saved to the next backlink.
-
-        History:
-
-            0.0.0       Tue 20.Feb.2024     Initial release
-            0.0.0       Sun 26.Mar.2023     More features
-            1.2.0       Mon 26.Feb.2024     Moved pip home to pydbase/
-            1.4.0       Tue 27.Feb.2024     Addedd pgdebug
-            1.4.2       Wed 28.Feb.2024     Fixed multiple instances
-            1.4.3       Wed 28.Feb.2024     ChainAdm added
+    1.4.4       Fri 01.Mar.2024     Tests for chain functions
+    1.4.5       Fri 01.Mar.2024     Misc fixes
+    1.4.6       Mon 04.Mar.2024     Vacuum count on vacuumed records
+    1.4.7       Tue 05.Mar.2024     In place record update
+    1.4.8       Sat 09.Mar.2024     Added new locking mechanism
+    1.4.9       Mon 01.Apr.2024     Updated to run on MSYS2, new locking
+    1.5.0       Tue 02.Apr.2024     Cleaned, pip upload
+    1.5.1       Wed 10.Apr.2024     Dangling lock .. fixed
 
+    </pre>
 '''
 
 import  os, sys, getopt, signal, select, socket, time, struct
 import  random, stat, os.path, datetime, threading, uuid
 import  struct, io, hashlib
 
 import pyvpacker
@@ -85,18 +93,17 @@
 
 class TwinChain(TwinCore):
 
     '''
         Derive from database to accomodate block chain.
     '''
 
-    def __init__(self, fname = "pydbchain.pydb", pgdebug = 0, core_verbose =
-0):
+    def __init__(self, fname = "pydbchain.pydb", pgdebug = 0, verbose = 0):
 
-        self.core_verbose = core_verbose
+        self.chain_verbose = verbose
 
         # Upper lock name
         ulockname = os.path.splitext(fname)[0] + ".ulock"
         self.ulock = FileLock(ulockname)
         self.ulock.waitlock()    #(self.ulockname)
 
         super(TwinChain, self).__init__(fname, pgdebug)
@@ -224,17 +231,17 @@
             decoded = self.packer.decode_data(arr[1])
             #print("decoded", decoded)
         except:
             print("Cannot decode record at", recnum, recnum, sys.exc_info())
             raise
         dic = self._get_fields(decoded[0])
 
-        if self.core_verbose > 2:
+        if self.chain_verbose > 2:
             print(dic)
-        if self.core_verbose > 0:
+        if self.chain_verbose > 0:
             print(dic['header'] + " " + dic['now'], dic['payload'])
 
         return arr[0].decode(), dic['payload']
 
     def get_payoffs_bykey(self, keyval, maxrec = 1):
         " get payload offset by key"
         arr = []
@@ -268,15 +275,15 @@
         rrr = self.getdbsize()
         for aa in range(rrr -1, -1, -1):
             head = self.get_header(aa)
             if head == keyval:
                 ch = self.checkdata(aa)
                 li = self.linkintegrity(aa)
 
-                if self.core_verbose:
+                if self.chain_verbose:
                     print("li", li, "ch", ch)
 
                 if not ch:
                     raise  DBCheckError("Check failed at rec %a" % aa);
                 if not li:
                     raise  DBLinkError("Link checl failed at rec %a" % aa);
 
@@ -293,99 +300,99 @@
         if self.pgdebug > 5:
             print("get_header()", recnum)
         arr = self.get_rec(recnum)
         if not arr:
             if self.pgdebug > 5:
                 print("get_header(): empty/deleted record", recnum)
 
-            if self.core_verbose > 1:
+            if self.chain_verbose > 1:
                 print("get_header(): empty/deleted record", recnum)
             return []
 
-        if self.core_verbose > 1:
+        if self.chain_verbose > 1:
             print("arr", arr)
             uuu = uuid.UUID(arr[0].decode())
             ddd = str(uuid2date(uuu))
             print("header", arr[0])
         return arr[0].decode()
 
     def linkintegrity(self, recnum):
 
         ''' Scan one record an its integrity based on the previous one '''
 
         if recnum < 1:
-            if self.core_verbose:
+            if self.chain_verbose:
                 print("Cannot check initial record.")
             return True
 
-        if self.core_verbose > 4:
+        if self.chain_verbose > 4:
             print("Checking link ...", recnum)
 
         arr = self.get_rec(recnum-1)
         try:
             decoded = self.packer.decode_data(arr[1])
         except:
             print("Cannot decode prev:", recnum, sys.exc_info())
             return
         dicold = self._get_fields(decoded[0])
         arr2 = self.get_rec(recnum)
         try:
             decoded2 = self.packer.decode_data(arr2[1])
         except:
-            if self.core_verbose > 2:
+            if self.chain_verbose > 2:
                 print("Cannot decode curr:", recnum, sys.exc_info())
             return
         dic = self._get_fields(decoded2[0])
         backlink = self._build_backlink(dicold)
         hhh = self._hashtohex(backlink)
-        if self.core_verbose > 2:
+        if self.chain_verbose > 2:
             print("calc      ", hhh)
             print("backlink  ", dic['backlink'])
         return hhh == dic['backlink']
 
     def checkdata(self, recnum):
 
         ''' Integrity check of record. '''
 
         arr = self.get_rec(recnum)
         try:
             decoded = self.packer.decode_data(arr[1])
         except:
-            if self.core_verbose > 2:
+            if self.chain_verbose > 2:
                 print("Cannot decode:", recnum, sys.exc_info())
             return
 
         aaa = self._get_fields(decoded[0])
         sumstr = self._build_sumstr(aaa)
         hhh = self._hashtohex(sumstr)
-        if self.core_verbose > 1:
+        if self.chain_verbose > 1:
             print("data", hhh)
-        if self.core_verbose > 2:
+        if self.chain_verbose > 2:
             print("hash", aaa['hash256'])
         return hhh == aaa['hash256']
 
     def appendwith(self, header, datax):
 
         ''' Append data and header to the end of database '''
 
         #if type(header) != type(b""):
         #    header = header.encode() #errors='strict')
 
         #if type(datax) != type(b""):
         #    datax = datax.encode() #errors='strict')
 
-        if self.core_verbose > 0:
+        if self.chain_verbose > 0:
             print("Appendwith", header, datax)
 
         self.ulock.waitlock()    #self.ulockname)
 
         try:
             uuu = uuid.UUID(header)
         except:
-            if self.core_verbose:
+            if self.chain_verbose:
                 print("Header override must be a valid UUID string.")
 
             self.ulock.unlock() #self.ulockname)
             raise ValueError("Header override must be a valid UUID string.")
 
         old_dicx = {}
         # Get last data from db
@@ -414,26 +421,26 @@
         encoded = self.packer.encode_data("", aaa)
 
         #print("save", header, "-", encoded)
         #print("bbb", self.getdbsize())
         self.save_data(header, encoded)
         #print("eee", self.getdbsize())
 
-        if self.core_verbose > 1:
+        if self.chain_verbose > 1:
             bbb = self.packer.decode_data(encoded)
             print("Rec", bbb[0])
 
         self.ulock.unlock() #self.ulockname)
         return True
 
     def append(self, datax):
 
         ''' Append data to the end of database '''
 
-        if self.core_verbose > 0:
+        if self.chain_verbose > 0:
             print("Append", datax)
 
         # Get last data from db
         #sss = self.getdbsize()
         #if not sss:
         #    #raise ValueError("Invalid database, must have at least one
 record.")
@@ -482,27 +489,27 @@
       class DBLinkError(Exception):
 
           def __init__(self, message):
                self.message = message
       ******** AAnncceessttoorrss ********
           * builtins.Exception
           * builtins.BaseException
-  class TwinChain (fname='pydbchain.pydb', pgdebug=0, core_verbose=0)
+  class TwinChain (fname='pydbchain.pydb', pgdebug=0, verbose=0)
       Derive from database to accomodate block chain.
       Expand source code
       class TwinChain(TwinCore):
 
           '''
               Derive from database to accomodate block chain.
           '''
 
-          def __init__(self, fname = "pydbchain.pydb", pgdebug = 0,
-      core_verbose = 0):
+          def __init__(self, fname = "pydbchain.pydb", pgdebug = 0, verbose =
+      0):
 
-              self.core_verbose = core_verbose
+              self.chain_verbose = verbose
 
               # Upper lock name
               ulockname = os.path.splitext(fname)[0] + ".ulock"
               self.ulock = FileLock(ulockname)
               self.ulock.waitlock()    #(self.ulockname)
 
               super(TwinChain, self).__init__(fname, pgdebug)
@@ -633,17 +640,17 @@
                   #print("decoded", decoded)
               except:
                   print("Cannot decode record at", recnum, recnum, sys.exc_info
       ())
                   raise
               dic = self._get_fields(decoded[0])
 
-              if self.core_verbose > 2:
+              if self.chain_verbose > 2:
                   print(dic)
-              if self.core_verbose > 0:
+              if self.chain_verbose > 0:
                   print(dic['header'] + " " + dic['now'], dic['payload'])
 
               return arr[0].decode(), dic['payload']
 
           def get_payoffs_bykey(self, keyval, maxrec = 1):
               " get payload offset by key"
               arr = []
@@ -677,15 +684,15 @@
               rrr = self.getdbsize()
               for aa in range(rrr -1, -1, -1):
                   head = self.get_header(aa)
                   if head == keyval:
                       ch = self.checkdata(aa)
                       li = self.linkintegrity(aa)
 
-                      if self.core_verbose:
+                      if self.chain_verbose:
                           print("li", li, "ch", ch)
 
                       if not ch:
                           raise  DBCheckError("Check failed at rec %a" % aa);
                       if not li:
                           raise  DBLinkError("Link checl failed at rec %a" %
       aa);
@@ -703,100 +710,100 @@
               if self.pgdebug > 5:
                   print("get_header()", recnum)
               arr = self.get_rec(recnum)
               if not arr:
                   if self.pgdebug > 5:
                       print("get_header(): empty/deleted record", recnum)
 
-                  if self.core_verbose > 1:
+                  if self.chain_verbose > 1:
                       print("get_header(): empty/deleted record", recnum)
                   return []
 
-              if self.core_verbose > 1:
+              if self.chain_verbose > 1:
                   print("arr", arr)
                   uuu = uuid.UUID(arr[0].decode())
                   ddd = str(uuid2date(uuu))
                   print("header", arr[0])
               return arr[0].decode()
 
           def linkintegrity(self, recnum):
 
               ''' Scan one record an its integrity based on the previous one
       '''
 
               if recnum < 1:
-                  if self.core_verbose:
+                  if self.chain_verbose:
                       print("Cannot check initial record.")
                   return True
 
-              if self.core_verbose > 4:
+              if self.chain_verbose > 4:
                   print("Checking link ...", recnum)
 
               arr = self.get_rec(recnum-1)
               try:
                   decoded = self.packer.decode_data(arr[1])
               except:
                   print("Cannot decode prev:", recnum, sys.exc_info())
                   return
               dicold = self._get_fields(decoded[0])
               arr2 = self.get_rec(recnum)
               try:
                   decoded2 = self.packer.decode_data(arr2[1])
               except:
-                  if self.core_verbose > 2:
+                  if self.chain_verbose > 2:
                       print("Cannot decode curr:", recnum, sys.exc_info())
                   return
               dic = self._get_fields(decoded2[0])
               backlink = self._build_backlink(dicold)
               hhh = self._hashtohex(backlink)
-              if self.core_verbose > 2:
+              if self.chain_verbose > 2:
                   print("calc      ", hhh)
                   print("backlink  ", dic['backlink'])
               return hhh == dic['backlink']
 
           def checkdata(self, recnum):
 
               ''' Integrity check of record. '''
 
               arr = self.get_rec(recnum)
               try:
                   decoded = self.packer.decode_data(arr[1])
               except:
-                  if self.core_verbose > 2:
+                  if self.chain_verbose > 2:
                       print("Cannot decode:", recnum, sys.exc_info())
                   return
 
               aaa = self._get_fields(decoded[0])
               sumstr = self._build_sumstr(aaa)
               hhh = self._hashtohex(sumstr)
-              if self.core_verbose > 1:
+              if self.chain_verbose > 1:
                   print("data", hhh)
-              if self.core_verbose > 2:
+              if self.chain_verbose > 2:
                   print("hash", aaa['hash256'])
               return hhh == aaa['hash256']
 
           def appendwith(self, header, datax):
 
               ''' Append data and header to the end of database '''
 
               #if type(header) != type(b""):
               #    header = header.encode() #errors='strict')
 
               #if type(datax) != type(b""):
               #    datax = datax.encode() #errors='strict')
 
-              if self.core_verbose > 0:
+              if self.chain_verbose > 0:
                   print("Appendwith", header, datax)
 
               self.ulock.waitlock()    #self.ulockname)
 
               try:
                   uuu = uuid.UUID(header)
               except:
-                  if self.core_verbose:
+                  if self.chain_verbose:
                       print("Header override must be a valid UUID string.")
 
                   self.ulock.unlock() #self.ulockname)
                   raise ValueError("Header override must be a valid UUID
       string.")
 
               old_dicx = {}
@@ -827,26 +834,26 @@
               encoded = self.packer.encode_data("", aaa)
 
               #print("save", header, "-", encoded)
               #print("bbb", self.getdbsize())
               self.save_data(header, encoded)
               #print("eee", self.getdbsize())
 
-              if self.core_verbose > 1:
+              if self.chain_verbose > 1:
                   bbb = self.packer.decode_data(encoded)
                   print("Rec", bbb[0])
 
               self.ulock.unlock() #self.ulockname)
               return True
 
           def append(self, datax):
 
               ''' Append data to the end of database '''
 
-              if self.core_verbose > 0:
+              if self.chain_verbose > 0:
                   print("Append", datax)
 
               # Get last data from db
               #sss = self.getdbsize()
               #if not sss:
               #    #raise ValueError("Invalid database, must have at least one
       record.")
@@ -883,15 +890,15 @@
         def append(self, datax)
             Append data to the end of database
             Expand source code
             def append(self, datax):
 
                 ''' Append data to the end of database '''
 
-                if self.core_verbose > 0:
+                if self.chain_verbose > 0:
                     print("Append", datax)
 
                 # Get last data from db
                 #sss = self.getdbsize()
                 #if not sss:
                 #    #raise ValueError("Invalid database, must have at least
             one record.")
@@ -914,23 +921,23 @@
 
                 #if type(header) != type(b""):
                 #    header = header.encode() #errors='strict')
 
                 #if type(datax) != type(b""):
                 #    datax = datax.encode() #errors='strict')
 
-                if self.core_verbose > 0:
+                if self.chain_verbose > 0:
                     print("Appendwith", header, datax)
 
                 self.ulock.waitlock()    #self.ulockname)
 
                 try:
                     uuu = uuid.UUID(header)
                 except:
-                    if self.core_verbose:
+                    if self.chain_verbose:
                         print("Header override must be a valid UUID string.")
 
                     self.ulock.unlock() #self.ulockname)
                     raise ValueError("Header override must be a valid UUID
             string.")
 
                 old_dicx = {}
@@ -961,15 +968,15 @@
                 encoded = self.packer.encode_data("", aaa)
 
                 #print("save", header, "-", encoded)
                 #print("bbb", self.getdbsize())
                 self.save_data(header, encoded)
                 #print("eee", self.getdbsize())
 
-                if self.core_verbose > 1:
+                if self.chain_verbose > 1:
                     bbb = self.packer.decode_data(encoded)
                     print("Rec", bbb[0])
 
                 self.ulock.unlock() #self.ulockname)
                 return True
         def checkdata(self, recnum)
             Integrity check of record.
@@ -978,24 +985,24 @@
 
                 ''' Integrity check of record. '''
 
                 arr = self.get_rec(recnum)
                 try:
                     decoded = self.packer.decode_data(arr[1])
                 except:
-                    if self.core_verbose > 2:
+                    if self.chain_verbose > 2:
                         print("Cannot decode:", recnum, sys.exc_info())
                     return
 
                 aaa = self._get_fields(decoded[0])
                 sumstr = self._build_sumstr(aaa)
                 hhh = self._hashtohex(sumstr)
-                if self.core_verbose > 1:
+                if self.chain_verbose > 1:
                     print("data", hhh)
-                if self.core_verbose > 2:
+                if self.chain_verbose > 2:
                     print("hash", aaa['hash256'])
                 return hhh == aaa['hash256']
         def dump_rec(self, bbb)
             Dump one record to console
             Expand source code
             def dump_rec(self, bbb):
 
@@ -1033,15 +1040,15 @@
                 rrr = self.getdbsize()
                 for aa in range(rrr -1, -1, -1):
                     head = self.get_header(aa)
                     if head == keyval:
                         ch = self.checkdata(aa)
                         li = self.linkintegrity(aa)
 
-                        if self.core_verbose:
+                        if self.chain_verbose:
                             print("li", li, "ch", ch)
 
                         if not ch:
                             raise  DBCheckError("Check failed at rec %a" % aa);
                         if not li:
                             raise  DBLinkError("Link checl failed at rec %a" %
             aa);
@@ -1061,19 +1068,19 @@
                 if self.pgdebug > 5:
                     print("get_header()", recnum)
                 arr = self.get_rec(recnum)
                 if not arr:
                     if self.pgdebug > 5:
                         print("get_header(): empty/deleted record", recnum)
 
-                    if self.core_verbose > 1:
+                    if self.chain_verbose > 1:
                         print("get_header(): empty/deleted record", recnum)
                     return []
 
-                if self.core_verbose > 1:
+                if self.chain_verbose > 1:
                     print("arr", arr)
                     uuu = uuid.UUID(arr[0].decode())
                     ddd = str(uuid2date(uuu))
                     print("header", arr[0])
                 return arr[0].decode()
         def get_payload(self, recnum)
             Return the payload on record number
@@ -1090,17 +1097,17 @@
                     #print("decoded", decoded)
                 except:
                     print("Cannot decode record at", recnum, recnum,
             sys.exc_info())
                     raise
                 dic = self._get_fields(decoded[0])
 
-                if self.core_verbose > 2:
+                if self.chain_verbose > 2:
                     print(dic)
-                if self.core_verbose > 0:
+                if self.chain_verbose > 0:
                     print(dic['header'] + " " + dic['now'], dic['payload'])
 
                 return arr[0].decode(), dic['payload']
         def get_payoffs_bykey(self, keyval, maxrec=1)
             get payload offset by key
             Expand source code
             def get_payoffs_bykey(self, keyval, maxrec = 1):
@@ -1119,44 +1126,43 @@
             Expand source code
             def linkintegrity(self, recnum):
 
                 ''' Scan one record an its integrity based on the previous one
             '''
 
                 if recnum < 1:
-                    if self.core_verbose:
+                    if self.chain_verbose:
                         print("Cannot check initial record.")
                     return True
 
-                if self.core_verbose > 4:
+                if self.chain_verbose > 4:
                     print("Checking link ...", recnum)
 
                 arr = self.get_rec(recnum-1)
                 try:
                     decoded = self.packer.decode_data(arr[1])
                 except:
                     print("Cannot decode prev:", recnum, sys.exc_info())
                     return
                 dicold = self._get_fields(decoded[0])
                 arr2 = self.get_rec(recnum)
                 try:
                     decoded2 = self.packer.decode_data(arr2[1])
                 except:
-                    if self.core_verbose > 2:
+                    if self.chain_verbose > 2:
                         print("Cannot decode curr:", recnum, sys.exc_info())
                     return
                 dic = self._get_fields(decoded2[0])
                 backlink = self._build_backlink(dicold)
                 hhh = self._hashtohex(backlink)
-                if self.core_verbose > 2:
+                if self.chain_verbose > 2:
                     print("calc      ", hhh)
                     print("backlink  ", dic['backlink'])
                 return hhh == dic['backlink']
 ************ IInnddeexx ************
-    * _T_w_i_n_c_h_a_i_n
     * ******** _CC_ll_aa_ss_ss_ee_ss ********
           o ****** _DD_BB_CC_hh_ee_cc_kk_EE_rr_rr_oo_rr ******
           o ****** _DD_BB_LL_ii_nn_kk_EE_rr_rr_oo_rr ******
           o ****** _TT_ww_ii_nn_CC_hh_aa_ii_nn ******
                 # _a_p_p_e_n_d
                 # _a_p_p_e_n_d_w_i_t_h
                 # _c_h_e_c_k_d_a_t_a
```

### Comparing `pydbase-1.5.2/pydbase/docs/twincore.html` & `pydbase-1.7.1/pydbase/docs/twincore.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!doctype html>
 <html lang="en">
 <head>
 <meta charset="utf-8">
 <meta name="viewport" content="width=device-width, initial-scale=1, minimum-scale=1" />
 <meta name="generator" content="pdoc 0.10.0" />
 <title>twincore API documentation</title>
-<meta name="description" content="!
-@mainpage …" />
+<meta name="description" content="&lt;pre&gt;
+Database with two files. One for data, one for index; …" />
 <link rel="preload stylesheet" as="style" href="https://cdnjs.cloudflare.com/ajax/libs/10up-sanitize.css/11.0.1/sanitize.min.css" integrity="sha256-PK9q560IAAa6WVRRh76LtCaI8pjTJ2z11v0miyNNjrs=" crossorigin>
 <link rel="preload stylesheet" as="style" href="https://cdnjs.cloudflare.com/ajax/libs/10up-sanitize.css/11.0.1/typography.min.css" integrity="sha256-7l/o7C8jubJiy74VsKTidCy1yBkRtiUGbVkYBylBqUg=" crossorigin>
 <link rel="stylesheet preload" as="style" href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.1.1/styles/github.min.css" crossorigin>
 <style>:root{--highlight-color:#fe9}.flex{display:flex !important}body{line-height:1.5em}#content{padding:20px}#sidebar{padding:30px;overflow:hidden}#sidebar > *:last-child{margin-bottom:2cm}.http-server-breadcrumbs{font-size:130%;margin:0 0 15px 0}#footer{font-size:.75em;padding:5px 30px;border-top:1px solid #ddd;text-align:right}#footer p{margin:0 0 0 1em;display:inline-block}#footer p:last-child{margin-right:30px}h1,h2,h3,h4,h5{font-weight:300}h1{font-size:2.5em;line-height:1.1em}h2{font-size:1.75em;margin:1em 0 .50em 0}h3{font-size:1.4em;margin:25px 0 10px 0}h4{margin:0;font-size:105%}h1:target,h2:target,h3:target,h4:target,h5:target,h6:target{background:var(--highlight-color);padding:.2em 0}a{color:#058;text-decoration:none;transition:color .3s ease-in-out}a:hover{color:#e82}.title code{font-weight:bold}h2[id^="header-"]{margin-top:2em}.ident{color:#900}pre code{background:#f8f8f8;font-size:.8em;line-height:1.4em}code{background:#f2f2f1;padding:1px 4px;overflow-wrap:break-word}h1 code{background:transparent}pre{background:#f8f8f8;border:0;border-top:1px solid #ccc;border-bottom:1px solid #ccc;margin:1em 0;padding:1ex}#http-server-module-list{display:flex;flex-flow:column}#http-server-module-list div{display:flex}#http-server-module-list dt{min-width:10%}#http-server-module-list p{margin-top:0}.toc ul,#index{list-style-type:none;margin:0;padding:0}#index code{background:transparent}#index h3{border-bottom:1px solid #ddd}#index ul{padding:0}#index h4{margin-top:.6em;font-weight:bold}@media (min-width:200ex){#index .two-column{column-count:2}}@media (min-width:300ex){#index .two-column{column-count:3}}dl{margin-bottom:2em}dl dl:last-child{margin-bottom:4em}dd{margin:0 0 1em 3em}#header-classes + dl > dd{margin-bottom:3em}dd dd{margin-left:2em}dd p{margin:10px 0}.name{background:#eee;font-weight:bold;font-size:.85em;padding:5px 10px;display:inline-block;min-width:40%}.name:hover{background:#e0e0e0}dt:target .name{background:var(--highlight-color)}.name > span:first-child{white-space:nowrap}.name.class > span:nth-child(2){margin-left:.4em}.inherited{color:#999;border-left:5px solid #eee;padding-left:1em}.inheritance em{font-style:normal;font-weight:bold}.desc h2{font-weight:400;font-size:1.25em}.desc h3{font-size:1em}.desc dt code{background:inherit}.source summary,.git-link-div{color:#666;text-align:right;font-weight:400;font-size:.8em;text-transform:uppercase}.source summary > *{white-space:nowrap;cursor:pointer}.git-link{color:inherit;margin-left:1em}.source pre{max-height:500px;overflow:auto;margin:0}.source pre code{font-size:12px;overflow:visible}.hlist{list-style:none}.hlist li{display:inline}.hlist li:after{content:',\2002'}.hlist li:last-child:after{content:none}.hlist .hlist{display:inline;padding-left:1em}img{max-width:100%}td{padding:0 .5em}.admonition{padding:.1em .5em;margin-bottom:1em}.admonition-title{font-weight:bold}.admonition.note,.admonition.info,.admonition.important{background:#aef}.admonition.todo,.admonition.versionadded,.admonition.tip,.admonition.hint{background:#dfd}.admonition.warning,.admonition.versionchanged,.admonition.deprecated{background:#fd4}.admonition.error,.admonition.danger,.admonition.caution{background:lightpink}</style>
 <style media="screen and (min-width: 700px)">@media screen and (min-width:700px){#sidebar{width:30%;height:100vh;overflow:auto;position:sticky;top:0}#content{width:70%;max-width:100ch;padding:3em 4em;border-left:1px solid #ddd}pre code{font-size:1em}.item .name{font-size:1em}main{display:flex;flex-direction:row-reverse;justify-content:flex-end}.toc ul ul,#index ul{padding-left:1.5em}.toc > ul > li{margin-top:.5em}}</style>
 <style media="print">@media print{#sidebar h1{page-break-before:always}.source{display:none}}@media print{*{background:transparent !important;color:#000 !important;box-shadow:none !important;text-shadow:none !important}a[href]:after{content:" (" attr(href) ")";font-size:90%}a[href][title]:after{content:none}abbr[title]:after{content:" (" attr(title) ")"}.ir a:after,a[href^="javascript:"]:after,a[href^="#"]:after{content:""}pre,blockquote{border:1px solid #999;page-break-inside:avoid}thead{display:table-header-group}tr,img{page-break-inside:avoid}img{max-width:100% !important}@page{margin:0.5cm}p,h2,h3{orphans:3;widows:3}h1,h2,h3,h4,h5,h6{page-break-after:avoid}}</style>
 <script defer src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.1.1/highlight.min.js" integrity="sha256-Uv3H6lx7dJmRfRvH8TH6kJD1TSK1aFcwgx+mdg3epi8=" crossorigin></script>
@@ -19,17 +19,16 @@
 <body>
 <main>
 <article id="content">
 <header>
 <h1 class="title">Module <code>twincore</code></h1>
 </header>
 <section id="section-intro">
-<p>!
-@mainpage</p>
-<pre><code>Database with two files. One for data, one for index;
+<pre>
+Database with two files. One for data, one for index;
 
 The reason for the 'twin' name is that two files are created.
 The first contains the data, the second contains the
 offsets (indexes) and hashes.
 
 The second file can be re-built easily from the first
 using the reindex option.
@@ -63,105 +62,106 @@
 
 Debug:    (use the '-d' option with number)
 
     0 =  no output
     1 =  normal, some items
     2 =  more details
 
-History:
 
-    1.1         Tue 20.Feb.2024     Initial release
-    1.2.0       Mon 26.Feb.2024     Moved pip home to pydbase/
-    1.4.0       Tue 27.Feb.2024     Addedd pgdebug
-    1.4.2       Wed 28.Feb.2024     Fixed multiple instances
-    1.4.3       Wed 28.Feb.2024     ChainAdm added
-    1.4.4       Fri 01.Mar.2024     Tests for chain functions
-    1.4.5       Fri 01.Mar.2024     Misc fixes
-    1.4.6       Mon 04.Mar.2024     Vacuum count on vacuumed records
-    1.4.7       Tue 05.Mar.2024     In place record update
-    1.4.8       Sat 09.Mar.2024     Added new locking mechanism
-</code></pre>
+History
+-----=
+
+1.1         Tue 20.Feb.2024     Initial release
+1.2.0       Mon 26.Feb.2024     Moved pip home to pydbase/
+1.4.0       Tue 27.Feb.2024     Addedd pgdebug
+1.4.2       Wed 28.Feb.2024     Fixed multiple instances
+1.4.3       Wed 28.Feb.2024     ChainAdm added
+1.4.4       Fri 01.Mar.2024     Tests for chain functions
+1.4.5       Fri 01.Mar.2024     Misc fixes
+1.4.6       Mon 04.Mar.2024     Vacuum count on vacuumed records
+1.4.7       Tue 05.Mar.2024     In place record update
+1.4.8       Sat 09.Mar.2024     Added new locking mechanism
+... more ... see README.md
+</pre>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
 <pre><code class="python">#!/usr/bin/env python3
 
-&#39;&#39;&#39;!
-    @mainpage
-
-        Database with two files. One for data, one for index;
-
-        The reason for the &#39;twin&#39; name is that two files are created.
-        The first contains the data, the second contains the
-        offsets (indexes) and hashes.
-
-        The second file can be re-built easily from the first
-        using the reindex option.
-
-        Structure of the data:
-
-            32 byte header, starating with FILESIG;
-
-            4 bytes    4 bytes          4 bytes         Variable
-            ------------------------------------------------------------
-            RECSIG     Hash_of_key      Len_of_key      DATA_for_key
-            RECSEP     Hash_of_payload  Len_of_payload  DATA_for_payload
-                .
-                .
-
-            RECSIG     Hash_of_key      Len_of_key      DATA_for_key
-            RECSEP     Hash_of_payload  Len_of_payload  DATA_for_payload
-
-        Deleted records are marked with RECSIG mutated from RECB to RECX
-
-        New data is appended to the end, no duplicate filtering is done.
-        Retrieval is searched from reverse, the latest record with this key
-        is retrieved first.
-
-        Verbosity:    (use the &#39;-v&#39; option multiple times)
-
-            0 =  no output
-            1 =  normal, some items printed, short record ;
-            2 =  more detail; full record (-vv)
-            3 =  more detail + damaged records (-vvv)
-
-        Debug:    (use the &#39;-d&#39; option with number)
-
-            0 =  no output
-            1 =  normal, some items
-            2 =  more details
-
-        History:
-
-            1.1         Tue 20.Feb.2024     Initial release
-            1.2.0       Mon 26.Feb.2024     Moved pip home to pydbase/
-            1.4.0       Tue 27.Feb.2024     Addedd pgdebug
-            1.4.2       Wed 28.Feb.2024     Fixed multiple instances
-            1.4.3       Wed 28.Feb.2024     ChainAdm added
-            1.4.4       Fri 01.Mar.2024     Tests for chain functions
-            1.4.5       Fri 01.Mar.2024     Misc fixes
-            1.4.6       Mon 04.Mar.2024     Vacuum count on vacuumed records
-            1.4.7       Tue 05.Mar.2024     In place record update
-            1.4.8       Sat 09.Mar.2024     Added new locking mechanism
+&#39;&#39;&#39;
+    &lt;pre&gt;
+    Database with two files. One for data, one for index;
 
+    The reason for the &#39;twin&#39; name is that two files are created.
+    The first contains the data, the second contains the
+    offsets (indexes) and hashes.
+
+    The second file can be re-built easily from the first
+    using the reindex option.
+
+    Structure of the data:
+
+        32 byte header, starating with FILESIG;
+
+        4 bytes    4 bytes          4 bytes         Variable
+        ------------------------------------------------------------
+        RECSIG     Hash_of_key      Len_of_key      DATA_for_key
+        RECSEP     Hash_of_payload  Len_of_payload  DATA_for_payload
+            .
+            .
+
+        RECSIG     Hash_of_key      Len_of_key      DATA_for_key
+        RECSEP     Hash_of_payload  Len_of_payload  DATA_for_payload
+
+    Deleted records are marked with RECSIG mutated from RECB to RECX
+
+    New data is appended to the end, no duplicate filtering is done.
+    Retrieval is searched from reverse, the latest record with this key
+    is retrieved first.
+
+    Verbosity:    (use the &#39;-v&#39; option multiple times)
+
+        0 =  no output
+        1 =  normal, some items printed, short record ;
+        2 =  more detail; full record (-vv)
+        3 =  more detail + damaged records (-vvv)
+
+    Debug:    (use the &#39;-d&#39; option with number)
+
+        0 =  no output
+        1 =  normal, some items
+        2 =  more details
+
+    History:
+
+        1.1         Tue 20.Feb.2024     Initial release
+        1.2.0       Mon 26.Feb.2024     Moved pip home to pydbase/
+        1.4.0       Tue 27.Feb.2024     Addedd pgdebug
+        1.4.2       Wed 28.Feb.2024     Fixed multiple instances
+        1.4.3       Wed 28.Feb.2024     ChainAdm added
+        1.4.4       Fri 01.Mar.2024     Tests for chain functions
+        1.4.5       Fri 01.Mar.2024     Misc fixes
+        1.4.6       Mon 04.Mar.2024     Vacuum count on vacuumed records
+        1.4.7       Tue 05.Mar.2024     In place record update
+        1.4.8       Sat 09.Mar.2024     Added new locking mechanism
+        ... more ... see README.md
+        &lt;/pre&gt;
 &#39;&#39;&#39;
 
 import  os, sys, getopt, signal, select, socket, time, struct
 import  random, stat, os.path, datetime, threading
 import  struct, io
 
 base = os.path.dirname(os.path.realpath(__file__))
 sys.path.append(os.path.join(base))
 sys.path.append(os.path.join(base, &#39;..&#39;, &#39;pydbase&#39;))
 
 from twinbase import *
 
-Version = &#34;1.4.8&#34;
-
 # ------------------------------------------------------------------------
 
 class TwinCore(TwinCoreBase):
 
     &#39;&#39;&#39;
 
      Data file and index file; protected by locks
@@ -172,21 +172,22 @@
     def __init__(self, fname = &#34;pydbase.pydb&#34;, pgdebug = 0, devmode = 1):
 
         self.cnt = 0
         self.fname = fname
         self.lckname  = os.path.splitext(self.fname)[0] + &#34;.lock&#34;
         self.idxname  = os.path.splitext(self.fname)[0] + &#34;.pidx&#34;
         self.pgdebug = pgdebug
-        self.base_verbose  = 0
-        self.core_verbose  = 0
+        self.verbose  = 0
+        self.showdel  = 0
+        self.integrity = 0
         self.devmode = devmode
         self.lock = FileLock(self.lckname)
 
         # Make sure only one process can use this
-        self.lock.waitlock() #self.lckname)
+        self.lock.waitlock()
 
         super(TwinCore, self).__init__(pgdebug)
 
         #print(&#34;initializing core with&#34;, fname, pgdebug)
         #self.pool = threading.BoundedSemaphore(value=1)
 
         # It was informative at one point
@@ -231,31 +232,27 @@
             #self.ifp = self.softcreate(self.idxname)
             indexsize = self.getsize(self.ifp)
 
             # See if valid index
             if indexsize &lt; HEADSIZE:
                 self.create_idx(self.ifp)
                 # It was an existing data, new index needed
-                if self.base_verbose &gt; 0:
+                if self.verbose &gt; 0:
                     print(&#34;Reindexing&#34;)
                 self.__reindex()
 
         # Check
         if  self.getbuffstr(0, 4) != FILESIG:
-            if self.base_verbose &gt; 2:
+            if self.verbose &gt; 2:
                 print(&#34;Invalid data signature&#34;)
-            self.lock.unlock()  #dellock(self.lckname)
+            self.lock.unlock()
             raise  RuntimeError(&#34;Invalid database signature.&#34;)
 
         #print(&#34;buffsize&#34;, buffsize, &#34;indexsize&#34;, indexsize)
-        self.lock.unlock() #dellock(self.lckname)
-
-    def version(self):
-        &#39;&#39;&#39; Return version sting. &#39;&#39;&#39;
-        return Version
+        self.lock.unlock()
 
     def flush(self):
 
         &#39;&#39;&#39; Flush files to disk. &#39;&#39;&#39;
 
         if self.pgdebug &gt; 9:
             print(&#34;Flushing&#34;, self.fp, self.ifp)
@@ -293,61 +290,65 @@
             ret = 0
 
         return  ret
 
     # --------------------------------------------------------------------
     def _rec2arr(self, rec):
 
+        # Wed 10.Apr.2024 decision is made at the higher level
         arr = []
         sig = self.getbuffstr(rec, self.INTSIZE)
 
-        if sig == RECDEL:
-            return arr
-
-        if sig != RECSIG:
-            if self.base_verbose &gt; 0:
+        if sig != RECSIG and sig != RECDEL:
+            if self.verbose &gt; 0:
                 print(&#34; Damaged data (sig) &#39;%s&#39; at&#34; % sig, rec)
             return arr
 
         hash = self.getbuffint(rec+4)
         blen = self.getbuffint(rec+8)
         data = self.getbuffstr(rec + 12, blen)
 
-        if base_integrity:
+        if self.integrity:
             ccc = self.hash32(data)
-            if self.base_verbose &gt; 1:
+            if self.verbose &gt; 1:
                 print(&#34;rec&#34;, rec, &#34;hash&#34;, hex(hash), &#34;check&#34;, hex(ccc))
             if hash != ccc:
-                if self.base_verbose &gt; 0:
+                if self.verbose &gt; 0:
                     print(&#34;Error on hash at rec&#34;, rec, &#34;hash&#34;, hex(hash), &#34;check&#34;, hex(ccc))
                 return []
 
         #print(&#34;%5d pos %5d&#34; % (cnt, rec), &#34;hash %8x&#34; % hash, &#34;ok&#34;, ok, &#34;len=&#34;, blen, end=&#34; &#34;)
 
         endd = self.getbuffstr(rec + 12 + blen, self.INTSIZE)
         if endd != RECSEP:
-            if self.base_verbose &gt; 0:
+            if self.verbose &gt; 0:
                 print(&#34; Damaged data (sep) &#39;%s&#39; at&#34; % endd, rec)
             return arr
 
         rec2 = rec + 16 + blen;
         hash2 = self.getbuffint(rec2)
         blen2 = self.getbuffint(rec2+4)
         data2 = self.getbuffstr(rec2+8, blen2)
 
-        if base_integrity:
+        if self.integrity:
             ccc2 = self.hash32(data2)
-            if self.base_verbose &gt; 1:
+            if self.verbose &gt; 1:
                 print(&#34;rec&#34;, rec, &#34;hash2&#34;, hex(hash2), &#34;check2&#34;, hex(ccc2))
             if hash2 != ccc2:
-                if self.base_verbose &gt; 0:
+                if self.verbose &gt; 0:
                     print(&#34;Error on hash at rec&#34;, rec, &#34;hash2&#34;, hex(hash2), &#34;check2&#34;, hex(ccc2))
                 return []
 
-        arr = [data, data2]
+        if sig == RECDEL:
+            if self.showdel:
+                arr = [b&#34;del&#34;, data, data2]
+            else:
+                arr = []
+        else:
+            arr = [data, data2]
         return arr
 
     # -------------------------------------------------------------------
     # Originator, dump single record
 
     def  dump_rec(self, rec, cnt):
 
@@ -358,90 +359,90 @@
 
         cnt2 = 0
         sig = self.getbuffstr(rec, self.INTSIZE)
         if self.pgdebug &gt; 5:
             print(&#34;Sig &#34;, sig, &#34;at&#34;, rec)
 
         if sig == RECDEL:
-            if base_showdel:
+            if self.showdel:
                 klen = self.getbuffint(rec+8)
                 kdata = self.getbuffstr(rec+12, klen)
                 rec2 = rec + 16 + klen;
                 blen = self.getbuffint(rec2+4)
                 data = self.getbuffstr(rec2+8, blen)
                 print(&#34; Del at&#34;, rec, &#34;key:&#34;, kdata, &#34;data:&#34;, truncs(data))
-            if self.base_verbose &gt; 1:
+            if self.verbose &gt; 1:
                 klen = self.getbuffint(rec+8)
                 kdata = self.getbuffstr(rec+12, klen)
                 rec2 = rec + 16 + klen;
                 blen = self.getbuffint(rec2+4)
                 data = self.getbuffstr(rec2+8, blen)
-                if self.base_verbose &gt; 2:
+                if self.verbose &gt; 2:
                     print(&#34; Del at&#34;, rec, &#34;key:&#34;, kdata, &#34;data:&#34;, data)
                 else:
                     print(&#34; Del at&#34;, rec, &#34;key:&#34;, kdata, &#34;data:&#34;, truncs(data))
 
             return cnt2
 
         if sig != RECSIG:
-            if self.base_verbose &gt; 1:
+            if self.verbose &gt; 1:
                 print(&#34; Damaged data (sig) &#39;%s&#39; at&#34; % sig, rec)
             return cnt2
 
         hash = self.getbuffint(rec+4)
         blen = self.getbuffint(rec+8)
 
         if blen &lt; 0:
-            if self.base_verbose &gt; 2:
+            if self.verbose &gt; 2:
                 print(&#34;Invalid key length %d at %d&#34; % (blen, rec))
             return cnt2
 
         data = self.getbuffstr(rec+12, blen)
-        if base_integrity:
+        if self.integrity:
             ccc = self.hash32(data)
-            if self.base_verbose &gt; 1:
+            if self.verbose &gt; 1:
                 print(&#34;rec&#34;, rec, &#34;hash&#34;, hex(hash), &#34;check&#34;, hex(ccc))
             if hash != ccc:
-                if self.base_verbose &gt; 0:
+                if self.verbose &gt; 0:
                     print(&#34;Error on hash at rec&#34;, rec, &#34;hash&#34;, hex(hash), &#34;check&#34;, hex(ccc))
                 return []
 
         endd = self.getbuffstr(rec + 12 + blen, self.INTSIZE)
         if endd != RECSEP:
-            if self.base_verbose &gt; 0:
+            if self.verbose &gt; 0:
                 print(&#34; Damaged data (sep) &#39;%s&#39; at&#34; % endd, rec)
             return cnt2
 
         rec2 = rec + 16 + blen;
         hash2 = self.getbuffint(rec2)
         blen2 = self.getbuffint(rec2+4)
 
         if blen2 &lt; 0:
-            if self.base_verbose &gt; 1:
+            if self.verbose &gt; 1:
                 print(&#34;Invalid data length %d at %d&#34; % (blen2, rec))
             return cnt2
 
         data2 = self.getbuffstr(rec2+8, blen2)
-        if base_integrity:
+        if self.integrity:
             ccc2 = self.hash32(data2)
-            if self.base_verbose &gt; 1:
+            if self.verbose &gt; 1:
                 print(&#34;rec&#34;, rec, &#34;hash2&#34;, hex(hash), &#34;check2&#34;, hex(ccc))
             if hash2 != ccc2:
-                if self.base_verbose &gt; 0:
+                if self.verbose &gt; 0:
                     print(&#34;Error on hash at rec&#34;, rec, &#34;hash2&#34;, hex(hash), &#34;check2&#34;, hex(ccc))
                 return []
 
-        if self.base_verbose &gt; 2:
+        if self.verbose &gt; 2:
             print(&#34;%-5d pos %5d&#34; % (cnt, rec), &#34;%8x&#34; % hash, &#34;len&#34;, blen, data,
                                                         &#34;%8x&#34; % hash2,&#34;len&#34;, blen2, data2)
 
-        elif self.base_verbose &gt; 1:
+        elif self.verbose &gt; 1:
             print(&#34;%-5d pos %5d&#34; % (cnt, rec), &#34;%8x&#34; % hash, &#34;len&#34;, blen, data,
                                                         &#34;%8x&#34; % hash2,&#34;len&#34;, blen2, data2)
-        elif self.base_verbose:
+        elif self.verbose:
             print(&#34;%-5d pos %5d&#34; % (cnt, rec),  data, data2)
         else:
             print(&#34;%-5d pos %5d&#34; % (cnt, rec), &#34;Data:&#34;, truncs(data, 18), &#34;Data2:&#34;, truncs(data2, 18))
 
         cnt2 += 1
         return cnt2
 
@@ -450,72 +451,72 @@
         &#39;&#39;&#39; Check record. Verbose to the screen. Return number of errors.&#39;&#39;&#39;
 
         ret = 0
         sig = self.getbuffstr(rec, self.INTSIZE)
 
         # Do not check deleted, say OK
         if sig == RECDEL:
-            if self.base_verbose &gt; 1:
+            if self.verbose &gt; 1:
                 print(&#34; Deleted data &#39;%s&#39; at %d (%d)&#34; % (sig, rec, cnt2))
             ret = 1
             return ret
 
         if sig != RECSIG:
-            if self.base_verbose &gt; 0:
+            if self.verbose &gt; 0:
                 print(&#34; Damaged data (sig) &#39;%s&#39; at %d (%d)&#34; % (sig, rec, cnt2))
-            #if self.base_verbose &gt; 1:
+            #if self.verbose &gt; 1:
             #    print(&#34;Data&#34;, data)
 
             return ret
 
         hash = self.getbuffint(rec+4)
         blen = self.getbuffint(rec+8)
 
         if blen &lt;= 0:
-            if self.base_verbose &gt; 1:
+            if self.verbose &gt; 1:
                 print(&#34;Invalid key length %d at %d&#34; % (blen, rec))
             return ret
 
         data = self.getbuffstr(rec+12, blen)
         ccc = self.hash32(data)
         if hash != ccc:
-            if self.base_verbose &gt; 1:
+            if self.verbose &gt; 1:
                 print(&#34;Data&#34;, data)
-            elif self.base_verbose &gt; 0:
+            elif self.verbose &gt; 0:
                 print(&#34;Error on hash at rec&#34;, rec, cnt2, &#34;hash&#34;,
                                             hex(hash), &#34;check&#34;, hex(ccc))
 
             return ret
 
         endd = self.getbuffstr(rec + 12 + blen, self.INTSIZE)
         if endd != RECSEP:
-            if self.base_verbose &gt; 0:
+            if self.verbose &gt; 0:
                 print(&#34; Damaged data (sep) &#39;%s&#39; at %d %d %d&#34; % (endd, rec, cnt2))
             return ret
 
         rec2 = rec + 16 + blen;
         hash2 = self.getbuffint(rec2)
         blen2 = self.getbuffint(rec2+4)
 
         if blen2 &lt; 0:
-            if self.base_verbose &gt; 1:
+            if self.verbose &gt; 1:
                 print(&#34;Invalid data length2 %d at %d&#34; % (blen2, rec))
             return ret
 
         data2 = self.getbuffstr(rec2+8, blen2)
         ccc2 = self.hash32(data2)
         if hash2 != ccc2:
-            if self.base_verbose &gt; 1:
+            if self.verbose &gt; 1:
                 print(&#34;Data&#34;, data, &#34;Data2&#34;, data2)
-            elif self.base_verbose &gt; 0:
+            elif self.verbose &gt; 0:
                 print(&#34;Error on hash2 at rec&#34;, rec, cnt2, &#34;hash2&#34;,
                                         hex(hash2), &#34;check2&#34;, hex(ccc2))
             return ret
 
-        if self.base_verbose &gt; 2:
+        if self.verbose &gt; 2:
             print(&#34;Record at %d (%d) OK.&#34; % (rec, cnt2))
 
         ret += 1
         return ret
 
     # --------------------------------------------------------------------
     # Internal; no locking
@@ -536,26 +537,23 @@
         else:
             rrr = range(chash - self.INTSIZE * 2, HEADSIZE  - self.INTSIZE * 2, -self.INTSIZE * 2)
 
         for aa in rrr:
             rec = self.getidxint(aa)
 
             #print(aa, rec)
-            if not base_quiet:
-                cnt2 += 1
-                ret = self.dump_rec(rec, cnt)
-
-                if not ret:
-                    if self.pgdebug &gt; 5:
-                        print(&#34;Deleted / empty record at&#34;, cnt)
-
-                if ret:
-                    cnt += 1
-                    if cnt &gt;= lim:
-                        break
+            cnt2 += 1
+            ret = self.dump_rec(rec, cnt)
+            if not ret:
+                if self.pgdebug &gt; 5:
+                    print(&#34;Deleted / empty record at&#34;, cnt)
+            if ret:
+                cnt += 1
+                if cnt &gt;= lim:
+                    break
 
     def  dump_data(self, lim = INT_MAX, skip = 0):
 
         &#39;&#39;&#39; Put all data to screen. &#39;&#39;&#39;
 
         self.__dump_data(lim, skip, 1)
 
@@ -565,17 +563,17 @@
 
         self.__dump_data(lim, skip)
 
     def  reindex(self):
 
         &#39;&#39;&#39; Re create index file. &#39;&#39;&#39;
 
-        self.lock.waitlock() #self.lckname)
+        self.lock.waitlock()
         ret = self.__reindex()
-        self.lock.unlock()    #dellock(self.lckname)
+        self.lock.unlock()
         return ret
 
     # --------------------------------------------------------------------
 
     def  __reindex(self):
 
         &#39;&#39;&#39; Recover index. Make sure the DB in not in session.  &#39;&#39;&#39;
@@ -596,50 +594,50 @@
         tmplock = FileLock(relock)
         tmplock.waitlock()
 
         tempifp = self.softcreate(reidx)
         self.create_idx(tempifp)
         dlen = self.getsize(self.fp)
 
-        if self.base_verbose &gt; 2:
+        if self.verbose &gt; 2:
            print(&#34;curr&#34;, curr, &#34;dlen&#34;, dlen)
 
         aa =  HEADSIZE
         while 1:
             if aa &gt;= dlen:
                 break
 
             sig = self.getbuffstr(aa, self.INTSIZE)
             # Check if sig is correct
             if sig != RECSIG:
-                if self.core_verbose &gt; 0:
+                if self.verbose &gt; 0:
                     print(&#34;Invalid sig .. resync needed&#34;)
                 raise
 
             #print(&#34;reind&#34;, aa)
 
             try:
                 hhh2 = self.getbuffint(aa + 4)
                 lenx = self.getbuffint(aa + 8)
                 if lenx &lt; 0:
-                    if self.core_verbose &gt; 0:
+                    if self.verbose &gt; 0:
                         print(&#34;Invalid key length.&#34;)
                 sep =  self.getbuffstr(aa + 12 + lenx, self.INTSIZE)
                 len2 =  self.getbuffint(aa + 20 + lenx)
                 if len2 &lt; 0:
-                    if self.core_verbose &gt; 0:
+                    if self.verbose &gt; 0:
                         print(&#34;Invalid record length&#34;)
             except:
-                if self.core_verbose &gt; 2:
+                if self.verbose &gt; 2:
                     print(&#34;in reindex&#34;, sys.exc_info())
 
-            if self.base_verbose == 1:
+            if self.verbose == 1:
                 print(aa, &#34;sig&#34;, sig, &#34;hhh2&#34;, hex(hhh2), &#34;len&#34;, lenx, \
                     &#34;sep&#34;, sep, &#34;len2&#34;, len2)
-            if self.base_verbose &gt; 1:
+            if self.verbose &gt; 1:
                 data =  self.getbuffstr(aa + 12, lenx)
                 data2 =  self.getbuffstr(aa + 24 + lenx, len2)
                 print(aa, &#34;sig&#34;, sig, &#34;data&#34;, data, &#34;data2&#34;, data2)
 
             # Update / Append index
             #hashpos = self._getint(tempifp, CURROFFS)
             hashpos =  HEADSIZE  + self._getdbsize(tempifp) * self.INTSIZE * 2
@@ -712,17 +710,17 @@
         &#39;&#39;&#39;
             Remove all deleted data. Reindex.
             The db is locked while the vacuum is in operation, but
             make sure the DB in not in session, and no pending
             operations are present (like find / retrieve cycle).
         &#39;&#39;&#39;
 
-        self.lock.waitlock() #self.lckname)
+        self.lock.waitlock()
         ret = self._vacuum()
-        self.lock.unlock()  #dellock(self.lckname)
+        self.lock.unlock()
         return ret
 
     def  _vacuum(self):
 
         vacname = os.path.splitext(self.fname)[0] + &#34;_vac_&#34; + &#34;.pydb&#34;
         vacerr  = os.path.splitext(self.fname)[0] +  &#34;.perr&#34;
         vacidx = os.path.splitext(vacname)[0]  + &#34;.pidx&#34;
@@ -758,24 +756,21 @@
                 sig = self.getbuffstr(rec, self.INTSIZE)
                 if sig == RECDEL:
                     ret += 1
                     vac += 1
                     if self.pgdebug &gt; 1:
                         print(&#34;deleted&#34;, rec)
                 elif sig != RECSIG:
-                    if self.base_verbose:
+                    if self.verbose:
                         print(&#34;Detected error at %d&#34; % rec)
                     ret += 1
                     self.__save_error(rec, vacerrfp)
                 else:
-                    global base_integrity
-                    tmpi = base_integrity
-                    base_integrity = True
+                    self.integrity = True
                     arr = self.get_rec_byoffs(rec)
-                    base_integrity = tmpi
 
                     if self.pgdebug &gt; 1:
                         print(cnt, &#34;vac rec&#34;, rec, arr)
 
                     if len(arr) &gt; 1:
                         hhh2 = self.hash32(arr[0])
                         hhh3 = self.hash32(arr[1])
@@ -787,103 +782,103 @@
                         if self.pgdebug &gt; 0:
                             print(&#34;Error on vac: %d&#34; % rec)
                 cnt += 1
 
             vacdb.fp.close()
             vacdb.ifp.close()
 
-            vacdb.lock.unlock()  #dellock(vacdb.lckname)
+            vacdb.lock.unlock()
 
             # if vacerr is empty
             try:
                 if os.stat(vacerr).st_size == 0:
                     #print(&#34;Vac error empty&#34;)
                     os.remove(vacerr)
             except:
-                if self.core_verbose &gt; 0:
+                if self.verbose &gt; 0:
                     print(&#34;vacerr&#34;, sys.exc_info())
 
         # Any vacummed?
         if vac &gt; 0:
             # Make it go out of scope
             self.fp.flush(); self.ifp.flush()
             self.fp.close(); self.ifp.close()
 
             # Now move files
             try:
                 os.remove(self.fname);
             except:
-                if self.core_verbose &gt; 0:
+                if self.verbose &gt; 0:
                     print(&#34;vacuum remove&#34;, self.fname, sys.exc_info())
                 pass
 
             try:
                 os.remove(self.idxname)
             except:
-                if self.core_verbose &gt; 2:
+                if self.verbose &gt; 2:
                     print(&#34;vacuum idx remove&#34;, self.idxname, sys.exc_info())
                 pass
 
             if self.pgdebug &gt; 1:
                 print(&#34;rename&#34;, vacname, &#34;-&gt;&#34;, self.fname)
                 print(&#34;rename&#34;, vacidx, &#34;-&gt;&#34;, self.idxname)
 
             try:
                 os.rename(vacname, self.fname)
             except:
-                if self.core_verbose &gt; 2:
+                if self.verbose &gt; 2:
                     print(&#34;vacuum rename&#34;, vacname, sys.exc_info())
             try:
                 os.rename(vacidx, self.idxname)
             except:
-                if self.core_verbose &gt; 2:
+                if self.verbose &gt; 2:
                     print(&#34;vacuum idx rename&#34;, vacidx, sys.exc_info())
 
-            self.lock.waitlock() #self.lckname)
+            self.lock.waitlock()
             self.fp = self.softcreate(self.fname)
             self.ifp = self.softcreate(self.idxname)
-            #self.lock.unlock()  #dellock(self.lckname)
+            #self.lock.unlock()
 
         else:
             # Just remove non vacuumed files
             if self.pgdebug &gt; 1:
                 print(&#34;deleted&#34;, vacname, vacidx)
             try:
                 os.remove(vacname)
                 os.remove(vacidx)
             except:
                 pass
 
         #self.lock.unlock()
-        #dellock(self.lckname)
+
 
         #print(&#34;ended vacuum&#34;)
         return ret, vac
 
     def  get_rec(self, recnum):
 
         &#39;&#39;&#39; Get record from database; recnum is a zero based record counter. &#39;&#39;&#39;
 
         if self.pgdebug:
-            print(&#34;getrec()&#34;, recnum)
+            print(&#34;get_rec()&#34;, recnum)
 
         rsize = self._getdbsize(self.ifp)
         if recnum &gt;= rsize:
-            if self.core_verbose &gt; 0:
+            if self.verbose &gt; 0:
                 print(&#34;Past end of data.&#34;);
-            raise  RuntimeError( \
-                    &#34;Past end of Data. Asking for %d while max is 0 .. %d records.&#34; \
-                                     % (recnum, rsize-1) )
+            errx =  &#34;Past end of Data. (ask: %d max: %d)&#34;  % (recnum, rsize-1)
+            raise  RuntimeError(errx)
             return []
 
         chash = self.getidxint(CURROFFS)
         #print(&#34;chash&#34;, chash)
         offs = self.getidxint(HEADSIZE + recnum * self.INTSIZE * 2)
 
-        #print(&#34;offs&#34;, offs)
+        #sig = self.getbuffstr(offs, self.INTSIZE)
+
         return self._rec2arr(offs)
 
     def  get_rec_byoffs(self, recoffs):
 
         &#39;&#39;&#39; Return record by offset. &#39;&#39;&#39;
 
         rsize = self.getsize(self.fp)
@@ -892,19 +887,18 @@
             raise  RuntimeError( \
                     &#34;Past end of File. Asking for offset %d file size is %d.&#34; \
                                      % (recoffs, rsize) )
             return []
 
         sig = self.getbuffstr(recoffs, self.INTSIZE)
         if sig == RECDEL:
-            if self.base_verbose:
+            if self.verbose:
                 print(&#34;Deleted record.&#34;)
-            return []
         if sig != RECSIG:
-            if self.core_verbose &gt; 0:
+            if self.verbose &gt; 0:
                 print(&#34;Unlikely offset %d is not at record boundary.&#34; % recoffs, sig)
             return []
         #print(&#34;recoffs&#34;, recoffs)
         return self._rec2arr(recoffs)
 
     def  get_key_offs(self, recoffs):
 
@@ -916,19 +910,19 @@
             raise  RuntimeError( \
                     &#34;Past end of File. Asking for offset %d file size is %d.&#34; \
                                      % (recoffs, rsize) )
             return []
 
         sig = self.getbuffstr(recoffs, self.INTSIZE)
         if sig == RECDEL:
-            if self.base_verbose:
+            if self.verbose:
                 print(&#34;Deleted record.&#34;)
             return []
         if sig != RECSIG:
-            if self.core_verbose &gt; 0:
+            if self.verbose &gt; 0:
                 print(&#34;Unlikely offset %d is not at record boundary.&#34; % recoffs, sig)
             return []
         #print(&#34;recoffs&#34;, recoffs)
         return self._rec2arr(recoffs)[0]
 
     def  del_rec(self, recnum):
 
@@ -936,24 +930,24 @@
             Deleted record is marked as deleted but not removed.
             Deleted records are ignored in further operations.
             Use &#39;vacuum&#39; to actually remove record.
         &#39;&#39;&#39;
 
         rsize = self._getdbsize(self.ifp)
         if recnum &gt;= rsize:
-            if self.base_verbose:
+            if self.verbose:
                 print(&#34;Past end of data.&#34;);
             return False
         chash = self.getidxint(CURROFFS)
         #print(&#34;chash&#34;, chash)
         offs = self.getidxint(HEADSIZE + recnum * self.INTSIZE * 2)
         #print(&#34;offs&#34;, offs)
         old = self.getbuffstr(offs, self.INTSIZE)
         if old == RECDEL:
-            if self.base_verbose:
+            if self.verbose:
                 print(&#34;Record at %d already deleted.&#34; % offs);
             return False
 
         self.putbuffstr(offs, RECDEL)
         return True
 
     def  del_rec_offs(self, recoffs):
@@ -966,44 +960,44 @@
             raise  RuntimeError( \
                     &#34;Past end of File. Asking for offset %d file size is %d.&#34; \
                                      % (recoffs, rsize) )
             return False
 
         sig = self.getbuffstr(recoffs, self.INTSIZE)
         if sig != RECSIG  and sig != RECDEL:
-            if self.core_verbose &gt; 0:
+            if self.verbose &gt; 0:
                 print(&#34;Unlikely offset %d is not at record boundary.&#34; % recoffs, sig)
             return False
 
         self.putbuffstr(recoffs, RECDEL)
         return True
 
     # Check integrity
 
     def integrity_check(self, skip = 0, count = 0xffffffff):
 
         &#39;&#39;&#39; Check record integrity for &#39;count&#39; records.
             Skip number of records.
         &#39;&#39;&#39;
 
-        self.lock.waitlock()    #(self.lckname)
+        self.lock.waitlock()
         ret = 0; cnt2 = 0; cnt3 = 0;
         #chash = self.getidxint(CURROFFS)        #;print(&#34;chash&#34;, chash)
         chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
         # Direction sensitivity
         rrr = range(HEADSIZE + skip * self.INTSIZE * 2, chash, self.INTSIZE * 2)
         for aa in rrr:
             rec = self.getidxint(aa)
             #print(aa, rec)
             ret += self.check_rec(rec, cnt2)
             cnt2 += 1
             cnt3 += 1
             if cnt3 &gt;= count:
                 break
-        self.lock.unlock() #dellock(self.lckname)
+        self.lock.unlock()
         return ret, cnt2
 
     def  retrieve(self, strx, limx = 1):
 
         &#39;&#39;&#39; Retrive in reverse, limit it. &#39;&#39;&#39;
 
         if type(strx) != type(b&#34;&#34;):
@@ -1015,33 +1009,33 @@
 
         #chash = self.getidxint(CURROFFS)
         chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
 
         #;print(&#34;chash&#34;, chash)
         arr = []
 
-        self.lock.waitlock() #(self.lckname)
+        self.lock.waitlock()
 
         #for aa in range(HEADSIZE + self.INTSIZE * 2, chash, self.INTSIZE * 2):
         for aa in range(chash - self.INTSIZE * 2, HEADSIZE  - self.INTSIZE * 2, -self.INTSIZE * 2):
             rec = self.getidxint(aa)
             sig = self.getbuffstr(rec, self.INTSIZE)
             if sig == RECDEL:
-                if self.base_verbose &gt; 3:
+                if self.verbose &gt; 3:
                     print(&#34; Deleted record &#39;%s&#39; at&#34; % sig, rec)
             elif sig != RECSIG:
-                if self.base_verbose:
+                if self.verbose:
                     print(&#34; Damaged data &#39;%s&#39; at&#34; % sig, rec)
             else:
                 hhh = self.getbuffint(rec+4)
                 if hhh == hhhh:
                     arr.append(self.get_rec_byoffs(rec))
                     if len(arr) &gt;= limx:
                         break
-        self.lock.unlock()  #dellock(self.lckname)
+        self.lock.unlock()
 
         return arr
 
     # Return record offset
 
     def  _recoffset(self, strx, limx = INT_MAX, skipx = 0):
 
@@ -1058,151 +1052,153 @@
         #print(&#34;_recoffset&#34;, strx2)
 
         #for aa in range(HEADSIZE + self.INTSIZE * 2, chash, self.INTSIZE * 2):
         for aa in range(chash - self.INTSIZE * 2, HEADSIZE  - self.INTSIZE * 2, -self.INTSIZE * 2):
             rec = self.getidxint(aa)
             sig = self.getbuffstr(rec, self.INTSIZE)
             if sig == RECDEL:
-                if base_showdel:
+                if self.showdel:
                     print(&#34; Deleted record &#39;%s&#39; at&#34; % sig, rec)
             elif sig != RECSIG:
-                if self.base_verbose &gt; 0:
+                if self.verbose &gt; 0:
                     print(&#34; Damaged data &#39;%s&#39; at&#34; % sig, rec)
             else:
                 blen = self.getbuffint(rec+8)
                 keyz = self.getbuffstr(rec + 12, blen)
-                if self.base_verbose &gt; 1:
+                if self.verbose &gt; 1:
                     print(&#34;_recoffset&#34;, keyz)
                 if strx2 == keyz:
                     sig = self.getbuffstr(rec + 16 + blen,  self.INTSIZE)
                     xlen = self.getbuffint(rec + 20 + blen)
                     data = self.getbuffstr(rec + 24 + blen, xlen)
                     #print(&#34;rec offset&#34;, rec + 12,  &#34;key:&#34;, keyz, &#34;data:&#34;, data)
                     break       # Only the last one
         return rec, rec+24 + blen, len(data)
 
     def  findrec(self, strx, limx = INT_MAX, skipx = 0):
 
-        &#39;&#39;&#39; Find by string matching substring. &#39;&#39;&#39;
+        &#39;&#39;&#39; Find key by matching strx with substring.
+        Return record(s).
+        &#39;&#39;&#39;
 
-        self.lock.waitlock()    #(self.lckname)
+        self.lock.waitlock()
 
         #chash = self.getidxint(CURROFFS)            #;print(&#34;chash&#34;, chash)
         chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
 
         arr = []
         strx2 = strx.encode(errors=&#39;strict&#39;);
 
         #print(&#34;findrec&#34;, strx2)
 
         #for aa in range(HEADSIZE + self.INTSIZE * 2, chash, self.INTSIZE * 2):
         for aa in range(chash - self.INTSIZE * 2, HEADSIZE  - self.INTSIZE * 2, -self.INTSIZE * 2):
             rec = self.getidxint(aa)
             sig = self.getbuffstr(rec, self.INTSIZE)
             if sig == RECDEL:
-                if base_showdel:
+                if self.showdel:
                     print(&#34; Deleted record &#39;%s&#39; at&#34; % sig, rec)
             elif sig != RECSIG:
-                if self.base_verbose &gt; 0:
+                if self.verbose &gt; 0:
                     print(&#34; Damaged data &#39;%s&#39; at&#34; % sig, rec)
             else:
                 blen = self.getbuffint(rec+8)
                 data = self.getbuffstr(rec + 12, blen)
-                if self.base_verbose &gt; 1:
+                if self.verbose &gt; 1:
                     print(&#34;find&#34;, data)
                 #if str(strx2) in str(data):
                 if strx2 in data:
                     arr.append(self.get_key_offs(rec))
                     #arr.append(rec)
 
                     if len(arr) &gt;= limx:
                         break
-        self.lock.unlock()  #dellock(self.lckname)
+        self.lock.unlock()
 
         return arr
 
     def  findrecpos(self, strx, limx = INT_MAX, skipx = 0):
 
-        &#39;&#39;&#39; Find record, return array of positions. &#39;&#39;&#39;
+        &#39;&#39;&#39; Find record by key, return array of positions. &#39;&#39;&#39;
 
-        self.lock.waitlock()    #(self.lckname)
+        self.lock.waitlock()
         chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
         arr = []
         if type(strx) != type(b&#34;&#34;):
             strx = strx.encode(errors=&#39;strict&#39;);
 
         for aa in range(chash - self.INTSIZE * 2, HEADSIZE  - self.INTSIZE * 2, -self.INTSIZE * 2):
             rec = self.getidxint(aa)
             sig = self.getbuffstr(rec, self.INTSIZE)
             if sig == RECDEL:
-                if base_showdel:
+                if self.showdel:
                     print(&#34; Deleted record &#39;%s&#39; at&#34; % sig, rec)
             elif sig != RECSIG:
-                if self.base_verbose &gt; 0:
+                if self.verbose &gt; 0:
                     print(&#34; Damaged data &#39;%s&#39; at&#34; % sig, rec)
             else:
                 blen = self.getbuffint(rec+8)
                 data = self.getbuffstr(rec + 12, blen)
-                if self.base_verbose &gt; 1:
+                if self.verbose &gt; 1:
                     print(&#34;frecpos&#34;, data)
                 if strx == data:
                     arr.append(rec)
                     if len(arr) &gt;= limx:
                         break
 
-        self.lock.unlock()  #dellock(self.lckname)
+        self.lock.unlock()
 
         return arr
 
-    def  findrec(self, strx, limx = INT_MAX, skipx = 0):
+    def  findrecsub(self, strx, limx = INT_MAX, skipx = 0):
 
-        &#39;&#39;&#39; Find by string matching substring. &#39;&#39;&#39;
+        &#39;&#39;&#39; Find record by matching substring. &#39;&#39;&#39;
 
-        self.lock.waitlock()    #(self.lckname)
+        self.lock.waitlock()
         chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
         arr = []
         if type(strx) != type(b&#34;&#34;):
             strx2 = strx.encode(errors=&#39;strict&#39;);
 
         #print(&#34;findrec&#34;, strx2)
 
         #for aa in range(HEADSIZE + self.INTSIZE * 2, chash, self.INTSIZE * 2):
         for aa in range(chash - self.INTSIZE * 2, HEADSIZE  - self.INTSIZE * 2, -self.INTSIZE * 2):
             rec = self.getidxint(aa)
             sig = self.getbuffstr(rec, self.INTSIZE)
             if sig == RECDEL:
-                if base_showdel:
+                if self.showdel:
                     print(&#34; Deleted record &#39;%s&#39; at&#34; % sig, rec)
             elif sig != RECSIG:
-                if self.base_verbose &gt; 0:
+                if self.verbose &gt; 0:
                     print(&#34; Damaged data &#39;%s&#39; at&#34; % sig, rec)
             else:
                 blen = self.getbuffint(rec+8)
                 data = self.getbuffstr(rec + 12, blen)
-                if self.base_verbose &gt; 1:
+                if self.verbose &gt; 1:
                     print(&#34;find&#34;, data)
                 #if str(strx2) in str(data):
                 if strx2 in data:
                     #arr.append(self.get_key_offs(rec))
                     #arr.append(rec)
                     arr.append(self._rec2arr(rec))
                     if len(arr) &gt;= limx:
                         break
-        self.lock.unlock()    #dellock(self.lckname)
+        self.lock.unlock()
 
         return arr
 
     # --------------------------------------------------------------------
     # List all active records
 
     def  listall(self):
 
         &#39;&#39;&#39; List all active records. Return array id record indexes. &#39;&#39;&#39;
 
-        self.lock.waitlock()    #(self.lckname)
+        self.lock.waitlock()
         keys = []; arr = []; cnt = 0
 
         chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
         maxrec = chash - self.INTSIZE * 2
         rsize = self._getdbsize(self.ifp) - 1
 
         rrr =  range(maxrec,
@@ -1210,39 +1206,42 @@
         for aa in rrr:
             rec = self.getidxint(aa)
 
             #print(&#34; Scanning at %d %d&#34; % (rec, cnt))
 
             sig = self.getbuffstr(rec, self.INTSIZE)
             if sig == RECDEL:
-                if 1: #base_showdel:
+                if 1: #self.showdel:
                     print(&#34;Deleted record &#39;%s&#39; at&#34; % sig, rec)
             elif sig != RECSIG:
-                if 1: #self.base_verbose &gt; 0:
+                if 1: #self.verbose &gt; 0:
                     print(&#34; Damaged data &#39;%s&#39; at&#34; % sig, rec)
             else:
                     hhh = self.getbuffint(rec+4)
                     print(&#34; Good data &#39;%s&#39; at&#34; % sig, rec, hhh)
                     if hhh not in keys:
                         keys.append(hhh)
                         # as we are going backwards
                         arr.append(rsize - cnt)
                         #print(&#34;found&#34;, hhh)
             cnt += 1
 
         keys = []
-        self.lock.unlock()  #dellock()self.lckname)
+        self.lock.unlock()
 
         return arr
 
     def  find_key(self, keyx, limx = 0xffffffff):
 
-        &#39;&#39;&#39; Find record by key Search from the end, so latest comes first. &#39;&#39;&#39;
+        &#39;&#39;&#39; Find record by key value.
+            Search from the end, so latest comes first.
+            This operates on the hash, so it reaches the answer fast.
+        &#39;&#39;&#39;
 
-        self.lock.waitlock()   #self.lckname)
+        self.lock.waitlock()
 
         skip = 0; arr = []; cnt = 0
         try:
             arg2e = keyx.encode()
         except:
             arg2e = keyx
 
@@ -1254,32 +1253,32 @@
                 HEADSIZE - self.INTSIZE * 2, -self.INTSIZE * 2)
         for aa in rrr:
             rec = self.getidxint(aa)
             #print(&#34; Scanning at %d %d&#34; % (rec, cnt))
 
             sig = self.getbuffstr(rec, self.INTSIZE)
             if sig == RECDEL:
-                if base_showdel:
+                if self.showdel:
                     print(&#34;Deleted record &#39;%s&#39; at&#34; % sig, rec)
             elif sig != RECSIG:
-                if self.base_verbose &gt; 0:
+                if self.verbose &gt; 0:
                     print(&#34; Damaged data &#39;%s&#39; at&#34; % sig, rec)
             else:
                 hhh = self.getbuffint(rec+4)
                 if hhh == hhhh:
                     if len(arr) &gt;= limx - 1:
                         arr.append([&#34;More data ...&#34;,])
                         break
                     arr.append(rec)
                 else:
                     pass
                     #print(&#34;no match&#34;, hex(hhh))
 
             cnt += 1
-        self.lock.unlock()  #dellock()self.lckname)
+        self.lock.unlock()
 
         return arr
 
 
     def  del_data(self, hash, skip = 1):
 
         &#39;&#39;&#39; Delete data by hash. &#39;&#39;&#39;
@@ -1299,15 +1298,15 @@
             #    print(&#34; Damaged data &#39;%s&#39; at&#34; % sig, rec)
 
             #blen = self.getbuffint(rec+8)
             #print(&#34;data &#39;%s&#39; at&#34; % sig, rec, &#34;blen&#34;, blen)
 
             hhh = self.getbuffint(rec+4)
             if hash == hhh:
-                if self.base_verbose &gt; 0:
+                if self.verbose &gt; 0:
                     print(&#34;Would delete&#34;, hhh)
 
             self.putbuffstr(rec, RECDEL)
 
             cnt += 1
 
         return arr
@@ -1332,15 +1331,15 @@
         &#39;&#39;&#39; Delete records by key string; needs bin str, converted
             automatically on entry.
         &#39;&#39;&#39;
 
         if type(strx) != type(b&#34;&#34;):
             strx = strx.encode()
 
-        if self.base_verbose &gt; 1:
+        if self.verbose &gt; 1:
             print(&#34;Start delete &#34;, strx, &#34;skip&#34;, skip)
 
         cnt = 0; cnt3 = 0
         #chash = self.getidxint(CURROFFS)    #;print(&#34;chash&#34;, chash)
         chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
 
         # Direction sensitivity
@@ -1350,58 +1349,58 @@
             rrr = range(chash - self.INTSIZE * 2, HEADSIZE  - self.INTSIZE * 2, -self.INTSIZE * 2)
 
         #for aa in range(HEADSIZE, chash, self.INTSIZE * 2):
         for aa in rrr:
             rec = self.getidxint(aa)
             sig = self.getbuffstr(rec, self.INTSIZE)
             if sig == RECDEL:
-                if base_showdel:
+                if self.showdel:
                     print(&#34; Deleted record &#39;%s&#39; at&#34; % sig, rec)
             elif sig != RECSIG:
-                if self.base_verbose &gt; 0:
+                if self.verbose &gt; 0:
                     print(&#34; Damaged data &#39;%s&#39; at&#34; % sig, rec)
             else:
                 blen = self.getbuffint(rec+8)
                 data = self.getbuffstr(rec + 12, blen)
-                if self.base_verbose &gt; 2:
+                if self.verbose &gt; 2:
                     print(&#34;del iterate recs&#34;, cnt3, data, strx)
 
                 if strx == data:
-                    if self.base_verbose &gt; 0:
+                    if self.verbose &gt; 0:
                         print(&#34;Deleting&#34;, cnt3, aa, data)
                     self.putbuffstr(rec, RECDEL)
                     cnt += 1
                     if cnt &gt;= maxdelrec:
                         break
             cnt3 += 1
         return cnt
 
     def  save_data(self, header, datax, replace = False):
 
         &#39;&#39;&#39; Append to the end of file. If replace flag is set, try to overwrite
-            in place. If new record is larger, add it as ususal. If smaller,
+            in place. If new record is larger, add it as usual. If smaller,
             the record is padded with spaces. This should not influence most ops.
             (like: int())
             This feature allows the database update wthout creating new records.
-            Useful for counters or dynamically changing data.
+            Useful for counters or dynamically changing data. To be useful,
+            use  create fixed size data. Like sprintf(%12d).
 
                     Input:
                         header     Header
                         datax      Data
 
                      Return:
                         The offset of saved data
             &#39;&#39;&#39;
 
         if self.pgdebug &gt; 0:
             print(&#34;Save_data()&#34;, header, datax)
 
-        self.lock.waitlock()   #self.lckname)
-        ret = 0
-        was = False
+        self.lock.waitlock()
+        ret = 0 ; was = False
         # Put new data in place
         if replace:
             if type(datax) != type(b&#34;&#34;):
                 mrep2 = datax.encode()
             else:
                 mrep2 = datax
 
@@ -1416,17 +1415,18 @@
                     ccc = self.hash32(padded)
                     self.putbuffint(rrr[1] - 8, ccc)
                     #print(&#34;ccc&#34;, hex(ccc))
                     self.putbuffstr(rrr[1], padded)
                     was = True
                     ret =  rrr[0]
         if not was:
+            #print(&#34;Saving longer data&#34;, header, datax)
             ret = self._save_data2(header, datax)
 
-        self.lock.unlock()  #dellock()self.lckname)
+        self.lock.unlock()
 
         return ret
 
     # --------------------------------------------------------------------
     # Save data to database file
 
     def  _save_data2(self, arg2, arg3):
@@ -1491,15 +1491,15 @@
         self.putidxint(curr, dcurr)
         self.putidxint(curr + self.INTSIZE, hhh2)
         #self.putidxint(CURROFFS, self.ifp.tell())
 
         self.fp.flush()
         self.ifp.flush()
 
-        return curr
+        return dcurr
 
     def __del__(self):
 
         &#39;&#39;&#39; flush file handles and close files. &#39;&#39;&#39;
 
         if hasattr(self, &#34;pgdebug&#34;):
             if self.pgdebug &gt; 9:
@@ -1515,14 +1515,18 @@
 
         if hasattr(self, &#34;ifp&#34;):
                 if self.ifp:
                     if not self.ifp.closed:
                         self.ifp.flush()
                         self.ifp.close()
 
+        # remove lockfile
+        if hasattr(self, &#34;lock&#34;):
+            self.lock.unlock()
+
 # EOF</code></pre>
 </details>
 </section>
 <section>
 </section>
 <section>
 </section>
@@ -1554,21 +1558,22 @@
     def __init__(self, fname = &#34;pydbase.pydb&#34;, pgdebug = 0, devmode = 1):
 
         self.cnt = 0
         self.fname = fname
         self.lckname  = os.path.splitext(self.fname)[0] + &#34;.lock&#34;
         self.idxname  = os.path.splitext(self.fname)[0] + &#34;.pidx&#34;
         self.pgdebug = pgdebug
-        self.base_verbose  = 0
-        self.core_verbose  = 0
+        self.verbose  = 0
+        self.showdel  = 0
+        self.integrity = 0
         self.devmode = devmode
         self.lock = FileLock(self.lckname)
 
         # Make sure only one process can use this
-        self.lock.waitlock() #self.lckname)
+        self.lock.waitlock()
 
         super(TwinCore, self).__init__(pgdebug)
 
         #print(&#34;initializing core with&#34;, fname, pgdebug)
         #self.pool = threading.BoundedSemaphore(value=1)
 
         # It was informative at one point
@@ -1613,31 +1618,27 @@
             #self.ifp = self.softcreate(self.idxname)
             indexsize = self.getsize(self.ifp)
 
             # See if valid index
             if indexsize &lt; HEADSIZE:
                 self.create_idx(self.ifp)
                 # It was an existing data, new index needed
-                if self.base_verbose &gt; 0:
+                if self.verbose &gt; 0:
                     print(&#34;Reindexing&#34;)
                 self.__reindex()
 
         # Check
         if  self.getbuffstr(0, 4) != FILESIG:
-            if self.base_verbose &gt; 2:
+            if self.verbose &gt; 2:
                 print(&#34;Invalid data signature&#34;)
-            self.lock.unlock()  #dellock(self.lckname)
+            self.lock.unlock()
             raise  RuntimeError(&#34;Invalid database signature.&#34;)
 
         #print(&#34;buffsize&#34;, buffsize, &#34;indexsize&#34;, indexsize)
-        self.lock.unlock() #dellock(self.lckname)
-
-    def version(self):
-        &#39;&#39;&#39; Return version sting. &#39;&#39;&#39;
-        return Version
+        self.lock.unlock()
 
     def flush(self):
 
         &#39;&#39;&#39; Flush files to disk. &#39;&#39;&#39;
 
         if self.pgdebug &gt; 9:
             print(&#34;Flushing&#34;, self.fp, self.ifp)
@@ -1675,61 +1676,65 @@
             ret = 0
 
         return  ret
 
     # --------------------------------------------------------------------
     def _rec2arr(self, rec):
 
+        # Wed 10.Apr.2024 decision is made at the higher level
         arr = []
         sig = self.getbuffstr(rec, self.INTSIZE)
 
-        if sig == RECDEL:
-            return arr
-
-        if sig != RECSIG:
-            if self.base_verbose &gt; 0:
+        if sig != RECSIG and sig != RECDEL:
+            if self.verbose &gt; 0:
                 print(&#34; Damaged data (sig) &#39;%s&#39; at&#34; % sig, rec)
             return arr
 
         hash = self.getbuffint(rec+4)
         blen = self.getbuffint(rec+8)
         data = self.getbuffstr(rec + 12, blen)
 
-        if base_integrity:
+        if self.integrity:
             ccc = self.hash32(data)
-            if self.base_verbose &gt; 1:
+            if self.verbose &gt; 1:
                 print(&#34;rec&#34;, rec, &#34;hash&#34;, hex(hash), &#34;check&#34;, hex(ccc))
             if hash != ccc:
-                if self.base_verbose &gt; 0:
+                if self.verbose &gt; 0:
                     print(&#34;Error on hash at rec&#34;, rec, &#34;hash&#34;, hex(hash), &#34;check&#34;, hex(ccc))
                 return []
 
         #print(&#34;%5d pos %5d&#34; % (cnt, rec), &#34;hash %8x&#34; % hash, &#34;ok&#34;, ok, &#34;len=&#34;, blen, end=&#34; &#34;)
 
         endd = self.getbuffstr(rec + 12 + blen, self.INTSIZE)
         if endd != RECSEP:
-            if self.base_verbose &gt; 0:
+            if self.verbose &gt; 0:
                 print(&#34; Damaged data (sep) &#39;%s&#39; at&#34; % endd, rec)
             return arr
 
         rec2 = rec + 16 + blen;
         hash2 = self.getbuffint(rec2)
         blen2 = self.getbuffint(rec2+4)
         data2 = self.getbuffstr(rec2+8, blen2)
 
-        if base_integrity:
+        if self.integrity:
             ccc2 = self.hash32(data2)
-            if self.base_verbose &gt; 1:
+            if self.verbose &gt; 1:
                 print(&#34;rec&#34;, rec, &#34;hash2&#34;, hex(hash2), &#34;check2&#34;, hex(ccc2))
             if hash2 != ccc2:
-                if self.base_verbose &gt; 0:
+                if self.verbose &gt; 0:
                     print(&#34;Error on hash at rec&#34;, rec, &#34;hash2&#34;, hex(hash2), &#34;check2&#34;, hex(ccc2))
                 return []
 
-        arr = [data, data2]
+        if sig == RECDEL:
+            if self.showdel:
+                arr = [b&#34;del&#34;, data, data2]
+            else:
+                arr = []
+        else:
+            arr = [data, data2]
         return arr
 
     # -------------------------------------------------------------------
     # Originator, dump single record
 
     def  dump_rec(self, rec, cnt):
 
@@ -1740,90 +1745,90 @@
 
         cnt2 = 0
         sig = self.getbuffstr(rec, self.INTSIZE)
         if self.pgdebug &gt; 5:
             print(&#34;Sig &#34;, sig, &#34;at&#34;, rec)
 
         if sig == RECDEL:
-            if base_showdel:
+            if self.showdel:
                 klen = self.getbuffint(rec+8)
                 kdata = self.getbuffstr(rec+12, klen)
                 rec2 = rec + 16 + klen;
                 blen = self.getbuffint(rec2+4)
                 data = self.getbuffstr(rec2+8, blen)
                 print(&#34; Del at&#34;, rec, &#34;key:&#34;, kdata, &#34;data:&#34;, truncs(data))
-            if self.base_verbose &gt; 1:
+            if self.verbose &gt; 1:
                 klen = self.getbuffint(rec+8)
                 kdata = self.getbuffstr(rec+12, klen)
                 rec2 = rec + 16 + klen;
                 blen = self.getbuffint(rec2+4)
                 data = self.getbuffstr(rec2+8, blen)
-                if self.base_verbose &gt; 2:
+                if self.verbose &gt; 2:
                     print(&#34; Del at&#34;, rec, &#34;key:&#34;, kdata, &#34;data:&#34;, data)
                 else:
                     print(&#34; Del at&#34;, rec, &#34;key:&#34;, kdata, &#34;data:&#34;, truncs(data))
 
             return cnt2
 
         if sig != RECSIG:
-            if self.base_verbose &gt; 1:
+            if self.verbose &gt; 1:
                 print(&#34; Damaged data (sig) &#39;%s&#39; at&#34; % sig, rec)
             return cnt2
 
         hash = self.getbuffint(rec+4)
         blen = self.getbuffint(rec+8)
 
         if blen &lt; 0:
-            if self.base_verbose &gt; 2:
+            if self.verbose &gt; 2:
                 print(&#34;Invalid key length %d at %d&#34; % (blen, rec))
             return cnt2
 
         data = self.getbuffstr(rec+12, blen)
-        if base_integrity:
+        if self.integrity:
             ccc = self.hash32(data)
-            if self.base_verbose &gt; 1:
+            if self.verbose &gt; 1:
                 print(&#34;rec&#34;, rec, &#34;hash&#34;, hex(hash), &#34;check&#34;, hex(ccc))
             if hash != ccc:
-                if self.base_verbose &gt; 0:
+                if self.verbose &gt; 0:
                     print(&#34;Error on hash at rec&#34;, rec, &#34;hash&#34;, hex(hash), &#34;check&#34;, hex(ccc))
                 return []
 
         endd = self.getbuffstr(rec + 12 + blen, self.INTSIZE)
         if endd != RECSEP:
-            if self.base_verbose &gt; 0:
+            if self.verbose &gt; 0:
                 print(&#34; Damaged data (sep) &#39;%s&#39; at&#34; % endd, rec)
             return cnt2
 
         rec2 = rec + 16 + blen;
         hash2 = self.getbuffint(rec2)
         blen2 = self.getbuffint(rec2+4)
 
         if blen2 &lt; 0:
-            if self.base_verbose &gt; 1:
+            if self.verbose &gt; 1:
                 print(&#34;Invalid data length %d at %d&#34; % (blen2, rec))
             return cnt2
 
         data2 = self.getbuffstr(rec2+8, blen2)
-        if base_integrity:
+        if self.integrity:
             ccc2 = self.hash32(data2)
-            if self.base_verbose &gt; 1:
+            if self.verbose &gt; 1:
                 print(&#34;rec&#34;, rec, &#34;hash2&#34;, hex(hash), &#34;check2&#34;, hex(ccc))
             if hash2 != ccc2:
-                if self.base_verbose &gt; 0:
+                if self.verbose &gt; 0:
                     print(&#34;Error on hash at rec&#34;, rec, &#34;hash2&#34;, hex(hash), &#34;check2&#34;, hex(ccc))
                 return []
 
-        if self.base_verbose &gt; 2:
+        if self.verbose &gt; 2:
             print(&#34;%-5d pos %5d&#34; % (cnt, rec), &#34;%8x&#34; % hash, &#34;len&#34;, blen, data,
                                                         &#34;%8x&#34; % hash2,&#34;len&#34;, blen2, data2)
 
-        elif self.base_verbose &gt; 1:
+        elif self.verbose &gt; 1:
             print(&#34;%-5d pos %5d&#34; % (cnt, rec), &#34;%8x&#34; % hash, &#34;len&#34;, blen, data,
                                                         &#34;%8x&#34; % hash2,&#34;len&#34;, blen2, data2)
-        elif self.base_verbose:
+        elif self.verbose:
             print(&#34;%-5d pos %5d&#34; % (cnt, rec),  data, data2)
         else:
             print(&#34;%-5d pos %5d&#34; % (cnt, rec), &#34;Data:&#34;, truncs(data, 18), &#34;Data2:&#34;, truncs(data2, 18))
 
         cnt2 += 1
         return cnt2
 
@@ -1832,72 +1837,72 @@
         &#39;&#39;&#39; Check record. Verbose to the screen. Return number of errors.&#39;&#39;&#39;
 
         ret = 0
         sig = self.getbuffstr(rec, self.INTSIZE)
 
         # Do not check deleted, say OK
         if sig == RECDEL:
-            if self.base_verbose &gt; 1:
+            if self.verbose &gt; 1:
                 print(&#34; Deleted data &#39;%s&#39; at %d (%d)&#34; % (sig, rec, cnt2))
             ret = 1
             return ret
 
         if sig != RECSIG:
-            if self.base_verbose &gt; 0:
+            if self.verbose &gt; 0:
                 print(&#34; Damaged data (sig) &#39;%s&#39; at %d (%d)&#34; % (sig, rec, cnt2))
-            #if self.base_verbose &gt; 1:
+            #if self.verbose &gt; 1:
             #    print(&#34;Data&#34;, data)
 
             return ret
 
         hash = self.getbuffint(rec+4)
         blen = self.getbuffint(rec+8)
 
         if blen &lt;= 0:
-            if self.base_verbose &gt; 1:
+            if self.verbose &gt; 1:
                 print(&#34;Invalid key length %d at %d&#34; % (blen, rec))
             return ret
 
         data = self.getbuffstr(rec+12, blen)
         ccc = self.hash32(data)
         if hash != ccc:
-            if self.base_verbose &gt; 1:
+            if self.verbose &gt; 1:
                 print(&#34;Data&#34;, data)
-            elif self.base_verbose &gt; 0:
+            elif self.verbose &gt; 0:
                 print(&#34;Error on hash at rec&#34;, rec, cnt2, &#34;hash&#34;,
                                             hex(hash), &#34;check&#34;, hex(ccc))
 
             return ret
 
         endd = self.getbuffstr(rec + 12 + blen, self.INTSIZE)
         if endd != RECSEP:
-            if self.base_verbose &gt; 0:
+            if self.verbose &gt; 0:
                 print(&#34; Damaged data (sep) &#39;%s&#39; at %d %d %d&#34; % (endd, rec, cnt2))
             return ret
 
         rec2 = rec + 16 + blen;
         hash2 = self.getbuffint(rec2)
         blen2 = self.getbuffint(rec2+4)
 
         if blen2 &lt; 0:
-            if self.base_verbose &gt; 1:
+            if self.verbose &gt; 1:
                 print(&#34;Invalid data length2 %d at %d&#34; % (blen2, rec))
             return ret
 
         data2 = self.getbuffstr(rec2+8, blen2)
         ccc2 = self.hash32(data2)
         if hash2 != ccc2:
-            if self.base_verbose &gt; 1:
+            if self.verbose &gt; 1:
                 print(&#34;Data&#34;, data, &#34;Data2&#34;, data2)
-            elif self.base_verbose &gt; 0:
+            elif self.verbose &gt; 0:
                 print(&#34;Error on hash2 at rec&#34;, rec, cnt2, &#34;hash2&#34;,
                                         hex(hash2), &#34;check2&#34;, hex(ccc2))
             return ret
 
-        if self.base_verbose &gt; 2:
+        if self.verbose &gt; 2:
             print(&#34;Record at %d (%d) OK.&#34; % (rec, cnt2))
 
         ret += 1
         return ret
 
     # --------------------------------------------------------------------
     # Internal; no locking
@@ -1918,26 +1923,23 @@
         else:
             rrr = range(chash - self.INTSIZE * 2, HEADSIZE  - self.INTSIZE * 2, -self.INTSIZE * 2)
 
         for aa in rrr:
             rec = self.getidxint(aa)
 
             #print(aa, rec)
-            if not base_quiet:
-                cnt2 += 1
-                ret = self.dump_rec(rec, cnt)
-
-                if not ret:
-                    if self.pgdebug &gt; 5:
-                        print(&#34;Deleted / empty record at&#34;, cnt)
-
-                if ret:
-                    cnt += 1
-                    if cnt &gt;= lim:
-                        break
+            cnt2 += 1
+            ret = self.dump_rec(rec, cnt)
+            if not ret:
+                if self.pgdebug &gt; 5:
+                    print(&#34;Deleted / empty record at&#34;, cnt)
+            if ret:
+                cnt += 1
+                if cnt &gt;= lim:
+                    break
 
     def  dump_data(self, lim = INT_MAX, skip = 0):
 
         &#39;&#39;&#39; Put all data to screen. &#39;&#39;&#39;
 
         self.__dump_data(lim, skip, 1)
 
@@ -1947,17 +1949,17 @@
 
         self.__dump_data(lim, skip)
 
     def  reindex(self):
 
         &#39;&#39;&#39; Re create index file. &#39;&#39;&#39;
 
-        self.lock.waitlock() #self.lckname)
+        self.lock.waitlock()
         ret = self.__reindex()
-        self.lock.unlock()    #dellock(self.lckname)
+        self.lock.unlock()
         return ret
 
     # --------------------------------------------------------------------
 
     def  __reindex(self):
 
         &#39;&#39;&#39; Recover index. Make sure the DB in not in session.  &#39;&#39;&#39;
@@ -1978,50 +1980,50 @@
         tmplock = FileLock(relock)
         tmplock.waitlock()
 
         tempifp = self.softcreate(reidx)
         self.create_idx(tempifp)
         dlen = self.getsize(self.fp)
 
-        if self.base_verbose &gt; 2:
+        if self.verbose &gt; 2:
            print(&#34;curr&#34;, curr, &#34;dlen&#34;, dlen)
 
         aa =  HEADSIZE
         while 1:
             if aa &gt;= dlen:
                 break
 
             sig = self.getbuffstr(aa, self.INTSIZE)
             # Check if sig is correct
             if sig != RECSIG:
-                if self.core_verbose &gt; 0:
+                if self.verbose &gt; 0:
                     print(&#34;Invalid sig .. resync needed&#34;)
                 raise
 
             #print(&#34;reind&#34;, aa)
 
             try:
                 hhh2 = self.getbuffint(aa + 4)
                 lenx = self.getbuffint(aa + 8)
                 if lenx &lt; 0:
-                    if self.core_verbose &gt; 0:
+                    if self.verbose &gt; 0:
                         print(&#34;Invalid key length.&#34;)
                 sep =  self.getbuffstr(aa + 12 + lenx, self.INTSIZE)
                 len2 =  self.getbuffint(aa + 20 + lenx)
                 if len2 &lt; 0:
-                    if self.core_verbose &gt; 0:
+                    if self.verbose &gt; 0:
                         print(&#34;Invalid record length&#34;)
             except:
-                if self.core_verbose &gt; 2:
+                if self.verbose &gt; 2:
                     print(&#34;in reindex&#34;, sys.exc_info())
 
-            if self.base_verbose == 1:
+            if self.verbose == 1:
                 print(aa, &#34;sig&#34;, sig, &#34;hhh2&#34;, hex(hhh2), &#34;len&#34;, lenx, \
                     &#34;sep&#34;, sep, &#34;len2&#34;, len2)
-            if self.base_verbose &gt; 1:
+            if self.verbose &gt; 1:
                 data =  self.getbuffstr(aa + 12, lenx)
                 data2 =  self.getbuffstr(aa + 24 + lenx, len2)
                 print(aa, &#34;sig&#34;, sig, &#34;data&#34;, data, &#34;data2&#34;, data2)
 
             # Update / Append index
             #hashpos = self._getint(tempifp, CURROFFS)
             hashpos =  HEADSIZE  + self._getdbsize(tempifp) * self.INTSIZE * 2
@@ -2094,17 +2096,17 @@
         &#39;&#39;&#39;
             Remove all deleted data. Reindex.
             The db is locked while the vacuum is in operation, but
             make sure the DB in not in session, and no pending
             operations are present (like find / retrieve cycle).
         &#39;&#39;&#39;
 
-        self.lock.waitlock() #self.lckname)
+        self.lock.waitlock()
         ret = self._vacuum()
-        self.lock.unlock()  #dellock(self.lckname)
+        self.lock.unlock()
         return ret
 
     def  _vacuum(self):
 
         vacname = os.path.splitext(self.fname)[0] + &#34;_vac_&#34; + &#34;.pydb&#34;
         vacerr  = os.path.splitext(self.fname)[0] +  &#34;.perr&#34;
         vacidx = os.path.splitext(vacname)[0]  + &#34;.pidx&#34;
@@ -2140,24 +2142,21 @@
                 sig = self.getbuffstr(rec, self.INTSIZE)
                 if sig == RECDEL:
                     ret += 1
                     vac += 1
                     if self.pgdebug &gt; 1:
                         print(&#34;deleted&#34;, rec)
                 elif sig != RECSIG:
-                    if self.base_verbose:
+                    if self.verbose:
                         print(&#34;Detected error at %d&#34; % rec)
                     ret += 1
                     self.__save_error(rec, vacerrfp)
                 else:
-                    global base_integrity
-                    tmpi = base_integrity
-                    base_integrity = True
+                    self.integrity = True
                     arr = self.get_rec_byoffs(rec)
-                    base_integrity = tmpi
 
                     if self.pgdebug &gt; 1:
                         print(cnt, &#34;vac rec&#34;, rec, arr)
 
                     if len(arr) &gt; 1:
                         hhh2 = self.hash32(arr[0])
                         hhh3 = self.hash32(arr[1])
@@ -2169,103 +2168,103 @@
                         if self.pgdebug &gt; 0:
                             print(&#34;Error on vac: %d&#34; % rec)
                 cnt += 1
 
             vacdb.fp.close()
             vacdb.ifp.close()
 
-            vacdb.lock.unlock()  #dellock(vacdb.lckname)
+            vacdb.lock.unlock()
 
             # if vacerr is empty
             try:
                 if os.stat(vacerr).st_size == 0:
                     #print(&#34;Vac error empty&#34;)
                     os.remove(vacerr)
             except:
-                if self.core_verbose &gt; 0:
+                if self.verbose &gt; 0:
                     print(&#34;vacerr&#34;, sys.exc_info())
 
         # Any vacummed?
         if vac &gt; 0:
             # Make it go out of scope
             self.fp.flush(); self.ifp.flush()
             self.fp.close(); self.ifp.close()
 
             # Now move files
             try:
                 os.remove(self.fname);
             except:
-                if self.core_verbose &gt; 0:
+                if self.verbose &gt; 0:
                     print(&#34;vacuum remove&#34;, self.fname, sys.exc_info())
                 pass
 
             try:
                 os.remove(self.idxname)
             except:
-                if self.core_verbose &gt; 2:
+                if self.verbose &gt; 2:
                     print(&#34;vacuum idx remove&#34;, self.idxname, sys.exc_info())
                 pass
 
             if self.pgdebug &gt; 1:
                 print(&#34;rename&#34;, vacname, &#34;-&gt;&#34;, self.fname)
                 print(&#34;rename&#34;, vacidx, &#34;-&gt;&#34;, self.idxname)
 
             try:
                 os.rename(vacname, self.fname)
             except:
-                if self.core_verbose &gt; 2:
+                if self.verbose &gt; 2:
                     print(&#34;vacuum rename&#34;, vacname, sys.exc_info())
             try:
                 os.rename(vacidx, self.idxname)
             except:
-                if self.core_verbose &gt; 2:
+                if self.verbose &gt; 2:
                     print(&#34;vacuum idx rename&#34;, vacidx, sys.exc_info())
 
-            self.lock.waitlock() #self.lckname)
+            self.lock.waitlock()
             self.fp = self.softcreate(self.fname)
             self.ifp = self.softcreate(self.idxname)
-            #self.lock.unlock()  #dellock(self.lckname)
+            #self.lock.unlock()
 
         else:
             # Just remove non vacuumed files
             if self.pgdebug &gt; 1:
                 print(&#34;deleted&#34;, vacname, vacidx)
             try:
                 os.remove(vacname)
                 os.remove(vacidx)
             except:
                 pass
 
         #self.lock.unlock()
-        #dellock(self.lckname)
+
 
         #print(&#34;ended vacuum&#34;)
         return ret, vac
 
     def  get_rec(self, recnum):
 
         &#39;&#39;&#39; Get record from database; recnum is a zero based record counter. &#39;&#39;&#39;
 
         if self.pgdebug:
-            print(&#34;getrec()&#34;, recnum)
+            print(&#34;get_rec()&#34;, recnum)
 
         rsize = self._getdbsize(self.ifp)
         if recnum &gt;= rsize:
-            if self.core_verbose &gt; 0:
+            if self.verbose &gt; 0:
                 print(&#34;Past end of data.&#34;);
-            raise  RuntimeError( \
-                    &#34;Past end of Data. Asking for %d while max is 0 .. %d records.&#34; \
-                                     % (recnum, rsize-1) )
+            errx =  &#34;Past end of Data. (ask: %d max: %d)&#34;  % (recnum, rsize-1)
+            raise  RuntimeError(errx)
             return []
 
         chash = self.getidxint(CURROFFS)
         #print(&#34;chash&#34;, chash)
         offs = self.getidxint(HEADSIZE + recnum * self.INTSIZE * 2)
 
-        #print(&#34;offs&#34;, offs)
+        #sig = self.getbuffstr(offs, self.INTSIZE)
+
         return self._rec2arr(offs)
 
     def  get_rec_byoffs(self, recoffs):
 
         &#39;&#39;&#39; Return record by offset. &#39;&#39;&#39;
 
         rsize = self.getsize(self.fp)
@@ -2274,19 +2273,18 @@
             raise  RuntimeError( \
                     &#34;Past end of File. Asking for offset %d file size is %d.&#34; \
                                      % (recoffs, rsize) )
             return []
 
         sig = self.getbuffstr(recoffs, self.INTSIZE)
         if sig == RECDEL:
-            if self.base_verbose:
+            if self.verbose:
                 print(&#34;Deleted record.&#34;)
-            return []
         if sig != RECSIG:
-            if self.core_verbose &gt; 0:
+            if self.verbose &gt; 0:
                 print(&#34;Unlikely offset %d is not at record boundary.&#34; % recoffs, sig)
             return []
         #print(&#34;recoffs&#34;, recoffs)
         return self._rec2arr(recoffs)
 
     def  get_key_offs(self, recoffs):
 
@@ -2298,19 +2296,19 @@
             raise  RuntimeError( \
                     &#34;Past end of File. Asking for offset %d file size is %d.&#34; \
                                      % (recoffs, rsize) )
             return []
 
         sig = self.getbuffstr(recoffs, self.INTSIZE)
         if sig == RECDEL:
-            if self.base_verbose:
+            if self.verbose:
                 print(&#34;Deleted record.&#34;)
             return []
         if sig != RECSIG:
-            if self.core_verbose &gt; 0:
+            if self.verbose &gt; 0:
                 print(&#34;Unlikely offset %d is not at record boundary.&#34; % recoffs, sig)
             return []
         #print(&#34;recoffs&#34;, recoffs)
         return self._rec2arr(recoffs)[0]
 
     def  del_rec(self, recnum):
 
@@ -2318,24 +2316,24 @@
             Deleted record is marked as deleted but not removed.
             Deleted records are ignored in further operations.
             Use &#39;vacuum&#39; to actually remove record.
         &#39;&#39;&#39;
 
         rsize = self._getdbsize(self.ifp)
         if recnum &gt;= rsize:
-            if self.base_verbose:
+            if self.verbose:
                 print(&#34;Past end of data.&#34;);
             return False
         chash = self.getidxint(CURROFFS)
         #print(&#34;chash&#34;, chash)
         offs = self.getidxint(HEADSIZE + recnum * self.INTSIZE * 2)
         #print(&#34;offs&#34;, offs)
         old = self.getbuffstr(offs, self.INTSIZE)
         if old == RECDEL:
-            if self.base_verbose:
+            if self.verbose:
                 print(&#34;Record at %d already deleted.&#34; % offs);
             return False
 
         self.putbuffstr(offs, RECDEL)
         return True
 
     def  del_rec_offs(self, recoffs):
@@ -2348,44 +2346,44 @@
             raise  RuntimeError( \
                     &#34;Past end of File. Asking for offset %d file size is %d.&#34; \
                                      % (recoffs, rsize) )
             return False
 
         sig = self.getbuffstr(recoffs, self.INTSIZE)
         if sig != RECSIG  and sig != RECDEL:
-            if self.core_verbose &gt; 0:
+            if self.verbose &gt; 0:
                 print(&#34;Unlikely offset %d is not at record boundary.&#34; % recoffs, sig)
             return False
 
         self.putbuffstr(recoffs, RECDEL)
         return True
 
     # Check integrity
 
     def integrity_check(self, skip = 0, count = 0xffffffff):
 
         &#39;&#39;&#39; Check record integrity for &#39;count&#39; records.
             Skip number of records.
         &#39;&#39;&#39;
 
-        self.lock.waitlock()    #(self.lckname)
+        self.lock.waitlock()
         ret = 0; cnt2 = 0; cnt3 = 0;
         #chash = self.getidxint(CURROFFS)        #;print(&#34;chash&#34;, chash)
         chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
         # Direction sensitivity
         rrr = range(HEADSIZE + skip * self.INTSIZE * 2, chash, self.INTSIZE * 2)
         for aa in rrr:
             rec = self.getidxint(aa)
             #print(aa, rec)
             ret += self.check_rec(rec, cnt2)
             cnt2 += 1
             cnt3 += 1
             if cnt3 &gt;= count:
                 break
-        self.lock.unlock() #dellock(self.lckname)
+        self.lock.unlock()
         return ret, cnt2
 
     def  retrieve(self, strx, limx = 1):
 
         &#39;&#39;&#39; Retrive in reverse, limit it. &#39;&#39;&#39;
 
         if type(strx) != type(b&#34;&#34;):
@@ -2397,33 +2395,33 @@
 
         #chash = self.getidxint(CURROFFS)
         chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
 
         #;print(&#34;chash&#34;, chash)
         arr = []
 
-        self.lock.waitlock() #(self.lckname)
+        self.lock.waitlock()
 
         #for aa in range(HEADSIZE + self.INTSIZE * 2, chash, self.INTSIZE * 2):
         for aa in range(chash - self.INTSIZE * 2, HEADSIZE  - self.INTSIZE * 2, -self.INTSIZE * 2):
             rec = self.getidxint(aa)
             sig = self.getbuffstr(rec, self.INTSIZE)
             if sig == RECDEL:
-                if self.base_verbose &gt; 3:
+                if self.verbose &gt; 3:
                     print(&#34; Deleted record &#39;%s&#39; at&#34; % sig, rec)
             elif sig != RECSIG:
-                if self.base_verbose:
+                if self.verbose:
                     print(&#34; Damaged data &#39;%s&#39; at&#34; % sig, rec)
             else:
                 hhh = self.getbuffint(rec+4)
                 if hhh == hhhh:
                     arr.append(self.get_rec_byoffs(rec))
                     if len(arr) &gt;= limx:
                         break
-        self.lock.unlock()  #dellock(self.lckname)
+        self.lock.unlock()
 
         return arr
 
     # Return record offset
 
     def  _recoffset(self, strx, limx = INT_MAX, skipx = 0):
 
@@ -2440,151 +2438,153 @@
         #print(&#34;_recoffset&#34;, strx2)
 
         #for aa in range(HEADSIZE + self.INTSIZE * 2, chash, self.INTSIZE * 2):
         for aa in range(chash - self.INTSIZE * 2, HEADSIZE  - self.INTSIZE * 2, -self.INTSIZE * 2):
             rec = self.getidxint(aa)
             sig = self.getbuffstr(rec, self.INTSIZE)
             if sig == RECDEL:
-                if base_showdel:
+                if self.showdel:
                     print(&#34; Deleted record &#39;%s&#39; at&#34; % sig, rec)
             elif sig != RECSIG:
-                if self.base_verbose &gt; 0:
+                if self.verbose &gt; 0:
                     print(&#34; Damaged data &#39;%s&#39; at&#34; % sig, rec)
             else:
                 blen = self.getbuffint(rec+8)
                 keyz = self.getbuffstr(rec + 12, blen)
-                if self.base_verbose &gt; 1:
+                if self.verbose &gt; 1:
                     print(&#34;_recoffset&#34;, keyz)
                 if strx2 == keyz:
                     sig = self.getbuffstr(rec + 16 + blen,  self.INTSIZE)
                     xlen = self.getbuffint(rec + 20 + blen)
                     data = self.getbuffstr(rec + 24 + blen, xlen)
                     #print(&#34;rec offset&#34;, rec + 12,  &#34;key:&#34;, keyz, &#34;data:&#34;, data)
                     break       # Only the last one
         return rec, rec+24 + blen, len(data)
 
     def  findrec(self, strx, limx = INT_MAX, skipx = 0):
 
-        &#39;&#39;&#39; Find by string matching substring. &#39;&#39;&#39;
+        &#39;&#39;&#39; Find key by matching strx with substring.
+        Return record(s).
+        &#39;&#39;&#39;
 
-        self.lock.waitlock()    #(self.lckname)
+        self.lock.waitlock()
 
         #chash = self.getidxint(CURROFFS)            #;print(&#34;chash&#34;, chash)
         chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
 
         arr = []
         strx2 = strx.encode(errors=&#39;strict&#39;);
 
         #print(&#34;findrec&#34;, strx2)
 
         #for aa in range(HEADSIZE + self.INTSIZE * 2, chash, self.INTSIZE * 2):
         for aa in range(chash - self.INTSIZE * 2, HEADSIZE  - self.INTSIZE * 2, -self.INTSIZE * 2):
             rec = self.getidxint(aa)
             sig = self.getbuffstr(rec, self.INTSIZE)
             if sig == RECDEL:
-                if base_showdel:
+                if self.showdel:
                     print(&#34; Deleted record &#39;%s&#39; at&#34; % sig, rec)
             elif sig != RECSIG:
-                if self.base_verbose &gt; 0:
+                if self.verbose &gt; 0:
                     print(&#34; Damaged data &#39;%s&#39; at&#34; % sig, rec)
             else:
                 blen = self.getbuffint(rec+8)
                 data = self.getbuffstr(rec + 12, blen)
-                if self.base_verbose &gt; 1:
+                if self.verbose &gt; 1:
                     print(&#34;find&#34;, data)
                 #if str(strx2) in str(data):
                 if strx2 in data:
                     arr.append(self.get_key_offs(rec))
                     #arr.append(rec)
 
                     if len(arr) &gt;= limx:
                         break
-        self.lock.unlock()  #dellock(self.lckname)
+        self.lock.unlock()
 
         return arr
 
     def  findrecpos(self, strx, limx = INT_MAX, skipx = 0):
 
-        &#39;&#39;&#39; Find record, return array of positions. &#39;&#39;&#39;
+        &#39;&#39;&#39; Find record by key, return array of positions. &#39;&#39;&#39;
 
-        self.lock.waitlock()    #(self.lckname)
+        self.lock.waitlock()
         chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
         arr = []
         if type(strx) != type(b&#34;&#34;):
             strx = strx.encode(errors=&#39;strict&#39;);
 
         for aa in range(chash - self.INTSIZE * 2, HEADSIZE  - self.INTSIZE * 2, -self.INTSIZE * 2):
             rec = self.getidxint(aa)
             sig = self.getbuffstr(rec, self.INTSIZE)
             if sig == RECDEL:
-                if base_showdel:
+                if self.showdel:
                     print(&#34; Deleted record &#39;%s&#39; at&#34; % sig, rec)
             elif sig != RECSIG:
-                if self.base_verbose &gt; 0:
+                if self.verbose &gt; 0:
                     print(&#34; Damaged data &#39;%s&#39; at&#34; % sig, rec)
             else:
                 blen = self.getbuffint(rec+8)
                 data = self.getbuffstr(rec + 12, blen)
-                if self.base_verbose &gt; 1:
+                if self.verbose &gt; 1:
                     print(&#34;frecpos&#34;, data)
                 if strx == data:
                     arr.append(rec)
                     if len(arr) &gt;= limx:
                         break
 
-        self.lock.unlock()  #dellock(self.lckname)
+        self.lock.unlock()
 
         return arr
 
-    def  findrec(self, strx, limx = INT_MAX, skipx = 0):
+    def  findrecsub(self, strx, limx = INT_MAX, skipx = 0):
 
-        &#39;&#39;&#39; Find by string matching substring. &#39;&#39;&#39;
+        &#39;&#39;&#39; Find record by matching substring. &#39;&#39;&#39;
 
-        self.lock.waitlock()    #(self.lckname)
+        self.lock.waitlock()
         chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
         arr = []
         if type(strx) != type(b&#34;&#34;):
             strx2 = strx.encode(errors=&#39;strict&#39;);
 
         #print(&#34;findrec&#34;, strx2)
 
         #for aa in range(HEADSIZE + self.INTSIZE * 2, chash, self.INTSIZE * 2):
         for aa in range(chash - self.INTSIZE * 2, HEADSIZE  - self.INTSIZE * 2, -self.INTSIZE * 2):
             rec = self.getidxint(aa)
             sig = self.getbuffstr(rec, self.INTSIZE)
             if sig == RECDEL:
-                if base_showdel:
+                if self.showdel:
                     print(&#34; Deleted record &#39;%s&#39; at&#34; % sig, rec)
             elif sig != RECSIG:
-                if self.base_verbose &gt; 0:
+                if self.verbose &gt; 0:
                     print(&#34; Damaged data &#39;%s&#39; at&#34; % sig, rec)
             else:
                 blen = self.getbuffint(rec+8)
                 data = self.getbuffstr(rec + 12, blen)
-                if self.base_verbose &gt; 1:
+                if self.verbose &gt; 1:
                     print(&#34;find&#34;, data)
                 #if str(strx2) in str(data):
                 if strx2 in data:
                     #arr.append(self.get_key_offs(rec))
                     #arr.append(rec)
                     arr.append(self._rec2arr(rec))
                     if len(arr) &gt;= limx:
                         break
-        self.lock.unlock()    #dellock(self.lckname)
+        self.lock.unlock()
 
         return arr
 
     # --------------------------------------------------------------------
     # List all active records
 
     def  listall(self):
 
         &#39;&#39;&#39; List all active records. Return array id record indexes. &#39;&#39;&#39;
 
-        self.lock.waitlock()    #(self.lckname)
+        self.lock.waitlock()
         keys = []; arr = []; cnt = 0
 
         chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
         maxrec = chash - self.INTSIZE * 2
         rsize = self._getdbsize(self.ifp) - 1
 
         rrr =  range(maxrec,
@@ -2592,39 +2592,42 @@
         for aa in rrr:
             rec = self.getidxint(aa)
 
             #print(&#34; Scanning at %d %d&#34; % (rec, cnt))
 
             sig = self.getbuffstr(rec, self.INTSIZE)
             if sig == RECDEL:
-                if 1: #base_showdel:
+                if 1: #self.showdel:
                     print(&#34;Deleted record &#39;%s&#39; at&#34; % sig, rec)
             elif sig != RECSIG:
-                if 1: #self.base_verbose &gt; 0:
+                if 1: #self.verbose &gt; 0:
                     print(&#34; Damaged data &#39;%s&#39; at&#34; % sig, rec)
             else:
                     hhh = self.getbuffint(rec+4)
                     print(&#34; Good data &#39;%s&#39; at&#34; % sig, rec, hhh)
                     if hhh not in keys:
                         keys.append(hhh)
                         # as we are going backwards
                         arr.append(rsize - cnt)
                         #print(&#34;found&#34;, hhh)
             cnt += 1
 
         keys = []
-        self.lock.unlock()  #dellock()self.lckname)
+        self.lock.unlock()
 
         return arr
 
     def  find_key(self, keyx, limx = 0xffffffff):
 
-        &#39;&#39;&#39; Find record by key Search from the end, so latest comes first. &#39;&#39;&#39;
+        &#39;&#39;&#39; Find record by key value.
+            Search from the end, so latest comes first.
+            This operates on the hash, so it reaches the answer fast.
+        &#39;&#39;&#39;
 
-        self.lock.waitlock()   #self.lckname)
+        self.lock.waitlock()
 
         skip = 0; arr = []; cnt = 0
         try:
             arg2e = keyx.encode()
         except:
             arg2e = keyx
 
@@ -2636,32 +2639,32 @@
                 HEADSIZE - self.INTSIZE * 2, -self.INTSIZE * 2)
         for aa in rrr:
             rec = self.getidxint(aa)
             #print(&#34; Scanning at %d %d&#34; % (rec, cnt))
 
             sig = self.getbuffstr(rec, self.INTSIZE)
             if sig == RECDEL:
-                if base_showdel:
+                if self.showdel:
                     print(&#34;Deleted record &#39;%s&#39; at&#34; % sig, rec)
             elif sig != RECSIG:
-                if self.base_verbose &gt; 0:
+                if self.verbose &gt; 0:
                     print(&#34; Damaged data &#39;%s&#39; at&#34; % sig, rec)
             else:
                 hhh = self.getbuffint(rec+4)
                 if hhh == hhhh:
                     if len(arr) &gt;= limx - 1:
                         arr.append([&#34;More data ...&#34;,])
                         break
                     arr.append(rec)
                 else:
                     pass
                     #print(&#34;no match&#34;, hex(hhh))
 
             cnt += 1
-        self.lock.unlock()  #dellock()self.lckname)
+        self.lock.unlock()
 
         return arr
 
 
     def  del_data(self, hash, skip = 1):
 
         &#39;&#39;&#39; Delete data by hash. &#39;&#39;&#39;
@@ -2681,15 +2684,15 @@
             #    print(&#34; Damaged data &#39;%s&#39; at&#34; % sig, rec)
 
             #blen = self.getbuffint(rec+8)
             #print(&#34;data &#39;%s&#39; at&#34; % sig, rec, &#34;blen&#34;, blen)
 
             hhh = self.getbuffint(rec+4)
             if hash == hhh:
-                if self.base_verbose &gt; 0:
+                if self.verbose &gt; 0:
                     print(&#34;Would delete&#34;, hhh)
 
             self.putbuffstr(rec, RECDEL)
 
             cnt += 1
 
         return arr
@@ -2714,15 +2717,15 @@
         &#39;&#39;&#39; Delete records by key string; needs bin str, converted
             automatically on entry.
         &#39;&#39;&#39;
 
         if type(strx) != type(b&#34;&#34;):
             strx = strx.encode()
 
-        if self.base_verbose &gt; 1:
+        if self.verbose &gt; 1:
             print(&#34;Start delete &#34;, strx, &#34;skip&#34;, skip)
 
         cnt = 0; cnt3 = 0
         #chash = self.getidxint(CURROFFS)    #;print(&#34;chash&#34;, chash)
         chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
 
         # Direction sensitivity
@@ -2732,58 +2735,58 @@
             rrr = range(chash - self.INTSIZE * 2, HEADSIZE  - self.INTSIZE * 2, -self.INTSIZE * 2)
 
         #for aa in range(HEADSIZE, chash, self.INTSIZE * 2):
         for aa in rrr:
             rec = self.getidxint(aa)
             sig = self.getbuffstr(rec, self.INTSIZE)
             if sig == RECDEL:
-                if base_showdel:
+                if self.showdel:
                     print(&#34; Deleted record &#39;%s&#39; at&#34; % sig, rec)
             elif sig != RECSIG:
-                if self.base_verbose &gt; 0:
+                if self.verbose &gt; 0:
                     print(&#34; Damaged data &#39;%s&#39; at&#34; % sig, rec)
             else:
                 blen = self.getbuffint(rec+8)
                 data = self.getbuffstr(rec + 12, blen)
-                if self.base_verbose &gt; 2:
+                if self.verbose &gt; 2:
                     print(&#34;del iterate recs&#34;, cnt3, data, strx)
 
                 if strx == data:
-                    if self.base_verbose &gt; 0:
+                    if self.verbose &gt; 0:
                         print(&#34;Deleting&#34;, cnt3, aa, data)
                     self.putbuffstr(rec, RECDEL)
                     cnt += 1
                     if cnt &gt;= maxdelrec:
                         break
             cnt3 += 1
         return cnt
 
     def  save_data(self, header, datax, replace = False):
 
         &#39;&#39;&#39; Append to the end of file. If replace flag is set, try to overwrite
-            in place. If new record is larger, add it as ususal. If smaller,
+            in place. If new record is larger, add it as usual. If smaller,
             the record is padded with spaces. This should not influence most ops.
             (like: int())
             This feature allows the database update wthout creating new records.
-            Useful for counters or dynamically changing data.
+            Useful for counters or dynamically changing data. To be useful,
+            use  create fixed size data. Like sprintf(%12d).
 
                     Input:
                         header     Header
                         datax      Data
 
                      Return:
                         The offset of saved data
             &#39;&#39;&#39;
 
         if self.pgdebug &gt; 0:
             print(&#34;Save_data()&#34;, header, datax)
 
-        self.lock.waitlock()   #self.lckname)
-        ret = 0
-        was = False
+        self.lock.waitlock()
+        ret = 0 ; was = False
         # Put new data in place
         if replace:
             if type(datax) != type(b&#34;&#34;):
                 mrep2 = datax.encode()
             else:
                 mrep2 = datax
 
@@ -2798,17 +2801,18 @@
                     ccc = self.hash32(padded)
                     self.putbuffint(rrr[1] - 8, ccc)
                     #print(&#34;ccc&#34;, hex(ccc))
                     self.putbuffstr(rrr[1], padded)
                     was = True
                     ret =  rrr[0]
         if not was:
+            #print(&#34;Saving longer data&#34;, header, datax)
             ret = self._save_data2(header, datax)
 
-        self.lock.unlock()  #dellock()self.lckname)
+        self.lock.unlock()
 
         return ret
 
     # --------------------------------------------------------------------
     # Save data to database file
 
     def  _save_data2(self, arg2, arg3):
@@ -2873,15 +2877,15 @@
         self.putidxint(curr, dcurr)
         self.putidxint(curr + self.INTSIZE, hhh2)
         #self.putidxint(CURROFFS, self.ifp.tell())
 
         self.fp.flush()
         self.ifp.flush()
 
-        return curr
+        return dcurr
 
     def __del__(self):
 
         &#39;&#39;&#39; flush file handles and close files. &#39;&#39;&#39;
 
         if hasattr(self, &#34;pgdebug&#34;):
             if self.pgdebug &gt; 9:
@@ -2895,15 +2899,19 @@
                         self.fp.flush()
                         self.fp.close()
 
         if hasattr(self, &#34;ifp&#34;):
                 if self.ifp:
                     if not self.ifp.closed:
                         self.ifp.flush()
-                        self.ifp.close()</code></pre>
+                        self.ifp.close()
+
+        # remove lockfile
+        if hasattr(self, &#34;lock&#34;):
+            self.lock.unlock()</code></pre>
 </details>
 <h3>Ancestors</h3>
 <ul class="hlist">
 <li>twinbase.TwinCoreBase</li>
 </ul>
 <h3>Methods</h3>
 <dl>
@@ -2921,72 +2929,72 @@
     &#39;&#39;&#39; Check record. Verbose to the screen. Return number of errors.&#39;&#39;&#39;
 
     ret = 0
     sig = self.getbuffstr(rec, self.INTSIZE)
 
     # Do not check deleted, say OK
     if sig == RECDEL:
-        if self.base_verbose &gt; 1:
+        if self.verbose &gt; 1:
             print(&#34; Deleted data &#39;%s&#39; at %d (%d)&#34; % (sig, rec, cnt2))
         ret = 1
         return ret
 
     if sig != RECSIG:
-        if self.base_verbose &gt; 0:
+        if self.verbose &gt; 0:
             print(&#34; Damaged data (sig) &#39;%s&#39; at %d (%d)&#34; % (sig, rec, cnt2))
-        #if self.base_verbose &gt; 1:
+        #if self.verbose &gt; 1:
         #    print(&#34;Data&#34;, data)
 
         return ret
 
     hash = self.getbuffint(rec+4)
     blen = self.getbuffint(rec+8)
 
     if blen &lt;= 0:
-        if self.base_verbose &gt; 1:
+        if self.verbose &gt; 1:
             print(&#34;Invalid key length %d at %d&#34; % (blen, rec))
         return ret
 
     data = self.getbuffstr(rec+12, blen)
     ccc = self.hash32(data)
     if hash != ccc:
-        if self.base_verbose &gt; 1:
+        if self.verbose &gt; 1:
             print(&#34;Data&#34;, data)
-        elif self.base_verbose &gt; 0:
+        elif self.verbose &gt; 0:
             print(&#34;Error on hash at rec&#34;, rec, cnt2, &#34;hash&#34;,
                                         hex(hash), &#34;check&#34;, hex(ccc))
 
         return ret
 
     endd = self.getbuffstr(rec + 12 + blen, self.INTSIZE)
     if endd != RECSEP:
-        if self.base_verbose &gt; 0:
+        if self.verbose &gt; 0:
             print(&#34; Damaged data (sep) &#39;%s&#39; at %d %d %d&#34; % (endd, rec, cnt2))
         return ret
 
     rec2 = rec + 16 + blen;
     hash2 = self.getbuffint(rec2)
     blen2 = self.getbuffint(rec2+4)
 
     if blen2 &lt; 0:
-        if self.base_verbose &gt; 1:
+        if self.verbose &gt; 1:
             print(&#34;Invalid data length2 %d at %d&#34; % (blen2, rec))
         return ret
 
     data2 = self.getbuffstr(rec2+8, blen2)
     ccc2 = self.hash32(data2)
     if hash2 != ccc2:
-        if self.base_verbose &gt; 1:
+        if self.verbose &gt; 1:
             print(&#34;Data&#34;, data, &#34;Data2&#34;, data2)
-        elif self.base_verbose &gt; 0:
+        elif self.verbose &gt; 0:
             print(&#34;Error on hash2 at rec&#34;, rec, cnt2, &#34;hash2&#34;,
                                     hex(hash2), &#34;check2&#34;, hex(ccc2))
         return ret
 
-    if self.base_verbose &gt; 2:
+    if self.verbose &gt; 2:
         print(&#34;Record at %d (%d) OK.&#34; % (rec, cnt2))
 
     ret += 1
     return ret</code></pre>
 </details>
 </dd>
 <dt id="twincore.TwinCore.del_data"><code class="name flex">
@@ -3017,15 +3025,15 @@
         #    print(&#34; Damaged data &#39;%s&#39; at&#34; % sig, rec)
 
         #blen = self.getbuffint(rec+8)
         #print(&#34;data &#39;%s&#39; at&#34; % sig, rec, &#34;blen&#34;, blen)
 
         hhh = self.getbuffint(rec+4)
         if hash == hhh:
-            if self.base_verbose &gt; 0:
+            if self.verbose &gt; 0:
                 print(&#34;Would delete&#34;, hhh)
 
         self.putbuffstr(rec, RECDEL)
 
         cnt += 1
 
     return arr</code></pre>
@@ -3049,24 +3057,24 @@
         Deleted record is marked as deleted but not removed.
         Deleted records are ignored in further operations.
         Use &#39;vacuum&#39; to actually remove record.
     &#39;&#39;&#39;
 
     rsize = self._getdbsize(self.ifp)
     if recnum &gt;= rsize:
-        if self.base_verbose:
+        if self.verbose:
             print(&#34;Past end of data.&#34;);
         return False
     chash = self.getidxint(CURROFFS)
     #print(&#34;chash&#34;, chash)
     offs = self.getidxint(HEADSIZE + recnum * self.INTSIZE * 2)
     #print(&#34;offs&#34;, offs)
     old = self.getbuffstr(offs, self.INTSIZE)
     if old == RECDEL:
-        if self.base_verbose:
+        if self.verbose:
             print(&#34;Record at %d already deleted.&#34; % offs);
         return False
 
     self.putbuffstr(offs, RECDEL)
     return True</code></pre>
 </details>
 </dd>
@@ -3110,15 +3118,15 @@
     &#39;&#39;&#39; Delete records by key string; needs bin str, converted
         automatically on entry.
     &#39;&#39;&#39;
 
     if type(strx) != type(b&#34;&#34;):
         strx = strx.encode()
 
-    if self.base_verbose &gt; 1:
+    if self.verbose &gt; 1:
         print(&#34;Start delete &#34;, strx, &#34;skip&#34;, skip)
 
     cnt = 0; cnt3 = 0
     #chash = self.getidxint(CURROFFS)    #;print(&#34;chash&#34;, chash)
     chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
 
     # Direction sensitivity
@@ -3128,27 +3136,27 @@
         rrr = range(chash - self.INTSIZE * 2, HEADSIZE  - self.INTSIZE * 2, -self.INTSIZE * 2)
 
     #for aa in range(HEADSIZE, chash, self.INTSIZE * 2):
     for aa in rrr:
         rec = self.getidxint(aa)
         sig = self.getbuffstr(rec, self.INTSIZE)
         if sig == RECDEL:
-            if base_showdel:
+            if self.showdel:
                 print(&#34; Deleted record &#39;%s&#39; at&#34; % sig, rec)
         elif sig != RECSIG:
-            if self.base_verbose &gt; 0:
+            if self.verbose &gt; 0:
                 print(&#34; Damaged data &#39;%s&#39; at&#34; % sig, rec)
         else:
             blen = self.getbuffint(rec+8)
             data = self.getbuffstr(rec + 12, blen)
-            if self.base_verbose &gt; 2:
+            if self.verbose &gt; 2:
                 print(&#34;del iterate recs&#34;, cnt3, data, strx)
 
             if strx == data:
-                if self.base_verbose &gt; 0:
+                if self.verbose &gt; 0:
                     print(&#34;Deleting&#34;, cnt3, aa, data)
                 self.putbuffstr(rec, RECDEL)
                 cnt += 1
                 if cnt &gt;= maxdelrec:
                     break
         cnt3 += 1
     return cnt</code></pre>
@@ -3173,15 +3181,15 @@
         raise  RuntimeError( \
                 &#34;Past end of File. Asking for offset %d file size is %d.&#34; \
                                  % (recoffs, rsize) )
         return False
 
     sig = self.getbuffstr(recoffs, self.INTSIZE)
     if sig != RECSIG  and sig != RECDEL:
-        if self.core_verbose &gt; 0:
+        if self.verbose &gt; 0:
             print(&#34;Unlikely offset %d is not at record boundary.&#34; % recoffs, sig)
         return False
 
     self.putbuffstr(recoffs, RECDEL)
     return True</code></pre>
 </details>
 </dd>
@@ -3219,112 +3227,117 @@
 
     cnt2 = 0
     sig = self.getbuffstr(rec, self.INTSIZE)
     if self.pgdebug &gt; 5:
         print(&#34;Sig &#34;, sig, &#34;at&#34;, rec)
 
     if sig == RECDEL:
-        if base_showdel:
+        if self.showdel:
             klen = self.getbuffint(rec+8)
             kdata = self.getbuffstr(rec+12, klen)
             rec2 = rec + 16 + klen;
             blen = self.getbuffint(rec2+4)
             data = self.getbuffstr(rec2+8, blen)
             print(&#34; Del at&#34;, rec, &#34;key:&#34;, kdata, &#34;data:&#34;, truncs(data))
-        if self.base_verbose &gt; 1:
+        if self.verbose &gt; 1:
             klen = self.getbuffint(rec+8)
             kdata = self.getbuffstr(rec+12, klen)
             rec2 = rec + 16 + klen;
             blen = self.getbuffint(rec2+4)
             data = self.getbuffstr(rec2+8, blen)
-            if self.base_verbose &gt; 2:
+            if self.verbose &gt; 2:
                 print(&#34; Del at&#34;, rec, &#34;key:&#34;, kdata, &#34;data:&#34;, data)
             else:
                 print(&#34; Del at&#34;, rec, &#34;key:&#34;, kdata, &#34;data:&#34;, truncs(data))
 
         return cnt2
 
     if sig != RECSIG:
-        if self.base_verbose &gt; 1:
+        if self.verbose &gt; 1:
             print(&#34; Damaged data (sig) &#39;%s&#39; at&#34; % sig, rec)
         return cnt2
 
     hash = self.getbuffint(rec+4)
     blen = self.getbuffint(rec+8)
 
     if blen &lt; 0:
-        if self.base_verbose &gt; 2:
+        if self.verbose &gt; 2:
             print(&#34;Invalid key length %d at %d&#34; % (blen, rec))
         return cnt2
 
     data = self.getbuffstr(rec+12, blen)
-    if base_integrity:
+    if self.integrity:
         ccc = self.hash32(data)
-        if self.base_verbose &gt; 1:
+        if self.verbose &gt; 1:
             print(&#34;rec&#34;, rec, &#34;hash&#34;, hex(hash), &#34;check&#34;, hex(ccc))
         if hash != ccc:
-            if self.base_verbose &gt; 0:
+            if self.verbose &gt; 0:
                 print(&#34;Error on hash at rec&#34;, rec, &#34;hash&#34;, hex(hash), &#34;check&#34;, hex(ccc))
             return []
 
     endd = self.getbuffstr(rec + 12 + blen, self.INTSIZE)
     if endd != RECSEP:
-        if self.base_verbose &gt; 0:
+        if self.verbose &gt; 0:
             print(&#34; Damaged data (sep) &#39;%s&#39; at&#34; % endd, rec)
         return cnt2
 
     rec2 = rec + 16 + blen;
     hash2 = self.getbuffint(rec2)
     blen2 = self.getbuffint(rec2+4)
 
     if blen2 &lt; 0:
-        if self.base_verbose &gt; 1:
+        if self.verbose &gt; 1:
             print(&#34;Invalid data length %d at %d&#34; % (blen2, rec))
         return cnt2
 
     data2 = self.getbuffstr(rec2+8, blen2)
-    if base_integrity:
+    if self.integrity:
         ccc2 = self.hash32(data2)
-        if self.base_verbose &gt; 1:
+        if self.verbose &gt; 1:
             print(&#34;rec&#34;, rec, &#34;hash2&#34;, hex(hash), &#34;check2&#34;, hex(ccc))
         if hash2 != ccc2:
-            if self.base_verbose &gt; 0:
+            if self.verbose &gt; 0:
                 print(&#34;Error on hash at rec&#34;, rec, &#34;hash2&#34;, hex(hash), &#34;check2&#34;, hex(ccc))
             return []
 
-    if self.base_verbose &gt; 2:
+    if self.verbose &gt; 2:
         print(&#34;%-5d pos %5d&#34; % (cnt, rec), &#34;%8x&#34; % hash, &#34;len&#34;, blen, data,
                                                     &#34;%8x&#34; % hash2,&#34;len&#34;, blen2, data2)
 
-    elif self.base_verbose &gt; 1:
+    elif self.verbose &gt; 1:
         print(&#34;%-5d pos %5d&#34; % (cnt, rec), &#34;%8x&#34; % hash, &#34;len&#34;, blen, data,
                                                     &#34;%8x&#34; % hash2,&#34;len&#34;, blen2, data2)
-    elif self.base_verbose:
+    elif self.verbose:
         print(&#34;%-5d pos %5d&#34; % (cnt, rec),  data, data2)
     else:
         print(&#34;%-5d pos %5d&#34; % (cnt, rec), &#34;Data:&#34;, truncs(data, 18), &#34;Data2:&#34;, truncs(data2, 18))
 
     cnt2 += 1
     return cnt2</code></pre>
 </details>
 </dd>
 <dt id="twincore.TwinCore.find_key"><code class="name flex">
 <span>def <span class="ident">find_key</span></span>(<span>self, keyx, limx=4294967295)</span>
 </code></dt>
 <dd>
-<div class="desc"><p>Find record by key Search from the end, so latest comes first.</p></div>
+<div class="desc"><p>Find record by key value.
+Search from the end, so latest comes first.
+This operates on the hash, so it reaches the answer fast.</p></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
 <pre><code class="python">def  find_key(self, keyx, limx = 0xffffffff):
 
-    &#39;&#39;&#39; Find record by key Search from the end, so latest comes first. &#39;&#39;&#39;
+    &#39;&#39;&#39; Find record by key value.
+        Search from the end, so latest comes first.
+        This operates on the hash, so it reaches the answer fast.
+    &#39;&#39;&#39;
 
-    self.lock.waitlock()   #self.lckname)
+    self.lock.waitlock()
 
     skip = 0; arr = []; cnt = 0
     try:
         arg2e = keyx.encode()
     except:
         arg2e = keyx
 
@@ -3336,123 +3349,176 @@
             HEADSIZE - self.INTSIZE * 2, -self.INTSIZE * 2)
     for aa in rrr:
         rec = self.getidxint(aa)
         #print(&#34; Scanning at %d %d&#34; % (rec, cnt))
 
         sig = self.getbuffstr(rec, self.INTSIZE)
         if sig == RECDEL:
-            if base_showdel:
+            if self.showdel:
                 print(&#34;Deleted record &#39;%s&#39; at&#34; % sig, rec)
         elif sig != RECSIG:
-            if self.base_verbose &gt; 0:
+            if self.verbose &gt; 0:
                 print(&#34; Damaged data &#39;%s&#39; at&#34; % sig, rec)
         else:
             hhh = self.getbuffint(rec+4)
             if hhh == hhhh:
                 if len(arr) &gt;= limx - 1:
                     arr.append([&#34;More data ...&#34;,])
                     break
                 arr.append(rec)
             else:
                 pass
                 #print(&#34;no match&#34;, hex(hhh))
 
         cnt += 1
-    self.lock.unlock()  #dellock()self.lckname)
+    self.lock.unlock()
 
     return arr</code></pre>
 </details>
 </dd>
 <dt id="twincore.TwinCore.findrec"><code class="name flex">
 <span>def <span class="ident">findrec</span></span>(<span>self, strx, limx=4294967295, skipx=0)</span>
 </code></dt>
 <dd>
-<div class="desc"><p>Find by string matching substring.</p></div>
+<div class="desc"><p>Find key by matching strx with substring.
+Return record(s).</p></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
 <pre><code class="python">def  findrec(self, strx, limx = INT_MAX, skipx = 0):
 
-    &#39;&#39;&#39; Find by string matching substring. &#39;&#39;&#39;
+    &#39;&#39;&#39; Find key by matching strx with substring.
+    Return record(s).
+    &#39;&#39;&#39;
+
+    self.lock.waitlock()
 
-    self.lock.waitlock()    #(self.lckname)
+    #chash = self.getidxint(CURROFFS)            #;print(&#34;chash&#34;, chash)
     chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
+
     arr = []
-    if type(strx) != type(b&#34;&#34;):
-        strx2 = strx.encode(errors=&#39;strict&#39;);
+    strx2 = strx.encode(errors=&#39;strict&#39;);
 
     #print(&#34;findrec&#34;, strx2)
 
     #for aa in range(HEADSIZE + self.INTSIZE * 2, chash, self.INTSIZE * 2):
     for aa in range(chash - self.INTSIZE * 2, HEADSIZE  - self.INTSIZE * 2, -self.INTSIZE * 2):
         rec = self.getidxint(aa)
         sig = self.getbuffstr(rec, self.INTSIZE)
         if sig == RECDEL:
-            if base_showdel:
+            if self.showdel:
                 print(&#34; Deleted record &#39;%s&#39; at&#34; % sig, rec)
         elif sig != RECSIG:
-            if self.base_verbose &gt; 0:
+            if self.verbose &gt; 0:
                 print(&#34; Damaged data &#39;%s&#39; at&#34; % sig, rec)
         else:
             blen = self.getbuffint(rec+8)
             data = self.getbuffstr(rec + 12, blen)
-            if self.base_verbose &gt; 1:
+            if self.verbose &gt; 1:
                 print(&#34;find&#34;, data)
             #if str(strx2) in str(data):
             if strx2 in data:
-                #arr.append(self.get_key_offs(rec))
+                arr.append(self.get_key_offs(rec))
                 #arr.append(rec)
-                arr.append(self._rec2arr(rec))
+
                 if len(arr) &gt;= limx:
                     break
-    self.lock.unlock()    #dellock(self.lckname)
+    self.lock.unlock()
 
     return arr</code></pre>
 </details>
 </dd>
 <dt id="twincore.TwinCore.findrecpos"><code class="name flex">
 <span>def <span class="ident">findrecpos</span></span>(<span>self, strx, limx=4294967295, skipx=0)</span>
 </code></dt>
 <dd>
-<div class="desc"><p>Find record, return array of positions.</p></div>
+<div class="desc"><p>Find record by key, return array of positions.</p></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
 <pre><code class="python">def  findrecpos(self, strx, limx = INT_MAX, skipx = 0):
 
-    &#39;&#39;&#39; Find record, return array of positions. &#39;&#39;&#39;
+    &#39;&#39;&#39; Find record by key, return array of positions. &#39;&#39;&#39;
 
-    self.lock.waitlock()    #(self.lckname)
+    self.lock.waitlock()
     chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
     arr = []
     if type(strx) != type(b&#34;&#34;):
         strx = strx.encode(errors=&#39;strict&#39;);
 
     for aa in range(chash - self.INTSIZE * 2, HEADSIZE  - self.INTSIZE * 2, -self.INTSIZE * 2):
         rec = self.getidxint(aa)
         sig = self.getbuffstr(rec, self.INTSIZE)
         if sig == RECDEL:
-            if base_showdel:
+            if self.showdel:
                 print(&#34; Deleted record &#39;%s&#39; at&#34; % sig, rec)
         elif sig != RECSIG:
-            if self.base_verbose &gt; 0:
+            if self.verbose &gt; 0:
                 print(&#34; Damaged data &#39;%s&#39; at&#34; % sig, rec)
         else:
             blen = self.getbuffint(rec+8)
             data = self.getbuffstr(rec + 12, blen)
-            if self.base_verbose &gt; 1:
+            if self.verbose &gt; 1:
                 print(&#34;frecpos&#34;, data)
             if strx == data:
                 arr.append(rec)
                 if len(arr) &gt;= limx:
                     break
 
-    self.lock.unlock()  #dellock(self.lckname)
+    self.lock.unlock()
+
+    return arr</code></pre>
+</details>
+</dd>
+<dt id="twincore.TwinCore.findrecsub"><code class="name flex">
+<span>def <span class="ident">findrecsub</span></span>(<span>self, strx, limx=4294967295, skipx=0)</span>
+</code></dt>
+<dd>
+<div class="desc"><p>Find record by matching substring.</p></div>
+<details class="source">
+<summary>
+<span>Expand source code</span>
+</summary>
+<pre><code class="python">def  findrecsub(self, strx, limx = INT_MAX, skipx = 0):
+
+    &#39;&#39;&#39; Find record by matching substring. &#39;&#39;&#39;
+
+    self.lock.waitlock()
+    chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
+    arr = []
+    if type(strx) != type(b&#34;&#34;):
+        strx2 = strx.encode(errors=&#39;strict&#39;);
+
+    #print(&#34;findrec&#34;, strx2)
+
+    #for aa in range(HEADSIZE + self.INTSIZE * 2, chash, self.INTSIZE * 2):
+    for aa in range(chash - self.INTSIZE * 2, HEADSIZE  - self.INTSIZE * 2, -self.INTSIZE * 2):
+        rec = self.getidxint(aa)
+        sig = self.getbuffstr(rec, self.INTSIZE)
+        if sig == RECDEL:
+            if self.showdel:
+                print(&#34; Deleted record &#39;%s&#39; at&#34; % sig, rec)
+        elif sig != RECSIG:
+            if self.verbose &gt; 0:
+                print(&#34; Damaged data &#39;%s&#39; at&#34; % sig, rec)
+        else:
+            blen = self.getbuffint(rec+8)
+            data = self.getbuffstr(rec + 12, blen)
+            if self.verbose &gt; 1:
+                print(&#34;find&#34;, data)
+            #if str(strx2) in str(data):
+            if strx2 in data:
+                #arr.append(self.get_key_offs(rec))
+                #arr.append(rec)
+                arr.append(self._rec2arr(rec))
+                if len(arr) &gt;= limx:
+                    break
+    self.lock.unlock()
 
     return arr</code></pre>
 </details>
 </dd>
 <dt id="twincore.TwinCore.flush"><code class="name flex">
 <span>def <span class="ident">flush</span></span>(<span>self)</span>
 </code></dt>
@@ -3499,19 +3565,19 @@
         raise  RuntimeError( \
                 &#34;Past end of File. Asking for offset %d file size is %d.&#34; \
                                  % (recoffs, rsize) )
         return []
 
     sig = self.getbuffstr(recoffs, self.INTSIZE)
     if sig == RECDEL:
-        if self.base_verbose:
+        if self.verbose:
             print(&#34;Deleted record.&#34;)
         return []
     if sig != RECSIG:
-        if self.core_verbose &gt; 0:
+        if self.verbose &gt; 0:
             print(&#34;Unlikely offset %d is not at record boundary.&#34; % recoffs, sig)
         return []
     #print(&#34;recoffs&#34;, recoffs)
     return self._rec2arr(recoffs)[0]</code></pre>
 </details>
 </dd>
 <dt id="twincore.TwinCore.get_rec"><code class="name flex">
@@ -3524,30 +3590,30 @@
 <span>Expand source code</span>
 </summary>
 <pre><code class="python">def  get_rec(self, recnum):
 
     &#39;&#39;&#39; Get record from database; recnum is a zero based record counter. &#39;&#39;&#39;
 
     if self.pgdebug:
-        print(&#34;getrec()&#34;, recnum)
+        print(&#34;get_rec()&#34;, recnum)
 
     rsize = self._getdbsize(self.ifp)
     if recnum &gt;= rsize:
-        if self.core_verbose &gt; 0:
+        if self.verbose &gt; 0:
             print(&#34;Past end of data.&#34;);
-        raise  RuntimeError( \
-                &#34;Past end of Data. Asking for %d while max is 0 .. %d records.&#34; \
-                                 % (recnum, rsize-1) )
+        errx =  &#34;Past end of Data. (ask: %d max: %d)&#34;  % (recnum, rsize-1)
+        raise  RuntimeError(errx)
         return []
 
     chash = self.getidxint(CURROFFS)
     #print(&#34;chash&#34;, chash)
     offs = self.getidxint(HEADSIZE + recnum * self.INTSIZE * 2)
 
-    #print(&#34;offs&#34;, offs)
+    #sig = self.getbuffstr(offs, self.INTSIZE)
+
     return self._rec2arr(offs)</code></pre>
 </details>
 </dd>
 <dt id="twincore.TwinCore.get_rec_byoffs"><code class="name flex">
 <span>def <span class="ident">get_rec_byoffs</span></span>(<span>self, recoffs)</span>
 </code></dt>
 <dd>
@@ -3566,19 +3632,18 @@
         raise  RuntimeError( \
                 &#34;Past end of File. Asking for offset %d file size is %d.&#34; \
                                  % (recoffs, rsize) )
         return []
 
     sig = self.getbuffstr(recoffs, self.INTSIZE)
     if sig == RECDEL:
-        if self.base_verbose:
+        if self.verbose:
             print(&#34;Deleted record.&#34;)
-        return []
     if sig != RECSIG:
-        if self.core_verbose &gt; 0:
+        if self.verbose &gt; 0:
             print(&#34;Unlikely offset %d is not at record boundary.&#34; % recoffs, sig)
         return []
     #print(&#34;recoffs&#34;, recoffs)
     return self._rec2arr(recoffs)</code></pre>
 </details>
 </dd>
 <dt id="twincore.TwinCore.getdbsize"><code class="name flex">
@@ -3616,29 +3681,29 @@
 </summary>
 <pre><code class="python">def integrity_check(self, skip = 0, count = 0xffffffff):
 
     &#39;&#39;&#39; Check record integrity for &#39;count&#39; records.
         Skip number of records.
     &#39;&#39;&#39;
 
-    self.lock.waitlock()    #(self.lckname)
+    self.lock.waitlock()
     ret = 0; cnt2 = 0; cnt3 = 0;
     #chash = self.getidxint(CURROFFS)        #;print(&#34;chash&#34;, chash)
     chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
     # Direction sensitivity
     rrr = range(HEADSIZE + skip * self.INTSIZE * 2, chash, self.INTSIZE * 2)
     for aa in rrr:
         rec = self.getidxint(aa)
         #print(aa, rec)
         ret += self.check_rec(rec, cnt2)
         cnt2 += 1
         cnt3 += 1
         if cnt3 &gt;= count:
             break
-    self.lock.unlock() #dellock(self.lckname)
+    self.lock.unlock()
     return ret, cnt2</code></pre>
 </details>
 </dd>
 <dt id="twincore.TwinCore.listall"><code class="name flex">
 <span>def <span class="ident">listall</span></span>(<span>self)</span>
 </code></dt>
 <dd>
@@ -3647,15 +3712,15 @@
 <summary>
 <span>Expand source code</span>
 </summary>
 <pre><code class="python">def  listall(self):
 
     &#39;&#39;&#39; List all active records. Return array id record indexes. &#39;&#39;&#39;
 
-    self.lock.waitlock()    #(self.lckname)
+    self.lock.waitlock()
     keys = []; arr = []; cnt = 0
 
     chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
     maxrec = chash - self.INTSIZE * 2
     rsize = self._getdbsize(self.ifp) - 1
 
     rrr =  range(maxrec,
@@ -3663,31 +3728,31 @@
     for aa in rrr:
         rec = self.getidxint(aa)
 
         #print(&#34; Scanning at %d %d&#34; % (rec, cnt))
 
         sig = self.getbuffstr(rec, self.INTSIZE)
         if sig == RECDEL:
-            if 1: #base_showdel:
+            if 1: #self.showdel:
                 print(&#34;Deleted record &#39;%s&#39; at&#34; % sig, rec)
         elif sig != RECSIG:
-            if 1: #self.base_verbose &gt; 0:
+            if 1: #self.verbose &gt; 0:
                 print(&#34; Damaged data &#39;%s&#39; at&#34; % sig, rec)
         else:
                 hhh = self.getbuffint(rec+4)
                 print(&#34; Good data &#39;%s&#39; at&#34; % sig, rec, hhh)
                 if hhh not in keys:
                     keys.append(hhh)
                     # as we are going backwards
                     arr.append(rsize - cnt)
                     #print(&#34;found&#34;, hhh)
         cnt += 1
 
     keys = []
-    self.lock.unlock()  #dellock()self.lckname)
+    self.lock.unlock()
 
     return arr</code></pre>
 </details>
 </dd>
 <dt id="twincore.TwinCore.reindex"><code class="name flex">
 <span>def <span class="ident">reindex</span></span>(<span>self)</span>
 </code></dt>
@@ -3697,17 +3762,17 @@
 <summary>
 <span>Expand source code</span>
 </summary>
 <pre><code class="python">def  reindex(self):
 
     &#39;&#39;&#39; Re create index file. &#39;&#39;&#39;
 
-    self.lock.waitlock() #self.lckname)
+    self.lock.waitlock()
     ret = self.__reindex()
-    self.lock.unlock()    #dellock(self.lckname)
+    self.lock.unlock()
     return ret</code></pre>
 </details>
 </dd>
 <dt id="twincore.TwinCore.retrieve"><code class="name flex">
 <span>def <span class="ident">retrieve</span></span>(<span>self, strx, limx=1)</span>
 </code></dt>
 <dd>
@@ -3729,33 +3794,33 @@
 
     #chash = self.getidxint(CURROFFS)
     chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
 
     #;print(&#34;chash&#34;, chash)
     arr = []
 
-    self.lock.waitlock() #(self.lckname)
+    self.lock.waitlock()
 
     #for aa in range(HEADSIZE + self.INTSIZE * 2, chash, self.INTSIZE * 2):
     for aa in range(chash - self.INTSIZE * 2, HEADSIZE  - self.INTSIZE * 2, -self.INTSIZE * 2):
         rec = self.getidxint(aa)
         sig = self.getbuffstr(rec, self.INTSIZE)
         if sig == RECDEL:
-            if self.base_verbose &gt; 3:
+            if self.verbose &gt; 3:
                 print(&#34; Deleted record &#39;%s&#39; at&#34; % sig, rec)
         elif sig != RECSIG:
-            if self.base_verbose:
+            if self.verbose:
                 print(&#34; Damaged data &#39;%s&#39; at&#34; % sig, rec)
         else:
             hhh = self.getbuffint(rec+4)
             if hhh == hhhh:
                 arr.append(self.get_rec_byoffs(rec))
                 if len(arr) &gt;= limx:
                     break
-    self.lock.unlock()  #dellock(self.lckname)
+    self.lock.unlock()
 
     return arr</code></pre>
 </details>
 </dd>
 <dt id="twincore.TwinCore.revdump_data"><code class="name flex">
 <span>def <span class="ident">revdump_data</span></span>(<span>self, lim, skip=0)</span>
 </code></dt>
@@ -3773,53 +3838,55 @@
 </details>
 </dd>
 <dt id="twincore.TwinCore.save_data"><code class="name flex">
 <span>def <span class="ident">save_data</span></span>(<span>self, header, datax, replace=False)</span>
 </code></dt>
 <dd>
 <div class="desc"><p>Append to the end of file. If replace flag is set, try to overwrite
-in place. If new record is larger, add it as ususal. If smaller,
+in place. If new record is larger, add it as usual. If smaller,
 the record is padded with spaces. This should not influence most ops.
 (like: int())
 This feature allows the database update wthout creating new records.
-Useful for counters or dynamically changing data.</p>
+Useful for counters or dynamically changing data. To be useful,
+use
+create fixed size data. Like sprintf(%12d).</p>
 <pre><code>    Input:
         header     Header
         datax      Data
 
      Return:
         The offset of saved data
 </code></pre></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
 <pre><code class="python">def  save_data(self, header, datax, replace = False):
 
     &#39;&#39;&#39; Append to the end of file. If replace flag is set, try to overwrite
-        in place. If new record is larger, add it as ususal. If smaller,
+        in place. If new record is larger, add it as usual. If smaller,
         the record is padded with spaces. This should not influence most ops.
         (like: int())
         This feature allows the database update wthout creating new records.
-        Useful for counters or dynamically changing data.
+        Useful for counters or dynamically changing data. To be useful,
+        use  create fixed size data. Like sprintf(%12d).
 
                 Input:
                     header     Header
                     datax      Data
 
                  Return:
                     The offset of saved data
         &#39;&#39;&#39;
 
     if self.pgdebug &gt; 0:
         print(&#34;Save_data()&#34;, header, datax)
 
-    self.lock.waitlock()   #self.lckname)
-    ret = 0
-    was = False
+    self.lock.waitlock()
+    ret = 0 ; was = False
     # Put new data in place
     if replace:
         if type(datax) != type(b&#34;&#34;):
             mrep2 = datax.encode()
         else:
             mrep2 = datax
 
@@ -3834,17 +3901,18 @@
                 ccc = self.hash32(padded)
                 self.putbuffint(rrr[1] - 8, ccc)
                 #print(&#34;ccc&#34;, hex(ccc))
                 self.putbuffstr(rrr[1], padded)
                 was = True
                 ret =  rrr[0]
     if not was:
+        #print(&#34;Saving longer data&#34;, header, datax)
         ret = self._save_data2(header, datax)
 
-    self.lock.unlock()  #dellock()self.lckname)
+    self.lock.unlock()
 
     return ret</code></pre>
 </details>
 </dd>
 <dt id="twincore.TwinCore.vacuum"><code class="name flex">
 <span>def <span class="ident">vacuum</span></span>(<span>self)</span>
 </code></dt>
@@ -3862,34 +3930,20 @@
     &#39;&#39;&#39;
         Remove all deleted data. Reindex.
         The db is locked while the vacuum is in operation, but
         make sure the DB in not in session, and no pending
         operations are present (like find / retrieve cycle).
     &#39;&#39;&#39;
 
-    self.lock.waitlock() #self.lckname)
+    self.lock.waitlock()
     ret = self._vacuum()
-    self.lock.unlock()  #dellock(self.lckname)
+    self.lock.unlock()
     return ret</code></pre>
 </details>
 </dd>
-<dt id="twincore.TwinCore.version"><code class="name flex">
-<span>def <span class="ident">version</span></span>(<span>self)</span>
-</code></dt>
-<dd>
-<div class="desc"><p>Return version sting.</p></div>
-<details class="source">
-<summary>
-<span>Expand source code</span>
-</summary>
-<pre><code class="python">def version(self):
-    &#39;&#39;&#39; Return version sting. &#39;&#39;&#39;
-    return Version</code></pre>
-</details>
-</dd>
 </dl>
 </dd>
 </dl>
 </section>
 </article>
 <nav id="sidebar">
 <h1>Index</h1>
@@ -3908,27 +3962,27 @@
 <li><code><a title="twincore.TwinCore.del_rec_bykey" href="#twincore.TwinCore.del_rec_bykey">del_rec_bykey</a></code></li>
 <li><code><a title="twincore.TwinCore.del_rec_offs" href="#twincore.TwinCore.del_rec_offs">del_rec_offs</a></code></li>
 <li><code><a title="twincore.TwinCore.dump_data" href="#twincore.TwinCore.dump_data">dump_data</a></code></li>
 <li><code><a title="twincore.TwinCore.dump_rec" href="#twincore.TwinCore.dump_rec">dump_rec</a></code></li>
 <li><code><a title="twincore.TwinCore.find_key" href="#twincore.TwinCore.find_key">find_key</a></code></li>
 <li><code><a title="twincore.TwinCore.findrec" href="#twincore.TwinCore.findrec">findrec</a></code></li>
 <li><code><a title="twincore.TwinCore.findrecpos" href="#twincore.TwinCore.findrecpos">findrecpos</a></code></li>
+<li><code><a title="twincore.TwinCore.findrecsub" href="#twincore.TwinCore.findrecsub">findrecsub</a></code></li>
 <li><code><a title="twincore.TwinCore.flush" href="#twincore.TwinCore.flush">flush</a></code></li>
 <li><code><a title="twincore.TwinCore.get_key_offs" href="#twincore.TwinCore.get_key_offs">get_key_offs</a></code></li>
 <li><code><a title="twincore.TwinCore.get_rec" href="#twincore.TwinCore.get_rec">get_rec</a></code></li>
 <li><code><a title="twincore.TwinCore.get_rec_byoffs" href="#twincore.TwinCore.get_rec_byoffs">get_rec_byoffs</a></code></li>
 <li><code><a title="twincore.TwinCore.getdbsize" href="#twincore.TwinCore.getdbsize">getdbsize</a></code></li>
 <li><code><a title="twincore.TwinCore.integrity_check" href="#twincore.TwinCore.integrity_check">integrity_check</a></code></li>
 <li><code><a title="twincore.TwinCore.listall" href="#twincore.TwinCore.listall">listall</a></code></li>
 <li><code><a title="twincore.TwinCore.reindex" href="#twincore.TwinCore.reindex">reindex</a></code></li>
 <li><code><a title="twincore.TwinCore.retrieve" href="#twincore.TwinCore.retrieve">retrieve</a></code></li>
 <li><code><a title="twincore.TwinCore.revdump_data" href="#twincore.TwinCore.revdump_data">revdump_data</a></code></li>
 <li><code><a title="twincore.TwinCore.save_data" href="#twincore.TwinCore.save_data">save_data</a></code></li>
 <li><code><a title="twincore.TwinCore.vacuum" href="#twincore.TwinCore.vacuum">vacuum</a></code></li>
-<li><code><a title="twincore.TwinCore.version" href="#twincore.TwinCore.version">version</a></code></li>
 </ul>
 </li>
 </ul>
 </li>
 </ul>
 </nav>
 </main>
```

#### html2text {}

```diff
@@ -1,9 +1,8 @@
 ************ MMoodduullee ttwwiinnccoorree ************
-! @mainpage
 Database with two files. One for data, one for index;
 
 The reason for the 'twin' name is that two files are created.
 The first contains the data, the second contains the
 offsets (indexes) and hashes.
 
 The second file can be re-built easily from the first
@@ -38,101 +37,102 @@
 
 Debug:    (use the '-d' option with number)
 
     0 =  no output
     1 =  normal, some items
     2 =  more details
 
-History:
 
-    1.1         Tue 20.Feb.2024     Initial release
-    1.2.0       Mon 26.Feb.2024     Moved pip home to pydbase/
-    1.4.0       Tue 27.Feb.2024     Addedd pgdebug
-    1.4.2       Wed 28.Feb.2024     Fixed multiple instances
-    1.4.3       Wed 28.Feb.2024     ChainAdm added
-    1.4.4       Fri 01.Mar.2024     Tests for chain functions
-    1.4.5       Fri 01.Mar.2024     Misc fixes
-    1.4.6       Mon 04.Mar.2024     Vacuum count on vacuumed records
-    1.4.7       Tue 05.Mar.2024     In place record update
-    1.4.8       Sat 09.Mar.2024     Added new locking mechanism
+History
+-----=
+
+1.1         Tue 20.Feb.2024     Initial release
+1.2.0       Mon 26.Feb.2024     Moved pip home to pydbase/
+1.4.0       Tue 27.Feb.2024     Addedd pgdebug
+1.4.2       Wed 28.Feb.2024     Fixed multiple instances
+1.4.3       Wed 28.Feb.2024     ChainAdm added
+1.4.4       Fri 01.Mar.2024     Tests for chain functions
+1.4.5       Fri 01.Mar.2024     Misc fixes
+1.4.6       Mon 04.Mar.2024     Vacuum count on vacuumed records
+1.4.7       Tue 05.Mar.2024     In place record update
+1.4.8       Sat 09.Mar.2024     Added new locking mechanism
+... more ... see README.md
 Expand source code
 #!/usr/bin/env python3
 
-'''!
-    @mainpage
-
-        Database with two files. One for data, one for index;
-
-        The reason for the 'twin' name is that two files are created.
-        The first contains the data, the second contains the
-        offsets (indexes) and hashes.
-
-        The second file can be re-built easily from the first
-        using the reindex option.
-
-        Structure of the data:
-
-            32 byte header, starating with FILESIG;
-
-            4 bytes    4 bytes          4 bytes         Variable
-            ------------------------------------------------------------
-            RECSIG     Hash_of_key      Len_of_key      DATA_for_key
-            RECSEP     Hash_of_payload  Len_of_payload  DATA_for_payload
-                .
-                .
-
-            RECSIG     Hash_of_key      Len_of_key      DATA_for_key
-            RECSEP     Hash_of_payload  Len_of_payload  DATA_for_payload
-
-        Deleted records are marked with RECSIG mutated from RECB to RECX
-
-        New data is appended to the end, no duplicate filtering is done.
-        Retrieval is searched from reverse, the latest record with this key
-        is retrieved first.
-
-        Verbosity:    (use the '-v' option multiple times)
-
-            0 =  no output
-            1 =  normal, some items printed, short record ;
-            2 =  more detail; full record (-vv)
-            3 =  more detail + damaged records (-vvv)
-
-        Debug:    (use the '-d' option with number)
-
-            0 =  no output
-            1 =  normal, some items
-            2 =  more details
-
-        History:
-
-            1.1         Tue 20.Feb.2024     Initial release
-            1.2.0       Mon 26.Feb.2024     Moved pip home to pydbase/
-            1.4.0       Tue 27.Feb.2024     Addedd pgdebug
-            1.4.2       Wed 28.Feb.2024     Fixed multiple instances
-            1.4.3       Wed 28.Feb.2024     ChainAdm added
-            1.4.4       Fri 01.Mar.2024     Tests for chain functions
-            1.4.5       Fri 01.Mar.2024     Misc fixes
-            1.4.6       Mon 04.Mar.2024     Vacuum count on vacuumed records
-            1.4.7       Tue 05.Mar.2024     In place record update
-            1.4.8       Sat 09.Mar.2024     Added new locking mechanism
+'''
+    <pre>
+    Database with two files. One for data, one for index;
 
+    The reason for the 'twin' name is that two files are created.
+    The first contains the data, the second contains the
+    offsets (indexes) and hashes.
+
+    The second file can be re-built easily from the first
+    using the reindex option.
+
+    Structure of the data:
+
+        32 byte header, starating with FILESIG;
+
+        4 bytes    4 bytes          4 bytes         Variable
+        ------------------------------------------------------------
+        RECSIG     Hash_of_key      Len_of_key      DATA_for_key
+        RECSEP     Hash_of_payload  Len_of_payload  DATA_for_payload
+            .
+            .
+
+        RECSIG     Hash_of_key      Len_of_key      DATA_for_key
+        RECSEP     Hash_of_payload  Len_of_payload  DATA_for_payload
+
+    Deleted records are marked with RECSIG mutated from RECB to RECX
+
+    New data is appended to the end, no duplicate filtering is done.
+    Retrieval is searched from reverse, the latest record with this key
+    is retrieved first.
+
+    Verbosity:    (use the '-v' option multiple times)
+
+        0 =  no output
+        1 =  normal, some items printed, short record ;
+        2 =  more detail; full record (-vv)
+        3 =  more detail + damaged records (-vvv)
+
+    Debug:    (use the '-d' option with number)
+
+        0 =  no output
+        1 =  normal, some items
+        2 =  more details
+
+    History:
+
+        1.1         Tue 20.Feb.2024     Initial release
+        1.2.0       Mon 26.Feb.2024     Moved pip home to pydbase/
+        1.4.0       Tue 27.Feb.2024     Addedd pgdebug
+        1.4.2       Wed 28.Feb.2024     Fixed multiple instances
+        1.4.3       Wed 28.Feb.2024     ChainAdm added
+        1.4.4       Fri 01.Mar.2024     Tests for chain functions
+        1.4.5       Fri 01.Mar.2024     Misc fixes
+        1.4.6       Mon 04.Mar.2024     Vacuum count on vacuumed records
+        1.4.7       Tue 05.Mar.2024     In place record update
+        1.4.8       Sat 09.Mar.2024     Added new locking mechanism
+        ... more ... see README.md
+        </pre>
 '''
 
 import  os, sys, getopt, signal, select, socket, time, struct
 import  random, stat, os.path, datetime, threading
 import  struct, io
 
 base = os.path.dirname(os.path.realpath(__file__))
 sys.path.append(os.path.join(base))
 sys.path.append(os.path.join(base, '..', 'pydbase'))
 
 from twinbase import *
 
-Version = "1.4.8"
-
 # ------------------------------------------------------------------------
 
 class TwinCore(TwinCoreBase):
 
     '''
 
      Data file and index file; protected by locks
@@ -143,21 +143,22 @@
     def __init__(self, fname = "pydbase.pydb", pgdebug = 0, devmode = 1):
 
         self.cnt = 0
         self.fname = fname
         self.lckname  = os.path.splitext(self.fname)[0] + ".lock"
         self.idxname  = os.path.splitext(self.fname)[0] + ".pidx"
         self.pgdebug = pgdebug
-        self.base_verbose  = 0
-        self.core_verbose  = 0
+        self.verbose  = 0
+        self.showdel  = 0
+        self.integrity = 0
         self.devmode = devmode
         self.lock = FileLock(self.lckname)
 
         # Make sure only one process can use this
-        self.lock.waitlock() #self.lckname)
+        self.lock.waitlock()
 
         super(TwinCore, self).__init__(pgdebug)
 
         #print("initializing core with", fname, pgdebug)
         #self.pool = threading.BoundedSemaphore(value=1)
 
         # It was informative at one point
@@ -202,31 +203,27 @@
             #self.ifp = self.softcreate(self.idxname)
             indexsize = self.getsize(self.ifp)
 
             # See if valid index
             if indexsize < HEADSIZE:
                 self.create_idx(self.ifp)
                 # It was an existing data, new index needed
-                if self.base_verbose > 0:
+                if self.verbose > 0:
                     print("Reindexing")
                 self.__reindex()
 
         # Check
         if  self.getbuffstr(0, 4) != FILESIG:
-            if self.base_verbose > 2:
+            if self.verbose > 2:
                 print("Invalid data signature")
-            self.lock.unlock()  #dellock(self.lckname)
+            self.lock.unlock()
             raise  RuntimeError("Invalid database signature.")
 
         #print("buffsize", buffsize, "indexsize", indexsize)
-        self.lock.unlock() #dellock(self.lckname)
-
-    def version(self):
-        ''' Return version sting. '''
-        return Version
+        self.lock.unlock()
 
     def flush(self):
 
         ''' Flush files to disk. '''
 
         if self.pgdebug > 9:
             print("Flushing", self.fp, self.ifp)
@@ -265,64 +262,68 @@
             ret = 0
 
         return  ret
 
     # --------------------------------------------------------------------
     def _rec2arr(self, rec):
 
+        # Wed 10.Apr.2024 decision is made at the higher level
         arr = []
         sig = self.getbuffstr(rec, self.INTSIZE)
 
-        if sig == RECDEL:
-            return arr
-
-        if sig != RECSIG:
-            if self.base_verbose > 0:
+        if sig != RECSIG and sig != RECDEL:
+            if self.verbose > 0:
                 print(" Damaged data (sig) '%s' at" % sig, rec)
             return arr
 
         hash = self.getbuffint(rec+4)
         blen = self.getbuffint(rec+8)
         data = self.getbuffstr(rec + 12, blen)
 
-        if base_integrity:
+        if self.integrity:
             ccc = self.hash32(data)
-            if self.base_verbose > 1:
+            if self.verbose > 1:
                 print("rec", rec, "hash", hex(hash), "check", hex(ccc))
             if hash != ccc:
-                if self.base_verbose > 0:
+                if self.verbose > 0:
                     print("Error on hash at rec", rec, "hash", hex(hash),
 "check", hex(ccc))
                 return []
 
         #print("%5d pos %5d" % (cnt, rec), "hash %8x" % hash, "ok", ok, "len=",
 blen, end=" ")
 
         endd = self.getbuffstr(rec + 12 + blen, self.INTSIZE)
         if endd != RECSEP:
-            if self.base_verbose > 0:
+            if self.verbose > 0:
                 print(" Damaged data (sep) '%s' at" % endd, rec)
             return arr
 
         rec2 = rec + 16 + blen;
         hash2 = self.getbuffint(rec2)
         blen2 = self.getbuffint(rec2+4)
         data2 = self.getbuffstr(rec2+8, blen2)
 
-        if base_integrity:
+        if self.integrity:
             ccc2 = self.hash32(data2)
-            if self.base_verbose > 1:
+            if self.verbose > 1:
                 print("rec", rec, "hash2", hex(hash2), "check2", hex(ccc2))
             if hash2 != ccc2:
-                if self.base_verbose > 0:
+                if self.verbose > 0:
                     print("Error on hash at rec", rec, "hash2", hex(hash2),
 "check2", hex(ccc2))
                 return []
 
-        arr = [data, data2]
+        if sig == RECDEL:
+            if self.showdel:
+                arr = [b"del", data, data2]
+            else:
+                arr = []
+        else:
+            arr = [data, data2]
         return arr
 
     # -------------------------------------------------------------------
     # Originator, dump single record
 
     def  dump_rec(self, rec, cnt):
 
@@ -333,94 +334,94 @@
 
         cnt2 = 0
         sig = self.getbuffstr(rec, self.INTSIZE)
         if self.pgdebug > 5:
             print("Sig ", sig, "at", rec)
 
         if sig == RECDEL:
-            if base_showdel:
+            if self.showdel:
                 klen = self.getbuffint(rec+8)
                 kdata = self.getbuffstr(rec+12, klen)
                 rec2 = rec + 16 + klen;
                 blen = self.getbuffint(rec2+4)
                 data = self.getbuffstr(rec2+8, blen)
                 print(" Del at", rec, "key:", kdata, "data:", truncs(data))
-            if self.base_verbose > 1:
+            if self.verbose > 1:
                 klen = self.getbuffint(rec+8)
                 kdata = self.getbuffstr(rec+12, klen)
                 rec2 = rec + 16 + klen;
                 blen = self.getbuffint(rec2+4)
                 data = self.getbuffstr(rec2+8, blen)
-                if self.base_verbose > 2:
+                if self.verbose > 2:
                     print(" Del at", rec, "key:", kdata, "data:", data)
                 else:
                     print(" Del at", rec, "key:", kdata, "data:", truncs(data))
 
             return cnt2
 
         if sig != RECSIG:
-            if self.base_verbose > 1:
+            if self.verbose > 1:
                 print(" Damaged data (sig) '%s' at" % sig, rec)
             return cnt2
 
         hash = self.getbuffint(rec+4)
         blen = self.getbuffint(rec+8)
 
         if blen < 0:
-            if self.base_verbose > 2:
+            if self.verbose > 2:
                 print("Invalid key length %d at %d" % (blen, rec))
             return cnt2
 
         data = self.getbuffstr(rec+12, blen)
-        if base_integrity:
+        if self.integrity:
             ccc = self.hash32(data)
-            if self.base_verbose > 1:
+            if self.verbose > 1:
                 print("rec", rec, "hash", hex(hash), "check", hex(ccc))
             if hash != ccc:
-                if self.base_verbose > 0:
+                if self.verbose > 0:
                     print("Error on hash at rec", rec, "hash", hex(hash),
 "check", hex(ccc))
                 return []
 
         endd = self.getbuffstr(rec + 12 + blen, self.INTSIZE)
         if endd != RECSEP:
-            if self.base_verbose > 0:
+            if self.verbose > 0:
                 print(" Damaged data (sep) '%s' at" % endd, rec)
             return cnt2
 
         rec2 = rec + 16 + blen;
         hash2 = self.getbuffint(rec2)
         blen2 = self.getbuffint(rec2+4)
 
         if blen2 < 0:
-            if self.base_verbose > 1:
+            if self.verbose > 1:
                 print("Invalid data length %d at %d" % (blen2, rec))
             return cnt2
 
         data2 = self.getbuffstr(rec2+8, blen2)
-        if base_integrity:
+        if self.integrity:
             ccc2 = self.hash32(data2)
-            if self.base_verbose > 1:
+            if self.verbose > 1:
                 print("rec", rec, "hash2", hex(hash), "check2", hex(ccc))
             if hash2 != ccc2:
-                if self.base_verbose > 0:
+                if self.verbose > 0:
                     print("Error on hash at rec", rec, "hash2", hex(hash),
 "check2", hex(ccc))
                 return []
 
-        if self.base_verbose > 2:
+        if self.verbose > 2:
             print("%-5d pos %5d" % (cnt, rec), "%8x" % hash, "len", blen, data,
                                                         "%8x" % hash2,"len",
 blen2, data2)
 
-        elif self.base_verbose > 1:
+        elif self.verbose > 1:
             print("%-5d pos %5d" % (cnt, rec), "%8x" % hash, "len", blen, data,
                                                         "%8x" % hash2,"len",
 blen2, data2)
-        elif self.base_verbose:
+        elif self.verbose:
             print("%-5d pos %5d" % (cnt, rec),  data, data2)
         else:
             print("%-5d pos %5d" % (cnt, rec), "Data:", truncs(data, 18),
 "Data2:", truncs(data2, 18))
 
         cnt2 += 1
         return cnt2
@@ -430,73 +431,73 @@
         ''' Check record. Verbose to the screen. Return number of errors.'''
 
         ret = 0
         sig = self.getbuffstr(rec, self.INTSIZE)
 
         # Do not check deleted, say OK
         if sig == RECDEL:
-            if self.base_verbose > 1:
+            if self.verbose > 1:
                 print(" Deleted data '%s' at %d (%d)" % (sig, rec, cnt2))
             ret = 1
             return ret
 
         if sig != RECSIG:
-            if self.base_verbose > 0:
+            if self.verbose > 0:
                 print(" Damaged data (sig) '%s' at %d (%d)" % (sig, rec, cnt2))
-            #if self.base_verbose > 1:
+            #if self.verbose > 1:
             #    print("Data", data)
 
             return ret
 
         hash = self.getbuffint(rec+4)
         blen = self.getbuffint(rec+8)
 
         if blen <= 0:
-            if self.base_verbose > 1:
+            if self.verbose > 1:
                 print("Invalid key length %d at %d" % (blen, rec))
             return ret
 
         data = self.getbuffstr(rec+12, blen)
         ccc = self.hash32(data)
         if hash != ccc:
-            if self.base_verbose > 1:
+            if self.verbose > 1:
                 print("Data", data)
-            elif self.base_verbose > 0:
+            elif self.verbose > 0:
                 print("Error on hash at rec", rec, cnt2, "hash",
                                             hex(hash), "check", hex(ccc))
 
             return ret
 
         endd = self.getbuffstr(rec + 12 + blen, self.INTSIZE)
         if endd != RECSEP:
-            if self.base_verbose > 0:
+            if self.verbose > 0:
                 print(" Damaged data (sep) '%s' at %d %d %d" % (endd, rec,
 cnt2))
             return ret
 
         rec2 = rec + 16 + blen;
         hash2 = self.getbuffint(rec2)
         blen2 = self.getbuffint(rec2+4)
 
         if blen2 < 0:
-            if self.base_verbose > 1:
+            if self.verbose > 1:
                 print("Invalid data length2 %d at %d" % (blen2, rec))
             return ret
 
         data2 = self.getbuffstr(rec2+8, blen2)
         ccc2 = self.hash32(data2)
         if hash2 != ccc2:
-            if self.base_verbose > 1:
+            if self.verbose > 1:
                 print("Data", data, "Data2", data2)
-            elif self.base_verbose > 0:
+            elif self.verbose > 0:
                 print("Error on hash2 at rec", rec, cnt2, "hash2",
                                         hex(hash2), "check2", hex(ccc2))
             return ret
 
-        if self.base_verbose > 2:
+        if self.verbose > 2:
             print("Record at %d (%d) OK." % (rec, cnt2))
 
         ret += 1
         return ret
 
     # --------------------------------------------------------------------
     # Internal; no locking
@@ -521,26 +522,23 @@
             rrr = range(chash - self.INTSIZE * 2, HEADSIZE  - self.INTSIZE * 2,
 -self.INTSIZE * 2)
 
         for aa in rrr:
             rec = self.getidxint(aa)
 
             #print(aa, rec)
-            if not base_quiet:
-                cnt2 += 1
-                ret = self.dump_rec(rec, cnt)
-
-                if not ret:
-                    if self.pgdebug > 5:
-                        print("Deleted / empty record at", cnt)
-
-                if ret:
-                    cnt += 1
-                    if cnt >= lim:
-                        break
+            cnt2 += 1
+            ret = self.dump_rec(rec, cnt)
+            if not ret:
+                if self.pgdebug > 5:
+                    print("Deleted / empty record at", cnt)
+            if ret:
+                cnt += 1
+                if cnt >= lim:
+                    break
 
     def  dump_data(self, lim = INT_MAX, skip = 0):
 
         ''' Put all data to screen. '''
 
         self.__dump_data(lim, skip, 1)
 
@@ -550,17 +548,17 @@
 
         self.__dump_data(lim, skip)
 
     def  reindex(self):
 
         ''' Re create index file. '''
 
-        self.lock.waitlock() #self.lckname)
+        self.lock.waitlock()
         ret = self.__reindex()
-        self.lock.unlock()    #dellock(self.lckname)
+        self.lock.unlock()
         return ret
 
     # --------------------------------------------------------------------
 
     def  __reindex(self):
 
         ''' Recover index. Make sure the DB in not in session.  '''
@@ -581,50 +579,50 @@
         tmplock = FileLock(relock)
         tmplock.waitlock()
 
         tempifp = self.softcreate(reidx)
         self.create_idx(tempifp)
         dlen = self.getsize(self.fp)
 
-        if self.base_verbose > 2:
+        if self.verbose > 2:
            print("curr", curr, "dlen", dlen)
 
         aa =  HEADSIZE
         while 1:
             if aa >= dlen:
                 break
 
             sig = self.getbuffstr(aa, self.INTSIZE)
             # Check if sig is correct
             if sig != RECSIG:
-                if self.core_verbose > 0:
+                if self.verbose > 0:
                     print("Invalid sig .. resync needed")
                 raise
 
             #print("reind", aa)
 
             try:
                 hhh2 = self.getbuffint(aa + 4)
                 lenx = self.getbuffint(aa + 8)
                 if lenx < 0:
-                    if self.core_verbose > 0:
+                    if self.verbose > 0:
                         print("Invalid key length.")
                 sep =  self.getbuffstr(aa + 12 + lenx, self.INTSIZE)
                 len2 =  self.getbuffint(aa + 20 + lenx)
                 if len2 < 0:
-                    if self.core_verbose > 0:
+                    if self.verbose > 0:
                         print("Invalid record length")
             except:
-                if self.core_verbose > 2:
+                if self.verbose > 2:
                     print("in reindex", sys.exc_info())
 
-            if self.base_verbose == 1:
+            if self.verbose == 1:
                 print(aa, "sig", sig, "hhh2", hex(hhh2), "len", lenx, \
                     "sep", sep, "len2", len2)
-            if self.base_verbose > 1:
+            if self.verbose > 1:
                 data =  self.getbuffstr(aa + 12, lenx)
                 data2 =  self.getbuffstr(aa + 24 + lenx, len2)
                 print(aa, "sig", sig, "data", data, "data2", data2)
 
             # Update / Append index
             #hashpos = self._getint(tempifp, CURROFFS)
             hashpos =  HEADSIZE  + self._getdbsize(tempifp) * self.INTSIZE * 2
@@ -697,17 +695,17 @@
         '''
             Remove all deleted data. Reindex.
             The db is locked while the vacuum is in operation, but
             make sure the DB in not in session, and no pending
             operations are present (like find / retrieve cycle).
         '''
 
-        self.lock.waitlock() #self.lckname)
+        self.lock.waitlock()
         ret = self._vacuum()
-        self.lock.unlock()  #dellock(self.lckname)
+        self.lock.unlock()
         return ret
 
     def  _vacuum(self):
 
         vacname = os.path.splitext(self.fname)[0] + "_vac_" + ".pydb"
         vacerr  = os.path.splitext(self.fname)[0] +  ".perr"
         vacidx = os.path.splitext(vacname)[0]  + ".pidx"
@@ -744,24 +742,21 @@
                 sig = self.getbuffstr(rec, self.INTSIZE)
                 if sig == RECDEL:
                     ret += 1
                     vac += 1
                     if self.pgdebug > 1:
                         print("deleted", rec)
                 elif sig != RECSIG:
-                    if self.base_verbose:
+                    if self.verbose:
                         print("Detected error at %d" % rec)
                     ret += 1
                     self.__save_error(rec, vacerrfp)
                 else:
-                    global base_integrity
-                    tmpi = base_integrity
-                    base_integrity = True
+                    self.integrity = True
                     arr = self.get_rec_byoffs(rec)
-                    base_integrity = tmpi
 
                     if self.pgdebug > 1:
                         print(cnt, "vac rec", rec, arr)
 
                     if len(arr) > 1:
                         hhh2 = self.hash32(arr[0])
                         hhh3 = self.hash32(arr[1])
@@ -773,105 +768,104 @@
                         if self.pgdebug > 0:
                             print("Error on vac: %d" % rec)
                 cnt += 1
 
             vacdb.fp.close()
             vacdb.ifp.close()
 
-            vacdb.lock.unlock()  #dellock(vacdb.lckname)
+            vacdb.lock.unlock()
 
             # if vacerr is empty
             try:
                 if os.stat(vacerr).st_size == 0:
                     #print("Vac error empty")
                     os.remove(vacerr)
             except:
-                if self.core_verbose > 0:
+                if self.verbose > 0:
                     print("vacerr", sys.exc_info())
 
         # Any vacummed?
         if vac > 0:
             # Make it go out of scope
             self.fp.flush(); self.ifp.flush()
             self.fp.close(); self.ifp.close()
 
             # Now move files
             try:
                 os.remove(self.fname);
             except:
-                if self.core_verbose > 0:
+                if self.verbose > 0:
                     print("vacuum remove", self.fname, sys.exc_info())
                 pass
 
             try:
                 os.remove(self.idxname)
             except:
-                if self.core_verbose > 2:
+                if self.verbose > 2:
                     print("vacuum idx remove", self.idxname, sys.exc_info())
                 pass
 
             if self.pgdebug > 1:
                 print("rename", vacname, "->", self.fname)
                 print("rename", vacidx, "->", self.idxname)
 
             try:
                 os.rename(vacname, self.fname)
             except:
-                if self.core_verbose > 2:
+                if self.verbose > 2:
                     print("vacuum rename", vacname, sys.exc_info())
             try:
                 os.rename(vacidx, self.idxname)
             except:
-                if self.core_verbose > 2:
+                if self.verbose > 2:
                     print("vacuum idx rename", vacidx, sys.exc_info())
 
-            self.lock.waitlock() #self.lckname)
+            self.lock.waitlock()
             self.fp = self.softcreate(self.fname)
             self.ifp = self.softcreate(self.idxname)
-            #self.lock.unlock()  #dellock(self.lckname)
+            #self.lock.unlock()
 
         else:
             # Just remove non vacuumed files
             if self.pgdebug > 1:
                 print("deleted", vacname, vacidx)
             try:
                 os.remove(vacname)
                 os.remove(vacidx)
             except:
                 pass
 
         #self.lock.unlock()
-        #dellock(self.lckname)
+
 
         #print("ended vacuum")
         return ret, vac
 
     def  get_rec(self, recnum):
 
         ''' Get record from database; recnum is a zero based record counter.
 '''
 
         if self.pgdebug:
-            print("getrec()", recnum)
+            print("get_rec()", recnum)
 
         rsize = self._getdbsize(self.ifp)
         if recnum >= rsize:
-            if self.core_verbose > 0:
+            if self.verbose > 0:
                 print("Past end of data.");
-            raise  RuntimeError( \
-                    "Past end of Data. Asking for %d while max is 0 .. %d
-records." \
-                                     % (recnum, rsize-1) )
+            errx =  "Past end of Data. (ask: %d max: %d)"  % (recnum, rsize-1)
+            raise  RuntimeError(errx)
             return []
 
         chash = self.getidxint(CURROFFS)
         #print("chash", chash)
         offs = self.getidxint(HEADSIZE + recnum * self.INTSIZE * 2)
 
-        #print("offs", offs)
+        #sig = self.getbuffstr(offs, self.INTSIZE)
+
         return self._rec2arr(offs)
 
     def  get_rec_byoffs(self, recoffs):
 
         ''' Return record by offset. '''
 
         rsize = self.getsize(self.fp)
@@ -880,19 +874,18 @@
             raise  RuntimeError( \
                     "Past end of File. Asking for offset %d file size is %d." \
                                      % (recoffs, rsize) )
             return []
 
         sig = self.getbuffstr(recoffs, self.INTSIZE)
         if sig == RECDEL:
-            if self.base_verbose:
+            if self.verbose:
                 print("Deleted record.")
-            return []
         if sig != RECSIG:
-            if self.core_verbose > 0:
+            if self.verbose > 0:
                 print("Unlikely offset %d is not at record boundary." %
 recoffs, sig)
             return []
         #print("recoffs", recoffs)
         return self._rec2arr(recoffs)
 
     def  get_key_offs(self, recoffs):
@@ -905,19 +898,19 @@
             raise  RuntimeError( \
                     "Past end of File. Asking for offset %d file size is %d." \
                                      % (recoffs, rsize) )
             return []
 
         sig = self.getbuffstr(recoffs, self.INTSIZE)
         if sig == RECDEL:
-            if self.base_verbose:
+            if self.verbose:
                 print("Deleted record.")
             return []
         if sig != RECSIG:
-            if self.core_verbose > 0:
+            if self.verbose > 0:
                 print("Unlikely offset %d is not at record boundary." %
 recoffs, sig)
             return []
         #print("recoffs", recoffs)
         return self._rec2arr(recoffs)[0]
 
     def  del_rec(self, recnum):
@@ -926,24 +919,24 @@
             Deleted record is marked as deleted but not removed.
             Deleted records are ignored in further operations.
             Use 'vacuum' to actually remove record.
         '''
 
         rsize = self._getdbsize(self.ifp)
         if recnum >= rsize:
-            if self.base_verbose:
+            if self.verbose:
                 print("Past end of data.");
             return False
         chash = self.getidxint(CURROFFS)
         #print("chash", chash)
         offs = self.getidxint(HEADSIZE + recnum * self.INTSIZE * 2)
         #print("offs", offs)
         old = self.getbuffstr(offs, self.INTSIZE)
         if old == RECDEL:
-            if self.base_verbose:
+            if self.verbose:
                 print("Record at %d already deleted." % offs);
             return False
 
         self.putbuffstr(offs, RECDEL)
         return True
 
     def  del_rec_offs(self, recoffs):
@@ -956,15 +949,15 @@
             raise  RuntimeError( \
                     "Past end of File. Asking for offset %d file size is %d." \
                                      % (recoffs, rsize) )
             return False
 
         sig = self.getbuffstr(recoffs, self.INTSIZE)
         if sig != RECSIG  and sig != RECDEL:
-            if self.core_verbose > 0:
+            if self.verbose > 0:
                 print("Unlikely offset %d is not at record boundary." %
 recoffs, sig)
             return False
 
         self.putbuffstr(recoffs, RECDEL)
         return True
 
@@ -972,30 +965,30 @@
 
     def integrity_check(self, skip = 0, count = 0xffffffff):
 
         ''' Check record integrity for 'count' records.
             Skip number of records.
         '''
 
-        self.lock.waitlock()    #(self.lckname)
+        self.lock.waitlock()
         ret = 0; cnt2 = 0; cnt3 = 0;
         #chash = self.getidxint(CURROFFS)        #;print("chash", chash)
         chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
         # Direction sensitivity
         rrr = range(HEADSIZE + skip * self.INTSIZE * 2, chash, self.INTSIZE *
 2)
         for aa in rrr:
             rec = self.getidxint(aa)
             #print(aa, rec)
             ret += self.check_rec(rec, cnt2)
             cnt2 += 1
             cnt3 += 1
             if cnt3 >= count:
                 break
-        self.lock.unlock() #dellock(self.lckname)
+        self.lock.unlock()
         return ret, cnt2
 
     def  retrieve(self, strx, limx = 1):
 
         ''' Retrive in reverse, limit it. '''
 
         if type(strx) != type(b""):
@@ -1007,34 +1000,34 @@
 
         #chash = self.getidxint(CURROFFS)
         chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
 
         #;print("chash", chash)
         arr = []
 
-        self.lock.waitlock() #(self.lckname)
+        self.lock.waitlock()
 
         #for aa in range(HEADSIZE + self.INTSIZE * 2, chash, self.INTSIZE * 2):
         for aa in range(chash - self.INTSIZE * 2, HEADSIZE  - self.INTSIZE * 2,
 -self.INTSIZE * 2):
             rec = self.getidxint(aa)
             sig = self.getbuffstr(rec, self.INTSIZE)
             if sig == RECDEL:
-                if self.base_verbose > 3:
+                if self.verbose > 3:
                     print(" Deleted record '%s' at" % sig, rec)
             elif sig != RECSIG:
-                if self.base_verbose:
+                if self.verbose:
                     print(" Damaged data '%s' at" % sig, rec)
             else:
                 hhh = self.getbuffint(rec+4)
                 if hhh == hhhh:
                     arr.append(self.get_rec_byoffs(rec))
                     if len(arr) >= limx:
                         break
-        self.lock.unlock()  #dellock(self.lckname)
+        self.lock.unlock()
 
         return arr
 
     # Return record offset
 
     def  _recoffset(self, strx, limx = INT_MAX, skipx = 0):
 
@@ -1052,38 +1045,40 @@
 
         #for aa in range(HEADSIZE + self.INTSIZE * 2, chash, self.INTSIZE * 2):
         for aa in range(chash - self.INTSIZE * 2, HEADSIZE  - self.INTSIZE * 2,
 -self.INTSIZE * 2):
             rec = self.getidxint(aa)
             sig = self.getbuffstr(rec, self.INTSIZE)
             if sig == RECDEL:
-                if base_showdel:
+                if self.showdel:
                     print(" Deleted record '%s' at" % sig, rec)
             elif sig != RECSIG:
-                if self.base_verbose > 0:
+                if self.verbose > 0:
                     print(" Damaged data '%s' at" % sig, rec)
             else:
                 blen = self.getbuffint(rec+8)
                 keyz = self.getbuffstr(rec + 12, blen)
-                if self.base_verbose > 1:
+                if self.verbose > 1:
                     print("_recoffset", keyz)
                 if strx2 == keyz:
                     sig = self.getbuffstr(rec + 16 + blen,  self.INTSIZE)
                     xlen = self.getbuffint(rec + 20 + blen)
                     data = self.getbuffstr(rec + 24 + blen, xlen)
                     #print("rec offset", rec + 12,  "key:", keyz, "data:",
 data)
                     break       # Only the last one
         return rec, rec+24 + blen, len(data)
 
     def  findrec(self, strx, limx = INT_MAX, skipx = 0):
 
-        ''' Find by string matching substring. '''
+        ''' Find key by matching strx with substring.
+        Return record(s).
+        '''
 
-        self.lock.waitlock()    #(self.lckname)
+        self.lock.waitlock()
 
         #chash = self.getidxint(CURROFFS)            #;print("chash", chash)
         chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
 
         arr = []
         strx2 = strx.encode(errors='strict');
 
@@ -1091,116 +1086,116 @@
 
         #for aa in range(HEADSIZE + self.INTSIZE * 2, chash, self.INTSIZE * 2):
         for aa in range(chash - self.INTSIZE * 2, HEADSIZE  - self.INTSIZE * 2,
 -self.INTSIZE * 2):
             rec = self.getidxint(aa)
             sig = self.getbuffstr(rec, self.INTSIZE)
             if sig == RECDEL:
-                if base_showdel:
+                if self.showdel:
                     print(" Deleted record '%s' at" % sig, rec)
             elif sig != RECSIG:
-                if self.base_verbose > 0:
+                if self.verbose > 0:
                     print(" Damaged data '%s' at" % sig, rec)
             else:
                 blen = self.getbuffint(rec+8)
                 data = self.getbuffstr(rec + 12, blen)
-                if self.base_verbose > 1:
+                if self.verbose > 1:
                     print("find", data)
                 #if str(strx2) in str(data):
                 if strx2 in data:
                     arr.append(self.get_key_offs(rec))
                     #arr.append(rec)
 
                     if len(arr) >= limx:
                         break
-        self.lock.unlock()  #dellock(self.lckname)
+        self.lock.unlock()
 
         return arr
 
     def  findrecpos(self, strx, limx = INT_MAX, skipx = 0):
 
-        ''' Find record, return array of positions. '''
+        ''' Find record by key, return array of positions. '''
 
-        self.lock.waitlock()    #(self.lckname)
+        self.lock.waitlock()
         chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
         arr = []
         if type(strx) != type(b""):
             strx = strx.encode(errors='strict');
 
         for aa in range(chash - self.INTSIZE * 2, HEADSIZE  - self.INTSIZE * 2,
 -self.INTSIZE * 2):
             rec = self.getidxint(aa)
             sig = self.getbuffstr(rec, self.INTSIZE)
             if sig == RECDEL:
-                if base_showdel:
+                if self.showdel:
                     print(" Deleted record '%s' at" % sig, rec)
             elif sig != RECSIG:
-                if self.base_verbose > 0:
+                if self.verbose > 0:
                     print(" Damaged data '%s' at" % sig, rec)
             else:
                 blen = self.getbuffint(rec+8)
                 data = self.getbuffstr(rec + 12, blen)
-                if self.base_verbose > 1:
+                if self.verbose > 1:
                     print("frecpos", data)
                 if strx == data:
                     arr.append(rec)
                     if len(arr) >= limx:
                         break
 
-        self.lock.unlock()  #dellock(self.lckname)
+        self.lock.unlock()
 
         return arr
 
-    def  findrec(self, strx, limx = INT_MAX, skipx = 0):
+    def  findrecsub(self, strx, limx = INT_MAX, skipx = 0):
 
-        ''' Find by string matching substring. '''
+        ''' Find record by matching substring. '''
 
-        self.lock.waitlock()    #(self.lckname)
+        self.lock.waitlock()
         chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
         arr = []
         if type(strx) != type(b""):
             strx2 = strx.encode(errors='strict');
 
         #print("findrec", strx2)
 
         #for aa in range(HEADSIZE + self.INTSIZE * 2, chash, self.INTSIZE * 2):
         for aa in range(chash - self.INTSIZE * 2, HEADSIZE  - self.INTSIZE * 2,
 -self.INTSIZE * 2):
             rec = self.getidxint(aa)
             sig = self.getbuffstr(rec, self.INTSIZE)
             if sig == RECDEL:
-                if base_showdel:
+                if self.showdel:
                     print(" Deleted record '%s' at" % sig, rec)
             elif sig != RECSIG:
-                if self.base_verbose > 0:
+                if self.verbose > 0:
                     print(" Damaged data '%s' at" % sig, rec)
             else:
                 blen = self.getbuffint(rec+8)
                 data = self.getbuffstr(rec + 12, blen)
-                if self.base_verbose > 1:
+                if self.verbose > 1:
                     print("find", data)
                 #if str(strx2) in str(data):
                 if strx2 in data:
                     #arr.append(self.get_key_offs(rec))
                     #arr.append(rec)
                     arr.append(self._rec2arr(rec))
                     if len(arr) >= limx:
                         break
-        self.lock.unlock()    #dellock(self.lckname)
+        self.lock.unlock()
 
         return arr
 
     # --------------------------------------------------------------------
     # List all active records
 
     def  listall(self):
 
         ''' List all active records. Return array id record indexes. '''
 
-        self.lock.waitlock()    #(self.lckname)
+        self.lock.waitlock()
         keys = []; arr = []; cnt = 0
 
         chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
         maxrec = chash - self.INTSIZE * 2
         rsize = self._getdbsize(self.ifp) - 1
 
         rrr =  range(maxrec,
@@ -1208,39 +1203,42 @@
         for aa in rrr:
             rec = self.getidxint(aa)
 
             #print(" Scanning at %d %d" % (rec, cnt))
 
             sig = self.getbuffstr(rec, self.INTSIZE)
             if sig == RECDEL:
-                if 1: #base_showdel:
+                if 1: #self.showdel:
                     print("Deleted record '%s' at" % sig, rec)
             elif sig != RECSIG:
-                if 1: #self.base_verbose > 0:
+                if 1: #self.verbose > 0:
                     print(" Damaged data '%s' at" % sig, rec)
             else:
                     hhh = self.getbuffint(rec+4)
                     print(" Good data '%s' at" % sig, rec, hhh)
                     if hhh not in keys:
                         keys.append(hhh)
                         # as we are going backwards
                         arr.append(rsize - cnt)
                         #print("found", hhh)
             cnt += 1
 
         keys = []
-        self.lock.unlock()  #dellock()self.lckname)
+        self.lock.unlock()
 
         return arr
 
     def  find_key(self, keyx, limx = 0xffffffff):
 
-        ''' Find record by key Search from the end, so latest comes first. '''
+        ''' Find record by key value.
+            Search from the end, so latest comes first.
+            This operates on the hash, so it reaches the answer fast.
+        '''
 
-        self.lock.waitlock()   #self.lckname)
+        self.lock.waitlock()
 
         skip = 0; arr = []; cnt = 0
         try:
             arg2e = keyx.encode()
         except:
             arg2e = keyx
 
@@ -1252,32 +1250,32 @@
                 HEADSIZE - self.INTSIZE * 2, -self.INTSIZE * 2)
         for aa in rrr:
             rec = self.getidxint(aa)
             #print(" Scanning at %d %d" % (rec, cnt))
 
             sig = self.getbuffstr(rec, self.INTSIZE)
             if sig == RECDEL:
-                if base_showdel:
+                if self.showdel:
                     print("Deleted record '%s' at" % sig, rec)
             elif sig != RECSIG:
-                if self.base_verbose > 0:
+                if self.verbose > 0:
                     print(" Damaged data '%s' at" % sig, rec)
             else:
                 hhh = self.getbuffint(rec+4)
                 if hhh == hhhh:
                     if len(arr) >= limx - 1:
                         arr.append(["More data ...",])
                         break
                     arr.append(rec)
                 else:
                     pass
                     #print("no match", hex(hhh))
 
             cnt += 1
-        self.lock.unlock()  #dellock()self.lckname)
+        self.lock.unlock()
 
         return arr
 
 
     def  del_data(self, hash, skip = 1):
 
         ''' Delete data by hash. '''
@@ -1298,15 +1296,15 @@
             #    print(" Damaged data '%s' at" % sig, rec)
 
             #blen = self.getbuffint(rec+8)
             #print("data '%s' at" % sig, rec, "blen", blen)
 
             hhh = self.getbuffint(rec+4)
             if hash == hhh:
-                if self.base_verbose > 0:
+                if self.verbose > 0:
                     print("Would delete", hhh)
 
             self.putbuffstr(rec, RECDEL)
 
             cnt += 1
 
         return arr
@@ -1331,15 +1329,15 @@
         ''' Delete records by key string; needs bin str, converted
             automatically on entry.
         '''
 
         if type(strx) != type(b""):
             strx = strx.encode()
 
-        if self.base_verbose > 1:
+        if self.verbose > 1:
             print("Start delete ", strx, "skip", skip)
 
         cnt = 0; cnt3 = 0
         #chash = self.getidxint(CURROFFS)    #;print("chash", chash)
         chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
 
         # Direction sensitivity
@@ -1351,60 +1349,60 @@
 -self.INTSIZE * 2)
 
         #for aa in range(HEADSIZE, chash, self.INTSIZE * 2):
         for aa in rrr:
             rec = self.getidxint(aa)
             sig = self.getbuffstr(rec, self.INTSIZE)
             if sig == RECDEL:
-                if base_showdel:
+                if self.showdel:
                     print(" Deleted record '%s' at" % sig, rec)
             elif sig != RECSIG:
-                if self.base_verbose > 0:
+                if self.verbose > 0:
                     print(" Damaged data '%s' at" % sig, rec)
             else:
                 blen = self.getbuffint(rec+8)
                 data = self.getbuffstr(rec + 12, blen)
-                if self.base_verbose > 2:
+                if self.verbose > 2:
                     print("del iterate recs", cnt3, data, strx)
 
                 if strx == data:
-                    if self.base_verbose > 0:
+                    if self.verbose > 0:
                         print("Deleting", cnt3, aa, data)
                     self.putbuffstr(rec, RECDEL)
                     cnt += 1
                     if cnt >= maxdelrec:
                         break
             cnt3 += 1
         return cnt
 
     def  save_data(self, header, datax, replace = False):
 
         ''' Append to the end of file. If replace flag is set, try to overwrite
-            in place. If new record is larger, add it as ususal. If smaller,
+            in place. If new record is larger, add it as usual. If smaller,
             the record is padded with spaces. This should not influence most
 ops.
             (like: int())
             This feature allows the database update wthout creating new
 records.
-            Useful for counters or dynamically changing data.
+            Useful for counters or dynamically changing data. To be useful,
+            use  create fixed size data. Like sprintf(%12d).
 
                     Input:
                         header     Header
                         datax      Data
 
                      Return:
                         The offset of saved data
             '''
 
         if self.pgdebug > 0:
             print("Save_data()", header, datax)
 
-        self.lock.waitlock()   #self.lckname)
-        ret = 0
-        was = False
+        self.lock.waitlock()
+        ret = 0 ; was = False
         # Put new data in place
         if replace:
             if type(datax) != type(b""):
                 mrep2 = datax.encode()
             else:
                 mrep2 = datax
 
@@ -1419,17 +1417,18 @@
                     ccc = self.hash32(padded)
                     self.putbuffint(rrr[1] - 8, ccc)
                     #print("ccc", hex(ccc))
                     self.putbuffstr(rrr[1], padded)
                     was = True
                     ret =  rrr[0]
         if not was:
+            #print("Saving longer data", header, datax)
             ret = self._save_data2(header, datax)
 
-        self.lock.unlock()  #dellock()self.lckname)
+        self.lock.unlock()
 
         return ret
 
     # --------------------------------------------------------------------
     # Save data to database file
 
     def  _save_data2(self, arg2, arg3):
@@ -1494,15 +1493,15 @@
         self.putidxint(curr, dcurr)
         self.putidxint(curr + self.INTSIZE, hhh2)
         #self.putidxint(CURROFFS, self.ifp.tell())
 
         self.fp.flush()
         self.ifp.flush()
 
-        return curr
+        return dcurr
 
     def __del__(self):
 
         ''' flush file handles and close files. '''
 
         if hasattr(self, "pgdebug"):
             if self.pgdebug > 9:
@@ -1518,14 +1517,18 @@
 
         if hasattr(self, "ifp"):
                 if self.ifp:
                     if not self.ifp.closed:
                         self.ifp.flush()
                         self.ifp.close()
 
+        # remove lockfile
+        if hasattr(self, "lock"):
+            self.lock.unlock()
+
 # EOF
 ********** CCllaasssseess **********
   class TwinCore (fname='pydbase.pydb', pgdebug=0, devmode=1)
       Data file and index file; protected by locks The TWIN refers to separate
       files for data / index.
       Expand source code
       class TwinCore(TwinCoreBase):
@@ -1540,21 +1543,22 @@
           def __init__(self, fname = "pydbase.pydb", pgdebug = 0, devmode = 1):
 
               self.cnt = 0
               self.fname = fname
               self.lckname  = os.path.splitext(self.fname)[0] + ".lock"
               self.idxname  = os.path.splitext(self.fname)[0] + ".pidx"
               self.pgdebug = pgdebug
-              self.base_verbose  = 0
-              self.core_verbose  = 0
+              self.verbose  = 0
+              self.showdel  = 0
+              self.integrity = 0
               self.devmode = devmode
               self.lock = FileLock(self.lckname)
 
               # Make sure only one process can use this
-              self.lock.waitlock() #self.lckname)
+              self.lock.waitlock()
 
               super(TwinCore, self).__init__(pgdebug)
 
               #print("initializing core with", fname, pgdebug)
               #self.pool = threading.BoundedSemaphore(value=1)
 
               # It was informative at one point
@@ -1599,31 +1603,27 @@
                   #self.ifp = self.softcreate(self.idxname)
                   indexsize = self.getsize(self.ifp)
 
                   # See if valid index
                   if indexsize < HEADSIZE:
                       self.create_idx(self.ifp)
                       # It was an existing data, new index needed
-                      if self.base_verbose > 0:
+                      if self.verbose > 0:
                           print("Reindexing")
                       self.__reindex()
 
               # Check
               if  self.getbuffstr(0, 4) != FILESIG:
-                  if self.base_verbose > 2:
+                  if self.verbose > 2:
                       print("Invalid data signature")
-                  self.lock.unlock()  #dellock(self.lckname)
+                  self.lock.unlock()
                   raise  RuntimeError("Invalid database signature.")
 
               #print("buffsize", buffsize, "indexsize", indexsize)
-              self.lock.unlock() #dellock(self.lckname)
-
-          def version(self):
-              ''' Return version sting. '''
-              return Version
+              self.lock.unlock()
 
           def flush(self):
 
               ''' Flush files to disk. '''
 
               if self.pgdebug > 9:
                   print("Flushing", self.fp, self.ifp)
@@ -1665,65 +1665,69 @@
 
               return  ret
 
           # -------------------------------------------------------------------
       -
           def _rec2arr(self, rec):
 
+              # Wed 10.Apr.2024 decision is made at the higher level
               arr = []
               sig = self.getbuffstr(rec, self.INTSIZE)
 
-              if sig == RECDEL:
-                  return arr
-
-              if sig != RECSIG:
-                  if self.base_verbose > 0:
+              if sig != RECSIG and sig != RECDEL:
+                  if self.verbose > 0:
                       print(" Damaged data (sig) '%s' at" % sig, rec)
                   return arr
 
               hash = self.getbuffint(rec+4)
               blen = self.getbuffint(rec+8)
               data = self.getbuffstr(rec + 12, blen)
 
-              if base_integrity:
+              if self.integrity:
                   ccc = self.hash32(data)
-                  if self.base_verbose > 1:
+                  if self.verbose > 1:
                       print("rec", rec, "hash", hex(hash), "check", hex(ccc))
                   if hash != ccc:
-                      if self.base_verbose > 0:
+                      if self.verbose > 0:
                           print("Error on hash at rec", rec, "hash", hex(hash),
       "check", hex(ccc))
                       return []
 
               #print("%5d pos %5d" % (cnt, rec), "hash %8x" % hash, "ok", ok,
       "len=", blen, end=" ")
 
               endd = self.getbuffstr(rec + 12 + blen, self.INTSIZE)
               if endd != RECSEP:
-                  if self.base_verbose > 0:
+                  if self.verbose > 0:
                       print(" Damaged data (sep) '%s' at" % endd, rec)
                   return arr
 
               rec2 = rec + 16 + blen;
               hash2 = self.getbuffint(rec2)
               blen2 = self.getbuffint(rec2+4)
               data2 = self.getbuffstr(rec2+8, blen2)
 
-              if base_integrity:
+              if self.integrity:
                   ccc2 = self.hash32(data2)
-                  if self.base_verbose > 1:
+                  if self.verbose > 1:
                       print("rec", rec, "hash2", hex(hash2), "check2", hex
       (ccc2))
                   if hash2 != ccc2:
-                      if self.base_verbose > 0:
+                      if self.verbose > 0:
                           print("Error on hash at rec", rec, "hash2", hex
       (hash2), "check2", hex(ccc2))
                       return []
 
-              arr = [data, data2]
+              if sig == RECDEL:
+                  if self.showdel:
+                      arr = [b"del", data, data2]
+                  else:
+                      arr = []
+              else:
+                  arr = [data, data2]
               return arr
 
           # -------------------------------------------------------------------
           # Originator, dump single record
 
           def  dump_rec(self, rec, cnt):
 
@@ -1734,98 +1738,98 @@
 
               cnt2 = 0
               sig = self.getbuffstr(rec, self.INTSIZE)
               if self.pgdebug > 5:
                   print("Sig ", sig, "at", rec)
 
               if sig == RECDEL:
-                  if base_showdel:
+                  if self.showdel:
                       klen = self.getbuffint(rec+8)
                       kdata = self.getbuffstr(rec+12, klen)
                       rec2 = rec + 16 + klen;
                       blen = self.getbuffint(rec2+4)
                       data = self.getbuffstr(rec2+8, blen)
                       print(" Del at", rec, "key:", kdata, "data:", truncs
       (data))
-                  if self.base_verbose > 1:
+                  if self.verbose > 1:
                       klen = self.getbuffint(rec+8)
                       kdata = self.getbuffstr(rec+12, klen)
                       rec2 = rec + 16 + klen;
                       blen = self.getbuffint(rec2+4)
                       data = self.getbuffstr(rec2+8, blen)
-                      if self.base_verbose > 2:
+                      if self.verbose > 2:
                           print(" Del at", rec, "key:", kdata, "data:", data)
                       else:
                           print(" Del at", rec, "key:", kdata, "data:", truncs
       (data))
 
                   return cnt2
 
               if sig != RECSIG:
-                  if self.base_verbose > 1:
+                  if self.verbose > 1:
                       print(" Damaged data (sig) '%s' at" % sig, rec)
                   return cnt2
 
               hash = self.getbuffint(rec+4)
               blen = self.getbuffint(rec+8)
 
               if blen < 0:
-                  if self.base_verbose > 2:
+                  if self.verbose > 2:
                       print("Invalid key length %d at %d" % (blen, rec))
                   return cnt2
 
               data = self.getbuffstr(rec+12, blen)
-              if base_integrity:
+              if self.integrity:
                   ccc = self.hash32(data)
-                  if self.base_verbose > 1:
+                  if self.verbose > 1:
                       print("rec", rec, "hash", hex(hash), "check", hex(ccc))
                   if hash != ccc:
-                      if self.base_verbose > 0:
+                      if self.verbose > 0:
                           print("Error on hash at rec", rec, "hash", hex(hash),
       "check", hex(ccc))
                       return []
 
               endd = self.getbuffstr(rec + 12 + blen, self.INTSIZE)
               if endd != RECSEP:
-                  if self.base_verbose > 0:
+                  if self.verbose > 0:
                       print(" Damaged data (sep) '%s' at" % endd, rec)
                   return cnt2
 
               rec2 = rec + 16 + blen;
               hash2 = self.getbuffint(rec2)
               blen2 = self.getbuffint(rec2+4)
 
               if blen2 < 0:
-                  if self.base_verbose > 1:
+                  if self.verbose > 1:
                       print("Invalid data length %d at %d" % (blen2, rec))
                   return cnt2
 
               data2 = self.getbuffstr(rec2+8, blen2)
-              if base_integrity:
+              if self.integrity:
                   ccc2 = self.hash32(data2)
-                  if self.base_verbose > 1:
+                  if self.verbose > 1:
                       print("rec", rec, "hash2", hex(hash), "check2", hex(ccc))
                   if hash2 != ccc2:
-                      if self.base_verbose > 0:
+                      if self.verbose > 0:
                           print("Error on hash at rec", rec, "hash2", hex
       (hash), "check2", hex(ccc))
                       return []
 
-              if self.base_verbose > 2:
+              if self.verbose > 2:
                   print("%-5d pos %5d" % (cnt, rec), "%8x" % hash, "len", blen,
       data,
                                                               "%8x" %
       hash2,"len", blen2, data2)
 
-              elif self.base_verbose > 1:
+              elif self.verbose > 1:
                   print("%-5d pos %5d" % (cnt, rec), "%8x" % hash, "len", blen,
       data,
                                                               "%8x" %
       hash2,"len", blen2, data2)
-              elif self.base_verbose:
+              elif self.verbose:
                   print("%-5d pos %5d" % (cnt, rec),  data, data2)
               else:
                   print("%-5d pos %5d" % (cnt, rec), "Data:", truncs(data, 18),
       "Data2:", truncs(data2, 18))
 
               cnt2 += 1
               return cnt2
@@ -1836,74 +1840,74 @@
       errors.'''
 
               ret = 0
               sig = self.getbuffstr(rec, self.INTSIZE)
 
               # Do not check deleted, say OK
               if sig == RECDEL:
-                  if self.base_verbose > 1:
+                  if self.verbose > 1:
                       print(" Deleted data '%s' at %d (%d)" % (sig, rec, cnt2))
                   ret = 1
                   return ret
 
               if sig != RECSIG:
-                  if self.base_verbose > 0:
+                  if self.verbose > 0:
                       print(" Damaged data (sig) '%s' at %d (%d)" % (sig, rec,
       cnt2))
-                  #if self.base_verbose > 1:
+                  #if self.verbose > 1:
                   #    print("Data", data)
 
                   return ret
 
               hash = self.getbuffint(rec+4)
               blen = self.getbuffint(rec+8)
 
               if blen <= 0:
-                  if self.base_verbose > 1:
+                  if self.verbose > 1:
                       print("Invalid key length %d at %d" % (blen, rec))
                   return ret
 
               data = self.getbuffstr(rec+12, blen)
               ccc = self.hash32(data)
               if hash != ccc:
-                  if self.base_verbose > 1:
+                  if self.verbose > 1:
                       print("Data", data)
-                  elif self.base_verbose > 0:
+                  elif self.verbose > 0:
                       print("Error on hash at rec", rec, cnt2, "hash",
                                                   hex(hash), "check", hex(ccc))
 
                   return ret
 
               endd = self.getbuffstr(rec + 12 + blen, self.INTSIZE)
               if endd != RECSEP:
-                  if self.base_verbose > 0:
+                  if self.verbose > 0:
                       print(" Damaged data (sep) '%s' at %d %d %d" % (endd,
       rec, cnt2))
                   return ret
 
               rec2 = rec + 16 + blen;
               hash2 = self.getbuffint(rec2)
               blen2 = self.getbuffint(rec2+4)
 
               if blen2 < 0:
-                  if self.base_verbose > 1:
+                  if self.verbose > 1:
                       print("Invalid data length2 %d at %d" % (blen2, rec))
                   return ret
 
               data2 = self.getbuffstr(rec2+8, blen2)
               ccc2 = self.hash32(data2)
               if hash2 != ccc2:
-                  if self.base_verbose > 1:
+                  if self.verbose > 1:
                       print("Data", data, "Data2", data2)
-                  elif self.base_verbose > 0:
+                  elif self.verbose > 0:
                       print("Error on hash2 at rec", rec, cnt2, "hash2",
                                               hex(hash2), "check2", hex(ccc2))
                   return ret
 
-              if self.base_verbose > 2:
+              if self.verbose > 2:
                   print("Record at %d (%d) OK." % (rec, cnt2))
 
               ret += 1
               return ret
 
           # -------------------------------------------------------------------
       -
@@ -1929,26 +1933,23 @@
                   rrr = range(chash - self.INTSIZE * 2, HEADSIZE  -
       self.INTSIZE * 2, -self.INTSIZE * 2)
 
               for aa in rrr:
                   rec = self.getidxint(aa)
 
                   #print(aa, rec)
-                  if not base_quiet:
-                      cnt2 += 1
-                      ret = self.dump_rec(rec, cnt)
-
-                      if not ret:
-                          if self.pgdebug > 5:
-                              print("Deleted / empty record at", cnt)
-
-                      if ret:
-                          cnt += 1
-                          if cnt >= lim:
-                              break
+                  cnt2 += 1
+                  ret = self.dump_rec(rec, cnt)
+                  if not ret:
+                      if self.pgdebug > 5:
+                          print("Deleted / empty record at", cnt)
+                  if ret:
+                      cnt += 1
+                      if cnt >= lim:
+                          break
 
           def  dump_data(self, lim = INT_MAX, skip = 0):
 
               ''' Put all data to screen. '''
 
               self.__dump_data(lim, skip, 1)
 
@@ -1958,17 +1959,17 @@
 
               self.__dump_data(lim, skip)
 
           def  reindex(self):
 
               ''' Re create index file. '''
 
-              self.lock.waitlock() #self.lckname)
+              self.lock.waitlock()
               ret = self.__reindex()
-              self.lock.unlock()    #dellock(self.lckname)
+              self.lock.unlock()
               return ret
 
           # -------------------------------------------------------------------
       -
 
           def  __reindex(self):
 
@@ -1990,50 +1991,50 @@
               tmplock = FileLock(relock)
               tmplock.waitlock()
 
               tempifp = self.softcreate(reidx)
               self.create_idx(tempifp)
               dlen = self.getsize(self.fp)
 
-              if self.base_verbose > 2:
+              if self.verbose > 2:
                  print("curr", curr, "dlen", dlen)
 
               aa =  HEADSIZE
               while 1:
                   if aa >= dlen:
                       break
 
                   sig = self.getbuffstr(aa, self.INTSIZE)
                   # Check if sig is correct
                   if sig != RECSIG:
-                      if self.core_verbose > 0:
+                      if self.verbose > 0:
                           print("Invalid sig .. resync needed")
                       raise
 
                   #print("reind", aa)
 
                   try:
                       hhh2 = self.getbuffint(aa + 4)
                       lenx = self.getbuffint(aa + 8)
                       if lenx < 0:
-                          if self.core_verbose > 0:
+                          if self.verbose > 0:
                               print("Invalid key length.")
                       sep =  self.getbuffstr(aa + 12 + lenx, self.INTSIZE)
                       len2 =  self.getbuffint(aa + 20 + lenx)
                       if len2 < 0:
-                          if self.core_verbose > 0:
+                          if self.verbose > 0:
                               print("Invalid record length")
                   except:
-                      if self.core_verbose > 2:
+                      if self.verbose > 2:
                           print("in reindex", sys.exc_info())
 
-                  if self.base_verbose == 1:
+                  if self.verbose == 1:
                       print(aa, "sig", sig, "hhh2", hex(hhh2), "len", lenx, \
                           "sep", sep, "len2", len2)
-                  if self.base_verbose > 1:
+                  if self.verbose > 1:
                       data =  self.getbuffstr(aa + 12, lenx)
                       data2 =  self.getbuffstr(aa + 24 + lenx, len2)
                       print(aa, "sig", sig, "data", data, "data2", data2)
 
                   # Update / Append index
                   #hashpos = self._getint(tempifp, CURROFFS)
                   hashpos =  HEADSIZE  + self._getdbsize(tempifp) *
@@ -2107,17 +2108,17 @@
               '''
                   Remove all deleted data. Reindex.
                   The db is locked while the vacuum is in operation, but
                   make sure the DB in not in session, and no pending
                   operations are present (like find / retrieve cycle).
               '''
 
-              self.lock.waitlock() #self.lckname)
+              self.lock.waitlock()
               ret = self._vacuum()
-              self.lock.unlock()  #dellock(self.lckname)
+              self.lock.unlock()
               return ret
 
           def  _vacuum(self):
 
               vacname = os.path.splitext(self.fname)[0] + "_vac_" + ".pydb"
               vacerr  = os.path.splitext(self.fname)[0] +  ".perr"
               vacidx = os.path.splitext(vacname)[0]  + ".pidx"
@@ -2154,24 +2155,21 @@
                       sig = self.getbuffstr(rec, self.INTSIZE)
                       if sig == RECDEL:
                           ret += 1
                           vac += 1
                           if self.pgdebug > 1:
                               print("deleted", rec)
                       elif sig != RECSIG:
-                          if self.base_verbose:
+                          if self.verbose:
                               print("Detected error at %d" % rec)
                           ret += 1
                           self.__save_error(rec, vacerrfp)
                       else:
-                          global base_integrity
-                          tmpi = base_integrity
-                          base_integrity = True
+                          self.integrity = True
                           arr = self.get_rec_byoffs(rec)
-                          base_integrity = tmpi
 
                           if self.pgdebug > 1:
                               print(cnt, "vac rec", rec, arr)
 
                           if len(arr) > 1:
                               hhh2 = self.hash32(arr[0])
                               hhh3 = self.hash32(arr[1])
@@ -2183,106 +2181,106 @@
                               if self.pgdebug > 0:
                                   print("Error on vac: %d" % rec)
                       cnt += 1
 
                   vacdb.fp.close()
                   vacdb.ifp.close()
 
-                  vacdb.lock.unlock()  #dellock(vacdb.lckname)
+                  vacdb.lock.unlock()
 
                   # if vacerr is empty
                   try:
                       if os.stat(vacerr).st_size == 0:
                           #print("Vac error empty")
                           os.remove(vacerr)
                   except:
-                      if self.core_verbose > 0:
+                      if self.verbose > 0:
                           print("vacerr", sys.exc_info())
 
               # Any vacummed?
               if vac > 0:
                   # Make it go out of scope
                   self.fp.flush(); self.ifp.flush()
                   self.fp.close(); self.ifp.close()
 
                   # Now move files
                   try:
                       os.remove(self.fname);
                   except:
-                      if self.core_verbose > 0:
+                      if self.verbose > 0:
                           print("vacuum remove", self.fname, sys.exc_info())
                       pass
 
                   try:
                       os.remove(self.idxname)
                   except:
-                      if self.core_verbose > 2:
+                      if self.verbose > 2:
                           print("vacuum idx remove", self.idxname, sys.exc_info
       ())
                       pass
 
                   if self.pgdebug > 1:
                       print("rename", vacname, "->", self.fname)
                       print("rename", vacidx, "->", self.idxname)
 
                   try:
                       os.rename(vacname, self.fname)
                   except:
-                      if self.core_verbose > 2:
+                      if self.verbose > 2:
                           print("vacuum rename", vacname, sys.exc_info())
                   try:
                       os.rename(vacidx, self.idxname)
                   except:
-                      if self.core_verbose > 2:
+                      if self.verbose > 2:
                           print("vacuum idx rename", vacidx, sys.exc_info())
 
-                  self.lock.waitlock() #self.lckname)
+                  self.lock.waitlock()
                   self.fp = self.softcreate(self.fname)
                   self.ifp = self.softcreate(self.idxname)
-                  #self.lock.unlock()  #dellock(self.lckname)
+                  #self.lock.unlock()
 
               else:
                   # Just remove non vacuumed files
                   if self.pgdebug > 1:
                       print("deleted", vacname, vacidx)
                   try:
                       os.remove(vacname)
                       os.remove(vacidx)
                   except:
                       pass
 
               #self.lock.unlock()
-              #dellock(self.lckname)
+
 
               #print("ended vacuum")
               return ret, vac
 
           def  get_rec(self, recnum):
 
               ''' Get record from database; recnum is a zero based record
       counter. '''
 
               if self.pgdebug:
-                  print("getrec()", recnum)
+                  print("get_rec()", recnum)
 
               rsize = self._getdbsize(self.ifp)
               if recnum >= rsize:
-                  if self.core_verbose > 0:
+                  if self.verbose > 0:
                       print("Past end of data.");
-                  raise  RuntimeError( \
-                          "Past end of Data. Asking for %d while max is 0 .. %d
-      records." \
-                                           % (recnum, rsize-1) )
+                  errx =  "Past end of Data. (ask: %d max: %d)"  % (recnum,
+      rsize-1)
+                  raise  RuntimeError(errx)
                   return []
 
               chash = self.getidxint(CURROFFS)
               #print("chash", chash)
               offs = self.getidxint(HEADSIZE + recnum * self.INTSIZE * 2)
 
-              #print("offs", offs)
+              #sig = self.getbuffstr(offs, self.INTSIZE)
+
               return self._rec2arr(offs)
 
           def  get_rec_byoffs(self, recoffs):
 
               ''' Return record by offset. '''
 
               rsize = self.getsize(self.fp)
@@ -2292,19 +2290,18 @@
                           "Past end of File. Asking for offset %d file size is
       %d." \
                                            % (recoffs, rsize) )
                   return []
 
               sig = self.getbuffstr(recoffs, self.INTSIZE)
               if sig == RECDEL:
-                  if self.base_verbose:
+                  if self.verbose:
                       print("Deleted record.")
-                  return []
               if sig != RECSIG:
-                  if self.core_verbose > 0:
+                  if self.verbose > 0:
                       print("Unlikely offset %d is not at record boundary." %
       recoffs, sig)
                   return []
               #print("recoffs", recoffs)
               return self._rec2arr(recoffs)
 
           def  get_key_offs(self, recoffs):
@@ -2318,19 +2315,19 @@
                           "Past end of File. Asking for offset %d file size is
       %d." \
                                            % (recoffs, rsize) )
                   return []
 
               sig = self.getbuffstr(recoffs, self.INTSIZE)
               if sig == RECDEL:
-                  if self.base_verbose:
+                  if self.verbose:
                       print("Deleted record.")
                   return []
               if sig != RECSIG:
-                  if self.core_verbose > 0:
+                  if self.verbose > 0:
                       print("Unlikely offset %d is not at record boundary." %
       recoffs, sig)
                   return []
               #print("recoffs", recoffs)
               return self._rec2arr(recoffs)[0]
 
           def  del_rec(self, recnum):
@@ -2339,24 +2336,24 @@
                   Deleted record is marked as deleted but not removed.
                   Deleted records are ignored in further operations.
                   Use 'vacuum' to actually remove record.
               '''
 
               rsize = self._getdbsize(self.ifp)
               if recnum >= rsize:
-                  if self.base_verbose:
+                  if self.verbose:
                       print("Past end of data.");
                   return False
               chash = self.getidxint(CURROFFS)
               #print("chash", chash)
               offs = self.getidxint(HEADSIZE + recnum * self.INTSIZE * 2)
               #print("offs", offs)
               old = self.getbuffstr(offs, self.INTSIZE)
               if old == RECDEL:
-                  if self.base_verbose:
+                  if self.verbose:
                       print("Record at %d already deleted." % offs);
                   return False
 
               self.putbuffstr(offs, RECDEL)
               return True
 
           def  del_rec_offs(self, recoffs):
@@ -2370,15 +2367,15 @@
                           "Past end of File. Asking for offset %d file size is
       %d." \
                                            % (recoffs, rsize) )
                   return False
 
               sig = self.getbuffstr(recoffs, self.INTSIZE)
               if sig != RECSIG  and sig != RECDEL:
-                  if self.core_verbose > 0:
+                  if self.verbose > 0:
                       print("Unlikely offset %d is not at record boundary." %
       recoffs, sig)
                   return False
 
               self.putbuffstr(recoffs, RECDEL)
               return True
 
@@ -2386,30 +2383,30 @@
 
           def integrity_check(self, skip = 0, count = 0xffffffff):
 
               ''' Check record integrity for 'count' records.
                   Skip number of records.
               '''
 
-              self.lock.waitlock()    #(self.lckname)
+              self.lock.waitlock()
               ret = 0; cnt2 = 0; cnt3 = 0;
               #chash = self.getidxint(CURROFFS)        #;print("chash", chash)
               chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
               # Direction sensitivity
               rrr = range(HEADSIZE + skip * self.INTSIZE * 2, chash,
       self.INTSIZE * 2)
               for aa in rrr:
                   rec = self.getidxint(aa)
                   #print(aa, rec)
                   ret += self.check_rec(rec, cnt2)
                   cnt2 += 1
                   cnt3 += 1
                   if cnt3 >= count:
                       break
-              self.lock.unlock() #dellock(self.lckname)
+              self.lock.unlock()
               return ret, cnt2
 
           def  retrieve(self, strx, limx = 1):
 
               ''' Retrive in reverse, limit it. '''
 
               if type(strx) != type(b""):
@@ -2421,35 +2418,35 @@
 
               #chash = self.getidxint(CURROFFS)
               chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
 
               #;print("chash", chash)
               arr = []
 
-              self.lock.waitlock() #(self.lckname)
+              self.lock.waitlock()
 
               #for aa in range(HEADSIZE + self.INTSIZE * 2, chash, self.INTSIZE
       * 2):
               for aa in range(chash - self.INTSIZE * 2, HEADSIZE  -
       self.INTSIZE * 2, -self.INTSIZE * 2):
                   rec = self.getidxint(aa)
                   sig = self.getbuffstr(rec, self.INTSIZE)
                   if sig == RECDEL:
-                      if self.base_verbose > 3:
+                      if self.verbose > 3:
                           print(" Deleted record '%s' at" % sig, rec)
                   elif sig != RECSIG:
-                      if self.base_verbose:
+                      if self.verbose:
                           print(" Damaged data '%s' at" % sig, rec)
                   else:
                       hhh = self.getbuffint(rec+4)
                       if hhh == hhhh:
                           arr.append(self.get_rec_byoffs(rec))
                           if len(arr) >= limx:
                               break
-              self.lock.unlock()  #dellock(self.lckname)
+              self.lock.unlock()
 
               return arr
 
           # Return record offset
 
           def  _recoffset(self, strx, limx = INT_MAX, skipx = 0):
 
@@ -2468,38 +2465,40 @@
               #for aa in range(HEADSIZE + self.INTSIZE * 2, chash, self.INTSIZE
       * 2):
               for aa in range(chash - self.INTSIZE * 2, HEADSIZE  -
       self.INTSIZE * 2, -self.INTSIZE * 2):
                   rec = self.getidxint(aa)
                   sig = self.getbuffstr(rec, self.INTSIZE)
                   if sig == RECDEL:
-                      if base_showdel:
+                      if self.showdel:
                           print(" Deleted record '%s' at" % sig, rec)
                   elif sig != RECSIG:
-                      if self.base_verbose > 0:
+                      if self.verbose > 0:
                           print(" Damaged data '%s' at" % sig, rec)
                   else:
                       blen = self.getbuffint(rec+8)
                       keyz = self.getbuffstr(rec + 12, blen)
-                      if self.base_verbose > 1:
+                      if self.verbose > 1:
                           print("_recoffset", keyz)
                       if strx2 == keyz:
                           sig = self.getbuffstr(rec + 16 + blen,  self.INTSIZE)
                           xlen = self.getbuffint(rec + 20 + blen)
                           data = self.getbuffstr(rec + 24 + blen, xlen)
                           #print("rec offset", rec + 12,  "key:", keyz, "data:
       ", data)
                           break       # Only the last one
               return rec, rec+24 + blen, len(data)
 
           def  findrec(self, strx, limx = INT_MAX, skipx = 0):
 
-              ''' Find by string matching substring. '''
+              ''' Find key by matching strx with substring.
+              Return record(s).
+              '''
 
-              self.lock.waitlock()    #(self.lckname)
+              self.lock.waitlock()
 
               #chash = self.getidxint(CURROFFS)            #;print("chash",
       chash)
               chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
 
               arr = []
               strx2 = strx.encode(errors='strict');
@@ -2509,118 +2508,118 @@
               #for aa in range(HEADSIZE + self.INTSIZE * 2, chash, self.INTSIZE
       * 2):
               for aa in range(chash - self.INTSIZE * 2, HEADSIZE  -
       self.INTSIZE * 2, -self.INTSIZE * 2):
                   rec = self.getidxint(aa)
                   sig = self.getbuffstr(rec, self.INTSIZE)
                   if sig == RECDEL:
-                      if base_showdel:
+                      if self.showdel:
                           print(" Deleted record '%s' at" % sig, rec)
                   elif sig != RECSIG:
-                      if self.base_verbose > 0:
+                      if self.verbose > 0:
                           print(" Damaged data '%s' at" % sig, rec)
                   else:
                       blen = self.getbuffint(rec+8)
                       data = self.getbuffstr(rec + 12, blen)
-                      if self.base_verbose > 1:
+                      if self.verbose > 1:
                           print("find", data)
                       #if str(strx2) in str(data):
                       if strx2 in data:
                           arr.append(self.get_key_offs(rec))
                           #arr.append(rec)
 
                           if len(arr) >= limx:
                               break
-              self.lock.unlock()  #dellock(self.lckname)
+              self.lock.unlock()
 
               return arr
 
           def  findrecpos(self, strx, limx = INT_MAX, skipx = 0):
 
-              ''' Find record, return array of positions. '''
+              ''' Find record by key, return array of positions. '''
 
-              self.lock.waitlock()    #(self.lckname)
+              self.lock.waitlock()
               chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
               arr = []
               if type(strx) != type(b""):
                   strx = strx.encode(errors='strict');
 
               for aa in range(chash - self.INTSIZE * 2, HEADSIZE  -
       self.INTSIZE * 2, -self.INTSIZE * 2):
                   rec = self.getidxint(aa)
                   sig = self.getbuffstr(rec, self.INTSIZE)
                   if sig == RECDEL:
-                      if base_showdel:
+                      if self.showdel:
                           print(" Deleted record '%s' at" % sig, rec)
                   elif sig != RECSIG:
-                      if self.base_verbose > 0:
+                      if self.verbose > 0:
                           print(" Damaged data '%s' at" % sig, rec)
                   else:
                       blen = self.getbuffint(rec+8)
                       data = self.getbuffstr(rec + 12, blen)
-                      if self.base_verbose > 1:
+                      if self.verbose > 1:
                           print("frecpos", data)
                       if strx == data:
                           arr.append(rec)
                           if len(arr) >= limx:
                               break
 
-              self.lock.unlock()  #dellock(self.lckname)
+              self.lock.unlock()
 
               return arr
 
-          def  findrec(self, strx, limx = INT_MAX, skipx = 0):
+          def  findrecsub(self, strx, limx = INT_MAX, skipx = 0):
 
-              ''' Find by string matching substring. '''
+              ''' Find record by matching substring. '''
 
-              self.lock.waitlock()    #(self.lckname)
+              self.lock.waitlock()
               chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
               arr = []
               if type(strx) != type(b""):
                   strx2 = strx.encode(errors='strict');
 
               #print("findrec", strx2)
 
               #for aa in range(HEADSIZE + self.INTSIZE * 2, chash, self.INTSIZE
       * 2):
               for aa in range(chash - self.INTSIZE * 2, HEADSIZE  -
       self.INTSIZE * 2, -self.INTSIZE * 2):
                   rec = self.getidxint(aa)
                   sig = self.getbuffstr(rec, self.INTSIZE)
                   if sig == RECDEL:
-                      if base_showdel:
+                      if self.showdel:
                           print(" Deleted record '%s' at" % sig, rec)
                   elif sig != RECSIG:
-                      if self.base_verbose > 0:
+                      if self.verbose > 0:
                           print(" Damaged data '%s' at" % sig, rec)
                   else:
                       blen = self.getbuffint(rec+8)
                       data = self.getbuffstr(rec + 12, blen)
-                      if self.base_verbose > 1:
+                      if self.verbose > 1:
                           print("find", data)
                       #if str(strx2) in str(data):
                       if strx2 in data:
                           #arr.append(self.get_key_offs(rec))
                           #arr.append(rec)
                           arr.append(self._rec2arr(rec))
                           if len(arr) >= limx:
                               break
-              self.lock.unlock()    #dellock(self.lckname)
+              self.lock.unlock()
 
               return arr
 
           # -------------------------------------------------------------------
       -
           # List all active records
 
           def  listall(self):
 
               ''' List all active records. Return array id record indexes. '''
 
-              self.lock.waitlock()    #(self.lckname)
+              self.lock.waitlock()
               keys = []; arr = []; cnt = 0
 
               chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
               maxrec = chash - self.INTSIZE * 2
               rsize = self._getdbsize(self.ifp) - 1
 
               rrr =  range(maxrec,
@@ -2628,40 +2627,42 @@
               for aa in rrr:
                   rec = self.getidxint(aa)
 
                   #print(" Scanning at %d %d" % (rec, cnt))
 
                   sig = self.getbuffstr(rec, self.INTSIZE)
                   if sig == RECDEL:
-                      if 1: #base_showdel:
+                      if 1: #self.showdel:
                           print("Deleted record '%s' at" % sig, rec)
                   elif sig != RECSIG:
-                      if 1: #self.base_verbose > 0:
+                      if 1: #self.verbose > 0:
                           print(" Damaged data '%s' at" % sig, rec)
                   else:
                           hhh = self.getbuffint(rec+4)
                           print(" Good data '%s' at" % sig, rec, hhh)
                           if hhh not in keys:
                               keys.append(hhh)
                               # as we are going backwards
                               arr.append(rsize - cnt)
                               #print("found", hhh)
                   cnt += 1
 
               keys = []
-              self.lock.unlock()  #dellock()self.lckname)
+              self.lock.unlock()
 
               return arr
 
           def  find_key(self, keyx, limx = 0xffffffff):
 
-              ''' Find record by key Search from the end, so latest comes
-      first. '''
+              ''' Find record by key value.
+                  Search from the end, so latest comes first.
+                  This operates on the hash, so it reaches the answer fast.
+              '''
 
-              self.lock.waitlock()   #self.lckname)
+              self.lock.waitlock()
 
               skip = 0; arr = []; cnt = 0
               try:
                   arg2e = keyx.encode()
               except:
                   arg2e = keyx
 
@@ -2673,32 +2674,32 @@
                       HEADSIZE - self.INTSIZE * 2, -self.INTSIZE * 2)
               for aa in rrr:
                   rec = self.getidxint(aa)
                   #print(" Scanning at %d %d" % (rec, cnt))
 
                   sig = self.getbuffstr(rec, self.INTSIZE)
                   if sig == RECDEL:
-                      if base_showdel:
+                      if self.showdel:
                           print("Deleted record '%s' at" % sig, rec)
                   elif sig != RECSIG:
-                      if self.base_verbose > 0:
+                      if self.verbose > 0:
                           print(" Damaged data '%s' at" % sig, rec)
                   else:
                       hhh = self.getbuffint(rec+4)
                       if hhh == hhhh:
                           if len(arr) >= limx - 1:
                               arr.append(["More data ...",])
                               break
                           arr.append(rec)
                       else:
                           pass
                           #print("no match", hex(hhh))
 
                   cnt += 1
-              self.lock.unlock()  #dellock()self.lckname)
+              self.lock.unlock()
 
               return arr
 
 
           def  del_data(self, hash, skip = 1):
 
               ''' Delete data by hash. '''
@@ -2719,15 +2720,15 @@
                   #    print(" Damaged data '%s' at" % sig, rec)
 
                   #blen = self.getbuffint(rec+8)
                   #print("data '%s' at" % sig, rec, "blen", blen)
 
                   hhh = self.getbuffint(rec+4)
                   if hash == hhh:
-                      if self.base_verbose > 0:
+                      if self.verbose > 0:
                           print("Would delete", hhh)
 
                   self.putbuffstr(rec, RECDEL)
 
                   cnt += 1
 
               return arr
@@ -2755,15 +2756,15 @@
               ''' Delete records by key string; needs bin str, converted
                   automatically on entry.
               '''
 
               if type(strx) != type(b""):
                   strx = strx.encode()
 
-              if self.base_verbose > 1:
+              if self.verbose > 1:
                   print("Start delete ", strx, "skip", skip)
 
               cnt = 0; cnt3 = 0
               #chash = self.getidxint(CURROFFS)    #;print("chash", chash)
               chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
 
               # Direction sensitivity
@@ -2775,62 +2776,63 @@
       self.INTSIZE * 2, -self.INTSIZE * 2)
 
               #for aa in range(HEADSIZE, chash, self.INTSIZE * 2):
               for aa in rrr:
                   rec = self.getidxint(aa)
                   sig = self.getbuffstr(rec, self.INTSIZE)
                   if sig == RECDEL:
-                      if base_showdel:
+                      if self.showdel:
                           print(" Deleted record '%s' at" % sig, rec)
                   elif sig != RECSIG:
-                      if self.base_verbose > 0:
+                      if self.verbose > 0:
                           print(" Damaged data '%s' at" % sig, rec)
                   else:
                       blen = self.getbuffint(rec+8)
                       data = self.getbuffstr(rec + 12, blen)
-                      if self.base_verbose > 2:
+                      if self.verbose > 2:
                           print("del iterate recs", cnt3, data, strx)
 
                       if strx == data:
-                          if self.base_verbose > 0:
+                          if self.verbose > 0:
                               print("Deleting", cnt3, aa, data)
                           self.putbuffstr(rec, RECDEL)
                           cnt += 1
                           if cnt >= maxdelrec:
                               break
                   cnt3 += 1
               return cnt
 
           def  save_data(self, header, datax, replace = False):
 
               ''' Append to the end of file. If replace flag is set, try to
       overwrite
-                  in place. If new record is larger, add it as ususal. If
+                  in place. If new record is larger, add it as usual. If
       smaller,
                   the record is padded with spaces. This should not influence
       most ops.
                   (like: int())
                   This feature allows the database update wthout creating new
       records.
-                  Useful for counters or dynamically changing data.
+                  Useful for counters or dynamically changing data. To be
+      useful,
+                  use  create fixed size data. Like sprintf(%12d).
 
                           Input:
                               header     Header
                               datax      Data
 
                            Return:
                               The offset of saved data
                   '''
 
               if self.pgdebug > 0:
                   print("Save_data()", header, datax)
 
-              self.lock.waitlock()   #self.lckname)
-              ret = 0
-              was = False
+              self.lock.waitlock()
+              ret = 0 ; was = False
               # Put new data in place
               if replace:
                   if type(datax) != type(b""):
                       mrep2 = datax.encode()
                   else:
                       mrep2 = datax
 
@@ -2845,17 +2847,18 @@
                           ccc = self.hash32(padded)
                           self.putbuffint(rrr[1] - 8, ccc)
                           #print("ccc", hex(ccc))
                           self.putbuffstr(rrr[1], padded)
                           was = True
                           ret =  rrr[0]
               if not was:
+                  #print("Saving longer data", header, datax)
                   ret = self._save_data2(header, datax)
 
-              self.lock.unlock()  #dellock()self.lckname)
+              self.lock.unlock()
 
               return ret
 
           # -------------------------------------------------------------------
       -
           # Save data to database file
 
@@ -2922,15 +2925,15 @@
               self.putidxint(curr, dcurr)
               self.putidxint(curr + self.INTSIZE, hhh2)
               #self.putidxint(CURROFFS, self.ifp.tell())
 
               self.fp.flush()
               self.ifp.flush()
 
-              return curr
+              return dcurr
 
           def __del__(self):
 
               ''' flush file handles and close files. '''
 
               if hasattr(self, "pgdebug"):
                   if self.pgdebug > 9:
@@ -2945,14 +2948,18 @@
                               self.fp.close()
 
               if hasattr(self, "ifp"):
                       if self.ifp:
                           if not self.ifp.closed:
                               self.ifp.flush()
                               self.ifp.close()
+
+              # remove lockfile
+              if hasattr(self, "lock"):
+                  self.lock.unlock()
       ******** AAnncceessttoorrss ********
           * twinbase.TwinCoreBase
       ******** MMeetthhooddss ********
         def check_rec(self, rec, cnt2)
             Check record. Verbose to the screen. Return number of errors.
             Expand source code
             def  check_rec(self, rec, cnt2):
@@ -2961,77 +2968,77 @@
             errors.'''
 
                 ret = 0
                 sig = self.getbuffstr(rec, self.INTSIZE)
 
                 # Do not check deleted, say OK
                 if sig == RECDEL:
-                    if self.base_verbose > 1:
+                    if self.verbose > 1:
                         print(" Deleted data '%s' at %d (%d)" % (sig, rec,
             cnt2))
                     ret = 1
                     return ret
 
                 if sig != RECSIG:
-                    if self.base_verbose > 0:
+                    if self.verbose > 0:
                         print(" Damaged data (sig) '%s' at %d (%d)" % (sig,
             rec, cnt2))
-                    #if self.base_verbose > 1:
+                    #if self.verbose > 1:
                     #    print("Data", data)
 
                     return ret
 
                 hash = self.getbuffint(rec+4)
                 blen = self.getbuffint(rec+8)
 
                 if blen <= 0:
-                    if self.base_verbose > 1:
+                    if self.verbose > 1:
                         print("Invalid key length %d at %d" % (blen, rec))
                     return ret
 
                 data = self.getbuffstr(rec+12, blen)
                 ccc = self.hash32(data)
                 if hash != ccc:
-                    if self.base_verbose > 1:
+                    if self.verbose > 1:
                         print("Data", data)
-                    elif self.base_verbose > 0:
+                    elif self.verbose > 0:
                         print("Error on hash at rec", rec, cnt2, "hash",
                                                     hex(hash), "check", hex
             (ccc))
 
                     return ret
 
                 endd = self.getbuffstr(rec + 12 + blen, self.INTSIZE)
                 if endd != RECSEP:
-                    if self.base_verbose > 0:
+                    if self.verbose > 0:
                         print(" Damaged data (sep) '%s' at %d %d %d" % (endd,
             rec, cnt2))
                     return ret
 
                 rec2 = rec + 16 + blen;
                 hash2 = self.getbuffint(rec2)
                 blen2 = self.getbuffint(rec2+4)
 
                 if blen2 < 0:
-                    if self.base_verbose > 1:
+                    if self.verbose > 1:
                         print("Invalid data length2 %d at %d" % (blen2, rec))
                     return ret
 
                 data2 = self.getbuffstr(rec2+8, blen2)
                 ccc2 = self.hash32(data2)
                 if hash2 != ccc2:
-                    if self.base_verbose > 1:
+                    if self.verbose > 1:
                         print("Data", data, "Data2", data2)
-                    elif self.base_verbose > 0:
+                    elif self.verbose > 0:
                         print("Error on hash2 at rec", rec, cnt2, "hash2",
                                                 hex(hash2), "check2", hex
             (ccc2))
                     return ret
 
-                if self.base_verbose > 2:
+                if self.verbose > 2:
                     print("Record at %d (%d) OK." % (rec, cnt2))
 
                 ret += 1
                 return ret
         def del_data(self, hash, skip=1)
             Delete data by hash.
             Expand source code
@@ -3055,15 +3062,15 @@
                     #    print(" Damaged data '%s' at" % sig, rec)
 
                     #blen = self.getbuffint(rec+8)
                     #print("data '%s' at" % sig, rec, "blen", blen)
 
                     hhh = self.getbuffint(rec+4)
                     if hash == hhh:
-                        if self.base_verbose > 0:
+                        if self.verbose > 0:
                             print("Would delete", hhh)
 
                     self.putbuffstr(rec, RECDEL)
 
                     cnt += 1
 
                 return arr
@@ -3078,24 +3085,24 @@
                     Deleted record is marked as deleted but not removed.
                     Deleted records are ignored in further operations.
                     Use 'vacuum' to actually remove record.
                 '''
 
                 rsize = self._getdbsize(self.ifp)
                 if recnum >= rsize:
-                    if self.base_verbose:
+                    if self.verbose:
                         print("Past end of data.");
                     return False
                 chash = self.getidxint(CURROFFS)
                 #print("chash", chash)
                 offs = self.getidxint(HEADSIZE + recnum * self.INTSIZE * 2)
                 #print("offs", offs)
                 old = self.getbuffstr(offs, self.INTSIZE)
                 if old == RECDEL:
-                    if self.base_verbose:
+                    if self.verbose:
                         print("Record at %d already deleted." % offs);
                     return False
 
                 self.putbuffstr(offs, RECDEL)
                 return True
         def del_rec_bykey(self, strx, maxdelrec=4294967295, skip=0, dirx=0)
             Remove record by key. Remove maxdelrec occurances.
@@ -3129,15 +3136,15 @@
                 ''' Delete records by key string; needs bin str, converted
                     automatically on entry.
                 '''
 
                 if type(strx) != type(b""):
                     strx = strx.encode()
 
-                if self.base_verbose > 1:
+                if self.verbose > 1:
                     print("Start delete ", strx, "skip", skip)
 
                 cnt = 0; cnt3 = 0
                 #chash = self.getidxint(CURROFFS)    #;print("chash", chash)
                 chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE *
             2
 
@@ -3150,27 +3157,27 @@
             self.INTSIZE * 2, -self.INTSIZE * 2)
 
                 #for aa in range(HEADSIZE, chash, self.INTSIZE * 2):
                 for aa in rrr:
                     rec = self.getidxint(aa)
                     sig = self.getbuffstr(rec, self.INTSIZE)
                     if sig == RECDEL:
-                        if base_showdel:
+                        if self.showdel:
                             print(" Deleted record '%s' at" % sig, rec)
                     elif sig != RECSIG:
-                        if self.base_verbose > 0:
+                        if self.verbose > 0:
                             print(" Damaged data '%s' at" % sig, rec)
                     else:
                         blen = self.getbuffint(rec+8)
                         data = self.getbuffstr(rec + 12, blen)
-                        if self.base_verbose > 2:
+                        if self.verbose > 2:
                             print("del iterate recs", cnt3, data, strx)
 
                         if strx == data:
-                            if self.base_verbose > 0:
+                            if self.verbose > 0:
                                 print("Deleting", cnt3, aa, data)
                             self.putbuffstr(rec, RECDEL)
                             cnt += 1
                             if cnt >= maxdelrec:
                                 break
                     cnt3 += 1
                 return cnt
@@ -3188,15 +3195,15 @@
                             "Past end of File. Asking for offset %d file size
             is %d." \
                                              % (recoffs, rsize) )
                     return False
 
                 sig = self.getbuffstr(recoffs, self.INTSIZE)
                 if sig != RECSIG  and sig != RECDEL:
-                    if self.core_verbose > 0:
+                    if self.verbose > 0:
                         print("Unlikely offset %d is not at record boundary." %
             recoffs, sig)
                     return False
 
                 self.putbuffstr(recoffs, RECDEL)
                 return True
         def dump_data(self, lim=4294967295, skip=0)
@@ -3219,115 +3226,118 @@
 
                 cnt2 = 0
                 sig = self.getbuffstr(rec, self.INTSIZE)
                 if self.pgdebug > 5:
                     print("Sig ", sig, "at", rec)
 
                 if sig == RECDEL:
-                    if base_showdel:
+                    if self.showdel:
                         klen = self.getbuffint(rec+8)
                         kdata = self.getbuffstr(rec+12, klen)
                         rec2 = rec + 16 + klen;
                         blen = self.getbuffint(rec2+4)
                         data = self.getbuffstr(rec2+8, blen)
                         print(" Del at", rec, "key:", kdata, "data:", truncs
             (data))
-                    if self.base_verbose > 1:
+                    if self.verbose > 1:
                         klen = self.getbuffint(rec+8)
                         kdata = self.getbuffstr(rec+12, klen)
                         rec2 = rec + 16 + klen;
                         blen = self.getbuffint(rec2+4)
                         data = self.getbuffstr(rec2+8, blen)
-                        if self.base_verbose > 2:
+                        if self.verbose > 2:
                             print(" Del at", rec, "key:", kdata, "data:", data)
                         else:
                             print(" Del at", rec, "key:", kdata, "data:",
             truncs(data))
 
                     return cnt2
 
                 if sig != RECSIG:
-                    if self.base_verbose > 1:
+                    if self.verbose > 1:
                         print(" Damaged data (sig) '%s' at" % sig, rec)
                     return cnt2
 
                 hash = self.getbuffint(rec+4)
                 blen = self.getbuffint(rec+8)
 
                 if blen < 0:
-                    if self.base_verbose > 2:
+                    if self.verbose > 2:
                         print("Invalid key length %d at %d" % (blen, rec))
                     return cnt2
 
                 data = self.getbuffstr(rec+12, blen)
-                if base_integrity:
+                if self.integrity:
                     ccc = self.hash32(data)
-                    if self.base_verbose > 1:
+                    if self.verbose > 1:
                         print("rec", rec, "hash", hex(hash), "check", hex(ccc))
                     if hash != ccc:
-                        if self.base_verbose > 0:
+                        if self.verbose > 0:
                             print("Error on hash at rec", rec, "hash", hex
             (hash), "check", hex(ccc))
                         return []
 
                 endd = self.getbuffstr(rec + 12 + blen, self.INTSIZE)
                 if endd != RECSEP:
-                    if self.base_verbose > 0:
+                    if self.verbose > 0:
                         print(" Damaged data (sep) '%s' at" % endd, rec)
                     return cnt2
 
                 rec2 = rec + 16 + blen;
                 hash2 = self.getbuffint(rec2)
                 blen2 = self.getbuffint(rec2+4)
 
                 if blen2 < 0:
-                    if self.base_verbose > 1:
+                    if self.verbose > 1:
                         print("Invalid data length %d at %d" % (blen2, rec))
                     return cnt2
 
                 data2 = self.getbuffstr(rec2+8, blen2)
-                if base_integrity:
+                if self.integrity:
                     ccc2 = self.hash32(data2)
-                    if self.base_verbose > 1:
+                    if self.verbose > 1:
                         print("rec", rec, "hash2", hex(hash), "check2", hex
             (ccc))
                     if hash2 != ccc2:
-                        if self.base_verbose > 0:
+                        if self.verbose > 0:
                             print("Error on hash at rec", rec, "hash2", hex
             (hash), "check2", hex(ccc))
                         return []
 
-                if self.base_verbose > 2:
+                if self.verbose > 2:
                     print("%-5d pos %5d" % (cnt, rec), "%8x" % hash, "len",
             blen, data,
                                                                 "%8x" %
             hash2,"len", blen2, data2)
 
-                elif self.base_verbose > 1:
+                elif self.verbose > 1:
                     print("%-5d pos %5d" % (cnt, rec), "%8x" % hash, "len",
             blen, data,
                                                                 "%8x" %
             hash2,"len", blen2, data2)
-                elif self.base_verbose:
+                elif self.verbose:
                     print("%-5d pos %5d" % (cnt, rec),  data, data2)
                 else:
                     print("%-5d pos %5d" % (cnt, rec), "Data:", truncs(data,
             18), "Data2:", truncs(data2, 18))
 
                 cnt2 += 1
                 return cnt2
         def find_key(self, keyx, limx=4294967295)
-            Find record by key Search from the end, so latest comes first.
+            Find record by key value. Search from the end, so latest comes
+            first. This operates on the hash, so it reaches the answer fast.
             Expand source code
             def  find_key(self, keyx, limx = 0xffffffff):
 
-                ''' Find record by key Search from the end, so latest comes
-            first. '''
+                ''' Find record by key value.
+                    Search from the end, so latest comes first.
+                    This operates on the hash, so it reaches the answer fast.
+                '''
 
-                self.lock.waitlock()   #self.lckname)
+                self.lock.waitlock()
 
                 skip = 0; arr = []; cnt = 0
                 try:
                     arg2e = keyx.encode()
                 except:
                     arg2e = keyx
 
@@ -3340,112 +3350,160 @@
                         HEADSIZE - self.INTSIZE * 2, -self.INTSIZE * 2)
                 for aa in rrr:
                     rec = self.getidxint(aa)
                     #print(" Scanning at %d %d" % (rec, cnt))
 
                     sig = self.getbuffstr(rec, self.INTSIZE)
                     if sig == RECDEL:
-                        if base_showdel:
+                        if self.showdel:
                             print("Deleted record '%s' at" % sig, rec)
                     elif sig != RECSIG:
-                        if self.base_verbose > 0:
+                        if self.verbose > 0:
                             print(" Damaged data '%s' at" % sig, rec)
                     else:
                         hhh = self.getbuffint(rec+4)
                         if hhh == hhhh:
                             if len(arr) >= limx - 1:
                                 arr.append(["More data ...",])
                                 break
                             arr.append(rec)
                         else:
                             pass
                             #print("no match", hex(hhh))
 
                     cnt += 1
-                self.lock.unlock()  #dellock()self.lckname)
+                self.lock.unlock()
 
                 return arr
         def findrec(self, strx, limx=4294967295, skipx=0)
-            Find by string matching substring.
+            Find key by matching strx with substring. Return record(s).
             Expand source code
             def  findrec(self, strx, limx = INT_MAX, skipx = 0):
 
-                ''' Find by string matching substring. '''
+                ''' Find key by matching strx with substring.
+                Return record(s).
+                '''
+
+                self.lock.waitlock()
 
-                self.lock.waitlock()    #(self.lckname)
+                #chash = self.getidxint(CURROFFS)            #;print("chash",
+            chash)
                 chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE *
             2
+
                 arr = []
-                if type(strx) != type(b""):
-                    strx2 = strx.encode(errors='strict');
+                strx2 = strx.encode(errors='strict');
 
                 #print("findrec", strx2)
 
                 #for aa in range(HEADSIZE + self.INTSIZE * 2, chash,
             self.INTSIZE * 2):
                 for aa in range(chash - self.INTSIZE * 2, HEADSIZE  -
             self.INTSIZE * 2, -self.INTSIZE * 2):
                     rec = self.getidxint(aa)
                     sig = self.getbuffstr(rec, self.INTSIZE)
                     if sig == RECDEL:
-                        if base_showdel:
+                        if self.showdel:
                             print(" Deleted record '%s' at" % sig, rec)
                     elif sig != RECSIG:
-                        if self.base_verbose > 0:
+                        if self.verbose > 0:
                             print(" Damaged data '%s' at" % sig, rec)
                     else:
                         blen = self.getbuffint(rec+8)
                         data = self.getbuffstr(rec + 12, blen)
-                        if self.base_verbose > 1:
+                        if self.verbose > 1:
                             print("find", data)
                         #if str(strx2) in str(data):
                         if strx2 in data:
-                            #arr.append(self.get_key_offs(rec))
+                            arr.append(self.get_key_offs(rec))
                             #arr.append(rec)
-                            arr.append(self._rec2arr(rec))
+
                             if len(arr) >= limx:
                                 break
-                self.lock.unlock()    #dellock(self.lckname)
+                self.lock.unlock()
 
                 return arr
         def findrecpos(self, strx, limx=4294967295, skipx=0)
-            Find record, return array of positions.
+            Find record by key, return array of positions.
             Expand source code
             def  findrecpos(self, strx, limx = INT_MAX, skipx = 0):
 
-                ''' Find record, return array of positions. '''
+                ''' Find record by key, return array of positions. '''
 
-                self.lock.waitlock()    #(self.lckname)
+                self.lock.waitlock()
                 chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE *
             2
                 arr = []
                 if type(strx) != type(b""):
                     strx = strx.encode(errors='strict');
 
                 for aa in range(chash - self.INTSIZE * 2, HEADSIZE  -
             self.INTSIZE * 2, -self.INTSIZE * 2):
                     rec = self.getidxint(aa)
                     sig = self.getbuffstr(rec, self.INTSIZE)
                     if sig == RECDEL:
-                        if base_showdel:
+                        if self.showdel:
                             print(" Deleted record '%s' at" % sig, rec)
                     elif sig != RECSIG:
-                        if self.base_verbose > 0:
+                        if self.verbose > 0:
                             print(" Damaged data '%s' at" % sig, rec)
                     else:
                         blen = self.getbuffint(rec+8)
                         data = self.getbuffstr(rec + 12, blen)
-                        if self.base_verbose > 1:
+                        if self.verbose > 1:
                             print("frecpos", data)
                         if strx == data:
                             arr.append(rec)
                             if len(arr) >= limx:
                                 break
 
-                self.lock.unlock()  #dellock(self.lckname)
+                self.lock.unlock()
+
+                return arr
+        def findrecsub(self, strx, limx=4294967295, skipx=0)
+            Find record by matching substring.
+            Expand source code
+            def  findrecsub(self, strx, limx = INT_MAX, skipx = 0):
+
+                ''' Find record by matching substring. '''
+
+                self.lock.waitlock()
+                chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE *
+            2
+                arr = []
+                if type(strx) != type(b""):
+                    strx2 = strx.encode(errors='strict');
+
+                #print("findrec", strx2)
+
+                #for aa in range(HEADSIZE + self.INTSIZE * 2, chash,
+            self.INTSIZE * 2):
+                for aa in range(chash - self.INTSIZE * 2, HEADSIZE  -
+            self.INTSIZE * 2, -self.INTSIZE * 2):
+                    rec = self.getidxint(aa)
+                    sig = self.getbuffstr(rec, self.INTSIZE)
+                    if sig == RECDEL:
+                        if self.showdel:
+                            print(" Deleted record '%s' at" % sig, rec)
+                    elif sig != RECSIG:
+                        if self.verbose > 0:
+                            print(" Damaged data '%s' at" % sig, rec)
+                    else:
+                        blen = self.getbuffint(rec+8)
+                        data = self.getbuffstr(rec + 12, blen)
+                        if self.verbose > 1:
+                            print("find", data)
+                        #if str(strx2) in str(data):
+                        if strx2 in data:
+                            #arr.append(self.get_key_offs(rec))
+                            #arr.append(rec)
+                            arr.append(self._rec2arr(rec))
+                            if len(arr) >= limx:
+                                break
+                self.lock.unlock()
 
                 return arr
         def flush(self)
             Flush files to disk.
             Expand source code
             def flush(self):
 
@@ -3477,50 +3535,50 @@
                             "Past end of File. Asking for offset %d file size
             is %d." \
                                              % (recoffs, rsize) )
                     return []
 
                 sig = self.getbuffstr(recoffs, self.INTSIZE)
                 if sig == RECDEL:
-                    if self.base_verbose:
+                    if self.verbose:
                         print("Deleted record.")
                     return []
                 if sig != RECSIG:
-                    if self.core_verbose > 0:
+                    if self.verbose > 0:
                         print("Unlikely offset %d is not at record boundary." %
             recoffs, sig)
                     return []
                 #print("recoffs", recoffs)
                 return self._rec2arr(recoffs)[0]
         def get_rec(self, recnum)
             Get record from database; recnum is a zero based record counter.
             Expand source code
             def  get_rec(self, recnum):
 
                 ''' Get record from database; recnum is a zero based record
             counter. '''
 
                 if self.pgdebug:
-                    print("getrec()", recnum)
+                    print("get_rec()", recnum)
 
                 rsize = self._getdbsize(self.ifp)
                 if recnum >= rsize:
-                    if self.core_verbose > 0:
+                    if self.verbose > 0:
                         print("Past end of data.");
-                    raise  RuntimeError( \
-                            "Past end of Data. Asking for %d while max is 0 ..
-            %d records." \
-                                             % (recnum, rsize-1) )
+                    errx =  "Past end of Data. (ask: %d max: %d)"  % (recnum,
+            rsize-1)
+                    raise  RuntimeError(errx)
                     return []
 
                 chash = self.getidxint(CURROFFS)
                 #print("chash", chash)
                 offs = self.getidxint(HEADSIZE + recnum * self.INTSIZE * 2)
 
-                #print("offs", offs)
+                #sig = self.getbuffstr(offs, self.INTSIZE)
+
                 return self._rec2arr(offs)
         def get_rec_byoffs(self, recoffs)
             Return record by offset.
             Expand source code
             def  get_rec_byoffs(self, recoffs):
 
                 ''' Return record by offset. '''
@@ -3532,19 +3590,18 @@
                             "Past end of File. Asking for offset %d file size
             is %d." \
                                              % (recoffs, rsize) )
                     return []
 
                 sig = self.getbuffstr(recoffs, self.INTSIZE)
                 if sig == RECDEL:
-                    if self.base_verbose:
+                    if self.verbose:
                         print("Deleted record.")
-                    return []
                 if sig != RECSIG:
-                    if self.core_verbose > 0:
+                    if self.verbose > 0:
                         print("Unlikely offset %d is not at record boundary." %
             recoffs, sig)
                     return []
                 #print("recoffs", recoffs)
                 return self._rec2arr(recoffs)
         def getdbsize(self)
             Return the DB size in records. This includes ALL records, including
@@ -3568,15 +3625,15 @@
             Expand source code
             def integrity_check(self, skip = 0, count = 0xffffffff):
 
                 ''' Check record integrity for 'count' records.
                     Skip number of records.
                 '''
 
-                self.lock.waitlock()    #(self.lckname)
+                self.lock.waitlock()
                 ret = 0; cnt2 = 0; cnt3 = 0;
                 #chash = self.getidxint(CURROFFS)        #;print("chash",
             chash)
                 chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE *
             2
                 # Direction sensitivity
                 rrr = range(HEADSIZE + skip * self.INTSIZE * 2, chash,
@@ -3585,25 +3642,25 @@
                     rec = self.getidxint(aa)
                     #print(aa, rec)
                     ret += self.check_rec(rec, cnt2)
                     cnt2 += 1
                     cnt3 += 1
                     if cnt3 >= count:
                         break
-                self.lock.unlock() #dellock(self.lckname)
+                self.lock.unlock()
                 return ret, cnt2
         def listall(self)
             List all active records. Return array id record indexes.
             Expand source code
             def  listall(self):
 
                 ''' List all active records. Return array id record indexes.
             '''
 
-                self.lock.waitlock()    #(self.lckname)
+                self.lock.waitlock()
                 keys = []; arr = []; cnt = 0
 
                 chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE *
             2
                 maxrec = chash - self.INTSIZE * 2
                 rsize = self._getdbsize(self.ifp) - 1
 
@@ -3612,43 +3669,43 @@
                 for aa in rrr:
                     rec = self.getidxint(aa)
 
                     #print(" Scanning at %d %d" % (rec, cnt))
 
                     sig = self.getbuffstr(rec, self.INTSIZE)
                     if sig == RECDEL:
-                        if 1: #base_showdel:
+                        if 1: #self.showdel:
                             print("Deleted record '%s' at" % sig, rec)
                     elif sig != RECSIG:
-                        if 1: #self.base_verbose > 0:
+                        if 1: #self.verbose > 0:
                             print(" Damaged data '%s' at" % sig, rec)
                     else:
                             hhh = self.getbuffint(rec+4)
                             print(" Good data '%s' at" % sig, rec, hhh)
                             if hhh not in keys:
                                 keys.append(hhh)
                                 # as we are going backwards
                                 arr.append(rsize - cnt)
                                 #print("found", hhh)
                     cnt += 1
 
                 keys = []
-                self.lock.unlock()  #dellock()self.lckname)
+                self.lock.unlock()
 
                 return arr
         def reindex(self)
             Re create index file.
             Expand source code
             def  reindex(self):
 
                 ''' Re create index file. '''
 
-                self.lock.waitlock() #self.lckname)
+                self.lock.waitlock()
                 ret = self.__reindex()
-                self.lock.unlock()    #dellock(self.lckname)
+                self.lock.unlock()
                 return ret
         def retrieve(self, strx, limx=1)
             Retrive in reverse, limit it.
             Expand source code
             def  retrieve(self, strx, limx = 1):
 
                 ''' Retrive in reverse, limit it. '''
@@ -3663,86 +3720,87 @@
                 #chash = self.getidxint(CURROFFS)
                 chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE *
             2
 
                 #;print("chash", chash)
                 arr = []
 
-                self.lock.waitlock() #(self.lckname)
+                self.lock.waitlock()
 
                 #for aa in range(HEADSIZE + self.INTSIZE * 2, chash,
             self.INTSIZE * 2):
                 for aa in range(chash - self.INTSIZE * 2, HEADSIZE  -
             self.INTSIZE * 2, -self.INTSIZE * 2):
                     rec = self.getidxint(aa)
                     sig = self.getbuffstr(rec, self.INTSIZE)
                     if sig == RECDEL:
-                        if self.base_verbose > 3:
+                        if self.verbose > 3:
                             print(" Deleted record '%s' at" % sig, rec)
                     elif sig != RECSIG:
-                        if self.base_verbose:
+                        if self.verbose:
                             print(" Damaged data '%s' at" % sig, rec)
                     else:
                         hhh = self.getbuffint(rec+4)
                         if hhh == hhhh:
                             arr.append(self.get_rec_byoffs(rec))
                             if len(arr) >= limx:
                                 break
-                self.lock.unlock()  #dellock(self.lckname)
+                self.lock.unlock()
 
                 return arr
         def revdump_data(self, lim, skip=0)
             Put all data to screen in reverse order.
             Expand source code
             def  revdump_data(self, lim, skip = 0):
 
                 ''' Put all data to screen in reverse order. '''
 
                 self.__dump_data(lim, skip)
         def save_data(self, header, datax, replace=False)
             Append to the end of file. If replace flag is set, try to overwrite
-            in place. If new record is larger, add it as ususal. If smaller,
-            the record is padded with spaces. This should not influence most
-            ops. (like: int()) This feature allows the database update wthout
+            in place. If new record is larger, add it as usual. If smaller, the
+            record is padded with spaces. This should not influence most ops.
+            (like: int()) This feature allows the database update wthout
             creating new records. Useful for counters or dynamically changing
-            data.
+            data. To be useful, use create fixed size data. Like sprintf(%12d).
                 Input:
                     header     Header
                     datax      Data
 
                  Return:
                     The offset of saved data
             Expand source code
             def  save_data(self, header, datax, replace = False):
 
                 ''' Append to the end of file. If replace flag is set, try to
             overwrite
-                    in place. If new record is larger, add it as ususal. If
+                    in place. If new record is larger, add it as usual. If
             smaller,
                     the record is padded with spaces. This should not influence
             most ops.
                     (like: int())
                     This feature allows the database update wthout creating new
             records.
-                    Useful for counters or dynamically changing data.
+                    Useful for counters or dynamically changing data. To be
+            useful,
+                    use  create fixed size data. Like sprintf(%12d).
 
                             Input:
                                 header     Header
                                 datax      Data
 
                              Return:
                                 The offset of saved data
                     '''
 
                 if self.pgdebug > 0:
                     print("Save_data()", header, datax)
 
-                self.lock.waitlock()   #self.lckname)
-                ret = 0
-                was = False
+                self.lock.waitlock()
+                ret = 0 ; was = False
                 # Put new data in place
                 if replace:
                     if type(datax) != type(b""):
                         mrep2 = datax.encode()
                     else:
                         mrep2 = datax
 
@@ -3757,17 +3815,18 @@
                             ccc = self.hash32(padded)
                             self.putbuffint(rrr[1] - 8, ccc)
                             #print("ccc", hex(ccc))
                             self.putbuffstr(rrr[1], padded)
                             was = True
                             ret =  rrr[0]
                 if not was:
+                    #print("Saving longer data", header, datax)
                     ret = self._save_data2(header, datax)
 
-                self.lock.unlock()  #dellock()self.lckname)
+                self.lock.unlock()
 
                 return ret
         def vacuum(self)
             Remove all deleted data. Reindex. The db is locked while the vacuum
             is in operation, but make sure the DB in not in session, and no
             pending operations are present (like find / retrieve cycle).
             Expand source code
@@ -3776,44 +3835,38 @@
                 '''
                     Remove all deleted data. Reindex.
                     The db is locked while the vacuum is in operation, but
                     make sure the DB in not in session, and no pending
                     operations are present (like find / retrieve cycle).
                 '''
 
-                self.lock.waitlock() #self.lckname)
+                self.lock.waitlock()
                 ret = self._vacuum()
-                self.lock.unlock()  #dellock(self.lckname)
+                self.lock.unlock()
                 return ret
-        def version(self)
-            Return version sting.
-            Expand source code
-            def version(self):
-                ''' Return version sting. '''
-                return Version
 ************ IInnddeexx ************
     * ******** _CC_ll_aa_ss_ss_ee_ss ********
           o ****** _TT_ww_ii_nn_CC_oo_rr_ee ******
                 # _c_h_e_c_k___r_e_c
                 # _d_e_l___d_a_t_a
                 # _d_e_l___r_e_c
                 # _d_e_l___r_e_c___b_y_k_e_y
                 # _d_e_l___r_e_c___o_f_f_s
                 # _d_u_m_p___d_a_t_a
                 # _d_u_m_p___r_e_c
                 # _f_i_n_d___k_e_y
                 # _f_i_n_d_r_e_c
                 # _f_i_n_d_r_e_c_p_o_s
+                # _f_i_n_d_r_e_c_s_u_b
                 # _f_l_u_s_h
                 # _g_e_t___k_e_y___o_f_f_s
                 # _g_e_t___r_e_c
                 # _g_e_t___r_e_c___b_y_o_f_f_s
                 # _g_e_t_d_b_s_i_z_e
                 # _i_n_t_e_g_r_i_t_y___c_h_e_c_k
                 # _l_i_s_t_a_l_l
                 # _r_e_i_n_d_e_x
                 # _r_e_t_r_i_e_v_e
                 # _r_e_v_d_u_m_p___d_a_t_a
                 # _s_a_v_e___d_a_t_a
                 # _v_a_c_u_u_m
-                # _v_e_r_s_i_o_n
 Generated by_p_d_o_c_0_._1_0_._0.
```

### Comparing `pydbase-1.5.2/pydbase/portalocker.py` & `pydbase-1.7.1/pydbase/portalocker.py`

 * *Files identical despite different names*

### Comparing `pydbase-1.5.2/pydbase/twinbase.py` & `pydbase-1.7.1/pydbase/twinbase.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 
 '''!
     twinbase -- extracted from twincore to make it eazier to read
 '''
 
 import  os, sys, getopt, signal, select, socket, time, struct
-import  random, stat, os.path, datetime, threading
+import  random, stat, os.path, datetime
 import  struct, io, traceback, hashlib, traceback
 
 try:
     import fcntl
 except:
     fcntl = None
 
@@ -31,23 +31,21 @@
 FILESIG     = b"PYDB"
 IDXSIG      = b"PYIX"
 RECSIG      = b"RECB"
 RECDEL      = b"RECX"
 RECSEP      = b"RECS"
 RECEND      = b"RECE"
 
-version = "1.5.2"
+VERSION = "1.7.1"
 
 # Accessed from the main file as well
 
 base_locktout   = LOCK_TIMEOUT   # Settable from ...
 base_pgdebug    = 0
 base_quiet      = 0
-base_integrity  = 0
-base_showdel    = 0
 
 class TwinCoreBase():
 
     ''' This class provides basic services to twincore  '''
 
     INTSIZE     = 4
 
@@ -67,14 +65,18 @@
         self.ifp = None
         self.cnt = 0
 
         #self.fname = "" ;        self.idxname = ""
         #self.lckname = "";
         self.lasterr = ""
 
+    def get_version(self):
+        ''' Return version sting. '''
+        return VERSION
+
     #def __del__(self):
     #    print("Flushing")
 
     def getsize(self, buffio):
 
         ''' get the dabase file size '''
```

### Comparing `pydbase-1.5.2/pydbase/twinchain.py` & `pydbase-1.7.1/pydbase/twinchain.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 #!/usr/bin/env python3
 
-'''!
-    @mainpage
-
-    # Twinchain
+'''
+    <pre>
 
-        Block chain layer on top of twincore.
+ Block chain layer on top of twincore.
 
-            prev     curr
-                record
-        |   Time Now    |   Time  Now    |  Time Now     |
-        |   hash256   | |    hash256   | |   hash256   | |
-        |   Header    | |    Header    | |   Header    | |
-        |   Payload   | |    Payload   | |   Payload   | |
-        |   Backlink  | |    Backlink  | |   Backlink  | |
-                      |----->---|      |---->---|     |------ ...
-
-        The sum of fields saved to the next backlink.
-
-        History:
-
-            0.0.0       Tue 20.Feb.2024     Initial release
-            0.0.0       Sun 26.Mar.2023     More features
-            1.2.0       Mon 26.Feb.2024     Moved pip home to pydbase/
-            1.4.0       Tue 27.Feb.2024     Addedd pgdebug
-            1.4.2       Wed 28.Feb.2024     Fixed multiple instances
-            1.4.3       Wed 28.Feb.2024     ChainAdm added
+    |   Time Now    |   Time  Now    |  Time Now     |
+    |   hash256   | |    hash256   | |   hash256   | |
+    |   Header    | |    Header    | |   Header    | |
+    |   Payload   | |    Payload   | |   Payload   | |
+    |   Backlink  | |    Backlink  | |   Backlink  | |
+                  |----->---|      |---->---|     |------
+
+    The sum of fields saved to the next backlink.
+
+    History:
+
+    1.1         Tue 20.Feb.2024     Initial release
+    1.2.0       Mon 26.Feb.2024     Moved pip home to pydbase/
+    1.4.0       Tue 27.Feb.2024     Addedd pgdebug
+    1.4.2       Wed 28.Feb.2024     Fixed multiple instances
+    1.4.3       Wed 28.Feb.2024     ChainAdm added
+    1.4.4       Fri 01.Mar.2024     Tests for chain functions
+    1.4.5       Fri 01.Mar.2024     Misc fixes
+    1.4.6       Mon 04.Mar.2024     Vacuum count on vacuumed records
+    1.4.7       Tue 05.Mar.2024     In place record update
+    1.4.8       Sat 09.Mar.2024     Added new locking mechanism
+    1.4.9       Mon 01.Apr.2024     Updated to run on MSYS2, new locking
+    1.5.0       Tue 02.Apr.2024     Cleaned, pip upload
+    1.5.1       Wed 10.Apr.2024     Dangling lock .. fixed
 
+    </pre>
 '''
 
 import  os, sys, getopt, signal, select, socket, time, struct
 import  random, stat, os.path, datetime, threading, uuid
 import  struct, io, hashlib
 
 import pyvpacker
@@ -60,17 +64,17 @@
 
 class TwinChain(TwinCore):
 
     '''
         Derive from database to accomodate block chain.
     '''
 
-    def __init__(self, fname = "pydbchain.pydb", pgdebug = 0, core_verbose = 0):
+    def __init__(self, fname = "pydbchain.pydb", pgdebug = 0, verbose = 0):
 
-        self.core_verbose = core_verbose
+        self.chain_verbose = verbose
 
         # Upper lock name
         ulockname = os.path.splitext(fname)[0] + ".ulock"
         self.ulock = FileLock(ulockname)
         self.ulock.waitlock()    #(self.ulockname)
 
         super(TwinChain, self).__init__(fname, pgdebug)
@@ -198,17 +202,17 @@
             decoded = self.packer.decode_data(arr[1])
             #print("decoded", decoded)
         except:
             print("Cannot decode record at", recnum, recnum, sys.exc_info())
             raise
         dic = self._get_fields(decoded[0])
 
-        if self.core_verbose > 2:
+        if self.chain_verbose > 2:
             print(dic)
-        if self.core_verbose > 0:
+        if self.chain_verbose > 0:
             print(dic['header'] + " " + dic['now'], dic['payload'])
 
         return arr[0].decode(), dic['payload']
 
     def get_payoffs_bykey(self, keyval, maxrec = 1):
         " get payload offset by key"
         arr = []
@@ -241,15 +245,15 @@
         rrr = self.getdbsize()
         for aa in range(rrr -1, -1, -1):
             head = self.get_header(aa)
             if head == keyval:
                 ch = self.checkdata(aa)
                 li = self.linkintegrity(aa)
 
-                if self.core_verbose:
+                if self.chain_verbose:
                     print("li", li, "ch", ch)
 
                 if not ch:
                     raise  DBCheckError("Check failed at rec %a" % aa);
                 if not li:
                     raise  DBLinkError("Link checl failed at rec %a" % aa);
 
@@ -266,99 +270,99 @@
         if self.pgdebug > 5:
             print("get_header()", recnum)
         arr = self.get_rec(recnum)
         if not arr:
             if self.pgdebug > 5:
                 print("get_header(): empty/deleted record", recnum)
 
-            if self.core_verbose > 1:
+            if self.chain_verbose > 1:
                 print("get_header(): empty/deleted record", recnum)
             return []
 
-        if self.core_verbose > 1:
+        if self.chain_verbose > 1:
             print("arr", arr)
             uuu = uuid.UUID(arr[0].decode())
             ddd = str(uuid2date(uuu))
             print("header", arr[0])
         return arr[0].decode()
 
     def linkintegrity(self, recnum):
 
         ''' Scan one record an its integrity based on the previous one '''
 
         if recnum < 1:
-            if self.core_verbose:
+            if self.chain_verbose:
                 print("Cannot check initial record.")
             return True
 
-        if self.core_verbose > 4:
+        if self.chain_verbose > 4:
             print("Checking link ...", recnum)
 
         arr = self.get_rec(recnum-1)
         try:
             decoded = self.packer.decode_data(arr[1])
         except:
             print("Cannot decode prev:", recnum, sys.exc_info())
             return
         dicold = self._get_fields(decoded[0])
         arr2 = self.get_rec(recnum)
         try:
             decoded2 = self.packer.decode_data(arr2[1])
         except:
-            if self.core_verbose > 2:
+            if self.chain_verbose > 2:
                 print("Cannot decode curr:", recnum, sys.exc_info())
             return
         dic = self._get_fields(decoded2[0])
         backlink = self._build_backlink(dicold)
         hhh = self._hashtohex(backlink)
-        if self.core_verbose > 2:
+        if self.chain_verbose > 2:
             print("calc      ", hhh)
             print("backlink  ", dic['backlink'])
         return hhh == dic['backlink']
 
     def checkdata(self, recnum):
 
         ''' Integrity check of record. '''
 
         arr = self.get_rec(recnum)
         try:
             decoded = self.packer.decode_data(arr[1])
         except:
-            if self.core_verbose > 2:
+            if self.chain_verbose > 2:
                 print("Cannot decode:", recnum, sys.exc_info())
             return
 
         aaa = self._get_fields(decoded[0])
         sumstr = self._build_sumstr(aaa)
         hhh = self._hashtohex(sumstr)
-        if self.core_verbose > 1:
+        if self.chain_verbose > 1:
             print("data", hhh)
-        if self.core_verbose > 2:
+        if self.chain_verbose > 2:
             print("hash", aaa['hash256'])
         return hhh == aaa['hash256']
 
     def appendwith(self, header, datax):
 
         ''' Append data and header to the end of database '''
 
         #if type(header) != type(b""):
         #    header = header.encode() #errors='strict')
 
         #if type(datax) != type(b""):
         #    datax = datax.encode() #errors='strict')
 
-        if self.core_verbose > 0:
+        if self.chain_verbose > 0:
             print("Appendwith", header, datax)
 
         self.ulock.waitlock()    #self.ulockname)
 
         try:
             uuu = uuid.UUID(header)
         except:
-            if self.core_verbose:
+            if self.chain_verbose:
                 print("Header override must be a valid UUID string.")
 
             self.ulock.unlock() #self.ulockname)
             raise ValueError("Header override must be a valid UUID string.")
 
         old_dicx = {}
         # Get last data from db
@@ -386,26 +390,26 @@
         encoded = self.packer.encode_data("", aaa)
 
         #print("save", header, "-", encoded)
         #print("bbb", self.getdbsize())
         self.save_data(header, encoded)
         #print("eee", self.getdbsize())
 
-        if self.core_verbose > 1:
+        if self.chain_verbose > 1:
             bbb = self.packer.decode_data(encoded)
             print("Rec", bbb[0])
 
         self.ulock.unlock() #self.ulockname)
         return True
 
     def append(self, datax):
 
         ''' Append data to the end of database '''
 
-        if self.core_verbose > 0:
+        if self.chain_verbose > 0:
             print("Append", datax)
 
         # Get last data from db
         #sss = self.getdbsize()
         #if not sss:
         #    #raise ValueError("Invalid database, must have at least one record.")
         #    pass
```

### Comparing `pydbase-1.5.2/pydbase/twincore.py` & `pydbase-1.7.1/pydbase/twincore.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,81 +1,96 @@
 #!/usr/bin/env python3
 
-'''!
-    @mainpage
+# pylint: disable=C0321
+# pylint: disable=C0209
+# pylint: disable=C0103
+# pylint: disable=E0602
 
-        Database with two files. One for data, one for index;
-
-        The reason for the 'twin' name is that two files are created.
-        The first contains the data, the second contains the
-        offsets (indexes) and hashes.
-
-        The second file can be re-built easily from the first
-        using the reindex option.
-
-        Structure of the data:
-
-            32 byte header, starating with FILESIG;
-
-            4 bytes    4 bytes          4 bytes         Variable
-            ------------------------------------------------------------
-            RECSIG     Hash_of_key      Len_of_key      DATA_for_key
-            RECSEP     Hash_of_payload  Len_of_payload  DATA_for_payload
-                .
-                .
-
-            RECSIG     Hash_of_key      Len_of_key      DATA_for_key
-            RECSEP     Hash_of_payload  Len_of_payload  DATA_for_payload
-
-        Deleted records are marked with RECSIG mutated from RECB to RECX
-
-        New data is appended to the end, no duplicate filtering is done.
-        Retrieval is searched from reverse, the latest record with this key
-        is retrieved first.
-
-        Verbosity:    (use the '-v' option multiple times)
-
-            0 =  no output
-            1 =  normal, some items printed, short record ;
-            2 =  more detail; full record (-vv)
-            3 =  more detail + damaged records (-vvv)
-
-        Debug:    (use the '-d' option with number)
-
-            0 =  no output
-            1 =  normal, some items
-            2 =  more details
-
-        History:
+'''
+    <pre>
+    Database with two files. One for data, one for index;
 
-            1.1         Tue 20.Feb.2024     Initial release
-            1.2.0       Mon 26.Feb.2024     Moved pip home to pydbase/
-            1.4.0       Tue 27.Feb.2024     Addedd pgdebug
-            1.4.2       Wed 28.Feb.2024     Fixed multiple instances
-            1.4.3       Wed 28.Feb.2024     ChainAdm added
-            1.4.4       Fri 01.Mar.2024     Tests for chain functions
-            1.4.5       Fri 01.Mar.2024     Misc fixes
-            1.4.6       Mon 04.Mar.2024     Vacuum count on vacuumed records
-            1.4.7       Tue 05.Mar.2024     In place record update
-            1.4.8       Sat 09.Mar.2024     Added new locking mechanism
+    The reason for the 'twin' name is that two files are created.
+    The first contains the data, the second contains the
+    offsets (indexes) and hashes.
+
+    The second file can be re-built easily from the first
+    using the reindex option.
+
+    Structure of the data:
+
+        32 byte header, starating with FILESIG;
+
+        4 bytes    4 bytes          4 bytes         Variable
+        ------------------------------------------------------------
+        RECSIG     Hash_of_key      Len_of_key      DATA_for_key
+        RECSEP     Hash_of_payload  Len_of_payload  DATA_for_payload
+            .
+            .
+
+        RECSIG     Hash_of_key      Len_of_key      DATA_for_key
+        RECSEP     Hash_of_payload  Len_of_payload  DATA_for_payload
+
+    Deleted records are marked with RECSIG mutated from RECB to RECX
+
+    New data is appended to the end, no duplicate filtering is done.
+    Retrieval is searched from reverse, the latest record with this key
+    is retrieved first.
+
+    Verbosity:    (use the '-v' option multiple times)
+
+        0 =  no output
+        1 =  normal, some items printed, short record ;
+        2 =  more detail; full record (-vv)
+        3 =  more detail + damaged records (-vvv)
+
+    Debug:    (use the '-d' option with number)
+
+        0 =  no output
+        1 =  normal, some items
+        2 =  more details
+
+    History:
+
+        1.1         Tue 20.Feb.2024     Initial release
+        1.2.0       Mon 26.Feb.2024     Moved pip home to pydbase/
+        1.4.0       Tue 27.Feb.2024     Addedd pgdebug
+        1.4.2       Wed 28.Feb.2024     Fixed multiple instances
+        1.4.3       Wed 28.Feb.2024     ChainAdm added
+        1.4.4       Fri 01.Mar.2024     Tests for chain functions
+        1.4.5       Fri 01.Mar.2024     Misc fixes
+        1.4.6       Mon 04.Mar.2024     Vacuum count on vacuumed records
+        1.4.7       Tue 05.Mar.2024     In place record update
+        1.4.8       Sat 09.Mar.2024     Added new locking mechanism
+        1.4.9       Mon 01.Apr.2024     Updated to run on MSYS2, new locking
+        1.5.0       Tue 02.Apr.2024     Cleaned, pip upload
+        1.5.1       Wed 10.Apr.2024     Dangling lock .. fixed
+        1.6.0       Thu 25.Apr.2024     Added IDX pre and post callbacks
+        1.6.1       Mon 29.Apr.2024     D: option corrected
+
+        ... more ... see README.md
+
+    In the code the term positions and absolute positions refer to
+    the ordinal number of the record. The offset refers to the file
+    offset of the record.
 
+        </pre>
 '''
 
-import  os, sys, getopt, signal, select, socket, time, struct
-import  random, stat, os.path, datetime, threading
-import  struct, io
+import  os
+import  sys
+import  struct
+import  threading
 
 base = os.path.dirname(os.path.realpath(__file__))
 sys.path.append(os.path.join(base))
 sys.path.append(os.path.join(base, '..', 'pydbase'))
 
 from twinbase import *
 
-Version = "1.4.8"
-
 # ------------------------------------------------------------------------
 
 class TwinCore(TwinCoreBase):
 
     '''
 
      Data file and index file; protected by locks
@@ -86,21 +101,26 @@
     def __init__(self, fname = "pydbase.pydb", pgdebug = 0, devmode = 1):
 
         self.cnt = 0
         self.fname = fname
         self.lckname  = os.path.splitext(self.fname)[0] + ".lock"
         self.idxname  = os.path.splitext(self.fname)[0] + ".pidx"
         self.pgdebug = pgdebug
-        self.base_verbose  = 0
-        self.core_verbose  = 0
+        self.verbose  = 0
+        self.showdel  = 0
+        self.integrity = 0
         self.devmode = devmode
         self.lock = FileLock(self.lckname)
 
+        # Thu 25.Apr.2024 these are added for index creation
+        self.preexec = None
+        self.postexec = None
+
         # Make sure only one process can use this
-        self.lock.waitlock() #self.lckname)
+        self.lock.waitlock()
 
         super(TwinCore, self).__init__(pgdebug)
 
         #print("initializing core with", fname, pgdebug)
         #self.pool = threading.BoundedSemaphore(value=1)
 
         # It was informative at one point
@@ -145,31 +165,30 @@
             #self.ifp = self.softcreate(self.idxname)
             indexsize = self.getsize(self.ifp)
 
             # See if valid index
             if indexsize < HEADSIZE:
                 self.create_idx(self.ifp)
                 # It was an existing data, new index needed
-                if self.base_verbose > 0:
+                if self.verbose > 0:
                     print("Reindexing")
                 self.__reindex()
 
         # Check
         if  self.getbuffstr(0, 4) != FILESIG:
-            if self.base_verbose > 2:
+            if self.verbose > 2:
                 print("Invalid data signature")
-            self.lock.unlock()  #dellock(self.lckname)
+            self.lock.unlock()
             raise  RuntimeError("Invalid database signature.")
 
         #print("buffsize", buffsize, "indexsize", indexsize)
-        self.lock.unlock() #dellock(self.lckname)
+        self.lock.unlock()
 
     def version(self):
-        ''' Return version sting. '''
-        return Version
+        return VERSION
 
     def flush(self):
 
         ''' Flush files to disk. '''
 
         if self.pgdebug > 9:
             print("Flushing", self.fp, self.ifp)
@@ -207,61 +226,65 @@
             ret = 0
 
         return  ret
 
     # --------------------------------------------------------------------
     def _rec2arr(self, rec):
 
+        # Wed 10.Apr.2024 decision is made at the higher level
         arr = []
         sig = self.getbuffstr(rec, self.INTSIZE)
 
-        if sig == RECDEL:
-            return arr
-
-        if sig != RECSIG:
-            if self.base_verbose > 0:
+        if sig != RECSIG and sig != RECDEL:
+            if self.verbose > 0:
                 print(" Damaged data (sig) '%s' at" % sig, rec)
             return arr
 
         hash = self.getbuffint(rec+4)
         blen = self.getbuffint(rec+8)
         data = self.getbuffstr(rec + 12, blen)
 
-        if base_integrity:
+        if self.integrity:
             ccc = self.hash32(data)
-            if self.base_verbose > 1:
+            if self.verbose > 1:
                 print("rec", rec, "hash", hex(hash), "check", hex(ccc))
             if hash != ccc:
-                if self.base_verbose > 0:
+                if self.verbose > 0:
                     print("Error on hash at rec", rec, "hash", hex(hash), "check", hex(ccc))
                 return []
 
         #print("%5d pos %5d" % (cnt, rec), "hash %8x" % hash, "ok", ok, "len=", blen, end=" ")
 
         endd = self.getbuffstr(rec + 12 + blen, self.INTSIZE)
         if endd != RECSEP:
-            if self.base_verbose > 0:
+            if self.verbose > 0:
                 print(" Damaged data (sep) '%s' at" % endd, rec)
             return arr
 
-        rec2 = rec + 16 + blen;
+        rec2 = rec + 16 + blen
         hash2 = self.getbuffint(rec2)
         blen2 = self.getbuffint(rec2+4)
         data2 = self.getbuffstr(rec2+8, blen2)
 
-        if base_integrity:
+        if self.integrity:
             ccc2 = self.hash32(data2)
-            if self.base_verbose > 1:
+            if self.verbose > 1:
                 print("rec", rec, "hash2", hex(hash2), "check2", hex(ccc2))
             if hash2 != ccc2:
-                if self.base_verbose > 0:
+                if self.verbose > 0:
                     print("Error on hash at rec", rec, "hash2", hex(hash2), "check2", hex(ccc2))
                 return []
 
-        arr = [data, data2]
+        if sig == RECDEL:
+            if self.showdel:
+                arr = [b"del", data, data2]
+            else:
+                arr = []
+        else:
+            arr = [data, data2]
         return arr
 
     # -------------------------------------------------------------------
     # Originator, dump single record
 
     def  dump_rec(self, rec, cnt):
 
@@ -272,164 +295,165 @@
 
         cnt2 = 0
         sig = self.getbuffstr(rec, self.INTSIZE)
         if self.pgdebug > 5:
             print("Sig ", sig, "at", rec)
 
         if sig == RECDEL:
-            if base_showdel:
+            if self.showdel:
                 klen = self.getbuffint(rec+8)
                 kdata = self.getbuffstr(rec+12, klen)
-                rec2 = rec + 16 + klen;
+                rec2 = rec + 16 + klen
                 blen = self.getbuffint(rec2+4)
                 data = self.getbuffstr(rec2+8, blen)
                 print(" Del at", rec, "key:", kdata, "data:", truncs(data))
-            if self.base_verbose > 1:
+            if self.verbose > 1:
                 klen = self.getbuffint(rec+8)
                 kdata = self.getbuffstr(rec+12, klen)
-                rec2 = rec + 16 + klen;
+                rec2 = rec + 16 + klen
                 blen = self.getbuffint(rec2+4)
                 data = self.getbuffstr(rec2+8, blen)
-                if self.base_verbose > 2:
+                if self.verbose > 2:
                     print(" Del at", rec, "key:", kdata, "data:", data)
                 else:
                     print(" Del at", rec, "key:", kdata, "data:", truncs(data))
 
             return cnt2
 
         if sig != RECSIG:
-            if self.base_verbose > 1:
+            if self.verbose > 1:
                 print(" Damaged data (sig) '%s' at" % sig, rec)
             return cnt2
 
         hash = self.getbuffint(rec+4)
         blen = self.getbuffint(rec+8)
 
         if blen < 0:
-            if self.base_verbose > 2:
+            if self.verbose > 2:
                 print("Invalid key length %d at %d" % (blen, rec))
             return cnt2
 
         data = self.getbuffstr(rec+12, blen)
-        if base_integrity:
+        if self.integrity:
             ccc = self.hash32(data)
-            if self.base_verbose > 1:
+            if self.verbose > 1:
                 print("rec", rec, "hash", hex(hash), "check", hex(ccc))
             if hash != ccc:
-                if self.base_verbose > 0:
+                if self.verbose > 0:
                     print("Error on hash at rec", rec, "hash", hex(hash), "check", hex(ccc))
                 return []
 
         endd = self.getbuffstr(rec + 12 + blen, self.INTSIZE)
         if endd != RECSEP:
-            if self.base_verbose > 0:
+            if self.verbose > 0:
                 print(" Damaged data (sep) '%s' at" % endd, rec)
             return cnt2
 
-        rec2 = rec + 16 + blen;
+        rec2 = rec + 16 + blen
         hash2 = self.getbuffint(rec2)
         blen2 = self.getbuffint(rec2+4)
 
         if blen2 < 0:
-            if self.base_verbose > 1:
+            if self.verbose > 1:
                 print("Invalid data length %d at %d" % (blen2, rec))
             return cnt2
 
         data2 = self.getbuffstr(rec2+8, blen2)
-        if base_integrity:
+        if self.integrity:
             ccc2 = self.hash32(data2)
-            if self.base_verbose > 1:
+            if self.verbose > 1:
                 print("rec", rec, "hash2", hex(hash), "check2", hex(ccc))
             if hash2 != ccc2:
-                if self.base_verbose > 0:
+                if self.verbose > 0:
                     print("Error on hash at rec", rec, "hash2", hex(hash), "check2", hex(ccc))
                 return []
 
-        if self.base_verbose > 2:
+        if self.verbose > 2:
             print("%-5d pos %5d" % (cnt, rec), "%8x" % hash, "len", blen, data,
                                                         "%8x" % hash2,"len", blen2, data2)
 
-        elif self.base_verbose > 1:
+        elif self.verbose > 1:
             print("%-5d pos %5d" % (cnt, rec), "%8x" % hash, "len", blen, data,
                                                         "%8x" % hash2,"len", blen2, data2)
-        elif self.base_verbose:
+        elif self.verbose:
             print("%-5d pos %5d" % (cnt, rec),  data, data2)
         else:
-            print("%-5d pos %5d" % (cnt, rec), "Data:", truncs(data, 18), "Data2:", truncs(data2, 18))
+            print("%-5d pos %5d" % (cnt, rec),
+                    "Data:", truncs(data, 18),
+                            "Data2:", truncs(data2, 18))
 
         cnt2 += 1
         return cnt2
 
     def  check_rec(self, rec, cnt2):
 
         ''' Check record. Verbose to the screen. Return number of errors.'''
 
         ret = 0
         sig = self.getbuffstr(rec, self.INTSIZE)
 
         # Do not check deleted, say OK
         if sig == RECDEL:
-            if self.base_verbose > 1:
+            if self.verbose > 1:
                 print(" Deleted data '%s' at %d (%d)" % (sig, rec, cnt2))
             ret = 1
             return ret
 
         if sig != RECSIG:
-            if self.base_verbose > 0:
+            if self.verbose > 0:
                 print(" Damaged data (sig) '%s' at %d (%d)" % (sig, rec, cnt2))
-            #if self.base_verbose > 1:
+            #if self.verbose > 1:
             #    print("Data", data)
 
             return ret
 
-        hash = self.getbuffint(rec+4)
+        hashx = self.getbuffint(rec+4)
         blen = self.getbuffint(rec+8)
 
         if blen <= 0:
-            if self.base_verbose > 1:
+            if self.verbose > 1:
                 print("Invalid key length %d at %d" % (blen, rec))
             return ret
 
         data = self.getbuffstr(rec+12, blen)
         ccc = self.hash32(data)
-        if hash != ccc:
-            if self.base_verbose > 1:
+        if hashx != ccc:
+            if self.verbose > 1:
                 print("Data", data)
-            elif self.base_verbose > 0:
+            elif self.verbose > 0:
                 print("Error on hash at rec", rec, cnt2, "hash",
-                                            hex(hash), "check", hex(ccc))
-
+                                            hex(hashx), "check", hex(ccc))
             return ret
 
         endd = self.getbuffstr(rec + 12 + blen, self.INTSIZE)
         if endd != RECSEP:
-            if self.base_verbose > 0:
+            if self.verbose > 0:
                 print(" Damaged data (sep) '%s' at %d %d %d" % (endd, rec, cnt2))
             return ret
 
-        rec2 = rec + 16 + blen;
+        rec2 = rec + 16 + blen
         hash2 = self.getbuffint(rec2)
         blen2 = self.getbuffint(rec2+4)
 
         if blen2 < 0:
-            if self.base_verbose > 1:
+            if self.verbose > 1:
                 print("Invalid data length2 %d at %d" % (blen2, rec))
             return ret
 
         data2 = self.getbuffstr(rec2+8, blen2)
         ccc2 = self.hash32(data2)
         if hash2 != ccc2:
-            if self.base_verbose > 1:
+            if self.verbose > 1:
                 print("Data", data, "Data2", data2)
-            elif self.base_verbose > 0:
+            elif self.verbose > 0:
                 print("Error on hash2 at rec", rec, cnt2, "hash2",
                                         hex(hash2), "check2", hex(ccc2))
             return ret
 
-        if self.base_verbose > 2:
+        if self.verbose > 2:
             print("Record at %d (%d) OK." % (rec, cnt2))
 
         ret += 1
         return ret
 
     # --------------------------------------------------------------------
     # Internal; no locking
@@ -450,26 +474,23 @@
         else:
             rrr = range(chash - self.INTSIZE * 2, HEADSIZE  - self.INTSIZE * 2, -self.INTSIZE * 2)
 
         for aa in rrr:
             rec = self.getidxint(aa)
 
             #print(aa, rec)
-            if not base_quiet:
-                cnt2 += 1
-                ret = self.dump_rec(rec, cnt)
-
-                if not ret:
-                    if self.pgdebug > 5:
-                        print("Deleted / empty record at", cnt)
-
-                if ret:
-                    cnt += 1
-                    if cnt >= lim:
-                        break
+            cnt2 += 1
+            ret = self.dump_rec(rec, cnt)
+            if not ret:
+                if self.pgdebug > 5:
+                    print("Deleted / empty record at", cnt)
+            if ret:
+                cnt += 1
+                if cnt >= lim:
+                    break
 
     def  dump_data(self, lim = INT_MAX, skip = 0):
 
         ''' Put all data to screen. '''
 
         self.__dump_data(lim, skip, 1)
 
@@ -479,17 +500,17 @@
 
         self.__dump_data(lim, skip)
 
     def  reindex(self):
 
         ''' Re create index file. '''
 
-        self.lock.waitlock() #self.lckname)
+        self.lock.waitlock()
         ret = self.__reindex()
-        self.lock.unlock()    #dellock(self.lckname)
+        self.lock.unlock()
         return ret
 
     # --------------------------------------------------------------------
 
     def  __reindex(self):
 
         ''' Recover index. Make sure the DB in not in session.  '''
@@ -510,50 +531,50 @@
         tmplock = FileLock(relock)
         tmplock.waitlock()
 
         tempifp = self.softcreate(reidx)
         self.create_idx(tempifp)
         dlen = self.getsize(self.fp)
 
-        if self.base_verbose > 2:
-           print("curr", curr, "dlen", dlen)
+        if self.verbose > 2:
+            print("curr", curr, "dlen", dlen)
 
         aa =  HEADSIZE
         while 1:
             if aa >= dlen:
                 break
 
             sig = self.getbuffstr(aa, self.INTSIZE)
             # Check if sig is correct
             if sig != RECSIG:
-                if self.core_verbose > 0:
+                if self.verbose > 0:
                     print("Invalid sig .. resync needed")
                 raise
 
             #print("reind", aa)
 
             try:
                 hhh2 = self.getbuffint(aa + 4)
                 lenx = self.getbuffint(aa + 8)
                 if lenx < 0:
-                    if self.core_verbose > 0:
+                    if self.verbose > 0:
                         print("Invalid key length.")
                 sep =  self.getbuffstr(aa + 12 + lenx, self.INTSIZE)
                 len2 =  self.getbuffint(aa + 20 + lenx)
                 if len2 < 0:
-                    if self.core_verbose > 0:
+                    if self.verbose > 0:
                         print("Invalid record length")
             except:
-                if self.core_verbose > 2:
+                if self.verbose > 2:
                     print("in reindex", sys.exc_info())
 
-            if self.base_verbose == 1:
+            if self.verbose == 1:
                 print(aa, "sig", sig, "hhh2", hex(hhh2), "len", lenx, \
                     "sep", sep, "len2", len2)
-            if self.base_verbose > 1:
+            if self.verbose > 1:
                 data =  self.getbuffstr(aa + 12, lenx)
                 data2 =  self.getbuffstr(aa + 24 + lenx, len2)
                 print(aa, "sig", sig, "data", data, "data2", data2)
 
             # Update / Append index
             #hashpos = self._getint(tempifp, CURROFFS)
             hashpos =  HEADSIZE  + self._getdbsize(tempifp) * self.INTSIZE * 2
@@ -626,17 +647,17 @@
         '''
             Remove all deleted data. Reindex.
             The db is locked while the vacuum is in operation, but
             make sure the DB in not in session, and no pending
             operations are present (like find / retrieve cycle).
         '''
 
-        self.lock.waitlock() #self.lckname)
+        self.lock.waitlock()
         ret = self._vacuum()
-        self.lock.unlock()  #dellock(self.lckname)
+        self.lock.unlock()
         return ret
 
     def  _vacuum(self):
 
         vacname = os.path.splitext(self.fname)[0] + "_vac_" + ".pydb"
         vacerr  = os.path.splitext(self.fname)[0] +  ".perr"
         vacidx = os.path.splitext(vacname)[0]  + ".pidx"
@@ -672,24 +693,21 @@
                 sig = self.getbuffstr(rec, self.INTSIZE)
                 if sig == RECDEL:
                     ret += 1
                     vac += 1
                     if self.pgdebug > 1:
                         print("deleted", rec)
                 elif sig != RECSIG:
-                    if self.base_verbose:
+                    if self.verbose:
                         print("Detected error at %d" % rec)
                     ret += 1
                     self.__save_error(rec, vacerrfp)
                 else:
-                    global base_integrity
-                    tmpi = base_integrity
-                    base_integrity = True
+                    self.integrity = True
                     arr = self.get_rec_byoffs(rec)
-                    base_integrity = tmpi
 
                     if self.pgdebug > 1:
                         print(cnt, "vac rec", rec, arr)
 
                     if len(arr) > 1:
                         hhh2 = self.hash32(arr[0])
                         hhh3 = self.hash32(arr[1])
@@ -701,103 +719,103 @@
                         if self.pgdebug > 0:
                             print("Error on vac: %d" % rec)
                 cnt += 1
 
             vacdb.fp.close()
             vacdb.ifp.close()
 
-            vacdb.lock.unlock()  #dellock(vacdb.lckname)
+            vacdb.lock.unlock()
 
             # if vacerr is empty
             try:
                 if os.stat(vacerr).st_size == 0:
                     #print("Vac error empty")
                     os.remove(vacerr)
             except:
-                if self.core_verbose > 0:
+                if self.verbose > 0:
                     print("vacerr", sys.exc_info())
 
         # Any vacummed?
         if vac > 0:
             # Make it go out of scope
             self.fp.flush(); self.ifp.flush()
             self.fp.close(); self.ifp.close()
 
             # Now move files
             try:
-                os.remove(self.fname);
+                os.remove(self.fname)
             except:
-                if self.core_verbose > 0:
+                if self.verbose > 0:
                     print("vacuum remove", self.fname, sys.exc_info())
                 pass
 
             try:
                 os.remove(self.idxname)
             except:
-                if self.core_verbose > 2:
+                if self.verbose > 2:
                     print("vacuum idx remove", self.idxname, sys.exc_info())
                 pass
 
             if self.pgdebug > 1:
                 print("rename", vacname, "->", self.fname)
                 print("rename", vacidx, "->", self.idxname)
 
             try:
                 os.rename(vacname, self.fname)
             except:
-                if self.core_verbose > 2:
+                if self.verbose > 2:
                     print("vacuum rename", vacname, sys.exc_info())
             try:
                 os.rename(vacidx, self.idxname)
             except:
-                if self.core_verbose > 2:
+                if self.verbose > 2:
                     print("vacuum idx rename", vacidx, sys.exc_info())
 
-            self.lock.waitlock() #self.lckname)
+            self.lock.waitlock()
             self.fp = self.softcreate(self.fname)
             self.ifp = self.softcreate(self.idxname)
-            #self.lock.unlock()  #dellock(self.lckname)
+            #self.lock.unlock()
 
         else:
             # Just remove non vacuumed files
             if self.pgdebug > 1:
                 print("deleted", vacname, vacidx)
             try:
                 os.remove(vacname)
                 os.remove(vacidx)
             except:
                 pass
 
         #self.lock.unlock()
-        #dellock(self.lckname)
+
 
         #print("ended vacuum")
         return ret, vac
 
     def  get_rec(self, recnum):
 
         ''' Get record from database; recnum is a zero based record counter. '''
 
         if self.pgdebug:
-            print("getrec()", recnum)
+            print("get_rec()", recnum)
 
         rsize = self._getdbsize(self.ifp)
         if recnum >= rsize:
-            if self.core_verbose > 0:
-                print("Past end of data.");
-            raise  RuntimeError( \
-                    "Past end of Data. Asking for %d while max is 0 .. %d records." \
-                                     % (recnum, rsize-1) )
+            if self.verbose > 0:
+                print("Past end of data.")
+            errx =  "Past end of Data. (ask: %d max: %d)"  % (recnum, rsize-1)
+            raise  RuntimeError(errx)
             return []
 
         chash = self.getidxint(CURROFFS)
         #print("chash", chash)
         offs = self.getidxint(HEADSIZE + recnum * self.INTSIZE * 2)
 
-        #print("offs", offs)
+        #sig = self.getbuffstr(offs, self.INTSIZE)
+
         return self._rec2arr(offs)
 
     def  get_rec_byoffs(self, recoffs):
 
         ''' Return record by offset. '''
 
         rsize = self.getsize(self.fp)
@@ -806,19 +824,18 @@
             raise  RuntimeError( \
                     "Past end of File. Asking for offset %d file size is %d." \
                                      % (recoffs, rsize) )
             return []
 
         sig = self.getbuffstr(recoffs, self.INTSIZE)
         if sig == RECDEL:
-            if self.base_verbose:
+            if self.verbose:
                 print("Deleted record.")
-            return []
         if sig != RECSIG:
-            if self.core_verbose > 0:
+            if self.verbose > 0:
                 print("Unlikely offset %d is not at record boundary." % recoffs, sig)
             return []
         #print("recoffs", recoffs)
         return self._rec2arr(recoffs)
 
     def  get_key_offs(self, recoffs):
 
@@ -830,293 +847,302 @@
             raise  RuntimeError( \
                     "Past end of File. Asking for offset %d file size is %d." \
                                      % (recoffs, rsize) )
             return []
 
         sig = self.getbuffstr(recoffs, self.INTSIZE)
         if sig == RECDEL:
-            if self.base_verbose:
+            if self.verbose:
                 print("Deleted record.")
             return []
         if sig != RECSIG:
-            if self.core_verbose > 0:
+            if self.verbose > 0:
                 print("Unlikely offset %d is not at record boundary." % recoffs, sig)
             return []
         #print("recoffs", recoffs)
         return self._rec2arr(recoffs)[0]
 
     def  del_rec(self, recnum):
 
         ''' Delete by record number.
             Deleted record is marked as deleted but not removed.
             Deleted records are ignored in further operations.
             Use 'vacuum' to actually remove record.
         '''
 
+        if recnum < 0:
+            raise  RuntimeError("Invalid recnum %d" % recoffs)
+
         rsize = self._getdbsize(self.ifp)
         if recnum >= rsize:
-            if self.base_verbose:
-                print("Past end of data.");
+            if self.verbose:
+                print("Past end of data.")
             return False
         chash = self.getidxint(CURROFFS)
         #print("chash", chash)
         offs = self.getidxint(HEADSIZE + recnum * self.INTSIZE * 2)
         #print("offs", offs)
         old = self.getbuffstr(offs, self.INTSIZE)
         if old == RECDEL:
-            if self.base_verbose:
-                print("Record at %d already deleted." % offs);
+            if self.verbose:
+                print("Record at %d already deleted." % offs)
             return False
 
         self.putbuffstr(offs, RECDEL)
         return True
 
     def  del_rec_offs(self, recoffs):
 
         ''' Delete record by file offset. '''
 
+        if recoffs < 0:
+            raise  RuntimeError("Invalid offset %d" % recoffs)
+
         rsize = self.getsize(self.fp)
         if recoffs >= rsize:
             #print("Past end of data.");
             raise  RuntimeError( \
                     "Past end of File. Asking for offset %d file size is %d." \
                                      % (recoffs, rsize) )
             return False
 
         sig = self.getbuffstr(recoffs, self.INTSIZE)
         if sig != RECSIG  and sig != RECDEL:
-            if self.core_verbose > 0:
+            if self.verbose > 0:
                 print("Unlikely offset %d is not at record boundary." % recoffs, sig)
             return False
 
         self.putbuffstr(recoffs, RECDEL)
         return True
 
     # Check integrity
 
     def integrity_check(self, skip = 0, count = 0xffffffff):
 
         ''' Check record integrity for 'count' records.
             Skip number of records.
         '''
 
-        self.lock.waitlock()    #(self.lckname)
-        ret = 0; cnt2 = 0; cnt3 = 0;
+        self.lock.waitlock()
+        ret = 0; cnt2 = 0; cnt3 = 0
         #chash = self.getidxint(CURROFFS)        #;print("chash", chash)
         chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
         # Direction sensitivity
         rrr = range(HEADSIZE + skip * self.INTSIZE * 2, chash, self.INTSIZE * 2)
         for aa in rrr:
             rec = self.getidxint(aa)
             #print(aa, rec)
             ret += self.check_rec(rec, cnt2)
             cnt2 += 1
             cnt3 += 1
             if cnt3 >= count:
                 break
-        self.lock.unlock() #dellock(self.lckname)
+        self.lock.unlock()
         return ret, cnt2
 
     def  retrieve(self, strx, limx = 1):
 
-        ''' Retrive in reverse, limit it. '''
+        ''' Retrive in reverse, limit it. Compare by hash.'''
 
         if type(strx) != type(b""):
             strx = strx.encode(errors='strict')
 
         hhhh = self.hash32(strx)
         if self.pgdebug > 2:
             print("strx", strx, hhhh)
 
         #chash = self.getidxint(CURROFFS)
         chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
 
         #;print("chash", chash)
         arr = []
 
-        self.lock.waitlock() #(self.lckname)
+        self.lock.waitlock()
 
         #for aa in range(HEADSIZE + self.INTSIZE * 2, chash, self.INTSIZE * 2):
         for aa in range(chash - self.INTSIZE * 2, HEADSIZE  - self.INTSIZE * 2, -self.INTSIZE * 2):
             rec = self.getidxint(aa)
             sig = self.getbuffstr(rec, self.INTSIZE)
             if sig == RECDEL:
-                if self.base_verbose > 3:
+                if self.verbose > 3:
                     print(" Deleted record '%s' at" % sig, rec)
             elif sig != RECSIG:
-                if self.base_verbose:
+                if self.verbose:
                     print(" Damaged data '%s' at" % sig, rec)
             else:
                 hhh = self.getbuffint(rec+4)
                 if hhh == hhhh:
                     arr.append(self.get_rec_byoffs(rec))
                     if len(arr) >= limx:
                         break
-        self.lock.unlock()  #dellock(self.lckname)
+        self.lock.unlock()
 
         return arr
 
     # Return record offset
 
     def  _recoffset(self, strx, limx = INT_MAX, skipx = 0):
 
         #chash = self.getidxint(CURROFFS)
         #;print("chash", chash)
         chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
         rec = 0; blen = 0; data = ""
-        arr = []
+        #arr = []
         if type(strx) != type(b""):
-            strx2 = strx.encode(errors='strict');
+            strx2 = strx.encode(errors='strict')
         else:
             strx2 = strx
 
         #print("_recoffset", strx2)
 
         #for aa in range(HEADSIZE + self.INTSIZE * 2, chash, self.INTSIZE * 2):
         for aa in range(chash - self.INTSIZE * 2, HEADSIZE  - self.INTSIZE * 2, -self.INTSIZE * 2):
             rec = self.getidxint(aa)
             sig = self.getbuffstr(rec, self.INTSIZE)
             if sig == RECDEL:
-                if base_showdel:
+                if self.showdel:
                     print(" Deleted record '%s' at" % sig, rec)
             elif sig != RECSIG:
-                if self.base_verbose > 0:
+                if self.verbose > 0:
                     print(" Damaged data '%s' at" % sig, rec)
             else:
                 blen = self.getbuffint(rec+8)
                 keyz = self.getbuffstr(rec + 12, blen)
-                if self.base_verbose > 1:
+                if self.verbose > 1:
                     print("_recoffset", keyz)
                 if strx2 == keyz:
                     sig = self.getbuffstr(rec + 16 + blen,  self.INTSIZE)
                     xlen = self.getbuffint(rec + 20 + blen)
                     data = self.getbuffstr(rec + 24 + blen, xlen)
                     #print("rec offset", rec + 12,  "key:", keyz, "data:", data)
                     break       # Only the last one
         return rec, rec+24 + blen, len(data)
 
     def  findrec(self, strx, limx = INT_MAX, skipx = 0):
 
-        ''' Find by string matching substring. '''
+        ''' Find key by matching strx with substring.
+        Return record(s).
+        '''
 
-        self.lock.waitlock()    #(self.lckname)
+        self.lock.waitlock()
 
         #chash = self.getidxint(CURROFFS)            #;print("chash", chash)
         chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
 
         arr = []
-        strx2 = strx.encode(errors='strict');
+        strx2 = strx.encode(errors='strict')
 
         #print("findrec", strx2)
 
         #for aa in range(HEADSIZE + self.INTSIZE * 2, chash, self.INTSIZE * 2):
         for aa in range(chash - self.INTSIZE * 2, HEADSIZE  - self.INTSIZE * 2, -self.INTSIZE * 2):
             rec = self.getidxint(aa)
             sig = self.getbuffstr(rec, self.INTSIZE)
             if sig == RECDEL:
-                if base_showdel:
+                if self.showdel:
                     print(" Deleted record '%s' at" % sig, rec)
             elif sig != RECSIG:
-                if self.base_verbose > 0:
+                if self.verbose > 0:
                     print(" Damaged data '%s' at" % sig, rec)
             else:
                 blen = self.getbuffint(rec+8)
                 data = self.getbuffstr(rec + 12, blen)
-                if self.base_verbose > 1:
+                if self.verbose > 1:
                     print("find", data)
                 #if str(strx2) in str(data):
                 if strx2 in data:
-                    arr.append(self.get_key_offs(rec))
+                    #arr.append(self.get_key_offs(rec))
+                    arr.append(self.get_rec_byoffs(rec))
                     #arr.append(rec)
-
                     if len(arr) >= limx:
                         break
-        self.lock.unlock()  #dellock(self.lckname)
+        self.lock.unlock()
 
         return arr
 
     def  findrecpos(self, strx, limx = INT_MAX, skipx = 0):
 
-        ''' Find record, return array of positions. '''
+        ''' Find record by key, return array of positions. '''
 
-        self.lock.waitlock()    #(self.lckname)
+        if self.verbose > 1:
+            print("findrecpos", strx)
+
+        self.lock.waitlock()
         chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
         arr = []
         if type(strx) != type(b""):
-            strx = strx.encode(errors='strict');
+            strx = strx.encode(errors='strict')
 
         for aa in range(chash - self.INTSIZE * 2, HEADSIZE  - self.INTSIZE * 2, -self.INTSIZE * 2):
             rec = self.getidxint(aa)
             sig = self.getbuffstr(rec, self.INTSIZE)
             if sig == RECDEL:
-                if base_showdel:
+                if self.showdel:
                     print(" Deleted record '%s' at" % sig, rec)
             elif sig != RECSIG:
-                if self.base_verbose > 0:
+                if self.verbose > 0:
                     print(" Damaged data '%s' at" % sig, rec)
             else:
                 blen = self.getbuffint(rec+8)
                 data = self.getbuffstr(rec + 12, blen)
-                if self.base_verbose > 1:
+                if self.verbose > 1:
                     print("frecpos", data)
                 if strx == data:
-                    arr.append(rec)
+                    arr.append((aa - HEADSIZE) //  (self.INTSIZE * 2) )
                     if len(arr) >= limx:
                         break
-
-        self.lock.unlock()  #dellock(self.lckname)
-
+        self.lock.unlock()
         return arr
 
-    def  findrec(self, strx, limx = INT_MAX, skipx = 0):
+    def  findrecoffs(self, strx, limx = INT_MAX, skipx = 0):
 
-        ''' Find by string matching substring. '''
+        ''' Find record by matching substring.
+            Return array of offsets.
+        '''
 
-        self.lock.waitlock()    #(self.lckname)
+        self.lock.waitlock()
         chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
         arr = []
         if type(strx) != type(b""):
-            strx2 = strx.encode(errors='strict');
+            strx2 = strx.encode(errors='strict')
 
         #print("findrec", strx2)
 
         #for aa in range(HEADSIZE + self.INTSIZE * 2, chash, self.INTSIZE * 2):
         for aa in range(chash - self.INTSIZE * 2, HEADSIZE  - self.INTSIZE * 2, -self.INTSIZE * 2):
             rec = self.getidxint(aa)
             sig = self.getbuffstr(rec, self.INTSIZE)
             if sig == RECDEL:
-                if base_showdel:
+                if self.showdel:
                     print(" Deleted record '%s' at" % sig, rec)
             elif sig != RECSIG:
-                if self.base_verbose > 0:
+                if self.verbose > 0:
                     print(" Damaged data '%s' at" % sig, rec)
             else:
                 blen = self.getbuffint(rec+8)
                 data = self.getbuffstr(rec + 12, blen)
-                if self.base_verbose > 1:
+                if self.verbose > 1:
                     print("find", data)
                 #if str(strx2) in str(data):
                 if strx2 in data:
                     #arr.append(self.get_key_offs(rec))
-                    #arr.append(rec)
-                    arr.append(self._rec2arr(rec))
+                    arr.append(rec)
                     if len(arr) >= limx:
                         break
-        self.lock.unlock()    #dellock(self.lckname)
-
+        self.lock.unlock()
         return arr
 
-    # --------------------------------------------------------------------
+        # --------------------------------------------------------------------
     # List all active records
 
     def  listall(self):
 
         ''' List all active records. Return array id record indexes. '''
 
-        self.lock.waitlock()    #(self.lckname)
+        self.lock.waitlock()
         keys = []; arr = []; cnt = 0
 
         chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
         maxrec = chash - self.INTSIZE * 2
         rsize = self._getdbsize(self.ifp) - 1
 
         rrr =  range(maxrec,
@@ -1124,39 +1150,42 @@
         for aa in rrr:
             rec = self.getidxint(aa)
 
             #print(" Scanning at %d %d" % (rec, cnt))
 
             sig = self.getbuffstr(rec, self.INTSIZE)
             if sig == RECDEL:
-                if 1: #base_showdel:
+                if 1: #self.showdel:
                     print("Deleted record '%s' at" % sig, rec)
             elif sig != RECSIG:
-                if 1: #self.base_verbose > 0:
+                if 1: #self.verbose > 0:
                     print(" Damaged data '%s' at" % sig, rec)
             else:
-                    hhh = self.getbuffint(rec+4)
-                    print(" Good data '%s' at" % sig, rec, hhh)
-                    if hhh not in keys:
-                        keys.append(hhh)
-                        # as we are going backwards
-                        arr.append(rsize - cnt)
-                        #print("found", hhh)
+                hhh = self.getbuffint(rec+4)
+                print(" Good data '%s' at" % sig, rec, hhh)
+                if hhh not in keys:
+                    keys.append(hhh)
+                    # as we are going backwards
+                    arr.append(rsize - cnt)
+                    #print("found", hhh)
             cnt += 1
 
         keys = []
-        self.lock.unlock()  #dellock()self.lckname)
+        self.lock.unlock()
 
         return arr
 
     def  find_key(self, keyx, limx = 0xffffffff):
 
-        ''' Find record by key Search from the end, so latest comes first. '''
+        ''' Find record by key value.
+            Search from the end, so latest comes first.
+            This operates on the hash, so it reaches the answer fast.
+        '''
 
-        self.lock.waitlock()   #self.lckname)
+        self.lock.waitlock()
 
         skip = 0; arr = []; cnt = 0
         try:
             arg2e = keyx.encode()
         except:
             arg2e = keyx
 
@@ -1168,35 +1197,38 @@
                 HEADSIZE - self.INTSIZE * 2, -self.INTSIZE * 2)
         for aa in rrr:
             rec = self.getidxint(aa)
             #print(" Scanning at %d %d" % (rec, cnt))
 
             sig = self.getbuffstr(rec, self.INTSIZE)
             if sig == RECDEL:
-                if base_showdel:
+                if self.showdel:
                     print("Deleted record '%s' at" % sig, rec)
             elif sig != RECSIG:
-                if self.base_verbose > 0:
+                if self.verbose > 0:
                     print(" Damaged data '%s' at" % sig, rec)
             else:
                 hhh = self.getbuffint(rec+4)
                 if hhh == hhhh:
                     if len(arr) >= limx - 1:
                         arr.append(["More data ...",])
                         break
                     arr.append(rec)
                 else:
                     pass
                     #print("no match", hex(hhh))
 
             cnt += 1
-        self.lock.unlock()  #dellock()self.lckname)
+        self.lock.unlock()
 
         return arr
 
+    def idx2offs(self, idx):
+        offs = self.getidxint(HEADSIZE + idx * self.INTSIZE * 2)
+        return offs
 
     def  del_data(self, hash, skip = 1):
 
         ''' Delete data by hash. '''
 
         cnt = skip
         hhhh = int(hash, 16)                #;print("hash", hash, hhhh)
@@ -1213,15 +1245,15 @@
             #    print(" Damaged data '%s' at" % sig, rec)
 
             #blen = self.getbuffint(rec+8)
             #print("data '%s' at" % sig, rec, "blen", blen)
 
             hhh = self.getbuffint(rec+4)
             if hash == hhh:
-                if self.base_verbose > 0:
+                if self.verbose > 0:
                     print("Would delete", hhh)
 
             self.putbuffstr(rec, RECDEL)
 
             cnt += 1
 
         return arr
@@ -1246,15 +1278,15 @@
         ''' Delete records by key string; needs bin str, converted
             automatically on entry.
         '''
 
         if type(strx) != type(b""):
             strx = strx.encode()
 
-        if self.base_verbose > 1:
+        if self.verbose > 1:
             print("Start delete ", strx, "skip", skip)
 
         cnt = 0; cnt3 = 0
         #chash = self.getidxint(CURROFFS)    #;print("chash", chash)
         chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
 
         # Direction sensitivity
@@ -1264,58 +1296,62 @@
             rrr = range(chash - self.INTSIZE * 2, HEADSIZE  - self.INTSIZE * 2, -self.INTSIZE * 2)
 
         #for aa in range(HEADSIZE, chash, self.INTSIZE * 2):
         for aa in rrr:
             rec = self.getidxint(aa)
             sig = self.getbuffstr(rec, self.INTSIZE)
             if sig == RECDEL:
-                if base_showdel:
+                if self.showdel:
                     print(" Deleted record '%s' at" % sig, rec)
             elif sig != RECSIG:
-                if self.base_verbose > 0:
+                if self.verbose > 0:
                     print(" Damaged data '%s' at" % sig, rec)
             else:
                 blen = self.getbuffint(rec+8)
                 data = self.getbuffstr(rec + 12, blen)
-                if self.base_verbose > 2:
+                if self.verbose > 2:
                     print("del iterate recs", cnt3, data, strx)
 
                 if strx == data:
-                    if self.base_verbose > 0:
+                    if self.verbose > 0:
                         print("Deleting", cnt3, aa, data)
                     self.putbuffstr(rec, RECDEL)
                     cnt += 1
                     if cnt >= maxdelrec:
                         break
             cnt3 += 1
         return cnt
 
     def  save_data(self, header, datax, replace = False):
 
         ''' Append to the end of file. If replace flag is set, try to overwrite
-            in place. If new record is larger, add it as ususal. If smaller,
+            in place. If new record is larger, add it as usual. If smaller,
             the record is padded with spaces. This should not influence most ops.
             (like: int())
             This feature allows the database update wthout creating new records.
-            Useful for counters or dynamically changing data.
+            Useful for counters or dynamically changing data. To be useful,
+            use  / create fixed size data. Like: "%12d" % (var).
 
                     Input:
                         header     Header
                         datax      Data
 
                      Return:
                         The offset of saved data
             '''
 
         if self.pgdebug > 0:
             print("Save_data()", header, datax)
 
-        self.lock.waitlock()   #self.lckname)
-        ret = 0
-        was = False
+        self.lock.waitlock()
+
+        if self.preexec:
+            self.preexec(self, header)
+
+        ret = 0 ; was = False
         # Put new data in place
         if replace:
             if type(datax) != type(b""):
                 mrep2 = datax.encode()
             else:
                 mrep2 = datax
 
@@ -1330,17 +1366,21 @@
                     ccc = self.hash32(padded)
                     self.putbuffint(rrr[1] - 8, ccc)
                     #print("ccc", hex(ccc))
                     self.putbuffstr(rrr[1], padded)
                     was = True
                     ret =  rrr[0]
         if not was:
+            #print("Saving longer data", header, datax)
             ret = self._save_data2(header, datax)
 
-        self.lock.unlock()  #dellock()self.lckname)
+        if self.postexec:
+            self.postexec(self, header)
+
+        self.lock.unlock()
 
         return ret
 
     # --------------------------------------------------------------------
     # Save data to database file
 
     def  _save_data2(self, arg2, arg3):
@@ -1362,15 +1402,15 @@
 
         ret = self.__save_data(hhh2, arg2, hhh3, arg3)
 
         return ret
 
     def __save_data(self, hhh2, arg2e, hhh3, arg3e):
 
-        # Update / Append data
+        ''' Update / Append data. Note the doyuble underscore '''
 
         # Building array added some efficiency
         arr = []
         arr.append(RECSIG)
         arr.append(struct.pack("I", hhh2))
         arr.append(struct.pack("I", len(arg2e)))
         arr.append(arg2e)
@@ -1405,36 +1445,36 @@
         self.putidxint(curr, dcurr)
         self.putidxint(curr + self.INTSIZE, hhh2)
         #self.putidxint(CURROFFS, self.ifp.tell())
 
         self.fp.flush()
         self.ifp.flush()
 
-        return curr
+        return dcurr
 
     def __del__(self):
 
         ''' flush file handles and close files. '''
 
         if hasattr(self, "pgdebug"):
             if self.pgdebug > 9:
                 print("__del__ called.")
 
         #self.flush()
 
         if hasattr(self, "fp"):
-                if self.fp:
-                    if not self.fp.closed:
-                        self.fp.flush()
-                        self.fp.close()
+            if self.fp:
+                if not self.fp.closed:
+                    self.fp.flush()
+                    self.fp.close()
 
         if hasattr(self, "ifp"):
-                if self.ifp:
-                    if not self.ifp.closed:
-                        self.ifp.flush()
-                        self.ifp.close()
+            if self.ifp:
+                if not self.ifp.closed:
+                    self.ifp.flush()
+                    self.ifp.close()
 
         # remove lockfile
         if hasattr(self, "lock"):
-            self.lock.unlock()    #dellock(self.lckname)
+            self.lock.unlock()
 
 # EOF
```

### Comparing `pydbase-1.5.2/pydbase.egg-info/PKG-INFO` & `pydbase-1.7.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: pydbase
-Version: 1.5.2
-Summary: High speed database with key / data in python.
-Home-page: https://github.com/pglen/pydbase
-Author: Peter Glen
-Author-email: peterglen99@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-
 # pydbase
 
 ## High speed database with key / data
 
 #### see: blockchain functions at the end
 
  &nbsp; The motivation was to create a no frills way of saving / retrieving data.
@@ -347,9 +334,11 @@
     1.4.5       Fri 01.Mar.2024     Misc fixes
     1.4.6       Mon 04.Mar.2024     Vacuum count on vacuumed records
     1.4.7       Tue 05.Mar.2024     In place record update
     1.4.8       Sat 09.Mar.2024     Added new locking mechanism
     1.4.9       Mon 01.Apr.2024     Updated to run on MSYS2, new locking
     1.5.0       Tue 02.Apr.2024     Cleaned, pip upload
     1.5.1       Wed 10.Apr.2024     Dangling lock .. fixed
+    1.6.0       Thu 25.Apr.2024     Added IDX pre and post callbacks
+    1.6.1       Mon 29.Apr.2024     D: option corrected
 
 // EOF
```

### Comparing `pydbase-1.5.2/pydbase.egg-info/SOURCES.txt` & `pydbase-1.7.1/pydbase.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 pydbase.egg-info/top_level.txt
 pydbase/docs/twinbase.html
 pydbase/docs/twinchain.html
 pydbase/docs/twincore.html
 tests/test_acreate.py
 tests/test_bigdata.py
 tests/test_bindata.py
+tests/test_callback.py
 tests/test_chain.py
 tests/test_chain_data.py
 tests/test_chain_link.py
 tests/test_del.py
 tests/test_dump.py
 tests/test_find.py
 tests/test_findrec.py
```

### Comparing `pydbase-1.5.2/setup.py` & `pydbase-1.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,21 +15,20 @@
           'Intended Audience :: System Administrators',
           'License :: OSI Approved :: Python Software Foundation License',
           'Operating System :: Microsoft :: Windows',
           'Operating System :: POSIX',
           'Programming Language :: Python',
           'Topic :: Databases',
         ]
-
 # Get version number  from the server support file:
 fp = open("pydbase/twinbase.py", "rt")
 vvv = fp.read(); fp.close()
 loc_vers =  '1.0.0'     # Default
 for aa in vvv.split("\n"):
-    idx = aa.find("version =")
+    idx = aa.find("VERSION =")
     if idx == 0:        # At the beginning of line
         try:
             loc_vers = aa.split()[2].replace('"', "")
             break
         except:
             pass
 #print("loc_vers:", loc_vers)
```

### Comparing `pydbase-1.5.2/tests/test_acreate.py` & `pydbase-1.7.1/tests/test_acreate.py`

 * *Files identical despite different names*

### Comparing `pydbase-1.5.2/tests/test_bigdata.py` & `pydbase-1.7.1/tests/test_bigdata.py`

 * *Files identical despite different names*

### Comparing `pydbase-1.5.2/tests/test_bindata.py` & `pydbase-1.7.1/tests/test_bindata.py`

 * *Files identical despite different names*

### Comparing `pydbase-1.5.2/tests/test_chain.py` & `pydbase-1.7.1/tests/test_chain.py`

 * *Files identical despite different names*

### Comparing `pydbase-1.5.2/tests/test_chain_data.py` & `pydbase-1.7.1/tests/test_chain_data.py`

 * *Files identical despite different names*

### Comparing `pydbase-1.5.2/tests/test_chain_link.py` & `pydbase-1.7.1/tests/test_chain_link.py`

 * *Files identical despite different names*

### Comparing `pydbase-1.5.2/tests/test_del.py` & `pydbase-1.7.1/tests/test_del.py`

 * *Files identical despite different names*

### Comparing `pydbase-1.5.2/tests/test_dump.py` & `pydbase-1.7.1/tests/test_dump.py`

 * *Files identical despite different names*

### Comparing `pydbase-1.5.2/tests/test_find.py` & `pydbase-1.7.1/tests/test_find.py`

 * *Files 10% similar despite different names*

```diff
@@ -47,16 +47,16 @@
 
 def test_search():
 
     #return
 
     strx = "1111"
     ret = core.findrec(strx, 1)
-    #print(ret)
+    #print("ret", ret)
     assert ret ==[[b'11111', b'22222']]
 
     strx = "11111"
-    ret = core.findrec(strx, 1)
-    #print(ret)
+    ret2 = core.findrec(strx, 1)
+    #print("ret2", ret2)
     assert ret == [[b'11111', b'22222']]
 
 # EOF
```

### Comparing `pydbase-1.5.2/tests/test_findrec.py` & `pydbase-1.7.1/tests/test_findrec.py`

 * *Files identical despite different names*

### Comparing `pydbase-1.5.2/tests/test_getoffs.py` & `pydbase-1.7.1/tests/test_list.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,16 +14,22 @@
     core = create_db(fname)
     assert core != 0
 
     ret = core.save_data("1111", "2222")
     assert ret != 0
     ret = core.save_data("11111", "22222")
     assert ret != 0
+    ret = core.save_data("11111", "333333")
+    assert ret != 0
+    ret = core.save_data("3333", "4444")
+    assert ret != 0
     ret = core.save_data("111", "222")
     assert ret != 0
+    ret = core.save_data("1111", "3333")
+    assert ret != 0
 
 def teardown_module(module):
     """ teardown any state that was previously setup with a setup_module
     method.
     """
     uncreate_db()
 
@@ -36,28 +42,28 @@
     #assert 0, "test here, function %s" % function.__name__
     pass
 
 # ------------------------------------------------------------------------
 # Start
 
 def test_get():
-
-    # Get record, verify
-    ret = core.get_rec(2)
-    assert ret != 0
+    ret = core.get_rec(4)
     assert ret == [b'111', b'222']
 
-def test_getoffs():
+def test_list():
 
-    ret = core.findrecpos('1111', 1)
-    assert ret == [32]
-    ddd = core.get_rec_byoffs(ret[0])
-    assert ddd == [b'1111', b'2222']
-
-def test_getoffs2():
-
-    ret = core.findrecpos('11111', 1)
-    assert ret == [64]
-    ddd = core.get_rec_byoffs(ret[0])
-    assert ddd == [b'11111', b'22222']
+    ret = core.del_rec_bykey("3333")
+    #print("delrec", ret)
+    assert ret == 1
+
+    ret = core.listall()
+    #print("listall", ret)
+    assert ret == [5, 4, 2]
+
+    sss = []
+    for aa in ret:
+        ret = core.get_rec(aa)
+        sss.append(ret)
+    #print(sss)
+    assert sss == [[b'1111', b'3333'], [b'111', b'222'], [b'11111', b'333333']]
 
 # EOF
```

### Comparing `pydbase-1.5.2/tests/test_getrec.py` & `pydbase-1.7.1/tests/test_getrec.py`

 * *Files identical despite different names*

### Comparing `pydbase-1.5.2/tests/test_handles.py` & `pydbase-1.7.1/tests/test_handles.py`

 * *Files identical despite different names*

### Comparing `pydbase-1.5.2/tests/test_inplace.py` & `pydbase-1.7.1/tests/test_inplace.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,8 +62,31 @@
     #print(ret2)
     assert ret2 == [[b'11111', b'333  ']]
 
     ret3 = core.get_rec(1)
     #print(ret3)
     assert ret3 == [b'11111', b'333  ']
 
+def test_bigger():
+
+    org = core.findrecpos("11111", 1)
+    #print("org", org)
+
+    # This is in place, but longer
+    ret = core.save_data("11111", "444444", True)
+    #print("save bigger data", ret)
+    assert ret != org
+
+    ret4 = core.get_rec_byoffs(ret)
+    #print("get _rec_byoffs", ret4)
+    assert ret4 == [b'11111', b'444444']
+
+    ret5 = core.save_data("11111", "555555", True)
+    assert ret == ret5
+
+    ret6 = core.get_rec_byoffs(ret5)
+    assert ret6 == [b'11111', b'555555']
+
+    #core.dump_data()
+    #assert 0
+
 # EOF
```

### Comparing `pydbase-1.5.2/tests/test_integrity.py` & `pydbase-1.7.1/tests/test_integrity.py`

 * *Files identical despite different names*

### Comparing `pydbase-1.5.2/tests/test_list.py` & `pydbase-1.7.1/tests/test_getoffs.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,22 +14,19 @@
     core = create_db(fname)
     assert core != 0
 
     ret = core.save_data("1111", "2222")
     assert ret != 0
     ret = core.save_data("11111", "22222")
     assert ret != 0
-    ret = core.save_data("11111", "333333")
-    assert ret != 0
-    ret = core.save_data("3333", "4444")
+    # This is the record that will be found
+    ret = core.save_data("111111", "222222")
     assert ret != 0
     ret = core.save_data("111", "222")
     assert ret != 0
-    ret = core.save_data("1111", "3333")
-    assert ret != 0
 
 def teardown_module(module):
     """ teardown any state that was previously setup with a setup_module
     method.
     """
     uncreate_db()
 
@@ -42,28 +39,42 @@
     #assert 0, "test here, function %s" % function.__name__
     pass
 
 # ------------------------------------------------------------------------
 # Start
 
 def test_get():
-    ret = core.get_rec(4)
-    assert ret == [b'111', b'222']
-
-def test_list():
 
-    ret = core.del_rec_bykey("3333")
-    #print("delrec", ret)
-    assert ret == 1
-
-    ret = core.listall()
-    #print("listall", ret)
-    assert ret == [5, 4, 2]
-
-    sss = []
-    for aa in ret:
-        ret = core.get_rec(aa)
-        sss.append(ret)
-    #print(sss)
-    assert sss == [[b'1111', b'3333'], [b'111', b'222'], [b'11111', b'333333']]
+    # Get record, verify
+    ret = core.get_rec(0)
+    assert ret == [b'1111', b'2222']
+    assert ret
+
+    ret = core.get_rec(1)
+    assert ret
+    assert ret == [b'11111', b'22222']
+
+    # Provoke exception
+    err = 0
+    try:
+        ret = core.get_rec(100)
+    except:
+        err = 1
+    assert err == 1
+
+def test_getoffs():
+
+    ret = core.findrecoffs('111', 1)
+    #print("ret:", ret)
+    assert ret == [134]
+    ddd = core.get_rec_byoffs(ret[0])
+    assert ddd ==[b'111', b'222']
+
+def test_getoffs2():
+
+    ret2 = core.findrecoffs('11111', 1)
+    #print("ret2:", ret2)
+    assert ret2 == [98]
+    ddd = core.get_rec_byoffs(ret2[0])
+    assert ddd ==[b'111111', b'222222']
 
 # EOF
```

### Comparing `pydbase-1.5.2/tests/test_lockrel.py` & `pydbase-1.7.1/tests/test_lockrel.py`

 * *Files identical despite different names*

### Comparing `pydbase-1.5.2/tests/test_multi.py` & `pydbase-1.7.1/tests/test_multi.py`

 * *Files identical despite different names*

### Comparing `pydbase-1.5.2/tests/test_packer.py` & `pydbase-1.7.1/tests/test_packer.py`

 * *Files identical despite different names*

### Comparing `pydbase-1.5.2/tests/test_reindex.py` & `pydbase-1.7.1/tests/test_reindex.py`

 * *Files identical despite different names*

### Comparing `pydbase-1.5.2/tests/test_search.py` & `pydbase-1.7.1/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `pydbase-1.5.2/tests/test_vacuum.py` & `pydbase-1.7.1/tests/test_vacuum.py`

 * *Files identical despite different names*

