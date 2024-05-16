# Comparing `tmp/nrobo-2024.40.2.tar.gz` & `tmp/nrobo-2024.40.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nrobo-2024.40.2.tar", last modified: Thu Apr 11 06:47:03 2024, max compression
+gzip compressed data, was "nrobo-2024.40.3.tar", last modified: Thu May 16 07:11:22 2024, max compression
```

## Comparing `nrobo-2024.40.2.tar` & `nrobo-2024.40.3.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.138254 nrobo-2024.40.2/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1079 2024-02-02 05:31:36.000000 nrobo-2024.40.2/LICENSE
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    18169 2024-04-11 06:47:03.137607 nrobo-2024.40.2/PKG-INFO
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    16531 2024-04-11 06:46:47.000000 nrobo-2024.40.2/README.rst
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.104027 nrobo-2024.40.2/nrobo/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     8702 2024-04-11 06:46:40.000000 nrobo-2024.40.2/nrobo/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.107403 nrobo-2024.40.2/nrobo/appium/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      716 2024-03-11 11:20:45.000000 nrobo-2024.40.2/nrobo/appium/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       72 2024-03-11 14:41:50.000000 nrobo-2024.40.2/nrobo/appium/android_capability.yaml
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       73 2024-03-11 12:05:03.000000 nrobo-2024.40.2/nrobo/appium/ios_capability.yaml
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.107720 nrobo-2024.40.2/nrobo/aws/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      475 2024-04-06 18:19:37.000000 nrobo-2024.40.2/nrobo/aws/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.110091 nrobo-2024.40.2/nrobo/browserConfigs/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      452 2024-02-29 19:11:43.000000 nrobo-2024.40.2/nrobo/browserConfigs/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       35 2024-02-29 19:12:02.000000 nrobo-2024.40.2/nrobo/browserConfigs/capability.yaml
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       17 2024-02-19 15:42:30.000000 nrobo-2024.40.2/nrobo/browserConfigs/chrome_config.txt
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       39 2024-02-29 19:12:02.000000 nrobo-2024.40.2/nrobo/browserConfigs/chrome_prefs.yaml
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       63 2024-02-29 19:12:02.000000 nrobo-2024.40.2/nrobo/browserConfigs/markers.yaml
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.110631 nrobo-2024.40.2/nrobo/browsers/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      459 2024-02-15 02:56:21.000000 nrobo-2024.40.2/nrobo/browsers/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.111204 nrobo-2024.40.2/nrobo/browsers/chrome/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2168 2024-02-15 02:56:21.000000 nrobo-2024.40.2/nrobo/browsers/chrome/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.111797 nrobo-2024.40.2/nrobo/browsers/edge/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      468 2024-02-15 02:56:21.000000 nrobo-2024.40.2/nrobo/browsers/edge/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.112378 nrobo-2024.40.2/nrobo/browsers/firefox/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      472 2024-02-29 19:11:43.000000 nrobo-2024.40.2/nrobo/browsers/firefox/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.112944 nrobo-2024.40.2/nrobo/browsers/safari/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      477 2024-02-29 19:11:43.000000 nrobo-2024.40.2/nrobo/browsers/safari/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.117149 nrobo-2024.40.2/nrobo/cli/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2654 2024-03-23 16:37:25.000000 nrobo-2024.40.2/nrobo/cli/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2895 2024-03-11 13:01:11.000000 nrobo-2024.40.2/nrobo/cli/cli_constants.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       17 2024-02-15 02:56:21.000000 nrobo-2024.40.2/nrobo/cli/cli_version.yaml
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.117719 nrobo-2024.40.2/nrobo/cli/detection/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2585 2024-02-29 19:12:02.000000 nrobo-2024.40.2/nrobo/cli/detection/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.118257 nrobo-2024.40.2/nrobo/cli/formatting/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1226 2024-02-29 19:11:43.000000 nrobo-2024.40.2/nrobo/cli/formatting/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.119496 nrobo-2024.40.2/nrobo/cli/install/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    12266 2024-03-24 02:00:53.000000 nrobo-2024.40.2/nrobo/cli/install/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      987 2024-04-02 19:56:57.000000 nrobo-2024.40.2/nrobo/cli/install/requirements.txt
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    15058 2024-03-07 11:01:00.000000 nrobo-2024.40.2/nrobo/cli/launcher.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.120053 nrobo-2024.40.2/nrobo/cli/ncodes/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      594 2024-02-29 19:12:02.000000 nrobo-2024.40.2/nrobo/cli/ncodes/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1806 2024-03-01 03:35:55.000000 nrobo-2024.40.2/nrobo/cli/nglobals.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.120604 nrobo-2024.40.2/nrobo/cli/nrobo_args/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    25971 2024-03-11 13:04:58.000000 nrobo-2024.40.2/nrobo/cli/nrobo_args/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.121084 nrobo-2024.40.2/nrobo/cli/tools/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      813 2024-02-29 19:11:43.000000 nrobo-2024.40.2/nrobo/cli/tools/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.121438 nrobo-2024.40.2/nrobo/cli/upgrade/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     6308 2024-03-06 04:27:25.000000 nrobo-2024.40.2/nrobo/cli/upgrade/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    32195 2024-04-11 06:46:40.000000 nrobo-2024.40.2/nrobo/conftest.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.121763 nrobo-2024.40.2/nrobo/db/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      477 2024-04-06 18:20:42.000000 nrobo-2024.40.2/nrobo/db/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.122079 nrobo-2024.40.2/nrobo/exceptions/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1937 2024-02-29 19:12:02.000000 nrobo-2024.40.2/nrobo/exceptions/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.123946 nrobo-2024.40.2/nrobo/framework/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-02-05 04:31:26.000000 nrobo-2024.40.2/nrobo/framework/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      540 2024-02-16 15:47:33.000000 nrobo-2024.40.2/nrobo/framework/conftest-host.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      779 2024-03-07 13:19:52.000000 nrobo-2024.40.2/nrobo/framework/nrobo-config.yaml
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.124928 nrobo-2024.40.2/nrobo/framework/pages/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1506 2024-02-29 19:12:02.000000 nrobo-2024.40.2/nrobo/framework/pages/PagePyPiHome.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      485 2024-02-29 19:12:02.000000 nrobo-2024.40.2/nrobo/framework/pages/PageSearch.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2540 2024-02-29 19:12:02.000000 nrobo-2024.40.2/nrobo/framework/pages/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       26 2024-03-23 15:17:33.000000 nrobo-2024.40.2/nrobo/framework/requirements.txt
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-30 08:56:49.000000 nrobo-2024.40.2/nrobo/framework/secrets.yaml
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.125540 nrobo-2024.40.2/nrobo/framework/test-data/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 19:41:06.000000 nrobo-2024.40.2/nrobo/framework/test-data/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     6402 2024-02-13 06:51:47.000000 nrobo-2024.40.2/nrobo/framework/test-data/nRoBo-Logo.png
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.125891 nrobo-2024.40.2/nrobo/framework/tests/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        2 2024-02-07 04:51:13.000000 nrobo-2024.40.2/nrobo/framework/tests/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.098888 nrobo-2024.40.2/nrobo/framework/tests/mobile/
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.126234 nrobo-2024.40.2/nrobo/framework/tests/mobile/appium/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      383 2024-03-07 08:23:34.000000 nrobo-2024.40.2/nrobo/framework/tests/mobile/appium/test_appium.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.126582 nrobo-2024.40.2/nrobo/framework/tests/web/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1904 2024-02-29 19:12:02.000000 nrobo-2024.40.2/nrobo/framework/tests/web/PyPi_home_page_test.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.126920 nrobo-2024.40.2/nrobo/framework/tests/web/examples/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     6470 2024-02-29 19:12:02.000000 nrobo-2024.40.2/nrobo/framework/tests/web/examples/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.127617 nrobo-2024.40.2/nrobo/framework/tests/web/gui/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      723 2024-03-03 02:33:11.000000 nrobo-2024.40.2/nrobo/framework/tests/web/gui/PyPi_home_page_test.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-02-06 09:49:32.000000 nrobo-2024.40.2/nrobo/framework/tests/web/gui/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.127896 nrobo-2024.40.2/nrobo/framework/tests/web/no_gui/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-02-06 09:49:18.000000 nrobo-2024.40.2/nrobo/framework/tests/web/no_gui/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.130291 nrobo-2024.40.2/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-02-29 19:12:02.000000 nrobo-2024.40.2/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      820 2024-02-29 19:12:02.000000 nrobo-2024.40.2/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_action_chain_methods.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2427 2024-02-29 19:12:02.000000 nrobo-2024.40.2/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_alert_methods.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     8284 2024-04-05 20:33:08.000000 nrobo-2024.40.2/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_element_wrapper_methods.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    19118 2024-02-29 19:12:02.000000 nrobo-2024.40.2/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_nrobo_methods.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1418 2024-02-29 19:12:02.000000 nrobo-2024.40.2/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_nrobo_wait_methods.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     6860 2024-02-29 19:12:02.000000 nrobo-2024.40.2/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_select.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.130625 nrobo-2024.40.2/nrobo/selenese/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    49008 2024-04-06 08:38:03.000000 nrobo-2024.40.2/nrobo/selenese/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.131029 nrobo-2024.40.2/nrobo/util/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      431 2024-02-15 02:56:21.000000 nrobo-2024.40.2/nrobo/util/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.131363 nrobo-2024.40.2/nrobo/util/commands/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      431 2024-02-15 02:56:21.000000 nrobo-2024.40.2/nrobo/util/commands/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.131692 nrobo-2024.40.2/nrobo/util/commands/ncommands/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2105 2024-03-06 18:41:46.000000 nrobo-2024.40.2/nrobo/util/commands/ncommands/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.132029 nrobo-2024.40.2/nrobo/util/commands/posix/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      533 2024-02-29 19:11:43.000000 nrobo-2024.40.2/nrobo/util/commands/posix/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.132358 nrobo-2024.40.2/nrobo/util/commands/windows/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      535 2024-02-29 19:11:43.000000 nrobo-2024.40.2/nrobo/util/commands/windows/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.132690 nrobo-2024.40.2/nrobo/util/common/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     7376 2024-03-18 10:49:47.000000 nrobo-2024.40.2/nrobo/util/common/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.133128 nrobo-2024.40.2/nrobo/util/constants/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1686 2024-02-29 19:11:43.000000 nrobo-2024.40.2/nrobo/util/constants/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.133840 nrobo-2024.40.2/nrobo/util/database/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-30 08:55:53.000000 nrobo-2024.40.2/nrobo/util/database/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1992 2024-03-30 08:55:53.000000 nrobo-2024.40.2/nrobo/util/database/connectors.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.134216 nrobo-2024.40.2/nrobo/util/filesystem/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     6919 2024-02-29 19:12:02.000000 nrobo-2024.40.2/nrobo/util/filesystem/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.134577 nrobo-2024.40.2/nrobo/util/network/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      844 2024-02-29 19:12:02.000000 nrobo-2024.40.2/nrobo/util/network/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.134939 nrobo-2024.40.2/nrobo/util/platform/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      742 2024-02-29 19:11:43.000000 nrobo-2024.40.2/nrobo/util/platform/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.135279 nrobo-2024.40.2/nrobo/util/process/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     3322 2024-02-29 19:12:02.000000 nrobo-2024.40.2/nrobo/util/process/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.135631 nrobo-2024.40.2/nrobo/util/python/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2101 2024-02-29 19:11:43.000000 nrobo-2024.40.2/nrobo/util/python/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.135980 nrobo-2024.40.2/nrobo/util/regex/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      976 2024-02-29 19:11:43.000000 nrobo-2024.40.2/nrobo/util/regex/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.136317 nrobo-2024.40.2/nrobo/util/version/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     8316 2024-02-29 19:12:02.000000 nrobo-2024.40.2/nrobo/util/version/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-11 06:47:03.136792 nrobo-2024.40.2/nrobo.egg-info/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    18169 2024-04-11 06:47:03.000000 nrobo-2024.40.2/nrobo.egg-info/PKG-INFO
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2898 2024-04-11 06:47:03.000000 nrobo-2024.40.2/nrobo.egg-info/SOURCES.txt
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        1 2024-04-11 06:47:03.000000 nrobo-2024.40.2/nrobo.egg-info/dependency_links.txt
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       41 2024-04-11 06:47:03.000000 nrobo-2024.40.2/nrobo.egg-info/entry_points.txt
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       43 2024-04-11 06:47:03.000000 nrobo-2024.40.2/nrobo.egg-info/requires.txt
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        6 2024-04-11 06:47:03.000000 nrobo-2024.40.2/nrobo.egg-info/top_level.txt
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2545 2024-04-11 06:46:40.000000 nrobo-2024.40.2/pyproject.toml
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       38 2024-04-11 06:47:03.138372 nrobo-2024.40.2/setup.cfg
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.553110 nrobo-2024.40.3/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1079 2024-02-02 05:31:36.000000 nrobo-2024.40.3/LICENSE
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    18234 2024-05-16 07:11:22.552395 nrobo-2024.40.3/PKG-INFO
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    16596 2024-05-16 07:11:15.000000 nrobo-2024.40.3/README.rst
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.491688 nrobo-2024.40.3/nrobo/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     8702 2024-05-16 07:11:07.000000 nrobo-2024.40.3/nrobo/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.495955 nrobo-2024.40.3/nrobo/appium/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      716 2024-03-11 11:20:45.000000 nrobo-2024.40.3/nrobo/appium/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       72 2024-03-11 14:41:50.000000 nrobo-2024.40.3/nrobo/appium/android_capability.yaml
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       73 2024-03-11 12:05:03.000000 nrobo-2024.40.3/nrobo/appium/ios_capability.yaml
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.496388 nrobo-2024.40.3/nrobo/aws/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      475 2024-04-06 18:19:37.000000 nrobo-2024.40.3/nrobo/aws/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.500906 nrobo-2024.40.3/nrobo/browserConfigs/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      452 2024-02-29 19:11:43.000000 nrobo-2024.40.3/nrobo/browserConfigs/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       35 2024-02-29 19:12:02.000000 nrobo-2024.40.3/nrobo/browserConfigs/capability.yaml
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       17 2024-02-19 15:42:30.000000 nrobo-2024.40.3/nrobo/browserConfigs/chrome_config.txt
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       39 2024-02-29 19:12:02.000000 nrobo-2024.40.3/nrobo/browserConfigs/chrome_prefs.yaml
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       63 2024-02-29 19:12:02.000000 nrobo-2024.40.3/nrobo/browserConfigs/markers.yaml
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.501344 nrobo-2024.40.3/nrobo/browsers/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      459 2024-02-15 02:56:21.000000 nrobo-2024.40.3/nrobo/browsers/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.502254 nrobo-2024.40.3/nrobo/browsers/chrome/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2168 2024-02-15 02:56:21.000000 nrobo-2024.40.3/nrobo/browsers/chrome/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.502942 nrobo-2024.40.3/nrobo/browsers/edge/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      468 2024-02-15 02:56:21.000000 nrobo-2024.40.3/nrobo/browsers/edge/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.503562 nrobo-2024.40.3/nrobo/browsers/firefox/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      472 2024-02-29 19:11:43.000000 nrobo-2024.40.3/nrobo/browsers/firefox/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.504495 nrobo-2024.40.3/nrobo/browsers/safari/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      477 2024-02-29 19:11:43.000000 nrobo-2024.40.3/nrobo/browsers/safari/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.508931 nrobo-2024.40.3/nrobo/cli/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2654 2024-03-23 16:37:25.000000 nrobo-2024.40.3/nrobo/cli/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2895 2024-03-11 13:01:11.000000 nrobo-2024.40.3/nrobo/cli/cli_constants.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       17 2024-02-15 02:56:21.000000 nrobo-2024.40.3/nrobo/cli/cli_version.yaml
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.509791 nrobo-2024.40.3/nrobo/cli/detection/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2585 2024-02-29 19:12:02.000000 nrobo-2024.40.3/nrobo/cli/detection/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.510641 nrobo-2024.40.3/nrobo/cli/formatting/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1226 2024-02-29 19:11:43.000000 nrobo-2024.40.3/nrobo/cli/formatting/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.512413 nrobo-2024.40.3/nrobo/cli/install/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    12266 2024-03-24 02:00:53.000000 nrobo-2024.40.3/nrobo/cli/install/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      987 2024-04-02 19:56:57.000000 nrobo-2024.40.3/nrobo/cli/install/requirements.txt
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    15058 2024-03-07 11:01:00.000000 nrobo-2024.40.3/nrobo/cli/launcher.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.512895 nrobo-2024.40.3/nrobo/cli/ncodes/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      594 2024-02-29 19:12:02.000000 nrobo-2024.40.3/nrobo/cli/ncodes/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1806 2024-03-01 03:35:55.000000 nrobo-2024.40.3/nrobo/cli/nglobals.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.513706 nrobo-2024.40.3/nrobo/cli/nrobo_args/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    25971 2024-03-11 13:04:58.000000 nrobo-2024.40.3/nrobo/cli/nrobo_args/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.514849 nrobo-2024.40.3/nrobo/cli/tools/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      813 2024-02-29 19:11:43.000000 nrobo-2024.40.3/nrobo/cli/tools/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.515647 nrobo-2024.40.3/nrobo/cli/upgrade/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     6308 2024-03-06 04:27:25.000000 nrobo-2024.40.3/nrobo/cli/upgrade/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    32195 2024-05-16 07:11:07.000000 nrobo-2024.40.3/nrobo/conftest.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.516443 nrobo-2024.40.3/nrobo/db/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      477 2024-04-06 18:20:42.000000 nrobo-2024.40.3/nrobo/db/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.517298 nrobo-2024.40.3/nrobo/exceptions/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1937 2024-02-29 19:12:02.000000 nrobo-2024.40.3/nrobo/exceptions/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.520614 nrobo-2024.40.3/nrobo/framework/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-02-05 04:31:26.000000 nrobo-2024.40.3/nrobo/framework/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      540 2024-02-16 15:47:33.000000 nrobo-2024.40.3/nrobo/framework/conftest-host.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      779 2024-03-07 13:19:52.000000 nrobo-2024.40.3/nrobo/framework/nrobo-config.yaml
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.522465 nrobo-2024.40.3/nrobo/framework/pages/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1506 2024-02-29 19:12:02.000000 nrobo-2024.40.3/nrobo/framework/pages/PagePyPiHome.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      485 2024-02-29 19:12:02.000000 nrobo-2024.40.3/nrobo/framework/pages/PageSearch.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2540 2024-02-29 19:12:02.000000 nrobo-2024.40.3/nrobo/framework/pages/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       26 2024-03-23 15:17:33.000000 nrobo-2024.40.3/nrobo/framework/requirements.txt
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-30 08:56:49.000000 nrobo-2024.40.3/nrobo/framework/secrets.yaml
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.523458 nrobo-2024.40.3/nrobo/framework/test-data/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 19:41:06.000000 nrobo-2024.40.3/nrobo/framework/test-data/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     6402 2024-02-13 06:51:47.000000 nrobo-2024.40.3/nrobo/framework/test-data/nRoBo-Logo.png
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.524271 nrobo-2024.40.3/nrobo/framework/tests/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        2 2024-02-07 04:51:13.000000 nrobo-2024.40.3/nrobo/framework/tests/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.483798 nrobo-2024.40.3/nrobo/framework/tests/mobile/
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.525282 nrobo-2024.40.3/nrobo/framework/tests/mobile/appium/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      383 2024-03-07 08:23:34.000000 nrobo-2024.40.3/nrobo/framework/tests/mobile/appium/test_appium.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.526111 nrobo-2024.40.3/nrobo/framework/tests/web/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1904 2024-02-29 19:12:02.000000 nrobo-2024.40.3/nrobo/framework/tests/web/PyPi_home_page_test.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.526814 nrobo-2024.40.3/nrobo/framework/tests/web/examples/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     6470 2024-02-29 19:12:02.000000 nrobo-2024.40.3/nrobo/framework/tests/web/examples/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.528591 nrobo-2024.40.3/nrobo/framework/tests/web/gui/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      723 2024-03-03 02:33:11.000000 nrobo-2024.40.3/nrobo/framework/tests/web/gui/PyPi_home_page_test.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-02-06 09:49:32.000000 nrobo-2024.40.3/nrobo/framework/tests/web/gui/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.528926 nrobo-2024.40.3/nrobo/framework/tests/web/no_gui/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-02-06 09:49:18.000000 nrobo-2024.40.3/nrobo/framework/tests/web/no_gui/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.534514 nrobo-2024.40.3/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-02-29 19:12:02.000000 nrobo-2024.40.3/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      820 2024-02-29 19:12:02.000000 nrobo-2024.40.3/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_action_chain_methods.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2427 2024-02-29 19:12:02.000000 nrobo-2024.40.3/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_alert_methods.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     8284 2024-04-05 20:33:08.000000 nrobo-2024.40.3/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_element_wrapper_methods.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    19118 2024-02-29 19:12:02.000000 nrobo-2024.40.3/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_nrobo_methods.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1418 2024-02-29 19:12:02.000000 nrobo-2024.40.3/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_nrobo_wait_methods.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     6860 2024-02-29 19:12:02.000000 nrobo-2024.40.3/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_select.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.535338 nrobo-2024.40.3/nrobo/selenese/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    49008 2024-04-06 08:38:03.000000 nrobo-2024.40.3/nrobo/selenese/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.535854 nrobo-2024.40.3/nrobo/util/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      431 2024-02-15 02:56:21.000000 nrobo-2024.40.3/nrobo/util/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.536571 nrobo-2024.40.3/nrobo/util/commands/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      431 2024-02-15 02:56:21.000000 nrobo-2024.40.3/nrobo/util/commands/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.537179 nrobo-2024.40.3/nrobo/util/commands/ncommands/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2105 2024-03-06 18:41:46.000000 nrobo-2024.40.3/nrobo/util/commands/ncommands/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.538323 nrobo-2024.40.3/nrobo/util/commands/posix/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      533 2024-02-29 19:11:43.000000 nrobo-2024.40.3/nrobo/util/commands/posix/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.539406 nrobo-2024.40.3/nrobo/util/commands/windows/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      535 2024-02-29 19:11:43.000000 nrobo-2024.40.3/nrobo/util/commands/windows/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.540525 nrobo-2024.40.3/nrobo/util/common/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     7376 2024-03-18 10:49:47.000000 nrobo-2024.40.3/nrobo/util/common/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.541602 nrobo-2024.40.3/nrobo/util/constants/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1686 2024-02-29 19:11:43.000000 nrobo-2024.40.3/nrobo/util/constants/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.542978 nrobo-2024.40.3/nrobo/util/database/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-30 08:55:53.000000 nrobo-2024.40.3/nrobo/util/database/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1992 2024-03-30 08:55:53.000000 nrobo-2024.40.3/nrobo/util/database/connectors.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.544556 nrobo-2024.40.3/nrobo/util/filesystem/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     6919 2024-02-29 19:12:02.000000 nrobo-2024.40.3/nrobo/util/filesystem/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.545589 nrobo-2024.40.3/nrobo/util/network/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      844 2024-02-29 19:12:02.000000 nrobo-2024.40.3/nrobo/util/network/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.546323 nrobo-2024.40.3/nrobo/util/platform/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      742 2024-02-29 19:11:43.000000 nrobo-2024.40.3/nrobo/util/platform/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.547430 nrobo-2024.40.3/nrobo/util/process/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     3322 2024-02-29 19:12:02.000000 nrobo-2024.40.3/nrobo/util/process/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.548174 nrobo-2024.40.3/nrobo/util/python/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2101 2024-02-29 19:11:43.000000 nrobo-2024.40.3/nrobo/util/python/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.549243 nrobo-2024.40.3/nrobo/util/regex/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      976 2024-02-29 19:11:43.000000 nrobo-2024.40.3/nrobo/util/regex/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.550356 nrobo-2024.40.3/nrobo/util/version/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     8316 2024-02-29 19:12:02.000000 nrobo-2024.40.3/nrobo/util/version/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-05-16 07:11:22.551400 nrobo-2024.40.3/nrobo.egg-info/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    18234 2024-05-16 07:11:22.000000 nrobo-2024.40.3/nrobo.egg-info/PKG-INFO
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2898 2024-05-16 07:11:22.000000 nrobo-2024.40.3/nrobo.egg-info/SOURCES.txt
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        1 2024-05-16 07:11:22.000000 nrobo-2024.40.3/nrobo.egg-info/dependency_links.txt
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       41 2024-05-16 07:11:22.000000 nrobo-2024.40.3/nrobo.egg-info/entry_points.txt
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       43 2024-05-16 07:11:22.000000 nrobo-2024.40.3/nrobo.egg-info/requires.txt
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        6 2024-05-16 07:11:22.000000 nrobo-2024.40.3/nrobo.egg-info/top_level.txt
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2545 2024-05-16 07:11:07.000000 nrobo-2024.40.3/pyproject.toml
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       38 2024-05-16 07:11:22.553240 nrobo-2024.40.3/setup.cfg
```

### Comparing `nrobo-2024.40.2/LICENSE` & `nrobo-2024.40.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.2/PKG-INFO` & `nrobo-2024.40.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrobo
-Version: 2024.40.2
+Version: 2024.40.3
 Summary: Powerful! Yet, Easy to USE! Automated Testing Framework
 Author-email: Panchdev Singh Chauhan <erpanchdev@gmail.com>
 Maintainer-email: Panchdev Singh Chauhan <erpanchdev@gmail.com>
 Project-URL: Homepage, https://pypi.org/project/nrobo/
 Project-URL: GitHub Repo, https://github.com/pancht/ngrobo
 Project-URL: Bug Tracker, https://github.com/pancht/ngrobo/issues
 Project-URL: changelog, https://github.com/pancht/ngrobo/blob/master/CHANGELOG.md
