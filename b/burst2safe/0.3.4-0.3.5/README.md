# Comparing `tmp/burst2safe-0.3.4.tar.gz` & `tmp/burst2safe-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "burst2safe-0.3.4.tar", last modified: Tue May 14 12:52:22 2024, max compression
+gzip compressed data, was "burst2safe-0.3.5.tar", last modified: Thu May 16 14:26:32 2024, max compression
```

## Comparing `burst2safe-0.3.4.tar` & `burst2safe-0.3.5.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:52:22.690976 burst2safe-0.3.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:52:22.614976 burst2safe-0.3.4/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 12:52:17.000000 burst2safe-0.3.4/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-14 12:52:17.000000 burst2safe-0.3.4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:52:22.614976 burst2safe-0.3.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-14 12:52:17.000000 burst2safe-0.3.4/.github/workflows/build-and-deploy-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-14 12:52:17.000000 burst2safe-0.3.4/.github/workflows/build-and-deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-14 12:52:17.000000 burst2safe-0.3.4/.github/workflows/bump-version.yml
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-14 12:52:17.000000 burst2safe-0.3.4/.github/workflows/changelog-check.yml
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-14 12:52:17.000000 burst2safe-0.3.4/.github/workflows/labeled-pr-check.yml
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-14 12:52:17.000000 burst2safe-0.3.4/.github/workflows/pytest-golden.yml
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-14 12:52:17.000000 burst2safe-0.3.4/.github/workflows/pytest-integration.yml
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-14 12:52:17.000000 burst2safe-0.3.4/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-14 12:52:17.000000 burst2safe-0.3.4/.github/workflows/release-checklist-comment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-14 12:52:17.000000 burst2safe-0.3.4/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-14 12:52:17.000000 burst2safe-0.3.4/.github/workflows/static-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-14 12:52:17.000000 burst2safe-0.3.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-14 12:52:17.000000 burst2safe-0.3.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-14 12:52:17.000000 burst2safe-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9305 2024-05-14 12:52:22.686976 burst2safe-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8318 2024-05-14 12:52:17.000000 burst2safe-0.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-14 12:52:17.000000 burst2safe-0.3.4/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-14 12:52:17.000000 burst2safe-0.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 12:52:22.690976 burst2safe-0.3.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:52:22.610976 burst2safe-0.3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:52:22.618976 burst2safe-0.3.4/src/burst2safe/
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-14 12:52:17.000000 burst2safe-0.3.4/src/burst2safe/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    13777 2024-05-14 12:52:17.000000 burst2safe-0.3.4/src/burst2safe/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6593 2024-05-14 12:52:17.000000 burst2safe-0.3.4/src/burst2safe/burst2safe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-14 12:52:17.000000 burst2safe-0.3.4/src/burst2safe/calibration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:52:22.614976 burst2safe-0.3.4/src/burst2safe/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:52:22.618976 burst2safe-0.3.4/src/burst2safe/data/support_236/
--rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-14 12:52:17.000000 burst2safe-0.3.4/src/burst2safe/data/support_236/s1-level-1-calibration.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-14 12:52:17.000000 burst2safe-0.3.4/src/burst2safe/data/support_236/s1-level-1-measurement.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-05-14 12:52:17.000000 burst2safe-0.3.4/src/burst2safe/data/support_236/s1-level-1-noise.xsd
--rw-r--r--   0 runner    (1001) docker     (127)   147288 2024-05-14 12:52:17.000000 burst2safe-0.3.4/src/burst2safe/data/support_236/s1-level-1-product.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    62654 2024-05-14 12:52:17.000000 burst2safe-0.3.4/src/burst2safe/data/support_236/s1-object-types.xsd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:52:22.622976 burst2safe-0.3.4/src/burst2safe/data/support_245/
--rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-14 12:52:17.000000 burst2safe-0.3.4/src/burst2safe/data/support_245/s1-level-1-calibration.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-14 12:52:17.000000 burst2safe-0.3.4/src/burst2safe/data/support_245/s1-level-1-measurement.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-05-14 12:52:17.000000 burst2safe-0.3.4/src/burst2safe/data/support_245/s1-level-1-noise.xsd
--rw-r--r--   0 runner    (1001) docker     (127)   147222 2024-05-14 12:52:17.000000 burst2safe-0.3.4/src/burst2safe/data/support_245/s1-level-1-product.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    62654 2024-05-14 12:52:17.000000 burst2safe-0.3.4/src/burst2safe/data/support_245/s1-object-types.xsd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:52:22.622976 burst2safe-0.3.4/src/burst2safe/data/support_260/
--rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-14 12:52:17.000000 burst2safe-0.3.4/src/burst2safe/data/support_260/s1-level-1-calibration.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-14 12:52:17.000000 burst2safe-0.3.4/src/burst2safe/data/support_260/s1-level-1-measurement.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-05-14 12:52:17.000000 burst2safe-0.3.4/src/burst2safe/data/support_260/s1-level-1-noise.xsd
--rw-r--r--   0 runner    (1001) docker     (127)   147374 2024-05-14 12:52:17.000000 burst2safe-0.3.4/src/burst2safe/data/support_260/s1-level-1-product.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    62654 2024-05-14 12:52:17.000000 burst2safe-0.3.4/src/burst2safe/data/support_260/s1-object-types.xsd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:52:22.622976 burst2safe-0.3.4/src/burst2safe/data/support_290/
--rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-14 12:52:17.000000 burst2safe-0.3.4/src/burst2safe/data/support_290/s1-level-1-calibration.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-14 12:52:17.000000 burst2safe-0.3.4/src/burst2safe/data/support_290/s1-level-1-measurement.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-05-14 12:52:17.000000 burst2safe-0.3.4/src/burst2safe/data/support_290/s1-level-1-noise.xsd
--rw-r--r--   0 runner    (1001) docker     (127)   147374 2024-05-14 12:52:17.000000 burst2safe-0.3.4/src/burst2safe/data/support_290/s1-level-1-product.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    60608 2024-05-14 12:52:17.000000 burst2safe-0.3.4/src/burst2safe/data/support_290/s1-object-types.xsd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:52:22.622976 burst2safe-0.3.4/src/burst2safe/data/support_340/
--rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-14 12:52:17.000000 burst2safe-0.3.4/src/burst2safe/data/support_340/s1-level-1-calibration.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-14 12:52:17.000000 burst2safe-0.3.4/src/burst2safe/data/support_340/s1-level-1-measurement.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-05-14 12:52:17.000000 burst2safe-0.3.4/src/burst2safe/data/support_340/s1-level-1-noise.xsd
--rw-r--r--   0 runner    (1001) docker     (127)   149999 2024-05-14 12:52:17.000000 burst2safe-0.3.4/src/burst2safe/data/support_340/s1-level-1-product.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    16595 2024-05-14 12:52:17.000000 burst2safe-0.3.4/src/burst2safe/data/support_340/s1-level-1-rfi.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    61552 2024-05-14 12:52:17.000000 burst2safe-0.3.4/src/burst2safe/data/support_340/s1-object-types.xsd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:52:22.626976 burst2safe-0.3.4/src/burst2safe/data/support_371/
--rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-14 12:52:17.000000 burst2safe-0.3.4/src/burst2safe/data/support_371/s1-level-1-calibration.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-14 12:52:17.000000 burst2safe-0.3.4/src/burst2safe/data/support_371/s1-level-1-measurement.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-05-14 12:52:17.000000 burst2safe-0.3.4/src/burst2safe/data/support_371/s1-level-1-noise.xsd
--rw-r--r--   0 runner    (1001) docker     (127)   149999 2024-05-14 12:52:17.000000 burst2safe-0.3.4/src/burst2safe/data/support_371/s1-level-1-product.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    16595 2024-05-14 12:52:17.000000 burst2safe-0.3.4/src/burst2safe/data/support_371/s1-level-1-rfi.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    61720 2024-05-14 12:52:17.000000 burst2safe-0.3.4/src/burst2safe/data/support_371/s1-object-types.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-05-14 12:52:17.000000 burst2safe-0.3.4/src/burst2safe/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-05-14 12:52:17.000000 burst2safe-0.3.4/src/burst2safe/measurement.py
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-05-14 12:52:17.000000 burst2safe-0.3.4/src/burst2safe/noise.py
--rw-r--r--   0 runner    (1001) docker     (127)    12678 2024-05-14 12:52:17.000000 burst2safe-0.3.4/src/burst2safe/product.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-14 12:52:17.000000 burst2safe-0.3.4/src/burst2safe/rfi.py
--rw-r--r--   0 runner    (1001) docker     (127)    10988 2024-05-14 12:52:17.000000 burst2safe-0.3.4/src/burst2safe/safe.py
--rw-r--r--   0 runner    (1001) docker     (127)     7236 2024-05-14 12:52:17.000000 burst2safe-0.3.4/src/burst2safe/swath.py
--rw-r--r--   0 runner    (1001) docker     (127)     8595 2024-05-14 12:52:17.000000 burst2safe-0.3.4/src/burst2safe/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:52:22.686976 burst2safe-0.3.4/src/burst2safe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9305 2024-05-14 12:52:22.000000 burst2safe-0.3.4/src/burst2safe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-14 12:52:22.000000 burst2safe-0.3.4/src/burst2safe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 12:52:22.000000 burst2safe-0.3.4/src/burst2safe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-14 12:52:22.000000 burst2safe-0.3.4/src/burst2safe.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 12:52:21.000000 burst2safe-0.3.4/src/burst2safe.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-14 12:52:22.000000 burst2safe-0.3.4/src/burst2safe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 12:52:22.000000 burst2safe-0.3.4/src/burst2safe.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:52:22.626976 burst2safe-0.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-05-14 12:52:17.000000 burst2safe-0.3.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:52:22.626976 burst2safe-0.3.4/tests/etc/
--rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-05-14 12:52:17.000000 burst2safe-0.3.4/tests/etc/identify_ipf_differences.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-14 12:52:17.000000 burst2safe-0.3.4/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-14 12:52:17.000000 burst2safe-0.3.4/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     7394 2024-05-14 12:52:17.000000 burst2safe-0.3.4/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-14 12:52:17.000000 burst2safe-0.3.4/tests/test_burst2safe.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-14 12:52:17.000000 burst2safe-0.3.4/tests/test_calibration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:52:22.642976 burst2safe-0.3.4/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (127)  6288473 2024-05-14 12:52:17.000000 burst2safe-0.3.4/tests/test_data/S1A_IW_SLC__1SDV_20240408T015045_20240408T015113_053336_06778C_CB5D_VV.xml
--rw-r--r--   0 runner    (1001) docker     (127)  6073763 2024-05-14 12:52:17.000000 burst2safe-0.3.4/tests/test_data/S1A_IW_SLC__1SDV_20240408T015111_20240408T015138_053336_06778C_CA9A_VV.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:52:22.678976 burst2safe-0.3.4/tests/test_data/ipf/
--rw-r--r--   0 runner    (1001) docker     (127)  5647017 2024-05-14 12:52:17.000000 burst2safe-0.3.4/tests/test_data/ipf/S1A_IW_SLC__1SDV_20150117T170523_20150117T170551_004214_0051E7_AE35_VV.xml
--rw-r--r--   0 runner    (1001) docker     (127)  6067536 2024-05-14 12:52:17.000000 burst2safe-0.3.4/tests/test_data/ipf/S1A_IW_SLC__1SDV_20150622T170528_20150622T170556_006489_0089B0_EFBC_VV.xml
--rw-r--r--   0 runner    (1001) docker     (127)  6114849 2024-05-14 12:52:17.000000 burst2safe-0.3.4/tests/test_data/ipf/S1A_IW_SLC__1SDV_20160124T170510_20160124T170538_009639_00E0BA_7CC5_VV.xml
--rw-r--r--   0 runner    (1001) docker     (127)  6350843 2024-05-14 12:52:17.000000 burst2safe-0.3.4/tests/test_data/ipf/S1A_IW_SLC__1SDV_20211223T170557_20211223T170624_041139_04E360_B8E2_VV.xml
--rw-r--r--   0 runner    (1001) docker     (127)  6564579 2024-05-14 12:52:17.000000 burst2safe-0.3.4/tests/test_data/ipf/S1A_IW_SLC__1SDV_20240130T170606_20240130T170634_052339_065425_9A35_VV.xml
--rw-r--r--   0 runner    (1001) docker     (127)  6345069 2024-05-14 12:52:17.000000 burst2safe-0.3.4/tests/test_data/ipf/S1B_IW_SLC__1SDV_20180507T170449_20180507T170517_010818_013C70_6B12_VV.xml
--rw-r--r--   0 runner    (1001) docker     (127)    36523 2024-05-14 12:52:17.000000 burst2safe-0.3.4/tests/test_data/manifest_7C85.safe
--rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-05-14 12:52:17.000000 burst2safe-0.3.4/tests/test_golden.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-14 12:52:17.000000 burst2safe-0.3.4/tests/test_ipf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-05-14 12:52:17.000000 burst2safe-0.3.4/tests/test_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-05-14 12:52:17.000000 burst2safe-0.3.4/tests/test_measurement.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-14 12:52:17.000000 burst2safe-0.3.4/tests/test_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-14 12:52:17.000000 burst2safe-0.3.4/tests/test_product.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-14 12:52:17.000000 burst2safe-0.3.4/tests/test_rfi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-05-14 12:52:17.000000 burst2safe-0.3.4/tests/test_safe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-14 12:52:17.000000 burst2safe-0.3.4/tests/test_swath.py
--rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-05-14 12:52:17.000000 burst2safe-0.3.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:32.805987 burst2safe-0.3.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:32.729986 burst2safe-0.3.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-16 14:26:27.000000 burst2safe-0.3.5/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-16 14:26:27.000000 burst2safe-0.3.5/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:32.733986 burst2safe-0.3.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-16 14:26:27.000000 burst2safe-0.3.5/.github/workflows/build-and-deploy-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-16 14:26:27.000000 burst2safe-0.3.5/.github/workflows/build-and-deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-16 14:26:27.000000 burst2safe-0.3.5/.github/workflows/bump-version.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-16 14:26:27.000000 burst2safe-0.3.5/.github/workflows/changelog-check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-16 14:26:27.000000 burst2safe-0.3.5/.github/workflows/labeled-pr-check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-16 14:26:27.000000 burst2safe-0.3.5/.github/workflows/pytest-golden.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-16 14:26:27.000000 burst2safe-0.3.5/.github/workflows/pytest-integration.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-16 14:26:27.000000 burst2safe-0.3.5/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-16 14:26:27.000000 burst2safe-0.3.5/.github/workflows/release-checklist-comment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-16 14:26:27.000000 burst2safe-0.3.5/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-16 14:26:27.000000 burst2safe-0.3.5/.github/workflows/static-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-16 14:26:27.000000 burst2safe-0.3.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-16 14:26:27.000000 burst2safe-0.3.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-16 14:26:27.000000 burst2safe-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9305 2024-05-16 14:26:32.805987 burst2safe-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8318 2024-05-16 14:26:27.000000 burst2safe-0.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-16 14:26:27.000000 burst2safe-0.3.5/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-16 14:26:27.000000 burst2safe-0.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 14:26:32.805987 burst2safe-0.3.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:32.725985 burst2safe-0.3.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:32.733986 burst2safe-0.3.5/src/burst2safe/
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13777 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6727 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/burst2safe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/calibration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:32.729986 burst2safe-0.3.5/src/burst2safe/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:32.733986 burst2safe-0.3.5/src/burst2safe/data/support_236/
+-rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_236/s1-level-1-calibration.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_236/s1-level-1-measurement.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_236/s1-level-1-noise.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)   147288 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_236/s1-level-1-product.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    62654 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_236/s1-object-types.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:32.737986 burst2safe-0.3.5/src/burst2safe/data/support_245/
+-rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_245/s1-level-1-calibration.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_245/s1-level-1-measurement.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_245/s1-level-1-noise.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)   147222 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_245/s1-level-1-product.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    62654 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_245/s1-object-types.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:32.737986 burst2safe-0.3.5/src/burst2safe/data/support_260/
+-rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_260/s1-level-1-calibration.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_260/s1-level-1-measurement.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_260/s1-level-1-noise.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)   147374 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_260/s1-level-1-product.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    62654 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_260/s1-object-types.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:32.737986 burst2safe-0.3.5/src/burst2safe/data/support_290/
+-rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_290/s1-level-1-calibration.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_290/s1-level-1-measurement.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_290/s1-level-1-noise.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)   147374 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_290/s1-level-1-product.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    60608 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_290/s1-object-types.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:32.741986 burst2safe-0.3.5/src/burst2safe/data/support_340/
+-rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_340/s1-level-1-calibration.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_340/s1-level-1-measurement.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_340/s1-level-1-noise.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)   149999 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_340/s1-level-1-product.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    16595 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_340/s1-level-1-rfi.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    61552 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_340/s1-object-types.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:32.741986 burst2safe-0.3.5/src/burst2safe/data/support_371/
+-rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_371/s1-level-1-calibration.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_371/s1-level-1-measurement.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_371/s1-level-1-noise.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)   149999 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_371/s1-level-1-product.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    16595 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_371/s1-level-1-rfi.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    61720 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/data/support_371/s1-object-types.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6271 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12678 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/rfi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11110 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/safe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7236 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/swath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8595 2024-05-16 14:26:27.000000 burst2safe-0.3.5/src/burst2safe/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:32.805987 burst2safe-0.3.5/src/burst2safe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9305 2024-05-16 14:26:32.000000 burst2safe-0.3.5/src/burst2safe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-16 14:26:32.000000 burst2safe-0.3.5/src/burst2safe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 14:26:32.000000 burst2safe-0.3.5/src/burst2safe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-16 14:26:32.000000 burst2safe-0.3.5/src/burst2safe.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 14:26:32.000000 burst2safe-0.3.5/src/burst2safe.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-16 14:26:32.000000 burst2safe-0.3.5/src/burst2safe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-16 14:26:32.000000 burst2safe-0.3.5/src/burst2safe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:32.741986 burst2safe-0.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:32.745986 burst2safe-0.3.5/tests/etc/
+-rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/etc/identify_ipf_differences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7394 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/test_burst2safe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/test_calibration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:32.757986 burst2safe-0.3.5/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)  6288473 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/test_data/S1A_IW_SLC__1SDV_20240408T015045_20240408T015113_053336_06778C_CB5D_VV.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  6073763 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/test_data/S1A_IW_SLC__1SDV_20240408T015111_20240408T015138_053336_06778C_CA9A_VV.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:32.797987 burst2safe-0.3.5/tests/test_data/ipf/
+-rw-r--r--   0 runner    (1001) docker     (127)  5647017 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/test_data/ipf/S1A_IW_SLC__1SDV_20150117T170523_20150117T170551_004214_0051E7_AE35_VV.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  6067536 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/test_data/ipf/S1A_IW_SLC__1SDV_20150622T170528_20150622T170556_006489_0089B0_EFBC_VV.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  6114849 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/test_data/ipf/S1A_IW_SLC__1SDV_20160124T170510_20160124T170538_009639_00E0BA_7CC5_VV.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  6350843 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/test_data/ipf/S1A_IW_SLC__1SDV_20211223T170557_20211223T170624_041139_04E360_B8E2_VV.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  6564579 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/test_data/ipf/S1A_IW_SLC__1SDV_20240130T170606_20240130T170634_052339_065425_9A35_VV.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  6345069 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/test_data/ipf/S1B_IW_SLC__1SDV_20180507T170449_20180507T170517_010818_013C70_6B12_VV.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    36523 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/test_data/manifest_7C85.safe
+-rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/test_golden.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/test_ipf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/test_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/test_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/test_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/test_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/test_rfi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5861 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/test_safe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/test_swath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-05-16 14:26:27.000000 burst2safe-0.3.5/tests/test_utils.py
```

### Comparing `burst2safe-0.3.4/.github/workflows/build-and-deploy-test.yml` & `burst2safe-0.3.5/.github/workflows/build-and-deploy-test.yml`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/.github/workflows/build-and-deploy.yml` & `burst2safe-0.3.5/.github/workflows/build-and-deploy.yml`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/.github/workflows/pytest-golden.yml` & `burst2safe-0.3.5/.github/workflows/pytest-golden.yml`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/.github/workflows/pytest-integration.yml` & `burst2safe-0.3.5/.github/workflows/pytest-integration.yml`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/.github/workflows/pytest.yml` & `burst2safe-0.3.5/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/.github/workflows/static-analysis.yml` & `burst2safe-0.3.5/.github/workflows/static-analysis.yml`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/.gitignore` & `burst2safe-0.3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/CHANGELOG.md` & `burst2safe-0.3.5/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,23 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [PEP 440](https://www.python.org/dev/peps/pep-0440/)
 and uses [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.3.5]
+
+### Fixed
+* Polarization code now accurately reflects bursts contained in SAFE.
+* Measurement GeoTiff metadata now correctly specifies Sentinel-1 A or B.
+
+### Added
+* CLI argument for specifying output directory.
+
 ## [0.3.4]
 
 ### Added
 * Separate check of Earthdata credentials prior to download.
 
 ## [0.3.3]
```

