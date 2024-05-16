# Comparing `tmp/autowork-cli-0.1.6.tar.gz` & `tmp/autowork-cli-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autowork-cli-0.1.6.tar", last modified: Wed Oct 11 06:46:46 2023, max compression
+gzip compressed data, was "autowork-cli-0.4.5.tar", last modified: Thu May 16 09:21:13 2024, max compression
```

## Comparing `autowork-cli-0.1.6.tar` & `autowork-cli-0.4.5.tar`

### file list

```diff
@@ -1,93 +1,125 @@
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
+drwxrwxrwx   0        0        0        0 2024-05-16 09:21:13.856110 autowork-cli-0.4.5/
+-rw-rw-rw-   0        0        0     1091 2024-05-16 07:19:51.000000 autowork-cli-0.4.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      149 2024-05-16 09:21:13.854101 autowork-cli-0.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0      954 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 09:21:13.104113 autowork-cli-0.4.5/autowork_cli/
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/autowork_cli/__init__.py
+-rw-rw-rw-   0        0        0     1243 2024-05-09 09:36:39.000000 autowork-cli-0.4.5/autowork_cli/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:21:13.149253 autowork-cli-0.4.5/autowork_cli/cf/
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/autowork_cli/cf/__init__.py
+-rw-rw-rw-   0        0        0     1603 2024-05-11 06:37:16.000000 autowork-cli-0.4.5/autowork_cli/cf/cf_cmd.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:21:13.151227 autowork-cli-0.4.5/autowork_cli/common/
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/autowork_cli/common/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:21:13.233481 autowork-cli-0.4.5/autowork_cli/common/config/
+-rw-rw-rw-   0        0        0     1500 2024-05-15 05:53:36.000000 autowork-cli-0.4.5/autowork_cli/common/config/BaseURLConfig.py
+-rw-rw-rw-   0        0        0      620 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/autowork_cli/common/config/BusinessURLConfig.py
+-rw-rw-rw-   0        0        0      237 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/autowork_cli/common/config/ClientConfig.py
+-rw-rw-rw-   0        0        0      236 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/autowork_cli/common/config/ConfigModel.py
+-rw-rw-rw-   0        0        0     4883 2024-05-13 05:42:04.000000 autowork-cli-0.4.5/autowork_cli/common/config/LoginConfig.py
+-rw-rw-rw-   0        0        0      370 2024-05-13 03:52:17.000000 autowork-cli-0.4.5/autowork_cli/common/config/PublicConfig.py
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/autowork_cli/common/config/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:21:13.294283 autowork-cli-0.4.5/autowork_cli/common/config/template/
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/autowork_cli/common/config/template/__init__.py
+-rw-rw-rw-   0        0        0      172 2024-05-08 11:45:39.000000 autowork-cli-0.4.5/autowork_cli/common/config/template/hello_world_template.py
+-rw-rw-rw-   0        0        0      904 2024-05-08 08:56:35.000000 autowork-cli-0.4.5/autowork_cli/common/config/template/pyproject_template.py
+-rw-rw-rw-   0        0        0     1083 2024-05-11 06:37:16.000000 autowork-cli-0.4.5/autowork_cli/common/config/template/sandbox_readme_template.py
+-rw-rw-rw-   0        0        0      152 2024-05-08 11:45:39.000000 autowork-cli-0.4.5/autowork_cli/common/config/template/sandbox_start_template.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:21:13.353555 autowork-cli-0.4.5/autowork_cli/common/lang/
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/autowork_cli/common/lang/__init__.py
+-rw-rw-rw-   0        0        0     3353 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/autowork_cli/common/lang/async_requests.py
+-rw-rw-rw-   0        0        0     2722 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/autowork_cli/common/lang/dictclass.py
+-rw-rw-rw-   0        0        0      543 2024-05-07 11:38:48.000000 autowork-cli-0.4.5/autowork_cli/common/lang/logger_setting.py
+-rw-rw-rw-   0        0        0     1474 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/autowork_cli/common/lang/singleton.py
+-rw-rw-rw-   0        0        0      722 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/autowork_cli/common/lang/sync.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:21:13.362547 autowork-cli-0.4.5/autowork_cli/common/local/
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/autowork_cli/common/local/__init__.py
+-rw-rw-rw-   0        0        0      763 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/autowork_cli/common/local/clientinfo.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:21:13.379548 autowork-cli-0.4.5/autowork_cli/common/log/
+-rw-rw-rw-   0        0        0     2539 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/autowork_cli/common/log/AwLogger.py
+-rw-rw-rw-   0        0        0      439 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/autowork_cli/common/log/LogManager.py
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/autowork_cli/common/log/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:21:13.451227 autowork-cli-0.4.5/autowork_cli/common/request/
+-rw-rw-rw-   0        0        0     1827 2024-04-25 09:03:02.000000 autowork-cli-0.4.5/autowork_cli/common/request/CybotronAsyncClient.py
+-rw-rw-rw-   0        0        0      760 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/autowork_cli/common/request/CybotronSyncClient.py
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/autowork_cli/common/request/__init__.py
+-rw-rw-rw-   0        0        0     2324 2024-05-13 05:38:23.000000 autowork-cli-0.4.5/autowork_cli/common/request/forward_request.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:21:13.476239 autowork-cli-0.4.5/autowork_cli/file/
+-rw-rw-rw-   0        0        0     5239 2024-05-08 08:56:35.000000 autowork-cli-0.4.5/autowork_cli/file/CosFileManager.py
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/autowork_cli/file/__init__.py
+-rw-rw-rw-   0        0        0     3394 2024-05-08 08:56:35.000000 autowork-cli-0.4.5/autowork_cli/file/file_cmd.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:21:13.491388 autowork-cli-0.4.5/autowork_cli/flow/
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/autowork_cli/flow/__init__.py
+-rw-rw-rw-   0        0        0     1889 2024-04-25 09:03:02.000000 autowork-cli-0.4.5/autowork_cli/flow/flow_cmd.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:21:13.503389 autowork-cli-0.4.5/autowork_cli/log/
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/autowork_cli/log/__init__.py
+-rw-rw-rw-   0        0        0      773 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/autowork_cli/log/log_cmd.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:21:13.526421 autowork-cli-0.4.5/autowork_cli/login/
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/autowork_cli/login/__init__.py
+-rw-rw-rw-   0        0        0     7467 2024-05-13 03:50:30.000000 autowork-cli-0.4.5/autowork_cli/login/login_cmd.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:21:13.528406 autowork-cli-0.4.5/autowork_cli/repository/
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/autowork_cli/repository/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:21:13.529418 autowork-cli-0.4.5/autowork_cli/repository/cybotron/
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/autowork_cli/repository/cybotron/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:21:13.551418 autowork-cli-0.4.5/autowork_cli/repository/cybotron/model/
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/autowork_cli/repository/cybotron/model/__init__.py
+-rw-rw-rw-   0        0        0      143 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/autowork_cli/repository/cybotron/model/flowobj.py
+-rw-rw-rw-   0        0        0     2805 2024-04-25 09:03:02.000000 autowork-cli-0.4.5/autowork_cli/repository/cybotron/model/metadataobj.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:21:13.618100 autowork-cli-0.4.5/autowork_cli/repository/cybotron/service/
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/autowork_cli/repository/cybotron/service/__init__.py
+-rw-rw-rw-   0        0        0     3713 2024-03-13 05:46:37.000000 autowork-cli-0.4.5/autowork_cli/repository/cybotron/service/common_access.py
+-rw-rw-rw-   0        0        0     1305 2024-04-25 09:03:02.000000 autowork-cli-0.4.5/autowork_cli/repository/cybotron/service/data_accessor.py
+-rw-rw-rw-   0        0        0     1386 2024-04-25 09:03:02.000000 autowork-cli-0.4.5/autowork_cli/repository/cybotron/service/log_accessor.py
+-rw-rw-rw-   0        0        0     1325 2024-04-25 09:03:02.000000 autowork-cli-0.4.5/autowork_cli/repository/cybotron/service/metadata_accessor.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:21:13.698103 autowork-cli-0.4.5/autowork_cli/sidecar/
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/autowork_cli/sidecar/__init__.py
+-rw-rw-rw-   0        0        0     3843 2024-05-07 12:15:31.000000 autowork-cli-0.4.5/autowork_cli/sidecar/dev_register.py
+-rw-rw-rw-   0        0        0      378 2024-05-08 11:45:39.000000 autowork-cli-0.4.5/autowork_cli/sidecar/dev_websocket.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:21:13.706151 autowork-cli-0.4.5/autowork_cli/sidecar/dto/
+-rw-rw-rw-   0        0        0      126 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/autowork_cli/sidecar/dto/SandboxFuncRequest.py
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/autowork_cli/sidecar/dto/__init__.py
+-rw-rw-rw-   0        0        0     3552 2024-05-08 11:45:39.000000 autowork-cli-0.4.5/autowork_cli/sidecar/sidecar_app.py
+-rw-rw-rw-   0        0        0     1293 2024-05-08 08:56:35.000000 autowork-cli-0.4.5/autowork_cli/sidecar/sidecar_cmd.py
+-rw-rw-rw-   0        0        0     1229 2024-05-07 12:16:07.000000 autowork-cli-0.4.5/autowork_cli/sidecar/sidecar_mgr.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:21:13.744130 autowork-cli-0.4.5/autowork_cli/util/
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/autowork_cli/util/__init__.py
+-rw-rw-rw-   0        0        0      276 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/autowork_cli/util/apikeyutil.py
+-rw-rw-rw-   0        0        0    10043 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/autowork_cli/util/dateutil.py
+-rw-rw-rw-   0        0        0      182 2024-05-11 06:37:16.000000 autowork-cli-0.4.5/autowork_cli/util/fileutil.py
+-rw-rw-rw-   0        0        0      164 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/autowork_cli/util/jsonobjutil.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:21:13.776130 autowork-cli-0.4.5/autowork_cli/web_socket/
+-rw-rw-rw-   0        0        0       25 2024-05-08 11:45:39.000000 autowork-cli-0.4.5/autowork_cli/web_socket/__init__.py
+-rw-rw-rw-   0        0        0     1174 2024-05-14 05:34:49.000000 autowork-cli-0.4.5/autowork_cli/web_socket/model.py
+-rw-rw-rw-   0        0        0     4937 2024-05-14 05:34:49.000000 autowork-cli-0.4.5/autowork_cli/web_socket/web_socket.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:21:13.129084 autowork-cli-0.4.5/autowork_cli.egg-info/
+-rw-rw-rw-   0        0        0      149 2024-05-16 09:21:12.000000 autowork-cli-0.4.5/autowork_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3365 2024-05-16 09:21:12.000000 autowork-cli-0.4.5/autowork_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 09:21:12.000000 autowork-cli-0.4.5/autowork_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-05-16 09:21:12.000000 autowork-cli-0.4.5/autowork_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-05-16 09:21:12.000000 autowork-cli-0.4.5/autowork_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1077 2024-05-13 05:43:53.000000 autowork-cli-0.4.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-16 09:21:13.857116 autowork-cli-0.4.5/setup.cfg
+-rw-rw-rw-   0        0        0      310 2024-05-13 05:43:53.000000 autowork-cli-0.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:21:13.778100 autowork-cli-0.4.5/tests/
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:21:13.787101 autowork-cli-0.4.5/tests/cf/
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/tests/cf/__init__.py
+-rw-rw-rw-   0        0        0     1250 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/tests/cf/test_cf_cmd.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:21:13.789101 autowork-cli-0.4.5/tests/common/
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/tests/common/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:21:13.798101 autowork-cli-0.4.5/tests/common/config/
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/tests/common/config/__init__.py
+-rw-rw-rw-   0        0        0     1139 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/tests/common/config/test_login_config.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:21:13.807101 autowork-cli-0.4.5/tests/log/
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/tests/log/__init__.py
+-rw-rw-rw-   0        0        0      208 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/tests/log/test_log_cmd.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:21:13.829100 autowork-cli-0.4.5/tests/login/
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/tests/login/__init__.py
+-rw-rw-rw-   0        0        0      355 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/tests/login/test_hello.py
+-rw-rw-rw-   0        0        0     1174 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/tests/login/test_login_cmd.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:21:13.845100 autowork-cli-0.4.5/tests/sidecar/
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/tests/sidecar/__init__.py
+-rw-rw-rw-   0        0        0      495 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/tests/sidecar/test_dev_register.py
+-rw-rw-rw-   0        0        0      386 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/tests/sidecar/test_sidecar_mgr.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:21:13.853101 autowork-cli-0.4.5/tests/util/
+-rw-rw-rw-   0        0        0        0 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/tests/util/__init__.py
+-rw-rw-rw-   0        0        0      525 2023-12-26 03:22:40.000000 autowork-cli-0.4.5/tests/util/test_api_key_util.py
```

### Comparing `autowork-cli-0.1.6/README.md` & `autowork-cli-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `autowork-cli-0.1.6/autowork_cli/__main__.py` & `autowork-cli-0.4.5/autowork_cli/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import typer
 from rich import print
 
 from autowork_cli.cf.cf_cmd import cf_app
 from autowork_cli.log.log_cmd import log_app
 from autowork_cli.login.login_cmd import LoginCommand
 from autowork_cli.sidecar.sidecar_cmd import sc_app
-from autowork_cli.file.file_cmd import file_app
+# from autowork_cli.file.file_cmd import file_app
 from autowork_cli.flow.flow_cmd import flow_app
 
 # 备份字体：🅰🅱🅲🅳🅴🅵🅶🅷🅸🅹🅺🅻🅼🅽🅾🅿🆀🆁🆂🆃🆄🆅🆆🆇🆈🆉
 # 备份字体：🅐🅑🅒🅓🅔🅕🅖🅗🅘🅙🅚🅛🅜🅝🅞🅟🅠🅡🅢🅣🅤🅥🅦🅧🅨🅩
 
 app = typer.Typer(name='autowork', help='Autowork Command-line Tool')
 app.add_typer(cf_app, name="cf")
 app.add_typer(sc_app, name="sidecar")
-app.add_typer(file_app, name="file")
+# app.add_typer(file_app, name="file")
 app.add_typer(flow_app, name='flow')
 app.add_typer(log_app, name='log')
 # app.add_typer(sc_app, name="sc", help="边车服务sidecar缩写命令")
 
 
 @app.command(help="登录Autowork系统")
 def login():
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

### Comparing `autowork-cli-0.1.6/autowork_cli/cf/cf_cmd.py` & `autowork-cli-0.4.5/autowork_cli/cf/cf_cmd.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,46 @@
 # -*- coding: utf-8 -*-
