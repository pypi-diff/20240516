# Comparing `tmp/sinarax-1.1.7.tar.gz` & `tmp/sinarax-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinarax-1.1.7.tar", max compression
+gzip compressed data, was "sinarax-1.1.8.tar", max compression
```

## Comparing `sinarax-1.1.7.tar` & `sinarax-1.1.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    11357 2024-04-24 12:46:14.627865 sinarax-1.1.7/LICENSE
--rw-r--r--   0        0        0     2212 2024-04-24 12:46:14.627865 sinarax-1.1.7/README.md
--rw-r--r--   0        0        0     1129 2024-04-24 12:46:14.627865 sinarax-1.1.7/pyproject.toml
--rw-r--r--   0        0        0       61 2024-04-24 12:46:14.627865 sinarax-1.1.7/sinaraX/__init__.py
--rw-r--r--   0        0        0      428 2024-04-24 12:46:14.627865 sinarax-1.1.7/sinaraX/__main__.py
--rw-r--r--   0        0        0       93 2024-04-24 12:46:14.627865 sinarax-1.1.7/sinaraX/_version.py
--rw-r--r--   0        0        0      134 2024-04-24 12:46:14.627865 sinarax-1.1.7/sinaraX/screens/__init__.py
--rw-r--r--   0        0        0       68 2024-04-24 12:46:14.627865 sinarax-1.1.7/sinaraX/screens/file_screen/__init__.py
--rw-r--r--   0        0        0     3416 2024-04-24 12:46:14.627865 sinarax-1.1.7/sinaraX/screens/file_screen/file_tree.py
--rw-r--r--   0        0        0     6544 2024-04-24 12:46:14.627865 sinarax-1.1.7/sinaraX/screens/main.py
--rw-r--r--   0        0        0     6278 2024-04-24 12:46:14.627865 sinarax-1.1.7/sinaraX/screens/running.py
--rw-r--r--   0        0        0    13814 2024-04-24 12:46:14.627865 sinarax-1.1.7/sinaraX/screens/server.py
--rw-r--r--   0        0        0     2948 2024-04-24 12:46:14.627865 sinarax-1.1.7/sinaraX/screens/server_cfg.py
--rw-r--r--   0        0        0      963 2024-04-24 12:46:14.627865 sinarax-1.1.7/sinaraX/screens/style.css
--rw-r--r--   0        0        0     2403 2024-04-24 12:46:14.627865 sinarax-1.1.7/sinaraX/screens/update.py
--rw-r--r--   0        0        0      507 2024-04-24 12:46:14.627865 sinarax-1.1.7/sinaraX/screens/utils/__init__.py
--rw-r--r--   0        0        0     4616 2024-04-24 12:46:14.627865 sinarax-1.1.7/sinaraX/screens/utils/config.py
--rw-r--r--   0        0        0     5721 2024-04-24 12:46:14.627865 sinarax-1.1.7/sinaraX/screens/utils/infra.py
--rw-r--r--   0        0        0     1564 2024-04-24 12:46:14.627865 sinarax-1.1.7/sinaraX/screens/utils/process.py
--rw-r--r--   0        0        0      847 2024-04-24 12:46:14.627865 sinarax-1.1.7/sinaraX/screens/utils/sinara_server_utils.py
--rw-r--r--   0        0        0     3214 1970-01-01 00:00:00.000000 sinarax-1.1.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-16 07:51:03.361892 sinarax-1.1.8/LICENSE
+-rw-r--r--   0        0        0     2212 2024-05-16 07:51:03.361892 sinarax-1.1.8/README.md
+-rw-r--r--   0        0        0     1129 2024-05-16 07:51:03.361892 sinarax-1.1.8/pyproject.toml
+-rw-r--r--   0        0        0       61 2024-05-16 07:51:03.361892 sinarax-1.1.8/sinaraX/__init__.py
+-rw-r--r--   0        0        0      428 2024-05-16 07:51:03.361892 sinarax-1.1.8/sinaraX/__main__.py
+-rw-r--r--   0        0        0       93 2024-05-16 07:51:03.361892 sinarax-1.1.8/sinaraX/_version.py
+-rw-r--r--   0        0        0       85 2024-05-16 07:51:03.361892 sinarax-1.1.8/sinaraX/screens/__init__.py
+-rw-r--r--   0        0        0       68 2024-05-16 07:51:03.361892 sinarax-1.1.8/sinaraX/screens/file_screen/__init__.py
+-rw-r--r--   0        0        0     3416 2024-05-16 07:51:03.361892 sinarax-1.1.8/sinaraX/screens/file_screen/file_tree.py
+-rw-r--r--   0        0        0     6458 2024-05-16 07:51:03.361892 sinarax-1.1.8/sinaraX/screens/main.py
+-rw-r--r--   0        0        0     6278 2024-05-16 07:51:03.361892 sinarax-1.1.8/sinaraX/screens/running.py
+-rw-r--r--   0        0        0    14035 2024-05-16 07:51:03.361892 sinarax-1.1.8/sinaraX/screens/server.py
+-rw-r--r--   0        0        0     2948 2024-05-16 07:51:03.361892 sinarax-1.1.8/sinaraX/screens/server_cfg.py
+-rw-r--r--   0        0        0      963 2024-05-16 07:51:03.361892 sinarax-1.1.8/sinaraX/screens/style.css
+-rw-r--r--   0        0        0     2403 2024-05-16 07:51:03.361892 sinarax-1.1.8/sinaraX/screens/update.py
+-rw-r--r--   0        0        0      650 2024-05-16 07:51:03.361892 sinarax-1.1.8/sinaraX/screens/utils/__init__.py
+-rw-r--r--   0        0        0     5161 2024-05-16 07:51:03.361892 sinarax-1.1.8/sinaraX/screens/utils/config.py
+-rw-r--r--   0        0        0     5721 2024-05-16 07:51:03.361892 sinarax-1.1.8/sinaraX/screens/utils/infra.py
+-rw-r--r--   0        0        0     1564 2024-05-16 07:51:03.361892 sinarax-1.1.8/sinaraX/screens/utils/process.py
+-rw-r--r--   0        0        0      847 2024-05-16 07:51:03.361892 sinarax-1.1.8/sinaraX/screens/utils/sinara_server_utils.py
+-rw-r--r--   0        0        0     3214 1970-01-01 00:00:00.000000 sinarax-1.1.8/PKG-INFO
```

### Comparing `sinarax-1.1.7/LICENSE` & `sinarax-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sinarax-1.1.7/README.md` & `sinarax-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `sinarax-1.1.7/pyproject.toml` & `sinarax-1.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sinaraX"
-version = "1.1.7"
+version = "1.1.8"
 readme = "README.md"
 authors = ["MiXaiLL76 <mike.milos@yandex.ru>"]
 description = "sinaraX - TUI for sinaraml clin"
 keywords = ["sinaraX", "tui", "cli", "sinaraml", "sinara"]
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
```

