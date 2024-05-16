# Comparing `tmp/chik_dev_tools-1.2.3.tar.gz` & `tmp/chik_dev_tools-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chik_dev_tools-1.2.3.tar", last modified: Mon Nov 27 01:46:27 2023, max compression
+gzip compressed data, was "chik_dev_tools-1.2.6.tar", last modified: Thu May 16 05:40:32 2024, max compression
```

## Comparing `chik_dev_tools-1.2.3.tar` & `chik_dev_tools-1.2.6.tar`

### file list

```diff
@@ -1,103 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 01:46:27.195728 chik_dev_tools-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 01:46:27.179728 chik_dev_tools-1.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 01:46:27.179728 chik_dev_tools-1.2.3/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 01:46:27.183728 chik_dev_tools-1.2.3/.github/actions/install/
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/.github/actions/install/action.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)       51 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/.github/actions/install/install.ps1
--rwxr-xr-x   0 runner    (1001) docker     (127)       65 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/.github/actions/install/install.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 01:46:27.183728 chik_dev_tools-1.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      832 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/.github/workflows/codeql-analysis.yml.bak
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/.github/workflows/precommit.yml.bak
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/.github/workflows/run-test-suite.yml.bak
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/.github/workflows/super-linter.yml.bak
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/.github/workflows/test-blockchain-main.yml.bak
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      110 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/.markdown-lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    10240 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5595 2023-11-27 01:46:27.195728 chik_dev_tools-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4151 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      230 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/activated.ps1
--rwxr-xr-x   0 runner    (1001) docker     (127)      624 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/activated.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      230 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/activated.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 01:46:27.187728 chik_dev_tools-1.2.3/cdv/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/cdv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 01:46:27.187728 chik_dev_tools-1.2.3/cdv/clibs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/cdv/clibs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/cdv/clibs/condition_codes.clib
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/cdv/clibs/curry_and_treehash.clib
--rw-r--r--   0 runner    (1001) docker     (127)      244 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/cdv/clibs/sha256tree.clib
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/cdv/clibs/singleton_truths.clib
--rw-r--r--   0 runner    (1001) docker     (127)      462 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/cdv/clibs/utility_macros.clib
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 01:46:27.187728 chik_dev_tools-1.2.3/cdv/cmds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/cdv/cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29953 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/cdv/cmds/chik_inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/cdv/cmds/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7439 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/cdv/cmds/clsp.py
--rw-r--r--   0 runner    (1001) docker     (127)    15105 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/cdv/cmds/rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/cdv/cmds/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 01:46:27.187728 chik_dev_tools-1.2.3/cdv/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/cdv/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 01:46:27.187728 chik_dev_tools-1.2.3/cdv/examples/clsp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/cdv/examples/clsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/cdv/examples/clsp/piggybank.clsp
--rw-r--r--   0 runner    (1001) docker     (127)      503 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/cdv/examples/clsp/piggybank.clsp.hex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 01:46:27.187728 chik_dev_tools-1.2.3/cdv/examples/drivers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/cdv/examples/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/cdv/examples/drivers/piggybank_drivers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 01:46:27.187728 chik_dev_tools-1.2.3/cdv/examples/klvm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/cdv/examples/klvm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 01:46:27.187728 chik_dev_tools-1.2.3/cdv/examples/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5273 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/cdv/examples/tests/test_piggybank.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 01:46:27.187728 chik_dev_tools-1.2.3/cdv/test/
--rw-r--r--   0 runner    (1001) docker     (127)    29257 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/cdv/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/cdv/test/test_skeleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 01:46:27.191728 chik_dev_tools-1.2.3/cdv/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/cdv/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/cdv/util/keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/cdv/util/load_klvm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 01:46:27.195728 chik_dev_tools-1.2.3/chik_dev_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5595 2023-11-27 01:46:27.000000 chik_dev_tools-1.2.3/chik_dev_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2023-11-27 01:46:27.000000 chik_dev_tools-1.2.3/chik_dev_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-27 01:46:27.000000 chik_dev_tools-1.2.3/chik_dev_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-11-27 01:46:27.000000 chik_dev_tools-1.2.3/chik_dev_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      232 2023-11-27 01:46:27.000000 chik_dev_tools-1.2.3/chik_dev_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-11-27 01:46:27.000000 chik_dev_tools-1.2.3/chik_dev_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      519 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)      676 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       94 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-27 01:46:27.195728 chik_dev_tools-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 01:46:27.191728 chik_dev_tools-1.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/tests/build-init-files.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 01:46:27.191728 chik_dev_tools-1.2.3/tests/cmds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/tests/cmds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 01:46:27.183728 chik_dev_tools-1.2.3/tests/cmds/object_files/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 01:46:27.191728 chik_dev_tools-1.2.3/tests/cmds/object_files/coinrecords/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/tests/cmds/object_files/coinrecords/coinrecord.hex
--rw-r--r--   0 runner    (1001) docker     (127)      325 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/tests/cmds/object_files/coinrecords/coinrecord.json
--rw-r--r--   0 runner    (1001) docker     (127)      336 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/tests/cmds/object_files/coinrecords/coinrecord_invalid.json
--rw-r--r--   0 runner    (1001) docker     (127)      296 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/tests/cmds/object_files/coinrecords/coinrecord_metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 01:46:27.191728 chik_dev_tools-1.2.3/tests/cmds/object_files/coins/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/tests/cmds/object_files/coins/coin.json
--rw-r--r--   0 runner    (1001) docker     (127)      189 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/tests/cmds/object_files/coins/coin_invalid.json
--rw-r--r--   0 runner    (1001) docker     (127)      256 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/tests/cmds/object_files/coins/coin_metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 01:46:27.191728 chik_dev_tools-1.2.3/tests/cmds/object_files/spendbundles/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/tests/cmds/object_files/spendbundles/spendbundle.hex
--rw-r--r--   0 runner    (1001) docker     (127)      591 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/tests/cmds/object_files/spendbundles/spendbundle.json
--rw-r--r--   0 runner    (1001) docker     (127)      557 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/tests/cmds/object_files/spendbundles/spendbundle_invalid.json
--rw-r--r--   0 runner    (1001) docker     (127)      467 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/tests/cmds/object_files/spendbundles/spendbundle_metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 01:46:27.195728 chik_dev_tools-1.2.3/tests/cmds/object_files/spends/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/tests/cmds/object_files/spends/spend.hex
--rw-r--r--   0 runner    (1001) docker     (127)      506 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/tests/cmds/object_files/spends/spend.json
--rw-r--r--   0 runner    (1001) docker     (127)      394 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/tests/cmds/object_files/spends/spend_2.json
--rw-r--r--   0 runner    (1001) docker     (127)      288 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/tests/cmds/object_files/spends/spend_invalid.json
--rw-r--r--   0 runner    (1001) docker     (127)      489 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/tests/cmds/object_files/spends/spend_metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/tests/cmds/test_cdv.py
--rw-r--r--   0 runner    (1001) docker     (127)     8407 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/tests/cmds/test_clsp.py
--rw-r--r--   0 runner    (1001) docker     (127)    17212 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/tests/cmds/test_inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2023-11-27 01:45:55.000000 chik_dev_tools-1.2.3/tests/test_skeleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:40:32.495314 chik_dev_tools-1.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:40:32.479313 chik_dev_tools-1.2.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:40:32.479313 chik_dev_tools-1.2.6/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:40:32.483313 chik_dev_tools-1.2.6/.github/actions/install/
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/.github/actions/install/action.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)       51 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/.github/actions/install/install.ps1
+-rwxr-xr-x   0 runner    (1001) docker     (127)       65 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/.github/actions/install/install.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:40:32.487313 chik_dev_tools-1.2.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/.github/workflows/codeql-analysis.yml.bak
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/.github/workflows/precommit.yml.bak
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/.github/workflows/run-test-suite.yml.bak
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/.github/workflows/super-linter.yml.bak
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/.github/workflows/test-blockchain-main.yml.bak
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/.markdown-lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/.repo-content-updater.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-05-16 05:40:32.495314 chik_dev_tools-1.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      230 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/activated.ps1
+-rwxr-xr-x   0 runner    (1001) docker     (127)      624 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/activated.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      237 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/activated.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:40:32.487313 chik_dev_tools-1.2.6/cdv/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/cdv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:40:32.487313 chik_dev_tools-1.2.6/cdv/clibs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/cdv/clibs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/cdv/clibs/condition_codes.clib
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/cdv/clibs/curry_and_treehash.clib
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/cdv/clibs/sha256tree.clib
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/cdv/clibs/singleton_truths.clib
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/cdv/clibs/utility_macros.clib
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:40:32.487313 chik_dev_tools-1.2.6/cdv/cmds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/cdv/cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30431 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/cdv/cmds/chik_inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/cdv/cmds/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7439 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/cdv/cmds/clsp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15105 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/cdv/cmds/rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/cdv/cmds/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:40:32.487313 chik_dev_tools-1.2.6/cdv/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/cdv/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:40:32.487313 chik_dev_tools-1.2.6/cdv/examples/clsp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/cdv/examples/clsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/cdv/examples/clsp/piggybank.clsp
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/cdv/examples/clsp/piggybank.clsp.hex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:40:32.487313 chik_dev_tools-1.2.6/cdv/examples/drivers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/cdv/examples/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/cdv/examples/drivers/piggybank_drivers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:40:32.487313 chik_dev_tools-1.2.6/cdv/examples/klvm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/cdv/examples/klvm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:40:32.487313 chik_dev_tools-1.2.6/cdv/examples/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5239 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/cdv/examples/tests/test_piggybank.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:40:32.487313 chik_dev_tools-1.2.6/cdv/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    29257 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/cdv/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/cdv/test/test_skeleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:40:32.491313 chik_dev_tools-1.2.6/cdv/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/cdv/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/cdv/util/keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/cdv/util/load_klvm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:40:32.495314 chik_dev_tools-1.2.6/chik_dev_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-05-16 05:40:32.000000 chik_dev_tools-1.2.6/chik_dev_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-16 05:40:32.000000 chik_dev_tools-1.2.6/chik_dev_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 05:40:32.000000 chik_dev_tools-1.2.6/chik_dev_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-16 05:40:32.000000 chik_dev_tools-1.2.6/chik_dev_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-16 05:40:32.000000 chik_dev_tools-1.2.6/chik_dev_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-16 05:40:32.000000 chik_dev_tools-1.2.6/chik_dev_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 05:40:32.495314 chik_dev_tools-1.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:40:32.491313 chik_dev_tools-1.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/tests/build-init-files.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:40:32.491313 chik_dev_tools-1.2.6/tests/cmds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/tests/cmds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:40:32.483313 chik_dev_tools-1.2.6/tests/cmds/object_files/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:40:32.491313 chik_dev_tools-1.2.6/tests/cmds/object_files/coinrecords/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/tests/cmds/object_files/coinrecords/coinrecord.hex
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/tests/cmds/object_files/coinrecords/coinrecord.json
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/tests/cmds/object_files/coinrecords/coinrecord_invalid.json
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/tests/cmds/object_files/coinrecords/coinrecord_metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:40:32.491313 chik_dev_tools-1.2.6/tests/cmds/object_files/coins/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/tests/cmds/object_files/coins/coin.json
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/tests/cmds/object_files/coins/coin_invalid.json
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/tests/cmds/object_files/coins/coin_metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:40:32.495314 chik_dev_tools-1.2.6/tests/cmds/object_files/spendbundles/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/tests/cmds/object_files/spendbundles/spendbundle.hex
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/tests/cmds/object_files/spendbundles/spendbundle.json
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/tests/cmds/object_files/spendbundles/spendbundle_invalid.json
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/tests/cmds/object_files/spendbundles/spendbundle_metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:40:32.495314 chik_dev_tools-1.2.6/tests/cmds/object_files/spends/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/tests/cmds/object_files/spends/spend.hex
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/tests/cmds/object_files/spends/spend.json
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/tests/cmds/object_files/spends/spend_2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/tests/cmds/object_files/spends/spend_invalid.json
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/tests/cmds/object_files/spends/spend_metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/tests/cmds/test_cdv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8407 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/tests/cmds/test_clsp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17380 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/tests/cmds/test_inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-16 05:40:06.000000 chik_dev_tools-1.2.6/tests/test_skeleton.py
```

### Comparing `chik_dev_tools-1.2.3/.github/actions/install/action.yml` & `chik_dev_tools-1.2.6/.github/actions/install/action.yml`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.3/.github/workflows/codeql-analysis.yml.bak` & `chik_dev_tools-1.2.6/.github/workflows/codeql-analysis.yml.bak`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.3/.github/workflows/precommit.yml.bak` & `chik_dev_tools-1.2.6/.github/workflows/precommit.yml.bak`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.3/.github/workflows/publish-to-pypi.yml` & `chik_dev_tools-1.2.6/.github/workflows/publish-to-pypi.yml`

 * *Files 8% similar despite different names*

