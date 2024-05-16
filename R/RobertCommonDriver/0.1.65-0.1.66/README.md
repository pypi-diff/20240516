# Comparing `tmp/RobertCommonDriver-0.1.65.tar.gz` & `tmp/RobertCommonDriver-0.1.66.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RobertCommonDriver-0.1.65.tar", last modified: Mon Mar 11 07:52:05 2024, max compression
+gzip compressed data, was "RobertCommonDriver-0.1.66.tar", last modified: Thu May 16 02:10:14 2024, max compression
```

## Comparing `RobertCommonDriver-0.1.65.tar` & `RobertCommonDriver-0.1.66.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxrwx   0        0        0        0 2024-03-11 07:52:05.767203 RobertCommonDriver-0.1.65/
--rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonDriver-0.1.65/LICENSE
--rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonDriver-0.1.65/MANIFEST.in
--rw-rw-rw-   0        0        0      850 2024-03-11 07:52:05.767203 RobertCommonDriver-0.1.65/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-06-02 07:57:02.000000 RobertCommonDriver-0.1.65/README.md
-drwxrwxrwx   0        0        0        0 2024-03-11 07:52:05.703810 RobertCommonDriver-0.1.65/RobertCommonDriver.egg-info/
--rw-rw-rw-   0        0        0      850 2024-03-11 07:52:05.000000 RobertCommonDriver-0.1.65/RobertCommonDriver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2802 2024-03-11 07:52:05.000000 RobertCommonDriver-0.1.65/RobertCommonDriver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-11 07:52:05.000000 RobertCommonDriver-0.1.65/RobertCommonDriver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      214 2024-03-11 07:52:05.000000 RobertCommonDriver-0.1.65/RobertCommonDriver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2024-03-11 07:52:05.000000 RobertCommonDriver-0.1.65/RobertCommonDriver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      229 2024-01-16 07:43:55.000000 RobertCommonDriver-0.1.65/requirements.txt
-drwxrwxrwx   0        0        0        0 2024-03-11 07:52:05.704806 RobertCommonDriver-0.1.65/robertcommondriver/
--rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonDriver-0.1.65/robertcommondriver/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-11 07:52:05.705803 RobertCommonDriver-0.1.65/robertcommondriver/system/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.65/robertcommondriver/system/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-11 07:52:05.721156 RobertCommonDriver-0.1.65/robertcommondriver/system/driver/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.65/robertcommondriver/system/driver/__init__.py
--rw-rw-rw-   0        0        0    87436 2023-06-09 02:14:48.000000 RobertCommonDriver-0.1.65/robertcommondriver/system/driver/bacnet.py
--rw-rw-rw-   0        0        0   495630 2023-06-15 07:05:44.000000 RobertCommonDriver-0.1.65/robertcommondriver/system/driver/bacnetc.py
--rw-rw-rw-   0        0        0     6074 2024-01-22 03:09:43.000000 RobertCommonDriver-0.1.65/robertcommondriver/system/driver/base.py
--rw-rw-rw-   0        0        0        0 2021-10-25 01:55:43.000000 RobertCommonDriver-0.1.65/robertcommondriver/system/driver/iec104.py
--rw-rw-rw-   0        0        0    38348 2023-06-15 07:05:44.000000 RobertCommonDriver-0.1.65/robertcommondriver/system/driver/modbus.py
--rw-rw-rw-   0        0        0    14000 2022-12-01 09:27:31.000000 RobertCommonDriver-0.1.65/robertcommondriver/system/driver/obix.py
--rw-rw-rw-   0        0        0    60844 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.65/robertcommondriver/system/driver/opcda.py
--rw-rw-rw-   0        0        0    17038 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.65/robertcommondriver/system/driver/opcda_openopc.py
--rw-rw-rw-   0        0        0    15983 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.65/robertcommondriver/system/driver/opcua.py
--rw-rw-rw-   0        0        0    33507 2023-08-02 02:36:46.000000 RobertCommonDriver-0.1.65/robertcommondriver/system/driver/plcs7.py
--rw-rw-rw-   0        0        0    16600 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.65/robertcommondriver/system/driver/snmp.py
-drwxrwxrwx   0        0        0        0 2024-03-11 07:52:05.737391 RobertCommonDriver-0.1.65/robertcommondriver/system/iot/
--rw-rw-rw-   0        0        0        0 2022-06-15 07:27:26.000000 RobertCommonDriver-0.1.65/robertcommondriver/system/iot/__init__.py
--rw-rw-rw-   0        0        0    72246 2024-03-07 06:03:55.000000 RobertCommonDriver-0.1.65/robertcommondriver/system/iot/base.py
--rw-rw-rw-   0        0        0    66929 2024-01-18 08:31:41.000000 RobertCommonDriver-0.1.65/robertcommondriver/system/iot/iot_bacnet.py
--rw-rw-rw-   0        0        0   566426 2024-01-18 08:31:41.000000 RobertCommonDriver-0.1.65/robertcommondriver/system/iot/iot_bacnet_mstp.py
--rw-rw-rw-   0        0        0   144746 2024-01-31 07:10:00.000000 RobertCommonDriver-0.1.65/robertcommondriver/system/iot/iot_iec104.py
--rw-rw-rw-   0        0        0    34927 2024-03-11 07:51:49.000000 RobertCommonDriver-0.1.65/robertcommondriver/system/iot/iot_modbus.py
--rw-rw-rw-   0        0        0    18508 2024-01-18 08:31:41.000000 RobertCommonDriver-0.1.65/robertcommondriver/system/iot/iot_obix.py
--rw-rw-rw-   0        0        0    79313 2024-01-18 08:31:41.000000 RobertCommonDriver-0.1.65/robertcommondriver/system/iot/iot_opcda.py
--rw-rw-rw-   0        0        0    25840 2024-01-18 08:31:42.000000 RobertCommonDriver-0.1.65/robertcommondriver/system/iot/iot_opcua.py
--rw-rw-rw-   0        0        0    43574 2024-01-18 08:31:42.000000 RobertCommonDriver-0.1.65/robertcommondriver/system/iot/iot_plc_ab.py
--rw-rw-rw-   0        0        0    51831 2024-01-18 08:31:59.000000 RobertCommonDriver-0.1.65/robertcommondriver/system/iot/iot_plc_mitsubishi.py
--rw-rw-rw-   0        0        0    41842 2024-01-18 08:32:12.000000 RobertCommonDriver-0.1.65/robertcommondriver/system/iot/iot_plc_omron.py
--rw-rw-rw-   0        0        0    40158 2024-01-18 08:32:28.000000 RobertCommonDriver-0.1.65/robertcommondriver/system/iot/iot_plc_s7.py
--rw-rw-rw-   0        0        0    46487 2024-01-18 08:32:45.000000 RobertCommonDriver-0.1.65/robertcommondriver/system/iot/iot_plc_siemens.py
--rw-rw-rw-   0        0        0    13603 2024-03-11 07:18:37.000000 RobertCommonDriver-0.1.65/robertcommondriver/system/iot/iot_snmp.py
--rw-rw-rw-   0        0        0       42 2024-03-11 07:52:05.767203 RobertCommonDriver-0.1.65/setup.cfg
--rw-rw-rw-   0        0        0     3881 2024-03-11 07:51:49.000000 RobertCommonDriver-0.1.65/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-11 07:52:05.738645 RobertCommonDriver-0.1.65/tests/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonDriver-0.1.65/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-11 07:52:05.738645 RobertCommonDriver-0.1.65/tests/test_system/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:49:45.000000 RobertCommonDriver-0.1.65/tests/test_system/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-11 07:52:05.750033 RobertCommonDriver-0.1.65/tests/test_system/test_driver/
--rw-rw-rw-   0        0        0        0 2021-08-06 06:51:11.000000 RobertCommonDriver-0.1.65/tests/test_system/test_driver/__init__.py
--rw-rw-rw-   0        0        0     6948 2022-06-08 07:19:27.000000 RobertCommonDriver-0.1.65/tests/test_system/test_driver/test_bacnet.py
--rw-rw-rw-   0        0        0     2038 2022-04-14 03:52:19.000000 RobertCommonDriver-0.1.65/tests/test_system/test_driver/test_bacnet1.py
--rw-rw-rw-   0        0        0     3839 2022-08-02 01:50:14.000000 RobertCommonDriver-0.1.65/tests/test_system/test_driver/test_bacnetc.py
--rw-rw-rw-   0        0        0     7865 2022-06-14 02:23:23.000000 RobertCommonDriver-0.1.65/tests/test_system/test_driver/test_bacnetv1.py
--rw-rw-rw-   0        0        0     2008 2022-01-13 07:23:11.000000 RobertCommonDriver-0.1.65/tests/test_system/test_driver/test_modbus.py
--rw-rw-rw-   0        0        0     9784 2022-07-21 02:42:09.000000 RobertCommonDriver-0.1.65/tests/test_system/test_driver/test_obix.py
--rw-rw-rw-   0        0        0     5912 2022-07-07 09:34:12.000000 RobertCommonDriver-0.1.65/tests/test_system/test_driver/test_opcda.py
--rw-rw-rw-   0        0        0     1686 2022-07-13 03:25:06.000000 RobertCommonDriver-0.1.65/tests/test_system/test_driver/test_opcua.py
--rw-rw-rw-   0        0        0     2443 2022-08-12 05:55:46.000000 RobertCommonDriver-0.1.65/tests/test_system/test_driver/test_plcs7.py
--rw-rw-rw-   0        0        0     1444 2022-07-12 05:58:47.000000 RobertCommonDriver-0.1.65/tests/test_system/test_driver/test_snmp.py
-drwxrwxrwx   0        0        0        0 2024-03-11 07:52:05.766204 RobertCommonDriver-0.1.65/tests/test_system/test_iot/
--rw-rw-rw-   0        0        0        0 2022-06-15 07:28:45.000000 RobertCommonDriver-0.1.65/tests/test_system/test_iot/__init__.py
--rw-rw-rw-   0        0        0     3227 2022-06-20 07:43:32.000000 RobertCommonDriver-0.1.65/tests/test_system/test_iot/test_bacnet1.py
--rw-rw-rw-   0        0        0    25246 2023-10-08 12:56:05.000000 RobertCommonDriver-0.1.65/tests/test_system/test_iot/test_iot_bacnet.py
--rw-rw-rw-   0        0        0    20074 2023-04-17 06:34:20.000000 RobertCommonDriver-0.1.65/tests/test_system/test_iot/test_iot_bacnet_mstp.py
--rw-rw-rw-   0        0        0     5554 2024-01-31 07:03:54.000000 RobertCommonDriver-0.1.65/tests/test_system/test_iot/test_iot_iec104.py
--rw-rw-rw-   0        0        0    17686 2024-03-07 03:28:51.000000 RobertCommonDriver-0.1.65/tests/test_system/test_iot/test_iot_modbus.py
--rw-rw-rw-   0        0        0     4721 2024-01-12 07:59:56.000000 RobertCommonDriver-0.1.65/tests/test_system/test_iot/test_iot_obix.py
--rw-rw-rw-   0        0        0     6315 2023-10-11 07:31:18.000000 RobertCommonDriver-0.1.65/tests/test_system/test_iot/test_iot_opcda.py
--rw-rw-rw-   0        0        0     5146 2023-10-13 03:05:10.000000 RobertCommonDriver-0.1.65/tests/test_system/test_iot/test_iot_opcua.py
--rw-rw-rw-   0        0        0     1374 2023-04-14 09:46:49.000000 RobertCommonDriver-0.1.65/tests/test_system/test_iot/test_iot_plc_ab.py
--rw-rw-rw-   0        0        0     2510 2023-04-14 09:44:42.000000 RobertCommonDriver-0.1.65/tests/test_system/test_iot/test_iot_plc_mitsubishi.py
--rw-rw-rw-   0        0        0     2836 2023-04-14 09:45:55.000000 RobertCommonDriver-0.1.65/tests/test_system/test_iot/test_iot_plc_omron.py
--rw-rw-rw-   0        0        0    11822 2023-11-07 14:02:46.000000 RobertCommonDriver-0.1.65/tests/test_system/test_iot/test_iot_plc_s7.py
--rw-rw-rw-   0        0        0     4145 2023-07-27 06:41:53.000000 RobertCommonDriver-0.1.65/tests/test_system/test_iot/test_iot_plc_siemens.py
--rw-rw-rw-   0        0        0      350 2022-08-16 09:35:34.000000 RobertCommonDriver-0.1.65/tests/test_system/test_iot/test_iot_plc_simenses1.py
--rw-rw-rw-   0        0        0     3470 2024-03-11 06:22:29.000000 RobertCommonDriver-0.1.65/tests/test_system/test_iot/test_iot_snmp.py
+drwxrwxrwx   0        0        0        0 2024-05-16 02:10:14.373363 RobertCommonDriver-0.1.66/
+-rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonDriver-0.1.66/LICENSE
+-rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonDriver-0.1.66/MANIFEST.in
+-rw-rw-rw-   0        0        0      850 2024-05-16 02:10:14.373363 RobertCommonDriver-0.1.66/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-06-02 07:57:02.000000 RobertCommonDriver-0.1.66/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 02:10:14.295883 RobertCommonDriver-0.1.66/RobertCommonDriver.egg-info/
+-rw-rw-rw-   0        0        0      850 2024-05-16 02:10:14.000000 RobertCommonDriver-0.1.66/RobertCommonDriver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2802 2024-05-16 02:10:14.000000 RobertCommonDriver-0.1.66/RobertCommonDriver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 02:10:14.000000 RobertCommonDriver-0.1.66/RobertCommonDriver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      214 2024-05-16 02:10:14.000000 RobertCommonDriver-0.1.66/RobertCommonDriver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2024-05-16 02:10:14.000000 RobertCommonDriver-0.1.66/RobertCommonDriver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      229 2024-01-16 07:43:55.000000 RobertCommonDriver-0.1.66/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 02:10:14.295883 RobertCommonDriver-0.1.66/robertcommondriver/
+-rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonDriver-0.1.66/robertcommondriver/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 02:10:14.296926 RobertCommonDriver-0.1.66/robertcommondriver/system/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.66/robertcommondriver/system/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 02:10:14.310627 RobertCommonDriver-0.1.66/robertcommondriver/system/driver/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.66/robertcommondriver/system/driver/__init__.py
+-rw-rw-rw-   0        0        0    87436 2023-06-09 02:14:48.000000 RobertCommonDriver-0.1.66/robertcommondriver/system/driver/bacnet.py
+-rw-rw-rw-   0        0        0   495630 2023-06-15 07:05:44.000000 RobertCommonDriver-0.1.66/robertcommondriver/system/driver/bacnetc.py
+-rw-rw-rw-   0        0        0     6074 2024-01-22 03:09:43.000000 RobertCommonDriver-0.1.66/robertcommondriver/system/driver/base.py
+-rw-rw-rw-   0        0        0        0 2021-10-25 01:55:43.000000 RobertCommonDriver-0.1.66/robertcommondriver/system/driver/iec104.py
+-rw-rw-rw-   0        0        0    38349 2024-04-03 08:06:53.000000 RobertCommonDriver-0.1.66/robertcommondriver/system/driver/modbus.py
+-rw-rw-rw-   0        0        0    14000 2022-12-01 09:27:31.000000 RobertCommonDriver-0.1.66/robertcommondriver/system/driver/obix.py
+-rw-rw-rw-   0        0        0    60844 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.66/robertcommondriver/system/driver/opcda.py
+-rw-rw-rw-   0        0        0    17038 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.66/robertcommondriver/system/driver/opcda_openopc.py
+-rw-rw-rw-   0        0        0    15983 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.66/robertcommondriver/system/driver/opcua.py
+-rw-rw-rw-   0        0        0    33507 2023-08-02 02:36:46.000000 RobertCommonDriver-0.1.66/robertcommondriver/system/driver/plcs7.py
+-rw-rw-rw-   0        0        0    16600 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.66/robertcommondriver/system/driver/snmp.py
+drwxrwxrwx   0        0        0        0 2024-05-16 02:10:14.332559 RobertCommonDriver-0.1.66/robertcommondriver/system/iot/
+-rw-rw-rw-   0        0        0        0 2022-06-15 07:27:26.000000 RobertCommonDriver-0.1.66/robertcommondriver/system/iot/__init__.py
+-rw-rw-rw-   0        0        0    72774 2024-05-15 09:13:17.000000 RobertCommonDriver-0.1.66/robertcommondriver/system/iot/base.py
+-rw-rw-rw-   0        0        0    66929 2024-01-18 08:31:41.000000 RobertCommonDriver-0.1.66/robertcommondriver/system/iot/iot_bacnet.py
+-rw-rw-rw-   0        0        0   566426 2024-01-18 08:31:41.000000 RobertCommonDriver-0.1.66/robertcommondriver/system/iot/iot_bacnet_mstp.py
+-rw-rw-rw-   0        0        0   149923 2024-04-16 07:23:38.000000 RobertCommonDriver-0.1.66/robertcommondriver/system/iot/iot_iec104.py
+-rw-rw-rw-   0        0        0    34927 2024-03-11 07:51:49.000000 RobertCommonDriver-0.1.66/robertcommondriver/system/iot/iot_modbus.py
+-rw-rw-rw-   0        0        0    18508 2024-01-18 08:31:41.000000 RobertCommonDriver-0.1.66/robertcommondriver/system/iot/iot_obix.py
+-rw-rw-rw-   0        0        0    79413 2024-05-15 09:13:17.000000 RobertCommonDriver-0.1.66/robertcommondriver/system/iot/iot_opcda.py
+-rw-rw-rw-   0        0        0    25840 2024-01-18 08:31:42.000000 RobertCommonDriver-0.1.66/robertcommondriver/system/iot/iot_opcua.py
+-rw-rw-rw-   0        0        0    43574 2024-01-18 08:31:42.000000 RobertCommonDriver-0.1.66/robertcommondriver/system/iot/iot_plc_ab.py
+-rw-rw-rw-   0        0        0    51831 2024-01-18 08:31:59.000000 RobertCommonDriver-0.1.66/robertcommondriver/system/iot/iot_plc_mitsubishi.py
+-rw-rw-rw-   0        0        0    41842 2024-01-18 08:32:12.000000 RobertCommonDriver-0.1.66/robertcommondriver/system/iot/iot_plc_omron.py
+-rw-rw-rw-   0        0        0    40158 2024-01-18 08:32:28.000000 RobertCommonDriver-0.1.66/robertcommondriver/system/iot/iot_plc_s7.py
+-rw-rw-rw-   0        0        0    46487 2024-01-18 08:32:45.000000 RobertCommonDriver-0.1.66/robertcommondriver/system/iot/iot_plc_siemens.py
+-rw-rw-rw-   0        0        0    13603 2024-03-11 07:18:37.000000 RobertCommonDriver-0.1.66/robertcommondriver/system/iot/iot_snmp.py
+-rw-rw-rw-   0        0        0       42 2024-05-16 02:10:14.374363 RobertCommonDriver-0.1.66/setup.cfg
+-rw-rw-rw-   0        0        0     3881 2024-05-15 09:23:51.000000 RobertCommonDriver-0.1.66/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 02:10:14.333559 RobertCommonDriver-0.1.66/tests/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonDriver-0.1.66/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 02:10:14.334559 RobertCommonDriver-0.1.66/tests/test_system/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:49:45.000000 RobertCommonDriver-0.1.66/tests/test_system/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 02:10:14.351968 RobertCommonDriver-0.1.66/tests/test_system/test_driver/
+-rw-rw-rw-   0        0        0        0 2021-08-06 06:51:11.000000 RobertCommonDriver-0.1.66/tests/test_system/test_driver/__init__.py
+-rw-rw-rw-   0        0        0     6948 2022-06-08 07:19:27.000000 RobertCommonDriver-0.1.66/tests/test_system/test_driver/test_bacnet.py
+-rw-rw-rw-   0        0        0     2038 2022-04-14 03:52:19.000000 RobertCommonDriver-0.1.66/tests/test_system/test_driver/test_bacnet1.py
+-rw-rw-rw-   0        0        0     3839 2022-08-02 01:50:14.000000 RobertCommonDriver-0.1.66/tests/test_system/test_driver/test_bacnetc.py
+-rw-rw-rw-   0        0        0     7865 2022-06-14 02:23:23.000000 RobertCommonDriver-0.1.66/tests/test_system/test_driver/test_bacnetv1.py
+-rw-rw-rw-   0        0        0     2008 2022-01-13 07:23:11.000000 RobertCommonDriver-0.1.66/tests/test_system/test_driver/test_modbus.py
+-rw-rw-rw-   0        0        0     9784 2022-07-21 02:42:09.000000 RobertCommonDriver-0.1.66/tests/test_system/test_driver/test_obix.py
+-rw-rw-rw-   0        0        0     5912 2022-07-07 09:34:12.000000 RobertCommonDriver-0.1.66/tests/test_system/test_driver/test_opcda.py
+-rw-rw-rw-   0        0        0     1686 2022-07-13 03:25:06.000000 RobertCommonDriver-0.1.66/tests/test_system/test_driver/test_opcua.py
+-rw-rw-rw-   0        0        0     2443 2022-08-12 05:55:46.000000 RobertCommonDriver-0.1.66/tests/test_system/test_driver/test_plcs7.py
+-rw-rw-rw-   0        0        0     1444 2022-07-12 05:58:47.000000 RobertCommonDriver-0.1.66/tests/test_system/test_driver/test_snmp.py
+drwxrwxrwx   0        0        0        0 2024-05-16 02:10:14.372358 RobertCommonDriver-0.1.66/tests/test_system/test_iot/
+-rw-rw-rw-   0        0        0        0 2022-06-15 07:28:45.000000 RobertCommonDriver-0.1.66/tests/test_system/test_iot/__init__.py
+-rw-rw-rw-   0        0        0     3227 2022-06-20 07:43:32.000000 RobertCommonDriver-0.1.66/tests/test_system/test_iot/test_bacnet1.py
+-rw-rw-rw-   0        0        0    25246 2023-10-08 12:56:05.000000 RobertCommonDriver-0.1.66/tests/test_system/test_iot/test_iot_bacnet.py
+-rw-rw-rw-   0        0        0    20074 2023-04-17 06:34:20.000000 RobertCommonDriver-0.1.66/tests/test_system/test_iot/test_iot_bacnet_mstp.py
+-rw-rw-rw-   0        0        0     5551 2024-04-17 07:22:03.000000 RobertCommonDriver-0.1.66/tests/test_system/test_iot/test_iot_iec104.py
+-rw-rw-rw-   0        0        0    17551 2024-05-14 09:10:21.000000 RobertCommonDriver-0.1.66/tests/test_system/test_iot/test_iot_modbus.py
+-rw-rw-rw-   0        0        0     4721 2024-01-12 07:59:56.000000 RobertCommonDriver-0.1.66/tests/test_system/test_iot/test_iot_obix.py
+-rw-rw-rw-   0        0        0     6315 2023-10-11 07:31:18.000000 RobertCommonDriver-0.1.66/tests/test_system/test_iot/test_iot_opcda.py
+-rw-rw-rw-   0        0        0     5102 2024-04-17 08:39:37.000000 RobertCommonDriver-0.1.66/tests/test_system/test_iot/test_iot_opcua.py
+-rw-rw-rw-   0        0        0     1374 2023-04-14 09:46:49.000000 RobertCommonDriver-0.1.66/tests/test_system/test_iot/test_iot_plc_ab.py
+-rw-rw-rw-   0        0        0     2510 2023-04-14 09:44:42.000000 RobertCommonDriver-0.1.66/tests/test_system/test_iot/test_iot_plc_mitsubishi.py
+-rw-rw-rw-   0        0        0     2836 2023-04-14 09:45:55.000000 RobertCommonDriver-0.1.66/tests/test_system/test_iot/test_iot_plc_omron.py
+-rw-rw-rw-   0        0        0    11822 2023-11-07 14:02:46.000000 RobertCommonDriver-0.1.66/tests/test_system/test_iot/test_iot_plc_s7.py
+-rw-rw-rw-   0        0        0     4145 2023-07-27 06:41:53.000000 RobertCommonDriver-0.1.66/tests/test_system/test_iot/test_iot_plc_siemens.py
+-rw-rw-rw-   0        0        0      350 2022-08-16 09:35:34.000000 RobertCommonDriver-0.1.66/tests/test_system/test_iot/test_iot_plc_simenses1.py
+-rw-rw-rw-   0        0        0     3470 2024-03-11 06:22:29.000000 RobertCommonDriver-0.1.66/tests/test_system/test_iot/test_iot_snmp.py
```

### Comparing `RobertCommonDriver-0.1.65/LICENSE` & `RobertCommonDriver-0.1.66/LICENSE`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.65/PKG-INFO` & `RobertCommonDriver-0.1.66/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobertCommonDriver
-Version: 0.1.65
+Version: 0.1.66
 Summary: Robert Common Driver Library
 Home-page: https://github.com/hun0423/RobertCommonDriver
 Author: Robert0423
 Author-email: 851010070@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `RobertCommonDriver-0.1.65/RobertCommonDriver.egg-info/PKG-INFO` & `RobertCommonDriver-0.1.66/RobertCommonDriver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobertCommonDriver
