# Comparing `tmp/PKDevTools-0.13.20240512.115.tar.gz` & `tmp/PKDevTools-0.13.20240516.118.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PKDevTools-0.13.20240512.115.tar", last modified: Sun May 12 14:04:46 2024, max compression
+gzip compressed data, was "PKDevTools-0.13.20240516.118.tar", last modified: Thu May 16 18:14:21 2024, max compression
```

## Comparing `PKDevTools-0.13.20240512.115.tar` & `PKDevTools-0.13.20240516.118.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 14:04:46.035980 PKDevTools-0.13.20240512.115/
--rw-rw-rw-   0        0        0     1086 2024-05-12 14:02:42.000000 PKDevTools-0.13.20240512.115/LICENSE
-drwxrwxrwx   0        0        0        0 2024-05-12 14:04:46.020322 PKDevTools-0.13.20240512.115/PKDevTools/
--rw-rw-rw-   0        0        0     1176 2024-05-12 14:02:42.000000 PKDevTools-0.13.20240512.115/PKDevTools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 14:04:46.035980 PKDevTools-0.13.20240512.115/PKDevTools/classes/
--rw-rw-rw-   0        0        0     3402 2024-05-12 14:02:42.000000 PKDevTools-0.13.20240512.115/PKDevTools/classes/Archiver.py
--rw-rw-rw-   0        0        0     5178 2024-05-12 14:02:42.000000 PKDevTools-0.13.20240512.115/PKDevTools/classes/ColorText.py
--rw-rw-rw-   0        0        0     3599 2024-05-12 14:02:42.000000 PKDevTools-0.13.20240512.115/PKDevTools/classes/Committer.py
--rw-rw-rw-   0        0        0     6376 2024-05-12 14:02:42.000000 PKDevTools-0.13.20240512.115/PKDevTools/classes/CookieHelper.py
--rw-rw-rw-   0        0        0     8879 2024-05-12 14:02:42.000000 PKDevTools-0.13.20240512.115/PKDevTools/classes/Fetcher.py
--rw-rw-rw-   0        0        0     2514 2024-05-12 14:02:42.000000 PKDevTools-0.13.20240512.115/PKDevTools/classes/FunctionTimeouts.py
--rw-rw-rw-   0        0        0    11963 2024-05-12 14:02:42.000000 PKDevTools-0.13.20240512.115/PKDevTools/classes/MenuOptions.py
--rw-rw-rw-   0        0        0     2860 2024-05-12 14:02:42.000000 PKDevTools-0.13.20240512.115/PKDevTools/classes/OutputControls.py
--rw-rw-rw-   0        0        0    14576 2024-05-12 14:02:42.000000 PKDevTools-0.13.20240512.115/PKDevTools/classes/PKDateUtilities.py
--rw-rw-rw-   0        0        0     2988 2024-05-12 14:02:42.000000 PKDevTools-0.13.20240512.115/PKDevTools/classes/PKGitFolderDownloader.py
--rw-rw-rw-   0        0        0     5081 2024-05-12 14:02:42.000000 PKDevTools-0.13.20240512.115/PKDevTools/classes/PKJoinableQueue.py
--rw-rw-rw-   0        0        0    10868 2024-05-12 14:02:42.000000 PKDevTools-0.13.20240512.115/PKDevTools/classes/PKMultiProcessorClient.py
--rw-rw-rw-   0        0        0    14334 2024-05-12 14:02:42.000000 PKDevTools-0.13.20240512.115/PKDevTools/classes/PKPickler.py
--rw-rw-rw-   0        0        0     3433 2024-05-12 14:02:42.000000 PKDevTools-0.13.20240512.115/PKDevTools/classes/PKTimer.py
--rw-rw-rw-   0        0        0     4548 2024-05-12 14:02:42.000000 PKDevTools-0.13.20240512.115/PKDevTools/classes/Singleton.py
--rw-rw-rw-   0        0        0     2004 2024-05-12 14:02:42.000000 PKDevTools-0.13.20240512.115/PKDevTools/classes/SuppressOutput.py
--rw-rw-rw-   0        0        0    11301 2024-05-12 14:02:42.000000 PKDevTools-0.13.20240512.115/PKDevTools/classes/Telegram.py
--rw-rw-rw-   0        0        0    24543 2024-05-12 14:02:42.000000 PKDevTools-0.13.20240512.115/PKDevTools/classes/Utils.py
--rw-rw-rw-   0        0        0     9984 2024-05-12 14:02:42.000000 PKDevTools-0.13.20240512.115/PKDevTools/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-12 14:04:41.000000 PKDevTools-0.13.20240512.115/PKDevTools/classes/__init__.py
--rw-rw-rw-   0        0        0     3738 2024-05-12 14:02:42.000000 PKDevTools-0.13.20240512.115/PKDevTools/classes/githubutilities.py
--rw-rw-rw-   0        0        0    16136 2024-05-12 14:02:42.000000 PKDevTools-0.13.20240512.115/PKDevTools/classes/log.py
--rw-rw-rw-   0        0        0     7430 2024-05-12 14:02:42.000000 PKDevTools-0.13.20240512.115/PKDevTools/classes/multiprocessing_logging.py
--rw-rw-rw-   0        0        0     2864 2024-05-12 14:02:42.000000 PKDevTools-0.13.20240512.115/PKDevTools/classes/squash.py
--rw-rw-rw-   0        0        0     4846 2024-05-12 14:02:42.000000 PKDevTools-0.13.20240512.115/PKDevTools/classes/updater.py
-drwxrwxrwx   0        0        0        0 2024-05-12 14:04:46.020322 PKDevTools-0.13.20240512.115/PKDevTools.egg-info/
--rw-rw-rw-   0        0        0     5204 2024-05-12 14:04:45.000000 PKDevTools-0.13.20240512.115/PKDevTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1161 2024-05-12 14:04:45.000000 PKDevTools-0.13.20240512.115/PKDevTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 14:04:45.000000 PKDevTools-0.13.20240512.115/PKDevTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      363 2024-05-12 14:04:45.000000 PKDevTools-0.13.20240512.115/PKDevTools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-12 14:04:39.000000 PKDevTools-0.13.20240512.115/PKDevTools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      176 2024-05-12 14:04:45.000000 PKDevTools-0.13.20240512.115/PKDevTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-12 14:04:45.000000 PKDevTools-0.13.20240512.115/PKDevTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5204 2024-05-12 14:04:46.035980 PKDevTools-0.13.20240512.115/PKG-INFO
--rw-rw-rw-   0        0        0     4290 2024-05-12 14:02:42.000000 PKDevTools-0.13.20240512.115/README.md
--rw-rw-rw-   0        0        0       86 2024-05-12 14:04:46.035980 PKDevTools-0.13.20240512.115/setup.cfg
--rw-rw-rw-   0        0        0     4341 2024-05-12 14:02:42.000000 PKDevTools-0.13.20240512.115/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 18:14:21.070618 PKDevTools-0.13.20240516.118/
+-rw-rw-rw-   0        0        0     1086 2024-05-16 18:11:39.000000 PKDevTools-0.13.20240516.118/LICENSE
+drwxrwxrwx   0        0        0        0 2024-05-16 18:14:21.054991 PKDevTools-0.13.20240516.118/PKDevTools/
+-rw-rw-rw-   0        0        0     1176 2024-05-16 18:11:39.000000 PKDevTools-0.13.20240516.118/PKDevTools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 18:14:21.070618 PKDevTools-0.13.20240516.118/PKDevTools/classes/
+-rw-rw-rw-   0        0        0     4960 2024-05-16 18:11:39.000000 PKDevTools-0.13.20240516.118/PKDevTools/classes/Archiver.py
+-rw-rw-rw-   0        0        0     5178 2024-05-16 18:11:39.000000 PKDevTools-0.13.20240516.118/PKDevTools/classes/ColorText.py
+-rw-rw-rw-   0        0        0     3599 2024-05-16 18:11:39.000000 PKDevTools-0.13.20240516.118/PKDevTools/classes/Committer.py
+-rw-rw-rw-   0        0        0     6376 2024-05-16 18:11:39.000000 PKDevTools-0.13.20240516.118/PKDevTools/classes/CookieHelper.py
+-rw-rw-rw-   0        0        0     8879 2024-05-16 18:11:39.000000 PKDevTools-0.13.20240516.118/PKDevTools/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     2577 2024-05-16 18:11:39.000000 PKDevTools-0.13.20240516.118/PKDevTools/classes/FunctionTimeouts.py
+-rw-rw-rw-   0        0        0    11963 2024-05-16 18:11:39.000000 PKDevTools-0.13.20240516.118/PKDevTools/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0     2860 2024-05-16 18:11:39.000000 PKDevTools-0.13.20240516.118/PKDevTools/classes/OutputControls.py
+-rw-rw-rw-   0        0        0    14576 2024-05-16 18:11:39.000000 PKDevTools-0.13.20240516.118/PKDevTools/classes/PKDateUtilities.py
+-rw-rw-rw-   0        0        0     2988 2024-05-16 18:11:39.000000 PKDevTools-0.13.20240516.118/PKDevTools/classes/PKGitFolderDownloader.py
+-rw-rw-rw-   0        0        0     5081 2024-05-16 18:11:39.000000 PKDevTools-0.13.20240516.118/PKDevTools/classes/PKJoinableQueue.py
+-rw-rw-rw-   0        0        0    11018 2024-05-16 18:11:39.000000 PKDevTools-0.13.20240516.118/PKDevTools/classes/PKMultiProcessorClient.py
+-rw-rw-rw-   0        0        0    14334 2024-05-16 18:11:39.000000 PKDevTools-0.13.20240516.118/PKDevTools/classes/PKPickler.py
+-rw-rw-rw-   0        0        0     3433 2024-05-16 18:11:39.000000 PKDevTools-0.13.20240516.118/PKDevTools/classes/PKTimer.py
+-rw-rw-rw-   0        0        0     4548 2024-05-16 18:11:39.000000 PKDevTools-0.13.20240516.118/PKDevTools/classes/Singleton.py
+-rw-rw-rw-   0        0        0     2004 2024-05-16 18:11:39.000000 PKDevTools-0.13.20240516.118/PKDevTools/classes/SuppressOutput.py
+-rw-rw-rw-   0        0        0    11301 2024-05-16 18:11:39.000000 PKDevTools-0.13.20240516.118/PKDevTools/classes/Telegram.py
+-rw-rw-rw-   0        0        0    24543 2024-05-16 18:11:39.000000 PKDevTools-0.13.20240516.118/PKDevTools/classes/Utils.py
+-rw-rw-rw-   0        0        0     9984 2024-05-16 18:11:39.000000 PKDevTools-0.13.20240516.118/PKDevTools/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-16 18:14:15.000000 PKDevTools-0.13.20240516.118/PKDevTools/classes/__init__.py
+-rw-rw-rw-   0        0        0     3738 2024-05-16 18:11:39.000000 PKDevTools-0.13.20240516.118/PKDevTools/classes/githubutilities.py
+-rw-rw-rw-   0        0        0    16136 2024-05-16 18:11:39.000000 PKDevTools-0.13.20240516.118/PKDevTools/classes/log.py
+-rw-rw-rw-   0        0        0     7430 2024-05-16 18:11:39.000000 PKDevTools-0.13.20240516.118/PKDevTools/classes/multiprocessing_logging.py
+-rw-rw-rw-   0        0        0     2864 2024-05-16 18:11:39.000000 PKDevTools-0.13.20240516.118/PKDevTools/classes/squash.py
+-rw-rw-rw-   0        0        0     4846 2024-05-16 18:11:39.000000 PKDevTools-0.13.20240516.118/PKDevTools/classes/updater.py
+drwxrwxrwx   0        0        0        0 2024-05-16 18:14:21.054991 PKDevTools-0.13.20240516.118/PKDevTools.egg-info/
+-rw-rw-rw-   0        0        0     5204 2024-05-16 18:14:21.000000 PKDevTools-0.13.20240516.118/PKDevTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1161 2024-05-16 18:14:21.000000 PKDevTools-0.13.20240516.118/PKDevTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 18:14:21.000000 PKDevTools-0.13.20240516.118/PKDevTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      363 2024-05-16 18:14:21.000000 PKDevTools-0.13.20240516.118/PKDevTools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-16 18:14:12.000000 PKDevTools-0.13.20240516.118/PKDevTools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      176 2024-05-16 18:14:21.000000 PKDevTools-0.13.20240516.118/PKDevTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-16 18:14:21.000000 PKDevTools-0.13.20240516.118/PKDevTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5204 2024-05-16 18:14:21.070618 PKDevTools-0.13.20240516.118/PKG-INFO
+-rw-rw-rw-   0        0        0     4290 2024-05-16 18:11:39.000000 PKDevTools-0.13.20240516.118/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-16 18:14:21.070618 PKDevTools-0.13.20240516.118/setup.cfg
+-rw-rw-rw-   0        0        0     4341 2024-05-16 18:11:39.000000 PKDevTools-0.13.20240516.118/setup.py
```

### Comparing `PKDevTools-0.13.20240512.115/LICENSE` & `PKDevTools-0.13.20240516.118/LICENSE`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240512.115/PKDevTools/__init__.py` & `PKDevTools-0.13.20240516.118/PKDevTools/__init__.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240512.115/PKDevTools/classes/Archiver.py` & `PKDevTools-0.13.20240516.118/PKDevTools/classes/Archiver.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,18 +18,20 @@
     FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
     AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
     LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
     OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
     SOFTWARE.
 
 """
+import glob
 import os
 import os.path
 import tempfile
 import warnings
+from PKDevTools.classes.log import default_logger
 from datetime import datetime, timezone
 
 warnings.simplefilter("ignore", DeprecationWarning)
 warnings.simplefilter("ignore", FutureWarning)
 import pandas as pd
 import pytz
 
@@ -40,33 +42,45 @@
     filePath = os.path.join(dirPath, fileName)
     safe_open_w(filePath)
     return filePath
 
 
 def get_last_modified_datetime(file_path):
     from PKDevTools.classes.PKDateUtilities import PKDateUtilities
-    last_modified = datetime.utcfromtimestamp(os.path.getmtime(file_path))
-    return PKDateUtilities.utc_to_ist(last_modified)
+    last_modified = datetime.fromtimestamp(os.path.getmtime(file_path),tz=pytz.timezone("Asia/Kolkata"))
+    return last_modified
 
 
 def cacheFile(bData, fileName):
     filePath = resolveFilePath(fileName)
     with open(filePath, "wb") as f:
         f.write(bData)
 
 
 def findFile(fileName):
     filePath = resolveFilePath(fileName)
     try:
+        exists = os.path.exists(filePath)
         with open(filePath, "rb") as f:
             bData = f.read()
-        return bData, filePath, get_last_modified_datetime(filePath)
+        return bData, filePath, get_last_modified_datetime(filePath) if exists else None
     except Exception:
         return None, filePath, None
 
+def findFileInAppResultsDirectory(fileName):
+    filePath = os.path.join(get_user_outputs_dir(),fileName)
+    exists = os.path.exists(filePath)
+    data = None
+    try:
+        if exists:
+            with open(filePath, "r") as f:
+                data = f.read()
+        return data, filePath, get_last_modified_datetime(filePath) if exists else None
+    except Exception:
+        return None, filePath, None
 
 def saveData(data, fileName):
     if not len(data) > 0 or fileName == "" or fileName is None:
         return
     filePath = resolveFilePath(fileName)
     try:
         data.to_pickle(filePath)
@@ -93,8 +107,32 @@
     """Open "path" for writing, creating any parent directories as needed."""
     os.makedirs(os.path.dirname(path), exist_ok=True)
     # return open(path, 'wb')
 
 def get_user_outputs_dir():
     # Let's make the results directory where we'll push all outputs
     os.makedirs(os.path.dirname(os.path.join(os.getcwd(),f"results{os.sep}")), exist_ok=True)
-    return os.path.join(os.getcwd(),"results")
+    return os.path.join(os.getcwd(),"results")
+
+def deleteFileWithPattern(pattern=None, excludeFile=None, rootDir=None, recursive=False):
+    if pattern is None:
+        return
+    if rootDir is None:
+        rootDir = [get_user_outputs_dir(),get_user_outputs_dir().replace("results","actions-data-download")]
+    else:
+        rootDir = [rootDir]
+    for dir in rootDir:
+        files = glob.glob(pattern, root_dir=dir, recursive=recursive)
+        for f in files:
+            if excludeFile is not None:
+                if not f.endswith(excludeFile):
+                    try:
+                        os.remove(f if os.sep in f else os.path.join(dir,f))
+                    except Exception as e:
+                        default_logger().debug(e, exc_info=True)
+                        pass
+            else:
+                try:
+                    os.remove(f if os.sep in f else os.path.join(dir,f))
+                except Exception as e:
+                    default_logger().debug(e, exc_info=True)
+                    pass
```

