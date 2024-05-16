# Comparing `tmp/ibek-3.4.0b2.tar.gz` & `tmp/ibek-3.5.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibek-3.4.0b2.tar", last modified: Mon Mar 25 12:55:57 2024, max compression
+gzip compressed data, was "ibek-3.5.0b1.tar", last modified: Tue May 14 16:09:22 2024, max compression
```

## Comparing `ibek-3.4.0b2.tar` & `ibek-3.5.0b1.tar`

### file list

```diff
@@ -1,169 +1,203 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.596970 ibek-3.4.0b2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.576970 ibek-3.4.0b2/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-03-25 12:55:52.000000 ibek-3.4.0b2/.devcontainer/devcontainer.json
--rwxr-xr-x   0 runner    (1001) docker     (127)      537 2024-03-25 12:55:52.000000 ibek-3.4.0b2/.devcontainer/local_build.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.576970 ibek-3.4.0b2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-03-25 12:55:52.000000 ibek-3.4.0b2/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.568970 ibek-3.4.0b2/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.576970 ibek-3.4.0b2/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-03-25 12:55:52.000000 ibek-3.4.0b2/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-03-25 12:55:52.000000 ibek-3.4.0b2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.576970 ibek-3.4.0b2/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-25 12:55:52.000000 ibek-3.4.0b2/.github/pages/index.html
--rwxr-xr-x   0 runner    (1001) docker     (127)     3041 2024-03-25 12:55:52.000000 ibek-3.4.0b2/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.576970 ibek-3.4.0b2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-03-25 12:55:52.000000 ibek-3.4.0b2/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-03-25 12:55:52.000000 ibek-3.4.0b2/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-03-25 12:55:52.000000 ibek-3.4.0b2/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-25 12:55:52.000000 ibek-3.4.0b2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:52.000000 ibek-3.4.0b2/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-25 12:55:52.000000 ibek-3.4.0b2/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.576970 ibek-3.4.0b2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-03-25 12:55:52.000000 ibek-3.4.0b2/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-03-25 12:55:52.000000 ibek-3.4.0b2/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-03-25 12:55:52.000000 ibek-3.4.0b2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-03-25 12:55:52.000000 ibek-3.4.0b2/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-03-25 12:55:52.000000 ibek-3.4.0b2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-03-25 12:55:52.000000 ibek-3.4.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    20089 2024-03-25 12:55:57.596970 ibek-3.4.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5784 2024-03-25 12:55:52.000000 ibek-3.4.0b2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-03-25 12:55:52.000000 ibek-3.4.0b2/builder2ibek.README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)    19288 2024-03-25 12:55:52.000000 ibek-3.4.0b2/builder2ibek.support.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.576970 ibek-3.4.0b2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6527 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.576970 ibek-3.4.0b2/docs/developer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.576970 ibek-3.4.0b2/docs/developer/explanations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.580970 ibek-3.4.0b2/docs/developer/explanations/decisions/
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/developer/explanations/decisions.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/developer/explanations/entities.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.580970 ibek-3.4.0b2/docs/developer/how-to/
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/developer/how-to/build-docs.rst
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/developer/how-to/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/developer/how-to/lint.rst
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/developer/how-to/make-release.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/developer/how-to/pin-requirements.rst
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/developer/how-to/run-tests.rst
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/developer/how-to/static-analysis.rst
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/developer/how-to/test-container.rst
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/developer/how-to/update-tools.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/developer/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.580970 ibek-3.4.0b2/docs/developer/reference/
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/developer/reference/standards.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.580970 ibek-3.4.0b2/docs/developer/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/developer/tutorials/dev-install.rst
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/genindex.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.580970 ibek-3.4.0b2/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)     9460 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/images/ibek-arch.svg
--rw-r--r--   0 runner    (1001) docker     (127)    14318 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/images/ibek-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     9125 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/images/ibek-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.580970 ibek-3.4.0b2/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.580970 ibek-3.4.0b2/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/user/explanations/docs-structure.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.580970 ibek-3.4.0b2/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/user/how-to/edit-yaml.rst
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/user/how-to/run-container.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.580970 ibek-3.4.0b2/docs/user/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/user/reference/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/user/reference/naming.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.580970 ibek-3.4.0b2/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-03-25 12:55:52.000000 ibek-3.4.0b2/docs/user/tutorials/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.580970 ibek-3.4.0b2/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-03-25 12:55:52.000000 ibek-3.4.0b2/examples/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-03-25 12:55:52.000000 ibek-3.4.0b2/examples/test_refs1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.584970 ibek-3.4.0b2/examples/yaml/
--rwxr-xr-x   0 runner    (1001) docker     (127)      514 2024-03-25 12:55:52.000000 ibek-3.4.0b2/examples/yaml/test-ibek.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-03-25 12:55:52.000000 ibek-3.4.0b2/examples/yaml/test.ibek.ioc.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-25 12:55:52.000000 ibek-3.4.0b2/examples/yaml/test.ibek.ioc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-25 12:55:52.000000 ibek-3.4.0b2/examples/yaml/test.ibek.support.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-03-25 12:55:52.000000 ibek-3.4.0b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 12:55:57.596970 ibek-3.4.0b2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.572970 ibek-3.4.0b2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.584970 ibek-3.4.0b2/src/ibek/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-25 12:55:57.000000 ibek-3.4.0b2/src/ibek/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.584970 ibek-3.4.0b2/src/ibek/dev_cmds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/dev_cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/dev_cmds/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/gen_scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/ioc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.588970 ibek-3.4.0b2/src/ibek/ioc_cmds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/ioc_cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/ioc_cmds/assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/ioc_cmds/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/ioc_cmds/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/render.py
--rw-r--r--   0 runner    (1001) docker     (127)     4987 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/render_db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.588970 ibek-3.4.0b2/src/ibek/runtime_cmds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/runtime_cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/runtime_cmds/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     6860 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/support.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.588970 ibek-3.4.0b2/src/ibek/support_cmds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/support_cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/support_cmds/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/support_cmds/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/support_cmds/files.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.588970 ibek-3.4.0b2/src/ibek/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/templates/ioc.subst.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/templates/st.cmd.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.588970 ibek-3.4.0b2/src/ibek/templates/support/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/templates/support/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.588970 ibek-3.4.0b2/src/ibek/templates/support/configure/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/templates/support/configure/RELEASE
--rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-03-25 12:55:52.000000 ibek-3.4.0b2/src/ibek/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.596970 ibek-3.4.0b2/src/ibek.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20089 2024-03-25 12:55:57.000000 ibek-3.4.0b2/src/ibek.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-03-25 12:55:57.000000 ibek-3.4.0b2/src/ibek.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 12:55:57.000000 ibek-3.4.0b2/src/ibek.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-25 12:55:57.000000 ibek-3.4.0b2/src/ibek.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-25 12:55:57.000000 ibek-3.4.0b2/src/ibek.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-25 12:55:57.000000 ibek-3.4.0b2/src/ibek.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.588970 ibek-3.4.0b2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/conftest.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1760 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/generate_samples.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.572970 ibek-3.4.0b2/tests/samples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.572970 ibek-3.4.0b2/tests/samples/epics/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.592970 ibek-3.4.0b2/tests/samples/epics/pvi-defs/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/epics/pvi-defs/simple.pvi.device.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.592970 ibek-3.4.0b2/tests/samples/iocs/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/iocs/bad_counter.ibek.ioc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/iocs/bad_counter2.ibek.ioc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/iocs/bad_db.ibek.ioc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/iocs/bad_default.ibek.ioc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/iocs/bad_ref.ibek.ioc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/iocs/ibek-mo-ioc-01.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/iocs/utils.ibek.ioc.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.572970 ibek-3.4.0b2/tests/samples/outputs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.592970 ibek-3.4.0b2/tests/samples/outputs/motorSim/
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/outputs/motorSim/index.bob
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/outputs/motorSim/ioc.subst
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/outputs/motorSim/simple.pvi.bob
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/outputs/motorSim/simple.pvi.template
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/outputs/motorSim/st.cmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.592970 ibek-3.4.0b2/tests/samples/outputs/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/outputs/utils/index.bob
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/outputs/utils/ioc.subst
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/outputs/utils/st.cmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.592970 ibek-3.4.0b2/tests/samples/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    16310 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/schemas/ibek.support.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     9457 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/schemas/motorSim.ibek.ioc.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/schemas/single.ibek.ioc.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/schemas/utils.ibek.ioc.schema.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:55:57.596970 ibek-3.4.0b2/tests/samples/support/
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/support/asyn.ibek.support.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/support/bad_db.ibek.support.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/support/motorSim.ibek.support.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/support/simple.pvi.device.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/samples/support/utils.ibek.support.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)     2894 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/sys-test.sh
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/test_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/test_render.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/test_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-03-25 12:55:52.000000 ibek-3.4.0b2/tests/test_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.975936 ibek-3.5.0b1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.947936 ibek-3.5.0b1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-14 16:09:19.000000 ibek-3.5.0b1/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.943936 ibek-3.5.0b1/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.947936 ibek-3.5.0b1/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-14 16:09:19.000000 ibek-3.5.0b1/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-14 16:09:19.000000 ibek-3.5.0b1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.947936 ibek-3.5.0b1/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-14 16:09:19.000000 ibek-3.5.0b1/.github/pages/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3041 2024-05-14 16:09:19.000000 ibek-3.5.0b1/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.951936 ibek-3.5.0b1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-05-14 16:09:19.000000 ibek-3.5.0b1/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-05-14 16:09:19.000000 ibek-3.5.0b1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-14 16:09:19.000000 ibek-3.5.0b1/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-14 16:09:19.000000 ibek-3.5.0b1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:19.000000 ibek-3.5.0b1/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-14 16:09:19.000000 ibek-3.5.0b1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.951936 ibek-3.5.0b1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-14 16:09:19.000000 ibek-3.5.0b1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-14 16:09:19.000000 ibek-3.5.0b1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-14 16:09:19.000000 ibek-3.5.0b1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-14 16:09:19.000000 ibek-3.5.0b1/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-14 16:09:19.000000 ibek-3.5.0b1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-05-14 16:09:19.000000 ibek-3.5.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    20711 2024-05-14 16:09:22.975936 ibek-3.5.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-05-14 16:09:19.000000 ibek-3.5.0b1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.951936 ibek-3.5.0b1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6527 2024-05-14 16:09:19.000000 ibek-3.5.0b1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.951936 ibek-3.5.0b1/docs/developer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.951936 ibek-3.5.0b1/docs/developer/explanations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.951936 ibek-3.5.0b1/docs/developer/explanations/decisions/
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-14 16:09:19.000000 ibek-3.5.0b1/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-14 16:09:19.000000 ibek-3.5.0b1/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-14 16:09:19.000000 ibek-3.5.0b1/docs/developer/explanations/decisions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-05-14 16:09:19.000000 ibek-3.5.0b1/docs/developer/explanations/entities.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.955936 ibek-3.5.0b1/docs/developer/how-to/
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-14 16:09:19.000000 ibek-3.5.0b1/docs/developer/how-to/build-docs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-14 16:09:19.000000 ibek-3.5.0b1/docs/developer/how-to/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-14 16:09:19.000000 ibek-3.5.0b1/docs/developer/how-to/lint.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-14 16:09:19.000000 ibek-3.5.0b1/docs/developer/how-to/make-release.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-05-14 16:09:19.000000 ibek-3.5.0b1/docs/developer/how-to/pin-requirements.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-14 16:09:19.000000 ibek-3.5.0b1/docs/developer/how-to/run-tests.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-14 16:09:19.000000 ibek-3.5.0b1/docs/developer/how-to/static-analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-14 16:09:19.000000 ibek-3.5.0b1/docs/developer/how-to/test-container.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-14 16:09:19.000000 ibek-3.5.0b1/docs/developer/how-to/update-tools.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-14 16:09:19.000000 ibek-3.5.0b1/docs/developer/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.955936 ibek-3.5.0b1/docs/developer/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-14 16:09:19.000000 ibek-3.5.0b1/docs/developer/reference/standards.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.955936 ibek-3.5.0b1/docs/developer/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-14 16:09:19.000000 ibek-3.5.0b1/docs/developer/tutorials/dev-install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-14 16:09:19.000000 ibek-3.5.0b1/docs/genindex.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.955936 ibek-3.5.0b1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     9460 2024-05-14 16:09:19.000000 ibek-3.5.0b1/docs/images/ibek-arch.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    14318 2024-05-14 16:09:19.000000 ibek-3.5.0b1/docs/images/ibek-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     9125 2024-05-14 16:09:19.000000 ibek-3.5.0b1/docs/images/ibek-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-14 16:09:19.000000 ibek-3.5.0b1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.955936 ibek-3.5.0b1/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.955936 ibek-3.5.0b1/docs/user/explanations/
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-14 16:09:19.000000 ibek-3.5.0b1/docs/user/explanations/docs-structure.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.955936 ibek-3.5.0b1/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-14 16:09:19.000000 ibek-3.5.0b1/docs/user/how-to/edit-yaml.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-14 16:09:19.000000 ibek-3.5.0b1/docs/user/how-to/run-container.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-14 16:09:19.000000 ibek-3.5.0b1/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.955936 ibek-3.5.0b1/docs/user/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-14 16:09:19.000000 ibek-3.5.0b1/docs/user/reference/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-14 16:09:19.000000 ibek-3.5.0b1/docs/user/reference/naming.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.955936 ibek-3.5.0b1/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-14 16:09:19.000000 ibek-3.5.0b1/docs/user/tutorials/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.955936 ibek-3.5.0b1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-14 16:09:19.000000 ibek-3.5.0b1/examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-14 16:09:19.000000 ibek-3.5.0b1/examples/test_refs1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.955936 ibek-3.5.0b1/examples/yaml/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      514 2024-05-14 16:09:19.000000 ibek-3.5.0b1/examples/yaml/test-ibek.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-14 16:09:19.000000 ibek-3.5.0b1/examples/yaml/test.ibek.ioc.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-14 16:09:19.000000 ibek-3.5.0b1/examples/yaml/test.ibek.ioc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-14 16:09:19.000000 ibek-3.5.0b1/examples/yaml/test.ibek.support.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-05-14 16:09:19.000000 ibek-3.5.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 16:09:22.975936 ibek-3.5.0b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.943936 ibek-3.5.0b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.959936 ibek-3.5.0b1/src/ibek/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-14 16:09:19.000000 ibek-3.5.0b1/src/ibek/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-14 16:09:19.000000 ibek-3.5.0b1/src/ibek/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-14 16:09:22.000000 ibek-3.5.0b1/src/ibek/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-14 16:09:19.000000 ibek-3.5.0b1/src/ibek/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-14 16:09:19.000000 ibek-3.5.0b1/src/ibek/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-05-14 16:09:19.000000 ibek-3.5.0b1/src/ibek/definition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.959936 ibek-3.5.0b1/src/ibek/dev_cmds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:19.000000 ibek-3.5.0b1/src/ibek/dev_cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-14 16:09:19.000000 ibek-3.5.0b1/src/ibek/dev_cmds/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-05-14 16:09:19.000000 ibek-3.5.0b1/src/ibek/entity_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-14 16:09:19.000000 ibek-3.5.0b1/src/ibek/gen_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-05-14 16:09:19.000000 ibek-3.5.0b1/src/ibek/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-05-14 16:09:19.000000 ibek-3.5.0b1/src/ibek/ioc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.963936 ibek-3.5.0b1/src/ibek/ioc_cmds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:19.000000 ibek-3.5.0b1/src/ibek/ioc_cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-05-14 16:09:19.000000 ibek-3.5.0b1/src/ibek/ioc_cmds/assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-05-14 16:09:19.000000 ibek-3.5.0b1/src/ibek/ioc_cmds/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-14 16:09:19.000000 ibek-3.5.0b1/src/ibek/ioc_cmds/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-14 16:09:19.000000 ibek-3.5.0b1/src/ibek/ioc_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-05-14 16:09:19.000000 ibek-3.5.0b1/src/ibek/render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-05-14 16:09:19.000000 ibek-3.5.0b1/src/ibek/render_db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.963936 ibek-3.5.0b1/src/ibek/runtime_cmds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:19.000000 ibek-3.5.0b1/src/ibek/runtime_cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-05-14 16:09:19.000000 ibek-3.5.0b1/src/ibek/runtime_cmds/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-14 16:09:19.000000 ibek-3.5.0b1/src/ibek/sub_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-14 16:09:19.000000 ibek-3.5.0b1/src/ibek/support.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.963936 ibek-3.5.0b1/src/ibek/support_cmds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:19.000000 ibek-3.5.0b1/src/ibek/support_cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-05-14 16:09:19.000000 ibek-3.5.0b1/src/ibek/support_cmds/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10070 2024-05-14 16:09:19.000000 ibek-3.5.0b1/src/ibek/support_cmds/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-05-14 16:09:19.000000 ibek-3.5.0b1/src/ibek/support_cmds/files.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.963936 ibek-3.5.0b1/src/ibek/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-14 16:09:19.000000 ibek-3.5.0b1/src/ibek/templates/ioc.subst.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-14 16:09:19.000000 ibek-3.5.0b1/src/ibek/templates/st.cmd.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.963936 ibek-3.5.0b1/src/ibek/templates/support/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-14 16:09:19.000000 ibek-3.5.0b1/src/ibek/templates/support/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.963936 ibek-3.5.0b1/src/ibek/templates/support/configure/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-14 16:09:19.000000 ibek-3.5.0b1/src/ibek/templates/support/configure/RELEASE
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-05-14 16:09:19.000000 ibek-3.5.0b1/src/ibek/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.975936 ibek-3.5.0b1/src/ibek.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20711 2024-05-14 16:09:22.000000 ibek-3.5.0b1/src/ibek.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-05-14 16:09:22.000000 ibek-3.5.0b1/src/ibek.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 16:09:22.000000 ibek-3.5.0b1/src/ibek.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-14 16:09:22.000000 ibek-3.5.0b1/src/ibek.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-14 16:09:22.000000 ibek-3.5.0b1/src/ibek.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 16:09:22.000000 ibek-3.5.0b1/src/ibek.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.963936 ibek-3.5.0b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/conftest.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2875 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/generate_samples.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.947936 ibek-3.5.0b1/tests/samples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.947936 ibek-3.5.0b1/tests/samples/epics/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.967936 ibek-3.5.0b1/tests/samples/epics/pvi-defs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/epics/pvi-defs/NDPluginDriver.pvi.device.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11312 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/epics/pvi-defs/NDPluginStats.pvi.device.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6283 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/epics/pvi-defs/asynNDArrayDriver.pvi.device.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/epics/pvi-defs/simple.pvi.device.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.947936 ibek-3.5.0b1/tests/samples/epics/support/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.947936 ibek-3.5.0b1/tests/samples/epics/support/ADSimDetector/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.967936 ibek-3.5.0b1/tests/samples/epics/support/ADSimDetector/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/epics/support/ADSimDetector/db/.placeholder
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.967936 ibek-3.5.0b1/tests/samples/epics/support/configure/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/epics/support/configure/RELEASE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.967936 ibek-3.5.0b1/tests/samples/iocs/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/iocs/bad_counter.ibek.ioc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/iocs/bad_counter2.ibek.ioc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/iocs/bad_db.ibek.ioc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/iocs/bad_default.ibek.ioc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/iocs/bad_ref.ibek.ioc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/iocs/gauges.ibek.ioc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/iocs/ibek-mo-ioc-01.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/iocs/ipac-test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/iocs/quadem.ibek.ioc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/iocs/utils.ibek.ioc.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.947936 ibek-3.5.0b1/tests/samples/outputs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.967936 ibek-3.5.0b1/tests/samples/outputs/gauges/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/outputs/gauges/index.bob
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/outputs/gauges/ioc.subst
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/outputs/gauges/st.cmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.967936 ibek-3.5.0b1/tests/samples/outputs/ipac/
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/outputs/ipac/index.bob
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/outputs/ipac/ioc.subst
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/outputs/ipac/st.cmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.967936 ibek-3.5.0b1/tests/samples/outputs/motorSim/
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/outputs/motorSim/index.bob
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/outputs/motorSim/ioc.subst
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/outputs/motorSim/simple.pvi.bob
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/outputs/motorSim/simple.pvi.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/outputs/motorSim/st.cmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.971936 ibek-3.5.0b1/tests/samples/outputs/quadem/
+-rw-r--r--   0 runner    (1001) docker     (127)    92616 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/outputs/quadem/NDPluginStats.pvi.bob
+-rw-r--r--   0 runner    (1001) docker     (127)    41300 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/outputs/quadem/NDPluginStats.pvi.template
+-rw-r--r--   0 runner    (1001) docker     (127)     8631 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/outputs/quadem/index.bob
+-rw-r--r--   0 runner    (1001) docker     (127)     8624 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/outputs/quadem/ioc.subst
+-rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/outputs/quadem/st.cmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.971936 ibek-3.5.0b1/tests/samples/outputs/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/outputs/utils/index.bob
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/outputs/utils/ioc.subst
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/outputs/utils/st.cmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.971936 ibek-3.5.0b1/tests/samples/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     7030 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/schemas/gauges.ibek.ioc.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17581 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/schemas/ibek.support.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9469 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/schemas/motorSim.ibek.ioc.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)    86597 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/schemas/quadem.ibek.ioc.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5700 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/schemas/single.ibek.ioc.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/schemas/utils.ibek.ioc.schema.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:22.975936 ibek-3.5.0b1/tests/samples/support/
+-rw-r--r--   0 runner    (1001) docker     (127)    67566 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/support/ADCore.ibek.support.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/support/asyn.ibek.support.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/support/bad_db.ibek.support.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/support/epics.ibek.support.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/support/gauges.ibek.support.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/support/ipac.ibek.support.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/support/motorSim.ibek.support.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/support/quadem.ibek.support.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/support/simple.pvi.device.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/samples/support/utils.ibek.support.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2894 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/sys-test.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     7093 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/test_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/test_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-14 16:09:19.000000 ibek-3.5.0b1/tests/test_unit.py
```

### Comparing `ibek-3.4.0b2/.github/CONTRIBUTING.rst` & `ibek-3.5.0b1/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ibek-3.4.0b2/.github/actions/install_requirements/action.yml` & `ibek-3.5.0b1/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `ibek-3.4.0b2/.github/dependabot.yml` & `ibek-3.5.0b1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ibek-3.4.0b2/.github/pages/make_switcher.py` & `ibek-3.5.0b1/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `ibek-3.4.0b2/.github/workflows/code.yml` & `ibek-3.5.0b1/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `ibek-3.4.0b2/.github/workflows/docs.yml` & `ibek-3.5.0b1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `ibek-3.4.0b2/.github/workflows/docs_clean.yml` & `ibek-3.5.0b1/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `ibek-3.4.0b2/.gitignore` & `ibek-3.5.0b1/.gitignore`

 * *Files identical despite different names*

