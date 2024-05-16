# Comparing `tmp/alkymi-0.2.1.tar.gz` & `tmp/alkymi-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alkymi-0.2.1.tar", last modified: Thu Apr 27 10:26:18 2023, max compression
+gzip compressed data, was "alkymi-0.3.0.tar", last modified: Tue Apr 23 14:10:05 2024, max compression
```

## Comparing `alkymi-0.2.1.tar` & `alkymi-0.3.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 mathias   (1000) mathias   (1000)        0 2023-04-27 10:26:18.931690 alkymi-0.2.1/
--rw-rw-r--   0 mathias   (1000) mathias   (1000)     1066 2022-06-02 18:56:50.000000 alkymi-0.2.1/LICENSE.md
--rw-rw-r--   0 mathias   (1000) mathias   (1000)     6028 2023-04-27 10:26:18.931690 alkymi-0.2.1/PKG-INFO
--rw-rw-r--   0 mathias   (1000) mathias   (1000)     3818 2023-04-25 18:56:20.000000 alkymi-0.2.1/README.md
-drwxrwxr-x   0 mathias   (1000) mathias   (1000)        0 2023-04-27 10:26:18.931690 alkymi-0.2.1/alkymi/
--rw-rw-r--   0 mathias   (1000) mathias   (1000)      395 2023-03-07 20:55:52.000000 alkymi-0.2.1/alkymi/__init__.py
--rw-rw-r--   0 mathias   (1000) mathias   (1000)     6808 2023-03-26 09:01:00.000000 alkymi-0.2.1/alkymi/checksums.py
--rw-rw-r--   0 mathias   (1000) mathias   (1000)     4464 2023-04-11 02:15:19.000000 alkymi-0.2.1/alkymi/config.py
--rw-rw-r--   0 mathias   (1000) mathias   (1000)    22350 2023-04-27 10:26:15.000000 alkymi-0.2.1/alkymi/core.py
--rw-rw-r--   0 mathias   (1000) mathias   (1000)     4855 2023-03-26 08:25:39.000000 alkymi-0.2.1/alkymi/decorators.py
--rw-rw-r--   0 mathias   (1000) mathias   (1000)    12242 2023-04-11 02:15:19.000000 alkymi-0.2.1/alkymi/foreach_recipe.py
--rw-rw-r--   0 mathias   (1000) mathias   (1000)     9063 2023-04-25 18:56:20.000000 alkymi-0.2.1/alkymi/lab.py
--rw-rw-r--   0 mathias   (1000) mathias   (1000)      124 2022-02-10 21:09:03.000000 alkymi-0.2.1/alkymi/logging.py
--rw-rw-r--   0 mathias   (1000) mathias   (1000)     3781 2023-04-11 02:15:19.000000 alkymi-0.2.1/alkymi/progress.py
--rw-rw-r--   0 mathias   (1000) mathias   (1000)        0 2022-06-02 18:56:50.000000 alkymi-0.2.1/alkymi/py.typed
--rw-rw-r--   0 mathias   (1000) mathias   (1000)     9966 2023-04-11 02:15:19.000000 alkymi-0.2.1/alkymi/recipe.py
--rw-rw-r--   0 mathias   (1000) mathias   (1000)     6757 2022-06-02 18:56:50.000000 alkymi-0.2.1/alkymi/recipes.py
--rw-rw-r--   0 mathias   (1000) mathias   (1000)    13154 2023-04-25 18:56:20.000000 alkymi-0.2.1/alkymi/serialization.py
--rw-rw-r--   0 mathias   (1000) mathias   (1000)     1397 2023-04-25 18:56:20.000000 alkymi-0.2.1/alkymi/types.py
--rw-rw-r--   0 mathias   (1000) mathias   (1000)     3855 2023-04-27 10:26:15.000000 alkymi-0.2.1/alkymi/utils.py
--rw-rw-r--   0 mathias   (1000) mathias   (1000)      120 2023-04-27 10:26:15.000000 alkymi-0.2.1/alkymi/version.py
-drwxrwxr-x   0 mathias   (1000) mathias   (1000)        0 2023-04-27 10:26:18.931690 alkymi-0.2.1/alkymi.egg-info/
--rw-rw-r--   0 mathias   (1000) mathias   (1000)     6028 2023-04-27 10:26:18.000000 alkymi-0.2.1/alkymi.egg-info/PKG-INFO
--rw-rw-r--   0 mathias   (1000) mathias   (1000)      471 2023-04-27 10:26:18.000000 alkymi-0.2.1/alkymi.egg-info/SOURCES.txt
--rw-rw-r--   0 mathias   (1000) mathias   (1000)        1 2023-04-27 10:26:18.000000 alkymi-0.2.1/alkymi.egg-info/dependency_links.txt
--rw-rw-r--   0 mathias   (1000) mathias   (1000)       49 2023-04-27 10:26:18.000000 alkymi-0.2.1/alkymi.egg-info/requires.txt
--rw-rw-r--   0 mathias   (1000) mathias   (1000)        7 2023-04-27 10:26:18.000000 alkymi-0.2.1/alkymi.egg-info/top_level.txt
--rw-rw-r--   0 mathias   (1000) mathias   (1000)       38 2023-04-27 10:26:18.931690 alkymi-0.2.1/setup.cfg
--rw-rw-r--   0 mathias   (1000) mathias   (1000)     2077 2023-04-25 18:56:20.000000 alkymi-0.2.1/setup.py
+drwxrwxr-x   0 mathias   (1002) mathias   (1002)        0 2024-04-23 14:10:05.280389 alkymi-0.3.0/
+-rw-rw-r--   0 mathias   (1002) mathias   (1002)     1066 2023-07-16 18:29:23.000000 alkymi-0.3.0/LICENSE.md
+-rw-rw-r--   0 mathias   (1002) mathias   (1002)     5394 2024-04-23 14:10:05.280389 alkymi-0.3.0/PKG-INFO
+-rw-rw-r--   0 mathias   (1002) mathias   (1002)     3818 2023-07-16 18:29:23.000000 alkymi-0.3.0/README.md
+drwxrwxr-x   0 mathias   (1002) mathias   (1002)        0 2024-04-23 14:10:05.272389 alkymi-0.3.0/alkymi/
+-rw-rw-r--   0 mathias   (1002) mathias   (1002)      395 2023-07-16 18:29:23.000000 alkymi-0.3.0/alkymi/__init__.py
+-rw-rw-r--   0 mathias   (1002) mathias   (1002)     6808 2023-07-16 18:29:23.000000 alkymi-0.3.0/alkymi/checksums.py
+-rw-rw-r--   0 mathias   (1002) mathias   (1002)     4464 2023-07-16 18:29:23.000000 alkymi-0.3.0/alkymi/config.py
+-rw-rw-r--   0 mathias   (1002) mathias   (1002)    22449 2024-04-23 13:59:53.000000 alkymi-0.3.0/alkymi/core.py
+-rw-rw-r--   0 mathias   (1002) mathias   (1002)     6654 2024-04-23 13:59:53.000000 alkymi-0.3.0/alkymi/decorators.py
+-rw-rw-r--   0 mathias   (1002) mathias   (1002)    12313 2024-04-23 13:59:53.000000 alkymi-0.3.0/alkymi/foreach_recipe.py
+-rw-rw-r--   0 mathias   (1002) mathias   (1002)    12123 2024-04-23 13:59:53.000000 alkymi-0.3.0/alkymi/lab.py
+-rw-rw-r--   0 mathias   (1002) mathias   (1002)      124 2023-07-16 18:29:23.000000 alkymi-0.3.0/alkymi/logging.py
+-rw-rw-r--   0 mathias   (1002) mathias   (1002)     3787 2024-04-23 13:59:53.000000 alkymi-0.3.0/alkymi/progress.py
+-rw-rw-r--   0 mathias   (1002) mathias   (1002)        0 2023-07-16 18:29:23.000000 alkymi-0.3.0/alkymi/py.typed
+-rw-rw-r--   0 mathias   (1002) mathias   (1002)    10054 2024-04-23 13:59:53.000000 alkymi-0.3.0/alkymi/recipe.py
+-rw-rw-r--   0 mathias   (1002) mathias   (1002)     7307 2024-04-23 13:59:53.000000 alkymi-0.3.0/alkymi/recipes.py
+-rw-rw-r--   0 mathias   (1002) mathias   (1002)    13154 2023-07-16 18:29:23.000000 alkymi-0.3.0/alkymi/serialization.py
+-rw-rw-r--   0 mathias   (1002) mathias   (1002)     1397 2023-07-16 18:29:23.000000 alkymi-0.3.0/alkymi/types.py
+-rw-rw-r--   0 mathias   (1002) mathias   (1002)     5769 2024-04-23 13:59:53.000000 alkymi-0.3.0/alkymi/utils.py
+-rw-rw-r--   0 mathias   (1002) mathias   (1002)      120 2024-04-23 13:59:53.000000 alkymi-0.3.0/alkymi/version.py
+drwxrwxr-x   0 mathias   (1002) mathias   (1002)        0 2024-04-23 14:10:05.280389 alkymi-0.3.0/alkymi.egg-info/
+-rw-rw-r--   0 mathias   (1002) mathias   (1002)     5394 2024-04-23 14:10:05.000000 alkymi-0.3.0/alkymi.egg-info/PKG-INFO
+-rw-rw-r--   0 mathias   (1002) mathias   (1002)      471 2024-04-23 14:10:05.000000 alkymi-0.3.0/alkymi.egg-info/SOURCES.txt
+-rw-rw-r--   0 mathias   (1002) mathias   (1002)        1 2024-04-23 14:10:05.000000 alkymi-0.3.0/alkymi.egg-info/dependency_links.txt
+-rw-rw-r--   0 mathias   (1002) mathias   (1002)       49 2024-04-23 14:10:05.000000 alkymi-0.3.0/alkymi.egg-info/requires.txt
+-rw-rw-r--   0 mathias   (1002) mathias   (1002)        7 2024-04-23 14:10:05.000000 alkymi-0.3.0/alkymi.egg-info/top_level.txt
+-rw-rw-r--   0 mathias   (1002) mathias   (1002)       38 2024-04-23 14:10:05.280389 alkymi-0.3.0/setup.cfg
+-rw-rw-r--   0 mathias   (1002) mathias   (1002)     2077 2023-07-16 18:29:23.000000 alkymi-0.3.0/setup.py
```

### Comparing `alkymi-0.2.1/LICENSE.md` & `alkymi-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `alkymi-0.2.1/PKG-INFO` & `alkymi-0.3.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,100 +1,18 @@
 Metadata-Version: 2.1
 Name: alkymi
-Version: 0.2.1
+Version: 0.3.0
 Summary: alkymi - Pythonic task automation
 Home-page: https://github.com/MathiasStokholm/alkymi
 Author: Mathias Bøgh Stokholm
 Author-email: mathias.stokholm@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/MathiasStokholm/alkymi/
 Project-URL: Tracker, https://github.com/MathiasStokholm/alkymi/issues
 Project-URL: Documentation, https://alkymi.readthedocs.io/en/latest/
-Description: # alkymi ⚗️
-        
-        [![build](https://github.com/MathiasStokholm/alkymi/workflows/build/badge.svg?branch=master)](https://github.com/MathiasStokholm/alkymi/actions?query=workflow%3Abuild)
-        [![docs](https://readthedocs.org/projects/alkymi/badge/?version=latest)](https://alkymi.readthedocs.io/en/latest/?badge=latest)
-        [![coverage](https://codecov.io/gh/MathiasStokholm/alkymi/branch/develop/graph/badge.svg?token=L0DTW805NL)](https://codecov.io/gh/MathiasStokholm/alkymi)
-        [![pypi](https://img.shields.io/pypi/v/alkymi.svg)](https://pypi.org/project/alkymi)
-        [![versions](https://img.shields.io/pypi/pyversions/alkymi.svg)](https://pypi.org/project/alkymi)
-        
-        Alkymi is a pure Python (3.7+) library for describing and executing tasks and pipelines with built-in caching and
-        conditional evaluation based on checksums.
-        
-        Alkymi is easy to install, simple to use, and has very few dependencies outside of Python's standard library. The code
-        is cross-platform, and allows you to write your pipelines once and deploy to multiple operating systems (tested on
-        Linux, Windows and Mac).
-        
-        Documentation, including a quickstart guide, is provided [here](https://alkymi.readthedocs.io/en/latest/).
-        
-        ## Features
-        * Easily define complex data pipelines as decorated Python functions
-          * This allows you to run linting, type checking, etc. on your data pipelines
-        * Return values are automatically cached to disk, regardless of type
-        * Efficiently checks if pipeline is up-to-date
-          * Checks if external files have changed, bound functions have changed or if pipeline dependencies have changed
-        * No domain specific language (DSL) or CLI tool, just regular Python
-          * Supports caching and conditional evaluation in Jupyter Notebooks
-        * Cross-platform - works on Linux, Windows and Mac
-        * Expose recipes as a command-line interface (CLI) using alkymi's
-        [Lab](https://alkymi.readthedocs.io/en/latest/examples/command_line.html) type
-        
-        ## Sample Usage
-        For examples of how to use alkymi, see the
-        [quickstart guide](https://alkymi.readthedocs.io/en/latest/getting_started/quick_start.html).
-        
-        Example code:
-        ```python
-        import numpy as np
-        import alkymi as alk
-        
-        @alk.recipe()
-        def long_running_task() -> np.ndarray:
-            # Perform expensive computation here ...
-            hard_to_compute_result = np.array([42])
-            # Return value will be automatically cached to disk
-            return hard_to_compute_result
-        
-        result = long_running_task.brew()  # == np.ndarray([42])
-        ```
-        
-        Or one of the examples, e.g. [MNIST](https://alkymi.readthedocs.io/en/latest/examples/mnist.html).
-        
-        ## Installation
-        Install via pip:
-        ```shell script
-        pip install --user alkymi
-        ```
-        
-        Or see the [Installation page](https://alkymi.readthedocs.io/en/latest/getting_started/installation.html).
-        
-        ### Testing
-        After installing, you can run the test suite (use the `lint`, `coverage` and `type_check` recipes to perform those
-        actions):
-        ```shell script
-        python3 labfile.py brew test
-        ```
-        
-        ## License
-        alkymi is licensed under The MIT License as found in the LICENSE.md file
-        
-        ## Upcoming Features
-        The following features are being considered for future implementation:
-        * Type annotations propagated from bound functions to recipes
-        * Support for call/type checking all recipes (e.g. by adding a `check` command to `Lab`)
-        * Cache maintenance functionality
-        
-        ## Known Issues
-        * alkymi currently doesn't check custom objects for altered external files when computing cleanliness (e.g. `MyClass`
-        has a `self._some_path` that points to a file somewhere outside alkymi's internal cache)
-        * `alk.foreach()` currently only supports enumerable inputs of type `List` or `Dict`
-        * Recipes marked `transient` will always be dirty, and thus always require reevaluation. This functionality should be
-        replaced by a proper means of creating recipes that don't cache outputs, but only run when needed to provide inputs for
-        downstream recipes
-        
 Keywords: automation,pipeline,validation,preprocessing,make,build,task
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -111,7 +29,92 @@
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: xxhash
+License-File: LICENSE.md
+
+# alkymi ⚗️
+
+[![build](https://github.com/MathiasStokholm/alkymi/workflows/build/badge.svg?branch=master)](https://github.com/MathiasStokholm/alkymi/actions?query=workflow%3Abuild)
+[![docs](https://readthedocs.org/projects/alkymi/badge/?version=latest)](https://alkymi.readthedocs.io/en/latest/?badge=latest)
+[![coverage](https://codecov.io/gh/MathiasStokholm/alkymi/branch/develop/graph/badge.svg?token=L0DTW805NL)](https://codecov.io/gh/MathiasStokholm/alkymi)
+[![pypi](https://img.shields.io/pypi/v/alkymi.svg)](https://pypi.org/project/alkymi)
+[![versions](https://img.shields.io/pypi/pyversions/alkymi.svg)](https://pypi.org/project/alkymi)
+
+Alkymi is a pure Python (3.7+) library for describing and executing tasks and pipelines with built-in caching and
+conditional evaluation based on checksums.
+
+Alkymi is easy to install, simple to use, and has very few dependencies outside of Python's standard library. The code
+is cross-platform, and allows you to write your pipelines once and deploy to multiple operating systems (tested on
+Linux, Windows and Mac).
+
+Documentation, including a quickstart guide, is provided [here](https://alkymi.readthedocs.io/en/latest/).
+
+## Features
+* Easily define complex data pipelines as decorated Python functions
+  * This allows you to run linting, type checking, etc. on your data pipelines
+* Return values are automatically cached to disk, regardless of type
+* Efficiently checks if pipeline is up-to-date
+  * Checks if external files have changed, bound functions have changed or if pipeline dependencies have changed
+* No domain specific language (DSL) or CLI tool, just regular Python
+  * Supports caching and conditional evaluation in Jupyter Notebooks
+* Cross-platform - works on Linux, Windows and Mac
+* Expose recipes as a command-line interface (CLI) using alkymi's
+[Lab](https://alkymi.readthedocs.io/en/latest/examples/command_line.html) type
+
+## Sample Usage
+For examples of how to use alkymi, see the
+[quickstart guide](https://alkymi.readthedocs.io/en/latest/getting_started/quick_start.html).
+
+Example code:
+```python
+import numpy as np
+import alkymi as alk
+
+@alk.recipe()
+def long_running_task() -> np.ndarray:
+    # Perform expensive computation here ...
+    hard_to_compute_result = np.array([42])
+    # Return value will be automatically cached to disk
+    return hard_to_compute_result
+
+result = long_running_task.brew()  # == np.ndarray([42])
+```
+
+Or one of the examples, e.g. [MNIST](https://alkymi.readthedocs.io/en/latest/examples/mnist.html).
+
+## Installation
+Install via pip:
+```shell script
+pip install --user alkymi
+```
+
+Or see the [Installation page](https://alkymi.readthedocs.io/en/latest/getting_started/installation.html).
+
+### Testing
+After installing, you can run the test suite (use the `lint`, `coverage` and `type_check` recipes to perform those
+actions):
+```shell script
+python3 labfile.py brew test
+```
+
+## License
+alkymi is licensed under The MIT License as found in the LICENSE.md file
+
+## Upcoming Features
+The following features are being considered for future implementation:
+* Type annotations propagated from bound functions to recipes
+* Support for call/type checking all recipes (e.g. by adding a `check` command to `Lab`)
+* Cache maintenance functionality
+
+## Known Issues
+* alkymi currently doesn't check custom objects for altered external files when computing cleanliness (e.g. `MyClass`
+has a `self._some_path` that points to a file somewhere outside alkymi's internal cache)
+* `alk.foreach()` currently only supports enumerable inputs of type `List` or `Dict`
+* Recipes marked `transient` will always be dirty, and thus always require reevaluation. This functionality should be
+replaced by a proper means of creating recipes that don't cache outputs, but only run when needed to provide inputs for
+downstream recipes
+
+
```

