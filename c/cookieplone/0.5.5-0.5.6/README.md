# Comparing `tmp/cookieplone-0.5.5.tar.gz` & `tmp/cookieplone-0.5.6.tar.gz`

## Comparing `cookieplone-0.5.5.tar` & `cookieplone-0.5.6.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 cookieplone-0.5.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 cookieplone-0.5.5/CHANGES.md
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 cookieplone-0.5.5/Makefile
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cookieplone-0.5.5/tox.ini
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cookieplone-0.5.5/.github/workflows/changelog.yml
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 cookieplone-0.5.5/.github/workflows/main.yml
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 cookieplone-0.5.5/cookieplone/__init__.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 cookieplone-0.5.5/cookieplone/__main__.py
--rw-r--r--   0        0        0     5423 2020-02-02 00:00:00.000000 cookieplone-0.5.5/cookieplone/cli.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 cookieplone-0.5.5/cookieplone/data.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 cookieplone-0.5.5/cookieplone/exceptions.py
--rw-r--r--   0        0        0     4330 2020-02-02 00:00:00.000000 cookieplone-0.5.5/cookieplone/generator.py
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 cookieplone-0.5.5/cookieplone/repository.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 cookieplone-0.5.5/cookieplone/settings.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 cookieplone-0.5.5/cookieplone/filters/__init__.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 cookieplone-0.5.5/cookieplone/utils/__init__.py
--rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 cookieplone-0.5.5/cookieplone/utils/console.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 cookieplone-0.5.5/cookieplone/utils/containers.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 cookieplone-0.5.5/cookieplone/utils/files.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 cookieplone-0.5.5/cookieplone/utils/git.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 cookieplone-0.5.5/cookieplone/utils/internal.py
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 cookieplone-0.5.5/cookieplone/utils/sanity.py
--rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 cookieplone-0.5.5/cookieplone/utils/validators.py
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 cookieplone-0.5.5/cookieplone/utils/versions.py
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 cookieplone-0.5.5/cookieplone/utils/commands/__init__.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 cookieplone-0.5.5/news/.changelog_template.jinja
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cookieplone-0.5.5/tests/__init__.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 cookieplone-0.5.5/tests/conftest.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 cookieplone-0.5.5/tests/test_cli.py
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 cookieplone-0.5.5/tests/test_filters.py
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 cookieplone-0.5.5/tests/utils/test_commands.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 cookieplone-0.5.5/tests/utils/test_console.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 cookieplone-0.5.5/tests/utils/test_containers.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 cookieplone-0.5.5/tests/utils/test_files.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 cookieplone-0.5.5/tests/utils/test_git.py
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 cookieplone-0.5.5/tests/utils/test_internal.py
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 cookieplone-0.5.5/tests/utils/test_sanity.py
--rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 cookieplone-0.5.5/tests/utils/test_validators.py
--rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 cookieplone-0.5.5/tests/utils/test_versions.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 cookieplone-0.5.5/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 cookieplone-0.5.5/LICENSE
--rw-r--r--   0        0        0     5792 2020-02-02 00:00:00.000000 cookieplone-0.5.5/README.md
--rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 cookieplone-0.5.5/pyproject.toml
--rw-r--r--   0        0        0     7154 2020-02-02 00:00:00.000000 cookieplone-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 cookieplone-0.5.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 cookieplone-0.5.6/CHANGES.md
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 cookieplone-0.5.6/Makefile
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cookieplone-0.5.6/tox.ini
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cookieplone-0.5.6/.github/workflows/changelog.yml
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 cookieplone-0.5.6/.github/workflows/main.yml
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 cookieplone-0.5.6/cookieplone/__init__.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 cookieplone-0.5.6/cookieplone/__main__.py
+-rw-r--r--   0        0        0     5551 2020-02-02 00:00:00.000000 cookieplone-0.5.6/cookieplone/cli.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 cookieplone-0.5.6/cookieplone/data.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 cookieplone-0.5.6/cookieplone/exceptions.py
+-rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 cookieplone-0.5.6/cookieplone/generator.py
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 cookieplone-0.5.6/cookieplone/repository.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 cookieplone-0.5.6/cookieplone/settings.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 cookieplone-0.5.6/cookieplone/filters/__init__.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 cookieplone-0.5.6/cookieplone/utils/__init__.py
+-rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 cookieplone-0.5.6/cookieplone/utils/console.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 cookieplone-0.5.6/cookieplone/utils/containers.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 cookieplone-0.5.6/cookieplone/utils/files.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 cookieplone-0.5.6/cookieplone/utils/git.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 cookieplone-0.5.6/cookieplone/utils/internal.py
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 cookieplone-0.5.6/cookieplone/utils/sanity.py
+-rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 cookieplone-0.5.6/cookieplone/utils/validators.py
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 cookieplone-0.5.6/cookieplone/utils/versions.py
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 cookieplone-0.5.6/cookieplone/utils/commands/__init__.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 cookieplone-0.5.6/news/.changelog_template.jinja
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cookieplone-0.5.6/tests/__init__.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 cookieplone-0.5.6/tests/conftest.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 cookieplone-0.5.6/tests/test_cli.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 cookieplone-0.5.6/tests/test_filters.py
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 cookieplone-0.5.6/tests/utils/test_commands.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 cookieplone-0.5.6/tests/utils/test_console.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 cookieplone-0.5.6/tests/utils/test_containers.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 cookieplone-0.5.6/tests/utils/test_files.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 cookieplone-0.5.6/tests/utils/test_git.py
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 cookieplone-0.5.6/tests/utils/test_internal.py
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 cookieplone-0.5.6/tests/utils/test_sanity.py
+-rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 cookieplone-0.5.6/tests/utils/test_validators.py
+-rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 cookieplone-0.5.6/tests/utils/test_versions.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 cookieplone-0.5.6/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 cookieplone-0.5.6/LICENSE
+-rw-r--r--   0        0        0     5792 2020-02-02 00:00:00.000000 cookieplone-0.5.6/README.md
+-rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 cookieplone-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0     7154 2020-02-02 00:00:00.000000 cookieplone-0.5.6/PKG-INFO
```

### Comparing `cookieplone-0.5.5/.pre-commit-config.yaml` & `cookieplone-0.5.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.5/CHANGES.md` & `cookieplone-0.5.6/CHANGES.md`

 * *Files 5% similar despite different names*

```diff
@@ -5,20 +5,27 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 0.5.6 (2024-05-16)
+
+
+### Bug fixes:
+
+- Handle in `cookieplone.generator._get_repository_root` the local development of templates containing pre_prompt hooks [@ericof]
+
 ## 0.5.5 (2024-05-16)
 
 
 ### Bug fixes:
 
