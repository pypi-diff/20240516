# Comparing `tmp/opp_env-0.28.1.240417.tar.gz` & `tmp/opp_env-0.29.0.240422.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opp_env-0.28.1.240417.tar", last modified: Wed Apr 17 12:57:14 2024, max compression
+gzip compressed data, was "opp_env-0.29.0.240422.tar", last modified: Mon Apr 22 15:53:12 2024, max compression
```

## Comparing `opp_env-0.28.1.240417.tar` & `opp_env-0.29.0.240422.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:57:14.801293 opp_env-0.28.1.240417/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:57:14.793293 opp_env-0.28.1.240417/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:57:14.793293 opp_env-0.28.1.240417/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-04-17 12:57:06.000000 opp_env-0.28.1.240417/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-17 12:57:06.000000 opp_env-0.28.1.240417/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-17 12:57:06.000000 opp_env-0.28.1.240417/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11519 2024-04-17 12:57:14.801293 opp_env-0.28.1.240417/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9982 2024-04-17 12:57:06.000000 opp_env-0.28.1.240417/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:57:14.797293 opp_env-0.28.1.240417/docker/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-17 12:57:06.000000 opp_env-0.28.1.240417/docker/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-17 12:57:06.000000 opp_env-0.28.1.240417/docker/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (127)       66 2024-04-17 12:57:06.000000 opp_env-0.28.1.240417/docker/build
--rwxr-xr-x   0 runner    (1001) docker     (127)      155 2024-04-17 12:57:06.000000 opp_env-0.28.1.240417/docker/build-wsl-image
--rwxr-xr-x   0 runner    (1001) docker     (127)      268 2024-04-17 12:57:06.000000 opp_env-0.28.1.240417/docker/entrypoint.sh
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-17 12:57:06.000000 opp_env-0.28.1.240417/docker/nix.conf
--rwxr-xr-x   0 runner    (1001) docker     (127)       54 2024-04-17 12:57:06.000000 opp_env-0.28.1.240417/docker/opp_env.cmd
--rwxr-xr-x   0 runner    (1001) docker     (127)       24 2024-04-17 12:57:06.000000 opp_env-0.28.1.240417/docker/opp_env_distro.cmd
--rwxr-xr-x   0 runner    (1001) docker     (127)      131 2024-04-17 12:57:06.000000 opp_env-0.28.1.240417/docker/opp_env_distro_install.cmd
--rwxr-xr-x   0 runner    (1001) docker     (127)      103 2024-04-17 12:57:06.000000 opp_env-0.28.1.240417/docker/opp_env_distro_uninstall.cmd
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-17 12:57:06.000000 opp_env-0.28.1.240417/docker/profile
--rwxr-xr-x   0 runner    (1001) docker     (127)       53 2024-04-17 12:57:06.000000 opp_env-0.28.1.240417/docker/run
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-17 12:57:06.000000 opp_env-0.28.1.240417/docker/wsl.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:57:14.797293 opp_env-0.28.1.240417/misc/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1558 2024-04-17 12:57:06.000000 opp_env-0.28.1.240417/misc/make_patch_release
--rwxr-xr-x   0 runner    (1001) docker     (127)     2574 2024-04-17 12:57:06.000000 opp_env-0.28.1.240417/misc/make_patch_release_windows
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:57:14.797293 opp_env-0.28.1.240417/opp_env/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 12:57:06.000000 opp_env-0.28.1.240417/opp_env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-17 12:57:06.000000 opp_env-0.28.1.240417/opp_env/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-17 12:57:14.000000 opp_env-0.28.1.240417/opp_env/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:57:14.801293 opp_env-0.28.1.240417/opp_env/database/
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-17 12:57:06.000000 opp_env-0.28.1.240417/opp_env/database/external.json
--rw-r--r--   0 runner    (1001) docker     (127)   101545 2024-04-17 12:57:06.000000 opp_env-0.28.1.240417/opp_env/database/external.py
--rw-r--r--   0 runner    (1001) docker     (127)    18765 2024-04-17 12:57:06.000000 opp_env-0.28.1.240417/opp_env/database/inet.py
--rw-r--r--   0 runner    (1001) docker     (127)    30899 2024-04-17 12:57:06.000000 opp_env-0.28.1.240417/opp_env/database/omnetpp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-17 12:57:06.000000 opp_env-0.28.1.240417/opp_env/database/simu5g.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-17 12:57:06.000000 opp_env-0.28.1.240417/opp_env/database/simulte.py
--rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-04-17 12:57:06.000000 opp_env-0.28.1.240417/opp_env/database/veins.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    97506 2024-04-17 12:57:06.000000 opp_env-0.28.1.240417/opp_env/opp_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:57:14.793293 opp_env-0.28.1.240417/opp_env/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:57:14.793293 opp_env-0.28.1.240417/opp_env/templates/workspace/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:57:14.801293 opp_env-0.28.1.240417/opp_env/templates/workspace/22.11/
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-17 12:57:06.000000 opp_env-0.28.1.240417/opp_env/templates/workspace/22.11/flake.lock
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:57:14.801293 opp_env-0.28.1.240417/opp_env/templates/workspace/23.05/
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-17 12:57:06.000000 opp_env-0.28.1.240417/opp_env/templates/workspace/23.05/flake.lock
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:57:14.801293 opp_env-0.28.1.240417/opp_env.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11519 2024-04-17 12:57:14.000000 opp_env-0.28.1.240417/opp_env.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-17 12:57:14.000000 opp_env-0.28.1.240417/opp_env.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 12:57:14.000000 opp_env-0.28.1.240417/opp_env.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-17 12:57:14.000000 opp_env-0.28.1.240417/opp_env.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-17 12:57:14.000000 opp_env-0.28.1.240417/opp_env.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-17 12:57:14.000000 opp_env-0.28.1.240417/opp_env.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-17 12:57:06.000000 opp_env-0.28.1.240417/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-17 12:57:06.000000 opp_env-0.28.1.240417/setenv
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 12:57:14.801293 opp_env-0.28.1.240417/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-17 12:57:06.000000 opp_env-0.28.1.240417/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:57:14.801293 opp_env-0.28.1.240417/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-17 12:57:06.000000 opp_env-0.28.1.240417/tests/download_all.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      107 2024-04-17 12:57:06.000000 opp_env-0.28.1.240417/tests/test_external_build
--rwxr-xr-x   0 runner    (1001) docker     (127)       69 2024-04-17 12:57:06.000000 opp_env-0.28.1.240417/tests/test_inet_build
--rwxr-xr-x   0 runner    (1001) docker     (127)       72 2024-04-17 12:57:06.000000 opp_env-0.28.1.240417/tests/test_omnetpp_build
--rwxr-xr-x   0 runner    (1001) docker     (127)      270 2024-04-17 12:57:06.000000 opp_env-0.28.1.240417/tests/test_opp_env_project
--rwxr-xr-x   0 runner    (1001) docker     (127)     4485 2024-04-17 12:57:06.000000 opp_env-0.28.1.240417/tests/test_oppenv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:53:12.812307 opp_env-0.29.0.240422/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:53:12.804307 opp_env-0.29.0.240422/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:53:12.808307 opp_env-0.29.0.240422/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-22 15:53:08.000000 opp_env-0.29.0.240422/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-22 15:53:08.000000 opp_env-0.29.0.240422/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-04-22 15:53:08.000000 opp_env-0.29.0.240422/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-22 15:53:08.000000 opp_env-0.29.0.240422/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8885 2024-04-22 15:53:12.812307 opp_env-0.29.0.240422/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7324 2024-04-22 15:53:08.000000 opp_env-0.29.0.240422/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:53:12.808307 opp_env-0.29.0.240422/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-22 15:53:08.000000 opp_env-0.29.0.240422/docker/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-22 15:53:08.000000 opp_env-0.29.0.240422/docker/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (127)       66 2024-04-22 15:53:08.000000 opp_env-0.29.0.240422/docker/build
+-rwxr-xr-x   0 runner    (1001) docker     (127)      155 2024-04-22 15:53:08.000000 opp_env-0.29.0.240422/docker/build-wsl-image
+-rwxr-xr-x   0 runner    (1001) docker     (127)      268 2024-04-22 15:53:08.000000 opp_env-0.29.0.240422/docker/entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-22 15:53:08.000000 opp_env-0.29.0.240422/docker/nix.conf
+-rwxr-xr-x   0 runner    (1001) docker     (127)       54 2024-04-22 15:53:08.000000 opp_env-0.29.0.240422/docker/opp_env.cmd
+-rwxr-xr-x   0 runner    (1001) docker     (127)       24 2024-04-22 15:53:08.000000 opp_env-0.29.0.240422/docker/opp_env_distro.cmd
+-rwxr-xr-x   0 runner    (1001) docker     (127)      131 2024-04-22 15:53:08.000000 opp_env-0.29.0.240422/docker/opp_env_distro_install.cmd
+-rwxr-xr-x   0 runner    (1001) docker     (127)      103 2024-04-22 15:53:08.000000 opp_env-0.29.0.240422/docker/opp_env_distro_uninstall.cmd
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-22 15:53:08.000000 opp_env-0.29.0.240422/docker/profile
+-rwxr-xr-x   0 runner    (1001) docker     (127)       53 2024-04-22 15:53:08.000000 opp_env-0.29.0.240422/docker/run
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-22 15:53:08.000000 opp_env-0.29.0.240422/docker/wsl.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:53:12.808307 opp_env-0.29.0.240422/misc/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1558 2024-04-22 15:53:08.000000 opp_env-0.29.0.240422/misc/make_patch_release
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2574 2024-04-22 15:53:08.000000 opp_env-0.29.0.240422/misc/make_patch_release_windows
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:53:12.808307 opp_env-0.29.0.240422/opp_env/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 15:53:08.000000 opp_env-0.29.0.240422/opp_env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-22 15:53:08.000000 opp_env-0.29.0.240422/opp_env/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-22 15:53:12.000000 opp_env-0.29.0.240422/opp_env/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:53:12.812307 opp_env-0.29.0.240422/opp_env/database/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-22 15:53:08.000000 opp_env-0.29.0.240422/opp_env/database/external.json
+-rw-r--r--   0 runner    (1001) docker     (127)   135486 2024-04-22 15:53:08.000000 opp_env-0.29.0.240422/opp_env/database/external.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19321 2024-04-22 15:53:08.000000 opp_env-0.29.0.240422/opp_env/database/inet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30899 2024-04-22 15:53:08.000000 opp_env-0.29.0.240422/opp_env/database/omnetpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-22 15:53:08.000000 opp_env-0.29.0.240422/opp_env/database/simu5g.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-22 15:53:08.000000 opp_env-0.29.0.240422/opp_env/database/simulte.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6875 2024-04-22 15:53:08.000000 opp_env-0.29.0.240422/opp_env/database/veins.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    96030 2024-04-22 15:53:08.000000 opp_env-0.29.0.240422/opp_env/opp_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:53:12.804307 opp_env-0.29.0.240422/opp_env/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:53:12.804307 opp_env-0.29.0.240422/opp_env/templates/workspace/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:53:12.812307 opp_env-0.29.0.240422/opp_env/templates/workspace/22.11/
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-22 15:53:08.000000 opp_env-0.29.0.240422/opp_env/templates/workspace/22.11/flake.lock
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:53:12.812307 opp_env-0.29.0.240422/opp_env/templates/workspace/23.05/
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-22 15:53:08.000000 opp_env-0.29.0.240422/opp_env/templates/workspace/23.05/flake.lock
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:53:12.812307 opp_env-0.29.0.240422/opp_env.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8885 2024-04-22 15:53:12.000000 opp_env-0.29.0.240422/opp_env.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-22 15:53:12.000000 opp_env-0.29.0.240422/opp_env.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 15:53:12.000000 opp_env-0.29.0.240422/opp_env.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-22 15:53:12.000000 opp_env-0.29.0.240422/opp_env.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-22 15:53:12.000000 opp_env-0.29.0.240422/opp_env.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-22 15:53:08.000000 opp_env-0.29.0.240422/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-22 15:53:08.000000 opp_env-0.29.0.240422/setenv
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 15:53:12.812307 opp_env-0.29.0.240422/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-22 15:53:08.000000 opp_env-0.29.0.240422/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:53:12.812307 opp_env-0.29.0.240422/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-22 15:53:08.000000 opp_env-0.29.0.240422/tests/download_all.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      107 2024-04-22 15:53:08.000000 opp_env-0.29.0.240422/tests/test_external_build
+-rwxr-xr-x   0 runner    (1001) docker     (127)       69 2024-04-22 15:53:08.000000 opp_env-0.29.0.240422/tests/test_inet_build
+-rwxr-xr-x   0 runner    (1001) docker     (127)       72 2024-04-22 15:53:08.000000 opp_env-0.29.0.240422/tests/test_omnetpp_build
+-rwxr-xr-x   0 runner    (1001) docker     (127)      270 2024-04-22 15:53:08.000000 opp_env-0.29.0.240422/tests/test_opp_env_project
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4485 2024-04-22 15:53:08.000000 opp_env-0.29.0.240422/tests/test_oppenv
```

### Comparing `opp_env-0.28.1.240417/.github/workflows/publish-to-pypi.yml` & `opp_env-0.29.0.240422/.github/workflows/publish-to-pypi.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: Publish Python 🐍 distribution 📦 to PyPI and TestPyPI
+name: Publish opp_env Python distribution to PyPI
 
 on: push
 
 jobs:
   build:
     name: Build distribution 📦
     runs-on: ubuntu-latest
