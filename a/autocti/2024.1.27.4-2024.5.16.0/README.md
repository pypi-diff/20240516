# Comparing `tmp/autocti-2024.1.27.4.tar.gz` & `tmp/autocti-2024.5.16.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autocti-2024.1.27.4.tar", last modified: Sat Jan 27 19:56:41 2024, max compression
+gzip compressed data, was "autocti-2024.5.16.0.tar", last modified: Thu May 16 09:59:21 2024, max compression
```

## Comparing `autocti-2024.1.27.4.tar` & `autocti-2024.5.16.0.tar`

### file list

```diff
@@ -1,158 +1,271 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:41.743377 autocti-2024.1.27.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/CITATIONS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-01-27 19:56:41.743377 autocti-2024.1.27.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8271 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:41.727377 autocti-2024.1.27.4/autocti/
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:41.727377 autocti-2024.1.27.4/autocti/aggregator/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/aggregator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/aggregator/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/aggregator/cti.py
--rw-r--r--   0 runner    (1001) docker     (127)     6208 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/aggregator/dataset_1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/aggregator/fit_dataset_1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6999 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/aggregator/fit_imaging_ci.py
--rw-r--r--   0 runner    (1001) docker     (127)     6965 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/aggregator/imaging_ci.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:41.727377 autocti-2024.1.27.4/autocti/charge_injection/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/charge_injection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/charge_injection/ci_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/charge_injection/fit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/charge_injection/hyper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:41.727377 autocti-2024.1.27.4/autocti/charge_injection/imaging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/charge_injection/imaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13284 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/charge_injection/imaging/imaging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/charge_injection/imaging/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    10082 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/charge_injection/imaging/simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)    17201 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/charge_injection/layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/charge_injection/master.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:41.727377 autocti-2024.1.27.4/autocti/charge_injection/mock/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/charge_injection/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/charge_injection/mock/mock_result.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:41.731377 autocti-2024.1.27.4/autocti/charge_injection/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/charge_injection/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17282 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/charge_injection/model/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/charge_injection/model/result.py
--rw-r--r--   0 runner    (1001) docker     (127)    15116 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/charge_injection/model/visualizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9610 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/charge_injection/ou_sim_ci.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:41.731377 autocti-2024.1.27.4/autocti/charge_injection/plot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/charge_injection/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25316 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/charge_injection/plot/fit_ci_plotters.py
--rw-r--r--   0 runner    (1001) docker     (127)    19415 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/charge_injection/plot/imaging_ci_plotters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:41.731377 autocti-2024.1.27.4/autocti/clocker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/clocker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/clocker/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/clocker/one_d.py
--rw-r--r--   0 runner    (1001) docker     (127)    36772 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/clocker/two_d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:41.731377 autocti-2024.1.27.4/autocti/config/
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/config/general.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/config/notation.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:41.731377 autocti-2024.1.27.4/autocti/config/priors/
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/config/priors/ccd.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/config/priors/hyper.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/config/priors/traps.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/config/visualize.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:41.731377 autocti-2024.1.27.4/autocti/cosmics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/cosmics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11501 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/cosmics/cosmics.py
--rw-r--r--   0 runner    (1001) docker     (127)    41101 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/cosmics/cr_distances.py
--rw-r--r--   0 runner    (1001) docker     (127)    13590 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/cosmics/cr_lengths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:41.731377 autocti-2024.1.27.4/autocti/dataset_1d/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/dataset_1d/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:41.731377 autocti-2024.1.27.4/autocti/dataset_1d/dataset_1d/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/dataset_1d/dataset_1d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10350 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/dataset_1d/dataset_1d/dataset_1d.py
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/dataset_1d/dataset_1d/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/dataset_1d/dataset_1d/simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/dataset_1d/fit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:41.735377 autocti-2024.1.27.4/autocti/dataset_1d/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/dataset_1d/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11938 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/dataset_1d/model/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/dataset_1d/model/result.py
--rw-r--r--   0 runner    (1001) docker     (127)    12051 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/dataset_1d/model/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:41.735377 autocti-2024.1.27.4/autocti/dataset_1d/plot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/dataset_1d/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9794 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/dataset_1d/plot/dataset_1d_plotters.py
--rw-r--r--   0 runner    (1001) docker     (127)    13804 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/dataset_1d/plot/fit_plotters.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:41.735377 autocti-2024.1.27.4/autocti/extract/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/extract/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:41.735377 autocti-2024.1.27.4/autocti/extract/one_d/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/extract/one_d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7621 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/extract/one_d/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/extract/one_d/eper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/extract/one_d/fpr.py
--rw-r--r--   0 runner    (1001) docker     (127)    10366 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/extract/one_d/master.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/extract/one_d/overscan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/extract/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:41.735377 autocti-2024.1.27.4/autocti/extract/two_d/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/extract/two_d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19736 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/extract/two_d/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/extract/two_d/extract_2d_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    20389 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/extract/two_d/master.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:41.735377 autocti-2024.1.27.4/autocti/extract/two_d/parallel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/extract/two_d/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15134 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/extract/two_d/parallel/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    11608 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/extract/two_d/parallel/calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)     7164 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/extract/two_d/parallel/eper.py
--rw-r--r--   0 runner    (1001) docker     (127)     7123 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/extract/two_d/parallel/fpr.py
--rw-r--r--   0 runner    (1001) docker     (127)     4595 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/extract/two_d/parallel/overscan.py
--rw-r--r--   0 runner    (1001) docker     (127)     5472 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/extract/two_d/parallel/pedestal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/extract/two_d/parallel/pre_injection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:41.739377 autocti-2024.1.27.4/autocti/extract/two_d/serial/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/extract/two_d/serial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7765 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/extract/two_d/serial/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    10782 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/extract/two_d/serial/calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)     6160 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/extract/two_d/serial/eper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/extract/two_d/serial/fpr.py
--rw-r--r--   0 runner    (1001) docker     (127)     4595 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/extract/two_d/serial/overscan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/extract/two_d/serial/overscan_no_eper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/extract/two_d/serial/prescan.py
--rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:41.739377 autocti-2024.1.27.4/autocti/instruments/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/instruments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:41.739377 autocti-2024.1.27.4/autocti/instruments/acs/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/instruments/acs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6118 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/instruments/acs/acs_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    11226 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/instruments/acs/array_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/instruments/acs/header.py
--rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/instruments/acs/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/instruments/acs/layout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:41.739377 autocti-2024.1.27.4/autocti/instruments/euclid/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/instruments/euclid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12883 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/instruments/euclid/array_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/instruments/euclid/euclid_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/instruments/euclid/header.py
--rw-r--r--   0 runner    (1001) docker     (127)    17129 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/instruments/euclid/layout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:41.739377 autocti-2024.1.27.4/autocti/layout/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/layout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/layout/one_d.py
--rw-r--r--   0 runner    (1001) docker     (127)    11677 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/layout/two_d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:41.739377 autocti-2024.1.27.4/autocti/mask/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/mask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/mask/mask_1d.py
--rw-r--r--   0 runner    (1001) docker     (127)    16351 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/mask/mask_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:41.743377 autocti-2024.1.27.4/autocti/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/model/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/model/model_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/model/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/model/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/model/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:41.743377 autocti-2024.1.27.4/autocti/plot/
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/plot/abstract_plotters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:41.743377 autocti-2024.1.27.4/autocti/plot/get_visuals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/plot/get_visuals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/plot/get_visuals/one_d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/plot/get_visuals/two_d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/preloads.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:41.743377 autocti-2024.1.27.4/autocti/util/
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/autocti/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:41.743377 autocti-2024.1.27.4/autocti.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-01-27 19:56:41.000000 autocti-2024.1.27.4/autocti.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-27 19:56:41.743377 autocti-2024.1.27.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-01-27 19:56:34.000000 autocti-2024.1.27.4/setup.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:21.483326 autocti-2024.5.16.0/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:20.703813 autocti-2024.5.16.0/.github/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:20.769931 autocti-2024.5.16.0/.github/workflows/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      475 2022-10-20 11:42:03.000000 autocti-2024.5.16.0/.github/workflows/draft-pdf.yml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2616 2024-01-27 19:34:16.000000 autocti-2024.5.16.0/.github/workflows/main.yml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1111 2022-12-19 11:17:33.000000 autocti-2024.5.16.0/CITATIONS.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18831 2022-12-19 11:17:33.000000 autocti-2024.5.16.0/CODE_OF_CONDUCT.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2470 2022-10-20 11:42:03.000000 autocti-2024.5.16.0/CONTRIBUTING.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1095 2022-10-20 11:42:03.000000 autocti-2024.5.16.0/LICENSE
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      379 2022-11-28 11:07:42.000000 autocti-2024.5.16.0/MANIFEST.in
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9122 2024-05-16 09:59:21.481322 autocti-2024.5.16.0/PKG-INFO
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8271 2023-10-16 17:17:04.000000 autocti-2024.5.16.0/README.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:20.782578 autocti-2024.5.16.0/autocti/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3728 2024-05-16 09:55:27.000000 autocti-2024.5.16.0/autocti/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:20.799579 autocti-2024.5.16.0/autocti/aggregator/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      281 2023-05-15 17:43:12.000000 autocti-2024.5.16.0/autocti/aggregator/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1298 2024-03-09 18:55:45.000000 autocti-2024.5.16.0/autocti/aggregator/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4237 2024-03-12 18:45:29.000000 autocti-2024.5.16.0/autocti/aggregator/cti.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6208 2023-08-14 09:43:02.000000 autocti-2024.5.16.0/autocti/aggregator/dataset_1d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7205 2024-03-12 18:45:29.000000 autocti-2024.5.16.0/autocti/aggregator/fit_dataset_1d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7318 2024-03-12 18:45:29.000000 autocti-2024.5.16.0/autocti/aggregator/fit_imaging_ci.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6965 2023-10-16 17:17:04.000000 autocti-2024.5.16.0/autocti/aggregator/imaging_ci.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:20.820122 autocti-2024.5.16.0/autocti/charge_injection/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2024.5.16.0/autocti/charge_injection/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2899 2023-05-15 17:37:57.000000 autocti-2024.5.16.0/autocti/charge_injection/ci_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4971 2023-08-18 08:58:42.000000 autocti-2024.5.16.0/autocti/charge_injection/fit.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1500 2023-05-15 17:37:57.000000 autocti-2024.5.16.0/autocti/charge_injection/hyper.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:20.836280 autocti-2024.5.16.0/autocti/charge_injection/imaging/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2024.5.16.0/autocti/charge_injection/imaging/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13284 2023-12-11 15:32:15.000000 autocti-2024.5.16.0/autocti/charge_injection/imaging/imaging.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4096 2024-05-03 12:25:18.000000 autocti-2024.5.16.0/autocti/charge_injection/imaging/readout_persistence.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1813 2024-04-08 18:55:04.000000 autocti-2024.5.16.0/autocti/charge_injection/imaging/settings.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13034 2024-05-03 12:25:18.000000 autocti-2024.5.16.0/autocti/charge_injection/imaging/simulator.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    17201 2024-02-23 13:18:19.000000 autocti-2024.5.16.0/autocti/charge_injection/layout.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1174 2023-01-13 16:58:40.000000 autocti-2024.5.16.0/autocti/charge_injection/master.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:20.841618 autocti-2024.5.16.0/autocti/charge_injection/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2024.5.16.0/autocti/charge_injection/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3786 2024-02-19 15:47:21.000000 autocti-2024.5.16.0/autocti/charge_injection/mock/mock_result.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:20.858126 autocti-2024.5.16.0/autocti/charge_injection/model/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2024.5.16.0/autocti/charge_injection/model/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11313 2024-05-03 12:25:18.000000 autocti-2024.5.16.0/autocti/charge_injection/model/analysis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    15032 2024-05-03 12:25:18.000000 autocti-2024.5.16.0/autocti/charge_injection/model/plotter_interface.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1132 2023-06-03 10:26:26.000000 autocti-2024.5.16.0/autocti/charge_injection/model/result.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7736 2024-05-03 12:25:18.000000 autocti-2024.5.16.0/autocti/charge_injection/model/visualizer.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9610 2023-05-15 17:37:57.000000 autocti-2024.5.16.0/autocti/charge_injection/ou_sim_ci.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:20.867126 autocti-2024.5.16.0/autocti/charge_injection/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2024.5.16.0/autocti/charge_injection/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    25257 2024-05-03 12:25:18.000000 autocti-2024.5.16.0/autocti/charge_injection/plot/fit_ci_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    19402 2024-02-01 14:11:03.000000 autocti-2024.5.16.0/autocti/charge_injection/plot/imaging_ci_plotters.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:20.879589 autocti-2024.5.16.0/autocti/clocker/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2024.5.16.0/autocti/clocker/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1567 2024-02-15 11:02:38.000000 autocti-2024.5.16.0/autocti/clocker/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8640 2023-12-11 15:32:15.000000 autocti-2024.5.16.0/autocti/clocker/one_d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    36772 2023-12-11 15:32:15.000000 autocti-2024.5.16.0/autocti/clocker/two_d.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:20.888588 autocti-2024.5.16.0/autocti/config/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      503 2023-10-16 17:24:50.000000 autocti-2024.5.16.0/autocti/config/general.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      840 2023-12-18 14:52:57.000000 autocti-2024.5.16.0/autocti/config/notation.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:20.897587 autocti-2024.5.16.0/autocti/config/priors/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      648 2023-02-27 14:53:06.000000 autocti-2024.5.16.0/autocti/config/priors/ccd.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      210 2022-12-02 15:59:51.000000 autocti-2024.5.16.0/autocti/config/priors/hyper.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1145 2022-12-05 10:42:13.000000 autocti-2024.5.16.0/autocti/config/priors/traps.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1868 2023-11-13 18:55:03.000000 autocti-2024.5.16.0/autocti/config/visualize.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:20.908591 autocti-2024.5.16.0/autocti/cosmics/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2024.5.16.0/autocti/cosmics/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11501 2023-10-20 17:59:09.000000 autocti-2024.5.16.0/autocti/cosmics/cosmics.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    41101 2022-12-17 13:44:39.000000 autocti-2024.5.16.0/autocti/cosmics/cr_distances.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13590 2022-12-17 13:44:38.000000 autocti-2024.5.16.0/autocti/cosmics/cr_lengths.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:20.914586 autocti-2024.5.16.0/autocti/dataset_1d/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2024.5.16.0/autocti/dataset_1d/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:20.924587 autocti-2024.5.16.0/autocti/dataset_1d/dataset_1d/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2024.5.16.0/autocti/dataset_1d/dataset_1d/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10103 2024-04-08 18:55:04.000000 autocti-2024.5.16.0/autocti/dataset_1d/dataset_1d/dataset_1d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5608 2023-12-11 15:32:15.000000 autocti-2024.5.16.0/autocti/dataset_1d/dataset_1d/simulator.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      970 2022-12-13 16:21:22.000000 autocti-2024.5.16.0/autocti/dataset_1d/fit.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:20.940592 autocti-2024.5.16.0/autocti/dataset_1d/model/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2024.5.16.0/autocti/dataset_1d/model/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6828 2024-05-03 12:25:18.000000 autocti-2024.5.16.0/autocti/dataset_1d/model/analysis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11971 2024-05-03 12:25:18.000000 autocti-2024.5.16.0/autocti/dataset_1d/model/plotter_interface.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      101 2023-05-15 17:37:57.000000 autocti-2024.5.16.0/autocti/dataset_1d/model/result.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6842 2024-05-03 12:25:18.000000 autocti-2024.5.16.0/autocti/dataset_1d/model/visualizer.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:20.950588 autocti-2024.5.16.0/autocti/dataset_1d/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2024.5.16.0/autocti/dataset_1d/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9794 2023-10-16 17:17:04.000000 autocti-2024.5.16.0/autocti/dataset_1d/plot/dataset_1d_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13804 2023-10-16 17:17:04.000000 autocti-2024.5.16.0/autocti/dataset_1d/plot/fit_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      558 2023-12-19 16:22:29.000000 autocti-2024.5.16.0/autocti/exc.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:20.955588 autocti-2024.5.16.0/autocti/extract/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2024.5.16.0/autocti/extract/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:20.974587 autocti-2024.5.16.0/autocti/extract/one_d/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2024.5.16.0/autocti/extract/one_d/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7755 2024-02-01 14:11:03.000000 autocti-2024.5.16.0/autocti/extract/one_d/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2113 2023-05-15 17:37:57.000000 autocti-2024.5.16.0/autocti/extract/one_d/eper.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1059 2023-03-21 12:51:53.000000 autocti-2024.5.16.0/autocti/extract/one_d/fpr.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10366 2023-05-15 17:37:57.000000 autocti-2024.5.16.0/autocti/extract/one_d/master.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1227 2023-03-21 12:51:53.000000 autocti-2024.5.16.0/autocti/extract/one_d/overscan.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2146 2023-11-16 20:20:07.000000 autocti-2024.5.16.0/autocti/extract/settings.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:20.988890 autocti-2024.5.16.0/autocti/extract/two_d/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2024.5.16.0/autocti/extract/two_d/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    19891 2024-02-01 14:11:03.000000 autocti-2024.5.16.0/autocti/extract/two_d/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2356 2023-03-21 12:51:53.000000 autocti-2024.5.16.0/autocti/extract/two_d/extract_2d_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    20389 2023-10-16 17:24:50.000000 autocti-2024.5.16.0/autocti/extract/two_d/master.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:21.018331 autocti-2024.5.16.0/autocti/extract/two_d/parallel/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2024.5.16.0/autocti/extract/two_d/parallel/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    15134 2023-11-16 20:25:45.000000 autocti-2024.5.16.0/autocti/extract/two_d/parallel/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11608 2023-06-03 10:32:33.000000 autocti-2024.5.16.0/autocti/extract/two_d/parallel/calibration.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7150 2024-02-01 14:11:03.000000 autocti-2024.5.16.0/autocti/extract/two_d/parallel/eper.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7182 2024-02-01 14:11:03.000000 autocti-2024.5.16.0/autocti/extract/two_d/parallel/fpr.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4595 2023-10-16 17:24:50.000000 autocti-2024.5.16.0/autocti/extract/two_d/parallel/overscan.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5472 2023-09-26 14:52:19.000000 autocti-2024.5.16.0/autocti/extract/two_d/parallel/pedestal.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3781 2023-10-16 17:24:50.000000 autocti-2024.5.16.0/autocti/extract/two_d/parallel/pre_injection.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:21.049102 autocti-2024.5.16.0/autocti/extract/two_d/serial/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2024.5.16.0/autocti/extract/two_d/serial/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7765 2023-11-16 20:25:45.000000 autocti-2024.5.16.0/autocti/extract/two_d/serial/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10782 2023-06-03 10:32:33.000000 autocti-2024.5.16.0/autocti/extract/two_d/serial/calibration.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6160 2023-03-21 12:51:53.000000 autocti-2024.5.16.0/autocti/extract/two_d/serial/eper.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3793 2023-03-21 12:51:53.000000 autocti-2024.5.16.0/autocti/extract/two_d/serial/fpr.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4595 2023-03-21 12:51:53.000000 autocti-2024.5.16.0/autocti/extract/two_d/serial/overscan.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3790 2023-09-26 17:29:31.000000 autocti-2024.5.16.0/autocti/extract/two_d/serial/overscan_no_eper.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3103 2023-10-16 17:24:50.000000 autocti-2024.5.16.0/autocti/extract/two_d/serial/prescan.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5775 2024-03-26 13:07:02.000000 autocti-2024.5.16.0/autocti/fixtures.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:21.053104 autocti-2024.5.16.0/autocti/instruments/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      122 2022-10-21 09:42:48.000000 autocti-2024.5.16.0/autocti/instruments/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:21.073322 autocti-2024.5.16.0/autocti/instruments/acs/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      151 2022-10-24 13:23:41.000000 autocti-2024.5.16.0/autocti/instruments/acs/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6118 2023-08-14 09:43:02.000000 autocti-2024.5.16.0/autocti/instruments/acs/acs_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11226 2023-05-15 17:37:58.000000 autocti-2024.5.16.0/autocti/instruments/acs/array_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3037 2023-05-15 17:37:58.000000 autocti-2024.5.16.0/autocti/instruments/acs/header.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4794 2023-05-15 17:37:58.000000 autocti-2024.5.16.0/autocti/instruments/acs/image.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1061 2022-10-21 13:55:34.000000 autocti-2024.5.16.0/autocti/instruments/acs/layout.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:21.091338 autocti-2024.5.16.0/autocti/instruments/euclid/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      107 2022-10-21 13:47:30.000000 autocti-2024.5.16.0/autocti/instruments/euclid/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12883 2023-01-13 16:58:40.000000 autocti-2024.5.16.0/autocti/instruments/euclid/array_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      711 2023-05-15 17:37:58.000000 autocti-2024.5.16.0/autocti/instruments/euclid/euclid_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      851 2023-05-15 17:37:58.000000 autocti-2024.5.16.0/autocti/instruments/euclid/header.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    17129 2023-05-15 17:37:58.000000 autocti-2024.5.16.0/autocti/instruments/euclid/layout.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:21.098321 autocti-2024.5.16.0/autocti/layout/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:04.000000 autocti-2024.5.16.0/autocti/layout/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2819 2023-05-30 13:00:37.000000 autocti-2024.5.16.0/autocti/layout/one_d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11884 2024-02-23 13:18:19.000000 autocti-2024.5.16.0/autocti/layout/two_d.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:21.107324 autocti-2024.5.16.0/autocti/mask/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:04.000000 autocti-2024.5.16.0/autocti/mask/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2447 2023-05-15 17:37:58.000000 autocti-2024.5.16.0/autocti/mask/mask_1d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    16351 2023-12-11 15:32:15.000000 autocti-2024.5.16.0/autocti/mask/mask_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      193 2023-02-08 17:48:18.000000 autocti-2024.5.16.0/autocti/mock.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:21.127331 autocti-2024.5.16.0/autocti/model/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:04.000000 autocti-2024.5.16.0/autocti/model/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4407 2024-05-03 12:25:18.000000 autocti-2024.5.16.0/autocti/model/analysis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3921 2024-03-20 18:25:10.000000 autocti-2024.5.16.0/autocti/model/model_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1028 2024-05-03 12:25:18.000000 autocti-2024.5.16.0/autocti/model/plotter_interface.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      845 2024-05-03 12:25:18.000000 autocti-2024.5.16.0/autocti/model/result.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4827 2023-10-16 17:24:50.000000 autocti-2024.5.16.0/autocti/model/settings.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:21.134322 autocti-2024.5.16.0/autocti/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2672 2024-03-10 19:17:55.000000 autocti-2024.5.16.0/autocti/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5150 2023-12-11 15:32:15.000000 autocti-2024.5.16.0/autocti/plot/abstract_plotters.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:21.143322 autocti-2024.5.16.0/autocti/plot/get_visuals/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-11 16:14:32.000000 autocti-2024.5.16.0/autocti/plot/get_visuals/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1215 2022-11-11 16:14:32.000000 autocti-2024.5.16.0/autocti/plot/get_visuals/one_d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3107 2023-06-03 09:58:40.000000 autocti-2024.5.16.0/autocti/plot/get_visuals/two_d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2885 2022-12-18 14:37:25.000000 autocti-2024.5.16.0/autocti/preloads.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:21.146338 autocti-2024.5.16.0/autocti/util/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      829 2022-10-20 11:42:04.000000 autocti-2024.5.16.0/autocti/util/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:21.479322 autocti-2024.5.16.0/autocti.egg-info/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7815 2024-05-16 09:59:20.000000 autocti-2024.5.16.0/autocti.egg-info/SOURCES.txt
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:21.154342 autocti-2024.5.16.0/docs/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:21.157323 autocti-2024.5.16.0/docs/_static/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       11 2022-10-20 11:42:04.000000 autocti-2024.5.16.0/docs/_static/.gitignore
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:21.163322 autocti-2024.5.16.0/docs/_templates/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      832 2022-12-21 16:35:52.000000 autocti-2024.5.16.0/docs/_templates/custom-class-template.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1293 2022-12-16 17:06:50.000000 autocti-2024.5.16.0/docs/_templates/custom_module_template.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:21.167322 autocti-2024.5.16.0/docs/advanced/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6864 2023-10-17 17:17:26.000000 autocti-2024.5.16.0/docs/advanced/database.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:21.184321 autocti-2024.5.16.0/docs/api/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      809 2022-12-20 20:00:42.000000 autocti-2024.5.16.0/docs/api/arctic.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      545 2022-12-20 20:00:42.000000 autocti-2024.5.16.0/docs/api/clocking.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1190 2024-05-03 12:25:18.000000 autocti-2024.5.16.0/docs/api/data.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      303 2022-12-20 20:00:42.000000 autocti-2024.5.16.0/docs/api/fitting.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1472 2023-10-16 17:17:04.000000 autocti-2024.5.16.0/docs/api/modeling.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2903 2024-03-20 19:26:25.000000 autocti-2024.5.16.0/docs/api/plot.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4364 2023-06-07 13:32:55.000000 autocti-2024.5.16.0/docs/conf.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:21.198347 autocti-2024.5.16.0/docs/general/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1315 2023-06-16 08:24:22.000000 autocti-2024.5.16.0/docs/general/citations.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1015 2022-11-27 17:21:24.000000 autocti-2024.5.16.0/docs/general/configs.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      360 2022-11-27 17:21:24.000000 autocti-2024.5.16.0/docs/general/credits.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2042 2023-06-07 12:03:29.000000 autocti-2024.5.16.0/docs/general/workspace.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5283 2023-06-07 12:10:51.000000 autocti-2024.5.16.0/docs/index.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:21.221324 autocti-2024.5.16.0/docs/installation/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1381 2022-12-06 16:43:06.000000 autocti-2024.5.16.0/docs/installation/arctic.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3275 2023-10-26 13:36:13.000000 autocti-2024.5.16.0/docs/installation/conda.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3340 2023-06-11 12:27:38.000000 autocti-2024.5.16.0/docs/installation/numba.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2456 2023-10-23 12:35:45.000000 autocti-2024.5.16.0/docs/installation/overview.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2657 2023-10-26 13:36:13.000000 autocti-2024.5.16.0/docs/installation/pip.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4642 2023-05-15 17:43:12.000000 autocti-2024.5.16.0/docs/installation/source.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2575 2023-07-05 15:15:06.000000 autocti-2024.5.16.0/docs/installation/troubleshooting.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:21.241323 autocti-2024.5.16.0/docs/overview/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:21.264323 autocti-2024.5.16.0/docs/overview/images/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   397515 2022-10-20 11:42:04.000000 autocti-2024.5.16.0/docs/overview/images/ccd.gif
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   281375 2022-10-20 11:42:04.000000 autocti-2024.5.16.0/docs/overview/images/ccd_schematic.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   514636 2022-10-20 11:42:04.000000 autocti-2024.5.16.0/docs/overview/images/cti.gif
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   132888 2022-10-20 11:42:04.000000 autocti-2024.5.16.0/docs/overview/images/cti_time_evolution.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:21.279323 autocti-2024.5.16.0/docs/overview/images/overview_1/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    21797 2022-10-20 11:42:04.000000 autocti-2024.5.16.0/docs/overview/images/overview_1/array_1d.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    23382 2022-10-20 11:42:04.000000 autocti-2024.5.16.0/docs/overview/images/overview_1/array_1d_cti_corrected.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    22695 2022-10-20 11:42:04.000000 autocti-2024.5.16.0/docs/overview/images/overview_1/array_1d_with_cti.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:21.304324 autocti-2024.5.16.0/docs/overview/images/overview_2/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    25837 2024-02-21 09:59:40.000000 autocti-2024.5.16.0/docs/overview/images/overview_2/post_cti_data_2d_corrected.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    23657 2024-02-21 09:59:39.000000 autocti-2024.5.16.0/docs/overview/images/overview_2/post_cti_data_2d_parallel.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    26417 2024-02-21 09:59:40.000000 autocti-2024.5.16.0/docs/overview/images/overview_2/post_cti_data_2d_parallel_serial.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    23358 2024-02-21 09:59:39.000000 autocti-2024.5.16.0/docs/overview/images/overview_2/post_cti_data_2d_serial.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    22803 2024-02-21 09:59:39.000000 autocti-2024.5.16.0/docs/overview/images/overview_2/pre_cti_data_2d.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:21.332323 autocti-2024.5.16.0/docs/overview/images/overview_3/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    23633 2024-02-21 10:06:29.000000 autocti-2024.5.16.0/docs/overview/images/overview_3/density_1.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    24271 2024-02-21 10:06:29.000000 autocti-2024.5.16.0/docs/overview/images/overview_3/density_2.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    24800 2024-02-21 10:06:29.000000 autocti-2024.5.16.0/docs/overview/images/overview_3/timescale_1.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    23556 2024-02-21 10:06:29.000000 autocti-2024.5.16.0/docs/overview/images/overview_3/timescale_2.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    21374 2024-02-21 10:06:30.000000 autocti-2024.5.16.0/docs/overview/images/overview_3/volume_1.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    21362 2024-02-21 10:06:30.000000 autocti-2024.5.16.0/docs/overview/images/overview_3/volume_2.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:21.374324 autocti-2024.5.16.0/docs/overview/images/overview_4/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    29112 2024-02-21 11:26:30.000000 autocti-2024.5.16.0/docs/overview/images/overview_4/binned_parallel_eper.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    21641 2024-02-21 11:26:32.000000 autocti-2024.5.16.0/docs/overview/images/overview_4/binned_parallel_fpr.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    29391 2024-02-21 11:28:29.000000 autocti-2024.5.16.0/docs/overview/images/overview_4/binned_serial_eper.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    22523 2024-02-21 11:28:31.000000 autocti-2024.5.16.0/docs/overview/images/overview_4/binned_serial_fpr.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    60755 2024-02-21 11:31:47.000000 autocti-2024.5.16.0/docs/overview/images/overview_4/imaging_ci.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    52020 2024-02-21 11:24:41.000000 autocti-2024.5.16.0/docs/overview/images/overview_4/imaging_ci_eper.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    54778 2024-02-21 11:31:52.000000 autocti-2024.5.16.0/docs/overview/images/overview_4/imaging_ci_fpr.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   351059 2022-10-20 11:42:04.000000 autocti-2024.5.16.0/docs/overview/images/overview_4/imaging_ci_non_uniform_cosmic_rays.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    33706 2024-02-21 11:32:09.000000 autocti-2024.5.16.0/docs/overview/images/overview_4/pre_cti_data.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:21.446323 autocti-2024.5.16.0/docs/overview/images/overview_5/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    34048 2024-02-21 10:46:31.000000 autocti-2024.5.16.0/docs/overview/images/overview_5/chi_squared_map.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    42146 2024-02-21 10:46:33.000000 autocti-2024.5.16.0/docs/overview/images/overview_5/chi_squared_map_1d.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    33488 2024-02-21 10:46:31.000000 autocti-2024.5.16.0/docs/overview/images/overview_5/chi_squared_map_good.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    30195 2024-02-21 10:46:32.000000 autocti-2024.5.16.0/docs/overview/images/overview_5/chi_squared_map_masked.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    30728 2024-02-21 10:46:32.000000 autocti-2024.5.16.0/docs/overview/images/overview_5/ci_image_masked.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    27278 2024-02-21 11:43:11.000000 autocti-2024.5.16.0/docs/overview/images/overview_5/data.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    46392 2024-02-21 10:46:33.000000 autocti-2024.5.16.0/docs/overview/images/overview_5/dataset_1d.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    36115 2024-02-21 10:46:31.000000 autocti-2024.5.16.0/docs/overview/images/overview_5/normalized_residual_map.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    46251 2024-02-21 10:46:33.000000 autocti-2024.5.16.0/docs/overview/images/overview_5/normalized_residual_map_1d.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    36647 2024-02-21 10:46:31.000000 autocti-2024.5.16.0/docs/overview/images/overview_5/normalized_residual_map_good.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    32029 2024-02-21 10:46:32.000000 autocti-2024.5.16.0/docs/overview/images/overview_5/normalized_residual_map_masked.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    23977 2024-02-21 11:43:11.000000 autocti-2024.5.16.0/docs/overview/images/overview_5/pre_cti_data.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    33744 2024-02-21 10:46:30.000000 autocti-2024.5.16.0/docs/overview/images/overview_5/residual_map.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    23101 2024-02-21 10:46:33.000000 autocti-2024.5.16.0/docs/overview/images/overview_5/residual_map_1d.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    33526 2024-02-21 10:46:31.000000 autocti-2024.5.16.0/docs/overview/images/overview_5/residual_map_good.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    27955 2024-02-21 10:46:32.000000 autocti-2024.5.16.0/docs/overview/images/overview_5/residual_map_masked.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:21.453321 autocti-2024.5.16.0/docs/overview/images/overview_6/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   139326 2024-02-21 11:39:35.000000 autocti-2024.5.16.0/docs/overview/images/overview_6/fit_1d_100.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   193189 2024-02-21 11:41:44.000000 autocti-2024.5.16.0/docs/overview/images/overview_6/fit_2d_100.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   542080 2022-10-20 11:42:04.000000 autocti-2024.5.16.0/docs/overview/images/what_is_cti.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12544 2023-10-16 17:17:04.000000 autocti-2024.5.16.0/docs/overview/overview_1_what_is_cti.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10880 2023-06-07 12:08:16.000000 autocti-2024.5.16.0/docs/overview/overview_2_parallel_and_serial.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10013 2023-01-13 16:58:40.000000 autocti-2024.5.16.0/docs/overview/overview_3_cti_features.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11490 2023-06-07 13:25:07.000000 autocti-2024.5.16.0/docs/overview/overview_4_charge_injection_data.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14813 2024-02-21 11:45:09.000000 autocti-2024.5.16.0/docs/overview/overview_5_fitting.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14908 2023-10-16 17:17:04.000000 autocti-2024.5.16.0/docs/overview/overview_6_cti_calibration.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      160 2024-05-16 09:55:27.000000 autocti-2024.5.16.0/docs/requirements.txt
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       30 2022-10-20 11:42:04.000000 autocti-2024.5.16.0/eden.ini
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:21.462323 autocti-2024.5.16.0/files/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    19359 2023-06-16 08:34:40.000000 autocti-2024.5.16.0/files/citations.bib
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1484 2023-06-16 08:34:40.000000 autocti-2024.5.16.0/files/citations.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2089 2023-06-16 08:34:40.000000 autocti-2024.5.16.0/files/citations.tex
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       50 2023-12-19 16:37:45.000000 autocti-2024.5.16.0/optional_requirements.txt
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:59:21.476321 autocti-2024.5.16.0/paper/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      180 2022-10-20 11:42:04.000000 autocti-2024.5.16.0/paper/README.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   881609 2022-10-20 11:42:04.000000 autocti-2024.5.16.0/paper/cti_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    97784 2024-04-08 18:55:00.000000 autocti-2024.5.16.0/paper/paper.bib
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      829 2022-10-20 11:42:04.000000 autocti-2024.5.16.0/paper/paper.json
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10612 2024-04-08 18:55:00.000000 autocti-2024.5.16.0/paper/paper.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      917 2022-11-23 10:12:20.000000 autocti-2024.5.16.0/profiling
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      210 2022-10-20 11:42:04.000000 autocti-2024.5.16.0/readthedocs.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       23 2024-03-09 18:55:45.000000 autocti-2024.5.16.0/requirements.txt
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       38 2024-05-16 09:59:21.483326 autocti-2024.5.16.0/setup.cfg
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1706 2024-05-16 09:56:09.000000 autocti-2024.5.16.0/setup.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1875 2022-10-20 11:42:04.000000 autocti-2024.5.16.0/to_do_list
```

### Comparing `autocti-2024.1.27.4/CITATIONS.rst` & `autocti-2024.5.16.0/CITATIONS.rst`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/LICENSE` & `autocti-2024.5.16.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/PKG-INFO` & `autocti-2024.5.16.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autocti
-Version: 2024.1.27.4
+Version: 2024.5.16.0
 Summary: PyAutoCTI: Charge Transfer Inefficiency Modeling
 Home-page: https://github.com/jammy2211/PyAutoCTI
 Author: James Nightingale, Richard Massey, Jacob Kegerreis and Richard Hayes
 Author-email: james.w.nightingale@durham.ac.uk
 License: MIT License
 Keywords: cli
 Classifier: Intended Audience :: Science/Research
@@ -15,18 +15,14 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: nautilus-sampler==0.7.4
-Requires-Dist: autoconf==2024.1.27.4
-Requires-Dist: autofit==2024.1.27.4
-Requires-Dist: autoarray==2024.1.27.4
 
 PyAutoCTI: Charge Transfer Inefficiency Modeling
 ================================================
 
 .. |nbsp| unicode:: 0xA0
     :trim:
```

