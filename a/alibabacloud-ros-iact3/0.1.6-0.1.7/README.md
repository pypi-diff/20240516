# Comparing `tmp/alibabacloud-ros-iact3-0.1.6.tar.gz` & `tmp/alibabacloud-ros-iact3-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud-ros-iact3-0.1.6.tar", last modified: Wed Feb 21 08:24:56 2024, max compression
+gzip compressed data, was "dist/alibabacloud-ros-iact3-0.1.7.tar", last modified: Thu May 16 11:40:09 2024, max compression
```

## Comparing `alibabacloud-ros-iact3-0.1.6.tar` & `alibabacloud-ros-iact3-0.1.7.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/
--rw-r--r--   0 root         (0) root         (0)      111 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1582 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      679 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/alibabacloud_ros_iact3.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1582 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/alibabacloud_ros_iact3.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1045 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/alibabacloud_ros_iact3.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/alibabacloud_ros_iact3.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1448 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/alibabacloud_ros_iact3.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/alibabacloud_ros_iact3.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/bin/
--rwxr-xr-x   0 root         (0) root         (0)      450 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/bin/iact3
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/iact3/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/iact3/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11139 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/iact3/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/iact3/cli_modules/
--rw-r--r--   0 root         (0) root         (0)      206 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/iact3/cli_modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4177 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/iact3/cli_modules/base.py
--rw-r--r--   0 root         (0) root         (0)     1230 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/iact3/cli_modules/cost.py
--rw-r--r--   0 root         (0) root         (0)     1652 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/iact3/cli_modules/delete.py
--rw-r--r--   0 root         (0) root         (0)     4439 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/iact3/cli_modules/list.py
--rw-r--r--   0 root         (0) root         (0)     2441 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/iact3/cli_modules/policy.py
--rw-r--r--   0 root         (0) root         (0)     1591 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/iact3/cli_modules/preview.py
--rw-r--r--   0 root         (0) root         (0)     4287 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/iact3/cli_modules/test.py
--rw-r--r--   0 root         (0) root         (0)     2450 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/iact3/cli_modules/validate.py
--rw-r--r--   0 root         (0) root         (0)    18487 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/iact3/config.py
--rw-r--r--   0 root         (0) root         (0)      521 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/iact3/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    17415 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/iact3/generate_params.py
--rw-r--r--   0 root         (0) root         (0)     1862 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/iact3/logger.py
--rwxr-xr-x   0 root         (0) root         (0)     1829 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/iact3/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/iact3/plugin/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/iact3/plugin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8040 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/iact3/plugin/base_plugin.py
--rw-r--r--   0 root         (0) root         (0)      963 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/iact3/plugin/ecs.py
--rw-r--r--   0 root         (0) root         (0)     1096 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/iact3/plugin/error_code.py
--rw-r--r--   0 root         (0) root         (0)     3550 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/iact3/plugin/oss.py
--rw-r--r--   0 root         (0) root         (0)     8547 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/iact3/plugin/ros.py
--rw-r--r--   0 root         (0) root         (0)     1074 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/iact3/plugin/vpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/iact3/report/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/iact3/report/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13884 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/iact3/report/generate_reports.py
--rw-r--r--   0 root         (0) root         (0)     3805 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/iact3/report/html.css
--rw-r--r--   0 root         (0) root         (0)    17804 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/iact3/stack.py
--rw-r--r--   0 root         (0) root         (0)    13288 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/iact3/termial_print.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/iact3/testing/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/iact3/testing/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5951 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/iact3/testing/base.py
--rw-r--r--   0 root         (0) root         (0)     2214 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/iact3/testing/ros_stack.py
--rw-r--r--   0 root         (0) root         (0)      808 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/iact3/util.py
--rw-r--r--   0 root         (0) root         (0)       37 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/requirements-dev.txt
--rw-r--r--   0 root         (0) root         (0)     1448 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1230 2024-02-21 08:24:56.000000 alibabacloud-ros-iact3-0.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 11:40:09.000000 alibabacloud-ros-iact3-0.1.7/
+-rw-r--r--   0 root         (0) root         (0)      111 2024-05-16 11:40:08.000000 alibabacloud-ros-iact3-0.1.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1582 2024-05-16 11:40:09.000000 alibabacloud-ros-iact3-0.1.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      679 2024-05-16 11:40:08.000000 alibabacloud-ros-iact3-0.1.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 11:40:09.000000 alibabacloud-ros-iact3-0.1.7/alibabacloud_ros_iact3.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1582 2024-05-16 11:40:09.000000 alibabacloud-ros-iact3-0.1.7/alibabacloud_ros_iact3.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1045 2024-05-16 11:40:09.000000 alibabacloud-ros-iact3-0.1.7/alibabacloud_ros_iact3.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 11:40:09.000000 alibabacloud-ros-iact3-0.1.7/alibabacloud_ros_iact3.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1448 2024-05-16 11:40:09.000000 alibabacloud-ros-iact3-0.1.7/alibabacloud_ros_iact3.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-16 11:40:09.000000 alibabacloud-ros-iact3-0.1.7/alibabacloud_ros_iact3.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 11:40:09.000000 alibabacloud-ros-iact3-0.1.7/bin/
+-rwxr-xr-x   0 root         (0) root         (0)      450 2024-05-16 11:40:08.000000 alibabacloud-ros-iact3-0.1.7/bin/iact3
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 11:40:09.000000 alibabacloud-ros-iact3-0.1.7/iact3/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 11:40:08.000000 alibabacloud-ros-iact3-0.1.7/iact3/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11139 2024-05-16 11:40:08.000000 alibabacloud-ros-iact3-0.1.7/iact3/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 11:40:09.000000 alibabacloud-ros-iact3-0.1.7/iact3/cli_modules/
+-rw-r--r--   0 root         (0) root         (0)      206 2024-05-16 11:40:08.000000 alibabacloud-ros-iact3-0.1.7/iact3/cli_modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4177 2024-05-16 11:40:08.000000 alibabacloud-ros-iact3-0.1.7/iact3/cli_modules/base.py
+-rw-r--r--   0 root         (0) root         (0)     1230 2024-05-16 11:40:08.000000 alibabacloud-ros-iact3-0.1.7/iact3/cli_modules/cost.py
+-rw-r--r--   0 root         (0) root         (0)     1714 2024-05-16 11:40:08.000000 alibabacloud-ros-iact3-0.1.7/iact3/cli_modules/delete.py
+-rw-r--r--   0 root         (0) root         (0)     4501 2024-05-16 11:40:08.000000 alibabacloud-ros-iact3-0.1.7/iact3/cli_modules/list.py
+-rw-r--r--   0 root         (0) root         (0)     2441 2024-05-16 11:40:08.000000 alibabacloud-ros-iact3-0.1.7/iact3/cli_modules/policy.py
+-rw-r--r--   0 root         (0) root         (0)     1591 2024-05-16 11:40:08.000000 alibabacloud-ros-iact3-0.1.7/iact3/cli_modules/preview.py
+-rw-r--r--   0 root         (0) root         (0)     4457 2024-05-16 11:40:08.000000 alibabacloud-ros-iact3-0.1.7/iact3/cli_modules/test.py
+-rw-r--r--   0 root         (0) root         (0)     2450 2024-05-16 11:40:08.000000 alibabacloud-ros-iact3-0.1.7/iact3/cli_modules/validate.py
+-rw-r--r--   0 root         (0) root         (0)    18487 2024-05-16 11:40:08.000000 alibabacloud-ros-iact3-0.1.7/iact3/config.py
+-rw-r--r--   0 root         (0) root         (0)      521 2024-05-16 11:40:08.000000 alibabacloud-ros-iact3-0.1.7/iact3/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    17415 2024-05-16 11:40:08.000000 alibabacloud-ros-iact3-0.1.7/iact3/generate_params.py
+-rw-r--r--   0 root         (0) root         (0)     1862 2024-05-16 11:40:08.000000 alibabacloud-ros-iact3-0.1.7/iact3/logger.py
+-rwxr-xr-x   0 root         (0) root         (0)     1829 2024-05-16 11:40:08.000000 alibabacloud-ros-iact3-0.1.7/iact3/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 11:40:09.000000 alibabacloud-ros-iact3-0.1.7/iact3/plugin/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 11:40:08.000000 alibabacloud-ros-iact3-0.1.7/iact3/plugin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8040 2024-05-16 11:40:08.000000 alibabacloud-ros-iact3-0.1.7/iact3/plugin/base_plugin.py
+-rw-r--r--   0 root         (0) root         (0)      963 2024-05-16 11:40:08.000000 alibabacloud-ros-iact3-0.1.7/iact3/plugin/ecs.py
+-rw-r--r--   0 root         (0) root         (0)     1096 2024-05-16 11:40:08.000000 alibabacloud-ros-iact3-0.1.7/iact3/plugin/error_code.py
+-rw-r--r--   0 root         (0) root         (0)     3550 2024-05-16 11:40:08.000000 alibabacloud-ros-iact3-0.1.7/iact3/plugin/oss.py
+-rw-r--r--   0 root         (0) root         (0)     8581 2024-05-16 11:40:08.000000 alibabacloud-ros-iact3-0.1.7/iact3/plugin/ros.py
+-rw-r--r--   0 root         (0) root         (0)     1074 2024-05-16 11:40:08.000000 alibabacloud-ros-iact3-0.1.7/iact3/plugin/vpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 11:40:09.000000 alibabacloud-ros-iact3-0.1.7/iact3/report/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 11:40:08.000000 alibabacloud-ros-iact3-0.1.7/iact3/report/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13884 2024-05-16 11:40:08.000000 alibabacloud-ros-iact3-0.1.7/iact3/report/generate_reports.py
+-rw-r--r--   0 root         (0) root         (0)     3805 2024-05-16 11:40:08.000000 alibabacloud-ros-iact3-0.1.7/iact3/report/html.css
+-rw-r--r--   0 root         (0) root         (0)    17804 2024-05-16 11:40:08.000000 alibabacloud-ros-iact3-0.1.7/iact3/stack.py
+-rw-r--r--   0 root         (0) root         (0)    13288 2024-05-16 11:40:08.000000 alibabacloud-ros-iact3-0.1.7/iact3/termial_print.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 11:40:09.000000 alibabacloud-ros-iact3-0.1.7/iact3/testing/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 11:40:08.000000 alibabacloud-ros-iact3-0.1.7/iact3/testing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5951 2024-05-16 11:40:08.000000 alibabacloud-ros-iact3-0.1.7/iact3/testing/base.py
+-rw-r--r--   0 root         (0) root         (0)     2214 2024-05-16 11:40:08.000000 alibabacloud-ros-iact3-0.1.7/iact3/testing/ros_stack.py
+-rw-r--r--   0 root         (0) root         (0)      808 2024-05-16 11:40:08.000000 alibabacloud-ros-iact3-0.1.7/iact3/util.py
+-rw-r--r--   0 root         (0) root         (0)       37 2024-05-16 11:40:08.000000 alibabacloud-ros-iact3-0.1.7/requirements-dev.txt
+-rw-r--r--   0 root         (0) root         (0)     1448 2024-05-16 11:40:08.000000 alibabacloud-ros-iact3-0.1.7/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-16 11:40:09.000000 alibabacloud-ros-iact3-0.1.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1230 2024-05-16 11:40:08.000000 alibabacloud-ros-iact3-0.1.7/setup.py
```

### Comparing `alibabacloud-ros-iact3-0.1.6/PKG-INFO` & `alibabacloud-ros-iact3-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-ros-iact3
-Version: 0.1.6
+Version: 0.1.7
 Summary: Iact3 is a tool that tests Terraform and ROS(Resource Orchestration Service) templates.
 Home-page: UNKNOWN
 Author: AlibabaCloud
 License: UNKNOWN
 Description: # IaC Template Testing Tool
         
         Iact3(IaC Template Testing Tool) is a tool that tests [Alibaba Cloud ROS(Resource Orchestration Service)](https://www.alibabacloud.com/help/resource-orchestration-service) templates and  [Terraform](https://developer.hashicorp.com/terraform). It deploys your template in multiple Alibaba Cloud Regions and generates a report for each region via a simple configuration file.
```

### Comparing `alibabacloud-ros-iact3-0.1.6/README.md` & `alibabacloud-ros-iact3-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.6/alibabacloud_ros_iact3.egg-info/PKG-INFO` & `alibabacloud-ros-iact3-0.1.7/alibabacloud_ros_iact3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-ros-iact3
-Version: 0.1.6
+Version: 0.1.7
 Summary: Iact3 is a tool that tests Terraform and ROS(Resource Orchestration Service) templates.
 Home-page: UNKNOWN
 Author: AlibabaCloud
 License: UNKNOWN
 Description: # IaC Template Testing Tool
         
         Iact3(IaC Template Testing Tool) is a tool that tests [Alibaba Cloud ROS(Resource Orchestration Service)](https://www.alibabacloud.com/help/resource-orchestration-service) templates and  [Terraform](https://developer.hashicorp.com/terraform). It deploys your template in multiple Alibaba Cloud Regions and generates a report for each region via a simple configuration file.
```

### Comparing `alibabacloud-ros-iact3-0.1.6/alibabacloud_ros_iact3.egg-info/SOURCES.txt` & `alibabacloud-ros-iact3-0.1.7/alibabacloud_ros_iact3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.6/alibabacloud_ros_iact3.egg-info/requires.txt` & `alibabacloud-ros-iact3-0.1.7/alibabacloud_ros_iact3.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.6/iact3/cli.py` & `alibabacloud-ros-iact3-0.1.7/iact3/cli.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.6/iact3/cli_modules/base.py` & `alibabacloud-ros-iact3-0.1.7/iact3/cli_modules/base.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.6/iact3/cli_modules/cost.py` & `alibabacloud-ros-iact3-0.1.7/iact3/cli_modules/cost.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.6/iact3/cli_modules/delete.py` & `alibabacloud-ros-iact3-0.1.7/iact3/cli_modules/delete.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,17 +24,18 @@
         self.config_file = config_file
         self.project_path = project_path
 
     @classmethod
     async def create(cls, regions: str = None,
                      config_file: str = None,
                      project_path: str = None,
-                     tags: dict = None):
+                     tags: dict = None,
+                     stack_id: str = None):
         credential = List.get_credential(config_file, project_path)
-        all_stacks = await List.create(regions, config_file, project_path, tags)
+        all_stacks = await List.create(regions, config_file, project_path, tags, stack_id=stack_id)
         if not all_stacks:
             LOG.info('can not find stack to delete.')
             return
         LOG.info('Start delete above stacks')
         printer = TerminalPrinter()
 
         for i in range(0, len(all_stacks), LIMIT):
```

### Comparing `alibabacloud-ros-iact3-0.1.6/iact3/cli_modules/list.py` & `alibabacloud-ros-iact3-0.1.7/iact3/cli_modules/list.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,30 +26,31 @@
         self.config_file = config_file
         self.project_path = project_path
 
     @classmethod
     async def create(cls, regions: str = None,
                      config_file: str = None,
                      project_path: str = None,
-                     tags: dict = None):
+                     tags: dict = None,
+                     stack_id: str = None):
         credential = cls.get_credential(config_file, project_path)
         if regions:
             regions = regions.split(',')
         else:
             region_plugin = StackPlugin(region_id='cn-hangzhou', credential=credential)
             regions = await region_plugin.get_regions()
         list_tasks = []
         if tags:
             tags.update(SYS_TAGS)
         else:
             tags = SYS_TAGS
         for region in regions:
             stack_plugin = StackPlugin(region_id=region, credential=credential)
             list_tasks.append(
-                asyncio.create_task(stack_plugin.fetch_all_stacks(tags))
+                asyncio.create_task(stack_plugin.fetch_all_stacks(tags, stack_id=stack_id))
             )
         stacks = await asyncio.gather(*list_tasks)
         all_stacks, project_length, test_length, stack_name_length = cls._get_all_stacks(stacks)
         if not all_stacks:
             LOG.info('can not find any stack.')
             return
         header = f'ProjectName{" "*project_length}TestName{" "*test_length}StackName{" "*stack_name_length}Region'
