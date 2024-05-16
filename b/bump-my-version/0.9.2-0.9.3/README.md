# Comparing `tmp/bump-my-version-0.9.2.tar.gz` & `tmp/bump-my-version-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bump-my-version-0.9.2.tar", last modified: Mon Aug  7 14:13:59 2023, max compression
+gzip compressed data, was "bump-my-version-0.9.3.tar", last modified: Fri Aug 25 14:20:48 2023, max compression
```

## Comparing `bump-my-version-0.9.2.tar` & `bump-my-version-0.9.3.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:13:59.077245 bump-my-version-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)    23198 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)    10135 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-08-07 14:13:59.077245 bump-my-version-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6855 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:13:59.069244 bump-my-version-0.9.2/bump_my_version.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-08-07 14:13:59.000000 bump-my-version-0.9.2/bump_my_version.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-08-07 14:13:59.000000 bump-my-version-0.9.2/bump_my_version.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 14:13:59.000000 bump-my-version-0.9.2/bump_my_version.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-07 14:13:59.000000 bump-my-version-0.9.2/bump_my_version.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-08-07 14:13:59.000000 bump-my-version-0.9.2/bump_my_version.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-07 14:13:59.000000 bump-my-version-0.9.2/bump_my_version.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:13:59.073244 bump-my-version-0.9.2/bumpversion/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/bumpversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/bumpversion/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/bumpversion/aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/bumpversion/autocast.py
--rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/bumpversion/bump.py
--rw-r--r--   0 runner    (1001) docker     (123)    13849 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/bumpversion/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    14241 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/bumpversion/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/bumpversion/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10003 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/bumpversion/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/bumpversion/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/bumpversion/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    13150 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/bumpversion/scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/bumpversion/show.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/bumpversion/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/bumpversion/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/bumpversion/version_part.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/bumpversion/yaml_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-07 14:13:59.077245 bump-my-version-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:13:59.073244 bump-my-version-0.9.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:13:59.073244 bump-my-version-0.9.2/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/fixtures/basic_cfg.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/fixtures/basic_cfg.toml
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/fixtures/basic_cfg_expected.json
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/fixtures/basic_cfg_expected.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/fixtures/basic_cfg_expected.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/fixtures/basic_cfg_expected_full.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:13:59.073244 bump-my-version-0.9.2/tests/fixtures/csharp/
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/fixtures/csharp/.bumpversion.toml
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/fixtures/csharp/AssemblyInfo.cs
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/fixtures/csharp/FULL_VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/fixtures/csharp/Version.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:13:59.077245 bump-my-version-0.9.2/tests/fixtures/glob/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:13:59.077245 bump-my-version-0.9.2/tests/fixtures/glob/directory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/fixtures/glob/directory/file3.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/fixtures/glob/file1.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/fixtures/glob/file2.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/fixtures/glob/not-text.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:13:59.077245 bump-my-version-0.9.2/tests/fixtures/interpolation/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/fixtures/interpolation/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/fixtures/interpolation/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/fixtures/interpolation/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/fixtures/pep440.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/test_autocast.py
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/test_bump.py
--rw-r--r--   0 runner    (1001) docker     (123)    18732 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8951 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    16079 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/test_show.py
--rw-r--r--   0 runner    (1001) docker     (123)    11946 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/test_version_part.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/test_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 14:20:48.059519 bump-my-version-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (999)    25242 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (999)     4900 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (999)    10135 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (999)     1075 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (999)      162 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (999)     9452 2023-08-25 14:20:48.059519 bump-my-version-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)     6805 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 14:20:48.051519 bump-my-version-0.9.3/bump_my_version.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (999)     9452 2023-08-25 14:20:48.000000 bump-my-version-0.9.3/bump_my_version.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)     1631 2023-08-25 14:20:48.000000 bump-my-version-0.9.3/bump_my_version.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-25 14:20:48.000000 bump-my-version-0.9.3/bump_my_version.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       90 2023-08-25 14:20:48.000000 bump-my-version-0.9.3/bump_my_version.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (999)      310 2023-08-25 14:20:48.000000 bump-my-version-0.9.3/bump_my_version.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       31 2023-08-25 14:20:48.000000 bump-my-version-0.9.3/bump_my_version.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 14:20:48.055519 bump-my-version-0.9.3/bumpversion/
+-rw-r--r--   0 runner    (1001) docker     (999)       73 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/bumpversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)       73 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/bumpversion/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1925 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/bumpversion/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2245 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/bumpversion/autocast.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4019 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/bumpversion/bump.py
+-rw-r--r--   0 runner    (1001) docker     (999)    13849 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/bumpversion/cli.py
+-rw-r--r--   0 runner    (1001) docker     (999)    14253 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/bumpversion/config.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1243 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/bumpversion/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (999)    10003 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/bumpversion/files.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3373 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/bumpversion/functions.py
+-rw-r--r--   0 runner    (1001) docker     (999)      747 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/bumpversion/logging.py
+-rw-r--r--   0 runner    (1001) docker     (999)    13150 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/bumpversion/scm.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5016 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/bumpversion/show.py
+-rw-r--r--   0 runner    (1001) docker     (999)      391 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/bumpversion/ui.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1781 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/bumpversion/utils.py
+-rw-r--r--   0 runner    (1001) docker     (999)    10465 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/bumpversion/version_part.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3709 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/bumpversion/yaml_dump.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5879 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (999)       66 2023-08-25 14:20:48.059519 bump-my-version-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (999)       62 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 14:20:48.055519 bump-my-version-0.9.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (999)       41 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1694 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 14:20:48.059519 bump-my-version-0.9.3/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (999)      556 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/tests/fixtures/basic_cfg.cfg
+-rw-r--r--   0 runner    (1001) docker     (999)      865 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/tests/fixtures/basic_cfg.toml
+-rw-r--r--   0 runner    (1001) docker     (999)      632 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/tests/fixtures/basic_cfg_expected.json
+-rw-r--r--   0 runner    (1001) docker     (999)     2750 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/tests/fixtures/basic_cfg_expected.txt
+-rw-r--r--   0 runner    (1001) docker     (999)     2118 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/tests/fixtures/basic_cfg_expected.yaml
+-rw-r--r--   0 runner    (1001) docker     (999)     2562 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/tests/fixtures/basic_cfg_expected_full.json
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 14:20:48.059519 bump-my-version-0.9.3/tests/fixtures/csharp/
+-rw-r--r--   0 runner    (1001) docker     (999)     1540 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/tests/fixtures/csharp/.bumpversion.toml
+-rw-r--r--   0 runner    (1001) docker     (999)       97 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/tests/fixtures/csharp/AssemblyInfo.cs
+-rw-r--r--   0 runner    (1001) docker     (999)       20 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/tests/fixtures/csharp/FULL_VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       22 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/tests/fixtures/csharp/Version.csv
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 14:20:48.059519 bump-my-version-0.9.3/tests/fixtures/glob/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 14:20:48.059519 bump-my-version-0.9.3/tests/fixtures/glob/directory/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/tests/fixtures/glob/directory/file3.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/tests/fixtures/glob/file1.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/tests/fixtures/glob/file2.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/tests/fixtures/glob/not-text.md
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 14:20:48.059519 bump-my-version-0.9.3/tests/fixtures/interpolation/
+-rw-r--r--   0 runner    (1001) docker     (999)      136 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/tests/fixtures/interpolation/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (999)      168 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/tests/fixtures/interpolation/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (999)      139 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/tests/fixtures/interpolation/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (999)     1619 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/tests/fixtures/pep440.toml
+-rw-r--r--   0 runner    (1001) docker     (999)     2418 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/tests/test_autocast.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6580 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/tests/test_bump.py
+-rw-r--r--   0 runner    (1001) docker     (999)    18732 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (999)     8951 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (999)    16705 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2044 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (999)     7535 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/tests/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5417 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/tests/test_show.py
+-rw-r--r--   0 runner    (1001) docker     (999)    11946 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/tests/test_version_part.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2059 2023-08-25 14:20:19.000000 bump-my-version-0.9.3/tests/test_yaml.py
```

### Comparing `bump-my-version-0.9.2/CHANGELOG.md` & `bump-my-version-0.9.3/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,49 @@
 # Changelog
 
