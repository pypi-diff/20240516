# Comparing `tmp/qbitrr2-4.6.0.tar.gz` & `tmp/qbitrr2-4.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbitrr2-4.6.0.tar", last modified: Wed May  8 13:10:09 2024, max compression
+gzip compressed data, was "qbitrr2-4.6.1.tar", last modified: Thu May 16 09:50:00 2024, max compression
```

## Comparing `qbitrr2-4.6.0.tar` & `qbitrr2-4.6.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:10:09.584696 qbitrr2-4.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-08 13:10:05.000000 qbitrr2-4.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-05-08 13:10:09.584696 qbitrr2-4.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-05-08 13:10:05.000000 qbitrr2-4.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-08 13:10:05.000000 qbitrr2-4.6.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:10:09.580696 qbitrr2-4.6.0/qBitrr/
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-08 13:10:05.000000 qbitrr2-4.6.0/qBitrr/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)   226069 2024-05-08 13:10:05.000000 qbitrr2-4.6.0/qBitrr/arss.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-08 13:10:05.000000 qbitrr2-4.6.0/qBitrr/bundled_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-05-08 13:10:05.000000 qbitrr2-4.6.0/qBitrr/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-08 13:10:05.000000 qbitrr2-4.6.0/qBitrr/env_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-08 13:10:05.000000 qbitrr2-4.6.0/qBitrr/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-05-08 13:10:05.000000 qbitrr2-4.6.0/qBitrr/ffprobe.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    26629 2024-05-08 13:10:05.000000 qbitrr2-4.6.0/qBitrr/gen_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-08 13:10:05.000000 qbitrr2-4.6.0/qBitrr/home_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-05-08 13:10:05.000000 qbitrr2-4.6.0/qBitrr/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     8467 2024-05-08 13:10:05.000000 qbitrr2-4.6.0/qBitrr/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-08 13:10:05.000000 qbitrr2-4.6.0/qBitrr/tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-05-08 13:10:05.000000 qbitrr2-4.6.0/qBitrr/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:10:09.580696 qbitrr2-4.6.0/qBitrr2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-05-08 13:10:09.000000 qbitrr2-4.6.0/qBitrr2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-08 13:10:09.000000 qbitrr2-4.6.0/qBitrr2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 13:10:09.000000 qbitrr2-4.6.0/qBitrr2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-08 13:10:09.000000 qbitrr2-4.6.0/qBitrr2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-08 13:10:09.000000 qbitrr2-4.6.0/qBitrr2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-08 13:10:09.000000 qbitrr2-4.6.0/qBitrr2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-08 13:10:09.584696 qbitrr2-4.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 13:10:05.000000 qbitrr2-4.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:50:00.069096 qbitrr2-4.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-16 09:49:54.000000 qbitrr2-4.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-05-16 09:50:00.069096 qbitrr2-4.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-05-16 09:49:54.000000 qbitrr2-4.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-16 09:49:54.000000 qbitrr2-4.6.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:50:00.065096 qbitrr2-4.6.1/qBitrr/
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-16 09:49:54.000000 qbitrr2-4.6.1/qBitrr/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   226108 2024-05-16 09:49:54.000000 qbitrr2-4.6.1/qBitrr/arss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-16 09:49:54.000000 qbitrr2-4.6.1/qBitrr/bundled_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-05-16 09:49:54.000000 qbitrr2-4.6.1/qBitrr/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-16 09:49:54.000000 qbitrr2-4.6.1/qBitrr/env_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-16 09:49:54.000000 qbitrr2-4.6.1/qBitrr/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-05-16 09:49:54.000000 qbitrr2-4.6.1/qBitrr/ffprobe.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26629 2024-05-16 09:49:54.000000 qbitrr2-4.6.1/qBitrr/gen_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-16 09:49:54.000000 qbitrr2-4.6.1/qBitrr/home_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-05-16 09:49:54.000000 qbitrr2-4.6.1/qBitrr/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8467 2024-05-16 09:49:54.000000 qbitrr2-4.6.1/qBitrr/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-16 09:49:54.000000 qbitrr2-4.6.1/qBitrr/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-16 09:49:54.000000 qbitrr2-4.6.1/qBitrr/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:50:00.069096 qbitrr2-4.6.1/qBitrr2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-05-16 09:50:00.000000 qbitrr2-4.6.1/qBitrr2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-16 09:50:00.000000 qbitrr2-4.6.1/qBitrr2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 09:50:00.000000 qbitrr2-4.6.1/qBitrr2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-16 09:50:00.000000 qbitrr2-4.6.1/qBitrr2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-16 09:50:00.000000 qbitrr2-4.6.1/qBitrr2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-16 09:50:00.000000 qbitrr2-4.6.1/qBitrr2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-16 09:50:00.069096 qbitrr2-4.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 09:49:54.000000 qbitrr2-4.6.1/setup.py
```

### Comparing `qbitrr2-4.6.0/LICENSE` & `qbitrr2-4.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.0/PKG-INFO` & `qbitrr2-4.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qBitrr2
-Version: 4.6.0
+Version: 4.6.1
 Summary: "A simple Python script to talk to qBittorrent and Arr's"
 Home-page: https://github.com/Feramance/qBitrr
 Author: Feramance
 Author-email: fera@fera.wtf
 License: MIT
 Project-URL: Issue Tracker, https://github.com/Feramance/qBitrr/issues
 Project-URL: Source Code, https://github.com/Feramance/qBitrr