-
-import shutil
-import urllib.request
-
-import requests
 import typer
 import os
 
-from autowork_cli.common.config.TemplateConfig import SANDBOX_BOOT_URL
 from autowork_cli.common.config.template.hello_world_template import HELLO_WORD
 from autowork_cli.common.config.template.pyproject_template import PYPROJECT_TEMPLATE
-from autowork_cli.common.config.template.sandbox_function_template import SANDBOX_FUNCTION
+from autowork_cli.common.config.template.sandbox_readme_template import SANDBOX_README_TEMPLATE
+from autowork_cli.common.config.template.sandbox_start_template import SANDBOX_START
 from autowork_cli.util.fileutil import FileUtil
 
+
 cf_app = typer.Typer(name='cf', help='Autowork Cloud Function Tool')
 
 
 @cf_app.command(help='初始沙盒函数工程')
-def init(project_id: str = typer.Option(None, '-p', '--project-id', prompt='工程ID', help='工程ID'),
-         app_id: str = typer.Option(None, '-a', '--app-id', prompt='所属应用ID', help='所属应用ID')):
+def init(project_id: str = typer.Option(None, '-p', '--project-id', prompt='工程ID', help='工程ID')):
     # 初始化函数
     src_dir = project_id.strip().lower()
     if not os.path.exists(src_dir):
         os.mkdir(src_dir)
     if not os.path.exists('tests'):
         os.mkdir('tests')
 
     # init pyproject.toml
     content = PYPROJECT_TEMPLATE.replace('{project_id}', src_dir, 2)
