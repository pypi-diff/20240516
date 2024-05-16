# Comparing `tmp/plextraktsync-0.30.6.tar.gz` & `tmp/plextraktsync-0.30.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plextraktsync-0.30.6.tar", last modified: Sat May 11 08:46:16 2024, max compression
+gzip compressed data, was "plextraktsync-0.30.7.tar", last modified: Wed May 15 18:42:12 2024, max compression
```

## Comparing `plextraktsync-0.30.6.tar` & `plextraktsync-0.30.7.tar`

### file list

```diff
@@ -1,171 +1,172 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 08:46:16.287308 plextraktsync-0.30.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    30223 2024-05-11 08:46:16.287308 plextraktsync-0.30.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 08:46:16.287308 plextraktsync-0.30.6/PlexTraktSync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    30223 2024-05-11 08:46:16.000000 plextraktsync-0.30.6/PlexTraktSync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-05-11 08:46:16.000000 plextraktsync-0.30.6/PlexTraktSync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 08:46:16.000000 plextraktsync-0.30.6/PlexTraktSync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-11 08:46:16.000000 plextraktsync-0.30.6/PlexTraktSync.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-11 08:46:16.000000 plextraktsync-0.30.6/PlexTraktSync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-11 08:46:16.000000 plextraktsync-0.30.6/PlexTraktSync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    26819 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 08:46:16.263308 plextraktsync-0.30.6/plextraktsync/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-11 08:46:12.000000 plextraktsync-0.30.6/plextraktsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 08:46:16.267308 plextraktsync-0.30.6/plextraktsync/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/commands/bug_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/commands/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/commands/clear_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/commands/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/commands/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/commands/imdb_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/commands/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/commands/inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/commands/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/commands/plex_login.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/commands/self_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/commands/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/commands/trakt_login.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/commands/unmatched.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/commands/watch.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/commands/watched_shows.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 08:46:16.271308 plextraktsync-0.30.6/plextraktsync/config/
--rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/config/Config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/config/ConfigLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/config/ConfigMergeMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/config/HttpCacheConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/config/PlexServerConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/config/RunConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/config/ServerConfigFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/config/SyncConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/config.default.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 08:46:16.271308 plextraktsync-0.30.6/plextraktsync/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/decorators/coro.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/decorators/flatten.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/decorators/measure_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/decorators/memoize.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/decorators/nocache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/decorators/rate_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/decorators/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/decorators/time_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 08:46:16.271308 plextraktsync-0.30.6/plextraktsync/logger/
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/logger/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/logger/init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 08:46:16.271308 plextraktsync-0.30.6/plextraktsync/media/
--rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/media/Media.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/media/MediaFactory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 08:46:16.271308 plextraktsync-0.30.6/plextraktsync/mixin/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/mixin/ChangeNotifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/mixin/RichMarkup.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/mixin/SetWindowTitle.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/path.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 08:46:16.271308 plextraktsync-0.30.6/plextraktsync/plan/
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/plan/WalkConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/plan/WalkPlan.py
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/plan/WalkPlanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     7534 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/plan/Walker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 08:46:16.275308 plextraktsync-0.30.6/plextraktsync/plex/
--rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/plex/PlexApi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/plex/PlexAudioCodec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/plex/PlexGuid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/plex/PlexGuidProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/plex/PlexGuidProviderIMDB.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/plex/PlexGuidProviderLocal.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/plex/PlexGuidProviderMbid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/plex/PlexGuidProviderTMDB.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/plex/PlexGuidProviderTVDB.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/plex/PlexId.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/plex/PlexIdFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)    11251 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/plex/PlexLibraryItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/plex/PlexLibrarySection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/plex/PlexPlaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/plex/PlexPlaylistCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/plex/PlexRatings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/plex/PlexSectionPager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/plex/PlexServerConnection.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/plex/PlexWatchList.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/plex/SessionCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/plex/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 08:46:16.275308 plextraktsync-0.30.6/plextraktsync/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/pytrakt_extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 08:46:16.275308 plextraktsync-0.30.6/plextraktsync/queue/
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/queue/BackgroundTask.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/queue/Queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/queue/TraktBatchWorker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/queue/TraktMarkWatchedWorker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/queue/TraktScrobbleWorker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 08:46:16.279308 plextraktsync-0.30.6/plextraktsync/rich/
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/rich/RichHighlighter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/rich/RichProgressBar.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/style.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 08:46:16.279308 plextraktsync-0.30.6/plextraktsync/sync/
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/sync/AddCollectionPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/sync/ClearCollectedPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/sync/LikedListsPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/sync/Sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/sync/SyncRatingsPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/sync/SyncWatchedPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/sync/TraktListsPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/sync/WatchListPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/sync/WatchProgressPlugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 08:46:16.279308 plextraktsync-0.30.6/plextraktsync/sync/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/sync/plugin/SyncPluginInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/sync/plugin/SyncPluginManager.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/sync/plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 08:46:16.283308 plextraktsync-0.30.6/plextraktsync/trakt/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/trakt/PartialTraktMedia.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/trakt/ScrobblerCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/trakt/ScrobblerProxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/trakt/TraktApi.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/trakt/TraktItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/trakt/TraktLookup.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/trakt/TraktRatingCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/trakt/TraktUserList.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/trakt/TraktUserListCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/trakt/TraktWatchlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/trakt/WatchProgress.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/trakt/trakt_set.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/trakt/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 08:46:16.283308 plextraktsync-0.30.6/plextraktsync/util/
--rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/util/Factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/util/Path.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/util/Rating.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/util/Timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/util/Version.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/util/execp.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/util/execx.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/util/expand_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/util/git_version_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/util/local_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/util/openurl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/util/packaging.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/util/parse_date.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/util/remove_empty_values.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 08:46:16.283308 plextraktsync-0.30.6/plextraktsync/watch/
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/watch/EventDispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/watch/EventFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/watch/ProgressBar.py
--rw-r--r--   0 runner    (1001) docker     (127)     6917 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/watch/WatchStateUpdater.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/watch/WebSocketListener.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/plextraktsync/watch/events.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-11 08:46:13.000000 plextraktsync-0.30.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-11 08:46:16.287308 plextraktsync-0.30.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 08:46:16.287308 plextraktsync-0.30.6/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1923 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/tests/test_collection_metadata.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1443 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/tests/test_config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2703 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/tests/test_events.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      341 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/tests/test_logger.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      977 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/tests/test_new_agent.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2104 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/tests/test_plex_id.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      529 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/tests/test_rating.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      503 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/tests/test_threading.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1174 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/tests/test_timer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      572 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/tests/test_trakt_progress.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3584 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/tests/test_tv_lookup.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1977 2024-05-11 08:46:11.000000 plextraktsync-0.30.6/tests/test_walker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:42:12.168187 plextraktsync-0.30.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    30195 2024-05-15 18:42:12.168187 plextraktsync-0.30.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:42:12.168187 plextraktsync-0.30.7/PlexTraktSync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    30195 2024-05-15 18:42:12.000000 plextraktsync-0.30.7/PlexTraktSync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-05-15 18:42:12.000000 plextraktsync-0.30.7/PlexTraktSync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 18:42:12.000000 plextraktsync-0.30.7/PlexTraktSync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-15 18:42:12.000000 plextraktsync-0.30.7/PlexTraktSync.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-15 18:42:12.000000 plextraktsync-0.30.7/PlexTraktSync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 18:42:12.000000 plextraktsync-0.30.7/PlexTraktSync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    26819 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:42:12.148187 plextraktsync-0.30.7/plextraktsync/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-15 18:42:00.000000 plextraktsync-0.30.7/plextraktsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:42:12.148187 plextraktsync-0.30.7/plextraktsync/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/commands/bug_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/commands/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/commands/clear_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/commands/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/commands/imdb_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/commands/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/commands/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/commands/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/commands/plex_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/commands/self_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/commands/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/commands/trakt_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/commands/unmatched.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/commands/watch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/commands/watched_shows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:42:12.152186 plextraktsync-0.30.7/plextraktsync/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/config/Config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/config/ConfigLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/config/ConfigMergeMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/config/HttpCacheConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/config/PlexServerConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/config/RunConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/config/ServerConfigFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/config/SyncConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/config.default.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:42:12.152186 plextraktsync-0.30.7/plextraktsync/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/decorators/coro.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/decorators/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/decorators/measure_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/decorators/memoize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/decorators/nocache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/decorators/rate_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/decorators/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/decorators/time_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:42:12.152186 plextraktsync-0.30.7/plextraktsync/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/logger/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/logger/init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:42:12.152186 plextraktsync-0.30.7/plextraktsync/media/
+-rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/media/Media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/media/MediaFactory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:42:12.152186 plextraktsync-0.30.7/plextraktsync/mixin/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/mixin/ChangeNotifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/mixin/RichMarkup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/mixin/SetWindowTitle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/path.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:42:12.152186 plextraktsync-0.30.7/plextraktsync/plan/
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/plan/WalkConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/plan/WalkPlan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/plan/WalkPlanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8091 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/plan/Walker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:42:12.156187 plextraktsync-0.30.7/plextraktsync/plex/
+-rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/plex/PlexApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/plex/PlexAudioCodec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/plex/PlexGuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/plex/PlexGuidProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/plex/PlexGuidProviderIMDB.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/plex/PlexGuidProviderLocal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/plex/PlexGuidProviderMbid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/plex/PlexGuidProviderTMDB.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/plex/PlexGuidProviderTVDB.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/plex/PlexId.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/plex/PlexIdFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11251 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/plex/PlexLibraryItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/plex/PlexLibrarySection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/plex/PlexPlaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/plex/PlexPlaylistCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/plex/PlexRatings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/plex/PlexSectionPager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/plex/PlexServerConnection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/plex/PlexWatchList.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/plex/SessionCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/plex/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:42:12.156187 plextraktsync-0.30.7/plextraktsync/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/pytrakt_extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:42:12.160187 plextraktsync-0.30.7/plextraktsync/queue/
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/queue/BackgroundTask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/queue/Queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/queue/TraktBatchWorker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/queue/TraktMarkWatchedWorker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/queue/TraktScrobbleWorker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:42:12.160187 plextraktsync-0.30.7/plextraktsync/rich/
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/rich/RichHighlighter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/rich/RichProgressBar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/style.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:42:12.160187 plextraktsync-0.30.7/plextraktsync/sync/
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/sync/AddCollectionPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/sync/ClearCollectedPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/sync/LikedListsPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/sync/Sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/sync/SyncRatingsPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/sync/SyncWatchedPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/sync/TraktListsPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/sync/WatchListPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/sync/WatchProgressPlugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:42:12.160187 plextraktsync-0.30.7/plextraktsync/sync/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/sync/plugin/SyncPluginInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/sync/plugin/SyncPluginManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/sync/plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:42:12.164187 plextraktsync-0.30.7/plextraktsync/trakt/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/trakt/PartialTraktMedia.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/trakt/ScrobblerCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/trakt/ScrobblerProxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/trakt/TraktApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/trakt/TraktItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/trakt/TraktLookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/trakt/TraktRatingCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/trakt/TraktUserList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/trakt/TraktUserListCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/trakt/TraktWatchlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/trakt/WatchProgress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/trakt/trakt_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/trakt/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:42:12.164187 plextraktsync-0.30.7/plextraktsync/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/util/Factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/util/Path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/util/Rating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/util/Timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/util/Version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/util/execp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/util/execx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/util/expand_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/util/git_version_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/util/local_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/util/openurl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/util/packaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/util/parse_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/util/remove_empty_values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:42:12.168187 plextraktsync-0.30.7/plextraktsync/watch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/watch/EventDispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/watch/EventFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/watch/ProgressBar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6917 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/watch/WatchStateUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/watch/WebSocketListener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/plextraktsync/watch/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-15 18:42:08.000000 plextraktsync-0.30.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-15 18:42:12.172187 plextraktsync-0.30.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:42:12.168187 plextraktsync-0.30.7/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1964 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/tests/test_collection_metadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1499 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/tests/test_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2703 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/tests/test_events.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      341 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/tests/test_logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      977 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/tests/test_new_agent.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2104 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/tests/test_plex_id.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      224 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/tests/test_plugin.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      529 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/tests/test_rating.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      503 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/tests/test_threading.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1174 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/tests/test_timer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      627 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/tests/test_trakt_progress.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3762 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/tests/test_tv_lookup.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1977 2024-05-15 18:41:59.000000 plextraktsync-0.30.7/tests/test_walker.py
```

### Comparing `plextraktsync-0.30.6/LICENSE` & `plextraktsync-0.30.7/LICENSE`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/PKG-INFO` & `plextraktsync-0.30.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlexTraktSync
-Version: 0.30.6
+Version: 0.30.7
 Summary: Plex-Trakt-Sync is a two-way-sync between trakt.tv and Plex Media Server
 Home-page: https://github.com/Taxel/PlexTraktSync
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Taxel/PlexTraktSync/issues
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,15 +30,15 @@
 Requires-Dist: humanize==4.9.0; python_version >= "3.8"
 Requires-Dist: idna==3.7; python_version >= "3.5"
 Requires-Dist: inquirerpy==0.3.4; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: markdown-it-py==3.0.0; python_version >= "3.7" and python_version >= "3.8"
 Requires-Dist: mdurl==0.1.2; python_version >= "3.7"
 Requires-Dist: oauthlib==3.2.2; python_version >= "3.6"
 Requires-Dist: pfzy==0.3.4; python_version >= "3.7" and python_version < "4.0"
-Requires-Dist: platformdirs==4.2.1; python_version >= "3.7" and python_version >= "3.8"
+Requires-Dist: platformdirs==4.2.2; python_version >= "3.8"
 Requires-Dist: plexapi==4.15.12; python_version >= "3.8"
 Requires-Dist: pluggy==1.5.0; python_version >= "3.8"
 Requires-Dist: prompt-toolkit==3.0.43; python_full_version >= "3.7.0"
 Requires-Dist: pygments==2.18.0; python_version >= "3.8"
 Requires-Dist: python-dotenv==1.0.1; python_version >= "3.8"
 Requires-Dist: python-git-info==0.8.3
 Requires-Dist: pytimeparse==1.1.8
```

