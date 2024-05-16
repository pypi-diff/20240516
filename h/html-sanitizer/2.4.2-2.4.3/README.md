# Comparing `tmp/html_sanitizer-2.4.2.tar.gz` & `tmp/html_sanitizer-2.4.3.tar.gz`

## Comparing `html_sanitizer-2.4.2.tar` & `html_sanitizer-2.4.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 html_sanitizer-2.4.2/.editorconfig
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 html_sanitizer-2.4.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     6354 2020-02-02 00:00:00.000000 html_sanitizer-2.4.2/CHANGELOG.rst
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 html_sanitizer-2.4.2/tox.ini
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 html_sanitizer-2.4.2/.github/workflows/test.yml
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 html_sanitizer-2.4.2/html_sanitizer/__init__.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 html_sanitizer-2.4.2/html_sanitizer/__main__.py
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 html_sanitizer-2.4.2/html_sanitizer/django.py
--rw-r--r--   0        0        0    13787 2020-02-02 00:00:00.000000 html_sanitizer-2.4.2/html_sanitizer/sanitizer.py
--rw-r--r--   0        0        0    24536 2020-02-02 00:00:00.000000 html_sanitizer-2.4.2/html_sanitizer/tests.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 html_sanitizer-2.4.2/.gitignore
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 html_sanitizer-2.4.2/LICENSE
--rw-r--r--   0        0        0     6795 2020-02-02 00:00:00.000000 html_sanitizer-2.4.2/README.rst
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 html_sanitizer-2.4.2/pyproject.toml
--rw-r--r--   0        0        0     7924 2020-02-02 00:00:00.000000 html_sanitizer-2.4.2/PKG-INFO
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 html_sanitizer-2.4.3/.editorconfig
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 html_sanitizer-2.4.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     6410 2020-02-02 00:00:00.000000 html_sanitizer-2.4.3/CHANGELOG.rst
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 html_sanitizer-2.4.3/tox.ini
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 html_sanitizer-2.4.3/.github/workflows/test.yml
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 html_sanitizer-2.4.3/html_sanitizer/__init__.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 html_sanitizer-2.4.3/html_sanitizer/__main__.py
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 html_sanitizer-2.4.3/html_sanitizer/django.py
+-rw-r--r--   0        0        0    13871 2020-02-02 00:00:00.000000 html_sanitizer-2.4.3/html_sanitizer/sanitizer.py
+-rw-r--r--   0        0        0    25020 2020-02-02 00:00:00.000000 html_sanitizer-2.4.3/html_sanitizer/tests.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 html_sanitizer-2.4.3/.gitignore
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 html_sanitizer-2.4.3/LICENSE
+-rw-r--r--   0        0        0     6795 2020-02-02 00:00:00.000000 html_sanitizer-2.4.3/README.rst
+-rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 html_sanitizer-2.4.3/pyproject.toml
+-rw-r--r--   0        0        0     7920 2020-02-02 00:00:00.000000 html_sanitizer-2.4.3/PKG-INFO
```

### Comparing `html_sanitizer-2.4.2/.pre-commit-config.yaml` & `html_sanitizer-2.4.3/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 exclude: ".yarn/|yarn.lock|\\.min\\.(css|js)$"
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: check-added-large-files
       - id: check-builtin-literals
       - id: check-executables-have-shebangs
       - id: check-merge-conflict
       - id: check-toml
       - id: check-yaml
       - id: detect-private-key
       - id: end-of-file-fixer
       - id: mixed-line-ending
       - id: trailing-whitespace
   - repo: https://github.com/adamchainz/django-upgrade
-    rev: 1.15.0
+    rev: 1.17.0
     hooks:
       - id: django-upgrade
         args: [--target-version, "3.2"]
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.1.11"
+    rev: "v0.4.4"
     hooks:
       - id: ruff
       - id: ruff-format
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: v4.0.0-alpha.8
     hooks:
       - id: prettier
         entry: env PRETTIER_LEGACY_CLI=1 prettier
         types_or: [javascript, css, markdown]
         args: [--no-semi]
         exclude: "^conf/|.*\\.html$"
   - repo: https://github.com/tox-dev/pyproject-fmt