### Comparing `burst2safe-0.3.4/LICENSE` & `burst2safe-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/PKG-INFO` & `burst2safe-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: burst2safe
-Version: 0.3.4
+Version: 0.3.5
 Summary: A package for converting ASF-derived Sentinel-1 burst SLC products to the ESA SAFE format
 Author-email: Forrest Williams <ffwilliams2@alaska.edu>
 Project-URL: Homepage, https://github.com/forrestfwilliams/burst2safe
 Project-URL: Bug Tracker, https://github.com/forrestfwilliams/burst2safe/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `burst2safe-0.3.4/README.md` & `burst2safe-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/pyproject.toml` & `burst2safe-0.3.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/src/burst2safe/auth.py` & `burst2safe-0.3.5/src/burst2safe/auth.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/src/burst2safe/base.py` & `burst2safe-0.3.5/src/burst2safe/base.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/src/burst2safe/burst2safe.py` & `burst2safe-0.3.5/src/burst2safe/burst2safe.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 from typing import Iterable, List, Optional
 
 import asf_search
 from asf_search.Products.S1BurstProduct import S1BurstProduct
 from shapely import box
 from shapely.geometry import Polygon
 
+from burst2safe.auth import get_earthdata_credentials
 from burst2safe.safe import Safe
 from burst2safe.utils import BurstInfo, download_url_with_retries, get_burst_infos, optional_wd
