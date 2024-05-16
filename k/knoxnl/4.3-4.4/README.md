# Comparing `tmp/knoxnl-4.3.tar.gz` & `tmp/knoxnl-4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knoxnl-4.3.tar", last modified: Wed May  1 22:07:14 2024, max compression
+gzip compressed data, was "knoxnl-4.4.tar", last modified: Thu May  2 12:54:21 2024, max compression
```

## Comparing `knoxnl-4.3.tar` & `knoxnl-4.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-05-01 22:07:14.014052 knoxnl-4.3/
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)     1068 2024-03-12 20:07:00.000000 knoxnl-4.3/LICENSE
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)    19058 2024-05-01 22:07:14.003862 knoxnl-4.3/PKG-INFO
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)    18636 2024-05-01 17:17:52.000000 knoxnl-4.3/README.md
-drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-05-01 22:07:13.572540 knoxnl-4.3/knoxnl/
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)       17 2024-05-01 17:17:56.000000 knoxnl-4.3/knoxnl/__init__.py
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)    55612 2024-05-01 22:06:26.000000 knoxnl-4.3/knoxnl/knoxnl.py
-drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-05-01 22:07:13.986807 knoxnl-4.3/knoxnl.egg-info/
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)    19058 2024-05-01 22:07:12.000000 knoxnl-4.3/knoxnl.egg-info/PKG-INFO
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)      273 2024-05-01 22:07:13.000000 knoxnl-4.3/knoxnl.egg-info/SOURCES.txt
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)        1 2024-05-01 22:07:12.000000 knoxnl-4.3/knoxnl.egg-info/dependency_links.txt
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)       46 2024-05-01 22:07:12.000000 knoxnl-4.3/knoxnl.egg-info/entry_points.txt
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)        1 2024-03-15 11:47:02.000000 knoxnl-4.3/knoxnl.egg-info/not-zip-safe
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)       60 2024-05-01 22:07:13.000000 knoxnl-4.3/knoxnl.egg-info/requires.txt
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)        7 2024-05-01 22:07:13.000000 knoxnl-4.3/knoxnl.egg-info/top_level.txt
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)       38 2024-05-01 22:07:14.024739 knoxnl-4.3/setup.cfg
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)     2365 2024-05-01 17:17:54.000000 knoxnl-4.3/setup.py
+drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-05-02 12:54:21.310217 knoxnl-4.4/
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)     1068 2024-03-12 20:07:00.000000 knoxnl-4.4/LICENSE
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)    19058 2024-05-02 12:54:21.296822 knoxnl-4.4/PKG-INFO
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)    18636 2024-05-02 12:53:04.000000 knoxnl-4.4/README.md
+drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-05-02 12:54:21.018870 knoxnl-4.4/knoxnl/
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)       17 2024-05-02 12:52:57.000000 knoxnl-4.4/knoxnl/__init__.py
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)    55582 2024-05-02 12:52:39.000000 knoxnl-4.4/knoxnl/knoxnl.py
+drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-05-02 12:54:21.275371 knoxnl-4.4/knoxnl.egg-info/
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)    19058 2024-05-02 12:54:20.000000 knoxnl-4.4/knoxnl.egg-info/PKG-INFO
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)      273 2024-05-02 12:54:20.000000 knoxnl-4.4/knoxnl.egg-info/SOURCES.txt
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)        1 2024-05-02 12:54:20.000000 knoxnl-4.4/knoxnl.egg-info/dependency_links.txt
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)       46 2024-05-02 12:54:20.000000 knoxnl-4.4/knoxnl.egg-info/entry_points.txt
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)        1 2024-03-15 11:47:02.000000 knoxnl-4.4/knoxnl.egg-info/not-zip-safe
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)       60 2024-05-02 12:54:20.000000 knoxnl-4.4/knoxnl.egg-info/requires.txt
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)        7 2024-05-02 12:54:20.000000 knoxnl-4.4/knoxnl.egg-info/top_level.txt
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)       38 2024-05-02 12:54:21.314090 knoxnl-4.4/setup.cfg
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)     2365 2024-05-01 17:17:54.000000 knoxnl-4.4/setup.py
```

### Comparing `knoxnl-4.3/LICENSE` & `knoxnl-4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `knoxnl-4.3/PKG-INFO` & `knoxnl-4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: knoxnl
-Version: 4.3
+Version: 4.4
 Summary: A python wrapper around the amazing KNOXSS API by Brute Logic (requires an API Key)
 Home-page: https://github.com/xnl-h4ck3r/knoxnl
 Author: @xnl-h4ck3r
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: argparse
 Requires-Dist: requests
 Requires-Dist: termcolor
 Requires-Dist: pyaml
 Requires-Dist: urlparse3
 Requires-Dist: python-dateutil
 
 <center><img src="https://github.com/xnl-h4ck3r/knoxnl/blob/main/knoxnl/images/title.png"></center>
 
-## About - v4.3
+## About - v4.4
 
 This is a python wrapper around the amazing [KNOXSS API](https://knoxss.me/?page_id=2729) by Brute Logic.
 To use this tool (and the underlying API), you must have a valid KNOXSS API key. Don't have one? Go visit https://knoxss.me and subscribe!
 This was inspired by the ["knoxssme" tool](https://github.com/edoardottt/lit-bb-hack-tools/tree/main/knoxssme) by @edoardottt2, but developed to allow for greater options.
 
 **DISCLAIMER: We are not responsible for any use, and especially misuse, of this tool or the KNOXSS API**
```

