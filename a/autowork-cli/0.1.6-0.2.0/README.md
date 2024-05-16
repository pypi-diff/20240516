# Comparing `tmp/autowork-cli-0.1.6.tar.gz` & `tmp/autowork-cli-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autowork-cli-0.1.6.tar", last modified: Wed Oct 11 06:46:46 2023, max compression
+gzip compressed data, was "autowork-cli-0.2.0.tar", last modified: Fri Mar 29 10:42:36 2024, max compression
```

## Comparing `autowork-cli-0.1.6.tar` & `autowork-cli-0.2.0.tar`

### file list

```diff
@@ -1,93 +1,119 @@
-drwxrwxrwx   0        0        0        0 2023-10-11 06:46:46.478920 autowork-cli-0.1.6/
--rw-rw-rw-   0        0        0      118 2023-10-11 06:46:46.478920 autowork-cli-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      954 2023-09-08 11:45:37.000000 autowork-cli-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-10-11 06:46:46.329331 autowork-cli-0.1.6/autowork_cli/
--rw-rw-rw-   0        0        0        0 2023-09-08 10:30:56.000000 autowork-cli-0.1.6/autowork_cli/__init__.py
--rw-rw-rw-   0        0        0     1282 2023-09-13 06:06:10.000000 autowork-cli-0.1.6/autowork_cli/__main__.py
-drwxrwxrwx   0        0        0        0 2023-10-11 06:46:46.348889 autowork-cli-0.1.6/autowork_cli/cf/
--rw-rw-rw-   0        0        0        0 2023-09-08 10:30:56.000000 autowork-cli-0.1.6/autowork_cli/cf/__init__.py
--rw-rw-rw-   0        0        0     1788 2023-09-27 10:07:51.000000 autowork-cli-0.1.6/autowork_cli/cf/cf_cmd.py
-drwxrwxrwx   0        0        0        0 2023-10-11 06:46:46.348889 autowork-cli-0.1.6/autowork_cli/common/
--rw-rw-rw-   0        0        0        0 2023-09-08 10:30:56.000000 autowork-cli-0.1.6/autowork_cli/common/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-11 06:46:46.358849 autowork-cli-0.1.6/autowork_cli/common/config/
--rw-rw-rw-   0        0        0      521 2023-10-11 01:10:55.000000 autowork-cli-0.1.6/autowork_cli/common/config/BaseURLConfig.py
--rw-rw-rw-   0        0        0      620 2023-09-13 06:06:10.000000 autowork-cli-0.1.6/autowork_cli/common/config/BusinessURLConfig.py
--rw-rw-rw-   0        0        0      237 2023-10-09 09:11:06.000000 autowork-cli-0.1.6/autowork_cli/common/config/ClientConfig.py
--rw-rw-rw-   0        0        0      236 2023-09-13 06:06:10.000000 autowork-cli-0.1.6/autowork_cli/common/config/ConfigModel.py
--rw-rw-rw-   0        0        0     3349 2023-09-13 06:06:10.000000 autowork-cli-0.1.6/autowork_cli/common/config/LoginConfig.py
--rw-rw-rw-   0        0        0      337 2023-09-28 01:49:47.000000 autowork-cli-0.1.6/autowork_cli/common/config/TemplateConfig.py
--rw-rw-rw-   0        0        0        0 2023-09-08 10:30:56.000000 autowork-cli-0.1.6/autowork_cli/common/config/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-11 06:46:46.368854 autowork-cli-0.1.6/autowork_cli/common/config/template/
--rw-rw-rw-   0        0        0        0 2023-09-19 11:28:56.000000 autowork-cli-0.1.6/autowork_cli/common/config/template/__init__.py
--rw-rw-rw-   0        0        0       89 2023-09-21 08:03:32.000000 autowork-cli-0.1.6/autowork_cli/common/config/template/hello_world_template.py
--rw-rw-rw-   0        0        0      900 2023-09-26 02:01:45.000000 autowork-cli-0.1.6/autowork_cli/common/config/template/pyproject_template.py
--rw-rw-rw-   0        0        0      196 2023-09-21 08:10:05.000000 autowork-cli-0.1.6/autowork_cli/common/config/template/sandbox_function_template.py
-drwxrwxrwx   0        0        0        0 2023-10-11 06:46:46.388848 autowork-cli-0.1.6/autowork_cli/common/lang/
--rw-rw-rw-   0        0        0        0 2023-09-08 10:30:56.000000 autowork-cli-0.1.6/autowork_cli/common/lang/__init__.py
--rw-rw-rw-   0        0        0     3353 2023-09-15 03:58:00.000000 autowork-cli-0.1.6/autowork_cli/common/lang/async_requests.py
--rw-rw-rw-   0        0        0     2722 2023-09-08 10:30:56.000000 autowork-cli-0.1.6/autowork_cli/common/lang/dictclass.py
--rw-rw-rw-   0        0        0      543 2023-09-08 10:30:56.000000 autowork-cli-0.1.6/autowork_cli/common/lang/logger_setting.py
--rw-rw-rw-   0        0        0     1474 2023-09-08 11:45:37.000000 autowork-cli-0.1.6/autowork_cli/common/lang/singleton.py
--rw-rw-rw-   0        0        0      722 2023-09-08 10:31:27.000000 autowork-cli-0.1.6/autowork_cli/common/lang/sync.py
-drwxrwxrwx   0        0        0        0 2023-10-11 06:46:46.388848 autowork-cli-0.1.6/autowork_cli/common/local/
--rw-rw-rw-   0        0        0        0 2023-09-08 10:30:56.000000 autowork-cli-0.1.6/autowork_cli/common/local/__init__.py
--rw-rw-rw-   0        0        0      763 2023-09-14 12:24:06.000000 autowork-cli-0.1.6/autowork_cli/common/local/clientinfo.py
-drwxrwxrwx   0        0        0        0 2023-10-11 06:46:46.398854 autowork-cli-0.1.6/autowork_cli/common/log/
--rw-rw-rw-   0        0        0     2430 2023-10-10 08:39:03.000000 autowork-cli-0.1.6/autowork_cli/common/log/AwLogger.py
--rw-rw-rw-   0        0        0      439 2023-09-14 07:25:30.000000 autowork-cli-0.1.6/autowork_cli/common/log/LogManager.py
--rw-rw-rw-   0        0        0        0 2023-09-13 06:06:10.000000 autowork-cli-0.1.6/autowork_cli/common/log/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-11 06:46:46.403391 autowork-cli-0.1.6/autowork_cli/common/request/
--rw-rw-rw-   0        0        0     1513 2023-10-11 06:15:34.000000 autowork-cli-0.1.6/autowork_cli/common/request/CybotronAsyncClient.py
--rw-rw-rw-   0        0        0      760 2023-09-08 11:45:37.000000 autowork-cli-0.1.6/autowork_cli/common/request/CybotronSyncClient.py
--rw-rw-rw-   0        0        0        0 2023-09-08 10:30:56.000000 autowork-cli-0.1.6/autowork_cli/common/request/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-11 06:46:46.408910 autowork-cli-0.1.6/autowork_cli/file/
--rw-rw-rw-   0        0        0     4987 2023-09-14 07:29:32.000000 autowork-cli-0.1.6/autowork_cli/file/CosFileManager.py
--rw-rw-rw-   0        0        0        0 2023-09-13 06:06:10.000000 autowork-cli-0.1.6/autowork_cli/file/__init__.py
--rw-rw-rw-   0        0        0     3252 2023-09-28 01:45:23.000000 autowork-cli-0.1.6/autowork_cli/file/file_cmd.py
-drwxrwxrwx   0        0        0        0 2023-10-11 06:46:46.408910 autowork-cli-0.1.6/autowork_cli/flow/
--rw-rw-rw-   0        0        0        0 2023-09-13 06:06:11.000000 autowork-cli-0.1.6/autowork_cli/flow/__init__.py
--rw-rw-rw-   0        0        0     1843 2023-10-11 06:44:35.000000 autowork-cli-0.1.6/autowork_cli/flow/flow_cmd.py
-drwxrwxrwx   0        0        0        0 2023-10-11 06:46:46.418920 autowork-cli-0.1.6/autowork_cli/log/
--rw-rw-rw-   0        0        0        0 2023-09-13 06:06:11.000000 autowork-cli-0.1.6/autowork_cli/log/__init__.py
--rw-rw-rw-   0        0        0      773 2023-09-13 08:55:01.000000 autowork-cli-0.1.6/autowork_cli/log/log_cmd.py
-drwxrwxrwx   0        0        0        0 2023-10-11 06:46:46.418920 autowork-cli-0.1.6/autowork_cli/login/
--rw-rw-rw-   0        0        0        0 2023-09-08 10:30:56.000000 autowork-cli-0.1.6/autowork_cli/login/__init__.py
--rw-rw-rw-   0        0        0     2356 2023-09-13 06:06:11.000000 autowork-cli-0.1.6/autowork_cli/login/login_cmd.py
-drwxrwxrwx   0        0        0        0 2023-10-11 06:46:46.418920 autowork-cli-0.1.6/autowork_cli/repository/
--rw-rw-rw-   0        0        0        0 2023-09-13 06:06:11.000000 autowork-cli-0.1.6/autowork_cli/repository/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-11 06:46:46.428920 autowork-cli-0.1.6/autowork_cli/repository/cybotron/
--rw-rw-rw-   0        0        0        0 2023-09-13 06:06:11.000000 autowork-cli-0.1.6/autowork_cli/repository/cybotron/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-11 06:46:46.428920 autowork-cli-0.1.6/autowork_cli/repository/cybotron/model/
--rw-rw-rw-   0        0        0        0 2023-09-13 06:06:11.000000 autowork-cli-0.1.6/autowork_cli/repository/cybotron/model/__init__.py
--rw-rw-rw-   0        0        0      143 2023-09-13 06:06:11.000000 autowork-cli-0.1.6/autowork_cli/repository/cybotron/model/flowobj.py
--rw-rw-rw-   0        0        0     2715 2023-09-13 06:06:11.000000 autowork-cli-0.1.6/autowork_cli/repository/cybotron/model/metadataobj.py
-drwxrwxrwx   0        0        0        0 2023-10-11 06:46:46.438918 autowork-cli-0.1.6/autowork_cli/repository/cybotron/service/
--rw-rw-rw-   0        0        0        0 2023-09-13 06:06:11.000000 autowork-cli-0.1.6/autowork_cli/repository/cybotron/service/__init__.py
--rw-rw-rw-   0        0        0     3710 2023-09-13 06:06:11.000000 autowork-cli-0.1.6/autowork_cli/repository/cybotron/service/common_access.py
--rw-rw-rw-   0        0        0     1299 2023-09-13 06:06:11.000000 autowork-cli-0.1.6/autowork_cli/repository/cybotron/service/data_accessor.py
--rw-rw-rw-   0        0        0     1377 2023-09-13 06:06:11.000000 autowork-cli-0.1.6/autowork_cli/repository/cybotron/service/log_accessor.py
--rw-rw-rw-   0        0        0     1319 2023-09-13 06:06:11.000000 autowork-cli-0.1.6/autowork_cli/repository/cybotron/service/metadata_accessor.py
-drwxrwxrwx   0        0        0        0 2023-10-11 06:46:46.448923 autowork-cli-0.1.6/autowork_cli/sidecar/
--rw-rw-rw-   0        0        0        0 2023-09-08 10:30:56.000000 autowork-cli-0.1.6/autowork_cli/sidecar/__init__.py
--rw-rw-rw-   0        0        0     2912 2023-10-10 03:05:43.000000 autowork-cli-0.1.6/autowork_cli/sidecar/dev_register.py
-drwxrwxrwx   0        0        0        0 2023-10-11 06:46:46.458920 autowork-cli-0.1.6/autowork_cli/sidecar/dto/
--rw-rw-rw-   0        0        0      126 2023-09-08 10:30:56.000000 autowork-cli-0.1.6/autowork_cli/sidecar/dto/SandboxFuncRequest.py
--rw-rw-rw-   0        0        0        0 2023-09-08 10:30:56.000000 autowork-cli-0.1.6/autowork_cli/sidecar/dto/__init__.py
--rw-rw-rw-   0        0        0     2230 2023-10-10 08:57:47.000000 autowork-cli-0.1.6/autowork_cli/sidecar/sidecar_app.py
--rw-rw-rw-   0        0        0     1293 2023-09-21 07:05:48.000000 autowork-cli-0.1.6/autowork_cli/sidecar/sidecar_cmd.py
--rw-rw-rw-   0        0        0     1229 2023-09-21 07:06:06.000000 autowork-cli-0.1.6/autowork_cli/sidecar/sidecar_mgr.py
-drwxrwxrwx   0        0        0        0 2023-10-11 06:46:46.468926 autowork-cli-0.1.6/autowork_cli/util/
--rw-rw-rw-   0        0        0        0 2023-09-11 02:04:37.000000 autowork-cli-0.1.6/autowork_cli/util/__init__.py
--rw-rw-rw-   0        0        0      276 2023-09-13 06:06:11.000000 autowork-cli-0.1.6/autowork_cli/util/apikeyutil.py
--rw-rw-rw-   0        0        0    10043 2023-09-13 06:06:11.000000 autowork-cli-0.1.6/autowork_cli/util/dateutil.py
--rw-rw-rw-   0        0        0      176 2023-09-21 06:39:50.000000 autowork-cli-0.1.6/autowork_cli/util/fileutil.py
--rw-rw-rw-   0        0        0      164 2023-09-13 06:06:11.000000 autowork-cli-0.1.6/autowork_cli/util/jsonobjutil.py
-drwxrwxrwx   0        0        0        0 2023-10-11 06:46:46.338846 autowork-cli-0.1.6/autowork_cli.egg-info/
--rw-rw-rw-   0        0        0      118 2023-10-11 06:46:46.000000 autowork-cli-0.1.6/autowork_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2664 2023-10-11 06:46:46.000000 autowork-cli-0.1.6/autowork_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-11 06:46:46.000000 autowork-cli-0.1.6/autowork_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-10-11 06:46:46.000000 autowork-cli-0.1.6/autowork_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       13 2023-10-11 06:46:46.000000 autowork-cli-0.1.6/autowork_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1008 2023-10-11 06:46:28.000000 autowork-cli-0.1.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-10-11 06:46:46.478920 autowork-cli-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      306 2023-10-11 06:46:24.000000 autowork-cli-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-29 10:42:36.454075 autowork-cli-0.2.0/
+-rw-rw-rw-   0        0        0      118 2024-03-29 10:42:36.453103 autowork-cli-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      954 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-03-29 10:42:35.929783 autowork-cli-0.2.0/autowork_cli/
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/__init__.py
+-rw-rw-rw-   0        0        0     1239 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/__main__.py
+drwxrwxrwx   0        0        0        0 2024-03-29 10:42:35.979783 autowork-cli-0.2.0/autowork_cli/cf/
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/cf/__init__.py
+-rw-rw-rw-   0        0        0     4739 2024-03-13 05:46:37.000000 autowork-cli-0.2.0/autowork_cli/cf/cf_cmd.py
+-rw-rw-rw-   0        0        0     8444 2024-03-13 05:46:37.000000 autowork-cli-0.2.0/autowork_cli/cf/sync_cf_data.py
+drwxrwxrwx   0        0        0        0 2024-03-29 10:42:35.980790 autowork-cli-0.2.0/autowork_cli/common/
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/common/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-29 10:42:36.044073 autowork-cli-0.2.0/autowork_cli/common/config/
+-rw-rw-rw-   0        0        0      727 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/common/config/BaseURLConfig.py
+-rw-rw-rw-   0        0        0      620 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/common/config/BusinessURLConfig.py
+-rw-rw-rw-   0        0        0      237 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/common/config/ClientConfig.py
+-rw-rw-rw-   0        0        0      236 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/common/config/ConfigModel.py
+-rw-rw-rw-   0        0        0     3540 2024-03-21 03:11:28.000000 autowork-cli-0.2.0/autowork_cli/common/config/LoginConfig.py
+-rw-rw-rw-   0        0        0      337 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/common/config/TemplateConfig.py
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/common/config/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-29 10:42:36.086072 autowork-cli-0.2.0/autowork_cli/common/config/template/
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/common/config/template/__init__.py
+-rw-rw-rw-   0        0        0       89 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/common/config/template/hello_world_template.py
+-rw-rw-rw-   0        0        0      881 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/common/config/template/pyproject_template.py
+-rw-rw-rw-   0        0        0      202 2024-03-13 05:46:37.000000 autowork-cli-0.2.0/autowork_cli/common/config/template/repo_mapping_template.py
+-rw-rw-rw-   0        0        0      214 2024-03-13 05:46:37.000000 autowork-cli-0.2.0/autowork_cli/common/config/template/sandbox_function_template.py
+drwxrwxrwx   0        0        0        0 2024-03-29 10:42:36.118074 autowork-cli-0.2.0/autowork_cli/common/lang/
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/common/lang/__init__.py
+-rw-rw-rw-   0        0        0     3353 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/common/lang/async_requests.py
+-rw-rw-rw-   0        0        0     2722 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/common/lang/dictclass.py
+-rw-rw-rw-   0        0        0      543 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/common/lang/logger_setting.py
+-rw-rw-rw-   0        0        0     1474 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/common/lang/singleton.py
+-rw-rw-rw-   0        0        0      722 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/common/lang/sync.py
+drwxrwxrwx   0        0        0        0 2024-03-29 10:42:36.125074 autowork-cli-0.2.0/autowork_cli/common/local/
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/common/local/__init__.py
+-rw-rw-rw-   0        0        0      763 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/common/local/clientinfo.py
+drwxrwxrwx   0        0        0        0 2024-03-29 10:42:36.140073 autowork-cli-0.2.0/autowork_cli/common/log/
+-rw-rw-rw-   0        0        0     2539 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/common/log/AwLogger.py
+-rw-rw-rw-   0        0        0      439 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/common/log/LogManager.py
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/common/log/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-29 10:42:36.181075 autowork-cli-0.2.0/autowork_cli/common/request/
+-rw-rw-rw-   0        0        0     1677 2024-03-19 08:56:08.000000 autowork-cli-0.2.0/autowork_cli/common/request/CybotronAsyncClient.py
+-rw-rw-rw-   0        0        0      760 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/common/request/CybotronSyncClient.py
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/common/request/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-29 10:42:36.201074 autowork-cli-0.2.0/autowork_cli/file/
+-rw-rw-rw-   0        0        0     4987 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/file/CosFileManager.py
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/file/__init__.py
+-rw-rw-rw-   0        0        0     3252 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/file/file_cmd.py
+drwxrwxrwx   0        0        0        0 2024-03-29 10:42:36.220072 autowork-cli-0.2.0/autowork_cli/flow/
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/flow/__init__.py
+-rw-rw-rw-   0        0        0     1843 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/flow/flow_cmd.py
+drwxrwxrwx   0        0        0        0 2024-03-29 10:42:36.232072 autowork-cli-0.2.0/autowork_cli/log/
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/log/__init__.py
+-rw-rw-rw-   0        0        0      773 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/log/log_cmd.py
+drwxrwxrwx   0        0        0        0 2024-03-29 10:42:36.251074 autowork-cli-0.2.0/autowork_cli/login/
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/login/__init__.py
+-rw-rw-rw-   0        0        0     3607 2024-03-21 03:10:55.000000 autowork-cli-0.2.0/autowork_cli/login/login_cmd.py
+drwxrwxrwx   0        0        0        0 2024-03-29 10:42:36.252075 autowork-cli-0.2.0/autowork_cli/repository/
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/repository/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-29 10:42:36.252075 autowork-cli-0.2.0/autowork_cli/repository/cybotron/
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/repository/cybotron/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-29 10:42:36.283105 autowork-cli-0.2.0/autowork_cli/repository/cybotron/model/
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/repository/cybotron/model/__init__.py
+-rw-rw-rw-   0        0        0      143 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/repository/cybotron/model/flowobj.py
+-rw-rw-rw-   0        0        0     2716 2024-03-13 05:46:37.000000 autowork-cli-0.2.0/autowork_cli/repository/cybotron/model/metadataobj.py
+drwxrwxrwx   0        0        0        0 2024-03-29 10:42:36.345104 autowork-cli-0.2.0/autowork_cli/repository/cybotron/service/
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/repository/cybotron/service/__init__.py
+-rw-rw-rw-   0        0        0     3713 2024-03-13 05:46:37.000000 autowork-cli-0.2.0/autowork_cli/repository/cybotron/service/common_access.py
+-rw-rw-rw-   0        0        0     1299 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/repository/cybotron/service/data_accessor.py
+-rw-rw-rw-   0        0        0     1377 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/repository/cybotron/service/log_accessor.py
+-rw-rw-rw-   0        0        0     1319 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/repository/cybotron/service/metadata_accessor.py
+drwxrwxrwx   0        0        0        0 2024-03-29 10:42:36.355084 autowork-cli-0.2.0/autowork_cli/sidecar/
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/sidecar/__init__.py
+-rw-rw-rw-   0        0        0     2999 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/sidecar/dev_register.py
+drwxrwxrwx   0        0        0        0 2024-03-29 10:42:36.362075 autowork-cli-0.2.0/autowork_cli/sidecar/dto/
+-rw-rw-rw-   0        0        0      126 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/sidecar/dto/SandboxFuncRequest.py
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/sidecar/dto/__init__.py
+-rw-rw-rw-   0        0        0     2209 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/sidecar/sidecar_app.py
+-rw-rw-rw-   0        0        0     1461 2024-03-13 05:46:37.000000 autowork-cli-0.2.0/autowork_cli/sidecar/sidecar_cmd.py
+-rw-rw-rw-   0        0        0     1229 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/sidecar/sidecar_mgr.py
+drwxrwxrwx   0        0        0        0 2024-03-29 10:42:36.396104 autowork-cli-0.2.0/autowork_cli/util/
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/util/__init__.py
+-rw-rw-rw-   0        0        0      276 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/util/apikeyutil.py
+-rw-rw-rw-   0        0        0    10043 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/util/dateutil.py
+-rw-rw-rw-   0        0        0      176 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/util/fileutil.py
+-rw-rw-rw-   0        0        0      164 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/autowork_cli/util/jsonobjutil.py
+drwxrwxrwx   0        0        0        0 2024-03-29 10:42:35.947781 autowork-cli-0.2.0/autowork_cli.egg-info/
+-rw-rw-rw-   0        0        0      118 2024-03-29 10:42:35.000000 autowork-cli-0.2.0/autowork_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3196 2024-03-29 10:42:35.000000 autowork-cli-0.2.0/autowork_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-29 10:42:35.000000 autowork-cli-0.2.0/autowork_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-03-29 10:42:35.000000 autowork-cli-0.2.0/autowork_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-03-29 10:42:35.000000 autowork-cli-0.2.0/autowork_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1026 2024-03-21 03:27:52.000000 autowork-cli-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-03-29 10:42:36.454075 autowork-cli-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      306 2024-03-21 03:27:52.000000 autowork-cli-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-29 10:42:36.397073 autowork-cli-0.2.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-29 10:42:36.405074 autowork-cli-0.2.0/tests/cf/
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/tests/cf/__init__.py
+-rw-rw-rw-   0        0        0     1250 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/tests/cf/test_cf_cmd.py
+drwxrwxrwx   0        0        0        0 2024-03-29 10:42:36.406076 autowork-cli-0.2.0/tests/common/
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/tests/common/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-29 10:42:36.414105 autowork-cli-0.2.0/tests/common/config/
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/tests/common/config/__init__.py
+-rw-rw-rw-   0        0        0     1139 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/tests/common/config/test_login_config.py
+drwxrwxrwx   0        0        0        0 2024-03-29 10:42:36.421075 autowork-cli-0.2.0/tests/log/
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/tests/log/__init__.py
+-rw-rw-rw-   0        0        0      208 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/tests/log/test_log_cmd.py
+drwxrwxrwx   0        0        0        0 2024-03-29 10:42:36.441073 autowork-cli-0.2.0/tests/login/
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/tests/login/__init__.py
+-rw-rw-rw-   0        0        0      355 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/tests/login/test_hello.py
+-rw-rw-rw-   0        0        0     1174 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/tests/login/test_login_cmd.py
+drwxrwxrwx   0        0        0        0 2024-03-29 10:42:36.444074 autowork-cli-0.2.0/tests/sidecar/
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/tests/sidecar/__init__.py
+-rw-rw-rw-   0        0        0      495 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/tests/sidecar/test_dev_register.py
+-rw-rw-rw-   0        0        0      386 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/tests/sidecar/test_sidecar_mgr.py
+drwxrwxrwx   0        0        0        0 2024-03-29 10:42:36.452074 autowork-cli-0.2.0/tests/util/
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/tests/util/__init__.py
+-rw-rw-rw-   0        0        0      525 2023-12-26 03:22:40.000000 autowork-cli-0.2.0/tests/util/test_api_key_util.py
```

### Comparing `autowork-cli-0.1.6/README.md` & `autowork-cli-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `autowork-cli-0.1.6/autowork_cli/__main__.py` & `autowork-cli-0.2.0/autowork_cli/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 @app.command(help="显示Autowork版本号")
 def version():
     typer.echo("Autowork 1.0.0")
 
 
 @app.callback()
 def main():
-    print("[blue]🅰🆄🆃🅾🆆🅾🆁🅺")
+    pass
 
 
 def run():
     app()
 
 
 if __name__ == "__main__":
```

