# Comparing `tmp/rucio_jupyterlab-0.9.7.tar.gz` & `tmp/rucio_jupyterlab-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rucio_jupyterlab-0.9.7.tar", last modified: Mon May 23 11:20:56 2022, max compression
+gzip compressed data, was "rucio_jupyterlab-0.9.8.tar", last modified: Tue Oct 11 09:37:24 2022, max compression
```

## Comparing `rucio_jupyterlab-0.9.7.tar` & `rucio_jupyterlab-0.9.8.tar`

### file list

```diff
@@ -1,160 +1,160 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:20:56.815160 rucio_jupyterlab-0.9.7/
--rw-r--r--   0 runner    (1001) docker     (121)     1013 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/.eslintrc.js
--rw-r--r--   0 runner    (1001) docker     (121)      260 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (121)     8670 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/CONFIGURATION.md
--rw-r--r--   0 runner    (1001) docker     (121)     2124 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)    11356 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      698 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4524 2022-05-23 11:20:56.815160 rucio_jupyterlab-0.9.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3683 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1140 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/RELEASE.md
--rw-r--r--   0 runner    (1001) docker     (121)      193 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/install.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:20:56.791159 rucio_jupyterlab-0.9.7/jupyter-config/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:20:56.799159 rucio_jupyterlab-0.9.7/jupyter-config/jupyter_notebook_config.d/
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/jupyter-config/jupyter_notebook_config.d/rucio_jupyterlab.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:20:56.799159 rucio_jupyterlab-0.9.7/jupyter-config/jupyter_server_config.d/
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/jupyter-config/jupyter_server_config.d/rucio_jupyterlab.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:20:56.799159 rucio_jupyterlab-0.9.7/jupyter-config/nb-config/
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/jupyter-config/nb-config/rucio_jupyterlab.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:20:56.799159 rucio_jupyterlab-0.9.7/jupyter-config/server-config/
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/jupyter-config/server-config/rucio_jupyterlab.json
--rw-r--r--   0 runner    (1001) docker     (121)     3516 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/package.json
--rw-r--r--   0 runner    (1001) docker     (121)      599 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:20:56.799159 rucio_jupyterlab-0.9.7/rucio_jupyterlab/
--rw-r--r--   0 runner    (1001) docker     (121)      409 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:20:56.799159 rucio_jupyterlab-0.9.7/rucio_jupyterlab/config/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4138 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/config/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     2981 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/config/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     6195 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/db.py
--rw-r--r--   0 runner    (1001) docker     (121)      680 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/entity.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:20:56.803159 rucio_jupyterlab-0.9.7/rucio_jupyterlab/handlers/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1704 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/handlers/auth_config.py
--rw-r--r--   0 runner    (1001) docker     (121)      908 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2051 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/handlers/did_browser.py
--rw-r--r--   0 runner    (1001) docker     (121)     1654 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/handlers/did_details.py
--rw-r--r--   0 runner    (1001) docker     (121)     1471 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/handlers/did_make_available.py
--rw-r--r--   0 runner    (1001) docker     (121)     2317 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/handlers/did_search.py
--rw-r--r--   0 runner    (1001) docker     (121)     1596 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/handlers/file_browser.py
--rw-r--r--   0 runner    (1001) docker     (121)     3152 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/handlers/handlers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1777 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/handlers/instances.py
--rw-r--r--   0 runner    (1001) docker     (121)     1036 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/handlers/list_rses.py
--rw-r--r--   0 runner    (1001) docker     (121)      935 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/handlers/list_scopes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1557 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/handlers/oidc_auth_check.py
--rw-r--r--   0 runner    (1001) docker     (121)    11136 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/handlers/open_replication_rule.py
--rw-r--r--   0 runner    (1001) docker     (121)      671 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/handlers/purge_cache.py
--rw-r--r--   0 runner    (1001) docker     (121)     1877 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/handlers/upload.py
--rw-r--r--   0 runner    (1001) docker     (121)      858 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/handlers/upload_jobs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1286 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/handlers/upload_jobs_details.py
--rw-r--r--   0 runner    (1001) docker     (121)     1037 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/handlers/upload_jobs_log.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:20:56.803159 rucio_jupyterlab-0.9.7/rucio_jupyterlab/kernels/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/kernels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:20:56.803159 rucio_jupyterlab-0.9.7/rucio_jupyterlab/kernels/ipython/
--rw-r--r--   0 runner    (1001) docker     (121)     2823 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/kernels/ipython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2049 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/kernels/ipython/types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:20:56.803159 rucio_jupyterlab-0.9.7/rucio_jupyterlab/labextension/
--rw-r--r--   0 runner    (1001) docker     (121)     3659 2022-05-23 11:16:38.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:20:56.807159 rucio_jupyterlab-0.9.7/rucio_jupyterlab/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (121)     4419 2022-05-23 11:16:38.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/labextension/static/130.7365b614084ad0cbc49d.js
--rw-r--r--   0 runner    (1001) docker     (121)    34990 2022-05-23 11:16:38.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/labextension/static/20.53c11c5b79a94ee424cb.js
--rw-r--r--   0 runner    (1001) docker     (121)     7400 2022-05-23 11:16:38.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/labextension/static/392.c6f78101fd8442eea43d.js
--rw-r--r--   0 runner    (1001) docker     (121)     1161 2022-05-23 11:16:38.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/labextension/static/429.407b01bdf4a8a104bc25.js
--rw-r--r--   0 runner    (1001) docker     (121)    96293 2022-05-23 11:16:38.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/labextension/static/437.e8e22924cb4070990f2f.js
--rw-r--r--   0 runner    (1001) docker     (121)    59978 2022-05-23 11:16:38.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/labextension/static/448.47f3f7fec352ce0129f5.js
--rw-r--r--   0 runner    (1001) docker     (121)      412 2022-05-23 11:16:38.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/labextension/static/448.47f3f7fec352ce0129f5.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5479 2022-05-23 11:16:38.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/labextension/static/594.bb16e01fd6647f801c63.js
--rw-r--r--   0 runner    (1001) docker     (121)    28168 2022-05-23 11:16:38.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/labextension/static/608.9fe7f346a912ad2fd318.js
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-05-23 11:16:38.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/labextension/static/608.9fe7f346a912ad2fd318.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)    25126 2022-05-23 11:16:38.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/labextension/static/61.3ba6ce361770a986be36.js
--rw-r--r--   0 runner    (1001) docker     (121)     7400 2022-05-23 11:16:38.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/labextension/static/728.5c0c1b3668a79b1563d4.js
--rw-r--r--   0 runner    (1001) docker     (121)     5479 2022-05-23 11:16:38.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/labextension/static/855.fd11e9ed650c9ff9d8e6.js
--rw-r--r--   0 runner    (1001) docker     (121)    92253 2022-05-23 11:16:38.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/labextension/static/937.d7571d64b2695fcc8cb8.js
--rw-r--r--   0 runner    (1001) docker     (121)     9569 2022-05-23 11:16:38.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/labextension/static/remoteEntry.13b02eee40e64df104ad.js
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-05-23 11:16:29.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (121)    69860 2022-05-23 11:16:38.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/labextension/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:20:56.807159 rucio_jupyterlab-0.9.7/rucio_jupyterlab/mode_handlers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/mode_handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4021 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/mode_handlers/download.py
--rw-r--r--   0 runner    (1001) docker     (121)     6987 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/mode_handlers/replica.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:20:56.807159 rucio_jupyterlab-0.9.7/rucio_jupyterlab/rucio/
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/rucio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2909 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/rucio/authenticators.py
--rw-r--r--   0 runner    (1001) docker     (121)     7057 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/rucio/client_environment.py
--rw-r--r--   0 runner    (1001) docker     (121)     3418 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/rucio/download.py
--rw-r--r--   0 runner    (1001) docker     (121)     9326 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/rucio/rucio.py
--rw-r--r--   0 runner    (1001) docker     (121)     4628 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/rucio/upload.py
--rw-r--r--   0 runner    (1001) docker     (121)      813 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/rucio/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      846 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/server.py
--rw-r--r--   0 runner    (1001) docker     (121)      919 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:20:56.799159 rucio_jupyterlab-0.9.7/rucio_jupyterlab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4524 2022-05-23 11:20:56.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4894 2022-05-23 11:20:56.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-23 11:20:56.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-23 11:17:38.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-05-23 11:20:56.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-05-23 11:20:56.000000 rucio_jupyterlab-0.9.7/rucio_jupyterlab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-23 11:20:56.815160 rucio_jupyterlab-0.9.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3654 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:20:56.807159 rucio_jupyterlab-0.9.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:20:56.807159 rucio_jupyterlab-0.9.7/src/commands/
--rw-r--r--   0 runner    (1001) docker     (121)     1335 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/src/commands/uploadFile.ts
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:20:56.811159 rucio_jupyterlab-0.9.7/src/components/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:20:56.811159 rucio_jupyterlab-0.9.7/src/components/@Explore/
--rw-r--r--   0 runner    (1001) docker     (121)     5470 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/src/components/@Explore/AddToNotebookPopover.tsx
--rw-r--r--   0 runner    (1001) docker     (121)     9402 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/src/components/@Explore/CollectionDIDItemDetails.tsx
--rw-r--r--   0 runner    (1001) docker     (121)     3493 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/src/components/@Explore/DIDListItem.tsx
--rw-r--r--   0 runner    (1001) docker     (121)     7718 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/src/components/@Explore/ExploreTab.tsx
--rw-r--r--   0 runner    (1001) docker     (121)     7704 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/src/components/@Explore/FileDIDItemDetails.tsx
--rw-r--r--   0 runner    (1001) docker     (121)     3075 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/src/components/@Explore/InlineDropdown.tsx
--rw-r--r--   0 runner    (1001) docker     (121)     5749 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/src/components/@Explore/ListAttachedFilesPopover.tsx
--rw-r--r--   0 runner    (1001) docker     (121)     5519 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/src/components/@Explore/ListScopesPopover.tsx
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:20:56.811159 rucio_jupyterlab-0.9.7/src/components/@Notebook/
--rw-r--r--   0 runner    (1001) docker     (121)     7366 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/src/components/@Notebook/NotebookAttachmentListItem.tsx
--rw-r--r--   0 runner    (1001) docker     (121)     2390 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/src/components/@Notebook/NotebookTab.tsx
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:20:56.811159 rucio_jupyterlab-0.9.7/src/components/@Settings/
--rw-r--r--   0 runner    (1001) docker     (121)     6730 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/src/components/@Settings/FilePickerPopover.tsx
--rw-r--r--   0 runner    (1001) docker     (121)    13018 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/src/components/@Settings/SettingsTab.tsx
--rw-r--r--   0 runner    (1001) docker     (121)     3296 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/src/components/@Settings/UserPassAuth.tsx
--rw-r--r--   0 runner    (1001) docker     (121)     4003 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/src/components/@Settings/X509Auth.tsx
--rw-r--r--   0 runner    (1001) docker     (121)     3245 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/src/components/@Settings/X509ProxyAuth.tsx
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:20:56.811159 rucio_jupyterlab-0.9.7/src/components/@Uploads/
--rw-r--r--   0 runner    (1001) docker     (121)     4099 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/src/components/@Uploads/UploadJobListItem.tsx
--rw-r--r--   0 runner    (1001) docker     (121)     2443 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/src/components/@Uploads/UploadsTab.tsx
--rw-r--r--   0 runner    (1001) docker     (121)      932 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/src/components/Alert.tsx
--rw-r--r--   0 runner    (1001) docker     (121)     2332 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/src/components/Button.tsx
--rw-r--r--   0 runner    (1001) docker     (121)      789 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/src/components/Header.tsx
--rw-r--r--   0 runner    (1001) docker     (121)      927 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/src/components/HorizontalHeading.tsx
--rw-r--r--   0 runner    (1001) docker     (121)     2198 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/src/components/MenuBar.tsx
--rw-r--r--   0 runner    (1001) docker     (121)     7150 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/src/components/RucioLogo.tsx
--rw-r--r--   0 runner    (1001) docker     (121)      958 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/src/components/Spinning.tsx
--rw-r--r--   0 runner    (1001) docker     (121)     1765 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/src/components/TextField.tsx
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/src/const.ts
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:20:56.811159 rucio_jupyterlab-0.9.7/src/icons/
--rw-r--r--   0 runner    (1001) docker     (121)     5011 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/src/icons/RucioIcon.tsx
--rw-r--r--   0 runner    (1001) docker     (121)     3314 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/src/index.ts
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:20:56.815160 rucio_jupyterlab-0.9.7/src/stores/
--rw-r--r--   0 runner    (1001) docker     (121)      735 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/src/stores/ExtensionStore.ts
--rw-r--r--   0 runner    (1001) docker     (121)     1043 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/src/stores/UIStore.ts
--rw-r--r--   0 runner    (1001) docker     (121)     2496 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/src/types.ts
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:20:56.815160 rucio_jupyterlab-0.9.7/src/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     6705 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/src/utils/Actions.tsx
--rw-r--r--   0 runner    (1001) docker     (121)     4099 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/src/utils/ActiveNotebookListener.ts
--rw-r--r--   0 runner    (1001) docker     (121)     1447 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/src/utils/ApiRequest.ts
--rw-r--r--   0 runner    (1001) docker     (121)     2995 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/src/utils/DIDPollingManager.tsx
--rw-r--r--   0 runner    (1001) docker     (121)     2023 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/src/utils/Helpers.ts
--rw-r--r--   0 runner    (1001) docker     (121)    13071 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/src/utils/NotebookListener.ts
--rw-r--r--   0 runner    (1001) docker     (121)     5485 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/src/utils/NotebookPollingListener.ts
--rw-r--r--   0 runner    (1001) docker     (121)      603 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/src/utils/useInterval.ts
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:20:56.815160 rucio_jupyterlab-0.9.7/src/widgets/
--rw-r--r--   0 runner    (1001) docker     (121)     4774 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/src/widgets/InjectNotebookToolbar.tsx
--rw-r--r--   0 runner    (1001) docker     (121)     9392 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/src/widgets/RucioUploadDialog.tsx
--rw-r--r--   0 runner    (1001) docker     (121)     5047 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/src/widgets/SidebarPanel.tsx
--rw-r--r--   0 runner    (1001) docker     (121)     1875 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/src/widgets/UploadLogViewerWidget.tsx
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:20:56.815160 rucio_jupyterlab-0.9.7/style/
--rw-r--r--   0 runner    (1001) docker     (121)      989 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/style/index.css
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/style/index.js
--rw-r--r--   0 runner    (1001) docker     (121)      549 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/tsconfig.json
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/webpack.config.js
--rw-r--r--   0 runner    (1001) docker     (121)   391483 2022-05-23 11:15:07.000000 rucio_jupyterlab-0.9.7/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 09:37:24.670516 rucio_jupyterlab-0.9.8/
+-rw-r--r--   0 runner    (1001) docker     (121)     1013 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/.eslintrc.js
+-rw-r--r--   0 runner    (1001) docker     (121)      260 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (121)     8670 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/CONFIGURATION.md
+-rw-r--r--   0 runner    (1001) docker     (121)     2124 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (121)    11356 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      698 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     4524 2022-10-11 09:37:24.670516 rucio_jupyterlab-0.9.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3683 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1140 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/RELEASE.md
+-rw-r--r--   0 runner    (1001) docker     (121)      193 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/install.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 09:37:24.654515 rucio_jupyterlab-0.9.8/jupyter-config/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 09:37:24.658515 rucio_jupyterlab-0.9.8/jupyter-config/jupyter_notebook_config.d/
+-rw-r--r--   0 runner    (1001) docker     (121)      100 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/jupyter-config/jupyter_notebook_config.d/rucio_jupyterlab.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 09:37:24.658515 rucio_jupyterlab-0.9.8/jupyter-config/jupyter_server_config.d/
+-rw-r--r--   0 runner    (1001) docker     (121)       98 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/jupyter-config/jupyter_server_config.d/rucio_jupyterlab.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 09:37:24.658515 rucio_jupyterlab-0.9.8/jupyter-config/nb-config/
+-rw-r--r--   0 runner    (1001) docker     (121)      100 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/jupyter-config/nb-config/rucio_jupyterlab.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 09:37:24.658515 rucio_jupyterlab-0.9.8/jupyter-config/server-config/
+-rw-r--r--   0 runner    (1001) docker     (121)       98 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/jupyter-config/server-config/rucio_jupyterlab.json
+-rw-r--r--   0 runner    (1001) docker     (121)     3517 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/package.json
+-rw-r--r--   0 runner    (1001) docker     (121)      599 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 09:37:24.658515 rucio_jupyterlab-0.9.8/rucio_jupyterlab/
+-rw-r--r--   0 runner    (1001) docker     (121)      409 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       72 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 09:37:24.658515 rucio_jupyterlab-0.9.8/rucio_jupyterlab/config/
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4138 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2981 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/config/schema.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6195 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/db.py
+-rw-r--r--   0 runner    (1001) docker     (121)      680 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/entity.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 09:37:24.662515 rucio_jupyterlab-0.9.8/rucio_jupyterlab/handlers/
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1704 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/handlers/auth_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)      908 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2051 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/handlers/did_browser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1654 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/handlers/did_details.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1471 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/handlers/did_make_available.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2317 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/handlers/did_search.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1596 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/handlers/file_browser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3152 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/handlers/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1777 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/handlers/instances.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1036 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/handlers/list_rses.py
+-rw-r--r--   0 runner    (1001) docker     (121)      935 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/handlers/list_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1557 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/handlers/oidc_auth_check.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11136 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/handlers/open_replication_rule.py
+-rw-r--r--   0 runner    (1001) docker     (121)      671 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/handlers/purge_cache.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1877 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/handlers/upload.py
+-rw-r--r--   0 runner    (1001) docker     (121)      858 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/handlers/upload_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1286 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/handlers/upload_jobs_details.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1037 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/handlers/upload_jobs_log.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 09:37:24.662515 rucio_jupyterlab-0.9.8/rucio_jupyterlab/kernels/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/kernels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 09:37:24.662515 rucio_jupyterlab-0.9.8/rucio_jupyterlab/kernels/ipython/
+-rw-r--r--   0 runner    (1001) docker     (121)     2823 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/kernels/ipython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2049 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/kernels/ipython/types.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 09:37:24.662515 rucio_jupyterlab-0.9.8/rucio_jupyterlab/labextension/
+-rw-r--r--   0 runner    (1001) docker     (121)     3659 2022-10-11 09:34:04.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 09:37:24.662515 rucio_jupyterlab-0.9.8/rucio_jupyterlab/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4419 2022-10-11 09:34:04.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/labextension/static/130.7365b614084ad0cbc49d.js
+-rw-r--r--   0 runner    (1001) docker     (121)    88672 2022-10-11 09:34:04.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/labextension/static/162.f78f93f2c02451004fb9.js
+-rw-r--r--   0 runner    (1001) docker     (121)    34990 2022-10-11 09:34:04.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/labextension/static/20.53c11c5b79a94ee424cb.js
+-rw-r--r--   0 runner    (1001) docker     (121)     7400 2022-10-11 09:34:04.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/labextension/static/392.c6f78101fd8442eea43d.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1161 2022-10-11 09:34:04.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/labextension/static/429.407b01bdf4a8a104bc25.js
+-rw-r--r--   0 runner    (1001) docker     (121)    59978 2022-10-11 09:34:04.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/labextension/static/448.47f3f7fec352ce0129f5.js
+-rw-r--r--   0 runner    (1001) docker     (121)      412 2022-10-11 09:34:04.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/labextension/static/448.47f3f7fec352ce0129f5.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5479 2022-10-11 09:34:04.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/labextension/static/594.bb16e01fd6647f801c63.js
+-rw-r--r--   0 runner    (1001) docker     (121)    28168 2022-10-11 09:34:04.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/labextension/static/608.9fe7f346a912ad2fd318.js
+-rw-r--r--   0 runner    (1001) docker     (121)      192 2022-10-11 09:34:04.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/labextension/static/608.9fe7f346a912ad2fd318.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    25126 2022-10-11 09:34:04.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/labextension/static/61.3ba6ce361770a986be36.js
+-rw-r--r--   0 runner    (1001) docker     (121)     7400 2022-10-11 09:34:04.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/labextension/static/728.5c0c1b3668a79b1563d4.js
+-rw-r--r--   0 runner    (1001) docker     (121)     5479 2022-10-11 09:34:04.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/labextension/static/855.fd11e9ed650c9ff9d8e6.js
+-rw-r--r--   0 runner    (1001) docker     (121)    92253 2022-10-11 09:34:04.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/labextension/static/937.d7571d64b2695fcc8cb8.js
+-rw-r--r--   0 runner    (1001) docker     (121)     9571 2022-10-11 09:34:04.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/labextension/static/remoteEntry.ce6881670499ee5dfee1.js
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-10-11 09:33:58.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (121)    69860 2022-10-11 09:34:04.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/labextension/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 09:37:24.662515 rucio_jupyterlab-0.9.8/rucio_jupyterlab/mode_handlers/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/mode_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4021 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/mode_handlers/download.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6987 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/mode_handlers/replica.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 09:37:24.662515 rucio_jupyterlab-0.9.8/rucio_jupyterlab/rucio/
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/rucio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2909 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/rucio/authenticators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7057 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/rucio/client_environment.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3418 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/rucio/download.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9326 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/rucio/rucio.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4628 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/rucio/upload.py
+-rw-r--r--   0 runner    (1001) docker     (121)      813 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/rucio/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      846 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/server.py
+-rw-r--r--   0 runner    (1001) docker     (121)      919 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 09:37:24.658515 rucio_jupyterlab-0.9.8/rucio_jupyterlab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4524 2022-10-11 09:37:24.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4894 2022-10-11 09:37:24.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-11 09:37:24.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-11 09:34:52.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      115 2022-10-11 09:37:24.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-10-11 09:37:24.000000 rucio_jupyterlab-0.9.8/rucio_jupyterlab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-11 09:37:24.670516 rucio_jupyterlab-0.9.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     3654 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 09:37:24.666516 rucio_jupyterlab-0.9.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 09:37:24.666516 rucio_jupyterlab-0.9.8/src/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)     1335 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/src/commands/uploadFile.ts
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 09:37:24.666516 rucio_jupyterlab-0.9.8/src/components/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 09:37:24.666516 rucio_jupyterlab-0.9.8/src/components/@Explore/
+-rw-r--r--   0 runner    (1001) docker     (121)     5470 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/src/components/@Explore/AddToNotebookPopover.tsx
+-rw-r--r--   0 runner    (1001) docker     (121)     9402 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/src/components/@Explore/CollectionDIDItemDetails.tsx
+-rw-r--r--   0 runner    (1001) docker     (121)     3493 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/src/components/@Explore/DIDListItem.tsx
+-rw-r--r--   0 runner    (1001) docker     (121)     7718 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/src/components/@Explore/ExploreTab.tsx
+-rw-r--r--   0 runner    (1001) docker     (121)     7704 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/src/components/@Explore/FileDIDItemDetails.tsx
+-rw-r--r--   0 runner    (1001) docker     (121)     3075 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/src/components/@Explore/InlineDropdown.tsx
+-rw-r--r--   0 runner    (1001) docker     (121)     5749 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/src/components/@Explore/ListAttachedFilesPopover.tsx
+-rw-r--r--   0 runner    (1001) docker     (121)     5519 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/src/components/@Explore/ListScopesPopover.tsx
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 09:37:24.666516 rucio_jupyterlab-0.9.8/src/components/@Notebook/
+-rw-r--r--   0 runner    (1001) docker     (121)     7366 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/src/components/@Notebook/NotebookAttachmentListItem.tsx
+-rw-r--r--   0 runner    (1001) docker     (121)     2390 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/src/components/@Notebook/NotebookTab.tsx
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 09:37:24.666516 rucio_jupyterlab-0.9.8/src/components/@Settings/
+-rw-r--r--   0 runner    (1001) docker     (121)     6730 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/src/components/@Settings/FilePickerPopover.tsx
+-rw-r--r--   0 runner    (1001) docker     (121)    13018 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/src/components/@Settings/SettingsTab.tsx
+-rw-r--r--   0 runner    (1001) docker     (121)     3296 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/src/components/@Settings/UserPassAuth.tsx
+-rw-r--r--   0 runner    (1001) docker     (121)     4003 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/src/components/@Settings/X509Auth.tsx
+-rw-r--r--   0 runner    (1001) docker     (121)     3245 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/src/components/@Settings/X509ProxyAuth.tsx
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 09:37:24.666516 rucio_jupyterlab-0.9.8/src/components/@Uploads/
+-rw-r--r--   0 runner    (1001) docker     (121)     4099 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/src/components/@Uploads/UploadJobListItem.tsx
+-rw-r--r--   0 runner    (1001) docker     (121)     2443 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/src/components/@Uploads/UploadsTab.tsx
+-rw-r--r--   0 runner    (1001) docker     (121)      932 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/src/components/Alert.tsx
+-rw-r--r--   0 runner    (1001) docker     (121)     2332 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/src/components/Button.tsx
+-rw-r--r--   0 runner    (1001) docker     (121)      789 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/src/components/Header.tsx
+-rw-r--r--   0 runner    (1001) docker     (121)      927 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/src/components/HorizontalHeading.tsx
+-rw-r--r--   0 runner    (1001) docker     (121)     2198 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/src/components/MenuBar.tsx
+-rw-r--r--   0 runner    (1001) docker     (121)     7150 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/src/components/RucioLogo.tsx
+-rw-r--r--   0 runner    (1001) docker     (121)      958 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/src/components/Spinning.tsx
+-rw-r--r--   0 runner    (1001) docker     (121)     1765 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/src/components/TextField.tsx
+-rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/src/const.ts
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 09:37:24.666516 rucio_jupyterlab-0.9.8/src/icons/
+-rw-r--r--   0 runner    (1001) docker     (121)     5011 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/src/icons/RucioIcon.tsx
+-rw-r--r--   0 runner    (1001) docker     (121)     3323 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/src/index.ts
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 09:37:24.666516 rucio_jupyterlab-0.9.8/src/stores/
+-rw-r--r--   0 runner    (1001) docker     (121)      735 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/src/stores/ExtensionStore.ts
+-rw-r--r--   0 runner    (1001) docker     (121)     1043 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/src/stores/UIStore.ts
+-rw-r--r--   0 runner    (1001) docker     (121)     2496 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/src/types.ts
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 09:37:24.666516 rucio_jupyterlab-0.9.8/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)     6705 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/src/utils/Actions.tsx
+-rw-r--r--   0 runner    (1001) docker     (121)     4099 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/src/utils/ActiveNotebookListener.ts
+-rw-r--r--   0 runner    (1001) docker     (121)     1447 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/src/utils/ApiRequest.ts
+-rw-r--r--   0 runner    (1001) docker     (121)     2995 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/src/utils/DIDPollingManager.tsx
+-rw-r--r--   0 runner    (1001) docker     (121)     2023 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/src/utils/Helpers.ts
+-rw-r--r--   0 runner    (1001) docker     (121)    13071 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/src/utils/NotebookListener.ts
+-rw-r--r--   0 runner    (1001) docker     (121)     5485 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/src/utils/NotebookPollingListener.ts
+-rw-r--r--   0 runner    (1001) docker     (121)      603 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/src/utils/useInterval.ts
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 09:37:24.666516 rucio_jupyterlab-0.9.8/src/widgets/
+-rw-r--r--   0 runner    (1001) docker     (121)     4774 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/src/widgets/InjectNotebookToolbar.tsx
+-rw-r--r--   0 runner    (1001) docker     (121)     9392 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/src/widgets/RucioUploadDialog.tsx
+-rw-r--r--   0 runner    (1001) docker     (121)     5047 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/src/widgets/SidebarPanel.tsx
+-rw-r--r--   0 runner    (1001) docker     (121)     1875 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/src/widgets/UploadLogViewerWidget.tsx
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 09:37:24.666516 rucio_jupyterlab-0.9.8/style/
+-rw-r--r--   0 runner    (1001) docker     (121)      989 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/style/index.css
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/style/index.js
+-rw-r--r--   0 runner    (1001) docker     (121)      550 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (121)      158 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/webpack.config.js
+-rw-r--r--   0 runner    (1001) docker     (121)   391483 2022-10-11 09:32:41.000000 rucio_jupyterlab-0.9.8/yarn.lock
```

### Comparing `rucio_jupyterlab-0.9.7/.eslintrc.js` & `rucio_jupyterlab-0.9.8/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/CONFIGURATION.md` & `rucio_jupyterlab-0.9.8/CONFIGURATION.md`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/CONTRIBUTING.md` & `rucio_jupyterlab-0.9.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/LICENSE` & `rucio_jupyterlab-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/MANIFEST.in` & `rucio_jupyterlab-0.9.8/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/PKG-INFO` & `rucio_jupyterlab-0.9.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rucio_jupyterlab
-Version: 0.9.7
+Version: 0.9.8
 Summary: JupyterLab extension for integrating Rucio
 Home-page: https://github.com/rucio/jupyterlab-extension
 Author: Muhammad Aditya Hilmy
 Author-email: mhilmy@hey.com
 License: Apache-2.0
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `rucio_jupyterlab-0.9.7/README.md` & `rucio_jupyterlab-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/RELEASE.md` & `rucio_jupyterlab-0.9.8/RELEASE.md`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/package.json` & `rucio_jupyterlab-0.9.8/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'version'": "'0.9.8'"}*

```diff
@@ -104,9 +104,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/src/index.d.ts",
-    "version": "0.9.7"
+    "version": "0.9.8"
 }
