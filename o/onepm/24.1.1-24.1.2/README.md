# Comparing `tmp/onepm-24.1.1.tar.gz` & `tmp/onepm-24.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onepm-24.1.1.tar", last modified: Wed Mar  6 03:39:03 2024, max compression
+gzip compressed data, was "onepm-24.1.2.tar", last modified: Thu May 16 00:57:46 2024, max compression
```

## Comparing `onepm-24.1.1.tar` & `onepm-24.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1067 2024-03-06 03:38:54.452982 onepm-24.1.1/LICENSE
--rw-r--r--   0        0        0     2749 2024-03-06 03:38:54.452982 onepm-24.1.1/README.md
--rw-r--r--   0        0        0     2148 2024-03-06 03:39:03.336930 onepm-24.1.1/pyproject.toml
--rw-r--r--   0        0        0      618 2024-03-06 03:38:54.452982 onepm-24.1.1/src/onepm/__init__.py
--rw-r--r--   0        0        0     1940 2024-03-06 03:38:54.452982 onepm-24.1.1/src/onepm/cli.py
--rw-r--r--   0        0        0     8370 2024-03-06 03:38:54.452982 onepm-24.1.1/src/onepm/core.py
--rw-r--r--   0        0        0        0 2024-03-06 03:38:54.452982 onepm-24.1.1/src/onepm/pm/__init__.py
--rw-r--r--   0        0        0     4309 2024-03-06 03:38:54.452982 onepm-24.1.1/src/onepm/pm/base.py
--rw-r--r--   0        0        0      997 2024-03-06 03:38:54.452982 onepm-24.1.1/src/onepm/pm/pdm.py
--rw-r--r--   0        0        0     3477 2024-03-06 03:38:54.452982 onepm-24.1.1/src/onepm/pm/pip.py
--rw-r--r--   0        0        0      665 2024-03-06 03:38:54.452982 onepm-24.1.1/src/onepm/pm/pipenv.py
--rw-r--r--   0        0        0      980 2024-03-06 03:38:54.452982 onepm-24.1.1/src/onepm/pm/poetry.py
--rw-r--r--   0        0        0     2947 2024-03-06 03:38:54.452982 onepm-24.1.1/src/onepm/pm/uv.py
--rw-r--r--   0        0        0        0 2024-03-06 03:38:54.452982 onepm-24.1.1/src/onepm/py.typed
--rw-r--r--   0        0        0     1781 2024-03-06 03:38:54.452982 onepm-24.1.1/tests/conftest.py
--rw-r--r--   0        0        0     1391 2024-03-06 03:38:54.452982 onepm-24.1.1/tests/test_pdm.py
--rw-r--r--   0        0        0     3020 2024-03-06 03:38:54.452982 onepm-24.1.1/tests/test_pip.py
--rw-r--r--   0        0        0     1229 2024-03-06 03:38:54.452982 onepm-24.1.1/tests/test_pipenv.py
--rw-r--r--   0        0        0     1305 2024-03-06 03:38:54.452982 onepm-24.1.1/tests/test_poetry.py
--rw-r--r--   0        0        0     1367 2024-03-06 03:38:54.452982 onepm-24.1.1/tests/test_utils.py
--rw-r--r--   0        0        0     1566 2024-03-06 03:38:54.452982 onepm-24.1.1/tests/test_uv.py
--rw-r--r--   0        0        0     3602 1970-01-01 00:00:00.000000 onepm-24.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-16 00:57:36.478268 onepm-24.1.2/LICENSE
+-rw-r--r--   0        0        0     2749 2024-05-16 00:57:36.478268 onepm-24.1.2/README.md
+-rw-r--r--   0        0        0     2148 2024-05-16 00:57:46.830358 onepm-24.1.2/pyproject.toml
+-rw-r--r--   0        0        0      618 2024-05-16 00:57:36.478268 onepm-24.1.2/src/onepm/__init__.py
+-rw-r--r--   0        0        0     1954 2024-05-16 00:57:36.478268 onepm-24.1.2/src/onepm/cli.py
+-rw-r--r--   0        0        0     8548 2024-05-16 00:57:36.478268 onepm-24.1.2/src/onepm/core.py
+-rw-r--r--   0        0        0        0 2024-05-16 00:57:36.478268 onepm-24.1.2/src/onepm/pm/__init__.py
+-rw-r--r--   0        0        0     4309 2024-05-16 00:57:36.478268 onepm-24.1.2/src/onepm/pm/base.py
+-rw-r--r--   0        0        0      997 2024-05-16 00:57:36.478268 onepm-24.1.2/src/onepm/pm/pdm.py
+-rw-r--r--   0        0        0     3477 2024-05-16 00:57:36.478268 onepm-24.1.2/src/onepm/pm/pip.py
+-rw-r--r--   0        0        0      665 2024-05-16 00:57:36.478268 onepm-24.1.2/src/onepm/pm/pipenv.py
+-rw-r--r--   0        0        0      980 2024-05-16 00:57:36.478268 onepm-24.1.2/src/onepm/pm/poetry.py
+-rw-r--r--   0        0        0     2947 2024-05-16 00:57:36.478268 onepm-24.1.2/src/onepm/pm/uv.py
+-rw-r--r--   0        0        0        0 2024-05-16 00:57:36.478268 onepm-24.1.2/src/onepm/py.typed
+-rw-r--r--   0        0        0     1781 2024-05-16 00:57:36.478268 onepm-24.1.2/tests/conftest.py
+-rw-r--r--   0        0        0     1391 2024-05-16 00:57:36.478268 onepm-24.1.2/tests/test_pdm.py
+-rw-r--r--   0        0        0     3020 2024-05-16 00:57:36.478268 onepm-24.1.2/tests/test_pip.py
+-rw-r--r--   0        0        0     1229 2024-05-16 00:57:36.478268 onepm-24.1.2/tests/test_pipenv.py
+-rw-r--r--   0        0        0     1305 2024-05-16 00:57:36.478268 onepm-24.1.2/tests/test_poetry.py
+-rw-r--r--   0        0        0     1367 2024-05-16 00:57:36.478268 onepm-24.1.2/tests/test_utils.py
+-rw-r--r--   0        0        0     1566 2024-05-16 00:57:36.478268 onepm-24.1.2/tests/test_uv.py
+-rw-r--r--   0        0        0     3602 1970-01-01 00:00:00.000000 onepm-24.1.2/PKG-INFO
```

### Comparing `onepm-24.1.1/LICENSE` & `onepm-24.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `onepm-24.1.1/README.md` & `onepm-24.1.2/README.md`

 * *Files identical despite different names*

