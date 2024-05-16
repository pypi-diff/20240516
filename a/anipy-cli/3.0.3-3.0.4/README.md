# Comparing `tmp/anipy_cli-3.0.3.tar.gz` & `tmp/anipy_cli-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anipy_cli-3.0.3.tar", max compression
+gzip compressed data, was "anipy_cli-3.0.4.tar", max compression
```

## Comparing `anipy_cli-3.0.3.tar` & `anipy_cli-3.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1974 2024-05-14 16:34:45.680884 anipy_cli-3.0.3/README.md
--rw-r--r--   0        0        0      855 2024-05-14 16:34:45.680884 anipy_cli-3.0.3/pyproject.toml
--rw-r--r--   0        0        0       48 2024-05-14 16:34:45.680884 anipy_cli-3.0.3/src/anipy_cli/__init__.py
--rw-r--r--   0        0        0     5299 2024-05-14 16:34:45.680884 anipy_cli-3.0.3/src/anipy_cli/arg_parser.py
--rw-r--r--   0        0        0     1922 2024-05-14 16:34:45.680884 anipy_cli-3.0.3/src/anipy_cli/cli.py
--rw-r--r--   0        0        0      411 2024-05-14 16:34:45.680884 anipy_cli-3.0.3/src/anipy_cli/clis/__init__.py
--rw-r--r--   0        0        0      609 2024-05-14 16:34:45.680884 anipy_cli-3.0.3/src/anipy_cli/clis/base_cli.py
--rw-r--r--   0        0        0     2281 2024-05-14 16:34:45.680884 anipy_cli-3.0.3/src/anipy_cli/clis/binge_cli.py
--rw-r--r--   0        0        0     2815 2024-05-14 16:34:45.680884 anipy_cli-3.0.3/src/anipy_cli/clis/default_cli.py
--rw-r--r--   0        0        0     3197 2024-05-14 16:34:45.680884 anipy_cli-3.0.3/src/anipy_cli/clis/download_cli.py
--rw-r--r--   0        0        0     2676 2024-05-14 16:34:45.680884 anipy_cli-3.0.3/src/anipy_cli/clis/history_cli.py
--rw-r--r--   0        0        0     2260 2024-05-14 16:34:45.680884 anipy_cli-3.0.3/src/anipy_cli/clis/mal_cli.py
--rw-r--r--   0        0        0      616 2024-05-14 16:34:45.680884 anipy_cli-3.0.3/src/anipy_cli/clis/seasonal_cli.py
--rw-r--r--   0        0        0      916 2024-05-14 16:34:45.680884 anipy_cli-3.0.3/src/anipy_cli/colors.py
--rw-r--r--   0        0        0    15404 2024-05-14 16:34:45.680884 anipy_cli-3.0.3/src/anipy_cli/config.py
--rw-r--r--   0        0        0     1160 2024-05-14 16:34:45.680884 anipy_cli-3.0.3/src/anipy_cli/discord.py
--rw-r--r--   0        0        0     6981 2024-05-14 16:34:45.680884 anipy_cli-3.0.3/src/anipy_cli/mal_proxy.py
--rw-r--r--   0        0        0      185 2024-05-14 16:34:45.680884 anipy_cli-3.0.3/src/anipy_cli/menus/__init__.py
--rw-r--r--   0        0        0     1140 2024-05-14 16:34:45.680884 anipy_cli-3.0.3/src/anipy_cli/menus/base_menu.py
--rw-r--r--   0        0        0    24091 2024-05-14 16:34:45.680884 anipy_cli-3.0.3/src/anipy_cli/menus/mal_menu.py
--rw-r--r--   0        0        0     6179 2024-05-14 16:34:45.680884 anipy_cli-3.0.3/src/anipy_cli/menus/menu.py
--rw-r--r--   0        0        0     9097 2024-05-14 16:34:45.680884 anipy_cli-3.0.3/src/anipy_cli/menus/seasonal_menu.py
--rw-r--r--   0        0        0     6989 2024-05-14 16:34:45.680884 anipy_cli-3.0.3/src/anipy_cli/prompts.py
--rw-r--r--   0        0        0     7684 2024-05-14 16:34:45.680884 anipy_cli-3.0.3/src/anipy_cli/util.py
--rw-r--r--   0        0        0     3084 1970-01-01 00:00:00.000000 anipy_cli-3.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1974 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/README.md
+-rw-r--r--   0        0        0      855 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/pyproject.toml
+-rw-r--r--   0        0        0       48 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/src/anipy_cli/__init__.py
+-rw-r--r--   0        0        0     5299 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/src/anipy_cli/arg_parser.py
+-rw-r--r--   0        0        0     1922 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/src/anipy_cli/cli.py
+-rw-r--r--   0        0        0      411 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/src/anipy_cli/clis/__init__.py
+-rw-r--r--   0        0        0      609 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/src/anipy_cli/clis/base_cli.py
+-rw-r--r--   0        0        0     2281 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/src/anipy_cli/clis/binge_cli.py
+-rw-r--r--   0        0        0     2815 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/src/anipy_cli/clis/default_cli.py
+-rw-r--r--   0        0        0     3197 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/src/anipy_cli/clis/download_cli.py
+-rw-r--r--   0        0        0     2675 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/src/anipy_cli/clis/history_cli.py
+-rw-r--r--   0        0        0     2258 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/src/anipy_cli/clis/mal_cli.py
+-rw-r--r--   0        0        0      616 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/src/anipy_cli/clis/seasonal_cli.py
+-rw-r--r--   0        0        0      916 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/src/anipy_cli/colors.py
+-rw-r--r--   0        0        0    15404 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/src/anipy_cli/config.py
+-rw-r--r--   0        0        0     1160 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/src/anipy_cli/discord.py
+-rw-r--r--   0        0        0     6981 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/src/anipy_cli/mal_proxy.py
+-rw-r--r--   0        0        0      185 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/src/anipy_cli/menus/__init__.py
+-rw-r--r--   0        0        0     1140 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/src/anipy_cli/menus/base_menu.py
+-rw-r--r--   0        0        0    24077 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/src/anipy_cli/menus/mal_menu.py
+-rw-r--r--   0        0        0     6179 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/src/anipy_cli/menus/menu.py
+-rw-r--r--   0        0        0     9097 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/src/anipy_cli/menus/seasonal_menu.py
+-rw-r--r--   0        0        0     7119 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/src/anipy_cli/prompts.py
+-rw-r--r--   0        0        0     7684 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/src/anipy_cli/util.py
+-rw-r--r--   0        0        0     3084 1970-01-01 00:00:00.000000 anipy_cli-3.0.4/PKG-INFO
```

### Comparing `anipy_cli-3.0.3/README.md` & `anipy_cli-3.0.4/README.md`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.3/pyproject.toml` & `anipy_cli-3.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anipy-cli"
-version = "3.0.3"
+version = "3.0.4"
 description = "Watch and Download anime from the comfort of your Terminal"
 authors = ["sdaqo <sdaqo.dev@protonmail.com>"]
 license = "GPL-3.0"
 repository = "https://github.com/sdaqo/anipy-cli"
 homepage = "https://sdaqo.github.io/anipy-cli"
 documentation = "https://sdaqo.github.io/anipy-cli/getting-started-cli"
 keywords = ["anime", "cli"]
```

