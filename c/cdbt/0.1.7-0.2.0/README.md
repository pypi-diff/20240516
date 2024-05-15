# Comparing `tmp/cdbt-0.1.7.tar.gz` & `tmp/cdbt-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdbt-0.1.7.tar", last modified: Mon May 13 03:17:39 2024, max compression
+gzip compressed data, was "cdbt-0.2.0.tar", last modified: Tue May 14 20:57:03 2024, max compression
```

## Comparing `cdbt-0.1.7.tar` & `cdbt-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-13 03:17:39.663321 cdbt-0.1.7/
--rw-r--r--   0 craiglathrop   (501) staff       (20)      391 2024-05-13 03:17:39.660417 cdbt-0.1.7/PKG-INFO
--rw-r--r--   0 craiglathrop   (501) staff       (20)     3396 2024-05-12 23:47:32.000000 cdbt-0.1.7/README.md
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-13 03:17:39.649650 cdbt-0.1.7/cdbt/
--rw-r--r--   0 craiglathrop   (501) staff       (20)        0 2024-05-11 20:22:05.000000 cdbt-0.1.7/cdbt/__init__.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)     3892 2024-05-13 03:16:28.000000 cdbt-0.1.7/cdbt/cmdline.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)    12555 2024-05-13 03:16:29.000000 cdbt-0.1.7/cdbt/main.py
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-13 03:17:39.659659 cdbt-0.1.7/cdbt.egg-info/
--rw-r--r--   0 craiglathrop   (501) staff       (20)      391 2024-05-13 03:17:39.000000 cdbt-0.1.7/cdbt.egg-info/PKG-INFO
--rw-r--r--   0 craiglathrop   (501) staff       (20)      253 2024-05-13 03:17:39.000000 cdbt-0.1.7/cdbt.egg-info/SOURCES.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)        1 2024-05-13 03:17:39.000000 cdbt-0.1.7/cdbt.egg-info/dependency_links.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)       43 2024-05-13 03:17:39.000000 cdbt-0.1.7/cdbt.egg-info/entry_points.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)        6 2024-05-13 03:17:39.000000 cdbt-0.1.7/cdbt.egg-info/requires.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)        5 2024-05-13 03:17:39.000000 cdbt-0.1.7/cdbt.egg-info/top_level.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)       38 2024-05-13 03:17:39.663474 cdbt-0.1.7/setup.cfg
--rwxrwx---   0 craiglathrop   (501) staff       (20)      644 2024-05-13 03:16:39.000000 cdbt-0.1.7/setup.py
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-13 03:17:39.659024 cdbt-0.1.7/tests/
--rw-r--r--   0 craiglathrop   (501) staff       (20)     7405 2024-05-13 01:54:07.000000 cdbt-0.1.7/tests/test_main.py
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-14 20:57:03.157595 cdbt-0.2.0/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      466 2024-05-14 20:57:03.157003 cdbt-0.2.0/PKG-INFO
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     3805 2024-05-14 20:47:33.000000 cdbt-0.2.0/README.md
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-14 20:57:03.142255 cdbt-0.2.0/cdbt/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        0 2024-05-11 20:22:05.000000 cdbt-0.2.0/cdbt/__init__.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     6103 2024-05-14 20:54:39.000000 cdbt-0.2.0/cdbt/build_dbt_docs_ai.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     7330 2024-05-14 20:05:36.000000 cdbt-0.2.0/cdbt/build_unit_test_data_ai.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     5317 2024-05-14 20:49:22.000000 cdbt-0.2.0/cdbt/cmdline.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)    15157 2024-05-14 20:41:20.000000 cdbt-0.2.0/cdbt/main.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)    17490 2024-05-14 18:52:01.000000 cdbt-0.2.0/cdbt/prompts.py
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-14 20:57:03.156262 cdbt-0.2.0/cdbt.egg-info/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      466 2024-05-14 20:57:03.000000 cdbt-0.2.0/cdbt.egg-info/PKG-INFO
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      327 2024-05-14 20:57:03.000000 cdbt-0.2.0/cdbt.egg-info/SOURCES.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        1 2024-05-14 20:57:03.000000 cdbt-0.2.0/cdbt.egg-info/dependency_links.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)       43 2024-05-14 20:57:03.000000 cdbt-0.2.0/cdbt.egg-info/entry_points.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)       51 2024-05-14 20:57:03.000000 cdbt-0.2.0/cdbt.egg-info/requires.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        5 2024-05-14 20:57:03.000000 cdbt-0.2.0/cdbt.egg-info/top_level.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)       38 2024-05-14 20:57:03.157687 cdbt-0.2.0/setup.cfg
+-rwxrwx---   0 craiglathrop   (501) staff       (20)      710 2024-05-14 19:57:38.000000 cdbt-0.2.0/setup.py
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-14 20:57:03.155441 cdbt-0.2.0/tests/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     7050 2024-05-14 00:33:23.000000 cdbt-0.2.0/tests/test_main.py
```

### Comparing `cdbt-0.1.7/README.md` & `cdbt-0.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -15,63 +15,77 @@
 
 ```bash
 pip install cdbt
 ```
 
 Ensure that you have Python 3.8 or higher installed, as it is required for `cdbt` to function properly.
 
