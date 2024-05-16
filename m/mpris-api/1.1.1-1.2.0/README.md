# Comparing `tmp/mpris-api-1.1.1.tar.gz` & `tmp/mpris-api-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/pawel/workspace/repo/mpris-api/dist/.tmp-xo2xgk9d/mpris-api-1.1.1.tar", last modified: Tue May 14 14:24:13 2024, max compression
+gzip compressed data, was "/home/pawel/workspace/repo/mpris-api/dist/.tmp-8xjss3lc/mpris-api-1.2.0.tar", last modified: Wed May 15 19:05:15 2024, max compression
```

## Comparing `mpris-api-1.1.1.tar` & `mpris-api-1.2.0.tar`

### file list

```diff
@@ -1,50 +1,54 @@
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-14 14:24:13.000000 mpris-api-1.1.1/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1072 2024-04-06 19:49:23.000000 mpris-api-1.1.1/LICENSE.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)      102 2024-05-12 15:19:56.000000 mpris-api-1.1.1/MANIFEST.in
--rw-r--r--   0 pawel     (1000) pawel     (1000)     3053 2024-05-14 14:24:13.000000 mpris-api-1.1.1/PKG-INFO
--rw-r--r--   0 pawel     (1000) pawel     (1000)     2434 2024-05-12 12:01:51.000000 mpris-api-1.1.1/README.md
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-14 14:24:13.000000 mpris-api-1.1.1/pkg/
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-14 14:24:13.000000 mpris-api-1.1.1/pkg/mpris_api/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     5218 2024-05-12 11:28:20.000000 mpris-api-1.1.1/pkg/mpris_api/MprisService.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     2040 2024-05-14 14:07:54.000000 mpris-api-1.1.1/pkg/mpris_api/MprisUpdateNotifier.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      280 2024-05-14 14:22:59.000000 mpris-api-1.1.1/pkg/mpris_api/__init__.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-14 14:24:13.000000 mpris-api-1.1.1/pkg/mpris_api/adapter/
--rw-r--r--   0 pawel     (1000) pawel     (1000)      835 2024-05-12 09:32:33.000000 mpris-api-1.1.1/pkg/mpris_api/adapter/IMprisAdapterPlayLists.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     2151 2024-05-12 08:39:29.000000 mpris-api-1.1.1/pkg/mpris_api/adapter/IMprisAdapterPlayer.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      945 2024-05-11 08:53:04.000000 mpris-api-1.1.1/pkg/mpris_api/adapter/IMprisAdapterRoot.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      789 2024-05-12 11:03:06.000000 mpris-api-1.1.1/pkg/mpris_api/adapter/IMprisAdapterTrackList.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)       78 2024-05-09 17:49:43.000000 mpris-api-1.1.1/pkg/mpris_api/adapter/__init__.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-14 14:24:13.000000 mpris-api-1.1.1/pkg/mpris_api/common/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1485 2024-05-12 11:19:02.000000 mpris-api-1.1.1/pkg/mpris_api/common/DbusObject.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     3678 2024-05-12 11:46:26.000000 mpris-api-1.1.1/pkg/mpris_api/common/DbusObjectSpec.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      483 2024-05-12 09:42:57.000000 mpris-api-1.1.1/pkg/mpris_api/common/DbusType.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)       78 2024-05-09 18:20:04.000000 mpris-api-1.1.1/pkg/mpris_api/common/__init__.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      209 2024-05-12 09:55:02.000000 mpris-api-1.1.1/pkg/mpris_api/common/dbusDecorators.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      557 2024-05-14 14:19:55.000000 mpris-api-1.1.1/pkg/mpris_api/common/dbusEnums.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-14 14:24:13.000000 mpris-api-1.1.1/pkg/mpris_api/interface/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1686 2024-05-14 14:11:03.000000 mpris-api-1.1.1/pkg/mpris_api/interface/MprisInterfaceBase.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     2909 2024-05-14 14:01:30.000000 mpris-api-1.1.1/pkg/mpris_api/interface/MprisInterfacePlayLists.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     7493 2024-05-14 14:01:30.000000 mpris-api-1.1.1/pkg/mpris_api/interface/MprisInterfacePlayer.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     3572 2024-05-14 14:01:30.000000 mpris-api-1.1.1/pkg/mpris_api/interface/MprisInterfaceRoot.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     3601 2024-05-14 14:01:30.000000 mpris-api-1.1.1/pkg/mpris_api/interface/MprisInterfaceTrackList.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)       78 2024-05-09 17:49:43.000000 mpris-api-1.1.1/pkg/mpris_api/interface/__init__.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-14 14:24:13.000000 mpris-api-1.1.1/pkg/mpris_api/model/
--rw-r--r--   0 pawel     (1000) pawel     (1000)      254 2024-05-12 11:21:27.000000 mpris-api-1.1.1/pkg/mpris_api/model/MprisConstant.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      226 2024-05-14 14:19:19.000000 mpris-api-1.1.1/pkg/mpris_api/model/MprisLoopStatus.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     2632 2024-05-14 13:51:57.000000 mpris-api-1.1.1/pkg/mpris_api/model/MprisMetaData.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      236 2024-05-14 14:19:31.000000 mpris-api-1.1.1/pkg/mpris_api/model/MprisPlaybackStatus.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      713 2024-05-14 13:51:36.000000 mpris-api-1.1.1/pkg/mpris_api/model/MprisPlaylist.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      341 2024-05-14 14:19:05.000000 mpris-api-1.1.1/pkg/mpris_api/model/MprisPlaylistOrdering.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      343 2024-05-12 11:22:22.000000 mpris-api-1.1.1/pkg/mpris_api/model/MprisTrack.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)       78 2024-05-09 21:44:38.000000 mpris-api-1.1.1/pkg/mpris_api/model/__init__.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)        0 2024-05-12 07:49:45.000000 mpris-api-1.1.1/pkg/mpris_api/py.typed
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-14 14:24:13.000000 mpris-api-1.1.1/pkg/mpris_api.egg-info/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     3053 2024-05-14 14:24:13.000000 mpris-api-1.1.1/pkg/mpris_api.egg-info/PKG-INFO
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1386 2024-05-14 14:24:13.000000 mpris-api-1.1.1/pkg/mpris_api.egg-info/SOURCES.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2024-05-14 14:24:13.000000 mpris-api-1.1.1/pkg/mpris_api.egg-info/dependency_links.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)       41 2024-05-14 14:24:13.000000 mpris-api-1.1.1/pkg/mpris_api.egg-info/requires.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)       10 2024-05-14 14:24:13.000000 mpris-api-1.1.1/pkg/mpris_api.egg-info/top_level.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)      903 2024-05-12 15:43:25.000000 mpris-api-1.1.1/pyproject.toml
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-14 14:24:13.000000 mpris-api-1.1.1/requirements/
--rw-r--r--   0 pawel     (1000) pawel     (1000)       51 2024-05-12 15:43:43.000000 mpris-api-1.1.1/requirements/release.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)       38 2024-05-14 14:24:13.000000 mpris-api-1.1.1/setup.cfg
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-15 19:05:15.000000 mpris-api-1.2.0/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1072 2024-04-06 19:49:23.000000 mpris-api-1.2.0/LICENSE.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      102 2024-05-12 15:19:56.000000 mpris-api-1.2.0/MANIFEST.in
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     3053 2024-05-15 19:05:15.000000 mpris-api-1.2.0/PKG-INFO
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     2434 2024-05-12 12:01:51.000000 mpris-api-1.2.0/README.md
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-15 19:05:15.000000 mpris-api-1.2.0/pkg/
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-15 19:05:15.000000 mpris-api-1.2.0/pkg/mpris_api/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     5159 2024-05-15 18:22:32.000000 mpris-api-1.2.0/pkg/mpris_api/MprisService.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     2040 2024-05-14 14:07:54.000000 mpris-api-1.2.0/pkg/mpris_api/MprisUpdateNotifier.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      280 2024-05-15 18:58:59.000000 mpris-api-1.2.0/pkg/mpris_api/__init__.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-15 19:05:15.000000 mpris-api-1.2.0/pkg/mpris_api/adapter/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      835 2024-05-12 09:32:33.000000 mpris-api-1.2.0/pkg/mpris_api/adapter/IMprisAdapterPlayLists.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     2219 2024-05-15 19:00:38.000000 mpris-api-1.2.0/pkg/mpris_api/adapter/IMprisAdapterPlayer.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      945 2024-05-11 08:53:04.000000 mpris-api-1.2.0/pkg/mpris_api/adapter/IMprisAdapterRoot.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      789 2024-05-12 11:03:06.000000 mpris-api-1.2.0/pkg/mpris_api/adapter/IMprisAdapterTrackList.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       78 2024-05-09 17:49:43.000000 mpris-api-1.2.0/pkg/mpris_api/adapter/__init__.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-15 19:05:15.000000 mpris-api-1.2.0/pkg/mpris_api/common/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      520 2024-05-15 18:30:46.000000 mpris-api-1.2.0/pkg/mpris_api/common/DbusArray.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      590 2024-05-15 18:31:14.000000 mpris-api-1.2.0/pkg/mpris_api/common/DbusMaybe.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1824 2024-05-15 18:46:23.000000 mpris-api-1.2.0/pkg/mpris_api/common/DbusObject.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     3678 2024-05-12 11:46:26.000000 mpris-api-1.2.0/pkg/mpris_api/common/DbusObjectSpec.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      645 2024-05-15 18:56:48.000000 mpris-api-1.2.0/pkg/mpris_api/common/DbusPrimitive.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      736 2024-05-15 18:22:10.000000 mpris-api-1.2.0/pkg/mpris_api/common/DbusType.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      390 2024-05-15 18:34:34.000000 mpris-api-1.2.0/pkg/mpris_api/common/IDbusTypeWrapper.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       78 2024-05-09 18:20:04.000000 mpris-api-1.2.0/pkg/mpris_api/common/__init__.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1882 2024-05-15 18:21:41.000000 mpris-api-1.2.0/pkg/mpris_api/common/dbusDecorators.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      557 2024-05-14 14:19:55.000000 mpris-api-1.2.0/pkg/mpris_api/common/dbusEnums.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-15 19:05:15.000000 mpris-api-1.2.0/pkg/mpris_api/interface/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1686 2024-05-14 14:11:03.000000 mpris-api-1.2.0/pkg/mpris_api/interface/MprisInterfaceBase.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     3836 2024-05-15 18:35:40.000000 mpris-api-1.2.0/pkg/mpris_api/interface/MprisInterfacePlayLists.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     9710 2024-05-15 18:36:40.000000 mpris-api-1.2.0/pkg/mpris_api/interface/MprisInterfacePlayer.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     4501 2024-05-15 18:19:23.000000 mpris-api-1.2.0/pkg/mpris_api/interface/MprisInterfaceRoot.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     4684 2024-05-15 18:47:34.000000 mpris-api-1.2.0/pkg/mpris_api/interface/MprisInterfaceTrackList.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       78 2024-05-09 17:49:43.000000 mpris-api-1.2.0/pkg/mpris_api/interface/__init__.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-15 19:05:15.000000 mpris-api-1.2.0/pkg/mpris_api/model/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      254 2024-05-12 11:21:27.000000 mpris-api-1.2.0/pkg/mpris_api/model/MprisConstant.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      226 2024-05-14 14:19:19.000000 mpris-api-1.2.0/pkg/mpris_api/model/MprisLoopStatus.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     3350 2024-05-15 18:47:57.000000 mpris-api-1.2.0/pkg/mpris_api/model/MprisMetaData.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      236 2024-05-14 14:19:31.000000 mpris-api-1.2.0/pkg/mpris_api/model/MprisPlaybackStatus.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1027 2024-05-15 18:34:52.000000 mpris-api-1.2.0/pkg/mpris_api/model/MprisPlaylist.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      341 2024-05-14 14:19:05.000000 mpris-api-1.2.0/pkg/mpris_api/model/MprisPlaylistOrdering.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      343 2024-05-12 11:22:22.000000 mpris-api-1.2.0/pkg/mpris_api/model/MprisTrack.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       78 2024-05-09 21:44:38.000000 mpris-api-1.2.0/pkg/mpris_api/model/__init__.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        0 2024-05-12 07:49:45.000000 mpris-api-1.2.0/pkg/mpris_api/py.typed
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-15 19:05:15.000000 mpris-api-1.2.0/pkg/mpris_api.egg-info/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     3053 2024-05-15 19:05:15.000000 mpris-api-1.2.0/pkg/mpris_api.egg-info/PKG-INFO
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1533 2024-05-15 19:05:15.000000 mpris-api-1.2.0/pkg/mpris_api.egg-info/SOURCES.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2024-05-15 19:05:15.000000 mpris-api-1.2.0/pkg/mpris_api.egg-info/dependency_links.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       41 2024-05-15 19:05:15.000000 mpris-api-1.2.0/pkg/mpris_api.egg-info/requires.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       10 2024-05-15 19:05:15.000000 mpris-api-1.2.0/pkg/mpris_api.egg-info/top_level.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      903 2024-05-12 15:43:25.000000 mpris-api-1.2.0/pyproject.toml
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-15 19:05:15.000000 mpris-api-1.2.0/requirements/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       51 2024-05-12 15:43:43.000000 mpris-api-1.2.0/requirements/release.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       38 2024-05-15 19:05:15.000000 mpris-api-1.2.0/setup.cfg
```

### Comparing `mpris-api-1.1.1/LICENSE.txt` & `mpris-api-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mpris-api-1.1.1/PKG-INFO` & `mpris-api-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpris-api
-Version: 1.1.1
+Version: 1.2.0
 Summary: Make your multimedia app discoverable by linux desktop.
 Author-email: "P.J. Grochowski" <pawel.grochowski.dev@gmail.com>
 License: MIT
 Project-URL: Repository, https://bitbucket.org/massultidev/mpris-api
 Keywords: mpris,player,multimedia,linux
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mpris-api-1.1.1/README.md` & `mpris-api-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mpris-api-1.1.1/pkg/mpris_api/MprisService.py` & `mpris-api-1.2.0/pkg/mpris_api/MprisService.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 from mpris_api import __logger as logger
 from mpris_api.MprisUpdateNotifier import MprisUpdateNotifier
 from mpris_api.adapter.IMprisAdapterPlayLists import IMprisAdapterPlayLists
 from mpris_api.adapter.IMprisAdapterPlayer import IMprisAdapterPlayer
 from mpris_api.adapter.IMprisAdapterRoot import IMprisAdapterRoot
 from mpris_api.adapter.IMprisAdapterTrackList import IMprisAdapterTrackList