### Comparing `sinarax-1.1.7/sinaraX/screens/file_screen/file_tree.py` & `sinarax-1.1.8/sinaraX/screens/file_screen/file_tree.py`

 * *Files identical despite different names*

### Comparing `sinarax-1.1.7/sinaraX/screens/main.py` & `sinarax-1.1.8/sinaraX/screens/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 from pathlib import Path
 
 from sinaraml._version import __version__ as sinaraml_version
 from textual import on, work
 from textual.app import App
 from textual.containers import Horizontal
-from textual.events import Event
 from textual.widgets import Button, Footer, Label, Log, Static
 
 try:
     from sinaraX._version import __version__ as sinaraX_version
 except ImportError:
     sinaraX_version = "__dev__"
 
 from .running import RunningScreen
 from .server import ServerScreen
 from .server_cfg import BaseFunctions
 from .update import UpdateScreen
-from .utils.config import AppConfig
 from .utils.infra import (
     check_docker,
     check_docker_group,
     check_last_version,
     check_platform,
 )
 
 
 class SinaraX(App, BaseFunctions):
     CSS_PATH = "style.css"
     system_info_data = None
-    config = AppConfig()
     SCREENS = {
         "server_screen": ServerScreen(),
         "update_screen": UpdateScreen(),
         "running_screen": RunningScreen(),
     }
 
     BINDINGS = [
@@ -205,10 +202,10 @@
     def running_screen_start(self):
         self.push_screen("running_screen")
 
     @on(Button.Pressed, "#exit_button")
     def exit_button(self):
         self.exit()
 
-    def on_event(self, event: Event):
-        self.app.refresh(layout=True)
-        return super().on_event(event)
+    # def on_event(self, event: Event):
+    #     # self.app.refresh(layout=True)
+    #     return super().on_event(event)
```

### Comparing `sinarax-1.1.7/sinaraX/screens/running.py` & `sinarax-1.1.8/sinaraX/screens/running.py`

 * *Files identical despite different names*

### Comparing `sinarax-1.1.7/sinaraX/screens/server.py` & `sinarax-1.1.8/sinaraX/screens/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,20 +133,26 @@
                                 value="jovyan-single-use",
                                 name="instanceName",
                             )
 
                         with Horizontal():
                             with Vertical():
                                 with Collapsible(
-                                    title="Host where the server is run",
+                                    title=(
+                                        "Host where the server is run"
+                                        " (disabled!)"
+                                    ),
                                     collapsed=False,
                                 ):
-                                    with RadioSet(name="platform"):
+                                    with RadioSet(
+                                        name="platform",
+                                        disabled=True,
+                                    ):
                                         yield RadioButton("Desktop", value=True)
-                                        yield RadioButton("Remote VM")
+                                        yield RadioButton("Remote")
 
                             with Vertical():
                                 with Collapsible(
                                     title="Sinara image for", collapsed=False
                                 ):
                                     with RadioSet(name="sinara_image_num"):
                                         yield RadioButton("CV", value=True)