-## Usage
 
-### Basic DBT Shadowed Commands
+## Basic DBT Shadowed Commands
 These commands act as a pass-through to DBT, and are provided for convenience. They are not the primary focus of `cdbt`.
 
 - `cdbt run`
 - `cdbt test`
 - `cdbt build`
 
-### `trun` (Run and Test)
+## `trun` (Run and Test)
 
 This command runs the `run` and `test` commands in sequence. It is useful for running both commands in a single step. without executing a snapshot and seed.
 
 ```bash
 cdbt trun --select my_model
 ```
 
-### State Build Commands
+## 'unittest'
 
-#### Important Notes
+Executes the unit tests for selected, or all models. 
+```bash
+bash unittest --select my_model
+```
+
+## State Build Commands
+
+### Important Notes
 
-##### Auto Full Refresh
+#### Auto Full Refresh
 
 Both the `sbuild` and `pbuild` commands will scan the models to be built and automatically initiate a full refresh if an incrementally materialized model is found in the list (as per `dbt ls`). If you wish to force a `--full-refresh` for other reasons such as a column being added to a seed, add the `--full-refresh` flag.  
 
-##### State Build Commands with Parent and Child Modifiers
+#### State Build Commands with Parent and Child Modifiers
 
 Both the `sbuild` and `pbuild` commands can include modifications to build parent or child dependencies by appending a `+` and an optional integer to the command.
 
 - `+` or `+<number>` at the end of the command includes child dependencies up to the specified depth.
 - `+<number>` at the beginning of the command includes parent dependencies up to the specified depth.
 
 Example:
 
 - `cdbt pbuild+` and `cdbt pbuild+3` will build all state based variance models along with all child models up to 3 levels deep, respectively.
 - `cdbt 3+pbuild` will include parent models up to 3 levels up in the build.
 
-#### Production Build `pbuild`
+### Production Build `pbuild`
 This command initiates a state based build based on the manifest.json file associated with the master branch. This will use the DBT macro provided by Datacoves `get_last_artifacts` to pull the artifacts from the Snowflake file stage and save to the `./logs` folder. Then comparison is made against this file. This file is updated during the production deployment CI process.
 
    ```bash
    cdbt pbuild
    ```
 
-#### Local State Build `sbuild`   
+### Local State Build `sbuild`   
 Initiates a production state build. 
 
 ** Error Handling: **
 
 If an error occurs duing an sbuild operation, the manifest file copied to the `_artifacts` location will be moved back to `target`. This avoids an issue where after executing a state based build with a failure, the next build will not properly compare the state of the models.
 ```bash
 cdbt sbuild
 ```
 
+## AI DBT Docs Build
+The command `cdbt build-docs --select model_name` will automatically build, or update the DBT YML file for a selected model. 
+
+## AI Build DBT Unit Test Mock Data
+The command `cdbt build-unit --select model_name` will automatically build, or update the DBT YML file for a selected model.
+
+
+
 ## License
 Distributed under the MIT License. See `LICENSE` for more information.
