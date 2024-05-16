# Comparing `tmp/bdownload-0.2.0.tar.gz` & `tmp/bdownload-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdownload-0.2.0.tar", last modified: Sun May  5 06:08:57 2024, max compression
+gzip compressed data, was "bdownload-0.2.1.tar", last modified: Thu May 16 10:45:03 2024, max compression
```

## Comparing `bdownload-0.2.0.tar` & `bdownload-0.2.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 06:08:57.835804 bdownload-0.2.0/
--rw-rw-rw-   0        0        0     1035 2024-03-08 08:14:53.000000 bdownload-0.2.0/.readthedocs.yaml
--rw-rw-rw-   0        0        0      745 2024-05-03 15:37:49.000000 bdownload-0.2.0/.travis.yml
--rw-rw-rw-   0        0        0      178 2024-03-15 02:56:16.000000 bdownload-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0    23632 2024-05-05 06:08:57.835804 bdownload-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    21568 2024-05-05 03:35:24.000000 bdownload-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-05 06:08:57.801825 bdownload-0.2.0/docs/
--rw-rw-rw-   0        0        0      584 2021-11-10 14:24:48.000000 bdownload-0.2.0/docs/Makefile
--rwxrwxrwx   0        0        0      756 2021-11-10 14:24:48.000000 bdownload-0.2.0/docs/make.bat
-drwxrwxrwx   0        0        0        0 2024-05-05 06:08:57.811050 bdownload-0.2.0/docs/source/
--rw-rw-rw-   0        0        0      449 2024-03-15 02:56:16.000000 bdownload-0.2.0/docs/source/bdownload.rst
--rw-rw-rw-   0        0        0      231 2022-02-23 10:08:54.000000 bdownload-0.2.0/docs/source/cli.rst
--rw-rw-rw-   0        0        0     6494 2024-03-08 06:08:09.000000 bdownload-0.2.0/docs/source/conf.py
--rw-rw-rw-   0        0        0     8440 2024-04-24 14:26:25.000000 bdownload-0.2.0/docs/source/index.rst
--rw-rw-rw-   0        0        0      314 2024-03-08 08:14:53.000000 bdownload-0.2.0/docs/source/requirements.txt
--rw-rw-rw-   0        0        0      267 2022-02-23 10:23:42.000000 bdownload-0.2.0/docs/source/test_bdownloader.rst
--rw-rw-rw-   0        0        0      359 2022-02-23 10:23:42.000000 bdownload-0.2.0/docs/source/test_multisource_download.rst
--rw-rw-rw-   0        0        0       80 2024-05-03 15:37:49.000000 bdownload-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0      470 2024-05-05 06:00:39.000000 bdownload-0.2.0/requirements.txt
--rw-rw-rw-   0        0        0       90 2024-05-05 06:08:57.837803 bdownload-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     2806 2024-05-03 15:37:49.000000 bdownload-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-05 06:08:57.760147 bdownload-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-05 06:08:57.820907 bdownload-0.2.0/src/bdownload/
--rw-rw-rw-   0        0        0        5 2024-05-05 03:35:24.000000 bdownload-0.2.0/src/bdownload/VERSION
--rw-rw-rw-   0        0        0      364 2022-03-05 07:28:46.000000 bdownload-0.2.0/src/bdownload/__init__.py
--rw-rw-rw-   0        0        0      351 2024-03-15 02:56:16.000000 bdownload-0.2.0/src/bdownload/__main__.py
--rw-rw-rw-   0        0        0    21262 2024-04-17 05:19:12.000000 bdownload-0.2.0/src/bdownload/cli.py
--rw-rw-rw-   0        0        0   101868 2024-05-03 15:37:49.000000 bdownload-0.2.0/src/bdownload/download.py
--rw-rw-rw-   0        0        0     6157 2024-03-15 02:56:16.000000 bdownload-0.2.0/src/bdownload/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-05 06:08:57.827802 bdownload-0.2.0/tests/
--rw-rw-rw-   0        0        0        0 2021-11-10 14:24:48.000000 bdownload-0.2.0/tests/__init__.py
--rw-rw-rw-   0        0        0     4248 2021-11-19 11:24:44.000000 bdownload-0.2.0/tests/test_bdownloader.py
--rw-rw-rw-   0        0        0     1521 2024-03-17 06:34:08.000000 bdownload-0.2.0/tests/test_cli.py
--rw-rw-rw-   0        0        0     3331 2024-03-17 10:05:27.000000 bdownload-0.2.0/tests/test_multisource_download.py
-drwxrwxrwx   0        0        0        0 2024-05-05 06:08:57.762658 bdownload-0.2.0/third_parties/
-drwxrwxrwx   0        0        0        0 2024-05-05 06:08:57.830672 bdownload-0.2.0/third_parties/setupext_janitor/
--rw-rw-rw-   0        0        0     5228 2021-11-10 14:24:48.000000 bdownload-0.2.0/third_parties/setupext_janitor/README.rst
--rw-rw-rw-   0        0        0     7272 2021-11-10 14:24:48.000000 bdownload-0.2.0/third_parties/setupext_janitor/janitor.py
--rw-rw-rw-   0        0        0      171 2024-05-03 15:37:49.000000 bdownload-0.2.0/tox.ini
+drwxrwxrwx   0        0        0        0 2024-05-16 10:45:03.200066 bdownload-0.2.1/
+-rw-rw-rw-   0        0        0     1035 2024-03-08 08:14:53.000000 bdownload-0.2.1/.readthedocs.yaml
+-rw-rw-rw-   0        0        0      745 2024-05-03 15:37:49.000000 bdownload-0.2.1/.travis.yml
+-rw-rw-rw-   0        0        0      178 2024-03-15 02:56:16.000000 bdownload-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    23658 2024-05-16 10:45:03.199052 bdownload-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0    21594 2024-05-07 10:24:09.000000 bdownload-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 10:45:03.162032 bdownload-0.2.1/docs/
+-rw-rw-rw-   0        0        0      584 2021-11-10 14:24:48.000000 bdownload-0.2.1/docs/Makefile
+-rwxrwxrwx   0        0        0      756 2021-11-10 14:24:48.000000 bdownload-0.2.1/docs/make.bat
+drwxrwxrwx   0        0        0        0 2024-05-16 10:45:03.172884 bdownload-0.2.1/docs/source/
+-rw-rw-rw-   0        0        0      449 2024-03-15 02:56:16.000000 bdownload-0.2.1/docs/source/bdownload.rst
+-rw-rw-rw-   0        0        0      231 2022-02-23 10:08:54.000000 bdownload-0.2.1/docs/source/cli.rst
+-rw-rw-rw-   0        0        0     6494 2024-03-08 06:08:09.000000 bdownload-0.2.1/docs/source/conf.py
+-rw-rw-rw-   0        0        0     8440 2024-04-24 14:26:25.000000 bdownload-0.2.1/docs/source/index.rst
+-rw-rw-rw-   0        0        0      314 2024-03-08 08:14:53.000000 bdownload-0.2.1/docs/source/requirements.txt
+-rw-rw-rw-   0        0        0      267 2022-02-23 10:23:42.000000 bdownload-0.2.1/docs/source/test_bdownloader.rst
+-rw-rw-rw-   0        0        0      359 2022-02-23 10:23:42.000000 bdownload-0.2.1/docs/source/test_multisource_download.rst
+-rw-rw-rw-   0        0        0       80 2024-05-03 15:37:49.000000 bdownload-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0      573 2024-05-07 03:10:43.000000 bdownload-0.2.1/requirements.txt
+-rw-rw-rw-   0        0        0       90 2024-05-16 10:45:03.201344 bdownload-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     2806 2024-05-03 15:37:49.000000 bdownload-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 10:45:03.117026 bdownload-0.2.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-16 10:45:03.184665 bdownload-0.2.1/src/bdownload/
+-rw-rw-rw-   0        0        0        5 2024-05-16 10:42:12.000000 bdownload-0.2.1/src/bdownload/VERSION
+-rw-rw-rw-   0        0        0      364 2022-03-05 07:28:46.000000 bdownload-0.2.1/src/bdownload/__init__.py
+-rw-rw-rw-   0        0        0      351 2024-03-15 02:56:16.000000 bdownload-0.2.1/src/bdownload/__main__.py
+-rw-rw-rw-   0        0        0    21262 2024-04-17 05:19:12.000000 bdownload-0.2.1/src/bdownload/cli.py
+-rw-rw-rw-   0        0        0   103068 2024-05-16 10:42:12.000000 bdownload-0.2.1/src/bdownload/download.py
+-rw-rw-rw-   0        0        0     6157 2024-03-15 02:56:16.000000 bdownload-0.2.1/src/bdownload/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-16 10:45:03.191275 bdownload-0.2.1/tests/
+-rw-rw-rw-   0        0        0        0 2021-11-10 14:24:48.000000 bdownload-0.2.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     4248 2021-11-19 11:24:44.000000 bdownload-0.2.1/tests/test_bdownloader.py
+-rw-rw-rw-   0        0        0     1521 2024-03-17 06:34:08.000000 bdownload-0.2.1/tests/test_cli.py
+-rw-rw-rw-   0        0        0     3331 2024-03-17 10:05:27.000000 bdownload-0.2.1/tests/test_multisource_download.py
+drwxrwxrwx   0        0        0        0 2024-05-16 10:45:03.121363 bdownload-0.2.1/third_parties/
+drwxrwxrwx   0        0        0        0 2024-05-16 10:45:03.195684 bdownload-0.2.1/third_parties/setupext_janitor/
+-rw-rw-rw-   0        0        0     5228 2021-11-10 14:24:48.000000 bdownload-0.2.1/third_parties/setupext_janitor/README.rst
+-rw-rw-rw-   0        0        0     7272 2021-11-10 14:24:48.000000 bdownload-0.2.1/third_parties/setupext_janitor/janitor.py
+-rw-rw-rw-   0        0        0      171 2024-05-03 15:37:49.000000 bdownload-0.2.1/tox.ini
```

### Comparing `bdownload-0.2.0/.readthedocs.yaml` & `bdownload-0.2.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `bdownload-0.2.0/.travis.yml` & `bdownload-0.2.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `bdownload-0.2.0/PKG-INFO` & `bdownload-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdownload
-Version: 0.2.0
+Version: 0.2.1
 Summary: A multi-threaded and multi-source aria2-like batch file downloading library for Python
 Home-page: https://github.com/Jesseatgao/bdownload
 Author: Jesse Gao
 Author-email: changxigao@gmail.com
 License: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
