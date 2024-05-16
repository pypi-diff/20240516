# Comparing `tmp/twine-4.0.2.tar.gz` & `tmp/twine-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/twine/twine/dist/.tmp-_mzg2zgy/twine-4.0.2.tar", last modified: Thu Dec  1 01:47:40 2022, max compression
+gzip compressed data, was "twine-5.0.0.tar", last modified: Sun Feb 11 13:45:14 2024, max compression
```

## Comparing `twine-4.0.2.tar` & `twine-5.0.0.tar`

### file list

```diff
@@ -1,98 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 01:47:40.000000 twine-4.0.2/
--rw-r--r--   0 runner    (1001) docker     (122)       13 2022-12-01 01:46:58.000000 twine-4.0.2/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (122)      274 2022-12-01 01:46:58.000000 twine-4.0.2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (122)      496 2022-12-01 01:46:58.000000 twine-4.0.2/.flake8
--rw-r--r--   0 runner    (1001) docker     (122)      443 2022-12-01 01:46:58.000000 twine-4.0.2/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 01:47:40.000000 twine-4.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (122)      947 2022-12-01 01:46:58.000000 twine-4.0.2/.github/ISSUE_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 01:47:40.000000 twine-4.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2197 2022-12-01 01:46:58.000000 twine-4.0.2/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2703 2022-12-01 01:46:58.000000 twine-4.0.2/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1323 2022-12-01 01:46:58.000000 twine-4.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      137 2022-12-01 01:46:58.000000 twine-4.0.2/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      591 2022-12-01 01:46:58.000000 twine-4.0.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1497 2022-12-01 01:46:58.000000 twine-4.0.2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (122)     9695 2022-12-01 01:46:58.000000 twine-4.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     2930 2022-12-01 01:47:40.000000 twine-4.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1600 2022-12-01 01:46:58.000000 twine-4.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 01:47:40.000000 twine-4.0.2/changelog/
--rw-r--r--   0 runner    (1001) docker     (122)       12 2022-12-01 01:46:58.000000 twine-4.0.2/changelog/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 01:47:40.000000 twine-4.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (122)    23001 2022-12-01 01:46:58.000000 twine-4.0.2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (122)     9349 2022-12-01 01:46:58.000000 twine-4.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     9795 2022-12-01 01:46:58.000000 twine-4.0.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (122)     8944 2022-12-01 01:46:58.000000 twine-4.0.2/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 01:47:40.000000 twine-4.0.2/docs/internal/
--rw-r--r--   0 runner    (1001) docker     (122)       64 2022-12-01 01:46:58.000000 twine-4.0.2/docs/internal/twine.auth.rst
--rw-r--r--   0 runner    (1001) docker     (122)       61 2022-12-01 01:46:58.000000 twine-4.0.2/docs/internal/twine.cli.rst
--rw-r--r--   0 runner    (1001) docker     (122)       94 2022-12-01 01:46:58.000000 twine-4.0.2/docs/internal/twine.commands.check.rst
--rw-r--r--   0 runner    (1001) docker     (122)      103 2022-12-01 01:46:58.000000 twine-4.0.2/docs/internal/twine.commands.register.rst
--rw-r--r--   0 runner    (1001) docker     (122)      185 2022-12-01 01:46:58.000000 twine-4.0.2/docs/internal/twine.commands.rst
--rw-r--r--   0 runner    (1001) docker     (122)       97 2022-12-01 01:46:58.000000 twine-4.0.2/docs/internal/twine.commands.upload.rst
--rw-r--r--   0 runner    (1001) docker     (122)       82 2022-12-01 01:46:58.000000 twine-4.0.2/docs/internal/twine.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (122)       73 2022-12-01 01:46:58.000000 twine-4.0.2/docs/internal/twine.package.rst
--rw-r--r--   0 runner    (1001) docker     (122)       82 2022-12-01 01:46:58.000000 twine-4.0.2/docs/internal/twine.repository.rst
--rw-r--r--   0 runner    (1001) docker     (122)      249 2022-12-01 01:46:58.000000 twine-4.0.2/docs/internal/twine.rst
--rw-r--r--   0 runner    (1001) docker     (122)       76 2022-12-01 01:46:58.000000 twine-4.0.2/docs/internal/twine.settings.rst
--rw-r--r--   0 runner    (1001) docker     (122)       67 2022-12-01 01:46:58.000000 twine-4.0.2/docs/internal/twine.utils.rst
--rw-r--r--   0 runner    (1001) docker     (122)       67 2022-12-01 01:46:58.000000 twine-4.0.2/docs/internal/twine.wheel.rst
--rw-r--r--   0 runner    (1001) docker     (122)       73 2022-12-01 01:46:58.000000 twine-4.0.2/docs/internal/twine.wininst.rst
--rw-r--r--   0 runner    (1001) docker     (122)       99 2022-12-01 01:46:58.000000 twine-4.0.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      921 2022-12-01 01:46:58.000000 twine-4.0.2/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (122)      355 2022-12-01 01:46:58.000000 twine-4.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      292 2022-12-01 01:46:58.000000 twine-4.0.2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (122)     1714 2022-12-01 01:47:40.000000 twine-4.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 01:47:40.000000 twine-4.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-01 01:46:58.000000 twine-4.0.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 01:47:40.000000 twine-4.0.2/tests/alt-fixtures/
--rw-r--r--   0 runner    (1001) docker     (122)    15816 2022-12-01 01:46:58.000000 twine-4.0.2/tests/alt-fixtures/twine-1.5.0-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (122)     2034 2022-12-01 01:46:58.000000 twine-4.0.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 01:47:40.000000 twine-4.0.2/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (122)       75 2022-12-01 01:46:58.000000 twine-4.0.2/tests/fixtures/deprecated-pypirc
--rw-r--r--   0 runner    (1001) docker     (122)       10 2022-12-01 01:46:58.000000 twine-4.0.2/tests/fixtures/malformed.tar.gz
--rw-r--r--   0 runner    (1001) docker     (122)    15816 2022-12-01 01:46:58.000000 twine-4.0.2/tests/fixtures/twine-1.5.0-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (122)        9 2022-12-01 01:46:58.000000 twine-4.0.2/tests/fixtures/twine-1.5.0-py2.py3-none-any.whl.asc
--rw-r--r--   0 runner    (1001) docker     (122)    21271 2022-12-01 01:46:58.000000 twine-4.0.2/tests/fixtures/twine-1.5.0.tar.gz
--rw-r--r--   0 runner    (1001) docker     (122)    22387 2022-12-01 01:46:58.000000 twine-4.0.2/tests/fixtures/twine-1.6.5-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (122)    26716 2022-12-01 01:46:58.000000 twine-4.0.2/tests/fixtures/twine-1.6.5.tar.gz
--rw-r--r--   0 runner    (1001) docker     (122)    65898 2022-12-01 01:46:58.000000 twine-4.0.2/tests/fixtures/twine-3.3.0-py3.9.egg
--rw-r--r--   0 runner    (1001) docker     (122)     1551 2022-12-01 01:46:58.000000 twine-4.0.2/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)     7899 2022-12-01 01:46:58.000000 twine-4.0.2/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     7665 2022-12-01 01:46:58.000000 twine-4.0.2/tests/test_check.py
--rw-r--r--   0 runner    (1001) docker     (122)     1050 2022-12-01 01:46:58.000000 twine-4.0.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     1279 2022-12-01 01:46:58.000000 twine-4.0.2/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (122)     6497 2022-12-01 01:46:58.000000 twine-4.0.2/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (122)     2738 2022-12-01 01:46:58.000000 twine-4.0.2/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (122)    13452 2022-12-01 01:46:58.000000 twine-4.0.2/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (122)     3007 2022-12-01 01:46:58.000000 twine-4.0.2/tests/test_register.py
--rw-r--r--   0 runner    (1001) docker     (122)    10943 2022-12-01 01:46:58.000000 twine-4.0.2/tests/test_repository.py
--rw-r--r--   0 runner    (1001) docker     (122)     4657 2022-12-01 01:46:58.000000 twine-4.0.2/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (122)    16112 2022-12-01 01:46:58.000000 twine-4.0.2/tests/test_upload.py
--rw-r--r--   0 runner    (1001) docker     (122)     8790 2022-12-01 01:46:58.000000 twine-4.0.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3076 2022-12-01 01:46:58.000000 twine-4.0.2/tests/test_wheel.py
--rw-r--r--   0 runner    (1001) docker     (122)     2879 2022-12-01 01:46:58.000000 twine-4.0.2/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 01:47:40.000000 twine-4.0.2/twine/
--rw-r--r--   0 runner    (1001) docker     (122)     1343 2022-12-01 01:46:58.000000 twine-4.0.2/twine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1475 2022-12-01 01:46:58.000000 twine-4.0.2/twine/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3129 2022-12-01 01:46:58.000000 twine-4.0.2/twine/auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     3738 2022-12-01 01:46:58.000000 twine-4.0.2/twine/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 01:47:40.000000 twine-4.0.2/twine/commands/
--rw-r--r--   0 runner    (1001) docker     (122)     1802 2022-12-01 01:46:58.000000 twine-4.0.2/twine/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5727 2022-12-01 01:46:58.000000 twine-4.0.2/twine/commands/check.py
--rw-r--r--   0 runner    (1001) docker     (122)     2904 2022-12-01 01:46:58.000000 twine-4.0.2/twine/commands/register.py
--rw-r--r--   0 runner    (1001) docker     (122)     7469 2022-12-01 01:46:58.000000 twine-4.0.2/twine/commands/upload.py
--rw-r--r--   0 runner    (1001) docker     (122)     3814 2022-12-01 01:46:58.000000 twine-4.0.2/twine/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    11024 2022-12-01 01:46:58.000000 twine-4.0.2/twine/package.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-01 01:46:58.000000 twine-4.0.2/twine/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     8713 2022-12-01 01:46:58.000000 twine-4.0.2/twine/repository.py
--rw-r--r--   0 runner    (1001) docker     (122)    12269 2022-12-01 01:46:58.000000 twine-4.0.2/twine/settings.py
--rw-r--r--   0 runner    (1001) docker     (122)    10867 2022-12-01 01:46:58.000000 twine-4.0.2/twine/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3049 2022-12-01 01:46:58.000000 twine-4.0.2/twine/wheel.py
--rw-r--r--   0 runner    (1001) docker     (122)     1795 2022-12-01 01:46:58.000000 twine-4.0.2/twine/wininst.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 01:47:40.000000 twine-4.0.2/twine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2930 2022-12-01 01:47:40.000000 twine-4.0.2/twine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2021 2022-12-01 01:47:40.000000 twine-4.0.2/twine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-01 01:47:40.000000 twine-4.0.2/twine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      185 2022-12-01 01:47:40.000000 twine-4.0.2/twine.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      167 2022-12-01 01:47:40.000000 twine-4.0.2/twine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2022-12-01 01:47:40.000000 twine-4.0.2/twine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 13:45:14.069720 twine-5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-02-11 13:45:06.000000 twine-5.0.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-02-11 13:45:06.000000 twine-5.0.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-02-11 13:45:06.000000 twine-5.0.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 13:45:14.057720 twine-5.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 13:45:14.057720 twine-5.0.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     4299 2024-02-11 13:45:06.000000 twine-5.0.0/.github/ISSUE_TEMPLATE/01_upload_failed.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-02-11 13:45:06.000000 twine-5.0.0/.github/ISSUE_TEMPLATE/02_bug.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-02-11 13:45:06.000000 twine-5.0.0/.github/ISSUE_TEMPLATE/03_feature.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-02-11 13:45:06.000000 twine-5.0.0/.github/ISSUE_TEMPLATE/04_other.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-02-11 13:45:06.000000 twine-5.0.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-02-11 13:45:06.000000 twine-5.0.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 13:45:14.057720 twine-5.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-02-11 13:45:06.000000 twine-5.0.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-02-11 13:45:06.000000 twine-5.0.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-02-11 13:45:06.000000 twine-5.0.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-02-11 13:45:06.000000 twine-5.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-02-11 13:45:06.000000 twine-5.0.0/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-02-11 13:45:06.000000 twine-5.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-02-11 13:45:06.000000 twine-5.0.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     9695 2024-02-11 13:45:06.000000 twine-5.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-02-11 13:45:14.069720 twine-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-02-11 13:45:06.000000 twine-5.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 13:45:14.057720 twine-5.0.0/changelog/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-11 13:45:06.000000 twine-5.0.0/changelog/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 13:45:14.061720 twine-5.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)    23391 2024-02-11 13:45:06.000000 twine-5.0.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9639 2024-02-11 13:45:06.000000 twine-5.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9795 2024-02-11 13:45:06.000000 twine-5.0.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-02-11 13:45:06.000000 twine-5.0.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 13:45:14.061720 twine-5.0.0/docs/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-11 13:45:06.000000 twine-5.0.0/docs/internal/twine.auth.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-11 13:45:06.000000 twine-5.0.0/docs/internal/twine.cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-11 13:45:06.000000 twine-5.0.0/docs/internal/twine.commands.check.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-11 13:45:06.000000 twine-5.0.0/docs/internal/twine.commands.register.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-02-11 13:45:06.000000 twine-5.0.0/docs/internal/twine.commands.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-11 13:45:06.000000 twine-5.0.0/docs/internal/twine.commands.upload.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-11 13:45:06.000000 twine-5.0.0/docs/internal/twine.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-11 13:45:06.000000 twine-5.0.0/docs/internal/twine.package.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-11 13:45:06.000000 twine-5.0.0/docs/internal/twine.repository.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-02-11 13:45:06.000000 twine-5.0.0/docs/internal/twine.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-11 13:45:06.000000 twine-5.0.0/docs/internal/twine.settings.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-11 13:45:06.000000 twine-5.0.0/docs/internal/twine.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-11 13:45:06.000000 twine-5.0.0/docs/internal/twine.wheel.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-11 13:45:06.000000 twine-5.0.0/docs/internal/twine.wininst.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-02-11 13:45:06.000000 twine-5.0.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-02-11 13:45:06.000000 twine-5.0.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-02-11 13:45:06.000000 twine-5.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-02-11 13:45:06.000000 twine-5.0.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-02-11 13:45:14.069720 twine-5.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 13:45:14.065720 twine-5.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-11 13:45:06.000000 twine-5.0.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 13:45:14.065720 twine-5.0.0/tests/alt-fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)    15816 2024-02-11 13:45:06.000000 twine-5.0.0/tests/alt-fixtures/twine-1.5.0-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-02-11 13:45:06.000000 twine-5.0.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 13:45:14.065720 twine-5.0.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-11 13:45:06.000000 twine-5.0.0/tests/fixtures/deprecated-pypirc
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-11 13:45:06.000000 twine-5.0.0/tests/fixtures/malformed.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    15816 2024-02-11 13:45:06.000000 twine-5.0.0/tests/fixtures/twine-1.5.0-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-11 13:45:06.000000 twine-5.0.0/tests/fixtures/twine-1.5.0-py2.py3-none-any.whl.asc
+-rw-r--r--   0 runner    (1001) docker     (127)    21271 2024-02-11 13:45:06.000000 twine-5.0.0/tests/fixtures/twine-1.5.0.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    22387 2024-02-11 13:45:06.000000 twine-5.0.0/tests/fixtures/twine-1.6.5-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (127)    26716 2024-02-11 13:45:06.000000 twine-5.0.0/tests/fixtures/twine-1.6.5.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    65898 2024-02-11 13:45:06.000000 twine-5.0.0/tests/fixtures/twine-3.3.0-py3.9.egg
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-02-11 13:45:06.000000 twine-5.0.0/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-02-11 13:45:06.000000 twine-5.0.0/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7672 2024-02-11 13:45:06.000000 twine-5.0.0/tests/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-02-11 13:45:06.000000 twine-5.0.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-02-11 13:45:06.000000 twine-5.0.0/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-02-11 13:45:06.000000 twine-5.0.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-02-11 13:45:06.000000 twine-5.0.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13452 2024-02-11 13:45:06.000000 twine-5.0.0/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-02-11 13:45:06.000000 twine-5.0.0/tests/test_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10943 2024-02-11 13:45:06.000000 twine-5.0.0/tests/test_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-02-11 13:45:06.000000 twine-5.0.0/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19078 2024-02-11 13:45:06.000000 twine-5.0.0/tests/test_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8790 2024-02-11 13:45:06.000000 twine-5.0.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-02-11 13:45:06.000000 twine-5.0.0/tests/test_wheel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-02-11 13:45:06.000000 twine-5.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 13:45:14.069720 twine-5.0.0/twine/
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-02-11 13:45:06.000000 twine-5.0.0/twine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-02-11 13:45:06.000000 twine-5.0.0/twine/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-02-11 13:45:06.000000 twine-5.0.0/twine/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-02-11 13:45:06.000000 twine-5.0.0/twine/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 13:45:14.069720 twine-5.0.0/twine/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-02-11 13:45:06.000000 twine-5.0.0/twine/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6088 2024-02-11 13:45:06.000000 twine-5.0.0/twine/commands/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-02-11 13:45:06.000000 twine-5.0.0/twine/commands/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8727 2024-02-11 13:45:06.000000 twine-5.0.0/twine/commands/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-02-11 13:45:06.000000 twine-5.0.0/twine/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11018 2024-02-11 13:45:06.000000 twine-5.0.0/twine/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-11 13:45:06.000000 twine-5.0.0/twine/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     8713 2024-02-11 13:45:06.000000 twine-5.0.0/twine/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11938 2024-02-11 13:45:06.000000 twine-5.0.0/twine/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10979 2024-02-11 13:45:06.000000 twine-5.0.0/twine/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-02-11 13:45:06.000000 twine-5.0.0/twine/wheel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-02-11 13:45:06.000000 twine-5.0.0/twine/wininst.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 13:45:14.069720 twine-5.0.0/twine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-02-11 13:45:14.000000 twine-5.0.0/twine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-02-11 13:45:14.000000 twine-5.0.0/twine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-11 13:45:14.000000 twine-5.0.0/twine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-02-11 13:45:14.000000 twine-5.0.0/twine.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-02-11 13:45:14.000000 twine-5.0.0/twine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-11 13:45:14.000000 twine-5.0.0/twine.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `twine-4.0.2/.github/workflows/main.yml` & `twine-5.0.0/.github/workflows/main.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,101 +1,124 @@
 name: Main
 
 on:
   push:
+    branches:
+      - main
   pull_request:
   schedule:
     - cron: "0 0 * * *" # daily
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.event.pull_request.number || github.sha }}
   cancel-in-progress: true
 
 env:
   FORCE_COLOR: "1"
   TOX_TESTENV_PASSENV: "FORCE_COLOR"
-  MIN_PYTHON_VERSION: "3.7"
-  DEFAULT_PYTHON_VERSION: "3.9"
+  MIN_PYTHON_VERSION: "3.8"
+  DEFAULT_PYTHON_VERSION: "3.10"
+
+permissions:
+  contents: read
 
 jobs:
   lint:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v2
-      - uses: actions/setup-python@v2
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: ${{ env.DEFAULT_PYTHON_VERSION }}
       - name: Install dependencies
         run: python -m pip install tox
       - name: Run linting
         run: python -m tox -e lint
 
   test:
     strategy:
       matrix:
         python-version:
-          - "3.7"
           - "3.8"
           - "3.9"
           - "3.10"
+          - "3.11"
+          - "3.12"
         platform:
           - ubuntu-latest
           - macos-latest
           - windows-latest
     runs-on: ${{ matrix.platform }}
     steps:
-      - uses: actions/checkout@v2
-      - uses: actions/setup-python@v2
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: python -m pip install tox
       - name: Run type-checking
         run: python -m tox -e types
       - name: Run tests
         run: python -m tox -e py
 
   # Because the tests can be flaky, they shouldn't be required for merge, but
   # it's still helpful to run them on PRs. See:
   # https://github.com/pypa/twine/issues/684#issuecomment-703150619
   integration:
+    # Only run on Ubuntu because most of the tests are skipped on Windows
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v2
-      - uses: actions/setup-python@v2
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: ${{ env.MIN_PYTHON_VERSION }}
       - name: Install dependencies
         run: python -m pip install tox
       - name: Run tests
         run: python -m tox -e integration
 
   docs:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v2
-      - uses: actions/setup-python@v2
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: ${{ env.MIN_PYTHON_VERSION }}
       - name: Install dependencies
         run: python -m pip install tox
       - name: Build docs
         run: python -m tox -e docs
 
-  release:
+  # https://github.com/marketplace/actions/alls-green#why
+  check:  # This job does nothing and is only used for the branch protection
+    if: always()
+
     needs:
       - lint
       - test
-      # Not requiring integration, because they can be flaky
+      - integration
       - docs
+
+    runs-on: ubuntu-latest
+
+    steps:
+    - name: Decide whether the needed jobs succeeded or failed
+      uses: re-actors/alls-green@release/v1
+      with:
+        allowed-failures: integration  # can be flaky
+        jobs: ${{ toJSON(needs) }}
+
+  release:
+    needs:
+      - check
     if: github.event_name == 'push' && contains(github.ref, 'refs/tags/')
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v2
-      - uses: actions/setup-python@v2
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: ${{ env.MIN_PYTHON_VERSION }}
       - name: Install dependencies
         run: python -m pip install tox
       - name: Release
         run: tox -e release
         env:
```