### Comparing `plextraktsync-0.30.6/PlexTraktSync.egg-info/PKG-INFO` & `plextraktsync-0.30.7/PlexTraktSync.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlexTraktSync
-Version: 0.30.6
+Version: 0.30.7
 Summary: Plex-Trakt-Sync is a two-way-sync between trakt.tv and Plex Media Server
 Home-page: https://github.com/Taxel/PlexTraktSync
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Taxel/PlexTraktSync/issues
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,15 +30,15 @@
 Requires-Dist: humanize==4.9.0; python_version >= "3.8"
 Requires-Dist: idna==3.7; python_version >= "3.5"
 Requires-Dist: inquirerpy==0.3.4; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: markdown-it-py==3.0.0; python_version >= "3.7" and python_version >= "3.8"
 Requires-Dist: mdurl==0.1.2; python_version >= "3.7"
 Requires-Dist: oauthlib==3.2.2; python_version >= "3.6"
 Requires-Dist: pfzy==0.3.4; python_version >= "3.7" and python_version < "4.0"
-Requires-Dist: platformdirs==4.2.1; python_version >= "3.7" and python_version >= "3.8"
+Requires-Dist: platformdirs==4.2.2; python_version >= "3.8"
 Requires-Dist: plexapi==4.15.12; python_version >= "3.8"
 Requires-Dist: pluggy==1.5.0; python_version >= "3.8"
 Requires-Dist: prompt-toolkit==3.0.43; python_full_version >= "3.7.0"
 Requires-Dist: pygments==2.18.0; python_version >= "3.8"
 Requires-Dist: python-dotenv==1.0.1; python_version >= "3.8"
 Requires-Dist: python-git-info==0.8.3
 Requires-Dist: pytimeparse==1.1.8
