# Comparing `tmp/sema4ai_actions-0.5.0.tar.gz` & `tmp/sema4ai_actions-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sema4ai_actions-0.5.0.tar", max compression
+gzip compressed data, was "sema4ai_actions-0.6.0.tar", max compression
```

## Comparing `sema4ai_actions-0.5.0.tar` & `sema4ai_actions-0.6.0.tar`

### file list

```diff
@@ -1,33 +1,35 @@
--rw-r--r--   0        0        0     2971 2024-05-08 19:14:34.472609 sema4ai_actions-0.5.0/README.md
--rw-r--r--   0        0        0      971 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     5474 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/__init__.py
--rw-r--r--   0        0        0       80 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/__main__.py
--rw-r--r--   0        0        0    12093 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_action.py
--rw-r--r--   0        0        0     7567 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_action_context.py
--rw-r--r--   0        0        0    11151 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_args_dispatcher.py
--rw-r--r--   0        0        0     1494 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_callback.py
--rw-r--r--   0        0        0     8376 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_collect_actions.py
--rw-r--r--   0        0        0    31992 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_commands.py
--rw-r--r--   0        0        0     2276 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_config.py
--rw-r--r--   0        0        0      336 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_constants.py
--rw-r--r--   0        0        0        0 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_customization/__init__.py
--rw-r--r--   0        0        0     2722 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_customization/_extension_points.py
--rw-r--r--   0        0        0     9922 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_customization/_plugin_manager.py
--rw-r--r--   0        0        0      252 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_exceptions.py
--rw-r--r--   0        0        0     5638 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_fixtures.py
--rw-r--r--   0        0        0     2500 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_hooks.py
--rw-r--r--   0        0        0     7491 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_interrupts.py
--rw-r--r--   0        0        0     1367 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_lifecycle.py
--rw-r--r--   0        0        0    12522 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_lint_action.py
--rw-r--r--   0        0        0     1082 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_log_auto_setup.py
--rw-r--r--   0        0        0     3074 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_log_output_setup.py
--rw-r--r--   0        0        0     5261 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_managed_parameters.py
--rw-r--r--   0        0        0     6023 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_protocols.py
--rw-r--r--   0        0        0    13813 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_remove_refs.py
--rw-r--r--   0        0        0     2906 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_request.py
--rw-r--r--   0        0        0     1023 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_request_impl.py
--rw-r--r--   0        0        0     4478 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_secret.py
--rw-r--r--   0        0        0     3134 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/api.py
--rw-r--r--   0        0        0     2277 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/cli.py
--rw-r--r--   0        0        0        0 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/py.typed
--rw-r--r--   0        0        0     3788 1970-01-01 00:00:00.000000 sema4ai_actions-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     2971 2024-05-16 19:14:01.084860 sema4ai_actions-0.6.0/README.md
+-rw-r--r--   0        0        0      971 2024-05-16 19:14:01.084860 sema4ai_actions-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     5508 2024-05-16 19:14:01.084860 sema4ai_actions-0.6.0/src/sema4ai/actions/__init__.py
+-rw-r--r--   0        0        0       80 2024-05-16 19:14:01.084860 sema4ai_actions-0.6.0/src/sema4ai/actions/__main__.py
+-rw-r--r--   0        0        0    15553 2024-05-16 19:14:01.084860 sema4ai_actions-0.6.0/src/sema4ai/actions/_action.py
+-rw-r--r--   0        0        0     7567 2024-05-16 19:14:01.084860 sema4ai_actions-0.6.0/src/sema4ai/actions/_action_context.py
+-rw-r--r--   0        0        0    11151 2024-05-16 19:14:01.084860 sema4ai_actions-0.6.0/src/sema4ai/actions/_args_dispatcher.py
+-rw-r--r--   0        0        0     1494 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_callback.py
+-rw-r--r--   0        0        0     8339 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_collect_actions.py
+-rw-r--r--   0        0        0    32316 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_commands.py
+-rw-r--r--   0        0        0     2276 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_config.py
+-rw-r--r--   0        0        0      336 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_constants.py
+-rw-r--r--   0        0        0        0 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_customization/__init__.py
+-rw-r--r--   0        0        0     2722 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_customization/_extension_points.py
+-rw-r--r--   0        0        0     9922 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_customization/_plugin_manager.py
+-rw-r--r--   0        0        0      220 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_exceptions.py
+-rw-r--r--   0        0        0     5638 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_fixtures.py
+-rw-r--r--   0        0        0     2500 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_hooks.py
+-rw-r--r--   0        0        0     7491 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_interrupts.py
+-rw-r--r--   0        0        0     1367 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_lifecycle.py
+-rw-r--r--   0        0        0    13368 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_lint_action.py
+-rw-r--r--   0        0        0     1082 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_log_auto_setup.py
+-rw-r--r--   0        0        0     3074 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_log_output_setup.py
+-rw-r--r--   0        0        0     6342 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_managed_parameters.py
+-rw-r--r--   0        0        0     6023 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_protocols.py
+-rw-r--r--   0        0        0    13813 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_remove_refs.py
+-rw-r--r--   0        0        0     2906 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_request.py
+-rw-r--r--   0        0        0     1023 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_request_impl.py
+-rw-r--r--   0        0        0     6615 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_secret/__init__.py
+-rw-r--r--   0        0        0     5153 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_secret/_oauth2_secret.py
+-rw-r--r--   0        0        0     2678 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_secret/_secret.py
+-rw-r--r--   0        0        0     3134 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/api.py
+-rw-r--r--   0        0        0     2277 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/cli.py
+-rw-r--r--   0        0        0        0 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/py.typed
+-rw-r--r--   0        0        0     3788 1970-01-01 00:00:00.000000 sema4ai_actions-0.6.0/PKG-INFO
```

### Comparing `sema4ai_actions-0.5.0/README.md` & `sema4ai_actions-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.5.0/pyproject.toml` & `sema4ai_actions-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sema4ai-actions"
-version = "0.5.0"
+version = "0.6.0"
 description = "Sema4AI Actions"
 authors = [
 	"Fabio Z. <fabio@robocorp.com>",
 ]
 readme = "README.md"
 repository = "https://github.com/Sema4AI/actions/"
 license = "Apache-2.0"
