# Comparing `tmp/mpris-api-1.2.0.tar.gz` & `tmp/mpris-api-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/pawel/workspace/repo/mpris-api/dist/.tmp-8xjss3lc/mpris-api-1.2.0.tar", last modified: Wed May 15 19:05:15 2024, max compression
+gzip compressed data, was "/home/pawel/workspace/repo/mpris-api/dist/.tmp-zxur9abh/mpris-api-1.2.1.tar", last modified: Thu May 16 12:41:13 2024, max compression
```

## Comparing `mpris-api-1.2.0.tar` & `mpris-api-1.2.1.tar`

### file list

```diff
@@ -1,54 +1,56 @@
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-15 19:05:15.000000 mpris-api-1.2.0/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1072 2024-04-06 19:49:23.000000 mpris-api-1.2.0/LICENSE.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)      102 2024-05-12 15:19:56.000000 mpris-api-1.2.0/MANIFEST.in
--rw-r--r--   0 pawel     (1000) pawel     (1000)     3053 2024-05-15 19:05:15.000000 mpris-api-1.2.0/PKG-INFO
--rw-r--r--   0 pawel     (1000) pawel     (1000)     2434 2024-05-12 12:01:51.000000 mpris-api-1.2.0/README.md
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-15 19:05:15.000000 mpris-api-1.2.0/pkg/
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-15 19:05:15.000000 mpris-api-1.2.0/pkg/mpris_api/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     5159 2024-05-15 18:22:32.000000 mpris-api-1.2.0/pkg/mpris_api/MprisService.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     2040 2024-05-14 14:07:54.000000 mpris-api-1.2.0/pkg/mpris_api/MprisUpdateNotifier.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      280 2024-05-15 18:58:59.000000 mpris-api-1.2.0/pkg/mpris_api/__init__.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-15 19:05:15.000000 mpris-api-1.2.0/pkg/mpris_api/adapter/
--rw-r--r--   0 pawel     (1000) pawel     (1000)      835 2024-05-12 09:32:33.000000 mpris-api-1.2.0/pkg/mpris_api/adapter/IMprisAdapterPlayLists.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     2219 2024-05-15 19:00:38.000000 mpris-api-1.2.0/pkg/mpris_api/adapter/IMprisAdapterPlayer.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      945 2024-05-11 08:53:04.000000 mpris-api-1.2.0/pkg/mpris_api/adapter/IMprisAdapterRoot.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      789 2024-05-12 11:03:06.000000 mpris-api-1.2.0/pkg/mpris_api/adapter/IMprisAdapterTrackList.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)       78 2024-05-09 17:49:43.000000 mpris-api-1.2.0/pkg/mpris_api/adapter/__init__.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-15 19:05:15.000000 mpris-api-1.2.0/pkg/mpris_api/common/
--rw-r--r--   0 pawel     (1000) pawel     (1000)      520 2024-05-15 18:30:46.000000 mpris-api-1.2.0/pkg/mpris_api/common/DbusArray.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      590 2024-05-15 18:31:14.000000 mpris-api-1.2.0/pkg/mpris_api/common/DbusMaybe.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1824 2024-05-15 18:46:23.000000 mpris-api-1.2.0/pkg/mpris_api/common/DbusObject.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     3678 2024-05-12 11:46:26.000000 mpris-api-1.2.0/pkg/mpris_api/common/DbusObjectSpec.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      645 2024-05-15 18:56:48.000000 mpris-api-1.2.0/pkg/mpris_api/common/DbusPrimitive.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      736 2024-05-15 18:22:10.000000 mpris-api-1.2.0/pkg/mpris_api/common/DbusType.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      390 2024-05-15 18:34:34.000000 mpris-api-1.2.0/pkg/mpris_api/common/IDbusTypeWrapper.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)       78 2024-05-09 18:20:04.000000 mpris-api-1.2.0/pkg/mpris_api/common/__init__.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1882 2024-05-15 18:21:41.000000 mpris-api-1.2.0/pkg/mpris_api/common/dbusDecorators.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      557 2024-05-14 14:19:55.000000 mpris-api-1.2.0/pkg/mpris_api/common/dbusEnums.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-15 19:05:15.000000 mpris-api-1.2.0/pkg/mpris_api/interface/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1686 2024-05-14 14:11:03.000000 mpris-api-1.2.0/pkg/mpris_api/interface/MprisInterfaceBase.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     3836 2024-05-15 18:35:40.000000 mpris-api-1.2.0/pkg/mpris_api/interface/MprisInterfacePlayLists.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     9710 2024-05-15 18:36:40.000000 mpris-api-1.2.0/pkg/mpris_api/interface/MprisInterfacePlayer.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     4501 2024-05-15 18:19:23.000000 mpris-api-1.2.0/pkg/mpris_api/interface/MprisInterfaceRoot.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     4684 2024-05-15 18:47:34.000000 mpris-api-1.2.0/pkg/mpris_api/interface/MprisInterfaceTrackList.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)       78 2024-05-09 17:49:43.000000 mpris-api-1.2.0/pkg/mpris_api/interface/__init__.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-15 19:05:15.000000 mpris-api-1.2.0/pkg/mpris_api/model/
--rw-r--r--   0 pawel     (1000) pawel     (1000)      254 2024-05-12 11:21:27.000000 mpris-api-1.2.0/pkg/mpris_api/model/MprisConstant.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      226 2024-05-14 14:19:19.000000 mpris-api-1.2.0/pkg/mpris_api/model/MprisLoopStatus.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     3350 2024-05-15 18:47:57.000000 mpris-api-1.2.0/pkg/mpris_api/model/MprisMetaData.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      236 2024-05-14 14:19:31.000000 mpris-api-1.2.0/pkg/mpris_api/model/MprisPlaybackStatus.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1027 2024-05-15 18:34:52.000000 mpris-api-1.2.0/pkg/mpris_api/model/MprisPlaylist.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      341 2024-05-14 14:19:05.000000 mpris-api-1.2.0/pkg/mpris_api/model/MprisPlaylistOrdering.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      343 2024-05-12 11:22:22.000000 mpris-api-1.2.0/pkg/mpris_api/model/MprisTrack.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)       78 2024-05-09 21:44:38.000000 mpris-api-1.2.0/pkg/mpris_api/model/__init__.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)        0 2024-05-12 07:49:45.000000 mpris-api-1.2.0/pkg/mpris_api/py.typed
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-15 19:05:15.000000 mpris-api-1.2.0/pkg/mpris_api.egg-info/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     3053 2024-05-15 19:05:15.000000 mpris-api-1.2.0/pkg/mpris_api.egg-info/PKG-INFO
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1533 2024-05-15 19:05:15.000000 mpris-api-1.2.0/pkg/mpris_api.egg-info/SOURCES.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2024-05-15 19:05:15.000000 mpris-api-1.2.0/pkg/mpris_api.egg-info/dependency_links.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)       41 2024-05-15 19:05:15.000000 mpris-api-1.2.0/pkg/mpris_api.egg-info/requires.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)       10 2024-05-15 19:05:15.000000 mpris-api-1.2.0/pkg/mpris_api.egg-info/top_level.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)      903 2024-05-12 15:43:25.000000 mpris-api-1.2.0/pyproject.toml
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-15 19:05:15.000000 mpris-api-1.2.0/requirements/
--rw-r--r--   0 pawel     (1000) pawel     (1000)       51 2024-05-12 15:43:43.000000 mpris-api-1.2.0/requirements/release.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)       38 2024-05-15 19:05:15.000000 mpris-api-1.2.0/setup.cfg
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-16 12:41:13.000000 mpris-api-1.2.1/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1072 2024-04-06 19:49:23.000000 mpris-api-1.2.1/LICENSE.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      102 2024-05-12 15:19:56.000000 mpris-api-1.2.1/MANIFEST.in
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     3053 2024-05-16 12:41:13.000000 mpris-api-1.2.1/PKG-INFO
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     2434 2024-05-12 12:01:51.000000 mpris-api-1.2.1/README.md
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-16 12:41:13.000000 mpris-api-1.2.1/pkg/
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-16 12:41:13.000000 mpris-api-1.2.1/pkg/mpris_api/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     5159 2024-05-15 18:22:32.000000 mpris-api-1.2.1/pkg/mpris_api/MprisService.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     2040 2024-05-14 14:07:54.000000 mpris-api-1.2.1/pkg/mpris_api/MprisUpdateNotifier.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      280 2024-05-16 12:39:38.000000 mpris-api-1.2.1/pkg/mpris_api/__init__.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-16 12:41:13.000000 mpris-api-1.2.1/pkg/mpris_api/adapter/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      835 2024-05-12 09:32:33.000000 mpris-api-1.2.1/pkg/mpris_api/adapter/IMprisAdapterPlayLists.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     2219 2024-05-15 19:00:38.000000 mpris-api-1.2.1/pkg/mpris_api/adapter/IMprisAdapterPlayer.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      945 2024-05-11 08:53:04.000000 mpris-api-1.2.1/pkg/mpris_api/adapter/IMprisAdapterRoot.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      789 2024-05-12 11:03:06.000000 mpris-api-1.2.1/pkg/mpris_api/adapter/IMprisAdapterTrackList.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       78 2024-05-09 17:49:43.000000 mpris-api-1.2.1/pkg/mpris_api/adapter/__init__.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-16 12:41:13.000000 mpris-api-1.2.1/pkg/mpris_api/common/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      520 2024-05-16 11:57:09.000000 mpris-api-1.2.1/pkg/mpris_api/common/DbusArray.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      725 2024-05-16 12:28:25.000000 mpris-api-1.2.1/pkg/mpris_api/common/DbusDict.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      590 2024-05-16 11:56:56.000000 mpris-api-1.2.1/pkg/mpris_api/common/DbusMaybe.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1824 2024-05-15 18:46:23.000000 mpris-api-1.2.1/pkg/mpris_api/common/DbusObject.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     3678 2024-05-12 11:46:26.000000 mpris-api-1.2.1/pkg/mpris_api/common/DbusObjectSpec.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      645 2024-05-15 18:56:48.000000 mpris-api-1.2.1/pkg/mpris_api/common/DbusPrimitive.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      763 2024-05-16 12:30:57.000000 mpris-api-1.2.1/pkg/mpris_api/common/DbusTuple.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      736 2024-05-15 18:22:10.000000 mpris-api-1.2.1/pkg/mpris_api/common/DbusType.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      390 2024-05-15 18:34:34.000000 mpris-api-1.2.1/pkg/mpris_api/common/IDbusTypeWrapper.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       78 2024-05-09 18:20:04.000000 mpris-api-1.2.1/pkg/mpris_api/common/__init__.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1882 2024-05-15 18:21:41.000000 mpris-api-1.2.1/pkg/mpris_api/common/dbusDecorators.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      557 2024-05-14 14:19:55.000000 mpris-api-1.2.1/pkg/mpris_api/common/dbusEnums.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-16 12:41:13.000000 mpris-api-1.2.1/pkg/mpris_api/interface/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1686 2024-05-14 14:11:03.000000 mpris-api-1.2.1/pkg/mpris_api/interface/MprisInterfaceBase.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     3836 2024-05-15 18:35:40.000000 mpris-api-1.2.1/pkg/mpris_api/interface/MprisInterfacePlayLists.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     9710 2024-05-15 18:36:40.000000 mpris-api-1.2.1/pkg/mpris_api/interface/MprisInterfacePlayer.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     4501 2024-05-15 18:19:23.000000 mpris-api-1.2.1/pkg/mpris_api/interface/MprisInterfaceRoot.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     4684 2024-05-15 18:47:34.000000 mpris-api-1.2.1/pkg/mpris_api/interface/MprisInterfaceTrackList.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       78 2024-05-09 17:49:43.000000 mpris-api-1.2.1/pkg/mpris_api/interface/__init__.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-16 12:41:13.000000 mpris-api-1.2.1/pkg/mpris_api/model/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      254 2024-05-12 11:21:27.000000 mpris-api-1.2.1/pkg/mpris_api/model/MprisConstant.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      226 2024-05-14 14:19:19.000000 mpris-api-1.2.1/pkg/mpris_api/model/MprisLoopStatus.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     3395 2024-05-16 12:01:19.000000 mpris-api-1.2.1/pkg/mpris_api/model/MprisMetaData.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      236 2024-05-14 14:19:31.000000 mpris-api-1.2.1/pkg/mpris_api/model/MprisPlaybackStatus.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1130 2024-05-16 12:28:04.000000 mpris-api-1.2.1/pkg/mpris_api/model/MprisPlaylist.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      341 2024-05-14 14:19:05.000000 mpris-api-1.2.1/pkg/mpris_api/model/MprisPlaylistOrdering.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      343 2024-05-12 11:22:22.000000 mpris-api-1.2.1/pkg/mpris_api/model/MprisTrack.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       78 2024-05-09 21:44:38.000000 mpris-api-1.2.1/pkg/mpris_api/model/__init__.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        0 2024-05-12 07:49:45.000000 mpris-api-1.2.1/pkg/mpris_api/py.typed
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-16 12:41:13.000000 mpris-api-1.2.1/pkg/mpris_api.egg-info/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     3053 2024-05-16 12:41:13.000000 mpris-api-1.2.1/pkg/mpris_api.egg-info/PKG-INFO
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1600 2024-05-16 12:41:13.000000 mpris-api-1.2.1/pkg/mpris_api.egg-info/SOURCES.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2024-05-16 12:41:13.000000 mpris-api-1.2.1/pkg/mpris_api.egg-info/dependency_links.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       41 2024-05-16 12:41:13.000000 mpris-api-1.2.1/pkg/mpris_api.egg-info/requires.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       10 2024-05-16 12:41:13.000000 mpris-api-1.2.1/pkg/mpris_api.egg-info/top_level.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      903 2024-05-12 15:43:25.000000 mpris-api-1.2.1/pyproject.toml
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-16 12:41:13.000000 mpris-api-1.2.1/requirements/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       51 2024-05-12 15:43:43.000000 mpris-api-1.2.1/requirements/release.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       38 2024-05-16 12:41:13.000000 mpris-api-1.2.1/setup.cfg
```

### Comparing `mpris-api-1.2.0/LICENSE.txt` & `mpris-api-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mpris-api-1.2.0/PKG-INFO` & `mpris-api-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpris-api
-Version: 1.2.0
+Version: 1.2.1
 Summary: Make your multimedia app discoverable by linux desktop.
 Author-email: "P.J. Grochowski" <pawel.grochowski.dev@gmail.com>
 License: MIT
 Project-URL: Repository, https://bitbucket.org/massultidev/mpris-api
 Keywords: mpris,player,multimedia,linux
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mpris-api-1.2.0/README.md` & `mpris-api-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `mpris-api-1.2.0/pkg/mpris_api/MprisService.py` & `mpris-api-1.2.1/pkg/mpris_api/MprisService.py`

 * *Files identical despite different names*