-    rev: 1.5.3
+    rev: 2.1.1
     hooks:
       - id: pyproject-fmt
   - repo: https://github.com/abravalheri/validate-pyproject
-    rev: v0.15
+    rev: v0.17
     hooks:
       - id: validate-pyproject
```

### Comparing `html_sanitizer-2.4.2/CHANGELOG.rst` & `html_sanitizer-2.4.3/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 Next version
 ============
 
 - **Vulnerability:** Fixed an issue where normalizing unicode too late in the
   process would keep disallowed tags when using specially crafted HTML. Fixed
   in 2.4.2.
+- Fixed missing whitespace while merging adjacent tags.
 
 
 2.4 (2024-04-01)
 ================
 
 - Fixed an edge case where ``br`` tag attributes weren't removed if the br tag
   appears first.
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_8lrdt1gw_/tmprsxzp0vq_TarContainer/0/2.rst", line 189, column 0: CDATA terminal not found*

```diff
@@ -1,13 +1,14 @@
 ========== Change log ========== Next version ============ - **Vulnerability:**
 Fixed an issue where normalizing unicode too late in the process would keep
-disallowed tags when using specially crafted HTML. Fixed in 2.4.2. 2.4 (2024-
-04-01) ================ - Fixed an edge case where ``br`` tag attributes
-weren't removed if the br tag appears first. - Updated the ``lxml`` dependency
-to 5.2 and added the now-required ``lxml[html_clean]`` extra. 2.3 (2024-02-07)
+disallowed tags when using specially crafted HTML. Fixed in 2.4.2. - Fixed
+missing whitespace while merging adjacent tags. 2.4 (2024-04-01)
+================ - Fixed an edge case where ``br`` tag attributes weren't
+removed if the br tag appears first. - Updated the ``lxml`` dependency to 5.2
+and added the now-required ``lxml[html_clean]`` extra. 2.3 (2024-02-07)
 ================ - Avoided adding whitespace when merging tags of the same
 type. - Updated the tests. - Switched from black to the ruff formatter. 2.2
 (2023-07-03) ================ - Changed ``keep_normalized_whitespace`` to
 preserve whitespace at the tail of tags, not just between tags. - Changed the
 parameters of ``normalize_whitespace_in_text_or_tail`` to be keyword-only. 2.1
 (2023-06-29) ================ - Added a test for a type of misconfiguration. -
 Changed the sanitizer configuration validation to not allow unexpected data
```

### Comparing `html_sanitizer-2.4.2/.github/workflows/test.yml` & `html_sanitizer-2.4.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `html_sanitizer-2.4.2/html_sanitizer/django.py` & `html_sanitizer-2.4.3/html_sanitizer/django.py`

 * *Files identical despite different names*

### Comparing `html_sanitizer-2.4.2/html_sanitizer/sanitizer.py` & `html_sanitizer-2.4.3/html_sanitizer/sanitizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -368,15 +368,17 @@
                     if nx.text:
                         if len(element):
                             list(element)[-1].tail = "{}{}".format(
                                 list(element)[-1].tail or "",
                                 nx.text,
                             )
                         else:
-                            element.text = "{}{}".format(element.text or "", nx.text)
+                            element.text = "{}{}{}".format(
+                                element.text or "", element.tail or "", nx.text
+                            )
 
                     for child in nx:
                         element.append(child)
 
                     # tail is merged with previous element.
                     nx.drop_tree()
```

### Comparing `html_sanitizer-2.4.2/html_sanitizer/tests.py` & `html_sanitizer-2.4.3/html_sanitizer/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -661,7 +661,22 @@
             [
                 (
                     "\uff1cimg src=x onerror=\uff02alert(window.location)\uff02\uff1e",
                     "",
                 ),
             ]
         )