### Comparing `ibek-3.4.0b2/.vscode/launch.json` & `ibek-3.5.0b1/.vscode/launch.json`

 * *Files 18% similar despite different names*

```diff
@@ -10,15 +10,16 @@
             "name": "builder2ibek",
             "type": "python",
             "python": "/dls_sw/prod/tools/RHEL7-x86_64/defaults/bin/dls-python",
             "request": "launch",
             "program": "builder2ibek.support.py",
             "console": "integratedTerminal",
             "args": [
-                "/dls_sw/prod/R3.14.12.7/support/devIocStats/3-1-14dls3-3"
+                "/dls_sw/prod/R3.14.12.7/support/quadEM/9-4dls1",
+                "../quadEM.ibek.support.yaml"
             ],
             "justMyCode": false
         },
         {
             "name": "Debug example test",
             "type": "python",
             "request": "launch",
```

### Comparing `ibek-3.4.0b2/LICENSE` & `ibek-3.5.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `ibek-3.4.0b2/PKG-INFO` & `ibek-3.5.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibek
-Version: 3.4.0b2
+Version: 3.5.0b1
 Summary: IOC Builder for EPICS and Kubernetes
 Author-email: Tom Cobb <tom.cobb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -214,14 +214,15 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: pydantic==2.6.4
 Requires-Dist: typer
 Requires-Dist: ruamel.yaml
 Requires-Dist: jinja2
 Requires-Dist: GitPython
+Requires-Dist: semantic-version
 Requires-Dist: pvi~=0.8
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pipdeptree; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pydata-sphinx-theme>=0.12; extra == "dev"
@@ -251,14 +252,28 @@
   ============== ==============================================================
   PyPI           ``pip install ibek``
   Source code    https://github.com/epics-containers/ibek
   Documentation  https://epics-containers.github.io/ibek
   Releases       https://github.com/epics-containers/ibek/releases
   ============== ==============================================================
 
+UPDATE: Version 2.0.0
+=====================
+
+There have been a number of breaking changes since version 1.8.0. These are
+primarily to support RTEMS cross compiled IOCs. But we have also taken the
+opportunity to clarify the CLI.
+
+All changes are compatible with 2.0.0 of ibek-support and 3.4.0 of all other
+epics-containers repos. When using ioc-template 3.4.0 to update your generic
+IOCs, make sure you also update the ibek-support submodule to 2.0.0 or newer,
+then you should have all compatible versions.
+
+--------------------------------------------------------------------------------
+
 
 The documentation is still under construction. For the moment the best
 pages to read are the following:
 
 - `Modules, Definitions and Entities <https://epics-containers.github.io/ibek/main/developer/explanations/entities.html//>`_
   A description of the basic concepts of ibek.
```

### Comparing `ibek-3.4.0b2/README.rst` & `ibek-3.5.0b1/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,28 @@
   ============== ==============================================================
   PyPI           ``pip install ibek``
   Source code    https://github.com/epics-containers/ibek
   Documentation  https://epics-containers.github.io/ibek
   Releases       https://github.com/epics-containers/ibek/releases
   ============== ==============================================================
 
+UPDATE: Version 2.0.0
+=====================
+
+There have been a number of breaking changes since version 1.8.0. These are
+primarily to support RTEMS cross compiled IOCs. But we have also taken the
+opportunity to clarify the CLI.
+
+All changes are compatible with 2.0.0 of ibek-support and 3.4.0 of all other
+epics-containers repos. When using ioc-template 3.4.0 to update your generic
+IOCs, make sure you also update the ibek-support submodule to 2.0.0 or newer,
+then you should have all compatible versions.
+
+--------------------------------------------------------------------------------
+
 
 The documentation is still under construction. For the moment the best
 pages to read are the following:
 
 - `Modules, Definitions and Entities <https://epics-containers.github.io/ibek/main/developer/explanations/entities.html//>`_
   A description of the basic concepts of ibek.
