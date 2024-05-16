# Comparing `tmp/1password-secrets-0.0.7.tar.gz` & `tmp/1password-secrets-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "1password-secrets-0.0.7.tar", last modified: Fri Dec 15 10:28:22 2023, max compression
+gzip compressed data, was "1password-secrets-0.0.8.tar", last modified: Mon Mar 18 11:19:25 2024, max compression
```

## Comparing `1password-secrets-0.0.7.tar` & `1password-secrets-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 10:28:22.515504 1password-secrets-0.0.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 10:28:22.515504 1password-secrets-0.0.7/1password_secrets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4249 2023-12-15 10:28:22.000000 1password-secrets-0.0.7/1password_secrets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      299 2023-12-15 10:28:22.000000 1password-secrets-0.0.7/1password_secrets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-15 10:28:22.000000 1password-secrets-0.0.7/1password_secrets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-15 10:28:22.000000 1password-secrets-0.0.7/1password_secrets.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-15 10:28:22.000000 1password-secrets-0.0.7/1password_secrets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-12-15 10:28:22.000000 1password-secrets-0.0.7/1password_secrets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4249 2023-12-15 10:28:22.515504 1password-secrets-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3516 2023-12-15 10:28:15.000000 1password-secrets-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    14199 2023-12-15 10:28:15.000000 1password-secrets-0.0.7/onepassword_secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2023-12-15 10:28:22.515504 1password-secrets-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2023-12-15 10:28:15.000000 1password-secrets-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 11:19:25.040691 1password-secrets-0.0.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 11:19:25.040691 1password-secrets-0.0.8/1password_secrets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-03-18 11:19:24.000000 1password-secrets-0.0.8/1password_secrets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-18 11:19:25.000000 1password-secrets-0.0.8/1password_secrets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 11:19:24.000000 1password-secrets-0.0.8/1password_secrets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-18 11:19:24.000000 1password-secrets-0.0.8/1password_secrets.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-18 11:19:24.000000 1password-secrets-0.0.8/1password_secrets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-18 11:19:24.000000 1password-secrets-0.0.8/1password_secrets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-03-18 11:19:25.040691 1password-secrets-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-03-18 11:19:11.000000 1password-secrets-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    17381 2024-03-18 11:19:11.000000 1password-secrets-0.0.8/onepassword_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-18 11:19:25.040691 1password-secrets-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-03-18 11:19:11.000000 1password-secrets-0.0.8/setup.py
```

### Comparing `1password-secrets-0.0.7/1password_secrets.egg-info/PKG-INFO` & `1password-secrets-0.0.8/1password_secrets.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 1password-secrets
-Version: 0.0.7
+Version: 0.0.8
 Summary: 1password-secrets is a set of utilities to sync 1Password secrets.
 Home-page: https://github.com/significa/fly-1password-secrets
 Author: Significa
 License: MIT
 Keywords: fly.io,1password,secrets
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -58,27 +58,40 @@
   Python >= `3.9`
 
   ```
   brew install --cask 1password 1password-cli && \
   brew install flyctl
   ```
 