-from mpris_api.common.DbusObjectSpec import DbusObjectSpec
 from mpris_api.interface.MprisInterfacePlayLists import MprisInterfacePlayLists
 from mpris_api.interface.MprisInterfacePlayer import MprisInterfacePlayer
 from mpris_api.interface.MprisInterfaceRoot import MprisInterfaceRoot
 from mpris_api.interface.MprisInterfaceTrackList import MprisInterfaceTrackList
 from mpris_api.model.MprisConstant import MprisConstant
```

### Comparing `mpris-api-1.1.1/pkg/mpris_api/MprisUpdateNotifier.py` & `mpris-api-1.2.0/pkg/mpris_api/MprisUpdateNotifier.py`

 * *Files identical despite different names*

### Comparing `mpris-api-1.1.1/pkg/mpris_api/adapter/IMprisAdapterPlayLists.py` & `mpris-api-1.2.0/pkg/mpris_api/adapter/IMprisAdapterPlayLists.py`

 * *Files identical despite different names*

### Comparing `mpris-api-1.1.1/pkg/mpris_api/adapter/IMprisAdapterPlayer.py` & `mpris-api-1.2.0/pkg/mpris_api/adapter/IMprisAdapterPlayer.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from mpris_api.model.MprisLoopStatus import MprisLoopStatus
 from mpris_api.model.MprisMetaData import MprisMetaData
 from mpris_api.model.MprisPlaybackStatus import MprisPlaybackStatus
 
 
 class IMprisAdapterPlayer(ABC):
 
