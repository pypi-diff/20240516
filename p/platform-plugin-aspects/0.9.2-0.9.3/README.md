# Comparing `tmp/platform_plugin_aspects-0.9.2.tar.gz` & `tmp/platform_plugin_aspects-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "platform_plugin_aspects-0.9.2.tar", last modified: Thu May  9 11:45:59 2024, max compression
+gzip compressed data, was "platform_plugin_aspects-0.9.3.tar", last modified: Thu May 16 19:47:21 2024, max compression
```

## Comparing `platform_plugin_aspects-0.9.2.tar` & `platform_plugin_aspects-0.9.3.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:45:59.011207 platform_plugin_aspects-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-09 11:45:52.000000 platform_plugin_aspects-0.9.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-09 11:45:52.000000 platform_plugin_aspects-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-09 11:45:52.000000 platform_plugin_aspects-0.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12106 2024-05-09 11:45:59.011207 platform_plugin_aspects-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8698 2024-05-09 11:45:52.000000 platform_plugin_aspects-0.9.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:45:59.003207 platform_plugin_aspects-0.9.2/platform_plugin_aspects/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-09 11:45:52.000000 platform_plugin_aspects-0.9.2/platform_plugin_aspects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-09 11:45:52.000000 platform_plugin_aspects-0.9.2/platform_plugin_aspects/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:45:59.003207 platform_plugin_aspects-0.9.2/platform_plugin_aspects/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 11:45:52.000000 platform_plugin_aspects-0.9.2/platform_plugin_aspects/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-09 11:45:52.000000 platform_plugin_aspects-0.9.2/platform_plugin_aspects/extensions/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:45:59.003207 platform_plugin_aspects-0.9.2/platform_plugin_aspects/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 11:45:52.000000 platform_plugin_aspects-0.9.2/platform_plugin_aspects/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:45:59.007207 platform_plugin_aspects-0.9.2/platform_plugin_aspects/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 11:45:52.000000 platform_plugin_aspects-0.9.2/platform_plugin_aspects/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-05-09 11:45:52.000000 platform_plugin_aspects-0.9.2/platform_plugin_aspects/management/commands/dump_data_to_clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (127)    10177 2024-05-09 11:45:52.000000 platform_plugin_aspects-0.9.2/platform_plugin_aspects/management/commands/load_test_tracking_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    14268 2024-05-09 11:45:52.000000 platform_plugin_aspects-0.9.2/platform_plugin_aspects/management/commands/monitor_load_test_tracking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:45:59.007207 platform_plugin_aspects-0.9.2/platform_plugin_aspects/settings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 11:45:52.000000 platform_plugin_aspects-0.9.2/platform_plugin_aspects/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-09 11:45:52.000000 platform_plugin_aspects-0.9.2/platform_plugin_aspects/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-09 11:45:52.000000 platform_plugin_aspects-0.9.2/platform_plugin_aspects/settings/production.py
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-05-09 11:45:52.000000 platform_plugin_aspects-0.9.2/platform_plugin_aspects/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:45:59.007207 platform_plugin_aspects-0.9.2/platform_plugin_aspects/sinks/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-09 11:45:52.000000 platform_plugin_aspects-0.9.2/platform_plugin_aspects/sinks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12821 2024-05-09 11:45:52.000000 platform_plugin_aspects-0.9.2/platform_plugin_aspects/sinks/base_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-05-09 11:45:52.000000 platform_plugin_aspects-0.9.2/platform_plugin_aspects/sinks/course_overview_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-09 11:45:52.000000 platform_plugin_aspects-0.9.2/platform_plugin_aspects/sinks/external_id_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-09 11:45:52.000000 platform_plugin_aspects-0.9.2/platform_plugin_aspects/sinks/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-09 11:45:52.000000 platform_plugin_aspects-0.9.2/platform_plugin_aspects/sinks/user_profile_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-09 11:45:52.000000 platform_plugin_aspects-0.9.2/platform_plugin_aspects/sinks/user_retire_sink.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:45:58.999207 platform_plugin_aspects-0.9.2/platform_plugin_aspects/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:45:59.007207 platform_plugin_aspects-0.9.2/platform_plugin_aspects/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-09 11:45:52.000000 platform_plugin_aspects-0.9.2/platform_plugin_aspects/static/css/superset.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:45:59.007207 platform_plugin_aspects-0.9.2/platform_plugin_aspects/static/html/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-09 11:45:52.000000 platform_plugin_aspects-0.9.2/platform_plugin_aspects/static/html/superset.html
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-09 11:45:52.000000 platform_plugin_aspects-0.9.2/platform_plugin_aspects/static/html/superset_student.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:45:59.007207 platform_plugin_aspects-0.9.2/platform_plugin_aspects/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-09 11:45:52.000000 platform_plugin_aspects-0.9.2/platform_plugin_aspects/static/js/embed_dashboard.js
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-09 11:45:52.000000 platform_plugin_aspects-0.9.2/platform_plugin_aspects/static/js/install_required.js
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-09 11:45:52.000000 platform_plugin_aspects-0.9.2/platform_plugin_aspects/static/js/superset.js
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-09 11:45:52.000000 platform_plugin_aspects-0.9.2/platform_plugin_aspects/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:45:58.999207 platform_plugin_aspects-0.9.2/platform_plugin_aspects/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:45:59.007207 platform_plugin_aspects-0.9.2/platform_plugin_aspects/templates/instructor_dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-09 11:45:52.000000 platform_plugin_aspects-0.9.2/platform_plugin_aspects/templates/instructor_dashboard/aspects.html
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-09 11:45:52.000000 platform_plugin_aspects-0.9.2/platform_plugin_aspects/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-05-09 11:45:52.000000 platform_plugin_aspects-0.9.2/platform_plugin_aspects/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-09 11:45:52.000000 platform_plugin_aspects-0.9.2/platform_plugin_aspects/views.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-09 11:45:52.000000 platform_plugin_aspects-0.9.2/platform_plugin_aspects/waffle.py
--rw-r--r--   0 runner    (1001) docker     (127)     7152 2024-05-09 11:45:52.000000 platform_plugin_aspects-0.9.2/platform_plugin_aspects/xblock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:45:59.007207 platform_plugin_aspects-0.9.2/platform_plugin_aspects.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12106 2024-05-09 11:45:58.000000 platform_plugin_aspects-0.9.2/platform_plugin_aspects.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-05-09 11:45:58.000000 platform_plugin_aspects-0.9.2/platform_plugin_aspects.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 11:45:58.000000 platform_plugin_aspects-0.9.2/platform_plugin_aspects.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-09 11:45:58.000000 platform_plugin_aspects-0.9.2/platform_plugin_aspects.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 11:45:58.000000 platform_plugin_aspects-0.9.2/platform_plugin_aspects.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-09 11:45:58.000000 platform_plugin_aspects-0.9.2/platform_plugin_aspects.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-09 11:45:58.000000 platform_plugin_aspects-0.9.2/platform_plugin_aspects.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:45:59.007207 platform_plugin_aspects-0.9.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-09 11:45:52.000000 platform_plugin_aspects-0.9.2/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-09 11:45:52.000000 platform_plugin_aspects-0.9.2/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-09 11:45:59.011207 platform_plugin_aspects-0.9.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     6997 2024-05-09 11:45:52.000000 platform_plugin_aspects-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:47:21.935549 platform_plugin_aspects-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12229 2024-05-16 19:47:21.935549 platform_plugin_aspects-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8698 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:47:21.931549 platform_plugin_aspects-0.9.3/platform_plugin_aspects/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:47:21.935549 platform_plugin_aspects-0.9.3/platform_plugin_aspects/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/extensions/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:47:21.935549 platform_plugin_aspects-0.9.3/platform_plugin_aspects/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:47:21.935549 platform_plugin_aspects-0.9.3/platform_plugin_aspects/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/management/commands/dump_data_to_clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10177 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/management/commands/load_test_tracking_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14268 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/management/commands/monitor_load_test_tracking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:47:21.935549 platform_plugin_aspects-0.9.3/platform_plugin_aspects/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/settings/production.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:47:21.935549 platform_plugin_aspects-0.9.3/platform_plugin_aspects/sinks/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/sinks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12821 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/sinks/base_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/sinks/course_overview_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/sinks/external_id_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/sinks/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/sinks/user_profile_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/sinks/user_retire_sink.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:47:21.931549 platform_plugin_aspects-0.9.3/platform_plugin_aspects/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:47:21.935549 platform_plugin_aspects-0.9.3/platform_plugin_aspects/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/static/css/superset.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:47:21.935549 platform_plugin_aspects-0.9.3/platform_plugin_aspects/static/html/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/static/html/superset.html
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/static/html/superset_student.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:47:21.935549 platform_plugin_aspects-0.9.3/platform_plugin_aspects/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/static/js/embed_dashboard.js
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/static/js/install_required.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/static/js/superset.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:47:21.931549 platform_plugin_aspects-0.9.3/platform_plugin_aspects/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:47:21.935549 platform_plugin_aspects-0.9.3/platform_plugin_aspects/templates/instructor_dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/templates/instructor_dashboard/aspects.html
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/waffle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7152 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/xblock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:47:21.935549 platform_plugin_aspects-0.9.3/platform_plugin_aspects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12229 2024-05-16 19:47:21.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-05-16 19:47:21.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 19:47:21.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-16 19:47:21.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 19:47:21.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-16 19:47:21.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-16 19:47:21.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:47:21.935549 platform_plugin_aspects-0.9.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-16 19:47:21.939549 platform_plugin_aspects-0.9.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6997 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/setup.py
```

### Comparing `platform_plugin_aspects-0.9.2/CHANGELOG.rst` & `platform_plugin_aspects-0.9.3/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,23 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
+0.9.3 - 2024-05-15
+******************
+
+Fixes
+=====
+
+* Change wording of the "go to Superset" link, and make it optional.
+
+
 0.9.2 - 2024-05-08
 ******************
 
 Fixes
 =====
 
 * Remove caching of Superset guest token to fix various display errors and token refresh edge cases.