+
+    def test_typographic_whitespace_tags_merging(self):
+        html = "This is <strong>some</strong> <strong>text</strong> with adjacent tags."
+        sanitizer = Sanitizer(
+            {
+                "whitespace": set(),
+                "keep_typographic_whitespace": True,
+            }
+        )
+        self.run_tests(
+            [
+                (html, "This is <strong>some text</strong>  with adjacent tags."),
+            ],
+            sanitizer=sanitizer,
+        )
```

### Comparing `html_sanitizer-2.4.2/LICENSE` & `html_sanitizer-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `html_sanitizer-2.4.2/README.rst` & `html_sanitizer-2.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `html_sanitizer-2.4.2/pyproject.toml` & `html_sanitizer-2.4.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -4,17 +4,17 @@
   "hatchling",
 ]
 
 [project]
 name = "html-sanitizer"
 description = "HTML sanitizer"
 readme = "README.rst"
-license = {text = "BSD-3-Clause"}
+license = { text = "BSD-3-Clause" }
 authors = [
-    { name = "Matthias Kestenholz", email = "mk@feinheit.ch" },
+  { name = "Matthias Kestenholz", email = "mk@feinheit.ch" },
 ]
 requires-python = ">=3.8"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Environment :: Web Environment",
   "Framework :: Django",
   "Intended Audience :: Developers",
@@ -31,27 +31,32 @@
   "Topic :: Software Development",
 ]
 dynamic = [
   "version",
 ]
 dependencies = [
   "beautifulsoup4",
-  "lxml>=5.2.0",
-  "lxml-html-clean>=0.1.0",
+  "lxml>=5.2",
+  "lxml-html-clean>=0.1",
 ]
-[project.urls]
-Homepage = "https://github.com/matthiask/html-sanitizer/"
+urls.Homepage = "https://github.com/matthiask/html-sanitizer/"
 
 [tool.hatch.version]
 path = "html_sanitizer/__init__.py"
 
 [tool.ruff]
+target-version = "py38"
+
+fix = true
+show-fixes = true
 extend-select = [
   # pyflakes, pycodestyle
-  "F", "E", "W",
+  "F",
+  "E",
+  "W",
   # mmcabe
   "C90",
   # isort
   "I",
   # pep8-naming
   "N",
   # pyupgrade
@@ -75,35 +80,28 @@
   # flake8-tidy-imports
   "TID",
   # flake8-gettext
   "INT",
   # pygrep-hooks
   "PGH",
   # pylint
-  "PLC", "PLE", "PLW",
+  "PLC",
+  "PLE",
+  "PLW",
   # unused noqa
   "RUF100",
 ]
 extend-ignore = [
   # Allow zip() without strict=
   "B905",
   # No line length errors
   "E501",
 ]
-fix = true
-show-fixes = true
-target-version = "py38"
-
-[tool.ruff.isort]
-combine-as-imports = true
-lines-after-imports = 2
-
-[tool.ruff.mccabe]
-max-complexity = 15
-
-[tool.ruff.per-file-ignores]
-"*/migrat*/*" = [
+mccabe.max-complexity = 15
+per-file-ignores."*/migrat*/*" = [
   # Allow using PascalCase model names in migrations
   "N806",
   # Ignore the fact that migration files are invalid module names
   "N999",
 ]
+isort.combine-as-imports = true
+isort.lines-after-imports = 2
```

### Comparing `html_sanitizer-2.4.2/PKG-INFO` & `html_sanitizer-2.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html-sanitizer
-Version: 2.4.2
+Version: 2.4.3
 Summary: HTML sanitizer
 Project-URL: Homepage, https://github.com/matthiask/html-sanitizer/
 Author-email: Matthias Kestenholz <mk@feinheit.ch>
 License: BSD-3-Clause
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -19,16 +19,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8
 Requires-Dist: beautifulsoup4
-Requires-Dist: lxml-html-clean>=0.1.0
-Requires-Dist: lxml>=5.2.0
+Requires-Dist: lxml-html-clean>=0.1
+Requires-Dist: lxml>=5.2
 Description-Content-Type: text/x-rst
 
 ==============
 HTML sanitizer
 ==============
 
 This is a allowlist-based and very opinionated HTML sanitizer that
```

