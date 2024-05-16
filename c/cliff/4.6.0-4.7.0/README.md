# Comparing `tmp/cliff-4.6.0.tar.gz` & `tmp/cliff-4.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cliff-4.6.0.tar", last modified: Thu Feb 22 14:56:41 2024, max compression
+gzip compressed data, was "cliff-4.7.0.tar", last modified: Thu May 16 12:52:01 2024, max compression
```

## Comparing `cliff-4.6.0.tar` & `cliff-4.7.0.tar`

### file list

```diff
@@ -1,117 +1,118 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:56:41.261216 cliff-4.6.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      874 2024-02-22 14:56:13.000000 cliff-4.6.0/.pre-commit-config.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       39 2024-02-22 14:56:13.000000 cliff-4.6.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1086 2024-02-22 14:56:13.000000 cliff-4.6.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4437 2024-02-22 14:56:41.000000 cliff-4.6.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      371 2024-02-22 14:56:13.000000 cliff-4.6.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25244 2024-02-22 14:56:40.000000 cliff-4.6.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11358 2024-02-22 14:56:13.000000 cliff-4.6.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2037 2024-02-22 14:56:41.261216 cliff-4.6.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      920 2024-02-22 14:56:13.000000 cliff-4.6.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       40 2024-02-22 14:56:13.000000 cliff-4.6.0/bandit.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:56:41.237215 cliff-4.6.0/cliff/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:56:13.000000 cliff-4.6.0/cliff/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3811 2024-02-22 14:56:13.000000 cliff-4.6.0/cliff/_argparse.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16720 2024-02-22 14:56:13.000000 cliff-4.6.0/cliff/app.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1613 2024-02-22 14:56:13.000000 cliff-4.6.0/cliff/columns.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7592 2024-02-22 14:56:13.000000 cliff-4.6.0/cliff/command.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5860 2024-02-22 14:56:13.000000 cliff-4.6.0/cliff/commandmanager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6529 2024-02-22 14:56:13.000000 cliff-4.6.0/cliff/complete.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4834 2024-02-22 14:56:13.000000 cliff-4.6.0/cliff/display.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:56:41.241215 cliff-4.6.0/cliff/formatters/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:56:13.000000 cliff-4.6.0/cliff/formatters/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2604 2024-02-22 14:56:13.000000 cliff-4.6.0/cliff/formatters/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1807 2024-02-22 14:56:13.000000 cliff-4.6.0/cliff/formatters/commaseparated.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1863 2024-02-22 14:56:13.000000 cliff-4.6.0/cliff/formatters/json_format.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2377 2024-02-22 14:56:13.000000 cliff-4.6.0/cliff/formatters/shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7829 2024-02-22 14:56:13.000000 cliff-4.6.0/cliff/formatters/table.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1400 2024-02-22 14:56:13.000000 cliff-4.6.0/cliff/formatters/value.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1789 2024-02-22 14:56:13.000000 cliff-4.6.0/cliff/formatters/yaml_format.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5695 2024-02-22 14:56:13.000000 cliff-4.6.0/cliff/help.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1953 2024-02-22 14:56:13.000000 cliff-4.6.0/cliff/hooks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8444 2024-02-22 14:56:13.000000 cliff-4.6.0/cliff/interactive.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4653 2024-02-22 14:56:13.000000 cliff-4.6.0/cliff/lister.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1888 2024-02-22 14:56:13.000000 cliff-4.6.0/cliff/show.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13016 2024-02-22 14:56:13.000000 cliff-4.6.0/cliff/sphinxext.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:56:41.249216 cliff-4.6.0/cliff/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:56:13.000000 cliff-4.6.0/cliff/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1121 2024-02-22 14:56:13.000000 cliff-4.6.0/cliff/tests/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2011 2024-02-22 14:56:13.000000 cliff-4.6.0/cliff/tests/test__argparse.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19882 2024-02-22 14:56:13.000000 cliff-4.6.0/cliff/tests/test_app.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1872 2024-02-22 14:56:13.000000 cliff-4.6.0/cliff/tests/test_columns.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7837 2024-02-22 14:56:13.000000 cliff-4.6.0/cliff/tests/test_command.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13898 2024-02-22 14:56:13.000000 cliff-4.6.0/cliff/tests/test_command_hooks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10890 2024-02-22 14:56:13.000000 cliff-4.6.0/cliff/tests/test_commandmanager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6880 2024-02-22 14:56:13.000000 cliff-4.6.0/cliff/tests/test_complete.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2967 2024-02-22 14:56:13.000000 cliff-4.6.0/cliff/tests/test_formatters_csv.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3980 2024-02-22 14:56:13.000000 cliff-4.6.0/cliff/tests/test_formatters_json.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3369 2024-02-22 14:56:13.000000 cliff-4.6.0/cliff/tests/test_formatters_shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24448 2024-02-22 14:56:13.000000 cliff-4.6.0/cliff/tests/test_formatters_table.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2220 2024-02-22 14:56:13.000000 cliff-4.6.0/cliff/tests/test_formatters_value.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4604 2024-02-22 14:56:13.000000 cliff-4.6.0/cliff/tests/test_formatters_yaml.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6891 2024-02-22 14:56:13.000000 cliff-4.6.0/cliff/tests/test_help.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3537 2024-02-22 14:56:13.000000 cliff-4.6.0/cliff/tests/test_interactive.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6699 2024-02-22 14:56:13.000000 cliff-4.6.0/cliff/tests/test_lister.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2523 2024-02-22 14:56:13.000000 cliff-4.6.0/cliff/tests/test_show.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8454 2024-02-22 14:56:13.000000 cliff-4.6.0/cliff/tests/test_sphinxext.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1338 2024-02-22 14:56:13.000000 cliff-4.6.0/cliff/tests/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1391 2024-02-22 14:56:13.000000 cliff-4.6.0/cliff/tests/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3248 2024-02-22 14:56:13.000000 cliff-4.6.0/cliff/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:56:41.241215 cliff-4.6.0/cliff.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2037 2024-02-22 14:56:41.000000 cliff-4.6.0/cliff.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2723 2024-02-22 14:56:41.000000 cliff-4.6.0/cliff.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-02-22 14:56:41.000000 cliff-4.6.0/cliff.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      987 2024-02-22 14:56:41.000000 cliff-4.6.0/cliff.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-02-22 14:56:41.000000 cliff-4.6.0/cliff.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-02-22 14:56:41.000000 cliff-4.6.0/cliff.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2024-02-22 14:56:41.000000 cliff-4.6.0/cliff.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        6 2024-02-22 14:56:41.000000 cliff-4.6.0/cliff.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:56:41.249216 cliff-4.6.0/demoapp/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      959 2024-02-22 14:56:13.000000 cliff-4.6.0/demoapp/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:56:41.253216 cliff-4.6.0/demoapp/cliffdemo/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:56:13.000000 cliff-4.6.0/demoapp/cliffdemo/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2024-02-22 14:56:13.000000 cliff-4.6.0/demoapp/cliffdemo/__main__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      455 2024-02-22 14:56:13.000000 cliff-4.6.0/demoapp/cliffdemo/encoding.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1510 2024-02-22 14:56:13.000000 cliff-4.6.0/demoapp/cliffdemo/hook.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2024-02-22 14:56:13.000000 cliff-4.6.0/demoapp/cliffdemo/list.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      858 2024-02-22 14:56:13.000000 cliff-4.6.0/demoapp/cliffdemo/main.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      812 2024-02-22 14:56:13.000000 cliff-4.6.0/demoapp/cliffdemo/show.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      551 2024-02-22 14:56:13.000000 cliff-4.6.0/demoapp/cliffdemo/simple.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1800 2024-02-22 14:56:13.000000 cliff-4.6.0/demoapp/setup.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:56:41.253216 cliff-4.6.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2024-02-22 14:56:13.000000 cliff-4.6.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:56:41.253216 cliff-4.6.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8458 2024-02-22 14:56:13.000000 cliff-4.6.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:56:41.253216 cliff-4.6.0/doc/source/contributors/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1612 2024-02-22 14:56:13.000000 cliff-4.6.0/doc/source/contributors/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      477 2024-02-22 14:56:13.000000 cliff-4.6.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:56:41.253216 cliff-4.6.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      747 2024-02-22 14:56:13.000000 cliff-4.6.0/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:56:41.253216 cliff-4.6.0/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      925 2024-02-22 14:56:13.000000 cliff-4.6.0/doc/source/reference/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:56:41.257216 cliff-4.6.0/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1216 2024-02-22 14:56:13.000000 cliff-4.6.0/doc/source/user/complete.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9043 2024-02-22 14:56:13.000000 cliff-4.6.0/doc/source/user/demoapp.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       32 2024-02-22 14:56:13.000000 cliff-4.6.0/doc/source/user/history.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2024-02-22 14:56:13.000000 cliff-4.6.0/doc/source/user/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2650 2024-02-22 14:56:13.000000 cliff-4.6.0/doc/source/user/interactive_mode.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2781 2024-02-22 14:56:13.000000 cliff-4.6.0/doc/source/user/introduction.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3611 2024-02-22 14:56:13.000000 cliff-4.6.0/doc/source/user/list_commands.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3517 2024-02-22 14:56:13.000000 cliff-4.6.0/doc/source/user/show_commands.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7121 2024-02-22 14:56:13.000000 cliff-4.6.0/doc/source/user/sphinxext.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:56:41.257216 cliff-4.6.0/integration-tests/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      477 2024-02-22 14:56:13.000000 cliff-4.6.0/integration-tests/neutronclient-tip.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      599 2024-02-22 14:56:13.000000 cliff-4.6.0/integration-tests/openstackclient-tip.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:56:41.229215 cliff-4.6.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:56:41.261216 cliff-4.6.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      914 2024-02-22 14:56:13.000000 cliff-4.6.0/releasenotes/notes/add-Lister-sort-direction-5f34dba3c9743572.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2024-02-22 14:56:13.000000 cliff-4.6.0/releasenotes/notes/command-group-8c00f260340a130c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      426 2024-02-22 14:56:13.000000 cliff-4.6.0/releasenotes/notes/comparable-FormattableColumn-31c0030ced70b7fb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2024-02-22 14:56:13.000000 cliff-4.6.0/releasenotes/notes/drop-python27-support-b16c9e5a9e2000ef.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      353 2024-02-22 14:56:13.000000 cliff-4.6.0/releasenotes/notes/handle-none-values-when-sorting-de40e36c66ad95ca.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2024-02-22 14:56:13.000000 cliff-4.6.0/releasenotes/notes/strip-period-from-help-strings-be368e5cf5bd5269.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2024-02-22 14:56:13.000000 cliff-4.6.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1851 2024-02-22 14:56:41.261216 cliff-4.6.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      803 2024-02-22 14:56:13.000000 cliff-4.6.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      335 2024-02-22 14:56:13.000000 cliff-4.6.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1607 2024-02-22 14:56:13.000000 cliff-4.6.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:52:01.255100 cliff-4.7.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2024-05-16 12:51:30.000000 cliff-4.7.0/.git-blame-ignore-revs
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      869 2024-05-16 12:51:30.000000 cliff-4.7.0/.pre-commit-config.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       39 2024-05-16 12:51:30.000000 cliff-4.7.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1086 2024-05-16 12:51:30.000000 cliff-4.7.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4437 2024-05-16 12:52:01.000000 cliff-4.7.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      371 2024-05-16 12:51:30.000000 cliff-4.7.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25395 2024-05-16 12:52:01.000000 cliff-4.7.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11358 2024-05-16 12:51:30.000000 cliff-4.7.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2037 2024-05-16 12:52:01.255100 cliff-4.7.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      920 2024-05-16 12:51:30.000000 cliff-4.7.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       40 2024-05-16 12:51:30.000000 cliff-4.7.0/bandit.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:52:01.243099 cliff-4.7.0/cliff/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:51:30.000000 cliff-4.7.0/cliff/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3839 2024-05-16 12:51:30.000000 cliff-4.7.0/cliff/_argparse.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16702 2024-05-16 12:51:30.000000 cliff-4.7.0/cliff/app.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1588 2024-05-16 12:51:30.000000 cliff-4.7.0/cliff/columns.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7541 2024-05-16 12:51:30.000000 cliff-4.7.0/cliff/command.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5858 2024-05-16 12:51:30.000000 cliff-4.7.0/cliff/commandmanager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6617 2024-05-16 12:51:30.000000 cliff-4.7.0/cliff/complete.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4776 2024-05-16 12:51:30.000000 cliff-4.7.0/cliff/display.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:52:01.247100 cliff-4.7.0/cliff/formatters/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:51:30.000000 cliff-4.7.0/cliff/formatters/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2593 2024-05-16 12:51:30.000000 cliff-4.7.0/cliff/formatters/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1905 2024-05-16 12:51:30.000000 cliff-4.7.0/cliff/formatters/commaseparated.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1986 2024-05-16 12:51:30.000000 cliff-4.7.0/cliff/formatters/json_format.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2351 2024-05-16 12:51:30.000000 cliff-4.7.0/cliff/formatters/shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7860 2024-05-16 12:51:30.000000 cliff-4.7.0/cliff/formatters/table.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1553 2024-05-16 12:51:30.000000 cliff-4.7.0/cliff/formatters/value.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1788 2024-05-16 12:51:30.000000 cliff-4.7.0/cliff/formatters/yaml_format.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5631 2024-05-16 12:51:30.000000 cliff-4.7.0/cliff/help.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1953 2024-05-16 12:51:30.000000 cliff-4.7.0/cliff/hooks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8421 2024-05-16 12:51:30.000000 cliff-4.7.0/cliff/interactive.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4741 2024-05-16 12:51:30.000000 cliff-4.7.0/cliff/lister.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1818 2024-05-16 12:51:30.000000 cliff-4.7.0/cliff/show.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13169 2024-05-16 12:51:30.000000 cliff-4.7.0/cliff/sphinxext.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:52:01.251100 cliff-4.7.0/cliff/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:51:30.000000 cliff-4.7.0/cliff/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1120 2024-05-16 12:51:30.000000 cliff-4.7.0/cliff/tests/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2010 2024-05-16 12:51:30.000000 cliff-4.7.0/cliff/tests/test__argparse.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19673 2024-05-16 12:51:30.000000 cliff-4.7.0/cliff/tests/test_app.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1870 2024-05-16 12:51:30.000000 cliff-4.7.0/cliff/tests/test_columns.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7797 2024-05-16 12:51:30.000000 cliff-4.7.0/cliff/tests/test_command.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13397 2024-05-16 12:51:30.000000 cliff-4.7.0/cliff/tests/test_command_hooks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11094 2024-05-16 12:51:30.000000 cliff-4.7.0/cliff/tests/test_commandmanager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6833 2024-05-16 12:51:30.000000 cliff-4.7.0/cliff/tests/test_complete.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2966 2024-05-16 12:51:30.000000 cliff-4.7.0/cliff/tests/test_formatters_csv.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3854 2024-05-16 12:51:30.000000 cliff-4.7.0/cliff/tests/test_formatters_json.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3408 2024-05-16 12:51:30.000000 cliff-4.7.0/cliff/tests/test_formatters_shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24498 2024-05-16 12:51:30.000000 cliff-4.7.0/cliff/tests/test_formatters_table.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2219 2024-05-16 12:51:30.000000 cliff-4.7.0/cliff/tests/test_formatters_value.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4480 2024-05-16 12:51:30.000000 cliff-4.7.0/cliff/tests/test_formatters_yaml.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6899 2024-05-16 12:51:30.000000 cliff-4.7.0/cliff/tests/test_help.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3579 2024-05-16 12:51:30.000000 cliff-4.7.0/cliff/tests/test_interactive.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6778 2024-05-16 12:51:30.000000 cliff-4.7.0/cliff/tests/test_lister.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2520 2024-05-16 12:51:30.000000 cliff-4.7.0/cliff/tests/test_show.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8927 2024-05-16 12:51:30.000000 cliff-4.7.0/cliff/tests/test_sphinxext.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1337 2024-05-16 12:51:30.000000 cliff-4.7.0/cliff/tests/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1388 2024-05-16 12:51:30.000000 cliff-4.7.0/cliff/tests/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3208 2024-05-16 12:51:30.000000 cliff-4.7.0/cliff/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:52:01.243099 cliff-4.7.0/cliff.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2037 2024-05-16 12:52:01.000000 cliff-4.7.0/cliff.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2746 2024-05-16 12:52:01.000000 cliff-4.7.0/cliff.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-16 12:52:01.000000 cliff-4.7.0/cliff.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      987 2024-05-16 12:52:01.000000 cliff-4.7.0/cliff.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-16 12:52:01.000000 cliff-4.7.0/cliff.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-05-16 12:52:01.000000 cliff-4.7.0/cliff.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2024-05-16 12:52:01.000000 cliff-4.7.0/cliff.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        6 2024-05-16 12:52:01.000000 cliff-4.7.0/cliff.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:52:01.251100 cliff-4.7.0/demoapp/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      959 2024-05-16 12:51:30.000000 cliff-4.7.0/demoapp/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:52:01.251100 cliff-4.7.0/demoapp/cliffdemo/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:51:30.000000 cliff-4.7.0/demoapp/cliffdemo/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2024-05-16 12:51:30.000000 cliff-4.7.0/demoapp/cliffdemo/__main__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      437 2024-05-16 12:51:30.000000 cliff-4.7.0/demoapp/cliffdemo/encoding.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1510 2024-05-16 12:51:30.000000 cliff-4.7.0/demoapp/cliffdemo/hook.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      396 2024-05-16 12:51:30.000000 cliff-4.7.0/demoapp/cliffdemo/list.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      853 2024-05-16 12:51:30.000000 cliff-4.7.0/demoapp/cliffdemo/main.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      775 2024-05-16 12:51:30.000000 cliff-4.7.0/demoapp/cliffdemo/show.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      551 2024-05-16 12:51:30.000000 cliff-4.7.0/demoapp/cliffdemo/simple.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1768 2024-05-16 12:51:30.000000 cliff-4.7.0/demoapp/setup.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:52:01.251100 cliff-4.7.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2024-05-16 12:51:30.000000 cliff-4.7.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:52:01.251100 cliff-4.7.0/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8493 2024-05-16 12:51:30.000000 cliff-4.7.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:52:01.251100 cliff-4.7.0/doc/source/contributors/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1612 2024-05-16 12:51:30.000000 cliff-4.7.0/doc/source/contributors/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      477 2024-05-16 12:51:30.000000 cliff-4.7.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:52:01.251100 cliff-4.7.0/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      747 2024-05-16 12:51:30.000000 cliff-4.7.0/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:52:01.251100 cliff-4.7.0/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      925 2024-05-16 12:51:30.000000 cliff-4.7.0/doc/source/reference/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:52:01.255100 cliff-4.7.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1216 2024-05-16 12:51:30.000000 cliff-4.7.0/doc/source/user/complete.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9043 2024-05-16 12:51:30.000000 cliff-4.7.0/doc/source/user/demoapp.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       32 2024-05-16 12:51:30.000000 cliff-4.7.0/doc/source/user/history.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2024-05-16 12:51:30.000000 cliff-4.7.0/doc/source/user/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2650 2024-05-16 12:51:30.000000 cliff-4.7.0/doc/source/user/interactive_mode.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2781 2024-05-16 12:51:30.000000 cliff-4.7.0/doc/source/user/introduction.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3611 2024-05-16 12:51:30.000000 cliff-4.7.0/doc/source/user/list_commands.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3517 2024-05-16 12:51:30.000000 cliff-4.7.0/doc/source/user/show_commands.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7121 2024-05-16 12:51:30.000000 cliff-4.7.0/doc/source/user/sphinxext.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:52:01.255100 cliff-4.7.0/integration-tests/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      477 2024-05-16 12:51:30.000000 cliff-4.7.0/integration-tests/neutronclient-tip.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      599 2024-05-16 12:51:30.000000 cliff-4.7.0/integration-tests/openstackclient-tip.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:52:01.235099 cliff-4.7.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:52:01.255100 cliff-4.7.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      914 2024-05-16 12:51:30.000000 cliff-4.7.0/releasenotes/notes/add-Lister-sort-direction-5f34dba3c9743572.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2024-05-16 12:51:30.000000 cliff-4.7.0/releasenotes/notes/command-group-8c00f260340a130c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      426 2024-05-16 12:51:30.000000 cliff-4.7.0/releasenotes/notes/comparable-FormattableColumn-31c0030ced70b7fb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2024-05-16 12:51:30.000000 cliff-4.7.0/releasenotes/notes/drop-python27-support-b16c9e5a9e2000ef.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      353 2024-05-16 12:51:30.000000 cliff-4.7.0/releasenotes/notes/handle-none-values-when-sorting-de40e36c66ad95ca.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2024-05-16 12:51:30.000000 cliff-4.7.0/releasenotes/notes/strip-period-from-help-strings-be368e5cf5bd5269.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2024-05-16 12:51:30.000000 cliff-4.7.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1851 2024-05-16 12:52:01.259101 cliff-4.7.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      736 2024-05-16 12:51:30.000000 cliff-4.7.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      295 2024-05-16 12:51:30.000000 cliff-4.7.0/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2001 2024-05-16 12:51:30.000000 cliff-4.7.0/tox.ini
```

### Comparing `cliff-4.6.0/.pre-commit-config.yaml` & `cliff-4.7.0/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 ---
 default_language_version:
   # force all unspecified python hooks to run python3
   python: python3
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.4.0
+    rev: v4.5.0
     hooks:
       - id: trailing-whitespace
       - id: mixed-line-ending
         args: ['--fix', 'lf']
         exclude: '.*\.(svg)$'
       - id: check-byte-order-marker
       - id: check-executables-have-shebangs
       - id: check-merge-conflict
       - id: debug-statements
       - id: check-yaml
         files: .*\.(yaml|yml)$
         exclude: '^zuul.d/.*$'
   - repo: https://github.com/PyCQA/bandit
-    rev: 1.7.5
+    rev: 1.7.7
     hooks:
       - id: bandit
         args: ['-c', 'bandit.yaml']
-#  - repo: https://github.com/psf/black
-#    rev: 23.3.0
-#    hooks:
-#      - id: black
-#        args: ['-S', '-l', '79']
+  - repo: https://github.com/psf/black
+    rev: 24.2.0
+    hooks:
+      - id: black
+        args: ['-S', '-l', '79']
   - repo: https://github.com/pycqa/flake8
-    rev: 6.1.0
+    rev: 7.0.0
     hooks:
       - id: flake8