-from burst2safe.auth import get_earthdata_credentials
 
 
 warnings.filterwarnings('ignore')
 
 DESCRIPTION = """Convert a set of ASF burst SLCs to the ESA SAFE format.
 You can either provide a list of burst granules, or define a burst group by
 providing the absolute orbit number, starting burst ID, ending burst ID, swaths,
@@ -163,22 +163,24 @@
 
 def main() -> None:
     parser = ArgumentParser(description=DESCRIPTION)
     parser.add_argument('granules', nargs='*', help='A list of bursts to convert to SAFE')
     parser.add_argument('--orbit', type=int, help='The absolute orbit number of the bursts')
     parser.add_argument('--bbox', type=float, nargs=4, help='Bounding box of the bursts (W S E N in lat/lon)')
     parser.add_argument('--pols', type=str, nargs='+', help='The polarizations of the bursts (i.e., VV VH)')
+    parser.add_argument('--output-dir', type=str, default=None, help='Output directory to save to')
     parser.add_argument('--keep-files', action='store_true', default=False, help='Keep the intermediate files')
     args = parser.parse_args()
 
     if args.bbox:
         args.bbox = box(*args.bbox)
     if args.pols:
         args.pols = [pol.upper() for pol in args.pols]
 
     burst2safe(
         granules=args.granules,
         orbit=args.orbit,
         footprint=args.bbox,
         polarizations=args.pols,
         keep_files=args.keep_files,
+        work_dir=args.output_dir,
     )
```

### Comparing `burst2safe-0.3.4/src/burst2safe/calibration.py` & `burst2safe-0.3.5/src/burst2safe/calibration.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/src/burst2safe/data/support_236/s1-level-1-calibration.xsd` & `burst2safe-0.3.5/src/burst2safe/data/support_236/s1-level-1-calibration.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/src/burst2safe/data/support_236/s1-level-1-noise.xsd` & `burst2safe-0.3.5/src/burst2safe/data/support_236/s1-level-1-noise.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/src/burst2safe/data/support_236/s1-level-1-product.xsd` & `burst2safe-0.3.5/src/burst2safe/data/support_236/s1-level-1-product.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/src/burst2safe/data/support_236/s1-object-types.xsd` & `burst2safe-0.3.5/src/burst2safe/data/support_236/s1-object-types.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/src/burst2safe/data/support_245/s1-level-1-calibration.xsd` & `burst2safe-0.3.5/src/burst2safe/data/support_245/s1-level-1-calibration.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/src/burst2safe/data/support_245/s1-level-1-noise.xsd` & `burst2safe-0.3.5/src/burst2safe/data/support_245/s1-level-1-noise.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/src/burst2safe/data/support_245/s1-level-1-product.xsd` & `burst2safe-0.3.5/src/burst2safe/data/support_245/s1-level-1-product.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/src/burst2safe/data/support_245/s1-object-types.xsd` & `burst2safe-0.3.5/src/burst2safe/data/support_245/s1-object-types.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/src/burst2safe/data/support_260/s1-level-1-calibration.xsd` & `burst2safe-0.3.5/src/burst2safe/data/support_260/s1-level-1-calibration.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/src/burst2safe/data/support_260/s1-level-1-noise.xsd` & `burst2safe-0.3.5/src/burst2safe/data/support_260/s1-level-1-noise.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/src/burst2safe/data/support_260/s1-level-1-product.xsd` & `burst2safe-0.3.5/src/burst2safe/data/support_260/s1-level-1-product.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/src/burst2safe/data/support_260/s1-object-types.xsd` & `burst2safe-0.3.5/src/burst2safe/data/support_260/s1-object-types.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/src/burst2safe/data/support_290/s1-level-1-calibration.xsd` & `burst2safe-0.3.5/src/burst2safe/data/support_290/s1-level-1-calibration.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/src/burst2safe/data/support_290/s1-level-1-noise.xsd` & `burst2safe-0.3.5/src/burst2safe/data/support_290/s1-level-1-noise.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/src/burst2safe/data/support_290/s1-level-1-product.xsd` & `burst2safe-0.3.5/src/burst2safe/data/support_290/s1-level-1-product.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/src/burst2safe/data/support_290/s1-object-types.xsd` & `burst2safe-0.3.5/src/burst2safe/data/support_290/s1-object-types.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/src/burst2safe/data/support_340/s1-level-1-calibration.xsd` & `burst2safe-0.3.5/src/burst2safe/data/support_340/s1-level-1-calibration.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/src/burst2safe/data/support_340/s1-level-1-noise.xsd` & `burst2safe-0.3.5/src/burst2safe/data/support_340/s1-level-1-noise.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/src/burst2safe/data/support_340/s1-level-1-product.xsd` & `burst2safe-0.3.5/src/burst2safe/data/support_340/s1-level-1-product.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/src/burst2safe/data/support_340/s1-level-1-rfi.xsd` & `burst2safe-0.3.5/src/burst2safe/data/support_340/s1-level-1-rfi.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/src/burst2safe/data/support_340/s1-object-types.xsd` & `burst2safe-0.3.5/src/burst2safe/data/support_340/s1-object-types.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/src/burst2safe/data/support_371/s1-level-1-calibration.xsd` & `burst2safe-0.3.5/src/burst2safe/data/support_371/s1-level-1-calibration.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/src/burst2safe/data/support_371/s1-level-1-noise.xsd` & `burst2safe-0.3.5/src/burst2safe/data/support_371/s1-level-1-noise.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/src/burst2safe/data/support_371/s1-level-1-product.xsd` & `burst2safe-0.3.5/src/burst2safe/data/support_371/s1-level-1-product.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/src/burst2safe/data/support_371/s1-level-1-rfi.xsd` & `burst2safe-0.3.5/src/burst2safe/data/support_371/s1-level-1-rfi.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/src/burst2safe/data/support_371/s1-object-types.xsd` & `burst2safe-0.3.5/src/burst2safe/data/support_371/s1-object-types.xsd`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/src/burst2safe/manifest.py` & `burst2safe-0.3.5/src/burst2safe/manifest.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/src/burst2safe/measurement.py` & `burst2safe-0.3.5/src/burst2safe/measurement.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,22 +17,24 @@
 
     def __init__(self, burst_infos: Iterable[BurstInfo], gcps: Iterable[GeoPoint], ipf_version: str, image_number: int):
         """Initialize a Measurement object.
 
         Args:
             burst_infos: A list of BurstInfo objects
             gcps: A list of GeoPoint objects