-- Fix `cookieplone --version` cli command [@ericof] 
+- Fix `cookieplone --version` cli command [@ericof]
 
 ## 0.5.4 (2024-05-16)
 
 
 ### Bug fixes:
 
 - Fix `cookieplone.generator._get_repository_root` to get the repository from the **_repo_dir** context variable [@ericof] [#20](https://github.com/plone/cookieplone/issues/20)
```

### Comparing `cookieplone-0.5.5/Makefile` & `cookieplone-0.5.6/Makefile`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.5/.github/workflows/changelog.yml` & `cookieplone-0.5.6/.github/workflows/changelog.yml`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.5/.github/workflows/main.yml` & `cookieplone-0.5.6/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.5/cookieplone/cli.py` & `cookieplone-0.5.6/cookieplone/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,14 +134,16 @@
     )
     if not output_dir:
         output_dir = Path().cwd()
     configure_logger(stream_level="DEBUG" if verbose else "INFO", debug_file=debug_file)
     # Annotate extra_context
     extra_context = parse_extra_content(extra_context)
     extra_context["__generator_signature"] = internal.signature_md(repo_path)
+    extra_context["__cookieplone_repository_path"] = f"{repo_path}"
+    extra_context["__cookieplone_template"] = f"{template}"
     # Run generator
     try:
         generate(
             repository,
             tag,
             no_input,
             extra_context,
```

### Comparing `cookieplone-0.5.5/cookieplone/data.py` & `cookieplone-0.5.6/cookieplone/data.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.5/cookieplone/exceptions.py` & `cookieplone-0.5.6/cookieplone/exceptions.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.5/cookieplone/generator.py` & `cookieplone-0.5.6/cookieplone/generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,27 +18,27 @@
         key: value for key, value in context.items() if not key.startswith("_")
     }
     return new_context
 
 
 def _get_repository_root(context: OrderedDict, template: str) -> Path:
     """Return the templates root."""
