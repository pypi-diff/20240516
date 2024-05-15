# Comparing `tmp/pipefunc-0.5.0.tar.gz` & `tmp/pipefunc-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipefunc-0.5.0.tar", last modified: Tue Apr 30 22:04:13 2024, max compression
+gzip compressed data, was "pipefunc-0.6.0.tar", last modified: Wed May 15 05:46:33 2024, max compression
```

## Comparing `pipefunc-0.5.0.tar` & `pipefunc-0.6.0.tar`

### file list

```diff
@@ -1,33 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:13.094823 pipefunc-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-30 22:04:07.000000 pipefunc-0.5.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-30 22:04:07.000000 pipefunc-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-30 22:04:07.000000 pipefunc-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9371 2024-04-30 22:04:13.094823 pipefunc-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7074 2024-04-30 22:04:07.000000 pipefunc-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:13.098823 pipefunc-0.5.0/pipefunc/
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-30 22:04:07.000000 pipefunc-0.5.0/pipefunc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15439 2024-04-30 22:04:07.000000 pipefunc-0.5.0/pipefunc/_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-30 22:04:07.000000 pipefunc-0.5.0/pipefunc/_lazy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-04-30 22:04:07.000000 pipefunc-0.5.0/pipefunc/_perf.py
--rw-r--r--   0 runner    (1001) docker     (127)    11190 2024-04-30 22:04:07.000000 pipefunc-0.5.0/pipefunc/_pipefunc.py
--rw-r--r--   0 runner    (1001) docker     (127)    45131 2024-04-30 22:04:07.000000 pipefunc-0.5.0/pipefunc/_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-04-30 22:04:07.000000 pipefunc-0.5.0/pipefunc/_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-04-30 22:04:07.000000 pipefunc-0.5.0/pipefunc/_simplify.py
--rw-r--r--   0 runner    (1001) docker     (127)    24844 2024-04-30 22:04:07.000000 pipefunc-0.5.0/pipefunc/_sweep.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-30 22:04:07.000000 pipefunc-0.5.0/pipefunc/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-30 22:04:13.098823 pipefunc-0.5.0/pipefunc/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:13.094823 pipefunc-0.5.0/pipefunc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9371 2024-04-30 22:04:13.000000 pipefunc-0.5.0/pipefunc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-30 22:04:13.000000 pipefunc-0.5.0/pipefunc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 22:04:13.000000 pipefunc-0.5.0/pipefunc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-30 22:04:13.000000 pipefunc-0.5.0/pipefunc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 22:04:13.000000 pipefunc-0.5.0/pipefunc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-04-30 22:04:07.000000 pipefunc-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-30 22:04:13.098823 pipefunc-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:13.094823 pipefunc-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11272 2024-04-30 22:04:07.000000 pipefunc-0.5.0/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-30 22:04:07.000000 pipefunc-0.5.0/tests/test_dag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-30 22:04:07.000000 pipefunc-0.5.0/tests/test_perf.py
--rw-r--r--   0 runner    (1001) docker     (127)    15337 2024-04-30 22:04:07.000000 pipefunc-0.5.0/tests/test_pipefunc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6013 2024-04-30 22:04:07.000000 pipefunc-0.5.0/tests/test_simplify.py
--rw-r--r--   0 runner    (1001) docker     (127)    12579 2024-04-30 22:04:07.000000 pipefunc-0.5.0/tests/test_sweep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:46:33.552420 pipefunc-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-15 05:46:27.000000 pipefunc-0.6.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-15 05:46:27.000000 pipefunc-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-15 05:46:27.000000 pipefunc-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9549 2024-05-15 05:46:33.552420 pipefunc-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7072 2024-05-15 05:46:27.000000 pipefunc-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:46:33.552420 pipefunc-0.6.0/pipefunc/
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-15 05:46:27.000000 pipefunc-0.6.0/pipefunc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16472 2024-05-15 05:46:27.000000 pipefunc-0.6.0/pipefunc/_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-05-15 05:46:27.000000 pipefunc-0.6.0/pipefunc/_lazy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-05-15 05:46:27.000000 pipefunc-0.6.0/pipefunc/_perf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13061 2024-05-15 05:46:27.000000 pipefunc-0.6.0/pipefunc/_pipefunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46348 2024-05-15 05:46:27.000000 pipefunc-0.6.0/pipefunc/_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-05-15 05:46:27.000000 pipefunc-0.6.0/pipefunc/_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5862 2024-05-15 05:46:27.000000 pipefunc-0.6.0/pipefunc/_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24740 2024-05-15 05:46:27.000000 pipefunc-0.6.0/pipefunc/_sweep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-05-15 05:46:27.000000 pipefunc-0.6.0/pipefunc/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-15 05:46:33.552420 pipefunc-0.6.0/pipefunc/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-15 05:46:27.000000 pipefunc-0.6.0/pipefunc/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:46:33.548421 pipefunc-0.6.0/pipefunc/map/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-15 05:46:27.000000 pipefunc-0.6.0/pipefunc/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-05-15 05:46:27.000000 pipefunc-0.6.0/pipefunc/map/_adaptive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6635 2024-05-15 05:46:27.000000 pipefunc-0.6.0/pipefunc/map/_filearray.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11481 2024-05-15 05:46:27.000000 pipefunc-0.6.0/pipefunc/map/_mapspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11839 2024-05-15 05:46:27.000000 pipefunc-0.6.0/pipefunc/map/_run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:46:33.548421 pipefunc-0.6.0/pipefunc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9549 2024-05-15 05:46:33.000000 pipefunc-0.6.0/pipefunc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-15 05:46:33.000000 pipefunc-0.6.0/pipefunc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 05:46:33.000000 pipefunc-0.6.0/pipefunc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-15 05:46:33.000000 pipefunc-0.6.0/pipefunc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 05:46:33.000000 pipefunc-0.6.0/pipefunc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-15 05:46:27.000000 pipefunc-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-15 05:46:33.552420 pipefunc-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:46:33.548421 pipefunc-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11506 2024-05-15 05:46:27.000000 pipefunc-0.6.0/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-05-15 05:46:27.000000 pipefunc-0.6.0/tests/test_dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-15 05:46:27.000000 pipefunc-0.6.0/tests/test_perf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17590 2024-05-15 05:46:27.000000 pipefunc-0.6.0/tests/test_pipefunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-05-15 05:46:27.000000 pipefunc-0.6.0/tests/test_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12579 2024-05-15 05:46:27.000000 pipefunc-0.6.0/tests/test_sweep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-15 05:46:27.000000 pipefunc-0.6.0/tests/test_utils.py
```

### Comparing `pipefunc-0.5.0/LICENSE` & `pipefunc-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pipefunc-0.5.0/PKG-INFO` & `pipefunc-0.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipefunc
-Version: 0.5.0
+Version: 0.6.0
 Summary: A Python library for defining, managing, and executing function pipelines.
 Maintainer-email: Bas Nijholt <bas@nijho.lt>
 License: MIT
 Project-URL: homepage, https://pipefunc.readthedocs.io/
 Project-URL: documentation, https://pipefunc.readthedocs.io/
 Project-URL: repository, https://github.com/basnijholt/pipefunc
 Classifier: Development Status :: 4 - Beta
@@ -26,33 +26,38 @@
 License-File: LICENSE
 License-File: AUTHORS.md
 Requires-Dist: networkx
 Requires-Dist: psutil
 Requires-Dist: versioningit
 Requires-Dist: typing_extensions; python_version <= "3.9"
 Requires-Dist: cloudpickle
+Requires-Dist: numpy
+Provides-Extra: adaptive
+Requires-Dist: adaptive; extra == "adaptive"
+Requires-Dist: adaptive-scheduler; extra == "adaptive"
 Provides-Extra: plotting
 Requires-Dist: matplotlib; extra == "plotting"
 Requires-Dist: pygraphviz; extra == "plotting"
 Requires-Dist: holoviews; extra == "plotting"
 Requires-Dist: bokeh; extra == "plotting"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pandas; extra == "test"
+Requires-Dist: adaptive; extra == "test"
 Provides-Extra: docs
 Requires-Dist: myst-nb; extra == "docs"
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
 Requires-Dist: emoji; extra == "docs"
 Requires-Dist: jupytext; extra == "docs"
 Requires-Dist: jupyterlite-sphinx; extra == "docs"
-Requires-Dist: jupyterlite-xeus-python; extra == "docs"
+Requires-Dist: jupyterlite-xeus; extra == "docs"
 Requires-Dist: pandas; extra == "docs"
 Provides-Extra: dev
 Requires-Dist: black[jupyter]; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 
@@ -145,15 +150,15 @@
 assert h_e(a=2, b=3, x=1) == 75
 assert h_e(c=5, d=15, x=1) == 75
 
 # Visualize the pipeline
 pipeline.visualize()
 
 # Get all possible argument mappings for each function
-all_args = pipeline.all_arg_combinations()
+all_args = pipeline.all_arg_combinations
 print(all_args)
 
 # Show resource reporting (only works if profile=True)
 pipeline.resources_report()
 ```
 
 This example demonstrates defining a pipeline with `f_c`, `f_d`, `f_e` functions, accessing and executing these functions using the pipeline, visualizing the pipeline graph, getting all possible argument mappings, and reporting on the resource usage.
```

### Comparing `pipefunc-0.5.0/README.md` & `pipefunc-0.6.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 assert h_e(a=2, b=3, x=1) == 75
 assert h_e(c=5, d=15, x=1) == 75
 
 # Visualize the pipeline
 pipeline.visualize()
 
 # Get all possible argument mappings for each function
-all_args = pipeline.all_arg_combinations()
+all_args = pipeline.all_arg_combinations
 print(all_args)
 
 # Show resource reporting (only works if profile=True)
 pipeline.resources_report()
 ```
 
 This example demonstrates defining a pipeline with `f_c`, `f_d`, `f_e` functions, accessing and executing these functions using the pipeline, visualizing the pipeline graph, getting all possible argument mappings, and reporting on the resource usage.
```

### Comparing `pipefunc-0.5.0/pipefunc/__init__.py` & `pipefunc-0.6.0/pipefunc/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 """PipeFunc: A Python library for defining, managing, and executing function pipelines."""
 
 from pipefunc._lazy import construct_dag, evaluate_lazy
-from pipefunc._pipefunc import (
-    PipelineFunction,
-    pipefunc,
-)
+from pipefunc._pipefunc import PipeFunc, pipefunc
 from pipefunc._pipeline import Pipeline
 from pipefunc._sweep import (
     MultiSweep,
     Sweep,
     count_sweep,
     generate_sweep,
     get_precalculation_order,
@@ -22,11 +19,11 @@
     "count_sweep",
     "evaluate_lazy",
     "generate_sweep",
     "get_precalculation_order",
     "MultiSweep",
     "pipefunc",
     "Pipeline",
-    "PipelineFunction",
+    "PipeFunc",
     "set_cache_for_sweep",
     "Sweep",
 ]
```

### Comparing `pipefunc-0.5.0/pipefunc/_cache.py` & `pipefunc-0.6.0/pipefunc/_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -283,15 +283,15 @@
             self._cache_queue = manager.list()
             self._cache_lock = manager.Lock()
         else:
             self._cache_dict = {}  # type: ignore[assignment]
             self._cache_queue = []  # type: ignore[assignment]
             self._cache_lock = nullcontext()  # type: ignore[assignment]
 
-    def get(self, key: Hashable) -> tuple[bool, Any]:
+    def get(self, key: Hashable) -> Any:
         """Get a value from the cache by key."""
         with self._cache_lock:
             value = self._cache_dict.get(key)
             if value is not None:  # Move key to back of queue
                 self._cache_queue.remove(key)
                 self._cache_queue.append(key)
         if value is not None:
@@ -339,14 +339,49 @@
         with self._cache_lock:
             keys = list(self._cache_dict.keys())
             for key in keys:
                 del self._cache_dict[key]
             del self._cache_queue[:]
 
 
