# Comparing `tmp/cookieplone-0.5.2.tar.gz` & `tmp/cookieplone-0.5.3.tar.gz`

## Comparing `cookieplone-0.5.2.tar` & `cookieplone-0.5.3.tar`

### file list

```diff
@@ -1,43 +1,44 @@
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 cookieplone-0.5.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 cookieplone-0.5.2/CHANGES.md
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 cookieplone-0.5.2/Makefile
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cookieplone-0.5.2/tox.ini
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cookieplone-0.5.2/.github/workflows/changelog.yml
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 cookieplone-0.5.2/.github/workflows/main.yml
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 cookieplone-0.5.2/cookieplone/__init__.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 cookieplone-0.5.2/cookieplone/__main__.py
--rw-r--r--   0        0        0     5394 2020-02-02 00:00:00.000000 cookieplone-0.5.2/cookieplone/cli.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 cookieplone-0.5.2/cookieplone/data.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 cookieplone-0.5.2/cookieplone/exceptions.py
--rw-r--r--   0        0        0     4330 2020-02-02 00:00:00.000000 cookieplone-0.5.2/cookieplone/generator.py
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 cookieplone-0.5.2/cookieplone/repository.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 cookieplone-0.5.2/cookieplone/settings.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 cookieplone-0.5.2/cookieplone/filters/__init__.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 cookieplone-0.5.2/cookieplone/utils/__init__.py
--rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 cookieplone-0.5.2/cookieplone/utils/console.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 cookieplone-0.5.2/cookieplone/utils/containers.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 cookieplone-0.5.2/cookieplone/utils/files.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 cookieplone-0.5.2/cookieplone/utils/git.py
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 cookieplone-0.5.2/cookieplone/utils/internal.py
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 cookieplone-0.5.2/cookieplone/utils/sanity.py
--rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 cookieplone-0.5.2/cookieplone/utils/validators.py
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 cookieplone-0.5.2/cookieplone/utils/versions.py
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 cookieplone-0.5.2/cookieplone/utils/commands/__init__.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 cookieplone-0.5.2/news/.changelog_template.jinja
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cookieplone-0.5.2/tests/__init__.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 cookieplone-0.5.2/tests/conftest.py
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 cookieplone-0.5.2/tests/test_filters.py
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 cookieplone-0.5.2/tests/utils/test_commands.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 cookieplone-0.5.2/tests/utils/test_console.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 cookieplone-0.5.2/tests/utils/test_containers.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 cookieplone-0.5.2/tests/utils/test_files.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 cookieplone-0.5.2/tests/utils/test_git.py
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 cookieplone-0.5.2/tests/utils/test_internal.py
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 cookieplone-0.5.2/tests/utils/test_sanity.py
--rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 cookieplone-0.5.2/tests/utils/test_validators.py
--rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 cookieplone-0.5.2/tests/utils/test_versions.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 cookieplone-0.5.2/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 cookieplone-0.5.2/LICENSE
--rw-r--r--   0        0        0     5792 2020-02-02 00:00:00.000000 cookieplone-0.5.2/README.md
--rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 cookieplone-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     7154 2020-02-02 00:00:00.000000 cookieplone-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 cookieplone-0.5.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 cookieplone-0.5.3/CHANGES.md
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 cookieplone-0.5.3/Makefile
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cookieplone-0.5.3/tox.ini
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cookieplone-0.5.3/.github/workflows/changelog.yml
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 cookieplone-0.5.3/.github/workflows/main.yml
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 cookieplone-0.5.3/cookieplone/__init__.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 cookieplone-0.5.3/cookieplone/__main__.py
+-rw-r--r--   0        0        0     5431 2020-02-02 00:00:00.000000 cookieplone-0.5.3/cookieplone/cli.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 cookieplone-0.5.3/cookieplone/data.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 cookieplone-0.5.3/cookieplone/exceptions.py
+-rw-r--r--   0        0        0     4330 2020-02-02 00:00:00.000000 cookieplone-0.5.3/cookieplone/generator.py
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 cookieplone-0.5.3/cookieplone/repository.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 cookieplone-0.5.3/cookieplone/settings.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 cookieplone-0.5.3/cookieplone/filters/__init__.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 cookieplone-0.5.3/cookieplone/utils/__init__.py
+-rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 cookieplone-0.5.3/cookieplone/utils/console.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 cookieplone-0.5.3/cookieplone/utils/containers.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 cookieplone-0.5.3/cookieplone/utils/files.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 cookieplone-0.5.3/cookieplone/utils/git.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 cookieplone-0.5.3/cookieplone/utils/internal.py
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 cookieplone-0.5.3/cookieplone/utils/sanity.py
+-rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 cookieplone-0.5.3/cookieplone/utils/validators.py
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 cookieplone-0.5.3/cookieplone/utils/versions.py
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 cookieplone-0.5.3/cookieplone/utils/commands/__init__.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 cookieplone-0.5.3/news/.changelog_template.jinja
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cookieplone-0.5.3/tests/__init__.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 cookieplone-0.5.3/tests/conftest.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 cookieplone-0.5.3/tests/test_cli.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 cookieplone-0.5.3/tests/test_filters.py
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 cookieplone-0.5.3/tests/utils/test_commands.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 cookieplone-0.5.3/tests/utils/test_console.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 cookieplone-0.5.3/tests/utils/test_containers.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 cookieplone-0.5.3/tests/utils/test_files.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 cookieplone-0.5.3/tests/utils/test_git.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 cookieplone-0.5.3/tests/utils/test_internal.py
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 cookieplone-0.5.3/tests/utils/test_sanity.py
+-rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 cookieplone-0.5.3/tests/utils/test_validators.py
+-rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 cookieplone-0.5.3/tests/utils/test_versions.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 cookieplone-0.5.3/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 cookieplone-0.5.3/LICENSE
+-rw-r--r--   0        0        0     5792 2020-02-02 00:00:00.000000 cookieplone-0.5.3/README.md
+-rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 cookieplone-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     7154 2020-02-02 00:00:00.000000 cookieplone-0.5.3/PKG-INFO
```

