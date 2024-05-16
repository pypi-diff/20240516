# Comparing `tmp/deephaven-plugin-matplotlib-0.3.0.tar.gz` & `tmp/deephaven_plugin_matplotlib-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deephaven-plugin-matplotlib-0.3.0.tar", last modified: Fri Dec 22 21:19:49 2023, max compression
+gzip compressed data, was "deephaven_plugin_matplotlib-0.4.0.tar", last modified: Thu May 16 17:26:03 2024, max compression
```

## Comparing `deephaven-plugin-matplotlib-0.3.0.tar` & `deephaven_plugin_matplotlib-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:19:48.995904 deephaven-plugin-matplotlib-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2023-12-22 21:18:55.000000 deephaven-plugin-matplotlib-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5370 2023-12-22 21:19:48.995904 deephaven-plugin-matplotlib-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4395 2023-12-22 21:18:55.000000 deephaven-plugin-matplotlib-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       98 2023-12-22 21:18:55.000000 deephaven-plugin-matplotlib-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2023-12-22 21:19:48.995904 deephaven-plugin-matplotlib-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:19:48.995904 deephaven-plugin-matplotlib-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:19:48.991904 deephaven-plugin-matplotlib-0.3.0/src/deephaven/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:19:48.991904 deephaven-plugin-matplotlib-0.3.0/src/deephaven/plugin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:19:48.995904 deephaven-plugin-matplotlib-0.3.0/src/deephaven/plugin/matplotlib/
--rw-r--r--   0 runner    (1001) docker     (127)     5787 2023-12-22 21:18:55.000000 deephaven-plugin-matplotlib-0.3.0/src/deephaven/plugin/matplotlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2023-12-22 21:18:55.000000 deephaven-plugin-matplotlib-0.3.0/src/deephaven/plugin/matplotlib/deephaven.mplstyle
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2023-12-22 21:18:55.000000 deephaven-plugin-matplotlib-0.3.0/src/deephaven/plugin/matplotlib/figure_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:19:48.995904 deephaven-plugin-matplotlib-0.3.0/src/deephaven_plugin_matplotlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5370 2023-12-22 21:19:48.000000 deephaven-plugin-matplotlib-0.3.0/src/deephaven_plugin_matplotlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      516 2023-12-22 21:19:48.000000 deephaven-plugin-matplotlib-0.3.0/src/deephaven_plugin_matplotlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-22 21:19:48.000000 deephaven-plugin-matplotlib-0.3.0/src/deephaven_plugin_matplotlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2023-12-22 21:19:48.000000 deephaven-plugin-matplotlib-0.3.0/src/deephaven_plugin_matplotlib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2023-12-22 21:19:48.000000 deephaven-plugin-matplotlib-0.3.0/src/deephaven_plugin_matplotlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-12-22 21:19:48.000000 deephaven-plugin-matplotlib-0.3.0/src/deephaven_plugin_matplotlib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:26:03.792767 deephaven_plugin_matplotlib-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-16 17:24:44.000000 deephaven_plugin_matplotlib-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5418 2024-05-16 17:26:03.792767 deephaven_plugin_matplotlib-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-05-16 17:24:44.000000 deephaven_plugin_matplotlib-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-16 17:24:44.000000 deephaven_plugin_matplotlib-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-16 17:26:03.792767 deephaven_plugin_matplotlib-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-16 17:24:44.000000 deephaven_plugin_matplotlib-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:26:03.788767 deephaven_plugin_matplotlib-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:26:03.788767 deephaven_plugin_matplotlib-0.4.0/src/deephaven/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:26:03.788767 deephaven_plugin_matplotlib-0.4.0/src/deephaven/plugin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:26:03.792767 deephaven_plugin_matplotlib-0.4.0/src/deephaven/plugin/matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-05-16 17:24:44.000000 deephaven_plugin_matplotlib-0.4.0/src/deephaven/plugin/matplotlib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:26:03.792767 deephaven_plugin_matplotlib-0.4.0/src/deephaven/plugin/matplotlib/_js/
+-rw-r--r--   0 runner    (1001) docker     (127)     9793 1985-10-26 08:15:00.000000 deephaven_plugin_matplotlib-0.4.0/src/deephaven/plugin/matplotlib/_js/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      290 1985-10-26 08:15:00.000000 deephaven_plugin_matplotlib-0.4.0/src/deephaven/plugin/matplotlib/_js/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:26:03.792767 deephaven_plugin_matplotlib-0.4.0/src/deephaven/plugin/matplotlib/_js/dist/
+-rw-r--r--   0 runner    (1001) docker     (127)     6157 1985-10-26 08:15:00.000000 deephaven_plugin_matplotlib-0.4.0/src/deephaven/plugin/matplotlib/_js/dist/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 1985-10-26 08:15:00.000000 deephaven_plugin_matplotlib-0.4.0/src/deephaven/plugin/matplotlib/_js/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-16 17:24:44.000000 deephaven_plugin_matplotlib-0.4.0/src/deephaven/plugin/matplotlib/_js_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-16 17:24:44.000000 deephaven_plugin_matplotlib-0.4.0/src/deephaven/plugin/matplotlib/_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-16 17:24:44.000000 deephaven_plugin_matplotlib-0.4.0/src/deephaven/plugin/matplotlib/deephaven.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-05-16 17:24:44.000000 deephaven_plugin_matplotlib-0.4.0/src/deephaven/plugin/matplotlib/figure_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:26:03.792767 deephaven_plugin_matplotlib-0.4.0/src/deephaven_plugin_matplotlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5418 2024-05-16 17:26:03.000000 deephaven_plugin_matplotlib-0.4.0/src/deephaven_plugin_matplotlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-16 17:26:03.000000 deephaven_plugin_matplotlib-0.4.0/src/deephaven_plugin_matplotlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 17:26:03.000000 deephaven_plugin_matplotlib-0.4.0/src/deephaven_plugin_matplotlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-16 17:26:03.000000 deephaven_plugin_matplotlib-0.4.0/src/deephaven_plugin_matplotlib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-16 17:26:03.000000 deephaven_plugin_matplotlib-0.4.0/src/deephaven_plugin_matplotlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 17:26:03.000000 deephaven_plugin_matplotlib-0.4.0/src/deephaven_plugin_matplotlib.egg-info/top_level.txt
```

### Comparing `deephaven-plugin-matplotlib-0.3.0/LICENSE` & `deephaven_plugin_matplotlib-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-matplotlib-0.3.0/PKG-INFO` & `deephaven_plugin_matplotlib-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deephaven-plugin-matplotlib
-Version: 0.3.0
+Version: 0.4.0
 Summary: Deephaven Plugin for matplotlib
 Home-page: https://github.com/deephaven/deephaven-plugins
 Author: Devin Smith
 Author-email: devinsmith@deephaven.io
 Project-URL: Source Code, https://github.com/deephaven/deephaven-plugins
 Project-URL: Bug Tracker, https://github.com/deephaven/deephaven-plugins/issues
 Keywords: deephaven,plugin,matplotlib