### Comparing `mpris-api-1.2.0/pkg/mpris_api/MprisUpdateNotifier.py` & `mpris-api-1.2.1/pkg/mpris_api/MprisUpdateNotifier.py`

 * *Files identical despite different names*

### Comparing `mpris-api-1.2.0/pkg/mpris_api/adapter/IMprisAdapterPlayLists.py` & `mpris-api-1.2.1/pkg/mpris_api/adapter/IMprisAdapterPlayLists.py`

 * *Files identical despite different names*

### Comparing `mpris-api-1.2.0/pkg/mpris_api/adapter/IMprisAdapterPlayer.py` & `mpris-api-1.2.1/pkg/mpris_api/adapter/IMprisAdapterPlayer.py`

 * *Files identical despite different names*

### Comparing `mpris-api-1.2.0/pkg/mpris_api/adapter/IMprisAdapterRoot.py` & `mpris-api-1.2.1/pkg/mpris_api/adapter/IMprisAdapterRoot.py`

 * *Files identical despite different names*

### Comparing `mpris-api-1.2.0/pkg/mpris_api/adapter/IMprisAdapterTrackList.py` & `mpris-api-1.2.1/pkg/mpris_api/adapter/IMprisAdapterTrackList.py`

 * *Files identical despite different names*

### Comparing `mpris-api-1.2.0/pkg/mpris_api/common/DbusArray.py` & `mpris-api-1.2.1/pkg/mpris_api/common/DbusArray.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Any, List, Optional, Type
 
 from mpris_api.common.DbusType import IDbusType
 
 
 class DbusArray(IDbusType):
 