-Version: 0.1.65
+Version: 0.1.66
 Summary: Robert Common Driver Library
 Home-page: https://github.com/hun0423/RobertCommonDriver
 Author: Robert0423
 Author-email: 851010070@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `RobertCommonDriver-0.1.65/RobertCommonDriver.egg-info/SOURCES.txt` & `RobertCommonDriver-0.1.66/RobertCommonDriver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.65/robertcommondriver/system/driver/bacnet.py` & `RobertCommonDriver-0.1.66/robertcommondriver/system/driver/bacnet.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.65/robertcommondriver/system/driver/bacnetc.py` & `RobertCommonDriver-0.1.66/robertcommondriver/system/driver/bacnetc.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.65/robertcommondriver/system/driver/base.py` & `RobertCommonDriver-0.1.66/robertcommondriver/system/driver/base.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.65/robertcommondriver/system/driver/modbus.py` & `RobertCommonDriver-0.1.66/robertcommondriver/system/driver/modbus.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,15 +226,15 @@
                         self.modbus_client.set_timeout(self.modbus_time_out)
                     else:
                         modbus_com = modbus_info['port']  # com5 或/dev/tty0
                         if modbus_com.find('/dev/tty') == 0:
                             self.modbus_client = modbus_rtu.RtuMaster(Serial(port=modbus_com, baudrate=modbus_info['baudrate'], bytesize=modbus_info['bytesize'], parity=modbus_info['parity'], stopbits=modbus_info['stopbits'], xonxoff=modbus_info['xonxoff']))
                             self.modbus_client.set_timeout(self.modbus_time_out)
                         else:
-                            if modbus_com.starswith('com') is False:
+                            if modbus_com.startswith('com') is False:
                                 modbus_com = f"com{modbus_com}"
                             self.modbus_client = modbus_rtu.RtuMaster(Serial(port=modbus_com, baudrate=modbus_info['baudrate'], bytesize=modbus_info['bytesize'], parity=modbus_info['parity'], stopbits=modbus_info['stopbits'], xonxoff=modbus_info['xonxoff']))
 
                         self.modbus_client.set_timeout(self.modbus_time_out)
                         self.modbus_client.set_verbose(True)
         except Exception as e:
             raise e
```