@@ -17,36 +17,40 @@
 Classifier: Development Status :: 3 - Alpha
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: deephaven-core>=0.27.0
 Requires-Dist: jpy>=0.14.0
 Requires-Dist: deephaven-plugin>=0.5.0
 Requires-Dist: matplotlib
+Requires-Dist: deephaven-plugin-utilities
 Provides-Extra: seaborn
 Requires-Dist: seaborn>=0.13.0; extra == "seaborn"
 
 # Deephaven Plugin for matplotlib
 
 The Deephaven Plugin for matplotlib. Allows for opening matplotlib plots in a Deephaven environment. Any matplotlib plot
 should be viewable by default. For example:
+
 ```python
 import matplotlib.pyplot as plt
 
 fig = plt.figure()
 ax = fig.subplots()  # Create a figure containing a single axes.
 ax.plot([1, 2, 3, 4], [4, 2, 6, 7])  # Plot some data on the axes.
 ```
+
 You can also use `TableAnimation`, which allows updating a plot whenever a Deephaven Table is updated.
 
 ## `TableAnimation` Usage
 
 `TableAnimation` is a matplotlib `Animation` that is driven by updates in a Deephaven Table. Every time the table that
 is being listened to updates, the provided function will run again.
 
 ### Line Plot
+
 ```python
 import matplotlib.pyplot as plt
 from deephaven import time_table
 from deephaven.plugin.matplotlib import TableAnimation
 
 # Create a ticking table with the sin function
 tt = time_table("PT00:00:01").update(["x=i", "y=Math.sin(x)"])
@@ -67,15 +71,17 @@
 
 
 # Create our animation. It will listen for updates on `tt` and call `update_fig` whenever there is an update
 ani = TableAnimation(fig, tt, update_fig)
 ```
 
 ### Scatter Plot
+
 Scatter plots require data in a different format that Line plots, so need to pass in the data differently.
