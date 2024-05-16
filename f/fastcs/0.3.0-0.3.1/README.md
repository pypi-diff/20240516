# Comparing `tmp/fastcs-0.3.0.tar.gz` & `tmp/fastcs-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastcs-0.3.0.tar", last modified: Fri Apr 12 15:21:56 2024, max compression
+gzip compressed data, was "fastcs-0.3.1.tar", last modified: Thu May 16 10:31:23 2024, max compression
```

## Comparing `fastcs-0.3.0.tar` & `fastcs-0.3.1.tar`

### file list

```diff
@@ -1,95 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:21:56.916255 fastcs-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-12 15:21:49.000000 fastcs-0.3.0/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:21:56.904255 fastcs-0.3.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-12 15:21:49.000000 fastcs-0.3.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:21:56.904255 fastcs-0.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-12 15:21:49.000000 fastcs-0.3.0/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:21:56.900255 fastcs-0.3.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:21:56.904255 fastcs-0.3.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-12 15:21:49.000000 fastcs-0.3.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-12 15:21:49.000000 fastcs-0.3.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:21:56.904255 fastcs-0.3.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-12 15:21:49.000000 fastcs-0.3.0/.github/pages/index.html
--rwxr-xr-x   0 runner    (1001) docker     (127)     2889 2024-04-12 15:21:49.000000 fastcs-0.3.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:21:56.904255 fastcs-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-12 15:21:49.000000 fastcs-0.3.0/.github/workflows/_check.yml
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-12 15:21:49.000000 fastcs-0.3.0/.github/workflows/_dist.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-12 15:21:49.000000 fastcs-0.3.0/.github/workflows/_docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-12 15:21:49.000000 fastcs-0.3.0/.github/workflows/_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-12 15:21:49.000000 fastcs-0.3.0/.github/workflows/_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-12 15:21:49.000000 fastcs-0.3.0/.github/workflows/_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-12 15:21:49.000000 fastcs-0.3.0/.github/workflows/_tox.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-12 15:21:49.000000 fastcs-0.3.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-12 15:21:49.000000 fastcs-0.3.0/.github/workflows/periodic.yml
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-12 15:21:49.000000 fastcs-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-12 15:21:49.000000 fastcs-0.3.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:21:56.908255 fastcs-0.3.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-12 15:21:49.000000 fastcs-0.3.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-12 15:21:49.000000 fastcs-0.3.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-12 15:21:49.000000 fastcs-0.3.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-12 15:21:49.000000 fastcs-0.3.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-12 15:21:49.000000 fastcs-0.3.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-12 15:21:49.000000 fastcs-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15544 2024-04-12 15:21:56.916255 fastcs-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-12 15:21:49.000000 fastcs-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-12 15:21:49.000000 fastcs-0.3.0/catalog-info.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:21:56.908255 fastcs-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6214 2024-04-12 15:21:49.000000 fastcs-0.3.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:21:56.908255 fastcs-0.3.0/docs/explanations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:21:56.908255 fastcs-0.3.0/docs/explanations/decisions/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-12 15:21:49.000000 fastcs-0.3.0/docs/explanations/decisions/0001-record-architecture-decisions.md
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-12 15:21:49.000000 fastcs-0.3.0/docs/explanations/decisions/0002-switched-to-python-copier-template.md
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-12 15:21:49.000000 fastcs-0.3.0/docs/explanations/decisions/COPYME
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-12 15:21:49.000000 fastcs-0.3.0/docs/explanations/decisions.md
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-12 15:21:49.000000 fastcs-0.3.0/docs/explanations.md
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-12 15:21:49.000000 fastcs-0.3.0/docs/genindex.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:21:56.908255 fastcs-0.3.0/docs/how-to/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-12 15:21:49.000000 fastcs-0.3.0/docs/how-to/contribute.md
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-12 15:21:49.000000 fastcs-0.3.0/docs/how-to.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:21:56.908255 fastcs-0.3.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-12 15:21:49.000000 fastcs-0.3.0/docs/images/fastcs.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-12 15:21:49.000000 fastcs-0.3.0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:21:56.908255 fastcs-0.3.0/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-12 15:21:49.000000 fastcs-0.3.0/docs/reference/api.md
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-12 15:21:49.000000 fastcs-0.3.0/docs/reference.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:21:56.908255 fastcs-0.3.0/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-12 15:21:49.000000 fastcs-0.3.0/docs/tutorials/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-12 15:21:49.000000 fastcs-0.3.0/docs/tutorials.md
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-12 15:21:49.000000 fastcs-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 15:21:56.916255 fastcs-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:21:56.900255 fastcs-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:21:56.912255 fastcs-0.3.0/src/fastcs/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-12 15:21:49.000000 fastcs-0.3.0/src/fastcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-12 15:21:49.000000 fastcs-0.3.0/src/fastcs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-12 15:21:56.000000 fastcs-0.3.0/src/fastcs/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-04-12 15:21:49.000000 fastcs-0.3.0/src/fastcs/attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-04-12 15:21:49.000000 fastcs-0.3.0/src/fastcs/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:21:56.912255 fastcs-0.3.0/src/fastcs/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-12 15:21:49.000000 fastcs-0.3.0/src/fastcs/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-12 15:21:49.000000 fastcs-0.3.0/src/fastcs/backends/asyncio_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:21:56.912255 fastcs-0.3.0/src/fastcs/backends/epics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 15:21:49.000000 fastcs-0.3.0/src/fastcs/backends/epics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-12 15:21:49.000000 fastcs-0.3.0/src/fastcs/backends/epics/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-12 15:21:49.000000 fastcs-0.3.0/src/fastcs/backends/epics/docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-04-12 15:21:49.000000 fastcs-0.3.0/src/fastcs/backends/epics/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-04-12 15:21:49.000000 fastcs-0.3.0/src/fastcs/backends/epics/ioc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:21:56.912255 fastcs-0.3.0/src/fastcs/connections/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-12 15:21:49.000000 fastcs-0.3.0/src/fastcs/connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-12 15:21:49.000000 fastcs-0.3.0/src/fastcs/connections/ip_connection.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1645 2024-04-12 15:21:49.000000 fastcs-0.3.0/src/fastcs/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-12 15:21:49.000000 fastcs-0.3.0/src/fastcs/cs_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-12 15:21:49.000000 fastcs-0.3.0/src/fastcs/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-12 15:21:49.000000 fastcs-0.3.0/src/fastcs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-12 15:21:49.000000 fastcs-0.3.0/src/fastcs/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-12 15:21:49.000000 fastcs-0.3.0/src/fastcs/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:21:56.912255 fastcs-0.3.0/src/fastcs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15544 2024-04-12 15:21:56.000000 fastcs-0.3.0/src/fastcs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-12 15:21:56.000000 fastcs-0.3.0/src/fastcs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 15:21:56.000000 fastcs-0.3.0/src/fastcs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-12 15:21:56.000000 fastcs-0.3.0/src/fastcs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-12 15:21:56.000000 fastcs-0.3.0/src/fastcs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 15:21:56.000000 fastcs-0.3.0/src/fastcs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:21:56.912255 fastcs-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-12 15:21:49.000000 fastcs-0.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-12 15:21:49.000000 fastcs-0.3.0/tests/test_boilerplate_removed.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-12 15:21:49.000000 fastcs-0.3.0/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:31:23.009618 fastcs-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-16 10:31:18.000000 fastcs-0.3.1/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:31:22.997618 fastcs-0.3.1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-16 10:31:18.000000 fastcs-0.3.1/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:31:22.997618 fastcs-0.3.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-16 10:31:18.000000 fastcs-0.3.1/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:31:22.997618 fastcs-0.3.1/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:31:23.001618 fastcs-0.3.1/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-16 10:31:18.000000 fastcs-0.3.1/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-16 10:31:18.000000 fastcs-0.3.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:31:23.001618 fastcs-0.3.1/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-16 10:31:18.000000 fastcs-0.3.1/.github/pages/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2889 2024-05-16 10:31:18.000000 fastcs-0.3.1/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:31:23.001618 fastcs-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-16 10:31:18.000000 fastcs-0.3.1/.github/workflows/_check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-16 10:31:18.000000 fastcs-0.3.1/.github/workflows/_dist.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-16 10:31:18.000000 fastcs-0.3.1/.github/workflows/_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-16 10:31:18.000000 fastcs-0.3.1/.github/workflows/_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-16 10:31:18.000000 fastcs-0.3.1/.github/workflows/_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-16 10:31:18.000000 fastcs-0.3.1/.github/workflows/_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-16 10:31:18.000000 fastcs-0.3.1/.github/workflows/_tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-16 10:31:18.000000 fastcs-0.3.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-16 10:31:18.000000 fastcs-0.3.1/.github/workflows/periodic.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-16 10:31:18.000000 fastcs-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-16 10:31:18.000000 fastcs-0.3.1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:31:23.001618 fastcs-0.3.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-16 10:31:18.000000 fastcs-0.3.1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-16 10:31:18.000000 fastcs-0.3.1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-16 10:31:18.000000 fastcs-0.3.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-16 10:31:18.000000 fastcs-0.3.1/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-16 10:31:18.000000 fastcs-0.3.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-16 10:31:18.000000 fastcs-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15544 2024-05-16 10:31:23.009618 fastcs-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-16 10:31:18.000000 fastcs-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-16 10:31:18.000000 fastcs-0.3.1/catalog-info.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:31:23.001618 fastcs-0.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6214 2024-05-16 10:31:18.000000 fastcs-0.3.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:31:23.001618 fastcs-0.3.1/docs/explanations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:31:23.001618 fastcs-0.3.1/docs/explanations/decisions/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-16 10:31:18.000000 fastcs-0.3.1/docs/explanations/decisions/0001-record-architecture-decisions.md
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-16 10:31:18.000000 fastcs-0.3.1/docs/explanations/decisions/0002-switched-to-python-copier-template.md
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-16 10:31:18.000000 fastcs-0.3.1/docs/explanations/decisions/COPYME
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-16 10:31:18.000000 fastcs-0.3.1/docs/explanations/decisions.md
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-16 10:31:18.000000 fastcs-0.3.1/docs/explanations.md
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-16 10:31:18.000000 fastcs-0.3.1/docs/genindex.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:31:23.001618 fastcs-0.3.1/docs/how-to/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-16 10:31:18.000000 fastcs-0.3.1/docs/how-to/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-16 10:31:18.000000 fastcs-0.3.1/docs/how-to.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:31:23.005618 fastcs-0.3.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-16 10:31:18.000000 fastcs-0.3.1/docs/images/fastcs.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-16 10:31:18.000000 fastcs-0.3.1/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:31:23.005618 fastcs-0.3.1/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-16 10:31:18.000000 fastcs-0.3.1/docs/reference/api.md
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-16 10:31:18.000000 fastcs-0.3.1/docs/reference.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:31:23.005618 fastcs-0.3.1/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-16 10:31:18.000000 fastcs-0.3.1/docs/tutorials/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-16 10:31:18.000000 fastcs-0.3.1/docs/tutorials.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-16 10:31:18.000000 fastcs-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 10:31:23.009618 fastcs-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:31:22.997618 fastcs-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:31:23.005618 fastcs-0.3.1/src/fastcs/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-16 10:31:18.000000 fastcs-0.3.1/src/fastcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-16 10:31:18.000000 fastcs-0.3.1/src/fastcs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-16 10:31:22.000000 fastcs-0.3.1/src/fastcs/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-05-16 10:31:18.000000 fastcs-0.3.1/src/fastcs/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-05-16 10:31:18.000000 fastcs-0.3.1/src/fastcs/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:31:23.005618 fastcs-0.3.1/src/fastcs/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-16 10:31:18.000000 fastcs-0.3.1/src/fastcs/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-16 10:31:18.000000 fastcs-0.3.1/src/fastcs/backends/asyncio_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:31:23.009618 fastcs-0.3.1/src/fastcs/backends/epics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 10:31:18.000000 fastcs-0.3.1/src/fastcs/backends/epics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-16 10:31:18.000000 fastcs-0.3.1/src/fastcs/backends/epics/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-16 10:31:18.000000 fastcs-0.3.1/src/fastcs/backends/epics/docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5837 2024-05-16 10:31:18.000000 fastcs-0.3.1/src/fastcs/backends/epics/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-05-16 10:31:18.000000 fastcs-0.3.1/src/fastcs/backends/epics/ioc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:31:23.009618 fastcs-0.3.1/src/fastcs/connections/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-16 10:31:18.000000 fastcs-0.3.1/src/fastcs/connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-16 10:31:18.000000 fastcs-0.3.1/src/fastcs/connections/ip_connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1645 2024-05-16 10:31:18.000000 fastcs-0.3.1/src/fastcs/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-16 10:31:18.000000 fastcs-0.3.1/src/fastcs/cs_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-16 10:31:18.000000 fastcs-0.3.1/src/fastcs/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-16 10:31:18.000000 fastcs-0.3.1/src/fastcs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-16 10:31:18.000000 fastcs-0.3.1/src/fastcs/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-16 10:31:18.000000 fastcs-0.3.1/src/fastcs/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-16 10:31:18.000000 fastcs-0.3.1/src/fastcs/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:31:23.009618 fastcs-0.3.1/src/fastcs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15544 2024-05-16 10:31:22.000000 fastcs-0.3.1/src/fastcs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-16 10:31:22.000000 fastcs-0.3.1/src/fastcs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 10:31:22.000000 fastcs-0.3.1/src/fastcs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-16 10:31:22.000000 fastcs-0.3.1/src/fastcs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-16 10:31:22.000000 fastcs-0.3.1/src/fastcs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-16 10:31:22.000000 fastcs-0.3.1/src/fastcs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:31:23.009618 fastcs-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-16 10:31:18.000000 fastcs-0.3.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-16 10:31:18.000000 fastcs-0.3.1/tests/test_boilerplate_removed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-16 10:31:18.000000 fastcs-0.3.1/tests/test_cli.py
```

### Comparing `fastcs-0.3.0/.copier-answers.yml` & `fastcs-0.3.1/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `fastcs-0.3.0/.devcontainer/devcontainer.json` & `fastcs-0.3.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `fastcs-0.3.0/.github/CONTRIBUTING.md` & `fastcs-0.3.1/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fastcs-0.3.0/.github/actions/install_requirements/action.yml` & `fastcs-0.3.1/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `fastcs-0.3.0/.github/dependabot.yml` & `fastcs-0.3.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `fastcs-0.3.0/.github/pages/make_switcher.py` & `fastcs-0.3.1/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `fastcs-0.3.0/.github/workflows/_check.yml` & `fastcs-0.3.1/.github/workflows/_check.yml`

 * *Files identical despite different names*