```

### Comparing `sema4ai_actions-0.5.0/src/sema4ai/actions/__init__.py` & `sema4ai_actions-0.6.0/src/sema4ai/actions/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,17 +34,17 @@
 
 from pathlib import Path
 from typing import Callable, Optional, overload
 
 from ._fixtures import setup, teardown
 from ._protocols import IAction, Status
 from ._request import Request
-from ._secret import Secret
+from ._secret import OAuth2Secret, Secret
 
-__version__ = "0.5.0"
+__version__ = "0.6.0"
 version_info = [int(x) for x in __version__.split(".")]
 
 
 @overload
 def action(func: Callable) -> Callable:
     ...
 
@@ -189,14 +189,15 @@
     return _action.get_current_action()
 
 
 __all__ = [
     "IAction",
     "Request",
     "Secret",
+    "OAuth2Secret",
     "Status",
     "action",
     "action_cache",
     "get_current_action",
     "get_output_dir",
     "session_cache",
     "setup",
```

### Comparing `sema4ai_actions-0.5.0/src/sema4ai/actions/_action.py` & `sema4ai_actions-0.6.0/src/sema4ai/actions/_action.py`

 * *Files 14% similar despite different names*

```diff
@@ -104,25 +104,103 @@
 
         if param_name:
             properties["title"] = param_name.replace("_", " ").title()
         return properties
 
     @property
     def managed_params_schema(self) -> Dict[str, Any]:
+        from typing import get_args, get_origin
+
         from sema4ai.actions._commands import _get_managed_param_type, _is_managed_param
+        from sema4ai.actions._exceptions import ActionsCollectError
 
         managed_params_schema: Dict[str, Any] = {}
         sig = inspect.signature(self.method)
 
         param_name_to_description = self._get_param_name_to_description()
         for param in sig.parameters.values():
             if _is_managed_param(self._pm, param.name, param=param):
                 tp = _get_managed_param_type(self._pm, param.name, param=param).__name__
 
-                dct = {"type": tp}
+                dct: dict[str, Any] = {"type": tp}
+                if tp == "OAuth2Secret":
+                    # In this case we need to make some introspection to get additional information
+                    # on the type (provider, scopes, ...)
+                    annotation_args = get_args(param.annotation)
+                    error_message = f"""
+Invalid OAuth2Secret annotation found.
+
+The OAuth2Secret must be parametrized with 2 arguments, 
+the first being a Literal with the provider name 
+(i.e.: `Literal["google"]`) 
+and the second a list with one Literal with the (multiple) scopes that are required
+(i.e.: `list[Literal["scope1", "scope2", ...]])
+
+Full Example for a parameter named `google_secret` requiring google sheets 
+and google drive scopes:
+
+google_secret: OAuth2Secret[
+    Literal["google"],
+    list[
+        Literal[
+            "https://www.googleapis.com/auth/drive.readonly",
+            "https://www.googleapis.com/auth/spreadsheets.readonly",
+        ]
+    ],
+]
+
+File with @action: {self.filename}
+@action name: {self.name}
+"""
+                    if not annotation_args or len(annotation_args) != 2:
+                        raise ActionsCollectError(error_message)
+
+                    provider = annotation_args[0]
+                    scopes = annotation_args[1]
+                    if get_origin(provider) != Literal:
+                        raise ActionsCollectError(
+                            f"First parameter is not a Literal.\n{error_message}"
+                        )
+                    if get_origin(scopes) not in (list, List):
+                        raise ActionsCollectError(
+                            f"Second parameter is not a list.\n{error_message}"
+                        )
+                    provider_args = get_args(provider)
+                    if not provider_args or len(provider_args) != 1:
+                        raise ActionsCollectError(
+                            f"First parameter does not have a single provider argument.\n{error_message}"
+                        )
+                    provider_str = provider_args[0]
+                    if not isinstance(provider_str, str):
+                        raise ActionsCollectError(
+                            f"First parameter Literal does not have a string.\n{error_message}"
+                        )
+
+                    dct["provider"] = provider_str
+
+                    scope_args = get_args(scopes)
+                    if not scope_args or len(scope_args) != 1:
+                        raise ActionsCollectError(
+                            f"Second parameter is not a list with a single Literal.\n{error_message}"
+                        )
+
+                    scope_args_literal = scope_args[0]
+                    if get_origin(scope_args_literal) != Literal:
+                        raise ActionsCollectError(
+                            f"Second parameter is not a list with a single Literal.\n{error_message}"
+                        )
+
+                    scope_strs = get_args(scope_args_literal)
+                    for entry in scope_strs:
+                        if not isinstance(entry, str):
+                            raise ActionsCollectError(
+                                f"Second parameter is not a list with a literal with strings.\n{error_message}"
+                            )
+
+                    dct["scopes"] = scope_strs
 
                 desc = param_name_to_description.get(param.name)
                 if desc:
                     dct["description"] = desc
                 managed_params_schema[param.name] = dct
 
         return managed_params_schema
```

### Comparing `sema4ai_actions-0.5.0/src/sema4ai/actions/_action_context.py` & `sema4ai_actions-0.6.0/src/sema4ai/actions/_action_context.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.5.0/src/sema4ai/actions/_args_dispatcher.py` & `sema4ai_actions-0.6.0/src/sema4ai/actions/_args_dispatcher.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.5.0/src/sema4ai/actions/_callback.py` & `sema4ai_actions-0.6.0/src/sema4ai/actions/_callback.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.5.0/src/sema4ai/actions/_collect_actions.py` & `sema4ai_actions-0.6.0/src/sema4ai/actions/_collect_actions.py`

 * *Files 11% similar despite different names*

```diff
@@ -143,14 +143,16 @@
     pm: PluginManager,
     path: Path,
     action_names: Sequence[str] = (),
     glob: Optional[str] = None,
 ) -> Iterator[IAction]:
     """
     Note: collecting actions is not thread-safe.
+
+    Raises: ActionsCollectError
     """
     from sema4ai.actions import _constants, _hooks
 
     path = path.absolute()
     action_names_as_set = set(action_names)
 
     _hooks.before_collect_actions(path, action_names_as_set)
