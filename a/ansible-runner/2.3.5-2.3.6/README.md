# Comparing `tmp/ansible-runner-2.3.5.tar.gz` & `tmp/ansible-runner-2.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-runner-2.3.5.tar", last modified: Tue Feb 13 19:16:52 2024, max compression
+gzip compressed data, was "ansible-runner-2.3.6.tar", last modified: Tue Mar 12 15:20:33 2024, max compression
```

## Comparing `ansible-runner-2.3.5.tar` & `ansible-runner-2.3.6.tar`

### file list

```diff
@@ -1,321 +1,321 @@
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.580576 ansible-runner-2.3.5/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      209 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/.cherry_picker.toml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      287 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/.coveragerc
--rw-rw-r--   0 shrews    (1000) shrews    (1000)        5 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/.dockerignore
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.560577 ansible-runner-2.3.5/.github/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      162 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/.github/CODE_OF_CONDUCT.md
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.564576 ansible-runner-2.3.5/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     1939 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       27 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/.github/ISSUE_TEMPLATE/config.yml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      611 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/.github/ISSUE_TEMPLATE/documentation_report.yml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      588 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       23 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/.github/issue_labeler.yml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      117 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/.github/patchback.yml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       37 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/.github/pr_labeler_existing.yml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       90 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/.github/pr_labeler_new.yml
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.564576 ansible-runner-2.3.5/.github/workflows/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     3011 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/.github/workflows/ci.yml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      763 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/.github/workflows/triage_existing.yml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      734 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/.github/workflows/triage_new.yml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      114 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/.pre-commit-config.yaml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      334 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/.readthedocs.yaml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      466 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/.yamllint
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.564576 ansible-runner-2.3.5/.zuul.d/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     8029 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/.zuul.d/jobs.yaml
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.564576 ansible-runner-2.3.5/.zuul.d/playbooks/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/.zuul.d/playbooks/.zuul.ignore
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.564576 ansible-runner-2.3.5/.zuul.d/playbooks/ansible-runner-container-image-base/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      331 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/.zuul.d/playbooks/ansible-runner-container-image-base/pre.yaml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      795 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/.zuul.d/project.yaml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     4358 2024-02-13 19:16:52.000000 ansible-runner-2.3.5/AUTHORS
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      306 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/CODEOWNERS
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     1422 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/CONTRIBUTING.md
--rw-rw-r--   0 shrews    (1000) shrews    (1000)    49746 2024-02-13 19:16:52.000000 ansible-runner-2.3.5/ChangeLog
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     2547 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/Dockerfile
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     9304 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/LICENSE.md
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       55 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/MANIFEST.in
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     5345 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/Makefile
--rw-r--r--   0 shrews    (1000) shrews    (1000)     3505 2024-02-13 19:16:52.580576 ansible-runner-2.3.5/PKG-INFO
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     2044 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/README.md
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      313 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/SECURITY.md
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.564576 ansible-runner-2.3.5/ansible_runner/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      708 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/ansible_runner/__init__.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)    35764 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/ansible_runner/__main__.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     6609 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/ansible_runner/cleanup.py
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.564576 ansible-runner-2.3.5/ansible_runner/config/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/ansible_runner/config/__init__.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)    29029 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/ansible_runner/config/_base.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     3381 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/ansible_runner/config/ansible_cfg.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     4323 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/ansible_runner/config/command.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     6418 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/ansible_runner/config/doc.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     4897 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/ansible_runner/config/inventory.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)    17441 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/ansible_runner/config/runner.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      408 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/ansible_runner/defaults.py
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.564576 ansible-runner-2.3.5/ansible_runner/display_callback/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/ansible_runner/display_callback/__init__.py
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.564576 ansible-runner-2.3.5/ansible_runner/display_callback/callback/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/ansible_runner/display_callback/callback/__init__.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)    31150 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/ansible_runner/display_callback/callback/awx_display.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      256 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/ansible_runner/exceptions.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)    64207 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/ansible_runner/interface.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     5986 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/ansible_runner/loader.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     3008 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/ansible_runner/output.py
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.564576 ansible-runner-2.3.5/ansible_runner/plugins/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/ansible_runner/plugins/__init__.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)    26164 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/ansible_runner/runner.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      905 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/ansible_runner/runner_config.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)    14322 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/ansible_runner/streaming.py
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.568576 ansible-runner-2.3.5/ansible_runner/utils/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)    17031 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/ansible_runner/utils/__init__.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)    11731 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/ansible_runner/utils/base64io.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     1719 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/ansible_runner/utils/capacity.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      159 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/ansible_runner/utils/importlib_compat.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     4931 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/ansible_runner/utils/streaming.py
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.580576 ansible-runner-2.3.5/ansible_runner.egg-info/
--rw-r--r--   0 shrews    (1000) shrews    (1000)     3505 2024-02-13 19:16:52.000000 ansible-runner-2.3.5/ansible_runner.egg-info/PKG-INFO
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     7516 2024-02-13 19:16:52.000000 ansible-runner-2.3.5/ansible_runner.egg-info/SOURCES.txt
--rw-rw-r--   0 shrews    (1000) shrews    (1000)        1 2024-02-13 19:16:52.000000 ansible-runner-2.3.5/ansible_runner.egg-info/dependency_links.txt
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       64 2024-02-13 19:16:52.000000 ansible-runner-2.3.5/ansible_runner.egg-info/entry_points.txt
--rw-rw-r--   0 shrews    (1000) shrews    (1000)        1 2024-02-13 19:16:52.000000 ansible-runner-2.3.5/ansible_runner.egg-info/not-zip-safe
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       47 2024-02-13 19:16:52.000000 ansible-runner-2.3.5/ansible_runner.egg-info/pbr.json
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      107 2024-02-13 19:16:52.000000 ansible-runner-2.3.5/ansible_runner.egg-info/requires.txt
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       15 2024-02-13 19:16:52.000000 ansible-runner-2.3.5/ansible_runner.egg-info/top_level.txt
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      155 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/bindep.txt
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.556577 ansible-runner-2.3.5/demo/
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.568576 ansible-runner-2.3.5/demo/env/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       18 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/demo/env/envvars
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       40 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/demo/env/extravars
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       39 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/demo/env/passwords
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       60 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/demo/env/settings
--rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/demo/env/ssh_key
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.568576 ansible-runner-2.3.5/demo/inventory/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       94 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/demo/inventory/hosts
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.568576 ansible-runner-2.3.5/demo/project/
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.556577 ansible-runner-2.3.5/demo/project/roles/
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.568576 ansible-runner-2.3.5/demo/project/roles/testrole/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     1328 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/demo/project/roles/testrole/README.md
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.568576 ansible-runner-2.3.5/demo/project/roles/testrole/defaults/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       33 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/demo/project/roles/testrole/defaults/main.yml
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.568576 ansible-runner-2.3.5/demo/project/roles/testrole/handlers/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       33 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/demo/project/roles/testrole/handlers/main.yml
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.568576 ansible-runner-2.3.5/demo/project/roles/testrole/meta/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     1767 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/demo/project/roles/testrole/meta/main.yml
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.568576 ansible-runner-2.3.5/demo/project/roles/testrole/tasks/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      129 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/demo/project/roles/testrole/tasks/main.yml
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.568576 ansible-runner-2.3.5/demo/project/roles/testrole/tests/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       11 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/demo/project/roles/testrole/tests/inventory
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       67 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/demo/project/roles/testrole/tests/test.yml
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.568576 ansible-runner-2.3.5/demo/project/roles/testrole/vars/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       29 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/demo/project/roles/testrole/vars/main.yml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       51 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/demo/project/test.yml
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.568576 ansible-runner-2.3.5/docs/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      611 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/docs/Makefile
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      225 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/docs/ansible_runner.config.rst
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      445 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/docs/ansible_runner.display_callback.rst
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     1142 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/docs/ansible_runner.rst
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     5594 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/docs/conf.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     1749 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/docs/container.rst
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     5153 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/docs/execution_environments.rst
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     2339 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/docs/external_interface.rst
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     2288 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/docs/index.rst
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     1793 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/docs/install.rst
--rw-rw-r--   0 shrews    (1000) shrews    (1000)    18971 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/docs/intro.rst
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      818 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/docs/make.bat
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       97 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/docs/modules.rst
--rw-rw-r--   0 shrews    (1000) shrews    (1000)    17999 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/docs/python_interface.rst
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     4146 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/docs/remote_jobs.rst
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       36 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/docs/requirements.in
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      625 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/docs/requirements.txt
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     5917 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/docs/standalone.rst
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.556577 ansible-runner-2.3.5/packaging/
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.568576 ansible-runner-2.3.5/packaging/debian/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      129 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/packaging/debian/changelog
--rw-rw-r--   0 shrews    (1000) shrews    (1000)        2 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/packaging/debian/compat
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      802 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/packaging/debian/control
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     9703 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/packaging/debian/copyright
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.572576 ansible-runner-2.3.5/packaging/debian/docker/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      302 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/packaging/debian/docker/Dockerfile
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      284 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/packaging/debian/docker/docker-compose.yml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       32 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/packaging/debian/pydist-overrides
--rwxrwxr-x   0 shrews    (1000) shrews    (1000)      264 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/packaging/debian/rules
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.572576 ansible-runner-2.3.5/packaging/debian/source/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       12 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/packaging/debian/source/format
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.572576 ansible-runner-2.3.5/packaging/rpm/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      236 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/packaging/rpm/Dockerfile.epel-7-x86_64
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      277 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/packaging/rpm/Dockerfile.epel-8-x86_64
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     4832 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/packaging/rpm/ansible-runner.spec.j2
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      460 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/packaging/rpm/docker-compose.yml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      339 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/pytest.ini
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      185 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/requirements.txt
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     1472 2024-02-13 19:16:52.580576 ansible-runner-2.3.5/setup.cfg
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      104 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/setup.py
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.572576 ansible-runner-2.3.5/test/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/__init__.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     2739 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/conftest.py
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.556577 ansible-runner-2.3.5/test/fixtures/
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.560577 ansible-runner-2.3.5/test/fixtures/projects/
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.572576 ansible-runner-2.3.5/test/fixtures/projects/collection_role/
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.556577 ansible-runner-2.3.5/test/fixtures/projects/collection_role/collections/
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.556577 ansible-runner-2.3.5/test/fixtures/projects/collection_role/collections/ansible_collections/
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.556577 ansible-runner-2.3.5/test/fixtures/projects/collection_role/collections/ansible_collections/groovy/
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.572576 ansible-runner-2.3.5/test/fixtures/projects/collection_role/collections/ansible_collections/groovy/peanuts/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/fixtures/projects/collection_role/collections/ansible_collections/groovy/peanuts/README.md
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      290 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/fixtures/projects/collection_role/collections/ansible_collections/groovy/peanuts/galaxy.yml
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.556577 ansible-runner-2.3.5/test/fixtures/projects/collection_role/collections/ansible_collections/groovy/peanuts/roles/
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.556577 ansible-runner-2.3.5/test/fixtures/projects/collection_role/collections/ansible_collections/groovy/peanuts/roles/hello/
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.572576 ansible-runner-2.3.5/test/fixtures/projects/collection_role/collections/ansible_collections/groovy/peanuts/roles/hello/tasks/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       34 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/fixtures/projects/collection_role/collections/ansible_collections/groovy/peanuts/roles/hello/tasks/main.yml
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.572576 ansible-runner-2.3.5/test/fixtures/projects/collection_role/env/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       26 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/fixtures/projects/collection_role/env/envvars
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.572576 ansible-runner-2.3.5/test/fixtures/projects/collection_role/inventory/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      126 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/fixtures/projects/collection_role/inventory/hosts
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       74 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/fixtures/projects/collection_role/use_role.yml
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.556577 ansible-runner-2.3.5/test/fixtures/projects/containerized/
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.572576 ansible-runner-2.3.5/test/fixtures/projects/containerized/env/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       26 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/fixtures/projects/containerized/env/envvars
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       78 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/fixtures/projects/containerized/env/settings
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.572576 ansible-runner-2.3.5/test/fixtures/projects/containerized/inventory/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      126 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/fixtures/projects/containerized/inventory/hosts
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.572576 ansible-runner-2.3.5/test/fixtures/projects/containerized/project/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      266 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/fixtures/projects/containerized/project/test-container.yml
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.556577 ansible-runner-2.3.5/test/fixtures/projects/debug/
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.572576 ansible-runner-2.3.5/test/fixtures/projects/debug/env/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       26 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/fixtures/projects/debug/env/envvars
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.572576 ansible-runner-2.3.5/test/fixtures/projects/debug/inventory/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       91 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/fixtures/projects/debug/inventory/inv_1
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       91 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/fixtures/projects/debug/inventory/inv_2
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.572576 ansible-runner-2.3.5/test/fixtures/projects/debug/project/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       55 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/fixtures/projects/debug/project/debug.yml
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.556577 ansible-runner-2.3.5/test/fixtures/projects/debug/project/roles/
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.556577 ansible-runner-2.3.5/test/fixtures/projects/debug/project/roles/hello_world/
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.572576 ansible-runner-2.3.5/test/fixtures/projects/debug/project/roles/hello_world/tasks/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       62 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/fixtures/projects/debug/project/roles/hello_world/tasks/main.yml
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.556577 ansible-runner-2.3.5/test/fixtures/projects/directory_isolation/
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.572576 ansible-runner-2.3.5/test/fixtures/projects/directory_isolation/env/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      103 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/fixtures/projects/directory_isolation/env/settings
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.572576 ansible-runner-2.3.5/test/fixtures/projects/directory_isolation/project/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       86 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/fixtures/projects/directory_isolation/project/main.yml
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.572576 ansible-runner-2.3.5/test/fixtures/projects/files/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       70 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/fixtures/projects/files/test_ee.py
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.572576 ansible-runner-2.3.5/test/fixtures/projects/host_status/
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.572576 ansible-runner-2.3.5/test/fixtures/projects/host_status/env/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       26 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/fixtures/projects/host_status/env/envvars
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      187 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/fixtures/projects/host_status/inventory
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.572576 ansible-runner-2.3.5/test/fixtures/projects/host_status/project/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     1068 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/fixtures/projects/host_status/project/gen_host_status.yml
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.556577 ansible-runner-2.3.5/test/fixtures/projects/job_env/
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.572576 ansible-runner-2.3.5/test/fixtures/projects/job_env/env/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       42 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/fixtures/projects/job_env/env/envvars
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       28 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/fixtures/projects/job_env/env/settings
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.572576 ansible-runner-2.3.5/test/fixtures/projects/job_env/inventory/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      126 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/fixtures/projects/job_env/inventory/hosts
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.572576 ansible-runner-2.3.5/test/fixtures/projects/job_env/project/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       97 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/fixtures/projects/job_env/project/printenv.yml
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.556577 ansible-runner-2.3.5/test/fixtures/projects/music/
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.556577 ansible-runner-2.3.5/test/fixtures/projects/music/project/
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.556577 ansible-runner-2.3.5/test/fixtures/projects/music/project/roles/
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.556577 ansible-runner-2.3.5/test/fixtures/projects/music/project/roles/Into_The_Mystic/
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.572576 ansible-runner-2.3.5/test/fixtures/projects/music/project/roles/Into_The_Mystic/meta/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      405 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/fixtures/projects/music/project/roles/Into_The_Mystic/meta/argument_specs.yml
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.556577 ansible-runner-2.3.5/test/fixtures/projects/pexpect_timeout_data_loss/
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.572576 ansible-runner-2.3.5/test/fixtures/projects/pexpect_timeout_data_loss/project/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      469 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/fixtures/projects/pexpect_timeout_data_loss/project/pb.yml
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.556577 ansible-runner-2.3.5/test/fixtures/projects/printenv/
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.572576 ansible-runner-2.3.5/test/fixtures/projects/printenv/env/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       26 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/fixtures/projects/printenv/env/envvars
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.572576 ansible-runner-2.3.5/test/fixtures/projects/printenv/inventory/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      126 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/fixtures/projects/printenv/inventory/hosts
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.572576 ansible-runner-2.3.5/test/fixtures/projects/printenv/project/
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.572576 ansible-runner-2.3.5/test/fixtures/projects/printenv/project/action_plugins/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      618 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/fixtures/projects/printenv/project/action_plugins/look_at_environment.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       69 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/fixtures/projects/printenv/project/get_environment.yml
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.560577 ansible-runner-2.3.5/test/fixtures/projects/sleep/
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.572576 ansible-runner-2.3.5/test/fixtures/projects/sleep/env/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       26 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/fixtures/projects/sleep/env/envvars
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.576576 ansible-runner-2.3.5/test/fixtures/projects/sleep/inventory/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      126 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/fixtures/projects/sleep/inventory/hosts
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.576576 ansible-runner-2.3.5/test/fixtures/projects/sleep/project/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      226 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/fixtures/projects/sleep/project/sleep.yml
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.576576 ansible-runner-2.3.5/test/fixtures/projects/use_role/
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.576576 ansible-runner-2.3.5/test/fixtures/projects/use_role/env/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       26 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/fixtures/projects/use_role/env/envvars
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.576576 ansible-runner-2.3.5/test/fixtures/projects/use_role/inventory/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      126 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/fixtures/projects/use_role/inventory/hosts
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.560577 ansible-runner-2.3.5/test/fixtures/projects/use_role/roles/
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.560577 ansible-runner-2.3.5/test/fixtures/projects/use_role/roles/benthomasson.hello_role/
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.576576 ansible-runner-2.3.5/test/fixtures/projects/use_role/roles/benthomasson.hello_role/meta/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       60 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/fixtures/projects/use_role/roles/benthomasson.hello_role/meta/.galaxy_install_info
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      184 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/fixtures/projects/use_role/roles/benthomasson.hello_role/meta/main.yml
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.576576 ansible-runner-2.3.5/test/fixtures/projects/use_role/roles/benthomasson.hello_role/tasks/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       13 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/fixtures/projects/use_role/roles/benthomasson.hello_role/tasks/main.yml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       77 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/fixtures/projects/use_role/use_role.yml
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.576576 ansible-runner-2.3.5/test/integration/
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.576576 ansible-runner-2.3.5/test/integration/callback/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      298 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/integration/callback/other_callback.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     2131 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/integration/conftest.py
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.576576 ansible-runner-2.3.5/test/integration/containerized/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     2350 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/integration/containerized/test_cleanup_images.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     2676 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/integration/containerized/test_cli_containerized.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     5952 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/integration/containerized/test_container_management.py
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.576576 ansible-runner-2.3.5/test/integration/exec_env/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      262 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/integration/exec_env/Containerfile
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     1052 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/integration/exec_env/demo.yml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       87 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/integration/exec_env/inventory.ini
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     4685 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/integration/test___main__.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     1561 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/integration/test_config.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)    13911 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/integration/test_display_callback.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     6796 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/integration/test_events.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)    16766 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/integration/test_interface.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     6042 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/integration/test_main.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     9296 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/integration/test_runner.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)    19164 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/integration/test_transmit_worker_process.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       94 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/requirements.txt
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.576576 ansible-runner-2.3.5/test/unit/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/unit/__init__.py
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.576576 ansible-runner-2.3.5/test/unit/__main__/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/unit/__main__/__init__.py
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.576576 ansible-runner-2.3.5/test/unit/__main__/main/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     1782 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/unit/__main__/main/test_worker.py
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.576576 ansible-runner-2.3.5/test/unit/config/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/unit/config/__init__.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)    12787 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/unit/config/test__base.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     3635 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/unit/config/test_ansible_cfg.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     4062 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/unit/config/test_command.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     7830 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/unit/config/test_container_volmount_generation.py
--rwxrwxr-x   0 shrews    (1000) shrews    (1000)     6317 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/unit/config/test_doc.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     5672 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/unit/config/test_inventory.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)    25407 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/unit/config/test_runner.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      214 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/unit/conftest.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     3074 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/unit/test_cleanup.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     6299 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/unit/test_event_filter.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      914 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/unit/test_interface.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     3727 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/unit/test_loader.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     6937 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/unit/test_runner.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      394 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/unit/test_utils.py
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.580576 ansible-runner-2.3.5/test/unit/utils/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/unit/utils/__init__.py
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.580576 ansible-runner-2.3.5/test/unit/utils/capacity/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/unit/utils/capacity/__init__.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     3125 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/unit/utils/capacity/test_uuid.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      659 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/unit/utils/test_cleanup_folder.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     6476 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/unit/utils/test_dump_artifacts.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      621 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/unit/utils/test_fifo_pipe.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)    10741 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/unit/utils/test_utils.py
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.580576 ansible-runner-2.3.5/test/utils/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     1162 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/test/utils/common.py
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.580576 ansible-runner-2.3.5/tools/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      947 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/tools/bindep.txt
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       24 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/tools/build-requirements.txt
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      187 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/tools/requirements-stable-2.10.txt
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      187 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/tools/requirements-stable-2.11.txt
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      187 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/tools/requirements-stable-2.12.txt
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      182 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/tools/requirements-stable-2.9.txt
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      187 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/tools/requirements.txt
--rwxrwxr-x   0 shrews    (1000) shrews    (1000)      455 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/tools/test-setup.sh
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       18 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/tools/upper-constraints-stable-2.10.txt
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       18 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/tools/upper-constraints-stable-2.11.txt
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       13 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/tools/upper-constraints-stable-2.12.txt
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       13 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/tools/upper-constraints-stable-2.9.txt
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     1341 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/tox.ini
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-02-13 19:16:52.580576 ansible-runner-2.3.5/utils/
--rwxrwxr-x   0 shrews    (1000) shrews    (1000)     4291 2024-02-13 19:16:26.000000 ansible-runner-2.3.5/utils/entrypoint.sh
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.455338 ansible-runner-2.3.6/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      209 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/.cherry_picker.toml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      287 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/.coveragerc
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)        5 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/.dockerignore
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.439338 ansible-runner-2.3.6/.github/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      162 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/.github/CODE_OF_CONDUCT.md
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.439338 ansible-runner-2.3.6/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     1939 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       27 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/.github/ISSUE_TEMPLATE/config.yml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      611 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/.github/ISSUE_TEMPLATE/documentation_report.yml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      588 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       23 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/.github/issue_labeler.yml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      117 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/.github/patchback.yml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       37 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/.github/pr_labeler_existing.yml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       90 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/.github/pr_labeler_new.yml
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.439338 ansible-runner-2.3.6/.github/workflows/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     3011 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/.github/workflows/ci.yml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      763 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/.github/workflows/triage_existing.yml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      734 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/.github/workflows/triage_new.yml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      114 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/.pre-commit-config.yaml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      334 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/.readthedocs.yaml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      466 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/.yamllint
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.439338 ansible-runner-2.3.6/.zuul.d/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     8029 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/.zuul.d/jobs.yaml
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.439338 ansible-runner-2.3.6/.zuul.d/playbooks/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/.zuul.d/playbooks/.zuul.ignore
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.439338 ansible-runner-2.3.6/.zuul.d/playbooks/ansible-runner-container-image-base/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      331 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/.zuul.d/playbooks/ansible-runner-container-image-base/pre.yaml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      795 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/.zuul.d/project.yaml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     4358 2024-03-12 15:20:33.000000 ansible-runner-2.3.6/AUTHORS
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      306 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/CODEOWNERS
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     1422 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/CONTRIBUTING.md
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)    49825 2024-03-12 15:20:33.000000 ansible-runner-2.3.6/ChangeLog
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     2547 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/Dockerfile
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     9304 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/LICENSE.md
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       55 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/MANIFEST.in
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     5345 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/Makefile
+-rw-r--r--   0 shrews    (1000) shrews    (1000)     3505 2024-03-12 15:20:33.455338 ansible-runner-2.3.6/PKG-INFO
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     2044 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/README.md
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      313 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/SECURITY.md
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.443338 ansible-runner-2.3.6/ansible_runner/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      708 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/ansible_runner/__init__.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)    35764 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/ansible_runner/__main__.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     7131 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/ansible_runner/cleanup.py
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.443338 ansible-runner-2.3.6/ansible_runner/config/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/ansible_runner/config/__init__.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)    29029 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/ansible_runner/config/_base.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     3381 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/ansible_runner/config/ansible_cfg.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     4323 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/ansible_runner/config/command.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     6418 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/ansible_runner/config/doc.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     4897 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/ansible_runner/config/inventory.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)    17441 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/ansible_runner/config/runner.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      408 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/ansible_runner/defaults.py
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.443338 ansible-runner-2.3.6/ansible_runner/display_callback/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/ansible_runner/display_callback/__init__.py
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.443338 ansible-runner-2.3.6/ansible_runner/display_callback/callback/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/ansible_runner/display_callback/callback/__init__.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)    31150 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/ansible_runner/display_callback/callback/awx_display.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      256 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/ansible_runner/exceptions.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)    64207 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/ansible_runner/interface.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     5986 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/ansible_runner/loader.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     3008 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/ansible_runner/output.py
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.443338 ansible-runner-2.3.6/ansible_runner/plugins/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/ansible_runner/plugins/__init__.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)    26164 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/ansible_runner/runner.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      905 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/ansible_runner/runner_config.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)    14322 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/ansible_runner/streaming.py
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.443338 ansible-runner-2.3.6/ansible_runner/utils/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)    17031 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/ansible_runner/utils/__init__.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)    11731 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/ansible_runner/utils/base64io.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     1719 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/ansible_runner/utils/capacity.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      159 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/ansible_runner/utils/importlib_compat.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     4931 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/ansible_runner/utils/streaming.py
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.455338 ansible-runner-2.3.6/ansible_runner.egg-info/
+-rw-r--r--   0 shrews    (1000) shrews    (1000)     3505 2024-03-12 15:20:33.000000 ansible-runner-2.3.6/ansible_runner.egg-info/PKG-INFO
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     7516 2024-03-12 15:20:33.000000 ansible-runner-2.3.6/ansible_runner.egg-info/SOURCES.txt
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)        1 2024-03-12 15:20:33.000000 ansible-runner-2.3.6/ansible_runner.egg-info/dependency_links.txt
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       64 2024-03-12 15:20:33.000000 ansible-runner-2.3.6/ansible_runner.egg-info/entry_points.txt
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)        1 2024-03-12 15:20:33.000000 ansible-runner-2.3.6/ansible_runner.egg-info/not-zip-safe
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       47 2024-03-12 15:20:33.000000 ansible-runner-2.3.6/ansible_runner.egg-info/pbr.json
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      107 2024-03-12 15:20:33.000000 ansible-runner-2.3.6/ansible_runner.egg-info/requires.txt
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       15 2024-03-12 15:20:33.000000 ansible-runner-2.3.6/ansible_runner.egg-info/top_level.txt
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      155 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/bindep.txt
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.431338 ansible-runner-2.3.6/demo/
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.443338 ansible-runner-2.3.6/demo/env/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       18 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/demo/env/envvars
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       40 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/demo/env/extravars
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       39 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/demo/env/passwords
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       60 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/demo/env/settings
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/demo/env/ssh_key
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.443338 ansible-runner-2.3.6/demo/inventory/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       94 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/demo/inventory/hosts
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.443338 ansible-runner-2.3.6/demo/project/
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.431338 ansible-runner-2.3.6/demo/project/roles/
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.443338 ansible-runner-2.3.6/demo/project/roles/testrole/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     1328 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/demo/project/roles/testrole/README.md
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.443338 ansible-runner-2.3.6/demo/project/roles/testrole/defaults/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       33 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/demo/project/roles/testrole/defaults/main.yml
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.443338 ansible-runner-2.3.6/demo/project/roles/testrole/handlers/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       33 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/demo/project/roles/testrole/handlers/main.yml
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.443338 ansible-runner-2.3.6/demo/project/roles/testrole/meta/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     1767 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/demo/project/roles/testrole/meta/main.yml
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.443338 ansible-runner-2.3.6/demo/project/roles/testrole/tasks/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      129 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/demo/project/roles/testrole/tasks/main.yml
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.447338 ansible-runner-2.3.6/demo/project/roles/testrole/tests/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       11 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/demo/project/roles/testrole/tests/inventory
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       67 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/demo/project/roles/testrole/tests/test.yml
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.447338 ansible-runner-2.3.6/demo/project/roles/testrole/vars/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       29 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/demo/project/roles/testrole/vars/main.yml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       51 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/demo/project/test.yml
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.447338 ansible-runner-2.3.6/docs/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      611 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/docs/Makefile
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      225 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/docs/ansible_runner.config.rst
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      445 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/docs/ansible_runner.display_callback.rst
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     1142 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/docs/ansible_runner.rst
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     5594 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/docs/conf.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     1749 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/docs/container.rst
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     5153 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/docs/execution_environments.rst
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     2339 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/docs/external_interface.rst
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     2288 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/docs/index.rst
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     1793 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/docs/install.rst
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)    18971 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/docs/intro.rst
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      818 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/docs/make.bat
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       97 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/docs/modules.rst
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)    17999 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/docs/python_interface.rst
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     4146 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/docs/remote_jobs.rst
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       36 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/docs/requirements.in
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      625 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/docs/requirements.txt
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     5917 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/docs/standalone.rst
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.435338 ansible-runner-2.3.6/packaging/
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.447338 ansible-runner-2.3.6/packaging/debian/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      129 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/packaging/debian/changelog
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)        2 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/packaging/debian/compat
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      802 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/packaging/debian/control
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     9703 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/packaging/debian/copyright
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.447338 ansible-runner-2.3.6/packaging/debian/docker/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      302 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/packaging/debian/docker/Dockerfile
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      284 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/packaging/debian/docker/docker-compose.yml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       32 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/packaging/debian/pydist-overrides
+-rwxrwxr-x   0 shrews    (1000) shrews    (1000)      264 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/packaging/debian/rules
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.447338 ansible-runner-2.3.6/packaging/debian/source/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       12 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/packaging/debian/source/format
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.447338 ansible-runner-2.3.6/packaging/rpm/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      236 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/packaging/rpm/Dockerfile.epel-7-x86_64
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      277 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/packaging/rpm/Dockerfile.epel-8-x86_64
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     4832 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/packaging/rpm/ansible-runner.spec.j2
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      460 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/packaging/rpm/docker-compose.yml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      339 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/pytest.ini
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      185 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/requirements.txt
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     1472 2024-03-12 15:20:33.459338 ansible-runner-2.3.6/setup.cfg
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      104 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/setup.py
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.447338 ansible-runner-2.3.6/test/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/__init__.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     2739 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/conftest.py
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.435338 ansible-runner-2.3.6/test/fixtures/
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.435338 ansible-runner-2.3.6/test/fixtures/projects/
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.447338 ansible-runner-2.3.6/test/fixtures/projects/collection_role/
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.435338 ansible-runner-2.3.6/test/fixtures/projects/collection_role/collections/
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.435338 ansible-runner-2.3.6/test/fixtures/projects/collection_role/collections/ansible_collections/
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.435338 ansible-runner-2.3.6/test/fixtures/projects/collection_role/collections/ansible_collections/groovy/
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.447338 ansible-runner-2.3.6/test/fixtures/projects/collection_role/collections/ansible_collections/groovy/peanuts/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/fixtures/projects/collection_role/collections/ansible_collections/groovy/peanuts/README.md
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      290 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/fixtures/projects/collection_role/collections/ansible_collections/groovy/peanuts/galaxy.yml
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.435338 ansible-runner-2.3.6/test/fixtures/projects/collection_role/collections/ansible_collections/groovy/peanuts/roles/
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.435338 ansible-runner-2.3.6/test/fixtures/projects/collection_role/collections/ansible_collections/groovy/peanuts/roles/hello/
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.447338 ansible-runner-2.3.6/test/fixtures/projects/collection_role/collections/ansible_collections/groovy/peanuts/roles/hello/tasks/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       34 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/fixtures/projects/collection_role/collections/ansible_collections/groovy/peanuts/roles/hello/tasks/main.yml
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.447338 ansible-runner-2.3.6/test/fixtures/projects/collection_role/env/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       26 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/fixtures/projects/collection_role/env/envvars
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.447338 ansible-runner-2.3.6/test/fixtures/projects/collection_role/inventory/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      126 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/fixtures/projects/collection_role/inventory/hosts
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       74 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/fixtures/projects/collection_role/use_role.yml
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.435338 ansible-runner-2.3.6/test/fixtures/projects/containerized/
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.447338 ansible-runner-2.3.6/test/fixtures/projects/containerized/env/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       26 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/fixtures/projects/containerized/env/envvars
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       78 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/fixtures/projects/containerized/env/settings
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.447338 ansible-runner-2.3.6/test/fixtures/projects/containerized/inventory/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      126 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/fixtures/projects/containerized/inventory/hosts
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.451338 ansible-runner-2.3.6/test/fixtures/projects/containerized/project/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      266 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/fixtures/projects/containerized/project/test-container.yml
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.435338 ansible-runner-2.3.6/test/fixtures/projects/debug/
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.451338 ansible-runner-2.3.6/test/fixtures/projects/debug/env/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       26 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/fixtures/projects/debug/env/envvars
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.451338 ansible-runner-2.3.6/test/fixtures/projects/debug/inventory/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       91 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/fixtures/projects/debug/inventory/inv_1
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       91 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/fixtures/projects/debug/inventory/inv_2
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.451338 ansible-runner-2.3.6/test/fixtures/projects/debug/project/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       55 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/fixtures/projects/debug/project/debug.yml
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.435338 ansible-runner-2.3.6/test/fixtures/projects/debug/project/roles/
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.435338 ansible-runner-2.3.6/test/fixtures/projects/debug/project/roles/hello_world/
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.451338 ansible-runner-2.3.6/test/fixtures/projects/debug/project/roles/hello_world/tasks/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       62 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/fixtures/projects/debug/project/roles/hello_world/tasks/main.yml
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.435338 ansible-runner-2.3.6/test/fixtures/projects/directory_isolation/
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.451338 ansible-runner-2.3.6/test/fixtures/projects/directory_isolation/env/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      103 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/fixtures/projects/directory_isolation/env/settings
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.451338 ansible-runner-2.3.6/test/fixtures/projects/directory_isolation/project/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       86 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/fixtures/projects/directory_isolation/project/main.yml
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.451338 ansible-runner-2.3.6/test/fixtures/projects/files/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       70 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/fixtures/projects/files/test_ee.py
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.451338 ansible-runner-2.3.6/test/fixtures/projects/host_status/
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.451338 ansible-runner-2.3.6/test/fixtures/projects/host_status/env/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       26 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/fixtures/projects/host_status/env/envvars
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      187 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/fixtures/projects/host_status/inventory
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.451338 ansible-runner-2.3.6/test/fixtures/projects/host_status/project/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     1068 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/fixtures/projects/host_status/project/gen_host_status.yml
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.435338 ansible-runner-2.3.6/test/fixtures/projects/job_env/
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.451338 ansible-runner-2.3.6/test/fixtures/projects/job_env/env/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       42 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/fixtures/projects/job_env/env/envvars
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       28 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/fixtures/projects/job_env/env/settings
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.451338 ansible-runner-2.3.6/test/fixtures/projects/job_env/inventory/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      126 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/fixtures/projects/job_env/inventory/hosts
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.451338 ansible-runner-2.3.6/test/fixtures/projects/job_env/project/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       97 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/fixtures/projects/job_env/project/printenv.yml
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.435338 ansible-runner-2.3.6/test/fixtures/projects/music/
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.435338 ansible-runner-2.3.6/test/fixtures/projects/music/project/
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.435338 ansible-runner-2.3.6/test/fixtures/projects/music/project/roles/
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.435338 ansible-runner-2.3.6/test/fixtures/projects/music/project/roles/Into_The_Mystic/
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.451338 ansible-runner-2.3.6/test/fixtures/projects/music/project/roles/Into_The_Mystic/meta/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      405 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/fixtures/projects/music/project/roles/Into_The_Mystic/meta/argument_specs.yml
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.435338 ansible-runner-2.3.6/test/fixtures/projects/pexpect_timeout_data_loss/
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.451338 ansible-runner-2.3.6/test/fixtures/projects/pexpect_timeout_data_loss/project/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      469 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/fixtures/projects/pexpect_timeout_data_loss/project/pb.yml
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.435338 ansible-runner-2.3.6/test/fixtures/projects/printenv/
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.451338 ansible-runner-2.3.6/test/fixtures/projects/printenv/env/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       26 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/fixtures/projects/printenv/env/envvars
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.451338 ansible-runner-2.3.6/test/fixtures/projects/printenv/inventory/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      126 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/fixtures/projects/printenv/inventory/hosts
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.451338 ansible-runner-2.3.6/test/fixtures/projects/printenv/project/
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.451338 ansible-runner-2.3.6/test/fixtures/projects/printenv/project/action_plugins/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      618 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/fixtures/projects/printenv/project/action_plugins/look_at_environment.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       69 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/fixtures/projects/printenv/project/get_environment.yml
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.435338 ansible-runner-2.3.6/test/fixtures/projects/sleep/
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.451338 ansible-runner-2.3.6/test/fixtures/projects/sleep/env/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       26 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/fixtures/projects/sleep/env/envvars
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.451338 ansible-runner-2.3.6/test/fixtures/projects/sleep/inventory/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      126 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/fixtures/projects/sleep/inventory/hosts
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.451338 ansible-runner-2.3.6/test/fixtures/projects/sleep/project/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      226 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/fixtures/projects/sleep/project/sleep.yml
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.451338 ansible-runner-2.3.6/test/fixtures/projects/use_role/
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.451338 ansible-runner-2.3.6/test/fixtures/projects/use_role/env/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       26 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/fixtures/projects/use_role/env/envvars
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.451338 ansible-runner-2.3.6/test/fixtures/projects/use_role/inventory/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      126 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/fixtures/projects/use_role/inventory/hosts
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.435338 ansible-runner-2.3.6/test/fixtures/projects/use_role/roles/
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.435338 ansible-runner-2.3.6/test/fixtures/projects/use_role/roles/benthomasson.hello_role/
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.451338 ansible-runner-2.3.6/test/fixtures/projects/use_role/roles/benthomasson.hello_role/meta/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       60 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/fixtures/projects/use_role/roles/benthomasson.hello_role/meta/.galaxy_install_info
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      184 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/fixtures/projects/use_role/roles/benthomasson.hello_role/meta/main.yml
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.451338 ansible-runner-2.3.6/test/fixtures/projects/use_role/roles/benthomasson.hello_role/tasks/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       13 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/fixtures/projects/use_role/roles/benthomasson.hello_role/tasks/main.yml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       77 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/fixtures/projects/use_role/use_role.yml
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.451338 ansible-runner-2.3.6/test/integration/
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.451338 ansible-runner-2.3.6/test/integration/callback/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      298 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/integration/callback/other_callback.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     2131 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/integration/conftest.py
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.451338 ansible-runner-2.3.6/test/integration/containerized/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     2350 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/integration/containerized/test_cleanup_images.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     2676 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/integration/containerized/test_cli_containerized.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     5952 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/integration/containerized/test_container_management.py
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.455338 ansible-runner-2.3.6/test/integration/exec_env/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      262 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/integration/exec_env/Containerfile
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     1052 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/integration/exec_env/demo.yml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       87 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/integration/exec_env/inventory.ini
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     4685 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/integration/test___main__.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     1561 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/integration/test_config.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)    13911 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/integration/test_display_callback.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     6796 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/integration/test_events.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)    16766 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/integration/test_interface.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     6042 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/integration/test_main.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     9296 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/integration/test_runner.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)    19164 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/integration/test_transmit_worker_process.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       94 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/requirements.txt
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.455338 ansible-runner-2.3.6/test/unit/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/unit/__init__.py
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.455338 ansible-runner-2.3.6/test/unit/__main__/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/unit/__main__/__init__.py
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.455338 ansible-runner-2.3.6/test/unit/__main__/main/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     1782 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/unit/__main__/main/test_worker.py
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.455338 ansible-runner-2.3.6/test/unit/config/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/unit/config/__init__.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)    12787 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/unit/config/test__base.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     3635 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/unit/config/test_ansible_cfg.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     4062 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/unit/config/test_command.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     7830 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/unit/config/test_container_volmount_generation.py
+-rwxrwxr-x   0 shrews    (1000) shrews    (1000)     6317 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/unit/config/test_doc.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     5672 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/unit/config/test_inventory.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)    25407 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/unit/config/test_runner.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      214 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/unit/conftest.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     3074 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/unit/test_cleanup.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     6299 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/unit/test_event_filter.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      914 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/unit/test_interface.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     3727 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/unit/test_loader.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     6937 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/unit/test_runner.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      394 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/unit/test_utils.py
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.455338 ansible-runner-2.3.6/test/unit/utils/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/unit/utils/__init__.py
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.455338 ansible-runner-2.3.6/test/unit/utils/capacity/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/unit/utils/capacity/__init__.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     3125 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/unit/utils/capacity/test_uuid.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      659 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/unit/utils/test_cleanup_folder.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     6476 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/unit/utils/test_dump_artifacts.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      621 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/unit/utils/test_fifo_pipe.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)    10741 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/unit/utils/test_utils.py
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.455338 ansible-runner-2.3.6/test/utils/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     1162 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/test/utils/common.py
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.455338 ansible-runner-2.3.6/tools/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      947 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/tools/bindep.txt
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       24 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/tools/build-requirements.txt
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      187 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/tools/requirements-stable-2.10.txt
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      187 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/tools/requirements-stable-2.11.txt
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      187 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/tools/requirements-stable-2.12.txt
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      182 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/tools/requirements-stable-2.9.txt
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      187 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/tools/requirements.txt
+-rwxrwxr-x   0 shrews    (1000) shrews    (1000)      455 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/tools/test-setup.sh
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       18 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/tools/upper-constraints-stable-2.10.txt
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       18 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/tools/upper-constraints-stable-2.11.txt
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       13 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/tools/upper-constraints-stable-2.12.txt
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       13 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/tools/upper-constraints-stable-2.9.txt
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     1341 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/tox.ini
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2024-03-12 15:20:33.455338 ansible-runner-2.3.6/utils/
+-rwxrwxr-x   0 shrews    (1000) shrews    (1000)     4291 2024-03-12 15:20:03.000000 ansible-runner-2.3.6/utils/entrypoint.sh
```

### Comparing `ansible-runner-2.3.5/.github/ISSUE_TEMPLATE/bug_report.yml` & `ansible-runner-2.3.6/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/.github/ISSUE_TEMPLATE/documentation_report.yml` & `ansible-runner-2.3.6/.github/ISSUE_TEMPLATE/documentation_report.yml`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/.github/ISSUE_TEMPLATE/feature_request.yml` & `ansible-runner-2.3.6/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/.github/workflows/ci.yml` & `ansible-runner-2.3.6/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/.github/workflows/triage_existing.yml` & `ansible-runner-2.3.6/.github/workflows/triage_existing.yml`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/.github/workflows/triage_new.yml` & `ansible-runner-2.3.6/.github/workflows/triage_new.yml`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/.zuul.d/jobs.yaml` & `ansible-runner-2.3.6/.zuul.d/jobs.yaml`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/.zuul.d/project.yaml` & `ansible-runner-2.3.6/.zuul.d/project.yaml`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/AUTHORS` & `ansible-runner-2.3.6/AUTHORS`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/CONTRIBUTING.md` & `ansible-runner-2.3.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/ChangeLog` & `ansible-runner-2.3.6/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 CHANGES
 =======
 