+    DEFAULT_MIN_RATE: float = 1.0
+    DEFAULT_MAX_RATE: float = 1.0
     DEFAULT_RATE: float = 1.0
     MIN_VOLUME: float = 0.0
     MAX_VOLUME: float = 1.0
 
     @abstractmethod
     def canControl(self) -> bool: ...
     @abstractmethod
```

### Comparing `mpris-api-1.1.1/pkg/mpris_api/adapter/IMprisAdapterRoot.py` & `mpris-api-1.2.0/pkg/mpris_api/adapter/IMprisAdapterRoot.py`

 * *Files identical despite different names*

### Comparing `mpris-api-1.1.1/pkg/mpris_api/adapter/IMprisAdapterTrackList.py` & `mpris-api-1.2.0/pkg/mpris_api/adapter/IMprisAdapterTrackList.py`

 * *Files identical despite different names*

### Comparing `mpris-api-1.1.1/pkg/mpris_api/common/DbusObject.py` & `mpris-api-1.2.0/pkg/mpris_api/common/DbusObject.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,34 +3,44 @@
 # Copyright by: P.J. Grochowski
 
 from __future__ import annotations  # TODO: Remove when support dropped for: Python < ?
 
 from typing import Any
 
 from mpris_api.common.DbusObjectSpec import DbusObjectSpec