```

### Comparing `platform_plugin_aspects-0.9.2/LICENSE` & `platform_plugin_aspects-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.2/PKG-INFO` & `platform_plugin_aspects-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platform-plugin-aspects
-Version: 0.9.2
+Version: 0.9.3
 Summary: Aspects plugins for edx-platform
 Home-page: https://github.com/openedx/platform-plugin-aspects
 Author: Open edX Project
 Author-email: oscm@openedx.org
 License: Apache 2.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -272,14 +272,23 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
+0.9.3 - 2024-05-15
+******************
+
+Fixes
+=====
+
+* Change wording of the "go to Superset" link, and make it optional.
+
+
 0.9.2 - 2024-05-08
 ******************
 
 Fixes
 =====
 
 * Remove caching of Superset guest token to fix various display errors and token refresh edge cases.
```

### Comparing `platform_plugin_aspects-0.9.2/README.rst` & `platform_plugin_aspects-0.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.2/platform_plugin_aspects/apps.py` & `platform_plugin_aspects-0.9.3/platform_plugin_aspects/apps.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.2/platform_plugin_aspects/extensions/filters.py` & `platform_plugin_aspects-0.9.3/platform_plugin_aspects/extensions/filters.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,20 +26,26 @@
         """Execute filter that modifies the instructor dashboard context.
         Args:
             context (dict): the context for the instructor dashboard.
             _ (str): instructor dashboard template name.
         """
         course = context["course"]
         dashboards = settings.ASPECTS_INSTRUCTOR_DASHBOARDS