```diff
@@ -9,28 +9,28 @@
   id-token: write
 
 jobs:
   build-n-publish:
     name: Build and publish Python distributions to PyPI and TestPyPI
     runs-on: ubuntu-20.04
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
       with:
         fetch-depth: 0
 
     - run: |
         git fetch origin +refs/tags/*:refs/tags/*
 
     - name: Set Job Env
       uses: Chik-Network/actions/setjobenv@main
       env:
         GH_TOKEN: ${{ secrets.GITHUB_TOKEN }}
 
     - name: Set up Python 3.8
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: "3.8"
 
     - name: Install build tools (pep517 compatible)
       run: >-
         python -m
         pip install ."[dev]"
```

### Comparing `chik_dev_tools-1.2.3/.github/workflows/run-test-suite.yml.bak` & `chik_dev_tools-1.2.6/.github/workflows/run-test-suite.yml.bak`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.3/.github/workflows/super-linter.yml.bak` & `chik_dev_tools-1.2.6/.github/workflows/super-linter.yml.bak`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.3/.github/workflows/test-blockchain-main.yml.bak` & `chik_dev_tools-1.2.6/.github/workflows/test-blockchain-main.yml.bak`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.3/.markdown-lint.yml` & `chik_dev_tools-1.2.6/.markdown-lint.yml`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.3/.pre-commit-config.yaml` & `chik_dev_tools-1.2.6/.pre-commit-config.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -24,14 +24,19 @@
         require_serial: true
         language: python
         language_version: python3
         types_or: [cython, pyi, python]
         args: ['--filter-files']
         minimum_pre_commit_version: '2.9.2'
         additional_dependencies: [isort==5.10.1]
