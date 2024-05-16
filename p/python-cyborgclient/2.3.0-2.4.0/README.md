# Comparing `tmp/python-cyborgclient-2.3.0.tar.gz` & `tmp/python-cyborgclient-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-cyborgclient-2.3.0.tar", last modified: Thu Nov 16 10:44:04 2023, max compression
+gzip compressed data, was "python-cyborgclient-2.4.0.tar", last modified: Thu May 16 12:53:17 2024, max compression
```

## Comparing `python-cyborgclient-2.3.0.tar` & `python-cyborgclient-2.4.0.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-16 10:44:04.887836 python-cyborgclient-2.3.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1323 2023-11-16 10:44:04.000000 python-cyborgclient-2.3.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      649 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5007 2023-11-16 10:44:04.000000 python-cyborgclient-2.3.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5946 2023-11-16 10:44:04.887836 python-cyborgclient-2.3.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4171 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-16 10:44:04.863836 python-cyborgclient-2.3.0/cyborgclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      675 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-16 10:44:04.867836 python-cyborgclient-2.3.0/cyborgclient/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/common/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-16 10:44:04.867836 python-cyborgclient-2.3.0/cyborgclient/common/apiclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/common/apiclient/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3516 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/common/apiclient/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12412 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/common/apiclient/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4704 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/common/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16061 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/common/cliutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13131 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/common/http.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16234 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/common/httpclient.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4955 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/common/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15110 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      767 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/i18n.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-16 10:44:04.867836 python-cyborgclient-2.3.0/cyborgclient/osc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/osc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4094 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/osc/plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-16 10:44:04.867836 python-cyborgclient-2.3.0/cyborgclient/osc/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/osc/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2039 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/osc/v1/accelerator.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-16 10:44:04.871836 python-cyborgclient-2.3.0/cyborgclient/osc/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/osc/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10625 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/osc/v2/accelerator_request.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5900 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/osc/v2/attribute.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5283 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/osc/v2/deployable.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5452 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/osc/v2/device.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6333 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/osc/v2/device_profile.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26205 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/shell.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-16 10:44:04.871836 python-cyborgclient-2.3.0/cyborgclient/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      794 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/tests/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-16 10:44:04.871836 python-cyborgclient-2.3.0/cyborgclient/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/tests/functional/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      788 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/tests/test_cyborgclient.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-16 10:44:04.871836 python-cyborgclient-2.3.0/cyborgclient/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/tests/unit/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1895 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/tests/unit/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-16 10:44:04.871836 python-cyborgclient-2.3.0/cyborgclient/tests/unit/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/tests/unit/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12756 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/tests/unit/common/test_httpclient.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1509 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/tests/unit/common/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-16 10:44:04.871836 python-cyborgclient-2.3.0/cyborgclient/tests/unit/osc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/tests/unit/osc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1845 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/tests/unit/osc/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2503 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/tests/unit/osc/test_plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-16 10:44:04.875836 python-cyborgclient-2.3.0/cyborgclient/tests/unit/osc/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/tests/unit/osc/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4728 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/tests/unit/osc/v2/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9514 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/tests/unit/osc/v2/test_accelerator_request.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7509 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/tests/unit/osc/v2/test_attribute.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7189 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/tests/unit/osc/v2/test_deployable.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5107 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/tests/unit/osc/v2/test_device.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9338 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/tests/unit/osc/v2/test_device_profile.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11138 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/tests/unit/test_shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5689 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/tests/unit/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-16 10:44:04.875836 python-cyborgclient-2.3.0/cyborgclient/tests/unit/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/tests/unit/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1882 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/tests/unit/v1/shell_test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2847 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/tests/unit/v1/test_accelerators.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      842 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/tests/unit/v1/test_accelerators_shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2634 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/tests/unit/v1/test_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6284 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/tests/unit/v1/test_deployables.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-16 10:44:04.879836 python-cyborgclient-2.3.0/cyborgclient/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      949 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/v1/accelerators.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1663 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/v1/accelerators_shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4208 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/v1/basemodels.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7165 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/v1/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2796 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/v1/deployables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      685 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/v1/shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      659 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/cyborgclient/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-16 10:44:04.879836 python-cyborgclient-2.3.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-16 10:44:04.879836 python-cyborgclient-2.3.0/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-16 10:44:04.879836 python-cyborgclient-2.3.0/doc/source/admin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/doc/source/admin/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-16 10:44:04.879836 python-cyborgclient-2.3.0/doc/source/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/doc/source/cli/index.rst
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2587 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-16 10:44:04.879836 python-cyborgclient-2.3.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1936 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/doc/source/contributor/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      801 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-16 10:44:04.879836 python-cyborgclient-2.3.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      307 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-16 10:44:04.879836 python-cyborgclient-2.3.0/doc/source/library/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/doc/source/library/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/doc/source/readme.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-16 10:44:04.879836 python-cyborgclient-2.3.0/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       69 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/doc/source/reference/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-16 10:44:04.879836 python-cyborgclient-2.3.0/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/doc/source/user/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-16 10:44:04.883836 python-cyborgclient-2.3.0/python_cyborgclient.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5946 2023-11-16 10:44:04.000000 python-cyborgclient-2.3.0/python_cyborgclient.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3643 2023-11-16 10:44:04.000000 python-cyborgclient-2.3.0/python_cyborgclient.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-11-16 10:44:04.000000 python-cyborgclient-2.3.0/python_cyborgclient.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1952 2023-11-16 10:44:04.000000 python-cyborgclient-2.3.0/python_cyborgclient.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-11-16 10:44:04.000000 python-cyborgclient-2.3.0/python_cyborgclient.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-11-16 10:44:04.000000 python-cyborgclient-2.3.0/python_cyborgclient.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      280 2023-11-16 10:44:04.000000 python-cyborgclient-2.3.0/python_cyborgclient.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2023-11-16 10:44:04.000000 python-cyborgclient-2.3.0/python_cyborgclient.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-16 10:44:04.859836 python-cyborgclient-2.3.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-16 10:44:04.883836 python-cyborgclient-2.3.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/releasenotes/notes/drop-py-2-7-d47826d4387f40fe.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/releasenotes/notes/show-dp-by-name-4d22b106b718f215.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      294 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/releasenotes/notes/support-project-id-931fc61c818da675.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-16 10:44:04.887836 python-cyborgclient-2.3.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/releasenotes/source/2023.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/releasenotes/source/2023.2.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-16 10:44:04.887836 python-cyborgclient-2.3.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-16 10:44:04.887836 python-cyborgclient-2.3.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8815 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      663 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2808 2023-11-16 10:44:04.887836 python-cyborgclient-2.3.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      434 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1606 2023-11-16 10:43:21.000000 python-cyborgclient-2.3.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:53:17.133520 python-cyborgclient-2.4.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1323 2024-05-16 12:53:17.000000 python-cyborgclient-2.4.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      649 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5061 2024-05-16 12:53:17.000000 python-cyborgclient-2.4.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6048 2024-05-16 12:53:17.133520 python-cyborgclient-2.4.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4171 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:53:17.125520 python-cyborgclient-2.4.0/cyborgclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      675 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:53:17.125520 python-cyborgclient-2.4.0/cyborgclient/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/common/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:53:17.125520 python-cyborgclient-2.4.0/cyborgclient/common/apiclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/common/apiclient/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3516 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/common/apiclient/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12412 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/common/apiclient/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4704 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/common/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16061 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/common/cliutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13131 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/common/http.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16234 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/common/httpclient.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4955 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/common/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15110 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      767 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/i18n.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:53:17.125520 python-cyborgclient-2.4.0/cyborgclient/osc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/osc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4094 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/osc/plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:53:17.125520 python-cyborgclient-2.4.0/cyborgclient/osc/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/osc/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2039 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/osc/v1/accelerator.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:53:17.125520 python-cyborgclient-2.4.0/cyborgclient/osc/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/osc/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10625 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/osc/v2/accelerator_request.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5900 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/osc/v2/attribute.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5283 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/osc/v2/deployable.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5452 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/osc/v2/device.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6333 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/osc/v2/device_profile.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26205 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/shell.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:53:17.129520 python-cyborgclient-2.4.0/cyborgclient/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      794 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/tests/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:53:17.129520 python-cyborgclient-2.4.0/cyborgclient/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/tests/functional/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      788 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/tests/test_cyborgclient.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:53:17.129520 python-cyborgclient-2.4.0/cyborgclient/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/tests/unit/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1895 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/tests/unit/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:53:17.129520 python-cyborgclient-2.4.0/cyborgclient/tests/unit/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/tests/unit/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12756 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/tests/unit/common/test_httpclient.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1509 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/tests/unit/common/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:53:17.129520 python-cyborgclient-2.4.0/cyborgclient/tests/unit/osc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/tests/unit/osc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1845 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/tests/unit/osc/fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2503 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/tests/unit/osc/test_plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:53:17.129520 python-cyborgclient-2.4.0/cyborgclient/tests/unit/osc/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/tests/unit/osc/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4728 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/tests/unit/osc/v2/fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9514 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/tests/unit/osc/v2/test_accelerator_request.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7509 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/tests/unit/osc/v2/test_attribute.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7189 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/tests/unit/osc/v2/test_deployable.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5107 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/tests/unit/osc/v2/test_device.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9338 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/tests/unit/osc/v2/test_device_profile.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11138 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/tests/unit/test_shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5689 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/tests/unit/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:53:17.129520 python-cyborgclient-2.4.0/cyborgclient/tests/unit/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/tests/unit/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1882 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/tests/unit/v1/shell_test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2847 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/tests/unit/v1/test_accelerators.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      842 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/tests/unit/v1/test_accelerators_shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2634 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/tests/unit/v1/test_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6284 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/tests/unit/v1/test_deployables.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:53:17.129520 python-cyborgclient-2.4.0/cyborgclient/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      949 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/v1/accelerators.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1663 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/v1/accelerators_shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4208 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/v1/basemodels.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7165 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/v1/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2796 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/v1/deployables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      685 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/v1/shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      659 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/cyborgclient/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:53:17.129520 python-cyborgclient-2.4.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:53:17.129520 python-cyborgclient-2.4.0/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:53:17.129520 python-cyborgclient-2.4.0/doc/source/admin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/doc/source/admin/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:53:17.129520 python-cyborgclient-2.4.0/doc/source/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/doc/source/cli/index.rst
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2587 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:53:17.129520 python-cyborgclient-2.4.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1936 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/doc/source/contributor/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      801 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:53:17.129520 python-cyborgclient-2.4.0/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      307 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:53:17.129520 python-cyborgclient-2.4.0/doc/source/library/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/doc/source/library/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/doc/source/readme.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:53:17.129520 python-cyborgclient-2.4.0/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       69 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/doc/source/reference/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:53:17.129520 python-cyborgclient-2.4.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/doc/source/user/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:53:17.129520 python-cyborgclient-2.4.0/python_cyborgclient.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6048 2024-05-16 12:53:17.000000 python-cyborgclient-2.4.0/python_cyborgclient.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3643 2024-05-16 12:53:17.000000 python-cyborgclient-2.4.0/python_cyborgclient.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-16 12:53:17.000000 python-cyborgclient-2.4.0/python_cyborgclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1952 2024-05-16 12:53:17.000000 python-cyborgclient-2.4.0/python_cyborgclient.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-16 12:53:17.000000 python-cyborgclient-2.4.0/python_cyborgclient.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-05-16 12:53:17.000000 python-cyborgclient-2.4.0/python_cyborgclient.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      280 2024-05-16 12:53:17.000000 python-cyborgclient-2.4.0/python_cyborgclient.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2024-05-16 12:53:17.000000 python-cyborgclient-2.4.0/python_cyborgclient.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:53:17.125520 python-cyborgclient-2.4.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:53:17.133520 python-cyborgclient-2.4.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/releasenotes/notes/drop-py-2-7-d47826d4387f40fe.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/releasenotes/notes/show-dp-by-name-4d22b106b718f215.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      294 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/releasenotes/notes/support-project-id-931fc61c818da675.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:53:17.133520 python-cyborgclient-2.4.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/releasenotes/source/2023.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/releasenotes/source/2023.2.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:53:17.133520 python-cyborgclient-2.4.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:53:17.133520 python-cyborgclient-2.4.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8815 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      663 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2888 2024-05-16 12:53:17.133520 python-cyborgclient-2.4.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      434 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1606 2024-05-16 12:52:52.000000 python-cyborgclient-2.4.0/tox.ini
```

### Comparing `python-cyborgclient-2.3.0/AUTHORS` & `python-cyborgclient-2.4.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/CONTRIBUTING.rst` & `python-cyborgclient-2.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/ChangeLog` & `python-cyborgclient-2.4.0/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 CHANGES
 =======
 
