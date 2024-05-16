# Comparing `tmp/fh_fablib-1.0.20240116.tar.gz` & `tmp/fh_fablib-1.0.20240516.tar.gz`

## Comparing `fh_fablib-1.0.20240116.tar` & `fh_fablib-1.0.20240516.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240116/.editorconfig
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240116/.pre-commit-config.yaml
--rw-r--r--   0        0        0    21162 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240116/CHANGELOG.rst
--rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240116/bumpversion.sh
--rw-r--r--   0        0        0    26878 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240116/fh_fablib/__init__.py
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240116/fh_fablib/extract_js_gettext_strings.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240116/fh_fablib/dotfiles/.editorconfig
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240116/fh_fablib/dotfiles/.eslintrc.js
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240116/fh_fablib/dotfiles/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240116/fh_fablib/dotfiles/pyproject.toml
--rw-r--r--   0        0        0     6432 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240116/fh_fablib/dotfiles/webpack.library.js
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240116/.gitignore
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240116/LICENSE
--rw-r--r--   0        0        0     7322 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240116/README.rst
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240116/pyproject.toml
--rw-r--r--   0        0        0     7724 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240116/PKG-INFO
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240516/.editorconfig
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240516/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    21344 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240516/CHANGELOG.rst
+-rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240516/bumpversion.sh
+-rw-r--r--   0        0        0    26869 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240516/fh_fablib/__init__.py
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240516/fh_fablib/extract_js_gettext_strings.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240516/fh_fablib/dotfiles/.editorconfig
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240516/fh_fablib/dotfiles/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240516/fh_fablib/dotfiles/pyproject.toml
+-rw-r--r--   0        0        0     6465 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240516/fh_fablib/dotfiles/webpack.library.js
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240516/.gitignore
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240516/LICENSE
+-rw-r--r--   0        0        0     7322 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240516/README.rst
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240516/pyproject.toml
+-rw-r--r--   0        0        0     7724 2020-02-02 00:00:00.000000 fh_fablib-1.0.20240516/PKG-INFO
```

### Comparing `fh_fablib-1.0.20240116/.pre-commit-config.yaml` & `fh_fablib-1.0.20240516/.pre-commit-config.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 exclude: ".yarn/|yarn.lock"
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
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.1.13"
+    rev: "v0.4.4"
     hooks:
       - id: ruff
       - id: ruff-format
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v3.0.3
+    rev: v3.1.0
     hooks:
       - id: prettier
         args: [--list-different, --no-semi]
         exclude: "^conf/|.*\\.html$"
```

### Comparing `fh_fablib-1.0.20240116/CHANGELOG.rst` & `fh_fablib-1.0.20240516/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 ==========
 Change log
 ==========
 
 Next version
 ~~~~~~~~~~~~
 
+1.0.20240516
+~~~~~~~~~~~~
+
+- Prepared the webpack library for configuration schema changes in
+  webpack-dev-server 5.
+- Avoid the very annoying creation of dotfiles over and over.
+
+
 1.0.20240116
 ~~~~~~~~~~~~
 
 - Added Python 3.12 detection when rebuilding the local virtualenv.
 - Changed the webpack dev server configuration to disable the compilation
   warnings overlay by default. Re-enabled SASS warnings from dependencies now
   that warnings are less annoying.
```

### Comparing `fh_fablib-1.0.20240116/fh_fablib/__init__.py` & `fh_fablib-1.0.20240516/fh_fablib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from fabric import Connection, task
 from invoke import Collection  # noqa: F401
 from speckenv_django import django_database_url
 
 from fh_fablib.extract_js_gettext_strings import generate_strings
 
 
-__version__ = "1.0.20240116"
+__version__ = "1.0.20240516"
 
 
 # I don't care, in this context.
 warnings.simplefilter("ignore", category=ResourceWarning)
 
 
 def ansi(code):
@@ -87,15 +87,15 @@
                 f'fl.require("{__version__}")\n'
                 if line.startswith("fl.require")
                 else line
                 for line in old.splitlines(keepends=True)
             )
             if new != old:
                 path.write_text(new)