### Comparing `anipy_cli-3.0.3/src/anipy_cli/arg_parser.py` & `anipy_cli-3.0.4/src/anipy_cli/arg_parser.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.3/src/anipy_cli/cli.py` & `anipy_cli-3.0.4/src/anipy_cli/cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.3/src/anipy_cli/clis/base_cli.py` & `anipy_cli-3.0.4/src/anipy_cli/clis/base_cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.3/src/anipy_cli/clis/binge_cli.py` & `anipy_cli-3.0.4/src/anipy_cli/clis/binge_cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.3/src/anipy_cli/clis/default_cli.py` & `anipy_cli-3.0.4/src/anipy_cli/clis/default_cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.3/src/anipy_cli/clis/download_cli.py` & `anipy_cli-3.0.4/src/anipy_cli/clis/download_cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.3/src/anipy_cli/clis/history_cli.py` & `anipy_cli-3.0.4/src/anipy_cli/clis/history_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         history = self.history_list.get_all()
         history.sort(key=lambda h: h.timestamp, reverse=True)
 
         if not history:
             print("You have no History, exiting")
             sys.exit(0)
 
-        entry = inquirer.select(  # type: ignore
+        entry = inquirer.fuzzy(  # type: ignore
             message="Select History Entry:",
             choices=history,
             long_instruction="To cancel this prompt press ctrl+z",
             mandatory=False,
         ).execute()
 
         if entry is None:
```

### Comparing `anipy_cli-3.0.3/src/anipy_cli/clis/mal_cli.py` & `anipy_cli-3.0.4/src/anipy_cli/clis/mal_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,23 +26,23 @@
     def take_input(self):
         config = Config()
         self.user = config.mal_user
         self.password = self.options.mal_password or config.mal_password
 
         if not self.user:
             self.user = inquirer.text(  # type: ignore
-                "Your MyAnimeList Username: ",
+                "Your MyAnimeList Username:",
                 validate=lambda x: len(x) > 1,
                 invalid_message="You must enter a username!",
                 long_instruction="Hint: You can save your username and password in the config!",
             ).execute()
 
         if not self.password:
             self.password = inquirer.secret(  # type: ignore
-                "Your MyAnimeList Password: ",
+                "Your MyAnimeList Password:",
                 transformer=lambda _: "[hidden]",
                 validate=lambda x: len(x) > 1,
                 invalid_message="You must enter a password!",
                 long_instruction="Hint: You can also pass the password via the `--mal-password` option!",
             ).execute()
 
     def process(self):
```

### Comparing `anipy_cli-3.0.3/src/anipy_cli/clis/seasonal_cli.py` & `anipy_cli-3.0.4/src/anipy_cli/clis/seasonal_cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.3/src/anipy_cli/colors.py` & `anipy_cli-3.0.4/src/anipy_cli/colors.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.3/src/anipy_cli/config.py` & `anipy_cli-3.0.4/src/anipy_cli/config.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.3/src/anipy_cli/discord.py` & `anipy_cli-3.0.4/src/anipy_cli/discord.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.3/src/anipy_cli/mal_proxy.py` & `anipy_cli-3.0.4/src/anipy_cli/mal_proxy.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.3/src/anipy_cli/menus/base_menu.py` & `anipy_cli-3.0.4/src/anipy_cli/menus/base_menu.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.3/src/anipy_cli/menus/mal_menu.py` & `anipy_cli-3.0.4/src/anipy_cli/menus/mal_menu.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
         with DotSpinner("Searching for ", colors.BLUE, query, "..."):
             results = self.mal.get_search(query)
 
         anime = inquirer.fuzzy(  # type: ignore
             message="Select Show:",
             choices=[Choice(value=r, name=self._format_mal_anime(r)) for r in results],
-            transformer=lambda x: [e.split("|")[-1].strip() for e in x],
+            transformer=lambda x: x.split("|")[-1].strip(),
             long_instruction="To skip this prompt press crtl+z",
             mandatory=False,
         ).execute()
 
         if anime is None:
             return
 
@@ -149,15 +149,15 @@
             error("your list is empty")
             return
 
         inquirer.fuzzy(  # type: ignore
             message="View your List",
             choices=mylist,
             mandatory=False,
-            transformer=lambda x: [e.split("|")[-1].strip() for e in x],
+            transformer=lambda x: x.split("|")[-1].strip(),
             long_instruction="To skip this prompt press ctrl+z",
         ).execute()
 
         self.print_options()
 
     def tag_anime(self):
         with DotSpinner("Fetching your MAL..."):
@@ -543,15 +543,15 @@
         if not failed or self.options.auto_update:
             self.print_options()
             print("Everything is mapped")
             return mappings
 
         for f in failed:
             cprint("Manually mapping ", colors.BLUE, f.title)
-            anime = search_show_prompt("mal")
+            anime = search_show_prompt("mal", skip_season_search=True)
             if not anime:
                 continue
 
             map = self.mal_proxy.map_from_mal(f, anime)
             if map is not None:
                 mappings.update({f: map})
 
@@ -614,15 +614,15 @@
                 results = self.mal.get_search(query)
 
             anime = inquirer.fuzzy(  # type: ignore
                 message="Select Show:",
                 choices=[
                     Choice(value=r, name=self._format_mal_anime(r)) for r in results
                 ],
-                transformer=lambda x: [e.split("|")[-1].strip() for e in x],
+                transformer=lambda x: x.split("|")[-1].strip(),
                 long_instruction="To skip this prompt press crtl+z",
                 mandatory=False,
             ).execute()
 
             if not anime:
                 continue
```

### Comparing `anipy_cli-3.0.3/src/anipy_cli/menus/menu.py` & `anipy_cli-3.0.4/src/anipy_cli/menus/menu.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.3/src/anipy_cli/menus/seasonal_menu.py` & `anipy_cli-3.0.4/src/anipy_cli/menus/seasonal_menu.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.3/src/anipy_cli/prompts.py` & `anipy_cli-3.0.4/src/anipy_cli/prompts.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,16 +21,18 @@
 from anipy_cli.config import Config
 
 
 if TYPE_CHECKING:
     from anipy_api.provider import Episode
 
 
-def search_show_prompt(mode: str) -> Optional["Anime"]:
-    if not Config().skip_season_search:
+def search_show_prompt(
+    mode: str, skip_season_search: bool = False
+) -> Optional["Anime"]:
+    if not (Config().skip_season_search or skip_season_search):
         season_provider = None
         for p in get_prefered_providers(mode):
             if p.FILTER_CAPS & (
                 FilterCapabilities.SEASON
                 | FilterCapabilities.YEAR
                 | FilterCapabilities.NO_QUERY
             ):
@@ -61,15 +63,16 @@
                     Anime.from_search_result(provider, x)
                     for x in provider.get_search(query)
                 ]
             )
 
     if len(results) == 0:
         error("no search results")
