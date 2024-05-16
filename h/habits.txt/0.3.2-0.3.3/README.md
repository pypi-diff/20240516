# Comparing `tmp/habits_txt-0.3.2.tar.gz` & `tmp/habits_txt-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "habits_txt-0.3.2.tar", max compression
+gzip compressed data, was "habits_txt-0.3.3.tar", max compression
```

## Comparing `habits_txt-0.3.2.tar` & `habits_txt-0.3.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     3109 2024-05-14 20:37:42.341037 habits_txt-0.3.2/README.md
--rwxr-xr-x   0        0        0      788 2024-05-15 17:43:14.132064 habits_txt-0.3.2/bin/hbtxt.py
--rw-r--r--   0        0        0        0 2024-05-14 20:25:35.415585 habits_txt-0.3.2/habits_txt/__init__.py
--rw-r--r--   0        0        0    13971 2024-05-15 17:43:14.132064 habits_txt-0.3.2/habits_txt/builder.py
--rw-r--r--   0        0        0     7842 2024-05-15 17:57:35.675452 habits_txt-0.3.2/habits_txt/cli.py
--rw-r--r--   0        0        0     2154 2024-05-14 20:25:35.415585 habits_txt-0.3.2/habits_txt/config.py
--rw-r--r--   0        0        0      224 2024-05-14 20:25:35.415585 habits_txt-0.3.2/habits_txt/defaults.py
--rw-r--r--   0        0        0     2323 2024-05-15 17:43:14.132064 habits_txt-0.3.2/habits_txt/directives.py
--rw-r--r--   0        0        0      380 2024-05-14 20:25:35.415585 habits_txt-0.3.2/habits_txt/exceptions.py
--rw-r--r--   0        0        0     8107 2024-05-15 17:57:35.675452 habits_txt-0.3.2/habits_txt/journal.py
--rw-r--r--   0        0        0     2940 2024-05-15 17:43:14.132064 habits_txt-0.3.2/habits_txt/models.py
--rw-r--r--   0        0        0     9037 2024-05-15 17:43:14.132064 habits_txt-0.3.2/habits_txt/parser.py
--rw-r--r--   0        0        0      952 2024-05-14 20:25:35.415585 habits_txt-0.3.2/habits_txt/records_query.py
--rw-r--r--   0        0        0      627 2024-05-15 17:57:35.675452 habits_txt-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     3482 1970-01-01 00:00:00.000000 habits_txt-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     3109 2024-05-14 20:37:42.341037 habits_txt-0.3.3/README.md
+-rwxr-xr-x   0        0        0      788 2024-05-15 17:43:14.132064 habits_txt-0.3.3/bin/hbtxt.py
+-rw-r--r--   0        0        0        0 2024-05-14 20:25:35.415585 habits_txt-0.3.3/habits_txt/__init__.py
+-rw-r--r--   0        0        0    13971 2024-05-15 17:43:14.132064 habits_txt-0.3.3/habits_txt/builder.py
+-rw-r--r--   0        0        0     7849 2024-05-15 18:03:05.969504 habits_txt-0.3.3/habits_txt/cli.py
+-rw-r--r--   0        0        0     2154 2024-05-14 20:25:35.415585 habits_txt-0.3.3/habits_txt/config.py
+-rw-r--r--   0        0        0      224 2024-05-14 20:25:35.415585 habits_txt-0.3.3/habits_txt/defaults.py
+-rw-r--r--   0        0        0     2323 2024-05-15 17:43:14.132064 habits_txt-0.3.3/habits_txt/directives.py
+-rw-r--r--   0        0        0      380 2024-05-14 20:25:35.415585 habits_txt-0.3.3/habits_txt/exceptions.py
+-rw-r--r--   0        0        0     8107 2024-05-15 18:01:28.344968 habits_txt-0.3.3/habits_txt/journal.py
+-rw-r--r--   0        0        0     2940 2024-05-15 17:43:14.132064 habits_txt-0.3.3/habits_txt/models.py
+-rw-r--r--   0        0        0     9037 2024-05-15 17:43:14.132064 habits_txt-0.3.3/habits_txt/parser.py
+-rw-r--r--   0        0        0      952 2024-05-14 20:25:35.415585 habits_txt-0.3.3/habits_txt/records_query.py
+-rw-r--r--   0        0        0      627 2024-05-15 18:03:05.969504 habits_txt-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     3482 1970-01-01 00:00:00.000000 habits_txt-0.3.3/PKG-INFO
```

### Comparing `habits_txt-0.3.2/README.md` & `habits_txt-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `habits_txt-0.3.2/bin/hbtxt.py` & `habits_txt-0.3.3/bin/hbtxt.py`

 * *Files identical despite different names*

### Comparing `habits_txt-0.3.2/habits_txt/builder.py` & `habits_txt-0.3.3/habits_txt/builder.py`

 * *Files identical despite different names*

### Comparing `habits_txt-0.3.2/habits_txt/cli.py` & `habits_txt-0.3.3/habits_txt/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,15 +210,15 @@
 
 def _style_record(record: models_.HabitRecord) -> str:
     return " ".join(
         [
             click.style(
                 dt.datetime.strftime(record.date, defaults.DATE_FMT), fg="blue"
             ),
-            click.style(record.habit_name, fg="green"),
+            f'"{click.style(record.habit_name, fg="green")}"',
             click.style(record._str_value(), fg="yellow"),
         ]
     )
 
 
 def _style_completion_info(habit_completion_info: models_.HabitCompletionInfo) -> str:
     def process_average(x):
```

### Comparing `habits_txt-0.3.2/habits_txt/config.py` & `habits_txt-0.3.3/habits_txt/config.py`

 * *Files identical despite different names*

### Comparing `habits_txt-0.3.2/habits_txt/directives.py` & `habits_txt-0.3.3/habits_txt/directives.py`

 * *Files identical despite different names*

### Comparing `habits_txt-0.3.2/habits_txt/journal.py` & `habits_txt-0.3.3/habits_txt/journal.py`

 * *Files identical despite different names*

### Comparing `habits_txt-0.3.2/habits_txt/models.py` & `habits_txt-0.3.3/habits_txt/models.py`

 * *Files identical despite different names*

### Comparing `habits_txt-0.3.2/habits_txt/parser.py` & `habits_txt-0.3.3/habits_txt/parser.py`

 * *Files identical despite different names*

### Comparing `habits_txt-0.3.2/habits_txt/records_query.py` & `habits_txt-0.3.3/habits_txt/records_query.py`

 * *Files identical despite different names*

### Comparing `habits_txt-0.3.2/pyproject.toml` & `habits_txt-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "habits.txt"
-version = "0.3.2"
+version = "0.3.3"
 description = ""
 authors = ["estebanthi <esteban.thilliez@gmail.com>"]
 readme = "README.md"
 packages = [
     {include = "habits_txt"}, {include = "bin"}
 ]
```

### Comparing `habits_txt-0.3.2/PKG-INFO` & `habits_txt-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: habits.txt
-Version: 0.3.2
+Version: 0.3.3
 Summary: 
 Author: estebanthi
 Author-email: esteban.thilliez@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
```