-                _update_dotfiles(force=True)
+                _update_dotfiles()
                 warning(
                     "The fabfile and dotfiles have been updated automatically.\n\nPlease check the result twice before committing!"
                 )
 
 
 def run(c, *a, **kw):
     """A Context.run or Connection.run with better defaults"""
@@ -202,29 +202,28 @@
 for job in $(jobs -p); do wait $job; done
 """
         )
         f.flush()
         run_local(ctx, f"bash {f.name}", replace_env=False)
 
 
-def _update_dotfiles(*, force):
+def _update_dotfiles():
     source = Path(__file__).parent / "dotfiles"
     target = config.base
     for s in sorted(source.glob("*")):
         t = target / s.name
-        if force or not t.exists():
-            shutil.copy(s, t)
+        shutil.copy(s, t)
 
 
 @task(auto_shortflags=False, help={"force": "Overwrite existing pre-commit files"})
 def hook(ctx, force=False):
     """
     Add default pre-commit configuration and install hook running coding style checks
     """
-    _update_dotfiles(force=force)
+    _update_dotfiles()
     run_local(ctx, "pre-commit install -f")
 
 
 @task(auto_shortflags=False)
 def dev(ctx, host="127.0.0.1", port=8000):
     """Run the development server for the frontend and backend"""
     progress(f"Starting server at http://{host}:{port}/")
@@ -404,15 +403,15 @@
         run_local(ctx, f"rm -rf venv && {_python3()} -m venv venv")
     _pip_up(ctx)
     extra = "" if stable else "--pre"
     run_local(
         ctx, f"venv/bin/python -m pip install -U -r requirements-to-freeze.txt {extra}"
     )
     freeze(ctx)
-    hook(ctx)
+    run_local(ctx, "pre-commit install -f")
 
 
 @task
 def freeze(ctx):
     """Freeze the virtualenv's state"""
     run_local(
         ctx,
@@ -437,15 +436,15 @@
             "venv/bin/python -m pip install -r requirements.txt",
             "git submodule update --init",
             'find . -name "*.pyc" -delete',
             "yarn",
         ],
     )
     run_local(ctx, "venv/bin/python manage.py migrate", warn=True)
-    hook(ctx)
+    run_local(ctx, "pre-commit install -f")
 
 
 def _local_dotenv_if_not_exists():
     dotenv = config.base / ".env"
     if dotenv.exists():
         return
```

### Comparing `fh_fablib-1.0.20240116/fh_fablib/extract_js_gettext_strings.py` & `fh_fablib-1.0.20240516/fh_fablib/extract_js_gettext_strings.py`

 * *Files identical despite different names*

### Comparing `fh_fablib-1.0.20240116/fh_fablib/dotfiles/.pre-commit-config.yaml` & `fh_fablib-1.0.20240516/fh_fablib/dotfiles/.pre-commit-config.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 exclude: ".yarn/|yarn.lock"
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
@@ -21,54 +21,36 @@
       - id: django-check
         name: django check
         entry: venv/bin/python manage.py check
         pass_filenames: false
         language: system
         always_run: true
   - repo: https://github.com/adamchainz/django-upgrade
-    rev: 1.15.0
+    rev: 1.17.0
     hooks:
       - id: django-upgrade
         args: [--target-version, "4.0"]
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.1.13"
+    rev: "v0.4.4"
     hooks:
       - id: ruff
       - id: ruff-format
-  - repo: https://github.com/pre-commit/mirrors-eslint
-    rev: v8.56.0
-    hooks:
-      - id: eslint
-        args: [--fix]
-        types_or: [css, scss, javascript]
-        verbose: true
-        additional_dependencies:
-          - eslint
-          - eslint-config-prettier
-          - eslint-config-preact
-          - eslint-plugin-compat
-          - eslint-plugin-jest
-          - eslint-plugin-react
-          - eslint-plugin-react-hooks
-          - "@babel/core"
-          - "@babel/eslint-parser"
-          - "@babel/preset-env"
-          - "@babel/preset-react"
-          - "@babel/plugin-syntax-class-properties"
-          - "@babel/plugin-syntax-decorators"
-          - "@babel/plugin-syntax-jsx"
-          - jest
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: v3.1.0
     hooks:
       - id: prettier
         args: [--list-different, --no-semi]