+            ipf_version: The IPF version of the measurement data
             image_number: The image number of the measurement
         """
         self.burst_infos = burst_infos
         self.gcps = gcps
         self.version = ipf_version
         self.image_number = image_number
 
         self.swath = self.burst_infos[0].swath
+        self.s1_platform = self.burst_infos[0].slc_granule[2].upper()
 
         burst_lengths = sorted(list(set([info.length for info in burst_infos])))
         if len(burst_lengths) != 1:
             raise ValueError(f'All burst are not the same length. Found {" ".join([str(x) for x in burst_lengths])}')
         self.burst_length = burst_lengths[0]
         self.total_length = self.burst_length * len(self.burst_infos)
 
@@ -96,16 +98,15 @@
         """
         gdal_gcps = [gdal.GCP(gcp.x, gcp.y, gcp.z, gcp.pixel, gcp.line) for gcp in self.gcps]
         srs = osr.SpatialReference()
         srs.ImportFromEPSG(4326)
         dataset.SetGCPs(gdal_gcps, srs.ExportToWkt())
 
         dataset.SetMetadataItem('TIFFTAG_DATETIME', self.get_time_tag())
-        # TODO make sure A/B is being set correctly.
-        dataset.SetMetadataItem('TIFFTAG_IMAGEDESCRIPTION', 'Sentinel-1A IW SLC L1')
+        dataset.SetMetadataItem('TIFFTAG_IMAGEDESCRIPTION', f'Sentinel-1{self.s1_platform} IW SLC L1')
         dataset.SetMetadataItem('TIFFTAG_SOFTWARE', f'Sentinel-1 IPF {self.version}')
 
     def create_geotiff(self, out_path: Path, update_info=True):
         """Create a GeoTIFF of SLC data from the constituent burst SLC GeoTIFFs.
         Optionally update Measurment metadata.
 
         Args:
```

### Comparing `burst2safe-0.3.4/src/burst2safe/noise.py` & `burst2safe-0.3.5/src/burst2safe/noise.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/src/burst2safe/product.py` & `burst2safe-0.3.5/src/burst2safe/product.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/src/burst2safe/rfi.py` & `burst2safe-0.3.5/src/burst2safe/rfi.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/src/burst2safe/safe.py` & `burst2safe-0.3.5/src/burst2safe/safe.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         """
         self.burst_infos = burst_infos
         self.work_dir = optional_wd(work_dir)
 
         self.check_group_validity(self.burst_infos)
 
         self.grouped_burst_infos = self.group_burst_infos(self.burst_infos)