### Comparing `RobertCommonDriver-0.1.65/robertcommondriver/system/driver/obix.py` & `RobertCommonDriver-0.1.66/robertcommondriver/system/driver/obix.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.65/robertcommondriver/system/driver/opcda.py` & `RobertCommonDriver-0.1.66/robertcommondriver/system/driver/opcda.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.65/robertcommondriver/system/driver/opcda_openopc.py` & `RobertCommonDriver-0.1.66/robertcommondriver/system/driver/opcda_openopc.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.65/robertcommondriver/system/driver/opcua.py` & `RobertCommonDriver-0.1.66/robertcommondriver/system/driver/opcua.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.65/robertcommondriver/system/driver/plcs7.py` & `RobertCommonDriver-0.1.66/robertcommondriver/system/driver/plcs7.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.65/robertcommondriver/system/driver/snmp.py` & `RobertCommonDriver-0.1.66/robertcommondriver/system/driver/snmp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.65/robertcommondriver/system/iot/base.py` & `RobertCommonDriver-0.1.66/robertcommondriver/system/iot/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -557,20 +557,21 @@
             return results_dict if dict_result else results_list
 
         def cost(self):
             return self.pool_cost
 
     class IECSocketClient:
 
-        def __init__(self, host: str, port: int, timeout: float, callbacks: Optional[dict] = None):
+        def __init__(self, host: str, port: int, timeout: float, rec_timeout: Optional[float] = None, callbacks: Optional[dict] = None):
             self.valid = True
             self.host = host
             self.port = port
             self.sock = None
             self.timeout = timeout
+            self.rec_timeout = None
             self.lock = Lock()
             self.callbacks = {} if callbacks is None else callbacks
             self.connect()
             IOTBaseCommon.function_thread(self.receive, True, f"iecclient({host}:{port})").start()
             self.handle_connect()
 
         def __str__(self):
