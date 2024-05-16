# Comparing `tmp/proxmox-grapple-1.5.3.tar.gz` & `tmp/proxmox-grapple-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxmox-grapple-1.5.3.tar", last modified: Fri Mar  1 06:18:08 2024, max compression
+gzip compressed data, was "proxmox-grapple-1.5.4.tar", last modified: Sat Mar  2 06:55:01 2024, max compression
```

## Comparing `proxmox-grapple-1.5.3.tar` & `proxmox-grapple-1.5.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2024-03-01 06:18:08.711083 proxmox-grapple-1.5.3/
--rw-r--r--   0 jason     (1000) jason     (1000)    35148 2024-02-29 22:39:55.000000 proxmox-grapple-1.5.3/LICENSE
--rw-r--r--   0 jason     (1000) jason     (1000)     2557 2024-03-01 06:18:08.711083 proxmox-grapple-1.5.3/PKG-INFO
--rw-r--r--   0 jason     (1000) jason     (1000)     1856 2024-03-01 06:14:09.000000 proxmox-grapple-1.5.3/README.md
--rw-r--r--   0 jason     (1000) jason     (1000)      948 2024-03-01 05:44:57.000000 proxmox-grapple-1.5.3/pyproject.toml
--rw-r--r--   0 jason     (1000) jason     (1000)       38 2024-03-01 06:18:08.711083 proxmox-grapple-1.5.3/setup.cfg
-drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2024-03-01 06:18:08.711083 proxmox-grapple-1.5.3/src/
-drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2024-03-01 06:18:08.711083 proxmox-grapple-1.5.3/src/proxmox_grapple/
--rw-r--r--   0 jason     (1000) jason     (1000)       22 2024-03-01 06:09:49.000000 proxmox-grapple-1.5.3/src/proxmox_grapple/__init__.py
--rw-r--r--   0 jason     (1000) jason     (1000)     1318 2024-02-29 22:39:55.000000 proxmox-grapple-1.5.3/src/proxmox_grapple/config.py
--rw-r--r--   0 jason     (1000) jason     (1000)     3688 2024-02-29 22:39:55.000000 proxmox-grapple-1.5.3/src/proxmox_grapple/vma_extractor.py
--rwxr-xr-x   0 jason     (1000) jason     (1000)     4882 2024-02-29 22:53:58.000000 proxmox-grapple-1.5.3/src/proxmox_grapple/vzdump_hook_script.py
-drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2024-03-01 06:18:08.711083 proxmox-grapple-1.5.3/src/proxmox_grapple.egg-info/
--rw-r--r--   0 jason     (1000) jason     (1000)     2557 2024-03-01 06:18:08.000000 proxmox-grapple-1.5.3/src/proxmox_grapple.egg-info/PKG-INFO
--rw-r--r--   0 jason     (1000) jason     (1000)      505 2024-03-01 06:18:08.000000 proxmox-grapple-1.5.3/src/proxmox_grapple.egg-info/SOURCES.txt
--rw-r--r--   0 jason     (1000) jason     (1000)        1 2024-03-01 06:18:08.000000 proxmox-grapple-1.5.3/src/proxmox_grapple.egg-info/dependency_links.txt
--rw-r--r--   0 jason     (1000) jason     (1000)       76 2024-03-01 06:18:08.000000 proxmox-grapple-1.5.3/src/proxmox_grapple.egg-info/entry_points.txt
--rw-r--r--   0 jason     (1000) jason     (1000)       47 2024-03-01 06:18:08.000000 proxmox-grapple-1.5.3/src/proxmox_grapple.egg-info/requires.txt
--rw-r--r--   0 jason     (1000) jason     (1000)       16 2024-03-01 06:18:08.000000 proxmox-grapple-1.5.3/src/proxmox_grapple.egg-info/top_level.txt
-drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2024-03-01 06:18:08.711083 proxmox-grapple-1.5.3/tests/
--rw-r--r--   0 jason     (1000) jason     (1000)     1409 2024-02-29 22:53:57.000000 proxmox-grapple-1.5.3/tests/test_script_runs.py
--rw-r--r--   0 jason     (1000) jason     (1000)      466 2024-02-29 22:39:55.000000 proxmox-grapple-1.5.3/tests/test_vzdump_hook_script_help_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-02 06:55:01.130774 proxmox-grapple-1.5.4/
+-rw-rw-rw-   0 root         (0) root         (0)    35148 2024-03-01 00:47:23.000000 proxmox-grapple-1.5.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3927 2024-03-02 06:55:01.130774 proxmox-grapple-1.5.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3226 2024-03-02 06:48:53.000000 proxmox-grapple-1.5.4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      948 2024-03-01 06:16:09.000000 proxmox-grapple-1.5.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-03-02 06:55:01.130774 proxmox-grapple-1.5.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-02 06:55:01.126774 proxmox-grapple-1.5.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-02 06:55:01.126774 proxmox-grapple-1.5.4/src/proxmox_grapple/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-03-02 06:48:53.000000 proxmox-grapple-1.5.4/src/proxmox_grapple/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1316 2024-03-02 06:48:53.000000 proxmox-grapple-1.5.4/src/proxmox_grapple/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3688 2024-03-01 00:47:23.000000 proxmox-grapple-1.5.4/src/proxmox_grapple/vma_extractor.py
+-rwxrwxrwx   0 root         (0) root         (0)     4882 2024-03-01 00:47:23.000000 proxmox-grapple-1.5.4/src/proxmox_grapple/vzdump_hook_script.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-02 06:55:01.126774 proxmox-grapple-1.5.4/src/proxmox_grapple.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3927 2024-03-02 06:55:01.000000 proxmox-grapple-1.5.4/src/proxmox_grapple.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      505 2024-03-02 06:55:01.000000 proxmox-grapple-1.5.4/src/proxmox_grapple.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-02 06:55:01.000000 proxmox-grapple-1.5.4/src/proxmox_grapple.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       76 2024-03-02 06:55:01.000000 proxmox-grapple-1.5.4/src/proxmox_grapple.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       47 2024-03-02 06:55:01.000000 proxmox-grapple-1.5.4/src/proxmox_grapple.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-03-02 06:55:01.000000 proxmox-grapple-1.5.4/src/proxmox_grapple.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-02 06:55:01.126774 proxmox-grapple-1.5.4/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1409 2024-03-01 00:47:23.000000 proxmox-grapple-1.5.4/tests/test_script_runs.py
+-rw-rw-rw-   0 root         (0) root         (0)      466 2024-03-01 00:47:23.000000 proxmox-grapple-1.5.4/tests/test_vzdump_hook_script_help_version.py
```

### Comparing `proxmox-grapple-1.5.3/LICENSE` & `proxmox-grapple-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `proxmox-grapple-1.5.3/PKG-INFO` & `proxmox-grapple-1.5.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxmox-grapple
-Version: 1.5.3
+Version: 1.5.4
 Summary: The grappling hook for Proxmox backups.
 Author-email: Jason Lingohr <jason@lucid.net.au>
 Project-URL: Homepage, https://github.com/lingfish/proxmox-grapple
 Project-URL: Issues, https://github.com/lingfish/proxmox-grapple/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
@@ -23,17 +23,48 @@
 The Python app that "hooks" into Proxmox.
 
 This is a clone of [vzdump-hook-script.pl](https://github.com/proxmox/pve-manager/blob/master/vzdump-hook-script.pl) that is
 written in Python, and that offers a lot more configurability.
 
 Different phases of the `vzdump` backup can be hooked into, and scripts can be run.
 
+<!-- TOC -->
+* [Proxmox-grapple](#proxmox-grapple)
+  * [Installation](#installation)
+  * [Configuration](#configuration)
+    * [Overview](#overview)
+    * [Location](#location)
+    * [Configuration environments](#configuration-environments)
+  * [Supported versions](#supported-versions)
+<!-- TOC -->
+
+## Installation
+
+The recommended way to install `proxmox-grapple` is to use [pipx](https://pipx.pypa.io/stable/).
+
+After getting `pipx` installed, simply run:
+
+```shell
+username@proxmox:~$ pipx install proxmox-grapple
+```
+
+Please, please [don't use pip system-wide](https://docs.python.org/3.11/installing/index.html#installing-into-the-system-python-on-linux).
+
+Once installed, you need to tell Proxmox (specifically `vzdump`) to use the app. Edit `/etc/vzdump.conf` and add or edit
+the `script` setting:
+
+```yaml
+script: /home/username/.local/bin/proxmox-grapple
+```
+
 
 ## Configuration
 
+### Overview
+
 `proxmox-grapple` is configured with a YAML-style file.  An example:
 
 ```yaml
 production:
   job-end:
     script:
       - echo 'hi'
