# Comparing `tmp/qci_client-3.2.1.tar.gz` & `tmp/qci_client-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qci_client-3.2.1.tar", last modified: Mon Apr 15 14:31:03 2024, max compression
+gzip compressed data, was "qci_client-4.0.0.tar", last modified: Tue May 14 18:19:31 2024, max compression
```

## Comparing `qci_client-3.2.1.tar` & `qci_client-4.0.0.tar`

### file list

```diff
@@ -1,29 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 14:31:03.319787 qci_client-3.2.1/
--rw-rw-rw-   0 root         (0) root         (0)      167 2024-04-15 14:27:48.000000 qci_client-3.2.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     5309 2024-04-15 14:27:48.000000 qci_client-3.2.1/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      562 2024-04-15 14:27:48.000000 qci_client-3.2.1/.mega-linter.yml
--rw-rw-rw-   0 root         (0) root         (0)    11354 2024-04-15 14:27:48.000000 qci_client-3.2.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       81 2024-04-15 14:27:48.000000 qci_client-3.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2157 2024-04-15 14:31:03.319787 qci_client-3.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1008 2024-04-15 14:27:48.000000 qci_client-3.2.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2590 2024-04-15 14:27:48.000000 qci_client-3.2.1/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 14:31:03.315787 qci_client-3.2.1/qci_client/
--rw-rw-rw-   0 root         (0) root         (0)      136 2024-04-15 14:27:48.000000 qci_client-3.2.1/qci_client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6253 2024-04-15 14:27:48.000000 qci_client-3.2.1/qci_client/base.py
--rw-rw-rw-   0 root         (0) root         (0)     5420 2024-04-15 14:27:48.000000 qci_client-3.2.1/qci_client/data_converter.py
--rw-rw-rw-   0 root         (0) root         (0)     1724 2024-04-15 14:27:48.000000 qci_client-3.2.1/qci_client/enum.py
--rw-rw-rw-   0 root         (0) root         (0)    27439 2024-04-15 14:27:48.000000 qci_client-3.2.1/qci_client/qci_client.py
--rw-rw-rw-   0 root         (0) root         (0)    13726 2024-04-15 14:27:48.000000 qci_client-3.2.1/qci_client/types.py
--rw-rw-rw-   0 root         (0) root         (0)    16845 2024-04-15 14:27:48.000000 qci_client-3.2.1/qci_client/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 14:31:03.315787 qci_client-3.2.1/qci_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2157 2024-04-15 14:31:03.000000 qci_client-3.2.1/qci_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      513 2024-04-15 14:31:03.000000 qci_client-3.2.1/qci_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 14:31:03.000000 qci_client-3.2.1/qci_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      264 2024-04-15 14:31:03.000000 qci_client-3.2.1/qci_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-04-15 14:31:03.000000 qci_client-3.2.1/qci_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-15 14:31:03.319787 qci_client-3.2.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 14:31:03.315787 qci_client-3.2.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-15 14:27:48.000000 qci_client-3.2.1/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9336 2024-04-15 14:27:48.000000 qci_client-3.2.1/tests/test_data_converter.py
--rw-rw-rw-   0 root         (0) root         (0)    32560 2024-04-15 14:27:48.000000 qci_client-3.2.1/tests/test_qci_client.py
--rw-rw-rw-   0 root         (0) root         (0)     9725 2024-04-15 14:27:48.000000 qci_client-3.2.1/tests/test_remote_jobs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 18:19:31.921609 qci_client-4.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)      167 2024-05-14 18:16:19.000000 qci_client-4.0.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     5383 2024-05-14 18:16:19.000000 qci_client-4.0.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      562 2024-05-14 18:16:19.000000 qci_client-4.0.0/.mega-linter.yml
+-rw-rw-rw-   0 root         (0) root         (0)    11354 2024-05-14 18:16:19.000000 qci_client-4.0.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      144 2024-05-14 18:16:19.000000 qci_client-4.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2341 2024-05-14 18:19:31.921609 qci_client-4.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1186 2024-05-14 18:16:19.000000 qci_client-4.0.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2316 2024-05-14 18:16:19.000000 qci_client-4.0.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 18:19:31.917610 qci_client-4.0.0/qci_client/
+-rw-rw-rw-   0 root         (0) root         (0)      317 2024-05-14 18:16:19.000000 qci_client-4.0.0/qci_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 18:19:31.917610 qci_client-4.0.0/qci_client/auth/
+-rw-rw-rw-   0 root         (0) root         (0)       85 2024-05-14 18:16:19.000000 qci_client-4.0.0/qci_client/auth/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6651 2024-05-14 18:16:19.000000 qci_client-4.0.0/qci_client/auth/client.py
+-rw-rw-rw-   0 root         (0) root         (0)      719 2024-05-14 18:16:19.000000 qci_client-4.0.0/qci_client/auth/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 18:19:31.921609 qci_client-4.0.0/qci_client/optimization/
+-rw-rw-rw-   0 root         (0) root         (0)       93 2024-05-14 18:16:19.000000 qci_client-4.0.0/qci_client/optimization/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    25878 2024-05-14 18:16:19.000000 qci_client-4.0.0/qci_client/optimization/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     3656 2024-05-14 18:16:19.000000 qci_client-4.0.0/qci_client/optimization/data_converter.py
+-rw-rw-rw-   0 root         (0) root         (0)     3886 2024-05-14 18:16:19.000000 qci_client-4.0.0/qci_client/optimization/enum.py
+-rw-rw-rw-   0 root         (0) root         (0)    11371 2024-05-14 18:16:19.000000 qci_client-4.0.0/qci_client/optimization/types.py
+-rw-rw-rw-   0 root         (0) root         (0)    11517 2024-05-14 18:16:19.000000 qci_client-4.0.0/qci_client/optimization/utilities.py
+-rw-rw-rw-   0 root         (0) root         (0)      958 2024-05-14 18:16:19.000000 qci_client-4.0.0/qci_client/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 18:19:31.921609 qci_client-4.0.0/qci_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2341 2024-05-14 18:19:31.000000 qci_client-4.0.0/qci_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      826 2024-05-14 18:19:31.000000 qci_client-4.0.0/qci_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 18:19:31.000000 qci_client-4.0.0/qci_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      270 2024-05-14 18:19:31.000000 qci_client-4.0.0/qci_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-14 18:19:31.000000 qci_client-4.0.0/qci_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-14 18:19:31.921609 qci_client-4.0.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 18:19:31.921609 qci_client-4.0.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       85 2024-05-14 18:16:19.000000 qci_client-4.0.0/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 18:19:31.921609 qci_client-4.0.0/tests/auth/
+-rw-rw-rw-   0 root         (0) root         (0)       97 2024-05-14 18:16:19.000000 qci_client-4.0.0/tests/auth/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1151 2024-05-14 18:16:19.000000 qci_client-4.0.0/tests/auth/test_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 18:19:31.921609 qci_client-4.0.0/tests/optimization/
+-rw-rw-rw-   0 root         (0) root         (0)       95 2024-05-14 18:16:19.000000 qci_client-4.0.0/tests/optimization/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    34308 2024-05-14 18:16:19.000000 qci_client-4.0.0/tests/optimization/test_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     9304 2024-05-14 18:16:19.000000 qci_client-4.0.0/tests/optimization/test_data_converter.py
+-rw-rw-rw-   0 root         (0) root         (0)     8359 2024-05-14 18:16:19.000000 qci_client-4.0.0/tests/optimization/test_enum.py
+-rw-rw-rw-   0 root         (0) root         (0)     1578 2024-05-14 18:16:19.000000 qci_client-4.0.0/tests/test_utilities.py
```

### Comparing `qci_client-3.2.1/.gitlab-ci.yml` & `qci_client-4.0.0/.gitlab-ci.yml`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     - pyenv global ${PYTHON_VERSION}
     - python --version
     # Install and activate venv.
     - python -m venv ../venv
     - . ../venv/bin/activate
     # Install/upgrade build tools.
     - export SETUPTOOLS_SCM_DEBUG=1
-    - python -m pip install --upgrade --progress-bar off pip setuptools wheel
+    - python -m pip install --upgrade --progress-bar off pip setuptools
     - python -m pip --version
     # Install package.
     - python -m pip install --progress-bar off .[dev]
     - python -m pip list
     - python -m build
     - python -m check_manifest
 
@@ -74,16 +74,16 @@
     - echo Creating documentation artifact that expires in 1 week.
     - apt-get install -y --no-install-recommends zip
     - cd docs
     - mkdir dist
     - mkdir dist/html
     - mkdir dist/xml
     - make clean
-    - sphinx-build -b html source build/html
-    - sphinx-build -b xml source build/xml
+    - sphinx-build -W -b html source build/html
+    - sphinx-build -W -b xml source build/xml
     - cd build/html
     - zip -r ../../dist/html/${CI_PROJECT_NAME}-docs-${CI_COMMIT_BRANCH}-${CI_COMMIT_SHORT_SHA}.zip *
     - cd ../xml
     - zip -r ../../dist/xml/${CI_PROJECT_NAME}-docs-${CI_COMMIT_BRANCH}-${CI_COMMIT_SHORT_SHA}.zip *.xml
   artifacts:
     name: ${CI_PROJECT_NAME}-docs-${CI_COMMIT_BRANCH}-${CI_COMMIT_SHORT_SHA}
     when: always
@@ -100,16 +100,16 @@
     - echo Creating documentation artifact that expires never.
     - apt-get install -y --no-install-recommends zip
     - cd docs
     - mkdir dist
     - mkdir dist/html
     - mkdir dist/xml
     - make clean
-    - sphinx-build -b html source build/html
-    - sphinx-build -b xml source build/xml
+    - sphinx-build -W -b html source build/html
+    - sphinx-build -W -b xml source build/xml
     - cd build/html
     - zip -r ../../dist/html/${CI_PROJECT_NAME}-docs-${CI_COMMIT_TAG}.zip *
     - cd ../xml
     - zip -r ../../dist/xml/${CI_PROJECT_NAME}-docs-${CI_COMMIT_TAG}.zip *.xml
   artifacts:
     name: ${CI_PROJECT_NAME}-docs-${CI_COMMIT_TAG}
     when: always
@@ -150,20 +150,22 @@
       - megalinter-reports
     expire_in: 1 week
 
 tests:
   stage: test
   <<: *build_module
   script:
-    # Do not run full set of tests yet due to remote setup issues (100% NOT yet required in pyproject.toml).
-    - python -m coverage run --source=qci_client -m pytest -v -m "offline and not timing"
+    # Do not run timiing tests which are fragile in CI environment.
+    # Tests require QCI_TOKEN and QCI_API_URL be set in environment.
+    - python -m coverage run --source=qci_client -m pytest -v -m "not timing"
+    # 100% coverage NOT yet required in pyproject.toml.
     - python -m coverage report -m
     # Python linters/autoformatters.
-    # - python -m pylint .
-    # - python -m black --check .
+    - python -m pylint .
+    - python -m black --check .
   parallel:
     matrix:
       - PYTHON_VERSION: ['3.8.18', '3.9.18', '3.10.13', '3.11.8', '3.12.2']
 
 publish-package-dev:
   stage: publish
   rules:
```

### Comparing `qci_client-3.2.1/.mega-linter.yml` & `qci_client-4.0.0/.mega-linter.yml`

 * *Files identical despite different names*

### Comparing `qci_client-3.2.1/LICENSE` & `qci_client-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qci_client-3.2.1/PKG-INFO` & `qci_client-4.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qci-client
-Version: 3.2.1
+Version: 4.0.0
 Summary: Client Package for using Qatalyst Optimization Suite
 Author: Quantum Computing Inc.
 Author-email: support@quantumcomputinginc.com
 License: Apache 2.0
 Project-URL: documentation, https://quantumcomputinginc.com/learn/reference-documentation
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
@@ -14,19 +14,19 @@
 License-File: LICENSE
 Requires-Dist: requests<3,>=2.22.1
 Requires-Dist: requests-futures<2,>=1.0.0
 Requires-Dist: networkx<3,>=2.6.3
 Requires-Dist: numpy<2,>=1.21.1
 Requires-Dist: scipy<2,>=1.7.3
 Provides-Extra: dev
-Requires-Dist: black==23.1.0; extra == "dev"
+Requires-Dist: black<25,>=24.3.0; extra == "dev"
 Requires-Dist: build<0.11,>=0.10.0; extra == "dev"
 Requires-Dist: check-manifest<0.49,>=0.48; extra == "dev"
 Requires-Dist: coverage[toml]<7,>=6.4.2; extra == "dev"
-Requires-Dist: pylint==2.16.2; extra == "dev"
+Requires-Dist: pylint<4,>=3.1.0; extra == "dev"
 Requires-Dist: pytest<8,>=7.2.1; extra == "dev"
 Requires-Dist: sphinx-rtd-theme>=1.3.0; extra == "dev"
 Requires-Dist: twine<4,>=3.7.1; extra == "dev"
 
 # QCI Client
 
 ## Getting started
