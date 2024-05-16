# Comparing `tmp/cyclopts-2.6.1.tar.gz` & `tmp/cyclopts-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyclopts-2.6.1.tar", max compression
+gzip compressed data, was "cyclopts-2.6.2.tar", max compression
```

## Comparing `cyclopts-2.6.1.tar` & `cyclopts-2.6.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    11357 2024-04-16 22:38:05.108343 cyclopts-2.6.1/LICENSE
--rw-r--r--   0        0        0    10910 2024-04-16 22:38:05.108343 cyclopts-2.6.1/README.md
--rw-r--r--   0        0        0      974 2024-04-16 22:38:17.328337 cyclopts-2.6.1/cyclopts/__init__.py
--rw-r--r--   0        0        0    12220 2024-04-16 22:38:05.112343 cyclopts-2.6.1/cyclopts/_convert.py
--rw-r--r--   0        0        0    13552 2024-04-16 22:38:05.112343 cyclopts-2.6.1/cyclopts/bind.py
--rw-r--r--   0        0        0    34683 2024-04-16 22:38:05.112343 cyclopts-2.6.1/cyclopts/core.py
--rw-r--r--   0        0        0     9666 2024-04-16 22:38:05.112343 cyclopts-2.6.1/cyclopts/exceptions.py
--rw-r--r--   0        0        0     4989 2024-04-16 22:38:05.112343 cyclopts-2.6.1/cyclopts/group.py
--rw-r--r--   0        0        0     2639 2024-04-16 22:38:05.112343 cyclopts-2.6.1/cyclopts/group_extractors.py
--rw-r--r--   0        0        0     9889 2024-04-16 22:38:05.112343 cyclopts-2.6.1/cyclopts/help.py
--rw-r--r--   0        0        0     7991 2024-04-16 22:38:05.112343 cyclopts-2.6.1/cyclopts/parameter.py
--rw-r--r--   0        0        0      190 2024-04-16 22:38:05.112343 cyclopts-2.6.1/cyclopts/protocols.py
--rw-r--r--   0        0        0        0 2024-04-16 22:38:05.112343 cyclopts-2.6.1/cyclopts/py.typed
--rw-r--r--   0        0        0     9514 2024-04-16 22:38:05.112343 cyclopts-2.6.1/cyclopts/resolve.py
--rw-r--r--   0        0        0     3851 2024-04-16 22:38:05.112343 cyclopts-2.6.1/cyclopts/types.py
--rw-r--r--   0        0        0     6027 2024-04-16 22:38:05.112343 cyclopts-2.6.1/cyclopts/utils.py
--rw-r--r--   0        0        0      205 2024-04-16 22:38:05.112343 cyclopts-2.6.1/cyclopts/validators/__init__.py
--rw-r--r--   0        0        0     1233 2024-04-16 22:38:05.116343 cyclopts-2.6.1/cyclopts/validators/_group.py
--rw-r--r--   0        0        0     1459 2024-04-16 22:38:05.116343 cyclopts-2.6.1/cyclopts/validators/_number.py
--rw-r--r--   0        0        0     1298 2024-04-16 22:38:05.116343 cyclopts-2.6.1/cyclopts/validators/_path.py
--rw-r--r--   0        0        0     4458 2024-04-16 22:38:17.324337 cyclopts-2.6.1/pyproject.toml
--rw-r--r--   0        0        0    11886 1970-01-01 00:00:00.000000 cyclopts-2.6.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-16 12:47:00.568541 cyclopts-2.6.2/LICENSE
+-rw-r--r--   0        0        0    10910 2024-05-16 12:47:00.568541 cyclopts-2.6.2/README.md
+-rw-r--r--   0        0        0      974 2024-05-16 12:47:27.244817 cyclopts-2.6.2/cyclopts/__init__.py
+-rw-r--r--   0        0        0    12184 2024-05-16 12:47:00.572541 cyclopts-2.6.2/cyclopts/_convert.py
+-rw-r--r--   0        0        0    13560 2024-05-16 12:47:00.572541 cyclopts-2.6.2/cyclopts/bind.py
+-rw-r--r--   0        0        0    35336 2024-05-16 12:47:00.572541 cyclopts-2.6.2/cyclopts/core.py
+-rw-r--r--   0        0        0     9682 2024-05-16 12:47:00.572541 cyclopts-2.6.2/cyclopts/exceptions.py
+-rw-r--r--   0        0        0     4989 2024-05-16 12:47:00.572541 cyclopts-2.6.2/cyclopts/group.py
+-rw-r--r--   0        0        0     2639 2024-05-16 12:47:00.572541 cyclopts-2.6.2/cyclopts/group_extractors.py
+-rw-r--r--   0        0        0    12421 2024-05-16 12:47:00.572541 cyclopts-2.6.2/cyclopts/help.py
+-rw-r--r--   0        0        0     8033 2024-05-16 12:47:00.572541 cyclopts-2.6.2/cyclopts/parameter.py
+-rw-r--r--   0        0        0      182 2024-05-16 12:47:00.572541 cyclopts-2.6.2/cyclopts/protocols.py
+-rw-r--r--   0        0        0        0 2024-05-16 12:47:00.572541 cyclopts-2.6.2/cyclopts/py.typed
+-rw-r--r--   0        0        0     9514 2024-05-16 12:47:00.572541 cyclopts-2.6.2/cyclopts/resolve.py
+-rw-r--r--   0        0        0     3851 2024-05-16 12:47:00.572541 cyclopts-2.6.2/cyclopts/types.py
+-rw-r--r--   0        0        0     6027 2024-05-16 12:47:00.572541 cyclopts-2.6.2/cyclopts/utils.py
+-rw-r--r--   0        0        0      205 2024-05-16 12:47:00.572541 cyclopts-2.6.2/cyclopts/validators/__init__.py
+-rw-r--r--   0        0        0     1233 2024-05-16 12:47:00.572541 cyclopts-2.6.2/cyclopts/validators/_group.py
+-rw-r--r--   0        0        0     1274 2024-05-16 12:47:00.572541 cyclopts-2.6.2/cyclopts/validators/_number.py
+-rw-r--r--   0        0        0     1298 2024-05-16 12:47:00.572541 cyclopts-2.6.2/cyclopts/validators/_path.py
+-rw-r--r--   0        0        0     4507 2024-05-16 12:47:27.240816 cyclopts-2.6.2/pyproject.toml
+-rw-r--r--   0        0        0    11886 1970-01-01 00:00:00.000000 cyclopts-2.6.2/PKG-INFO
```

### Comparing `cyclopts-2.6.1/LICENSE` & `cyclopts-2.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cyclopts-2.6.1/README.md` & `cyclopts-2.6.2/README.md`

 * *Files identical despite different names*

### Comparing `cyclopts-2.6.1/cyclopts/__init__.py` & `cyclopts-2.6.2/cyclopts/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Don't manually change, let poetry-dynamic-versioning handle it.
-__version__ = "2.6.1"
+__version__ = "2.6.2"
 
 __all__ = [
     "App",
     "CoercionError",
     "CommandCollisionError",
     "CycloptsError",
     "Dispatcher",
```

### Comparing `cyclopts-2.6.1/cyclopts/_convert.py` & `cyclopts-2.6.2/cyclopts/_convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,23 +16,23 @@
     Tuple,
     Type,
     Union,
     get_args,
     get_origin,
 )
 