-    FileUtil.genFile('./pyproject.toml', content)
+    FileUtil.generate_file('./pyproject.toml', content)
 
-    # init sandbox_function.json
-    content = SANDBOX_FUNCTION.replace('{app_id}', app_id, 1).replace('{project_id}', src_dir, 1)
-    FileUtil.genFile('./sandbox_function.json', content)
+    # init SANDBOX_README.md
+    FileUtil.generate_file('./SANDBOX_README.md', SANDBOX_README_TEMPLATE)
 
     # init hello world
-    FileUtil.genFile(f"./{src_dir}/hello_world.py", HELLO_WORD)
+    FileUtil.generate_file(f"./{src_dir}/hello_world.py", HELLO_WORD)
+    FileUtil.generate_file(f"./{src_dir}/__init__.py", '')
+
+    # add tests init
+    FileUtil.generate_file(f"./tests/__init__.py", '')
 
-    # add sandbox-boot
-    urllib.request.urlretrieve(SANDBOX_BOOT_URL, 'sandbox_boot.zip')
-    shutil.unpack_archive('sandbox_boot.zip', './', format='zip')
-    os.remove('sandbox_boot.zip')
+    # init sandbox_start
+    FileUtil.generate_file(f"./sandbox_start.py", SANDBOX_START)
 
     typer.echo("project inited")
 
 
 @cf_app.command()
 def run():
     # 初始化函数
```

### Comparing `autowork-cli-0.1.6/autowork_cli/common/config/BusinessURLConfig.py` & `autowork-cli-0.4.5/autowork_cli/common/config/BusinessURLConfig.py`

 * *Files identical despite different names*

### Comparing `autowork-cli-0.1.6/autowork_cli/common/config/template/pyproject_template.py` & `autowork-cli-0.4.5/autowork_cli/common/config/template/pyproject_template.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,23 +3,16 @@
 name = "{project_id}"
 version = "0.1.0"
 description = ""
 authors = ["user <user@yunzhangfang.com>"]
 packages = [{ include = "{project_id}" }]
 
 [tool.poetry.dependencies]
-python = "^3.11"
-httpx = "^0.24.1"
-fastapi = "^0.103.1"
-uvicorn = "^0.23.2"
-requests = "^2.28.1"
-psutil = "^5.9.4"
-tencentcloud-sdk-python = "^3.0.979"
-pytest = "^7.4.2"
-sandbox-func = "^0.1.0"
+python = "^3.11,<3.12"
+sandbox-func = {version = "^0.4.1", source = "private"}
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 pytest-asyncio = "^0.21.1"
 
 [build-system]
 requires = ["poetry-core"]
