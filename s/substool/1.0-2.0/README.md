# Comparing `tmp/substool-1.0.tar.gz` & `tmp/substool-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "substool-1.0.tar", last modified: Sun May 12 20:30:46 2024, max compression
+gzip compressed data, was "substool-2.0.tar", last modified: Thu May 16 11:53:18 2024, max compression
```

## Comparing `substool-1.0.tar` & `substool-2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 facundo   (1000) facundo   (1000)        0 2024-05-12 20:30:46.132050 substool-1.0/
--rw-rw-r--   0 facundo   (1000) facundo   (1000)    11357 2024-02-03 23:21:18.000000 substool-1.0/LICENSE
--rw-rw-r--   0 facundo   (1000) facundo   (1000)      566 2024-05-12 20:30:46.132050 substool-1.0/PKG-INFO
--rw-rw-r--   0 facundo   (1000) facundo   (1000)       64 2024-02-03 23:24:45.000000 substool-1.0/README.md
--rw-rw-r--   0 facundo   (1000) facundo   (1000)       38 2024-05-12 20:30:46.132050 substool-1.0/setup.cfg
--rwxrwxr-x   0 facundo   (1000) facundo   (1000)      990 2024-05-12 20:29:51.000000 substool-1.0/setup.py
-drwxrwxr-x   0 facundo   (1000) facundo   (1000)        0 2024-05-12 20:30:46.132050 substool-1.0/substool.egg-info/
--rw-rw-r--   0 facundo   (1000) facundo   (1000)      566 2024-05-12 20:30:46.000000 substool-1.0/substool.egg-info/PKG-INFO
--rw-rw-r--   0 facundo   (1000) facundo   (1000)      356 2024-05-12 20:30:46.000000 substool-1.0/substool.egg-info/SOURCES.txt
--rw-rw-r--   0 facundo   (1000) facundo   (1000)        1 2024-05-12 20:30:46.000000 substool-1.0/substool.egg-info/dependency_links.txt
--rw-rw-r--   0 facundo   (1000) facundo   (1000)       51 2024-05-12 20:30:46.000000 substool-1.0/substool.egg-info/entry_points.txt
--rw-rw-r--   0 facundo   (1000) facundo   (1000)       10 2024-05-12 20:30:46.000000 substool-1.0/substool.egg-info/requires.txt
--rw-rw-r--   0 facundo   (1000) facundo   (1000)       10 2024-05-12 20:30:46.000000 substool-1.0/substool.egg-info/top_level.txt
-drwxrwxr-x   0 facundo   (1000) facundo   (1000)        0 2024-05-12 20:30:46.132050 substool-1.0/subtitles/
--rw-rw-r--   0 facundo   (1000) facundo   (1000)      267 2024-03-06 20:32:18.000000 substool-1.0/subtitles/__main__.py
--rw-rw-r--   0 facundo   (1000) facundo   (1000)     8151 2024-04-27 18:09:41.000000 substool-1.0/subtitles/command_check.py
--rw-rw-r--   0 facundo   (1000) facundo   (1000)    11261 2024-04-25 17:05:43.000000 substool-1.0/subtitles/commands_rest.py
--rw-rw-r--   0 facundo   (1000) facundo   (1000)     3451 2024-03-10 14:40:09.000000 substool-1.0/subtitles/helpers.py
--rw-rw-r--   0 facundo   (1000) facundo   (1000)     1623 2024-03-10 14:47:01.000000 substool-1.0/subtitles/main.py
--rw-rw-r--   0 facundo   (1000) facundo   (1000)     8429 2024-03-10 14:40:41.000000 substool-1.0/subtitles/parsers.py
+drwxrwxr-x   0 facundo   (1000) facundo   (1000)        0 2024-05-16 11:53:18.819956 substool-2.0/
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)    11357 2024-05-16 11:45:12.000000 substool-2.0/LICENSE
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)      564 2024-05-16 11:53:18.819956 substool-2.0/PKG-INFO
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)       63 2024-05-16 11:45:26.000000 substool-2.0/README.md
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)       38 2024-05-16 11:53:18.819956 substool-2.0/setup.cfg
+-rwxrwxr-x   0 facundo   (1000) facundo   (1000)      984 2024-05-16 11:48:53.000000 substool-2.0/setup.py
+drwxrwxr-x   0 facundo   (1000) facundo   (1000)        0 2024-05-16 11:53:18.819956 substool-2.0/substool/
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)      264 2024-05-16 11:49:52.000000 substool-2.0/substool/__main__.py
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)     8148 2024-05-16 11:50:02.000000 substool-2.0/substool/command_check.py
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)    11247 2024-05-16 11:50:45.000000 substool-2.0/substool/commands_rest.py
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)     3450 2024-05-16 11:50:57.000000 substool-2.0/substool/helpers.py
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)     1618 2024-05-16 11:51:10.000000 substool-2.0/substool/main.py
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)     8427 2024-05-16 11:51:15.000000 substool-2.0/substool/parsers.py
+drwxrwxr-x   0 facundo   (1000) facundo   (1000)        0 2024-05-16 11:53:18.819956 substool-2.0/substool.egg-info/
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)      564 2024-05-16 11:53:18.000000 substool-2.0/substool.egg-info/PKG-INFO
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)      350 2024-05-16 11:53:18.000000 substool-2.0/substool.egg-info/SOURCES.txt
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)        1 2024-05-16 11:53:18.000000 substool-2.0/substool.egg-info/dependency_links.txt
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)       49 2024-05-16 11:53:18.000000 substool-2.0/substool.egg-info/entry_points.txt
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)       10 2024-05-16 11:53:18.000000 substool-2.0/substool.egg-info/requires.txt
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)        9 2024-05-16 11:53:18.000000 substool-2.0/substool.egg-info/top_level.txt
```

### Comparing `substool-1.0/LICENSE` & `substool-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `substool-1.0/PKG-INFO` & `substool-2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: substool
-Version: 1.0
+Version: 2.0
 Summary: Tool to handle and fix subtitles general issues.
-Home-page: https://github.com/facundobatista/subtitles
+Home-page: https://github.com/facundobatista/substool
 Author: Facundo Batista
 Author-email: facundo@taniquetil.com.ar
 License: Apace-v2
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 License-File: LICENSE
 
-# subtitles
+# substool
 
 Tool to handle and fix subtitles general issues.
```