-    repository = context.get("_repo_dir") or context.get("_template")
-    if not repository:
-        raise exc.RepositoryNotFound()
-    repository = Path(repository).resolve()
-    if not repository:
-        raise exc.RepositoryNotFound()
-    elif not (repository / template).exists():
-        # We are probably inside a template folder,
-        # try to check the parent
-        repository = repository.parent
-        if not (repository / template).exists():
-            raise exc.RepositoryNotFound()
-    return repository
+    possible_keys = [
+        "__cookieplone_repository_path",
+        "_repo_dir",
+        "_template",
+    ]
+    for key in possible_keys:
+        repository_path = context.get(key)
+        if not repository_path:
+            continue
+        repository = Path(repository_path).resolve()
+        if (repository / template).exists() or (repository.parent / template).exists():
+            return repository
+    raise exc.RepositoryNotFound()
 
 
 def generate(
     repository,
     tag,
     no_input,
     extra_context,
```

### Comparing `cookieplone-0.5.5/cookieplone/repository.py` & `cookieplone-0.5.6/cookieplone/repository.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.5/cookieplone/settings.py` & `cookieplone-0.5.6/cookieplone/settings.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.5/cookieplone/filters/__init__.py` & `cookieplone-0.5.6/cookieplone/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.5/cookieplone/utils/console.py` & `cookieplone-0.5.6/cookieplone/utils/console.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.5/cookieplone/utils/files.py` & `cookieplone-0.5.6/cookieplone/utils/files.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.5/cookieplone/utils/git.py` & `cookieplone-0.5.6/cookieplone/utils/git.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.5/cookieplone/utils/internal.py` & `cookieplone-0.5.6/cookieplone/utils/internal.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.5/cookieplone/utils/sanity.py` & `cookieplone-0.5.6/cookieplone/utils/sanity.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.5/cookieplone/utils/validators.py` & `cookieplone-0.5.6/cookieplone/utils/validators.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.5/cookieplone/utils/versions.py` & `cookieplone-0.5.6/cookieplone/utils/versions.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.5/cookieplone/utils/commands/__init__.py` & `cookieplone-0.5.6/cookieplone/utils/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.5/tests/test_cli.py` & `cookieplone-0.5.6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.5/tests/test_filters.py` & `cookieplone-0.5.6/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.5/tests/utils/test_commands.py` & `cookieplone-0.5.6/tests/utils/test_commands.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.5/tests/utils/test_console.py` & `cookieplone-0.5.6/tests/utils/test_console.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.5/tests/utils/test_files.py` & `cookieplone-0.5.6/tests/utils/test_files.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.5/tests/utils/test_git.py` & `cookieplone-0.5.6/tests/utils/test_git.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.5/tests/utils/test_internal.py` & `cookieplone-0.5.6/tests/utils/test_internal.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.5/tests/utils/test_sanity.py` & `cookieplone-0.5.6/tests/utils/test_sanity.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.5/tests/utils/test_validators.py` & `cookieplone-0.5.6/tests/utils/test_validators.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.5/tests/utils/test_versions.py` & `cookieplone-0.5.6/tests/utils/test_versions.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.5/.gitignore` & `cookieplone-0.5.6/.gitignore`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.5/LICENSE` & `cookieplone-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.5/README.md` & `cookieplone-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.5/pyproject.toml` & `cookieplone-0.5.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.5/PKG-INFO` & `cookieplone-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cookieplone
-Version: 0.5.5
+Version: 0.5.6
 Summary: Create Plone projects, addons, documentation with ease!
 Project-URL: Documentation, https://github.com/plone/cookieplone#readme
 Project-URL: Issues, https://github.com/plone/cookieplone/issues
 Project-URL: Source, https://github.com/plone/cookieplone
 Author-email: Plone Community <dev@plone.org>
 License-Expression: MIT
 License-File: LICENSE
```

