# Comparing `tmp/tach-0.1.8.tar.gz` & `tmp/tach-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tach-0.1.8.tar", last modified: Wed May  8 01:31:01 2024, max compression
+gzip compressed data, was "tach-0.1.9.tar", last modified: Thu May  9 15:44:29 2024, max compression
```

## Comparing `tach-0.1.8.tar` & `tach-0.1.9.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.448600 tach-0.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.428600 tach-0.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.432600 tach-0.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-08 01:30:57.000000 tach-0.1.8/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-08 01:30:57.000000 tach-0.1.8/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-08 01:30:57.000000 tach-0.1.8/.github/workflows/publish_docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-08 01:30:57.000000 tach-0.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-08 01:30:57.000000 tach-0.1.8/.pre-commit-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-08 01:30:57.000000 tach-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-05-08 01:31:01.448600 tach-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-05-08 01:30:57.000000 tach-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-08 01:30:57.000000 tach-0.1.8/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.436601 tach-0.1.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-08 01:30:57.000000 tach-0.1.8/docs/configuration.md
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-08 01:30:57.000000 tach-0.1.8/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-08 01:30:57.000000 tach-0.1.8/docs/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-08 01:30:57.000000 tach-0.1.8/docs/getting-started.md
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-08 01:30:57.000000 tach-0.1.8/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-08 01:30:57.000000 tach-0.1.8/docs/strict-mode.md
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-08 01:30:57.000000 tach-0.1.8/docs/tach-ignore.md
--rw-r--r--   0 runner    (1001) docker     (127)    92208 2024-05-08 01:30:57.000000 tach-0.1.8/docs/tach_demo.mp4
--rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-05-08 01:30:57.000000 tach-0.1.8/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-08 01:30:57.000000 tach-0.1.8/docs/why-tach.md
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-08 01:30:57.000000 tach-0.1.8/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-08 01:30:57.000000 tach-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 01:31:01.448600 tach-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.436601 tach-0.1.8/tach/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:30:57.000000 tach-0.1.8/tach/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-05-08 01:30:57.000000 tach-0.1.8/tach/add.py
--rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-05-08 01:30:57.000000 tach-0.1.8/tach/check.py
--rw-r--r--   0 runner    (1001) docker     (127)     7491 2024-05-08 01:30:57.000000 tach-0.1.8/tach/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.436601 tach-0.1.8/tach/colors/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-08 01:30:57.000000 tach-0.1.8/tach/colors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-08 01:30:57.000000 tach-0.1.8/tach/colors/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.436601 tach-0.1.8/tach/constants/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-08 01:30:57.000000 tach-0.1.8/tach/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-08 01:30:57.000000 tach-0.1.8/tach/constants/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.436601 tach-0.1.8/tach/core/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-08 01:30:57.000000 tach-0.1.8/tach/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-05-08 01:30:57.000000 tach-0.1.8/tach/core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-08 01:30:57.000000 tach-0.1.8/tach/core/package.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-08 01:30:57.000000 tach-0.1.8/tach/core/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.436601 tach-0.1.8/tach/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-08 01:30:57.000000 tach-0.1.8/tach/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-08 01:30:57.000000 tach-0.1.8/tach/errors/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.440600 tach-0.1.8/tach/filesystem/
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-08 01:30:57.000000 tach-0.1.8/tach/filesystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-08 01:30:57.000000 tach-0.1.8/tach/filesystem/install.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-08 01:30:57.000000 tach-0.1.8/tach/filesystem/package.py
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-08 01:30:57.000000 tach-0.1.8/tach/filesystem/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-08 01:30:57.000000 tach-0.1.8/tach/filesystem/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     9347 2024-05-08 01:30:57.000000 tach-0.1.8/tach/filesystem/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.440600 tach-0.1.8/tach/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (127)       83 2024-05-08 01:30:57.000000 tach-0.1.8/tach/hooks/pre-commit
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-05-08 01:30:57.000000 tach-0.1.8/tach/init.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-08 01:30:57.000000 tach-0.1.8/tach/loading.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-08 01:30:57.000000 tach-0.1.8/tach/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.440600 tach-0.1.8/tach/parsing/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-08 01:30:57.000000 tach-0.1.8/tach/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-08 01:30:57.000000 tach-0.1.8/tach/parsing/ast_visitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-08 01:30:57.000000 tach-0.1.8/tach/parsing/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4807 2024-05-08 01:30:57.000000 tach-0.1.8/tach/parsing/imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-08 01:30:57.000000 tach-0.1.8/tach/parsing/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-08 01:30:57.000000 tach-0.1.8/tach/parsing/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-08 01:30:57.000000 tach-0.1.8/tach/parsing/packages.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.444600 tach-0.1.8/tach.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-05-08 01:31:01.000000 tach-0.1.8/tach.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-08 01:31:01.000000 tach-0.1.8/tach.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 01:31:01.000000 tach-0.1.8/tach.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-08 01:31:01.000000 tach-0.1.8/tach.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-08 01:31:01.000000 tach-0.1.8/tach.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-08 01:31:01.000000 tach-0.1.8/tach.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-08 01:30:57.000000 tach-0.1.8/tach.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.440600 tach-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:30:57.000000 tach-0.1.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.440600 tach-0.1.8/tests/example/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.440600 tach-0.1.8/tests/example/domain_one/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/domain_one/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/domain_one/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.440600 tach-0.1.8/tests/example/domain_one/subdomain/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/domain_one/subdomain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/domain_one/subdomain/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.440600 tach-0.1.8/tests/example/domain_three/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/domain_three/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/domain_three/core.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/domain_three/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.444600 tach-0.1.8/tests/example/domain_two/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/domain_two/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/domain_two/core.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/domain_two/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.444600 tach-0.1.8/tests/example/domain_two/subdomain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/domain_two/subdomain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/domain_two/subdomain/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.444600 tach-0.1.8/tests/example/invalid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/invalid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.444600 tach-0.1.8/tests/example/invalid/empty/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/invalid/empty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/invalid/empty/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/invalid/empty/tach.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.444600 tach-0.1.8/tests/example/invalid/hidden/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.444600 tach-0.1.8/tests/example/invalid/hidden/.hidden/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/invalid/hidden/.hidden/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/invalid/hidden/.hidden/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/invalid/hidden/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/invalid/hidden/tach.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.444600 tach-0.1.8/tests/example/invalid/hidden/unhidden/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/invalid/hidden/unhidden/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/invalid/hidden/unhidden/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/invalid/hidden/unhidden/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/invalid/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/invalid/tach.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.444600 tach-0.1.8/tests/example/valid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/valid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.444600 tach-0.1.8/tests/example/valid/domain_one/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/valid/domain_one/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/valid/domain_one/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.444600 tach-0.1.8/tests/example/valid/domain_three/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/valid/domain_three/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/valid/domain_three/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.444600 tach-0.1.8/tests/example/valid/domain_two/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/valid/domain_two/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/valid/domain_two/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/valid/tach.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-05-08 01:30:57.000000 tach-0.1.8/tests/test_add.py
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-05-08 01:30:57.000000 tach-0.1.8/tests/test_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-08 01:30:57.000000 tach-0.1.8/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-08 01:30:57.000000 tach-0.1.8/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-08 01:30:57.000000 tach-0.1.8/tests/test_module_trie.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-08 01:30:57.000000 tach-0.1.8/tests/test_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 01:30:57.000000 tach-0.1.8/tests/test_show.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.905271 tach-0.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.881271 tach-0.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.889271 tach-0.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-09 15:44:24.000000 tach-0.1.9/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-09 15:44:24.000000 tach-0.1.9/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-09 15:44:24.000000 tach-0.1.9/.github/workflows/publish_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-09 15:44:24.000000 tach-0.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-09 15:44:24.000000 tach-0.1.9/.pre-commit-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-09 15:44:24.000000 tach-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-05-09 15:44:29.905271 tach-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-05-09 15:44:24.000000 tach-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-09 15:44:24.000000 tach-0.1.9/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.889271 tach-0.1.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-09 15:44:24.000000 tach-0.1.9/docs/configuration.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-09 15:44:24.000000 tach-0.1.9/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-09 15:44:24.000000 tach-0.1.9/docs/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-09 15:44:24.000000 tach-0.1.9/docs/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-09 15:44:24.000000 tach-0.1.9/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-09 15:44:24.000000 tach-0.1.9/docs/strict-mode.md
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-09 15:44:24.000000 tach-0.1.9/docs/tach-ignore.md
+-rw-r--r--   0 runner    (1001) docker     (127)    92208 2024-05-09 15:44:24.000000 tach-0.1.9/docs/tach_demo.mp4
+-rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-05-09 15:44:24.000000 tach-0.1.9/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-09 15:44:24.000000 tach-0.1.9/docs/why-tach.md
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-09 15:44:24.000000 tach-0.1.9/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-09 15:44:24.000000 tach-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 15:44:29.905271 tach-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.889271 tach-0.1.9/tach/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:24.000000 tach-0.1.9/tach/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-05-09 15:44:24.000000 tach-0.1.9/tach/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-05-09 15:44:24.000000 tach-0.1.9/tach/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7491 2024-05-09 15:44:24.000000 tach-0.1.9/tach/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.893271 tach-0.1.9/tach/colors/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-09 15:44:24.000000 tach-0.1.9/tach/colors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-09 15:44:24.000000 tach-0.1.9/tach/colors/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.893271 tach-0.1.9/tach/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-09 15:44:24.000000 tach-0.1.9/tach/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-09 15:44:24.000000 tach-0.1.9/tach/constants/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.893271 tach-0.1.9/tach/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-09 15:44:24.000000 tach-0.1.9/tach/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-05-09 15:44:24.000000 tach-0.1.9/tach/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-09 15:44:24.000000 tach-0.1.9/tach/core/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-09 15:44:24.000000 tach-0.1.9/tach/core/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.893271 tach-0.1.9/tach/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-09 15:44:24.000000 tach-0.1.9/tach/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-09 15:44:24.000000 tach-0.1.9/tach/errors/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.893271 tach-0.1.9/tach/filesystem/
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-09 15:44:24.000000 tach-0.1.9/tach/filesystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-09 15:44:24.000000 tach-0.1.9/tach/filesystem/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-09 15:44:24.000000 tach-0.1.9/tach/filesystem/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-09 15:44:24.000000 tach-0.1.9/tach/filesystem/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-09 15:44:24.000000 tach-0.1.9/tach/filesystem/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9347 2024-05-09 15:44:24.000000 tach-0.1.9/tach/filesystem/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.893271 tach-0.1.9/tach/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      405 2024-05-09 15:44:24.000000 tach-0.1.9/tach/hooks/pre-commit
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-05-09 15:44:24.000000 tach-0.1.9/tach/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-09 15:44:24.000000 tach-0.1.9/tach/loading.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-09 15:44:24.000000 tach-0.1.9/tach/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.897271 tach-0.1.9/tach/parsing/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-09 15:44:24.000000 tach-0.1.9/tach/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-09 15:44:24.000000 tach-0.1.9/tach/parsing/ast_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-09 15:44:24.000000 tach-0.1.9/tach/parsing/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4807 2024-05-09 15:44:24.000000 tach-0.1.9/tach/parsing/imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-09 15:44:24.000000 tach-0.1.9/tach/parsing/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-09 15:44:24.000000 tach-0.1.9/tach/parsing/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-09 15:44:24.000000 tach-0.1.9/tach/parsing/packages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.905271 tach-0.1.9/tach.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-05-09 15:44:29.000000 tach-0.1.9/tach.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-09 15:44:29.000000 tach-0.1.9/tach.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 15:44:29.000000 tach-0.1.9/tach.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-09 15:44:29.000000 tach-0.1.9/tach.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-09 15:44:29.000000 tach-0.1.9/tach.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-09 15:44:29.000000 tach-0.1.9/tach.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-09 15:44:24.000000 tach-0.1.9/tach.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.897271 tach-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:24.000000 tach-0.1.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.897271 tach-0.1.9/tests/example/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.897271 tach-0.1.9/tests/example/domain_one/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/domain_one/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/domain_one/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.897271 tach-0.1.9/tests/example/domain_one/subdomain/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/domain_one/subdomain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/domain_one/subdomain/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.901271 tach-0.1.9/tests/example/domain_three/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/domain_three/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/domain_three/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/domain_three/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.901271 tach-0.1.9/tests/example/domain_two/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/domain_two/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/domain_two/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/domain_two/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.901271 tach-0.1.9/tests/example/domain_two/subdomain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/domain_two/subdomain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/domain_two/subdomain/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.901271 tach-0.1.9/tests/example/invalid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/invalid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.901271 tach-0.1.9/tests/example/invalid/empty/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/invalid/empty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/invalid/empty/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/invalid/empty/tach.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.901271 tach-0.1.9/tests/example/invalid/hidden/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.901271 tach-0.1.9/tests/example/invalid/hidden/.hidden/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/invalid/hidden/.hidden/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/invalid/hidden/.hidden/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/invalid/hidden/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/invalid/hidden/tach.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.901271 tach-0.1.9/tests/example/invalid/hidden/unhidden/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/invalid/hidden/unhidden/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/invalid/hidden/unhidden/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/invalid/hidden/unhidden/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/invalid/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/invalid/tach.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.901271 tach-0.1.9/tests/example/valid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/valid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.905271 tach-0.1.9/tests/example/valid/domain_one/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/valid/domain_one/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/valid/domain_one/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.905271 tach-0.1.9/tests/example/valid/domain_three/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/valid/domain_three/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/valid/domain_three/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.905271 tach-0.1.9/tests/example/valid/domain_two/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/valid/domain_two/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/valid/domain_two/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/valid/tach.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-05-09 15:44:24.000000 tach-0.1.9/tests/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-05-09 15:44:24.000000 tach-0.1.9/tests/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-09 15:44:24.000000 tach-0.1.9/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-09 15:44:24.000000 tach-0.1.9/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-09 15:44:24.000000 tach-0.1.9/tests/test_module_trie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-09 15:44:24.000000 tach-0.1.9/tests/test_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 15:44:24.000000 tach-0.1.9/tests/test_show.py
```

### Comparing `tach-0.1.8/.github/workflows/ci.yml` & `tach-0.1.9/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `tach-0.1.8/.github/workflows/publish.yml` & `tach-0.1.9/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `tach-0.1.8/.github/workflows/publish_docs.yml` & `tach-0.1.9/.github/workflows/publish_docs.yml`

 * *Files identical despite different names*

### Comparing `tach-0.1.8/.gitignore` & `tach-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `tach-0.1.8/LICENSE` & `tach-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tach-0.1.8/PKG-INFO` & `tach-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tach
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Python tool to maintain a modular package architecture.
 Author-email: Caelean Barnes <caeleanb@gmail.com>, Evan Doyle <evanmdoyle@gmail.com>
 Project-URL: Homepage, https://github.com/never-over/tach
 Project-URL: Issues, https://github.com/never-over/tach/issues
 Keywords: python,module,package,guard,enforcement,boundary,enforcer,domain,architecture
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `tach-0.1.8/README.md` & `tach-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `tach-0.1.8/docs/configuration.md` & `tach-0.1.9/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `tach-0.1.8/docs/faq.md` & `tach-0.1.9/docs/faq.md`

 * *Files identical despite different names*

### Comparing `tach-0.1.8/docs/favicon.ico` & `tach-0.1.9/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `tach-0.1.8/docs/getting-started.md` & `tach-0.1.9/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `tach-0.1.8/docs/index.md` & `tach-0.1.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `tach-0.1.8/docs/strict-mode.md` & `tach-0.1.9/docs/strict-mode.md`

 * *Files identical despite different names*