@@ -29,10 +22,14 @@
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
+[[tool.poetry.source]]
+name = "private"
+url = "http://172.23.50.109:18083/repository/pypi-group/simple"
 """
```

### Comparing `autowork-cli-0.1.6/autowork_cli/common/lang/async_requests.py` & `autowork-cli-0.4.5/autowork_cli/common/lang/async_requests.py`

 * *Files identical despite different names*

### Comparing `autowork-cli-0.1.6/autowork_cli/common/lang/dictclass.py` & `autowork-cli-0.4.5/autowork_cli/common/lang/dictclass.py`

 * *Files identical despite different names*

### Comparing `autowork-cli-0.1.6/autowork_cli/common/lang/logger_setting.py` & `autowork-cli-0.4.5/autowork_cli/common/lang/logger_setting.py`

 * *Files identical despite different names*

### Comparing `autowork-cli-0.1.6/autowork_cli/common/lang/singleton.py` & `autowork-cli-0.4.5/autowork_cli/common/lang/singleton.py`

 * *Files identical despite different names*

### Comparing `autowork-cli-0.1.6/autowork_cli/common/lang/sync.py` & `autowork-cli-0.4.5/autowork_cli/common/lang/sync.py`

 * *Files identical despite different names*

### Comparing `autowork-cli-0.1.6/autowork_cli/common/local/clientinfo.py` & `autowork-cli-0.4.5/autowork_cli/common/local/clientinfo.py`

 * *Files identical despite different names*

### Comparing `autowork-cli-0.1.6/autowork_cli/common/log/AwLogger.py` & `autowork-cli-0.4.5/autowork_cli/common/log/AwLogger.py`

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

### Comparing `autowork-cli-0.1.6/autowork_cli/common/request/CybotronSyncClient.py` & `autowork-cli-0.4.5/autowork_cli/common/request/CybotronSyncClient.py`

 * *Files identical despite different names*

### Comparing `autowork-cli-0.1.6/autowork_cli/file/CosFileManager.py` & `autowork-cli-0.4.5/autowork_cli/file/CosFileManager.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,131 +1,130 @@
-# -*- coding:utf-8 -*-
-from enum import Enum
-
-import requests
-
-from autowork_cli.common.config.LoginConfig import DefaultLoginConfig
-from autowork_cli.common.config.BaseURLConfig import BaseURLConfig
-from autowork_cli.common.config.ClientConfig import USER_AGENT
-from autowork_cli.common.lang.async_requests import AsyncRequests
-from autowork_cli.repository.cybotron.service.data_accessor import DataAccessor
-from autowork_cli.repository.cybotron.model.metadataobj import GetOptions
-from autowork_cli.repository.cybotron.model.metadataobj import GetListRequest
-
-
-class BucketExpireTime(Enum):
-    E_FOREVER = "tc_forever"
-    E_30_DAYS = "tc_30days"
-    E_3_MONTH = "tc_3months"
-    E_1_YEAR = "tc_1year"
-
-    @staticmethod
-    def get_expire_time(expire_type: int):
-        match expire_type:
-            case 1:
-                return BucketExpireTime.E_FOREVER
-            case 2:
-                return BucketExpireTime.E_30_DAYS
-            case 3:
-                return BucketExpireTime.E_3_MONTH
-            case _:
-                return BucketExpireTime.E_1_YEAR
-
-
-class CosFileManager:
-    """
-    文件存储腾讯云接口类
-    """
-
-    def __init__(self):
-        self.remote_data_accessor = DataAccessor()
-        self.client = AsyncRequests(BaseURLConfig.get_api_base_url(DefaultLoginConfig.get_env()))
-
-    @classmethod
-    def __save_file_with_response(cls, local_file_path, response):
-        """
-        根据网络响应，保存文件
-        :param local_file_path: 本地保存的文件路径
-        :param response: 云端响应
-        :return:
-        """
-        with open(local_file_path, 'wb') as f:
-            for chunk in response.iter_content(chunk_size=512):
-                if chunk:
-                    f.write(chunk)
-                    f.flush()
-
-    async def __get_bucket(self, expire_time: BucketExpireTime) -> str:
-        """
-        查询元数据表，获取到指定时间的桶id
-        :param expire_time: 有效时间
-        :return: 数据库中的桶id
-        """
-        options = GetOptions()
-        req = GetListRequest(
-            appCode="metabase",
-            tableCode="mb_file_bucket",
-            options=options,
-            filter={"code": expire_time.value}
-        )
-        res_list = await self.remote_data_accessor.getList(req)
-        if res_list.total > 0:
-            return res_list.data[0].get('id')
-        else:
-            raise Exception(
-                f'腾讯云存储，上传或下载时，没有从数据库中获取到存储桶id，metabase mb_file_bucket {expire_time}')
-
-    async def __send_request(self, url: str, file_path: str, bucket_id: str):
-        """
-        给元数据后台发送请求
-        :param url: 接口url
-        :param file_path: 腾讯云文件路径
-        :param bucket_id: 桶id
-        :return: 接口返回的result
-        """
-        req = self.client.build_request(
-            method="post", url=url, timeout=15,
-            json={
-                "bucketId": bucket_id,
-                "filePath": file_path,
-                "expiration": None
-            },
-            headers={
-                'User-Agent': USER_AGENT,
-                'X-API-KEY': DefaultLoginConfig.get_api_key()
-            }
-        )
-        response = await self.client.send(req)
-        response = response.json()
-        if not response.get("success"):
-            raise Exception(response.get("message"))
-        return response["result"]
-
-    async def upload_file(self, local_file_path, cloud_file_path, expire_time=BucketExpireTime.E_FOREVER) -> str:
-        """
-        上传文件
-        :param local_file_path: 本地要上传的文件路径
-        :param cloud_file_path: 云端存储文件路径
-        :param expire_time: 有效时间
-        :return: 成功/失败
-        """
-        # 读取文件内容
-        bucket_id = await self.__get_bucket(expire_time)
-        with open(local_file_path, 'rb') as f:
-            url = await self.__send_request('/cbn/api/v1/file/upload/generatePreSignedUrl', cloud_file_path, bucket_id)
-            response = requests.put(url=url, data=f.read())
-            if response.status_code != 200:
-                raise Exception(response.text)
-            return str(url).split('?')[0]
-
-    async def download_file(self, local_file_path, cloud_file_path, expire_time=BucketExpireTime.E_FOREVER):
-        """
-        下载文件
-        :param local_file_path: 本地要下载的路径
-        :param cloud_file_path: 云端文件路径
-        :param expire_time: 有效时间
-        :return:
-        """
-        bucket_id = await self.__get_bucket(expire_time)
-        url = await self.__send_request('/cbn/api/v1/file/download/generatePreSignedUrl', cloud_file_path, bucket_id)
-        response = requests.get(url=url)
-        self.__save_file_with_response(local_file_path, response)
+# # -*- coding:utf-8 -*-
+# import requests
+# from enum import Enum
+#
+# from autowork_cli.common.config.LoginConfig import DefaultLoginConfig
+# from autowork_cli.common.config.BaseURLConfig import DefaultURLConfig
+# from autowork_cli.common.config.ClientConfig import USER_AGENT
+# from autowork_cli.common.lang.async_requests import AsyncRequests
+# from autowork_cli.repository.cybotron.service.data_accessor import DataAccessor
+# from autowork_cli.repository.cybotron.model.metadataobj import GetOptions
+# from autowork_cli.repository.cybotron.model.metadataobj import GetListRequest
+#
+#
+# class BucketExpireTime(Enum):
+#     E_FOREVER = "tc_forever"
+#     E_30_DAYS = "tc_30days"
+#     E_3_MONTH = "tc_3months"
+#     E_1_YEAR = "tc_1year"
+#
+#     @staticmethod
+#     def get_expire_time(expire_type: int):
+#         match expire_type:
+#             case 1:
+#                 return BucketExpireTime.E_FOREVER
+#             case 2:
+#                 return BucketExpireTime.E_30_DAYS
+#             case 3:
+#                 return BucketExpireTime.E_3_MONTH
+#             case _:
+#                 return BucketExpireTime.E_1_YEAR
+#
+#
+# class CosFileManager:
+#     """
+#     文件存储腾讯云接口类
+#     """
+#
+#     def __init__(self):
+#         self.remote_data_accessor = DataAccessor()
+#         self.client = AsyncRequests(DefaultURLConfig.get_api_base_url(DefaultLoginConfig.get_env()))
+#
+#     @classmethod
+#     def __save_file_with_response(cls, local_file_path, response):
+#         """
+#         根据网络响应，保存文件
+#         :param local_file_path: 本地保存的文件路径
+#         :param response: 云端响应
+#         :return:
+#         """
+#         with open(local_file_path, 'wb') as f:
+#             for chunk in response.iter_content(chunk_size=512):
+#                 if chunk:
+#                     f.write(chunk)
+#                     f.flush()
+#
+#     async def __get_bucket(self, expire_time: BucketExpireTime) -> str:
+#         """
+#         查询元数据表，获取到指定时间的桶id
+#         :param expire_time: 有效时间
+#         :return: 数据库中的桶id
+#         """
+#         options = GetOptions()
+#         req = GetListRequest(
+#             appCode="metabase",
+#             tableCode="mb_file_bucket",
+#             options=options,
+#             filter={"code": expire_time.value}
+#         )
+#         res_list = await self.remote_data_accessor.getList(req)
+#         if res_list.total > 0:
+#             return res_list.data[0].get('id')
+#         else:
+#             raise Exception(
+#                 f'腾讯云存储，上传或下载时，没有从数据库中获取到存储桶id，metabase mb_file_bucket {expire_time}')
+#
+#     async def __send_request(self, url: str, file_path: str, bucket_id: str):
+#         """
+#         给元数据后台发送请求
+#         :param url: 接口url
+#         :param file_path: 腾讯云文件路径
+#         :param bucket_id: 桶id
+#         :return: 接口返回的result
+#         """
+#         req = self.client.build_request(
+#             method="post", url=url, timeout=15,
+#             json={
+#                 "bucketId": bucket_id,
+#                 "filePath": file_path,
+#                 "expiration": None
+#             },
+#             headers={
+#                 'User-Agent': USER_AGENT,
+#                 'X-API-KEY': DefaultLoginConfig.get_api_key()
+#             }
+#         )
+#         response = await self.client.send(req)
+#         response = response.json()
+#         if not response.get("success"):
+#             raise Exception(response.get("message"))
+#         return response["result"]
+#
+#     async def upload_file(self, local_file_path, cloud_file_path, expire_time=BucketExpireTime.E_FOREVER) -> str:
+#         """
+#         上传文件
+#         :param local_file_path: 本地要上传的文件路径
+#         :param cloud_file_path: 云端存储文件路径
+#         :param expire_time: 有效时间
+#         :return: 成功/失败
+#         """
+#         # 读取文件内容
+#         bucket_id = await self.__get_bucket(expire_time)
+#         with open(local_file_path, 'rb') as f:
+#             url = await self.__send_request('/cbn/api/v1/file/upload/generatePreSignedUrl', cloud_file_path, bucket_id)
+#             response = requests.put(url=url, data=f.read())
+#             if response.status_code != 200:
+#                 raise Exception(response.text)
+#             return str(url).split('?')[0]
+#
+#     async def download_file(self, local_file_path, cloud_file_path, expire_time=BucketExpireTime.E_FOREVER):
+#         """
+#         下载文件
+#         :param local_file_path: 本地要下载的路径
+#         :param cloud_file_path: 云端文件路径
+#         :param expire_time: 有效时间
+#         :return:
+#         """
+#         bucket_id = await self.__get_bucket(expire_time)
+#         url = await self.__send_request('/cbn/api/v1/file/download/generatePreSignedUrl', cloud_file_path, bucket_id)
+#         response = requests.get(url=url)
+#         self.__save_file_with_response(local_file_path, response)
```

### Comparing `autowork-cli-0.1.6/autowork_cli/file/file_cmd.py` & `autowork-cli-0.4.5/autowork_cli/file/file_cmd.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-import asyncio
-import os
-import uuid
-import warnings
-from pathlib import Path
-
-import typer
-from typing_extensions import Annotated
-
-from autowork_cli.file.CosFileManager import CosFileManager, BucketExpireTime
-from autowork_cli.util.dateutil import DateUtil
-
-file_app = typer.Typer(name='file', help='Autowork File Tool')
-warnings.filterwarnings("ignore")
-
-
-@file_app.command(help='上传文件')
-def upload(file: Annotated[str, typer.Argument(help='上传的文件')],
-           target: str = typer.Option(None, '-t', '--target-file', help='目标文件,默认autowork/YYYYmmdd/uuid'),
-           expire_type: int = typer.Option(1, '-e', '--expire-type', help='过期类型')):
-    if file is None:
-        typer.secho('请指定要上传的文件', fg=typer.colors.RED)
-
-    if file.startswith("./"):
-        upload_file = Path(__file__).resolve().parent.joinpath(file)
-        if not upload_file.exists():
-            typer.secho('指定的文件不存在', fg=typer.colors.RED)
-            return
-    else:
-        upload_file = Path(file)
-        if not Path(file).exists():
-            typer.secho('指定的文件不存在', fg=typer.colors.RED)
-            return
-
-    if target is None:
-        upload_file_name = str(uuid.uuid4()).replace('-', '') + '.' + upload_file.name.split('.')[-1]
-        cloud_file_path = f"autowork/{DateUtil().now().strftime('%Y%m%d')}/{upload_file_name}"
-    else:
-        cloud_file_path = target if target.startswith('autowork') else f'autowork/${target}'
-
-    try:
-        res = asyncio.run(CosFileManager().upload_file(upload_file,
-                                                       cloud_file_path,
-                                                       BucketExpireTime.get_expire_time(expire_type)))
-        if res:
-            typer.secho(f"文件上传成功, 上传地址：{res}", fg=typer.colors.GREEN)
-    except Exception as e:
-        typer.secho(f"上传文件报错：{e}", fg=typer.colors.RED)
-
-
-@file_app.command(help="下载文件")
-def download(file: Annotated[str, typer.Argument(help='待下载的文件, ')],
-             outdir: str = typer.Option(None, '-d', '--out-dir', help='下载保存目录'),
-             expire_type: int = typer.Option(1, '-e', '--expire-type', help='过期类型')):
-    global download_dir
-    if file.startswith('http'):
-        file = '/'.join(file.split('/')[3:])
-
-    if outdir is not None:
-        if outdir.startswith('./'):
-            download_dir = Path(os.getcwd()).parent.joinpath(outdir)
-        else:
-            download_dir = Path(outdir)
-    else:
-        download_dir = Path(os.getcwd())
-
-    if not download_dir.exists():
-        download_dir.mkdir(parents=True, exist_ok=True)
-
-    download_file = download_dir.joinpath(Path(file).name)
-
-    try:
-        asyncio.run(CosFileManager().download_file(download_file,
-                                                   file,
-                                                   BucketExpireTime.get_expire_time(expire_type)))
-        typer.secho(f"下载文件成功，地址：{download_file}", fg=typer.colors.RED)
-    except Exception as e:
-        typer.secho(f"下载文件报错：{e}", fg=typer.colors.RED)
+# import asyncio
+# import os
+# import uuid
+# import warnings
+# from pathlib import Path
+#
+# import typer
+# from typing_extensions import Annotated
+#
+# from autowork_cli.file.CosFileManager import CosFileManager, BucketExpireTime
+# from autowork_cli.util.dateutil import DateUtil
+#
+# file_app = typer.Typer(name='file', help='Autowork File Tool')
+# warnings.filterwarnings("ignore")
+#
+#
+# @file_app.command(help='上传文件')
+# def upload(file: Annotated[str, typer.Argument(help='上传的文件')],
+#            target: str = typer.Option(None, '-t', '--target-file', help='目标文件,默认autowork/YYYYmmdd/uuid'),
+#            expire_type: int = typer.Option(1, '-e', '--expire-type', help='过期类型')):
+#     if file is None:
+#         typer.secho('请指定要上传的文件', fg=typer.colors.RED)
+#
+#     if file.startswith("./"):
+#         upload_file = Path(__file__).resolve().parent.joinpath(file)
+#         if not upload_file.exists():
+#             typer.secho('指定的文件不存在', fg=typer.colors.RED)
+#             return
+#     else:
+#         upload_file = Path(file)
+#         if not Path(file).exists():
+#             typer.secho('指定的文件不存在', fg=typer.colors.RED)
+#             return
+#
+#     if target is None:
+#         upload_file_name = str(uuid.uuid4()).replace('-', '') + '.' + upload_file.name.split('.')[-1]
+#         cloud_file_path = f"autowork/{DateUtil().now().strftime('%Y%m%d')}/{upload_file_name}"
+#     else:
+#         cloud_file_path = target if target.startswith('autowork') else f'autowork/${target}'
+#
+#     try:
+#         res = asyncio.run(CosFileManager().upload_file(upload_file,
+#                                                        cloud_file_path,
+#                                                        BucketExpireTime.get_expire_time(expire_type)))
+#         if res:
+#             typer.secho(f"文件上传成功, 上传地址：{res}", fg=typer.colors.GREEN)
+#     except Exception as e:
+#         typer.secho(f"上传文件报错：{e}", fg=typer.colors.RED)
+#
+#
+# @file_app.command(help="下载文件")
+# def download(file: Annotated[str, typer.Argument(help='待下载的文件, ')],
+#              outdir: str = typer.Option(None, '-d', '--out-dir', help='下载保存目录'),
+#              expire_type: int = typer.Option(1, '-e', '--expire-type', help='过期类型')):
+#     global download_dir
+#     if file.startswith('http'):
+#         file = '/'.join(file.split('/')[3:])
+#
+#     if outdir is not None:
+#         if outdir.startswith('./'):
+#             download_dir = Path(os.getcwd()).parent.joinpath(outdir)
+#         else:
+#             download_dir = Path(outdir)
+#     else:
+#         download_dir = Path(os.getcwd())
+#
+#     if not download_dir.exists():
+#         download_dir.mkdir(parents=True, exist_ok=True)
+#
+#     download_file = download_dir.joinpath(Path(file).name)
+#
+#     try:
+#         asyncio.run(CosFileManager().download_file(download_file,
+#                                                    file,
+#                                                    BucketExpireTime.get_expire_time(expire_type)))
+#         typer.secho(f"下载文件成功，地址：{download_file}", fg=typer.colors.RED)
+#     except Exception as e:
+#         typer.secho(f"下载文件报错：{e}", fg=typer.colors.RED)
```

### Comparing `autowork-cli-0.1.6/autowork_cli/flow/flow_cmd.py` & `autowork-cli-0.4.5/autowork_cli/flow/flow_cmd.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 
 
 @flow_app.command(help='基于CODE的流程编排')
 def service(app_code: str = typer.Option(None, '-a', '--app-code', prompt='APP CODE', help='应用编码'),
             flow_code: str = typer.Option(None, '-f', '--flow-code', prompt='FLOW CODE', help='流程编码'),
             data: str = typer.Option(None, '-d', '--data', help='详细参数')):
     url = f"{BusinessURLConfig.get_flow_url()}/{app_code}/{flow_code}"