```

### Comparing `cliff-4.6.0/.zuul.yaml` & `cliff-4.7.0/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `cliff-4.6.0/AUTHORS` & `cliff-4.7.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `cliff-4.6.0/ChangeLog` & `cliff-4.7.0/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 CHANGES
 =======
 
+4.7.0
+-----
+
+* Add fixtures explicitly in test requirements
+* tox: Use pre-commit for linter checks
+* Blacken code base
+* requirements: Bump minimums
+
 4.6.0
 -----
 
 * Test python 3.10 and 3.11
 
 4.5.0
 -----
```

### Comparing `cliff-4.6.0/LICENSE` & `cliff-4.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cliff-4.6.0/PKG-INFO` & `cliff-4.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: cliff
-Version: 4.6.0
+Version: 4.7.0
 Summary: Command Line Interface Formulation Framework
 Home-page: https://docs.openstack.org/cliff/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `cliff-4.6.0/README.rst` & `cliff-4.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `cliff-4.6.0/cliff/_argparse.py` & `cliff-4.7.0/cliff/_argparse.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import argparse as orig_argparse
 import warnings
 
 from autopage import argparse
 
 
 class _ArgumentContainerMixIn(object):
-
     # NOTE(dhellmann): We have to override the methods for creating
     # groups to return our objects that know how to deal with the
     # special conflict handler.
 
     def add_argument_group(self, *args, **kwargs):
         group = _ArgumentGroup(self, *args, **kwargs)
         self._action_groups.append(group)
@@ -40,53 +39,59 @@
             self._option_string_actions,
             action,
             conflicting_actions,
         )
 
 
 class ArgumentParser(_ArgumentContainerMixIn, argparse.ArgumentParser):
-
     pass
 
 
-def _handle_conflict_ignore(container, option_string_actions,
-                            new_action, conflicting_actions):
-
+def _handle_conflict_ignore(
+    container,
+    option_string_actions,
+    new_action,
+    conflicting_actions,
+):
     # Remember the option strings the new action starts with so we can
     # restore them as part of error reporting if we need to.
     original_option_strings = new_action.option_strings
 
     # Remove all of the conflicting option strings from the new action
     # and report an error if none are left at the end.
     for option_string, action in conflicting_actions:
-
         # remove the conflicting option from the new action
         new_action.option_strings.remove(option_string)
         warnings.warn(
-            ('Ignoring option string {} for new action '
-             'because it conflicts with an existing option.').format(
-                 option_string))
+            (
+                'Ignoring option string {} for new action '
+                'because it conflicts with an existing option.'
+            ).format(option_string)
+        )
 
         # if the option now has no option string, remove it from the
         # container holding it
         if not new_action.option_strings:
             new_action.option_strings = original_option_strings
             raise argparse.ArgumentError(
                 new_action,
-                ('Cannot resolve conflicting option string, '
-                 'all names conflict.'),
+                (
+                    'Cannot resolve conflicting option string, '
+                    'all names conflict.'
+                ),
             )
 
 
 class _ArgumentGroup(_ArgumentContainerMixIn, orig_argparse._ArgumentGroup):
     pass
 
 
-class _MutuallyExclusiveGroup(_ArgumentContainerMixIn,
-                              orig_argparse._MutuallyExclusiveGroup):
+class _MutuallyExclusiveGroup(
+    _ArgumentContainerMixIn, orig_argparse._MutuallyExclusiveGroup
+):
     pass
 
 
 class SmartHelpFormatter(argparse.HelpFormatter):
     """Smart help formatter to output raw help message if help contain \n.
 
     Some command help messages maybe have multiple line content, the built-in
```

### Comparing `cliff-4.6.0/cliff/app.py` & `cliff-4.7.0/cliff/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,25 +59,32 @@
 
     NAME = os.path.splitext(os.path.basename(sys.argv[0]))[0]
     if NAME == '__main__':
         NAME = os.path.split(os.path.dirname(sys.argv[0]))[-1]
     LOG = logging.getLogger(NAME)
 
     CONSOLE_MESSAGE_FORMAT = '%(message)s'
-    LOG_FILE_MESSAGE_FORMAT = \
+    LOG_FILE_MESSAGE_FORMAT = (
         '[%(asctime)s] %(levelname)-8s %(name)s %(message)s'
+    )
     DEFAULT_VERBOSE_LEVEL = 1
     DEFAULT_OUTPUT_ENCODING = 'utf-8'
 
-    def __init__(self, description, version, command_manager,
-                 stdin=None, stdout=None, stderr=None,
-                 interactive_app_factory=None,
-                 deferred_help=False):
-        """Initialize the application.
-        """
+    def __init__(
+        self,
+        description,
+        version,
+        command_manager,
+        stdin=None,
+        stdout=None,
+        stderr=None,
+        interactive_app_factory=None,
+        deferred_help=False,
+    ):
+        """Initialize the application."""
         self.command_manager = command_manager
         self.command_manager.add_command('help', help.HelpCommand)
         self.command_manager.add_command('complete', complete.CompleteCommand)
         self._set_streams(stdin, stdout, stderr)
         self.interactive_app_factory = interactive_app_factory
         self.deferred_help = deferred_help
         self.parser = self.build_option_parser(description, version)
@@ -116,16 +123,15 @@
         # has not already already wrapped sys.stdin, sys.stdout and
         # sys.stderr as this is a common recommendation.
 
         self.stdin = stdin or sys.stdin
         self.stdout = stdout or sys.stdout
         self.stderr = stderr or sys.stderr
 
-    def build_option_parser(self, description, version,
-                            argparse_kwargs=None):
+    def build_option_parser(self, description, version, argparse_kwargs=None):
         """Return an argparse option parser for this application.
 
         Subclasses may override this method to extend
         the parser with more global options.
 
         :param description: full description of the application
         :paramtype description: str
@@ -133,88 +139,90 @@
         :paramtype version: str
         :param argparse_kwargs: extra keyword argument passed to the
                                 ArgumentParser constructor
         :paramtype extra_kwargs: dict
         """
         argparse_kwargs = argparse_kwargs or {}
         parser = _argparse.ArgumentParser(
-            description=description,
-            add_help=False,
-            **argparse_kwargs
+            description=description, add_help=False, **argparse_kwargs
         )
         parser.add_argument(
             '--version',
             action='version',
             version='{0} {1}'.format(App.NAME, version),
         )
         verbose_group = parser.add_mutually_exclusive_group()
         verbose_group.add_argument(
-            '-v', '--verbose',
+            '-v',
+            '--verbose',
             action='count',
             dest='verbose_level',
             default=self.DEFAULT_VERBOSE_LEVEL,
             help='Increase verbosity of output. Can be repeated.',
         )
         verbose_group.add_argument(
-            '-q', '--quiet',
+            '-q',
+            '--quiet',
             action='store_const',
             dest='verbose_level',
             const=0,
             help='Suppress output except warnings and errors.',
         )
         parser.add_argument(
             '--log-file',
             action='store',
             default=None,
             help='Specify a file to log output. Disabled by default.',
         )
         if self.deferred_help:
             parser.add_argument(
-                '-h', '--help',
+                '-h',
+                '--help',
                 dest='deferred_help',
                 action='store_true',
                 help="Show help message and exit.",
             )
         else:
             parser.add_argument(
-                '-h', '--help',
+                '-h',
+                '--help',
                 action=help.HelpAction,
                 nargs=0,
                 default=self,  # tricky
                 help="Show help message and exit.",
             )
         parser.add_argument(
             '--debug',
             default=False,
             action='store_true',
             help='Show tracebacks on errors.',
         )
         return parser
 
     def configure_logging(self):
-        """Create logging handlers for any log output.
-        """
+        """Create logging handlers for any log output."""
         root_logger = logging.getLogger('')
         root_logger.setLevel(logging.DEBUG)
 
         # Set up logging to a file
         if self.options.log_file:
             file_handler = logging.FileHandler(
                 filename=self.options.log_file,
             )
             formatter = logging.Formatter(self.LOG_FILE_MESSAGE_FORMAT)
             file_handler.setFormatter(formatter)
             root_logger.addHandler(file_handler)
 
         # Always send higher-level messages to the console via stderr
         console = logging.StreamHandler(self.stderr)
-        console_level = {0: logging.WARNING,
-                         1: logging.INFO,
-                         2: logging.DEBUG,
-                         }.get(self.options.verbose_level, logging.DEBUG)
+        console_level = {
+            0: logging.WARNING,
+            1: logging.INFO,
+            2: logging.DEBUG,
+        }.get(self.options.verbose_level, logging.DEBUG)
         console.setLevel(console_level)
         formatter = logging.Formatter(self.CONSOLE_MESSAGE_FORMAT)
         console.setFormatter(formatter)
         root_logger.addHandler(console)
         return
 
     def print_help_if_requested(self):
@@ -316,39 +324,43 @@
 
     def interact(self):
         # Defer importing .interactive as cmd2 is a slow import
         from .interactive import InteractiveApp
 
         if self.interactive_app_factory is None:
             self.interactive_app_factory = InteractiveApp
-        self.interpreter = self.interactive_app_factory(self,
-                                                        self.command_manager,
-                                                        self.stdin,
-                                                        self.stdout,
-                                                        )
+        self.interpreter = self.interactive_app_factory(
+            self,
+            self.command_manager,
+            self.stdin,
+            self.stdout,
+        )
         return self.interpreter.cmdloop()
 
     def get_fuzzy_matches(self, cmd):
-        """return fuzzy matches of unknown command
-        """
+        """return fuzzy matches of unknown command"""
 
         sep = '_'
         if self.command_manager.convert_underscores:
             sep = ' '
         all_cmds = [k[0] for k in self.command_manager]
         dist = []
         for candidate in sorted(all_cmds):
             prefix = candidate.split(sep)[0]
             # Give prefix match a very good score
             if candidate.startswith(cmd):
                 dist.append((0, candidate))
                 continue
             # Levenshtein distance
-            dist.append((utils.damerau_levenshtein(cmd, prefix, utils.COST)+1,
-                         candidate))
+            dist.append(
+                (
+                    utils.damerau_levenshtein(cmd, prefix, utils.COST) + 1,
+                    candidate,
+                )
+            )
 
         matches = []
         match_distance = 0
         for distance, candidate in sorted(dist):
             if distance > match_distance:
                 if match_distance:
                     # we copied all items with minimum distance, we are done
@@ -367,18 +379,25 @@
             # If there was no exact match, try to find a fuzzy match
             the_cmd = argv[0]
             fuzzy_matches = self.get_fuzzy_matches(the_cmd)
             if fuzzy_matches:
                 article = 'a'
                 if self.NAME[0] in 'aeiou':
                     article = 'an'
-                self.stdout.write('%s: \'%s\' is not %s %s command. '
-                                  'See \'%s --help\'.\n'
-                                  % (self.NAME, ' '.join(argv), article,
-                                      self.NAME, self.NAME))
+                self.stdout.write(
+                    '%s: \'%s\' is not %s %s command. '
+                    'See \'%s --help\'.\n'
+                    % (
+                        self.NAME,
+                        ' '.join(argv),
+                        article,
+                        self.NAME,
+                        self.NAME,
+                    )
+                )
                 self.stdout.write('Did you mean one of these?\n')
                 for match in fuzzy_matches:
                     self.stdout.write('  %s\n' % match)
             else:
                 if self.options.debug:
                     raise
                 else:
@@ -389,25 +408,27 @@
         if 'cmd_name' in inspect.getfullargspec(cmd_factory.__init__).args:
             kwargs['cmd_name'] = cmd_name
         cmd = cmd_factory(self, self.options, **kwargs)
         result = 1
         err = None
         try:
             self.prepare_to_run_command(cmd)
-            full_name = (cmd_name
-                         if self.interactive_mode
-                         else ' '.join([self.NAME, cmd_name])
-                         )
+            full_name = (
+                cmd_name
+                if self.interactive_mode
+                else ' '.join([self.NAME, cmd_name])
+            )
             cmd_parser = cmd.get_parser(full_name)
             try:
                 parsed_args = cmd_parser.parse_args(sub_argv)
             except SystemExit as ex:
                 if self.interactive_mode:
                     # Defer importing cmd2 as it is a slow import
                     import cmd2
+
                     raise cmd2.exceptions.Cmd2ArgparseError from ex
                 else:
                     raise ex
             result = cmd.run(parsed_args)
         except BrokenPipeError as err1:
             result = _SIGPIPE_EXIT
             err = err1
```

### Comparing `cliff-4.6.0/cliff/columns.py` & `cliff-4.7.0/cliff/columns.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,27 +13,24 @@
 """Formattable column tools.
 """
 
 import abc
 
 
 class FormattableColumn(object, metaclass=abc.ABCMeta):
-
     def __init__(self, value):
         self._value = value
 
     def __eq__(self, other):
         return (
             self.__class__ == other.__class__ and self._value == other._value
         )
 
     def __lt__(self, other):
-        return (
-            self.__class__ == other.__class__ and self._value < other._value
-        )
+        return self.__class__ == other.__class__ and self._value < other._value
 
     def __str__(self):
         return self.human_readable()
 
     def __repr__(self):
         return '%s(%r)' % (self.__class__.__name__, self.machine_readable())
```

### Comparing `cliff-4.6.0/cliff/command.py` & `cliff-4.7.0/cliff/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,17 +35,15 @@
     always match. We want to report which distribution caused the
     command to be installed, so we need to look up the values.
     """
     global _dists_by_mods
     if _dists_by_mods is None:
         # There can be multiple distribution in the case of namespace packages
         # so we'll just grab the first one
-        _dists_by_mods = {
-            k: v[0] for k, v in packages_distributions().items()
-        }
+        _dists_by_mods = {k: v[0] for k, v in packages_distributions().items()}
     return _dists_by_mods
 
 
 def _get_distribution_for_module(module):
     "Return the distribution containing the module."
     dist_name = None
     if module:
@@ -81,15 +79,15 @@
         self._load_hooks()
 
     def _load_hooks(self):
         # Look for command extensions
         if self.app and self.cmd_name:
             namespace = '{}.{}'.format(
                 self.app.command_manager.namespace,
-                self.cmd_name.replace(' ', '_')
+                self.cmd_name.replace(' ', '_'),
             )
             self._hooks = extension.ExtensionManager(
                 namespace=namespace,
                 invoke_on_load=True,
                 invoke_kwds={
                     'command': self,
                 },
@@ -128,29 +126,27 @@
         parts = [self._epilog or '']
         hook_epilogs = filter(
             None,
             (h.obj.get_epilog() for h in self._hooks),
         )
         parts.extend(hook_epilogs)
         app_dist_name = getattr(
-            self, 'app_dist_name', _get_distribution_for_module(
-                inspect.getmodule(self.app)
-            )
+            self,
+            'app_dist_name',
+            _get_distribution_for_module(inspect.getmodule(self.app)),
         )
         dist_name = _get_distribution_for_module(inspect.getmodule(self))
         if dist_name and dist_name != app_dist_name:
             parts.append(
-                'This command is provided by the %s plugin.' %
-                (dist_name,)
+                'This command is provided by the %s plugin.' % (dist_name,)
             )
         return '\n\n'.join(parts)
 
     def get_parser(self, prog_name):
-        """Return an :class:`argparse.ArgumentParser`.
-        """
+        """Return an :class:`argparse.ArgumentParser`."""
         parser = _argparse.ArgumentParser(
             description=self.get_description(),
             epilog=self.get_epilog(),
             prog=prog_name,
             formatter_class=_argparse.SmartHelpFormatter,
             conflict_handler=self.conflict_handler,
         )
```

### Comparing `cliff-4.6.0/cliff/commandmanager.py` & `cliff-4.7.0/cliff/commandmanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,16 +31,15 @@
             continue
         if all(command_parts[i].startswith(args[i]) for i in range(n)):
             candidates.append(command_name)
     return candidates
 
 
 class EntryPointWrapper(object):
-    """Wrap up a command class already imported to make it look like a plugin.
-    """
+    """Wrap up a command class already imported to make it look like a plugin."""
 
     def __init__(self, name, command_class):
         self.name = name
         self.command_class = command_class
 
     def load(self, require=False):
         return self.command_class
@@ -50,14 +49,15 @@
     """Discovers commands and handles lookup based on argv data.
 
     :param namespace: String containing the entrypoint namespace for the
         plugins to be loaded. For example, ``'cliff.formatter.list'``.
     :param convert_underscores: Whether cliff should convert underscores to
         spaces in entry_point commands.
     """
+
     def __init__(self, namespace, convert_underscores=True):
         self.commands = {}
         self._legacy = {}
         self.namespace = namespace
         self.convert_underscores = convert_underscores
         self.group_list = []
         self._load_commands()
@@ -68,17 +68,19 @@
             self.load_commands(self.namespace)
 
     def load_commands(self, namespace):
         """Load all the commands from an entrypoint"""
         self.group_list.append(namespace)
         for ep in stevedore.ExtensionManager(namespace):
             LOG.debug('found command %r', ep.name)
-            cmd_name = (ep.name.replace('_', ' ')
-                        if self.convert_underscores
-                        else ep.name)
+            cmd_name = (
+                ep.name.replace('_', ' ')
+                if self.convert_underscores
+                else ep.name
+            )
             self.commands[cmd_name] = ep.entry_point
         return
 
     def __iter__(self):
         return iter(self.commands.items())
 
     def add_command(self, name, command_class):
@@ -110,15 +112,16 @@
                 name = self._legacy[name]
 
             found = None
             if name in self.commands:
                 found = name
             else:
                 candidates = _get_commands_by_partial_name(
-                    argv[:i], self.commands)
+                    argv[:i], self.commands
+                )
                 if len(candidates) == 1:
                     found = candidates[0]
             if found:
                 cmd_ep = self.commands[found]
                 if hasattr(cmd_ep, 'resolve'):
                     cmd_factory = cmd_ep.resolve()
                 else:
@@ -127,16 +130,15 @@
                     arg_spec = inspect.getfullargspec(cmd_ep.load)
                     if 'require' in arg_spec[0]:
                         cmd_factory = cmd_ep.load(require=False)
                     else:
                         cmd_factory = cmd_ep.load()
                 return (cmd_factory, return_name, search_args)
         else:
-            raise ValueError('Unknown command %r' %
-                             (argv,))
+            raise ValueError('Unknown command %r' % (argv,))
 
     def _get_last_possible_command_index(self, argv):
         """Returns the index after the last argument
         in argv that can be a command word
         """
         for i, arg in enumerate(argv):
             if arg.startswith('-'):
```

### Comparing `cliff-4.6.0/cliff/complete.py` & `cliff-4.7.0/cliff/complete.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,23 +17,23 @@
 
 import stevedore
 
 from cliff import command
 
 
 class CompleteDictionary:
-    """dictionary for bash completion
-    """
+    """dictionary for bash completion"""
 
     def __init__(self):
         self._dictionary = {}
 
     def add_command(self, command, actions):
-        optstr = ' '.join(opt for action in actions
-                          for opt in action.option_strings)
+        optstr = ' '.join(
+            opt for action in actions for opt in action.option_strings
+        )
         dicto = self._dictionary
         last_cmd = command[-1]
         for subcmd in command[:-1]:
             subdata = dicto.get(subcmd)
             # If there is a string in corresponding dictionary, it means the
             # verb used for the command exists already.
             # For example, {'cmd': 'action'}, and we add the command
@@ -65,16 +65,16 @@
         return ray
 
     def get_data(self):
         return sorted(self._get_data_recurse(self._dictionary, ""))
 
 
 class CompleteShellBase(object):
-    """base class for bash completion generation
-    """
+    """base class for bash completion generation"""
+
     def __init__(self, name, output):
         self.name = str(name)
         self.output = output
 
     def write(self, cmdo, data):
         self.output.write(self.get_header())
         self.output.write("  cmds='{0}'\n".format(cmdo))
@@ -85,44 +85,49 @@
 
     @property
     def escaped_name(self):
         return self.name.replace('-', '_')
 
 
 class CompleteNoCode(CompleteShellBase):
-    """completion with no code
-    """
+    """completion with no code"""
+
     def __init__(self, name, output):
         super(CompleteNoCode, self).__init__(name, output)
 
     def get_header(self):
         return ''
 
     def get_trailer(self):
         return ''
 
 
 class CompleteBash(CompleteShellBase):
-    """completion for bash
-    """
+    """completion for bash"""
+
     def __init__(self, name, output):
         super(CompleteBash, self).__init__(name, output)
 
     def get_header(self):
-        return ('_' + self.escaped_name + """()
+        return (
+            '_'
+            + self.escaped_name
+            + """()
 {
   local cur prev words
   COMPREPLY=()
   _get_comp_words_by_ref -n : cur prev words
 
   # Command data:
-""")
+"""
+        )
 
     def get_trailer(self):
-        return ("""
+        return (
+            """
   dash=-
   underscore=_
   cmd=""
   words[0]=""
   completed="${cmds}"
   for var in "${words[@]:1}"
   do
@@ -153,20 +158,24 @@
   if [ -z "${completed}" ] ; then
     COMPREPLY=( $( compgen -f -- "$cur" ) $( compgen -d -- "$cur" ) )
   else
     COMPREPLY=( $(compgen -W "${completed}" -- ${cur}) )
   fi
   return 0
 }
-complete -F _""" + self.escaped_name + ' ' + self.name + '\n')
+complete -F _"""
+            + self.escaped_name
+            + ' '
+            + self.name
+            + '\n'
+        )
 
 
 class CompleteCommand(command.Command):
