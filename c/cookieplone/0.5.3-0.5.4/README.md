# Comparing `tmp/cookieplone-0.5.3.tar.gz` & `tmp/cookieplone-0.5.4.tar.gz`

## Comparing `cookieplone-0.5.3.tar` & `cookieplone-0.5.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 cookieplone-0.5.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 cookieplone-0.5.3/CHANGES.md
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 cookieplone-0.5.3/Makefile
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cookieplone-0.5.3/tox.ini
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cookieplone-0.5.3/.github/workflows/changelog.yml
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 cookieplone-0.5.3/.github/workflows/main.yml
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 cookieplone-0.5.3/cookieplone/__init__.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 cookieplone-0.5.3/cookieplone/__main__.py
--rw-r--r--   0        0        0     5431 2020-02-02 00:00:00.000000 cookieplone-0.5.3/cookieplone/cli.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 cookieplone-0.5.3/cookieplone/data.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 cookieplone-0.5.3/cookieplone/exceptions.py
--rw-r--r--   0        0        0     4330 2020-02-02 00:00:00.000000 cookieplone-0.5.3/cookieplone/generator.py
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 cookieplone-0.5.3/cookieplone/repository.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 cookieplone-0.5.3/cookieplone/settings.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 cookieplone-0.5.3/cookieplone/filters/__init__.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 cookieplone-0.5.3/cookieplone/utils/__init__.py
--rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 cookieplone-0.5.3/cookieplone/utils/console.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 cookieplone-0.5.3/cookieplone/utils/containers.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 cookieplone-0.5.3/cookieplone/utils/files.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 cookieplone-0.5.3/cookieplone/utils/git.py
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 cookieplone-0.5.3/cookieplone/utils/internal.py
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 cookieplone-0.5.3/cookieplone/utils/sanity.py
--rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 cookieplone-0.5.3/cookieplone/utils/validators.py
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 cookieplone-0.5.3/cookieplone/utils/versions.py
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 cookieplone-0.5.3/cookieplone/utils/commands/__init__.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 cookieplone-0.5.3/news/.changelog_template.jinja
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cookieplone-0.5.3/tests/__init__.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 cookieplone-0.5.3/tests/conftest.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 cookieplone-0.5.3/tests/test_cli.py
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 cookieplone-0.5.3/tests/test_filters.py
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 cookieplone-0.5.3/tests/utils/test_commands.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 cookieplone-0.5.3/tests/utils/test_console.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 cookieplone-0.5.3/tests/utils/test_containers.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 cookieplone-0.5.3/tests/utils/test_files.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 cookieplone-0.5.3/tests/utils/test_git.py
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 cookieplone-0.5.3/tests/utils/test_internal.py
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 cookieplone-0.5.3/tests/utils/test_sanity.py
--rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 cookieplone-0.5.3/tests/utils/test_validators.py
--rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 cookieplone-0.5.3/tests/utils/test_versions.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 cookieplone-0.5.3/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 cookieplone-0.5.3/LICENSE
--rw-r--r--   0        0        0     5792 2020-02-02 00:00:00.000000 cookieplone-0.5.3/README.md
--rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 cookieplone-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     7154 2020-02-02 00:00:00.000000 cookieplone-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 cookieplone-0.5.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 cookieplone-0.5.4/CHANGES.md
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 cookieplone-0.5.4/Makefile
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cookieplone-0.5.4/tox.ini
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cookieplone-0.5.4/.github/workflows/changelog.yml
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 cookieplone-0.5.4/.github/workflows/main.yml
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 cookieplone-0.5.4/cookieplone/__init__.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 cookieplone-0.5.4/cookieplone/__main__.py
+-rw-r--r--   0        0        0     5431 2020-02-02 00:00:00.000000 cookieplone-0.5.4/cookieplone/cli.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 cookieplone-0.5.4/cookieplone/data.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 cookieplone-0.5.4/cookieplone/exceptions.py
+-rw-r--r--   0        0        0     4330 2020-02-02 00:00:00.000000 cookieplone-0.5.4/cookieplone/generator.py
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 cookieplone-0.5.4/cookieplone/repository.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 cookieplone-0.5.4/cookieplone/settings.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 cookieplone-0.5.4/cookieplone/filters/__init__.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 cookieplone-0.5.4/cookieplone/utils/__init__.py
+-rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 cookieplone-0.5.4/cookieplone/utils/console.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 cookieplone-0.5.4/cookieplone/utils/containers.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 cookieplone-0.5.4/cookieplone/utils/files.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 cookieplone-0.5.4/cookieplone/utils/git.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 cookieplone-0.5.4/cookieplone/utils/internal.py
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 cookieplone-0.5.4/cookieplone/utils/sanity.py
+-rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 cookieplone-0.5.4/cookieplone/utils/validators.py
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 cookieplone-0.5.4/cookieplone/utils/versions.py
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 cookieplone-0.5.4/cookieplone/utils/commands/__init__.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 cookieplone-0.5.4/news/.changelog_template.jinja
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cookieplone-0.5.4/tests/__init__.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 cookieplone-0.5.4/tests/conftest.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 cookieplone-0.5.4/tests/test_cli.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 cookieplone-0.5.4/tests/test_filters.py
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 cookieplone-0.5.4/tests/utils/test_commands.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 cookieplone-0.5.4/tests/utils/test_console.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 cookieplone-0.5.4/tests/utils/test_containers.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 cookieplone-0.5.4/tests/utils/test_files.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 cookieplone-0.5.4/tests/utils/test_git.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 cookieplone-0.5.4/tests/utils/test_internal.py
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 cookieplone-0.5.4/tests/utils/test_sanity.py
+-rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 cookieplone-0.5.4/tests/utils/test_validators.py
+-rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 cookieplone-0.5.4/tests/utils/test_versions.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 cookieplone-0.5.4/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 cookieplone-0.5.4/LICENSE
+-rw-r--r--   0        0        0     5792 2020-02-02 00:00:00.000000 cookieplone-0.5.4/README.md
+-rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 cookieplone-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     7154 2020-02-02 00:00:00.000000 cookieplone-0.5.4/PKG-INFO
```

### Comparing `cookieplone-0.5.3/.pre-commit-config.yaml` & `cookieplone-0.5.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.3/CHANGES.md` & `cookieplone-0.5.4/CHANGES.md`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,21 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 0.5.4 (2024-05-16)
+
+
+### Bug fixes:
+
+- Fix `cookieplone.generator._get_repository_root` to get the repository from the **_repo_dir** context variable [@ericof] [#20](https://github.com/plone/cookieplone/issues/20)
+
 ## 0.5.3 (2024-05-15)
 
 
 ### Bug fixes:
 
 - Fix extra_context parsing [@ericof] [#18](https://github.com/plone/cookieplone/issues/18)
```