@@ -23,38 +23,14 @@
       run: python3 -m build
     - name: Store the distribution packages
       uses: actions/upload-artifact@v3
       with:
         name: python-package-distributions
         path: dist/
 
-  publish-to-testpypi:
-    name: Publish Python 🐍 distribution 📦 to TestPyPI
-    needs:
-    - build
-    runs-on: ubuntu-latest
-
-    environment:
-      name: testpypi
-      url: https://test.pypi.org/p/opp-env
-
-    permissions:
-      id-token: write  # IMPORTANT: mandatory for trusted publishing
-
-    steps:
-    - name: Download all the dists
-      uses: actions/download-artifact@v3
-      with:
-        name: python-package-distributions
-        path: dist/
-    - name: Publish distribution 📦 to TestPyPI
-      uses: pypa/gh-action-pypi-publish@release/v1
-      with:
-        repository-url: https://test.pypi.org/legacy/
-
   publish-to-pypi:
     name: >-
       Publish Python 🐍 distribution 📦 to PyPI
     if: startsWith(github.ref, 'refs/tags/')  # only publish to PyPI on tag pushes
     needs:
     - build
     runs-on: ubuntu-latest
```

### Comparing `opp_env-0.28.1.240417/LICENSE` & `opp_env-0.29.0.240422/LICENSE`

 * *Files identical despite different names*

### Comparing `opp_env-0.28.1.240417/PKG-INFO` & `opp_env-0.29.0.240422/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: opp_env
-Version: 0.28.1.240417
+Version: 0.29.0.240422
 Summary: A tool, that sets up the development environment for OMNeT++ projects
 Author-email: András Varga <andras@omnetpp.org>, Levente Mészáros <levy@omnetpp.org>, Rudolf Hornig <rudi@omnetpp.org>
 Maintainer-email: Rudolf Hornig <rudi@omnetpp.org>
 Project-URL: Homepage, https://omnetpp.org
 Project-URL: Documentation, https://github.com/omnetpp/opp_env/blob/main/README.md