### Comparing `autowork-cli-0.1.6/autowork_cli/common/config/BaseURLConfig.py` & `autowork-cli-0.2.0/autowork_cli/common/config/BaseURLConfig.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 URL_DICT = {
+    "LOCAL": "http://127.0.0.1:8080",
     "DEV": "http://cybotron-dev.yunzhangfang.com",
     "ALPHA": "http://cybotron-alpha.yunzhangfang.com",
     "BETA": "http://cybotron-beta.yunzhangfang.com",
+    "TEST": "http://cybotron-test.yunzhangfang.com",
     "PROD": "http://cybotron.yunzhangfang.com",
 }
 
 
 class BaseURLConfig:
     @staticmethod
-    def get_api_base_url(env):
-        return URL_DICT[env] + "/cybotron-client"
+    def get_api_base_url(env: str):
+        env = env.upper()
+        if env == 'LOCAL':
+            return URL_DICT[env]
+        else:
+            return URL_DICT[env] + "/cybotron-client"
 
     @staticmethod
     def get_domain_url(env):
         return URL_DICT[env]
 
     @staticmethod
     def get_env_list():
```

### Comparing `autowork-cli-0.1.6/autowork_cli/common/config/BusinessURLConfig.py` & `autowork-cli-0.2.0/autowork_cli/common/config/BusinessURLConfig.py`

 * *Files identical despite different names*

### Comparing `autowork-cli-0.1.6/autowork_cli/common/config/LoginConfig.py` & `autowork-cli-0.2.0/autowork_cli/common/config/LoginConfig.py`

 * *Files 14% similar despite different names*

```diff
@@ -98,15 +98,21 @@
 
     def get_api_key(self):
         env = self.get_env()
         if env not in self.data:
             self.data[env] = DictClass()
         return self.data[env].get('API_KEY')
 