@@ -384,145 +384,151 @@
    :align: center
    :header-rows: 1
 
    * - Country
      - Percent
      - Download Count
    * - US
-     - 39.12%
-     - 24,003
+     - 40.48%
+     - 26,552
    * - CN
-     - 12.84%
-     - 7,878
+     - 12.31%
+     - 8,074
    * - DE
-     - 6.98%
-     - 4,282
+     - 6.79%
+     - 4,453
    * - SG
-     - 5.48%
-     - 3,364
+     - 5.26%
+     - 3,447
    * - RU
-     - 5.22%
-     - 3,202
+     - 5.14%
+     - 3,374
    * - HK
-     - 4.05%
-     - 2,486
+     - 4.10%
+     - 2,690
    * - JP
      - 3.01%
-     - 1,846
+     - 1,976
    * - FR
-     - 2.80%
-     - 1,719
+     - 2.99%
+     - 1,961
    * - KR
-     - 2.69%
-     - 1,652
+     - 2.53%
+     - 1,661
    * - CA
-     - 2.62%
-     - 1,607
+     - 2.46%
+     - 1,613
    * - NO
-     - 2.16%
-     - 1,327
+     - 2.21%
+     - 1,449
    * - GB
-     - 1.79%
-     - 1,100
+     - 1.76%
+     - 1,155
    * - AU