+Project-URL: Changes, https://github.com/omnetpp/opp_env/blob/main/CHANGES.md
 Project-URL: Repository, https://github.com/omnetpp/opp_env
 Project-URL: Issues, https://github.com/omnetpp/opp_env/issues
 Project-URL: Changelog, https://github.com/omnetpp/opp_env/commits/main
 Keywords: omnetpp,omnest,simulation,discrete,event,package manager,model
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
@@ -20,19 +21,17 @@
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Topic :: Education
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Software Distribution
-Requires-Python: >=3.11
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pip>=23.0.0
-Requires-Dist: packaging
 
 # opp_env: Automated Installation of OMNeT++ Simulation Frameworks
 
 `opp_env` is a powerful tool that allows for the easy and automated installation
 of OMNeT++ simulation frameworks and models, including dependencies like INET
 Framework and OMNeT++ itself. It can install any version of OMNeT++ and INET, as
 well as currently selected versions of Veins, SimuLTE, Simu5G and other models.
@@ -215,64 +214,7 @@
 
 Once you have `build` installed, you can build the package by running:
 
     python3 -m build
 
 If you have any issues or questions, feel free to open an issue on the GitHub
 repository. We are always happy to help!
-
-## Supported Simulation Frameworks
-
-As of version 0.25.0 of `opp_env`, the following simulation frameworks are
-supported:
-
-```
-$ opp_env list
-
-omnetpp                  6.0.2  6.0.1  6.0.0  5.7.1  5.7.0  5.6.3  5.6.2  5.6.1  5.6.0  5.5.2  5.5.1  5.5.0  5.4.2  5.4.1  5.4.0  5.3.1  5.3.0  5.2.2  5.2.1  5.2.0  5.1.2  5.1.1  5.1.0  5.0.1  5.0.0  4.6.1 4.6.0  4.5.1  4.5.0  4.4.2  4.4.1  4.4.0  4.3.2  4.3.1  4.3.0  4.2.3  4.2.2  4.2.1  4.2.0  4.1.1  4.1.0  4.0.2  4.0.1  3.3.2  3.3.1  6.0.x  5.7.x  5.6.x  5.5.x  5.4.x  5.3.x  5.2.x  5.1.x  5.0.x  4.6.x  4.5.x  4.4.x  4.3.x  4.2.x  4.1.x  4.0.x  3.3.x  master
-inet                     4.5.2  4.5.1  4.5.0  4.4.1  4.4.0  4.3.9  4.3.8  4.3.7  4.2.10  4.2.9  4.2.8  4.2.7  4.2.6  4.2.5  4.2.4  4.2.3  4.2.2  4.2.1  4.2.0  4.1.2  4.1.1  4.1.0  4.0.0  3.8.3  3.8.2  3.8.13.8.0  3.7.1  3.7.0  3.6.8  3.6.7  3.6.6  3.6.5  3.6.4  3.6.3  3.6.2  3.6.1  3.6.0  3.5.x  3.5.0  3.4.0  3.3.0  3.2.4  3.2.3  3.2.2  3.2.1  3.2.0  3.1.x  3.1.1  3.1.0  3.0.x  3.0.0  2.6.x  2.6.0  2.5.x  2.5.0  2.4.x  2.4.0  2.3.x  2.3.0  2.2.x  2.2.0  2.1.x  2.1.0  2.0.x  2.0.0  20100323  20061020  master
-afdx                     20220904
-ansa                     inet3.4.0
-can_allinone             0.1.0
-castalia                 3.3  3.2
-cell                     20140729
-chaosmanager             20221210
-core4inet                221109
-dctrafficgen             20181016
-fico4omnet               20210113
-flora                    1.1.0
-gptp                     20200311
-gradys                   0.5
-hnocs                    20221212
-icancloud                1.0
-ieee802154standalone     20180310
-inet_hnrl                20170217
-inetgpl                  1.0
-inetmanet                4.0.0  3.8.2
-lora_icn                 paper
-lre_omnet                1.0.1
-mixim                    2.3
-nesting                  0.9.1
-omnet_tdma               1.0.2
-opencv2x_veins           1.4.1
-oppbsd                   4.0
-ops_allinone             20230331
-opslite                  20190624
-os3                      1.0
-oversim                  20190424
-quisp                    20230807
-rease                    20130819
-rinasim                  20200903
-rspsim                   6.1.2
-seapp                    20191230
-sedencontroller_allinone 20230305
-simcan                   1.2
-simproctc                2.0.2
-simu5g                   1.2.2  1.2.1  1.1.0
-simulte                  1.2.0  1.1.0  0.9.1
-solarleach               1.01
-stochasticbattery        20170224
-swim_allinone            20180221
-tsch_allinone            6tisch_paper
-veins                    5.2  5.1  5.0  4.7.1  4.7  4.6  4.4  4.3  3.0  master
-wifidirect_allinone      3.4
-```
```

### Comparing `opp_env-0.28.1.240417/README.md` & `opp_env-0.29.0.240422/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -183,64 +183,7 @@
 
 Once you have `build` installed, you can build the package by running:
 
     python3 -m build
 
 If you have any issues or questions, feel free to open an issue on the GitHub
 repository. We are always happy to help!