+    def set_tenant_id(self, tenant_id):
+        self.get_global_config().TENANT_ID = tenant_id
+
+    def get_tenant_id(self):
+        return self.get_global_config().get("TENANT_ID")
+
     def __str__(self):
         return str(self.data)
 
     def __repr__(self):
         return self.__str__()
 
 
-DefaultLoginConfig = LoginConfig()
+DefaultLoginConfig = LoginConfig()
```

### Comparing `autowork-cli-0.1.6/autowork_cli/common/config/template/pyproject_template.py` & `autowork-cli-0.2.0/autowork_cli/common/config/template/pyproject_template.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,21 +4,14 @@
 version = "0.1.0"
 description = ""
 authors = ["user <user@yunzhangfang.com>"]
 packages = [{ include = "{project_id}" }]
 
 [tool.poetry.dependencies]
 python = "^3.11"
-httpx = "^0.24.1"
-fastapi = "^0.103.1"
-uvicorn = "^0.23.2"
-requests = "^2.28.1"
-psutil = "^5.9.4"
-tencentcloud-sdk-python = "^3.0.979"
-pytest = "^7.4.2"
 sandbox-func = "^0.1.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 pytest-asyncio = "^0.21.1"
 
 [build-system]
@@ -29,10 +22,15 @@
 log_cli = true
 log_cli_level = "INFO"
 log_cli_format = "%(asctime)s [%(levelname)5s] %(name)s:%(filename)s:%(lineno)s - %(message)s"
 log_cli_date_format = "%Y-%m-%d %H:%M:%S"
 
 [[tool.poetry.source]]
 name = "custom"