+from cyclopts.exceptions import CoercionError
+from cyclopts.utils import default_name_transform, is_union
+
 if sys.version_info < (3, 9):
     from typing_extensions import Annotated  # pragma: no cover
 else:
     from typing import Annotated  # pragma: no cover
 
 
-from cyclopts.exceptions import CoercionError
-from cyclopts.utils import default_name_transform, is_union
-
 if TYPE_CHECKING:
     from cyclopts.parameter import Parameter
 
 # from types import NoneType is available >=3.10
 NoneType = type(None)
 AnnotatedType = type(Annotated[int, 0])
 
@@ -213,28 +213,28 @@
             raise TypeError(f"Unsupported Type: {type_}")
     else:
         if origin_type in _unsupported_target_types:
             raise TypeError(f"Unsupported Type: {type_}")
     return origin_type
 
 
-def resolve(type_: Type) -> Type:
+def resolve(type_: Any) -> Type:
     """Perform all simplifying resolutions."""
     if type_ is inspect.Parameter.empty:
         return str
 
     type_prev = None
     while type_ != type_prev:
         type_prev = type_
         type_ = resolve_annotated(type_)
         type_ = resolve_optional(type_)
     return type_
 
 
-def resolve_optional(type_: Type) -> Type:
+def resolve_optional(type_: Any) -> Type:
     """Only resolves Union's of None + one other type (i.e. Optional)."""
     # Python will automatically flatten out nested unions when possible.
     # So we don't need to loop over resolution.
 
     if not is_union(get_origin(type_)):
         return type_
 
@@ -249,22 +249,22 @@
         return Union[tuple(resolve_optional(x) for x in non_none_types)]  # pyright: ignore
     else:
         raise NotImplementedError
 
     return type_
 
 
-def resolve_annotated(type_: Type) -> Type:
+def resolve_annotated(type_: Any) -> Type:
     if type(type_) is AnnotatedType:
         type_ = get_args(type_)[0]
     return type_
 
 
 def convert(
-    type_: Type,
+    type_: Any,
     *args: str,
     converter: Optional[Callable[[Type, str], Any]] = None,
     name_transform: Optional[Callable[[str], str]] = None,
 ):
     """Coerce variables into a specified type.
 
     Internally used to coercing string CLI tokens into python builtin types.
@@ -335,15 +335,15 @@
         return convert(type_, args)
     elif len(args) == 1:
         return convert(type_, args[0])
     else:
         return [convert(type_, item) for item in args]
 
 
-def token_count(type_: Union[Type[Any], inspect.Parameter]) -> Tuple[int, bool]:
+def token_count(type_: Any) -> Tuple[int, bool]:
     """The number of tokens after a keyword the parameter should consume.
 
     Parameters
     ----------
     type_: Type
         A type hint/annotation to infer token_count from if not explicitly specified.
```

### Comparing `cyclopts-2.6.1/cyclopts/bind.py` & `cyclopts-2.6.2/cyclopts/bind.py`

 * *Files 1% similar despite different names*

```diff
@@ -379,15 +379,15 @@
             for group, iparams in command.groups_iparams:
                 names = tuple(x.name for x in iparams)
                 for validator in group.validator:  # pyright: ignore
                     validator(**{k: bound.arguments[k] for k in names if k in bound.arguments})
         except (AssertionError, ValueError, TypeError) as e:
             # group will always be set from the above for loop if an exception occurs.
             raise ValidationError(
-                value=e.args[0] if e.args else "", group=group  # pyright: ignore[reportUnboundVariable]
+                value=e.args[0] if e.args else "", group=group  # pyright: ignore[reportPossiblyUnboundVariable]
             ) from e
 
     except CycloptsError as e:
         e.target = command.command
         e.root_input_tokens = tokens
         e.cli2parameter = command.cli2parameter
         e.parameter2cli = command.parameter2cli