```

### Comparing `plextraktsync-0.30.6/PlexTraktSync.egg-info/SOURCES.txt` & `plextraktsync-0.30.7/PlexTraktSync.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -138,13 +138,14 @@
 plextraktsync/watch/events.py
 tests/test_collection_metadata.py
 tests/test_config.py
 tests/test_events.py
 tests/test_logger.py
 tests/test_new_agent.py
 tests/test_plex_id.py
+tests/test_plugin.py
 tests/test_rating.py
 tests/test_threading.py
 tests/test_timer.py
 tests/test_trakt_progress.py
 tests/test_tv_lookup.py
 tests/test_walker.py
```

### Comparing `plextraktsync-0.30.6/PlexTraktSync.egg-info/requires.txt` & `plextraktsync-0.30.7/PlexTraktSync.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -48,19 +48,19 @@
 [:python_version >= "3.7" and python_version < "4.0"]
 inquirerpy==0.3.4
 pfzy==0.3.4
 
 [:python_version >= "3.7" and python_version >= "3.8"]
 cattrs==23.2.3
 markdown-it-py==3.0.0
-platformdirs==4.2.1
 
 [:python_version >= "3.8"]
 apluggy==0.9.4
 humanize==4.9.0
+platformdirs==4.2.2
 plexapi==4.15.12
 pluggy==1.5.0
 pygments==2.18.0
 python-dotenv==1.0.1
 requests-cache==1.2.0
 types-decorator==5.1.8.20240310
 urllib3==2.2.1
