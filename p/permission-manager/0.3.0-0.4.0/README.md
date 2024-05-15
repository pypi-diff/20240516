# Comparing `tmp/permission_manager-0.3.0.tar.gz` & `tmp/permission_manager-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "permission_manager-0.3.0.tar", max compression
+gzip compressed data, was "permission_manager-0.4.0.tar", max compression
```

## Comparing `permission_manager-0.3.0.tar` & `permission_manager-0.4.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1075 2024-04-28 01:55:53.317114 permission_manager-0.3.0/LICENSE
--rw-r--r--   0        0        0     2508 2024-04-28 01:55:53.317114 permission_manager-0.3.0/README.md
--rw-r--r--   0        0        0      160 2024-04-28 01:55:53.317114 permission_manager-0.3.0/permission_manager/__init__.py
--rw-r--r--   0        0        0     1201 2024-04-28 01:55:53.317114 permission_manager-0.3.0/permission_manager/decorators.py
--rw-r--r--   0        0        0      198 2024-04-28 01:55:53.317114 permission_manager-0.3.0/permission_manager/exceptions.py
--rw-r--r--   0        0        0     4848 2024-04-28 01:55:53.317114 permission_manager-0.3.0/permission_manager/manager.py
--rw-r--r--   0        0        0     1495 2024-04-28 01:55:53.317114 permission_manager-0.3.0/permission_manager/result.py
--rw-r--r--   0        0        0     2241 2024-04-28 01:55:53.317114 permission_manager-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3217 1970-01-01 00:00:00.000000 permission_manager-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-05-15 03:03:20.232421 permission_manager-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2602 2024-05-15 03:03:20.232421 permission_manager-0.4.0/README.md
+-rw-r--r--   0        0        0      160 2024-05-15 03:03:20.232421 permission_manager-0.4.0/permission_manager/__init__.py
+-rw-r--r--   0        0        0     1388 2024-05-15 03:03:20.232421 permission_manager-0.4.0/permission_manager/decorators.py
+-rw-r--r--   0        0        0      296 2024-05-15 03:03:20.232421 permission_manager-0.4.0/permission_manager/exceptions.py
+-rw-r--r--   0        0        0     4447 2024-05-15 03:03:20.232421 permission_manager-0.4.0/permission_manager/manager.py
+-rw-r--r--   0        0        0     1495 2024-05-15 03:03:20.232421 permission_manager-0.4.0/permission_manager/result.py
+-rw-r--r--   0        0        0      705 2024-05-15 03:03:20.232421 permission_manager-0.4.0/permission_manager/utils.py
+-rw-r--r--   0        0        0     2322 2024-05-15 03:03:20.232421 permission_manager-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3311 1970-01-01 00:00:00.000000 permission_manager-0.4.0/PKG-INFO
```

### Comparing `permission_manager-0.3.0/LICENSE` & `permission_manager-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `permission_manager-0.3.0/README.md` & `permission_manager-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Permission Manager
 
 A simple way to manage object permissions.
 
+Full documentation on [read the docs](https://permission-manager.readthedocs.io/en/latest/).
+
 ## Install
 
 ```bash
 pip install permission-manager
 ```
 
 ## Example
```

### Comparing `permission_manager-0.3.0/permission_manager/decorators.py` & `permission_manager-0.4.0/permission_manager/decorators.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,15 +35,23 @@
         except KeyError:
             self._cache[fn.__name__] = fn(self)
             return self._cache[fn.__name__]
 
     return wrapper
 
 
-def alias(name: str) -> Callable:
-    """Decorator that add alias to permission."""
+def alias(names: list[str]) -> Callable:
+    """Decorator that add aliases to permission.
+
+    Args:
+        names (list[str]): The alias name(s) to be added to the permission
+            function.
+
+    Returns:
+        Callable: decorated function.
+    """
 
     def decorator(fn) -> Callable:
-        fn.permission_manager_alias = name
+        fn.aliases = getattr(fn, 'aliases', []) + names
         return fn
 
     return decorator
```

### Comparing `permission_manager-0.3.0/permission_manager/manager.py` & `permission_manager-0.4.0/permission_manager/manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import re
 from collections.abc import Iterable
 from contextlib import suppress
 from functools import cached_property
 from typing import Any
 
 from .decorators import cache_permission, catch_denied_exception
-from .exceptions import PermissionManagerError
-from .result import PermissionResult
+from .exceptions import AliasAlreadyExistsError, PermissionManagerError
+from .utils import get_result_value
 
 
 permission_re = re.compile(r'^has_(\w+)_permission$')
 
 
 class BasePermissionMeta(type):
     """Metaclass for bind permission actions."""
@@ -28,17 +28,21 @@
             if action_name := permission_re.match(attr_name):
                 permission_fn = cache_permission(
                     catch_denied_exception(getattr(cls, attr_name))
                 )
                 setattr(cls, attr_name, permission_fn)
                 cls._actions[action_name.group(1)] = permission_fn
 
