# Comparing `tmp/pyfancytranslator-1.0.1.tar.gz` & `tmp/pyfancytranslator-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfancytranslator-1.0.1.tar", last modified: Fri May  3 13:56:34 2024, max compression
+gzip compressed data, was "pyfancytranslator-1.0.3.tar", last modified: Sat May  4 11:59:46 2024, max compression
```

## Comparing `pyfancytranslator-1.0.1.tar` & `pyfancytranslator-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 13:56:34.619759 pyfancytranslator-1.0.1/
-drwxrwxrwx   0        0        0        0 2024-05-03 13:56:34.610495 pyfancytranslator-1.0.1/FancyTranslator/
--rw-rw-rw-   0        0        0      174 2024-05-03 11:48:29.000000 pyfancytranslator-1.0.1/FancyTranslator/__init__.py
--rw-rw-rw-   0        0        0     6362 2024-05-03 13:19:21.000000 pyfancytranslator-1.0.1/FancyTranslator/classes.py
--rw-rw-rw-   0        0        0     2596 2024-05-03 13:56:34.618574 pyfancytranslator-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2001 2024-05-03 13:55:21.000000 pyfancytranslator-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 13:56:34.617067 pyfancytranslator-1.0.1/pyfancytranslator.egg-info/
--rw-rw-rw-   0        0        0     2596 2024-05-03 13:56:34.000000 pyfancytranslator-1.0.1/pyfancytranslator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2024-05-03 13:56:34.000000 pyfancytranslator-1.0.1/pyfancytranslator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 13:56:34.000000 pyfancytranslator-1.0.1/pyfancytranslator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-03 13:56:34.000000 pyfancytranslator-1.0.1/pyfancytranslator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      716 2024-05-03 13:55:21.000000 pyfancytranslator-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-03 13:56:34.619759 pyfancytranslator-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-05-03 13:27:10.000000 pyfancytranslator-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 11:59:46.216307 pyfancytranslator-1.0.3/
+drwxrwxrwx   0        0        0        0 2024-05-04 11:59:46.203167 pyfancytranslator-1.0.3/FancyTranslator/
+-rw-rw-rw-   0        0        0      175 2024-05-04 11:59:22.000000 pyfancytranslator-1.0.3/FancyTranslator/__init__.py
+-rw-rw-rw-   0        0        0     6363 2024-05-04 11:59:22.000000 pyfancytranslator-1.0.3/FancyTranslator/classes.py
+-rw-rw-rw-   0        0        0     2596 2024-05-04 11:59:46.215345 pyfancytranslator-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2001 2024-05-03 13:55:21.000000 pyfancytranslator-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 11:59:46.214312 pyfancytranslator-1.0.3/pyfancytranslator.egg-info/
+-rw-rw-rw-   0        0        0     2596 2024-05-04 11:59:46.000000 pyfancytranslator-1.0.3/pyfancytranslator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2024-05-04 11:59:46.000000 pyfancytranslator-1.0.3/pyfancytranslator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 11:59:46.000000 pyfancytranslator-1.0.3/pyfancytranslator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-04 11:59:46.000000 pyfancytranslator-1.0.3/pyfancytranslator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      716 2024-05-04 11:59:22.000000 pyfancytranslator-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-04 11:59:46.216307 pyfancytranslator-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-05-03 13:27:10.000000 pyfancytranslator-1.0.3/setup.py
```

### Comparing `pyfancytranslator-1.0.1/FancyTranslator/classes.py` & `pyfancytranslator-1.0.3/FancyTranslator/classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
                     obj = getattr(obj, path.pop(0), None)
 
             text.replace(f'%{placeholder}%', str(obj) if obj is not None else f'None({placeholder})')
 
         return text
 
 
-_TL = TypeVar('_TL', bind=Language)
+_TL = TypeVar('_TL', bound=Language)
 
 
 class Translator:
     """
     Class holding all languages in the translation folder given.
     Parameters:
         :param path (str): The path to look for all translation files. Does not support nested folders.
```

### Comparing `pyfancytranslator-1.0.1/PKG-INFO` & `pyfancytranslator-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfancytranslator
-Version: 1.0.1
+Version: 1.0.3
 Summary: A well built translator with placeholders
 Author-email: Ashenguard <ashenguard@agmstudio.xyz>
 Project-URL: Homepage, https://github.com/agm-studio/fancytranslator
 Project-URL: Bug Tracker, https://github.com/agm-studio/fancytranslator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyfancytranslator-1.0.1/README.md` & `pyfancytranslator-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyfancytranslator-1.0.1/pyfancytranslator.egg-info/PKG-INFO` & `pyfancytranslator-1.0.3/pyfancytranslator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfancytranslator
-Version: 1.0.1
+Version: 1.0.3
 Summary: A well built translator with placeholders
 Author-email: Ashenguard <ashenguard@agmstudio.xyz>
 Project-URL: Homepage, https://github.com/agm-studio/fancytranslator
 Project-URL: Bug Tracker, https://github.com/agm-studio/fancytranslator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyfancytranslator-1.0.1/pyproject.toml` & `pyfancytranslator-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyfancytranslator"
-version = "1.0.1"
+version = "1.0.3"
 authors = [
     { name = "Ashenguard", email = "ashenguard@agmstudio.xyz" },
 ]
 description = "A well built translator with placeholders"
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
```