### Comparing `tach-0.1.8/docs/tach-ignore.md` & `tach-0.1.9/docs/tach-ignore.md`

 * *Files identical despite different names*

### Comparing `tach-0.1.8/docs/tach_demo.mp4` & `tach-0.1.9/docs/tach_demo.mp4`

 * *Files identical despite different names*

### Comparing `tach-0.1.8/docs/usage.md` & `tach-0.1.9/docs/usage.md`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
 ### With pre-commit framework
 If you use the [pre-commit framework](https://github.com/pre-commit/pre-commit), you can add the following to your `.pre-commit-hooks.yaml`:
 
 ```yaml
 repos:
 -   repo: https://github.com/Never-Over/tach
-    rev: v0.1.2
+    rev: v0.1.9  # change this to the latest tag!
     hooks:
     -   id: tach
 ```
 
 Note that you should specify the version you are using in the `rev` key.
```

### Comparing `tach-0.1.8/docs/why-tach.md` & `tach-0.1.9/docs/why-tach.md`

 * *Files identical despite different names*

### Comparing `tach-0.1.8/mkdocs.yml` & `tach-0.1.9/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `tach-0.1.8/pyproject.toml` & `tach-0.1.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tach"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="Caelean Barnes", email="caeleanb@gmail.com" },
   { name="Evan Doyle", email="evanmdoyle@gmail.com" },
 ]
 description = "A Python tool to maintain a modular package architecture."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `tach-0.1.8/tach/add.py` & `tach-0.1.9/tach/add.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.8/tach/check.py` & `tach-0.1.9/tach/check.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.8/tach/cli.py` & `tach-0.1.9/tach/cli.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.8/tach/core/config.py` & `tach-0.1.9/tach/core/config.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.8/tach/core/package.py` & `tach-0.1.9/tach/core/package.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.8/tach/filesystem/__init__.py` & `tach-0.1.9/tach/filesystem/__init__.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.8/tach/filesystem/install.py` & `tach-0.1.9/tach/filesystem/install.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.8/tach/filesystem/project.py` & `tach-0.1.9/tach/filesystem/project.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.8/tach/filesystem/service.py` & `tach-0.1.9/tach/filesystem/service.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.8/tach/init.py` & `tach-0.1.9/tach/init.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.8/tach/loading.py` & `tach-0.1.9/tach/loading.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.8/tach/parsing/config.py` & `tach-0.1.9/tach/parsing/config.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.8/tach/parsing/imports.py` & `tach-0.1.9/tach/parsing/imports.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.8/tach/parsing/interface.py` & `tach-0.1.9/tach/parsing/interface.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.8/tach/parsing/packages.py` & `tach-0.1.9/tach/parsing/packages.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.8/tach.egg-info/PKG-INFO` & `tach-0.1.9/tach.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tach
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Python tool to maintain a modular package architecture.
 Author-email: Caelean Barnes <caeleanb@gmail.com>, Evan Doyle <evanmdoyle@gmail.com>
 Project-URL: Homepage, https://github.com/never-over/tach
 Project-URL: Issues, https://github.com/never-over/tach/issues
 Keywords: python,module,package,guard,enforcement,boundary,enforcer,domain,architecture
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `tach-0.1.8/tach.egg-info/SOURCES.txt` & `tach-0.1.9/tach.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tach-0.1.8/tests/test_add.py` & `tach-0.1.9/tests/test_add.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.8/tests/test_check.py` & `tach-0.1.9/tests/test_check.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.8/tests/test_cli.py` & `tach-0.1.9/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.8/tests/test_init.py` & `tach-0.1.9/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.8/tests/test_module_trie.py` & `tach-0.1.9/tests/test_module_trie.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.8/tests/test_parsing.py` & `tach-0.1.9/tests/test_parsing.py`

 * *Files identical despite different names*