-        types_or: [css, scss, javascript]
+        types_or: [css, scss]
         exclude: "^conf/|.*\\.html$|.*\\.json$"
   - repo: https://github.com/tox-dev/pyproject-fmt
-    rev: 1.6.0
+    rev: 2.1.1
     hooks:
       - id: pyproject-fmt
   - repo: https://github.com/abravalheri/validate-pyproject
-    rev: v0.15
+    rev: v0.17
     hooks:
       - id: validate-pyproject
+  - repo: https://github.com/biomejs/pre-commit
+    rev: "v0.1.0"
+    hooks:
+      - id: biome-check
+        additional_dependencies: ["@biomejs/biome@1.7.3"]
```

### Comparing `fh_fablib-1.0.20240116/fh_fablib/dotfiles/pyproject.toml` & `fh_fablib-1.0.20240516/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,73 +1,84 @@
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[project]
+name = "fh-fablib"
+dynamic = ["version"]
+description = "fh-fablib"
+readme = "README.rst"
+license = {text = "BSD-3-Clause"}
+requires-python = ">=3.9"
+authors = [
+    { name = "Matthias Kestenholz", email = "mk@feinheit.ch" },
+]
+classifiers = [
+    "License :: OSI Approved :: BSD License",
+]
+dependencies = [
+    "fabric>=3",
+    "speckenv>=6.2",
+]
+
+[project.scripts]
+fl = "fabric.main:program.run"
+
+[project.urls]
+Homepage = "https://github.com/feinheit/fh-fablib/"
+
+[tool.hatch.version]
+path = "fh_fablib/__init__.py"
+
 [tool.ruff]
 extend-select = [
   # pyflakes, pycodestyle
   "F", "E", "W",
   # mmcabe
   "C90",
   # isort
   "I",
   # pep8-naming
   "N",
   # pyupgrade
   "UP",
   # flake8-2020
   "YTT",
-  # flake8-async
-  "ASYNC",
   # flake8-boolean-trap
   "FBT",
   # flake8-bugbear
   "B",
   # flake8-comprehensions
   "C4",
   # flake8-django
   "DJ",
-  # flake8-implicit-string-concatenation
-  "ISC",
-  # flake8-no-pep420
-  "INP",
   # flake8-pie
   "PIE",
-  # flake8-return
-  "RET",
-  # flake8-slots
-  "SLOT",
   # flake8-simplify
   "SIM",
-  # flake8-tidy-imports
-  "TID",
   # flake8-gettext
   "INT",
-  # flake8-use-pathlib
-  "PTH",
   # pygrep-hooks
   "PGH",
   # pylint
-  "PLC", "PLE", "PLW",
-  # tryceratops
-  "TRY",
-  # refurb
-  "FURB",
-  # flake8-logging
-  "LOG",
-  # ruff
-  "RUF005", "RUF006", "RUF007", "RUF008", "RUF009", "RUF010", "RUF011",
-  "RUF015", "RUF016", "RUF017", "RUF100", "RUF200",
+  "PL",
+  # unused noqa
+  "RUF100",
 ]
 extend-ignore = [
   # Allow zip() without strict=
   "B905",
   # No line length errors
   "E501",
+  # Fabric/invoke do not support keyword-only arguments unfortunately
+  "FBT002",
 ]
 fix = true
 show-fixes = true
-target-version = "py310"
-preview = true
+target-version = "py39"
 
 [tool.ruff.isort]
 combine-as-imports = true
 lines-after-imports = 2
 
 [tool.ruff.mccabe]
 max-complexity = 15
@@ -75,31 +86,7 @@
 [tool.ruff.per-file-ignores]
 "*/migrat*/*" = [
   # Allow using PascalCase model names in migrations
   "N806",
   # Ignore the fact that migration files are invalid module names
   "N999",
 ]
