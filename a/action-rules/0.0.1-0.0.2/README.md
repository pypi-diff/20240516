# Comparing `tmp/action_rules-0.0.1.tar.gz` & `tmp/action_rules-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "action_rules-0.0.1.tar", last modified: Wed May 15 22:16:28 2024, max compression
+gzip compressed data, was "action_rules-0.0.2.tar", last modified: Wed May 15 22:27:38 2024, max compression
```

## Comparing `action_rules-0.0.1.tar` & `action_rules-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 22:16:28.621169 action_rules-0.0.1/
--rw-rw-rw-   0        0        0     1088 2024-05-15 21:29:35.000000 action_rules-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     2470 2024-05-15 22:16:28.619197 action_rules-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2152 2024-05-15 22:16:21.000000 action_rules-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 22:16:28.581567 action_rules-0.0.1/action_rules/
--rw-rw-rw-   0        0        0        0 2024-05-15 21:43:28.000000 action_rules-0.0.1/action_rules/__init__.py
--rw-rw-rw-   0        0        0    16926 2024-05-15 22:16:21.000000 action_rules-0.0.1/action_rules/action_rules.py
-drwxrwxrwx   0        0        0        0 2024-05-15 22:16:28.613606 action_rules-0.0.1/action_rules.egg-info/
--rw-rw-rw-   0        0        0     2470 2024-05-15 22:16:28.000000 action_rules-0.0.1/action_rules.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2024-05-15 22:16:28.000000 action_rules-0.0.1/action_rules.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 22:16:28.000000 action_rules-0.0.1/action_rules.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-15 22:16:28.000000 action_rules-0.0.1/action_rules.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-15 22:16:28.000000 action_rules-0.0.1/action_rules.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 22:16:28.622167 action_rules-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      632 2024-05-15 21:52:00.000000 action_rules-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 22:27:38.307068 action_rules-0.0.2/
+-rw-rw-rw-   0        0        0     1088 2024-05-15 21:29:35.000000 action_rules-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     2470 2024-05-15 22:27:38.305000 action_rules-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2152 2024-05-15 22:16:21.000000 action_rules-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 22:27:38.274179 action_rules-0.0.2/action_rules/
+-rw-rw-rw-   0        0        0       29 2024-05-15 22:27:17.000000 action_rules-0.0.2/action_rules/__init__.py
+-rw-rw-rw-   0        0        0    16926 2024-05-15 22:16:21.000000 action_rules-0.0.2/action_rules/action_rules.py
+drwxrwxrwx   0        0        0        0 2024-05-15 22:27:38.301986 action_rules-0.0.2/action_rules.egg-info/
+-rw-rw-rw-   0        0        0     2470 2024-05-15 22:27:38.000000 action_rules-0.0.2/action_rules.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2024-05-15 22:27:38.000000 action_rules-0.0.2/action_rules.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 22:27:38.000000 action_rules-0.0.2/action_rules.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-15 22:27:38.000000 action_rules-0.0.2/action_rules.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-15 22:27:38.000000 action_rules-0.0.2/action_rules.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 22:27:38.307068 action_rules-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      632 2024-05-15 22:27:36.000000 action_rules-0.0.2/setup.py
```

### Comparing `action_rules-0.0.1/LICENSE.txt` & `action_rules-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `action_rules-0.0.1/PKG-INFO` & `action_rules-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: action_rules
-Version: 0.0.1
+Version: 0.0.2
 Summary: Action Rules Mining Tool.
 Home-page: https://github.com/lukassykora/actionrules
 Author: Lukas Sykora
 Author-email: lukas.sykora@vse.cz
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `action_rules-0.0.1/README.md` & `action_rules-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `action_rules-0.0.1/action_rules/action_rules.py` & `action_rules-0.0.2/action_rules/action_rules.py`

 * *Files identical despite different names*

### Comparing `action_rules-0.0.1/action_rules.egg-info/PKG-INFO` & `action_rules-0.0.2/action_rules.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: action-rules
-Version: 0.0.1
+Version: 0.0.2
 Summary: Action Rules Mining Tool.
 Home-page: https://github.com/lukassykora/actionrules
 Author: Lukas Sykora
 Author-email: lukas.sykora@vse.cz
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `action_rules-0.0.1/setup.py` & `action_rules-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 working_directory = path.abspath(path.dirname(__file__))
 
 with open(path.join(working_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='action_rules',
-    version='0.0.1',
+    version='0.0.2',
     url='https://github.com/lukassykora/actionrules',
     author='Lukas Sykora',
     author_email='lukas.sykora@vse.cz',
     description='Action Rules Mining Tool.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

