# Comparing `tmp/ezcord-0.6.2.tar.gz` & `tmp/ezcord-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezcord-0.6.2.tar", last modified: Thu Mar 14 21:23:44 2024, max compression
+gzip compressed data, was "ezcord-0.6.3.tar", last modified: Thu May 16 15:17:49 2024, max compression
```

## Comparing `ezcord-0.6.2.tar` & `ezcord-0.6.3.tar`

### file list

```diff
@@ -1,58 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 21:23:44.488759 ezcord-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-14 21:23:39.000000 ezcord-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-14 21:23:39.000000 ezcord-0.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-03-14 21:23:44.488759 ezcord-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-03-14 21:23:39.000000 ezcord-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 21:23:44.480759 ezcord-0.6.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-14 21:23:39.000000 ezcord-0.6.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 21:23:44.484759 ezcord-0.6.2/ezcord/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-03-14 21:23:39.000000 ezcord-0.6.2/ezcord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-03-14 21:23:39.000000 ezcord-0.6.2/ezcord/blacklist.py
--rw-r--r--   0 runner    (1001) docker     (127)    34862 2024-03-14 21:23:39.000000 ezcord-0.6.2/ezcord/bot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 21:23:44.484759 ezcord-0.6.2/ezcord/cogs/
--rw-r--r--   0 runner    (1001) docker     (127)    10403 2024-03-14 21:23:39.000000 ezcord-0.6.2/ezcord/cogs/blacklist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 21:23:44.484759 ezcord-0.6.2/ezcord/cogs/dpy/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-14 21:23:39.000000 ezcord-0.6.2/ezcord/cogs/dpy/blacklist_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-14 21:23:39.000000 ezcord-0.6.2/ezcord/cogs/dpy/help_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-14 21:23:39.000000 ezcord-0.6.2/ezcord/cogs/dpy/status_changer_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    13342 2024-03-14 21:23:39.000000 ezcord-0.6.2/ezcord/cogs/help.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 21:23:44.488759 ezcord-0.6.2/ezcord/cogs/pyc/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-14 21:23:39.000000 ezcord-0.6.2/ezcord/cogs/pyc/blacklist_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-14 21:23:39.000000 ezcord-0.6.2/ezcord/cogs/pyc/help_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-14 21:23:39.000000 ezcord-0.6.2/ezcord/cogs/pyc/status_changer_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-03-14 21:23:39.000000 ezcord-0.6.2/ezcord/cogs/status_changer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6683 2024-03-14 21:23:39.000000 ezcord-0.6.2/ezcord/components.py
--rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-03-14 21:23:39.000000 ezcord-0.6.2/ezcord/emb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-03-14 21:23:39.000000 ezcord-0.6.2/ezcord/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-03-14 21:23:39.000000 ezcord-0.6.2/ezcord/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    28168 2024-03-14 21:23:39.000000 ezcord-0.6.2/ezcord/i18n.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 21:23:44.488759 ezcord-0.6.2/ezcord/internal/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-03-14 21:23:39.000000 ezcord-0.6.2/ezcord/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-03-14 21:23:39.000000 ezcord-0.6.2/ezcord/internal/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-03-14 21:23:39.000000 ezcord-0.6.2/ezcord/internal/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 21:23:44.488759 ezcord-0.6.2/ezcord/internal/dc/
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-03-14 21:23:39.000000 ezcord-0.6.2/ezcord/internal/dc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-14 21:23:39.000000 ezcord-0.6.2/ezcord/internal/dc/dc_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-03-14 21:23:39.000000 ezcord-0.6.2/ezcord/internal/embed_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 21:23:44.488759 ezcord-0.6.2/ezcord/internal/language/
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-03-14 21:23:39.000000 ezcord-0.6.2/ezcord/internal/language/de.json
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-03-14 21:23:39.000000 ezcord-0.6.2/ezcord/internal/language/en.json
--rw-r--r--   0 runner    (1001) docker     (127)     5385 2024-03-14 21:23:39.000000 ezcord-0.6.2/ezcord/internal/language/languages.py
--rw-r--r--   0 runner    (1001) docker     (127)     7140 2024-03-14 21:23:39.000000 ezcord-0.6.2/ezcord/internal/ready_style.py
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-03-14 21:23:39.000000 ezcord-0.6.2/ezcord/internal/translation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12570 2024-03-14 21:23:39.000000 ezcord-0.6.2/ezcord/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11065 2024-03-14 21:23:39.000000 ezcord-0.6.2/ezcord/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-03-14 21:23:39.000000 ezcord-0.6.2/ezcord/times.py
--rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-03-14 21:23:39.000000 ezcord-0.6.2/ezcord/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 21:23:44.488759 ezcord-0.6.2/ezcord.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-03-14 21:23:44.000000 ezcord-0.6.2/ezcord.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-03-14 21:23:44.000000 ezcord-0.6.2/ezcord.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 21:23:44.000000 ezcord-0.6.2/ezcord.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-14 21:23:44.000000 ezcord-0.6.2/ezcord.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-14 21:23:44.000000 ezcord-0.6.2/ezcord.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-03-14 21:23:39.000000 ezcord-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-14 21:23:39.000000 ezcord-0.6.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 21:23:44.488759 ezcord-0.6.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 21:23:44.488759 ezcord-0.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-03-14 21:23:39.000000 ezcord-0.6.2/tests/test_libs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-03-14 21:23:39.000000 ezcord-0.6.2/tests/test_times.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:17:49.723100 ezcord-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-16 15:17:40.000000 ezcord-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-16 15:17:40.000000 ezcord-0.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4904 2024-05-16 15:17:49.723100 ezcord-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-16 15:17:40.000000 ezcord-0.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:17:49.715100 ezcord-0.6.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-16 15:17:40.000000 ezcord-0.6.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:17:49.715100 ezcord-0.6.3/ezcord/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/blacklist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35717 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:17:49.719100 ezcord-0.6.3/ezcord/cogs/
+-rw-r--r--   0 runner    (1001) docker     (127)    10403 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/cogs/blacklist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:17:49.719100 ezcord-0.6.3/ezcord/cogs/dpy/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/cogs/dpy/blacklist_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/cogs/dpy/help_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/cogs/dpy/status_changer_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13342 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/cogs/help.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:17:49.719100 ezcord-0.6.3/ezcord/cogs/pyc/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/cogs/pyc/blacklist_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/cogs/pyc/help_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/cogs/pyc/status_changer_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/cogs/status_changer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/emb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28260 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/i18n.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:17:49.719100 ezcord-0.6.3/ezcord/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/internal/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/internal/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:17:49.719100 ezcord-0.6.3/ezcord/internal/dc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/internal/dc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/internal/dc/dc_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/internal/embed_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:17:49.723100 ezcord-0.6.3/ezcord/internal/language/
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/internal/language/de.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/internal/language/en.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5385 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/internal/language/languages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7140 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/internal/ready_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/internal/translation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12424 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/logs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:17:49.723100 ezcord-0.6.3/ezcord/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7515 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/sql/postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11065 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/sql/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/times.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:17:49.723100 ezcord-0.6.3/ezcord.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4904 2024-05-16 15:17:49.000000 ezcord-0.6.3/ezcord.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-16 15:17:49.000000 ezcord-0.6.3/ezcord.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 15:17:49.000000 ezcord-0.6.3/ezcord.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-16 15:17:49.000000 ezcord-0.6.3/ezcord.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-16 15:17:49.000000 ezcord-0.6.3/ezcord.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-16 15:17:40.000000 ezcord-0.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-16 15:17:40.000000 ezcord-0.6.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 15:17:49.723100 ezcord-0.6.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:17:49.723100 ezcord-0.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-16 15:17:40.000000 ezcord-0.6.3/tests/test_libs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-05-16 15:17:40.000000 ezcord-0.6.3/tests/test_times.py
```

### Comparing `ezcord-0.6.2/LICENSE` & `ezcord-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ezcord-0.6.2/PKG-INFO` & `ezcord-0.6.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezcord
-Version: 0.6.2
+Version: 0.6.3
 Summary: An easy-to-use extension for Discord.py and Pycord
 Author: tibue99
 License: MIT
 Project-URL: GitHub, https://github.com/tibue99/ezcord
 Project-URL: Documentation, https://ezcord.readthedocs.io
 Keywords: discord,pycord,py-cord,discord.py
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: colorama
 Requires-Dist: aiosqlite
