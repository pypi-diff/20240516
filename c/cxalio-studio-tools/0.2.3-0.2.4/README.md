# Comparing `tmp/cxalio_studio_tools-0.2.3.tar.gz` & `tmp/cxalio_studio_tools-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cxalio_studio_tools-0.2.3.tar", max compression
+gzip compressed data, was "cxalio_studio_tools-0.2.4.tar", max compression
```

## Comparing `cxalio_studio_tools-0.2.3.tar` & `cxalio_studio_tools-0.2.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0    35821 2024-04-16 07:18:25.822233 cxalio_studio_tools-0.2.3/LICENSE
--rw-r--r--   0        0        0     1064 2024-05-15 06:13:48.713797 cxalio_studio_tools-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     1552 2024-05-15 06:13:48.729431 cxalio_studio_tools-0.2.3/README.md
--rw-r--r--   0        0        0      188 2024-05-15 04:56:11.320786 cxalio_studio_tools-0.2.3/src/cx_core/__init__.py
--rw-r--r--   0        0        0      145 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.3/src/cx_core/abstract_app.py
--rw-r--r--   0        0        0      838 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.3/src/cx_core/abstract_env.py
--rw-r--r--   0        0        0     1286 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.3/src/cx_core/app_logger.py
--rw-r--r--   0        0        0     2024 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.3/src/cx_core/datapackage.py
--rw-r--r--   0        0        0     1826 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.3/src/cx_core/ffmpeg_progress_parser.py
--rw-r--r--   0        0        0     1462 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.3/src/cx_core/folder_expander.py
--rw-r--r--   0        0        0      465 2024-05-15 04:56:11.320786 cxalio_studio_tools-0.2.3/src/cx_core/osinfo.py
--rw-r--r--   0        0        0     1421 2024-05-15 04:56:11.321788 cxalio_studio_tools-0.2.3/src/cx_core/tag_replacer.py
--rw-r--r--   0        0        0     2991 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.3/src/cx_core/timecode.py
--rw-r--r--   0        0        0     1640 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.3/src/cx_core/timepoint.py
--rw-r--r--   0        0        0      466 2024-05-15 04:56:11.321788 cxalio_studio_tools-0.2.3/src/cx_core/tui_elements.py
--rw-r--r--   0        0        0     2813 2024-05-15 05:48:14.513139 cxalio_studio_tools-0.2.3/src/cx_core/utils.py
--rw-r--r--   0        0        0      101 2024-05-15 04:56:11.321788 cxalio_studio_tools-0.2.3/src/cx_subtitle/__init__.py
--rw-r--r--   0        0        0     4611 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.3/src/cx_subtitle/loader.py
--rw-r--r--   0        0        0     5394 2024-05-15 04:56:11.322788 cxalio_studio_tools-0.2.3/src/cx_subtitle/saver.py
--rw-r--r--   0        0        0      731 2024-05-15 04:56:11.322788 cxalio_studio_tools-0.2.3/src/cx_subtitle/subtitle.py
--rw-r--r--   0        0        0     2858 2024-05-15 04:56:11.322788 cxalio_studio_tools-0.2.3/src/cx_subtitle/subtitle_formatter.py
--rw-r--r--   0        0        0       35 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.3/src/media_killer/__init__.py
--rw-r--r--   0        0        0     1312 2024-05-15 04:56:11.322788 cxalio_studio_tools-0.2.3/src/media_killer/env.py
--rw-r--r--   0        0        0     2958 2024-05-15 04:56:11.323789 cxalio_studio_tools-0.2.3/src/media_killer/example_project.toml
--rw-r--r--   0        0        0      364 2024-05-15 04:56:11.323789 cxalio_studio_tools-0.2.3/src/media_killer/exceptions.py
--rw-r--r--   0        0        0     5453 2024-05-15 04:56:11.323789 cxalio_studio_tools-0.2.3/src/media_killer/help.md
--rw-r--r--   0        0        0     7970 2024-05-15 06:13:48.702290 cxalio_studio_tools-0.2.3/src/media_killer/media_killer_app.py
--rw-r--r--   0        0        0     6844 2024-05-15 06:12:37.164339 cxalio_studio_tools-0.2.3/src/media_killer/mission.py
--rw-r--r--   0        0        0     1269 2024-05-15 04:56:11.324789 cxalio_studio_tools-0.2.3/src/media_killer/option_package.py
--rw-r--r--   0        0        0     3827 2024-05-15 04:56:11.324789 cxalio_studio_tools-0.2.3/src/media_killer/planner.py
--rw-r--r--   0        0        0     3484 2024-05-15 06:06:25.055916 cxalio_studio_tools-0.2.3/src/media_killer/profile_loader.py
--rw-r--r--   0        0        0     1762 2024-05-15 04:56:11.325789 cxalio_studio_tools-0.2.3/src/media_killer/script_writer.py
--rw-r--r--   0        0        0     2793 2024-05-15 04:56:11.325789 cxalio_studio_tools-0.2.3/src/media_killer/source_adapter.py
--rw-r--r--   0        0        0     4092 2024-05-15 06:12:37.158335 cxalio_studio_tools-0.2.3/src/media_killer/transcoder.py
--rw-r--r--   0        0        0       30 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.3/src/sub_conv/__init__.py
--rw-r--r--   0        0        0     1132 2024-05-15 04:56:11.326789 cxalio_studio_tools-0.2.3/src/sub_conv/env.py
--rw-r--r--   0        0        0       44 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.3/src/sub_conv/exceptions.py
--rw-r--r--   0        0        0     3316 2024-05-15 04:56:11.326789 cxalio_studio_tools-0.2.3/src/sub_conv/help.md
--rw-r--r--   0        0        0     9947 2024-05-15 04:56:11.326789 cxalio_studio_tools-0.2.3/src/sub_conv/subconv_app.py
--rw-r--r--   0        0        0     1624 2024-05-15 04:56:11.326789 cxalio_studio_tools-0.2.3/src/sub_conv/subtitle_translator.py
--rw-r--r--   0        0        0        0 2024-05-15 04:56:11.326789 cxalio_studio_tools-0.2.3/src/systools/__init__.py
--rw-r--r--   0        0        0      278 2024-05-15 04:56:11.328045 cxalio_studio_tools-0.2.3/src/systools/env.py
--rw-r--r--   0        0        0     3722 2024-05-15 04:56:11.328045 cxalio_studio_tools-0.2.3/src/systools/update_githubhosts.py
--rw-r--r--   0        0        0     2443 1970-01-01 00:00:00.000000 cxalio_studio_tools-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    35821 2024-04-16 07:18:25.822233 cxalio_studio_tools-0.2.4/LICENSE
+-rw-r--r--   0        0        0     1064 2024-05-15 06:20:20.649688 cxalio_studio_tools-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     1552 2024-05-15 06:20:32.458521 cxalio_studio_tools-0.2.4/README.md
+-rw-r--r--   0        0        0      188 2024-05-15 04:56:11.320786 cxalio_studio_tools-0.2.4/src/cx_core/__init__.py
+-rw-r--r--   0        0        0      145 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.4/src/cx_core/abstract_app.py
+-rw-r--r--   0        0        0      838 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.4/src/cx_core/abstract_env.py
+-rw-r--r--   0        0        0     1286 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.4/src/cx_core/app_logger.py
+-rw-r--r--   0        0        0     2024 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.4/src/cx_core/datapackage.py
+-rw-r--r--   0        0        0     1826 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.4/src/cx_core/ffmpeg_progress_parser.py
+-rw-r--r--   0        0        0     1462 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.4/src/cx_core/folder_expander.py
+-rw-r--r--   0        0        0      465 2024-05-15 04:56:11.320786 cxalio_studio_tools-0.2.4/src/cx_core/osinfo.py
+-rw-r--r--   0        0        0     1421 2024-05-15 04:56:11.321788 cxalio_studio_tools-0.2.4/src/cx_core/tag_replacer.py
+-rw-r--r--   0        0        0     2991 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.4/src/cx_core/timecode.py
+-rw-r--r--   0        0        0     1640 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.4/src/cx_core/timepoint.py
+-rw-r--r--   0        0        0      466 2024-05-15 04:56:11.321788 cxalio_studio_tools-0.2.4/src/cx_core/tui_elements.py
+-rw-r--r--   0        0        0     2813 2024-05-15 05:48:14.513139 cxalio_studio_tools-0.2.4/src/cx_core/utils.py
+-rw-r--r--   0        0        0      101 2024-05-15 04:56:11.321788 cxalio_studio_tools-0.2.4/src/cx_subtitle/__init__.py
+-rw-r--r--   0        0        0     4611 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.4/src/cx_subtitle/loader.py
+-rw-r--r--   0        0        0     5394 2024-05-15 04:56:11.322788 cxalio_studio_tools-0.2.4/src/cx_subtitle/saver.py
+-rw-r--r--   0        0        0      731 2024-05-15 04:56:11.322788 cxalio_studio_tools-0.2.4/src/cx_subtitle/subtitle.py
+-rw-r--r--   0        0        0     2858 2024-05-15 04:56:11.322788 cxalio_studio_tools-0.2.4/src/cx_subtitle/subtitle_formatter.py
+-rw-r--r--   0        0        0       35 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.4/src/media_killer/__init__.py
+-rw-r--r--   0        0        0     1312 2024-05-15 04:56:11.322788 cxalio_studio_tools-0.2.4/src/media_killer/env.py
+-rw-r--r--   0        0        0     2958 2024-05-15 04:56:11.323789 cxalio_studio_tools-0.2.4/src/media_killer/example_project.toml
+-rw-r--r--   0        0        0      364 2024-05-15 04:56:11.323789 cxalio_studio_tools-0.2.4/src/media_killer/exceptions.py
+-rw-r--r--   0        0        0     5453 2024-05-15 04:56:11.323789 cxalio_studio_tools-0.2.4/src/media_killer/help.md
+-rw-r--r--   0        0        0     7970 2024-05-15 06:20:32.481259 cxalio_studio_tools-0.2.4/src/media_killer/media_killer_app.py
+-rw-r--r--   0        0        0     6865 2024-05-15 06:19:40.286547 cxalio_studio_tools-0.2.4/src/media_killer/mission.py
+-rw-r--r--   0        0        0     1269 2024-05-15 04:56:11.324789 cxalio_studio_tools-0.2.4/src/media_killer/option_package.py
+-rw-r--r--   0        0        0     3827 2024-05-15 04:56:11.324789 cxalio_studio_tools-0.2.4/src/media_killer/planner.py
+-rw-r--r--   0        0        0     3484 2024-05-15 06:06:25.055916 cxalio_studio_tools-0.2.4/src/media_killer/profile_loader.py
+-rw-r--r--   0        0        0     1762 2024-05-15 04:56:11.325789 cxalio_studio_tools-0.2.4/src/media_killer/script_writer.py
+-rw-r--r--   0        0        0     2793 2024-05-15 04:56:11.325789 cxalio_studio_tools-0.2.4/src/media_killer/source_adapter.py
+-rw-r--r--   0        0        0     4092 2024-05-15 06:12:37.158335 cxalio_studio_tools-0.2.4/src/media_killer/transcoder.py
+-rw-r--r--   0        0        0       30 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.4/src/sub_conv/__init__.py
+-rw-r--r--   0        0        0     1132 2024-05-15 04:56:11.326789 cxalio_studio_tools-0.2.4/src/sub_conv/env.py
+-rw-r--r--   0        0        0       44 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.4/src/sub_conv/exceptions.py
+-rw-r--r--   0        0        0     3316 2024-05-15 04:56:11.326789 cxalio_studio_tools-0.2.4/src/sub_conv/help.md
+-rw-r--r--   0        0        0     9947 2024-05-15 04:56:11.326789 cxalio_studio_tools-0.2.4/src/sub_conv/subconv_app.py
+-rw-r--r--   0        0        0     1624 2024-05-15 04:56:11.326789 cxalio_studio_tools-0.2.4/src/sub_conv/subtitle_translator.py
+-rw-r--r--   0        0        0        0 2024-05-15 04:56:11.326789 cxalio_studio_tools-0.2.4/src/systools/__init__.py
+-rw-r--r--   0        0        0      278 2024-05-15 04:56:11.328045 cxalio_studio_tools-0.2.4/src/systools/env.py
+-rw-r--r--   0        0        0     3722 2024-05-15 04:56:11.328045 cxalio_studio_tools-0.2.4/src/systools/update_githubhosts.py
+-rw-r--r--   0        0        0     2443 1970-01-01 00:00:00.000000 cxalio_studio_tools-0.2.4/PKG-INFO
```

### Comparing `cxalio_studio_tools-0.2.3/LICENSE` & `cxalio_studio_tools-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.3/pyproject.toml` & `cxalio_studio_tools-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cxalio-studio-tools"
-version = "0.2.3"
+version = "0.2.4"
 description = "Scripts for po studio made by cxalio"
 authors = ["xiii_1991 <xiii_1991@163.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 packages = [
     { include = "cx_core", from = "src" },
     { include = "media_killer", from = "src" },
```

### Comparing `cxalio_studio_tools-0.2.3/README.md` & `cxalio_studio_tools-0.2.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 ## To-do
 
 - media-inspector 解析媒体信息
 
 ## Change-log
 
-### 0.2.3
+### 0.2.4
 mediakiller:
 
 - 修复了 duration 无法解析时崩溃的 bug。
 - 修复了目标目录解析为当前目录的错误。
 - 增加了扩展名检查，强制生成的配置文件扩展名为`toml`。
 - 修改了当前任务进度条的样式，减少闪烁。
 - 修复了不可覆盖输出文件时，转码卡住的问题。
```

### Comparing `cxalio_studio_tools-0.2.3/src/cx_core/abstract_env.py` & `cxalio_studio_tools-0.2.4/src/cx_core/abstract_env.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.3/src/cx_core/app_logger.py` & `cxalio_studio_tools-0.2.4/src/cx_core/app_logger.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.3/src/cx_core/datapackage.py` & `cxalio_studio_tools-0.2.4/src/cx_core/datapackage.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.3/src/cx_core/ffmpeg_progress_parser.py` & `cxalio_studio_tools-0.2.4/src/cx_core/ffmpeg_progress_parser.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.3/src/cx_core/folder_expander.py` & `cxalio_studio_tools-0.2.4/src/cx_core/folder_expander.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.3/src/cx_core/tag_replacer.py` & `cxalio_studio_tools-0.2.4/src/cx_core/tag_replacer.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.3/src/cx_core/timecode.py` & `cxalio_studio_tools-0.2.4/src/cx_core/timecode.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.3/src/cx_core/timepoint.py` & `cxalio_studio_tools-0.2.4/src/cx_core/timepoint.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.3/src/cx_core/utils.py` & `cxalio_studio_tools-0.2.4/src/cx_core/utils.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.3/src/cx_subtitle/loader.py` & `cxalio_studio_tools-0.2.4/src/cx_subtitle/loader.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.3/src/cx_subtitle/saver.py` & `cxalio_studio_tools-0.2.4/src/cx_subtitle/saver.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.3/src/cx_subtitle/subtitle.py` & `cxalio_studio_tools-0.2.4/src/cx_subtitle/subtitle.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.3/src/cx_subtitle/subtitle_formatter.py` & `cxalio_studio_tools-0.2.4/src/cx_subtitle/subtitle_formatter.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.3/src/media_killer/env.py` & `cxalio_studio_tools-0.2.4/src/media_killer/env.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.3/src/media_killer/example_project.toml` & `cxalio_studio_tools-0.2.4/src/media_killer/example_project.toml`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.3/src/media_killer/help.md` & `cxalio_studio_tools-0.2.4/src/media_killer/help.md`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.3/src/media_killer/media_killer_app.py` & `cxalio_studio_tools-0.2.4/src/media_killer/media_killer_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from .planner import Planner
 from .profile_loader import ProfileLoader, ProfileNoFoundError
 from .script_writer import ScriptWriter
 from .transcoder import Transcoder
 
 
 class MediaKillerApp(AbstractApp):
-    APP_VERSION = '0.2.3'
+    APP_VERSION = '0.2.4'
     APP_NAME = 'mediakiller'
 
     def __init__(self):
         super(MediaKillerApp, self).__init__()
         self.global_task = None
 
         parser = ArgumentParser(prog=MediaKillerApp.APP_NAME, formatter_class=RichHelpFormatter,
```

### Comparing `cxalio_studio_tools-0.2.3/src/media_killer/mission.py` & `cxalio_studio_tools-0.2.4/src/media_killer/mission.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,14 +176,15 @@
         """检测全部目标文件是否可写入"""
         if self.profile.general.overwrite_existed:
             return True
         for o in self.outputs:
             file = o.filename
             if file.exists():
                 return False
+        return True
 
 
 class MissionMaker:
     def __init__(self, profile):
         self.profile = profile
 
     def __call__(self, sources: [Path]):
```

### Comparing `cxalio_studio_tools-0.2.3/src/media_killer/option_package.py` & `cxalio_studio_tools-0.2.4/src/media_killer/option_package.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.3/src/media_killer/planner.py` & `cxalio_studio_tools-0.2.4/src/media_killer/planner.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.3/src/media_killer/profile_loader.py` & `cxalio_studio_tools-0.2.4/src/media_killer/profile_loader.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.3/src/media_killer/script_writer.py` & `cxalio_studio_tools-0.2.4/src/media_killer/script_writer.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.3/src/media_killer/source_adapter.py` & `cxalio_studio_tools-0.2.4/src/media_killer/source_adapter.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.3/src/media_killer/transcoder.py` & `cxalio_studio_tools-0.2.4/src/media_killer/transcoder.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.3/src/sub_conv/env.py` & `cxalio_studio_tools-0.2.4/src/sub_conv/env.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.3/src/sub_conv/help.md` & `cxalio_studio_tools-0.2.4/src/sub_conv/help.md`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.3/src/sub_conv/subconv_app.py` & `cxalio_studio_tools-0.2.4/src/sub_conv/subconv_app.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.3/src/sub_conv/subtitle_translator.py` & `cxalio_studio_tools-0.2.4/src/sub_conv/subtitle_translator.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.3/src/systools/update_githubhosts.py` & `cxalio_studio_tools-0.2.4/src/systools/update_githubhosts.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.3/PKG-INFO` & `cxalio_studio_tools-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cxalio-studio-tools
-Version: 0.2.3
+Version: 0.2.4
 Summary: Scripts for po studio made by cxalio
 Home-page: https://gitee.com/xiii_1991/cxalio-studio-tools
 License: GPL-3.0-or-later
 Keywords: ffmpeg,tool
 Author: xiii_1991
 Author-email: xiii_1991@163.com
 Requires-Python: >=3.11,<4.0
@@ -58,15 +58,15 @@
 
 ## To-do
 
 - media-inspector 解析媒体信息
 
 ## Change-log
 
-### 0.2.3
+### 0.2.4
 mediakiller:
 
 - 修复了 duration 无法解析时崩溃的 bug。
 - 修复了目标目录解析为当前目录的错误。
 - 增加了扩展名检查，强制生成的配置文件扩展名为`toml`。
 - 修改了当前任务进度条的样式，减少闪烁。
 - 修复了不可覆盖输出文件时，转码卡住的问题。
```