+  More information and installation instructions for other systems can be found
+  [in the 1password documentation](https://developer.1password.com/docs/cli/get-started/).
+
 - Allow 1Password to connect to 1Password-CLI by going to `Settings` -> `Developer` ->
   `Command-Line Interface (CLI)` and select `Connect with 1Password CLI`.
 
-- Sign into your 1Password and Fly account (if you wish to use the fly integration).
+- Sign into your 1Password desktop and if you wish to use the fly integration, also make sure
+  the CLI is authenticated.
 
 ### Installation
 
 In most systems (Mac and Linux) when `pip3` (Python's 3 PIP) is in path
 and you want to install it at the user level:
 
 `pip3 install -U 1password-secrets`
 
-Otherwise adapt it accordingly.
+Otherwise you may need to install it with invoking your preferred Python version:
+`python3 -m pip install -U 1password-secrets`.
+
+Or, even more specific `python3.12 -m pip install -U 1password-secrets`
+
+Also, if your "_environment is externally managed_" you _can_ bypass it with:
+`python3 -m pip install -U --break-system-packages 1password-secrets`
+
+If you use tools like `pipx` or manage your environment differently adapt the installation
+instructions.
 
 ## Usage
 
 ### Local
 
 From within a valid git repository with remote "origin" ending in `<owner>/<repo>.git`,
 1password-secrets will be able to `pull` and `push` secrets to a 1password secure note containing
```

### Comparing `1password-secrets-0.0.7/PKG-INFO` & `1password-secrets-0.0.8/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 1password-secrets
-Version: 0.0.7
+Version: 0.0.8
 Summary: 1password-secrets is a set of utilities to sync 1Password secrets.
 Home-page: https://github.com/significa/fly-1password-secrets
 Author: Significa
 License: MIT
 Keywords: fly.io,1password,secrets
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -58,27 +58,40 @@
   Python >= `3.9`
 
   ```
   brew install --cask 1password 1password-cli && \
   brew install flyctl
   ```
 
+  More information and installation instructions for other systems can be found
+  [in the 1password documentation](https://developer.1password.com/docs/cli/get-started/).
+
 - Allow 1Password to connect to 1Password-CLI by going to `Settings` -> `Developer` ->
   `Command-Line Interface (CLI)` and select `Connect with 1Password CLI`.
 
-- Sign into your 1Password and Fly account (if you wish to use the fly integration).
+- Sign into your 1Password desktop and if you wish to use the fly integration, also make sure
+  the CLI is authenticated.
 
 ### Installation
 
 In most systems (Mac and Linux) when `pip3` (Python's 3 PIP) is in path
 and you want to install it at the user level:
 
 `pip3 install -U 1password-secrets`
 
-Otherwise adapt it accordingly.
+Otherwise you may need to install it with invoking your preferred Python version:
+`python3 -m pip install -U 1password-secrets`.
+
+Or, even more specific `python3.12 -m pip install -U 1password-secrets`
+
+Also, if your "_environment is externally managed_" you _can_ bypass it with:
+`python3 -m pip install -U --break-system-packages 1password-secrets`
+
+If you use tools like `pipx` or manage your environment differently adapt the installation
+instructions.
 
 ## Usage
 
 ### Local
 
 From within a valid git repository with remote "origin" ending in `<owner>/<repo>.git`,
 1password-secrets will be able to `pull` and `push` secrets to a 1password secure note containing
```

### Comparing `1password-secrets-0.0.7/README.md` & `1password-secrets-0.0.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -38,27 +38,40 @@
   Python >= `3.9`
 
   ```
   brew install --cask 1password 1password-cli && \
   brew install flyctl
   ```
 
+  More information and installation instructions for other systems can be found
+  [in the 1password documentation](https://developer.1password.com/docs/cli/get-started/).
+
 - Allow 1Password to connect to 1Password-CLI by going to `Settings` -> `Developer` ->
   `Command-Line Interface (CLI)` and select `Connect with 1Password CLI`.
 
-- Sign into your 1Password and Fly account (if you wish to use the fly integration).
+- Sign into your 1Password desktop and if you wish to use the fly integration, also make sure
+  the CLI is authenticated.
 
 ### Installation
 
 In most systems (Mac and Linux) when `pip3` (Python's 3 PIP) is in path
 and you want to install it at the user level:
 
 `pip3 install -U 1password-secrets`
 
-Otherwise adapt it accordingly.
+Otherwise you may need to install it with invoking your preferred Python version:
+`python3 -m pip install -U 1password-secrets`.
+
+Or, even more specific `python3.12 -m pip install -U 1password-secrets`
+
+Also, if your "_environment is externally managed_" you _can_ bypass it with:
+`python3 -m pip install -U --break-system-packages 1password-secrets`
+
+If you use tools like `pipx` or manage your environment differently adapt the installation
+instructions.
 
 ## Usage
 
 ### Local
 
 From within a valid git repository with remote "origin" ending in `<owner>/<repo>.git`,
 1password-secrets will be able to `pull` and `push` secrets to a 1password secure note containing
```

### Comparing `1password-secrets-0.0.7/onepassword_secrets.py` & `1password-secrets-0.0.8/onepassword_secrets.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 import argparse
 import json
 import logging
+import os
 import re
 import subprocess
 import sys
 from datetime import datetime
 from io import StringIO
 from tempfile import NamedTemporaryFile
 
 from dotenv import dotenv_values
 from sgqlc.endpoint.http import HTTPEndpoint
 
 FLY_GRAPHQL_ENDPOINT = 'https://api.fly.io/graphql'
 DATE_FORMAT = '%Y/%m/%d %H:%M:%S'
 DEFAULT_ENV_FILE_NAME = '.env'
+ONE_PASSWORD_FILE_PATH_FIELD_NAME = 'file_name'
+ONE_PASSWORD_NOTES_CONTENT_FIELD_NAME = 'notesPlain'
+ONE_PASSWORD_SECURE_NOTE_CATEGORY = 'Secure Note'
 
 
 class UserError(RuntimeError):
     pass
 
 
 def _setup_logger():
@@ -46,15 +50,15 @@
     secure_notes = json.loads(
         subprocess.check_output(
             [
                 'op',
                 'item',
                 'list',
                 '--categories',
-                'Secure Note',
+                ONE_PASSWORD_SECURE_NOTE_CATEGORY,
                 '--format',
                 'json',
             ]
         )
     )
 
     item_ids = list(
@@ -87,29 +91,29 @@
 
 def get_envs_from_1password(item_id):
     item = get_item_from_1password(item_id)
 
     result = first(
         field.get('value')
         for field in item['fields']
-        if field['id'] == 'notesPlain'
+        if field['id'] == ONE_PASSWORD_NOTES_CONTENT_FIELD_NAME
     )
     if result is None or result == '':
         raise_error('Empty secrets, aborting')
 
     return result
 
 
 def get_filename_from_1password(item_id):
     item = get_item_from_1password(item_id)
 
     result = first(
         field.get('value')
         for field in item['fields']
-        if field['label'] == 'file_name'
+        if field['label'] == ONE_PASSWORD_FILE_PATH_FIELD_NAME
     )
 
     return result
 
 
 def get_fly_auth_token():
     return json.loads(
@@ -306,14 +310,39 @@
                 if len(items) != 0
             )
         )
     ):
         raise_error('Aborted by user')
 
 
+def create_1password_secrets(
+    file_path,
+    raw_secrets,
+    title,
+):
+    logger.debug('Creating 1password secret note')
+
+    return json.loads(
+        subprocess.check_output([
+            'op',
+            'item',
+            'create',
+            '--category',
+            ONE_PASSWORD_SECURE_NOTE_CATEGORY,
+            '--title',
+            title,
+            f'{ONE_PASSWORD_NOTES_CONTENT_FIELD_NAME}={raw_secrets}',
+            f'{ONE_PASSWORD_FILE_PATH_FIELD_NAME}[text]={file_path}',
+            _make_last_edited_1password_custom_field_cli_argument(),
+            '--format',
+            'json',
+        ])
+    )
+
+
 def update_1password_secrets(
     item_id,
     new_raw_secrets,
     previous_raw_secrets=None
 ):
     if previous_raw_secrets is None:
         previous_raw_secrets = get_envs_from_1password(item_id)
@@ -325,31 +354,46 @@
 
     logger.debug(f'Updating 1password secret note content for item {item_id!r}')
     subprocess.check_output([
         'op',
         'item',
         'edit',
         item_id,
-        f'notesPlain={new_raw_secrets}'
+        f'notesPlain={new_raw_secrets}',
+        _make_last_edited_1password_custom_field_cli_argument(),
     ])
 
 
 def update_1password_custom_field(item_id, field, value):
     logger.debug(f'Updating 1password custom field for item {item_id!r}')
     subprocess.check_output([
         'op',
         'item',
         'edit',
         item_id,
-        f'Generated by 1password-secrets.{field}[text]={value}',
+        _make_1password_custom_field_cli_argument(field, value),
         '--format',
         'json'
     ])
 
 
+def _make_1password_custom_field_cli_argument(field_name, value):
+    PREFIX = 'Generated by 1password-secrets'
+    return f'{PREFIX}.{field_name}[text]={value}'
+
+
+def _make_last_edited_1password_custom_field_cli_argument():
+    now_formatted = datetime.now().strftime(DATE_FORMAT)
+
+    return _make_1password_custom_field_cli_argument(
+        field_name='last edited at',
+        value=now_formatted,
+    )
+
+
 def get_secrets_from_envs(input: str):
     secrets = dotenv_values(stream=StringIO(input))
 
     keys_with_values_null_values = [
         key
         for key, value in secrets.items()
         if value is None
@@ -397,31 +441,24 @@
 
     update_1password_secrets(
         item_id,
         new_raw_secrets=new_raw_secrets,
         previous_raw_secrets=current_raw_secrets
     )
 
-    now_formatted = datetime.now().strftime(DATE_FORMAT)
-    update_1password_custom_field(
-        item_id,
-        'last edited at',
-        now_formatted
-    )
-
     if _boolean_prompt(
         'Secrets updated in 1password, '
         f'do you wish to import secrets to the fly app {app_id}?'
     ):
         import_1password_secrets_to_fly(app_id)
 
 
 def pull_local_secrets():
-    repository = get_git_repository_name_from_current_directory()
-    item_id = get_1password_env_file_item_id(f'repo:{repository}')
+    secret_note_label = get_secret_name_label_from_current_directory()
+    item_id = get_1password_env_file_item_id(secret_note_label)
 
     secrets = get_envs_from_1password(item_id)
 
     env_file_name = get_filename_from_1password(item_id) or DEFAULT_ENV_FILE_NAME
 
     previous_raw_secrets = _get_file_contents(env_file_name, raise_if_not_found=False)
 
@@ -434,57 +471,112 @@
     with open(env_file_name, 'w') as file:
         file.writelines(secrets)
 
     print(f'Successfully updated {env_file_name} from 1password')
 
 
 def push_local_secrets():
-    repository_name = get_git_repository_name_from_current_directory()
-    item_id = get_1password_env_file_item_id(f'repo:{repository_name}')
+    secret_note_label = get_secret_name_label_from_current_directory()
+    item_id = get_1password_env_file_item_id(secret_note_label)
 
     env_file_name = get_filename_from_1password(item_id) or DEFAULT_ENV_FILE_NAME
 
     secrets = _get_file_contents(env_file_name, raise_if_not_found=True)
 
     update_1password_secrets(item_id, secrets)
 
-    now_formatted = datetime.now().strftime(DATE_FORMAT)
-    update_1password_custom_field(
-        item_id,
-        'last edited at',
-        now_formatted
+    print(f'Successfully pushed secrets from {env_file_name} to 1password')
+
+
+def create_local_secrets(secrets_file_path):
+    secret_note_label = get_secret_name_label_from_current_directory()
+
+    raw_secrets = _get_file_contents(secrets_file_path, raise_if_not_found=True)
+
+    title = f'{secrets_file_path} local development {secret_note_label}'
+
+    item = create_1password_secrets(
+        file_path=secrets_file_path,
+        raw_secrets=raw_secrets,
+        title=title,
     )
 
-    print(f'Successfully pushed secrets from {env_file_name} to 1password')
+    print(f'Item {title!r} created in 1password!\n')
+
+    item_url = (
+        subprocess.check_output([
+            'op',
+            'item',
+            'get',
+            item["id"],
+            '--share-link',
+        ])
+        .decode('utf-8')
+    ).strip()
 
+    print(item_url)
+    print(item_url.replace('https://start.1password.com/', 'onepassword://'))
 
-def get_git_repository_name_from_current_directory():
-    GIT_REPOSITORY_REGEX = r'^(https|git)(:\/\/|@)([^\/:]+)[\/:]([^\/:]+)\/(.+).git$'
+
+def _get_git_remote_origin_name() -> tuple[str | None, str | None]:
+    GIT_REPOSITORY_REGEX = r'^(\w+)(:\/\/|@)([^\/:]+)[\/:]([^\/:]+)\/(.+).git$'
+
+    git_remote_origin_url = None
 
     try:
         git_remote_origin_url = subprocess.check_output([
             'git',
             'config',
             '--get',
             'remote.origin.url'
         ]).decode('utf-8')
-    except subprocess.CalledProcessError:
-        raise_error('Either not in a git repository or remote "origin" is not set')
+
+    except FileNotFoundError:
+        return ('git not in the PATH', None)
+
+    except subprocess.CalledProcessError as error:
+        exit_code, _command = error.args
+
+        if exit_code == 1:
+            return ('Either not in a git repository or remote "origin" is not set', None)
+
+        return ('Failed to retrieve the git remote "origin" url', None)
 
     regex_match = re.match(
         GIT_REPOSITORY_REGEX,
         git_remote_origin_url
     )
 
     if regex_match is None:
-        raise_error('Could not get remote "origin" url from git repository')
+        return ('Failed to parse git remote "origin"', None)
+
+    return (
+        None,
+        f'{regex_match.group(4)}/{regex_match.group(5)}',
+    )
+
+
+def get_secret_name_label_from_current_directory() -> str:
+    """
+    Returns a predictable label for identifying the secrets based on the current directory.
+    If within a git repository with a remote named "origin" (and git is installed), it will output
+     something like: `repo:my-org/my-repo` or `repo:my-org/my-team/my-repo`.
+    Otherwise it will return the name of the directory as `local-dir:my-directory-name`.
+    """
+
+    error_message, git_remote_origin_name = _get_git_remote_origin_name()
 
-    repository_name = f'{regex_match.group(4)}/{regex_match.group(5)}'
+    if not error_message:
+        return f'repo:{git_remote_origin_name}'
 
-    return repository_name
+    directory_name = os.path.basename(os.getcwd())
+    label = f'local-dir:{directory_name}'
+
+    print(f'{error_message}, using the label based on the current directory: {label!r}')
+    return label
 
 
 def raise_error(message):
     print(message)
     raise UserError(message)
 
 
@@ -510,31 +602,45 @@
     subparsers = parser.add_subparsers(dest='subcommand', required=True)
 
     fly_parser = subparsers.add_parser('fly', help='manage fly secrets')
     fly_parser.add_argument('action', type=str, choices=['import', 'edit'])
     fly_parser.add_argument('app_name', type=str, help='fly application name')
 
     local_parser = subparsers.add_parser('local', help='manage local secrets')
-    local_parser.add_argument('action', type=str, choices=['pull', 'push'])
+    local_subparsers = local_parser.add_subparsers(dest='action', required=True)
+
+    local_subparsers.add_parser('pull')
+    local_subparsers.add_parser('push')
+
+    create_parser = local_subparsers.add_parser('create')
+    create_parser.add_argument(
+        'secrets_file_path',
+        type=str,
+        help='secrets file path',
+    )
 
     args = parser.parse_args()
 
     if args.debug:
         logger.setLevel(logging.DEBUG)
 
     try:
         if args.subcommand == 'fly':
             if args.action == 'import':
                 import_1password_secrets_to_fly(args.app_name)
             elif args.action == 'edit':
                 edit_1password_fly_secrets(args.app_name)
+
         elif args.subcommand == 'local':
             if args.action == 'pull':
                 pull_local_secrets()
             elif args.action == 'push':
                 push_local_secrets()
+            elif args.action == 'create':
+                create_local_secrets(args.secrets_file_path)
+
     except UserError:
         sys.exit(1)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `1password-secrets-0.0.7/setup.py` & `1password-secrets-0.0.8/setup.py`

 * *Files identical despite different names*