### Comparing `alkymi-0.2.1/README.md` & `alkymi-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `alkymi-0.2.1/alkymi/checksums.py` & `alkymi-0.3.0/alkymi/checksums.py`

 * *Files identical despite different names*

### Comparing `alkymi-0.2.1/alkymi/config.py` & `alkymi-0.3.0/alkymi/config.py`

 * *Files identical despite different names*

### Comparing `alkymi-0.2.1/alkymi/core.py` & `alkymi-0.3.0/alkymi/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 OutputsAndChecksums = Tuple[R, Optional[str]]
 
 
 def create_graph(recipe: Recipe[R]) -> nx.DiGraph:
     """
     Create a Directed Acyclic Graph (DAG) based on the provided recipe
-    Each node in the graph represents a recipe, and has an associated "status" attribute
+    Each node in the graph represents a recipe
 
     :param recipe: The recipe to construct a graph for
     :return: The constructed graph
     """
     log.debug(f'Building graph for {recipe.name}')
     graph = nx.DiGraph()
     _add_recipe_to_graph(recipe, graph)
@@ -382,19 +382,22 @@
 
     # Return the output and checksum of the final recipe
     if progress is not None:
         progress.start()
 
     # Check if the event loop is already running - if this is the case, execution must be pushed to a new thread to
     # avoid crashing due to the already running event loop