@@ -247,17 +253,15 @@
             yield Button(
                 "Exit",
                 id="exit_button",
                 classes="exit_button button",
                 variant="error",
             )
 
-        self.log_window: Log = Log(
-            highlight=True, id="output_text_area", classes="log_window"
-        )
+        self.log_window: Log = Log(highlight=True, classes="log_window")
         yield self.log_window
 
     @on(Button.Pressed, "#server_create_button")
     def server_create_button(self):
         if self.generate_config():
             cmd = "sinara server create --verbose "
             for key, val in self.config_dict.items():
```

### Comparing `sinarax-1.1.7/sinaraX/screens/server_cfg.py` & `sinarax-1.1.8/sinaraX/screens/server_cfg.py`

 * *Files identical despite different names*

### Comparing `sinarax-1.1.7/sinaraX/screens/style.css` & `sinarax-1.1.8/sinaraX/screens/style.css`

 * *Files identical despite different names*

### Comparing `sinarax-1.1.7/sinaraX/screens/update.py` & `sinarax-1.1.8/sinaraX/screens/update.py`

 * *Files identical despite different names*

### Comparing `sinarax-1.1.7/sinaraX/screens/utils/config.py` & `sinarax-1.1.8/sinaraX/screens/utils/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,30 @@
-import argparse
+import enum
 import json
 from pathlib import Path
 from typing import Iterable
 
 from textual.widgets import DirectoryTree, RadioSet
 
 from .sinara_server_utils import get_memory_size_limit
 
 
-class AppConfig(argparse.Namespace):
-    pass
+class SinaraImageType(enum.Enum):
+    CV = 0
+    ML = 1
+
+
+class SinaraRunMode(enum.Enum):
+    Quick = 0
+    Basic = 1
+
+
+class SinaraPlatform(enum.Enum):
+    Desktop = 0
+    Remote = 1
 
 
 class FilteredConfigTree(DirectoryTree):
     def filter_paths(self, paths: Iterable[Path]) -> Iterable[Path]:
         return [
             path
             for path in paths
@@ -29,17 +40,26 @@
 def remap_checkbox(_dict: dict, key: str, remap_dict: dict):
     if _dict.get(key) is not None:
         _dict[key] = remap_dict.get(_dict[key], False)
 
 
 def remap_config(_dict: dict, _from_screen=True):
     _remap_radio = {
-        "runMode": {0: "q", 1: "b"},
-        "sinara_image_num": {0: "2", 1: "1"},
-        "platform": {0: "desktop", 1: "remote_vm"},
+        "runMode": {
+            SinaraRunMode.Quick.value: "q",
+            SinaraRunMode.Basic.value: "b",
+        },
+        "sinara_image_num": {
+            SinaraImageType.CV.value: "2",
+            SinaraImageType.ML.value: "1",
+        },
+        "platform": {
+            SinaraPlatform.Desktop.value: "desktop",
+            SinaraPlatform.Remote.value: "remote",
+        },
     }
 
     _remap_checkbox = {
         "createFolders": {True: "y", False: "n"},
         "gpuEnabled": {True: "y", False: "n"},
         "experimental": {True: " ", False: None},
         "insecure": {True: " ", False: None},
@@ -100,25 +120,30 @@
     else:
         image = _dict.get("image")
         if image:
             if "exp" in image:
                 _dict["experimental"] = True
 
             if "cv" in image:
-                _dict["sinara_image_num"] = 0
+                _dict["sinara_image_num"] = SinaraImageType.CV.value
             else:
-                _dict["sinara_image_num"] = 1
+                _dict["sinara_image_num"] = SinaraImageType.ML.value
 
 
 def load_from_file(screen, file):
     with open(file) as fd:
         config = json.load(fd)
 
     remap_config(config, False)
 
+    # disabled
+    for key in ["platform", "createFolders"]:
+        if key in config:
+            del config[key]
+
     for child in screen.walk_children():
         if config.get(child.name) is not None:
             if type(child) is RadioSet:
                 child._selected = config[child.name]
                 child.action_toggle_button()
             else:
                 child.value = config[child.name]
```

### Comparing `sinarax-1.1.7/sinaraX/screens/utils/infra.py` & `sinarax-1.1.8/sinaraX/screens/utils/infra.py`

 * *Files identical despite different names*

### Comparing `sinarax-1.1.7/sinaraX/screens/utils/process.py` & `sinarax-1.1.8/sinaraX/screens/utils/process.py`

 * *Files identical despite different names*

### Comparing `sinarax-1.1.7/sinaraX/screens/utils/sinara_server_utils.py` & `sinarax-1.1.8/sinaraX/screens/utils/sinara_server_utils.py`

 * *Files identical despite different names*

### Comparing `sinarax-1.1.7/PKG-INFO` & `sinarax-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinaraX
-Version: 1.1.7
+Version: 1.1.8
 Summary: sinaraX - TUI for sinaraml clin
 Keywords: sinaraX,tui,cli,sinaraml,sinara
 Author: MiXaiLL76
 Author-email: mike.milos@yandex.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Apache Software License
```