+-   repo: https://github.com/scop/pre-commit-shfmt
+    rev: v3.8.0-1
+    hooks:
+    -   id: shfmt
+        args: ["--diff", "--write", "-i", "2"]
 -   repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.0.1
     hooks:
     -   id: check-yaml
     -   id: end-of-file-fixer
         exclude: ".*?(.hex|.klvm|.clib)"
     -   id: trailing-whitespace
```

### Comparing `chik_dev_tools-1.2.3/LICENSE` & `chik_dev_tools-1.2.6/LICENSE`

 * *Files 22% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-Apache License
-Version 2.0, January 2004
-http://www.apache.org/licenses/
-
-TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-1. Definitions.
-
-"License" shall mean the terms and conditions for use, reproduction,
-and distribution as defined by Sections 1 through 9 of this document.
-
-"Licensor" shall mean the copyright owner or entity authorized by
-the copyright owner that is granting the License.
-
-"Legal Entity" shall mean the union of the acting entity and all
-other entities that control, are controlled by, or are under common
-control with that entity. For the purposes of this definition,
-"control" means (i) the power, direct or indirect, to cause the
-direction or management of such entity, whether by contract or
-otherwise, or (ii) ownership of fifty percent (50%) or more of the
-outstanding shares, or (iii) beneficial ownership of such entity.
-
-"You" (or "Your") shall mean an individual or Legal Entity
-exercising permissions granted by this License.
-
-"Source" form shall mean the preferred form for making modifications,
-including but not limited to software source code, documentation
-source, and configuration files.
-
-"Object" form shall mean any form resulting from mechanical
-transformation or translation of a Source form, including but
-not limited to compiled object code, generated documentation,
-and conversions to other media types.
-
-"Work" shall mean the work of authorship, whether in Source or
-Object form, made available under the License, as indicated by a
-copyright notice that is included in or attached to the work
-(an example is provided in the Appendix below).
-
-"Derivative Works" shall mean any work, whether in Source or Object
-form, that is based on (or derived from) the Work and for which the
-editorial revisions, annotations, elaborations, or other modifications
-represent, as a whole, an original work of authorship. For the purposes
-of this License, Derivative Works shall not include works that remain
-separable from, or merely link (or bind by name) to the interfaces of,
-the Work and Derivative Works thereof.
-
-"Contribution" shall mean any work of authorship, including
-the original version of the Work and any modifications or additions
-to that Work or Derivative Works thereof, that is intentionally
-submitted to Licensor for inclusion in the Work by the copyright owner
-or by an individual or Legal Entity authorized to submit on behalf of
-the copyright owner. For the purposes of this definition, "submitted"
-means any form of electronic, verbal, or written communication sent
-to the Licensor or its representatives, including but not limited to
-communication on electronic mailing lists, source code control systems,
-and issue tracking systems that are managed by, or on behalf of, the
-Licensor for the purpose of discussing and improving the Work, but
-excluding communication that is conspicuously marked or otherwise
-designated in writing by the copyright owner as "Not a Contribution."
-
-"Contributor" shall mean Licensor and any individual or Legal Entity
-on behalf of whom a Contribution has been received by Licensor and
-subsequently incorporated within the Work.
-
-2. Grant of Copyright License. Subject to the terms and conditions of
-this License, each Contributor hereby grants to You a perpetual,
-worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-copyright license to reproduce, prepare Derivative Works of,
-publicly display, publicly perform, sublicense, and distribute the
-Work and such Derivative Works in Source or Object form.
-
-3. Grant of Patent License. Subject to the terms and conditions of
-this License, each Contributor hereby grants to You a perpetual,
-worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-(except as stated in this section) patent license to make, have made,
-use, offer to sell, sell, import, and otherwise transfer the Work,
-where such license applies only to those patent claims licensable
-by such Contributor that are necessarily infringed by their
-Contribution(s) alone or by combination of their Contribution(s)
-with the Work to which such Contribution(s) was submitted. If You
-institute patent litigation against any entity (including a
-cross-claim or counterclaim in a lawsuit) alleging that the Work
-or a Contribution incorporated within the Work constitutes direct
-or contributory patent infringement, then any patent licenses
-granted to You under this License for that Work shall terminate
-as of the date such litigation is filed.
-
-4. Redistribution. You may reproduce and distribute copies of the
-Work or Derivative Works thereof in any medium, with or without
-modifications, and in Source or Object form, provided that You
-meet the following conditions:
-
-(a) You must give any other recipients of the Work or
-Derivative Works a copy of this License; and
-
-(b) You must cause any modified files to carry prominent notices
-stating that You changed the files; and
-
-(c) You must retain, in the Source form of any Derivative Works
-that You distribute, all copyright, patent, trademark, and
-attribution notices from the Source form of the Work,
-excluding those notices that do not pertain to any part of
-the Derivative Works; and
-
-(d) If the Work includes a "NOTICE" text file as part of its
-distribution, then any Derivative Works that You distribute must
-include a readable copy of the attribution notices contained
-within such NOTICE file, excluding those notices that do not
-pertain to any part of the Derivative Works, in at least one
-of the following places: within a NOTICE text file distributed
-as part of the Derivative Works; within the Source form or
-documentation, if provided along with the Derivative Works; or,
-within a display generated by the Derivative Works, if and
-wherever such third-party notices normally appear. The contents
-of the NOTICE file are for informational purposes only and
-do not modify the License. You may add Your own attribution
-notices within Derivative Works that You distribute, alongside
-or as an addendum to the NOTICE text from the Work, provided
-that such additional attribution notices cannot be construed
-as modifying the License.
-
-You may add Your own copyright statement to Your modifications and
-may provide additional or different license terms and conditions
-for use, reproduction, or distribution of Your modifications, or
-for any such Derivative Works as a whole, provided Your use,
-reproduction, and distribution of the Work otherwise complies with
-the conditions stated in this License.
-
-5. Submission of Contributions. Unless You explicitly state otherwise,
-any Contribution intentionally submitted for inclusion in the Work
-by You to the Licensor shall be under the terms and conditions of
-this License, without any additional terms or conditions.
-Notwithstanding the above, nothing herein shall supersede or modify
-the terms of any separate license agreement you may have executed
-with Licensor regarding such Contributions.
-
-6. Trademarks. This License does not grant permission to use the trade
-names, trademarks, service marks, or product names of the Licensor,
-except as required for reasonable and customary use in describing the
-origin of the Work and reproducing the content of the NOTICE file.
-
-7. Disclaimer of Warranty. Unless required by applicable law or
-agreed to in writing, Licensor provides the Work (and each
-Contributor provides its Contributions) on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-implied, including, without limitation, any warranties or conditions
-of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-PARTICULAR PURPOSE. You are solely responsible for determining the
-appropriateness of using or redistributing the Work and assume any
-risks associated with Your exercise of permissions under this License.
-
-8. Limitation of Liability. In no event and under no legal theory,
-whether in tort (including negligence), contract, or otherwise,
-unless required by applicable law (such as deliberate and grossly
-negligent acts) or agreed to in writing, shall any Contributor be
-liable to You for damages, including any direct, indirect, special,
-incidental, or consequential damages of any character arising as a
-result of this License or out of the use or inability to use the
-Work (including but not limited to damages for loss of goodwill,
-work stoppage, computer failure or malfunction, or any and all
-other commercial damages or losses), even if such Contributor
-has been advised of the possibility of such damages.
-
-9. Accepting Warranty or Additional Liability. While redistributing
-the Work or Derivative Works thereof, You may choose to offer,
-and charge a fee for, acceptance of support, warranty, indemnity,
-or other liability obligations and/or rights consistent with this
-License. However, in accepting such obligations, You may act only
-on Your own behalf and on Your sole responsibility, not on behalf
-of any other Contributor, and only if You agree to indemnify,
-defend, and hold each Contributor harmless for any liability
-incurred by, or claims asserted against, such Contributor by reason
-of your accepting any such warranty or additional liability.
-
-END OF TERMS AND CONDITIONS
-
-APPENDIX: How to apply the Apache License to your work.
-
-To apply the Apache License to your work, attach the following
-boilerplate notice, with the fields enclosed by brackets "[]"
-replaced with your own identifying information. (Don't include
-the brackets!)  The text should be enclosed in the appropriate
-comment syntax for the file format. We also recommend that a
-file or class name and description of purpose be included on the
-same "printed page" as the copyright notice for easier
-identification within third-party archives.
-
-Copyright 2023 Chik Network
-
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright 2024 Chik Network Inc.
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `chik_dev_tools-1.2.3/PKG-INFO` & `chik_dev_tools-1.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chik_dev_tools
-Version: 1.2.3
+Version: 1.2.6
 Summary: Chik development commands
 Home-page: https://github.com/Chik-Network
 Author: Quexington
 Author-email: m.hauff@chiknetwork.com
 License: https://opensource.org/licenses/Apache-2.0
 Project-URL: Bug Reports, https://github.com/Chik-Network/chik-dev-tools
 Project-URL: Source, https://github.com/Chik-Network/chik-dev-tools