-        return search_show_prompt(mode)
+        # Do not prompt for season again
+        return search_show_prompt(mode, skip_season_search=True)
 
     anime = inquirer.fuzzy(  # type: ignore
         message="Select Show:",
         choices=results,
         long_instruction="\nS = Anime is available in sub\nD = Anime is available in dub\nTo skip this prompt press ctrl+z",
         mandatory=False,
     ).execute()
```

### Comparing `anipy_cli-3.0.3/src/anipy_cli/util.py` & `anipy_cli-3.0.4/src/anipy_cli/util.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.3/PKG-INFO` & `anipy_cli-3.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anipy-cli
-Version: 3.0.3
+Version: 3.0.4
 Summary: Watch and Download anime from the comfort of your Terminal
 Home-page: https://sdaqo.github.io/anipy-cli
 License: GPL-3.0
 Keywords: anime,cli
 Author: sdaqo
 Author-email: sdaqo.dev@protonmail.com
 Requires-Python: >=3.9,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: anipy-cli Version: 3.0.3 Summary: Watch and
+Metadata-Version: 2.1 Name: anipy-cli Version: 3.0.4 Summary: Watch and
 Download anime from the comfort of your Terminal Home-page: https://
 sdaqo.github.io/anipy-cli License: GPL-3.0 Keywords: anime,cli Author: sdaqo
 Author-email: sdaqo.dev@protonmail.com Requires-Python: >=3.9,<4.0 Classifier:
 License :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
```