```

### Comparing `plextraktsync-0.30.6/README.md` & `plextraktsync-0.30.7/README.md`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/cli.py` & `plextraktsync-0.30.7/plextraktsync/cli.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/commands/bug_report.py` & `plextraktsync-0.30.7/plextraktsync/commands/bug_report.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/commands/cache.py` & `plextraktsync-0.30.7/plextraktsync/commands/cache.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/commands/clear_collections.py` & `plextraktsync-0.30.7/plextraktsync/commands/clear_collections.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/commands/config.py` & `plextraktsync-0.30.7/plextraktsync/commands/config.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/commands/download.py` & `plextraktsync-0.30.7/plextraktsync/commands/download.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/commands/imdb_import.py` & `plextraktsync-0.30.7/plextraktsync/commands/imdb_import.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/commands/info.py` & `plextraktsync-0.30.7/plextraktsync/commands/info.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/commands/inspect.py` & `plextraktsync-0.30.7/plextraktsync/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/commands/login.py` & `plextraktsync-0.30.7/plextraktsync/commands/login.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/commands/plex_login.py` & `plextraktsync-0.30.7/plextraktsync/commands/plex_login.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/commands/self_update.py` & `plextraktsync-0.30.7/plextraktsync/commands/self_update.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/commands/sync.py` & `plextraktsync-0.30.7/plextraktsync/commands/sync.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/commands/trakt_login.py` & `plextraktsync-0.30.7/plextraktsync/commands/trakt_login.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/commands/unmatched.py` & `plextraktsync-0.30.7/plextraktsync/commands/unmatched.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/commands/watch.py` & `plextraktsync-0.30.7/plextraktsync/commands/watch.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/commands/watched_shows.py` & `plextraktsync-0.30.7/plextraktsync/commands/watched_shows.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/config/Config.py` & `plextraktsync-0.30.7/plextraktsync/config/Config.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/config/ConfigLoader.py` & `plextraktsync-0.30.7/plextraktsync/config/ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/config/HttpCacheConfig.py` & `plextraktsync-0.30.7/plextraktsync/config/HttpCacheConfig.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/config/PlexServerConfig.py` & `plextraktsync-0.30.7/plextraktsync/config/PlexServerConfig.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/config/ServerConfigFactory.py` & `plextraktsync-0.30.7/plextraktsync/config/ServerConfigFactory.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/config/SyncConfig.py` & `plextraktsync-0.30.7/plextraktsync/config/SyncConfig.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/config.default.yml` & `plextraktsync-0.30.7/plextraktsync/config.default.yml`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/decorators/measure_time.py` & `plextraktsync-0.30.7/plextraktsync/decorators/measure_time.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/decorators/rate_limit.py` & `plextraktsync-0.30.7/plextraktsync/decorators/rate_limit.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/decorators/retry.py` & `plextraktsync-0.30.7/plextraktsync/decorators/retry.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/logger/filter.py` & `plextraktsync-0.30.7/plextraktsync/logger/filter.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/logger/init.py` & `plextraktsync-0.30.7/plextraktsync/logger/init.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/media/Media.py` & `plextraktsync-0.30.7/plextraktsync/media/Media.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/media/MediaFactory.py` & `plextraktsync-0.30.7/plextraktsync/media/MediaFactory.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/mixin/ChangeNotifier.py` & `plextraktsync-0.30.7/plextraktsync/mixin/ChangeNotifier.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/plan/WalkConfig.py` & `plextraktsync-0.30.7/plextraktsync/plan/WalkConfig.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/plan/WalkPlanner.py` & `plextraktsync-0.30.7/plextraktsync/plan/WalkPlanner.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/plan/Walker.py` & `plextraktsync-0.30.7/plextraktsync/plan/Walker.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,23 +8,25 @@
 from plextraktsync.mixin.SetWindowTitle import SetWindowTitle
 from plextraktsync.plex.PlexGuid import PlexGuid
 from plextraktsync.plex.PlexLibraryItem import PlexLibraryItem
 from plextraktsync.trakt.TraktApi import TraktApi
 from plextraktsync.trakt.TraktItem import TraktItem
 
 if TYPE_CHECKING:
-    from typing import Any, Generator, Iterable
+    from typing import Any, AsyncGenerator, AsyncIterable, Generator, Iterable
 
     from plexapi.video import Episode
 
     from plextraktsync.media.Media import Media
     from plextraktsync.media.MediaFactory import MediaFactory
     from plextraktsync.plan.WalkConfig import WalkConfig
     from plextraktsync.plex.PlexApi import PlexApi
     from plextraktsync.plex.PlexLibrarySection import PlexLibrarySection
+    from plextraktsync.plex.PlexWatchList import PlexWatchList
+    from plextraktsync.trakt.TraktWatchlist import TraktWatchList
 
 
 class Walker(SetWindowTitle):
     """
     Class dealing with finding and walking library, movies/shows, episodes
     """
     logger = logging.getLogger(__name__)
@@ -65,144 +67,152 @@
 
         if self.plan.shows:
             print(f"Sync Shows: {[x.title for x in self.plan.shows]}")
 
         if self.plan.episodes:
             print(f"Sync Episodes: {[x.title for x in self.plan.episodes]}")
 
-    def get_plex_movies(self) -> Generator[PlexLibraryItem, Any, None]:
+    async def get_plex_movies(self) -> Generator[PlexLibraryItem, Any, None]:
         """
         Iterate over movie sections unless specific movie is requested
         """
         if self.plan.movies:
             movies = self.media_from_items("movie", self.plan.movies)
         elif self.plan.movie_sections:
             movies = self.media_from_sections(self.plan.movie_sections)
         else:
             return
 
-        yield from movies
+        async for m in movies:
+            yield m
 
-    def find_movies(self) -> Generator[Media, Any, None]:
-        for plex in self.get_plex_movies():
+    async def find_movies(self) -> Generator[Media, Any, None]:
+        async for plex in self.get_plex_movies():
             movie = self.mf.resolve_any(plex)
             if not movie:
                 continue
             yield movie
 
-    def get_plex_shows(self) -> Generator[PlexLibraryItem, Any, None]:
+    async def get_plex_shows(self) -> AsyncGenerator[PlexLibraryItem, Any, None]:
         if self.plan.shows:
-            shows = self.media_from_items("show", self.plan.shows)
+            it = self.media_from_items("show", self.plan.shows)
         elif self.plan.show_sections:
-            shows = self.media_from_sections(self.plan.show_sections)
+            it = self.media_from_sections(self.plan.show_sections)
         else:
             return
 
-        yield from shows
+        async for m in it:
+            yield m
 
-    def find_episodes(self):
+    async def find_episodes(self):
         if self.plan.episodes:
-            yield from self.get_plex_episodes(self.plan.episodes)
+            async for m in self.get_plex_episodes(self.plan.episodes):
+                yield m
 
         # Preload plex shows
         plex_shows: dict[int, PlexLibraryItem] = {}
         self.logger.info("Preload shows data")
-        for show in self.get_plex_shows():
+        async for show in self.get_plex_shows():
             plex_shows[show.key] = show
         self.logger.info(f"Preloaded shows data ({len(plex_shows)} shows)")
 
         # Preload matches for shows
         show_cache: dict[int, Media] = {}
         self.logger.info("Preload shows matches")
         it = self.progressbar(plex_shows.items(), desc="Processing show matches")
-        for show_id, ps in it:
+        async for show_id, ps in it:
             show_cache[show_id] = self.mf.resolve_any(ps)
         self.logger.info(f"Preloaded shows matches ({len(show_cache)} shows)")
 
-        for ep in self.episodes_from_sections(self.plan.show_sections):
+        async for ep in self.episodes_from_sections(self.plan.show_sections):
             show_id = ep.show_id
             ep.show = plex_shows[show_id]
             show = show_cache[show_id] if show_id in show_cache else None
             m = self.mf.resolve_any(ep, show)
             if not m:
                 continue
             if show:
                 m.show = show
             show_cache[show_id] = m.show
             yield m
 
-    def walk_shows(self, shows: set[Media], title="Processing Shows"):
+    async def walk_shows(self, shows: set[Media], title="Processing Shows"):
         if not shows:
             return
-        yield from self.progressbar(shows, desc=title)
+        async for show in self.progressbar(shows, desc=title):
+            yield show
 
-    def get_plex_episodes(self, episodes: list[Episode]) -> Generator[Media, Any, None]:
+    async def get_plex_episodes(self, episodes: list[Episode]) -> Generator[Media, Any, None]:
         it = self.progressbar(episodes, desc="Processing episodes")