-     - 1.74%
-     - 1,065
-   * - IN
-     - 1.50%
-     - 923
+     - 1.63%
+     - 1,071
    * - SE
-     - 1.18%
-     - 725
+     - 1.43%
+     - 940
+   * - IN
+     - 1.41%
+     - 927
    * - TH
-     - 0.77%
-     - 475
+     - 0.73%
+     - 479
    * - HR
-     - 0.76%
-     - 468
-   * - IE
-     - 0.65%
-     - 399
+     - 0.72%
+     - 470
    * - DK
-     - 0.65%
-     - 397
+     - 0.67%
+     - 439
+   * - IE
+     - 0.61%
+     - 403
    * - TW
-     - 0.59%
+     - 0.55%
      - 363
    * - IL
-     - 0.56%
+     - 0.52%
      - 341
    * - NL
-     - 0.48%
+     - 0.45%
      - 297
    * - ES
-     - 0.43%
+     - 0.40%
      - 262
    * - CH
-     - 0.42%
-     - 255
+     - 0.39%
+     - 257
    * - AE
-     - 0.34%
+     - 0.32%
      - 209
    * - CZ
-     - 0.23%
+     - 0.22%
      - 144
    * - FI
      - 0.16%
-     - 99
+     - 107
    * - ZA
-     - 0.15%
+     - 0.14%
      - 89
    * - BR