-    process(url, data)
+    return process(url, data)
 
 
 @flow_app.command(help='基于ID的流程编排')
 def service_call(app_id: str = typer.Option(None, '-a', '--app-id', prompt='APP ID', help='应用编号'),
                  flow_id: str = typer.Option(None, '-f', '--flow-id', prompt='FLOW ID', help='流程编号'),
                  data: str = typer.Option(None, '-d', '--data', help='详细参数')):
     url = f"{BusinessURLConfig.get_flow_url()}/{app_id}/{flow_id}/call"
-    process(url, data)
+    return process(url, data)
 
 
 def process(url: str, data: str):
     client = CybotronSyncClient()
     if data is None:
         data = FlowWebRequest()
     else:
@@ -33,9 +33,11 @@
 
     try:
         res = client.send(url, 'POST', data.model_dump())
         if not res.get('success'):
             typer.secho(res.get('message'), fg=typer.colors.RED)
         else:
             typer.secho(f"调用成功, 返回结果：{res}", fg=typer.colors.GREEN)
+        return res['result']
     except Exception as e:
         typer.secho(f"调用报错：{e}", fg=typer.colors.RED)
+
```

### Comparing `autowork-cli-0.1.6/autowork_cli/log/log_cmd.py` & `autowork-cli-0.4.5/autowork_cli/log/log_cmd.py`

 * *Files identical despite different names*

### Comparing `autowork-cli-0.1.6/autowork_cli/repository/cybotron/model/metadataobj.py` & `autowork-cli-0.4.5/autowork_cli/repository/cybotron/model/metadataobj.py`

 * *Files 5% similar despite different names*

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
@@ -125,7 +125,13 @@
 
 class BulkUpdateResponse(BaseModel):
     count: int
 
 
 class BulkDeleteResponse(BaseModel):
     count: int
+
+
+class ServiceFlow(BaseModel):
+    appCode: str
+    FlowCode: str
+    input: dict
```

