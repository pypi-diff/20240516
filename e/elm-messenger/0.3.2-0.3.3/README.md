# Comparing `tmp/elm_messenger-0.3.2.tar.gz` & `tmp/elm_messenger-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elm_messenger-0.3.2.tar", last modified: Tue May 14 21:24:32 2024, max compression
+gzip compressed data, was "elm_messenger-0.3.3.tar", last modified: Wed May 15 19:16:10 2024, max compression
```

## Comparing `elm_messenger-0.3.2.tar` & `elm_messenger-0.3.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 wayland   (1000) wayland   (1000)        0 2024-05-14 21:24:32.310885 elm_messenger-0.3.2/
--rw-r--r--   0 wayland   (1000) wayland   (1000)       18 2024-05-12 21:23:16.000000 elm_messenger-0.3.2/MANIFEST.in
--rw-r--r--   0 wayland   (1000) wayland   (1000)     7452 2024-05-14 21:24:32.310885 elm_messenger-0.3.2/PKG-INFO
--rw-r--r--   0 wayland   (1000) wayland   (1000)     7181 2024-05-12 21:23:16.000000 elm_messenger-0.3.2/Readme.md
-drwxr-xr-x   0 wayland   (1000) wayland   (1000)        0 2024-05-14 21:24:32.310885 elm_messenger-0.3.2/elm_messenger.egg-info/
--rw-r--r--   0 wayland   (1000) wayland   (1000)     7452 2024-05-14 21:24:32.000000 elm_messenger-0.3.2/elm_messenger.egg-info/PKG-INFO
--rw-r--r--   0 wayland   (1000) wayland   (1000)      368 2024-05-14 21:24:32.000000 elm_messenger-0.3.2/elm_messenger.egg-info/SOURCES.txt
--rw-r--r--   0 wayland   (1000) wayland   (1000)        1 2024-05-14 21:24:32.000000 elm_messenger-0.3.2/elm_messenger.egg-info/dependency_links.txt
--rw-r--r--   0 wayland   (1000) wayland   (1000)       61 2024-05-14 21:24:32.000000 elm_messenger-0.3.2/elm_messenger.egg-info/entry_points.txt
--rw-r--r--   0 wayland   (1000) wayland   (1000)        6 2024-05-14 21:24:32.000000 elm_messenger-0.3.2/elm_messenger.egg-info/requires.txt
--rw-r--r--   0 wayland   (1000) wayland   (1000)       13 2024-05-14 21:24:32.000000 elm_messenger-0.3.2/elm_messenger.egg-info/top_level.txt
-drwxr-xr-x   0 wayland   (1000) wayland   (1000)        0 2024-05-14 21:24:32.310885 elm_messenger-0.3.2/messengercli/
--rwxr-xr-x   0 wayland   (1000) wayland   (1000)        0 2024-05-12 21:23:17.000000 elm_messenger-0.3.2/messengercli/__init__.py
--rwxr-xr-x   0 wayland   (1000) wayland   (1000)      120 2024-05-12 21:23:17.000000 elm_messenger-0.3.2/messengercli/command_line.py
--rwxr-xr-x   0 wayland   (1000) wayland   (1000)    13990 2024-05-14 21:15:13.000000 elm_messenger-0.3.2/messengercli/messenger.py
--rw-r--r--   0 wayland   (1000) wayland   (1000)     1170 2024-05-12 21:23:17.000000 elm_messenger-0.3.2/messengercli/updater.py
--rw-r--r--   0 wayland   (1000) wayland   (1000)      392 2024-05-14 21:24:32.314885 elm_messenger-0.3.2/setup.cfg
--rw-r--r--   0 wayland   (1000) wayland   (1000)      161 2024-05-12 21:23:17.000000 elm_messenger-0.3.2/setup.py
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2024-05-15 19:16:10.907402 elm_messenger-0.3.3/
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       18 2024-05-04 14:47:23.000000 elm_messenger-0.3.3/MANIFEST.in
+-rw-r--r--   0 linsy     (1000) linsy     (1000)     1159 2024-05-15 19:16:10.907402 elm_messenger-0.3.3/PKG-INFO
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      888 2024-05-15 03:21:04.000000 elm_messenger-0.3.3/Readme.md
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2024-05-15 19:16:10.907402 elm_messenger-0.3.3/elm_messenger.egg-info/
+-rw-r--r--   0 linsy     (1000) linsy     (1000)     1159 2024-05-15 19:16:10.000000 elm_messenger-0.3.3/elm_messenger.egg-info/PKG-INFO
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      368 2024-05-15 19:16:10.000000 elm_messenger-0.3.3/elm_messenger.egg-info/SOURCES.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)        1 2024-05-15 19:16:10.000000 elm_messenger-0.3.3/elm_messenger.egg-info/dependency_links.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       61 2024-05-15 19:16:10.000000 elm_messenger-0.3.3/elm_messenger.egg-info/entry_points.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)        6 2024-05-15 19:16:10.000000 elm_messenger-0.3.3/elm_messenger.egg-info/requires.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       13 2024-05-15 19:16:10.000000 elm_messenger-0.3.3/elm_messenger.egg-info/top_level.txt
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2024-05-15 19:16:10.907402 elm_messenger-0.3.3/messengercli/
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2024-05-04 14:47:23.000000 elm_messenger-0.3.3/messengercli/__init__.py
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)      120 2024-05-04 14:47:23.000000 elm_messenger-0.3.3/messengercli/command_line.py
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)    14071 2024-05-15 18:41:56.000000 elm_messenger-0.3.3/messengercli/messenger.py
+-rw-r--r--   0 linsy     (1000) linsy     (1000)     1090 2024-05-15 18:35:42.000000 elm_messenger-0.3.3/messengercli/updater.py
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      392 2024-05-15 19:16:10.910736 elm_messenger-0.3.3/setup.cfg
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      161 2024-05-04 14:47:23.000000 elm_messenger-0.3.3/setup.py
```

### Comparing `elm_messenger-0.3.2/messengercli/messenger.py` & `elm_messenger-0.3.3/messengercli/messenger.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,8 @@
 #!/usr/bin/env python3