### Comparing `cookieplone-0.5.2/.pre-commit-config.yaml` & `cookieplone-0.5.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.2/CHANGES.md` & `cookieplone-0.5.3/CHANGES.md`

 * *Files 21% similar despite different names*

```diff
@@ -5,14 +5,21 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 0.5.3 (2024-05-15)
+
+
+### Bug fixes:
+
+- Fix extra_context parsing [@ericof] [#18](https://github.com/plone/cookieplone/issues/18)
+
 ## 0.5.2 (2024-05-13)
 
 
 ### Bug fixes:
 
 - Set default `tag` value to **main** instead of the empty string [@ericof] [#15](https://github.com/plone/cookieplone/issues/15)
```

### Comparing `cookieplone-0.5.2/Makefile` & `cookieplone-0.5.3/Makefile`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.2/.github/workflows/changelog.yml` & `cookieplone-0.5.3/.github/workflows/changelog.yml`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.2/.github/workflows/main.yml` & `cookieplone-0.5.3/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.2/cookieplone/cli.py` & `cookieplone-0.5.3/cookieplone/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,27 +15,32 @@
 from cookieplone import data, settings
 from cookieplone.exceptions import GeneratorException
 from cookieplone.generator import generate
 from cookieplone.repository import get_base_repository, get_template_options
 from cookieplone.utils import console, internal
 
 
-def validate_extra_context(value: list[str] | None = None):
+def validate_extra_context(value: list[str] | None = None) -> list[str]:
     """Validate extra content follows the correct pattern."""
     if not value:
-        return {}
-    for string in value:
-        if "=" not in string:
+        return []
+    for item in value:
+        if "=" not in item:
             raise typer.BadParameter(
                 f"EXTRA_CONTEXT should contain items of the form key=value; "
-                f"'{string}' doesn't match that form"
+                f"'{item}' doesn't match that form"
             )