+from mpris_api.common.DbusPrimitive import DbusPrimitive
+from mpris_api.common.DbusType import IDbusType
+from mpris_api.common.IDbusTypeWrapper import IDbusTypeWrapper
 
 
 class DbusObjectComparisonException(Exception):
     pass
 
 
-class DbusObject:
+class DbusObject(IDbusTypeWrapper[str]):
 
     def __init__(self, value: str) -> None:
         self._value: str = DbusObjectSpec.sanitizeOrThrow(dbusObj=value)
 
     def __eq__(self, other: Any) -> bool:
         return self._value == self._adjustOther(other=other)._value
 
     def __ne__(self, other: Any) -> bool:
         return self._value != self._adjustOther(other=other)._value
 
     def __str__(self) -> str:
         return self._value
 
+    @classmethod
+    def getType(cls) -> IDbusType:
+        return DbusPrimitive.OBJECT
+
+    def getValue(self) -> str:
+        return self._value
+
     @staticmethod
     def _adjustOther(other: Any) -> DbusObject:
         if not isinstance(other, DbusObject):
             raise DbusObjectComparisonException(f'{DbusObject.__name__} can only be compared with another instance of the same type! type(other)="{type(other)}"')
         return other
 
     @classmethod
```

### Comparing `mpris-api-1.1.1/pkg/mpris_api/common/DbusObjectSpec.py` & `mpris-api-1.2.0/pkg/mpris_api/common/DbusObjectSpec.py`

 * *Files identical despite different names*

### Comparing `mpris-api-1.1.1/pkg/mpris_api/common/dbusEnums.py` & `mpris-api-1.2.0/pkg/mpris_api/common/dbusEnums.py`

 * *Files identical despite different names*

### Comparing `mpris-api-1.1.1/pkg/mpris_api/interface/MprisInterfaceBase.py` & `mpris-api-1.2.0/pkg/mpris_api/interface/MprisInterfaceBase.py`

 * *Files identical despite different names*

### Comparing `mpris-api-1.1.1/pkg/mpris_api/interface/MprisInterfaceRoot.py` & `mpris-api-1.2.0/pkg/mpris_api/interface/MprisInterfaceRoot.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright by: P.J. Grochowski
 
 from pathlib import Path