```

### Comparing `alibabacloud-ros-iact3-0.1.6/iact3/cli_modules/policy.py` & `alibabacloud-ros-iact3-0.1.7/iact3/cli_modules/policy.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.6/iact3/cli_modules/preview.py` & `alibabacloud-ros-iact3-0.1.7/iact3/cli_modules/preview.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.6/iact3/cli_modules/test.py` & `alibabacloud-ros-iact3-0.1.7/iact3/cli_modules/test.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,20 +64,22 @@
             Test._get_parameters(tests)
             return
 
         async with tests:
             await tests.report(output_directory, project_path, log_format)
 
     @staticmethod
-    async def clean(regions: str = None):
+    @CliCore.longform_param_required('stack_id')
+    async def clean(regions: str = None, stack_id: str = None):
         '''
         Manually clean up the stacks which were created by Iact3
         :param regions: comma separated list of regions to delete from, default will scan all regions
+        :param stack_id: stack_id to delete from, default will scan all regions
         '''
-        await Delete.create(regions)
+        await Delete.create(regions, stack_id=stack_id)
 
     @staticmethod
     async def list(regions: str = None):
         '''
         List stacks which were created by Iact3 for all regions
         :param regions:  comma separated list of regions to delete from, default will scan all regions
         '''
```

### Comparing `alibabacloud-ros-iact3-0.1.6/iact3/cli_modules/validate.py` & `alibabacloud-ros-iact3-0.1.7/iact3/cli_modules/validate.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.6/iact3/config.py` & `alibabacloud-ros-iact3-0.1.7/iact3/config.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.6/iact3/exceptions.py` & `alibabacloud-ros-iact3-0.1.7/iact3/exceptions.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.6/iact3/generate_params.py` & `alibabacloud-ros-iact3-0.1.7/iact3/generate_params.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.6/iact3/logger.py` & `alibabacloud-ros-iact3-0.1.7/iact3/logger.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.6/iact3/main.py` & `alibabacloud-ros-iact3-0.1.7/iact3/main.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.6/iact3/plugin/base_plugin.py` & `alibabacloud-ros-iact3-0.1.7/iact3/plugin/base_plugin.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.6/iact3/plugin/ecs.py` & `alibabacloud-ros-iact3-0.1.7/iact3/plugin/ecs.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.6/iact3/plugin/error_code.py` & `alibabacloud-ros-iact3-0.1.7/iact3/plugin/error_code.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.6/iact3/plugin/oss.py` & `alibabacloud-ros-iact3-0.1.7/iact3/plugin/oss.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.6/iact3/plugin/ros.py` & `alibabacloud-ros-iact3-0.1.7/iact3/plugin/ros.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,16 +108,16 @@
         request_kwargs = dict(
             StackId=stack_id,
             StackName=[stack_name] if stack_name else None
         )
         result = await self.send_request('ListStacksRequest', **request_kwargs)
         return result.get('Stacks')
 