```

### Comparing `qbitrr2-4.6.0/README.md` & `qbitrr2-4.6.1/README.md`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.0/pyproject.toml` & `qbitrr2-4.6.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 [tool.black]
 line-length = 99
 target-version = ['py38']
 
 [tool.poetry]
 name = "pypi-public"
-version = "4.6.0"
+version = "4.6.1"
 description = "A simple script to monitor qBit and communicate with Radarr and Sonarr"
 authors = ["Drapersniper", "Feramance"]
 readme = "README.md"
 repository = "https://github.com/Feramance/qBitrr"
 url = "https://pypi.org/simple/"
 
 [tool.autopep8]
```

### Comparing `qbitrr2-4.6.0/qBitrr/arss.py` & `qbitrr2-4.6.1/qBitrr/arss.py`

 * *Files 0% similar despite different names*

```diff
@@ -4816,40 +4816,41 @@
     def run_search_loop(self):
         return
 
 
 class FreeSpaceManager(Arr):
     def __init__(self, categories: set[str], manager: ArrManager):
         self._name = "FreeSpaceManager"
-        self.categories = categories
         self.manager = manager
-        self.pause = set()
-        self.resume = set()
-        self.expiring_bool = ExpiringSet(max_age_seconds=10)
-        self.ignore_torrents_younger_than = CONFIG.get(
-            "Settings.IgnoreTorrentsYoungerThan", fallback=600
-        )
-        self.timed_ignore_cache = ExpiringSet(max_age_seconds=self.ignore_torrents_younger_than)
-        self.needs_cleanup = False
+        self.logger = logging.getLogger(f"qBitrr.{self._name}")
         self._LOG_LEVEL = self.manager.qbit_manager.logger.level
         if ENABLE_LOGS:
             LOGS_FOLDER = HOME_PATH.joinpath("logs")
             LOGS_FOLDER.mkdir(parents=True, exist_ok=True)
             LOGS_FOLDER.chmod(mode=0o777)
             logfile = LOGS_FOLDER.joinpath(self._name + ".log")
             if pathlib.Path(logfile).is_file():
                 logold = LOGS_FOLDER.joinpath(self._name + ".log.old")
                 logfile.rename(logold)
             fh = logging.FileHandler(logfile)
-            self.logger = logging.getLogger(f"qBitrr.{self._name}")
             self.logger.addHandler(fh)
-        else:
-            self.logger = logging.getLogger(f"qBitrr.{self._name}")
         run_logs(self.logger)
-        self.completed_folder = pathlib.Path(COMPLETED_DOWNLOAD_FOLDER)
+        self.categories = categories
+        self.logger.trace("Categories: %s", self.categories)
+        self.pause = set()
+        self.resume = set()
+        self.expiring_bool = ExpiringSet(max_age_seconds=10)
+        self.ignore_torrents_younger_than = CONFIG.get(
+            "Settings.IgnoreTorrentsYoungerThan", fallback=600
+        )
+        self.timed_ignore_cache = ExpiringSet(max_age_seconds=self.ignore_torrents_younger_than)
+        self.needs_cleanup = False
+        self.completed_folder = pathlib.Path(COMPLETED_DOWNLOAD_FOLDER).joinpath(
+            list(self.categories)[0]
+        )
         self.min_free_space = FREE_SPACE
         self.current_free_space = shutil.disk_usage(self.completed_folder).free - parse_size(
             self.min_free_space
         )
         self.logger.trace("Current free space: %s", self.current_free_space)
         self.manager.qbit_manager.client.torrents_create_tags(
             [
@@ -4894,15 +4895,15 @@
             elif (
                 torrent.state_enum == TorrentStates.PAUSED_DOWNLOAD
                 and self.current_free_space > torrent["amount_left"]
             ):
                 self.current_free_space = free_space_test
                 self.logger.trace("Can download: Free space %s", self.current_free_space)
                 torrent.remove_tags(tags=["qBitrr-free_space_paused"])
-        elif self.is_complete_state(torrent) and "qBitrr-free_space_paused" in torrent.tags:
+        elif not self.is_downloading_state(torrent) and "qBitrr-free_space_paused" in torrent.tags:
             self.logger.trace(
                 "Removing tag[%s] for completed torrent[%s]: Free space %s",
                 "qBitrr-free_space_paused",
                 torrent,
                 self.current_free_space,
             )
             torrent.remove_tags(tags=["qBitrr-free_space_paused"])
```

