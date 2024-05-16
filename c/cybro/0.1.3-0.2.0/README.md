# Comparing `tmp/cybro-0.1.3.tar.gz` & `tmp/cybro-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybro-0.1.3.tar", max compression
+gzip compressed data, was "cybro-0.2.0.tar", max compression
```

## Comparing `cybro-0.1.3.tar` & `cybro-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2024-03-20 19:17:35.234701 cybro-0.1.3/LICENSE
--rw-r--r--   0        0        0     2144 2024-03-20 19:17:35.234701 cybro-0.1.3/README.md
--rw-r--r--   0        0        0     4298 2024-03-20 19:17:35.238701 cybro-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      491 2024-03-20 19:17:35.238701 cybro-0.1.3/src/cybro/__init__.py
--rw-r--r--   0        0        0    17260 2024-03-20 19:17:35.238701 cybro-0.1.3/src/cybro/cybro.py
--rw-r--r--   0        0        0      450 2024-03-20 19:17:35.238701 cybro-0.1.3/src/cybro/exceptions.py
--rw-r--r--   0        0        0    14970 2024-03-20 19:17:35.238701 cybro-0.1.3/src/cybro/models.py
--rw-r--r--   0        0        0     3641 1970-01-01 00:00:00.000000 cybro-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-16 18:58:37.113793 cybro-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2144 2024-05-16 18:58:37.113793 cybro-0.2.0/README.md
+-rw-r--r--   0        0        0     4297 2024-05-16 18:58:37.113793 cybro-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      491 2024-05-16 18:58:37.113793 cybro-0.2.0/src/cybro/__init__.py
+-rw-r--r--   0        0        0    17434 2024-05-16 18:58:37.113793 cybro-0.2.0/src/cybro/cybro.py
+-rw-r--r--   0        0        0      450 2024-05-16 18:58:37.113793 cybro-0.2.0/src/cybro/exceptions.py
+-rw-r--r--   0        0        0    15177 2024-05-16 18:58:37.113793 cybro-0.2.0/src/cybro/models.py
+-rw-r--r--   0        0        0     3641 1970-01-01 00:00:00.000000 cybro-0.2.0/PKG-INFO
```

### Comparing `cybro-0.1.3/LICENSE` & `cybro-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cybro-0.1.3/README.md` & `cybro-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cybro-0.1.3/pyproject.toml` & `cybro-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cybro"
-version = "0.1.3"
+version = "0.2.0"
 description = "Asynchronous Python client for Cybro scgi server."
 authors = ["Daniel Gangl <killer007@gmx.at>"]
 maintainers = ["Daniel Gangl <killer007@gmx.at>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/killer0071234/python-cybro"
 repository = "https://github.com/killer0071234/python-cybro"
@@ -34,28 +34,28 @@
 yarl = ">=1.7.2"
 backoff = ">=1.11.0"
 cachetools = ">=5.0.0"
 xmltodict = "^0.13.0"
 
 [tool.poetry.dev-dependencies]
 aresponses = "^3.0.0"
-black = "^22.12"
+black = "^24.4"
 blacken-docs = "^1.16.0"
 coverage = {version = "^7.4", extras = ["toml"]}
 flake8 = "^4.0.1"
 flake8-docstrings = "^1.7.0"
 isort = "^5.13.2"
 mypy = "^1.8"
 pre-commit = "^3.5.0"
 pre-commit-hooks = "^4.5.0"
 pylint = "^3.0.3"
 pytest = "^7.4.3"
-pytest-asyncio = "^0.23.3"
+pytest-asyncio = "^0.23.6"
 pytest-cov = "^4.1.0"
-yamllint = "^1.33.0"
+yamllint = "^1.35.1"
 pyupgrade = "^3.8.0"
 flake8-simplify = "^0.21.0"
 vulture = "^2.11"
 flake8-bandit = "^3.0.0"
 flake8-bugbear = "^23.3.12"
 flake8-builtins = "^2.2.0"
 flake8-comprehensions = "^3.14.0"
```

### Comparing `cybro-0.1.3/src/cybro/cybro.py` & `cybro-0.2.0/src/cybro/cybro.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,17 +312,20 @@
     async def read_var_bool(
         self,
         name: str,
     ) -> bool:
         """Read a single variable from scgi server as float."""
         return await self.read_var(name, VarType.BOOL)
 
-    def add_var(self, name: str) -> None:
-        """Add a variable into update buffer."""
-        self._device.add_var(name)
+    def add_var(self, name: str, allow_all: bool = False) -> None:
+        """Add a variable into update buffer.
+
+        name: Variable name to read eg: c1000.scan_time
+        allow_all: Optionally allow to add also non existing variables"""
+        self._device.add_var(name, allow_all=allow_all)
 
     def remove_var(self, name: str) -> None:
         """Remove a variable from update buffer."""
         self._device.remove_var(name)
 
     async def __aenter__(self) -> Cybro:
         """Async enter.
```

### Comparing `cybro-0.1.3/src/cybro/models.py` & `cybro-0.2.0/src/cybro/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -385,22 +385,26 @@
                 self.vars_types.update({_var["name"]: var_type})
                 self.user_vars.update({_var["name"]: ""})
                 return self.vars[_var["name"]].value
         except (KeyError, TypeError):
             pass
         return "?"
 
-    def add_var(self, name: str, var_type: VarType = 0) -> None:
+    def add_var(
+        self, name: str, var_type: VarType = 0, allow_all: bool = False
+    ) -> None:
         """Adds a variable to the update list.
 
         Args:
             name: Variable name to read eg: c1000.scan_time
-            var_type: Optionally defines a Varaibe Type"""
-        self.user_vars.update({name: ""})
-        self.vars_types.update({name: var_type})
+            var_type: Optionally defines a Variable Type
+            allow_all: Optionally allow to add also non existing variables"""
+        if allow_all or name in self.plc_info.plc_vars or name.find(".sys.") != -1:
+            self.user_vars.update({name: ""})
+            self.vars_types.update({name: var_type})
 
     def remove_var(self, name: str) -> None:
         """Removes a variable from the read list.
 
         Args:
             name: Variable name to delete from user_vars"""
         self.user_vars.pop(name, "")
```

### Comparing `cybro-0.1.3/PKG-INFO` & `cybro-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybro
-Version: 0.1.3
+Version: 0.2.0
 Summary: Asynchronous Python client for Cybro scgi server.
 Home-page: https://github.com/killer0071234/python-cybro
 License: MIT
 Keywords: cybro,api,async,client
 Author: Daniel Gangl
 Author-email: killer007@gmx.at
 Maintainer: Daniel Gangl
```