### Comparing `twine-4.0.2/.gitignore` & `twine-5.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `twine-4.0.2/.readthedocs.yaml` & `twine-5.0.0/.readthedocs.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -9,17 +9,20 @@
   fail_on_warning: true
 
 formats:
   - htmlzip
   - pdf
   - epub
 
+build:
+  os: ubuntu-22.04
+  tools:
+    python: "3.11"
+
 python:
-  # Mininum supported Python version
-  version: "3.7"
   # Install twine first, because RTD uses `--upgrade-strategy eager`,
   # which installs the latest version of docutils via readme_renderer.
   # However, Sphinx 4.2.0 requires docutils>=0.14,<0.18.
   install:
     - method: pip
       path: .
     - requirements: docs/requirements.txt
```

### Comparing `twine-4.0.2/AUTHORS` & `twine-5.0.0/AUTHORS`

 * *Files 5% similar despite different names*

```diff
@@ -28,7 +28,8 @@
 Peter Stensmyr <peter.stensmyr@gmail.com> (http://www.peterstensmyr.com)
 Felipe Mulinari Rocha Campos <felipecampos@google.com>
 Devesh Kumar Singh <deveshkusingh@gmail.com>
 Yesha Maggi <yesha.maggic@gmail.com>
 Cyril de Catheu <cdecatheu@gmail.com> (https://catheu.tech/)
 Thomas Miedema <thomasmiedema@gmail.com>
 Hugo van Kemenade (https://github.com/hugovk)
+Jacob Woliver <jacob@jmw.sh> (jmw.sh)
```

### Comparing `twine-4.0.2/LICENSE` & `twine-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `twine-4.0.2/PKG-INFO` & `twine-5.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twine
-Version: 4.0.2
+Version: 5.0.0
 Summary: Collection of utilities for publishing packages on PyPI
 Home-page: https://twine.readthedocs.io/
 Author: Donald Stufft and individual contributors
 Author-email: donald@stufft.io
 Project-URL: Source, https://github.com/pypa/twine/
 Project-URL: Documentation, https://twine.readthedocs.io/en/latest/
 Project-URL: Packaging tutorial, https://packaging.python.org/tutorials/packaging-projects/
@@ -15,33 +15,43 @@
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: BSD
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: pkginfo>=1.8.1
+Requires-Dist: readme-renderer>=35.0
+Requires-Dist: requests>=2.20
+Requires-Dist: requests-toolbelt!=0.9.0,>=0.8.0
+Requires-Dist: urllib3>=1.26.0
+Requires-Dist: importlib-metadata>=3.6
+Requires-Dist: keyring>=15.1
+Requires-Dist: rfc3986>=1.4.0
+Requires-Dist: rich>=12.0.0
 
 .. image:: https://img.shields.io/pypi/v/twine.svg
    :target: https://pypi.org/project/twine
 
 .. image:: https://img.shields.io/pypi/pyversions/twine.svg
    :target: https://pypi.org/project/twine
 
 .. image:: https://img.shields.io/readthedocs/twine
    :target: https://twine.readthedocs.io
 
-.. image:: https://img.shields.io/github/workflow/status/pypa/twine/Main
+.. image:: https://img.shields.io/github/actions/workflow/status/pypa/twine/main.yml?branch=main
    :target: https://github.com/pypa/twine/actions
 
 twine
 =====
 
 Twine is a utility for `publishing`_ Python packages on `PyPI`_.
```

### Comparing `twine-4.0.2/README.rst` & `twine-5.0.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 .. image:: https://img.shields.io/pypi/pyversions/twine.svg
    :target: https://pypi.org/project/twine
 
 .. image:: https://img.shields.io/readthedocs/twine
    :target: https://twine.readthedocs.io
 
-.. image:: https://img.shields.io/github/workflow/status/pypa/twine/Main
+.. image:: https://img.shields.io/github/actions/workflow/status/pypa/twine/main.yml?branch=main
    :target: https://github.com/pypa/twine/actions
 
 twine
 =====
 
 Twine is a utility for `publishing`_ Python packages on `PyPI`_.
```

### Comparing `twine-4.0.2/docs/changelog.rst` & `twine-5.0.0/docs/changelog.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,36 @@
 =========
 Changelog
 =========
 
-This project follows the `semantic versioning <https://packaging.python.org/guides/distributing-packages-using-setuptools/#semantic-versioning-preferred>`_
-and `pre-release versioning <https://packaging.python.org/guides/distributing-packages-using-setuptools/#pre-release-versioning>`_
+This project follows the `semantic versioning <https://packaging.python.org/en/latest/discussions/versioning/#semantic-versioning-vs-calendar-versioning>`_
+and `pre-release versioning <https://packaging.python.org/en/latest/discussions/versioning/>`_
 schemes recommended by the Python Packaging Authority.
 
 .. Do *NOT* add changelog entries here!
    This changelog is managed by towncrier and is built at release time.
    See https://twine.readthedocs.io/en/latest/contributing.html#changelog-entries for details.
 
 .. towncrier release notes start
 
+Twine 5.0.0 (2024-02-10)
+------------------------
+
+Bugfixes
+^^^^^^^^
+
+- Use ``email.message`` instead of ``cgi`` as ``cgi`` has been deprecated (`#969 <https://github.com/pypa/twine/issues/969>`_)
+
+
+Misc
+^^^^
+
+- `#931 <https://github.com/pypa/twine/issues/931>`_, `#991 <https://github.com/pypa/twine/issues/991>`_, `#1028 <https://github.com/pypa/twine/issues/1028>`_, `#1040 <https://github.com/pypa/twine/issues/1040>`_
+
+
 Twine 4.0.2 (2022-11-30)
 ------------------------
 
 Bugfixes
 ^^^^^^^^
 
 - Remove deprecated function to fix ``twine check`` with pkginfo 1.9.0. (`#941 <https://github.com/pypa/twine/issues/941>`_)
@@ -24,15 +39,15 @@
 Twine 4.0.1 (2022-06-01)
 ------------------------
 
 Bugfixes
 ^^^^^^^^
 
 - Improve logging when keyring fails. (`#890 <https://github.com/pypa/twine/issues/890>`_)
-- Reconfgure root logger to show all log messages. (`#896 <https://github.com/pypa/twine/issues/896>`_)
+- Reconfigure root logger to show all log messages. (`#896 <https://github.com/pypa/twine/issues/896>`_)
 
 
 Twine 4.0.0 (2022-03-31)
 ------------------------
 
 Features
 ^^^^^^^^
```

### Comparing `twine-4.0.2/docs/conf.py` & `twine-5.0.0/docs/conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -261,23 +261,27 @@
 
 # If false, no module index is generated.
 # texinfo_domain_indices = True
 
 # How to display URL addresses: 'footnote', 'no', or 'inline'.
 # texinfo_show_urls = 'footnote'
 
+# See https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-linkcheck_ignore
 linkcheck_ignore = [
-    "http://127.0.0.1*",
+    r"https?://127\.0\.0\.1.*",
     # Avoid errors due to GitHub rate limit
     # https://github.com/sphinx-doc/sphinx/issues/7388
-    "https://github.com/pypa/twine/issues/*",
+    r"https://github\.com/pypa/twine/issues/.*",
     # Avoid errors from channels interpreted as anchors
-    "https://web.libera.chat/#",
+    r"https://web\.libera\.chat/#",
     # Avoid error from InvalidPyPIUploadURL docstring
-    "https://upload.pypi.org/legacy",
+    r"https://upload\.pypi\.org/legacy/?",
+    # Avoid errors from 403/Login Redirects
+    r"https://(test\.)?pypi\.org/manage/project/twine/collaboration/?",
+    r"https://pypi\.org/manage/project/twine/collaboration/?",
 ]
 
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3", None),
     "requests": ("https://requests.readthedocs.io/en/latest/", None),
 }
```

### Comparing `twine-4.0.2/docs/contributing.rst` & `twine-5.0.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `twine-4.0.2/docs/index.rst` & `twine-5.0.0/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -173,16 +173,15 @@
 without ``export``-ing it for other tools:
 
 .. code-block:: bash
 
    HTTPS_PROXY=socks5://user:pass@host:port twine upload dist/*
 
 For more information, see the Requests documentation on
-`proxies <https://requests.readthedocs.io/en/latest/user/advanced/#proxies>`_ and
-`SOCKS <https://requests.readthedocs.io/en/latest/user/advanced/#socks>`_ , and
+:ref:`requests:proxies` and :ref:`requests:socks`, and
 `an in-depth article about proxy environment variables
 <https://about.gitlab.com/blog/2021/01/27/we-need-to-talk-no-proxy/>`_.
 
 Keyring Support
 ---------------
 
 Instead of typing in your password every time you upload a distribution, Twine
```

### Comparing `twine-4.0.2/mypy.ini` & `twine-5.0.0/mypy.ini`

 * *Files 16% similar despite different names*

```diff
@@ -14,18 +14,14 @@
 check_untyped_defs = True
 disallow_untyped_decorators = True
 no_implicit_optional = True
 warn_return_any = True
 no_implicit_reexport = True
 strict_equality = True
 
-[mypy-pkginfo]
-; https://bugs.launchpad.net/pkginfo/+bug/1876591
-ignore_missing_imports = True
-
 [mypy-requests_toolbelt,requests_toolbelt.*]
 ; https://github.com/requests/toolbelt/issues/279
 ignore_missing_imports = True
 
 [mypy-rfc3986]
 ignore_missing_imports = True
```

### Comparing `twine-4.0.2/setup.cfg` & `twine-5.0.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-license_file = LICENSE
+license_files = LICENSE
 name = twine
 author = Donald Stufft and individual contributors
 author_email = donald@stufft.io
 description = Collection of utilities for publishing packages on PyPI
 long_description = file:README.rst
 long_description_content_type = text/x-rst
 url = https://twine.readthedocs.io/
@@ -19,25 +19,26 @@
 	Operating System :: POSIX
 	Operating System :: POSIX :: BSD
 	Operating System :: POSIX :: Linux
 	Operating System :: Microsoft :: Windows
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Programming Language :: Python :: Implementation :: CPython
 
 [options]
 packages = 
 	twine
 	twine.commands
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
 	pkginfo >= 1.8.1
 	readme-renderer >= 35.0
 	requests >= 2.20
 	requests-toolbelt >= 0.8.0, != 0.9.0
 	urllib3 >= 1.26.0
 	importlib-metadata >= 3.6
```

### Comparing `twine-4.0.2/tests/alt-fixtures/twine-1.5.0-py2.py3-none-any.whl` & `twine-5.0.0/tests/alt-fixtures/twine-1.5.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `twine-4.0.2/tests/conftest.py` & `twine-5.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `twine-4.0.2/tests/fixtures/twine-1.5.0-py2.py3-none-any.whl` & `twine-5.0.0/tests/fixtures/twine-1.5.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `twine-4.0.2/tests/fixtures/twine-1.5.0.tar.gz` & `twine-5.0.0/tests/fixtures/twine-1.5.0.tar.gz`

 * *Files identical despite different names*

### Comparing `twine-4.0.2/tests/fixtures/twine-1.6.5-py2.py3-none-any.whl` & `twine-5.0.0/tests/fixtures/twine-1.6.5-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `twine-4.0.2/tests/fixtures/twine-1.6.5.tar.gz` & `twine-5.0.0/tests/fixtures/twine-1.6.5.tar.gz`

 * *Files identical despite different names*

### Comparing `twine-4.0.2/tests/fixtures/twine-3.3.0-py3.9.egg` & `twine-5.0.0/tests/fixtures/twine-3.3.0-py3.9.egg`

 * *Files identical despite different names*

### Comparing `twine-4.0.2/tests/helpers.py` & `twine-5.0.0/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `twine-4.0.2/tests/test_auth.py` & `twine-5.0.0/tests/test_auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,15 +215,15 @@
         r".+KeyError: 'HOME'"
         r".+KeyError: 'uid not found: 999'",
         caplog.text,
         re.DOTALL,
     )
 
 
-def test_logs_cli_values(caplog):
+def test_logs_cli_values(caplog, config):
     caplog.set_level(logging.INFO, "twine")
 
     res = auth.Resolver(config, auth.CredentialInput("username", "password"))
 
     assert res.username == "username"
     assert res.password == "password"
```

### Comparing `twine-4.0.2/tests/test_check.py` & `twine-5.0.0/tests/test_check.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import pretend
 import pytest
 
 from twine.commands import check
 
 
 class TestWarningStream:
-    def setup(self):
+    def setup_method(self):
         self.stream = check._WarningStream()
 
     def test_write_match(self):
         self.stream.write("<string>:2: (WARNING/2) Title underline too short.")
         assert self.stream.getvalue() == "line 2: Warning: Title underline too short.\n"
 
     def test_write_nomatch(self):
```

### Comparing `twine-4.0.2/tests/test_cli.py` & `twine-5.0.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `twine-4.0.2/tests/test_commands.py` & `twine-5.0.0/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `twine-4.0.2/tests/test_integration.py` & `twine-5.0.0/tests/test_integration.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,49 +1,59 @@
 import contextlib
 import datetime
 import functools
 import pathlib
+import platform
 import re
 import secrets
 import subprocess
 import sys
+from types import SimpleNamespace
 
-import jaraco.envs
-import munch
-import portend
 import pytest
 import requests
 
 from twine import __main__ as dunder_main
 from twine import cli
 
-pytestmark = [
-    pytest.mark.enable_socket,
-    pytest.mark.flaky(reruns=3, reruns_delay=1),
-]
+pytestmark = [pytest.mark.enable_socket]
+
+skip_if_windows = pytest.mark.skipif(
+    platform.system() == "Windows",
+    reason="pytest-services fixtures don't support Windows",
+)
+
+run = functools.partial(subprocess.run, check=True)
 
 
 @pytest.fixture(scope="session")
-def sampleproject_dist(tmp_path_factory):
+def sampleproject_dist(tmp_path_factory: pytest.TempPathFactory):
     checkout = tmp_path_factory.mktemp("sampleproject", numbered=False)
-    subprocess.run(
-        ["git", "clone", "https://github.com/pypa/sampleproject", str(checkout)]
-    )
-    with (checkout / "setup.py").open("r+") as setup:
-        orig = setup.read()
-        sub = orig.replace('name="sampleproject"', 'name="twine-sampleproject"')
-        assert orig != sub
-        setup.seek(0)
-        setup.write(sub)
     tag = datetime.datetime.now().strftime("%Y%m%d%H%M%S%f")
-    subprocess.run(
-        [sys.executable, "setup.py", "egg_info", "--tag-build", f"post{tag}", "sdist"],
-        cwd=str(checkout),
+
+    run(["git", "clone", "https://github.com/pypa/sampleproject", str(checkout)])
+
+    pyproject = checkout / "pyproject.toml"
+    pyproject.write_text(
+        pyproject.read_text()
+        .replace(
+            'name = "sampleproject"',
+            'name = "twine-sampleproject"',
+        )
+        .replace(
+            'version = "3.0.0"',
+            f'version = "3.0.0post{tag}"',
+        )
     )
-    (dist,) = checkout.joinpath("dist").glob("*")
+
+    run([sys.executable, "-m", "build", "--sdist"], cwd=checkout)
+
+    [dist, *_] = (checkout / "dist").glob("*")
+    assert dist.name == f"twine-sampleproject-3.0.0.post{tag}.tar.gz"
+
     return dist
 
 
 sampleproject_token = (
     "pypi-AgENdGVzdC5weXBpLm9yZwIkNDgzYTFhMjEtMzEwYi00NT"
     "kzLTkwMzYtYzc1Zjg4NmFiMjllAAJEeyJwZXJtaXNzaW9ucyI6IH"
     "sicHJvamVjdHMiOiBbInR3aW5lLXNhbXBsZXByb2plY3QiXX0sIC"
@@ -101,147 +111,93 @@
         "twine-1.6.5-py2.py3-none-any.whl",
     ]
 )
 def uploadable_dist(request):
     return pathlib.Path(__file__).parent / "fixtures" / request.param
 
 
-class DevPiEnv(jaraco.envs.ToxEnv):
-    """Run devpi using tox:testenv:devpi."""
-
-    name = "devpi"
+@pytest.fixture(scope="session")
+def devpi_server(request, port_getter, watcher_getter, tmp_path_factory):
+    server_dir = tmp_path_factory.mktemp("devpi")
     username = "foober"
+    password = secrets.token_urlsafe()
+    port = port_getter()
+    url = f"http://localhost:{port}/"
+    repo = f"{url}/{username}/dev/"
 
-    def create(self, root, password):
-        super().create()
-        self.base = root
-        self.password = password
-        self.port = portend.find_available_local_port()
-        cmd = [
-            self.exe("devpi-init"),
-            "--serverdir",
-            str(root),
-            "--root-passwd",
-            password,
-        ]
-        subprocess.run(cmd, check=True)
-
-    @property
-    def url(self):
-        return f"http://localhost:{self.port}/"
-
-    @property
-    def repo(self):
-        return f"{self.url}/{self.username}/dev/"
+    run(["devpi-init", "--serverdir", server_dir, "--root-passwd", password])
 
-    def ready(self):
+    def ready():
         with contextlib.suppress(Exception):
-            return requests.get(self.url)
-
-    def init(self):
-        run = functools.partial(subprocess.run, check=True)
-        client_dir = self.base / "client"
-        devpi_client = [
-            self.exe("devpi"),
-            "--clientdir",
-            str(client_dir),
-        ]
-        run(devpi_client + ["use", self.url + "root/pypi/"])
-        run(
-            devpi_client
-            + ["user", "--create", self.username, f"password={self.password}"]
-        )
-        run(devpi_client + ["login", self.username, "--password", self.password])
-        run(devpi_client + ["index", "-c", "dev"])
+            return requests.get(url)
 
-
-@pytest.fixture(scope="session")
-def devpi_server(request, watcher_getter, tmp_path_factory):
-    env = DevPiEnv()
-    password = secrets.token_urlsafe()
-    root = tmp_path_factory.mktemp("devpi")
-    env.create(root, password)
-    proc = watcher_getter(
-        name=str(env.exe("devpi-server")),
-        arguments=["--port", str(env.port), "--serverdir", str(root)],
-        checker=env.ready,
+    watcher_getter(
+        name="devpi-server",
+        arguments=["--port", str(port), "--serverdir", server_dir],
+        checker=ready,
         # Needed for the correct execution order of finalizers
         request=request,
     )
-    env.init()
-    username = env.username
-    url = env.repo
-    return munch.Munch.fromDict(locals())
 
+    def devpi_run(cmd):
+        return run(["devpi", "--clientdir", server_dir / "client", *cmd])
 
-@pytest.mark.xfail(
-    sys.platform == "win32",
-    reason="pytest-services watcher_getter fixture does not support Windows",
-)
+    devpi_run(["use", url + "root/pypi/"])
+    devpi_run(["user", "--create", username, f"password={password}"])
+    devpi_run(["login", username, "--password", password])
+    devpi_run(["index", "-c", "dev"])
+
+    return SimpleNamespace(url=repo, username=username, password=password)
+
+
+@skip_if_windows
 def test_devpi_upload(devpi_server, uploadable_dist):
     command = [
         "upload",
         "--repository-url",
         devpi_server.url,
         "--username",
         devpi_server.username,
         "--password",
         devpi_server.password,
         str(uploadable_dist),
     ]
     cli.dispatch(command)
 
 
-class PypiserverEnv(jaraco.envs.ToxEnv):
-    """Run pypiserver using tox:testenv:pypiserver."""
-
-    name = "pypiserver"
-
-    @property
-    @functools.lru_cache()
-    def port(self):
-        return portend.find_available_local_port()
-
-    @property
-    def url(self):
-        return f"http://localhost:{self.port}/"
+@pytest.fixture(scope="session")
+def pypiserver_instance(request, port_getter, watcher_getter, tmp_path_factory):
+    port = port_getter()
+    url = f"http://localhost:{port}/"
 
-    def ready(self):
+    def ready():
         with contextlib.suppress(Exception):
-            return requests.get(self.url)
-
+            return requests.get(url)
 
-@pytest.fixture(scope="session")
-def pypiserver_instance(request, watcher_getter, tmp_path_factory):
-    env = PypiserverEnv()
-    env.create()
-    proc = watcher_getter(
-        name=str(env.exe("pypi-server")),
+    watcher_getter(
+        name="pypi-server",
         arguments=[
             "--port",
-            str(env.port),
+            str(port),
             # allow anonymous uploads
             "-P",
             ".",
             "-a",
             ".",
             tmp_path_factory.mktemp("packages"),
         ],
-        checker=env.ready,
+        checker=ready,
         # Needed for the correct execution order of finalizers
         request=request,
     )
-    url = env.url
-    return munch.Munch.fromDict(locals())
 
+    return SimpleNamespace(url=url)
 
-@pytest.mark.xfail(
-    sys.platform == "win32",
-    reason="pytest-services watcher_getter fixture does not support Windows",
-)
+
+@skip_if_windows
 def test_pypiserver_upload(pypiserver_instance, uploadable_dist):
     command = [
         "upload",
         "--repository-url",
         pypiserver_instance.url,
         "--username",
         "any",
```

### Comparing `twine-4.0.2/tests/test_main.py` & `twine-5.0.0/tests/test_main.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,30 +14,36 @@
 
 import pretend
 import requests
 
 from twine import __main__ as dunder_main
 from twine.commands import upload
 
+# Hard-coding control characters for red text; couldn't find a succinct alternative
+RED_ERROR = "\x1b[31mERROR   \x1b[0m"
+PLAIN_ERROR = "ERROR   "
+
+
+def _unwrap_lines(text):
+    # Testing wrapped lines was ugly and inconsistent across environments
+    return " ".join(line.strip() for line in text.splitlines())
+
 
 def test_exception_handling(monkeypatch, capsys):
     monkeypatch.setattr(sys, "argv", ["twine", "upload", "missing.whl"])
 
     error = dunder_main.main()
     assert error
 
     captured = capsys.readouterr()
 
-    # Hard-coding control characters for red text; couldn't find a succinct alternative.
-    # Removing trailing whitespace on wrapped lines; trying to test it was ugly.
-    level = "\x1b[31mERROR   \x1b[0m"
-    assert [line.rstrip() for line in captured.out.splitlines()] == [
-        f"{level} InvalidDistribution: Cannot find file (or expand pattern):",
-        "         'missing.whl'",
-    ]
+    assert _unwrap_lines(captured.out) == (
+        f"{RED_ERROR} InvalidDistribution: Cannot find file (or expand pattern): "
+        "'missing.whl'"
+    )
 
 
 def test_http_exception_handling(monkeypatch, capsys):
     monkeypatch.setattr(sys, "argv", ["twine", "upload", "test.whl"])
     monkeypatch.setattr(
         upload,
         "upload",
@@ -53,32 +59,28 @@
     )
 
     error = dunder_main.main()
     assert error
 
     captured = capsys.readouterr()
 
-    # Hard-coding control characters for red text; couldn't find a succinct alternative.
-    # Removing trailing whitespace on wrapped lines; trying to test it was ugly.
-    level = "\x1b[31mERROR   \x1b[0m"
-    assert [line.rstrip() for line in captured.out.splitlines()] == [
-        f"{level} HTTPError: 400 Bad Request from https://example.org",
-        "         Error reason",
-    ]
+    assert _unwrap_lines(captured.out) == (
+        f"{RED_ERROR} HTTPError: 400 Bad Request from https://example.org "
+        "Error reason"
+    )
 
 
 def test_no_color_exception(monkeypatch, capsys):
     monkeypatch.setattr(sys, "argv", ["twine", "--no-color", "upload", "missing.whl"])
 
     error = dunder_main.main()
     assert error
 
     captured = capsys.readouterr()
 
-    # Removing trailing whitespace on wrapped lines; trying to test it was ugly.
-    assert [line.rstrip() for line in captured.out.splitlines()] == [
-        "ERROR    InvalidDistribution: Cannot find file (or expand pattern):",
-        "         'missing.whl'",
-    ]
+    assert _unwrap_lines(captured.out) == (
+        f"{PLAIN_ERROR} InvalidDistribution: Cannot find file (or expand pattern): "
+        "'missing.whl'"
+    )
 
 
 # TODO: Test verbose output formatting
```

### Comparing `twine-4.0.2/tests/test_package.py` & `twine-5.0.0/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `twine-4.0.2/tests/test_register.py` & `twine-5.0.0/tests/test_register.py`

 * *Files 18% similar despite different names*

```diff
@@ -75,26 +75,63 @@
     with pytest.raises(
         exceptions.PackageNotFound,
         match=f'"{package}" does not exist on the file system.',
     ):
         register.register(register_settings, package)
 
 
-def test_values_from_env(monkeypatch):
+@pytest.mark.parametrize("repo", ["pypi", "testpypi"])
+def test_values_from_env_pypi(monkeypatch, repo):
     """Use env vars for settings when run from command line."""
 
     def none_register(*args, **settings_kwargs):
         pass
 
     replaced_register = pretend.call_recorder(none_register)
     monkeypatch.setattr(register, "register", replaced_register)
     testenv = {
-        "TWINE_USERNAME": "pypiuser",
+        "TWINE_REPOSITORY": repo,
+        # Ignored because the TWINE_REPOSITORY is PyPI/TestPyPI
+        "TWINE_USERNAME": "this-is-ignored",
         "TWINE_PASSWORD": "pypipassword",
         "TWINE_CERT": "/foo/bar.crt",
     }
     with helpers.set_env(**testenv):
         cli.dispatch(["register", helpers.WHEEL_FIXTURE])
     register_settings = replaced_register.calls[0].args[0]
     assert "pypipassword" == register_settings.password
-    assert "pypiuser" == register_settings.username
+    assert "__token__" == register_settings.username
+    assert "/foo/bar.crt" == register_settings.cacert
+
+
+def test_values_from_env_not_pypi(monkeypatch, write_config_file):
+    """Use env vars for settings when run from command line."""
+    write_config_file(
+        """
+        [distutils]
+        index-servers =
+            notpypi
+
+        [notpypi]
+        repository: https://upload.example.org/legacy/
+        username:someusername
+        password:password
+        """
+    )
+
+    def none_register(*args, **settings_kwargs):
+        pass
+
+    replaced_register = pretend.call_recorder(none_register)
+    monkeypatch.setattr(register, "register", replaced_register)
+    testenv = {
+        "TWINE_REPOSITORY": "notpypi",
+        "TWINE_USERNAME": "someusername",
+        "TWINE_PASSWORD": "pypipassword",
+        "TWINE_CERT": "/foo/bar.crt",
+    }
+    with helpers.set_env(**testenv):
+        cli.dispatch(["register", helpers.WHEEL_FIXTURE])
+    register_settings = replaced_register.calls[0].args[0]
+    assert "pypipassword" == register_settings.password
+    assert "someusername" == register_settings.username
     assert "/foo/bar.crt" == register_settings.cacert
```

### Comparing `twine-4.0.2/tests/test_repository.py` & `twine-5.0.0/tests/test_repository.py`

 * *Files identical despite different names*

### Comparing `twine-4.0.2/tests/test_settings.py` & `twine-5.0.0/tests/test_settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for the Settings class and module."""
+
 # Copyright 2018 Ian Stapleton Cordasco
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # https://www.apache.org/licenses/LICENSE-2.0
@@ -23,31 +24,61 @@
 
 def test_settings_takes_no_positional_arguments():
     """Raise an exception when Settings is initialized without keyword arguments."""
     with pytest.raises(TypeError):
         settings.Settings("a", "b", "c")
 
 
-def test_settings_transforms_repository_config(write_config_file):
-    """Set repository config and defaults when .pypirc is provided."""
+def test_settings_transforms_repository_config_pypi(write_config_file):
+    """Set repository config and defaults when .pypirc is provided.
+
+    Ignores the username setting due to PyPI being the index.
+    """
     config_file = write_config_file(
         """
         [pypi]
         repository: https://upload.pypi.org/legacy/
-        username:username
+        username:this-is-ignored
         password:password
         """
     )
 
     s = settings.Settings(config_file=config_file)
     assert s.repository_config["repository"] == "https://upload.pypi.org/legacy/"
     assert s.sign is False
     assert s.sign_with == "gpg"
     assert s.identity is None
-    assert s.username == "username"
+    assert s.username == "__token__"
+    assert s.password == "password"
+    assert s.cacert is None
+    assert s.client_cert is None
+    assert s.disable_progress_bar is False
+
+
+def test_settings_transforms_repository_config_non_pypi(write_config_file):
+    """Set repository config and defaults when .pypirc is provided."""
+    config_file = write_config_file(
+        """
+        [distutils]
+        index-servers =
+            notpypi
+
+        [notpypi]
+        repository: https://upload.example.org/legacy/
+        username:someusername
+        password:password
+        """
+    )
+
+    s = settings.Settings(config_file=config_file, repository_name="notpypi")
+    assert s.repository_config["repository"] == "https://upload.example.org/legacy/"
+    assert s.sign is False
+    assert s.sign_with == "gpg"
+    assert s.identity is None
+    assert s.username == "someusername"
     assert s.password == "password"
     assert s.cacert is None
     assert s.client_cert is None
     assert s.disable_progress_bar is False
 
 
 @pytest.mark.parametrize(
@@ -73,15 +104,15 @@
     if verbose:
         assert caplog.messages == [f"Using configuration from {config_file}"]
     else:
         assert caplog.messages == []
 
 
 def test_identity_requires_sign():
-    """Raise an exception when user provides identity but doesn't require sigining."""
+    """Raise an exception when user provides identity but doesn't require signing."""
     with pytest.raises(exceptions.InvalidSigningConfiguration):
         settings.Settings(sign=False, identity="fakeid")
 
 
 @pytest.mark.parametrize("client_cert", [None, ""])
 def test_password_is_required_if_no_client_cert(client_cert, entered_password):
     """Set password when client_cert is not provided."""
```

### Comparing `twine-4.0.2/tests/test_upload.py` & `twine-5.0.0/tests/test_upload.py`

 * *Files 4% similar despite different names*

```diff
@@ -141,15 +141,15 @@
 
     assert [m for m in caplog.messages if m.endswith("KB)")] == [
         f"{filename} ({size})" for filename, size in dists_to_upload.items()
     ]
 
 
 def test_print_response_if_verbose(upload_settings, stub_response, caplog):
-    """Print details about the response from the repostiry."""
+    """Print details about the response from the repository."""
     upload_settings.verbose = True
 
     result = upload.upload(
         upload_settings,
         [helpers.WHEEL_FIXTURE, helpers.SDIST_FIXTURE],
     )
     assert result is None
@@ -158,29 +158,83 @@
         f"Response from {stub_response.url}:\n"
         f"{stub_response.status_code} {stub_response.reason}"
     )
 
     assert caplog.messages.count(response_log) == 2
 
 
-def test_success_with_pre_signed_distribution(upload_settings, stub_repository):
+def test_success_with_pre_signed_distribution(upload_settings, stub_repository, caplog):
     """Add GPG signature provided by user to uploaded package."""
     # Upload a pre-signed distribution
     result = upload.upload(
         upload_settings, [helpers.WHEEL_FIXTURE, helpers.WHEEL_FIXTURE + ".asc"]
     )
     assert result is None
 
     # The signature should be added via package.add_gpg_signature()
     package = stub_repository.upload.calls[0].args[0]
     assert package.gpg_signature == (
         "twine-1.5.0-py2.py3-none-any.whl.asc",
         b"signature",
     )
 
+    # Ensure that a warning is emitted.
+    assert (
+        "One or more packages has an associated PGP signature; these will "
+        "be silently ignored by the index" in caplog.messages
+    )
+
+
+def test_warns_potential_pgp_removal_on_3p_index(
+    make_settings, stub_repository, caplog
+):
+    """Warn when a PGP signature is specified for upload to a third-party index."""
+    upload_settings = make_settings(
+        """
+        [pypi]
+        repository: https://example.com/not-a-real-index/
+        username:foo
+        password:bar
+        """
+    )
+    upload_settings.create_repository = lambda: stub_repository
+
+    # Upload a pre-signed distribution
+    result = upload.upload(
+        upload_settings, [helpers.WHEEL_FIXTURE, helpers.WHEEL_FIXTURE + ".asc"]
+    )
+    assert result is None
+
+    # The signature should be added via package.add_gpg_signature()
+    package = stub_repository.upload.calls[0].args[0]
+    assert package.gpg_signature == (
+        "twine-1.5.0-py2.py3-none-any.whl.asc",
+        b"signature",
+    )
+
+    # Ensure that a warning is emitted.
+    assert (
+        "One or more packages has an associated PGP signature; a future "
+        "version of twine may silently ignore these. See "
+        "https://github.com/pypa/twine/issues/1009 for more information"
+        in caplog.messages
+    )
+
+
+def test_exception_with_only_pre_signed_file(upload_settings, stub_repository):
+    """Raise an exception when only a signed file is uploaded."""
+    # Upload only pre-signed file
+    with pytest.raises(exceptions.InvalidDistribution) as err:
+        upload.upload(upload_settings, [helpers.WHEEL_FIXTURE + ".asc"])
+
+    assert (
+        "Cannot upload signed files by themselves, must upload with a "
+        "corresponding distribution file." in err.value.args[0]
+    )
+
 
 def test_success_when_gpg_is_run(upload_settings, stub_repository, monkeypatch):
     """Add GPG signature generated by gpg command to uploaded package."""
     # Indicate that upload() should run_gpg() to generate the signature, which
     # we'll stub out to use WHEEL_FIXTURE + ".asc"
     upload_settings.sign = True
     upload_settings.sign_with = "gpg"
@@ -486,30 +540,66 @@
     assert not upload.skip_upload(
         response=pretend.stub(),
         skip_existing=False,
         package=package_file.PackageFile.from_filename(helpers.WHEEL_FIXTURE, None),
     )
 
 
-def test_values_from_env(monkeypatch):
+@pytest.mark.parametrize("repo", ["pypi", "testpypi"])
+def test_values_from_env_pypi(monkeypatch, repo):
+    def none_upload(*args, **settings_kwargs):
+        pass
+
+    replaced_upload = pretend.call_recorder(none_upload)
+    monkeypatch.setattr(upload, "upload", replaced_upload)
+    testenv = {
+        "TWINE_REPOSITORY": repo,
+        # Ignored because TWINE_REPOSITORY is PyPI/TestPyPI
+        "TWINE_USERNAME": "this-is-ignored",
+        "TWINE_PASSWORD": "pypipassword",
+        "TWINE_CERT": "/foo/bar.crt",
+    }
+    with helpers.set_env(**testenv):
+        cli.dispatch(["upload", "path/to/file"])
+    upload_settings = replaced_upload.calls[0].args[0]
+    assert "pypipassword" == upload_settings.password
+    assert "__token__" == upload_settings.username
+    assert "/foo/bar.crt" == upload_settings.cacert
+
+
+def test_values_from_env_non_pypi(monkeypatch, write_config_file):
+    write_config_file(
+        """
+        [distutils]
+        index-servers =
+            notpypi
+
+        [notpypi]
+        repository: https://upload.example.org/legacy/
+        username:someusername
+        password:password
+        """
+    )
+
     def none_upload(*args, **settings_kwargs):
         pass
 
     replaced_upload = pretend.call_recorder(none_upload)
     monkeypatch.setattr(upload, "upload", replaced_upload)
     testenv = {
-        "TWINE_USERNAME": "pypiuser",
+        "TWINE_REPOSITORY": "notpypi",
+        "TWINE_USERNAME": "someusername",
         "TWINE_PASSWORD": "pypipassword",
         "TWINE_CERT": "/foo/bar.crt",
     }
     with helpers.set_env(**testenv):
         cli.dispatch(["upload", "path/to/file"])
     upload_settings = replaced_upload.calls[0].args[0]
     assert "pypipassword" == upload_settings.password
-    assert "pypiuser" == upload_settings.username
+    assert "someusername" == upload_settings.username
     assert "/foo/bar.crt" == upload_settings.cacert
 
 
 @pytest.mark.parametrize(
     "repo_url",
     ["https://upload.pypi.org/", "https://test.pypi.org/", "https://pypi.org/"],
 )
```

### Comparing `twine-4.0.2/tests/test_utils.py` & `twine-5.0.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `twine-4.0.2/tests/test_wheel.py` & `twine-5.0.0/tests/test_wheel.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 
 
 def test_version_parsing(example_wheel):
     assert example_wheel.py_version == "py2.py3"
 
 
 def test_version_parsing_missing_pyver(monkeypatch, example_wheel):
-
     wheel.wheel_file_re = pretend.stub(match=lambda a: None)
     assert example_wheel.py_version == "any"
 
 
 def test_find_metadata_files():
     names = [
         "package/lib/__init__.py",
```

### Comparing `twine-4.0.2/tox.ini` & `twine-5.0.0/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -1,48 +1,54 @@
 [tox]
-minversion = 3.3
-envlist = lint,types,py{37,38,39,310},integration,docs
+minversion = 3.8
+envlist = lint,types,py{38,39,310,311,312},integration,docs
 isolated_build = True
 
 [testenv]
 deps =
     pretend
     pytest
     pytest-socket
     build
     coverage
+    # Needed on 3.12 and newer due to setuptools not being pre-installed
+    # in fresh venvs.
+    # See: https://github.com/python/cpython/issues/95299
+    setuptools
 passenv =
     PYTEST_ADDOPTS
 commands =
-    python -m coverage run -m pytest --ignore-glob '*integration*.py'
-    python -m coverage html --show-contexts
-    python -m coverage report -m --fail-under 97
+    python -m coverage run -m pytest {posargs}
+    python -m coverage html
+    python -m coverage report --skip-covered --show-missing --fail-under 97
 
 [testenv:integration]
 deps =
     {[testenv]deps}
-    jaraco.envs
-    munch
-    portend
     pytest-rerunfailures
     pytest-services
+    devpi-server
+    devpi
+    pypiserver
 passenv =
     PYTEST_ADDOPTS
 commands =
-    pytest -r aR tests/test_integration.py
+    pytest -r aR tests/test_integration.py {posargs}
 
 [testenv:docs]
 deps =
     -rdocs/requirements.txt
+allowlist_externals =
+    sh
 commands =
     sphinx-build -W --keep-going -b html -d {envtmpdir}/doctrees docs docs/_build/html
     sphinx-build -W --keep-going -b doctest -d {envtmpdir}/doctrees docs docs/_build/html
     doc8 docs README.rst --ignore-path docs/_build/html
     sphinx-build -W --keep-going -b linkcheck -d {envtmpdir}/doctrees docs docs/_build/linkcheck
-    python -m twine check --strict {distdir}/*
+    sh -c "python -m twine check --strict $TOX_PACKAGE"
 
 [testenv:watch-docs]
 deps =
     -rdocs/requirements.txt
     sphinx-autobuild
 commands =
     sphinx-autobuild -b html -d {envtmpdir}/doctrees \
@@ -115,16 +121,7 @@
     {[testenv:lint]deps}
     {[testenv:types]deps}
 download = True
 usedevelop = True
 commands =
     python -c 'import sys; print(sys.executable)'
     python --version
-
-[testenv:devpi]
-deps =
-    devpi-server
-    devpi
-
-[testenv:pypiserver]
-deps =
-    pypiserver
```

### Comparing `twine-4.0.2/twine/__init__.py` & `twine-5.0.0/twine/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Top-level module for Twine.
 
 The contents of this package are not a public API. For more details, see
 https://github.com/pypa/twine/issues/194 and https://github.com/pypa/twine/issues/665.
 """
+
 # Copyright 2018 Donald Stufft and individual contributors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # https://www.apache.org/licenses/LICENSE-2.0
@@ -36,8 +37,8 @@
 
 __title__ = metadata["name"]
 __summary__ = metadata["summary"]
 __uri__ = metadata["home-page"]
 __version__ = metadata["version"]
 __author__ = metadata["author"]
 __email__ = metadata["author-email"]
-__license__ = metadata["license"]
+__license__ = None
```

### Comparing `twine-4.0.2/twine/__main__.py` & `twine-5.0.0/twine/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import http
 import logging
 import sys
-from typing import Any
+from typing import Any, cast
 
 import requests
 
 from twine import cli
 from twine import exceptions
 
 logger = logging.getLogger(__name__)
@@ -28,21 +28,24 @@
 def main() -> Any:
     # Ensure that all errors are logged, even before argparse
     cli.configure_output()
 
     try:
         error = cli.dispatch(sys.argv[1:])
     except requests.HTTPError as exc:
+        # Assuming this response will never be None
+        response = cast(requests.Response, exc.response)
+
         error = True
-        status_code = exc.response.status_code
+        status_code = response.status_code
         status_phrase = http.HTTPStatus(status_code).phrase
         logger.error(
             f"{exc.__class__.__name__}: {status_code} {status_phrase} "
-            f"from {exc.response.url}\n"
-            f"{exc.response.reason}"
+            f"from {response.url}\n"
+            f"{response.reason}"
         )
     except exceptions.TwineException as exc:
         error = True
         logger.error(f"{exc.__class__.__name__}: {exc.args[0]}")
 
     return error
```

### Comparing `twine-4.0.2/twine/auth.py` & `twine-5.0.0/twine/auth.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,14 +27,21 @@
     @classmethod
     def choose(cls, interactive: bool) -> Type["Resolver"]:
         return cls if interactive else Private
 
     @property
     @functools.lru_cache()
     def username(self) -> Optional[str]:
+        if cast(str, self.config["repository"]).startswith(
+            (utils.DEFAULT_REPOSITORY, utils.TEST_REPOSITORY)
+        ):
+            # As of 2024-01-01, PyPI requires API tokens for uploads, meaning
+            # that the username is invariant.
+            return "__token__"
+
         return utils.get_userpass_value(
             self.input.username,
             self.config,
             key="username",
             prompt_strategy=self.username_from_keyring_or_prompt,
         )
 
@@ -86,15 +93,24 @@
 
     def password_from_keyring_or_prompt(self) -> str:
         password = self.get_password_from_keyring()
         if password:
             logger.info("password set from keyring")
             return password
 
-        return self.prompt("password", getpass.getpass)
+        # As of 2024-01-01, PyPI requires API tokens for uploads;
+        # specialize the prompt to clarify that an API token must be provided.
+        if cast(str, self.config["repository"]).startswith(
+            (utils.DEFAULT_REPOSITORY, utils.TEST_REPOSITORY)
+        ):
+            prompt = "API token"
+        else:
+            prompt = "password"
+
+        return self.prompt(prompt, getpass.getpass)
 
     def prompt(self, what: str, how: Callable[..., str]) -> str:
         return how(f"Enter your {what}: ")
 
 
 class Private(Resolver):
     def prompt(self, what: str, how: Optional[Callable[..., str]] = None) -> str:
```

### Comparing `twine-4.0.2/twine/cli.py` & `twine-5.0.0/twine/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         "importlib-metadata",
         "keyring",
         "pkginfo",
         "requests",
         "requests-toolbelt",
         "urllib3",
     )
-    return [(dep, importlib_metadata.version(dep)) for dep in deps]  # type: ignore[no-untyped-call] # python/importlib_metadata#288  # noqa: E501
+    return [(dep, importlib_metadata.version(dep)) for dep in deps]
 
 
 def dep_versions() -> str:
     return ", ".join(
         "{}: {}".format(*dependency) for dependency in list_dependencies_and_versions()
     )
 
@@ -114,10 +114,10 @@
         help=argparse.SUPPRESS,
         nargs=argparse.REMAINDER,
     )
     parser.parse_args(argv, namespace=args)
 
     configure_output()
 
-    main = registered_commands[args.command].load()
+    main = registered_commands[args.command].load()  # type: ignore[no-untyped-call] # python/importlib_metadata#288  # noqa: E501
 
     return main(args.args)
```

### Comparing `twine-4.0.2/twine/commands/__init__.py` & `twine-5.0.0/twine/commands/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Module containing the logic for the ``twine`` sub-commands.
 
 The contents of this package are not a public API. For more details, see
 https://github.com/pypa/twine/issues/194 and https://github.com/pypa/twine/issues/665.
 """
+
 # Copyright 2013 Donald Stufft
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # https://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `twine-4.0.2/twine/commands/check.py` & `twine-5.0.0/twine/commands/check.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 """Module containing the logic for ``twine check``."""
+
 # Copyright 2018 Dustin Ingram
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import argparse
-import cgi
+import email.message
 import io
 import logging
 import re
-from typing import List, Optional, Tuple, cast
+from typing import Dict, List, Optional, Tuple, cast
 
 import readme_renderer.rst
 from rich import print
 
 from twine import commands
 from twine import package as package_file
 
@@ -59,14 +60,24 @@
 
         return super().write(text)
 
     def __str__(self) -> str:
         return self.getvalue().strip()
 
 
+def _parse_content_type(value: str) -> Tuple[str, Dict[str, str]]:
+    """Implement logic of deprecated cgi.parse_header().
+
+    From https://docs.python.org/3.11/library/cgi.html#cgi.parse_header.
+    """
+    msg = email.message.EmailMessage()
+    msg["content-type"] = value
+    return msg.get_content_type(), msg["content-type"].params
+
+
 def _check_file(
     filename: str, render_warning_stream: _WarningStream
 ) -> Tuple[List[str], bool]:
     """Check given distribution."""
     warnings = []
     is_ok = True
 
@@ -78,15 +89,15 @@
 
     if description_content_type is None:
         warnings.append(
             "`long_description_content_type` missing. defaulting to `text/x-rst`."
         )
         description_content_type = "text/x-rst"
 
-    content_type, params = cgi.parse_header(description_content_type)
+    content_type, params = _parse_content_type(description_content_type)
     renderer = _RENDERERS.get(content_type, _RENDERERS[None])
 
     if description is None or description.rstrip() == "UNKNOWN":
         warnings.append("`long_description` missing.")
     elif renderer:
         rendering_result = renderer.render(
             description, stream=render_warning_stream, **params
```

### Comparing `twine-4.0.2/twine/commands/register.py` & `twine-5.0.0/twine/commands/register.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module containing the logic for ``twine register``."""
+
 # Copyright 2015 Ian Cordasco
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # https://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `twine-4.0.2/twine/commands/upload.py` & `twine-5.0.0/twine/commands/upload.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module containing the logic for ``twine upload``."""
+
 # Copyright 2013 Donald Stufft
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # https://www.apache.org/licenses/LICENSE-2.0
@@ -120,17 +121,43 @@
     repository_url = cast(str, upload_settings.repository_config["repository"])
     print(f"Uploading distributions to {repository_url}")
 
     packages_to_upload = [
         _make_package(filename, signatures, upload_settings) for filename in uploads
     ]
 
+    if any(p.gpg_signature for p in packages_to_upload):
+        if repository_url.startswith((utils.DEFAULT_REPOSITORY, utils.TEST_REPOSITORY)):
+            # Warn the user if they're trying to upload a PGP signature to PyPI
+            # or TestPyPI, which will (as of May 2023) ignore it.
+            # This warning is currently limited to just those indices, since other
+            # indices may still support PGP signatures.
+            logger.warning(
+                "One or more packages has an associated PGP signature; "
+                "these will be silently ignored by the index"
+            )
+        else:
+            # On other indices, warn the user that twine is considering
+            # removing PGP support outright.
+            logger.warning(
+                "One or more packages has an associated PGP signature; "
+                "a future version of twine may silently ignore these. "
+                "See https://github.com/pypa/twine/issues/1009 for more "
+                "information"
+            )
+
     repository = upload_settings.create_repository()
     uploaded_packages = []
 
+    if signatures and not packages_to_upload:
+        raise exceptions.InvalidDistribution(
+            "Cannot upload signed files by themselves, must upload with a "
+            "corresponding distribution file."
+        )
+
     for package in packages_to_upload:
         skip_message = (
             f"Skipping {package.basefilename} because it appears to already exist"
         )
 
         # Note: The skip_existing check *needs* to be first, because otherwise
         #       we're going to generate extra HTTP requests against a hardcoded
```

### Comparing `twine-4.0.2/twine/exceptions.py` & `twine-5.0.0/twine/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module containing exceptions raised by twine."""
+
 # Copyright 2015 Ian Stapleton Cordasco
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # https://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `twine-4.0.2/twine/package.py` & `twine-5.0.0/twine/package.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 import hashlib
 import io
 import logging
 import os
 import re
 import subprocess
-from typing import Dict, NamedTuple, Optional, Sequence, Tuple, Union
+from typing import Dict, NamedTuple, Optional, Sequence, Tuple, Union, cast
 
 import importlib_metadata
 import pkginfo
 from rich import print
 
 from twine import exceptions
 from twine import wheel
@@ -39,15 +39,15 @@
     ".exe": "bdist_wininst",
     ".egg": "bdist_egg",
     ".tar.bz2": "sdist",
     ".tar.gz": "sdist",
     ".zip": "sdist",
 }
 
-MetadataValue = Union[str, Sequence[str]]
+MetadataValue = Union[Optional[str], Sequence[str], Tuple[str, bytes]]
 
 logger = logging.getLogger(__name__)
 
 
 def _safe_name(name: str) -> str:
     """Convert an arbitrary string to a standard distribution name.
 
@@ -120,34 +120,32 @@
                 "Make sure the distribution includes the files where those fields "
                 "are specified, and is using a supported Metadata-Version: "
                 f"{', '.join(supported_metadata)}."
             )
 
         py_version: Optional[str]
         if dtype == "bdist_egg":
-            (dist,) = importlib_metadata.Distribution.discover(  # type: ignore[no-untyped-call] # python/importlib_metadata#288  # noqa: E501
-                path=[filename]
-            )
+            (dist,) = importlib_metadata.Distribution.discover(path=[filename])
             py_version = dist.metadata["Version"]
         elif dtype == "bdist_wheel":
-            py_version = meta.py_version
+            py_version = cast(wheel.Wheel, meta).py_version
         elif dtype == "bdist_wininst":
-            py_version = meta.py_version
+            py_version = cast(wininst.WinInst, meta).py_version
         else:
             py_version = None
 
         return cls(filename, comment, meta, py_version, dtype)
 
     def metadata_dictionary(self) -> Dict[str, MetadataValue]:
         """Merge multiple sources of metadata into a single dictionary.
 
         Includes values from filename, PKG-INFO, hashers, and signature.
         """
         meta = self.metadata
-        data = {
+        data: Dict[str, MetadataValue] = {
             # identify release
             "name": self.safe_name,
             "version": meta.version,
             # file content
             "filetype": self.filetype,
             "pyversion": self.python_version,
             # additional meta-data
```

### Comparing `twine-4.0.2/twine/repository.py` & `twine-5.0.0/twine/repository.py`

 * *Files identical despite different names*

### Comparing `twine-4.0.2/twine/settings.py` & `twine-5.0.0/twine/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module containing logic for handling settings."""
+
 # Copyright 2018 Ian Stapleton Cordasco
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # https://www.apache.org/licenses/LICENSE-2.0
@@ -123,22 +124,20 @@
         self.auth = auth.Resolver.choose(not non_interactive)(
             self.repository_config,
             auth.CredentialInput(username, password),
         )
 
     @property
     def username(self) -> Optional[str]:
-        # Workaround for https://github.com/python/mypy/issues/5858
-        return cast(Optional[str], self.auth.username)
+        return self.auth.username
 
     @property
     def password(self) -> Optional[str]:
         with self._allow_noninteractive():
-            # Workaround for https://github.com/python/mypy/issues/5858
-            return cast(Optional[str], self.auth.password)
+            return self.auth.password
 
     def _allow_noninteractive(self) -> "contextlib.AbstractContextManager[None]":
         """Bypass NonInteractive error when client cert is present."""
         suppressed = (exceptions.NonInteractive,) if self.client_cert else ()
         return contextlib.suppress(*suppressed)
 
     @property
@@ -293,17 +292,14 @@
         self, repository_name: str, repository_url: Optional[str]
     ) -> None:
         self.repository_config = utils.get_repository_from_config(
             self.config_file,
             repository_name,
             repository_url,
         )
-        self.repository_config["repository"] = utils.normalize_repository_url(
-            cast(str, self.repository_config["repository"]),
-        )
 
     def _handle_certificates(
         self, cacert: Optional[str], client_cert: Optional[str]
     ) -> None:
         self.cacert = utils.get_cacert(cacert, self.repository_config)
         self.client_cert = utils.get_clientcert(client_cert, self.repository_config)
```

### Comparing `twine-4.0.2/twine/utils.py` & `twine-5.0.0/twine/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import collections
 import configparser
 import functools
 import logging
 import os
 import os.path
 import unicodedata
-from typing import Any, Callable, DefaultDict, Dict, Optional, Sequence, Union
+from typing import Any, Callable, DefaultDict, Dict, Optional, Sequence, Union, cast
 from urllib.parse import urlparse
 from urllib.parse import urlunparse
 
 import requests
 import rfc3986
 
 from twine import exceptions
@@ -129,23 +129,26 @@
         return {
             "repository": repository_url,
             "username": None,
             "password": None,
         }
 
     try:
-        return get_config(config_file)[repository]
+        config = get_config(config_file)[repository]
     except OSError as exc:
         raise exceptions.InvalidConfiguration(str(exc))
     except KeyError:
         raise exceptions.InvalidConfiguration(
             f"Missing '{repository}' section from {config_file}.\n"
             f"More info: https://packaging.python.org/specifications/pypirc/ "
         )
 
+    config["repository"] = normalize_repository_url(cast(str, config["repository"]))
+    return config
+
 
 _HOSTNAMES = {
     "pypi.python.org",
     "testpypi.python.org",
     "upload.pypi.org",
     "test.pypi.org",
 }
```

### Comparing `twine-4.0.2/twine/wheel.py` & `twine-5.0.0/twine/wheel.py`

 * *Files identical despite different names*

### Comparing `twine-4.0.2/twine/wininst.py` & `twine-5.0.0/twine/wininst.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,17 +39,15 @@
         else:
             raise exceptions.InvalidDistribution(
                 "Not a known archive format for file: %s" % fqn
             )
 
         try:
             tuples = [
-                x.split("/")
-                for x in names
-                if x.endswith(".egg-info") or x.endswith("PKG-INFO")
+                x.split("/") for x in names if x.endswith((".egg-info", "PKG-INFO"))
             ]
             schwarz = sorted((len(x), x) for x in tuples)
             for path in [x[1] for x in schwarz]:
                 candidate = "/".join(path)
                 data = read_file(candidate)
                 if b"Metadata-Version" in data:
                     return data
```

### Comparing `twine-4.0.2/twine.egg-info/PKG-INFO` & `twine-5.0.0/twine.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twine
-Version: 4.0.2
+Version: 5.0.0
 Summary: Collection of utilities for publishing packages on PyPI
 Home-page: https://twine.readthedocs.io/
 Author: Donald Stufft and individual contributors
 Author-email: donald@stufft.io
 Project-URL: Source, https://github.com/pypa/twine/
 Project-URL: Documentation, https://twine.readthedocs.io/en/latest/
 Project-URL: Packaging tutorial, https://packaging.python.org/tutorials/packaging-projects/
@@ -15,33 +15,43 @@
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: BSD
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: pkginfo>=1.8.1
+Requires-Dist: readme-renderer>=35.0
+Requires-Dist: requests>=2.20
+Requires-Dist: requests-toolbelt!=0.9.0,>=0.8.0
+Requires-Dist: urllib3>=1.26.0
+Requires-Dist: importlib-metadata>=3.6
+Requires-Dist: keyring>=15.1
+Requires-Dist: rfc3986>=1.4.0
+Requires-Dist: rich>=12.0.0
 
 .. image:: https://img.shields.io/pypi/v/twine.svg
    :target: https://pypi.org/project/twine
 
 .. image:: https://img.shields.io/pypi/pyversions/twine.svg
    :target: https://pypi.org/project/twine
 
 .. image:: https://img.shields.io/readthedocs/twine
    :target: https://twine.readthedocs.io
 
-.. image:: https://img.shields.io/github/workflow/status/pypa/twine/Main
+.. image:: https://img.shields.io/github/actions/workflow/status/pypa/twine/main.yml?branch=main
    :target: https://github.com/pypa/twine/actions
 
 twine
 =====
 
 Twine is a utility for `publishing`_ Python packages on `PyPI`_.
```

### Comparing `twine-4.0.2/twine.egg-info/SOURCES.txt` & `twine-5.0.0/twine.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,30 @@
-.codecov.yml
 .coveragerc
 .flake8
 .git-blame-ignore-revs
 .gitignore
 .isort.cfg
 .readthedocs.yaml
 AUTHORS
 LICENSE
 README.rst
 mypy.ini
 pyproject.toml
 pytest.ini
 setup.cfg
 tox.ini
-.github/ISSUE_TEMPLATE.md
+.github/dependabot.yml
+.github/ISSUE_TEMPLATE/01_upload_failed.yml
+.github/ISSUE_TEMPLATE/02_bug.yml
+.github/ISSUE_TEMPLATE/03_feature.yml
+.github/ISSUE_TEMPLATE/04_other.yml
+.github/ISSUE_TEMPLATE/config.yml
 .github/workflows/codeql-analysis.yml
 .github/workflows/main.yml
+.github/workflows/release.yml
 changelog/.gitignore
 docs/changelog.rst
 docs/conf.py
 docs/contributing.rst
 docs/index.rst
 docs/requirements.txt
 docs/internal/twine.auth.rst
```