+class SimpleCache(_CacheBase):
+    """A simple cache without any eviction strategy."""
+
+    def __init__(self) -> None:
+        """Initialize the cache."""
+        self._cache_dict: dict[Hashable, Any] = {}
+
+    def get(self, key: Hashable) -> Any:
+        """Get a value from the cache by key."""
+        return self._cache_dict.get(key)
+
+    def put(self, key: Hashable, value: Any) -> None:
+        """Insert a key value pair into the cache."""
+        self._cache_dict[key] = value
+
+    def __contains__(self, key: Hashable) -> bool:
+        """Check if a key is present in the cache."""
+        return key in self._cache_dict
+
+    @property
+    def cache(self) -> dict:
+        """Returns a copy of the cache."""
+        return self._cache_dict
+
+    def __len__(self) -> int:
+        """Return the number of entries in the cache."""
+        return len(self._cache_dict)
+
+    def clear(self) -> None:
+        """Clear the cache."""
+        keys = list(self._cache_dict.keys())
+        for key in keys:
+            del self._cache_dict[key]
+
+
 class DiskCache(_CacheBase):
     """Disk cache implementation using pickle or cloudpickle for serialization.
 
     Parameters
     ----------
     cache_dir
         The directory where the cache files are stored.
```

### Comparing `pipefunc-0.5.0/pipefunc/_perf.py` & `pipefunc-0.6.0/pipefunc/_perf.py`

 * *Files identical despite different names*

### Comparing `pipefunc-0.5.0/pipefunc/_pipefunc.py` & `pipefunc-0.6.0/pipefunc/_pipefunc.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,40 +13,36 @@
 from __future__ import annotations
 
 import contextlib
 import functools
 import inspect
 import os
 import sys
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Generic,
-    Tuple,
-    TypeVar,
-    Union,
-)
+from typing import TYPE_CHECKING, Any, Generic, Tuple, TypeVar, Union
 
 import cloudpickle
 
 from pipefunc._lazy import evaluate_lazy
 from pipefunc._perf import ProfilingStats, ResourceProfiler
 from pipefunc._utils import at_least_tuple
 
 if sys.version_info < (3, 9):  # pragma: no cover
     from typing import Callable
 else:
     from collections.abc import Callable
 
+from pipefunc.map._mapspec import MapSpec
+
 if TYPE_CHECKING:
     from pathlib import Path
 
 
 T = TypeVar("T", bound=Callable[..., Any])
 _OUTPUT_TYPE = Union[str, Tuple[str, ...]]
+MAX_PARAMS_LEN = 15
 
 
 def _default_output_picker(
     output: Any,
     name: str,
     output_name: _OUTPUT_TYPE,
 ) -> Any:
@@ -56,15 +52,15 @@
 
 def _update_wrapper(wrapper, wrapped) -> None:  # noqa: ANN001
     functools.update_wrapper(wrapper, wrapped)
     # Need to manually update __wrapped__ to keep functions picklable
     del wrapper.__dict__["__wrapped__"]
 
 
-class PipelineFunction(Generic[T]):
+class PipeFunc(Generic[T]):
     """Function wrapper class for pipeline functions with additional attributes.
 
     Parameters
     ----------
     func
         The original function to be wrapped.
     output_name
@@ -81,24 +77,28 @@
         Flag indicating whether debug information should be printed.
     cache
         Flag indicating whether the wrapped function should be cached.
     save
         Flag indicating whether the output of the wrapped function should be saved.
     save_function
         A function that takes the filename and a dict containing the inputs and output.
+    mapspec
+        This is a specification for mapping that dictates how input values should
+        be merged together. If None, the default behavior is that the input directly
+        maps to the output.
 
     Returns
     -------
         The identifier for the output of the wrapped function.
 
     Examples
     --------
     >>> def add_one(a, b):
     ...     return a + 1, b + 1
-    >>> add_one_func = PipelineFunction(
+    >>> add_one_func = PipeFunc(
     ...     add_one,
     ...     output_name="a_plus_one",
     ...     renames={"a": "x", "b": "y"},
     ... )
     >>> add_one_func(x=1, y=2)
     (2, 3)
 
@@ -112,22 +112,26 @@
         output_picker: Callable[[str, Any], Any] | None = None,
         renames: dict[str, str] | None = None,
         profile: bool = False,
         debug: bool = False,
         cache: bool = False,
         save: bool | None = None,
         save_function: Callable[[str | Path, dict[str, Any]], None] | None = None,
+        mapspec: str | MapSpec | None = None,
     ) -> None:
         """Function wrapper class for pipeline functions with additional attributes."""
         _update_wrapper(self, func)
         self.func: Callable[..., Any] = func
         self.output_name: _OUTPUT_TYPE = output_name
         self.debug = debug
         self.cache = cache
         self.save_function = save_function
+        self.mapspec = (
+            MapSpec.from_string(mapspec) if isinstance(mapspec, str) else mapspec
+        )
         self.save = save if save is not None else save_function is not None
         self.output_picker: Callable[[Any, str], Any] | None = output_picker
         if output_picker is None and isinstance(output_name, tuple):
             self.output_picker = functools.partial(
                 _default_output_picker,
                 output_name=self.output_name,
             )
@@ -140,14 +144,15 @@
         self.defaults: dict[str, Any] = {
             self.renames.get(k, k): v.default
             for k, v in parameters.items()
             if v.default is not inspect.Parameter.empty
         }
         self.profiling_stats: ProfilingStats | None
         self.set_profiling(enable=profile)
+        self._validate_mapspec()
 
     def __call__(self, *args: Any, **kwargs: Any) -> Any:
         """Call the wrapped function with the given arguments.
 
         Returns
         -------
         Any
@@ -159,16 +164,17 @@
             args = evaluate_lazy(args)
             kwargs = evaluate_lazy(kwargs)
             result = self.func(*args, **kwargs)
 
         if self.debug and self.profiling_stats is not None:
             dt = self.profiling_stats.time.average
             print(
-                f"Function {self.func.__name__} called with args={args},"
-                f" kwargs={kwargs}, took {dt:.2e} seconds to execute.",
+                f"Function `{self.func.__name__}` -> with `output_name={self.output_name}`"
+                f" took {dt:.2e} seconds to execute and was"
+                f" called with `{args=}`, `{kwargs=}`, `{result=}`.",
             )
         return result
 
     @property
     def profile(self) -> bool:
         """Return whether profiling is enabled for the wrapped function."""
         return self._profile
@@ -216,52 +222,51 @@
         Any
             The value of the attribute.
 
         """
         return getattr(self.func, name)
 
     def __str__(self) -> str:
-        """Return a string representation of the PipelineFunction instance.
+        """Return a string representation of the PipeFunc instance.
 
         Returns
         -------
         str
-            A string representation of the PipelineFunction instance.
+            A string representation of the PipeFunc instance.
 
         """
-        params = ", ".join(self.parameters)
         outputs = ", ".join(at_least_tuple(self.output_name))
-        return f"{self.func.__name__}({params}) → {outputs}"
+        return f"{self.func.__name__}(...) → {outputs}"
 
     def __repr__(self) -> str:
-        """Return a string representation of the PipelineFunction instance.
+        """Return a string representation of the PipeFunc instance.
 
         Returns
         -------
         str
-            A string representation of the PipelineFunction instance.
+            A string representation of the PipeFunc instance.
 
         """
-        return f"PipelineFunction({self.func.__name__})"
+        return f"PipeFunc({self.func.__name__})"
 
     def __getstate__(self) -> dict:
         """Prepare the state of the current object for pickling.
 
         The state includes all picklable instance variables.
         For non-picklable instance variable,  they are transformed
         into a picklable form or ignored.
 
         Returns
         -------
         state : dict
             A dictionary containing the picklable state of the object.
 
         """
-        state = self.__dict__.copy()
-        state["func"] = cloudpickle.dumps(state.pop("func"))
+        state = {k: v for k, v in self.__dict__.items() if k != "func"}
+        state["func"] = cloudpickle.dumps(self.func)
         return state
 
     def __setstate__(self, state: dict) -> None:
         """Restore the state of the current object from the provided state.
 
         It also handles restoring non-picklable instance variable
         into their original form.
@@ -271,26 +276,58 @@
         state : dict
             A dictionary containing the picklable state of the object.
 
         """
         self.__dict__.update(state)
         self.func = cloudpickle.loads(self.func)
 
+    def _validate_mapspec(self) -> None:
+        if self.mapspec is None:
+            return
+
+        if not isinstance(self.mapspec, MapSpec):
+            msg = (
+                "The 'mapspec' argument should be an instance of MapSpec,"
+                f" not {type(self.mapspec)}."
+            )
+            raise TypeError(msg)
+
+        mapspec_input_names = {x.name for x in self.mapspec.inputs}
+        input_names = set(self.parameters)
+        if extra := mapspec_input_names - input_names:
+            msg = (
+                f"The input of the function `{self.__name__}` should match"
+                f" the input of the MapSpec `{self.mapspec}`:"
+                f" `{extra} not in {input_names}`."
+            )
+            raise ValueError(msg)
+
+        mapspec_output_names = {x.name for x in self.mapspec.outputs}
+        output_names = set(at_least_tuple(self.output_name))
+        if mapspec_output_names != output_names:
+            msg = (
+                f"The output of the function `{self.__name__}` should match"
+                f" the output of the MapSpec `{self.mapspec}`:"
+                f" `{mapspec_output_names} != {output_names}`."
+            )
+            raise ValueError(msg)
+
 
 def pipefunc(
     output_name: _OUTPUT_TYPE,
     *,
     output_picker: Callable[[Any, str], Any] | None = None,
     renames: dict[str, str] | None = None,
     profile: bool = False,
     debug: bool = False,
     cache: bool = False,
     save: bool | None = None,
     save_function: Callable[[str | Path, dict[str, Any]], None] | None = None,
-) -> Callable[[Callable[..., Any]], PipelineFunction]:
+    mapspec: str | MapSpec | None = None,
+) -> Callable[[Callable[..., Any]], PipeFunc]:
     """A decorator for tagging pipeline functions with a return identifier.
 
     Parameters
     ----------
     output_name
         The identifier for the output of the decorated function.
     output_picker
@@ -305,43 +342,48 @@
         Flag indicating whether debug information should be printed.
     cache
         Flag indicating whether the decorated function should be cached.
     save
         Flag indicating whether the output of the wrapped function should be saved.
     save_function
         A function that takes the filename and a dict containing the inputs and output.
+    mapspec
+        This is a specification for mapping that dictates how input values should
+        be merged together. If None, the default behavior is that the input directly
+        maps to the output.
 
     Returns
     -------
-    Callable[[Callable[..., Any]], PipelineFunction]
+    Callable[[Callable[..., Any]], PipeFunc]
         A decorator function that takes the original function and output_name a
-        PipelineFunction instance with the specified return identifier.
+        PipeFunc instance with the specified return identifier.
 
     """
 
-    def decorator(f: Callable[..., Any]) -> PipelineFunction:
-        """Wraps the original function in a PipelineFunction instance.
+    def decorator(f: Callable[..., Any]) -> PipeFunc:
+        """Wraps the original function in a PipeFunc instance.
 
         Parameters
         ----------
         f
             The original function to be wrapped.
 
         Returns
         -------
-        PipelineFunction
+        PipeFunc
             The wrapped function with the specified return identifier.
 
         """
-        return PipelineFunction(
+        return PipeFunc(
             f,
             output_name,
             output_picker=output_picker,
             renames=renames,
             profile=profile,
             debug=debug,
             cache=cache,
             save=save,
             save_function=save_function,
+            mapspec=mapspec,
         )
 
     return decorator
```

### Comparing `pipefunc-0.5.0/pipefunc/_pipeline.py` & `pipefunc-0.6.0/pipefunc/_pipeline.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,30 +18,30 @@
 import sys
 import time
 import warnings
 from collections import defaultdict
 from typing import (
     TYPE_CHECKING,
     Any,
-    Generator,
     Iterable,
     Literal,
     Tuple,
     Union,
-    cast,
 )
 
 import networkx as nx
 
-from pipefunc._cache import DiskCache, HybridCache, LRUCache
-from pipefunc._lazy import _LazyFunction
-from pipefunc._pipefunc import PipelineFunction
+from pipefunc._cache import DiskCache, HybridCache, LRUCache, SimpleCache
+from pipefunc._lazy import _LazyFunction, task_graph
+from pipefunc._pipefunc import PipeFunc
 from pipefunc._plotting import visualize, visualize_holoviews
 from pipefunc._simplify import _combine_nodes, _get_signature, _wrap_dict_to_tuple
-from pipefunc._utils import at_least_tuple, generate_filename_from_dict
+from pipefunc._utils import at_least_tuple, generate_filename_from_dict, handle_error
+from pipefunc.exceptions import UnusedParametersError
+from pipefunc.map._mapspec import MapSpec
 
 if sys.version_info < (3, 10):  # pragma: no cover
     from typing_extensions import TypeAlias
 else:
     from typing import TypeAlias
 
 
@@ -105,15 +105,15 @@
 
         Returns
         -------
         Any
             The return value of the pipeline function.
 
         """