-    # Convert list -- e.g.: ['program_name=foobar', 'startsecs=66']
-    # to dict -- e.g.: {'program_name': 'foobar', 'startsecs': '66'}
-    return dict([s.split("=", 1) for s in value])
+    return value
+
+
+def parse_extra_content(value: list[str]) -> dict:
+    """Parse extra content and return a dictionary with options."""
+    if not value:
+        return {}
+    return dict([s.split("=") for s in value])
 
 
 def prompt_for_template(base_path: Path) -> str:
     """Parse cookiecutter.json in base_path and prompt user to choose."""
     templates = get_template_options(base_path)
     choices = {i[0]: i[1] for i in templates}
     console.welcome_screen(templates)
@@ -128,15 +133,15 @@
     passwd = os.environ.get(
         settings.REPO_PASSWORD, os.environ.get("COOKIECUTTER_REPO_PASSWORD")
     )
     if not output_dir:
         output_dir = Path().cwd()
     configure_logger(stream_level="DEBUG" if verbose else "INFO", debug_file=debug_file)
     # Annotate extra_context
-    extra_context = extra_context if extra_context else {}
+    extra_context = parse_extra_content(extra_context)
     extra_context["__generator_signature"] = internal.signature_md(repo_path)
     # Run generator
     try:
         generate(
             repository,
             tag,
             no_input,
```

### Comparing `cookieplone-0.5.2/cookieplone/data.py` & `cookieplone-0.5.3/cookieplone/data.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.2/cookieplone/exceptions.py` & `cookieplone-0.5.3/cookieplone/exceptions.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.2/cookieplone/generator.py` & `cookieplone-0.5.3/cookieplone/generator.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.2/cookieplone/repository.py` & `cookieplone-0.5.3/cookieplone/repository.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.2/cookieplone/settings.py` & `cookieplone-0.5.3/cookieplone/settings.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.2/cookieplone/filters/__init__.py` & `cookieplone-0.5.3/cookieplone/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.2/cookieplone/utils/console.py` & `cookieplone-0.5.3/cookieplone/utils/console.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.2/cookieplone/utils/files.py` & `cookieplone-0.5.3/cookieplone/utils/files.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.2/cookieplone/utils/git.py` & `cookieplone-0.5.3/cookieplone/utils/git.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.2/cookieplone/utils/internal.py` & `cookieplone-0.5.3/cookieplone/utils/internal.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.2/cookieplone/utils/sanity.py` & `cookieplone-0.5.3/cookieplone/utils/sanity.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.2/cookieplone/utils/validators.py` & `cookieplone-0.5.3/cookieplone/utils/validators.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.2/cookieplone/utils/versions.py` & `cookieplone-0.5.3/cookieplone/utils/versions.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.2/cookieplone/utils/commands/__init__.py` & `cookieplone-0.5.3/cookieplone/utils/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.2/tests/test_filters.py` & `cookieplone-0.5.3/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.2/tests/utils/test_commands.py` & `cookieplone-0.5.3/tests/utils/test_commands.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.2/tests/utils/test_console.py` & `cookieplone-0.5.3/tests/utils/test_console.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.2/tests/utils/test_files.py` & `cookieplone-0.5.3/tests/utils/test_files.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.2/tests/utils/test_git.py` & `cookieplone-0.5.3/tests/utils/test_git.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.2/tests/utils/test_internal.py` & `cookieplone-0.5.3/tests/utils/test_internal.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.2/tests/utils/test_sanity.py` & `cookieplone-0.5.3/tests/utils/test_sanity.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.2/tests/utils/test_validators.py` & `cookieplone-0.5.3/tests/utils/test_validators.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.2/tests/utils/test_versions.py` & `cookieplone-0.5.3/tests/utils/test_versions.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.2/.gitignore` & `cookieplone-0.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.2/LICENSE` & `cookieplone-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.2/README.md` & `cookieplone-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.2/pyproject.toml` & `cookieplone-0.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.2/PKG-INFO` & `cookieplone-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cookieplone
-Version: 0.5.2
+Version: 0.5.3
 Summary: Create Plone projects, addons, documentation with ease!
 Project-URL: Documentation, https://github.com/plone/cookieplone#readme
 Project-URL: Issues, https://github.com/plone/cookieplone/issues
 Project-URL: Source, https://github.com/plone/cookieplone
 Author-email: Plone Community <dev@plone.org>
 License-Expression: MIT
 License-File: LICENSE
```

