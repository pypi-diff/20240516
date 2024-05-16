# Comparing `tmp/pluralize-20240413.1.tar.gz` & `tmp/pluralize-20240515.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pluralize-20240413.1.tar", last modified: Sat Apr 13 17:39:06 2024, max compression
+gzip compressed data, was "pluralize-20240515.1.tar", last modified: Thu May 16 06:48:55 2024, max compression
```

## Comparing `pluralize-20240413.1.tar` & `pluralize-20240515.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-13 17:39:06.724103 pluralize-20240413.1/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2748 2024-04-13 17:39:06.724103 pluralize-20240413.1/PKG-INFO
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2195 2021-07-16 07:51:13.000000 pluralize-20240413.1/README.md
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-13 17:39:06.720769 pluralize-20240413.1/pluralize/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5555 2024-04-13 07:11:53.000000 pluralize-20240413.1/pluralize/__init__.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-13 17:39:06.724103 pluralize-20240413.1/pluralize.egg-info/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2748 2024-04-13 17:39:06.000000 pluralize-20240413.1/pluralize.egg-info/PKG-INFO
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      199 2024-04-13 17:39:06.000000 pluralize-20240413.1/pluralize.egg-info/SOURCES.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2024-04-13 17:39:06.000000 pluralize-20240413.1/pluralize.egg-info/dependency_links.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       10 2024-04-13 17:39:06.000000 pluralize-20240413.1/pluralize.egg-info/top_level.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      563 2024-04-13 07:10:28.000000 pluralize-20240413.1/pyproject.toml
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       38 2024-04-13 17:39:06.724103 pluralize-20240413.1/setup.cfg
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-13 17:39:06.720769 pluralize-20240413.1/tests/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1355 2021-07-16 07:50:13.000000 pluralize-20240413.1/tests/test_simple.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-16 06:48:55.580986 pluralize-20240515.1/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2748 2024-05-16 06:48:55.580986 pluralize-20240515.1/PKG-INFO
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2195 2021-07-16 07:51:13.000000 pluralize-20240515.1/README.md
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-16 06:48:55.577653 pluralize-20240515.1/pluralize/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5719 2024-05-16 06:42:17.000000 pluralize-20240515.1/pluralize/__init__.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-16 06:48:55.580986 pluralize-20240515.1/pluralize.egg-info/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2748 2024-05-16 06:48:55.000000 pluralize-20240515.1/pluralize.egg-info/PKG-INFO
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      199 2024-05-16 06:48:55.000000 pluralize-20240515.1/pluralize.egg-info/SOURCES.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2024-05-16 06:48:55.000000 pluralize-20240515.1/pluralize.egg-info/dependency_links.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       10 2024-05-16 06:48:55.000000 pluralize-20240515.1/pluralize.egg-info/top_level.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      563 2024-05-16 06:42:06.000000 pluralize-20240515.1/pyproject.toml
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       38 2024-05-16 06:48:55.580986 pluralize-20240515.1/setup.cfg
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-16 06:48:55.580986 pluralize-20240515.1/tests/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1355 2021-07-16 07:50:13.000000 pluralize-20240515.1/tests/test_simple.py
```

### Comparing `pluralize-20240413.1/PKG-INFO` & `pluralize-20240515.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pluralize
-Version: 20240413.1
+Version: 20240515.1
 Summary: i18n + pluralization library with multi-plural form support and thread safe for web apps
 Author-email: Massimo Di Pierro <massimo.dipierro@gmail.com>
 Project-URL: Homepage, https://github.com/web2py/pluralize
 Project-URL: Bug Tracker, https://github.com/web2py/yatl/pluralize
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `pluralize-20240413.1/README.md` & `pluralize-20240515.1/README.md`

 * *Files identical despite different names*

### Comparing `pluralize-20240413.1/pluralize/__init__.py` & `pluralize-20240515.1/pluralize/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import re
 import json
 import threading
 import ast
 
-__version__ = "20240413.1"
+__version__ = "20240515.1"
 
 re_language = re.compile(r"^\w\w(-\w+)*.json$")
 
 
 class lazyT(object):
 
     """accesssory object used to represent a T("string")"""
@@ -42,46 +42,47 @@
 
     def xml(self):
         """same as str but for interoperability with yatl helpers"""
         return self.translator(self.text, **self.kwargs)
 
 
 class Translator(object):
