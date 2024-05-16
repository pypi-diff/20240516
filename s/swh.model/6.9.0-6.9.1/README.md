# Comparing `tmp/swh.model-6.9.0.tar.gz` & `tmp/swh.model-6.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swh.model-6.9.0.tar", last modified: Tue Nov 14 17:47:10 2023, max compression
+gzip compressed data, was "swh.model-6.9.1.tar", last modified: Mon Nov 20 13:51:30 2023, max compression
```

## Comparing `swh.model-6.9.0.tar` & `swh.model-6.9.1.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-11-14 17:47:10.833196 swh.model-6.9.0/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      140 2023-11-14 17:47:04.000000 swh.model-6.9.0/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) jenkins    (120)      137 2023-11-14 17:47:04.000000 swh.model-6.9.0/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)      848 2023-11-14 17:47:04.000000 swh.model-6.9.0/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      112 2023-11-14 17:47:04.000000 swh.model-6.9.0/AUTHORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2023-11-14 17:47:04.000000 swh.model-6.9.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) jenkins    (120)       63 2023-11-14 17:47:04.000000 swh.model-6.9.0/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2023-11-14 17:47:04.000000 swh.model-6.9.0/LICENSE
--rw-r--r--   0 jenkins    (115) jenkins    (120)      157 2023-11-14 17:47:04.000000 swh.model-6.9.0/MANIFEST.in
--rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2023-11-14 17:47:04.000000 swh.model-6.9.0/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2023-11-14 17:47:04.000000 swh.model-6.9.0/Makefile.local
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2729 2023-11-14 17:47:10.833196 swh.model-6.9.0/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)      620 2023-11-14 17:47:04.000000 swh.model-6.9.0/README.md
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-11-14 17:47:10.809197 swh.model-6.9.0/bin/
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)      438 2023-11-14 17:47:04.000000 swh.model-6.9.0/bin/git-revhash
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)     1433 2023-11-14 17:47:04.000000 swh.model-6.9.0/bin/swh-hashtree
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)     1260 2023-11-14 17:47:04.000000 swh.model-6.9.0/bin/swh-revhash
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-11-14 17:47:10.813197 swh.model-6.9.0/docs/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2023-11-14 17:47:04.000000 swh.model-6.9.0/docs/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)       63 2023-11-14 17:47:04.000000 swh.model-6.9.0/docs/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)      199 2023-11-14 17:47:04.000000 swh.model-6.9.0/docs/Makefile.local
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-11-14 17:47:10.813197 swh.model-6.9.0/docs/_static/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2023-11-14 17:47:04.000000 swh.model-6.9.0/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-11-14 17:47:10.813197 swh.model-6.9.0/docs/_templates/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2023-11-14 17:47:04.000000 swh.model-6.9.0/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) jenkins    (120)      119 2023-11-14 17:47:04.000000 swh.model-6.9.0/docs/cli.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)       43 2023-11-14 17:47:04.000000 swh.model-6.9.0/docs/conf.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    14636 2023-11-14 17:47:04.000000 swh.model-6.9.0/docs/data-model.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1377 2023-11-14 17:47:04.000000 swh.model-6.9.0/docs/iana-swh-template.txt
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-11-14 17:47:10.813197 swh.model-6.9.0/docs/images/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       38 2023-11-14 17:47:04.000000 swh.model-6.9.0/docs/images/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2023-11-14 17:47:04.000000 swh.model-6.9.0/docs/images/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8072 2023-11-14 17:47:04.000000 swh.model-6.9.0/docs/images/swh-merkle-dag.dia
--rw-r--r--   0 jenkins    (115) jenkins    (120)      395 2023-11-14 17:47:04.000000 swh.model-6.9.0/docs/index.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)    18387 2023-11-14 17:47:04.000000 swh.model-6.9.0/docs/persistent-identifiers.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      104 2023-11-14 17:47:04.000000 swh.model-6.9.0/mypy.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)      237 2023-11-14 17:47:04.000000 swh.model-6.9.0/pyproject.toml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      276 2023-11-14 17:47:04.000000 swh.model-6.9.0/pytest.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)       30 2023-11-14 17:47:04.000000 swh.model-6.9.0/requirements-cli.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       71 2023-11-14 17:47:04.000000 swh.model-6.9.0/requirements-test.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      380 2023-11-14 17:47:04.000000 swh.model-6.9.0/requirements.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      120 2023-11-14 17:47:10.833196 swh.model-6.9.0/setup.cfg
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)     2504 2023-11-14 17:47:04.000000 swh.model-6.9.0/setup.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-11-14 17:47:10.813197 swh.model-6.9.0/swh/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       76 2023-11-14 17:47:04.000000 swh.model-6.9.0/swh/__init__.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-11-14 17:47:10.821197 swh.model-6.9.0/swh/model/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2023-11-14 17:47:04.000000 swh.model-6.9.0/swh/model/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     9357 2023-11-14 17:47:04.000000 swh.model-6.9.0/swh/model/cli.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1907 2023-11-14 17:47:04.000000 swh.model-6.9.0/swh/model/collections.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8701 2023-11-14 17:47:04.000000 swh.model-6.9.0/swh/model/discovery.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5460 2023-11-14 17:47:04.000000 swh.model-6.9.0/swh/model/exceptions.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-11-14 17:47:10.821197 swh.model-6.9.0/swh/model/fields/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      625 2023-11-14 17:47:04.000000 swh.model-6.9.0/swh/model/fields/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4153 2023-11-14 17:47:04.000000 swh.model-6.9.0/swh/model/fields/compound.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3547 2023-11-14 17:47:04.000000 swh.model-6.9.0/swh/model/fields/hashes.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2336 2023-11-14 17:47:04.000000 swh.model-6.9.0/swh/model/fields/simple.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    21670 2023-11-14 17:47:04.000000 swh.model-6.9.0/swh/model/from_disk.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    22350 2023-11-14 17:47:04.000000 swh.model-6.9.0/swh/model/git_objects.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10539 2023-11-14 17:47:04.000000 swh.model-6.9.0/swh/model/hashutil.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    16945 2023-11-14 17:47:04.000000 swh.model-6.9.0/swh/model/hypothesis_strategies.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3267 2023-11-14 17:47:04.000000 swh.model-6.9.0/swh/model/identifiers.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7112 2023-11-14 17:47:04.000000 swh.model-6.9.0/swh/model/merkle.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    68125 2023-11-14 17:47:04.000000 swh.model-6.9.0/swh/model/model.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2023-11-14 17:47:04.000000 swh.model-6.9.0/swh/model/py.typed
--rw-r--r--   0 jenkins    (115) jenkins    (120)    15405 2023-11-14 17:47:04.000000 swh.model-6.9.0/swh/model/swhids.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-11-14 17:47:10.825197 swh.model-6.9.0/swh/model/tests/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2023-11-14 17:47:04.000000 swh.model-6.9.0/swh/model/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-11-14 17:47:10.805197 swh.model-6.9.0/swh/model/tests/data/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-11-14 17:47:10.825197 swh.model-6.9.0/swh/model/tests/data/dir-folders/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      555 2023-11-14 17:47:04.000000 swh.model-6.9.0/swh/model/tests/data/dir-folders/sample-folder.tgz
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-11-14 17:47:10.825197 swh.model-6.9.0/swh/model/tests/data/repos/
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12201 2023-11-14 17:47:04.000000 swh.model-6.9.0/swh/model/tests/data/repos/sample-repo.tgz
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-11-14 17:47:10.829197 swh.model-6.9.0/swh/model/tests/fields/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2023-11-14 17:47:04.000000 swh.model-6.9.0/swh/model/tests/fields/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8690 2023-11-14 17:47:04.000000 swh.model-6.9.0/swh/model/tests/fields/test_compound.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6084 2023-11-14 17:47:04.000000 swh.model-6.9.0/swh/model/tests/fields/test_hashes.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4698 2023-11-14 17:47:04.000000 swh.model-6.9.0/swh/model/tests/fields/test_simple.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1996 2023-11-14 17:47:04.000000 swh.model-6.9.0/swh/model/tests/generate_testdata.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3233 2023-11-14 17:47:04.000000 swh.model-6.9.0/swh/model/tests/generate_testdata_from_disk.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    13391 2023-11-14 17:47:04.000000 swh.model-6.9.0/swh/model/tests/swh_model_data.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8813 2023-11-14 17:47:04.000000 swh.model-6.9.0/swh/model/tests/test_cli.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2282 2023-11-14 17:47:04.000000 swh.model-6.9.0/swh/model/tests/test_collections.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2633 2023-11-14 17:47:04.000000 swh.model-6.9.0/swh/model/tests/test_discovery.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    39005 2023-11-14 17:47:04.000000 swh.model-6.9.0/swh/model/tests/test_from_disk.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1534 2023-11-14 17:47:04.000000 swh.model-6.9.0/swh/model/tests/test_generate_testdata.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10729 2023-11-14 17:47:04.000000 swh.model-6.9.0/swh/model/tests/test_hashutil.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6717 2023-11-14 17:47:04.000000 swh.model-6.9.0/swh/model/tests/test_hypothesis_strategies.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    43208 2023-11-14 17:47:04.000000 swh.model-6.9.0/swh/model/tests/test_identifiers.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8944 2023-11-14 17:47:04.000000 swh.model-6.9.0/swh/model/tests/test_merkle.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    61315 2023-11-14 17:47:04.000000 swh.model-6.9.0/swh/model/tests/test_model.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2055 2023-11-14 17:47:04.000000 swh.model-6.9.0/swh/model/tests/test_swh_model_data.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    24447 2023-11-14 17:47:04.000000 swh.model-6.9.0/swh/model/tests/test_swhids.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2655 2023-11-14 17:47:04.000000 swh.model-6.9.0/swh/model/tests/test_toposort.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2840 2023-11-14 17:47:04.000000 swh.model-6.9.0/swh/model/tests/test_validators.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1484 2023-11-14 17:47:04.000000 swh.model-6.9.0/swh/model/toposort.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2814 2023-11-14 17:47:04.000000 swh.model-6.9.0/swh/model/validators.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-11-14 17:47:10.817197 swh.model-6.9.0/swh.model.egg-info/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2729 2023-11-14 17:47:10.000000 swh.model-6.9.0/swh.model.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2194 2023-11-14 17:47:10.000000 swh.model-6.9.0/swh.model.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2023-11-14 17:47:10.000000 swh.model-6.9.0/swh.model.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      104 2023-11-14 17:47:10.000000 swh.model-6.9.0/swh.model.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      333 2023-11-14 17:47:10.000000 swh.model-6.9.0/swh.model.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2023-11-14 17:47:10.000000 swh.model-6.9.0/swh.model.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1865 2023-11-14 17:47:04.000000 swh.model-6.9.0/tox.ini
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-11-20 13:51:30.860470 swh.model-6.9.1/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      140 2023-11-20 13:51:19.000000 swh.model-6.9.1/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      137 2023-11-20 13:51:19.000000 swh.model-6.9.1/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      848 2023-11-20 13:51:19.000000 swh.model-6.9.1/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      112 2023-11-20 13:51:19.000000 swh.model-6.9.1/AUTHORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2023-11-20 13:51:19.000000 swh.model-6.9.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       63 2023-11-20 13:51:19.000000 swh.model-6.9.1/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2023-11-20 13:51:19.000000 swh.model-6.9.1/LICENSE
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      157 2023-11-20 13:51:19.000000 swh.model-6.9.1/MANIFEST.in
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2023-11-20 13:51:19.000000 swh.model-6.9.1/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2023-11-20 13:51:19.000000 swh.model-6.9.1/Makefile.local
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2778 2023-11-20 13:51:30.860470 swh.model-6.9.1/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      672 2023-11-20 13:51:19.000000 swh.model-6.9.1/README.rst
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-11-20 13:51:30.832470 swh.model-6.9.1/bin/
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)      438 2023-11-20 13:51:19.000000 swh.model-6.9.1/bin/git-revhash
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)     1433 2023-11-20 13:51:19.000000 swh.model-6.9.1/bin/swh-hashtree
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)     1260 2023-11-20 13:51:19.000000 swh.model-6.9.1/bin/swh-revhash
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-11-20 13:51:30.836470 swh.model-6.9.1/docs/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2023-11-20 13:51:19.000000 swh.model-6.9.1/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       63 2023-11-20 13:51:19.000000 swh.model-6.9.1/docs/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      199 2023-11-20 13:51:19.000000 swh.model-6.9.1/docs/Makefile.local
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-11-20 13:51:30.836470 swh.model-6.9.1/docs/_static/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2023-11-20 13:51:19.000000 swh.model-6.9.1/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-11-20 13:51:30.836470 swh.model-6.9.1/docs/_templates/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2023-11-20 13:51:19.000000 swh.model-6.9.1/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      119 2023-11-20 13:51:19.000000 swh.model-6.9.1/docs/cli.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       43 2023-11-20 13:51:19.000000 swh.model-6.9.1/docs/conf.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    14636 2023-11-20 13:51:19.000000 swh.model-6.9.1/docs/data-model.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1377 2023-11-20 13:51:19.000000 swh.model-6.9.1/docs/iana-swh-template.txt
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-11-20 13:51:30.836470 swh.model-6.9.1/docs/images/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       38 2023-11-20 13:51:19.000000 swh.model-6.9.1/docs/images/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2023-11-20 13:51:19.000000 swh.model-6.9.1/docs/images/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8072 2023-11-20 13:51:19.000000 swh.model-6.9.1/docs/images/swh-merkle-dag.dia
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      282 2023-11-20 13:51:19.000000 swh.model-6.9.1/docs/index.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    18387 2023-11-20 13:51:19.000000 swh.model-6.9.1/docs/persistent-identifiers.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      104 2023-11-20 13:51:19.000000 swh.model-6.9.1/mypy.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      237 2023-11-20 13:51:19.000000 swh.model-6.9.1/pyproject.toml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      276 2023-11-20 13:51:19.000000 swh.model-6.9.1/pytest.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       30 2023-11-20 13:51:19.000000 swh.model-6.9.1/requirements-cli.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       71 2023-11-20 13:51:19.000000 swh.model-6.9.1/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      380 2023-11-20 13:51:19.000000 swh.model-6.9.1/requirements.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      120 2023-11-20 13:51:30.860470 swh.model-6.9.1/setup.cfg
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)     2502 2023-11-20 13:51:19.000000 swh.model-6.9.1/setup.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-11-20 13:51:30.836470 swh.model-6.9.1/swh/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       76 2023-11-20 13:51:19.000000 swh.model-6.9.1/swh/__init__.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-11-20 13:51:30.844470 swh.model-6.9.1/swh/model/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2023-11-20 13:51:19.000000 swh.model-6.9.1/swh/model/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     9357 2023-11-20 13:51:19.000000 swh.model-6.9.1/swh/model/cli.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1907 2023-11-20 13:51:19.000000 swh.model-6.9.1/swh/model/collections.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8701 2023-11-20 13:51:19.000000 swh.model-6.9.1/swh/model/discovery.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5460 2023-11-20 13:51:19.000000 swh.model-6.9.1/swh/model/exceptions.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-11-20 13:51:30.844470 swh.model-6.9.1/swh/model/fields/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      625 2023-11-20 13:51:19.000000 swh.model-6.9.1/swh/model/fields/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4153 2023-11-20 13:51:19.000000 swh.model-6.9.1/swh/model/fields/compound.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3547 2023-11-20 13:51:19.000000 swh.model-6.9.1/swh/model/fields/hashes.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2336 2023-11-20 13:51:19.000000 swh.model-6.9.1/swh/model/fields/simple.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    21670 2023-11-20 13:51:19.000000 swh.model-6.9.1/swh/model/from_disk.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    22350 2023-11-20 13:51:19.000000 swh.model-6.9.1/swh/model/git_objects.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    10539 2023-11-20 13:51:19.000000 swh.model-6.9.1/swh/model/hashutil.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    16945 2023-11-20 13:51:19.000000 swh.model-6.9.1/swh/model/hypothesis_strategies.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3267 2023-11-20 13:51:19.000000 swh.model-6.9.1/swh/model/identifiers.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7112 2023-11-20 13:51:19.000000 swh.model-6.9.1/swh/model/merkle.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    68154 2023-11-20 13:51:19.000000 swh.model-6.9.1/swh/model/model.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2023-11-20 13:51:19.000000 swh.model-6.9.1/swh/model/py.typed
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    15405 2023-11-20 13:51:19.000000 swh.model-6.9.1/swh/model/swhids.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-11-20 13:51:30.852470 swh.model-6.9.1/swh/model/tests/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2023-11-20 13:51:19.000000 swh.model-6.9.1/swh/model/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-11-20 13:51:30.824470 swh.model-6.9.1/swh/model/tests/data/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-11-20 13:51:30.852470 swh.model-6.9.1/swh/model/tests/data/dir-folders/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      555 2023-11-20 13:51:19.000000 swh.model-6.9.1/swh/model/tests/data/dir-folders/sample-folder.tgz
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-11-20 13:51:30.852470 swh.model-6.9.1/swh/model/tests/data/repos/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12201 2023-11-20 13:51:19.000000 swh.model-6.9.1/swh/model/tests/data/repos/sample-repo.tgz
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-11-20 13:51:30.856470 swh.model-6.9.1/swh/model/tests/fields/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2023-11-20 13:51:19.000000 swh.model-6.9.1/swh/model/tests/fields/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8690 2023-11-20 13:51:19.000000 swh.model-6.9.1/swh/model/tests/fields/test_compound.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6084 2023-11-20 13:51:19.000000 swh.model-6.9.1/swh/model/tests/fields/test_hashes.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4698 2023-11-20 13:51:19.000000 swh.model-6.9.1/swh/model/tests/fields/test_simple.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1996 2023-11-20 13:51:19.000000 swh.model-6.9.1/swh/model/tests/generate_testdata.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3233 2023-11-20 13:51:19.000000 swh.model-6.9.1/swh/model/tests/generate_testdata_from_disk.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    13391 2023-11-20 13:51:19.000000 swh.model-6.9.1/swh/model/tests/swh_model_data.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8813 2023-11-20 13:51:19.000000 swh.model-6.9.1/swh/model/tests/test_cli.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2282 2023-11-20 13:51:19.000000 swh.model-6.9.1/swh/model/tests/test_collections.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2633 2023-11-20 13:51:19.000000 swh.model-6.9.1/swh/model/tests/test_discovery.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    39005 2023-11-20 13:51:19.000000 swh.model-6.9.1/swh/model/tests/test_from_disk.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1534 2023-11-20 13:51:19.000000 swh.model-6.9.1/swh/model/tests/test_generate_testdata.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    10729 2023-11-20 13:51:19.000000 swh.model-6.9.1/swh/model/tests/test_hashutil.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6717 2023-11-20 13:51:19.000000 swh.model-6.9.1/swh/model/tests/test_hypothesis_strategies.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    43208 2023-11-20 13:51:19.000000 swh.model-6.9.1/swh/model/tests/test_identifiers.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8944 2023-11-20 13:51:19.000000 swh.model-6.9.1/swh/model/tests/test_merkle.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    61430 2023-11-20 13:51:19.000000 swh.model-6.9.1/swh/model/tests/test_model.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2055 2023-11-20 13:51:19.000000 swh.model-6.9.1/swh/model/tests/test_swh_model_data.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    24447 2023-11-20 13:51:19.000000 swh.model-6.9.1/swh/model/tests/test_swhids.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2655 2023-11-20 13:51:19.000000 swh.model-6.9.1/swh/model/tests/test_toposort.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2840 2023-11-20 13:51:19.000000 swh.model-6.9.1/swh/model/tests/test_validators.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1484 2023-11-20 13:51:19.000000 swh.model-6.9.1/swh/model/toposort.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2814 2023-11-20 13:51:19.000000 swh.model-6.9.1/swh/model/validators.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-11-20 13:51:30.840470 swh.model-6.9.1/swh.model.egg-info/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2778 2023-11-20 13:51:30.000000 swh.model-6.9.1/swh.model.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2195 2023-11-20 13:51:30.000000 swh.model-6.9.1/swh.model.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2023-11-20 13:51:30.000000 swh.model-6.9.1/swh.model.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      104 2023-11-20 13:51:30.000000 swh.model-6.9.1/swh.model.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      333 2023-11-20 13:51:30.000000 swh.model-6.9.1/swh.model.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2023-11-20 13:51:30.000000 swh.model-6.9.1/swh.model.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1865 2023-11-20 13:51:19.000000 swh.model-6.9.1/tox.ini
```

### Comparing `swh.model-6.9.0/.pre-commit-config.yaml` & `swh.model-6.9.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh.model-6.9.0/CODE_OF_CONDUCT.md` & `swh.model-6.9.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.model-6.9.0/LICENSE` & `swh.model-6.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.model-6.9.0/PKG-INFO` & `swh.model-6.9.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: swh.model
-Version: 6.9.0
+Version: 6.9.1
 Summary: Software Heritage data model
 Home-page: https://forge.softwareheritage.org/diffusion/DMOD/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-model
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-model/
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 Requires-Dist: attrs!=21.1.0
 Requires-Dist: attrs_strict>=0.0.7
 Requires-Dist: deprecated
 Requires-Dist: hypothesis
 Requires-Dist: iso8601