-     - 0.13%
-     - 77
+     - 0.12%
+     - 78
    * - PL
-     - 0.10%
+     - 0.09%
      - 61
    * - TR
      - 0.07%
      - 46
    * - CW
      - 0.07%
      - 44
-   * - IS
-     - 0.07%
-     - 42
    * - OM
-     - 0.07%
+     - 0.06%
+     - 42
+   * - IS
+     - 0.06%
      - 42
    * - RO
      - 0.04%
      - 24
    * - GF
      - 0.02%
-     - 10
+     - 14
    * - UA
      - 0.01%
      - 8
    * - CY
      - 0.01%
+     - 7
+   * - BE
+     - 0.01%
      - 6
    * - DZ
      - 0.01%
      - 4
    * - AR
      - 0.00%
      - 3
    * - EE
      - 0.00%
      - 3
+   * - CL
+     - 0.00%
+     - 2
    * - SK
      - 0.00%
      - 2
-   * - MX
+   * - RS
      - 0.00%
      - 1
-   * - RS
+   * - MX
      - 0.00%
      - 1
    * - PT
      - 0.00%
      - 1
    * - **Total**
      - **100.00%**
-     - **61,352**
+     - **65,592**
```

### Comparing `nrobo-2024.40.2/README.rst` & `nrobo-2024.40.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -348,145 +348,151 @@
    :align: center
    :header-rows: 1
 
    * - Country
      - Percent
      - Download Count
    * - US