-
-## Supported Simulation Frameworks
-
-As of version 0.25.0 of `opp_env`, the following simulation frameworks are
-supported:
-
-```
-$ opp_env list
-
-omnetpp                  6.0.2  6.0.1  6.0.0  5.7.1  5.7.0  5.6.3  5.6.2  5.6.1  5.6.0  5.5.2  5.5.1  5.5.0  5.4.2  5.4.1  5.4.0  5.3.1  5.3.0  5.2.2  5.2.1  5.2.0  5.1.2  5.1.1  5.1.0  5.0.1  5.0.0  4.6.1 4.6.0  4.5.1  4.5.0  4.4.2  4.4.1  4.4.0  4.3.2  4.3.1  4.3.0  4.2.3  4.2.2  4.2.1  4.2.0  4.1.1  4.1.0  4.0.2  4.0.1  3.3.2  3.3.1  6.0.x  5.7.x  5.6.x  5.5.x  5.4.x  5.3.x  5.2.x  5.1.x  5.0.x  4.6.x  4.5.x  4.4.x  4.3.x  4.2.x  4.1.x  4.0.x  3.3.x  master
-inet                     4.5.2  4.5.1  4.5.0  4.4.1  4.4.0  4.3.9  4.3.8  4.3.7  4.2.10  4.2.9  4.2.8  4.2.7  4.2.6  4.2.5  4.2.4  4.2.3  4.2.2  4.2.1  4.2.0  4.1.2  4.1.1  4.1.0  4.0.0  3.8.3  3.8.2  3.8.13.8.0  3.7.1  3.7.0  3.6.8  3.6.7  3.6.6  3.6.5  3.6.4  3.6.3  3.6.2  3.6.1  3.6.0  3.5.x  3.5.0  3.4.0  3.3.0  3.2.4  3.2.3  3.2.2  3.2.1  3.2.0  3.1.x  3.1.1  3.1.0  3.0.x  3.0.0  2.6.x  2.6.0  2.5.x  2.5.0  2.4.x  2.4.0  2.3.x  2.3.0  2.2.x  2.2.0  2.1.x  2.1.0  2.0.x  2.0.0  20100323  20061020  master
-afdx                     20220904
-ansa                     inet3.4.0
-can_allinone             0.1.0
-castalia                 3.3  3.2
-cell                     20140729
-chaosmanager             20221210
-core4inet                221109
-dctrafficgen             20181016
-fico4omnet               20210113
-flora                    1.1.0
-gptp                     20200311
-gradys                   0.5
-hnocs                    20221212
-icancloud                1.0
-ieee802154standalone     20180310
-inet_hnrl                20170217
-inetgpl                  1.0
-inetmanet                4.0.0  3.8.2
-lora_icn                 paper
-lre_omnet                1.0.1
-mixim                    2.3
-nesting                  0.9.1
-omnet_tdma               1.0.2
-opencv2x_veins           1.4.1
-oppbsd                   4.0
-ops_allinone             20230331
-opslite                  20190624
-os3                      1.0
-oversim                  20190424
-quisp                    20230807
-rease                    20130819
-rinasim                  20200903
-rspsim                   6.1.2
-seapp                    20191230
-sedencontroller_allinone 20230305
-simcan                   1.2
-simproctc                2.0.2
-simu5g                   1.2.2  1.2.1  1.1.0
-simulte                  1.2.0  1.1.0  0.9.1
-solarleach               1.01
-stochasticbattery        20170224
-swim_allinone            20180221
-tsch_allinone            6tisch_paper
-veins                    5.2  5.1  5.0  4.7.1  4.7  4.6  4.4  4.3  3.0  master
-wifidirect_allinone      3.4
-```
```

### Comparing `opp_env-0.28.1.240417/docker/Dockerfile` & `opp_env-0.29.0.240422/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `opp_env-0.28.1.240417/docker/profile` & `opp_env-0.29.0.240422/docker/profile`

 * *Files identical despite different names*

### Comparing `opp_env-0.28.1.240417/misc/make_patch_release` & `opp_env-0.29.0.240422/misc/make_patch_release`

 * *Files identical despite different names*

### Comparing `opp_env-0.28.1.240417/misc/make_patch_release_windows` & `opp_env-0.29.0.240422/misc/make_patch_release_windows`

 * *Files identical despite different names*

### Comparing `opp_env-0.28.1.240417/opp_env/database/inet.py` & `opp_env-0.29.0.240422/opp_env/database/inet.py`

 * *Files 4% similar despite different names*

```diff
@@ -158,29 +158,29 @@
         ["4.2.6", ["5.7.*"]],
         ["4.2.5", ["5.6.*", "5.7.*"]],
         ["4.2.4", ["5.4.2", "5.4.1", "5.4.x", "5.5.*", "5.6.*", "5.7.*"]],
         ["4.2.3", ["5.4.2", "5.4.1", "5.4.x", "5.5.*", "5.6.*", "5.7.*"]],
         ["4.2.2", ["5.4.2", "5.4.1", "5.4.x", "5.5.*", "5.6.*", "5.7.*"]],
         ["4.2.1", ["5.4.2", "5.4.1", "5.4.x", "5.5.*", "5.6.*", "5.7.*"]],
         ["4.2.0", ["5.4.2", "5.4.1", "5.4.x", "5.5.*", "5.6.*", "5.7.*"]],
-        ["4.1.2", ["5.4.2", "5.4.1", "5.4.x", "5.5.*", "5.6.*", "5.7.*"]],
-        ["4.1.1", ["5.4.2", "5.4.1", "5.4.x", "5.5.*", "5.6.*", "5.7.*"]],
+        ["4.1.2", ["5.4.2", "5.4.1", "5.4.x", "5.5.*"]], # with omnetpp-5.6.*, omnetpp-5.7.*: error: Direct deletion of a module is illegal, use deleteModule() instead
+        ["4.1.1", ["5.4.2", "5.4.1", "5.4.x", "5.5.*"]], # with omnetpp-5.6.*, omnetpp-5.7.*: error: Direct deletion of a module is illegal, use deleteModule() instead
         ["4.1.0", ["5.4.2", "5.4.1", "5.4.x"]], # with omnetpp-5.5.1: error: PacketQueue.cc:23: cPacketQueue constructor call is ambiguous
         ["4.0.0", ["5.4.2", "5.4.1", "5.4.x"]], # with omnetpp-5.5.1: error: PacketQueue.cc:23: cPacketQueue constructor call is ambiguous
 
         ["3.8.3", ["5.7.*", "6.0.*"]],
         ["3.8.2", ["5.7.*", "6.0.*"]],
         ["3.8.1", ["5.7.*"]],
         ["3.8.0", ["5.7.*"]],
         ["3.7.1", ["5.3.*", "5.4.*", "5.5.*", "5.6.*", "5.7.*"]],
         ["3.7.0", ["5.3.*", "5.4.*", "5.5.*", "5.6.*", "5.7.*"]],
         ["3.6.8", ["5.3.*", "5.4.*", "5.5.*", "5.6.*", "5.7.*"]],
-        ["3.6.7", ["5.3.*", "5.4.*", "5.5.*", "5.6.*", "5.7.*"]],
-        ["3.6.6", ["5.3.*", "5.4.*", "5.5.*", "5.6.*", "5.7.*"]],
-        ["3.6.5", ["5.3.*", "5.4.*", "5.5.*", "5.6.*", "5.7.*"]],
+        ["3.6.7", ["5.3.*", "5.4.*", "5.5.*"]], # with omnetpp-5.6.*, omnetpp-5.7.*: error: Direct deletion of a module is illegal, use deleteModule() instead
+        ["3.6.6", ["5.3.*", "5.4.*", "5.5.*"]], # with omnetpp-5.6.*, omnetpp-5.7.*: error: Direct deletion of a module is illegal, use deleteModule() instead
+        ["3.6.5", ["5.3.*", "5.4.*", "5.5.*"]], # with omnetpp-5.6.*, omnetpp-5.7.*: error: Direct deletion of a module is illegal, use deleteModule() instead
         ["3.6.4", ["5.1.*", "5.2.*", "5.3.*", "5.4.*"]], # note: this adds support for changed cMessagePrinter API in omnetpp-5.3; omnetpp-5.5 fails due to cPacketQueue constructor ambiguity
         ["3.6.3", ["5.1.*", "5.2.*"]], # with with omnetpp-5.3: error due to cMessagePrinter::printMessage() interface change
         ["3.6.2", ["5.1.*", "5.2.*"]], # with with omnetpp-5.3: error due to cMessagePrinter::printMessage() interface change
         ["3.6.1", ["5.1.*", "5.2.*"]], # with with omnetpp-5.3: error due to cMessagePrinter::printMessage() interface change
         ["3.6.0", ["5.1.*"]], # with omnetpp-5.2: Ieee80211ControlInfoDescr.h:16:6: error: Version mismatch! Probably this file was generated by an earlier version of nedtool
         ["3.5.x", ["5.1.*"]],
         ["3.5.0", ["5.1.*"]],
@@ -218,25 +218,26 @@
     return [
         *get_all_inet_released_versions(),
         inet_20100323, inet_20061020, # hand-picked time-stamped versions
         make_inet_project_description("master", ["6.0.*"]),
     ]
 
 inet_20100323 = {
+    # release only, because dependent projects (such as quagga) link with the release mode lib
     "name": "inet", "version": "20100323",
     "required_projects": {"omnetpp": ["4.1.0"]},        # TODO: try with 4.1.* -> build error
     "download_url": "https://github.com/inet-framework/inet/releases/download/master_20100323/inet-20100323-src.tgz",
     "patch_commands": [
         "sed -i 's|  int octals\\[8\\] = |  unsigned int octals[8] = |' src/networklayer/contract/IPv6Address.cc",
         "sed -i 's|findGap(int \\*octals|findGap(unsigned int *octals|' src/networklayer/contract/IPv6Address.cc",
         "sed -i 's|machine/endian|endian|' src/util/headerserializers/headers/defs.h",
         "sed -i 's|info\\[\\]|info[0]|' src/util/headerserializers/headers/sctp.h",
         "sed -i 's|addr.sin_len|// addr.sin_len|' src/linklayer/ext/*.cc",  # ugly hack? this is needed on apple
     ],
-    "build_commands": ["make makefiles && make -j$NIX_BUILD_CORES MODE=$BUILD_MODE"],
+    "build_commands": ["make makefiles && make -j$NIX_BUILD_CORES MODE=release"],
     "clean_commands": ["make clean"],
 }
 
 inet_20061020 = {
     "name": "inet", "version": "20061020",
     "required_projects": {"omnetpp": ["3.3.1"]},        # TODO try with 3.3.* -> build error
     "download_url": "https://github.com/inet-framework/inet/releases/download/v1.x/INET-20061020-src.tgz",
```