-        for pe in it:
+        async for pe in it:
             guid = PlexGuid(pe.grandparentGuid, "show")
             show = self.mf.resolve_guid(guid)
             if not show:
                 continue
             me = self.mf.resolve_any(PlexLibraryItem(pe, plex=self.plex), show)
             if not me:
                 continue
 
             me.show = show
             yield me
 
-    def media_from_sections(self, sections: list[PlexLibrarySection]) -> Generator[PlexLibraryItem, Any, None]:
+    async def media_from_sections(self, sections: list[PlexLibrarySection]) -> AsyncGenerator[PlexLibraryItem, Any, None]:
         for section in sections:
             with measure_time(f"{section.title_link} processed", extra={"markup": True}):
                 self.set_window_title(f"Processing {section.title}")
                 it = self.progressbar(
                     section.pager(),
                     desc=f"Processing {section.title_link}",
                 )
-                yield from it
+                async for m in it:
+                    yield m
 
-    def episodes_from_sections(self, sections: list[PlexLibrarySection]) -> Generator[PlexLibraryItem, Any, None]:
+    async def episodes_from_sections(self, sections: list[PlexLibrarySection]) -> Generator[PlexLibraryItem, Any, None]:
         for section in sections:
             with measure_time(f"{section.title_link} processed", extra={"markup": True}):
                 self.set_window_title(f"Processing {section.title}")
                 it = self.progressbar(
                     section.pager("episode"),
                     desc=f"Processing {section.title_link}",
                 )
-                yield from it
+                async for m in it:
+                    yield m
 
-    def media_from_items(self, libtype: str, items: list) -> Generator[PlexLibraryItem, Any, None]:
+    async def media_from_items(self, libtype: str, items: list) -> AsyncGenerator[PlexLibraryItem, Any, None]:
         it = self.progressbar(items, desc=f"Processing {libtype}s")
-        for m in it:
+        async for m in it:
             yield PlexLibraryItem(m, plex=self.plex)
 
-    def episode_from_show(self, show: Media) -> Generator[Media, Any, None]:
+    async def episode_from_show(self, show: Media) -> Generator[Media, Any, None]:
         for pe in show.plex.episodes():
             me = self.mf.resolve_any(pe, show)
             if not me:
                 continue
 
             me.show = show
             yield me
 
-    def progressbar(self, iterable: Iterable, **kwargs):
+    async def progressbar(self, iterable: AsyncIterable | Iterable, **kwargs):
         if self._progressbar:
             pb = self._progressbar(iterable, **kwargs)
             with pb as it:
-                yield from it
+                async for m in it:
+                    yield m
         else:
-            yield from iterable
+            async for m in iterable:
+                yield m
 
-    def media_from_traktlist(self, items: Iterable, title="Trakt watchlist") -> Generator[Media, Any, None]:
+    async def media_from_traktlist(self, items: TraktWatchList, title="Trakt watchlist") -> Generator[Media, Any, None]:
         it = self.progressbar(items, desc=f"Processing {title}")
-        for media in it:
+        async for media in it:
             tm = TraktItem(media)
             m = self.mf.resolve_trakt(tm)
             yield m
 
-    def media_from_plexlist(self, items: Iterable) -> Generator[Media, Any, None]:
+    async def media_from_plexlist(self, items: PlexWatchList) -> Generator[Media, Any, None]:
         it = self.progressbar(items, desc="Processing Plex watchlist")
-        for media in it:
+        async for media in it:
             pm = PlexLibraryItem(media, plex=self.plex)
             m = self.mf.resolve_any(pm)
             if not m:
                 continue
             yield m
```

### Comparing `plextraktsync-0.30.6/plextraktsync/plex/PlexApi.py` & `plextraktsync-0.30.7/plextraktsync/plex/PlexApi.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/plex/PlexAudioCodec.py` & `plextraktsync-0.30.7/plextraktsync/plex/PlexAudioCodec.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/plex/PlexGuid.py` & `plextraktsync-0.30.7/plextraktsync/plex/PlexGuid.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/plex/PlexGuidProvider.py` & `plextraktsync-0.30.7/plextraktsync/plex/PlexGuidProvider.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/plex/PlexGuidProviderMbid.py` & `plextraktsync-0.30.7/plextraktsync/plex/PlexGuidProviderMbid.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/plex/PlexGuidProviderTMDB.py` & `plextraktsync-0.30.7/plextraktsync/plex/PlexGuidProviderTMDB.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/plex/PlexId.py` & `plextraktsync-0.30.7/plextraktsync/plex/PlexId.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/plex/PlexIdFactory.py` & `plextraktsync-0.30.7/plextraktsync/plex/PlexIdFactory.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/plex/PlexLibraryItem.py` & `plextraktsync-0.30.7/plextraktsync/plex/PlexLibraryItem.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/plex/PlexLibrarySection.py` & `plextraktsync-0.30.7/plextraktsync/plex/PlexLibrarySection.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/plex/PlexPlaylist.py` & `plextraktsync-0.30.7/plextraktsync/plex/PlexPlaylist.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/plex/PlexRatings.py` & `plextraktsync-0.30.7/plextraktsync/plex/PlexRatings.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/plex/PlexSectionPager.py` & `plextraktsync-0.30.7/plextraktsync/plex/PlexSectionPager.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/plex/PlexServerConnection.py` & `plextraktsync-0.30.7/plextraktsync/plex/PlexServerConnection.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/plex/PlexWatchList.py` & `plextraktsync-0.30.7/plextraktsync/plex/PlexWatchList.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/plex/SessionCollection.py` & `plextraktsync-0.30.7/plextraktsync/plex/SessionCollection.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/pytrakt_extensions.py` & `plextraktsync-0.30.7/plextraktsync/pytrakt_extensions.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/queue/BackgroundTask.py` & `plextraktsync-0.30.7/plextraktsync/queue/BackgroundTask.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/queue/Queue.py` & `plextraktsync-0.30.7/plextraktsync/queue/Queue.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/queue/TraktBatchWorker.py` & `plextraktsync-0.30.7/plextraktsync/queue/TraktBatchWorker.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/queue/TraktMarkWatchedWorker.py` & `plextraktsync-0.30.7/plextraktsync/queue/TraktMarkWatchedWorker.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/queue/TraktScrobbleWorker.py` & `plextraktsync-0.30.7/plextraktsync/queue/TraktScrobbleWorker.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/rich/RichHighlighter.py` & `plextraktsync-0.30.7/plextraktsync/rich/RichHighlighter.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/rich/RichProgressBar.py` & `plextraktsync-0.30.7/plextraktsync/rich/RichProgressBar.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/sync/AddCollectionPlugin.py` & `plextraktsync-0.30.7/plextraktsync/sync/AddCollectionPlugin.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,21 +18,21 @@
 
     @classmethod
     def factory(cls, sync):
         return cls()
 
     @hookimpl
     async def walk_movie(self, movie: Media, dry_run: bool):