-     - 39.12%
-     - 24,003
+     - 40.48%
+     - 26,552
    * - CN
-     - 12.84%
-     - 7,878
+     - 12.31%
+     - 8,074
    * - DE
-     - 6.98%
-     - 4,282
+     - 6.79%
+     - 4,453
    * - SG
-     - 5.48%
-     - 3,364
+     - 5.26%
+     - 3,447
    * - RU
-     - 5.22%
-     - 3,202
+     - 5.14%
+     - 3,374
    * - HK
-     - 4.05%
-     - 2,486
+     - 4.10%
+     - 2,690
    * - JP
      - 3.01%
-     - 1,846
+     - 1,976
    * - FR
-     - 2.80%
-     - 1,719
+     - 2.99%
+     - 1,961
    * - KR
-     - 2.69%
-     - 1,652
+     - 2.53%
+     - 1,661
    * - CA
-     - 2.62%
-     - 1,607
+     - 2.46%
+     - 1,613
    * - NO
-     - 2.16%
-     - 1,327
+     - 2.21%
+     - 1,449
    * - GB
-     - 1.79%
-     - 1,100
+     - 1.76%
+     - 1,155
    * - AU
-     - 1.74%
-     - 1,065
-   * - IN
-     - 1.50%
-     - 923
+     - 1.63%
+     - 1,071
    * - SE