-from typing import no_type_check
+from typing import List
 
 from dbus_next import PropertyAccess
 
 from mpris_api.adapter.IMprisAdapterRoot import IMprisAdapterRoot
-from mpris_api.common.DbusType import DbusType
-from mpris_api.common.dbusDecorators import dbusMethod, dbusProperty
+from mpris_api.common.DbusArray import DbusArray
+from mpris_api.common.DbusPrimitive import DbusPrimitive
+from mpris_api.common.dbusDecorators import dbusInterfaceSignature, dbusMethod, dbusProperty
 from mpris_api.common.dbusEnums import DbusMethodId, DbusPropertyId
 from mpris_api.interface.MprisInterfaceBase import MprisInterfaceBase
 from mpris_api.model.MprisConstant import MprisConstant
 
 
 class MprisRootPropertyId(DbusPropertyId):
     CAN_QUIT = 'CanQuit'
@@ -35,67 +36,103 @@
 class MprisInterfaceRoot(MprisInterfaceBase):
 
     def __init__(self, adapter: IMprisAdapterRoot) -> None:
         super().__init__(MprisConstant.NAME)
         self._adapter: IMprisAdapterRoot = adapter
 
     @dbusProperty(name=MprisRootPropertyId.CAN_QUIT.value, access=PropertyAccess.READ)
-    @no_type_check
-    def canQuit(self) -> DbusType.BOOL:
+    @dbusInterfaceSignature(
+        argTypes=[],
+        returnType=DbusPrimitive.BOOL
+    )
+    def canQuit(self) -> bool:
         return self._adapter.canQuit()
 
     @dbusProperty(name=MprisRootPropertyId.CAN_RAISE.value, access=PropertyAccess.READ)
-    @no_type_check
-    def canRaise(self) -> DbusType.BOOL:
+    @dbusInterfaceSignature(
+        argTypes=[],
+        returnType=DbusPrimitive.BOOL
+    )
+    def canRaise(self) -> bool:
         return self._adapter.canRaise()
 
     @dbusProperty(name=MprisRootPropertyId.CAN_SET_FULL_SCREEN.value, access=PropertyAccess.READ)