-        return self.pipeline._run_pipeline(output_name=self.output_name, **kwargs)
+        return self.pipeline._run_pipeline(output_name=self.output_name, kwargs=kwargs)
 
     def call_full_output(self, **kwargs: Any) -> dict[str, Any]:
         """Call the pipeline function with the given arguments and return all outputs.
 
         Parameters
         ----------
         kwargs
@@ -124,15 +124,15 @@
         Any
             The return value of the pipeline function.
 
         """
         return self.pipeline._run_pipeline(
             output_name=self.output_name,
             full_output=True,
-            **kwargs,
+            kwargs=kwargs,
         )
 
     def call_with_dict(self, kwargs: dict[str, Any]) -> Any:
         """Call the pipeline function with the given arguments.
 
         Parameters
         ----------
@@ -159,37 +159,27 @@
             setattr(self, slot, state[slot])
         # Initialize _call_with_root_args if necessary
         self._call_with_root_args = None
 
     def _create_call_with_parameters_method(
         self,
         parameters: tuple[str, ...],
-        output_name: _OUTPUT_TYPE | None = None,
     ) -> Callable[..., Any]:
         sig = inspect.signature(self.__call__)
         new_params = [
             inspect.Parameter(name, inspect.Parameter.POSITIONAL_OR_KEYWORD)
             for name in parameters
         ]
         new_sig = sig.replace(parameters=new_params)
 
         def call(*args: Any, **kwargs: Any) -> Any:
             """Call the pipeline function with the root arguments."""
             bound = new_sig.bind(*args, **kwargs)
             bound.apply_defaults()
-            if output_name is None:
-                return self(**bound.arguments)
-            all_results = self.pipeline._run_pipeline(
-                output_name=self.output_name,
-                **bound.arguments,
-                full_output=True,
-            )
-            if isinstance(output_name, str):
-                return all_results[output_name]
-            return tuple(all_results[o] for o in output_name)
+            return self(**bound.arguments)
 
         call.__signature__ = new_sig  # type: ignore[attr-defined]
         return call
 
     def _create_call_with_root_args_method(self) -> Callable[..., Any]:
         return self._create_call_with_parameters_method(self.root_args)
 
@@ -201,88 +191,83 @@
     ----------
     functions
         A list of functions that form the pipeline.
     lazy
         Flag indicating whether the pipeline should be lazy.
     debug
         Flag indicating whether debug information should be printed.
-        If None, the value of each PipelineFunction's debug attribute is used.
+        If None, the value of each PipeFunc's debug attribute is used.
     profile
         Flag indicating whether profiling information should be collected.
-        If None, the value of each PipelineFunction's profile attribute is used.
+        If None, the value of each PipeFunc's profile attribute is used.
     cache_type
         The type of cache to use.
     cache_kwargs
         Keyword arguments passed to
 
     """
 
     def __init__(
         self,
-        functions: list[PipelineFunction],
+        functions: list[PipeFunc | tuple[PipeFunc, str | MapSpec]],
         *,
         lazy: bool = False,
         debug: bool | None = None,
         profile: bool | None = None,
-        cache_type: Literal["lru", "hybrid", "disk"] | None = "lru",
+        cache_type: Literal["lru", "hybrid", "disk", "simple"] | None = "lru",
         cache_kwargs: dict[str, Any] | None = None,
     ) -> None:
         """Pipeline class for managing and executing a sequence of functions."""
-        self.functions: list[PipelineFunction] = []
+        self.functions: list[PipeFunc] = []
         self.lazy = lazy
         self._debug = debug
         self._profile = profile
-        self.output_to_func: dict[_OUTPUT_TYPE, PipelineFunction] = {}
+        self.output_to_func: dict[_OUTPUT_TYPE, PipeFunc] = {}
         for f in functions:
-            self.add(f)
+            if isinstance(f, tuple):
+                f, mapspec = f  # noqa: PLW2901
+            else:
+                mapspec = None
+            self.add(f, mapspec=mapspec)
         self._init_internal_cache()
-        self._set_cache(cache_type, lazy, cache_kwargs)
+        self._cache_type = cache_type
+        self._cache_kwargs = cache_kwargs
+        self.cache = _create_cache(cache_type, lazy, cache_kwargs)
 
     def _init_internal_cache(self) -> None:
         # Internal Pipeline cache
         self._arg_combinations: dict[_OUTPUT_TYPE, set[tuple[str, ...]]] = {}
         self._root_args: dict[_OUTPUT_TYPE, tuple[str, ...]] = {}
         self._func: dict[_OUTPUT_TYPE, _Function] = {}
         with contextlib.suppress(AttributeError):
             del self.graph
         with contextlib.suppress(AttributeError):
             del self.root_nodes
         with contextlib.suppress(AttributeError):
             del self.leaf_nodes
         with contextlib.suppress(AttributeError):
             del self.unique_leaf_node
+        with contextlib.suppress(AttributeError):
+            del self.map_parameters
+        with contextlib.suppress(AttributeError):
+            del self.defaults
+        with contextlib.suppress(AttributeError):
+            del self.node_mapping
+        with contextlib.suppress(AttributeError):
+            del self.all_arg_combinations
+        with contextlib.suppress(AttributeError):
+            del self.all_root_args
+        with contextlib.suppress(AttributeError):
+            del self.topological_generations
 
-    def _set_cache(
-        self,
-        cache_type: Literal["lru", "hybrid", "disk"] | None,
-        lazy: bool,  # noqa: FBT001
-        cache_kwargs: dict[str, Any] | None,
-    ) -> None:
-        # Function result cache
-        self.cache: LRUCache | HybridCache | DiskCache | None = None
-        if cache_type is None:
-            return
-        if cache_kwargs is None:
-            cache_kwargs = {}
-        if cache_type == "lru":
-            cache_kwargs.setdefault("shared", not lazy)
-            self.cache = LRUCache(**cache_kwargs)
-        elif cache_type == "hybrid":
-            if lazy:
-                warnings.warn(
-                    "Hybrid cache uses function evaluation duration which"
-                    " is not measured correctly when using `lazy=True`.",
-                    UserWarning,
-                    stacklevel=2,
-                )
-            cache_kwargs.setdefault("shared", not lazy)
-            self.cache = HybridCache(**cache_kwargs)
-        elif cache_type == "disk":
-            cache_kwargs.setdefault("lru_shared", not lazy)
-            self.cache = DiskCache(**cache_kwargs)
+    def get_cache(self) -> LRUCache | HybridCache | DiskCache | SimpleCache | None:
+        """Return the cache used by the pipeline."""
+        if not isinstance(self.cache, SimpleCache) and (tg := task_graph()) is not None:
+            return tg.cache
+        return self.cache
 
     @property
     def profile(self) -> bool | None:
         """Flag indicating whether profiling information should be collected."""
         return self._profile
 
     @profile.setter
@@ -302,65 +287,109 @@
     def debug(self, value: bool | None) -> None:
         """Set the debug flag for the pipeline and all functions."""
         self._debug = value
         if value is not None:
             for f in self.functions:
                 f.debug = value
 
-    def add(self, f: PipelineFunction) -> None:
+    def add(
+        self,
+        f: PipeFunc | Callable,
+        mapspec: str | MapSpec | None = None,
+    ) -> PipeFunc:
         """Add a function to the pipeline.
 
         Parameters
         ----------
         f
             The function to add to the pipeline.
+        profile
+            Flag indicating whether profiling information should be collected.
+        mapspec
+            This is a specification for mapping that dictates how input values should
+            be merged together. If None, the default behavior is that the input directly
+            maps to the output.
 
         """
-        if not isinstance(f, PipelineFunction):
-            f = PipelineFunction(f, output_name=f.__name__)
+        if not isinstance(f, PipeFunc):
+            f = PipeFunc(f, output_name=f.__name__)
+        elif mapspec is not None:
+            msg = (
+                "Initializing the `Pipeline` using `MapSpec`s and"
+                " `PipeFunc`s modifies the `PipeFunc`s inplace."
+            )
+            warnings.warn(msg, UserWarning, stacklevel=2)
+
+        if mapspec is not None:
+            if isinstance(mapspec, str):
+                mapspec = MapSpec.from_string(mapspec)
+            f.mapspec = mapspec
+            f._validate_mapspec()
+
         self.functions.append(f)
 
         self.output_to_func[f.output_name] = f
         if isinstance(f.output_name, tuple):
             for name in f.output_name:
                 self.output_to_func[name] = f
 
         if self.profile is not None:
             f.set_profiling(enable=self.profile)
+
         if self.debug is not None:
             f.debug = self.debug
 
         self._init_internal_cache()  # reset cache
+        return f
 
-    def _check_consistent_defaults(self) -> None:
-        """Check that the default values for shared arguments are consistent."""
-        arg_defaults = defaultdict(set)
-        for f in self.functions:
-            for arg, default_value in f.defaults.items():
-                arg_defaults[arg].add(default_value)
-                if len(arg_defaults[arg]) > 1:
-                    msg = (
-                        f"Inconsistent default values for argument '{arg}' in"
-                        " functions. Please make sure the shared input arguments have"
-                        " the same default value or are set only for one function.",
-                    )
-                    raise ValueError(msg)
+    def drop(
+        self,
+        *,
+        f: PipeFunc | None = None,
+        output_name: _OUTPUT_TYPE | None = None,
+    ) -> None:
+        """Drop a function from the pipeline.
+
+        Parameters
+        ----------
+        f
+            The function to drop from the pipeline.
+        output_name
+            The name of the output to drop from the pipeline.
+
+        """
+        if (f is not None and output_name is not None) or (
+            f is None and output_name is None
+        ):
+            msg = "One of `f` or `output_name` should be provided."
+            raise ValueError(msg)
+        if f is not None:
+            self.functions.remove(f)
+            if isinstance(f.output_name, tuple):
+                for name in f.output_name:
+                    del self.output_to_func[name]
+            else:
+                del self.output_to_func[f.output_name]
+        elif output_name is not None:
+            f = self.output_to_func[output_name]
+            self.drop(f=f)
+        self._init_internal_cache()
 
     @functools.cached_property
     def graph(self) -> nx.DiGraph:
         """Create a directed graph representing the pipeline.
 
         Returns
         -------
         nx.DiGraph
             A directed graph with nodes representing functions and edges
             representing dependencies between functions.
 
         """
-        self._check_consistent_defaults()
+        _check_consistent_defaults(self.functions)
         g = nx.DiGraph()
         for f in self.functions:
             g.add_node(f)
             assert f.parameters is not None
             for arg in f.parameters:
                 if arg in self.output_to_func:  # is function output
                     edge = (self.output_to_func[arg], f)
@@ -426,131 +455,100 @@
             The return value of the pipeline.
 
         """
         if __output_name__ is None:
             __output_name__ = self.unique_leaf_node.output_name
         return self.func(__output_name__)(**kwargs)
 
-    def _compute_cache_key(
+    def _get_func_args(
         self,
-        output_name: _OUTPUT_TYPE,
+        func: PipeFunc,
         kwargs: dict[str, Any],
-    ) -> _CACHE_KEY_TYPE | None:
-        """Compute the cache key for a specific output name.
-
-        The cache key is a tuple consisting of the output name and a tuple of
-        root input keys and their corresponding values. Root inputs are the
-        inputs that are not derived from any other function in the pipeline.
-
-        If any of the root inputs required for the output_name are not available
-        in kwargs, the cache key computation is skipped, and the method returns
-        None. This can happen when a non-root input is directly provided as an
-        input to another function, in which case the result should not be
-        cached.
-
-        Parameters
-        ----------
-        output_name
-            The identifier for the return value of the pipeline.
-        kwargs
-            Keyword arguments to be passed to the pipeline functions.
-
-        Returns
-        -------
-        _CACHE_KEY_TYPE | None
-            A tuple containing the output name and a tuple of root input keys
-            and their corresponding values, or None if the cache key computation
-            is skipped.
-
-        """
-        root_args = self.root_args(output_name)
-        assert isinstance(root_args, tuple)
-        cache_key_items = []
-        for k in sorted(root_args):
-            if k not in kwargs:
-                # This means the computation was run with non-root inputs
-                # i.e., the output of a function was directly provided as an input to
-                # another function. In this case, we don't want to cache the result.
-                return None
-            cache_key_items.append((k, kwargs[k]))
-
-        return output_name, tuple(cache_key_items)
-
-    def _execute_pipeline(  # noqa: PLR0912
-        self,
-        *,
-        output_name: _OUTPUT_TYPE,
-        kwargs: Any,
         all_results: dict[_OUTPUT_TYPE, Any],
-        full_output: bool,
-    ) -> Any:
-        if output_name in all_results:
-            return all_results[output_name]
-
-        func = self.output_to_func[output_name]
-        assert func.parameters is not None
-        result_from_cache = False
-        if func.cache and self.cache is not None:
-            cache_key = self._compute_cache_key(func.output_name, kwargs)
-            if cache_key is not None and cache_key in self.cache:
-                r = self.cache.get(cache_key)
-                _update_all_results(func, r, output_name, all_results, self.lazy)
-                result_from_cache = True
-                if not full_output:
-                    return all_results[output_name]
-
+        full_output: bool,  # noqa: FBT001
+        used_parameters: set[str | None],
+    ) -> dict[str, Any]:
+        # Used in _execute_pipeline
         func_args = {}
         for arg in func.parameters:
             if arg in kwargs:
                 func_args[arg] = kwargs[arg]
             elif arg in func.defaults:
                 func_args[arg] = func.defaults[arg]
             else:
                 func_args[arg] = self._execute_pipeline(
                     output_name=arg,
                     kwargs=kwargs,
                     all_results=all_results,
                     full_output=full_output,
+                    used_parameters=used_parameters,
                 )
+        used_parameters.update(func_args)
+        return func_args
 
-        if result_from_cache:
-            # Can only happen if full_output is True
-            return all_results[output_name]
-        start_time = time.perf_counter()
+    def _execute_pipeline(
+        self,
+        *,
+        output_name: _OUTPUT_TYPE,
+        kwargs: Any,
+        all_results: dict[_OUTPUT_TYPE, Any],
+        full_output: bool,
+        used_parameters: set[str | None],
+    ) -> Any:
+        func = self.output_to_func[output_name]
+        assert func.parameters is not None
 
-        r = _LazyFunction(func, kwargs=func_args) if self.lazy else func(**func_args)
+        cache = self.get_cache()
+        use_cache = (func.cache and cache is not None) or task_graph() is not None
 
-        if func.cache and cache_key is not None and self.cache is not None:
-            if isinstance(self.cache, HybridCache):
-                duration = time.perf_counter() - start_time
-                self.cache.put(cache_key, r, duration)
-            else:
-                self.cache.put(cache_key, r)
+        root_args = self.root_args(output_name)
+        result_from_cache = False
+        if use_cache:
+            assert cache is not None
+            cache_key = _compute_cache_key(func.output_name, kwargs, root_args)
+            return_now, result_from_cache = _get_result_from_cache(
+                func,
+                cache,
+                cache_key,
+                output_name,
+                all_results,
+                full_output,
+                used_parameters,
+                self.lazy,
+            )
+            if return_now:
+                return all_results[output_name]
 
-        _update_all_results(func, r, output_name, all_results, self.lazy)
-        if func.save and not result_from_cache:
-            to_save = {k: all_results[k] for k in self.root_args(output_name)}
-            filename = generate_filename_from_dict(to_save)  # type: ignore[arg-type]
-            filename = func.__name__ / filename
-            to_save[output_name] = all_results[output_name]  # type: ignore[index]
-            assert func.save_function is not None
-            if self.lazy:
-                lazy_save = _LazyFunction(func.save_function, args=(filename, to_save))
-                r.add_delayed_callback(lazy_save)
-            else:
-                func.save_function(filename, to_save)  # type: ignore[arg-type]
+        func_args = self._get_func_args(
+            func,
+            kwargs,
+            all_results,
+            full_output,
+            used_parameters,
+        )
 
+        if result_from_cache:
+            assert full_output
+            return all_results[output_name]
+
+        start_time = time.perf_counter()
+        r = _execute_func(func, func_args, self.lazy)
+        if use_cache and cache_key is not None:
+            assert cache is not None
+            _update_cache(cache, cache_key, r, start_time)
+        _update_all_results(func, r, output_name, all_results, self.lazy)
+        _save_results(func, r, output_name, all_results, root_args, self.lazy)
         return all_results[output_name]
 
     def _run_pipeline(
         self,
         output_name: _OUTPUT_TYPE,
         *,
         full_output: bool = False,
-        **kwargs: Any,
+        kwargs: dict[str, Any],
     ) -> Any:
         """Execute the pipeline for a specific return value.
 
         Parameters
         ----------
         output_name
             The identifier for the return value of the pipeline.