-    output, checksum = utils.run_on_thread(_setup_and_execute) if utils.check_current_thread_has_running_event_loop() \
-        else _setup_and_execute()
+    try:
+        output, checksum = utils.run_on_thread(
+            _setup_and_execute)() if utils.check_current_thread_has_running_event_loop() else _setup_and_execute()
+    finally:
+        # Ensure that the progress is always stopped (to return the cursor correctly to the terminal)
+        if progress is not None:
+            progress.stop()
 
-    if progress is not None:
-        progress.stop()
     return output, checksum
 
 
 def is_clean(recipe: Recipe[R], new_input_checksums: Tuple[Optional[str], ...]) -> Status:
     """
     Check whether a Recipe is clean (result is cached) based on a set of (potentially new) input checksums
```

### Comparing `alkymi-0.2.1/alkymi/decorators.py` & `alkymi-0.3.0/alkymi/decorators.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,24 +4,59 @@
 from .config import CacheType
 from .foreach_recipe import ForeachRecipe
 from .recipe import Recipe
 
 R = TypeVar("R")  # The return type of the bound function
 
 
-def recipe(ingredients=(), name: Optional[str] = None, transient: bool = False, cache: CacheType = CacheType.Auto) -> \
-        Callable[[Callable[..., R]], Recipe[R]]:
+def _parse_docstring_from_func(func: Callable) -> str:
+    """
+    Attempt to parse a useful recipe docstring from a bound function
+
+    :param func: The function to parse the docstring from
+    :return: The parsed docstring, or an empty string of no valid docstring could be found
+    """
+    # Try to read the docstring of the function itself
+    maybe_doc = inspect.getdoc(func)
+    if not maybe_doc:
+        # Try to read a leading comment (e.g. for a lambda)
+        maybe_doc = inspect.getcomments(func)
+        if not maybe_doc:
+            # Give up and return an empty string
+            return ""
+        else:
+            # Comment string contains something - remove any leading comment signs and ending newlines
+            maybe_doc = maybe_doc.lstrip("#").strip()
+
+    # If only one line exists, just return that
+    num_lines = len(maybe_doc.splitlines())
+    if num_lines == 1:
+        return maybe_doc
+
+    # Attempt to find the first double line return (signalling the end of a possibly multi-line function description)
+    double_line_splits = maybe_doc.split("\n\n")
+    if len(double_line_splits) == 1:
+        # No double line return found, fall back to first line
+        return maybe_doc.splitlines()[0]
+
+    # Convert possible multi-line to a single string
+    return double_line_splits[0].replace("\n", " ")
+
+
+def recipe(ingredients=(), name: Optional[str] = None, transient: bool = False, doc: Optional[str] = None,
+           cache: CacheType = CacheType.Auto) -> Callable[[Callable[..., R]], Recipe[R]]:
     """
     Convert a function into an alkymi Recipe to enable caching and conditional evaluation
 
     :param ingredients: The dependencies of this Recipe - the outputs of these Recipes will be provided as arguments to
                         the bound function when called in the order that they were provided. If not all arguments are
                         provided directly, alkymi will look up recipes that match the name of arguments automatically
     :param name: The name to assign to the created recipe - if not provided, the bound function's name will be used
     :param transient: Whether to always (re)evaluate the created Recipe