```

### Comparing `rucio_jupyterlab-0.9.7/pyproject.toml` & `rucio_jupyterlab-0.9.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/config/config.py` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/config/config.py`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/config/schema.py` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/config/schema.py`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/db.py` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/db.py`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/entity.py` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/entity.py`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/handlers/auth_config.py` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/handlers/auth_config.py`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/handlers/base.py` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/handlers/base.py`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/handlers/did_browser.py` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/handlers/did_browser.py`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/handlers/did_details.py` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/handlers/did_details.py`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/handlers/did_make_available.py` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/handlers/did_make_available.py`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/handlers/did_search.py` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/handlers/did_search.py`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/handlers/file_browser.py` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/handlers/file_browser.py`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/handlers/handlers.py` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/handlers/handlers.py`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/handlers/instances.py` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/handlers/instances.py`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/handlers/list_rses.py` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/handlers/list_rses.py`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/handlers/list_scopes.py` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/handlers/list_scopes.py`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/handlers/oidc_auth_check.py` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/handlers/oidc_auth_check.py`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/handlers/open_replication_rule.py` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/handlers/open_replication_rule.py`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/handlers/purge_cache.py` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/handlers/purge_cache.py`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/handlers/upload.py` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/handlers/upload.py`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/handlers/upload_jobs.py` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/handlers/upload_jobs.py`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/handlers/upload_jobs_details.py` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/handlers/upload_jobs_details.py`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/handlers/upload_jobs_log.py` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/handlers/upload_jobs_log.py`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/kernels/ipython/__init__.py` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/kernels/ipython/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/kernels/ipython/types.py` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/kernels/ipython/types.py`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/labextension/package.json` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9745833333333334%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.ce6881670499ee5dfee1.js'}}",*

 * * "'version'": "'0.9.8'"}*