+        show_dashboard_link = settings.SUPERSET_SHOW_INSTRUCTOR_DASHBOARD_LINK
 
         user = get_current_user()
 
-        user_language = (
-            get_model("user_preference").get_value(user, "pref-lang") or "en"
-        )
+        try:
+            user_language = (
+                get_model("user_preference").get_value(user, "pref-lang") or "en"
+            )
+        # If there is no user_preferences model defined this will get thrown
+        except AttributeError:
+            user_language = "en"
+
         formatted_language = user_language.lower().replace("-", "_")
         if formatted_language not in [
             loc.lower().replace("-", "_") for loc in settings.SUPERSET_DASHBOARD_LOCALES
         ]:
             formatted_language = "en"
 
         context["course_id"] = course.id
@@ -58,15 +64,18 @@
             "fragment": frag,
             "section_key": BLOCK_CATEGORY,
             "section_display_name": _("Reports"),
             "course_id": str(context.get("course_id")),
             "superset_guest_token_url": str(context.get("superset_guest_token_url")),
             "superset_url": str(context.get("superset_url")),
             "template_path_prefix": TEMPLATE_ABSOLUTE_PATH,
+            "show_dashboard_link": show_dashboard_link,
         }
+
+        print(section_data)
         context["sections"].append(section_data)
         return {
             "context": context,
         }
 
     def resource_string(self, path):
         """Handy helper for getting resources from our kit."""