@@ -39,35 +39,37 @@
 Install `qci-client` from the [public PyPI server](https://pypi.org/)
 into your Python virtual environment using--
 
 ```bash
 pip install qci-client
 ```
 
-### Instantiating a Client
+### Instantiating a Client for Optimization
 
 #### With Environment Variables
 
 To access the API, set these environment variables--
 
 <!-- markdown-link-check-disable-next-line -->
 - QCI_API_URL - URL for Qatalyst API, Example: "https://api.qci-prod.com"
 - QCI_TOKEN - refresh token string for securely accessing Qatalyst API
 
 then instantiate a `QciClient` as follows--
 
 ```python
+# An alias for `from qci_client.optimization.client import Client as QciClient`.
 from qci_client import QciClient
 
 client = QciClient()
 ```
 
 #### Without Environment Variables
 
 Access the API without first defining environment variables by instantiating a
 `QciClient` as follows--
 
 ```python
+# A alias for `from qci_client.optimization.client import Client as QciClient`.
 from qci_client import QciClient
 
 client = QciClient(url="https://api.qci-prod.com", api_token="<secret-token>")
 ```
```

### Comparing `qci_client-3.2.1/README.md` & `qci_client-4.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -10,35 +10,37 @@
 Install `qci-client` from the [public PyPI server](https://pypi.org/)
 into your Python virtual environment using--
 
 ```bash
 pip install qci-client
 ```
 
-### Instantiating a Client
+### Instantiating a Client for Optimization
 
 #### With Environment Variables
 
 To access the API, set these environment variables--
 
 <!-- markdown-link-check-disable-next-line -->
 - QCI_API_URL - URL for Qatalyst API, Example: "https://api.qci-prod.com"
 - QCI_TOKEN - refresh token string for securely accessing Qatalyst API
 
 then instantiate a `QciClient` as follows--
 
 ```python
+# An alias for `from qci_client.optimization.client import Client as QciClient`.
 from qci_client import QciClient
 
 client = QciClient()
 ```
 
 #### Without Environment Variables
 
 Access the API without first defining environment variables by instantiating a
 `QciClient` as follows--
 
 ```python
+# A alias for `from qci_client.optimization.client import Client as QciClient`.
 from qci_client import QciClient
 
 client = QciClient(url="https://api.qci-prod.com", api_token="<secret-token>")
 ```
```

### Comparing `qci_client-3.2.1/pyproject.toml` & `qci_client-4.0.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -30,37 +30,34 @@
 
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 
+# Be sure to also update the dependencies list in the documentation.
 dependencies = [
     "requests >=2.22.1, <3",
     "requests-futures >=1.0.0, <2",
     "networkx >=2.6.3, <3",
     "numpy >=1.21.1, <2",
     "scipy >=1.7.3, <2",
 ]
 
 dynamic = [
     "version"
 ]
 
 [project.optional-dependencies]
 dev = [
-    # Try to match black version in megalinter that runs in CI:
-    # https://github.com/oxsecurity/megalinter/blob/main/docs/descriptors/python_black.md#black-documentation
-    "black ==23.1.0",
+    "black >=24.3.0, <25",
     "build >=0.10.0, <0.11",
     "check-manifest >=0.48, <0.49",
     "coverage[toml] >=6.4.2, <7",
-    # Try to match pylint version in megalinter that runs in CI:
-    # https://github.com/oxsecurity/megalinter/blob/main/docs/descriptors/python_pylint.md#pylint-documentation
-    "pylint ==2.16.2",
+    "pylint >=3.1.0, <4",
     "pytest >=7.2.1, <8",
     "sphinx-rtd-theme >=1.3.0",
     "twine >=3.7.1, <4"
 ]
 
 [project.urls]
     documentation = "https://quantumcomputinginc.com/learn/reference-documentation"
```

### Comparing `qci_client-3.2.1/qci_client/base.py` & `qci_client-4.0.0/qci_client/auth/client.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,177 +1,200 @@
-"""Base class for API clients."""
+# Copyright 2023-2024, Quantum Computing Incorporated
+"""Client for QCi's auth API."""
 
-from dataclasses import dataclass, field
+from copy import deepcopy
 from datetime import datetime
-import functools
 import os
-from posixpath import join
-from typing import Callable, Optional
+from typing import Optional
 
 import requests
-from requests.adapters import HTTPAdapter, Retry
+from requests.compat import urljoin
 
-# We are uploading files we want to retry when we receive certain error codes
-RETRY_TOTAL = 7
-BACKOFF_FACTOR = 2
-STATUS_FORCELIST = [502, 503, 504]
-
-
-@dataclass
-class BaseApi:  # pylint: disable=too-many-instance-attributes
-    """
-    Base class for clients to QCi APIs, especially the authorization layer.
-
-    :param url: url basepath to API endpoint, including scheme, if None, then falls back
-        to QCI_API_URL environment variable
-    :param api_token: refresh token for authenticating to API, if None, then falls back
-        to QCI_TOKEN environment variable
-    :param access_tokens: url path fragment to specify access-tokens API endpoint
-    :param set_bearer_token_on_init: flag to turn on/off access token retrieval on
-        object initialization
-    :param timeout: number of seconds before timing out requests, None waits indefinitely
-    :param debug: flag to turn on/off debug prints
-    """
-
-    url: Optional[str] = None
-    # Hide sensistive info to prevent accidental logging when printing client objects.
-    api_token: Optional[str] = field(default=None, repr=False)
-    access_tokens: str = "auth/v1/access-tokens"
-    set_bearer_token_on_init: bool = True
-    # Request timeout in seconds for connection & read. None for infinite timeout.
-    timeout: Optional[float] = None
-    debug: bool = False
+from qci_client.auth import types
+from qci_client.utilities import raise_for_status
 
-    def __post_init__(self):
-        self.url = self.url if self.url else os.getenv("QCI_API_URL")
+TOKEN_EXPIRATION_MARGIN: float = 10 * 60.0  # seconds.
 
-        if self.url is None:
-            raise AssertionError(
-                "QCI_API_URL environment variable is empty. Specify url or add the "
-                "necessary environment variable"
+
+class AuthClient:
+    """Used to authenticate to QCi applications."""
+
+    def __init__(
+        self,
+        *,
+        url: Optional[str] = None,
+        api_token: Optional[str] = None,
+        timeout: Optional[float] = None,
+    ):
+        """
+        Handles authentication against QCi cloud APIs.
+
+        :param url: url basepath to API endpoint, including scheme, if None, then falls
+            back to QCI_API_URL environment variable
+        :param api_token: refresh token for authenticating to API, if None, then falls
+            back to QCI_TOKEN environment variable
+        :param timeout: number of seconds before timing out requests, None waits
+            indefinitely
+        """
+        if not url:
+            self._url = os.getenv("QCI_API_URL", "")
+        else:
+            self._url = url
+
+        if not self._url:
+            raise ValueError(
+                "must specify url argument or QCI_API_URL environment variable"
             )
 
-        # removing trailling / so can add paths simply
-        self.url.rstrip("/")
+        if self._url[-1] != "/":
+            self._url = self._url + "/"
 
-        self.api_token = self.api_token if self.api_token else os.getenv("QCI_TOKEN")
+        if not api_token:
+            self._refresh_token = os.getenv("QCI_TOKEN", "")
+        else:
+            self._refresh_token = api_token
 
-        if self.api_token is None:
+        if not self._refresh_token:
             raise AssertionError(
-                "QCI_TOKEN environment variable is empty. Specify api_token or add the "
-                "necessary environment variable"
+                "must specify api_token argument or QCI_TOKEN environment variable"
             )
 
-        self.session = requests.Session()
-        retries = Retry(
-            total=RETRY_TOTAL,
-            backoff_factor=BACKOFF_FACTOR,
-            status_forcelist=STATUS_FORCELIST,
-        )
-        self.session.mount("https://", HTTPAdapter(max_retries=retries))
+        self._timeout = timeout
+        self._access_token_info: Optional[types.AccessTokensPostResponseBody] = None
+
+    @property
+    def url(self) -> str:
+        """Return API URL."""
+        return self._url
+
+    @property
+    def api_token(self) -> str:
+        """Return API token."""
+        return self._refresh_token
+
+    @property
+    def timeout(self) -> Optional[float]:
+        """Return timeout setting."""
+        return self._timeout
+
+    @property
+    def access_tokens_url(self) -> str:
+        """URL used for obtaining access tokens."""
+        return self.url + "auth/v1/access-tokens/"
+
+    @property
+    def access_token_info(self) -> types.AccessTokensPostResponseBody:
+        """Return user's access token info, retrieving anew when absent or expired."""
+        if self._access_token_info:
+            # Authenticating with an expired token simply returns a 401: Status
+            # Unauthorized, so proactively check here for expiration impending or
+            # already happened. Expiration times look like "2023-07-15T08:16:59Z".
+            expiration = datetime.strptime(
+                self._access_token_info["expires_at_rfc3339"], "%Y-%m-%dT%H:%M:%SZ"
+            )
+            seconds_to_expiration = (expiration - datetime.utcnow()).total_seconds()
+
+            # Renew access token if it has expired or expiration is impending.
+            if seconds_to_expiration < TOKEN_EXPIRATION_MARGIN:
+                self._access_token_info = None
 
-        self._bearer_info = {}
+        if not self._access_token_info:
+            # Retrieve new access token info.
+            self._access_token_info = self.post_access_tokens()
 
-        if self.set_bearer_token_on_init:
-            self.set_bearer_token()
+        return deepcopy(self._access_token_info)
 
     @property
-    def auth_url(self) -> str:
-        """Return the URL used for authorization."""
-        return join(self.url, self.access_tokens)
+    def access_token(self) -> str:
+        """Return user's access token, refreshing if expired or near expiration."""
+        return self.access_token_info["access_token"]
 
     @property
-    def headers_without_token(self):
-        """Headers without cached bearer token."""
+    def expires_at_rfc3339(self) -> str:
+        """Return expiration of user's access token."""
+        return self.access_token_info["expires_at_rfc3339"]
+
+    @property
+    def token_type(self) -> str:
+        """Return type of user's access token."""
+        return self.access_token_info["token_type"]
+
+    @property
+    def organization_id(self) -> str:
+        """Return user's organization ID."""
+        return self.access_token_info["organization_id"]
+
+    @property
+    def user_id(self) -> str:
+        """Return user's user ID."""
+        return self.access_token_info["user_id"]
+
+    @property
+    def headers_without_authorization(self) -> dict:
+        """
+        HTTP headers without bearer token in Authorization header, but with
+        Content-Type, Connection, and optional X-Request-Timeout-Nano headers.
+        """
         headers = {
             "Content-Type": "application/json",
+            # Simple, sessionless requests, so close connection proactively.
             "Connection": "close",
         }
 
         if self.timeout is not None:
-            # Provide client's request timeout to server (latency provides some buffer).
-            headers.update({"X-Request-Timeout-Nano": str(int(10**9 * self.timeout))})
+            # Tell server when client will stop waiting for response.
+            headers["X-Request-Timeout-Nano"] = str(int(10**9 * self.timeout))
 
         return headers
 
     @property
-    def headers(self):
-        """Headers with cached bearer token."""
-        headers = self.headers_without_token
-        headers["Authorization"] = f"Bearer {self._bearer_info.get('access_token', '')}"
+    def headers(self) -> dict:
+        """HTTP headers with bearer token in Authorization header."""
+        headers = self.headers_without_authorization
+        headers["Authorization"] = f"Bearer {self.access_token}"
 
         return headers
 
     @property
     def headers_without_connection_close(self):
         """Headers with cached bearer token, but without connection closing."""
         headers = self.headers
         headers.pop("Connection", None)
 
         return headers
 
-    @classmethod
-    def _check_response_error(cls, response: requests.Response) -> None:
-        """
-        Single place to update error check and message for API calls
-        :param response: a response from any API call using the requests package
-        """
-        try:
-            # The requests package does special handling here, so build off of this.
-            response.raise_for_status()
-        except requests.HTTPError as err:
-            # Include response body in exception message to aid user understanding.
-            raise requests.HTTPError(
-                str(err) + f" with response body: {response.text}"
-            ) from err
-
-    def get_bearer_token(self) -> requests.Response:
-        """Request new bearer token. (Not cached here, see set_bearer_token.)"""
-        payload = {"refresh_token": self.api_token}
-
-        response = self.session.request(
-            "POST",
-            self.auth_url,
-            json=payload,
-            headers=self.headers_without_token,
+    def get_access_tokens_health(self) -> types.AccessTokensHealthGetResponseBody:
+        """GET health."""
+        response = requests.get(
+            urljoin(self.access_tokens_url, "health"),
+            headers=self.headers_without_authorization,
             timeout=self.timeout,
         )
+        raise_for_status(response=response)
 
-        self._check_response_error(response)
-
-        return response
+        return response.json()
 
-    def set_bearer_token(self) -> None:
-        """Set bearer token from request."""
-        resp = self.get_bearer_token()
-        self._bearer_info = resp.json()
-
-    def is_bearer_token_expired(self) -> bool:
-        """Is current time > 'expires' time."""
-        if "expires_at_rfc3339" not in self._bearer_info:
-            return True
-
-        expiration = datetime.strptime(
-            self._bearer_info["expires_at_rfc3339"], "%Y-%m-%dT%H:%M:%SZ"
+    def get_access_tokens_version(self) -> types.AccessTokensVersionGetResponseBody:
+        """GET version."""
+        response = requests.get(
+            urljoin(self.access_tokens_url, "version"),
+            headers=self.headers_without_authorization,
+            timeout=self.timeout,
         )
-        seconds_to_expiration = (expiration - datetime.utcnow()).total_seconds()
+        raise_for_status(response=response)
 
-        # adding 10 second buffer for expiration
-        return seconds_to_expiration < 10
+        return response.json()
 
-    @staticmethod
-    def refresh_token(func) -> Callable:
-        """Return a wrapper function that can check an auth token."""
-
-        @functools.wraps(func)
-        def check_token(api, *args, **kwargs):
-            # Because the decorated function is receiving 'self', we need to pass this
-            # additional argument along in the 'api' arg.
-            is_expired = api.is_bearer_token_expired()
-            # expired, reset the token
-            if is_expired:
-                api.set_bearer_token()
-                return func(api, *args, **kwargs)
-            # still have time on the token, so just pass the wrapped func through
-            return func(api, *args, **kwargs)
+    def post_access_tokens(self) -> types.AccessTokensPostResponseBody:
+        """
+        Authorize user via refresh token used to retrieve finite-lived access_token.
+        """
+        json: types.AccessTokensPostRequestBody = {"refresh_token": self._refresh_token}
+        response = requests.post(
+            self.access_tokens_url,
+            headers=self.headers_without_authorization,
+            json=json,
+            timeout=self.timeout,
+        )
+        raise_for_status(response=response)
 
-        return check_token
+        return response.json()
```

### Comparing `qci_client-3.2.1/qci_client/data_converter.py` & `qci_client-4.0.0/qci_client/optimization/data_converter.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,121 +1,65 @@
+# Copyright 2023-2024, Quantum Computing Incorporated
 """Functions for data conversion."""
 
-from math import floor
-import sys
+import logging
 import time
-from typing import Union
 
 import networkx as nx
 import numpy as np
 import scipy.sparse as sp
 
-from qci_client import enum
+from qci_client.optimization import utilities
+from qci_client.optimization import enum
 
 # We want to limit the memory size of each uploaded chunk to be safely below the max of 15 * MebiByte (~15MB).
 # See https://git.qci-dev.com/qci-dev/qphoton-files-api/-/blob/main/service/files.go#L32.
 MEMORY_MAX: int = 8 * 1000000  # 8MB
 
 
-def get_size(obj, seen=None) -> int:
-    """
-    Recursively finds size of objects
-
-    :param obj: data object to recursively compute size of
-    :param seen: takes a set and is used in the recursive step only to record whether an object has been counted yet.
-
-    :return int:
-    """
-    size = sys.getsizeof(obj)
-    if seen is None:
-        seen = set()
-    obj_id = id(obj)
-    if obj_id in seen:
-        return 0
-    # Important mark as seen *before* entering recursion to gracefully handle
-    # self-referential objects
-    seen.add(obj_id)
-    if isinstance(obj, dict):
-        size += sum(get_size(v, seen) for v in obj.values())
-        size += sum(get_size(k, seen) for k in obj.keys())
-    elif hasattr(obj, "__dict__"):
-        size += get_size(obj.__dict__, seen)
-    elif hasattr(obj, "__iter__") and not isinstance(obj, (str, bytes, bytearray)):
-        size += sum(get_size(i, seen) for i in obj)
-    return size
-
-
-def _get_soln_size(soln):
-    # Check whether first entry is a graph node/class assignment, eg., {'id': 4, 'class': 2}
-    if isinstance(soln[0], dict):
-        return get_size(soln)
-
-    return sys.getsizeof(soln[0]) * len(soln)
-
-
-def compute_results_step_len(data: Union[np.ndarray, list]) -> int:
-    """
-    Compute the step length for "chunking" the providd data.
-
-    Args:
-        data: An numpy array or list of data
-
-    Returns:
-        The step length for "chunking" the data
-    """
-    # total mem size of soln vector
-    soln_mem = _get_soln_size(data)
-    # num_vars * step_len < 30k => step_len < 30k/num_vars
-    chunk_ratio = MEMORY_MAX / soln_mem
-    step_len = floor(chunk_ratio) if chunk_ratio >= 1 else 1
-    return step_len
-
-def data_to_json(file: dict, debug: bool = False) -> dict:
+def data_to_json(*, file: dict) -> dict:  # pylint: disable=too-many-branches
     """
     Converts data in file input into JSON-serializable dictionary that can be passed to Qatalyst REST API
 
     Args:
         file: file dictionary whose data of type numpy.ndarray, scipy.sparse.spmatrix, or networkx.Graph is to be converted
-        debug: Optional, if set to True, enables debug output (default = False for no debug output)
 
     Returns:
         file dictionary with JSON-serializable data
     """
     start_time_s = time.perf_counter()
 
-    supported_file_types = [type.value for type in enum.JOB_INPUTS_FILE_TYPES]
-    supported_file_types.sort()
-    supported_file_types = tuple(supported_file_types)
-    matrix_file_types = [type.value for type in enum.JOB_INPUTS_MATRIX_FILE_TYPES]
-    matrix_file_types.sort()
-    matrix_file_types = tuple(matrix_file_types)
-
-    file_type = enum.get_file_type(file=file).value
+    file_config, file_type = utilities.get_file_config(file=file)
 
-    if file_type not in supported_file_types:
+    if file_type not in enum.FILE_TYPES_JOB_INPUTS:
+        input_file_types = [
+            input_file_type.value for input_file_type in enum.FILE_TYPES_JOB_INPUTS
+        ]
+        input_file_types.sort()
         raise AssertionError(
-            f"data conversion not supported for file type '{file_type}', supported "
-            f"types are {supported_file_types}"
+            f"unsupported file type, must be one of {input_file_types}"
         )
 
-    data = file['file_config'][file_type]['data']
+    data = file["file_config"][file_type.value]["data"]
 
-    if file_type == "graph":
+    if file_type == enum.FileType.GRAPH:
         if not isinstance(data, nx.Graph):
-            raise AssertionError("file_type 'graph' data must be a networkx.Graph")
+            raise AssertionError(
+                f"file type '{file_type.value}' data must be type networkx.Graph"
+            )
 
         file_config = {
             **nx.node_link_data(data),
             "num_edges": data.number_of_edges(),
             "num_nodes": data.number_of_nodes(),
         }
-    elif file_type in matrix_file_types:
+    elif file_type in enum.FILE_TYPES_JOB_INPUTS_MATRIX:
         if isinstance(data, nx.Graph):
             raise AssertionError(
-                f"file_type '{file_type}' data cannot be a networkx.Graph"
+                f"file type '{file_type.value}' does not support networkx.Graph data"
             )
 
         data_ls = []
 
         if sp.isspmatrix_dok(data):
             for idx, val in zip(data.keys(), data.values()):
                 # dok type has trouble subsequently serializing to json without type
@@ -126,31 +70,32 @@
 
             for i, j, val in zip(
                 data.row.tolist(), data.col.tolist(), data.data.tolist()
             ):
                 data_ls.append({"i": i, "j": j, "val": val})
         else:
             raise ValueError(
-                f"file_type '{file_type}' only supports types numpy.ndarray and "
-                f"scipy.sparse.spmatrix, got {type(data)}"
+                f"file type '{file_type.value}' only supports numpy.ndarray and "
+                f"scipy.sparse.spmatrix data types, got '{type(data)}'"
             )
 
         file_config = {"data": data_ls}
         rows, cols = data.get_shape()
 
-        if file_type == "constraints":
+        if file_type == enum.FileType.CONSTRAINTS:
             # Constraints matrix is [A | -b]
-            file_config.update({"num_constraints": rows, "num_variables": cols-1})
+            file_config.update({"num_constraints": rows, "num_variables": cols - 1})
         else:
             # This works for hamiltonians, qubos, and objectives.
             file_config["num_variables"] = rows
     else:
         # Polynomial file types do not require translation.
-        file_config = file["file_config"][file_type]
+        file_config = file["file_config"][file_type.value]
 
-    if debug:
-        print(f"Time to convert data to json: {time.perf_counter()-start_time_s} s.")
+    logging.debug(
+        "Time to convert data to json: %s s.", time.perf_counter() - start_time_s
+    )
 
     return {
-        "file_name": file.get("file_name", f"{file_type}.json"),
-        "file_config": {file_type: file_config}
+        "file_name": file.get("file_name", f"{file_type.value}.json"),
+        "file_config": {file_type.value: file_config},
     }
```

### Comparing `qci_client-3.2.1/qci_client/qci_client.py` & `qci_client-4.0.0/qci_client/optimization/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,123 +1,140 @@
-"""
-QciClient
-Utility class for user interactions with QCI API
-"""
+# Copyright 2023-2024, Quantum Computing Incorporated
+"""Client for QCi's optimization API."""
 
 import concurrent.futures
-from dataclasses import dataclass
-from datetime import datetime
-import gzip
-from io import BytesIO
-import json
-from posixpath import join
 import time
-from typing import ClassVar, Optional
+from typing import Optional, Union
+import warnings
 
+import requests
 from requests.adapters import HTTPAdapter, Retry
+from requests.compat import urljoin
 from requests_futures.sessions import FuturesSession
 
-from qci_client import utilities
-from qci_client.base import BaseApi, BACKOFF_FACTOR, RETRY_TOTAL, STATUS_FORCELIST
-from qci_client.data_converter import data_to_json
-
-TIMEOUT_DEFAULT: Optional[float] = 2 * 60.0  # seconds, or None for infinite.
-COMPRESS_DEFAULT = False
-MAX_WORKERS = 8
-
-class JobStatus:  # pylint: disable=too-few-public-methods
-    """Allowed jobs statuses."""
-
-    QUEUED = "QUEUED"
-    SUBMITTED = "SUBMITTED"
-    RUNNING = "RUNNING"
-    COMPLETED = "COMPLETED"
-    ERRORED = "ERRORED"
-    CANCELLED = "CANCELLED"
-
-FINAL_STATUSES = frozenset([JobStatus.COMPLETED, JobStatus.ERRORED, JobStatus.CANCELLED])
-
-@dataclass
-class QciClient(BaseApi):  # pylint: disable=too-many-public-methods
-    """
-    Provides requests for QCi's public API for running optimization problems on Dirac
-    devices, including file uploads/downloads and submitting/retrieving entire jobs.
-
-    Accepts same parameters as :class:`qci_client.base.BaseApi` as well as:
-
-    :param files: url path fragment to specify files API endpoint
-    :param jobs: url path fragment to specify jobs API endpoint
-    :param max_workers: number of threads for concurrent file download calls
-    :param compress: compress file metadata and parts before uploading
-    """
-    files: str = "optimization/v1/files"
-    jobs: str = "optimization/v1/jobs"
-    max_workers: int = 8
-    compress: bool = COMPRESS_DEFAULT
-
-    _supported_job_types: ClassVar[frozenset] = frozenset(
-        [
-            "sample-qubo",
-            "graph-partitioning",
-            "sample-constraint",
-            "sample-hamiltonian",
-            "sample-hamiltonian-ising",
-        ]
-    )
+from qci_client.utilities import log_to_console
+import qci_client.auth.client
+from qci_client.optimization import utilities
+from qci_client.optimization.data_converter import data_to_json
+from qci_client.optimization import enum
+from qci_client.utilities import raise_for_status
+
+RESULTS_CHECK_INTERVAL_S = 2.5
+# We are uploading files we want to retry when we receive certain error codes.
+RETRY_TOTAL = 7
+BACKOFF_FACTOR = 2
+STATUS_FORCELIST = [502, 503, 504]
+
+
+class OptimizationClient:  # pylint: disable=too-many-public-methods
+    """Used to run optimization jobs against QCi hardware."""
+
+    def __init__(  # pylint: disable=too-many-arguments
+        self,
+        *,
+        url: Optional[str] = None,
+        api_token: Optional[str] = None,
+        timeout: Optional[float] = None,
+        max_workers: int = 8,
+        compress: bool = False,
+    ):
+        """
+        Provides access to QCi's public API for running optimization problems on Dirac
+        devices, including file uploads/downloads and submitting/retrieving entire jobs.
+
+        :param url: url basepath to API endpoint, including scheme, if None, then falls
+            back to QCI_API_URL environment variable
+        :param api_token: refresh token for authenticating to API, if None, then falls
+            back to QCI_TOKEN environment variable
+        :param timeout: number of seconds before timing out requests, None waits
+            indefinitely
+        :param max_workers: number of threads for concurrent file download calls
+        :param compress: compress file metadata and parts before uploading
+        """
+        # The optimization client defers to auth client for url, api_token, and timeout.
+        self._auth_client = qci_client.auth.client.AuthClient(
+            url=url, api_token=api_token, timeout=timeout
+        )
+
+        self._max_workers = max_workers
+        self._compress = compress
+
+        # Session usage can improve performance. Used in non-concurrent situations.
+        self._session = requests.Session()
+        self._session.mount(
+            "https://",
+            HTTPAdapter(
+                max_retries=Retry(
+                    total=RETRY_TOTAL,
+                    backoff_factor=BACKOFF_FACTOR,
+                    status_forcelist=STATUS_FORCELIST,
+                )
+            ),
+        )
+
+    @property
+    def url(self) -> str:
+        """Return API URL."""
+        return self._auth_client.url
+
+    @property
+    def api_token(self) -> str:
+        """Return API token."""
+        return self._auth_client.api_token
+
+    @property
+    def timeout(self) -> Optional[float]:
+        """Return timeout setting."""
+        return self._auth_client.timeout
+
+    @property
+    def max_workers(self) -> int:
+        """Return maximum number of concurrent workers for file operations."""
+        return self._max_workers
+
+    @property
+    def compress(self) -> bool:
+        """Return file compression usage flag."""
+        return self._compress
 
     @property
     def jobs_url(self):
         """Get jobs URL."""
-        return join(self.url, self.jobs)
+        return urljoin(self.url, "optimization/v1/jobs")
 
-    def get_job_id_url(self, job_id: str) -> str:
+    def get_job_id_url(self, *, job_id: str) -> str:
         """Get job URL with job ID."""
-        return join(self.jobs_url, job_id)
+        return f"{self.jobs_url}/{job_id}"
 
-    def get_job_status_url(self, job_id: str) -> str:
-        """Get job status using job ID."""
-        return join(self.get_job_id_url(job_id), "status")
+    def get_job_status_url(self, *, job_id: str) -> str:
+        """Get job-status URL using job ID."""
+        return f"{self.get_job_id_url(job_id=job_id)}/status"
+
+    def get_job_metrics_url(self, job_id: str) -> str:
+        """Get job-metrics URL using job ID."""
+        return f"{self.get_job_id_url(job_id=job_id)}/metrics"
 
     def get_job_allocations_url(self) -> str:
-        """Get job allocations"""
-        return join(self.jobs_url, "allocations")
+        """Get job-allocations URL."""
+        return f"{self.jobs_url}/allocations"
 
     @property
     def files_url(self):
         """Get files URL."""
-        return join(self.url, self.files)
+        return urljoin(self.url, "optimization/v1/files")
 
-    def get_file_id_url(self, file_id: str) -> str:
+    def get_file_id_url(self, *, file_id: str) -> str:
         """Get file URL with file ID."""
-        return join(self.files_url, file_id)
+        return f"{self.files_url}/{file_id}"
 
-    def get_file_contents_url(self, file_id: str, part_num: int) -> str:
+    def get_file_contents_url(self, *, file_id: str, part_number: int) -> str:
         """Get file contents URL with file ID and file part number."""
-        return join(self.get_file_id_url(file_id), "contents", str(part_num))
+        return f"{self.get_file_id_url(file_id=file_id)}/contents/{str(part_number)}"
 
-    @property
-    def headers_without_authorization(self) -> dict:
-        """HTTP headers without bearer token."""
-        headers = {
-            "Content-Type": "application/json",
-            # Simple, sessionless requests, so close connection proactively.
-            "Connection": "close",
-        }
-
-        if self.timeout is not None:
-            # Tell server when client will stop waiting for response.
-            headers["X-Request-Timeout-Nano"] = str(int(10**9 * self.timeout))
-
-        return headers
-
-    @BaseApi.refresh_token
-    def upload_file(  # pylint: disable=too-many-branches, too-many-locals, too-many-statements
-        self,
-        file: dict,
-    ) -> dict:
+    def upload_file(self, *, file: dict) -> dict:
         """
         Upload file (metadata and then parts concurrently). Returns dict with file ID.
         """
         # Use session with maintained connection and multipart concurrency for
         # efficiency.
         file = data_to_json(file=file)
 
@@ -131,65 +148,67 @@
                         status_forcelist=STATUS_FORCELIST,
                     )
                 ),
             )
 
             post_response_future = session.post(
                 self.files_url,
-                headers=self.headers_without_connection_close,
+                headers=self._auth_client.headers_without_connection_close,
                 timeout=self.timeout,
                 json=utilities.get_post_request_body(file=file),
             )
 
             for response_future in concurrent.futures.as_completed(
                 [post_response_future], self.timeout
             ):
                 response = response_future.result()
-                self._check_response_error(response)
+                raise_for_status(response=response)
 
             file_id = response.json()["file_id"]
             file_part_generator = utilities.file_part_generator(
                 file=file, compress=self.compress
             )
             patch_response_futures = []
 
             if self.compress:
                 for part_body, part_number in file_part_generator:
                     patch_response_futures.append(
                         session.patch(
-                            join(self.files_url, f"{file_id}/contents/{part_number}"),
-                            headers=self.headers_without_connection_close,
+                            self.get_file_contents_url(
+                                file_id=file_id, part_number=part_number
+                            ),
+                            headers=self._auth_client.headers_without_connection_close,
                             timeout=self.timeout,
                             data=utilities.zip_payload(
                                 payload=utilities.get_patch_request_body(file=part_body)
                             ),
                         )
                     )
             else:
                 for part_body, part_number in file_part_generator:
                     patch_response_futures.append(
                         session.patch(
-                            join(self.files_url, f"{file_id}/contents/{part_number}"),
-                            headers=self.headers_without_connection_close,
+                            self.get_file_contents_url(
+                                file_id=file_id, part_number=part_number
+                            ),
+                            headers=self._auth_client.headers_without_connection_close,
                             timeout=self.timeout,
                             json=utilities.get_patch_request_body(file=part_body),
                         )
                     )
 
             # Due to timeout in underlying PATCH, this should not hang despite no
             # timeout.
             for response_future in concurrent.futures.as_completed(
                 patch_response_futures
             ):
-                response = response_future.result()
-                self._check_response_error(response)
+                raise_for_status(response=response_future.result())
 
         return {"file_id": file_id}
 
-    @BaseApi.refresh_token
     def download_file(self, *, file_id: str) -> dict:
         """Download file (metadata and then parts concurrently)."""
         # Use session with maintained connection and multipart concurrency for
         # efficiency.
         with FuturesSession(max_workers=self.max_workers) as session:
             session.mount(
                 "https://",
@@ -199,49 +218,48 @@
                         backoff_factor=BACKOFF_FACTOR,
                         status_forcelist=STATUS_FORCELIST,
                     )
                 ),
             )
 
             get_response_future = session.get(
-                #urljoin(self.files_url, file_id),
-                join(self.files_url, file_id),
-                headers=self.headers_without_connection_close,
+                self.get_file_id_url(file_id=file_id),
+                headers=self._auth_client.headers_without_connection_close,
                 timeout=self.timeout,
             )
 
             for response_future in concurrent.futures.as_completed(
                 [get_response_future], self.timeout
             ):
                 response = response_future.result()