-    """print bash completion command
-    """
+    """print bash completion command"""
 
     log = logging.getLogger(__name__ + '.CompleteCommand')
 
     def __init__(self, app, app_args, cmd_name=None):
         super(CompleteCommand, self).__init__(app, app_args, cmd_name)
         self._formatters = stevedore.ExtensionManager(
             namespace='cliff.formatter.completion',
@@ -174,33 +183,33 @@
 
     def get_parser(self, prog_name):
         parser = super(CompleteCommand, self).get_parser(prog_name)
         parser.add_argument(
             "--name",
             default=None,
             metavar='<command_name>',
-            help="Command name to support with command completion"
+            help="Command name to support with command completion",
         )
         parser.add_argument(
             "--shell",
             default='bash',
             metavar='<shell>',
             choices=sorted(self._formatters.names()),
-            help="Shell being used. Use none for data only (default: bash)"
+            help="Shell being used. Use none for data only (default: bash)",
         )
         return parser
 
     def get_actions(self, command):
         the_cmd = self.app.command_manager.find_command(command)
         cmd_factory, cmd_name, search_args = the_cmd
         cmd = cmd_factory(self.app, search_args)
         if self.app.interactive_mode:
-            full_name = (cmd_name)
+            full_name = cmd_name
         else:
-            full_name = (' '.join([self.app.NAME, cmd_name]))
+            full_name = ' '.join([self.app.NAME, cmd_name])
         cmd_parser = cmd.get_parser(full_name)
         return cmd_parser._get_optional_actions()
 
     def take_action(self, parsed_args):
         self.log.debug('take_action(%s)' % parsed_args)
 
         name = parsed_args.name or self.app.NAME
```

### Comparing `cliff-4.6.0/cliff/display.py` & `cliff-4.7.0/cliff/display.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,20 +17,20 @@
 
 import stevedore
 
 from . import command
 
 
 class DisplayCommandBase(command.Command, metaclass=abc.ABCMeta):
-    """Command base class for displaying data about a single object.
-    """
+    """Command base class for displaying data about a single object."""
 
     def __init__(self, app, app_args, cmd_name=None):
-        super(DisplayCommandBase, self).__init__(app, app_args,
-                                                 cmd_name=cmd_name)
+        super(DisplayCommandBase, self).__init__(
+            app, app_args, cmd_name=cmd_name
+        )
         self._formatter_plugins = self._load_formatter_plugins()
 
     @property
     @abc.abstractmethod
     def formatter_namespace(self):
         "String specifying the namespace to use for loading formatter plugins."
 
@@ -54,29 +54,31 @@
         )
         self._formatter_group = formatter_group
         formatter_choices = sorted(self._formatter_plugins.names())
         formatter_default = self.formatter_default
         if formatter_default not in formatter_choices:
             formatter_default = formatter_choices[0]
         formatter_group.add_argument(
-            '-f', '--format',
+            '-f',
+            '--format',
             dest='formatter',
             action='store',
             choices=formatter_choices,
             default=formatter_default,
             help='the output format, defaults to %s' % formatter_default,
         )
         formatter_group.add_argument(
-            '-c', '--column',
+            '-c',
+            '--column',
             action='append',
             default=[],
             dest='columns',
             metavar='COLUMN',
             help='specify the column(s) to include, can be '
-                 'repeated to show multiple columns',
+            'repeated to show multiple columns',
         )
         for formatter in self._formatter_plugins:
             formatter.obj.add_argument_group(parser)
         return parser
 
     @abc.abstractmethod
     def produce_output(self, parsed_args, column_names, data):
@@ -95,31 +97,34 @@
         :param column_names: sequence of strings containing names
                              of output columns
         """
         if not parsed_args.columns:
             columns_to_include = column_names
             selector = None
         else:
-            columns_to_include = [c for c in column_names
-                                  if c in parsed_args.columns]
+            columns_to_include = [
+                c for c in column_names if c in parsed_args.columns
+            ]
             if not columns_to_include:
-                raise ValueError('No recognized column names in %s. '
-                                 'Recognized columns are %s.' %
-                                 (str(parsed_args.columns), str(column_names)))
+                raise ValueError(
+                    'No recognized column names in %s. '
+                    'Recognized columns are %s.'
+                    % (str(parsed_args.columns), str(column_names))
+                )
 
             # Set up argument to compress()
-            selector = [(c in columns_to_include)
-                        for c in column_names]
+            selector = [(c in columns_to_include) for c in column_names]
         return columns_to_include, selector
 
     def run(self, parsed_args):
         parsed_args = self._run_before_hooks(parsed_args)
         self.formatter = self._formatter_plugins[parsed_args.formatter].obj
         column_names, data = self.take_action(parsed_args)
-        column_names, data = self._run_after_hooks(parsed_args,
-                                                   (column_names, data))
+        column_names, data = self._run_after_hooks(
+            parsed_args, (column_names, data)
+        )
         self.produce_output(parsed_args, column_names, data)
         return 0
 
     @staticmethod
     def _compress_iterable(iterable, selectors):
         return compress(iterable, selectors)
```

### Comparing `cliff-4.6.0/cliff/formatters/base.py` & `cliff-4.7.0/cliff/formatters/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,26 +13,24 @@
 """Base classes for formatters.
 """
 
 import abc
 
 
 class Formatter(object, metaclass=abc.ABCMeta):
-
     @abc.abstractmethod
     def add_argument_group(self, parser):
         """Add any options to the argument parser.
 
         Should use our own argument group.
         """
 
 
 class ListFormatter(Formatter, metaclass=abc.ABCMeta):
-    """Base class for formatters that know how to deal with multiple objects.
-    """
+    """Base class for formatters that know how to deal with multiple objects."""
 
     @abc.abstractmethod
     def emit_list(self, column_names, data, stdout, parsed_args):
         """Format and print the list from the iterable data source.
 
         Data values can be primitive types like ints and strings, or
         can be an instance of a :class:`FormattableColumn` for
@@ -46,16 +44,15 @@
         :param stdout: output stream where data should be written
         :param parsed_args: argparse namespace from our local options
 
         """
 
 
 class SingleFormatter(Formatter, metaclass=abc.ABCMeta):
-    """Base class for formatters that work with single objects.
-    """
+    """Base class for formatters that work with single objects."""
 
     @abc.abstractmethod
     def emit_one(self, column_names, data, stdout, parsed_args):
         """Format and print the values associated with the single object.
 
         Data values can be primitive types like ints and strings, or
         can be an instance of a :class:`FormattableColumn` for
```

### Comparing `cliff-4.6.0/cliff/formatters/commaseparated.py` & `cliff-4.7.0/cliff/formatters/commaseparated.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 import os
 
 from .base import ListFormatter
 from cliff import columns
 
 
 class CSVLister(ListFormatter):
-
     QUOTE_MODES = {
         'all': csv.QUOTE_ALL,
         'minimal': csv.QUOTE_MINIMAL,
         'nonnumeric': csv.QUOTE_NONNUMERIC,
         'none': csv.QUOTE_NONE,
     }
 
@@ -46,13 +45,17 @@
             escapechar='\\',
         )
 
         writer = csv.writer(stdout, **writer_kwargs)
         writer.writerow(column_names)
         for row in data:
             writer.writerow(
-                [(str(c.machine_readable())
-                  if isinstance(c, columns.FormattableColumn)
-                  else c)
-                 for c in row]
+                [
+                    (
+                        str(c.machine_readable())
+                        if isinstance(c, columns.FormattableColumn)
+                        else c
+                    )
+                    for c in row
+                ]
             )
         return
```

### Comparing `cliff-4.6.0/cliff/formatters/json_format.py` & `cliff-4.7.0/cliff/formatters/json_format.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,40 +16,45 @@
 import json
 
 from . import base
 from cliff import columns
 
 
 class JSONFormatter(base.ListFormatter, base.SingleFormatter):
-
     def add_argument_group(self, parser):
         group = parser.add_argument_group(title='json formatter')
         group.add_argument(
             '--noindent',
             action='store_true',
             dest='noindent',
-            help='whether to disable indenting the JSON'
+            help='whether to disable indenting the JSON',
         )
 
     def emit_list(self, column_names, data, stdout, parsed_args):
         items = []
         for item in data:
             items.append(
-                {n: (i.machine_readable()
-                     if isinstance(i, columns.FormattableColumn)
-                     else i)
-                 for n, i in zip(column_names, item)}
+                {
+                    n: (
+                        i.machine_readable()
+                        if isinstance(i, columns.FormattableColumn)
+                        else i
+                    )
+                    for n, i in zip(column_names, item)
+                }
             )
         indent = None if parsed_args.noindent else 2
         json.dump(items, stdout, indent=indent)
         stdout.write('\n')
 
     def emit_one(self, column_names, data, stdout, parsed_args):
         one = {
-            n: (i.machine_readable()
+            n: (
+                i.machine_readable()
                 if isinstance(i, columns.FormattableColumn)
-                else i)
+                else i
+            )
             for n, i in zip(column_names, data)
         }
         indent = None if parsed_args.noindent else 2
         json.dump(one, stdout, indent=indent)
         stdout.write('\n')
```

### Comparing `cliff-4.6.0/cliff/formatters/shell.py` & `cliff-4.7.0/cliff/formatters/shell.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from . import base
 from cliff import columns
 
 import argparse
 
 
 class ShellFormatter(base.SingleFormatter):
-
     def add_argument_group(self, parser):
         group = parser.add_argument_group(
             title='shell formatter',
             description='a format a UNIX shell can parse (variable="value")',
         )
         group.add_argument(
             '--variable',
@@ -39,23 +38,23 @@
             action='store',
             default='',
             dest='prefix',
             help='add a prefix to all variable names',
         )
 
     def emit_one(self, column_names, data, stdout, parsed_args):
-        variable_names = [c.lower().replace(' ', '_')
-                          for c in column_names
-                          ]
+        variable_names = [c.lower().replace(' ', '_') for c in column_names]
         desired_columns = parsed_args.variables
         for name, value in zip(variable_names, data):
             if name in desired_columns or not desired_columns:
-                value = (str(value.machine_readable())
-                         if isinstance(value, columns.FormattableColumn)
-                         else value)
+                value = (
+                    str(value.machine_readable())
+                    if isinstance(value, columns.FormattableColumn)
+                    else value
+                )
                 if isinstance(value, str):
                     value = value.replace('"', '\\"')
                 if isinstance(name, str):
                     # Colons and dashes may appear as a resource property but
                     # are invalid to use in a shell, replace them with an
                     # underscore.
                     name = name.replace(':', '_')
```

### Comparing `cliff-4.6.0/cliff/formatters/table.py` & `cliff-4.7.0/cliff/formatters/table.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,40 +38,43 @@
         # NOTE(pas-ha) the isatty is not reliable enough on Windows,
         # so do not try to auto-fit
         return fit_width
     return sys.stdout.isatty() or fit_width
 
 
 class TableFormatter(base.ListFormatter, base.SingleFormatter):
-
     ALIGNMENTS = {
         int: 'r',
         str: 'l',
         float: 'r',
     }
 
     def add_argument_group(self, parser):
         group = parser.add_argument_group('table formatter')
         group.add_argument(
             '--max-width',
             metavar='<integer>',
             default=int(os.environ.get('CLIFF_MAX_TERM_WIDTH', 0)),
             type=int,
-            help=('Maximum display width, <1 to disable. You can also '
-                  'use the CLIFF_MAX_TERM_WIDTH environment variable, '
-                  'but the parameter takes precedence.'),
+            help=(
+                'Maximum display width, <1 to disable. You can also '
+                'use the CLIFF_MAX_TERM_WIDTH environment variable, '
+                'but the parameter takes precedence.'
+            ),
         )
         group.add_argument(
             '--fit-width',
             action='store_true',
             default=bool(int(os.environ.get('CLIFF_FIT_WIDTH', 0))),
-            help=('Fit the table to the display width. '
-                  'Implied if --max-width greater than 0. '
-                  'Set the environment variable CLIFF_FIT_WIDTH=1 '
-                  'to always enable'),
+            help=(
+                'Fit the table to the display width. '
+                'Implied if --max-width greater than 0. '
+                'Set the environment variable CLIFF_FIT_WIDTH=1 '
+                'to always enable'
+            ),
         )
         group.add_argument(
             '--print-empty',
             action='store_true',
             help='Print empty table if there is no data to show.',
         )
 
@@ -105,50 +108,50 @@
             self.add_rows(x, column_names, data)
 
         # Choose a reasonable min_width to better handle many columns on a
         # narrow console. The table will overflow the console width in
         # preference to wrapping columns smaller than 8 characters.
         min_width = 8
         self._assign_max_widths(
-            x, int(parsed_args.max_width), min_width,
-            parsed_args.fit_width)
+            x, int(parsed_args.max_width), min_width, parsed_args.fit_width
+        )
 
         formatted = x.get_string()
         stdout.write(formatted)
         stdout.write('\n')
         return
 
     def emit_one(self, column_names, data, stdout, parsed_args):
-        x = prettytable.PrettyTable(field_names=('Field', 'Value'),
-                                    print_empty=False)
+        x = prettytable.PrettyTable(
+            field_names=('Field', 'Value'), print_empty=False
+        )
         x.padding_width = 1
         # Align all columns left because the values are
         # not all the same type.
         x.align['Field'] = 'l'
         x.align['Value'] = 'l'
         for name, value in zip(column_names, data):
             x.add_row(_format_row((name, value)))
 
         # Choose a reasonable min_width to better handle a narrow
         # console. The table will overflow the console width in preference
         # to wrapping columns smaller than 16 characters in an attempt to keep
         # the Field column readable.
         min_width = 16
         self._assign_max_widths(
-            x, int(parsed_args.max_width), min_width,
-            parsed_args.fit_width)
+            x, int(parsed_args.max_width), min_width, parsed_args.fit_width
+        )
 
         formatted = x.get_string()
         stdout.write(formatted)
         stdout.write('\n')
         return
 
     @staticmethod
     def _field_widths(field_names, first_line):
-
         # use the first line +----+-------+ to infer column widths
         # accounting for padding and dividers
         widths = [max(0, len(i) - 2) for i in first_line.split('+')[1:-1]]
         return dict(zip(field_names, widths))
 
     @staticmethod
     def _width_info(term_width, field_count):
@@ -160,16 +163,17 @@
             optimal_width = 0
         else:
             optimal_width = max(0, usable_total_width // field_count)
 
         return usable_total_width, optimal_width
 
     @staticmethod
-    def _build_shrink_fields(usable_total_width, optimal_width,
-                             field_widths, field_names):
+    def _build_shrink_fields(
+        usable_total_width, optimal_width, field_widths, field_names
+    ):
         shrink_fields = []
         shrink_remaining = usable_total_width
         for field in field_names:
             w = field_widths[field]
             if w <= optimal_width:
                 # leave alone columns which are smaller than the optimal width
                 shrink_remaining -= w
@@ -200,20 +204,22 @@
             first_line = x.get_string().splitlines()[0]
             if len(first_line) <= term_width:
                 return
         except IndexError:
             return
 
         usable_total_width, optimal_width = TableFormatter._width_info(
-            term_width, field_count)
+            term_width, field_count
+        )
 
         field_widths = TableFormatter._field_widths(x.field_names, first_line)
 
         shrink_fields, shrink_remaining = TableFormatter._build_shrink_fields(
-            usable_total_width, optimal_width, field_widths, x.field_names)
+            usable_total_width, optimal_width, field_widths, x.field_names
+        )
 
         shrink_to = shrink_remaining // len(shrink_fields)
         # make all shrinkable fields size shrink_to apart from the last one
         for field in shrink_fields[:-1]:
             x.max_width[field] = max(min_width, shrink_to)
             shrink_remaining -= shrink_to
```

### Comparing `cliff-4.6.0/cliff/formatters/value.py` & `cliff-4.7.0/cliff/formatters/value.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,29 +14,36 @@
 """
 
 from . import base
 from cliff import columns
 
 
 class ValueFormatter(base.ListFormatter, base.SingleFormatter):
-
     def add_argument_group(self, parser):
         pass
 
     def emit_list(self, column_names, data, stdout, parsed_args):
         for row in data:
             stdout.write(
                 ' '.join(
-                    str(c.machine_readable()
+                    str(
+                        c.machine_readable()
                         if isinstance(c, columns.FormattableColumn)
-                        else c)
-                    for c in row) + '\n')
+                        else c
+                    )
+                    for c in row
+                )
+                + '\n'
+            )
         return
 
     def emit_one(self, column_names, data, stdout, parsed_args):
         for value in data:
-            stdout.write('%s\n' % str(
-                value.machine_readable()
-                if isinstance(value, columns.FormattableColumn)
-                else value)
+            stdout.write(
+                '%s\n'
+                % str(
+                    value.machine_readable()
+                    if isinstance(value, columns.FormattableColumn)
+                    else value
+                )
             )
         return
```

### Comparing `cliff-4.6.0/cliff/formatters/yaml_format.py` & `cliff-4.7.0/cliff/formatters/yaml_format.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     elif hasattr(value, "to_dict"):
         return value.to_dict()
     else:
         return value
 
 
 class YAMLFormatter(base.ListFormatter, base.SingleFormatter):
-
     def add_argument_group(self, parser):
         pass
 
     def emit_list(self, column_names, data, stdout, parsed_args):
         # the yaml import is slow, so defer loading until we know we want it
         import yaml
```

### Comparing `cliff-4.6.0/cliff/help.py` & `cliff-4.7.0/cliff/help.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,21 +26,21 @@
     anything that used to catch SystemExit, but use a different class
     so that cliff's Application can tell the difference between
     something trying to hard-exit and help saying it's done.
     """
 
 
 class HelpAction(argparse.Action):
-
     """Provide a custom action so the -h and --help options
     to the main app will print a list of the commands.
 
     The commands are determined by checking the CommandManager
     instance, passed in as the "default" value for the action.
     """
+
     def __call__(self, parser, namespace, values, option_string=None):
         app = self.default
         pager = autopage.argparse.help_pager(app.stdout)
         color = pager.to_terminal()
         autopage.argparse.use_color_for_parser(parser, color)
         with pager as out:
             parser.print_help(out)
@@ -86,56 +86,60 @@
                 if color:
                     name = '\033[36m%s\033[39m' % name
                 out.write('  %-13s  %s%s\n' % (name, one_liner, dist_info))
         raise HelpExit()
 
 
 class HelpCommand(command.Command):
-    """print detailed help for another command
-    """
+    """print detailed help for another command"""
 
     def get_parser(self, prog_name):
         parser = super(HelpCommand, self).get_parser(prog_name)
-        parser.add_argument('cmd',
-                            nargs='*',
-                            help='name of the command',
-                            )
+        parser.add_argument(
+            'cmd',
+            nargs='*',
+            help='name of the command',
+        )
         return parser
 
     def take_action(self, parsed_args):
         if parsed_args.cmd:
             try:
                 the_cmd = self.app.command_manager.find_command(
                     parsed_args.cmd,
                 )
                 cmd_factory, cmd_name, search_args = the_cmd
             except ValueError:
                 # Did not find an exact match
                 cmd = parsed_args.cmd[0]
-                fuzzy_matches = [k[0] for k in self.app.command_manager
-                                 if k[0].startswith(cmd)
-                                 ]
+                fuzzy_matches = [
+                    k[0]
+                    for k in self.app.command_manager
+                    if k[0].startswith(cmd)
+                ]
                 if not fuzzy_matches:
                     raise
                 self.app.stdout.write('Command "%s" matches:\n' % cmd)
                 for fm in sorted(fuzzy_matches):
                     self.app.stdout.write('  %s\n' % fm)
                 return
             self.app_args.cmd = search_args
             kwargs = {}
             if 'cmd_name' in inspect.getfullargspec(cmd_factory.__init__).args:
                 kwargs['cmd_name'] = cmd_name
             cmd = cmd_factory(self.app, self.app_args, **kwargs)
-            full_name = (cmd_name
-                         if self.app.interactive_mode
-                         else ' '.join([self.app.NAME, cmd_name])
-                         )
+            full_name = (
+                cmd_name
+                if self.app.interactive_mode
+                else ' '.join([self.app.NAME, cmd_name])
+            )
             cmd_parser = cmd.get_parser(full_name)
             pager = autopage.argparse.help_pager(self.app.stdout)
             with pager as out:
-                autopage.argparse.use_color_for_parser(cmd_parser,
-                                                       pager.to_terminal())
+                autopage.argparse.use_color_for_parser(
+                    cmd_parser, pager.to_terminal()
+                )
                 cmd_parser.print_help(out)
         else:
             action = HelpAction(None, None, default=self.app)
             action(self.app.parser, self.app.options, None, None)
         return 0
```

### Comparing `cliff-4.6.0/cliff/hooks.py` & `cliff-4.7.0/cliff/hooks.py`

 * *Files identical despite different names*

### Comparing `cliff-4.6.0/cliff/interactive.py` & `cliff-4.7.0/cliff/interactive.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,16 +38,17 @@
     :param stdout: Standard output stream
     """
 
     use_rawinput = True
     doc_header = "Shell commands (type help <topic>):"
     app_cmd_header = "Application commands (type help <topic>):"
 
-    def __init__(self, parent_app, command_manager, stdin, stdout,
-                 errexit=False):
+    def __init__(
+        self, parent_app, command_manager, stdin, stdout, errexit=False
+    ):
         self.parent_app = parent_app
         if not hasattr(sys.stdin, 'isatty') or sys.stdin.isatty():
             self.prompt = '(%s) ' % parent_app.NAME
         else:
             # batch/pipe mode
             self.prompt = ''
         self.command_manager = command_manager
@@ -113,16 +114,17 @@
         if arg:
             # Check if the arg is a builtin command or something
             # coming from the command manager
             arg_parts = shlex.split(arg)
             method_name = '_'.join(
                 itertools.chain(
                     ['do'],
-                    itertools.takewhile(lambda x: not x.startswith('-'),
-                                        arg_parts)
+                    itertools.takewhile(
+                        lambda x: not x.startswith('-'), arg_parts
+                    ),
                 )
             )
             # Have the command manager version of the help
             # command produce the help text since cmd and
             # cmd2 do not provide help for "help"
             if hasattr(self, method_name):
                 return cmd2.Cmd.do_help(self, arg)
@@ -156,18 +158,17 @@
     # Create exit alias to quit the interactive shell.
     do_exit = cmd2.Cmd.do_quit
 
     def get_names(self):
         # Override the base class version to filter out
         # things that look like they should be hidden
         # from the user.
-        return [n
-                for n in cmd2.Cmd.get_names(self)
-                if not n.startswith('do__')
-                ]
+        return [
+            n for n in cmd2.Cmd.get_names(self) if not n.startswith('do__')
+        ]
 
     def precmd(self, statement):
         """Hook method executed just before the command is executed by
         :meth:`~cmd2.Cmd.onecmd` and after adding it to history.
 
         :param statement: subclass of str which also contains the parsed input
         :return: a potentially modified version of the input Statement object