### Comparing `autowork-cli-0.1.6/autowork_cli/repository/cybotron/service/common_access.py` & `autowork-cli-0.4.5/autowork_cli/repository/cybotron/service/common_access.py`

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

### Comparing `autowork-cli-0.1.6/autowork_cli/repository/cybotron/service/data_accessor.py` & `autowork-cli-0.4.5/autowork_cli/repository/cybotron/service/metadata_accessor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from autowork_cli.common.config.LoginConfig import DefaultLoginConfig
-from autowork_cli.common.config.BaseURLConfig import BaseURLConfig
+from autowork_cli.common.config.BaseURLConfig import DefaultURLConfig
 from autowork_cli.common.config.BusinessURLConfig import BusinessURLConfig, DataTypeEnum
 from autowork_cli.repository.cybotron.service.common_access import CommonAccess
-from autowork_cli.repository.cybotron.model.metadataobj import GetRequest, GetResponse, GetListRequest, GetListResponse
+from autowork_cli.repository.cybotron.model.metadataobj import GetMetaRequest, GetMetaListRequest, GetResponse, GetListResponse
 
 
-class DataAccessor(CommonAccess):
+class MetaDataAccessor(CommonAccess):
     def __init__(self):
         super().__init__()
-        self.URL = BaseURLConfig.get_api_base_url(DefaultLoginConfig.get_env()) + BusinessURLConfig.get_url(
-            DataTypeEnum.DATA)
+        self.URL = DefaultURLConfig.get_api_base_url(DefaultLoginConfig.get_env()) + BusinessURLConfig.get_url(
+            DataTypeEnum.META)
         self.X_API_KEY = DefaultLoginConfig.get_api_key()
 