-                self._check_response_error(response)
+                raise_for_status(response=response_future.result())
 
             # File metadata is base for returned fully assembled file.
             file = {**response.json()}
 
             # Remove metadata fields that are not well-defined for fully assembled file.
             file.pop("last_accessed_rfc3339")
             file.pop("upload_date_rfc3339")
 
             get_response_futures = [
                 session.get(
-                    #urljoin(self.files_url, f"{file_id}/contents/{part_number}"),
-                    join(self.files_url, f"{file_id}/contents/{part_number}"),
-                    headers=self.headers_without_connection_close,
+                    self.get_file_contents_url(
+                        file_id=file_id, part_number=part_number
+                    ),
+                    headers=self._auth_client.headers_without_connection_close,
                     timeout=self.timeout,
                 )
                 for part_number in range(1, file["num_parts"] + 1)
             ]
 
             # Due to timeout in underlying GET, this should not hang despite no timeout.
             for response_future in concurrent.futures.as_completed(
                 get_response_futures
             ):
-                response = response_future.result()
-                self._check_response_error(response)
+                raise_for_status(response=response_future.result())
 
             # Unpack in order.
             for response_future in get_response_futures:
                 file_part = response_future.result().json()
                 # Append to all array fields.
                 for file_type, file_type_config in file_part["file_config"].items():
                     if file_type not in file["file_config"]:
@@ -251,472 +269,426 @@
                         if key not in file["file_config"][file_type]:
                             file["file_config"][file_type][key] = []
 
                         file["file_config"][file_type][key] += value
 
         return file
 
-    @BaseApi.refresh_token
-    def submit_job(self, job_body: dict, job_type: str) -> dict:
+    def submit_job(self, *, job_body: dict) -> dict:
         """
-        Submit a job via a request to QCI public API.
+        Submit a job via a request to QCi's optimization API.
 
         Args:
             job_body: formatted json body that includes all parameters for the job
-            job_type: one of the _supported_job_types
 
         Returns:
-            Response from POST call to API
+            Response from POST call to API (see :meth:`get_job_results`)
         """