-     - 1.18%
-     - 725
+     - 1.43%
+     - 940
+   * - IN
+     - 1.41%
+     - 927
    * - TH
-     - 0.77%
-     - 475
+     - 0.73%
+     - 479
    * - HR
-     - 0.76%
-     - 468
-   * - IE
-     - 0.65%
-     - 399
+     - 0.72%
+     - 470
    * - DK
-     - 0.65%
-     - 397
+     - 0.67%
+     - 439
+   * - IE
+     - 0.61%
+     - 403
    * - TW
-     - 0.59%
+     - 0.55%
      - 363
    * - IL
-     - 0.56%
+     - 0.52%
      - 341
    * - NL
-     - 0.48%
+     - 0.45%
      - 297
    * - ES
-     - 0.43%
+     - 0.40%
      - 262
    * - CH
-     - 0.42%
-     - 255
+     - 0.39%
+     - 257
    * - AE
-     - 0.34%
+     - 0.32%
      - 209
    * - CZ
-     - 0.23%
+     - 0.22%
      - 144
    * - FI
      - 0.16%
-     - 99
+     - 107
    * - ZA
-     - 0.15%
+     - 0.14%
      - 89
    * - BR
-     - 0.13%
-     - 77
+     - 0.12%
+     - 78
    * - PL
-     - 0.10%
+     - 0.09%
      - 61
    * - TR
      - 0.07%
      - 46
    * - CW
      - 0.07%
      - 44
-   * - IS
-     - 0.07%
-     - 42
    * - OM
-     - 0.07%
+     - 0.06%
+     - 42
+   * - IS
+     - 0.06%
      - 42
    * - RO
      - 0.04%
      - 24
    * - GF
      - 0.02%
-     - 10
+     - 14
    * - UA
      - 0.01%
      - 8
    * - CY
      - 0.01%
+     - 7
+   * - BE
+     - 0.01%
      - 6
    * - DZ
      - 0.01%
      - 4
    * - AR
      - 0.00%
      - 3
    * - EE
      - 0.00%
      - 3
+   * - CL
+     - 0.00%
+     - 2
    * - SK
      - 0.00%
      - 2
-   * - MX
+   * - RS
      - 0.00%
      - 1