@@ -16,20 +16,20 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: packaging
 Requires-Dist: pytest
 Requires-Dist: pytest-asyncio
 Requires-Dist: pytimeparse
 Requires-Dist: anyio
-Requires-Dist: chik-blockchain==2.1.1
+Requires-Dist: chik-blockchain==2.3.0
 Provides-Extra: dev
 Requires-Dist: anyio; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
-Requires-Dist: black==23.7.0; extra == "dev"
+Requires-Dist: black==24.4.2; extra == "dev"
 Requires-Dist: types-aiofiles; extra == "dev"
 Requires-Dist: types-click; extra == "dev"
 Requires-Dist: types-cryptography; extra == "dev"
 Requires-Dist: types-pkg_resources; extra == "dev"
 Requires-Dist: types-pyyaml; extra == "dev"
 Requires-Dist: types-setuptools; extra == "dev"
 Requires-Dist: isort; extra == "dev"
```

### Comparing `chik_dev_tools-1.2.3/README.md` & `chik_dev_tools-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.3/activated.py` & `chik_dev_tools-1.2.6/activated.py`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.3/cdv/clibs/condition_codes.clib` & `chik_dev_tools-1.2.6/cdv/clibs/condition_codes.clib`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.3/cdv/clibs/curry_and_treehash.clib` & `chik_dev_tools-1.2.6/cdv/clibs/curry_and_treehash.clib`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.3/cdv/clibs/singleton_truths.clib` & `chik_dev_tools-1.2.6/cdv/clibs/singleton_truths.clib`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.3/cdv/cmds/chik_inspect.py` & `chik_dev_tools-1.2.6/cdv/cmds/chik_inspect.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,38 +3,38 @@
 import json
 import sys
 from pprint import pprint
 from secrets import token_bytes
 from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, Union
 
 import click
-from blspy import AugSchemeMPL, G1Element, G2Element, PrivateKey
 from chik.consensus.cost_calculator import NPCResult
 from chik.consensus.default_constants import DEFAULT_CONSTANTS
 from chik.full_node.bundle_tools import simple_solution_generator
 from chik.full_node.mempool_check_conditions import get_name_puzzle_conditions
 from chik.types.blockchain_format.coin import Coin
 from chik.types.blockchain_format.program import INFINITE_COST, Program
 from chik.types.blockchain_format.sized_bytes import bytes32
 from chik.types.coin_record import CoinRecord
-from chik.types.coin_spend import CoinSpend
+from chik.types.coin_spend import CoinSpend, make_spend
 from chik.types.generator_types import BlockGenerator
 from chik.types.spend_bundle import SpendBundle
 from chik.util.byte_types import hexstr_to_bytes
 from chik.util.condition_tools import conditions_dict_for_solution, pkm_pairs_for_conditions_dict
 from chik.util.config import load_config
 from chik.util.default_root import DEFAULT_ROOT_PATH
 from chik.util.ints import uint32, uint64
 from chik.util.keychain import bytes_to_mnemonic, mnemonic_to_seed
 from chik.wallet.derive_keys import _derive_path
 from chik.wallet.puzzles.p2_delegated_puzzle_or_hidden_puzzle import (
     DEFAULT_HIDDEN_PUZZLE_HASH,
     calculate_synthetic_public_key,
     calculate_synthetic_secret_key,
 )
+from chik_rs import AugSchemeMPL, G1Element, G2Element, PrivateKey
 
 from cdv.cmds.util import parse_program
 
 """
 This group of commands is for guessing the types of objects when you don't know what they are,
 but also for building them from scratch and for modifying them once you have them completely loaded/built.
 """
@@ -157,28 +157,30 @@
 
         input_objects.append(in_obj)
 
     for obj in input_objects:
         if type(obj) == str:
             print(f"Could not guess the type of {obj}")
         elif type(obj) == Coin:  # type: ignore[comparison-overlap]
+            assert isinstance(obj, Coin)  # mypy otherwise complains that obj is a str
             do_inspect_coin_cmd(ctx, [obj])
         elif type(obj) == CoinSpend:  # type: ignore[comparison-overlap]
+            assert isinstance(obj, CoinSpend)
             do_inspect_coin_spend_cmd(ctx, [obj])
         elif type(obj) == SpendBundle:  # type: ignore[comparison-overlap]
             do_inspect_spend_bundle_cmd(ctx, [obj])
         elif type(obj) == CoinRecord:  # type: ignore[comparison-overlap]
             do_inspect_coin_record_cmd(ctx, [obj])
         elif type(obj) == Program:
             do_inspect_program_cmd(ctx, [obj])
-        elif type(obj) == G1Element:
+        elif type(obj) == G1Element:  # type: ignore[comparison-overlap]
             do_inspect_keys_cmd(ctx, public_key=obj)
-        elif type(obj) == PrivateKey:
+        elif type(obj) == PrivateKey:  # type: ignore[comparison-overlap]
             do_inspect_keys_cmd(ctx, secret_key=obj)