-                if alias := getattr(
-                    permission_fn, 'permission_manager_alias', None
-                ):
+                for alias in getattr(permission_fn, 'aliases', ()):
+                    if alias in cls._aliases:
+                        msg = (
+                            f'The alias "{alias}" is already in use for '
+                            f'"{cls._aliases[alias].__name__}".'
+                        )
+                        raise AliasAlreadyExistsError(msg)
                     cls._aliases[alias] = permission_fn
 
 
 class BasePermissionManager(metaclass=BasePermissionMeta):
     """Base permission manager class."""
 
     def __init__(
@@ -72,51 +76,26 @@
         try:
             return self._aliases[action](self)
         except KeyError as exc:
             raise ValueError(
                 f'"{self.__class__.__name__}" doesn\'t have "{action}" action.'
             ) from exc
 
-    def get_result_value(
-        self,
-        *,
-        value: bool | dict | PermissionResult,
-        with_messages: bool = False,
-    ) -> bool | dict:
-        """Serialize result value."""
-        if isinstance(value, dict):
-            return {
-                k: self.get_result_value(
-                    value=v,
-                    with_messages=with_messages,
-                )
-                for k, v in value.items()
-            }
-
-        result = bool(value)
-
-        if with_messages:
-            result = {
-                'allow': result,
-                'messages': getattr(value, 'returned_message', None),
-            }
-        return result
-
     def resolve(
         self,
         *,
         actions: Iterable | None = None,
         with_messages: bool = False,
     ) -> dict:
         """Resolve list of actions."""
         if actions is None:
             actions = self._actions.keys()
 
         return {
-            action: self.get_result_value(
+            action: get_result_value(
                 value=self.has_permission(action),
                 with_messages=with_messages,
             )
             for action in actions
         }
```

### Comparing `permission_manager-0.3.0/permission_manager/result.py` & `permission_manager-0.4.0/permission_manager/result.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 class PermissionResult:
     """Class for storing permission values and messages.
 
     Attributes:
         message (str | list | None): The message associated with the
             permission result.
         value (bool): The boolean value indicating the permission result.
-        message_if_false (bool): A flag indicating whether to include the
-            message when the value is False.
+        message_if_true (bool): A flag indicating whether to include the
+            message when the value is True.
     """
 
     message: str | list | None = None
     value: bool = False
-    message_if_false: bool = True
+    message_if_true: bool = False
 
     def __post_init__(self) -> None:
         """Ensure the value is a list."""
         if self.message and not isinstance(self.message, list):
             self.message = [self.message]
 
     def __bool__(self) -> bool:
@@ -30,16 +30,16 @@
         """Return a string representation of the PermissionResult object."""
         return (
             f'PermissionResult(value={self.value!r}, message={self.message!r})'
         )
 
     @property
     def returned_message(self) -> list | None:
-        """Return the message based on the value and message_if_false flag.
+        """Return the message based on the value and message_if_true flag.
 
         Returns:
             list | None: The message associated with the permission result,
-                or None if the value is True and message_if_false is True.
+                or None if the value is True and message_if_true is False.
         """
-        if self.value and self.message_if_false:
+        if self.value and not self.message_if_true:
             return None
         return self.message
```

### Comparing `permission_manager-0.3.0/pyproject.toml` & `permission_manager-0.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "permission-manager"
-version = "0.3.0"
+version = "0.4.0"
 description = "A simple way to manage object permissions."
 authors = ["Grigory Mishchenko <grishkokot@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "permission_manager"}]
 repository = "https://github.com/kindlycat/permission-manager"
 keywords = ["permissions"]
@@ -20,14 +20,17 @@
 python = "^3.10"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "^8.24"
 ipdb = "^0.13.13"
 pytest = "^8.1.2"
 ruff = "^0.4.2"
+pytest-cov = "^5.0.0"
+sphinx = "^7.3.7"
+furo = "^2024.4.27"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 exclude = [
@@ -70,14 +73,15 @@
     "D100", "D101", "ANN101", "D102", "EXE001", "D107", "ANN003", "ANN001",
     "ARG002", "ANN002", "D103", "D106", "D104", "ANN201", "COM812", "ISC001",
     "ANN401", "ANN102", "TRY003", "EM102", "EM101"
 ]
 
 fixable = ["ALL"]
 unfixable = []
+exclude = ['docs/*']
 
 [tool.ruff.lint.per-file-ignores]
 "tests/*" = ["S101", "S106", "RUF012", "D105", "PLR2004"]
 
 [tool.ruff.lint.isort]
 section-order = [
     "future", "standard-library", "third-party", "first-party", "local-folder"
```

### Comparing `permission_manager-0.3.0/PKG-INFO` & `permission_manager-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: permission-manager
-Version: 0.3.0
+Version: 0.4.0
 Summary: A simple way to manage object permissions.
 Home-page: https://github.com/kindlycat/permission-manager
 License: MIT
 Keywords: permissions
 Author: Grigory Mishchenko
 Author-email: grishkokot@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -17,14 +17,16 @@
 Project-URL: Repository, https://github.com/kindlycat/permission-manager
 Description-Content-Type: text/markdown
 
 # Permission Manager
 
 A simple way to manage object permissions.
 
+Full documentation on [read the docs](https://permission-manager.readthedocs.io/en/latest/).
+
 ## Install
 
 ```bash
 pip install permission-manager
 ```
 
 ## Example
```

