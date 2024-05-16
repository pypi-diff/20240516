# Comparing `tmp/anipy_api-3.0.3.tar.gz` & `tmp/anipy_api-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anipy_api-3.0.3.tar", max compression
+gzip compressed data, was "anipy_api-3.0.4.tar", max compression
```

## Comparing `anipy_api-3.0.3.tar` & `anipy_api-3.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      227 2024-05-14 16:34:45.680884 anipy_api-3.0.3/README.md
--rw-r--r--   0        0        0      847 2024-05-14 16:34:45.680884 anipy_api-3.0.3/pyproject.toml
--rw-r--r--   0        0        0       48 2024-05-14 16:34:45.680884 anipy_api-3.0.3/src/anipy_api/__init__.py
--rw-r--r--   0        0        0     5417 2024-05-14 16:34:45.680884 anipy_api-3.0.3/src/anipy_api/anime.py
--rw-r--r--   0        0        0    11474 2024-05-14 16:34:45.680884 anipy_api-3.0.3/src/anipy_api/download.py
--rw-r--r--   0        0        0     2765 2024-05-14 16:34:45.680884 anipy_api-3.0.3/src/anipy_api/error.py
--rw-r--r--   0        0        0     7953 2024-05-14 16:34:45.680884 anipy_api-3.0.3/src/anipy_api/locallist.py
--rw-r--r--   0        0        0    20790 2024-05-14 16:34:45.680884 anipy_api-3.0.3/src/anipy_api/mal.py
--rw-r--r--   0        0        0      132 2024-05-14 16:34:45.680884 anipy_api-3.0.3/src/anipy_api/player/__init__.py
--rw-r--r--   0        0        0     5499 2024-05-14 16:34:45.680884 anipy_api-3.0.3/src/anipy_api/player/base.py
--rw-r--r--   0        0        0     1692 2024-05-14 16:34:45.680884 anipy_api-3.0.3/src/anipy_api/player/player.py
--rw-r--r--   0        0        0      267 2024-05-14 16:34:45.680884 anipy_api-3.0.3/src/anipy_api/player/players/__init__.py
--rw-r--r--   0        0        0     1147 2024-05-14 16:34:45.680884 anipy_api-3.0.3/src/anipy_api/player/players/mpv.py
--rw-r--r--   0        0        0     2669 2024-05-14 16:34:45.680884 anipy_api-3.0.3/src/anipy_api/player/players/mpv_control.py
--rw-r--r--   0        0        0      941 2024-05-14 16:34:45.680884 anipy_api-3.0.3/src/anipy_api/player/players/syncplay.py
--rw-r--r--   0        0        0      918 2024-05-14 16:34:45.680884 anipy_api-3.0.3/src/anipy_api/player/players/vlc.py
--rw-r--r--   0        0        0      628 2024-05-14 16:34:45.680884 anipy_api-3.0.3/src/anipy_api/provider/__init__.py
--rw-r--r--   0        0        0     5321 2024-05-14 16:34:45.680884 anipy_api-3.0.3/src/anipy_api/provider/base.py
--rw-r--r--   0        0        0     3397 2024-05-14 16:34:45.680884 anipy_api-3.0.3/src/anipy_api/provider/filter.py
--rw-r--r--   0        0        0     1543 2024-05-14 16:34:45.680884 anipy_api-3.0.3/src/anipy_api/provider/provider.py
--rw-r--r--   0        0        0       96 2024-05-14 16:34:45.680884 anipy_api-3.0.3/src/anipy_api/provider/providers/__init__.py
--rw-r--r--   0        0        0    12230 2024-05-14 16:34:45.680884 anipy_api-3.0.3/src/anipy_api/provider/providers/gogo_provider.py
--rw-r--r--   0        0        0     1482 2024-05-14 16:34:45.680884 anipy_api-3.0.3/src/anipy_api/provider/utils.py
--rw-r--r--   0        0        0     1452 1970-01-01 00:00:00.000000 anipy_api-3.0.3/PKG-INFO
+-rw-r--r--   0        0        0      227 2024-05-16 14:00:40.760930 anipy_api-3.0.4/README.md
+-rw-r--r--   0        0        0      847 2024-05-16 14:00:40.760930 anipy_api-3.0.4/pyproject.toml
+-rw-r--r--   0        0        0       48 2024-05-16 14:00:40.760930 anipy_api-3.0.4/src/anipy_api/__init__.py
+-rw-r--r--   0        0        0     5417 2024-05-16 14:00:40.760930 anipy_api-3.0.4/src/anipy_api/anime.py
+-rw-r--r--   0        0        0    11550 2024-05-16 14:00:40.760930 anipy_api-3.0.4/src/anipy_api/download.py
+-rw-r--r--   0        0        0     2765 2024-05-16 14:00:40.760930 anipy_api-3.0.4/src/anipy_api/error.py
+-rw-r--r--   0        0        0     7953 2024-05-16 14:00:40.760930 anipy_api-3.0.4/src/anipy_api/locallist.py
+-rw-r--r--   0        0        0    20790 2024-05-16 14:00:40.760930 anipy_api-3.0.4/src/anipy_api/mal.py
+-rw-r--r--   0        0        0      132 2024-05-16 14:00:40.760930 anipy_api-3.0.4/src/anipy_api/player/__init__.py
+-rw-r--r--   0        0        0     5499 2024-05-16 14:00:40.760930 anipy_api-3.0.4/src/anipy_api/player/base.py
+-rw-r--r--   0        0        0     1692 2024-05-16 14:00:40.760930 anipy_api-3.0.4/src/anipy_api/player/player.py
+-rw-r--r--   0        0        0      267 2024-05-16 14:00:40.764930 anipy_api-3.0.4/src/anipy_api/player/players/__init__.py
+-rw-r--r--   0        0        0     1147 2024-05-16 14:00:40.764930 anipy_api-3.0.4/src/anipy_api/player/players/mpv.py
+-rw-r--r--   0        0        0     2651 2024-05-16 14:00:40.764930 anipy_api-3.0.4/src/anipy_api/player/players/mpv_control.py
+-rw-r--r--   0        0        0      941 2024-05-16 14:00:40.764930 anipy_api-3.0.4/src/anipy_api/player/players/syncplay.py
+-rw-r--r--   0        0        0      918 2024-05-16 14:00:40.764930 anipy_api-3.0.4/src/anipy_api/player/players/vlc.py
+-rw-r--r--   0        0        0      628 2024-05-16 14:00:40.764930 anipy_api-3.0.4/src/anipy_api/provider/__init__.py
+-rw-r--r--   0        0        0     5321 2024-05-16 14:00:40.764930 anipy_api-3.0.4/src/anipy_api/provider/base.py
+-rw-r--r--   0        0        0     3397 2024-05-16 14:00:40.764930 anipy_api-3.0.4/src/anipy_api/provider/filter.py
+-rw-r--r--   0        0        0     1543 2024-05-16 14:00:40.764930 anipy_api-3.0.4/src/anipy_api/provider/provider.py
+-rw-r--r--   0        0        0       96 2024-05-16 14:00:40.764930 anipy_api-3.0.4/src/anipy_api/provider/providers/__init__.py
+-rw-r--r--   0        0        0    12230 2024-05-16 14:00:40.764930 anipy_api-3.0.4/src/anipy_api/provider/providers/gogo_provider.py
+-rw-r--r--   0        0        0     1482 2024-05-16 14:00:40.764930 anipy_api-3.0.4/src/anipy_api/provider/utils.py
+-rw-r--r--   0        0        0     1452 1970-01-01 00:00:00.000000 anipy_api-3.0.4/PKG-INFO
```

### Comparing `anipy_api-3.0.3/pyproject.toml` & `anipy_api-3.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anipy-api"
-version = "3.0.3"
+version = "3.0.4"
 description = "api for anipy-cli"
 authors = ["sdaqo <sdaqo.dev@protonmail.com>"]
 license = "GPL-3.0"
 repository = "https://github.com/sdaqo/anipy-cli"
 homepage = "https://sdaqo.github.io/anipy-cli"
 documentation = "https://sdaqo.github.io/anipy-cli/getting-started-api"
 keywords = ["anime", "api"]