-        self.validate_job_type(job_type=job_type)
-        response = self.session.request(
-            "POST",
+        response = self._session.post(
             self.jobs_url,
             json=job_body,
-            headers=self.headers,
+            headers=self._auth_client.headers_without_connection_close,
             timeout=self.timeout,
         )
-        self._check_response_error(response=response)
+        raise_for_status(response=response)
+
         return response.json()
 
-    @BaseApi.refresh_token
-    def get_job_status(self, job_id: str) -> dict:
+    def get_job_results(self, *, job_id: str) -> dict:
+        """
+        Get job_info, status, and results of a (possibly uncompleted) job by its ID.
+
+        Args:
+            job_id: ID of job
+
+        Returns:
+            Dictionary with latest job_info, status, and results.
+        """
+        job_info = self.get_job_response(job_id=job_id)
+        status = enum.JobStatus(self.get_job_status(job_id=job_id)["status"])
+
+        if status == enum.JobStatus.COMPLETED:
+            # Simplify file results for users who wait for known results.
+            file = self.download_file(file_id=job_info["job_result"]["file_id"])
+            results = utilities.get_file_config(file=file)[0]
+        else:
+            results = None
+
+        return {"job_info": job_info, "status": status.value, "results": results}
+
+    def get_job_status(self, *, job_id: str) -> dict:
         """
         Get the status of a job by its ID.
 
         Args:
             job_id: ID of job
 
         Returns:
             Response from GET call to API
         """
-        response = self.session.request(
-            "GET",
-            self.get_job_status_url(job_id),
-            headers=self.headers,
+        response = self._session.get(
+            self.get_job_status_url(job_id=job_id),
+            headers=self._auth_client.headers_without_connection_close,
             timeout=self.timeout,
         )
+        raise_for_status(response=response)
 
-        self._check_response_error(response=response)
         return response.json()
 
-    @BaseApi.refresh_token
-    def get_job_response(self, job_id: str, job_type: str) -> dict:
+    def get_job_metrics(self, *, job_id: str) -> dict:
         """
-        Get a response for a job by id and type, which may/may not be finished.
+        Get the metrics for a job by its ID.
 
-        :param job_id: ID of job
-        :param job_type: type of job, one of []
+        Args:
+            job_id: ID of job
 
-        :return dict: loaded json file
+        Returns:
+            Response from GET call to API
         """
-        self.validate_job_type(job_type=job_type)
-        response = self.session.request(
-            "GET",
-            self.get_job_id_url(job_id),
-            headers=self.headers,
+        response = self._session.get(
+            self.get_job_metrics_url(job_id=job_id),
+            headers=self._auth_client.headers_without_connection_close,
             timeout=self.timeout,
         )
+        raise_for_status(response=response)
 
-        self._check_response_error(response=response)
         return response.json()
 
-    def validate_job_type(self, job_type: str) -> None:
+    def get_job_response(self, *, job_id: str) -> dict:
         """
-        Checks if a provided job type is a supported job type.
+        Get a response for a job by id, which may/may not be finished.
 
-        Args:
-            job_type: a job type to validate
+        :param job_id: ID of job
 
-        Returns:
-            None
+        :return dict: json response
+        """
+        response = self._session.get(
+            self.get_job_id_url(job_id=job_id),
+            headers=self._auth_client.headers_without_connection_close,
+            timeout=self.timeout,
+        )
+        raise_for_status(response=response)
+
+        return response.json()
 
-        Raises AssertionError if job_type is not one of the _supported_job_types.
+    def get_allocations(self) -> dict:
         """
-        if job_type not in self._supported_job_types:
-            raise AssertionError(
-                f"Provided job_type '{job_type}' is not one of "
-                f"{self._supported_job_types}"
-            )
+        Get allocations for running jobs on different device classes.
+
+        :return dict: json response
+        """
+        response = self._session.get(
+            self.get_job_allocations_url(),
+            headers=self._auth_client.headers_without_connection_close,
+            timeout=self.timeout,
+        )
+        raise_for_status(response=response)
 
-    def build_job_body(  # pylint: disable=too-many-arguments
+        return response.json()
+
+    def build_job_body(  # pylint: disable=too-many-arguments,too-many-locals,too-many-branches,too-many-statements
         self,
-        job_type: str,
+        *,
+        job_type: Union[enum.JobType, str],
         job_params: dict,
         qubo_file_id: Optional[str] = None,
         graph_file_id: Optional[str] = None,
         hamiltonian_file_id: Optional[str] = None,
         objective_file_id: Optional[str] = None,
         constraints_file_id: Optional[str] = None,
         polynomial_file_id: Optional[str] = None,
         job_name: Optional[str] = None,
         job_tags: Optional[list] = None,
     ) -> dict:
         """
-        Constructs body for job submission requests
+        Constructs body for job submission requests.
 
         Args:
-            job_type: one of _supported_job_types
+            job_type: an enum.JobType or one of the string values defined in enum.JobType
             job_params: dict of params to be passed to job submission in "params" key
             qubo_file_id: file id from files API for uploaded qubo
             graph_file_id: file id from files API for uploaded graph
             hamiltonian_file_id: file id from files API for uploaded hamiltonian
             objective_file_id: file id from files API for uploaded objective
             constraints_file_id: file id from files API for uploaded constraints
             polynomial_file_id: file id from files API for uploaded polynomial
             job_name: user specified name for job submission
             job_tags: user specified labels for classifying and filtering user jobs after submission
 
         Returns:
             None
         """
-        # TODO: Need to add validation for job parameters
-        self.validate_job_type(job_type=job_type)
-
         problem_config = {}
         device_config = {}
 
-        if "sampler_type" not in job_params:
+        # This works even when job_type is already an enum.JobType.
+        job_type = enum.JobType(job_type)
+
+        device_type_param = job_params.get("device_type")
+
+        if device_type_param is None:
+            if "sampler_type" in job_params:
+                warnings.warn(
+                    "the 'sampler_type' key is deprecated, please update your usage to "
+                    "'device_type'"
+                )
+                device_type_param = job_params["sampler_type"]
+
+        if device_type_param is None:
             raise ValueError(
-                "Must define sampler_type in job_params (dirac-1, dirac-2, or dirac-3)."
+                "no 'device_type' specified in job_params, must be one of "
+                f"{enum.DEVICE_TYPES_SORTED}"
             )
 
-        device_name = job_params['sampler_type']
-
-        # TODO: remove this in the future for now map dirac- to eqc but warn of deprecation
-        if "eqc" in device_name:
-            print("WARNING: " + device_name + " will be a deprecated sampler type dirac-(1-3) will be the supported sampler types in the future")
-            device_name = device_name.replace("eqc", "dirac-")
+        # This works even when device_type_param is already an enum.DeviceType.
+        device_type = enum.DeviceType(device_type_param)
 
-        # Optional nsamples.
-        num_samples = job_params.get("nsamples")
+        num_samples = job_params.get("num_samples")
 
         if num_samples is None:
             # Fallback to checking deprecated fields.
             if "n_samples" in job_params:
-                print("WARNING: the key n_samples will be a deprecated parameter in the future, nsamples will be the supported parameter.")
+                warnings.warn(
+                    "the 'n_samples' key is deprecated, please update your usage to "
+                    "'num_samples'"
+                )
                 num_samples = job_params["n_samples"]
-            elif "num_samples" in job_params:
-                print("WARNING: the key num_samples will be a deprecated parameter in the future, nsamples will be the supported parameter.")
-                num_samples = job_params["num_samples"]
+            elif "nsamples" in job_params:
+                warnings.warn(
+                    "the 'nsamples' key is deprecated, please update your usage to "
+                    "'num_samples'"
+                )
+                num_samples = job_params["nsamples"]
             elif "num_solutions" in job_params:
-                print("WARNING: the key num_solutions will be a deprecated parameter in the future, nsamples will be the supported parameter.")
+                warnings.warn(
+                    "the 'num_solutions' key is deprecated, please update your usage "
+                    "to 'num_samples'"
+                )
                 num_samples = job_params["num_solutions"]
 
         if num_samples is not None:
             # Optional parameter.
             device_config["num_samples"] = num_samples
 
-        if job_type == 'sample-qubo':
-            if device_name in ('dirac-2', 'dirac-3'):
+        if job_type == enum.JobType.GRAPH_PARTITIONING:
+            if device_type not in enum.DEVICE_TYPES_QUBIT:
                 raise ValueError(
-                    f"{job_type} not supported on dirac-2 and dirac-3. Consider using "
-                    "job_type sample-hamiltonian for dirac-2 and dirac-3."
+                    f"{job_type.value} not supported on {device_type.value}."
                 )
 
-            problem_name = 'quadratic_unconstrained_binary_optimization'
+            problem_type = enum.ProblemType.GP
 
-            if not qubo_file_id:
+            if not graph_file_id:
                 raise AssertionError(
-                    "qubo_file_id must be specified for job_type='sample-qubo'"
+                    "graph_file_id must be specified for the given job_type "
+                    f"'{job_type.value}'"
                 )
 
-            problem_config["qubo_file_id"] = qubo_file_id
-        elif job_type == 'sample-hamiltonian':
-            if device_name == 'dirac-2':
+            problem_config["graph_file_id"] = graph_file_id
+
+            if "num_paritions" in job_params:
+                # Optional parameter.
+                problem_config["num_paritions"] = job_params["num_paritions"]
+
+            if "alpha" in job_params:
+                # Optional parameter.
+                problem_config["alpha"] = job_params["alpha"]
+
+            if "gamma" in job_params:
+                # Optional parameter when num_paritions > 2.
+                problem_config["gamma"] = job_params["gamma"]
+        elif job_type == enum.JobType.SAMPLE_CONTRAINT:
+            if device_type not in enum.DEVICE_TYPES_QUBIT:
+                raise ValueError(
+                    f"{job_type.value} not supported on {device_type.value}."
+                )
+
+            problem_type = enum.ProblemType.QLCBO
+
+            if not constraints_file_id:
+                raise AssertionError(
+                    "At least constraints_file_id must be specified for job_type "
+                    f"'{job_type.value}'"
+                )
+
+            problem_config["constraints_file_id"] = constraints_file_id
+            problem_config["objective_file_id"] = objective_file_id  # May be None.
+
+            if "alpha" in job_params:
+                # Optional parameter.
+                problem_config["alpha"] = job_params["alpha"]
+
+            if "atol" in job_params:
+                # Optional parameter.
+                problem_config["atol"] = job_params["atol"]
+        elif job_type == enum.JobType.SAMPLE_HAMILTONIAN:
+            if device_type not in enum.DEVICE_TYPES_QUDIT:
+                raise ValueError(
+                    f"{job_type.value} not supported on {device_type.value}."
+                )
+
+            if device_type == enum.DeviceType.DIRAC2:
                 if job_params.get("solution_precision") != 1:
-                    problem_name = 'normalized_qudit_hamiltonian_optimization_continuous'
+                    problem_type = enum.ProblemType.NQHO_CONTINUOUS
                 else:
-                    problem_name = 'normalized_qudit_hamiltonian_optimization_integer'
-            elif device_name == 'dirac-3':
-                problem_name = 'normalized_qudit_hamiltonian_optimization'
+                    problem_type = enum.ProblemType.NQHO_INTEGER
+            elif device_type == enum.DeviceType.DIRAC3:
+                problem_type = enum.ProblemType.NQHO
 
                 if "relaxation_schedule" in job_params:
                     # Optional parameter.
-                    device_config["relaxation_schedule"] = job_params["relaxation_schedule"]
+                    device_config["relaxation_schedule"] = job_params[
+                        "relaxation_schedule"
+                    ]
 
                 if "solution_precision" in job_params:
                     # Optional parameter.
-                    device_config["solution_precision"] = job_params["solution_precision"]
+                    device_config["solution_precision"] = job_params[
+                        "solution_precision"
+                    ]
 
                 if "sum_constraint" in job_params:
                     # Optional parameter.
                     device_config["sum_constraint"] = job_params["sum_constraint"]
             else:
-                raise ValueError(f"{job_type} not supported on {device_name}.")
+                raise ValueError(
+                    f"{job_type.value} not supported on {device_type.value}."
+                )
 
-            if (not hamiltonian_file_id and not polynomial_file_id) or \
-                (hamiltonian_file_id and polynomial_file_id):
+            if (not hamiltonian_file_id and not polynomial_file_id) or (
+                hamiltonian_file_id and polynomial_file_id
+            ):
                 raise AssertionError(
                     "exactly one of hamiltonian_file_id or polynomial_file_id must be "
-                    "specified for job_type='sample-hamiltonian'"
+                    f"specified for job_type='{job_type.value}'"
                 )
 
             if hamiltonian_file_id:
-                problem_config["hamiltonian_file_id"] = hamiltonian_file_id
+                problem_config["hamiltonian_file_id"] = (
+                    hamiltonian_file_id  # Deprecated.
+                )
             else:
                 problem_config["polynomial_file_id"] = polynomial_file_id
-        elif job_type == 'sample-hamiltonian-ising':
-            if device_name in ('dirac-2', 'dirac-3'):
+        elif job_type == enum.JobType.SAMPLE_HAMILTONIAN_ISING:
+            if device_type not in enum.DEVICE_TYPES_QUBIT:
                 raise ValueError(
-                    f"{job_type} not supported on dirac-2 and dirac-3. Consider using "
-                    "job_type sample-hamiltonian for dirac-2 and dirac-3."
+                    f"{job_type.value} not supported on {device_type.value}."
                 )
 
-            problem_name = 'ising_hamiltonian_optimization'
-            
-            if (not hamiltonian_file_id and not polynomial_file_id) or \
-                (hamiltonian_file_id and polynomial_file_id):
+            problem_type = enum.ProblemType.IHO
+
+            if (not hamiltonian_file_id and not polynomial_file_id) or (
+                hamiltonian_file_id and polynomial_file_id
+            ):
                 raise AssertionError(
                     "exactly one of hamiltonian_file_id or polynomial_file_id must be "
-                    "specified for job_type='sample-hamiltonian-ising'"
+                    f"specified for job_type='{job_type.value}'"
                 )
 
             if hamiltonian_file_id:
-                problem_config["hamiltonian_file_id"] = hamiltonian_file_id
+                problem_config["hamiltonian_file_id"] = (
+                    hamiltonian_file_id  # Deprecated.
+                )
             else:
                 problem_config["polynomial_file_id"] = polynomial_file_id
-        elif job_type == "sample-constraint":
-            if device_name in ('dirac-2', 'dirac-3'):
+        elif job_type == enum.JobType.SAMPLE_QUBO:
+            if device_type not in enum.DEVICE_TYPES_QUBIT:
                 raise ValueError(
-                    f"{job_type} not supported on dirac-2 and dirac-3. Consider using "
-                    "job_type sample-hamiltonian for dirac-2 and dirac-3."
-                )
-
-            problem_name = 'quadratic_linearly_constrained_binary_optimization'
-
-            if not constraints_file_id:
-                raise AssertionError(
-                    "At least constraints_file_id must be specified for "
-                    "job_type='sample-constraint'"
+                    f"{job_type.value} not supported on {device_type.value}."
                 )
 
-            problem_config["constraints_file_id"] = constraints_file_id
-            problem_config["objective_file_id"] = objective_file_id  # Optional.
+            problem_type = enum.ProblemType.QUBO
 
-            if "alpha" in job_params:
-                # Optional parameter.
-                problem_config["alpha"] = job_params["alpha"]
-
-            if "atol" in job_params:
-                # Optional parameter.
-                problem_config["atol"] = job_params["atol"]
-        elif job_type == "graph-partitioning":
-            if device_name in ('dirac-2', 'dirac-3'):
-                raise ValueError(
-                    f"{job_type} not supported on dirac-2 and dirac-3. Consider using "
-                    "job_type sample-hamiltonian for dirac-2 and dirac-3."
-                )
-
-            problem_name = 'graph_partitioning'
-
-            if not graph_file_id:
+            if not qubo_file_id:
                 raise AssertionError(
-                    "graph_file_id must be specified for the given "
-                    "job_type='graph-partitioning'"
+                    f"qubo_file_id must be specified for job_type '{job_type.value}'"
                 )
 
-            problem_config["graph_file_id"] = graph_file_id
-
-            if "num_paritions" in job_params:
-                # Optional parameter.
-                problem_config["num_paritions"] = job_params["num_paritions"]
-
-            if "alpha" in job_params:
-                # Optional parameter.
-                problem_config["alpha"] = job_params["alpha"]
-
-            if "gamma" in job_params:
-                # Optional parameter when num_paritions > 2.
-                problem_config["gamma"] = job_params["gamma"]
+            problem_config["qubo_file_id"] = qubo_file_id
         else:
-            raise ValueError(f"Unsupported job_type '{job_type}'.")
+            raise ValueError(f"unsupported job_type '{job_type.value}'.")
 
-        job_submission = {
-            "problem_config": {problem_name: problem_config},
-            "device_config": {device_name: device_config},
+        job_submission: dict = {
+            "problem_config": {problem_type.value: problem_config},
+            "device_config": {device_type.value: device_config},
         }
 
         if job_name is not None:
             # Optional field.
             job_submission["job_name"] = job_name
 
         if job_tags is not None:
             # Optional field.
             job_submission["job_tags"] = job_tags
 
         return {"job_submission": job_submission}
 
-    def print_job_log(self, message: str) -> None:
-        """
-        Formats a messages for updating user with a time stamp appended
-        :param message: a string to be passed in print statement
-        """
-        print(f"{message}: {datetime.now().strftime('%Y/%m/%d %H:%M:%S')}")
-
-    def process_job(self, job_type: str, job_body: dict, wait: bool = True) -> dict:
+    def process_job(
+        self, *, job_body: dict, wait: bool = True, verbose: bool = True
+    ) -> dict:
         """
-        :param job_type: the type of job being processed must be one of _supported_job_types
         :param job_body: formatted json dict for body of job submission request
-        :param wait: bool indicating whether or not user wants to wait for job to complete
+        :param wait: wait synchronously for job to complete
+        :param verbose: track operations' progress using timestamped console logs
 
         :return:
-            if wait is True, then dict with job_info response and results file
-                (results is None if ERRORED or CANCELLED)
-            if wait is False, then response dict from submitted job, which includes job
-                ID for subsequent retrieval
-        :note: what else do we want to return with the results? response_id, obviously job_id
+            if wait is True, then dict with job_info, status, and results and results
+                fields (results is None if job is not successfully COMPLETED)
+            if wait is False, then response dict from submitted job, which includes
+                job_id for subsequent retrieval (see :meth:`get_job_results`)
         """
-        self.validate_job_type(job_type=job_type)
+        dirac_allocation = self.get_allocations()["allocations"]["dirac"]
+        dirac_allocation_s = dirac_allocation["seconds"]
 
-        allocations_response = self.session.request(
-            "GET",
-            self.get_job_allocations_url(),
-            headers=self.headers,
-            timeout=self.timeout,
-        ).json()
-        dirac_allocation = allocations_response['allocations']['dirac']['seconds']
-    
-        if allocations_response['allocations']['dirac']['metered']:
-            print(f"Dirac allocation balance = {dirac_allocation} s")
-        else:
-            print(f"Dirac allocation balance = {dirac_allocation} s (unmetered)")
-    
-        submit_response = self.submit_job(job_body=job_body, job_type=job_type)
-        job_id = submit_response["job_id"]
-        self.print_job_log(message=f"Job submitted job_id='{job_id}'-")
+        log = f"Dirac allocation balance = {dirac_allocation_s} s"
 
-        if wait:
-            curr_status = ""
-            while curr_status not in FINAL_STATUSES:
-                time.sleep(1)
-                iter_status = self.get_job_status(job_id=job_id)["status"]
-
-                if iter_status != curr_status:
-                    self.print_job_log(message=iter_status)
-                    curr_status = iter_status
+        if not dirac_allocation["metered"]:
+            log += " (unmetered)"
 
-            job_response = self.get_job_response(job_id=job_id, job_type=job_type)
-            job_response['details'] = {'status': curr_status}
+        log_to_console(log=log, verbose=verbose)
 
-            if curr_status in [JobStatus.CANCELLED, JobStatus.ERRORED]:
-                results = None
-            else:
-                results = self.download_file(file_id=job_response["job_result"]["file_id"])
+        submit_job_response = self.submit_job(job_body=job_body)
+        job_id = submit_job_response["job_id"]
 
-            allocations_response = self.session.request(
-                "GET",
-                self.get_job_allocations_url(),
-                headers=self.headers,
-                timeout=self.timeout,
-            ).json()
-            dirac_allocation = allocations_response['allocations']['dirac']['seconds']
-        
-            if allocations_response['allocations']['dirac']['metered']:
-                print(f"Dirac allocation balance = {dirac_allocation} s")
-            else:
-                print(f"Dirac allocation balance = {dirac_allocation} s (unmetered)")
+        log_to_console(log=f"Job submitted: job_id='{job_id}'", verbose=verbose)
 
-            return {"job_info": job_response, "results": results}
-
-        return submit_response
-
-    @BaseApi.refresh_token
-    def list_files(self, username: Optional[str] = None) -> dict:
-        """
-        :param username: Optional str - username (to search for files owned by the named user)
-            mostly useful when run by users with administrator privileges (such as QCI users) who can see all files.
-            When called by an administrator, the username parameter is used to restrict the list files returned
-            to be only the files owned by the user specified in the username parameter.
-            When run by non-privileged users, this parameter is truly optional because non-privileged users
-            will only ever see lists of files that they created.
-
-        :return: dict containing list of files
-        """
-        if username:
-            querystring = {"regname": "username", "regvalue": username}
-
-            response = self.session.request(
-                "GET",
-                self.files_url,
-                headers=self.headers,
-                params=querystring,
-                timeout=self.timeout,
-            )
-        else:
-            response = self.session.request(
-                "GET",
-                self.files_url,
-                headers=self.headers,
-                timeout=self.timeout,
-            )
-
-        self._check_response_error(response=response)
-        return response.json()
-
-    @BaseApi.refresh_token
-    def delete_file(self, file_id: str) -> dict:
-        """
-        :param file_id: str - file_id of file to be deleted
-
-        :return: dict containing information about file deleted (or error)
-        """
-
-        if self.debug:
-            print(f"Deleting file with ID {file_id}...")
-
-        start_time_s = time.perf_counter()
+        if wait:
+            status = enum.JobStatus.SUBMITTED
+            while status not in enum.JOB_STATUSES_FINAL:
+                latest_status = enum.JobStatus(
+                    self.get_job_status(job_id=job_id)["status"]
+                )
 
-        response = self.session.request(
-            "DELETE",
-            self.get_file_id_url(file_id),
-            headers=self.headers,
-            timeout=self.timeout,
-        )
+                if latest_status != status:
+                    status = latest_status
+                    log_to_console(log=status.value, verbose=verbose)
 
-        stop_time_s = time.perf_counter()
+                time.sleep(RESULTS_CHECK_INTERVAL_S)
 
-        if self.debug:
-            print(f"Deleting file with ID {file_id}...done.")
-            print(f"\tElapsed time: {stop_time_s - start_time_s} s.")
+            dirac_allocation = self.get_allocations()["allocations"]["dirac"]
+            dirac_allocation_s = dirac_allocation["seconds"]
 
-        self._check_response_error(response=response)
+            log = f"Dirac allocation balance = {dirac_allocation_s} s"
 
-        return response.json()
+            if not dirac_allocation["metered"]:
+                log += " (unmetered)"
 
-    @BaseApi.refresh_token
-    def zip_payload(self, payload: str) -> bytes:
-        """
-        Zip contents of json file
+            log_to_console(log=log, verbose=verbose)
 
-        Args:
-            payload: str - json contents of file to be zipped
+            return self.get_job_results(job_id=job_id)
 
-        Returns:
-            zipped request_body
-        """
-        out = BytesIO()
-        with gzip.GzipFile(fileobj=out, mode="w", compresslevel=6) as file:
-            file.write(json.dumps(payload).encode("utf-8"))
-        request_body = out.getvalue()
-        out.close()
-        return request_body
+        return submit_job_response
 
-    def get_job_type_from_job_id(self, job_id: str) -> str:
+    def list_files(self) -> dict:
         """
-        Get job type from job ID.
-
-        Args:
-            job_id: ID of the job
+        List files (metadata only).
 
-        Returns:
-            Type of the job
+        :return: dict containing list of files
         """
-        response_job_metadata_short = self.session.request(
-            "GET",
-            self.get_job_id_url(job_id),
-            headers=self.headers,
+        response = self._session.get(
+            self.files_url,
+            headers=self._auth_client.headers_without_connection_close,
             timeout=self.timeout,
         )
-        self._check_response_error(response=response_job_metadata_short)
+        raise_for_status(response=response)
 
-        return response_job_metadata_short.json()["type"].replace("_", "-")
+        return response.json()
```

### Comparing `qci_client-3.2.1/qci_client/types.py` & `qci_client-4.0.0/qci_client/optimization/types.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,11 @@
-"""
-Types for Python client for files REST API for optimization service.
+# Copyright 2023-2024, Quantum Computing Incorporated
+"""Types."""
 
-Copyright 2023, Quantum Computing Incorporated
-"""
-
-from typing import Dict, List, Literal, Protocol, TypedDict, Union
-
-# Literals should match corresponding values in enum.FileType.
-Hamiltonian = Literal["hamiltonian"]
-Qubo = Literal["qubo"]
-Objective = Literal["objective"]
-Polynomial = Literal["polynomial"]
-Constraints = Literal["constraints"]
-Graph = Literal["graph"]
-GpResults = Literal["graph_partitioning_results"]
-IhoResults = Literal["ising_hamiltonian_optimization_results"]
-NqhoContinuousResults = Literal[
-    "normalized_qudit_hamiltonian_optimization_continuous_results"
-]
-NqhoIntegerResults = Literal[
-    "normalized_qudit_hamiltonian_optimization_integer_results"
-]
-QlcboResults = Literal["quadratic_linearly_constrained_binary_optimization_results"]
-QuboResults = Literal["quadratic_unconstrained_binary_optimization_results"]
-
-
-class HealthGetResponseBody(TypedDict):
-    """GET health response body."""
-
-    message: str
-
-
-class VersionGetResponseBody(TypedDict):
-    """GET version response body."""
-
-    application_name: str
-    version: str
-
-
-class CountsGetResponseBody(TypedDict):
-    """GET file counts response body."""
-
-    count: int
+from typing import Dict, List, TypedDict, Union
 
 
 class ConstraintsMetadata(TypedDict):
     """Constraints file metadata."""
 
     num_constraints: int
     num_variables: int
@@ -151,30 +111,34 @@
 
 class NqhoContinuousResultsMetadataConfig(TypedDict):
     """
     Continuous Normalized-Qudit Hamiltonian Optimization (NQHO) results file metadata
     configuration.
     """
 
-    normalized_qudit_hamiltonian_optimization_continuous_results: NqhoContinuousResultsMetadata  # pylint: disable=line-too-long
+    normalized_qudit_hamiltonian_optimization_continuous_results: (
+        NqhoContinuousResultsMetadata  # pylint: disable=line-too-long
+    )
 
 
 class NqhoIntegerResultsMetadata(TypedDict):
     """
     Integer normalized-Qudit Hamiltonian Optimization (NQHO) results file metadata.
     """
 
 
 class NqhoIntegerResultsMetadataConfig(TypedDict):
     """
     Integer Normalized-Qudit Hamiltonian Optimization (NQHO) results file metadata
     configuration.
     """
 
-    normalized_qudit_hamiltonian_optimization_integer_results: NqhoIntegerResultsMetadata  # pylint: disable=line-too-long
+    normalized_qudit_hamiltonian_optimization_integer_results: (
+        NqhoIntegerResultsMetadata  # pylint: disable=line-too-long
+    )
 
 
 class NqhoResultsMetadata(TypedDict):
     """Normalized-Qudit Hamiltonian Optimization (NQHO) results file metadata."""
 
 
 class NqhoResultsMetadataConfig(TypedDict):
@@ -216,50 +180,27 @@
 
 class MetadataOptionalPostRequestBody(TypedDict, total=False):
     """Optional file metadata."""
 
     file_name: str
 
 
-class InputMetadataPostRequestBody(MetadataOptionalPostRequestBody):
-    """Request body for POSTing any input file metadata."""
+class MetadataPostRequestBody(MetadataOptionalPostRequestBody):
+    """Request body for POSTing (input) file metadata."""
 
     file_config: Union[
         ConstraintsMetadataConfig,
         GraphMetadataConfig,
         HamiltonianMetadataConfig,
         ObjectiveMetadataConfig,
         PolynomialMetadataConfig,
         QuboMetadataConfig,
     ]
 
 
-class ResultsMetadataPostRequestBody(MetadataOptionalPostRequestBody):
-    """Request body for POSTing any results file metadata."""
-
-    organization_id: str
-    user_id: str
-    file_config: Union[
-        GpResultsMetadataConfig,
-        IhoResultsMetadataConfig,
-        NqhoContinuousResultsMetadataConfig,
-        NqhoIntegerResultsMetadataConfig,
-        NqhoResultsMetadataConfig,
-        QlcboResultsMetadataConfig,
-        QuboResultsMetadataConfig,
-    ]
-
-
-# Request body for POSTing any file metadata.
-MetadataPostRequestBody = Union[
-    InputMetadataPostRequestBody,
-    ResultsMetadataPostRequestBody,
-]
-
-
 class MetadataPostResponseBody(TypedDict):
     """File metadata POST response body."""
 
     file_id: str
 
 
 class MatrixElement(TypedDict):
@@ -408,15 +349,17 @@
     energies: List[float]
     solutions: List[List[float]]
 
 
 class NqhoContinuousResultsPartConfig(TypedDict):
     """Continuous NQHO results file part configuration."""
 
-    normalized_qudit_hamiltonian_optimization_continuous_results: NqhoContinuousResultsPart  # pylint: disable=line-too-long
+    normalized_qudit_hamiltonian_optimization_continuous_results: (
+        NqhoContinuousResultsPart  # pylint: disable=line-too-long
+    )
 
 
 class NqhoIntegerResultsPart(TypedDict):
     """Integer NQHO results file part."""
 
     counts: List[int]
     energies: List[float]
@@ -444,15 +387,16 @@
     distilled_solutions: List[List[int]]
 
 
 class NqhoResultsPartConfig(TypedDict):
     """NQHO results file part configuration."""
 
     normalized_qudit_hamiltonian_optimization_results: Union[
-        NqhoResultsPartWithoutDistilled, NqhoResultsPartWithDistilled,
+        NqhoResultsPartWithoutDistilled,
+        NqhoResultsPartWithDistilled,
     ]
 
 
 class QlcboResultsPart(TypedDict):
     """QLCBO results file part."""
 
     counts: List[int]
@@ -479,30 +423,23 @@
 class QuboResultsPartConfig(TypedDict):
     """QUBO results file part configuration."""
 
     quadratic_unconstrained_binary_optimization_results: QuboResultsPart
 
 
 class PartPatchRequestBody(TypedDict):
-    """The request body for PATCHing all input and results file parts."""
+    """The request body for PATCHing (input) file parts."""
 
     file_config: Union[
         ConstraintsPartConfig,
         GraphPartConfig,
         HamiltonianPartConfig,
         ObjectivePartConfig,
         PolynomialPartConfig,
         QuboPartConfig,
-        GpResultsPartConfig,
-        IhoResultsPartConfig,
-        NqhoContinuousResultsPartConfig,
-        NqhoIntegerResultsPartConfig,
-        NqhoResultsPartConfig,
-        QlcboResultsPartConfig,
-        QuboResultsPartConfig,
     ]
 
 
 class PartPatchResponseBody(TypedDict):
     """File part PATCH response body."""
 
     file_id: str
@@ -562,22 +499,7 @@
         IhoResultsPartConfig,
         NqhoContinuousResultsPartConfig,
         NqhoIntegerResultsPartConfig,
         NqhoResultsPartConfig,
         QlcboResultsPartConfig,
         QuboResultsPartConfig,
     ]
-
-
-class DeleteResponseBody(TypedDict):
-    """File DELETE response body."""
-
-    num_deleted: int
-
-
-class SupportsAccessTokens(Protocol):  # pylint: disable=too-few-public-methods
-    """Interface for clients that are injected to retrieve access tokens."""
-
-    @property
-    def access_token(self) -> str:
-        """Return a valid access token for the API."""
-        ...  # pylint: disable=unnecessary-ellipsis
```

### Comparing `qci_client-3.2.1/qci_client.egg-info/PKG-INFO` & `qci_client-4.0.0/qci_client.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qci-client
-Version: 3.2.1
+Version: 4.0.0
 Summary: Client Package for using Qatalyst Optimization Suite
 Author: Quantum Computing Inc.
 Author-email: support@quantumcomputinginc.com
 License: Apache 2.0
 Project-URL: documentation, https://quantumcomputinginc.com/learn/reference-documentation
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
@@ -14,19 +14,19 @@
 License-File: LICENSE
 Requires-Dist: requests<3,>=2.22.1
 Requires-Dist: requests-futures<2,>=1.0.0
 Requires-Dist: networkx<3,>=2.6.3
 Requires-Dist: numpy<2,>=1.21.1
 Requires-Dist: scipy<2,>=1.7.3
 Provides-Extra: dev
-Requires-Dist: black==23.1.0; extra == "dev"
+Requires-Dist: black<25,>=24.3.0; extra == "dev"
 Requires-Dist: build<0.11,>=0.10.0; extra == "dev"
 Requires-Dist: check-manifest<0.49,>=0.48; extra == "dev"
 Requires-Dist: coverage[toml]<7,>=6.4.2; extra == "dev"
-Requires-Dist: pylint==2.16.2; extra == "dev"
+Requires-Dist: pylint<4,>=3.1.0; extra == "dev"
 Requires-Dist: pytest<8,>=7.2.1; extra == "dev"
 Requires-Dist: sphinx-rtd-theme>=1.3.0; extra == "dev"
 Requires-Dist: twine<4,>=3.7.1; extra == "dev"
 
 # QCI Client
 
 ## Getting started
@@ -39,35 +39,37 @@
 Install `qci-client` from the [public PyPI server](https://pypi.org/)
 into your Python virtual environment using--
 
 ```bash
 pip install qci-client
 ```
 
-### Instantiating a Client
+### Instantiating a Client for Optimization
 
 #### With Environment Variables
 
 To access the API, set these environment variables--
 
 <!-- markdown-link-check-disable-next-line -->
 - QCI_API_URL - URL for Qatalyst API, Example: "https://api.qci-prod.com"
 - QCI_TOKEN - refresh token string for securely accessing Qatalyst API
 
 then instantiate a `QciClient` as follows--
 
 ```python
+# An alias for `from qci_client.optimization.client import Client as QciClient`.
 from qci_client import QciClient
 
 client = QciClient()
 ```
 
 #### Without Environment Variables
 
 Access the API without first defining environment variables by instantiating a
 `QciClient` as follows--
 
 ```python
+# A alias for `from qci_client.optimization.client import Client as QciClient`.
 from qci_client import QciClient
 
 client = QciClient(url="https://api.qci-prod.com", api_token="<secret-token>")
 ```
```

### Comparing `qci_client-3.2.1/tests/test_data_converter.py` & `qci_client-4.0.0/tests/optimization/test_data_converter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,70 +1,69 @@
+# Copyright 2023-2024, Quantum Computing Incorporated
 """Test for data conversion functions."""
 
 import time
 import unittest
 
 import networkx as nx
 import numpy as np
 import pytest
 import scipy.sparse as sp
 
-from qci_client.data_converter import data_to_json
+from qci_client.optimization.data_converter import data_to_json
+
 
 @pytest.mark.offline
 class TestDataToJson(unittest.TestCase):
     """Test suite for data conversion to JSON."""
 
     def test_file_type_assert(self):
         """Test file generation for bad file type."""
         # test file_type assertion
         with self.assertRaises(AssertionError) as context:
-            data_to_json(file={
-                "file_config": {"graph_partitioning_results": {"data": []}}
-            })
+            data_to_json(
+                file={"file_config": {"graph_partitioning_results": {"data": []}}}
+            )
 
         self.assertEqual(
-           str(context.exception),
-           "data conversion not supported for file type 'graph_partitioning_results', "
-           "supported types are ('constraints', 'graph', 'hamiltonian', 'objective', "
-           "'polynomial', 'qubo')"
+            str(context.exception),
+            "unsupported file type, must be one of ['constraints', 'graph', "
+            "'hamiltonian', 'objective', 'polynomial', 'qubo']",
         )
 
     def test_graph_file_body(self):
         """Test file generation for graph data."""
         graph_file = {
             "file_name": "graph.json",
-            "file_config": {
-                "graph": {"data": nx.Graph((((1, 2), (1, 3))))}
-            },
+            "file_config": {"graph": {"data": nx.Graph((((1, 2), (1, 3))))}},
         }
         expected = {
             "file_name": "graph.json",
             "file_config": {
                 "graph": {
                     "num_edges": 2,
                     "num_nodes": 3,
                     "directed": False,
                     "multigraph": False,
                     "graph": {},
-                    "nodes": [{'id': 1}, {'id': 2}, {'id': 3}],
+                    "nodes": [{"id": 1}, {"id": 2}, {"id": 3}],
                     "links": [{"source": 1, "target": 2}, {"source": 1, "target": 3}],
                 },
             },
         }
         got = data_to_json(file=graph_file)
         self.assertDictEqual(got, expected)
 
         graph_file["file_config"]["graph"]["data"] = []
 
         with self.assertRaises(AssertionError) as context:
-           data_to_json(file=graph_file)
+            data_to_json(file=graph_file)
 
         self.assertEqual(
-           str(context.exception), "file_type 'graph' data must be a networkx.Graph"
+            str(context.exception), "file type 'graph' data must be type networkx.Graph"
         )
 
     @pytest.mark.timing
     def test_large_data_conversion(self):
         """Test file generation for large data is sufficiently fast."""
         large_qubo = np.random.normal(size=(3000, 3000))
         large_qubo = large_qubo + large_qubo.T
@@ -90,35 +89,35 @@
         }
 
         with self.assertRaises(AssertionError) as context:
             data_to_json(file=bad_hamiltonian_file)
 
         self.assertEqual(
             str(context.exception),
-            "file_type 'hamiltonian' data cannot be a networkx.Graph",
+            "file type 'hamiltonian' does not support networkx.Graph data",
         )
 
     def test_assert_type_not_list(self):
         """Test file generation for improperly formatted qubo data."""
         bad_qubo_file = {
             "file_config": {
                 "qubo": {
                     "num_variables": 3,
                     "data": [[1, -1], [-1, 1]],
                 }
             }
         }
-    
+
         with self.assertRaises(ValueError) as context:
             data_to_json(file=bad_qubo_file)
 
         self.assertEqual(
             str(context.exception),
-            "file_type 'qubo' only supports types numpy.ndarray and "
-            "scipy.sparse.spmatrix, got <class 'list'>",
+            "file type 'qubo' only supports numpy.ndarray and scipy.sparse.spmatrix "
+            "data types, got '<class 'list'>'",
         )
 
     def test_hamiltonian_file_body(self):
         """Test file generation for a hamiltonian matrix."""
         expected = {
             "file_name": "hamiltonian.json",
             "file_config": {
@@ -127,30 +126,30 @@
                     "data": [
                         {"i": 0, "j": 0, "val": -1.0},
                         {"i": 0, "j": 1, "val": 1.0},
                         {"i": 0, "j": 2, "val": 1.0},
                         {"i": 1, "j": 0, "val": 1.0},
                         {"i": 1, "j": 1, "val": -1.0},
                         {"i": 1, "j": 2, "val": 1.0},
-                    ]
+                    ],
                 }
-            }
+            },
         }
 
         ham_np = np.array([[-1, 1, 1], [1, -1, 1]])
 
         file = {
             "file_name": "hamiltonian.json",
-            "file_config": {"hamiltonian": {"data": ham_np}}
+            "file_config": {"hamiltonian": {"data": ham_np}},
         }
         self.assertDictEqual(data_to_json(file=file), expected)
 
         file = {
             "file_name": "hamiltonian.json",
-            "file_config": {"hamiltonian": {"data": sp.dok_matrix(ham_np)}}
+            "file_config": {"hamiltonian": {"data": sp.dok_matrix(ham_np)}},
         }
         self.assertDictEqual(data_to_json(file=file), expected)
 
     def test_qubo_file_body(self):
         """Test file generation for a qubo matrix."""
         expected = {
             "file_name": "qubo.json",
@@ -158,30 +157,27 @@
                 "qubo": {
                     "num_variables": 2,
                     "data": [
                         {"i": 0, "j": 0, "val": -1.0},
                         {"i": 0, "j": 1, "val": 1.0},
                         {"i": 1, "j": 0, "val": 1.0},
                         {"i": 1, "j": 1, "val": -1.0},
-                    ]
+                    ],
                 }
-            }
+            },
         }
 
         q_obj_np = np.array([[-1.0, 1.0], [1.0, -1.0]])
 
