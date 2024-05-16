# Comparing `tmp/ipyoptimade-0.2.0.tar.gz` & `tmp/ipyoptimade-1.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipyoptimade-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ipyoptimade-1.0.0a0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ipyoptimade-0.2.0.tar` & `ipyoptimade-1.0.0a0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     7486 2024-02-02 10:25:28.644656 ipyoptimade-0.2.0/README.md
--rw-r--r--   0        0        0     2303 2024-02-02 10:25:28.648656 ipyoptimade-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      584 2024-02-02 10:25:28.648656 ipyoptimade-0.2.0/src/ipyoptimade/__init__.py
--rw-r--r--   0        0        0     1077 2024-02-02 10:25:28.648656 ipyoptimade-0.2.0/src/ipyoptimade/default_parameters.py
--rw-r--r--   0        0        0     4514 2024-02-02 10:25:28.648656 ipyoptimade-0.2.0/src/ipyoptimade/exceptions.py
--rw-r--r--   0        0        0    16738 2024-02-02 10:25:28.648656 ipyoptimade-0.2.0/src/ipyoptimade/informational.py
--rw-r--r--   0        0        0    10287 2024-02-02 10:25:28.652656 ipyoptimade-0.2.0/src/ipyoptimade/logger.py
--rw-r--r--   0        0        0    22047 2024-02-02 10:25:28.652656 ipyoptimade-0.2.0/src/ipyoptimade/query_filter.py
--rw-r--r--   0        0        0     4212 2024-02-02 10:25:28.652656 ipyoptimade-0.2.0/src/ipyoptimade/query_provider.py
--rw-r--r--   0        0        0   122043 2024-02-02 10:25:28.652656 ipyoptimade-0.2.0/src/ipyoptimade/statics/optimade-text-right-transparent-bg.png
--rw-r--r--   0        0        0      648 2024-02-02 10:25:28.652656 ipyoptimade-0.2.0/src/ipyoptimade/subwidgets/__init__.py
--rw-r--r--   0        0        0    22105 2024-02-02 10:25:28.652656 ipyoptimade-0.2.0/src/ipyoptimade/subwidgets/filter_inputs.py
--rw-r--r--   0        0        0      509 2024-02-02 10:25:28.652656 ipyoptimade-0.2.0/src/ipyoptimade/subwidgets/intrangeslider.py
--rw-r--r--   0        0        0     2964 2024-02-02 10:25:28.652656 ipyoptimade-0.2.0/src/ipyoptimade/subwidgets/multi_checkbox.py
--rw-r--r--   0        0        0    12316 2024-02-02 10:25:28.652656 ipyoptimade-0.2.0/src/ipyoptimade/subwidgets/output_summary.py
--rw-r--r--   0        0        0     3578 2024-02-02 10:25:28.652656 ipyoptimade-0.2.0/src/ipyoptimade/subwidgets/periodic_table.py
--rw-r--r--   0        0        0    27934 2024-02-02 10:25:28.652656 ipyoptimade-0.2.0/src/ipyoptimade/subwidgets/provider_database.py
--rw-r--r--   0        0        0    14475 2024-02-02 10:25:28.652656 ipyoptimade-0.2.0/src/ipyoptimade/subwidgets/results.py
--rw-r--r--   0        0        0     6558 2024-02-02 10:25:28.652656 ipyoptimade-0.2.0/src/ipyoptimade/subwidgets/sort_selector.py
--rw-r--r--   0        0        0    20287 2024-02-02 10:25:28.652656 ipyoptimade-0.2.0/src/ipyoptimade/summary.py
--rw-r--r--   0        0        0    24610 2024-02-02 10:25:28.652656 ipyoptimade-0.2.0/src/ipyoptimade/utils.py
--rw-r--r--   0        0        0       22 2024-02-02 10:25:28.652656 ipyoptimade-0.2.0/src/ipyoptimade/version.py
--rw-r--r--   0        0        0      635 2024-02-02 10:25:28.652656 ipyoptimade-0.2.0/src/ipyoptimade/warnings.py
--rw-r--r--   0        0        0     9507 1970-01-01 00:00:00.000000 ipyoptimade-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     7491 2024-05-16 15:28:57.575510 ipyoptimade-1.0.0a0/README.md
+-rw-r--r--   0        0        0     2218 2024-05-16 15:28:57.579510 ipyoptimade-1.0.0a0/pyproject.toml
+-rw-r--r--   0        0        0      584 2024-05-16 15:28:57.579510 ipyoptimade-1.0.0a0/src/ipyoptimade/__init__.py
+-rw-r--r--   0        0        0      784 2024-05-16 15:28:57.579510 ipyoptimade-1.0.0a0/src/ipyoptimade/default_parameters.py
+-rw-r--r--   0        0        0     4514 2024-05-16 15:28:57.579510 ipyoptimade-1.0.0a0/src/ipyoptimade/exceptions.py
+-rw-r--r--   0        0        0    16491 2024-05-16 15:28:57.579510 ipyoptimade-1.0.0a0/src/ipyoptimade/informational.py
+-rw-r--r--   0        0        0    10287 2024-05-16 15:28:57.579510 ipyoptimade-1.0.0a0/src/ipyoptimade/logger.py
+-rw-r--r--   0        0        0    22047 2024-05-16 15:28:57.579510 ipyoptimade-1.0.0a0/src/ipyoptimade/query_filter.py
+-rw-r--r--   0        0        0     3895 2024-05-16 15:28:57.579510 ipyoptimade-1.0.0a0/src/ipyoptimade/query_provider.py
+-rw-r--r--   0        0        0   122043 2024-05-16 15:28:57.579510 ipyoptimade-1.0.0a0/src/ipyoptimade/statics/optimade-text-right-transparent-bg.png
+-rw-r--r--   0        0        0      648 2024-05-16 15:28:57.579510 ipyoptimade-1.0.0a0/src/ipyoptimade/subwidgets/__init__.py
+-rw-r--r--   0        0        0    22105 2024-05-16 15:28:57.579510 ipyoptimade-1.0.0a0/src/ipyoptimade/subwidgets/filter_inputs.py
+-rw-r--r--   0        0        0      509 2024-05-16 15:28:57.579510 ipyoptimade-1.0.0a0/src/ipyoptimade/subwidgets/intrangeslider.py
+-rw-r--r--   0        0        0     2964 2024-05-16 15:28:57.579510 ipyoptimade-1.0.0a0/src/ipyoptimade/subwidgets/multi_checkbox.py
+-rw-r--r--   0        0        0    12316 2024-05-16 15:28:57.579510 ipyoptimade-1.0.0a0/src/ipyoptimade/subwidgets/output_summary.py
+-rw-r--r--   0        0        0     3578 2024-05-16 15:28:57.579510 ipyoptimade-1.0.0a0/src/ipyoptimade/subwidgets/periodic_table.py
+-rw-r--r--   0        0        0    27063 2024-05-16 15:28:57.583510 ipyoptimade-1.0.0a0/src/ipyoptimade/subwidgets/provider_database.py
+-rw-r--r--   0        0        0    14475 2024-05-16 15:28:57.583510 ipyoptimade-1.0.0a0/src/ipyoptimade/subwidgets/results.py
+-rw-r--r--   0        0        0     6558 2024-05-16 15:28:57.583510 ipyoptimade-1.0.0a0/src/ipyoptimade/subwidgets/sort_selector.py
+-rw-r--r--   0        0        0    20234 2024-05-16 15:28:57.583510 ipyoptimade-1.0.0a0/src/ipyoptimade/summary.py
+-rw-r--r--   0        0        0    24566 2024-05-16 15:28:57.583510 ipyoptimade-1.0.0a0/src/ipyoptimade/utils.py
+-rw-r--r--   0        0        0       24 2024-05-16 15:28:57.583510 ipyoptimade-1.0.0a0/src/ipyoptimade/version.py
+-rw-r--r--   0        0        0      635 2024-05-16 15:28:57.583510 ipyoptimade-1.0.0a0/src/ipyoptimade/warnings.py
+-rw-r--r--   0        0        0     9500 1970-01-01 00:00:00.000000 ipyoptimade-1.0.0a0/PKG-INFO
```

### Comparing `ipyoptimade-0.2.0/README.md` & `ipyoptimade-1.0.0a0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 # OPTIMADE Jupyter widgets and Voilà application
 
 [![MaterialsCloud](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/CasperWA/voila-optimade-client/develop/docs/resources/mcloud_badge.json)](https://materialscloud.org/optimadeclient/)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/aiidalab/ipyoptimade/main?urlpath=%2Fvoila%2Frender%2Foptimade-client.ipynb)
 [![codecov](https://codecov.io/gh/aiidalab/ipyoptimade/branch/main/graph/badge.svg)](https://codecov.io/gh/aiidalab/ipyoptimade)
+[![PyPI - Version](https://img.shields.io/pypi/v/ipyoptimade?color=4CC61E)](https://pypi.org/project/ipyoptimade/)
 
 Query for and import structures from [OPTIMADE](https://www.optimade.org) providers (COD, MaterialsCloud, NoMaD, Materials Project, ODBX, OQMD, and more ...).
 The package provides a Jupyter widget for querying OPTIMADE providers and an example Voilà application to stack widgets into an web application.
 
 Current supported OPTIMADE API versions: `1.1.0`, `1.0.0`, `1.0.0-rc.2`, `1.0.0-rc.1`, `0.10.1`
 
+Install with
+
+```bash
+pip install ipyoptimade
+```
+
 ## Run the client
 
 This Jupyter-based app is intended to run either:
 
 - In [AiiDAlab](https://aiidalab.materialscloud.org) as well as inside a [Quantum Mobile](https://materialscloud.org/work/quantum-mobile) Virtual Machine;
 - As a [MaterialsCloud tool](https://materialscloud.org/optimadeclient/);
 - As a standalone [MyBinder application](https://mybinder.org/v2/gh/CasperWA/voila-optimade-client/develop?urlpath=%2Fvoila%2Frender%2FOPTIMADE-Client.ipynb); or
@@ -111,49 +118,53 @@
 
 To see the full list of configurations you can call `voila` and pass `--help-all`.
 
 ### Running with "development" providers (Materials Cloud-specific)
 
 Set the environment variable `ipyoptimade_DEVELOPMENT_MODE` to `1` (the integer version for `True` (`1`) or `False` (`0`)) in order to force the use of development servers for providers (currently only relevant for Materials Cloud).
 
-## Contribute
-
-If you wish to contribute to the application, you can install it in "editable" mode by using the `-e` flag: `pip install -e .[dev]`.
-It is recommended that you use the GitHub-route mentioned above.
+## Development
 
-You should also install `pre-commit` in the cloned git repository by running:
+Install with
 
-```shell
+```bash
+pip install -e .[dev]
 pre-commit install
 ```
 
-To start making contributions, fork the repository and create PRs.
+Set
+
+```
+export ipyoptimade_DEBUG=1
+```
 
+to automatically open and show the debug & error messages in the `OptimadeLog()` widget.
 
-## For maintainers
+### Making a new release
 
 To create a new release, clone the repository, install development dependencies with `pip install -e '.[dev]'`, and then execute `bumpver update [--major|--minor|--patch] [--tag-num --tag [alpha|beta|rc]]`.
 This will:
 
-  1. Create a tagged release with bumped version and push it to the repository.
-  2. Trigger a GitHub actions workflow that creates a GitHub release and publishes it on PyPI.
+1. Create a tagged release with bumped version and push it to the repository.
+2. Trigger a GitHub actions workflow that creates a GitHub release and publishes it on PyPI.
 
 Additional notes:
 
-  - Use the `--dry` option to preview the release change.
-  - The release tag (e.g. a/b/rc) is determined from the last release.
-    Use the `--tag` option to switch the release tag.
-  - This package follows [semantic versioning](https://semver.org/).
+- Use the `--dry` option to preview the release change.
+- The release tag (e.g. a/b/rc) is determined from the last release.
+  Use the `--tag` option to switch the release tag.
+- This package follows [semantic versioning](https://semver.org/).
 
 ## License
 
 MIT. The terms of the license can be found in the [LICENSE](LICENSE) file.
 
 ## Acknowledgements
 
+<!-- prettier-ignore -->
 | | |
 |---|---|
 | [![BIG-MAP](https://avatars1.githubusercontent.com/u/72801303?s=200&v=4)](https://www.big-map.eu/) | [BIG-MAP](https://www.big-map.eu/); This project has received funding from the European Union’s Horizon 2020 research and innovation programme under grant agreement No 957189. The project is part of [BATTERY 2030+](https://battery2030.eu/), the large-scale European research initiative for inventing the sustainable batteries of the future. |
 
 ## Contact
 
 casper+github@welzel.nu
```

### Comparing `ipyoptimade-0.2.0/pyproject.toml` & `ipyoptimade-1.0.0a0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,81 +1,76 @@
 [build-system]
 requires = ["flit"]
 build-backend = "flit.buildapi"
 
 [project]
-name =  "ipyoptimade"
+name = "ipyoptimade"
 authors = [
-    {name = "Casper Welzel Andersen", email = "casper+github@welzel.nu"},
-    {name = "Kristjan Eimre", email = "kristan.eimre@epfl.ch"},
-    {name = "Jusong Yu", email = "jusong.yu@psi.ch"},
+  { name = "Casper Welzel Andersen", email = "casper+github@welzel.nu" },
+  { name = "Kristjan Eimre", email = "kristan.eimre@epfl.ch" },
+  { name = "Jusong Yu", email = "jusong.yu@psi.ch" },
 ]
 description = "Jupyter client for searching structures through OPTIMADE API"
 readme = "README.md"
 classifiers = [
-    "Development Status :: 5 - Production/Stable",
-    "Framework :: AiiDA",
-    "Framework :: Jupyter",
-    "Intended Audience :: Science/Research",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: MacOS :: MacOS X",
-    "Operating System :: POSIX :: Linux",
-    "Operating System :: Microsoft :: Windows",
-    "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Topic :: Database :: Front-Ends",
-    "Topic :: Scientific/Engineering",
-    "Topic :: Scientific/Engineering :: Chemistry",
-    "Topic :: Scientific/Engineering :: Physics",
-    "Topic :: Software Development :: Widget Sets",
+  "Development Status :: 5 - Production/Stable",
+  "Framework :: AiiDA",
+  "Framework :: Jupyter",
+  "Intended Audience :: Science/Research",
+  "License :: OSI Approved :: MIT License",
+  "Operating System :: MacOS :: MacOS X",
+  "Operating System :: POSIX :: Linux",
+  "Operating System :: Microsoft :: Windows",
+  "Programming Language :: Python :: 3 :: Only",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Topic :: Database :: Front-Ends",
+  "Topic :: Scientific/Engineering",
+  "Topic :: Scientific/Engineering :: Chemistry",
+  "Topic :: Scientific/Engineering :: Physics",
+  "Topic :: Software Development :: Widget Sets",
 ]
 requires-python = ">=3.9"
 dynamic = ["version"] # read version from src/ipyoptimade/__init__.py
 dependencies = [
-    "appdirs~=1.4.4",
-    "cachecontrol[filecache]~=0.13.1",
-    "ipywidgets~=7.7",
-    "ipywidgets-extended>=1.1.1,<2,!=1.2.0,!=1.2.1",
-    "nglview~=3.0",
-    "optimade~=1.0.0",
-    "ase~=3.22",
-    "pandas~=2.1",
-    "requests~=2.31",
-    "widget_periodictable~=3.1",
-    "semver~=3.0",
+  "appdirs~=1.4.4",
+  "cachecontrol[filecache]~=0.13.1",
+  "ipywidgets~=8.1",
+  "nglview~=3.0",
+  "optimade~=1.0.0",
+  "ase~=3.22",
+  "pandas~=2.1",
+  "requests~=2.31",
+  "widget_periodictable~=4.1",
+  "semver~=3.0",
 ]
 
 [project.optional-dependencies]
 dev = [
-    "pre-commit~=3.6",
-    "pytest~=7.4",
-    "pytest-cov~=4.1",
-    "bumpver~=2023.1129",
-]
-voila = [
-    "voila~=0.4.0",
+  "pre-commit~=3.6",
+  "pytest~=7.4",
+  "pytest-cov~=4.1",
+  "bumpver>=2023.1129",
+  "pip-tools~=7.4",
 ]
+voila = ["voila~=0.5.0"]
 
 [project.urls]
 Documentation = "https://github.com/aiidalab/ipyoptimade#readme"
 Source = "https://github.com/aiidalab/ipyoptimade"
 Tracker = "https://github.com/aiidalab/ipyoptimade/issues"
 
 [tool.flit.module]
 name = "ipyoptimade"
 
-[bumpver]
-current_version = "0.2.0"
-version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
+[tool.bumpver]
+current_version = "v1.0.0a0"
+version_pattern = "vMAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "Bump version: {old_version} -> {new_version}"
 commit = true
+tag = true
 push = true
 
-[bumpver.file_patterns]
-"pyproject.toml" = [
-    'current_version = "{version}"',
-]
-"src/ipyoptimade/version.py" = [
-    '__version__ = "{version}"',
-]
+[tool.bumpver.file_patterns]
+"pyproject.toml" = ['current_version = "{version}"']
+"src/ipyoptimade/version.py" = ['__version__ = "{pep440_version}"']
```

### Comparing `ipyoptimade-0.2.0/src/ipyoptimade/__init__.py` & `ipyoptimade-1.0.0a0/src/ipyoptimade/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyoptimade-0.2.0/src/ipyoptimade/default_parameters.py` & `ipyoptimade-1.0.0a0/src/ipyoptimade/default_parameters.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,38 @@
 """Default initialization parameters
 
 The lists are set, based on the status of providers from
 https://www.optimade.org/providers-dashboard/.
-
-If the provider has no available databases, it should be put into the SKIP_PROVIDERS list,
-meaning it will not be supported.
-Providers in the DISABLE_PROVIDERS list are ones the client should support,
-but cannot because of one issue or another.
 """
 
+# If the provider has no available databases, it should be put into the SKIP_PROVIDERS list,
+# meaning it will not be supported.
 SKIP_PROVIDERS = [
-    "exmpl",
-    "optimade",
+    "matcloud",
     "aiida",
     "ccpnc",
-    "matcloud",
-    "necro",
     "httk",
+    "optimade",
+    "optimake",
     "pcod",
+    "exmpl",
+    "necro",
 ]
 
+# Providers in the DISABLE_PROVIDERS list are ones the client should support,
+# but cannot because of one issue or another.
 DISABLE_PROVIDERS = [
+    "aflow",
+    "cmr",
     "cod",
-    "tcod",
+    "jarvis",
+    "mpdd",
+    "mpds",
+    "mpod",
     "nmd",
     "oqmd",
-    "aflow",
-    "mpds",
-    "jarvis",
+    "tcod",
 ]
 
-PROVIDER_DATABASE_GROUPINGS = {
-    "Materials Cloud": {
-        "Main Projects": ["mc3d", "mc2d"],
-        "Contributed Projects": [
-            "2dtopo",
-            "pyrene-mofs",
-            "scdm",
-            "stoceriaitf",
-            "tc-applicability",
-            "tin-antimony-sulfoiodide",
-            "curated-cofs",
-        ],
-    }
-}
-
-
 SKIP_DATABASE = {
     "Materials Cloud": ["optimade-sample", "li-ion-conductors", "sssp"],
 }
```

### Comparing `ipyoptimade-0.2.0/src/ipyoptimade/exceptions.py` & `ipyoptimade-1.0.0a0/src/ipyoptimade/exceptions.py`

 * *Files identical despite different names*

### Comparing `ipyoptimade-0.2.0/src/ipyoptimade/informational.py` & `ipyoptimade-1.0.0a0/src/ipyoptimade/informational.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,24 +35,20 @@
 
     HEADER = f"""<p style="font-size:14px;">
 <b>Currently valid OPTIMADE API version</b>: <code>v{__optimade_version__[0]}</code><br>
 <b>Client version</b>: <code>{__ipyoptimade_version__}</code><br>
 <b>Source code</b>: <a href="{SOURCE_URL}" target="_blank">GitHub</a>
 </p>
 """
-    DESCRIPTION = f"""<p style="line-height:1.5;font-size:14px;">
+    DESCRIPTION = """<p style="line-height:1.5;font-size:14px;">
 This is a friendly client to search through databases and other implementations exposing an OPTIMADE RESTful API.
 To get more information about the OPTIMADE API,
 please see <a href="https://www.optimade.org/" target="_blank">the offical web page</a>.
 All providers are retrieved from <a href="https://providers.optimade.org/" target="_blank">the OPTIMADE consortium's list of providers</a>.
 </p>
-<p style="line-height:1.5;font-size:14px;margin-top:5px;">
-<i>Note</i>: The structure property <code>assemblies</code> is currently not supported.
-Follow <a href="{SOURCE_URL}issues/12" target="_blank">the issue on GitHub</a> to learn more.
-</p>
 """
     BUG_TEMPLATE = {
         "title": "[BUG] - TITLE",
         "body": (
             "## Bug description\n\nWhat happened?\n\n"
             "### Expected behaviour (optional)\n\nWhat should have happened?\n\n"
             "### Actual behavior (optional)\n\nWhat happened instead?\n\n"
```

### Comparing `ipyoptimade-0.2.0/src/ipyoptimade/logger.py` & `ipyoptimade-1.0.0a0/src/ipyoptimade/logger.py`

 * *Files identical despite different names*

### Comparing `ipyoptimade-0.2.0/src/ipyoptimade/query_filter.py` & `ipyoptimade-1.0.0a0/src/ipyoptimade/query_filter.py`

 * *Files identical despite different names*

### Comparing `ipyoptimade-0.2.0/src/ipyoptimade/query_provider.py` & `ipyoptimade-1.0.0a0/src/ipyoptimade/query_provider.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-from typing import Union, Tuple, List, Dict, Optional
 import warnings
+from typing import List, Optional, Tuple, Union
 
 import ipywidgets as ipw
 import traitlets
-
 from optimade.models import LinksResourceAttributes
 
+from ipyoptimade.default_parameters import (
+    DISABLE_PROVIDERS,
+    SKIP_DATABASE,
+    SKIP_PROVIDERS,
+)
 from ipyoptimade.subwidgets import (
     ProviderImplementationChooser,
     ProviderImplementationSummary,
 )
 from ipyoptimade.warnings import OptimadeClientWarning
-from ipyoptimade.default_parameters import (
-    PROVIDER_DATABASE_GROUPINGS,
-    SKIP_DATABASE,
-    SKIP_PROVIDERS,
-    DISABLE_PROVIDERS,
-)
 
 
 class OptimadeQueryProviderWidget(ipw.GridspecLayout):
     """Database/Implementation search and chooser widget for OPTIMADE
 
     NOTE: Only supports offset-pagination at the moment.
     """
@@ -36,38 +34,33 @@
         embedded: bool = False,
         database_limit: Optional[int] = None,
         width_ratio: Optional[Union[Tuple[int, int], List[int]]] = None,
         width_space: Optional[int] = None,
         disable_providers: Optional[List[str]] = None,
         skip_providers: Optional[List[str]] = None,
         skip_databases: Optional[List[str]] = None,
-        provider_database_groupings: Optional[Dict[str, Dict[str, List[str]]]] = None,
         **kwargs,
     ):
         # At the moment, the pagination does not work properly as each database is not tested for
         # validity immediately, only when each "page" is loaded. This can result in the pagination
         # failing. Instead the default is set to 100 in an attempt to never actually do paging.
         database_limit = (
             database_limit if database_limit and database_limit > 0 else 100
         )
         disable_providers = disable_providers or DISABLE_PROVIDERS
         skip_providers = skip_providers or SKIP_PROVIDERS
         skip_databases = skip_databases or SKIP_DATABASE
-        provider_database_groupings = (
-            provider_database_groupings or PROVIDER_DATABASE_GROUPINGS
-        )
 
         layout = ipw.Layout(width="100%", height="auto")
 
         self.chooser = ProviderImplementationChooser(
             child_db_limit=database_limit,
             disable_providers=disable_providers,
             skip_providers=skip_providers,
             skip_databases=skip_databases,
-            provider_database_groupings=provider_database_groupings,
             **kwargs,
         )
 
         self.summary = ProviderImplementationSummary(**kwargs) if not embedded else None
 
         if embedded:
             super().__init__(n_rows=1, n_columns=1, layout=layout, **kwargs)
```

### Comparing `ipyoptimade-0.2.0/src/ipyoptimade/statics/optimade-text-right-transparent-bg.png` & `ipyoptimade-1.0.0a0/src/ipyoptimade/statics/optimade-text-right-transparent-bg.png`

 * *Files identical despite different names*

### Comparing `ipyoptimade-0.2.0/src/ipyoptimade/subwidgets/__init__.py` & `ipyoptimade-1.0.0a0/src/ipyoptimade/subwidgets/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyoptimade-0.2.0/src/ipyoptimade/subwidgets/filter_inputs.py` & `ipyoptimade-1.0.0a0/src/ipyoptimade/subwidgets/filter_inputs.py`

 * *Files identical despite different names*

### Comparing `ipyoptimade-0.2.0/src/ipyoptimade/subwidgets/multi_checkbox.py` & `ipyoptimade-1.0.0a0/src/ipyoptimade/subwidgets/multi_checkbox.py`

 * *Files identical despite different names*

### Comparing `ipyoptimade-0.2.0/src/ipyoptimade/subwidgets/output_summary.py` & `ipyoptimade-1.0.0a0/src/ipyoptimade/subwidgets/output_summary.py`

 * *Files identical despite different names*

### Comparing `ipyoptimade-0.2.0/src/ipyoptimade/subwidgets/periodic_table.py` & `ipyoptimade-1.0.0a0/src/ipyoptimade/subwidgets/periodic_table.py`

 * *Files identical despite different names*

### Comparing `ipyoptimade-0.2.0/src/ipyoptimade/subwidgets/provider_database.py` & `ipyoptimade-1.0.0a0/src/ipyoptimade/subwidgets/provider_database.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,38 @@
 # pylint: disable=protected-access
-from copy import deepcopy
 import os
-from typing import Dict, List, Tuple, Union
 import urllib.parse
+from typing import Dict, List, Tuple, Union
 
 try:
     import simplejson as json
 except ImportError:
     import json
 
 import ipywidgets as ipw
 import requests
 import traitlets
-
-from ipywidgets_extended.dropdown import DropdownExtended
-
 from optimade.models import LinksResourceAttributes
 from optimade.models.links import LinkType
 
 from ipyoptimade.exceptions import OptimadeClientError, QueryError
 from ipyoptimade.logger import LOGGER
 from ipyoptimade.subwidgets.results import ResultsPageChooser
 from ipyoptimade.utils import (
+    SESSION,
+    TIMEOUT_SECONDS,
     get_list_of_valid_providers,
     get_versioned_base_url,
     handle_errors,
     ordered_query_url,
     perform_optimade_query,
-    SESSION,
-    TIMEOUT_SECONDS,
     update_old_links_resources,
     validate_api_version,
 )
 
-
 __all__ = ("ProviderImplementationChooser", "ProviderImplementationSummary")
 
 
 class ProviderImplementationChooser(  # pylint: disable=too-many-instance-attributes
     ipw.VBox
 ):
     """List all OPTIMADE providers and their implementations"""
@@ -46,30 +41,28 @@
     database = traitlets.Tuple(
         traitlets.Unicode(),
         traitlets.Instance(LinksResourceAttributes, allow_none=True),
         default_value=("", None),
     )
 
     HINT = {"provider": "Select a provider", "child_dbs": "Select a database"}
-    INITIAL_CHILD_DBS = [("", (("No provider chosen", None),))]
+    INITIAL_CHILD_DBS = [("No provider chosen", None)]
 
     def __init__(
         self,
         child_db_limit: int = None,
         disable_providers: List[str] = None,
         skip_providers: List[str] = None,
         skip_databases: Dict[str, List[str]] = None,
-        provider_database_groupings: Dict[str, Dict[str, List[str]]] = None,
         **kwargs,
     ):
         self.child_db_limit = (
             child_db_limit if child_db_limit and child_db_limit > 0 else 10
         )
         self.skip_child_dbs = skip_databases or {}
-        self.child_db_groupings = provider_database_groupings or {}
         self.offset = 0
         self.number = 1
         self.__perform_query = True
         self.__cached_child_dbs = {}
 
         self.debug = bool(os.environ.get("ipyoptimade_DEBUG", None))
 
@@ -88,24 +81,22 @@
                     "base_url": f"http://localhost:5000{VERSION_PARTS[0][0]}",
                     "homepage": "https://example.org",
                     "link_type": "external",
                 }
             )
             providers.insert(1, ("Local server", local_provider))
 
-        self.providers = DropdownExtended(
+        self.providers = ipw.Dropdown(
             options=providers,
-            disabled_options=invalid_providers,
+            # disabled_options=invalid_providers,
             layout=ipw.Layout(width="auto"),
         )
 
         self.show_child_dbs = ipw.Layout(width="auto", display="none")
-        self.child_dbs = DropdownExtended(
-            grouping=self.INITIAL_CHILD_DBS, layout=self.show_child_dbs
-        )
+        self.child_dbs = ipw.Dropdown(layout=self.show_child_dbs)
         self.page_chooser = ResultsPageChooser(
             page_limit=self.child_db_limit, layout=self.show_child_dbs
         )
 
         self.providers.observe(self._observe_providers, names="value")
         self.child_dbs.observe(self._observe_child_dbs, names="value")
         self.page_chooser.observe(
@@ -142,51 +133,60 @@
         self.offset = 0
         self.number = 1
 
         self.providers.disabled = False
         self.providers.index = 0
 
         self.show_child_dbs.display = "none"
-        self.child_dbs.grouping = self.INITIAL_CHILD_DBS
+        self.child_dbs.options = self.INITIAL_CHILD_DBS
 
     def _observe_providers(self, change: dict):
         """Update child database dropdown upon changing provider"""
-        value = change["new"]
-        self.show_child_dbs.display = "none"
-        self.provider = value
-        if value is None or not value:
+        try:
+            value = change["new"]
             self.show_child_dbs.display = "none"
-            self.child_dbs.grouping = self.INITIAL_CHILD_DBS
-            self.providers.index = 0
-            self.child_dbs.index = 0
-        else:
-            self._initialize_child_dbs()
-            if sum([len(_[1]) for _ in self.child_dbs.grouping]) <= 2:
-                # The provider either has 0 or 1 implementations
-                # or we have failed to retrieve any implementations.
-                # Automatically choose the 1 implementation (if there),
-                # while otherwise keeping the dropdown disabled.
+            self.provider = value
+            if value is None or not value:
                 self.show_child_dbs.display = "none"
-                try:
-                    self.child_dbs.index = 1
-                    LOGGER.debug(
-                        "Changed child_dbs index. New child_dbs: %s", self.child_dbs
-                    )
-                except IndexError:
-                    pass
+                self.child_dbs.options = self.INITIAL_CHILD_DBS
+                self.providers.index = 0
+                self.child_dbs.index = 0
             else:
-                self.show_child_dbs.display = None
+                self._initialize_child_dbs()
+                self.child_dbs.index = 0
+                if len(self.child_dbs.options) <= 2:
+                    # The provider either has 0 or 1 implementations
+                    # or we have failed to retrieve any implementations.
+                    # Automatically choose the 1 implementation (if there),
+                    # while otherwise keeping the dropdown disabled.
+                    self.show_child_dbs.display = "none"
+                    try:
+                        self.child_dbs.index = 1
+                        LOGGER.debug(
+                            "Changed child_dbs index. New child_dbs: %s", self.child_dbs
+                        )
+                    except IndexError:
+                        pass
+                else:
+                    self.show_child_dbs.display = None
+        except Exception as e:
+            # Without this, errors in callbacks don't seem to be logged/displayed
+            LOGGER.error(str(e), exc_info=True)
 
     def _observe_child_dbs(self, change: dict):
         """Update database traitlet with base URL for chosen child database"""
-        value = change["new"]
-        if value is None or not value:
-            self.database = "", None
-        else:
-            self.database = self.child_dbs.label.strip(), self.child_dbs.value
+        try:
+            value = change["new"]
+            if value is None or not value:
+                self.database = "", None
+            else:
+                self.database = self.child_dbs.label.strip(), self.child_dbs.value
+        except Exception as e:
+            # Without this, errors in callbacks don't seem to be logged/displayed
+            LOGGER.error(str(e), exc_info=True)
 
     @staticmethod
     def _remove_current_dropdown_option(dropdown: ipw.Dropdown) -> tuple:
         """Remove the current option from a Dropdown widget and return updated options
 
         Since Dropdown.options is a tuple there is a need to go through a list.
         """
@@ -282,43 +282,39 @@
                 LOGGER.debug(
                     "Remove target: %r. Will NOT remove target at %r: %r",
                     exc.remove_target,
                     self.providers.index,
                     self.providers.value,
                 )
                 self.show_child_dbs.display = "none"
-                self.child_dbs.grouping = self.INITIAL_CHILD_DBS
+                self.child_dbs.options = self.INITIAL_CHILD_DBS
 
         else:
             self.unfreeze()
 
     def _set_child_dbs(
         self,
         data: List[Tuple[str, List[Tuple[str, LinksResourceAttributes]]]],
     ) -> None:
         """Update the child_dbs options with `data`"""
         first_choice = (
             self.HINT["child_dbs"] if data else "No valid implementations found"
         )
         new_data = list(data)
-        new_data.insert(0, ("", [(first_choice, None)]))
-        self.child_dbs.grouping = new_data
+        new_data.insert(0, (first_choice, None))
+        self.child_dbs.options = new_data
 
     def _update_child_dbs(
         self, data: List[dict], skip_dbs: List[str] = None
     ) -> Tuple[
         List[str],
         List[List[Union[str, List[Tuple[str, LinksResourceAttributes]]]]],
     ]:
         """Update child DB dropdown from response data"""
-        child_dbs = (
-            {"": []}
-            if self.providers.label not in self.child_db_groupings
-            else deepcopy(self.child_db_groupings[self.providers.label])
-        )
+        child_dbs = []
         exclude_dbs = []
         skip_dbs = skip_dbs or []
 
         for entry in data:
             child_db = update_old_links_resources(entry)
             if child_db is None:
                 continue
@@ -359,32 +355,15 @@
                     "Skip %s: Could not determine versioned base URL for child DB: %r",
                     attributes.name,
                     child_db,
                 )
                 exclude_dbs.append(child_db.id)
                 continue
 
-            if self.providers.label in self.child_db_groupings:
-                for group, ids in self.child_db_groupings[self.providers.label].items():
-                    if child_db.id in ids:
-                        index = child_dbs[group].index(child_db.id)
-                        child_dbs[group][index] = (attributes.name, attributes)
-                        break
-                else:
-                    if "" in child_dbs:
-                        child_dbs[""].append((attributes.name, attributes))
-                    else:
-                        child_dbs[""] = [(attributes.name, attributes)]
-            else:
-                child_dbs[""].append((attributes.name, attributes))
-
-        if self.providers.label in self.child_db_groupings:
-            for group, ids in tuple(child_dbs.items()):
-                child_dbs[group] = [_ for _ in ids if isinstance(_, tuple)]
-        child_dbs = list(child_dbs.items())
+            child_dbs.append((attributes.name, attributes))
 
         LOGGER.debug("Final updated child_dbs: %s", child_dbs)
 
         return exclude_dbs, child_dbs
 
     def _get_more_child_dbs(self, change):
         """Query for more child DBs according to page_offset"""
@@ -482,15 +461,15 @@
                 LOGGER.debug(
                     "Remove target: %r. Will NOT remove target at %r: %r",
                     exc.remove_target,
                     self.providers.index,
                     self.providers.value,
                 )
                 self.show_child_dbs.display = "none"
-                self.child_dbs.grouping = self.INITIAL_CHILD_DBS
+                self.child_dbs.options = self.INITIAL_CHILD_DBS
 
         else:
             self.unfreeze()
 
     def _query(  # pylint: disable=too-many-locals,too-many-branches,too-many-statements
         self, link: str = None, exclude_ids: List[str] = None
     ) -> Tuple[List[dict], dict, int, int]:
```

### Comparing `ipyoptimade-0.2.0/src/ipyoptimade/subwidgets/results.py` & `ipyoptimade-1.0.0a0/src/ipyoptimade/subwidgets/results.py`

 * *Files identical despite different names*

### Comparing `ipyoptimade-0.2.0/src/ipyoptimade/subwidgets/sort_selector.py` & `ipyoptimade-1.0.0a0/src/ipyoptimade/subwidgets/sort_selector.py`

 * *Files identical despite different names*

### Comparing `ipyoptimade-0.2.0/src/ipyoptimade/summary.py` & `ipyoptimade-1.0.0a0/src/ipyoptimade/summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import tempfile
 from typing import Union
 import warnings
 
 import ipywidgets as ipw
 import traitlets
 
-from ipywidgets_extended import DropdownExtended
 import nglview
 
 try:
     from ase import Atoms as aseAtoms
 except ImportError:
     aseAtoms = None
 
@@ -205,15 +204,15 @@
                 )
         else:
             self._button_style = ButtonStyle.DEFAULT
 
         self._initialize_options()
         options = self._formats
         options.insert(0, ("Select a format", {}))
-        self.dropdown = DropdownExtended(options=options, layout={"width": "auto"})
+        self.dropdown = ipw.Dropdown(options=options, layout={"width": "auto"})
         self.download_button = ipw.HTML(
             self._download_button_format.format(
                 button_style=self._button_style.value,
                 disabled="disabled",
                 encoding="",
                 data="",
                 filename="",
```

### Comparing `ipyoptimade-0.2.0/src/ipyoptimade/utils.py` & `ipyoptimade-1.0.0a0/src/ipyoptimade/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,32 @@
-from collections import OrderedDict
-from enum import Enum, EnumMeta
+import json
 import os
-from pathlib import Path
 import re
-from typing import Tuple, List, Union, Iterable
-from urllib.parse import urlencode, urlparse, urlunparse, parse_qs
-
-import json
+from collections import OrderedDict
+from enum import Enum, EnumMeta
 from json import JSONDecodeError
+from pathlib import Path
+from typing import Iterable, List, Tuple, Union
+from urllib.parse import parse_qs, urlencode, urlparse, urlunparse
 
 import appdirs
+import requests
 from cachecontrol import CacheControlAdapter
 from cachecontrol.caches.file_cache import FileCache
 from cachecontrol.heuristics import ExpiresAfter
-from pydantic import ValidationError, AnyUrl  # pylint: disable=no-name-in-module
-import requests
-
-from optimade.models import LinksResource, OptimadeError, Link, LinksResourceAttributes
+from optimade.models import Link, LinksResource, LinksResourceAttributes, OptimadeError
 from optimade.models.links import LinkType
+from pydantic import AnyUrl, ValidationError  # pylint: disable=no-name-in-module
 
 from ipyoptimade.exceptions import (
     ApiVersionError,
     InputError,
 )
 from ipyoptimade.logger import LOGGER
 
-
 # Supported OPTIMADE spec versions
 __optimade_version__ = [
     "1.1.0",
     "1.0.1",
     "1.0.0",
 ]
 
@@ -412,15 +409,15 @@
 
     Return formatted list of tuples to use with a dropdown-widget.
     """
     providers = fetch_providers()
     res = []
     invalid_providers = []
     disable_providers = disable_providers or []
-    skip_providers = skip_providers or ["exmpl", "optimade", "aiida"]
+    skip_providers = skip_providers or ["exmpl"]
 
     for entry in providers:
         provider = LinksResource(**entry)
 
         if provider.id in skip_providers:
             LOGGER.debug("Skipping provider: %s", provider)
             continue
@@ -477,15 +474,15 @@
                 "Could not determine versioned base URL for provider: %s", str(provider)
             )
             invalid_providers.append((attributes.name, attributes))
             continue
 
         res.append((attributes.name, attributes))
 
-    return res + invalid_providers, [name for name, _ in invalid_providers]
+    return res, [name for name, _ in invalid_providers]
 
 
 def validate_api_version(version: str, raise_on_fail: bool = True) -> str:
     """Given an OPTIMADE API version, validate it against current supported API version"""
     if not version:
         msg = (
             "No version found in response. "
```

### Comparing `ipyoptimade-0.2.0/src/ipyoptimade/warnings.py` & `ipyoptimade-1.0.0a0/src/ipyoptimade/warnings.py`

 * *Files identical despite different names*

### Comparing `ipyoptimade-0.2.0/PKG-INFO` & `ipyoptimade-1.0.0a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyoptimade
-Version: 0.2.0
+Version: 1.0.0a0
 Summary: Jupyter client for searching structures through OPTIMADE API
 Author-email: Casper Welzel Andersen <casper+github@welzel.nu>, Kristjan Eimre <kristan.eimre@epfl.ch>, Jusong Yu <jusong.yu@psi.ch>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AiiDA
 Classifier: Framework :: Jupyter
@@ -20,45 +20,52 @@
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Widget Sets
 Requires-Dist: appdirs~=1.4.4
 Requires-Dist: cachecontrol[filecache]~=0.13.1
-Requires-Dist: ipywidgets~=7.7
-Requires-Dist: ipywidgets-extended>=1.1.1,<2,!=1.2.0,!=1.2.1
+Requires-Dist: ipywidgets~=8.1
 Requires-Dist: nglview~=3.0
 Requires-Dist: optimade~=1.0.0
 Requires-Dist: ase~=3.22
 Requires-Dist: pandas~=2.1
 Requires-Dist: requests~=2.31
-Requires-Dist: widget_periodictable~=3.1
+Requires-Dist: widget_periodictable~=4.1
 Requires-Dist: semver~=3.0
 Requires-Dist: pre-commit~=3.6 ; extra == "dev"
 Requires-Dist: pytest~=7.4 ; extra == "dev"
 Requires-Dist: pytest-cov~=4.1 ; extra == "dev"
-Requires-Dist: bumpver~=2023.1129 ; extra == "dev"
-Requires-Dist: voila~=0.4.0 ; extra == "voila"
+Requires-Dist: bumpver>=2023.1129 ; extra == "dev"
+Requires-Dist: pip-tools~=7.4 ; extra == "dev"
+Requires-Dist: voila~=0.5.0 ; extra == "voila"
 Project-URL: Documentation, https://github.com/aiidalab/ipyoptimade#readme
 Project-URL: Source, https://github.com/aiidalab/ipyoptimade
 Project-URL: Tracker, https://github.com/aiidalab/ipyoptimade/issues
 Provides-Extra: dev
 Provides-Extra: voila
 
 # OPTIMADE Jupyter widgets and Voilà application
 
 [![MaterialsCloud](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/CasperWA/voila-optimade-client/develop/docs/resources/mcloud_badge.json)](https://materialscloud.org/optimadeclient/)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/aiidalab/ipyoptimade/main?urlpath=%2Fvoila%2Frender%2Foptimade-client.ipynb)
 [![codecov](https://codecov.io/gh/aiidalab/ipyoptimade/branch/main/graph/badge.svg)](https://codecov.io/gh/aiidalab/ipyoptimade)
+[![PyPI - Version](https://img.shields.io/pypi/v/ipyoptimade?color=4CC61E)](https://pypi.org/project/ipyoptimade/)
 
 Query for and import structures from [OPTIMADE](https://www.optimade.org) providers (COD, MaterialsCloud, NoMaD, Materials Project, ODBX, OQMD, and more ...).
 The package provides a Jupyter widget for querying OPTIMADE providers and an example Voilà application to stack widgets into an web application.
 
 Current supported OPTIMADE API versions: `1.1.0`, `1.0.0`, `1.0.0-rc.2`, `1.0.0-rc.1`, `0.10.1`
 
+Install with
+
+```bash
+pip install ipyoptimade
+```
+
 ## Run the client
 
 This Jupyter-based app is intended to run either:
 
 - In [AiiDAlab](https://aiidalab.materialscloud.org) as well as inside a [Quantum Mobile](https://materialscloud.org/work/quantum-mobile) Virtual Machine;
 - As a [MaterialsCloud tool](https://materialscloud.org/optimadeclient/);
 - As a standalone [MyBinder application](https://mybinder.org/v2/gh/CasperWA/voila-optimade-client/develop?urlpath=%2Fvoila%2Frender%2FOPTIMADE-Client.ipynb); or
@@ -157,49 +164,53 @@
 
 To see the full list of configurations you can call `voila` and pass `--help-all`.
 
 ### Running with "development" providers (Materials Cloud-specific)
 
 Set the environment variable `ipyoptimade_DEVELOPMENT_MODE` to `1` (the integer version for `True` (`1`) or `False` (`0`)) in order to force the use of development servers for providers (currently only relevant for Materials Cloud).
 
-## Contribute
-
-If you wish to contribute to the application, you can install it in "editable" mode by using the `-e` flag: `pip install -e .[dev]`.
-It is recommended that you use the GitHub-route mentioned above.
+## Development
 
-You should also install `pre-commit` in the cloned git repository by running:
+Install with
 
-```shell
+```bash
+pip install -e .[dev]
 pre-commit install
 ```
 
-To start making contributions, fork the repository and create PRs.
+Set
+
+```
+export ipyoptimade_DEBUG=1
+```
 
+to automatically open and show the debug & error messages in the `OptimadeLog()` widget.
 
-## For maintainers
+### Making a new release
 
 To create a new release, clone the repository, install development dependencies with `pip install -e '.[dev]'`, and then execute `bumpver update [--major|--minor|--patch] [--tag-num --tag [alpha|beta|rc]]`.
 This will:
 
-  1. Create a tagged release with bumped version and push it to the repository.
-  2. Trigger a GitHub actions workflow that creates a GitHub release and publishes it on PyPI.
+1. Create a tagged release with bumped version and push it to the repository.
+2. Trigger a GitHub actions workflow that creates a GitHub release and publishes it on PyPI.
 
 Additional notes:
 
-  - Use the `--dry` option to preview the release change.
-  - The release tag (e.g. a/b/rc) is determined from the last release.
-    Use the `--tag` option to switch the release tag.
-  - This package follows [semantic versioning](https://semver.org/).
+- Use the `--dry` option to preview the release change.
+- The release tag (e.g. a/b/rc) is determined from the last release.
+  Use the `--tag` option to switch the release tag.
+- This package follows [semantic versioning](https://semver.org/).
 
 ## License
 
 MIT. The terms of the license can be found in the [LICENSE](LICENSE) file.
 
 ## Acknowledgements
 
+<!-- prettier-ignore -->
 | | |
 |---|---|
 | [![BIG-MAP](https://avatars1.githubusercontent.com/u/72801303?s=200&v=4)](https://www.big-map.eu/) | [BIG-MAP](https://www.big-map.eu/); This project has received funding from the European Union’s Horizon 2020 research and innovation programme under grant agreement No 957189. The project is part of [BATTERY 2030+](https://battery2030.eu/), the large-scale European research initiative for inventing the sustainable batteries of the future. |
 
 ## Contact
 
 casper+github@welzel.nu
```