-    async def get(self, req: GetRequest) -> GetResponse:
+    async def get(self, req: GetMetaRequest) -> GetResponse:
         """
         单条查询接口
         """
         result = await self.get_response(req, "get")
         data = {} if not result.get('data', "") else result['data']  # 查询结果为空, 返回空字典
         return GetResponse(data=data)
 
-    async def getList(self, req: GetListRequest) -> GetListResponse:
+    async def getList(self, req: GetMetaListRequest) -> GetListResponse:
         """
         分页查询接口
         """
         result = await self.get_response(req, "getList")
         return GetListResponse(data=result["data"], total=result["total"])
```

### Comparing `autowork-cli-0.1.6/autowork_cli/repository/cybotron/service/log_accessor.py` & `autowork-cli-0.4.5/autowork_cli/repository/cybotron/service/log_accessor.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from autowork_cli.common.config.BaseURLConfig import BaseURLConfig
+from autowork_cli.common.config.BaseURLConfig import DefaultURLConfig
 from autowork_cli.common.config.BusinessURLConfig import BusinessURLConfig, DataTypeEnum
 from autowork_cli.common.config.ClientConfig import LOG_APP_CODE, LOG_TABLE_CODE
 from autowork_cli.common.config.LoginConfig import DefaultLoginConfig
 from autowork_cli.common.request.CybotronSyncClient import CybotronSyncClient
 from autowork_cli.repository.cybotron.service.common_access import CommonAccess
 
 
 class LogAccessor(CommonAccess):
 
     def __init__(self):
         super().__init__()