-    @no_type_check
-    def canSetFullscreen(self) -> DbusType.BOOL:
+    @dbusInterfaceSignature(
+        argTypes=[],
+        returnType=DbusPrimitive.BOOL
+    )
+    def canSetFullscreen(self) -> bool:
         return self._adapter.canSetFullscreen()
 
     @dbusProperty(name=MprisRootPropertyId.IDENTITY.value, access=PropertyAccess.READ)
-    @no_type_check
-    def identity(self) -> DbusType.STRING:
+    @dbusInterfaceSignature(
+        argTypes=[],
+        returnType=DbusPrimitive.STRING
+    )
+    def identity(self) -> str:
         return self._adapter.getIdentity()
 
     @dbusProperty(name=MprisRootPropertyId.DESKTOP_ENTRY.value, access=PropertyAccess.READ)
-    @no_type_check
-    def desktopEntry(self) -> DbusType.STRING:
+    @dbusInterfaceSignature(
+        argTypes=[],
+        returnType=DbusPrimitive.STRING
+    )
+    def desktopEntry(self) -> str:
         desktopEntry = self._adapter.getDesktopEntry()
         return '' if desktopEntry is None\
             else str(Path(desktopEntry).with_suffix(''))
 
     @dbusProperty(name=MprisRootPropertyId.SUPPORTED_URI_SCHEMES.value, access=PropertyAccess.READ)
-    @no_type_check
-    def supportedUriSchemes(self) -> DbusType.STRING_ARRAY:
+    @dbusInterfaceSignature(
+        argTypes=[],
+        returnType=DbusArray(DbusPrimitive.STRING)
+    )
+    def supportedUriSchemes(self) -> List[str]:
         return self._adapter.getSupportedUriSchemes()
 
     @dbusProperty(name=MprisRootPropertyId.SUPPORTED_MIME_TYPES.value, access=PropertyAccess.READ)
-    @no_type_check
-    def supportedMimeTypes(self) -> DbusType.STRING_ARRAY:
+    @dbusInterfaceSignature(
+        argTypes=[],
+        returnType=DbusArray(DbusPrimitive.STRING)
+    )
+    def supportedMimeTypes(self) -> List[str]:
         return self._adapter.getSupportedMimeTypes()
 
     @dbusProperty(name=MprisRootPropertyId.HAS_TRACK_LIST.value, access=PropertyAccess.READ)
-    @no_type_check
-    def hasTracklist(self) -> DbusType.BOOL:
+    @dbusInterfaceSignature(
+        argTypes=[],
+        returnType=DbusPrimitive.BOOL
+    )
+    def hasTracklist(self) -> bool:
         return self._adapter.hasTracklist()
 
     @dbusProperty(name=MprisRootPropertyId.FULL_SCREEN.value)
-    @no_type_check
-    def fullScreen(self) -> DbusType.BOOL:
+    @dbusInterfaceSignature(
+        argTypes=[],
+        returnType=DbusPrimitive.BOOL
+    )
+    def fullScreen(self) -> bool:
         return self._adapter.isFullScreen()
 
     @fullScreen.setter  # type: ignore
-    @no_type_check
-    def fullScreen(self, value: DbusType.BOOL) -> None:
+    @dbusInterfaceSignature(
+        argTypes=[DbusPrimitive.BOOL],
+        returnType=DbusPrimitive.NOTHING
+    )
+    def fullScreen(self, value: bool) -> None:
         self._adapter.setFullScreen(value=value)
 
     @dbusMethod(name=MprisRootMethodId.QUIT.value)
-    @no_type_check
+    @dbusInterfaceSignature(
+        argTypes=[],
+        returnType=DbusPrimitive.NOTHING
+    )
     def quitApp(self) -> None:
         self._adapter.quitApp()
 
     @dbusMethod(name=MprisRootMethodId.RAISE.value)
-    @no_type_check
+    @dbusInterfaceSignature(
+        argTypes=[],
+        returnType=DbusPrimitive.NOTHING
+    )
     def raiseApp(self) -> None:
         self._adapter.raiseApp()