-   * - RS
+   * - MX
      - 0.00%
      - 1
    * - PT
      - 0.00%
      - 1
    * - **Total**
      - **100.00%**
-     - **61,352**
+     - **65,592**
```

### Comparing `nrobo-2024.40.2/nrobo/__init__.py` & `nrobo-2024.40.3/nrobo/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 nrobo module loads nRoBo globals.
 
 
 @author: Panchdev Singh Chauhan
 @email: erpanchdev@gmail.com
 """
 
-__version__ = '2024.40.2'
+__version__ = '2024.40.3'
 
 # install rich library
 import os
 from pathlib import Path
 
 
 class DB_CONNECTOR_TYPE:
```

### Comparing `nrobo-2024.40.2/nrobo/appium/__init__.py` & `nrobo-2024.40.3/nrobo/appium/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.2/nrobo/browsers/chrome/__init__.py` & `nrobo-2024.40.3/nrobo/browsers/chrome/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.2/nrobo/cli/__init__.py` & `nrobo-2024.40.3/nrobo/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.2/nrobo/cli/cli_constants.py` & `nrobo-2024.40.3/nrobo/cli/cli_constants.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.2/nrobo/cli/detection/__init__.py` & `nrobo-2024.40.3/nrobo/cli/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.2/nrobo/cli/formatting/__init__.py` & `nrobo-2024.40.3/nrobo/cli/formatting/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.2/nrobo/cli/install/__init__.py` & `nrobo-2024.40.3/nrobo/cli/install/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.2/nrobo/cli/install/requirements.txt` & `nrobo-2024.40.3/nrobo/cli/install/requirements.txt`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.2/nrobo/cli/launcher.py` & `nrobo-2024.40.3/nrobo/cli/launcher.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.2/nrobo/cli/ncodes/__init__.py` & `nrobo-2024.40.3/nrobo/cli/ncodes/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.2/nrobo/cli/nglobals.py` & `nrobo-2024.40.3/nrobo/cli/nglobals.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.2/nrobo/cli/nrobo_args/__init__.py` & `nrobo-2024.40.3/nrobo/cli/nrobo_args/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.2/nrobo/cli/tools/__init__.py` & `nrobo-2024.40.3/nrobo/cli/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.2/nrobo/cli/upgrade/__init__.py` & `nrobo-2024.40.3/nrobo/cli/upgrade/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.2/nrobo/conftest.py` & `nrobo-2024.40.3/nrobo/conftest.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.2/nrobo/exceptions/__init__.py` & `nrobo-2024.40.3/nrobo/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.2/nrobo/framework/conftest-host.py` & `nrobo-2024.40.3/nrobo/framework/conftest-host.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.2/nrobo/framework/nrobo-config.yaml` & `nrobo-2024.40.3/nrobo/framework/nrobo-config.yaml`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.2/nrobo/framework/pages/PagePyPiHome.py` & `nrobo-2024.40.3/nrobo/framework/pages/PagePyPiHome.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.2/nrobo/framework/pages/__init__.py` & `nrobo-2024.40.3/nrobo/framework/pages/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.2/nrobo/framework/test-data/nRoBo-Logo.png` & `nrobo-2024.40.3/nrobo/framework/test-data/nRoBo-Logo.png`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.2/nrobo/framework/tests/web/PyPi_home_page_test.py` & `nrobo-2024.40.3/nrobo/framework/tests/web/PyPi_home_page_test.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.2/nrobo/framework/tests/web/examples/__init__.py` & `nrobo-2024.40.3/nrobo/framework/tests/web/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.2/nrobo/framework/tests/web/gui/PyPi_home_page_test.py` & `nrobo-2024.40.3/nrobo/framework/tests/web/gui/PyPi_home_page_test.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.2/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_action_chain_methods.py` & `nrobo-2024.40.3/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_action_chain_methods.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.2/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_alert_methods.py` & `nrobo-2024.40.3/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_alert_methods.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.2/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_element_wrapper_methods.py` & `nrobo-2024.40.3/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_element_wrapper_methods.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.2/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_nrobo_methods.py` & `nrobo-2024.40.3/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_nrobo_methods.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.2/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_nrobo_wait_methods.py` & `nrobo-2024.40.3/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_nrobo_wait_methods.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.2/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_select.py` & `nrobo-2024.40.3/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_select.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.2/nrobo/selenese/__init__.py` & `nrobo-2024.40.3/nrobo/selenese/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.2/nrobo/util/commands/ncommands/__init__.py` & `nrobo-2024.40.3/nrobo/util/commands/ncommands/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.2/nrobo/util/commands/posix/__init__.py` & `nrobo-2024.40.3/nrobo/util/commands/posix/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.2/nrobo/util/commands/windows/__init__.py` & `nrobo-2024.40.3/nrobo/util/commands/windows/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.2/nrobo/util/common/__init__.py` & `nrobo-2024.40.3/nrobo/util/common/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.2/nrobo/util/constants/__init__.py` & `nrobo-2024.40.3/nrobo/util/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.2/nrobo/util/database/connectors.py` & `nrobo-2024.40.3/nrobo/util/database/connectors.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.2/nrobo/util/filesystem/__init__.py` & `nrobo-2024.40.3/nrobo/util/filesystem/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.2/nrobo/util/network/__init__.py` & `nrobo-2024.40.3/nrobo/util/network/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.2/nrobo/util/platform/__init__.py` & `nrobo-2024.40.3/nrobo/util/platform/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.2/nrobo/util/process/__init__.py` & `nrobo-2024.40.3/nrobo/util/process/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.2/nrobo/util/python/__init__.py` & `nrobo-2024.40.3/nrobo/util/python/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.2/nrobo/util/regex/__init__.py` & `nrobo-2024.40.3/nrobo/util/regex/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.2/nrobo/util/version/__init__.py` & `nrobo-2024.40.3/nrobo/util/version/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.2/nrobo.egg-info/PKG-INFO` & `nrobo-2024.40.3/nrobo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrobo
-Version: 2024.40.2
+Version: 2024.40.3
 Summary: Powerful! Yet, Easy to USE! Automated Testing Framework
 Author-email: Panchdev Singh Chauhan <erpanchdev@gmail.com>
 Maintainer-email: Panchdev Singh Chauhan <erpanchdev@gmail.com>
 Project-URL: Homepage, https://pypi.org/project/nrobo/
 Project-URL: GitHub Repo, https://github.com/pancht/ngrobo
 Project-URL: Bug Tracker, https://github.com/pancht/ngrobo/issues
 Project-URL: changelog, https://github.com/pancht/ngrobo/blob/master/CHANGELOG.md
@@ -384,145 +384,151 @@
    :align: center
    :header-rows: 1
 
    * - Country
      - Percent
      - Download Count
    * - US
-     - 39.12%
-     - 24,003
+     - 40.48%
+     - 26,552
    * - CN
-     - 12.84%
-     - 7,878
+     - 12.31%
+     - 8,074
    * - DE
-     - 6.98%
-     - 4,282
+     - 6.79%
+     - 4,453
    * - SG
-     - 5.48%
-     - 3,364
+     - 5.26%
+     - 3,447
    * - RU
-     - 5.22%
-     - 3,202
+     - 5.14%
+     - 3,374
    * - HK
-     - 4.05%
-     - 2,486
+     - 4.10%
+     - 2,690
    * - JP
      - 3.01%
-     - 1,846
+     - 1,976
    * - FR
-     - 2.80%
-     - 1,719
+     - 2.99%
+     - 1,961
    * - KR
-     - 2.69%
-     - 1,652
+     - 2.53%
+     - 1,661
    * - CA
-     - 2.62%
-     - 1,607
+     - 2.46%
+     - 1,613
    * - NO
-     - 2.16%
-     - 1,327
+     - 2.21%
+     - 1,449
    * - GB
-     - 1.79%
-     - 1,100
+     - 1.76%
+     - 1,155
    * - AU
-     - 1.74%
-     - 1,065
-   * - IN
-     - 1.50%
-     - 923
+     - 1.63%
+     - 1,071
    * - SE
-     - 1.18%
-     - 725
+     - 1.43%
+     - 940
+   * - IN
+     - 1.41%
+     - 927
    * - TH
-     - 0.77%
-     - 475
+     - 0.73%
+     - 479
    * - HR
-     - 0.76%
-     - 468
-   * - IE
-     - 0.65%
-     - 399
+     - 0.72%
+     - 470
    * - DK
-     - 0.65%
-     - 397
+     - 0.67%
+     - 439
+   * - IE
+     - 0.61%
+     - 403
    * - TW
-     - 0.59%
+     - 0.55%
      - 363
    * - IL
-     - 0.56%
+     - 0.52%
      - 341
    * - NL
-     - 0.48%
+     - 0.45%
      - 297
    * - ES
-     - 0.43%
+     - 0.40%
      - 262
    * - CH
-     - 0.42%
-     - 255
+     - 0.39%
+     - 257
    * - AE
-     - 0.34%
+     - 0.32%
      - 209
    * - CZ
-     - 0.23%
+     - 0.22%
      - 144
    * - FI
      - 0.16%
-     - 99
+     - 107
    * - ZA
-     - 0.15%
+     - 0.14%
      - 89
    * - BR
-     - 0.13%
-     - 77
+     - 0.12%
+     - 78
    * - PL
-     - 0.10%
+     - 0.09%
      - 61
    * - TR
      - 0.07%
      - 46
    * - CW
      - 0.07%
      - 44
-   * - IS
-     - 0.07%
-     - 42
    * - OM
-     - 0.07%
+     - 0.06%
+     - 42
+   * - IS
+     - 0.06%
      - 42
    * - RO
      - 0.04%
      - 24
    * - GF
      - 0.02%
-     - 10
+     - 14
    * - UA
      - 0.01%
      - 8
    * - CY
      - 0.01%
+     - 7
+   * - BE
+     - 0.01%
      - 6
    * - DZ
      - 0.01%
      - 4
    * - AR
      - 0.00%
      - 3
    * - EE
      - 0.00%
      - 3
+   * - CL
+     - 0.00%
+     - 2
    * - SK
      - 0.00%
      - 2
-   * - MX
+   * - RS
      - 0.00%
      - 1
-   * - RS
+   * - MX
      - 0.00%
      - 1
    * - PT
      - 0.00%
      - 1
    * - **Total**
      - **100.00%**
-     - **61,352**
+     - **65,592**
```

### Comparing `nrobo-2024.40.2/nrobo.egg-info/SOURCES.txt` & `nrobo-2024.40.3/nrobo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.2/pyproject.toml` & `nrobo-2024.40.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [build-system]
 requires = ["setuptools >= 40.7.0",]
 build-backend = "setuptools.build_meta"
 
 # Project details
 [project]
 name = "nrobo"
-version = "2024.40.2"
+version = "2024.40.3"
 authors = [{name="Panchdev Singh Chauhan", email="erpanchdev@gmail.com"}]
 maintainers = [{name="Panchdev Singh Chauhan", email="erpanchdev@gmail.com"}]
 description = "Powerful! Yet, Easy to USE! Automated Testing Framework"
 readme = "README.rst"
 keywords = ["test automation", "test automation framework", "automated testing", "automation testing", "testing", "qa", "acceptance test", "automation"]
 classifiers = [
     "Programming Language :: Python :: 3 :: Only",
```