### Comparing `substool-1.0/setup.py` & `substool-2.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 #!/usr/bin/env python3
 
 # Copyright 2024 Facundo Batista
 # Licensed under the Apache v2 License
-# For further info, check https://github.com/facundobatista/subtitles
+# For further info, check https://github.com/facundobatista/substool
 
-"""Setup script for subtitles."""
+"""Setup script for substool."""
 
 from setuptools import setup
 
 
-VERSION = "1.0"
+VERSION = "2.0"
 
 
 setup(
     name="substool",
     version=VERSION,
     author="Facundo Batista",
     author_email="facundo@taniquetil.com.ar",
     description="Tool to handle and fix subtitles general issues.",
     long_description=open("README.md", "rt", encoding="utf8").read(),
-    url="https://github.com/facundobatista/subtitles",
+    url="https://github.com/facundobatista/substool",
     license="Apace-v2",
-    packages=["subtitles"],
+    packages=["substool"],
     classifiers=[
         "Environment :: Console",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
     ],
     entry_points={
-        "console_scripts": ["subtitles = subtitles.main:main"],
+        "console_scripts": ["substool = substool.main:main"],
     },
     install_requires=["craft_cli"],
     python_requires=">=3",
 )
```

### Comparing `substool-1.0/substool.egg-info/PKG-INFO` & `substool-2.0/substool.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: substool
-Version: 1.0
+Version: 2.0
 Summary: Tool to handle and fix subtitles general issues.