-"""
-@Author: King
-@Date: 2023-05-03 21:46:45
-@Email: linsy_king@sjtu.edu.cn
-"""
 
 import typer
 import os
 import shutil
 import json
 from .updater import Updater
 
@@ -16,15 +11,15 @@
 
 
 class Messenger:
     config = None
 
     def __init__(self) -> None:
         """
-        Check if `messager.json` exists and load it.
+        Check if `messenger.json` exists and load it.
         """
         if os.path.exists("messenger.json"):
             with open("messenger.json", "r") as f:
                 self.config = json.load(f)
             if "version" not in self.config:
                 raise Exception("Messenger API version not found in the config file.")
             if self.config["version"] != API_VERSION:
@@ -187,15 +182,15 @@
                     f"src/Scenes/{scene}/{dir}/{name}/Model.elm",
                 ],
             ).rep("Scenes").rep(scene).rep(dir).rep(name)
 
     def format(self):
         os.system("elm-format src/ --yes")
 
-    def add_layer(self, scene: str, layer: str, has_component: bool, is_proto: bool):
+    def add_layer(self, scene: str, layer: str, has_component: bool, is_proto: bool, dir: str):
         """
         Add a layer to a scene
         """
         if is_proto:
             if scene not in self.config["sceneprotos"]:
                 raise Exception("Scene doesn't exist.")
             if layer in self.config["sceneprotos"][scene]:
@@ -211,15 +206,15 @@
                 Updater(
                     [
                         ".messenger/layer/ModelC.elm",
                     ],
                     [
                         f"src/SceneProtos/{scene}/{layer}/Model.elm",
                     ],
-                ).rep("SceneProtos").rep(scene).rep(layer)
+                ).rep("SceneProtos").rep(scene).rep(layer).rep(dir)
             else:
                 Updater(
                     [
                         ".messenger/layer/Model.elm",
                     ],
                     [
                         f"src/SceneProtos/{scene}/{layer}/Model.elm",
@@ -241,15 +236,15 @@
                 Updater(
                     [
                         ".messenger/layer/ModelC.elm",
                     ],
                     [
                         f"src/Scenes/{scene}/{layer}/Model.elm",
                     ],
-                ).rep("Scenes").rep(scene).rep(layer)
+                ).rep("Scenes").rep(scene).rep(layer).rep(dir)
             else:
                 Updater(
                     [
                         ".messenger/layer/Model.elm",
                     ],
                     [
                         f"src/Scenes/{scene}/{layer}/Model.elm",
@@ -391,24 +386,27 @@
 @app.command()
 def layer(
     scene: str,
     layer: str,
     has_component: bool = typer.Option(
         False, "--with-component", "-c", help="Use components in this layer"
     ),
+    compdir: str = typer.Option(
+        "Components", "--cdir", "-cd", help="Directory of components in the scene"
+    ),
     is_proto: bool = typer.Option(
         False, "--proto", "-p", help="Create layer in sceneproto"
     ),
 ):
     scene = check_name(scene)
     layer = check_name(layer)
     msg = Messenger()
     input(
         f"You are going to create a layer named {layer} under {'sceneproto' if is_proto else 'scene'} {scene}, continue?"
     )
-    msg.add_layer(scene, layer, has_component, is_proto)
+    msg.add_layer(scene, layer, has_component, is_proto, compdir)
     msg.format()
     print("Done!")
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `elm_messenger-0.3.2/messengercli/updater.py` & `elm_messenger-0.3.3/messengercli/updater.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,8 @@
 #!/usr/bin/env python3
-"""
-@Author: King
-@Date: 2023-05-12 12:34:46
-@Email: linsy_king@sjtu.edu.cn
-"""
 from __future__ import annotations
 
 
 class Updater:
     proto: list[str] = []
     target: list[str] = []
     dollar = 0
```