@@ -584,15 +585,15 @@
 
         def connect(self):
             with self.lock:
                 self.sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
                 self.sock.settimeout(self.timeout)  # 设置连接超时
                 self.sock.setsockopt(socket.SOL_SOCKET, socket.SO_LINGER, pack('ii', 1, 0))    # 避免TIME_WAIT
                 self.sock.connect((self.host, self.port))
-                self.sock.settimeout(None)
+                self.sock.settimeout(self.rec_timeout)
 
         def close(self):
             self.valid = False
             with self.lock:
                 try:
                     if self.sock:
                         self.sock.close()
@@ -625,19 +626,25 @@
                 return None
             return data
 
         def receive(self):
             try:
                 while self.valid is True:
                     start_bytes = self.recv_bytes(2)
-                    if isinstance(start_bytes, bytes) and len(start_bytes) == 2 and start_bytes[0] == 0x68:
-                        datas = self.recv_bytes(start_bytes[1])
-                        if isinstance(datas, bytes) and len(datas) >= 0:
-                            if 'handle_data' in self.callbacks.keys():
-                                self.callbacks['handle_data'](self, start_bytes + datas)
+                    if isinstance(start_bytes, bytes) and len(start_bytes) == 2:
+                        length = 0
+                        if start_bytes[0] == 0x68:
+                            length = start_bytes[1]
+                        elif start_bytes[1] == 0x68:
+                            length = self.recv_bytes(1)[0]
+                        if length > 0:
+                            datas = self.recv_bytes(length)
+                            if isinstance(datas, bytes) and len(datas) >= 0:
+                                if 'handle_data' in self.callbacks.keys():
+                                    self.callbacks['handle_data'](self, start_bytes + datas)
             except socket.timeout as e:
                 pass
             except IOTBaseCommon.NormalException as e:
                 logging.error(f"normal error({e.__str__()})")
             except IOTBaseCommon.CloseException as e:
                 self.handle_close(e.__str__())
             except (ConnectionResetError, BaseException, Exception, socket.error, OSError) as e:
@@ -1524,14 +1531,18 @@
     @abstractmethod
     def read(self, **kwargs):
         raise NotImplementedError()
 
     def write(self, **kwargs):
         raise NotImplementedError()
 
+    def copy_new_self(self):
+        """复制自身"""
+        return self
+
     def update(self, **kwargs):
         self.kwargs.update(kwargs)
         self.configure(**kwargs)
 
     def configure(self, **kwargs):
         if 'configs' in kwargs.keys():
             self.configs = kwargs.get('configs')
@@ -1644,24 +1655,27 @@
         return self.debug_pos
 
     def clear_device(self, device_address: Optional[str]):
         if device_address in self.devices.keys():
             self.devices.pop(device_address)
 
     def update_device(self, device_address: Optional[str], address: Optional[Any] = None, **kwargs):
-        if device_address not in self.devices.keys():
-            self.devices[device_address] = {}
-
-        values = kwargs.get('values')
-        if isinstance(values, dict) and len(values) > 0:
-            self.devices[device_address].update(values)
-        elif address is not None:
-            if address not in self.devices[device_address].keys():
-                self.devices[device_address][address] = {}
-            self.devices[device_address][address].update(**kwargs)
+        try:
+            if device_address not in self.devices.keys():
+                self.devices[device_address] = {}
+
+            values = kwargs.get('values')
+            if isinstance(values, dict) and len(values) > 0:
+                self.devices[device_address].update(values)
+            elif address is not None:
+                if address not in self.devices[device_address].keys():
+                    self.devices[device_address][address] = {}
+                self.devices[device_address][address].update(**kwargs)
+        except:
+            pass
 
     def get_device_property(self, device_address: Optional[str], address: Optional[Any], property: Optional[Union[str, list]] = None):
         device_property = self.devices.get(device_address, {}).get(address, {})
         if property is None:
             return device_property
         elif isinstance(property, str):
             return device_property.get(property)
```

### Comparing `RobertCommonDriver-0.1.65/robertcommondriver/system/iot/iot_bacnet.py` & `RobertCommonDriver-0.1.66/robertcommondriver/system/iot/iot_bacnet.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.65/robertcommondriver/system/iot/iot_bacnet_mstp.py` & `RobertCommonDriver-0.1.66/robertcommondriver/system/iot/iot_bacnet_mstp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.65/robertcommondriver/system/iot/iot_iec104.py` & `RobertCommonDriver-0.1.66/robertcommondriver/system/iot/iot_iec104.py`

 * *Files 6% similar despite different names*

```diff
@@ -2414,15 +2414,15 @@
         C_DC_TA_1 = 59,  # 带时标CP56Time2a的双命令
         C_RC_TA_1 = 60,  # 带时标CP56Time2a的步调节命令
         C_SE_TA_1 = 61,  # 带时标CP56Time2a的设定值命令，归一化值
         C_SE_TB_1 = 62,  # 带时标CP56Time2a的设定值命令，标度化值
         C_SE_TC_1 = 63,  # 带时标CP56Time2a的设定值命令，短浮点数
         C_BO_TA_1 = 64,  # 带时标CP56Time2a的32比特串
         # 监视方向的系统信息
-        # M_EI_NA_1 = 70,  # 初始化结束
+        M_EI_NA_1 = 70,  # 初始化结束
         # 控制方向的系统信息
         C_IC_NA_1 = 100,  # 总召唤命令
         C_CI_NA_1 = 101,  # 电能脉冲召唤命令
         C_RD_NA_1 = 102,  # 读命令
         C_CS_NA_1 = 103,  # 时钟同步命令
         # C_TS_NA_1 = 103,  # 测试命令
         # C_RP_NA_1 = 105,  # 复位进程命令
@@ -2982,14 +2982,20 @@
     ASDU_C_BO_TA_1 = Struct(
         "ASDU_C_BO_TA_1",
         EmbeddedBitStruct(BitField("address", 24, swapped=True)),  # 信息对象地址
         ULInt32("value"),
         cp56time2a,
     )
 
+    # 70 M_EI_NA_1 初始化结束
+    ASDU_M_EI_NA_1 = Struct(
+        "ASDU_M_EI_NA_1",
+        EmbeddedBitStruct(BitField("address", 24, swapped=True)),  # 信息对象地址
+    )
+
     # 100 总召唤命令
     ASDU_C_IC_NA_1 = Struct(
         "ASDU_C_IC_NA_1",
         EmbeddedBitStruct(BitField("address", 24, swapped=True)),  # 信息对象地址
         # ULInt8("QOI"),  # 0 未用 20 站召唤（总招） 21~36 第1~16组召唤
         Magic(b"\x14"),
     )
@@ -3455,34 +3461,248 @@
             values = {}
             if not isinstance(self.payload, NoPayload):
                 values[self.payload.name] = self.payload.info()
                 if not isinstance(self.payload.payload, NoPayload):
                     values[self.payload.payload.name] = self.payload.payload.info()
             return values
 