-        self.name = self.get_name(self.burst_infos)
+        self.name = self.get_name()
         self.safe_path = self.work_dir / self.name
         self.swaths = []
         self.manifest = None
 
         self.version = self.get_ipf_version(self.burst_infos[0].metadata_path)
         self.major_version, self.minor_version = [int(x) for x in self.version.split('.')]
         self.support_dir = self.get_support_dir()
@@ -97,31 +97,36 @@
             min_diff = burst_range[swath1][working_pol][0] - burst_range[swath2][working_pol][0]
             if np.abs(min_diff) > 1:
                 raise ValueError(f'Products from swaths {swath1} and {swath2} do not overlap')
             max_diff = burst_range[swath1][working_pol][1] - burst_range[swath2][working_pol][1]
             if np.abs(max_diff) > 1:
                 raise ValueError(f'Products from swaths {swath1} and {swath2} do not overlap')
 
-    @staticmethod
-    def get_name(burst_infos: Iterable[BurstInfo], unique_id: str = '0000') -> str:
+    def get_name(self, unique_id: str = '0000') -> str:
         """Create a name for the SAFE file.
 
         Args:
             burst_infos: A list of BurstInfo objects
             unique_id: A unique identifier for the SAFE file
 
         Returns:
             The name of the SAFE file
         """