```

### Comparing `platform_plugin_aspects-0.9.2/platform_plugin_aspects/management/commands/dump_data_to_clickhouse.py` & `platform_plugin_aspects-0.9.3/platform_plugin_aspects/management/commands/dump_data_to_clickhouse.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.2/platform_plugin_aspects/management/commands/load_test_tracking_events.py` & `platform_plugin_aspects-0.9.3/platform_plugin_aspects/management/commands/load_test_tracking_events.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.2/platform_plugin_aspects/management/commands/monitor_load_test_tracking.py` & `platform_plugin_aspects-0.9.3/platform_plugin_aspects/management/commands/monitor_load_test_tracking.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.2/platform_plugin_aspects/settings/common.py` & `platform_plugin_aspects-0.9.3/platform_plugin_aspects/settings/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,14 +42,15 @@
         {
             "name": _("At-Risk Learners Dashboard"),
             "slug": "learner-groups",
             "uuid": "8661d20c-cee6-4245-9fcc-610daea5fd24",
             "allow_translations": True,
         },
     ]
+    settings.SUPERSET_SHOW_INSTRUCTOR_DASHBOARD_LINK = True
     settings.SUPERSET_EXTRA_FILTERS_FORMAT = []
     settings.SUPERSET_DASHBOARD_LOCALES = ["en"]
     settings.EVENT_SINK_CLICKHOUSE_BACKEND_CONFIG = {
         # URL to a running ClickHouse server's HTTP interface. ex: https://foo.openedx.org:8443/ or
         # http://foo.openedx.org:8123/ . Note that we only support the ClickHouse HTTP interface
         # to avoid pulling in more dependencies to the platform than necessary.
         "url": "http://clickhouse:8123",
```

### Comparing `platform_plugin_aspects-0.9.2/platform_plugin_aspects/settings/production.py` & `platform_plugin_aspects-0.9.3/platform_plugin_aspects/settings/production.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.2/platform_plugin_aspects/signals.py` & `platform_plugin_aspects-0.9.3/platform_plugin_aspects/signals.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.2/platform_plugin_aspects/sinks/base_sink.py` & `platform_plugin_aspects-0.9.3/platform_plugin_aspects/sinks/base_sink.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.2/platform_plugin_aspects/sinks/course_overview_sink.py` & `platform_plugin_aspects-0.9.3/platform_plugin_aspects/sinks/course_overview_sink.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.2/platform_plugin_aspects/sinks/external_id_sink.py` & `platform_plugin_aspects-0.9.3/platform_plugin_aspects/sinks/external_id_sink.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.2/platform_plugin_aspects/sinks/serializers.py` & `platform_plugin_aspects-0.9.3/platform_plugin_aspects/sinks/serializers.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.2/platform_plugin_aspects/sinks/user_profile_sink.py` & `platform_plugin_aspects-0.9.3/platform_plugin_aspects/sinks/user_profile_sink.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.2/platform_plugin_aspects/sinks/user_retire_sink.py` & `platform_plugin_aspects-0.9.3/platform_plugin_aspects/sinks/user_retire_sink.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.2/platform_plugin_aspects/static/css/superset.css` & `platform_plugin_aspects-0.9.3/platform_plugin_aspects/static/css/superset.css`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.2/platform_plugin_aspects/static/html/superset.html` & `platform_plugin_aspects-0.9.3/platform_plugin_aspects/static/html/superset.html`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.2/platform_plugin_aspects/static/js/embed_dashboard.js` & `platform_plugin_aspects-0.9.3/platform_plugin_aspects/static/js/embed_dashboard.js`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.2/platform_plugin_aspects/static/js/superset.js` & `platform_plugin_aspects-0.9.3/platform_plugin_aspects/static/js/superset.js`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.2/platform_plugin_aspects/tasks.py` & `platform_plugin_aspects-0.9.3/platform_plugin_aspects/tasks.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.2/platform_plugin_aspects/templates/instructor_dashboard/aspects.html` & `platform_plugin_aspects-0.9.3/platform_plugin_aspects/templates/instructor_dashboard/aspects.html`

 * *Files 16% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 from django.utils.translation import gettext as _
 from openedx.core.djangolib.markup import HTML
 %>
 
 <%include file="/courseware/xqa_interface.html/"/>
 <%
 superset_url = section_data.get("superset_url")
+show_superset_link = superset_url and section_data.get("show_dashboard_link")
 %>
 
 <section class="superset">
-    % if superset_url:
+    % if show_superset_link:
     <div class="superset-link">
-      <a href="${superset_url}login/openedxsso">${_("Go to Superset to create new or further customize the reports below.")}</a>
+      <a href="${superset_url}login/openedxsso">${_("View dashboards in Superset")}</a>
     </div>
     % endif
     ${HTML(section_data['fragment'].body_html())}
 </section>
```

#### html2text {}

```diff
@@ -1,6 +1,8 @@
 ## mako <%page args="section_data" expression_filter="h"/> <%! from
 django.utils.translation import gettext as _ from openedx.core.djangolib.markup
 import HTML %> <%include file="/courseware/xqa_interface.html/"/> <%
-superset_url = section_data.get("superset_url") %> % if superset_url:
-_$_{___(_"_G_o_ _t_o_ _S_u_p_e_r_s_e_t_ _t_o_ _c_r_e_a_t_e_ _n_e_w_ _o_r_ _f_u_r_t_h_e_r_ _c_u_s_t_o_m_i_z_e_ _t_h_e_ _r_e_p_o_r_t_s_ _b_e_l_o_w_._"_)_}
+superset_url = section_data.get("superset_url") show_superset_link =
+superset_url and section_data.get("show_dashboard_link") %> % if
+show_superset_link:
+_$_{___(_"_V_i_e_w_ _d_a_s_h_b_o_a_r_d_s_ _i_n_ _S_u_p_e_r_s_e_t_"_)_}
 % endif ${HTML(section_data['fragment'].body_html())}
```

### Comparing `platform_plugin_aspects-0.9.2/platform_plugin_aspects/urls.py` & `platform_plugin_aspects-0.9.3/platform_plugin_aspects/urls.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.2/platform_plugin_aspects/utils.py` & `platform_plugin_aspects-0.9.3/platform_plugin_aspects/utils.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.2/platform_plugin_aspects/views.py` & `platform_plugin_aspects-0.9.3/platform_plugin_aspects/views.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.2/platform_plugin_aspects/xblock.py` & `platform_plugin_aspects-0.9.3/platform_plugin_aspects/xblock.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.2/platform_plugin_aspects.egg-info/PKG-INFO` & `platform_plugin_aspects-0.9.3/platform_plugin_aspects.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platform-plugin-aspects
-Version: 0.9.2
+Version: 0.9.3
 Summary: Aspects plugins for edx-platform
 Home-page: https://github.com/openedx/platform-plugin-aspects
 Author: Open edX Project
 Author-email: oscm@openedx.org
 License: Apache 2.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -272,14 +272,23 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
+0.9.3 - 2024-05-15
+******************
+
+Fixes
+=====
+
+* Change wording of the "go to Superset" link, and make it optional.
+
+
 0.9.2 - 2024-05-08
 ******************
 
 Fixes
 =====
 
 * Remove caching of Superset guest token to fix various display errors and token refresh edge cases.
```

### Comparing `platform_plugin_aspects-0.9.2/platform_plugin_aspects.egg-info/SOURCES.txt` & `platform_plugin_aspects-0.9.3/platform_plugin_aspects.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.2/requirements/constraints.txt` & `platform_plugin_aspects-0.9.3/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.2/setup.py` & `platform_plugin_aspects-0.9.3/setup.py`

 * *Files identical despite different names*