```

### Comparing `cdbt-0.1.7/cdbt/main.py` & `cdbt-0.2.0/cdbt/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,114 +1,110 @@
 import json
 import subprocess
 import re
 import sys
 import shutil
 import os
-from typing import List, Optional
 import typing as t
 from click.core import Context, Command
 
 
 class ColdBoreCapitalDBT:
 
     def __init__(self, test_mode: bool = False):
         self.test_mode = test_mode
         self.dbt_ls_test_mode_output = None
         self.dbt_test_mode_command_check_value = None
         self.exclude_seed_snapshot = 'resource_type:snapshot resource_type:seed'
 
-    def build(self, ctx: Context, full_refresh, select, fail_fast, threads):
-        args = self._create_common_args(ctx, threads)
+        self.dbt_execute_command_output = ''
 
-        if select:
-            args.append('--select')
-            args.append(select)
-        if fail_fast:
-            args.append('--fail-fast')
-        if full_refresh:
-            args.append('--full-refresh')
+    def build(self, ctx: Context, full_refresh, select, fail_fast, threads):
+        flags = {'select': select, 'fail_fast': fail_fast, 'threads': threads, 'full_refresh': full_refresh}
+        args = self._create_common_args(flags)
         try:
-            run_result = self.execute_dbt_command('build', args)
+            run_result = self.execute_dbt_command_stream('build', args)
         except subprocess.CalledProcessError as e:
-            print(e)
-            sys.exit(1)
+            print(f'Failure while running command: {" ".join(e.cmd)}')
+            print(e.stderr)
+            print(e.stdout)
+            sys.exit(e.returncode)
 
         if not run_result:
             raise DbtError('DBT build failed with errors.')
 
     def trun(self, ctx: Context, full_refresh, select, fail_fast, threads):
-        args = self._create_common_args(ctx, threads)
+        flags = {'select': select, 'fail_fast': fail_fast, 'threads': threads, 'full_refresh': full_refresh}
+        args = self._create_common_args(flags)
         args = args + ['--exclude', self.exclude_seed_snapshot]
-        if select:
-            args.append('--select')
-            args.append(select)
-        if fail_fast:
-            args.append('--fail-fast')
-
-        if full_refresh:
-            args.append('--full-refresh')
-
         try:
-            run_result = self.execute_dbt_command('build', args)
+            run_result = self.execute_dbt_command_stream('build', args)
         except subprocess.CalledProcessError as e:
-            print(e)
-            print('dbt build ' + ' '.join(args))
-            sys.exit(1)
+            print(f'Failure while running command: {" ".join(e.cmd)}')
+            print(e.stderr)
+            print(e.stdout)
+            sys.exit(e.returncode)
 
         if not run_result:
             raise DbtError('DBT build failed with errors.')
 
     def run(self, ctx: Context, full_refresh, select, fail_fast, threads):
-        args = self._create_common_args(ctx, threads)
-        if select:
-            args.append('--select')
-            args.append(select)
-        if fail_fast:
-            args.append('--fail-fast')
-
-        run_args = args
-        if full_refresh:
-            run_args.append('--full-refresh')
+        flags = {'select': select, 'fail_fast': fail_fast, 'threads': threads, 'full_refresh': full_refresh}
+        args = self._create_common_args(flags)
         try:
-            run_result = self.execute_dbt_command('run', run_args)
+            run_result = self.execute_dbt_command_stream('run', args)
         except subprocess.CalledProcessError as e:
-            print(e)
-            print('dbt run ' + ' '.join(args))
-            sys.exit(1)
+            print(f'Failure while running command: {" ".join(e.cmd)}')
+            print(e.stderr)
+            print(e.stdout)
+            sys.exit(e.returncode)
 
         if not run_result:
             raise DbtError('DBT build failed with errors.')
 
     def test(self, ctx: Context, select, fail_fast, threads):