```diff
@@ -51,15 +51,15 @@
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "style/index.js"
     ],
     "homepage": "https://github.com/rucio/jupyterlab-extension",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.13b02eee40e64df104ad.js",
+            "load": "static/remoteEntry.ce6881670499ee5dfee1.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "rucio_jupyterlab"
                 },
@@ -109,9 +109,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/src/index.d.ts",
-    "version": "0.9.7"
+    "version": "0.9.8"
 }
```

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/labextension/static/130.7365b614084ad0cbc49d.js` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/labextension/static/130.7365b614084ad0cbc49d.js`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/labextension/static/20.53c11c5b79a94ee424cb.js` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/labextension/static/20.53c11c5b79a94ee424cb.js`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/labextension/static/392.c6f78101fd8442eea43d.js` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/labextension/static/392.c6f78101fd8442eea43d.js`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/labextension/static/429.407b01bdf4a8a104bc25.js` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/labextension/static/429.407b01bdf4a8a104bc25.js`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/labextension/static/437.e8e22924cb4070990f2f.js` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/labextension/static/162.f78f93f2c02451004fb9.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,33 +1,30 @@
 "use strict";
 (self.webpackChunkrucio_jupyterlab = self.webpackChunkrucio_jupyterlab || []).push([
-    [437], {
-        1437: (e, t, a) => {
-            a.r(t), a.d(t, {
-                default: () => Nt
+    [162], {
+        4162: (e, t, n) => {
+            n.r(t), n.d(t, {
+                default: () => Et
             });
-            var n = a(362),
-                o = a(309),
-                l = a(9876),
-                i = a(9839),
-                r = a(8918),
-                s = a(6271),
-                c = a.n(s);
-            const d = "rucio-jupyterlab",
-                m = "rucio_attachments",
-                p = `${d}:kernel`,
-                u = `${d}:frontend`;
-            var v;
-            ! function(e) {
-                e.UploadFile = `${d}:upload-file`, e.OpenUploadLog = `${d}:open-upload-log`
-            }(v || (v = {}));
+            var a = n(9334),
+                o = n(613),
+                l = n(3655),
+                r = n(4306),
+                i = (n(8918), n(6271)),
+                c = n.n(i);
+            const s = "rucio-jupyterlab",
+                d = "rucio_attachments",
+                m = `${s}:kernel`,
+                p = `${s}:frontend`;
+            var u, v;
+            (v = u || (u = {})).UploadFile = `${s}:upload-file`, v.OpenUploadLog = `${s}:open-upload-log`;
             const h = c().createContext(void 0);
-            var g = a(8053),
-                f = a(4057),
-                b = a(5766);
+            var g = n(8053),
+                f = n(9061),
+                b = n(5766);
             const E = () => c().createElement("div", {
                     dangerouslySetInnerHTML: {
                         __html: '\n<svg width="100px" viewBox="0 0 1779 453" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" xml:space="preserve" xmlns:serif="http://www.serif.com/" style="fill-rule:evenodd;clip-rule:evenodd;stroke-linejoin:round;stroke-miterlimit:2;">\n    <g transform="matrix(1,0,0,1,-3188,-9151.54)">\n        <g transform="matrix(4.16667,0,0,4.16667,4082.17,9382.56)">\n            <g transform="matrix(1,0,0,1,-297.64,-209.765)">\n                <path d="M237.05,194.69C237.05,180.103 226.987,172.807 206.86,172.8L182.59,172.8L182.59,246.88L202.59,246.88L202.59,219.88L207.66,219.88L223.37,246.88L246.06,246.88L224.49,214.6C232.87,209.913 237.057,203.277 237.05,194.69ZM206.35,204.87L202.6,204.87L202.6,188L206.6,188C213.46,188 216.89,190.55 216.89,195.65C216.857,201.797 213.343,204.87 206.35,204.87Z" style="fill:var(--jp-ui-font-color1);fill-rule:nonzero;"/>\n                <path d="M295.78,216.17C295.78,221.503 294.857,225.347 293.01,227.7C291.163,230.053 288.2,231.227 284.12,231.22C280.307,231.22 277.42,230.037 275.46,227.67C273.5,225.303 272.52,221.503 272.52,216.27L272.52,172.8L252.41,172.8L252.41,217.8C252.41,227.487 255.12,234.917 260.54,240.09C265.96,245.263 273.72,247.847 283.82,247.84C294.16,247.84 302.073,245.173 307.56,239.84C313.047,234.507 315.79,227 315.79,217.32L315.79,172.8L295.79,172.8L295.78,216.17Z" style="fill:var(--jp-ui-font-color1);fill-rule:nonzero;"/>\n                <path d="M364.33,188.15C367.318,188.127 370.29,188.572 373.14,189.47C375.943,190.374 378.685,191.456 381.35,192.71L387.48,177C380.307,173.543 372.442,171.758 364.48,171.78C357.8,171.615 351.196,173.234 345.35,176.47C339.944,179.581 335.6,184.252 332.89,189.87C329.922,196.157 328.456,203.049 328.61,210C328.61,222.26 331.59,231.633 337.55,238.12C343.51,244.607 352.08,247.85 363.26,247.85C370.47,247.972 377.625,246.575 384.26,243.75L384.26,226.86C381.23,228.122 378.136,229.223 374.99,230.16C371.896,231.071 368.686,231.529 365.46,231.52C354.62,231.52 349.2,224.393 349.2,210.14C349.2,203.293 350.533,197.917 353.2,194.01C355.621,190.243 359.854,188.014 364.33,188.15Z" style="fill:var(--jp-ui-font-color1);fill-rule:nonzero;"/>\n                <rect x="398.68" y="172.8" width="20.11" height="74.07" style="fill:var(--jp-ui-font-color1);"/>\n                <path d="M495,181.31C488.92,174.863 479.983,171.64 468.19,171.64C456.397,171.64 447.437,174.89 441.31,181.39C435.15,187.89 432.07,197.307 432.07,209.64C432.07,222.1 435.17,231.59 441.37,238.11C447.57,244.63 456.477,247.89 468.09,247.89C479.883,247.89 488.833,244.647 494.94,238.16C501.047,231.673 504.107,222.2 504.12,209.74C504.12,197.247 501.08,187.77 495,181.31ZM479.37,226C476.923,229.48 473.163,231.22 468.09,231.22C458.13,231.22 453.15,224.06 453.15,209.74C453.15,195.28 458.15,188.05 468.15,188.05C473.083,188.05 476.79,189.817 479.27,193.35C481.75,196.883 482.993,202.347 483,209.74C483,217.1 481.79,222.52 479.37,226Z" style="fill:var(--jp-ui-font-color1);fill-rule:nonzero;"/>\n                <path d="M164.12,233.55L164.12,242.81C164.115,243.788 163.308,244.59 162.33,244.59L96.24,244.59C95.264,244.59 94.46,243.786 94.46,242.81L91.16,242.81C91.165,245.595 93.455,247.885 96.24,247.89L162.33,247.89C165.115,247.885 167.405,245.595 167.41,242.81L167.41,230.59C166.513,231.779 165.396,232.784 164.12,233.55Z" style="fill:var(--jp-ui-font-color1);fill-rule:nonzero;"/>\n                <path d="M164.12,176.72L164.12,213.52C165.401,214.298 166.518,215.316 167.41,216.52L167.41,176.72C167.405,173.935 165.115,171.645 162.33,171.64L125.18,171.64L125.18,174.93L162.33,174.93C163.312,174.93 164.12,175.738 164.12,176.72Z" style="fill:var(--jp-ui-font-color1);fill-rule:nonzero;"/>\n                <path d="M162.92,215.14L154.52,210.3L145,204.79C139.786,201.786 133.026,203.589 130,208.79L111.2,241.3L136.65,241.3L146,225.13L149,226.85C150.396,230.665 154.047,233.217 158.109,233.217C163.431,233.217 167.809,228.838 167.809,223.517C167.809,220.072 165.975,216.877 163,215.14L162.92,215.14ZM143.56,210.31C144.272,209.069 145.598,208.301 147.029,208.301C149.223,208.301 151.029,210.107 151.029,212.301C151.029,214.496 149.223,216.301 147.029,216.301C146.323,216.301 145.63,216.114 145.02,215.76C143.129,214.662 142.472,212.206 143.56,210.31ZM165.93,228.08C164.312,230.883 161.312,232.615 158.075,232.615C154.269,232.615 150.849,230.218 149.55,226.64L149.47,226.43L149.27,226.31L146.27,224.59L149.01,219.85C149.12,219.66 149.23,219.46 149.32,219.27L154.19,210.84L162.59,215.68C166.903,218.169 168.41,223.762 165.93,228.08Z" style="fill:var(--jp-ui-font-color1);fill-rule:nonzero;"/>\n                <circle cx="164.08" cy="223.16" r="1.7" style="fill:var(--jp-ui-font-color1);"/>\n                <path d="M110.09,238.4L107.4,236.85L108.96,234.15L111.65,235.71L110.09,238.4ZM113.2,233L110.51,231.45L112.07,228.76L114.76,230.31L113.2,233ZM116.31,227.62L113.62,226.06L115.18,223.37L117.87,224.93L116.31,227.62ZM119.42,222.23L116.73,220.68L118.28,217.99L120.98,219.54L119.42,222.23ZM122.53,216.85L119.84,215.29L121.39,212.6L124.09,214.16L122.53,216.85ZM125.64,211.46L123,209.92L124.55,207.23L127.25,208.78L125.64,211.46ZM128.74,206.29L126.25,204.43C126.93,203.509 127.708,202.664 128.57,201.91L130.62,204.24C129.922,204.858 129.291,205.548 128.74,206.3L128.74,206.29ZM146.21,202.7C145.404,202.235 144.553,201.853 143.67,201.56L144.67,198.61C145.757,198.963 146.804,199.432 147.79,200.01L146.21,202.7ZM132.89,202.63L131.36,199.92C132.359,199.363 133.411,198.907 134.5,198.56L135.44,201.56C134.556,201.835 133.702,202.197 132.89,202.64L132.89,202.63ZM141,201C140.076,200.9 139.144,200.9 138.22,201L137.91,197.9C139.047,197.78 140.193,197.78 141.33,197.9L141,201Z" style="fill:var(--jp-ui-font-color1);fill-rule:nonzero;"/>\n                <path d="M111.56,181.07C111.454,180.947 111.396,180.79 111.396,180.627C111.396,180.254 111.703,179.947 112.076,179.947C112.135,179.947 112.193,179.955 112.25,179.97C120.411,181.977 126.373,189.084 126.93,197.47C126.931,197.484 126.931,197.499 126.931,197.513C126.931,197.887 126.624,198.193 126.251,198.193C126.05,198.193 125.859,198.104 125.73,197.95L111.56,181.07Z" style="fill:var(--jp-ui-font-color1);fill-rule:nonzero;"/>\n                <path d="M96.6,189.58C96.469,189.503 96.319,189.463 96.167,189.463C95.695,189.463 95.307,189.851 95.307,190.323C95.307,190.442 95.332,190.561 95.38,190.67C99.674,200.429 109.871,206.314 120.47,205.15C120.902,205.1 121.232,204.73 121.232,204.296C121.232,203.988 121.067,203.703 120.8,203.55L96.6,189.58Z" style="fill:var(--jp-ui-font-color1);fill-rule:nonzero;"/>\n                <circle cx="149.3" cy="212.22" r="1.7" style="fill:var(--jp-ui-font-color1);"/>\n                <path d="M166,228.18C162.98,228.18 159.967,227.899 157,227.34L156.7,228.91C159.388,229.422 162.114,229.71 164.85,229.77C165.296,229.295 165.691,228.776 166.03,228.22L166,228.18Z" style="fill:var(--jp-ui-font-color1);fill-rule:nonzero;"/>\n            </g>\n        </g>\n    </g>\n</svg>\n'
                     }
                 }),
                 x = (0, g.createUseStyles)({
                     container: {
@@ -86,34 +83,34 @@
                         extend: "tabItem",
                         float: "right"
                     }
                 }),
                 S = ({
                     menus: e,
                     value: t,
-                    onChange: a
+                    onChange: n
                 }) => {
-                    const n = I();
+                    const a = I();
                     return c().createElement("div", null, c().createElement("ul", {
-                        className: n.tab
+                        className: a.tab
                     }, e.map((e => {
                         const o = e.value === t ? "active" : "",
                             l = e.disabled ? "disabled" : "",
-                            i = e.right ? n.tabItemRight : n.tabItem;
+                            r = e.right ? a.tabItemRight : a.tabItem;
                         return c().createElement("li", {
-                            onClick: e.disabled ? void 0 : () => a(e.value),
+                            onClick: e.disabled ? void 0 : () => n(e.value),
                             key: e.value,
-                            className: `${i} ${o} ${l}`
+                            className: `${r} ${o} ${l}`
                         }, e.title)
                     }))))
                 };
-            var k = a(7370),
-                w = a(8196),
-                j = a.n(w);
-            const L = (0, g.createUseStyles)({
+            var k = n(7370),
+                w = n(8196),
+                j = n.n(w);
+            const A = (0, g.createUseStyles)({
                     control: {
                         display: "flex",
                         flexDirection: "row",
                         border: e => `1px solid ${e.outlineColor||"var(--jp-border-color1)"}`,
                         alignItems: "stretch"
                     },
                     input: {
@@ -125,40 +122,40 @@
                         minWidth: 0,
                         color: e => e.color || "var(--jp-ui-font-color1)"
                     },
                     block: {
                         width: "100%"
                     }
                 }),
-                A = c().forwardRef(((e, t) => {
+                L = c().forwardRef(((e, t) => {
                     const {
-                        block: a,
-                        before: n,
+                        block: n,
+                        before: a,
                         after: o,
                         outlineColor: l,
-                        className: i,
-                        containerStyle: r
+                        className: r,
+                        containerStyle: i
                     } = e, s = function(e, t) {
-                        var a = {};
-                        for (var n in e) Object.prototype.hasOwnProperty.call(e, n) && t.indexOf(n) < 0 && (a[n] = e[n]);
+                        var n = {};
+                        for (var a in e) Object.prototype.hasOwnProperty.call(e, a) && t.indexOf(a) < 0 && (n[a] = e[a]);
                         if (null != e && "function" == typeof Object.getOwnPropertySymbols) {
                             var o = 0;
-                            for (n = Object.getOwnPropertySymbols(e); o < n.length; o++) t.indexOf(n[o]) < 0 && Object.prototype.propertyIsEnumerable.call(e, n[o]) && (a[n[o]] = e[n[o]])
+                            for (a = Object.getOwnPropertySymbols(e); o < a.length; o++) t.indexOf(a[o]) < 0 && Object.prototype.propertyIsEnumerable.call(e, a[o]) && (n[a[o]] = e[a[o]])
                         }
-                        return a
-                    }(e, ["block", "before", "after", "outlineColor", "className", "containerStyle"]), d = L({
+                        return n
+                    }(e, ["block", "before", "after", "outlineColor", "className", "containerStyle"]), d = A({
                         outlineColor: l
                     }), m = [d.input];
-                    return a && m.push(d.block), c().createElement("div", {
+                    return n && m.push(d.block), c().createElement("div", {
                         className: d.control,
-                        style: r
-                    }, n, c().createElement("input", Object.assign({
+                        style: i
+                    }, a, c().createElement("input", Object.assign({
                         ref: t,
                         type: "text",
-                        className: m.join(" ") + " " + i || ""
+                        className: m.join(" ") + " " + r || ""
                     }, s)), o)
                 })),
                 O = (0, g.createUseStyles)({
                     heading: {
                         borderBottom: "1px solid var(--jp-border-color2)",
                         margin: 0,
                         padding: "24px 16px 8px 16px",
@@ -172,16 +169,16 @@
                     title: e
                 }) => {
                     const t = O();
                     return c().createElement("div", {
                         className: t.heading
                     }, e)
                 };
-            var R = a(7697),
-                P = a(4139);
+            var R = n(5012),
+                P = n(5322);
             const T = (0, g.createUseStyles)({
                     "@keyframes rotation": {
                         from: {
                             transform: "rotate(0deg)"
                         },
                         to: {
                             transform: "rotate(359deg)"
@@ -191,260 +188,260 @@
                         animation: "$rotation 1s infinite linear",
                         animationName: "$rotation"
                     }
                 }),
                 M = e => {
                     var {
                         children: t,
-                        className: a
-                    } = e, n = function(e, t) {
-                        var a = {};
-                        for (var n in e) Object.prototype.hasOwnProperty.call(e, n) && t.indexOf(n) < 0 && (a[n] = e[n]);
+                        className: n
+                    } = e, a = function(e, t) {
+                        var n = {};
+                        for (var a in e) Object.prototype.hasOwnProperty.call(e, a) && t.indexOf(a) < 0 && (n[a] = e[a]);
                         if (null != e && "function" == typeof Object.getOwnPropertySymbols) {
                             var o = 0;
-                            for (n = Object.getOwnPropertySymbols(e); o < n.length; o++) t.indexOf(n[o]) < 0 && Object.prototype.propertyIsEnumerable.call(e, n[o]) && (a[n[o]] = e[n[o]])
+                            for (a = Object.getOwnPropertySymbols(e); o < a.length; o++) t.indexOf(a[o]) < 0 && Object.prototype.propertyIsEnumerable.call(e, a[o]) && (n[a[o]] = e[a[o]])
                         }
-                        return a
+                        return n
                     }(e, ["children", "className"]);
                     const o = T();
                     return c().createElement("span", Object.assign({
-                        className: `${a} ${o.rotate}`
-                    }, n), t)
+                        className: `${n} ${o.rotate}`
+                    }, a), t)
                 };
-            var F = a(7673),
-                _ = a(3760),
-                U = a.n(_);
-            async function z(e = "", t = {}, a = !0) {
-                const n = P.ServerConnection.makeSettings(),
-                    o = R.URLExt.join(n.baseUrl, d, e);
+            var F = n(7673),
+                z = n(3760),
+                $ = n.n(z);
+            async function U(e = "", t = {}, n = !0) {
+                const a = P.ServerConnection.makeSettings(),
+                    o = R.URLExt.join(a.baseUrl, s, e);
                 let l;
                 try {
-                    l = await P.ServerConnection.makeRequest(o, t, n)
+                    l = await P.ServerConnection.makeRequest(o, t, a)
                 } catch (e) {
                     throw new P.ServerConnection.NetworkError(e)
                 }
-                const i = await l.json();
-                if (!l.ok) throw new P.ServerConnection.ResponseError(l, i.message);
-                return a ? U()(i) : i
+                const r = await l.json();
+                if (!l.ok) throw new P.ServerConnection.ResponseError(l, r.message);
+                return n ? $()(r) : r
             }
-            const $ = new class {
+            const _ = new class {
                 async fetchInstancesConfig() {
-                    return z("instances")
+                    return U("instances")
                 }
                 async postActiveInstance(e, t) {
-                    return z("instances", {
+                    return U("instances", {
                         method: "PUT",
                         body: JSON.stringify({
                             instance: e,
                             auth: t
                         })
                     })
                 }
                 async fetchAuthConfig(e, t) {
-                    const a = {
+                    const n = {
                         namespace: e,
                         type: t
                     };
-                    return z(`auth?${F.encode(a)}`)
+                    return U(`auth?${F.encode(n)}`)
                 }
-                async putAuthConfig(e, t, a) {
-                    return z("auth", {
+                async putAuthConfig(e, t, n) {
+                    return U("auth", {
                         method: "PUT",
                         body: JSON.stringify({
                             namespace: e,
                             type: t,
-                            params: a
+                            params: n
                         })
                     })
                 }
-                async searchDID(e, t, a) {
-                    const n = {
+                async searchDID(e, t, n) {
+                    const a = {
                         namespace: e,
                         did: t,
-                        type: a
+                        type: n
                     };
-                    return z(`did-search?${F.encode(n)}`)
+                    return U(`did-search?${F.encode(a)}`)
                 }
                 async fetchScopes(e) {
                     const t = {
                         namespace: e
                     };
-                    return z(`list-scopes?${F.encode(t)}`)
+                    return U(`list-scopes?${F.encode(t)}`)
                 }
                 async fetchRSEs(e, t) {
-                    const a = {
+                    const n = {
                         namespace: e,
                         expression: t
                     };
-                    return z(`list-rses?${F.encode(a)}`)
+                    return U(`list-rses?${F.encode(n)}`)
                 }
                 async fetchAttachedFileDIDs(e, t) {
-                    const a = {
+                    const n = {
                         namespace: e,
                         did: t
                     };
-                    return z(`files?${F.encode(a)}`)
+                    return U(`files?${F.encode(n)}`)
                 }
-                async fetchDIDDetails(e, t, a = !1) {
-                    const n = {
+                async fetchDIDDetails(e, t, n = !1) {
+                    const a = {
                         namespace: e,
                         did: t,
-                        poll: a ? 1 : void 0
+                        poll: n ? 1 : void 0
                     };
-                    return z("did?" + F.encode(n))
+                    return U("did?" + F.encode(a))
                 }
-                async getFileDIDDetails(e, t, a = !1) {
-                    const n = C.getRawState().fileDetails[t];
-                    if (!a && n) return n;
-                    const o = await this.fetchDIDDetails(e, t, a),
+                async getFileDIDDetails(e, t, n = !1) {
+                    const a = C.getRawState().fileDetails[t];
+                    if (!n && a) return a;
+                    const o = await this.fetchDIDDetails(e, t, n),
                         l = o.reduce(((e, t) => (e[t.did] = t, e)), {});
                     return C.update((e => {
                         e.fileDetails = Object.assign(Object.assign({}, e.fileDetails), l)
                     })), o[0]
                 }
-                async getCollectionDIDDetails(e, t, a = !1) {
-                    const n = C.getRawState().collectionDetails[t];
-                    if (!a && n) return n;
-                    const o = await this.fetchDIDDetails(e, t, a);
+                async getCollectionDIDDetails(e, t, n = !1) {
+                    const a = C.getRawState().collectionDetails[t];
+                    if (!n && a) return a;
+                    const o = await this.fetchDIDDetails(e, t, n);
                     return C.update((e => {
                         e.collectionDetails[t] = o
                     })), o
                 }
                 async makeFileAvailable(e, t) {
-                    const a = C.getRawState().fileDetails[t];
+                    const n = C.getRawState().fileDetails[t];
                     C.update((e => {
-                        e.fileDetails[t] = Object.assign(Object.assign({}, a), {
+                        e.fileDetails[t] = Object.assign(Object.assign({}, n), {
                             status: "REPLICATING"
                         })
                     }));
-                    const n = {
+                    const a = {
                         method: "POST",
                         body: JSON.stringify({
                             did: t
                         })
                     };
-                    return z("did/make-available?namespace=" + encodeURIComponent(e), n)
+                    return U("did/make-available?namespace=" + encodeURIComponent(e), a)
                 }
                 async makeCollectionAvailable(e, t) {
-                    const a = C.getRawState().collectionDetails[t].map((e => Object.assign(Object.assign({}, e), {
+                    const n = C.getRawState().collectionDetails[t].map((e => Object.assign(Object.assign({}, e), {
                         status: "OK" === e.status ? "OK" : "REPLICATING"
                     })));
                     C.update((e => {
-                        e.collectionDetails[t] = a
+                        e.collectionDetails[t] = n
                     }));
-                    const n = {
+                    const a = {
                         method: "POST",
                         body: JSON.stringify({
                             did: t
                         })
                     };
-                    return z("did/make-available?namespace=" + encodeURIComponent(e), n)
+                    return U("did/make-available?namespace=" + encodeURIComponent(e), a)
                 }
                 async listDirectory(e) {
-                    return z("file-browser?path=" + encodeURIComponent(e))
+                    return U("file-browser?path=" + encodeURIComponent(e))
                 }
                 async purgeCache() {
-                    return z("purge-cache", {
+                    return U("purge-cache", {
                         method: "POST"
                     })
                 }
                 async uploadFile(e, t) {
                     const {
-                        paths: a,
-                        rse: n,
+                        paths: n,
+                        rse: a,
                         fileScope: o,
                         datasetName: l,
-                        addToDataset: i,
-                        datasetScope: r,
-                        lifetime: s
-                    } = t, c = {
+                        addToDataset: r,
+                        datasetScope: i,
+                        lifetime: c
+                    } = t, s = {
                         method: "POST",
                         body: JSON.stringify({
-                            file_paths: a,
-                            rse: n,
+                            file_paths: n,
+                            rse: a,
                             scope: o,
-                            add_to_dataset: !!i,
-                            dataset_scope: r,
+                            add_to_dataset: !!r,
+                            dataset_scope: i,
                             dataset_name: l,
-                            lifetime: s
+                            lifetime: c
                         })
                     };
-                    return z("upload?namespace=" + encodeURIComponent(e), c)
+                    return U("upload?namespace=" + encodeURIComponent(e), s)
                 }
                 async fetchUploadJobs(e) {
                     const t = {
                         namespace: e
                     };
-                    return z("upload/jobs?" + F.encode(t))
+                    return U("upload/jobs?" + F.encode(t))
                 }
                 async fetchUploadJobLog(e, t) {
-                    const a = {
+                    const n = {
                         namespace: e,
                         id: t
                     };
-                    return z("upload/jobs/log?" + F.encode(a))
+                    return U("upload/jobs/log?" + F.encode(n))
                 }
                 async deleteUploadJob(e, t) {
-                    const a = {
+                    const n = {
                         namespace: e,
                         id: t
                     };
-                    return z("upload/jobs/details?" + F.encode(a), {
+                    return U("upload/jobs/details?" + F.encode(n), {
                         method: "DELETE"
                     })
                 }
             };
 
             function B(e) {
                 return class extends c().Component {
                     render() {
                         const t = function(e, t) {
-                            var a = {};
-                            for (var n in e) Object.prototype.hasOwnProperty.call(e, n) && t.indexOf(n) < 0 && (a[n] = e[n]);
+                            var n = {};
+                            for (var a in e) Object.prototype.hasOwnProperty.call(e, a) && t.indexOf(a) < 0 && (n[a] = e[a]);
                             if (null != e && "function" == typeof Object.getOwnPropertySymbols) {
                                 var o = 0;
-                                for (n = Object.getOwnPropertySymbols(e); o < n.length; o++) t.indexOf(n[o]) < 0 && Object.prototype.propertyIsEnumerable.call(e, n[o]) && (a[n[o]] = e[n[o]])
+                                for (a = Object.getOwnPropertySymbols(e); o < a.length; o++) t.indexOf(a[o]) < 0 && Object.prototype.propertyIsEnumerable.call(e, a[o]) && (n[a[o]] = e[a[o]])
                             }
-                            return a
+                            return n
                         }(this.props, []);
                         return c().createElement(e, Object.assign({}, t, {
-                            actions: $
+                            actions: _
                         }))
                     }
                 }
             }
-            var V = a(454),
-                K = a.n(V);
-            const Z = new b.Store({}),
+            var K = n(454),
+                Z = n.n(K);
+            const V = new b.Store({}),
                 G = e => {
                     if (!e) return !1;
                     if (0 === e.length) return "EMPTY";
                     const t = e.find((e => "OK" === e.status)),
-                        a = e.find((e => "NOT_AVAILABLE" === e.status)),
-                        n = e.find((e => "REPLICATING" === e.status)),
+                        n = e.find((e => "NOT_AVAILABLE" === e.status)),
+                        a = e.find((e => "REPLICATING" === e.status)),
                         o = e.find((e => "STUCK" === e.status));
-                    return n ? "REPLICATING" : o ? "STUCK" : t ? a ? "PARTIALLY_AVAILABLE" : "AVAILABLE" : "NOT_AVAILABLE"
+                    return a ? "REPLICATING" : o ? "STUCK" : t ? n ? "PARTIALLY_AVAILABLE" : "AVAILABLE" : "NOT_AVAILABLE"
                 },
                 J = e => !!e && !!e.match(/^[a-zA-Z0-9_]*$/) && !!isNaN(parseInt(e.charAt(0))),
-                W = e => {
+                q = e => {
                     if (e / 1073741824 >= 1) {
                         const t = e / 1073741824;
                         return Math.round(100 * t) / 100 + "GiB"
                     }
                     if (e / 1048576 >= 1) {
                         const t = e / 1048576;
                         return Math.round(100 * t) / 100 + "MiB"
                     }
                     if (e / 1024 >= 1) {
                         const t = e / 1024;
                         return Math.round(100 * t) / 100 + "KiB"
                     }
                     return `${e}B`
                 },
-                q = (0, g.createUseStyles)({
+                W = (0, g.createUseStyles)({
                     main: {
                         background: "var(--jp-layout-color1)",
                         color: "var(--jp-ui-font-color1)"
                     },
                     textField: {
                         width: "200px",
                         background: "var(--jp-layout-color1)",
@@ -475,102 +472,102 @@
                     error: {
                         color: "var(--jp-error-color2)"
                     }
                 }),
                 H = ({
                     children: e,
                     did: t,
-                    type: a
+                    type: n
                 }) => {
-                    const n = q(),
-                        o = (0, s.useRef)(null),
-                        [l, i] = (0, s.useState)(!1),
-                        [r, d] = (0, s.useState)(),
-                        [m, p] = (0, s.useState)(""),
-                        u = (0, b.useStoreState)(Z, (e => e.activeNotebookPanel)),
-                        v = (0, b.useStoreState)(Z, (e => e.activeNotebookAttachment)),
-                        h = (0, s.useMemo)((() => v ? v.map((e => e.variableName)) : []), [v]),
-                        g = (0, s.useMemo)((() => !!v && !!v.find((e => e.did === t))), [v]),
-                        f = (0, s.useCallback)((e => {
-                            27 === e.keyCode && i(!1)
+                    const a = W(),
+                        o = (0, i.useRef)(null),
+                        [l, r] = (0, i.useState)(!1),
+                        [s, d] = (0, i.useState)(),
+                        [m, p] = (0, i.useState)(""),
+                        u = (0, b.useStoreState)(V, (e => e.activeNotebookPanel)),
+                        v = (0, b.useStoreState)(V, (e => e.activeNotebookAttachment)),
+                        h = (0, i.useMemo)((() => v ? v.map((e => e.variableName)) : []), [v]),
+                        g = (0, i.useMemo)((() => !!v && !!v.find((e => e.did === t))), [v]),
+                        f = (0, i.useCallback)((e => {
+                            27 === e.keyCode && r(!1)
                         }), []);
-                    (0, s.useEffect)((() => (document.addEventListener("keydown", f, !1), () => {
+                    (0, i.useEffect)((() => (document.addEventListener("keydown", f, !1), () => {
                         document.removeEventListener("keydown", f, !1)
                     })), []);
                     const E = () => {
                             if (!J(m) || x(m)) return;
-                            i(!1);
+                            r(!1);
                             const e = {
                                     did: t,
-                                    type: a,
+                                    type: n,
                                     variableName: m
                                 },
-                                n = v ? [...v, e] : [e];
+                                a = v ? [...v, e] : [e];
                             var o;
-                            o = n, Z.update((e => {
+                            o = a, V.update((e => {
                                 e.activeNotebookAttachment = o
                             }))
                         },
                         x = e => h.includes(e),
                         y = c().createElement("div", {
-                            className: n.proceedButton,
+                            className: a.proceedButton,
                             onClick: E
                         }, c().createElement("i", {
-                            className: `${n.proceedIcon} material-icons`
+                            className: `${a.proceedIcon} material-icons`
                         }, "arrow_forward")),
                         C = c().createElement("div", {
-                            className: n.main
-                        }, c().createElement(A, {
+                            className: a.main
+                        }, c().createElement(L, {
                             ref: o,
-                            className: n.textField,
+                            className: a.textField,
                             outlineColor: "var(--jp-layout-color1)",
                             placeholder: "Enter a variable name",
                             onKeyPress: e => {
                                 "Enter" === e.key && E()
                             },
                             after: y,
                             value: m,
                             onChange: e => {
                                 return t = e.target.value, p(t), void(t && !J(t) ? d("Invalid variable name") : x(t) ? d("Variable name exists") : d(void 0));
                                 var t
                             }
                         }), c().createElement("div", {
-                            className: n.instructions
-                        }, !r && c().createElement("span", null, "Press Enter to proceed, Esc to cancel"), !!r && c().createElement("span", {
-                            className: n.error
-                        }, r)));
-                    return c().createElement(c().Fragment, null, !!u && !g && c().createElement(K(), {
+                            className: a.instructions
+                        }, !s && c().createElement("span", null, "Press Enter to proceed, Esc to cancel"), !!s && c().createElement("span", {
+                            className: a.error
+                        }, s)));
+                    return c().createElement(c().Fragment, null, !!u && !g && c().createElement(Z(), {
                         enterExitTransitionDurationMs: 0,
                         isOpen: l,
                         preferPlace: "below",
                         body: C,
-                        onOuterAction: () => i(!1)
+                        onOuterAction: () => r(!1)
                     }, c().createElement("div", {
                         onClick: () => {
-                            i(!0), p(""), d(void 0), setTimeout((() => {
+                            r(!0), p(""), d(void 0), setTimeout((() => {
                                 var e;
                                 null === (e = o.current) || void 0 === e || e.focus()
                             }), 10)
                         }
                     }, e)))
                 };
             class Y {}
             const X = new class {
                 constructor() {
                     this.pollingRequesterMap = {}, setInterval((() => {
                         this.poll()
                     }), 1e4)
                 }
-                requestPolling(e, t, a, n = !0) {
+                requestPolling(e, t, n, a = !0) {
                     this.pollingRequesterMap[e] || (this.pollingRequesterMap[e] = {
                         type: t,
                         refs: []
                     });
-                    const o = a || new Y;
-                    return this.pollingRequesterMap[e].refs.push(o), n && this.fetchDid(e), () => {
+                    const o = n || new Y;
+                    return this.pollingRequesterMap[e].refs.push(o), a && this.fetchDid(e), () => {
                         this.disablePolling(e, o)
                     }
                 }
                 disablePolling(e, t) {
                     this.pollingRequesterMap[e] && (this.pollingRequesterMap[e].refs = this.pollingRequesterMap[e].refs.filter((e => e !== t)))
                 }
                 poll() {
@@ -580,37 +577,37 @@
                 }
                 fetchDid(e) {
                     const {
                         activeInstance: t
                     } = C.getRawState();
                     if (t) switch (this.pollingRequesterMap[e].type) {
                         case "file":
-                            $.getFileDIDDetails(t.name, e, !0).then((t => {
+                            _.getFileDIDDetails(t.name, e, !0).then((t => {
                                 "REPLICATING" !== t.status && delete this.pollingRequesterMap[e]
                             }));
                             break;
                         case "collection":
-                            $.getCollectionDIDDetails(t.name, e, !0).then((t => {
+                            _.getCollectionDIDDetails(t.name, e, !0).then((t => {
                                 t.find((e => "REPLICATING" === e.status)) || delete this.pollingRequesterMap[e]
                             }))
                     }
                 }
             };
 
             function Q(e) {
                 return class extends c().Component {
                     render() {
                         const t = function(e, t) {
-                            var a = {};
-                            for (var n in e) Object.prototype.hasOwnProperty.call(e, n) && t.indexOf(n) < 0 && (a[n] = e[n]);
+                            var n = {};
+                            for (var a in e) Object.prototype.hasOwnProperty.call(e, a) && t.indexOf(a) < 0 && (n[a] = e[a]);
                             if (null != e && "function" == typeof Object.getOwnPropertySymbols) {
                                 var o = 0;
-                                for (n = Object.getOwnPropertySymbols(e); o < n.length; o++) t.indexOf(n[o]) < 0 && Object.prototype.propertyIsEnumerable.call(e, n[o]) && (a[n[o]] = e[n[o]])
+                                for (a = Object.getOwnPropertySymbols(e); o < a.length; o++) t.indexOf(a[o]) < 0 && Object.prototype.propertyIsEnumerable.call(e, a[o]) && (n[a[o]] = e[a[o]])
                             }
-                            return a
+                            return n
                         }(this.props, []);
                         return c().createElement(e, Object.assign({}, t, {
                             didPollingManager: X
                         }))
                     }
                 }
             }
@@ -668,157 +665,157 @@
                         color: "var(--jp-rucio-primary-blue-color)",
                         cursor: "pointer"
                     }
                 }),
                 te = ({
                     did: e,
                     path: t,
-                    showReplicationRuleUrl: a
+                    showReplicationRuleUrl: n
                 }) => {
-                    const n = ee();
+                    const a = ee();
                     return c().createElement("div", {
-                        className: n.statusAvailable
+                        className: a.statusAvailable
                     }, c().createElement("i", {
-                        className: `${n.icon} material-icons`
-                    }, "check_circle"), a && c().createElement("div", {
-                        className: n.clickableStatusText
+                        className: `${a.icon} material-icons`
+                    }, "check_circle"), n && c().createElement("div", {
+                        className: a.clickableStatusText
                     }, c().createElement("a", {
-                        href: a,
+                        href: n,
                         target: "_blank",
                         rel: "noreferrer",
                         title: "Show replication rule"
-                    }, "Available")), !a && c().createElement("div", {
-                        className: n.statusText
+                    }, "Available")), !n && c().createElement("div", {
+                        className: a.statusText
                     }, "Available"), c().createElement("div", {
-                        className: n.action
+                        className: a.action
                     }, c().createElement(H, {
                         did: e,
                         type: "file"
                     }, "Add to Notebook")))
                 },
-                ae = ({
+                ne = ({
                     onMakeAvailableClicked: e
                 }) => {
                     const t = ee();
                     return c().createElement("div", {
                         className: t.statusNotAvailable
                     }, c().createElement("i", {
                         className: `${t.icon} material-icons`
                     }, "lens"), c().createElement("div", {
                         className: t.statusText
                     }, "Not Available"), c().createElement("div", {
                         className: t.action,
                         onClick: e
                     }, "Make Available"))
                 },
-                ne = ({
+                ae = ({
                     did: e,
                     showReplicationRuleUrl: t
                 }) => {
-                    const a = ee();
+                    const n = ee();
                     return c().createElement("div", {
-                        className: a.statusReplicating
+                        className: n.statusReplicating
                     }, c().createElement(M, {
-                        className: `${a.icon} material-icons`
+                        className: `${n.icon} material-icons`
                     }, "hourglass_top"), t && c().createElement("div", {
-                        className: a.clickableStatusText
+                        className: n.clickableStatusText
                     }, c().createElement("a", {
                         href: t,
                         target: "_blank",
                         rel: "noreferrer",
                         title: "Show replication rule"
                     }, "Replicating files...")), !t && c().createElement("div", {
-                        className: a.statusText
+                        className: n.statusText
                     }, "Replicating files..."), c().createElement("div", {
-                        className: a.action
+                        className: n.action
                     }, c().createElement(H, {
                         did: e,
                         type: "collection"
                     }, "Add to Notebook")))
                 },
                 oe = ({
                     onMakeAvailableClicked: e,
                     showReplicationRuleUrl: t
                 }) => {
-                    const a = ee();
+                    const n = ee();
                     return c().createElement("div", {
-                        className: a.statusNotAvailable
+                        className: n.statusNotAvailable
                     }, c().createElement("i", {
-                        className: `${a.icon} material-icons`
+                        className: `${n.icon} material-icons`
                     }, "error"), t && c().createElement("div", {
-                        className: a.clickableStatusText
+                        className: n.clickableStatusText
                     }, c().createElement("a", {
                         href: t,
                         target: "_blank",
                         rel: "noreferrer",
                         title: "Show replication rule"
                     }, "Something went wrong")), !t && c().createElement("div", {
-                        className: a.statusText
+                        className: n.statusText
                     }, "Something went wrong"), e && c().createElement("div", {
-                        className: a.action,
+                        className: n.action,
                         onClick: e
                     }, "Make Available"))
                 },
                 le = Q(B((e => {
                     var {
                         did: t
-                    } = e, a = function(e, t) {
-                        var a = {};
-                        for (var n in e) Object.prototype.hasOwnProperty.call(e, n) && t.indexOf(n) < 0 && (a[n] = e[n]);
+                    } = e, n = function(e, t) {
+                        var n = {};
+                        for (var a in e) Object.prototype.hasOwnProperty.call(e, a) && t.indexOf(a) < 0 && (n[a] = e[a]);
                         if (null != e && "function" == typeof Object.getOwnPropertySymbols) {
                             var o = 0;
-                            for (n = Object.getOwnPropertySymbols(e); o < n.length; o++) t.indexOf(n[o]) < 0 && Object.prototype.propertyIsEnumerable.call(e, n[o]) && (a[n[o]] = e[n[o]])
+                            for (a = Object.getOwnPropertySymbols(e); o < a.length; o++) t.indexOf(a[o]) < 0 && Object.prototype.propertyIsEnumerable.call(e, a[o]) && (n[a[o]] = e[a[o]])
                         }
-                        return a
+                        return n
                     }(e, ["did"]);
-                    const n = ee(),
+                    const a = ee(),
                         {
                             actions: o
-                        } = a,
+                        } = n,
                         {
                             didPollingManager: l
-                        } = a,
-                        i = (0, b.useStoreState)(C, (e => e.fileDetails[t])),
-                        r = (0, b.useStoreState)(C, (e => e.activeInstance)),
-                        [m] = (0, s.useState)((() => new Y)),
+                        } = n,
+                        r = (0, b.useStoreState)(C, (e => e.fileDetails[t])),
+                        d = (0, b.useStoreState)(C, (e => e.activeInstance)),
+                        [m] = (0, i.useState)((() => new Y)),
                         p = () => {
                             l.requestPolling(t, "file", m)
                         };
-                    (0, s.useEffect)((() => (p(), () => {
+                    (0, i.useEffect)((() => (p(), () => {
                         l.disablePolling(t, m)
                     })), []);
                     const u = () => {
-                            r && (null == o || o.makeFileAvailable(r.name, t).then((() => p())).catch((e => console.log(e))))
+                            d && (null == o || o.makeFileAvailable(d.name, t).then((() => p())).catch((e => console.log(e))))
                         },
                         v = P.ServerConnection.makeSettings(),
-                        h = R.URLExt.join(v.baseUrl, d, "open-replication-rule"),
-                        g = (null == r ? void 0 : r.webuiUrl) && "replica" === r.mode ? `${h}?namespace=${null==r?void 0:r.name}&did=${t}` : void 0;
+                        h = R.URLExt.join(v.baseUrl, s, "open-replication-rule"),
+                        g = (null == d ? void 0 : d.webuiUrl) && "replica" === d.mode ? `${h}?namespace=${null==d?void 0:d.name}&did=${t}` : void 0;
                     return c().createElement("div", {
-                        className: n.container
-                    }, !i && c().createElement("div", {
-                        className: n.loading
+                        className: a.container
+                    }, !r && c().createElement("div", {
+                        className: a.loading
                     }, c().createElement(M, {
-                        className: `${n.icon} material-icons`
+                        className: `${a.icon} material-icons`
                     }, "hourglass_top"), c().createElement("span", {
-                        className: n.statusText
-                    }, "Loading...")), !!i && "OK" === i.status && i.path && c().createElement(te, {
+                        className: a.statusText
+                    }, "Loading...")), !!r && "OK" === r.status && r.path && c().createElement(te, {
                         did: t,
-                        path: i.path,
+                        path: r.path,
                         showReplicationRuleUrl: g
-                    }), !!i && "NOT_AVAILABLE" === i.status && c().createElement(ae, {
+                    }), !!r && "NOT_AVAILABLE" === r.status && c().createElement(ne, {
                         onMakeAvailableClicked: u
-                    }), !!i && "REPLICATING" === i.status && c().createElement(ne, {
+                    }), !!r && "REPLICATING" === r.status && c().createElement(ae, {
                         did: t,
                         showReplicationRuleUrl: g
-                    }), !!i && "STUCK" === i.status && c().createElement(oe, {
-                        onMakeAvailableClicked: "download" === (null == r ? void 0 : r.mode) ? u : void 0,
+                    }), !!r && "STUCK" === r.status && c().createElement(oe, {
+                        onMakeAvailableClicked: "download" === (null == d ? void 0 : d.mode) ? u : void 0,
                         showReplicationRuleUrl: g
                     }))
                 })));
-            const ie = (0, g.createUseStyles)({
+            const re = (0, g.createUseStyles)({
                     container: {
                         padding: "4px 16px 4px 16px",
                         backgroundColor: "var(--jp-layout-color2)",
                         boxSizing: "border-box",
                         height: "32px",
                         alignItems: "center"
                     },
@@ -873,196 +870,196 @@
                     },
                     action: {
                         fontSize: "9pt",
                         color: "var(--jp-rucio-primary-blue-color)",
                         cursor: "pointer"
                     }
                 }),
-                re = ({
+                ie = ({
                     did: e,
                     showReplicationRuleUrl: t
                 }) => {
-                    const a = ie();
+                    const n = re();
                     return c().createElement("div", {
-                        className: a.statusAvailable
+                        className: n.statusAvailable
                     }, c().createElement("i", {
-                        className: `${a.icon} material-icons`
+                        className: `${n.icon} material-icons`
                     }, "check_circle"), t && c().createElement("div", {
-                        className: a.clickableStatusText
+                        className: n.clickableStatusText
                     }, c().createElement("a", {
                         href: t,
                         target: "_blank",
                         rel: "noreferrer",
                         title: "Show replication rule"
                     }, "All files available")), !t && c().createElement("div", {
-                        className: a.statusText
+                        className: n.statusText
                     }, "All files available"), c().createElement("div", {
-                        className: a.action
+                        className: n.action
                     }, c().createElement(H, {
                         did: e,
                         type: "collection"
                     }, "Add to Notebook")))
                 },
-                se = ({
+                ce = ({
                     onMakeAvailableClicked: e
                 }) => {
-                    const t = ie();
+                    const t = re();
                     return c().createElement("div", {
                         className: t.statusNotAvailable
                     }, c().createElement("i", {
                         className: `${t.icon} material-icons`
                     }, "lens"), c().createElement("div", {
                         className: t.statusText
                     }, "Not available"), c().createElement("div", {
                         className: t.action,
                         onClick: e
                     }, "Make Available"))
                 },
-                ce = ({
+                se = ({
                     onMakeAvailableClicked: e,
                     showReplicationRuleUrl: t
                 }) => {
-                    const a = ie();
+                    const n = re();
                     return c().createElement("div", {
-                        className: a.statusPartiallyAvailable
+                        className: n.statusPartiallyAvailable
                     }, c().createElement("i", {
-                        className: `${a.icon} material-icons`
+                        className: `${n.icon} material-icons`
                     }, "lens"), t && c().createElement("div", {
-                        className: a.clickableStatusText
+                        className: n.clickableStatusText
                     }, c().createElement("a", {
                         href: t,
                         target: "_blank",
                         rel: "noreferrer",
                         title: "Show replication rule"
                     }, "Partially available")), !t && c().createElement("div", {
-                        className: a.statusText
+                        className: n.statusText
                     }, "Partially available"), c().createElement("div", {
-                        className: a.action,
+                        className: n.action,
                         onClick: e
                     }, "Make Available"))
                 },
                 de = ({
                     did: e,
                     showReplicationRuleUrl: t
                 }) => {
-                    const a = ie();
+                    const n = re();
                     return c().createElement("div", {
-                        className: a.statusReplicating
+                        className: n.statusReplicating
                     }, c().createElement(M, {
-                        className: `${a.icon} material-icons`
+                        className: `${n.icon} material-icons`
                     }, "hourglass_top"), t && c().createElement("div", {
-                        className: a.clickableStatusText
+                        className: n.clickableStatusText
                     }, c().createElement("a", {
                         href: t,
                         target: "_blank",
                         rel: "noreferrer",
                         title: "Show replication rule"
                     }, "Replicating files...")), !t && c().createElement("div", {
-                        className: a.statusText
+                        className: n.statusText
                     }, "Replicating files..."), c().createElement("div", {
-                        className: a.action
+                        className: n.action
                     }, c().createElement(H, {
                         did: e,
                         type: "collection"
                     }, "Add to Notebook")))
                 },
                 me = ({
                     onMakeAvailableClicked: e,
                     showReplicationRuleUrl: t
                 }) => {
-                    const a = ie();
+                    const n = re();
                     return c().createElement("div", {
-                        className: a.statusNotAvailable
+                        className: n.statusNotAvailable
                     }, c().createElement("i", {
-                        className: `${a.icon} material-icons`
+                        className: `${n.icon} material-icons`
                     }, "error"), t && c().createElement("div", {
-                        className: a.clickableStatusText
+                        className: n.clickableStatusText
                     }, c().createElement("a", {
                         href: t,
                         target: "_blank",
                         rel: "noreferrer",
                         title: "Show replication rule"
                     }, "Something went wrong")), !t && c().createElement("div", {
-                        className: a.statusText
+                        className: n.statusText
                     }, "Something went wrong"), e && c().createElement("div", {
-                        className: a.action,
+                        className: n.action,
                         onClick: e
                     }, "Make Available"))
                 },
                 pe = () => {
-                    const e = ie();
+                    const e = re();
                     return c().createElement("div", {
                         className: e.statusEmpty
                     }, c().createElement("i", {
                         className: `${e.icon} material-icons`
                     }, "warning"), c().createElement("div", {
                         className: e.statusText
                     }, "Collection is empty"))
                 },
                 ue = Q(B((e => {
                     var {
                         did: t
-                    } = e, a = function(e, t) {
-                        var a = {};
-                        for (var n in e) Object.prototype.hasOwnProperty.call(e, n) && t.indexOf(n) < 0 && (a[n] = e[n]);
+                    } = e, n = function(e, t) {
+                        var n = {};
+                        for (var a in e) Object.prototype.hasOwnProperty.call(e, a) && t.indexOf(a) < 0 && (n[a] = e[a]);
                         if (null != e && "function" == typeof Object.getOwnPropertySymbols) {
                             var o = 0;
-                            for (n = Object.getOwnPropertySymbols(e); o < n.length; o++) t.indexOf(n[o]) < 0 && Object.prototype.propertyIsEnumerable.call(e, n[o]) && (a[n[o]] = e[n[o]])
+                            for (a = Object.getOwnPropertySymbols(e); o < a.length; o++) t.indexOf(a[o]) < 0 && Object.prototype.propertyIsEnumerable.call(e, a[o]) && (n[a[o]] = e[a[o]])
                         }
-                        return a
+                        return n
                     }(e, ["did"]);
-                    const n = ie(),
+                    const a = re(),
                         {
                             actions: o
-                        } = a,
+                        } = n,
                         {
                             didPollingManager: l
-                        } = a,
-                        i = (0, b.useStoreState)(C, (e => e.collectionDetails[t])),
-                        r = (0, b.useStoreState)(C, (e => e.activeInstance)),
-                        [m] = (0, s.useState)((() => new Y)),
+                        } = n,
+                        r = (0, b.useStoreState)(C, (e => e.collectionDetails[t])),
+                        d = (0, b.useStoreState)(C, (e => e.activeInstance)),
+                        [m] = (0, i.useState)((() => new Y)),
                         p = () => {
                             l.requestPolling(t, "collection", m)
                         };
-                    (0, s.useEffect)((() => (p(), () => {
+                    (0, i.useEffect)((() => (p(), () => {
                         l.disablePolling(t, m)
                     })), []);
                     const u = () => {
-                            r && (null == o || o.makeCollectionAvailable(r.name, t).then((() => p())).catch((e => console.log(e))))
+                            d && (null == o || o.makeCollectionAvailable(d.name, t).then((() => p())).catch((e => console.log(e))))
                         },
-                        v = (0, s.useMemo)((() => i ? G(i) : void 0), [i]),
+                        v = (0, i.useMemo)((() => r ? G(r) : void 0), [r]),
                         h = P.ServerConnection.makeSettings(),
-                        g = R.URLExt.join(h.baseUrl, d, "open-replication-rule"),
-                        f = (null == r ? void 0 : r.webuiUrl) && "replica" === r.mode ? `${g}?namespace=${null==r?void 0:r.name}&did=${t}` : void 0;
+                        g = R.URLExt.join(h.baseUrl, s, "open-replication-rule"),
+                        f = (null == d ? void 0 : d.webuiUrl) && "replica" === d.mode ? `${g}?namespace=${null==d?void 0:d.name}&did=${t}` : void 0;
                     return c().createElement("div", {
-                        className: n.container
-                    }, !i && c().createElement("div", {
-                        className: n.loading
+                        className: a.container
+                    }, !r && c().createElement("div", {
+                        className: a.loading
                     }, c().createElement(M, {
-                        className: `${n.icon} material-icons`
+                        className: `${a.icon} material-icons`
                     }, "hourglass_top"), c().createElement("span", {
-                        className: n.statusText
-                    }, "Loading...")), "AVAILABLE" === v && c().createElement(re, {
+                        className: a.statusText
+                    }, "Loading...")), "AVAILABLE" === v && c().createElement(ie, {
                         did: t,
                         showReplicationRuleUrl: f
-                    }), "PARTIALLY_AVAILABLE" === v && c().createElement(ce, {
+                    }), "PARTIALLY_AVAILABLE" === v && c().createElement(se, {
                         onMakeAvailableClicked: u,
                         showReplicationRuleUrl: f
-                    }), "NOT_AVAILABLE" === v && c().createElement(se, {
+                    }), "NOT_AVAILABLE" === v && c().createElement(ce, {
                         onMakeAvailableClicked: u
                     }), "REPLICATING" === v && c().createElement(de, {
                         did: t,
                         showReplicationRuleUrl: f
                     }), "STUCK" === v && c().createElement(me, {
-                        onMakeAvailableClicked: "download" === (null == r ? void 0 : r.mode) ? u : void 0,
+                        onMakeAvailableClicked: "download" === (null == d ? void 0 : d.mode) ? u : void 0,
                         showReplicationRuleUrl: f
                     }), "EMPTY" === v && c().createElement(pe, null))
                 })));
-            var ve = a(2638),
-                he = a.n(ve);
+            var ve = n(2638),
+                he = n.n(ve);
             const ge = (0, g.createUseStyles)({
                     main: {
                         width: "300px",
                         background: "var(--jp-layout-color1)",
                         color: "var(--jp-ui-font-color1)"
                     },
                     heading: {
@@ -1149,92 +1146,92 @@
                         verticalAlign: "middle"
                     }
                 }),
                 fe = ({
                     children: e,
                     did: t
                 }) => {
-                    const a = ge(),
-                        [n, o] = (0, s.useState)(!1),
-                        [l, i] = (0, s.useState)(!1),
-                        [r, d] = (0, s.useState)([]),
+                    const n = ge(),
+                        [a, o] = (0, i.useState)(!1),
+                        [l, r] = (0, i.useState)(!1),
+                        [s, d] = (0, i.useState)([]),
                         m = (0, b.useStoreState)(C, (e => e.activeInstance)),
-                        p = (0, s.useCallback)((e => {
+                        p = (0, i.useCallback)((e => {
                             27 === e.keyCode && o(!1)
                         }), []);
-                    (0, s.useEffect)((() => (document.addEventListener("keydown", p, !1), () => {
+                    (0, i.useEffect)((() => (document.addEventListener("keydown", p, !1), () => {
                         document.removeEventListener("keydown", p, !1)
                     })), []);
                     const u = c().createElement("div", {
-                        className: a.main
+                        className: n.main
                     }, c().createElement("div", {
-                        className: a.heading
+                        className: n.heading
                     }, c().createElement("div", {
-                        className: a.headingText
+                        className: n.headingText
                     }, "Files of ", c().createElement("b", null, t)), c().createElement("i", {
-                        className: `${a.headingCloseButton} material-icons`,
+                        className: `${n.headingCloseButton} material-icons`,
                         onClick: () => o(!1)
                     }, "close")), c().createElement("div", {
-                        className: a.content
+                        className: n.content
                     }, l && c().createElement("div", {
-                        className: a.loading
+                        className: n.loading
                     }, c().createElement(M, {
-                        className: `${a.loadingIcon} material-icons`
+                        className: `${n.loadingIcon} material-icons`
                     }, "hourglass_top"), c().createElement("span", {
-                        className: a.iconText
+                        className: n.iconText
                     }, "Loading...")), c().createElement(k.FixedSizeList, {
-                        height: Math.min(250, 32 * r.length),
-                        itemCount: r.length,
+                        height: Math.min(250, 32 * s.length),
+                        itemCount: s.length,
                         itemSize: 32,
                         width: "100%"
                     }, (({
                         index: e,
                         style: t
                     }) => {
-                        const a = r[e];
+                        const n = s[e];
                         return c().createElement(be, {
                             style: t,
-                            did: a.did,
-                            size: a.size
+                            did: n.did,
+                            size: n.size
                         })
                     }))));
-                    return c().createElement(K(), {
+                    return c().createElement(Z(), {
                         enterExitTransitionDurationMs: 0,
-                        isOpen: n,
+                        isOpen: a,
                         preferPlace: "below",
                         body: u,
                         onOuterAction: () => o(!1)
                     }, c().createElement("div", {
                         onClick: () => {
-                            o(!0), m && (i(!0), d([]), $.fetchAttachedFileDIDs(m.name, t).then((e => d(e))).catch((e => console.log(e))).finally((() => i(!1))))
+                            o(!0), m && (r(!0), d([]), _.fetchAttachedFileDIDs(m.name, t).then((e => d(e))).catch((e => console.log(e))).finally((() => r(!1))))
                         }
                     }, e))
                 },
                 be = ({
                     did: e,
                     size: t,
-                    style: a
+                    style: n
                 }) => {
-                    const n = ge();
+                    const a = ge();
                     return c().createElement("div", {
-                        className: n.listItem,
-                        style: a
+                        className: a.listItem,
+                        style: n
                     }, c().createElement("div", {
-                        className: n.iconContainer
+                        className: a.iconContainer
                     }, c().createElement("i", {
-                        className: `${n.fileIcon} material-icons`
+                        className: `${a.fileIcon} material-icons`
                     }, "attachment")), c().createElement(he(), {
                         text: e
                     }, c().createElement("div", {
-                        className: n.textContainer
+                        className: a.textContainer
                     }, e, " ", c().createElement("i", {
                         className: "material-icons copy"
                     }, "file_copy"))), !!t && c().createElement("div", {
-                        className: n.sizeContainer
-                    }, W(t)))
+                        className: a.sizeContainer
+                    }, q(t)))
                 },
                 Ee = (0, g.createUseStyles)({
                     listItemContainer: {
                         borderBottom: "1px solid var(--jp-border-color2)",
                         overflow: "hidden",
                         boxSizing: "border-box"
                     },
@@ -1290,49 +1287,49 @@
                         color: "#2196F3",
                         cursor: "pointer"
                     }
                 }),
                 xe = ({
                     did: e,
                     size: t,
-                    type: a,
-                    onClick: n,
+                    type: n,
+                    onClick: a,
                     expand: o,
                     style: l
                 }) => {
-                    const i = Ee();
+                    const r = Ee();
                     return c().createElement("div", {
-                        className: i.listItemContainer,
+                        className: r.listItemContainer,
                         style: l
                     }, c().createElement("div", {
-                        className: o ? i.listItemExpanded : i.listItemCollapsed,
-                        onClick: n
+                        className: o ? r.listItemExpanded : r.listItemCollapsed,
+                        onClick: a
                     }, c().createElement("div", {
-                        className: i.iconContainer
-                    }, "file" === a && c().createElement("i", {
-                        className: `${i.fileIcon} material-icons`
-                    }, "attachment"), "container" === a && c().createElement("i", {
-                        className: `${i.containerIcon} material-icons`
-                    }, "folder"), "dataset" === a && c().createElement("i", {
-                        className: `${i.datasetIcon} material-icons`
+                        className: r.iconContainer
+                    }, "file" === n && c().createElement("i", {
+                        className: `${r.fileIcon} material-icons`
+                    }, "attachment"), "container" === n && c().createElement("i", {
+                        className: `${r.containerIcon} material-icons`
+                    }, "folder"), "dataset" === n && c().createElement("i", {
+                        className: `${r.datasetIcon} material-icons`
                     }, "folder_open")), c().createElement("div", {
-                        className: i.textContainer
-                    }, e), "file" === a && !!t && c().createElement("div", {
-                        className: i.sizeContainer
-                    }, W(t)), ("container" === a || "dataset" === a) && c().createElement("div", {
+                        className: r.textContainer
+                    }, e), "file" === n && !!t && c().createElement("div", {
+                        className: r.sizeContainer
+                    }, q(t)), ("container" === n || "dataset" === n) && c().createElement("div", {
                         onClick: e => {
                             e.stopPropagation()
                         }
                     }, c().createElement(fe, {
                         did: e
                     }, c().createElement("i", {
-                        className: `${i.listFilesIcon} material-icons`
-                    }, "visibility")))), !!o && "file" === a && c().createElement(le, {
+                        className: `${r.listFilesIcon} material-icons`
+                    }, "visibility")))), !!o && "file" === n && c().createElement(le, {
                         did: e
-                    }), !!o && ("container" === a || "dataset" === a) && c().createElement(ue, {
+                    }), !!o && ("container" === n || "dataset" === n) && c().createElement(ue, {
                         did: e
                     }))
                 };
             const ye = (0, g.createUseStyles)({
                     dropdown: {
                         position: "relative",
                         display: "inline-block"
@@ -1372,51 +1369,51 @@
                         fontSize: "16px",
                         verticalAlign: "middle"
                     }
                 }),
                 Ce = e => {
                     var {
                         options: t,
-                        value: a,
-                        onItemSelected: n,
+                        value: n,
+                        onItemSelected: a,
                         optionWidth: o
                     } = e, l = function(e, t) {
-                        var a = {};
-                        for (var n in e) Object.prototype.hasOwnProperty.call(e, n) && t.indexOf(n) < 0 && (a[n] = e[n]);
+                        var n = {};
+                        for (var a in e) Object.prototype.hasOwnProperty.call(e, a) && t.indexOf(a) < 0 && (n[a] = e[a]);
                         if (null != e && "function" == typeof Object.getOwnPropertySymbols) {
                             var o = 0;
-                            for (n = Object.getOwnPropertySymbols(e); o < n.length; o++) t.indexOf(n[o]) < 0 && Object.prototype.propertyIsEnumerable.call(e, n[o]) && (a[n[o]] = e[n[o]])
+                            for (a = Object.getOwnPropertySymbols(e); o < a.length; o++) t.indexOf(a[o]) < 0 && Object.prototype.propertyIsEnumerable.call(e, a[o]) && (n[a[o]] = e[a[o]])
                         }
-                        return a
+                        return n
                     }(e, ["options", "value", "onItemSelected", "optionWidth"]);
-                    const i = ye({
+                    const r = ye({
                             optionWidth: o
                         }),
-                        [r, d] = (0, s.useState)(!1),
-                        m = t.find((e => e.value === a)),
-                        p = (0, s.useRef)(null),
+                        [s, d] = (0, i.useState)(!1),
+                        m = t.find((e => e.value === n)),
+                        p = (0, i.useRef)(null),
                         u = e => {
                             var t;
                             p && !(null === (t = p.current) || void 0 === t ? void 0 : t.contains(e.target)) && d(!1)
                         };
-                    return (0, s.useEffect)((() => (document.addEventListener("mousedown", u), () => {
+                    return (0, i.useEffect)((() => (document.addEventListener("mousedown", u), () => {
                         document.removeEventListener("mousedown", u)
                     }))), c().createElement("span", {
-                        className: i.dropdown,
-                        onClick: () => d(!r),
+                        className: r.dropdown,
+                        onClick: () => d(!s),
                         ref: p
                     }, c().createElement("span", Object.assign({
-                        className: i.dropdownTitle
+                        className: r.dropdownTitle
                     }, l), m ? m.title : "(select)", c().createElement("span", {
-                        className: `${i.icon} material-icons`
+                        className: `${r.icon} material-icons`
                     }, "arrow_drop_down")), c().createElement("div", {
-                        className: r ? i.dropdownActive : i.dropdownContent
+                        className: s ? r.dropdownActive : r.dropdownContent
                     }, t.map((e => c().createElement("div", {
-                        className: i.dropdownListItem,
-                        onClick: () => n && n(e.value),
+                        className: r.dropdownListItem,
+                        onClick: () => a && a(e.value),
                         key: e.value
                     }, e.title)))))
                 },
                 Ne = (0, g.createUseStyles)({
                     main: {
                         width: "300px",
                         background: "var(--jp-layout-color1)",
@@ -1503,90 +1500,90 @@
                         verticalAlign: "middle"
                     }
                 }),
                 Ie = ({
                     children: e,
                     onScopeClicked: t
                 }) => {
-                    const a = Ne(),
-                        [n, o] = (0, s.useState)(!1),
-                        [l, i] = (0, s.useState)(!1),
-                        [r, d] = (0, s.useState)([]),
+                    const n = Ne(),
+                        [a, o] = (0, i.useState)(!1),
+                        [l, r] = (0, i.useState)(!1),
+                        [s, d] = (0, i.useState)([]),
                         m = (0, b.useStoreState)(C, (e => e.activeInstance)),
-                        p = (0, s.useCallback)((e => {
+                        p = (0, i.useCallback)((e => {
                             27 === e.keyCode && o(!1)
                         }), []);
-                    (0, s.useEffect)((() => (document.addEventListener("keydown", p, !1), () => {
+                    (0, i.useEffect)((() => (document.addEventListener("keydown", p, !1), () => {
                         document.removeEventListener("keydown", p, !1)
                     })), []);
                     const u = c().createElement("div", {
-                        className: a.main
+                        className: n.main
                     }, c().createElement("div", {
-                        className: a.heading
+                        className: n.heading
                     }, c().createElement("div", {
-                        className: a.headingText
+                        className: n.headingText
                     }, "Available scopes"), c().createElement("i", {
-                        className: `${a.headingCloseButton} material-icons`,
+                        className: `${n.headingCloseButton} material-icons`,
                         onClick: () => o(!1)
                     }, "close")), c().createElement("div", {
-                        className: a.content
-                    }, l && 0 === r.length && c().createElement("div", {
-                        className: a.loading
+                        className: n.content
+                    }, l && 0 === s.length && c().createElement("div", {
+                        className: n.loading
                     }, c().createElement(M, {
-                        className: `${a.loadingIcon} material-icons`
+                        className: `${n.loadingIcon} material-icons`
                     }, "hourglass_top"), c().createElement("span", {
-                        className: a.iconText
+                        className: n.iconText
                     }, "Loading...")), c().createElement(k.FixedSizeList, {
-                        height: Math.min(250, 32 * r.length),
-                        itemCount: r.length,
+                        height: Math.min(250, 32 * s.length),
+                        itemCount: s.length,
                         itemSize: 32,
                         width: "100%"
                     }, (({
                         index: e,
-                        style: a
+                        style: n
                     }) => {
-                        const n = r[e];
+                        const a = s[e];
                         return c().createElement(Se, {
-                            style: a,
-                            scope: n,
+                            style: n,
+                            scope: a,
                             onClick: () => (e => {
                                 o(!1), null == t || t(e)
-                            })(n)
+                            })(a)
                         })
                     }))));
-                    return c().createElement(K(), {
+                    return c().createElement(Z(), {
                         enterExitTransitionDurationMs: 0,
-                        isOpen: n,
+                        isOpen: a,
                         preferPlace: "below",
                         body: u,
                         onOuterAction: () => o(!1)
                     }, c().createElement("div", {
                         onClick: () => {
-                            o(!0), m && (i(!0), $.fetchScopes(m.name).then((e => {
+                            o(!0), m && (r(!0), _.fetchScopes(m.name).then((e => {
                                 e.sort(((e, t) => e.localeCompare(t))), d(e)
-                            })).catch((e => console.log(e))).finally((() => i(!1))))
+                            })).catch((e => console.log(e))).finally((() => r(!1))))
                         }
                     }, e))
                 },
                 Se = ({
                     scope: e,
                     style: t,
-                    onClick: a
+                    onClick: n
                 }) => {
-                    const n = Ne();
+                    const a = Ne();
                     return c().createElement("div", {
-                        className: n.listItem,
+                        className: a.listItem,
                         style: t
                     }, c().createElement("div", {
-                        className: n.iconContainer
+                        className: a.iconContainer
                     }, c().createElement("i", {
-                        className: `${n.scopeIcon} material-icons`
+                        className: `${a.scopeIcon} material-icons`
                     }, "topic")), c().createElement("div", {
-                        className: n.textContainer,
-                        onClick: a
+                        className: a.textContainer,
+                        onClick: n
                     }, e))
                 },
                 ke = (0, g.createUseStyles)({
                     mainContainer: {
                         height: "100%",
                         display: "flex",
                         flexDirection: "column",
@@ -1662,116 +1659,116 @@
                 }, {
                     title: "Files",
                     value: "file"
                 }],
                 je = B((e => {
                     const t = ke(),
                         {
-                            actions: a
+                            actions: n
                         } = e,
-                        [n, o] = (0, s.useState)(""),
-                        [l, i] = (0, s.useState)("all"),
-                        [r, d] = (0, s.useState)(),
-                        [m, p] = (0, s.useState)({}),
-                        [u, v] = (0, s.useState)(),
-                        [h, g] = (0, s.useState)(""),
-                        [f, E] = (0, s.useState)(!1),
+                        [a, o] = (0, i.useState)(""),
+                        [l, r] = (0, i.useState)("all"),
+                        [s, d] = (0, i.useState)(),
+                        [m, p] = (0, i.useState)({}),
+                        [u, v] = (0, i.useState)(),
+                        [h, g] = (0, i.useState)(""),
+                        [f, E] = (0, i.useState)(!1),
                         x = (0, b.useStoreState)(C, (e => e.activeInstance)),
                         y = (e, t) => e.type === t.type ? e.did.toLowerCase() < t.did.toLowerCase() ? -1 : 1 : "container" === e.type && "dataset" === t.type ? -1 : "container" !== e.type && "dataset" !== e.type || "file" !== t.type ? 1 : -1;
-                    (0, s.useEffect)((() => {
-                        h && x && (E(!0), d(void 0), p({}), v(void 0), a.searchDID(x.name, n, l).then((e => e.sort(y))).then((e => d(e))).catch((e => {
+                    (0, i.useEffect)((() => {
+                        h && x && (E(!0), d(void 0), p({}), v(void 0), n.searchDID(x.name, a, l).then((e => e.sort(y))).then((e => d(e))).catch((e => {
                             d([]), 401 !== e.response.status ? 400 === e.response.status && v("Wildcard search is disabled.") : v("Authentication error. Perhaps you set an invalid credential?")
                         })).finally((() => E(!1))))
                     }), [h, l]);
-                    const N = (0, s.useRef)(null),
+                    const N = (0, i.useRef)(null),
                         I = c().createElement(Ie, {
                             onScopeClicked: e => {
                                 var t;
                                 o(e + ":"), null === (t = null == N ? void 0 : N.current) || void 0 === t || t.focus()
                             }
                         }, c().createElement("div", {
                             className: t.listScopesButton
                         }, c().createElement("i", {
                             className: `${t.listScopesIcon} material-icons`
                         }, "topic"))),
                         S = c().createElement("div", {
                             className: t.searchButton,
-                            onClick: () => g(n)
+                            onClick: () => g(a)
                         }, c().createElement("i", {
                             className: `${t.searchIcon} material-icons`
                         }, "search")),
-                        w = (0, s.useRef)(null),
-                        L = e => !0 === m[e] ? 64 : 32,
+                        w = (0, i.useRef)(null),
+                        A = e => !0 === m[e] ? 64 : 32,
                         O = ({
                             index: e,
                             style: t
                         }) => {
-                            if (!r) return c().createElement(c().Fragment, null);
-                            const a = r[e],
-                                n = !!m[e];
+                            if (!s) return c().createElement(c().Fragment, null);
+                            const n = s[e],
+                                a = !!m[e];
                             return c().createElement(xe, {
                                 style: t,
-                                type: a.type,
-                                did: a.did,
-                                size: a.size,
-                                key: a.did,
-                                expand: n,
+                                type: n.type,
+                                did: n.did,
+                                size: n.size,
+                                key: n.did,
+                                expand: a,
                                 onClick: () => (e => {
                                     var t;
                                     null === (t = w.current) || void 0 === t || t.resetAfterIndex(e), m[e] = !m[e], p(m)
                                 })(e)
                             })
                         };
                     return c().createElement("div", {
                         className: t.mainContainer
                     }, c().createElement("div", {
                         className: t.searchContainer
-                    }, c().createElement(A, {
+                    }, c().createElement(L, {
                         placeholder: "Enter a Data Identifier (DID)",
                         after: [I, S],
-                        value: n,
+                        value: a,
                         onChange: e => o(e.target.value),
                         onKeyPress: e => {
-                            "Enter" === e.key && g(n)
+                            "Enter" === e.key && g(a)
                         },
                         autoComplete: "off",
                         ref: N
                     })), c().createElement("div", {
                         className: t.filterContainer
                     }, "Search", c().createElement(Ce, {
                         className: t.dropdown,
                         options: we,
                         value: l,
-                        onItemSelected: i,
+                        onItemSelected: r,
                         optionWidth: "180px"
                     })), f && c().createElement("div", {
                         className: t.loading
                     }, c().createElement(M, {
                         className: `${t.icon} material-icons`
                     }, "hourglass_top"), c().createElement("span", {
                         className: t.iconText
-                    }, "Loading...")), !!r && c().createElement(c().Fragment, null, c().createElement(D, {
+                    }, "Loading...")), !!s && c().createElement(c().Fragment, null, c().createElement(D, {
                         title: "Search Results"
-                    }), (!!r && 0 === r.length || !!u) && c().createElement("div", {
+                    }), (!!s && 0 === s.length || !!u) && c().createElement("div", {
                         className: t.loading
                     }, u || "No results found"), c().createElement("div", {
                         className: t.resultsContainer
                     }, c().createElement(j(), {
                         disableWidth: !0
                     }, (({
                         height: e
                     }) => c().createElement(k.VariableSizeList, {
                         ref: w,
                         height: e,
-                        itemCount: r.length,
-                        itemSize: L,
+                        itemCount: s.length,
+                        itemSize: A,
                         width: "100%"
                     }, O))))))
                 }));
-            const Le = (0, g.createUseStyles)({
+            const Ae = (0, g.createUseStyles)({
                     listItemContainer: {
                         display: "flex",
                         flexDirection: "row",
                         borderBottom: "1px solid var(--jp-border-color2)",
                         padding: "8px 16px 8px 16px",
                         fontSize: "9pt"
                     },
@@ -1837,18 +1834,18 @@
                     },
                     action: {
                         fontSize: "9pt",
                         color: "var(--jp-rucio-primary-blue-color)",
                         cursor: "pointer"
                     }
                 }),
-                Ae = ({
+                Le = ({
                     status: e
                 }) => {
-                    const t = Le();
+                    const t = Ae();
                     switch (e) {
                         case "RESOLVING":
                             return c().createElement(M, {
                                 className: `${t.statusIcon} material-icons`
                             }, "hourglass_top");
                         case "PENDING_INJECTION":
                             return c().createElement("i", {
@@ -1868,121 +1865,121 @@
                             }, "lens")
                     }
                 },
                 Oe = ({
                     status: e,
                     resolverStatus: t
                 }) => {
-                    const a = Le();
+                    const n = Ae();
                     switch (e) {
                         case "REPLICATING":
                             return c().createElement(M, {
-                                className: `${a.replicatingIcon} material-icons`
+                                className: `${n.replicatingIcon} material-icons`
                             }, "hourglass_top");
                         case "NOT_AVAILABLE":
                         case "STUCK":
                             return c().createElement("i", {
-                                className: `${a.notAvailableIcon} material-icons`
+                                className: `${n.notAvailableIcon} material-icons`
                             }, "lens");
                         default:
-                            return c().createElement(Ae, {
+                            return c().createElement(Le, {
                                 status: t
                             })
                     }
                 },
                 De = ({
                     status: e,
                     resolverStatus: t
                 }) => {
-                    const a = Le();
+                    const n = Ae();
                     switch (e) {
                         case "REPLICATING":
                             return c().createElement(M, {
-                                className: `${a.replicatingIcon} material-icons`
+                                className: `${n.replicatingIcon} material-icons`
                             }, "hourglass_top");
                         case "NOT_AVAILABLE":
                         case "STUCK":
                         case "PARTIALLY_AVAILABLE":
                             return c().createElement("i", {
-                                className: `${a.notAvailableIcon} material-icons`
+                                className: `${n.notAvailableIcon} material-icons`
                             }, "lens");
                         default:
-                            return c().createElement(Ae, {
+                            return c().createElement(Le, {
                                 status: t
                             })
                     }
                 },
                 Re = B((e => {
                     var {
                         attachment: t,
-                        status: a
-                    } = e, n = function(e, t) {
-                        var a = {};
-                        for (var n in e) Object.prototype.hasOwnProperty.call(e, n) && t.indexOf(n) < 0 && (a[n] = e[n]);
+                        status: n
+                    } = e, a = function(e, t) {
+                        var n = {};
+                        for (var a in e) Object.prototype.hasOwnProperty.call(e, a) && t.indexOf(a) < 0 && (n[a] = e[a]);
                         if (null != e && "function" == typeof Object.getOwnPropertySymbols) {
                             var o = 0;
-                            for (n = Object.getOwnPropertySymbols(e); o < n.length; o++) t.indexOf(n[o]) < 0 && Object.prototype.propertyIsEnumerable.call(e, n[o]) && (a[n[o]] = e[n[o]])
+                            for (a = Object.getOwnPropertySymbols(e); o < a.length; o++) t.indexOf(a[o]) < 0 && Object.prototype.propertyIsEnumerable.call(e, a[o]) && (n[a[o]] = e[a[o]])
                         }
-                        return a
+                        return n
                     }(e, ["attachment", "status"]);
-                    const o = Le(),
+                    const o = Ae(),
                         {
                             actions: l
-                        } = n,
+                        } = a,
                         {
-                            did: i,
-                            type: r
+                            did: r,
+                            type: s
                         } = t,
-                        d = (0, b.useStoreState)(C, (e => e.fileDetails[i])),
-                        m = (0, b.useStoreState)(C, (e => e.collectionDetails[i])),
+                        d = (0, b.useStoreState)(C, (e => e.fileDetails[r])),
+                        m = (0, b.useStoreState)(C, (e => e.collectionDetails[r])),
                         p = (0, b.useStoreState)(C, (e => e.activeInstance));
-                    (0, s.useEffect)((() => {
-                        p && ("file" === r ? l.getFileDIDDetails(p.name, i) : l.getCollectionDIDDetails(p.name, i))
+                    (0, i.useEffect)((() => {
+                        p && ("file" === s ? l.getFileDIDDetails(p.name, r) : l.getCollectionDIDDetails(p.name, r))
                     }), []);
-                    const u = (0, s.useMemo)((() => m ? G(m) : void 0), [m]),
+                    const u = (0, i.useMemo)((() => m ? G(m) : void 0), [m]),
                         v = (() => {
                             const e = "download" === (null == p ? void 0 : p.mode);
-                            return "file" === r ? "NOT_AVAILABLE" === (null == d ? void 0 : d.status) || "STUCK" === (null == d ? void 0 : d.status) && e : "collection" === r && ("NOT_AVAILABLE" === u || "PARTIALLY_AVAILABLE" === u || "STUCK" === u && e)
+                            return "file" === s ? "NOT_AVAILABLE" === (null == d ? void 0 : d.status) || "STUCK" === (null == d ? void 0 : d.status) && e : "collection" === s && ("NOT_AVAILABLE" === u || "PARTIALLY_AVAILABLE" === u || "STUCK" === u && e)
                         })();
                     return c().createElement("div", {
                         className: o.listItemContainer
                     }, c().createElement("div", {
                         className: o.listItemIconContainer
-                    }, !d && !m && c().createElement(Ae, {
-                        status: a
-                    }), !!d && "file" === r && c().createElement(Oe, {
+                    }, !d && !m && c().createElement(Le, {
+                        status: n
+                    }), !!d && "file" === s && c().createElement(Oe, {
                         status: d.status,
-                        resolverStatus: a
-                    }), !!u && "collection" === r && c().createElement(De, {
+                        resolverStatus: n
+                    }), !!u && "collection" === s && c().createElement(De, {
                         status: u,
-                        resolverStatus: a
+                        resolverStatus: n
                     })), c().createElement("div", {
                         className: o.listItemContent
                     }, c().createElement("div", {
                         className: o.did
                     }, t.did), c().createElement("div", {
                         className: o.variableName
                     }, t.variableName), v && c().createElement("div", {
                         className: o.action,
                         onClick: () => {
                             if (!p) return;
                             const {
                                 did: e,
-                                type: a
+                                type: n
                             } = t;
-                            "file" === a ? l.makeFileAvailable(p.name, e) : l.makeCollectionAvailable(p.name, e)
+                            "file" === n ? l.makeFileAvailable(p.name, e) : l.makeCollectionAvailable(p.name, e)
                         }
                     }, "Make Available")), c().createElement("div", {
                         className: o.actionContainer
                     }, c().createElement("div", {
                         className: o.clearButton,
                         onClick: () => {
-                            Z.update((e => {
+                            V.update((e => {
                                 var t;
-                                e.activeNotebookAttachment = null === (t = e.activeNotebookAttachment) || void 0 === t ? void 0 : t.filter((e => e.did !== i))
+                                e.activeNotebookAttachment = null === (t = e.activeNotebookAttachment) || void 0 === t ? void 0 : t.filter((e => e.did !== r))
                             }))
                         }
                     }, c().createElement("i", {
                         className: `${o.clearIcon} material-icons`
                     }, "clear"))))
                 })),
                 Pe = (0, g.createUseStyles)({
@@ -2034,31 +2031,31 @@
                         color: "#c0ca33"
                     }
                 }),
                 Te = ({
                     notebookPanel: e,
                     onClick: t
                 }) => {
-                    const a = Pe(),
-                        n = Ue()[e.id],
-                        o = n ? Object.keys(n).map((e => n[e])) : null,
-                        l = (0, s.useMemo)((() => (e => e ? 0 === e.length ? "NOT_RESOLVED" : e.includes("FAILED") ? "FAILED" : e.includes("NOT_RESOLVED") ? "NOT_RESOLVED" : e.includes("RESOLVING") ? "RESOLVING" : e.includes("PENDING_INJECTION") ? "PENDING_INJECTION" : "READY" : null)(o)), [n]);
+                    const n = Pe(),
+                        a = $e()[e.id],
+                        o = a ? Object.keys(a).map((e => a[e])) : null,
+                        l = (0, i.useMemo)((() => (e => e ? 0 === e.length ? "NOT_RESOLVED" : e.includes("FAILED") ? "FAILED" : e.includes("NOT_RESOLVED") ? "NOT_RESOLVED" : e.includes("RESOLVING") ? "RESOLVING" : e.includes("PENDING_INJECTION") ? "PENDING_INJECTION" : "READY" : null)(o)), [a]);
                     return c().createElement(c().Fragment, null, !!l && c().createElement("div", {
-                        className: a.main,
+                        className: n.main,
                         onClick: t
                     }, c().createElement(Me, {
                         status: l
                     }), "NOT_RESOLVED" === l && c().createElement("span", null, "Attach Variables"), "FAILED" === l && c().createElement("span", {
-                        className: a.failed
+                        className: n.failed
                     }, "Failed to Attach"), "RESOLVING" === l && c().createElement("span", {
-                        className: a.resolving
+                        className: n.resolving
                     }, "Resolving"), "PENDING_INJECTION" === l && c().createElement("span", {
-                        className: a.injecting
+                        className: n.injecting
                     }, "Attaching"), "READY" === l && c().createElement("span", {
-                        className: a.ready
+                        className: n.ready
                     }, "Ready")))
                 },
                 Me = ({
                     status: e
                 }) => {
                     const t = Pe();
                     switch (e) {
@@ -2098,202 +2095,202 @@
                     } = this.options;
                     return c().createElement(Te, {
                         notebookPanel: e,
                         onClick: t
                     })
                 }
             }
-            const _e = new b.Store({
+            const ze = new b.Store({
                 status: {}
             });
 
-            function Ue() {
-                return (0, b.useStoreState)(_e, (e => e.status))
+            function $e() {
+                return (0, b.useStoreState)(ze, (e => e.status))
             }
-            class ze {
+            class Ue {
                 constructor(e) {
                     this.kernelNotebookMapping = {}, this.options = e, this.setup()
                 }
                 setup() {
                     const {
                         notebookTracker: e
                     } = this.options, t = () => {
-                        _e.update((e => {
+                        ze.update((e => {
                             e.status = {}
                         })), e.forEach((e => this.reinject(e)))
                     };
                     C.subscribe((e => e.activeInstance), (e => {
                         e && t()
                     })), e.widgetAdded.connect(this.onNotebookOpened, this)
                 }
                 onNotebookOpened(e, t) {
-                    t.sessionContext.statusChanged.connect(((e, a) => {
-                        var n;
-                        if ("restarting" === a) {
-                            const a = null === (n = e.session) || void 0 === n ? void 0 : n.kernel;
-                            a && this.onKernelRestarted(t, a), t.sessionContext.ready.then((() => {
-                                a && this.onKernelAttached(t, a)
+                    t.sessionContext.statusChanged.connect(((e, n) => {
+                        var a;
+                        if ("restarting" === n) {
+                            const n = null === (a = e.session) || void 0 === a ? void 0 : a.kernel;
+                            n && this.onKernelRestarted(t, n), t.sessionContext.ready.then((() => {
+                                n && this.onKernelAttached(t, n)
                             }))
                         }
-                    })), t.sessionContext.kernelChanged.connect(((e, a) => {
-                        const n = a.oldValue;
-                        n && this.onKernelDetached(t, n);
-                        const o = a.newValue;
+                    })), t.sessionContext.kernelChanged.connect(((e, n) => {
+                        const a = n.oldValue;
+                        a && this.onKernelDetached(t, a);
+                        const o = n.newValue;
                         o && t.sessionContext.ready.then((() => {
                             this.onKernelAttached(t, o)
                         }))
                     })), this.insertInjectButton(t)
                 }
                 insertInjectButton(e) {
                     const t = new Fe({
                         notebookPanel: e,
                         onClick: () => {
-                            var t, a;
-                            (null === (a = null === (t = e.sessionContext) || void 0 === t ? void 0 : t.session) || void 0 === a ? void 0 : a.kernel) && this.reinject(e)
+                            var t, n;
+                            (null === (n = null === (t = e.sessionContext) || void 0 === t ? void 0 : t.session) || void 0 === n ? void 0 : n.kernel) && this.reinject(e)
                         }
                     });
                     e.toolbar.insertAfter("spacer", "InjectButton", t)
                 }
                 onKernelRestarted(e, t) {
                     this.clearKernelResolverStatus(t.id)
                 }
                 onKernelDetached(e, t) {
                     this.clearKernelResolverStatus(t.id), this.deleteKernelNotebookMapping(t.id)
                 }
                 onKernelAttached(e, t) {
                     this.setKernelNotebookMapping(t.id, e.id), this.setupKernelReceiverComm(t);
-                    const a = this.getAttachmentsFromMetadata(e);
-                    this.injectAttachments(t, a)
+                    const n = this.getAttachmentsFromMetadata(e);
+                    this.injectAttachments(t, n)
                 }
                 clearKernelResolverStatus(e) {
                     const t = this.getNotebookIdFromKernelConnectionId(e);
-                    _e.update((e => {
+                    ze.update((e => {
                         e.status[t] = {}
                     }))
                 }
                 setupKernelReceiverComm(e) {
-                    e.registerCommTarget(u, ((t, a) => {
-                        t.onMsg = a => {
-                            this.processIncomingMessage(e, t, a)
-                        }, this.processIncomingMessage(e, t, a)
+                    e.registerCommTarget(p, ((t, n) => {
+                        t.onMsg = n => {
+                            this.processIncomingMessage(e, t, n)
+                        }, this.processIncomingMessage(e, t, n)
                     }))
                 }
-                processIncomingMessage(e, t, a) {
-                    if ("request-inject" === a.content.data.action) {
+                processIncomingMessage(e, t, n) {
+                    if ("request-inject" === n.content.data.action) {
                         const {
-                            activeInstance: a
-                        } = C.getRawState(), n = this.getNotebookIdFromKernelConnectionId(e.id), {
+                            activeInstance: n
+                        } = C.getRawState(), a = this.getNotebookIdFromKernelConnectionId(e.id), {
                             notebookTracker: o
-                        } = this.options, l = o.find((e => e.id === n));
-                        if (!l || !a) return;
-                        const i = this.getAttachmentsFromMetadata(l);
-                        this.resolveAttachments(i, e.id).then((a => t.send({
+                        } = this.options, l = o.find((e => e.id === a));
+                        if (!l || !n) return;
+                        const r = this.getAttachmentsFromMetadata(l);
+                        this.resolveAttachments(r, e.id).then((n => t.send({
                             action: "inject",
-                            dids: a
+                            dids: n
                         }).done.then((() => {
-                            a.forEach((t => this.setResolveStatus(e.id, t.did, "READY")))
+                            n.forEach((t => this.setResolveStatus(e.id, t.did, "READY")))
                         })).catch((t => {
-                            console.error(t), a.forEach((t => this.setResolveStatus(e.id, t.did, "FAILED")))
+                            console.error(t), n.forEach((t => this.setResolveStatus(e.id, t.did, "FAILED")))
                         }))))
                     }
                 }
                 injectUninjected(e) {
-                    var t, a;
-                    const n = this.getAttachmentsFromMetadata(e),
-                        o = null === (a = null === (t = e.sessionContext) || void 0 === t ? void 0 : t.session) || void 0 === a ? void 0 : a.kernel;
-                    o && (this.injectUninjectedAttachments(o, n), this.removeNonExistentInjectedAttachments(null == o ? void 0 : o.id, n))
+                    var t, n;
+                    const a = this.getAttachmentsFromMetadata(e),
+                        o = null === (n = null === (t = e.sessionContext) || void 0 === t ? void 0 : t.session) || void 0 === n ? void 0 : n.kernel;
+                    o && (this.injectUninjectedAttachments(o, a), this.removeNonExistentInjectedAttachments(null == o ? void 0 : o.id, a))
                 }
                 reinject(e) {
-                    var t, a;
-                    const n = this.getAttachmentsFromMetadata(e),
-                        o = null === (a = null === (t = e.sessionContext) || void 0 === t ? void 0 : t.session) || void 0 === a ? void 0 : a.kernel;
-                    o && this.injectAttachments(o, n)
+                    var t, n;
+                    const a = this.getAttachmentsFromMetadata(e),
+                        o = null === (n = null === (t = e.sessionContext) || void 0 === t ? void 0 : t.session) || void 0 === n ? void 0 : n.kernel;
+                    o && this.injectAttachments(o, a)
                 }
                 reinjectSpecificDID(e, t) {
-                    var a, n;
+                    var n, a;
                     const o = this.getAttachmentsFromMetadata(e).find((e => e.did === t)),
-                        l = null === (n = null === (a = e.sessionContext) || void 0 === a ? void 0 : a.session) || void 0 === n ? void 0 : n.kernel;
+                        l = null === (a = null === (n = e.sessionContext) || void 0 === n ? void 0 : n.session) || void 0 === a ? void 0 : a.kernel;
                     l && o && this.injectAttachments(l, [o])
                 }
                 getAttachmentsFromMetadata(e) {
-                    var t, a;
-                    return null !== (a = null === (t = e.model) || void 0 === t ? void 0 : t.metadata.get(m)) && void 0 !== a ? a : []
+                    var t, n;
+                    return null !== (n = null === (t = e.model) || void 0 === t ? void 0 : t.metadata.get(d)) && void 0 !== n ? n : []
                 }
                 injectUninjectedAttachments(e, t) {
-                    const a = null == e ? void 0 : e.id,
-                        n = this.getNotebookIdFromKernelConnectionId(a),
-                        o = _e.getRawState().status[n] || {},
+                    const n = null == e ? void 0 : e.id,
+                        a = this.getNotebookIdFromKernelConnectionId(n),
+                        o = ze.getRawState().status[a] || {},
                         l = t.filter((e => !o[e.did]));
                     this.injectAttachments(e, l)
                 }
                 removeNonExistentInjectedAttachments(e, t) {
-                    const a = this.getNotebookIdFromKernelConnectionId(e);
-                    _e.update((e => {
-                        const n = e.status[a];
-                        n && Object.keys(n).filter((e => !t.find((t => t.did === e)))).forEach((t => delete e.status[a][t]))
+                    const n = this.getNotebookIdFromKernelConnectionId(e);
+                    ze.update((e => {
+                        const a = e.status[n];
+                        a && Object.keys(a).filter((e => !t.find((t => t.did === e)))).forEach((t => delete e.status[n][t]))
                     }))
                 }
                 injectAttachments(e, t) {
                     this.isExtensionProperlySetup() && t && this.resolveAttachments(t, e.id).then((t => this.injectVariables(e, t))).then((() => {
                         t.forEach((t => this.setResolveStatus(e.id, t.did, "READY")))
-                    })).catch((a => {
-                        console.error(a), t.forEach((t => this.setResolveStatus(e.id, t.did, "FAILED")))
+                    })).catch((n => {
+                        console.error(n), t.forEach((t => this.setResolveStatus(e.id, t.did, "FAILED")))
                     }))
                 }
                 injectVariables(e, t) {
                     if (0 === t.length) return Promise.resolve();
-                    const a = e.createComm(p);
-                    return a.open().done.then((() => a.send({
+                    const n = e.createComm(m);
+                    return n.open().done.then((() => n.send({
                         action: "inject",
                         dids: t
-                    }).done)).then((() => a.close().done))
+                    }).done)).then((() => n.close().done))
                 }
                 async resolveAttachments(e, t) {
-                    const a = e.map((e => this.resolveAttachment(e, t)));
-                    return Promise.all(a)
+                    const n = e.map((e => this.resolveAttachment(e, t)));
+                    return Promise.all(n)
                 }
                 async resolveAttachment(e, t) {
                     const {
-                        variableName: a,
-                        type: n,
+                        variableName: n,
+                        type: a,
                         did: o
                     } = e;
                     this.setResolveStatus(t, o, "RESOLVING");
                     try {
-                        if ("collection" === n) {
+                        if ("collection" === a) {
                             const e = await this.resolveCollectionDIDDetails(o),
-                                n = this.getCollectionFiles(e);
+                                a = this.getCollectionFiles(e);
                             this.setResolveStatus(t, o, "PENDING_INJECTION");
                             return {
                                 type: "collection",
-                                variableName: a,
-                                files: n,
+                                variableName: n,
+                                files: a,
                                 did: o,
                                 didAvailable: "AVAILABLE" === G(e)
                             }
                         } {
                             const e = await this.resolveFileDIDDetails(o),
-                                n = this.getFile(e);
+                                a = this.getFile(e);
                             this.setResolveStatus(t, o, "PENDING_INJECTION");
                             return {
                                 type: "file",
-                                variableName: a,
-                                files: n ? [n] : null,
+                                variableName: n,
+                                files: a ? [a] : null,
                                 did: o,
                                 didAvailable: "OK" === e.status
                             }
                         }
                     } catch (e) {
                         throw this.setResolveStatus(t, o, "FAILED"), e
                     }
                 }
-                setResolveStatus(e, t, a) {
-                    const n = this.getNotebookIdFromKernelConnectionId(e);
-                    _e.update((e => {
-                        e.status[n] || (e.status[n] = {}), e.status[n][t] = a
+                setResolveStatus(e, t, n) {
+                    const a = this.getNotebookIdFromKernelConnectionId(e);
+                    ze.update((e => {
+                        e.status[a] || (e.status[a] = {}), e.status[a][t] = n
                     }))
                 }
                 getCollectionFiles(e) {
                     return e.map((e => this.getFile(e))).filter((e => !!e))
                 }
                 getFile(e) {
                     return e.path ? {
@@ -2302,22 +2299,22 @@
                     } : null
                 }
                 async resolveFileDIDDetails(e) {
                     const {
                         activeInstance: t
                     } = C.getRawState();
                     if (!t) throw new Error("activeInstance cannot be empty");
-                    return $.getFileDIDDetails(t.name, e)
+                    return _.getFileDIDDetails(t.name, e)
                 }
                 async resolveCollectionDIDDetails(e) {
                     const {
                         activeInstance: t
                     } = C.getRawState();
                     if (!t) throw new Error("activeInstance cannot be empty");
-                    return $.getCollectionDIDDetails(t.name, e)
+                    return _.getCollectionDIDDetails(t.name, e)
                 }
                 getNotebookIdFromKernelConnectionId(e) {
                     return this.kernelNotebookMapping[e]
                 }
                 setKernelNotebookMapping(e, t) {
                     this.kernelNotebookMapping[e] = t
                 }
@@ -2327,45 +2324,45 @@
                 isExtensionProperlySetup() {
                     const {
                         activeInstance: e
                     } = C.getRawState();
                     return !!e
                 }
             }
-            const $e = (0, g.createUseStyles)({
+            const _e = (0, g.createUseStyles)({
                     container: {
                         padding: "16px 0 16px 0"
                     },
                     messageContainer: {
                         padding: "16px"
                     }
                 }),
                 Be = () => {
-                    const e = $e(),
-                        t = (0, b.useStoreState)(Z, (e => e.activeNotebookPanel)),
-                        a = (0, b.useStoreState)(Z, (e => e.activeNotebookAttachment)),
-                        n = Ue(),
-                        o = (null == t ? void 0 : t.id) ? n[null == t ? void 0 : t.id] : null;
-                    return c().createElement(c().Fragment, null, !!t && !!a && a.length > 0 && c().createElement("div", {
+                    const e = _e(),
+                        t = (0, b.useStoreState)(V, (e => e.activeNotebookPanel)),
+                        n = (0, b.useStoreState)(V, (e => e.activeNotebookAttachment)),
+                        a = $e(),
+                        o = (null == t ? void 0 : t.id) ? a[null == t ? void 0 : t.id] : null;
+                    return c().createElement(c().Fragment, null, !!t && !!n && n.length > 0 && c().createElement("div", {
                         className: e.container
-                    }, a.length > 0 && c().createElement(c().Fragment, null, c().createElement(D, {
+                    }, n.length > 0 && c().createElement(c().Fragment, null, c().createElement(D, {
                         title: "Attached DIDs"
-                    }), a.map((e => c().createElement(Re, {
+                    }), n.map((e => c().createElement(Re, {
                         key: e.did,
                         attachment: e,
                         status: o ? o[e.did] : void 0
-                    }))))), !!t && !!a && 0 === a.length && c().createElement("div", {
+                    }))))), !!t && !!n && 0 === n.length && c().createElement("div", {
                         className: e.messageContainer
                     }, "You have not attached any DID. Use the Explore menu to add a DID to this notebook."), !t && c().createElement("div", {
                         className: e.messageContainer
                     }, "Please open a Notebook."))
                 };
-            var Ve = a(1626),
-                Ke = a.n(Ve);
-            const Ze = (0, g.createUseStyles)({
+            var Ke = n(1626),
+                Ze = n.n(Ke);
+            const Ve = (0, g.createUseStyles)({
                     button: {
                         background: "none",
                         padding: 0,
                         border: "1px solid",
                         borderColor: e => `${e.outlineColor||"var(--jp-border-color1)"}`,
                         color: e => e.color || "var(--jp-ui-font-color1)",
                         outline: "none",
@@ -2398,33 +2395,33 @@
                     childrenContainer: {
                         margin: "8px 16px 8px 16px"
                     }
                 }),
                 Ge = e => {
                     var {
                         children: t,
-                        block: a,
-                        onClick: n,
+                        block: n,
+                        onClick: a,
                         className: o
                     } = e, l = function(e, t) {
-                        var a = {};
-                        for (var n in e) Object.prototype.hasOwnProperty.call(e, n) && t.indexOf(n) < 0 && (a[n] = e[n]);
+                        var n = {};
+                        for (var a in e) Object.prototype.hasOwnProperty.call(e, a) && t.indexOf(a) < 0 && (n[a] = e[a]);
                         if (null != e && "function" == typeof Object.getOwnPropertySymbols) {
                             var o = 0;
-                            for (n = Object.getOwnPropertySymbols(e); o < n.length; o++) t.indexOf(n[o]) < 0 && Object.prototype.propertyIsEnumerable.call(e, n[o]) && (a[n[o]] = e[n[o]])
+                            for (a = Object.getOwnPropertySymbols(e); o < a.length; o++) t.indexOf(a[o]) < 0 && Object.prototype.propertyIsEnumerable.call(e, a[o]) && (n[a[o]] = e[a[o]])
                         }
-                        return a
+                        return n
                     }(e, ["children", "block", "onClick", "className"]);
-                    const i = Ze(l),
-                        r = [i.button, o];
-                    return a && r.push(i.block), c().createElement("button", Object.assign({
-                        className: r.join(" "),
-                        onClick: n
+                    const r = Ve(l),
+                        i = [r.button, o];
+                    return n && i.push(r.block), c().createElement("button", Object.assign({
+                        className: i.join(" "),
+                        onClick: a
                     }, l), c().createElement("div", {
-                        className: i.childrenContainer
+                        className: r.childrenContainer
                     }, t))
                 },
                 Je = (0, g.createUseStyles)({
                     container: {
                         padding: "8px 16px 8px 16px"
                     },
                     label: {
@@ -2444,82 +2441,82 @@
                     },
                     loadingContainer: {
                         padding: "0 8px 0 8px",
                         display: "flex",
                         alignItems: "center"
                     }
                 }),
-                We = ({
+                qe = ({
                     params: e = {
                         username: "",
                         password: "",
                         account: ""
                     },
                     loading: t,
-                    onAuthParamsChange: a
+                    onAuthParamsChange: n
                 }) => {
-                    const n = Je(),
+                    const a = Je(),
                         o = c().createElement("div", {
-                            className: n.loadingContainer
+                            className: a.loadingContainer
                         }, c().createElement(M, {
-                            className: `${n.loadingIcon} material-icons`
+                            className: `${a.loadingIcon} material-icons`
                         }, "hourglass_top"));
                     return c().createElement(c().Fragment, null, c().createElement("div", {
-                        className: n.container
+                        className: a.container
                     }, c().createElement("div", {
-                        className: n.textFieldContainer
+                        className: a.textFieldContainer
                     }, c().createElement("div", {
-                        className: n.label
-                    }, "Username"), c().createElement(A, {
+                        className: a.label
+                    }, "Username"), c().createElement(L, {
                         placeholder: "Username",
                         value: e.username,
                         onChange: t => {
-                            return n = t.target.value, void a(Object.assign(Object.assign({}, e), {
-                                username: n
+                            return a = t.target.value, void n(Object.assign(Object.assign({}, e), {
+                                username: a
                             }));
-                            var n
+                            var a
                         },
                         disabled: t,
                         after: t ? o : void 0
                     })), c().createElement("div", {
-                        className: n.textFieldContainer
+                        className: a.textFieldContainer
                     }, c().createElement("div", {
-                        className: n.label
-                    }, "Password"), c().createElement(A, {
+                        className: a.label
+                    }, "Password"), c().createElement(L, {
                         placeholder: "Password",
                         type: "password",
                         value: e.password,
                         onChange: t => {
-                            return n = t.target.value, void a(Object.assign(Object.assign({}, e), {
-                                password: n
+                            return a = t.target.value, void n(Object.assign(Object.assign({}, e), {
+                                password: a
                             }));
-                            var n
+                            var a
                         },
                         disabled: t,
                         after: t ? o : void 0
                     })), c().createElement("div", {
-                        className: n.warning
+                        className: a.warning
                     }, "Your password will be stored in plain text inside your user directory."), c().createElement("div", {
-                        className: n.textFieldContainer
+                        className: a.textFieldContainer
                     }, c().createElement("div", {
-                        className: n.label
-                    }, "Account"), c().createElement(A, {
+                        className: a.label
+                    }, "Account"), c().createElement(L, {
                         placeholder: "Account",
                         value: e.account,
                         onChange: t => {
-                            return n = t.target.value, void a(Object.assign(Object.assign({}, e), {
-                                account: n
+                            return a = t.target.value, void n(Object.assign(Object.assign({}, e), {
+                                account: a
                             }));
-                            var n
+                            var a
                         },
                         disabled: t,
                         after: t ? o : void 0
                     }))))
                 };
-            const qe = (0, g.createUseStyles)({
+            const We = (0, g.createUseStyles)({
                     main: {
                         width: "300px",
                         background: "var(--jp-layout-color1)",
                         color: "var(--jp-ui-font-color1)"
                     },
                     heading: {
                         background: "var(--jp-layout-color2)",
@@ -2578,119 +2575,119 @@
                         extend: "icon",
                         color: "#5DC0FD"
                     }
                 }),
                 He = ({
                     directoryItem: e,
                     onClick: t,
-                    style: a
+                    style: n
                 }) => {
-                    const n = qe();
+                    const a = We();
                     return c().createElement("div", {
-                        className: n.listItem,
+                        className: a.listItem,
                         onClick: t,
-                        style: a
+                        style: n
                     }, c().createElement("div", {
-                        className: n.iconContainer
+                        className: a.iconContainer
                     }, "file" === e.type && c().createElement("i", {
-                        className: `${n.fileIcon} material-icons`
+                        className: `${a.fileIcon} material-icons`
                     }, "attachment"), "dir" === e.type && c().createElement("i", {
-                        className: `${n.dirIcon} material-icons`
+                        className: `${a.dirIcon} material-icons`
                     }, "folder")), c().createElement("div", {
-                        className: n.textContainer
+                        className: a.textContainer
                     }, e.name))
                 },
                 Ye = B((e => {
                     var {
                         children: t,
-                        onFilePicked: a
-                    } = e, n = function(e, t) {
-                        var a = {};
-                        for (var n in e) Object.prototype.hasOwnProperty.call(e, n) && t.indexOf(n) < 0 && (a[n] = e[n]);
+                        onFilePicked: n
+                    } = e, a = function(e, t) {
+                        var n = {};
+                        for (var a in e) Object.prototype.hasOwnProperty.call(e, a) && t.indexOf(a) < 0 && (n[a] = e[a]);
                         if (null != e && "function" == typeof Object.getOwnPropertySymbols) {
                             var o = 0;
-                            for (n = Object.getOwnPropertySymbols(e); o < n.length; o++) t.indexOf(n[o]) < 0 && Object.prototype.propertyIsEnumerable.call(e, n[o]) && (a[n[o]] = e[n[o]])
+                            for (a = Object.getOwnPropertySymbols(e); o < a.length; o++) t.indexOf(a[o]) < 0 && Object.prototype.propertyIsEnumerable.call(e, a[o]) && (n[a[o]] = e[a[o]])
                         }
-                        return a
+                        return n
                     }(e, ["children", "onFilePicked"]);
                     const {
                         actions: o
-                    } = n, l = qe(), [i, r] = (0, s.useState)([]), [d, m] = (0, s.useState)(!1), [p, u] = (0, s.useState)(!1), [v, h] = (0, s.useState)([]), [g, f] = (0, s.useState)({}), b = (e, t) => e.type === t.type ? e.name.toLowerCase() < t.name.toLowerCase() ? -1 : 1 : "dir" === e.type && "file" === t.type ? -1 : 1;
-                    (0, s.useEffect)((() => {
-                        const e = i.join("/");
+                    } = a, l = We(), [r, s] = (0, i.useState)([]), [d, m] = (0, i.useState)(!1), [p, u] = (0, i.useState)(!1), [v, h] = (0, i.useState)([]), [g, f] = (0, i.useState)({}), b = (e, t) => e.type === t.type ? e.name.toLowerCase() < t.name.toLowerCase() ? -1 : 1 : "dir" === e.type && "file" === t.type ? -1 : 1;
+                    (0, i.useEffect)((() => {
+                        const e = r.join("/");
                         g[e] ? h(g[e]) : (u(!0), o.listDirectory(e).then((e => e.sort(b))).then((t => {
-                            const a = Object.assign({}, g);
-                            a[e] = t, f(a), h(t)
+                            const n = Object.assign({}, g);
+                            n[e] = t, f(n), h(t)
                         })).catch((() => h([]))).finally((() => {
                             u(!1)
                         })))
-                    }), [i]);
-                    const E = (0, s.useCallback)((e => {
+                    }), [r]);
+                    const E = (0, i.useCallback)((e => {
                         27 === e.keyCode && m(!1)
                     }), []);
-                    (0, s.useEffect)((() => (document.addEventListener("keydown", E, !1), () => {
+                    (0, i.useEffect)((() => (document.addEventListener("keydown", E, !1), () => {
                         document.removeEventListener("keydown", E, !1)
                     })), []);
                     const x = ({
                             index: e,
                             style: t
                         }) => {
-                            const n = v[e];
+                            const a = v[e];
                             return c().createElement(He, {
                                 style: t,
-                                directoryItem: n,
-                                key: n.path,
+                                directoryItem: a,
+                                key: a.path,
                                 onClick: () => (e => {
-                                    "dir" === e.type ? r([...i, e.name]) : (a(e.path), m(!1))
-                                })(n)
+                                    "dir" === e.type ? s([...r, e.name]) : (n(e.path), m(!1))
+                                })(a)
                             })
                         },
                         y = c().createElement("div", {
                             className: l.main
                         }, c().createElement("div", {
                             className: l.heading
                         }, c().createElement("span", {
                             className: `material-icons ${l.icon} ${l.clickable}`,
                             onClick: () => {
-                                r([])
+                                s([])
                             }
-                        }, "home"), 0 === i.length && c().createElement("span", {
+                        }, "home"), 0 === r.length && c().createElement("span", {
                             className: l.folderName
-                        }, "  Home"), i.length >= 1 && c().createElement("span", {
+                        }, "  Home"), r.length >= 1 && c().createElement("span", {
                             className: `material-icons ${l.icon}`
-                        }, "navigate_next"), i.length >= 2 && c().createElement(c().Fragment, null, c().createElement("span", {
+                        }, "navigate_next"), r.length >= 2 && c().createElement(c().Fragment, null, c().createElement("span", {
                             className: `material-icons ${l.icon} ${l.clickable}`,
                             onClick: () => {
-                                const e = i.filter(((e, t) => t < i.length - 1));
-                                r(e)
+                                const e = r.filter(((e, t) => t < r.length - 1));
+                                s(e)
                             }
                         }, "more_horiz"), c().createElement("span", {
                             className: `material-icons ${l.icon}`
                         }, "navigate_next")), c().createElement("span", {
                             className: l.folderName
-                        }, i ? i[i.length - 1] : "")), c().createElement("div", {
+                        }, r ? r[r.length - 1] : "")), c().createElement("div", {
                             className: `${l.content} ${p?"loading":""}`
                         }, c().createElement(j(), null, (({
                             height: e,
                             width: t
                         }) => c().createElement(k.FixedSizeList, {
                             height: e,
                             itemCount: v.length,
                             itemSize: 32,
                             width: t
                         }, x)))));
-                    return c().createElement(K(), {
+                    return c().createElement(Z(), {
                         enterExitTransitionDurationMs: 0,
                         isOpen: d,
                         preferPlace: "above",
                         body: y,
                         onOuterAction: () => m(!1)
                     }, c().createElement("div", {
                         onClick: () => {
-                            m(!0), r([]), h([]), f({})
+                            m(!0), s([]), h([]), f({})
                         }
                     }, t))
                 })),
                 Xe = (0, g.createUseStyles)({
                     container: {
                         padding: "8px 16px 8px 16px"
                     },
@@ -2722,75 +2719,75 @@
                 Qe = ({
                     params: e = {
                         certificate: "",
                         key: "",
                         account: ""
                     },
                     loading: t,
-                    onAuthParamsChange: a
+                    onAuthParamsChange: n
                 }) => {
-                    const n = Xe(),
+                    const a = Xe(),
                         o = t => {
-                            a(Object.assign(Object.assign({}, e), {
+                            n(Object.assign(Object.assign({}, e), {
                                 certificate: t
                             }))
                         },
                         l = t => {
-                            a(Object.assign(Object.assign({}, e), {
+                            n(Object.assign(Object.assign({}, e), {
                                 key: t
                             }))
                         },
-                        i = c().createElement("div", {
-                            className: n.iconContainer
+                        r = c().createElement("div", {
+                            className: a.iconContainer
                         }, c().createElement(M, {
-                            className: `${n.icon} material-icons`
+                            className: `${a.icon} material-icons`
                         }, "hourglass_top"));
                     return c().createElement(c().Fragment, null, c().createElement("div", {
-                        className: n.container
+                        className: a.container
                     }, c().createElement("div", {
-                        className: n.textFieldContainer
+                        className: a.textFieldContainer
                     }, c().createElement("div", {
-                        className: n.label
-                    }, "Certificate file path"), c().createElement(A, {
+                        className: a.label
+                    }, "Certificate file path"), c().createElement(L, {
                         placeholder: "Path to certificate file",
                         value: e.certificate,
                         onChange: e => o(e.target.value),
                         disabled: t,
-                        after: t ? i : c().createElement(et, {
+                        after: t ? r : c().createElement(et, {
                             onFilePicked: e => o(e)
                         })
                     })), c().createElement("div", {
-                        className: n.textFieldContainer
+                        className: a.textFieldContainer
                     }, c().createElement("div", {
-                        className: n.label
-                    }, "Key file path"), c().createElement(A, {
+                        className: a.label
+                    }, "Key file path"), c().createElement(L, {
                         placeholder: "Path to key file",
                         value: e.key,
                         onChange: e => l(e.target.value),
                         disabled: t,
-                        after: t ? i : c().createElement(et, {
+                        after: t ? r : c().createElement(et, {
                             onFilePicked: e => l(e)
                         })
                     })), c().createElement("div", {
-                        className: n.warning
+                        className: a.warning
                     }, "Enter the private key path if the certificate file does not include it. Passphrase-protected certificate is not supported."), c().createElement("div", {
-                        className: n.textFieldContainer
+                        className: a.textFieldContainer
                     }, c().createElement("div", {
-                        className: n.label
-                    }, "Account"), c().createElement(A, {
+                        className: a.label
+                    }, "Account"), c().createElement(L, {
                         placeholder: "Account",
                         value: e.account,
                         onChange: t => {
-                            return n = t.target.value, void a(Object.assign(Object.assign({}, e), {
-                                account: n
+                            return a = t.target.value, void n(Object.assign(Object.assign({}, e), {
+                                account: a
                             }));
-                            var n
+                            var a
                         },
                         disabled: t,
-                        after: t ? i : void 0
+                        after: t ? r : void 0
                     }))))
                 },
                 et = ({
                     onFilePicked: e
                 }) => {
                     const t = Xe();
                     return c().createElement("div", {
@@ -2826,65 +2823,65 @@
                         alignItems: "center"
                     },
                     action: {
                         cursor: "pointer",
                         color: "var(--jp-rucio-primary-blue-color)"
                     }
                 }),
-                at = ({
+                nt = ({
                     params: e = {
                         proxy: "",
                         account: ""
                     },
                     loading: t,
-                    onAuthParamsChange: a
+                    onAuthParamsChange: n
                 }) => {
-                    const n = tt(),
+                    const a = tt(),
                         o = t => {
-                            a(Object.assign(Object.assign({}, e), {
+                            n(Object.assign(Object.assign({}, e), {
                                 proxy: t
                             }))
                         },
                         l = c().createElement("div", {
-                            className: n.iconContainer
+                            className: a.iconContainer
                         }, c().createElement(M, {
-                            className: `${n.icon} material-icons`
+                            className: `${a.icon} material-icons`
                         }, "hourglass_top"));
                     return c().createElement(c().Fragment, null, c().createElement("div", {
-                        className: n.container
+                        className: a.container
                     }, c().createElement("div", {
-                        className: n.textFieldContainer
+                        className: a.textFieldContainer
                     }, c().createElement("div", {
-                        className: n.label
-                    }, "Proxy file path"), c().createElement(A, {
+                        className: a.label
+                    }, "Proxy file path"), c().createElement(L, {
                         placeholder: "Path to proxy PEM file",
                         value: e.proxy,
                         onChange: e => o(e.target.value),
                         disabled: t,
-                        after: t ? l : c().createElement(nt, {
+                        after: t ? l : c().createElement(at, {
                             onFilePicked: e => o(e)
                         })
                     })), c().createElement("div", {
-                        className: n.textFieldContainer
+                        className: a.textFieldContainer
                     }, c().createElement("div", {
-                        className: n.label
-                    }, "Account"), c().createElement(A, {
+                        className: a.label
+                    }, "Account"), c().createElement(L, {
                         placeholder: "Account",
                         value: e.account,
                         onChange: t => {
-                            return n = t.target.value, void a(Object.assign(Object.assign({}, e), {
-                                account: n
+                            return a = t.target.value, void n(Object.assign(Object.assign({}, e), {
+                                account: a
                             }));
-                            var n
+                            var a
                         },
                         disabled: t,
                         after: t ? l : void 0
                     }))))
                 },
-                nt = ({
+                at = ({
                     onFilePicked: e
                 }) => {
                     const t = tt();
                     return c().createElement("div", {
                         className: t.iconContainer
                     }, c().createElement(Ye, {
                         onFilePicked: e
@@ -2966,215 +2963,215 @@
                     purgeButton: {
                         marginTop: "16px"
                     }
                 }),
                 lt = B((e => {
                     const {
                         actions: t
-                    } = e, a = ot(), n = (0, b.useStoreState)(C, (e => e.activeInstance)), o = (0, b.useStoreState)(C, (e => e.activeAuthType)), l = (0, b.useStoreState)(C, (e => e.instances)) || [], [i, r] = (0, s.useState)(null == n ? void 0 : n.name), d = (0, s.useMemo)((() => l.find((e => e.name === i))), [l, i]), m = d ? [d.oidcEnabled ? {
+                    } = e, n = ot(), a = (0, b.useStoreState)(C, (e => e.activeInstance)), o = (0, b.useStoreState)(C, (e => e.activeAuthType)), l = (0, b.useStoreState)(C, (e => e.instances)) || [], [r, s] = (0, i.useState)(null == a ? void 0 : a.name), d = (0, i.useMemo)((() => l.find((e => e.name === r))), [l, r]), m = d ? [d.oidcEnabled ? {
                         label: "OpenID Connect",
                         value: "oidc"
                     } : void 0, {
                         label: "X.509 User Certificate",
                         value: "x509"
                     }, {
                         label: "X.509 Proxy Certificate",
                         value: "x509_proxy"
                     }, {
                         label: "Username & Password",
                         value: "userpass"
-                    }].filter((e => !!e)) : [], p = o ? m.find((e => e.value === o)) : void 0, [u, v] = (0, s.useState)(o), [h, g] = (0, s.useState)(), [f, E] = (0, s.useState)(), [x, y] = (0, s.useState)(), [N, I] = (0, s.useState)(!0), [S, k] = (0, s.useState)(!1), [w, j] = (0, s.useState)(!1), [L, A] = (0, s.useState)(!1), [O, R] = (0, s.useState)(!1), [P, T] = (0, s.useState)(!1), M = (0, s.useMemo)((() => null == l ? void 0 : l.map((e => ({
+                    }].filter((e => !!e)) : [], p = o ? m.find((e => e.value === o)) : void 0, [u, v] = (0, i.useState)(o), [h, g] = (0, i.useState)(), [f, E] = (0, i.useState)(), [x, y] = (0, i.useState)(), [N, I] = (0, i.useState)(!0), [S, k] = (0, i.useState)(!1), [w, j] = (0, i.useState)(!1), [A, L] = (0, i.useState)(!1), [O, R] = (0, i.useState)(!1), [P, T] = (0, i.useState)(!1), M = (0, i.useMemo)((() => null == l ? void 0 : l.map((e => ({
                         label: e.displayName,
                         value: e.name
                     })))), [l]);
-                    (0, s.useEffect)((() => {
-                        i && (I(!0), "userpass" === u ? t.fetchAuthConfig(i, u).then((e => g(e))).catch((() => g(void 0))).finally((() => I(!1))) : "x509" === u ? t.fetchAuthConfig(i, u).then((e => E(e))).catch((() => E(void 0))).finally((() => I(!1))) : "x509_proxy" === u && t.fetchAuthConfig(i, u).then((e => y(e))).catch((() => y(void 0))).finally((() => I(!1))))
-                    }), [i, u]);
-                    const F = i && u,
-                        _ = {
+                    (0, i.useEffect)((() => {
+                        r && (I(!0), "userpass" === u ? t.fetchAuthConfig(r, u).then((e => g(e))).catch((() => g(void 0))).finally((() => I(!1))) : "x509" === u ? t.fetchAuthConfig(r, u).then((e => E(e))).catch((() => E(void 0))).finally((() => I(!1))) : "x509_proxy" === u && t.fetchAuthConfig(r, u).then((e => y(e))).catch((() => y(void 0))).finally((() => I(!1))))
+                    }), [r, u]);
+                    const F = r && u,
+                        z = {
                             control: (e, t) => Object.assign(Object.assign({}, e), {
                                 borderRadius: 0,
                                 borderColor: "var(--jp-border-color1)",
                                 background: "var(--jp-layout-color1)"
                             }),
                             singleValue: (e, t) => Object.assign(Object.assign({}, e), {
                                 color: "var(--jp-ui-font-color1)"
                             }),
                             menu: (e, t) => Object.assign(Object.assign({}, e), {
                                 background: "var(--jp-layout-color1)",
                                 color: "var(--jp-ui-font-color1)"
                             }),
                             option: (e, {
                                 isFocused: t,
-                                isSelected: a
+                                isSelected: n
                             }) => Object.assign(Object.assign({}, e), {
-                                background: t ? a ? e.background : "var(--jp-layout-color2)" : e.background,
+                                background: t ? n ? e.background : "var(--jp-layout-color2)" : e.background,
                                 ":active": Object.assign(Object.assign({}, e[":active"]), {
-                                    background: a ? e.background : "var(--jp-layout-color2)"
+                                    background: n ? e.background : "var(--jp-layout-color2)"
                                 })
                             })
                         },
-                        U = n ? {
-                            label: n.displayName,
-                            value: n.name
+                        $ = a ? {
+                            label: a.displayName,
+                            value: a.name
                         } : null;
                     return c().createElement("div", {
-                        className: a.content
+                        className: n.content
                     }, c().createElement("div", {
-                        className: a.scrollable
+                        className: n.scrollable
                     }, c().createElement("div", {
-                        className: a.container
+                        className: n.container
                     }, c().createElement("div", {
-                        className: a.formItem
+                        className: n.formItem
                     }, c().createElement("div", {
-                        className: a.label
-                    }, "Active Instance"), c().createElement(Ke(), {
-                        className: a.formControl,
+                        className: n.label
+                    }, "Active Instance"), c().createElement(Ze(), {
+                        className: n.formControl,
                         options: M,
-                        styles: _,
-                        defaultValue: U,
-                        onChange: e => r(e.value)
+                        styles: z,
+                        defaultValue: $,
+                        onChange: e => s(e.value)
                     })), c().createElement("div", {
-                        className: a.formItem
+                        className: n.formItem
                     }, c().createElement("div", {
-                        className: a.label
-                    }, "Authentication"), c().createElement(Ke(), {
-                        className: a.formControl,
+                        className: n.label
+                    }, "Authentication"), c().createElement(Ze(), {
+                        className: n.formControl,
                         options: m,
-                        styles: _,
+                        styles: z,
                         defaultValue: p,
                         onChange: e => v(e.value)
                     }))), c().createElement("div", null, c().createElement("div", {
-                        className: i && "userpass" === u ? "" : a.hidden
+                        className: r && "userpass" === u ? "" : n.hidden
                     }, c().createElement(D, {
                         title: "Username & Password"
-                    }), c().createElement(We, {
+                    }), c().createElement(qe, {
                         loading: N,
                         params: h,
                         onAuthParamsChange: e => g(e)
                     })), c().createElement("div", {
-                        className: i && "x509" === u ? "" : a.hidden
+                        className: r && "x509" === u ? "" : n.hidden
                     }, c().createElement(D, {
                         title: "X.509 User Certificate"
                     }), c().createElement(Qe, {
                         loading: N,
                         params: f,
                         onAuthParamsChange: e => E(e)
                     })), c().createElement("div", {
-                        className: i && "x509_proxy" === u ? "" : a.hidden
+                        className: r && "x509_proxy" === u ? "" : n.hidden
                     }, c().createElement(D, {
                         title: "X.509 Proxy Certificate"
-                    }), c().createElement(at, {
+                    }), c().createElement(nt, {
                         loading: N,
                         params: x,
                         onAuthParamsChange: e => y(e)
                     }))), c().createElement("div", {
-                        className: L ? void 0 : a.hidden
+                        className: A ? void 0 : n.hidden
                     }, c().createElement(D, {
                         title: "Advanced Settings"
                     }), c().createElement("div", {
-                        className: a.container
+                        className: n.container
                     }, c().createElement("div", {
-                        className: a.formItem
+                        className: n.formItem
                     }, c().createElement("div", {
-                        className: a.textFieldContainer
+                        className: n.textFieldContainer
                     }, c().createElement("div", {
-                        className: a.label
+                        className: n.label
                     }, "Purge cache"), c().createElement("div", {
-                        className: a.subtitle
+                        className: n.subtitle
                     }, "Remove all caches, including search results and DID paths."), c().createElement(Ge, {
                         block: !0,
                         onClick: () => {
                             T(!1), R(!0), t.purgeCache().then((() => {
                                 T(!0), setTimeout((() => T(!1)), 3e3)
                             })).finally((() => R(!1)))
                         },
                         disabled: O,
                         outlineColor: "var(--jp-error-color1)",
                         color: !O && P ? "#FFFFFF" : "var(--jp-error-color1)",
-                        className: !O && P ? a.buttonPurgedAcknowledgement : a.purgeButton
+                        className: !O && P ? n.buttonPurgedAcknowledgement : n.purgeButton
                     }, !O && !P && c().createElement(c().Fragment, null, "Purge Cache"), O && c().createElement(c().Fragment, null, "Purging..."), !O && P && c().createElement(c().Fragment, null, "Purged!")))))), c().createElement("div", {
-                        className: a.container
-                    }, !L && c().createElement("div", {
-                        className: a.action,
-                        onClick: () => A(!0)
-                    }, "Show Advanced Settings"), L && c().createElement("div", {
-                        className: a.action,
-                        onClick: () => A(!1)
+                        className: n.container
+                    }, !A && c().createElement("div", {
+                        className: n.action,
+                        onClick: () => L(!0)
+                    }, "Show Advanced Settings"), A && c().createElement("div", {
+                        className: n.action,
+                        onClick: () => L(!1)
                     }, "Hide Advanced Settings"))), c().createElement("div", {
-                        className: a.buttonContainer
+                        className: n.buttonContainer
                     }, c().createElement(Ge, {
                         block: !0,
                         onClick: () => {
-                            if (!i) return;
+                            if (!r) return;
                             const e = [];
-                            if (i && u) {
-                                const o = (a = i, n = u, C.update((e => {
+                            if (r && u) {
+                                const o = (n = r, a = u, C.update((e => {
                                     var t;
-                                    if ((null === (t = e.activeInstance) || void 0 === t ? void 0 : t.name) !== a) {
+                                    if ((null === (t = e.activeInstance) || void 0 === t ? void 0 : t.name) !== n) {
                                         C.update((e => {
                                             e.fileDetails = {}, e.collectionDetails = {}
                                         }));
-                                        const t = l.find((e => e.name === a));
+                                        const t = l.find((e => e.name === n));
                                         e.activeInstance = t
                                     }
-                                    e.activeAuthType !== n && (e.activeAuthType = n)
-                                })), t.postActiveInstance(a, n).catch((e => console.log(e))));
+                                    e.activeAuthType !== a && (e.activeAuthType = a)
+                                })), t.postActiveInstance(n, a).catch((e => console.log(e))));
                                 e.push(o)
                             }
-                            var a, n;
+                            var n, a;
                             if (u) {
-                                const a = (() => {
+                                const n = (() => {
                                     switch (u) {
                                         case "userpass":
                                             return h;
                                         case "x509":
                                             return f;
                                         case "x509_proxy":
                                             return x
                                     }
                                 })();
-                                if (a) {
-                                    const n = t.putAuthConfig(i, u, a);
-                                    e.push(n)
+                                if (n) {
+                                    const a = t.putAuthConfig(r, u, n);
+                                    e.push(a)
                                 }
                             }
                             k(!0), Promise.all(e).then((() => {
                                 j(!0), setTimeout((() => j(!1)), 3e3)
                             })).finally((() => k(!1)))
                         },
                         disabled: !F || S,
                         outlineColor: !S && w ? "#689f38" : void 0,
                         color: !S && w ? "#FFFFFF" : void 0,
-                        className: !S && w ? a.buttonSavedAcknowledgement : void 0
+                        className: !S && w ? n.buttonSavedAcknowledgement : void 0
                     }, !S && !w && c().createElement(c().Fragment, null, "Save Settings"), S && c().createElement(c().Fragment, null, "Saving..."), !S && w && c().createElement(c().Fragment, null, "Saved!"))))
                 }));
-            var it;
+            var rt;
             ! function(e) {
                 class t extends f.VDomModel {
                     constructor() {
                         super(...arguments), this._log = ""
                     }
                     get log() {
                         return this._log
                     }
                     set log(e) {
                         this._log = e, this.stateChanged.emit(void 0)
                     }
                 }
                 e.Model = t;
-                class a extends f.VDomRenderer {
+                class n extends f.VDomRenderer {
                     constructor(t) {
-                        super(new e.Model), this.uploadJobId = t, this.title.icon = l.fileUploadIcon, this.id = `${d}:upload-log-viewer-${t}`, this.title.label = `Upload Job #${t}`, this.title.closable = !0
+                        super(new e.Model), this.uploadJobId = t, this.title.icon = l.fileUploadIcon, this.id = `${s}:upload-log-viewer-${t}`, this.title.label = `Upload Job #${t}`, this.title.closable = !0
                     }
                     onAfterAttach() {
                         const {
                             activeInstance: e
                         } = C.getRawState();
-                        e && $.fetchUploadJobLog(e.name, this.uploadJobId).then((e => {
+                        e && _.fetchUploadJobLog(e.name, this.uploadJobId).then((e => {
                             this.model.log = e.text
                         })).catch((e => {
                             console.log(e), this.model.log = "Error reading upload job log."
                         }))
                     }
                     render() {
                         return c().createElement("div", {
@@ -3191,24 +3188,24 @@
                         }, c().createElement("code", {
                             style: {
                                 whiteSpace: "pre"
                             }
                         }, this.model.log)))
                     }
                 }
-                e.WidgetBody = a
-            }(it || (it = {}));
-            class rt extends f.MainAreaWidget {
+                e.WidgetBody = n
+            }(rt || (rt = {}));
+            class it extends f.MainAreaWidget {
                 constructor(e) {
                     super({
-                        content: new it.WidgetBody(e)
+                        content: new rt.WidgetBody(e)
                     })
                 }
             }
