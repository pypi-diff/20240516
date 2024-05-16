# Comparing `tmp/aopp_deconv_tool-0.1.8.tar.gz` & `tmp/aopp_deconv_tool-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aopp_deconv_tool-0.1.8.tar", last modified: Thu Apr 18 14:40:03 2024, max compression
+gzip compressed data, was "aopp_deconv_tool-0.1.9.tar", last modified: Tue Apr 23 13:24:27 2024, max compression
```

## Comparing `aopp_deconv_tool-0.1.8.tar` & `aopp_deconv_tool-0.1.9.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-18 14:40:03.743302 aopp_deconv_tool-0.1.8/
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)       12 2024-04-15 11:59:42.000000 aopp_deconv_tool-0.1.8/MANIFEST.in
--rw-r--r--   0 dobinsonl  (1001) dobinsonl  (1002)    11824 2024-04-18 14:40:03.743302 aopp_deconv_tool-0.1.8/PKG-INFO
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)    17376 2024-04-15 12:48:17.000000 aopp_deconv_tool-0.1.8/README.md
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)    10776 2024-04-18 14:37:53.000000 aopp_deconv_tool-0.1.8/USAGE.md
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     1366 2024-04-18 14:39:55.000000 aopp_deconv_tool-0.1.8/pyproject.toml
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)       38 2024-04-18 14:40:03.743302 aopp_deconv_tool-0.1.8/setup.cfg
-drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-18 14:40:03.731302 aopp_deconv_tool-0.1.8/src/
-drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-18 14:40:03.735302 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-15 11:42:19.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/__init__.py
-drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-18 14:40:03.735302 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/algorithm/
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)        2 2023-09-13 10:17:41.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/algorithm/__init__.py
-drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-18 14:40:03.735302 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/algorithm/bad_pixels/
--rw-r--r--   0 dobinsonl  (1001) dobinsonl  (1002)      757 2024-04-11 11:09:47.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/algorithm/bad_pixels/__init__.py
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)    10563 2024-04-11 11:10:24.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/algorithm/bad_pixels/ssa_sum_prob.py
-drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-18 14:40:03.739302 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/algorithm/deconv/
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)        2 2023-09-13 10:17:33.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/algorithm/deconv/__init__.py
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     6484 2024-04-11 11:10:48.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/algorithm/deconv/base.py
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)    13868 2024-04-16 14:31:28.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/algorithm/deconv/clean_modified.py
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     7629 2024-04-11 11:11:20.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/algorithm/deconv/lucy_richardson.py
-drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-18 14:40:03.739302 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/algorithm/interpolate/
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-03-06 14:06:01.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/algorithm/interpolate/__init__.py
--rw-r--r--   0 dobinsonl  (1001) dobinsonl  (1002)     3309 2024-04-16 14:41:10.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/algorithm/interpolate/ssa_interp.py
-drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-18 14:40:03.739302 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/astropy_helper/
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)        0 2023-09-14 14:46:22.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/astropy_helper/__init__.py
-drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-18 14:40:03.739302 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/astropy_helper/fits/
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)        0 2023-09-14 14:47:01.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/astropy_helper/fits/__init_.py
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     4327 2024-04-16 14:02:00.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/astropy_helper/fits/header.py
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     6984 2024-04-16 14:01:32.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/astropy_helper/fits/specifier.py
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     1149 2024-03-21 13:51:28.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/cast.py
-drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-18 14:40:03.739302 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/cfg/
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)       38 2023-09-26 10:28:06.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/cfg/__init__.py
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     1750 2024-04-08 13:36:09.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/cfg/logs.py
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)       33 2023-09-26 10:36:39.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/cfg/settings.py
-drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-18 14:40:03.739302 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/context/
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)        0 2023-09-13 12:51:00.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/context/__init__.py
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)      361 2024-03-06 11:08:00.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/context/alias.py
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)      487 2024-03-06 11:09:24.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/context/next.py
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)      739 2023-09-13 12:59:11.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/context/temp.py
-drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-18 14:40:03.739302 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/data_structures/
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)       50 2024-01-11 16:49:39.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/data_structures/__init__.py
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     1446 2024-01-11 16:48:15.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/data_structures/bi_directional_map.py
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)      861 2024-03-19 14:41:28.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/data_structures/pointer.py
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     9365 2024-04-17 12:35:17.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/deconvolve.py
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     1088 2024-04-17 10:31:00.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/estimate_noise.py
--rw-r--r--   0 dobinsonl  (1001) dobinsonl  (1002)     1474 2024-04-17 10:34:56.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/gaussian_psf_model.py
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     3869 2024-04-17 10:41:37.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/geo_array.py
-drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-18 14:40:03.739302 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/geometry/
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)      397 2023-10-09 13:17:50.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/geometry/__init__.py
--rw-r--r--   0 dobinsonl  (1001) dobinsonl  (1002)     2366 2024-04-11 11:01:06.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/geometry/bounding_box.py
-drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-18 14:40:03.739302 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/geometry/shape/
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     1747 2024-04-11 11:00:55.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/geometry/shape/__init__.py
-drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-18 14:40:03.739302 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/graphical_frontends/
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-03-11 11:21:30.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/graphical_frontends/__init__.py
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)    32684 2024-04-18 14:38:58.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/graphical_frontends/ssa_filtering.py
-drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-18 14:40:03.739302 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/image_processing/
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)        0 2023-09-11 14:31:16.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/image_processing/__init__.py
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     6556 2024-04-17 10:57:17.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/image_processing/otsu_thresholding.py
-drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-18 14:40:03.739302 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/instrument_model/
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     1060 2024-04-11 11:02:18.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/instrument_model/instrument_base.py
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     1983 2024-04-11 11:02:36.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/instrument_model/vlt.py
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     4089 2024-03-21 14:01:25.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/mfunc.py
-drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-18 14:40:03.739302 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/numpy_helper/
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)        0 2023-10-04 13:04:06.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/numpy_helper/__init__.py
-drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-18 14:40:03.743302 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/numpy_helper/array/
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     4000 2024-04-11 11:03:12.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/numpy_helper/array/__init__.py
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     2034 2024-04-11 11:03:22.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/numpy_helper/array/index.py
-drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-18 14:40:03.743302 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/numpy_helper/array/mask/
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     1294 2024-04-11 11:02:50.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/numpy_helper/array/mask/__init__.py
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     5681 2024-04-11 11:03:04.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/numpy_helper/array/mask/interp.py
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)      705 2024-04-11 11:03:29.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/numpy_helper/array/pad.py
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     2261 2024-04-11 11:03:43.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/numpy_helper/array/shift.py
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     3990 2024-04-17 11:00:02.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/numpy_helper/axes.py
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     3883 2024-04-17 11:04:29.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/numpy_helper/slice.py
-drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-18 14:40:03.743302 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/optics/
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)      860 2024-04-11 11:04:31.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/optics/adaptive_optics_model.py
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     1592 2024-04-11 11:04:41.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/optics/function.py
-drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-18 14:40:03.743302 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/optics/geometric/
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     4080 2023-10-23 09:49:35.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/optics/geometric/light_beam.py
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)    13939 2024-04-11 11:04:26.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/optics/geometric/optical_component.py
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     2030 2024-04-17 11:05:46.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/optics/telescope_model.py
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     2032 2024-04-11 11:05:27.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/optics/turbulence_model.py
-drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-18 14:40:03.743302 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/optimise_compat/
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)    14378 2024-04-11 11:05:42.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/optimise_compat/__init__.py
--rw-r--r--   0 dobinsonl  (1001) dobinsonl  (1002)    12087 2024-04-11 11:06:11.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/optimise_compat/ultranest_compat.py
-drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-18 14:40:03.743302 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/plot_helper/
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     7321 2024-04-17 11:08:23.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/plot_helper/__init__.py
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     5991 2024-04-17 11:15:09.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/plot_helper/base.py
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     9432 2024-04-17 11:15:11.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/plot_helper/plotters.py
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     8334 2024-04-11 11:34:16.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/psf_data_ops.py
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)    14295 2024-04-17 10:43:06.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/psf_model.py
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)    13370 2024-04-16 14:43:34.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/psf_model_dependency_injector.py
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)    23784 2024-04-11 11:25:28.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/py_ssa.py
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     5389 2024-04-11 11:09:13.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/py_svd.py
--rw-r--r--   0 dobinsonl  (1001) dobinsonl  (1002)     1191 2024-01-26 11:13:05.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/radial_psf_model.py
-drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-18 14:40:03.743302 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/scipy_helper/
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-03-06 12:11:00.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/scipy_helper/__init__.py
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     2137 2024-03-06 12:13:49.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/scipy_helper/interp.py
-drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-18 14:40:03.743302 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/stats/
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-03-06 11:14:11.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/stats/__init__.py
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     1887 2024-04-17 11:15:10.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/stats/empirical.py
-drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-18 14:40:03.743302 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/text/
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     2484 2024-04-16 14:03:00.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/text/__init__.py
--rw-r--r--   0 dobinsonl  (1001) dobinsonl  (1002)     2781 2024-04-17 10:44:35.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/turbulence_psf_model.py
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)      247 2024-04-05 11:04:15.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/typedef.py
-drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-18 14:40:03.743302 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool.egg-info/
--rw-r--r--   0 dobinsonl  (1001) dobinsonl  (1002)    11824 2024-04-18 14:40:03.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool.egg-info/PKG-INFO
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     3550 2024-04-18 14:40:03.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool.egg-info/SOURCES.txt
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)        1 2024-04-18 14:40:03.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool.egg-info/dependency_links.txt
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)       59 2024-04-18 14:40:03.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool.egg-info/requires.txt
--rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)       17 2024-04-18 14:40:03.000000 aopp_deconv_tool-0.1.8/src/aopp_deconv_tool.egg-info/top_level.txt
+drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-23 13:24:27.734518 aopp_deconv_tool-0.1.9/
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)       12 2024-04-15 11:59:42.000000 aopp_deconv_tool-0.1.9/MANIFEST.in
+-rw-r--r--   0 dobinsonl  (1001) dobinsonl  (1002)    20865 2024-04-23 13:24:27.734518 aopp_deconv_tool-0.1.9/PKG-INFO
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)    17376 2024-04-15 12:48:17.000000 aopp_deconv_tool-0.1.9/README.md
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)    19817 2024-04-23 13:23:34.000000 aopp_deconv_tool-0.1.9/USAGE.md
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     1366 2024-04-23 13:24:23.000000 aopp_deconv_tool-0.1.9/pyproject.toml
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)       38 2024-04-23 13:24:27.734518 aopp_deconv_tool-0.1.9/setup.cfg
+drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-23 13:24:27.722518 aopp_deconv_tool-0.1.9/src/
+drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-23 13:24:27.726518 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-15 11:42:19.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/__init__.py
+drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-23 13:24:27.726518 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/algorithm/
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)        2 2023-09-13 10:17:41.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/algorithm/__init__.py
+drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-23 13:24:27.726518 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/algorithm/bad_pixels/
+-rw-r--r--   0 dobinsonl  (1001) dobinsonl  (1002)      757 2024-04-11 11:09:47.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/algorithm/bad_pixels/__init__.py
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)    10563 2024-04-11 11:10:24.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/algorithm/bad_pixels/ssa_sum_prob.py
+drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-23 13:24:27.726518 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/algorithm/deconv/
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)        2 2023-09-13 10:17:33.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/algorithm/deconv/__init__.py
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     6484 2024-04-11 11:10:48.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/algorithm/deconv/base.py
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)    13868 2024-04-16 14:31:28.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/algorithm/deconv/clean_modified.py
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     7629 2024-04-11 11:11:20.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/algorithm/deconv/lucy_richardson.py
+drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-23 13:24:27.726518 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/algorithm/interpolate/
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-03-06 14:06:01.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/algorithm/interpolate/__init__.py
+-rw-r--r--   0 dobinsonl  (1001) dobinsonl  (1002)     3309 2024-04-16 14:41:10.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/algorithm/interpolate/ssa_interp.py
+drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-23 13:24:27.726518 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/astropy_helper/
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)        0 2023-09-14 14:46:22.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/astropy_helper/__init__.py
+drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-23 13:24:27.726518 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/astropy_helper/fits/
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)        0 2023-09-14 14:47:01.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/astropy_helper/fits/__init_.py
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     4327 2024-04-16 14:02:00.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/astropy_helper/fits/header.py
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     6984 2024-04-16 14:01:32.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/astropy_helper/fits/specifier.py
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     1149 2024-03-21 13:51:28.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/cast.py
+drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-23 13:24:27.730518 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/cfg/
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)       38 2023-09-26 10:28:06.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/cfg/__init__.py
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     1750 2024-04-08 13:36:09.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/cfg/logs.py
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)       33 2023-09-26 10:36:39.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/cfg/settings.py
+drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-23 13:24:27.730518 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/context/
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)        0 2023-09-13 12:51:00.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/context/__init__.py
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)      361 2024-03-06 11:08:00.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/context/alias.py
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)      487 2024-03-06 11:09:24.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/context/next.py
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)      739 2023-09-13 12:59:11.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/context/temp.py
+drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-23 13:24:27.730518 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/data_structures/
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)       50 2024-01-11 16:49:39.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/data_structures/__init__.py
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     1446 2024-01-11 16:48:15.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/data_structures/bi_directional_map.py
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)      861 2024-03-19 14:41:28.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/data_structures/pointer.py
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     9365 2024-04-17 12:35:17.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/deconvolve.py
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     1088 2024-04-17 10:31:00.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/estimate_noise.py
+-rw-r--r--   0 dobinsonl  (1001) dobinsonl  (1002)     1474 2024-04-17 10:34:56.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/gaussian_psf_model.py
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     3869 2024-04-17 10:41:37.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/geo_array.py
+drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-23 13:24:27.730518 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/geometry/
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)      397 2023-10-09 13:17:50.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/geometry/__init__.py
+-rw-r--r--   0 dobinsonl  (1001) dobinsonl  (1002)     2366 2024-04-11 11:01:06.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/geometry/bounding_box.py
+drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-23 13:24:27.730518 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/geometry/shape/
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     1747 2024-04-11 11:00:55.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/geometry/shape/__init__.py
+drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-23 13:24:27.730518 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/graphical_frontends/
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-03-11 11:21:30.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/graphical_frontends/__init__.py
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)    32684 2024-04-18 14:38:58.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/graphical_frontends/ssa_filtering.py
+drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-23 13:24:27.730518 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/image_processing/
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)        0 2023-09-11 14:31:16.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/image_processing/__init__.py
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     6556 2024-04-17 10:57:17.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/image_processing/otsu_thresholding.py
+drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-23 13:24:27.730518 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/instrument_model/
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     1060 2024-04-11 11:02:18.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/instrument_model/instrument_base.py
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     1983 2024-04-11 11:02:36.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/instrument_model/vlt.py
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     4089 2024-03-21 14:01:25.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/mfunc.py
+drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-23 13:24:27.730518 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/numpy_helper/
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)        0 2023-10-04 13:04:06.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/numpy_helper/__init__.py
+drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-23 13:24:27.730518 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/numpy_helper/array/
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     4000 2024-04-11 11:03:12.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/numpy_helper/array/__init__.py
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     2034 2024-04-11 11:03:22.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/numpy_helper/array/index.py
+drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-23 13:24:27.730518 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/numpy_helper/array/mask/
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     1294 2024-04-11 11:02:50.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/numpy_helper/array/mask/__init__.py
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     5681 2024-04-11 11:03:04.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/numpy_helper/array/mask/interp.py
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)      705 2024-04-11 11:03:29.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/numpy_helper/array/pad.py
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     2261 2024-04-11 11:03:43.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/numpy_helper/array/shift.py
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     3990 2024-04-17 11:00:02.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/numpy_helper/axes.py
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     3883 2024-04-17 11:04:29.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/numpy_helper/slice.py
+drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-23 13:24:27.730518 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/optics/
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)      860 2024-04-11 11:04:31.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/optics/adaptive_optics_model.py
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     1592 2024-04-11 11:04:41.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/optics/function.py
+drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-23 13:24:27.730518 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/optics/geometric/
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     4080 2023-10-23 09:49:35.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/optics/geometric/light_beam.py
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)    13939 2024-04-11 11:04:26.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/optics/geometric/optical_component.py
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     2030 2024-04-17 11:05:46.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/optics/telescope_model.py
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     2032 2024-04-11 11:05:27.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/optics/turbulence_model.py
+drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-23 13:24:27.730518 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/optimise_compat/
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)    14378 2024-04-11 11:05:42.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/optimise_compat/__init__.py
+-rw-r--r--   0 dobinsonl  (1001) dobinsonl  (1002)    12087 2024-04-11 11:06:11.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/optimise_compat/ultranest_compat.py
+drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-23 13:24:27.730518 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/plot_helper/
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     7321 2024-04-17 11:08:23.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/plot_helper/__init__.py
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     5991 2024-04-17 11:15:09.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/plot_helper/base.py
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     9432 2024-04-17 11:15:11.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/plot_helper/plotters.py
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     8334 2024-04-11 11:34:16.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/psf_data_ops.py
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)    14295 2024-04-17 10:43:06.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/psf_model.py
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)    13370 2024-04-16 14:43:34.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/psf_model_dependency_injector.py
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)    23784 2024-04-11 11:25:28.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/py_ssa.py
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     5389 2024-04-11 11:09:13.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/py_svd.py
+-rw-r--r--   0 dobinsonl  (1001) dobinsonl  (1002)     1191 2024-01-26 11:13:05.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/radial_psf_model.py
+drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-23 13:24:27.734518 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/scipy_helper/
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-03-06 12:11:00.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/scipy_helper/__init__.py
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     2137 2024-03-06 12:13:49.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/scipy_helper/interp.py
+drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-23 13:24:27.734518 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/stats/
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-03-06 11:14:11.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/stats/__init__.py
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     1887 2024-04-17 11:15:10.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/stats/empirical.py
+drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-23 13:24:27.734518 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/text/
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     2484 2024-04-16 14:03:00.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/text/__init__.py
+-rw-r--r--   0 dobinsonl  (1001) dobinsonl  (1002)     2781 2024-04-17 10:44:35.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/turbulence_psf_model.py
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)      247 2024-04-05 11:04:15.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/typedef.py
+drwxrwxr-x   0 dobinsonl  (1001) dobinsonl  (1002)        0 2024-04-23 13:24:27.734518 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool.egg-info/
+-rw-r--r--   0 dobinsonl  (1001) dobinsonl  (1002)    20865 2024-04-23 13:24:27.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool.egg-info/PKG-INFO
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)     3550 2024-04-23 13:24:27.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool.egg-info/SOURCES.txt
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)        1 2024-04-23 13:24:27.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool.egg-info/dependency_links.txt
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)       59 2024-04-23 13:24:27.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool.egg-info/requires.txt
+-rw-rw-r--   0 dobinsonl  (1001) dobinsonl  (1002)       17 2024-04-23 13:24:27.000000 aopp_deconv_tool-0.1.9/src/aopp_deconv_tool.egg-info/top_level.txt
```

### Comparing `aopp_deconv_tool-0.1.8/README.md` & `aopp_deconv_tool-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/pyproject.toml` & `aopp_deconv_tool-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aopp_deconv_tool"
-version = "0.1.8" # Increment this whenever we upload a new version to Pypi (or the test pypi).
+version = "0.1.9" # Increment this whenever we upload a new version to Pypi (or the test pypi).
 dependencies = [
 	"numpy",
 	"astropy",
 	"scipy",
 	"matplotlib",
 	"ultranest",
 	"h5py",
```

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/algorithm/bad_pixels/__init__.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/algorithm/bad_pixels/__init__.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/algorithm/bad_pixels/ssa_sum_prob.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/algorithm/bad_pixels/ssa_sum_prob.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/algorithm/deconv/base.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/algorithm/deconv/base.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/algorithm/deconv/clean_modified.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/algorithm/deconv/clean_modified.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/algorithm/deconv/lucy_richardson.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/algorithm/deconv/lucy_richardson.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/algorithm/interpolate/ssa_interp.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/algorithm/interpolate/ssa_interp.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/astropy_helper/fits/header.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/astropy_helper/fits/header.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/astropy_helper/fits/specifier.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/astropy_helper/fits/specifier.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/cast.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/cast.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/cfg/logs.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/cfg/logs.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/context/temp.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/context/temp.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/data_structures/bi_directional_map.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/data_structures/bi_directional_map.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/data_structures/pointer.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/data_structures/pointer.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/deconvolve.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/deconvolve.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/estimate_noise.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/estimate_noise.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/gaussian_psf_model.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/gaussian_psf_model.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/geo_array.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/geo_array.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/geometry/bounding_box.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/geometry/bounding_box.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/geometry/shape/__init__.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/geometry/shape/__init__.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/graphical_frontends/ssa_filtering.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/graphical_frontends/ssa_filtering.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/image_processing/otsu_thresholding.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/image_processing/otsu_thresholding.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/instrument_model/instrument_base.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/instrument_model/instrument_base.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/instrument_model/vlt.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/instrument_model/vlt.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/mfunc.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/mfunc.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/numpy_helper/array/__init__.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/numpy_helper/array/__init__.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/numpy_helper/array/index.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/numpy_helper/array/index.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/numpy_helper/array/mask/__init__.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/numpy_helper/array/mask/__init__.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/numpy_helper/array/mask/interp.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/numpy_helper/array/mask/interp.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/numpy_helper/array/pad.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/numpy_helper/array/pad.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/numpy_helper/array/shift.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/numpy_helper/array/shift.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/numpy_helper/axes.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/numpy_helper/axes.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/numpy_helper/slice.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/numpy_helper/slice.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/optics/adaptive_optics_model.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/optics/adaptive_optics_model.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/optics/function.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/optics/function.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/optics/geometric/light_beam.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/optics/geometric/light_beam.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/optics/geometric/optical_component.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/optics/geometric/optical_component.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/optics/telescope_model.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/optics/telescope_model.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/optics/turbulence_model.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/optics/turbulence_model.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/optimise_compat/__init__.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/optimise_compat/__init__.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/optimise_compat/ultranest_compat.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/optimise_compat/ultranest_compat.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/plot_helper/__init__.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/plot_helper/__init__.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/plot_helper/base.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/plot_helper/base.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/plot_helper/plotters.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/plot_helper/plotters.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/psf_data_ops.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/psf_data_ops.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/psf_model.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/psf_model.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/psf_model_dependency_injector.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/psf_model_dependency_injector.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/py_ssa.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/py_ssa.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/py_svd.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/py_svd.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/radial_psf_model.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/radial_psf_model.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/scipy_helper/interp.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/scipy_helper/interp.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/stats/empirical.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/stats/empirical.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/text/__init__.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/text/__init__.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool/turbulence_psf_model.py` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool/turbulence_psf_model.py`

 * *Files identical despite different names*

### Comparing `aopp_deconv_tool-0.1.8/src/aopp_deconv_tool.egg-info/SOURCES.txt` & `aopp_deconv_tool-0.1.9/src/aopp_deconv_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