+    :param doc: Documentation string for this recipe - if not provided, the bound function docstring will be used
     :param cache: The type of caching to use for this Recipe
     :return: A callable that will yield the Recipe created from the bound function
     """
     ingredients = list(ingredients)
     num_provided_ingredients = len(ingredients)
 
     # Capture locals of calling scope to allow lookup of dependent Recipes in decorator
@@ -41,32 +76,34 @@
             if arg is None:
                 raise RuntimeError("Unable to find Recipe with name {} in enclosing scope".format(arg_name))
             if not isinstance(arg, Recipe):
                 raise RuntimeError("Found argument with name {}, but not a Recipe".format(arg_name))
             ingredients.append(arg)
 
         recipe_name = func.__name__ if name is None else name
-        return Recipe(func, ingredients, recipe_name, transient, cache)
+        parsed_doc = _parse_docstring_from_func(func) if doc is None else doc
+        return Recipe(func, ingredients, recipe_name, transient, parsed_doc, cache)
 
     return _decorator
 
 
 def foreach(mapped_inputs: Recipe, ingredients=(), name: Optional[str] = None, transient: bool = False,
-            cache: CacheType = CacheType.Auto) -> \
+            doc: Optional[str] = None, cache: CacheType = CacheType.Auto) -> \
         Callable[[Callable[..., R]], ForeachRecipe[R]]:
     """
     Convert a function into an alkymi Recipe to enable caching and conditional evaluation
 
     :param mapped_inputs: A single Recipe to whose output (a list or dictionary) the bound function will be applied to
                           generate the new outputs (similar to Python's built-in map() function)
     :param ingredients: The dependencies of this Recipe - the outputs of these Recipes will be provided as arguments to
                         the bound function when called in the order that they were provided. If not all arguments are
                         provided directly, alkymi will look up recipes that match the name of arguments automatically
     :param name: The name to assign to the created recipe - if not provided, the bound function's name will be used
     :param transient: Whether to always (re)evaluate the created Recipe
+    :param doc: Documentation string for this recipe - if not provided, the bound function docstring will be used
     :param cache: The type of caching to use for this Recipe
     :return: A callable that will yield the Recipe created from the bound function
     """
     ingredients = list(ingredients)
     num_provided_ingredients = len(ingredients)
 
     # Capture locals of calling scope to allow lookup of dependent Recipes in decorator
@@ -86,10 +123,11 @@
             if arg is None:
                 raise RuntimeError("Unable to find Recipe with name {} in enclosing scope".format(arg_name))
             if not isinstance(arg, Recipe):
                 raise RuntimeError("Found argument with name {}, but not a Recipe".format(arg_name))
             ingredients.append(arg)
 
         recipe_name = func.__name__ if name is None else name
-        return ForeachRecipe(mapped_inputs, ingredients, func, recipe_name, transient, cache)
+        parsed_doc = _parse_docstring_from_func(func) if doc is None else doc
+        return ForeachRecipe(mapped_inputs, ingredients, func, recipe_name, transient, parsed_doc, cache)
 
     return _decorator
```

### Comparing `alkymi-0.2.1/alkymi/foreach_recipe.py` & `alkymi-0.3.0/alkymi/foreach_recipe.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,35 +20,36 @@
     Special type of Recipe that applies its bound function to each input from a list or dictionary (similar to Python's
     built-in map() function). Evaluations of the bound function are cached and used to avoid reevaluation previously
     seen inputs, this means that changing the inputs to a ForeachRecipe may only trigger reevaluation of the bound
     function for some inputs, avoiding the overhead of recomputing things
     """
 
     def __init__(self, mapped_recipe: Recipe, ingredients: Iterable[Recipe], func: Callable[..., R], name: str,
-                 transient: bool, cache: CacheType, cleanliness_func: Optional[CleanlinessFunc] = None):
+                 transient: bool, doc: str, cache: CacheType, cleanliness_func: Optional[CleanlinessFunc] = None):
         """
         Create a new ForeachRecipe
 
         :param mapped_recipe: A single Recipe to whose output (a list or dictionary) the bound function will be applied
                               to generate the new outputs (similar to Python's built-in map() function)
         :param ingredients: The dependencies of this Recipe - the outputs of these Recipes will be provided as arguments
                             to the bound function when called (following the item from the mapped_inputs sequence)
         :param func: The function to bind to this recipe
         :param name: The name of this Recipe
         :param transient: Whether to always (re)evaluate the created Recipe
+        :param doc: Documentation string for this recipe
         :param cache: The type of caching to use for this Recipe
         :param cleanliness_func: A function to allow a custom cleanliness check
         """
         self._mapped_inputs: Optional[MappedInputs] = None
         self._mapped_inputs_type: Optional[type] = None
         self._mapped_inputs_checksums: Optional[MappedInputsChecksums] = None
         self._mapped_inputs_checksum: Optional[str] = None
         self._mapped_outputs: Optional[MappedOutputs] = None
         self._mapped_outputs_checksum: Optional[str] = None
-        super().__init__(func, chain([mapped_recipe], ingredients), name, transient, cache, cleanliness_func)
+        super().__init__(func, chain([mapped_recipe], ingredients), name, transient, doc, cache, cleanliness_func)
 
     @property
     def mapped_inputs_type(self) -> Optional[type]:
         return self._mapped_inputs_type
 
     @property
     def mapped_inputs_checksums(self) -> Optional[MappedInputsChecksums]:
@@ -214,15 +215,14 @@
             output_checksum=self.output_checksum,
             last_function_hash=self._last_function_hash,
             mapped_inputs_checksums=self.mapped_inputs_checksums,
             mapped_inputs_checksum=self.mapped_inputs_checksum,
             mapped_type="dict" if self.mapped_inputs_type == dict else "list"
         )
 
-
     def restore_from_dict(self, old_state: Dict) -> None:
         """
         Restores the state of this ForeachRecipe from a previously cached state
 
         :param old_state: The old cached state to restore
         """
         log.debug("Restoring {} from dict".format(self._name))
```

### Comparing `alkymi-0.2.1/alkymi/lab.py` & `alkymi-0.3.0/alkymi/lab.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import argparse
 import logging
 import sys
+import traceback
 from typing import Dict, Union, Any, List, Optional
 from typing import Iterable, TextIO
 
 from rich import console
+from rich.control import Control
 
 from .core import Status, compute_recipe_status, create_graph
 from .logging import log
 from .recipe import Recipe
 from .recipes import Arg
 from .types import ProgressType
 
@@ -72,16 +74,23 @@
         """
 
         # Helper function to call brew on the matched recipe with CTRL-C handling
         def _call_brew(_recipe: Recipe) -> Any:
             try:
                 return _recipe.brew(jobs=jobs, progress_type=progress_type)
             except KeyboardInterrupt:
-                self._console.print("[bold red]Interrupted by user")
+                # Signal that execution was interrupted by the user and return cursor to normal state
+                self._console.print("\n[bold red]Interrupted by user")
+                self._console.control(Control.show_cursor(True))
                 sys.exit(1)
+            except Exception as e:  # noqa: Catch-all to fix traceback
+                # Omit the '_call_brew' stack frame, this exception handler stack frame and the
+                # '_remove_alkymi_internals_from_traceback' call from traceback
+                sys.stderr.write(Lab._remove_alkymi_internals_from_traceback(e, num_stack_frames_to_omit=3))
+                sys.exit(2)
 
         if isinstance(target_recipe, str):
             # Try to match name
             for recipe in self._recipes:
                 if recipe.name == target_recipe:
                     return _call_brew(recipe)
             raise ValueError("Unknown recipe: {}".format(target_recipe))
@@ -120,27 +129,64 @@
         """
         status: Dict[Recipe, Status] = {}
         for recipe in self._recipes:
             graph = create_graph(recipe)
             status.update(compute_recipe_status(recipe, graph))
         return status
 