-Home-page: https://github.com/facundobatista/subtitles
+Home-page: https://github.com/facundobatista/substool
 Author: Facundo Batista
 Author-email: facundo@taniquetil.com.ar
 License: Apace-v2
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 License-File: LICENSE
 
-# subtitles
+# substool
 
 Tool to handle and fix subtitles general issues.
```

### Comparing `substool-1.0/subtitles/command_check.py` & `substool-2.0/substool/command_check.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Copyright 2014-2024 Facundo Batista
 # Licensed under the Apache v2 License
-# For further info, check https://github.com/facundobatista/subtitles
+# For further info, check https://github.com/facundobatista/substool
 
 """The Check command."""
 
 import textwrap
 
 from craft_cli import BaseCommand, emit
 
-from subtitles.helpers import open_rar, open_zip, save_srt, SubItem, valid_filepath
-from subtitles.parsers import parse_subtitle
+from substool.helpers import open_rar, open_zip, save_srt, SubItem, valid_filepath
+from substool.parsers import parse_subtitle
 
 # lines longer than this (in chars) do not fit nicely in the screen
 MAX_TEXT_LENGTH = 90
 
 
 # subs with this text will be removed
 SPAM_STRINGS = [
```

### Comparing `substool-1.0/subtitles/commands_rest.py` & `substool-2.0/substool/commands_rest.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # Copyright 2014-2024 Facundo Batista
 # Licensed under the Apache v2 License
-# For further info, check https://github.com/facundobatista/subtitles
+# For further info, check https://github.com/facundobatista/substool
 
 """The generic small commands."""
 
 import itertools
 import textwrap
 
 from craft_cli import BaseCommand, emit, ArgumentParsingError
 
-from subtitles.helpers import save_srt, SubItem, valid_filepath, time_sub2stamp, time_stamp2sub
-from subtitles.parsers import parse_subtitle
+from substool.helpers import save_srt, SubItem, valid_filepath, time_sub2stamp, time_stamp2sub
+from substool.parsers import parse_subtitle
 
 
 def _subtime(value):
     """Return a valid timestamp; else ArgumentParsingError is raised."""
     try:
         return time_sub2stamp(value)
     except ValueError as exc:
@@ -48,15 +48,15 @@
 
     name = "rescale-points"
     help_msg = "Rescale using two points in time."
     overview = textwrap.dedent("""
         Rescale a subtitles file using two points (id1 and id2) displacing
         them to the new times (time1 and time2).
 
-          e.g.:  subtitles rescale-points Movie.srt 4 43,5 168 1:02:15
+          e.g.:  substool rescale-points Movie.srt 4 43,5 168 1:02:15
 
         If id1 is 0, time1 is ignored and all is calculated against beginning.
     """)
 
     def fill_parser(self, parser):
         """Add own parameters to the general parser."""
         parser.add_argument("filepath", type=valid_filepath, help="The subtitle to process")
@@ -100,15 +100,15 @@
     """Rescale a subs file using parameters delta and speed."""
 
     name = "rescale-params"
     help_msg = "Rescale using parameters delta and speed."
     overview = textwrap.dedent("""
         Rescale a subtitles file using parameters delta and speed.
 
-          e.g.: subtitles rescale-params Movie.srt 2.3 1.0014
+          e.g.: substool rescale-params Movie.srt 2.3 1.0014
 
         These params are normally retrieved from rescale-points applied to a similar file.
     """)
 
     def fill_parser(self, parser):
         """Add own parameters to the general parser."""
         parser.add_argument("filepath", type=valid_filepath, help="The subtitle to process")
@@ -126,15 +126,15 @@
     """Do several checks on the subtitle file(s); decompress and extract if needed."""
 
     name = "rescale-mimic"
     help_msg = "Rescale using a source file."
     overview = textwrap.dedent("""
         Rescale a subtitles file using initial and final points from 'source' subtitles file.
 
-          e.g.: subtitles rescale-mimic subs-to-fix.srt source-subs.srt
+          e.g.: substool rescale-mimic subs-to-fix.srt source-subs.srt
     """)
 
     def fill_parser(self, parser):
         """Add own parameters to the general parser."""
         parser.add_argument("tofix-filepath", type=valid_filepath, help="The subtitle to fix")
         parser.add_argument("source-filepath", type=valid_filepath, help="The source subtitle")
 
@@ -161,16 +161,16 @@
     """Shift the times in a subtitles file the specified seconds."""
 
     name = "shift"
     help_msg = "Shift times in a subtitles file."
     overview = textwrap.dedent("""
         Shift the times in a subtitles file the specified seconds.
 
-          example: subtitles.py shift Movie.srt 3.22
-                   subtitles.py shift Movie.srt -2,1
+          example: substool shift Movie.srt 3.22
+                   substool shift Movie.srt -2,1
     """)
 
     def fill_parser(self, parser):
         """Add own parameters to the general parser."""
         parser.add_argument("filepath", type=valid_filepath, help="The subtitle to process")
         parser.add_argument("delta", type=_friendly_float, help="Delta seconds to shift all times")
```

### Comparing `substool-1.0/subtitles/helpers.py` & `substool-2.0/substool/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright 2014-2024 Facundo Batista
 # Licensed under the Apache v2 License
-# For further info, check https://github.com/facundobatista/subtitles
+# For further info, check https://github.com/facundobatista/substool
 
 """Helpers for the different commands."""
 
 import collections
 import os
 import pathlib
 import subprocess
```

### Comparing `substool-1.0/subtitles/main.py` & `substool-2.0/substool/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright 2024 Facundo Batista
 # Licensed under the Apache v2 License
-# For further info, check https://github.com/facundobatista/subtitles
+# For further info, check https://github.com/facundobatista/substool
 
 """Main entry point of the modules."""
 
 import sys
 
 from craft_cli import (
     ArgumentParsingError,
@@ -12,34 +12,34 @@
     CraftError,
     Dispatcher,
     EmitterMode,
     ProvideHelpException,
     emit,
 )
 
-from subtitles import command_check, commands_rest
+from substool import command_check, commands_rest
 
 commands = [
     command_check.CheckCommand,
     commands_rest.RescalePointsCommand,
     commands_rest.RescaleParamsCommand,
     commands_rest.RescaleMimicCommand,
     commands_rest.ShiftCommand,
     commands_rest.AdjustCommand,
 ]
 
 
 def main():
     """Handle the main entry point."""
-    emit.init(EmitterMode.BRIEF, "subtitles", "Starting the subtitles app.")
+    emit.init(EmitterMode.BRIEF, "substool", "Starting the substool app.")
     command_groups = [CommandGroup("Basic", commands)]
     summary = "Tool to handle and fix subtitles general issues."
 
     try:
-        dispatcher = Dispatcher("subtitles", command_groups, summary=summary)
+        dispatcher = Dispatcher("substool", command_groups, summary=summary)
         dispatcher.pre_parse_args(sys.argv[1:])
         dispatcher.load_command(None)
         dispatcher.run()
     except (ArgumentParsingError, ProvideHelpException) as err:
         print(err, file=sys.stderr)  # to stderr, as argparse normally does
         emit.ended_ok()
     except CraftError as err:
```

### Comparing `substool-1.0/subtitles/parsers.py` & `substool-2.0/substool/parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Copyright 2014-2024 Facundo Batista
 # Licensed under the Apache v2 License
-# For further info, check https://github.com/facundobatista/subtitles
+# For further info, check https://github.com/facundobatista/substool
 
 """Subtitles parsers."""
 
 import re
 from xml.etree import ElementTree
 
 from craft_cli import emit, CraftError
 
-from subtitles.helpers import time_sub2stamp, SubItem
+from substool.helpers import time_sub2stamp, SubItem
 
 
 # to clean some tags
 RE_TAGS = re.compile("<[^>]*>")
 
 
 def _build_sub_item(pack):
```