### Comparing `autocti-2024.1.27.4/README.rst` & `autocti-2024.5.16.0/README.rst`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/__init__.py` & `autocti-2024.5.16.0/autocti/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,24 +41,24 @@
 from .extract.two_d.serial.eper import Extract2DSerialEPER
 from .extract.two_d.parallel.calibration import Extract2DParallelCalibration
 from .extract.two_d.serial.calibration import Extract2DSerialCalibration
 from .extract.two_d.master import Extract2DMaster
 from .instruments import euclid
 from .instruments import acs
 from .charge_injection.fit import FitImagingCI
+from .charge_injection.imaging.readout_persistence import ReadoutPersistence
 from .mask.mask_2d import Mask2D
 from .mask.mask_2d import SettingsMask2D
 from .mask.mask_1d import Mask1D
 from .mask.mask_1d import SettingsMask1D
 from .extract.one_d.overscan import Extract1DOverscan
 from .extract.one_d.fpr import Extract1DFPR
 from .extract.one_d.eper import Extract1DEPER
 from .extract.one_d.master import Extract1DMaster
 from .layout.one_d import Layout1D
-from .dataset_1d.dataset_1d.settings import SettingsDataset1D
 from .dataset_1d.dataset_1d.dataset_1d import Dataset1D
 from .dataset_1d.dataset_1d.simulator import SimulatorDataset1D
 from .dataset_1d.fit import FitDataset1D
 from .dataset_1d.model.analysis import AnalysisDataset1D
 from .dataset_1d.model.result import ResultDataset1D
 from .charge_injection.model.analysis import AnalysisImagingCI
 from .charge_injection.model.result import ResultImagingCI