+2.4.0
+-----
+
+* Update python classifier in setup.cfg
+
 2.3.0
 -----
 
 * Update master for stable/2023.2
 * Add client api for enable and disable device
 * resolve keyerror for string format
 * add ut for delete attribute client exception error
```

### Comparing `python-cyborgclient-2.3.0/LICENSE` & `python-cyborgclient-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/PKG-INFO` & `python-cyborgclient-2.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: python-cyborgclient
-Version: 2.3.0
+Version: 2.4.0
 Summary: Python client for cyborg API
 Home-page: https://docs.openstack.org/python-cyborgclient/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
@@ -126,8 +126,10 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
```

### Comparing `python-cyborgclient-2.3.0/README.rst` & `python-cyborgclient-2.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/cyborgclient/__init__.py` & `python-cyborgclient-2.4.0/cyborgclient/__init__.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/cyborgclient/common/apiclient/base.py` & `python-cyborgclient-2.4.0/cyborgclient/common/apiclient/base.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/cyborgclient/common/apiclient/exceptions.py` & `python-cyborgclient-2.4.0/cyborgclient/common/apiclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/cyborgclient/common/base.py` & `python-cyborgclient-2.4.0/cyborgclient/common/base.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/cyborgclient/common/cliutils.py` & `python-cyborgclient-2.4.0/cyborgclient/common/cliutils.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/cyborgclient/common/http.py` & `python-cyborgclient-2.4.0/cyborgclient/common/http.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/cyborgclient/common/httpclient.py` & `python-cyborgclient-2.4.0/cyborgclient/common/httpclient.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/cyborgclient/common/utils.py` & `python-cyborgclient-2.4.0/cyborgclient/common/utils.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/cyborgclient/exceptions.py` & `python-cyborgclient-2.4.0/cyborgclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/cyborgclient/i18n.py` & `python-cyborgclient-2.4.0/cyborgclient/i18n.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/cyborgclient/osc/plugin.py` & `python-cyborgclient-2.4.0/cyborgclient/osc/plugin.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/cyborgclient/osc/v1/accelerator.py` & `python-cyborgclient-2.4.0/cyborgclient/osc/v1/accelerator.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/cyborgclient/osc/v2/accelerator_request.py` & `python-cyborgclient-2.4.0/cyborgclient/osc/v2/accelerator_request.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/cyborgclient/osc/v2/attribute.py` & `python-cyborgclient-2.4.0/cyborgclient/osc/v2/attribute.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/cyborgclient/osc/v2/deployable.py` & `python-cyborgclient-2.4.0/cyborgclient/osc/v2/deployable.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/cyborgclient/osc/v2/device.py` & `python-cyborgclient-2.4.0/cyborgclient/osc/v2/device.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/cyborgclient/osc/v2/device_profile.py` & `python-cyborgclient-2.4.0/cyborgclient/osc/v2/device_profile.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/cyborgclient/shell.py` & `python-cyborgclient-2.4.0/cyborgclient/shell.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/cyborgclient/tests/base.py` & `python-cyborgclient-2.4.0/cyborgclient/tests/base.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/cyborgclient/tests/test_cyborgclient.py` & `python-cyborgclient-2.4.0/cyborgclient/tests/test_cyborgclient.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/cyborgclient/tests/unit/base.py` & `python-cyborgclient-2.4.0/cyborgclient/tests/unit/base.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/cyborgclient/tests/unit/common/test_httpclient.py` & `python-cyborgclient-2.4.0/cyborgclient/tests/unit/common/test_httpclient.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/cyborgclient/tests/unit/common/test_utils.py` & `python-cyborgclient-2.4.0/cyborgclient/tests/unit/common/test_utils.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/cyborgclient/tests/unit/osc/fakes.py` & `python-cyborgclient-2.4.0/cyborgclient/tests/unit/osc/fakes.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/cyborgclient/tests/unit/osc/test_plugin.py` & `python-cyborgclient-2.4.0/cyborgclient/tests/unit/osc/test_plugin.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/cyborgclient/tests/unit/osc/v2/fakes.py` & `python-cyborgclient-2.4.0/cyborgclient/tests/unit/osc/v2/fakes.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/cyborgclient/tests/unit/osc/v2/test_accelerator_request.py` & `python-cyborgclient-2.4.0/cyborgclient/tests/unit/osc/v2/test_accelerator_request.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/cyborgclient/tests/unit/osc/v2/test_attribute.py` & `python-cyborgclient-2.4.0/cyborgclient/tests/unit/osc/v2/test_attribute.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/cyborgclient/tests/unit/osc/v2/test_deployable.py` & `python-cyborgclient-2.4.0/cyborgclient/tests/unit/osc/v2/test_deployable.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/cyborgclient/tests/unit/osc/v2/test_device.py` & `python-cyborgclient-2.4.0/cyborgclient/tests/unit/osc/v2/test_device.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/cyborgclient/tests/unit/osc/v2/test_device_profile.py` & `python-cyborgclient-2.4.0/cyborgclient/tests/unit/osc/v2/test_device_profile.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/cyborgclient/tests/unit/test_shell.py` & `python-cyborgclient-2.4.0/cyborgclient/tests/unit/test_shell.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/cyborgclient/tests/unit/utils.py` & `python-cyborgclient-2.4.0/cyborgclient/tests/unit/utils.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/cyborgclient/tests/unit/v1/shell_test_base.py` & `python-cyborgclient-2.4.0/cyborgclient/tests/unit/v1/shell_test_base.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/cyborgclient/tests/unit/v1/test_accelerators.py` & `python-cyborgclient-2.4.0/cyborgclient/tests/unit/v1/test_accelerators.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/cyborgclient/tests/unit/v1/test_accelerators_shell.py` & `python-cyborgclient-2.4.0/cyborgclient/tests/unit/v1/test_accelerators_shell.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/cyborgclient/tests/unit/v1/test_client.py` & `python-cyborgclient-2.4.0/cyborgclient/tests/unit/v1/test_client.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/cyborgclient/tests/unit/v1/test_deployables.py` & `python-cyborgclient-2.4.0/cyborgclient/tests/unit/v1/test_deployables.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/cyborgclient/v1/accelerators.py` & `python-cyborgclient-2.4.0/cyborgclient/v1/accelerators.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/cyborgclient/v1/accelerators_shell.py` & `python-cyborgclient-2.4.0/cyborgclient/v1/accelerators_shell.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/cyborgclient/v1/basemodels.py` & `python-cyborgclient-2.4.0/cyborgclient/v1/basemodels.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/cyborgclient/v1/client.py` & `python-cyborgclient-2.4.0/cyborgclient/v1/client.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/cyborgclient/v1/deployables.py` & `python-cyborgclient-2.4.0/cyborgclient/v1/deployables.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/cyborgclient/v1/shell.py` & `python-cyborgclient-2.4.0/cyborgclient/v1/shell.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/cyborgclient/version.py` & `python-cyborgclient-2.4.0/cyborgclient/version.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/doc/source/conf.py` & `python-cyborgclient-2.4.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/doc/source/contributor/contributing.rst` & `python-cyborgclient-2.4.0/doc/source/contributor/contributing.rst`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/doc/source/index.rst` & `python-cyborgclient-2.4.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/python_cyborgclient.egg-info/PKG-INFO` & `python-cyborgclient-2.4.0/python_cyborgclient.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: python-cyborgclient
-Version: 2.3.0
+Version: 2.4.0
 Summary: Python client for cyborg API
 Home-page: https://docs.openstack.org/python-cyborgclient/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
@@ -126,8 +126,10 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
```

### Comparing `python-cyborgclient-2.3.0/python_cyborgclient.egg-info/SOURCES.txt` & `python-cyborgclient-2.4.0/python_cyborgclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/python_cyborgclient.egg-info/entry_points.txt` & `python-cyborgclient-2.4.0/python_cyborgclient.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/releasenotes/source/conf.py` & `python-cyborgclient-2.4.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/requirements.txt` & `python-cyborgclient-2.4.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/setup.cfg` & `python-cyborgclient-2.4.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [files]
 packages = 
 	cyborgclient
 
 [entry_points]
 console_scripts =
```

### Comparing `python-cyborgclient-2.3.0/setup.py` & `python-cyborgclient-2.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `python-cyborgclient-2.3.0/tox.ini` & `python-cyborgclient-2.4.0/tox.ini`

 * *Files identical despite different names*