-        elif type(obj) == G2Element:
+        elif type(obj) == G2Element:  # type: ignore[comparison-overlap]
             print("That's a BLS aggregated signature")  # This is more helpful than just printing it back to them
 
 
 """
 Most of the following commands are designed to also be available as importable functions and usable by the "any" cmd.
 This is why there's the cmd/do_cmd pattern in all of them.
 The objects they are inspecting can be a list of strings (from the cmd line), or a list of the object being inspected.
@@ -267,28 +269,28 @@
         del kwargs["cost"]
         del kwargs["ignore_byte_cost"]
     # If this is being built from the command line and the two required args are there
     if kwargs and all([kwargs["puzzle_reveal"], kwargs["solution"]]):
         # If they specified the coin components
         if (not kwargs["coin"]) and all([kwargs["parent_id"], kwargs["puzzle_hash"], kwargs["amount"]]):
             coin_spend_objs: List[CoinSpend] = [
-                CoinSpend(
+                make_spend(
                     Coin(
                         bytes32.from_hexstr(kwargs["parent_id"]),
                         bytes32.from_hexstr(kwargs["puzzle_hash"]),
                         uint64(kwargs["amount"]),
                     ),
                     parse_program(kwargs["puzzle_reveal"]),
                     parse_program(kwargs["solution"]),
                 )
             ]
         # If they specifed a coin object to parse
         elif kwargs["coin"]:
             coin_spend_objs = [
-                CoinSpend(
+                make_spend(
                     do_inspect_coin_cmd(ctx, [kwargs["coin"]], print_results=False)[0],
                     parse_program(kwargs["puzzle_reveal"]),
                     parse_program(kwargs["solution"]),
                 )
             ]
         else:
             print("Invalid arguments specified.")
@@ -316,15 +318,15 @@
                 npc_result: NPCResult = get_name_puzzle_conditions(
                     program,
                     INFINITE_COST,
                     height=DEFAULT_CONSTANTS.SOFT_FORK2_HEIGHT,  # so that all opcodes are available
                     mempool_mode=True,
                     constants=DEFAULT_CONSTANTS,
                 )
-                cost: int = npc_result.cost
+                cost = int(0 if npc_result.conds is None else npc_result.conds.cost)
                 if ignore_byte_cost:
                     cost -= len(bytes(coin_spend.puzzle_reveal)) * DEFAULT_CONSTANTS.COST_PER_BYTE
                 print(f"Cost: {cost}")
 
     return coin_spend_objs
 
 
@@ -370,15 +372,17 @@
     bundles: Union[Tuple[str], List[SpendBundle]],
     print_results: bool = True,
     **kwargs,
 ) -> List[SpendBundle]:
     # If this is from the command line and they've specified at lease one spend to parse
     if kwargs and (len(kwargs["spend"]) > 0):
         if len(kwargs["aggsig"]) > 0:
-            sig: G2Element = AugSchemeMPL.aggregate([G2Element(hexstr_to_bytes(sig)) for sig in kwargs["aggsig"]])
+            sig: G2Element = AugSchemeMPL.aggregate(
+                [G2Element.from_bytes(hexstr_to_bytes(sig)) for sig in kwargs["aggsig"]]
+            )
         else:
             sig = G2Element()
         spend_bundle_objs: List[SpendBundle] = [
             SpendBundle(
                 do_inspect_coin_spend_cmd(ctx, kwargs["spend"], print_results=False),
                 sig,
             )
@@ -405,15 +409,15 @@
                     npc_result: NPCResult = get_name_puzzle_conditions(
                         program,
                         INFINITE_COST,
                         height=DEFAULT_CONSTANTS.SOFT_FORK2_HEIGHT,  # so that all opcodes are available
                         mempool_mode=True,
                         constants=DEFAULT_CONSTANTS,
                     )
-                    cost: int = npc_result.cost
+                    cost = int(0 if npc_result.conds is None else npc_result.conds.cost)
                     if kwargs["ignore_byte_cost"]:
                         for coin_spend in spend_bundle.coin_spends:
                             cost -= len(bytes(coin_spend.puzzle_reveal)) * DEFAULT_CONSTANTS.COST_PER_BYTE
                     print(f"Cost: {cost}")
             if kwargs["debug"]:
                 print("")
                 print("Debugging Information")
@@ -428,15 +432,15 @@
                 print("")
                 print("Public Key/Message Pairs")
                 print("------------------------")
                 pkm_dict: Dict[str, List[bytes]] = {}
                 for obj in spend_bundle_objs:
                     for coin_spend in obj.coin_spends:
                         conditions_dict = conditions_dict_for_solution(
-                            coin_spend.puzzle_reveal, coin_spend.solution, INFINITE_COST
+                            coin_spend.puzzle_reveal.to_program(), coin_spend.solution.to_program(), INFINITE_COST
                         )
                         if conditions_dict is None:
                             print(f"Generating conditions failed, con:{conditions_dict}")
                         else:
                             config = load_config(DEFAULT_ROOT_PATH, "config.yaml")
                             genesis_challenge = config["network_overrides"]["constants"][kwargs["network"]][
                                 "GENESIS_CHALLENGE"
@@ -622,14 +626,15 @@
     sk: Optional[PrivateKey] = None
     pk: G1Element = G1Element()
     path: str = "m"
     # If we're receiving this from the any command
     if len(kwargs) == 1:
         if "secret_key" in kwargs:
             sk = kwargs["secret_key"]
+            assert sk is not None
             pk = sk.get_g1()
         elif "public_key" in kwargs:
             pk = kwargs["public_key"]
     else:
         condition_list = [
             kwargs["public_key"],
             kwargs["secret_key"],
@@ -672,14 +677,15 @@
                 if case == "backup":
                     list_path = [12381, 8444, 4, 0]
                 if case == "owner":
                     list_path = [12381, 8444, 5, 0]
                 if case == "auth":
                     list_path = [12381, 8444, 6, 0]
             if list_path:
+                assert sk is not None
                 sk = _derive_path(sk, list_path)
                 pk = sk.get_g1()
                 path = "m/" + "/".join([str(e) for e in path])
 
             if kwargs["synthetic"]:
                 if sk:
                     sk = calculate_synthetic_secret_key(sk, bytes32.from_hexstr((kwargs["hidden_puzhash"])))
```

### Comparing `chik_dev_tools-1.2.3/cdv/cmds/cli.py` & `chik_dev_tools-1.2.6/cdv/cmds/cli.py`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.3/cdv/cmds/clsp.py` & `chik_dev_tools-1.2.6/cdv/cmds/clsp.py`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.3/cdv/cmds/rpc.py` & `chik_dev_tools-1.2.6/cdv/cmds/rpc.py`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.3/cdv/cmds/util.py` & `chik_dev_tools-1.2.6/cdv/cmds/util.py`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.3/cdv/examples/clsp/piggybank.clsp` & `chik_dev_tools-1.2.6/cdv/examples/clsp/piggybank.clsp`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.3/cdv/examples/drivers/piggybank_drivers.py` & `chik_dev_tools-1.2.6/cdv/examples/drivers/piggybank_drivers.py`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.3/cdv/examples/tests/test_piggybank.py` & `chik_dev_tools-1.2.6/cdv/examples/tests/test_piggybank.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 from cdv.test import CoinWrapper
 from cdv.test import setup as setup_test
 
 
 class TestStandardTransaction:
     @pytest_asyncio.fixture(scope="function")
     async def setup(self):
-        network, alice, bob = await setup_test()
-        await network.farm_block()
-        yield network, alice, bob
+        async with setup_test() as (network, alice, bob):
+            await network.farm_block()
+            yield network, alice, bob
 
     async def make_and_spend_piggybank(self, network, alice, bob, CONTRIBUTION_AMOUNT) -> Dict[str, List[Coin]]:
         # Get our alice wallet some money
         await network.farm_block(farmer=alice)
 
         # This will use one mojo to create our piggybank on the blockchain.
         piggybank_coin: Optional[CoinWrapper] = await alice.launch_smart_coin(
@@ -83,15 +83,15 @@
                         addition.puzzle_hash == create_piggybank_puzzle(1000000000000, bob.puzzle_hash).get_tree_hash()
                     ),
                     result["additions"],
                 )
             )
             assert len(filtered_result) == 1
         finally:
-            await network.close()
+            pass
 
     @pytest.mark.asyncio
     async def test_piggybank_completion(self, setup):
         network, alice, bob = setup
         try:
             result: Dict[str, List[Coin]] = await self.make_and_spend_piggybank(network, alice, bob, 1000000000000)
 
@@ -114,20 +114,20 @@
                 filter(
                     lambda addition: (addition.amount == 1000000000001) and (addition.puzzle_hash == bob.puzzle_hash),
                     result["additions"],
                 )
             )
             assert len(filtered_result) == 1
         finally:
-            await network.close()
+            pass
 
     @pytest.mark.asyncio
     async def test_piggybank_stealing(self, setup):
         network, alice, bob = setup
         try:
             result: Dict[str, List[Coin]] = await self.make_and_spend_piggybank(network, alice, bob, -100)
             assert "error" in result
             assert (
                 "GENERATOR_RUNTIME_ERROR" in result["error"]
             )  # This fails during puzzle execution, not in driver code
         finally:
-            await network.close()
+            pass
```

### Comparing `chik_dev_tools-1.2.3/cdv/test/__init__.py` & `chik_dev_tools-1.2.6/cdv/test/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 from __future__ import annotations
 
 import binascii
+import contextlib
 import datetime
 import struct
-from typing import Dict, List, Optional, Tuple, Union
+from contextlib import asynccontextmanager
+from typing import AsyncIterator, Dict, List, Optional, Tuple, Type, TypeVar, Union
 
 import pytimeparse
-from blspy import AugSchemeMPL, G1Element, G2Element, PrivateKey
 from chik.klvm.spend_sim import SimClient, SpendSim
 from chik.consensus.default_constants import DEFAULT_CONSTANTS
 from chik.types.blockchain_format.coin import Coin
 from chik.types.blockchain_format.program import Program
 from chik.types.blockchain_format.sized_bytes import bytes32
 from chik.types.coin_record import CoinRecord
-from chik.types.coin_spend import CoinSpend
+from chik.types.coin_spend import CoinSpend, make_spend
 from chik.types.spend_bundle import SpendBundle
 from chik.util.condition_tools import ConditionOpcode
 from chik.util.hash import std_hash
 from chik.util.ints import uint32, uint64
 from chik.wallet.derive_keys import master_sk_to_wallet_sk
 from chik.wallet.puzzles.p2_delegated_puzzle_or_hidden_puzzle import (  # standard_transaction
     DEFAULT_HIDDEN_PUZZLE_HASH,
     calculate_synthetic_secret_key,
     puzzle_for_pk,
 )
 from chik.wallet.sign_coin_spends import sign_coin_spends
+from chik_rs import AugSchemeMPL, G1Element, G2Element, PrivateKey
 
 from cdv.util.keys import private_key_for_index, public_key_for_index
 
 duration_div = 86400.0
 block_time = (600.0 / 32.0) / duration_div
 # Allowed subdivisions of 1 coin
 
@@ -449,21 +451,15 @@
                 delegated_puzzle_solution.get_tree_hash()
                 + found_coin.name()
                 + DEFAULT_CONSTANTS.AGG_SIG_ME_ADDITIONAL_DATA
             ),
         )
 
         spend_bundle = SpendBundle(
-            [
-                CoinSpend(
-                    found_coin.coin,  # Coin to spend
-                    self.puzzle,  # Puzzle used for found_coin
-                    solution,  # The solution to the puzzle locking found_coin
-                )
-            ],
+            [make_spend(found_coin.coin, self.puzzle, solution)],
             signature,
         )
         pushed: Dict[str, Union[str, List[Coin]]] = await self.parent.push_tx(spend_bundle)
         if "error" not in pushed:
             return cw.custom_coin(found_coin.coin, amt)
         else:
             return None
@@ -529,19 +525,15 @@
             delegated_puzzle_solution = Program.to((1, solution_list))
             # Solution is the solution for the old coin.
             solution = Program.to([[], delegated_puzzle_solution, []])
         else:
             delegated_puzzle_solution = Program.to(kwargs["args"])
             solution = delegated_puzzle_solution
 
-        solution_for_coin = CoinSpend(
-            coin.coin,
-            coin.puzzle(),
-            solution,
-        )
+        solution_for_coin = make_spend(coin.coin, coin.puzzle(), solution)
 
         # The reason this use of sign_coin_spends exists is that it correctly handles
         # the signing for non-standard coins.  I don't fully understand the difference but
         # this definitely does the right thing.
         try:
             spend_bundle: SpendBundle = await sign_coin_spends(
                 [solution_for_coin],
@@ -560,38 +552,40 @@
         if pushtx:
             pushed: Dict[str, Union[str, List[Coin]]] = await self.parent.push_tx(spend_bundle)
             return SpendResult(pushed)
         else:
             return spend_bundle
 
 
+_T_Network = TypeVar("_T_Network", bound="Network")
+
+
 # A user oriented (domain specific) view of the chik network.
 class Network:
     """An object that owns a simulation, responsible for managing Wallet actors,
     time and initialization."""
 
     time: datetime.timedelta
     sim: SpendSim
     sim_client: SimClient
     wallets: Dict[str, Wallet]
     nobody: Wallet
 
     @classmethod
-    async def create(cls) -> "Network":
+    @contextlib.asynccontextmanager
+    async def managed(cls: Type[_T_Network]) -> AsyncIterator[_T_Network]:
         self = cls()
         self.time = datetime.timedelta(days=18750, seconds=61201)  # Past the initial transaction freeze
-        self.sim = await SpendSim.create()
-        self.sim_client = SimClient(self.sim)
-        self.wallets = {}
-        self.nobody = self.make_wallet("nobody")
-        self.wallets[str(self.nobody.pk())] = self.nobody
-        return self
-
-    async def close(self):
-        await self.sim.close()
+        async with SpendSim.managed() as sim:
+            self.sim = sim
+            self.sim_client = SimClient(self.sim)
+            self.wallets = {}
+            self.nobody = self.make_wallet("nobody")
+            self.wallets[str(self.nobody.pk())] = self.nobody
+            yield self
 
     # Have the system farm one block with a specific beneficiary (nobody if not specified).
     async def farm_block(self, **kwargs) -> Tuple[List[Coin], List[Coin]]:
         """Given a farmer, farm a block with that actor as the beneficiary of the farm
         reward.
 
         Used for causing chik balance to exist so the system can do things.