@@ -158,19 +160,19 @@
     def accept_action(action: IAction):
         if not action_names:
             return True
 
         return action.name in action_names
 
     def on_func_found(func, options: Dict):
-        from sema4ai.actions._exceptions import RobocorpActionsError
+        from sema4ai.actions._exceptions import ActionsError
 
         key = (func.__code__.co_name, func.__code__.co_filename)
         if key in _found_as_set:
-            raise RobocorpActionsError(
+            raise ActionsError(
                 f"Error: an action with the name '{func.__code__.co_name}' was "
                 + f"already found in: {func.__code__.co_filename}."
             )
         _found_as_set.add(key)
 
         _methods_marked_as_actions_found.append(
             (
@@ -210,22 +212,20 @@
 
         elif path.is_file():
             root = _get_root(path, is_dir=False)
             with _add_to_sys_path_0(root):
                 import_path(path, root=root)
 
         else:
-            from ._exceptions import RobocorpActionsCollectError
+            from ._exceptions import ActionsCollectError
 
             if not path.exists():
-                raise RobocorpActionsCollectError(f"Path: {path} does not exist")
+                raise ActionsCollectError(f"Path: {path} does not exist")
 
-            raise RobocorpActionsCollectError(
-                f"Expected {path} to map to a directory or file."
-            )
+            raise ActionsCollectError(f"Expected {path} to map to a directory or file.")
 
     from sema4ai.actions._action import Action
 
     for method, options in _methods_marked_as_actions_found:
         module_name = method.__module__
         module_file = method.__code__.co_filename
```

### Comparing `sema4ai_actions-0.5.0/src/sema4ai/actions/_commands.py` & `sema4ai_actions-0.6.0/src/sema4ai/actions/_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     Args:
         path: The path (file or directory) from where actions should be collected.
     """
     from contextlib import redirect_stdout
 
     from sema4ai.actions._action import Context
     from sema4ai.actions._collect_actions import collect_actions
+    from sema4ai.actions._exceptions import ActionsCollectError
     from sema4ai.actions._protocols import ActionsListActionTypedDict
 
     p = Path(path)
     context = Context()
     if not p.exists():
         context.show_error(f"Path: {path} does not exist")
         return 1
@@ -60,31 +61,39 @@
     original_stdout = sys.stdout
     if __stream__ is not None:
         write_to = __stream__
     else:
         write_to = original_stdout
 
     with redirect_stdout(sys.stderr):
-        action: IAction
-        actions_found: List[ActionsListActionTypedDict] = []
-        for action in collect_actions(pm, p, glob=glob):
-            entry: ActionsListActionTypedDict = {
-                "name": action.name,
-                "line": action.lineno,
-                "file": action.filename,
-                "docs": getattr(action.method, "__doc__") or "",
-                "input_schema": action.input_schema,
-                "output_schema": action.output_schema,
-                "managed_params_schema": action.managed_params_schema,
-                "options": action.options,
-            }
-            actions_found.append(entry)
+        try:
+            action: IAction
+            actions_found: List[ActionsListActionTypedDict] = []
+            for action in collect_actions(pm, p, glob=glob):
+                entry: ActionsListActionTypedDict = {
+                    "name": action.name,
+                    "line": action.lineno,
+                    "file": action.filename,
+                    "docs": getattr(action.method, "__doc__") or "",
+                    "input_schema": action.input_schema,
+                    "output_schema": action.output_schema,
+                    "managed_params_schema": action.managed_params_schema,
+                    "options": action.options,
+                }
+                actions_found.append(entry)
+
+            write_to.write(json.dumps(actions_found))
+            write_to.flush()
+        except Exception as e:
+            if not isinstance(e, ActionsCollectError):
+                traceback.print_exc()
+            else:
+                context.show_error(str(e))
+            return 1
 
-        write_to.write(json.dumps(actions_found))
-        write_to.flush()
     return 0
 
 
 def _os_exit(retcode: int):
     """
     Kills subprocesses and exits with the given returncode.
     """
@@ -220,15 +229,15 @@
         read_pyproject_toml,
         read_robocorp_auto_log_config,
     )
 
     from sema4ai.actions._action import Context, set_current_action
     from sema4ai.actions._collect_actions import collect_actions
     from sema4ai.actions._config import RunConfig, set_config
-    from sema4ai.actions._exceptions import RobocorpActionsCollectError
+    from sema4ai.actions._exceptions import ActionsCollectError
     from sema4ai.actions._hooks import (
         after_action_run,
         after_all_actions_run,
         before_action_run,
         before_all_actions_run,
     )
     from sema4ai.actions._interrupts import interrupt_on_timeout
@@ -414,23 +423,23 @@
                         )
 
                     actions: List[IAction] = list(
                         collect_actions(pm, p, action_names, glob)
                     )
 
                     if not actions:
-                        raise RobocorpActionsCollectError(
+                        raise ActionsCollectError(
                             f"Did not find any actions in: {path}"
                         )
                 except Exception as e:
                     run_status = "ERROR"
                     setup_message = str(e)
 
                     log.exception()
-                    if not isinstance(e, RobocorpActionsCollectError):
+                    if not isinstance(e, ActionsCollectError):
                         traceback.print_exc()
                     else:
                         context.show_error(setup_message)
 
                     retcode = 1
                     return retcode
                 finally:
```

### Comparing `sema4ai_actions-0.5.0/src/sema4ai/actions/_config.py` & `sema4ai_actions-0.6.0/src/sema4ai/actions/_config.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.5.0/src/sema4ai/actions/_customization/_extension_points.py` & `sema4ai_actions-0.6.0/src/sema4ai/actions/_customization/_extension_points.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.5.0/src/sema4ai/actions/_customization/_plugin_manager.py` & `sema4ai_actions-0.6.0/src/sema4ai/actions/_customization/_plugin_manager.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.5.0/src/sema4ai/actions/_fixtures.py` & `sema4ai_actions-0.6.0/src/sema4ai/actions/_fixtures.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.5.0/src/sema4ai/actions/_hooks.py` & `sema4ai_actions-0.6.0/src/sema4ai/actions/_hooks.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.5.0/src/sema4ai/actions/_interrupts.py` & `sema4ai_actions-0.6.0/src/sema4ai/actions/_interrupts.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.5.0/src/sema4ai/actions/_lifecycle.py` & `sema4ai_actions-0.6.0/src/sema4ai/actions/_lifecycle.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.5.0/src/sema4ai/actions/_lint_action.py` & `sema4ai_actions-0.6.0/src/sema4ai/actions/_lint_action.py`

 * *Files 4% similar despite different names*

```diff
@@ -274,14 +274,22 @@
                             f"Parameter: `{arg.arg}` documentation not found in docstring. "
                             "Please update docstring to add it (as it will be added to the "
                             "secrets metadata explaining the secret).",
                         )
 
                 continue
 
+            # Note: at this time we don't do handling for OAuth2 parameters here because
+            # we currently don't follow aliases, so, in practice it'll consider OAuth2
+            # parameters (when using static analysis) as any other parameter.
+            # -- given that the only difference is a better error message, this is
+            # a reasonable compromise at this point (in runtime the types are
+            # resolved properly and the actual type is then verified to inject
+            # properly as a managed parameter).
+
             if not desc:
                 yield _make_error(
                     arg,
                     f"Parameter: `{arg.arg}` documentation not found in docstring. "
                     "Please update docstring to add it as an LLM needs this info "
                     "to understand what needs to be passed to call this action.",
                 )
@@ -298,15 +306,22 @@
 def iter_lint_errors(
     action_contents_file: Union[str, bytes], pm: Optional[PluginManager] = None
 ) -> Iterator[Error]:
     ast = ast_module.parse(action_contents_file, "<string>")
     for _stack, node in _iter_nodes(ast, recursive=False):
         if isinstance(node, ast_module.FunctionDef):
             for decorator in node.decorator_list:
-                if isinstance(decorator, ast_module.Name) and decorator.id == "action":
+                if (
+                    isinstance(decorator, ast_module.Name) and decorator.id == "action"
+                ) or (
+                    isinstance(decorator, ast_module.Attribute)
+                    and decorator.attr == "action"
+                    and isinstance(decorator.value, ast_module.Name)
+                    and decorator.value.id == "actions"
+                ):
                     # We found an @action. Do the needed checks.
 
                     # Check for docstring
                     docstring: str = ast_module.get_docstring(node) or ""
                     if docstring:
                         docstring = docstring.strip()
```

### Comparing `sema4ai_actions-0.5.0/src/sema4ai/actions/_log_auto_setup.py` & `sema4ai_actions-0.6.0/src/sema4ai/actions/_log_auto_setup.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.5.0/src/sema4ai/actions/_log_output_setup.py` & `sema4ai_actions-0.6.0/src/sema4ai/actions/_log_output_setup.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.5.0/src/sema4ai/actions/_managed_parameters.py` & `sema4ai_actions-0.6.0/src/sema4ai/actions/_managed_parameters.py`

 * *Files 22% similar despite different names*

```diff
@@ -27,28 +27,34 @@
     def is_managed_param(
         self,
         param_name: str,
         *,
         node: Optional[FunctionDef] = None,
         param: Optional[inspect.Parameter] = None,
     ) -> bool:
-        from sema4ai.actions._secret import Secret
+        from sema4ai.actions._secret import (
+            is_oauth2_secret_subclass,
+            is_secret_subclass,
+        )
 
         if param_name in self._param_name_to_instance:
             return True
 
         if node is not None:
             assert (
                 param is None
             ), "Either node or param is expected, but not both at the same time."
             return self._is_secret_node(param_name, node)
 
         elif param is not None:
-            if param.annotation and issubclass(param.annotation, Secret):
-                return True
+            if param.annotation:
+                if is_secret_subclass(param.annotation):
+                    return True
+                if is_oauth2_secret_subclass(param.annotation):
+                    return True
 
         else:
             raise AssertionError("Either node or param must be passed.")
 
         return False
 
     def _is_secret_node(self, param_name: str, node: FunctionDef) -> bool:
@@ -73,44 +79,62 @@
     def inject_managed_params(
         self,
         sig: inspect.Signature,
         new_kwargs: Dict[str, Any],
         original_kwargs: Dict[str, Any],
     ) -> Dict[str, Any]:
         from sema4ai.actions._action_context import ActionContext
-        from sema4ai.actions._secret import Secret
+        from sema4ai.actions._request import Request
+        from sema4ai.actions._secret import (
+            OAuth2Secret,
+            Secret,
+            is_oauth2_secret_subclass,
+            is_secret_subclass,
+        )
 
         use_kwargs = new_kwargs.copy()
 
         request = new_kwargs.get("request")
         if request is None:
+            req = original_kwargs.get("request")
+            if req is not None:
+                request = Request.model_validate(req)
+        if request is None:
             request = self._param_name_to_instance.get("request")
 
         x_action_context = ActionContext.from_request(request)
 
         for param in sig.parameters.values():
             if (
                 param.name not in use_kwargs
                 and param.name in self._param_name_to_instance
             ):
                 use_kwargs[param.name] = self._param_name_to_instance[param.name]
 
-            elif param.annotation and issubclass(param.annotation, Secret):
-                # Handle a secret
-                secret_value = original_kwargs.get(param.name)
-
-                if secret_value is not None:
-                    # Gotten directly from the input.json (or command line)
-                    # as a value in the root.
-                    use_kwargs[param.name] = Secret.model_validate(secret_value)
-
-                elif x_action_context is not None:
-                    use_kwargs[param.name] = Secret.from_action_context(
-                        x_action_context, f"secrets/{param.name}"
-                    )
+            elif param.annotation:
+                use_class: Optional[Any] = None
+                if is_secret_subclass(param.annotation):
+                    use_class = Secret
+
+                elif is_oauth2_secret_subclass(param.annotation):
+                    use_class = OAuth2Secret
+
+                if use_class is not None:
+                    # Handle a secret
+                    secret_value = original_kwargs.get(param.name)
+
+                    if secret_value is not None:
+                        # Gotten directly from the input.json (or command line)
+                        # as a value in the root.
+                        use_kwargs[param.name] = use_class.model_validate(secret_value)
+
+                    elif x_action_context is not None:
+                        use_kwargs[param.name] = use_class.from_action_context(
+                            x_action_context, f"secrets/{param.name}"
+                        )
 
         return use_kwargs
 
     @overload
     def get_managed_param_type(
         self, param_name: str, *, param: inspect.Parameter
     ) -> type:
@@ -124,29 +148,38 @@
         self,
         param_name: str,
         *,
         param: Optional[inspect.Parameter] = None,
         node: Optional[FunctionDef] = None,
     ) -> type | str:
         from sema4ai.actions._request import Request
-        from sema4ai.actions._secret import Secret
+        from sema4ai.actions._secret import (
+            OAuth2Secret,
+            Secret,
+            is_oauth2_secret_subclass,
+            is_secret_subclass,
+        )
 
         if param_name == "request":
             return Request
 
         if node is None and param is None:
             raise ValueError("Either node or param are required.")
         if node is not None and param is not None:
             raise ValueError(
                 "Either node or param is expected, but not both at the same time."
             )
 
         if param is not None:
-            if param.annotation and issubclass(param.annotation, Secret):
-                return Secret
+            if param.annotation:
+                if is_secret_subclass(param.annotation):
+                    return Secret
+
+                if is_oauth2_secret_subclass(param.annotation):
+                    return OAuth2Secret
         else:
             assert node is not None
             if self._is_secret_node(param_name, node):
                 return "Secret"
 
         raise RuntimeError(
             f"Unable to get managed parameter type for parameter: {param}"
```

### Comparing `sema4ai_actions-0.5.0/src/sema4ai/actions/_protocols.py` & `sema4ai_actions-0.6.0/src/sema4ai/actions/_protocols.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.5.0/src/sema4ai/actions/_remove_refs.py` & `sema4ai_actions-0.6.0/src/sema4ai/actions/_remove_refs.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.5.0/src/sema4ai/actions/_request.py` & `sema4ai_actions-0.6.0/src/sema4ai/actions/_request.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.5.0/src/sema4ai/actions/_request_impl.py` & `sema4ai_actions-0.6.0/src/sema4ai/actions/_request_impl.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.5.0/src/sema4ai/actions/_secret.py` & `sema4ai_actions-0.6.0/src/sema4ai/actions/_secret/_oauth2_secret.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,102 +1,49 @@
-import typing
+from typing import Any, Optional
 
-if typing.TYPE_CHECKING:
-    from sema4ai.actions._action_context import ActionContext
+from sema4ai.actions._action_context import ActionContext
+from sema4ai.actions._secret import JSONValue, OAuth2Secret, ProviderT, ScopesT
 
 
-class Secret:
-    """
-    This class should be used to receive secrets.
-
-    The way to use it is by declaring a variable with the 'Secret' type
-    in the @action.
-
-    Example:
-
-        ```
-        from sema4ai.actions import action, Secret
-
-        @action
-        def my_action(password: Secret):
-            login(password.value)
-        ```
+class _BaseInternalOAuth2Secret(OAuth2Secret):
+    def __init__(
+        self,
+        provider: ProviderT,
+        scopes: ScopesT,
+        access_token: str,
+        metadata: JSONValue = None,
+    ):
+        self._provider = provider
+        self._scopes = scopes
+        self._access_token = access_token
+        self._metadata = metadata
 
-    Note: this class is abstract and is not meant to be instanced by clients.
-        An instance can be created from one of the factory methods (`model_validate`
-        or `from_action_context`).
-    """
-
-    @classmethod
-    def model_validate(cls, value: str) -> "Secret":
-        """
-        Creates a secret given a string (expected when the user
-        is passing the arguments using a json input).
-
-        Args:
-            value: The raw-text value to be used in the secret.
-
-        Return: A Secret instance with the given value.
-
-        Note: the model_validate method is used for compatibility with
-            the pydantic API.
-        """
-        return _RawSecret(value)
-
-    @classmethod
-    def from_action_context(
-        cls, action_context: "ActionContext", path: str
-    ) -> "Secret":
-        """
-        Creates a secret given the action context (which may be encrypted
-        in memory until the actual secret value is requested).
-
-        Args:
-            action_context: The action context which has the secret.
-
-            path: The path inside of the action context for the secret data
-            requested (Example: 'secrets/my_secret_name').
+        from robocorp import log
 
-        Return: A Secret instance collected from the passed action context.
-        """
-        return _SecretInActionContext(action_context, path)
+        log.hide_from_output(access_token)
+        log.hide_from_output(repr(access_token))
 
     @property
-    def value(self) -> str:
-        raise NotImplementedError(
-            "The Secret class is abstract and should not be directly used."
-        )
-
-
-class _RawSecret(Secret):
-    """
-    Internal API to wrap a secret which is not passed encrypted.
-    """
+    def provider(self) -> str:
+        return self._provider
 
-    def __init__(self, value: str):
-        """
-        Args:
-            value: The secret value to be wrapped in this class (note that
-                it's automatically hidden in the logs).
-        """
-        from robocorp import log
+    @property
+    def scopes(self) -> list[str]:
+        return self._scopes
 
-        log.hide_from_output(value)
-        log.hide_from_output(repr(value))
-        self.__value = value
+    @property
+    def access_token(self) -> str:
+        return self._access_token
 
     @property
-    def value(self) -> str:
-        """
-        Provides the actual secret wrapped in this class.
-        """
-        return self.__value
+    def metadata(self) -> JSONValue:
+        return self._metadata
 
 
-class _SecretInActionContext(Secret):
+class _OAuth2SecretInActionContext(_BaseInternalOAuth2Secret):
     """
     Internal API to wrap a secret which is passed encrypted.
     """
 
     def __init__(self, action_context: "ActionContext", path: str):
         """
         Args:
@@ -106,19 +53,15 @@
         """
         if not path:
             raise RuntimeError("A valid path must be passed.")
 
         self._action_context = action_context
         self._paths = path.split("/")
 
-    @property
-    def value(self) -> str:
-        """
-        Provides the actual secret wrapped in this class.
-        """
+    def _get_dict_in_action_context(self) -> dict:
         from robocorp import log
 
         with log.suppress():
             dct = self._action_context.value
 
             v = None
             for path in self._paths:
@@ -137,14 +80,92 @@
 
             dct = None  # Remove from context
             if v is None:
                 raise RuntimeError(
                     f"Error. Path ({self._paths}) invalid for the action context."
                 )
 
-            if not isinstance(v, str):
+            if not isinstance(v, dict):
                 del v
                 raise RuntimeError(
-                    f"Error. Path ({self._paths}) did not map to a string in the action context."
+                    f"Error. Path ({self._paths}) did not map to a dict in the action context."
                 )
 
             return v
+
+    @property
+    def access_token(self) -> str:
+        """
+        Provides the actual access_token wrapped in this class.
+        """
+        from robocorp import log
+
+        with log.suppress():
+            dct = self._get_dict_in_action_context()
+            ret = dct["access_token"]
+            log.hide_from_output(ret)
+            log.hide_from_output(repr(ret))
+            return ret
+
+    @property
+    def provider(self) -> str:
+        """
+        Provides the actual provider wrapped in this class.
+        """
+        from robocorp import log
+
+        with log.suppress():
+            dct = self._get_dict_in_action_context()
+            return dct["provider"]
+
+    @property
+    def scopes(self) -> list[str]:
+        """
+        Provides the actual scopes wrapped in this class.
+        """
+        from robocorp import log
+
+        with log.suppress():
+            dct = self._get_dict_in_action_context()
+            return dct["scopes"]
+
+    @property
+    def metadata(self) -> Optional[Any]:
+        """
+        Provides the actual metadata wrapped in this class.
+        """
+        from robocorp import log
+
+        with log.suppress():
+            dct = self._get_dict_in_action_context()
+            return dct.get("metadata")
+
+
+class _RawOauth2Secret(_BaseInternalOAuth2Secret):
+    """
+    Internal API to wrap a secret which is not passed encrypted.
+    """
+
+    def __init__(self, value: dict):
+        """
+        Args:
+            value: A dict with the values meant to be wrapped in this class.
+        """
+
+        access_token = value.get("access_token")
+        if not access_token:
+            raise KeyError(
+                "Error. The `access_token` key is required to build an OAuth2Secret, but it wasn't passed."
+            )
+        provider = value.get("provider")
+        if not provider:
+            raise KeyError(
+                "Error. The `provider` key is required to build an OAuth2Secret, but it wasn't passed."
+            )
+        scopes = value.get("scopes")
+        if not scopes:
+            raise KeyError(
+                "Error. The `scopes` key is required to build an OAuth2Secret, but it wasn't passed."
+            )
+
+        metadata = value.get("metadata")  # This is optional
+        super().__init__(provider, scopes, access_token, metadata)
```

### Comparing `sema4ai_actions-0.5.0/src/sema4ai/actions/api.py` & `sema4ai_actions-0.6.0/src/sema4ai/actions/api.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.5.0/src/sema4ai/actions/cli.py` & `sema4ai_actions-0.6.0/src/sema4ai/actions/cli.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.5.0/PKG-INFO` & `sema4ai_actions-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sema4ai-actions
-Version: 0.5.0
+Version: 0.6.0
 Summary: Sema4AI Actions
 Home-page: https://github.com/Sema4AI/actions/
 License: Apache-2.0
 Author: Fabio Z.
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