### Comparing `knoxnl-4.3/README.md` & `knoxnl-4.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <center><img src="https://github.com/xnl-h4ck3r/knoxnl/blob/main/knoxnl/images/title.png"></center>
 
-## About - v4.3
+## About - v4.4
 
 This is a python wrapper around the amazing [KNOXSS API](https://knoxss.me/?page_id=2729) by Brute Logic.
 To use this tool (and the underlying API), you must have a valid KNOXSS API key. Don't have one? Go visit https://knoxss.me and subscribe!
 This was inspired by the ["knoxssme" tool](https://github.com/edoardottt/lit-bb-hack-tools/tree/main/knoxssme) by @edoardottt2, but developed to allow for greater options.
 
 **DISCLAIMER: We are not responsible for any use, and especially misuse, of this tool or the KNOXSS API**
```

### Comparing `knoxnl-4.3/knoxnl/knoxnl.py` & `knoxnl-4.4/knoxnl/knoxnl.py`

 * *Files 0% similar despite different names*

```diff
@@ -451,15 +451,15 @@
                                 knoxssResponse.Calls = 'Unknown'
                             knoxssResponse.Error = str(jsonResponse['Error'])
                             
                             # If service unavailable flag to stop
                             if knoxssResponse.Error == 'service unavailable':
                                 needToRetry = True
                             # If the API rate limit is exceeded, flag to stop
-                            elif latestApiCalls == '22/5000': #knoxssResponse.Error == 'API rate limit exceeded.':
+                            elif knoxssResponse.Error == 'API rate limit exceeded.':
                                 rateLimitExceeded = True
                                 knoxssResponse.Calls = 'API rate limit exceeded!'
                                 # Flag to stop if we aren't going to wait until the API limit is reset
                                 if not (timeAPIReset is not None and args.pause_until_reset):
                                     needToStop = True
                             else: # remove the URL from the int input set
                                 inputValues.discard(targetUrl)
```

### Comparing `knoxnl-4.3/knoxnl.egg-info/PKG-INFO` & `knoxnl-4.4/knoxnl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: knoxnl
-Version: 4.3
+Version: 4.4
 Summary: A python wrapper around the amazing KNOXSS API by Brute Logic (requires an API Key)
 Home-page: https://github.com/xnl-h4ck3r/knoxnl
 Author: @xnl-h4ck3r
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: argparse
 Requires-Dist: requests
 Requires-Dist: termcolor
 Requires-Dist: pyaml
 Requires-Dist: urlparse3
 Requires-Dist: python-dateutil
 
 <center><img src="https://github.com/xnl-h4ck3r/knoxnl/blob/main/knoxnl/images/title.png"></center>
 
-## About - v4.3
+## About - v4.4
 
 This is a python wrapper around the amazing [KNOXSS API](https://knoxss.me/?page_id=2729) by Brute Logic.
 To use this tool (and the underlying API), you must have a valid KNOXSS API key. Don't have one? Go visit https://knoxss.me and subscribe!
 This was inspired by the ["knoxssme" tool](https://github.com/edoardottt/lit-bb-hack-tools/tree/main/knoxssme) by @edoardottt2, but developed to allow for greater options.
 
 **DISCLAIMER: We are not responsible for any use, and especially misuse, of this tool or the KNOXSS API**
```

### Comparing `knoxnl-4.3/setup.py` & `knoxnl-4.4/setup.py`

 * *Files identical despite different names*