@@ -563,210 +561,175 @@
         Returns
         -------
         Any
             The return value of the pipeline or a dictionary mapping function
             names to their return values if full_output is True.
 
         """
+        if output_name in kwargs:
+            msg = f"The `output_name='{output_name}'` argument cannot be provided in `kwargs={kwargs}`."
+            raise ValueError(msg)
+
         all_results: dict[_OUTPUT_TYPE, Any] = kwargs.copy()  # type: ignore[assignment]
+        used_parameters: set[str | None] = set()
+
         self._execute_pipeline(
             output_name=output_name,
             kwargs=kwargs,
             all_results=all_results,
             full_output=full_output,
+            used_parameters=used_parameters,
         )
+
+        # if has None, result was from cache, so we don't know which parameters were used
+        if None not in used_parameters and (
+            unused := set(kwargs) - set(used_parameters)
+        ):
+            unused_str = ", ".join(sorted(unused))
+            msg = f"Unused keyword arguments: `{unused_str}`. {kwargs=}, {used_parameters=}"
+            raise UnusedParametersError(msg)
+
         return all_results if full_output else all_results[output_name]
 
-    @property
-    def node_mapping(self) -> dict[_OUTPUT_TYPE, PipelineFunction | str]:
+    @functools.cached_property
+    def node_mapping(self) -> dict[_OUTPUT_TYPE, PipeFunc | str]:
         """Return a mapping from node names to nodes.
 
         Returns
         -------
-        Dict[_OUTPUT_TYPE, PipelineFunction | str]
+        Dict[_OUTPUT_TYPE, PipeFunc | str]
             A mapping from node names to nodes.
 
         """
-        mapping: dict[_OUTPUT_TYPE, PipelineFunction | str] = {}
+        mapping: dict[_OUTPUT_TYPE, PipeFunc | str] = {}
         for node in self.graph.nodes:
-            if isinstance(node, PipelineFunction):
+            if isinstance(node, PipeFunc):
                 if isinstance(node.output_name, tuple):
                     for name in node.output_name:
                         mapping[name] = node
                 mapping[node.output_name] = node
             else:
                 assert isinstance(node, str)
                 mapping[node] = node
         return mapping
 
-    def _next_root_args(
-        self,
-        arg_set: set[tuple[str, ...]],
-    ) -> tuple[str, ...]:
-        """Find the tuple of root arguments."""
-        return next(
-            args
-            for args in arg_set
-            if all(isinstance(self.node_mapping[n], str) for n in args)
-        )
-
-    def arg_combinations(
-        self,
-        output_name: _OUTPUT_TYPE,
-        *,
-        root_args_only: bool = False,
-    ) -> set[tuple[str, ...]] | tuple[str, ...]:
+    def arg_combinations(self, output_name: _OUTPUT_TYPE) -> set[tuple[str, ...]]:
         """Return the arguments required to compute a specific output.
 
         Parameters
         ----------
         output_name
             The identifier for the return value of the pipeline.
-        root_args_only
-            If True, only return the root arguments required to compute the
-            output. If False, return all arguments required to compute the
-            output.
 
         Returns
         -------
         Set[Tuple[str, ...]]
             A set of tuples containing possible argument combinations.
+            The tuples are sorted in lexicographical order.
 
         """
         if r := self._arg_combinations.get(output_name):
-            if root_args_only:
-                return self._next_root_args(r)
             return r
-
-        def names(nodes: Iterable[PipelineFunction | str]) -> tuple[str, ...]:
-            names: list[str] = []
-            for n in nodes:
-                if isinstance(n, PipelineFunction):
-                    names.extend(at_least_tuple(n.output_name))
-                else:
-                    assert isinstance(n, str)
-                    names.append(n)
-            return tuple(names)
-
-        def sort_key(node: PipelineFunction | str) -> str:
-            if isinstance(node, PipelineFunction):
-                if isinstance(node.output_name, tuple):
-                    return ",".join(node.output_name)
-                return node.output_name
-            return node
-
-        def unique(
-            nodes: Iterable[PipelineFunction | str],
-        ) -> tuple[PipelineFunction | str, ...]:
-            return tuple(sorted(set(nodes), key=sort_key))
-
-        def filter_funcs(
-            funcs: Iterable[PipelineFunction | str],
-        ) -> list[PipelineFunction]:
-            return [f for f in funcs if isinstance(f, PipelineFunction)]
-
-        def compute_arg_mapping(
-            node: PipelineFunction,
-            head: PipelineFunction,
-            args: list[PipelineFunction | str],
-            replaced: list[PipelineFunction | str],
-        ) -> None:
-            preds = [n for n in self.graph.predecessors(node) if n not in replaced]
-            deps = unique(args + preds)
-            deps_names = names(deps)
-            if deps_names in arg_set:
-                return
-            arg_set.add(deps_names)
-
-            for func in filter_funcs(deps):
-                new_args = [dep for dep in deps if dep != func]
-                compute_arg_mapping(func, head, new_args, [*replaced, node])
-
         head = self.node_mapping[output_name]
         arg_set: set[tuple[str, ...]] = set()
-        compute_arg_mapping(head, head, [], [])  # type: ignore[arg-type]
+        _compute_arg_mapping(self.graph, head, head, [], [], arg_set)  # type: ignore[arg-type]
         self._arg_combinations[output_name] = arg_set
-        if root_args_only:
-            return self._next_root_args(arg_set)
         return arg_set
 
     def root_args(self, output_name: _OUTPUT_TYPE) -> tuple[str, ...]:
         """Return the root arguments required to compute a specific output."""
         if r := self._root_args.get(output_name):
             return r
-        root_args = self.arg_combinations(output_name, root_args_only=True)
-        root_args = cast(Tuple[str, ...], root_args)
+        arg_combos = self.arg_combinations(output_name)
+        root_args = next(
+            args
+            for args in arg_combos
+            if all(isinstance(self.node_mapping[n], str) for n in args)
+        )
         self._root_args[output_name] = root_args
         return root_args
 
     def func_dependencies(self, output_name: _OUTPUT_TYPE) -> list[_OUTPUT_TYPE]:
         """Return the functions required to compute a specific output."""
 
-        def _predecessors(x: _OUTPUT_TYPE | PipelineFunction) -> list[_OUTPUT_TYPE]:
+        def _predecessors(x: _OUTPUT_TYPE | PipeFunc) -> list[_OUTPUT_TYPE]:
             preds = set()
             if isinstance(x, (str, tuple)):
                 x = self.node_mapping[x]
             for pred in self.graph.predecessors(x):
-                if isinstance(pred, PipelineFunction):
+                if isinstance(pred, PipeFunc):
                     preds.add(pred.output_name)
                     for p in _predecessors(pred):
                         preds.add(p)
             return preds  # type: ignore[return-value]
 
         return sorted(_predecessors(output_name), key=at_least_tuple)
 
-    def all_arg_combinations(
-        self,
-        *,
-        root_args_only: bool = False,
-    ) -> dict[_OUTPUT_TYPE, set[tuple[str, ...]]]:
+    @functools.cached_property
+    def all_arg_combinations(self) -> dict[_OUTPUT_TYPE, set[tuple[str, ...]]]:
         """Compute all possible argument mappings for the pipeline.
 
-        Considering only the root input nodes if `root_args_only` is
-        set to True.
-
-        Parameters
-        ----------
-        root_args_only
-            If True, the function will only consider the root input nodes
-            (i.e., nodes with no predecessor functions) while calculating the
-            possible argument combinations. If False, all predecessor nodes,
-            including intermediate functions, will be considered.
-
         Returns
         -------
         Dict[_OUTPUT_TYPE, Set[Tuple[str, ...]]]
             A dictionary mapping function names to sets of tuples containing
             possible argument combinations.
 
         """
-        mapping: dict[_OUTPUT_TYPE, set[tuple[str, ...]]] = defaultdict(set)
-        for node in self.graph.nodes:
-            if isinstance(node, PipelineFunction):
-                arg_combinations = self.arg_combinations(
-                    node.output_name,
-                    root_args_only=root_args_only,
-                )
-                if not isinstance(arg_combinations, set):  # root_args_only=True
-                    arg_combinations = {arg_combinations}
-                mapping[node.output_name] = arg_combinations
-        return mapping
+        return {
+            node.output_name: self.arg_combinations(node.output_name)
+            for node in self.graph.nodes
+            if isinstance(node, PipeFunc)
+        }
+
+    @functools.cached_property
+    def all_root_args(self) -> dict[_OUTPUT_TYPE, tuple[str, ...]]:
+        """Return the root arguments required to compute all outputs."""
+        return {
+            node.output_name: self.root_args(node.output_name)
+            for node in self.graph.nodes
+            if isinstance(node, PipeFunc)
+        }
 
     @functools.cached_property
-    def unique_leaf_node(self) -> PipelineFunction:
+    def map_parameters(self) -> set[str]:
+        map_parameters: set[str] = set()
+        for func in self.functions:
+            if func.mapspec:
+                map_parameters.update(func.mapspec.parameters)
+                for output in func.mapspec.outputs:
+                    map_parameters.add(output.name)
+        return map_parameters
+
+    @functools.cached_property
+    def defaults(self) -> dict[str, Any]:
+        defaults = {}
+        for func in self.functions:
+            defaults.update(func.defaults)
+        return defaults
+
+    @functools.cached_property
+    def unique_leaf_node(self) -> PipeFunc:
         """Return the unique leaf node of the pipeline graph."""
         leaf_nodes = self.leaf_nodes
         if len(leaf_nodes) != 1:  # pragma: no cover
             msg = (
                 "The pipeline has multiple leaf nodes. Please specify the output_name"
                 " argument to disambiguate.",
             )
             raise ValueError(msg)
         return leaf_nodes[0]
 
+    @functools.cached_property
+    def topological_generations(self) -> tuple[list[str], list[list[PipeFunc]]]:
+        generations = list(nx.topological_generations(self.graph))
+        assert all(isinstance(x, str) for x in generations[0])
+        assert all(isinstance(x, PipeFunc) for gen in generations[1:] for x in gen)
+        return generations[0], generations[1:]
+
     def _func_node_colors(
         self,
         *,
         conservatively_combine: bool = False,
         output_name: _OUTPUT_TYPE | None = None,
     ) -> list[str]:
         if output_name is None:
@@ -777,15 +740,15 @@
             output_name=output_name,
             conservatively_combine=conservatively_combine,
         )
         combinable_nodes = _combine_nodes(combinable_nodes)
         node_sets = [{k, *v} for k, v in combinable_nodes.items()]
         color_index = len(node_sets)  # for non-combinable nodes
         for node in self.graph.nodes:
-            if isinstance(node, PipelineFunction):
+            if isinstance(node, PipeFunc):
                 i = next(
                     (i for i, nodes in enumerate(node_sets) if node in nodes),
                     None,
                 )
                 if i is not None:
                     func_node_colors.append(f"C{i}")
                 else:
@@ -851,18 +814,18 @@
             )
 
     def _identify_combinable_nodes(
         self,
         output_name: _OUTPUT_TYPE,
         *,
         conservatively_combine: bool = False,
-    ) -> dict[PipelineFunction, set[PipelineFunction]]:
+    ) -> dict[PipeFunc, set[PipeFunc]]:
         """Identify which function nodes can be combined into a single function.
 