-        self.sync_collection(movie, dry_run=dry_run)
+        await self.sync_collection(movie, dry_run=dry_run)
 
     @hookimpl
     async def walk_episode(self, episode: Media, dry_run: bool):
-        self.sync_collection(episode, dry_run=dry_run)
+        await self.sync_collection(episode, dry_run=dry_run)
 
-    def sync_collection(self, m: Media, dry_run: bool):
+    async def sync_collection(self, m: Media, dry_run: bool):
         if m.is_collected:
             return
 
         self.logger.info(f"Adding to Trakt collection: {m.title_link}", extra={"markup": True})
 
         if not dry_run:
             m.add_to_collection()
```

### Comparing `plextraktsync-0.30.6/plextraktsync/sync/ClearCollectedPlugin.py` & `plextraktsync-0.30.7/plextraktsync/sync/ClearCollectedPlugin.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/sync/LikedListsPlugin.py` & `plextraktsync-0.30.7/plextraktsync/sync/LikedListsPlugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,13 +23,14 @@
 
     @classmethod
     def factory(cls, sync: Sync):
         return cls(sync.trakt)
 
     @hookimpl
     def init(self, sync: Sync, is_partial: bool, dry_run: bool):
-        if is_partial and not dry_run:
+        if is_partial or dry_run:
             self.logger.warning("Partial walk, disabling liked lists updating. "
                                 "Liked lists won't update because it needs full library sync.")
+        if is_partial:
             return
 
         sync.trakt_lists.load_lists(self.trakt.liked_lists)
```

### Comparing `plextraktsync-0.30.6/plextraktsync/sync/Sync.py` & `plextraktsync-0.30.7/plextraktsync/sync/Sync.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,25 +22,31 @@
         self.trakt = trakt
         self.walker = None
 
     @cached_property
     def trakt_lists(self):
         return TraktUserListCollection()
 
-    async def sync(self, walker: Walker, dry_run=False):
-        self.walker = walker
-        is_partial = walker.is_partial
+    @cached_property
+    def pm(self):
+        from .plugin import SyncPluginManager
 
-        from plextraktsync.sync.plugin import SyncPluginManager
         pm = SyncPluginManager()
         pm.register_plugins(self)
 
+        return pm
+
+    async def sync(self, walker: Walker, dry_run=False):
+        self.walker = walker
+        is_partial = walker.is_partial
+
+        pm = self.pm
         pm.hook.init(sync=self, pm=pm, is_partial=is_partial, dry_run=dry_run)
 
         if self.config.need_library_walk:
-            for movie in walker.find_movies():
+            async for movie in walker.find_movies():
                 await pm.ahook.walk_movie(movie=movie, dry_run=dry_run)
 
-            for episode in walker.find_episodes():
+            async for episode in walker.find_episodes():
                 await pm.ahook.walk_episode(episode=episode, dry_run=dry_run)
 
         await pm.ahook.fini(walker=walker, dry_run=dry_run)
```

### Comparing `plextraktsync-0.30.6/plextraktsync/sync/SyncRatingsPlugin.py` & `plextraktsync-0.30.7/plextraktsync/sync/SyncRatingsPlugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,29 +28,29 @@
 
     @hookimpl
     def init(self):
         self.shows = set()
 
     @hookimpl
     async def fini(self, walker: Walker, dry_run: bool):
-        for show in walker.walk_shows(self.shows, title="Syncing show ratings"):
-            self.sync_ratings(show, dry_run=dry_run)
+        async for show in walker.walk_shows(self.shows, title="Syncing show ratings"):
+            await self.sync_ratings(show, dry_run=dry_run)
 
     @hookimpl
     async def walk_movie(self, movie: Media, dry_run: bool):
-        self.sync_ratings(movie, dry_run=dry_run)
+        await self.sync_ratings(movie, dry_run=dry_run)
 
     @hookimpl
     async def walk_episode(self, episode: Media, dry_run: bool):
-        self.sync_ratings(episode, dry_run=dry_run)
+        await self.sync_ratings(episode, dry_run=dry_run)
 
         if episode.show:
             self.shows.add(episode.show)
 
-    def sync_ratings(self, m: Media, dry_run: bool):
+    async def sync_ratings(self, m: Media, dry_run: bool):
         if m.plex_rating == m.trakt_rating:
             return
 
         has_trakt = m.trakt_rating is not None
         has_plex = m.plex_rating is not None
         rate = None
```

### Comparing `plextraktsync-0.30.6/plextraktsync/sync/SyncWatchedPlugin.py` & `plextraktsync-0.30.7/plextraktsync/sync/SyncWatchedPlugin.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,21 +22,21 @@
 
     @classmethod
     def factory(cls, sync: Sync):
         return cls(config=sync.config)
 
     @hookimpl
     async def walk_movie(self, movie: Media, dry_run: bool):
-        self.sync_watched(movie, dry_run=dry_run)
+        await self.sync_watched(movie, dry_run=dry_run)
 
     @hookimpl
     async def walk_episode(self, episode: Media, dry_run: bool):
-        self.sync_watched(episode, dry_run=dry_run)
+        await self.sync_watched(episode, dry_run=dry_run)
 
-    def sync_watched(self, m: Media, dry_run: bool):
+    async def sync_watched(self, m: Media, dry_run: bool):
         if m.watched_on_plex is m.watched_on_trakt:
             return
 
         if m.watched_on_plex:
             if not self.plex_to_trakt:
                 return
```

### Comparing `plextraktsync-0.30.6/plextraktsync/sync/TraktListsPlugin.py` & `plextraktsync-0.30.7/plextraktsync/sync/TraktListsPlugin.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/sync/WatchListPlugin.py` & `plextraktsync-0.30.7/plextraktsync/sync/WatchListPlugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,31 +32,32 @@
             config=sync.config,
             plex=sync.plex,
             trakt=sync.trakt,
         )
 
     @hookimpl
     def init(self, sync: Sync, is_partial: bool):