-        args = self._create_common_args(ctx, threads)
-        if select:
-            args.append('--select')
-            args.append(select)
-        if fail_fast:
-            args.append('--fail-fast')
-        run_args = args
+        flags = {'select': select, 'fail_fast': fail_fast, 'threads': threads}
+        args = self._create_common_args(flags)
         try:
-            run_result = self.execute_dbt_command('test', run_args)
+            run_result = self.execute_dbt_command_stream('test', args)
         except subprocess.CalledProcessError as e:
-            print(e)
-            print('dbt test ' + ' '.join(args))
-            sys.exit(1)
+            print(f'Failure while running command: {" ".join(e.cmd)}')
+            print(e.stderr)
+            print(e.stdout)
+            sys.exit(e.returncode)
 
         if not run_result:
             raise DbtError('DBT build failed with errors.')
 
+    def unittest(self, ctx: Context, select, fail_fast):
+        select = f'{select},tag:unit-test'  # Comma is an and condition.
+        flags = {'select': select, 'fail_fast': fail_fast}
+        args = self._create_common_args(flags)
+        try:
+            run_result = self.execute_dbt_command_stream('test', args)
+        except subprocess.CalledProcessError as e:
+            print(f'Failure while running command: {" ".join(e.cmd)}')
+            print(e.stderr)
+            print(e.stdout)
+            sys.exit(e.returncode)
+
+        if not run_result:
+            raise DbtError('DBT build failed with errors.')
+
+
+
     def compile(self, ctx: Context, threads):
         # We ignore the ctx object as compile has no threads.
         try:
-            self.execute_dbt_command('compile', [])
+            self.execute_dbt_command_stream('compile', [])
         except subprocess.CalledProcessError as e:
-            print(e)
-            print('dbt compile')
-            sys.exit(1)
+            print(f'Failure while running command: {" ".join(e.cmd)}')
+            print(e.stderr)
+            print(e.stdout)
+            sys.exit(e.returncode)
 
     def sbuild(self, ctx: Context, full_refresh, threads):
         print('Starting a state build based on local manifest.json')
         artifact_dir = '_artifacts'
         target_dir = 'target'
         # Path to the artifacts file that will be generated by the dbt compile command representing the current state.
         manifest_path = os.path.join('./', target_dir, 'manifest.json')
@@ -123,17 +119,18 @@
         artifact_dir = 'logs'
         target_dir = 'target'
         # Pull artifacts from Snowflake. These are the latest production artifacts.
         try:
             if not self.test_mode:
                 subprocess.run(['dbt', 'run-operation', 'get_last_artifacts'], check=True)
         except subprocess.CalledProcessError as e:
-            print(e)
-            print('dbt run-operation get_last_artifacts')
-            sys.exit(1)
+            print(f'Failure while running command: {" ".join(e.cmd)}')
+            print(e.stderr)
+            print(e.stdout)
+            sys.exit(e.returncode)
 
         manifest_path = os.path.join('.', target_dir, 'manifest.json')
         manifest_artifact_path = os.path.join('.', artifact_dir, 'manifest.json')
 
         self.execute_state_based_build(ctx, artifact_dir, manifest_artifact_path, manifest_path, full_refresh, threads,
                                        roll_back_manifest_flag=False)
 
@@ -144,16 +141,20 @@
             # Move the manifest from ./target to ./_artifacts. This becomes the prior state. Only used for local state
             # build. Not used for pdbuild (production build).
             shutil.move(manifest_path, manifest_artifact_path)
         # Execute dbt compile
         try:
             if not self.test_mode:
                 subprocess.run(['dbt', 'compile'], check=True)
-        except subprocess.CalledProcessError:
-            sys.exit(1)
+        except subprocess.CalledProcessError as e:
+            print(f'Failure while running command: {" ".join(e.cmd)}')
+            print(e.stderr)
+            print(e.stdout)
+            sys.exit(e.returncode)
+
         # Construct state commands
         build_children = ctx.obj.get('build_children', False)
         build_children_count = ctx.obj.get('build_children_count', None)
         build_parents = ctx.obj.get('build_parents', False)
         build_parent_count = ctx.obj.get('build_parents_count', None)
         state_modified_str = 'state:modified'
         if build_children:
@@ -168,90 +169,131 @@
         state_flags = [
             '--select', state_modified_str,
             '--state', os.path.join('.', artifact_dir) + '/'
         ]
         exclude_flags = ['--exclude', self.exclude_seed_snapshot]
         # Get a list of models and their config
 
-        args = state_flags + exclude_flags
-        args = args + ['--output-keys', 'name resource_type config', '--output', 'json']
-        cmd = ['dbt', 'ls']
-        cmd = cmd + args
-        try:
-            if self.test_mode:
-                output = self.dbt_ls_test_mode_output
-            else:
-                output = subprocess.run(cmd, check=True, text=True, capture_output=True).stdout
-        except subprocess.CalledProcessError as e:
-            print(e)
-            print(' '.join(cmd))
-            sys.exit(1)
-
-        # The results come back with a few header lines that need to be removed, then a series of JSON string with a format
-        # like: {"name": "active_patient_metrics", "resource_type": "model", "config": {"materialized": "incremental"}}
-        # RE removes the header stuff and finds the json lines.
-        json_lines = re.findall(r'^{.*$', output, re.MULTILINE)
-
-        # Split lines and filter to get only JSON strings
-        models_json = [json.loads(line) for line in json_lines]
-
-        if not full_refresh:
-            full_refresh = self.test_full_refresh(models_json)
+        full_refresh = self._scan_for_incremental_full_refresh(state_flags, exclude_flags, full_refresh)
 
         run_result = None
         # Execute dbt build excluding snapshots and seeds
         # Rest the args.
-        args = self._create_common_args(ctx, threads)
+        args = self._create_common_args({'threads': threads})
         args = args + state_flags + exclude_flags
         if full_refresh:
             args = args + ['--full-refresh']
 
         try:
-            run_result = self.execute_dbt_command('build', args)
+            run_result = self.execute_dbt_command_stream('build', args)
         except subprocess.CalledProcessError as e:
-            print(e)
+            print(f'Failure while running command: {" ".join(e.cmd)}')
+            print(e.stderr)
+            print(e.stdout)
             if roll_back_manifest_flag and not self.test_mode:
                 self.roll_back_manifest(e, manifest_artifact_path, manifest_path)
             else:
-                print('dbt build ' + ' '.join(args))
-                sys.exit(1)
+                sys.exit(e.returncode)
 
         if not run_result:
             e = 'DBT build failed with errors.'
             self.roll_back_manifest(e, manifest_artifact_path, manifest_path)
             raise DbtError('DBT build failed with errors.')
 
+    def _scan_for_incremental_full_refresh(self, state_flags, exclude_flags, full_refresh):
+        args = state_flags + exclude_flags
+        ls_args = args + ['--output-keys', 'name resource_type config', '--output', 'json']
+        models_json = self.dbt_ls_to_json(args)
+        if not full_refresh:
+            for model in models_json:
+                if model['config']['materialized'] == 'incremental':
+                    full_refresh = True
+                    print(f'Found incremental build model: {model["name"]}. Initiating full refresh.')
+                    break
+        return full_refresh
+
+    def dbt_ls_to_json(self, args):
+        cmd = ['dbt', 'ls']
+        cmd = cmd + args
+        try:
+            if self.test_mode:
+                output = self.dbt_ls_test_mode_output
+            else:
+                output = subprocess.run(cmd, check=True, text=True, capture_output=True).stdout
+        except subprocess.CalledProcessError as e:
+            print(e.stderr)
+            print(e.stdout)
+            print(' '.join(cmd))
+            sys.exit(e.returncode)
+        # The results come back with a few header lines that need to be removed, then a series of JSON string with a format
+        # like: {"name": "active_patient_metrics", "resource_type": "model", "config": {"materialized": "incremental"}}
+        # RE removes the header stuff and finds the json lines.
+        json_lines = re.findall(r'^{.*$', output, re.MULTILINE)
+        # Split lines and filter to get only JSON strings
+        models_json = [json.loads(line) for line in json_lines]
+        return models_json
+
     @staticmethod