+    class IEC104:
+        """IEC连接参数"""
+
+        T0 = 10  # 30s 主站连接从站超时 - 连接建立超时
+        T1 = 15  # 15s 发送U帧测试帧到收到测试确认帧的时间 如果超时关闭连接(发送I帧或U帧后，等待对方应答，等待超过T1则重启链路) - 发送或测试超时
+        T2 = 10  # 10s 从站主动上报数据（突发）到收到S帧确认帧的时间  从站相应召唤到收到S帧确认帧的时间(接收到I帧后等待T2时间，然后发送对I帧的应答) - 无数据报文超时  从站发送完所有I帧，但未收到S帧
+        T3 = 20  # 20s 没有任何数据时的超时时间，超时发送U帧测试帧 其中 t3>t1>t2(T3时间内未收到任何报文，发送TESTFR) - 长期空闲超时
+        K = 12  # 从站发送12个AODU报文就必须收到确认帧，否则关闭数据传送，用于从站(发送方在有k个I格式报文未得到对方的确认时，将停止数据传送)
+        W = 8  # 主站收到8个APDU就必须回复一个S帧的确认帧，用于主站(接收方最迟在接收了w个I格式报文后应发出认可) w不能超过k的2/3
+
+        def __init__(self, host: str, port: int,  t0: Optional[float] = 10, t1: Optional[float] = 15, t2: Optional[float] = 10, t3: Optional[float] = 20, k: Optional[int] = 12, w: Optional[int] = 8, **kwargs):
+            self.T0 = t0 if t0 is not None else self.T0
+            self.T1 = t1 if t1 is not None else self.T1
+            self.T2 = t2 if t2 is not None else self.T2
+            self.T3 = t3 if t3 is not None else self.T3
+            self.K = k if k is not None else self.K
+            self.W = w if w is not None else self.W
+            self.HOST = host
+            self.PORT = port
+            self.PZ = kwargs.get('pz', 0)     # 总召间隔时间
+            self.PD = kwargs.get('pd', 0)     # 电度间隔
+
+            self.is_connected = False   # 连接状态
+            self.client = None      # TCP连接
+            self.last_frame_received_time = None  # 最后收到数据时间
+            self.last_frame_received_i_time = None  # 最后收到I帧数据时间
+            self.last_frame_send_time = None  # 最后发送数据时间
+            self.last_frame_send_u_time = None      # 最后发送U帧时间 需要确认 否则认为超时
+            self.last_frame_send_s_time = None      # 最后发送S帧时间
+            self.last_frame_send_z_time = None      # 最后发送总召时间
+            self.last_frame_send_d_time = None      # 最后发送电度召唤时间
+
+            self.event_for_startdt_con = 0      # 等待启动命令事件
+            self.event_for_zongzhao = 0         # 等待总召结束事件 0:send 1: config 2 terminal
+            self.event_for_diandu = 0           # 等待电度结束事件
+
+            self.rsn_i = 0    # 接收到的I帧 用于判断是否发送S帧
+            self.ssn = 0        # 最新发送序列号
+            self.rsn = 0        # 最新收到的接收序列号
+            self.logging_call = None
+
+        def __str__(self):
+            return f"{self.HOST}:{self.PORT}"
+
+        def __del__(self):
+            self.exit()
+
+        def exit(self):
+            self.set_is_connected(False)
+
+        def set_logging(self, logging_call):
+            self.logging_call = logging_call
+
+        def logging(self, content: str):
+            if self.logging_call:
+                self.logging_call(content=content)
+
+        def info(self, **kwargs) -> dict:
+            return {'ssn': self.ssn, 'rsn_i': self.rsn_i, 'rsn': self.rsn, 'last_frame_received_time': self.last_frame_received_time, 'last_frame_received_i_time': self.last_frame_received_i_time, 'last_frame_send_time': self.last_frame_send_time, 'last_frame_send_u_time': self.last_frame_send_u_time, 'last_frame_send_s_time': self.last_frame_send_s_time, 'last_frame_send_z_time': self.last_frame_send_z_time, 'last_frame_send_d_time': self.last_frame_send_d_time, 'is_connected': self.check_is_connected()}
+
+        def connect(self, callbacks: Optional[dict] = None):
+            client = IOTBaseCommon.IECSocketClient(self.HOST, self.PORT, self.T0, self.T3, callbacks=callbacks)
+            self.set_is_connected(True, client)
+
+        def set_is_connected(self, is_connected, client: Optional[Any] = None):
+            """设置连接状态"""
+            self.is_connected = is_connected
+            if is_connected is True:
+                self.client = client if client is not None else self.client
+            else:
+                try:
+                    if self.client is not None:
+                        self.client.exit()
+                except:
+                    pass
+                finally:
+                    self.client = None
+
+        def check_is_connected(self) -> bool:
+            """获取连接状态"""
+            return self.is_connected and self.client and self.client.check_invalid()
+
+        def parse(self, datas: bytes) -> tuple:
+            """初步解析"""
+            self.last_frame_received_time = IOTBaseCommon.get_datetime()
+
+            type, options = '', {}
+            if datas[2] & 1 == 0 and len(datas) >= 12:  # I-Frame
+                self.rsn_i += 1
+                self.last_frame_received_i_time = IOTBaseCommon.get_datetime()
+                self.rsn = self.inc_counter((datas[3] << 7) | ((datas[2] & 0xFE) >> 1))
+                options['rsn'] = self.rsn
+                options['type_id'] = datas[6]  # 类型(1)
+                options['cause_id'] = datas[8] & 0x3F  # 原因
+                type = 'I'
+                if options['type_id'] == 100:  # 总召
+                    if options['cause_id'] == 7:  # 总召确认
+                        self.event_for_zongzhao = 1
+                    elif options['cause_id'] == 10:  # 总召结束
+                        self.event_for_zongzhao = 2
+                elif options['type_id'] == 101:  # 电能脉冲召唤命令
+                    if options['cause_id'] == 7:  # 电能确认
+                        self.event_for_diandu = 1
+                    elif options['cause_id'] == 10:  # 电能结束
+                        self.event_for_diandu = 2
+                elif options['type_id'] == 103:  # 时钟同步
+                    pass
+            elif datas[2] & 3 == 1:  # S-Frame
+                type = 'S'
+            elif datas[2] & 3 == 3:  # U-Frame
+                type = 'U'
+                options['u_type'] = (datas[2] & 0xfc) >> 2
+                if options['u_type'] == 0x02:  # U帧激活确认 发送总召命令
+                    self.last_frame_send_u_time = None
+                    self.event_for_startdt_con = 1
+                elif options['u_type'] == 0x08:  # U帧结束确认
+                    self.set_is_connected(False)
+                elif options['u_type'] == 0x10:  # U帧测试确认
+                    self.send_u_frame(0x20)
+                elif options['u_type'] == 0x20:  # U帧测试回复
+                    self.last_frame_send_u_time = None
+            return type, options
+
+        def send_frame(self, datas) -> bool:
+            """发送数据"""
+            if self.check_is_connected():
+                self.client.send(datas)
+                self.last_frame_send_time = IOTBaseCommon.get_datetime()
+                return True
+            return False
+
+        def send_i_frame(self, type_id: int, cause_id: int) -> str:
+            """发送I帧"""
+            datas = None
+            if type_id == 100:  # 总召
+                pkt = IOTIEC104.APDU()
+                pkt /= IOTIEC104.APCI(ApduLen=14, Type=0x00, Tx=self.ssn, Rx=self.rsn)
+                pkt /= IOTIEC104.ASDU(Type=100, SQ=0, Cause=6, Num=1, Test=0, OA=0, Addr=1, IOA=[IECData.IOAS[100](IOA=0, QOI=0x14)])
+                datas = pkt.build()
+            elif type_id == 101:  # 电能脉冲召唤
+                pkt = IOTIEC104.APDU()
+                pkt /= IOTIEC104.APCI(ApduLen=14, Type=0x00, Tx=self.ssn, Rx=self.rsn)
+                pkt /= IOTIEC104.ASDU(Type=101, SQ=0, Cause=6, Num=1, Test=0, OA=0, Addr=1, IOA=[IECData.IOAS[101](IOA=0, QCC=0x0)])
+                datas = pkt.build()
+
+            content = ''
+            if isinstance(datas, bytes) and len(datas) > 0 and self.send_frame(datas) is True:
+                self.ssn = self.inc_counter(self.ssn)
+                if type_id == 100:
+                    self.last_frame_send_z_time = IOTBaseCommon.get_datetime()
+                    self.event_for_zongzhao = 0
+                elif type_id == 101:
+                    self.last_frame_send_d_time = IOTBaseCommon.get_datetime()
+                    self.event_for_diandu = 0
+                content = f"iec104({self}) send I {self.ssn} ({IOTBaseCommon.DataTransform.format_bytes(datas)})"
+                self.logging(content)
+            return content
+
+        def send_s_frame(self) -> str:
+            """检查是否发送S确认帧"""
+            content = ''
+            if self.rsn_i >= self.W > 0:
+                datas = (IOTIEC104.APDU() / IOTIEC104.APCI(ApduLen=4, Type=0x01, Rx=self.rsn)).build()
+                if self.send_frame(datas) is True:
+                    self.rsn_i = 0
+                    self.last_frame_send_s_time = IOTBaseCommon.get_datetime()
+                    content = f"iec104({self}) send S ({IOTBaseCommon.DataTransform.format_bytes(datas)})"
+                    self.logging(content)
+            return content
+
+        def send_u_frame(self, utype: int) -> str:
+            """发送U帧"""
+            content = ''
+            datas = (IOTIEC104.APDU() / IOTIEC104.APCI(ApduLen=4, Type=0x03, UType=utype)).build()
+            if self.send_frame(datas) is True:
+                if utype in [0x01, 0x10]:
+                    self.last_frame_send_u_time = IOTBaseCommon.get_datetime()
+                content = f"iec104({self}) send U ({IOTBaseCommon.DataTransform.format_bytes(datas)})"
+                self.logging(content)
+            return content
+
+        def inc_counter(self, value):
+            return value + 1 if value < 32767 else 0
+
+        def auto_cmd(self):
+            """自动命令"""
+            if self.check_is_connected() is True:
+
+                if self.event_for_startdt_con == 0:   # 尚未收到激活命令
+                    # T0 没收到激活命令 结束
+                    if isinstance(self.last_frame_send_u_time, datetime) and (IOTBaseCommon.get_datetime() - self.last_frame_send_u_time).total_seconds() > self.T0 > 0:
+                        self.set_is_connected(False)
+                        return
+                else:
+                    # T1 15s 未收到U帧回复(发送I帧或U帧后，等待对方应答，等待超过T1则重启链路)
+                    if self.check_is_connected() is True and isinstance(self.last_frame_send_u_time, datetime) and 0 < self.T1 < (IOTBaseCommon.get_datetime() - self.last_frame_send_u_time).total_seconds():
+                        self.set_is_connected(False)
+                        return
+
+                    # T2 10s 从站主动上报数据（突发）到收到S帧确认帧的时间  从站相应召唤到收到S帧确认帧的时间(接收到I帧后等待T2时间，然后发送对I帧的应答) - 无数据报文超时  从站发送完所有I帧，但未收到S帧
+                    if self.check_is_connected() is True and isinstance(self.last_frame_received_i_time, datetime) and 0 < self.T2 < (IOTBaseCommon.get_datetime() - self.last_frame_received_i_time).total_seconds() and (self.last_frame_send_s_time is None or self.last_frame_send_s_time < self.last_frame_received_i_time):
+                        self.send_s_frame()
+
+                    # T3 20s 有任何数据时的超时时间，超时发送U帧测试帧 t3>t1>t2
+                    if self.check_is_connected() is True and 0 < self.T3 < (IOTBaseCommon.get_datetime() - max(self.last_frame_received_time, self.last_frame_send_time)).total_seconds():
+                        self.send_u_frame(0x10)
+                        return
+
+                    # 总召
+                    if self.event_for_zongzhao != 2 and isinstance(self.last_frame_send_z_time, datetime) and (IOTBaseCommon.get_datetime() - self.last_frame_send_z_time).total_seconds() < self.T3:  # 总召命令未超时 不允许发送新总召或者电能命令
+                        return
+
+                    # 电度
+                    if self.event_for_diandu != 2 and isinstance(self.last_frame_send_d_time, datetime) and (IOTBaseCommon.get_datetime() - self.last_frame_send_d_time).total_seconds() < self.T3:  # 电能命令未超时 不允许发送新总召或者电能命令
+                        return
+
+                    # 优先总召
+                    if self.check_is_connected() is True and (self.last_frame_send_z_time is None or 0 < self.PZ < (IOTBaseCommon.get_datetime() - self.last_frame_send_z_time).total_seconds()):
+                        self.send_i_frame(type_id=100, cause_id=6)
+
+                    # 电度
+                    if self.check_is_connected() is True and (self.last_frame_send_d_time is None or 0 < self.PZ < (IOTBaseCommon.get_datetime() - self.last_frame_send_d_time).total_seconds()):
+                        self.send_i_frame(type_id=101, cause_id=6)
+
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.lock_client = Lock()
         self.reinit()
 
     def reinit(self):