-            const st = (0, g.createUseStyles)({
+            const ct = (0, g.createUseStyles)({
                     listItemContainer: {
                         display: "flex",
                         flexDirection: "row",
                         borderBottom: "1px solid var(--jp-border-color2)",
                         padding: "8px 16px 8px 16px",
                         fontSize: "9pt"
                     },
@@ -3274,18 +3271,18 @@
                     },
                     action: {
                         fontSize: "9pt",
                         color: "var(--jp-rucio-primary-blue-color)",
                         cursor: "pointer"
                     }
                 }),
-                ct = ({
+                st = ({
                     status: e
                 }) => {
-                    const t = st();
+                    const t = ct();
                     switch (e) {
                         case "UPLOADING":
                             return c().createElement(M, {
                                 className: `${t.replicatingIcon} material-icons`
                             }, "hourglass_top");
                         case "OK":
                             return c().createElement("i", {
@@ -3299,96 +3296,96 @@
                             return c().createElement("span", null)
                     }
                 },
                 dt = B((({
                     job: e,
                     onDeleteClick: t
                 }) => {
-                    const a = st(),
-                        n = (0, s.useContext)(h);
+                    const n = ct(),
+                        a = (0, i.useContext)(h);
                     return c().createElement("div", {
-                        className: a.listItemContainer
+                        className: n.listItemContainer
                     }, c().createElement("div", {
-                        className: a.listItemIconContainer
-                    }, c().createElement(ct, {
+                        className: n.listItemIconContainer
+                    }, c().createElement(st, {
                         status: e.status
                     })), c().createElement("div", {
-                        className: a.listItemContent
+                        className: n.listItemContent
                     }, c().createElement("div", {
-                        className: a.did
+                        className: n.did
                     }, e.did), c().createElement("div", {
-                        className: a.variableName
+                        className: n.variableName
                     }, e.path, " → ", e.rse), "FAILED" === e.status && c().createElement("div", {
-                        className: a.action,
+                        className: n.action,
                         onClick: () => {
-                            const t = new rt(e.id);
-                            null == n || n.shell.add(t, "main")
+                            const t = new it(e.id);
+                            null == a || a.shell.add(t, "main")
                         }
                     }, "Show Log")), c().createElement("div", {
-                        className: a.actionContainer
+                        className: n.actionContainer
                     }, "UPLOADING" !== e.status && !!t && c().createElement("div", {
-                        className: a.clearButton,
+                        className: n.clearButton,
                         onClick: t
                     }, c().createElement("i", {
-                        className: `${a.clearIcon} material-icons`
+                        className: `${n.clearIcon} material-icons`
                     }, "clear"))))
                 })),
                 mt = (0, g.createUseStyles)({
                     container: {
                         padding: "16px 0 16px 0"
                     },
                     messageContainer: {
                         padding: "16px"
                     }
                 }),
                 pt = ({
                     visible: e
                 }) => {
                     const t = mt(),
-                        a = (0, b.useStoreState)(C, (e => e.activeInstance)),
-                        [n, o] = (0, s.useState)([]),
+                        n = (0, b.useStoreState)(C, (e => e.activeInstance)),
+                        [a, o] = (0, i.useState)([]),
                         l = () => {
-                            a && $.fetchUploadJobs(a.name).then((e => o(e))).catch((e => console.log(e)))
+                            n && _.fetchUploadJobs(n.name).then((e => o(e))).catch((e => console.log(e)))
                         };
-                    return (0, s.useEffect)((() => {
+                    return (0, i.useEffect)((() => {
                             e && l()
-                        }), [a, e]),
+                        }), [n, e]),
                         function(e, t) {
-                            const a = (0, s.useRef)();
-                            (0, s.useEffect)((() => {
-                                a.current = e
-                            }), [e]), (0, s.useEffect)((() => {
+                            const n = (0, i.useRef)();
+                            (0, i.useEffect)((() => {
+                                n.current = e
+                            }), [e]), (0, i.useEffect)((() => {
                                 {
                                     const e = setInterval((function() {
-                                        const e = a.current;
+                                        const e = n.current;
                                         null == e || e()
                                     }), t);
                                     return () => clearInterval(e)
                                 }
                             }), [t])
                         }((() => {
                             e && l()
-                        }), 5e3), c().createElement("div", null, n.length > 0 && c().createElement("div", {
+                        }), 5e3), c().createElement("div", null, a.length > 0 && c().createElement("div", {
                             className: t.container
                         }, c().createElement(c().Fragment, null, c().createElement(D, {
                             title: "Upload Jobs"
-                        }), n.map((e => c().createElement(dt, {
+                        }), a.map((e => c().createElement(dt, {
                             key: e.id,
                             job: e,
                             onDeleteClick: () => {
-                                return t = e.id, void(a && $.deleteUploadJob(a.name, t).then((() => {
+                                return t = e.id, void(n && _.deleteUploadJob(n.name, t).then((() => {
                                     console.log("Job deleted");
-                                    const e = n.filter((e => e.id !== t));
+                                    const e = a.filter((e => e.id !== t));
                                     o(e)
                                 })).finally((() => {
                                     l()
                                 })));
                                 var t
                             }
-                        }))))), 0 === n.length && c().createElement("div", {
+                        }))))), 0 === a.length && c().createElement("div", {
                             className: t.messageContainer
                         }, "You do not have upload jobs."))
                 },
                 ut = (0, g.createUseStyles)({
                     panel: {
                         height: "100%",
                         display: "flex",
@@ -3430,15 +3427,15 @@
                     hidden: {
                         display: "none"
                     }
                 }),
                 vt = () => {
                     const e = ut(),
                         t = (0, b.useStoreState)(C, (e => e.activeInstance)),
-                        [a, n] = (0, s.useState)(t ? 1 : 3),
+                        [n, a] = (0, i.useState)(t ? 1 : 3),
                         o = [{
                             title: "Explore",
                             value: 1,
                             right: !1,
                             disabled: !t
                         }, {
                             title: "Notebook",
@@ -3466,55 +3463,55 @@
                         className: e.panel
                     }, c().createElement(y, null), c().createElement("div", {
                         className: e.container
                     }, c().createElement("div", {
                         className: e.menuBar
                     }, c().createElement(S, {
                         menus: o,
-                        value: a,
-                        onChange: n
+                        value: n,
+                        onChange: a
                     })), c().createElement("div", {
                         className: e.content
                     }, c().createElement("div", {
-                        className: 1 !== a ? e.hidden : ""
+                        className: 1 !== n ? e.hidden : ""
                     }, t && c().createElement(je, null)), c().createElement("div", {
-                        className: 2 !== a ? e.hidden : ""
+                        className: 2 !== n ? e.hidden : ""
                     }, t && c().createElement(Be, null)), c().createElement("div", {
-                        className: 3 !== a ? e.hidden : ""
+                        className: 3 !== n ? e.hidden : ""
                     }, c().createElement(lt, null)), c().createElement("div", {
-                        className: 4 !== a ? e.hidden : ""
+                        className: 4 !== n ? e.hidden : ""
                     }, c().createElement(pt, {
-                        visible: 4 === a
+                        visible: 4 === n
                     })))))
                 },
                 ht = ({
                     error: e
                 }) => {
                     const t = ut();
                     return c().createElement("div", {
                         className: t.content
                     }, e)
                 };
             class gt extends f.VDomRenderer {
                 constructor(e, t) {
                     super(), super.addClass("jp-RucioExtensionPanel"), super.title.closable = !0, super.title.icon = N;
                     const {
-                        app: a,
-                        instanceConfig: n
+                        app: n,
+                        instanceConfig: a
                     } = e;
-                    this.app = a, t ? this.error = null != t ? t : "Failed to activate extension. Make sure that the extension is configured and installed properly." : (this.instanceConfig = n, this.populateUIStore(n))
+                    this.app = n, t ? this.error = null != t ? t : "Failed to activate extension. Make sure that the extension is configured and installed properly." : (this.instanceConfig = a, this.populateUIStore(a))
                 }
                 populateUIStore(e) {
                     const {
                         activeInstance: t,
-                        authType: a,
-                        instances: n
-                    } = e, o = n.find((e => e.name === t));
+                        authType: n,
+                        instances: a
+                    } = e, o = a.find((e => e.name === t));
                     C.update((e => {
-                        e.activeInstance = o, e.activeAuthType = a, e.instances = n
+                        e.activeInstance = o, e.activeAuthType = n, e.instances = a
                     }))
                 }
                 render() {
                     return this.error ? c().createElement(ht, {
                         error: this.error
                     }) : this.instanceConfig ? c().createElement(h.Provider, {
                         value: this.app
@@ -3527,114 +3524,114 @@
                 constructor(e) {
                     this.options = e, this.setup()
                 }
                 setup() {
                     const {
                         labShell: e
                     } = this.options;
-                    Z.subscribe((e => e.activeNotebookAttachment), ((e, t) => {
+                    V.subscribe((e => e.activeNotebookAttachment), ((e, t) => {
                         e && this.onNotebookAttachmentChanged(e, t)
                     })), e.currentChanged.connect(this.onCurrentTabChanged, this)
                 }
                 onNotebookAttachmentChanged(e, t) {
-                    var a;
+                    var n;
                     const {
-                        activeNotebookPanel: n
+                        activeNotebookPanel: a
                     } = t;
-                    e && n && (this.setJupyterNotebookFileRucioMetadata(e, t), (null === (a = n.sessionContext.session) || void 0 === a ? void 0 : a.kernel) && n.sessionContext.ready.then((() => {
+                    e && a && (this.setJupyterNotebookFileRucioMetadata(e, t), (null === (n = a.sessionContext.session) || void 0 === n ? void 0 : n.kernel) && a.sessionContext.ready.then((() => {
                         const {
                             notebookListener: e
                         } = this.options;
-                        e.injectUninjected(n)
+                        e.injectUninjected(a)
                     })))
                 }
                 setJupyterNotebookFileRucioMetadata(e, t) {
-                    var a, n;
-                    const o = null === (n = null === (a = t.activeNotebookPanel) || void 0 === a ? void 0 : a.model) || void 0 === n ? void 0 : n.metadata;
+                    var n, a;
+                    const o = null === (a = null === (n = t.activeNotebookPanel) || void 0 === n ? void 0 : n.model) || void 0 === a ? void 0 : a.metadata;
                     if (!o) return;
-                    const l = o.get(m),
-                        i = e;
-                    l !== i && (0 === i.length ? l && o.delete(m) : o.set(m, i))
+                    const l = o.get(d),
+                        r = e;
+                    l !== r && (0 === r.length ? l && o.delete(d) : o.set(d, r))
                 }
                 onCurrentTabChanged() {
                     if (!this.isCurrentTabANotebook()) return this.setActiveNotebook(void 0), void this.setActiveNotebookAttachments(void 0);
                     const {
                         notebookTracker: e
                     } = this.options, t = e.currentWidget;
                     t && t.revealed.then((() => {
                         var e;
                         this.setActiveNotebook(t);
-                        const a = null === (e = t.model) || void 0 === e ? void 0 : e.metadata.get(m);
-                        if (!a) return void this.setActiveNotebookAttachments([]);
-                        const n = a;
-                        this.setActiveNotebookAttachments(n)
+                        const n = null === (e = t.model) || void 0 === e ? void 0 : e.metadata.get(d);
+                        if (!n) return void this.setActiveNotebookAttachments([]);
+                        const a = n;
+                        this.setActiveNotebookAttachments(a)
                     }))
                 }
                 isCurrentTabANotebook() {
                     const {
                         labShell: e,
                         notebookTracker: t
-                    } = this.options, a = e.currentWidget, n = t.currentWidget;
-                    return !!a && a === n
+                    } = this.options, n = e.currentWidget, a = t.currentWidget;
+                    return !!n && n === a
                 }
                 setActiveNotebook(e) {
-                    Z.update((t => {
+                    V.update((t => {
                         t.activeNotebookPanel = e
                     }))
                 }
                 setActiveNotebookAttachments(e) {
-                    Z.update((t => {
+                    V.update((t => {
                         t.activeNotebookAttachment = e
                     }))
                 }
             }
             class bt {
                 constructor(e) {
-                    this.activePolling = [], this.activeNotebookAttachmentDIDs = [], this.notebookListener = e, this.pollingRef = new Y, Z.subscribe((e => e.activeNotebookAttachment), (e => {
+                    this.activePolling = [], this.activeNotebookAttachmentDIDs = [], this.notebookListener = e, this.pollingRef = new Y, V.subscribe((e => e.activeNotebookAttachment), (e => {
                         this.removeUnfocusedDIDs(e), this.processNewAttachments(e), this.activeNotebookAttachmentDIDs = (null == e ? void 0 : e.map((e => e.did))) || []
-                    })), C.subscribe((e => e.fileDetails), ((e, t, a) => {
+                    })), C.subscribe((e => e.fileDetails), ((e, t, n) => {
                         e && Object.keys(e).filter((e => this.activeNotebookAttachmentDIDs.includes(e))).map((t => ({
                             did: t,
                             file: {
                                 current: e[t],
-                                prev: a[t]
+                                prev: n[t]
                             }
                         }))).forEach((({
                             did: e,
                             file: t
                         }) => {
-                            var a;
+                            var n;
                             if ("REPLICATING" === t.current.status) this.enablePolling(e, "file");
-                            else if (this.activePolling.includes(e) && this.disablePolling(e), "OK" === t.current.status && "REPLICATING" === (null === (a = t.prev) || void 0 === a ? void 0 : a.status)) {
+                            else if (this.activePolling.includes(e) && this.disablePolling(e), "OK" === t.current.status && "REPLICATING" === (null === (n = t.prev) || void 0 === n ? void 0 : n.status)) {
                                 const {
                                     activeNotebookPanel: t
-                                } = Z.getRawState();
+                                } = V.getRawState();
                                 t && this.notebookListener.reinjectSpecificDID(t, e)
                             }
                         }))
-                    })), C.subscribe((e => e.collectionDetails), ((e, t, a) => {
+                    })), C.subscribe((e => e.collectionDetails), ((e, t, n) => {
                         e && Object.keys(e).filter((e => this.activeNotebookAttachmentDIDs.includes(e))).map((t => ({
                             did: t,
                             file: {
                                 current: e[t],
-                                prev: a[t]
+                                prev: n[t]
                             }
                         }))).forEach((({
                             did: e,
                             file: t
                         }) => {
-                            const a = G(t.current);
-                            if ("REPLICATING" === a) this.enablePolling(e, "collection");
+                            const n = G(t.current);
+                            if ("REPLICATING" === n) this.enablePolling(e, "collection");
                             else {
                                 this.activePolling.includes(e) && this.disablePolling(e);
-                                const n = G(t.prev);
-                                if ("AVAILABLE" === a && "REPLICATING" === n) {
+                                const a = G(t.prev);
+                                if ("AVAILABLE" === n && "REPLICATING" === a) {
                                     const {
                                         activeNotebookPanel: t
-                                    } = Z.getRawState();
+                                    } = V.getRawState();
                                     t && this.notebookListener.reinjectSpecificDID(t, e)
                                 }
                             }
                         }))
                     }))
                 }
                 removeUnfocusedDIDs(e = []) {
@@ -3647,409 +3644,74 @@
                         }))
                     }))
                 }
                 async shouldEnablePolling(e) {
                     const {
                         activeInstance: t
                     } = C.getRawState();
-                    return !!t && ("file" === e.type ? "REPLICATING" === (await $.getFileDIDDetails(t.name, e.did)).status : (await $.getCollectionDIDDetails(t.name, e.did)).find((e => "REPLICATING" === e.status)))
+                    return !!t && ("file" === e.type ? "REPLICATING" === (await _.getFileDIDDetails(t.name, e.did)).status : (await _.getCollectionDIDDetails(t.name, e.did)).find((e => "REPLICATING" === e.status)))
                 }
                 enablePolling(e, t) {
                     X.requestPolling(e, t, this.pollingRef, !1), this.activePolling.push(e)
                 }
                 disablePolling(e) {
                     X.disablePolling(e, this.pollingRef), this.activePolling = this.activePolling.filter((t => t !== e))
                 }
             }
-            const Et = (0, g.createUseStyles)({
-                    root: {
-                        padding: "8px",
-                        border: "1px solid var(--jp-warn-color1)",
-                        color: "var(--jp-warn-color1)",
-                        borderRadius: "4px",
-                        maxWidth: "400px",
-                        display: "flex",
-                        flexDirection: "row",
-                        alignItems: "center"
-                    },
-                    icon: {
-                        color: "var(--jp-warn-color1)"
-                    },
-                    textContainer: {
-                        flex: 1,
-                        paddingLeft: "8px"
-                    }
-                }),
-                xt = e => {
-                    var {
-                        children: t
-                    } = e, a = function(e, t) {
-                        var a = {};
-                        for (var n in e) Object.prototype.hasOwnProperty.call(e, n) && t.indexOf(n) < 0 && (a[n] = e[n]);
-                        if (null != e && "function" == typeof Object.getOwnPropertySymbols) {
-                            var o = 0;
-                            for (n = Object.getOwnPropertySymbols(e); o < n.length; o++) t.indexOf(n[o]) < 0 && Object.prototype.propertyIsEnumerable.call(e, n[o]) && (a[n[o]] = e[n[o]])
-                        }
-                        return a
-                    }(e, ["children"]);
-                    const n = Et();
-                    return c().createElement("div", Object.assign({
-                        className: n.root
-                    }, a), c().createElement("div", null, c().createElement("i", {
-                        className: `material-icons ${n.icon}`
-                    }, "warning")), c().createElement("div", {
-                        className: n.textContainer
-                    }, t))
-                };
-            var yt;
-            ! function(e) {
-                class t extends f.VDomModel {
-                    constructor() {
-                        super(...arguments), this._rses = [], this._rse = "", this._lifetime = "", this._scopes = [], this._selectedScope = "", this._selectedDatasetScope = "", this._datasetName = "", this._scopesLoading = !1, this._rsesLoading = !1, this._addToDataset = !1
-                    }
-                    get rses() {
-                        return this._rses
-                    }
-                    set rses(e) {
-                        this._rses = e, this.stateChanged.emit(void 0)
-                    }
-                    set rse(e) {
-                        this._rse = e, this.stateChanged.emit(void 0)
-                    }
-                    get rse() {
-                        return this._rse
-                    }
-                    set lifetime(e) {
-                        this._lifetime = e, this.stateChanged.emit(void 0)
-                    }
-                    get lifetime() {
-                        return this._lifetime
-                    }
-                    get scopes() {
-                        return this._scopes
-                    }
-                    set scopes(e) {
-                        this._scopes = e, this.stateChanged.emit(void 0)
-                    }
-                    get selectedScope() {
-                        return this._selectedScope
-                    }
-                    set selectedScope(e) {
-                        this._selectedScope = e, this.stateChanged.emit(void 0)
-                    }
-                    get selectedDatasetScope() {
-                        return this._selectedDatasetScope
-                    }
-                    set selectedDatasetScope(e) {
-                        this._selectedDatasetScope = e, this.stateChanged.emit(void 0)
-                    }
-                    get datasetName() {
-                        return this._datasetName
-                    }
-                    set datasetName(e) {
-                        this._datasetName = e, this.stateChanged.emit(void 0)
-                    }
-                    get scopesLoading() {
-                        return this._scopesLoading
-                    }
-                    set scopesLoading(e) {
-                        this._scopesLoading = e, this.stateChanged.emit(void 0)
-                    }
-                    get rsesLoading() {
-                        return this._rsesLoading
-                    }
-                    set rsesLoading(e) {
-                        this._rsesLoading = e, this.stateChanged.emit(void 0)
-                    }
-                    get addToDataset() {
-                        return this._addToDataset
-                    }
-                    set addToDataset(e) {
-                        this._addToDataset = e, this.stateChanged.emit(void 0)
-                    }
-                }
-                e.Model = t;
-                class a extends f.VDomRenderer {
-                    constructor(t) {
-                        super(new e.Model), this.files = t
-                    }
-                    onAfterAttach() {
-                        const {
-                            activeInstance: e
-                        } = C.getRawState();
-                        e && (this.model.scopesLoading = !0, $.fetchScopes(e.name).then((e => {
-                            e.sort(((e, t) => e.localeCompare(t))), this.model.scopes = e
-                        })).finally((() => this.model.scopesLoading = !1)), this.model.rsesLoading = !0, $.fetchRSEs(e.name, "availability_write=True").then((e => {
-                            e.sort(((e, t) => e.localeCompare(t))), this.model.rses = e
-                        })).finally((() => this.model.rsesLoading = !1)))
-                    }
-                    render() {
-                        const e = {
-                                control: (e, t) => Object.assign(Object.assign({}, e), {
-                                    borderRadius: 0,
-                                    borderColor: "var(--jp-border-color1)",
-                                    background: "var(--jp-layout-color1)",
-                                    marginLeft: "1px",
-                                    marginRight: "1px"
-                                }),
-                                singleValue: (e, t) => Object.assign(Object.assign({}, e), {
-                                    color: "var(--jp-ui-font-color1)"
-                                }),
-                                menu: (e, t) => Object.assign(Object.assign({}, e), {
-                                    background: "var(--jp-layout-color1)",
-                                    color: "var(--jp-ui-font-color1)"
-                                }),
-                                menuPortal: e => Object.assign(Object.assign({}, e), {
-                                    zIndex: 99999
-                                }),
-                                option: (e, {
-                                    isFocused: t,
-                                    isSelected: a
-                                }) => Object.assign(Object.assign({}, e), {
-                                    background: t ? a ? e.background : "var(--jp-layout-color2)" : e.background,
-                                    ":active": Object.assign(Object.assign({}, e[":active"]), {
-                                        background: a ? e.background : "var(--jp-layout-color2)"
-                                    })
-                                })
-                            },
-                            {
-                                activeAuthType: t
-                            } = C.getRawState();
-                        return c().createElement("div", null, this.files.length > 1 && c().createElement("h2", {
-                            style: {
-                                marginTop: 0
-                            }
-                        }, "Upload ", this.files.length, " files to Rucio"), 1 === this.files.length && c().createElement("h2", {
-                            style: {
-                                marginTop: 0
-                            }
-                        }, "Upload ", this.files[0].name, " to Rucio"), !("x509" === t || "x509_proxy" === t) && c().createElement(xt, {
-                            style: {
-                                marginTop: "8px",
-                                marginBottom: "8px"
-                            }
-                        }, "You are not using X509 as the authentication method, upload may fail if the destination RSE does not support your authentication method."), c().createElement("p", {
-                            style: {
-                                marginTop: "16px"
-                            }
-                        }, "Destination RSE:"), c().createElement("div", {
-                            style: {
-                                marginTop: "4px",
-                                marginBottom: "8px"
-                            }
-                        }, c().createElement(Ke(), {
-                            isLoading: this.model.rsesLoading,
-                            menuPortalTarget: document.body,
-                            styles: e,
-                            options: this.model.rses.map((e => ({
-                                value: e,
-                                label: e
-                            }))),
-                            defaultValue: {
-                                value: this.model.rse,
-                                label: this.model.rse
-                            },
-                            onChange: e => this.model.rse = e.value
-                        })), c().createElement("p", {
-                            style: {
-                                marginTop: "16px"
-                            }
-                        }, "Lifetime (in seconds):"), c().createElement(A, {
-                            type: "number",
-                            value: this.model.lifetime,
-                            placeholder: "Leave empty for indefinite",
-                            onChange: e => this.model.lifetime = e.target.value,
-                            containerStyle: {
-                                marginTop: "4px",
-                                marginBottom: "8px"
-                            }
-                        }), c().createElement("p", {
-                            style: {
-                                marginTop: "16px"
-                            }
-                        }, "Scope:"), c().createElement("div", {
-                            style: {
-                                marginTop: "4px",
-                                marginBottom: "8px"
-                            }
-                        }, c().createElement(Ke(), {
-                            isLoading: this.model.scopesLoading,
-                            menuPortalTarget: document.body,
-                            styles: e,
-                            options: this.model.scopes.map((e => ({
-                                value: e,
-                                label: e
-                            }))),
-                            defaultValue: {
-                                value: this.model.selectedScope,
-                                label: this.model.selectedScope
-                            },
-                            onChange: e => this.model.selectedScope = e.value
-                        })), c().createElement(c().Fragment, null, c().createElement("label", null, c().createElement("input", {
-                            type: "checkbox",
-                            checked: this.model.addToDataset,
-                            onChange: e => this.model.addToDataset = e.target.checked
-                        }), "Add files to a dataset"), this.model.addToDataset && c().createElement("div", {
-                            style: {
-                                marginTop: "16px"
-                            }
-                        }, c().createElement("p", null, "Dataset Scope:"), c().createElement("div", {
-                            style: {
-                                marginTop: "4px",
-                                marginBottom: "8px"
-                            }
-                        }, c().createElement(Ke(), {
-                            isLoading: this.model.scopesLoading,
-                            menuPortalTarget: document.body,
-                            styles: e,
-                            options: this.model.scopes.map((e => ({
-                                value: e,
-                                label: e
-                            }))),
-                            defaultValue: {
-                                value: this.model.selectedDatasetScope,
-                                label: this.model.selectedDatasetScope
-                            },
-                            onChange: e => this.model.selectedDatasetScope = e.value
-                        })), c().createElement("p", {
-                            style: {
-                                marginTop: "16px"
-                            }
-                        }, "Dataset Name:"), c().createElement(A, {
-                            value: this.model.datasetName,
-                            onChange: e => this.model.datasetName = e.target.value,
-                            containerStyle: {
-                                marginTop: "4px",
-                                marginBottom: "8px"
-                            }
-                        }))))
-                    }
-                    getValue() {
-                        return {
-                            rse: this.model.rse,
-                            lifetime: this.model.lifetime,
-                            fileScope: this.model.selectedScope,
-                            datasetScope: this.model.selectedDatasetScope,
-                            datasetName: this.model.datasetName,
-                            addToDataset: this.model.addToDataset
-                        }
-                    }
-                }
-                e.DialogBody = a
-            }(yt || (yt = {}));
-            class Ct extends f.Dialog {
-                constructor(e) {
-                    super({
-                        title: c().createElement(E, null),
-                        body: new yt.DialogBody(e),
-                        buttons: [f.Dialog.cancelButton(), f.Dialog.okButton({
-                            label: "Upload"
-                        })]
-                    })
-                }
-                handleEvent(e) {
-                    "keydown" === e.type && "Enter" === e.key || super.handleEvent(e)
-                }
-            }
-            const Nt = {
-                id: d,
+            const Et = {
+                id: s,
                 autoStart: !0,
-                requires: [n.ILabShell, o.INotebookTracker, i.IFileBrowserFactory],
-                activate: async (e, t, a, n) => {
+                requires: [a.ILabShell, o.INotebookTracker, r.IFileBrowserFactory],
+                activate: async (e, t, n, a) => {
                     try {
-                        ! function(e, t, a) {
-                            const n = new gt({
+                        ! function(e, t, n) {
+                            const a = new gt({
                                 app: e,
-                                instanceConfig: a
+                                instanceConfig: n
                             });
-                            n.id = d + ":panel", t.add(n, "left", {
+                            a.id = s + ":panel", t.add(a, "left", {
                                 rank: 900
-                            }), t.activateById(n.id)
-                        }(e, t, await $.fetchInstancesConfig()),
-                        function(e, t, a) {
-                            const n = new ze({
+                            }), t.activateById(a.id)
+                        }(e, t, await _.fetchInstancesConfig()),
+                        function(e, t, n) {
+                            const a = new Ue({
                                 labShell: t,
-                                notebookTracker: a,
+                                notebookTracker: n,
                                 sessionManager: e.serviceManager.sessions
                             });
                             new ft({
                                 labShell: t,
-                                notebookTracker: a,
+                                notebookTracker: n,
                                 sessionManager: e.serviceManager.sessions,
-                                notebookListener: n
-                            }), new bt(n)
-                        }(e, t, a),
-                        function(e, t) {
-                            e.commands.addCommand(v.UploadFile, {
-                                icon: l.fileUploadIcon,
-                                label: "Upload File(s) to Rucio",
-                                execute: async () => {
-                                    const e = t.tracker.currentWidget;
-                                    if (e) {
-                                        const t = (0, r.toArray)(e.selectedItems()).filter((e => "directory" !== e.type));
-                                        if (0 === t.length) return;
-                                        !async function(e) {
-                                            const t = new Ct(e),
-                                                a = await t.launch(),
-                                                {
-                                                    activeInstance: n
-                                                } = C.getRawState();
-                                            if (n && a.value) {
-                                                const {
-                                                    rse: t,
-                                                    lifetime: o,
-                                                    fileScope: l,
-                                                    datasetScope: i,
-                                                    datasetName: r,
-                                                    addToDataset: s
-                                                } = a.value;
-                                                if (!t || !l) return void(0, f.showErrorMessage)("Upload cancelled", "Destination RSE and/or scope is not specified.");
-                                                if (s && (!i || !r)) return void(0, f.showErrorMessage)("Upload cancelled", "Dataset scope and/or name is not specified.");
-                                                await $.uploadFile(n.name, {
-                                                    paths: e.map((e => e.path)),
-                                                    rse: t,
-                                                    lifetime: o ? parseInt(o) : void 0,
-                                                    fileScope: l,
-                                                    datasetScope: i,
-                                                    datasetName: r,
-                                                    addToDataset: s
-                                                }), (0, f.showErrorMessage)("Upload is commencing", "Your files are uploading, you can see the upload status on the Rucio sidebar.")
-                                            }
-                                        }(t)
-                                    }
-                                }
-                            }), e.contextMenu.addItem({
-                                command: v.UploadFile,
-                                selector: '.jp-DirListing-item[data-isdir="false"]',
-                                rank: 10
-                            })
-                        }(e, n)
+                                notebookListener: a
+                            }), new bt(a)
+                        }(e, t, n)
                     } catch (e) {
                         console.log(e)
                     }
                 }
             }
         },
         2587: e => {
             function t(e, t) {
                 return Object.prototype.hasOwnProperty.call(e, t)
             }
-            e.exports = function(e, a, n, o) {
-                a = a || "&", n = n || "=";
+            e.exports = function(e, n, a, o) {
+                n = n || "&", a = a || "=";
                 var l = {};
                 if ("string" != typeof e || 0 === e.length) return l;
-                var i = /\+/g;
-                e = e.split(a);
-                var r = 1e3;
-                o && "number" == typeof o.maxKeys && (r = o.maxKeys);
-                var s = e.length;
-                r > 0 && s > r && (s = r);
-                for (var c = 0; c < s; ++c) {
-                    var d, m, p, u, v = e[c].replace(i, "%20"),
-                        h = v.indexOf(n);
+                var r = /\+/g;
+                e = e.split(n);
+                var i = 1e3;
+                o && "number" == typeof o.maxKeys && (i = o.maxKeys);
+                var c = e.length;
+                i > 0 && c > i && (c = i);
+                for (var s = 0; s < c; ++s) {
+                    var d, m, p, u, v = e[s].replace(r, "%20"),
+                        h = v.indexOf(a);
                     h >= 0 ? (d = v.substr(0, h), m = v.substr(h + 1)) : (d = v, m = ""), p = decodeURIComponent(d), u = decodeURIComponent(m), t(l, p) ? Array.isArray(l[p]) ? l[p].push(u) : l[p] = [l[p], u] : l[p] = u
                 }
                 return l
             }
         },
         2361: e => {
             var t = function(e) {
@@ -4060,21 +3722,21 @@
                         return e ? "true" : "false";
                     case "number":
                         return isFinite(e) ? e : "";
                     default:
                         return ""
                 }
             };
-            e.exports = function(e, a, n, o) {
-                return a = a || "&", n = n || "=", null === e && (e = void 0), "object" == typeof e ? Object.keys(e).map((function(o) {
-                    var l = encodeURIComponent(t(o)) + n;
+            e.exports = function(e, n, a, o) {
+                return n = n || "&", a = a || "=", null === e && (e = void 0), "object" == typeof e ? Object.keys(e).map((function(o) {
+                    var l = encodeURIComponent(t(o)) + a;
                     return Array.isArray(e[o]) ? e[o].map((function(e) {
                         return l + encodeURIComponent(t(e))
-                    })).join(a) : l + encodeURIComponent(t(e[o]))
-                })).join(a) : o ? encodeURIComponent(t(o)) + n + encodeURIComponent(t(e)) : ""
+                    })).join(n) : l + encodeURIComponent(t(e[o]))
+                })).join(n) : o ? encodeURIComponent(t(o)) + a + encodeURIComponent(t(e)) : ""
             }
         },
-        7673: (e, t, a) => {
-            t.decode = t.parse = a(2587), t.encode = t.stringify = a(2361)
+        7673: (e, t, n) => {
+            t.decode = t.parse = n(2587), t.encode = t.stringify = n(2361)
         }
     }
 ]);
```

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/labextension/static/448.47f3f7fec352ce0129f5.js` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/labextension/static/448.47f3f7fec352ce0129f5.js`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/labextension/static/594.bb16e01fd6647f801c63.js` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/labextension/static/594.bb16e01fd6647f801c63.js`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/labextension/static/608.9fe7f346a912ad2fd318.js` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/labextension/static/608.9fe7f346a912ad2fd318.js`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/labextension/static/61.3ba6ce361770a986be36.js` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/labextension/static/61.3ba6ce361770a986be36.js`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/labextension/static/728.5c0c1b3668a79b1563d4.js` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/labextension/static/728.5c0c1b3668a79b1563d4.js`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/labextension/static/855.fd11e9ed650c9ff9d8e6.js` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/labextension/static/855.fd11e9ed650c9ff9d8e6.js`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/labextension/static/937.d7571d64b2695fcc8cb8.js` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/labextension/static/937.d7571d64b2695fcc8cb8.js`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/labextension/static/remoteEntry.13b02eee40e64df104ad.js` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/labextension/static/remoteEntry.ce6881670499ee5dfee1.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
     var e, r, t, a, o, n, l, i, u, d, c, f, s, p, b, h, v, m, y = {
             7309: (e, r, t) => {
                 var a = {
-                        "./index": () => Promise.all([t.e(271), t.e(437)]).then((() => () => t(1437))),
-                        "./extension": () => Promise.all([t.e(271), t.e(437)]).then((() => () => t(1437))),
+                        "./index": () => Promise.all([t.e(271), t.e(162)]).then((() => () => t(4162))),
+                        "./extension": () => Promise.all([t.e(271), t.e(162)]).then((() => () => t(4162))),
                         "./style": () => t.e(130).then((() => () => t(4130)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     n = (e, r) => {
                         if (t.S) {
@@ -47,33 +47,33 @@
             enumerable: !0,
             get: r[t]
         })
     }, w.f = {}, w.e = e => Promise.all(Object.keys(w.f).reduce(((r, t) => (w.f[t](e, r), r)), [])), w.u = e => e + "." + {
         20: "53c11c5b79a94ee424cb",
         61: "3ba6ce361770a986be36",
         130: "7365b614084ad0cbc49d",
+        162: "f78f93f2c02451004fb9",
         271: "33fc31001c0f0927aeb2",
         392: "c6f78101fd8442eea43d",
         429: "407b01bdf4a8a104bc25",
-        437: "e8e22924cb4070990f2f",
         448: "47f3f7fec352ce0129f5",
         456: "e8372238df39d8fd11b6",
         594: "bb16e01fd6647f801c63",
         608: "9fe7f346a912ad2fd318",
         728: "5c0c1b3668a79b1563d4",
         855: "fd11e9ed650c9ff9d8e6",
         937: "d7571d64b2695fcc8cb8"
     } [e] + ".js?v=" + {
         20: "53c11c5b79a94ee424cb",
         61: "3ba6ce361770a986be36",
         130: "7365b614084ad0cbc49d",
+        162: "f78f93f2c02451004fb9",
         271: "33fc31001c0f0927aeb2",
         392: "c6f78101fd8442eea43d",
         429: "407b01bdf4a8a104bc25",
-        437: "e8e22924cb4070990f2f",
         448: "47f3f7fec352ce0129f5",
         456: "e8372238df39d8fd11b6",
         594: "bb16e01fd6647f801c63",
         608: "9fe7f346a912ad2fd318",
         728: "5c0c1b3668a79b1563d4",
         855: "fd11e9ed650c9ff9d8e6",
         937: "d7571d64b2695fcc8cb8"
@@ -139,15 +139,15 @@
                             from: l,
                             eager: !!a
                         })
                     },
                     u = [];
                 switch (t) {
                     case "default":
-                        i("camelcase-keys-deep", "0.1.0", (() => w.e(429).then((() => () => w(2429))))), i("pullstate", "1.22.1", (() => Promise.all([w.e(20), w.e(271)]).then((() => () => w(1020))))), i("react-copy-to-clipboard", "5.0.4", (() => Promise.all([w.e(271), w.e(855)]).then((() => () => w(4855))))), i("react-jss", "10.7.1", (() => Promise.all([w.e(448), w.e(271)]).then((() => () => w(3448))))), i("react-popover", "0.5.10", (() => Promise.all([w.e(608), w.e(271), w.e(456)]).then((() => () => w(7608))))), i("react-select", "3.2.0", (() => Promise.all([w.e(937), w.e(271), w.e(456)]).then((() => () => w(4937))))), i("react-virtualized-auto-sizer", "1.0.6", (() => Promise.all([w.e(271), w.e(728)]).then((() => () => w(1728))))), i("react-window", "1.8.6", (() => Promise.all([w.e(61), w.e(271)]).then((() => () => w(4061))))), i("rucio-jupyterlab", "0.9.7", (() => Promise.all([w.e(271), w.e(437)]).then((() => () => w(1437)))))
+                        i("camelcase-keys-deep", "0.1.0", (() => w.e(429).then((() => () => w(2429))))), i("pullstate", "1.22.1", (() => Promise.all([w.e(20), w.e(271)]).then((() => () => w(1020))))), i("react-copy-to-clipboard", "5.0.4", (() => Promise.all([w.e(271), w.e(855)]).then((() => () => w(4855))))), i("react-jss", "10.7.1", (() => Promise.all([w.e(448), w.e(271)]).then((() => () => w(3448))))), i("react-popover", "0.5.10", (() => Promise.all([w.e(608), w.e(271), w.e(456)]).then((() => () => w(7608))))), i("react-select", "3.2.0", (() => Promise.all([w.e(937), w.e(271), w.e(456)]).then((() => () => w(4937))))), i("react-virtualized-auto-sizer", "1.0.6", (() => Promise.all([w.e(271), w.e(728)]).then((() => () => w(1728))))), i("react-window", "1.8.6", (() => Promise.all([w.e(61), w.e(271)]).then((() => () => w(4061))))), i("rucio-jupyterlab", "0.9.8", (() => Promise.all([w.e(271), w.e(162)]).then((() => () => w(4162)))))
                 }
                 return e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         w.g.importScripts && (e = w.g.location + "");
@@ -247,34 +247,34 @@
         var n = w.I(r);
         return n && n.then ? n.then(e.bind(e, r, w.S[r], t, a, o)) : e(r, w.S[r], t, a, o)
     })(((e, r, t, a) => (l(e, t), d(r, 0, t, a)))), b = s(((e, r, t, a, o) => {
         var n = r && w.o(r, t) && c(r, t, a);
         return n ? f(n) : o()
     })), h = {}, v = {
         6271: () => p("default", "react", [1, 17, 0, 1]),
-        309: () => p("default", "@jupyterlab/notebook", [1, 3, 4, 2]),
-        362: () => p("default", "@jupyterlab/application", [1, 3, 4, 2]),
         454: () => b("default", "react-popover", [2, 0, 5, 10], (() => Promise.all([w.e(608), w.e(456)]).then((() => () => w(7608))))),
+        613: () => p("default", "@jupyterlab/notebook", [1, 3, 4, 8]),
         1626: () => b("default", "react-select", [1, 3, 1, 0], (() => Promise.all([w.e(937), w.e(456)]).then((() => () => w(4937))))),
         2638: () => b("default", "react-copy-to-clipboard", [1, 5, 0, 2], (() => w.e(594).then((() => () => w(4855))))),
+        3655: () => p("default", "@jupyterlab/ui-components", [1, 3, 4, 8]),
         3760: () => b("default", "camelcase-keys-deep", [2, 0, 1, 0], (() => w.e(429).then((() => () => w(2429))))),
-        4057: () => p("default", "@jupyterlab/apputils", [1, 3, 4, 2]),
-        4139: () => p("default", "@jupyterlab/services", [1, 6, 4, 2]),
+        4306: () => p("default", "@jupyterlab/filebrowser", [1, 3, 4, 8]),
+        5012: () => p("default", "@jupyterlab/coreutils", [1, 5, 4, 8]),
+        5322: () => p("default", "@jupyterlab/services", [1, 6, 4, 8]),
         5766: () => b("default", "pullstate", [1, 1, 13, 2], (() => w.e(20).then((() => () => w(1020))))),
         7370: () => b("default", "react-window", [1, 1, 8, 6], (() => w.e(61).then((() => () => w(4061))))),
-        7697: () => p("default", "@jupyterlab/coreutils", [1, 5, 4, 2]),
         8053: () => b("default", "react-jss", [1, 10, 1, 1], (() => w.e(448).then((() => () => w(3448))))),
         8196: () => b("default", "react-virtualized-auto-sizer", [1, 1, 0, 2], (() => w.e(392).then((() => () => w(1728))))),
         8918: () => p("default", "@lumino/algorithm", [1, 1, 9, 0]),
-        9839: () => p("default", "@jupyterlab/filebrowser", [1, 3, 4, 2]),
-        9876: () => p("default", "@jupyterlab/ui-components", [1, 3, 4, 2]),
+        9061: () => p("default", "@jupyterlab/apputils", [1, 3, 4, 8]),
+        9334: () => p("default", "@jupyterlab/application", [1, 3, 4, 8]),
         4456: () => p("default", "react-dom", [1, 17, 0, 1])
     }, m = {
+        162: [454, 613, 1626, 2638, 3655, 3760, 4306, 5012, 5322, 5766, 7370, 8053, 8196, 8918, 9061, 9334],
         271: [6271],
-        437: [309, 362, 454, 1626, 2638, 3760, 4057, 4139, 5766, 7370, 7697, 8053, 8196, 8918, 9839, 9876],
         456: [4456]
     }, w.f.consumes = (e, r) => {
         w.o(m, e) && m[e].forEach((e => {
             if (w.o(h, e)) return r.push(h[e]);
             var t = r => {
                     h[e] = 0, w.m[e] = t => {
                         delete w.c[e], t.exports = r()
```

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/labextension/static/third-party-licenses.json` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/mode_handlers/download.py` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/mode_handlers/download.py`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/mode_handlers/replica.py` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/mode_handlers/replica.py`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/rucio/authenticators.py` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/rucio/authenticators.py`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/rucio/client_environment.py` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/rucio/client_environment.py`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/rucio/download.py` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/rucio/download.py`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/rucio/rucio.py` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/rucio/rucio.py`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/rucio/upload.py` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/rucio/upload.py`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/rucio/utils.py` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/rucio/utils.py`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/server.py` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/server.py`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab/utils.py` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab/utils.py`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab.egg-info/PKG-INFO` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rucio-jupyterlab
-Version: 0.9.7
+Version: 0.9.8
 Summary: JupyterLab extension for integrating Rucio
 Home-page: https://github.com/rucio/jupyterlab-extension
 Author: Muhammad Aditya Hilmy
 Author-email: mhilmy@hey.com
 License: Apache-2.0
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `rucio_jupyterlab-0.9.7/rucio_jupyterlab.egg-info/SOURCES.txt` & `rucio_jupyterlab-0.9.8/rucio_jupyterlab.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -52,28 +52,28 @@
 rucio_jupyterlab/handlers/upload_jobs_details.py
 rucio_jupyterlab/handlers/upload_jobs_log.py
 rucio_jupyterlab/kernels/__init__.py
 rucio_jupyterlab/kernels/ipython/__init__.py
 rucio_jupyterlab/kernels/ipython/types.py
 rucio_jupyterlab/labextension/package.json
 rucio_jupyterlab/labextension/static/130.7365b614084ad0cbc49d.js
+rucio_jupyterlab/labextension/static/162.f78f93f2c02451004fb9.js
 rucio_jupyterlab/labextension/static/20.53c11c5b79a94ee424cb.js
 rucio_jupyterlab/labextension/static/392.c6f78101fd8442eea43d.js
 rucio_jupyterlab/labextension/static/429.407b01bdf4a8a104bc25.js
-rucio_jupyterlab/labextension/static/437.e8e22924cb4070990f2f.js
 rucio_jupyterlab/labextension/static/448.47f3f7fec352ce0129f5.js
 rucio_jupyterlab/labextension/static/448.47f3f7fec352ce0129f5.js.LICENSE.txt
 rucio_jupyterlab/labextension/static/594.bb16e01fd6647f801c63.js
 rucio_jupyterlab/labextension/static/608.9fe7f346a912ad2fd318.js
 rucio_jupyterlab/labextension/static/608.9fe7f346a912ad2fd318.js.LICENSE.txt
 rucio_jupyterlab/labextension/static/61.3ba6ce361770a986be36.js
 rucio_jupyterlab/labextension/static/728.5c0c1b3668a79b1563d4.js
 rucio_jupyterlab/labextension/static/855.fd11e9ed650c9ff9d8e6.js
 rucio_jupyterlab/labextension/static/937.d7571d64b2695fcc8cb8.js
-rucio_jupyterlab/labextension/static/remoteEntry.13b02eee40e64df104ad.js
+rucio_jupyterlab/labextension/static/remoteEntry.ce6881670499ee5dfee1.js
 rucio_jupyterlab/labextension/static/style.js
 rucio_jupyterlab/labextension/static/third-party-licenses.json
 rucio_jupyterlab/mode_handlers/__init__.py
 rucio_jupyterlab/mode_handlers/download.py
 rucio_jupyterlab/mode_handlers/replica.py
 rucio_jupyterlab/rucio/__init__.py
 rucio_jupyterlab/rucio/authenticators.py
```

### Comparing `rucio_jupyterlab-0.9.7/setup.py` & `rucio_jupyterlab-0.9.8/setup.py`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/src/commands/uploadFile.ts` & `rucio_jupyterlab-0.9.8/src/commands/uploadFile.ts`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/src/components/@Explore/AddToNotebookPopover.tsx` & `rucio_jupyterlab-0.9.8/src/components/@Explore/AddToNotebookPopover.tsx`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/src/components/@Explore/CollectionDIDItemDetails.tsx` & `rucio_jupyterlab-0.9.8/src/components/@Explore/CollectionDIDItemDetails.tsx`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/src/components/@Explore/DIDListItem.tsx` & `rucio_jupyterlab-0.9.8/src/components/@Explore/DIDListItem.tsx`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/src/components/@Explore/ExploreTab.tsx` & `rucio_jupyterlab-0.9.8/src/components/@Explore/ExploreTab.tsx`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/src/components/@Explore/FileDIDItemDetails.tsx` & `rucio_jupyterlab-0.9.8/src/components/@Explore/FileDIDItemDetails.tsx`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/src/components/@Explore/InlineDropdown.tsx` & `rucio_jupyterlab-0.9.8/src/components/@Explore/InlineDropdown.tsx`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/src/components/@Explore/ListAttachedFilesPopover.tsx` & `rucio_jupyterlab-0.9.8/src/components/@Explore/ListAttachedFilesPopover.tsx`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/src/components/@Explore/ListScopesPopover.tsx` & `rucio_jupyterlab-0.9.8/src/components/@Explore/ListScopesPopover.tsx`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/src/components/@Notebook/NotebookAttachmentListItem.tsx` & `rucio_jupyterlab-0.9.8/src/components/@Notebook/NotebookAttachmentListItem.tsx`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/src/components/@Notebook/NotebookTab.tsx` & `rucio_jupyterlab-0.9.8/src/components/@Notebook/NotebookTab.tsx`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/src/components/@Settings/FilePickerPopover.tsx` & `rucio_jupyterlab-0.9.8/src/components/@Settings/FilePickerPopover.tsx`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/src/components/@Settings/SettingsTab.tsx` & `rucio_jupyterlab-0.9.8/src/components/@Settings/SettingsTab.tsx`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/src/components/@Settings/UserPassAuth.tsx` & `rucio_jupyterlab-0.9.8/src/components/@Settings/UserPassAuth.tsx`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/src/components/@Settings/X509Auth.tsx` & `rucio_jupyterlab-0.9.8/src/components/@Settings/X509Auth.tsx`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/src/components/@Settings/X509ProxyAuth.tsx` & `rucio_jupyterlab-0.9.8/src/components/@Settings/X509ProxyAuth.tsx`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/src/components/@Uploads/UploadJobListItem.tsx` & `rucio_jupyterlab-0.9.8/src/components/@Uploads/UploadJobListItem.tsx`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/src/components/@Uploads/UploadsTab.tsx` & `rucio_jupyterlab-0.9.8/src/components/@Uploads/UploadsTab.tsx`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/src/components/Alert.tsx` & `rucio_jupyterlab-0.9.8/src/components/Alert.tsx`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/src/components/Button.tsx` & `rucio_jupyterlab-0.9.8/src/components/Button.tsx`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/src/components/Header.tsx` & `rucio_jupyterlab-0.9.8/src/components/Header.tsx`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/src/components/HorizontalHeading.tsx` & `rucio_jupyterlab-0.9.8/src/components/HorizontalHeading.tsx`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/src/components/MenuBar.tsx` & `rucio_jupyterlab-0.9.8/src/components/MenuBar.tsx`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/src/components/RucioLogo.tsx` & `rucio_jupyterlab-0.9.8/src/components/RucioLogo.tsx`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/src/components/Spinning.tsx` & `rucio_jupyterlab-0.9.8/src/components/Spinning.tsx`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/src/components/TextField.tsx` & `rucio_jupyterlab-0.9.8/src/components/TextField.tsx`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/src/const.ts` & `rucio_jupyterlab-0.9.8/src/const.ts`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/src/icons/RucioIcon.tsx` & `rucio_jupyterlab-0.9.8/src/icons/RucioIcon.tsx`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/src/index.ts` & `rucio_jupyterlab-0.9.8/src/index.ts`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     notebookTracker: INotebookTracker,
     fileBrowserFactory: IFileBrowserFactory
   ) => {
     try {
       const instanceConfig = await actions.fetchInstancesConfig();
       activateSidebarPanel(app, labShell, instanceConfig);
       activateNotebookListener(app, labShell, notebookTracker);
-      activateRucioUploadWidget(app, fileBrowserFactory);
+      //       activateRucioUploadWidget(app, fileBrowserFactory);
     } catch (e) {
       console.log(e);
     }
   }
 };
 
 function activateSidebarPanel(app: JupyterFrontEnd, labShell: ILabShell, instanceConfig: InstanceConfig) {
```

### Comparing `rucio_jupyterlab-0.9.7/src/stores/ExtensionStore.ts` & `rucio_jupyterlab-0.9.8/src/stores/ExtensionStore.ts`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/src/stores/UIStore.ts` & `rucio_jupyterlab-0.9.8/src/stores/UIStore.ts`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/src/types.ts` & `rucio_jupyterlab-0.9.8/src/types.ts`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/src/utils/Actions.tsx` & `rucio_jupyterlab-0.9.8/src/utils/Actions.tsx`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/src/utils/ActiveNotebookListener.ts` & `rucio_jupyterlab-0.9.8/src/utils/ActiveNotebookListener.ts`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/src/utils/ApiRequest.ts` & `rucio_jupyterlab-0.9.8/src/utils/ApiRequest.ts`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/src/utils/DIDPollingManager.tsx` & `rucio_jupyterlab-0.9.8/src/utils/DIDPollingManager.tsx`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/src/utils/Helpers.ts` & `rucio_jupyterlab-0.9.8/src/utils/Helpers.ts`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/src/utils/NotebookListener.ts` & `rucio_jupyterlab-0.9.8/src/utils/NotebookListener.ts`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/src/utils/NotebookPollingListener.ts` & `rucio_jupyterlab-0.9.8/src/utils/NotebookPollingListener.ts`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/src/utils/useInterval.ts` & `rucio_jupyterlab-0.9.8/src/utils/useInterval.ts`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/src/widgets/InjectNotebookToolbar.tsx` & `rucio_jupyterlab-0.9.8/src/widgets/InjectNotebookToolbar.tsx`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/src/widgets/RucioUploadDialog.tsx` & `rucio_jupyterlab-0.9.8/src/widgets/RucioUploadDialog.tsx`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/src/widgets/SidebarPanel.tsx` & `rucio_jupyterlab-0.9.8/src/widgets/SidebarPanel.tsx`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/src/widgets/UploadLogViewerWidget.tsx` & `rucio_jupyterlab-0.9.8/src/widgets/UploadLogViewerWidget.tsx`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/style/index.css` & `rucio_jupyterlab-0.9.8/style/index.css`

 * *Files identical despite different names*

### Comparing `rucio_jupyterlab-0.9.7/tsconfig.json` & `rucio_jupyterlab-0.9.8/tsconfig.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9930555555555556%*

 * *Differences: {"'compilerOptions'": "{'noUnusedLocals': False}"}*

```diff
@@ -6,15 +6,15 @@
         "esModuleInterop": true,
         "incremental": true,
         "jsx": "react",
         "module": "esnext",
         "moduleResolution": "node",
         "noEmitOnError": true,
         "noImplicitAny": true,
-        "noUnusedLocals": true,
+        "noUnusedLocals": false,
         "outDir": "lib",
         "preserveWatchOutput": true,
         "resolveJsonModule": true,
         "strict": true,
         "strictNullChecks": true,
         "target": "es2017",
         "types": [
```

### Comparing `rucio_jupyterlab-0.9.7/yarn.lock` & `rucio_jupyterlab-0.9.8/yarn.lock`

 * *Files identical despite different names*