-        This method identifies the PipelineFunctions in the execution graph that
+        This method identifies the PipeFuncs in the execution graph that
         can be combined into a single function. The criterion for combinability
         is that the functions share the same root arguments.
 
         Parameters
         ----------
         output_name
             The name of the output from the pipeline function we are starting
@@ -873,23 +836,23 @@
             of its predecessors have the same root arguments as the function
             node itself. If False, combine a function node with its predecessors
             if any of its predecessors have the same root arguments as the
             function node.
 
         Returns
         -------
-        dict[PipelineFunction, set[PipelineFunction]]
-            A dictionary where each key is a PipelineFunction that can be
+        dict[PipeFunc, set[PipeFunc]]
+            A dictionary where each key is a PipeFunc that can be
             combined with others. The value associated with each key is a set of
-            PipelineFunctions that can be combined with the key function.
+            PipeFuncs that can be combined with the key function.
 
         Notes
         -----
         This function works by performing a depth-first search through the
-        pipeline's execution graph. Starting from the PipelineFunction
+        pipeline's execution graph. Starting from the PipeFunc
         corresponding to the `output_name`, it goes through each predecessor in
         the graph (functions that need to be executed before the current one).
         For each predecessor function, it recursively checks if it can be
         combined with others by comparing their root arguments.
 
         If a function's root arguments are identical to the head function's root
         arguments, it is considered combinable and added to the set of