-    def _add_user_args_(self, parser: argparse.ArgumentParser) -> None:
+    def _add_user_args_(self, parser: argparse.ArgumentParser, args: Dict[str, Arg]) -> None:
         """
         Adds user provided arguments to an ArgumentParser instance
 
         :param parser: The parser to add the user-provided arguments to
+        :param args: The arguments to add
         """
-        for arg_name, arg in self._args.items():
+        for arg_name, arg in args.items():
             # For iterables (e.g. lists), the "type" keyword is actually the type of elements in the iterable
             if issubclass(arg.type, Iterable) and not arg.type == str:
                 subtype = arg.subtype if arg.subtype is not None else str
-                parser.add_argument("--{}".format(arg_name), type=subtype, nargs="*", dest=arg_name)
+                parser.add_argument("--{}".format(arg_name), type=subtype, nargs="*", dest=arg_name, help=arg.doc)
             else:
-                parser.add_argument("--{}".format(arg_name), type=arg.type, dest=arg_name)
+                parser.add_argument("--{}".format(arg_name), type=arg.type, dest=arg_name, help=arg.doc)
+
+    @staticmethod
+    def _remove_alkymi_internals_from_traceback(e: Exception, num_stack_frames_to_omit: int) -> str:
+        """
+
+
+        :param e: The exception to load the traceback from
+        :param num_stack_frames_to_omit: A number of stack frames to omit - can be used to e.g. ignore this call on the
+                                         stack
+        :return: A string representing the created traceback without alkymi internals
+        """
+
+        # Search from the beginning until the first item containing Recipe.__call__
+        # This denotes the first time alkymi has handed over control to user code
+        frames = traceback.extract_tb(e.__traceback__)
+        idx = 0
+        for i, frame in enumerate(frames):
+            if frame.name == "__call__" and "alkymi/recipe.py" in frame.filename:
+                idx = i + 1
+                break
+        filtered_frames = frames[idx:]
+
+        # Next, find the call stack up to the beginning of the traceback frame
+        stack = traceback.StackSummary.extract(traceback.walk_stack(None))
+
+        # Remove the most recent frames if requested
+        if num_stack_frames_to_omit > 0:
+            del stack[0:num_stack_frames_to_omit]
+
+        # Reverse stack to get the expected output order
+        stack.reverse()
+
+        # Finally, combine the stack with an "omitted" statement and the filtered traceback
+        return "".join(stack.format()) + \
+            "    <alkymi internals omitted...>\n" + \
+            "".join(traceback.StackSummary.from_list(filtered_frames).format())
 
     def __repr__(self) -> str:
         """
         :return: A string representation of this Lab with recipes and their statuses
         """
         status = self._build_full_status()
         state = ''
@@ -182,29 +228,39 @@
         if args is None:
             args = sys.argv[1:]
 
         # Create the top-level parser
         parser = argparse.ArgumentParser('CLI for {}'.format(self._name))
         parser.add_argument("-v", "--verbose", action="store_true", help="Turn on verbose logging")
 
-        subparsers = parser.add_subparsers(help='sub-command help', dest='subparser_name')
+        subparsers = parser.add_subparsers(dest='subparser_name', metavar="")
 
         # Create the parser for the "status" command
-        status_parser = subparsers.add_parser('status', help='Prints the detailed status of the lab')
-        self._add_user_args_(status_parser)
+        status_parser = subparsers.add_parser('status', help='Prints the detailed status of the lab',
+                                              formatter_class=argparse.MetavarTypeHelpFormatter)
+        self._add_user_args_(status_parser, self._args)
 
-        # Create the parser for the "brew" command
+        # Create the parser for the "brew" command along with brew-specific arguments
         brew_parser = subparsers.add_parser('brew', help='Brew the selected recipe')
