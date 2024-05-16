# Comparing `tmp/plsp-0.1.tar.gz` & `tmp/plsp-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plsp-0.1.tar", last modified: Thu May 16 03:03:06 2024, max compression
+gzip compressed data, was "plsp-0.2.tar", last modified: Thu May 16 09:52:27 2024, max compression
```

## Comparing `plsp-0.1.tar` & `plsp-0.2.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxrwxr-x   0 joel-watson  (1000) joel-watson  (1000)        0 2024-05-16 03:03:06.515986 plsp-0.1/
--rw-r--r--   0 joel-watson  (1000) joel-watson  (1000)     6008 2024-05-16 03:03:06.499986 plsp-0.1/PKG-INFO
--rw-rw-r--   0 joel-watson  (1000) joel-watson  (1000)     5748 2024-05-16 03:00:31.000000 plsp-0.1/README.md
-drwxrwxr-x   0 joel-watson  (1000) joel-watson  (1000)        0 2024-05-16 03:03:06.499986 plsp-0.1/plsp/
--rw-rw-r--   0 joel-watson  (1000) joel-watson  (1000)     4369 2024-05-16 02:49:19.000000 plsp-0.1/plsp/DebugContext.py
--rw-rw-r--   0 joel-watson  (1000) joel-watson  (1000)      921 2024-05-16 01:51:27.000000 plsp-0.1/plsp/DebugMode.py
--rw-rw-r--   0 joel-watson  (1000) joel-watson  (1000)      257 2024-05-16 02:48:17.000000 plsp-0.1/plsp/Direction.py
--rw-rw-r--   0 joel-watson  (1000) joel-watson  (1000)     8155 2024-05-16 03:01:57.000000 plsp-0.1/plsp/Logger.py
--rw-rw-r--   0 joel-watson  (1000) joel-watson  (1000)     2284 2024-05-16 02:35:45.000000 plsp-0.1/plsp/__init__.py
-drwxrwxr-x   0 joel-watson  (1000) joel-watson  (1000)        0 2024-05-16 03:03:06.499986 plsp-0.1/plsp/formatters/
--rw-rw-r--   0 joel-watson  (1000) joel-watson  (1000)     1063 2024-05-16 01:51:27.000000 plsp-0.1/plsp/formatters/FinalFormatter.py
--rw-rw-r--   0 joel-watson  (1000) joel-watson  (1000)     1269 2024-05-16 01:51:27.000000 plsp-0.1/plsp/formatters/Formatter.py
--rw-rw-r--   0 joel-watson  (1000) joel-watson  (1000)       53 2024-05-16 02:35:34.000000 plsp-0.1/plsp/formatters/__init__.py
--rw-rw-r--   0 joel-watson  (1000) joel-watson  (1000)      222 2024-05-16 02:35:10.000000 plsp-0.1/plsp/formatters/defaults.py
-drwxrwxr-x   0 joel-watson  (1000) joel-watson  (1000)        0 2024-05-16 03:03:06.499986 plsp-0.1/plsp/infoinject/
--rw-rw-r--   0 joel-watson  (1000) joel-watson  (1000)    10444 2024-05-16 03:02:06.000000 plsp-0.1/plsp/infoinject/InfoInjector.py
--rw-rw-r--   0 joel-watson  (1000) joel-watson  (1000)       38 2024-05-16 02:35:56.000000 plsp-0.1/plsp/infoinject/__init__.py
-drwxrwxr-x   0 joel-watson  (1000) joel-watson  (1000)        0 2024-05-16 03:03:06.499986 plsp-0.1/plsp.egg-info/
--rw-r--r--   0 joel-watson  (1000) joel-watson  (1000)     6008 2024-05-16 03:03:06.000000 plsp-0.1/plsp.egg-info/PKG-INFO
--rw-rw-r--   0 joel-watson  (1000) joel-watson  (1000)      398 2024-05-16 03:03:06.000000 plsp-0.1/plsp.egg-info/SOURCES.txt
--rw-rw-r--   0 joel-watson  (1000) joel-watson  (1000)        1 2024-05-16 03:03:06.000000 plsp-0.1/plsp.egg-info/dependency_links.txt
--rw-rw-r--   0 joel-watson  (1000) joel-watson  (1000)        5 2024-05-16 03:03:06.000000 plsp-0.1/plsp.egg-info/top_level.txt
--rw-rw-r--   0 joel-watson  (1000) joel-watson  (1000)       38 2024-05-16 03:03:06.515986 plsp-0.1/setup.cfg
--rw-rw-r--   0 joel-watson  (1000) joel-watson  (1000)      254 2024-05-16 03:00:36.000000 plsp-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:52:27.586383 plsp-0.2/
+-rw-rw-rw-   0        0        0     6318 2024-05-16 09:52:27.585356 plsp-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5929 2024-05-16 09:31:25.000000 plsp-0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 09:52:27.572222 plsp-0.2/plsp/
+-rw-rw-rw-   0        0        0     4630 2024-05-16 09:31:25.000000 plsp-0.2/plsp/DebugContext.py
+-rw-rw-rw-   0        0        0      964 2024-05-16 09:31:25.000000 plsp-0.2/plsp/DebugMode.py
+-rw-rw-rw-   0        0        0      267 2024-05-16 09:31:25.000000 plsp-0.2/plsp/Direction.py
+-rw-rw-rw-   0        0        0     9084 2024-05-16 09:31:25.000000 plsp-0.2/plsp/Logger.py
+-rw-rw-rw-   0        0        0     2102 2024-05-16 09:31:25.000000 plsp-0.2/plsp/SharedLogger.py
+-rw-rw-rw-   0        0        0     2516 2024-05-16 09:31:25.000000 plsp-0.2/plsp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:52:27.581320 plsp-0.2/plsp/formatters/
+-rw-rw-rw-   0        0        0     1114 2024-05-16 09:31:25.000000 plsp-0.2/plsp/formatters/FinalFormatter.py
+-rw-rw-rw-   0        0        0     1445 2024-05-16 09:31:25.000000 plsp-0.2/plsp/formatters/Formatter.py
+-rw-rw-rw-   0        0        0      103 2024-05-16 09:31:25.000000 plsp-0.2/plsp/formatters/__init__.py
+-rw-rw-rw-   0        0        0     1224 2024-05-16 09:31:25.000000 plsp-0.2/plsp/formatters/bundled.py
+-rw-rw-rw-   0        0        0      243 2024-05-16 09:31:25.000000 plsp-0.2/plsp/formatters/defaults.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:52:27.583341 plsp-0.2/plsp/infoinject/
+-rw-rw-rw-   0        0        0    10840 2024-05-16 09:31:25.000000 plsp-0.2/plsp/infoinject/InfoInjector.py
+-rw-rw-rw-   0        0        0       38 2024-05-16 09:31:25.000000 plsp-0.2/plsp/infoinject/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:52:27.584352 plsp-0.2/plsp.egg-info/
+-rw-rw-rw-   0        0        0     6318 2024-05-16 09:52:27.000000 plsp-0.2/plsp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      473 2024-05-16 09:52:27.000000 plsp-0.2/plsp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 09:52:27.000000 plsp-0.2/plsp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-16 09:52:27.000000 plsp-0.2/plsp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-16 09:52:27.000000 plsp-0.2/plsp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 09:52:27.586383 plsp-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      314 2024-05-16 09:50:49.000000 plsp-0.2/setup.py
```

### Comparing `plsp-0.1/PKG-INFO` & `plsp-0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,191 +1,192 @@
-Metadata-Version: 2.1
-Name: plsp
-Version: 0.1
-Summary: A simple, easy to use, and powerful logging library for Python.
-Author: matrikater (Joel Watson)
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-
-# Please Log Shit Please (or `plsp`)
-
-## Notes
-
-```text
-info inject is a module allowing you to compile python source code with added debug information.
-this means that the interesting parts of the code stay separate from printing and other debug code.
-```
-
-```text
-=====================
-Pieces of the puzzle.
-=====================
-
-Logger 			- The piece that does the logging.
-
-DebugContext 		- Use this along side with the logger to separate different areas of an application.
-			- For example, you may have a rendering context and a physics context inside a game engine.
-
-DebugMode 		- Use this to specify different levels of debug information.
-			- For example, you may have a "info" mode and a "detail" mode.
-			- If the "info" mode is active, any messages that are in the "detail" mode will not be printed.
-			- This is because the "detail" mode extends from the "info" mode.
-			- If the "detail" mode is active, any messages that are in the "info"
-			-   and "detail" mode will be printed.
-
-ColorConfiguration 	- Use this to specify the colors of the debug information.
-			- For example, you may want to have the rendering context to be in green
-			-   and the physics context to be in red.
-
-InfoInjector 		- The piece that injects the debug information into the source code.
-			- Uses the Logger to log the debug information.
-
-formatters/ 		- The pieces that format the debug information.
-			- For example, you may want to have the time of the debug information to
-			-   be formatted in a specific way.
-			- You may also want to have the caller of the debug information to be formatted in a specific way.
-			- The formatters may be added onto any specified debug context. Then, when the Logger is used
-			-   by said context, the formatters will be used to format the debug information.
-
-
-
-====================================
-How the pieces relate to each other.
-====================================
-
-> Nodes A that is down from node B means that A depends on, or is used by, B.
-
-	Logger
-	/ \
-	+  +--------------------+
-	|                       |
-	Debug Context           Debug Mode
-	/ \
-	+  +--------------------+
-	|                       |
-	Color Configuration     formatters/
-```
-
-## Usage
-
-```python
-from pls.Logger import plsp
-#from formatters import TimeFormatter, CallerFormatter
-from plsp.DebugMode import DebugMode
-from plsp.Direction import IODirection
-
-import sys
-
-# use below to separate log files based on debug mode instead of debug context.
-#plsp.set("io_based_on_mode", True)
-
-
-
-# The below sets the global context to generic.
-plsp.set("global_context", "generic")
-
-
-
-# Below is adding a debug context.
-# It is a bit more complicated than setting up debug contexts so you dont have to set all the parameters at once.
-plsp.add_debug_context("generic")
-plsp.add_debug_context("rendering")
-plsp.add_debug_context("physics")
-
-
-
-# Below is adding a debug mode.
-# You can:
-# - Use the `write_to_file` parameter to specify a file to write to.
-# - Use the `write_to_io` parameter to specify an io object to write to.
-# - Use the `separate` parameter to specify if this is a standalone debug mode, meaning, if this mode is active,
-#     the previous debug mode will not be active.
-plsp.add_debug_mode("info")
-plsp.add_debug_mode("detail")
-plsp.add_debug_mode("debug")
-plsp.add_debug_mode("error", separate=True)
-
-
-
-# START OF MODIFYING DEBUG CONTEXTS #
-
-# You may modify the debug contexts after they are created.
-# Access the debug context by using the `Logger.debug_contexts` dictionary.
-
-pls.get_debug_context("generic").set_can_ever_write(True)
-plsp.get_debug_context("generic").add_direction(IODirection(False, sys.stdout.fileno(), None))
-plsp.get_debug_context("rendering").set_can_ever_write(True)
-plsp.get_debug_context("rendering").add_direction(IODirection(False, sys.stdout.fileno(), None))
-plsp.get_debug_context("physics").set_can_ever_write(True)
-plsp.get_debug_context("physics").add_direction(IODirection(False, sys.stdout.fileno(), None))
-					       
-# The below will add the time before each log message.
-#plsp.get_debug_context("generic").add_format_layer(TimeFormatter)
-#plsp.get_debug_context("rendering").add_format_layer(TimeFormatter)
-#plsp.get_debug_context("physics").add_format_layer(TimeFormatter)
-#
-## The below will add which ever function called the log message.
-#plsp.get_debug_context("generic").add_format_layer(CallerFormatter)
-#plsp.get_debug_context("rendering").add_format_layer(CallerFormatter)
-#plsp.get_debug_context("physics").add_format_layer(CallerFormatter)
-#
-
-# END OF MODIFYING DEBUG CONTEXTS #
-
-
-
-# Now we can use the debug contexts to log messages.
-plsp.set_debug_mode("info")
-
-plsp().info("This is using the generic context.")
-plsp().info("It works since we set a global context.")
-
-
-
-class renderer:
-	def __init__(self):
-		plsp().rendering.detail("The rendering engine in this engine is pretty simple!")
-
-
-
-class physics:
-	def __init__(self):
-		plsp().physics.detail("The physics engine in this engine is pretty simple!")
-
-
-#my_renderer = renderer()
-my_physics = physics()
-
-plsp.set_debug_mode("detail")
-
-my_physics = physics()
-
-
-
-
-
-
-
-from plsp.infoinject import InfoInjector
-
-@InfoInjector.add_instruction(line=1, debug_mode="info", debug_context="generic", args_for_logger=(
-	f"n = {InfoInjector.VariableReference('n')}",
-))
-@InfoInjector.add_instruction(line=2, debug_mode="detail", debug_context="generic", args_for_logger=(
-	f"n is", "less than or equal to 1"
-),
-	end="\n.\n"
-)
-@InfoInjector.add_instruction(line=4, debug_mode="info", debug_context="generic", args_for_logger=(
-	f"n is greater than 1",
-	f"Now actually calculating... n-1 and n-2"
-))
-@InfoInjector.inject(globals(), locals())
-def fib(n):
-	if n <= 1:
-		return n
-	else:
-		return fib(n-1) + fib(n-2)
-
-fib(5)
-```
-## V0.01 released on 16th/5/2024
-init
+Metadata-Version: 2.1
+Name: plsp
+Version: 0.2
+Summary: A simple, easy to use, and powerful logging library for Python.
+Author: matrikater (Joel Watson)
+Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Requires-Dist: templated_setup
+
+# Please Log Shit Please (or `plsp`)
+
+## Notes
+
+```text
+info inject is a module allowing you to compile python source code with added debug information.
+this means that the interesting parts of the code stay separate from printing and other debug code.
+```
+
+```text
+=====================
+Pieces of the puzzle.
+=====================
+
+Logger 			- The piece that does the logging.
+
+DebugContext 		- Use this along side with the logger to separate different areas of an application.
+			- For example, you may have a rendering context and a physics context inside a game engine.
+
+DebugMode 		- Use this to specify different levels of debug information.
+			- For example, you may have a "info" mode and a "detail" mode.
+			- If the "info" mode is active, any messages that are in the "detail" mode will not be printed.
+			- This is because the "detail" mode extends from the "info" mode.
+			- If the "detail" mode is active, any messages that are in the "info"
+			-   and "detail" mode will be printed.
+
+ColorConfiguration 	- Use this to specify the colors of the debug information.
+			- For example, you may want to have the rendering context to be in green
+			-   and the physics context to be in red.
+
+InfoInjector 		- The piece that injects the debug information into the source code.
+			- Uses the Logger to log the debug information.
+
+formatters/ 		- The pieces that format the debug information.
+			- For example, you may want to have the time of the debug information to
+			-   be formatted in a specific way.
+			- You may also want to have the caller of the debug information to be formatted in a specific way.
+			- The formatters may be added onto any specified debug context. Then, when the Logger is used
+			-   by said context, the formatters will be used to format the debug information.
+
+
+
+====================================
+How the pieces relate to each other.
+====================================
+
+> Nodes A that is down from node B means that A depends on, or is used by, B.
+
+	Logger
+	/ \
+	+  +--------------------+
+	|                       |
+	Debug Context           Debug Mode
+	/ \
+	+  +--------------------+
+	|                       |
+	Color Configuration     formatters/
+```
+
+## Usage
+
+```python
+from pls.Logger import plsp
+#from formatters import TimeFormatter, CallerFormatter
+from plsp.DebugMode import DebugMode
+from plsp.Direction import IODirection
+
+import sys
+
+# use below to separate log files based on debug mode instead of debug context.
+#plsp.set("io_based_on_mode", True)
+
+
+
+# The below sets the global context to generic.
+plsp.set("global_context", "generic")
+
+
+
+# Below is adding a debug context.
+# It is a bit more complicated than setting up debug contexts so you dont have to set all the parameters at once.
+plsp.add_debug_context("generic")
+plsp.add_debug_context("rendering")
+plsp.add_debug_context("physics")
+
+
+
+# Below is adding a debug mode.
+# You can:
+# - Use the `write_to_file` parameter to specify a file to write to.
+# - Use the `write_to_io` parameter to specify an io object to write to.
+# - Use the `separate` parameter to specify if this is a standalone debug mode, meaning, if this mode is active,
+#     the previous debug mode will not be active.
+plsp.add_debug_mode("info")
+plsp.add_debug_mode("detail")
+plsp.add_debug_mode("debug")
+plsp.add_debug_mode("error", separate=True)
+
+
+
+# START OF MODIFYING DEBUG CONTEXTS #
+
+# You may modify the debug contexts after they are created.
+# Access the debug context by using the `Logger.debug_contexts` dictionary.
+
+pls.get_debug_context("generic").set_can_ever_write(True)
+plsp.get_debug_context("generic").add_direction(IODirection(False, sys.stdout.fileno(), None))
+plsp.get_debug_context("rendering").set_can_ever_write(True)
+plsp.get_debug_context("rendering").add_direction(IODirection(False, sys.stdout.fileno(), None))
+plsp.get_debug_context("physics").set_can_ever_write(True)
+plsp.get_debug_context("physics").add_direction(IODirection(False, sys.stdout.fileno(), None))
+					       
+# The below will add the time before each log message.
+#plsp.get_debug_context("generic").add_format_layer(TimeFormatter)
+#plsp.get_debug_context("rendering").add_format_layer(TimeFormatter)
+#plsp.get_debug_context("physics").add_format_layer(TimeFormatter)
+#
+## The below will add which ever function called the log message.
+#plsp.get_debug_context("generic").add_format_layer(CallerFormatter)
+#plsp.get_debug_context("rendering").add_format_layer(CallerFormatter)
+#plsp.get_debug_context("physics").add_format_layer(CallerFormatter)
+#
+
+# END OF MODIFYING DEBUG CONTEXTS #
+
+
+
+# Now we can use the debug contexts to log messages.
+plsp.set_debug_mode("info")
+
+plsp().info("This is using the generic context.")
+plsp().info("It works since we set a global context.")
+
+
+
+class renderer:
+	def __init__(self):
+		plsp().rendering.detail("The rendering engine in this engine is pretty simple!")
+
+
+
+class physics:
+	def __init__(self):
+		plsp().physics.detail("The physics engine in this engine is pretty simple!")
+
+
+#my_renderer = renderer()
+my_physics = physics()
+
+plsp.set_debug_mode("detail")
+
+my_physics = physics()
+
+
+
+
+
+
+
+from plsp.infoinject import InfoInjector
+
+@InfoInjector.add_instruction(line=1, debug_mode="info", debug_context="generic", args_for_logger=(
+	f"n = {InfoInjector.VariableReference('n')}",
+))
+@InfoInjector.add_instruction(line=2, debug_mode="detail", debug_context="generic", args_for_logger=(
+	f"n is", "less than or equal to 1"
+),
+	end="\n.\n"
+)
+@InfoInjector.add_instruction(line=4, debug_mode="info", debug_context="generic", args_for_logger=(
+	f"n is greater than 1",
+	f"Now actually calculating... n-1 and n-2"
+))
+@InfoInjector.inject(globals(), locals())
+def fib(n):
+	if n <= 1:
+		return n
+	else:
+		return fib(n-1) + fib(n-2)
+
+fib(5)
+```
+## V0.2 released on 16th/5/2024
+added shared state feature that allows sharing `Logger` instance between separate processes.
```

### Comparing `plsp-0.1/README.md` & `plsp-0.2/plsp.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,182 +1,192 @@
-# Please Log Shit Please (or `plsp`)
-
-## Notes
-
-```text
-info inject is a module allowing you to compile python source code with added debug information.
-this means that the interesting parts of the code stay separate from printing and other debug code.
-```
-
-```text
-=====================
-Pieces of the puzzle.
-=====================
-
-Logger 			- The piece that does the logging.
-
-DebugContext 		- Use this along side with the logger to separate different areas of an application.
-			- For example, you may have a rendering context and a physics context inside a game engine.
-
-DebugMode 		- Use this to specify different levels of debug information.
-			- For example, you may have a "info" mode and a "detail" mode.
-			- If the "info" mode is active, any messages that are in the "detail" mode will not be printed.
-			- This is because the "detail" mode extends from the "info" mode.
-			- If the "detail" mode is active, any messages that are in the "info"
-			-   and "detail" mode will be printed.
-
-ColorConfiguration 	- Use this to specify the colors of the debug information.
-			- For example, you may want to have the rendering context to be in green
-			-   and the physics context to be in red.
-
-InfoInjector 		- The piece that injects the debug information into the source code.
-			- Uses the Logger to log the debug information.
-
-formatters/ 		- The pieces that format the debug information.
-			- For example, you may want to have the time of the debug information to
-			-   be formatted in a specific way.
-			- You may also want to have the caller of the debug information to be formatted in a specific way.
-			- The formatters may be added onto any specified debug context. Then, when the Logger is used
-			-   by said context, the formatters will be used to format the debug information.
-
-
-
-====================================
-How the pieces relate to each other.
-====================================
-
-> Nodes A that is down from node B means that A depends on, or is used by, B.
-
-	Logger
-	/ \
-	+  +--------------------+
-	|                       |
-	Debug Context           Debug Mode
-	/ \
-	+  +--------------------+
-	|                       |
-	Color Configuration     formatters/
-```
-
-## Usage
-
-```python
-from pls.Logger import plsp
-#from formatters import TimeFormatter, CallerFormatter
-from plsp.DebugMode import DebugMode
-from plsp.Direction import IODirection
-
-import sys
-
-# use below to separate log files based on debug mode instead of debug context.
-#plsp.set("io_based_on_mode", True)
-
-
-
-# The below sets the global context to generic.
-plsp.set("global_context", "generic")
-
-
-
-# Below is adding a debug context.
-# It is a bit more complicated than setting up debug contexts so you dont have to set all the parameters at once.
-plsp.add_debug_context("generic")
-plsp.add_debug_context("rendering")
-plsp.add_debug_context("physics")
-
-
-
-# Below is adding a debug mode.
-# You can:
-# - Use the `write_to_file` parameter to specify a file to write to.
-# - Use the `write_to_io` parameter to specify an io object to write to.
-# - Use the `separate` parameter to specify if this is a standalone debug mode, meaning, if this mode is active,
-#     the previous debug mode will not be active.
-plsp.add_debug_mode("info")
-plsp.add_debug_mode("detail")
-plsp.add_debug_mode("debug")
-plsp.add_debug_mode("error", separate=True)
-
-
-
-# START OF MODIFYING DEBUG CONTEXTS #
-
-# You may modify the debug contexts after they are created.
-# Access the debug context by using the `Logger.debug_contexts` dictionary.
-
-pls.get_debug_context("generic").set_can_ever_write(True)
-plsp.get_debug_context("generic").add_direction(IODirection(False, sys.stdout.fileno(), None))
-plsp.get_debug_context("rendering").set_can_ever_write(True)
-plsp.get_debug_context("rendering").add_direction(IODirection(False, sys.stdout.fileno(), None))
-plsp.get_debug_context("physics").set_can_ever_write(True)
-plsp.get_debug_context("physics").add_direction(IODirection(False, sys.stdout.fileno(), None))
-					       
-# The below will add the time before each log message.
-#plsp.get_debug_context("generic").add_format_layer(TimeFormatter)
-#plsp.get_debug_context("rendering").add_format_layer(TimeFormatter)
-#plsp.get_debug_context("physics").add_format_layer(TimeFormatter)
-#
-## The below will add which ever function called the log message.
-#plsp.get_debug_context("generic").add_format_layer(CallerFormatter)
-#plsp.get_debug_context("rendering").add_format_layer(CallerFormatter)
-#plsp.get_debug_context("physics").add_format_layer(CallerFormatter)
-#
-
-# END OF MODIFYING DEBUG CONTEXTS #
-
-
-
-# Now we can use the debug contexts to log messages.
-plsp.set_debug_mode("info")
-
-plsp().info("This is using the generic context.")
-plsp().info("It works since we set a global context.")
-
-
-
-class renderer:
-	def __init__(self):
-		plsp().rendering.detail("The rendering engine in this engine is pretty simple!")
-
-
-
-class physics:
-	def __init__(self):
-		plsp().physics.detail("The physics engine in this engine is pretty simple!")
-
-
-#my_renderer = renderer()
-my_physics = physics()
-
-plsp.set_debug_mode("detail")
-
-my_physics = physics()
-
-
-
-
-
-
-
-from plsp.infoinject import InfoInjector
-
-@InfoInjector.add_instruction(line=1, debug_mode="info", debug_context="generic", args_for_logger=(
-	f"n = {InfoInjector.VariableReference('n')}",
-))
-@InfoInjector.add_instruction(line=2, debug_mode="detail", debug_context="generic", args_for_logger=(
-	f"n is", "less than or equal to 1"
-),
-	end="\n.\n"
-)
-@InfoInjector.add_instruction(line=4, debug_mode="info", debug_context="generic", args_for_logger=(
-	f"n is greater than 1",
-	f"Now actually calculating... n-1 and n-2"
-))
-@InfoInjector.inject(globals(), locals())
-def fib(n):
-	if n <= 1:
-		return n
-	else:
-		return fib(n-1) + fib(n-2)
-
-fib(5)
-```
+Metadata-Version: 2.1
+Name: plsp
+Version: 0.2
+Summary: A simple, easy to use, and powerful logging library for Python.
+Author: matrikater (Joel Watson)
+Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Requires-Dist: templated_setup
+
+# Please Log Shit Please (or `plsp`)
+
+## Notes
+
+```text
+info inject is a module allowing you to compile python source code with added debug information.
+this means that the interesting parts of the code stay separate from printing and other debug code.
+```
+
+```text
+=====================
+Pieces of the puzzle.
+=====================
+
+Logger 			- The piece that does the logging.
+
+DebugContext 		- Use this along side with the logger to separate different areas of an application.
+			- For example, you may have a rendering context and a physics context inside a game engine.
+
+DebugMode 		- Use this to specify different levels of debug information.
+			- For example, you may have a "info" mode and a "detail" mode.
+			- If the "info" mode is active, any messages that are in the "detail" mode will not be printed.
+			- This is because the "detail" mode extends from the "info" mode.
+			- If the "detail" mode is active, any messages that are in the "info"
+			-   and "detail" mode will be printed.
+
+ColorConfiguration 	- Use this to specify the colors of the debug information.
+			- For example, you may want to have the rendering context to be in green
+			-   and the physics context to be in red.
+
+InfoInjector 		- The piece that injects the debug information into the source code.
+			- Uses the Logger to log the debug information.
+
+formatters/ 		- The pieces that format the debug information.
+			- For example, you may want to have the time of the debug information to
+			-   be formatted in a specific way.
+			- You may also want to have the caller of the debug information to be formatted in a specific way.
+			- The formatters may be added onto any specified debug context. Then, when the Logger is used
+			-   by said context, the formatters will be used to format the debug information.
+
+
+
+====================================
+How the pieces relate to each other.
+====================================
+
+> Nodes A that is down from node B means that A depends on, or is used by, B.
+
+	Logger
+	/ \
+	+  +--------------------+
+	|                       |
+	Debug Context           Debug Mode
+	/ \
+	+  +--------------------+
+	|                       |
+	Color Configuration     formatters/
+```
+
+## Usage
+
+```python
+from pls.Logger import plsp
+#from formatters import TimeFormatter, CallerFormatter
+from plsp.DebugMode import DebugMode
+from plsp.Direction import IODirection
+
+import sys
+
+# use below to separate log files based on debug mode instead of debug context.
+#plsp.set("io_based_on_mode", True)
+
+
+
+# The below sets the global context to generic.
+plsp.set("global_context", "generic")
+
+
+
+# Below is adding a debug context.
+# It is a bit more complicated than setting up debug contexts so you dont have to set all the parameters at once.
+plsp.add_debug_context("generic")
+plsp.add_debug_context("rendering")
+plsp.add_debug_context("physics")
+
+
+
+# Below is adding a debug mode.
+# You can:
+# - Use the `write_to_file` parameter to specify a file to write to.
+# - Use the `write_to_io` parameter to specify an io object to write to.
+# - Use the `separate` parameter to specify if this is a standalone debug mode, meaning, if this mode is active,
+#     the previous debug mode will not be active.
+plsp.add_debug_mode("info")
+plsp.add_debug_mode("detail")
+plsp.add_debug_mode("debug")
+plsp.add_debug_mode("error", separate=True)
+
+
+
+# START OF MODIFYING DEBUG CONTEXTS #
+
+# You may modify the debug contexts after they are created.
+# Access the debug context by using the `Logger.debug_contexts` dictionary.
+
+pls.get_debug_context("generic").set_can_ever_write(True)
+plsp.get_debug_context("generic").add_direction(IODirection(False, sys.stdout.fileno(), None))
+plsp.get_debug_context("rendering").set_can_ever_write(True)
+plsp.get_debug_context("rendering").add_direction(IODirection(False, sys.stdout.fileno(), None))
+plsp.get_debug_context("physics").set_can_ever_write(True)
+plsp.get_debug_context("physics").add_direction(IODirection(False, sys.stdout.fileno(), None))
+					       
+# The below will add the time before each log message.
+#plsp.get_debug_context("generic").add_format_layer(TimeFormatter)
+#plsp.get_debug_context("rendering").add_format_layer(TimeFormatter)
+#plsp.get_debug_context("physics").add_format_layer(TimeFormatter)
+#
+## The below will add which ever function called the log message.
+#plsp.get_debug_context("generic").add_format_layer(CallerFormatter)
+#plsp.get_debug_context("rendering").add_format_layer(CallerFormatter)
+#plsp.get_debug_context("physics").add_format_layer(CallerFormatter)
+#
+
+# END OF MODIFYING DEBUG CONTEXTS #
+
+
+
+# Now we can use the debug contexts to log messages.
+plsp.set_debug_mode("info")
+
+plsp().info("This is using the generic context.")
+plsp().info("It works since we set a global context.")
+
+
+
+class renderer:
+	def __init__(self):
+		plsp().rendering.detail("The rendering engine in this engine is pretty simple!")
+
+
+
+class physics:
+	def __init__(self):
+		plsp().physics.detail("The physics engine in this engine is pretty simple!")
+
+
+#my_renderer = renderer()
+my_physics = physics()
+
+plsp.set_debug_mode("detail")
+
+my_physics = physics()
+
+
+
+
+
+
+
+from plsp.infoinject import InfoInjector
+
+@InfoInjector.add_instruction(line=1, debug_mode="info", debug_context="generic", args_for_logger=(
+	f"n = {InfoInjector.VariableReference('n')}",
+))
+@InfoInjector.add_instruction(line=2, debug_mode="detail", debug_context="generic", args_for_logger=(
+	f"n is", "less than or equal to 1"
+),
+	end="\n.\n"
+)
+@InfoInjector.add_instruction(line=4, debug_mode="info", debug_context="generic", args_for_logger=(
+	f"n is greater than 1",
+	f"Now actually calculating... n-1 and n-2"
+))
+@InfoInjector.inject(globals(), locals())
+def fib(n):
+	if n <= 1:
+		return n
+	else:
+		return fib(n-1) + fib(n-2)
+
+fib(5)
+```
+## V0.2 released on 16th/5/2024
+added shared state feature that allows sharing `Logger` instance between separate processes.
```

### Comparing `plsp-0.1/plsp/DebugContext.py` & `plsp-0.2/plsp/DebugContext.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,177 +1,181 @@
-import sys
-from .DebugMode import DebugMode
-from .formatters.Formatter import IFormatter
-from .formatters.FinalFormatter import IFinalFormatter
-from .formatters.defaults import DefaultFinalFormatter
-from .Direction import IODirection
-
-from io import IOBase, TextIOWrapper
-import base64
-
-
-
-
-
-
-
-def _debug_print(self, prefix:str, *args, **kwargs):
-
-	"""
-	DO NOT CALL THIS DIRECTLY.
-
-	At the end of the day, this is our special function that actually prints to the screen (or file).
-
-	Args:
-		prefix (str): 	The prefix to the log message.
-		*args: 		The log message, works like the `print` function.
-		**kwargs: 	The keyword arguments to pass to the print function.
-				  Currently, only the `end` keyword argument is supported.
-
-	Raises:
-	    Exception: If an unknown keyword argument is passed.
-	"""
-
-	str = f"{prefix}"
-	for arg in args:
-		str += f"{arg} "
-	str += "\033[0m"
-
-	for kwarg in kwargs:
-		if kwarg == "end":
-			continue
-		else:
-			raise Exception(f"Unknown keyword argument {kwarg}.")
-
-	if "end" in kwargs:
-		str += kwargs["end"]
-
-	self._add_contents_to_log(str)
-
-
-
-
-
-
-
-class DebugContext:
-
-
-
-	def __init__(self, name:str) -> None:
-		self.format_layers:"list[IFormatter]" = []
-		self.final_formatter:"IFinalFormatter" = DefaultFinalFormatter()
-
-		self.can_ever_write:"bool|None" = None
-		self.directions:"list[IODirection]|None" = None
-
-
-
-	def set_final_formatter(self, formatter:"IFinalFormatter") -> None:
-		self.final_formatter = formatter
-
-
-
-	def set_can_ever_write(self, can_ever_write:bool) -> None:
-		self.can_ever_write = can_ever_write
-
-
-
-	def add_direction(self, direction:IODirection) -> None:
-		if self.directions is None:
-			self.directions = []
-		self.directions.append(direction)
-
-
-
-	def add_format_layer(self, formatter):
-		self.format_layers.append(formatter)
-
-
-
-
-	def _evaluate_instruction(self, instruction_part, arg_part):
-		if instruction_part == "can_ever_write":
-			self.can_ever_write = eval(arg_part)
-		
-		elif instruction_part == "write_to_handle":
-			self.write_to_handle = eval(arg_part)
-
-		elif instruction_part == "write_to_file":
-			self.write_to_file = eval(arg_part)
-
-
-
-	def __add_contents_to_log(self, contents:str, direction: IODirection) -> None:
-		try:
-
-			f = None
-
-			direction.validate()
-
-			if direction.file_handle is not None:
-				if direction.file_handle == 1:
-					f = sys.stdout
-				elif direction.file_handle == 2:
-					f = sys.stderr
-				else:
-					f = open(direction.file_handle, "a")
-			elif direction.file_path is not None:
-				f = open(direction.file_path, "a")
-			else:
-				raise Exception("No file handle or file path to write to.")
-
-			if not isinstance(f, IOBase):
-				raise Exception("No file handle to write to.")
-			
-			f.write(contents)
-			f.write("\n")
-
-		finally:
-			if f and (not direction.file_handle in [1,2]) and not f.closed:
-				f.close()
-
-
-
-	def _add_contents_to_log(self, contents:str) -> None:
-		assert self.directions is not None, "No directions to write to."
-		for direction in self.directions:
-			self.__add_contents_to_log(contents, direction)
-
-
-
-	def handle(self, debug_mode:"DebugMode", active_debug_level:"DebugMode", *args, **kwargs):
-		# QUICK NOTE: the `debug_mode` parameter should be used to change the output and the
-		# `active_debug_mode` parameter should be used to determine if we should write to the output.
-
-		# First check that this context is valid.
-		if self.can_ever_write is None and self.write_to_handle is None:
-			raise Exception("`can_ever_write` and `write_to_handle` cannot both be None.")
-
-		str = ""
-		
-		for format_layer in self.format_layers:
-			str = format_layer.handle(str)
-		
-		str = self.final_formatter.raw_handle(str)
-		
-		override_instructions = debug_mode.override_instructions or []
-
-		for instruction in override_instructions:
-			instruction_part, arg_part = instruction.split("=")
-			self._evaluate_instruction(instruction_part, arg_part)
-
-		# All conditions where we cannot write.
-		if active_debug_level.level == -1 and debug_mode.level == -1:
-			if not active_debug_level.name == debug_mode.name:
-				return
-		elif active_debug_level.level < debug_mode.level:
-			return
-		elif self.can_ever_write is None or (self.can_ever_write is not None and not self.can_ever_write):
-			return
-
-		if active_debug_level.level >= debug_mode.level:
-			_debug_print(self, str, *args, **kwargs)
-			return
-
-		raise Exception("This should never happen.")
-			
+import sys
+from .DebugMode import DebugMode
+from .formatters.Formatter import IFormatter
+from .formatters.FinalFormatter import IFinalFormatter
+from .formatters.defaults import DefaultFinalFormatter
+from .Direction import IODirection
+
+from io import IOBase, TextIOWrapper
+import base64
+
+
+
+
+
+
+
+def _debug_print(self, prefix:str, *args, **kwargs):
+
+	"""
+	DO NOT CALL THIS DIRECTLY.
+
+	At the end of the day, this is our special function that actually prints to the screen (or file).
+
+	Args:
+		prefix (str): 	The prefix to the log message.
+		*args: 		The log message, works like the `print` function.
+		**kwargs: 	The keyword arguments to pass to the print function.
+				  Currently, only the `end` keyword argument is supported.
+
+	Raises:
+	    Exception: If an unknown keyword argument is passed.
+	"""
+
+	str = f"{prefix}"
+	for arg in args:
+		str += f"{arg} "
+	str += "\033[0m"
+
+	for kwarg in kwargs:
+		if kwarg == "end":
+			continue
+		else:
+			raise Exception(f"Unknown keyword argument {kwarg}.")
+
+	if "end" in kwargs:
+		str += kwargs["end"]
+
+	self._add_contents_to_log(str)
+
+
+
+
+
+
+
+class DebugContext:
+
+
+
+	def __init__(self, name:str) -> None:
+		self.name = name
+
+		self.format_layers:"list[IFormatter]" = []
+		self.final_formatter:"IFinalFormatter" = DefaultFinalFormatter()
+
+		self.can_ever_write:"bool|None" = None
+		self.directions:"list[IODirection]|None" = None
+
+
+
+	def set_final_formatter(self, formatter:"IFinalFormatter") -> None:
+		self.final_formatter = formatter
+
+
+
+	def set_can_ever_write(self, can_ever_write:bool) -> None:
+		self.can_ever_write = can_ever_write
+
+
+
+	def add_direction(self, direction:IODirection) -> None:
+		if self.directions is None:
+			self.directions = []
+		self.directions.append(direction)
+
+
+
+	def add_format_layer(self, formatter):
+		self.format_layers.append(formatter)
+
+
+
+
+	def _evaluate_instruction(self, instruction_part, arg_part):
+		if instruction_part == "can_ever_write":
+			self.can_ever_write = eval(arg_part)
+		
+		elif instruction_part == "write_to_handle":
+			self.write_to_handle = eval(arg_part)
+
+		elif instruction_part == "write_to_file":
+			self.write_to_file = eval(arg_part)
+
+
+
+	def __add_contents_to_log(self, contents:str, direction: IODirection) -> None:
+		try:
+
+			f = None
+
+			direction.validate()
+
+			if direction.file_handle is not None:
+				if direction.file_handle == 1:
+					f = sys.stdout
+				elif direction.file_handle == 2:
+					f = sys.stderr
+				else:
+					f = open(direction.file_handle, "a")
+			elif direction.file_path is not None:
+				f = open(direction.file_path, "a")
+			else:
+				raise Exception("No file handle or file path to write to.")
+
+			if not isinstance(f, IOBase):
+				raise Exception("No file handle to write to.")
+			
+			f.write(contents)
+			f.write("\n")
+
+		finally:
+			if f and (not direction.file_handle in [1,2]) and not f.closed:
+				f.close()
+
+
+
+	def _add_contents_to_log(self, contents:str) -> None:
+		assert self.directions is not None, "No directions to write to."
+		for direction in self.directions:
+			self.__add_contents_to_log(contents, direction)
+
+
+
+	def handle(self, debug_mode:"DebugMode", active_debug_level:"DebugMode", *args, **kwargs):
+		# QUICK NOTE: the `debug_mode` parameter should be used to change the output and the
+		# `active_debug_mode` parameter should be used to determine if we should write to the output.
+
+		# First check that this context is valid.
+		if self.can_ever_write is None and self.write_to_handle is None:
+			raise Exception("`can_ever_write` and `write_to_handle` cannot both be None.")
+
+		str = ""
+		
+		is_first = True
+		for format_layer in self.format_layers:
+			str = IFormatter.handle(format_layer, str, is_first)
+			is_first = False
+		
+		str = self.final_formatter.raw_handle(str)
+		
+		override_instructions = debug_mode.override_instructions or []
+
+		for instruction in override_instructions:
+			instruction_part, arg_part = instruction.split("=")
+			self._evaluate_instruction(instruction_part, arg_part)
+
+		# All conditions where we cannot write.
+		if active_debug_level.level == -1 and debug_mode.level == -1:
+			if not active_debug_level.name == debug_mode.name:
+				return
+		elif active_debug_level.level < debug_mode.level:
+			return
+		elif self.can_ever_write is None or (self.can_ever_write is not None and not self.can_ever_write):
+			return
+
+		if active_debug_level.level >= debug_mode.level:
+			_debug_print(self, str, *args, **kwargs)
+			return
+
+		raise Exception("This should never happen.")
+
```

### Comparing `plsp-0.1/plsp/DebugMode.py` & `plsp-0.2/plsp/DebugMode.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-import dataclasses
-
-
-
-
-
-
-
-@dataclasses.dataclass
-class DebugMode:
-
-
-
-	name: str
-	level: int
-	override_instructions: "list[str]|None"
-
-
-
-	def set_override_do_ever_write(self, do_ever_write: bool) -> None:
-		if self.override_instructions is None:
-			self.override_instructions = []
-		self.override_instructions.append(
-			f"do_ever_write={'None' if do_ever_write is None else do_ever_write}"
-		)
-	
-
-
-	def set_override_write_to_handle(self, file_handle: "int|None") -> None:
-		if self.override_instructions is None:
-			self.override_instructions = []
-		self.override_instructions.append(
-			f"write_to_handle={'None' if file_handle is None else str(file_handle)}"
-		)
-
-
-	
-	def set_override_write_to_file(self, file_name: "str|None") -> None:
-		if self.override_instructions is None:
-			self.override_instructions = []
-		self.override_instructions.append(
-			f"write_to_file={'None' if file_name is None else file_name}"
-		)
+import dataclasses
+
+
+
+
+
+
+
+@dataclasses.dataclass
+class DebugMode:
+
+
+
+	name: str
+	level: int
+	override_instructions: "list[str]|None"
+
+
+
+	def set_override_do_ever_write(self, do_ever_write: bool) -> None:
+		if self.override_instructions is None:
+			self.override_instructions = []
+		self.override_instructions.append(
+			f"do_ever_write={'None' if do_ever_write is None else do_ever_write}"
+		)
+	
+
+
+	def set_override_write_to_handle(self, file_handle: "int|None") -> None:
+		if self.override_instructions is None:
+			self.override_instructions = []
+		self.override_instructions.append(
+			f"write_to_handle={'None' if file_handle is None else str(file_handle)}"
+		)
+
+
+	
+	def set_override_write_to_file(self, file_name: "str|None") -> None:
+		if self.override_instructions is None:
+			self.override_instructions = []
+		self.override_instructions.append(
+			f"write_to_file={'None' if file_name is None else file_name}"
+		)
```

### Comparing `plsp-0.1/plsp/Logger.py` & `plsp-0.2/plsp/Logger.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,320 +1,334 @@
-from .DebugContext import DebugContext, DebugMode
-
-from typing import Any
-
-
-
-
-
-
-
-DYNAMIC_PIE = {}
-class DynamicVariableContainer:
-
-
-
-	"""
-	Represents a container for dynamically managing variables.
-
-	This class allows you to dynamically set and retrieve variables without explicitly defining them in the class definition.
-
-	Usage:
-	```python
-	# Create a DynamicVariableContainer instance
-	container = DynamicVariableContainer("container1")
-
-	# Dynamically set a variable in the container
-	container.set("variable1", 10)
-
-	# Dynamically get the value of a variable from the container
-	value = container.variable1
-	print(value)  # Output: 10
-
-	# Dynamically get all the variables in the container
-	variables = container.get_children()
-
-	# Dynamically delete a variable from the container
-	container.del("variable1")
-	```
-
-	Attributes:
-		name (str): The name of the container.
-
-	Notes on the hackiness of this class:
-	- This class uses a global dictionary to store the variables.
-	- This class uses a static method to set and delete the variables, among other things.
-
-	Because of this, please DO NOT EVER call the static methods directly.
-	Instead, use the `set`, `del`, and `get_children` methods of the instance of this class.
-	Beware that you will not get good intellisense support but it WILL work, trust me bro. ^_^
-	"""
-
-
-
-	def __init__(self, name):
-		global DYNAMIC_PIE
-
-		self.name = name
-
-		DYNAMIC_PIE[name] = {}
-		DynamicVariableContainer._post_setup(name)
-	
-
-
-	@staticmethod
-	def _post_setup(__name:str):
-		global DYNAMIC_PIE
-
-		def __wrapper_for_set(*args, **kwargs):
-			DynamicVariableContainer._set(__name, *args, **kwargs)
-
-		def __wrapper_for_del(*args, **kwargs):
-			DynamicVariableContainer._del(__name, *args, **kwargs)
-
-		def __wrapper_for_get_children(*args, **kwargs):
-			return DynamicVariableContainer._get_children(__name, *args, **kwargs)
-
-		def __wrapper_for_get_name(*args, **kwargs):
-			return DynamicVariableContainer._get_name(__name, *args, **kwargs)
-
-		DYNAMIC_PIE[__name]["set"] = __wrapper_for_set
-		DYNAMIC_PIE[__name]["del"] = __wrapper_for_del
-		DYNAMIC_PIE[__name]["get_children"] = __wrapper_for_get_children
-		DYNAMIC_PIE[__name]["get_name"] = __wrapper_for_get_name
-	
-
-
-	@staticmethod
-	def _set(__name_of_self:str, name: str, value) -> None:
-		global DYNAMIC_PIE
-
-		name_of_self = __name_of_self
-		piece_of_pie = DYNAMIC_PIE[name_of_self]
-
-		piece_of_pie[name] = value
-
-
-
-	@staticmethod
-	def _del(__name_of_self:str, name: str) -> None:
-		global DYNAMIC_PIE
-
-		name_of_self = __name_of_self
-		piece_of_pie = DYNAMIC_PIE[name_of_self]
-
-		del piece_of_pie[name]
-
-
-
-	@staticmethod
-	def _get_children(__name_of_self:str) -> dict:
-		global DYNAMIC_PIE
-
-		name_of_self = __name_of_self
-		piece_of_pie = DYNAMIC_PIE[name_of_self]
-
-		return piece_of_pie
-	
-
-
-	@staticmethod
-	def _get_name(__name_of_self:str) -> str:
-		return __name_of_self
-
-
-
-	def __getattribute__(self, __name: str):
-		global DYNAMIC_PIE
-
-		name_of_self = super().__getattribute__("name")
-		piece_of_pie = DYNAMIC_PIE[name_of_self]
-
-		if __name in piece_of_pie:
-			return piece_of_pie[__name]
-		
-		err_str = f"'{name_of_self}' object has no attribute '{__name}'"
-		raise AttributeError(err_str)
-
-
-
-
-
-
-
-class Logger:
-
-
-
-	"""
-	The actual meat and potatoes of the logging system.
-	"""
-
-
-
-	def __init__(self) -> None:
-		"""
-		YOU MUST NEVER CALL THIS DIRECTLY.
-
-		Raises:
-		    Exception: If the Logger is already initialized. Hence why i said never call this directly.
-
-		Side Effects:
-		- Adds a "disabled" debug mode to the system.
-		"""
-		global plsp
-
-		try:
-			if plsp is not None:
-				raise Exception("Logger already initialized")
-		except NameError:
-			pass
-		plsp = self
-
-		self.configuration_vars = {}
-		self.debug_modes:"dict[str,DebugMode]" = {}
-		self.debug_contexts = {}
-		self.active_debug_mode = None
-
-		self.LOGGER_HELPER = DynamicVariableContainer("LOGGER_HELPER")
-
-		plsp._add_debug_mode("disabled", 0)
-		plsp.get_debug_mode("disabled").set_override_do_ever_write(False)
-
-
-	
-	def __call__(self, *args: Any, **kwds: Any) -> Any:
-		return self.LOGGER_HELPER
-
-
-
-	def set_debug_mode(self, name:"str") -> None:
-		"""
-		Sets the active debug mode.
-
-		Args:
-		    name (str): The name of the debug mode to set as active.
-		"""
-		self.active_debug_mode = self.debug_modes[name]
-
-
-
-	def _add_debug_mode(self, name:"str", level:"int"):
-		"""
-		YOU MUST NEVER CALL THIS DIRECTLY.
-
-		This is an inner function used by the `add_debug_mode` method (note without the underscore).
-		"""
-
-		# Check that the name isn't already in use.
-		if name in self.debug_modes:
-			raise Exception(f"Debug mode {name} already exists.")
-
-		# Construct the debug mode.
-		self.debug_modes[name] = DebugMode(name, level, None)
-
-		self._update_state_after_adding_debug_mode(
-			name,
-			level
-		)
-
-	
-
-	def _update_state_after_adding_debug_mode(self, name_of_debug_mode, level):
-		# The below wrapper is what actually gets called when you do `plsp().<insert name of debug mode>(...)`
-		# NOTE: Remember, this is only for the global context.
-		def wrapper_for_global_handler(*args, **kwargs):
-			context = self.debug_contexts[self.configuration_vars["global_context"]]
-			mode = self.debug_modes[name_of_debug_mode]
-			context.handle(mode, self.active_debug_mode, *args, **kwargs)
-
-		# And here is the wrapper for when we specify a context.
-		# E.g., `plsp().our_context.our_debug_mode(...)`...
-		# This wrapper is the `our_debug_mode` part.
-		# The actual `our_context` is made in the `add_debug_context` method and it is a `DynamicVariableContainer`
-		#  instance that is a child of the `LOGGER_HELPER` instance.
-		def wrapper_for_context_specified_handler(context, *args, **kwargs):
-			mode = self.debug_modes[name_of_debug_mode]
-			context.handle(mode, self.active_debug_mode, *args, **kwargs)
-
-		# We only want to use the `wrapper_for_global_handler` if the global context is set.
-		if self.configuration_vars.get("global_context") is not None:
-			self.LOGGER_HELPER.set(name_of_debug_mode, wrapper_for_global_handler)
-
-		# Now to update the context-specific wrappers.
-		keys_no_globals = [k for k in self.LOGGER_HELPER.get_children().keys() if k not in self.debug_modes.keys()]
-		keys_no_globals = [k for k in keys_no_globals if k not in ["set", "del", "get_children", "get_name"]]
-		for child_key in keys_no_globals:
-			container = self.LOGGER_HELPER.get_children()[child_key]
-			def _wrapper_for_the_wrapper(*args, **kwargs):
-				nonlocal container
-				context = self.debug_contexts[container.get_name()]
-				wrapper_for_context_specified_handler(context, *args, **kwargs)
-			container.set(name_of_debug_mode, _wrapper_for_the_wrapper)
-
-
-
-	def add_debug_mode(self, name:"str", separate=False):
-		"""
-		Adds a debug mode to the system.
-
-		Args:
-		    name (str): The name of the debug mode.
-		
-		Optional Keyword Args:
-		- write_to_file (str|None): 	The file to write to (if any).
-		- write_to_io (int|None): 	The io object to write to (if any).
-		- separate (bool): 		If this is a standalone debug mode, meaning, if this mode is active,
-					  	  all other debug mode will not be active.
-
-		NOTE: You must specify at least one of `write_to_file` or `write_to_io`.
-		"""
-
-		if separate:
-			level = -1
-		else:
-			level = len(self.debug_modes)+1
-
-		self._add_debug_mode(name, level)
-
-
-
-	def add_debug_context(self, name:"str"):
-		if name in self.debug_contexts:
-			raise Exception(f"Debug context {name} already exists.")
-		self.debug_contexts[name] = DebugContext(name)
-		self.LOGGER_HELPER.set(name, DynamicVariableContainer(name))
-
-
-
-	def get_debug_context(self, name:"str") -> "DebugContext":
-		return self.debug_contexts[name]
-	
-
-
-	def get_debug_mode(self, name:"str") -> "DebugMode":
-		return self.debug_modes[name]
-
-
-
-	def set(self, name:"str", value) -> None:
-		accepted_vars = ["global_context"]
-
-		if name not in accepted_vars:
-			raise Exception(f"Variable {name} not accepted.")
-
-		self.configuration_vars[name] = value
-
-
-
-
-
-
-
-"""
-Below is the Logger global variable.
-We are doing things a bit different.
-
-We are using the `pls` as a singleton class of `Logger`.
-Its a bit of a hack but it makes the usage of this API pretty nice.
-"""
-plsp:"Logger" = Logger()
+from .DebugContext import DebugContext, DebugMode
+
+from pickle import dumps as pickle_X_dumps
+from pickle import loads as pickle_X_loads
+from typing import Any
+
+
+
+
+
+
+
+DYNAMIC_PIE = {}
+class DynamicVariableContainer:
+
+
+
+	"""
+	Represents a container for dynamically managing variables.
+
+	This class allows you to dynamically set and retrieve variables without explicitly defining them in the class definition.
+
+	Usage:
+	```python
+	# Create a DynamicVariableContainer instance
+	container = DynamicVariableContainer("container1")
+
+	# Dynamically set a variable in the container
+	container.set("variable1", 10)
+
+	# Dynamically get the value of a variable from the container
+	value = container.variable1
+	print(value)  # Output: 10
+
+	# Dynamically get all the variables in the container
+	variables = container.get_children()
+
+	# Dynamically delete a variable from the container
+	container.del("variable1")
+	```
+
+	Attributes:
+		name (str): The name of the container.
+
+	Notes on the hackiness of this class:
+	- This class uses a global dictionary to store the variables.
+	- This class uses a static method to set and delete the variables, among other things.
+
+	Because of this, please DO NOT EVER call the static methods directly.
+	Instead, use the `set`, `del`, and `get_children` methods of the instance of this class.
+	Beware that you will not get good intellisense support but it WILL work, trust me bro. ^_^
+	"""
+
+
+
+	def __init__(self, name):
+		global DYNAMIC_PIE
+
+		self.name = name
+
+		DYNAMIC_PIE[name] = {}
+		DynamicVariableContainer._post_setup(name)
+	
+
+
+	@staticmethod
+	def _post_setup(__name:str):
+		global DYNAMIC_PIE
+
+		def __wrapper_for_set(*args, **kwargs):
+			DynamicVariableContainer._set(__name, *args, **kwargs)
+
+		def __wrapper_for_del(*args, **kwargs):
+			DynamicVariableContainer._del(__name, *args, **kwargs)
+
+		def __wrapper_for_get_children(*args, **kwargs):
+			return DynamicVariableContainer._get_children(__name, *args, **kwargs)
+
+		def __wrapper_for_get_name(*args, **kwargs):
+			return DynamicVariableContainer._get_name(__name, *args, **kwargs)
+
+		DYNAMIC_PIE[__name]["set"] = __wrapper_for_set
+		DYNAMIC_PIE[__name]["del"] = __wrapper_for_del
+		DYNAMIC_PIE[__name]["get_children"] = __wrapper_for_get_children
+		DYNAMIC_PIE[__name]["get_name"] = __wrapper_for_get_name
+	
+
+
+	@staticmethod
+	def _set(__name_of_self:str, name: str, value) -> None:
+		global DYNAMIC_PIE
+
+		name_of_self = __name_of_self
+		piece_of_pie = DYNAMIC_PIE[name_of_self]
+
+		piece_of_pie[name] = value
+
+
+
+	@staticmethod
+	def _del(__name_of_self:str, name: str) -> None:
+		global DYNAMIC_PIE
+
+		name_of_self = __name_of_self
+		piece_of_pie = DYNAMIC_PIE[name_of_self]
+
+		del piece_of_pie[name]
+
+
+
+	@staticmethod
+	def _get_children(__name_of_self:str) -> dict:
+		global DYNAMIC_PIE
+
+		name_of_self = __name_of_self
+		piece_of_pie = DYNAMIC_PIE[name_of_self]
+
+		return piece_of_pie
+	
+
+
+	@staticmethod
+	def _get_name(__name_of_self:str) -> str:
+		return __name_of_self
+
+
+
+	def __getattribute__(self, __name: str):
+		global DYNAMIC_PIE
+
+		name_of_self = super().__getattribute__("name")
+		piece_of_pie = DYNAMIC_PIE[name_of_self]
+
+		if __name in piece_of_pie:
+			return piece_of_pie[__name]
+		
+		err_str = f"'{name_of_self}' object has no attribute '{__name}'"
+		raise AttributeError(err_str)
+
+
+
+
+
+
+
+class Logger:
+
+
+
+	"""
+	The actual meat and potatoes of the logging system.
+	"""
+
+
+
+	@staticmethod
+	def _pickle_dump(inst) -> "dict":	
+		return {
+			"configuration_vars": pickle_X_dumps(inst.configuration_vars),
+			"debug_modes": pickle_X_dumps(inst.debug_modes),
+			"debug_contexts": pickle_X_dumps(inst.debug_contexts),
+			"active_debug_mode": pickle_X_dumps(inst.active_debug_mode)
+		}
+
+
+
+	@staticmethod
+	def _pickle_load(data:"dict") -> "Logger":
+		x = {}
+		for d in data:
+			x[d] = pickle_X_loads(data[d])
+		data = x
+		inst = Logger()
+		inst.configuration_vars = data["configuration_vars"]
+		inst.active_debug_mode = data["active_debug_mode"]
+		inst.debug_modes = data["debug_modes"]
+		inst.debug_contexts = data["debug_contexts"]
+		for name in inst.debug_contexts:
+			inst.LOGGER_HELPER.set(name, DynamicVariableContainer(name))
+		for name in inst.debug_modes:
+			inst._update_state_after_adding_debug_mode(name, inst.debug_modes[name].level)
+		return inst
+
+
+
+	def __init__(self) -> None:
+		"""
+		YOU MUST NEVER CALL THIS DIRECTLY.
+
+		Raises:
+		    Exception: If the Logger is already initialized. Hence why i said never call this directly.
+
+		Side Effects:
+		- Adds a "disabled" debug mode to the system.
+		"""
+
+		self.configuration_vars = {}
+		self.debug_modes:"dict[str,DebugMode]" = {}
+		self.debug_contexts = {}
+		self.active_debug_mode = None
+
+		self.LOGGER_HELPER = DynamicVariableContainer("LOGGER_HELPER")
+
+		self._add_debug_mode("disabled", 0)
+		self.get_debug_mode("disabled").set_override_do_ever_write(False)
+
+
+	
+	def __call__(self, *args: Any, **kwds: Any) -> Any:
+		return self.LOGGER_HELPER
+
+
+
+	def set_debug_mode(self, name:"str") -> None:
+		"""
+		Sets the active debug mode.
+
+		Args:
+		    name (str): The name of the debug mode to set as active.
+		"""
+		self.active_debug_mode = self.debug_modes[name]
+
+
+
+	def _add_debug_mode(self, name:"str", level:"int"):
+		"""
+		YOU MUST NEVER CALL THIS DIRECTLY.
+
+		This is an inner function used by the `add_debug_mode` method (note without the underscore).
+		"""
+
+		# Check that the name isn't already in use.
+		if name in self.debug_modes:
+			raise Exception(f"Debug mode {name} already exists.")
+
+		# Construct the debug mode.
+		self.debug_modes[name] = DebugMode(name, level, None)
+
+		self._update_state_after_adding_debug_mode(
+			name,
+			level
+		)
+
+	
+
+	def _update_state_after_adding_debug_mode(self, name_of_debug_mode, level):
+		# The below wrapper is what actually gets called when you do `plsp().<insert name of debug mode>(...)`
+		# NOTE: Remember, this is only for the global context.
+		def wrapper_for_global_handler(*args, **kwargs):
+			context = self.debug_contexts[self.configuration_vars["global_context"]]
+			mode = self.debug_modes[name_of_debug_mode]
+			context.handle(mode, self.active_debug_mode, *args, **kwargs)
+
+		# And here is the wrapper for when we specify a context.
+		# E.g., `plsp().our_context.our_debug_mode(...)`...
+		# This wrapper is the `our_debug_mode` part.
+		# The actual `our_context` is made in the `add_debug_context` method and it is a `DynamicVariableContainer`
+		#  instance that is a child of the `LOGGER_HELPER` instance.
+		def wrapper_for_context_specified_handler(context, *args, **kwargs):
+			mode = self.debug_modes[name_of_debug_mode]
+			context.handle(mode, self.active_debug_mode, *args, **kwargs)
+
+		# We only want to use the `wrapper_for_global_handler` if the global context is set.
+		if self.configuration_vars.get("global_context") is not None:
+			self.LOGGER_HELPER.set(name_of_debug_mode, wrapper_for_global_handler)
+
+		# Now to update the context-specific wrappers.
+		keys_no_globals = [k for k in self.LOGGER_HELPER.get_children().keys() if k not in self.debug_modes.keys()]
+		keys_no_globals = [k for k in keys_no_globals if k not in ["set", "del", "get_children", "get_name"]]
+		for child_key in keys_no_globals:
+			container = self.LOGGER_HELPER.get_children()[child_key]
+			def _wrapper_for_the_wrapper(*args, **kwargs):
+				nonlocal container
+				context = self.debug_contexts[container.get_name()]
+				wrapper_for_context_specified_handler(context, *args, **kwargs)
+			container.set(name_of_debug_mode, _wrapper_for_the_wrapper)
+
+
+
+	def add_debug_mode(self, name:"str", separate=False):
+		"""
+		Adds a debug mode to the system.
+
+		Args:
+		    name (str): The name of the debug mode.
+		
+		Optional Keyword Args:
+		- write_to_file (str|None): 	The file to write to (if any).
+		- write_to_io (int|None): 	The io object to write to (if any).
+		- separate (bool): 		If this is a standalone debug mode, meaning, if this mode is active,
+					  	  all other debug mode will not be active.
+
+		NOTE: You must specify at least one of `write_to_file` or `write_to_io`.
+		"""
+
+		if separate:
+			level = -1
+		else:
+			level = len(self.debug_modes)+1
+
+		self._add_debug_mode(name, level)
+
+
+
+	def add_debug_context(self, name:"str"):
+		if name in self.debug_contexts:
+			raise Exception(f"Debug context {name} already exists.")
+		self.debug_contexts[name] = DebugContext(name)
+		self.LOGGER_HELPER.set(name, DynamicVariableContainer(name))
+
+
+
+	def get_debug_context(self, name:"str") -> "DebugContext":
+		return self.debug_contexts[name]
+	
+
+
+	def get_debug_mode(self, name:"str") -> "DebugMode":
+		return self.debug_modes[name]
+
+
+
+	def set(self, name:"str", value) -> None:
+		accepted_vars = ["global_context"]
+
+		if name not in accepted_vars:
+			raise Exception(f"Variable {name} not accepted.")
+
+		self.configuration_vars[name] = value
+
+
+
+
+
```

### Comparing `plsp-0.1/plsp/__init__.py` & `plsp-0.2/plsp/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,78 +1,80 @@
-"""
-info inject is a module allowing you to compile python source code with added debug information.
-this means that the interesting parts of the code stay separate from printing and other debug code.
-"""
-
-
-
-
-
-
-
-from . import Logger
-from . import DebugContext
-from . import DebugMode
-
-from . import infoinject
-from . import formatters
-
-
-
-
-
-
-
-"""
-
-=====================
-Pieces of the puzzle.
-=====================
-
-Logger 			- The piece that does the logging.
-
-DebugContext 		- Use this along side with the logger to separate different areas of an application.
-			- For example, you may have a rendering context and a physics context inside a game engine.
-
-DebugMode 		- Use this to specify different levels of debug information.
-			- For example, you may have a "info" mode and a "detail" mode.
-			- If the "info" mode is active, any messages that are in the "detail" mode will not be printed.
-			- This is because the "detail" mode extends from the "info" mode.
-			- If the "detail" mode is active, any messages that are in the "info"
-			-   and "detail" mode will be printed.
-
-ColorConfiguration 	- Use this to specify the colors of the debug information.
-			- For example, you may want to have the rendering context to be in green
-			-   and the physics context to be in red.
-
-InfoInjector 		- The piece that injects the debug information into the source code.
-			- Uses the Logger to log the debug information.
-
-formatters/ 		- The pieces that format the debug information.
-			- For example, you may want to have the time of the debug information to
-			-   be formatted in a specific way.
-			- You may also want to have the caller of the debug information to be formatted in a specific way.
-			- The formatters may be added onto any specified debug context. Then, when the Logger is used
-			-   by said context, the formatters will be used to format the debug information.
-formatters/TimeFormatter.py
-formatters/CallerFormatter.py
-
-
-
-====================================
-How the pieces relate to each other.
-====================================
-
-> Nodes A that is down from node B means that A depends on, or is used by, B.
-
-	Logger
-	/ \
-	+  +--------------------+
-	| 			|
-	Debug Context 		Debug Mode
-	/ \
-	+  +--------------------+
-	| 			|
-	Color Configuration	formatters/
- 
-
+"""
+info inject is a module allowing you to compile python source code with added debug information.
+this means that the interesting parts of the code stay separate from printing and other debug code.
+"""
+
+
+
+
+
+
+
+from .Logger import Logger
+from .SharedLogger import load as load_logger
+from .SharedLogger import save as save_logger
+from .DebugContext import DebugContext
+from .DebugMode import DebugMode
+from .Direction import IODirection
+
+from . import infoinject
+from . import formatters
+
+
+
+
+
+
+"""
+
+=====================
+Pieces of the puzzle.
+=====================
+
+Logger 			- The piece that does the logging.
+
+DebugContext 		- Use this along side with the logger to separate different areas of an application.
+			- For example, you may have a rendering context and a physics context inside a game engine.
+
+DebugMode 		- Use this to specify different levels of debug information.
+			- For example, you may have a "info" mode and a "detail" mode.
+			- If the "info" mode is active, any messages that are in the "detail" mode will not be printed.
+			- This is because the "detail" mode extends from the "info" mode.
+			- If the "detail" mode is active, any messages that are in the "info"
+			-   and "detail" mode will be printed.
+
+ColorConfiguration 	- Use this to specify the colors of the debug information.
+			- For example, you may want to have the rendering context to be in green
+			-   and the physics context to be in red.
+
+InfoInjector 		- The piece that injects the debug information into the source code.
+			- Uses the Logger to log the debug information.
+
+formatters/ 		- The pieces that format the debug information.
+			- For example, you may want to have the time of the debug information to
+			-   be formatted in a specific way.
+			- You may also want to have the caller of the debug information to be formatted in a specific way.
+			- The formatters may be added onto any specified debug context. Then, when the Logger is used
+			-   by said context, the formatters will be used to format the debug information.
+formatters/TimeFormatter.py
+formatters/CallerFormatter.py
+
+
+
+====================================
+How the pieces relate to each other.
+====================================
+
+> Nodes A that is down from node B means that A depends on, or is used by, B.
+
+	Logger
+	/ \
+	+  +--------------------+
+	| 			|
+	Debug Context 		Debug Mode
+	/ \
+	+  +--------------------+
+	| 			|
+	Color Configuration	formatters/
+ 
+
 """
```

### Comparing `plsp-0.1/plsp/infoinject/InfoInjector.py` & `plsp-0.2/plsp/infoinject/InfoInjector.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,397 +1,397 @@
-from typing import Callable
-import inspect
-import re
-
-
-
-
-
-
-
-class _InfoInjector:
-
-
-
-	def __init__(self):
-
-		self._instruction_stack = []
-
-		# End of `__init__`
-
-
-
-	def inject(self, globals, locals):
-		def wrapper_one(original_func):
-			def wrapper_two(*args, **kwargs):
-				
-				code = self._get_generated_func(original_func, self._instruction_stack)
-
-				# For some edge cases, we must sanitize the generated function.
-				# For example, if, in the instructions, we call the original function...
-				# This will throw an error, because the original function doesn't exist in this context.
-				complete = False
-				while not complete:
-					code, complete = self._sanitize_generated_func(code, original_func)
-
-				# The below loads the generated function into the global scope.
-				# We force it to save the function as a global variable.
-				exec(code, globals, locals)
-
-				locals["args"] = args
-				locals["kwargs"] = kwargs
-
-				# The below runs the generated function and saves the return value.
-				exec(f"__ret__ = __{original_func.__name__}__(*args, **kwargs)", globals, locals)
-
-				return locals["__ret__"]
-
-			return wrapper_two
-		return wrapper_one
-		# End of `def inject(self, globals, locals):`
-
-
-
-	def add_instruction(self, line:"int", debug_mode:"str", debug_context:"str",
-		     		  args_for_logger:"tuple", **kwargs_for_logger
-	):
-		def wrapper_one(original_func):
-			self._instruction_stack.append({
-				"line": line,
-				"debug_mode": debug_mode,
-				"debug_context": debug_context,
-				"args_for_logger": args_for_logger,
-				"kwargs_for_logger": kwargs_for_logger
-			})
-			return original_func
-		return wrapper_one
-		# End of `add_instruction`
-	
-
-
-	class VariableReference:
-		"""
-		When calling `InfoInjector.add_instruction`, you may use this class to reference variables.
-
-		For example:
-		```python
-		@InfoInjector.add_instruction(line=1, debug_mode="info", debug_context="generic", args_to_logger=(
-			f"n = {InfoInjector.VariableReference("n")}"
-		))
-		@InfoInjector.inject(globals(), locals())
-		def fib(n):
-			if n <= 1:
-				return n
-			else:
-				return fib(n-1) + fib(n-2)
-		```
-		
-		> When the code is put together to create our new function:
-
-		```python
-		def fib(n):
-			Logger().generic.info(f"n = {n}")
-			if n <= 1:
-				return n
-			else:
-				return fib(n-1) + fib(n-2)
-		```
-
-		> Notice the new line that was added.
-
-		Basically, the `VariableReference` class is used as a placeholder for the variable `n`.
-		It does not actually fetch anything at any time.
-
-		This is because python does the fetching when the newly compiled function is called.
-		"""
-
-		SALT = "|`VARIABLE_REFERENCE`|"
-
-		def __init__(self, name:"str"):
-			self.name = name
-
-		def __repr__(self):
-			return f"{self.SALT}{self.name}{self.SALT}"
-
-
-
-	###########
-	# HELPERS #
-	###########
-
-
-
-	def _sanitize_generated_func(self, generated_func, original_func) -> "tuple[str,bool]":
-		try:
-
-			completely_sanitized = True
-
-			# Pass 1: if the original function is called, replace it with the modified function name.
-			compiled = re.compile(rf"\b{original_func.__name__}\b\s*\(")
-			line_of_original_func_call = None
-			lines = generated_func.split("\n")
-			for i, line in enumerate(lines):
-				if compiled.search(line):
-					completely_sanitized = False
-					lines[i] = compiled.sub(f"__{original_func.__name__}__(", line)
-					line_of_original_func_call = i
-					break
-			
-
-			# We must wrap this in an exec statement.
-			#prefix_i = None
-			#for i, c in enumerate(lines[line_of_original_func_call]):
-			#	if c not in [" ", "\t"]:
-			#		prefix_i = i
-			#		break
-			#assert prefix_i is not None
-			#new = ""
-			#new += lines[line_of_original_func_call][:prefix_i] 
-			#new += f"exec('{lines[line_of_original_func_call][prefix_i:]}', globals(), locals())"
-			#lines[line_of_original_func_call] = new
-			## Then we run into even more problems, because if inside the exec statement is more "'" characters,
-			##   it will break.
-			## So we must escape all "'" characters.
-			#line = lines[line_of_original_func_call][prefix_i+6:-23]
-			#j = 0
-			#for i, char in enumerate(line):
-			#	if char == "'":
-			#		new = ""
-			#		new += line[:i+j]
-			#		new += "\\"
-			#		new += line[i+j:]
-			#		line = new
-			#		j += 1
-			#new = ""
-			#new += lines[line_of_original_func_call][:prefix_i+6]
-			#new += line
-			#new += lines[line_of_original_func_call][-23:]
-			#lines[line_of_original_func_call] = new
-
-			return "\n".join(lines), completely_sanitized
-		
-		except Exception as e:
-			print(e)
-			return generated_func, True
-		# End of `def _sanitize_generated_func(self, generated_func, original_func) -> "str":`
-	
-
-
-	def _get_generated_func(self, original_func, instruction_stack) -> "str":
-		for instruction in instruction_stack:
-			if not self._is_valid_instruction(instruction):
-				raise Exception("Invalid instruction")
-
-		# Step 1: get original function source code...
-		source = inspect.getsource(original_func)
-		original_func_name = original_func.__name__
-
-		# Step 2: remove the function decorator call from the original source code...
-		source = self._remove_decorator_call(source, original_func_name)
-		lines = source.split("\n")
-
-		# Step 4: find the indentation type...
-		# TODO: TEST THIS WITH DIFFERENT INDENTATIONS...
-		# I use tabs, idk if it works with spaces...
-		indentation_type = self._get_indentation_type(lines)
-		
-		# If we have multiple instructions, we need to add some value j to the line number.
-		# This is because we are adding lines to the source code, and the line numbers will change.
-		j = 0
-		while len(instruction_stack) > 0:
-			instruction = instruction_stack.pop(-1)
-			line_no = instruction["line"]
-			debug_mode = instruction["debug_mode"]
-			debug_context = instruction["debug_context"]
-			args_for_logger = instruction["args_for_logger"]
-			kwargs_for_logger = instruction["kwargs_for_logger"]
-			
-			# Replace the newline character with the repr for such.
-			for i, arg in enumerate(args_for_logger):
-				for y, c in enumerate(arg):
-					if c == "\n":
-						args_for_logger[i] = arg[:y-1] + "\\n" + arg[y+1:]
-			for key in kwargs_for_logger.keys():
-				value = kwargs_for_logger[key]
-				i = 0
-				while True:
-					try:
-						c = value[i]
-					except IndexError:
-						break
-					if c == "\n":
-						value = value[:i] + "\\n" + value[i+1:]
-						i += 2
-					else:
-						i += 1
-				kwargs_for_logger[key] = value
-
-			args_for_logger = self._parse_variable_references(args_for_logger)
-			args_for_logger = [f"f\"{arg}\"" for arg in args_for_logger]
-
-			line_no += j
-			prefix = indentation_type*self._get_indentation_level(lines, line_no, indentation_type)
-
-			# Step 5: inject the code...
-			new_line = f"{prefix}plsp().{debug_context}.{debug_mode}("
-			new_line += ", ".join(args_for_logger)
-
-			for key, value in kwargs_for_logger.items():
-				new_line += f", {key}=\"{value}\""
-
-			new_line += ")"
-
-			for line in new_line.split("\n"):
-				lines.insert(line_no, line)
-				line_no += 1
-				j += 1
-
-		# Step 6: rename the function...
-		self._rename_function(lines, original_func_name)
-
-		return "\n".join(lines)
-
-		# End of `def _get_generated_func(self, original_func, instructions):`
-			
-
-
-	def _parse_variable_references(self, args_for_logger:"tuple") -> "list[str]":
-		list_copy = []
-
-		for arg in args_for_logger:
-			list_copy.append(arg)
-
-		for i, arg in enumerate(list_copy):
-			if isinstance(arg, self.VariableReference):
-				list_copy[i] = f"{{{arg.name}}}"
-			new = list_copy[i]
-			x = 0
-			assert isinstance(new, str)
-			while self.VariableReference.SALT in new:
-				x += 1
-				pos = new.find(self.VariableReference.SALT)
-				if x == 1:
-					new = new[:pos] + "{" + new[pos+len(self.VariableReference.SALT):]
-				else:
-					new = new[:pos] + "}" + new[pos+len(self.VariableReference.SALT):]
-				if x == 2:
-					x = 0
-			list_copy[i] = new
-
-		return list_copy
-
-		# End of `def _parse_variable_references(self, args_for_logger):`
-
-
-
-	def _get_indentation_level(self, lines, line, indentation_type) -> "int":
-
-		indentation_level = 0
-		compare_buff = ""
-
-		for c in lines[line-1]:
-			keep_going = True
-			while keep_going:
-				if compare_buff == indentation_type:
-					indentation_level += 1
-					compare_buff = ""
-					break
-
-				if c == indentation_type[len(compare_buff)]:
-					compare_buff += c
-					continue
-				else:
-					compare_buff = ""
-				
-				keep_going = False
-
-		# check if the previous line has a ":" at the end.
-		prev_line = lines[line-1]
-		if prev_line[-1] == ":":
-			indentation_level += 1
-
-		return indentation_level
-
-		# End of `def _get_indentation_level(self, lines, line):`
-
-
-
-	def _is_valid_instruction(self, instruction) -> "bool":
-		ret = True
-
-		# TODO: do we need this function?
-
-		return ret
-	
-		# End of `def _is_valid_instruction(self, instruction):`
-
-
-
-	def _remove_decorator_call(self, source, original_func_name) -> "str":
-
-		lines = source.split("\n")
-		line_no_of_end_of_decorator_call = None
-
-		# compile our regex pattern
-		pattern = r"\bdef\s+" + re.escape(original_func_name) + r"\s*\("
-		compiled = re.compile(pattern)
-
-		for i, line in enumerate(lines):
-			# check if the line contains the pattern
-			if compiled.search(line):
-				line_no_of_end_of_decorator_call = i
-				break
-
-		if line_no_of_end_of_decorator_call is None:
-			raise Exception("Failure of regex")
-		
-		lines = lines[line_no_of_end_of_decorator_call:]
-		return "\n".join(lines)
-
-		# End of `def _remove_decorator_call(self, source, original_func_name):`
-
-
-
-	def _get_indentation_type(self, lines) -> "str":
-		indentation_type = None
-
-		for li in range(len(lines)):
-			for j, c in enumerate(lines[li]):
-				if c not in [" ", "\t"]:
-					break
-				if c == "\t":
-					indentation_type = "\t"
-					break
-
-		if indentation_type is None:
-			raise Exception("Unsupported indentation type.")
-
-		return indentation_type
-	
-		# End of `def _get_indentation_type(self, lines):`
-
-
-
-	def _rename_function(self, lines, original_func_name):
-		for li in range(len(lines)):
-			for j, c in enumerate(lines[li]):
-				if self._find_if_str_ahead(lines[li], j, f"def {original_func_name}"):
-
-					new_line = lines[li][:j]
-					new_line += f"def __{original_func_name}__" + lines[li][j+len(f"def {original_func_name}"):]
-					lines[li] = new_line
-
-		# End of `def _rename_function(self, lines, original_func_name):`
-
-
-
-	def _find_if_str_ahead(self, source, i, str) -> "bool":
-
-		s = source[i:i+len(str)]
-		return s == str
-
-		# End of `def _find_if_str_ahead(self, source, i, str):`
-
-
-
-
+from typing import Callable
+import inspect
+import re
+
+
+
+
+
+
+
+class _InfoInjector:
+
+
+
+	def __init__(self):
+
+		self._instruction_stack = []
+
+		# End of `__init__`
+
+
+
+	def inject(self, globals, locals):
+		def wrapper_one(original_func):
+			def wrapper_two(*args, **kwargs):
+				
+				code = self._get_generated_func(original_func, self._instruction_stack)
+
+				# For some edge cases, we must sanitize the generated function.
+				# For example, if, in the instructions, we call the original function...
+				# This will throw an error, because the original function doesn't exist in this context.
+				complete = False
+				while not complete:
+					code, complete = self._sanitize_generated_func(code, original_func)
+
+				# The below loads the generated function into the global scope.
+				# We force it to save the function as a global variable.
+				exec(code, globals, locals)
+
+				locals["args"] = args
+				locals["kwargs"] = kwargs
+
+				# The below runs the generated function and saves the return value.
+				exec(f"__ret__ = __{original_func.__name__}__(*args, **kwargs)", globals, locals)
+
+				return locals["__ret__"]
+
+			return wrapper_two
+		return wrapper_one
+		# End of `def inject(self, globals, locals):`
+
+
+
+	def add_instruction(self, line:"int", debug_mode:"str", debug_context:"str",
+		     		  args_for_logger:"tuple", **kwargs_for_logger
+	):
+		def wrapper_one(original_func):
+			self._instruction_stack.append({
+				"line": line,
+				"debug_mode": debug_mode,
+				"debug_context": debug_context,
+				"args_for_logger": args_for_logger,
+				"kwargs_for_logger": kwargs_for_logger
+			})
+			return original_func
+		return wrapper_one
+		# End of `add_instruction`
+	
+
+
+	class VariableReference:
+		"""
+		When calling `InfoInjector.add_instruction`, you may use this class to reference variables.
+
+		For example:
+		```python
+		@InfoInjector.add_instruction(line=1, debug_mode="info", debug_context="generic", args_to_logger=(
+			f"n = {InfoInjector.VariableReference("n")}"
+		))
+		@InfoInjector.inject(globals(), locals())
+		def fib(n):
+			if n <= 1:
+				return n
+			else:
+				return fib(n-1) + fib(n-2)
+		```
+		
+		> When the code is put together to create our new function:
+
+		```python
+		def fib(n):
+			Logger().generic.info(f"n = {n}")
+			if n <= 1:
+				return n
+			else:
+				return fib(n-1) + fib(n-2)
+		```
+
+		> Notice the new line that was added.
+
+		Basically, the `VariableReference` class is used as a placeholder for the variable `n`.
+		It does not actually fetch anything at any time.
+
+		This is because python does the fetching when the newly compiled function is called.
+		"""
+
+		SALT = "|`VARIABLE_REFERENCE`|"
+
+		def __init__(self, name:"str"):
+			self.name = name
+
+		def __repr__(self):
+			return f"{self.SALT}{self.name}{self.SALT}"
+
+
+
+	###########
+	# HELPERS #
+	###########
+
+
+
+	def _sanitize_generated_func(self, generated_func, original_func) -> "tuple[str,bool]":
+		try:
+
+			completely_sanitized = True
+
+			# Pass 1: if the original function is called, replace it with the modified function name.
+			compiled = re.compile(rf"\b{original_func.__name__}\b\s*\(")
+			line_of_original_func_call = None
+			lines = generated_func.split("\n")
+			for i, line in enumerate(lines):
+				if compiled.search(line):
+					completely_sanitized = False
+					lines[i] = compiled.sub(f"__{original_func.__name__}__(", line)
+					line_of_original_func_call = i
+					break
+			
+
+			# We must wrap this in an exec statement.
+			#prefix_i = None
+			#for i, c in enumerate(lines[line_of_original_func_call]):
+			#	if c not in [" ", "\t"]:
+			#		prefix_i = i
+			#		break
+			#assert prefix_i is not None
+			#new = ""
+			#new += lines[line_of_original_func_call][:prefix_i] 
+			#new += f"exec('{lines[line_of_original_func_call][prefix_i:]}', globals(), locals())"
+			#lines[line_of_original_func_call] = new
+			## Then we run into even more problems, because if inside the exec statement is more "'" characters,
+			##   it will break.
+			## So we must escape all "'" characters.
+			#line = lines[line_of_original_func_call][prefix_i+6:-23]
+			#j = 0
+			#for i, char in enumerate(line):
+			#	if char == "'":
+			#		new = ""
+			#		new += line[:i+j]
+			#		new += "\\"
+			#		new += line[i+j:]
+			#		line = new
+			#		j += 1
+			#new = ""
+			#new += lines[line_of_original_func_call][:prefix_i+6]
+			#new += line
+			#new += lines[line_of_original_func_call][-23:]
+			#lines[line_of_original_func_call] = new
+
+			return "\n".join(lines), completely_sanitized
+		
+		except Exception as e:
+			print(e)
+			return generated_func, True
+		# End of `def _sanitize_generated_func(self, generated_func, original_func) -> "str":`
+	
+
+
+	def _get_generated_func(self, original_func, instruction_stack) -> "str":
+		for instruction in instruction_stack:
+			if not self._is_valid_instruction(instruction):
+				raise Exception("Invalid instruction")
+
+		# Step 1: get original function source code...
+		source = inspect.getsource(original_func)
+		original_func_name = original_func.__name__
+
+		# Step 2: remove the function decorator call from the original source code...
+		source = self._remove_decorator_call(source, original_func_name)
+		lines = source.split("\n")
+
+		# Step 4: find the indentation type...
+		# TODO: TEST THIS WITH DIFFERENT INDENTATIONS...
+		# I use tabs, idk if it works with spaces...
+		indentation_type = self._get_indentation_type(lines)
+		
+		# If we have multiple instructions, we need to add some value j to the line number.
+		# This is because we are adding lines to the source code, and the line numbers will change.
+		j = 0
+		while len(instruction_stack) > 0:
+			instruction = instruction_stack.pop(-1)
+			line_no = instruction["line"]
+			debug_mode = instruction["debug_mode"]
+			debug_context = instruction["debug_context"]
+			args_for_logger = instruction["args_for_logger"]
+			kwargs_for_logger = instruction["kwargs_for_logger"]
+			
+			# Replace the newline character with the repr for such.
+			for i, arg in enumerate(args_for_logger):
+				for y, c in enumerate(arg):
+					if c == "\n":
+						args_for_logger[i] = arg[:y-1] + "\\n" + arg[y+1:]
+			for key in kwargs_for_logger.keys():
+				value = kwargs_for_logger[key]
+				i = 0
+				while True:
+					try:
+						c = value[i]
+					except IndexError:
+						break
+					if c == "\n":
+						value = value[:i] + "\\n" + value[i+1:]
+						i += 2
+					else:
+						i += 1
+				kwargs_for_logger[key] = value
+
+			args_for_logger = self._parse_variable_references(args_for_logger)
+			args_for_logger = [f"f\"{arg}\"" for arg in args_for_logger]
+
+			line_no += j
+			prefix = indentation_type*self._get_indentation_level(lines, line_no, indentation_type)
+
+			# Step 5: inject the code...
+			new_line = f"{prefix}plsp().{debug_context}.{debug_mode}("
+			new_line += ", ".join(args_for_logger)
+
+			for key, value in kwargs_for_logger.items():
+				new_line += f", {key}=\"{value}\""
+
+			new_line += ")"
+
+			for line in new_line.split("\n"):
+				lines.insert(line_no, line)
+				line_no += 1
+				j += 1
+
+		# Step 6: rename the function...
+		self._rename_function(lines, original_func_name)
+
+		return "\n".join(lines)
+
+		# End of `def _get_generated_func(self, original_func, instructions):`
+			
+
+
+	def _parse_variable_references(self, args_for_logger:"tuple") -> "list[str]":
+		list_copy = []
+
+		for arg in args_for_logger:
+			list_copy.append(arg)
+
+		for i, arg in enumerate(list_copy):
+			if isinstance(arg, self.VariableReference):
+				list_copy[i] = f"{{{arg.name}}}"
+			new = list_copy[i]
+			x = 0
+			assert isinstance(new, str)
+			while self.VariableReference.SALT in new:
+				x += 1
+				pos = new.find(self.VariableReference.SALT)
+				if x == 1:
+					new = new[:pos] + "{" + new[pos+len(self.VariableReference.SALT):]
+				else:
+					new = new[:pos] + "}" + new[pos+len(self.VariableReference.SALT):]
+				if x == 2:
+					x = 0
+			list_copy[i] = new
+
+		return list_copy
+
+		# End of `def _parse_variable_references(self, args_for_logger):`
+
+
+
+	def _get_indentation_level(self, lines, line, indentation_type) -> "int":
+
+		indentation_level = 0
+		compare_buff = ""
+
+		for c in lines[line-1]:
+			keep_going = True
+			while keep_going:
+				if compare_buff == indentation_type:
+					indentation_level += 1
+					compare_buff = ""
+					break
+
+				if c == indentation_type[len(compare_buff)]:
+					compare_buff += c
+					continue
+				else:
+					compare_buff = ""
+				
+				keep_going = False
+
+		# check if the previous line has a ":" at the end.
+		prev_line = lines[line-1]
+		if prev_line[-1] == ":":
+			indentation_level += 1
+
+		return indentation_level
+
+		# End of `def _get_indentation_level(self, lines, line):`
+
+
+
+	def _is_valid_instruction(self, instruction) -> "bool":
+		ret = True
+
+		# TODO: do we need this function?
+
+		return ret
+	
+		# End of `def _is_valid_instruction(self, instruction):`
+
+
+
+	def _remove_decorator_call(self, source, original_func_name) -> "str":
+
+		lines = source.split("\n")
+		line_no_of_end_of_decorator_call = None
+
+		# compile our regex pattern
+		pattern = r"\bdef\s+" + re.escape(original_func_name) + r"\s*\("
+		compiled = re.compile(pattern)
+
+		for i, line in enumerate(lines):
+			# check if the line contains the pattern
+			if compiled.search(line):
+				line_no_of_end_of_decorator_call = i
+				break
+
+		if line_no_of_end_of_decorator_call is None:
+			raise Exception("Failure of regex")
+		
+		lines = lines[line_no_of_end_of_decorator_call:]
+		return "\n".join(lines)
+
+		# End of `def _remove_decorator_call(self, source, original_func_name):`
+
+
+
+	def _get_indentation_type(self, lines) -> "str":
+		indentation_type = None
+
+		for li in range(len(lines)):
+			for j, c in enumerate(lines[li]):
+				if c not in [" ", "\t"]:
+					break
+				if c == "\t":
+					indentation_type = "\t"
+					break
+
+		if indentation_type is None:
+			raise Exception("Unsupported indentation type.")
+
+		return indentation_type
+	
+		# End of `def _get_indentation_type(self, lines):`
+
+
+
+	def _rename_function(self, lines, original_func_name):
+		for li in range(len(lines)):
+			for j, c in enumerate(lines[li]):
+				if self._find_if_str_ahead(lines[li], j, f"def {original_func_name}"):
+
+					new_line = lines[li][:j]
+					new_line += f"def __{original_func_name}__" + lines[li][j+len(f"def {original_func_name}"):]
+					lines[li] = new_line
+
+		# End of `def _rename_function(self, lines, original_func_name):`
+
+
+
+	def _find_if_str_ahead(self, source, i, str) -> "bool":
+
+		s = source[i:i+len(str)]
+		return s == str
+
+		# End of `def _find_if_str_ahead(self, source, i, str):`
+
+
+
+
 InfoInjector = _InfoInjector()
```

### Comparing `plsp-0.1/plsp.egg-info/PKG-INFO` & `plsp-0.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,191 +1,182 @@
-Metadata-Version: 2.1
-Name: plsp
-Version: 0.1
-Summary: A simple, easy to use, and powerful logging library for Python.
-Author: matrikater (Joel Watson)
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-
-# Please Log Shit Please (or `plsp`)
-
-## Notes
-
-```text
-info inject is a module allowing you to compile python source code with added debug information.
-this means that the interesting parts of the code stay separate from printing and other debug code.
-```
-
-```text
-=====================
-Pieces of the puzzle.
-=====================
-
-Logger 			- The piece that does the logging.
-
-DebugContext 		- Use this along side with the logger to separate different areas of an application.
-			- For example, you may have a rendering context and a physics context inside a game engine.
-
-DebugMode 		- Use this to specify different levels of debug information.
-			- For example, you may have a "info" mode and a "detail" mode.
-			- If the "info" mode is active, any messages that are in the "detail" mode will not be printed.
-			- This is because the "detail" mode extends from the "info" mode.
-			- If the "detail" mode is active, any messages that are in the "info"
-			-   and "detail" mode will be printed.
-
-ColorConfiguration 	- Use this to specify the colors of the debug information.
-			- For example, you may want to have the rendering context to be in green
-			-   and the physics context to be in red.
-
-InfoInjector 		- The piece that injects the debug information into the source code.
-			- Uses the Logger to log the debug information.
-
-formatters/ 		- The pieces that format the debug information.
-			- For example, you may want to have the time of the debug information to
-			-   be formatted in a specific way.
-			- You may also want to have the caller of the debug information to be formatted in a specific way.
-			- The formatters may be added onto any specified debug context. Then, when the Logger is used
-			-   by said context, the formatters will be used to format the debug information.
-
-
-
-====================================
-How the pieces relate to each other.
-====================================
-
-> Nodes A that is down from node B means that A depends on, or is used by, B.
-
-	Logger
-	/ \
-	+  +--------------------+
-	|                       |
-	Debug Context           Debug Mode
-	/ \
-	+  +--------------------+
-	|                       |
-	Color Configuration     formatters/
-```
-
-## Usage
-
-```python
-from pls.Logger import plsp
-#from formatters import TimeFormatter, CallerFormatter
-from plsp.DebugMode import DebugMode
-from plsp.Direction import IODirection
-
-import sys
-
-# use below to separate log files based on debug mode instead of debug context.
-#plsp.set("io_based_on_mode", True)
-
-
-
-# The below sets the global context to generic.
-plsp.set("global_context", "generic")
-
-
-
-# Below is adding a debug context.
-# It is a bit more complicated than setting up debug contexts so you dont have to set all the parameters at once.
-plsp.add_debug_context("generic")
-plsp.add_debug_context("rendering")
-plsp.add_debug_context("physics")
-
-
-
-# Below is adding a debug mode.
-# You can:
-# - Use the `write_to_file` parameter to specify a file to write to.
-# - Use the `write_to_io` parameter to specify an io object to write to.
-# - Use the `separate` parameter to specify if this is a standalone debug mode, meaning, if this mode is active,
-#     the previous debug mode will not be active.
-plsp.add_debug_mode("info")
-plsp.add_debug_mode("detail")
-plsp.add_debug_mode("debug")
-plsp.add_debug_mode("error", separate=True)
-
-
-
-# START OF MODIFYING DEBUG CONTEXTS #
-
-# You may modify the debug contexts after they are created.
-# Access the debug context by using the `Logger.debug_contexts` dictionary.
-
-pls.get_debug_context("generic").set_can_ever_write(True)
-plsp.get_debug_context("generic").add_direction(IODirection(False, sys.stdout.fileno(), None))
-plsp.get_debug_context("rendering").set_can_ever_write(True)
-plsp.get_debug_context("rendering").add_direction(IODirection(False, sys.stdout.fileno(), None))
-plsp.get_debug_context("physics").set_can_ever_write(True)
-plsp.get_debug_context("physics").add_direction(IODirection(False, sys.stdout.fileno(), None))
-					       
-# The below will add the time before each log message.
-#plsp.get_debug_context("generic").add_format_layer(TimeFormatter)
-#plsp.get_debug_context("rendering").add_format_layer(TimeFormatter)
-#plsp.get_debug_context("physics").add_format_layer(TimeFormatter)
-#
-## The below will add which ever function called the log message.
-#plsp.get_debug_context("generic").add_format_layer(CallerFormatter)
-#plsp.get_debug_context("rendering").add_format_layer(CallerFormatter)
-#plsp.get_debug_context("physics").add_format_layer(CallerFormatter)
-#
-
-# END OF MODIFYING DEBUG CONTEXTS #
-
-
-
-# Now we can use the debug contexts to log messages.
-plsp.set_debug_mode("info")
-
-plsp().info("This is using the generic context.")
-plsp().info("It works since we set a global context.")
-
-
-
-class renderer:
-	def __init__(self):
-		plsp().rendering.detail("The rendering engine in this engine is pretty simple!")
-
-
-
-class physics:
-	def __init__(self):
-		plsp().physics.detail("The physics engine in this engine is pretty simple!")
-
-
-#my_renderer = renderer()
-my_physics = physics()
-
-plsp.set_debug_mode("detail")
-
-my_physics = physics()
-
-
-
-
-
-
-
-from plsp.infoinject import InfoInjector
-
-@InfoInjector.add_instruction(line=1, debug_mode="info", debug_context="generic", args_for_logger=(
-	f"n = {InfoInjector.VariableReference('n')}",
-))
-@InfoInjector.add_instruction(line=2, debug_mode="detail", debug_context="generic", args_for_logger=(
-	f"n is", "less than or equal to 1"
-),
-	end="\n.\n"
-)
-@InfoInjector.add_instruction(line=4, debug_mode="info", debug_context="generic", args_for_logger=(
-	f"n is greater than 1",
-	f"Now actually calculating... n-1 and n-2"
-))
-@InfoInjector.inject(globals(), locals())
-def fib(n):
-	if n <= 1:
-		return n
-	else:
-		return fib(n-1) + fib(n-2)
-
-fib(5)
-```
-## V0.01 released on 16th/5/2024
-init
+# Please Log Shit Please (or `plsp`)
+
+## Notes
+
+```text
+info inject is a module allowing you to compile python source code with added debug information.
+this means that the interesting parts of the code stay separate from printing and other debug code.
+```
+
+```text
+=====================
+Pieces of the puzzle.
+=====================
+
+Logger 			- The piece that does the logging.
+
+DebugContext 		- Use this along side with the logger to separate different areas of an application.
+			- For example, you may have a rendering context and a physics context inside a game engine.
+
+DebugMode 		- Use this to specify different levels of debug information.
+			- For example, you may have a "info" mode and a "detail" mode.
+			- If the "info" mode is active, any messages that are in the "detail" mode will not be printed.
+			- This is because the "detail" mode extends from the "info" mode.
+			- If the "detail" mode is active, any messages that are in the "info"
+			-   and "detail" mode will be printed.
+
+ColorConfiguration 	- Use this to specify the colors of the debug information.
+			- For example, you may want to have the rendering context to be in green
+			-   and the physics context to be in red.
+
+InfoInjector 		- The piece that injects the debug information into the source code.
+			- Uses the Logger to log the debug information.
+
+formatters/ 		- The pieces that format the debug information.
+			- For example, you may want to have the time of the debug information to
+			-   be formatted in a specific way.
+			- You may also want to have the caller of the debug information to be formatted in a specific way.
+			- The formatters may be added onto any specified debug context. Then, when the Logger is used
+			-   by said context, the formatters will be used to format the debug information.
+
+
+
+====================================
+How the pieces relate to each other.
+====================================
+
+> Nodes A that is down from node B means that A depends on, or is used by, B.
+
+	Logger
+	/ \
+	+  +--------------------+
+	|                       |
+	Debug Context           Debug Mode
+	/ \
+	+  +--------------------+
+	|                       |
+	Color Configuration     formatters/
+```
+
+## Usage
+
+```python
+from pls.Logger import plsp
+#from formatters import TimeFormatter, CallerFormatter
+from plsp.DebugMode import DebugMode
+from plsp.Direction import IODirection
+
+import sys
+
+# use below to separate log files based on debug mode instead of debug context.
+#plsp.set("io_based_on_mode", True)
+
+
+
+# The below sets the global context to generic.
+plsp.set("global_context", "generic")
+
+
+
+# Below is adding a debug context.
+# It is a bit more complicated than setting up debug contexts so you dont have to set all the parameters at once.
+plsp.add_debug_context("generic")
+plsp.add_debug_context("rendering")
+plsp.add_debug_context("physics")
+
+
+
+# Below is adding a debug mode.
+# You can:
+# - Use the `write_to_file` parameter to specify a file to write to.
+# - Use the `write_to_io` parameter to specify an io object to write to.
+# - Use the `separate` parameter to specify if this is a standalone debug mode, meaning, if this mode is active,
+#     the previous debug mode will not be active.
+plsp.add_debug_mode("info")
+plsp.add_debug_mode("detail")
+plsp.add_debug_mode("debug")
+plsp.add_debug_mode("error", separate=True)
+
+
+
+# START OF MODIFYING DEBUG CONTEXTS #
+
+# You may modify the debug contexts after they are created.
+# Access the debug context by using the `Logger.debug_contexts` dictionary.
+
+pls.get_debug_context("generic").set_can_ever_write(True)
+plsp.get_debug_context("generic").add_direction(IODirection(False, sys.stdout.fileno(), None))
+plsp.get_debug_context("rendering").set_can_ever_write(True)
+plsp.get_debug_context("rendering").add_direction(IODirection(False, sys.stdout.fileno(), None))
+plsp.get_debug_context("physics").set_can_ever_write(True)
+plsp.get_debug_context("physics").add_direction(IODirection(False, sys.stdout.fileno(), None))
+					       
+# The below will add the time before each log message.
+#plsp.get_debug_context("generic").add_format_layer(TimeFormatter)
+#plsp.get_debug_context("rendering").add_format_layer(TimeFormatter)
+#plsp.get_debug_context("physics").add_format_layer(TimeFormatter)
+#
+## The below will add which ever function called the log message.
+#plsp.get_debug_context("generic").add_format_layer(CallerFormatter)
+#plsp.get_debug_context("rendering").add_format_layer(CallerFormatter)
+#plsp.get_debug_context("physics").add_format_layer(CallerFormatter)
+#
+
+# END OF MODIFYING DEBUG CONTEXTS #
+
+
+
+# Now we can use the debug contexts to log messages.
+plsp.set_debug_mode("info")
+
+plsp().info("This is using the generic context.")
+plsp().info("It works since we set a global context.")
+
+
+
+class renderer:
+	def __init__(self):
+		plsp().rendering.detail("The rendering engine in this engine is pretty simple!")
+
+
+
+class physics:
+	def __init__(self):
+		plsp().physics.detail("The physics engine in this engine is pretty simple!")
+
+
+#my_renderer = renderer()
+my_physics = physics()
+
+plsp.set_debug_mode("detail")
+
+my_physics = physics()
+
+
+
+
+
+
+
+from plsp.infoinject import InfoInjector
+
+@InfoInjector.add_instruction(line=1, debug_mode="info", debug_context="generic", args_for_logger=(
+	f"n = {InfoInjector.VariableReference('n')}",
+))
+@InfoInjector.add_instruction(line=2, debug_mode="detail", debug_context="generic", args_for_logger=(
+	f"n is", "less than or equal to 1"
+),
+	end="\n.\n"
+)
+@InfoInjector.add_instruction(line=4, debug_mode="info", debug_context="generic", args_for_logger=(
+	f"n is greater than 1",
+	f"Now actually calculating... n-1 and n-2"
+))
+@InfoInjector.inject(globals(), locals())
+def fib(n):
+	if n <= 1:
+		return n
+	else:
+		return fib(n-1) + fib(n-2)
+
+fib(5)
+```
```