@@ -903,32 +866,32 @@
         The function 'head' in the nested function `_recurse` represents the
         current function being checked in the execution graph.
 
         """
         # Nested function _recurse performs the depth-first search and updates the
         # `combinable_nodes` dictionary.
 
-        def _recurse(head: PipelineFunction) -> None:
+        def _recurse(head: PipeFunc) -> None:
             head_args = self.root_args(head.output_name)
             funcs = set()
             i = 0
             for node in self.graph.predecessors(head):
                 if isinstance(node, (tuple, str)):  # node is root_arg
                     continue
                 i += 1
                 _recurse(node)
                 node_args = self.root_args(node.output_name)
                 if node_args == head_args:
                     funcs.add(node)
             if funcs and (not conservatively_combine or i == len(funcs)):
                 combinable_nodes[head] = funcs
 
-        combinable_nodes: dict[PipelineFunction, set[PipelineFunction]] = {}
+        combinable_nodes: dict[PipeFunc, set[PipeFunc]] = {}
         func = self.node_mapping[output_name]
-        assert isinstance(func, PipelineFunction)
+        assert isinstance(func, PipeFunc)
         _recurse(func)
         return combinable_nodes
 
     def simplified_pipeline(
         self,
         output_name: _OUTPUT_TYPE | None = None,
         *,
@@ -1012,171 +975,79 @@
                 continue
             if f in combinable_nodes:
                 inputs = tuple(sorted(in_sig[f]))
                 outputs = tuple(sorted(out_sig[f]))
                 if len(outputs) == 1:
                     outputs = outputs[0]  # type: ignore[assignment]
                 funcs = [f, *combinable_nodes[f]]
-                mini_pipeline = Pipeline(funcs, debug=False, profile=False)
+                mini_pipeline = Pipeline(funcs)  # type: ignore[arg-type]
                 func = mini_pipeline.func(f.output_name).call_full_output
                 f_combined = _wrap_dict_to_tuple(func, inputs, outputs)
                 f_combined.__name__ = f"combined_{f.__name__}"
-                f_pipefunc = PipelineFunction(
+                f_pipefunc = PipeFunc(
                     f_combined,
                     outputs,
                     profile=f.profile,
                     save=f.save,
                     cache=f.cache,
                     save_function=f.save_function,
                 )
                 # Disable saving for all functions that are being combined
                 for f_ in funcs:
                     f_.save = False
                 f_pipefunc.parameters = list(inputs)
                 new_functions.append(f_pipefunc)
             elif f not in skip:
                 new_functions.append(f)
-        return Pipeline(new_functions)
-
-    def all_execution_orders(
-        self,
-        output_name: str,
-    ) -> Generator[list[PipelineFunction], None, None]:
-        """Generate all possible execution orders for the functions in the pipeline.
-
-        This method generates all possible topological sorts (execution orders)
-        of the functions in the pipeline's execution graph. It first simplifies the
-        pipeline to a version where combinable function nodes have been merged
-        into single function nodes, and then generates all topological sorts of
-        the functions in the simplified graph.
-
-        The method only considers the functions in the graph and ignores the
-        root arguments.
-
-        Parameters
-        ----------
-        output_name
-            The name of the output from the pipeline function we are starting
-            from. It is used to get the starting function in the pipeline and to
-            determine the simplified pipeline.
-
-        Returns
-        -------
-        Generator[list[str], None, None]
-            A generator that yields lists of function names, each list
-            representing a possible execution order of the functions in the
-            pipeline.
-
-        Notes
-        -----
-        A topological sort of a directed graph is a linear ordering of its
-        vertices such that for every directed edge U -> V from vertex U to
-        vertex V, U comes before V in the ordering. For a pipeline, this means
-        that each function only gets executed after all its dependencies have
-        been executed.
-
-        The method uses the NetworkX function `all_topological_sorts` to
-        generate all possible topological sorts. If there are cycles in the
-        graph (i.e., there's a circular dependency between functions), the
-        method will raise a NetworkXUnfeasible exception.
-
-        The function 'head' in the nested function `_recurse` represents the
-        current function being checked in the execution graph.
-
-        """
-        simplified_pipeline = self.simplified_pipeline(output_name)
-        func_only_graph = simplified_pipeline.graph.copy()
-        root_args = simplified_pipeline.arg_combinations(
-            output_name,
-            root_args_only=True,
-        )
-        for arg in root_args:
-            func_only_graph.remove_node(arg)
-        return nx.all_topological_sorts(func_only_graph)
+        return Pipeline(new_functions)  # type: ignore[arg-type]
 
     @functools.cached_property
-    def leaf_nodes(self) -> list[PipelineFunction]:
+    def leaf_nodes(self) -> list[PipeFunc]:
         """Return the leaf nodes in the pipeline's execution graph."""
         return [node for node in self.graph.nodes() if self.graph.out_degree(node) == 0]
 
     @functools.cached_property
-    def root_nodes(self) -> list[PipelineFunction]:
+    def root_nodes(self) -> list[PipeFunc]:
         """Return the root nodes in the pipeline's execution graph."""
         return [node for node in self.graph.nodes() if self.graph.in_degree(node) == 0]
 
-    def all_transitive_paths(
-        self,
-        output_name: str,
-        *,
-        simplify: bool = False,
-    ) -> list[list[list[PipelineFunction]]]:
-        """Get all possible transitive paths for a specified output.
-
-        This method retrieves all the possible ways the functions in the
-        pipeline can be ordered (transitive paths) to produce a specified
-        output.
-
-        Parameters
-        ----------
-        output_name
-            The name of the output variable to find paths for.
-        simplify
-            A flag indicating whether to simplify the pipeline before computing
-            the paths. If True, the pipeline is first simplified to a sub-pipeline
-            that is necessary for producing the output_name. If False, the paths
-            are computed on the full pipeline. Default is False.
-
-        Returns
-        -------
-        list[list[list[PipelineFunction]]]
-            A list of lists of lists of `PipelineFunction`s. Each list of lists
-            represents an independent chain of computation in the pipeline that
-            can produce the output. Each list of `PipelineFunction` represents a
-            possible ordering of functions in that chain.
-
-        """
-        pipeline = self.simplified_pipeline(output_name) if simplify else self
-
-        func_only_graph = pipeline.graph.copy()
-        root_args = pipeline.root_args(output_name)
-        for arg in root_args:
-            func_only_graph.remove_node(arg)
-
-        leaf = next(
-            n
-            for n in func_only_graph.nodes
-            if output_name in at_least_tuple(n.output_name)
-        )
-        roots = [n for n, d in func_only_graph.in_degree() if d == 0]
-        graph = nx.transitive_reduction(func_only_graph)
-        return [list(nx.all_simple_paths(graph, root, leaf)) for root in roots]
-
     @property
     def profiling_stats(self) -> dict[str, ProfilingStats]:
         """Return the profiling data for each function in the pipeline."""
         return {
             f.__name__: f.profiling_stats for f in self.functions if f.profiling_stats
         }
 
     def __str__(self) -> str:
         """Return a string representation of the pipeline."""
         pipeline_str = "Pipeline:\n"
         for node in self.graph.nodes:
-            if isinstance(node, PipelineFunction):
+            if isinstance(node, PipeFunc):
                 fn = node
-                input_args = self.all_arg_combinations()[fn.output_name]
+                input_args = self.all_arg_combinations[fn.output_name]
                 pipeline_str += (
                     f"  {fn.output_name} = {fn.__name__}({', '.join(fn.parameters)})\n"
                 )
                 pipeline_str += f"    Possible input arguments: {input_args}\n"
         return pipeline_str
 
+    def copy(self) -> Pipeline:
+        """Return a copy of the pipeline."""
+        return Pipeline(
+            self.functions,  # type: ignore[arg-type]
+            lazy=self.lazy,
+            debug=self._debug,
+            profile=self._profile,
+            cache_type=self._cache_type,
+            cache_kwargs=self._cache_kwargs,
+        )
+
 
 def _update_all_results(
-    func: PipelineFunction,
+    func: PipeFunc,
     r: Any,
     output_name: _OUTPUT_TYPE,
     all_results: dict[_OUTPUT_TYPE, Any],
     lazy: bool,  # noqa: FBT001
 ) -> None:
     if isinstance(func.output_name, tuple) and not isinstance(output_name, tuple):
         # Function produces multiple outputs, but only one is requested
@@ -1185,7 +1056,234 @@
             all_results[name] = (
                 _LazyFunction(func.output_picker, args=(r, name))
                 if lazy
                 else func.output_picker(r, name)
             )
     else:
         all_results[func.output_name] = r
+
+
+def _valid_key(key: Any) -> Any:
+    if isinstance(key, dict):
+        return tuple(sorted(key.items()))
+    if isinstance(key, list):
+        return tuple(key)
+    if isinstance(key, set):
+        return tuple(sorted(key))
+    return key
+
+
+def _update_cache(
+    cache: LRUCache | HybridCache | DiskCache | SimpleCache,
+    cache_key: _CACHE_KEY_TYPE,
+    r: Any,
+    start_time: float,
+) -> None:
+    # Used in _execute_pipeline
+    if isinstance(cache, HybridCache):
+        duration = time.perf_counter() - start_time
+        cache.put(cache_key, r, duration)
+    else:
+        cache.put(cache_key, r)
+
+
+def _get_result_from_cache(
+    func: PipeFunc,
+    cache: LRUCache | HybridCache | DiskCache | SimpleCache,
+    cache_key: _CACHE_KEY_TYPE | None,
+    output_name: _OUTPUT_TYPE,
+    all_results: dict[_OUTPUT_TYPE, Any],
+    full_output: bool,  # noqa: FBT001
+    used_parameters: set[str | None],
+    lazy: bool = False,  # noqa: FBT002, FBT001
+) -> tuple[bool, bool]:
+    # Used in _execute_pipeline
+    result_from_cache = False
+    if cache_key is not None and cache_key in cache:
+        r = cache.get(cache_key)
+        _update_all_results(func, r, output_name, all_results, lazy)
+        result_from_cache = True
+        if not full_output:
+            used_parameters.add(None)  # indicate that the result was from cache
+            return True, result_from_cache
+    return False, result_from_cache
+
+
+def _check_consistent_defaults(functions: list[PipeFunc]) -> None:
+    """Check that the default values for shared arguments are consistent."""
+    arg_defaults = defaultdict(set)
+    for f in functions:
+        for arg, default_value in f.defaults.items():
+            arg_defaults[arg].add(default_value)
+            if len(arg_defaults[arg]) > 1:
+                msg = (
+                    f"Inconsistent default values for argument '{arg}' in"
+                    " functions. Please make sure the shared input arguments have"
+                    " the same default value or are set only for one function.",
+                )
+                raise ValueError(msg)
+
+
+def _create_cache(
+    cache_type: Literal["lru", "hybrid", "disk", "simple"] | None,
+    lazy: bool,  # noqa: FBT001
+    cache_kwargs: dict[str, Any] | None,
+) -> LRUCache | HybridCache | DiskCache | SimpleCache | None:
+    if cache_type is None:
+        return None
+    if cache_kwargs is None:
+        cache_kwargs = {}
+    if cache_type == "lru":
+        cache_kwargs.setdefault("shared", not lazy)
+        return LRUCache(**cache_kwargs)
+    if cache_type == "hybrid":
+        if lazy:
+            warnings.warn(
+                "Hybrid cache uses function evaluation duration which"
+                " is not measured correctly when using `lazy=True`.",
+                UserWarning,
+                stacklevel=2,
+            )
+        cache_kwargs.setdefault("shared", not lazy)
+        return HybridCache(**cache_kwargs)
+    if cache_type == "disk":
+        cache_kwargs.setdefault("lru_shared", not lazy)
+        return DiskCache(**cache_kwargs)
+    if cache_type == "simple":
+        return SimpleCache()
+
+    msg = f"Invalid cache type: {cache_type}."
+    raise ValueError(msg)
+
+
+def _execute_func(func: PipeFunc, func_args: dict[str, Any], lazy: bool) -> Any:  # noqa: FBT001
+    if lazy:
+        return _LazyFunction(func, kwargs=func_args)
+    try:
+        return func(**func_args)
+    except Exception as e:
+        handle_error(e, func, func_args)
+        raise  # handle_error raises but mypy doesn't know that
+
+
+def _compute_cache_key(
+    output_name: _OUTPUT_TYPE,
+    kwargs: dict[str, Any],
+    root_args: tuple[str, ...],
+) -> _CACHE_KEY_TYPE | None:
+    """Compute the cache key for a specific output name.
+
+    The cache key is a tuple consisting of the output name and a tuple of
+    root input keys and their corresponding values. Root inputs are the
+    inputs that are not derived from any other function in the pipeline.
+
+    If any of the root inputs required for the output_name are not available
+    in kwargs, the cache key computation is skipped, and the method returns
+    None. This can happen when a non-root input is directly provided as an
+    input to another function, in which case the result should not be
+    cached.
+
+    Parameters
+    ----------
+    output_name
+        The identifier for the return value of the pipeline.
+    kwargs
+        Keyword arguments to be passed to the pipeline functions.
+    root_args
+        The names of the pipeline function's root inputs.
+
+    Returns
+    -------
+    _CACHE_KEY_TYPE | None
+        A tuple containing the output name and a tuple of root input keys
+        and their corresponding values, or None if the cache key computation
+        is skipped.
+
+    """
+    cache_key_items = []
+    for k in root_args:
+        if k not in kwargs:
+            # This means the computation was run with non-root inputs
+            # i.e., the output of a function was directly provided as an input to
+            # another function. In this case, we don't want to cache the result.
+            return None
+        key = _valid_key(kwargs[k])
+        cache_key_items.append((k, key))
+
+    return output_name, tuple(cache_key_items)
+
+
+def _save_results(
+    func: PipeFunc,
+    r: Any,
+    output_name: _OUTPUT_TYPE,
+    all_results: dict[_OUTPUT_TYPE, Any],
+    root_args: tuple[str, ...],
+    lazy: bool,  # noqa: FBT001
+) -> None:
+    # Used in _execute_pipeline
+    if func.save:
+        to_save = {k: all_results[k] for k in root_args}
+        filename = generate_filename_from_dict(to_save)  # type: ignore[arg-type]
+        filename = func.__name__ / filename
+        to_save[output_name] = all_results[output_name]  # type: ignore[index]
+        assert func.save_function is not None
+        if lazy:
+            lazy_save = _LazyFunction(
+                func.save_function,
+                args=(filename, to_save),
+                add_to_graph=False,
+            )
+            r.add_delayed_callback(lazy_save)
+        else:
+            func.save_function(filename, to_save)  # type: ignore[arg-type]
+
+
+def _names(nodes: Iterable[PipeFunc | str]) -> tuple[str, ...]:
+    names: list[str] = []
+    for n in nodes:
+        if isinstance(n, PipeFunc):
+            names.extend(at_least_tuple(n.output_name))
+        else:
+            assert isinstance(n, str)
+            names.append(n)
+    return tuple(sorted(names))
+
+
+def _sort_key(node: PipeFunc | str) -> str:
+    if isinstance(node, PipeFunc):
+        if isinstance(node.output_name, tuple):
+            return ",".join(node.output_name)
+        return node.output_name
+    return node
+
+
+def _unique(
+    nodes: Iterable[PipeFunc | str],
+) -> tuple[PipeFunc | str, ...]:
+    return tuple(sorted(set(nodes), key=_sort_key))
+
+
+def _filter_funcs(
+    funcs: Iterable[PipeFunc | str],
+) -> list[PipeFunc]:
+    return [f for f in funcs if isinstance(f, PipeFunc)]
+
+
+def _compute_arg_mapping(
+    graph: nx.DiGraph,
+    node: PipeFunc,
+    head: PipeFunc,
+    args: list[PipeFunc | str],
+    replaced: list[PipeFunc | str],
+    arg_set: set[tuple[str, ...]],
+) -> None:
+    preds = [n for n in graph.predecessors(node) if n not in replaced]
+    deps = _unique(args + preds)
+    deps_names = _names(deps)
+    if deps_names in arg_set:
+        return
+    arg_set.add(deps_names)
+
+    for func in _filter_funcs(deps):
+        new_args = [dep for dep in deps if dep != func]
+        _compute_arg_mapping(graph, func, head, new_args, [*replaced, node], arg_set)
```

### Comparing `pipefunc-0.5.0/pipefunc/_plotting.py` & `pipefunc-0.6.0/pipefunc/_plotting.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
     pos = _get_graph_layout(graph)
     arg_nodes = []
     func_nodes = []
     for node in graph.nodes:
         if isinstance(node, str):
             arg_nodes.append(node)
-        else:  # is PipelineFunction
+        else:  # is PipeFunc
             func_nodes.append(node)
 
     plt.figure(figsize=figsize)
     nx.draw_networkx_nodes(
         graph,
         pos,
         nodelist=arg_nodes,
@@ -96,15 +96,15 @@
         a, b = edge
         if isinstance(a, str):
             default_value = graph.nodes[a]["default_value"]
             if default_value is not inspect.Parameter.empty:
                 inputs[edge] = f"{a}={default_value}"
             else:
                 inputs[edge] = a
-        else:  # is PipelineFunction
+        else:  # is PipeFunc
             arg = attrs["arg"]
             if isinstance(arg, tuple):
                 arg = ", ".join(arg)
             outputs[edge] = arg
 
     nx.draw_networkx_edge_labels(
         graph,
```

### Comparing `pipefunc-0.5.0/pipefunc/_simplify.py` & `pipefunc-0.6.0/pipefunc/_simplify.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 from __future__ import annotations
 
 import inspect
 from collections import OrderedDict
-from typing import (
-    TYPE_CHECKING,
-    Any,
-)
+from typing import TYPE_CHECKING, Any
 
 from pipefunc._utils import at_least_tuple
 
 if TYPE_CHECKING:
     import sys
 
     if sys.version_info < (3, 9):  # pragma: no cover
         from typing import Callable
     else:
         from collections.abc import Callable
 
     import networkx as nx
 
-    from pipefunc._pipefunc import PipelineFunction
+    from pipefunc._pipefunc import PipeFunc
 
 
 def _wrap_dict_to_tuple(
     func: Callable[..., Any],
     inputs: tuple[str, ...],
     output_name: str | tuple[str, ...],
 ) -> Callable[..., Any]:
@@ -45,22 +42,22 @@
 
     call.__signature__ = new_sig  # type: ignore[attr-defined]
 
     return call
 
 
 def _combine_nodes(
-    combinable_nodes: dict[PipelineFunction, set[PipelineFunction]],
-) -> dict[PipelineFunction, set[PipelineFunction]]:
+    combinable_nodes: dict[PipeFunc, set[PipeFunc]],
+) -> dict[PipeFunc, set[PipeFunc]]:
     """Reduce the dictionary of combinable nodes to a minimal set.
 
     The input dictionary `combinable_nodes` indicates which nodes
     (functions in the pipeline) can be combined together. The dictionary
-    keys are PipelineFunction objects, and the values are sets of
-    PipelineFunction objects that the key depends on and can be
+    keys are PipeFunc objects, and the values are sets of
+    PipeFunc objects that the key depends on and can be
     combined with. For example,
     if `combinable_nodes = {f6: {f5}, f5: {f1, f4}}`, it means that `f6`
     can be combined with `f5`, and `f5` can be combined with `f1` and `f4`.
 
     This method simplifies the input dictionary by iteratively checking each
     node in the dictionary to see if it is a dependency of any other nodes.
     If it is, the method replaces that dependency with the node's own
@@ -73,21 +70,21 @@
     The aim is to get a dictionary where each node only depends on nodes
     that cannot be further combined. This simplified dictionary is useful for
     constructing a simplified graph of the computation.
 
     Parameters
     ----------
     combinable_nodes
-        A dictionary where the keys are PipelineFunction objects, and the
-        values are sets of PipelineFunction objects that can be combined
+        A dictionary where the keys are PipeFunc objects, and the
+        values are sets of PipeFunc objects that can be combined
         with the key.
 
     Returns
     -------
-    Dict[PipelineFunction, Set[PipelineFunction]]
+    Dict[PipeFunc, Set[PipeFunc]]
         A simplified dictionary where each node only depends on nodes
         that cannot be further combined.
 
     """
     combinable_nodes = OrderedDict(combinable_nodes)
     for _ in range(len(combinable_nodes)):
         node, deps = combinable_nodes.popitem(last=False)
@@ -98,17 +95,17 @@
                 added_nodes.append(_node)
         if not added_nodes:
             combinable_nodes[node] = deps
     return dict(combinable_nodes)
 
 
 def _get_signature(
-    combinable_nodes: dict[PipelineFunction, set[PipelineFunction]],
+    combinable_nodes: dict[PipeFunc, set[PipeFunc]],
     graph: nx.DiGraph,
-) -> tuple[dict[PipelineFunction, set[str]], dict[PipelineFunction, set[str]]]:
+) -> tuple[dict[PipeFunc, set[str]], dict[PipeFunc, set[str]]]:
     """Retrieve the inputs and outputs for the signature of the combinable nodes.
 
     This function generates a mapping of the inputs and outputs required for
     each node in the combinable_nodes dictionary. For each node, it collects
     the outputs of all nodes it depends on and the parameters it and its
     dependent nodes require. In addition, it considers additional outputs
     based on the dependencies in the graph. It then filters these lists to
@@ -124,18 +121,18 @@
     graph
         The directed graph of the pipeline functions. Each node represents a
         function, and each edge represents a dependency relationship between
         functions.
 
     Returns
     -------
-    all_inputs : dict[PipelineFunction, set[str]]
+    all_inputs : dict[PipeFunc, set[str]]
         Dictionary where keys are nodes and values are sets of parameter
         names that the node and its dependent nodes require.
-    all_outputs : dict[PipelineFunction, set[str]]
+    all_outputs : dict[PipeFunc, set[str]]
         Dictionary where keys are nodes and values are sets of output names
         that the node and its dependent nodes produce, plus additional output
         names based on the dependency relationships in the graph.
 
     """
     all_inputs = {}
     all_outputs = {}
```

### Comparing `pipefunc-0.5.0/pipefunc/_sweep.py` & `pipefunc-0.6.0/pipefunc/_sweep.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import TYPE_CHECKING, Any, Callable, Generator, Hashable, Sequence
 
 import networkx as nx
 
 from pipefunc._utils import at_least_tuple
 
 if TYPE_CHECKING:
-    from pipefunc._pipeline import _OUTPUT_TYPE, Pipeline, PipelineFunction
+    from pipefunc._pipeline import _OUTPUT_TYPE, PipeFunc, Pipeline
 
 
 def _combined_exclude(
     *func: Callable[[Mapping[str, Any]], bool] | None,
 ) -> Callable[[Mapping[str, Any]], bool] | None:
     """Combine multiple exclude functions into one."""
     funcs = [f for f in func if f is not None]
@@ -95,15 +95,14 @@
         self,
         items: dict[str, Sequence[Any]],
         dims: list[str | tuple[str, ...]] | None = None,
         exclude: Callable[[Mapping[str, Any]], bool] | None = None,
         constants: Mapping[str, Any] | None = None,
         derivers: dict[str, Callable[[dict[str, Any]], Any]] | None = None,
     ) -> None:
-        """Initialize the sweep."""
         self.items = items
         self.dims = dims
         self.exclude = exclude
         self.constants = constants
         self.derivers = derivers
 
     def generate(self) -> Generator[dict[str, Any], None, None]:  # noqa: PLR0912
@@ -464,15 +463,15 @@
     if isinstance(sweep, Sweep):
         # TODO: we can likely special case this to be faster.
         sweep = sweep.list()  # type: ignore[assignment]
     assert isinstance(sweep, Iterable)
     counts: dict[_OUTPUT_TYPE, dict[tuple[Any, ...], int]] = {}
     deps = pipeline.func_dependencies(output_name)
     for _output_name in deps:
-        arg_combination = pipeline.arg_combinations(_output_name, root_args_only=True)
+        arg_combination = pipeline.root_args(_output_name)
         assert isinstance(arg_combination, tuple)
         if use_pandas:
             import pandas as pd
 
             df = pd.DataFrame(list(sweep))
             cols = list(arg_combination)
             counts[_output_name] = df[cols].groupby(cols).size().to_dict()  # type: ignore[assignment]
@@ -506,15 +505,15 @@
         func.cache = enable_cache  # type: ignore[union-attr]
 
 
 def get_precalculation_order(
     pipeline: Pipeline,
     counts: dict[str | tuple[str, ...], dict[tuple[Any, ...], int]],
     min_executions: int = 2,
-) -> list[PipelineFunction]:
+) -> list[PipeFunc]:
     """Determine the order in which functions in a pipeline should be precalculated and cached.
 
     The order is determined by the topological dependencies of the functions
     and the count of their executions in the context of a parameter sweep.
     Only functions that are executed multiple times (as specified by `min_executions`)
     are included in the precalculation order.
 
@@ -527,20 +526,20 @@
         parameter combinations and their counts in the pipeline.
     min_executions
         The minimum number of times a function must be used in the pipeline
         for it to be included in the precalculation order. Defaults to 2.
 
     Returns
     -------
-    list[PipelineFunction]
+    list[PipeFunc]
         The ordered list of functions to be precalculated and cached.
 
     """
 