```

### Comparing `cyclopts-2.6.1/cyclopts/core.py` & `cyclopts-2.6.2/cyclopts/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,26 +2,31 @@
 import os
 import sys
 import traceback
 from contextlib import suppress
 from copy import copy
 from functools import partial
 from pathlib import Path
-from typing import TYPE_CHECKING, Callable, Dict, Iterable, Iterator, List, Literal, Optional, Tuple, Union
-
-import cyclopts.utils
-
-if sys.version_info < (3, 9):
-    from typing_extensions import Annotated
-else:
-    from typing import Annotated
-
+from typing import (
+    TYPE_CHECKING,
+    Callable,
+    Dict,
+    Iterable,
+    Iterator,
+    List,
+    Literal,
+    Optional,
+    Tuple,
+    TypeVar,
+    Union,
+)
 
 from attrs import define, field
 
+import cyclopts.utils
 from cyclopts.bind import create_bound_arguments, normalize_tokens
 from cyclopts.exceptions import (
     CommandCollisionError,
     CycloptsError,
     InvalidCommandError,
     UnusedCliTokensError,
     ValidationError,
@@ -31,19 +36,34 @@
 from cyclopts.group_extractors import groups_from_app, inverse_groups_from_app
 from cyclopts.help import (
     HelpPanel,
     create_parameter_help_panel,
     format_command_entries,
     format_doc,
     format_usage,
+    resolve_help_format,
 )
 from cyclopts.parameter import Parameter, validate_command
 from cyclopts.protocols import Dispatcher
 from cyclopts.resolve import ResolvedCommand
-from cyclopts.utils import default_name_transform, optional_to_tuple_converter, to_list_converter, to_tuple_converter
+from cyclopts.utils import (
+    default_name_transform,
+    optional_to_tuple_converter,
+    to_list_converter,
+    to_tuple_converter,
+)
+
+T = TypeVar("T", bound=Callable)
+
+
+if sys.version_info < (3, 9):
+    from typing_extensions import Annotated
+else:
+    from typing import Annotated
+
 
 with suppress(ImportError):
     # By importing, makes things like the arrow-keys work.
     import readline  # Not available on windows
 
 if TYPE_CHECKING:
     from rich.console import Console
@@ -185,15 +205,24 @@
     # This can ONLY ever be a Tuple[str, ...]
     _help_flags: Union[str, Iterable[str]] = field(
         default=["--help", "-h"],
         converter=to_tuple_converter,
         alias="help_flags",
         kw_only=True,
     )
-    help_format: Union[None, Literal["plaintext", "markdown", "md", "restructuredtext", "rst"]] = None
+    help_format: Optional[
+        Literal[
+            "markdown",
+            "md",
+            "plaintext",
+            "restructuredtext",
+            "rst",
+            "rich",
+        ]
+    ] = field(default=None, kw_only=True)
 
     # This can ONLY ever be Tuple[Union[Group, str], ...] due to converter.
     # The other types is to make mypy happy for Cyclopts users.
     group: Union[Group, str, Tuple[Union[Group, str], ...]] = field(
         default=None, converter=to_tuple_converter, kw_only=True
     )
 
@@ -294,15 +323,15 @@
                 help="Display this message and exit.",
             )
 
     @property
     def name(self) -> Tuple[str, ...]:
         """Application name(s). Dynamically derived if not previously set."""
         if self._name:
-            return self._name  # pyright: ignore[reportGeneralTypeIssues]
+            return self._name  # pyright: ignore[reportReturnType]
         elif self.default_command is None:
             name = Path(sys.argv[0]).name
             if name == "__main__.py":
                 name = _get_root_module_name()
             return (name,)
         else:
             return (self.name_transform(self.default_command.__name__),)
@@ -417,18 +446,18 @@
             command_chain.append(token)
             command_mapping = _combined_meta_command_mapping(app)
 
         return command_chain, apps, unused_tokens
 
     def command(
         self,
-        obj: Optional[Callable] = None,
+        obj: Optional[T] = None,
         name: Union[None, str, Iterable[str]] = None,
         **kwargs,
-    ) -> Callable:
+    ) -> T:
         """Decorator to register a function as a CLI command.
 
         Parameters
         ----------
         obj: Optional[Callable]
             Function or :class:`App` to be registered as a command.
         name: Union[None, str, Iterable[str]]
@@ -437,15 +466,15 @@
 
             * If registering an :class:`App`, then the app's name.
             * If registering a function, then the function's name.
         `**kwargs`
             Any argument that :class:`App` can take.
         """
         if obj is None:  # Called ``@app.command(...)``
-            return partial(self.command, name=name, **kwargs)
+            return partial(self.command, name=name, **kwargs)  # pyright: ignore[reportReturnType]
 
         if isinstance(obj, App):
             app = obj
 
             if app._name is None and name is None:
                 raise ValueError("Sub-app MUST have a name specified.")
 
@@ -477,26 +506,26 @@
                 raise CommandCollisionError(f'Command "{n}" already registered.')
 
             # Warning: app._name may not align with command name
             self._commands[n] = app
 
         app._parents.append(self)
 
-        return obj
+        return obj  # pyright: ignore[reportReturnType]
 
     def default(
         self,
-        obj: Optional[Callable] = None,
+        obj: Optional[T] = None,
         *,
         converter=None,
         validator=None,
-    ):
+    ) -> T:
         """Decorator to register a function as the default action handler."""
         if obj is None:  # Called ``@app.default_command(...)``
-            return partial(self.default, converter=converter, validator=validator)
+            return partial(self.default, converter=converter, validator=validator)  # pyright: ignore[reportReturnType]
 
         if isinstance(obj, App):  # Registering a sub-App
             raise TypeError("Cannot register a sub-App to default.")
 
         if self.default_command is not None:
             raise CommandCollisionError(f"Default command previously set to {self.default_command}.")
 