### Comparing `PKDevTools-0.13.20240512.115/PKDevTools/classes/ColorText.py` & `PKDevTools-0.13.20240516.118/PKDevTools/classes/ColorText.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240512.115/PKDevTools/classes/Committer.py` & `PKDevTools-0.13.20240516.118/PKDevTools/classes/Committer.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240512.115/PKDevTools/classes/CookieHelper.py` & `PKDevTools-0.13.20240516.118/PKDevTools/classes/CookieHelper.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240512.115/PKDevTools/classes/Fetcher.py` & `PKDevTools-0.13.20240516.118/PKDevTools/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240512.115/PKDevTools/classes/FunctionTimeouts.py` & `PKDevTools-0.13.20240516.118/PKDevTools/classes/FunctionTimeouts.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 import threading
 from time import sleep
 try:
     import thread
 except ImportError:
     import _thread as thread
 
+INTERMEDIATE_NUM_SECONDS_WARN=30
+
 def cdquit(fn_name):
     # print to stderr, unbuffered in Python 2.
     print('{0} took too long. Handle KeyboardInterrupt if you do not want to exit'.format(fn_name), file=sys.stderr)
     sys.stderr.flush() # Python 3 stderr is likely buffered.
     thread.interrupt_main() # raises KeyboardInterrupt
 
 def intermediateMessage(fn_name):