-    def __init__(self, itemSpec: IDbusType) -> None:
-        self._itemSpec: IDbusType = itemSpec
+    def __init__(self, itemType: IDbusType) -> None:
+        self._itemType: IDbusType = itemType
 
     def getSignaturePy(self) -> Optional[Type[Any]]:
-        return List[self._itemSpec.getSignaturePy()]  # type: ignore
+        return List[self._itemType.getSignaturePy()]  # type: ignore
 
     def getSignatureDbus(self) -> str:
-        return f'a{self._itemSpec.getSignatureDbus()}'
+        return f'a{self._itemType.getSignatureDbus()}'
```

### Comparing `mpris-api-1.2.0/pkg/mpris_api/common/DbusMaybe.py` & `mpris-api-1.2.1/pkg/mpris_api/common/DbusTuple.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright by: P.J. Grochowski
 
-from dataclasses import dataclass
-from typing import Any, Optional, Tuple, Type
+from typing import Any, List, Optional, Tuple, Type
 
 from mpris_api.common.DbusType import IDbusType
 
 
-@dataclass
-class DbusMaybe(IDbusType):
+class DbusTuple(IDbusType):
 
-    def __init__(self, valueSpec: IDbusType) -> None:
-        self._valueSpec: IDbusType = valueSpec
+    def __init__(self, *itemType: IDbusType) -> None:
+        self._itemTypes: List[IDbusType] = list(itemType)
 
     def getSignaturePy(self) -> Optional[Type[Any]]:
-        return Tuple[bool, Optional[self._valueSpec.getSignaturePy()]]  # type: ignore
+        itemSignatures = tuple([
+            itemType.getSignaturePy()
+            for itemType in self._itemTypes
+        ])
+        return Tuple[itemSignatures]  # type: ignore
 
     def getSignatureDbus(self) -> str:
-        return f'(b{self._valueSpec.getSignatureDbus()})'
+        itemSignatures = ''.join([
+            itemType.getSignatureDbus()
+            for itemType in self._itemTypes
+        ])
+        return f'({itemSignatures})'
```

### Comparing `mpris-api-1.2.0/pkg/mpris_api/common/DbusObject.py` & `mpris-api-1.2.1/pkg/mpris_api/common/DbusObject.py`

 * *Files identical despite different names*

### Comparing `mpris-api-1.2.0/pkg/mpris_api/common/DbusObjectSpec.py` & `mpris-api-1.2.1/pkg/mpris_api/common/DbusObjectSpec.py`

 * *Files identical despite different names*

### Comparing `mpris-api-1.2.0/pkg/mpris_api/common/DbusPrimitive.py` & `mpris-api-1.2.1/pkg/mpris_api/common/DbusPrimitive.py`

 * *Files identical despite different names*

### Comparing `mpris-api-1.2.0/pkg/mpris_api/common/DbusType.py` & `mpris-api-1.2.1/pkg/mpris_api/common/DbusType.py`

 * *Files identical despite different names*

### Comparing `mpris-api-1.2.0/pkg/mpris_api/common/dbusDecorators.py` & `mpris-api-1.2.1/pkg/mpris_api/common/dbusDecorators.py`

 * *Files identical despite different names*

### Comparing `mpris-api-1.2.0/pkg/mpris_api/common/dbusEnums.py` & `mpris-api-1.2.1/pkg/mpris_api/common/dbusEnums.py`

 * *Files identical despite different names*

### Comparing `mpris-api-1.2.0/pkg/mpris_api/interface/MprisInterfaceBase.py` & `mpris-api-1.2.1/pkg/mpris_api/interface/MprisInterfaceBase.py`

 * *Files identical despite different names*

### Comparing `mpris-api-1.2.0/pkg/mpris_api/interface/MprisInterfacePlayLists.py` & `mpris-api-1.2.1/pkg/mpris_api/interface/MprisInterfacePlayLists.py`

 * *Files identical despite different names*

### Comparing `mpris-api-1.2.0/pkg/mpris_api/interface/MprisInterfacePlayer.py` & `mpris-api-1.2.1/pkg/mpris_api/interface/MprisInterfacePlayer.py`

 * *Files identical despite different names*

### Comparing `mpris-api-1.2.0/pkg/mpris_api/interface/MprisInterfaceRoot.py` & `mpris-api-1.2.1/pkg/mpris_api/interface/MprisInterfaceRoot.py`

 * *Files identical despite different names*

### Comparing `mpris-api-1.2.0/pkg/mpris_api/interface/MprisInterfaceTrackList.py` & `mpris-api-1.2.1/pkg/mpris_api/interface/MprisInterfaceTrackList.py`

 * *Files identical despite different names*

### Comparing `mpris-api-1.2.0/pkg/mpris_api/model/MprisMetaData.py` & `mpris-api-1.2.1/pkg/mpris_api/model/MprisMetaData.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 from dataclasses import dataclass
 from typing import Dict, List, Optional
 
 from dbus_next import Variant
 from tunit.unit import Microseconds
 
 from mpris_api.common.DbusArray import DbusArray