+
 ```python
 import matplotlib.pyplot as plt
 from deephaven import time_table
 from deephaven.plugin.matplotlib import TableAnimation
 
 tt = time_table("PT00:00:01").update(
     ["x=Math.random()", "y=Math.random()", "z=Math.random()*50"]
@@ -104,15 +110,17 @@
     scat.set_sizes(scatter_sizes)
 
 
 ani = TableAnimation(fig, tt, update_fig)
 ```
 
 ### Multiple Series
+
 It's possible to have multiple kinds of series in the same figure. Here is an example driving a line and a scatter plot:
+
 ```python
 import matplotlib.pyplot as plt
 from deephaven import time_table
 from deephaven.plugin.matplotlib import TableAnimation
 
 tt = time_table("PT00:00:01").update(
     ["x=i", "y=Math.sin(x)", "z=Math.cos(x)", "r=Math.random()", "s=Math.random()*100"]
@@ -156,11 +164,11 @@
 
 To build:
 
 ```sh
 python -m build --wheel
 ```
 
-The wheel is stored in `dist/`. 
+The wheel is stored in `dist/`.
 
 To test within [deephaven-core](https://github.com/deephaven/deephaven-core), note where this wheel is stored (using `pwd`, for example).
 Then, follow the directions in the top-level README.md to install the wheel into your Deephaven environment.
```

### Comparing `deephaven-plugin-matplotlib-0.3.0/README.md` & `deephaven_plugin_matplotlib-0.4.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 # Deephaven Plugin for matplotlib
 
 The Deephaven Plugin for matplotlib. Allows for opening matplotlib plots in a Deephaven environment. Any matplotlib plot
 should be viewable by default. For example:
+
 ```python
 import matplotlib.pyplot as plt
 
 fig = plt.figure()
 ax = fig.subplots()  # Create a figure containing a single axes.
 ax.plot([1, 2, 3, 4], [4, 2, 6, 7])  # Plot some data on the axes.
 ```
+
 You can also use `TableAnimation`, which allows updating a plot whenever a Deephaven Table is updated.
 
 ## `TableAnimation` Usage
 
 `TableAnimation` is a matplotlib `Animation` that is driven by updates in a Deephaven Table. Every time the table that
 is being listened to updates, the provided function will run again.
 
 ### Line Plot
+
 ```python
 import matplotlib.pyplot as plt
 from deephaven import time_table
 from deephaven.plugin.matplotlib import TableAnimation
 
 # Create a ticking table with the sin function
 tt = time_table("PT00:00:01").update(["x=i", "y=Math.sin(x)"])
@@ -41,15 +44,17 @@
 
 
 # Create our animation. It will listen for updates on `tt` and call `update_fig` whenever there is an update
 ani = TableAnimation(fig, tt, update_fig)
 ```
 
 ### Scatter Plot
+
 Scatter plots require data in a different format that Line plots, so need to pass in the data differently.
+
 ```python
 import matplotlib.pyplot as plt
 from deephaven import time_table
 from deephaven.plugin.matplotlib import TableAnimation
 
 tt = time_table("PT00:00:01").update(
     ["x=Math.random()", "y=Math.random()", "z=Math.random()*50"]
@@ -78,15 +83,17 @@
     scat.set_sizes(scatter_sizes)
 
 
 ani = TableAnimation(fig, tt, update_fig)
 ```
 
 ### Multiple Series
+
 It's possible to have multiple kinds of series in the same figure. Here is an example driving a line and a scatter plot:
+
 ```python
 import matplotlib.pyplot as plt
 from deephaven import time_table
 from deephaven.plugin.matplotlib import TableAnimation
 
 tt = time_table("PT00:00:01").update(
     ["x=i", "y=Math.sin(x)", "z=Math.cos(x)", "r=Math.random()", "s=Math.random()*100"]
@@ -130,11 +137,11 @@
 
 To build:
 
 ```sh
 python -m build --wheel
 ```
 
-The wheel is stored in `dist/`. 
+The wheel is stored in `dist/`.
 
 To test within [deephaven-core](https://github.com/deephaven/deephaven-core), note where this wheel is stored (using `pwd`, for example).
-Then, follow the directions in the top-level README.md to install the wheel into your Deephaven environment.
+Then, follow the directions in the top-level README.md to install the wheel into your Deephaven environment.
```

### Comparing `deephaven-plugin-matplotlib-0.3.0/setup.cfg` & `deephaven_plugin_matplotlib-0.4.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = deephaven-plugin-matplotlib
 description = Deephaven Plugin for matplotlib
 long_description = file: README.md
 long_description_content_type = text/markdown