-        file = {
-            "file_name": "qubo.json",
-            "file_config": {"qubo": {"data": q_obj_np}}
-        }
+        file = {"file_name": "qubo.json", "file_config": {"qubo": {"data": q_obj_np}}}
         self.assertDictEqual(data_to_json(file=file), expected)
 
         file = {
             "file_name": "qubo.json",
-            "file_config": {"qubo": {"data": sp.dok_matrix(q_obj_np)}}
+            "file_config": {"qubo": {"data": sp.dok_matrix(q_obj_np)}},
         }
         self.assertDictEqual(data_to_json(file=file), expected)
 
     def test_objective_file_body(self):
         """Test file generation for an objective matrix."""
         expected = {
             "file_name": "objective.json",
@@ -189,30 +185,30 @@
                 "objective": {
                     "num_variables": 2,
                     "data": [
                         {"i": 0, "j": 0, "val": -1.0},
                         {"i": 0, "j": 1, "val": 1.0},
                         {"i": 1, "j": 0, "val": 1.0},
                         {"i": 1, "j": 1, "val": -1.0},
-                    ]
+                    ],
                 }
-            }
+            },
         }
 
         obj_np = np.array([[-1.0, 1.0], [1.0, -1.0]])
 
         file = {
             "file_name": "objective.json",
-            "file_config": {"objective": {"data": obj_np}}
+            "file_config": {"objective": {"data": obj_np}},
         }
         self.assertDictEqual(data_to_json(file=file), expected)
 
         file = {
             "file_name": "objective.json",
-            "file_config": {"objective": {"data": sp.dok_matrix(obj_np)}}
+            "file_config": {"objective": {"data": sp.dok_matrix(obj_np)}},
         }
         self.assertDictEqual(data_to_json(file=file), expected)
 
     def test_constraints_file_body(self):
         """Test file generation for a constraints matrix."""
         expected = {
             "file_name": "constraints.json",
@@ -220,30 +216,30 @@
                 "constraints": {
                     "num_constraints": 1,
                     "num_variables": 2,
                     "data": [
                         {"i": 0, "j": 0, "val": 1.0},
                         {"i": 0, "j": 1, "val": 1.0},
                         {"i": 0, "j": 2, "val": -2.0},
-                    ]
+                    ],
                 }