-    def _create_common_args(ctx: Context, threads: int = None) -> List[str]:
+    def _create_common_args(flags: t.Dict[str, t.Any]) -> t.List[str]:
+        threads = flags.get('threads', None)
+        select = flags.get('select', None)
+        fail_fast = flags.get('fail_fast', None)
+        full_refresh = flags.get('full_refresh', None)
         args = []
         if threads:
             args.append('--threads')
             args.append(str(threads))
+        if select:
+            args.append('--select')
+            args.append(select)
+        if fail_fast:
+            args.append('--fail-fast')
+        if full_refresh:
+            args.append('--full-refresh')
         return args
 
     @staticmethod
     def roll_back_manifest(e, manifest_artifact_path, manifest_path):
         print(f"DBT build failed. Rolling back manifest state with error\n {e}")
         # Move the manifest.json from _artifacts back to target dir. If the build failed, we want to rebuild against this
         # state, not the one generated by the compile command.
         shutil.move(manifest_artifact_path, manifest_path)
-        sys.exit(1)
+        sys.exit(e.returncode)
 
     @staticmethod
-    def test_full_refresh(models_json):
-        includes_incremental_build = False
-        for model in models_json:
-            if model['config']['materialized'] == 'incremental':
-                includes_incremental_build = True
-                print(f'Found incremental build model: {model["name"]}. Initiating full refresh.')
-                break
-
-        return includes_incremental_build
-
-    def execute_dbt_command(self, command: str, args: List[str]):
+    def execute_dbt_command_capture(command:str, args: t.List[str]) -> str:
+        """
+        Executes a DBT command and captures the output without streaming to the stdout.
+        Args:
+            command: The DBT command to run.
+            args: A list of args to pass into the command.
+
+        Returns:
+            A string containing the results of the command.
+        """
+        cmd = ['dbt', command] + args
+        try:
+            output = subprocess.run(cmd, check=True, text=True, capture_output=True).stdout
+        except subprocess.CalledProcessError as e:
+            print(f'Failure while running command: {" ".join(cmd)}')
+            print(e.stderr)
+            print(e.stdout)
+            sys.exit(e.returncode)
+        return output
+
+    def execute_dbt_command_stream(self, command: str, args: t.List[str]) -> bool:
+        """
+        Execute a dbt command with the given arguments. This function will stream the output of the command in real-time
+        Args:
+            command: The DBT command to run.
+            args: A list of args to pass into the command.
+
+        Returns:
+            True if successful, False if error.
+        """
 
         dbt_command = ['dbt', command] + args
         print(f'Running command: {" ".join(dbt_command)}')
         if self.test_mode:
             self.dbt_test_mode_command_check_value = dbt_command
             return True
         else:
@@ -279,14 +321,15 @@
             if process.returncode != 0:
                 print(f"Command resulted in an error: {stderr}")
                 raise subprocess.CalledProcessError(returncode=process.returncode, cmd=dbt_command, output=stderr)
 
             # Check for errors using a regex method if necessary
             if self.contains_errors(stdout + stderr):
                 return False
+
             return True
 
     @staticmethod
     def contains_errors(text):
         pattern = r"([2-9]|\d{2,})\s+errors?"
         error_flag = bool(re.search(pattern, text))
         return error_flag
```

### Comparing `cdbt-0.1.7/setup.py` & `cdbt-0.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cdbt',
-    version='0.1.7',
+    version='0.2.0',
     description='A CLI tool to manage dbt builds with state handling and manifest management',
     author='Craig Lathrop',
     author_email='development@coldborecapital.com',
     packages=find_packages(),
     install_requires=[
         'click',
+        'pyperclip',
+        'snowflake-connector-python[pandas]'
     ],
     entry_points={
         'console_scripts': [
             'cdbt=cdbt.cmdline:cdbt',
         ],
     },
     classifiers=[
```