-        brew_parser.add_argument('recipe', choices=[recipe.name for recipe in self._recipes], nargs="+",
-                                 help='Recipe(s) to brew')
-        brew_parser.add_argument("-j", "--jobs", type=int, default=1,
+        brew_parser.add_argument("-j", "--jobs", type=int, default=1, metavar="N",
                                  help="Use N jobs to evaluate the recipe, more than 1 job will parallelize evaluation")
         brew_parser.add_argument("--progress", type=ProgressType, default=ProgressType.Fancy,
                                  choices=list(ProgressType), help="The type of progress indication to use")
-        self._add_user_args_(brew_parser)
+        brew_subparsers = brew_parser.add_subparsers(metavar="")
+
+        # Create a parser (command) for each recipe that can be brewed
+        for recipe in self._recipes:
+            recipe_parser = brew_subparsers.add_parser(recipe.name, help=recipe.doc, description=recipe.doc,
+                                                       formatter_class=argparse.MetavarTypeHelpFormatter)
+            recipe_parser.set_defaults(recipe=recipe.name)
+
+            # Use graph to only expose args that are connected to this recipe
+            graph = create_graph(recipe)
+            applicable_args = {arg_name: arg for arg_name, arg in self._args.items() if arg in graph}
+            self._add_user_args_(recipe_parser, applicable_args)
 
         parsed_args = parser.parse_args(args)
         log.addHandler(logging.StreamHandler(stream))
         if parsed_args.verbose:
             log.setLevel(logging.DEBUG)
         else:
             log.setLevel(logging.INFO)
@@ -218,12 +274,15 @@
             provided_val = getattr(parsed_args, arg_name, None)
             if provided_val is not None:
                 arg.set(provided_val)
 
         if parsed_args.subparser_name == 'status':
             self.print_status()
         elif parsed_args.subparser_name == 'brew':
-            for recipe in parsed_args.recipe:
-                self.brew(recipe, jobs=parsed_args.jobs, progress_type=parsed_args.progress)
+            # If not recipe was provided to brew, just print help
+            if "recipe" not in parsed_args:
+                brew_parser.print_help()
+                return
+            self.brew(parsed_args.recipe, jobs=parsed_args.jobs, progress_type=parsed_args.progress)
         else:
             # No recognized command provided - print help
             parser.print_help(file=stream)
```

### Comparing `alkymi-0.2.1/alkymi/progress.py` & `alkymi-0.3.0/alkymi/progress.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         """
         self._console = rich.console.Console() if console is None else console
         self._recipe_name = target_recipe.name
 
         # Define the columns to use for progress table
         super().__init__(TextColumn("[deep_sky_blue2]{task.description}"),
                          BarColumn(),
-                         TextColumn("{task.completed}/{task.total} ({task.percentage}%)"),
+                         TextColumn("{task.completed}/{task.total} ({task.percentage:>3.0f}%)"),
                          TextColumn("•"),
                          TimeElapsedColumn(),
                          console=self._console, redirect_stdout=True, redirect_stderr=True)
 
         # Build the progress table by adding all required tasks sorted topographically (target recipe at the bottom)
         self._recipe_tasks: Dict[Recipe, TaskID] = {
             recipe: self.add_task(recipe.name, start=False, total=1, completed=0)
```

### Comparing `alkymi-0.2.1/alkymi/recipe.py` & `alkymi-0.3.0/alkymi/recipe.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,31 +20,33 @@
     it then calls when asked to by alkymi's execution engine. The result of the bound function evaluation can be
     automatically cached to disk to allow for checking of cleanliness (whether a Recipe is up-to-date), and to avoid
     invoking the bound function if necessary on subsequent evaluations
     """
 
     CACHE_DIRECTORY_NAME = ".alkymi_cache"
 
-    def __init__(self, func: Callable[..., R], ingredients: Iterable['Recipe'], name: str, transient: bool,
+    def __init__(self, func: Callable[..., R], ingredients: Iterable['Recipe'], name: str, transient: bool, doc: str,
                  cache: CacheType, cleanliness_func: Optional[CleanlinessFunc[R]] = None):
         """
         Create a new Recipe
 
         :param ingredients: The dependencies of this Recipe - the outputs of these Recipes will be provided as arguments
                             to the bound function when called (following the item from the mapped_inputs sequence)
         :param func: The function to bind to this recipe
         :param name: The name of this Recipe
         :param transient: Whether to always (re)evaluate the created Recipe
+        :param doc: Documentation string for this recipe
         :param cache: The type of caching to use for this Recipe
         :param cleanliness_func: A function to allow a custom cleanliness check
         """
         self._func = func
         self._ingredients = list(ingredients)
         self._name = name
         self._transient = transient
+        self._doc = doc
         self._cleanliness_func = cleanliness_func
 
         # Set cache type based on default value (in AlkymiConfig)
         if cache == CacheType.Auto:
             # Pick based on what is in the config
             self._cache = CacheType.Cache if AlkymiConfig.get().cache else CacheType.NoCache
         else:
@@ -165,14 +167,21 @@
     def transient(self) -> bool:
         """
         :return: Whether to always (re)evaluate the created Recipe
         """
         return self._transient
 
     @property
+    def doc(self) -> str:
+        """
+        :return: The documentation string for this recipe
+        """
+        return self._doc
+
+    @property
     def cache(self) -> CacheType:
         """
         :return: The type of caching to use for this Recipe
         """
         return self._cache
 
     @property
@@ -242,15 +251,13 @@
     def restore_from_dict(self, old_state) -> None:
         """
         Restores the state of this Recipe from a previously cached state
 
         :param old_state: The old cached state to restore
         """
         log.debug("Restoring {} from dict".format(self._name))
-        if old_state["input_checksums"] is not None:
-            self._input_checksums = tuple(old_state["input_checksums"])
-        if old_state["outputs"] is not None and old_state["output_checksum"] is not None:
-            self._outputs = CachedOutput(None, old_state["output_checksum"], old_state["outputs"])
+        self._input_checksums = tuple(old_state["input_checksums"])
+        self._outputs = CachedOutput(None, old_state["output_checksum"], old_state["outputs"])
         self._last_function_hash = cast(str, old_state["last_function_hash"])
 
     def __repr__(self) -> str:
         return self.name
```

### Comparing `alkymi-0.2.1/alkymi/recipes.py` & `alkymi-0.3.0/alkymi/recipes.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,16 @@
         :param last_outputs: The last set of outputs created by this Recipe
         :return: True if clean
         """
         if last_outputs is None:
             return False
         return _glob_recipe() == last_outputs
 
-    return Recipe(_glob_recipe, [], name, transient=False, cache=cache, cleanliness_func=_check_clean)
+    doc = f"Find and return files in {directory} with pattern '{pattern}'" + (" recursively" if recursive else "")
+    return Recipe(_glob_recipe, [], name, transient=False, doc=doc, cache=cache, cleanliness_func=_check_clean)
 
 
 def file(name: str, path: Path, cache=CacheType.Auto) -> Recipe[Path]:
     """
     Create a Recipe that outputs a single file
 
     :param name: The name to give the created Recipe
@@ -54,15 +55,16 @@
     """
     # Reference the path as a string to avoid changes to the Path object to change the checksum of the function
     path_as_str = str(path)
 
     def _file_recipe() -> Path:
         return Path(path_as_str)
 
-    return Recipe(_file_recipe, [], name, transient=False, cache=cache)
+    doc = f"Return {path}"
+    return Recipe(_file_recipe, [], name, transient=False, doc=doc, cache=cache)
 
 
 def zip_results(name: str, recipes: Iterable[Recipe], cache=CacheType.Auto) \
         -> Recipe[Union[List[Tuple[Any, ...]], Dict[Any, Tuple[Any, ...]]]]:
     """
     Create a Recipe that zips the outputs from a number of recipes into elements, similar to Python's built-in zip().
     Notably, dictionaries are handled a bit differently, in that a dictionary is returned with keys mapping to tuples
@@ -100,41 +102,45 @@
             return {
                 key: tuple(iterable[key] for iterable in iterables)
                 for key in first_iterable.keys()
             }
         else:
             raise ValueError("Type: {} not supported in _zip_results()".format(type(first_iterable)))
 
-    return Recipe(_zip_results, recipes, name, transient=False, cache=cache)
+    doc = f"Zip together results from {[r.name for r in recipes]}"
+    return Recipe(_zip_results, recipes, name, transient=False, doc=doc, cache=cache)
 
 
 T = TypeVar('T')
 
 
 class Arg(Recipe[T]):
     """
     Class providing a stateful argument
 
     To use, create an Arg instance with the initial value for your argument, e.g. ``Arg(0)``, then provide as a
     recipe to downstream recipes. To change the input arguments, call ``set()`` again - this will mark the recipe as
     dirty and cause reevaluation of downstream recipe(s)
     """
 
-    def __init__(self, arg: T, name: str, cache=CacheType.Auto):
+    def __init__(self, arg: T, name: str, doc: str, cache=CacheType.Auto):
         """
         Create a new Arg instance with initial argument value
 
         :param arg: The initial argument value
         :param name: The name to give the created Recipe
+        :param doc: Documentation string for this argument - will be used in alkymi's Lab command line interface
         :param cache: The type of caching to use for this Recipe
         """
         self._arg = arg
         self._type = type(arg)
         self._subtype = next((type(val) for val in arg), None) if isinstance(arg, Iterable) else None
-        super().__init__(self._produce_arg, [], name, transient=False, cache=cache, cleanliness_func=self._clean)
+        self._doc = doc
+        super().__init__(self._produce_arg, [], name, transient=False, doc=doc, cache=cache,
+                         cleanliness_func=self._clean)
 
     @property
     def type(self) -> Type[T]:
         """
         :return: The type of the argument
         """
         return self._type
@@ -169,17 +175,18 @@
         :param _arg: The new argument
         """
         if not isinstance(_arg, self._type):
             raise TypeError("Type of argument ({}) not {}".format(type(_arg), self._type))
         self._arg = _arg
 
 
-def arg(_arg: T, name: str, cache=CacheType.Auto) -> Arg[T]:
+def arg(_arg: T, name: str, doc: str = "", cache=CacheType.Auto) -> Arg[T]:
     """
     Shorthand for creating an ``Arg`` instance
 
     :param _arg: The initial argument to use
     :param name: The name to give the created Recipe
+    :param doc: Documentation string for this argument - will be used in alkymi's Lab command line interface
     :param cache: The type of caching to use for this Recipe
     :return: The created ``Arg`` instance
     """
-    return Arg(_arg, name=name, cache=cache)
+    return Arg(_arg, name=name, doc=doc, cache=cache)
```

### Comparing `alkymi-0.2.1/alkymi/serialization.py` & `alkymi-0.3.0/alkymi/serialization.py`

 * *Files identical despite different names*

### Comparing `alkymi-0.2.1/alkymi/types.py` & `alkymi-0.3.0/alkymi/types.py`

 * *Files identical despite different names*

### Comparing `alkymi-0.2.1/alkymi/utils.py` & `alkymi-0.3.0/alkymi/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,111 +1,150 @@
 import asyncio
 import subprocess
 import sys
 import threading
-from typing import List, TextIO, Optional, TypeVar, Callable
-
-from .logging import log
+from typing import List, TextIO, Optional, TypeVar, Callable, IO, Any
 
 
 def call(args: List[str], echo_error_to_stream: Optional[TextIO] = sys.stderr,
          echo_output_to_stream: Optional[TextIO] = sys.stdout) -> subprocess.CompletedProcess:
     """
-    Utility command to run a system command and return the result (stdout and stderr will also be printed to the debug
-    log)
+    Utility command to run a system command and return the result
 
     :param args: The arguments representing the command to run, e.g. ["echo", "test"]
-    :param echo_error_to_stream: A stream to which to echo the call's stderr on a non-zero exit code
+    :param echo_error_to_stream: A stream to which to echo the call's stderr while the command is executing
     :param echo_output_to_stream: A stream to which to echo the call's stdout while the command is executing
     :return: The result of the execution as a subprocess.CompletedProcess instance
     """
     # If running through a Lab CLI, sys.stdout may have been redirected
     if echo_output_to_stream is not None and getattr(echo_output_to_stream, "name", None) == sys.stdout.name:
         echo_output_to_stream = sys.stdout
 
+    # If running through a Lab CLI, sys.stderr may have been redirected
+    if echo_error_to_stream is not None and getattr(echo_error_to_stream, "name", None) == sys.stderr.name:
+        echo_error_to_stream = sys.stderr
+
+    # Use shorthands - note that the full check is still used in some places below to satisfy mypy
+    live_stdout = echo_output_to_stream is not None
+    live_stderr = echo_error_to_stream is not None
+
     # Buffer one line at a time if echoing live, otherwise just use the default
-    buffer_size = 1 if echo_output_to_stream is not None else -1
+    buffer_size = 1 if (live_stdout or live_stderr) else -1
     proc = subprocess.Popen(args, universal_newlines=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE,
                             bufsize=buffer_size)
 
     # Since we set these to PIPE, these should never be None
     assert proc.stdout is not None
     assert proc.stderr is not None
 
+    # Variables that will hold the read stdout and stderr
     stdout: str = ""
-    if echo_output_to_stream is not None:
-        # Print each line to the stream as it arrives
-        while proc.poll() is None:
-            line = proc.stdout.readline()
-            echo_output_to_stream.write(line)
-            stdout += line
-
-        # Program has finished executing, check if any part of stdout still needs to be piped
-        line = proc.stdout.readline()
-        if line:
-            echo_output_to_stream.write(line)
-            stdout += line
+    stderr: str = ""
+
+    # If reading both stdout and stderr, use threads to avoid blocking
+    if live_stdout and live_stderr:
+        assert echo_output_to_stream is not None
+        assert echo_error_to_stream is not None
+        stdout_fut = run_on_thread(_tee_pipe, proc, proc.stdout, echo_output_to_stream)
+        stderr_fut = run_on_thread(_tee_pipe, proc, proc.stderr, echo_error_to_stream)
+        stdout = stdout_fut()
+        stderr = stderr_fut()
+    elif live_stdout:
+        assert echo_output_to_stream is not None
+        stdout = _tee_pipe(proc, proc.stdout, echo_output_to_stream)
+    elif live_stderr:
+        assert echo_error_to_stream is not None
+        stderr = _tee_pipe(proc, proc.stderr, echo_error_to_stream)
     else:
-        # Otherwise, simply wait for the command to finish and then grab stdout
+        # Otherwise, simply wait for the command to finish and then grab stdout and/or stderr
         proc.wait()
         stdout = proc.stdout.read()
-
-    stderr = proc.stderr.read()
-
-    # Send to alkymi log
-    log.debug(stdout)
-    log.debug(stderr)
-
-    # Always forward error messages to stderr if needed
-    if echo_error_to_stream is not None and proc.returncode != 0:
-        echo_error_to_stream.write(stderr)
+        stderr = proc.stderr.read()
 
     # Raise an error on failure
     if proc.returncode != 0:
         raise subprocess.CalledProcessError(proc.returncode, proc.args, stdout, stderr)
     return subprocess.CompletedProcess(proc.args, proc.returncode, stdout, stderr)
 
 
+def _tee_pipe(proc: subprocess.Popen, input_stream: IO[str], output_stream: TextIO) -> str:
+    """
+    Reads the content of an input stream while the provided process is running, and echoes it to the provided output
+    stream in real time, while also collecting everything read into a string that is returned once the process has
+    finished executing and all output has been read
+
+    :param proc: The process that produces the output
+    :param input_stream: The stream to read from (should be `proc.stdout` or `proc.stderr`)
+    :param output_stream: The stream to write output to
+    :return: Everything that was read
+    """
+    content: str = ""
+
+    # Program is executing, echo lines as they come in
+    while proc.poll() is None:
+        line = input_stream.readline()
+        output_stream.write(line)
+        content += line
+
+    # Program has finished executing, check if any part of stdout or stderr still needs to be piped
+    line = " "
+    while line:
+        line = input_stream.readline()
+        output_stream.write(line)
+        content += line
+
+    return content
+
+
 T = TypeVar('T')
 
 
-def run_on_thread(func: Callable[..., T]) -> T:
+def run_on_thread(func: Callable[..., T], *args: Any) -> Callable[[], T]:
     """
-    Execute a function on a new thread and return the result - exceptions will be propagated by re-raising
+    Execute a function on a new thread and return a function that can be used to wait for the result - exceptions will
+    be propagated by re-raising once the result is waited for
+
     :param func: The function to run on the new thread
-    :return: The result of the function call
+    :param args: The arguments to pass to the function
+    :return: A function (future) that can be called to block and return the value of the function call
     """
 
     # Mutable object used to store result
     result: List[T] = []
-    ex = []
+    ex: List[Exception] = []
 
     def _call_and_set_result():
-        nonlocal result
+        nonlocal result, ex
         try:
-            result.append(func())
+            result.append(func(*args))
         except Exception as e:
             ex.append(e)
 
     t = threading.Thread(target=_call_and_set_result)
     t.start()
-    t.join()
 
-    # Check if an exception occurred, and reraise
-    if len(ex) != 0:
-        raise ex[0]
-
-    # Ensure that result has been set, and return it
-    assert len(result) == 1, "Function call should have stored return value in result variable"
-    return result[0]
+    def get_result() -> T:
+        # Wait for thread to finish executing
+        t.join()
+
+        # Check if an exception occurred, and reraise
+        if len(ex) != 0:
+            raise ex[0]
+
+        # Ensure that result has been set, and return it
+        assert len(result) == 1, "Function call should have stored return value in result variable"
+        return result[0]
+
+    return get_result
 
 
 def check_current_thread_has_running_event_loop():
     """
     Check if the calling thread has an associated running event loop
+
     :return: True if the calling thread has a running event loop associated with it
     """
     try:
         asyncio.get_running_loop()
         return True
     except RuntimeError:
         return False
```

### Comparing `alkymi-0.2.1/alkymi.egg-info/PKG-INFO` & `alkymi-0.3.0/alkymi.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,100 +1,18 @@
 Metadata-Version: 2.1
 Name: alkymi
-Version: 0.2.1
+Version: 0.3.0
 Summary: alkymi - Pythonic task automation
 Home-page: https://github.com/MathiasStokholm/alkymi
 Author: Mathias Bøgh Stokholm
 Author-email: mathias.stokholm@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/MathiasStokholm/alkymi/
 Project-URL: Tracker, https://github.com/MathiasStokholm/alkymi/issues
 Project-URL: Documentation, https://alkymi.readthedocs.io/en/latest/
-Description: # alkymi ⚗️
-        
-        [![build](https://github.com/MathiasStokholm/alkymi/workflows/build/badge.svg?branch=master)](https://github.com/MathiasStokholm/alkymi/actions?query=workflow%3Abuild)
-        [![docs](https://readthedocs.org/projects/alkymi/badge/?version=latest)](https://alkymi.readthedocs.io/en/latest/?badge=latest)
-        [![coverage](https://codecov.io/gh/MathiasStokholm/alkymi/branch/develop/graph/badge.svg?token=L0DTW805NL)](https://codecov.io/gh/MathiasStokholm/alkymi)
-        [![pypi](https://img.shields.io/pypi/v/alkymi.svg)](https://pypi.org/project/alkymi)
-        [![versions](https://img.shields.io/pypi/pyversions/alkymi.svg)](https://pypi.org/project/alkymi)
-        
-        Alkymi is a pure Python (3.7+) library for describing and executing tasks and pipelines with built-in caching and
-        conditional evaluation based on checksums.
-        
-        Alkymi is easy to install, simple to use, and has very few dependencies outside of Python's standard library. The code
-        is cross-platform, and allows you to write your pipelines once and deploy to multiple operating systems (tested on
-        Linux, Windows and Mac).
-        
-        Documentation, including a quickstart guide, is provided [here](https://alkymi.readthedocs.io/en/latest/).
-        
-        ## Features
-        * Easily define complex data pipelines as decorated Python functions
-          * This allows you to run linting, type checking, etc. on your data pipelines
-        * Return values are automatically cached to disk, regardless of type
-        * Efficiently checks if pipeline is up-to-date
-          * Checks if external files have changed, bound functions have changed or if pipeline dependencies have changed
-        * No domain specific language (DSL) or CLI tool, just regular Python
-          * Supports caching and conditional evaluation in Jupyter Notebooks
-        * Cross-platform - works on Linux, Windows and Mac
-        * Expose recipes as a command-line interface (CLI) using alkymi's
-        [Lab](https://alkymi.readthedocs.io/en/latest/examples/command_line.html) type
-        
-        ## Sample Usage
-        For examples of how to use alkymi, see the
-        [quickstart guide](https://alkymi.readthedocs.io/en/latest/getting_started/quick_start.html).
-        
-        Example code:
-        ```python
-        import numpy as np
-        import alkymi as alk
-        
-        @alk.recipe()
-        def long_running_task() -> np.ndarray:
-            # Perform expensive computation here ...
-            hard_to_compute_result = np.array([42])
-            # Return value will be automatically cached to disk
-            return hard_to_compute_result
-        
-        result = long_running_task.brew()  # == np.ndarray([42])
-        ```
-        
-        Or one of the examples, e.g. [MNIST](https://alkymi.readthedocs.io/en/latest/examples/mnist.html).
-        
-        ## Installation
-        Install via pip:
-        ```shell script
-        pip install --user alkymi
-        ```
-        
-        Or see the [Installation page](https://alkymi.readthedocs.io/en/latest/getting_started/installation.html).
-        
-        ### Testing
-        After installing, you can run the test suite (use the `lint`, `coverage` and `type_check` recipes to perform those
-        actions):
-        ```shell script
-        python3 labfile.py brew test
-        ```
-        
-        ## License
-        alkymi is licensed under The MIT License as found in the LICENSE.md file
-        
-        ## Upcoming Features
-        The following features are being considered for future implementation:
-        * Type annotations propagated from bound functions to recipes
-        * Support for call/type checking all recipes (e.g. by adding a `check` command to `Lab`)
-        * Cache maintenance functionality
-        
-        ## Known Issues
-        * alkymi currently doesn't check custom objects for altered external files when computing cleanliness (e.g. `MyClass`
-        has a `self._some_path` that points to a file somewhere outside alkymi's internal cache)
-        * `alk.foreach()` currently only supports enumerable inputs of type `List` or `Dict`
-        * Recipes marked `transient` will always be dirty, and thus always require reevaluation. This functionality should be
-        replaced by a proper means of creating recipes that don't cache outputs, but only run when needed to provide inputs for
-        downstream recipes
-        
 Keywords: automation,pipeline,validation,preprocessing,make,build,task
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -111,7 +29,92 @@
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: xxhash
+License-File: LICENSE.md
+
+# alkymi ⚗️
+
+[![build](https://github.com/MathiasStokholm/alkymi/workflows/build/badge.svg?branch=master)](https://github.com/MathiasStokholm/alkymi/actions?query=workflow%3Abuild)
+[![docs](https://readthedocs.org/projects/alkymi/badge/?version=latest)](https://alkymi.readthedocs.io/en/latest/?badge=latest)
+[![coverage](https://codecov.io/gh/MathiasStokholm/alkymi/branch/develop/graph/badge.svg?token=L0DTW805NL)](https://codecov.io/gh/MathiasStokholm/alkymi)
+[![pypi](https://img.shields.io/pypi/v/alkymi.svg)](https://pypi.org/project/alkymi)
+[![versions](https://img.shields.io/pypi/pyversions/alkymi.svg)](https://pypi.org/project/alkymi)
+
+Alkymi is a pure Python (3.7+) library for describing and executing tasks and pipelines with built-in caching and
+conditional evaluation based on checksums.
+
+Alkymi is easy to install, simple to use, and has very few dependencies outside of Python's standard library. The code
+is cross-platform, and allows you to write your pipelines once and deploy to multiple operating systems (tested on
+Linux, Windows and Mac).
+
+Documentation, including a quickstart guide, is provided [here](https://alkymi.readthedocs.io/en/latest/).
+
+## Features
+* Easily define complex data pipelines as decorated Python functions
+  * This allows you to run linting, type checking, etc. on your data pipelines
+* Return values are automatically cached to disk, regardless of type
+* Efficiently checks if pipeline is up-to-date
+  * Checks if external files have changed, bound functions have changed or if pipeline dependencies have changed
+* No domain specific language (DSL) or CLI tool, just regular Python
+  * Supports caching and conditional evaluation in Jupyter Notebooks
+* Cross-platform - works on Linux, Windows and Mac
+* Expose recipes as a command-line interface (CLI) using alkymi's
+[Lab](https://alkymi.readthedocs.io/en/latest/examples/command_line.html) type
+
+## Sample Usage
+For examples of how to use alkymi, see the
+[quickstart guide](https://alkymi.readthedocs.io/en/latest/getting_started/quick_start.html).
+
+Example code:
+```python
+import numpy as np
+import alkymi as alk
+
+@alk.recipe()
+def long_running_task() -> np.ndarray:
+    # Perform expensive computation here ...
+    hard_to_compute_result = np.array([42])
+    # Return value will be automatically cached to disk
+    return hard_to_compute_result
+
+result = long_running_task.brew()  # == np.ndarray([42])
+```
+
+Or one of the examples, e.g. [MNIST](https://alkymi.readthedocs.io/en/latest/examples/mnist.html).
+
+## Installation
+Install via pip:
+```shell script
+pip install --user alkymi
+```
+
+Or see the [Installation page](https://alkymi.readthedocs.io/en/latest/getting_started/installation.html).
+
+### Testing
+After installing, you can run the test suite (use the `lint`, `coverage` and `type_check` recipes to perform those
+actions):
+```shell script
+python3 labfile.py brew test
+```
+
+## License
+alkymi is licensed under The MIT License as found in the LICENSE.md file
+
+## Upcoming Features
+The following features are being considered for future implementation:
+* Type annotations propagated from bound functions to recipes
+* Support for call/type checking all recipes (e.g. by adding a `check` command to `Lab`)
+* Cache maintenance functionality
+
+## Known Issues
+* alkymi currently doesn't check custom objects for altered external files when computing cleanliness (e.g. `MyClass`
+has a `self._some_path` that points to a file somewhere outside alkymi's internal cache)
+* `alk.foreach()` currently only supports enumerable inputs of type `List` or `Dict`
+* Recipes marked `transient` will always be dirty, and thus always require reevaluation. This functionality should be
+replaced by a proper means of creating recipes that don't cache outputs, but only run when needed to provide inputs for
+downstream recipes
+
+
```

### Comparing `alkymi-0.2.1/setup.py` & `alkymi-0.3.0/setup.py`

 * *Files identical despite different names*