-    def __init__(self, folder=None):
+    def __init__(self, folder=None, encoding="utf-8"):
         """
         creates a translator object loading languages and pluralizations from translations/en-US.py files
         usage:
 
             T =  Translator('translations')
             print(T('dog'))
         """
         self.local = threading.local()
         self.languages = {}
         self.local.tag = None
         self.local.language = None
         self.missing = set()
         self.folder = folder
+        self.encoding = encoding
         if folder:
             self.load(folder)
 
     def load(self, folder):
         """loads languages and pluralizations from folder/en-US.json files"""
         self.languages = {}
         for filename in os.listdir(folder):
             if re_language.match(filename):
-                with open(os.path.join(folder, filename), "r", encoding="utf-8") as fp:
+                with open(os.path.join(folder, filename), "r", encoding=self.encoding) as fp:
                     self.languages[filename[:-5].lower()] = json.load(fp)
 
-    def save(self, folder=None):
+    def save(self, folder=None, ensure_ascii=True):
         """save the loaded translation files"""
         folder = folder or self.folder
         for key in self.languages:
             filename = "%s.json" % key
-            with open(os.path.join(folder, filename), "w") as fp:
-                json.dump(self.languages[key], fp, sort_keys=True, indent=4)
+            with open(os.path.join(folder, filename), "w", encoding=self.encoding) as fp:
+                json.dump(self.languages[key], fp, sort_keys=True, indent=4, ensure_ascii=ensure_ascii)
 
     def select(self, accepted_languages="fr-CH, fr;q=0.9, en;q=0.8, de;q=0.7, *;q=0.5"):
         """given appected_langauges string from HTTP header, picks the best match"""
         if isinstance(accepted_languages, str):
             accepted_languages = [
                 tag.split(";")[0].replace("_", "-").strip()
                 for tag in accepted_languages.split(",")
@@ -116,30 +117,30 @@
                 self.missing.add(text)
             elif isinstance(translations, dict) and translations:
                 k = max(int(i) for i in translations.keys() if int(i) <= n)
                 text = translations[str(k)].format(**kwargs)
         return text.format(**kwargs)
 
     @staticmethod
-    def find_matches(folder, name="T", extensions=["py", "js", "html"]):
+    def find_matches(folder, name="T", extensions=["py", "js", "html"], encoding="utf-8"):
         """finds all strings in files in folder needing translations"""
         matches_found = set()
         re_string_t = (
             r"(?<=[^\w]%s\()(?P<name>"
             r"[uU]?[rR]?(?:'''(?:[^']|'{1,2}(?!'))*''')"
             r"|(?:'(?:[^'\\]|\\.)*')"
             r'|(?:"""(?:[^"]|"{1,2}(?!"))*""")'
             r'|(?:"(?:[^"\\]|\\.)*"))'
         ) % name
         regex_t = re.compile(re_string_t)
         for root, dirs, files in os.walk(folder):
             for name in files:
                 if name.split(".")[-1] in extensions:
                     path = os.path.join(root, name)
-                    with open(path) as fp:
+                    with open(path, encoding=encoding) as fp:
                         data = fp.read()
                     items = regex_t.findall(data)
                     matches_found |= set(map(ast.literal_eval, items))
         return list(matches_found)
 
     def update_languages(self, items):
         """updates all loaded language files with the items, typically items returned by find_matches
```

### Comparing `pluralize-20240413.1/pluralize.egg-info/PKG-INFO` & `pluralize-20240515.1/pluralize.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pluralize
-Version: 20240413.1
+Version: 20240515.1
 Summary: i18n + pluralization library with multi-plural form support and thread safe for web apps
 Author-email: Massimo Di Pierro <massimo.dipierro@gmail.com>
 Project-URL: Homepage, https://github.com/web2py/pluralize
 Project-URL: Bug Tracker, https://github.com/web2py/yatl/pluralize
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `pluralize-20240413.1/pyproject.toml` & `pluralize-20240515.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pluralize"
-version = "20240413.1"
+version = "20240515.1"
 authors = [{ name="Massimo Di Pierro", email="massimo.dipierro@gmail.com" },]
 description = "i18n + pluralization library with multi-plural form support and thread safe for web apps"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
       "Programming Language :: Python :: 3",
       "License :: OSI Approved :: BSD License",
```

### Comparing `pluralize-20240413.1/tests/test_simple.py` & `pluralize-20240515.1/tests/test_simple.py`

 * *Files identical despite different names*