+## 0.9.3 (2023-08-25)
+[Compare the full difference.](https://github.com/callowayproject/bump-my-version/compare/0.9.2...0.9.3)
+
+### Fixes
+
+- Fixed file configuration overrides. [c1ef3b2](https://github.com/callowayproject/bump-my-version/commit/c1ef3b290746e10e24dcdcb56c52effb6b324464)
+    
+  Fixes #55
+
+  The file config was ignoring falsey values when constructing the dict.
+
+  It now ignores `None` values.
+- Fixed documentation regarding regex config. [cd71a1a](https://github.com/callowayproject/bump-my-version/commit/cd71a1a4216286e49e0d1b8b9d867a26ee88eff8)
+    
+  - TOML requires the double backslash while INI doesn't
+- Fixed requirements for docs. [7856ee0](https://github.com/callowayproject/bump-my-version/commit/7856ee01559289e943a26af7e36382855973e485)
+    
+### New
+
+- Added documentation building workflow. [48980d7](https://github.com/callowayproject/bump-my-version/commit/48980d7d3445a323c7f8532a8edd61dc09d3fb51)
+    
+### Other
+
+- [pre-commit.ci] pre-commit autoupdate. [7c38c40](https://github.com/callowayproject/bump-my-version/commit/7c38c401a3755329bce5f127a956e4603c7c4645)
+    
+  **updates:** - [github.com/astral-sh/ruff-pre-commit: v0.0.284 → v0.0.285](https://github.com/astral-sh/ruff-pre-commit/compare/v0.0.284...v0.0.285)
+
+- [pre-commit.ci] pre-commit autoupdate. [c30bd12](https://github.com/callowayproject/bump-my-version/commit/c30bd128ca27adea1a93876a29656c5cb7f6d178)
+    
+  **updates:** - [github.com/astral-sh/ruff-pre-commit: v0.0.282 → v0.0.284](https://github.com/astral-sh/ruff-pre-commit/compare/v0.0.282...v0.0.284)
+
+- [pre-commit.ci] pre-commit autoupdate. [95c89fb](https://github.com/callowayproject/bump-my-version/commit/95c89fb94ea6cfa5c9d28ed06ee6def9f98ab59f)
+    
+  **updates:** - [github.com/astral-sh/ruff-pre-commit: v0.0.281 → v0.0.282](https://github.com/astral-sh/ruff-pre-commit/compare/v0.0.281...v0.0.282)
+
+### Updates
+
+- Removed mentions of Python 3.7. [a91f690](https://github.com/callowayproject/bump-my-version/commit/a91f690ab2c36bef9243058f9e9bbdc1968e9af1)
+    
+
 ## 0.9.2 (2023-08-07)
 [Compare the full difference.](https://github.com/callowayproject/bump-my-version/compare/0.9.1...0.9.2)
 
 ### Fixes
 
 - Fixed modified context when committing. [130bbe0](https://github.com/callowayproject/bump-my-version/commit/130bbe0dc9cbc436ed2d4a74878937fc784fbccd)
```

### Comparing `bump-my-version-0.9.2/CODE_OF_CONDUCT.md` & `bump-my-version-0.9.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.2/CONTRIBUTING.md` & `bump-my-version-0.9.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.2/LICENSE` & `bump-my-version-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.2/PKG-INFO` & `bump-my-version-0.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bump-my-version
-Version: 0.9.2
+Version: 0.9.3
 Summary: Version bump your Python project
 Author-email: Corey Oordt <coreyoordt@gmail.com>
 License: MIT License
         
         Copyright (c) 2013-2014 Filip Noetzel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,15 +32,14 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Build Tools
@@ -77,15 +76,15 @@
 
 A small command line tool to simplify releasing software by updating all version strings in your source code by the correct increment and optionally commit and tag the changes.
 
 * version formats are highly configurable
 * works without any source code manager, but happily reads tag information from and writes
   commits and tags to Git and Mercurial if available
 * just handles text files, so it's not specific to any programming language
-* supports Python 3.8+ and PyPy3. Python 3.7 should work but isn't actively tested.
+* supports Python 3.8+ and PyPy3.
 
 ## Future Direction
 
 - Make it easier to get the current version
 - Switch having both the version part and files to change as arguments on the command line.
 - Make the version part argument _truly_ optional when `--new-version` is specified
 - Allow for multiple tags, including one that moves for having a `v2` that always points to the latest version of version 2. [For example](https://github.com/actions/toolkit/blob/master/docs/action-versioning.md#recommendations)
```

### Comparing `bump-my-version-0.9.2/README.md` & `bump-my-version-0.9.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 A small command line tool to simplify releasing software by updating all version strings in your source code by the correct increment and optionally commit and tag the changes.
 
 * version formats are highly configurable
 * works without any source code manager, but happily reads tag information from and writes
   commits and tags to Git and Mercurial if available
 * just handles text files, so it's not specific to any programming language
-* supports Python 3.8+ and PyPy3. Python 3.7 should work but isn't actively tested.
+* supports Python 3.8+ and PyPy3.
 
 ## Future Direction
 
 - Make it easier to get the current version
 - Switch having both the version part and files to change as arguments on the command line.
 - Make the version part argument _truly_ optional when `--new-version` is specified
 - Allow for multiple tags, including one that moves for having a `v2` that always points to the latest version of version 2. [For example](https://github.com/actions/toolkit/blob/master/docs/action-versioning.md#recommendations)
```

### Comparing `bump-my-version-0.9.2/bump_my_version.egg-info/PKG-INFO` & `bump-my-version-0.9.3/bump_my_version.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bump-my-version
-Version: 0.9.2
+Version: 0.9.3
 Summary: Version bump your Python project
 Author-email: Corey Oordt <coreyoordt@gmail.com>
 License: MIT License
         
         Copyright (c) 2013-2014 Filip Noetzel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,15 +32,14 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Build Tools
@@ -77,15 +76,15 @@
 
 A small command line tool to simplify releasing software by updating all version strings in your source code by the correct increment and optionally commit and tag the changes.
 
 * version formats are highly configurable
 * works without any source code manager, but happily reads tag information from and writes
   commits and tags to Git and Mercurial if available
 * just handles text files, so it's not specific to any programming language
-* supports Python 3.8+ and PyPy3. Python 3.7 should work but isn't actively tested.
+* supports Python 3.8+ and PyPy3.
 
 ## Future Direction
 
 - Make it easier to get the current version
 - Switch having both the version part and files to change as arguments on the command line.
 - Make the version part argument _truly_ optional when `--new-version` is specified
 - Allow for multiple tags, including one that moves for having a `v2` that always points to the latest version of version 2. [For example](https://github.com/actions/toolkit/blob/master/docs/action-versioning.md#recommendations)
```

### Comparing `bump-my-version-0.9.2/bump_my_version.egg-info/SOURCES.txt` & `bump-my-version-0.9.3/bump_my_version.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.2/bumpversion/aliases.py` & `bump-my-version-0.9.3/bumpversion/aliases.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.2/bumpversion/autocast.py` & `bump-my-version-0.9.3/bumpversion/autocast.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.2/bumpversion/bump.py` & `bump-my-version-0.9.3/bumpversion/bump.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.2/bumpversion/cli.py` & `bump-my-version-0.9.3/bumpversion/cli.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.2/bumpversion/config.py` & `bump-my-version-0.9.3/bumpversion/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
         "parse": config_dict["parse"],
         "serialize": config_dict["serialize"],
         "search": config_dict["search"],
         "replace": config_dict["replace"],
         "ignore_missing_version": config_dict["ignore_missing_version"],
         "no_regex": config_dict["no_regex"],
     }
-    files = [{k: v for k, v in filecfg.items() if v} for filecfg in config_dict["files"]]
+    files = [{k: v for k, v in filecfg.items() if v is not None} for filecfg in config_dict["files"]]
     for f in files:
         f.update({k: v for k, v in defaults.items() if k not in f})
     return [FileConfig(**f) for f in files]
 
 
 def get_configuration(config_file: Union[str, Path, None] = None, **overrides) -> Config:
     """
```

### Comparing `bump-my-version-0.9.2/bumpversion/exceptions.py` & `bump-my-version-0.9.3/bumpversion/exceptions.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.2/bumpversion/files.py` & `bump-my-version-0.9.3/bumpversion/files.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.2/bumpversion/functions.py` & `bump-my-version-0.9.3/bumpversion/functions.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.2/bumpversion/logging.py` & `bump-my-version-0.9.3/bumpversion/logging.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.2/bumpversion/scm.py` & `bump-my-version-0.9.3/bumpversion/scm.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.2/bumpversion/show.py` & `bump-my-version-0.9.3/bumpversion/show.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.2/bumpversion/utils.py` & `bump-my-version-0.9.3/bumpversion/utils.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.2/bumpversion/version_part.py` & `bump-my-version-0.9.3/bumpversion/version_part.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.2/bumpversion/yaml_dump.py` & `bump-my-version-0.9.3/bumpversion/yaml_dump.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.2/pyproject.toml` & `bump-my-version-0.9.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 [build-system]
-
-requires = [
-    "setuptools >= 40.9.0",
-    "wheel",
-]
+requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bump-my-version"
 description = "Version bump your Python project"
 authors = [
     { name = "Corey Oordt", email = "coreyoordt@gmail.com" }
@@ -16,15 +12,14 @@
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Software Development :: Build Tools",
@@ -63,14 +58,15 @@
 ]
 docs = [
     "ghp-import",
     "linkify-it-py",
     "myst-parser",
     "furo",
     "Sphinx>=4.3.0",
+    "sphinx-autodoc2",
     "sphinx-autodoc-typehints",
     "sphinx-click",
     "sphinx-copybutton",
 ]
 test = [
     "coverage",
     "pre-commit",
@@ -154,14 +150,15 @@
 # "UP" "TRY" "PLR"
 select = ["E", "W", "F", "I", "N", "B", "BLE", "C", "D", "E", "F", "I", "N", "S", "T", "W", "RUF", "NPY", "PD", "PGH", "ANN", "C90", "PLC", "PLE", "PLW", "TCH"]
 ignore = [
     "ANN002", "ANN003", "ANN101", "ANN102", "ANN204", "ANN401",
     "S101", "S104",
     "D105", "D106", "D107", "D200", "D212",
     "PD011",
+    "PLW1510",
 ]
 
 # Allow autofix for all enabled rules (when `--fix`) is provided.
 fixable = ["E", "W", "F", "I", "N", "B", "BLE", "C", "D", "E", "F", "I", "N", "S", "T", "W", "RUF", "NPY", "PD", "PGH", "ANN", "C90", "PL", "PLC", "PLE", "PLW", "TCH"]
 unfixable = []
 
 # Exclude a variety of commonly ignored directories.
@@ -206,23 +203,23 @@
 [tool.ruff.isort]
 order-by-type = true
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
 [tool.bumpversion]
-current_version = "0.9.2"
+current_version = "0.9.3"
 commit = true
 commit_args = "--no-verify"
 tag = true
 tag_name = "{new_version}"
 allow_dirty = true
-parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)(\\.(?P<dev>dev\\d+))?"
+parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)(\\.(?P<dev>dev)\\d+\\+[-_a-zA-Z0-9]+)?"
 serialize = [
-    "{major}.{minor}.{patch}.{dev}{distance_to_latest_tag}",
+    "{major}.{minor}.{patch}.{dev}{distance_to_latest_tag}+{short_branch_name}",
     "{major}.{minor}.{patch}"
 ]
 message = "Version updated from {current_version} to {new_version}"
 
 [tool.bumpversion.parts.dev]
 values = ["release", "dev"]
```

### Comparing `bump-my-version-0.9.2/tests/conftest.py` & `bump-my-version-0.9.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.2/tests/fixtures/basic_cfg.cfg` & `bump-my-version-0.9.3/tests/fixtures/basic_cfg.cfg`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.2/tests/fixtures/basic_cfg.toml` & `bump-my-version-0.9.3/tests/fixtures/basic_cfg.toml`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.2/tests/fixtures/basic_cfg_expected.json` & `bump-my-version-0.9.3/tests/fixtures/basic_cfg_expected.json`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.2/tests/fixtures/basic_cfg_expected.txt` & `bump-my-version-0.9.3/tests/fixtures/basic_cfg_expected.txt`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.2/tests/fixtures/basic_cfg_expected.yaml` & `bump-my-version-0.9.3/tests/fixtures/basic_cfg_expected.yaml`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.2/tests/fixtures/basic_cfg_expected_full.json` & `bump-my-version-0.9.3/tests/fixtures/basic_cfg_expected_full.json`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.2/tests/fixtures/csharp/.bumpversion.toml` & `bump-my-version-0.9.3/tests/fixtures/csharp/.bumpversion.toml`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.2/tests/fixtures/pep440.toml` & `bump-my-version-0.9.3/tests/fixtures/pep440.toml`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.2/tests/test_autocast.py` & `bump-my-version-0.9.3/tests/test_autocast.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.2/tests/test_bump.py` & `bump-my-version-0.9.3/tests/test_bump.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.2/tests/test_cli.py` & `bump-my-version-0.9.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.2/tests/test_config.py` & `bump-my-version-0.9.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.2/tests/test_files.py` & `bump-my-version-0.9.3/tests/test_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -345,32 +345,45 @@
         cfg_file = files.ConfiguredFile(file_cfg, version_config)
         cfg_file.replace_version(current_version, new_version, get_context(conf))
 
     # Assert
     assert alphabet_path.read_text() == "A\nB\nC\n10.0.0\n"
 
 
-def test_ignore_missing_version(tmp_path: Path) -> None:
+@pytest.mark.parametrize(
+    ["global_value", "file_value", "should_raise"],
+    [
+        param(True, True, False, id="ignore global and file"),
+        param(True, False, True, id="ignore global only"),
+        param(False, True, False, id="ignore file only"),
+        param(False, False, True, id="ignore none"),
+    ],
+)
+def test_ignore_missing_version(global_value: bool, file_value: bool, should_raise: bool, tmp_path: Path) -> None:
     """If the version is not found in the file, do nothing."""
     # Arrange
     version_path = tmp_path / Path("VERSION")
     version_path.write_text("1.2.3")
 
     overrides = {
         "current_version": "1.2.5",
-        "ignore_missing_version": True,
-        "files": [{"filename": str(version_path)}],
+        "ignore_missing_version": global_value,
+        "files": [{"filename": str(version_path), "ignore_missing_version": file_value}],
     }
-    conf, version_config, current_version = get_config_data(overrides)
-    assert conf.ignore_missing_version is True
-    new_version = current_version.bump("patch", version_config.order)
-    cfg_files = [files.ConfiguredFile(file_cfg, version_config) for file_cfg in conf.files]
-
-    # Act
-    files.modify_files(cfg_files, current_version, new_version, get_context(conf))
+    with inside_dir(tmp_path):
+        conf, version_config, current_version = get_config_data(overrides)
+        new_version = current_version.bump("patch", version_config.order)
+        cfg_files = [files.ConfiguredFile(file_cfg, version_config) for file_cfg in conf.files]
+
+        # Act
+        if should_raise:
+            with pytest.raises(VersionNotFoundError):
+                files.modify_files(cfg_files, current_version, new_version, get_context(conf))
+        else:
+            files.modify_files(cfg_files, current_version, new_version, get_context(conf))
 
     # Assert
     assert version_path.read_text() == "1.2.3"
 
 
 def test_regex_search(tmp_path: Path) -> None:
     """A regex search string is found and replaced."""
```

### Comparing `bump-my-version-0.9.2/tests/test_functions.py` & `bump-my-version-0.9.3/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.2/tests/test_scm.py` & `bump-my-version-0.9.3/tests/test_scm.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.2/tests/test_show.py` & `bump-my-version-0.9.3/tests/test_show.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.2/tests/test_version_part.py` & `bump-my-version-0.9.3/tests/test_version_part.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.2/tests/test_yaml.py` & `bump-my-version-0.9.3/tests/test_yaml.py`

 * *Files identical despite different names*

