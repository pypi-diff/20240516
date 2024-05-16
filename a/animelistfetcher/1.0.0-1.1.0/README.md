# Comparing `tmp/animelistfetcher-1.0.0.tar.gz` & `tmp/animelistfetcher-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "animelistfetcher-1.0.0.tar", last modified: Tue May 14 12:24:18 2024, max compression
+gzip compressed data, was "animelistfetcher-1.1.0.tar", last modified: Thu May 16 21:51:48 2024, max compression
```

## Comparing `animelistfetcher-1.0.0.tar` & `animelistfetcher-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:24:18.921450 animelistfetcher-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-05-14 12:24:14.000000 animelistfetcher-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-14 12:24:18.921450 animelistfetcher-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-14 12:24:14.000000 animelistfetcher-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:24:18.921450 animelistfetcher-1.0.0/animelistfetcher/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-14 12:24:14.000000 animelistfetcher-1.0.0/animelistfetcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-14 12:24:14.000000 animelistfetcher-1.0.0/animelistfetcher/animelist_fetcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:24:18.921450 animelistfetcher-1.0.0/animelistfetcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-14 12:24:18.000000 animelistfetcher-1.0.0/animelistfetcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-14 12:24:18.000000 animelistfetcher-1.0.0/animelistfetcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 12:24:18.000000 animelistfetcher-1.0.0/animelistfetcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-14 12:24:18.000000 animelistfetcher-1.0.0/animelistfetcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-14 12:24:18.000000 animelistfetcher-1.0.0/animelistfetcher.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-14 12:24:14.000000 animelistfetcher-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 12:24:18.921450 animelistfetcher-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-14 12:24:14.000000 animelistfetcher-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:51:48.604089 animelistfetcher-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-05-16 21:51:43.000000 animelistfetcher-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-16 21:51:48.600089 animelistfetcher-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-05-16 21:51:43.000000 animelistfetcher-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:51:48.600089 animelistfetcher-1.1.0/animelistfetcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-16 21:51:43.000000 animelistfetcher-1.1.0/animelistfetcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-05-16 21:51:43.000000 animelistfetcher-1.1.0/animelistfetcher/animelist_fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:51:48.600089 animelistfetcher-1.1.0/animelistfetcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-16 21:51:48.000000 animelistfetcher-1.1.0/animelistfetcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-16 21:51:48.000000 animelistfetcher-1.1.0/animelistfetcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 21:51:48.000000 animelistfetcher-1.1.0/animelistfetcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-16 21:51:48.000000 animelistfetcher-1.1.0/animelistfetcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-16 21:51:48.000000 animelistfetcher-1.1.0/animelistfetcher.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-16 21:51:43.000000 animelistfetcher-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 21:51:48.604089 animelistfetcher-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-16 21:51:43.000000 animelistfetcher-1.1.0/setup.py
```

### Comparing `animelistfetcher-1.0.0/LICENSE` & `animelistfetcher-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `animelistfetcher-1.0.0/PKG-INFO` & `animelistfetcher-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animelistfetcher
-Version: 1.0.0
+Version: 1.1.0
 Summary: A Python wrapper for my anime libraries
 Author: Dominik Procházka
 Maintainer: Dominik Procházka
 Project-URL: Homepage, https://github.com/prochy-exe/animelistfetcher
 Project-URL: Documentation, https://github.com/prochy-exe/animelistfetcher/wiki
 Project-URL: Source, https://github.com/prochy-exe/animelistfetcher
 Keywords: python,anilist,al,mal,myanimelist
@@ -68,14 +68,16 @@
 * When importing this library for the first time, you will be taken through the setup process
 
 ## Help
 
 If you encounter any issues, feel free to open a new issue. If you have any new ideas or fixes, please open a pull request, they are more than welcome!
 
 ## Version History
+* [1.1.0](https://github.com/prochy-exe/animelistfetcher/releases/tag/v1.1.0)
+    * [import libraries when necessary](https://github.com/prochy-exe/animelistfetcher/commit/1367260f28f0d100f71d492d0ccbe8b44edfcc04)
 * [1.0.0](https://github.com/prochy-exe/animelistfetcher/releases/tag/v1.0.0)
     * [Initial Release](https://github.com/prochy-exe/animelistfetcher/commit/06b2666c3f0c938bd4ee66d8b7019a7f4c0377cf)
 
 ## Acknowledgments
 
 Huge thanks to the AniList and MyAnimeList teams:
 * [AniList](https://anilist.co/home)
```

### Comparing `animelistfetcher-1.0.0/README.md` & `animelistfetcher-1.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -42,14 +42,16 @@
 * When importing this library for the first time, you will be taken through the setup process
 
 ## Help
 
 If you encounter any issues, feel free to open a new issue. If you have any new ideas or fixes, please open a pull request, they are more than welcome!
 
 ## Version History