### Comparing `opp_env-0.28.1.240417/opp_env/database/omnetpp.py` & `opp_env-0.29.0.240422/opp_env/database/omnetpp.py`

 * *Files identical despite different names*

### Comparing `opp_env-0.28.1.240417/opp_env/database/simu5g.py` & `opp_env-0.29.0.240422/opp_env/database/simu5g.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,21 @@
     return {
         "name": "simu5g", "version": simu5g_version,
         "description": "5G NR and LTE/LTE-A user-plane simulation model",
         "metadata": {
             "catalog_url": "https://omnetpp.org/download-items/Simu5G.html",
         },
         "required_projects": {"inet": inet_versions, "omnetpp": omnetpp_versions},
+        "smoke_test_commands": [
+            "cd simulations/LTE/demo" if simu5g_version >= "1.2.1" else "cd simulations/demo",
+            "SIMU5G_EMULATION_ROOT=$SIMU5G_ROOT/emulation" if simu5g_version >= "1.2.1" else ""
+            """if [ "$BUILD_MODE" = "debug" ]; then BUILD_MODE_SUFFIX="_dbg"; fi""",
+            """if [ "$BUILD_MODE" = "release" ]; then BUILD_MODE_SUFFIX=""; fi""",
+            "opp_run$BUILD_MODE_SUFFIX -l $SIMU5G_ROOT/src/simu5g -l $INET_ROOT/src/INET -n $SIMU5G_ROOT/simulations:$SIMU5G_EMULATION_ROOT:$SIMU5G_ROOT/src:$INET_ROOT/src -c VideoStreaming -r 0 -u Cmdenv --sim-time-limit=10s > /dev/null",
+        ],
         "download_url": f"https://github.com/Unipisa/Simu5G/archive/refs/tags/v{simu5g_version}.tar.gz",
         "patch_commands": [
             "sed -i -E 's|-KINET_PROJ=[^ ]+|-KINET_PROJ=$(INET_ROOT)|' Makefile",
             "sed -i -E 's|^INET_SRC=.*|INET_SRC=$INET_ROOT/src|' bin/simu5g",
             "find . -name omnetpp.ini | xargs -n1 sed -i -E 's|^image-path|#image-path|'", # we use OMNETPP_IMAGE_PATH instead
         ],
         "setenv_commands": [
```

### Comparing `opp_env-0.28.1.240417/opp_env/database/simulte.py` & `opp_env-0.29.0.240422/opp_env/database/simulte.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,14 +6,22 @@
         "metadata": {
             "catalog_url": "https://omnetpp.org/download-items/SimuLTE.html",
         },
         "required_projects": {"inet": inet_versions, "omnetpp": omnetpp_versions},
         "download_url":
             f"https://github.com/inet-framework/simulte/releases/download/v{simulte_version}/simulte-{simulte_version}-src.tgz" if simulte_version == "1.2.0" else
             f"https://github.com/inet-framework/simulte/archive/refs/tags/v{simulte_version}.tar.gz",
+        "smoke_test_commands": [
+            "cd simulations/demo",
+            """if [ "$BUILD_MODE" = "debug" ]; then SIMULTE_LIB=$(echo $SIMULTE_ROOT/out/*-debug/src/*lte*); fi""",
+            """if [ "$BUILD_MODE" = "debug" ]; then BUILD_MODE_SUFFIX="_dbg"; fi""" if simulte_version >= "1.1.0" else """if [ "$BUILD_MODE" = "debug" ]; then BUILD_MODE_SUFFIX=""; fi""",
+            """if [ "$BUILD_MODE" = "release" ]; then SIMULTE_LIB=$(echo $SIMULTE_ROOT/out/*-release/src/*lte*); BUILD_MODE_SUFFIX=""; fi""",
+            """if [ "$BUILD_MODE" = "release" ]; then BUILD_MODE_SUFFIX=""; fi""" if simulte_version >= "1.1.0" else """if [ "$BUILD_MODE" = "release" ]; then BUILD_MODE_SUFFIX="_release"; fi""",
+            "opp_run$BUILD_MODE_SUFFIX -l $SIMULTE_LIB -n $SIMULTE_ROOT/simulations:$SIMULTE_ROOT/src:$INET_ROOT/src -c VideoStreaming -r 0 -u Cmdenv --sim-time-limit=10s > /dev/null"
+        ],
         "patch_commands": [
             "sed -i -E 's|-KINET_PROJ=[^ ]+|-KINET_PROJ=$(INET_ROOT)|' Makefile",
             "sed -i -E 's|^INET_DIR=.*|INET_DIR=$INET_ROOT/src|' src/run_lte",
             "find . -name omnetpp.ini | xargs -n1 sed -i -E 's|^image-path|#image-path|'", # we use OMNETPP_IMAGE_PATH instead
         ],
         "setenv_commands": [
             'export OMNETPP_IMAGE_PATH="$OMNETPP_IMAGE_PATH:$SIMULTE_ROOT/images"',
```

### Comparing `opp_env-0.28.1.240417/opp_env/database/veins.py` & `opp_env-0.29.0.240422/opp_env/database/veins.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,14 +18,24 @@
         ],
         "setenv_commands": [
             'export OMNETPP_IMAGE_PATH="$OMNETPP_IMAGE_PATH:$VEINS_ROOT/images"',
             "export SUMO_ROOT=${pkgs.sumo}",
             "source setenv" if version >= "5.1" else "",
             "if [[ ! ($INET_VERSION < '4.0.0') ]]; then cd subprojects/veins_inet && source setenv; else cd subprojects/veins_inet3 && source setenv; fi" if version >= "5.1" else "",
         ],
+        "smoke_test_commands": [
+            # can't test 4.7.1 -> no sumo before 5.0
+            """if [ "$BUILD_MODE" = "debug" ]; then DEBUG_POSTFIX="-d"; fi""",
+            """if [ "$BUILD_MODE" = "release" ]; then DEBUG_POSTFIX=""; fi""",
+            "./sumo-launchd.py &> /dev/null & bg_pid=$! &> /dev/null",
+            "cd examples/veins && ./run $DEBUG_POSTFIX -c Default -u Cmdenv > /dev/null",
+            "export VEINS_INET_INI_CONFIG='-c plain'" if version >= "5.1" else "",
+            "if [[ ! ($INET_VERSION < '4.0.0') ]]; then cd ../../subprojects/veins_inet/examples/veins_inet && ./run $DEBUG_POSTFIX $VEINS_INET_INI_CONFIG -u Cmdenv > /dev/null; else cd ../../subprojects/veins_inet3/examples/veins_inet && ./run $DEBUG_POSTFIX -u Cmdenv > /dev/null; fi",
+            "kill $bg_pid &> /dev/null",
+        ] if version >= "5.0" else ["echo 'Skipping test because required sumo version is not available as a nix package.'"],
         "build_commands": [ 
             "./configure && make -j$NIX_BUILD_CORES MODE=$BUILD_MODE" if version >= "4.5" else "./configure --with-inet=$INET_ROOT && make -j$NIX_BUILD_CORES MODE=$BUILD_MODE",
             # this is a hack so that the veins_inet subproject's configure can query the inet version
             "cd $INET_ROOT && mkdir -p _scripts && echo 'echo $INET_VERSION' > _scripts/get_version && chmod +x _scripts/get_version && cd -" if version == "5.0" else "cd $INET_ROOT && mkdir -p _scripts && echo '#!/usr/bin/env sh\n\necho $INET_VERSION' > _scripts/get_version && chmod +x _scripts/get_version && cd -",
             "if [[ ! ($INET_VERSION < '4.0.0') ]]; then cd subprojects/veins_inet && ./configure --with-inet=$INET_ROOT --with-veins=$VEINS_ROOT && make -j$NIX_BUILD_CORES MODE=$BUILD_MODE; else cd subprojects/veins_inet3 && ./configure --with-inet=$INET_ROOT --with-veins=$VEINS_ROOT && make -j$NIX_BUILD_CORES MODE=$BUILD_MODE; fi" if version >= "5.0" else "",
             "cd subprojects/veins_inet && ./configure --with-inet=$INET_ROOT --with-veins=$VEINS_ROOT && make -j$NIX_BUILD_CORES MODE=$BUILD_MODE" if version >= "4.5" and version < "5.0" else "",
             ],
```

### Comparing `opp_env-0.28.1.240417/opp_env/opp_env.py` & `opp_env-0.29.0.240422/opp_env/opp_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import subprocess
 import sys
 import re
 import shutil
 import tempfile
 import importlib
 import importlib.metadata
-from packaging.version import Version
 import platform
 import urllib.request
 
 # make sure that this run-time version check is in synch with the metadata for python requirement in the project.toml file.
 if sys.version_info < (3,9):
     v = sys.version_info
     print(f"Python version 3.9 or above is required, the current one is {v.major}.{v.minor}.{v.micro} ({sys.executable}).") # e.g. str.removeprefix()
@@ -308,19 +307,14 @@
         "mode",
         "quiet",
         "no-isolated",
         "keep",
         "local"
     ])
 