+Requires-Dist: asyncpg
 Requires-Dist: python-dotenv
 Provides-Extra: docs
 Requires-Dist: py-cord; extra == "docs"
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
@@ -43,15 +44,15 @@
 and [Pycord](https://github.com/Pycord-Development/pycord) with some utility functions.
 
 ## Features
 ### ✏️ Reduce boilerplate code
 - Easy cog management
 - Embed templates
 - Datetime and file utilities
-- Wrapper for [aiosqlite](https://github.com/omnilib/aiosqlite)
+- Wrapper for [aiosqlite](https://github.com/omnilib/aiosqlite) and [asyncpg](https://github.com/MagicStack/asyncpg)
 
 ### ✨ Error handling
 - Automatic error handling for slash commands
 - Error webhook reports
 - Custom logging
 
 ### 📚 i18n
```

### Comparing `ezcord-0.6.2/README.md` & `ezcord-0.6.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 and [Pycord](https://github.com/Pycord-Development/pycord) with some utility functions.
 
 ## Features
 ### ✏️ Reduce boilerplate code
 - Easy cog management
 - Embed templates
 - Datetime and file utilities
-- Wrapper for [aiosqlite](https://github.com/omnilib/aiosqlite)
+- Wrapper for [aiosqlite](https://github.com/omnilib/aiosqlite) and [asyncpg](https://github.com/MagicStack/asyncpg)
 
 ### ✨ Error handling
 - Automatic error handling for slash commands
 - Error webhook reports
 - Custom logging
 
 ### 📚 i18n
```

### Comparing `ezcord-0.6.2/ezcord/blacklist.py` & `ezcord-0.6.3/ezcord/blacklist.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.6.2/ezcord/bot.py` & `ezcord-0.6.3/ezcord/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,17 +23,26 @@
     localize_cog,
     localize_command,
     print_custom_ready,
     print_ready,
     tr,
 )
 from .internal.config import Blacklist
-from .internal.dc import DPY, PYCORD, CogMeta, bridge, checks, commands, discord
+from .internal.dc import (
+    DPY,
+    PYCORD,
+    AutoShardedBot,
+    CogMeta,
+    bridge,
+    checks,
+    commands,
+    discord,
+)
 from .logs import DEFAULT_LOG, custom_log, set_log
-from .sql import DBHandler
+from .sql import DBHandler, PGHandler
 from .times import dc_timestamp
 
 if PYCORD:
     _main_bot = discord.Bot
 else:
     _main_bot = commands.Bot
 
@@ -135,15 +144,15 @@
             else:
                 self.add_listener(self._error_event, "on_application_command_error")
 
         self.ready_event = ready_event
         if ready_event:
             self.add_listener(self._ready_event, "on_ready")
         self.add_listener(self._check_cog_groups, "on_ready")
-        self.add_listener(self._db_setup, "on_ready")
+        self.add_listener(self._db_setup, "on_connect")
 
         self.ready_event_adds: dict = {}
         self.ready_event_removes: list[int | str] = []
 
         self.enabled_extensions: list[str] = []
         self.initial_cogs: list[str] = []
 
@@ -395,18 +404,33 @@
         if DPY:
             self.all_dpy_commands = await self.tree.fetch_commands()
 
     @staticmethod
     async def _db_setup():
         """Calls the setup method of all registered :class:`.DBHandler` instances."""
 
-        setup_copy = DBHandler._auto_setup.copy()
+        load_dotenv()
+        auto_setup = os.getenv("PGAUTOSETUP", "1") == "1"
+
+        if len(PGHandler._auto_setup) != 0:
+            await PGHandler()._check_pool()  # make sure that pool is created before setup
+            for instance in PGHandler._auto_pool.copy():
+                await instance._check_pool()
+
+        if not auto_setup:
+            return
+
+        setup_copy = DBHandler._auto_setup.copy() + PGHandler._auto_setup.copy()
+
+        tasks = []
         for instance in setup_copy:
             if hasattr(instance, "setup") and callable(instance.setup):
-                await instance.setup()
+                tasks.append(instance.setup())
+
+        await asyncio.gather(*tasks)
 
     async def _check_cog_groups(self):
         """Checks if all cog groups are valid."""
         for cog in self.cogs.values():
             if hasattr(cog, "group") and cog.group:
                 if cog.group not in self.cogs.keys():
                     self.logger.warning(
@@ -932,14 +956,24 @@
     This is only needed for Pycord.
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
 
+class AutoShardedBot(Bot, AutoShardedBot):  # type: ignore
+    """A subclass of :class:`discord.AutoShardedBot` that implements the :class:`Bot` class.
+
+    This class can be used if you want to use EzCord with an auto-sharded bot.
+    """
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+
 class _CogMeta(CogMeta):
     """A metaclass for cogs that adds an ``emoji`` attribute."""
 
     def __new__(cls, *args, **kwargs) -> CogMeta:
         name, bases, attrs = args
         attrs["emoji"] = kwargs.pop("emoji", None)
         attrs["group"] = kwargs.pop("group", None)
```

### Comparing `ezcord-0.6.2/ezcord/cogs/blacklist.py` & `ezcord-0.6.3/ezcord/cogs/blacklist.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.6.2/ezcord/cogs/help.py` & `ezcord-0.6.3/ezcord/cogs/help.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.6.2/ezcord/cogs/status_changer.py` & `ezcord-0.6.3/ezcord/cogs/status_changer.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.6.2/ezcord/components.py` & `ezcord-0.6.3/ezcord/components.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
             class MyView(View):  # right
                 ...
 
             class MyView(discord.ui.View):  # wrong
                 ...
 """
+
 from __future__ import annotations
 
 import asyncio
 import inspect
 import os
 from typing import Callable
```

### Comparing `ezcord-0.6.2/ezcord/emb.py` & `ezcord-0.6.3/ezcord/emb.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.6.2/ezcord/enums.py` & `ezcord-0.6.3/ezcord/enums.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.6.2/ezcord/errors.py` & `ezcord-0.6.3/ezcord/errors.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,14 +19,18 @@
     """Base exception class for all Ezcord exceptions."""
 
 
 class ConvertTimeError(EzcordException):
     """Raised when a time conversion fails."""
 
 
+class DurationError(ConvertTimeError):
+    """Raised when a given duration is too long."""
+
+
 class Blacklisted(EzcordException):
     """Can be raised when a blacklisted user tries to use a command.
 
     This error can be caught in a command error handler to send a custom response.
     """
```

### Comparing `ezcord-0.6.2/ezcord/i18n.py` & `ezcord-0.6.3/ezcord/i18n.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,18 +178,20 @@
                     )
 
     return kwargs
 
 
 def _localize_send(send_func):
     async def wrapper(
-        self: discord.InteractionResponse
-        | discord.Webhook
-        | discord.abc.Messageable
-        | discord.Interaction,
+        self: (
+            discord.InteractionResponse
+            | discord.Webhook
+            | discord.abc.Messageable
+            | discord.Interaction
+        ),
         content=None,
         *,
         count: int | None = None,
         use_locale: LOCALE_OBJECT | None = None,
         **kwargs,
     ):
         """Wrapper to localize the content and the embed of a message.
@@ -350,27 +352,29 @@
         *,
         fallback_locale: str = "en-US",
         process_strings: bool = True,
         prefer_user_locale: bool = False,
         localize_numbers: bool = True,
         ignore_discord_ids: bool = True,
         exclude_methods: list[str] | None = None,
-        disable_translations: list[
-            Literal[
-                "send",
-                "edit",
-                "send_message",
-                "send_modal",
-                "edit_message",
-                "edit_original_response",
-                "webhook_send",
-                "webhook_edit_message",
+        disable_translations: (
+            list[
+                Literal[
+                    "send",
+                    "edit",
+                    "send_message",
+                    "send_modal",
+                    "edit_message",
+                    "edit_original_response",
+                    "webhook_send",
+                    "webhook_edit_message",
+                ]
             ]
-        ]
-        | None = None,
+            | None
+        ) = None,
         debug: bool = True,
         **variables,
     ):
         I18N.initialized = True
         if "en" in localizations:
             en = localizations.pop("en")
             localizations["en-GB"] = en
@@ -421,21 +425,19 @@
         if "webhook_edit_message" not in disable_translations:
             setattr(discord.Webhook, "edit_message", _localize_edit(WEBHOOK_EDIT_MESSAGE))
         if "webhook_edit_message" not in disable_translations:
             setattr(discord.WebhookMessage, "edit_message", _localize_edit(WEBHOOK_EDIT))
 
     @staticmethod
     @overload
-    def get_locale(obj: str) -> str:
-        ...
+    def get_locale(obj: str) -> str: ...
 
     @staticmethod
     @overload
-    def get_locale(obj: LOCALE_OBJECT) -> str:
-        ...
+    def get_locale(obj: LOCALE_OBJECT) -> str: ...
 
     @staticmethod
     def get_locale(obj):
         """Get the locale from the given object. By default, this is the guild's locale.
 
         Parameters
         ----------
```

### Comparing `ezcord-0.6.2/ezcord/internal/colors.py` & `ezcord-0.6.3/ezcord/internal/colors.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.6.2/ezcord/internal/config.py` & `ezcord-0.6.3/ezcord/internal/config.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.6.2/ezcord/internal/dc/__init__.py` & `ezcord-0.6.3/ezcord/internal/dc/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -28,22 +28,23 @@
 except ImportError:
     # EzCord is used without a supported Discord library
     discord = commands = FakeDiscord()  # type: ignore
     tasks, checks = None, commands  # type: ignore
 
 
 if discord.__title__ == "pycord":
-    from discord import CogMeta
+    from discord import AutoShardedBot, CogMeta
     from discord.ext import bridge
 
     slash_command = discord.slash_command
     checks = commands
 
 else:
     CogMeta = commands.CogMeta
+    AutoShardedBot = commands.AutoShardedBot
     bridge = commands
 
     if discord.__title__ == "discord":
         slash_command = discord.app_commands.command
         checks = discord.app_commands.checks
 
     elif discord.__title__ == "nextcord":
```

### Comparing `ezcord-0.6.2/ezcord/internal/embed_templates.py` & `ezcord-0.6.3/ezcord/internal/embed_templates.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 
     if interaction.guild and interaction.guild.icon:
         replace["server_icon"] = interaction.guild.icon.url
     else:
         replace["server_icon"] = interaction.client.user.display_avatar.url
 
     for key, value in replace.items():
-        s = s.replace("{" + key + "}", value)
+        s = s.replace("{" + key + "}", str(value))
 
     return s
 
 
 def replace_dict(
     content: dict | str, interaction: discord.Interaction, custom_dict: dict[str, str] | None = None
 ) -> dict | str:
```

### Comparing `ezcord-0.6.2/ezcord/internal/language/de.json` & `ezcord-0.6.3/ezcord/internal/language/de.json`

 * *Files identical despite different names*

### Comparing `ezcord-0.6.2/ezcord/internal/language/en.json` & `ezcord-0.6.3/ezcord/internal/language/en.json`

 * *Files identical despite different names*

### Comparing `ezcord-0.6.2/ezcord/internal/language/languages.py` & `ezcord-0.6.3/ezcord/internal/language/languages.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.6.2/ezcord/internal/ready_style.py` & `ezcord-0.6.3/ezcord/internal/ready_style.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.6.2/ezcord/internal/translation.py` & `ezcord-0.6.3/ezcord/internal/translation.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.6.2/ezcord/logs.py` & `ezcord-0.6.3/ezcord/logs.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,18 +208,15 @@
                 formatter = logging.Formatter(log_format)
                 msg = formatter.format(record)
             else:
                 msg = self.format(record)
 
         if self.webhook_url:
             loop = asyncio.get_event_loop()
-            if loop.is_running():
-                loop.create_task(_send_discord_log(self.webhook_url, record, msg))
-            else:
-                loop.run_until_complete(_send_discord_log(self.webhook_url, record, msg))
+            loop.create_task(_send_discord_log(self.webhook_url, record, msg))
 
 
 async def _send_discord_log(webhook_url: str, record: logging.LogRecord, msg):
     async with aiohttp.ClientSession() as session:
         webhook = discord.Webhook.from_url(webhook_url, session=session)
         name = "EzCord" if record.name == DEFAULT_LOG else record.name
         try:
```

### Comparing `ezcord-0.6.2/ezcord/sql.py` & `ezcord-0.6.3/ezcord/sql/sqlite.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.6.2/ezcord/times.py` & `ezcord-0.6.3/ezcord/times.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import re
 from datetime import datetime, timedelta, timezone
 from typing import TYPE_CHECKING, Literal
 
-from .errors import ConvertTimeError
+from .errors import ConvertTimeError, DurationError
 from .internal import tp
 from .internal.dc import discord
 
 if TYPE_CHECKING:
     from .i18n import LOCALE_OBJECT
 
 
@@ -148,14 +148,16 @@
     :class:`int`
         The amount of seconds.
 
     Raises
     ------
     :exc:`ConvertTimeError`
          No valid number was found, or ``default_unit`` is ``None`` while no valid unit was found.
+    :exc:`DurationError`
+        The duration is too long.
 
     Example
     -------
     >>> convert_to_seconds("1m 9s")
     69
     >>> convert_to_seconds("1.5m")
     90
@@ -198,8 +200,13 @@
         raise ConvertTimeError(f"Could not convert '{string}' to seconds.")
 
     if "months" in found_units:
         found_units.setdefault("days", 0)
         found_units["days"] = found_units["months"] * 30
         del found_units["months"]
 
-    return int(timedelta(**found_units).total_seconds())
+    try:
+        return int(timedelta(**found_units).total_seconds())
+    except OverflowError:
+        if error:
+            raise DurationError(f"Duration '{string}' is too long.")
+        return 0
```

### Comparing `ezcord-0.6.2/ezcord/utils.py` & `ezcord-0.6.3/ezcord/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -167,25 +167,28 @@
     return autocomplete_callback
 
 
 def count_lines(
     directory: str | None = None,
     *,
     count_empty_lines: bool = True,
+    include_hidden: bool = False,
     ignored_dirs: list[str] | None = None,
     ignored_files: list[str] | None = None,
 ) -> int:
     """Counts the total amount of lines in all Python files in the given directory.
 
     Parameters
     ----------
     directory:
         The directory to count the lines in. Defaults to the current working directory.
     count_empty_lines:
         Whether to count empty lines. Defaults to ``True``.
+    include_hidden:
+        Whether to include directories starting with a dot. Defaults to ``False``.
     ignored_dirs:
         A list of directories to ignore. By default, venv folders and folders starting with a dot
         are ignored.
     ignored_files:
         A list of file patterns to ignore.
     """
     if directory is None:
@@ -193,14 +196,16 @@
     if ignored_dirs is None:
         ignored_dirs = []
     if ignored_files is None:
         ignored_files = []
 
     total_lines = 0
     for root, _, files in os.walk(directory):
+        if not include_hidden and Path(root).parts[-1].startswith("."):
+            ignored_dirs.append(root)
         if "pyvenv.cfg" in files:  # ignore venv folders
             ignored_dirs.append(root)
 
         if any([True for pattern in ignored_dirs if pattern in str(Path(root))]):
             continue
 
         for file in files:
```

### Comparing `ezcord-0.6.2/ezcord.egg-info/PKG-INFO` & `ezcord-0.6.3/ezcord.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezcord
-Version: 0.6.2
+Version: 0.6.3
 Summary: An easy-to-use extension for Discord.py and Pycord
 Author: tibue99
 License: MIT
 Project-URL: GitHub, https://github.com/tibue99/ezcord
 Project-URL: Documentation, https://ezcord.readthedocs.io
 Keywords: discord,pycord,py-cord,discord.py
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: colorama
 Requires-Dist: aiosqlite
+Requires-Dist: asyncpg
 Requires-Dist: python-dotenv
 Provides-Extra: docs
 Requires-Dist: py-cord; extra == "docs"
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
@@ -43,15 +44,15 @@
 and [Pycord](https://github.com/Pycord-Development/pycord) with some utility functions.
 
 ## Features
 ### ✏️ Reduce boilerplate code
 - Easy cog management
 - Embed templates
 - Datetime and file utilities
-- Wrapper for [aiosqlite](https://github.com/omnilib/aiosqlite)
+- Wrapper for [aiosqlite](https://github.com/omnilib/aiosqlite) and [asyncpg](https://github.com/MagicStack/asyncpg)
 
 ### ✨ Error handling
 - Automatic error handling for slash commands
 - Error webhook reports
 - Custom logging
 
 ### 📚 i18n
```

### Comparing `ezcord-0.6.2/ezcord.egg-info/SOURCES.txt` & `ezcord-0.6.3/ezcord.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 ezcord/bot.py
 ezcord/components.py
 ezcord/emb.py
 ezcord/enums.py
 ezcord/errors.py
 ezcord/i18n.py
 ezcord/logs.py
-ezcord/sql.py
 ezcord/times.py
 ezcord/utils.py
 ezcord.egg-info/PKG-INFO
 ezcord.egg-info/SOURCES.txt
 ezcord.egg-info/dependency_links.txt
 ezcord.egg-info/requires.txt
 ezcord.egg-info/top_level.txt
@@ -37,9 +36,12 @@
 ezcord/internal/ready_style.py
 ezcord/internal/translation.py
 ezcord/internal/dc/__init__.py
 ezcord/internal/dc/dc_imports.py
 ezcord/internal/language/de.json
 ezcord/internal/language/en.json
 ezcord/internal/language/languages.py
+ezcord/sql/__init__.py
+ezcord/sql/postgresql.py
+ezcord/sql/sqlite.py
 tests/test_libs.py
 tests/test_times.py
```

### Comparing `ezcord-0.6.2/pyproject.toml` & `ezcord-0.6.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ezcord-0.6.2/tests/test_libs.py` & `ezcord-0.6.3/tests/test_libs.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.6.2/tests/test_times.py` & `ezcord-0.6.3/tests/test_times.py`

 * *Files identical despite different names*