-        self.URL = BaseURLConfig.get_api_base_url(DefaultLoginConfig.get_env()) + BusinessURLConfig.get_url(
+        self.URL = DefaultURLConfig.get_api_base_url(DefaultLoginConfig.get_env()) + BusinessURLConfig.get_url(
             DataTypeEnum.DATA)
         self.X_API_KEY = DefaultLoginConfig.get_api_key()
 
     @staticmethod
     def send_log(log_message: dict) -> bool:
         client = CybotronSyncClient()
-        base_url = BaseURLConfig.get_api_base_url(DefaultLoginConfig.get_env())
+        base_url = DefaultURLConfig.get_api_base_url(DefaultLoginConfig.get_env())
         business_url = f"{base_url}{BusinessURLConfig.get_url(DataTypeEnum.DATA)}/{LOG_APP_CODE}/{LOG_TABLE_CODE}/create"
 
         req = {
             "values": log_message,
             "options": {
                 "conflictToUpdate": False
             }
```

### Comparing `autowork-cli-0.1.6/autowork_cli/repository/cybotron/service/metadata_accessor.py` & `autowork-cli-0.4.5/autowork_cli/repository/cybotron/service/data_accessor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from autowork_cli.common.config.LoginConfig import DefaultLoginConfig
-from autowork_cli.common.config.BaseURLConfig import BaseURLConfig
+from autowork_cli.common.config.BaseURLConfig import DefaultURLConfig
 from autowork_cli.common.config.BusinessURLConfig import BusinessURLConfig, DataTypeEnum
 from autowork_cli.repository.cybotron.service.common_access import CommonAccess
-from autowork_cli.repository.cybotron.model.metadataobj import GetMetaRequest, GetMetaListRequest, GetResponse, GetListResponse
+from autowork_cli.repository.cybotron.model.metadataobj import GetRequest, GetResponse, GetListRequest, GetListResponse
 
 
-class MetaDataAccessor(CommonAccess):
+class DataAccessor(CommonAccess):
     def __init__(self):
         super().__init__()
-        self.URL = BaseURLConfig.get_api_base_url(DefaultLoginConfig.get_env()) + BusinessURLConfig.get_url(
-            DataTypeEnum.META)
+        self.URL = DefaultURLConfig.get_api_base_url(DefaultLoginConfig.get_env()) + BusinessURLConfig.get_url(
+            DataTypeEnum.DATA)
         self.X_API_KEY = DefaultLoginConfig.get_api_key()
 
-    async def get(self, req: GetMetaRequest) -> GetResponse:
+    async def get(self, req: GetRequest) -> GetResponse:
         """
         单条查询接口
         """
         result = await self.get_response(req, "get")
         data = {} if not result.get('data', "") else result['data']  # 查询结果为空, 返回空字典
         return GetResponse(data=data)
 
-    async def getList(self, req: GetMetaListRequest) -> GetListResponse:
+    async def getList(self, req: GetListRequest) -> GetListResponse:
         """
         分页查询接口
         """
         result = await self.get_response(req, "getList")
         return GetListResponse(data=result["data"], total=result["total"])
```

### Comparing `autowork-cli-0.1.6/autowork_cli/sidecar/sidecar_app.py` & `autowork-cli-0.4.5/autowork_cli/sidecar/sidecar_app.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import os
 
-from autowork_cli.common.log.AwLogger import AwLogger, Log
+from autowork_cli.common.log.AwLogger import AwLogger, Log, LogRecord
 from fastapi import Request
 from fastapi import FastAPI
 from fastapi.middleware.cors import CORSMiddleware
-
 from autowork_cli.common.lang import logger_setting
 from autowork_cli.common.lang.async_requests import AsyncRequests
 from autowork_cli.sidecar.dev_register import DevRouterRegister
+from autowork_cli.sidecar.dev_websocket import DevWebSocketStart
 from autowork_cli.sidecar.sidecar_mgr import SidecarManager
+from autowork_cli.common.request.forward_request import ForwardRequest
 
 logger_setting.init()
 logger = AwLogger.getLogger(__name__)
 
 sidecar_mgr = SidecarManager()
 app = FastAPI(title="Autowork CLI Sidecar")
 
@@ -23,46 +24,79 @@
     allow_methods=["*"],
     allow_headers=["*"],
 )
 
 
 @app.on_event("startup")
 def dev_router_startup():
-    DevRouterRegister.start()
+    DevWebSocketStart.start()
 
 
 @app.on_event("shutdown")
 async def dev_router_shutdown():
-    await DevRouterRegister.stop()
+    pass
 
 
 @app.get("/health")
 async def health():
     return {
         "pid": os.getpid()
     }
 
 
+@app.post("/forward-request")
+async def forward_request(request: Request):
+    """
+    转发业务请求
+    :param request:
+    :return:
+    """
+    res = await ForwardRequest.send(request)
+    return res
+
+
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
+
+
+async def exec_sandbox_func(app_id: str, func_id: str, data):
+    global trace_id
+    try:
+        app_port = sidecar_mgr.app_port
+        client = AsyncRequests(f"http://localhost:{str(app_port)}")
+
+
+        trace_id = data['traceId']
+        cybotron_access_info = Log(
+            trace_id=trace_id,
+            app_id=app_id,
+            func_id=func_id,
+        )
+        AwLogger.cybotron_access_info[trace_id] = cybotron_access_info
+        logger.info(f'本地边车服务转发赛博坦平台请求，应用编号：{app_id}, 函数编号：{func_id}, 参数：{data}', LogRecord(trace_id=trace_id))
+
+        resp = await client.request(f"/sandbox/call", data, timeout=3600)
+        return resp.json()
+    except BaseException as e:
+        logger.info(f'本地边车服务转发赛博坦平台请求报错，应用编号：{app_id}, 函数编号：{func_id}, 参数：{data}, 报错信息：{e}', LogRecord(trace_id=trace_id))
+        return {"error": str(e), "success": False}
```

### Comparing `autowork-cli-0.1.6/autowork_cli/sidecar/sidecar_cmd.py` & `autowork-cli-0.4.5/autowork_cli/sidecar/sidecar_cmd.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 sc_app = typer.Typer(name='sidecar', help='Autowork边车服务')
 
 sidecar_mgr = SidecarManager()
 
 
 @sc_app.command(help="启动边车服务")
-def start(port: Annotated[int, typer.Option(help="边车端口号")] = 9080,
+def start(port: Annotated[int, typer.Option(help="边车端口号")] = 8081,
           app_port: Annotated[int, typer.Option(help="应用端口号")] = 9000):
     if port == app_port:
         rich.print("[red]边车端口号和应用端口号不能相同")
         return
     rich.print(f"[blue]启动边车服务，监听本地端口号{app_port}")
     sidecar_mgr.port = port
     sidecar_mgr.app_port = app_port
```

### Comparing `autowork-cli-0.1.6/autowork_cli/sidecar/sidecar_mgr.py` & `autowork-cli-0.4.5/autowork_cli/sidecar/sidecar_mgr.py`

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

### Comparing `autowork-cli-0.1.6/autowork_cli/util/dateutil.py` & `autowork-cli-0.4.5/autowork_cli/util/dateutil.py`

 * *Files identical despite different names*

### Comparing `autowork-cli-0.1.6/pyproject.toml` & `autowork-cli-0.4.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autowork-cli"
-version = "0.1.6"
+version = "0.4.5"
 description = ""
 authors = ["Your Name <you@example.com>"]
 readme = "README.md"
 packages = [{include = "autowork_cli"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
@@ -13,14 +13,17 @@
 configparser2 = "^4.0.0"
 httpx = "^0.24.1"
 fastapi = "^0.103.1"
 uvicorn = "^0.23.2"
 requests = "^2.28.1"
 psutil = "^5.9.4"
 coloredlogs = "^15.0.1"
+twine = "^4.0.2"
+websocket-client = "^1.8.0"
+websockets = "^12.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 pytest-asyncio = "^0.21.1"
 
 [build-system]
 requires = ["poetry-core"]
```