```

### Comparing `cliff-4.6.0/cliff/lister.py` & `cliff-4.7.0/cliff/lister.py`

 * *Files 8% similar despite different names*

```diff
@@ -79,48 +79,54 @@
             help=('sort the column(s) in descending order'),
         )
         return parser
 
     def produce_output(self, parsed_args, column_names, data):
         if parsed_args.sort_columns and self.need_sort_by_cliff:
             indexes = [
-                column_names.index(c) for c in parsed_args.sort_columns
+                column_names.index(c)
+                for c in parsed_args.sort_columns
                 if c in column_names
             ]
             reverse = parsed_args.sort_direction == 'desc'
             for index in indexes[::-1]:
                 try:
                     # We need to handle unset values (i.e. None) so we sort on
                     # multiple conditions: the first comparing the results of
                     # an 'is None' type check and the second comparing the
                     # actual value. The second condition will only be checked
                     # if the first returns True, which only happens if the
                     # returns from the 'is None' check on the two values are
                     # the same, i.e. both None or both not-None
                     data = sorted(
-                        data, key=lambda k: (k[index] is None, k[index]),
+                        data,
+                        key=lambda k: (k[index] is None, k[index]),
                         reverse=reverse,
                     )
                 except TypeError:
                     # Simply log and then ignore this; sorting is best effort
                     self.log.warning(
                         "Could not sort on field '%s'; unsortable types",
                         parsed_args.sort_columns[index],
                     )
 
         columns_to_include, selector = self._generate_columns_and_selector(
-            parsed_args, column_names,
+            parsed_args,
+            column_names,
         )
         if selector:
             # Generator expression to only return the parts of a row
             # of data that the user has expressed interest in
             # seeing. We have to convert the compress() output to a
             # list so the table formatter can ask for its length.
             data = (
                 list(self._compress_iterable(row, selector)) for row in data
             )
 
         self.formatter.emit_list(
-            columns_to_include, data, self.app.stdout, parsed_args,
+            columns_to_include,
+            data,
+            self.app.stdout,
+            parsed_args,
         )
 
         return 0
```

### Comparing `cliff-4.6.0/cliff/show.py` & `cliff-4.7.0/cliff/show.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,16 +14,15 @@
 """
 import abc
 
 from . import display
 
 
 class ShowOne(display.DisplayCommandBase, metaclass=abc.ABCMeta):
-    """Command base class for displaying data about a single object.
-    """
+    """Command base class for displaying data about a single object."""
 
     @property
     def formatter_namespace(self):
         return 'cliff.formatter.show'
 
     @property
     def formatter_default(self):
@@ -33,21 +32,21 @@
     def take_action(self, parsed_args):
         """Return a two-part tuple with a tuple of column names
         and a tuple of values.
         """
 
     def produce_output(self, parsed_args, column_names, data):
         (columns_to_include, selector) = self._generate_columns_and_selector(
-            parsed_args, column_names)
+            parsed_args, column_names
+        )
         if selector:
             data = list(self._compress_iterable(data, selector))
-        self.formatter.emit_one(columns_to_include,
-                                data,
-                                self.app.stdout,
-                                parsed_args)
+        self.formatter.emit_one(
+            columns_to_include, data, self.app.stdout, parsed_args
+        )
         return 0
 
     def dict2columns(self, data):
         """Implement the common task of converting a dict-based object
         to the two-column output that ShowOne expects.
         """
         if not data:
```

### Comparing `cliff-4.6.0/cliff/sphinxext.py` & `cliff-4.7.0/cliff/sphinxext.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,15 +42,16 @@
 def _format_description(parser):
     """Get parser description.
 
     We parse this as reStructuredText, allowing users to embed rich
     information in their help messages if they so choose.
     """
     for line in statemachine.string2lines(
-            parser.description, tab_width=4, convert_whitespace=True):
+        parser.description, tab_width=4, convert_whitespace=True
+    ):
         yield line
 
 
 def _format_usage(parser):
     """Get usage without a prefix."""
     fmt = argparse.HelpFormatter(parser.prog)
 
@@ -60,20 +61,23 @@
 
     # hacked variant of the regex used by the actual argparse module. Unlike
     # that version, this one attempts to group long and short opts with their
     # optional arguments ensuring that, for example, '--format <FORMAT>'
     # becomes ['--format <FORMAT>'] and not ['--format', '<FORMAT>'].
     # Yes, they really do use regexes to break apart and rewrap their help
     # string. Don't ask me why.
-    part_regexp = re.compile(r"""
+    part_regexp = re.compile(
+        r"""
         \(.*?\)+ |
         \[.*?\]+ |
         (?:(?:-\w|--\w+(?:-\w+)*)(?:\s+<?\w[\w-]*>?)?) |
         \S+
-    """, re.VERBOSE)
+    """,
+        re.VERBOSE,
+    )
 
     opt_usage = fmt._format_actions_usage(optionals, groups)
     pos_usage = fmt._format_actions_usage(positionals, groups)
 
     opt_parts = part_regexp.findall(opt_usage)
     pos_parts = part_regexp.findall(pos_usage)
     parts = opt_parts + pos_parts
@@ -87,55 +91,60 @@
 def _format_epilog(parser):
     """Get parser epilog.
 
     We parse this as reStructuredText, allowing users to embed rich
     information in their help messages if they so choose.
     """
     for line in statemachine.string2lines(
-            parser.epilog, tab_width=4, convert_whitespace=True):
+        parser.epilog, tab_width=4, convert_whitespace=True
+    ):
         yield line
 
 
 def _format_positional_action(action):
     """Format a positional action."""
     if action.help == argparse.SUPPRESS:
         return
 
     # NOTE(stephenfin): We strip all types of brackets from 'metavar' because
     # the 'option' directive dictates that only option argument names should be
     # surrounded by angle brackets
     yield '.. option:: {}'.format(
-        (action.metavar or action.dest).strip('<>[]() '))
+        (action.metavar or action.dest).strip('<>[]() ')
+    )
     if action.help:
         yield ''
         for line in statemachine.string2lines(
-                action.help, tab_width=4, convert_whitespace=True):
+            action.help, tab_width=4, convert_whitespace=True
+        ):
             yield _indent(line)
 
 
 def _format_optional_action(action):
     """Format an optional action."""
     if action.help == argparse.SUPPRESS:
         return
 
     if action.nargs == 0:
         yield '.. option:: {}'.format(', '.join(action.option_strings))
     else:
         # TODO(stephenfin): At some point, we may wish to provide more
         # information about the options themselves, for example, if nargs is
         # specified
-        option_strings = [' '.join(
-            [x, action.metavar or '<{}>'.format(action.dest.upper())])
-            for x in action.option_strings]
+        option_strings = [
+            ' '.join([x, action.metavar or '<{}>'.format(action.dest.upper())])
+            for x in action.option_strings
+        ]
         yield '.. option:: {}'.format(', '.join(option_strings))
 
     if action.help:
         yield ''
         for line in statemachine.string2lines(
-                action.help, tab_width=4, convert_whitespace=True):
+            action.help, tab_width=4, convert_whitespace=True
+        ):
             yield _indent(line)
 
 
 def _format_parser(parser):
     """Format the output of an argparse 'ArgumentParser' object.
 
     Given the following parser::
@@ -216,16 +225,17 @@
         'ignored': directives.unchanged,
         'application': directives.unchanged,
     }
 
     def _get_ignored_opts(self):
         global_ignored = self.env.config.autoprogram_cliff_ignored
         local_ignored = self.options.get('ignored', '')
-        local_ignored = [x.strip() for x in local_ignored.split(',')
-                         if x.strip()]
+        local_ignored = [
+            x.strip() for x in local_ignored.split(',') if x.strip()
+        ]
         return list(set(global_ignored + local_ignored))
 
     def _drop_ignored_options(self, parser, ignored_opts):
         for action in list(parser._actions):
             for option_string in action.option_strings:
                 if option_string in ignored_opts:
                     del parser._actions[parser._actions.index(action)]
@@ -252,40 +262,47 @@
 
     def _load_command(self, manager, command_name):
         """Load a command using an instance of a `CommandManager`."""
         try:
             # find_command expects the value of argv so split to emulate that
             return manager.find_command(command_name.split())[0]
         except ValueError:
-            raise self.error('"{}" is not a valid command in the "{}" '
-                             'namespace'.format(
-                                 command_name, manager.namespace))
+            raise self.error(
+                '"{}" is not a valid command in the "{}" '
+                'namespace'.format(command_name, manager.namespace)
+            )
 
     def _load_commands(self):
         # TODO(sfinucan): We should probably add this wildcarding functionality
         # to the CommandManager itself to allow things like "show me the
         # commands like 'foo *'"
         command_pattern = self.options.get('command')
         manager = commandmanager.CommandManager(self.arguments[0])
         if command_pattern:
-            commands = [x for x in manager.commands
-                        if fnmatch.fnmatch(x, command_pattern)]
+            commands = [
+                x
+                for x in manager.commands
+                if fnmatch.fnmatch(x, command_pattern)
+            ]
         else:
             commands = manager.commands.keys()
 
         if not commands:
             msg = 'No commands found in the "{}" namespace'
             if command_pattern:
                 msg += ' using the "{}" command name/pattern'
-            msg += ('. Are you sure this is correct and the application being '
-                    'documented is installed?')
+            msg += (
+                '. Are you sure this is correct and the application being '
+                'documented is installed?'
+            )
             raise self.warning(msg.format(self.arguments[0], command_pattern))
 
-        return dict((name, self._load_command(manager, name))
-                    for name in commands)
+        return dict(
+            (name, self._load_command(manager, name)) for name in commands
+        )
 
     def _generate_app_node(self, app, application_name):
         ignored_opts = self._get_ignored_opts()
 
         parser = app.parser
 
         self._drop_ignored_options(parser, ignored_opts)
@@ -299,16 +316,17 @@
 
         section = nodes.section()
         self.state.nested_parse(result, 0, section)
 
         # return [section.children]
         return section.children
 
-    def _generate_nodes_per_command(self, title, command_name, command_class,
-                                    ignored_opts):
+    def _generate_nodes_per_command(
+        self, title, command_name, command_class, ignored_opts
+    ):
         """Generate the relevant Sphinx nodes.
 
         This doesn't bother using raw docutils nodes as they simply don't offer
         the power of directives, like Sphinx's 'option' directive. Instead, we
         generate reStructuredText and parse this in a nested context (to obtain
         correct header levels). Refer to [1] for more information.
 
@@ -320,25 +338,27 @@
         :param prefix: Prefix to apply before command, if any
         :param ignored_opts: A list of options to exclude from output, if any
         :returns: A list of nested docutil nodes
         """
         command = command_class(None, None)
         if not getattr(command, 'app_dist_name', None):
             command.app_dist_name = (
-                self.env.config.autoprogram_cliff_app_dist_name)
+                self.env.config.autoprogram_cliff_app_dist_name
+            )
         parser = command.get_parser(command_name)
         ignored_opts = ignored_opts or []
 
         self._drop_ignored_options(parser, ignored_opts)
 
         section = nodes.section(
             '',
             nodes.title(text=title),
             ids=[nodes.make_id(title)],
-            names=[nodes.fully_normalize_name(title)])
+            names=[nodes.fully_normalize_name(title)],
+        )
 
         source_name = '<{}>'.format(command.__class__.__name__)
         result = statemachine.ViewList()
 
         for line in _format_parser(parser):
             result.append(line, source_name)
 
@@ -351,24 +371,29 @@
         output = []
         for command_name in sorted(commands):
             command_class = commands[command_name]
             title = command_name
             if application_name:
                 command_name = ' '.join([application_name, command_name])
 
-            output.extend(self._generate_nodes_per_command(
-                title, command_name, command_class, ignored_opts))
+            output.extend(
+                self._generate_nodes_per_command(
+                    title, command_name, command_class, ignored_opts
+                )
+            )
 
         return output
 
     def run(self):
         self.env = self.state.document.settings.env
 
-        application_name = (self.options.get('application')
-                            or self.env.config.autoprogram_cliff_application)
+        application_name = (
+            self.options.get('application')
+            or self.env.config.autoprogram_cliff_application
+        )
 
         app = self._load_app()
         if app:
             return self._generate_app_node(app, application_name)
 
         commands = self._load_commands()
         return self._generate_command_nodes(commands, application_name)
```

### Comparing `cliff-4.6.0/cliff/tests/base.py` & `cliff-4.7.0/cliff/tests/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 import testtools
 
 import fixtures
 
 
 class TestBase(testtools.TestCase):
-
     def setUp(self):
         super(TestBase, self).setUp()
         self._stdout_fixture = fixtures.StringStream('stdout')
         self.stdout = self.useFixture(self._stdout_fixture).stream
         self.useFixture(fixtures.MonkeyPatch('sys.stdout', self.stdout))
         self._stderr_fixture = fixtures.StringStream('stderr')
         self.stderr = self.useFixture(self._stderr_fixture).stream
```

### Comparing `cliff-4.6.0/cliff/tests/test__argparse.py` & `cliff-4.7.0/cliff/tests/test__argparse.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 
 import unittest
 
 from cliff import _argparse
 
 
 class TestArgparse(unittest.TestCase):
-
     def test_argument_parser(self):
         _argparse.ArgumentParser(conflict_handler='ignore')
 
     def test_argument_parser_add_group(self):
         parser = _argparse.ArgumentParser(conflict_handler='ignore')
         parser.add_argument_group()
```

### Comparing `cliff-4.6.0/cliff/tests/test_app.py` & `cliff-4.7.0/cliff/tests/test_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,40 +44,36 @@
     )
     err_command.return_value = err_command_inst
     cmd_mgr.add_command('error', err_command)
 
     # Register a command that is interrrupted
     interrupt_command = mock.Mock(name='interrupt_command', spec=c_cmd.Command)
     interrupt_command_inst = mock.Mock(spec=c_cmd.Command)
-    interrupt_command_inst.run = mock.Mock(
-        side_effect=KeyboardInterrupt
-    )
+    interrupt_command_inst.run = mock.Mock(side_effect=KeyboardInterrupt)
     interrupt_command.return_value = interrupt_command_inst
     cmd_mgr.add_command('interrupt', interrupt_command)
 
     # Register a command that is interrrupted by a broken pipe
     pipeclose_command = mock.Mock(name='pipeclose_command', spec=c_cmd.Command)
     pipeclose_command_inst = mock.Mock(spec=c_cmd.Command)
-    pipeclose_command_inst.run = mock.Mock(
-        side_effect=BrokenPipeError
-    )
+    pipeclose_command_inst.run = mock.Mock(side_effect=BrokenPipeError)
     pipeclose_command.return_value = pipeclose_command_inst
     cmd_mgr.add_command('pipe-close', pipeclose_command)
 
-    app = application.App('testing interactive mode',
-                          '1',
-                          cmd_mgr,
-                          stderr=mock.Mock(),  # suppress warning messages
-                          **kwargs
-                          )
+    app = application.App(
+        'testing interactive mode',
+        '1',
+        cmd_mgr,
+        stderr=mock.Mock(),  # suppress warning messages
+        **kwargs
+    )
     return app, command
 
 
 class TestInteractiveMode(base.TestBase):
-
     def test_no_args_triggers_interactive_mode(self):
         app, command = make_app()
         app.interact = mock.MagicMock(name='inspect')
         app.run([])
         app.interact.assert_called_once_with()
 
     def test_interactive_mode_cmdloop(self):
@@ -106,15 +102,14 @@
         self.assertIsNotNone(app.interpreter)
         cmdloop = app.interactive_app_factory.return_value.cmdloop
         cmdloop.assert_called_once_with()
         self.assertNotEqual(ret, 0)
 
 
 class TestInitAndCleanup(base.TestBase):
-
     def test_initialize_app(self):
         app, command = make_app()
         app.initialize_app = mock.MagicMock(name='initialize_app')
         app.run(['mock'])
         app.initialize_app.assert_called_once_with(['mock'])
 
     def test_prepare_to_run_command(self):
@@ -262,29 +257,30 @@
 
         self.assertTrue(app.clean_up.called)
         call_args = app.clean_up.call_args_list[0]
         self.assertEqual(mock.call(mock.ANY, 0, None), call_args)
 
 
 class TestOptionParser(base.TestBase):
-
     def test_conflicting_option_should_throw(self):
         class MyApp(application.App):
             def __init__(self):
                 super(MyApp, self).__init__(
                     description='testing',
                     version='0.1',
                     command_manager=commandmanager.CommandManager('tests'),
                 )
 
             def build_option_parser(self, description, version):
-                parser = super(MyApp, self).build_option_parser(description,
-                                                                version)
+                parser = super(MyApp, self).build_option_parser(
+                    description, version
+                )
                 parser.add_argument(
-                    '-h', '--help',
+                    '-h',
+                    '--help',
                     default=self,  # tricky
                     help="Show help message and exit.",
                 )
 
         self.assertRaises(
             argparse.ArgumentError,
             MyApp,
@@ -298,19 +294,19 @@
                     version='0.1',
                     command_manager=commandmanager.CommandManager('tests'),
                 )
 
             def build_option_parser(self, description, version):
                 argparse_kwargs = {'conflict_handler': 'resolve'}
                 parser = super(MyApp, self).build_option_parser(
-                    description,
-                    version,
-                    argparse_kwargs=argparse_kwargs)
+                    description, version, argparse_kwargs=argparse_kwargs
+                )
                 parser.add_argument(
-                    '-h', '--help',
+                    '-h',
+                    '--help',
                     default=self,  # tricky
                     help="Show help message and exit.",
                 )
 
         MyApp()
 
     def test_option_parser_abbrev_issue(self):
@@ -335,31 +331,32 @@
                     command_manager=MyCommandManager(None),
                 )
 
             def build_option_parser(self, description, version):
                 parser = super(MyApp, self).build_option_parser(
                     description,
                     version,
-                    argparse_kwargs={'allow_abbrev': False})
+                    argparse_kwargs={'allow_abbrev': False},
+                )
                 parser.add_argument('--endpoint')
                 return parser
 
         app = MyApp()
         # NOTE(jd) --debug is necessary so assert in take_action()
         # raises correctly here
         app.run(['--debug', 'mycommand', '--end', '123'])
 
 
 class TestHelpHandling(base.TestBase):
-
     def _test_help(self, deferred_help):
         app, _ = make_app(deferred_help=deferred_help)
         with mock.patch.object(app, 'initialize_app') as init:
-            with mock.patch('cliff.help.HelpAction.__call__',
-                            side_effect=SystemExit(0)) as helper:
+            with mock.patch(
+                'cliff.help.HelpAction.__call__', side_effect=SystemExit(0)
+            ) as helper:
                 self.assertRaises(
                     SystemExit,
                     app.run,
                     ['--help'],
                 )
                 self.assertTrue(helper.called)
             self.assertEqual(deferred_help, init.called)
@@ -368,29 +365,31 @@
         self._test_help(False)
 
     def test_deferred_help(self):
         self._test_help(True)
 
     def _test_interrupted_help(self, deferred_help):
         app, _ = make_app(deferred_help=deferred_help)
-        with mock.patch('cliff.help.HelpAction.__call__',
-                        side_effect=KeyboardInterrupt):
+        with mock.patch(
+            'cliff.help.HelpAction.__call__', side_effect=KeyboardInterrupt
+        ):
             result = app.run(['--help'])
             self.assertEqual(result, 130)
 
     def test_interrupted_help(self):
         self._test_interrupted_help(False)
 
     def test_interrupted_deferred_help(self):
         self._test_interrupted_help(True)
 
     def _test_pipeclose_help(self, deferred_help):
         app, _ = make_app(deferred_help=deferred_help)
-        with mock.patch('cliff.help.HelpAction.__call__',
-                        side_effect=BrokenPipeError):
+        with mock.patch(
+            'cliff.help.HelpAction.__call__', side_effect=BrokenPipeError
+        ):
             app.run(['--help'])
 
     def test_pipeclose_help(self):
         self._test_pipeclose_help(False)
 
     def test_pipeclose_deferred_help(self):
         self._test_pipeclose_help(True)
@@ -411,40 +410,42 @@
         with mock.patch.object(app, 'run_subcommand') as helper:
             app.run(['show', 'files', '--help'])
 
         helper.assert_called_once_with(['help', 'show', 'files'])
 
 
 class TestCommandLookup(base.TestBase):
-
     def test_unknown_cmd(self):
         app, command = make_app()
         self.assertEqual(2, app.run(['hell']))
 
     def test_unknown_cmd_debug(self):
         app, command = make_app()
         try:
             self.assertEqual(2, app.run(['--debug', 'hell']))
         except ValueError as err:
             self.assertIn("['hell']", str(err))
 
     def test_list_matching_commands(self):
         stdout = io.StringIO()
-        app = application.App('testing', '1',
-                              test_utils.TestCommandManager(
-                                  test_utils.TEST_NAMESPACE),
-                              stdout=stdout)
+        app = application.App(
+            'testing',
+            '1',
+            test_utils.TestCommandManager(test_utils.TEST_NAMESPACE),
+            stdout=stdout,
+        )
         app.NAME = 'test'
         try:
             self.assertEqual(2, app.run(['t']))
         except SystemExit:
             pass
         output = stdout.getvalue()
-        self.assertIn("test: 't' is not a test command. See 'test --help'.",
-                      output)
+        self.assertIn(
+            "test: 't' is not a test command. See 'test --help'.", output
+        )
         self.assertIn('Did you mean one of these?', output)
         self.assertIn('three word command\n  two words\n', output)
 
     def test_fuzzy_no_commands(self):
         cmd_mgr = commandmanager.CommandManager('cliff.fuzzy')
         app = application.App('test', '1.0', cmd_mgr)
         cmd_mgr.commands = {}
@@ -480,15 +481,14 @@
         app = application.App('test', '1.0', cmd_mgr)
         cmd_mgr.add_command('user', test_utils.TestCommand)
         matches = app.get_fuzzy_matches('uesr')
         self.assertEqual(['user'], matches)
 
 
 class TestVerboseMode(base.TestBase):
-
     def test_verbose(self):
         app, command = make_app()
         app.clean_up = mock.MagicMock(name='clean_up')
         app.run(['--verbose', 'mock'])
         app.clean_up.assert_called_once_with(command.return_value, 0, None)
         app.clean_up.reset_mock()
         app.run(['--quiet', 'mock'])
@@ -497,37 +497,34 @@
             SystemExit,
             app.run,
             ['--verbose', '--quiet', 'mock'],
         )
 
 
 class TestIO(base.TestBase):
-
     def test_io_streams(self):
         cmd_mgr = commandmanager.CommandManager('cliff.tests')
         io = mock.Mock()
 
         app = application.App('no io streams', 1, cmd_mgr)
         self.assertIs(sys.stdin, app.stdin)
         self.assertIs(sys.stdout, app.stdout)
         self.assertIs(sys.stderr, app.stderr)
 
         app = application.App('with stdin io stream', 1, cmd_mgr, stdin=io)
         self.assertIs(io, app.stdin)
         self.assertIs(sys.stdout, app.stdout)
         self.assertIs(sys.stderr, app.stderr)
 
-        app = application.App('with stdout io stream', 1, cmd_mgr,
-                              stdout=io)
+        app = application.App('with stdout io stream', 1, cmd_mgr, stdout=io)
         self.assertIs(sys.stdin, app.stdin)
         self.assertIs(io, app.stdout)
         self.assertIs(sys.stderr, app.stderr)
 