```

### Comparing `ibek-3.4.0b2/docs/conf.py` & `ibek-3.5.0b1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ibek-3.4.0b2/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst` & `ibek-3.5.0b1/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst`

 * *Files identical despite different names*

### Comparing `ibek-3.4.0b2/docs/developer/explanations/decisions.rst` & `ibek-3.5.0b1/docs/developer/explanations/decisions.rst`

 * *Files identical despite different names*

### Comparing `ibek-3.4.0b2/docs/developer/explanations/entities.rst` & `ibek-3.5.0b1/docs/developer/explanations/entities.rst`

 * *Files identical despite different names*

### Comparing `ibek-3.4.0b2/docs/developer/how-to/build-docs.rst` & `ibek-3.5.0b1/docs/developer/how-to/build-docs.rst`

 * *Files identical despite different names*

### Comparing `ibek-3.4.0b2/docs/developer/how-to/lint.rst` & `ibek-3.5.0b1/docs/developer/how-to/lint.rst`

 * *Files identical despite different names*

### Comparing `ibek-3.4.0b2/docs/developer/how-to/make-release.rst` & `ibek-3.5.0b1/docs/developer/how-to/make-release.rst`

 * *Files identical despite different names*

### Comparing `ibek-3.4.0b2/docs/developer/how-to/pin-requirements.rst` & `ibek-3.5.0b1/docs/developer/how-to/pin-requirements.rst`

 * *Files identical despite different names*

### Comparing `ibek-3.4.0b2/docs/developer/how-to/test-container.rst` & `ibek-3.5.0b1/docs/developer/how-to/test-container.rst`

 * *Files identical despite different names*

### Comparing `ibek-3.4.0b2/docs/developer/how-to/update-tools.rst` & `ibek-3.5.0b1/docs/developer/how-to/update-tools.rst`

 * *Files identical despite different names*

### Comparing `ibek-3.4.0b2/docs/developer/index.rst` & `ibek-3.5.0b1/docs/developer/index.rst`

 * *Files identical despite different names*

### Comparing `ibek-3.4.0b2/docs/developer/reference/standards.rst` & `ibek-3.5.0b1/docs/developer/reference/standards.rst`

 * *Files identical despite different names*

### Comparing `ibek-3.4.0b2/docs/developer/tutorials/dev-install.rst` & `ibek-3.5.0b1/docs/developer/tutorials/dev-install.rst`

 * *Files identical despite different names*

### Comparing `ibek-3.4.0b2/docs/images/ibek-arch.svg` & `ibek-3.5.0b1/docs/images/ibek-arch.svg`

 * *Files identical despite different names*

### Comparing `ibek-3.4.0b2/docs/images/ibek-favicon.ico` & `ibek-3.5.0b1/docs/images/ibek-favicon.ico`

 * *Files identical despite different names*

### Comparing `ibek-3.4.0b2/docs/images/ibek-logo.svg` & `ibek-3.5.0b1/docs/images/ibek-logo.svg`

 * *Files identical despite different names*

### Comparing `ibek-3.4.0b2/docs/index.rst` & `ibek-3.5.0b1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ibek-3.4.0b2/docs/user/explanations/docs-structure.rst` & `ibek-3.5.0b1/docs/user/explanations/docs-structure.rst`

 * *Files identical despite different names*

### Comparing `ibek-3.4.0b2/docs/user/index.rst` & `ibek-3.5.0b1/docs/user/index.rst`

 * *Files identical despite different names*

### Comparing `ibek-3.4.0b2/docs/user/reference/api.rst` & `ibek-3.5.0b1/docs/user/reference/api.rst`

 * *Files identical despite different names*

### Comparing `ibek-3.4.0b2/docs/user/reference/naming.rst` & `ibek-3.5.0b1/docs/user/reference/naming.rst`

 * *Files identical despite different names*

### Comparing `ibek-3.4.0b2/docs/user/tutorials/installation.rst` & `ibek-3.5.0b1/docs/user/tutorials/installation.rst`

 * *Files identical despite different names*

### Comparing `ibek-3.4.0b2/examples/README.md` & `ibek-3.5.0b1/examples/README.md`

 * *Files identical despite different names*

### Comparing `ibek-3.4.0b2/examples/test_refs1.py` & `ibek-3.5.0b1/examples/test_refs1.py`

 * *Files identical despite different names*

### Comparing `ibek-3.4.0b2/examples/yaml/test-ibek.sh` & `ibek-3.5.0b1/examples/yaml/test-ibek.sh`

 * *Files identical despite different names*

### Comparing `ibek-3.4.0b2/examples/yaml/test.ibek.ioc.schema.json` & `ibek-3.5.0b1/examples/yaml/test.ibek.ioc.schema.json`

 * *Files identical despite different names*

### Comparing `ibek-3.4.0b2/examples/yaml/test.ibek.support.yaml` & `ibek-3.5.0b1/examples/yaml/test.ibek.support.yaml`

 * *Files identical despite different names*

### Comparing `ibek-3.4.0b2/pyproject.toml` & `ibek-3.5.0b1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 description = "IOC Builder for EPICS and Kubernetes"
 dependencies = [
     "pydantic==2.6.4",
     "typer",
     "ruamel.yaml",
     "jinja2",
     "GitPython",
-    "pvi~=0.8",  # pvi currently tracks breaking changes with minor version
+    "semantic-version",
+    "pvi~=0.8",         # pvi currently tracks breaking changes with minor version
 ] # Add project dependencies here, e.g. ["click", "numpy"]
 dynamic = ["version"]
 license.file = "LICENSE"
 readme = "README.rst"
 requires-python = ">=3.10"
 
 [project.optional-dependencies]
@@ -105,27 +106,27 @@
     pre-commit: pre-commit run --all-files {posargs}
     docs: sphinx-{posargs:build -EW --keep-going} -T docs build/html
 """
 
 
 [tool.ruff]
 src = ["src", "tests"]
-ignore = [
+lint.ignore = [
     "C408", # Unnecessary collection call - e.g. list(...) instead of [...]
     "E501", # Line too long, should be fixed by black.
 ]
 line-length = 88
-select = [
+lint.select = [
     "C4",   # flake8-comprehensions - https://beta.ruff.rs/docs/rules/#flake8-comprehensions-c4
     "E",    # pycodestyle errors - https://beta.ruff.rs/docs/rules/#error-e
     "F",    # pyflakes rules - https://beta.ruff.rs/docs/rules/#pyflakes-f
     "W",    # pycodestyle warnings - https://beta.ruff.rs/docs/rules/#warning-w
     "I001", # isort
 ]
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "builder2ibek.support.py" = ["E402"]
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools.package-data]
 "ibek.templates" = ["**/*"]
```

### Comparing `ibek-3.4.0b2/src/ibek/__main__.py` & `ibek-3.5.0b1/src/ibek/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Optional
 
 import typer
 from ruamel.yaml import YAML
 
 from ibek._version import __version__
+from ibek.commands import semver_compare
 from ibek.dev_cmds.commands import dev_cli
 from ibek.globals import NaturalOrderGroup
 from ibek.ioc_cmds.commands import ioc_cli
 from ibek.runtime_cmds.commands import runtime_cli
 from ibek.support_cmds.commands import support_cli
 
 cli = typer.Typer(cls=NaturalOrderGroup)
@@ -55,11 +56,29 @@
     """IOC Builder for EPICS and Kubernetes
 
     Provides support for building generic EPICS IOC container images and for
     running IOC instances in a Kubernetes cluster.
     """
 
 
+@cli.command()
+def compare(
+    base: str = typer.Argument(
+        help='SemVer string e.g. "1.2.0"',
+    ),
+    target: str = typer.Argument(
+        help='An operator (<=,>=,==,<,>) followed by a SemVer string e.g.">=1.2.0"',
+    ),
+):
+    """
+    Compare two SemVer strings similarly to pip's requirements specifier syntax
+    """
+    if semver_compare(base, target):
+        raise typer.Exit(code=0)
+    else:
+        raise typer.Exit(code=1)
+
+
 # test with:
 #     pipenv run python -m ibek
 if __name__ == "__main__":
     cli()
```

### Comparing `ibek-3.4.0b2/src/ibek/dev_cmds/commands.py` & `ibek-3.5.0b1/src/ibek/dev_cmds/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import shutil
 from pathlib import Path
 
 import typer
 
-from ibek.globals import CONFIG_DIR_NAME, IOC_FOLDER, NaturalOrderGroup
+from ibek.globals import GLOBALS, NaturalOrderGroup
 
 log = logging.getLogger(__name__)
 dev_cli = typer.Typer(cls=NaturalOrderGroup)
 
 
 @dev_cli.command()
 def instance(
@@ -30,17 +30,17 @@
     available and also under version control.
 
     e.g. if instance is /workspaces/bl38p/iocs/bl38p-mo-panda-01 then we need:
     - /epics/ioc/config -> /workspaces/bl38p/iocs/bl38p-mo-panda-01/config
     """
 
     # validate the instance folder has a config folder
-    ioc_folder = IOC_FOLDER
-    config_folder = ioc_folder / CONFIG_DIR_NAME
-    instance_config = instance / CONFIG_DIR_NAME
+    ioc_folder = GLOBALS.IOC_FOLDER
+    config_folder = ioc_folder / GLOBALS.CONFIG_DIR_NAME
+    instance_config = instance / GLOBALS.CONFIG_DIR_NAME
 
     # verify that the expected folder exists
     if not ioc_folder.exists():
         log.error(f"Could not find ioc folder {ioc_folder}")
         raise typer.Exit(1)
 
     # remove any existing config folder from /epics/ioc
```

### Comparing `ibek-3.4.0b2/src/ibek/ioc.py` & `ibek-3.5.0b1/src/ibek/entity_factory.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,200 +1,177 @@
 """
-Functions for generating an IocInstance derived class from a
-support module definition YAML file
+A class for constructing Entity classes from Definitions
 """
 
 from __future__ import annotations
 
 import builtins
-from enum import Enum
-from typing import Annotated, Any, Dict, Literal, Sequence, Tuple, Type, Union
+from pathlib import Path
+from typing import Any, Dict, List, Literal, Tuple, Type
 
-from pydantic import (
-    Field,
-    create_model,
-    field_validator,
-    model_validator,
-)
+from pydantic import create_model, field_validator
 from pydantic.fields import FieldInfo
 from pydantic_core import PydanticUndefined
+from ruamel.yaml.main import YAML
 
-from .globals import BaseSettings
-from .support import Definition, EnumArg, IdArg, ObjectArg, Support
+from .args import EnumArg, IdArg, ObjectArg
+from .ioc import Entity, EnumVal, clear_entity_model_ids, get_entity_by_id
+from .support import EntityDefinition, Support
 from .utils import UTILS
 
-id_to_entity: Dict[str, Entity] = {}
 
-
-class EnumVal(Enum):
-    """
-    An enum that is printed as its name only
-    """
-
-    def __str__(self):
-        return self.name
-
-
-class Entity(BaseSettings):
-    """
-    A baseclass for all generated Entity classes.
-    """
-
-    type: str = Field(description="The type of this entity")
-    entity_enabled: bool = Field(
-        description="enable or disable this entity instance", default=True
-    )
-    __definition__: Definition
-
-    @model_validator(mode="after")  # type: ignore
-    def add_ibek_attributes(cls, entity: Entity):
+class EntityFactory:
+    def __init__(self) -> None:
         """
-        Whole Entity model validation
+        EntityFactory tracks all the Entity Models created in self._entity_classes
         """
+        self._entity_models: Dict[str, Type[Entity]] = {}
+        # starting a new EntityFactory implies we should throw away any existing
+        # Entity instances - this is required for tests which create multiple
+        # EntityFactories
+        clear_entity_model_ids()
 
-        # find the id field in this Entity if it has one
-        ids = {a.name for a in entity.__definition__.args if isinstance(a, IdArg)}
-
-        entity_dict = entity.model_dump()
-        for arg, value in entity_dict.items():
-            if arg in ids:
-                # add this entity to the global id index
-                if value in id_to_entity:
-                    raise ValueError(f"Duplicate id {value} in {list(id_to_entity)}")
-                id_to_entity[value] = entity
-            elif isinstance(value, str):
-                # Jinja expansion of any of the Entity's string args/values
-                setattr(entity, arg, UTILS.render(entity_dict, value))
-        return entity
-
-    def __str__(self):
-        # if this entity has an id then its string representation is the value of id
-        id_name = self.__definition__._get_id_arg()
-        return getattr(self, id_name) if id_name else super().__str__()
-
-
-def make_entity_model(definition: Definition, support: Support) -> Type[Entity]:
-    """
-    Create an Entity Model from a Definition instance and a Support instance.
-    """
-
-    def add_arg(name, typ, description, default):
-        if default is None:
-            default = PydanticUndefined
-        args[name] = (
-            typ,
-            FieldInfo(description=description, default=default),
-        )
-
-    args: Dict[str, Tuple[type, Any]] = {}
-    validators: Dict[str, Any] = {}
-
-    # fully qualified name of the Entity class including support module
-    full_name = f"{support.module}.{definition.name}"
-
-    # add in each of the arguments as a Field in the Entity
-    for arg in definition.args:
-        full_arg_name = f"{full_name}.{arg.name}"
-        arg_type: Any
-
-        if isinstance(arg, ObjectArg):
-
-            @field_validator(arg.name, mode="after")
-            def lookup_instance(cls, id):
-                try:
-                    return id_to_entity[id]
-                except KeyError:
-                    raise ValueError(f"object {id} not found in {list(id_to_entity)}")
-
-            validators[full_arg_name] = lookup_instance
-            arg_type = object
-
-        elif isinstance(arg, IdArg):
-            arg_type = str
-
-        elif isinstance(arg, EnumArg):
-            # Pydantic uses the values of the Enum as the options in the schema.
-            # Here we arrange for the keys to be in the schema (what a user supplies)
-            # but the values to be what is rendered when jinja refers to the enum
-            enum_swapped = {}
-            for k, v in arg.values.items():
-                enum_swapped[str(v) if v else str(k)] = k
-            val_enum = EnumVal(arg.name, enum_swapped)  # type: ignore
-            arg_type = val_enum
-
-        else:
-            # arg.type is str, int, float, etc.
-            arg_type = getattr(builtins, arg.type)
-        default = getattr(arg, "default", None)
-        add_arg(arg.name, arg_type, arg.description, default)
-
-    # add in the calculated values Jinja Templates as Fields in the Entity
-    for value in definition.values:
-        add_arg(value.name, str, value.description, value.value)
-
-    # add the type literal which discriminates between the different Entity classes
-    typ = Literal[full_name]  # type: ignore
-    add_arg("type", typ, "The type of this entity", full_name)
-
-    entity_cls = create_model(
-        full_name.replace(".", "_"),
-        **args,
-        __validators__=validators,
-        __base__=Entity,
-    )  # type: ignore
-
-    # add a link back to the Definition Instance that generated this Entity Class
-    entity_cls.__definition__ = definition
-
-    return entity_cls
+    def make_entity_models(self, definition_yaml: List[Path]) -> List[Type[Entity]]:
+        """
+        Read a set of *.ibek.support.yaml files and generate Entity classes
+        from their Definition entries
+        """
 
+        for definition in definition_yaml:
+            support_dict = YAML(typ="safe").load(definition)
 
-def make_entity_models(support: Support):
-    """
-    Create Entity subclasses for all Definition instances in the given
-    Support instance. Returns a list of the Entity subclasses Models.
-    """
+            Support.model_validate(support_dict)
 
-    entity_models = []
-    entity_names = []
+            # deserialize the support module definition file
+            support = Support(**support_dict)
+            # make Entity classes described in the support module definition file
+            self._make_entity_models(support)
 