-        self.client = None
-        self.is_connected = False
-        self.ole_zongzhao = IOTBaseCommon.get_datetime() - timedelta(days=1)   # 总召时间
-        self.ole_dianneng = IOTBaseCommon.get_datetime() - timedelta(days=1)    # 电能召唤时间
-        self.ole_recv = IOTBaseCommon.get_datetime() - timedelta(days=1)  # 收到回复数据时间
-        self.ole_send = IOTBaseCommon.get_datetime() - timedelta(days=1)  # 命令发送时间
-
-        self.event_zongzhao = 0   # 总召事件激活 0:send 1: config 2 terminal
-        self.event_dianneng = 0  # 电能
+        self.iec104 = self.IEC104(self.configs.get('host'), self.configs.get('port'), t0=self.configs.get('timeout', 10), w=self.configs.get('s_interval', 8), pz=self.configs.get('zongzhao_interval', 8), pd=self.configs.get('dianneng_interval', 8))
+        self.iec104.set_logging(self.logging)
         self.threads = {}   # 线程
         self.values = {}
-        self.send_count = 0
-        self.recv_count = 0
-        self.recv_i_count = 0
         self.thread_exit = False
         self.cache_queue = deque(maxlen=2000)   # Queue()
 
     def exit(self):
         self._release_client()
 
     @classmethod
@@ -3563,151 +3783,102 @@
             results[name] = result
             if result[0] is not True:
                 self.logging(content=f"write value({name}) fail({result[1]})", level='ERROR', source=name, pos=self.stack_pos)
         return results
 
     def ping(self, **kwargs) -> bool:
         self.update_info(used=IOTBaseCommon.get_datetime_str())
-        return self.is_connected
+        return self.iec104 and self.iec104.check_is_connected()
 
     def _read(self, read_items: list):
         try:
             if len(read_items) > 0 and self._get_client():
                 pass
         except Exception as e:
             for read_item in read_items:
                 self.update_device(f"{self.configs.get('host')}:{self.configs.get('port')}", read_item, **self.gen_read_write_result(False, e.__str__()))
 
     def _write(self, type: int, address: int, value):
         raise NotImplementedError()
 
     def _release_client(self):
         with self.lock_client:
-            self.is_connected = False
             self.thread_exit = True
+            if self.iec104:
+                self.iec104.set_is_connected(False)
             try:
                 for name, thread in self.threads.items():
                     thread.join(5)
                     IOTBaseCommon.stop_thread(thread)
-                if self.client:
-                    self.client.exit()
             except Exception as e:
                 pass
             finally:
                 self.reinit()
 
     def _get_client(self):
         try:
-            if self.client is not None and (self.is_connected is False or self.client.check_invalid() is False):
+            if self.iec104.check_is_connected() is False:
                 self._release_client()
 
-            if self.client is None:
-                self.clear_device(f"{self.configs.get('host')}:{self.configs.get('port')}")
-                client = IOTBaseCommon.IECSocketClient(self.configs.get('host'), self.configs.get('port'), self.configs.get('timeout', 4), callbacks={'handle_data': self.handle_data, 'handle_connect': self.handle_connect, 'handle_close': self.handle_close, 'handle_error': self.handle_error})
-                self.client = client
-            return self.client
+                self.iec104.connect(callbacks={'handle_connect': self.handle_connect, 'handle_close': self.handle_close, 'handle_error': self.handle_error, 'handle_data': self.handle_data})
+
+            if self.iec104.check_is_connected() is False:
+                raise Exception(f"Unconnected")
         except Exception as e:
             raise Exception(f"connect fail({e.__str__()})")
+        return self.iec104.check_is_connected()
 
     def handle_connect(self, client):
         # 连接成功 U帧启动报文
-        self.is_connected = True
-        self._send_frame(client, 'U', utype=0x01)
+        self.iec104.set_is_connected(True, client)
+        self.create_auo_cmd_frame_thread()
 
     # 关闭事件
     def handle_close(self, client, reason: str):
-        self.is_connected = False
+        self.iec104.set_is_connected(False)
         self.logging(content=f"iec104({client}) close({reason})", level='ERROR', pos=self.stack_pos)
 
     def handle_error(self, client, msg: str):
-        self.is_connected = False
+        self.iec104.set_is_connected(False)
         self.logging(content=f"iec104({client}) error({msg})", level='ERROR', pos=self.stack_pos)
 
-    def inc_send_recv(self, current_send: Optional[int] = None, current_recv: Optional[int] = None, clear_i: Optional[bool] = False):
-        if isinstance(current_recv, int):
-            recv_count = current_recv if current_recv is not None else self.recv_count
-            self.recv_count = recv_count + 1 if recv_count < 32767 else 0
-            self.recv_i_count = self.recv_i_count + 1 if self.recv_i_count < 32767 else 0
-
-        if isinstance(current_send, int):
-            self.send_count = current_send + 1 if current_send < 32767 else 0
-
-        if clear_i is True:
-            self.recv_i_count = 0
-
     def set_data_cache(self, datas: tuple):
         self.cache_queue.append(datas)
 
     def analyze_data_cache_thread(self):
         while self.thread_exit is False:
-            while len(self.cache_queue) > 0:
+            while self.thread_exit is False and len(self.cache_queue) > 0:
                 self.analyze_data_cache(self.cache_queue.popleft(), True)
                 self.delay(0.001)
             self.delay(0.1)
 
     def analyze_data_cache(self, caches: Union[List, tuple], is_frame_parse: bool = True):
         if isinstance(caches, tuple) and len(caches) >= 2:
-            send, datas = caches
+            send, datas, options = caches
             try:
                 if isinstance(datas, bytes) and len(datas) > 0:
                     if isinstance(send, str) and len(send) > 0:
                         self.logging(content=f"{send} cache: {len(self.cache_queue)}", pos=self.stack_pos)
+                    self.logging(content=f"iec104({self.iec104}) recv I {options.get('rsn')} {self._get_frame_name(options.get('type_id'), options.get('cause_id'))}", pos=self.stack_pos)
                     if is_frame_parse is True:
                         frame = IECFrame.iec_104.parse(datas)   # 解析速度快
                         self.update_device(f"{self.configs.get('host')}:{self.configs.get('port')}", values={f"{frame.ASDU.TYP}_{v.address}" if frame.ASDU.sq == 0 else f"{frame.ASDU.TYP}_{frame.ASDU.StartAddress + i}": self.gen_read_write_result(True, v.value) for i, v in enumerate(frame.ASDU.data) if hasattr(v, 'value')})
                     else:
                         self.update_device(f"{self.configs.get('host')}:{self.configs.get('port')}", values={k: self.gen_read_write_result(True, v) for k, v in IOTIEC104.ASDU(datas[6:]).values().items()})
             except (Exception, BaseException) as e:
-                self.logging(content=f"iec104({self.client}) analyze data fail({e.__str__()}) {len(datas)}[{self.format_bytes(datas)}]", level='ERROR', pos=self.stack_pos)
+                self.logging(content=f"iec104({self.iec104}) analyze data fail({e.__str__()}) {len(datas)}[{self.format_bytes(datas)}]", level='ERROR', pos=self.stack_pos)
 
     def handle_data(self, client, datas: bytes):
         try:
             if isinstance(datas, bytes) and len(datas) > 2 and client is not None:
-                self.ole_recv = IOTBaseCommon.get_datetime()
-                if datas[2] & 1 == 0 and len(datas) >= 12:  # I帧
-                    rsn = (datas[3] << 7) | (datas[2] >> 1)
-                    type_id = datas[6]  # 类型(1)
-                    cause_id = datas[8] & 0x3F  # 原因
-                    self.inc_send_recv(current_recv=rsn)
-                    send = ''
-                    if self.recv_i_count >= self.configs.get('s_interval', 0) > 0:
-                        send = self._send_frame(client, 'S', disable_log=True)   # 发送S帧
-                    self.set_data_cache((send, datas))
-
-                    content=f"iec104({client}) recv I {rsn} {self._get_frame_name(type_id, cause_id)}"
-                    if type_id == 100:  # 总召
-                        if cause_id == 7:  # 总召确认
-                            self.event_zongzhao = 1
-                            self.logging(content=content, pos=self.stack_pos)
-                        elif cause_id == 10:  # 总召结束
-                            self.event_zongzhao = 2
-                            self.logging(content=content, pos=self.stack_pos)
-                    elif type_id == 101:  # 电能脉冲召唤命令
-                        if cause_id == 7:  # 电能确认
-                            self.event_dianneng = 1
-                            self.logging(content=content, pos=self.stack_pos)
-                        elif cause_id == 10:  # 电能结束
-                            self.event_dianneng = 2
-                            self.logging(content=content, pos=self.stack_pos)
-                    elif type_id == 103:  # 时钟同步
-                        pass
-
-                elif datas[2] & 3 == 1:  # S帧
-                    self.logging(content=f"iec104({client}) recv S: [{self.format_bytes(datas)}]", pos=self.stack_pos)
-                elif datas[2] & 3 == 3:
-                    u_type = (datas[2] & 0xfc) >> 2
-                    self.logging(content=f"iec104({client}) recv U: [{self.format_bytes(datas)}]", pos=self.stack_pos)
-                    if u_type == 0x02:  # U帧激活确认 发送总召命令
-                        self.create_auo_cmd_frame_thread()
-                    elif u_type == 0x08:     # U帧结束确认
-                        self.is_connected = False
-                    elif u_type == 0x10:     # U帧测试确认
-                        self._send_frame(client, 'U', utype=0x20)
-                    elif u_type == 0x20:     # U帧测试确认
-                        pass
+                type, options = self.iec104.parse(datas)
+                if type == 'I':  # I-Frame
+                    self.set_data_cache((self.iec104.send_s_frame(), datas, options))
+                else:  # S-Frame
+                    self.logging(content=f"iec104({client}) recv {type}: [{self.format_bytes(datas)}]", pos=self.stack_pos)
         except Exception as e:
             self.logging(content=f"iec104({client}) handle data fail({e.__str__()})({self.format_bytes(datas)})", level='ERROR', pos=self.stack_pos)
 
     def _get_value(self, name: str, device_address: str, address: str, type: int):
         try:
             [result, value] = self.get_device_property(device_address, f"{type}_{address}", [self.get_read_quality, self.get_read_result])
             if result is True:
@@ -3717,61 +3888,14 @@
                     raise Exception(f"value is none")
             else:
                 raise Exception(str(value))
         except Exception as e:
             self.update_results(name, False, e.__str__())
         return None
 
-    def _send_frame(self, client, acpi_type: str, **kwargs) -> str:
-        content = ''
-        with self.lock_client:
-            if self.is_connected is True and client is not None and client.check_invalid():
-                datas = None
-                if acpi_type == 'I':
-                    type_id = kwargs.get('type_id')
-                    cause_id = kwargs.get('cause_id')
-                    if type_id == 100:  # 总召
-                        pkt = IOTIEC104.APDU()
-                        pkt /= IOTIEC104.APCI(ApduLen=14, Type=0x00, Tx=self.send_count, Rx=self.recv_count)
-                        pkt /= IOTIEC104.ASDU(Type=100, SQ=0, Cause=6, Num=1, Test=0, OA=0, Addr=1, IOA=[IECData.IOAS[100](IOA=0, QOI=0x14)])
-                        datas = pkt.build()
-
-                        self.event_zongzhao = 0
-                    elif type_id == 101:  # 电能脉冲召唤
-                        pkt = IOTIEC104.APDU()
-                        pkt /= IOTIEC104.APCI(ApduLen=14, Type=0x00, Tx=self.send_count, Rx=self.recv_count)
-                        pkt /= IOTIEC104.ASDU(Type=101, SQ=0, Cause=6, Num=1, Test=0, OA=0, Addr=1, IOA=[IECData.IOAS[101](IOA=0, QCC=0x0)])
-                        datas = pkt.build()
-
-                        self.event_dianneng = 0
-
-                    content = f"iec104({client}) send I {self.send_count} {self._get_frame_name(type_id, cause_id)}: [{self.format_bytes(datas)}]"
-                elif acpi_type == 'U':
-                    datas = (IOTIEC104.APDU() / IOTIEC104.APCI(ApduLen=4, Type=0x03, UType=kwargs.get('utype', 0x10))).build()
-                    content=f"iec104({client}) send U ({self.format_bytes(datas)})"
-                elif acpi_type == 'S':
-                    datas = (IOTIEC104.APDU() / IOTIEC104.APCI(ApduLen=4, Type=0x01, Rx=self.recv_count)).build()
-                    content=f"iec104({client}) send S {self.recv_count}"
-
-                if kwargs.get('disable_log', False) is False:
-                    self.logging(content=content, pos=self.stack_pos)
-
-                client.send(datas)
-                now = IOTBaseCommon.get_datetime()
-                self.ole_send = now
-                if acpi_type == 'I':
-                    self.inc_send_recv(current_send=self.send_count)
-                    if type_id == 100:  # 总召
-                        self.ole_zongzhao = IOTBaseCommon.get_datetime()
-                    elif type_id == 101:  # 电能脉冲召唤
-                        self.ole_dianneng = IOTBaseCommon.get_datetime()
-                elif acpi_type == 'S':
-                    self.inc_send_recv(clear_i=True)
-        return content
-
     def _get_frame_name(self, type_id: int, cause_id: int) -> str:
         return f"{IECDefine.ASDU_TYPE.get(type_id)} {IECDefine.ASDU_CAUSE.get(cause_id)}"
 
     def create_auo_cmd_frame_thread(self):
         """启动命令线程"""
         thread_name = f"iecclient({self.configs.get('host')}:{self.configs.get('port')}) cmd"
         self.threads[thread_name] = IOTBaseCommon.function_thread(self.send_auo_cmd_frame_thread, True, thread_name)
@@ -3779,66 +3903,31 @@
         thread_name = f"iecclient({self.configs.get('host')}:{self.configs.get('port')}) analyze"
         self.threads[thread_name] = IOTBaseCommon.function_thread(self.analyze_data_cache_thread, True, thread_name)
         for name, thread in self.threads.items():
             thread.start()
 
     def send_auo_cmd_frame_thread(self):
         """命令线程"""
-        dianneng_interval = self.configs.get('dianneng_interval', 0)
-        dianneng_timeout = self.configs.get('dianneng_timeout', 30)
-        zongzhao_interval = self.configs.get('zongzhao_interval', 0)
-        zongzhao_timeout = self.configs.get('zongzhao_timeout', 30)
-        u_test_timeout = self.configs.get('u_test_timeout', 10)
-
-        # 首先发送总召命令
-        self._send_frame(self.client, 'I', type_id=100, cause_id=6)
-
-        while self.is_connected:
-            self.delay(1)
+        try:
+            self.iec104.send_u_frame(0x01)
+        except (Exception, BaseException) as e:
+            pass
 
+        while self.iec104 and self.iec104.check_is_connected() is True:
+            self.delay(0.5)
             try:
-                now = IOTBaseCommon.get_datetime()
-
-                if isinstance(u_test_timeout, int) and 0 < u_test_timeout <= (now - max(self.ole_recv, self.ole_send)).total_seconds():     # 超过一定时间没有下发报文或者装置没有上送任何报文 发送U帧测试帧
-                    self._send_frame(self.client, 'U', utype=0x10)
-                    continue
-
-                if isinstance(u_test_timeout, int) and 0 < u_test_timeout * 2 <= (now - self.ole_recv).total_seconds():         # 超过一定时间没有收到回复 认为掉线了
-                    self.is_connected = False
-                    continue
-
-                if isinstance(zongzhao_interval, int) and 0 < zongzhao_interval:    # 需要发送总召命令
-                    if self.event_zongzhao == 0:     # 未收到总召确认
-                        if (now - self.ole_zongzhao).total_seconds() <= u_test_timeout:         # 总召命令未超时 不允许发送新总召或者电能命令
-                            continue
-                    else:   # 收到总召确认
-                        if self.event_zongzhao == 1 and (now - self.ole_zongzhao).total_seconds() <= zongzhao_timeout:     # 总召尚未结束 且尚未超时
-                            continue
-
-                if isinstance(dianneng_interval, int) and 0 < dianneng_interval:    # 需要发送电度命令
-                    if self.event_dianneng == 0:     # 未收到电能确认
-                        if (now - self.ole_dianneng).total_seconds() <= u_test_timeout: # 电能命令未超时 不允许发送新总召或者电能命令
-                            continue
-                    else:   # 收到电能确认
-                        if self.event_dianneng == 1 and (now - self.ole_dianneng).total_seconds() <= dianneng_timeout:     # 电能尚未结束 且尚未超时
-                            continue
-
-                if isinstance(zongzhao_interval, int) and 0 < zongzhao_interval <= (now - self.ole_zongzhao).total_seconds():    # 优先总召
-                    self._send_frame(self.client, 'I', type_id=100, cause_id=6)
-                    continue
-
-                if isinstance(dianneng_interval, int) and 0 < dianneng_interval <= (now - self.ole_dianneng).total_seconds():   # 电能召唤
-                    self._send_frame(self.client, 'I', type_id=101, cause_id=6)  # 电能召唤
-                    continue
-
+                self.iec104.auto_cmd()
             except (Exception, BaseException) as e:
-                self.logging(content=f"iec104({self.client}) send data fail({e.__str__()})", level='ERROR', pos=self.stack_pos)
+                self.logging(content=f"iec104({self.iec104}) send data fail({e.__str__()})", level='ERROR', pos=self.stack_pos)
                 self.delay(2)
 
     def format_bytes(self, data: bytes) -> str:
         if isinstance(data, bytes):
             return ' '.join(["%02X" % x for x in data]).strip()
         return ''
 
     @property
     def stack_pos(self, pos: int = 900):
         return f"iot_iec104.py({pos})"
+
+    def info(self, **kwargs) -> dict:
+        return self.iec104.info() if self.iec104 else {}
```

### Comparing `RobertCommonDriver-0.1.65/robertcommondriver/system/iot/iot_modbus.py` & `RobertCommonDriver-0.1.66/robertcommondriver/system/iot/iot_modbus.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.65/robertcommondriver/system/iot/iot_obix.py` & `RobertCommonDriver-0.1.66/robertcommondriver/system/iot/iot_obix.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.65/robertcommondriver/system/iot/iot_opcda.py` & `RobertCommonDriver-0.1.66/robertcommondriver/system/iot/iot_opcda.py`

 * *Files 0% similar despite different names*

```diff
@@ -1785,7 +1785,11 @@
     def info(self, **kwargs):
         if self._get_client():
             return self.client.get_info()
 
     @property
     def stack_pos(self, pos: int = 900):
         return f"iot_opcda.py({pos})"