@@ -712,12 +706,13 @@
         additions, removals = await self.farm_block()
         return {
             "additions": additions,
             "removals": removals,
         }
 
 
-async def setup() -> Tuple[Network, Wallet, Wallet]:
-    network: Network = await Network.create()
-    alice: Wallet = network.make_wallet("alice")
-    bob: Wallet = network.make_wallet("bob")
-    return network, alice, bob
+@asynccontextmanager
+async def setup() -> AsyncIterator[Tuple[Network, Wallet, Wallet]]:
+    async with Network.managed() as network:
+        alice = network.make_wallet("alice")
+        bob = network.make_wallet("bob")
+        yield network, alice, bob
```

### Comparing `chik_dev_tools-1.2.3/cdv/test/test_skeleton.py` & `chik_dev_tools-1.2.6/cdv/test/test_skeleton.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 
 from cdv.test import setup as setup_test
 
 
 class TestSomething:
     @pytest_asyncio.fixture(scope="function")
     async def setup(self):
-        network, alice, bob = await setup_test()
-        await network.farm_block()
-        yield network, alice, bob
+        async with setup_test() as (network, alice, bob):
+            await network.farm_block()
+            yield network, alice, bob
 
     @pytest.mark.asyncio
     async def test_something(self, setup):
         network, alice, bob = setup
         try:
             pass
         finally:
-            await network.close()
+            pass
```

### Comparing `chik_dev_tools-1.2.3/cdv/util/keys.py` & `chik_dev_tools-1.2.6/cdv/util/keys.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 from typing import Dict, List
 
-from blspy import AugSchemeMPL, BasicSchemeMPL, G1Element, G2Element, PrivateKey
 from chik.util.hash import std_hash
+from chik_rs import AugSchemeMPL, G1Element, G2Element, PrivateKey
 
 
 def secret_exponent_for_index(index: int) -> int:
     blob = index.to_bytes(32, "big")
-    hashed_blob = BasicSchemeMPL.key_gen(std_hash(b"foo" + blob))
+    hashed_blob = AugSchemeMPL.key_gen(std_hash(b"foo" + blob))
     r = int.from_bytes(hashed_blob, "big")
     return r
 
 
 def private_key_for_index(index: int) -> PrivateKey:
     r = secret_exponent_for_index(index)
     return PrivateKey.from_bytes(r.to_bytes(32, "big"))
```

### Comparing `chik_dev_tools-1.2.3/cdv/util/load_klvm.py` & `chik_dev_tools-1.2.6/cdv/util/load_klvm.py`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.3/chik_dev_tools.egg-info/PKG-INFO` & `chik_dev_tools-1.2.6/chik_dev_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: chik-dev-tools
-Version: 1.2.3
+Name: chik_dev_tools
+Version: 1.2.6
 Summary: Chik development commands
 Home-page: https://github.com/Chik-Network
 Author: Quexington
 Author-email: m.hauff@chiknetwork.com
 License: https://opensource.org/licenses/Apache-2.0
 Project-URL: Bug Reports, https://github.com/Chik-Network/chik-dev-tools
 Project-URL: Source, https://github.com/Chik-Network/chik-dev-tools
@@ -16,20 +16,20 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: packaging
 Requires-Dist: pytest
 Requires-Dist: pytest-asyncio
 Requires-Dist: pytimeparse
 Requires-Dist: anyio
-Requires-Dist: chik-blockchain==2.1.1
+Requires-Dist: chik-blockchain==2.3.0
 Provides-Extra: dev
 Requires-Dist: anyio; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
-Requires-Dist: black==23.7.0; extra == "dev"
+Requires-Dist: black==24.4.2; extra == "dev"
 Requires-Dist: types-aiofiles; extra == "dev"
 Requires-Dist: types-click; extra == "dev"
 Requires-Dist: types-cryptography; extra == "dev"
 Requires-Dist: types-pkg_resources; extra == "dev"
 Requires-Dist: types-pyyaml; extra == "dev"
 Requires-Dist: types-setuptools; extra == "dev"
 Requires-Dist: isort; extra == "dev"
```

### Comparing `chik_dev_tools-1.2.3/chik_dev_tools.egg-info/SOURCES.txt` & `chik_dev_tools-1.2.6/chik_dev_tools.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 .flake8
 .gitignore
 .isort.cfg
 .markdown-lint.yml
 .pre-commit-config.yaml
+.repo-content-updater.yml
 LICENSE
 README.md
 activated.ps1
 activated.py
 activated.sh
 mypy.ini
 pyproject.toml
```

### Comparing `chik_dev_tools-1.2.3/mypy.ini` & `chik_dev_tools-1.2.6/mypy.ini`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.3/pyproject.toml` & `chik_dev_tools-1.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.3/setup.py` & `chik_dev_tools-1.2.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 
 dependencies = [
     "packaging",
     "pytest",
     "pytest-asyncio",
     "pytimeparse",
     "anyio",
-    "chik-blockchain==2.1.1",
+    "chik-blockchain==2.3.0",
 ]
 
 dev_dependencies = [
     "anyio",
     "flake8",
     "mypy",
-    "black==23.7.0",
+    "black==24.4.2",
     "types-aiofiles",
     "types-click",
     "types-cryptography",
     "types-pkg_resources",
     "types-pyyaml",
     "types-setuptools",
     "isort",
```

### Comparing `chik_dev_tools-1.2.3/tests/build-init-files.py` & `chik_dev_tools-1.2.6/tests/build-init-files.py`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.3/tests/cmds/object_files/spendbundles/spendbundle.json` & `chik_dev_tools-1.2.6/tests/cmds/object_files/spendbundles/spendbundle.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666667%*

 * *Differences: {"'spend_bundle'": "{'coin_spends': {0: {'solution': '0x80'}}}"}*

```diff
@@ -5,12 +5,12 @@
             {
                 "coin": {
                     "amount": 0,
                     "parent_coin_info": "0x0000000000000000000000000000000000000000000000000000000000000000",
                     "puzzle_hash": "0x0000000000000000000000000000000000000000000000000000000000000000"
                 },
                 "puzzle_reveal": "0x01",
-                "solution": "80"
+                "solution": "0x80"
             }
         ]
     }
 }
```

### Comparing `chik_dev_tools-1.2.3/tests/cmds/object_files/spendbundles/spendbundle_invalid.json` & `chik_dev_tools-1.2.6/tests/cmds/object_files/spendbundles/spendbundle_invalid.json`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.3/tests/cmds/test_cdv.py` & `chik_dev_tools-1.2.6/tests/cmds/test_cdv.py`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.3/tests/cmds/test_clsp.py` & `chik_dev_tools-1.2.6/tests/cmds/test_clsp.py`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.3/tests/cmds/test_inspect.py` & `chik_dev_tools-1.2.6/tests/cmds/test_inspect.py`

 * *Files 4% similar despite different names*