```

### Comparing `anipy_api-3.0.3/src/anipy_api/anime.py` & `anipy_api-3.0.4/src/anipy_api/anime.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.3/src/anipy_api/download.py` & `anipy_api-3.0.4/src/anipy_api/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     def _get_valid_pathname(name: str):
         if sys.platform == "win32":
             INVALID_CHARS = ["\\", "/", ":", "*", "?", "<", ">", "|", '"', "."]
         else:
             INVALID_CHARS = [".", "/"]
 
         name = "".join(
-            [i for i in name if i.isascii() and not i in INVALID_CHARS]
+            [i for i in name if i.isascii() and i not in INVALID_CHARS]
         )  # Verify all chars are ascii (eject if not)
 
         return name
 
     def m3u8_download(self, stream: "ProviderStream", download_path: Path) -> Path:
         """Download a m3u8/hls stream to a specified download path in a ts container.
 
@@ -104,15 +104,17 @@
 
         counter = 0
 
         def download_ts(segment: m3u8.Segment):
             nonlocal counter
             url = urljoin(segment.base_uri, segment.uri)
             segment_uri = Path(segment.uri)
-            fname = (temp_folder / self._get_valid_pathname(segment_uri.stem)).with_suffix(segment_uri.suffix)
+            fname = (
+                temp_folder / self._get_valid_pathname(segment_uri.stem)
+            ).with_suffix(segment_uri.suffix)
             try:
                 res = self._session.get(str(url))
                 res.raise_for_status()
 
                 with fname.open("wb") as fout:
                     fout.write(res.content)
 
@@ -141,15 +143,17 @@
 
             self._info_callback("Parts Downloaded")
 
             self._info_callback("Merging Parts...")
             with download_path.open("wb") as merged:
                 for segment in m3u8_content.segments:
                     uri = Path(segment.uri)
-                    fname = (temp_folder / self._get_valid_pathname(uri.stem)).with_suffix(uri.suffix)
+                    fname = (
+                        temp_folder / self._get_valid_pathname(uri.stem)
+                    ).with_suffix(uri.suffix)
                     if not fname.is_file():
                         raise DownloadError(
                             f"Could not merge, missing a segment of this playlist: {stream.url}"
                         )
 
                     with fname.open("rb") as mergefile:
                         shutil.copyfileobj(mergefile, merged)
```

### Comparing `anipy_api-3.0.3/src/anipy_api/error.py` & `anipy_api-3.0.4/src/anipy_api/error.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.3/src/anipy_api/locallist.py` & `anipy_api-3.0.4/src/anipy_api/locallist.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.3/src/anipy_api/mal.py` & `anipy_api-3.0.4/src/anipy_api/mal.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.3/src/anipy_api/player/base.py` & `anipy_api-3.0.4/src/anipy_api/player/base.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.3/src/anipy_api/player/player.py` & `anipy_api-3.0.4/src/anipy_api/player/player.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.3/src/anipy_api/player/players/mpv.py` & `anipy_api-3.0.4/src/anipy_api/player/players/mpv.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.3/src/anipy_api/player/players/mpv_control.py` & `anipy_api-3.0.4/src/anipy_api/player/players/mpv_control.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,54 +5,54 @@
 if TYPE_CHECKING:
     from anipy_api.provider import ProviderStream
     from anipy_api.anime import Anime
 
 
 class MpvControllable(PlayerBase):
     """This player can be controlled and it also does not close if