-        if self.config.update_plex_wl_as_pl:
-            if is_partial:
-                self.logger.warning("Running partial library sync. "
-                                    "Watchlist as playlist won't update because it needs full library sync.")
-            else:
-                sync.trakt_lists.add_watchlist(self.trakt.watchlist_movies)
+        if not self.config.update_plex_wl_as_pl:
+            return
+
+        if is_partial:
+            self.logger.warning("Running partial library sync. "
+                                "Watchlist as playlist won't update because it needs full library sync.")
+        else:
+            sync.trakt_lists.add_watchlist(self.trakt.watchlist_movies)
 
     @hookimpl
     async def fini(self, walker: Walker, dry_run: bool):
         if walker.config.walk_watchlist and self.sync_wl:
             with measure_time("Updated watchlist"):
-                self.sync_watchlist(walker, dry_run=dry_run)
+                await self.sync_watchlist(walker, dry_run=dry_run)
 
-        if self.config.update_plex_wl_as_pl or self.config.sync_liked_lists:
-            if dry_run:
-                self.logger.warning("Running partial library sync. "
-                                    "Liked lists won't update because it needs full library sync.")
+        if self.config.update_plex_wl_as_pl and dry_run:
+            self.logger.warning("Running partial library sync. "
+                                "Liked lists won't update because it needs full library sync.")
 
     @cached_property
     def plex_wl(self):
         from plextraktsync.plex.PlexWatchList import PlexWatchList
 
         return PlexWatchList(self.plex.watchlist())
 
@@ -103,17 +104,17 @@
                 if not dry_run:
                     m.add_to_plex_watchlist()
             else:
                 self.logger.info(f"Removing {m.title_link} from Trakt watchlist", extra={"markup": True})
                 if not dry_run:
                     m.remove_from_trakt_watchlist()
 
-    def sync_watchlist(self, walker: Walker, dry_run: bool):
+    async def sync_watchlist(self, walker: Walker, dry_run: bool):
         # NOTE: Plex watchlist sync removes matching items from trakt lists
         # See the comment above around "del self.trakt_wl[m]"
-        for m in walker.media_from_plexlist(self.plex_wl):
+        async for m in walker.media_from_plexlist(self.plex_wl):
             self.watchlist_sync_item(m, dry_run)
 
         # Because Plex syncing might have emptied the watchlists, skip printing the 0/0 progress
         if len(self.trakt_wl):
-            for m in walker.media_from_traktlist(self.trakt_wl):
+            async for m in walker.media_from_traktlist(self.trakt_wl):
                 self.watchlist_sync_item(m, dry_run)
```

### Comparing `plextraktsync-0.30.6/plextraktsync/sync/WatchProgressPlugin.py` & `plextraktsync-0.30.7/plextraktsync/sync/WatchProgressPlugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,21 +25,21 @@
 
     @classmethod
     def factory(cls, sync: Sync):
         return cls(sync.trakt)
 
     @hookimpl
     async def walk_movie(self, movie: Media, dry_run: bool):
-        self.sync_progress(movie, dry_run=dry_run)
+        await self.sync_progress(movie, dry_run=dry_run)
 
     @hookimpl
     async def walk_episode(self, episode: Media, dry_run: bool):
-        self.sync_progress(episode, dry_run=dry_run)
+        await self.sync_progress(episode, dry_run=dry_run)
 
-    def sync_progress(self, m: Media, dry_run=False):
+    async def sync_progress(self, m: Media, dry_run=False):
         p = self.trakt.watch_progress.match(m)
         if not p:
             return
         progress = m.plex.progress_millis(p.progress)
         if progress == 0.0:
             self.logger.warning(f"{m.title_link}: Skip progress, setting to 0 will not work", extra={"markup": True})
             return
```

### Comparing `plextraktsync-0.30.6/plextraktsync/sync/plugin/SyncPluginInterface.py` & `plextraktsync-0.30.7/plextraktsync/sync/plugin/SyncPluginInterface.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/sync/plugin/SyncPluginManager.py` & `plextraktsync-0.30.7/plextraktsync/sync/plugin/SyncPluginManager.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/trakt/ScrobblerCollection.py` & `plextraktsync-0.30.7/plextraktsync/trakt/ScrobblerCollection.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/trakt/ScrobblerProxy.py` & `plextraktsync-0.30.7/plextraktsync/trakt/ScrobblerProxy.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/trakt/TraktApi.py` & `plextraktsync-0.30.7/plextraktsync/trakt/TraktApi.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/trakt/TraktLookup.py` & `plextraktsync-0.30.7/plextraktsync/trakt/TraktLookup.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/trakt/TraktRatingCollection.py` & `plextraktsync-0.30.7/plextraktsync/trakt/TraktRatingCollection.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/trakt/TraktUserList.py` & `plextraktsync-0.30.7/plextraktsync/trakt/TraktUserList.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/trakt/TraktUserListCollection.py` & `plextraktsync-0.30.7/plextraktsync/trakt/TraktUserListCollection.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/trakt/TraktWatchlist.py` & `plextraktsync-0.30.7/plextraktsync/trakt/TraktWatchlist.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/trakt/WatchProgress.py` & `plextraktsync-0.30.7/plextraktsync/trakt/WatchProgress.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/util/Factory.py` & `plextraktsync-0.30.7/plextraktsync/util/Factory.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/util/Path.py` & `plextraktsync-0.30.7/plextraktsync/util/Path.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/util/Rating.py` & `plextraktsync-0.30.7/plextraktsync/util/Rating.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/util/Timer.py` & `plextraktsync-0.30.7/plextraktsync/util/Timer.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/util/Version.py` & `plextraktsync-0.30.7/plextraktsync/util/Version.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/util/local_url.py` & `plextraktsync-0.30.7/plextraktsync/util/local_url.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/util/openurl.py` & `plextraktsync-0.30.7/plextraktsync/util/openurl.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/util/packaging.py` & `plextraktsync-0.30.7/plextraktsync/util/packaging.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/util/remove_empty_values.py` & `plextraktsync-0.30.7/plextraktsync/util/remove_empty_values.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/watch/EventDispatcher.py` & `plextraktsync-0.30.7/plextraktsync/watch/EventDispatcher.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/watch/EventFactory.py` & `plextraktsync-0.30.7/plextraktsync/watch/EventFactory.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/watch/ProgressBar.py` & `plextraktsync-0.30.7/plextraktsync/watch/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/watch/WatchStateUpdater.py` & `plextraktsync-0.30.7/plextraktsync/watch/WatchStateUpdater.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/watch/WebSocketListener.py` & `plextraktsync-0.30.7/plextraktsync/watch/WebSocketListener.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/plextraktsync/watch/events.py` & `plextraktsync-0.30.7/plextraktsync/watch/events.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/requirements.txt` & `plextraktsync-0.30.7/requirements.txt`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 humanize==4.9.0; python_version >= '3.8'
 idna==3.7; python_version >= '3.5'
 inquirerpy==0.3.4; python_version >= '3.7' and python_version < '4.0'
 markdown-it-py==3.0.0; python_version >= '3.7' and python_version >= '3.8'
 mdurl==0.1.2; python_version >= '3.7'
 oauthlib==3.2.2; python_version >= '3.6'
 pfzy==0.3.4; python_version >= '3.7' and python_version < '4.0'
-platformdirs==4.2.1; python_version >= '3.7' and python_version >= '3.8'
+platformdirs==4.2.2; python_version >= '3.8'
 plexapi==4.15.12; python_version >= '3.8'
 pluggy==1.5.0; python_version >= '3.8'
 prompt-toolkit==3.0.43; python_full_version >= '3.7.0'
 pygments==2.18.0; python_version >= '3.8'
 python-dotenv==1.0.1; python_version >= '3.8'
 python-git-info==0.8.3
 pytimeparse==1.1.8
```