@@ -596,15 +625,15 @@
                             validator(**bound.arguments)
                         for command_group in command_groups:
                             for validator in command_group.validator:  # pyright: ignore
                                 validator(**bound.arguments)
                     except (AssertionError, ValueError, TypeError) as e:
                         raise ValidationError(
                             value=e.args[0] if e.args else "",
-                            group=command_group,  # pyright: ignore[reportUnboundVariable]
+                            group=command_group,  # pyright: ignore[reportPossiblyUnboundVariable]
                         ) from e
 
                 else:
                     if unused_tokens:
                         raise InvalidCommandError(unused_tokens=unused_tokens)
                     else:
                         # Running the application with no arguments and no registered
@@ -796,22 +825,18 @@
         #    my-app command COMMAND [ARGS] [OPTIONS]
         if executing_app.usage is None:
             console.print(format_usage(self, command_chain))
         elif executing_app.usage:  # i.e. skip empty-string.
             console.print(executing_app.usage + "\n")
 
         # Print the App/Command's Doc String.
-        # Resolve help_format; None fallsback to parent; non-None overwrites parent.
-        help_format = "restructuredtext"
-        for app in apps:
-            if app.help_format is not None:
-                help_format = app.help_format
+        help_format = resolve_help_format(apps)
         console.print(format_doc(self, executing_app, help_format))
 
-        for help_panel in self._assemble_help_panels(tokens):
+        for help_panel in self._assemble_help_panels(tokens, help_format):
             console.print(help_panel)
 
     def _resolve_command(
         self,
         tokens: Union[None, str, Iterable[str]] = None,
         parse_docstring: bool = True,
     ) -> ResolvedCommand:
@@ -827,18 +852,24 @@
             apps[-1].group_parameters,
             parse_docstring=parse_docstring,
         )
         return resolved_command
 
     def _assemble_help_panels(
         self,
-        tokens: Union[None, str, Iterable[str]] = None,
+        tokens: Union[None, str, Iterable[str]],
+        help_format,
     ) -> List[HelpPanel]:
+        from rich.console import Group as RichGroup
+        from rich.console import NewLine
+
         _, apps, _ = self.parse_commands(tokens)
 
+        help_format = resolve_help_format(apps)
+
         panels: Dict[str, Tuple[Group, HelpPanel]] = {}
         # Handle commands first; there's an off chance they may be "upgraded"
         # to an argument/parameter panel.
         for subapp in walk_metas(apps[-1]):
             # Handle Commands
             for group, elements in groups_from_app(subapp):
                 if not group.show:
@@ -850,20 +881,24 @@
                     command_panel = HelpPanel(
                         format="command",
                         title=group.name,
                     )
                     panels[group.name] = (group, command_panel)
 
                 if group.help:
+                    import cyclopts.help
+
+                    group_help = cyclopts.help._format(group.help, format=help_format)
+
                     if command_panel.description:
-                        command_panel.description += "\n" + group.help
+                        command_panel.description = RichGroup(command_panel.description, NewLine(), group_help)
                     else:
-                        command_panel.description = group.help
+                        command_panel.description = group_help
 