+
+    def copy_new_self(self):
+        """复制自身"""
+        return IOTOPCDA(**self.kwargs)
```

### Comparing `RobertCommonDriver-0.1.65/robertcommondriver/system/iot/iot_opcua.py` & `RobertCommonDriver-0.1.66/robertcommondriver/system/iot/iot_opcua.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.65/robertcommondriver/system/iot/iot_plc_ab.py` & `RobertCommonDriver-0.1.66/robertcommondriver/system/iot/iot_plc_ab.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.65/robertcommondriver/system/iot/iot_plc_mitsubishi.py` & `RobertCommonDriver-0.1.66/robertcommondriver/system/iot/iot_plc_mitsubishi.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.65/robertcommondriver/system/iot/iot_plc_omron.py` & `RobertCommonDriver-0.1.66/robertcommondriver/system/iot/iot_plc_omron.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.65/robertcommondriver/system/iot/iot_plc_s7.py` & `RobertCommonDriver-0.1.66/robertcommondriver/system/iot/iot_plc_s7.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.65/robertcommondriver/system/iot/iot_plc_siemens.py` & `RobertCommonDriver-0.1.66/robertcommondriver/system/iot/iot_plc_siemens.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.65/robertcommondriver/system/iot/iot_snmp.py` & `RobertCommonDriver-0.1.66/robertcommondriver/system/iot/iot_snmp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.65/setup.py` & `RobertCommonDriver-0.1.66/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 # Package meta-data.
 NAME = 'RobertCommonDriver'
 DESCRIPTION = 'Robert Common Driver Library'
 URL = 'https://github.com/hun0423/RobertCommonDriver'
 EMAIL = '851010070@qq.com'
 AUTHOR = 'Robert0423'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.65'
-DATE = '2024-03-11'
+VERSION = '0.1.66'
+DATE = '2024-05-15'
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
 
 # The rest you shouldn't have to touch too much :)
```

### Comparing `RobertCommonDriver-0.1.65/tests/test_system/test_driver/test_bacnet.py` & `RobertCommonDriver-0.1.66/tests/test_system/test_driver/test_bacnet.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.65/tests/test_system/test_driver/test_bacnet1.py` & `RobertCommonDriver-0.1.66/tests/test_system/test_driver/test_bacnet1.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.65/tests/test_system/test_driver/test_bacnetc.py` & `RobertCommonDriver-0.1.66/tests/test_system/test_driver/test_bacnetc.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.65/tests/test_system/test_driver/test_bacnetv1.py` & `RobertCommonDriver-0.1.66/tests/test_system/test_driver/test_bacnetv1.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.65/tests/test_system/test_driver/test_modbus.py` & `RobertCommonDriver-0.1.66/tests/test_system/test_driver/test_modbus.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.65/tests/test_system/test_driver/test_obix.py` & `RobertCommonDriver-0.1.66/tests/test_system/test_driver/test_obix.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.65/tests/test_system/test_driver/test_opcda.py` & `RobertCommonDriver-0.1.66/tests/test_system/test_driver/test_opcda.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.65/tests/test_system/test_driver/test_opcua.py` & `RobertCommonDriver-0.1.66/tests/test_system/test_driver/test_opcua.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.65/tests/test_system/test_driver/test_plcs7.py` & `RobertCommonDriver-0.1.66/tests/test_system/test_driver/test_plcs7.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.65/tests/test_system/test_driver/test_snmp.py` & `RobertCommonDriver-0.1.66/tests/test_system/test_driver/test_snmp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.65/tests/test_system/test_iot/test_bacnet1.py` & `RobertCommonDriver-0.1.66/tests/test_system/test_iot/test_bacnet1.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.65/tests/test_system/test_iot/test_iot_bacnet.py` & `RobertCommonDriver-0.1.66/tests/test_system/test_iot/test_iot_bacnet.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.65/tests/test_system/test_iot/test_iot_bacnet_mstp.py` & `RobertCommonDriver-0.1.66/tests/test_system/test_iot/test_iot_bacnet_mstp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.65/tests/test_system/test_iot/test_iot_iec104.py` & `RobertCommonDriver-0.1.66/tests/test_system/test_iot/test_iot_iec104.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,26 +85,26 @@
     print(IOTIEC104().format_bytes(pkt.build()))
 
     info = IOTIEC104.APDU(bytes.fromhex('68 1A 0E 00 00 00 0D 02 01 00 01 00 01 40 00 A4 70 92 42 00 06 40 00 88 1D 12 41 00')).info()
     print(info)
 
 
 def test_dianneng():
-    dict_config = {'host': '127.0.0.1', 'port': 2404, 'timeout': 5, 'zongzhao_interval': 0, 'zongzhao_timeout': 30, 'dianneng_interval': 20, 'dianneng_timeout': 10, 'u_test_timeout': 10,  's_interval': 1}
+    dict_config = {'host': '127.0.0.1', 'port': 2404, 'timeout': 5, 'zongzhao_interval': 0, 'zongzhao_timeout': 30, 'dianneng_interval': 20, 'dianneng_timeout': 10, 'u_test_timeout': 10,  's_interval': 4}
     dict_point = {}
-    dict_point['iec1'] = {'point_writable': True, 'point_name': 'iec1', 'point_type': 1, 'point_address': 100, 'point_scale': '1'}
-    dict_point['iec2'] = {'point_writable': True, 'point_name': 'iec2', 'point_type': 13, 'point_address': 600, 'point_scale': '1'}
-    dict_point['iec3'] = {'point_writable': True, 'point_name': 'iec3', 'point_type': 15, 'point_address': 25633, 'point_scale': '1'}   # 37515
-    dict_point['iec4'] = {'point_writable': True, 'point_name': 'iec4', 'point_type': 15, 'point_address': 25697, 'point_scale': '1'}   # 500315
+    dict_point['iec1'] = {'point_writable': True, 'point_name': 'iec1', 'point_type': 13, 'point_address': 2, 'point_scale': '1'}
+    dict_point['iec2'] = {'point_writable': True, 'point_name': 'iec2', 'point_type': 13, 'point_address': 16385, 'point_scale': '1'}
+    dict_point['iec3'] = {'point_writable': True, 'point_name': 'iec3', 'point_type': 1, 'point_address': 1176, 'point_scale': '1'}   # 37515
+    dict_point['iec4'] = {'point_writable': True, 'point_name': 'iec4', 'point_type': 1, 'point_address': 1, 'point_scale': '1'}   # 500315
 
     client = IOTIEC104(configs = dict_config, points= dict_point)
     client.logging(call_logging=logging_print)
     while True:
         try:
             result = client.read(names=list(dict_point.keys()))
             print(result)
         except Exception as e:
             print(f"error: {e.__str__()}")
-        time.sleep(5)
+        time.sleep(10)
 
 
-test_parse1()
+test_dianneng()
```

### Comparing `RobertCommonDriver-0.1.65/tests/test_system/test_iot/test_iot_modbus.py` & `RobertCommonDriver-0.1.66/tests/test_system/test_iot/test_iot_modbus.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,17 +96,17 @@
         print(dict_result_scrap)
         time.sleep(2)
 
 
 def test_read3():
     #配置项
     dict_config = {
-                        'multi_read': 100,                             # 批量读取个数
-                        'cmd_interval': 0.3,                         # 命令间隔
-                        'time_out': 5                                 # 超时时间
+                        'multi_read': 100,
+                        'cmd_interval': 0.3,
+                        'time_out': 5
                     }
     #点表
     dict_point = {}
     dict_point['modbus_1'] = {'point_writable': True, 'point_name': 'modbus_1', 'point_device_address': '172.168.12.13/502',  'point_slave_id': 255, 'point_fun_code': 4, 'point_address': 28, 'point_data_type': 18, 'point_data_length': 2, 'point_data_order': 2, 'point_scale':'1'}
 
     modbus_driver = IOTModbus(configs=dict_config, points=dict_point)
     modbus_driver.logging(call_logging=logging_print)
```

### Comparing `RobertCommonDriver-0.1.65/tests/test_system/test_iot/test_iot_obix.py` & `RobertCommonDriver-0.1.66/tests/test_system/test_iot/test_iot_obix.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.65/tests/test_system/test_iot/test_iot_opcda.py` & `RobertCommonDriver-0.1.66/tests/test_system/test_iot/test_iot_opcda.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.65/tests/test_system/test_iot/test_iot_opcua.py` & `RobertCommonDriver-0.1.66/tests/test_system/test_iot/test_iot_opcua.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,31 +125,30 @@
         except Exception as e:
             print(e.__str__())
         time.sleep(5)
 
 
 def test_rw_list():
     dict_config = {
-        'endpoint': 'opc.tcp://localhost:4841',
+        'endpoint': 'opc.tcp://20.25.34.201:4840',
         'timeout': 4,
         'security': '',  #
         'auth': {},  #
         'subscript_add': 1000,
         'subscript_interval': 500,
     }
 
     dict_point = {}
-    dict_point['opcua1'] = {'point_writable': True, 'point_name': 'opcua1', 'point_node_id': 'ns=2;i=17', 'point_scale': '_in(v,1)'}
+    dict_point['opcua1'] = {'point_writable': True, 'point_name': 'opcua1', 'point_node_id': '20.25.34.201:4840', 'point_scale': '1'}
 
     client = IOTOPCUA(configs=dict_config, points=dict_point)
     client.logging(call_logging=logging_print)
     while True:
         try:
             result = client.read()
             print(result)
-            client.write(values={'opcua1': 1})
         except Exception as e:
             print(e.__str__())
         time.sleep(5)
 
 
 test_rw_list()
```

### Comparing `RobertCommonDriver-0.1.65/tests/test_system/test_iot/test_iot_plc_ab.py` & `RobertCommonDriver-0.1.66/tests/test_system/test_iot/test_iot_plc_ab.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.65/tests/test_system/test_iot/test_iot_plc_mitsubishi.py` & `RobertCommonDriver-0.1.66/tests/test_system/test_iot/test_iot_plc_mitsubishi.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.65/tests/test_system/test_iot/test_iot_plc_omron.py` & `RobertCommonDriver-0.1.66/tests/test_system/test_iot/test_iot_plc_omron.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.65/tests/test_system/test_iot/test_iot_plc_s7.py` & `RobertCommonDriver-0.1.66/tests/test_system/test_iot/test_iot_plc_s7.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.65/tests/test_system/test_iot/test_iot_plc_siemens.py` & `RobertCommonDriver-0.1.66/tests/test_system/test_iot/test_iot_plc_siemens.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.65/tests/test_system/test_iot/test_iot_snmp.py` & `RobertCommonDriver-0.1.66/tests/test_system/test_iot/test_iot_snmp.py`

 * *Files identical despite different names*