@@ -45,44 +76,53 @@
     extract:
       enabled: false
       source_directory: /tmp
       destination_directory: /tmp
   #    exclude_storeids:
 ```
 
-The default location for the configuration is `/etc/proxmox_grapple.yml`, but this can also be specified on the
-commandline.
+### Location
+
+The default location for the configuration is `/etc/proxmox_grapple.yml`, or `proxmox_grapple.yml` in the current
+working directory, but this can also be specified on the commandline.
+
+If a non-absolute path is given, Dynaconf will iterate upwards: it will look at each parent up to the root of the
+system. For each visited folder, it will also try looking inside a `/config` folder.
+
+### Configuration environments
+
+It can also use different configuration settings based on arbitrary environment names (eg. `production`, `lab`, etc.) It
+uses the [Dynaconf](https://www.dynaconf.com/) Python project for configuration, so using environment variables to
+choose the environment and any other configuration option is possible.
+
+>⚠️ The default environment is `production`
 
-It can also use different configuration based on environments. It uses the [Dynaconf](https://www.dynaconf.com/) Python
-project for configuration, so using environment variables to choose the environment and any other configuration option is possible.
+For example, to choose a different configuration environment, set the environment variable `ENV_FOR_DYNACONF=lab`:
 
+```shell
+root@proxmox:~# ENV_FOR_DYNACONF=lab proxmox-grapple --dump-config
+```
 Each top-level key should match the different `vzdump` phases.  The currently recognised phases are:
 
 * job-init
 * job-start
 * job-end
 * job-abort
 * backup-start
 * backup-end
 * backup-abort
 * log-end
 * pre-stop
 * pre-restart
 * post-restart
 
-> [!NOTE]
-> The extract argument is currently not tested, and should be treated as a proof-of-concept only.
+>⚠️ The extract argument is currently not tested, and should be treated as a proof-of-concept only.
 
 
 ## Supported versions
 
 `proxmox-grapple` supports the following VE versions:
 
 | VE version | Debian version | Python version | VE EoL  |
 |------------|----------------|----------------|---------|
 | 8          | 12 (Bookworm)  | 3.11           | TBA     |
 | 7          | 11 (Bullseye)  | 3.9            | 2024-07 |
-
-
-## Installation
-
-The recommended way to install `proxmox-grapple` is to use [pipx](https://pipx.pypa.io/stable/).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `proxmox-grapple-1.5.3/pyproject.toml` & `proxmox-grapple-1.5.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `proxmox-grapple-1.5.3/src/proxmox_grapple/config.py` & `proxmox-grapple-1.5.4/src/proxmox_grapple/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dynaconf import Dynaconf, Validator
 
 settings = Dynaconf(
     settings_files=['proxmox_grapple.yml', '/etc/proxmox_grapple.yml'],
     environments=True,
-    # env='production',
+    env='production',
     apply_default_on_none=True,
     core_loaders=['YAML'],
     validators=[
         Validator('job-init', 'job-start', 'job-end', 'job-abort', 'backup-start', 'backup-end', 'backup-abort',
                   'log-end', 'pre-stop', 'pre-restart', 'post-restart', default={'script': None}
                   ),
         Validator(
```