-                command_panel.entries.extend(format_command_entries(elements))
+                command_panel.entries.extend(format_command_entries(elements, format=help_format))
 
         # Handle Arguments/Parameters
         for subapp in walk_metas(apps[-1]):
             if not subapp.default_command:
                 continue
             command = ResolvedCommand(
                 subapp.default_command,
@@ -875,23 +910,25 @@
                 if not group.show:
                     continue
                 cparams = [command.iparam_to_cparam[x] for x in iparams]
                 try:
                     _, existing_panel = panels[group.name]
                 except KeyError:
                     existing_panel = None
-                new_panel = create_parameter_help_panel(group, iparams, cparams)
+                new_panel = create_parameter_help_panel(group, iparams, cparams, help_format)
 
                 if existing_panel:
                     # An imperfect merging process
                     existing_panel.format = "parameter"
                     existing_panel.entries = new_panel.entries + existing_panel.entries  # Commands go last
                     if new_panel.description:
                         if existing_panel.description:
-                            existing_panel.description += "\n" + new_panel.description
+                            existing_panel.description = RichGroup(
+                                existing_panel.description, NewLine(), new_panel.description
+                            )
                         else:
                             existing_panel.description = new_panel.description
                 else:
                     panels[group.name] = (group, new_panel)
 
         groups = [x[0] for x in panels.values()]
         help_panels = [x[1] for x in panels.values()]
@@ -974,15 +1011,15 @@
                 pass
             except Exception:
                 print(traceback.format_exc())
 
     def __repr__(self):
         """Only shows non-default values."""
         non_defaults = {}
-        for a in self.__attrs_attrs__:  # pyright: ignore[reportGeneralTypeIssues]
+        for a in self.__attrs_attrs__:  # pyright: ignore[reportAttributeAccessIssue]
             if not a.init:
                 continue
             v = getattr(self, a.name)
             # Compare types first because of some weird attribute issues.
             if type(v) != type(a.default) or v != a.default:  # noqa: E721
                 non_defaults[a.alias] = v
```

### Comparing `cyclopts-2.6.1/cyclopts/exceptions.py` & `cyclopts-2.6.2/cyclopts/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,26 +194,26 @@
     def __str__(self):
         if self.parameter:
             assert self.parameter2cli is not None
             parameter_cli_name = ",".join(self.parameter2cli[self.parameter])
 
         if self.msg is not None:
             if self.parameter:
-                return f"{parameter_cli_name}: " + self.msg  # pyright: ignore[reportUnboundVariable]
+                return f"{parameter_cli_name}: " + self.msg  # pyright: ignore[reportPossiblyUnboundVariable]
             else:
                 return self.msg
 
         response = f'Error converting value "{self.input_value}"'
 
         if self.target_type is not None:
             target_type = str(self.target_type).lstrip("typing.")  # lessens the verbosity a little bit.
             response += f" to {target_type}"
 
         if self.parameter:
-            response += f' for "{parameter_cli_name}"'  # pyright: ignore[reportUnboundVariable]
+            response += f' for "{parameter_cli_name}"'  # pyright: ignore[reportPossiblyUnboundVariable]
 
         return super().__str__() + response + "."
 
 
 class InvalidCommandError(CycloptsError):
     """CLI token combination did not yield a valid command."""
```

### Comparing `cyclopts-2.6.1/cyclopts/group.py` & `cyclopts-2.6.2/cyclopts/group.py`

 * *Files identical despite different names*

### Comparing `cyclopts-2.6.1/cyclopts/group_extractors.py` & `cyclopts-2.6.2/cyclopts/group_extractors.py`

 * *Files identical despite different names*

### Comparing `cyclopts-2.6.1/cyclopts/help.py` & `cyclopts-2.6.2/cyclopts/help.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,34 @@
 import inspect
 from enum import Enum
 from functools import lru_cache, partial
 from inspect import isclass
-from typing import TYPE_CHECKING, Callable, List, Literal, Tuple, Type, Union, get_args, get_origin
+from typing import (
+    TYPE_CHECKING,
+    Callable,
+    Iterable,
+    List,
+    Literal,
+    Tuple,
+    Type,
+    Union,
+    get_args,
+    get_origin,
+)
 
 import docstring_parser
 from attrs import define, field, frozen
 
 import cyclopts.utils
 from cyclopts.group import Group
 from cyclopts.parameter import Parameter, get_hint_parameter
 
 if TYPE_CHECKING:
+    from rich.console import RenderableType
+
     from cyclopts.core import App
 
 
 @lru_cache(maxsize=16)
 def docstring_parse(doc: str):
     """Addon to :func:`docstring_parser.parse` that double checks the `short_description`."""
     res = docstring_parser.parse(doc)
@@ -29,53 +42,69 @@
         res.short_description = None
     return res
 
 
 @frozen
 class HelpEntry:
     name: str
-    short: str = ""
-    description: str = ""
+    short: str
+    description: "RenderableType"
     required: bool = False
 
 
+def _text_factory():
+    from rich.text import Text
+
+    return Text()
+
+
 @define
 class HelpPanel:
     format: Literal["command", "parameter"]
     title: str
-    description: str = ""
+    description: "RenderableType" = field(factory=_text_factory)
     entries: List[HelpEntry] = field(factory=list)
 
     def remove_duplicates(self):
         seen, out = set(), []
         for item in self.entries:
-            if item not in seen:
-                seen.add(item)
+            hashable = (item.name, item.short)
+            if hashable not in seen:
+                seen.add(hashable)
                 out.append(item)
         self.entries = out
 
     def sort(self):
         self.entries.sort(key=lambda x: (x.name.startswith("-"), x.name))
 
     def __rich__(self):
         if not self.entries:
             return _silent
         from rich.box import ROUNDED
         from rich.console import Group as RichGroup
+        from rich.console import NewLine
+        from rich.panel import Panel
         from rich.table import Table
         from rich.text import Text
 
         table = Table.grid(padding=(0, 1))
-        text = Text(end="")
-        if self.description:
-            text.append(self.description + "\n\n")
-        from rich.panel import Panel
+        panel_description = self.description
+
+        if isinstance(panel_description, Text):
+            panel_description.end = ""
+
+            if panel_description.plain:
+                panel_description = RichGroup(panel_description, NewLine(2))
+        else:
+            # Should be either a RST or Markdown object
+            if panel_description.markup:  # pyright: ignore[reportAttributeAccessIssue]
+                panel_description = RichGroup(panel_description, NewLine(1))
 
         panel = Panel(
-            RichGroup(text, table),
+            RichGroup(panel_description, table),
             box=ROUNDED,
             expand=True,
             title_align="left",
             title=self.title,
         )
 
         if self.format == "command":
@@ -159,45 +188,83 @@
         usage.extend(sorted(to_show))
 
     return Text(" ".join(usage) + "\n", style="bold")
 
 
 def format_doc(root_app, app: "App", format: str = "restructuredtext"):
     from rich.console import Group as RichGroup
+    from rich.console import NewLine
     from rich.text import Text
 
-    from cyclopts.core import App  # noqa: F811
-
     raw_doc_string = app.help
 
     if not raw_doc_string:
         return _silent
 
     parsed = docstring_parse(raw_doc_string)
 
-    components: List[Tuple[str, str]] = []
+    components: List[Union[str, Tuple[str, str]]] = []
     if parsed.short_description:
-        components.append((parsed.short_description + "\n", "default"))
+        components.append(parsed.short_description + "\n")
 
     if parsed.long_description:
         if parsed.short_description:
-            components.append(("\n", "default"))
+            components.append("\n")
         components.append((parsed.long_description + "\n", "info"))
 
+    return RichGroup(_format(*components, format=format), NewLine())
+
+
+def _format(*components: Union[str, Tuple[str, str]], format: str = "restructuredtext") -> "RenderableType":
     format = format.lower()
+
     if format == "plaintext":
-        return Text.assemble(*components)
+        from rich.text import Text
+
+        aggregate = []
+        for component in components:
+            if isinstance(component, str):
+                aggregate.append(component)
+            else:
+                aggregate.append(component[0])
+        return Text.assemble("".join(aggregate).rstrip())
     elif format in ("markdown", "md"):
         from rich.markdown import Markdown
 
-        return RichGroup(Markdown("".join(x[0] for x in components)), Text(""))
+        aggregate = []
+        for component in components:
+            if isinstance(component, str):
+                aggregate.append(component)
+            else:
+                # Ignore style for now :(
+                aggregate.append(component[0])
+
+        return Markdown("".join(aggregate))
     elif format in ("restructuredtext", "rst"):
         from rich_rst import RestructuredText
 
-        return RestructuredText("".join(x[0] for x in components))
+        aggregate = []
+        for component in components:
+            if isinstance(component, str):
+                aggregate.append(component)
+            else:
+                # Ignore style for now :(
+                aggregate.append(component[0])
+        return RestructuredText("".join(aggregate))
+    elif format == "rich":
+        from rich.text import Text
+
+        def walk_components():
+            for component in components:
+                if isinstance(component, str):
+                    yield Text.from_markup(component.rstrip())
+                else:
+                    yield Text.from_markup(component[0].rstrip(), style=component[1])
+
+        return Text().join(walk_components())
     else:
         raise ValueError(f'Unknown help_format "{format}"')
 
 
 def _get_choices(type_: Type, name_transform: Callable[[str], str]) -> str:
     get_choices = partial(_get_choices, name_transform=name_transform)
     choices: str = ""
@@ -212,23 +279,36 @@
     elif _origin in (list, set, tuple):
         args = get_args(type_)
         if len(args) == 1 or (_origin is tuple and len(args) == 2 and args[1] is Ellipsis):
             choices = get_choices(args[0])
     return choices
 
 
-def create_parameter_help_panel(group: "Group", iparams, cparams: List[Parameter]) -> HelpPanel:
-    help_panel = HelpPanel(format="parameter", title=group.name, description=group.help)
+def create_parameter_help_panel(
+    group: "Group",
+    iparams,
+    cparams: List[Parameter],
+    format: str,
+) -> HelpPanel:
+    help_panel = HelpPanel(format="parameter", title=group.name, description=_format(group.help, format=format))
     icparams = [(ip, cp) for ip, cp in zip(iparams, cparams) if cp.show]
 
     if not icparams:
         return help_panel
 
     iparams, cparams = (list(x) for x in zip(*icparams))
 
+    def help_append(text, style=""):
+        if help_components:
+            text = " " + text
+        if style:
+            help_components.append((text, style))
+        else:
+            help_components.append(text)
+
     for iparam, cparam in icparams:
         assert cparam.name is not None
         assert cparam.name_transform is not None
         type_ = get_hint_parameter(iparam)[0]
         options = list(cparam.name)
         options.extend(cparam.get_negatives(type_, *options))
 
@@ -244,59 +324,68 @@
                 short_options.append(option)
             else:
                 long_options.append(option)
 
         help_components = []
 
         if cparam.help:
-            help_components.append(cparam.help)
+            help_append(cparam.help)
 
         if cparam.show_choices:
             choices = _get_choices(type_, cparam.name_transform)
             if choices:
-                help_components.append(rf"[dim]\[choices: {choices}][/dim]")
+                help_append(rf"[choices: {choices}]", "dim")
 
         if cparam.show_env_var and cparam.env_var:
             env_vars = " ".join(cparam.env_var)
-            help_components.append(rf"[dim]\[env var: {env_vars}][/dim]")
+            help_append(rf"[env var: {env_vars}]", "dim")
 
         if cparam.show_default or (
             cparam.show_default is None and iparam.default not in {None, inspect.Parameter.empty}
         ):
             default = ""
             if isclass(type_) and issubclass(type_, Enum):
                 default = cparam.name_transform(iparam.default.name)
             else:
                 default = iparam.default
 
-            help_components.append(rf"[dim]\[default: {default}][/dim]")
+            help_append(rf"[default: {default}]", "dim")
 
         if cparam.required:
-            help_components.append(r"[red][dim]\[required][/dim][/red]")
+            help_append(r"[required]", "dim red")
 
         # populate row
         help_panel.entries.append(
             HelpEntry(
                 name=",".join(long_options),
-                description=" ".join(help_components),
+                description=_format(*help_components, format=format),
                 short=",".join(short_options),
                 required=bool(cparam.required),
             )
         )
 
     return help_panel
 
 
-def format_command_entries(elements) -> List:
+def format_command_entries(apps: Iterable["App"], format: str) -> List:
     entries = []
-    for element in elements:
+    for app in apps:
         short_names, long_names = [], []
-        for name in element.name:
+        for name in app.name:
             short_names.append(name) if _is_short(name) else long_names.append(name)
         entry = HelpEntry(
             name=",".join(long_names),
             short=",".join(short_names),
-            description=docstring_parse(element.help).short_description or "",
+            description=_format(docstring_parse(app.help).short_description or "", format=format),
         )
         if entry not in entries:
             entries.append(entry)
     return entries
+
+
+def resolve_help_format(app_chain: Iterable["App"]) -> str:
+    # Resolve help_format; None fallsback to parent; non-None overwrites parent.
+    help_format = "restructuredtext"
+    for app in app_chain:
+        if app.help_format is not None:
+            help_format = app.help_format
+    return help_format
```

### Comparing `cyclopts-2.6.1/cyclopts/parameter.py` & `cyclopts-2.6.2/cyclopts/parameter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,40 @@
 import inspect
 from functools import partial
-from typing import Any, Callable, Iterable, Optional, Tuple, Type, Union, cast, get_args, get_origin
+from typing import (
+    Any,
+    Callable,
+    Iterable,
+    Optional,
+    Tuple,
+    Type,
+    Union,
+    cast,
+    get_args,
+    get_origin,
+)
 
 import attrs
 from attrs import field, frozen
 
 import cyclopts.utils
 from cyclopts._convert import (
     AnnotatedType,
     convert,
     get_origin_and_validate,
     resolve,
     resolve_optional,
 )
 from cyclopts.group import Group
-from cyclopts.utils import default_name_transform, optional_to_tuple_converter, record_init, to_tuple_converter
+from cyclopts.utils import (
+    default_name_transform,
+    optional_to_tuple_converter,
+    record_init,
+    to_tuple_converter,
+)
 
 
 def _double_hyphen_validator(instance, attribute, values):
     if not values:
         return
 
     for value in values:
@@ -141,15 +157,15 @@
         return tuple(out)
 
     def __repr__(self):
         """Only shows non-default values."""
         content = ", ".join(
             [
                 f"{a.alias}={getattr(self, a.name)!r}"
-                for a in self.__attrs_attrs__  # pyright: ignore[reportGeneralTypeIssues]
+                for a in self.__attrs_attrs__  # pyright: ignore[reportAttributeAccessIssue]
                 if a.alias in self._provided_args
             ]
         )
         return f"{type(self).__name__}({content})"
 
     @classmethod
     def combine(cls, *parameters: Optional["Parameter"]) -> "Parameter":
@@ -161,29 +177,29 @@
              Parameters who's attributes override ``self`` attributes.
              Ordered from least-to-highest attribute priority.
         """
         kwargs = {}
         for parameter in parameters:
             if parameter is None:
                 continue
-            for a in parameter.__attrs_attrs__:  # pyright: ignore[reportGeneralTypeIssues]
+            for a in parameter.__attrs_attrs__:  # pyright: ignore[reportAttributeAccessIssue]
                 if a.init and a.alias in parameter._provided_args:
                     kwargs[a.alias] = getattr(parameter, a.name)
 
         return cls(**kwargs)
 
     @classmethod
     def default(cls) -> "Parameter":
         """Create a Parameter with all Cyclopts-default values.
 
         This is different than just :class:`Parameter` because the default
         values will be recorded and override all upstream parameter values.
         """
         return cls(
-            **{a.alias: a.default for a in cls.__attrs_attrs__ if a.init}  # pyright: ignore[reportGeneralTypeIssues]
+            **{a.alias: a.default for a in cls.__attrs_attrs__ if a.init}  # pyright: ignore[reportAttributeAccessIssue]
         )
 
 
 def validate_command(f: Callable):
     """Validate if a function abides by Cyclopts's rules.
 
     Raises
@@ -195,17 +211,15 @@
     for iparam in signature.parameters.values():
         get_origin_and_validate(iparam.annotation)
         type_, cparam = get_hint_parameter(iparam)
         if not cparam.parse and iparam.kind is not iparam.KEYWORD_ONLY:
             raise ValueError("Parameter.parse=False must be used with a KEYWORD_ONLY function parameter.")
 
 
-def get_hint_parameter(
-    type_: Union[Type, inspect.Parameter], *default_parameters: Optional[Parameter]
-) -> Tuple[Type, Parameter]:
+def get_hint_parameter(type_: Any, *default_parameters: Optional[Parameter]) -> Tuple[Type, Parameter]:
     """Get the type hint and Cyclopts :class:`Parameter` from a type-hint.
 
     If a ``cyclopts.Parameter`` is not found, a default Parameter is returned.
     """
     cyclopts_parameters = []
 
     if isinstance(type_, inspect.Parameter):
```

### Comparing `cyclopts-2.6.1/cyclopts/resolve.py` & `cyclopts-2.6.2/cyclopts/resolve.py`

 * *Files identical despite different names*

### Comparing `cyclopts-2.6.1/cyclopts/types.py` & `cyclopts-2.6.2/cyclopts/types.py`

 * *Files identical despite different names*

### Comparing `cyclopts-2.6.1/cyclopts/utils.py` & `cyclopts-2.6.2/cyclopts/utils.py`

 * *Files identical despite different names*

### Comparing `cyclopts-2.6.1/cyclopts/validators/_group.py` & `cyclopts-2.6.2/cyclopts/validators/_group.py`

 * *Files identical despite different names*

### Comparing `cyclopts-2.6.1/cyclopts/validators/_number.py` & `cyclopts-2.6.2/cyclopts/validators/_number.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional, Type, Union, get_args, get_origin
 
 from attrs import frozen
 
-Numeric = Union[int, float, complex]
+Numeric = Union[int, float]
 
 
 @frozen(kw_only=True)
 class Number:
     """Limit input number to a value range."""
 
     lt: Optional[Numeric] = None
@@ -24,18 +24,18 @@
     def __call__(self, type_: Type, value: Numeric):
         origin = get_origin(type_) or type_
         if origin not in get_args(Numeric):
             raise TypeError
         if not isinstance(value, get_args(Numeric)):
             raise TypeError
 
-        if self.lt is not None and value >= self.lt:  # pyright: ignore[reportGeneralTypeIssues]
+        if self.lt is not None and value >= self.lt:
             raise ValueError(f"Must be < {self.lt}")
 
-        if self.lte is not None and value > self.lte:  # pyright: ignore[reportGeneralTypeIssues]
+        if self.lte is not None and value > self.lte:
             raise ValueError(f"Must be <= {self.lte}")
 
-        if self.gt is not None and value <= self.gt:  # pyright: ignore[reportGeneralTypeIssues]
+        if self.gt is not None and value <= self.gt:
             raise ValueError(f"Must be > {self.gt}")
 
-        if self.gte is not None and value < self.gte:  # pyright: ignore[reportGeneralTypeIssues]
+        if self.gte is not None and value < self.gte:
             raise ValueError(f"Must be >= {self.gte}")
```

### Comparing `cyclopts-2.6.1/cyclopts/validators/_path.py` & `cyclopts-2.6.2/cyclopts/validators/_path.py`

 * *Files identical despite different names*

### Comparing `cyclopts-2.6.1/pyproject.toml` & `cyclopts-2.6.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "semver"
 
 [tool.poetry]
 name = "cyclopts"
-version = "2.6.1"  # Do not change, let poetry-dynamic-versioning handle it.
+version = "2.6.2"  # Do not change, let poetry-dynamic-versioning handle it.
 homepage = "https://github.com/BrianPugh/cyclopts"
 repository = "https://github.com/BrianPugh/cyclopts"
 license = "Apache-2.0"
 description = ""
 authors = ["Brian Pugh"]
 readme = "README.md"
 packages = [{include = "cyclopts"}]
@@ -28,22 +28,22 @@
 # Be as loose as possible if writing a library.
 python = "^3.8"
 typing-extensions = { version = ">=4.8.0", python = "^3.8.0" }
 importlib-metadata = { version = ">=4.4", python = '<3.10' }
 attrs = ">=23.1.0"
 rich = ">=13.6.0"
 docstring-parser = "^0.15"
-rich-rst = "^1.2.0"
+rich-rst = "^1.3.1"
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "~7.1.2"
 sphinx_rtd_theme = ">=1.3,<2.1"
 gitpython = ">=3.1.31"
 sphinx-copybutton = "^0.5"
-myst-parser = {extras = ["linkify"], version = "^2.0.0"}
+myst-parser = {extras = ["linkify"], version = "^3.0.1"}
 sphinx-autodoc-typehints = ">=1.25.2,<3.0.0"
 
 [tool.poetry.group.dev.dependencies]
 coverage = {extras = ["toml"], version = ">=5.1"}
 pre_commit = ">=2.16.0"
 pytest = ">=7.1.2"
 pytest-cov = ">=3.0.0"
@@ -101,14 +101,27 @@
 [tool.pyright]
 venvPath = "."
 venv = ".venv"
 ignore = ["docs/", ]
 
 [tool.ruff]
 target-version = 'py38'
+line-length = 120  # Must agree with Black
+exclude = [
+    "migrations",
+    "__pycache__",
+    "manage.py",
+    "settings.py",
+    "env",
+    ".env",
+    "venv",
+    ".venv",
+]
+
+[tool.ruff.lint]
 select = [
     "B",  # flake8-bugbear
     "C4", # flake8-comprehensions
     "D",  # pydocstyle
     "E",  # Error
     "F",  # pyflakes
     "I",  # isort
@@ -119,25 +132,14 @@
     "Q",  # flake8-quotes
     "TRY",  # tryceratops
     "UP",  # pyupgrade
     "W",  # Warning
     "YTT", # flake8-2020
 ]
 
-exclude = [
-    "migrations",
-    "__pycache__",
-    "manage.py",
-    "settings.py",
-    "env",
-    ".env",
-    "venv",
-    ".venv",
-]
-
 ignore = [
     "B905",  # zip strict=True; remove once python <3.10 support is dropped.
     "D100",
     "D101",
     "D102",
     "D103",
     "D104",
@@ -149,46 +151,46 @@
     "E402",
     "E501",
     "F401",
     "PGH003",  # Use specific rule codes when ignoring type issues
     "TRY003",  # Avoid specifying messages outside exception class; overly strict, especially for ValueError
     "TRY300",  # Consider moving this statement to an `else` block
 ]
-line-length = 120  # Must agree with Black
 
-[tool.ruff.flake8-bugbear]
+[tool.ruff.lint.flake8-bugbear]
 extend-immutable-calls = [
     "chr",
     "typer.Argument",
     "typer.Option",
 ]
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "numpy"
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "tests/*.py" = [
     "D100",
     "D101",
     "D102",
     "D103",
     "D104",
     "D105",
     "D106",
     "D107",
     "D205",
+    "D404",
     "S102",  # use of "exec"
     "S106",  # possible hardcoded password.
     "PGH001",  # use of "eval"
 ]
 "docs/*.py" = [
     "F811",  # redefinition
 ]
 
-[tool.ruff.pep8-naming]
+[tool.ruff.lint.pep8-naming]
 staticmethod-decorators = [
     "pydantic.validator",
     "pydantic.root_validator",
 ]
 
 [tool.codespell]
 skip = 'poetry.lock,'
```

### Comparing `cyclopts-2.6.1/PKG-INFO` & `cyclopts-2.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyclopts
-Version: 2.6.1
+Version: 2.6.2
 Summary: 
 Home-page: https://github.com/BrianPugh/cyclopts
 License: Apache-2.0
 Author: Brian Pugh
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: attrs (>=23.1.0)
 Requires-Dist: docstring-parser (>=0.15,<0.16)
 Requires-Dist: importlib-metadata (>=4.4) ; python_version < "3.10"
 Requires-Dist: rich (>=13.6.0)
-Requires-Dist: rich-rst (>=1.2.0,<2.0.0)
+Requires-Dist: rich-rst (>=1.3.1,<2.0.0)
 Requires-Dist: typing-extensions (>=4.8.0) ; python_full_version >= "3.8.0" and python_full_version < "4.0.0"
 Project-URL: Repository, https://github.com/BrianPugh/cyclopts
 Description-Content-Type: text/markdown
 
 <div align="center">
   <img src="https://raw.githubusercontent.com/BrianPugh/Cyclopts/main/assets/logo_512w.png">
 </div>
```