```

### Comparing `mpris-api-1.1.1/pkg/mpris_api/model/MprisMetaData.py` & `mpris-api-1.2.0/pkg/mpris_api/model/MprisMetaData.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,15 +5,19 @@
 import sys
 from dataclasses import dataclass
 from typing import Dict, List, Optional
 
 from dbus_next import Variant
 from tunit.unit import Microseconds
 
+from mpris_api.common.DbusArray import DbusArray
 from mpris_api.common.DbusObject import DbusObject
+from mpris_api.common.DbusPrimitive import DbusPrimitive
+from mpris_api.common.DbusType import DbusType, IDbusType
+from mpris_api.common.IDbusTypeWrapper import IDbusTypeWrapper
 
 
 class MprisMetaDataField:
     TRACK_ID: str = 'mpris:trackid'
     LENGTH: str = 'mpris:length'
     ART_URL: str = 'mpris:artUrl'
     URL: str = 'xesam:url'
@@ -22,55 +26,66 @@
     ALBUM: str = 'xesam:album'
     ALBUM_ARTIST: str = 'xesam:albumArtist'
     DISC_NUMBER: str = 'xesam:discNumber'
     TRACK_NUMBER: str = 'xesam:trackNumber'
     COMMENT: str = 'xesam:comment'
 
 