-    for definition in support.defs:
-        entity_models.append(make_entity_model(definition, support))
-        if definition.name in entity_names:
-            # not tested because schema validation will always catch this first
-            raise ValueError(f"Duplicate entity name {definition.name}")
-        entity_names.append(definition.name)
+        return list(self._entity_models.values())
 
-    return entity_models
+    def _make_entity_model(
+        self, definition: EntityDefinition, support: Support
+    ) -> Type[Entity]:
+        """
+        Create an Entity Model from a Definition instance and a Support instance.
+        """
 
+        def add_arg(name, typ, description, default):
+            if default is None:
+                default = PydanticUndefined
+            args[name] = (
+                typ,
+                FieldInfo(description=description, default=default),
+            )
+
+        args: Dict[str, Tuple[type, Any]] = {}
+        validators: Dict[str, Any] = {}
+
+        # fully qualified name of the Entity class including support module
+        full_name = f"{support.module}.{definition.name}"
+
+        # add in each of the arguments as a Field in the Entity
+        for arg in definition.args:
+            full_arg_name = f"{full_name}.{arg.name}"
+            arg_type: Any
+
+            if isinstance(arg, ObjectArg):
+
+                @field_validator(arg.name, mode="after")
+                def lookup_instance(cls, id):
+                    return get_entity_by_id(id)
+
+                validators[full_arg_name] = lookup_instance
+                arg_type = object
+
+            elif isinstance(arg, IdArg):
+                arg_type = str
+
+            elif isinstance(arg, EnumArg):
+                # Pydantic uses the values of the Enum as the options in the schema.
+                # Here we arrange for the keys to be in the schema (what a user supplies)
+                # but the values to be what is rendered when jinja refers to the enum
+                enum_swapped = {}
+                for k, v in arg.values.items():
+                    enum_swapped[str(v) if v else str(k)] = k
+                # TODO review enums especially with respect to Pydantic 2.7.1
+                val_enum = EnumVal(arg.name, enum_swapped)  # type: ignore
+                arg_type = val_enum
+
+            else:
+                # arg.type is str, int, float, etc.
+                arg_type = getattr(builtins, arg.type)
+            add_arg(arg.name, arg_type, arg.description, getattr(arg, "default"))
+
+        # add in the calculated values Jinja Templates as Fields in the Entity
+        for value in definition.values:
+            add_arg(value.name, str, value.description, value.value)
+
+        # add the type literal which discriminates between the different Entity classes
+        typ = Literal[full_name]  # type: ignore
+        add_arg("type", typ, definition.description, full_name)
+
+        class_name = full_name.replace(".", "_")
+        entity_cls = create_model(
+            class_name,
+            **args,
+            __validators__=validators,
+            __base__=Entity,
+        )  # type: ignore
+
+        # add a link back to the Definition Instance that generated this Entity Class
+        entity_cls.__definition__ = definition
 
-def make_ioc_model(entity_models: Sequence[Type[Entity]]) -> Type[IOC]:
-    """
-    Create an IOC derived model, by setting its entities attribute to
-    be of type 'list of Entity derived classes'.
-    """
+        # store this Entity class in the factory
+        self._entity_models[full_name] = entity_cls
 
-    entity_union = Union[tuple(entity_models)]  # type: ignore
-    discriminated = Annotated[entity_union, Field(discriminator="type")]  # type: ignore
+        return entity_cls
 
-    class NewIOC(IOC):
-        entities: Sequence[discriminated] = Field(
-            description="List of entities this IOC instantiates"
-        )
+    def _make_entity_models(self, support: Support) -> List[Type[Entity]]:
+        """
+        Create Entity subclasses for all Definition instances in the given
+        Support instance. Returns a list of the Entity subclasses Models.
+        """
+        entity_names = []
+        entity_models = []
 
-    return NewIOC
+        for definition in support.defs:
+            if definition.name in entity_names:
+                # not tested because schema validation will always catch this first
+                raise ValueError(f"Duplicate entity name {definition.name}")
 
+            entity_models.append(self._make_entity_model(definition, support))
 
-def clear_entity_model_ids():
-    """Resets the global id_to_entity dict."""
+            entity_names.append(definition.name)
+        return entity_models
 
-    id_to_entity.clear()
+    def process_collections(self, entities: List[Entity]):
+        """
+        Process all the SubEntity collections in a list of Entity instances
+        """
+        all_entities: List[Entity] = []
 
+        def resolve_sub_entities(entity: Entity):
+            # recursive function to scan for SubEntities in an entity
+            definition = entity.__definition__
+
+            # add the parent standard entity
+            all_entities.append(entity)
+
+            # add in SubEntities if any
+            for sub_entity in definition.sub_entities:
+                # find the Entity Class that the SubEntity represents
+                entity_cls = self._entity_models[sub_entity.type]
+                # get the SubEntity arguments
+                sub_args_dict = sub_entity.model_dump()
+                # jinja render any references to parent Args in the SubEntity Args
+                for key, arg in sub_args_dict.items():
+                    sub_args_dict[key] = UTILS.render(entity, arg)
+                # cast the SubEntity to its concrete Entity subclass
+                cast_entity = entity_cls(**sub_args_dict)
+                # recursively scan the SubEntity for more SubEntities
+                resolve_sub_entities(cast_entity)
 
-class IOC(BaseSettings):
-    """
-    Used to load an IOC instance entities yaml file into a Pydantic Model.
-    """
+        for entity in entities:
+            resolve_sub_entities(entity)
 
-    ioc_name: str = Field(description="Name of IOC instance")
-    description: str = Field(description="Description of what the IOC does")
-    entities: Sequence[Entity]
+        return all_entities
```

### Comparing `ibek-3.4.0b2/src/ibek/ioc_cmds/assets.py` & `ibek-3.5.0b1/src/ibek/ioc_cmds/assets.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import shutil
 import subprocess
 from pathlib import Path
 from typing import List
 
 import typer
 
-from ibek.globals import GLOBALS, IOC_FOLDER
+from ibek.globals import GLOBALS
 
 log = logging.getLogger(__name__)
 
 
 def move_file(src: Path, dest: Path, binary: List[str]):
     """
     Move a file / tree / symlink from src to dest, stripping symbols from
@@ -58,16 +58,18 @@
 
     # a default set of assets that all IOCs will need at runtime
     if defaults:
         default_assets = [
             source / "support" / "configure",
             GLOBALS.PVI_DEFS,
             GLOBALS.IBEK_DEFS,
-            IOC_FOLDER,  # get the IOC folder symlink
-            Path.readlink(IOC_FOLDER),  # get contents of IOC folder
+            GLOBALS.IOC_FOLDER,  # get the IOC folder symlink
+            Path.readlink(
+                GLOBALS.IOC_FOLDER
+            ).parent,  # get contents of IOC folder and its source (parent)
             Path("/venv"),  # get the virtualenv
         ] + list(
             source.glob("ibek*")
         )  # get ibek-support and related folders
     else:
         default_assets = []
```

### Comparing `ibek-3.4.0b2/src/ibek/ioc_cmds/commands.py` & `ibek-3.5.0b1/src/ibek/ioc_cmds/commands.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import json
 import logging
 from pathlib import Path
 from typing import Annotated, List, Optional
 
 import typer
 
-from ibek.gen_scripts import ioc_create_model
+from ibek.entity_factory import EntityFactory
 from ibek.globals import (
     GLOBALS,
     SUPPORT_YAML_PATTERN,
     NaturalOrderGroup,
 )
 from ibek.ioc_cmds.docker import build_dockerfile
+from ibek.ioc_factory import IocFactory
 
 from .assets import extract_assets
 
 log = logging.getLogger(__name__)
 ioc_cli = typer.Typer(cls=NaturalOrderGroup)
 
 
@@ -75,15 +76,19 @@
         # which are in a known location after the container is built
         definitions += GLOBALS.IBEK_DEFS.glob(SUPPORT_YAML_PATTERN)
 
     if not definitions:
         log.error(f"No `definitions` given and none found in {GLOBALS.IBEK_DEFS}")
         raise typer.Exit(1)
 
-    ioc_model = ioc_create_model(definitions)
+    entity_factory = EntityFactory()
+    entity_models = entity_factory.make_entity_models(definitions)
+    ioc_factory = IocFactory()
+    ioc_model = ioc_factory.make_ioc_model(entity_models)
+
     schema = json.dumps(ioc_model.model_json_schema(), indent=2)
     if output is None:
         typer.echo(schema)
     else:
         output.write_text(schema)
```

### Comparing `ibek-3.4.0b2/src/ibek/ioc_cmds/docker.py` & `ibek-3.5.0b1/src/ibek/ioc_cmds/docker.py`

 * *Files identical despite different names*

### Comparing `ibek-3.4.0b2/src/ibek/render.py` & `ibek-3.5.0b1/src/ibek/render.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Functions for rendering lines in the boot script using Jinja2
 """
 
-from typing import Callable, List, Optional, Union
+from typing import Callable, List, Optional, Sequence, Union
 
-from .ioc import IOC, Entity
-from .support import Comment, Script, Text, When
+from .definition import Comment, Script, Text, When
+from .ioc import Entity
 from .utils import UTILS
 
 
 class Render:
     """
     A class for generating snippets of startup script / EPICS DB
     by using Jinja to combine snippet templates from support module
@@ -100,37 +100,39 @@
             env_var_txt += UTILS.render(
                 instance,
                 env_template,
             )  # type: ignore
         return env_var_txt + "\n"
 
     def render_elements(
-        self, ioc: IOC, method: Callable[[Entity], Union[str, None]]
+        self,
+        entities: Sequence[Entity],
+        render_element: Callable[[Entity], Union[str, None]],
     ) -> str:
         """
         Render elements of a given IOC instance based on calling the correct method
         """
         elements = ""
-        for entity in ioc.entities:
+        for entity in entities:
             if entity.entity_enabled:
-                element = method(entity)
+                element = render_element(entity)
                 if element:
                     elements += element
         return elements
 
-    def render_pre_ioc_init_elements(self, ioc: IOC) -> str:
+    def render_pre_ioc_init_elements(self, entities: Sequence[Entity]) -> str:
         """
         Render all of the startup script entries for a given IOC instance
         """
-        return self.render_elements(ioc, self.render_pre_ioc_init)
+        return self.render_elements(entities, self.render_pre_ioc_init)
 
-    def render_post_ioc_init_elements(self, ioc: IOC) -> str:
+    def render_post_ioc_init_elements(self, entities: Sequence[Entity]) -> str:
         """
         Render all of the post-iocInit elements for a given IOC instance
         """
-        return self.render_elements(ioc, self.render_post_ioc_init)
+        return self.render_elements(entities, self.render_post_ioc_init)
 
-    def render_environment_variable_elements(self, ioc: IOC) -> str:
+    def render_environment_variable_elements(self, entities: Sequence[Entity]) -> str:
         """
         Render all of the environment variable entries for a given IOC instance
         """
-        return self.render_elements(ioc, self.render_environment_variables)
+        return self.render_elements(entities, self.render_environment_variables)
```

### Comparing `ibek-3.4.0b2/src/ibek/render_db.py` & `ibek-3.5.0b1/src/ibek/render_db.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 """
 A class for rendering a substitution file from multiple instantiations of
 support module definitions
 """
 
 from dataclasses import dataclass
-from typing import Any, Dict, List, Mapping, Optional, Tuple
+from typing import Any, Dict, List, Mapping, Optional, Sequence, Tuple
 
-from ibek.ioc import IOC, Entity
-from ibek.support import Database
+from ibek.definition import Database
+from ibek.ioc import Entity
 from ibek.utils import UTILS
 
 
 def str_to_bool(v):
     return v.lower() in ("yes", "true", "1")
 
 
 class RenderDb:
     @dataclass
     class RenderDbTemplate:
         filename: str
         rows: List[List[str]]
         columns: List[int]
 
-    def __init__(self, ioc_instance: IOC) -> None:
-        self.ioc_instance = ioc_instance
+    def __init__(self, entities: Sequence[Entity]) -> None:
+        self.entities = entities
         # a mapping from template file name to details of instances of that template
         self.render_templates: Dict[str, RenderDb.RenderDbTemplate] = {}
 
     def add_row(self, filename: str, args: Mapping[str, Any], entity: Entity) -> None:
         """
         Accumulate rows of arguments for each template file,
         Adding a new template file if it does not already exist.
@@ -51,15 +51,15 @@
         self.render_templates[filename].rows.append(row)
 
     def parse_instances(self) -> None:
         """
         Gather the database template instantiations from all entities
         while validating the arguments
         """
-        for entity in self.ioc_instance.entities:
+        for entity in self.entities:
             databases = entity.__definition__.databases
 
             # Not all entities instantiate database templates
             if entity.entity_enabled and databases is not None:
                 for database in databases:
                     self.add_database(database, entity)
```

### Comparing `ibek-3.4.0b2/src/ibek/runtime_cmds/commands.py` & `ibek-3.5.0b1/src/ibek/runtime_cmds/commands.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 
 import typer
 from pvi._format.base import IndexEntry
 from pvi._format.dls import DLSFormatter
 from pvi._format.template import format_template
 from pvi.device import Device
 
-from ibek.gen_scripts import create_boot_script, create_db_script, ioc_deserialize
+from ibek.definition import Database
+from ibek.entity_factory import EntityFactory
+from ibek.gen_scripts import create_boot_script, create_db_script
 from ibek.globals import GLOBALS, NaturalOrderGroup
 from ibek.ioc import IOC, Entity
-from ibek.support import Database
+from ibek.ioc_factory import IocFactory
 from ibek.utils import UTILS
 
 runtime_cli = typer.Typer(cls=NaturalOrderGroup)
 
 
 @runtime_cli.command()
 def generate(
@@ -32,32 +34,38 @@
 ):
     """
     Build a startup script for an IOC instance
     """
     # the file name under of the instance definition provides the IOC name
     UTILS.set_file_name(instance)
 