-            }
+            },
         }
 
         con_np = np.array([[1.0, 1.0, -2.0]])
 
         file = {
             "file_name": "constraints.json",
-            "file_config": {"constraints": {"data": con_np}}
+            "file_config": {"constraints": {"data": con_np}},
         }
         self.assertDictEqual(data_to_json(file=file), expected)
 
         file = {
             "file_name": "constraints.json",
-            "file_config": {"constraints": {"data": sp.dok_matrix(con_np)}}
+            "file_config": {"constraints": {"data": sp.dok_matrix(con_np)}},
         }
         self.assertDictEqual(data_to_json(file=file), expected)
 
     def test_polynomial_file_body(self):
         """Test file generation for a polynomial."""
         data = [
             {"idx": [0, 0, 0], "val": 1.0},
@@ -263,22 +259,22 @@
             "file_config": {
                 "polynomial": {
                     "min_degree": 0,
                     "max_degree": 3,
                     "num_variables": 2,
                     "data": data,
                 }
-            }
+            },
         }
 
         file = {
             "file_name": "polynomial.json",
             "file_config": {
                 "polynomial": {
                     "min_degree": 0,
                     "max_degree": 3,
                     "num_variables": 2,
                     "data": data,
                 }
-            }
+            },
         }
         self.assertDictEqual(data_to_json(file=file), expected)
```

### Comparing `qci_client-3.2.1/tests/test_qci_client.py` & `qci_client-4.0.0/tests/optimization/test_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,241 +1,421 @@
-"""
-Missing tests:
- - failures should be accounted for under the BaseApi
- - Each job should also be covered for process_job only 3/5 currently are.
-"""
-
-from contextlib import redirect_stdout
-from datetime import datetime
-import io
-from math import ceil
-from typing import Optional
+# Copyright 2023-2024, Quantum Computing Incorporated
+"""Test client for QCi's optimization API."""
+
+from itertools import product
 import unittest
 import unittest.mock
 
 import networkx as nx
 import numpy as np
 import pytest
-import requests
 import scipy.sparse as sp
 
-from qci_client import JobStatus, QciClient, compute_results_step_len
+import qci_client
 
 
 @pytest.mark.offline
-class TestJobStatus(unittest.TestCase):
-    """JobStatus-related test suite."""
+class TestClientOffline(unittest.TestCase):
+    """Jobs-API-related test suite that can be run without backend."""
+
+    def setUp(self):
+        with pytest.MonkeyPatch().context() as mp:
+            mp.setenv("QCI_TOKEN", "test_api_token")
+            mp.setenv("QCI_API_URL", "test_url")
+            self.client = qci_client.QciClient()
+        self.job_id = "63b717a22da68618ec444eac"
+        self.file_id = "73b717a22da68618ec444eab"
+
+    def test_jobs_url(self) -> None:
+        """Test getting jobs URL."""
+        self.assertEqual(self.client.jobs_url, "test_url/optimization/v1/jobs")
+
+    def test_get_job_id_url(self) -> None:
+        """Test getting jobs URL for given job ID."""
+        self.assertEqual(
+            self.client.get_job_id_url(job_id=self.job_id),
+            f"test_url/optimization/v1/jobs/{self.job_id}",
+        )
+
+    def test_get_job_status_url(self) -> None:
+        """Test getting jobs-status URL for given job ID."""
+        self.assertEqual(
+            self.client.get_job_status_url(job_id=self.job_id),
+            f"test_url/optimization/v1/jobs/{self.job_id}/status",
+        )
+
+    def test_get_job_allocations_url(self) -> None:
+        """Test getting jobs-allocations URL."""
+        self.assertEqual(
+            self.client.get_job_allocations_url(),
+            "test_url/optimization/v1/jobs/allocations",
+        )
+
+    def test_files_url(self) -> None:
+        """Test getting files URL."""
+        self.assertEqual(self.client.files_url, "test_url/optimization/v1/files")
+
+    def test_get_file_id_url(self) -> None:
+        """Test getting files URL for given file ID."""
+        self.assertEqual(
+            self.client.get_file_id_url(file_id=self.file_id),
+            f"test_url/optimization/v1/files/{self.file_id}",
+        )
+
+    def test_get_file_contents_url(self) -> None:
+        """Test getting files contents URL for given file ID."""
+        self.assertEqual(
+            self.client.get_file_contents_url(file_id=self.file_id, part_number=24),
+            f"test_url/optimization/v1/files/{self.file_id}/contents/24",
+        )
+
+    def test_build_job_body(self):
+        """Test building of various jobs' request bodies."""
+
+        with self.assertRaises(ValueError) as context:
+            self.client.build_job_body(
+                job_type="sample-qubo",
+                job_params={},
+                qubo_file_id="qubo_file_id",
+            )
+
+        self.assertEqual(
+            str(context.exception),
+            "no 'device_type' specified in job_params, must be one of "
+            "('dirac-1', 'dirac-2', 'dirac-3')",
+        )
+
+        constraint_body = self.client.build_job_body(
+            job_type="sample-constraint",
+            job_params={
+                "device_type": "dirac-1",
+                "alpha": 5.0,
+            },
+            objective_file_id="obj_fid",
+            constraints_file_id="cons_fid",
+            job_name="foobar_name",
+            job_tags=["foobar_tag1", "foobar_tag2"],
+        )
+
+        self.assertDictEqual(
+            constraint_body,
+            {
+                "job_submission": {
+                    "job_name": "foobar_name",
+                    "job_tags": ["foobar_tag1", "foobar_tag2"],
+                    "problem_config": {
+                        "quadratic_linearly_constrained_binary_optimization": {
+                            "objective_file_id": "obj_fid",
+                            "constraints_file_id": "cons_fid",
+                            "alpha": 5.0,
+                        }
+                    },
+                    "device_config": {"dirac-1": {}},
+                }
+            },
+        )
 
-    def test_jobstatus(self):
-        """Test all job statuses."""
-        job_status = JobStatus()
-        self.assertEqual(job_status.QUEUED, "QUEUED")
-        self.assertEqual(job_status.SUBMITTED, "SUBMITTED")
-        self.assertEqual(job_status.RUNNING, "RUNNING")
-        self.assertEqual(job_status.COMPLETED, "COMPLETED")
-        self.assertEqual(job_status.ERRORED, "ERRORED")
-        self.assertEqual(job_status.CANCELLED, "CANCELLED")
+        qubo_body = self.client.build_job_body(
+            job_type="sample-qubo",
+            job_params={
+                "num_samples": 24,
+                "device_type": "dirac-1",
+            },
+            qubo_file_id="qubo_fid",
+            job_name="foobar_name",
+        )
 
+        self.assertDictEqual(
+            qubo_body,
+            {
+                "job_submission": {
+                    "job_name": "foobar_name",
+                    "problem_config": {
+                        "quadratic_unconstrained_binary_optimization": {
+                            "qubo_file_id": "qubo_fid",
+                        }
+                    },
+                    "device_config": {"dirac-1": {"num_samples": 24}},
+                }
+            },
+        )
 
-class TestQciClientFiles(unittest.TestCase):
-    """Files-API-related test suite."""
+        hamiltonian_body = self.client.build_job_body(
+            job_type="sample-hamiltonian",
+            job_params={
+                "num_samples": 24,
+                "device_type": "dirac-3",
+                "sum_constraint": 200,
+                "solution_precision": 1,
+            },
+            hamiltonian_file_id="hamiltonian_fid",
+            job_tags=["foobar_tag1", "foobar_tag2"],
+        )
+
+        self.assertDictEqual(
+            hamiltonian_body,
+            {
+                "job_submission": {
+                    "job_tags": ["foobar_tag1", "foobar_tag2"],
+                    "problem_config": {
+                        "normalized_qudit_hamiltonian_optimization": {
+                            "hamiltonian_file_id": "hamiltonian_fid",
+                        }
+                    },
+                    "device_config": {
+                        "dirac-3": {
+                            "num_samples": 24,
+                            "sum_constraint": 200,
+                            "solution_precision": 1,
+                        }
+                    },
+                }
+            },
+        )
+
+        hamiltonian_body = self.client.build_job_body(
+            job_type="sample-hamiltonian",
+            job_params={
+                "device_type": "dirac-3",
+                "sum_constraint": 200,
+                "solution_precision": 1,
+            },
+            polynomial_file_id="polynomial_fid",
+        )
+
+        self.assertDictEqual(
+            hamiltonian_body,
+            {
+                "job_submission": {
+                    "problem_config": {
+                        "normalized_qudit_hamiltonian_optimization": {
+                            "polynomial_file_id": "polynomial_fid",
+                        }
+                    },
+                    "device_config": {
+                        "dirac-3": {
+                            "sum_constraint": 200,
+                            "solution_precision": 1,
+                        }
+                    },
+                }
+            },
+        )
+
+        hamiltonian_body = self.client.build_job_body(
+            job_type="sample-hamiltonian",
+            job_params={"device_type": "dirac-3", "sum_constraint": 2.4},
+            polynomial_file_id="polynomial_fid",
+        )
+
+        self.assertDictEqual(
+            hamiltonian_body,
+            {
+                "job_submission": {
+                    "problem_config": {
+                        "normalized_qudit_hamiltonian_optimization": {
+                            "polynomial_file_id": "polynomial_fid",
+                        }
+                    },
+                    "device_config": {
+                        "dirac-3": {
+                            "sum_constraint": 2.4,
+                        }
+                    },
+                }
+            },
+        )
+
+        hamiltonian_body = self.client.build_job_body(
+            job_type="sample-hamiltonian",
+            job_params={
+                "device_type": "dirac-3",
+                "sum_constraint": 2.4,
+                "solution_precision": 0.1,
+            },
+            hamiltonian_file_id="hamiltonian_fid",
+        )
+
+        self.assertDictEqual(
+            hamiltonian_body,
+            {
+                "job_submission": {
+                    "problem_config": {
+                        "normalized_qudit_hamiltonian_optimization": {
+                            "hamiltonian_file_id": "hamiltonian_fid",
+                        }
+                    },
+                    "device_config": {
+                        "dirac-3": {
+                            "sum_constraint": 2.4,
+                            "solution_precision": 0.1,
+                        }
+                    },
+                }
+            },
+        )
+
+        graph_body = self.client.build_job_body(
+            job_type="graph-partitioning",
+            job_params={
+                "device_type": "dirac-1",
+                "num_samples": 42,
+            },
+            graph_file_id="graph_fid",
+        )
+
+        self.assertDictEqual(
+            graph_body,
+            {
+                "job_submission": {
+                    "problem_config": {
+                        "graph_partitioning": {
+                            "graph_file_id": "graph_fid",
+                        }
+                    },
+                    "device_config": {
+                        "dirac-1": {
+                            "num_samples": 42,
+                        }
+                    },
+                }
+            },
+        )
+
+
+class TestClient(unittest.TestCase):  # pylint: disable=too-many-public-methods
+    """Collection of tests for file uploads and jobs with results downloads."""
 
     @classmethod
     def setUpClass(cls):
-        cls.q1 = QciClient()
+        cls.client = qci_client.QciClient()
         cls.graph_dict_input = {
             "file_name": "graph.json",
-            "file_config": {
-                "graph": {
-                    "data": nx.Graph(((1, 2), (1, 3)))
-                }
-            }
+            "file_config": {"graph": {"data": nx.Graph(((1, 2), (1, 3)))}},
         }
 
         cls.qubo_dict_input = {
             "file_name": "qubo.json",
             "file_config": {
-                "qubo": {
-                    "data": sp.csr_matrix(
-                        [
-                            [-1.0, 1.0],
-                            [1.0, -1.0]
-                        ]
-                    )
-                }
-            }
+                "qubo": {"data": sp.csr_matrix([[-1.0, 1.0], [1.0, -1.0]])}
+            },
         }
 
         cls.objective_dict_input = {
             "file_name": "objective.json",
             "file_config": {
-                "objective": {
-                    "data": sp.csc_matrix(
-                        [
-                            [-1.0, 1.0],
-                            [1.0, -1.0]
-                        ]
-                    )
-                }
-            }
+                "objective": {"data": sp.csc_matrix([[-1.0, 1.0], [1.0, -1.0]])}
+            },
         }
 
         cls.constraint_dict_input = {
             "file_name": "constraints.json",
             "file_config": {
                 "constraints": {
                     "data": sp.coo_matrix(
                         [
                             [-1.0, 1.0, 1.0],
                         ]
                     )
                 }
-            }
+            },
         }
 
         cls.hamiltonian_dict_input = {
             "file_name": "hamiltonian.json",
             "file_config": {
-                "hamiltonian": {
-                    "data": np.array(
-                        [
-                            [1.0, 1.0, 0.0],
-                            [2.0, 0.0, 1.0]
-                        ]
-                    )
-                }
-            }
+                "hamiltonian": {"data": np.array([[1.0, 1.0, 0.0], [2.0, 0.0, 1.0]])}
+            },
         }
 
         cls.polynomial_dict_hamiltonian_input = {
             "file_name": "polynomial-hamiltonian.json",
             "file_config": {
                 "polynomial": {
                     "min_degree": 1,
                     "max_degree": 2,
                     "num_variables": 2,
                     "data": [
-                        {
-                            "idx": [0, 1],
-                            "val": 1.0
-                        },
-                        {
-                            "idx": [1, 1],
-                            "val": -2.0
-                        },
-                        {
-                            "idx": [1, 2],
-                            "val": 1.0
-                        },
-                        {
-                            "idx": [2, 2],
-                            "val": -1.0
-                        }
-
-                    ]
+                        {"idx": [0, 1], "val": 1.0},
+                        {"idx": [1, 1], "val": -2.0},
+                        {"idx": [1, 2], "val": 1.0},
+                        {"idx": [2, 2], "val": -1.0},
+                    ],
                 }
-            }
+            },
         }
 
         cls.polynomial_dict_input = {
             "file_name": "polynomial.json",
             "file_config": {
                 "polynomial": {
                     "min_degree": 2,
                     "max_degree": 4,
                     "num_variables": 2,
                     "data": [
-                        {
-                            "idx": [0, 0, 1, 1],
-                            "val": 1.0
-                        },
-                        {
-                            "idx": [0, 1, 1, 1],
-                            "val": -2.0
-                        },
-                        {
-                            "idx": [1, 1, 1, 1],
-                            "val": 1.0
-                        }
-                    ]
+                        {"idx": [0, 0, 1, 1], "val": 1.0},
+                        {"idx": [0, 1, 1, 1], "val": -2.0},
+                        {"idx": [1, 1, 1, 1], "val": 1.0},
+                    ],
                 }
-            }
+            },
         }
 
-        cls.graph_file_id = cls.q1.upload_file(file=cls.graph_dict_input)["file_id"]
-        cls.qubo_file_id = cls.q1.upload_file(file=cls.qubo_dict_input)["file_id"]
-        cls.objective_file_id = cls.q1.upload_file(file=cls.objective_dict_input)[
-            "file_id"
-        ]
-        cls.constraints_file_id = cls.q1.upload_file(file=cls.constraint_dict_input)[
+        cls.graph_file_id = cls.client.upload_file(file=cls.graph_dict_input)["file_id"]
+        cls.qubo_file_id = cls.client.upload_file(file=cls.qubo_dict_input)["file_id"]
+        cls.objective_file_id = cls.client.upload_file(file=cls.objective_dict_input)[
             "file_id"
         ]
-        cls.hamiltonian_file_id = cls.q1.upload_file(file=cls.hamiltonian_dict_input)[
-            "file_id"
-        ]
-        cls.polynomial_hamiltonian_file_id = cls.q1.upload_file(
+        cls.constraints_file_id = cls.client.upload_file(
+            file=cls.constraint_dict_input
+        )["file_id"]
+        cls.hamiltonian_file_id = cls.client.upload_file(
+            file=cls.hamiltonian_dict_input
+        )["file_id"]
+        cls.polynomial_hamiltonian_file_id = cls.client.upload_file(
             file=cls.polynomial_dict_hamiltonian_input
         )["file_id"]
-        cls.polynomial_min_degree_2_max_degree_4_file_id = cls.q1.upload_file(
-            file=cls.polynomial_dict_input)["file_id"]
-
-        cls.all_statuses = [
-            JobStatus.QUEUED,
-            JobStatus.SUBMITTED,
-            JobStatus.RUNNING,
-            JobStatus.COMPLETED,
-            JobStatus.ERRORED,
-            JobStatus.CANCELLED,
-        ]
-
-        cls.final_status = [JobStatus.COMPLETED, JobStatus.ERRORED, JobStatus.CANCELLED]
+        cls.polynomial_min_degree_2_max_degree_4_file_id = cls.client.upload_file(
+            file=cls.polynomial_dict_input
+        )["file_id"]
 
-        cls.job_info = set(("job_id", "details", "job_results", "job_submission",))
-        cls.result_keys = ["samples", "energies", "file_name", "file_type"]
+        cls.job_info = set(("job_info", "results", "status"))
 
         cls.graph_job_body = {
             "job_submission": {
                 "job_name": "job_0",
                 "problem_config": {
-                    "graph_partitioning": {
-                        "graph_file_id": cls.graph_file_id
-                    },
+                    "graph_partitioning": {"graph_file_id": cls.graph_file_id},
                 },
-                "device_config": {
-                    "dirac-1": {}
-                }
+                "device_config": {"dirac-1": {}},
             }
         }
 
         cls.qubo_job_body = {
             "job_submission": {
                 "job_name": "job_0",
                 "problem_config": {
                     "quadratic_unconstrained_binary_optimization": {
                         "qubo_file_id": cls.qubo_file_id
                     },
                 },
-                "device_config": {
-                    "dirac-1": {}
-                }
+                "device_config": {"dirac-1": {}},
             }
         }
 
         cls.constraint_job_body = {
             "job_submission": {
                 "job_name": "job_0",
                 "problem_config": {
                     "quadratic_linearly_constrained_binary_optimization": {
                         "objective_file_id": cls.objective_file_id,
-                        "constraints_file_id": cls.constraints_file_id
+                        "constraints_file_id": cls.constraints_file_id,
                     }
                 },
-                "device_config": {
-                    "dirac-1": {}
-                }
+                "device_config": {"dirac-1": {}},
             }
         }
 
         cls.hamiltonian_job_body_ising_dirac1 = {
             "job_submission": {
                 "job_name": "dirac-1",
                 "problem_config": {
@@ -243,72 +423,63 @@
                         "hamiltonian_file_id": cls.hamiltonian_file_id
                     },
                 },
                 "device_config": {
                     "dirac-1": {
                         "num_samples": 2,
                     }
-                }
+                },
             }
         }
 
         cls.polynomial_job_body_ising_dirac1 = {
             "job_submission": {
                 "job_name": "dirac-1",
                 "problem_config": {
                     "ising_hamiltonian_optimization": {
                         "polynomial_file_id": cls.polynomial_hamiltonian_file_id
                     },
                 },
-                "device_config": {
-                    "dirac-1": {
-                    }
-                }
+                "device_config": {"dirac-1": {}},
             }
         }
 
         cls.hamiltonian_job_body_continous_dirac2 = {
             "job_submission": {
                 "job_name": "dirac-2",
                 "problem_config": {
                     "normalized_qudit_hamiltonian_optimization_continuous": {
                         "hamiltonian_file_id": cls.hamiltonian_file_id
                     }
                 },
-                "device_config": {
-                    "dirac-2": {}
-                }
+                "device_config": {"dirac-2": {}},
             }
         }
 
         cls.hamiltonian_job_body_integer_dirac2 = {
             "job_submission": {
                 "job_name": "dirac-2",
                 "problem_config": {
                     "normalized_qudit_hamiltonian_optimization_integer": {
                         "hamiltonian_file_id": cls.hamiltonian_file_id
                     },
                 },
-                "device_config": {
-                    "dirac-2": {}
-                }
+                "device_config": {"dirac-2": {}},
             }
         }
 
         cls.polynomial_job_body_hamiltonian_continuous_dirac2 = {
             "job_submission": {
                 "job_name": "dirac-2",
                 "problem_config": {
                     "normalized_qudit_hamiltonian_optimization_continuous": {
                         "polynomial_file_id": cls.polynomial_hamiltonian_file_id
                     },
                 },
-                "device_config": {
-                    "dirac-2": {}
-                }
+                "device_config": {"dirac-2": {}},
             }
         }
 
         cls.polynomial_job_body_hamiltonian_integer_dirac2 = {
             "job_submission": {
                 "job_name": "dirac-2",
                 "problem_config": {
@@ -316,15 +487,15 @@
                         "polynomial_file_id": cls.polynomial_hamiltonian_file_id
                     },
                 },
                 "device_config": {
                     "dirac-2": {
                         "num_samples": 2,
                     }
-                }
+                },
             }
         }
 
         cls.hamiltonian_job_body_undistilled_dirac3 = {
             "job_submission": {
                 "job_name": "dirac-3",
                 "problem_config": {
@@ -333,15 +504,15 @@
                     }
                 },
                 "device_config": {
                     "dirac-3": {
                         "relaxation_parameter": 1,
                         "sum_constraint": 2.4,
                     }
-                }
+                },
             }
         }
 
         cls.hamiltonian_job_body_distilled_continuous_dirac3 = {
             "job_submission": {
                 "job_name": "dirac-3",
                 "problem_config": {
@@ -351,15 +522,15 @@
                 },
                 "device_config": {
                     "dirac-3": {
                         "relaxation_parameter": 1,
                         "sum_constraint": 2.4,
                         "solution_precision": 0.1,
                     }
-                }
+                },
             }
         }
 
         cls.hamiltonian_job_body_distilled_integer_dirac3 = {
             "job_submission": {
                 "job_name": "dirac-3",
                 "problem_config": {
@@ -368,15 +539,15 @@
                     }
                 },
                 "device_config": {
                     "dirac-3": {
                         "relaxation_parameter": 1,
                         "solution_precision": 1,
                     }
-                }
+                },
             }
         }
 
         cls.polynomial_min_degree_2_max_degree_4_job_body_distilled_continuous_dirac3 = {
             "job_submission": {
                 "job_name": "dirac-3",
                 "problem_config": {
@@ -386,538 +557,374 @@
                 },
                 "device_config": {
                     "dirac-3": {
                         "relaxation_parameter": 2,
                         "sum_constraint": 2.4,
                         "solution_precision": 0.1,
                     }
-                }
+                },
             }
         }
 