```diff
@@ -183,20 +183,26 @@
         assert id in result.output
         assert modified_cost in result.output
 
     def test_spendbundles(self):
         spend_path = Path(__file__).parent.joinpath("object_files/spends/spend.json")
         spend_path_2 = Path(__file__).parent.joinpath("object_files/spends/spend_2.json")
         pubkey: str = "80df54b2a616f5c79baaed254134ae5dfc6e24e2d8e1165b251601ceb67b1886db50aacf946eb20f00adc303e7534dd0"
-        signable_data: str = "24f5a5fd42d16a20302798ef6ed309979b43003d2320d9f0e8ea9831a92759fb4bccd5bb71183532bff220ba46c268991a3ff07eb358e8255a65c30a2dce0e5fbb"  # noqa
-        agg_sig: str = "b83fe374efbc5776735df7cbfb7e27ede5079b41cd282091450e4de21c4b772e254ce906508834b0c2dcd3d58c47a96914c782f0baf8eaff7ece3b070d2035cd878f744deadcd6c6625c1d0a1b418437ee3f25c2df08ffe08bdfe06b8a83b514"  # noqa
+        signable_data: str = (
+            "24f5a5fd42d16a20302798ef6ed309979b43003d2320d9f0e8ea9831a92759fb4bccd5bb71183532bff220ba46c268991a3ff07eb358e8255a65c30a2dce0e5fbb"  # noqa
+        )
+        agg_sig: str = (
+            "b83fe374efbc5776735df7cbfb7e27ede5079b41cd282091450e4de21c4b772e254ce906508834b0c2dcd3d58c47a96914c782f0baf8eaff7ece3b070d2035cd878f744deadcd6c6625c1d0a1b418437ee3f25c2df08ffe08bdfe06b8a83b514"  # noqa
+        )
         id_no_sig: str = "3fc441c1048a4e0b9fd1648d7647fdebd220cf7dd51b6967dcaf76f7043e83d6"
         id_with_sig: str = "7d6f0da915deed117ad5589aa8bd6bf99beb69f48724b14b2134f6f8af6d8afc"
         network_modifier: str = "testnet7"
-        modified_signable_data: str = "24f5a5fd42d16a20302798ef6ed309979b43003d2320d9f0e8ea9831a92759fb4b117816bf8f01cfea414140de5dae2223b00361a396177a9cb410ff61f20015af"  # noqa
+        modified_signable_data: str = (
+            "24f5a5fd42d16a20302798ef6ed309979b43003d2320d9f0e8ea9831a92759fb4b117816bf8f01cfea414140de5dae2223b00361a396177a9cb410ff61f20015af"  # noqa
+        )
         cost: str = "6692283"
         modified_cost: str = "6668283"
 
         runner = CliRunner()
 
         # Build with only the spends
         result: Result = runner.invoke(
@@ -343,23 +349,25 @@
         runner = CliRunner()
 
         result: Result = runner.invoke(cli, ["inspect", "--id", "programs", program])
         assert result.exit_code == 0
         assert id in result.output
 
     def test_keys(self):
-        mnemonic: str = "chik chik chik chik chik chik chik chik chik chik chik chik chik chik chik chik chik chik chik chik chik chik chik chik"  # noqa
-        sk: str = "6e66bc91c04127f1178cb725faf82b55214b5f215b10bd53bf2eb1ee9e76d2cc"
-        pk: str = "8777e5c4f5b21840eb69d9cc09433655b044a8e80048cd9583bab9a90f4774d2d57c1b19196ae132c9502db5902f3e5d"
+        mnemonic: str = (
+            "spend spend spend spend spend spend spend spend spend spend spend spend spend spend spend spend spend spend spend spend spend spend spend spend"  # noqa
+        )
+        sk: str = "1ef0ff42df2fdd4472312e033f555c569d18b85ba0d9f1b09ed87b254dc18a8e"
+        pk: str = "ae6c7589432cb60a00d84fc83971f50a98fd728863d3ceb189300f2f80d6839e9a2e761ef6cdce809caee83a4e73b623"
         hd_modifier: str = "m/12381/8444/0/0"
         type_modifier: str = "farmer"  # Should be same as above HD Path
-        farmer_sk: str = "1d4a4c2f2059ac889fe066d1116a0fe5dc3d6aa016645306698968c78e8df916"
-        synthetic_sk: str = "6963ce75cd541a0b49cc6feb15185675beb513bd5808e744d475ec50cf75b2c0"
+        farmer_sk: str = "6a97995a8b35c69418ad60152a5e1c9a32d159bcb7c343c5ccf83c71e4df2038"
+        synthetic_sk: str = "4272b71ba1c628948e308148e92c1a9b24a785d52f604610a436d2088f72d578"
         ph_modifier: str = "69ae360134b1fae04326e5546f25dc794a19192a1f22a44a46d038e7f0d1ecbb"
-        modified_synthetic_sk: str = "2dc18bb076849fce06d9c36e59821ff43e8b81068d33fcc5ada3568fb9dcdb7f"
+        modified_synthetic_sk: str = "405d969856846304eec6b243d810665cb3b7e94b56747b87e8e5597948ba1da6"
 
         runner = CliRunner()
 
         # Build the key from secret key
         result: Result = runner.invoke(cli, ["inspect", "keys", "-sk", sk])
         assert result.exit_code == 0
         assert sk in result.output
@@ -403,16 +411,20 @@
         assert modified_synthetic_sk in result.output
 
     def test_signatures(self):
         secret_key_1: str = "70432627e84c13c1a6e6007bf6d9a7a0342018fdef7fc911757aad5a6929d20a"
         secret_key_2: str = "0f01f7f68935f8594548bca3892fec419c6b2aa7cff54c3353a2e9b1011f09c7"
         text_message: str = "cafe food"
         bytes_message: str = "0xcafef00d"
-        extra_signature: str = "b5d4e653ec9a737d19abe9af7050d37b0f464f9570ec66a8457fbdabdceb50a77c6610eb442ed1e4ace39d9ecc6d40560de239c1c8f7a115e052438385d594be7394df9287cf30c3254d39f0ae21daefc38d3d07ba3e373628bf8ed73f074a80"  # noqa
-        final_signature: str = "b7a6ab2c825068eb40298acab665f95c13779e828d900b8056215b54e47d8b8314e8b61fbb9c98a23ef8a134155a35b109ba284bd5f1f90f96e0d41427132b3ca6a83faae0806daa632ee6b1602a0b4bad92f2743fdeb452822f0599dfa147c0"  # noqa
+        extra_signature: str = (
+            "b5d4e653ec9a737d19abe9af7050d37b0f464f9570ec66a8457fbdabdceb50a77c6610eb442ed1e4ace39d9ecc6d40560de239c1c8f7a115e052438385d594be7394df9287cf30c3254d39f0ae21daefc38d3d07ba3e373628bf8ed73f074a80"  # noqa
+        )
+        final_signature: str = (
+            "b7a6ab2c825068eb40298acab665f95c13779e828d900b8056215b54e47d8b8314e8b61fbb9c98a23ef8a134155a35b109ba284bd5f1f90f96e0d41427132b3ca6a83faae0806daa632ee6b1602a0b4bad92f2743fdeb452822f0599dfa147c0"  # noqa
+        )
 
         runner = CliRunner()
 
         # Test that an empty command returns an empty signature
         result = runner.invoke(cli, ["inspect", "signatures"])
         assert result.exit_code == 0
         assert EMPTY_SIG in result.output
```

### Comparing `chik_dev_tools-1.2.3/tests/test_skeleton.py` & `chik_dev_tools-1.2.6/tests/test_skeleton.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 
 from cdv.test import setup as setup_test
 
 
 class TestSomething:
     @pytest_asyncio.fixture(scope="function")
     async def setup(self):
-        network, alice, bob = await setup_test()
-        await network.farm_block()
-        yield network, alice, bob
+        async with setup_test() as (network, alice, bob):
+            await network.farm_block()
+            yield network, alice, bob
 
     @pytest.mark.asyncio
     async def test_something(self, setup):
         network, alice, bob = setup
         try:
             pass
         finally:
-            await network.close()
+            pass
```