-    ioc_instance = ioc_deserialize(instance, definitions)
+    entity_factory = EntityFactory()
+    entity_models = entity_factory.make_entity_models(definitions)
+    ioc_instance = IocFactory().deserialize_ioc(instance, entity_models)
+
+    # post processing to insert SubEntity instances
+    all_entities = entity_factory.process_collections(ioc_instance.entities)
+    ioc_instance.entities = all_entities
 
     # Clear out generated files so developers know if something stops being generated
     shutil.rmtree(GLOBALS.RUNTIME_OUTPUT, ignore_errors=True)
     GLOBALS.RUNTIME_OUTPUT.mkdir(exist_ok=True)
     shutil.rmtree(GLOBALS.OPI_OUTPUT, ignore_errors=True)
     GLOBALS.OPI_OUTPUT.mkdir(exist_ok=True)
 
     pvi_index_entries, pvi_databases = generate_pvi(ioc_instance)
     generate_index(ioc_instance.ioc_name, pvi_index_entries)
 
-    script_txt = create_boot_script(ioc_instance)
+    script_txt = create_boot_script(ioc_instance.entities)
     script_output = GLOBALS.RUNTIME_OUTPUT / "st.cmd"
     script_output.parent.mkdir(parents=True, exist_ok=True)
     with script_output.open("w") as stream:
         stream.write(script_txt)
 
-    db_txt = create_db_script(ioc_instance, pvi_databases)
+    db_txt = create_db_script(ioc_instance.entities, pvi_databases)
     db_output = GLOBALS.RUNTIME_OUTPUT / "ioc.subst"
     with db_output.open("w") as stream:
         stream.write(db_txt)
 
 
 def generate_pvi(ioc: IOC) -> Tuple[List[IndexEntry], List[Tuple[Database, Entity]]]:
     """Generate pvi bob and template files to add to UI index and IOC database.
@@ -73,17 +81,18 @@
     index_entries: List[IndexEntry] = []
     databases: List[Tuple[Database, Entity]] = []
 
     formatter = DLSFormatter()
 
     formatted_pvi_devices: List[str] = []
     for entity in ioc.entities:
-        entity_pvi = entity.__definition__.pvi
-        if entity_pvi is None:
+        definition = entity.__definition__
+        if not hasattr(definition, "pvi") or definition.pvi is None:
             continue
+        entity_pvi = definition.pvi
 
         pvi_yaml = GLOBALS.PVI_DEFS / entity_pvi.yaml_path
         device_name = pvi_yaml.name.split(".")[0]
         device_bob = GLOBALS.OPI_OUTPUT / f"{device_name}.pvi.bob"
 
         # Skip deserializing yaml if not needed
         if entity_pvi.pv or device_name not in formatted_pvi_devices:
```

### Comparing `ibek-3.4.0b2/src/ibek/support.py` & `ibek-3.5.0b1/src/ibek/definition.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """
-The Support Class represents a deserialized <MODULE_NAME>.ibek.support.yaml file.
+The Definition class describes what a given support module can instantiate.
 """
 
 from __future__ import annotations
 
-import json
 from enum import Enum
-from typing import Any, Dict, Mapping, Optional, Sequence, Union
+from typing import Any, Mapping, Optional, Sequence, Union
 
 from pydantic import Field, PydanticUndefinedAnnotation
 from typing_extensions import Literal
 
+from .args import Arg, IdArg, Value
 from .globals import BaseSettings
+from .sub_entity import SubEntity
 
 
 def default(T: type):
     """
     defines a default type which may be
     """
     return Field(
@@ -26,79 +27,14 @@
 
 class When(Enum):
     first = "first"
     every = "every"
     last = "last"
 
 
-class Arg(BaseSettings):
-    """Base class for all Argument Types"""
-
-    type: str
-    name: str = Field(
-        description="Name of the argument that the IOC instance should pass"
-    )
-    description: str = Field(
-        description="Description of what the argument will be used for"
-    )
-
-
-class FloatArg(Arg):
-    """An argument with a float value"""
-
-    type: Literal["float"] = "float"
-    default: Optional[float] = None
-
-
-class StrArg(Arg):
-    """An argument with a str value"""
-
-    type: Literal["str"] = "str"
-    default: Optional[str] = None
-
-
-class IntArg(Arg):
-    """An argument with an int value"""
-
-    type: Literal["int"] = "int"
-    default: Optional[int] = None
-
-
-class BoolArg(Arg):
-    """An argument with an bool value"""
-
-    type: Literal["bool"] = "bool"
-    default: Optional[bool] = None
-
-
-class ObjectArg(Arg):
-    """A reference to another entity defined in this IOC"""
-
-    type: Literal["object"] = "object"
-    default: Optional[str] = None
-
-
-class IdArg(Arg):
-    """Explicit ID argument that an object can refer to"""
-
-    type: Literal["id"] = "id"
-    default: Optional[str] = None
-
-
-class EnumArg(Arg):
-    """An argument with an enum value"""
-
-    type: Literal["enum"] = "enum"
-    default: Optional[Any] = None
-
-    values: Dict[str, Any] = Field(
-        description="provides a list of values to make this argument an Enum",
-    )
-
-
 class Database(BaseSettings):
     """
     A database file that should be loaded by the startup script and its args
     """
 
     file: str = Field(
         description="Filename of the database template in <module_root>/db"
@@ -145,24 +81,14 @@
     """
 
     type: Literal["text"] = "text"
     when: str = Field(description="One of first / every / last", default="every")
     value: str = Field(description="raw text to add to the startup script", default="")
 
 
-class Value(BaseSettings):
-    """A calculated string value for a definition"""
-
-    name: str = Field(description="Name of the value that the IOC instance will expose")
-    description: str = Field(
-        description="Description of what the value will be used for"
-    )
-    value: str = Field(description="The contents of the value")
-
-
 Script = Sequence[Union[Text, Comment]]
 
 
 class EntityPVI(BaseSettings):
     """Entity PVI definition"""
 
     yaml_path: str = Field(
@@ -185,15 +111,15 @@
             "Whether to generate a PVI PV. This adds a database template with info "
             "tags that create a PVAccess PV representing the device structure."
         ),
     )
     pv_prefix: str = Field("", description='PV prefix for PVI PV - e.g. "$(P)"')
 
 
-class Definition(BaseSettings):
+class EntityDefinition(BaseSettings):
     """
     A single definition of a class of Entity that an IOC instance may instantiate
     """
 
     name: str = Field(
         description="Publish Definition as type <module>.<name> for IOC instances"
     )
@@ -201,46 +127,42 @@
         description="A description of the Support module defined here"
     )
     # declare Arg as Union of its subclasses for Pydantic to be able to deserialize
     args: Sequence[Union[tuple(Arg.__subclasses__())]] = Field(  # type: ignore
         description="The arguments IOC instance should supply", default=()
     )
     values: Sequence[Value] = Field(
-        description="The values IOC instance should supply", default=()
+        description="Calculated values to use as additional arguments", default=()
     )
     databases: Sequence[Database] = Field(
         description="Databases to instantiate", default=[]
     )
     pre_init: Script = Field(
         description="Startup script snippets to add before iocInit()", default=()
     )
     post_init: Script = Field(
         description="Startup script snippets to add post iocInit(), such as dbpf",
         default=(),
     )
     env_vars: Sequence[EnvironmentVariable] = Field(
         description="Environment variables to set in the boot script", default=()
     )
-    pvi: EntityPVI = Field(description="PVI definition for Entity", default=None)
+    pvi: Optional[EntityPVI] = Field(
+        description="PVI definition for Entity", default=None
+    )
+
+    # list of additional entities to instantiate for each instance of this definition
+    sub_entities: Sequence[SubEntity] = Field(
+        description="The sub-entity instances that this collection is to instantiate",
+        default=(),
+    )
+
+    shared: Sequence[Any] = Field(
+        description="A place to create any anchors required for repeating YAML",
+        default=(),
+    )
 
     def _get_id_arg(self):
         """Returns the name of the ID argument for this definition, if it exists"""
         for arg in self.args:
             if isinstance(arg, IdArg):
                 return arg.name
-
-
-class Support(BaseSettings):
-    """
-    Lists the definitions for a support module, this defines what Entities it supports
-
-    Provides the deserialize entry point.
-    """
-
-    module: str = Field(description="Support module name, normally the repo name")
-    defs: Sequence[Definition] = Field(
-        description="The definitions an IOC can create using this module"
-    )
-
-    @classmethod
-    def get_schema(cls):
-        return json.dumps(cls.model_json_schema(), indent=2)
```

### Comparing `ibek-3.4.0b2/src/ibek/support_cmds/checks.py` & `ibek-3.5.0b1/src/ibek/support_cmds/checks.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import re
 import shutil
 from pathlib import Path
 
 import typer
 
-from ibek.globals import MODULES, RELEASE, RELEASE_SH, SUPPORT, TEMPLATES
+from ibek.globals import GLOBALS, TEMPLATES
 
 # turn RELEASE macros into bash macros
 SHELL_FIND = re.compile(r"\$\(([^\)]*)\)")
 SHELL_REPLACE = r"${\1}"
 
 # find macros, including ones with blank values
 PARSE_MACROS_NULL = re.compile(r"^([A-Z_a-z0-9]*)\s*=(.*)$", flags=re.M)
@@ -42,31 +42,31 @@
     """
     Fix up the global release file to include all support modules registered
     """
     validate_support()
 
     # parse the global release file
     global_release_paths = {}
-    text = RELEASE.read_text()
+    text = GLOBALS.RELEASE.read_text()
     for match in PARSE_MACROS_NULL.findall(text):
         global_release_paths[match[0]] = match[1]
 
     # generate the MODULES file for inclusion into the root Makefile
     # it simply defines a variable to hold each of the support module
     # directories in the order they are presented in RELEASE, except that
-    s = str(SUPPORT)
+    s = str(GLOBALS.SUPPORT)
     paths = [
         path[len(s) + 1 :]
         for path in global_release_paths.values()
         if path.startswith(s)
     ]
     if "IOC" in global_release_paths:
         paths.append(global_release_paths["IOC"])
     mod_list = f'MODULES := {" ".join(paths)}\n'
-    MODULES.write_text(mod_list)
+    GLOBALS.MODULES.write_text(mod_list)
 
     # generate RELEASE.shell file for inclusion into the ioc launch shell script.
     # This adds all module paths to the environment and also adds their db
     # folders to the database search path env variable EPICS_DB_INCLUDE_PATH
     release_sh = []
     for module, path in global_release_paths.items():
         release_sh.append(f'export {module}="{path}"')
@@ -75,15 +75,44 @@
         f"{path}/db" for path in global_release_paths.values() if path.startswith(s)
     ]
     db_path_list = ":".join(db_paths)
     release_sh.append(f'export EPICS_DB_INCLUDE_PATH="{db_path_list}"')
 
     shell_text = "\n".join(release_sh) + "\n"
     shell_text = SHELL_FIND.sub(SHELL_REPLACE, shell_text)
-    RELEASE_SH.write_text(shell_text)
+    GLOBALS.RELEASE_SH.write_text(shell_text)
+
+
+def check_deps(deps: list[str]) -> None:
+    """
+    Check if specified dependencies have been supplied
+    """
+    for dependency in deps:
+        # Check if UCASE module name exist in RELEASE
+        with open(GLOBALS.RELEASE) as file:
+            release_file = file.read()
+            if dependency.upper() in release_file:
+                pass
+            else:
+                raise Exception(f"{dependency.upper()} not in {GLOBALS.RELEASE}")
+
+        # Check if folder with the module name exist in /epics/support
+        support_dir = GLOBALS.SUPPORT / dependency
+        if Path.exists(support_dir):
+            # Check if contains at least one of db, dbd or lib
+            res = [Path.exists(support_dir / _dir) for _dir in ["db", "dbd", "lib"]]
+            if any(res):
+                pass
+            else:
+                raise Exception(f"db, dbd or lib directory not found in {support_dir}")
+
+        else:
+            raise Exception(f"{dependency} directory not in {GLOBALS.SUPPORT}")
+
+        print(f"SUCCESS: {dependency} checked")
 
 
 def add_macro(macro: str, value: str, file: Path, replace: bool = True):
     """
     add or replace a macro in a RELEASE or CONFIG file
     """
     validate_support()
@@ -107,17 +136,17 @@
 def validate_support():
     """
     Validate that the support folder exists and setup initial template files
     if required
     """
     template_support = TEMPLATES / "support"
     release = Path("configure") / "RELEASE"
-    global_release = SUPPORT / release
+    global_release = GLOBALS.SUPPORT / release
 
-    if not SUPPORT.exists():
-        typer.echo(f"INITIALIZING {SUPPORT} folder with template")
-        shutil.copytree(template_support, SUPPORT)
+    if not GLOBALS.SUPPORT.exists():
+        typer.echo(f"INITIALIZING {GLOBALS.SUPPORT} folder with template")
+        shutil.copytree(template_support, GLOBALS.SUPPORT)
     else:
         if not global_release.exists():
             global_release.parent.mkdir(parents=True, exist_ok=True)
-            typer.echo(f"INITIALIZING {SUPPORT / release} folder with template")
+            typer.echo(f"INITIALIZING {GLOBALS.SUPPORT / release} folder with template")
             shutil.copy2(template_support / release, global_release)