@@ -74,8 +74,8 @@
 from . import plot
 from . import mock as m  # noqa
 
 from autoconf import conf
 
 conf.instance.register(__file__)
 
-__version__ = "2024.1.27.4"
+__version__ = "2024.5.16.0"
```

### Comparing `autocti-2024.1.27.4/autocti/aggregator/cti.py` & `autocti-2024.5.16.0/autocti/aggregator/cti.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from __future__ import annotations
 import logging
-from typing import TYPE_CHECKING, List, Union
+from typing import TYPE_CHECKING, Optional, Union
+
+from autocti.aggregator.abstract import AggBase
 
 if TYPE_CHECKING:
     from autocti.model.model_util import CTI1D
     from autocti.model.model_util import CTI2D
 
 import autofit as af
 
-from autocti.aggregator.abstract import AbstractAgg
-
 logger = logging.getLogger(__name__)
 
 
 def _cti_from(fit: af.Fit) -> Union[CTI1D, CTI2D]:
     """
     Returns a list of `CTI` objects from a `PyAutoFit` sqlite database `Fit` object.
 
@@ -50,15 +50,15 @@
             so proceed with caution!
             """
         )
 
     return fit.instance.cti
 
 
-class CTIAgg(AbstractAgg):
+class CTIAgg(AggBase):
     """
     Interfaces with an `PyAutoFit` aggregator object to create instances of `CTI` objects from the results
     of a model-fit.
 
     The results of a model-fit can be stored in a sqlite database, including the following attributes of the fit:
 
     - The model and its best fit parameters (e.g. `model.json`).
@@ -81,26 +81,29 @@
 
     Parameters
     ----------
     aggregator
         A `PyAutoFit` aggregator object which can load the results of model-fits.
     """
 
-    def object_via_gen_from(self, fit, cti: Union[CTI1D, CTI2D]) -> Union[CTI1D, CTI2D]:
+    def object_via_gen_from(
+        self, fit, instance: Optional[af.ModelInstance] = None
+    ) -> Union[CTI1D, CTI2D]:
         """
         Returns a generator of `CTI` objects from an input aggregator.
 
         See `__init__` for a description of how the `CTI` objects are created by this method.
 
         Parameters
         ----------
         fit
             A `PyAutoFit` `Fit` object which contains the results of a model-fit as an entry in a sqlite database.
-        cti
-            A CTI model corresponding to a sample of the non-linear search.
+        instance
+            A manual instance that overwrites the max log likelihood instance in fit (e.g. for drawing the instance
+            randomly from the PDF).
 
         Returns
         -------
         CTI
             A list of `CTI` objects whose parameters are a sample of the non-linear search.
         """
         return _cti_from(fit=fit)
```

### Comparing `autocti-2024.1.27.4/autocti/aggregator/dataset_1d.py` & `autocti-2024.5.16.0/autocti/aggregator/dataset_1d.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/aggregator/fit_dataset_1d.py` & `autocti-2024.5.16.0/autocti/aggregator/fit_imaging_ci.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,150 +1,160 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING, List, Optional, Union
 
 if TYPE_CHECKING:
     from autocti.clocker.abstract import AbstractClocker
     from autocti.model.model_util import CTI1D
     from autocti.model.model_util import CTI2D
-    from autocti.dataset_1d.fit import FitDataset1D
+    from autocti.charge_injection.fit import FitImagingCI
 
 import autofit as af
 
-from autocti.aggregator.abstract import AbstractAgg
-from autocti.aggregator.dataset_1d import _dataset_1d_list_from
+from autocti.aggregator.abstract import AggBase
+from autocti.aggregator.imaging_ci import _imaging_ci_list_from
 
 
-def _fit_dataset_1d_list_from(
+def _fit_imaging_ci_list_from(
     fit: af.Fit,
-    cti: Union[CTI1D, CTI2D],
+    instance: Optional[af.ModelInstance] = None,
     use_dataset_full: bool = False,
     clocker_list: Optional[AbstractClocker] = None,
-) -> List[FitDataset1D]:
+) -> List[FitImagingCI]:
     """
-    Returns a list of `FitDataset1D` object from a `PyAutoFit` sqlite database `Fit` object.
+    Returns a list of `FitImagingCI` object from a `PyAutoFit` sqlite database `Fit` object.
 
     The results of a model-fit can be stored in a sqlite database, including the following attributes of the fit:
 
     - The masked dataset (e.g. data / noise map / pre cti data) as .fits files (contained in `dataset` folder).
     - The clocker used to add  CTI in the fit (`dataset/clocker.json`).
     - The settings used for clocking CIT (contained in `dataset/settings_cti.json`).
 
     Each individual attribute can be loaded from the database via the `fit.value()` method.
 
-    This method combines all of these attributes and returns a  list of `FitDataset1D` objects, by loading the masked
+    This method combines all of these attributes and returns a  list of `FitImagingCI` objects, by loading the masked
     dataset adding CTI to its pre-cti data via the cti model and clocking and fitting the model image to the dataset.
 
-    If multiple `Dataset1D` objects were fitted simultaneously via analysis summing, the `fit.child_values()` method
-    is instead used to load lists of the datasets, perform the fit and return a list of `FitDataset1D` objects.
+    If multiple `ImagingCI` objects were fitted simultaneously via analysis summing, the `fit.child_values()` method
+    is instead used to load lists of the datasets, perform the fit and return a list of `FitImagingCI` objects.
 
     If a `dataset_full` is input into the `Analysis` class when a model-fit is performed and therefore accessible
     to the database, the input `use_dataset_full` can be switched in to fit the full dataset instead.
 
     Parameters
     ----------
     fit
         A `PyAutoFit` `Fit` object which contains the results of a model-fit as an entry in a sqlite database.
+    instance
+        A manual instance that overwrites the max log likelihood instance in fit (e.g. for drawing the instance
+        randomly from the PDF).
     use_dataset_full
         If a `dataset_full` is input into the `Analysis` class when a model-fit is performed and therefore accessible
-        to the database, the input `use_dataset_full` can be switched in to load instead the full `Dataset1D` objects.
+        to the database, the input `use_dataset_full` can be switched in to load instead the full `ImagingCI` objects.
     clocker_list
         If input, overwrites the clocker used in the fit with a new clocker which is used to perform the fit.
     """
 
-    from autocti.dataset_1d.fit import FitDataset1D
+    from autocti.charge_injection.fit import FitImagingCI
 
-    dataset_list = _dataset_1d_list_from(fit=fit, use_dataset_full=use_dataset_full)
+    dataset_list = _imaging_ci_list_from(fit=fit, use_dataset_full=use_dataset_full)
 
     if clocker_list is None:
         if not fit.children:
             clocker_list = [fit.value(name="clocker")]
         else:
             clocker_list = fit.child_values(name="clocker")
 