### Comparing `proxmox-grapple-1.5.3/src/proxmox_grapple/vma_extractor.py` & `proxmox-grapple-1.5.4/src/proxmox_grapple/vma_extractor.py`

 * *Files identical despite different names*

### Comparing `proxmox-grapple-1.5.3/src/proxmox_grapple/vzdump_hook_script.py` & `proxmox-grapple-1.5.4/src/proxmox_grapple/vzdump_hook_script.py`

 * *Files identical despite different names*

### Comparing `proxmox-grapple-1.5.3/src/proxmox_grapple.egg-info/PKG-INFO` & `proxmox-grapple-1.5.4/src/proxmox_grapple.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxmox-grapple
-Version: 1.5.3
+Version: 1.5.4
 Summary: The grappling hook for Proxmox backups.
 Author-email: Jason Lingohr <jason@lucid.net.au>
 Project-URL: Homepage, https://github.com/lingfish/proxmox-grapple
 Project-URL: Issues, https://github.com/lingfish/proxmox-grapple/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
@@ -23,17 +23,48 @@
 The Python app that "hooks" into Proxmox.
 
 This is a clone of [vzdump-hook-script.pl](https://github.com/proxmox/pve-manager/blob/master/vzdump-hook-script.pl) that is
 written in Python, and that offers a lot more configurability.
 
 Different phases of the `vzdump` backup can be hooked into, and scripts can be run.
 
+<!-- TOC -->
+* [Proxmox-grapple](#proxmox-grapple)
+  * [Installation](#installation)
+  * [Configuration](#configuration)
+    * [Overview](#overview)
+    * [Location](#location)
+    * [Configuration environments](#configuration-environments)
+  * [Supported versions](#supported-versions)
+<!-- TOC -->
+
+## Installation
+
+The recommended way to install `proxmox-grapple` is to use [pipx](https://pipx.pypa.io/stable/).
+
+After getting `pipx` installed, simply run:
+
+```shell
+username@proxmox:~$ pipx install proxmox-grapple
+```
+
+Please, please [don't use pip system-wide](https://docs.python.org/3.11/installing/index.html#installing-into-the-system-python-on-linux).
+
+Once installed, you need to tell Proxmox (specifically `vzdump`) to use the app. Edit `/etc/vzdump.conf` and add or edit
+the `script` setting:
+
+```yaml
+script: /home/username/.local/bin/proxmox-grapple
+```
+
 
 ## Configuration
 
+### Overview
+
 `proxmox-grapple` is configured with a YAML-style file.  An example:
 
 ```yaml
 production:
   job-end:
     script:
       - echo 'hi'
@@ -45,44 +76,53 @@
     extract:
       enabled: false
       source_directory: /tmp
       destination_directory: /tmp
   #    exclude_storeids:
 ```
 
-The default location for the configuration is `/etc/proxmox_grapple.yml`, but this can also be specified on the
-commandline.
+### Location
+
+The default location for the configuration is `/etc/proxmox_grapple.yml`, or `proxmox_grapple.yml` in the current
+working directory, but this can also be specified on the commandline.
+
+If a non-absolute path is given, Dynaconf will iterate upwards: it will look at each parent up to the root of the
+system. For each visited folder, it will also try looking inside a `/config` folder.
+
+### Configuration environments
+
+It can also use different configuration settings based on arbitrary environment names (eg. `production`, `lab`, etc.) It
+uses the [Dynaconf](https://www.dynaconf.com/) Python project for configuration, so using environment variables to
+choose the environment and any other configuration option is possible.
+
+>⚠️ The default environment is `production`
 
-It can also use different configuration based on environments. It uses the [Dynaconf](https://www.dynaconf.com/) Python
-project for configuration, so using environment variables to choose the environment and any other configuration option is possible.
+For example, to choose a different configuration environment, set the environment variable `ENV_FOR_DYNACONF=lab`:
 
+```shell
+root@proxmox:~# ENV_FOR_DYNACONF=lab proxmox-grapple --dump-config
+```
 Each top-level key should match the different `vzdump` phases.  The currently recognised phases are:
 
 * job-init
 * job-start
 * job-end
 * job-abort
 * backup-start
 * backup-end
 * backup-abort
 * log-end
 * pre-stop
 * pre-restart
 * post-restart
 
-> [!NOTE]
-> The extract argument is currently not tested, and should be treated as a proof-of-concept only.
+>⚠️ The extract argument is currently not tested, and should be treated as a proof-of-concept only.
 
 
 ## Supported versions
 
 `proxmox-grapple` supports the following VE versions:
 
 | VE version | Debian version | Python version | VE EoL  |
 |------------|----------------|----------------|---------|
 | 8          | 12 (Bookworm)  | 3.11           | TBA     |
 | 7          | 11 (Bullseye)  | 3.9            | 2024-07 |
-
-
-## Installation
-
-The recommended way to install `proxmox-grapple` is to use [pipx](https://pipx.pypa.io/stable/).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `proxmox-grapple-1.5.3/tests/test_script_runs.py` & `proxmox-grapple-1.5.4/tests/test_script_runs.py`

 * *Files identical despite different names*