### Comparing `qbitrr2-4.6.0/qBitrr/config.py` & `qbitrr2-4.6.1/qBitrr/config.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.0/qBitrr/env_config.py` & `qbitrr2-4.6.1/qBitrr/env_config.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.0/qBitrr/errors.py` & `qbitrr2-4.6.1/qBitrr/errors.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.0/qBitrr/ffprobe.py` & `qbitrr2-4.6.1/qBitrr/ffprobe.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.0/qBitrr/gen_config.py` & `qbitrr2-4.6.1/qBitrr/gen_config.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.0/qBitrr/home_path.py` & `qbitrr2-4.6.1/qBitrr/home_path.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.0/qBitrr/logger.py` & `qbitrr2-4.6.1/qBitrr/logger.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.0/qBitrr/main.py` & `qbitrr2-4.6.1/qBitrr/main.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.0/qBitrr/tables.py` & `qbitrr2-4.6.1/qBitrr/tables.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.0/qBitrr/utils.py` & `qbitrr2-4.6.1/qBitrr/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 ping3.EXCEPTIONS = True
 
 logger = logging.getLogger("qBitrr.Utils")
 
 CACHE = TTLCache(maxsize=50, ttl=60)
 
 UNITS = {
-    "k": 1e3,
-    "m": 1e6,
-    "g": 1e9,
-    "t": 1e12,
+    "k": 1024,
+    "m": 1048576,
+    "g": 1073741824,
+    "t": 1099511627776,
 }
 
 
 def absolute_file_paths(directory: pathlib.Path | str) -> Iterator[pathlib.Path]:
     file_counter = 0
     error = True
     while error:
```

### Comparing `qbitrr2-4.6.0/qBitrr2.egg-info/PKG-INFO` & `qbitrr2-4.6.1/qBitrr2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qBitrr2
-Version: 4.6.0
+Version: 4.6.1
 Summary: "A simple Python script to talk to qBittorrent and Arr's"
 Home-page: https://github.com/Feramance/qBitrr
 Author: Feramance
 Author-email: fera@fera.wtf
 License: MIT
 Project-URL: Issue Tracker, https://github.com/Feramance/qBitrr/issues
 Project-URL: Source Code, https://github.com/Feramance/qBitrr
```

### Comparing `qbitrr2-4.6.0/qBitrr2.egg-info/requires.txt` & `qbitrr2-4.6.1/qBitrr2.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.0/setup.cfg` & `qbitrr2-4.6.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = qBitrr2
-version = 4.6.0
+version = 4.6.1
 description = "A simple Python script to talk to qBittorrent and Arr's"
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Feramance/qBitrr
 author = Feramance
 author_email = fera@fera.wtf
 license = MIT
```