-        platform, beam_mode, product_type = burst_infos[0].slc_granule.split('_')[:3]
-        product_info = f'1SS{burst_infos[0].polarization[0]}'
-        min_date = min([x.date for x in burst_infos]).strftime('%Y%m%dT%H%M%S')
-        max_date = max([x.date for x in burst_infos]).strftime('%Y%m%dT%H%M%S')
-        absolute_orbit = f'{burst_infos[0].absolute_orbit:06d}'
-        mission_data_take = burst_infos[0].slc_granule.split('_')[-2]
+
+        platform, beam_mode, product_type = self.burst_infos[0].slc_granule.split('_')[:3]
+
+        pol_codes = {'HH': 'SH', 'VV': 'SV', 'HH_HV': 'DH', 'VH_VV': 'DV'}
+        pols = sorted(list(set([x.polarization for x in self.burst_infos])))
+        pol_code = pol_codes['_'.join(pols)]
+        product_info = f'1S{pol_code}'
+
+        min_date = min([x.date for x in self.burst_infos]).strftime('%Y%m%dT%H%M%S')
+        max_date = max([x.date for x in self.burst_infos]).strftime('%Y%m%dT%H%M%S')
+        absolute_orbit = f'{self.burst_infos[0].absolute_orbit:06d}'
+        mission_data_take = self.burst_infos[0].slc_granule.split('_')[-2]
         product_name = f'{platform}_{beam_mode}_{product_type}__{product_info}_{min_date}_{max_date}_{absolute_orbit}_{mission_data_take}_{unique_id}.SAFE'
         return product_name
 
     @staticmethod
     def group_burst_infos(burst_infos: Iterable[BurstInfo]) -> dict:
         """Group burst infos by swath and polarization.
 
@@ -228,15 +233,15 @@
         manifest = Manifest(content_units, metadata_objects, data_objects, self.get_bbox(), template_manifest)
         manifest.assemble()
         manifest.write(manifest_name)
         self.manifest = manifest
 
     def update_product_identifier(self):
         """Update the product identifier using the CRC of the manifest file."""
-        new_new = self.get_name(self.burst_infos, unique_id=self.manifest.crc)
+        new_new = self.get_name(unique_id=self.manifest.crc)
         new_path = self.work_dir / new_new
         if new_path.exists():
             shutil.rmtree(new_path)
         shutil.move(self.safe_path, new_path)
         self.name = new_new
         self.safe_path = new_path
         for swath in self.swaths:
```

### Comparing `burst2safe-0.3.4/src/burst2safe/swath.py` & `burst2safe-0.3.5/src/burst2safe/swath.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/src/burst2safe/utils.py` & `burst2safe-0.3.5/src/burst2safe/utils.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/src/burst2safe.egg-info/PKG-INFO` & `burst2safe-0.3.5/src/burst2safe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: burst2safe
-Version: 0.3.4
+Version: 0.3.5
 Summary: A package for converting ASF-derived Sentinel-1 burst SLC products to the ESA SAFE format
 Author-email: Forrest Williams <ffwilliams2@alaska.edu>
 Project-URL: Homepage, https://github.com/forrestfwilliams/burst2safe
 Project-URL: Bug Tracker, https://github.com/forrestfwilliams/burst2safe/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `burst2safe-0.3.4/src/burst2safe.egg-info/SOURCES.txt` & `burst2safe-0.3.5/src/burst2safe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/tests/conftest.py` & `burst2safe-0.3.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/tests/etc/identify_ipf_differences.py` & `burst2safe-0.3.5/tests/etc/identify_ipf_differences.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/tests/helpers.py` & `burst2safe-0.3.5/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/tests/test_auth.py` & `burst2safe-0.3.5/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/tests/test_base.py` & `burst2safe-0.3.5/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/tests/test_data/S1A_IW_SLC__1SDV_20240408T015045_20240408T015113_053336_06778C_CB5D_VV.xml` & `burst2safe-0.3.5/tests/test_data/S1A_IW_SLC__1SDV_20240408T015045_20240408T015113_053336_06778C_CB5D_VV.xml`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/tests/test_data/S1A_IW_SLC__1SDV_20240408T015111_20240408T015138_053336_06778C_CA9A_VV.xml` & `burst2safe-0.3.5/tests/test_data/S1A_IW_SLC__1SDV_20240408T015111_20240408T015138_053336_06778C_CA9A_VV.xml`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/tests/test_data/ipf/S1A_IW_SLC__1SDV_20150117T170523_20150117T170551_004214_0051E7_AE35_VV.xml` & `burst2safe-0.3.5/tests/test_data/ipf/S1A_IW_SLC__1SDV_20150117T170523_20150117T170551_004214_0051E7_AE35_VV.xml`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/tests/test_data/ipf/S1A_IW_SLC__1SDV_20150622T170528_20150622T170556_006489_0089B0_EFBC_VV.xml` & `burst2safe-0.3.5/tests/test_data/ipf/S1A_IW_SLC__1SDV_20150622T170528_20150622T170556_006489_0089B0_EFBC_VV.xml`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/tests/test_data/ipf/S1A_IW_SLC__1SDV_20160124T170510_20160124T170538_009639_00E0BA_7CC5_VV.xml` & `burst2safe-0.3.5/tests/test_data/ipf/S1A_IW_SLC__1SDV_20160124T170510_20160124T170538_009639_00E0BA_7CC5_VV.xml`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/tests/test_data/ipf/S1A_IW_SLC__1SDV_20211223T170557_20211223T170624_041139_04E360_B8E2_VV.xml` & `burst2safe-0.3.5/tests/test_data/ipf/S1A_IW_SLC__1SDV_20211223T170557_20211223T170624_041139_04E360_B8E2_VV.xml`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/tests/test_data/ipf/S1A_IW_SLC__1SDV_20240130T170606_20240130T170634_052339_065425_9A35_VV.xml` & `burst2safe-0.3.5/tests/test_data/ipf/S1A_IW_SLC__1SDV_20240130T170606_20240130T170634_052339_065425_9A35_VV.xml`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/tests/test_data/ipf/S1B_IW_SLC__1SDV_20180507T170449_20180507T170517_010818_013C70_6B12_VV.xml` & `burst2safe-0.3.5/tests/test_data/ipf/S1B_IW_SLC__1SDV_20180507T170449_20180507T170517_010818_013C70_6B12_VV.xml`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/tests/test_data/manifest_7C85.safe` & `burst2safe-0.3.5/tests/test_data/manifest_7C85.safe`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/tests/test_golden.py` & `burst2safe-0.3.5/tests/test_golden.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/tests/test_ipf.py` & `burst2safe-0.3.5/tests/test_ipf.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/tests/test_manifest.py` & `burst2safe-0.3.5/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/tests/test_measurement.py` & `burst2safe-0.3.5/tests/test_measurement.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/tests/test_noise.py` & `burst2safe-0.3.5/tests/test_noise.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/tests/test_product.py` & `burst2safe-0.3.5/tests/test_product.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/tests/test_swath.py` & `burst2safe-0.3.5/tests/test_swath.py`

 * *Files identical despite different names*

### Comparing `burst2safe-0.3.4/tests/test_utils.py` & `burst2safe-0.3.5/tests/test_utils.py`

 * *Files identical despite different names*