-"fabfile.py" = [
-  # No boolean trap in function definitions in the fabfile
-  "FBT002",
-]
-"conf/*" = [
-  # Allow Python files in conf/ without __init__
-  "INP",
-]
-"scripts/*" = [
-  # Allow Python files in scripts/ without __init__
-  "INP",
-]
-
-[tool.coverage.run]
-branch = true
-omit = [
-    "*migrate*",
-    "*migrations*",
-    "*venv*",
-]
-
-[tool.coverage.report]
-skip_covered = true
-show_missing = true
```

### Comparing `fh_fablib-1.0.20240116/fh_fablib/dotfiles/webpack.library.js` & `fh_fablib-1.0.20240516/fh_fablib/dotfiles/webpack.library.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -186,20 +186,22 @@
                 devMiddleware: {
                     headers: {
                         "Access-Control-Allow-Origin": "*"
                     },
                     index: true,
                     writeToDisk: (path) => /\.html$/.test(path),
                 },
-                proxy: proxySettings ?
+                proxy: [
+                    proxySettings ?
                     {
                         context: () => true,
                         target: `http://127.0.0.1:${proxySettings.backendPort}`,
                     } :
                     {},
+                ],
             }
         },
         assetRule() {
             return {
                 test: /\.(png|woff2?|svg|eot|ttf|otf|gif|jpe?g|mp3|wav)$/i,
                 type: "asset",
                 parser: {
```

### Comparing `fh_fablib-1.0.20240116/LICENSE` & `fh_fablib-1.0.20240516/LICENSE`

 * *Files identical despite different names*

### Comparing `fh_fablib-1.0.20240116/README.rst` & `fh_fablib-1.0.20240516/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 3. Add a ``fabfile.py`` to your project. A minimal example follows:
 
    .. code-block:: python
 
        import fh_fablib as fl
 
-       fl.require("1.0.20240116")
+       fl.require("1.0.20240516")
        fl.config.update(host="www-data@feinheit06.nine.ch")
 
        environments = [
            fl.environment(
                "production",
                {
                    "domain": "example.com",
@@ -90,15 +90,15 @@
 
 If you need multiple environments, add environment tasks as follows:
 
 .. code-block:: python
 
     import fh_fablib as fl
 
-    fl.require("1.0.20240116")
+    fl.require("1.0.20240516")
     fl.config.update(host="www-data@feinheit06.nine.ch")
 
     environments = [
         fl.environment(
             "production",
             {
                 "domain": "example.com",
```

### Comparing `fh_fablib-1.0.20240116/PKG-INFO` & `fh_fablib-1.0.20240516/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: fh-fablib
-Version: 1.0.20240116
+Version: 1.0.20240516
 Summary: fh-fablib
 Project-URL: Homepage, https://github.com/feinheit/fh-fablib/
 Author-email: Matthias Kestenholz <mk@feinheit.ch>
 License: BSD-3-Clause
 License-File: LICENSE
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.9
 Requires-Dist: fabric>=3
-Requires-Dist: speckenv>=3.3
+Requires-Dist: speckenv>=6.2
 Description-Content-Type: text/x-rst
 
 =========
 fh-fablib
 =========
 
 Usage
@@ -28,15 +28,15 @@
 
 3. Add a ``fabfile.py`` to your project. A minimal example follows:
 
    .. code-block:: python
 
        import fh_fablib as fl
 
-       fl.require("1.0.20240116")
+       fl.require("1.0.20240516")
        fl.config.update(host="www-data@feinheit06.nine.ch")
 
        environments = [
            fl.environment(
                "production",
                {
                    "domain": "example.com",
@@ -104,15 +104,15 @@
 
 If you need multiple environments, add environment tasks as follows:
 
 .. code-block:: python
 
     import fh_fablib as fl
 
-    fl.require("1.0.20240116")
+    fl.require("1.0.20240516")
     fl.config.update(host="www-data@feinheit06.nine.ch")
 
     environments = [
         fl.environment(
             "production",
             {
                 "domain": "example.com",
```