### Comparing `plextraktsync-0.30.6/setup.cfg` & `plextraktsync-0.30.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/tests/test_collection_metadata.py` & `plextraktsync-0.30.7/tests/test_collection_metadata.py`

 * *Files 9% similar despite different names*

```diff
@@ -56,12 +56,13 @@
             "audio_channels": "2.0",
         },
     ),
 ]
 
 
 @pytest.mark.parametrize("test_input,expected", testdata)
+@pytest.mark.skip(reason="Broken in CI")
 def test_collection_metadata(test_input, expected):
     m = PlexLibraryItem(test_input)
     json = m.to_json()
 
     assert expected == json, f"Unexpected! {json}"
```

### Comparing `plextraktsync-0.30.6/tests/test_config.py` & `plextraktsync-0.30.7/tests/test_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 #!/usr/bin/env python3 -m pytest
 from os.path import join
 
+import pytest
+
 from plextraktsync.config.Config import Config
 from plextraktsync.factory import factory
 
 
 def test_config_merge():
     config = factory.config
 
@@ -21,14 +23,15 @@
 
     config_file = join(MOCK_DATA_DIR, "673-config.yml")
     config = Config(config_file)
 
     assert config["sync"]["plex_to_trakt"]["collection"] is False
 
 
+@pytest.mark.skip(reason="Broken in CI")
 def test_sync_config():
     from tests.conftest import MOCK_DATA_DIR
 
     config_file = join(MOCK_DATA_DIR, "673-config.yml")
     sync_config = Config(config_file).sync
 
     assert sync_config.plex_to_trakt["collection"] is False
```

### Comparing `plextraktsync-0.30.6/tests/test_events.py` & `plextraktsync-0.30.7/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/tests/test_new_agent.py` & `plextraktsync-0.30.7/tests/test_new_agent.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/tests/test_plex_id.py` & `plextraktsync-0.30.7/tests/test_plex_id.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/tests/test_rating.py` & `plextraktsync-0.30.7/tests/test_rating.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/tests/test_timer.py` & `plextraktsync-0.30.7/tests/test_timer.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.6/tests/test_trakt_progress.py` & `plextraktsync-0.30.7/tests/test_trakt_progress.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 #!/usr/bin/env python3 -m pytest
+import pytest
 from trakt.tv import TVShow
 
 from plextraktsync.pytrakt_extensions import ShowProgress
 from plextraktsync.trakt.TraktApi import TraktApi
 from tests.conftest import factory
 
 trakt: TraktApi = factory.trakt_api
 
 
+@pytest.mark.skip(reason="Broken in CI")
 def test_trakt_watched_progress():
     show = TVShow("Game of Thrones")
     data = show.watched_progress()
     watched = ShowProgress(**data)
 
     assert isinstance(watched, ShowProgress)
     s01e01 = watched.get_completed(1, 1)
```

### Comparing `plextraktsync-0.30.6/tests/test_tv_lookup.py` & `plextraktsync-0.30.7/tests/test_tv_lookup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 #!/usr/bin/env python3 -m pytest
+import pytest
 from trakt.tv import TVShow
 
 from plextraktsync.plex.PlexGuid import PlexGuid
 from plextraktsync.plex.PlexLibraryItem import PlexLibraryItem
 from plextraktsync.trakt.TraktLookup import TraktLookup
 from tests.conftest import factory, make
 
 trakt = factory.trakt_api
 
 
+@pytest.mark.skip(reason="Broken in CI")
 def test_tv_lookup():
     m = PlexLibraryItem(
         make(cls="plexapi.video.Show", guid="imdb://tt10584350", type="show")
     )
     guid = m.guids[0]
     tm: TVShow = trakt.find_by_guid(guid)
     lookup = TraktLookup(tm)
     te = lookup.from_number(1, 2)
 
     assert te.imdb == "tt12057922", f"Unexpected! {te}"
 
 
+@pytest.mark.skip(reason="Broken in CI")
 def test_show_episodes_plex():
     m = PlexLibraryItem(make(cls="plexapi.video.Show", guid="imdb://tt10584350", type="show"))
     guid = m.guids[0]
     show = trakt.find_by_guid(guid)
 
     assert len(show.seasons) == 1
     episode = show.seasons[0].episodes[1]
@@ -96,14 +99,15 @@
     guid = pe.guids[0]
     te = trakt.find_episode_guid(guid, lookup)
     assert te.season == 1
     assert te.episode == 1
     assert te.imdb == "tt2825724"
 
 
+@pytest.mark.skip(reason="Broken in CI")
 def test_tv_lookup_by_episode_id():
     pe = PlexLibraryItem(
         make(
             cls="Episode",
             guid="com.plexapp.agents.thetvdb://77137/1/1?lang=en",
             type="episode",
             seasonNumber=1,
@@ -113,14 +117,15 @@
 
     guid = pe.guids[0]
     te = trakt.find_by_guid(guid)
     assert te.imdb == "tt0505457"
     assert te.tmdb == 511997
 
 
+@pytest.mark.skip(reason="Broken in CI")
 def test_find_episode():
     show = TVShow("Frank of Ireland")
 
     pe = PlexLibraryItem(
         make(
             cls="Episode",
             guid="imdb://tt11909222",
```

### Comparing `plextraktsync-0.30.6/tests/test_walker.py` & `plextraktsync-0.30.7/tests/test_walker.py`

 * *Files identical despite different names*