+    # Files tests.
+
     def test_upload_file_error(self):
         """Test uploading improperly formatted file."""
-        with self.assertRaises(KeyError):
-            error_input = {
-                "file_type": "graph",
+        with self.assertRaises(AssertionError):
+            bad_file = {
                 "file_name": "qubo.json",
-                "data": [
-                    {"i": 0, "j": 0, "val": -1.0},
-                    {"i": 0, "j": 1, "val": 1.0},
-                    {"i": 1, "j": 0, "val": 1.0},
-                    {"i": 1, "j": 1, "val": -1.0},
-                ],
-                "num_variables": 2,
+                "file_config": {
+                    "graph": {
+                        "data": [
+                            {"i": 0, "j": 0, "val": -1.0},
+                            {"i": 0, "j": 1, "val": 1.0},
+                            {"i": 1, "j": 0, "val": 1.0},
+                            {"i": 1, "j": 1, "val": -1.0},
+                        ],
+                        "num_variables": 2,
+                    }
+                },
             }
-            self.q1.upload_file(file=error_input)
+            self.client.upload_file(file=bad_file)
 
     def test_upload_file(self):
         """Test uploading of various file types."""
-        graph_upload = self.q1.upload_file(file=self.graph_dict_input)
+        graph_upload = self.client.upload_file(file=self.graph_dict_input)
         self.assertIn("file_id", graph_upload)
         self.assertIsInstance(graph_upload["file_id"], str)
 
-        qubo_upload = self.q1.upload_file(file=self.qubo_dict_input)
+        qubo_upload = self.client.upload_file(file=self.qubo_dict_input)
         self.assertIn("file_id", qubo_upload)
         self.assertIsInstance(qubo_upload["file_id"], str)
 
-        objective_upload = self.q1.upload_file(file=self.objective_dict_input)
+        objective_upload = self.client.upload_file(file=self.objective_dict_input)
         self.assertIn("file_id", objective_upload)
         self.assertIsInstance(objective_upload["file_id"], str)
 
-        constraint_upload = self.q1.upload_file(file=self.constraint_dict_input)
+        constraint_upload = self.client.upload_file(file=self.constraint_dict_input)
         self.assertIn("file_id", constraint_upload)
         self.assertIsInstance(constraint_upload["file_id"], str)
 
-        hamiltonian_upload = self.q1.upload_file(file=self.hamiltonian_dict_input)
+        hamiltonian_upload = self.client.upload_file(file=self.hamiltonian_dict_input)
         self.assertIn("file_id", hamiltonian_upload)
         self.assertIsInstance(hamiltonian_upload["file_id"], str)
 
-    def test_validate_job_type(self):
-        """Test validation of job type against whitelist."""
-        test_job_type = "fake_job_type"
-        expected_err_str = f"Provided job_type '{test_job_type}' is not one of {self.q1._supported_job_types}"  # pylint: disable=protected-access
+    def test_upload_download_file_hamiltonian_matrix_multipart(self):
+        """Test uploading and downloading a larger multipart file for square matrix."""
+        num_parts_expected = 2
+        num_variables = 150
+        density = 0.5
+        format_ = "dok"
+        dtype = np.float32
+        J = sp.random(  # pylint: disable=invalid-name
+            num_variables, num_variables, density=density, format=format_, dtype=dtype
+        )
+        J = (J + J.T) / 2  # pylint: disable=invalid-name
+        h = sp.random(num_variables, 1, density=density, format=format_, dtype=dtype)
+        matrix_upload = sp.hstack((h, J), format=format_, dtype=dtype)
 
-        with self.assertRaises(AssertionError) as context:
-            self.q1.validate_job_type(job_type=test_job_type)
+        file_upload = {
+            "file_name": "multipart-matrix-upload-download-test",
+            "file_config": {
+                "hamiltonian": {
+                    "num_variables": num_variables,
+                    "data": matrix_upload,
+                },
+            },
+        }
 
-        # TODO: consider asserting on exception type instead of specific text of assert msg
-        # because aserting on the specific text of the assert msg makes this test fairly fragile
-        self.assertEqual(
-            str(context.exception),
-            expected_err_str
+        upload_response = self.client.upload_file(file=file_upload)
+        download_response = self.client.download_file(
+            file_id=upload_response["file_id"]
         )
 
-        try:
-            self.q1.validate_job_type(job_type="sample-qubo")
-        except Exception as exc:  # pylint: disable=broad-exception-caught
-            self.fail(
-                f"validate_job_type failed with exception '{exc}' with supported job_type"
-            )
-
-    def test_build_job_body(self):
-        """Test building of various jobs' request bodies."""
-        with self.assertRaises(ValueError) as context:
-            self.q1.build_job_body(
-                job_type="sample-qubo",
-                job_params={},
-                qubo_file_id="qubo_file_id",
+        if download_response["num_parts"] != num_parts_expected:
+            pytest.fail(
+                f"num_parts {download_response['num_parts']} in downloaded file does "
+                f"not equal {num_parts_expected}"
             )
 
-        self.assertEqual(
-            str(context.exception),
-            "Must define sampler_type in job_params (dirac-1, dirac-2, or dirac-3)."
+        matrix_download = sp.dok_matrix(
+            (
+                download_response["file_config"]["hamiltonian"]["num_variables"],
+                download_response["file_config"]["hamiltonian"]["num_variables"] + 1,
+            ),
+            dtype=dtype,
         )
 
-        constraint_body = self.q1.build_job_body(
-            job_type="sample-constraint",
-            job_params={
-                "sampler_type": "dirac-1",
-                "alpha": 5.0,
-            },
-            objective_file_id="obj_fid",
-            constraints_file_id="cons_fid",
-            job_name="foobar_name",
-            job_tags=["foobar_tag1", "foobar_tag2"],
-        )
+        for datum in download_response["file_config"]["hamiltonian"]["data"]:
+            matrix_download[datum["i"], datum["j"]] = datum["val"]
+
+        if (matrix_download != matrix_upload).nnz != 0:
+            pytest.fail(
+                "sparse matrix in downloaded file does not equal sparse matrix in "
+                "uploaded file"
+            )
 
-        self.assertDictEqual(
-            constraint_body,
-            {
-                "job_submission": {
-                    "job_name": "foobar_name",
-                    "job_tags": ["foobar_tag1", "foobar_tag2"],
-                    "problem_config": {
-                        "quadratic_linearly_constrained_binary_optimization": {
-                            "objective_file_id": "obj_fid",
-                            "constraints_file_id": "cons_fid",
-                            "alpha": 5.0
-                        }
-                    },
-                    "device_config": {
-                        "dirac-1": {}
-                    }
+    def test_upload_download_file_polynomial_multipart(self):
+        """Test uploading and downloading a larger multipart file for square matrix."""
+        num_parts_expected = 2
+        num_variables = 40
+        min_degree = 0
+        max_degree = 3
+        idx_list = list(range(num_variables + 1))  # Include constant index.
+
+        polynomial_upload = []
+
+        for idx in product(idx_list, idx_list, idx_list):
+            # Ensure non-decreasing indices.
+            if idx[0] > idx[1] or idx[1] > idx[2]:
+                continue
+
+            polynomial_upload.append(
+                {
+                    "idx": list(idx),
+                    "val": np.random.uniform(low=-3.14, high=3.14),
                 }
-            }
-        )
+            )
 
-        qubo_body = self.q1.build_job_body(
-            job_type="sample-qubo",
-            job_params={
-                "nsamples": 24,
-                "sampler_type": "dirac-1",
+        file_upload = {
+            "file_name": "multipart-polynomial-upload-download-test",
+            "file_config": {
+                "polynomial": {
+                    "num_variables": num_variables,
+                    "min_degree": min_degree,
+                    "max_degree": max_degree,
+                    "data": polynomial_upload,
+                },
             },
-            qubo_file_id="qubo_fid",
-            job_name="foobar_name",
-        )
+        }
 
-        self.assertDictEqual(
-            qubo_body,
-            {
-                "job_submission": {
-                    "job_name": "foobar_name",
-                    "problem_config": {
-                        "quadratic_unconstrained_binary_optimization": {
-                            "qubo_file_id": "qubo_fid",
-                        }
-                    },
-                    "device_config": {
-                        "dirac-1": {
-                            "num_samples": 24
-                        }
-                    }
-                }
-            }
+        upload_response = self.client.upload_file(file=file_upload)
+        download_response = self.client.download_file(
+            file_id=upload_response["file_id"]
         )
 
-        hamiltonian_body = self.q1.build_job_body(
-            job_type="sample-hamiltonian",
-            job_params={
-                "n_samples": 24,
-                "sampler_type": "dirac-3",
-                "sum_constraint": 200,
-                "solution_precision": 1,
-            },
-            hamiltonian_file_id="hamiltonian_fid",
-            job_tags=["foobar_tag1", "foobar_tag2"],
-        )
+        if download_response["num_parts"] != num_parts_expected:
+            pytest.fail(
+                f"num_parts {download_response['num_parts']} in downloaded file does "
+                f"not equal {num_parts_expected}"
+            )
 
-        self.assertDictEqual(
-            hamiltonian_body,
-            {
-                "job_submission": {
-                    "job_tags": ["foobar_tag1", "foobar_tag2"],
-                    "problem_config": {
-                        "normalized_qudit_hamiltonian_optimization": {
-                            "hamiltonian_file_id": "hamiltonian_fid",
-                        }
-                    },
-                    "device_config": {
-                        "dirac-3": {
-                            "num_samples": 24,
-                            "sum_constraint": 200,
-                            "solution_precision": 1,
-                        }
-                    }
-                }
-            }
-        )
+        polynomial_download = download_response["file_config"]["polynomial"]["data"]
 
-        hamiltonian_body = self.q1.build_job_body(
-            job_type="sample-hamiltonian",
-            job_params={
-                "sampler_type": "dirac-3",
-                "sum_constraint": 200,
-                "solution_precision": 1,
-            },
-            polynomial_file_id="polynomial_fid"
-        )
+        self.assertEqual(len(polynomial_download), len(polynomial_upload))
 
-        self.assertDictEqual(
-            hamiltonian_body,
-            {
-                "job_submission": {
-                    "problem_config": {
-                        "normalized_qudit_hamiltonian_optimization": {
-                            "polynomial_file_id": "polynomial_fid",
-                        }
-                    },
-                    "device_config": {
-                        "dirac-3": {
-                            "sum_constraint": 200,
-                            "solution_precision": 1,
-                        }
-                    }
-                }
-            }
-        )
+        for download_datum, upload_datum in zip(polynomial_download, polynomial_upload):
+            self.assertDictEqual(download_datum, upload_datum)
 
-        hamiltonian_body = self.q1.build_job_body(
-            job_type="sample-hamiltonian",
-            job_params={
-                "sampler_type": "dirac-3",
-                "sum_constraint": 2.4
-            },
-            polynomial_file_id="polynomial_fid"
-        )
+    # Jobs tests, which refer back to some of the above files.
 
-        self.assertDictEqual(
-            hamiltonian_body,
-            {
-                "job_submission": {
-                    "problem_config": {
-                        "normalized_qudit_hamiltonian_optimization": {
-                            "polynomial_file_id": "polynomial_fid",
-                        }
-                    },
-                    "device_config": {
-                        "dirac-3": {
-                            "sum_constraint": 2.4,
-                        }
-                    }
-                }
-            }
-        )
+    def run_end_end(self, job_body: dict):
+        """
+        Utility function for testing end to end pipeline.
+        :param job_body: a validate job request
+        Testing each in series:
+            - submit_job
+            - get_job_status (repeating until job finished)
+            - get_job_results
+            - download_file (compares file_config to results from previous step)
+        """
+
+        job_id = self.client.submit_job(job_body=job_body)
+
+        self.assertIn("job_id", job_id)
+        self.assertIsInstance(job_id["job_id"], str)
+
+        status = qci_client.JobStatus.SUBMITTED
+        while status not in qci_client.JOB_STATUSES_FINAL:
+            status = qci_client.JobStatus(
+                self.client.get_job_status(job_id=job_id["job_id"])["status"]
+            )
+        self.assertEqual(status, qci_client.JobStatus.COMPLETED)
 
-        hamiltonian_body = self.q1.build_job_body(
-            job_type="sample-hamiltonian",
-            job_params={
-                "sampler_type": "dirac-3",
-                "sum_constraint": 2.4,
-                "solution_precision": 0.1,
-            },
-            hamiltonian_file_id="hamiltonian_fid"
-        )
+        response = self.client.get_job_results(job_id=job_id["job_id"])
+        self.assertEqual(self.job_info, set(response.keys()))
 
-        self.assertDictEqual(
-            hamiltonian_body,
-            {
-                "job_submission": {
-                    "problem_config": {
-                        "normalized_qudit_hamiltonian_optimization": {
-                            "hamiltonian_file_id": "hamiltonian_fid",
-                        }
-                    },
-                    "device_config": {
-                        "dirac-3": {
-                            "sum_constraint": 2.4,
-                            "solution_precision": 0.1,
-                        }
-                    }
-                }
-            }
+        result = self.client.download_file(
+            file_id=response["job_info"]["job_result"]["file_id"]
         )
-
-        graph_body = self.q1.build_job_body(
-            job_type="graph-partitioning",
-            job_params={
-                "sampler_type": "dirac-1",
-                "num_samples": 42,
-            },
-            graph_file_id="graph_fid"
+        file_type_expected = (
+            list(job_body["job_submission"]["problem_config"].keys())[0] + "_results"
         )
-
         self.assertDictEqual(
-            graph_body,
-            {
-                "job_submission": {
-                    "problem_config": {
-                        "graph_partitioning": {
-                            "graph_file_id": "graph_fid",
-                        }
-                    },
-                    "device_config": {
-                        "dirac-1": {
-                            "num_samples": 42,
-                        }
-                    }
-                }
-            }
+            response["results"], result["file_config"][file_type_expected]
         )
 
-    def test_print_job_log(self):
-        """Test printing of job log messages."""
-        string_io = io.StringIO()
-        with redirect_stdout(string_io):
-            self.q1.print_job_log(message="fake message")
-        out = string_io.getvalue()
-        date_now = str(datetime.now().strftime("%Y/%m/%d %H:%M:%S"))[0:10]
-        self.assertTrue(out.startswith(f"fake message: {date_now}"))
+    def process_job_check(self, job_body):
+        """Utility function for checking job types."""
+        process_key = ["job_info", "status", "results"]
+        job_output = self.client.process_job(job_body=job_body, wait=True)
+        self.assertTrue(all(key in process_key for key in list(job_output.keys())))
+        job_id = job_output["job_info"]["job_id"]
+        self.assertEqual(job_output, self.client.get_job_results(job_id=job_id))
+
+    def test_large_job(self):
+        """Test large sample-qubo job."""
+        num_variables = 1000
+        large_qubo = sp.random(
+            num_variables, num_variables, density=0.5, format="dok", dtype=np.float32
+        )
+        large_qubo = (large_qubo + large_qubo.T) / 2
+        large_qubo_dict = {
+            "file_name": "test_large_qubo",
+            "file_config": {"qubo": {"data": large_qubo}},
+        }
+        large_file_id = self.client.upload_file(file=large_qubo_dict)["file_id"]
+        print("LARGE FILE ID", large_file_id)
+        large_job_body = {
+            "job_submission": {
+                "job_name": "large_qubo_test_job",
+                "problem_config": {
+                    "quadratic_unconstrained_binary_optimization": {
+                        "qubo_file_id": large_file_id
+                    }
+                },
+                "device_config": {"dirac-1": {}},
+            }
+        }
 
+        self.process_job_check(job_body=large_job_body)
 
-class TestMultipartUpload(unittest.TestCase):
-    """Multipart-file upload test suite."""
+    def test_process_qubo(self):
+        """Test that sample-qubo job process can be checked."""
+        self.process_job_check(job_body=self.qubo_job_body)
 
-    @classmethod
-    def setUpClass(cls):
-        cls.q1 = QciClient()
+    def test_process_constraint(self):
+        """Test that sample-constraint job process can be checked."""
+        self.process_job_check(job_body=self.constraint_job_body)
 
-    # TODO This client no longer uploads results files, only test download.
-    def test_multipart_results_upload_and_download(self):
-        """Test uploading/downloading multipart qubo results file."""
-        # BIG number of samples, each one num_vars in length
-        num_vars = 1700
-        num_samp = 300
-        is_results_file = True
-        samples = np.ones((num_samp, num_vars)).astype(int)
-        counts = np.ones((num_samp, 1)).astype(int)
-        energies = np.ones((num_samp, 1))
-
-        resdata = {
-            "file_name": "test-file.json",
-            "file_type": "job_results_sample_qubo",
-            "organization_id": "5ddf5db3fed87d53b6bf392a",
-            "username": "test_user",
-            "counts": counts.flatten().tolist(),
-            "energies": energies.flatten().tolist(),
-            "samples": samples.tolist(),
-        }
-
-        step_len = compute_results_step_len(resdata["samples"][0])
-        expected_parts = ceil(num_samp / step_len)
-        self.assertGreater(expected_parts, 1)
-
-        #resp = self.q1.upload_file(file=resdata)
-        #meta = self.q1.get_file_metadata(file_id=resp["file_id"], is_results_file=is_results_file)
-        #self.assertEqual(meta["num_parts"], expected_parts)
-
-        #test_res_whole = self.q1.get_file_whole(file_id=resp["file_id"], is_results_file=is_results_file)
-        #self.assertEqual(len(test_res_whole["counts"]), counts.shape[0])
-        #self.assertEqual(len(test_res_whole["energies"]), energies.shape[0])
-        #self.assertEqual(len(test_res_whole["samples"]), samples.shape[0])
-        #self.assertEqual(len(test_res_whole["samples"][0]), samples.shape[1])
-
-        #del_resp = self.q1.delete_file(resp["file_id"])
-        #assert del_resp["num_deleted"] == 1
-
-    # TODO This client no longer uploads results files, only test download.
-    def test_multipart_results_upload_and_download_hamiltonian(self):
-        """Test uploading/downloading multipart hamiltonian results file."""
-        # Tests float uploads, so we use Hamiltonian job type so the API can handle floats
-        num_vars = 20000
-        num_samp = 30
-        samples = np.ones((num_samp, num_vars)).astype(float)
-        counts = np.ones((num_samp, 1)).astype(int)
-        energies = np.ones((num_samp, 1))
-        is_results_file = True
-
-        resdata = {
-            "file_name": "test-file.json",
-            "file_type": "job_results_sample_hamiltonian",
-            "organization_id": "5ddf5db3fed87d53b6bf392a",
-            "username": "test_user",
-            #"solution_type": "continuous",
-            "counts": counts.flatten().tolist(),
-            "energies": energies.flatten().tolist(),
-            "samples": samples.tolist(),
-        }
-
-        step_len = compute_results_step_len(resdata["samples"][0])
-        expected_parts = ceil(num_samp / step_len)
-        self.assertGreater(expected_parts, 1)
-
-        # resp = self.q1.upload_file(file=resdata)
-        #meta = self.q1.get_file_metadata(file_id=resp["file_id"], is_results_file=is_results_file)
-        #self.assertEqual(meta["num_parts"], expected_parts)
-
-        #test_res_whole = self.q1.get_file_whole(file_id=resp["file_id"], is_results_file=is_results_file)
-        #self.assertEqual(len(test_res_whole["counts"]), len(test_vec_int))
-        #self.assertEqual(len(test_res_whole["energies"]), test_vec.shape[0])
-        #self.assertEqual(len(test_res_whole["samples"]), num_samples)
-        #self.assertEqual(len(test_res_whole["samples"][0]), num_nodes)
+    def test_process_hamiltonian_ising_dirac1(self):
+        """Test that sample-hamiltonian-ising process job on dirac-1 can be checked."""
+        self.process_job_check(job_body=self.hamiltonian_job_body_ising_dirac1)
 
-        # del_resp = self.q1.delete_file(resp["file_id"])
-        # assert del_resp["num_deleted"] == 1
+    def test_process_hamiltonian_dirac2(self):
+        """Test that integer sample-hamiltonian process job on dirac-2 can be checked."""
+        self.process_job_check(job_body=self.hamiltonian_job_body_integer_dirac2)
 
-    # TODO This client no longer uploads results files, only test download.
-    def test_multipart_results_upload_and_download_huge(self):
-        """Test uploading/downloading very large multipart qubo results file."""
-        # Now try something too large
-        # BIG number of samples, each one num_vars in length
-        num_vars = 100000
-        num_samp = 300
-        samples = np.ones((num_samp, num_vars)).astype(int)
-        counts = np.ones((num_samp, 1)).astype(int)
-        energies = np.ones((num_samp, 1))
-        is_results_file = True
-
-        resdata = {
-            "file_name": "test-file.json",
-            "file_type": "job_results_sample_qubo",
-            "organization_id": "5ddf5db3fed87d53b6bf392a",
-            "username": "test_user",
-            "counts": counts.flatten().tolist(),
-            "energies": energies.flatten().tolist(),
-            "samples": samples.tolist(),
-        }
-
-        step_len = compute_results_step_len(samples[0])
-        expected_parts = ceil(num_samp / step_len)
-        self.assertGreater(expected_parts, 1)
-
-        # resp = self.q1.upload_file(file=resdata)
-        #meta = self.q1.get_file_metadata(file_id=resp["file_id"], is_results_file=is_results_file)
-        #self.assertEqual(meta["num_parts"], expected_parts)
-
-        #test_res_whole = self.q1.get_file_whole(file_id=resp["file_id"], is_results_file=is_results_file)
-        #self.assertEqual(len(test_res_whole["counts"]), counts.shape[0])
-        #self.assertEqual(len(test_res_whole["energies"]), energies.shape[0])
-        #self.assertEqual(len(test_res_whole["samples"]), samples.shape[0])
-        #self.assertEqual(len(test_res_whole["samples"][0]), samples.shape[1])
-
-
-    # TODO This client no longer uploads results files, only test download.
-    def test_multipart_graph_partitioning_results_upload_and_download(self):
-        """Test uploading/downloading multipart graph-partitioning results file."""
-        num_samples = 10
-        num_nodes = 10000
-        test_vec = np.arange(num_samples)
-        test_vec_int = np.arange(num_samples).astype(int)
-        is_results_file = True
-
-        samples = [
-            [
-                {"id": int(np.random.randint(0, 10)), "class": np.random.randint(0, 3)}
-                for _ in range(num_nodes)
-            ]  # pretend we have a graph with 100 nodes
-            for _ in range(num_samples)  # and we asked for 1000 samples
-        ]
+    def test_process_hamiltonian_dirac3(self):
+        """
+        Test that undistilled sample-hamiltonian process on dirac-3 job can be checked.
+        """
+        self.process_job_check(job_body=self.hamiltonian_job_body_undistilled_dirac3)
 
-        gp_results = {
-            "file_name": "test-file.json",
-            "file_type": "job_results_graph_partitioning",
-            "organization_id": "5ddf5db3fed87d53b6bf392a",
-            "username": "test_user",
-            "balance": test_vec.tolist(),
-            "counts": test_vec.tolist(),
-            "cut_size": test_vec_int.tolist(),
-            "energies": test_vec.tolist(),
-            "is_feasible": [True] * num_samples,
-            "samples": samples,
-        }
-
-        step_len = compute_results_step_len(samples[0])
-        expected_parts = ceil(num_samples / step_len)
-        self.assertGreater(expected_parts, 1)
+    def test_graph_partitioning(self):
+        """Test graph-partitioning job."""
+        self.run_end_end(job_body=self.graph_job_body)
 
-        # resp = self.q1.upload_file(file=gp_results)
+    def test_sample_qubo(self):
+        """Test sample-qubo job."""
+        self.run_end_end(job_body=self.qubo_job_body)
 
-        #meta = self.q1.get_file_metadata(file_id=resp["file_id"], is_results_file=is_results_file)
-        #self.assertEqual(meta["num_parts"], expected_parts)
+    def test_sample_constraint(self):
+        """Test sample-constraint job."""
+        self.run_end_end(job_body=self.constraint_job_body)
 
-        #del_resp = self.q1.delete_file(resp["file_id"])
-        #assert del_resp["num_deleted"] == 1
+    def test_sample_hamiltonian_ising_polynomial_dirac1(self):
+        """Test sample-hamiltonian-ising job using polynomial on dirac-1."""
+        self.run_end_end(job_body=self.polynomial_job_body_ising_dirac1)
 
+    def test_sample_hamiltonian_ising_hamiltonian_dirac1(self):
+        """Test sample-hamiltonian-ising job using hamiltonian matrix on dirac-1."""
+        self.run_end_end(job_body=self.hamiltonian_job_body_ising_dirac1)
 
-@pytest.mark.offline
-class TestJobsApiWithRequestMocks(unittest.TestCase):
-    """Jobs-API-related test suite that can be run without backend."""
+    def test_sample_hamiltonian_polynomial_continuous_dirac2(self):
+        """Test sample-hamiltonian continuous job using polynomial on dirac-2."""
+        self.run_end_end(
+            job_body=self.polynomial_job_body_hamiltonian_continuous_dirac2
+        )
 
-    def setUp(self):
-        with pytest.MonkeyPatch().context() as mp:
-            mp.setenv('QCI_TOKEN', 'test_api_token')
-            mp.setenv('QCI_API_URL', 'test_url')
-            self.qci_client = QciClient(set_bearer_token_on_init=False)
-        self.job_id = "63b717a22da68618ec444eac"
-        self.job_type = "sample-hamiltonian"
-        self.file_id = "73b717a22da68618ec444eab"
+    def test_sample_hamiltonian_polynomial_integer_dirac2(self):
+        """Test sample-hamiltonian integer job using polynomial on dirac-2."""
+        self.run_end_end(job_body=self.polynomial_job_body_hamiltonian_integer_dirac2)
 
-        # Bad GET jobs response.
-        self.get_response_bad = requests.Response()
-        self.get_response_bad.status_code = 404
+    def test_sample_hamiltonian_continuous_dirac2(self):
+        """Test continuous sample-hamiltonian job on dirac-2."""
+        self.run_end_end(job_body=self.hamiltonian_job_body_continous_dirac2)
 
-    def test_jobs_url(self) -> None:
-        """Test getting jobs URL."""
-        self.assertEqual(self.qci_client.jobs_url, "test_url/optimization/v1/jobs")
+    def test_sample_hamiltonian_integer_dirac2(self):
+        """Test integer sample-hamiltonian job on dirac-2."""
+        self.run_end_end(job_body=self.hamiltonian_job_body_integer_dirac2)
 
-    def test_get_job_id_url(self) -> None:
-        """Test getting jobs URL for given job ID."""
-        self.assertEqual(
-            self.qci_client.get_job_id_url(self.job_id), f"test_url/optimization/v1/jobs/{self.job_id}"
+    def test_sample_hamiltonian_polynomial_distilled_continuous_dirac3(self):
+        """
+        Test distilled-to-continuous sample-hamiltonian job using polynomial on dirac-3.
+        """
+        self.run_end_end(
+            job_body=self.polynomial_min_degree_2_max_degree_4_job_body_distilled_continuous_dirac3
         )
 
-    def test_get_job_status_url(self) -> None:
-        """Test getting jobs-status URL for given job ID."""
-        self.assertEqual(
-            self.qci_client.get_job_status_url(self.job_id),
-            f"test_url/optimization/v1/jobs/{self.job_id}/status",
-        )
+    def test_sample_hamiltonian_undistilled_dirac3(self):
+        """Test undistilled sample-hamiltonian job on dirac-3."""
+        self.run_end_end(job_body=self.hamiltonian_job_body_undistilled_dirac3)
 
-    def test_files_url(self) -> None:
-        """Test getting files URL."""
-        self.assertEqual(self.qci_client.files_url, "test_url/optimization/v1/files")
+    def test_sample_hamiltonian_distilled_continuous_dirac3(self):
+        """Test distilled-to-continuous sample-hamiltonian job on dirac-3."""
+        self.run_end_end(job_body=self.hamiltonian_job_body_distilled_continuous_dirac3)
 
-    def test_get_file_id_url(self) -> None:
-        """Test getting files URL for given file ID."""
-        self.assertEqual(
-            self.qci_client.get_file_id_url(self.file_id),
-            f"test_url/optimization/v1/files/{self.file_id}",
-        )
+    def test_sample_hamiltonian_distilled_integer_dirac3(self):
+        """Test distilled-to-integer sample-hamiltonian job on dirac-3."""
+        self.run_end_end(job_body=self.hamiltonian_job_body_distilled_integer_dirac3)
 
-    def test_get_job_type_from_job_id(self) -> None:
-        """Test getting job type from job ID."""
-        # GET short jobs response.
-        get_jobs_response_short = requests.Response()
-        get_jobs_response_short.status_code = 200
-        get_jobs_response_short._content = (  # pylint: disable=protected-access
-            b"""{
-    "job_id": "%b",
-    "status": "COMPLETED",
-    "type": "sample_hamiltonian",
-    "organization_id": "6edf5db3def87d53b6bf375b",
-    "username": "test_user"
-}"""
-            % self.job_id.encode()
-        )
 
-        self.qci_client.session.request = unittest.mock.MagicMock(
-            return_value=get_jobs_response_short
-        )
-        self.assertEqual(
-            self.qci_client.get_job_type_from_job_id(self.job_id), self.job_type
-        )
+class TestMultipartUploadDownload(unittest.TestCase):
+    """Multipart-file upload/download test suite."""
 
-        self.qci_client.session.request = unittest.mock.MagicMock(
-            return_value=self.get_response_bad
-        )
-        with self.assertRaises(requests.HTTPError):
-            self.qci_client.get_job_type_from_job_id(self.job_id)
+    @classmethod
+    def setUpClass(cls):
+        cls.client = qci_client.QciClient()
+
+    def test_multipart_upload_download_hamiltonian(self):
+        """Test uploading/downloading multipart hamiltonian matrix file."""
+        # num_variables = 1700
+
+        # resdata = {
+        #     "file_name": "test-file.json",
+        #     "file_type": "job_results_sample_qubo",
+        #     "organization_id": "5ddf5db3fed87d53b6bf392a",
+        #     "username": "test_user",
+        #     "counts": counts.flatten().tolist(),
+        #     "energies": energies.flatten().tolist(),
+        #     "samples": samples.tolist(),
+        # }
+
+        # resp = self.client.upload_file(file=resdata)
+        # meta = self.client.get_file_metadata(file_id=resp["file_id"], is_results_file=is_results_file)
+        # self.assertEqual(meta["num_parts"], expected_parts)
+
+        # test_res_whole = self.client.get_file_whole(file_id=resp["file_id"], is_results_file=is_results_file)
+        # self.assertEqual(len(test_res_whole["counts"]), counts.shape[0])
+        # self.assertEqual(len(test_res_whole["energies"]), energies.shape[0])
+        # self.assertEqual(len(test_res_whole["samples"]), samples.shape[0])
+        # self.assertEqual(len(test_res_whole["samples"][0]), samples.shape[1])
+
+        # del_resp = self.client.delete_file(resp["file_id"])
+        # assert del_resp["num_deleted"] == 1
+
+    def test_multipart_upload_download_polynomial(self):
+        """Test uploading/downloading multipart polynomial file."""
+        # Tests float uploads, so we use Hamiltonian job type so the API can handle floats
+        # num_variables = 20000
+
+        # resdata = {
+        #     "file_name": "test-file.json",
+        #     "file_type": "job_results_sample_hamiltonian",
+        #     "organization_id": "5ddf5db3fed87d53b6bf392a",
+        #     "username": "test_user",
+        #     # "solution_type": "continuous",
+        #     "counts": counts.flatten().tolist(),
+        #     "energies": energies.flatten().tolist(),
+        #     "samples": samples.tolist(),
+        # }
+
+        # resp = self.client.upload_file(file=resdata)
+        # meta = self.client.get_file_metadata(file_id=resp["file_id"], is_results_file=is_results_file)
+        # self.assertEqual(meta["num_parts"], expected_parts)
+
+        # test_res_whole = self.client.get_file_whole(file_id=resp["file_id"], is_results_file=is_results_file)
+        # self.assertEqual(len(test_res_whole["counts"]), len(test_vec_int))
+        # self.assertEqual(len(test_res_whole["energies"]), test_vec.shape[0])
+        # self.assertEqual(len(test_res_whole["samples"]), num_samples)
+        # self.assertEqual(len(test_res_whole["samples"][0]), num_nodes)
+
+        # del_resp = self.client.delete_file(resp["file_id"])
+        # assert del_resp["num_deleted"] == 1
```

