# Comparing `tmp/cepack-0.0.5.tar.gz` & `tmp/cepack-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cepack-0.0.5.tar", last modified: Tue May 14 10:40:12 2024, max compression
+gzip compressed data, was "cepack-0.0.6.tar", last modified: Thu May 16 05:58:59 2024, max compression
```

## Comparing `cepack-0.0.5.tar` & `cepack-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:40:12.461459 cepack-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-14 10:40:08.000000 cepack-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-14 10:40:08.000000 cepack-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    41458 2024-05-14 10:40:12.461459 cepack-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-14 10:40:08.000000 cepack-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:40:12.457459 cepack-0.0.5/cepack/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-14 10:40:08.000000 cepack-0.0.5/cepack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-05-14 10:40:08.000000 cepack-0.0.5/cepack/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-05-14 10:40:08.000000 cepack-0.0.5/cepack/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:40:12.457459 cepack-0.0.5/cepack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    41458 2024-05-14 10:40:12.000000 cepack-0.0.5/cepack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-14 10:40:12.000000 cepack-0.0.5/cepack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 10:40:12.000000 cepack-0.0.5/cepack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-14 10:40:12.000000 cepack-0.0.5/cepack.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-14 10:40:12.000000 cepack-0.0.5/cepack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-14 10:40:12.000000 cepack-0.0.5/cepack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-14 10:40:08.000000 cepack-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 10:40:12.461459 cepack-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:40:12.457459 cepack-0.0.5/test/
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-14 10:40:08.000000 cepack-0.0.5/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-05-14 10:40:08.000000 cepack-0.0.5/test/test_ci.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-14 10:40:08.000000 cepack-0.0.5/test/test_utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:40:12.457459 cepack-0.0.5/test/utility/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-14 10:40:08.000000 cepack-0.0.5/test/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-14 10:40:08.000000 cepack-0.0.5/test/utility/env_manage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:58:59.976175 cepack-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-16 05:58:52.000000 cepack-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 05:58:52.000000 cepack-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-16 05:58:59.976175 cepack-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-16 05:58:52.000000 cepack-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:58:59.972175 cepack-0.0.6/cepack/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-16 05:58:52.000000 cepack-0.0.6/cepack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-05-16 05:58:52.000000 cepack-0.0.6/cepack/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-05-16 05:58:52.000000 cepack-0.0.6/cepack/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:58:59.976175 cepack-0.0.6/cepack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-16 05:58:59.000000 cepack-0.0.6/cepack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-16 05:58:59.000000 cepack-0.0.6/cepack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 05:58:59.000000 cepack-0.0.6/cepack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-16 05:58:59.000000 cepack-0.0.6/cepack.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-16 05:58:59.000000 cepack-0.0.6/cepack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-16 05:58:59.000000 cepack-0.0.6/cepack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-16 05:58:52.000000 cepack-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 05:58:59.976175 cepack-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:58:59.972175 cepack-0.0.6/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-16 05:58:52.000000 cepack-0.0.6/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-05-16 05:58:52.000000 cepack-0.0.6/test/test_ci.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-16 05:58:52.000000 cepack-0.0.6/test/test_utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:58:59.972175 cepack-0.0.6/test/utility/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-16 05:58:52.000000 cepack-0.0.6/test/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-16 05:58:52.000000 cepack-0.0.6/test/utility/env_manage.py
```

### Comparing `cepack-0.0.5/LICENSE` & `cepack-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cepack-0.0.5/cepack/main.py` & `cepack-0.0.6/cepack/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from typing_extensions import Annotated
 
 import typer
 import logging
 import toml
-from .utility import download_repo, download_release, get_repo_info
+from .utility import download_repo, download_release, get_repo_info, delete_pack
 import requests
 import sys
 from pathlib import Path
+import shutil
 
 from .utility import TomlDepend
 
 log = logging.getLogger("rich")
 
 app = typer.Typer()
 
@@ -51,18 +52,20 @@
             download_release(release_url, repo)
         except KeyError:
             download_repo(lib_url, repo)
 
 
 @app.command()
 def add(
-        pack_name: str,
-        pack_url: str,
-        pack_type: Annotated[bool, typer.Option(help="True: download release False: download repo")] = False,
-        pack_version: Annotated[str, typer.Option(help="pack version")] = None,
+    pack_name: str,
+    pack_url: str,
+    pack_type: Annotated[
+        bool, typer.Option(help="True: download release False: download repo")
+    ] = False,
+    pack_version: Annotated[str, typer.Option(help="pack version")] = None,
 ):
     if pack_type:
         if pack_version is None:
             log.error("Unspecified release version!")
             sys.exit()
 
     toml_depend = TomlDepend()