-        app = application.App('with stderr io stream', 1, cmd_mgr,
-                              stderr=io)
+        app = application.App('with stderr io stream', 1, cmd_mgr, stderr=io)
         self.assertIs(sys.stdin, app.stdin)
         self.assertIs(sys.stdout, app.stdout)
         self.assertIs(io, app.stderr)
 
     def test_writer_encoding(self):
         # The word "test" with the e replaced by
         # Unicode latin small letter e with acute,
```

### Comparing `cliff-4.6.0/cliff/tests/test_columns.py` & `cliff-4.7.0/cliff/tests/test_columns.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,21 +12,19 @@
 
 import unittest
 
 from cliff import columns
 
 
 class FauxColumn(columns.FormattableColumn):
-
     def human_readable(self):
         return 'I made this string myself: {}'.format(self._value)
 
 
 class TestColumns(unittest.TestCase):
-
     def test_machine_readable(self):
         c = FauxColumn(['list', 'of', 'values'])
         self.assertEqual(['list', 'of', 'values'], c.machine_readable())
 
     def test_human_readable(self):
         c = FauxColumn(['list', 'of', 'values'])
         self.assertEqual(
```

### Comparing `cliff-4.6.0/cliff/tests/test_command.py` & `cliff-4.7.0/cliff/tests/test_command.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,63 +14,59 @@
 import functools
 
 from cliff import command
 from cliff.tests import base
 
 
 class TestCommand(command.Command):
-    """Description of command.
-    """
+    """Description of command."""
 
     def get_parser(self, prog_name):
         parser = super(TestCommand, self).get_parser(prog_name)
         parser.add_argument(
             'long_help_argument',
             help="Create a NIC on the server.\n"
-                 "Specify option multiple times to create multiple NICs. "
-                 "Either net-id or port-id must be provided, but not both.\n"
-                 "net-id: attach NIC to network with this UUID\n"
-                 "port-id: attach NIC to port with this UUID\n"
-                 "v4-fixed-ip: IPv4 fixed address for NIC (optional)\n"
-                 "v6-fixed-ip: IPv6 fixed address for NIC (optional)\n"
-                 "none: (v2.37+) no network is attached\n"
-                 "auto: (v2.37+) the compute service will automatically "
-                 "allocate a network.\n"
-                 "Specifying a --nic of auto or none "
-                 "cannot be used with any other --nic value.",
+            "Specify option multiple times to create multiple NICs. "
+            "Either net-id or port-id must be provided, but not both.\n"
+            "net-id: attach NIC to network with this UUID\n"
+            "port-id: attach NIC to port with this UUID\n"
+            "v4-fixed-ip: IPv4 fixed address for NIC (optional)\n"
+            "v6-fixed-ip: IPv6 fixed address for NIC (optional)\n"
+            "none: (v2.37+) no network is attached\n"
+            "auto: (v2.37+) the compute service will automatically "
+            "allocate a network.\n"
+            "Specifying a --nic of auto or none "
+            "cannot be used with any other --nic value.",
         )
         parser.add_argument(
             'regular_help_argument',
-            help="The quick brown fox jumps "
-                 "over the lazy dog.",
+            help="The quick brown fox jumps " "over the lazy dog.",
         )
         parser.add_argument(
             '-z',
             dest='zippy',
             default='zippy-default',
             help='defined in TestCommand and used in TestArgumentParser',
         )
         return parser
 
     def take_action(self, parsed_args):
         return 42
 
 
 class TestCommandNoDocstring(command.Command):
-
     def take_action(self, parsed_args):
         return 42
 
 
 class TestDescription(base.TestBase):
-
     def test_get_description_docstring(self):
         cmd = TestCommand(None, None)
         desc = cmd.get_description()
-        assert desc == "Description of command.\n    "
+        assert desc == "Description of command."
 
     def test_get_description_attribute(self):
         cmd = TestCommand(None, None)
         # Artificially inject a value for _description to verify that it
         # overrides the docstring.
         cmd._description = 'this is not the default'
         desc = cmd.get_description()
@@ -79,15 +75,14 @@
     def test_get_description_default(self):
         cmd = TestCommandNoDocstring(None, None)
         desc = cmd.get_description()
         assert desc == ''
 
 
 class TestBasicValues(base.TestBase):
-
     def test_get_parser(self):
         cmd = TestCommand(None, None)
         parser = cmd.get_parser('NAME')
         assert parser.prog == 'NAME'
 
     def test_get_name(self):
         cmd = TestCommand(None, None, cmd_name='object action')
@@ -114,15 +109,14 @@
                         any other --nic value.
   regular_help_argument
                         The quick brown fox jumps over the lazy dog.
 """
 
 
 class TestHelp(base.TestBase):
-
     def test_smart_help_formatter(self):
         cmd = TestCommand(None, None)
         parser = cmd.get_parser('NAME')
         # Set up the formatter to always use a width=80 so that the
         # terminal width of the developer's system does not cause the
         # test to fail. Trying to mock os.environ failed, but there is
         # an arg to HelpFormatter to set the width
@@ -134,15 +128,14 @@
             parser.formatter_class,
             width=78,
         )
         self.assertIn(expected_help_message, parser.format_help())
 
 
 class TestArgumentParser(base.TestBase):
-
     def test_option_name_collision(self):
         cmd = TestCommand(None, None)
         parser = cmd.get_parser('NAME')
         # We should have an exception registering an option with a
         # name that already exists because we configure the argument
         # parser to ignore conflicts but this option has no other name
         # to be used.
@@ -161,15 +154,16 @@
         # --zero even if the -z is ignored.
         parser.add_argument('-z', '--zero')
 
     def test_resolve_option_with_name_collision(self):
         cmd = TestCommand(None, None)
         parser = cmd.get_parser('NAME')
         parser.add_argument(
-            '-z', '--zero',
+            '-z',
+            '--zero',
             dest='zero',
             default='zero-default',
         )
         args = parser.parse_args(['-z', 'foo', 'a', 'b'])
         self.assertEqual(args.zippy, 'foo')
         self.assertEqual(args.zero, 'zero-default')
 
@@ -179,35 +173,38 @@
         parser = cmd.get_parser('NAME')
         self.assertEqual(parser.conflict_handler, 'resolve')
 
     def test_raise_conflict_argument_error(self):
         cmd = TestCommand(None, None)
         parser = cmd.get_parser('NAME')
         parser.add_argument(
-            '-f', '--foo',
+            '-f',
+            '--foo',
             dest='foo',
             default='foo',
         )
         self.assertRaises(
             argparse.ArgumentError,
             parser.add_argument,
             '-f',
         )
 
     def test_resolve_conflict_argument(self):
         cmd = TestCommand(None, None)
         cmd.conflict_handler = 'resolve'
         parser = cmd.get_parser('NAME')
         parser.add_argument(
-            '-f', '--foo',
+            '-f',
+            '--foo',
             dest='foo',
             default='foo',
         )
         parser.add_argument(
-            '-f', '--foo',
+            '-f',
+            '--foo',
             dest='foo',
             default='bar',
         )
         args = parser.parse_args(['a', 'b'])
         self.assertEqual(args.foo, 'bar')
 
     def test_wrong_conflict_handler(self):
```

### Comparing `cliff-4.6.0/cliff/tests/test_command_hooks.py` & `cliff-4.7.0/cliff/tests/test_command_hooks.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,53 +37,50 @@
     err_command_inst = mock.Mock(spec=command.Command)
     err_command_inst.run = mock.Mock(
         side_effect=RuntimeError('test exception')
     )
     err_command.return_value = err_command_inst
     cmd_mgr.add_command('error', err_command)
 
-    app = application.App('testing command hooks',
-                          '1',
-                          cmd_mgr,
-                          stderr=mock.Mock(),  # suppress warning messages
-                          **kwargs
-                          )
+    app = application.App(
+        'testing command hooks',
+        '1',
+        cmd_mgr,
+        stderr=mock.Mock(),  # suppress warning messages
+        **kwargs
+    )
     return app
 
 
 class TestCommand(command.Command):
-    """Description of command.
-    """
+    """Description of command."""
 
     def get_parser(self, prog_name):
         parser = super(TestCommand, self).get_parser(prog_name)
         return parser
 
     def take_action(self, parsed_args):
         return 42
 
 
 class TestShowCommand(show.ShowOne):
-    """Description of command.
-    """
+    """Description of command."""
 
     def take_action(self, parsed_args):
         return (('Name',), ('value',))
 
 
 class TestListerCommand(lister.Lister):
-    """Description of command.
-    """
+    """Description of command."""
 
     def take_action(self, parsed_args):
         return (('Name',), [('value',)])
 
 
 class TestHook(hooks.CommandHook):
-
     _before_called = False
     _after_called = False
 
     def get_parser(self, parser):
         parser.add_argument('--added-by-hook')
         return parser
 
@@ -94,15 +91,14 @@
         self._before_called = True
 
     def after(self, parsed_args, return_code):
         self._after_called = True
 
 
 class TestChangeHook(hooks.CommandHook):
-
     _before_called = False
     _after_called = False
 
     def get_parser(self, parser):
         parser.add_argument('--added-by-hook')
         return parser
 
@@ -117,15 +113,14 @@
 
     def after(self, parsed_args, return_code):
         self._after_called = True
         return 24
 
 
 class TestDisplayChangeHook(hooks.CommandHook):
-
     _before_called = False
     _after_called = False
 
     def get_parser(self, parser):
         parser.add_argument('--added-by-hook')
         return parser
 
@@ -140,15 +135,14 @@
 
     def after(self, parsed_args, return_code):
         self._after_called = True
         return (('Name',), ('othervalue',))
 
 
 class TestListerChangeHook(hooks.CommandHook):
-
     _before_called = False
     _after_called = False
 
     def get_parser(self, parser):
         parser.add_argument('--added-by-hook')
         return parser
 
@@ -163,15 +157,14 @@
 
     def after(self, parsed_args, return_code):
         self._after_called = True
         return (('Name',), [('othervalue',)])
 
 
 class TestCommandLoadHooks(base.TestBase):
-
     def test_no_app_or_name(self):
         cmd = TestCommand(None, None)
         self.assertEqual([], cmd._hooks)
 
     @mock.patch('stevedore.extension.ExtensionManager')
     def test_app_and_name(self, em):
         app = make_app()
@@ -179,26 +172,21 @@
         print(em.mock_calls[0])
         name, args, kwargs = em.mock_calls[0]
         print(kwargs)
         self.assertEqual('cliff.tests.test', kwargs['namespace'])
 
 
 class TestHooks(base.TestBase):
-
     def setUp(self):
         super(TestHooks, self).setUp()
         self.app = make_app()
         self.cmd = TestCommand(self.app, None, cmd_name='test')
         self.hook = TestHook(self.cmd)
         self.mgr = extension.ExtensionManager.make_test_instance(
-            [extension.Extension(
-                'parser-hook',
-                None,
-                None,
-                self.hook)],
+            [extension.Extension('parser-hook', None, None, self.hook)],
         )
         # Replace the auto-loaded hooks with our explicitly created
         # manager.
         self.cmd._hooks = self.mgr
 
     def test_get_parser(self):
         parser = self.cmd.get_parser('test')
@@ -218,26 +206,21 @@
         self.assertFalse(self.hook._after_called)
         result = self.cmd.run(None)
         self.assertTrue(self.hook._after_called)
         self.assertEqual(result, 42)
 
 
 class TestChangeHooks(base.TestBase):
-
     def setUp(self):
         super(TestChangeHooks, self).setUp()
         self.app = make_app()
         self.cmd = TestCommand(self.app, None, cmd_name='test')
         self.hook = TestChangeHook(self.cmd)
         self.mgr = extension.ExtensionManager.make_test_instance(
-            [extension.Extension(
-                'parser-hook',
-                None,
-                None,
-                self.hook)],
+            [extension.Extension('parser-hook', None, None, self.hook)],
         )
         # Replace the auto-loaded hooks with our explicitly created
         # manager.
         self.cmd._hooks = self.mgr
 
     def test_get_parser(self):
         parser = self.cmd.get_parser('test')
@@ -263,26 +246,21 @@
         results = parser.parse_args(['--added-by-hook', 'value'])
         result = self.cmd.run(results)
         self.assertTrue(self.hook._after_called)
         self.assertEqual(result, 24)
 
 
 class TestShowOneHooks(base.TestBase):
-
     def setUp(self):
         super(TestShowOneHooks, self).setUp()
         self.app = make_app()
         self.cmd = TestShowCommand(self.app, None, cmd_name='test')
         self.hook = TestHook(self.cmd)
         self.mgr = extension.ExtensionManager.make_test_instance(
-            [extension.Extension(
-                'parser-hook',
-                None,
-                None,
-                self.hook)],
+            [extension.Extension('parser-hook', None, None, self.hook)],
         )
         # Replace the auto-loaded hooks with our explicitly created
         # manager.
         self.cmd._hooks = self.mgr
 
     def test_get_parser(self):
         parser = self.cmd.get_parser('test')
@@ -305,26 +283,21 @@
         parser = self.cmd.get_parser('test')
         results = parser.parse_args(['--added-by-hook', 'value'])
         self.cmd.run(results)
         self.assertTrue(self.hook._after_called)
 
 
 class TestShowOneChangeHooks(base.TestBase):
-
     def setUp(self):
         super(TestShowOneChangeHooks, self).setUp()
         self.app = make_app()
         self.cmd = TestShowCommand(self.app, None, cmd_name='test')
         self.hook = TestDisplayChangeHook(self.cmd)
         self.mgr = extension.ExtensionManager.make_test_instance(
-            [extension.Extension(
-                'parser-hook',
-                None,
-                None,
-                self.hook)],
+            [extension.Extension('parser-hook', None, None, self.hook)],
         )
         # Replace the auto-loaded hooks with our explicitly created
         # manager.
         self.cmd._hooks = self.mgr
 
     def test_get_parser(self):
         parser = self.cmd.get_parser('test')
@@ -350,26 +323,21 @@
         results = parser.parse_args(['--added-by-hook', 'value'])
         result = self.cmd.run(results)
         self.assertTrue(self.hook._after_called)
         self.assertEqual(result, 0)
 
 
 class TestListerHooks(base.TestBase):
-
     def setUp(self):
         super(TestListerHooks, self).setUp()
         self.app = make_app()
         self.cmd = TestListerCommand(self.app, None, cmd_name='test')
         self.hook = TestHook(self.cmd)
         self.mgr = extension.ExtensionManager.make_test_instance(
-            [extension.Extension(
-                'parser-hook',
-                None,
-                None,
-                self.hook)],
+            [extension.Extension('parser-hook', None, None, self.hook)],
         )
         # Replace the auto-loaded hooks with our explicitly created
         # manager.
         self.cmd._hooks = self.mgr
 
     def test_get_parser(self):
         parser = self.cmd.get_parser('test')
@@ -392,26 +360,21 @@
         parser = self.cmd.get_parser('test')
         results = parser.parse_args(['--added-by-hook', 'value'])
         self.cmd.run(results)
         self.assertTrue(self.hook._after_called)
 
 
 class TestListerChangeHooks(base.TestBase):
-
     def setUp(self):
         super(TestListerChangeHooks, self).setUp()
         self.app = make_app()
         self.cmd = TestListerCommand(self.app, None, cmd_name='test')
         self.hook = TestListerChangeHook(self.cmd)
         self.mgr = extension.ExtensionManager.make_test_instance(
-            [extension.Extension(
-                'parser-hook',
-                None,
-                None,
-                self.hook)],
+            [extension.Extension('parser-hook', None, None, self.hook)],
         )
         # Replace the auto-loaded hooks with our explicitly created
         # manager.
         self.cmd._hooks = self.mgr
 
     def test_get_parser(self):
         parser = self.cmd.get_parser('test')
```

### Comparing `cliff-4.6.0/cliff/tests/test_commandmanager.py` & `cliff-4.7.0/cliff/tests/test_commandmanager.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 from cliff.tests import utils
 
 
 load_tests = testscenarios.load_tests_apply_scenarios
 
 
 class TestLookupAndFind(base.TestBase):
-
     scenarios = [
         ('one-word', {'argv': ['one']}),
         ('two-words', {'argv': ['two', 'words']}),
         ('three-words', {'argv': ['three', 'word', 'command']}),
     ]
 
     def test(self):
@@ -35,30 +34,28 @@
         cmd, name, remaining = mgr.find_command(self.argv)
         self.assertTrue(cmd)
         self.assertEqual(' '.join(self.argv), name)
         self.assertFalse(remaining)
 
 
 class TestLookupWithRemainder(base.TestBase):
-
     scenarios = [
         ('one', {'argv': ['one', '--opt']}),
         ('two', {'argv': ['two', 'words', '--opt']}),
         ('three', {'argv': ['three', 'word', 'command', '--opt']}),
     ]
 
     def test(self):
         mgr = utils.TestCommandManager(utils.TEST_NAMESPACE)
         cmd, name, remaining = mgr.find_command(self.argv)
         self.assertTrue(cmd)
         self.assertEqual(['--opt'], remaining)
 
 
 class TestFindInvalidCommand(base.TestBase):
-
     scenarios = [
         ('no-such-command', {'argv': ['a', '-b']}),
         ('no-command-given', {'argv': ['-b']}),
     ]
 
     def test(self):
         mgr = utils.TestCommandManager(utils.TEST_NAMESPACE)
@@ -69,27 +66,25 @@
             self.assertIn(self.argv[0], str(err))
             self.assertIn('-b', str(err))
         else:
             self.fail('expected a failure')
 
 
 class TestFindUnknownCommand(base.TestBase):
-
     def test(self):
         mgr = utils.TestCommandManager(utils.TEST_NAMESPACE)
         try:
             mgr.find_command(['a', 'b'])
         except ValueError as err:
             self.assertIn("['a', 'b']", str(err))
         else:
             self.fail('expected a failure')
 
 
 class TestDynamicCommands(base.TestBase):
-
     def test_add(self):
         mgr = utils.TestCommandManager(utils.TEST_NAMESPACE)
         mock_cmd = mock.Mock()
         mgr.add_command('mock', mock_cmd)
         found_cmd, name, args = mgr.find_command(['mock'])
         self.assertIs(mock_cmd, found_cmd)
 
@@ -108,67 +103,67 @@
         self.assertIs(
             foo,
             mgr.find_command(['foo', 'arg0'])[0],
         )
 
 
 class TestLoad(base.TestBase):
-
     def test_load_commands(self):
         testcmd = mock.Mock(name='testcmd')
         testcmd.name.replace.return_value = 'test'
         mock_get_group_all = mock.Mock(return_value=[testcmd])
-        with mock.patch('stevedore.ExtensionManager',
-                        mock_get_group_all) as mock_manager:
+        with mock.patch(
+            'stevedore.ExtensionManager', mock_get_group_all
+        ) as mock_manager:
             mgr = commandmanager.CommandManager('test')
             mock_manager.assert_called_once_with('test')
             names = [n for n, v in mgr]
             self.assertEqual(['test'], names)
 
     def test_load_commands_keep_underscores(self):
         testcmd = mock.Mock()
         testcmd.name = 'test_cmd'
         mock_get_group_all = mock.Mock(return_value=[testcmd])
-        with mock.patch('stevedore.ExtensionManager',
-                        mock_get_group_all) as mock_manager:
+        with mock.patch(
+            'stevedore.ExtensionManager', mock_get_group_all
+        ) as mock_manager:
             mgr = commandmanager.CommandManager(
                 'test',
                 convert_underscores=False,
             )
             mock_manager.assert_called_once_with('test')
             names = [n for n, v in mgr]
             self.assertEqual(['test_cmd'], names)
 
     def test_load_commands_replace_underscores(self):
         testcmd = mock.Mock()
         testcmd.name = 'test_cmd'
         mock_get_group_all = mock.Mock(return_value=[testcmd])
-        with mock.patch('stevedore.ExtensionManager',
-                        mock_get_group_all) as mock_manager:
+        with mock.patch(
+            'stevedore.ExtensionManager', mock_get_group_all
+        ) as mock_manager:
             mgr = commandmanager.CommandManager(
                 'test',
                 convert_underscores=True,
             )
             mock_manager.assert_called_once_with('test')
             names = [n for n, v in mgr]
             self.assertEqual(['test cmd'], names)
 
 
 class FauxCommand(command.Command):
-
     def take_action(self, parsed_args):
         return 0
 
 
 class FauxCommand2(FauxCommand):
     pass
 
 
 class TestLegacyCommand(base.TestBase):
-
     def test_find_legacy(self):
         mgr = utils.TestCommandManager(None)
         mgr.add_command('new name', FauxCommand)
         mgr.add_legacy_command('old name', 'new name')
         cmd, name, remaining = mgr.find_command(['old', 'name'])
         self.assertIs(cmd, FauxCommand)
         self.assertEqual(name, 'old name')
@@ -198,15 +193,14 @@
             ValueError,
             mgr.find_command,
             ['cmd2'],
         )
 
 
 class TestLookupAndFindPartialName(base.TestBase):
-
     scenarios = [
         ('one-word', {'argv': ['o']}),
         ('two-words', {'argv': ['t', 'w']}),
         ('three-words', {'argv': ['t', 'w', 'c']}),
     ]
 
     def test(self):
@@ -214,53 +208,69 @@
         cmd, name, remaining = mgr.find_command(self.argv)
         self.assertTrue(cmd)
         self.assertEqual(' '.join(self.argv), name)
         self.assertFalse(remaining)
 
 
 class TestGetByPartialName(base.TestBase):
-
     def setUp(self):
         super(TestGetByPartialName, self).setUp()
         self.commands = {
             'resource provider list': 1,
             'resource class list': 2,
             'server list': 3,
-            'service list': 4}
+            'service list': 4,
+        }
 
     def test_no_candidates(self):
         self.assertEqual(
-            [], commandmanager._get_commands_by_partial_name(
-                ['r', 'p'], self.commands))
+            [],
+            commandmanager._get_commands_by_partial_name(
+                ['r', 'p'], self.commands
+            ),
+        )
         self.assertEqual(
-            [], commandmanager._get_commands_by_partial_name(
-                ['r', 'p', 'c'], self.commands))
+            [],
+            commandmanager._get_commands_by_partial_name(
+                ['r', 'p', 'c'], self.commands
+            ),
+        )
 
     def test_multiple_candidates(self):
         self.assertEqual(
-            2, len(commandmanager._get_commands_by_partial_name(
-                ['se', 'li'], self.commands)))
+            2,
+            len(
+                commandmanager._get_commands_by_partial_name(
+                    ['se', 'li'], self.commands
+                )
+            ),
+        )
 
     def test_one_candidate(self):
         self.assertEqual(
             ['resource provider list'],
             commandmanager._get_commands_by_partial_name(
-                ['r', 'p', 'l'], self.commands))
+                ['r', 'p', 'l'], self.commands
+            ),
+        )
         self.assertEqual(
             ['resource provider list'],
             commandmanager._get_commands_by_partial_name(
-                ['resource', 'provider', 'list'], self.commands))
+                ['resource', 'provider', 'list'], self.commands
+            ),
+        )
         self.assertEqual(
             ['server list'],
             commandmanager._get_commands_by_partial_name(
-                ['serve', 'l'], self.commands))
+                ['serve', 'l'], self.commands
+            ),
+        )
 
 
 class FakeCommand(object):
-
     @classmethod
     def load(cls):
         return cls
 
     def __init__(self):
         return
 
@@ -282,15 +292,14 @@
         elif namespace == 'greek':
             self.commands['alpha'] = FAKE_CMD_ALPHA
             self.commands['beta'] = FAKE_CMD_BETA
             self.group_list.append(namespace)
 
 
 class TestCommandManagerGroups(base.TestBase):
-
     def test_add_command_group(self):
         mgr = FakeCommandManager('test')
 
         # Make sure add_command() still functions
         mock_cmd_one = mock.Mock()
         mgr.add_command('mock', mock_cmd_one)
         cmd_mock, name, args = mgr.find_command(['mock'])
```

### Comparing `cliff-4.6.0/cliff/tests/test_complete.py` & `cliff-4.7.0/cliff/tests/test_complete.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,46 +18,53 @@
 from cliff import app as application
 from cliff import commandmanager
 from cliff import complete
 from cliff.tests import base
 
 
 class TestCompletion(base.TestBase):
-
     def test_dictionary(self):
         sot = complete.CompleteDictionary()
-        sot.add_command("image delete".split(),
-                        [mock.Mock(option_strings=["1"])])
-        sot.add_command("image list".split(),
-                        [mock.Mock(option_strings=["2"])])
-        sot.add_command("image create".split(),
-                        [mock.Mock(option_strings=["3"])])
-        sot.add_command("volume type create".split(),
-                        [mock.Mock(option_strings=["4"])])
-        sot.add_command("volume type delete".split(),
-                        [mock.Mock(option_strings=["5"])])
+        sot.add_command(
+            "image delete".split(), [mock.Mock(option_strings=["1"])]
+        )
+        sot.add_command(
+            "image list".split(), [mock.Mock(option_strings=["2"])]
+        )
+        sot.add_command(
+            "image create".split(), [mock.Mock(option_strings=["3"])]
+        )
+        sot.add_command(
+            "volume type create".split(), [mock.Mock(option_strings=["4"])]
+        )
+        sot.add_command(
+            "volume type delete".split(), [mock.Mock(option_strings=["5"])]
+        )
         self.assertEqual("image volume", sot.get_commands())
         result = sot.get_data()
         self.assertEqual("image", result[0][0])
         self.assertEqual("create delete list", result[0][1])
         self.assertEqual("image_create", result[1][0])
         self.assertEqual("3", result[1][1])
         self.assertEqual("image_delete", result[2][0])
         self.assertEqual("1", result[2][1])
         self.assertEqual("image_list", result[3][0])
         self.assertEqual("2", result[3][1])
 
     def test_complete_dictionary_subcmd(self):
         sot = complete.CompleteDictionary()
-        sot.add_command("image delete".split(),
-                        [mock.Mock(option_strings=["1"])])
-        sot.add_command("image list".split(),
-                        [mock.Mock(option_strings=["2"])])
-        sot.add_command("image list better".split(),
-                        [mock.Mock(option_strings=["3"])])
+        sot.add_command(
+            "image delete".split(), [mock.Mock(option_strings=["1"])]
+        )
+        sot.add_command(
+            "image list".split(), [mock.Mock(option_strings=["2"])]
+        )
+        sot.add_command(
+            "image list better".split(), [mock.Mock(option_strings=["3"])]
+        )
         self.assertEqual("image", sot.get_commands())
         result = sot.get_data()
         self.assertEqual("image", result[0][0])
         self.assertEqual("delete list list_better", result[0][1])
         self.assertEqual("image_delete", result[1][0])
         self.assertEqual("1", result[1][1])
         self.assertEqual("image_list", result[2][0])
@@ -77,22 +84,23 @@
         result = ''
         for line in self.content:
             result = result + line
         return result
 
 
 class TestCompletionAlternatives(base.TestBase):
-
     def given_cmdo_data(self):
         cmdo = "image server"
-        data = [("image", "create"),
-                ("image_create", "--eolus"),
-                ("server", "meta ssh"),
-                ("server_meta_delete", "--wilson"),
-                ("server_ssh", "--sunlight")]
+        data = [
+            ("image", "create"),
+            ("image_create", "--eolus"),
+            ("server", "meta ssh"),
+            ("server_meta_delete", "--wilson"),
+            ("server_ssh", "--sunlight"),
+        ]
         return cmdo, data
 
     def then_data(self, content):
         self.assertIn("  cmds='image server'\n", content)
         self.assertIn("  cmds_image='create'\n", content)
         self.assertIn("  cmds_image_create='--eolus'\n", content)
         self.assertIn("  cmds_server='meta ssh'\n", content)
@@ -113,30 +121,29 @@
         self.assertIn("_openstack()\n", output.content[0])
         self.assertIn("complete -F _openstack openstack\n", output.content[-1])
 
     def test_complete_command_parser(self):
         sot = complete.CompleteCommand(mock.Mock(), mock.Mock())
         parser = sot.get_parser('nothing')
         self.assertEqual("nothing", parser.prog)
-        self.assertEqual("print bash completion command\n    ",
-                         parser.description)
+        self.assertEqual("print bash completion command", parser.description)
 
 
 class TestCompletionAction(base.TestBase):
-
     def given_complete_command(self):
         cmd_mgr = commandmanager.CommandManager('cliff.tests')
         app = application.App('testing', '1', cmd_mgr, stdout=FakeStdout())
         sot = complete.CompleteCommand(app, mock.Mock())
         cmd_mgr.add_command('complete', complete.CompleteCommand)
         return sot, app, cmd_mgr
 
     def then_actions_equal(self, actions):
-        optstr = ' '.join(opt for action in actions
-                          for opt in action.option_strings)
+        optstr = ' '.join(
+            opt for action in actions for opt in action.option_strings
+        )
         self.assertEqual('-h --help --name --shell', optstr)
 
     def test_complete_command_get_actions(self):
         sot, app, cmd_mgr = self.given_complete_command()
         app.interactive_mode = False
         actions = sot.get_actions(["complete"])
         self.then_actions_equal(actions)
```

### Comparing `cliff-4.6.0/cliff/tests/test_formatters_csv.py` & `cliff-4.7.0/cliff/tests/test_formatters_csv.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 from unittest import mock
 
 from cliff.formatters import commaseparated
 from cliff.tests import test_columns
 
 
 class TestCSVFormatter(unittest.TestCase):
-
     def test_commaseparated_list_formatter(self):
         sf = commaseparated.CSVLister()
         c = ('a', 'b', 'c')
         d1 = ('A', 'B', 'C')
         d2 = ('D', 'E', 'F')
         data = [d1, d2]
         expected = 'a,b,c\nA,B,C\nD,E,F\n'
```

### Comparing `cliff-4.6.0/cliff/tests/test_formatters_json.py` & `cliff-4.7.0/cliff/tests/test_formatters_json.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,25 +18,19 @@
 
 from cliff.formatters import json_format
 from cliff.tests import base
 from cliff.tests import test_columns
 
 
 class TestJSONFormatter(base.TestBase):
-
     def test_one(self):
         sf = json_format.JSONFormatter()
         c = ('a', 'b', 'c', 'd')
         d = ('A', 'B', 'C', '"escape me"')
-        expected = {
-            'a': 'A',
-            'b': 'B',
-            'c': 'C',
-            'd': '"escape me"'
-        }
+        expected = {'a': 'A', 'b': 'B', 'c': 'C', 'd': '"escape me"'}
         args = mock.Mock()
         sf.add_argument_group(args)
 
         args.noindent = True
         output = io.StringIO()
         sf.emit_one(c, d, output, args)
         value = output.getvalue()
@@ -74,23 +68,19 @@
         self.assertEqual(1, len(value.splitlines()))
         actual = json.loads(value)
         self.assertEqual(expected, actual)
 
     def test_list(self):
         sf = json_format.JSONFormatter()
         c = ('a', 'b', 'c')
-        d = (
-            ('A1', 'B1', 'C1'),
-            ('A2', 'B2', 'C2'),
-            ('A3', 'B3', 'C3')
-        )
+        d = (('A1', 'B1', 'C1'), ('A2', 'B2', 'C2'), ('A3', 'B3', 'C3'))
         expected = [
             {'a': 'A1', 'b': 'B1', 'c': 'C1'},
             {'a': 'A2', 'b': 'B2', 'c': 'C2'},
-            {'a': 'A3', 'b': 'B3', 'c': 'C3'}
+            {'a': 'A3', 'b': 'B3', 'c': 'C3'},
         ]
         args = mock.Mock()
         sf.add_argument_group(args)
 
         args.noindent = True
         output = io.StringIO()
         sf.emit_list(c, d, output, args)
@@ -106,17 +96,15 @@
         self.assertEqual(17, len(value.splitlines()))
         actual = json.loads(value)
         self.assertEqual(expected, actual)
 
     def test_formattablecolumn_list(self):
         sf = json_format.JSONFormatter()
         c = ('a', 'b', 'c')
-        d = (
-            ('A1', 'B1', test_columns.FauxColumn(['the', 'value'])),
-        )
+        d = (('A1', 'B1', test_columns.FauxColumn(['the', 'value'])),)
         expected = [
             {'a': 'A1', 'b': 'B1', 'c': ['the', 'value']},
         ]
         args = mock.Mock()
         sf.add_argument_group(args)
 
         args.noindent = True
```

### Comparing `cliff-4.6.0/cliff/tests/test_formatters_shell.py` & `cliff-4.7.0/cliff/tests/test_formatters_shell.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 
 from cliff.formatters import shell
 from cliff.tests import base
 from cliff.tests import test_columns
 
 
 class TestShellFormatter(base.TestBase):
-
     def test(self):
         sf = shell.ShellFormatter()
         c = ('a', 'b', 'c', 'd')
         d = ('A', 'B', 'C', '"escape me"')
         expected = 'a="A"\nb="B"\nd="\\"escape me\\""\n'
         output = io.StringIO()
         args = mock.Mock()
@@ -50,33 +49,36 @@
         actual = output.getvalue()
         self.assertEqual(expected, actual)
 
     def test_formattable_column(self):
         sf = shell.ShellFormatter()
         c = ('a', 'b', 'c')
         d = ('A', 'B', test_columns.FauxColumn(['the', 'value']))
-        expected = '\n'.join([
-            'a="A"',
-            'b="B"',
-            'c="[\'the\', \'value\']"\n',
-        ])
+        expected = '\n'.join(
+            [
+                'a="A"',
+                'b="B"',
+                'c="[\'the\', \'value\']"\n',
+            ]
+        )
         output = io.StringIO()
         args = mock.Mock()
         args.variables = ['a', 'b', 'c']
         args.prefix = ''
         sf.emit_one(c, d, output, args)
         actual = output.getvalue()
         self.assertEqual(expected, actual)
 
     def test_non_string_values(self):
         sf = shell.ShellFormatter()
         c = ('a', 'b', 'c', 'd', 'e')
         d = (True, False, 100, '"esc"', str('"esc"'))
-        expected = ('a="True"\nb="False"\nc="100"\n'
-                    'd="\\"esc\\""\ne="\\"esc\\""\n')
+        expected = (
+            'a="True"\nb="False"\nc="100"\n' 'd="\\"esc\\""\ne="\\"esc\\""\n'
+        )
         output = io.StringIO()
         args = mock.Mock()
         args.variables = ['a', 'b', 'c', 'd', 'e']
         args.prefix = ''
         sf.emit_one(c, d, output, args)
         actual = output.getvalue()
         self.assertEqual(expected, actual)
```

### Comparing `cliff-4.6.0/cliff/tests/test_formatters_table.py` & `cliff-4.7.0/cliff/tests/test_formatters_table.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,74 +62,80 @@
     output = StringIO()
     emitter = sf.emit_list if type(data) is list else sf.emit_one
     emitter(tags, data, output, parsed_args)
     return output.getvalue()
 
 
 class TestTableFormatter(base.TestBase):
-
     @mock.patch('cliff.utils.terminal_width')
     def test(self, tw):
         tw.return_value = 80
         c = ('a', 'b', 'c', 'd')
         d = ('A', 'B', 'C', 'test\rcarriage\r\nreturn')
-        expected = textwrap.dedent('''\
+        expected = textwrap.dedent(
+            '''\
         +-------+---------------+
         | Field | Value         |
         +-------+---------------+
         | a     | A             |
         | b     | B             |
         | c     | C             |
         | d     | test carriage |
         |       | return        |
         +-------+---------------+
-        ''')
+        '''
+        )
         self.assertEqual(expected, _table_tester_helper(c, d))
 
 
 class TestTerminalWidth(base.TestBase):
-
     # Multi-line output when width is restricted to 42 columns
-    expected_ml_val = textwrap.dedent('''\
+    expected_ml_val = textwrap.dedent(
+        '''\
     +-------+--------------------------------+
     | Field | Value                          |
     +-------+--------------------------------+
     | a     | A                              |
     | b     | B                              |
     | c     | C                              |
     | d     | dddddddddddddddddddddddddddddd |
     |       | dddddddddddddddddddddddddddddd |
     |       | ddddddddddddddddd              |
     +-------+--------------------------------+
-    ''')
+    '''
+    )
 
     # Multi-line output when width is restricted to 80 columns
-    expected_ml_80_val = textwrap.dedent('''\
+    expected_ml_80_val = textwrap.dedent(
+        '''\
     +-------+----------------------------------------------------------------------+
     | Field | Value                                                                |
     +-------+----------------------------------------------------------------------+
     | a     | A                                                                    |
     | b     | B                                                                    |
     | c     | C                                                                    |
     | d     | dddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddd |
     |       | ddddddddd                                                            |
     +-------+----------------------------------------------------------------------+
-    ''')  # noqa
+    '''
+    )  # noqa
 
     # Single-line output, for when no line length restriction apply
-    expected_sl_val = textwrap.dedent('''\
+    expected_sl_val = textwrap.dedent(
+        '''\
     +-------+-------------------------------------------------------------------------------+
     | Field | Value                                                                         |
     +-------+-------------------------------------------------------------------------------+
     | a     | A                                                                             |
     | b     | B                                                                             |
     | c     | C                                                                             |
     | d     | ddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddd |
     +-------+-------------------------------------------------------------------------------+
-    ''')  # noqa
+    '''
+    )  # noqa
 
     @mock.patch('cliff.utils.terminal_width')
     def test_table_formatter_no_cli_param(self, tw):
         tw.return_value = 80
         c = ('a', 'b', 'c', 'd')
         d = ('A', 'B', 'C', 'd' * 77)
         self.assertEqual(
@@ -188,207 +194,223 @@
         self.assertEqual(
             self.expected_ml_val,
             _table_tester_helper(c, d, extra_args=['--max-width', '42']),
         )
 
 
 class TestMaxWidth(base.TestBase):
-
-    expected_80 = textwrap.dedent('''\
+    expected_80 = textwrap.dedent(
+        '''\
     +--------------------------+---------------------------------------------+
     | Field                    | Value                                       |
     +--------------------------+---------------------------------------------+
     | field_name               | the value                                   |
     | a_really_long_field_name | a value significantly longer than the field |
     +--------------------------+---------------------------------------------+
-    ''')
+    '''
+    )
 
     @mock.patch('cliff.utils.terminal_width')
     def test_80(self, tw):
         tw.return_value = 80
         c = ('field_name', 'a_really_long_field_name')
         d = ('the value', 'a value significantly longer than the field')
         self.assertEqual(self.expected_80, _table_tester_helper(c, d))
 
     @mock.patch('cliff.utils.terminal_width')
     def test_70(self, tw):
         # resize value column
         tw.return_value = 70
         c = ('field_name', 'a_really_long_field_name')
         d = ('the value', 'a value significantly longer than the field')
-        expected = textwrap.dedent('''\
+        expected = textwrap.dedent(
+            '''\
         +--------------------------+-----------------------------------------+
         | Field                    | Value                                   |
         +--------------------------+-----------------------------------------+
         | field_name               | the value                               |
         | a_really_long_field_name | a value significantly longer than the   |
         |                          | field                                   |
         +--------------------------+-----------------------------------------+
-        ''')
+        '''
+        )
         self.assertEqual(
             expected,
             _table_tester_helper(c, d, extra_args=['--fit-width']),
         )
 
     @mock.patch('cliff.utils.terminal_width')
     def test_50(self, tw):
         # resize both columns
         tw.return_value = 50
         c = ('field_name', 'a_really_long_field_name')
         d = ('the value', 'a value significantly longer than the field')
-        expected = textwrap.dedent('''\
+        expected = textwrap.dedent(
+            '''\
         +-----------------------+------------------------+
         | Field                 | Value                  |
         +-----------------------+------------------------+
         | field_name            | the value              |
         | a_really_long_field_n | a value significantly  |
         | ame                   | longer than the field  |
         +-----------------------+------------------------+
-        ''')
+        '''
+        )
         self.assertEqual(
             expected,
             _table_tester_helper(c, d, extra_args=['--fit-width']),
         )
 
     @mock.patch('cliff.utils.terminal_width')
     def test_10(self, tw):
         # resize all columns limited by min_width=16
         tw.return_value = 10
         c = ('field_name', 'a_really_long_field_name')
         d = ('the value', 'a value significantly longer than the field')
-        expected = textwrap.dedent('''\
+        expected = textwrap.dedent(
+            '''\
         +------------------+------------------+
         | Field            | Value            |
         +------------------+------------------+
         | field_name       | the value        |
         | a_really_long_fi | a value          |
         | eld_name         | significantly    |
         |                  | longer than the  |
         |                  | field            |
         +------------------+------------------+
-        ''')
+        '''
+        )
         self.assertEqual(
             expected,
             _table_tester_helper(c, d, extra_args=['--fit-width']),
         )
 
 
 class TestListFormatter(base.TestBase):
-
     _col_names = ('one', 'two', 'three')
-    _col_data = [(
-        'one one one one one',
-        'two two two two',
-        'three three')]
+    _col_data = [('one one one one one', 'two two two two', 'three three')]
 
     _expected_mv = {
-        80: textwrap.dedent('''\
+        80: textwrap.dedent(
+            '''\
         +---------------------+-----------------+-------------+
         | one                 | two             | three       |
         +---------------------+-----------------+-------------+
         | one one one one one | two two two two | three three |
         +---------------------+-----------------+-------------+
-        '''),
-
-        50: textwrap.dedent('''\
+        '''
+        ),
+        50: textwrap.dedent(
+            '''\
         +----------------+-----------------+-------------+
         | one            | two             | three       |
         +----------------+-----------------+-------------+
         | one one one    | two two two two | three three |
         | one one        |                 |             |
         +----------------+-----------------+-------------+
-        '''),
-
-        47: textwrap.dedent('''\
+        '''
+        ),
+        47: textwrap.dedent(
+            '''\
         +---------------+---------------+-------------+
         | one           | two           | three       |
         +---------------+---------------+-------------+
         | one one one   | two two two   | three three |
         | one one       | two           |             |
         +---------------+---------------+-------------+
-        '''),
-
-        45: textwrap.dedent('''\
+        '''
+        ),
+        45: textwrap.dedent(
+            '''\
         +--------------+--------------+-------------+
         | one          | two          | three       |
         +--------------+--------------+-------------+
         | one one one  | two two two  | three three |
         | one one      | two          |             |
         +--------------+--------------+-------------+
-        '''),
-
-        40: textwrap.dedent('''\
+        '''
+        ),
+        40: textwrap.dedent(
+            '''\
         +------------+------------+------------+
         | one        | two        | three      |
         +------------+------------+------------+
         | one one    | two two    | three      |
         | one one    | two two    | three      |
         | one        |            |            |
         +------------+------------+------------+
-        '''),
-
-        10: textwrap.dedent('''\
+        '''
+        ),
+        10: textwrap.dedent(
+            '''\
         +----------+----------+----------+
         | one      | two      | three    |
         +----------+----------+----------+
         | one one  | two two  | three    |
         | one one  | two two  | three    |
         | one      |          |          |
         +----------+----------+----------+
-        '''),
+        '''
+        ),
     }
 
     @mock.patch('cliff.utils.terminal_width')
     def test_table_list_formatter(self, tw):
         tw.return_value = 80
         c = ('a', 'b', 'c')
         d1 = ('A', 'B', 'C')
         d2 = ('D', 'E', 'test\rcarriage\r\nreturn')
         data = [d1, d2]
-        expected = textwrap.dedent('''\
+        expected = textwrap.dedent(
+            '''\
         +---+---+---------------+
         | a | b | c             |
         +---+---+---------------+
         | A | B | C             |
         | D | E | test carriage |
         |   |   | return        |
         +---+---+---------------+
-        ''')
+        '''
+        )
         self.assertEqual(expected, _table_tester_helper(c, data))
 
     @mock.patch('cliff.utils.terminal_width')
     def test_table_formatter_formattable_column(self, tw):
         tw.return_value = 0
         c = ('a', 'b', 'c', 'd')
         d = ('A', 'B', 'C', test_columns.FauxColumn(['the', 'value']))
-        expected = textwrap.dedent('''\
+        expected = textwrap.dedent(
+            '''\
         +-------+---------------------------------------------+
         | Field | Value                                       |
         +-------+---------------------------------------------+
         | a     | A                                           |
         | b     | B                                           |
         | c     | C                                           |
         | d     | I made this string myself: ['the', 'value'] |
         +-------+---------------------------------------------+
-        ''')
+        '''
+        )
         self.assertEqual(expected, _table_tester_helper(c, d))
 
     @mock.patch('cliff.utils.terminal_width')
     def test_formattable_column(self, tw):
         tw.return_value = 80
         c = ('a', 'b', 'c')
         d1 = ('A', 'B', test_columns.FauxColumn(['the', 'value']))
         data = [d1]
-        expected = textwrap.dedent('''\
+        expected = textwrap.dedent(
+            '''\
         +---+---+---------------------------------------------+
         | a | b | c                                           |
         +---+---+---------------------------------------------+
         | A | B | I made this string myself: ['the', 'value'] |
         +---+---+---------------------------------------------+
-        ''')
+        '''
+        )
         self.assertEqual(expected, _table_tester_helper(c, data))
 
     @mock.patch('cliff.utils.terminal_width')
     def test_max_width_80(self, tw):
         # no resize
         width = tw.return_value = 80
         self.assertEqual(
@@ -396,43 +418,47 @@
             _table_tester_helper(self._col_names, self._col_data),
         )
 
     @mock.patch('cliff.utils.terminal_width')
     def test_max_width_50(self, tw):
         # resize 1 column
         width = tw.return_value = 50
-        actual = _table_tester_helper(self._col_names, self._col_data,
-                                      extra_args=['--fit-width'])
+        actual = _table_tester_helper(
+            self._col_names, self._col_data, extra_args=['--fit-width']
+        )
         self.assertEqual(self._expected_mv[width], actual)
         self.assertEqual(width, len(actual.splitlines()[0]))
 
     @mock.patch('cliff.utils.terminal_width')
     def test_max_width_45(self, tw):
         # resize 2 columns
         width = tw.return_value = 45
-        actual = _table_tester_helper(self._col_names, self._col_data,
-                                      extra_args=['--fit-width'])
+        actual = _table_tester_helper(
+            self._col_names, self._col_data, extra_args=['--fit-width']
+        )
         self.assertEqual(self._expected_mv[width], actual)
         self.assertEqual(width, len(actual.splitlines()[0]))
 
     @mock.patch('cliff.utils.terminal_width')
     def test_max_width_40(self, tw):
         # resize all columns
         width = tw.return_value = 40
-        actual = _table_tester_helper(self._col_names, self._col_data,
-                                      extra_args=['--fit-width'])
+        actual = _table_tester_helper(
+            self._col_names, self._col_data, extra_args=['--fit-width']
+        )
         self.assertEqual(self._expected_mv[width], actual)
         self.assertEqual(width, len(actual.splitlines()[0]))
 
     @mock.patch('cliff.utils.terminal_width')
     def test_max_width_10(self, tw):
         # resize all columns limited by min_width=8
         width = tw.return_value = 10
-        actual = _table_tester_helper(self._col_names, self._col_data,
-                                      extra_args=['--fit-width'])
+        actual = _table_tester_helper(
+            self._col_names, self._col_data, extra_args=['--fit-width']
+        )
         self.assertEqual(self._expected_mv[width], actual)
         # 3 columns each 8 wide, plus table spacing and borders
         expected_width = 11 * 3 + 1
         self.assertEqual(expected_width, len(actual.splitlines()[0]))
 
     # Force a wide terminal by overriding its width with envvar
     @mock.patch('cliff.utils.terminal_width')
@@ -546,24 +572,26 @@
         expected_width = 11 * 3 + 1
         self.assertEqual(expected_width, len(actual.splitlines()[0]))
 
     @mock.patch.dict(os.environ, {'CLIFF_MAX_TERM_WIDTH': '42'})
     def test_env_maxwidth_args_big(self):
         self.assertEqual(
             self._expected_mv[80],
-            _table_tester_helper(self._col_names, self._col_data,
-                                 extra_args=args(666)),
+            _table_tester_helper(
+                self._col_names, self._col_data, extra_args=args(666)
+            ),
         )
 
     @mock.patch.dict(os.environ, {'CLIFF_MAX_TERM_WIDTH': '42'})
     def test_env_maxwidth_args_tiny(self):
         self.assertEqual(
             self._expected_mv[40],
-            _table_tester_helper(self._col_names, self._col_data,
-                                 extra_args=args(40)),
+            _table_tester_helper(
+                self._col_names, self._col_data, extra_args=args(40)
+            ),
         )
 
     @mock.patch('cliff.utils.terminal_width')
     def test_empty(self, tw):
         tw.return_value = 80
         c = ('a', 'b', 'c')
         data = []
@@ -571,54 +599,43 @@
         self.assertEqual(expected, _table_tester_helper(c, data))
 
     @mock.patch('cliff.utils.terminal_width')
     def test_empty_table(self, tw):
         tw.return_value = 80
         c = ('a', 'b', 'c')
         data = []
-        expected = textwrap.dedent('''\
+        expected = textwrap.dedent(
+            '''\
         +---+---+---+
         | a | b | c |
         +---+---+---+
         +---+---+---+
-        ''')
+        '''
+        )
         self.assertEqual(
             expected,
-            _table_tester_helper(c, data,
-                                 extra_args=['--print-empty']),
+            _table_tester_helper(c, data, extra_args=['--print-empty']),
         )
 
 
 class TestFieldWidths(base.TestBase):
-
     def test(self):
         tf = table.TableFormatter
         self.assertEqual(
-            {
-                'a': 1,
-                'b': 2,
-                'c': 3,
-                'd': 10
-            },
+            {'a': 1, 'b': 2, 'c': 3, 'd': 10},
             tf._field_widths(
-                ('a', 'b', 'c', 'd'),
-                '+---+----+-----+------------+'),
+                ('a', 'b', 'c', 'd'), '+---+----+-----+------------+'
+            ),
         )
 
     def test_zero(self):
         tf = table.TableFormatter
         self.assertEqual(
-            {
-                'a': 0,
-                'b': 0,
-                'c': 0
-            },
-            tf._field_widths(
-                ('a', 'b', 'c'),
-                '+--+-++'),
+            {'a': 0, 'b': 0, 'c': 0},
+            tf._field_widths(('a', 'b', 'c'), '+--+-++'),
         )
 
     def test_info(self):
         tf = table.TableFormatter
         self.assertEqual((49, 4), (tf._width_info(80, 10)))
         self.assertEqual((76, 76), (tf._width_info(80, 1)))
         self.assertEqual((79, 0), (tf._width_info(80, 0)))
```

### Comparing `cliff-4.6.0/cliff/tests/test_formatters_value.py` & `cliff-4.7.0/cliff/tests/test_formatters_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 from cliff.formatters import value
 from cliff.tests import base
 from cliff.tests import test_columns
 
 
 class TestValueFormatter(base.TestBase):
-
     def test(self):
         sf = value.ValueFormatter()
         c = ('a', 'b', 'c', 'd')
         d = ('A', 'B', 'C', '"no escape me"')
         expected = 'A\nB\nC\n"no escape me"\n'
         output = StringIO()
         sf.emit_one(c, d, output, None)
```

### Comparing `cliff-4.6.0/cliff/tests/test_formatters_yaml.py` & `cliff-4.7.0/cliff/tests/test_formatters_yaml.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
 from cliff.formatters import yaml_format
 from cliff.tests import base
 from cliff.tests import test_columns
 
 
 class _toDict:
-
     def __init__(self, **kwargs):
         self._data = kwargs
 
     def toDict(self):
         return self._data
 
 
@@ -36,25 +35,19 @@
         self._data = kwargs
 
     def to_dict(self):
         return self._data
 
 
 class TestYAMLFormatter(base.TestBase):
-
     def test_format_one(self):
         sf = yaml_format.YAMLFormatter()
         c = ('a', 'b', 'c', 'd')
         d = ('A', 'B', 'C', '"escape me"')
-        expected = {
-            'a': 'A',
-            'b': 'B',
-            'c': 'C',
-            'd': '"escape me"'
-        }
+        expected = {'a': 'A', 'b': 'B', 'c': 'C', 'd': '"escape me"'}
         output = StringIO()
         args = mock.Mock()
         sf.emit_one(c, d, output, args)
         actual = yaml.safe_load(output.getvalue())
         self.assertEqual(expected, actual)
 
     def test_formattablecolumn_one(self):
@@ -77,37 +70,31 @@
         print(len(value.splitlines()))
         actual = yaml.safe_load(output.getvalue())
         self.assertEqual(expected, actual)
 
     def test_list(self):
         sf = yaml_format.YAMLFormatter()
         c = ('a', 'b', 'c')
-        d = (
-            ('A1', 'B1', 'C1'),
-            ('A2', 'B2', 'C2'),
-            ('A3', 'B3', 'C3')
-        )
+        d = (('A1', 'B1', 'C1'), ('A2', 'B2', 'C2'), ('A3', 'B3', 'C3'))
         expected = [
             {'a': 'A1', 'b': 'B1', 'c': 'C1'},
             {'a': 'A2', 'b': 'B2', 'c': 'C2'},
-            {'a': 'A3', 'b': 'B3', 'c': 'C3'}
+            {'a': 'A3', 'b': 'B3', 'c': 'C3'},
         ]
         output = StringIO()
         args = mock.Mock()
         sf.add_argument_group(args)
         sf.emit_list(c, d, output, args)
         actual = yaml.safe_load(output.getvalue())
         self.assertEqual(expected, actual)
 
     def test_formattablecolumn_list(self):
         sf = yaml_format.YAMLFormatter()
         c = ('a', 'b', 'c')
-        d = (
-            ('A1', 'B1', test_columns.FauxColumn(['the', 'value'])),
-        )
+        d = (('A1', 'B1', test_columns.FauxColumn(['the', 'value'])),)
         expected = [
             {'a': 'A1', 'b': 'B1', 'c': ['the', 'value']},
         ]
         args = mock.Mock()
         sf.add_argument_group(args)
 
         args.noindent = True
@@ -120,34 +107,34 @@
         sf = yaml_format.YAMLFormatter()
         c = ('a', 'b', 'toDict', 'to_dict')
         d = ('A', 'B', _toDict(spam="ham"), _to_Dict(ham="eggs"))
         expected = {
             'a': 'A',
             'b': 'B',
             'toDict': {"spam": "ham"},
-            'to_dict': {"ham": "eggs"}
+            'to_dict': {"ham": "eggs"},
         }
         output = StringIO()
         args = mock.Mock()
         sf.emit_one(c, d, output, args)
         actual = yaml.safe_load(output.getvalue())
         self.assertEqual(expected, actual)
 
     def test_list_custom_object(self):
         sf = yaml_format.YAMLFormatter()
         c = ('a', 'toDict', 'to_dict')
         d = (
             ('A1', _toDict(B=1), _to_Dict(C=1)),
             ('A2', _toDict(B=2), _to_Dict(C=2)),
-            ('A3', _toDict(B=3), _to_Dict(C=3))
+            ('A3', _toDict(B=3), _to_Dict(C=3)),
         )
         expected = [
             {'a': 'A1', 'toDict': {'B': 1}, 'to_dict': {'C': 1}},
             {'a': 'A2', 'toDict': {'B': 2}, 'to_dict': {'C': 2}},
-            {'a': 'A3', 'toDict': {'B': 3}, 'to_dict': {'C': 3}}
+            {'a': 'A3', 'toDict': {'B': 3}, 'to_dict': {'C': 3}},
         ]
         output = StringIO()
         args = mock.Mock()
         sf.add_argument_group(args)
         sf.emit_list(c, d, output, args)
         actual = yaml.safe_load(output.getvalue())
         self.assertEqual(expected, actual)
```

### Comparing `cliff-4.6.0/cliff/tests/test_help.py` & `cliff-4.7.0/cliff/tests/test_help.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,23 +20,25 @@
 from cliff import commandmanager
 from cliff import help
 from cliff.tests import base
 from cliff.tests import utils
 
 
 class TestHelp(base.TestBase):
-
     def test_show_help_for_command(self):
         # FIXME(dhellmann): Are commands tied too closely to the app? Or
         # do commands know too much about apps by using them to get to the
         # command manager?
         stdout = io.StringIO()
-        app = application.App('testing', '1',
-                              utils.TestCommandManager(utils.TEST_NAMESPACE),
-                              stdout=stdout)
+        app = application.App(
+            'testing',
+            '1',
+            utils.TestCommandManager(utils.TEST_NAMESPACE),
+            stdout=stdout,
+        )
         app.NAME = 'test'
         help_cmd = help.HelpCommand(app, mock.Mock())
         parser = help_cmd.get_parser('test')
         parsed_args = parser.parse_args(['one'])
         try:
             help_cmd.run(parsed_args)
         except help.HelpExit:
@@ -44,17 +46,20 @@
         self.assertEqual('TestParser', stdout.getvalue())
 
     def test_list_matching_commands(self):
         # FIXME(dhellmann): Are commands tied too closely to the app? Or
         # do commands know too much about apps by using them to get to the
         # command manager?
         stdout = io.StringIO()
-        app = application.App('testing', '1',
-                              utils.TestCommandManager(utils.TEST_NAMESPACE),
-                              stdout=stdout)
+        app = application.App(
+            'testing',
+            '1',
+            utils.TestCommandManager(utils.TEST_NAMESPACE),
+            stdout=stdout,
+        )
         app.NAME = 'test'
         help_cmd = help.HelpCommand(app, mock.Mock())
         parser = help_cmd.get_parser('test')
         parsed_args = parser.parse_args(['t'])
         try:
             help_cmd.run(parsed_args)
         except help.HelpExit:
@@ -64,17 +69,20 @@
         self.assertIn('three word command\n  two words\n', help_output)
 
     def test_list_matching_commands_no_match(self):
         # FIXME(dhellmann): Are commands tied too closely to the app? Or
         # do commands know too much about apps by using them to get to the
         # command manager?
         stdout = io.StringIO()
-        app = application.App('testing', '1',
-                              utils.TestCommandManager(utils.TEST_NAMESPACE),
-                              stdout=stdout)
+        app = application.App(
+            'testing',
+            '1',
+            utils.TestCommandManager(utils.TEST_NAMESPACE),
+            stdout=stdout,
+        )
         app.NAME = 'test'
         help_cmd = help.HelpCommand(app, mock.Mock())
         parser = help_cmd.get_parser('test')
         parsed_args = parser.parse_args(['z'])
         self.assertRaises(
             ValueError,
             help_cmd.run,
@@ -82,17 +90,20 @@
         )
 
     def test_show_help_for_help(self):
         # FIXME(dhellmann): Are commands tied too closely to the app? Or
         # do commands know too much about apps by using them to get to the
         # command manager?
         stdout = io.StringIO()
-        app = application.App('testing', '1',
-                              utils.TestCommandManager(utils.TEST_NAMESPACE),
-                              stdout=stdout)
+        app = application.App(
+            'testing',
+            '1',
+            utils.TestCommandManager(utils.TEST_NAMESPACE),
+            stdout=stdout,
+        )
         app.NAME = 'test'
         app.options = mock.Mock()
         help_cmd = help.HelpCommand(app, mock.Mock())
         parser = help_cmd.get_parser('test')
         parsed_args = parser.parse_args([])
         try:
             help_cmd.run(parsed_args)
@@ -109,34 +120,43 @@
         self.assertIn(expected, help_text)
 
     def test_list_deprecated_commands(self):
         # FIXME(dhellmann): Are commands tied too closely to the app? Or
         # do commands know too much about apps by using them to get to the
         # command manager?
         stdout = io.StringIO()
-        app = application.App('testing', '1',
-                              utils.TestCommandManager(utils.TEST_NAMESPACE),
-                              stdout=stdout)
+        app = application.App(
+            'testing',
+            '1',
+            utils.TestCommandManager(utils.TEST_NAMESPACE),
+            stdout=stdout,
+        )
         app.NAME = 'test'
         try:
             app.run(['--help'])
         except help.HelpExit:
             pass
         help_output = stdout.getvalue()
         self.assertIn('two words', help_output)
         self.assertIn('three word command', help_output)
         self.assertNotIn('old cmd', help_output)
 
-    @mock.patch.object(commandmanager.EntryPointWrapper, 'load',
-                       side_effect=Exception('Could not load EntryPoint'))
+    @mock.patch.object(
+        commandmanager.EntryPointWrapper,
+        'load',
+        side_effect=Exception('Could not load EntryPoint'),
+    )
     def test_show_help_with_ep_load_fail(self, mock_load):
         stdout = io.StringIO()
-        app = application.App('testing', '1',
-                              utils.TestCommandManager(utils.TEST_NAMESPACE),
-                              stdout=stdout)
+        app = application.App(
+            'testing',
+            '1',
+            utils.TestCommandManager(utils.TEST_NAMESPACE),
+            stdout=stdout,
+        )
         app.NAME = 'test'
         app.options = mock.Mock()
         app.options.debug = False
         help_cmd = help.HelpCommand(app, mock.Mock())
         parser = help_cmd.get_parser('test')
         parsed_args = parser.parse_args([])
         try:
@@ -144,21 +164,27 @@
         except help.HelpExit:
             pass
         help_output = stdout.getvalue()
         self.assertIn('Commands:', help_output)
         self.assertIn('Could not load', help_output)
         self.assertNotIn('Exception: Could not load EntryPoint', help_output)
 
-    @mock.patch.object(commandmanager.EntryPointWrapper, 'load',
-                       side_effect=Exception('Could not load EntryPoint'))
+    @mock.patch.object(
+        commandmanager.EntryPointWrapper,
+        'load',
+        side_effect=Exception('Could not load EntryPoint'),
+    )
     def test_show_help_print_exc_with_ep_load_fail(self, mock_load):
         stdout = io.StringIO()
-        app = application.App('testing', '1',
-                              utils.TestCommandManager(utils.TEST_NAMESPACE),
-                              stdout=stdout)
+        app = application.App(
+            'testing',
+            '1',
+            utils.TestCommandManager(utils.TEST_NAMESPACE),
+            stdout=stdout,
+        )
         app.NAME = 'test'
         app.options = mock.Mock()
         app.options.debug = True
         help_cmd = help.HelpCommand(app, mock.Mock())
         parser = help_cmd.get_parser('test')
         parsed_args = parser.parse_args([])
         try:
```

### Comparing `cliff-4.6.0/cliff/tests/test_interactive.py` & `cliff-4.7.0/cliff/tests/test_interactive.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,24 +19,29 @@
 
 
 class FakeApp(object):
     NAME = 'Fake'
 
 
 class TestInteractive(base.TestBase):
-
     def make_interactive_app(self, errexit, *command_names):
         fake_command_manager = [(x, None) for x in command_names]
-        return InteractiveApp(FakeApp, fake_command_manager,
-                              stdin=None, stdout=None, errexit=errexit)
+        return InteractiveApp(
+            FakeApp,
+            fake_command_manager,
+            stdin=None,
+            stdout=None,
+            errexit=errexit,
+        )
 
     def _test_completenames(self, expecteds, prefix):
         app = self.make_interactive_app(False, 'hips', 'hippo', 'nonmatching')
         self.assertEqual(
-            set(app.completenames(prefix, '', 0, 1)), set(expecteds))
+            set(app.completenames(prefix, '', 0, 1)), set(expecteds)
+        )
 
     def test_cmd2_completenames(self):
         # cmd2.Cmd define do_help method
         self._test_completenames(['help'], 'he')
 
     def test_cliff_completenames(self):
         self._test_completenames(['hips', 'hippo'], 'hip')
@@ -52,16 +57,17 @@
         #                requirement.
         if hasattr(cmd2.Cmd, "do_hi"):
             self._test_completenames(['hi', 'history', 'hips', 'hippo'], 'hi')
         else:
             self._test_completenames(['history', 'hips', 'hippo'], 'hi')
 
     def _test_completedefault(self, expecteds, line, begidx):
-        command_names = set(['show file', 'show folder', 'show  long',
-                             'list all'])
+        command_names = set(
+            ['show file', 'show folder', 'show  long', 'list all']
+        )
         app = self.make_interactive_app(False, *command_names)
         observeds = app.completedefault(None, line, begidx, None)
         self.assertEqual(set(expecteds), set(observeds))
         self.assertTrue(
             set([line[:begidx] + x for x in observeds]) <= command_names
         )
```

### Comparing `cliff-4.6.0/cliff/tests/test_lister.py` & `cliff-4.7.0/cliff/tests/test_lister.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,53 +17,47 @@
 from unittest import mock
 
 from cliff import lister
 from cliff.tests import base
 
 
 class FauxFormatter(object):
-
     def __init__(self):
         self.args = []
         self.obj = weakref.proxy(self)
 
     def emit_list(self, columns, data, stdout, args):
         self.args.append((columns, data))
 
 
 class ExerciseLister(lister.Lister):
-
     data = [('a', 'A'), ('b', 'B'), ('c', 'A')]
 
     def _load_formatter_plugins(self):
         return {
             'test': FauxFormatter(),
         }
 
     def take_action(self, parsed_args):
         return (parsed_args.columns, self.data)
 
 
 class ExerciseListerCustomSort(ExerciseLister):
-
     need_sort_by_cliff = False
 
 
 class ExerciseListerNullValues(ExerciseLister):
-
     data = ExerciseLister.data + [(None, None)]
 
 
 class ExerciseListerDifferentTypes(ExerciseLister):
-
     data = ExerciseLister.data + [(1, 0)]
 
 
 class TestLister(base.TestBase):
-
     def test_formatter_args(self):
         app = mock.Mock()
         test_lister = ExerciseLister(app, [])
 
         parsed_args = mock.Mock()
         parsed_args.columns = ('Col1', 'Col2')
         parsed_args.formatter = 'test'
@@ -144,15 +138,16 @@
 
         test_lister.run(parsed_args)
 
         f = test_lister._formatter_plugins['test']
         args = f.args[0]
         data = list(args[1])
         self.assertEqual(
-            [['a', 'A'], ['c', 'A'], ['b', 'B'], [None, None]], data)
+            [['a', 'A'], ['c', 'A'], ['b', 'B'], [None, None]], data
+        )
 
     def test_sort_by_column_with_different_types(self):
         test_lister = ExerciseListerDifferentTypes(mock.Mock(), [])
         parsed_args = mock.Mock()
         parsed_args.columns = ('Col1', 'Col2')
         parsed_args.formatter = 'test'
         parsed_args.sort_columns = ['Col2', 'Col1']
@@ -160,32 +155,36 @@
         with mock.patch.object(lister.Lister, 'log') as mock_log:
             test_lister.run(parsed_args)
 
         f = test_lister._formatter_plugins['test']
         args = f.args[0]
         data = list(args[1])
         # The output should be unchanged
-        self.assertEqual(
-            [['a', 'A'], ['b', 'B'], ['c', 'A'], [1, 0]], data)
+        self.assertEqual([['a', 'A'], ['b', 'B'], ['c', 'A'], [1, 0]], data)
         # but we should have logged a warning
-        mock_log.warning.assert_has_calls([
-            mock.call("Could not sort on field '%s'; unsortable types", col)
-            for col in parsed_args.sort_columns
-        ])
+        mock_log.warning.assert_has_calls(
+            [
+                mock.call(
+                    "Could not sort on field '%s'; unsortable types", col
+                )
+                for col in parsed_args.sort_columns
+            ]
+        )
 
     def test_sort_by_non_displayed_column(self):
         test_lister = ExerciseLister(mock.Mock(), [])
         parsed_args = mock.Mock()
         parsed_args.columns = ('Col1',)
         parsed_args.formatter = 'test'
         parsed_args.sort_columns = ['Col2']
 
         with mock.patch.object(test_lister, 'take_action') as mock_take_action:
             mock_take_action.return_value = (
-                ('Col1', 'Col2'), [['a', 'A'], ['b', 'B'], ['c', 'A']]
+                ('Col1', 'Col2'),
+                [['a', 'A'], ['b', 'B'], ['c', 'A']],
             )
             test_lister.run(parsed_args)
 
         f = test_lister._formatter_plugins['test']
         args = f.args[0]
         data = list(args[1])
         self.assertEqual([['a'], ['c'], ['b']], data)
```

### Comparing `cliff-4.6.0/cliff/tests/test_show.py` & `cliff-4.7.0/cliff/tests/test_show.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,39 +17,36 @@
 from unittest import mock
 
 from cliff import show
 from cliff.tests import base
 
 
 class FauxFormatter(object):
-
     def __init__(self):
         self.args = []
         self.obj = weakref.proxy(self)
 
     def emit_one(self, columns, data, stdout, args):
         self.args.append((columns, data))
 
 
 class ExerciseShowOne(show.ShowOne):
-
     def _load_formatter_plugins(self):
         return {
             'test': FauxFormatter(),
         }
 
     def take_action(self, parsed_args):
         return (
             parsed_args.columns,
             [('a', 'A'), ('b', 'B')],
         )
 
 
 class TestShow(base.TestBase):
-
     def test_formatter_args(self):
         app = mock.Mock()
         test_show = ExerciseShowOne(app, [])
 
         parsed_args = mock.Mock()
         parsed_args.columns = ('Col1', 'Col2')
         parsed_args.formatter = 'test'
```

### Comparing `cliff-4.6.0/cliff/tests/test_sphinxext.py` & `cliff-4.7.0/cliff/tests/test_sphinxext.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,161 +16,212 @@
 import textwrap
 
 from cliff import sphinxext
 from cliff.tests import base
 
 
 class TestSphinxExtension(base.TestBase):
-
     def test_empty_help(self):
         """Handle positional and optional actions without help messages."""
         parser = argparse.ArgumentParser(prog='hello-world', add_help=False)
         parser.add_argument('name', action='store')
         parser.add_argument('--language', dest='lang')
 
         output = '\n'.join(sphinxext._format_parser(parser))
-        self.assertEqual(textwrap.dedent("""
+        self.assertEqual(
+            textwrap.dedent(
+                """
         .. program:: hello-world
         .. code-block:: shell
 
             hello-world [--language LANG] name
 
         .. option:: --language <LANG>
 
         .. option:: name
-        """).lstrip(), output)
+        """
+            ).lstrip(),
+            output,
+        )
 
     def test_nonempty_help(self):
         """Handle positional and optional actions with help messages."""
         parser = argparse.ArgumentParser(prog='hello-world', add_help=False)
         parser.add_argument('name', help='user name')
-        parser.add_argument('--language', dest='lang',
-                            help='greeting language')
+        parser.add_argument(
+            '--language', dest='lang', help='greeting language'
+        )
 
         output = '\n'.join(sphinxext._format_parser(parser))
-        self.assertEqual(textwrap.dedent("""
+        self.assertEqual(
+            textwrap.dedent(
+                """
         .. program:: hello-world
         .. code-block:: shell
 
             hello-world [--language LANG] name
 
         .. option:: --language <LANG>
 
             greeting language
 
         .. option:: name
 
             user name
-        """).lstrip(), output)
+        """
+            ).lstrip(),
+            output,
+        )
 
     def test_description_epilog(self):
         """Handle a parser description, epilog."""
-        parser = argparse.ArgumentParser(prog='hello-world', add_help=False,
-                                         description='A "Hello, World" app.',
-                                         epilog='What am I doing down here?')
+        parser = argparse.ArgumentParser(
+            prog='hello-world',
+            add_help=False,
+            description='A "Hello, World" app.',
+            epilog='What am I doing down here?',
+        )
         parser.add_argument('name', action='store')
         parser.add_argument('--language', dest='lang')
 
         output = '\n'.join(sphinxext._format_parser(parser))
-        self.assertEqual(textwrap.dedent("""
+        self.assertEqual(
+            textwrap.dedent(
+                """
         A "Hello, World" app.
 
         .. program:: hello-world
         .. code-block:: shell
 
             hello-world [--language LANG] name
 
         .. option:: --language <LANG>
 
         .. option:: name
 
         What am I doing down here?
-        """).lstrip(), output)
+        """
+            ).lstrip(),
+            output,
+        )
 
     def test_flag(self):
         """Handle a boolean argparse action."""
         parser = argparse.ArgumentParser(prog='hello-world', add_help=False)
         parser.add_argument('name', help='user name')
-        parser.add_argument('--translate', action='store_true',
-                            help='translate to local language')
+        parser.add_argument(
+            '--translate',
+            action='store_true',
+            help='translate to local language',
+        )
 
         output = '\n'.join(sphinxext._format_parser(parser))
-        self.assertEqual(textwrap.dedent("""
+        self.assertEqual(
+            textwrap.dedent(
+                """
         .. program:: hello-world
         .. code-block:: shell
 
             hello-world [--translate] name
 
         .. option:: --translate
 
             translate to local language
 
         .. option:: name
 
             user name
-        """).lstrip(), output)
+        """
+            ).lstrip(),
+            output,
+        )
 
     def test_supressed(self):
         """Handle a supressed action."""
         parser = argparse.ArgumentParser(prog='hello-world', add_help=False)
         parser.add_argument('name', help='user name')
         parser.add_argument('--variable', help=argparse.SUPPRESS)
 
         output = '\n'.join(sphinxext._format_parser(parser))
-        self.assertEqual(textwrap.dedent("""
+        self.assertEqual(
+            textwrap.dedent(
+                """
         .. program:: hello-world
         .. code-block:: shell
 
             hello-world name
 
 
         .. option:: name
 
             user name
-        """).lstrip(), output)
+        """
+            ).lstrip(),
+            output,
+        )
 
     def test_metavar(self):
         """Handle an option with a metavar."""
         parser = argparse.ArgumentParser(prog='hello-world', add_help=False)
-        parser.add_argument('names', metavar='<NAME>', nargs='+',
-                            help='a user name')
+        parser.add_argument(
+            'names', metavar='<NAME>', nargs='+', help='a user name'
+        )
 
         output = '\n'.join(sphinxext._format_parser(parser))
-        self.assertEqual(textwrap.dedent("""
+        self.assertEqual(
+            textwrap.dedent(
+                """
         .. program:: hello-world
         .. code-block:: shell
 
             hello-world <NAME> [<NAME> ...]
 
         .. option:: NAME
 
             a user name
-        """).lstrip(), output)
+        """
+            ).lstrip(),
+            output,
+        )
 
     def test_multiple_opts(self):
         """Correctly output multiple opts on separate lines."""
         parser = argparse.ArgumentParser(prog='hello-world', add_help=False)
         parser.add_argument('name', help='user name')
-        parser.add_argument('--language', dest='lang',
-                            help='greeting language')
-        parser.add_argument('--translate', action='store_true',
-                            help='translate to local language')
-        parser.add_argument('--write-to-var-log-something-or-other',
-                            action='store_true',
-                            help='a long opt to force wrapping')
-        parser.add_argument('--required-arg', dest='stuff', required=True,
-                            help='a required argument')
+        parser.add_argument(
+            '--language', dest='lang', help='greeting language'
+        )
+        parser.add_argument(
+            '--translate',
+            action='store_true',
+            help='translate to local language',
+        )
+        parser.add_argument(
+            '--write-to-var-log-something-or-other',
+            action='store_true',
+            help='a long opt to force wrapping',
+        )
+        parser.add_argument(
+            '--required-arg',
+            dest='stuff',
+            required=True,
+            help='a required argument',
+        )
         style_group = parser.add_mutually_exclusive_group(required=True)
-        style_group.add_argument('--polite', action='store_true',
-                                 help='use a polite greeting')
-        style_group.add_argument('--profane', action='store_true',
-                                 help='use a less polite greeting')
+        style_group.add_argument(
+            '--polite', action='store_true', help='use a polite greeting'
+        )
+        style_group.add_argument(
+            '--profane', action='store_true', help='use a less polite greeting'
+        )
 
         output = '\n'.join(sphinxext._format_parser(parser))
-        self.assertEqual(textwrap.dedent("""
+        self.assertEqual(
+            textwrap.dedent(
+                """
         .. program:: hello-world
         .. code-block:: shell
 
             hello-world
                 [--language LANG]
                 [--translate]
                 [--write-to-var-log-something-or-other]
@@ -201,34 +252,44 @@
         .. option:: --profane
 
             use a less polite greeting
 
         .. option:: name
 
             user name
-        """).lstrip(), output)
+        """
+            ).lstrip(),
+            output,
+        )
 
     def test_various_option_names_with_hyphen(self):
         """Handle options whose name and/or metavar contain hyphen(s)"""
         parser = argparse.ArgumentParser(prog='hello-world', add_help=False)
-        parser.add_argument('--foo-bar', metavar='<foo-bar>',
-                            help='foo bar', required=True)
-        parser.add_argument('--foo-bar-baz', metavar='<foo-bar-baz>',
-                            help='foo bar baz', required=True)
-        parser.add_argument('--foo', metavar='<foo>',
-                            help='foo', required=True)
-        parser.add_argument('--alpha', metavar='<A>',
-                            help='alpha')
-        parser.add_argument('--alpha-beta', metavar='<A-B>',
-                            help='alpha beta')
-        parser.add_argument('--alpha-beta-gamma', metavar='<A-B-C>',
-                            help='alpha beta gamma')
+        parser.add_argument(
+            '--foo-bar', metavar='<foo-bar>', help='foo bar', required=True
+        )
+        parser.add_argument(
+            '--foo-bar-baz',
+            metavar='<foo-bar-baz>',
+            help='foo bar baz',
+            required=True,
+        )
+        parser.add_argument(
+            '--foo', metavar='<foo>', help='foo', required=True
+        )
+        parser.add_argument('--alpha', metavar='<A>', help='alpha')
+        parser.add_argument('--alpha-beta', metavar='<A-B>', help='alpha beta')
+        parser.add_argument(
+            '--alpha-beta-gamma', metavar='<A-B-C>', help='alpha beta gamma'
+        )
 
         output = '\n'.join(sphinxext._format_parser(parser))
-        self.assertEqual(textwrap.dedent("""
+        self.assertEqual(
+            textwrap.dedent(
+                """
         .. program:: hello-world
         .. code-block:: shell
 
             hello-world
                 --foo-bar <foo-bar>
                 --foo-bar-baz <foo-bar-baz>
                 --foo <foo>
@@ -255,8 +316,11 @@
         .. option:: --alpha-beta <A-B>
 
             alpha beta
 
         .. option:: --alpha-beta-gamma <A-B-C>
 
             alpha beta gamma
-        """).lstrip(), output)
+        """
+            ).lstrip(),
+            output,
+        )
```

### Comparing `cliff-4.6.0/cliff/tests/test_utils.py` & `cliff-4.7.0/cliff/tests/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from unittest import mock
 
 from cliff.tests import base
 from cliff import utils
 
 
 class TestTerminalWidth(base.TestBase):
-
     def test(self):
         width = utils.terminal_width()
         # Results are specific to the execution environment, so only assert
         # that no error is raised.
         if width is not None:
             self.assertIsInstance(width, int)
```

### Comparing `cliff-4.6.0/cliff/tests/utils.py` & `cliff-4.7.0/cliff/tests/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 from cliff.command import Command
 from cliff.commandmanager import CommandManager
 
 TEST_NAMESPACE = 'cliff.test'
 
 
 class TestParser(object):
-
     def print_help(self, stdout):
         stdout.write('TestParser')
 
 
 class TestCommand(Command):
     "Test command."
 
@@ -31,18 +30,16 @@
         return TestParser()
 
     def take_action(self, args):
         return
 
 
 class TestDeprecatedCommand(TestCommand):
-
     deprecated = True
 
 
 class TestCommandManager(CommandManager):
-
     def load_commands(self, namespace):
         if namespace == TEST_NAMESPACE:
             for key in ('one', 'two words', 'three word command'):
                 self.add_command(key, TestCommand)
             self.add_command('old cmd', TestDeprecatedCommand)
```

### Comparing `cliff-4.6.0/cliff/utils.py` & `cliff-4.7.0/cliff/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,30 +55,30 @@
     row2 = row1[:]
     row0 = row1[:]
 
     for i in range(len1):
         row2[0] = (i + 1) * cost['d']
 
         for j in range(len2):
-
             # substitution
             sub_cost = row1[j] + (s1[i] != s2[j]) * cost['s']
 
             # insertion
             ins_cost = row2[j] + cost['a']
 
             # deletion
             del_cost = row1[j + 1] + cost['d']
 
             # swap
-            swp_condition = ((i > 0) and
-                             (j > 0) and
-                             (s1[i - 1] == s2[j]) and
-                             (s1[i] == s2[j - 1])
-                             )
+            swp_condition = (
+                (i > 0)
+                and (j > 0)
+                and (s1[i - 1] == s2[j])
+                and (s1[i] == s2[j - 1])
+            )
 
             # min cost
             if swp_condition:
                 swp_cost = row0[j - 1] + cost['w']
                 p_cost = min(sub_cost, ins_cost, del_cost, swp_cost)
             else:
                 p_cost = min(sub_cost, ins_cost, del_cost)
```

### Comparing `cliff-4.6.0/cliff.egg-info/PKG-INFO` & `cliff-4.7.0/cliff.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: cliff
-Version: 4.6.0
+Version: 4.7.0
 Summary: Command Line Interface Formulation Framework
 Home-page: https://docs.openstack.org/cliff/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `cliff-4.6.0/cliff.egg-info/SOURCES.txt` & `cliff-4.7.0/cliff.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+.git-blame-ignore-revs
 .pre-commit-config.yaml
 .stestr.conf
 .zuul.yaml
 AUTHORS
 CONTRIBUTING.rst
 ChangeLog
 LICENSE
```

### Comparing `cliff-4.6.0/cliff.egg-info/entry_points.txt` & `cliff-4.7.0/cliff.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `cliff-4.6.0/demoapp/README.rst` & `cliff-4.7.0/demoapp/README.rst`

 * *Files identical despite different names*

### Comparing `cliff-4.6.0/demoapp/cliffdemo/hook.py` & `cliff-4.7.0/demoapp/cliffdemo/hook.py`

 * *Files identical despite different names*

### Comparing `cliff-4.6.0/demoapp/cliffdemo/main.py` & `cliff-4.7.0/demoapp/cliffdemo/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import sys
 
 from cliff.app import App
 from cliff.commandmanager import CommandManager
 
 
 class DemoApp(App):
-
     def __init__(self):
         super(DemoApp, self).__init__(
             description='cliff demo app',
             version='0.1',
             command_manager=CommandManager('cliff.demo'),
             deferred_help=True,
-            )
+        )
 
     def initialize_app(self, argv):
         self.LOG.debug('initialize_app')
 
     def prepare_to_run_command(self, cmd):
         self.LOG.debug('prepare_to_run_command %s', cmd.__class__.__name__)
```

### Comparing `cliff-4.6.0/demoapp/cliffdemo/show.py` & `cliff-4.7.0/demoapp/cliffdemo/show.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,20 +12,22 @@
     def get_parser(self, prog_name):
         parser = super(File, self).get_parser(prog_name)
         parser.add_argument('filename', nargs='?', default='.')
         return parser
 
     def take_action(self, parsed_args):
         stat_data = os.stat(parsed_args.filename)
-        columns = ('Name',
-                   'Size',
-                   'UID',
-                   'GID',
-                   'Modified Time',
-                   )
-        data = (parsed_args.filename,
-                stat_data.st_size,
-                stat_data.st_uid,
-                stat_data.st_gid,
-                stat_data.st_mtime,
-                )
+        columns = (
+            'Name',
+            'Size',
+            'UID',
+            'GID',
+            'Modified Time',
+        )
+        data = (
+            parsed_args.filename,
+            stat_data.st_size,
+            stat_data.st_uid,
+            stat_data.st_gid,
+            stat_data.st_mtime,
+        )
         return (columns, data)
```

### Comparing `cliff-4.6.0/demoapp/cliffdemo/simple.py` & `cliff-4.7.0/demoapp/cliffdemo/simple.py`

 * *Files identical despite different names*

### Comparing `cliff-4.6.0/demoapp/setup.py` & `cliff-4.7.0/demoapp/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,49 +12,38 @@
     long_description = open('README.rst', 'rt').read()
 except IOError:
     long_description = ''
 
 setup(
     name=PROJECT,
     version=VERSION,
-
     description='Demo app for cliff',
     long_description=long_description,
-
     author='Doug Hellmann',
     author_email='doug.hellmann@gmail.com',
-
     url='https://github.com/openstack/cliff',
     download_url='https://github.com/openstack/cliff/tarball/master',
-
     classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3 :: Only',
         'Intended Audience :: Developers',
         'Environment :: Console',
     ],
-
     platforms=['Any'],
-
     scripts=[],
-
     provides=[],
     install_requires=['cliff'],
-
     namespace_packages=[],
     packages=find_packages(),
     include_package_data=True,
-
     entry_points={
-        'console_scripts': [
-            'cliffdemo = cliffdemo.main:main'
-        ],
+        'console_scripts': ['cliffdemo = cliffdemo.main:main'],
         'cliff.demo': [
             'simple = cliffdemo.simple:Simple',
             'two_part = cliffdemo.simple:Simple',
             'error = cliffdemo.simple:Error',
             'list files = cliffdemo.list:Files',
             'files = cliffdemo.list:Files',
             'file = cliffdemo.show:File',
@@ -62,10 +51,9 @@
             'unicode = cliffdemo.encoding:Encoding',
             'hooked = cliffdemo.hook:Hooked',
         ],
         'cliff.demo.hooked': [
             'sample-hook = cliffdemo.hook:Hook',
         ],
     },
-
     zip_safe=False,
 )
```

### Comparing `cliff-4.6.0/doc/source/conf.py` & `cliff-4.7.0/doc/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,28 +193,25 @@
 
 
 # -- Options for LaTeX output ------------------------------------------------
 
 latex_elements = {
     # The paper size ('letterpaper' or 'a4paper').
     # 'papersize': 'letterpaper',
-
     # The font size ('10pt', '11pt' or '12pt').
     # 'pointsize': '10pt',
-
     # Additional stuff for the LaTeX preamble.
     # 'preamble': '',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author,
 # documentclass [howto/manual]).
 latex_documents = [
-    ('index', 'cliff.tex', 'cliff Documentation',
-     'Doug Hellmann', 'manual'),
+    ('index', 'cliff.tex', 'cliff Documentation', 'Doug Hellmann', 'manual'),
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
 # latex_logo = None
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
@@ -234,32 +231,35 @@
 # latex_domain_indices = True
 
 
 # -- Options for manual page output ------------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
-man_pages = [
-    ('index', 'cliff', 'cliff Documentation',
-     ['Doug Hellmann'], 1)
-]
+man_pages = [('index', 'cliff', 'cliff Documentation', ['Doug Hellmann'], 1)]
 
 # If true, show URL addresses after external links.
 # man_show_urls = False
 
 
 # -- Options for Texinfo output ----------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-    ('index', 'cliff', 'cliff Documentation',
-     'Doug Hellmann', 'cliff', 'One line description of project.',
-     'Miscellaneous'),
+    (
+        'index',
+        'cliff',
+        'cliff Documentation',
+        'Doug Hellmann',
+        'cliff',
+        'One line description of project.',
+        'Miscellaneous',
+    ),
 ]
 
 # Documents to append as an appendix to all manuals.
 # texinfo_appendices = []
 
 # If false, no module index is generated.
 # texinfo_domain_indices = True
```

### Comparing `cliff-4.6.0/doc/source/contributors/index.rst` & `cliff-4.7.0/doc/source/contributors/index.rst`

 * *Files identical despite different names*

### Comparing `cliff-4.6.0/doc/source/install/index.rst` & `cliff-4.7.0/doc/source/install/index.rst`

 * *Files identical despite different names*

### Comparing `cliff-4.6.0/doc/source/reference/index.rst` & `cliff-4.7.0/doc/source/reference/index.rst`

 * *Files identical despite different names*

### Comparing `cliff-4.6.0/doc/source/user/complete.rst` & `cliff-4.7.0/doc/source/user/complete.rst`

 * *Files identical despite different names*

### Comparing `cliff-4.6.0/doc/source/user/demoapp.rst` & `cliff-4.7.0/doc/source/user/demoapp.rst`

 * *Files identical despite different names*

### Comparing `cliff-4.6.0/doc/source/user/interactive_mode.rst` & `cliff-4.7.0/doc/source/user/interactive_mode.rst`

 * *Files identical despite different names*

### Comparing `cliff-4.6.0/doc/source/user/introduction.rst` & `cliff-4.7.0/doc/source/user/introduction.rst`

 * *Files identical despite different names*

### Comparing `cliff-4.6.0/doc/source/user/list_commands.rst` & `cliff-4.7.0/doc/source/user/list_commands.rst`

 * *Files identical despite different names*

### Comparing `cliff-4.6.0/doc/source/user/show_commands.rst` & `cliff-4.7.0/doc/source/user/show_commands.rst`

 * *Files identical despite different names*

### Comparing `cliff-4.6.0/doc/source/user/sphinxext.rst` & `cliff-4.7.0/doc/source/user/sphinxext.rst`

 * *Files identical despite different names*

### Comparing `cliff-4.6.0/integration-tests/openstackclient-tip.sh` & `cliff-4.7.0/integration-tests/openstackclient-tip.sh`

 * *Files identical despite different names*

### Comparing `cliff-4.6.0/releasenotes/notes/add-Lister-sort-direction-5f34dba3c9743572.yaml` & `cliff-4.7.0/releasenotes/notes/add-Lister-sort-direction-5f34dba3c9743572.yaml`

 * *Files identical despite different names*

### Comparing `cliff-4.6.0/setup.cfg` & `cliff-4.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `cliff-4.6.0/setup.py` & `cliff-4.7.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
 # implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# THIS FILE IS MANAGED BY THE GLOBAL REQUIREMENTS REPO - DO NOT EDIT
 import setuptools
 
 setuptools.setup(
     setup_requires=['pbr>=2.0.0'],
     install_requires=['setuptools'],
-    pbr=True)
+    pbr=True,
+)
```