+* [1.1.0](https://github.com/prochy-exe/animelistfetcher/releases/tag/v1.1.0)
+    * [import libraries when necessary](https://github.com/prochy-exe/animelistfetcher/commit/1367260f28f0d100f71d492d0ccbe8b44edfcc04)
 * [1.0.0](https://github.com/prochy-exe/animelistfetcher/releases/tag/v1.0.0)
     * [Initial Release](https://github.com/prochy-exe/animelistfetcher/commit/06b2666c3f0c938bd4ee66d8b7019a7f4c0377cf)
 
 ## Acknowledgments
 
 Huge thanks to the AniList and MyAnimeList teams:
 * [AniList](https://anilist.co/home)
```

### Comparing `animelistfetcher-1.0.0/animelistfetcher/animelist_fetcher.py` & `animelistfetcher-1.1.0/animelistfetcher/animelist_fetcher.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,64 +1,81 @@
-import alfetcher, malfetcher, time
+import time
 
 def get_userdata(service, service_token = None):
     service = service.lower()
     if service == "al" or service == "anilist":
+        import alfetcher
         return alfetcher.get_userdata(service_token)
     elif service == "mal" or service == "myanimelist":
+        import malfetcher
         return malfetcher.get_userdata(service_token)
 
 def clear_cache(service):
     service = service.lower()
     if service == "al" or service == "anilist":
+        import alfetcher
         return alfetcher.clear_cache()
     elif service == "mal" or service == "myanimelist":
+        import malfetcher
         return malfetcher.clear_cache()
 
 def config():
+    import alfetcher, malfetcher
     print("Starting AniList setup")
     alfetcher.config_setup()
     time.sleep(5)
     print("Starting MyAnimeList setup")
     malfetcher.config_setup()
 
 def get_latest_anime_entry_for_user(service, status = "ALL", service_token = None, username = None):
     service = service.lower()
     if service == "al" or service == "anilist":
+        import alfetcher
         return alfetcher.get_latest_anime_entry_for_user(status, service_token, username)
     elif service == "mal" or service == "myanimelist":
+        import malfetcher
         return malfetcher.get_latest_anime_entry_for_user(status, service_token, username)
 
 def get_all_anime_for_user(service, status_array = "ALL", service_token = None, username = None):
     service = service.lower()
     if service == "al" or service == "anilist":
+        import alfetcher
         return alfetcher.get_all_anime_for_user(status_array, service_token, username)
     elif service == "mal" or service == "myanimelist":
+        import malfetcher
         return malfetcher.get_all_anime_for_user(status_array, service_token, username)
 
 def get_anime_entry_for_user(service, anime_id, service_token = None, username = None):
     service = service.lower()
     if service == "al" or service == "anilist":
+        import alfetcher
         return alfetcher.get_anime_entry_for_user(anime_id, service_token, username)
     elif service == "mal" or service == "myanimelist":
+        import malfetcher
         return malfetcher.get_anime_entry_for_user(anime_id, service_token)
 
 def get_anime_info(service, anime_id, service_token = None):
     service = service.lower()
     if service == "al" or service == "anilist":
+        import alfetcher
         return alfetcher.get_anime_info(anime_id, False, service_token)
     elif service == "mal" or service == "myanimelist":
+        import malfetcher
         return malfetcher.get_anime_info(anime_id, False, service_token)
 
 def get_id(service, search_string, service_token = None):
     service = service.lower()
     if service == "al" or service == "anilist":
+        import alfetcher
         return alfetcher.get_id(search_string, service_token)
     elif service == "mal" or service == "myanimelist":
+        import malfetcher
         return malfetcher.get_id(search_string, service_token)
 
 def update_entry(service, anime_id, progress, service_token=None):
     service = service.lower()
     if service == "al" or service == "anilist":
+        import alfetcher
         return alfetcher.update_entry(anime_id, progress, service_token)
     elif service == "mal" or service == "myanimelist":
+        import malfetcher
         return malfetcher.update_entry(anime_id, progress, service_token)
```

### Comparing `animelistfetcher-1.0.0/animelistfetcher.egg-info/PKG-INFO` & `animelistfetcher-1.1.0/animelistfetcher.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animelistfetcher
-Version: 1.0.0
+Version: 1.1.0
 Summary: A Python wrapper for my anime libraries
 Author: Dominik Procházka
 Maintainer: Dominik Procházka
 Project-URL: Homepage, https://github.com/prochy-exe/animelistfetcher
 Project-URL: Documentation, https://github.com/prochy-exe/animelistfetcher/wiki
 Project-URL: Source, https://github.com/prochy-exe/animelistfetcher
 Keywords: python,anilist,al,mal,myanimelist
@@ -68,14 +68,16 @@
 * When importing this library for the first time, you will be taken through the setup process
 
 ## Help
 
 If you encounter any issues, feel free to open a new issue. If you have any new ideas or fixes, please open a pull request, they are more than welcome!
 
 ## Version History
+* [1.1.0](https://github.com/prochy-exe/animelistfetcher/releases/tag/v1.1.0)
+    * [import libraries when necessary](https://github.com/prochy-exe/animelistfetcher/commit/1367260f28f0d100f71d492d0ccbe8b44edfcc04)
 * [1.0.0](https://github.com/prochy-exe/animelistfetcher/releases/tag/v1.0.0)
     * [Initial Release](https://github.com/prochy-exe/animelistfetcher/commit/06b2666c3f0c938bd4ee66d8b7019a7f4c0377cf)
 
 ## Acknowledgments
 
 Huge thanks to the AniList and MyAnimeList teams:
 * [AniList](https://anilist.co/home)
```

### Comparing `animelistfetcher-1.0.0/pyproject.toml` & `animelistfetcher-1.1.0/pyproject.toml`

 * *Files identical despite different names*