@@ -45,25 +45,26 @@
 Requires-Dist: types-click; extra == "testing"
 Requires-Dist: types-python-dateutil; extra == "testing"
 Requires-Dist: types-pytz; extra == "testing"
 Requires-Dist: swh.core>=0.3; extra == "testing"
 Requires-Dist: Click; extra == "testing"
 Requires-Dist: dulwich; extra == "testing"
 
-swh-model
-=========
+Software Heritage - Data model
+==============================
 
 Implementation of the Data model of the Software Heritage project, used to
 archive source code artifacts.
 
-This module defines the notion of SoftWare Heritage persistent IDentifiers
+This module defines the notion of SoftWare Hash persistent IDentifiers
 (SWHIDs) and provides tools to compute them:
 
-```sh
+.. code-block:: shell
+
    $ swh-identify fork.c kmod.c sched/deadline.c
    swh:1:cnt:2e391c754ae730bd2d8520c2ab497c403220c6e3    fork.c
    swh:1:cnt:0277d1216f80ae1adeed84a686ed34c9b2931fc2    kmod.c
    swh:1:cnt:57b939c81bce5d06fa587df8915f05affbe22b82    sched/deadline.c
 
    $ swh-identify --no-filename /usr/src/linux/kernel/
    swh:1:dir:f9f858a48d663b3809c9e2f336412717496202ab
-```
+
```

### Comparing `swh.model-6.9.0/README.md` & `swh.model-6.9.1/README.rst`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-swh-model
-=========
+Software Heritage - Data model
+==============================
 
 Implementation of the Data model of the Software Heritage project, used to
 archive source code artifacts.
 
-This module defines the notion of SoftWare Heritage persistent IDentifiers
+This module defines the notion of SoftWare Hash persistent IDentifiers
 (SWHIDs) and provides tools to compute them:
 
-```sh
+.. code-block:: shell
+
    $ swh-identify fork.c kmod.c sched/deadline.c
    swh:1:cnt:2e391c754ae730bd2d8520c2ab497c403220c6e3    fork.c
    swh:1:cnt:0277d1216f80ae1adeed84a686ed34c9b2931fc2    kmod.c
    swh:1:cnt:57b939c81bce5d06fa587df8915f05affbe22b82    sched/deadline.c
 
    $ swh-identify --no-filename /usr/src/linux/kernel/
    swh:1:dir:f9f858a48d663b3809c9e2f336412717496202ab