### Comparing `fastcs-0.3.0/.github/workflows/_dist.yml` & `fastcs-0.3.1/.github/workflows/_dist.yml`

 * *Files identical despite different names*

### Comparing `fastcs-0.3.0/.github/workflows/_docs.yml` & `fastcs-0.3.1/.github/workflows/_docs.yml`

 * *Files identical despite different names*

### Comparing `fastcs-0.3.0/.github/workflows/_release.yml` & `fastcs-0.3.1/.github/workflows/_release.yml`

 * *Files identical despite different names*

### Comparing `fastcs-0.3.0/.github/workflows/_test.yml` & `fastcs-0.3.1/.github/workflows/_test.yml`

 * *Files identical despite different names*

### Comparing `fastcs-0.3.0/.github/workflows/ci.yml` & `fastcs-0.3.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `fastcs-0.3.0/.gitignore` & `fastcs-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `fastcs-0.3.0/.pre-commit-config.yaml` & `fastcs-0.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fastcs-0.3.0/.vscode/launch.json` & `fastcs-0.3.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `fastcs-0.3.0/LICENSE` & `fastcs-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastcs-0.3.0/PKG-INFO` & `fastcs-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastcs
-Version: 0.3.0
+Version: 0.3.1
 Summary: Control system agnostic framework for building Device support in Python that will work for both EPICS and Tango
 Author-email: Martin Gaughran <martin.gaughran@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `fastcs-0.3.0/README.md` & `fastcs-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `fastcs-0.3.0/docs/conf.py` & `fastcs-0.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `fastcs-0.3.0/docs/explanations/decisions/0002-switched-to-python-copier-template.md` & `fastcs-0.3.1/docs/explanations/decisions/0002-switched-to-python-copier-template.md`

 * *Files identical despite different names*

