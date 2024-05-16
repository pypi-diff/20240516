# Comparing `tmp/ldif-4.2.4.tar.gz` & `tmp/ldif-4.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ldif-4.2.4.tar", max compression
+gzip compressed data, was "ldif-4.2.5.tar", max compression
```

## Comparing `ldif-4.2.4.tar` & `ldif-4.2.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1399 2020-11-16 18:16:35.000000 ldif-4.2.4/LICENSE
--rw-r--r--   0        0        0     2054 2023-03-29 08:42:39.861991 ldif-4.2.4/README.md
--rw-r--r--   0        0        0     1396 2024-01-05 16:12:08.089090 ldif-4.2.4/pyproject.toml
--rw-r--r--   0        0        0    13179 2024-01-05 16:12:01.455206 ldif-4.2.4/src/ldif.py
--rw-r--r--   0        0        0     3068 1970-01-01 00:00:00.000000 ldif-4.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1399 2020-11-16 18:16:35.000000 ldif-4.2.5/LICENSE
+-rw-r--r--   0        0        0     2054 2023-03-29 08:42:39.861991 ldif-4.2.5/README.md
+-rw-r--r--   0        0        0     1348 2024-05-16 08:55:53.240446 ldif-4.2.5/pyproject.toml
+-rw-r--r--   0        0        0    13171 2024-05-16 08:55:32.790938 ldif-4.2.5/src/ldif.py
+-rw-r--r--   0        0        0     3030 1970-01-01 00:00:00.000000 ldif-4.2.5/PKG-INFO
```

### Comparing `ldif-4.2.4/LICENSE` & `ldif-4.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ldif-4.2.4/README.md` & `ldif-4.2.5/README.md`

 * *Files identical despite different names*

### Comparing `ldif-4.2.4/pyproject.toml` & `ldif-4.2.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ldif"
-version = "4.2.4"
+version = "4.2.5"
 description = "generate and parse LDIF data (see RFC 2849)."
 license = "BSD"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "License :: OSI Approved :: BSD License",
@@ -14,35 +14,33 @@
 homepage = "https://github.com/abilian/ldif"
 documentation = "https://ldif.readthedocs.io/en/latest/"
 authors = ["Abilian SAS <dev@abilian.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-pip = "^23.0.1"
 
-[tool.poetry.dev-dependencies]
-abilian-devtools = "^0.4.13"
+[tool.poetry.group.dev.dependencies]
+abilian-devtools = "^0.5"
 
 # Testing
 # pytest = "*"
 pytest-randomly = "*"
 coveralls = "*"
 typeguard = "*"
 
 # Needed for some reason
-pyyaml = "*"
+# pyyaml = "*"
 
 # Doc
 sphinx = "*"
 sphinx-rtd-theme = "*"
 restructuredtext_lint = "*"
 recommonmark = "*"
 
-[tool.poetry.group.dev.dependencies]
 docformatter = "^1.6.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
```

### Comparing `ldif-4.2.4/src/ldif.py` & `ldif-4.2.5/src/ldif.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
         self._fold_line(line.encode("ascii"))
 
     def _unparse_entry_record(self, entry):
         """
         :type entry: Dict[string, List[string]]
         :param entry: Dictionary holding an entry
         """
-        for attr_type in sorted(entry.keys()):
+        for attr_type in entry.keys():
             for attr_value in entry[attr_type]:
                 self._unparse_attr(attr_type, attr_value)
 
     def _unparse_changetype(self, mod_len):
         """Detect and write the changetype."""
         if mod_len == 2:
             changetype = "add"
```

### Comparing `ldif-4.2.4/PKG-INFO` & `ldif-4.2.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ldif
-Version: 4.2.4
+Version: 4.2.5
 Summary: generate and parse LDIF data (see RFC 2849).
 Home-page: https://github.com/abilian/ldif
 License: BSD
 Author: Abilian SAS
 Author-email: dev@abilian.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,15 +15,14 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Systems Administration :: Authentication/Directory :: LDAP
-Requires-Dist: pip (>=23.0.1,<24.0.0)
 Project-URL: Documentation, https://ldif.readthedocs.io/en/latest/
 Description-Content-Type: text/markdown
 
 # ldif - parse and generate LDIF data (see [RFC 2849](https://tools.ietf.org/html/rfc2849)).
 
 ![Commit activity](https://img.shields.io/github/commit-activity/m/abilian/ldif)
 ![Code size in bytes](https://img.shields.io/github/languages/code-size/abilian/ldif)
```