-```
+
```

### Comparing `swh.model-6.9.0/bin/swh-hashtree` & `swh.model-6.9.1/bin/swh-hashtree`

 * *Files identical despite different names*

### Comparing `swh.model-6.9.0/bin/swh-revhash` & `swh.model-6.9.1/bin/swh-revhash`

 * *Files identical despite different names*

### Comparing `swh.model-6.9.0/docs/data-model.rst` & `swh.model-6.9.1/docs/data-model.rst`

 * *Files identical despite different names*

### Comparing `swh.model-6.9.0/docs/iana-swh-template.txt` & `swh.model-6.9.1/docs/iana-swh-template.txt`

 * *Files identical despite different names*

### Comparing `swh.model-6.9.0/docs/images/swh-merkle-dag.dia` & `swh.model-6.9.1/docs/images/swh-merkle-dag.dia`

 * *Files identical despite different names*

### Comparing `swh.model-6.9.0/docs/persistent-identifiers.rst` & `swh.model-6.9.1/docs/persistent-identifiers.rst`

 * *Files identical despite different names*

### Comparing `swh.model-6.9.0/setup.py` & `swh.model-6.9.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from os import path
 
 from setuptools import find_packages, setup
 
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
-with open(path.join(here, "README.md"), encoding="utf-8") as f:
+with open(path.join(here, "README.rst"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 def parse_requirements(name=None):
     if name:
         reqf = "requirements-%s.txt" % name
     else:
@@ -35,15 +35,15 @@
     return requirements
 
 
 setup(
     name="swh.model",
     description="Software Heritage data model",
     long_description=long_description,
-    long_description_content_type="text/markdown",
+    long_description_content_type="text/x-rst",
     python_requires=">=3.7",
     author="Software Heritage developers",
     author_email="swh-devel@inria.fr",
     url="https://forge.softwareheritage.org/diffusion/DMOD/",
     packages=find_packages(),
     setup_requires=["setuptools-scm"],
     use_scm_version=True,
```

### Comparing `swh.model-6.9.0/swh/model/cli.py` & `swh.model-6.9.1/swh/model/cli.py`

 * *Files identical despite different names*

### Comparing `swh.model-6.9.0/swh/model/collections.py` & `swh.model-6.9.1/swh/model/collections.py`

 * *Files identical despite different names*

### Comparing `swh.model-6.9.0/swh/model/discovery.py` & `swh.model-6.9.1/swh/model/discovery.py`

 * *Files identical despite different names*

### Comparing `swh.model-6.9.0/swh/model/exceptions.py` & `swh.model-6.9.1/swh/model/exceptions.py`

 * *Files identical despite different names*

### Comparing `swh.model-6.9.0/swh/model/fields/__init__.py` & `swh.model-6.9.1/swh/model/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.model-6.9.0/swh/model/fields/compound.py` & `swh.model-6.9.1/swh/model/fields/compound.py`

 * *Files identical despite different names*

### Comparing `swh.model-6.9.0/swh/model/fields/hashes.py` & `swh.model-6.9.1/swh/model/fields/hashes.py`

 * *Files identical despite different names*

### Comparing `swh.model-6.9.0/swh/model/fields/simple.py` & `swh.model-6.9.1/swh/model/fields/simple.py`

 * *Files identical despite different names*

### Comparing `swh.model-6.9.0/swh/model/from_disk.py` & `swh.model-6.9.1/swh/model/from_disk.py`

 * *Files identical despite different names*

### Comparing `swh.model-6.9.0/swh/model/git_objects.py` & `swh.model-6.9.1/swh/model/git_objects.py`

 * *Files identical despite different names*

### Comparing `swh.model-6.9.0/swh/model/hashutil.py` & `swh.model-6.9.1/swh/model/hashutil.py`

 * *Files identical despite different names*

### Comparing `swh.model-6.9.0/swh/model/hypothesis_strategies.py` & `swh.model-6.9.1/swh/model/hypothesis_strategies.py`

 * *Files identical despite different names*

### Comparing `swh.model-6.9.0/swh/model/identifiers.py` & `swh.model-6.9.1/swh/model/identifiers.py`

 * *Files identical despite different names*

### Comparing `swh.model-6.9.0/swh/model/merkle.py` & `swh.model-6.9.1/swh/model/merkle.py`

 * *Files identical despite different names*

### Comparing `swh.model-6.9.0/swh/model/model.py` & `swh.model-6.9.1/swh/model/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -378,15 +378,15 @@
         attr.validate(self)  # type: ignore[arg-type]
 
 
 def _compute_hash_from_manifest(manifest: bytes) -> Sha1Git:
     return hashlib.new("sha1", manifest).digest()
 
 
-class HashableObject(metaclass=ABCMeta):
+class BaseHashableModel(BaseModel, metaclass=ABCMeta):
     """Mixin to automatically compute object identifier hash when
     the associated model is instantiated."""
 
     __slots__ = ()
 
     id: Sha1Git
 
@@ -408,22 +408,25 @@
             obj_id = self.compute_hash()
             object.__setattr__(self, "id", obj_id)
 
     def unique_key(self) -> KeyType:
         return self.id
 
     def check(self) -> None:
-        super().check()  # type: ignore
+        super().check()
 
         if self.id != self.compute_hash():
             raise ValueError("'id' does not match recomputed hash.")
 
 
-class HashableObjectWithManifest(HashableObject):
-    """Derived class of HashableObject, for objects that may need to store
+HashableObject = BaseHashableModel  # deprecated alias
+
+
+class HashableObjectWithManifest(BaseHashableModel):
+    """Derived class of BaseHashableModel, for objects that may need to store
     verbatim git objects as ``raw_manifest`` to preserve original hashes."""
 
     __slots__ = ()
 
     raw_manifest: Optional[bytes] = None
     """Stores the original content of git objects when they cannot be faithfully
     represented using only the other attributes.
@@ -763,15 +766,15 @@
         ... ).offset_minutes()
         330
         """
         return self._parse_offset_bytes(self.offset_bytes)
 
 
 @attr.s(frozen=True, slots=True, field_transformer=optimize_all_validators)
-class Origin(HashableObject, BaseModel):
+class Origin(BaseHashableModel):
     """Represents a software source: a VCS and an URL."""
 
     object_type: Final = "origin"
 
     url = attr.ib(type=str, validator=generic_type_validator)
 
     id = attr.ib(type=Sha1Git, validator=generic_type_validator, default=b"")
@@ -929,15 +932,15 @@
             return None
         return CoreSWHID(
             object_id=self.target, object_type=SwhidObjectType[self.target_type.name]
         )
 
 
 @attr.s(frozen=True, slots=True, field_transformer=optimize_all_validators)
-class Snapshot(HashableObject, BaseModel):
+class Snapshot(BaseHashableModel):
     """Represents the full state of an origin at a given point in time."""
 
     object_type: Final = "snapshot"
 
     branches = attr.ib(
         type=ImmutableDict[bytes, Optional[SnapshotBranch]],
         validator=generic_type_validator,
@@ -1647,15 +1650,15 @@
         raise ValueError("discovery_date must be a timezone-aware datetime.")
 
     # Normalize timezone to utc, and truncate microseconds to 0
     return value.astimezone(datetime.timezone.utc).replace(microsecond=0)
 
 
 @attr.s(frozen=True, slots=True, field_transformer=optimize_all_validators)
-class RawExtrinsicMetadata(HashableObject, BaseModel):
+class RawExtrinsicMetadata(BaseHashableModel):
     object_type: Final = "raw_extrinsic_metadata"
 
     # target object
     target = attr.ib(type=ExtendedSWHID, validator=generic_type_validator)
 
     # source
     discovery_date = attr.ib(type=datetime.datetime, converter=normalize_discovery_date)
@@ -1893,15 +1896,15 @@
         return ExtendedSWHID(
             object_type=SwhidExtendedObjectType.RAW_EXTRINSIC_METADATA,
             object_id=self.id,
         )
 
 
 @attr.s(frozen=True, slots=True, field_transformer=optimize_all_validators)
-class ExtID(HashableObject, BaseModel):
+class ExtID(BaseHashableModel):
     object_type: Final = "extid"
 
     extid_type = attr.ib(type=str, validator=generic_type_validator)
     extid = attr.ib(type=bytes, validator=generic_type_validator)
     target = attr.ib(type=CoreSWHID, validator=generic_type_validator)
     extid_version = attr.ib(type=int, validator=generic_type_validator, default=0)
```

### Comparing `swh.model-6.9.0/swh/model/swhids.py` & `swh.model-6.9.1/swh/model/swhids.py`

 * *Files identical despite different names*

### Comparing `swh.model-6.9.0/swh/model/tests/data/dir-folders/sample-folder.tgz` & `swh.model-6.9.1/swh/model/tests/data/dir-folders/sample-folder.tgz`

 * *Files identical despite different names*

### Comparing `swh.model-6.9.0/swh/model/tests/data/repos/sample-repo.tgz` & `swh.model-6.9.1/swh/model/tests/data/repos/sample-repo.tgz`

 * *Files identical despite different names*

### Comparing `swh.model-6.9.0/swh/model/tests/fields/test_compound.py` & `swh.model-6.9.1/swh/model/tests/fields/test_compound.py`

 * *Files identical despite different names*

### Comparing `swh.model-6.9.0/swh/model/tests/fields/test_hashes.py` & `swh.model-6.9.1/swh/model/tests/fields/test_hashes.py`

 * *Files identical despite different names*

### Comparing `swh.model-6.9.0/swh/model/tests/fields/test_simple.py` & `swh.model-6.9.1/swh/model/tests/fields/test_simple.py`

 * *Files identical despite different names*

### Comparing `swh.model-6.9.0/swh/model/tests/generate_testdata.py` & `swh.model-6.9.1/swh/model/tests/generate_testdata.py`

 * *Files identical despite different names*

### Comparing `swh.model-6.9.0/swh/model/tests/generate_testdata_from_disk.py` & `swh.model-6.9.1/swh/model/tests/generate_testdata_from_disk.py`

 * *Files identical despite different names*

### Comparing `swh.model-6.9.0/swh/model/tests/swh_model_data.py` & `swh.model-6.9.1/swh/model/tests/swh_model_data.py`

 * *Files identical despite different names*

### Comparing `swh.model-6.9.0/swh/model/tests/test_cli.py` & `swh.model-6.9.1/swh/model/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `swh.model-6.9.0/swh/model/tests/test_collections.py` & `swh.model-6.9.1/swh/model/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `swh.model-6.9.0/swh/model/tests/test_discovery.py` & `swh.model-6.9.1/swh/model/tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `swh.model-6.9.0/swh/model/tests/test_from_disk.py` & `swh.model-6.9.1/swh/model/tests/test_from_disk.py`

 * *Files identical despite different names*

### Comparing `swh.model-6.9.0/swh/model/tests/test_generate_testdata.py` & `swh.model-6.9.1/swh/model/tests/test_generate_testdata.py`

 * *Files identical despite different names*

### Comparing `swh.model-6.9.0/swh/model/tests/test_hashutil.py` & `swh.model-6.9.1/swh/model/tests/test_hashutil.py`

 * *Files identical despite different names*

### Comparing `swh.model-6.9.0/swh/model/tests/test_hypothesis_strategies.py` & `swh.model-6.9.1/swh/model/tests/test_hypothesis_strategies.py`

 * *Files identical despite different names*

### Comparing `swh.model-6.9.0/swh/model/tests/test_identifiers.py` & `swh.model-6.9.1/swh/model/tests/test_identifiers.py`

 * *Files identical despite different names*

### Comparing `swh.model-6.9.0/swh/model/tests/test_merkle.py` & `swh.model-6.9.1/swh/model/tests/test_merkle.py`

 * *Files identical despite different names*

### Comparing `swh.model-6.9.0/swh/model/tests/test_model.py` & `swh.model-6.9.1/swh/model/tests/test_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1505,17 +1505,21 @@
 @given(strategies.objects(split_content=True))
 def test_object_type(objtype_and_obj):
     obj_type, obj = objtype_and_obj
     assert obj_type == obj.object_type
 
 
 def test_object_type_is_final():
+    checked_classes = set()
     object_types = set()
 
     def check_final(cls):
+        if cls in checked_classes:
+            return
+        checked_classes.add(cls)
         if hasattr(cls, "object_type"):
             assert cls.object_type not in object_types
             object_types.add(cls.object_type)
         if cls.__subclasses__():
             assert not hasattr(cls, "object_type")
         for subcls in cls.__subclasses__():
             check_final(subcls)
```

### Comparing `swh.model-6.9.0/swh/model/tests/test_swh_model_data.py` & `swh.model-6.9.1/swh/model/tests/test_swh_model_data.py`

 * *Files identical despite different names*

### Comparing `swh.model-6.9.0/swh/model/tests/test_swhids.py` & `swh.model-6.9.1/swh/model/tests/test_swhids.py`

 * *Files identical despite different names*

### Comparing `swh.model-6.9.0/swh/model/tests/test_toposort.py` & `swh.model-6.9.1/swh/model/tests/test_toposort.py`

 * *Files identical despite different names*

### Comparing `swh.model-6.9.0/swh/model/tests/test_validators.py` & `swh.model-6.9.1/swh/model/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `swh.model-6.9.0/swh/model/toposort.py` & `swh.model-6.9.1/swh/model/toposort.py`

 * *Files identical despite different names*

### Comparing `swh.model-6.9.0/swh/model/validators.py` & `swh.model-6.9.1/swh/model/validators.py`

 * *Files identical despite different names*

### Comparing `swh.model-6.9.0/swh.model.egg-info/PKG-INFO` & `swh.model-6.9.1/swh.model.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: swh.model
-Version: 6.9.0
+Version: 6.9.1
 Summary: Software Heritage data model
 Home-page: https://forge.softwareheritage.org/diffusion/DMOD/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-model
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-model/
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 Requires-Dist: attrs!=21.1.0
 Requires-Dist: attrs_strict>=0.0.7
 Requires-Dist: deprecated
 Requires-Dist: hypothesis
 Requires-Dist: iso8601
@@ -45,25 +45,26 @@
 Requires-Dist: types-click; extra == "testing"
 Requires-Dist: types-python-dateutil; extra == "testing"
 Requires-Dist: types-pytz; extra == "testing"
 Requires-Dist: swh.core>=0.3; extra == "testing"
 Requires-Dist: Click; extra == "testing"
 Requires-Dist: dulwich; extra == "testing"
 
-swh-model
-=========
+Software Heritage - Data model
+==============================
 
 Implementation of the Data model of the Software Heritage project, used to
 archive source code artifacts.
 
-This module defines the notion of SoftWare Heritage persistent IDentifiers
+This module defines the notion of SoftWare Hash persistent IDentifiers
 (SWHIDs) and provides tools to compute them:
 
-```sh
+.. code-block:: shell
+
    $ swh-identify fork.c kmod.c sched/deadline.c
    swh:1:cnt:2e391c754ae730bd2d8520c2ab497c403220c6e3    fork.c
    swh:1:cnt:0277d1216f80ae1adeed84a686ed34c9b2931fc2    kmod.c
    swh:1:cnt:57b939c81bce5d06fa587df8915f05affbe22b82    sched/deadline.c
 
    $ swh-identify --no-filename /usr/src/linux/kernel/
    swh:1:dir:f9f858a48d663b3809c9e2f336412717496202ab
-```
+
```

### Comparing `swh.model-6.9.0/swh.model.egg-info/SOURCES.txt` & `swh.model-6.9.1/swh.model.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 AUTHORS
 CODE_OF_CONDUCT.md
 CONTRIBUTORS
 LICENSE
 MANIFEST.in
 Makefile
 Makefile.local
-README.md
+README.rst
 mypy.ini
 pyproject.toml
 pytest.ini
 requirements-cli.txt
 requirements-test.txt
 requirements.txt
 setup.cfg
```

### Comparing `swh.model-6.9.0/tox.ini` & `swh.model-6.9.1/tox.ini`

 * *Files identical despite different names*