-    subparser = subparsers.add_parser("upgrade", help="Upgrades opp_env to the latest version", description="Upgrades opp_env to the latest version")
-    subparser.add_argument("-n", "--dry-run", default=False, action='store_true', help="Test if an upgrade is available and simulate the upgrade without actually carrying out the installation")
-    subparser.add_argument("-c", "--check", default=False, action='store_true', help="Only test if an upgrade is available")
-    subparser.add_argument("--from-pypi", default=False, action='store_true', help="Use the latest version from PyPI instead of the latest version from the Git repository")
-
     subparser = subparsers.add_parser("maint", help="Maintenance functions", description="Maintenance functions")
     subparser.add_argument("-u", "--update-catalog", metavar="download-items-dir", dest="catalog_dir", help="Update the opp_env installation commands in the model catalog of omnetpp.org. The argument should point to the `download-items/` subdir of a checked-out copy of the https://github.com/omnetpp/omnetpp.org/ repository.")
 
     return parser
 
 def process_arguments():
     parser = create_arg_parser()
@@ -368,31 +362,14 @@
           
 To run a simulation model directly with the latest version of OMNeT++, run:
   opp_env run --install omnetpp-latest -c 'cd $OMNETPP_ROOT/samples/aloha;./aloha'""")
 
 def get_version():
     return importlib.metadata.version("opp_env")
 
-def get_latest_version_from_github():
-    try:
-        response = urllib.request.urlopen("https://api.github.com/repos/omnetpp/opp_env/git/refs/tags")
-        tag_refs = json.loads(response.read().decode('utf-8'))
-        tags = [ tag_ref['ref'].split('/')[-1] for tag_ref in tag_refs ]
-        return max([ tag for tag in tags if is_semver(tag)], key=natural_sort_key)
-    except Exception as e:
-        return None
-
-def get_latest_version_from_pypi():
-    try:
-        response = urllib.request.urlopen("https://pypi.org/pypi/opp_env/json")
-        json_data = json.loads(response.read().decode("utf-8"))
-        return json_data["info"]["version"]
-    except Exception as e:
-        return None
-
 def detect_nix():
     minimum_nix_version = "2.9"
     # check nix is installed
     try:
         _logger.debug(f"Running nix --version")
         result = subprocess.run(['nix', '--version'], stdout=subprocess.PIPE, stderr=subprocess.DEVNULL)
         output = result.stdout.decode('utf-8')
@@ -621,15 +598,15 @@
         version_to_project_dict = self.index[project_reference.name]
         return [v for v,p in version_to_project_dict.items() if p.version != v and p.version == project_reference.version]
 
     def get_project_description(self, project_reference):
         if type(project_reference) is str:
             project_reference = ProjectReference.parse(project_reference)
         if project_reference.name not in self.index:
-            raise Exception(f"Cannot resolve '{project_reference}': Unknown project '{project_reference.name}'")
+            raise Exception(f"Cannot resolve '{project_reference}': " + self.get_unknown_project_message(project_reference.name))
         if not project_reference.version:
             raise Exception(f"Which version of '{project_reference.name}' do you mean? (Use '{project_reference.name}-latest' for latest version)")
         project_description = self.index[project_reference.name].get(project_reference.version)
         if not project_description:
             raise Exception(f"Project '{project_reference.name}' has no version '{project_reference.version}'")
         if project_reference.version != project_description.version:
             _logger.debug(f"Resolved {cyan(project_reference)} as {cyan(project_description)}")
@@ -718,14 +695,30 @@
                 selected_project_descriptions = list(reversed(selected_project_descriptions))  # most derived project first, omnetpp last (usually)
                 if return_all:
                     result.append(selected_project_descriptions)
                 else:
                     return selected_project_descriptions
         return result
 
+    def get_unknown_project_message(self, project_name):
+        def jaccard_similarity(word1, word2):
+            set1 = set(word1)
+            set2 = set(word2)
+            intersection = len(set1.intersection(set2))
+            union = len(set1) + len(set2) - intersection
+            similarity = intersection / union if union != 0 else 0
+            return similarity
+        names = self.get_project_names()
+        most_similar =  max(names, key=lambda p: jaccard_similarity(project_name.lower(), p.lower()))
+        more_candidates = [p for p in names if p!=most_similar and (p.lower() in project_name.lower() or project_name.lower() in p.lower())]
+        if more_candidates:
+            return f"Unknown project '{project_name}'. Did you mean one of {[most_similar] + more_candidates}?"
+        else:
+            return f"Unknown project '{project_name}'. Did you mean '{most_similar}'?"
+
 def activate_project_options(project_descriptions, requested_options):
     # check requested options exist at all
     all_supported_options = []
     for desc in project_descriptions:
         all_supported_options += desc.get_supported_options()
     all_supported_options = uniq(all_supported_options)
     for option in requested_options or []:
@@ -1451,15 +1444,15 @@
         project_descriptions = []
         for project in projects:
             if '-' in project:
                 project_descriptions += [project_registry.get_project_description(ProjectReference.parse(project))]
             elif project in project_registry.get_project_names():
                 project_descriptions += [project_registry.get_project_description(ProjectReference(project, version)) for version in project_registry.get_project_versions(project)]
             else:
-                raise Exception(f"Unknown project name '{project}'")
+                raise Exception(project_registry.get_unknown_project_message(project))
 
     if raw:
         serializable = [vars(p.activate_project_options(requested_options)) for p in project_descriptions]
         print(json.dumps(serializable, indent=4))
         return
 
     # print info for each
@@ -1626,29 +1619,14 @@
 
     commands = ["build_all", command] if build or (install and not install_without_build) else [command]
 
     kind = "nixless" if workspace.nixless else "isolated" if isolated else "non-isolated"
     _logger.info(f"Running {'test ' if run_test else 'smoke_test ' if run_smoke_test else ''}command for projects {cyan(str(effective_project_descriptions))} in workspace {cyan(workspace.root_directory)} in {cyan(kind)} mode")
     workspace.nix_develop(effective_project_descriptions, workspace_directory, commands=commands, **dict(kwargs, suppress_stdout=False))
 
-def upgrade_subcommand_main(dry_run=False, from_pypi=False, check=False, **kwargs):
-    latest_version = get_latest_version_from_pypi() if from_pypi else get_latest_version_from_github()
-    version = get_version()
-    upgrade_needed = Version(version) < Version(latest_version)
-    _logger.info(f"An upgrade is available for opp_env" if upgrade_needed else f"opp_env is up-to-date")
-    _logger.info(f"Installed version: {cyan(version)}, latest version: {cyan(latest_version)}")
-    if check:
-        return
-    dry_run_option = "--dry-run" if dry_run else ""
-    module_spec = f"opp_env=={latest_version}" if from_pypi else f"git+https://github.com/omnetpp/opp_env.git@{latest_version}"
-    if upgrade_needed:
-        upgrade_command = f"pip3 install --user --upgrade --break-system-packages {dry_run_option} {module_spec}"
-        _logger.debug(f"Executing command: {upgrade_command}")
-        subprocess.run(["bash", "-c", upgrade_command])
-
 def maint_subcommand_main(catalog_dir, **kwargs):
     update_catalog(catalog_dir)
 
 def update_catalog(catalog_dir):
     # collect catalog URLs by project name
     _logger.info(f"Collecting catalog_url entries from projects")
     global project_registry
@@ -1701,16 +1679,14 @@
             init_subcommand_main(**kwargs)
         elif subcommand == "install":
             install_subcommand_main(**kwargs)
         elif subcommand == "shell":
             shell_subcommand_main(**kwargs)
         elif subcommand == "run":
             run_subcommand_main(**kwargs)
-        elif subcommand == "upgrade":
-            upgrade_subcommand_main(**kwargs)
         elif subcommand == "maint":
             maint_subcommand_main(**kwargs)
         else:
             raise Exception(f"Unknown subcommand '{subcommand}'")
         _logger.debug(f"The {cyan(subcommand)} operation completed successfully")
         return 0
     except Exception as e:
```

### Comparing `opp_env-0.28.1.240417/opp_env/templates/workspace/22.11/flake.lock` & `opp_env-0.29.0.240422/opp_env/templates/workspace/22.11/flake.lock`

 * *Files identical despite different names*

### Comparing `opp_env-0.28.1.240417/opp_env/templates/workspace/23.05/flake.lock` & `opp_env-0.29.0.240422/opp_env/templates/workspace/23.05/flake.lock`

 * *Files identical despite different names*

### Comparing `opp_env-0.28.1.240417/opp_env.egg-info/PKG-INFO` & `opp_env-0.29.0.240422/opp_env.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: opp_env
-Version: 0.28.1.240417
+Version: 0.29.0.240422
 Summary: A tool, that sets up the development environment for OMNeT++ projects
 Author-email: András Varga <andras@omnetpp.org>, Levente Mészáros <levy@omnetpp.org>, Rudolf Hornig <rudi@omnetpp.org>
 Maintainer-email: Rudolf Hornig <rudi@omnetpp.org>
 Project-URL: Homepage, https://omnetpp.org
 Project-URL: Documentation, https://github.com/omnetpp/opp_env/blob/main/README.md
+Project-URL: Changes, https://github.com/omnetpp/opp_env/blob/main/CHANGES.md
 Project-URL: Repository, https://github.com/omnetpp/opp_env
 Project-URL: Issues, https://github.com/omnetpp/opp_env/issues
 Project-URL: Changelog, https://github.com/omnetpp/opp_env/commits/main
 Keywords: omnetpp,omnest,simulation,discrete,event,package manager,model
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
@@ -20,19 +21,17 @@
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Topic :: Education
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Software Distribution
-Requires-Python: >=3.11
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pip>=23.0.0
-Requires-Dist: packaging
 
 # opp_env: Automated Installation of OMNeT++ Simulation Frameworks
 
 `opp_env` is a powerful tool that allows for the easy and automated installation
 of OMNeT++ simulation frameworks and models, including dependencies like INET
 Framework and OMNeT++ itself. It can install any version of OMNeT++ and INET, as
 well as currently selected versions of Veins, SimuLTE, Simu5G and other models.
@@ -215,64 +214,7 @@
 
 Once you have `build` installed, you can build the package by running:
 
     python3 -m build
 
 If you have any issues or questions, feel free to open an issue on the GitHub
 repository. We are always happy to help!
-
-## Supported Simulation Frameworks
-
-As of version 0.25.0 of `opp_env`, the following simulation frameworks are
-supported:
-
-```
-$ opp_env list
-
-omnetpp                  6.0.2  6.0.1  6.0.0  5.7.1  5.7.0  5.6.3  5.6.2  5.6.1  5.6.0  5.5.2  5.5.1  5.5.0  5.4.2  5.4.1  5.4.0  5.3.1  5.3.0  5.2.2  5.2.1  5.2.0  5.1.2  5.1.1  5.1.0  5.0.1  5.0.0  4.6.1 4.6.0  4.5.1  4.5.0  4.4.2  4.4.1  4.4.0  4.3.2  4.3.1  4.3.0  4.2.3  4.2.2  4.2.1  4.2.0  4.1.1  4.1.0  4.0.2  4.0.1  3.3.2  3.3.1  6.0.x  5.7.x  5.6.x  5.5.x  5.4.x  5.3.x  5.2.x  5.1.x  5.0.x  4.6.x  4.5.x  4.4.x  4.3.x  4.2.x  4.1.x  4.0.x  3.3.x  master
-inet                     4.5.2  4.5.1  4.5.0  4.4.1  4.4.0  4.3.9  4.3.8  4.3.7  4.2.10  4.2.9  4.2.8  4.2.7  4.2.6  4.2.5  4.2.4  4.2.3  4.2.2  4.2.1  4.2.0  4.1.2  4.1.1  4.1.0  4.0.0  3.8.3  3.8.2  3.8.13.8.0  3.7.1  3.7.0  3.6.8  3.6.7  3.6.6  3.6.5  3.6.4  3.6.3  3.6.2  3.6.1  3.6.0  3.5.x  3.5.0  3.4.0  3.3.0  3.2.4  3.2.3  3.2.2  3.2.1  3.2.0  3.1.x  3.1.1  3.1.0  3.0.x  3.0.0  2.6.x  2.6.0  2.5.x  2.5.0  2.4.x  2.4.0  2.3.x  2.3.0  2.2.x  2.2.0  2.1.x  2.1.0  2.0.x  2.0.0  20100323  20061020  master
-afdx                     20220904
-ansa                     inet3.4.0
-can_allinone             0.1.0
-castalia                 3.3  3.2
-cell                     20140729
-chaosmanager             20221210
-core4inet                221109
-dctrafficgen             20181016
-fico4omnet               20210113
-flora                    1.1.0
-gptp                     20200311
-gradys                   0.5
-hnocs                    20221212
-icancloud                1.0
-ieee802154standalone     20180310
-inet_hnrl                20170217
-inetgpl                  1.0
-inetmanet                4.0.0  3.8.2
-lora_icn                 paper
-lre_omnet                1.0.1
-mixim                    2.3
-nesting                  0.9.1
-omnet_tdma               1.0.2
-opencv2x_veins           1.4.1
-oppbsd                   4.0
-ops_allinone             20230331
-opslite                  20190624
-os3                      1.0
-oversim                  20190424
-quisp                    20230807
-rease                    20130819
-rinasim                  20200903
-rspsim                   6.1.2
-seapp                    20191230
-sedencontroller_allinone 20230305
-simcan                   1.2
-simproctc                2.0.2
-simu5g                   1.2.2  1.2.1  1.1.0
-simulte                  1.2.0  1.1.0  0.9.1
-solarleach               1.01
-stochasticbattery        20170224
-swim_allinone            20180221
-tsch_allinone            6tisch_paper
-veins                    5.2  5.1  5.0  4.7.1  4.7  4.6  4.4  4.3  3.0  master
-wifidirect_allinone      3.4
-```
```

### Comparing `opp_env-0.28.1.240417/opp_env.egg-info/SOURCES.txt` & `opp_env-0.29.0.240422/opp_env.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 .gitignore
+CHANGES.md
 LICENSE
 README.md
 pyproject.toml
 setenv
 setup.py
 .github/workflows/publish-to-pypi.yml
 docker/.dockerignore
@@ -24,15 +25,14 @@
 opp_env/__main__.py
 opp_env/_version.py
 opp_env/opp_env.py
 opp_env.egg-info/PKG-INFO
 opp_env.egg-info/SOURCES.txt
 opp_env.egg-info/dependency_links.txt
 opp_env.egg-info/entry_points.txt
-opp_env.egg-info/requires.txt
 opp_env.egg-info/top_level.txt
 opp_env/database/external.json
 opp_env/database/external.py
 opp_env/database/inet.py
 opp_env/database/omnetpp.py
 opp_env/database/simu5g.py
 opp_env/database/simulte.py
```

### Comparing `opp_env-0.28.1.240417/pyproject.toml` & `opp_env-0.29.0.240422/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -28,24 +28,22 @@
     "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
     "Topic :: Education",
     "Topic :: Software Development :: Build Tools",
     "Topic :: Software Development :: Libraries",
     "Topic :: System :: Software Distribution",
 ]
 readme = "README.md"
-requires-python = ">=3.11"
-dependencies = [
-    'pip >= 23.0.0',
-    'packaging',
-]
+requires-python = ">=3.9"
+dependencies = []
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://omnetpp.org"
 Documentation = "https://github.com/omnetpp/opp_env/blob/main/README.md"
+Changes = "https://github.com/omnetpp/opp_env/blob/main/CHANGES.md"
 Repository = "https://github.com/omnetpp/opp_env"
 Issues = "https://github.com/omnetpp/opp_env/issues"
 Changelog = "https://github.com/omnetpp/opp_env/commits/main"
 
 [project.optional-dependencies]
 
 [project.scripts]
```

### Comparing `opp_env-0.28.1.240417/setenv` & `opp_env-0.29.0.240422/setenv`

 * *Files identical despite different names*

### Comparing `opp_env-0.28.1.240417/tests/test_oppenv` & `opp_env-0.29.0.240422/tests/test_oppenv`

 * *Files identical despite different names*