@@ -32,15 +32,15 @@
 Requires-Dist: clint
 Requires-Dist: futures; python_version == "2.7"
 Requires-Dist: certifi==2021.10.8; python_version == "2.7"
 Requires-Dist: setuptools; python_version >= "3.12"
 
 ## bdownload
 [![Latest Version](https://img.shields.io/pypi/v/bdownload.svg)](https://pypi.org/project/bdownload/)
-[![Build Status](https://travis-ci.com/Jesseatgao/bdownload.svg?branch=master)](https://travis-ci.com/Jesseatgao/bdownload)
+[![Build Status](https://api.travis-ci.com/Jesseatgao/bdownload.svg?branch=master)](https://api.travis-ci.com/Jesseatgao/bdownload.svg?branch=master)
 [![Supported Versions](https://img.shields.io/pypi/pyversions/bdownload.svg)](https://pypi.org/project/bdownload)
 
 A multi-threaded and multi-source aria2-like batch file downloading library for Python 2.7 and 3.6+
 
 > **:bulb:** **Note**\
 > See also [https://bdownload.readthedocs.io](https://bdownload.readthedocs.io) for API reference.
```

### Comparing `bdownload-0.2.0/README.md` & `bdownload-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ## bdownload
 [![Latest Version](https://img.shields.io/pypi/v/bdownload.svg)](https://pypi.org/project/bdownload/)
-[![Build Status](https://travis-ci.com/Jesseatgao/bdownload.svg?branch=master)](https://travis-ci.com/Jesseatgao/bdownload)
+[![Build Status](https://api.travis-ci.com/Jesseatgao/bdownload.svg?branch=master)](https://api.travis-ci.com/Jesseatgao/bdownload.svg?branch=master)
 [![Supported Versions](https://img.shields.io/pypi/pyversions/bdownload.svg)](https://pypi.org/project/bdownload)
 
 A multi-threaded and multi-source aria2-like batch file downloading library for Python 2.7 and 3.6+
 
 > **:bulb:** **Note**\
 > See also [https://bdownload.readthedocs.io](https://bdownload.readthedocs.io) for API reference.
```

### Comparing `bdownload-0.2.0/docs/Makefile` & `bdownload-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bdownload-0.2.0/docs/make.bat` & `bdownload-0.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `bdownload-0.2.0/docs/source/conf.py` & `bdownload-0.2.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `bdownload-0.2.0/docs/source/index.rst` & `bdownload-0.2.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `bdownload-0.2.0/setup.py` & `bdownload-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `bdownload-0.2.0/src/bdownload/cli.py` & `bdownload-0.2.1/src/bdownload/cli.py`

 * *Files identical despite different names*

### Comparing `bdownload-0.2.0/src/bdownload/download.py` & `bdownload-0.2.1/src/bdownload/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,38 +17,31 @@
 
 # Extracted from `futures`
 try:
     from multiprocessing import cpu_count
 except ImportError:
     # some platforms don't have multiprocessing
     def cpu_count():
-        return None
+        return 0
 
 try:
     from urllib.parse import unquote, urlparse
 
     unichr = chr
 except ImportError:
     from urllib import unquote
     from urlparse import urlparse
 
 try:
     import cPickle as pickle
 except ImportError:
     import pickle
 
-try:
-    distutils
-except NameError:
-    # On Python 3.12 and beyond
-    from setuptools import distutils
-finally:
-    from distutils.dir_util import mkpath, remove_tree
-    from distutils.errors import DistutilsFileError
-
+from distutils.dir_util import mkpath, remove_tree
+from distutils.errors import DistutilsFileError
 import requests
 from requests.adapters import HTTPAdapter
 from requests.packages.urllib3.util.retry import Retry
 from requests import Session
 from requests.auth import AuthBase, HTTPBasicAuth, HTTPDigestAuth, extract_cookies_to_jar
 from requests.cookies import cookielib, RequestsCookieJar
 from clint.textui import progress as clint_progress
@@ -79,15 +72,15 @@
 #: float: Default retry backoff factor.
 RETRY_BACKOFF_FACTOR = 0.1
 
 #: set: Default status codes to retry on intended for the underlying ``urllib3``.
 URLLIB3_RETRY_STATUS_CODES = frozenset([413, 429, 500, 502, 503, 504])
 
 #: set: Default status codes that should be avoided retrying on before handled
-RETRY_EXEMPT_STATUS_CODES = frozenset([401, 407])
+RETRY_EXEMPT_STATUS_CODES = frozenset([401, 407, 511])
 
 COOKIE_STR_REGEX = re.compile(r'^\s*(?:[^,; =]+=[^,; ]+\s*(?:$|\s+|;\s*))+\s*$')
 """regex: A compiled regular expression object used to match the cookie string in the form of key/value pairs.
 
 See also :meth:`BDownloader.__init__()` for more details about `cookies`.
 """
 
@@ -115,20 +108,20 @@
 PICKLE_PROTOCOL_NUMBER = 2
 
 
 def _cpu_count():
     """A simple wrapper around the ``cpu_count()`` for escaping the `NotImplementedError`.
 
     Returns:
-        The number of CPUs in the system. Return `None` if not obtained.
+        int: The number of CPUs in the system. Return ``0`` if not obtained.
     """
     try:
         cpus = cpu_count()
     except NotImplementedError:
-        cpus = None
+        cpus = 0
 
     return cpus
 
 
 def set_requests_retries_factor(retries):
     """Set the retries factor for the decorator :func:`retry_requests`.
 
@@ -623,14 +616,16 @@
     """The class for executing and managing download jobs.
 
     The context of the current downloading job is structured as::
 
         ctx = {
             "total_size": 2000,  # total size of all the to-be-downloaded files, maybe inaccurate due to chunked transfer encoding
             "accurate": True,  # Is `total_size` accurate?
+            "last_progress": 0,  # the overall progress, in bytes, from last run loaded when resuming from interruption
+            "downloaded": 0,  # newly accumulated bytes from this run of downloads, which are updated on completion of every worker thread
             "orig_path_urls": [('file1', 'url1\turl2\turl3'), ('file2', 'url4\turl5\turl6')],  # originally added downloads,
                 # which don't necessarily correspond to `files` e.g. due to duplicate or interruption
             "file_cnt": 2,  # number of current downloading files
             "alt_files": [("full_path_to_file1", `ctx_file1_obj`), ("full_path_to_file2", `ctx_file2_obj`)],  # flattened `files`
             "active_files": [("full_path_to_file1", `ctx_file1_obj`)],  # scheduled, in-processing file downloads
             "active_downloads": 1,  # number of in-processing file downloads
             "next_download": 1,  # index to the next to schedule to download file
@@ -855,16 +850,17 @@
         self.all_submitted = False
         self.sigint = False  # Received the SIGINT (i.e. `KeyboardInterrupt`) signal, e.g. raised by hitting `Ctrl-C`?
         self.cmdquit = False  # Received the QUIT command, e.g. triggered by pressing `q`?
         # Flag indicating that cancellation of all the tasks have been done on demand, e.g. by pressing `Ctrl-C` or `q`
         self.cancelled_on_interrupt = False
         self.stop = False  # Flag signaling waiting threads to exit
         # The download context that maintains the status of the downloading files and the corresponding chunks
-        self._dl_ctx = {'total_size': 0, 'accurate': True, 'orig_path_urls': [], 'file_cnt': 0, 'files': {},
-                        'alt_files': [], 'active_files': [], 'next_download': 0, 'active_downloads': 0, 'poll_changed': False}
+        self._dl_ctx = {'total_size': 0, 'accurate': True, 'last_progress': 0, 'downloaded': 0, 'orig_path_urls': [],
+                        'file_cnt': 0, 'files': {}, 'alt_files': [], 'active_files': [], 'next_download': 0,
+                        'active_downloads': 0, 'poll_changed': False}
 
         # list: A downloadable subset of all the `(path, url)`\ s that were passed to :meth:`BDownloader.download` or
         # :meth:`BDownloader.downloads`.
         self.active_downloads_added = []
         # list: The non-downloadable `(path, url)`\ s that were filtered out before downloading actually begins.
         # Together with :attr:`BDownloader.active_downloads_added`, they form the whole of the input downloads.
         self.failed_downloads_on_addition = []
@@ -1564,14 +1560,15 @@
 
             ctx_file['alt_ranges'] = [(req_range, ctx_range) for req_range, ctx_range in ctx_file['ranges'].items()]
             ctx_file['alt_ranges'].reverse()  # To pop from the range stack and download from the beginning of the file
 
             # make the file visible to the world
             self._dl_ctx['alt_files'].append((file_path_name, ctx_file))
             self._dl_ctx['file_cnt'] += 1
+            self._dl_ctx['last_progress'] += ctx_file['last_progress']
 
         return downloadable, path_url, orig_path_url
 
     def _build_ctx(self, path_urls):
         """Build the context for downloading the file(s).
 
         Args:
@@ -1819,14 +1816,15 @@
             ranges_have_dones = False
 
             for _, ctx_range in ctx_file['worker_ranges']:
                 future = ctx_range['future']
                 if future.done():
                     ranges_have_dones = True
                     ctx_file['downloaded'] += ctx_range['offset']
+                    self._dl_ctx['downloaded'] += ctx_range['offset']
 
                     try:
                         exception = future.exception()
                         if exception is None:
                             ctx_range['download_state'] = self.SUCCEEDED
                             ctx_file['ranges_succeeded'] += 1
                             ctx_file['progress'] += ctx_range['offset']
@@ -1929,14 +1927,26 @@
         else:
             progress_bar.last_progress = self._dl_ctx['total_size'] \
                 if self._dl_ctx['accurate'] and not (self.failed_downloads_in_running or self.sigint or self.cmdquit) \
                 else self._calc_completed()
             progress_bar.expected_size = self._dl_ctx['total_size']
             progress_bar.done()
 
+    def progress_all(self):
+        """Get the coarse-grained, overall progress of the downloads.
+
+        Returns:
+            tuple: The 3-tuple of the form ``(completed_bytes, total_bytes, is_accurate)``. ``completed_bytes`` is updated
+            on a chunk basis from the worker threads by the management task. If ``is_accurate`` is `False` then ``total_bytes``
+            is inaccurate, i.e. some downloads have undetermined sizes, which also means ``completed_bytes`` may be greater
+            than the ``total_bytes``; otherwise, ``total_bytes`` is the exact sum of sizes of all the downloads. Note that
+            ``total_bytes`` (and ``is_accurate``) may vary during the phase of submitting the downloads.
+        """
+        return self._dl_ctx['last_progress'] + self._dl_ctx['downloaded'], self._dl_ctx['total_size'], self._dl_ctx['accurate']
+
     def downloads(self, path_urls):
         """Submit multiple downloading jobs at a time to the downloading queue.
 
         Args:
             path_urls (:obj:`list` of :obj:`tuple`\ s): `path_urls` accepts a list of tuples of the form ``(path, url)``,
                 where ``path`` should be a pathname, optionally prefixed with absolute or relative paths, and ``url`` should
                 be a URL string, which may consist of multiple TAB-separated URLs pointing to the same file.
```

### Comparing `bdownload-0.2.0/src/bdownload/utils.py` & `bdownload-0.2.1/src/bdownload/utils.py`

 * *Files identical despite different names*

### Comparing `bdownload-0.2.0/tests/test_bdownloader.py` & `bdownload-0.2.1/tests/test_bdownloader.py`

 * *Files identical despite different names*

### Comparing `bdownload-0.2.0/tests/test_cli.py` & `bdownload-0.2.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `bdownload-0.2.0/tests/test_multisource_download.py` & `bdownload-0.2.1/tests/test_multisource_download.py`

 * *Files identical despite different names*

### Comparing `bdownload-0.2.0/third_parties/setupext_janitor/README.rst` & `bdownload-0.2.1/third_parties/setupext_janitor/README.rst`

 * *Files identical despite different names*

### Comparing `bdownload-0.2.0/third_parties/setupext_janitor/janitor.py` & `bdownload-0.2.1/third_parties/setupext_janitor/janitor.py`

 * *Files identical despite different names*