+    if instance is not None:
+        cti = instance.cti
+    else:
+        cti = fit.instance.cti
+
     post_cti_data_list = [
         clocker.add_cti(data=dataset.pre_cti_data, cti=cti)
         for dataset, clocker in zip(dataset_list, clocker_list)
     ]
 
     return [
-        FitDataset1D(
+        FitImagingCI(
             dataset=dataset,
             post_cti_data=post_cti_data,
         )
         for dataset, post_cti_data in zip(dataset_list, post_cti_data_list)
     ]
 
 
-class FitDataset1DAgg(AbstractAgg):
+class FitImagingCIAgg(AggBase):
     def __init__(
         self,
         aggregator: af.Aggregator,
         use_dataset_full: bool = False,
         clocker_list: Optional[List[AbstractClocker]] = None,
     ):
         """
-        Interfaces with an `PyAutoFit` aggregator object to create instances of `Dataset1D` objects from the results
+        Interfaces with an `PyAutoFit` aggregator object to create instances of `ImagingCI` objects from the results
         of a model-fit.
 
         The results of a model-fit can be stored in a sqlite database, including the following attributes of the fit:
 
         - The masked dataset (e.g. data / noise map / pre cti data) as .fits files (contained in `dataset` folder).
         - The clocker used to add  CTI in the fit (`dataset/clocker.json`).
         - The settings used for clocking CIT (contained in `dataset/settings_cti.json`).
 
         The `aggregator` contains the path to each of these files, and they can be loaded individually. This class
-        can load them all at once and create a `FitDataset1D` object via the `_fit_dataset_1d_from` method.
+        can load them all at once and create a `FitImagingCI` object via the `_fit_dataset_1d_from` method.
 
-        This class's methods returns generators which create the instances of the `FitDataset1D` objects. This ensures
+        This class's methods returns generators which create the instances of the `FitImagingCI` objects. This ensures
         that large sets of results can be efficiently loaded from the hard-disk and do not require storing all
-        `Dataset1D` instances in the memory at once.
+        `ImagingCI` instances in the memory at once.
 
         For example, if the `aggregator` contains 3 model-fits, this class can be used to create a generator which
-        creates instances of the corresponding 3 `Dataset1D` objects.
+        creates instances of the corresponding 3 `ImagingCI` objects.
 
-        If multiple `Dataset1D` objects were fitted simultaneously via analysis summing, the `fit.child_values()` method
-        is instead used to load lists of the datasets, perform the fit and return a list of `FitDataset1D` objects.
+        If multiple `ImagingCI` objects were fitted simultaneously via analysis summing, the `fit.child_values()` method
+        is instead used to load lists of the datasets, perform the fit and return a list of `FitImagingCI` objects.
 
         If a `dataset_full` is input into the `Analysis` class when a model-fit is performed and therefore accessible
         to the database, the input `use_dataset_full` can be switched in to fit the full dataset instead.
 
         This can be done manually, but this object provides a more concise API.
 
         Parameters
         ----------
         aggregator
             A `PyAutoFit` aggregator object which can load the results of model-fits.
         use_dataset_full
             If a `dataset_full` is input into the `Analysis` class when a model-fit is performed and therefore
             accessible to the database, the input `use_dataset_full` can be switched in to load instead the
-            full `Dataset1D` objects.
+            full `ImagingCI` objects.
         clocker_list
             If input, overwrites the clocker used in the fit with a new clocker which is used to perform the fit.
         """
         super().__init__(
             aggregator=aggregator,
             use_dataset_full=use_dataset_full,
             clocker_list=clocker_list,
         )
 
-    def object_via_gen_from(self, fit, cti: Union[CTI1D, CTI2D]) -> List[FitDataset1D]:
+    def object_via_gen_from(
+        self, fit, instance: Optional[af.ModelInstance] = None
+    ) -> List[FitImagingCI]:
         """
-        Returns a generator of `FitDataset1D` objects from an input aggregator.
+        Returns a generator of `FitImagingCI` objects from an input aggregator.
 
-        See `__init__` for a description of how the `FitDataset1D` objects are created by this method.
+        See `__init__` for a description of how the `FitImagingCI` objects are created by this method.
 
         If a `dataset_full` is input into the `Analysis` class when a model-fit is performed and therefore accessible
         to the database, the input `use_dataset_full` can be switched in to fit the full dataset instead.
 
         Parameters
         ----------
         fit
             A `PyAutoFit` `Fit` object which contains the results of a model-fit as an entry in a sqlite database.
         cti
             The CTI model used to add CTI to the dataset to perform the fit.
         """
-        return _fit_dataset_1d_list_from(
+        return _fit_imaging_ci_list_from(
             fit=fit,
-            cti=cti,
+            instance=instance,
             use_dataset_full=self.use_dataset_full,
             clocker_list=self.clocker_list,
         )
```

### Comparing `autocti-2024.1.27.4/autocti/aggregator/fit_imaging_ci.py` & `autocti-2024.5.16.0/autocti/aggregator/imaging_ci.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,150 +1,150 @@
-from __future__ import annotations
-from typing import TYPE_CHECKING, List, Optional, Union
-
-if TYPE_CHECKING:
-    from autocti.clocker.abstract import AbstractClocker
-    from autocti.model.model_util import CTI1D
-    from autocti.model.model_util import CTI2D
-    from autocti.charge_injection.fit import FitImagingCI
-
-import autofit as af
-
-from autocti.aggregator.abstract import AbstractAgg
-from autocti.aggregator.imaging_ci import _imaging_ci_list_from
-
-
-def _fit_imaging_ci_list_from(
-    fit: af.Fit,
-    cti: Union[CTI1D, CTI2D],
-    use_dataset_full: bool = False,
-    clocker_list: Optional[AbstractClocker] = None,
-) -> List[FitImagingCI]:
-    """
-    Returns a list of `FitImagingCI` object from a `PyAutoFit` sqlite database `Fit` object.
-
-    The results of a model-fit can be stored in a sqlite database, including the following attributes of the fit:
-
-    - The masked dataset (e.g. data / noise map / pre cti data) as .fits files (contained in `dataset` folder).
-    - The clocker used to add  CTI in the fit (`dataset/clocker.json`).
-    - The settings used for clocking CIT (contained in `dataset/settings_cti.json`).
-
-    Each individual attribute can be loaded from the database via the `fit.value()` method.
-
-    This method combines all of these attributes and returns a  list of `FitImagingCI` objects, by loading the masked
-    dataset adding CTI to its pre-cti data via the cti model and clocking and fitting the model image to the dataset.
-
-    If multiple `ImagingCI` objects were fitted simultaneously via analysis summing, the `fit.child_values()` method
-    is instead used to load lists of the datasets, perform the fit and return a list of `FitImagingCI` objects.
-
-    If a `dataset_full` is input into the `Analysis` class when a model-fit is performed and therefore accessible
-    to the database, the input `use_dataset_full` can be switched in to fit the full dataset instead.
-
-    Parameters
-    ----------
-    fit
-        A `PyAutoFit` `Fit` object which contains the results of a model-fit as an entry in a sqlite database.
-    use_dataset_full
-        If a `dataset_full` is input into the `Analysis` class when a model-fit is performed and therefore accessible
-        to the database, the input `use_dataset_full` can be switched in to load instead the full `ImagingCI` objects.
-    clocker_list
-        If input, overwrites the clocker used in the fit with a new clocker which is used to perform the fit.
-    """
-
-    from autocti.charge_injection.fit import FitImagingCI
-
-    dataset_list = _imaging_ci_list_from(fit=fit, use_dataset_full=use_dataset_full)
-
-    if clocker_list is None:
-        if not fit.children:
-            clocker_list = [fit.value(name="clocker")]
-        else:
-            clocker_list = fit.child_values(name="clocker")
-
-    post_cti_data_list = [
-        clocker.add_cti(data=dataset.pre_cti_data, cti=cti)
-        for dataset, clocker in zip(dataset_list, clocker_list)
-    ]
-
-    return [
-        FitImagingCI(
-            dataset=dataset,
-            post_cti_data=post_cti_data,
-        )
-        for dataset, post_cti_data in zip(dataset_list, post_cti_data_list)
-    ]
-
-
-class FitImagingCIAgg(AbstractAgg):
-    def __init__(
-        self,
-        aggregator: af.Aggregator,
-        use_dataset_full: bool = False,
-        clocker_list: Optional[List[AbstractClocker]] = None,
-    ):
-        """
-        Interfaces with an `PyAutoFit` aggregator object to create instances of `ImagingCI` objects from the results
-        of a model-fit.
-
-        The results of a model-fit can be stored in a sqlite database, including the following attributes of the fit:
-
-        - The masked dataset (e.g. data / noise map / pre cti data) as .fits files (contained in `dataset` folder).
-        - The clocker used to add  CTI in the fit (`dataset/clocker.json`).
-        - The settings used for clocking CIT (contained in `dataset/settings_cti.json`).
-
-        The `aggregator` contains the path to each of these files, and they can be loaded individually. This class
-        can load them all at once and create a `FitImagingCI` object via the `_fit_dataset_1d_from` method.
-
-        This class's methods returns generators which create the instances of the `FitImagingCI` objects. This ensures
-        that large sets of results can be efficiently loaded from the hard-disk and do not require storing all
-        `ImagingCI` instances in the memory at once.
-
-        For example, if the `aggregator` contains 3 model-fits, this class can be used to create a generator which
-        creates instances of the corresponding 3 `ImagingCI` objects.
-
-        If multiple `ImagingCI` objects were fitted simultaneously via analysis summing, the `fit.child_values()` method
-        is instead used to load lists of the datasets, perform the fit and return a list of `FitImagingCI` objects.
-
-        If a `dataset_full` is input into the `Analysis` class when a model-fit is performed and therefore accessible
-        to the database, the input `use_dataset_full` can be switched in to fit the full dataset instead.
-
-        This can be done manually, but this object provides a more concise API.
-
-        Parameters
-        ----------
-        aggregator
-            A `PyAutoFit` aggregator object which can load the results of model-fits.
-        use_dataset_full
-            If a `dataset_full` is input into the `Analysis` class when a model-fit is performed and therefore
-            accessible to the database, the input `use_dataset_full` can be switched in to load instead the
-            full `ImagingCI` objects.
-        clocker_list
-            If input, overwrites the clocker used in the fit with a new clocker which is used to perform the fit.
-        """
-        super().__init__(
-            aggregator=aggregator,
-            use_dataset_full=use_dataset_full,
-            clocker_list=clocker_list,
-        )
-
-    def object_via_gen_from(self, fit, cti: Union[CTI1D, CTI2D]) -> List[FitImagingCI]:
-        """
-        Returns a generator of `FitImagingCI` objects from an input aggregator.
-
-        See `__init__` for a description of how the `FitImagingCI` objects are created by this method.
-
-        If a `dataset_full` is input into the `Analysis` class when a model-fit is performed and therefore accessible
-        to the database, the input `use_dataset_full` can be switched in to fit the full dataset instead.
-
-        Parameters
-        ----------
-        fit
-            A `PyAutoFit` `Fit` object which contains the results of a model-fit as an entry in a sqlite database.
-        cti
-            The CTI model used to add CTI to the dataset to perform the fit.
-        """
-        return _fit_imaging_ci_list_from(
-            fit=fit,
-            cti=cti,
-            use_dataset_full=self.use_dataset_full,
-            clocker_list=self.clocker_list,
-        )
+from functools import partial
+
+import autoarray as aa
+import autofit as af
+
+from autocti.charge_injection.imaging.imaging import ImagingCI
+
+
+def _imaging_ci_list_from(fit: af.Fit, use_dataset_full: bool = False):
+    """
+    Returns a `ImagingCI` object from a `PyAutoFit` sqlite database `Fit` object.
+
+    The results of a model-fit can be stored in a sqlite database, including the following attributes of the fit:
+
+    - The charge injection dataset data as a .fits file (`dataset/data.fits`).
+    - The noise-map as a .fits file (`dataset/noise_map.fits`).
+    - The pre CTI data as a .fits file (`dataset/pre_cti_data.fits`).
+    - The cosmic ray map (if included) as a .fits file (`dataset/cosmic_ray_map.fits`).
+    - The layout of the `ImagingCI` data structure used in the fit (`dataset/layout.json`).
+    - The settings dictionary of the data (if used) as a .json file (`dataset/settings_dict.json`).
+    - The mask used to mask the `ImagingCI` data structure in the fit (`dataset/mask.fits`).
+
+    Each individual attribute can be loaded from the database via the `fit.value()` method.
+
+    This method combines all of these attributes and returns a `ImagingCI` object, has the mask applied to the
+    `ImagingCI` data structure and its settings updated to the values used by the model-fit.
+
+    If multiple `ImagingCI` objects were fitted simultaneously via analysis summing, the `fit.child_values()` method
+    is instead used to load lists of the data, noise-map, pre CTI data, layout and mask and combine them into a list of
+    `ImagingCI` objects.
+
+    If a `dataset_full` is input into the `Analysis` class when a model-fit is performed and therefore accessible
+    to the database, the input `use_dataset_full` can be switched in to load instead the full `ImagingCI` objects.
+
+    Parameters
+    ----------
+    fit
+        A `PyAutoFit` `Fit` object which contains the results of a model-fit as an entry in a sqlite database.
+    use_dataset_full
+        If a `dataset_full` is input into the `Analysis` class when a model-fit is performed and therefore accessible
+        to the database, the input `use_dataset_full` can be switched in to load instead the full `ImagingCI` objects.
+    """
+
+    if use_dataset_full:
+        folder = "dataset_full"
+    else:
+        folder = "dataset"
+
+    if not fit.children:
+        fit_list = [fit]
+    else:
+        fit_list = fit.children
+
+    dataset_list = []
+
+    for fit in fit_list:
+        layout = fit.value(name=f"{folder}.layout")
+
+        data = aa.Array2D.from_primary_hdu(primary_hdu=fit.value(name=f"{folder}.data"))
+        noise_map = aa.Array2D.from_primary_hdu(
+            primary_hdu=fit.value(name=f"{folder}.noise_map")
+        )
+        pre_cti_data = aa.Array2D.from_primary_hdu(
+            primary_hdu=fit.value(name=f"{folder}.pre_cti_data")
+        )
+        try:
+            cosmic_ray_map = aa.Array2D.from_primary_hdu(
+                primary_hdu=fit.value(name=f"{folder}.cosmic_ray_map")
+            )
+        except AttributeError:
+            cosmic_ray_map = None
+
+        settings_dict = fit.value(name="dataset.settings_dict")
+
+        dataset = ImagingCI(
+            data=data,
+            noise_map=noise_map,
+            pre_cti_data=pre_cti_data,
+            cosmic_ray_map=cosmic_ray_map,
+            settings_dict=settings_dict,
+            layout=layout,
+        )
+
+        mask = aa.Mask2D.from_primary_hdu(primary_hdu=fit.value(name=f"{folder}.mask"))
+
+        dataset_list.append(dataset.apply_mask(mask=mask))
+
+    return dataset_list
+
+
+class ImagingCIAgg:
+    def __init__(self, aggregator: af.Aggregator, use_dataset_full: bool = False):
+        """
+        Interfaces with an `PyAutoFit` aggregator object to create instances of `ImagingCI` objects from the results
+        of a model-fit.
+
+        The results of a model-fit can be stored in a sqlite database, including the following attributes of the fit:
+
+        - The charge injection dataset data as a .fits file (`dataset/data.fits`).
+        - The noise-map as a .fits file (`dataset/noise_map.fits`).
+        - The pre CTI data as a .fits file (`dataset/pre_cti_data.fits`).
+        - The cosmic ray map (if included) as a .fits file (`dataset/cosmic_ray_map.fits`).
+        - The layout of the `ImagingCI` data structure used in the fit (`dataset/layout.json`).
+        - The settings dictionary of the data (if used) as a .json file (`dataset/settings_dict.json`).
+        - The mask used to mask the `ImagingCI` data structure in the fit (`dataset/mask.fits`).
+
+        The `aggregator` contains the path to each of these files, and they can be loaded individually. This class
+        can load them all at once and create an `ImagingCI` object via the `_dataset_1d_from` method.
+
+        This class's methods returns generators which create the instances of the `ImagingCI` objects. This ensures
+        that large sets of results can be efficiently loaded from the hard-disk and do not require storing all
+        `ImagingCI` instances in the memory at once.
+
+        For example, if the `aggregator` contains 3 model-fits, this class can be used to create a generator which
+        creates instances of the corresponding 3 `ImagingCI` objects.
+
+        If multiple `ImagingCI` objects were fitted simultaneously via analysis summing, the `fit.child_values()`
+        method is instead used to load lists of the data, noise-map, pre CTI data, layout and mask and combine them
+        into a list of `ImagingCI` objects.
+
+        If a `dataset_full` is input into the `Analysis` class when a model-fit is performed and therefore accessible
+        to the database, the input `use_dataset_full` can be switched in to load instead the full `ImagingCI` objects.
+
+        This can be done manually, but this object provides a more concise API.
+
+        Parameters
+        ----------
+        aggregator
+            A `PyAutoFit` aggregator object which can load the results of model-fits.
+        use_dataset_full
+            If a `dataset_full` is input into the `Analysis` class when a model-fit is performed and therefore
+            accessible to the database, the input `use_dataset_full` can be switched in to load instead the
+            full `ImagingCI` objects.
+        """
+        self.aggregator = aggregator
+        self.use_dataset_full = use_dataset_full
+
+    def dataset_list_gen_from(
+        self,
+    ):
+        """
+        Returns a generator of `ImagingCI` objects from an input aggregator.
+
+        See `__init__` for a description of how the `ImagingCI` objects are created by this method.
+
+        If a `dataset_full` is input into the `Analysis` class when a model-fit is performed and therefore accessible
+        to the database, the input `use_dataset_full` can be switched in to load instead the full `ImagingCI` objects.
+        """
+        func = partial(_imaging_ci_list_from, use_dataset_full=self.use_dataset_full)
+        return self.aggregator.map(func=func)
```

### Comparing `autocti-2024.1.27.4/autocti/charge_injection/ci_util.py` & `autocti-2024.5.16.0/autocti/charge_injection/ci_util.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/charge_injection/fit.py` & `autocti-2024.5.16.0/autocti/charge_injection/fit.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/charge_injection/hyper.py` & `autocti-2024.5.16.0/autocti/charge_injection/hyper.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/charge_injection/imaging/imaging.py` & `autocti-2024.5.16.0/autocti/charge_injection/imaging/imaging.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/charge_injection/imaging/settings.py` & `autocti-2024.5.16.0/autocti/charge_injection/imaging/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import copy
 
 import autoarray as aa
 
 from typing import Tuple
 
 
-class SettingsImagingCI(aa.SettingsImaging):
+class SettingsImagingCI:
     def __init__(
         self,
         parallel_pixels: Tuple[int, int] = None,
         serial_pixels: Tuple[int, int] = None,
     ):
         super().__init__()
```

### Comparing `autocti-2024.1.27.4/autocti/charge_injection/imaging/simulator.py` & `autocti-2024.5.16.0/autocti/extract/two_d/serial/calibration.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,272 +1,272 @@
-import copy
+from copy import deepcopy
 import numpy as np
-from typing import List
+from typing import Optional, Tuple
 
 import autoarray as aa
 
-from autoarray.dataset.imaging.simulator import SimulatorImaging
-
 from autocti.charge_injection.imaging.imaging import ImagingCI
-from autocti.charge_injection.layout import Layout2DCI
-from autocti.clocker.two_d import Clocker2D
-from autocti.extract.settings import SettingsExtract
-from autocti.model.model_util import CTI2D
-
-from typing import Optional
+from autocti.mask.mask_2d import Mask2D
 
 
-class SimulatorImagingCI(SimulatorImaging):
+class Extract2DSerialCalibration:
     def __init__(
         self,
-        pixel_scales: aa.type.PixelScales,
-        norm: float,
-        max_norm: float = np.inf,
-        column_sigma: Optional[float] = None,
-        row_slope: Optional[float] = 0.0,
-        non_uniform_norm_limit=None,
-        read_noise: Optional[float] = None,
-        charge_noise: Optional[float] = None,
-        noise_if_add_noise_false: float = 0.1,
-        noise_seed: int = -1,
-        ci_seed: int = -1,
+        shape_2d: Tuple[int, int],
+        region_list: aa.type.Region2DList,
+        serial_prescan: Optional[aa.type.Region2DLike] = None,
+        serial_overscan: Optional[aa.type.Region2DLike] = None,
     ):
-        """A class representing a Imaging observation, using the shape of the image, the pixel scale,
-        psf, exposure time, etc.
-
-        Parameters
-        ----------
-        exposure_time_map
-            The exposure time of an observation using this data_type.
         """
+        Class containing methods for extracting a serial calibration dataset from a 2D CTI calibration dataset.
 
-        super().__init__(
-            exposure_time=1.0,
-            noise_if_add_noise_false=noise_if_add_noise_false,
-            noise_seed=noise_seed,
-        )
-
-        self.pixel_scales = pixel_scales
-
-        self.norm = norm
-        self.max_norm = max_norm
-        self.column_sigma = column_sigma
-        self.row_slope = row_slope
-        self.non_uniform_norm_limit = non_uniform_norm_limit
-        self.read_noise = read_noise
-        self.charge_noise = charge_noise
+        The serial calibration region is the region of a dataset that is necessary for fitting a serial-only CTI
+        model. For example, for charge injection imaging, serial EPERs form only in rows of the CCD where charge
+        is injected and the regions in between have no signal. The serial calibration dataset therefore extracts only
+        these rows.
 
-        self.ci_seed = ci_seed
+        A subset of the serial calibration data may also be extracted (e.g. only the first row of every charge region)
+        for fast initial CTI modeling.
 
-    @property
-    def _ci_seed(self) -> int:
-        if self.ci_seed == -1:
-            return np.random.randint(0, int(1e9))
-        return self.ci_seed
+        This uses the `region_list`, which contains the regions with charge (e.g. the charge injection regions) in
+        pixel coordinates.
 
-    def median_list_from(self, total_columns: int) -> List[float]:
-        np.random.seed(self._ci_seed)
-
-        injection_norm_list = []
-
-        for column_number in range(total_columns):
-            injection_norm = 0
-
-            while injection_norm <= 0 or injection_norm >= self.max_norm:
-                injection_norm = np.random.normal(self.norm, self.column_sigma)
-
-            injection_norm_list.append(injection_norm)
+        Parameters
+        ----------
+        shape_2d
+            The two dimensional shape of the charge injection imaging, corresponding to the number of rows (pixels
+            in parallel direction) and columns (pixels in serial direction).
+        region_list
+            Integer pixel coordinates specifying the corners of each charge region (top-row, bottom-row,
+            left-column, right-column).
+        serial_prescan
+            Integer pixel coordinates specifying the corners of the serial prescan (top-row, bottom-row,
+            left-column, right-column).
+        serial_overscan
+            Integer pixel coordinates specifying the corners of the serial overscan (top-row, bottom-row,
+            left-column, right-column).
+        """
+        self.shape_2d = shape_2d
+        self.region_list = list(map(aa.Region2D, region_list))
+        self.serial_prescan = serial_prescan
+        self.serial_overscan = serial_overscan
 
-        return injection_norm_list
+    def array_2d_list_from(self, array: aa.Array2D):
+        """
+        Extract each charge injection region image for the serial calibration arrays when creating the
+        """
 
-    def injection_norm_list_with_limit_from(self, total_columns: int) -> List[float]:
-        injection_norm_list = self.median_list_from(
-            total_columns=self.non_uniform_norm_limit
+        calibration_region_list = list(
+            map(
+                lambda ci_region: ci_region.parallel_full_region_from(
+                    shape_2d=self.shape_2d
+                ),
+                self.region_list,
+            )
+        )
+        return list(
+            map(lambda region: array.native[region.slice], calibration_region_list)
         )
 
-        injection_norm_limited_list = []
+    def mask_2d_from(self, mask: aa.Mask2D, rows: Tuple[int, int]) -> Mask2D:
+        """
+        Extract a serial calibration array from a charge injection array, where this arrays is a sub-set of the
+        array which can be used for serial-only calibration. Specifically, this array is all charge injection
+        scans and their serial over-scan trails.
+
+        The diagram below illustrates the arrays that is extracted from a array with column=5:
+
+        ---KEY---
+        ---------
+
+        [] = read-out electronics   [==========] = read-out register
+
+        [xxxxxxxxxx]                [..........] = serial prescan       [ssssssssss] = serial overscan
+        [xxxxxxxxxx] = CCDPhase panel    [pppppppppp] = parallel overscan    [cccccccccc] = charge injection region
+        [xxxxxxxxxx]                [tttttttttt] = parallel / serial charge injection region trail
+
+        P = Parallel Direction      S = Serial Direction
+
+               [ppppppppppppppppppppp]
+               [pppppppppppppppppppp ]
+          [...][xxxxxxxxxxxxxxxxxxxxx][sss]
+          [...][ccccccccccccccccccccc][tst]
+        | [...][ccccccccccccccccccccc][sts]    |
+        | [...][xxxxxxxxxxxxxxxxxxxxx][sss]    | Direction
+        P [...][xxxxxxxxxxxxxxxxxxxxx][sss]    | of
+        | [...][ccccccccccccccccccccc][tst]    | clocking
+          [...][ccccccccccccccccccccc][sts]    |
+
+        []     [=====================]
+               <--------Ser---------
+
+        The extracted array keeps just the trails following all charge injection scans and replaces all other
+        values with 0s:
+
+        |                                      |
+        |      [cccccccccccccccc][tst]         | Direction
+        P      [cccccccccccccccc][tst]         | of
+        |      [cccccccccccccccc][tst]         | clocking
+               [cccccccccccccccc][tst]         |
 
-        for i in range(total_columns):
-            injection_norm = np.random.choice(injection_norm_list)
+        []     [=====================]
+               <--------Ser---------
+        """
 
-            injection_norm_limited_list.append(injection_norm)
+        calibration_region_list = list(
+            map(
+                lambda ci_region: ci_region.parallel_full_region_from(
+                    shape_2d=self.shape_2d
+                ),
+                self.region_list,
+            )
+        )
+        calibration_masks = list(
+            map(lambda region: mask[region.slice], calibration_region_list)
+        )
 
-        return injection_norm_limited_list
+        calibration_masks = list(
+            map(lambda mask: mask[rows[0] : rows[1], :], calibration_masks)
+        )
+        return Mask2D(
+            mask=np.concatenate(calibration_masks, axis=0),
+            pixel_scales=mask.pixel_scales,
+        )
 
-    def pre_cti_data_uniform_from(self, layout: Layout2DCI) -> aa.Array2D:
+    def array_2d_from(self, array: aa.Array2D, rows: Tuple[int, int]) -> aa.Array2D:
         """
-        Use this charge injection layout_ci to generate a pre-cti charge injection image. This is performed by \
-        going to its charge injection regions and adding the charge injection normalization value.
+        Extract a serial calibration array from a charge injection array, where this arrays is a sub-set of the
+        array which can be used for serial-only calibration. Specifically, this array is all charge injection
+        scans and their serial over-scan trails.
+
+        The diagram below illustrates the arrays that is extracted from a array with column=5:
+
+        [] = read-out electronics
+        [==========] = read-out register
+        [..........] = serial prescan
+        [pppppppppp] = parallel overscan
+        [ssssssssss] = serial overscan
+        [f#ff#f#f#f] = signal region (FPR) (0 / 1 indicate the region index)
+        [tttttttttt] = parallel / serial charge injection region trail
+
+               [ppppppppppppppppppppp]
+               [pppppppppppppppppppp ]
+          [...][xxxxxxxxxxxxxxxxxxxxx][sss]
+          [...][ccccccccccccccccccccc][tst]
+        | [...][ccccccccccccccccccccc][sts]    |
+        | [...][xxxxxxxxxxxxxxxxxxxxx][sss]    | Direction
+        P [...][xxxxxxxxxxxxxxxxxxxxx][sss]    | of
+        | [...][ccccccccccccccccccccc][tst]    | clocking
+          [...][ccccccccccccccccccccc][sts]    |
+
+        []     [=====================]
+               <--------Ser---------
+
+        The extracted array keeps just the trails following all charge injection scans and replaces all other
+        values with 0s:
+
+        |                                      |
+        |      [cccccccccccccccc][tst]         | Direction
+        P      [cccccccccccccccc][tst]         | of
+        |      [cccccccccccccccc][tst]         | clocking
+               [cccccccccccccccc][tst]         |
 
-        Parameters
-        ----------
-        shape_native
-            The image_shape of the pre_cti_datas to be created.
+        []     [=====================]
+               <--------Ser---------
         """
-        return layout.pre_cti_data_uniform_from(
-            norm=self.norm, pixel_scales=self.pixel_scales
+        calibration_images = self.array_2d_list_from(array=array)
+        calibration_images = list(
+            map(lambda image: image[rows[0] : rows[1], :], calibration_images)
         )
 
-    def pre_cti_data_non_uniform_from(self, layout: Layout2DCI) -> aa.Array2D:
-        """
-        Use this charge injection layout to generate a pre-cti charge injection image. This is performed by going
-        to its charge injection regions and adding an input normalization value to each column, which are
-        passed in as a list.
-
-        For one column of a non-uniform charge injection pre-cti image, this function assumes that each non-uniform
-        charge  injection region has the same overall normalization value. This assumes the spikes / troughs in the
-        injection current that cause non-uniformity occur in an identical fashion for each charge injection region.
-
-        Non-uniformity across the rows of a charge injection layout_ci is due to a drop-off in voltage in the current.
-        Therefore, it appears smooth and be modeled as an analytic function, which this code assumes is a
-        power-law with slope `row_slope`.
+        new_array = np.concatenate(calibration_images, axis=0)
 
-        Parameters
-        ----------
-        shape_native
-            The image_shape of the pre_cti_datas to be created.
-        row_slope
-            The power-law slope of non-uniformity in the row charge injection profile.
-        ci_seed
-            Input ci_seed for the random number generator to give reproducible results. A new ci_seed is always used for each \
-            pre_cti_datas, ensuring each non-uniform ci_region has the same column non-uniformity layout_ci.
-        """
+        mask_2d = self.mask_2d_from(mask=array.mask, rows=rows)
 
-        for region in layout.region_list:
-            if self.non_uniform_norm_limit is None:
-                injection_norm_list = self.median_list_from(
-                    total_columns=region.total_columns
-                )
-            else:
-                injection_norm_list = self.injection_norm_list_with_limit_from(
-                    total_columns=region.total_columns
-                )
+        return aa.Array2D(
+            values=new_array,
+            mask=mask_2d,
+            header=array.header,
+        )
 
-        return layout.pre_cti_data_non_uniform_from(
-            injection_norm_list=injection_norm_list,
-            pixel_scales=self.pixel_scales,
-            row_slope=self.row_slope,
+    def extracted_layout_from(self, layout, new_shape_2d, rows):
+        serial_prescan = (
+            (0, new_shape_2d[0], self.serial_prescan[2], self.serial_prescan[3])
+            if self.serial_prescan is not None
+            else None
+        )
+        serial_overscan = (
+            (0, new_shape_2d[0], self.serial_overscan[2], self.serial_overscan[3])
+            if self.serial_overscan is not None
+            else None
         )
 
-    def via_layout_from(
-        self,
-        layout: Layout2DCI,
-        clocker: Optional[Clocker2D],
-        cti: Optional[CTI2D],
-        cosmic_ray_map: Optional[aa.Array2D] = None,
-    ) -> ImagingCI:
-        """Simulate a charge injection image, including effects like noises.
+        x0 = self.region_list[0][2]
+        x1 = self.region_list[0][3]
+        offset = 0
+
+        new_pattern_region_list_ci = []
+
+        for region in self.region_list:
+            labelsize = rows[1] - rows[0]
+            new_pattern_region_list_ci.append(
+                aa.Region2D(region=(offset, offset + labelsize, x0, x1))
+            )
+            offset += labelsize
 
-        Parameters
-        ----------
-        pre_cti_data
-        cosmic_ray_map
-            The dimensions of the output simulated charge injection image.
-        frame_geometry
-            The quadrant geometry of the simulated image, defining where the parallel / serial overscans are and \
-            therefore the direction of clocking and rotations before input into the cti algorithm.
-        layout
-            The charge injection layout_ci (regions, normalization, etc.) of the charge injection image.
-        cti_params
-            The CTI model parameters (trap density, trap release_timescales etc.).
-        clocker
-            The settings that control the cti clocking algorithm (e.g. ccd well_depth express option).
-        read_noise
-            The FWHM of the Gaussian read-noises added to the image.
-        noise_seed
-            Seed for the read-noises added to the image.
+        new_layout = deepcopy(layout)
+        new_layout.region_list = new_pattern_region_list_ci
+        new_layout.serial_prescan = serial_prescan
+        new_layout.serial_overscan = serial_overscan
+
+        return new_layout
+
+    def imaging_ci_from(self, dataset: ImagingCI, rows) -> ImagingCI:
+        """
+        Returnss a function to extract a serial section for given rows
         """
 
-        if self.column_sigma is not None:
-            pre_cti_data = self.pre_cti_data_non_uniform_from(layout=layout)
-        else:
-            pre_cti_data = self.pre_cti_data_uniform_from(layout=layout)
+        from autocti.charge_injection.imaging.imaging import ImagingCI
 
-        return self.via_pre_cti_data_from(
-            pre_cti_data=pre_cti_data.native,
-            layout=layout,
-            clocker=clocker,
-            cti=cti,
-            cosmic_ray_map=cosmic_ray_map,
+        cosmic_ray_map = (
+            dataset.layout.extract.serial_calibration.array_2d_from(
+                array=dataset.cosmic_ray_map, rows=rows
+            )
+            if dataset.cosmic_ray_map is not None
+            else None
         )
 
-    def via_pre_cti_data_from(
-        self,
-        pre_cti_data: aa.Array2D,
-        layout: Layout2DCI,
-        clocker: Optional[Clocker2D],
-        cti: Optional[CTI2D],
-        cosmic_ray_map: Optional[aa.Array2D] = None,
-    ) -> ImagingCI:
-        pre_cti_data = pre_cti_data.native
-
-        if cosmic_ray_map is not None:
-            pre_cti_data += cosmic_ray_map.native
-
-        if self.charge_noise is not None:
-            pre_cti_data = layout.extract.parallel_fpr.add_gaussian_noise_to(
-                array=pre_cti_data,
-                noise_sigma=self.charge_noise,
-                noise_seed=self.noise_seed,
-                settings=SettingsExtract(
-                    pixels_from_end=layout.extract.parallel_fpr.total_rows_min
-                ),
-            )
+        if dataset.noise_scaling_map_dict is not None:
+            noise_scaling_map_dict = {
+                key: dataset.layout.extract.serial_calibration.array_2d_from(
+                    array=noise_scaling_map, rows=rows
+                )
+                for key, noise_scaling_map in dataset.noise_scaling_map_dict.items()
+            }
 
-        if cti is not None:
-            post_cti_data = clocker.add_cti(data=pre_cti_data, cti=cti)
         else:
-            post_cti_data = copy.copy(pre_cti_data)
+            noise_scaling_map_dict = None
 
-        if cosmic_ray_map is not None:
-            pre_cti_data -= cosmic_ray_map.native
-
-        return self.via_post_cti_data_from(
-            post_cti_data=post_cti_data,
-            pre_cti_data=pre_cti_data,
-            layout=layout,
-            cosmic_ray_map=cosmic_ray_map,
+        image = dataset.layout.extract.serial_calibration.array_2d_from(
+            array=dataset.data, rows=rows
         )
 
-    def via_post_cti_data_from(
-        self,
-        post_cti_data: aa.Array2D,
-        pre_cti_data: aa.Array2D,
-        layout: Layout2DCI,
-        cosmic_ray_map: Optional[aa.Array2D] = None,
-    ) -> ImagingCI:
-        if self.read_noise is not None:
-            ci_image = aa.preprocess.data_with_gaussian_noise_added(
-                data=post_cti_data, sigma=self.read_noise, seed=self.noise_seed
-            )
-
-            ci_image = aa.Array2D.no_mask(
-                values=ci_image, pixel_scales=self.pixel_scales
-            )
+        mask = self.mask_2d_from(mask=dataset.mask, rows=rows)
 
-            ci_noise_map = (
-                self.read_noise
-                * aa.Array2D.ones(
-                    shape_native=layout.shape_2d, pixel_scales=self.pixel_scales
-                ).native
-            )
-        else:
-            ci_image = post_cti_data
-            ci_noise_map = aa.Array2D.full(
-                fill_value=self.noise_if_add_noise_false,
-                shape_native=layout.shape_2d,
-                pixel_scales=self.pixel_scales,
-            ).native
-
-        return ImagingCI(
-            data=aa.Array2D.no_mask(
-                values=ci_image.native, pixel_scales=self.pixel_scales
+        dataset = ImagingCI(
+            data=image,
+            noise_map=dataset.layout.extract.serial_calibration.array_2d_from(
+                array=dataset.noise_map, rows=rows
             ),
-            noise_map=aa.Array2D.no_mask(
-                values=ci_noise_map, pixel_scales=self.pixel_scales
+            pre_cti_data=dataset.layout.extract.serial_calibration.array_2d_from(
+                array=dataset.pre_cti_data, rows=rows
             ),
-            pre_cti_data=aa.Array2D.no_mask(
-                values=pre_cti_data.native, pixel_scales=self.pixel_scales
+            layout=dataset.layout.extract.serial_calibration.extracted_layout_from(
+                layout=dataset.layout, new_shape_2d=image.shape, rows=rows
             ),
             cosmic_ray_map=cosmic_ray_map,
-            layout=layout,
+            noise_scaling_map_dict=noise_scaling_map_dict,
+            fpr_value=dataset.fpr_value,
+            settings_dict=dataset.settings_dict,
         )
+
+        return dataset.apply_mask(mask=mask)
```

### Comparing `autocti-2024.1.27.4/autocti/charge_injection/layout.py` & `autocti-2024.5.16.0/autocti/charge_injection/layout.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/charge_injection/master.py` & `autocti-2024.5.16.0/autocti/charge_injection/master.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/charge_injection/mock/mock_result.py` & `autocti-2024.5.16.0/autocti/charge_injection/mock/mock_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
             instance=instance,
             model=model,
             analysis=analysis,
             search=search,
         )
 
         self.previous_model = model
-        self.gaussian_tuples = None
+        self.prior_means = None
         self.mask = None
         self.positions = None
         self.mask = mask
         self.model_image = model_image
         self.noise_scaling_map_dict_list_of_regions_ci = (
             noise_scaling_map_dict_list_of_regions_ci
         )
```

### Comparing `autocti-2024.1.27.4/autocti/charge_injection/model/result.py` & `autocti-2024.5.16.0/autocti/charge_injection/model/result.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/charge_injection/model/visualizer.py` & `autocti-2024.5.16.0/autocti/charge_injection/model/plotter_interface.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import logging
 
 import autoarray.plot as aplt
 
 import autocti.plot as aplt
 
-from autocti.model.visualizer import Visualizer
-from autocti.model.visualizer import plot_setting
+from autocti.model.plotter_interface import PlotterInterface
+from autocti.model.plotter_interface import plot_setting
 
 from autocti import exc
 
 logger = logging.getLogger(__name__)
 
 logger.setLevel(level="INFO")
 
 
-class VisualizerImagingCI(Visualizer):
-    def visualize_dataset(self, dataset, folder_suffix: str = ""):
+class PlotterInterfaceImagingCI(PlotterInterface):
+    def dataset(self, dataset, folder_suffix: str = ""):
         def should_plot(name):
             return plot_setting(section="dataset", name=name)
 
         mat_plot = self.mat_plot_2d_from(subfolders=f"dataset{folder_suffix}")
 
         dataset_plotter = aplt.ImagingCIPlotter(
             dataset=dataset, mat_plot_2d=mat_plot, include_2d=self.include_2d
@@ -32,15 +32,15 @@
             data=should_plot("data"),
             noise_map=should_plot("noise_map"),
             signal_to_noise_map=should_plot("signal_to_noise_map"),
             pre_cti_data=should_plot("pre_cti_data"),
             cosmic_ray_map=should_plot("cosmic_ray_map"),
         )
 
-    def visualize_dataset_regions(self, dataset, region_list, folder_suffix: str = ""):
+    def dataset_regions(self, dataset, region_list, folder_suffix: str = ""):
         def should_plot(name):
             return plot_setting(section="dataset", name=name)
 
         mat_plot = self.mat_plot_1d_from(subfolders=f"dataset{folder_suffix}")
 
         dataset_plotter = aplt.ImagingCIPlotter(
             dataset=dataset, mat_plot_1d=mat_plot, include_2d=self.include_2d
@@ -61,15 +61,15 @@
                 )
 
             except (exc.RegionException, TypeError, ValueError):
                 logger.info(
                     f"VISUALIZATION - Could not visualize the ImagingCI 1D {region}"
                 )
 
-    def visualize_dataset_combined(
+    def dataset_combined(
         self, dataset_list, folder_suffix: str = "", filename_suffix: str = ""
     ):
         def should_plot(name):
             return plot_setting(section="dataset", name=name)
 
         mat_plot = self.mat_plot_2d_from(subfolders=f"dataset_combined{folder_suffix}")
 
@@ -109,15 +109,15 @@
             )
             multi_plotter.subplot_of_figure(
                 func_name="figures_2d",
                 figure_name="cosmic_ray_map",
                 filename_suffix=filename_suffix,
             )
 
-    def visualize_dataset_regions_combined(
+    def dataset_regions_combined(
         self,
         dataset_list,
         region_list,
         folder_suffix: str = "",
         filename_suffix: str = "",
     ):
         def should_plot(name):
@@ -168,15 +168,15 @@
                 if should_plot(figure_name):
                     multi_plotter.subplot_of_figure(
                         func_name="figures_1d_data_binned",
                         figure_name=figure_name,
                         filename_suffix=f"{filename_suffix}",
                     )
 
-    def visualize_fit(self, fit, during_analysis, folder_suffix: str = ""):
+    def fit(self, fit, during_analysis, folder_suffix: str = ""):
         def should_plot(name):
             return plot_setting(section="fit", name=name)
 
         mat_plot = self.mat_plot_2d_from(subfolders=f"fit_dataset{folder_suffix}")
 
         fit_plotter = aplt.FitImagingCIPlotter(
             fit=fit, mat_plot_2d=mat_plot, include_2d=self.include_2d
@@ -203,20 +203,20 @@
                     post_cti_data=True,
                     residual_map=True,
                     normalized_residual_map=True,
                     chi_squared_map=True,
                 )
 
             if should_plot("all_at_end_fits"):
-                self.visualize_fit_in_fits(fit=fit)
+                self.fit_in_fits(fit=fit)
 
         if should_plot("subplot_fit"):
             fit_plotter.subplot_fit()
 
-    def visualize_fit_1d_regions(
+    def fit_1d_regions(
         self, fit, region_list, during_analysis, folder_suffix: str = ""
     ):
         def should_plot(name):
             return plot_setting(section="fit", name=name)
 
         mat_plot = self.mat_plot_1d_from(subfolders=f"fit_dataset{folder_suffix}")
 
@@ -259,17 +259,15 @@
                         )
 
             except (exc.RegionException, TypeError, ValueError):
                 logger.info(
                     f"VISUALIZATION - Could not visualize the ImagingCI 1D {region}"
                 )
 
-    def visualize_fit_combined(
-        self, fit_list, during_analysis, folder_suffix: str = ""
-    ):
+    def fit_combined(self, fit_list, during_analysis, folder_suffix: str = ""):
         def should_plot(name):
             return plot_setting(section="fit", name=name)
 
         mat_plot = self.mat_plot_2d_from(
             subfolders=f"fit_dataset_combined{folder_suffix}"
         )
 
@@ -292,15 +290,15 @@
             )
 
         if should_plot("chi_squared_map"):
             multi_plotter.subplot_of_figure(
                 func_name="figures_2d", figure_name="chi_squared_map"
             )
 
-    def visualize_fit_1d_regions_combined(
+    def fit_1d_regions_combined(
         self, fit_list, region_list, during_analysis, folder_suffix: str = ""
     ):
         def should_plot(name):
             return plot_setting(section="fit", name=name)
 
         mat_plot = self.mat_plot_1d_from(
             subfolders=f"fit_dataset_combined{folder_suffix}"
@@ -378,15 +376,15 @@
             ]:
                 if should_plot(figure_name):
                     multi_plotter.subplot_of_figure(
                         func_name="figures_1d_data_binned",
                         figure_name=figure_name,
                     )
 
-    def visualize_fit_in_fits(self, fit):
+    def fit_in_fits(self, fit):
         mat_plot_2d = self.mat_plot_2d_from(subfolders="fit_imaging/fit", format="fit")
 
         fit_plotter = aplt.FitImagingCIPlotter(
             fit=fit, mat_plot_2d=mat_plot_2d, include_2d=self.include_2d
         )
 
         fit_plotter.figures_2d(
```

### Comparing `autocti-2024.1.27.4/autocti/charge_injection/ou_sim_ci.py` & `autocti-2024.5.16.0/autocti/charge_injection/ou_sim_ci.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/charge_injection/plot/fit_ci_plotters.py` & `autocti-2024.5.16.0/autocti/charge_injection/plot/fit_ci_plotters.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,15 +261,15 @@
                     title=f"Data {title_str} [log10]",
                     yunit="e-",
                     filename=f"data_logy_{region}",
                 ),
             )
 
         if noise_map:
-            y = self.extract_region_from(array=self.fit.image, region=region)
+            y = self.extract_region_from(array=self.fit.data, region=region)
 
             self.mat_plot_1d.plot_yx(
                 y=y,
                 x=range(len(y)),
                 visuals_1d=self.visuals_1d,
                 auto_labels=AutoLabels(
                     title=f"Noise-Map {title_str}",
@@ -415,18 +415,18 @@
             Whether to plot the data binned over columns with the FPR regions included.
         """
 
         fpr_mask = self.fpr_mask_from()
 
         if rows_fpr:
             data = copy.copy(self.dataset.data)
-            y = data.apply_mask(mask=np.invert(fpr_mask)).binned_across_rows
+            y = data.apply_mask(mask=fpr_mask.invert()).binned_across_rows
 
             model_data = copy.copy(self.fit.model_data)
-            y_extra = model_data.apply_mask(mask=np.invert(fpr_mask)).binned_across_rows
+            y_extra = model_data.apply_mask(mask=fpr_mask.invert()).binned_across_rows
 
             self.mat_plot_1d.plot_yx(
                 y=y,
                 x=range(len(y)),
                 y_extra=y_extra,
                 text_manual_dict=self.text_manual_dict_from(),
                 text_manual_dict_y=self.text_manual_dict_y_from(),
@@ -457,20 +457,18 @@
                     yunit="e-",
                     filename=f"fit_data_binned_rows_no_fpr",
                 ),
             )
 
         if columns_fpr:
             data = copy.copy(self.dataset.data)
-            y = data.apply_mask(mask=np.invert(fpr_mask)).binned_across_columns
+            y = data.apply_mask(mask=fpr_mask).binned_across_columns
 
             model_data = copy.copy(self.fit.model_data)
-            y_extra = model_data.apply_mask(
-                mask=np.invert(fpr_mask)
-            ).binned_across_columns
+            y_extra = model_data.apply_mask(mask=fpr_mask).binned_across_columns
 
             self.mat_plot_1d.plot_yx(
                 y=y,
                 x=range(len(y)),
                 y_extra=y_extra,
                 text_manual_dict=self.text_manual_dict_from(),
                 text_manual_dict_y=self.text_manual_dict_y_from(),
```

### Comparing `autocti-2024.1.27.4/autocti/charge_injection/plot/imaging_ci_plotters.py` & `autocti-2024.5.16.0/autocti/charge_injection/plot/imaging_ci_plotters.py`

 * *Files 2% similar despite different names*

```diff
@@ -338,15 +338,15 @@
         """
 
         fpr_mask = self.fpr_mask_from()
 
         if rows_fpr:
             data = copy.copy(self.dataset.data)
 
-            y = data.apply_mask(mask=np.invert(fpr_mask)).binned_across_rows
+            y = data.apply_mask(mask=fpr_mask.invert()).binned_across_rows
 
             self.mat_plot_1d.plot_yx(
                 y=y,
                 x=range(len(y)),
                 text_manual_dict=self.text_manual_dict_from(),
                 text_manual_dict_y=self.text_manual_dict_y_from(),
                 visuals_1d=self.get_visuals_1d(),
@@ -374,15 +374,15 @@
                     filename=f"data_binned_rows_no_fpr",
                 ),
             )
 
         if columns_fpr:
             data = copy.copy(self.dataset.data)
 
-            y = data.apply_mask(mask=np.invert(fpr_mask)).binned_across_columns
+            y = data.apply_mask(mask=fpr_mask).binned_across_columns
 
             self.mat_plot_1d.plot_yx(
                 y=y,
                 x=range(len(y)),
                 text_manual_dict=self.text_manual_dict_from(),
                 text_manual_dict_y=self.text_manual_dict_y_from(),
                 visuals_1d=self.get_visuals_1d(),
```

### Comparing `autocti-2024.1.27.4/autocti/clocker/abstract.py` & `autocti-2024.5.16.0/autocti/clocker/abstract.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,12 @@
-from typing import List, Optional
-
 from arcticpy import CCD
 from arcticpy import CCDPhase
-from arcticpy import PixelBounce
-from arcticpy import TrapInstantCapture
 
 from autoconf.dictable import from_json, output_to_json
 
-from autocti import exc
-
 
 class AbstractClocker:
     def __init__(self, iterations: int = 1, verbosity: int = 0):
         """
         An abstract clocker, which wraps the c++ arctic CTI clocking algorithm in **PyAutoCTI**.
 
         Parameters
```

### Comparing `autocti-2024.1.27.4/autocti/clocker/one_d.py` & `autocti-2024.5.16.0/autocti/clocker/one_d.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/clocker/two_d.py` & `autocti-2024.5.16.0/autocti/clocker/two_d.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/config/notation.yaml` & `autocti-2024.5.16.0/autocti/config/notation.yaml`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/config/priors/ccd.yaml` & `autocti-2024.5.16.0/autocti/config/priors/ccd.yaml`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/config/priors/traps.yaml` & `autocti-2024.5.16.0/autocti/config/priors/traps.yaml`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/config/visualize.yaml` & `autocti-2024.5.16.0/autocti/config/visualize.yaml`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/cosmics/cosmics.py` & `autocti-2024.5.16.0/autocti/cosmics/cosmics.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/cosmics/cr_distances.py` & `autocti-2024.5.16.0/autocti/cosmics/cr_distances.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/cosmics/cr_lengths.py` & `autocti-2024.5.16.0/autocti/cosmics/cr_lengths.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/dataset_1d/dataset_1d/dataset_1d.py` & `autocti-2024.5.16.0/autocti/dataset_1d/dataset_1d/dataset_1d.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 import numpy as np
 from pathlib import Path
 from typing import Optional, Dict, Union
 
 import autoarray as aa
 
 from autocti import exc
-from autocti.dataset_1d.dataset_1d.settings import SettingsDataset1D
 from autocti.extract.settings import SettingsExtract
 from autocti.layout.one_d import Layout1D
 
 
 class Dataset1D(aa.AbstractDataset):
     def __init__(
         self,
         data: aa.Array1D,
         noise_map: aa.Array1D,
         pre_cti_data: aa.Array1D,
         layout: Layout1D,
         fpr_value: Optional[float] = None,
-        settings: SettingsDataset1D = SettingsDataset1D(),
         settings_dict: Optional[Dict] = None,
     ):
-        super().__init__(data=data, noise_map=noise_map, settings=settings)
+        super().__init__(data=data, noise_map=noise_map)
 
         self.data = data
         self.noise_map = noise_map
         self.pre_cti_data = pre_cti_data
         self.layout = layout
 
         if fpr_value is None:
@@ -56,17 +54,14 @@
             noise_map=noise_map,
             pre_cti_data=self.pre_cti_data,
             layout=self.layout,
             fpr_value=self.fpr_value,
             settings_dict=self.settings_dict,
         )
 
-    def apply_settings(self, settings: SettingsDataset1D) -> "Dataset1D":
-        return self
-
     @classmethod
     def from_fits(
         cls,
         pixel_scales: aa.type.PixelScales,
         layout: Layout1D,
         data_path: Optional[Union[Path, str]] = None,
         data_hdu: int = 0,
```

### Comparing `autocti-2024.1.27.4/autocti/dataset_1d/dataset_1d/simulator.py` & `autocti-2024.5.16.0/autocti/dataset_1d/dataset_1d/simulator.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/dataset_1d/fit.py` & `autocti-2024.5.16.0/autocti/dataset_1d/fit.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/dataset_1d/model/visualizer.py` & `autocti-2024.5.16.0/autocti/dataset_1d/model/plotter_interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import logging
 
 import autocti.plot as aplt
 
-from autocti.model.visualizer import Visualizer
-from autocti.model.visualizer import plot_setting
+from autocti.model.plotter_interface import PlotterInterface
+from autocti.model.plotter_interface import plot_setting
 from autocti import exc
 
 logger = logging.getLogger(__name__)
 
 logger.setLevel(level="INFO")
 
 
-class VisualizerDataset1D(Visualizer):
-    def visualize_dataset(self, dataset, folder_suffix=""):
+class PlotterInterfaceDataset1D(PlotterInterface):
+    def dataset(self, dataset, folder_suffix=""):
         def should_plot(name):
             return plot_setting(section="dataset", name=name)
 
         mat_plot_1d = self.mat_plot_1d_from(subfolders=f"dataset{folder_suffix}")
 
         dataset_plotter = aplt.Dataset1DPlotter(
             dataset=dataset, mat_plot_1d=mat_plot_1d, include_1d=self.include_1d
@@ -29,15 +29,15 @@
             data=should_plot("data"),
             data_logy=should_plot("data_logy"),
             noise_map=should_plot("noise_map"),
             signal_to_noise_map=should_plot("signal_to_noise_map"),
             pre_cti_data=should_plot("pre_cti_data"),
         )
 
-    def visualize_dataset_regions(self, dataset, region_list, folder_suffix=""):
+    def dataset_regions(self, dataset, region_list, folder_suffix=""):
         def should_plot(name):
             return plot_setting(section="dataset", name=name)
 
         mat_plot_1d = self.mat_plot_1d_from(subfolders=f"dataset{folder_suffix}")
 
         dataset_plotter = aplt.Dataset1DPlotter(
             dataset=dataset, mat_plot_1d=mat_plot_1d, include_1d=self.include_1d
@@ -58,15 +58,15 @@
                 )
 
             except (exc.RegionException, TypeError, ValueError):
                 logger.info(
                     f"VISUALIZATION - Could not visualize the Dataset1D {region}"
                 )
 
-    def visualize_dataset_combined(self, dataset_list, folder_suffix=""):
+    def dataset_combined(self, dataset_list, folder_suffix=""):
         def should_plot(name):
             return plot_setting(section="dataset", name=name)
 
         mat_plot_1d = self.mat_plot_1d_from(subfolders=f"dataset{folder_suffix}")
 
         dataset_plotter_list = [
             aplt.Dataset1DPlotter(
@@ -75,17 +75,15 @@
             for dataset in dataset_list
         ]
         multi_plotter = aplt.MultiFigurePlotter(plotter_list=dataset_plotter_list)
 
         if should_plot("subplot_dataset"):
             multi_plotter.subplot_of_figure(func_name="figures_1d", figure_name="data")
 
-    def visualize_dataset_regions_combined(
-        self, dataset_list, region_list, folder_suffix=""
-    ):
+    def dataset_regions_combined(self, dataset_list, region_list, folder_suffix=""):
         def should_plot(name):
             return plot_setting(section="dataset", name=name)
 
         mat_plot_1d = self.mat_plot_1d_from(subfolders=f"dataset{folder_suffix}")
 
         dataset_plotter_list = [
             aplt.Dataset1DPlotter(
@@ -113,15 +111,15 @@
                         filename_suffix=f"_{region}",
                     )
             except (exc.RegionException, TypeError, ValueError):
                 logger.info(
                     f"VISUALIZATION - Could not visualize the Dataset1D {region}"
                 )
 
-    def visualize_fit(self, fit, during_analysis, folder_suffix=""):
+    def fit(self, fit, during_analysis, folder_suffix=""):
         def should_plot(name):
             return plot_setting(section="fit", name=name)
 
         mat_plot_1d = self.mat_plot_1d_from(subfolders=f"fit_dataset{folder_suffix}")
 
         fit_plotter = aplt.FitDataset1DPlotter(
             fit=fit, mat_plot_1d=mat_plot_1d, include_1d=self.include_1d
@@ -153,17 +151,15 @@
                     normalized_residual_map=True,
                     chi_squared_map=True,
                 )
 
         if should_plot("subplot_fit"):
             fit_plotter.subplot_fit()
 
-    def visualize_fit_regions(
-        self, fit, region_list, during_analysis, folder_suffix=""
-    ):
+    def fit_regions(self, fit, region_list, during_analysis, folder_suffix=""):
         def should_plot(name):
             return plot_setting(section="fit", name=name)
 
         mat_plot_1d = self.mat_plot_1d_from(subfolders=f"fit_dataset{folder_suffix}")
 
         fit_plotter = aplt.FitDataset1DPlotter(
             fit=fit, mat_plot_1d=mat_plot_1d, include_1d=self.include_1d
@@ -189,15 +185,15 @@
                 )
 
             except (exc.RegionException, TypeError, ValueError):
                 logger.info(
                     f"VISUALIZATION - Could not visualize the Dataset1D {region}"
                 )
 
-    def visualize_fit_combined(self, fit_list, during_analysis, folder_suffix=""):
+    def fit_combined(self, fit_list, during_analysis, folder_suffix=""):
         def should_plot(name):
             return plot_setting(section="fit", name=name)
 
         mat_plot_1d = self.mat_plot_1d_from(
             subfolders=f"fit_dataset_combined{folder_suffix}"
         )
 
@@ -233,15 +229,15 @@
             )
 
         if should_plot("chi_squared_map"):
             multi_plotter.subplot_of_figure(
                 func_name="figures_1d", figure_name="chi_squared_map"
             )
 
-    def visualize_fit_region_combined(
+    def fit_region_combined(
         self, fit_list, region_list, during_analysis, folder_suffix=""
     ):
         def should_plot(name):
             return plot_setting(section="fit", name=name)
 
         mat_plot_1d = self.mat_plot_1d_from(
             subfolders=f"fit_dataset_combined{folder_suffix}"
```

### Comparing `autocti-2024.1.27.4/autocti/dataset_1d/plot/dataset_1d_plotters.py` & `autocti-2024.5.16.0/autocti/dataset_1d/plot/dataset_1d_plotters.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/dataset_1d/plot/fit_plotters.py` & `autocti-2024.5.16.0/autocti/dataset_1d/plot/fit_plotters.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/exc.py` & `autocti-2024.5.16.0/autocti/exc.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/extract/one_d/abstract.py` & `autocti-2024.5.16.0/autocti/extract/one_d/abstract.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import copy
 import numpy as np
 from typing import List, Optional, Tuple
 
 import autoarray as aa
+from autoarray import Mask1D
 
 from autocti.extract.settings import SettingsExtract
 
 
 class Extract1D:
     def __init__(
         self,
@@ -133,15 +134,18 @@
 
         stacked_array_1d = np.mean(
             np.asarray(arr_list), axis=0, where=np.invert(np.asarray(mask_1d_list))
         )
 
         return aa.Array1D(
             values=np.asarray(stacked_array_1d.data),
-            mask=sum(mask_1d_list) == len(mask_1d_list),
+            mask=aa.Mask1D(
+                sum(mask_1d_list) == len(mask_1d_list),
+                pixel_scales=mask_1d_list[0].pixel_scales,
+            ),
         ).native
 
     def add_to_array(
         self, new_array: aa.Array1D, array: aa.Array1D, settings: SettingsExtract
     ) -> aa.Array1D:
         """
         Extracts the region (e.g. the FPRs) from the line dataset and adds them to a line dataset.
```

### Comparing `autocti-2024.1.27.4/autocti/extract/one_d/eper.py` & `autocti-2024.5.16.0/autocti/extract/one_d/eper.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/extract/one_d/fpr.py` & `autocti-2024.5.16.0/autocti/extract/one_d/fpr.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/extract/one_d/master.py` & `autocti-2024.5.16.0/autocti/extract/one_d/master.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/extract/one_d/overscan.py` & `autocti-2024.5.16.0/autocti/extract/one_d/overscan.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/extract/settings.py` & `autocti-2024.5.16.0/autocti/extract/settings.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/extract/two_d/abstract.py` & `autocti-2024.5.16.0/autocti/extract/two_d/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from typing import Optional, List, Tuple, Union
+from typing import Optional, List, Tuple
 
 import autoarray as aa
 
 from autocti.charge_injection.imaging.imaging import ImagingCI
 from autocti.dataset_1d.dataset_1d.dataset_1d import Dataset1D
 from autocti.extract.settings import SettingsExtract
 from autocti.layout.one_d import Layout1D
@@ -230,15 +230,15 @@
         return [
             aa.Array2D(values=arr, mask=mask_2d).native
             for arr, mask_2d in zip(arr_list, mask_2d_list)
         ]
 
     def stacked_array_2d_from(
         self, array: aa.Array2D, settings: SettingsExtract
-    ) -> np.ndarray:
+    ) -> aa.Array2D:
         """
         Extract a region (e.g. the parallel FPR) of every signal region (e.g. the charge injection region of charge
         injection data) on the CTI calibration data and stack them by taking their mean.
 
         This returns the 2D average of the extracted regions (e.g. the parallel FPRs) of all of the charge injection
         regions, which for certain CCD charge injection electronics one may expect to be similar.
 
@@ -269,20 +269,23 @@
 
         stacked_array_2d = np.mean(
             arr_list, axis=0, where=np.invert(np.asarray(mask_2d_list))
         )
 
         return aa.Array2D(
             values=np.asarray(stacked_array_2d.data),
-            mask=sum(mask_2d_list) == len(mask_2d_list),
+            mask=Mask2D(
+                sum(mask_2d_list) == len(mask_2d_list),
+                pixel_scales=array.pixel_scale,
+            ),
         ).native
 
     def stacked_array_2d_total_pixels_from(
         self, array: aa.Array2D, settings: SettingsExtract
-    ) -> np.ndarray:
+    ) -> aa.Array2D:
         """
         The function `stacked_array_2d_from` extracts a region (e.g. the parallel FPR) of every charge injection
         region on the charge injection image and stacks them by taking their mean.
 
         If the data being stacked is a noise-map, we need to know how many pixels were used in the stacking of every
         final pixel on the stacked 2d array in order to compute the new noise map via quadrature.
 
@@ -301,15 +304,17 @@
             for region in self.region_list_from(settings=settings)
         ]
 
         arr_total_pixels = sum([np.invert(mask_2d) for mask_2d in mask_2d_list])
 
         return aa.Array2D(
             values=np.asarray(arr_total_pixels),
-            mask=sum(mask_2d_list) == len(mask_2d_list),
+            mask=Mask2D(
+                sum(mask_2d_list) == len(mask_2d_list), pixel_scales=array.pixel_scale
+            ),
         ).native
 
     def binned_array_1d_from(
         self, array: aa.Array2D, settings: SettingsExtract
     ) -> aa.Array1D:
         """
         Extract a region (e.g. the parallel FPR) of every signal region (e.g. the charge injection region of
```

### Comparing `autocti-2024.1.27.4/autocti/extract/two_d/extract_2d_util.py` & `autocti-2024.5.16.0/autocti/extract/two_d/extract_2d_util.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/extract/two_d/master.py` & `autocti-2024.5.16.0/autocti/extract/two_d/master.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/extract/two_d/parallel/abstract.py` & `autocti-2024.5.16.0/autocti/extract/two_d/parallel/abstract.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/extract/two_d/parallel/calibration.py` & `autocti-2024.5.16.0/autocti/extract/two_d/parallel/calibration.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/extract/two_d/parallel/eper.py` & `autocti-2024.5.16.0/autocti/extract/two_d/parallel/eper.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,16 +139,16 @@
         """
 
         array_2d = array.native.copy()
 
         for region in self.region_list:
             array_2d[region.slice] = 0.0
 
-        array_2d.native[self.serial_prescan.slice] = 0.0
-        array_2d.native[self.serial_overscan.slice] = 0.0
+        array_2d[self.serial_overscan.slice] = 0.0
+        array_2d[self.serial_prescan.slice] = 0.0
 
         return array_2d
 
     def binned_region_1d_from(self, settings: SettingsExtract) -> aa.Region1D:
         """
         The `Extract` objects allow one to extract a `Dataset1D` from a 2D CTI dataset, which is used to perform
         CTI modeling in 1D.
```

### Comparing `autocti-2024.1.27.4/autocti/extract/two_d/parallel/fpr.py` & `autocti-2024.5.16.0/autocti/extract/two_d/parallel/fpr.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,33 +5,36 @@
 import autoarray as aa
 
 from autocti.extract.two_d.parallel.abstract import Extract2DParallel
 from autocti.extract.settings import SettingsExtract
 
 from autocti.extract.two_d import extract_2d_util
 
-@aa.numba_util.jit()
-def capture_estimate_from(array, mask, x0, x1, y0, y1, pixels_from_start, pixels_from_end):
 
+@aa.numba_util.jit()
+def capture_estimate_from(
+    array, mask, x0, x1, y0, y1, pixels_from_start, pixels_from_end
+):
     value_list = []
 
     for x in range(x0, x1):
-
-        fpr = array[y0: y1, x]
-        mask_ = mask[y0: y1, x]
+        fpr = array[y0:y1, x]
+        mask_ = mask[y0:y1, x]
 
         if np.sum(mask_):
-
-            injection_estimate = np.median(fpr[-pixels_from_end:][mask_[-pixels_from_end:]])
-            capture_estimate = np.sum(injection_estimate - fpr[0:pixels_from_start][mask_[0:pixels_from_start]])
-
-            value_list.append(
-                capture_estimate
+            injection_estimate = np.median(
+                fpr[-pixels_from_end:][mask_[-pixels_from_end:]]
+            )
+            capture_estimate = np.sum(
+                injection_estimate
+                - fpr[0:pixels_from_start][mask_[0:pixels_from_start]]
             )
 
+            value_list.append(capture_estimate)
+
     return value_list
 
 
 class Extract2DParallelFPR(Extract2DParallel):
     def region_list_from(self, settings: SettingsExtract) -> List[aa.Region2D]:
         """
         Returns a list of the 2D parallel FPR regions from the `region_list` containing signal  (e.g. the charge
@@ -151,17 +154,16 @@
         Returns
         -------
         An estimate of the total number of electrons captured in each column of the parallel FPRs.
         """
         capture_list = []
 
         for region in self.region_list:
-
             capture_list_ = capture_estimate_from(
-                array=array.native,
+                array=np.array(array.native),
                 mask=np.invert(array.mask),
                 x0=int(region.x0),
                 x1=int(region.x1),
                 y0=int(region.y0),
                 y1=int(region.y1),
                 pixels_from_start=pixels_from_start,
                 pixels_from_end=pixels_from_end,
```

### Comparing `autocti-2024.1.27.4/autocti/extract/two_d/parallel/overscan.py` & `autocti-2024.5.16.0/autocti/extract/two_d/parallel/overscan.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/extract/two_d/parallel/pedestal.py` & `autocti-2024.5.16.0/autocti/extract/two_d/parallel/pedestal.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/extract/two_d/parallel/pre_injection.py` & `autocti-2024.5.16.0/autocti/extract/two_d/parallel/pre_injection.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/extract/two_d/serial/abstract.py` & `autocti-2024.5.16.0/autocti/extract/two_d/serial/abstract.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/extract/two_d/serial/calibration.py` & `autocti-2024.5.16.0/autocti/layout/two_d.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,272 +1,286 @@
 from copy import deepcopy
 import numpy as np
-from typing import Optional, Tuple
+from typing import List, Optional, Tuple
 
 import autoarray as aa
 
-from autocti.charge_injection.imaging.imaging import ImagingCI
-from autocti.mask.mask_2d import Mask2D
+from autocti.extract.settings import SettingsExtract
 
+from autocti import exc
 
-class Extract2DSerialCalibration:
+
+class Layout2D(aa.Layout2D):
     def __init__(
         self,
         shape_2d: Tuple[int, int],
         region_list: aa.type.Region2DList,
+        original_roe_corner: Tuple[int, int] = (1, 0),
+        parallel_overscan: Optional[aa.type.Region2DLike] = None,
         serial_prescan: Optional[aa.type.Region2DLike] = None,
         serial_overscan: Optional[aa.type.Region2DLike] = None,
     ):
         """
-        Class containing methods for extracting a serial calibration dataset from a 2D CTI calibration dataset.
-
-        The serial calibration region is the region of a dataset that is necessary for fitting a serial-only CTI
-        model. For example, for charge injection imaging, serial EPERs form only in rows of the CCD where charge
-        is injected and the regions in between have no signal. The serial calibration dataset therefore extracts only
-        these rows.
-
-        A subset of the serial calibration data may also be extracted (e.g. only the first row of every charge region)
-        for fast initial CTI modeling.
+        A charge injection layout, which defines the regions charge injections appear on a charge injection image.
 
-        This uses the `region_list`, which contains the regions with charge (e.g. the charge injection regions) in
-        pixel coordinates.
+        It also contains over regions of the image, for example the serial prescan, overscan and paralle overscan.
 
         Parameters
         ----------
         shape_2d
             The two dimensional shape of the charge injection imaging, corresponding to the number of rows (pixels
             in parallel direction) and columns (pixels in serial direction).
         region_list
-            Integer pixel coordinates specifying the corners of each charge region (top-row, bottom-row,
+            Integer pixel coordinates specifying the corners of each charge injection region (top-row, bottom-row,
+            left-column, right-column).
+        original_roe_corner
+            The original read-out electronics corner of the charge injeciton imaging, which is internally rotated to a
+            common orientation in **PyAutoCTI**.
+        parallel_overscan
+            Integer pixel coordinates specifying the corners of the parallel overscan (top-row, bottom-row,
             left-column, right-column).
         serial_prescan
             Integer pixel coordinates specifying the corners of the serial prescan (top-row, bottom-row,
             left-column, right-column).
         serial_overscan
             Integer pixel coordinates specifying the corners of the serial overscan (top-row, bottom-row,
             left-column, right-column).
+        electronics
+            The charge injection electronics parameters of the image (e.g. the IG1 and IG2 voltages).
         """
-        self.shape_2d = shape_2d
-        self.region_list = list(map(aa.Region2D, region_list))
-        self.serial_prescan = serial_prescan
-        self.serial_overscan = serial_overscan
 
-    def array_2d_list_from(self, array: aa.Array2D):
-        """
-        Extract each charge injection region image for the serial calibration arrays when creating the
-        """
+        self.region_list = list(map(aa.Region2D, region_list))
 
-        calibration_region_list = list(
-            map(
-                lambda ci_region: ci_region.parallel_full_region_from(
-                    shape_2d=self.shape_2d
-                ),
-                self.region_list,
-            )
-        )
-        return list(
-            map(lambda region: array.native[region.slice], calibration_region_list)
-        )
+        for region in self.region_list:
+            if region.y1 > shape_2d[0] or region.x1 > shape_2d[1]:
+                raise exc.LayoutException(
+                    f"""
+                    The charge injection layout regions are bigger than the image image_shape
+                    
+                    The shape of the region is: {region}.
+                    The shape of the image is: {shape_2d}.                    
+                    """
+                )
 
-    def mask_2d_from(self, mask: aa.Mask2D, rows: Tuple[int, int]) -> Mask2D:
+        super().__init__(
+            shape_2d=shape_2d,
+            original_roe_corner=original_roe_corner,
+            parallel_overscan=parallel_overscan,
+            serial_prescan=serial_prescan,
+            serial_overscan=serial_overscan,
+        )
+
+    @property
+    def extract(self):
+        from autocti.extract.two_d.master import Extract2DMaster
+
+        return Extract2DMaster(
+            shape_2d=self.shape_2d,
+            region_list=self.region_list,
+            parallel_overscan=self.parallel_overscan,
+            serial_prescan=self.serial_prescan,
+            serial_overscan=self.serial_overscan,
+        )
+
+    def layout_extracted_from(
+        self, extraction_region: aa.type.Region2DLike
+    ) -> "Layout2D":
         """
-        Extract a serial calibration array from a charge injection array, where this arrays is a sub-set of the
-        array which can be used for serial-only calibration. Specifically, this array is all charge injection
-        scans and their serial over-scan trails.
-
-        The diagram below illustrates the arrays that is extracted from a array with column=5:
-
-        ---KEY---
-        ---------
-
-        [] = read-out electronics   [==========] = read-out register
-
-        [xxxxxxxxxx]                [..........] = serial prescan       [ssssssssss] = serial overscan
-        [xxxxxxxxxx] = CCDPhase panel    [pppppppppp] = parallel overscan    [cccccccccc] = charge injection region
-        [xxxxxxxxxx]                [tttttttttt] = parallel / serial charge injection region trail
-
-        P = Parallel Direction      S = Serial Direction
+        The charge injection layout after an extraction is performed on its associated charge injection image, where
+        the extraction is defined by a region of pixel coordinates:
 
-               [ppppppppppppppppppppp]
-               [pppppppppppppppppppp ]
-          [...][xxxxxxxxxxxxxxxxxxxxx][sss]
-          [...][ccccccccccccccccccccc][tst]
-        | [...][ccccccccccccccccccccc][sts]    |
-        | [...][xxxxxxxxxxxxxxxxxxxxx][sss]    | Direction
-        P [...][xxxxxxxxxxxxxxxxxxxxx][sss]    | of
-        | [...][ccccccccccccccccccccc][tst]    | clocking
-          [...][ccccccccccccccccccccc][sts]    |
+        (top-row, bottom-row, left-column, right-column) = (y0, y1, x0, x1)
 
-        []     [=====================]
-               <--------Ser---------
+        For example, if a charge injection region occupies the pixels (0, 10, 0, 5) on a 100 x 100 charge injection
+        image, and the first 5 columns of this charge injection image are extracted to create a 100 x 5 image, the
+        new charge injection region will be (0, 20, 0, 5).
 
-        The extracted array keeps just the trails following all charge injection scans and replaces all other
-        values with 0s:
-
-        |                                      |
-        |      [cccccccccccccccc][tst]         | Direction
-        P      [cccccccccccccccc][tst]         | of
-        |      [cccccccccccccccc][tst]         | clocking
-               [cccccccccccccccc][tst]         |
-
-        []     [=====================]
-               <--------Ser---------
+        Parameters
+        ----------
+        extraction_region
+            The (y0, y1, x0, x1) pixel coordinates defining the region which the layout is extracted from.
         """
 
-        calibration_region_list = list(
-            map(
-                lambda ci_region: ci_region.parallel_full_region_from(
-                    shape_2d=self.shape_2d
-                ),
-                self.region_list,
+        layout = super().layout_extracted_from(extraction_region=extraction_region)
+
+        region_list = [
+            aa.util.layout.region_after_extraction(
+                original_region=region, extraction_region=extraction_region
             )
-        )
-        calibration_masks = list(
-            map(lambda region: mask[region.slice], calibration_region_list)
-        )
+            for region in self.region_list
+        ]
 
-        calibration_masks = list(
-            map(lambda mask: mask[rows[0] : rows[1], :], calibration_masks)
-        )
-        return Mask2D(
-            mask=np.concatenate(calibration_masks, axis=0),
-            pixel_scales=mask.pixel_scales,
+        return self.__class__(
+            original_roe_corner=self.original_roe_corner,
+            shape_2d=self.shape_2d,
+            region_list=region_list,
+            parallel_overscan=layout.parallel_overscan,
+            serial_prescan=layout.serial_prescan,
+            serial_overscan=layout.serial_overscan,
         )
 
-    def array_2d_from(self, array: aa.Array2D, rows: Tuple[int, int]) -> aa.Array2D:
+    @property
+    def parallel_rows_between_regions(self) -> List[int]:
         """
-        Extract a serial calibration array from a charge injection array, where this arrays is a sub-set of the
-        array which can be used for serial-only calibration. Specifically, this array is all charge injection
-        scans and their serial over-scan trails.
-
-        The diagram below illustrates the arrays that is extracted from a array with column=5:
-
-        [] = read-out electronics
-        [==========] = read-out register
-        [..........] = serial prescan
-        [pppppppppp] = parallel overscan
-        [ssssssssss] = serial overscan
-        [f#ff#f#f#f] = signal region (FPR) (0 / 1 indicate the region index)
-        [tttttttttt] = parallel / serial charge injection region trail
-
-               [ppppppppppppppppppppp]
-               [pppppppppppppppppppp ]
-          [...][xxxxxxxxxxxxxxxxxxxxx][sss]
-          [...][ccccccccccccccccccccc][tst]
-        | [...][ccccccccccccccccccccc][sts]    |
-        | [...][xxxxxxxxxxxxxxxxxxxxx][sss]    | Direction
-        P [...][xxxxxxxxxxxxxxxxxxxxx][sss]    | of
-        | [...][ccccccccccccccccccccc][tst]    | clocking
-          [...][ccccccccccccccccccccc][sts]    |
-
-        []     [=====================]
-               <--------Ser---------
-
-        The extracted array keeps just the trails following all charge injection scans and replaces all other
-        values with 0s:
-
-        |                                      |
-        |      [cccccccccccccccc][tst]         | Direction
-        P      [cccccccccccccccc][tst]         | of
-        |      [cccccccccccccccc][tst]         | clocking
-               [cccccccccccccccc][tst]         |
-
-        []     [=====================]
-               <--------Ser---------
-        """
-        calibration_images = self.array_2d_list_from(array=array)
-        calibration_images = list(
-            map(lambda image: image[rows[0] : rows[1], :], calibration_images)
-        )
-
-        new_array = np.concatenate(calibration_images, axis=0)
-
-        mask_2d = self.mask_2d_from(mask=array.mask, rows=rows)
-
-        return aa.Array2D(
-            values=new_array,
-            mask=mask_2d,
-            header=array.header,
-        )
-
-    def extracted_layout_from(self, layout, new_shape_2d, rows):
-        serial_prescan = (
-            (0, new_shape_2d[0], self.serial_prescan[2], self.serial_prescan[3])
-            if self.serial_prescan is not None
-            else None
-        )
-        serial_overscan = (
-            (0, new_shape_2d[0], self.serial_overscan[2], self.serial_overscan[3])
-            if self.serial_overscan is not None
-            else None
-        )
-
-        x0 = self.region_list[0][2]
-        x1 = self.region_list[0][3]
-        offset = 0
+        Returns a list where each entry is the number of pixels a charge injection region and its neighboring
+        charge injection region.
+        """
+        return self.extract.parallel_fpr.parallel_rows_between_regions
 
-        new_pattern_region_list_ci = []
+    @property
+    def parallel_rows_within_regions(self) -> List[int]:
+        """
+        Returns a list where each entry is the number of pixels a charge injection region and its neighboring
+        charge injection region.
+        """
+        return [region.y1 - region.y0 for region in self.region_list]
 
-        for region in self.region_list:
-            labelsize = rows[1] - rows[0]
-            new_pattern_region_list_ci.append(
-                aa.Region2D(region=(offset, offset + labelsize, x0, x1))
-            )
-            offset += labelsize
+    @property
+    def parallel_rows_to_array_edge(self) -> int:
+        """
+        The number of pixels from the edge of the parallel EPERs to the edge of the array.
 
-        new_layout = deepcopy(layout)
-        new_layout.region_list = new_pattern_region_list_ci
-        new_layout.serial_prescan = serial_prescan
-        new_layout.serial_overscan = serial_overscan
+        This is the number of pixels from the last charge injection FPR edge to the read out register and electronics
+        and will include the parallel overscan if the CCD has one.
+        """
+        return self.extract.parallel_fpr.parallel_rows_to_array_edge
 
-        return new_layout
+    @property
+    def smallest_parallel_rows_between_ci_regions(self) -> int:
+        """
+        The smallest number of pixels between any two charge injection regions, or the distance of the last
+        charge injection region to the edge of the charge injeciton image (e.g. in the direction away from the
+        readout register and electronics).
+        """
+        parallel_rows_between_regions = self.parallel_rows_between_regions
+        parallel_rows_between_regions.append(self.parallel_rows_to_array_edge)
+        return np.min(parallel_rows_between_regions)
 
-    def imaging_ci_from(self, dataset: ImagingCI, rows) -> ImagingCI:
+    @property
+    def smallest_parallel_rows_within_ci_regions(self) -> int:
         """
-        Returnss a function to extract a serial section for given rows
+        The smallest number of pixels within any of the charge injection regions.
+
+        This can be used to extract the FPR of each charge injection region using a
+        number of pixels which does not exceed the size of any.
         """
+        return np.min(self.parallel_rows_within_regions)
 
-        from autocti.charge_injection.imaging.imaging import ImagingCI
+    def with_extracted_regions(
+        self, extraction_region: aa.type.Region2DLike
+    ) -> "Layout2D":
+        layout = deepcopy(self)
 
-        cosmic_ray_map = (
-            dataset.layout.extract.serial_calibration.array_2d_from(
-                array=dataset.cosmic_ray_map, rows=rows
+        extracted_region_list = list(
+            map(
+                lambda region: aa.util.layout.region_after_extraction(
+                    original_region=region, extraction_region=extraction_region
+                ),
+                self.region_list,
             )
-            if dataset.cosmic_ray_map is not None
-            else None
         )
+        extracted_region_list = list(filter(None, extracted_region_list))
+        if not extracted_region_list:
+            extracted_region_list = None
+
+        layout.region_list = extracted_region_list
+        return layout
+
+    def extract_region_from(self, array: aa.Array2D, region: str) -> aa.Array1D:
+        if region == "parallel_fpr":
+            return self.extract.parallel_fpr.binned_array_1d_from(
+                array=array,
+                settings=SettingsExtract(
+                    pixels=(0, self.extract.parallel_fpr.total_rows_min)
+                ),
+            )
+        elif region == "parallel_eper":
+            return self.extract.parallel_eper.binned_array_1d_from(
+                array=array,
+                settings=SettingsExtract(
+                    pixels=(0, self.smallest_parallel_rows_between_ci_regions)
+                ),
+            )
+        elif region == "serial_fpr" or region == "fpr_non_uniformity":
+            return self.extract.serial_fpr.binned_array_1d_from(
+                array=array,
+                settings=SettingsExtract(
+                    pixels=(0, self.extract.serial_fpr.total_columns_min)
+                ),
+            )
+        elif region == "serial_eper":
+            return self.extract.serial_eper.binned_array_1d_from(
+                array=array,
+                settings=SettingsExtract(pixels=(0, self.serial_eper_pixels)),
+            )
+        else:
+            raise exc.PlottingException(
+                "The line region specified for the plotting of a line was invalid"
+            )
 
-        if dataset.noise_scaling_map_dict is not None:
-            noise_scaling_map_dict = {
-                key: dataset.layout.extract.serial_calibration.array_2d_from(
-                    array=noise_scaling_map, rows=rows
+    def extract_region_noise_map_from(
+        self, array: aa.Array2D, region: str
+    ) -> aa.Array1D:
+        if region == "parallel_fpr":
+            binned_noise_map_1d = self.extract.parallel_fpr.binned_array_1d_from(
+                array=array,
+                settings=SettingsExtract(
+                    pixels=(0, self.extract.parallel_fpr.total_rows_min)
+                ),
+            )
+            binned_noise_map_1d_total_pixels = (
+                self.extract.parallel_fpr.binned_array_1d_total_pixels_from(
+                    array=array,
+                    settings=SettingsExtract(
+                        pixels=(0, self.extract.parallel_fpr.total_rows_min)
+                    ),
                 )
-                for key, noise_scaling_map in dataset.noise_scaling_map_dict.items()
-            }
-
+            )
+        elif region == "parallel_eper":
+            binned_noise_map_1d = self.extract.parallel_eper.binned_array_1d_from(
+                array=array,
+                settings=SettingsExtract(
+                    pixels=(0, self.smallest_parallel_rows_between_ci_regions)
+                ),
+            )
+            binned_noise_map_1d_total_pixels = (
+                self.extract.parallel_eper.binned_array_1d_total_pixels_from(
+                    array=array,
+                    settings=SettingsExtract(
+                        pixels=(0, self.smallest_parallel_rows_between_ci_regions),
+                    ),
+                )
+            )
+        elif region == "serial_fpr" or region == "fpr_non_uniformity":
+            binned_noise_map_1d = self.extract.serial_fpr.binned_array_1d_from(
+                array=array,
+                settings=SettingsExtract(
+                    pixels=(0, self.extract.serial_fpr.total_columns_min)
+                ),
+            )
+            binned_noise_map_1d_total_pixels = (
+                self.extract.serial_fpr.binned_array_1d_total_pixels_from(
+                    array=array,
+                    settings=SettingsExtract(
+                        pixels=(0, self.extract.serial_fpr.total_columns_min)
+                    ),
+                )
+            )
+        elif region == "serial_eper":
+            binned_noise_map_1d = self.extract.serial_eper.binned_array_1d_from(
+                array=array,
+                settings=SettingsExtract(pixels=(0, self.serial_eper_pixels)),
+            )
+            binned_noise_map_1d_total_pixels = (
+                self.extract.serial_eper.binned_array_1d_total_pixels_from(
+                    array=array,
+                    settings=SettingsExtract(pixels=(0, self.serial_eper_pixels)),
+                )
+            )
         else:
-            noise_scaling_map_dict = None
-
-        image = dataset.layout.extract.serial_calibration.array_2d_from(
-            array=dataset.data, rows=rows
-        )
-
-        mask = self.mask_2d_from(mask=dataset.mask, rows=rows)
+            raise exc.PlottingException(
+                "The line region specified for the plotting of a line was invalid"
+            )
 
-        dataset = ImagingCI(
-            data=image,
-            noise_map=dataset.layout.extract.serial_calibration.array_2d_from(
-                array=dataset.noise_map, rows=rows
-            ),
-            pre_cti_data=dataset.layout.extract.serial_calibration.array_2d_from(
-                array=dataset.pre_cti_data, rows=rows
-            ),
-            layout=dataset.layout.extract.serial_calibration.extracted_layout_from(
-                layout=dataset.layout, new_shape_2d=image.shape, rows=rows
-            ),
-            cosmic_ray_map=cosmic_ray_map,
-            noise_scaling_map_dict=noise_scaling_map_dict,
-            fpr_value=dataset.fpr_value,
-            settings_dict=dataset.settings_dict,
-        )
+        binned_noise_map_1d /= np.sqrt(binned_noise_map_1d_total_pixels)
 
-        return dataset.apply_mask(mask=mask)
+        return binned_noise_map_1d
```

### Comparing `autocti-2024.1.27.4/autocti/extract/two_d/serial/eper.py` & `autocti-2024.5.16.0/autocti/extract/two_d/serial/eper.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/extract/two_d/serial/fpr.py` & `autocti-2024.5.16.0/autocti/extract/two_d/serial/fpr.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/extract/two_d/serial/overscan.py` & `autocti-2024.5.16.0/autocti/extract/two_d/serial/overscan.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/extract/two_d/serial/overscan_no_eper.py` & `autocti-2024.5.16.0/autocti/extract/two_d/serial/overscan_no_eper.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/extract/two_d/serial/prescan.py` & `autocti-2024.5.16.0/autocti/extract/two_d/serial/prescan.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/fixtures.py` & `autocti-2024.5.16.0/autocti/fixtures.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from autofit.non_linear.mock.mock_samples import MockSamples
+from autofit.non_linear.mock.mock_samples_summary import MockSamplesSummary
 
 from autoarray.fixtures import *
 
 import autofit as af
 import autocti as ac
 
 import numpy as np
@@ -204,31 +204,31 @@
         hyper_noise_scalar_dict=make_hyper_noise_scalar_dict(),
     )
 
 
 # ### PHASES ###
 
 
-def make_samples_with_result():
+def make_samples_summary_with_result():
     model = af.Collection(
         cti=af.Model(
             ac.CTI2D,
             parallel_trap_list=[ac.TrapInstantCapture],
             parallel_ccd=make_ccd(),
             serial_trap_list=[ac.TrapInstantCapture],
             serial_ccd=make_ccd(),
         ),
     )
 
     instance = model.instance_from_prior_medians()
 
-    return MockSamples(
-        model=model,
+    return MockSamplesSummary(
         max_log_likelihood_instance=instance,
-        gaussian_tuples=[(1.0, 2.0)] * model.prior_count,
+        model=model,
+        prior_means=[1.0] * model.prior_count,
     )
 
 
 def make_analysis_imaging_ci_7x7():
     return ac.AnalysisImagingCI(
         dataset=make_imaging_ci_7x7(), clocker=make_parallel_clocker_2d()
     )
```

### Comparing `autocti-2024.1.27.4/autocti/instruments/acs/acs_util.py` & `autocti-2024.5.16.0/autocti/instruments/acs/acs_util.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/instruments/acs/array_2d.py` & `autocti-2024.5.16.0/autocti/instruments/acs/array_2d.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/instruments/acs/header.py` & `autocti-2024.5.16.0/autocti/instruments/acs/header.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/instruments/acs/image.py` & `autocti-2024.5.16.0/autocti/instruments/acs/image.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/instruments/acs/layout.py` & `autocti-2024.5.16.0/autocti/instruments/acs/layout.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/instruments/euclid/array_2d.py` & `autocti-2024.5.16.0/autocti/instruments/euclid/array_2d.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/instruments/euclid/euclid_util.py` & `autocti-2024.5.16.0/autocti/instruments/euclid/euclid_util.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/instruments/euclid/header.py` & `autocti-2024.5.16.0/autocti/instruments/euclid/header.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/instruments/euclid/layout.py` & `autocti-2024.5.16.0/autocti/instruments/euclid/layout.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/layout/one_d.py` & `autocti-2024.5.16.0/autocti/layout/one_d.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/mask/mask_1d.py` & `autocti-2024.5.16.0/autocti/mask/mask_1d.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/mask/mask_2d.py` & `autocti-2024.5.16.0/autocti/mask/mask_2d.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/model/analysis.py` & `autocti-2024.5.16.0/autocti/model/analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 from autocti.charge_injection.model.result import ResultImagingCI
 from autocti.clocker.one_d import Clocker1D
 from autocti.clocker.two_d import Clocker2D
 from autocti.dataset_1d.dataset_1d.dataset_1d import Dataset1D
 from autocti.model.settings import SettingsCTI1D
 from autocti.model.settings import SettingsCTI2D
 
-from autocti import exc
-
 
 class AnalysisCTI(af.Analysis):
     def __init__(
         self,
         dataset: Union[Dataset1D, ImagingCI],
         clocker: Union[Clocker1D, Clocker2D],
         settings_cti: Union[SettingsCTI1D, SettingsCTI2D],
@@ -55,15 +53,15 @@
         self.clocker = clocker
         self.settings_cti = settings_cti
         self.dataset_full = dataset_full
 
     def region_list_from(self) -> List:
         raise NotImplementedError
 
-    def save_results(self, paths: af.DirectoryPaths, result: ResultImagingCI):
+    def save_results_combined(self, paths: af.DirectoryPaths, result: ResultImagingCI):
         """
         At the end of a model-fit, this routine saves attributes of the `Analysis` object to the `files`
         folder such that they can be loaded after the analysis using PyAutoFit's database and aggregator tools.
 
         For this analysis it outputs the following:
 
         - The Israel et al requirement on the spurious ellipticity based on the errors of the fit.
@@ -73,48 +71,42 @@
         paths
             The PyAutoFit paths object which manages all paths, e.g. where the non-linear search outputs are stored,
             visualization and the pickled objects used by the aggregator output by this function.
         result
             The result of a model fit, including the non-linear search and samples.
         """
 
+        if result.samples is None:
+            return
+
         weight_list = []
         delta_ellipticity_list = []
 
-        try:
-            for sample in result.samples.sample_list:
-                try:
-                    instance = sample.instance_for_model(model=result.samples.model)
-                except exc.FitException:
-                    continue
-
-                weight_list.append(sample.weight)
-                delta_ellipticity_list.append(instance.cti.delta_ellipticity)
-
-            (
-                median_delta_ellipticity,
-                upper_delta_ellipticity,
-                lower_delta_ellipticity,
-            ) = af.marginalize(
-                parameter_list=delta_ellipticity_list,
-                sigma=2.0,
-                weight_list=weight_list,
-            )
-
-            delta_ellipticity = (
-                upper_delta_ellipticity - lower_delta_ellipticity
-            ) / 2.0
-
-            output_to_json(
-                obj=delta_ellipticity,
-                file_path=paths._files_path / "delta_ellipticity.json",
-            )
+        for sample in result.samples.sample_list:
+            instance = sample.instance_for_model(model=result.samples.model)
+
+            weight_list.append(sample.weight)
+            delta_ellipticity_list.append(instance.cti.delta_ellipticity)
 
-        except AttributeError:
-            pass
+        (
+            median_delta_ellipticity,
+            upper_delta_ellipticity,
+            lower_delta_ellipticity,
+        ) = af.marginalize(
+            parameter_list=delta_ellipticity_list,
+            sigma=2.0,
+            weight_list=weight_list,
+        )
+
+        delta_ellipticity = (upper_delta_ellipticity - lower_delta_ellipticity) / 2.0
+
+        output_to_json(
+            obj=delta_ellipticity,
+            file_path=paths._files_path / "delta_ellipticity.json",
+        )
 
     def in_ascending_fpr_order_from(self, quantity_list, fpr_value_list):
         if not conf.instance["visualize"]["general"]["general"][
             "subplot_ascending_fpr"
         ]:
             return quantity_list
```

### Comparing `autocti-2024.1.27.4/autocti/model/model_util.py` & `autocti-2024.5.16.0/autocti/model/model_util.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/model/settings.py` & `autocti-2024.5.16.0/autocti/model/settings.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/model/visualizer.py` & `autocti-2024.5.16.0/autocti/model/plotter_interface.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,27 +11,23 @@
     return conf.instance["visualize"]["plots"][section][name]
 
 
 def plot_setting(section, name):
     return setting(section, name)
 
 
-class Visualizer:
-    def __init__(self, visualize_path):
-        self.visualize_path = visualize_path
+class PlotterInterface:
+    def __init__(self, image_path):
+        self.image_path = image_path
 
         self.include_1d = Include1D()
         self.include_2d = Include2D()
 
     def mat_plot_1d_from(self, subfolders, format="png"):
         return MatPlot1D(
-            output=Output(
-                path=path.join(self.visualize_path, subfolders), format=format
-            )
+            output=Output(path=path.join(self.image_path, subfolders), format=format)
         )
 
     def mat_plot_2d_from(self, subfolders, format="png"):
         return MatPlot2D(
-            output=Output(
-                path=path.join(self.visualize_path, subfolders), format=format
-            )
+            output=Output(path=path.join(self.image_path, subfolders), format=format)
         )
```

### Comparing `autocti-2024.1.27.4/autocti/plot/__init__.py` & `autocti-2024.5.16.0/autocti/plot/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,10 @@
-from autofit.plot.samples_plotters import SamplesPlotter
-from autofit.non_linear.search.nest.dynesty.plotter import DynestyPlotter
-from autofit.non_linear.search.nest.nautilus.plotter import NautilusPlotter
-from autofit.non_linear.search.nest.ultranest.plotter import UltraNestPlotter
-from autofit.non_linear.search.mcmc.emcee.plotter import EmceePlotter
-from autofit.non_linear.search.mcmc.zeus.plotter import ZeusPlotter
-from autofit.non_linear.search.optimize.pyswarms.plotter import PySwarmsPlotter
+from autofit.non_linear.plot.nest_plotters import NestPlotter
+from autofit.non_linear.plot.mcmc_plotters import MCMCPlotter
+from autofit.non_linear.plot.optimize_plotters import OptimizePlotter
 
 from autoarray.plot.wrap.base import Axis
 from autoarray.plot.wrap.base import Units
 from autoarray.plot.wrap.base import Figure
 from autoarray.plot.wrap.base import Cmap
 from autoarray.plot.wrap.base import Colorbar
 from autoarray.plot.wrap.base import ColorbarTickParams
```

### Comparing `autocti-2024.1.27.4/autocti/plot/abstract_plotters.py` & `autocti-2024.5.16.0/autocti/plot/abstract_plotters.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/plot/get_visuals/one_d.py` & `autocti-2024.5.16.0/autocti/plot/get_visuals/one_d.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/plot/get_visuals/two_d.py` & `autocti-2024.5.16.0/autocti/plot/get_visuals/two_d.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/preloads.py` & `autocti-2024.5.16.0/autocti/preloads.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/autocti/util/__init__.py` & `autocti-2024.5.16.0/autocti/util/__init__.py`

 * *Files identical despite different names*

### Comparing `autocti-2024.1.27.4/setup.py` & `autocti-2024.5.16.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 this_dir = abspath(dirname(__file__))
 with open(join(this_dir, "README.rst"), encoding="utf-8") as file:
     long_description = file.read()
 
 with open(join(this_dir, "requirements.txt")) as f:
     requirements = f.read().split("\n")
 
-version = environ.get("VERSION", "1.0.dev0")
+version = environ.get("VERSION", "2024.5.16.0")
 requirements.extend(
     [f"autoconf=={version}", f"autofit=={version}", f"autoarray=={version}"]
 )
 
 setup(
     name="autocti",
     version=version,
```