@@ -49,15 +51,15 @@
     use as decorator to exit process if 
     function takes longer than s seconds
     '''
     def outer(fn):
         def inner(*args, **kwargs):
             timer = threading.Timer(s, cdquit, args=[fn.__name__])
             timer.start()
-            timer_mid = threading.Timer(10, intermediateMessage, args=[fn.__name__])
+            timer_mid = threading.Timer(INTERMEDIATE_NUM_SECONDS_WARN, intermediateMessage, args=[fn.__name__])
             timer_mid.start()
             try:
                 result = fn(*args, **kwargs)
             finally:
                 timer.cancel()
                 timer_mid.cancel()
             return result
```

### Comparing `PKDevTools-0.13.20240512.115/PKDevTools/classes/MenuOptions.py` & `PKDevTools-0.13.20240516.118/PKDevTools/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240512.115/PKDevTools/classes/OutputControls.py` & `PKDevTools-0.13.20240516.118/PKDevTools/classes/OutputControls.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240512.115/PKDevTools/classes/PKDateUtilities.py` & `PKDevTools-0.13.20240516.118/PKDevTools/classes/PKDateUtilities.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240512.115/PKDevTools/classes/PKGitFolderDownloader.py` & `PKDevTools-0.13.20240516.118/PKDevTools/classes/PKGitFolderDownloader.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240512.115/PKDevTools/classes/PKJoinableQueue.py` & `PKDevTools-0.13.20240516.118/PKDevTools/classes/PKJoinableQueue.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240512.115/PKDevTools/classes/PKMultiProcessorClient.py` & `PKDevTools-0.13.20240516.118/PKDevTools/classes/PKMultiProcessorClient.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,16 +138,16 @@
         logger.addHandler(handler)
 
         # On Windows, the level will not be inherited.  Also, we could just
         # set the level to log everything here and filter it in the main
         # process handlers.  For now, just set it from the global default.
         logger.setLevel(self.logLevel)
         self.default_logger = logger
-        if self.default_logger is not None:
-            self.default_logger.info("PKMultiProcessorClient initialized.")
+        # if self.default_logger is not None:
+        #     self.default_logger.info("PKMultiProcessorClient initialized.")
 
     def _reloadDatabase(self):
         if self.refreshDatabase and self.dbFileNamePrimary is not None:
             # Looks like we got the filename instead of stock dictionary
             # Let's load the saved stocks' data
             cache_file_primary = self.dbFileNamePrimary
             try:
@@ -188,14 +188,17 @@
                         if next_task is not None:
                             # Inject a reference to this instance of the client
                             # so that the task can still get access back to it.
                             next_task = (*(next_task), self)
                 except Empty as e:
                     self.default_logger.debug(e, exc_info=True)
                     continue
+                except KeyboardInterrupt as e:
+                    self.default_logger.debug(e, exc_info=True)
+                    sys.exit(0)
                 if next_task is None:
                     self.default_logger.info("No next task in queue")
                     if self.task_queue is not None:
                         self.task_queue.task_done()
                     break
                 if self.processorMethod is not None:
                     answer = self.processorMethod(*(next_task))
```

### Comparing `PKDevTools-0.13.20240512.115/PKDevTools/classes/PKPickler.py` & `PKDevTools-0.13.20240516.118/PKDevTools/classes/PKPickler.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240512.115/PKDevTools/classes/PKTimer.py` & `PKDevTools-0.13.20240516.118/PKDevTools/classes/PKTimer.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240512.115/PKDevTools/classes/Singleton.py` & `PKDevTools-0.13.20240516.118/PKDevTools/classes/Singleton.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240512.115/PKDevTools/classes/SuppressOutput.py` & `PKDevTools-0.13.20240516.118/PKDevTools/classes/SuppressOutput.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240512.115/PKDevTools/classes/Telegram.py` & `PKDevTools-0.13.20240516.118/PKDevTools/classes/Telegram.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240512.115/PKDevTools/classes/Utils.py` & `PKDevTools-0.13.20240516.118/PKDevTools/classes/Utils.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240512.115/PKDevTools/classes/WorkflowManager.py` & `PKDevTools-0.13.20240516.118/PKDevTools/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240512.115/PKDevTools/classes/githubutilities.py` & `PKDevTools-0.13.20240516.118/PKDevTools/classes/githubutilities.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240512.115/PKDevTools/classes/log.py` & `PKDevTools-0.13.20240516.118/PKDevTools/classes/log.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240512.115/PKDevTools/classes/multiprocessing_logging.py` & `PKDevTools-0.13.20240516.118/PKDevTools/classes/multiprocessing_logging.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240512.115/PKDevTools/classes/squash.py` & `PKDevTools-0.13.20240516.118/PKDevTools/classes/squash.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240512.115/PKDevTools/classes/updater.py` & `PKDevTools-0.13.20240516.118/PKDevTools/classes/updater.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240512.115/PKDevTools.egg-info/PKG-INFO` & `PKDevTools-0.13.20240516.118/PKDevTools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKDevTools
-Version: 0.13.20240512.115
+Version: 0.13.20240516.118
 Summary: A general day-to-day toolset for repos
 Home-page: https://github.com/pkjmesra/PKDevTools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240512.115.zip
+Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240516.118.zip
 Keywords: GitHub tools,Logging,Telegram,Fetcher
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKDevTools-0.13.20240512.115/PKDevTools.egg-info/SOURCES.txt` & `PKDevTools-0.13.20240516.118/PKDevTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240512.115/PKG-INFO` & `PKDevTools-0.13.20240516.118/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKDevTools
-Version: 0.13.20240512.115
+Version: 0.13.20240516.118
 Summary: A general day-to-day toolset for repos
 Home-page: https://github.com/pkjmesra/PKDevTools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240512.115.zip
+Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240516.118.zip
 Keywords: GitHub tools,Logging,Telegram,Fetcher
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKDevTools-0.13.20240512.115/README.md` & `PKDevTools-0.13.20240516.118/README.md`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240512.115/setup.py` & `PKDevTools-0.13.20240516.118/setup.py`

 * *Files identical despite different names*