### Comparing `cookieplone-0.5.3/Makefile` & `cookieplone-0.5.4/Makefile`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.3/.github/workflows/changelog.yml` & `cookieplone-0.5.4/.github/workflows/changelog.yml`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.3/.github/workflows/main.yml` & `cookieplone-0.5.4/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.3/cookieplone/cli.py` & `cookieplone-0.5.4/cookieplone/cli.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.3/cookieplone/data.py` & `cookieplone-0.5.4/cookieplone/data.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.3/cookieplone/exceptions.py` & `cookieplone-0.5.4/cookieplone/exceptions.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.3/cookieplone/generator.py` & `cookieplone-0.5.4/cookieplone/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         key: value for key, value in context.items() if not key.startswith("_")
     }
     return new_context
 
 
 def _get_repository_root(context: OrderedDict, template: str) -> Path:
     """Return the templates root."""
-    repository = context.get("_checkout") or context.get("_template")
+    repository = context.get("_repo_dir") or context.get("_template")
     if not repository:
         raise exc.RepositoryNotFound()
     repository = Path(repository).resolve()
     if not repository:
         raise exc.RepositoryNotFound()
     elif not (repository / template).exists():
         # We are probably inside a template folder,
```

### Comparing `cookieplone-0.5.3/cookieplone/repository.py` & `cookieplone-0.5.4/cookieplone/repository.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.3/cookieplone/settings.py` & `cookieplone-0.5.4/cookieplone/settings.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.3/cookieplone/filters/__init__.py` & `cookieplone-0.5.4/cookieplone/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.3/cookieplone/utils/console.py` & `cookieplone-0.5.4/cookieplone/utils/console.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.3/cookieplone/utils/files.py` & `cookieplone-0.5.4/cookieplone/utils/files.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.3/cookieplone/utils/git.py` & `cookieplone-0.5.4/cookieplone/utils/git.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.3/cookieplone/utils/internal.py` & `cookieplone-0.5.4/cookieplone/utils/internal.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.3/cookieplone/utils/sanity.py` & `cookieplone-0.5.4/cookieplone/utils/sanity.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.3/cookieplone/utils/validators.py` & `cookieplone-0.5.4/cookieplone/utils/validators.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.3/cookieplone/utils/versions.py` & `cookieplone-0.5.4/cookieplone/utils/versions.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.3/cookieplone/utils/commands/__init__.py` & `cookieplone-0.5.4/cookieplone/utils/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.3/tests/test_cli.py` & `cookieplone-0.5.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.3/tests/test_filters.py` & `cookieplone-0.5.4/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.3/tests/utils/test_commands.py` & `cookieplone-0.5.4/tests/utils/test_commands.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.3/tests/utils/test_console.py` & `cookieplone-0.5.4/tests/utils/test_console.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.3/tests/utils/test_files.py` & `cookieplone-0.5.4/tests/utils/test_files.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.3/tests/utils/test_git.py` & `cookieplone-0.5.4/tests/utils/test_git.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.3/tests/utils/test_internal.py` & `cookieplone-0.5.4/tests/utils/test_internal.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.3/tests/utils/test_sanity.py` & `cookieplone-0.5.4/tests/utils/test_sanity.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.3/tests/utils/test_validators.py` & `cookieplone-0.5.4/tests/utils/test_validators.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.3/tests/utils/test_versions.py` & `cookieplone-0.5.4/tests/utils/test_versions.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.3/.gitignore` & `cookieplone-0.5.4/.gitignore`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.3/LICENSE` & `cookieplone-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.3/README.md` & `cookieplone-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.3/pyproject.toml` & `cookieplone-0.5.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.3/PKG-INFO` & `cookieplone-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cookieplone
-Version: 0.5.3
+Version: 0.5.4
 Summary: Create Plone projects, addons, documentation with ease!
 Project-URL: Documentation, https://github.com/plone/cookieplone#readme
 Project-URL: Issues, https://github.com/plone/cookieplone/issues
 Project-URL: Source, https://github.com/plone/cookieplone
 Author-email: Plone Community <dev@plone.org>
 License-Expression: MIT
 License-File: LICENSE
```