+2.3.6
+-----
+
+* Untag instead of force remove image for podman (#1342) (#1344)
+
 2.3.5
 -----
 
 * fix pexpect child shutdown race (#1331) (#1336)
 
 2.3.4
 -----
```

### Comparing `ansible-runner-2.3.5/Dockerfile` & `ansible-runner-2.3.6/Dockerfile`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/LICENSE.md` & `ansible-runner-2.3.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/Makefile` & `ansible-runner-2.3.6/Makefile`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/PKG-INFO` & `ansible-runner-2.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-runner
-Version: 2.3.5
+Version: 2.3.6
 Summary: "Consistent Ansible Python API and CLI with container and process isolation runtime capabilities"
 Home-page: https://ansible-runner.readthedocs.io
 Author: Ansible, Inc.
 Author-email: info@ansible.com
 License: Apache Software License, Version 2.0
 Project-URL: Source, https://github.com/ansible/ansible-runner
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ansible-runner-2.3.5/README.md` & `ansible-runner-2.3.6/README.md`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/ansible_runner/__init__.py` & `ansible-runner-2.3.6/ansible_runner/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/ansible_runner/__main__.py` & `ansible-runner-2.3.6/ansible_runner/__main__.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/ansible_runner/cleanup.py` & `ansible-runner-2.3.6/ansible_runner/cleanup.py`

 * *Files 6% similar despite different names*

```diff
@@ -140,23 +140,37 @@
         if changed:
             ct += 1
 
     return ct
 
 
 def cleanup_images(images, runtime='podman'):
-    """Note: docker will just untag while podman will remove layers with same command"""
+    """
+    `docker rmi` will just untag while
+    `podman rmi` will untag and remove layers and cause runing container to be killed
+    for podman we use `untag` to achieve the same behavior
+
+    NOTE: this only untag the image and does not delete the image prune_images need to be call to delete
+    """
     rm_ct = 0
     for image_tag in images:
         stdout = run_command([runtime, 'images', '--format="{{.Repository}}:{{.Tag}}"', image_tag])
         if not stdout:
             continue
         for discovered_tag in stdout.split('\n'):
-            stdout = run_command([runtime, 'rmi', discovered_tag.strip().strip('"'), '-f'])
-            rm_ct += stdout.count('Untagged:')
+            if runtime == 'podman':
+                try:
+                    stdout = run_command([runtime, 'untag', image_tag])
+                    if not stdout:
+                        rm_ct += 1
+                except Exception:
+                    pass  # best effort untag
+            else:
+                stdout = run_command([runtime, 'rmi', discovered_tag.strip().strip('"'), '-f'])
+                rm_ct += stdout.count('Untagged:')
     return rm_ct
 
 
 def prune_images(runtime='podman'):
     """Run the prune images command and return changed status"""
     stdout = run_command([runtime, 'image', 'prune', '-f'])
     if not stdout or stdout == "Total reclaimed space: 0B":
```

### Comparing `ansible-runner-2.3.5/ansible_runner/config/_base.py` & `ansible-runner-2.3.6/ansible_runner/config/_base.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/ansible_runner/config/ansible_cfg.py` & `ansible-runner-2.3.6/ansible_runner/config/ansible_cfg.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/ansible_runner/config/command.py` & `ansible-runner-2.3.6/ansible_runner/config/command.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/ansible_runner/config/doc.py` & `ansible-runner-2.3.6/ansible_runner/config/doc.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/ansible_runner/config/inventory.py` & `ansible-runner-2.3.6/ansible_runner/config/inventory.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/ansible_runner/config/runner.py` & `ansible-runner-2.3.6/ansible_runner/config/runner.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/ansible_runner/display_callback/callback/awx_display.py` & `ansible-runner-2.3.6/ansible_runner/display_callback/callback/awx_display.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/ansible_runner/interface.py` & `ansible-runner-2.3.6/ansible_runner/interface.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/ansible_runner/loader.py` & `ansible-runner-2.3.6/ansible_runner/loader.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/ansible_runner/output.py` & `ansible-runner-2.3.6/ansible_runner/output.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/ansible_runner/runner.py` & `ansible-runner-2.3.6/ansible_runner/runner.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/ansible_runner/runner_config.py` & `ansible-runner-2.3.6/ansible_runner/runner_config.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/ansible_runner/streaming.py` & `ansible-runner-2.3.6/ansible_runner/streaming.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/ansible_runner/utils/__init__.py` & `ansible-runner-2.3.6/ansible_runner/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/ansible_runner/utils/base64io.py` & `ansible-runner-2.3.6/ansible_runner/utils/base64io.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/ansible_runner/utils/capacity.py` & `ansible-runner-2.3.6/ansible_runner/utils/capacity.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/ansible_runner/utils/streaming.py` & `ansible-runner-2.3.6/ansible_runner/utils/streaming.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/ansible_runner.egg-info/PKG-INFO` & `ansible-runner-2.3.6/ansible_runner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-runner
-Version: 2.3.5
+Version: 2.3.6
 Summary: "Consistent Ansible Python API and CLI with container and process isolation runtime capabilities"
 Home-page: https://ansible-runner.readthedocs.io
 Author: Ansible, Inc.
 Author-email: info@ansible.com
 License: Apache Software License, Version 2.0
 Project-URL: Source, https://github.com/ansible/ansible-runner
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ansible-runner-2.3.5/ansible_runner.egg-info/SOURCES.txt` & `ansible-runner-2.3.6/ansible_runner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/demo/project/roles/testrole/README.md` & `ansible-runner-2.3.6/demo/project/roles/testrole/README.md`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/demo/project/roles/testrole/meta/main.yml` & `ansible-runner-2.3.6/demo/project/roles/testrole/meta/main.yml`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/docs/Makefile` & `ansible-runner-2.3.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/docs/ansible_runner.rst` & `ansible-runner-2.3.6/docs/ansible_runner.rst`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/docs/conf.py` & `ansible-runner-2.3.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/docs/container.rst` & `ansible-runner-2.3.6/docs/container.rst`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/docs/execution_environments.rst` & `ansible-runner-2.3.6/docs/execution_environments.rst`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/docs/external_interface.rst` & `ansible-runner-2.3.6/docs/external_interface.rst`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/docs/index.rst` & `ansible-runner-2.3.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/docs/install.rst` & `ansible-runner-2.3.6/docs/install.rst`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/docs/intro.rst` & `ansible-runner-2.3.6/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/docs/make.bat` & `ansible-runner-2.3.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/docs/python_interface.rst` & `ansible-runner-2.3.6/docs/python_interface.rst`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/docs/remote_jobs.rst` & `ansible-runner-2.3.6/docs/remote_jobs.rst`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/docs/requirements.txt` & `ansible-runner-2.3.6/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/docs/standalone.rst` & `ansible-runner-2.3.6/docs/standalone.rst`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/packaging/debian/control` & `ansible-runner-2.3.6/packaging/debian/control`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/packaging/debian/copyright` & `ansible-runner-2.3.6/packaging/debian/copyright`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/packaging/rpm/ansible-runner.spec.j2` & `ansible-runner-2.3.6/packaging/rpm/ansible-runner.spec.j2`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/setup.cfg` & `ansible-runner-2.3.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/test/conftest.py` & `ansible-runner-2.3.6/test/conftest.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/test/fixtures/projects/host_status/project/gen_host_status.yml` & `ansible-runner-2.3.6/test/fixtures/projects/host_status/project/gen_host_status.yml`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/test/fixtures/projects/printenv/project/action_plugins/look_at_environment.py` & `ansible-runner-2.3.6/test/fixtures/projects/printenv/project/action_plugins/look_at_environment.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/test/integration/conftest.py` & `ansible-runner-2.3.6/test/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/test/integration/containerized/test_cleanup_images.py` & `ansible-runner-2.3.6/test/integration/containerized/test_cleanup_images.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/test/integration/containerized/test_cli_containerized.py` & `ansible-runner-2.3.6/test/integration/containerized/test_cli_containerized.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/test/integration/containerized/test_container_management.py` & `ansible-runner-2.3.6/test/integration/containerized/test_container_management.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/test/integration/exec_env/demo.yml` & `ansible-runner-2.3.6/test/integration/exec_env/demo.yml`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/test/integration/test___main__.py` & `ansible-runner-2.3.6/test/integration/test___main__.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/test/integration/test_config.py` & `ansible-runner-2.3.6/test/integration/test_config.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/test/integration/test_display_callback.py` & `ansible-runner-2.3.6/test/integration/test_display_callback.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/test/integration/test_events.py` & `ansible-runner-2.3.6/test/integration/test_events.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/test/integration/test_interface.py` & `ansible-runner-2.3.6/test/integration/test_interface.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/test/integration/test_main.py` & `ansible-runner-2.3.6/test/integration/test_main.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/test/integration/test_runner.py` & `ansible-runner-2.3.6/test/integration/test_runner.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/test/integration/test_transmit_worker_process.py` & `ansible-runner-2.3.6/test/integration/test_transmit_worker_process.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/test/unit/__main__/main/test_worker.py` & `ansible-runner-2.3.6/test/unit/__main__/main/test_worker.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/test/unit/config/test__base.py` & `ansible-runner-2.3.6/test/unit/config/test__base.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/test/unit/config/test_ansible_cfg.py` & `ansible-runner-2.3.6/test/unit/config/test_ansible_cfg.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/test/unit/config/test_command.py` & `ansible-runner-2.3.6/test/unit/config/test_command.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/test/unit/config/test_container_volmount_generation.py` & `ansible-runner-2.3.6/test/unit/config/test_container_volmount_generation.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/test/unit/config/test_doc.py` & `ansible-runner-2.3.6/test/unit/config/test_doc.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/test/unit/config/test_inventory.py` & `ansible-runner-2.3.6/test/unit/config/test_inventory.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/test/unit/config/test_runner.py` & `ansible-runner-2.3.6/test/unit/config/test_runner.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/test/unit/test_cleanup.py` & `ansible-runner-2.3.6/test/unit/test_cleanup.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/test/unit/test_event_filter.py` & `ansible-runner-2.3.6/test/unit/test_event_filter.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/test/unit/test_interface.py` & `ansible-runner-2.3.6/test/unit/test_interface.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/test/unit/test_loader.py` & `ansible-runner-2.3.6/test/unit/test_loader.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/test/unit/test_runner.py` & `ansible-runner-2.3.6/test/unit/test_runner.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/test/unit/utils/capacity/test_uuid.py` & `ansible-runner-2.3.6/test/unit/utils/capacity/test_uuid.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/test/unit/utils/test_cleanup_folder.py` & `ansible-runner-2.3.6/test/unit/utils/test_cleanup_folder.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/test/unit/utils/test_dump_artifacts.py` & `ansible-runner-2.3.6/test/unit/utils/test_dump_artifacts.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/test/unit/utils/test_fifo_pipe.py` & `ansible-runner-2.3.6/test/unit/utils/test_fifo_pipe.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/test/unit/utils/test_utils.py` & `ansible-runner-2.3.6/test/unit/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/test/utils/common.py` & `ansible-runner-2.3.6/test/utils/common.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/tools/bindep.txt` & `ansible-runner-2.3.6/tools/bindep.txt`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/tox.ini` & `ansible-runner-2.3.6/tox.ini`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.5/utils/entrypoint.sh` & `ansible-runner-2.3.6/utils/entrypoint.sh`

 * *Files identical despite different names*