-version = attr:deephaven.plugin.matplotlib.__version__
+version = 0.4.0
 url = https://github.com/deephaven/deephaven-plugins
 project_urls = 
 	Source Code = https://github.com/deephaven/deephaven-plugins
 	Bug Tracker = https://github.com/deephaven/deephaven-plugins/issues
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: Apache Software License
@@ -25,27 +25,25 @@
 	=src
 packages = find_namespace:
 install_requires = 
 	deephaven-core>=0.27.0
 	jpy>=0.14.0
 	deephaven-plugin>=0.5.0
 	matplotlib
+	deephaven-plugin-utilities
 include_package_data = True
 
 [options.extras_require]
 seaborn = 
 	seaborn>=0.13.0
 
 [options.packages.find]
 where = src
 
-[options.package_data]
-* = *.mplstyle
-
 [options.entry_points]
 deephaven.plugin = 
-	registration_cls = deephaven.plugin.matplotlib:MatplotlibRegistration
+	registration_cls = deephaven.plugin.matplotlib._register:MatplotlibRegistration
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `deephaven-plugin-matplotlib-0.3.0/src/deephaven/plugin/matplotlib/__init__.py` & `deephaven_plugin_matplotlib-0.4.0/src/deephaven/plugin/matplotlib/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,11 @@
 from deephaven import numpy as dhnp
-from deephaven.plugin import Registration, Callback
 from deephaven.table_listener import listen
-from importlib import resources
-import matplotlib.pyplot as plt
 from matplotlib.animation import Animation
 import itertools
-from deephaven.execution_context import get_exec_ctx
-
-
-__version__ = "0.3.0"
-
-
-def _init_theme():
-    # Set the Deephaven style globally.
-    # We use the savefig function to export the Figure, and that uses the Figure's properties for colours rather than temporary styling.
-    # The Figure's properties are set on creation time of the Figure, rather than when the Figure is exported
-    # We do not have hooks into when a user creates a new Figure, so we set the theme globally ahead of time
-    # https://github.com/matplotlib/matplotlib/issues/6592/
-    with resources.path(__package__, "deephaven.mplstyle") as p:
-        plt.style.use(["dark_background", p])
-
-
-class MatplotlibRegistration(Registration):
-    @classmethod
-    def register_into(cls, callback: Callback) -> None:
-        _init_theme()
-        plt.switch_backend("AGG")
-        from . import figure_type
-
-        callback.register(figure_type.FigureType)
 
 
 class TableEventSource:
     """
     Makes an event source for matplotlib that triggers whenever Deephaven Table updates.
 
     Parameters
@@ -142,28 +115,28 @@
         else:
             self._columns = columns
         self._last_update = None
         event_source = TableEventSource(table)
         super().__init__(fig, event_source, **kwargs)
 
         # Start the animation right away
-        self._start()
+        self._start()  # type: ignore
 
     def new_frame_seq(self):
         """
         new_frame_seq
         """
         # Use the generating function to generate a new frame sequence
         return itertools.count()
 
     def _step(self, update, *args):
         """Handler for getting events."""
         # Extends the _step() method for the Animation class. Used
         # to get the update information
         self._last_update = update
-        return super()._step(*args)
+        return super()._step(*args)  # type: ignore
 
     def _draw_frame(self, framedata):
         data = {}
         for column in self._columns:
             data[column] = dhnp.to_numpy(self._table, [column])[:, 0]
         self._func(data, self._last_update, *self._args)
```

### Comparing `deephaven-plugin-matplotlib-0.3.0/src/deephaven/plugin/matplotlib/figure_type.py` & `deephaven_plugin_matplotlib-0.4.0/src/deephaven/plugin/matplotlib/figure_type.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-matplotlib-0.3.0/src/deephaven_plugin_matplotlib.egg-info/PKG-INFO` & `deephaven_plugin_matplotlib-0.4.0/src/deephaven_plugin_matplotlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deephaven-plugin-matplotlib
-Version: 0.3.0
+Version: 0.4.0
 Summary: Deephaven Plugin for matplotlib
 Home-page: https://github.com/deephaven/deephaven-plugins
 Author: Devin Smith
 Author-email: devinsmith@deephaven.io
 Project-URL: Source Code, https://github.com/deephaven/deephaven-plugins
 Project-URL: Bug Tracker, https://github.com/deephaven/deephaven-plugins/issues
 Keywords: deephaven,plugin,matplotlib