@@ -83,24 +86,35 @@
         owner = lib_info["owner"]
         repo = lib_info["repo"]
         tag = pack_cfg[pack_name]["version"]
         list_releases = base_url + f"/repos/{owner}/{repo}/releases/tags/{tag}"
         log.debug(f"list_releases: {list_releases}")
 
         ret = requests.get(list_releases)
-        
+
         release_url = ret.json()["zipball_url"]
         download_release(release_url, pack_name)
     else:
         download_repo(pack_url, pack_name)
 
 
 @app.command()
-def init():
-    print("default")
+def remove(pack_name: str):
+    log.debug("run command 'remove'...")
+    log.info(f"remove {pack_name}")
+    pack_path = Path(f"lib/{pack_name}")
+    pack_toml = TomlDepend()
+
+    if pack_name in pack_toml.get_depend():
+        pack_toml.delete_depend(pack_name)
+        if pack_path.exists():
+            log.debug(f"delete {pack_name}")
+            delete_pack(pack_path)
+    else:
+        log.error("not pack!")
 
 
 def run():
     app()
 
 
 if __name__ == "__main__":
```

### Comparing `cepack-0.0.5/cepack/utility.py` & `cepack-0.0.6/cepack/utility.py`

 * *Files 7% similar despite different names*

```diff
@@ -101,23 +101,39 @@
     log.debug(f"findall_url:{a}")
     b = [i[1:] for i in a]
     c = {"owner": b[1], "repo": b[2], "remote": b[0]}
     log.debug(f"info:{c}")
     return c
 
 
+def delete_pack(path: Path):
+    if os.name == "nt":
+        result = subprocess.run(
+            ["rmdir", "/S", "/Q", path],
+            shell=True,
+            stdout=subprocess.PIPE,
+            stderr=subprocess.PIPE,
+        )
+        if result.stdout != b"":
+            log.info(result.stdout.decode("GBK"))
+        if result.stderr != b"":
+            log.error(result.stderr.decode("GBK"))
+    elif os.name == "posix":
+        shutil.rmtree(path)
+
+
 class TomlDepend:
     def __init__(self) -> None:
         try:
             self._cfg_file = toml.load("depend.toml")
         except:
             log.error("none depend.toml!")
             sys.exit()
 
-    def get_depend(self):
+    def get_depend(self) -> dict:
         return self._cfg_file.get("depend", {})
 
     def set_depend(self, name: str, url: str, version=None):
         log.info(f"Wire {name} to depend.toml")
         depend_lib = self.get_depend()
         if version is None:
             depend_lib[name] = {"url": url}
@@ -126,7 +142,14 @@
 
         self._cfg_file["depend"] = depend_lib
         log.debug(f"{name}: {self._cfg_file['depend'][name]}")
 
         with open(Path("depend.toml"), "w+") as fd:
             d = toml.dump(self._cfg_file, fd)
             log.debug(d)
+            
+    def delete_depend(self,name:str):
+        log.debug(f"Delete {name} from toml")
+        self.get_depend().pop(name)
+        with open(Path("depend.toml"), "w+") as fd:
+            d = toml.dump(self._cfg_file, fd)
+            log.debug(d)
```

### Comparing `cepack-0.0.5/pyproject.toml` & `cepack-0.0.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 [project]
 name = "cepack"
-version = "0.0.5"
+version = "0.0.6"
 authors = [{ name = "paopaozhi", email = "paopaozhi@hotmail.com" }]
 dependencies = ["typer","toml","requests"]
 description = "embedded pack manage"
 readme = "README.md"
 requires-python = ">=3.9"
-license = { file = "LICENSE" }
 classifiers = [
   "Programming Language :: Python :: 3.9",
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
   "Operating System :: OS Independent",
 ]
 
 [project.scripts]
```

### Comparing `cepack-0.0.5/test/test_utility.py` & `cepack-0.0.6/test/test_utility.py`

 * *Files identical despite different names*

### Comparing `cepack-0.0.5/test/utility/env_manage.py` & `cepack-0.0.6/test/utility/env_manage.py`

 * *Files identical despite different names*