-    the media is changed, the window stays open until `kill_player` is called. 
+    the media is changed, the window stays open until `kill_player` is called.
     You need libmpv for this, check the [python-mpv](https://github.com/jaseg/python-mpv?tab=readme-ov-file#requirements)
     project's requirements to know where to get it.
 
     For detailed documentation about the functions have a look at the [base class][anipy_api.player.base.PlayerBase].
 
     If you want to use the extra features of the controllable player look
     [here](https://github.com/jaseg/python-mpv?tab=readme-ov-file#usage)
     for documentation (or use your LSP), the python-mpv mpv instance lives in the mpv attribute.
 
     Attributes:
         mpv: The python-mpv mpv instance
     """
 
-    def __init__(self, play_callback: Optional[PlayCallback] = None, **mpv_args: Optional[Any]):
+    def __init__(
+        self, play_callback: Optional[PlayCallback] = None, **mpv_args: Optional[Any]
+    ):
         """__init__ of MpvControllable
 
         Args:
             play_callback: Callback called upon starting to play a title with `play_title`
             **mpv_args: Arguments passed to the MPV instance check the [python-mpv repo](https://github.com/jaseg/python-mpv?tab=readme-ov-file#usage)
-                or check the [official list of arguments](https://mpv.io/manual/master/#properties). There are some default arguments set, if you specify 
+                or check the [official list of arguments](https://mpv.io/manual/master/#properties). There are some default arguments set, if you specify
                 any arguments here, all the defaults will be discarded and this will be used instead.
         """
         super().__init__(play_callback=play_callback)
 
         # I know this is a crime, but pytohn-mpv loads the so/dll on import and this will break all the stuff for people that do not have that.
         from mpv import MPV
-        
+
         if len(mpv_args) <= 1:
             mpv_args = {
                 "input_default_bindings": True,
                 "input_vo_keyboard": True,
                 "force_window": "immediate",
                 "title": "MPV - Receiving Links from anipy-cli",
                 "osc": "True",
             }
 
-        self.mpv = MPV(
-            **mpv_args
-        )
+        self.mpv = MPV(**mpv_args)
 
     def play_title(self, anime: "Anime", stream: "ProviderStream"):
         self.mpv.force_media_title = self._get_media_title(anime, stream)
 
         self.mpv.play(stream.url)
 
         self._call_play_callback(anime, stream)
```

### Comparing `anipy_api-3.0.3/src/anipy_api/player/players/syncplay.py` & `anipy_api-3.0.4/src/anipy_api/player/players/syncplay.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.3/src/anipy_api/player/players/vlc.py` & `anipy_api-3.0.4/src/anipy_api/player/players/vlc.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.3/src/anipy_api/provider/__init__.py` & `anipy_api-3.0.4/src/anipy_api/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.3/src/anipy_api/provider/base.py` & `anipy_api-3.0.4/src/anipy_api/provider/base.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.3/src/anipy_api/provider/filter.py` & `anipy_api-3.0.4/src/anipy_api/provider/filter.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.3/src/anipy_api/provider/provider.py` & `anipy_api-3.0.4/src/anipy_api/provider/provider.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.3/src/anipy_api/provider/providers/gogo_provider.py` & `anipy_api-3.0.4/src/anipy_api/provider/providers/gogo_provider.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.3/src/anipy_api/provider/utils.py` & `anipy_api-3.0.4/src/anipy_api/provider/utils.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.3/PKG-INFO` & `anipy_api-3.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anipy-api
-Version: 3.0.3
+Version: 3.0.4
 Summary: api for anipy-cli
 Home-page: https://sdaqo.github.io/anipy-cli
 License: GPL-3.0
 Keywords: anime,api
 Author: sdaqo
 Author-email: sdaqo.dev@protonmail.com
 Requires-Python: >=3.9,<4.0
```