### Comparing `onepm-24.1.1/pyproject.toml` & `onepm-24.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 dynamic = []
-version = "24.1.1"
+version = "24.1.2"
 dependencies = [
     "packaging>=22.1",
     "tomlkit>=0.12.3",
 ]
 
 [project.license]
 text = "MIT"
```

### Comparing `onepm-24.1.1/src/onepm/__init__.py` & `onepm-24.1.2/src/onepm/__init__.py`

 * *Files identical despite different names*

### Comparing `onepm-24.1.1/src/onepm/cli.py` & `onepm-24.1.2/src/onepm/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,11 +50,11 @@
         case "install":
             core.get_package_manager()
         case "update" | "up ":
             core.update_package_manager()
         case "use":
             core.use_package_manager(args.spec)
         case "cleanup":
-            core.cleanup(args.name)
+            core.cleanup(args.name, args.version)
         case "list" | "ls":
             for installation in core.get_installations(args.name):
                 print(f"- {installation.version} ({installation.venv})")
```

### Comparing `onepm-24.1.1/src/onepm/core.py` & `onepm-24.1.2/src/onepm/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,20 +213,24 @@
 
     def update_package_manager(self) -> None:
         pm, requirement = self.detect_package_manager()
         self.install_tool(pm.name, requirement)
 
     def use_package_manager(self, spec: str) -> None:
         req = Requirement(spec)
-        self.install_tool(canonicalize_name(req.name), req)
+        name = canonicalize_name(req.name)
         self.pyproject.setdefault("tool", {}).setdefault("onepm", {})[
             "package-manager"
         ] = str(req)
         with open(self.path / "pyproject.toml", "w") as f:
             tomlkit.dump(self.pyproject, f)
+        for installation in self.get_installations(name):
+            if installation.version in req.specifier:
+                return
+        self.install_tool(canonicalize_name(req.name), req)
 
 
 @dataclass(frozen=True)
 class Installation:
     name: str
     distribution: Distribution
     venv: Path
```

### Comparing `onepm-24.1.1/src/onepm/pm/base.py` & `onepm-24.1.2/src/onepm/pm/base.py`

 * *Files identical despite different names*

### Comparing `onepm-24.1.1/src/onepm/pm/pdm.py` & `onepm-24.1.2/src/onepm/pm/pdm.py`

 * *Files identical despite different names*

### Comparing `onepm-24.1.1/src/onepm/pm/pip.py` & `onepm-24.1.2/src/onepm/pm/pip.py`

 * *Files identical despite different names*

### Comparing `onepm-24.1.1/src/onepm/pm/pipenv.py` & `onepm-24.1.2/src/onepm/pm/pipenv.py`

 * *Files identical despite different names*

### Comparing `onepm-24.1.1/src/onepm/pm/poetry.py` & `onepm-24.1.2/src/onepm/pm/poetry.py`

 * *Files identical despite different names*

### Comparing `onepm-24.1.1/src/onepm/pm/uv.py` & `onepm-24.1.2/src/onepm/pm/uv.py`

 * *Files identical despite different names*

### Comparing `onepm-24.1.1/tests/conftest.py` & `onepm-24.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `onepm-24.1.1/tests/test_pdm.py` & `onepm-24.1.2/tests/test_pdm.py`

 * *Files identical despite different names*

### Comparing `onepm-24.1.1/tests/test_pip.py` & `onepm-24.1.2/tests/test_pip.py`

 * *Files identical despite different names*

### Comparing `onepm-24.1.1/tests/test_pipenv.py` & `onepm-24.1.2/tests/test_pipenv.py`

 * *Files identical despite different names*

### Comparing `onepm-24.1.1/tests/test_poetry.py` & `onepm-24.1.2/tests/test_poetry.py`

 * *Files identical despite different names*

### Comparing `onepm-24.1.1/tests/test_utils.py` & `onepm-24.1.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `onepm-24.1.1/tests/test_uv.py` & `onepm-24.1.2/tests/test_uv.py`

 * *Files identical despite different names*

### Comparing `onepm-24.1.1/PKG-INFO` & `onepm-24.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onepm
-Version: 24.1.1
+Version: 24.1.2
 Summary: Picks the right package manager for you
 Author-Email: Frost Ming <mianghong@gmail.com>
 License: MIT
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
```