-url = "https://pypi.org/simple"
+url = "https://pypi.tuna.tsinghua.edu.cn/simple"
 default = true
+
+[package.source]
+type = "legacy"
+url = "http://172.23.50.109:18083/repository/pypi-group/simple"
+reference = "custom"
 """
```

### Comparing `autowork-cli-0.1.6/autowork_cli/common/lang/async_requests.py` & `autowork-cli-0.2.0/autowork_cli/common/lang/async_requests.py`

 * *Files identical despite different names*

### Comparing `autowork-cli-0.1.6/autowork_cli/common/lang/dictclass.py` & `autowork-cli-0.2.0/autowork_cli/common/lang/dictclass.py`

 * *Files identical despite different names*

### Comparing `autowork-cli-0.1.6/autowork_cli/common/lang/logger_setting.py` & `autowork-cli-0.2.0/autowork_cli/common/lang/logger_setting.py`

 * *Files identical despite different names*

### Comparing `autowork-cli-0.1.6/autowork_cli/common/lang/singleton.py` & `autowork-cli-0.2.0/autowork_cli/common/lang/singleton.py`

 * *Files identical despite different names*

### Comparing `autowork-cli-0.1.6/autowork_cli/common/lang/sync.py` & `autowork-cli-0.2.0/autowork_cli/common/lang/sync.py`

 * *Files identical despite different names*

### Comparing `autowork-cli-0.1.6/autowork_cli/common/local/clientinfo.py` & `autowork-cli-0.2.0/autowork_cli/common/local/clientinfo.py`

 * *Files identical despite different names*

### Comparing `autowork-cli-0.1.6/autowork_cli/common/log/AwLogger.py` & `autowork-cli-0.2.0/autowork_cli/common/log/AwLogger.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,18 +22,22 @@
     app_version_id: str
     func_id: str
     creator: str
     level: str
     message: str
 
 
+class LogRecord(UserDict):
+    trace_id: str
+
+
 class AwLogger:
     """autowork log warapper"""
 
-    cybotron_access_info: Log
+    cybotron_access_info: dict = {}
 
     @classmethod
     def getLogger(cls, filename: str, level: LogLevel = LogLevel.INFO):
         logger = logging.getLogger(filename)
         if level is None:
             logger.setLevel('INFO')
         else:
@@ -61,21 +65,24 @@
 
 
 class DBLogHandler(logging.Handler):
     def __init__(self):
         super().__init__()
 
     def emit(self, record: logging.LogRecord):
+        msg = record.getMessage()
+        trace_id = record.args.get("trace_id")
+        # trace_id = msg.split('-')[0]
+        # real_msg = msg.split('-')[1]
+        cybotron_access_info = AwLogger.cybotron_access_info[trace_id]
         log = Log(
-            trace_id=AwLogger.cybotron_access_info['trace_id'],
-            app_id=AwLogger.cybotron_access_info['app_id'],
-            app_version_id=AwLogger.cybotron_access_info['app_version_id'],
-            func_id=AwLogger.cybotron_access_info['func_id'],
-            creator=AwLogger.cybotron_access_info['creator'],
+            trace_id=cybotron_access_info['trace_id'],
+            app_id=cybotron_access_info['app_id'],
+            func_id=cybotron_access_info['func_id'],
             level=record.levelno,
-            message=record.getMessage()
+            message=msg
         )
 
         try:
             LogAccessor.send_log(log.data)
         except Exception as e:
             print(e)
```

### Comparing `autowork-cli-0.1.6/autowork_cli/common/request/CybotronAsyncClient.py` & `autowork-cli-0.2.0/autowork_cli/common/request/CybotronAsyncClient.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,19 +12,20 @@
     async def get(self, url, json=None):
         return await self.send(url, method="get", _json=json)
 
     async def send(self, url, method, _json=None):
         login_config = LoginConfig()
         env = login_config.get_env()
         api_key = login_config.get_api_key()
+        tenant_id = login_config.get_tenant_id()
         base_url = BaseURLConfig.get_api_base_url(env)
 
         client = AsyncRequests(base_url=base_url)
         data = json.dumps(_json)
-        request = client.build_request(method=method, url=url, data=data, headers=CybotronAsyncClient.__get_headers(api_key))
+        request = client.build_request(method=method, url=url, data=data, headers=CybotronAsyncClient.__get_headers(api_key, tenant_id))
 
         response = await client.send(request)
         response_json = response.json()
 
         if self.throw_exception and response_json.get("errorMessage"):
             raise Exception(response_json.get("errorMessage"))
 
@@ -32,13 +33,15 @@
 
     def post(self, url, json=None):
         if json is None:
             json = {}
         return self.send(url, method="post", _json=json)
 
     @staticmethod
-    def __get_headers(api_key):
+    def __get_headers(api_key, tenant_id):
         headers = {
             'Content-Type': 'application/json',
-            'X-API-KEY': api_key
+            'X-API-KEY': api_key,
         }
+        if tenant_id is not None:
+            headers.update({'X-TENANT-ID': tenant_id})
         return headers
```

### Comparing `autowork-cli-0.1.6/autowork_cli/common/request/CybotronSyncClient.py` & `autowork-cli-0.2.0/autowork_cli/common/request/CybotronSyncClient.py`

 * *Files identical despite different names*

### Comparing `autowork-cli-0.1.6/autowork_cli/file/CosFileManager.py` & `autowork-cli-0.2.0/autowork_cli/file/CosFileManager.py`

 * *Files identical despite different names*

### Comparing `autowork-cli-0.1.6/autowork_cli/file/file_cmd.py` & `autowork-cli-0.2.0/autowork_cli/file/file_cmd.py`

 * *Files identical despite different names*

### Comparing `autowork-cli-0.1.6/autowork_cli/flow/flow_cmd.py` & `autowork-cli-0.2.0/autowork_cli/flow/flow_cmd.py`

 * *Files identical despite different names*

### Comparing `autowork-cli-0.1.6/autowork_cli/log/log_cmd.py` & `autowork-cli-0.2.0/autowork_cli/log/log_cmd.py`

 * *Files identical despite different names*

### Comparing `autowork-cli-0.1.6/autowork_cli/login/login_cmd.py` & `autowork-cli-0.2.0/autowork_cli/login/login_cmd.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import sys
+
 import inquirer
 
 from autowork_cli.common.request.CybotronSyncClient import CybotronSyncClient
 from autowork_cli.common.config.BaseURLConfig import BaseURLConfig
 from autowork_cli.common.config.LoginConfig import LoginConfig
 from rich import print
 
@@ -14,14 +16,15 @@
 
     def run_login(self):
         # 初始化函数
         print("登录 Autowork...")
 
         self.ask_env()
         self.ask_api_key()
+        self.ask_tenant()
         self.ask_dev_apps()
 
         self.hello()
 
     def ask_env(self):
         # tuple (label, value) list
         choices_list = [(a + ": " + BaseURLConfig.get_domain_url(a), a) for a in BaseURLConfig.get_env_list()]
@@ -44,14 +47,35 @@
                           default=safe_apikey),
         ])
 
         if safe_apikey != answer["api_key"]:
             self.config.set_api_key(answer["api_key"])
             self.config.save()
 
+    def ask_tenant(self):
+        client = CybotronSyncClient()
+        try:
+            tenants_info = client.get("cbn/api/v1/tenant/user/tenants").get("result")
+            tenant_code_list = [(f'{tenant["code"]}({tenant["name"]})', tenant['id']) for tenant in tenants_info]
+            tenant_code_dict = dict(tenant_code_list)
+            if len(tenants_info) == 1:
+                tenant_code = tenant_code_list[0][0]
+                answer = inquirer.prompt([
+                    inquirer.Text('tenant', message=f"现在登录的是{tenant_code}租户", default=tenant_code)])
+            else:
+                tenant_code_list = [tenant[0] for tenant in tenant_code_list]
+                answer = inquirer.prompt([
+                    inquirer.List("tenant", message="选择要登录的租户?", choices=tenant_code_list, default=tenant_code_list[0])])
+            self.config.set_tenant_id(tenant_code_dict[answer["tenant"]])
+            self.config.save()
+        except Exception as e:
+            print(e)
+            print(f"[red]登录失败：无法连接到 {self.config.get_env()} 环境，请检查网络或联系管理员")
+            sys.exit(1)  # 退出登录流程
+
     def ask_dev_apps(self):
         answer = inquirer.prompt([
             inquirer.Text('dev_apps',
                           message="请输入您正要开发的应用编码，多个应用用逗号分隔",
                           default=self.config.get_dev_apps()),
         ])
         self.config.set_dev_apps(answer["dev_apps"])
```

### Comparing `autowork-cli-0.1.6/autowork_cli/repository/cybotron/model/metadataobj.py` & `autowork-cli-0.2.0/autowork_cli/repository/cybotron/model/metadataobj.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     options: GetMetaOptions = GetMetaOptions()  # 查询配置
 
 
 class GetListRequest(BaseRequest):
     query: str = None  # 查询条件
     filter: Union[dict, None] = {}
     sort: str = None
-    select: Union[str, None] = []
+    select: Union[list, None] = []
     pageSize: int = 10
     pageNum: int = 1
     options: GetOptions = GetOptions()  # 查询配置
 
 
 class GetMetaListRequest(GetListRequest):
     metadataAppId: str = ""  # 应用id
```

### Comparing `autowork-cli-0.1.6/autowork_cli/repository/cybotron/service/common_access.py` & `autowork-cli-0.2.0/autowork_cli/repository/cybotron/service/common_access.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,29 +46,29 @@
     async def delete(self, req: DeleteRequest) -> DeleteResponse:
         """
         单条删除接口
         """
         result = await self.get_response(req, "delete")
         return DeleteResponse(count=result["count"])
 
-    async def bulkCreate(self, req: BulkCreateRequest) -> BulkCreateResponse:
+    async def bulk_create(self, req: BulkCreateRequest) -> BulkCreateResponse:
         """
         批量创建接口
         """
         result = await self.get_response(req, "bulkCreate")
         return BulkCreateResponse(count=result["count"])
 
-    async def bulkUpdate(self, req: BulkUpdateRequest) -> BulkUpdateResponse:
+    async def bulk_update(self, req: BulkUpdateRequest) -> BulkUpdateResponse:
         """
         批量修改接口
         """
         result = await self.get_response(req, "bulkUpdate")
         return BulkUpdateResponse(count=result["count"])
 
-    async def bulkDelete(self, req: BulkDeleteRequest) -> BulkDeleteResponse:
+    async def bulk_delete(self, req: BulkDeleteRequest) -> BulkDeleteResponse:
         """
         批量删除接口
         """
         result = await self.get_response(req=req, method="bulkDelete")
         return BulkDeleteResponse(count=result["count"])
 
     async def get_response(self, req, method: str = "", re_method: str = "post") -> Dict:
```

### Comparing `autowork-cli-0.1.6/autowork_cli/repository/cybotron/service/data_accessor.py` & `autowork-cli-0.2.0/autowork_cli/repository/cybotron/service/data_accessor.py`

 * *Files identical despite different names*

### Comparing `autowork-cli-0.1.6/autowork_cli/repository/cybotron/service/log_accessor.py` & `autowork-cli-0.2.0/autowork_cli/repository/cybotron/service/log_accessor.py`

 * *Files identical despite different names*

### Comparing `autowork-cli-0.1.6/autowork_cli/repository/cybotron/service/metadata_accessor.py` & `autowork-cli-0.2.0/autowork_cli/repository/cybotron/service/metadata_accessor.py`

 * *Files identical despite different names*

### Comparing `autowork-cli-0.1.6/autowork_cli/sidecar/dev_register.py` & `autowork-cli-0.2.0/autowork_cli/sidecar/dev_register.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 
     @classmethod
     async def stop(cls):
         cls.interval_stop = True
         client = CybotronAsyncClient()
         response = await client.post(cls.unregister_url, json={})
         if response["success"] is True:
+            logger.info("关闭开发者路由成功")
             return True
         return False
 
     @classmethod
     async def query(cls):
         client = CybotronAsyncClient()
         response = await client.get(cls.query_url)
@@ -70,14 +71,15 @@
     @classmethod
     def register(cls):
         ip_address = ClientInfo.get_ip()
         config = DefaultLoginConfig
         dev_apps_config = config.get_dev_apps()
         if not dev_apps_config:
             logger.error("开发者路由注册失败：【未配置开发应用】")
-        data = {"devApps": dev_apps_config.split(","), "serviceId": "SandboxFunction", "address": ip_address}
+        data = {"devApps": dev_apps_config.split(","), "serviceId": "SandboxFunction", "address": ip_address,
+                "port": 8081}
 
         client = CybotronSyncClient()
         response = client.post(cls.dev_register_url, json=data)
         if response["success"] is True:
             return data
         return False
```

### Comparing `autowork-cli-0.1.6/autowork_cli/sidecar/sidecar_app.py` & `autowork-cli-0.2.0/autowork_cli/sidecar/sidecar_app.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-from autowork_cli.common.log.AwLogger import AwLogger, Log
+from autowork_cli.common.log.AwLogger import AwLogger, Log, LogRecord
 from fastapi import Request
 from fastapi import FastAPI
 from fastapi.middleware.cors import CORSMiddleware
 
 from autowork_cli.common.lang import logger_setting
 from autowork_cli.common.lang.async_requests import AsyncRequests
 from autowork_cli.sidecar.dev_register import DevRouterRegister
@@ -40,29 +40,28 @@
     return {
         "pid": os.getpid()
     }
 
 
 @app.post("/sandbox/call/{app_id}/{func_id}")
 async def call_sandbox_func(app_id: str, func_id: str, req: Request, debug: bool = False):
+    global trace_id
     try:
         app_port = sidecar_mgr.app_port
         client = AsyncRequests(f"http://localhost:{str(app_port)}")
         data = await req.json()
 
-        debug_info = data['debug']
+        trace_id = data['traceId']
         cybotron_access_info = Log(
-            trace_id=debug_info['traceId'],
-            app_id=debug_info['appId'],
-            app_version_id=debug_info['appVersionId'],
+            trace_id=trace_id,
+            app_id=app_id,
             func_id=func_id,
-            creator=debug_info['creator']
         )
-        AwLogger.cybotron_access_info = cybotron_access_info
-        logger.info(f'本地边车服务转发赛博坦平台请求，应用编号：{app_id}, 函数编号：{func_id}, 参数：{data}')
+        AwLogger.cybotron_access_info[trace_id] = cybotron_access_info
+        logger.info(f'本地边车服务转发赛博坦平台请求，应用编号：{app_id}, 函数编号：{func_id}, 参数：{data}', LogRecord(trace_id=trace_id))
 
-        timeout = 30*60 if debug else 10
+        timeout = 30 * 60 if debug else 10
         resp = await client.request(f"/sandbox/call/{app_id}/{func_id}/local", data, timeout)
         return resp.json()
     except BaseException as e:
-        logger.info(f'本地边车服务转发赛博坦平台请求报错，应用编号：{app_id}, 函数编号：{func_id}, 参数：{data}, 报错信息：{e}')
+        logger.info(f'本地边车服务转发赛博坦平台请求报错，应用编号：{app_id}, 函数编号：{func_id}, 参数：{data}, 报错信息：{e}', LogRecord(trace_id=trace_id))
         return {"message": str(e), "success": False}
```

### Comparing `autowork-cli-0.1.6/autowork_cli/sidecar/sidecar_cmd.py` & `autowork-cli-0.2.0/autowork_cli/sidecar/sidecar_cmd.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 from time import sleep
 from typing import Annotated
 
 import rich
 import typer
 
 from autowork_cli.sidecar.sidecar_mgr import SidecarManager
+from autowork_cli.cf.cf_cmd import publish
 
 sc_app = typer.Typer(name='sidecar', help='Autowork边车服务')
 
 sidecar_mgr = SidecarManager()
 
 
 @sc_app.command(help="启动边车服务")
-def start(port: Annotated[int, typer.Option(help="边车端口号")] = 9080,
+def start(port: Annotated[int, typer.Option(help="边车端口号")] = 8081,
           app_port: Annotated[int, typer.Option(help="应用端口号")] = 9000):
+    # 执行数据同步，未找到文件时跳过
+    res = publish(raise_error=False)
+    if not res:
+        return
     if port == app_port:
         rich.print("[red]边车端口号和应用端口号不能相同")
         return
     rich.print(f"[blue]启动边车服务，监听本地端口号{app_port}")
     sidecar_mgr.port = port
     sidecar_mgr.app_port = app_port
     sidecar_mgr.start()
```

### Comparing `autowork-cli-0.1.6/autowork_cli/sidecar/sidecar_mgr.py` & `autowork-cli-0.2.0/autowork_cli/sidecar/sidecar_mgr.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from autowork_cli.common.lang import logger_setting
 from autowork_cli.common.lang.singleton import SingletonMeta
 
 logger = logging.getLogger(__name__)
 
 
 class SidecarManager(metaclass=SingletonMeta):
-    def __init__(self, port: int = 9080):
+    def __init__(self, port: int = 8081):
         self.port = port
         self.app_port = 9000
 
     def start(self):
         logger.info("redirecting to app port: " + str(self.app_port))
         uvicorn.run("autowork_cli.sidecar.sidecar_app:app", host="0.0.0.0", port=self.port, log_level="info")
```

### Comparing `autowork-cli-0.1.6/autowork_cli/util/dateutil.py` & `autowork-cli-0.2.0/autowork_cli/util/dateutil.py`

 * *Files identical despite different names*

### Comparing `autowork-cli-0.1.6/autowork_cli.egg-info/SOURCES.txt` & `autowork-cli-0.2.0/autowork_cli.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -6,25 +6,27 @@
 autowork_cli.egg-info/PKG-INFO
 autowork_cli.egg-info/SOURCES.txt
 autowork_cli.egg-info/dependency_links.txt
 autowork_cli.egg-info/entry_points.txt
 autowork_cli.egg-info/top_level.txt
 autowork_cli/cf/__init__.py
 autowork_cli/cf/cf_cmd.py
+autowork_cli/cf/sync_cf_data.py
 autowork_cli/common/__init__.py
 autowork_cli/common/config/BaseURLConfig.py
 autowork_cli/common/config/BusinessURLConfig.py
 autowork_cli/common/config/ClientConfig.py
 autowork_cli/common/config/ConfigModel.py
 autowork_cli/common/config/LoginConfig.py
 autowork_cli/common/config/TemplateConfig.py
 autowork_cli/common/config/__init__.py
 autowork_cli/common/config/template/__init__.py
 autowork_cli/common/config/template/hello_world_template.py
 autowork_cli/common/config/template/pyproject_template.py
+autowork_cli/common/config/template/repo_mapping_template.py
 autowork_cli/common/config/template/sandbox_function_template.py
 autowork_cli/common/lang/__init__.py
 autowork_cli/common/lang/async_requests.py
 autowork_cli/common/lang/dictclass.py
 autowork_cli/common/lang/logger_setting.py
 autowork_cli/common/lang/singleton.py
 autowork_cli/common/lang/sync.py
@@ -62,8 +64,24 @@
 autowork_cli/sidecar/sidecar_mgr.py
 autowork_cli/sidecar/dto/SandboxFuncRequest.py
 autowork_cli/sidecar/dto/__init__.py
 autowork_cli/util/__init__.py
 autowork_cli/util/apikeyutil.py
 autowork_cli/util/dateutil.py
 autowork_cli/util/fileutil.py
-autowork_cli/util/jsonobjutil.py
+autowork_cli/util/jsonobjutil.py
+tests/__init__.py
+tests/cf/__init__.py
+tests/cf/test_cf_cmd.py
+tests/common/__init__.py
+tests/common/config/__init__.py
+tests/common/config/test_login_config.py
+tests/log/__init__.py
+tests/log/test_log_cmd.py
+tests/login/__init__.py
+tests/login/test_hello.py
+tests/login/test_login_cmd.py
+tests/sidecar/__init__.py
+tests/sidecar/test_dev_register.py
+tests/sidecar/test_sidecar_mgr.py
+tests/util/__init__.py
+tests/util/test_api_key_util.py
```

### Comparing `autowork-cli-0.1.6/pyproject.toml` & `autowork-cli-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autowork-cli"
-version = "0.1.6"
+version = "0.2.0"
 description = ""
 authors = ["Your Name <you@example.com>"]
 readme = "README.md"
 packages = [{include = "autowork_cli"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
@@ -13,14 +13,15 @@
 configparser2 = "^4.0.0"
 httpx = "^0.24.1"
 fastapi = "^0.103.1"
 uvicorn = "^0.23.2"
 requests = "^2.28.1"
 psutil = "^5.9.4"
 coloredlogs = "^15.0.1"
+twine = "^4.0.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 pytest-asyncio = "^0.21.1"
 
 [build-system]
 requires = ["poetry-core"]
```