-    def key_func(node: PipelineFunction) -> int:
+    def key_func(node: PipeFunc) -> int:
         return -sum(counts[node.output_name].values())
 
     m = pipeline.node_mapping
     # Get nodes with counts ≥min_executions
     nodes_with_counts = [
         m[node]
         for node, count_dict in counts.items()
@@ -620,15 +619,15 @@
         keys[left_overs[level]].add(k)
         if isinstance(v, dict):
             _assert_valid_sweep_dict(v, left_overs, keys, level + 1)
     return keys
 
 
 def get_min_sweep_sets(
-    execution_order: list[PipelineFunction],
+    execution_order: list[PipeFunc],
     pipeline: Pipeline,
     sweep: Sweep,
     output_name: str,
 ) -> tuple[list[tuple[str, ...]], dict]:
     """Create sweep combinations for each function in the execution order.
 
     This function iterates through the execution order of the pipeline functions
```

### Comparing `pipefunc-0.5.0/pipefunc.egg-info/PKG-INFO` & `pipefunc-0.6.0/pipefunc.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipefunc
-Version: 0.5.0
+Version: 0.6.0
 Summary: A Python library for defining, managing, and executing function pipelines.
 Maintainer-email: Bas Nijholt <bas@nijho.lt>
 License: MIT
 Project-URL: homepage, https://pipefunc.readthedocs.io/
 Project-URL: documentation, https://pipefunc.readthedocs.io/
 Project-URL: repository, https://github.com/basnijholt/pipefunc
 Classifier: Development Status :: 4 - Beta
@@ -26,33 +26,38 @@
 License-File: LICENSE
 License-File: AUTHORS.md
 Requires-Dist: networkx
 Requires-Dist: psutil
 Requires-Dist: versioningit
 Requires-Dist: typing_extensions; python_version <= "3.9"
 Requires-Dist: cloudpickle
+Requires-Dist: numpy
+Provides-Extra: adaptive
+Requires-Dist: adaptive; extra == "adaptive"
+Requires-Dist: adaptive-scheduler; extra == "adaptive"
 Provides-Extra: plotting
 Requires-Dist: matplotlib; extra == "plotting"
 Requires-Dist: pygraphviz; extra == "plotting"
 Requires-Dist: holoviews; extra == "plotting"
 Requires-Dist: bokeh; extra == "plotting"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pandas; extra == "test"
+Requires-Dist: adaptive; extra == "test"
 Provides-Extra: docs
 Requires-Dist: myst-nb; extra == "docs"
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
 Requires-Dist: emoji; extra == "docs"
 Requires-Dist: jupytext; extra == "docs"
 Requires-Dist: jupyterlite-sphinx; extra == "docs"
-Requires-Dist: jupyterlite-xeus-python; extra == "docs"
+Requires-Dist: jupyterlite-xeus; extra == "docs"
 Requires-Dist: pandas; extra == "docs"
 Provides-Extra: dev
 Requires-Dist: black[jupyter]; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 
@@ -145,15 +150,15 @@
 assert h_e(a=2, b=3, x=1) == 75
 assert h_e(c=5, d=15, x=1) == 75
 
 # Visualize the pipeline
 pipeline.visualize()
 
 # Get all possible argument mappings for each function
-all_args = pipeline.all_arg_combinations()
+all_args = pipeline.all_arg_combinations
 print(all_args)
 
 # Show resource reporting (only works if profile=True)
 pipeline.resources_report()
 ```
 
 This example demonstrates defining a pipeline with `f_c`, `f_d`, `f_e` functions, accessing and executing these functions using the pipeline, visualizing the pipeline graph, getting all possible argument mappings, and reporting on the resource usage.
```

### Comparing `pipefunc-0.5.0/pipefunc.egg-info/SOURCES.txt` & `pipefunc-0.6.0/pipefunc.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -11,18 +11,25 @@
 pipefunc/_pipefunc.py
 pipefunc/_pipeline.py
 pipefunc/_plotting.py
 pipefunc/_simplify.py
 pipefunc/_sweep.py
 pipefunc/_utils.py
 pipefunc/_version.py
+pipefunc/exceptions.py
 pipefunc.egg-info/PKG-INFO
 pipefunc.egg-info/SOURCES.txt
 pipefunc.egg-info/dependency_links.txt
 pipefunc.egg-info/requires.txt
 pipefunc.egg-info/top_level.txt
+pipefunc/map/__init__.py
+pipefunc/map/_adaptive.py
+pipefunc/map/_filearray.py
+pipefunc/map/_mapspec.py
+pipefunc/map/_run.py
 tests/test_cache.py
 tests/test_dag.py
 tests/test_perf.py
 tests/test_pipefunc.py
 tests/test_simplify.py
-tests/test_sweep.py
+tests/test_sweep.py
+tests/test_utils.py
```

### Comparing `pipefunc-0.5.0/pyproject.toml` & `pipefunc-0.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -27,27 +27,29 @@
 ]
 dependencies = [
     "networkx",
     "psutil",
     "versioningit",
     "typing_extensions; python_version <= '3.9'",
     "cloudpickle",
+    "numpy",
 ]
 [project.optional-dependencies]
+adaptive = ["adaptive", "adaptive-scheduler"]
 plotting = ["matplotlib", "pygraphviz", "holoviews", "bokeh"]
-test = ["pytest", "coverage", "pytest-cov", "pandas"]
+test = ["pytest", "coverage", "pytest-cov", "pandas", "adaptive"]
 docs = [
     "myst-nb",
     "sphinx",
     "furo",
     "myst-parser",
     "emoji",
     "jupytext",
     "jupyterlite-sphinx",
-    "jupyterlite-xeus-python",
+    "jupyterlite-xeus",
     "pandas",                  # used in example.ipynb
 ]
 dev = ["black[jupyter]", "pre-commit", "ruff", "mypy"]
 [project.urls]
 homepage = "https://pipefunc.readthedocs.io/"
 documentation = "https://pipefunc.readthedocs.io/"
 repository = "https://github.com/basnijholt/pipefunc"
```

### Comparing `pipefunc-0.5.0/tests/test_cache.py` & `pipefunc-0.6.0/tests/test_cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import pickle
 import time
 from typing import TYPE_CHECKING
 
 import pytest
 
-from pipefunc._cache import DiskCache, HybridCache, LRUCache
+from pipefunc._cache import DiskCache, HybridCache, LRUCache, SimpleCache
 
 if TYPE_CHECKING:
     from pathlib import Path
 
 
 @pytest.mark.parametrize("shared", [True, False])
 def test_hybrid_cache_init(shared):
@@ -368,7 +368,16 @@
 
     assert shared
     assert unpickled_cache.shared == shared
     # Test that the unpickled cache is still shared
     duration3 = (3.0,) if cache_cls == HybridCache else ()
     unpickled_cache.put("key3", "value3", *duration3)
     assert cache.get("key3") == "value3"
+
+
+def test_simple_cache():
+    cache = SimpleCache()
+    cache.put("key1", "value1")
+    assert "key1" in cache
+    assert "key2" not in cache
+    assert cache.get("key1") == "value1"
+    assert cache.get("key2") is None
```

### Comparing `pipefunc-0.5.0/tests/test_perf.py` & `pipefunc-0.6.0/tests/test_perf.py`

 * *Files identical despite different names*

### Comparing `pipefunc-0.5.0/tests/test_pipefunc.py` & `pipefunc-0.6.0/tests/test_pipefunc.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,21 +5,22 @@
 import inspect
 import pickle
 from typing import TYPE_CHECKING
 
 import pytest
 
 from pipefunc import (
+    PipeFunc,
     Pipeline,
-    PipelineFunction,
     Sweep,
     count_sweep,
     get_precalculation_order,
     pipefunc,
 )
+from pipefunc.exceptions import UnusedParametersError
 
 if TYPE_CHECKING:
     from pathlib import Path
 
 
 def test_pipeline_and_all_arg_combinations() -> None:
     @pipefunc(output_name="c")
@@ -41,24 +42,24 @@
     c = f1(a=2, b=3)
     assert fc(a=2, b=3) == c == fc(b=3, a=2) == 5
     assert fd(a=2, b=3) == f2(b=3, c=c) == fd(b=3, c=c) == 15
 
     fe = pipeline.func("e")
     assert fe(a=2, b=3, x=1) == fe(a=2, b=3, d=15, x=1) == f3(c=c, d=15, x=1) == 75
 
-    all_args = pipeline.all_arg_combinations()
+    all_args = pipeline.all_arg_combinations
     assert all_args == {
         "c": {("a", "b")},
         "d": {("a", "b", "x"), ("b", "c", "x")},
         "e": {("a", "b", "d", "x"), ("a", "b", "x"), ("b", "c", "x"), ("c", "d", "x")},
     }
-    assert pipeline.all_arg_combinations(root_args_only=True) == {
-        "c": {("a", "b")},
-        "d": {("a", "b", "x")},
-        "e": {("a", "b", "x")},
+    assert pipeline.all_root_args == {
+        "c": ("a", "b"),
+        "d": ("a", "b", "x"),
+        "e": ("a", "b", "x"),
     }
 
     kw = {"a": 2, "b": 3, "x": 1}
     kw["c"] = f1(a=kw["a"], b=kw["b"])
     kw["d"] = f2(b=kw["b"], c=kw["c"])
     kw["e"] = f3(c=kw["c"], d=kw["d"], x=kw["x"])
     for params in all_args["e"]:
@@ -91,34 +92,34 @@
     assert (
         fe(a=2, b=3, x=1).evaluate()
         == fe(a=2, b=3, d=15, x=1).evaluate()
         == f3(c=c, d=15, x=1)
         == 75
     )
 
-    all_args = pipeline.all_arg_combinations()
+    all_args = pipeline.all_arg_combinations
 
     kw = {"a": 2, "b": 3, "x": 1}
     kw["c"] = f1(a=kw["a"], b=kw["b"])
     kw["d"] = f2(b=kw["b"], c=kw["c"])
     kw["e"] = f3(c=kw["c"], d=kw["d"], x=kw["x"])
     for params in all_args["e"]:
         _kw = {k: kw[k] for k in params}
         assert fe(**_kw).evaluate() == kw["e"]
 
 
 @pytest.mark.parametrize(
     "f2",
     [
-        PipelineFunction(
+        PipeFunc(
             lambda b, c, x: b * c * x,
             output_name="d",
             renames={"x": "xx"},
         ),
-        PipelineFunction(lambda b, c, xx: b * c * xx, output_name="d"),
+        PipeFunc(lambda b, c, xx: b * c * xx, output_name="d"),
     ],
 )
 def test_pipeline_and_all_arg_combinations_rename(f2):
     @pipefunc(output_name="c")
     def f1(a, b):
         return a + b
 
@@ -132,36 +133,33 @@
     fd = pipeline.func("d")
     c = f1(a=2, b=3)
     assert fc(a=2, b=3) == c == fc(b=3, a=2) == 5
     assert fd(a=2, b=3, xx=1) == f2(b=3, c=c, xx=1) == fd(b=3, c=c, xx=1) == 15
 
     fe = pipeline.func("e")
     assert (
-        fe(a=2, b=3, x=1, xx=1)
-        == fe(a=2, b=3, d=15, x=1, xx=1)
-        == f3(c=c, d=15, x=1)
-        == 75
+        fe(a=2, b=3, x=1, xx=1) == fe(a=2, b=3, d=15, x=1) == f3(c=c, d=15, x=1) == 75
     )
 
-    all_args = pipeline.all_arg_combinations()
+    all_args = pipeline.all_arg_combinations
     assert all_args == {
         "c": {("a", "b")},
         "d": {("a", "b", "xx"), ("b", "c", "xx")},
         "e": {
             ("a", "b", "d", "x"),
             ("a", "b", "x", "xx"),
             ("b", "c", "x", "xx"),
             ("c", "d", "x"),
         },
     }
 
-    assert pipeline.all_arg_combinations(root_args_only=True) == {
-        "c": {("a", "b")},
-        "d": {("a", "b", "xx")},
-        "e": {("a", "b", "x", "xx")},
+    assert pipeline.all_root_args == {
+        "c": ("a", "b"),
+        "d": ("a", "b", "xx"),
+        "e": ("a", "b", "x", "xx"),
     }
 
 
 def test_disjoint_pipelines() -> None:
     @pipefunc(output_name="x")
     def f(a, b):
         return a + b
@@ -190,15 +188,17 @@
 
 
 def test_output_name_in_kwargs():
     @pipefunc(output_name="c")
     def f(a, b):
         return a + b
 
-    assert Pipeline([f])("a", a=1) == 1
+    p = Pipeline([f])
+    with pytest.raises(ValueError, match="cannot be provided in"):
+        assert p("a", a=1)
 
 
 def test_profiling():
     @pipefunc(output_name="c")
     def f(a, b):
         return a + b
 
@@ -211,27 +211,27 @@
     p.resources_report()
     for f in p.functions:
         f.set_profiling(enable=False)
     with pytest.raises(ValueError, match="Profiling is not enabled"):
         p.resources_report()
 
 
-def test_pipeline_function_and_execution():
+def test_pipe_func_and_execution():
     def func1(a, b=2):
         return a + b
 
     def func2(x):
         return 2 * x
 
     def func3(y, z=3):
         return y - z
 
-    pipe_func1 = PipelineFunction(func1, "out1", renames={"a": "a1"})
-    pipe_func2 = PipelineFunction(func2, "out2", renames={"x": "x2"})
-    pipe_func3 = PipelineFunction(func3, "out3", renames={"y": "y3", "z": "z3"})
+    pipe_func1 = PipeFunc(func1, "out1", renames={"a": "a1"})
+    pipe_func2 = PipeFunc(func2, "out2", renames={"x": "x2"})
+    pipe_func3 = PipeFunc(func3, "out3", renames={"y": "y3", "z": "z3"})
 
     pipeline = Pipeline([pipe_func1, pipe_func2, pipe_func3], debug=True, profile=True)
 
     # Create _Function instances
     function1 = pipeline.func("out1")
     function2 = pipeline.func("out2")
     function3 = pipeline.func("out3")
@@ -254,58 +254,58 @@
 
     # Test the pipeline object itself
     assert pipeline("out1", a1=3, b=2) == 5
     assert pipeline("out2", x2=4) == 8
     assert pipeline("out3", y3=9, z3=3) == 6
 
 
-def test_pipeline_function_profile():
+def test_pipe_func_profile():
     @pipefunc(output_name="c")
     def f1(a, b):
         return a + b
 
-    pipeline_function = PipelineFunction(f1, output_name="c", profile=True)
-    assert pipeline_function.profile
-    assert pipeline_function.profiling_stats is not None
-    pipeline_function.profile = False
-    assert not pipeline_function.profile
-    assert pipeline_function.profiling_stats is None
+    pipe_func = PipeFunc(f1, output_name="c", profile=True)
+    assert pipe_func.profile
+    assert pipe_func.profiling_stats is not None
+    pipe_func.profile = False
+    assert not pipe_func.profile
+    assert pipe_func.profiling_stats is None
 
 
-def test_pipeline_function_str():
+def test_pipe_func_str():
     @pipefunc(output_name="c")
     def f1(a, b):
         return a + b
 
-    pipeline_function = PipelineFunction(f1, output_name="c")
-    assert str(pipeline_function) == "f1(a, b) → c"
+    pipe_func = PipeFunc(f1, output_name="c")
+    assert str(pipe_func) == "f1(...) → c"
 
 
-def test_pipeline_function_getstate_setstate():
+def test_pipe_func_getstate_setstate():
     @pipefunc(output_name="c")
     def f1(a, b):
         return a + b
 
-    pipeline_function = PipelineFunction(f1, output_name="c")
-    state = pipeline_function.__getstate__()
+    pipe_func = PipeFunc(f1, output_name="c")
+    state = pipe_func.__getstate__()
 
     # We'll validate getstate by asserting that 'func' in the state
     # is a bytes object (dumped by cloudpickle) and other attributes
     # are as expected
     assert isinstance(state["func"], bytes)
     assert state["output_name"] == "c"
 
     # Now we'll test setstate by creating a new instance, applying setstate and
     # verifying that the object attributes match the original
-    new_pipeline_function = PipelineFunction.__new__(PipelineFunction)
-    new_pipeline_function.__setstate__(state)
+    new_pipe_func = PipeFunc.__new__(PipeFunc)
+    new_pipe_func.__setstate__(state)
 
-    assert new_pipeline_function.output_name == pipeline_function.output_name
-    assert new_pipeline_function.parameters == pipeline_function.parameters
-    assert new_pipeline_function.func(2, 3) == pipeline_function.func(
+    assert new_pipe_func.output_name == pipe_func.output_name
+    assert new_pipe_func.parameters == pipe_func.parameters
+    assert new_pipe_func.func(2, 3) == pipe_func.func(
         2,
         3,
     )  # the functions behave the same
 
 
 def test_complex_pipeline():
     def f1(a, b, c, d):
@@ -388,17 +388,17 @@
         lazy=True,
         cache_kwargs={"shared": False},
     )
     f = pipeline.func("i")
     r = f.call_full_output(a=1, b=2, x=3)["i"].evaluate()
     assert r == f(a=1, b=2, x=3).evaluate()
     assert (
-        pipeline.arg_combinations("g", root_args_only=True)
-        == pipeline.arg_combinations("h", root_args_only=True)
-        == pipeline.arg_combinations(("g", "h"), root_args_only=True)
+        pipeline.root_args("g")
+        == pipeline.root_args("h")
+        == pipeline.root_args(("g", "h"))
         == ("a", "b", "x")
     )
     key = (("d", "e"), (("a", 1), ("b", 2), ("x", 3)))
     assert pipeline.cache is not None
     assert pipeline.cache.cache[key].evaluate() == (6, 1)
     assert pipeline.func(("g", "h"))(a=1, b=2, x=3).evaluate().g == 4
     assert pipeline.func_dependencies("i") == [("c", "_throw"), ("d", "e"), ("g", "h")]
@@ -505,23 +505,23 @@
         "f3": 7,
     }
     if cache:
         assert len(list(cache_dir.glob("*.pkl"))) == 3
 
 
 def test_lazy_pipeline():
-    @pipefunc(output_name="c", cache=True)
+    @pipefunc(output_name="c")
     def f1(a, b):
         return a + b
 
-    @pipefunc(output_name="d", cache=True)
+    @pipefunc(output_name="d")
     def f2(b, c, x=1):
         return b * c * x
 
-    @pipefunc(output_name="e", cache=True)
+    @pipefunc(output_name="e")
     def f3(c, d, x=1):
         return c * d * x
 
     pipeline = Pipeline([f1, f2, f3], lazy=True)
 
     f = pipeline.func("e")
     r = f(a=1, b=2, x=3).evaluate()
@@ -558,7 +558,108 @@
 
     # Assert that the call_with_root_args method is recreated after unpickling
     assert unpickled_func.call_with_root_args is not None
     assert unpickled_func.call_with_root_args.__signature__.parameters.keys() == {
         "arg1",
         "arg2",
     }
+
+
+def test_drop_from_pipeline():
+    @pipefunc(output_name="c")
+    def f1(a, b):
+        return a + b
+
+    @pipefunc(output_name="d")
+    def f2(b, c, x=1):
+        return b * c * x
+
+    @pipefunc(output_name="e")
+    def f3(c, d, x=1):
+        return c * d * x
+
+    pipeline = Pipeline([f1, f2, f3])
+    assert "d" in pipeline.output_to_func
+    pipeline.drop(output_name="d")
+    assert "d" not in pipeline.output_to_func
+
+    pipeline = Pipeline([f1, f2, f3])
+    assert "d" in pipeline.output_to_func
+    pipeline.drop(f=f2)
+
+
+def test_used_variable():
+    @pipefunc(output_name="c")
+    def f1(a, b):
+        return a + b
+
+    pipeline = Pipeline([f1])
+    pipeline("c", a=1, b=2)
+    with pytest.raises(UnusedParametersError, match="Unused keyword arguments"):
+        pipeline("c", a=1, b=2, doesnotexist=3)
+
+    # Test regression with cache:
+    def f(a):
+        return a
+
+    pipeline = Pipeline([PipeFunc(f, output_name="c", cache=True)])
+    f = pipeline.func("c")
+    assert f(a=1) == 1
+    assert f(a=1) == 1  # should not raise an error
+
+
+def test_handle_error():
+    @pipefunc(output_name="c")
+    def f1(a, b):  # noqa: ARG001
+        msg = "Test error"
+        raise ValueError(msg)
+
+    pipeline = Pipeline([f1])
+    try:
+        pipeline("c", a=1, b=2)
+    except ValueError as e:
+        msg = "Error occurred while executing function `f1(a=1, b=2)`"
+        assert msg in str(e) or msg in str(e.__notes__)  # noqa: PT017
+        # NOTE: with pytest.raises match="..." does not work
+        # with add_note for some reason on my Mac, however,
+        # on CI it works fine (Linux)...
+
+
+def test_full_output_cache():
+    ran_f1 = False
+    ran_f2 = False
+
+    @pipefunc(output_name="c", cache=True)
+    def f1(a, b):
+        nonlocal ran_f1
+        if ran_f2:
+            raise RuntimeError
+        ran_f1 = True
+        return a + b
+
+    @pipefunc(output_name="d", cache=True)
+    def f2(b, c, x=1):
+        nonlocal ran_f2
+        if ran_f2:
+            raise RuntimeError
+        ran_f2 = True
+        return b * c * x
+
+    pipeline = Pipeline([f1, f2])
+    f = pipeline.func("d")
+    r = f.call_full_output(a=1, b=2, x=3)
+    expected = {"a": 1, "b": 2, "c": 3, "d": 18, "x": 3}
+    assert r == expected
+    assert len(pipeline.cache) == 2
+    r = f.call_full_output(a=1, b=2, x=3)
+    assert r == expected
+    r = f(a=1, b=2, x=3)
+    assert r == 18
+
+
+def test_output_picker_single_output():
+    @pipefunc(output_name=("y",), output_picker=dict.__getitem__)
+    def f(a, b):
+        return {"y": a + b, "_throw": 1}
+
+    pipeline = Pipeline([f])
+    assert pipeline("y", a=1, b=2) == 3
```

### Comparing `pipefunc-0.5.0/tests/test_simplify.py` & `pipefunc-0.6.0/tests/test_simplify.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 """Tests for pipefunc.py."""
 
 from __future__ import annotations
 
-from pipefunc import (
-    Pipeline,
-    pipefunc,
-)
+from pipefunc import Pipeline, pipefunc
 from pipefunc._simplify import _combine_nodes, _get_signature
 
 
 def test_identify_combinable_nodes():
     @pipefunc(output_name=("d", "e"))
     def f_d(b, g, x=1):  # noqa: ARG001
         pass
@@ -56,16 +53,16 @@
 
     @pipefunc(output_name="z")
     def f3(b, x, y):
         return x * y * b
 
     pipeline = Pipeline([f1, f2, f3], debug=True, profile=True)
 
-    root_args = pipeline.all_arg_combinations(root_args_only=True)
-    assert root_args == {"x": {("a",)}, "y": {("a", "b")}, "z": {("a", "b")}}
+    root_args = pipeline.all_root_args
+    assert root_args == {"x": ("a",), "y": ("a", "b"), "z": ("a", "b")}
 
     # Test with conservatively_combine=True
     combinable_nodes_true = pipeline._identify_combinable_nodes(
         "z",
         conservatively_combine=True,
     )
     assert combinable_nodes_true == {}
```

### Comparing `pipefunc-0.5.0/tests/test_sweep.py` & `pipefunc-0.6.0/tests/test_sweep.py`

 * *Files identical despite different names*