+from mpris_api.common.DbusDict import DbusDict
 from mpris_api.common.DbusObject import DbusObject
 from mpris_api.common.DbusPrimitive import DbusPrimitive
-from mpris_api.common.DbusType import DbusType, IDbusType
+from mpris_api.common.DbusType import IDbusType
 from mpris_api.common.IDbusTypeWrapper import IDbusTypeWrapper
 
 
 class MprisMetaDataField:
     TRACK_ID: str = 'mpris:trackid'
     LENGTH: str = 'mpris:length'
     ART_URL: str = 'mpris:artUrl'
@@ -58,17 +59,17 @@
     albumArtists: Optional[List[str]] = None
     discNumber: Optional[int] = None
     trackNumber: Optional[int] = None
     comments: Optional[List[str]] = None
 
     @classmethod
     def getType(cls) -> IDbusType:
-        return DbusType(
-            signaturePy=Dict[str, Variant],
-            signatureDbus='a{sv}'
+        return DbusDict(
+            keyType=DbusPrimitive.STRING,
+            valueType=DbusPrimitive.VARIANT
         )
 
     def getValue(self) -> Dict[str, Variant]:
         metaDataDict = {
             MprisMetaDataField.TRACK_ID: self.trackId.getValue(),
             MprisMetaDataField.LENGTH: int(self.length) if self.length is not None else None,
             MprisMetaDataField.ART_URL: self.artUrl,
```

### Comparing `mpris-api-1.2.0/pkg/mpris_api.egg-info/PKG-INFO` & `mpris-api-1.2.1/pkg/mpris_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpris-api
-Version: 1.2.0
+Version: 1.2.1
 Summary: Make your multimedia app discoverable by linux desktop.
 Author-email: "P.J. Grochowski" <pawel.grochowski.dev@gmail.com>
 License: MIT
 Project-URL: Repository, https://bitbucket.org/massultidev/mpris-api
 Keywords: mpris,player,multimedia,linux
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mpris-api-1.2.0/pkg/mpris_api.egg-info/SOURCES.txt` & `mpris-api-1.2.1/pkg/mpris_api.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,20 @@
 pkg/mpris_api.egg-info/top_level.txt
 pkg/mpris_api/adapter/IMprisAdapterPlayLists.py
 pkg/mpris_api/adapter/IMprisAdapterPlayer.py
 pkg/mpris_api/adapter/IMprisAdapterRoot.py
 pkg/mpris_api/adapter/IMprisAdapterTrackList.py
 pkg/mpris_api/adapter/__init__.py
 pkg/mpris_api/common/DbusArray.py
+pkg/mpris_api/common/DbusDict.py
 pkg/mpris_api/common/DbusMaybe.py
 pkg/mpris_api/common/DbusObject.py
 pkg/mpris_api/common/DbusObjectSpec.py
 pkg/mpris_api/common/DbusPrimitive.py
+pkg/mpris_api/common/DbusTuple.py
 pkg/mpris_api/common/DbusType.py
 pkg/mpris_api/common/IDbusTypeWrapper.py
 pkg/mpris_api/common/__init__.py
 pkg/mpris_api/common/dbusDecorators.py
 pkg/mpris_api/common/dbusEnums.py
 pkg/mpris_api/interface/MprisInterfaceBase.py
 pkg/mpris_api/interface/MprisInterfacePlayLists.py
```

### Comparing `mpris-api-1.2.0/pyproject.toml` & `mpris-api-1.2.1/pyproject.toml`

 * *Files identical despite different names*