-    async def fetch_all_stacks(self, tags):
-        kwargs = {}
+    async def fetch_all_stacks(self, tags, stack_id=None):
+        kwargs = {'StackId': stack_id}
         self._convert_tags(tags, kwargs, tag_key='Tag')
         return await self.fetch_all('ListStacksRequest', kwargs, 'Stacks')
 
     async def list_stack_resources(self, stack_id):
         kwargs = dict(
             StackId=stack_id
         )
```

### Comparing `alibabacloud-ros-iact3-0.1.6/iact3/plugin/vpc.py` & `alibabacloud-ros-iact3-0.1.7/iact3/plugin/vpc.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.6/iact3/report/generate_reports.py` & `alibabacloud-ros-iact3-0.1.7/iact3/report/generate_reports.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.6/iact3/report/html.css` & `alibabacloud-ros-iact3-0.1.7/iact3/report/html.css`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.6/iact3/stack.py` & `alibabacloud-ros-iact3-0.1.7/iact3/stack.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.6/iact3/termial_print.py` & `alibabacloud-ros-iact3-0.1.7/iact3/termial_print.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.6/iact3/testing/base.py` & `alibabacloud-ros-iact3-0.1.7/iact3/testing/base.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.6/iact3/testing/ros_stack.py` & `alibabacloud-ros-iact3-0.1.7/iact3/testing/ros_stack.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.6/iact3/util.py` & `alibabacloud-ros-iact3-0.1.7/iact3/util.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.6/requirements.txt` & `alibabacloud-ros-iact3-0.1.7/requirements.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.6/setup.py` & `alibabacloud-ros-iact3-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with open("README.md") as fp:
     long_description = fp.read()
 
 
 setuptools.setup(
     name="alibabacloud-ros-iact3",
-    version="0.1.6",
+    version="0.1.7",
 
     description="Iact3 is a tool that tests Terraform and ROS(Resource Orchestration Service) templates.",
     long_description=long_description,
     long_description_content_type="text/markdown",
 
     author="AlibabaCloud",
     packages=[
```