### Comparing `fastcs-0.3.0/docs/images/fastcs.svg` & `fastcs-0.3.1/docs/images/fastcs.svg`

 * *Files identical despite different names*

### Comparing `fastcs-0.3.0/docs/index.md` & `fastcs-0.3.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastcs-0.3.0/docs/tutorials/installation.md` & `fastcs-0.3.1/docs/tutorials/installation.md`

 * *Files identical despite different names*

### Comparing `fastcs-0.3.0/pyproject.toml` & `fastcs-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastcs-0.3.0/src/fastcs/attributes.py` & `fastcs-0.3.1/src/fastcs/attributes.py`

 * *Files identical despite different names*

### Comparing `fastcs-0.3.0/src/fastcs/backend.py` & `fastcs-0.3.1/src/fastcs/backend.py`

 * *Files identical despite different names*

### Comparing `fastcs-0.3.0/src/fastcs/backends/asyncio_backend.py` & `fastcs-0.3.1/src/fastcs/backends/asyncio_backend.py`

 * *Files identical despite different names*

### Comparing `fastcs-0.3.0/src/fastcs/backends/epics/backend.py` & `fastcs-0.3.1/src/fastcs/backends/epics/backend.py`

 * *Files identical despite different names*

### Comparing `fastcs-0.3.0/src/fastcs/backends/epics/gui.py` & `fastcs-0.3.1/src/fastcs/backends/epics/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 )
 
 from fastcs.attributes import Attribute, AttrR, AttrRW, AttrW
 from fastcs.cs_methods import Command
 from fastcs.datatypes import Bool, DataType, Float, Int, String
 from fastcs.exceptions import FastCSException
 from fastcs.mapping import Mapping, SingleMapping