@@ -17,36 +17,40 @@
 Classifier: Development Status :: 3 - Alpha
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: deephaven-core>=0.27.0
 Requires-Dist: jpy>=0.14.0
 Requires-Dist: deephaven-plugin>=0.5.0
 Requires-Dist: matplotlib
+Requires-Dist: deephaven-plugin-utilities
 Provides-Extra: seaborn
 Requires-Dist: seaborn>=0.13.0; extra == "seaborn"
 
 # Deephaven Plugin for matplotlib
 
 The Deephaven Plugin for matplotlib. Allows for opening matplotlib plots in a Deephaven environment. Any matplotlib plot
 should be viewable by default. For example:
+
 ```python
 import matplotlib.pyplot as plt
 
 fig = plt.figure()
 ax = fig.subplots()  # Create a figure containing a single axes.
 ax.plot([1, 2, 3, 4], [4, 2, 6, 7])  # Plot some data on the axes.
 ```
+
 You can also use `TableAnimation`, which allows updating a plot whenever a Deephaven Table is updated.
 
 ## `TableAnimation` Usage
 
 `TableAnimation` is a matplotlib `Animation` that is driven by updates in a Deephaven Table. Every time the table that
 is being listened to updates, the provided function will run again.
 
 ### Line Plot
+
 ```python
 import matplotlib.pyplot as plt
 from deephaven import time_table
 from deephaven.plugin.matplotlib import TableAnimation
 
 # Create a ticking table with the sin function
 tt = time_table("PT00:00:01").update(["x=i", "y=Math.sin(x)"])
@@ -67,15 +71,17 @@
 
 
 # Create our animation. It will listen for updates on `tt` and call `update_fig` whenever there is an update
 ani = TableAnimation(fig, tt, update_fig)
 ```
 
 ### Scatter Plot
+
 Scatter plots require data in a different format that Line plots, so need to pass in the data differently.
+
 ```python
 import matplotlib.pyplot as plt
 from deephaven import time_table
 from deephaven.plugin.matplotlib import TableAnimation
 
 tt = time_table("PT00:00:01").update(
     ["x=Math.random()", "y=Math.random()", "z=Math.random()*50"]
@@ -104,15 +110,17 @@
     scat.set_sizes(scatter_sizes)
 
 
 ani = TableAnimation(fig, tt, update_fig)
 ```
 
 ### Multiple Series
+
 It's possible to have multiple kinds of series in the same figure. Here is an example driving a line and a scatter plot:
+
 ```python
 import matplotlib.pyplot as plt
 from deephaven import time_table
 from deephaven.plugin.matplotlib import TableAnimation
 
 tt = time_table("PT00:00:01").update(
     ["x=i", "y=Math.sin(x)", "z=Math.cos(x)", "r=Math.random()", "s=Math.random()*100"]
@@ -156,11 +164,11 @@
 
 To build:
 
 ```sh
 python -m build --wheel
 ```
 
-The wheel is stored in `dist/`. 
+The wheel is stored in `dist/`.
 
 To test within [deephaven-core](https://github.com/deephaven/deephaven-core), note where this wheel is stored (using `pwd`, for example).
 Then, follow the directions in the top-level README.md to install the wheel into your Deephaven environment.
```

### Comparing `deephaven-plugin-matplotlib-0.3.0/src/deephaven_plugin_matplotlib.egg-info/SOURCES.txt` & `deephaven_plugin_matplotlib-0.4.0/src/deephaven_plugin_matplotlib.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
+setup.py
 src/deephaven/plugin/matplotlib/__init__.py
+src/deephaven/plugin/matplotlib/_js_plugin.py
+src/deephaven/plugin/matplotlib/_register.py
 src/deephaven/plugin/matplotlib/deephaven.mplstyle
 src/deephaven/plugin/matplotlib/figure_type.py
+src/deephaven/plugin/matplotlib/_js/LICENSE
+src/deephaven/plugin/matplotlib/_js/README.md
+src/deephaven/plugin/matplotlib/_js/package.json
+src/deephaven/plugin/matplotlib/_js/dist/index.js
 src/deephaven_plugin_matplotlib.egg-info/PKG-INFO
 src/deephaven_plugin_matplotlib.egg-info/SOURCES.txt
 src/deephaven_plugin_matplotlib.egg-info/dependency_links.txt
 src/deephaven_plugin_matplotlib.egg-info/entry_points.txt
 src/deephaven_plugin_matplotlib.egg-info/requires.txt
 src/deephaven_plugin_matplotlib.egg-info/top_level.txt
```