```

### Comparing `ibek-3.4.0b2/src/ibek/support_cmds/commands.py` & `ibek-3.5.0b1/src/ibek/support_cmds/commands.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,26 +14,22 @@
     pass  # Git Python is not needed for runtime (container build time only)
 
 from typing_extensions import Annotated
 
 from ibek.globals import (
     GLOBALS,
     IBEK_GLOBALS,
-    IOC_DBDS,
-    IOC_LIBS,
     PVI_YAML_PATTERN,
-    RELEASE,
-    RUNTIME_DEBS,
-    SUPPORT,
     SUPPORT_YAML_PATTERN,
     NaturalOrderGroup,
 )
 from ibek.support import Support
 from ibek.support_cmds.checks import (
     add_macro,
+    check_deps,
     do_dependencies,
     verify_release_includes_local,
 )
 from ibek.support_cmds.files import (
     Arch,
     add_list_to_file,
     add_text_once,
@@ -58,20 +54,23 @@
 
 def _install_debs(debs: List[str]) -> None:
     """
     Install a list of debian packages.
 
     If they have an http:// or https://
     prefix then they will be downloaded and installed from file.
+
+    args: debs: List[str] - list of debian packages to install - can also include
+                            any additional 'apt-get install' options required
     """
     temp = Path("/tmp")
     for i, pkg in enumerate(debs):
         if pkg.startswith("http://") or pkg.startswith("https://"):
             pkg_file = temp / pkg.split("/")[-1]
-            subprocess.call(["wget", pkg, "-O", str(pkg_file)])
+            subprocess.call(["busybox", "wget", pkg, "-O", str(pkg_file)])
             debs[i] = str(pkg_file)
 
     if len(debs) == 0:
         print("no packages to install")
         return
 
     print("installing packages: ", debs)
@@ -82,32 +81,40 @@
         f"{sudo} apt-get install -y --no-install-recommends " + " ".join(debs)
     )
     exit(subprocess.call(["bash", "-c", command]))
 
 
 @support_cli.command()
 def apt_install(
-    debs: List[str] = typer.Argument(None, help="list of debian packages to install"),
+    debs: List[str] = typer.Argument(
+        None,
+        help=(
+            "list of debian packages to install. Also may include any "
+            "additional 'apt-get install' options required"
+        ),
+    ),
 ):
     """
     Install packages
     """
     debs = debs or []
     _install_debs(debs)
 
 
 @support_cli.command()
 def add_runtime_packages(
     debs: List[str] = typer.Argument(None, help="list of debian packages to install"),
 ):
     """
     Add packages to RUNTIME_DEBS for later install with apt_install_runtime_packages
+
+    The list may include any additional 'apt-get install' options required.
     """
     debs = debs or []