+from fastcs.util import snake_to_pascal
 
 
 class EpicsGUIFormat(Enum):
     bob = ".bob"
     edl = ".edl"
 
 
@@ -94,15 +95,15 @@
                     read_widget=read_widget,
                 )
             case AttrR():
                 read_widget = self._get_read_widget(attribute.datatype)
                 return SignalR(name=name, read_pv=pv, read_widget=read_widget)
             case AttrW():
                 write_widget = self._get_write_widget(attribute.datatype)
-                return SignalW(name=name, write_pv=pv, write_widget=TextWrite())
+                return SignalW(name=name, write_pv=pv, write_widget=write_widget)
 
     def _get_command_component(self, attr_path: str, name: str):
         pv = self._get_pv(attr_path, name)
         name = name.title().replace("_", "")
 
         return SignalX(
             name=name,
@@ -126,15 +127,15 @@
         sub_controller_mappings = self._mapping.get_controller_mappings()[1:]
 
         components = self.extract_mapping_components(controller_mapping)
 
         for sub_controller_mapping in sub_controller_mappings:
             components.append(
                 Group(
-                    name=sub_controller_mapping.controller.path,
+                    name=snake_to_pascal(sub_controller_mapping.controller.path),
                     layout=SubScreen(),
                     children=self.extract_mapping_components(sub_controller_mapping),
                 )
             )
 
         device = Device(label="Simple Device", children=components)
```

### Comparing `fastcs-0.3.0/src/fastcs/backends/epics/ioc.py` & `fastcs-0.3.1/src/fastcs/backends/epics/ioc.py`

 * *Files identical despite different names*

### Comparing `fastcs-0.3.0/src/fastcs/connections/ip_connection.py` & `fastcs-0.3.1/src/fastcs/connections/ip_connection.py`

 * *Files identical despite different names*

### Comparing `fastcs-0.3.0/src/fastcs/controller.py` & `fastcs-0.3.1/src/fastcs/controller.py`

 * *Files identical despite different names*

### Comparing `fastcs-0.3.0/src/fastcs/cs_methods.py` & `fastcs-0.3.1/src/fastcs/cs_methods.py`

 * *Files identical despite different names*

### Comparing `fastcs-0.3.0/src/fastcs/datatypes.py` & `fastcs-0.3.1/src/fastcs/datatypes.py`

 * *Files identical despite different names*

### Comparing `fastcs-0.3.0/src/fastcs/mapping.py` & `fastcs-0.3.1/src/fastcs/mapping.py`

 * *Files identical despite different names*

### Comparing `fastcs-0.3.0/src/fastcs/wrappers.py` & `fastcs-0.3.1/src/fastcs/wrappers.py`

 * *Files identical despite different names*

### Comparing `fastcs-0.3.0/src/fastcs.egg-info/PKG-INFO` & `fastcs-0.3.1/src/fastcs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastcs
-Version: 0.3.0
+Version: 0.3.1
 Summary: Control system agnostic framework for building Device support in Python that will work for both EPICS and Tango
 Author-email: Martin Gaughran <martin.gaughran@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `fastcs-0.3.0/src/fastcs.egg-info/SOURCES.txt` & `fastcs-0.3.1/src/fastcs.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 src/fastcs/attributes.py
 src/fastcs/backend.py
 src/fastcs/controller.py
 src/fastcs/cs_methods.py
 src/fastcs/datatypes.py
 src/fastcs/exceptions.py
 src/fastcs/mapping.py
+src/fastcs/util.py
 src/fastcs/wrappers.py
 src/fastcs.egg-info/PKG-INFO
 src/fastcs.egg-info/SOURCES.txt
 src/fastcs.egg-info/dependency_links.txt
 src/fastcs.egg-info/entry_points.txt
 src/fastcs.egg-info/requires.txt
 src/fastcs.egg-info/top_level.txt
```

### Comparing `fastcs-0.3.0/tests/test_boilerplate_removed.py` & `fastcs-0.3.1/tests/test_boilerplate_removed.py`

 * *Files identical despite different names*