-META_DATA_TYPES: Dict[str, str] = {
-    MprisMetaDataField.TRACK_ID: 'o',
-    MprisMetaDataField.LENGTH: 'x',
-    MprisMetaDataField.ART_URL: 's',
-    MprisMetaDataField.URL: 's',
-    MprisMetaDataField.TITLE: 's',
-    MprisMetaDataField.ARTIST: 'as',
-    MprisMetaDataField.ALBUM: 's',
-    MprisMetaDataField.ALBUM_ARTIST: 'as',
-    MprisMetaDataField.DISC_NUMBER: 'i',
-    MprisMetaDataField.TRACK_NUMBER: 'i',
-    MprisMetaDataField.COMMENT: 'as',
+META_DATA_TYPES: Dict[str, IDbusType] = {
+    MprisMetaDataField.TRACK_ID: DbusPrimitive.OBJECT,
+    MprisMetaDataField.LENGTH: DbusPrimitive.INT64,
+    MprisMetaDataField.ART_URL: DbusPrimitive.STRING,
+    MprisMetaDataField.URL: DbusPrimitive.STRING,
+    MprisMetaDataField.TITLE: DbusPrimitive.STRING,
+    MprisMetaDataField.ARTIST: DbusArray(DbusPrimitive.STRING),
+    MprisMetaDataField.ALBUM: DbusPrimitive.STRING,
+    MprisMetaDataField.ALBUM_ARTIST: DbusArray(DbusPrimitive.STRING),
+    MprisMetaDataField.DISC_NUMBER: DbusPrimitive.INT32,
+    MprisMetaDataField.TRACK_NUMBER: DbusPrimitive.INT32,
+    MprisMetaDataField.COMMENT: DbusArray(DbusPrimitive.STRING),
 }
 
 
 @dataclass(frozen=True, **({'kw_only': True} if sys.version_info >= (3, 10) else {}))  # TODO: Adjust when support dropped for: Python < 3.10
-class MprisMetaData:
+class MprisMetaData(IDbusTypeWrapper[Dict[str, Variant]]):
+
     trackId: DbusObject
     length: Optional[Microseconds] = None
     artUrl: Optional[str] = None
     url: Optional[str] = None
     title: Optional[str] = None
     artists: Optional[List[str]] = None
     album: Optional[str] = None
     albumArtists: Optional[List[str]] = None
     discNumber: Optional[int] = None
     trackNumber: Optional[int] = None
     comments: Optional[List[str]] = None
 
-    def toVariantDict(self) -> Dict[str, Variant]:
+    @classmethod
+    def getType(cls) -> IDbusType:
+        return DbusType(
+            signaturePy=Dict[str, Variant],
+            signatureDbus='a{sv}'
+        )
+
+    def getValue(self) -> Dict[str, Variant]:
         metaDataDict = {
-            MprisMetaDataField.TRACK_ID: str(self.trackId),
+            MprisMetaDataField.TRACK_ID: self.trackId.getValue(),
             MprisMetaDataField.LENGTH: int(self.length) if self.length is not None else None,
             MprisMetaDataField.ART_URL: self.artUrl,
             MprisMetaDataField.URL: self.url,
             MprisMetaDataField.TITLE: self.title,
             MprisMetaDataField.ARTIST: self.artists,
             MprisMetaDataField.ALBUM: self.album,
             MprisMetaDataField.ALBUM_ARTIST: self.albumArtists,
             MprisMetaDataField.DISC_NUMBER: self.discNumber,
             MprisMetaDataField.TRACK_NUMBER: self.trackNumber,
             MprisMetaDataField.COMMENT: self.comments,
         }
         return {
-            key: Variant(signature=META_DATA_TYPES[key], value=value)
+            key: Variant(
+                signature=META_DATA_TYPES[key].getSignatureDbus(),
+                value=value
+            )
             for key, value in metaDataDict.items()
             if value is not None
         }
```

### Comparing `mpris-api-1.1.1/pkg/mpris_api/model/MprisPlaylist.py` & `mpris-api-1.2.0/pkg/mpris_api/model/MprisPlaylist.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,35 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright by: P.J. Grochowski
 
 import sys
 from dataclasses import dataclass
-from typing import Optional, Tuple
+from typing import Tuple
 
 from mpris_api.common.DbusObjectSpec import DbusObjectSpec
+from mpris_api.common.DbusType import DbusType, IDbusType
+from mpris_api.common.IDbusTypeWrapper import IDbusTypeWrapper
 
 
 @dataclass(frozen=True, **({'kw_only': True} if sys.version_info >= (3, 10) else {}))   # TODO: Adjust when support dropped for: Python < 3.10
-class MprisPlaylist:
+class MprisPlaylist(IDbusTypeWrapper[Tuple[str, str, str]]):
     playlistId: str
     name: str
-    iconUri: Optional[str] = None
+    iconUri: str = ''
 
     def __post_init__(self) -> None:
         DbusObjectSpec.assertValid(dbusObj=self.playlistId)
 
-    def toTuple(self) -> Tuple[str, str, Optional[str]]:
+    @classmethod
+    def getType(cls) -> IDbusType:
+        return DbusType(
+            signaturePy=Tuple[str, str, str],  # type: ignore
+            signatureDbus='(oss)'
+        )
+
+    def getValue(self) -> Tuple[str, str, str]:
         return (
             self.playlistId,
             self.name,
             self.iconUri
         )
```

### Comparing `mpris-api-1.1.1/pkg/mpris_api.egg-info/PKG-INFO` & `mpris-api-1.2.0/pkg/mpris_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpris-api
-Version: 1.1.1
+Version: 1.2.0
 Summary: Make your multimedia app discoverable by linux desktop.
 Author-email: "P.J. Grochowski" <pawel.grochowski.dev@gmail.com>
 License: MIT
 Project-URL: Repository, https://bitbucket.org/massultidev/mpris-api
 Keywords: mpris,player,multimedia,linux
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mpris-api-1.1.1/pkg/mpris_api.egg-info/SOURCES.txt` & `mpris-api-1.2.0/pkg/mpris_api.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -12,17 +12,21 @@
 pkg/mpris_api.egg-info/requires.txt
 pkg/mpris_api.egg-info/top_level.txt
 pkg/mpris_api/adapter/IMprisAdapterPlayLists.py
 pkg/mpris_api/adapter/IMprisAdapterPlayer.py
 pkg/mpris_api/adapter/IMprisAdapterRoot.py
 pkg/mpris_api/adapter/IMprisAdapterTrackList.py
 pkg/mpris_api/adapter/__init__.py
+pkg/mpris_api/common/DbusArray.py
+pkg/mpris_api/common/DbusMaybe.py
 pkg/mpris_api/common/DbusObject.py
 pkg/mpris_api/common/DbusObjectSpec.py
+pkg/mpris_api/common/DbusPrimitive.py
 pkg/mpris_api/common/DbusType.py
+pkg/mpris_api/common/IDbusTypeWrapper.py
 pkg/mpris_api/common/__init__.py
 pkg/mpris_api/common/dbusDecorators.py
 pkg/mpris_api/common/dbusEnums.py
 pkg/mpris_api/interface/MprisInterfaceBase.py
 pkg/mpris_api/interface/MprisInterfacePlayLists.py
 pkg/mpris_api/interface/MprisInterfacePlayer.py
 pkg/mpris_api/interface/MprisInterfaceRoot.py
```

### Comparing `mpris-api-1.1.1/pyproject.toml` & `mpris-api-1.2.0/pyproject.toml`

 * *Files identical despite different names*