-    add_list_to_file(RUNTIME_DEBS, debs)
+    add_list_to_file(GLOBALS.RUNTIME_DEBS, debs)
 
 
 @support_cli.command()
 def apt_install_runtime_packages(
     skip_non_native: bool = typer.Option(
         False, help="skip installation in cross-compile environment"
     ),
@@ -115,18 +122,17 @@
     """
     Install packages from the list collected by calls to add_runtime_packages
     """
     if not GLOBALS.NATIVE and skip_non_native:
         print("skipping runtime install in cross-compile environment")
         return
 
-    if RUNTIME_DEBS.exists():
-        debs = RUNTIME_DEBS.read_text().split()
-
-    _install_debs(debs)
+    if GLOBALS.RUNTIME_DEBS.exists():
+        debs = GLOBALS.RUNTIME_DEBS.read_text().split()
+        _install_debs(debs)
 
 
 @support_cli.command(
     context_settings={"allow_extra_args": True, "ignore_unknown_options": True}
 )
 def git_clone(
     ctx: typer.Context,
@@ -135,25 +141,33 @@
     org: str = typer.Option(
         "https://github.com/epics-modules/", help="repo organization URL"
     ),
     force: bool = typer.Option(False, help="overwrite existing clone"),
 ):
     """
     clone a support module from a remote repository
+
+    Add any additional arguments to the git clone command at the end of the
+    argument list.
     """
+    org = org if org.endswith("/") else org + "/"
     url = org + repo_name
-    location = SUPPORT / repo_name
+    location = GLOBALS.SUPPORT / repo_name
     if location.exists() and not force:
         print(f"skipping {location}, already cloned")
         return
     else:
         rmtree(location, ignore_errors=True)
 
     Repo.clone_from(
-        url, SUPPORT / repo_name, branch=version, depth=1, multi_options=ctx.args
+        url,
+        GLOBALS.SUPPORT / repo_name,
+        branch=version,
+        depth=1,
+        multi_options=ctx.args,
     )
 
 
 @support_cli.command()
 def register(
     name: str = typer.Argument(..., help="the name of the support module"),
     path: Annotated[
@@ -166,23 +180,23 @@
     macro: Optional[str] = typer.Option(None, help="Macro name for the module"),
 ):
     """
     prepare the configure RELEASE files to build a support module
     inside an epics-containers build
     """
     macro = name.upper() if macro is None else macro
-    path = SUPPORT / name if (path is None) else path
+    path = GLOBALS.SUPPORT / name if (path is None) else path
 
     # add or replace the macro for this module in the global RELEASE file
-    add_macro(macro, str(path), RELEASE)
+    add_macro(macro, str(path), GLOBALS.RELEASE)
 
     # bring the global release file into this module with a symlink
     local = path / "configure" / "RELEASE.local"
     local.unlink(missing_ok=True)
-    local.symlink_to(RELEASE)
+    local.symlink_to(GLOBALS.RELEASE)
 
     # make sure this module uses RELEASE.local
     verify_release_includes_local(path / "configure")
 
     do_dependencies()
 
 
@@ -190,38 +204,37 @@
 def add_libs(
     libs: List[str] = typer.Argument(None, help="list of libraries to add"),
 ) -> None:
     """
     declare the libraries for this support module for inclusion in IOC Makefile
     """
     libs = libs or []
-    add_list_to_file(IOC_LIBS, libs)
+    add_list_to_file(GLOBALS.IOC_LIBS, libs)
 
 
 @support_cli.command()
 def add_dbds(
     dbds: List[str] = typer.Argument(None, help="list of dbd files to add"),
 ) -> None:
     """
     declare the dbd files for this support module for inclusion in IOC Makefile
     """
     dbds = dbds or []
-    add_list_to_file(IOC_DBDS, dbds)
 
 
 @support_cli.command()
 def add_release_macro(
     macro: str = typer.Argument(..., help="macro name to update"),
     value: str = typer.Argument("", help="value to set for the macro"),
     replace: bool = typer.Option(True, help="overwrite previous value"),
 ):
     """
     add or replace a macro the global RELEASE file
     """
-    add_macro(macro, value, RELEASE, replace)
+    add_macro(macro, value, GLOBALS.RELEASE, replace)
 
 
 @support_cli.command()
 def add_config_macro(
     name: str = typer.Argument(..., help="the name of the support module"),
     macro: str = typer.Argument(..., help="macro name to update"),
     value: str = typer.Argument("", help="value to set for the macro"),
@@ -249,25 +262,37 @@
 
     # nothing to do if text is blank
     if text != "":
         config_site = get_config_site_file(module, host, target)
         add_text_once(config_site, text)
 
 
+@support_cli.command()
+def check_dependencies(
+    deps: List[str] = typer.Argument(help="list of dependencies to check"),
+):
+    """
+    Check if specified dependencies have been supplied
+    """
+    check_deps(deps)
+
+
 @support_cli.command(
     context_settings={"allow_extra_args": True, "ignore_unknown_options": True}
 )
 def compile(
     ctx: typer.Context,
     module: str = typer.Argument(..., help="support module name"),
 ):
     """
     compile a support module after preparation with `ibek support register` etc.
+
+    Add any extra compiler options to the end of the argument list
     """
-    path = SUPPORT / module
+    path = GLOBALS.SUPPORT / module
 
     command = f"make -C {path} -j $(nproc) " + " ".join(ctx.args)
     result = subprocess.call(["bash", "-c", command])
     # save size of developer container with make clean
     command = f"make -C {path} -j $(nproc) clean"
     subprocess.call(["bash", "-c", command])
     exit(result)
```

### Comparing `ibek-3.4.0b2/src/ibek/support_cmds/files.py` & `ibek-3.5.0b1/src/ibek/support_cmds/files.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from enum import Enum
 from pathlib import Path
 from typing import List
 
 import typer
 
-from ibek.globals import SUPPORT
+from ibek.globals import GLOBALS
 
 
 class Local(str, Enum):
     non_local = ""
     local = ".local"
 
 
@@ -31,15 +31,15 @@
     target: Arch = Arch.common,
 ) -> Path:
     """
     Return the path to an CONFIG_SITE file for a support module.
     Default is /epics/module/configure/CONFIG_SITE.local.linux-x86_64.Common
     """
     name = f"CONFIG_SITE{host.value}{target.value}"
-    filepath = SUPPORT / module / "configure" / name
+    filepath = GLOBALS.SUPPORT / module / "configure" / name
 
     return filepath
 
 
 def get_release_file(
     module: str,
     host: Arch = Arch.none,
@@ -47,15 +47,15 @@
     local: Local = Local.local,
 ) -> Path:
     """
     Return the path to an EPICS RELEASE file for a support
     default is /epics/module/configure/RELEASE.local
     """
     name = f"RELEASE{host.value}{target.value}{local.value}"
-    filepath = SUPPORT / module / "configure" / name
+    filepath = GLOBALS.SUPPORT / module / "configure" / name
 
     return filepath
 
 
 def add_list_to_file(file: Path, text_list: List[str]):
     """
     add a sequence of strings into a file, leaving previously existing
```

### Comparing `ibek-3.4.0b2/src/ibek/utils.py` & `ibek-3.5.0b1/src/ibek/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -97,18 +97,23 @@
                 )
         result = counter.current
         counter.increment(inc)
         self.counters[name] = counter
 
         return result
 
-    def render(self, context: Any, template_text: str) -> str:
+    def render(self, context: Any, template_text: Any) -> str:
         """
         Render a Jinja template with the global __utils__ object in the context
         """
+        if not isinstance(template_text, str):
+            # because this function is used to template arguments, it may
+            # be passed a non string which will always render to itself
+            return template_text
+
         jinja_template = Template(template_text)
         return jinja_template.render(
             context,
             __utils__=self,
             ioc_yaml_file_name=self.file_name,
             ioc_name=self.ioc_name,
         )
```

### Comparing `ibek-3.4.0b2/src/ibek.egg-info/PKG-INFO` & `ibek-3.5.0b1/src/ibek.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibek
-Version: 3.4.0b2
+Version: 3.5.0b1
 Summary: IOC Builder for EPICS and Kubernetes
 Author-email: Tom Cobb <tom.cobb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -214,14 +214,15 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: pydantic==2.6.4
 Requires-Dist: typer
 Requires-Dist: ruamel.yaml
 Requires-Dist: jinja2
 Requires-Dist: GitPython
+Requires-Dist: semantic-version
 Requires-Dist: pvi~=0.8
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pipdeptree; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pydata-sphinx-theme>=0.12; extra == "dev"
@@ -251,14 +252,28 @@
   ============== ==============================================================
   PyPI           ``pip install ibek``
   Source code    https://github.com/epics-containers/ibek
   Documentation  https://epics-containers.github.io/ibek
   Releases       https://github.com/epics-containers/ibek/releases
   ============== ==============================================================
 
+UPDATE: Version 2.0.0
+=====================
+
+There have been a number of breaking changes since version 1.8.0. These are
+primarily to support RTEMS cross compiled IOCs. But we have also taken the
+opportunity to clarify the CLI.
+
+All changes are compatible with 2.0.0 of ibek-support and 3.4.0 of all other
+epics-containers repos. When using ioc-template 3.4.0 to update your generic
+IOCs, make sure you also update the ibek-support submodule to 2.0.0 or newer,
+then you should have all compatible versions.
+
+--------------------------------------------------------------------------------
+
 
 The documentation is still under construction. For the moment the best
 pages to read are the following:
 
 - `Modules, Definitions and Entities <https://epics-containers.github.io/ibek/main/developer/explanations/entities.html//>`_
   A description of the basic concepts of ibek.
```

### Comparing `ibek-3.4.0b2/tests/conftest.py` & `ibek-3.5.0b1/tests/conftest.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import os
+import shutil
 from pathlib import Path
 
 from pytest import fixture
+from pytest_mock import MockerFixture
 from ruamel.yaml import YAML
 from typer.testing import CliRunner
 
-# This must be above the following imports so that it takes effect before
-# `globals.EPICS_ROOT` is imported (or anything built on top of it)
-os.environ["EPICS_ROOT"] = str(Path(__file__).parent / "samples" / "epics")
-
-# The `noqa`s on these imports are necessary because of the above
-from ibek.__main__ import cli  # noqa: E402
-from ibek.ioc import clear_entity_model_ids, make_entity_models  # noqa: E402
-from ibek.support import Support  # noqa: E402
+from ibek.__main__ import cli
+from ibek.entity_factory import EntityFactory
+from ibek.globals import GLOBALS
+from ibek.support import Support
 
 runner = CliRunner()
 
 
 def run_cli(*args):
     result = runner.invoke(cli, [str(x) for x in args])
     if result.exception:
@@ -51,37 +49,57 @@
 
 
 @fixture
 def ioc_defs(samples):
     return samples / "iocs"
 
 
+# only one IocFactory instance for each test
+@fixture(scope="function")
+def entity_factory():
+    return EntityFactory()
+
+
 @fixture
-def asyn_classes(support_defs):
-    # clear the entity classes to make sure there's nothing left
-    clear_entity_model_ids()
+def epics_root(samples: Path, tmp_path: Path, mocker: MockerFixture):
+    # create an partially populated epics_root structure in a temporary folder
+    epics = tmp_path / "epics"
+    shutil.copytree(samples / "epics", epics)
+    Path.mkdir(epics / "opi", exist_ok=True)
+    Path.mkdir(epics / "epics-base")
+    Path.mkdir(epics / "ioc/config", parents=True)
+    Path.mkdir(epics / "ibek-defs")
+    Path.mkdir(epics / "runtime")
+
+    mocker.patch.object(GLOBALS, "_EPICS_ROOT", epics)
+
+    # this should not be needed - what gives?
+    os.environ["IOC"] = "/epics/ioc"
+    os.environ["RUNTIME_DIR"] = "/epics/runtime"
 
+    return epics
+
+
+@fixture
+def asyn_classes(support_defs, entity_factory):
     asyn_support = get_support(support_defs / "asyn.ibek.support.yaml")
 
     # make entity subclasses for everything defined in it
-    namespace = make_entity_models(asyn_support)
+    namespace = entity_factory._make_entity_models(asyn_support)
 
     # return the namespace so that callers have access to all of the
     # generated dataclasses
     return namespace
 
 
 @fixture
-def motor_classes(support_defs):
-    # clear the entity classes to make sure there's nothing left
-    clear_entity_model_ids()
-
+def motor_classes(support_defs, entity_factory):
     asyn_support = get_support(support_defs / "asyn.ibek.support.yaml")
     motor_support = get_support(support_defs / "motorSim.ibek.support.yaml")
 
     # make entity subclasses for everything defined in it
-    namespace = make_entity_models(asyn_support)
-    namespace.extend(make_entity_models(motor_support))
+    namespace = entity_factory._make_entity_models(asyn_support)
+    namespace.extend(entity_factory._make_entity_models(motor_support))
 
     # return the namespace so that callers have access to all of the
     # generated dataclasses
     return namespace
```

### Comparing `ibek-3.4.0b2/tests/samples/iocs/ibek-mo-ioc-01.yaml` & `ibek-3.5.0b1/tests/samples/iocs/ibek-mo-ioc-01.yaml`

 * *Files identical despite different names*

### Comparing `ibek-3.4.0b2/tests/samples/outputs/motorSim/index.bob` & `ibek-3.5.0b1/tests/samples/outputs/motorSim/index.bob`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <display version="2.0.0">
-  <name>Display</name>
+  <name>ibek-mo-ioc-01</name>
   <x>0</x>
   <y use_class="true">0</y>
   <width>388</width>
   <height>55</height>
   <grid_step_x>4</grid_step_x>
   <grid_step_y>4</grid_step_y>
   <widget type="label" version="2.0.0">
```

### Comparing `ibek-3.4.0b2/tests/samples/outputs/motorSim/ioc.subst` & `ibek-3.5.0b1/tests/samples/outputs/motorSim/ioc.subst`

 * *Files identical despite different names*

### Comparing `ibek-3.4.0b2/tests/samples/outputs/motorSim/simple.pvi.bob` & `ibek-3.5.0b1/tests/samples/outputs/motorSim/simple.pvi.bob`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <display version="2.0.0">
-  <name>Display</name>
+  <name>Simple Device</name>
   <x>0</x>
   <y use_class="true">0</y>
   <width>388</width>
   <height>55</height>
   <grid_step_x>4</grid_step_x>
   <grid_step_y>4</grid_step_y>
   <widget type="label" version="2.0.0">
```

### Comparing `ibek-3.4.0b2/tests/samples/outputs/motorSim/st.cmd` & `ibek-3.5.0b1/tests/samples/outputs/motorSim/st.cmd`

 * *Files identical despite different names*

### Comparing `ibek-3.4.0b2/tests/samples/outputs/utils/index.bob` & `ibek-3.5.0b1/tests/samples/outputs/ipac/index.bob`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 <display version="2.0.0">
-  <name>Display</name>
+  <name>ipac-test</name>
   <x>0</x>
   <y use_class="true">0</y>
   <width>10</width>
   <height>35</height>
   <grid_step_x>4</grid_step_x>
   <grid_step_y>4</grid_step_y>
   <widget type="label" version="2.0.0">
     <name>Title</name>
     <class>TITLE</class>
-    <text>counter</text>
+    <text>ipac-test</text>
     <x use_class="true">0</x>
     <y use_class="true">0</y>
     <width>10</width>
     <height>25</height>
     <font use_class="true">
       <font name="Header 1" family="Liberation Sans" style="BOLD" size="22.0">
       </font>
```

### Comparing `ibek-3.4.0b2/tests/samples/schemas/ibek.support.schema.json` & `ibek-3.5.0b1/tests/samples/schemas/ibek.support.schema.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9862788865546219%*

 * *Differences: {"'$defs'": "{'EntityDefinition': OrderedDict([('additionalProperties', False), ('description', 'A "*

 * *            "single definition of a class of Entity that an IOC instance may instantiate'), "*

 * *            "('properties', OrderedDict([('name', OrderedDict([('description', 'Publish Definition "*

 * *            "as type <module>.<name> for IOC instances'), ('title', 'Name'), ('type', "*

 * *            "'string')])), ('description', OrderedDict([('description', 'A description of the "*

 * *            "Support module defi […]*

```diff
@@ -101,15 +101,15 @@
             "required": [
                 "file",
                 "args"
             ],
             "title": "Database",
             "type": "object"
         },
-        "Definition": {
+        "EntityDefinition": {
             "additionalProperties": false,
             "description": "A single definition of a class of Entity that an IOC instance may instantiate",
             "properties": {
                 "args": {
                     "default": [],
                     "description": "The arguments IOC instance should supply",
                     "items": {
@@ -197,37 +197,56 @@
                             }
                         ]
                     },
                     "title": "Pre Init",
                     "type": "array"
                 },
                 "pvi": {
-                    "allOf": [
+                    "anyOf": [
                         {
                             "$ref": "#/$defs/EntityPVI"
+                        },
+                        {
+                            "type": "null"
                         }
                     ],
                     "default": null,
                     "description": "PVI definition for Entity"
                 },
+                "shared": {
+                    "default": [],
+                    "description": "A place to create any anchors required for repeating YAML",
+                    "items": {},
+                    "title": "Shared",
+                    "type": "array"
+                },
+                "sub_entities": {
+                    "default": [],
+                    "description": "The sub-entity instances that this collection is to instantiate",
+                    "items": {
+                        "$ref": "#/$defs/SubEntity"
+                    },
+                    "title": "Sub Entities",
+                    "type": "array"
+                },
                 "values": {
                     "default": [],
-                    "description": "The values IOC instance should supply",
+                    "description": "Calculated values to use as additional arguments",
                     "items": {
                         "$ref": "#/$defs/Value"
                     },
                     "title": "Values",
                     "type": "array"
                 }
             },
             "required": [
                 "name",
                 "description"
             ],
-            "title": "Definition",
+            "title": "EntityDefinition",
             "type": "object"
         },
         "EntityPVI": {
             "additionalProperties": false,
             "description": "Entity PVI definition",
             "properties": {
                 "pv": {
@@ -532,14 +551,36 @@
             "required": [
                 "name",
                 "description"
             ],
             "title": "StrArg",
             "type": "object"
         },
+        "SubEntity": {
+            "additionalProperties": true,
+            "description": "A loosely defined class to declare the Entities\nin an ibek.support.yaml file in the 'sub_entities' property of an Entity\nsection",
+            "properties": {
+                "entity_enabled": {
+                    "default": true,
+                    "description": "enable or disable this entity instance",
+                    "title": "Entity Enabled",
+                    "type": "boolean"
+                },
+                "type": {
+                    "description": "The type of this entity",
+                    "title": "Type",
+                    "type": "string"
+                }
+            },
+            "required": [
+                "type"
+            ],
+            "title": "SubEntity",
+            "type": "object"
+        },
         "Text": {
             "additionalProperties": false,
             "description": "A script snippet to insert into the startup script",
             "properties": {
                 "type": {
                     "const": "text",
                     "default": "text",
@@ -601,15 +642,15 @@
     },
     "additionalProperties": false,
     "description": "Lists the definitions for a support module, this defines what Entities it supports\n\nProvides the deserialize entry point.",
     "properties": {
         "defs": {
             "description": "The definitions an IOC can create using this module",
             "items": {
-                "$ref": "#/$defs/Definition"
+                "$ref": "#/$defs/EntityDefinition"
             },
             "title": "Defs",
             "type": "array"
         },
         "module": {
             "description": "Support module name, normally the repo name",
             "title": "Module",
```

### Comparing `ibek-3.4.0b2/tests/samples/schemas/motorSim.ibek.ioc.schema.json` & `ibek-3.5.0b1/tests/samples/schemas/motorSim.ibek.ioc.schema.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999920083774251%*

 * *Differences: {"'$defs'": "{'asyn_AsynIP': {'properties': {'type': {'description': 'Asyn IP Port'}}}, "*

 * *            "'motorSim_simMotorAxis': {'properties': {'type': {'description': 'Creates a "*

 * *            "simulation motor axis'}}}, 'motorSim_simMotorController': {'properties': {'type': "*

 * *            "{'description': 'Creates a simulation motion controller'}}}}"}*

```diff
@@ -107,15 +107,15 @@
                     ],
                     "default": "1",
                     "description": "Stop Bits"
                 },
                 "type": {
                     "const": "asyn.AsynIP",
                     "default": "asyn.AsynIP",
-                    "description": "The type of this entity",
+                    "description": "Asyn IP Port",
                     "title": "Type"
                 }
             },
             "required": [
                 "port",
                 "name"
             ],
@@ -233,15 +233,15 @@
                     "description": "The starting position of the axis (in counts)",
                     "title": "Start",
                     "type": "string"
                 },
                 "type": {
                     "const": "motorSim.simMotorAxis",
                     "default": "motorSim.simMotorAxis",
-                    "description": "The type of this entity",
+                    "description": "Creates a simulation motor axis",
                     "title": "Type"
                 }
             },
             "required": [
                 "controller",
                 "M",
                 "ADDR"
@@ -282,15 +282,15 @@
                 "port": {
                     "description": "a reference to the asyn port for communication with the controller",
                     "title": "Port"
                 },
                 "type": {
                     "const": "motorSim.simMotorController",
                     "default": "motorSim.simMotorController",
-                    "description": "The type of this entity",
+                    "description": "Creates a simulation motion controller",
                     "title": "Type"
                 }
             },
             "required": [
                 "controllerName",
                 "P",
                 "numAxes",
```

### Comparing `ibek-3.4.0b2/tests/samples/schemas/single.ibek.ioc.schema.json` & `ibek-3.5.0b1/tests/samples/schemas/single.ibek.ioc.schema.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999818121693123%*

 * *Differences: {"'$defs'": "{'motorSim_simMotorAxis': {'properties': {'type': {'description': 'Creates a "*

 * *            "simulation motor axis'}}}, 'motorSim_simMotorController': {'properties': {'type': "*

 * *            "{'description': 'Creates a simulation motion controller'}}}}"}*

```diff
@@ -93,15 +93,15 @@
                     "description": "The starting position of the axis (in counts)",
                     "title": "Start",
                     "type": "string"
                 },
                 "type": {
                     "const": "motorSim.simMotorAxis",
                     "default": "motorSim.simMotorAxis",
-                    "description": "The type of this entity",
+                    "description": "Creates a simulation motor axis",
                     "title": "Type"
                 }
             },
             "required": [
                 "controller",
                 "M",
                 "ADDR"
@@ -142,15 +142,15 @@
                 "port": {
                     "description": "a reference to the asyn port for communication with the controller",
                     "title": "Port"
                 },
                 "type": {
                     "const": "motorSim.simMotorController",
                     "default": "motorSim.simMotorController",
-                    "description": "The type of this entity",
+                    "description": "Creates a simulation motion controller",
                     "title": "Type"
                 }
             },
             "required": [
                 "controllerName",
                 "P",
                 "numAxes",
```

### Comparing `ibek-3.4.0b2/tests/samples/schemas/utils.ibek.ioc.schema.json` & `ibek-3.5.0b1/tests/samples/schemas/utils.ibek.ioc.schema.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999305555555557%*

 * *Differences: {"'$defs'": "{'epics_InterruptVectorVME': {'properties': {'type': {'description': 'Reserve an "*

 * *            "interrupt vector for use with VME hardware.\\n'}}}, 'epics_InterruptVectorVME2': "*

 * *            "{'properties': {'type': {'description': 'naughty second use of same counter'}}}}"}*

```diff
@@ -25,15 +25,15 @@
                     "description": "test global variable setter",
                     "title": "Test Global Var",
                     "type": "string"
                 },
                 "type": {
                     "const": "epics.InterruptVectorVME",
                     "default": "epics.InterruptVectorVME",
-                    "description": "The type of this entity",
+                    "description": "Reserve an interrupt vector for use with VME hardware.\n",
                     "title": "Type"
                 }
             },
             "required": [
                 "name"
             ],
             "title": "epics_InterruptVectorVME",
@@ -52,15 +52,15 @@
                     "description": "A name for an interrupt vector variable",
                     "title": "Name",
                     "type": "string"
                 },
                 "type": {
                     "const": "epics.InterruptVectorVME2",
                     "default": "epics.InterruptVectorVME2",
-                    "description": "The type of this entity",
+                    "description": "naughty second use of same counter",
                     "title": "Type"
                 }
             },
             "required": [
                 "name"
             ],
             "title": "epics_InterruptVectorVME2",
```

### Comparing `ibek-3.4.0b2/tests/samples/support/asyn.ibek.support.yaml` & `ibek-3.5.0b1/tests/samples/support/asyn.ibek.support.yaml`

 * *Files identical despite different names*

### Comparing `ibek-3.4.0b2/tests/samples/support/bad_db.ibek.support.yaml` & `ibek-3.5.0b1/tests/samples/support/bad_db.ibek.support.yaml`

 * *Files identical despite different names*

### Comparing `ibek-3.4.0b2/tests/samples/support/motorSim.ibek.support.yaml` & `ibek-3.5.0b1/tests/samples/support/motorSim.ibek.support.yaml`

 * *Files identical despite different names*

### Comparing `ibek-3.4.0b2/tests/samples/support/utils.ibek.support.yaml` & `ibek-3.5.0b1/tests/samples/support/utils.ibek.support.yaml`

 * *Files identical despite different names*

### Comparing `ibek-3.4.0b2/tests/sys-test.sh` & `ibek-3.5.0b1/tests/sys-test.sh`

 * *Files identical despite different names*

### Comparing `ibek-3.4.0b2/tests/test_cli.py` & `ibek-3.5.0b1/tests/test_cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 """
 System tests that run the CLI commands and compare the output to expected
 results.
 """
 
 import json
-import os
 import subprocess
 import sys
 from pathlib import Path
 
 from pytest_mock import MockerFixture
 
+import ibek.utils as utils
 from ibek import __version__
 from ibek.globals import (
     GLOBALS,
     PVI_YAML_PATTERN,
     SUPPORT_YAML_PATTERN,
 )
-from ibek.ioc import clear_entity_model_ids
 from ibek.runtime_cmds.commands import generate
 from ibek.support_cmds.commands import generate_links
 from tests.conftest import run_cli
 
 
 def test_cli_version():
     cmd = [sys.executable, "-m", "ibek", "--version"]
@@ -38,30 +37,30 @@
 
     actual = json.loads((schema_path).read_text())
     assert expected == actual
 
 
 def test_single_schema(tmp_path: Path, samples: Path):
     """generate schema from a support module definition yaml"""
-    clear_entity_model_ids()
 
     schema_path = tmp_path / "single.ibek.support.schema.json"
     yaml_path = samples / "support" / "motorSim.ibek.support.yaml"
-    run_cli("ioc", "generate-schema", yaml_path, "--output", schema_path)
+    run_cli(
+        "ioc", "generate-schema", "--no-ibek-defs", yaml_path, "--output", schema_path
+    )
 
     expected = json.loads(
         (samples / "schemas" / "single.ibek.ioc.schema.json").read_text()
     )
 
     actual = json.loads((schema_path).read_text())
     assert expected == actual
 
 
 def test_motor_sim_schema(tmp_path: Path, samples: Path):
-    clear_entity_model_ids()
     """generate schema for a container with two support modules"""
 
     schema_combined = tmp_path / "motorSim.ibek.ioc.schema.json"
     yaml_path1 = samples / "support" / "asyn.ibek.support.yaml"
     yaml_path2 = samples / "support" / "motorSim.ibek.support.yaml"
     run_cli(
         "ioc",
@@ -77,83 +76,130 @@
         (samples / "schemas" / "motorSim.ibek.ioc.schema.json").read_text()
     )
 
     actual = json.loads((schema_combined).read_text())
     assert expected == actual
 
 
-def test_build_runtime_motorSim(mocker: MockerFixture, tmp_path: Path, samples: Path):
+def test_build_runtime_motorSim(epics_root: Path, samples: Path):
     """
     build an ioc runtime script from an IOC instance entity file
     and multiple support module definition files
 
     Also verifies database subst file generation for multiple
     entity instantiations.
     """
-    clear_entity_model_ids()
     ioc_yaml = samples / "iocs" / "ibek-mo-ioc-01.yaml"
     support_yaml1 = samples / "support" / "asyn.ibek.support.yaml"
     support_yaml2 = samples / "support" / "motorSim.ibek.support.yaml"
     expected_outputs = samples / "outputs" / "motorSim"
 
-    mocker.patch.object(GLOBALS, "RUNTIME_OUTPUT", tmp_path)
-    mocker.patch.object(GLOBALS, "OPI_OUTPUT", tmp_path)
-
-    os.environ["IOC"] = "/epics/ioc"
-    os.environ["RUNTIME_DIR"] = "/epics/runtime"
     generate(ioc_yaml, [support_yaml1, support_yaml2])
 
     example_boot = (expected_outputs / "st.cmd").read_text()
-    actual_boot = (tmp_path / "st.cmd").read_text()
+    actual_boot = (epics_root / "runtime" / "st.cmd").read_text()
     assert example_boot == actual_boot
 
     example_db = (expected_outputs / "ioc.subst").read_text()
-    actual_db = (tmp_path / "ioc.subst").read_text()
+    actual_db = (epics_root / "runtime" / "ioc.subst").read_text()
     assert example_db == actual_db
 
     example_index = (expected_outputs / "index.bob").read_text()
-    actual_index = (tmp_path / "index.bob").read_text()
+    actual_index = (epics_root / "opi" / "index.bob").read_text()
     assert example_index == actual_index
 
     example_bob = (expected_outputs / "simple.pvi.bob").read_text()
-    actual_bob = (tmp_path / "simple.pvi.bob").read_text()
+    actual_bob = (epics_root / "opi" / "simple.pvi.bob").read_text()
     assert example_bob == actual_bob
 
     example_template = (expected_outputs / "simple.pvi.template").read_text()
-    actual_template = (tmp_path / "simple.pvi.template").read_text()
+    actual_template = (epics_root / "runtime" / "simple.pvi.template").read_text()
     assert example_template == actual_template
 
 
-def test_build_utils_features(mocker: MockerFixture, tmp_path: Path, samples: Path):
+def test_build_utils_features(epics_root: Path, samples: Path):
     """
     build an ioc runtime script to verify utils features
     """
-    clear_entity_model_ids()
     ioc_yaml = samples / "iocs" / "utils.ibek.ioc.yaml"
     support_yaml = samples / "support" / "utils.ibek.support.yaml"
 
-    mocker.patch.object(GLOBALS, "RUNTIME_OUTPUT", tmp_path)
-
-    os.environ["IOC"] = "/epics/ioc"
-    os.environ["RUNTIME_DIR"] = "/epics/runtime"
     run_cli("runtime", "generate", ioc_yaml, support_yaml)
 
     example_boot = (samples / "outputs" / "utils" / "st.cmd").read_text()
-    actual_boot = (tmp_path / "st.cmd").read_text()
+    actual_boot = (epics_root / "runtime" / "st.cmd").read_text()
     assert example_boot == actual_boot
 
     example_db = (samples / "outputs" / "utils" / "ioc.subst").read_text()
-    actual_db = (tmp_path / "ioc.subst").read_text()
+    actual_db = (epics_root / "runtime" / "ioc.subst").read_text()
     assert example_db == actual_db
 
 
 def test_generate_links_ibek(samples: Path, mocker: MockerFixture):
     symlink_mock = mocker.patch("ibek.support_cmds.commands.symlink_files")
 
     generate_links(samples / "support")
 
     symlink_mock.assert_any_call(
         samples / "support", PVI_YAML_PATTERN, GLOBALS.PVI_DEFS
     )
     symlink_mock.assert_any_call(
         samples / "support", SUPPORT_YAML_PATTERN, GLOBALS.IBEK_DEFS
     )
+
+
+def test_ipac(epics_root: Path, samples: Path):
+    """
+    Tests that an id argument can include another argument in its default value
+    """
+
+    ioc_yaml = samples / "iocs" / "ipac-test.yaml"
+    support_yaml1 = samples / "support" / "ipac.ibek.support.yaml"
+    support_yaml2 = samples / "support" / "epics.ibek.support.yaml"
+    expected_outputs = samples / "outputs" / "ipac"
+
+    # reset the InterruptVector counter to its initial state (if already used)
+    if "InterruptVector" in utils.UTILS.counters:
+        utils.UTILS.counters["InterruptVector"].current = 192
+
+    generate(ioc_yaml, [support_yaml1, support_yaml2])
+
+    example_boot = (expected_outputs / "st.cmd").read_text()
+    actual_boot = (epics_root / "runtime" / "st.cmd").read_text()
+    assert example_boot == actual_boot
+
+
+def test_gauges(epics_root: Path, samples: Path):
+    """
+    Tests that an id argument can include another argument in its default value
+    """
+    ioc_yaml = samples / "iocs" / "gauges.ibek.ioc.yaml"
+    support_yaml1 = samples / "support" / "asyn.ibek.support.yaml"
+    support_yaml2 = samples / "support" / "gauges.ibek.support.yaml"
+    expected_outputs = samples / "outputs" / "gauges"
+
+    generate(ioc_yaml, [support_yaml1, support_yaml2])
+
+    example_boot = (expected_outputs / "st.cmd").read_text()
+    actual_boot = (epics_root / "runtime" / "st.cmd").read_text()
+    assert example_boot == actual_boot
+
+
+def test_quadem(epics_root: Path, samples: Path):
+    """
+    Tests the use of CollectionDefinitions in an IOC instance
+    this example uses the tetramm beam position monitor module
+    """
+    ioc_yaml = samples / "iocs" / "quadem.ibek.ioc.yaml"
+    support_yaml1 = samples / "support" / "ADCore.ibek.support.yaml"
+    support_yaml2 = samples / "support" / "quadem.ibek.support.yaml"
+    expected_outputs = samples / "outputs" / "quadem"
+
+    generate(ioc_yaml, [support_yaml1, support_yaml2])
+
+    example_boot = (expected_outputs / "st.cmd").read_text()
+    actual_boot = (epics_root / "runtime" / "st.cmd").read_text()
+    assert example_boot == actual_boot
+
+    example_db = (samples / "outputs" / "quadem" / "ioc.subst").read_text()
+    actual_db = (epics_root / "runtime" / "ioc.subst").read_text()
+    assert example_db == actual_db
```

### Comparing `ibek-3.4.0b2/tests/test_error.py` & `ibek-3.5.0b1/tests/test_error.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 """
 
 from pathlib import Path
 
 import pytest
 from ruamel.yaml import YAML
 
-from ibek.ioc import clear_entity_model_ids, make_entity_models, make_ioc_model
+from ibek.ioc_factory import IocFactory
 from ibek.support import Support
 from ibek.utils import UTILS
 from tests.conftest import run_cli
 
 
-def test_counter_reuse(tmp_path: Path, samples: Path):
+def test_counter_reuse(epics_root: Path, samples: Path):
     """
     Check you cannot redefine a counter with the same name and different params
     """
     UTILS.__reset__()
 
     entity_file = samples / "iocs" / "bad_counter.ibek.ioc.yaml"
     definition_file1 = samples / "support" / "utils.ibek.support.yaml"
@@ -26,89 +26,86 @@
         run_cli("runtime", "generate", entity_file, definition_file1)
     assert (
         str(ctx.value)
         == "Redefining counter InterruptVector with different start/stop values"
     )
 
 
-def test_counter_overuse(tmp_path: Path, samples: Path):
+def test_counter_overuse(epics_root: Path, samples: Path):
     """
     Check that counter limits are enforced
     """
     UTILS.__reset__()
 
     entity_file = samples / "iocs" / "bad_counter2.ibek.ioc.yaml"
     definition_file1 = samples / "support" / "utils.ibek.support.yaml"
 
     with pytest.raises(ValueError) as ctx:
         run_cli("runtime", "generate", entity_file, definition_file1)
-    assert str(ctx.value) == "Counter 195 exceeded stop value of 194"
 
+    assert "Counter 195 exceeded stop value of 194" in str(ctx.value)
 
-def test_bad_ref(tmp_path: Path, samples: Path):
+
+def test_bad_ref(samples: Path):
     """
     Check bad object references are caught
     """
     UTILS.__reset__()
 
     entity_file = samples / "iocs" / "bad_ref.ibek.ioc.yaml"
     definition_file1 = samples / "support" / "asyn.ibek.support.yaml"
     definition_file2 = samples / "support" / "motorSim.ibek.support.yaml"
 
     with pytest.raises(ValueError) as ctx:
         run_cli("runtime", "generate", entity_file, definition_file1, definition_file2)
     assert "object controllerOnePort_BAD_REF not found" in str(ctx.value)
 
 
-def test_bad_db(tmp_path: Path, samples: Path):
+def test_bad_db(epics_root: Path, samples: Path):
     """
     Check bad database args are caught
     """
     UTILS.__reset__()
 
     entity_file = samples / "iocs" / "bad_db.ibek.ioc.yaml"
     definition_file1 = samples / "support" / "bad_db.ibek.support.yaml"
 
     with pytest.raises(ValueError) as ctx:
         run_cli("runtime", "generate", entity_file, definition_file1)
     assert "'non-existant' in database template 'test.db' not found" in str(ctx.value)
 
 
-def test_loading_module_twice(tmp_path: Path, samples: Path):
+def test_loading_module_twice(entity_factory, samples: Path):
     """
     Verify we get a sensible error if we try to load a module twice
     without clearing the entity model ids
     """
-
-    clear_entity_model_ids()
-
     definition_file = samples / "support" / "utils.ibek.support.yaml"
     instance_file = samples / "iocs" / "utils.ibek.ioc.yaml"
 
     support = Support(**YAML(typ="safe").load(definition_file))
-    entities1 = make_entity_models(support)
-    entities2 = make_entity_models(support)
+    entities1 = entity_factory._make_entity_models(support)
+    entities2 = entity_factory._make_entity_models(support)
 
-    generic_ioc1 = make_ioc_model(entities1)
-    generic_ioc2 = make_ioc_model(entities2)
+    ioc_factory = IocFactory()
+    generic_ioc1 = ioc_factory.make_ioc_model(entities1)
+    generic_ioc2 = ioc_factory.make_ioc_model(entities2)
 
     instance = YAML(typ="safe").load(instance_file)
     generic_ioc1(**instance)
     with pytest.raises(ValueError) as ctx:
         generic_ioc2(**instance)
 
     assert "Duplicate id" in str(ctx.value)
 
 
 def test_defaults(tmp_path: Path, samples: Path):
     """
     Check you cannot redefine a counter with the same name and different params
     """
-
-    clear_entity_model_ids()
     entity_file = samples / "iocs" / "bad_default.ibek.ioc.yaml"
     definition_file1 = samples / "support" / "asyn.ibek.support.yaml"
 
     with pytest.raises(ValueError) as ctx:
         run_cli("runtime", "generate", entity_file, definition_file1)
 
     assert "Field required [type=missing" in str(ctx.value)
```

### Comparing `ibek-3.4.0b2/tests/test_render.py` & `ibek-3.5.0b1/tests/test_render.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 Unit tests for the rendering of scripts and database entries from generated
 Entity classes
 """
 
 from typing import Literal
 
-from ibek.ioc import IOC, clear_entity_model_ids
 from ibek.render import Render
 from ibek.render_db import RenderDb
 
 
 def find_entity_class(entity_classes, entity_type):
     for entity_class in entity_classes:
         literal = Literal[entity_type]  # type: ignore
@@ -76,23 +75,17 @@
         port="asyn1", controllerName="ctrl1", P="IBEK-MO-01:", numAxes=4, DESC="test"
     )
     motor1 = motor_def(controller="ctrl1", M="M1", ADDR=1)
     motor2 = motor_def(controller="ctrl1", M="M2", ADDR=2, is_cs=True)
 
     # make a dummy IOC with two entities as database render works against
     # a whole IOC rather than a single entity at a time.
-    clear_entity_model_ids()
+    entities = [asyn1, sim_motor, motor1, motor2]
 
-    ioc = IOC(
-        ioc_name="test_ioc",
-        description="for testing",
-        entities=[asyn1, sim_motor, motor1, motor2],
-    )
-
-    render_db = RenderDb(ioc)
+    render_db = RenderDb(entities)
     templates = render_db.render_database()
 
     assert templates == {
         "basic_asyn_motor.db": [
             '"P",           "M",  "DTYP",      "PORT",  "ADDR", "DESC",    "EGU",     "DIR", "VELO", "VMAX", "MRES", "DHLM",  "DLLM",   "INIT"',
             '"IBEK-MO-01:", "M1", "asynMotor", "ctrl1", "1",    "Motor 1", "degrees", "0",   "10.0", "10.0", ".01",  "20000", "-20000", ""    ',
         ],
```

