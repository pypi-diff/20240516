# Comparing `tmp/autogalaxy-2024.1.27.4.tar.gz` & `tmp/autogalaxy-2024.5.16.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogalaxy-2024.1.27.4.tar", last modified: Sat Jan 27 19:56:34 2024, max compression
+gzip compressed data, was "autogalaxy-2024.5.16.0.tar", last modified: Thu May 16 09:58:26 2024, max compression
```

## Comparing `autogalaxy-2024.1.27.4.tar` & `autogalaxy-2024.5.16.0.tar`

### file list

```diff
@@ -1,367 +1,519 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.280881 autogalaxy-2024.1.27.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/CITATIONS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8686 2024-01-27 19:56:34.280881 autogalaxy-2024.1.27.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7643 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.236881 autogalaxy-2024.1.27.4/autogalaxy/
--rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-01-27 19:56:27.000000 autogalaxy-2024.1.27.4/autogalaxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7792 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/abstract_fit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.236881 autogalaxy-2024.1.27.4/autogalaxy/aggregator/
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/aggregator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7129 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/aggregator/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/aggregator/agg_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     7787 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/aggregator/fit_imaging.py
--rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/aggregator/fit_interferometer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/aggregator/imaging.py
--rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/aggregator/interferometer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/aggregator/plane.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.236881 autogalaxy-2024.1.27.4/autogalaxy/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/analysis/adapt_images.py
--rw-r--r--   0 runner    (1001) docker     (127)    19495 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/analysis/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    10020 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/analysis/chaining_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     7567 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/analysis/clump_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/analysis/maker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.240881 autogalaxy-2024.1.27.4/autogalaxy/analysis/mock/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/analysis/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/analysis/mock/mock_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     9822 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/analysis/preloads.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/analysis/result.py
--rw-r--r--   0 runner    (1001) docker     (127)    20409 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/analysis/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.240881 autogalaxy-2024.1.27.4/autogalaxy/config/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/general.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/grids.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/notation.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.240881 autogalaxy-2024.1.27.4/autogalaxy/config/priors/
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/basis.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/cosmology.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.240881 autogalaxy-2024.1.27.4/autogalaxy/config/priors/galaxy/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/galaxy/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/galaxy/redshift.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.240881 autogalaxy-2024.1.27.4/autogalaxy/config/priors/image_mesh/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/image_mesh/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/image_mesh/hilbert.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/image_mesh/hilbert_balanced.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/image_mesh/kmeans.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/image_mesh/overlay.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.240881 autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.240881 autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/linear/
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/linear/chameleon.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/linear/dev_vaucouleurs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/linear/eff.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/linear/exponential.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/linear/exponential_core.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/linear/gaussian.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/linear/moffat.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/linear/sersic.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/linear/sersic_core.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.244881 autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/linear_operated/
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/linear_operated/gaussian.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/linear_operated/moffat.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.244881 autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/operated/
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/operated/gaussian.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/operated/moffat.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/operated/sersic.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.244881 autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/shapelets/
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/shapelets/cartesian.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/shapelets/exponential.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/shapelets/polar.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.244881 autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/standard/
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/standard/chameleon.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/standard/dev_vaucouleurs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/standard/eff.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/standard/exponential.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/standard/exponential_core.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/standard/gaussian.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/standard/moffat.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/standard/sersic.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/standard/sersic_core.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.244881 autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.244881 autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/dark/
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/dark/gnfw.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/dark/gnfw_mcr.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/dark/nfw.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/dark/nfw_mcr.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/dark/nfw_mcr_scatter.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/dark/nfw_truncated.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/dark/nfw_truncated_mcr.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/dark/nfw_virial_mass_conc.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.248881 autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/point/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/point/point.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/point/smbh.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/point/smbh_binary.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.248881 autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/sheets/
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/sheets/external_shear.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/sheets/mass_sheet.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.248881 autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/stellar/
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/stellar/chameleon.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/stellar/dev_vaucouleurs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/stellar/exponential.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/stellar/gaussian.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/stellar/sersic.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/stellar/sersic_core.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/stellar/sersic_radial_gradient.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.248881 autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/total/
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/total/isothermal.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/total/isothermal_core.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/total/power_law.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/total/power_law_broken.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/total/power_law_core.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/total/power_law_multipole.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.248881 autogalaxy-2024.1.27.4/autogalaxy/config/priors/mesh/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/mesh/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/mesh/delaunay.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/mesh/rectangular.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/mesh/voronoi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/mesh/voronoi_nn.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/point_sources.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.252881 autogalaxy-2024.1.27.4/autogalaxy/config/priors/regularization/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/regularization/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/regularization/adaptive_brightness.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/regularization/adaptive_brightness_split_zeroth.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/regularization/constant.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/regularization/constant_split.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/regularization/constant_zeroth.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/regularization/exponential_kernel.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/regularization/gaussian_kernel.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/regularization/matern_kernel.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/priors/regularization/zeroth.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.252881 autogalaxy-2024.1.27.4/autogalaxy/config/visualize/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/visualize/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/visualize/general.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/visualize/include.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/visualize/mat_wrap_1d.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/visualize/mat_wrap_2d.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/config/visualize/plots.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.252881 autogalaxy-2024.1.27.4/autogalaxy/cosmology/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/cosmology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14342 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/cosmology/lensing.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/cosmology/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/cosmology/wrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/exc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.252881 autogalaxy-2024.1.27.4/autogalaxy/galaxy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/galaxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20562 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/galaxy/galaxy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.252881 autogalaxy-2024.1.27.4/autogalaxy/galaxy/mock/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/galaxy/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/galaxy/mock/mock_galaxy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.252881 autogalaxy-2024.1.27.4/autogalaxy/galaxy/plot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/galaxy/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/galaxy/plot/adapt_plotters.py
--rw-r--r--   0 runner    (1001) docker     (127)    40483 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/galaxy/plot/galaxy_plotters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/galaxy/redshift.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/galaxy/stellar_dark_decomp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.252881 autogalaxy-2024.1.27.4/autogalaxy/gui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/gui/clicker.py
--rw-r--r--   0 runner    (1001) docker     (127)     6977 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/gui/scribbler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.256881 autogalaxy-2024.1.27.4/autogalaxy/imaging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/imaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12764 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/imaging/fit_imaging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.256881 autogalaxy-2024.1.27.4/autogalaxy/imaging/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/imaging/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16407 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/imaging/model/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/imaging/model/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/imaging/model/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.256881 autogalaxy-2024.1.27.4/autogalaxy/imaging/plot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/imaging/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9632 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/imaging/plot/fit_imaging_plotters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/imaging/simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.256881 autogalaxy-2024.1.27.4/autogalaxy/interferometer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/interferometer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10621 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/interferometer/fit_interferometer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.256881 autogalaxy-2024.1.27.4/autogalaxy/interferometer/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/interferometer/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17404 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/interferometer/model/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/interferometer/model/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/interferometer/model/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.256881 autogalaxy-2024.1.27.4/autogalaxy/interferometer/plot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/interferometer/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/interferometer/plot/fit_interferometer_plotters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/interferometer/simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.256881 autogalaxy-2024.1.27.4/autogalaxy/operate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/operate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37157 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/operate/deflections.py
--rw-r--r--   0 runner    (1001) docker     (127)    20242 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/operate/image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.256881 autogalaxy-2024.1.27.4/autogalaxy/plane/
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/plane/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15678 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/plane/plane.py
--rw-r--r--   0 runner    (1001) docker     (127)     8436 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/plane/plane_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.260881 autogalaxy-2024.1.27.4/autogalaxy/plane/plot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/plane/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14039 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/plane/plot/plane_plotters.py
--rw-r--r--   0 runner    (1001) docker     (127)    11640 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/plane/to_inversion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.260881 autogalaxy-2024.1.27.4/autogalaxy/plot/
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/plot/abstract_plotters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.260881 autogalaxy-2024.1.27.4/autogalaxy/plot/get_visuals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/plot/get_visuals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9924 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/plot/get_visuals/one_d.py
--rw-r--r--   0 runner    (1001) docker     (127)    13590 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/plot/get_visuals/two_d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.260881 autogalaxy-2024.1.27.4/autogalaxy/plot/include/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/plot/include/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/plot/include/one_d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/plot/include/two_d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/plot/mass_plotter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.260881 autogalaxy-2024.1.27.4/autogalaxy/plot/mat_plot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/plot/mat_plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6249 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/plot/mat_plot/one_d.py
--rw-r--r--   0 runner    (1001) docker     (127)    10323 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/plot/mat_plot/two_d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.260881 autogalaxy-2024.1.27.4/autogalaxy/plot/visuals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/plot/visuals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/plot/visuals/one_d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/plot/visuals/two_d.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/plot/wrap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.260881 autogalaxy-2024.1.27.4/autogalaxy/profiles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14374 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/geometry_profiles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.264881 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5442 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/basis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.264881 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/linear/
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/linear/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6948 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/linear/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/linear/chameleon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/linear/dev_vaucouleurs.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/linear/eff.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/linear/exponential.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/linear/exponential_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/linear/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/linear/moffat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/linear/sersic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/linear/sersic_core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.264881 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/linear_operated/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/linear_operated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/linear_operated/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/linear_operated/moffat.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/linear_operated/sersic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.264881 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/mock/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/mock/mock_light_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.264881 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/operated/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/operated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/operated/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/operated/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/operated/moffat.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/operated/sersic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.268881 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/shapelets/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/shapelets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/shapelets/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/shapelets/cartesian.py
--rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/shapelets/exponential.py
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/shapelets/polar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.268881 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/snr/
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/snr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/snr/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/snr/chameleon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/snr/dev_vaucouleurs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/snr/eff.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/snr/exponential.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/snr/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/snr/sersic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/snr/sersic_core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.268881 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/standard/
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/standard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5851 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/standard/chameleon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/standard/dev_vaucouleurs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/standard/eff.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/standard/exponential.py
--rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/standard/exponential_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/standard/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/standard/moffat.py
--rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/standard/sersic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light/standard/sersic_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    25207 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/light_and_mass_profiles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.268881 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.272881 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/abstract/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/abstract/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     7069 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/abstract/cse.py
--rw-r--r--   0 runner    (1001) docker     (127)     8675 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/abstract/mge.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.272881 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/dark/
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/dark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12551 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/dark/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    13480 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/dark/gnfw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/dark/gnfw_mcr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/dark/mcr_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    11544 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/dark/nfw.py
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/dark/nfw_mcr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/dark/nfw_mcr_scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/dark/nfw_truncated.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/dark/nfw_truncated_mcr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/dark/nfw_truncated_mcr_scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/dark/nfw_virial_mass_conc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.272881 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/mock/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/mock/mock_mass_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.272881 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/point/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/point/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/point/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/point/smbh.py
--rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/point/smbh_binary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.276881 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/sheets/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/sheets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/sheets/external_shear.py
--rw-r--r--   0 runner    (1001) docker     (127)     4977 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/sheets/input_deflections.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/sheets/mass_sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.276881 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/stellar/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/stellar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/stellar/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     8299 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/stellar/chameleon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/stellar/dev_vaucouleurs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/stellar/exponential.py
--rw-r--r--   0 runner    (1001) docker     (127)     7446 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/stellar/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)    16555 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/stellar/sersic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7038 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/stellar/sersic_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9653 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/stellar/sersic_radial_gradient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.276881 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/total/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/total/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6743 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/total/isothermal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/total/isothermal_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5545 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/total/power_law.py
--rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/total/power_law_broken.py
--rw-r--r--   0 runner    (1001) docker     (127)     8274 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/total/power_law_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9789 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/total/power_law_multipole.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.276881 autogalaxy-2024.1.27.4/autogalaxy/profiles/plot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12951 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/plot/light_profile_plotters.py
--rw-r--r--   0 runner    (1001) docker     (127)    14759 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/plot/mass_profile_plotters.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/point_sources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/profiles/scaling_relations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.280881 autogalaxy-2024.1.27.4/autogalaxy/quantity/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/quantity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11252 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/quantity/dataset_quantity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/quantity/fit_quantity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.280881 autogalaxy-2024.1.27.4/autogalaxy/quantity/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/quantity/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10071 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/quantity/model/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/quantity/model/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/quantity/model/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.280881 autogalaxy-2024.1.27.4/autogalaxy/quantity/plot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/quantity/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8126 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/quantity/plot/fit_quantity_plotters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.280881 autogalaxy-2024.1.27.4/autogalaxy/util/
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/util/error_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.280881 autogalaxy-2024.1.27.4/autogalaxy/util/mock/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/util/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/util/mock/mock_cosmology.py
--rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-01-27 19:56:26.000000 autogalaxy-2024.1.27.4/autogalaxy/util/shear_field.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:34.280881 autogalaxy-2024.1.27.4/autogalaxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12731 2024-01-27 19:56:34.000000 autogalaxy-2024.1.27.4/autogalaxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-01-27 19:56:27.000000 autogalaxy-2024.1.27.4/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-01-27 19:56:27.000000 autogalaxy-2024.1.27.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-27 19:56:34.280881 autogalaxy-2024.1.27.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-01-27 19:56:27.000000 autogalaxy-2024.1.27.4/setup.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.854380 autogalaxy-2024.5.16.0/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:25.662073 autogalaxy-2024.5.16.0/.github/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:25.742127 autogalaxy-2024.5.16.0/.github/workflows/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      475 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/.github/workflows/draft-pdf.yml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3398 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/.github/workflows/main.yml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1135 2022-12-19 11:17:33.000000 autogalaxy-2024.5.16.0/CITATIONS.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18987 2022-12-20 20:59:49.000000 autogalaxy-2024.5.16.0/CODE_OF_CONDUCT.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2494 2022-12-20 20:59:49.000000 autogalaxy-2024.5.16.0/CONTRIBUTING.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1095 2020-11-16 19:58:12.000000 autogalaxy-2024.5.16.0/LICENSE
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      388 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/MANIFEST.in
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8480 2024-05-16 09:58:26.853369 autogalaxy-2024.5.16.0/PKG-INFO
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7646 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/README.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:25.753665 autogalaxy-2024.5.16.0/autogalaxy/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5656 2024-05-16 09:55:27.000000 autogalaxy-2024.5.16.0/autogalaxy/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8874 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/abstract_fit.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:25.771457 autogalaxy-2024.5.16.0/autogalaxy/aggregator/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      314 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/aggregator/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6101 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/aggregator/agg_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2191 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/aggregator/dataset_model.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7623 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/aggregator/fit_imaging.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8104 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/aggregator/fit_interferometer.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4806 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/aggregator/galaxies.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4783 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/aggregator/imaging.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5702 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/aggregator/interferometer.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:25.785655 autogalaxy-2024.5.16.0/autogalaxy/analysis/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-08-21 09:36:45.000000 autogalaxy-2024.5.16.0/autogalaxy/analysis/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:25.792066 autogalaxy-2024.5.16.0/autogalaxy/analysis/adapt_images/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/analysis/adapt_images/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2204 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/analysis/adapt_images/adapt_image_maker.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8412 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/analysis/adapt_images/adapt_images.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:25.799085 autogalaxy-2024.5.16.0/autogalaxy/analysis/analysis/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/analysis/analysis/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10209 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/analysis/analysis/analysis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9286 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/analysis/analysis/dataset.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10020 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/analysis/chaining_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7567 2024-03-03 18:16:57.000000 autogalaxy-2024.5.16.0/autogalaxy/analysis/clump_model.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4736 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/analysis/maker.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:25.803613 autogalaxy-2024.5.16.0/autogalaxy/analysis/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/autogalaxy/analysis/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      961 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/analysis/mock/mock_result.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    15372 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/autogalaxy/analysis/plotter_interface.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9825 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/analysis/preloads.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5230 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/analysis/result.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:25.816613 autogalaxy-2024.5.16.0/autogalaxy/config/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       11 2020-11-11 16:43:14.000000 autogalaxy-2024.5.16.0/autogalaxy/config/.gitignore
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      630 2023-05-10 17:34:39.000000 autogalaxy-2024.5.16.0/autogalaxy/config/README.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      935 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/config/general.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1786 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/config/grids.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3426 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/config/notation.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:25.829129 autogalaxy-2024.5.16.0/autogalaxy/config/priors/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1607 2022-12-16 19:52:14.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/README.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       10 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/basis.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      620 2023-08-09 13:35:03.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/cosmology.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      182 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/dataset_model.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:25.835650 autogalaxy-2024.5.16.0/autogalaxy/config/priors/galaxy/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      253 2023-06-06 10:32:01.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/galaxy/README.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      204 2022-12-21 16:13:37.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/galaxy/redshift.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:25.849170 autogalaxy-2024.5.16.0/autogalaxy/config/priors/image_mesh/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      394 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/image_mesh/README.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      613 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/image_mesh/hilbert.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      612 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/image_mesh/kmeans.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      400 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/image_mesh/overlay.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:25.852170 autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1009 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/README.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:25.887688 autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/linear/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2105 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/linear/chameleon.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1739 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/linear/dev_vaucouleurs.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2097 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/linear/eff.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1733 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/linear/exponential.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2849 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/linear/exponential_core.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1705 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/linear/gaussian.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2061 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/linear/moffat.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2101 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/linear/sersic.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3217 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/linear/sersic_core.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:25.900691 autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/linear/shapelets/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1815 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/linear/shapelets/cartesian.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1819 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/linear/shapelets/exponential.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1807 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/linear/shapelets/polar.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:25.908689 autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/linear_operated/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1271 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/linear_operated/gaussian.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1251 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/linear_operated/moffat.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:25.920689 autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/operated/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1271 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/operated/gaussian.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1450 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/operated/moffat.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1469 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/operated/sersic.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:25.954689 autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/standard/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2503 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/standard/chameleon.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2137 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/standard/dev_vaucouleurs.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2495 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/standard/eff.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2131 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/standard/exponential.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3241 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/standard/exponential_core.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2103 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/standard/gaussian.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2459 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/standard/moffat.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2499 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/standard/sersic.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3609 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/standard/sersic_core.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:25.958704 autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      639 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/README.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:25.986687 autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/dark/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2457 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/dark/gnfw.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1682 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/dark/gnfw_mcr.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2077 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/dark/nfw.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3593 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/dark/nfw_mcr.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1274 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/dark/nfw_mcr_scatter.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1022 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/dark/nfw_truncated.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3402 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/dark/nfw_truncated_mcr.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1443 2023-10-16 10:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/dark/nfw_virial_mass_conc.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:25.997687 autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/point/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      640 2023-05-15 17:46:30.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/point/point.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1029 2023-05-15 17:46:30.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/point/smbh.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1604 2023-05-17 15:24:31.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/point/smbh_binary.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.003689 autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/sheets/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      389 2023-01-14 17:31:13.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/sheets/external_shear.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      632 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/sheets/mass_sheet.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.026686 autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/stellar/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2921 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/stellar/chameleon.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2545 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/stellar/dev_vaucouleurs.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2539 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/stellar/exponential.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1481 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/stellar/gaussian.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2907 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/stellar/sersic.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4027 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/stellar/sersic_core.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3337 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/stellar/sersic_radial_gradient.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.043687 autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/total/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1729 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/total/isothermal.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2113 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/total/isothermal_core.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2089 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/total/power_law.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2867 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/total/power_law_broken.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2473 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/total/power_law_core.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1327 2023-10-13 13:59:05.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/total/power_law_multipole.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.056687 autogalaxy-2024.5.16.0/autogalaxy/config/priors/mesh/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      225 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/mesh/README.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       10 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/mesh/delaunay.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      385 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/mesh/rectangular.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        8 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/mesh/voronoi.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       10 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/mesh/voronoi_nn.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1536 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/point_sources.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.082724 autogalaxy-2024.5.16.0/autogalaxy/config/priors/regularization/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      246 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/regularization/README.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1251 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/regularization/adaptive_brightness.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1087 2023-03-24 12:25:33.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/regularization/adaptive_brightness_split_zeroth.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      211 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/regularization/constant.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      216 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/regularization/constant_split.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      434 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/regularization/constant_zeroth.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      436 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/regularization/exponential_kernel.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      433 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/regularization/gaussian_kernel.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      620 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/regularization/matern_kernel.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      209 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/priors/regularization/zeroth.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.097687 autogalaxy-2024.5.16.0/autogalaxy/config/visualize/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      696 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/visualize/README.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      174 2023-05-10 13:41:17.000000 autogalaxy-2024.5.16.0/autogalaxy/config/visualize/general.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      275 2023-11-08 09:34:47.000000 autogalaxy-2024.5.16.0/autogalaxy/config/visualize/include.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      259 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/config/visualize/mat_wrap_1d.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      947 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/config/visualize/mat_wrap_2d.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6811 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/config/visualize/plots.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12336 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/convert.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.106690 autogalaxy-2024.5.16.0/autogalaxy/cosmology/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      150 2023-08-09 13:35:03.000000 autogalaxy-2024.5.16.0/autogalaxy/cosmology/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14342 2023-10-16 10:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/cosmology/lensing.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      933 2023-08-14 09:39:59.000000 autogalaxy-2024.5.16.0/autogalaxy/cosmology/model.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1431 2023-09-18 12:54:03.000000 autogalaxy-2024.5.16.0/autogalaxy/cosmology/wrap.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3666 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/exc.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7098 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/fixtures.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.119687 autogalaxy-2024.5.16.0/autogalaxy/galaxy/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/autogalaxy/galaxy/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    19754 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/galaxy/galaxies.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    22587 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/galaxy/galaxy.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.123686 autogalaxy-2024.5.16.0/autogalaxy/galaxy/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/autogalaxy/galaxy/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      714 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/galaxy/mock/mock_galaxy.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.133687 autogalaxy-2024.5.16.0/autogalaxy/galaxy/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2024.5.16.0/autogalaxy/galaxy/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2787 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/galaxy/plot/adapt_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13530 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/autogalaxy/galaxy/plot/galaxies_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    40483 2024-01-15 10:57:50.000000 autogalaxy-2024.5.16.0/autogalaxy/galaxy/plot/galaxy_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1002 2022-12-20 17:00:47.000000 autogalaxy-2024.5.16.0/autogalaxy/galaxy/redshift.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1772 2023-05-10 13:41:17.000000 autogalaxy-2024.5.16.0/autogalaxy/galaxy/stellar_dark_decomp.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11210 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/autogalaxy/galaxy/to_inversion.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.139686 autogalaxy-2024.5.16.0/autogalaxy/gui/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/autogalaxy/gui/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2041 2023-05-10 13:41:17.000000 autogalaxy-2024.5.16.0/autogalaxy/gui/clicker.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6979 2024-05-15 16:53:28.000000 autogalaxy-2024.5.16.0/autogalaxy/gui/scribbler.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.144963 autogalaxy-2024.5.16.0/autogalaxy/imaging/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2024.5.16.0/autogalaxy/imaging/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13374 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/imaging/fit_imaging.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.156847 autogalaxy-2024.5.16.0/autogalaxy/imaging/model/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2024.5.16.0/autogalaxy/imaging/model/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11706 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/imaging/model/analysis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6021 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/imaging/model/plotter_interface.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1689 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/imaging/model/result.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3656 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/imaging/model/visualizer.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.160073 autogalaxy-2024.5.16.0/autogalaxy/imaging/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2024.5.16.0/autogalaxy/imaging/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9595 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/imaging/plot/fit_imaging_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1526 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/imaging/simulator.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.166767 autogalaxy-2024.5.16.0/autogalaxy/interferometer/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2024.5.16.0/autogalaxy/interferometer/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11034 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/interferometer/fit_interferometer.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.177802 autogalaxy-2024.5.16.0/autogalaxy/interferometer/model/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2024.5.16.0/autogalaxy/interferometer/model/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12395 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/interferometer/model/analysis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7546 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/interferometer/model/plotter_interface.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2479 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/interferometer/model/result.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4165 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/interferometer/model/visualizer.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.182319 autogalaxy-2024.5.16.0/autogalaxy/interferometer/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2024.5.16.0/autogalaxy/interferometer/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8336 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/interferometer/plot/fit_interferometer_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1293 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/interferometer/simulator.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      341 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/mock.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.189346 autogalaxy-2024.5.16.0/autogalaxy/operate/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2024.5.16.0/autogalaxy/operate/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    36187 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/operate/deflections.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    20132 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/operate/image.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.197945 autogalaxy-2024.5.16.0/autogalaxy/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3354 2024-05-15 16:53:28.000000 autogalaxy-2024.5.16.0/autogalaxy/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      553 2024-01-15 10:57:44.000000 autogalaxy-2024.5.16.0/autogalaxy/plot/abstract_plotters.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.203412 autogalaxy-2024.5.16.0/autogalaxy/plot/get_visuals/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/plot/get_visuals/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9924 2023-05-10 13:41:17.000000 autogalaxy-2024.5.16.0/autogalaxy/plot/get_visuals/one_d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12066 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/plot/get_visuals/two_d.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.210369 autogalaxy-2024.5.16.0/autogalaxy/plot/include/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/plot/include/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1470 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/plot/include/one_d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2658 2023-05-10 13:41:17.000000 autogalaxy-2024.5.16.0/autogalaxy/plot/include/two_d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4725 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/plot/mass_plotter.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.218367 autogalaxy-2024.5.16.0/autogalaxy/plot/mat_plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/plot/mat_plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6249 2023-06-14 09:25:05.000000 autogalaxy-2024.5.16.0/autogalaxy/plot/mat_plot/one_d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10413 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/plot/mat_plot/two_d.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.224367 autogalaxy-2024.5.16.0/autogalaxy/plot/visuals/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/plot/visuals/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2123 2023-05-10 13:41:17.000000 autogalaxy-2024.5.16.0/autogalaxy/plot/visuals/one_d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4157 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/plot/visuals/two_d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      646 2023-03-18 16:31:03.000000 autogalaxy-2024.5.16.0/autogalaxy/plot/wrap.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.236368 autogalaxy-2024.5.16.0/autogalaxy/profiles/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2020-11-11 16:43:14.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13825 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/geometry_profiles.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.245388 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5547 2024-05-15 16:53:28.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1893 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/basis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2511 2024-04-03 17:53:55.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/decorators.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.274372 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/linear/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      617 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/linear/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7093 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/linear/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/linear/chameleon.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1859 2023-05-10 13:41:17.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/linear/dev_vaucouleurs.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/linear/eff.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1835 2023-05-10 13:41:17.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/linear/exponential.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1734 2022-12-16 19:36:21.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/linear/exponential_core.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1755 2023-09-21 10:00:31.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/linear/gaussian.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1749 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/linear/moffat.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2223 2023-05-10 13:41:17.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/linear/sersic.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2730 2022-12-16 19:36:21.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/linear/sersic_core.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.286368 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/linear/shapelets/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/linear/shapelets/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4497 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/linear/shapelets/cartesian.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4719 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/linear/shapelets/exponential.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2952 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/linear/shapelets/polar.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.297368 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/linear_operated/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       99 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/linear_operated/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      207 2023-05-10 13:41:17.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/linear_operated/gaussian.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      203 2023-05-10 13:41:17.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/linear_operated/moffat.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      203 2023-05-10 13:41:17.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/linear_operated/sersic.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.302368 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1030 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/mock/mock_light_profile.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.316368 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/operated/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      143 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/operated/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       39 2023-05-10 13:41:17.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/operated/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      200 2023-05-10 13:41:17.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/operated/gaussian.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      196 2023-05-10 13:41:17.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/operated/moffat.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      196 2023-05-10 13:41:17.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/operated/sersic.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.339367 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/snr/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      371 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/snr/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4017 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/snr/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3255 2022-12-16 19:36:21.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/snr/chameleon.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2581 2022-12-16 19:36:21.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/snr/dev_vaucouleurs.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2782 2022-12-16 19:36:21.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/snr/eff.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2504 2022-12-16 19:36:21.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/snr/exponential.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2227 2022-12-16 19:36:21.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/snr/gaussian.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2736 2022-12-16 19:36:21.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/snr/sersic.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2338 2022-12-16 19:36:21.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/snr/sersic_core.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.368368 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/standard/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      706 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/standard/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5909 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/standard/chameleon.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2351 2022-12-16 19:36:21.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/standard/dev_vaucouleurs.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4472 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/standard/eff.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2316 2022-12-16 19:36:21.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/standard/exponential.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3188 2022-12-16 19:36:21.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/standard/exponential_core.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4284 2024-05-15 16:53:28.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/standard/gaussian.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4963 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/standard/moffat.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7742 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/standard/sersic.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5744 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/standard/sersic_core.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.385369 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/standard/shapelets/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/standard/shapelets/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1218 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/standard/shapelets/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5062 2024-05-15 16:53:28.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/standard/shapelets/cartesian.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5315 2024-05-15 16:53:28.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/standard/shapelets/exponential.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5199 2024-05-15 16:53:28.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light/standard/shapelets/polar.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    25207 2023-05-10 13:41:17.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/light_and_mass_profiles.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.389372 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1047 2023-10-16 19:31:40.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.400367 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/abstract/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/abstract/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6039 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/abstract/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7141 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/abstract/cse.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8695 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/abstract/mge.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.433368 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/dark/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      496 2023-10-16 19:31:40.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/dark/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11758 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/dark/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13561 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/dark/gnfw.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1130 2023-05-10 13:41:17.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/dark/gnfw_mcr.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3823 2023-10-16 19:31:40.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/dark/mcr_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11757 2024-05-14 13:52:22.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/dark/nfw.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2439 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/dark/nfw_mcr.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2090 2024-05-14 13:52:22.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/dark/nfw_mcr_scatter.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4407 2024-05-14 13:51:28.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/dark/nfw_truncated.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2089 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/dark/nfw_truncated_mcr.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1161 2023-05-10 13:41:17.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/dark/nfw_truncated_mcr_scatter.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2747 2023-10-16 19:31:40.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/dark/nfw_virial_mass_conc.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.438369 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      714 2023-05-10 13:41:17.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/mock/mock_mass_profile.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.449367 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/point/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       91 2023-05-17 15:24:31.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/point/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1704 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/point/point.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1653 2023-08-09 13:35:04.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/point/smbh.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5023 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/point/smbh_binary.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.462369 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/sheets/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      127 2022-12-16 18:30:52.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/sheets/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2570 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/sheets/external_shear.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4930 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/sheets/input_deflections.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1385 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/sheets/mass_sheet.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.489392 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/stellar/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      372 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/stellar/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       33 2023-05-10 13:41:17.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/stellar/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8377 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/stellar/chameleon.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2478 2022-12-16 19:36:21.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/stellar/dev_vaucouleurs.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2472 2022-12-16 19:36:21.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/stellar/exponential.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7526 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/stellar/gaussian.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    16705 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/stellar/sersic.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7058 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/stellar/sersic_core.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9713 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/stellar/sersic_radial_gradient.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.509405 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/total/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      337 2023-05-31 17:24:34.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/total/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6760 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/total/isothermal.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2109 2022-12-16 19:36:21.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/total/isothermal_core.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5526 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/total/power_law.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6250 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/total/power_law_broken.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8263 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/total/power_law_core.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7633 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/total/power_law_multipole.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.519400 autogalaxy-2024.5.16.0/autogalaxy/profiles/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5835 2024-05-15 16:53:28.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/plot/basis_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12951 2024-01-15 10:57:46.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/plot/light_profile_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14759 2024-01-15 10:57:48.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/plot/mass_profile_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      467 2023-05-10 13:41:17.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/point_sources.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1450 2023-05-10 13:41:17.000000 autogalaxy-2024.5.16.0/autogalaxy/profiles/scaling_relations.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.525369 autogalaxy-2024.5.16.0/autogalaxy/quantity/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2024.5.16.0/autogalaxy/quantity/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9780 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/autogalaxy/quantity/dataset_quantity.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4474 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/autogalaxy/quantity/fit_quantity.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.538368 autogalaxy-2024.5.16.0/autogalaxy/quantity/model/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2024.5.16.0/autogalaxy/quantity/model/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7023 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/autogalaxy/quantity/model/analysis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3531 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/autogalaxy/quantity/model/plotter_interface.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      451 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/autogalaxy/quantity/model/result.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1923 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/autogalaxy/quantity/model/visualizer.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.542369 autogalaxy-2024.5.16.0/autogalaxy/quantity/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2024.5.16.0/autogalaxy/quantity/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8126 2023-05-10 13:41:17.000000 autogalaxy-2024.5.16.0/autogalaxy/quantity/plot/fit_quantity_plotters.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.549368 autogalaxy-2024.5.16.0/autogalaxy/util/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1288 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/autogalaxy/util/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2572 2023-05-10 13:41:17.000000 autogalaxy-2024.5.16.0/autogalaxy/util/error_util.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.553368 autogalaxy-2024.5.16.0/autogalaxy/util/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/autogalaxy/util/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1353 2023-08-09 13:35:03.000000 autogalaxy-2024.5.16.0/autogalaxy/util/mock/mock_cosmology.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4484 2023-12-01 11:10:14.000000 autogalaxy-2024.5.16.0/autogalaxy/util/shear_field.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.851369 autogalaxy-2024.5.16.0/autogalaxy.egg-info/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    17781 2024-05-16 09:58:25.000000 autogalaxy-2024.5.16.0/autogalaxy.egg-info/SOURCES.txt
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.558368 autogalaxy-2024.5.16.0/docs/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.562368 autogalaxy-2024.5.16.0/docs/_templates/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      832 2022-12-21 16:35:52.000000 autogalaxy-2024.5.16.0/docs/_templates/custom-class-template.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1293 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/docs/_templates/custom_module_template.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.569381 autogalaxy-2024.5.16.0/docs/advanced/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      388 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/docs/advanced/chaining.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6369 2023-10-16 19:31:40.000000 autogalaxy-2024.5.16.0/docs/advanced/database.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1374 2023-05-10 13:41:17.000000 autogalaxy-2024.5.16.0/docs/advanced/graphical.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.586371 autogalaxy-2024.5.16.0/docs/api/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2083 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/docs/api/data.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      293 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/docs/api/fitting.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      627 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/docs/api/galaxy.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:25.714043 autogalaxy-2024.5.16.0/docs/api/images/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.596434 autogalaxy-2024.5.16.0/docs/api/images/pixelization_image_plane/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    41383 2022-12-21 12:27:28.000000 autogalaxy-2024.5.16.0/docs/api/images/pixelization_image_plane/data_image_plane.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    34340 2022-12-21 12:27:28.000000 autogalaxy-2024.5.16.0/docs/api/images/pixelization_image_plane/grid_image_plane.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    49269 2022-12-21 12:27:49.000000 autogalaxy-2024.5.16.0/docs/api/images/pixelization_image_plane/image_plane_mesh.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.606428 autogalaxy-2024.5.16.0/docs/api/images/pixelization_masked_image_plane/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    40349 2022-12-21 12:22:21.000000 autogalaxy-2024.5.16.0/docs/api/images/pixelization_masked_image_plane/data_image_plane.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    26453 2022-12-21 12:22:21.000000 autogalaxy-2024.5.16.0/docs/api/images/pixelization_masked_image_plane/grid_image_plane.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    48007 2022-12-21 12:28:33.000000 autogalaxy-2024.5.16.0/docs/api/images/pixelization_masked_image_plane/image_plane_mesh.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.616402 autogalaxy-2024.5.16.0/docs/api/images/pixelization_masked_source_plane/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    56739 2022-12-21 13:10:07.000000 autogalaxy-2024.5.16.0/docs/api/images/pixelization_masked_source_plane/data_image_plane.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    27379 2022-12-21 13:10:07.000000 autogalaxy-2024.5.16.0/docs/api/images/pixelization_masked_source_plane/grid_image_plane.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    77426 2022-12-21 13:10:07.000000 autogalaxy-2024.5.16.0/docs/api/images/pixelization_masked_source_plane/source_plane_mesh.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      531 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/docs/api/light.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1338 2023-09-18 12:54:03.000000 autogalaxy-2024.5.16.0/docs/api/modeling.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1904 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/docs/api/pixelization.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3146 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/docs/api/plot.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2420 2023-05-31 17:24:34.000000 autogalaxy-2024.5.16.0/docs/api/source.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4631 2023-05-10 13:41:17.000000 autogalaxy-2024.5.16.0/docs/conf.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.631373 autogalaxy-2024.5.16.0/docs/general/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1335 2023-06-16 08:24:22.000000 autogalaxy-2024.5.16.0/docs/general/citations.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1035 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/docs/general/configs.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1315 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/docs/general/credits.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      981 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/docs/general/likelihood_function.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9304 2023-09-18 12:54:03.000000 autogalaxy-2024.5.16.0/docs/general/model_cookbook.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      236 2023-08-14 09:39:59.000000 autogalaxy-2024.5.16.0/docs/general/papers.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2450 2023-05-12 11:43:15.000000 autogalaxy-2024.5.16.0/docs/general/workspace.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.644369 autogalaxy-2024.5.16.0/docs/howtogalaxy/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1387 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/docs/howtogalaxy/chapter_1_introduction.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2658 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/docs/howtogalaxy/chapter_2_modeling.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1038 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/docs/howtogalaxy/chapter_3_search_chaining.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1416 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/docs/howtogalaxy/chapter_4_pixelizations.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      960 2023-06-06 10:32:01.000000 autogalaxy-2024.5.16.0/docs/howtogalaxy/chapter_optional.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3447 2023-05-12 10:01:56.000000 autogalaxy-2024.5.16.0/docs/howtogalaxy/howtogalaxy.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11362 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/docs/index.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.659368 autogalaxy-2024.5.16.0/docs/installation/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4014 2024-05-16 09:55:27.000000 autogalaxy-2024.5.16.0/docs/installation/conda.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3519 2023-05-12 10:01:56.000000 autogalaxy-2024.5.16.0/docs/installation/numba.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2409 2023-10-23 12:35:45.000000 autogalaxy-2024.5.16.0/docs/installation/overview.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3442 2024-05-16 09:55:27.000000 autogalaxy-2024.5.16.0/docs/installation/pip.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4703 2023-05-12 10:10:15.000000 autogalaxy-2024.5.16.0/docs/installation/source.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2678 2023-06-07 11:44:12.000000 autogalaxy-2024.5.16.0/docs/installation/troubleshooting.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.676368 autogalaxy-2024.5.16.0/docs/overview/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:25.722353 autogalaxy-2024.5.16.0/docs/overview/images/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.714368 autogalaxy-2024.5.16.0/docs/overview/images/fitting/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    37264 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/docs/overview/images/fitting/bad_chi_squared_map.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    63409 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/docs/overview/images/fitting/bad_normalized_residual_map.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    39647 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/docs/overview/images/fitting/bad_residual_map.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    51168 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/docs/overview/images/fitting/chi_squared_map.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    35309 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/docs/overview/images/fitting/image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    37035 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/docs/overview/images/fitting/masked_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    33220 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/docs/overview/images/fitting/model_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    44440 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/docs/overview/images/fitting/noise_map.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    69331 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/docs/overview/images/fitting/normalized_residual_map.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    30136 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/docs/overview/images/fitting/plane_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    31550 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/docs/overview/images/fitting/psf.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    65595 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/docs/overview/images/fitting/residual_map.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.732369 autogalaxy-2024.5.16.0/docs/overview/images/galaxies/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    28953 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/docs/overview/images/galaxies/galaxy.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    21591 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/docs/overview/images/galaxies/grid_2d.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    29995 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/docs/overview/images/galaxies/merging_galaxies.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    29232 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/docs/overview/images/galaxies/plane.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    29344 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/docs/overview/images/galaxies/sersic_light_profile.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    35172 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/docs/overview/images/galaxies/subplot_galaxies.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.757367 autogalaxy-2024.5.16.0/docs/overview/images/interferometry/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   107396 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/docs/overview/images/interferometry/dirty_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   113651 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/docs/overview/images/interferometry/dirty_signal_to_noise.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   390140 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/docs/overview/images/interferometry/fit_dirty_images.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    41276 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/docs/overview/images/interferometry/image_pre_ft.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    46706 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/docs/overview/images/interferometry/model_visibilities.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    45127 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/docs/overview/images/interferometry/reconstruction.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    29898 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/docs/overview/images/interferometry/uv_wavelengths.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    30950 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/docs/overview/images/interferometry/visibilities.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.766368 autogalaxy-2024.5.16.0/docs/overview/images/modeling/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)  1175623 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/docs/overview/images/modeling/cornerplot.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    39125 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/docs/overview/images/modeling/image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   231702 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/docs/overview/images/modeling/subplot_fit.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.783367 autogalaxy-2024.5.16.0/docs/overview/images/multiwavelength/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    73817 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/docs/overview/images/multiwavelength/dirty_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    75926 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/docs/overview/images/multiwavelength/g_decomposed_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   152814 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/docs/overview/images/multiwavelength/g_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   141963 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/docs/overview/images/multiwavelength/r_decomposed_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   140328 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/docs/overview/images/multiwavelength/r_image.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.789367 autogalaxy-2024.5.16.0/docs/overview/images/pixelizations/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    38896 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/docs/overview/images/pixelizations/image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    40489 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/docs/overview/images/pixelizations/rectangular.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.811368 autogalaxy-2024.5.16.0/docs/overview/images/simulating/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   106644 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/docs/overview/images/simulating/ao.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    37696 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/docs/overview/images/simulating/euclid.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    80336 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/docs/overview/images/simulating/hst.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    35633 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/docs/overview/images/simulating/image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    43310 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/docs/overview/images/simulating/noise_map.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    33339 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/docs/overview/images/simulating/psf.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    49620 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/docs/overview/images/simulating/vro.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8215 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/docs/overview/overview_1_galaxies.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6562 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/docs/overview/overview_2_fitting.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    23454 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/docs/overview/overview_3_modeling.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2958 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/docs/overview/overview_4_simulate.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4367 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/docs/overview/overview_5_pixelizations.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8861 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/docs/overview/overview_6_interferometry.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10653 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/docs/overview/overview_7_multi_wavelength.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      179 2022-12-16 17:06:50.000000 autogalaxy-2024.5.16.0/docs/requirements.txt
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       33 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/eden.ini
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.830369 autogalaxy-2024.5.16.0/files/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    25824 2023-06-16 08:34:40.000000 autogalaxy-2024.5.16.0/files/citations.bib
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1727 2023-06-16 08:34:40.000000 autogalaxy-2024.5.16.0/files/citations.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2307 2023-06-16 08:34:40.000000 autogalaxy-2024.5.16.0/files/citations.tex
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    43549 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/files/dirty_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    29819 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/files/model_dirty_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    67674 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/files/non_parametric.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   139037 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/files/observed.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    43670 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/files/parametric.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   223339 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/files/visibilities.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      113 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/optional_requirements.txt
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:26.850368 autogalaxy-2024.5.16.0/paper/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      190 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/paper/README.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   399405 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/paper/almacombined.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   342368 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/paper/hstcombined.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   122730 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/paper/observed.pdf
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    45539 2023-02-21 10:35:21.000000 autogalaxy-2024.5.16.0/paper/paper.bib
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      830 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/paper/paper.json
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13526 2023-10-23 12:35:45.000000 autogalaxy-2024.5.16.0/paper/paper.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    43670 2022-11-24 19:55:46.000000 autogalaxy-2024.5.16.0/paper/parametric.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      201 2022-12-19 13:59:53.000000 autogalaxy-2024.5.16.0/readthedocs.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       54 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/requirements.txt
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       38 2024-05-16 09:58:26.854380 autogalaxy-2024.5.16.0/setup.cfg
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2017 2024-05-16 09:56:09.000000 autogalaxy-2024.5.16.0/setup.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3014 2024-05-14 13:51:29.000000 autogalaxy-2024.5.16.0/zenodo.json
```

### Comparing `autogalaxy-2024.1.27.4/CITATIONS.rst` & `autogalaxy-2024.5.16.0/CITATIONS.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/LICENSE` & `autogalaxy-2024.5.16.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/PKG-INFO` & `autogalaxy-2024.5.16.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogalaxy
-Version: 2024.1.27.4
+Version: 2024.5.16.0
 Summary: Open-Source Multi Wavelength Galaxy Structure & Morphology
 Home-page: https://github.com/Jammy2211/PyAutoGalaxy
 Author: James Nightingale and Richard Hayes
 Author-email: james.w.nightingale@durham.ac.uk
 License: MIT License
 Keywords: cli
 Classifier: Intended Audience :: Science/Research
@@ -15,20 +15,14 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: colossus==1.3.1
-Requires-Dist: astropy>=5.0
-Requires-Dist: nautilus-sampler==0.7.4
-Requires-Dist: autoconf==2024.1.27.4
-Requires-Dist: autoarray==2024.1.27.4
-Requires-Dist: autofit==2024.1.27.4
 
 PyAutoGalaxy: Open-Source Multi Wavelength Galaxy Structure & Morphology
 ========================================================================
 
 .. image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/Jammy2211/autogalaxy_workspace/HEAD
 
@@ -134,15 +128,15 @@
         galaxies=[galaxy],
     )
 
     """
     We can use the Grid2D and Plane to perform many calculations, for example
     plotting the image of the galaxyed source.
     """
-    plane_plotter = aplt.PlanePlotter(plane=plane, grid=grid)
+    plane_plotter = aplt.GalaxiesPlotter(plane=plane, grid=grid)
     plane_plotter.figures_2d(image=True)
 
 
 With **PyAutoGalaxy**, you can begin modeling a galaxy in just a couple of minutes. The example below demonstrates a
 simple analysis which fits a galaxy's light.
 
 .. code-block:: python
```

### Comparing `autogalaxy-2024.1.27.4/README.rst` & `autogalaxy-2024.5.16.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         galaxies=[galaxy],
     )
 
     """
     We can use the Grid2D and Plane to perform many calculations, for example
     plotting the image of the galaxyed source.
     """
-    plane_plotter = aplt.PlanePlotter(plane=plane, grid=grid)
+    plane_plotter = aplt.GalaxiesPlotter(plane=plane, grid=grid)
     plane_plotter.figures_2d(image=True)
 
 
 With **PyAutoGalaxy**, you can begin modeling a galaxy in just a couple of minutes. The example below demonstrates a
 simple analysis which fits a galaxy's light.
 
 .. code-block:: python
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/__init__.py` & `autogalaxy-2024.5.16.0/autogalaxy/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,21 @@
 from autoconf.dictable import from_dict, from_json, output_to_json, to_dict
 from autoarray.dataset import preprocess  # noqa
-from autoarray.dataset.imaging.settings import SettingsImaging  # noqa
 from autoarray.dataset.imaging.dataset import Imaging  # noqa
 from autoarray.dataset.interferometer.dataset import Interferometer  # noqa
-from autoarray.dataset.interferometer.settings import SettingsInterferometer  # noqa
+from autoarray.dataset.dataset_model import DatasetModel
 from autoarray.inversion.pixelization import mesh  # noqa
 from autoarray.inversion import regularization as reg  # noqa
 from autoarray.inversion.pixelization import image_mesh
 from autoarray.inversion.pixelization.mappers.abstract import AbstractMapper  # noqa
 from autoarray.inversion.inversion.settings import SettingsInversion  # noqa
 from autoarray.inversion.inversion.factory import inversion_from as Inversion  # noqa
 from autoarray.inversion.pixelization.image_mesh.abstract import AbstractImageMesh
 from autoarray.inversion.pixelization.mesh.abstract import AbstractMesh
 from autoarray.inversion.regularization.abstract import AbstractRegularization
-from autoarray.inversion.inversion.factory import (
-    inversion_imaging_unpacked_from as InversionImaging,
-)  # noqa
-from autoarray.inversion.inversion.factory import (
-    inversion_interferometer_unpacked_from as InversionInterferometer,
-)  # noqa
 from autoarray.inversion.pixelization.pixelization import Pixelization  # noqa
 from autoarray.inversion.pixelization.mappers.abstract import AbstractMapper
 from autoarray.inversion.pixelization.mappers.mapper_grids import MapperGrids  # noqa
 from autoarray.inversion.pixelization.mappers.factory import (
     mapper_from as Mapper,
 )  # noqa
 from autoarray.mask.mask_1d import Mask1D  # noqa
@@ -34,29 +27,33 @@
 from autoarray.layout.layout import Layout2D  # noqa
 from autoarray.structures.arrays.uniform_1d import Array1D  # noqa
 from autoarray.structures.arrays.uniform_2d import Array2D  # noqa
 from autoarray.structures.arrays.irregular import ArrayIrregular  # noqa
 from autoarray.structures.header import Header  # noqa
 from autoarray.structures.grids.uniform_1d import Grid1D  # noqa
 from autoarray.structures.grids.uniform_2d import Grid2D  # noqa
-from autoarray.structures.grids.iterate_2d import Grid2DIterate  # noqa
 from autoarray.structures.grids.irregular_2d import Grid2DIrregular  # noqa
 from autoarray.structures.grids.irregular_2d import Grid2DIrregularUniform  # noqa
+from autoarray.operators.over_sampling.uniform import OverSamplingUniform  # noqa
+from autoarray.operators.over_sampling.uniform import OverSamplerUniform  # noqa
+from autoarray.operators.over_sampling.iterate import OverSamplingIterate
+from autoarray.operators.over_sampling.iterate import OverSamplerIterate
 from autoarray.structures.mesh.rectangular_2d import Mesh2DRectangular  # noqa
 from autoarray.structures.mesh.voronoi_2d import Mesh2DVoronoi  # noqa
 from autoarray.structures.mesh.delaunay_2d import Mesh2DDelaunay  # noqa
 from autoarray.structures.vectors.uniform import VectorYX2D  # noqa
 from autoarray.structures.vectors.irregular import VectorYX2DIrregular  # noqa
 from autoarray.layout.region import Region1D  # noqa
 from autoarray.layout.region import Region2D  # noqa
 from autoarray.structures.arrays.kernel_2d import Kernel2D  # noqa
 from autoarray.structures.visibilities import Visibilities  # noqa
 from autoarray.structures.visibilities import VisibilitiesNoiseMap  # noqa
 
-from .analysis.adapt_images import AdaptImages
+from .analysis.adapt_images.adapt_images import AdaptImages
+from .analysis.adapt_images.adapt_image_maker import AdaptImageMaker
 from .analysis.maker import FitMaker
 from .analysis.preloads import Preloads
 from . import aggregator as agg
 from . import exc
 from . import plot
 from . import util
 from .operate.image import OperateImage
@@ -71,32 +68,31 @@
 from .interferometer.fit_interferometer import FitInterferometer
 from .interferometer.model.analysis import AnalysisInterferometer
 
 from .quantity.fit_quantity import FitQuantity
 from .quantity.model.analysis import AnalysisQuantity
 from .quantity.dataset_quantity import DatasetQuantity
 from .galaxy.galaxy import Galaxy
+from .galaxy.galaxies import Galaxies
 from .galaxy.redshift import Redshift
 from .galaxy.stellar_dark_decomp import StellarDarkDecomp
-from .plane.plane import Plane
-from .plane.to_inversion import AbstractToInversion
-from .plane.to_inversion import PlaneToInversion
+from .galaxy.to_inversion import AbstractToInversion
+from .galaxy.to_inversion import GalaxiesToInversion
 from .profiles.geometry_profiles import EllProfile
 from .profiles import (
     point_sources as ps,
     mass as mp,
     light_and_mass_profiles as lmp,
     scaling_relations as sr,
 )
 from .profiles.light.abstract import LightProfile
 from .profiles.light import standard as lp
 from .profiles.light import basis as lp_basis
 from .profiles.light.linear import LightProfileLinearObjFuncList
 from .profiles.light import linear as lp_linear
-from .profiles.light import shapelets as lp_shapelets
 from .profiles.light import operated as lp_operated
 from .profiles.light import (
     linear_operated as lp_linear_operated,
 )
 from .profiles.light import snr as lp_snr
 from . import convert
 from . import mock as m  # noqa
@@ -108,8 +104,8 @@
 
 from .analysis.clump_model import ClumpModel
 
 from autoconf import conf
 
 conf.instance.register(__file__)
 
-__version__ = "2024.1.27.4"
+__version__ = "2024.5.16.0"
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/abstract_fit.py` & `autogalaxy-2024.5.16.0/autogalaxy/abstract_fit.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,31 +4,37 @@
 from autofit import ModelInstance
 
 if TYPE_CHECKING:
     from autogalaxy.galaxy.galaxy import Galaxy
 
 import autoarray as aa
 
+from autogalaxy.profiles.light.abstract import LightProfile
 from autogalaxy.profiles.light.linear import LightProfileLinear
 from autogalaxy.profiles.light.basis import Basis
 
 
 class AbstractFitInversion:
-    def __init__(self, model_obj, settings_inversion: aa.SettingsInversion):
+    def __init__(
+        self,
+        model_obj,
+        settings_inversion: aa.SettingsInversion,
+    ):
         """
         An abstract fit object which fits to datasets (e.g. imaging, interferometer) inherit from.
 
-        This object primarily inspects the `model_obj` (e.g. a plane object PyAutoGalaxy or tracer in PyAutoLens)
+        This object primarily inspects the `model_obj` (e.g. a galaxies object PyAutoGalaxy or tracer in PyAutoLens)
         and determines the properties used for the fit by inspecting the galaxies / light profiles in this object.
 
         Parameters
         ----------
         model_obj
             The object which contains the model components (e.g. light profiles, galaxies, etc) which are used to
-            create the model-data that fits the data. In PyAutoGalaxy this is a `Plane` and PyAutoLens it is a `Tracer`.
+            create the model-data that fits the data. In PyAutoGalaxy this is a list of galaxies and PyAutoLens
+            it is a `Tracer`.
         settings_inversion
             Settings controlling how an inversion is fitted for example which linear algebra formalism is used.
         """
         self.model_obj = model_obj
         self.settings_inversion = settings_inversion
 
     @property
@@ -142,15 +148,18 @@
         """
         if self.inversion is None:
             return {}
 
         galaxy_linear_obj_image_dict = {}
 
         for linear_obj in self.inversion.linear_obj_list:
-            galaxy = self.inversion.linear_obj_galaxy_dict[linear_obj]
+            try:
+                galaxy = self.inversion.linear_obj_galaxy_dict[linear_obj]
+            except KeyError:
+                continue
 
             if not use_image:
                 mapped_reconstructed = self.inversion.mapped_reconstructed_data_dict[
                     linear_obj
                 ]
 
             else:
@@ -174,25 +183,47 @@
         This means they are difficult to visualize, because they do not have a valid `intensity` parameter.
 
         To address this, this property creates a new `model_obj` where all linear light profiles are converted to
         ordinary light profiles whose `intensity` parameters are set to the results of the Inversion.
 
         Returns
         -------
-        A `model_obj` (E.g. `Plane` or `Tracer`) where the light profile intensity values are set to the results
+        A `model_obj` (E.g. galaxies or `Tracer`) where the light profile intensity values are set to the results
         of those inferred via the `Inversion`.
         """
 
         if self.linear_light_profile_intensity_dict is None:
             return self.model_obj
 
-        model_instance = ModelInstance(dict(model_obj=self.model_obj))
+        model_instance = self.append_linear_light_profiles_to_model(
+            model_instance=ModelInstance(dict(model_obj=self.model_obj))
+        )
+
+        return model_instance.model_obj
+
+    def append_linear_light_profiles_to_model(self, model_instance):
+        """
+        For a model instance, this function replaces all linear light profiles with instances of their standard
+        light profile counterparts/
+
+        The `intensity` parameter of each light profile is set to the value inferred via the `Inversion`.
+
+        Parameters
+        ----------
+        model_instance
+            An instance of the model object (e.g. galaxies or `Tracer`) whose linear light profiles are to be
+            replaced with instances of their standard light profile counterparts.
+
+        Returns
+        -------
+        A model instance with all linear light profiles replaced with instances of their standard light profile
+        """
 
         for path, instance in model_instance.path_instance_tuples_for_class(
             (LightProfileLinear, Basis)
         ):
             model_instance = model_instance.replacing_for_path(
                 path,
                 instance.lp_instance_from(self.linear_light_profile_intensity_dict),
             )
 
-        return model_instance.model_obj
+        return model_instance
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/aggregator/agg_util.py` & `autogalaxy-2024.5.16.0/autogalaxy/aggregator/agg_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 from __future__ import annotations
-from typing import TYPE_CHECKING, List, Optional
-
-if TYPE_CHECKING:
-    from autogalaxy.galaxy.galaxy import Galaxy
+from typing import List, Optional
 
 import autofit as af
 import autoarray as aa
 
-from autogalaxy.analysis.adapt_images import AdaptImages
+from autogalaxy.analysis.adapt_images.adapt_images import AdaptImages
 
 
 def adapt_images_from(
     fit: af.Fit,
 ) -> List[AdaptImages]:
     """
     Updates adaptive images when loading the galaxies from a `PyAutoFit` sqlite database `Fit` object.
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/aggregator/fit_imaging.py` & `autogalaxy-2024.5.16.0/autogalaxy/aggregator/fit_imaging.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING, Optional, List
 
 if TYPE_CHECKING:
-    from autogalaxy.galaxy.galaxy import Galaxy
     from autogalaxy.imaging.fit_imaging import FitImaging
 
 import autofit as af
 import autoarray as aa
 
-from autogalaxy.aggregator.abstract import AbstractAgg
 from autogalaxy.analysis.preloads import Preloads
 
 from autogalaxy.aggregator.imaging import _imaging_from
-from autogalaxy.aggregator.plane import _plane_from
+from autogalaxy.aggregator.galaxies import _galaxies_from
+from autogalaxy.aggregator.dataset_model import _dataset_model_from
 from autogalaxy.aggregator import agg_util
 
 
 def _fit_imaging_from(
     fit: af.Fit,
-    galaxies: List[Galaxy],
-    settings_dataset: aa.SettingsImaging = None,
+    instance: Optional[af.ModelInstance] = None,
     settings_inversion: aa.SettingsInversion = None,
     use_preloaded_grid: bool = True,
 ) -> List[FitImaging]:
     """
     Returns a list of `FitImaging` objects from a `PyAutoFit` sqlite database `Fit` object.
 
     The results of a model-fit can be stored in a sqlite database, including the following attributes of the fit:
@@ -37,77 +35,82 @@
     This method combines all of these attributes and returns a `FitImaging` object for a given non-linear search sample
     (e.g. the maximum likelihood model). This includes associating adapt images with their respective galaxies.
 
     If multiple `FitImaging` objects were fitted simultaneously via analysis summing, the `fit.child_values()` method
     is instead used to load lists of the data, noise-map, PSF and mask and combine them into a list of
     `FitImaging` objects.
 
-    The settings of a pixelization of inversion can be overwritten by inputting a `settings_dataset` object, for example
+    The settings of an inversion can be overwritten by inputting a `settings_inversion` object, for example
     if you want to use a grid with a different inversion solver.
 
     Parameters
     ----------
     fit
         A `PyAutoFit` `Fit` object which contains the results of a model-fit as an entry in a sqlite database.
-    galaxies
-        A list of galaxies corresponding to a sample of a non-linear search and model-fit.
-    settings_dataset
-        Optionally overwrite the `SettingsImaging` of the `Imaging` object that is created from the fit.
+    instance
+        A manual instance that overwrites the max log likelihood instance in fit (e.g. for drawing the instance
+        randomly from the PDF).
     settings_inversion
         Optionally overwrite the `SettingsInversion` of the `Inversion` object that is created from the fit.
     use_preloaded_grid
         Certain pixelization's construct their mesh in the source-plane from a stochastic KMeans algorithm. This grid
         may be output to hard-disk after the model-fit and loaded via the database to ensure the same grid is used
         as the fit.
     """
 
     from autogalaxy.imaging.fit_imaging import FitImaging
 
-    dataset_list = _imaging_from(fit=fit, settings_dataset=settings_dataset)
+    dataset_list = _imaging_from(fit=fit)
 
-    plane_list = _plane_from(fit=fit, galaxies=galaxies)
+    galaxies_list = _galaxies_from(fit=fit, instance=instance)
+
+    dataset_model_list = _dataset_model_from(fit=fit, instance=instance)
 
     adapt_images_list = agg_util.adapt_images_from(fit=fit)
 
     settings_inversion = settings_inversion or fit.value(name="settings_inversion")
 
     mesh_grids_of_planes_list = agg_util.mesh_grids_of_planes_list_from(
         fit=fit, total_fits=len(dataset_list), use_preloaded_grid=use_preloaded_grid
     )
 
     fit_dataset_list = []
 
-    for dataset, plane, adapt_images, mesh_grids_of_planes in zip(
-        dataset_list, plane_list, adapt_images_list, mesh_grids_of_planes_list
+    for dataset, galaxies, dataset_model, adapt_images, mesh_grids_of_planes in zip(
+        dataset_list,
+        galaxies_list,
+        dataset_model_list,
+        adapt_images_list,
+        mesh_grids_of_planes_list,
     ):
         preloads = agg_util.preloads_from(
             preloads_cls=Preloads,
             use_preloaded_grid=use_preloaded_grid,
             mesh_grids_of_planes=mesh_grids_of_planes,
             use_w_tilde=False,
         )
 
         fit_dataset_list.append(
             FitImaging(
                 dataset=dataset,
-                plane=plane,
+                galaxies=galaxies,
+                dataset_model=dataset_model,
                 adapt_images=adapt_images,
                 settings_inversion=settings_inversion,
                 preloads=preloads,
             )
         )
 
     return fit_dataset_list
 
 
-class FitImagingAgg(AbstractAgg):
+class FitImagingAgg(af.AggBase):
     def __init__(
         self,
         aggregator: af.Aggregator,
-        settings_dataset: Optional[aa.SettingsImaging] = None,
         settings_inversion: Optional[aa.SettingsInversion] = None,
         use_preloaded_grid: bool = True,
     ):
         """
         Interfaces with an `PyAutoFit` aggregator object to create instances of `FitImaging` objects from the results
         of a model-fit.
 
@@ -133,42 +136,41 @@
 
         This can be done manually, but this object provides a more concise API.
 
         Parameters
         ----------
         aggregator
             A `PyAutoFit` aggregator object which can load the results of model-fits.
-        settings_dataset
-            Optionally overwrite the `SettingsImaging` of the `Imaging` object that is created from the fit.
         settings_inversion
             Optionally overwrite the `SettingsInversion` of the `Inversion` object that is created from the fit.
         use_preloaded_grid
             Certain pixelization's construct their mesh in the source-plane from a stochastic KMeans algorithm. This
             grid may be output to hard-disk after the model-fit and loaded via the database to ensure the same grid is
             used as the fit.
         """
         super().__init__(aggregator=aggregator)
 
-        self.settings_dataset = settings_dataset
         self.settings_inversion = settings_inversion
         self.use_preloaded_grid = use_preloaded_grid
 
-    def object_via_gen_from(self, fit, galaxies) -> List[FitImaging]:
+    def object_via_gen_from(
+        self, fit, instance: Optional[af.ModelInstance] = None
+    ) -> List[FitImaging]:
         """
         Returns a generator of `FitImaging` objects from an input aggregator.
 
         See `__init__` for a description of how the `FitImaging` objects are created by this method.
 
         Parameters
         ----------
         fit
             A `PyAutoFit` `Fit` object which contains the results of a model-fit as an entry in a sqlite database.
-        galaxies
-            A list of galaxies corresponding to a sample of a non-linear search and model-fit.
+        instance
+            A manual instance that overwrites the max log likelihood instance in fit (e.g. for drawing the instance
+            randomly from the PDF).
         """
         return _fit_imaging_from(
             fit=fit,
-            galaxies=galaxies,
-            settings_dataset=self.settings_dataset,
+            instance=instance,
             settings_inversion=self.settings_inversion,
             use_preloaded_grid=self.use_preloaded_grid,
         )
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/aggregator/fit_interferometer.py` & `autogalaxy-2024.5.16.0/autogalaxy/aggregator/fit_interferometer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING, Optional, List
 
 if TYPE_CHECKING:
-    from autogalaxy.galaxy.galaxy import Galaxy
     from autogalaxy.interferometer.fit_interferometer import FitInterferometer
 
 import autofit as af
 import autoarray as aa
 
-from autogalaxy.aggregator.abstract import AbstractAgg
 from autogalaxy.analysis.preloads import Preloads
 
 from autogalaxy.aggregator import agg_util
 from autogalaxy.aggregator.interferometer import _interferometer_from
-from autogalaxy.aggregator.plane import _plane_from
+from autogalaxy.aggregator.dataset_model import _dataset_model_from
+from autogalaxy.aggregator.galaxies import _galaxies_from
 
 
 def _fit_interferometer_from(
     fit: af.Fit,
-    galaxies: List[Galaxy],
+    instance: Optional[af.ModelInstance] = None,
     real_space_mask: Optional[aa.Mask2D] = None,
-    settings_dataset: aa.SettingsInterferometer = None,
     settings_inversion: aa.SettingsInversion = None,
     use_preloaded_grid: bool = True,
 ) -> List[FitInterferometer]:
     """
     Returns a list of `FitInterferometer` objects from a `PyAutoFit` sqlite database `Fit` object.
 
     The results of a model-fit can be stored in a sqlite database, including the following attributes of the fit:
@@ -39,80 +37,84 @@
     search sample (e.g. the maximum likelihood model). This includes associating adapt images with their respective
     galaxies.
 
     If multiple `FitInterferometer` objects were fitted simultaneously via analysis summing, the `fit.child_values()`
     method is instead used to load lists of the data, noise-map, PSF and mask and combine them into a list of
     `FitInterferometer` objects.
 
-    The settings of a pixelization of inversion can be overwritten by inputting a `settings_dataset` object, for
+    The settings of an inversion can be overwritten by inputting a `settings_inversion` object, for
     example if you want to use a grid with a different inversion solver.
 
     Parameters
     ----------
     fit
         A `PyAutoFit` `Fit` object which contains the results of a model-fit as an entry in a sqlite database.
-    galaxies
-        A list of galaxies corresponding to a sample of a non-linear search and model-fit.
-    settings_dataset
-        Optionally overwrite the `SettingsInterferometer` of the `Interferometer` object that is created from the fit.
+    instance
+        A manual instance that overwrites the max log likelihood instance in fit (e.g. for drawing the instance
+        randomly from the PDF).
     settings_inversion
         Optionally overwrite the `SettingsInversion` of the `Inversion` object that is created from the fit.
     use_preloaded_grid
         Certain pixelization's construct their mesh in the source-plane from a stochastic KMeans algorithm. This grid
         may be output to hard-disk after the model-fit and loaded via the database to ensure the same grid is used
         as the fit.
     """
     from autogalaxy.interferometer.fit_interferometer import FitInterferometer
 
     dataset_list = _interferometer_from(
         fit=fit,
         real_space_mask=real_space_mask,
-        settings_dataset=settings_dataset,
     )
 
-    plane_list = _plane_from(fit=fit, galaxies=galaxies)
+    galaxies_list = _galaxies_from(fit=fit, instance=instance)
+
+    dataset_model_list = _dataset_model_from(fit=fit, instance=instance)
 
     adapt_images_list = agg_util.adapt_images_from(fit=fit)
 
     settings_inversion = settings_inversion or fit.value(name="settings_inversion")
 
     mesh_grids_of_planes_list = agg_util.mesh_grids_of_planes_list_from(
         fit=fit, total_fits=len(dataset_list), use_preloaded_grid=use_preloaded_grid
     )
 
     fit_dataset_list = []
 
-    for dataset, plane, adapt_images, mesh_grids_of_planes in zip(
-        dataset_list, plane_list, adapt_images_list, mesh_grids_of_planes_list
+    for dataset, galaxies, dataset_model, adapt_images, mesh_grids_of_planes in zip(
+        dataset_list,
+        galaxies_list,
+        dataset_model_list,
+        adapt_images_list,
+        mesh_grids_of_planes_list,
     ):
         preloads = agg_util.preloads_from(
             preloads_cls=Preloads,
             use_preloaded_grid=use_preloaded_grid,
             mesh_grids_of_planes=mesh_grids_of_planes,
             use_w_tilde=False,
         )
 
         fit_dataset_list.append(
             FitInterferometer(
                 dataset=dataset,
-                plane=plane,
+                galaxies=galaxies,
+                dataset_model=dataset_model,
                 adapt_images=adapt_images,
                 settings_inversion=settings_inversion,
                 preloads=preloads,
             )
         )
 
     return fit_dataset_list
 
 
-class FitInterferometerAgg(AbstractAgg):
+class FitInterferometerAgg(af.AggBase):
     def __init__(
         self,
         aggregator: af.Aggregator,
-        settings_dataset: Optional[aa.SettingsInterferometer] = None,
         settings_inversion: Optional[aa.SettingsInversion] = None,
         use_preloaded_grid: bool = True,
         real_space_mask: Optional[aa.Mask2D] = None,
     ):
         """
         Interfaces with an `PyAutoFit` aggregator object to create instances of `FitInterferometer` objects from the
         results of a model-fit.
@@ -139,43 +141,42 @@
 
         This can be done manually, but this object provides a more concise API.
 
         Parameters
         ----------
         aggregator
             A `PyAutoFit` aggregator object which can load the results of model-fits.
-        settings_dataset
-            Optionally overwrite the `SettingsInterferometer` of the `Interferometer` object that is created from the fit.
         settings_inversion
             Optionally overwrite the `SettingsInversion` of the `Inversion` object that is created from the fit.
         use_preloaded_grid
             Certain pixelization's construct their mesh in the source-plane from a stochastic KMeans algorithm. This
             grid may be output to hard-disk after the model-fit and loaded via the database to ensure the same grid is
             used as the fit.
         """
         super().__init__(aggregator=aggregator)
 
-        self.settings_dataset = settings_dataset
         self.settings_inversion = settings_inversion
         self.use_preloaded_grid = use_preloaded_grid
         self.real_space_mask = real_space_mask
 
-    def object_via_gen_from(self, fit, galaxies) -> List[FitInterferometer]:
+    def object_via_gen_from(
+        self, fit, instance: Optional[af.ModelInstance] = None
+    ) -> List[FitInterferometer]:
         """
         Returns a generator of `FitInterferometer` objects from an input aggregator.
 
         See `__init__` for a description of how the `FitInterferometer` objects are created by this method.
 
         Parameters
         ----------
         fit
             A `PyAutoFit` `Fit` object which contains the results of a model-fit as an entry in a sqlite database.
-        galaxies
-            A list of galaxies corresponding to a sample of a non-linear search and model-fit.
+        instance
+            A manual instance that overwrites the max log likelihood instance in fit (e.g. for drawing the instance
+            randomly from the PDF).
         """
         return _fit_interferometer_from(
             fit=fit,
-            galaxies=galaxies,
-            settings_dataset=self.settings_dataset,
+            instance=instance,
             settings_inversion=self.settings_inversion,
             use_preloaded_grid=self.use_preloaded_grid,
         )
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/aggregator/imaging.py` & `autogalaxy-2024.5.16.0/autogalaxy/aggregator/imaging.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from functools import partial
-from typing import List, Optional
+from typing import List
 
 import autofit as af
 import autoarray as aa
 
 
 def _imaging_from(
-    fit: af.Fit, settings_dataset: Optional[aa.SettingsImaging] = None
+    fit: af.Fit,
 ) -> List[aa.Imaging]:
     """
     Returns a list of `Imaging` objects from a `PyAutoFit` sqlite database `Fit` object.
 
     The results of a model-fit can be stored in a sqlite database, including the following attributes of the fit:
 
     - The imaging data as a .fits file (`dataset/data.fits`).
@@ -24,43 +24,42 @@
     This method combines all of these attributes and returns a `Imaging` object, has the mask applied to the
     `Imaging` data structure and its settings updated to the values used by the model-fit.
 
     If multiple `Imaging` objects were fitted simultaneously via analysis summing, the `fit.child_values()` method
     is instead used to load lists of the data, noise-map, PSF and mask and combine them into a list of
     `Imaging` objects.
 
-    The settings can be overwritten by inputting a `settings_dataset` object, for example if you want to use a grid
-    with a different level of sub-griding.
-
     Parameters
     ----------
     fit
         A `PyAutoFit` `Fit` object which contains the results of a model-fit as an entry in a sqlite database.
-    settings_dataset
-        Optionally overwrite the `SettingsImaging` of the `Imaging` object that is created from the fit.
     """
 
     fit_list = [fit] if not fit.children else fit.children
 
     dataset_list = []
 
     for fit in fit_list:
         data = aa.Array2D.from_primary_hdu(primary_hdu=fit.value(name="dataset.data"))
         noise_map = aa.Array2D.from_primary_hdu(
             primary_hdu=fit.value(name="dataset.noise_map")
         )
         psf = aa.Kernel2D.from_primary_hdu(primary_hdu=fit.value(name="dataset.psf"))
 
-        settings_dataset = settings_dataset or fit.value(name="dataset.settings")
+        over_sampling = fit.value(name="dataset.over_sampling")
+        over_sampling_pixelization = fit.value(
+            name="dataset.over_sampling_pixelization"
+        )
 
         dataset = aa.Imaging(
             data=data,
             noise_map=noise_map,
             psf=psf,
-            settings=settings_dataset,
+            over_sampling=over_sampling,
+            over_sampling_pixelization=over_sampling_pixelization,
             check_noise_map=False,
         )
 
         mask = aa.Mask2D.from_primary_hdu(primary_hdu=fit.value(name="dataset.mask"))
 
         dataset = dataset.apply_mask(mask=mask)
 
@@ -103,26 +102,18 @@
         ----------
         aggregator
             A `PyAutoFit` aggregator object which can load the results of model-fits.
         """
         self.aggregator = aggregator
 
     def dataset_gen_from(
-        self, settings_dataset: Optional[aa.SettingsImaging] = None
+        self,
     ) -> List[aa.Imaging]:
         """
         Returns a generator of `Imaging` objects from an input aggregator.
 
         See `__init__` for a description of how the `Imaging` objects are created by this method.
-
-        The settings can be overwritten by inputting a `settings_dataset` object, for example if you want to use a grid
-        with a different level of sub-griding.
-
-        Parameters
-        ----------
-        settings_dataset
-            Optionally overwrite the `SettingsImaging` of the `Imaging` object that is created from the fit.
         """
 
-        func = partial(_imaging_from, settings_dataset=settings_dataset)
+        func = partial(_imaging_from)
 
         return self.aggregator.map(func=func)
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/aggregator/interferometer.py` & `autogalaxy-2024.5.16.0/autogalaxy/aggregator/interferometer.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import autofit as af
 import autoarray as aa
 
 
 def _interferometer_from(
     fit: af.Fit,
     real_space_mask: Optional[aa.Mask2D] = None,
-    settings_dataset: Optional[aa.SettingsInterferometer] = None,
 ) -> List[aa.Interferometer]:
     """
     Returns a list of `Interferometer` objects from a `PyAutoFit` sqlite database `Fit` object.
 
     The results of a model-fit can be stored in a sqlite database, including the following attributes of the fit:
 
     - The interferometer visibilities data as a .fits file (`dataset/data.fits`).
@@ -26,23 +25,18 @@
     This method combines all of these attributes and returns a `Interferometer` object, including having its
     settings updated to the values used by the model-fit.
 
     If multiple `Interferometer` objects were fitted simultaneously via analysis summing, the `fit.child_values()`
     method is instead used to load lists of the data, noise-map, PSF and mask and combine them into a list of
     `Interferometer` objects.
 
-    The settings can be overwritten by inputting a `settings_dataset` object, for example if you want to use a grid
-    with a different level of sub-griding.
-
     Parameters
     ----------
     fit
         A `PyAutoFit` `Fit` object which contains the results of a model-fit as an entry in a sqlite database.
-    settings_dataset
-        Optionally overwrite the `SettingsInterferometer` of the `Interferometer` object that is created from the fit.
     """
 
     fit_list = [fit] if not fit.children else fit.children
 
     dataset_list = []
 
     for fit in fit_list:
@@ -57,25 +51,31 @@
         real_space_mask = (
             real_space_mask
             if real_space_mask is not None
             else aa.Mask2D.from_primary_hdu(
                 primary_hdu=fit.value(name="dataset.real_space_mask")
             )
         )
-        settings_dataset = settings_dataset or fit.value(name="dataset.settings")
+
+        over_sampling = fit.value(name="dataset.over_sampling")
+        over_sampling_pixelization = fit.value(
+            name="dataset.over_sampling_pixelization"
+        )
+        transformer_class = fit.value(name="dataset.transformer_class")
 
         dataset = aa.Interferometer(
             data=data,
             noise_map=noise_map,
             uv_wavelengths=uv_wavelengths,
             real_space_mask=real_space_mask,
+            over_sampling=over_sampling,
+            over_sampling_pixelization=over_sampling_pixelization,
+            transformer_class=transformer_class,
         )
 
-        dataset = dataset.apply_settings(settings=settings_dataset)
-
         dataset_list.append(dataset)
 
     return dataset_list
 
 
 class InterferometerAgg:
     def __init__(self, aggregator: af.Aggregator):
@@ -113,29 +113,24 @@
             A `PyAutoFit` aggregator object which can load the results of model-fits.
         """
         self.aggregator = aggregator
 
     def dataset_gen_from(
         self,
         real_space_mask: Optional[aa.Mask2D] = None,
-        settings_dataset: Optional[aa.SettingsInterferometer] = None,
     ) -> List[aa.Interferometer]:
         """
         Returns a generator of `Interferometer` objects from an input aggregator.
 
         See `__init__` for a description of how the `Interferometer` objects are created by this method.
 
-        The settings can be overwritten by inputting a `settings_dataset` object, for example if you want to use a grid
-        with a different level of sub-griding.
-
         Parameters
         ----------
-        settings_dataset
-            Optionally overwrite the `SettingsInterferometer` of the `Interferometer` object that is created from the fit.
+        real_space_mask
+            The real space mask.
         """
         func = partial(
             _interferometer_from,
             real_space_mask=real_space_mask,
-            settings_dataset=settings_dataset,
         )
 
         return self.aggregator.map(func=func)
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/aggregator/plane.py` & `autogalaxy-2024.5.16.0/autogalaxy/aggregator/galaxies.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,107 +1,117 @@
 from __future__ import annotations
 import logging
-from typing import TYPE_CHECKING, List
+from typing import TYPE_CHECKING, Optional, List
 
 if TYPE_CHECKING:
     from autogalaxy.galaxy.galaxy import Galaxy
-    from autogalaxy.plane.plane import Plane
 
 import autofit as af
 
-from autogalaxy.aggregator.abstract import AbstractAgg
-
-from autogalaxy.aggregator import agg_util
 
 logger = logging.getLogger(__name__)
 
 
-def _plane_from(fit: af.Fit, galaxies: List[Galaxy]) -> List[Plane]:
+def _galaxies_from(fit: af.Fit, instance: af.ModelInstance) -> List[Galaxy]:
     """
-    Returns an `Plane` object from a `PyAutoFit` sqlite database `Fit` object.
+    Returns a list of `Galaxy` objects from a `PyAutoFit` sqlite database `Fit` object.
 
     The results of a model-fit can be stored in a sqlite database, including the following attributes of the fit:
 
     - The model and its best fit parameters (e.g. `model.json`).
     - The adapt images associated with adaptive galaxy features (`adapt` folder).
 
     Each individual attribute can be loaded from the database via the `fit.value()` method.
 
-    This method combines all of these attributes and returns a `Plane` object for a given non-linear search sample
-    (e.g. the maximum likelihood model). This includes associating adapt images with their respective galaxies.
+    This method combines all of these attributes and returns a list of `Galaxy` object for a given non-linear search
+    sample (e.g. the maximum likelihood model). This includes associating adapt images with their respective galaxies.
 
-    If multiple `Plane` objects were fitted simultaneously via analysis summing, the `fit.child_values()` method
-    is instead used to load lists of planes. This is necessary if each plane has different galaxies (e.g. certain
+    If multiple `Galaxy` objects were fitted simultaneously via analysis summing, the `fit.child_values()` method
+    is instead used to load lists of galaxies. This is necessary if each analysis has different galaxies (e.g. certain
     parameters vary across each dataset and `Analysis` object).
 
     Parameters
     ----------
     fit
         A `PyAutoFit` `Fit` object which contains the results of a model-fit as an entry in a sqlite database.
-    galaxies
-        A list of galaxies corresponding to a sample of a non-linear search and model-fit.
+    instance
+        A manual instance that overwrites the max log likelihood instance in fit (e.g. for drawing the instance
+        randomly from the PDF).
     """
 
-    from autogalaxy.plane.plane import Plane
+    if instance is not None:
+        galaxies = instance.galaxies
+
+        if hasattr(instance, "clumps"):
+            galaxies = galaxies + fit.instance.clumps
 
-    if len(fit.children) > 0:
-        logger.info(
-            """
-            Using database for a fit with multiple summed Analysis objects.
+    else:
+        galaxies = fit.instance.galaxies
 
-            Plane objects do not fully support this yet (e.g. variables across Analysis objects may not be correct)
-            so proceed with caution!
-            """
-        )
+        if hasattr(fit.instance, "clumps"):
+            galaxies = galaxies + fit.instance.clumps
 
-        return [Plane(galaxies=galaxies)] * len(fit.children)
+    if fit.children is not None:
+        if len(fit.children) > 0:
+            logger.info(
+                """
+                Using database for a fit with multiple summed Analysis objects.
+    
+                Galaxy objects do not fully support this yet (e.g. variables across Analysis objects may not be correct)
+                so proceed with caution!
+                """
+            )
 
-    return [Plane(galaxies=galaxies)]
+            return [galaxies] * len(fit.children)
 
+    return [galaxies]
 
-class PlaneAgg(AbstractAgg):
+
+class GalaxiesAgg(af.AggBase):
     """
-    Interfaces with an `PyAutoFit` aggregator object to create instances of `Plane` objects from the results
+    Interfaces with an `PyAutoFit` aggregator object to create instances of `Galaxy` objects from the results
     of a model-fit.
 
     The results of a model-fit can be stored in a sqlite database, including the following attributes of the fit:
 
     - The model and its best fit parameters (e.g. `model.json`).
     - The adapt images associated with adaptive galaxy features (`adapt` folder).
 
     The `aggregator` contains the path to each of these files, and they can be loaded individually. This class
-    can load them all at once and create an `Plane` object via the `_plane_from` method.
+    can load them all at once and create lists of `Galaxy` objects via the `_galaxies_from` method.
 
-    This class's methods returns generators which create the instances of the `Plane` objects. This ensures
+    This class's methods returns generators which create the instances of the `Galaxy` objects. This ensures
     that large sets of results can be efficiently loaded from the hard-disk and do not require storing all
-    `Plane` instances in the memory at once.
+    `Galaxy` instances in the memory at once.
 
     For example, if the `aggregator` contains 3 model-fits, this class can be used to create a generator which
-    creates instances of the corresponding 3 `Plane` objects.
+    creates instances of the corresponding 3 `Galaxy` objects.
 
-    If multiple `Plane` objects were fitted simultaneously via analysis summing, the `fit.child_values()` method
-    is instead used to load lists of planes. This is necessary if each plane has different galaxies (e.g. certain
+    If multiple `Galaxy` objects were fitted simultaneously via analysis summing, the `fit.child_values()` method
+    is instead used to load lists of galaxies. This is necessary if each analysis has different galaxies (e.g. certain
     parameters vary across each dataset and `Analysis` object).
 
     This can be done manually, but this object provides a more concise API.
 
     Parameters
     ----------
     aggregator
         A `PyAutoFit` aggregator object which can load the results of model-fits.
     """
 
-    def object_via_gen_from(self, fit, galaxies) -> List[Plane]:
+    def object_via_gen_from(
+        self, fit, instance: Optional[af.ModelInstance] = None
+    ) -> List[Galaxy]:
         """
-        Returns a generator of `Plane` objects from an input aggregator.
+        Returns a generator of `Galaxy` objects from an input aggregator.
 
-        See `__init__` for a description of how the `Plane` objects are created by this method.
+        See `__init__` for a description of how the `Galaxy` objects are created by this method.
 
         Parameters
         ----------
         fit
             A `PyAutoFit` `Fit` object which contains the results of a model-fit as an entry in a sqlite database.
-        galaxies
-            A list of galaxies corresponding to a sample of a non-linear search and model-fit.
+        instance
+            A manual instance that overwrites the max log likelihood instance in fit (e.g. for drawing the instance
+            randomly from the PDF).
         """
-
-        return _plane_from(fit=fit, galaxies=galaxies)
+        return _galaxies_from(fit=fit, instance=instance)
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/analysis/adapt_images.py` & `autogalaxy-2024.5.16.0/autogalaxy/analysis/adapt_images/adapt_images.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,60 +68,72 @@
     def model_image(self) -> aa.Array2D:
         """
         The model-image is the sum of all individual galaxy images in the image dictionary.
 
         This is computed by summing the model-image of each individual adapt galaxy contained in the dictionary.
         """
         adapt_model_image = aa.Array2D(
-            values=np.zeros(self.mask.derive_mask.sub_1.pixels_in_mask),
-            mask=self.mask.derive_mask.sub_1,
+            values=np.zeros(self.mask.pixels_in_mask),
+            mask=self.mask,
         )
 
         try:
             for path in self.galaxy_image_dict.keys():
                 adapt_model_image += self.galaxy_image_dict[path]
         except AttributeError:
             for path in self.galaxy_name_image_dict.keys():
                 adapt_model_image += self.galaxy_name_image_dict[path]
 
         return adapt_model_image
 
     @classmethod
-    def from_result(cls, result) -> "AdaptImages":
+    def from_result(cls, result, use_model_images: bool = False) -> "AdaptImages":
         """
         Returns the adapt-images from a non-linear search result.
 
         For model-fitting, the adapt-images are typically setup using the maximum log likelihood model of the
         previous model-fit. This means the model-fitting is used to cleanly deblend the light of the different
         galaxies in the image (e.g. separate the lens light from the source light).
 
         This method uses attributes of a result (e.g. dictionary mapping galaxy instances to their model-images)
         to create the adapt-images.
 
+        This can use either:
+
+        - The model image of each galaxy in the best-fit model.
+        - The subtracted image of each galaxy in the best-fit model, where the subtracted image is the dataset
+          minus the model images of all other galaxies.
+
         Certain models produce galaxy-images with negative flux values (e.g. a pixelization), which can cause
         numerical issues with the adaptive schemes. To prevent this, we set a minimum flux value for each
         galaxy-image, which is a fraction of the maximum flux value of that image defined via a config file.
 
         Parameters
         ----------
         result
             The result of a previous model-fit, which contains the model-image of each galaxy.
+        use_model_images
+            If True, the model images of the galaxies are used to create the adapt images. If False, the subtracted
+            images of the galaxies are used.
 
         Returns
         -------
         The adapt-images, which are the model-image of each galaxy inferred via the previous model-fit.
         """
         adapt_minimum_percent = conf.instance["general"]["adapt"][
             "adapt_minimum_percent"
         ]
 
         galaxy_name_image_dict = {}
 
         for path, galaxy in result.path_galaxy_tuples:
-            galaxy_image = result.image_galaxy_dict[path]
+            if use_model_images:
+                galaxy_image = result.model_image_galaxy_dict[path]
+            else:
+                galaxy_image = result.subtracted_signal_to_noise_map_galaxy_dict[path]
 
             if not np.all(galaxy_image == 0):
                 minimum_galaxy_value = adapt_minimum_percent * max(galaxy_image)
                 galaxy_image[galaxy_image < minimum_galaxy_value] = minimum_galaxy_value
 
             galaxy_name_image_dict[path] = galaxy_image
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/analysis/chaining_util.py` & `autogalaxy-2024.5.16.0/autogalaxy/analysis/chaining_util.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/analysis/clump_model.py` & `autogalaxy-2024.5.16.0/autogalaxy/analysis/clump_model.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/analysis/maker.py` & `autogalaxy-2024.5.16.0/autogalaxy/analysis/maker.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/analysis/mock/mock_result.py` & `autogalaxy-2024.5.16.0/autogalaxy/analysis/mock/mock_result.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from __future__ import annotations
-from typing import TYPE_CHECKING, Dict
+from typing import TYPE_CHECKING, Dict, List
 
 if TYPE_CHECKING:
     from autogalaxy import mock
 
 import autofit as af
 import autogalaxy as ag
 
@@ -12,24 +12,24 @@
     def __init__(
         self,
         samples: mock.MockSamples = None,
         instance: af.Instance = None,
         model: af.Model = None,
         analysis: mock.MockAnalysis = None,
         search: af.mock.MockSearch = None,
-        max_log_likelihood_plane: ag.Plane = None,
+        max_log_likelihood_galaxies: List[ag.Galaxy] = None,
         max_log_likelihood_tracer=None,
     ):
         super().__init__(
             samples=samples,
             instance=instance,
             model=model,
             analysis=analysis,
             search=search,
         )
 
-        self.max_log_likelihood_plane = max_log_likelihood_plane
+        self.max_log_likelihood_galaxies = max_log_likelihood_galaxies
         self.max_log_likelihood_tracer = max_log_likelihood_tracer
 
     @property
     def last(self):
         return self
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/analysis/preloads.py` & `autogalaxy-2024.5.16.0/autogalaxy/analysis/preloads.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
         if isinstance(fit_0, aa.FitImaging):
             preloads.set_w_tilde_imaging(fit_0=fit_0, fit_1=fit_1)
             preloads.set_blurred_image(fit_0=fit_0, fit_1=fit_1)
 
         preloads.set_mapper_list(fit_0=fit_0, fit_1=fit_1)
 
         if preloads.mapper_list is not None:
-            preloads.mapper_galaxy_dict = fit_0.plane_to_inversion.mapper_galaxy_dict
+            preloads.mapper_galaxy_dict = fit_0.galaxies_to_inversion.mapper_galaxy_dict
 
         preloads.set_operated_mapping_matrix_with_preloads(fit_0=fit_0, fit_1=fit_1)
         preloads.set_linear_func_inversion_dicts(fit_0=fit_0, fit_1=fit_1)
         preloads.set_curvature_matrix(fit_0=fit_0, fit_1=fit_1)
         preloads.set_regularization_matrix_and_term(fit_0=fit_0, fit_1=fit_1)
 
         return preloads
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/analysis/visualizer.py` & `autogalaxy-2024.5.16.0/autogalaxy/analysis/plotter_interface.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 from os import path
 from typing import Dict, List, Union
 
 from autoconf import conf
 import autoarray as aa
 import autoarray.plot as aplt
 
-from autogalaxy.analysis.adapt_images import AdaptImages
+from autogalaxy.analysis.adapt_images.adapt_images import AdaptImages
 from autogalaxy.galaxy.galaxy import Galaxy
+from autogalaxy.galaxy.galaxies import Galaxies
 from autogalaxy.galaxy.plot.galaxy_plotters import GalaxyPlotter
+from autogalaxy.galaxy.plot.galaxies_plotters import GalaxiesPlotter
 from autogalaxy.galaxy.plot.adapt_plotters import AdaptPlotter
-from autogalaxy.plane.plane import Plane
-from autogalaxy.plane.plot.plane_plotters import PlanePlotter
 
 from autogalaxy.plot.include.two_d import Include2D
 from autogalaxy.plot.mat_plot.one_d import MatPlot1D
 from autogalaxy.plot.mat_plot.two_d import MatPlot2D
 
 
 def setting(section: Union[List[str], str], name: str):
@@ -31,44 +31,45 @@
     return conf.instance["visualize"]["plots"][section[0]][name]
 
 
 def plot_setting(section: Union[List[str], str], name: str) -> bool:
     return setting(section, name)
 
 
-class Visualizer:
-    def __init__(self, visualize_path: str):
+class PlotterInterface:
+    def __init__(self, image_path: str):
         """
-        Visualizes a model-fit, including components of the model and fit objects.
+        Provides an interface between an output path and all plotter objects.
 
-        The `Visualizer` is typically used in the `Analysis` class of a non-linear search to visualize the maximum
+        This is used to visualize the results of a model-fit, where the `image_path` points to the
+        folder where the results of the model-fit are stored on your hard-disk, which is typically the `image` folder
+        of a non-linear search.
+
+        The `PlotterInterface` is typically used in the `Analysis` class of a non-linear search to visualize the maximum
         log likelihood model of the model-fit so far.
 
-        The methods of the `Visualizer` are called throughout a non-linear search using the `Analysis`
+        The methods of the `PlotterInterface` are called throughout a non-linear search using the `Analysis.Visualizer`
         classes `visualize` method.
 
-        The images output by the `Visualizer` are customized using the file `config/visualize/plots.ini`.
+        The images output by the `PlotterInterface` are customized using the file `config/visualize/plots.yaml`.
 
         Parameters
         ----------
-        visualize_path
+        image_path
             The path on the hard-disk to the `image` folder of the non-linear searches results.
         """
-        self.visualize_path = visualize_path
+        self.image_path = image_path
 
         self.include_2d = Include2D()
 
-        try:
-            os.makedirs(visualize_path)
-        except FileExistsError:
-            pass
+        os.makedirs(image_path, exist_ok=True)
 
     def mat_plot_1d_from(self, subfolders: str, format: str = "png") -> MatPlot1D:
         """
-        Returns a 1D matplotlib plotting object whose `Output` class uses the `visualizer_path`, such that it outputs
+        Returns a 1D matplotlib plotting object whose `Output` class uses the `image_path`, such that it outputs
         images to the `image` folder of the non-linear search.
 
         Parameters
         ----------
         subfolders
             Subfolders between the `image` folder of the non-linear search and where the images are output. For example,
             images associsted with a fit are output to the subfolder `fit`.
@@ -78,21 +79,21 @@
         Returns
         -------
         MatPlot1D
             The 1D matplotlib plotter object.
         """
         return MatPlot1D(
             output=aplt.Output(
-                path=path.join(self.visualize_path, subfolders), format=format
+                path=path.join(self.image_path, subfolders), format=format
             )
         )
 
     def mat_plot_2d_from(self, subfolders, format="png") -> MatPlot2D:
         """
-        Returns a 2D matplotlib plotting object whose `Output` class uses the `visualizer_path`, such that it outputs
+        Returns a 2D matplotlib plotting object whose `Output` class uses the `image_path`, such that it outputs
         images to the `image` folder of the non-linear search.
 
         Parameters
         ----------
         subfolders
             Subfolders between the `image` folder of the non-linear search and where the images are output. For example,
             images associsted with a fit are output to the subfolder `fit`.
@@ -102,246 +103,158 @@
         Returns
         -------
         MatPlot2D
             The 2D matplotlib plotter object.
         """
         return MatPlot2D(
             output=aplt.Output(
-                path=path.join(self.visualize_path, subfolders), format=format
+                path=path.join(self.image_path, subfolders), format=format
             )
         )
 
-    def visualize_imaging(self, dataset: aa.Imaging):
-        """
-        Visualizes an `Imaging` dataset object.
-
-        Images are output to the `image` folder of the `visualize_path` in a subfolder called `imaging`. When used with
-        a non-linear search the `visualize_path` points to the search's results folder.
-        `.
-        Visualization includes individual images of attributes of the dataset (e.g. the image, noise map, PSF) and a
-        subplot of all these attributes on the same figure.
-
-        The images output by the `Visualizer` are customized using the file `config/visualize/plots.ini` under the
-        [dataset] header.
-
-        Parameters
-        ----------
-        dataset
-            The imaging dataset whose attributes are visualized.
-        """
-
-        def should_plot(name):
-            return plot_setting(section=["dataset", "imaging"], name=name)
-
-        mat_plot_2d = self.mat_plot_2d_from(subfolders="dataset")
-
-        dataset_plotter = aplt.ImagingPlotter(
-            dataset=dataset, mat_plot_2d=mat_plot_2d, include_2d=self.include_2d
-        )
-
-        dataset_plotter.figures_2d(
-            data=should_plot("data"),
-            noise_map=should_plot("noise_map"),
-            psf=should_plot("psf"),
-            signal_to_noise_map=should_plot("signal_to_noise_map"),
-        )
-
-        mat_plot_2d = self.mat_plot_2d_from(subfolders="")
-
-        dataset_plotter = aplt.ImagingPlotter(
-            dataset=dataset, mat_plot_2d=mat_plot_2d, include_2d=self.include_2d
-        )
-
-        if should_plot("subplot_dataset"):
-            dataset_plotter.subplot_dataset()
-
-    def visualize_interferometer(self, dataset: aa.Interferometer):
-        """
-        Visualizes an `Interferometer` dataset object.
-
-        Images are output to the `image` folder of the `visualize_path` in a subfolder called `interferometer`. When
-        used with a non-linear search the `visualize_path` points to the search's results folder.
-
-        Visualization includes individual images of attributes of the dataset (e.g. the visibilities, noise map,
-        uv-wavelengths) and a subplot of all these attributes on the same figure.
-
-        The images output by the `Visualizer` are customized using the file `config/visualize/plots.ini` under the
-        [dataset] header.
-
-        Parameters
-        ----------
-        dataset
-            The interferometer dataset whose attributes are visualized.
-        """
-
-        def should_plot(name):
-            return plot_setting(section=["dataset", "interferometer"], name=name)
-
-        mat_plot_2d = self.mat_plot_2d_from(subfolders="dataset")
-
-        dataset_plotter = aplt.InterferometerPlotter(
-            dataset=dataset,
-            include_2d=self.include_2d,
-            mat_plot_2d=mat_plot_2d,
-        )
-
-        dataset_plotter.figures_2d(
-            data=should_plot("data"),
-            u_wavelengths=should_plot("uv_wavelengths"),
-            v_wavelengths=should_plot("uv_wavelengths"),
-            amplitudes_vs_uv_distances=should_plot("amplitudes_vs_uv_distances"),
-            phases_vs_uv_distances=should_plot("phases_vs_uv_distances"),
-            dirty_image=should_plot("dirty_image"),
-            dirty_noise_map=should_plot("dirty_noise_map"),
-            dirty_signal_to_noise_map=should_plot("dirty_signal_to_noise_map"),
-        )
-
-        mat_plot_2d = self.mat_plot_2d_from(subfolders="")
-
-        dataset_plotter = aplt.InterferometerPlotter(
-            dataset=dataset,
-            include_2d=self.include_2d,
-            mat_plot_2d=mat_plot_2d,
-        )
-
-        if should_plot("subplot_dataset"):
-            dataset_plotter.subplot_dataset()
-
-    def visualize_plane(
-        self, plane: Plane, grid: aa.type.Grid2DLike, during_analysis: bool
+    def galaxies(
+        self, galaxies: List[Galaxy], grid: aa.type.Grid2DLike, during_analysis: bool
     ):
         """
-        Visualizes a `Plane` object.
+        Visualizes a list of galaxies.
 
-        Images are output to the `image` folder of the `visualize_path` in a subfolder called `plane`. When
-        used with a non-linear search the `visualize_path` points to the search's results folder and this function
-        visualizes the maximum log likelihood `Plane` inferred by the search so far.
+        Images are output to the `image` folder of the `image_path` in a subfolder called `galaxies`. When
+        used with a non-linear search the `image_path` points to the search's results folder and this function
+        visualizes the maximum log likelihood galaxies inferred by the search so far.
 
-        Visualization includes individual images of attributes of the plane (e.g. its image, convergence, deflection
+        Visualization includes individual images of attributes of the galaxies (e.g. its image, convergence, deflection
         angles) and a subplot of all these attributes on the same figure.
 
-        The images output by the `Visualizer` are customized using the file `config/visualize/plots.ini` under the
-        [plane] header.
+        The images output by the `PlotterInterface` are customized using the file `config/visualize/plots.yaml` under the
+        [galaxies] header.
 
         Parameters
         ----------
-        plane
-            The maximum log likelihood `Plane` of the non-linear search.
+        galaxies
+            The maximum log likelihood galaxies of the non-linear search.
         grid
             A 2D grid of (y,x) arc-second coordinates used to perform ray-tracing, which is the masked grid tied to
             the dataset.
         during_analysis
             Whether visualization is performed during a non-linear search or once it is completed.
         """
 
+        galaxies = Galaxies(galaxies=galaxies)
+
         def should_plot(name):
-            return plot_setting(section="plane", name=name)
+            return plot_setting(section="galaxies", name=name)
 
-        subfolders = "plane"
+        subfolders = "galaxies"
 
         mat_plot_2d = self.mat_plot_2d_from(subfolders=subfolders)
 
-        plane_plotter = PlanePlotter(
-            plane=plane, grid=grid, mat_plot_2d=mat_plot_2d, include_2d=self.include_2d
+        plotter = GalaxiesPlotter(
+            galaxies=galaxies,
+            grid=grid,
+            mat_plot_2d=mat_plot_2d,
+            include_2d=self.include_2d,
         )
 
         if should_plot("subplot_galaxy_images"):
-            plane_plotter.subplot_galaxy_images()
+            plotter.subplot_galaxy_images()
 
-        plane_plotter.figures_2d(
+        plotter.figures_2d(
             image=should_plot("image"),
             convergence=should_plot("convergence"),
             potential=should_plot("potential"),
             deflections_y=should_plot("deflections"),
             deflections_x=should_plot("deflections"),
             magnification=should_plot("magnification"),
         )
 
         if not during_analysis and should_plot("all_at_end_png"):
             mat_plot_2d = self.mat_plot_2d_from(
                 subfolders=path.join(subfolders, "end"),
             )
 
-            plane_plotter = PlanePlotter(
-                plane=plane,
+            plotter = GalaxiesPlotter(
+                galaxies=galaxies,
                 grid=grid,
                 mat_plot_2d=mat_plot_2d,
                 include_2d=self.include_2d,
             )
 
-            plane_plotter.figures_2d(
+            plotter.figures_2d(
                 image=True,
                 convergence=True,
                 potential=True,
                 deflections_y=True,
                 deflections_x=True,
                 magnification=True,
             )
 
         mat_plot_2d = self.mat_plot_2d_from(subfolders="")
 
-        plane_plotter = PlanePlotter(
-            plane=plane, grid=grid, mat_plot_2d=mat_plot_2d, include_2d=self.include_2d
+        plotter = GalaxiesPlotter(
+            galaxies=galaxies,
+            grid=grid,
+            mat_plot_2d=mat_plot_2d,
+            include_2d=self.include_2d,
         )
 
-        if should_plot("subplot_plane"):
-            plane_plotter.subplot()
+        if should_plot("subplot_galaxies"):
+            plotter.subplot()
 
         if not during_analysis and should_plot("all_at_end_fits"):
             mat_plot_2d = self.mat_plot_2d_from(
                 subfolders=path.join(subfolders, "fits"), format="fits"
             )
 
-            plane_plotter = PlanePlotter(
-                plane=plane,
+            plotter = GalaxiesPlotter(
+                galaxies=galaxies,
                 grid=grid,
                 mat_plot_2d=mat_plot_2d,
                 include_2d=self.include_2d,
             )
 
-            plane_plotter.figures_2d(
+            plotter.figures_2d(
                 image=True,
                 convergence=True,
                 potential=True,
                 deflections_y=True,
                 deflections_x=True,
                 magnification=True,
             )
 
-    def visualize_galaxies(
+    def galaxies_1d(
         self, galaxies: [List[Galaxy]], grid: aa.type.Grid2DLike, during_analysis: bool
     ):
         """
         Visualizes a list of `Galaxy` objects.
 
-        Images are output to the `image` folder of the `visualize_path` in a subfolder called `galaxies`. When
-        used with a non-linear search the `visualize_path` points to the search's results folder and this function
+        Images are output to the `image` folder of the `image_path` in a subfolder called `galaxies`. When
+        used with a non-linear search the `image_path` points to the search's results folder and this function
         visualizes the maximum log likelihood `Galaxy`'s inferred by the search so far.
 
         Visualization includes individual images of attributes of each galaxy (e.g. 1D plots of their image,
         convergence) and a subplot of all these attributes on the same figure.
 
-        The images output by the `Visualizer` are customized using the file `config/visualize/plots.ini` under the
+        The images output by the `PlotterInterface` are customized using the file `config/visualize/plots.yaml` under the
         [galaxies] header.
 
         Parameters
         ----------
         galaxies
             A list of the maximum log likelihood `Galaxy`'s of the non-linear search.
         grid
             A 2D grid of (y,x) arc-second coordinates used to perform ray-tracing, which is the masked grid tied to
             the dataset.
         during_analysis
             Whether visualization is performed during a non-linear search or once it is completed.
         """
 
         def should_plot(name):
-            return plot_setting(section="galaxies", name=name)
+            return plot_setting(section="galaxies_1d", name=name)
 
-        mat_plot_1d = self.mat_plot_1d_from(subfolders="galaxies")
+        mat_plot_1d = self.mat_plot_1d_from(subfolders="galaxies_1d")
 
         for galaxy in galaxies:
             galaxy_plotter = GalaxyPlotter(
                 galaxy=galaxy,
                 grid=grid,
                 mat_plot_1d=mat_plot_1d,
                 include_2d=self.include_2d,
@@ -352,26 +265,26 @@
                     image=should_plot("image"),
                     convergence=should_plot("convergence"),
                     potential=should_plot("potential"),
                 )
             except OverflowError:
                 pass
 
-    def visualize_inversion(self, inversion: aa.Inversion, during_analysis: bool):
+    def inversion(self, inversion: aa.Inversion, during_analysis: bool):
         """
         Visualizes an `Inversion` object.
 
-        Images are output to the `image` folder of the `visualize_path` in a subfolder called `inversion`. When
-        used with a non-linear search the `visualize_path` points to the search's results folder and this function
+        Images are output to the `image` folder of the `image_path` in a subfolder called `inversion`. When
+        used with a non-linear search the `image_path` points to the search's results folder and this function
         visualizes the maximum log likelihood `Inversion` inferred by the search so far.
 
         Visualization includes individual images of attributes of the dataset (e.g. the reconstructed image, the
         reconstruction) and a subplot of all these attributes on the same figure.
 
-        The images output by the `Visualizer` are customized using the file `config/visualize/plots.ini` under the
+        The images output by the `PlotterInterface` are customized using the file `config/visualize/plots.yaml` under the
         [inversion] header.
 
         Parameters
         ----------
         inversion
             The inversion used to fit the dataset whose attributes are visualized.
         during_analysis
@@ -448,28 +361,28 @@
                 reconstructed_image=True,
                 reconstruction=True,
                 errors=True,
                 regularization_weights=True,
                 interpolate_to_uniform=True,
             )
 
-    def visualize_adapt_images(
+    def adapt_images(
         self,
         adapt_images: AdaptImages,
     ):
         """
         Visualizes the adapt images used by a model-fit for adaptive pixelization mesh's and regularization.
 
-        Images are output to the `image` folder of the `visualize_path` in a subfolder called `adapt`. When
-        used with a non-linear search the `visualize_path` points to the search's results folder.
+        Images are output to the `image` folder of the `image_path` in a subfolder called `adapt`. When
+        used with a non-linear search the `image_path` points to the search's results folder.
 
         Visualization includes an image of the overall adapt model image and a subplot of all galaxy images on the same
         figure.
 
-        The images output by the `Visualizer` are customized using the file `config/visualize/plots.ini` under the
+        The images output by the `PlotterInterface` are customized using the file `config/visualize/plots.yaml` under the
         [adapt] header.
 
         Parameters
         ----------
         adapt_images
             The adapt images (e.g. overall model image, individual galaxy images).
         """
@@ -486,43 +399,7 @@
         if should_plot("model_image"):
             adapt_plotter.figure_model_image(model_image=adapt_images.model_image)
 
         if should_plot("images_of_galaxies"):
             adapt_plotter.subplot_images_of_galaxies(
                 adapt_galaxy_name_image_dict=adapt_images.galaxy_image_dict
             )
-
-    def visualize_contribution_maps(self, plane: Plane):
-        """
-        Visualizes the contribution maps that are used for adapt features which adapt a model to the dataset it is
-        fitting.
-
-        Images are output to the `image` folder of the `visualize_path` in a subfolder called `adapt`. When
-        used with a non-linear search the `visualize_path` points to the search's results folder and this function
-        visualizes the maximum log likelihood contribution maps inferred by the search so far.
-
-        Visualization includes individual images of attributes of the adapt image (e.g. the contribution map of
-        each galaxy) and a subplot of all contribution maps on the same figure.
-
-        The images output by the `Visualizer` are customized using the file `config/visualize/plots.ini` under the
-        [adapt] header.
-
-        Parameters
-        ----------
-        plane
-            The maximum log likelihood `Plane` of the non-linear search which is used to plot the contribution maps.
-        """
-
-        def should_plot(name):
-            return plot_setting(section="adapt", name=name)
-
-        mat_plot_2d = self.mat_plot_2d_from(subfolders="adapt")
-
-        adapt_plotter = AdaptPlotter(
-            mat_plot_2d=mat_plot_2d, include_2d=self.include_2d
-        )
-
-        if hasattr(plane, "contribution_map_list"):
-            if should_plot("contribution_map_list"):
-                adapt_plotter.subplot_contribution_map_list(
-                    contribution_map_list_list=plane.contribution_map_list
-                )
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/README.rst` & `autogalaxy-2024.5.16.0/autogalaxy/config/README.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/general.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/general.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -4,14 +4,13 @@
   flip_for_ds9: true
 grid:
   max_evaluation_grid_size: 1000   # An evaluation grid whose shape is adaptive chosen is used to compute quantities like critical curves, this integer is the max size of the grid ensuring faster run times.
 adapt:
   adapt_minimum_percent: 0.01
   adapt_noise_limit: 100000000.0
 inversion:
-  relocate_pix_border: true          # If True, by default a pixelization's border is used to relocate all pixels outside its border to the border.
+  use_border_relocator: true          # If True, by default a pixelization's border is used to relocate all pixels outside its border to the border.
 test:
-  check_figure_of_merit_sanity: false
-  bypass_figure_of_merit_sanity: false
+  check_likelihood_function: true   # if True, when a search is resumed the likelihood of a previous sample is recalculated to ensure it is consistent with the previous run.
   check_preloads: false
   exception_override: false
   preloads_check_threshold: 1.0     # If the figure of merit of a fit with and without preloads is greater than this threshold, the check preload test fails and an exception raised for a model-fit.
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/grids.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/grids.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     ExponentialCoreSph: 1.0e-06
     ExponentialSph: 1.0e-06
     ExternalShear: 1.0e-08
     Gaussian: 1.0e-08
     GaussianSph: 1.0e-08
     gNFW: 1.0e-06
     gNFWMCRLudlow: 1.0e-06
+    gNFWVirialMassConcSph: 1.0e-06
     gNFWSph: 1.0e-06
     Isothermal: 1.0e-08
     IsothermalCore: 1.0e-08
     IsothermalCoreSph: 1.0e-08
     IsothermalSph: 1.0e-08
     MassSheet: 1.0e-08
     Moffat: 1.0e-08
@@ -49,16 +50,16 @@
     PowerLawSph: 1.0e-08
     Sersic: 1.0e-06
     SersicCore: 1.0e-06
     SersicCoreSph: 1.0e-06
     SersicRadialGradient: 1.0e-06
     SersicSph: 1.0e-06
     SersicRadialGradientSph: 1.0e-06
+    ShapeletCartesianSph: 1.0e-8
     ShapeletCartesian: 1.0e-8
-    ShapeletCartesianEll: 1.0e-8
+    ShapeletPolarSph: 1.0e-8
     ShapeletPolar: 1.0e-8
-    ShapeletPolarEll: 1.0e-8
+    ShapeletExponentialSph: 1.0e-8
     ShapeletExponential: 1.0e-8
-    ShapeletExponentialEll: 1.0e-8
     SMBH: 1.0e-8
     SMBHBinary: 1.0e-8
     EllProfile: 1.0e-08
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/notation.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/notation.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
     angle_binary: \theta
     beta: \beta
     break_radius: \theta_{\rm B}
     centre_0: y
     centre_1: x
     coefficient: \lambda
     concentration: conc
-    contribution_factor: \omega_{\rm 0}
     core_radius: C_{\rm r}
     core_radius_0: C_{rm r0}
     core_radius_1: C_{\rm r1}
     effective_radius: R_{\rm eff}
     einstein_radius: \theta_{\rm Ein}
     ell_comps_0: \epsilon_{\rm 1}
     ell_comps_1: \epsilon_{\rm 2}
@@ -76,15 +75,14 @@
     angle_binary: '{:.4f}'
     angular_diameter_distance_to_earth: '{:.4f}'
     beta: '{:.4f}'
     centre_0: '{:.4f}'
     centre_1: '{:.4f}'
     coefficient: '{:.4f}'
     concentration: '{:.4f}'
-    contribution_factor: '{:.4f}'
     core_radius: '{:.4f}'
     core_radius_0: '{:.4f}'
     core_radius_1: '{:.4f}'
     effective_radius: '{:.4f}'
     einstein_mass: '{:.4e}'
     einstein_radius: '{:.4f}'
     ell_comps_0: '{:.4f}'
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/README.rst` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/README.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/cosmology.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/cosmology.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/image_mesh/hilbert.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/image_mesh/hilbert.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/image_mesh/hilbert_balanced.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/image_mesh/kmeans.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,31 @@
-HilbertBalanced:
+KMeans:
   pixels:
     type: Uniform
     lower_limit: 50.0
     upper_limit: 2500.0
     width_modifier:
       type: Absolute
       value: 100.0
     gaussian_limits:
       lower: 50.0
       upper: inf
   weight_floor:
-    type: Uniform
-    lower_limit: 0.0
-    upper_limit: 0.005
+    type: LogUniform
+    lower_limit: 0.00001
+    upper_limit: 1.0
     width_modifier:
       type: Absolute
       value: 0.1
     gaussian_limits:
       lower: 0.0
       upper: inf
   weight_power:
     type: Uniform
-    lower_limit: 2.5
-    upper_limit: 4.0
+    lower_limit: 0.0
+    upper_limit: 5.0
     width_modifier:
       type: Absolute
       value: 5.0
     gaussian_limits:
       lower: 0.0
-      upper: inf
-  ratio:
-    type: Constant
-    value: 0.2
+      upper: inf
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/image_mesh/kmeans.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/regularization/matern_kernel.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-KMeans:
-  pixels:
-    type: Uniform
-    lower_limit: 50.0
-    upper_limit: 2500.0
+MaternKernel:
+  coefficient:
+    type: LogUniform
+    lower_limit: 1.0e-06
+    upper_limit: 1000000.0
     width_modifier:
-      type: Absolute
-      value: 100.0
+      type: Relative
+      value: 0.5
     gaussian_limits:
-      lower: 50.0
+      lower: 0.0
       upper: inf
-  weight_floor:
+  scale:
     type: LogUniform
-    lower_limit: 0.00001
-    upper_limit: 1.0
+    lower_limit: 1.0e-06
+    upper_limit: 1000000.0
     width_modifier:
-      type: Absolute
-      value: 0.1
+      type: Relative
+      value: 0.2
     gaussian_limits:
       lower: 0.0
       upper: inf
-  weight_power:
+  nu:
     type: Uniform
-    lower_limit: 0.0
-    upper_limit: 5.0
+    lower_limit: 0.5
+    upper_limit: 5.5
     width_modifier:
-      type: Absolute
-      value: 5.0
+      type: Relative
+      value: 0.2
     gaussian_limits:
       lower: 0.0
-      upper: inf
+      upper: inf
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/README.rst` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The ``light`` folder contains configuration files for the default priors assumed for light profiles in **PyAutoGalaxy** (e.g. ``Sersic``, ``Gaussian``).
 
 Folders
 -------
 
 - ``standard``: Configs for standard light profiles (specified via ``ag.lp.``), which include an ``intensity`` parameter to control their overall amount of emission.
 - ``linear``: Configs for linear light profiles (specified via ``ag.lp_linear.``),, where the ``intensity`` parameter is implicitly solved for via linear algebra.
-- ``shapelets``: Configs for shapelets (specified via ``ag.lp_shapelets.``), which decomposed the light of a galaxy via shapelet basis functions.
+- ``shapelets``: Configs for shapelets (specified via ``ag.lp_linear.``), which decomposed the light of a galaxy via shapelet basis functions.
 - ``operated``: Configs for operated light profiles (specified via ``ag.lp_operated.``), where the light profile represents the already PSF convolved emission.
 - ``linear_operated``: Configs for linear operated light profiles (specified via ``ag.lp_linear_operated.``), which behave like operated light profiles but with a linearly solved for ``intensity``.
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/linear/chameleon.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/linear/chameleon.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/linear/dev_vaucouleurs.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/linear/dev_vaucouleurs.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/linear/eff.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/linear/eff.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/linear/exponential.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/linear/exponential.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/linear/exponential_core.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/linear/exponential_core.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/linear/gaussian.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/linear/gaussian.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/linear/moffat.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/linear/moffat.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/linear/sersic.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/linear/sersic.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/linear/sersic_core.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/linear/sersic_core.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/linear_operated/gaussian.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/linear_operated/gaussian.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/linear_operated/moffat.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/linear_operated/moffat.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/operated/gaussian.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/operated/gaussian.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/operated/moffat.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/operated/moffat.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/operated/sersic.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/operated/sersic.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/shapelets/cartesian.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/linear/shapelets/polar.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-ShapeletCartesian:
+ShapeletPolarSph:
   centre_0:
     type: Gaussian
     mean: 0.0
     sigma: 0.3
     lower_limit: -inf
     upper_limit: inf
     width_modifier:
@@ -29,15 +29,15 @@
     upper_limit: 30.0
     width_modifier:
       type: Relative
       value: 0.5
     gaussian_limits:
       lower: 0.0
       upper: inf
-ShapeletCartesianEll:
+ShapeletPolar:
   centre_0:
     type: Gaussian
     mean: 0.0
     sigma: 0.3
     lower_limit: -inf
     upper_limit: inf
     width_modifier:
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/shapelets/exponential.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/linear/shapelets/exponential.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-ShapeletExponential:
+ShapeletExponentialSph:
   centre_0:
     type: Gaussian
     mean: 0.0
     sigma: 0.3
     lower_limit: -inf
     upper_limit: inf
     width_modifier:
@@ -29,15 +29,15 @@
     upper_limit: 30.0
     width_modifier:
       type: Relative
       value: 0.5
     gaussian_limits:
       lower: 0.0
       upper: inf
-ShapeletExponentialEll:
+ShapeletExponential:
   centre_0:
     type: Gaussian
     mean: 0.0
     sigma: 0.3
     lower_limit: -inf
     upper_limit: inf
     width_modifier:
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/shapelets/polar.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/linear/shapelets/cartesian.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-ShapeletPolar:
+ShapeletCartesianSph:
   centre_0:
     type: Gaussian
     mean: 0.0
     sigma: 0.3
     lower_limit: -inf
     upper_limit: inf
     width_modifier:
@@ -29,15 +29,15 @@
     upper_limit: 30.0
     width_modifier:
       type: Relative
       value: 0.5
     gaussian_limits:
       lower: 0.0
       upper: inf
-ShapeletPolarEll:
+ShapeletCartesian:
   centre_0:
     type: Gaussian
     mean: 0.0
     sigma: 0.3
     lower_limit: -inf
     upper_limit: inf
     width_modifier:
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/standard/chameleon.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/standard/chameleon.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/standard/dev_vaucouleurs.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/standard/dev_vaucouleurs.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/standard/eff.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/standard/eff.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/standard/exponential.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/standard/exponential.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/standard/exponential_core.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/standard/exponential_core.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/standard/gaussian.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/standard/gaussian.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/standard/moffat.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/standard/moffat.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/standard/sersic.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/standard/sersic.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/light/standard/sersic_core.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/light/standard/sersic_core.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/README.rst` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/README.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/dark/gnfw.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/dark/gnfw.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/dark/gnfw_mcr.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/dark/gnfw_mcr.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/dark/nfw.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/dark/nfw.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/dark/nfw_mcr.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/dark/nfw_mcr.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/dark/nfw_mcr_scatter.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/dark/nfw_mcr_scatter.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/dark/nfw_truncated.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/dark/nfw_truncated.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/dark/nfw_truncated_mcr.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/dark/nfw_truncated_mcr.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/dark/nfw_virial_mass_conc.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/dark/nfw_virial_mass_conc.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/point/point.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/point/point.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/point/smbh.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/point/smbh.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/point/smbh_binary.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/point/smbh_binary.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/sheets/mass_sheet.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/sheets/mass_sheet.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/stellar/chameleon.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/stellar/chameleon.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/stellar/dev_vaucouleurs.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/stellar/dev_vaucouleurs.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/stellar/exponential.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/stellar/exponential.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/stellar/gaussian.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/stellar/gaussian.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/stellar/sersic.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/stellar/sersic.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/stellar/sersic_core.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/stellar/sersic_core.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/stellar/sersic_radial_gradient.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/stellar/sersic_radial_gradient.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/total/isothermal.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/total/isothermal.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/total/isothermal_core.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/total/isothermal_core.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/total/power_law.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/total/power_law.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/total/power_law_broken.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/total/power_law_broken.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/total/power_law_core.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/total/power_law_core.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/mass/total/power_law_multipole.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/mass/total/power_law_multipole.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/point_sources.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/point_sources.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/regularization/adaptive_brightness.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/regularization/adaptive_brightness.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/priors/regularization/adaptive_brightness_split_zeroth.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/priors/regularization/adaptive_brightness_split_zeroth.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/visualize/README.rst` & `autogalaxy-2024.5.16.0/autogalaxy/config/visualize/README.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/visualize/mat_wrap_2d.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/visualize/mat_wrap_2d.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/config/visualize/plots.yaml` & `autogalaxy-2024.5.16.0/autogalaxy/config/visualize/plots.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -25,44 +25,45 @@
   model_data: false                        # Plot individual plots of the model-data?
   residual_map: false                      # Plot individual plots of the residual-map?
   normalized_residual_map: false           # Plot individual plots of the normalized-residual-map?
   chi_squared_map: false                   # Plot individual plots of the chi-squared-map?
   residual_flux_fraction: false            # Plot individual plots of the residual_flux_fraction?
   model_images_of_galaxies: false          # Plot individual plots of each galaxy's model image?
 fit_imaging: {}                            # Settings for plots of fits to imaging datasets (e.g. FitImagingPlotter).
-plane:                                     # Settings for plots of planes (e.g. PlanePlotter).
-  subplot_plane: true                      # Plot subplot of all quantities in each plane (e.g. images, convergence)?
+galaxies:                                  # Settings for plots of galaxies (e.g. GalaxiesPlotter).
+  subplot_galaxies: true                   # Plot subplot of all quantities in each galaxies group (e.g. images, convergence)?
   all_at_end_png: true                     # Plot all individual plots listed below as .png (even if False)?
   all_at_end_fits: true                    # Plot all individual plots listed below as .fits (even if False)?
   all_at_end_pdf: false                    # Plot all individual plots listed below as publication-quality .pdf (even if False)?
   subplot_galaxy_images: false             # Plot subplot of the image of each galaxy in the model?
   image: false
   source_plane_image: false
   convergence: false
   deflections: false
   potential: false
   magnification: false
-galaxies:                                  # Settings for plots of galaxies (e.g GalaxyPlotter).
+galaxies_1d:                                  # Settings for 1D plots of galaxies (e.g. GalaxiesPlotter).
   image: false
   convergence: false
   potential: false
 inversion:                                 # Settings for plots of inversions (e.g. InversionPlotter).
   subplot_inversion: true                  # Plot subplot of all quantities in each inversion (e.g. reconstrucuted image, reconstruction)?
+  subplot_mappings: true                   # Plot subplot of the image-to-source pixels mappings of each pixelization?
   all_at_end_png: true                     # Plot all individual plots listed below as .png (even if False)?
   all_at_end_fits: true                    # Plot all individual plots listed below as .fits (even if False)?
   all_at_end_pdf: false                    # Plot all individual plots listed below as publication-quality .pdf (even if False)?
   data_subtracted: false                   # Plot individual plots of the data with the other inversion linear objects subtracted?
   errors: false                            # Plot image of the errors of every mesh-pixel reconstructed value?
-  mesh_pixels_per_image_pixels : false     # Plot the number of image-plane mesh pixels per masked data pixels?
+  sub_pixels_per_image_pixels: false      # Plot the number of sub pixels per masked data pixels?
+  mesh_pixels_per_image_pixels: false     # Plot the number of image-plane mesh pixels per masked data pixels?
   reconstructed_image: false               # Plot image of the reconstructed data (e.g. in the image-plane)?
   reconstruction: false                    # Plot the reconstructed inversion (e.g. the pixelization's mesh in the source-plane)?
   regularization_weights: false            # Plot the effective regularization weight of every inversion mesh pixel?
 adapt:                                     # Settings for plots of adapt images used by adaptive pixelizations.
   images_of_galaxies: true
-  contribution_map_list: true
   model_image: true
 interferometer:                            # Settings for plots of interferometer datasets (e.g. InterferometerPlotter).
   amplitudes_vs_uv_distances: false
   phases_vs_uv_distances: false
   uv_wavelengths: false
   dirty_image: false
   dirty_noise_map: false
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/convert.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/light/snr/chameleon.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,114 +1,83 @@
-import numpy as np
 from typing import Tuple
 
+from autogalaxy.profiles.light.snr.abstract import LightProfileSNR
 
-def ell_comps_from(axis_ratio, angle):
-    """
-    Convert an input axis ratio (0.0 > q > 1.0) and rotation position angle defined counter clockwise from the
-    positive x-axis(0.0 > angle > 180) to the (y,x) ellipitical components e1 and e2.
-
-    Parameters
-    ----------
-    axis_ratio
-        Ratio of light profiles ellipse's minor and major axes (b/a).
-    angle
-        Rotation angle of light profile counter-clockwise from positive x-axis.
-    """
-    angle *= np.pi / 180.0
-    fac = (1 - axis_ratio) / (1 + axis_ratio)
-    ellip_y = fac * np.sin(2 * angle)
-    ellip_x = fac * np.cos(2 * angle)
-    return (ellip_y, ellip_x)
-
-
-def axis_ratio_and_angle_from(ell_comps):
-    """
-    Convert the ellipitical components e1 and e2 to an axis ratio (0.0 > q > 1.0) and rotation position angle
-    defined counter clockwise from the positive x-axis(0.0 > angle > 180) to .
-
-    Parameters
-    ----------
-    ell_comps : (float, float)
-        The first and second ellipticity components of the elliptical coordinate system.
-    """
-    angle = np.arctan2(ell_comps[0], ell_comps[1]) / 2
-    angle *= 180.0 / np.pi
-    fac = np.sqrt(ell_comps[1] ** 2 + ell_comps[0] ** 2)
-    if fac > 0.999:
-        fac = 0.999  # avoid unphysical solution
-    # if fac > 1: print('unphysical e1,e2')
-    axis_ratio = (1 - fac) / (1 + fac)
-    return axis_ratio, angle
-
-
-def axis_ratio_from(ell_comps):
-    """
-    Convert the ellipitical components e1 and e2 to an axis ratio (0.0 > q > 1.0) and rotation position angle
-    defined counter clockwise from the positive x-axis(0.0 > angle > 180) to .
-
-    Parameters
-    ----------
-    ell_comps : (float, float)
-        The first and second ellipticity components of the elliptical coordinate system.
-    """
-    axis_ratio, angle = axis_ratio_and_angle_from(ell_comps=ell_comps)
-    return axis_ratio
-
-
-def angle_from(ell_comps):
-    """
-    Convert the ellipitical components e1 and e2 to an rotation position angle in degrees (0.0 > angle > 18-.0).
-
-    Parameters
-    ----------
-    ell_comps : (float, float)
-        The first and second ellipticity components of the elliptical coordinate system.
-    """
-    axis_ratio, angle = axis_ratio_and_angle_from(ell_comps=ell_comps)
-    return angle
-
-
-def shear_gamma_1_2_from(magnitude: float, angle: float) -> Tuple[float, float]:
-    """
-    :param angle: angel
-    :param magnitude: ellipticity
-    :return:
-    """
-    gamma_1 = magnitude * np.cos(2 * angle * np.pi / 180.0)
-    gamma_2 = magnitude * np.sin(2 * angle * np.pi / 180.0)
-    return (gamma_1, gamma_2)
-
-
-def shear_magnitude_and_angle_from(
-    gamma_1: float, gamma_2: float
-) -> Tuple[float, float]:
-    """
-    :param e1: ellipticity component
-    :param e2: ellipticity component
-    :return: angle and abs value of ellipticity
-    """
-    angle = np.arctan2(gamma_2, gamma_1) / 2 * 180.0 / np.pi
-    magnitude = np.sqrt(gamma_1**2 + gamma_2**2)
-    if angle < 0:
-        return magnitude, angle + 180.0
-    return magnitude, angle
-
-
-def shear_magnitude_from(gamma_1: float, gamma_2: float) -> float:
-    """
-    :param e1: ellipticity component
-    :param e2: ellipticity component
-    :return: angle and abs value of ellipticity
-    """
-    magnitude, angle = shear_magnitude_and_angle_from(gamma_1=gamma_1, gamma_2=gamma_2)
-    return magnitude
-
-
-def shear_angle_from(gamma_1: float, gamma_2: float) -> float:
-    """
-    :param e1: ellipticity component
-    :param e2: ellipticity component
-    :return: angle and abs value of ellipticity
-    """
-    magnitude, angle = shear_magnitude_and_angle_from(gamma_1=gamma_1, gamma_2=gamma_2)
-    return angle
+from autogalaxy.profiles.light import standard as lp
+
+
+class Chameleon(lp.Chameleon, LightProfileSNR):
+    def __init__(
+        self,
+        signal_to_noise_ratio: float = 10.0,
+        centre: Tuple[float, float] = (0.0, 0.0),
+        ell_comps: Tuple[float, float] = (0.0, 0.0),
+        core_radius_0: float = 0.01,
+        core_radius_1: float = 0.05,
+    ):
+        """
+        The elliptical Chameleon light profile.
+
+        Profile form:
+            mass_to_light_ratio * intensity *\
+                (1.0 / Sqrt(x^2 + (y/q)^2 + rc^2) - 1.0 / Sqrt(x^2 + (y/q)^2 + (rc + dr)**2.0))
+
+        Parameters
+        ----------
+        centre
+            The (y,x) arc-second coordinates of the profile centre.
+        ell_comps
+            The first and second ellipticity components of the elliptical coordinate system.
+        intensity
+            Overall intensity normalisation of the light profile (units are dimensionless and derived from the data
+            the light profile's image is compared too, which is expected to be electrons per second).
+        core_radius_0 : the core size of the first elliptical cored Isothermal profile.
+        core_radius_1 : rc + dr is the core size of the second elliptical cored Isothermal profile.
+             We use dr here is to avoid negative values.
+        """
+
+        super().__init__(
+            centre=centre,
+            ell_comps=ell_comps,
+            intensity=0.0,
+            core_radius_0=core_radius_0,
+            core_radius_1=core_radius_1,
+        )
+        LightProfileSNR.__init__(self, signal_to_noise_ratio=signal_to_noise_ratio)
+
+
+class ChameleonSph(lp.ChameleonSph, LightProfileSNR):
+    def __init__(
+        self,
+        signal_to_noise_ratio: float = 10.0,
+        centre: Tuple[float, float] = (0.0, 0.0),
+        core_radius_0: float = 0.01,
+        core_radius_1: float = 0.05,
+    ):
+        """
+        The spherical Chameleon light profile.
+
+        Profile form:
+            mass_to_light_ratio * intensity *\
+                (1.0 / Sqrt(x^2 + (y/q)^2 + rc^2) - 1.0 / Sqrt(x^2 + (y/q)^2 + (rc + dr)**2.0))
+
+        Parameters
+        ----------
+        centre
+            The (y,x) arc-second coordinates of the profile centre.
+        ell_comps
+            The first and second ellipticity components of the elliptical coordinate system.
+        intensity
+            Overall intensity normalisation of the light profile (units are dimensionless and derived from the data
+            the light profile's image is compared too, which is expected to be electrons per second).
+        core_radius_0 : the core size of the first elliptical cored Isothermal profile.
+        core_radius_1 : rc + dr is the core size of the second elliptical cored Isothermal profile.
+             We use dr here is to avoid negative values.
+        """
+
+        super().__init__(
+            centre=centre,
+            intensity=0.0,
+            core_radius_0=core_radius_0,
+            core_radius_1=core_radius_1,
+        )
+        LightProfileSNR.__init__(self, signal_to_noise_ratio=signal_to_noise_ratio)
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/cosmology/lensing.py` & `autogalaxy-2024.5.16.0/autogalaxy/cosmology/lensing.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/cosmology/model.py` & `autogalaxy-2024.5.16.0/autogalaxy/cosmology/model.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/cosmology/wrap.py` & `autogalaxy-2024.5.16.0/autogalaxy/cosmology/wrap.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/exc.py` & `autogalaxy-2024.5.16.0/autogalaxy/exc.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,25 +20,14 @@
     For example if stellar-mass specific calculations are used for a galaxy which does not have a stellar mas
     component.
     """
 
     pass
 
 
-class PlaneException(Exception):
-    """
-    Raises exceptions associated with the `plane` module and `Galaxy` class.
-
-    For example if no galaxies or redshifts are input into a plane, such that the plane does not know its redshift
-    relative to other planes.
-    """
-
-    pass
-
-
 class AnalysisException(Exception):
     """
     Raises exceptions associated with the `analysis` modules in the `model` packages and `Analysis` classes.
 
     For example if the figure of merit of the analysis class's `log_likelihood_function` has changed for a resumed
     run from a previous run.
     """
@@ -102,20 +91,20 @@
         using the solved for intensities. 
         
         If you are using PyAutoLens, you should use the attribute
         `fit.tracer_linear_light_profiles_to_light_profiles` to access a 
         `Tracer` with these converted light profiles.
 
         If you are using PyAutoGalaxy, you should instead use
-        `fit.plane_linear_light_profiles_to_light_profiles` to access a
-        `Plane` with these converted light profiles.
+        `fit.galaxies_linear_light_profiles_to_light_profiles` to access
+        `Galaxy` objects with these converted light profiles.
              
         If you are using database functionality and creating tracers
-        via the `TracerAgg` object or `PlaneAgg` object, you should 
+        via the `TracerAgg` object or `GalaxiesAgg` object, you should 
         instead use the `FitImagingAgg` object to create `FitImaging` 
         objects.
         
         You should then access what you need via 
         `fit.tracer_linear_light_profiles_to_light_profiles` or
-        `fit.plane_linear_light_profiles_to_light_profiles`.
+        `fit.galaxies_linear_light_profiles_to_light_profiles`.
         """
     )
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/fixtures.py` & `autogalaxy-2024.5.16.0/autogalaxy/fixtures.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from autoarray.fixtures import *
 
+import autofit as af
 import autogalaxy as ag
 import autogalaxy.plot as aplt
 
 
 def make_masked_imaging_7x7():
     imaging_7x7 = make_imaging_7x7()
 
-    masked_imaging_7x7 = imaging_7x7.apply_mask(mask=make_sub_mask_2d_7x7())
+    return imaging_7x7.apply_mask(mask=make_mask_2d_7x7())
 
-    return masked_imaging_7x7.apply_settings(settings=ag.SettingsImaging(sub_size=1))
+
+def make_masked_imaging_7x7_sub_2():
+    imaging_7x7 = make_imaging_7x7_sub_2()
+
+    return imaging_7x7.apply_mask(mask=make_mask_2d_7x7())
 
 
 def make_masked_imaging_covariance_7x7():
     imaging_7x7 = make_imaging_covariance_7x7()
 
-    masked_imaging_7x7 = imaging_7x7.apply_mask(mask=make_sub_mask_2d_7x7())
-
-    return masked_imaging_7x7.apply_settings(settings=ag.SettingsImaging(sub_size=1))
+    return imaging_7x7.apply_mask(mask=make_mask_2d_7x7())
 
 
 # PROFILES #
 
 
 def make_ps_0():
     # noinspection PyTypeChecker
@@ -112,33 +115,33 @@
 
 def make_gal_x1_lp_x1_mp():
     return ag.Galaxy(
         redshift=0.5, light_profile_0=make_lp_0(), mass_profile_0=make_mp_0()
     )
 
 
-# Plane #
+# Galaxies #
 
 
-def make_plane_7x7():
-    return ag.Plane(galaxies=[make_gal_x1_lp_x1_mp()])
+def make_galaxies_7x7():
+    return ag.Galaxies(galaxies=[make_gal_x1_lp_x1_mp()])
 
 
-def make_plane_x2_gal_7x7():
-    return ag.Plane(galaxies=[make_gal_x1_lp_x1_mp(), make_gal_x1_lp_x1_mp()])
+def make_galaxies_x2_7x7():
+    return ag.Galaxies(galaxies=[make_gal_x1_lp_x1_mp(), make_gal_x1_lp_x1_mp()])
 
 
-def make_plane_x2_galaxy_inversion_7x7():
+def make_galaxies_x2_inversion_7x7():
     source_gal_inversion = ag.Galaxy(
         redshift=1.0,
         pixelization=ag.mesh.Rectangular(),
         regularization=ag.reg.Constant(),
     )
 
-    return ag.Plane(galaxies=[make_gal_x1_lp(), source_gal_inversion])
+    return [make_gal_x1_lp(), source_gal_inversion]
 
 
 # COSMOLOGY #
 
 
 def make_Planck15():
     return ag.cosmo.Planck15()
@@ -164,23 +167,23 @@
         ),
     )
 
 
 def make_fit_quantity_7x7_array_2d():
     return ag.FitQuantity(
         dataset=make_dataset_quantity_7x7_array_2d(),
-        light_mass_obj=make_plane_7x7(),
+        light_mass_obj=make_galaxies_7x7(),
         func_str="convergence_2d_from",
     )
 
 
 def make_fit_quantity_7x7_vector_yx_2d():
     return ag.FitQuantity(
         dataset=make_dataset_quantity_7x7_vector_yx_2d(),
-        light_mass_obj=make_plane_7x7(),
+        light_mass_obj=make_galaxies_7x7(),
         func_str="deflections_yx_2d_from",
     )
 
 
 # galaxies #
 
 
@@ -205,70 +208,68 @@
 
 def make_adapt_images_7x7():
     return ag.AdaptImages(
         galaxy_name_image_dict=make_adapt_galaxy_name_image_dict_7x7(),
     )
 
 
-def make_fit_imaging_7x7():
-    return ag.FitImaging(dataset=make_masked_imaging_7x7(), plane=make_plane_7x7())
-
-
 def make_fit_imaging_x2_galaxy_7x7():
-    plane = ag.Plane(galaxies=[make_gal_x1_lp(), make_gal_x1_lp(), make_gal_x1_mp()])
-
-    return ag.FitImaging(dataset=make_masked_imaging_7x7(), plane=plane)
+    return ag.FitImaging(
+        dataset=make_masked_imaging_7x7(),
+        galaxies=[make_gal_x1_lp(), make_gal_x1_lp(), make_gal_x1_mp()],
+    )
 
 
 def make_fit_imaging_x2_galaxy_inversion_7x7():
     return ag.FitImaging(
-        dataset=make_masked_imaging_7x7(), plane=make_plane_x2_galaxy_inversion_7x7()
+        dataset=make_masked_imaging_7x7(), galaxies=make_galaxies_x2_inversion_7x7()
     )
 
 
 def make_fit_interferometer_7x7():
     return ag.FitInterferometer(
         dataset=make_interferometer_7(),
-        plane=make_plane_7x7(),
+        galaxies=make_galaxies_7x7(),
         settings_inversion=aa.SettingsInversion(use_w_tilde=False),
     )
 
 
 def make_fit_interferometer_x2_galaxy_inversion_7x7():
     return ag.FitInterferometer(
         dataset=make_interferometer_7(),
-        plane=make_plane_x2_galaxy_inversion_7x7(),
+        galaxies=make_galaxies_x2_inversion_7x7(),
         settings_inversion=aa.SettingsInversion(use_w_tilde=False),
     )
 
 
-def make_samples_with_result():
-    galaxies = [
-        ag.Galaxy(redshift=0.5, light=ag.lp.Sersic(intensity=1.0)),
-        ag.Galaxy(redshift=1.0, light=ag.lp.Sersic(intensity=2.0)),
-    ]
+def make_samples_summary_with_result():
+    galaxy = af.Model(ag.Galaxy, redshift=0.5, bulge=af.Model(ag.lp.Sersic))
+
+    model = af.Collection(galaxies=af.Collection(galaxy=galaxy))
 
-    plane = ag.Plane(galaxies=galaxies)
+    instance = model.instance_from_prior_medians()
 
-    return ag.m.MockSamples(max_log_likelihood_instance=plane)
+    return ag.m.MockSamplesSummary(max_log_likelihood_instance=instance)
 
 
 def make_analysis_imaging_7x7():
-    return ag.AnalysisImaging(
+    analysis = ag.AnalysisImaging(
         dataset=make_masked_imaging_7x7(),
-        adapt_images=make_adapt_images_7x7(),
         settings_inversion=aa.SettingsInversion(use_w_tilde=False),
     )
+    analysis._adapt_images = make_adapt_images_7x7()
+    return analysis
 
 
 def make_analysis_interferometer_7():
-    return ag.AnalysisInterferometer(
+    analysis = ag.AnalysisInterferometer(
         dataset=make_interferometer_7(),
-        adapt_images=make_adapt_images_7x7(),
     )
+    analysis._adapt_images = make_adapt_images_7x7()
+    return analysis
 
 
 def make_include_1d_all():
     return aplt.Include1D(half_light_radius=True)
 
 
 def make_include_2d_all():
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/galaxy/galaxy.py` & `autogalaxy-2024.5.16.0/autogalaxy/galaxy/galaxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from autogalaxy import exc
 from autogalaxy.operate.deflections import OperateDeflections
 from autogalaxy.operate.image import OperateImageList
 from autogalaxy.profiles.geometry_profiles import GeometryProfile
 from autogalaxy.profiles.light.abstract import LightProfile
 from autogalaxy.profiles.light.linear import LightProfileLinear
+from autogalaxy.profiles.light.snr.abstract import LightProfileSNR
 from autogalaxy.profiles.mass.abstract.abstract import MassProfile
 
 
 class Galaxy(af.ModelObject, OperateImageList, OperateDeflections):
     """
     @DynamicAttrs
     """
@@ -79,15 +80,15 @@
         return self.dict() == other.dict()
 
     @property
     def profile_dict(self) -> Dict:
         return {
             key: value
             for key, value in self.__dict__.items()
-            if isinstance(value, GeometryProfile)
+            if isinstance(value, GeometryProfile) or isinstance(value, aa.Pixelization)
         }
 
     def dict(self) -> Dict:
         d = instance_as_dict(self)
         d["arguments"] = {
             **d.get("arguments", {}),
             **{name: to_dict(profile) for name, profile in self.profile_dict.items()},
@@ -153,64 +154,33 @@
 
         radial_projected_shape_slim = self._radial_projected_shape_slim_from(grid=grid)
 
         return grid.grid_2d_radial_projected_from(
             centre=centre, angle=angle + 90, shape_slim=radial_projected_shape_slim
         )
 
-    @aa.grid_dec.grid_2d_to_structure
-    def image_2d_from(
-        self, grid: aa.type.Grid2DLike, operated_only: Optional[bool] = None
-    ) -> Union[np.ndarray, aa.Array2D]:
-        """
-        Returns the summed 2D image of the galaxy's light profiles from a 2D grid of Cartesian (y,x) coordinates.
-
-        If the galaxy has no light profiles, a numpy array of zeros is returned.
-
-        If the `operated_only` input is included, the function omits light profiles which are parents of
-        the `LightProfileOperated` object, which signifies that the light profile represents emission that has
-        already had the instrument operations (e.g. PSF convolution, a Fourier transform) applied to it.
-
-        See the `autogalaxy.profiles.light` package for details of how images are computed from a light
-        profile.
-
-        The decorator `grid_2d_to_structure` converts the output arrays from ndarrays to an `Array2D` data structure
-        using the input `grid`'s attributes.
-
-        Parameters
-        ----------
-        grid
-            The 2D (y, x) coordinates where values of the image are evaluated.
-        operated_only
-            By default, the image is the sum of light profile images (irrespective of whether they have been operatd on
-            or not). If this input is included as a bool, only images which are or are not already operated are summed
-            and returned.
-        """
-        if (
-            len(self.cls_list_from(cls=LightProfile, cls_filtered=LightProfileLinear))
-            > 0
-        ):
-            return sum(self.image_2d_list_from(grid=grid, operated_only=operated_only))
-
-        return np.zeros((grid.shape[0],))
-
     def image_2d_list_from(
         self, grid: aa.type.Grid2DLike, operated_only: Optional[bool] = None
     ) -> List[aa.Array2D]:
         """
         Returns a list of the 2D images of the galaxy's light profiles from a 2D grid of Cartesian (y,x) coordinates.
 
-        This function is primarily used in the `autogalaxy.operate.image` package, to output images of the `Galaxy`
-        that have operations such as a 2D convolution or Fourier transform applied to them.
-
         If the galaxy has no light profiles, a numpy array of zeros is returned.
 
+        The images output by this function do not include instrument operations, such as PSF convolution (for imaging
+        data) or a Fourier transform (for interferometer data).
+
+        Inherited methods in the `autogalaxy.operate.image` package can apply these operations to the images.
+        These functions may have the `operated_only` input passed to them, which is why this function includes
+        the `operated_only` input.
+
         If the `operated_only` input is included, the function omits light profiles which are parents of
         the `LightProfileOperated` object, which signifies that the light profile represents emission that has
-        already had the instrument operations (e.g. PSF convolution, a Fourier transform) applied to it.
+        already had the instrument operations (e.g. PSF convolution, a Fourier transform) applied to it and therefore
+        that operation is not performed again.
 
         See the `autogalaxy.profiles.light` package for details of how images are computed from a light
         profile.
 
         Parameters
         ----------
         grid
@@ -224,24 +194,56 @@
         return [
             light_profile.image_2d_from(grid=grid, operated_only=operated_only)
             for light_profile in self.cls_list_from(
                 cls=LightProfile, cls_filtered=LightProfileLinear
             )
         ]
 
-    @aa.grid_dec.grid_1d_output_structure
+    @aa.grid_dec.to_array
+    def image_2d_from(
+        self, grid: aa.type.Grid2DLike, operated_only: Optional[bool] = None
+    ) -> Union[np.ndarray, aa.Array2D]:
+        """
+        Returns the 2D image of all galaxy light profiles summed from a 2D grid of Cartesian (y,x) coordinates.
+
+        This function first computes the image of each galaxy, via the function `image_2d_list_from`. The
+        images are then summed to give the overall image of the galaxies.
+
+        Refer to the function `image_2d_list_from` for a full description of the calculation and how the `operated_only`
+        input is used.
+
+        Parameters
+        ----------
+        grid
+            The 2D (y, x) coordinates where values of the image are evaluated.
+        operated_only
+            The returned list from this function contains all light profile images, and they are never operated on
+            (e.g. via the imaging PSF). However, inherited methods in the `autogalaxy.operate.image` package can
+            apply these operations to the images, which may have the `operated_only` input passed to them. This input
+            therefore is used to pass the `operated_only` input to these methods.
+        """
+
+        if (
+            len(self.cls_list_from(cls=LightProfile, cls_filtered=LightProfileLinear))
+            > 0
+        ):
+            return sum(self.image_2d_list_from(grid=grid, operated_only=operated_only))
+
+        return np.zeros((grid.shape[0],))
+
+    @aa.grid_dec.to_projected
     def image_1d_from(self, grid: aa.type.Grid2DLike) -> np.ndarray:
         """
         Returns the summed 1D image of the galaxy's light profiles using a grid of Cartesian (y,x) coordinates.
 
         If the galaxy has no light profiles, a grid of zeros is returned.
 
         See `profiles.light` module for details of how this is performed.
 
-        The decorator `grid_1d_output_structure` converts the output arrays from ndarrays to an `Array1D` data
+        The decorator `to_projected` converts the output arrays from ndarrays to an `Array1D` data
         structure using the input `grid`'s attributes.
 
         Parameters
         ----------
         grid
             The 1D (x,) coordinates where values of the image are evaluated.
         """
@@ -257,27 +259,26 @@
 
                 image_1d_list.append(light_profile.image_1d_from(grid=grid_radial))
 
             return sum(image_1d_list)
 
         return np.zeros((grid.shape[0],))
 
-    @aa.grid_dec.grid_2d_to_vector_yx
-    @aa.grid_dec.grid_2d_to_structure
-    def deflections_yx_2d_from(self, grid: aa.type.Grid2DLike) -> np.ndarray:
+    @aa.grid_dec.to_vector_yx
+    def deflections_yx_2d_from(self, grid: aa.type.Grid2DLike, **kwargs) -> np.ndarray:
         """
         Returns the summed 2D deflection angles of the galaxy's mass profiles from a 2D grid of Cartesian (y,x)
         coordinates.
 
         If the galaxy has no mass profiles, a numpy array of zeros is returned.
 
         See the `autogalaxy.profiles.mass` package for details of how deflection angles are computed from a
         mass profile.
 
-        The decorator `grid_2d_to_vector_yx` converts the output arrays from ndarrays to a `VectorYX2D` data structure
+        The decorator `to_vector_yx` converts the output arrays from ndarrays to a `VectorYX2D` data structure
         using the input `grid`'s attributes.
 
         Parameters
         ----------
         grid
             The 2D (y, x) coordinates where values of the deflection angles are evaluated.
         """
@@ -286,16 +287,16 @@
                 map(
                     lambda p: p.deflections_yx_2d_from(grid=grid),
                     self.cls_list_from(cls=MassProfile),
                 )
             )
         return np.zeros((grid.shape[0], 2))
 
-    @aa.grid_dec.grid_2d_to_structure
-    def convergence_2d_from(self, grid: aa.type.Grid2DLike) -> np.ndarray:
+    @aa.grid_dec.to_array
+    def convergence_2d_from(self, grid: aa.type.Grid2DLike, **kwargs) -> np.ndarray:
         """
         Returns the summed 2D convergence of the galaxy's mass profiles from a 2D grid of Cartesian (y,x) coordinates.
 
         If the galaxy has no mass profiles, a numpy array of zeros is returned.
 
         See the `autogalaxy.profiles.mass` package for details of how convergences are computed from a mass
         profile.
@@ -313,24 +314,31 @@
                 map(
                     lambda p: p.convergence_2d_from(grid=grid),
                     self.cls_list_from(cls=MassProfile),
                 )
             )
         return np.zeros((grid.shape[0],))
 
-    @aa.grid_dec.grid_1d_output_structure
+    @aa.grid_dec.to_grid
+    def traced_grid_2d_from(self, grid: aa.type.Grid2DLike) -> aa.type.Grid2DLike:
+        """
+        Trace an input grid using the galaxy's its deflection angles.
+        """
+        return grid - self.deflections_yx_2d_from(grid=grid)
+
+    @aa.grid_dec.to_projected
     def convergence_1d_from(self, grid: aa.type.Grid1D2DLike) -> np.ndarray:
         """
         Returns the summed 1D convergence of the galaxy's mass profiles using a grid of Cartesian (y,x) coordinates.
 
         If the galaxy has no mass profiles, a grid of zeros is returned.
 
         See `profiles.mass` module for details of how this is performed.
 
-        The decorator `grid_1d_output_structure` converts the output arrays from ndarrays to an `Array1D` data
+        The decorator `to_projected` converts the output arrays from ndarrays to an `Array1D` data
         structure using the input `grid`'s attributes.
 
         Parameters
         ----------
         grid
             The 1D (x,) coordinates where values of the convergence are evaluated.
         """
@@ -346,16 +354,16 @@
                     mass_profile.convergence_1d_from(grid=grid_radial)
                 )
 
             return sum(convergence_1d_list)
 
         return np.zeros((grid.shape[0],))
 
-    @aa.grid_dec.grid_2d_to_structure
-    def potential_2d_from(self, grid: aa.type.Grid2DLike) -> np.ndarray:
+    @aa.grid_dec.to_array
+    def potential_2d_from(self, grid: aa.type.Grid2DLike, **kwargs) -> np.ndarray:
         """
         Returns the summed 2D potential of the galaxy's mass profiles from a 2D grid of Cartesian (y,x) coordinates.
 
         If the galaxy has no mass profiles, a numpy array of zeros is returned.
 
         See the `autogalaxy.profiles.mass` package for details of how potentials are computed from a mass
         profile.
@@ -373,24 +381,24 @@
                 map(
                     lambda p: p.potential_2d_from(grid=grid),
                     self.cls_list_from(cls=MassProfile),
                 )
             )
         return np.zeros((grid.shape[0],))
 
-    @aa.grid_dec.grid_1d_output_structure
+    @aa.grid_dec.to_projected
     def potential_1d_from(self, grid: aa.type.Grid2DLike) -> np.ndarray:
         """
         Returns the summed 1D potential of the galaxy's mass profiles using a grid of Cartesian (y,x) coordinates.
 
         If the galaxy has no mass profiles, a grid of zeros is returned.
 
         See `profiles.mass` module for details of how this is performed.
 
-        The decorator `grid_1d_output_structure` converts the output arrays from ndarrays to an `Array1D` data
+        The decorator `to_projected` converts the output arrays from ndarrays to an `Array1D` data
         structure using the input `grid`'s attributes.
 
         Parameters
         ----------
         grid
             The 1D (x,) coordinates where values of the potential are evaluated.
         """
@@ -511,7 +519,45 @@
                     self.cls_list_from(cls=MassProfile),
                 )
             )
         else:
             raise exc.GalaxyException(
                 "You cannot perform a mass-based calculation on a galaxy which does not have a mass-profile"
             )
+
+    def set_snr_of_snr_light_profiles(
+        self,
+        grid: aa.type.Grid2DLike,
+        exposure_time: float,
+        background_sky_level: float = 0.0,
+        psf: Optional[aa.Kernel2D] = None,
+    ):
+        """
+        Iterate over every galaxy finding all `LightProfileSNR` light profiles and set their `intensity` values to
+        values which give their input `signal_to_noise_ratio` value, which is performed as follows:
+
+        - Evaluate the image of each light profile on the input grid.
+        - Blur this image with a PSF, if included.
+        - Take the value of the brightest pixel.
+        - Use an input `exposure_time` and `background_sky` (e.g. from the `SimulatorImaging` object) to determine
+          what value of `intensity` gives the desired signal to noise ratio for the image.
+
+        Parameters
+        ----------
+        grid
+            The (y, x) coordinates in the original reference frame of the grid.
+        exposure_time
+            The exposure time of the simulated imaging.
+        background_sky_level
+            The level of the background sky of the simulated imaging.
+        psf
+            The psf of the simulated imaging which can change the S/N of the light profile due to spreading out
+            the emission.
+        """
+        for light_profile in self.cls_list_from(cls=LightProfile):
+            if isinstance(light_profile, LightProfileSNR):
+                light_profile.set_intensity_from(
+                    grid=grid,
+                    exposure_time=exposure_time,
+                    background_sky_level=background_sky_level,
+                    psf=psf,
+                )
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/galaxy/mock/mock_galaxy.py` & `autogalaxy-2024.5.16.0/autogalaxy/galaxy/mock/mock_galaxy.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 
 
 class MockGalaxy:
     def __init__(self, value, shape=1):
         self.value = value
         self.shape = shape
 
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.grid_dec.to_array
     def image_2d_from(self, grid):
         return np.full(shape=self.shape, fill_value=self.value)
 
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.grid_dec.to_array
     def convergence_2d_from(self, grid):
         return np.full(shape=self.shape, fill_value=self.value)
 
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.grid_dec.to_array
     def potential_2d_from(self, grid):
         return np.full(shape=self.shape, fill_value=self.value)
 
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.grid_dec.to_vector_yx
     def deflections_yx_2d_from(self, grid):
         return np.full(shape=(self.shape, 2), fill_value=self.value)
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/galaxy/plot/galaxy_plotters.py` & `autogalaxy-2024.5.16.0/autogalaxy/galaxy/plot/galaxy_plotters.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/galaxy/redshift.py` & `autogalaxy-2024.5.16.0/autogalaxy/galaxy/redshift.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/galaxy/stellar_dark_decomp.py` & `autogalaxy-2024.5.16.0/autogalaxy/galaxy/stellar_dark_decomp.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/gui/clicker.py` & `autogalaxy-2024.5.16.0/autogalaxy/gui/clicker.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/gui/scribbler.py` & `autogalaxy-2024.5.16.0/autogalaxy/gui/scribbler.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,15 @@
         plt.figure()
         plt.subplot(121)
         plt.imshow(junk_mask.astype("int"), cmap="gray")
         plt.title("Junk mask")
         plt.subplot(122)
         plt.imshow(feature_mask.astype("int"), cmap="gray")
         plt.title("Feature mask")
-        plt.show()
+        # plt.show()
         return junk_mask
 
     def add_circle_to_mask(self, center, radius, mask):
         if not center[0] or not center[1]:
             return
         xx, yy = np.mgrid[: self.im.shape[0], : self.im.shape[1]]
         circle_mask = (xx - center[1]) ** 2 + (yy - center[0]) ** 2 <= radius**2
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/imaging/fit_imaging.py` & `autogalaxy-2024.5.16.0/autogalaxy/imaging/fit_imaging.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,48 +2,49 @@
 from typing import Dict, List, Optional
 
 from autoconf import cached_property
 
 import autoarray as aa
 
 from autogalaxy.abstract_fit import AbstractFitInversion
-from autogalaxy.analysis.adapt_images import AdaptImages
+from autogalaxy.analysis.adapt_images.adapt_images import AdaptImages
 from autogalaxy.analysis.preloads import Preloads
 from autogalaxy.galaxy.galaxy import Galaxy
-from autogalaxy.plane.plane import Plane
-from autogalaxy.plane.to_inversion import PlaneToInversion
+from autogalaxy.galaxy.galaxies import Galaxies
+from autogalaxy.galaxy.to_inversion import GalaxiesToInversion
 from autogalaxy.profiles.light.abstract import LightProfile
 from autogalaxy.profiles.light.linear import LightProfileLinear
 from autogalaxy.profiles.light.operated.abstract import LightProfileOperated
 
 from autogalaxy import exc
 
 
 class FitImaging(aa.FitImaging, AbstractFitInversion):
     def __init__(
         self,
         dataset: aa.Imaging,
-        plane: Plane,
+        galaxies: List[Galaxy],
+        dataset_model: Optional[aa.DatasetModel] = None,
         adapt_images: Optional[AdaptImages] = None,
         settings_inversion: aa.SettingsInversion = aa.SettingsInversion(),
         preloads: aa.Preloads = Preloads(),
         run_time_dict: Optional[Dict] = None,
     ):
         """
-        Fits an imaging dataset using a `Plane` object.
+        Fits an imaging dataset using a list of galaxies.
 
         The fit performs the following steps:
 
-        1) Compute the sum of all images of galaxy light profiles in the `Plane`.
+        1) Compute the sum of all images of galaxy light profiles in the list of galaxies.
 
         2) Blur this with the imaging PSF to created the `blurred_image`.
 
         3) Subtract this image from the `data` to create the `profile_subtracted_image`.
 
-        4) If the `Plane` has any linear algebra objects (e.g. linear light profiles, a pixelization / regulariation)
+        4) If the galaxies list has any linear algebra objects (e.g. linear light profiles, a pixelization / regulariation)
            fit the `profile_subtracted_image` with these objects via an inversion.
 
         5) Compute the `model_data` as the sum of the `blurred_image` and `reconstructed_data` of the inversion (if
            an inversion is not performed the `model_data` is only the `blurred_image`.
 
         6) Subtract the `model_data` from the data and compute the residuals, chi-squared and likelihood via the
            noise-map (if an inversion is performed the `log_evidence`, including additional terms describing the linear
@@ -51,274 +52,280 @@
 
         When performing a `model-fit`via an `AnalysisImaging` object the `figure_of_merit` of this `FitImaging` object
         is called and returned in the `log_likelihood_function`.
 
         Parameters
         ----------
         dataset
-            The imaging dataset which is fitted by the galaxies in the plane.
-        plane
-            The plane of galaxies whose light profile images are used to fit the imaging data.
+            The imaging dataset which is fitted by the galaxies.
+        galaxies
+            The galaxies whose light profile images are used to fit the imaging data.
+        dataset_model
+            Attributes which allow for parts of a dataset to be treated as a model (e.g. the background sky level).
         adapt_images
             Contains the adapt-images which are used to make a pixelization's mesh and regularization adapt to the
             reconstructed galaxy's morphology.
         settings_inversion
             Settings controlling how an inversion is fitted for example which linear algebra formalism is used.
         preloads
             Contains preloaded calculations (e.g. linear algebra matrices) which can skip certain calculations in
             the fit.
         run_time_dict
             A dictionary which if passed to the fit records how long fucntion calls which have the `profile_func`
             decorator take to run.
         """
 
-        self.plane = plane
+        self.galaxies = Galaxies(galaxies=galaxies, run_time_dict=run_time_dict)
         self.preloads = preloads
 
         super().__init__(
             dataset=dataset,
+            dataset_model=dataset_model,
             run_time_dict=run_time_dict,
         )
         AbstractFitInversion.__init__(
-            self=self, model_obj=plane, settings_inversion=settings_inversion
+            self=self,
+            model_obj=self.galaxies,
+            settings_inversion=settings_inversion,
         )
 
         self.adapt_images = adapt_images
         self.settings_inversion = settings_inversion
 
     @property
-    def galaxies(self) -> List[Galaxy]:
-        return self.plane.galaxies
-
-    @property
-    def grid(self) -> aa.type.Grid2DLike:
-        return self.dataset.grid
-
-    @property
     def blurred_image(self) -> aa.Array2D:
         """
-        Returns the image of the light profiles of all galaxies in the fit's plane, convolved with the
-        imaging dataset's PSF.
+        Returns the image of the light profiles of all galaxies in the fit, convolved with the imaging dataset's PSF.
 
-        If the plane does not have any light profiles, the image is computed bypassing the convolution routine
+        If the galaxies do not have any light profiles, the image is computed bypassing the convolution routine
         altogether.
         """
 
-        if len(self.plane.cls_list_from(cls=LightProfile)) == len(
-            self.plane.cls_list_from(cls=LightProfileOperated)
+        if len(self.galaxies.cls_list_from(cls=LightProfile)) == len(
+            self.galaxies.cls_list_from(cls=LightProfileOperated)
         ):
-            return self.plane.image_2d_from(
-                grid=self.dataset.grid,
+            return self.galaxies.image_2d_from(
+                grid=self.grid,
             )
 
-        return self.plane.blurred_image_2d_from(
-            grid=self.dataset.grid,
+        return self.galaxies.blurred_image_2d_from(
+            grid=self.grid,
             convolver=self.dataset.convolver,
-            blurring_grid=self.dataset.blurring_grid,
+            blurring_grid=self.blurring_grid,
         )
 
     @property
     def profile_subtracted_image(self) -> aa.Array2D:
         """
-        Returns the dataset's image data with all blurred light profile images in the fit's plane subtracted.
-        """
-        return self.image - self.blurred_image
-
-    @property
-    def model_data(self) -> aa.Array2D:
-        """
-        Returns the model-image that is used to fit the data.
-
-        If the plane does not have any linear objects and therefore omits an inversion, the model data is the
-        sum of all light profile images blurred with the PSF.
-
-        If a inversion is included it is the sum of this image and the inversion's reconstruction of the image.
+        Returns the dataset's image data with all blurred light profile images in the fit subtracted.
         """
-        return self.blurred_image
+        return self.data - self.blurred_image
 
     @property
-    def plane_to_inversion(self) -> PlaneToInversion:
-        return PlaneToInversion(
-            plane=self.plane,
-            dataset=self.dataset,
+    def galaxies_to_inversion(self) -> GalaxiesToInversion:
+        dataset = aa.DatasetInterface(
             data=self.profile_subtracted_image,
             noise_map=self.noise_map,
+            convolver=self.dataset.convolver,
             w_tilde=self.w_tilde,
+            grid=self.grid,
+            grid_pixelization=self.grid_pixelization,
+            blurring_grid=self.blurring_grid,
+            border_relocator=self.dataset.border_relocator,
+        )
+
+        return GalaxiesToInversion(
+            dataset=dataset,
+            galaxies=self.galaxies,
             adapt_images=self.adapt_images,
             settings_inversion=self.settings_inversion,
             preloads=self.preloads,
             run_time_dict=self.run_time_dict,
         )
 
     @cached_property
     def inversion(self) -> Optional[aa.AbstractInversion]:
         """
-        If the plane has linear objects which are used to fit the data (e.g. a linear light profile / pixelization)
+        If the galaxies have linear objects which are used to fit the data (e.g. a linear light profile / pixelization)
         this function returns a linear inversion, where the flux values of these objects (e.g. the `intensity`
         of linear light profiles) are computed via linear matrix algebra.
 
-        The data passed to this function is the dataset's image with all light profile images of the plane subtracted,
+        The data passed to this function is the dataset's image with all light profile images of the galaxies subtracted,
         ensuring that the inversion only fits the data with ordinary light profiles subtracted.
         """
 
         if self.perform_inversion:
-            return self.plane_to_inversion.inversion
+            return self.galaxies_to_inversion.inversion
 
     @property
     def model_data(self) -> aa.Array2D:
         """
         Returns the model-image that is used to fit the data.
 
-        If the plane does not have any linear objects and therefore omits an inversion, the model data is the
+        If the galaxies do not have any linear objects and therefore omits an inversion, the model data is the
         sum of all light profile images blurred with the PSF.
 
         If a inversion is included it is the sum of this image and the inversion's reconstruction of the image.
         """
 
         if self.perform_inversion:
             return self.blurred_image + self.inversion.mapped_reconstructed_data
 
         return self.blurred_image
 
     @property
     def galaxy_model_image_dict(self) -> Dict[Galaxy, np.ndarray]:
         """
-        A dictionary which associates every galaxy in the plane with its `model_image`.
+        A dictionary which associates every galaxy in the fit with its `model_image`.
 
         This image is the image of the sum of:
 
-        - The images of all ordinary light profiles in that plane summed and convolved with the imaging data's PSF.
+        - The images of all ordinary light profiles summed and convolved with the imaging data's PSF.
         - The images of all linear objects (e.g. linear light profiles / pixelizations), where the images are solved
           for first via the inversion.
 
         For modeling, this dictionary is used to set up the `adapt_images` that adapt certain pixelizations to the
         data being fitted.
         """
 
-        galaxy_blurred_image_2d_dict = self.plane.galaxy_blurred_image_2d_dict_from(
+        galaxy_blurred_image_2d_dict = self.galaxies.galaxy_blurred_image_2d_dict_from(
             grid=self.grid,
             convolver=self.dataset.convolver,
-            blurring_grid=self.dataset.blurring_grid,
+            blurring_grid=self.blurring_grid,
         )
 
         galaxy_linear_obj_image_dict = self.galaxy_linear_obj_data_dict_from(
             use_image=True
         )
 
         return {**galaxy_blurred_image_2d_dict, **galaxy_linear_obj_image_dict}
 
     @property
-    def model_images_of_galaxies_list(self) -> List:
-        """
-        A list of the model images of each galaxy in the plane.
-        """
-        return list(self.galaxy_model_image_dict.values())
-
-    @property
-    def subtracted_images_of_galaxies_list(self) -> List[aa.Array2D]:
+    def subtracted_images_of_galaxies_dict(self) -> Dict[Galaxy, aa.Array2D]:
         """
-        A list of the subtracted image of every galaxy.
+        A dictionary associating every galaxy with its `subtracted_image`.
 
         A subtracted image of a galaxy is the data where all other galaxy images are subtracted from it, therefore
         showing how a galaxy appears in the data in the absence of all other galaxies.
 
         This is used to visualize the contribution of each galaxy in the data.
         """
 
-        subtracted_images_of_galaxies_list = []
+        subtracted_images_of_galaxies_dict = {}
 
         model_images_of_galaxies_list = self.model_images_of_galaxies_list
 
         for galaxy_index in range(len(self.galaxies)):
             other_galaxies_model_images = [
                 model_image
                 for i, model_image in enumerate(model_images_of_galaxies_list)
                 if i != galaxy_index
             ]
 
-            subtracted_image = self.image - sum(other_galaxies_model_images)
+            subtracted_image = self.data - sum(other_galaxies_model_images)
+
+            subtracted_images_of_galaxies_dict[
+                self.galaxies[galaxy_index]
+            ] = subtracted_image
+
+        return subtracted_images_of_galaxies_dict
+
+    @property
+    def model_images_of_galaxies_list(self) -> List:
+        """
+        A list of the model images of each galaxy.
+        """
+        return list(self.galaxy_model_image_dict.values())
+
+    @property
+    def subtracted_images_of_galaxies_list(self) -> List[aa.Array2D]:
+        """
+        A list of the subtracted image of every galaxy.
 
-            subtracted_images_of_galaxies_list.append(subtracted_image)
+        A subtracted image of a galaxy is the data where all other galaxy images are subtracted from it, therefore
+        showing how a galaxy appears in the data in the absence of all other galaxies.
 
-        return subtracted_images_of_galaxies_list
+        This is used to visualize the contribution of each galaxy in the data.
+        """
+        return list(self.subtracted_images_of_galaxies_dict.values())
 
     @property
     def unmasked_blurred_image(self) -> aa.Array2D:
         """
         The blurred image of the overall fit that would be evaluated without a mask being used.
 
         Linear objects are tied to the mask defined to used to perform the fit, therefore their unmasked blurred
         image cannot be computed.
         """
-        if self.plane.has(cls=LightProfileLinear):
+        if self.galaxies.has(cls=LightProfileLinear):
             exc.raise_linear_light_profile_in_unmasked()
 
-        return self.plane.unmasked_blurred_image_2d_from(
+        return self.galaxies.unmasked_blurred_image_2d_from(
             grid=self.grid, psf=self.dataset.psf
         )
 
     @property
     def unmasked_blurred_image_of_galaxies_list(self) -> List[aa.Array2D]:
         """
-        The blurred image of every galaxy int he plane used in this fit, that would be evaluated without a mask being
-        used.
+        The blurred image of every galaxy in the fit, that would be evaluated without a mask being used.
 
         Linear objects are tied to the mask defined to used to perform the fit, therefore their unmasked blurred
         image cannot be computed.
         """
-        if self.plane.has(cls=LightProfileLinear):
+        if self.galaxies.has(cls=LightProfileLinear):
             exc.raise_linear_light_profile_in_unmasked()
 
-        return self.plane.unmasked_blurred_image_2d_list_from(
+        return self.galaxies.unmasked_blurred_image_2d_list_from(
             grid=self.grid, psf=self.dataset.psf
         )
 
     @property
-    def plane_linear_light_profiles_to_light_profiles(self) -> Plane:
+    def galaxies_linear_light_profiles_to_light_profiles(self) -> List[Galaxy]:
         """
-        The `Plane` where all linear light profiles have been converted to ordinary light profiles, where their
+        The galaxy list where all linear light profiles have been converted to ordinary light profiles, where their
         `intensity` values are set to the values inferred by this fit.
 
         This is typically used for visualization, because linear light profiles cannot be used in `LightProfilePlotter`
         or `GalaxyPlotter` objects.
         """
         return self.model_obj_linear_light_profiles_to_light_profiles
 
     def refit_with_new_preloads(
         self,
         preloads: Preloads,
         settings_inversion: Optional[aa.SettingsInversion] = None,
     ) -> "FitImaging":
         """
-        Returns a new fit which uses the dataset, plane and other objects of this fit, but uses a different set of
+        Returns a new fit which uses the dataset, galaxies and other objects of this fit, but uses a different set of
         preloads input into this function.
 
         This is used when setting up the preloads objects, to concisely test how using different preloads objects
         changes the attributes of the fit.
 
         Parameters
         ----------
         preloads
             The new preloads which are used to refit the data using the
         settings_inversion
             Settings controlling how an inversion is fitted for example which linear algebra formalism is used.
 
         Returns
         -------
-        A new fit which has used new preloads input into this function but the same dataset, plane and other settings.
+        A new fit which has used new preloads input into this function but the same dataset, galaxies and other settings.
         """
         run_time_dict = {} if self.run_time_dict is not None else None
 
         settings_inversion = (
             self.settings_inversion
             if settings_inversion is None
             else settings_inversion
         )
 
         return FitImaging(
             dataset=self.dataset,
-            plane=self.plane,
+            galaxies=self.galaxies,
+            dataset_model=self.dataset_model,
             adapt_images=self.adapt_images,
             settings_inversion=settings_inversion,
             preloads=preloads,
             run_time_dict=run_time_dict,
         )
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/imaging/model/analysis.py` & `autogalaxy-2024.5.16.0/autogalaxy/imaging/model/analysis.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,66 +3,67 @@
 from typing import Dict, Optional, Tuple
 
 import autofit as af
 import autoarray as aa
 
 from autoarray.exc import PixelizationException
 
-from autogalaxy.analysis.adapt_images import AdaptImages
-from autogalaxy.analysis.analysis import AnalysisDataset
+from autogalaxy.analysis.adapt_images.adapt_image_maker import AdaptImageMaker
+from autogalaxy.analysis.analysis.dataset import AnalysisDataset
 from autogalaxy.analysis.preloads import Preloads
 from autogalaxy.cosmology.lensing import LensingCosmology
 from autogalaxy.cosmology.wrap import Planck15
-from autogalaxy.imaging.model.visualizer import VisualizerImaging
 from autogalaxy.imaging.model.result import ResultImaging
+from autogalaxy.imaging.model.visualizer import VisualizerImaging
 from autogalaxy.imaging.fit_imaging import FitImaging
-from autogalaxy.plane.plane import Plane
 
 from autogalaxy import exc
 
 
 class AnalysisImaging(AnalysisDataset):
+    Result = ResultImaging
+    Visualizer = VisualizerImaging
+
     def __init__(
         self,
         dataset: aa.Imaging,
-        adapt_images: Optional[AdaptImages] = None,
+        adapt_image_maker: Optional[AdaptImageMaker] = None,
         cosmology: LensingCosmology = Planck15(),
         settings_inversion: aa.SettingsInversion = None,
     ):
         """
         Fits a galaxy model to an imaging dataset via a non-linear search.
 
         The `Analysis` class defines the `log_likelihood_function` which fits the model to the dataset and returns the
         log likelihood value defining how well the model fitted the data.
 
         It handles many other tasks, such as visualization, outputting results to hard-disk and storing results in
         a format that can be loaded after the model-fit is complete.
 
-        This class is used for model-fits which fit galaxies (or objects containing galaxies like a `Plane`)
-        to an imaging dataset.
+        This class is used for model-fits which fit galaxies to an imaging dataset.
 
         This class stores the settings used to perform the model-fit for certain components of the model (e.g. a
         pixelization or inversion), the Cosmology used for the analysis and adapt images used for certain model
         classes.
 
         Parameters
         ----------
         dataset
             The `Imaging` dataset that the model is fitted to.
-        adapt_images
-            The adapt-model image and galaxies images of a previous result in a model-fitting pipeline, which are
+        adapt_image_maker
+            Makes the adapt-model image and galaxies images of a previous result in a model-fitting pipeline, which are
             used by certain classes for adapting the analysis to the properties of the dataset.
         cosmology
             The Cosmology assumed for this analysis.
         settings_inversion
             Settings controlling how an inversion is fitted for example which linear algebra formalism is used.
         """
         super().__init__(
             dataset=dataset,
-            adapt_images=adapt_images,
+            adapt_image_maker=adapt_image_maker,
             cosmology=cosmology,
             settings_inversion=settings_inversion,
         )
 
     @property
     def imaging(self):
         return self.dataset
@@ -104,18 +105,18 @@
 
         1) If the analysis has a adapt image, associated the model galaxy images of this dataset to the galaxies in
            the model instance.
 
         2) Extract attributes which model aspects of the data reductions, like the scaling the background sky
            and background noise.
 
-        3) Extracts all galaxies from the model instance and set up a `Plane`.
+        3) Extracts all galaxies from the model instance.
 
-        4) Use the `Plane` and other attributes to create a `FitImaging` object, which performs steps such as creating
-           model images of every galaxy in the plane, blurring them with the imaging dataset's PSF and computing residuals,
+        4) Use the galaxies and other attributes to create a `FitImaging` object, which performs steps such as creating
+           model images of every galaxy, blurring them with the imaging dataset's PSF and computing residuals,
            a chi-squared statistic and the log likelihood.
 
         Certain models will fail to fit the dataset and raise an exception. For example if an `Inversion` is used, the
         linear algebra calculation may be invalid and raise an Exception. In such circumstances the model is discarded
         and its likelihood value is passed to the non-linear search in a way that it ignores it (for example, using a
         value of -1.0e99).
 
@@ -165,155 +166,45 @@
             If a `Preload` object is input this is used instead of the preloads stored as an attribute in the analysis.
         run_time_dict
             A dictionary which times functions called to fit the model to data, for profiling.
 
         Returns
         -------
         FitImaging
-            The fit of the plane to the imaging dataset, which includes the log likelihood.
+            The fit of the galaxies to the imaging dataset, which includes the log likelihood.
         """
-        plane = self.plane_via_instance_from(
+
+        galaxies = self.galaxies_via_instance_from(
             instance=instance, run_time_dict=run_time_dict
         )
 
+        dataset_model = self.dataset_model_via_instance_from(instance=instance)
+
         adapt_images = self.adapt_images_via_instance_from(instance=instance)
 
         preloads = self.preloads if preload_overwrite is None else preload_overwrite
 
         return FitImaging(
             dataset=self.dataset,
-            plane=plane,
+            galaxies=galaxies,
+            dataset_model=dataset_model,
             adapt_images=adapt_images,
             settings_inversion=self.settings_inversion,
             preloads=preloads,
             run_time_dict=run_time_dict,
         )
 
-    def visualize_before_fit(self, paths: af.DirectoryPaths, model: af.Collection):
-        """
-        PyAutoFit calls this function immediately before the non-linear search begins.
-
-        It visualizes objects which do not change throughout the model fit like the dataset.
-
-        Parameters
-        ----------
-        paths
-            The PyAutoFit paths object which manages all paths, e.g. where the non-linear search outputs are stored,
-            visualization and the pickled objects used by the aggregator output by this function.
-        model
-            The PyAutoFit model object, which includes model components representing the galaxies that are fitted to
-            the imaging data.
-        """
-
-        visualizer = VisualizerImaging(visualize_path=paths.image_path)
-
-        visualizer.visualize_imaging(dataset=self.dataset)
-
-        if self.adapt_images is not None:
-            visualizer.visualize_adapt_images(adapt_images=self.adapt_images)
-
-    def visualize(
-        self,
-        paths: af.DirectoryPaths,
-        instance: af.ModelInstance,
-        during_analysis: bool,
-    ):
-        """
-        Output images of the maximum log likelihood model inferred by the model-fit. This function is called throughout
-        the non-linear search at regular intervals, and therefore provides on-the-fly visualization of how well the
-        model-fit is going.
-
-        The visualization performed by this function includes:
-
-        - Images of the best-fit `Plane`, including the images of each of its galaxies.
-
-        - Images of the best-fit `FitImaging`, including the model-image, residuals and chi-squared of its fit to
-          the imaging data.
-
-        - The adapt-images of the model-fit showing how the galaxies are used to represent different galaxies in
-          the dataset.
-
-        The images output by this function are customized using the file `config/visualize/plots.ini`.
-
-        Parameters
-        ----------
-        paths
-            The PyAutoFit paths object which manages all paths, e.g. where the non-linear search outputs are stored,
-            visualization, and the pickled objects used by the aggregator output by this function.
-        instance
-            An instance of the model that is being fitted to the data by this analysis (whose parameters have been set
-            via a non-linear search).
-        during_analysis
-            If True the visualization is being performed midway through the non-linear search before it is finished,
-            which may change which images are output.
-        """
-        fit = self.fit_from(instance=instance)
-
-        visualizer = VisualizerImaging(visualize_path=paths.image_path)
-        visualizer.visualize_imaging(dataset=self.dataset)
-
-        try:
-            visualizer.visualize_fit_imaging(fit=fit, during_analysis=during_analysis)
-        except exc.InversionException:
-            pass
-
-        plane = fit.plane_linear_light_profiles_to_light_profiles
-
-        visualizer.visualize_plane(
-            plane=plane, grid=fit.grid, during_analysis=during_analysis
-        )
-        visualizer.visualize_galaxies(
-            galaxies=plane.galaxies, grid=fit.grid, during_analysis=during_analysis
-        )
-        if fit.inversion is not None:
-            visualizer.visualize_inversion(
-                inversion=fit.inversion, during_analysis=during_analysis
-            )
-
-    def make_result(
-        self,
-        samples: af.SamplesPDF,
-    ) -> ResultImaging:
-        """
-        After the non-linear search is complete create its `Result`, which includes:
-
-        - The samples of the non-linear search (E.g. MCMC chains, nested sampling samples) which are used to compute
-          the maximum likelihood model, posteriors and other properties.
-
-        - The model used to fit the data, which uses the samples to create specific instances of the model (e.g.
-          an instance of the maximum log likelihood model).
-
-        - The non-linear search used to perform the model fit.
-
-        The `ResultImaging` object contains a number of methods which use the above objects to create the max
-        log likelihood `Plane`, `FitImaging`, adapt-galaxy images,etc.
-
-        Parameters
-        ----------
-        samples
-            A PyAutoFit object which contains the samples of the non-linear search, for example the chains of an MCMC
-            run of samples of the nested sampler.
-        search
-            The non-linear search used to perform this model-fit.
-
-        Returns
-        -------
-        ResultImaging
-            The result of fitting the model to the imaging dataset, via a non-linear search.
-        """
-        return ResultImaging(samples=samples, analysis=self)
-
     def save_attributes(self, paths: af.DirectoryPaths):
         """
          Before the non-linear search begins, this routine saves attributes of the `Analysis` object to the `pickles`
          folder such that they can be loaded after the analysis using PyAutoFit's database and aggregator tools.
 
          For this analysis, it uses the `AnalysisDataset` object's method to output the following:
 
-         - The imaging dataset (data / noise-map / settings / psf / etc.).
+         - The imaging dataset (data / noise-map / psf / over sampler / etc.).
          - The mask applied to the dataset.
          - The settings associated with the inversion.
          - The settings associated with the pixelization.
          - The Cosmology.
          - The adapt image's model image and galaxy images, if used.
 
          This function also outputs attributes specific to an imaging dataset:
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/imaging/model/result.py` & `autogalaxy-2024.5.16.0/autogalaxy/interferometer/model/result.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,76 +1,63 @@
-from typing import List
-
 import autoarray as aa
 
-from autogalaxy.analysis.result import ResultDataset
-from autogalaxy.plane.plane import Plane
-from autogalaxy.imaging.fit_imaging import FitImaging
+from typing import List
 
+from autogalaxy.analysis.adapt_images.adapt_images import AdaptImages
+from autogalaxy.analysis.result import ResultDataset
+from autogalaxy.galaxy.galaxy import Galaxy
+from autogalaxy.interferometer.fit_interferometer import FitInterferometer
 
-class ResultImaging(ResultDataset):
-    """
-    After the non-linear search of a fit to an imaging dataset is complete it creates this `ResultImaging`, object
-    which includes:
-
-    - The samples of the non-linear search (E.g. MCMC chains, nested sampling samples) which are used to compute
-    the maximum likelihood model, posteriors and other properties.
-
-    - The model used to fit the data, which uses the samples to create specific instances of the model (e.g.
-    an instance of the maximum log likelihood model).
-
-    - The non-linear search used to perform the model fit.
-
-    This class contains a number of methods which use the above objects to create the max log likelihood `Plane`,
-    `FitImaging`, adapt-galaxy images,etc.
-
-    Parameters
-    ----------
-    samples
-        A PyAutoFit object which contains the samples of the non-linear search, for example the chains of an MCMC
-        run of samples of the nested sampler.
-    model
-        The PyAutoFit model object, which includes model components representing the galaxies that are fitted to
-        the imaging data.
-    search
-        The non-linear search used to perform this model-fit.
-
-    Returns
-    -------
-    ResultImaging
-        The result of fitting the model to the imaging dataset, via a non-linear search.
-    """
 
+class ResultInterferometer(ResultDataset):
     @property
-    def max_log_likelihood_fit(self) -> FitImaging:
+    def max_log_likelihood_fit(self) -> FitInterferometer:
         """
-        An instance of a `FitImaging` corresponding to the maximum log likelihood model inferred by the non-linear
-        search.
+        An instance of a `FitInterferometer` corresponding to the maximum log likelihood model inferred by the
+        non-linear search.
         """
         return self.analysis.fit_from(instance=self.instance)
 
     @property
-    def max_log_likelihood_plane(self) -> Plane:
+    def max_log_likelihood_galaxies(self) -> List[Galaxy]:
         """
-        An instance of a `Plane` corresponding to the maximum log likelihood model inferred by the non-linear search.
+        An instance of the galaxies corresponding to the maximum log likelihood model inferred by the non-linear search.
 
-        The `Plane` is computed from the `max_log_likelihood_fit`, as this ensures that all linear light profiles
+        The galaxies are computed from the `max_log_likelihood_fit`, as this ensures that all linear light profiles
         are converted to normal light profiles with their `intensity` values updated.
         """
         return (
             self.max_log_likelihood_fit.model_obj_linear_light_profiles_to_light_profiles
         )
 
     @property
-    def unmasked_model_image(self) -> aa.Array2D:
+    def real_space_mask(self) -> aa.Mask2D:
         """
-        The model image of the maximum log likelihood model, creating without using a mask.
+        The real space mask used by this model-fit.
         """
-        return self.max_log_likelihood_fit.unmasked_blurred_image
+        return self.max_log_likelihood_fit.dataset.real_space_mask
 
-    @property
-    def unmasked_model_image_of_galaxies(self) -> List[aa.Array2D]:
+    def adapt_images_from(self, use_model_images: bool = False) -> AdaptImages:
         """
-        A list of the model image of every galaxy in the maximum log likelihood model, whereas all images are created
-        without using a mask.
+        Returns the adapt-images which are used to make a pixelization's mesh and regularization adapt to the
+        reconstructed galaxy's morphology.
+
+        This can use either:
+
+        - The model image of each galaxy in the best-fit model.
+        - The subtracted image of each galaxy in the best-fit model, where the subtracted image is the dataset
+          minus the model images of all other galaxies.
+
+        In **PyAutoLens** these adapt images have had lensing calculations performed on them and therefore for source
+        galaxies are their lensed model images in the image-plane.
+
+        Parameters
+        ----------
+        use_model_images
+            If True, the model images of the galaxies are used to create the adapt images. If False, the subtracted
+            images of the galaxies are used.
         """
-        return self.max_log_likelihood_fit.unmasked_blurred_image_of_galaxies_list
+
+        return AdaptImages.from_result(
+            result=self,
+            use_model_images=True,
+        )
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/imaging/plot/fit_imaging_plotters.py` & `autogalaxy-2024.5.16.0/autogalaxy/imaging/plot/fit_imaging_plotters.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import List, Optional
 
 import autoarray as aa
 import autoarray.plot as aplt
 
 from autoarray.fit.plot.fit_imaging_plotters import FitImagingPlotterMeta
 
-from autogalaxy.plane.plane import Plane
+from autogalaxy.galaxy.galaxy import Galaxy
 from autogalaxy.imaging.fit_imaging import FitImaging
 from autogalaxy.plot.abstract_plotters import Plotter
 from autogalaxy.plot.mat_plot.two_d import MatPlot2D
 from autogalaxy.plot.visuals.two_d import Visuals2D
 from autogalaxy.plot.include.two_d import Include2D
 
 
@@ -84,47 +84,46 @@
             inversion=self.fit.inversion,
             mat_plot_2d=self.mat_plot_2d,
             visuals_2d=self.get_visuals_2d(),
             include_2d=self.include_2d,
         )
 
     @property
-    def plane(self) -> Plane:
-        return self.fit.plane_linear_light_profiles_to_light_profiles
+    def galaxies(self) -> List[Galaxy]:
+        return self.fit.galaxies_linear_light_profiles_to_light_profiles
 
     @property
     def galaxy_indices(self) -> List[int]:
         """
         Returns a list of all indexes of the galaxies in the fit, which is iterated over in figures that plot
-        individual figures of each galaxy in a plane.
-
+        individual figures of each galaxy.
 
         Parameters
         ----------
         galaxy_index
             A specific galaxy index such that only a single galaxy index is returned.
 
         Returns
         -------
         list
-            A list of galaxy indexes corresponding to galaxies in the plane.
+            A list of galaxy indexes corresponding to the galaxies.
         """
         return list(range(len(self.fit.galaxies)))
 
     def figures_2d_of_galaxies(
         self,
         galaxy_index: Optional[int] = None,
         subtracted_image: bool = False,
         model_image: bool = False,
     ):
         """
-        Plots images representing each individual `Galaxy` in the plotter's `Plane` in 2D, which are computed via the
-        plotter's 2D grid object.
+        Plots images representing each individual `Galaxy` in the plotter's list of galaxies in 2D, which are
+        computed via the plotter's 2D grid object.
 
-        These images subtract or omit the contribution of other galaxies in the plane, such that plots showing
+        These images subtract or omit the contribution of other galaxies, such that plots showing
         each individual galaxy are made.
 
         The API is such that every plottable attribute of the `Galaxy` object is an input parameter of type bool of
         the function, which if switched to `True` means that it is plotted.
 
         Parameters
         ----------
@@ -132,15 +131,15 @@
             Whether to make a 2D plot (via `imshow`) of the subtracted image of a galaxy, where this image is
             the fit's `data` minus the model images of all other galaxies, thereby showing an individual galaxy in the
             data.
         model_image
             Whether to make a 2D plot (via `imshow`) of the model image of a galaxy, where this image is the
             model image of one galaxy, thereby showing how much it contributes to the overall model image.
         galaxy_index
-            If input, plots for only a single galaxy based on its index in the plane are created.
+            If input, plots for only a single galaxy based on its index are created.
         """
         if galaxy_index is None:
             galaxy_indices = self.galaxy_indices
         else:
             galaxy_indices = [galaxy_index]
 
         for galaxy_index in galaxy_indices:
@@ -197,27 +196,27 @@
         self.figures_2d(chi_squared_map=True)
 
         self.mat_plot_2d.output.subplot_to_figure(auto_filename="subplot_fit")
         self.close_subplot_figure()
 
     def subplot_of_galaxies(self, galaxy_index: Optional[int] = None):
         """
-        Plots images representing each individual `Galaxy` in the plotter's `Plane` in 2D on a subplot, which are
-        computed via the plotter's 2D grid object.
+        Plots images representing each individual `Galaxy` in the plotter's list of galaxies in 2D on a subplot,
+        which are computed via the plotter's 2D grid object.
 
-        These images subtract or omit the contribution of other galaxies in the plane, such that plots showing
-        each individual galaxy are made.
+        These images subtract or omit the contribution of other galaxies, such that plots showing each individual
+        galaxy are made.
 
         The subplot plots the subtracted image and model image of each galaxy, where are described in the
         `figures_2d_of_galaxies` function.
 
         Parameters
         ----------
         galaxy_index
-            If input, plots for only a single galaxy based on its index in the plane are created.
+            If input, plots for only a single galaxy based on its index are created.
         """
 
         if galaxy_index is None:
             galaxy_indices = self.galaxy_indices
         else:
             galaxy_indices = [galaxy_index]
 
@@ -226,15 +225,15 @@
 
             self.figures_2d(data=True)
             self.figures_2d_of_galaxies(
                 galaxy_index=galaxy_index, subtracted_image=True
             )
             self.figures_2d_of_galaxies(galaxy_index=galaxy_index, model_image=True)
 
-            if self.plane.has(cls=aa.Pixelization):
+            if self.galaxies.has(cls=aa.Pixelization):
                 self.inversion_plotter.figures_2d_of_pixelization(
                     pixelization_index=0, reconstruction=True
                 )
 
             self.mat_plot_2d.output.subplot_to_figure(
                 auto_filename=f"subplot_of_galaxy_{galaxy_index}"
             )
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/interferometer/fit_interferometer.py` & `autogalaxy-2024.5.16.0/autogalaxy/interferometer/fit_interferometer.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,44 +2,45 @@
 from typing import Dict, List, Optional
 
 from autoconf import cached_property
 
 import autoarray as aa
 
 from autogalaxy.abstract_fit import AbstractFitInversion
-from autogalaxy.analysis.adapt_images import AdaptImages
+from autogalaxy.analysis.adapt_images.adapt_images import AdaptImages
 from autogalaxy.analysis.preloads import Preloads
 from autogalaxy.galaxy.galaxy import Galaxy
-from autogalaxy.plane.plane import Plane
-from autogalaxy.plane.to_inversion import PlaneToInversion
+from autogalaxy.galaxy.galaxies import Galaxies
+from autogalaxy.galaxy.to_inversion import GalaxiesToInversion
 
 
 class FitInterferometer(aa.FitInterferometer, AbstractFitInversion):
     def __init__(
         self,
         dataset: aa.Interferometer,
-        plane: Plane,
+        galaxies: List[Galaxy],
+        dataset_model: Optional[aa.DatasetModel] = None,
         adapt_images: Optional[AdaptImages] = None,
         settings_inversion: aa.SettingsInversion = aa.SettingsInversion(),
         preloads: aa.Preloads = Preloads(),
         run_time_dict: Optional[Dict] = None,
     ):
         """
-        Fits an interferometer dataset using a `Plane` object.
+        Fits an interferometer dataset using a list of galaxies.
 
         The fit performs the following steps:
 
-        1) Compute the sum of all images of galaxy light profiles in the `Plane`.
+        1) Compute the sum of all images of galaxy light profiles.
 
         2) Fourier transform this image with the transformer object and `uv_wavelengths` to create
            the `profile_visibilities`.
 
         3) Subtract these visibilities from the `data` to create the `profile_subtracted_visibilities`.
 
-        4) If the `Plane` has any linear algebra objects (e.g. linear light profiles, a pixelization / regulariation)
+        4) If the galaxies have any linear algebra objects (e.g. linear light profiles, a pixelization / regulariation)
            fit the `profile_subtracted_visibilities` with these objects via an inversion.
 
         5) Compute the `model_data` as the sum of the `profile_visibilities` and `reconstructed_data` of the inversion
            (if an inversion is not performed the `model_data` is only the `profile_visibilities`.
 
         6) Subtract the `model_data` from the data and compute the residuals, chi-squared and likelihood via the
            noise-map (if an inversion is performed the `log_evidence`, including addition terms describing the linear
@@ -47,17 +48,19 @@
 
         When performing a model-fit` via ` AnalysisInterferometer` object the `figure_of_merit` of
         this `FitInterferometer` object is called and returned in the `log_likelihood_function`.
 
         Parameters
         ----------
         dataset
-            The interfometer dataset which is fitted by the galaxies in the plane.
-        plane
-            The plane of galaxies whose light profile images are used to fit the interferometer data.
+            The interfometer dataset which is fitted by the galaxies.
+        galaxies
+            The galaxies whose light profile images are used to fit the interferometer data.
+        dataset_model
+            Attributes which allow for parts of a dataset to be treated as a model (e.g. the background sky level).
         adapt_images
             Contains the adapt-images which are used to make a pixelization's mesh and regularization adapt to the
             reconstructed galaxy's morphology.
         settings_inversion
             Settings controlling how an inversion is fitted for example which linear algebra formalism is used.
         preloads
             Contains preloaded calculations (e.g. linear algebra matrices) which can skip certain calculations in
@@ -68,193 +71,198 @@
         """
 
         try:
             from autoarray.inversion.inversion import inversion_util_secret
         except ImportError:
             settings_inversion.use_w_tilde = False
 
+        self.galaxies = Galaxies(galaxies=galaxies, run_time_dict=run_time_dict)
+
         super().__init__(
-            dataset=dataset, use_mask_in_fit=False, run_time_dict=run_time_dict
+            dataset=dataset,
+            dataset_model=dataset_model,
+            use_mask_in_fit=False,
+            run_time_dict=run_time_dict,
         )
         AbstractFitInversion.__init__(
-            self=self, model_obj=plane, settings_inversion=settings_inversion
+            self=self,
+            model_obj=self.galaxies,
+            settings_inversion=settings_inversion,
         )
 
-        self.plane = plane
-
         self.adapt_images = adapt_images
         self.settings_inversion = settings_inversion
 
         self.preloads = preloads
 
     @property
     def profile_visibilities(self) -> aa.Visibilities:
         """
-        Returns the visibilities of every light profile of every galaxy in the plane, which are computed by performing
+        Returns the visibilities of every light profile of every galaxy, which are computed by performing
         a Fourier transform to the sum of light profile images.
         """
-        return self.plane.visibilities_from(
-            grid=self.dataset.grid, transformer=self.dataset.transformer
+        return self.galaxies.visibilities_from(
+            grid=self.grid, transformer=self.dataset.transformer
         )
 
     @property
     def profile_subtracted_visibilities(self) -> aa.Visibilities:
         """
-        Returns the interferometer dataset's visibilities with all transformed light profile images in the fit's
-        plane subtracted.
+        Returns the interferometer dataset's visibilities with all transformed light profile images subtracted.
         """
-        return self.visibilities - self.profile_visibilities
+        return self.data - self.profile_visibilities
 
     @property
-    def plane_to_inversion(self) -> PlaneToInversion:
-        return PlaneToInversion(
-            plane=self.plane,
-            dataset=self.dataset,
+    def galaxies_to_inversion(self) -> GalaxiesToInversion:
+        dataset = aa.DatasetInterface(
             data=self.profile_subtracted_visibilities,
             noise_map=self.noise_map,
+            transformer=self.dataset.transformer,
             w_tilde=self.w_tilde,
+            grid=self.grid,
+            grid_pixelization=self.grid_pixelization,
+            border_relocator=self.dataset.border_relocator,
+        )
+
+        return GalaxiesToInversion(
+            dataset=dataset,
+            galaxies=self.galaxies,
             adapt_images=self.adapt_images,
             settings_inversion=self.settings_inversion,
             preloads=self.preloads,
+            run_time_dict=self.run_time_dict,
         )
 
     @cached_property
     def inversion(self) -> Optional[aa.AbstractInversion]:
         """
-        If the plane has linear objects which are used to fit the data (e.g. a linear light profile / pixelization)
+        If the galaxies have linear objects which are used to fit the data (e.g. a linear light profile / pixelization)
         this function returns a linear inversion, where the flux values of these objects (e.g. the `intensity`
         of linear light profiles) are computed via linear matrix algebra.
 
-        The data passed to this function is the dataset's visibilities with all light profile visibilities of the
-        plane subtracted.
+        The data passed to this function is the dataset's visibilities with all light profile visibilities subtracted.
         """
         if self.perform_inversion:
-            return self.plane_to_inversion.inversion
+            return self.galaxies_to_inversion.inversion
 
     @property
     def model_data(self) -> aa.Visibilities:
         """
         Returns the model data that is used to fit the data.
 
-        If the plane does not have any linear objects and therefore omits an inversion, the model data is the
+        If the galaxies do not have any linear objects and therefore omits an inversion, the model data is the
         sum of all light profile images Fourier transformed to visibilities.
 
         If a inversion is included it is the sum of these visibilities and the inversion's reconstructed visibilities.
         """
 
         if self.perform_inversion:
             return self.profile_visibilities + self.inversion.mapped_reconstructed_data
 
         return self.profile_visibilities
 
     @property
-    def grid(self) -> aa.Grid2D:
-        return self.dataset.grid
-
-    @property
-    def galaxies(self) -> List[Galaxy]:
-        return self.plane.galaxies
-
-    @property
     def galaxy_model_image_dict(self) -> Dict[Galaxy, np.ndarray]:
         """
-        A dictionary which associates every galaxy in the plane with its `image`.
+        A dictionary which associates every galaxy with its `image`.
 
-        This image is the image of the sum of:
+        This image is the sum of:
 
-        - The images of all ordinary light profiles in that plane summed.
+        - The images of all ordinary light profiles summed.
         - The images of all linear objects (e.g. linear light profiles / pixelizations), where the images are solved
           for first via the inversion.
 
         For modeling, this dictionary is used to set up the `adapt_images` that adapt certain pixelizations to the
         data being fitted.
         """
-        galaxy_model_image_dict = self.plane.galaxy_image_2d_dict_from(grid=self.grid)
+        galaxy_model_image_dict = self.galaxies.galaxy_image_2d_dict_from(
+            grid=self.grid
+        )
 
         galaxy_linear_obj_image_dict = self.galaxy_linear_obj_data_dict_from(
             use_image=True
         )
 
         return {**galaxy_model_image_dict, **galaxy_linear_obj_image_dict}
 
     @property
     def galaxy_model_visibilities_dict(self) -> Dict[Galaxy, np.ndarray]:
         """
-        A dictionary which associates every galaxy in the plane with its model visibilities.
+        A dictionary which associates every galaxy with its model visibilities.
 
         These visibilities are the sum of:
 
-        - The visibilities of all ordinary light profiles in that plane summed and Fourier transformed to visibilities
-          space.
+        - The visibilities of all ordinary light profiles summed and Fourier transformed to visibilities space.
         - The visibilities of all linear objects (e.g. linear light profiles / pixelizations), where the visibilities
           are solved for first via the inversion.
 
         For modeling, this dictionary is used to set up the `adapt_visibilities` that adapt certain pixelizations to the
         data being fitted.
         """
-        galaxy_model_visibilities_dict = self.plane.galaxy_visibilities_dict_from(
-            grid=self.dataset.grid, transformer=self.dataset.transformer
+        galaxy_model_visibilities_dict = self.galaxies.galaxy_visibilities_dict_from(
+            grid=self.grid, transformer=self.dataset.transformer
         )
 
         galaxy_linear_obj_data_dict = self.galaxy_linear_obj_data_dict_from(
             use_image=False
         )
 
         return {**galaxy_model_visibilities_dict, **galaxy_linear_obj_data_dict}
 
     @property
     def model_visibilities_of_galaxies_list(self) -> List:
         """
-        A list of the model visibilities of each galaxy in the plane.
+        A list of the model visibilities of each galaxy.
         """
         return list(self.galaxy_model_visibilities_dict.values())
 
     @property
-    def plane_linear_light_profiles_to_light_profiles(self) -> Plane:
+    def galaxies_linear_light_profiles_to_light_profiles(self) -> List[Galaxy]:
         """
-        The `Plane` where all linear light profiles have been converted to ordinary light profiles, where their
+        The galaxies where all linear light profiles have been converted to ordinary light profiles, where their
         `intensity` values are set to the values inferred by this fit.
 
         This is typically used for visualization, because linear light profiles cannot be used in `LightProfilePlotter`
         or `GalaxyPlotter` objects.
         """
         return self.model_obj_linear_light_profiles_to_light_profiles
 
     def refit_with_new_preloads(
         self,
         preloads: Preloads,
         settings_inversion: Optional[aa.SettingsInversion] = None,
     ) -> "FitInterferometer":
         """
-        Returns a new fit which uses the dataset, plane and other objects of this fit, but uses a different set of
+        Returns a new fit which uses the dataset, galaxies and other objects of this fit, but uses a different set of
         preloads input into this function.
 
         This is used when setting up the preloads objects, to concisely test how using different preloads objects
         changes the attributes of the fit.
 
         Parameters
         ----------
         preloads
             The new preloads which are used to refit the data using the
         settings_inversion
             Settings controlling how an inversion is fitted for example which linear algebra formalism is used.
 
         Returns
         -------
-        A new fit which has used new preloads input into this function but the same dataset, plane and other settings.
+        A new fit which has used new preloads input into this function but the same dataset, galaxies and other settings.
         """
         if self.run_time_dict is not None:
             run_time_dict = {}
         else:
             run_time_dict = None
 
         if settings_inversion is None:
             settings_inversion = self.settings_inversion
 
         return FitInterferometer(
-            dataset=self.interferometer,
-            plane=self.plane,
+            dataset=self.dataset,
+            galaxies=self.galaxies,
+            dataset_model=self.dataset_model,
             adapt_images=self.adapt_images,
             settings_inversion=settings_inversion,
             preloads=preloads,
             run_time_dict=run_time_dict,
         )
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/interferometer/model/analysis.py` & `autogalaxy-2024.5.16.0/autogalaxy/interferometer/model/analysis.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,72 +1,74 @@
 import logging
 import numpy as np
 from typing import Dict, Optional, Tuple
 
+from autoconf.dictable import to_dict
+
 import autofit as af
 import autoarray as aa
 
 from autoarray.exc import PixelizationException
 
-from autogalaxy.analysis.adapt_images import AdaptImages
-from autogalaxy.analysis.analysis import AnalysisDataset
+from autogalaxy.analysis.adapt_images.adapt_image_maker import AdaptImageMaker
+from autogalaxy.analysis.analysis.dataset import AnalysisDataset
 from autogalaxy.analysis.preloads import Preloads
 from autogalaxy.cosmology.lensing import LensingCosmology
 from autogalaxy.cosmology.wrap import Planck15
 from autogalaxy.interferometer.model.result import ResultInterferometer
-from autogalaxy.interferometer.model.visualizer import VisualizerInterferometer
 from autogalaxy.interferometer.fit_interferometer import FitInterferometer
-from autogalaxy.plane.plane import Plane
-
+from autogalaxy.interferometer.model.visualizer import VisualizerInterferometer
 from autogalaxy import exc
 
 logger = logging.getLogger(__name__)
 
 logger.setLevel(level="INFO")
 
 
 class AnalysisInterferometer(AnalysisDataset):
+    Result = ResultInterferometer
+    Visualizer = VisualizerInterferometer
+
     def __init__(
         self,
         dataset: aa.Interferometer,
-        adapt_images: Optional[AdaptImages] = None,
+        adapt_image_maker: Optional[AdaptImageMaker] = None,
         cosmology: LensingCosmology = Planck15(),
         settings_inversion: aa.SettingsInversion = None,
     ):
         """
         Fits a galaxy model to an interferometer dataset via a non-linear search.
 
         The `Analysis` class defines the `log_likelihood_function` which fits the model to the dataset and returns the
         log likelihood value defining how well the model fitted the data.
 
         It handles many other tasks, such as visualization, outputting results to hard-disk and storing results in
         a format that can be loaded after the model-fit is complete.
 
-        This Analysis class is used for all model-fits which fit galaxies (or objects containing galaxies like a
-        `Plane`) to an interferometer dataset.
+        This Analysis class is used for all model-fits which fit galaxies to an interferometer dataset.
 
         This class stores the settings used to perform the model-fit for certain components of the model (e.g. a
         pixelization or inversion), the Cosmology used for the analysis and adapt images used for certain model
         classes.
 
         Parameters
         ----------
         dataset
             The interferometer dataset that the model is fitted too.
-        adapt_images
-            The adapt-model image and galaxies images of a previous result in a model-fitting pipeline, which are
+        adapt_image_maker
+            Makes the adapt-model image and galaxies images of a previous result in a model-fitting pipeline, which are
             used by certain classes for adapting the analysis to the properties of the dataset.
         cosmology
             The Cosmology assumed for this analysis.
         settings_inversion
             Settings controlling how an inversion is fitted, for example which linear algebra formalism is used.
         """
         super().__init__(
             dataset=dataset,
-            adapt_images=adapt_images,
+            adapt_image_maker=adapt_image_maker,
             cosmology=cosmology,
             settings_inversion=settings_inversion,
         )
 
     @property
     def interferometer(self):
         return self.dataset
@@ -111,18 +113,18 @@
         For this analysis class, this function performs the following steps:
 
         1) If the analysis has a adapt image, associated the model galaxy images of this dataset to the galaxies in
            the model instance.
 
         2) Extract attributes which model aspects of the data reductions, like scaling the background background noise.
 
-        3) Extracts all galaxies from the model instance and set up a `Plane`.
+        3) Extracts all galaxies from the model instance.
 
-        4) Use the `Plane` and other attributes to create a `FitInterferometer` object, which performs steps such as
-           creating model images of every galaxy in the plane, transforming them to the uv-plane via a Fourier transform
+        4) Use the galaxies and other attributes to create a `FitInterferometer` object, which performs steps such as
+           creating model images of every galaxy, transforming them to the uv-plane via a Fourier transform
            and computing residuals, a chi-squared statistic and the log likelihood.
 
         Certain models will fail to fit the dataset and raise an exception. For example if an `Inversion` is used, the
         linear algebra calculation may be invalid and raise an Exception. In such circumstances the model is discarded
         and its likelihood value is passed to the non-linear search in a way that it ignores it (for example, using a
         value of -1.0e99).
 
@@ -172,151 +174,33 @@
             If a `Preload` object is input this is used instead of the preloads stored as an attribute in the analysis.
         run_time_dict
             A dictionary which times functions called to fit the model to data, for profiling.
 
         Returns
         -------
         FitInterferometer
-            The fit of the plane to the interferometer dataset, which includes the log likelihood.
+            The fit of the galaxies to the interferometer dataset, which includes the log likelihood.
         """
-        plane = self.plane_via_instance_from(
+        galaxies = self.galaxies_via_instance_from(
             instance=instance, run_time_dict=run_time_dict
         )
 
         adapt_images = self.adapt_images_via_instance_from(instance=instance)
 
         preloads = self.preloads if preload_overwrite is None else preload_overwrite
 
         return FitInterferometer(
             dataset=self.dataset,
-            plane=plane,
+            galaxies=galaxies,
             adapt_images=adapt_images,
             settings_inversion=self.settings_inversion,
             preloads=preloads,
             run_time_dict=run_time_dict,
         )
 
-    def visualize_before_fit(self, paths: af.DirectoryPaths, model: af.Collection):
-        """
-        PyAutoFit calls this function immediately before the non-linear search begins.
-
-        It visualizes objects which do not change throughout the model fit like the dataset.
-
-        Parameters
-        ----------
-        paths
-            The PyAutoFit paths object which manages all paths, e.g. where the non-linear search outputs are stored,
-            visualization and the pickled objects used by the aggregator output by this function.
-        model
-            The PyAutoFit model object, which includes model components representing the galaxies that are fitted to
-            the imaging data.
-        """
-
-        visualizer = VisualizerInterferometer(visualize_path=paths.image_path)
-
-        visualizer.visualize_interferometer(dataset=self.interferometer)
-
-        if self.adapt_images is not None:
-            visualizer.visualize_adapt_images(adapt_images=self.adapt_images)
-
-    def visualize(self, paths: af.DirectoryPaths, instance, during_analysis):
-        """
-        Outputs images of the maximum log likelihood model inferred by the model-fit. This function is called
-        throughout the non-linear search at input intervals, and therefore provides on-the-fly visualization of how
-        well the model-fit is going.
-
-        The visualization performed by this function includes:
-
-        - Images of the best-fit `Plane`, including the images of each of its galaxies.
-
-        - Images of the best-fit `FitInterferometer`, including the model-image, residuals and chi-squared of its fit
-          to the imaging data.
-
-        - The adapt-images of the model-fit showing how the galaxies are used to represent different galaxies in
-          the dataset.
-
-        - If adapt features are used to scale the noise, a `FitInterferometer` with these features turned off may be
-          output, to indicate how much these features are altering the dataset.
-
-        The images output by this function are customized using the file `config/visualize/plots.ini`.
-
-        Parameters
-        ----------
-        paths
-            The PyAutoFit paths object which manages all paths, e.g. where the non-linear search outputs are stored,
-            visualization, and the pickled objects used by the aggregator output by this function.
-        instance
-            An instance of the model that is being fitted to the data by this analysis (whose parameters have been set
-            via a non-linear search).
-        during_analysis
-            If True the visualization is being performed midway through the non-linear search before it is finished,
-            which may change which images are output.
-        """
-        fit = self.fit_from(instance=instance)
-
-        visualizer = VisualizerInterferometer(visualize_path=paths.image_path)
-        visualizer.visualize_interferometer(dataset=self.interferometer)
-
-        plane = fit.plane_linear_light_profiles_to_light_profiles
-
-        visualizer.visualize_plane(
-            plane=plane, grid=fit.grid, during_analysis=during_analysis
-        )
-        visualizer.visualize_galaxies(
-            galaxies=plane.galaxies, grid=fit.grid, during_analysis=during_analysis
-        )
-
-        try:
-            visualizer.visualize_fit_interferometer(
-                fit=fit, during_analysis=during_analysis
-            )
-        except exc.InversionException:
-            pass
-
-        if fit.inversion is not None:
-            try:
-                visualizer.visualize_inversion(
-                    inversion=fit.inversion, during_analysis=during_analysis
-                )
-            except IndexError:
-                pass
-
-    def make_result(
-        self,
-        samples: af.SamplesPDF,
-    ) -> ResultInterferometer:
-        """
-        After the non-linear search is complete create its `Result`, which includes:
-
-        - The samples of the non-linear search (E.g. MCMC chains, nested sampling samples) which are used to compute
-          the maximum likelihood model, posteriors and other properties.
-
-        - The model used to fit the data, which uses the samples to create specific instances of the model (e.g.
-          an instance of the maximum log likelihood model).
-
-        - The non-linear search used to perform the model fit.
-
-        The `ResultInterferometer` object contains a number of methods which use the above objects to create the max
-        log likelihood `Plane`, `FitInterferometer`, adapt-galaxy images,etc.
-
-        Parameters
-        ----------
-        samples
-            A PyAutoFit object which contains the samples of the non-linear search, for example the chains of an MCMC
-            run of samples of the nested sampler.
-        search
-            The non-linear search used to perform this model-fit.
-
-        Returns
-        -------
-        ResultInterferometer
-            The result of fitting the model to the interferometer dataset, via a non-linear search.
-        """
-        return ResultInterferometer(samples=samples, analysis=self)
-
     def save_attributes(self, paths: af.DirectoryPaths):
         """
          Before the model-fit begins, this routine saves attributes of the `Analysis` object to the `pickles` folder
          such that they can be loaded after the analysis using PyAutoFit's database and aggregator tools.
 
          For this analysis, it uses the `AnalysisDataset` object's method to output the following:
 
@@ -350,14 +234,17 @@
         )
         paths.save_fits(name="uv_wavelengths", hdu=hdu, prefix="dataset")
         paths.save_fits(
             name="real_space_mask",
             hdu=self.dataset.real_space_mask.hdu_for_output,
             prefix="dataset",
         )
+        paths.save_json(
+            "transformer_class", to_dict(self.dataset.transformer.__class__), "dataset"
+        )
 
     def profile_log_likelihood_function(
         self, instance: af.ModelInstance, paths: Optional[af.DirectoryPaths] = None
     ) -> Tuple[Dict, Dict]:
         """
         This function is optionally called throughout a model-fit to profile the log likelihood function.
 
@@ -384,15 +271,15 @@
         Two dictionaries, the profiling dictionary and info dictionary, which contain the profiling times of the
         `log_likelihood_function` and information on the model and dataset used to perform the profiling.
         """
         run_time_dict, info_dict = super().profile_log_likelihood_function(
             instance=instance,
         )
 
-        info_dict["number_of_visibilities"] = self.dataset.visibilities.shape[0]
+        info_dict["number_of_visibilities"] = self.dataset.data.shape[0]
         info_dict["transformer_cls"] = self.dataset.transformer.__class__.__name__
 
         self.output_profiling_info(
             paths=paths, run_time_dict=run_time_dict, info_dict=info_dict
         )
 
         return run_time_dict, info_dict
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/interferometer/model/visualizer.py` & `autogalaxy-2024.5.16.0/autogalaxy/interferometer/model/plotter_interface.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,91 @@
 from os import path
 
+import autoarray as aa
+import autoarray.plot as aplt
+
 from autogalaxy.interferometer.fit_interferometer import FitInterferometer
 from autogalaxy.interferometer.plot.fit_interferometer_plotters import (
     FitInterferometerPlotter,
 )
-from autogalaxy.analysis.visualizer import Visualizer
+from autogalaxy.analysis.plotter_interface import PlotterInterface
+
+from autogalaxy.analysis.plotter_interface import plot_setting
+
+
+class PlotterInterfaceInterferometer(PlotterInterface):
+    def interferometer(self, dataset: aa.Interferometer):
+        """
+        Visualizes an `Interferometer` dataset object.
+
+        Images are output to the `image` folder of the `image_path` in a subfolder called `interferometer`. When
+        used with a non-linear search the `image_path` points to the search's results folder.
+
+        Visualization includes individual images of attributes of the dataset (e.g. the visibilities, noise map,
+        uv-wavelengths) and a subplot of all these attributes on the same figure.
+
+        The images output by the `PlotterInterface` are customized using the file `config/visualize/plots.yaml` under the
+        [dataset] header.
+
+        Parameters
+        ----------
+        dataset
+            The interferometer dataset whose attributes are visualized.
+        """
+
+        def should_plot(name):
+            return plot_setting(section=["dataset", "interferometer"], name=name)
+
+        mat_plot_2d = self.mat_plot_2d_from(subfolders="dataset")
 
-from autogalaxy.analysis.visualizer import plot_setting
+        dataset_plotter = aplt.InterferometerPlotter(
+            dataset=dataset,
+            include_2d=self.include_2d,
+            mat_plot_2d=mat_plot_2d,
+        )
+
+        dataset_plotter.figures_2d(
+            data=should_plot("data"),
+            u_wavelengths=should_plot("uv_wavelengths"),
+            v_wavelengths=should_plot("uv_wavelengths"),
+            amplitudes_vs_uv_distances=should_plot("amplitudes_vs_uv_distances"),
+            phases_vs_uv_distances=should_plot("phases_vs_uv_distances"),
+            dirty_image=should_plot("dirty_image"),
+            dirty_noise_map=should_plot("dirty_noise_map"),
+            dirty_signal_to_noise_map=should_plot("dirty_signal_to_noise_map"),
+        )
+
+        mat_plot_2d = self.mat_plot_2d_from(subfolders="")
+
+        dataset_plotter = aplt.InterferometerPlotter(
+            dataset=dataset,
+            include_2d=self.include_2d,
+            mat_plot_2d=mat_plot_2d,
+        )
 
+        if should_plot("subplot_dataset"):
+            dataset_plotter.subplot_dataset()
 
-class VisualizerInterferometer(Visualizer):
-    def visualize_fit_interferometer(
+    def fit_interferometer(
         self,
         fit: FitInterferometer,
         during_analysis: bool,
         subfolders: str = "fit_dataset",
     ):
         """
         Visualizes a `FitInterferometer` object, which fits an interferometer dataset.
 
-        Images are output to the `image` folder of the `visualize_path` in a subfolder called `fit`. When
-        used with a non-linear search the `visualize_path` points to the search's results folder and this function
+        Images are output to the `image` folder of the `image_path` in a subfolder called `fit`. When
+        used with a non-linear search the `image_path` points to the search's results folder and this function
         visualizes the maximum log likelihood `FitInterferometer` inferred by the search so far.
 
         Visualization includes individual images of attributes of the `FitInterferometer` (e.g. the model data,
         residual map) and a subplot of all `FitInterferometer`'s images on the same figure.
 
-        The images output by the `Visualizer` are customized using the file `config/visualize/plots.ini` under the
+        The images output by the `PlotterInterface` are customized using the file `config/visualize/plots.yaml` under the
         [fit] header.
 
         Parameters
         ----------
         fit
             The maximum log likelihood `FitInterferometer` of the non-linear search which is used to plot the fit.
         during_analysis
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/interferometer/plot/fit_interferometer_plotters.py` & `autogalaxy-2024.5.16.0/autogalaxy/interferometer/plot/fit_interferometer_plotters.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
+from typing import List
+
 import autoarray as aa
 import autoarray.plot as aplt
 
 from autoarray.fit.plot.fit_interferometer_plotters import FitInterferometerPlotterMeta
 
-from autogalaxy.plane.plane import Plane
+from autogalaxy.galaxy.galaxy import Galaxy
 from autogalaxy.interferometer.fit_interferometer import FitInterferometer
 from autogalaxy.plot.abstract_plotters import Plotter
 from autogalaxy.plot.mat_plot.one_d import MatPlot1D
 from autogalaxy.plot.mat_plot.two_d import MatPlot2D
 from autogalaxy.plot.visuals.one_d import Visuals1D
 from autogalaxy.plot.visuals.two_d import Visuals2D
 from autogalaxy.plot.include.one_d import Include1D
 from autogalaxy.plot.include.two_d import Include2D
 
-from autogalaxy.plane.plot.plane_plotters import PlanePlotter
+from autogalaxy.galaxy.plot.galaxies_plotters import GalaxiesPlotter
 
 
 class FitInterferometerPlotter(Plotter):
     def __init__(
         self,
         fit: FitInterferometer,
         mat_plot_1d: MatPlot1D = MatPlot1D(),
@@ -91,29 +93,29 @@
             self._fit_interferometer_meta_plotter.subplot_fit_dirty_images
         )
 
     def get_visuals_2d_real_space(self) -> Visuals2D:
         return self.get_2d.via_mask_from(mask=self.fit.dataset.real_space_mask)
 
     @property
-    def plane(self) -> Plane:
-        return self.fit.plane_linear_light_profiles_to_light_profiles
+    def galaxies(self) -> List[Galaxy]:
+        return self.fit.galaxies_linear_light_profiles_to_light_profiles
 
-    def plane_plotter_from(self, plane: Plane) -> PlanePlotter:
+    def galaxies_plotter_from(self, galaxies: List[Galaxy]) -> GalaxiesPlotter:
         """
-        Returns an `PlanePlotter` corresponding to an input `Plane` of the fit.
+        Returns a `GalaxiesPlotter` corresponding to an input galaxies list.
 
         Returns
         -------
-        plane
-            The plane used to make the `PlanePlotter`.
+        galaxies
+            The galaxies used to make the `GalaxiesPlotter`.
         """
-        return PlanePlotter(
-            plane=plane,
-            grid=self.fit.dataset.grid,
+        return GalaxiesPlotter(
+            galaxies=galaxies,
+            grid=self.fit.grid,
             mat_plot_2d=self.mat_plot_2d,
             visuals_2d=self.get_visuals_2d_real_space(),
             include_2d=self.include_2d,
         )
 
     @property
     def inversion_plotter(self) -> aplt.InversionPlotter:
@@ -178,25 +180,23 @@
         self.mat_plot_2d.output.subplot_to_figure(auto_filename="subplot_fit")
         self.close_subplot_figure()
 
     def subplot_fit_real_space(self):
         """
         Standard subplot of the real-space attributes of the plotter's `FitInterferometer` object.
 
-        Depending on whether `LightProfile`'s or an `Inversion` are used to represent galaxies in the `Plane`, different
+        Depending on whether `LightProfile`'s or an `Inversion` are used to represent galaxies, different
         methods are called to create these real-space images.
         """
-        if not self.plane.has(cls=aa.Pixelization):
-            plane_plotter = self.plane_plotter_from(plane=self.plane)
+        if not self.galaxies.has(cls=aa.Pixelization):
+            galaxies_plotter = self.galaxies_plotter_from(galaxies=self.galaxies)
 
-            plane_plotter.subplot(
-                image=True, plane_image=True, auto_filename="subplot_fit_real_space"
-            )
+            galaxies_plotter.subplot(image=True, auto_filename="subplot_fit_real_space")
 
-        elif self.plane.has(cls=aa.Pixelization):
+        elif self.galaxies.has(cls=aa.Pixelization):
             self.open_subplot_figure(number_subplots=6)
 
             mapper_index = 0
 
             self.inversion_plotter.figures_2d_of_pixelization(
                 pixelization_index=mapper_index, reconstructed_image=True
             )
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/operate/deflections.py` & `autogalaxy-2024.5.16.0/autogalaxy/operate/deflections.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from functools import wraps
 import logging
 import numpy as np
-from skimage import measure
 from typing import List, Tuple, Union
 
 from autoconf import conf
 
 import autoarray as aa
 
 from autogalaxy.util.shear_field import ShearYX2D
@@ -16,29 +15,25 @@
 
 def grid_scaled_2d_for_marching_squares_from(
     grid_pixels_2d: aa.Grid2D,
     shape_native: Tuple[int, int],
     mask: aa.Mask2D,
 ) -> aa.Grid2DIrregular:
     pixel_scales = mask.pixel_scales
-    sub_size = mask.sub_size
     origin = mask.origin
 
     grid_scaled_1d = aa.util.geometry.grid_scaled_2d_slim_from(
         grid_pixels_2d_slim=grid_pixels_2d,
         shape_native=shape_native,
-        pixel_scales=(
-            pixel_scales[0] / sub_size,
-            pixel_scales[1] / sub_size,
-        ),
+        pixel_scales=pixel_scales,
         origin=origin,
     )
 
-    grid_scaled_1d[:, 0] -= pixel_scales[0] / (2.0 * sub_size)
-    grid_scaled_1d[:, 1] += pixel_scales[1] / (2.0 * sub_size)
+    grid_scaled_1d[:, 0] -= pixel_scales[0] / 2.0
+    grid_scaled_1d[:, 1] += pixel_scales[1] / 2.0
 
     return aa.Grid2DIrregular(values=grid_scaled_1d)
 
 
 def precompute_jacobian(func):
     @wraps(func)
     def wrapper(lensing_obj, grid, jacobian=None):
@@ -92,28 +87,28 @@
 
     return wrapper
 
 
 class OperateDeflections:
     """
     Packages methods which manipulate the 2D deflection angle map returned from the `deflections_yx_2d_from` function
-    of a mass object (e.g. a `MassProfile`, `Galaxy`, `Plane`).
+    of a mass object (e.g. a `MassProfile`, `Galaxy`).
 
     The majority of methods are those which from the 2D deflection angle map compute lensing quantities like a 2D
     shear field, magnification map or the Einstein Radius.
 
     The methods in `CalcLens` are passed to the mass object to provide a concise API.
 
     Parameters
     ----------
     deflections_yx_2d_from
         The function which returns the mass object's 2D deflection angles.
     """
 
-    def deflections_yx_2d_from(self, grid: aa.type.Grid2DLike):
+    def deflections_yx_2d_from(self, grid: aa.type.Grid2DLike, **kwargs):
         raise NotImplementedError
 
     def __eq__(self, other):
         return self.__dict__ == other.__dict__ and self.__class__ is other.__class__
 
     @precompute_jacobian
     def tangential_eigen_value_from(self, grid, jacobian=None) -> aa.Array2D:
@@ -200,27 +195,27 @@
         buffer
             The spacing in the y and x directions around each grid coordinate where deflection angles are computed and
             used to estimate the derivative.
         """
         if deflections_func is None:
             deflections_func = self.deflections_yx_2d_from
 
-        grid_shift_y_up = np.zeros(grid.shape)
+        grid_shift_y_up = aa.Grid2DIrregular(values=np.zeros(grid.shape))
         grid_shift_y_up[:, 0] = grid[:, 0] + buffer
         grid_shift_y_up[:, 1] = grid[:, 1]
 
-        grid_shift_y_down = np.zeros(grid.shape)
+        grid_shift_y_down = aa.Grid2DIrregular(values=np.zeros(grid.shape))
         grid_shift_y_down[:, 0] = grid[:, 0] - buffer
         grid_shift_y_down[:, 1] = grid[:, 1]
 
-        grid_shift_x_left = np.zeros(grid.shape)
+        grid_shift_x_left = aa.Grid2DIrregular(values=np.zeros(grid.shape))
         grid_shift_x_left[:, 0] = grid[:, 0]
         grid_shift_x_left[:, 1] = grid[:, 1] - buffer
 
-        grid_shift_x_right = np.zeros(grid.shape)
+        grid_shift_x_right = aa.Grid2DIrregular(values=np.zeros(grid.shape))
         grid_shift_x_right[:, 0] = grid[:, 0]
         grid_shift_x_right[:, 1] = grid[:, 1] + buffer
 
         deflections_up = deflections_func(grid=grid_shift_y_up)
         deflections_down = deflections_func(grid=grid_shift_y_down)
         deflections_left = deflections_func(grid=grid_shift_x_left)
         deflections_right = deflections_func(grid=grid_shift_x_right)
@@ -255,15 +250,15 @@
             The spacing in the y and x directions around each grid coordinate where deflection angles are computed and
             used to estimate the derivative.
         """
         hessian_yy, hessian_xy, hessian_yx, hessian_xx = self.hessian_from(
             grid=grid, buffer=buffer
         )
 
-        return grid.values_from(array_slim=0.5 * (hessian_yy + hessian_xx))
+        return aa.ArrayIrregular(values=0.5 * (hessian_yy + hessian_xx))
 
     def shear_yx_2d_via_hessian_from(
         self, grid, buffer: float = 0.01
     ) -> ShearYX2DIrregular:
         """
         Returns the 2D (y,x) shear vectors of the lensing object, which are computed from the 2D deflection angle map
         via the Hessian using the expressions (see equation 57 https://inspirehep.net/literature/419263):
@@ -281,29 +276,29 @@
         entries for [:,0] are the gamma_2 values and entries for [:,1] are the gamma_1 values.
 
         Note therefore that this convention means the FIRST entries in the array are the gamma_2 values and the SECOND
         entries are the gamma_1 values.
 
         Parameters
         ----------
-        grid
+        grids
             The 2D grid of (y,x) arc-second coordinates the deflection angles and Hessian are computed on.
         buffer
             The spacing in the y and x directions around each grid coordinate where deflection angles are computed and
             used to estimate the derivative.
         """
 
         hessian_yy, hessian_xy, hessian_yx, hessian_xx = self.hessian_from(
             grid=grid, buffer=buffer
         )
 
         gamma_1 = 0.5 * (hessian_xx - hessian_yy)
         gamma_2 = hessian_xy
 
-        shear_yx_2d = np.zeros(shape=(grid.sub_shape_slim, 2))
+        shear_yx_2d = np.zeros(shape=(grid.shape_slim, 2))
 
         shear_yx_2d[:, 0] = gamma_2
         shear_yx_2d[:, 1] = gamma_1
 
         return ShearYX2DIrregular(values=shear_yx_2d, grid=grid)
 
     def magnification_2d_via_hessian_from(
@@ -330,15 +325,25 @@
         """
         hessian_yy, hessian_xy, hessian_yx, hessian_xx = self.hessian_from(
             grid=grid, buffer=buffer, deflections_func=deflections_func
         )
 
         det_A = (1 - hessian_xx) * (1 - hessian_yy) - hessian_xy * hessian_yx
 
-        return grid.values_from(array_slim=1.0 / det_A)
+        return aa.ArrayIrregular(values=1.0 / det_A)
+
+    def contour_list_from(self, grid, contour_array):
+        grid_contour = aa.Grid2DContour(
+            grid=grid,
+            pixel_scales=grid.pixel_scales,
+            shape_native=grid.shape_native,
+            contour_array=contour_array.native,
+        )
+
+        return grid_contour.contour_list
 
     @evaluation_grid
     def tangential_critical_curve_list_from(
         self, grid, pixel_scale: Union[Tuple[float, float], float] = 0.05
     ) -> List[aa.Grid2DIrregular]:
         """
         Returns all tangential critical curves of the lensing system, which are computed as follows:
@@ -356,33 +361,15 @@
             on.
         pixel_scale
             If input, the `evaluation_grid` decorator creates the 2D grid at this resolution, therefore enabling the
             critical curve to be computed more accurately using a higher resolution grid.
         """
         tangential_eigen_values = self.tangential_eigen_value_from(grid=grid)
 
-        tangential_critical_curve_indices_list = measure.find_contours(
-            tangential_eigen_values.native, 0
-        )
-
-        if len(tangential_critical_curve_indices_list) == 0:
-            return []
-
-        tangential_critical_curve_list = []
-
-        for tangential_critical_curve_indices in tangential_critical_curve_indices_list:
-            curve = grid_scaled_2d_for_marching_squares_from(
-                grid_pixels_2d=tangential_critical_curve_indices,
-                shape_native=tangential_eigen_values.sub_shape_native,
-                mask=grid.mask,
-            )
-
-            tangential_critical_curve_list.append(curve)
-
-        return tangential_critical_curve_list
+        return self.contour_list_from(grid=grid, contour_array=tangential_eigen_values)
 
     @evaluation_grid
     def radial_critical_curve_list_from(
         self, grid, pixel_scale: Union[Tuple[float, float], float] = 0.05
     ) -> List[aa.Grid2DIrregular]:
         """
         Returns all radial critical curves of the lensing system, which are computed as follows:
@@ -400,33 +387,15 @@
             on.
         pixel_scale
             If input, the `evaluation_grid` decorator creates the 2D grid at this resolution, therefore enabling the
             critical curve to be computed more accurately using a higher resolution grid.
         """
         radial_eigen_values = self.radial_eigen_value_from(grid=grid)
 
-        radial_critical_curve_indices_list = measure.find_contours(
-            radial_eigen_values.native, 0
-        )
-
-        if len(radial_critical_curve_indices_list) == 0:
-            return []
-
-        radial_critical_curve_list = []
-
-        for radial_critical_curve_indices in radial_critical_curve_indices_list:
-            curve = grid_scaled_2d_for_marching_squares_from(
-                grid_pixels_2d=radial_critical_curve_indices,
-                shape_native=radial_eigen_values.sub_shape_native,
-                mask=grid.mask,
-            )
-
-            radial_critical_curve_list.append(curve)
-
-        return radial_critical_curve_list
+        return self.contour_list_from(grid=grid, contour_array=radial_eigen_values)
 
     @evaluation_grid
     def tangential_caustic_list_from(
         self, grid, pixel_scale: Union[Tuple[float, float], float] = 0.05
     ) -> List[aa.Grid2DIrregular]:
         """
         Returns all tangential caustics of the lensing system, which are computed as follows:
@@ -755,14 +724,15 @@
         The Jacobian is returned as a list of lists, which reflect its structure as a 2x2 matrix.
 
         Parameters
         ----------
         grid
             The 2D grid of (y,x) arc-second coordinates the deflection angles and Jacobian are computed on.
         """
+
         deflections = self.deflections_yx_2d_from(grid=grid)
 
         # TODO : Can probably make this work on irregular grid? Is there any point?
 
         a11 = aa.Array2D(
             values=1.0
             - np.gradient(deflections.native[:, :, 1], grid.native[0, :, 1], axis=1),
@@ -833,14 +803,14 @@
         ----------
         grid
             The 2D grid of (y,x) arc-second coordinates the deflection angles and Jacobian are computed on.
         jacobian
             A precomputed lensing jacobian, which is passed throughout the `CalcLens` functions for efficiency.
         """
 
-        shear_yx_2d = np.zeros(shape=(grid.sub_shape_slim, 2))
+        shear_yx_2d = np.zeros(shape=(grid.shape_slim, 2))
         shear_yx_2d[:, 0] = -0.5 * (jacobian[0][1] + jacobian[1][0])
         shear_yx_2d[:, 1] = 0.5 * (jacobian[1][1] - jacobian[0][0])
 
         if isinstance(grid, aa.Grid2DIrregular):
             return ShearYX2DIrregular(values=shear_yx_2d, grid=grid)
         return ShearYX2D(values=shear_yx_2d, grid=grid, mask=grid.mask)
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/operate/image.py` & `autogalaxy-2024.5.16.0/autogalaxy/operate/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from autogalaxy import exc
 
 
 class OperateImage:
     """
     Packages methods which operate on the 2D image returned from the `image_2d_from` function of a light object
-    (e.g. a `LightProfile`, `Galaxy`, `Plane`).
+    (e.g. a `LightProfile`, `Galaxy`).
 
     The majority of methods apply data operators to the 2D image which perform tasks such as a 2D convolution or
     Fourier transform.
 
     The methods in `OperateImage` are inherited by light objects to provide a concise API.
     """
 
@@ -35,15 +35,15 @@
         image_2d: aa.Array2D,
         blurring_image_2d: aa.Array2D,
         psf: Optional[aa.Kernel2D],
         convolver: aa.Convolver,
     ) -> aa.Array2D:
         if psf is not None:
             return psf.convolved_array_with_mask_from(
-                array=image_2d.binned.native + blurring_image_2d.binned.native,
+                array=image_2d.native + blurring_image_2d.native,
                 mask=image_2d.mask,
             )
 
         elif convolver is not None:
             return convolver.convolve_image(
                 image=image_2d, blurring_image=blurring_image_2d
             )
@@ -85,23 +85,23 @@
 
         image_2d_not_operated = self.image_2d_from(grid=grid, operated_only=False)
         blurring_image_2d_not_operated = self.image_2d_from(
             grid=blurring_grid, operated_only=False
         )
 
         blurred_image_2d = self._blurred_image_2d_from(
-            image_2d=image_2d_not_operated.binned,
-            blurring_image_2d=blurring_image_2d_not_operated.binned,
+            image_2d=image_2d_not_operated,
+            blurring_image_2d=blurring_image_2d_not_operated,
             psf=psf,
             convolver=convolver,
         )
 
         if self.has(cls=LightProfileOperated):
             image_2d_operated = self.image_2d_from(grid=grid, operated_only=True)
-            return blurred_image_2d + image_2d_operated.binned
+            return blurred_image_2d + image_2d_operated
 
         return blurred_image_2d
 
     def padded_image_2d_from(self, grid, psf_shape_2d):
         """
         Evaluate the light object's 2D image from a input 2D grid of padded coordinates, where this padding is
         sufficient to encapsulate all surrounding pixels that will blur light into the original image given the
@@ -163,15 +163,15 @@
             grid=padded_grid, operated_only=True
         )
 
         padded_image_2d_operated = padded_grid.mask.trimmed_array_from(
             padded_array=padded_image_2d_operated, image_shape=grid.mask.shape
         )
 
-        return padded_image_2d + padded_image_2d_operated.binned
+        return padded_image_2d + padded_image_2d_operated
 
     @aa.profile_func
     def visibilities_from(
         self, grid: aa.Grid2D, transformer: aa.type.Transformer
     ) -> aa.Visibilities:
         """
         Evaluate the light object's 2D image from a input 2D grid of coordinates and transform this to an array of
@@ -199,21 +199,21 @@
         image_2d = self.image_2d_from(grid=grid)
 
         if not np.any(image_2d):
             return aa.Visibilities.zeros(
                 shape_slim=(transformer.uv_wavelengths.shape[0],)
             )
 
-        return transformer.visibilities_from(image=image_2d.binned)
+        return transformer.visibilities_from(image=image_2d)
 
 
 class OperateImageList(OperateImage):
     """
     Packages methods which operate on the list of 2D images returned from the `image_2d_list_from` function of a light
-    object which contains multiple light profiles (e.g. a `Galaxy`, `Plane`).
+    object which contains multiple light profiles (e.g. a `Galaxy`).
 
     The majority of methods apply data operators to the list of 2D images which perform tasks such as a 2D convolution
     of Fourier transform.
 
     The methods in `OperateImageList` are inherited by light objects to provide a concise API.
     """
 
@@ -266,15 +266,15 @@
             blurred_image_2d = self._blurred_image_2d_from(
                 image_2d=image_2d_not_operated,
                 blurring_image_2d=blurring_image_2d_not_operated,
                 psf=psf,
                 convolver=convolver,
             )
 
-            image_2d_operated = image_2d_operated_list[i].binned
+            image_2d_operated = image_2d_operated_list[i]
 
             blurred_image_2d_list.append(image_2d_operated + blurred_image_2d)
 
         return blurred_image_2d_list
 
     def unmasked_blurred_image_2d_list_from(
         self, grid: aa.Grid2D, psf: aa.Kernel2D
@@ -347,25 +347,25 @@
 
         for image_2d in image_2d_list:
             if not np.any(image_2d):
                 visibilities = aa.Visibilities.zeros(
                     shape_slim=(transformer.uv_wavelengths.shape[0],)
                 )
             else:
-                visibilities = transformer.visibilities_from(image=image_2d.binned)
+                visibilities = transformer.visibilities_from(image=image_2d)
 
             visibilities_list.append(visibilities)
 
         return visibilities_list
 
 
 class OperateImageGalaxies(OperateImageList):
     """
     Packages methods which using a list of galaxies returns a dictionary of their 2D images using the function
-    `galaxy_image_2d_dict_from` (e.g. a `Plane`, a `Tracer` in the library **PyAutoLens**).
+    `galaxy_image_2d_dict_from` (e.g. galaxies, a `Tracer` in the library **PyAutoLens**).
 
     The majority of methods apply data operators to the dictionary of 2D images which perform tasks such as a 2D
     convolution of Fourier transform. This retains the keys of the dictionary to maintain information on the galaxies.
 
     The methods in `OperateImageGalaxies` are inherited by light objects to provide a concise API.
     """
 
@@ -415,19 +415,19 @@
         for galaxy_key in galaxy_image_2d_not_operated_dict.keys():
             image_2d_not_operated = galaxy_image_2d_not_operated_dict[galaxy_key]
             blurring_image_2d_not_operated = galaxy_blurring_image_2d_not_operated_dict[
                 galaxy_key
             ]
 
             blurred_image_2d = convolver.convolve_image(
-                image=image_2d_not_operated.binned,
-                blurring_image=blurring_image_2d_not_operated.binned,
+                image=image_2d_not_operated,
+                blurring_image=blurring_image_2d_not_operated,
             )
 
-            image_2d_operated = galaxy_image_2d_operated_dict[galaxy_key].binned
+            image_2d_operated = galaxy_image_2d_operated_dict[galaxy_key]
 
             galaxy_blurred_image_2d_dict[galaxy_key] = (
                 image_2d_operated + blurred_image_2d
             )
 
         return galaxy_blurred_image_2d_dict
 
@@ -467,12 +467,12 @@
 
             if not np.any(image_2d):
                 visibilities = aa.Visibilities.zeros(
                     shape_slim=(transformer.uv_wavelengths.shape[0],)
                 )
 
             else:
-                visibilities = transformer.visibilities_from(image=image_2d.binned)
+                visibilities = transformer.visibilities_from(image=image_2d)
 
             galaxy_visibilities_dict[galaxy_key] = visibilities
 
         return galaxy_visibilities_dict
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/plane/plane.py` & `autogalaxy-2024.5.16.0/autogalaxy/galaxy/galaxies.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,283 +1,311 @@
-import json
 import numpy as np
-from pathlib import Path
 from typing import Dict, List, Optional, Tuple, Type, Union
 
+from autoconf import conf
 import autoarray as aa
 
 from autogalaxy.galaxy.galaxy import Galaxy
 from autogalaxy.profiles.light.basis import Basis
-from autogalaxy.profiles.light.abstract import LightProfile
 from autogalaxy.profiles.light.linear import LightProfileLinear
-from autogalaxy.profiles.light.snr import LightProfileSNR
 from autogalaxy.operate.image import OperateImageGalaxies
 from autogalaxy.operate.deflections import OperateDeflections
 
-from autogalaxy import exc
-from autogalaxy.plane import plane_util
 
-
-class Plane(OperateImageGalaxies, OperateDeflections):
+class Galaxies(List, OperateImageGalaxies, OperateDeflections):
     def __init__(
         self,
-        galaxies,
-        redshift: Optional[float] = None,
+        galaxies: List[Galaxy],
         run_time_dict: Optional[Dict] = None,
     ):
         """
-        A plane of galaxies where all galaxies are at the same redshift.
+        A collection of galaxies, used to perform operations on the galaxies as a group.
 
-        Parameters
-        ----------
-        redshift or None
-            The redshift of the plane.
-        galaxies : [Galaxy]
-            The list of galaxies in this plane.
-        """
-
-        if redshift is None:
-            if not galaxies:
-                raise exc.PlaneException(
-                    "No redshift and no galaxies were input to a Plane. A redshift for the Plane therefore cannot be"
-                    "determined"
-                )
-            elif not all(
-                [galaxies[0].redshift == galaxy.redshift for galaxy in galaxies]
-            ):
-                redshift = np.mean([galaxy.redshift for galaxy in galaxies])
-            else:
-                redshift = galaxies[0].redshift
+        It is common for a user to have multiple galaxies in a list, for which they may perform operations like
+        creating the image of the light profiles or all galaxies or the potential of the mass profiles of all galaxies.
 
-        self.redshift = redshift
-        self.galaxies = galaxies
+        Many of these calculations are straight forward, for example for the image of all galaxies we simply sum the
+        images of each galaxy.
 
-        self.run_time_dict = run_time_dict
-        self.run_time_dict = run_time_dict
+        However, there are more complex operations that can be performed on the galaxies as a group, for example
+        computing the blured image of a group of galaxies where some galaxies have operated light profiles (meaning
+        that PSF blurring is already applied to them and thus should be skipped) and another subset of galaxies have
+        normal light profiles (meaning that PSF blurring should be applied to them).
 
-    @property
-    def galaxy_redshifts(self) -> List[float]:
-        return [galaxy.redshift for galaxy in self.galaxies]
+        This calculation requires a careful set of operations to ensure that the PSF blurring is only applied to the
+        subset of galaxies that do not have operated light profiles. This is an example of a calculation that is
+        performed by the `Galaxies` class, simplifing the code required to perform this operation.
 
-    def has(self, cls: Union[Type, Tuple[Type]]) -> bool:
-        if self.galaxies is not None:
-            return any(list(map(lambda galaxy: galaxy.has(cls=cls), self.galaxies)))
-        return False
+        Users may find that they often omit the `Galaxies` class and instead perform these operations in a more manual
+        way. This is fine, but care must be taken to ensure that the operations are performed correctly.
 
-    def cls_list_from(self, cls: Type) -> List:
+        Parameters
+        ----------
+        galaxies
+            The list of galaxies whose calculations are performed by this class.
+        run_time_dict
+            A dictionary of information on the run-times of function calls, including the total time and time spent on
+            different calculations.
         """
-        Returns a list of objects in the plane which are an instance of the input `cls`.
 
-        For example:
+        super().__init__(galaxies)
+        self.run_time_dict = run_time_dict
 
-        - If the input is `cls=ag.LightProfile`, a list containing all light profiles in the plane is returned.
+    @property
+    def redshift(self):
+        return self[0].redshift
 
-        Returns
-        -------
-            The list of objects in the plane that inherit from input `cls`.
+    def image_2d_list_from(
+        self, grid: aa.type.Grid2DLike, operated_only: Optional[bool] = None
+    ) -> List[aa.Array2D]:
         """
-        cls_list = []
+        Returns a list of the 2D images for each galaxy from a 2D grid of Cartesian (y,x) coordinates.
 
-        for galaxy in self.galaxies:
-            if galaxy.has(cls=cls):
-                for cls_galaxy in galaxy.cls_list_from(cls=cls):
-                    cls_list.append(cls_galaxy)
+        The image of each galaxy is computed by summing the images of all light profiles in that galaxy. If a galaxy
+        has no light profiles, a numpy array of zeros is returned.
 
-        return cls_list
+        For example, if there are 3 galaxies and only the first two have light profiles, the returned list of images
+        will be the image of the first two galaxies. The image of the third galaxies will be a numpy array of zeros.
 
-    def galaxies_with_cls_list_from(self, cls: Type) -> List[Galaxy]:
-        return list(filter(lambda galaxy: galaxy.has(cls=cls), self.galaxies))
+        The images output by this function do not include instrument operations, such as PSF convolution (for imaging
+        data) or a Fourier transform (for interferometer data).
 
-    @aa.grid_dec.grid_2d_to_structure
-    def image_2d_from(
-        self, grid: aa.type.Grid2DLike, operated_only: Optional[bool] = None
-    ) -> aa.Array2D:
-        """
-        Returns the profile-image plane image of the list of galaxies of the plane's sub-grid, by summing the
-        individual images of each galaxy's light profile.
+        Inherited methods in the `autogalaxy.operate.image` package can apply these operations to the images.
+        These functions may have the `operated_only` input passed to them, which is why this function includes
+        the `operated_only` input.
 
         If the `operated_only` input is included, the function omits light profiles which are parents of
         the `LightProfileOperated` object, which signifies that the light profile represents emission that has
-        already had the instrument operations (e.g. PSF convolution, a Fourier transform) applied to it.
+        already had the instrument operations (e.g. PSF convolution, a Fourier transform) applied to it and therefore
+        that operation is not performed again.
 
-        If the plane has no galaxies (or no galaxies have mass profiles) an arrays of all zeros the shape of the plane's
-        sub-grid is returned.
+        See the `autogalaxy.profiles.light` package for details of how images are computed from a light
+        profile.
 
         Parameters
         ----------
         grid
             The 2D (y, x) coordinates where values of the image are evaluated.
         operated_only
-            By default, the image is the sum of light profile images (irrespective of whether they have been operatd on
-            or not). If this input is included as a bool, only images which are or are not already operated are summed
-            and returned.
+            The returned list from this function contains all light profile images, and they are never operated on
+            (e.g. via the imaging PSF). However, inherited methods in the `autogalaxy.operate.image` package can
+            apply these operations to the images, which may have the `operated_only` input passed to them. This input
+            therefore is used to pass the `operated_only` input to these methods.
         """
-        if self.galaxies:
-            return sum(self.image_2d_list_from(grid=grid, operated_only=operated_only))
-        return np.zeros((grid.shape[0],))
-
-    def image_2d_list_from(
-        self, grid: aa.type.Grid2DLike, operated_only: Optional[bool] = None
-    ) -> List[aa.Array2D]:
         return [
             galaxy.image_2d_from(grid=grid, operated_only=operated_only)
-            for galaxy in self.galaxies
+            for galaxy in self
         ]
 
+    @aa.grid_dec.to_array
+    def image_2d_from(
+        self, grid: aa.type.Grid2DLike, operated_only: Optional[bool] = None
+    ) -> aa.Array2D:
+        """
+        Returns the 2D image of all galaxies summed from a 2D grid of Cartesian (y,x) coordinates.
+
+        This function first computes the image of each galaxy, via the function `image_2d_list_from`. The
+        images are then summed to give the overall image of the galaxies.
+
+        Refer to the function `image_2d_list_from` for a full description of the calculation and how the `operated_only`
+        input is used.
+
+        Parameters
+        ----------
+        grid
+            The 2D (y, x) coordinates where values of the image are evaluated.
+        operated_only
+            The returned list from this function contains all light profile images, and they are never operated on
+            (e.g. via the imaging PSF). However, inherited methods in the `autogalaxy.operate.image` package can
+            apply these operations to the images, which may have the `operated_only` input passed to them. This input
+            therefore is used to pass the `operated_only` input to these methods.
+        """
+        return sum(self.image_2d_list_from(grid=grid, operated_only=operated_only))
+
     def galaxy_image_2d_dict_from(
         self, grid: aa.type.Grid2DLike, operated_only: Optional[bool] = None
     ) -> {Galaxy: np.ndarray}:
         """
-        Returns a dictionary associating every `Galaxy` object in the `Plane` with its corresponding 2D image, using
-        the instance of each galaxy as the dictionary keys.
+        Returns a dictionary associating every `Galaxy` object with its corresponding 2D image, using the instance
+        of each galaxy as the dictionary keys.
 
-        This object is used for adapt features, which use the image of each galaxy in a model-fit in order to
+        This object is used for adaptive-features, which use the image of each galaxy in a model-fit in order to
         adapt quantities like a pixelization or regularization scheme to the surface brightness of the galaxies being
         fitted.
 
         By inheriting from `OperateImageGalaxies` functions which apply operations of this dictionary are accessible,
         for example convolving every image with a PSF or applying a Fourier transform to create a galaxy-visibilities
         dictionary.
 
         Parameters
         ----------
         grid
             The 2D (y,x) coordinates of the (masked) grid, in its original geometric reference frame.
 
         Returns
         -------
-        A dictionary associated every galaxy in the plane with its corresponding 2D image.
+        A dictionary associated every galaxy with its corresponding 2D image.
         """
 
         galaxy_image_2d_dict = dict()
 
         image_2d_list = self.image_2d_list_from(grid=grid, operated_only=operated_only)
 
-        for galaxy_index, galaxy in enumerate(self.galaxies):
+        for galaxy_index, galaxy in enumerate(self):
             galaxy_image_2d_dict[galaxy] = image_2d_list[galaxy_index]
 
         return galaxy_image_2d_dict
 
-    def plane_image_2d_from(
-        self, grid: aa.type.Grid2DLike, zoom_to_brightest: bool = True
-    ) -> aa.Array2D:
-        return plane_util.plane_image_from(
-            galaxies=self.galaxies,
-            grid=grid.mask.derive_grid.all_false_sub_1,
-            zoom_to_brightest=zoom_to_brightest,
-        )
+    @aa.grid_dec.to_vector_yx
+    def deflections_yx_2d_from(self, grid: aa.type.Grid2DLike, **kwargs) -> np.ndarray:
+        """
+        Returns the summed 2D deflections angles of all galaxies from a 2D grid of Cartesian (y,x) coordinates.
 
-    @aa.grid_dec.grid_2d_to_vector_yx
-    @aa.grid_dec.grid_2d_to_structure
-    def deflections_yx_2d_from(self, grid: aa.type.Grid2DLike) -> np.ndarray:
-        if self.galaxies:
-            return sum(
-                map(lambda g: g.deflections_yx_2d_from(grid=grid), self.galaxies)
-            )
+        The deflections of each galaxy is computed by summing the deflections of all mass profiles in that galaxy. If a
+        galaxy has no mass profiles, a numpy array of zeros is returned.
+
+        This calculation does not account for multi-plane ray-tracing effects, it is simply the sum of the deflections
+        of all galaxies. The `Tracer` class in PyAutoLens is required for this.
+
+        For example, if there are 3 galaxies and only the first two have mass profiles, the returned list of deflections
+        will be the deflections of the first two galaxies. The deflections of the third galaxies will be a numpy
+        array of zeros.
+
+        See the `autogalaxy.profiles.mass` package for details of how deflections are computed from a mass profile.
+
+        Parameters
+        ----------
+        grid
+            The 2D (y, x) coordinates where values of the deflections are evaluated.
+        """
+        if self:
+            return sum(map(lambda g: g.deflections_yx_2d_from(grid=grid), self))
         return np.zeros(shape=(grid.shape[0], 2))
 
-    @aa.grid_dec.grid_2d_to_structure
-    def convergence_2d_from(self, grid: aa.type.Grid2DLike) -> np.ndarray:
+    @aa.grid_dec.to_grid
+    def traced_grid_2d_from(self, grid: aa.type.Grid2DLike) -> aa.type.Grid2DLike:
+        """
+        Trace this plane's grid_stacks to the next plane, using its deflection angles.
         """
-        Returns the convergence of the list of galaxies of the plane's sub-grid, by summing the individual convergences \
-        of each galaxy's mass profile.
+        return grid - self.deflections_yx_2d_from(grid=grid)
 
-        The convergence is calculated on the sub-grid and binned-up to the original grid by taking the mean
-        value of every set of sub-pixels, provided the *returned_binned_sub_grid* bool is `True`.
+    @aa.grid_dec.to_array
+    def convergence_2d_from(self, grid: aa.type.Grid2DLike, **kwargs) -> np.ndarray:
+        """
+        Returns the summed 2D convergence of all galaxies from a 2D grid of Cartesian (y,x) coordinates.
 
-        If the plane has no galaxies (or no galaxies have mass profiles) an arrays of all zeros the shape of the plane's
-        sub-grid is returned.
+        The convergence of each galaxy is computed by summing the convergence of all mass profiles in that galaxy. If a
+        galaxy has no mass profiles, a numpy array of zeros is returned.
 
-        Internally data structures are treated as ndarrays, however the decorator `grid_2d_to_structure` converts
-        the output to an `Array2D` using the input `grid`'s attributes.
+        This calculation does not account for multi-plane ray-tracing effects, it is simply the sum of the convergence
+        of all galaxies. The `Tracer` class in PyAutoLens is required for this.
+
+        For example, if there are 3 galaxies and only the first two have mass profiles, the returned list of convergence
+        will be the convergence of the first two galaxies. The convergence of the third galaxies will be a numpy
+        array of zeros.
+
+        See the `autogalaxy.profiles.mass` package for details of how convergence are computed from a mass profile.
 
         Parameters
         ----------
-        grid : Grid2D
-            The grid (or sub) of (y,x) arc-second coordinates at the centre of every unmasked pixel which the \
-            potential is calculated on.
-        galaxies : [Galaxy]
-            The galaxies whose mass profiles are used to compute the surface densities.
+        grid
+            The 2D (y, x) coordinates where values of the convergence are evaluated.
         """
-        if self.galaxies:
-            return sum(map(lambda g: g.convergence_2d_from(grid=grid), self.galaxies))
+        if self:
+            return sum(map(lambda g: g.convergence_2d_from(grid=grid), self))
         return np.zeros((grid.shape[0],))
 
-    @aa.grid_dec.grid_2d_to_structure
-    def potential_2d_from(self, grid: aa.type.Grid2DLike) -> np.ndarray:
+    @aa.grid_dec.to_array
+    def potential_2d_from(self, grid: aa.type.Grid2DLike, **kwargs) -> np.ndarray:
         """
-        Returns the potential of the list of galaxies of the plane's sub-grid, by summing the individual potentials \
-        of each galaxy's mass profile.
+        Returns the summed 2D potential of all galaxies from a 2D grid of Cartesian (y,x) coordinates.
 
-        The potential is calculated on the sub-grid and binned-up to the original grid by taking the mean
-        value of every set of sub-pixels, provided the *returned_binned_sub_grid* bool is `True`.
+        The potential of each galaxy is computed by summing the potential of all mass profiles in that galaxy. If a
+        galaxy has no mass profiles, a numpy array of zeros is returned.
 
-        If the plane has no galaxies (or no galaxies have mass profiles) an arrays of all zeros the shape of the plane's
-        sub-grid is returned.
+        This calculation does not account for multi-plane ray-tracing effects, it is simply the sum of the potential
+        of all galaxies. The `Tracer` class in PyAutoLens is required for this.
 
-        Internally data structures are treated as ndarrays, however the decorator `grid_2d_to_structure` converts
-        the output to an `Array2D` using the input `grid`'s attributes.
+        For example, if there are 3 galaxies and only the first two have mass profiles, the returned list of potential
+        will be the potential of the first two galaxies. The potential of the third galaxies will be a numpy
+        array of zeros.
+
+        See the `autogalaxy.profiles.mass` package for details of how potential are computed from a mass profile.
 
         Parameters
         ----------
-        grid : Grid2D
-            The grid (or sub) of (y,x) arc-second coordinates at the centre of every unmasked pixel which the \
-            potential is calculated on.
-        galaxies : [Galaxy]
-            The galaxies whose mass profiles are used to compute the surface densities.
+        grid
+            The 2D (y, x) coordinates where values of the potential are evaluated.
         """
-        if self.galaxies:
-            return sum(map(lambda g: g.potential_2d_from(grid=grid), self.galaxies))
+        if self:
+            return sum(map(lambda g: g.potential_2d_from(grid=grid), self))
         return np.zeros((grid.shape[0],))
 
-    @aa.grid_dec.grid_2d_to_structure
-    def traced_grid_from(self, grid: aa.type.Grid2DLike) -> aa.type.Grid2DLike:
+    def has(self, cls: Union[Type, Tuple[Type]]) -> bool:
         """
-        Trace this plane's grid_stacks to the next plane, using its deflection angles.
+        Returns a bool specifying whether any of the galaxies has a certain class type.
+
+        For example, for the input `cls=ag.LightProfile`, this function returns True if any galaxy has a
+        light profile and false if no galaxy has a light profile.
+
+        This function is used to check for mass profiles and specific types of profiles, like the linear light profile.
+
+        Parameters
+        ----------
+        cls
+            The class type of the galaxy which is checked for in the tracer.
+
+        Returns
+        -------
+        True if any galaxy in the tracer has the input class type, else False.
         """
-        return grid - self.deflections_yx_2d_from(grid=grid)
+        return any(list(map(lambda galaxy: galaxy.has(cls=cls), self)))
 
-    @property
-    def perform_inversion(self) -> bool:
+    def cls_list_from(self, cls: Type) -> List:
         """
-        Returns a bool specifying whether this fit object performs an inversion.
+        Returns a list of objects in the galaxies which are an instance of the input `cls`.
+
+        For example:
 
-        This is based on whether any of the galaxies in the `model_obj` have a `Pixelization` or `LightProfileLinear`
-        object, in which case an inversion is performed.
+        - If the input is `cls=ag.LightProfile`, a list containing all light profiles of all galaxies is returned.
 
         Returns
         -------
-            A bool which is True if an inversion is performed.
+            The list of objects in the galaxies that inherit from input `cls`.
         """
-        if self.has(cls=(aa.Pixelization, LightProfileLinear)):
-            return True
-        elif self.has(cls=Basis):
-            basis_list = self.cls_list_from(cls=Basis)
-            for basis in basis_list:
-                for light_profile in basis.light_profile_list:
-                    if isinstance(light_profile, LightProfileLinear):
-                        return True
+        cls_list = []
 
-        return False
+        for galaxy in self:
+            if galaxy.has(cls=cls):
+                for cls_galaxy in galaxy.cls_list_from(cls=cls):
+                    cls_list.append(cls_galaxy)
+
+        return cls_list
+
+    def galaxies_with_cls_list_from(self, cls: Type) -> List[Galaxy]:
+        return list(filter(lambda galaxy: galaxy.has(cls=cls), self))
+
+    def galaxy_has_cls(self, cls: Type) -> bool:
+        return any([galaxy.has(cls=cls) for galaxy in self])
 
     def extract_attribute(self, cls, attr_name):
         """
-        Returns an attribute of a class in `Plane` as a `ValueIrregular` or `Grid2DIrregular` object.
+        Returns an attribute of a class in all galaxies as a `ValueIrregular` or `Grid2DIrregular` object.
 
-        For example, if a plane has a galaxy which two light profiles and we want its axis-ratios, the following:
+        For example, if there is one galaxy with two light profiles and we want its axis-ratios, the following:
 
-        `plane.extract_attribute(cls=LightProfile, name="axis_ratio")`
+        `galaxies.extract_attribute(cls=LightProfile, name="axis_ratio")`
 
         would return:
 
         ArrayIrregular(values=[axis_ratio_0, axis_ratio_1])
 
         If a galaxy has three mass profiles and we want their centres, the following:
 
-        `plane.extract_attribute(cls=MassProfile, name="centres")`
+        `galaxies.extract_attribute(cls=MassProfile, name="centres")`
 
         would return:
 
         GridIrregular2D(grid=[(centre_y_0, centre_x_0), (centre_y_1, centre_x_1), (centre_y_2, centre_x_2)])
 
         This is used for visualization, for example plotting the centres of all mass profiles colored by their profile.
         """
@@ -286,98 +314,143 @@
             try:
                 return getattr(value, name)
             except (AttributeError, IndexError):
                 return None
 
         attributes = [
             extract(value, attr_name)
-            for galaxy in self.galaxies
+            for galaxy in self
             for value in galaxy.__dict__.values()
             if isinstance(value, cls)
         ]
 
         if attributes == []:
             return None
         elif isinstance(attributes[0], float):
             return aa.ArrayIrregular(values=attributes)
         elif isinstance(attributes[0], tuple):
             return aa.Grid2DIrregular(values=attributes)
 
-    def extract_attributes_of_galaxies(self, cls, attr_name, filter_nones=False):
+    @property
+    def perform_inversion(self) -> bool:
         """
-        Returns an attribute of a class in the plane as a list of `ValueIrregular` or `Grid2DIrregular` objects,
-        where the list indexes correspond to each galaxy in the plane..
+        Returns a bool specifying whether this fit object performs an inversion.
 
-        For example, if a plane has two galaxies which each have a light profile the following:
+        This is based on whether any of the galaxies have a `Pixelization` or `LightProfileLinear` object, in which
+        case an inversion is performed.
 
-        `plane.extract_attributes_of_galaxies(cls=LightProfile, name="axis_ratio")`
+        Returns
+        -------
+            A bool which is True if an inversion is performed.
+        """
+        if self.has(cls=(aa.Pixelization, LightProfileLinear)):
+            return True
+        elif self.has(cls=Basis):
+            basis_list = self.cls_list_from(cls=Basis)
+            for basis in basis_list:
+                for light_profile in basis.light_profile_list:
+                    if isinstance(light_profile, LightProfileLinear):
+                        return True
 
-        would return:
+        return False
 
-        [ArrayIrregular(values=[axis_ratio_0]), ArrayIrregular(values=[axis_ratio_1])]
+    def plane_image_2d_from(
+        self, grid: aa.type.Grid2DLike, zoom_to_brightest: bool = True
+    ) -> aa.Array2D:
+        return plane_image_from(
+            galaxies=self,
+            grid=grid.mask.derive_grid.all_false,
+            zoom_to_brightest=zoom_to_brightest,
+        )
 
-        If a plane has two galaxies, the first with a mass profile and the second with two mass profiles ,the following:
 
-        `plane.extract_attributes_of_galaxies(cls=MassProfile, name="centres")`
+def plane_image_from(
+    galaxies: List[Galaxy],
+    grid: aa.Grid2D,
+    buffer: float = 1.0e-2,
+    zoom_to_brightest: bool = True,
+) -> aa.Array2D:
+    """
+    Returns the plane image of a list of galaxies, by summing their individual images.
+
+    For lensing calculations performed by **PyAutoLens**, this function is used to return the unleensed image
+    source-plane galaxies.
+
+    By default, an adaptive grid is used to determine the grid that the images of the galaxies are computed on.
+    This grid adapts its dimensions to capture the brightest regions of the image, ensuring that visualization of
+    the plane-image is focused entirely on where the galaxies are brightest.
+
+    This adaptive grid is based on determining the size of the grid that contains all pixels with an
+    input % (typically 99%) of the total flux of the brightest pixel in the image.
+
+    The adaptive grid can be disabled such that the input grid is used to compute the image of the galaxies.
+
+    Parameters
+    ----------
+    galaxies
+        The list of galaxies whose images are summed to compute the plane image.
+    grid
+        The grid of (y,x) coordinates for which the image of the galaxies is computed on, or from which the adaptive
+        grid is derived.
+    buffer
+        The buffer around the adaptive grid that is used to ensure the image of the galaxies is not cut off.
+    zoom_to_brightest
+        If True, an adaptive grid is used to compute the image of the galaxies which zooms in on the brightest
+        regions of the image. If False, the input grid is used.
+
+    Returns
+    -------
+    The plane image of the galaxies, which is the sum of their individual images.
+    """
+
+    shape = grid.shape_native
+
+    if zoom_to_brightest:
+        try:
+            image = sum(map(lambda g: g.image_2d_from(grid=grid), galaxies))
+            image = image.native
 
-        would return:
-        [
-            Grid2DIrregular(values=[(centre_y_0, centre_x_0)]),
-            Grid2DIrregular(values=[(centre_y_0, centre_x_0), (centre_y_1, centre_x_1)])
-        ]
+            zoom_percent = conf.instance["visualize"]["general"]["zoom"][
+                "plane_percent"
+            ]
 
-        If a Profile does not have a certain entry, it is replaced with a None. Nones can be removed by
-        setting `filter_nones=True`.
+            fractional_value = np.max(image) * zoom_percent
 
-        This is used for visualization, for example plotting the centres of all mass profiles colored by their profile.
-        """
-        if filter_nones:
-            return [
-                galaxy.extract_attribute(cls=cls, attr_name=attr_name)
-                for galaxy in self.galaxies
-                if galaxy.extract_attribute(cls=cls, attr_name=attr_name) is not None
-            ]
+            fractional_bool = image > fractional_value
 
-        else:
-            return [
-                galaxy.extract_attribute(cls=cls, attr_name=attr_name)
-                for galaxy in self.galaxies
-            ]
+            true_indices = np.argwhere(fractional_bool)
 
-    def set_snr_of_snr_light_profiles(
-        self,
-        grid: aa.type.Grid2DLike,
-        exposure_time: float,
-        background_sky_level: float = 0.0,
-        psf: Optional[aa.Kernel2D] = None,
-    ):
-        """
-        Iterate over every `LightProfileSNR` in the plane and set their `intensity` values to values which give
-        their input `signal_to_noise_ratio` value, which is performed as follows:
+            y_max_pix = np.min(true_indices[:, 0])
+            y_min_pix = np.max(true_indices[:, 0])
+            x_min_pix = np.min(true_indices[:, 1])
+            x_max_pix = np.max(true_indices[:, 1])
 
-        - Evaluate the image of each light profile on the input grid.
-        - Blur this image with a PSF, if included.
-        - Take the value of the brightest pixel.
-        - Use an input `exposure_time` and `background_sky` (e.g. from the `SimulatorImaging` object) to determine
-          what value of `intensity` gives the desired signal to noise ratio for the image.
+            grid = grid.native
 
-        Parameters
-        ----------
-        grid
-            The (y, x) coordinates in the original reference frame of the grid.
-        exposure_time
-            The exposure time of the simulated imaging.
-        background_sky_level
-            The level of the background sky of the simulated imaging.
-        psf
-            The psf of the simulated imaging which can change the S/N of the light profile due to spreading out
-            the emission.
-        """
-        for galaxy in self.galaxies:
-            for light_profile in galaxy.cls_list_from(cls=LightProfile):
-                if isinstance(light_profile, LightProfileSNR):
-                    light_profile.set_intensity_from(
-                        grid=grid,
-                        exposure_time=exposure_time,
-                        background_sky_level=background_sky_level,
-                        psf=psf,
-                    )
+            extent = (
+                grid[0, x_min_pix][1] - buffer,
+                grid[0, x_max_pix][1] + buffer,
+                grid[y_min_pix, 0][0] - buffer,
+                grid[y_max_pix, 0][0] + buffer,
+            )
+
+            extent = aa.util.geometry.extent_symmetric_from(extent=extent)
+
+            pixel_scales = (
+                float((extent[3] - extent[2]) / shape[0]),
+                float((extent[1] - extent[0]) / shape[1]),
+            )
+            origin = ((extent[3] + extent[2]) / 2.0, (extent[1] + extent[0]) / 2.0)
+
+            grid = aa.Grid2D.uniform(
+                shape_native=grid.shape_native,
+                pixel_scales=pixel_scales,
+                origin=origin,
+            )
+        except ValueError:
+            pass
+
+    image = sum(map(lambda g: g.image_2d_from(grid=grid), galaxies))
+
+    return aa.Array2D.no_mask(
+        values=image.native, pixel_scales=grid.pixel_scales, origin=grid.origin
+    )
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/plane/plot/plane_plotters.py` & `autogalaxy-2024.5.16.0/autogalaxy/galaxy/plot/galaxies_plotters.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,190 +7,189 @@
 from autogalaxy.plot.mat_plot.one_d import MatPlot1D
 from autogalaxy.plot.mat_plot.two_d import MatPlot2D
 from autogalaxy.plot.visuals.one_d import Visuals1D
 from autogalaxy.plot.visuals.two_d import Visuals2D
 from autogalaxy.plot.include.one_d import Include1D
 from autogalaxy.plot.include.two_d import Include2D
 from autogalaxy.plot.mass_plotter import MassPlotter
+from autogalaxy.galaxy.galaxy import Galaxy
+from autogalaxy.galaxy.galaxies import Galaxies
 from autogalaxy.galaxy.plot.galaxy_plotters import GalaxyPlotter
 
 from autogalaxy import exc
-from autogalaxy.plane.plane import Plane
 
 
-class PlanePlotter(Plotter):
+class GalaxiesPlotter(Plotter):
     def __init__(
         self,
-        plane: Plane,
+        galaxies: List[Galaxy],
         grid: aa.type.Grid1D2DLike,
         mat_plot_1d: MatPlot1D = MatPlot1D(),
         visuals_1d: Visuals1D = Visuals1D(),
         include_1d: Include1D = Include1D(),
         mat_plot_2d: MatPlot2D = MatPlot2D(),
         visuals_2d: Visuals2D = Visuals2D(),
         include_2d: Include2D = Include2D(),
     ):
         """
-        Plots the attributes of `Plane` objects using the matplotlib methods `plot()` and `imshow()` and many
+        Plots the attributes of a list of galaxies using the matplotlib methods `plot()` and `imshow()` and many
         other matplotlib functions which customize the plot's appearance.
 
         The `mat_plot_1d` and `mat_plot_2d` attributes wrap matplotlib function calls to make the figure. By default,
         the settings passed to every matplotlib function called are those specified in
         the `config/visualize/mat_wrap/*.ini` files, but a user can manually input values into `MatPlot2D` to
         customize the figure's appearance.
 
         Overlaid on the figure are visuals, contained in the `Visuals1D` and `Visuals2D` objects. Attributes may be
         extracted from the `MassProfile` and plotted via the visuals object, if the corresponding entry is `True` in
         the `Include1D` or `Include2D` object or the `config/visualize/include.ini` file.
 
         Parameters
         ----------
-        plane
-            The plane the plotter plots.
+        galaxies
+            The galaxies the plotter plots.
         grid
-            The 2D (y,x) grid of coordinates used to evaluate the plane's light and mass quantities that are plotted.
+            The 2D (y,x) grid of coordinates used to evaluate the galaxies light and mass quantities that are plotted.
         mat_plot_1d
             Contains objects which wrap the matplotlib function calls that make 1D plots.
         visuals_1d
             Contains 1D visuals that can be overlaid on 1D plots.
         include_1d
             Specifies which attributes of the `MassProfile` are extracted and plotted as visuals for 1D plots.
         mat_plot_2d
             Contains objects which wrap the matplotlib function calls that make 2D plots.
         visuals_2d
             Contains 2D visuals that can be overlaid on 2D plots.
         include_2d
             Specifies which attributes of the `MassProfile` are extracted and plotted as visuals for 2D plots.
         """
 
+        self.galaxies = Galaxies(galaxies=galaxies)
+
         from autogalaxy.profiles.light.linear import (
             LightProfileLinear,
         )
 
-        if plane.has(cls=LightProfileLinear):
+        if self.galaxies.has(cls=LightProfileLinear):
             raise exc.raise_linear_light_profile_in_plot(
                 plotter_type=self.__class__.__name__,
             )
 
         super().__init__(
             mat_plot_2d=mat_plot_2d,
             include_2d=include_2d,
             visuals_2d=visuals_2d,
             mat_plot_1d=mat_plot_1d,
             include_1d=include_1d,
             visuals_1d=visuals_1d,
         )
 
-        self.plane = plane
         self.grid = grid
 
         self._mass_plotter = MassPlotter(
-            mass_obj=self.plane,
+            mass_obj=self.galaxies,
             grid=self.grid,
             get_visuals_2d=self.get_visuals_2d,
             mat_plot_2d=self.mat_plot_2d,
             include_2d=self.include_2d,
             visuals_2d=self.visuals_2d,
         )
 
     def get_visuals_2d(self) -> Visuals2D:
         return self.get_2d.via_light_mass_obj_from(
-            light_mass_obj=self.plane, grid=self.grid
+            light_mass_obj=self.galaxies, grid=self.grid
         )
 
     def get_visuals_2d_of_galaxy(self, galaxy_index: int) -> aplt.Visuals2D:
-        return self.get_2d.via_plane_from(
-            plane=self.plane, grid=self.grid, galaxy_index=galaxy_index
+        return self.get_2d.via_galaxies_from(
+            galaxies=self.galaxies, grid=self.grid, galaxy_index=galaxy_index
         )
 
     def galaxy_plotter_from(self, galaxy_index: int) -> GalaxyPlotter:
         """
         Returns an `GalaxyPlotter` corresponding to a `Galaxy` in the `Tracer`.
 
         Returns
         -------
         galaxy_index
             The index of the galaxy in the `Tracer` used to make the `GalaxyPlotter`.
         """
 
         return GalaxyPlotter(
-            galaxy=self.plane.galaxies[galaxy_index],
+            galaxy=self.galaxies[galaxy_index],
             grid=self.grid,
             mat_plot_2d=self.mat_plot_2d,
             visuals_2d=self.get_visuals_2d_of_galaxy(galaxy_index=galaxy_index),
             include_2d=self.include_2d,
         )
 
     def figures_2d(
         self,
         image: bool = False,
-        plane_image: bool = False,
-        plane_grid: bool = False,
         convergence: bool = False,
         potential: bool = False,
         deflections_y: bool = False,
         deflections_x: bool = False,
         magnification: bool = False,
+        plane_image: bool = False,
+        plane_grid: bool = False,
         zoom_to_brightest: bool = True,
         title_suffix: str = "",
         filename_suffix: str = "",
         source_plane_title: bool = False,
     ):
         """
-        Plots the individual attributes of the plotter's `Plane` object in 2D, which are computed via the plotter's 2D
+        Plots the individual attributes of the plotter's `Galaxies` object in 2D, which are computed via the plotter's 2D
         grid object.
 
-        The API is such that every plottable attribute of the `Plane` object is an input parameter of type bool of
+        The API is such that every plottable attribute of the `Galaxies` object is an input parameter of type bool of
         the function, which if switched to `True` means that it is plotted.
 
         Parameters
         ----------
         image
-            Whether to make a 2D plot (via `imshow`) of the image of plane in its image-plane (e.g. after
-            lensing).
-        plane_image
-            Whether to make a 2D plot (via `imshow`) of the image of the plane in the soure-plane (e.g. its
-            unlensed light).
+            Whether to make a 2D plot (via `imshow`) of the image of the galaxies.
         convergence
             Whether to make a 2D plot (via `imshow`) of the convergence.
         potential
             Whether to make a 2D plot (via `imshow`) of the potential.
         deflections_y
             Whether to make a 2D plot (via `imshow`) of the y component of the deflection angles.
         deflections_x
             Whether to make a 2D plot (via `imshow`) of the x component of the deflection angles.
         magnification
             Whether to make a 2D plot (via `imshow`) of the magnification.
+        plane_image
+            Whether to make a 2D plot (via `imshow`) of the image of the plane in the soure-plane (e.g. its
+            unlensed light).
         zoom_to_brightest
-            For images not in the image-plane (e.g. the `plane_image`), whether to automatically zoom the plot to
-            the brightest regions of the galaxies being plotted as opposed to the full extent of the grid.
+            Whether to automatically zoom the plot to the brightest regions of the galaxies being plotted as
+            opposed to the full extent of the grid.
         title_suffix
             Add a suffix to the end of the matplotlib title label.
         filename_suffix
             Add a suffix to the end of the filename the plot is saved to hard-disk using.
-        source_plane_title
-            If `True`, the title of the plot is overwritten to read "source-plane image".
         """
         if image:
             self.mat_plot_2d.plot_array(
-                array=self.plane.image_2d_from(grid=self.grid),
+                array=self.galaxies.image_2d_from(grid=self.grid),
                 visuals_2d=self.get_visuals_2d(),
                 auto_labels=aplt.AutoLabels(
                     title=f"Image{title_suffix}", filename=f"image_2d{filename_suffix}"
                 ),
             )
 
         if plane_image:
             if source_plane_title:
                 title = "Source Plane Image"
             else:
                 title = f"Plane Image{title_suffix}"
 
             self.mat_plot_2d.plot_array(
-                array=self.plane.plane_image_2d_from(
+                array=self.galaxies.plane_image_2d_from(
                     grid=self.grid, zoom_to_brightest=zoom_to_brightest
                 ),
                 visuals_2d=self.get_visuals_2d(),
                 auto_labels=aplt.AutoLabels(
                     title=title,
                     filename=f"plane_image{filename_suffix}",
                 ),
@@ -218,47 +217,47 @@
             deflections_x=deflections_x,
             magnification=magnification,
         )
 
     def galaxy_indexes_from(self, galaxy_index: Optional[int]) -> List[int]:
         """
         Returns a list of all indexes of the galaxys in the fit, which is iterated over in figures that plot
-        individual figures of each galaxy in a plane.
+        individual figures of each galaxy.
 
         Parameters
         ----------
         galaxy_index
             A specific galaxy index which when input means that only a single galaxy index is returned.
 
         Returns
         -------
         list
             A list of galaxy indexes corresponding to galaxys in the galaxy.
         """
         if galaxy_index is None:
-            return list(range(len(self.plane.galaxies)))
+            return list(range(len(self.galaxies)))
         return [galaxy_index]
 
     def figures_2d_of_galaxies(
         self, image: bool = False, galaxy_index: Optional[int] = None
     ):
         """
-        Plots galaxy images for each individual `Galaxy` in the plotter's `Plane` in 2D,  which are computed via the
+        Plots galaxy images for each individual `Galaxy` in the plotter's `Galaxies` in 2D,  which are computed via the
         plotter's 2D grid object.
 
         The API is such that every plottable attribute of the `galaxy` object is an input parameter of type bool of
         the function, which if switched to `True` means that it is plotted.
 
         Parameters
         ----------
         image
             Whether to make a 2D plot (via `imshow`) of the image of the galaxy in the soure-galaxy (e.g. its
             unlensed light).
         galaxy_index
-            If input, plots for only a single galaxy based on its index in the plane are created.
+            If input, plots for only a single galaxy based on its index are created.
         """
         galaxy_indexes = self.galaxy_indexes_from(galaxy_index=galaxy_index)
 
         for galaxy_index in galaxy_indexes:
             galaxy_plotter = self.galaxy_plotter_from(galaxy_index=galaxy_index)
 
             if image:
@@ -267,88 +266,80 @@
                     title_suffix=f" Of Galaxy {galaxy_index}",
                     filename_suffix=f"_of_galaxy_{galaxy_index}",
                 )
 
     def subplot(
         self,
         image: bool = False,
-        plane_image: bool = False,
-        plane_grid: bool = False,
         convergence: bool = False,
         potential: bool = False,
         deflections_y: bool = False,
         deflections_x: bool = False,
         magnification: bool = False,
-        auto_filename: str = "subplot_plane",
+        auto_filename: str = "subplot_galaxies",
     ):
         """
-        Plots the individual attributes of the plotter's `Plane` object in 2D on a subplot, which are computed via the
+        Plots the individual attributes of the plotter's `Galaxies` object in 2D on a subplot, which are computed via the
         plotter's 2D grid object.
 
-        The API is such that every plottable attribute of the `Plane` object is an input parameter of type bool of
+        The API is such that every plottable attribute of the `Galaxies` object is an input parameter of type bool of
         the function, which if switched to `True` means that it is included on the subplot.
 
         Parameters
         ----------
         image
-            Whether or not to  include a 2D plot (via `imshow`) of the image of plane in its image-plane (e.g. after
-            lensing).
-        plane_image
-            Whether or not to  include a 2D plot (via `imshow`) of the image of the plane in the soure-plane (e.g. its
-            unlensed light).
+            Whether or not to include a 2D plot (via `imshow`) of the image.
         convergence
-            Whether or not to  include a 2D plot (via `imshow`) of the convergence.
+            Whether or not to include a 2D plot (via `imshow`) of the convergence.
         potential
-            Whether or not to  include a 2D plot (via `imshow`) of the potential.
+            Whether or not to include a 2D plot (via `imshow`) of the potential.
         deflections_y
-            Whether or not to  include a 2D plot (via `imshow`) of the y component of the deflection angles.
+            Whether or not to include a 2D plot (via `imshow`) of the y component of the deflection angles.
         deflections_x
-            Whether or not to  include a 2D plot (via `imshow`) of the x component of the deflection angles.
+            Whether or not to include a 2D plot (via `imshow`) of the x component of the deflection angles.
         magnification
-            Whether or not to  include a 2D plot (via `imshow`) of the magnification.
+            Whether or not to include a 2D plot (via `imshow`) of the magnification.
         auto_filename
             The default filename of the output subplot if written to hard-disk.
         """
         self._subplot_custom_plot(
             image=image,
-            plane_image=plane_image,
-            plane_grid=plane_grid,
             convergence=convergence,
             potential=potential,
             deflections_y=deflections_y,
             deflections_x=deflections_x,
             magnification=magnification,
             auto_labels=aplt.AutoLabels(filename=auto_filename),
         )
 
-    def subplot_plane(self):
+    def subplot_galaxies(self):
         """
-        Standard subplot of the attributes of the plotter's `Plane` object.
+        Standard subplot of the attributes of the plotter's `Galaxies` object.
         """
         return self.subplot(
             image=True,
             convergence=True,
             potential=True,
             deflections_y=True,
             deflections_x=True,
         )
 
     def subplot_galaxy_images(self):
         """
-        Subplot of the image of every galaxy in the plane.
+        Subplot of the image of every galaxy.
 
-        For example, for a 2 galaxy `Plane`, this creates a subplot with 2 panels, one for each galaxy.
+        For example, for a 2 galaxy `Galaxies`, this creates a subplot with 2 panels, one for each galaxy.
         """
-        number_subplots = len(self.plane.galaxies)
+        number_subplots = len(self.galaxies)
 
         self.open_subplot_figure(number_subplots=number_subplots)
 
-        for galaxy_index in range(0, len(self.plane.galaxies)):
+        for galaxy_index in range(0, len(self.galaxies)):
             galaxy_plotter = self.galaxy_plotter_from(galaxy_index=galaxy_index)
             galaxy_plotter.figures_2d(
-                image=True, title_suffix=f" Of Plane {galaxy_index}"
+                image=True, title_suffix=f" Of Galaxies {galaxy_index}"
             )
 
         self.mat_plot_2d.output.subplot_to_figure(
             auto_filename=f"subplot_galaxy_images"
         )
         self.close_subplot_figure()
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/plane/to_inversion.py` & `autogalaxy-2024.5.16.0/autogalaxy/galaxy/to_inversion.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 from __future__ import annotations
-from typing import TYPE_CHECKING, Dict, List, Optional, Type, Union
-
-if TYPE_CHECKING:
-    from autogalaxy.plane.plane import Plane
+from typing import Dict, List, Optional, Type, Union
 
 from autoconf import cached_property
 
 import autoarray as aa
 
 from autoarray.inversion.pixelization.mappers.factory import mapper_from
-from autoarray.inversion.inversion.factory import inversion_unpacked_from
-from autogalaxy.analysis.adapt_images import AdaptImages
+from autoarray.inversion.inversion.factory import inversion_from
+from autogalaxy.analysis.adapt_images.adapt_images import AdaptImages
 from autogalaxy.profiles.light.linear import (
     LightProfileLinearObjFuncList,
 )
 from autogalaxy.profiles.light.basis import Basis
+from autogalaxy.profiles.light.abstract import LightProfile
 from autogalaxy.profiles.light.linear import LightProfileLinear
 from autogalaxy.galaxy.galaxy import Galaxy
+from autogalaxy.galaxy.galaxies import Galaxies
 from autogalaxy.analysis.preloads import Preloads
 
 
 class AbstractToInversion:
     def __init__(
         self,
-        dataset: Optional[Union[aa.Imaging, aa.Interferometer]] = None,
-        data: Optional[Union[aa.Array2D, aa.Visibilities]] = None,
-        noise_map: Optional[Union[aa.Array2D, aa.VisibilitiesNoiseMap]] = None,
-        w_tilde: Optional[Union[aa.WTildeImaging, aa.WTildeInterferometer]] = None,
+        dataset: Optional[Union[aa.Imaging, aa.Interferometer, aa.DatasetInterface]],
         adapt_images: Optional[AdaptImages] = None,
         settings_inversion: aa.SettingsInversion = aa.SettingsInversion(),
         preloads=Preloads(),
         run_time_dict: Optional[Dict] = None,
     ):
         if dataset is not None:
             if dataset.noise_covariance_matrix is not None:
@@ -41,24 +37,41 @@
                     
                     This is because the linear algebra implementation is only valid under the assumption 
                     of independent gaussian noise.
                     """
                 )
 
         self.dataset = dataset
-        self.data = data
-        self.noise_map = noise_map
-        self.w_tilde = w_tilde
+
         self.adapt_images = adapt_images
 
         self.settings_inversion = settings_inversion
 
         self.preloads = preloads
         self.run_time_dict = run_time_dict
 
+    @property
+    def convolver(self):
+        try:
+            return self.dataset.convolver
+        except AttributeError:
+            return None
+
+    @property
+    def transformer(self):
+        try:
+            return self.dataset.transformer
+        except AttributeError:
+            return None
+
+    @property
+    def border_relocator(self):
+        if self.settings_inversion.use_border_relocator:
+            return self.dataset.border_relocator
+
     def cls_light_profile_func_list_galaxy_dict_from(
         self, cls: Type
     ) -> Dict[LightProfileLinearObjFuncList, Galaxy]:
         raise NotImplementedError
 
     @cached_property
     def lp_linear_func_list_galaxy_dict(
@@ -85,89 +98,64 @@
         return list(self.linear_obj_galaxy_dict.keys())
 
     @cached_property
     def regularization_list(self) -> List[aa.AbstractRegularization]:
         return [linear_obj.regularization for linear_obj in self.linear_obj_list]
 
 
-class PlaneToInversion(AbstractToInversion):
+class GalaxiesToInversion(AbstractToInversion):
     def __init__(
         self,
-        plane: Plane,
-        dataset: Optional[Union[aa.Imaging, aa.Interferometer]] = None,
-        data: Optional[Union[aa.Array2D, aa.Visibilities]] = None,
-        noise_map: Optional[Union[aa.Array2D, aa.VisibilitiesNoiseMap]] = None,
-        w_tilde: Optional[Union[aa.WTildeImaging, aa.WTildeInterferometer]] = None,
+        dataset: Optional[Union[aa.Imaging, aa.Interferometer, aa.DatasetInterface]],
+        galaxies: List[Galaxy],
         adapt_images: Optional[AdaptImages] = None,
-        grid: Optional[aa.type.Grid2DLike] = None,
-        blurring_grid: Optional[aa.type.Grid2DLike] = None,
-        grid_pixelization: Optional[aa.type.Grid2DLike] = None,
         settings_inversion: aa.SettingsInversion = aa.SettingsInversion(),
         preloads=aa.Preloads(),
         run_time_dict: Optional[Dict] = None,
     ):
-        self.plane = plane
+        self.galaxies = Galaxies(galaxies)
 
         super().__init__(
             dataset=dataset,
-            data=data,
-            noise_map=noise_map,
-            w_tilde=w_tilde,
             adapt_images=adapt_images,
             settings_inversion=settings_inversion,
             preloads=preloads,
             run_time_dict=run_time_dict,
         )
 
-        if grid is not None:
-            self.grid = grid
-        elif dataset is not None:
-            self.grid = dataset.grid
-        else:
-            self.grid = None
-
-        if blurring_grid is not None:
-            self.blurring_grid = blurring_grid
-        elif dataset is not None:
-            self.blurring_grid = dataset.blurring_grid
-        else:
-            self.blurring_grid = None
-
-        if grid_pixelization is not None:
-            self.grid_pixelization = grid_pixelization
-        elif dataset is not None:
-            self.grid_pixelization = dataset.grid_pixelization
-        else:
-            self.grid_pixelization = None
+    @property
+    def has_mapper(self):
+        if self.galaxies.has(cls=aa.Pixelization):
+            return True
 
     def cls_light_profile_func_list_galaxy_dict_from(
         self, cls: Type
     ) -> Dict[LightProfileLinearObjFuncList, Galaxy]:
-        if not self.plane.has(cls=cls):
+        if not self.galaxies.has(cls=cls):
             return {}
 
         lp_linear_func_galaxy_dict = {}
 
-        for galaxy in self.plane.galaxies:
+        for galaxy in self.galaxies:
             if galaxy.has(cls=cls):
                 for light_profile in galaxy.cls_list_from(cls=cls):
                     if isinstance(light_profile, LightProfileLinear):
                         light_profile_list = [light_profile]
                     else:
                         light_profile_list = light_profile.light_profile_list
                         light_profile_list = [
                             light_profile
                             for light_profile in light_profile_list
                             if isinstance(light_profile, LightProfileLinear)
                         ]
 
                     if len(light_profile_list) > 0:
                         lp_linear_func = LightProfileLinearObjFuncList(
-                            grid=self.grid,
-                            blurring_grid=self.blurring_grid,
+                            grid=self.dataset.grid,
+                            blurring_grid=self.dataset.blurring_grid,
                             convolver=self.dataset.convolver,
                             light_profile_list=light_profile_list,
                             regularization=light_profile.regularization,
                         )
 
                         lp_linear_func_galaxy_dict[lp_linear_func] = galaxy
 
@@ -190,20 +178,20 @@
             **lp_basis_func_list_galaxy_dict,
         }
 
     @cached_property
     def image_plane_mesh_grid_list(
         self,
     ) -> Optional[List[aa.Grid2DIrregular]]:
-        if not self.plane.has(cls=aa.Pixelization):
+        if not self.galaxies.galaxy_has_cls(cls=aa.Pixelization):
             return None
 
         image_plane_mesh_grid_list = []
 
-        for galaxy in self.plane.galaxies_with_cls_list_from(cls=aa.Pixelization):
+        for galaxy in self.galaxies.galaxies_with_cls_list_from(cls=aa.Pixelization):
             pixelization = galaxy.cls_list_from(cls=aa.Pixelization)[0]
 
             if pixelization.image_mesh is not None:
                 try:
                     adapt_data = self.adapt_images.galaxy_image_dict[galaxy]
                 except (AttributeError, KeyError):
                     adapt_data = None
@@ -217,15 +205,15 @@
                             However, the adapt-images passed to the fit (E.g. FitImaging, FitInterferometer) 
                             is None. Without an adapt image, an image-mesh cannot be used.
                             """
                         )
 
                 image_plane_mesh_grid = (
                     pixelization.image_mesh.image_plane_mesh_grid_from(
-                        grid=self.grid_pixelization,
+                        mask=self.dataset.mask,
                         adapt_data=adapt_data,
                         settings=self.settings_inversion,
                     )
                 )
 
             else:
                 image_plane_mesh_grid = None
@@ -235,72 +223,83 @@
         return image_plane_mesh_grid_list
 
     def mapper_from(
         self,
         mesh: aa.AbstractMesh,
         regularization: aa.AbstractRegularization,
         source_plane_mesh_grid: aa.Grid2DIrregular,
+        source_plane_data_grid: aa.Grid2D,
         adapt_galaxy_image: aa.Array2D,
         image_plane_mesh_grid: Optional[aa.Grid2DIrregular] = None,
     ) -> aa.AbstractMapper:
         mapper_grids = mesh.mapper_grids_from(
-            source_plane_data_grid=self.grid_pixelization,
+            mask=self.dataset.mask,
+            border_relocator=self.border_relocator,
+            source_plane_data_grid=source_plane_data_grid,
             source_plane_mesh_grid=source_plane_mesh_grid,
             image_plane_mesh_grid=image_plane_mesh_grid,
-            relocate_pix_border=self.settings_inversion.relocate_pix_border,
             adapt_data=adapt_galaxy_image,
             preloads=self.preloads,
-            run_time_dict=self.plane.run_time_dict,
+            run_time_dict=self.run_time_dict,
         )
 
-        return mapper_from(mapper_grids=mapper_grids, regularization=regularization)
+        return mapper_from(
+            mapper_grids=mapper_grids,
+            over_sampler=self.dataset.grid_pixelization.over_sampling.over_sampler_from(
+                mask=self.dataset.mask
+            ),
+            regularization=regularization,
+            run_time_dict=self.run_time_dict,
+        )
 
     @cached_property
     def mapper_galaxy_dict(self) -> Dict[aa.AbstractMapper, Galaxy]:
-        if not self.plane.has(cls=aa.Pixelization):
+        if not self.galaxies.galaxy_has_cls(cls=aa.Pixelization):
             return {}
 
         mesh_grid_list = self.image_plane_mesh_grid_list
 
         mapper_galaxy_dict = {}
 
-        pixelization_list = self.plane.cls_list_from(cls=aa.Pixelization)
-        galaxies_with_pixelization_list = self.plane.galaxies_with_cls_list_from(
+        pixelization_list = []
+
+        galaxies_with_pixelization_list = self.galaxies.galaxies_with_cls_list_from(
             cls=aa.Pixelization
         )
 
+        for pix in self.galaxies.cls_list_from(cls=aa.Pixelization):
+            pixelization_list.append(pix)
+
         for mapper_index in range(len(mesh_grid_list)):
             galaxy = galaxies_with_pixelization_list[mapper_index]
 
             try:
                 adapt_galaxy_image = self.adapt_images.galaxy_image_dict[galaxy]
             except (AttributeError, KeyError):
                 adapt_galaxy_image = None
 
             mapper = self.mapper_from(
                 mesh=pixelization_list[mapper_index].mesh,
                 regularization=pixelization_list[mapper_index].regularization,
+                source_plane_data_grid=self.dataset.grid_pixelization.over_sampler.over_sampled_grid,
                 source_plane_mesh_grid=mesh_grid_list[mapper_index],
                 adapt_galaxy_image=adapt_galaxy_image,
                 image_plane_mesh_grid=mesh_grid_list[mapper_index],
             )
 
             mapper_galaxy_dict[mapper] = galaxy
 
         return mapper_galaxy_dict
 
     @property
     def inversion(self) -> aa.AbstractInversion:
-        inversion = inversion_unpacked_from(
+        inversion = inversion_from(
             dataset=self.dataset,
-            data=self.data,
-            noise_map=self.noise_map,
-            w_tilde=self.w_tilde,
             linear_obj_list=self.linear_obj_list,
             settings=self.settings_inversion,
             preloads=self.preloads,
-            run_time_dict=self.plane.run_time_dict,
+            run_time_dict=self.run_time_dict,
         )
 
         inversion.linear_obj_galaxy_dict = self.linear_obj_galaxy_dict
 
         return inversion
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/plot/__init__.py` & `autogalaxy-2024.5.16.0/autogalaxy/plot/__init__.py`

 * *Files 23% similar despite different names*

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
 
 from autoarray.plot.wrap.base import (
     Units,
     Figure,
     Axis,
     Cmap,
     Colorbar,
@@ -78,18 +74,20 @@
 from autogalaxy.plot.include.one_d import Include1D
 from autogalaxy.plot.include.two_d import Include2D
 from autogalaxy.plot.visuals.one_d import Visuals1D
 from autogalaxy.plot.visuals.two_d import Visuals2D
 
 from autogalaxy.profiles.plot.light_profile_plotters import LightProfilePlotter
 from autogalaxy.profiles.plot.light_profile_plotters import LightProfilePDFPlotter
+from autogalaxy.profiles.plot.basis_plotters import BasisPlotter
 from autogalaxy.profiles.plot.mass_profile_plotters import MassProfilePlotter
 from autogalaxy.profiles.plot.mass_profile_plotters import MassProfilePDFPlotter
 from autogalaxy.galaxy.plot.galaxy_plotters import GalaxyPlotter
 from autogalaxy.galaxy.plot.galaxy_plotters import GalaxyPDFPlotter
+from autogalaxy.galaxy.plot.galaxies_plotters import GalaxiesPlotter
 from autogalaxy.quantity.plot.fit_quantity_plotters import FitQuantityPlotter
 from autogalaxy.imaging.plot.fit_imaging_plotters import FitImagingPlotter
 from autogalaxy.interferometer.plot.fit_interferometer_plotters import (
     FitInterferometerPlotter,
 )
-from autogalaxy.plane.plot.plane_plotters import PlanePlotter
+from autogalaxy.galaxy.plot.galaxies_plotters import GalaxiesPlotter
 from autogalaxy.galaxy.plot.adapt_plotters import AdaptPlotter
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/plot/abstract_plotters.py` & `autogalaxy-2024.5.16.0/autogalaxy/plot/abstract_plotters.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/plot/get_visuals/one_d.py` & `autogalaxy-2024.5.16.0/autogalaxy/plot/get_visuals/one_d.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/plot/get_visuals/two_d.py` & `autogalaxy-2024.5.16.0/autogalaxy/plot/get_visuals/two_d.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-from typing import Union
+from typing import List, Union
 
 import autoarray as aa
 import autoarray.plot as aplt
 
 from autogalaxy.imaging.fit_imaging import FitImaging
 from autogalaxy.plot.include.two_d import Include2D
 from autogalaxy.plot.visuals.two_d import Visuals2D
 from autogalaxy.profiles.light.abstract import LightProfile
 from autogalaxy.profiles.mass.abstract.abstract import MassProfile
 from autogalaxy.galaxy.galaxy import Galaxy
-from autogalaxy.plane.plane import Plane
 
 
 class GetVisuals2D(aplt.GetVisuals2D):
     def __init__(self, include: Include2D, visuals: Visuals2D):
         """
         Class which gets 2D attributes and adds them to a `Visuals2D` objects, such that they are plotted on 2D figures.
 
@@ -31,18 +30,18 @@
             are extracted via the `GetVisuals2D` object).
         visuals
             The pre-existing visuals of the plotter which new visuals are added too via the `GetVisuals2D` class.
         """
         super().__init__(include=include, visuals=visuals)
 
     def via_light_obj_from(
-        self, light_obj: Union[LightProfile, Galaxy, Plane], grid
+        self, light_obj: Union[LightProfile, Galaxy], grid
     ) -> Visuals2D:
         """
-        From an object with light profiles (e.g. a `LightProfile`, `Galaxy`, `Plane`) get its attributes that can be
+        From an object with light profiles (e.g. a `LightProfile`, `Galaxy`) get its attributes that can be
         plotted and return them  in a `Visuals2D` object.
 
         Only attributes not already in `self.visuals` and with `True` entries in the `Include1D` object are extracted
         for plotting.
 
         From a light object the following 2D attributes can be extracted for plotting:
 
@@ -50,15 +49,15 @@
         - mask: the mask of the grid used to plot the light object's quantities in 2D.
         - border: the border of this mask.
         - light profile centres: the (y,x) centre of every `LightProfile` in the object.
 
         Parameters
         ----------
         light_obj
-            The light object (e.g. a `LightProfile`, `Galaxy`, `Plane`) whose attributes are extracted for plotting.
+            The light object (e.g. a `LightProfile`, `Galaxy`) whose attributes are extracted for plotting.
         grid
             The 2D grid of (y,x) coordinates used to plot the light object's quantities in 2D.
 
         Returns
         -------
         vis.Visuals2D
             The collection of attributes that can be plotted by a `Plotter` object.
@@ -80,18 +79,18 @@
         return (
             self.visuals
             + visuals_via_mask
             + self.visuals.__class__(light_profile_centres=light_profile_centres)
         )
 
     def via_mass_obj_from(
-        self, mass_obj: Union[MassProfile, Galaxy, Plane], grid: aa.type.Grid2DLike
+        self, mass_obj: Union[MassProfile, Galaxy], grid: aa.type.Grid2DLike
     ) -> Visuals2D:
         """
-        From an object with mass profiles (e.g. a `MassProfile`, `Galaxy`, `Plane`) get its attributes that can be
+        From an object with mass profiles (e.g. a `MassProfile`, `Galaxy`) get its attributes that can be
         plotted and return them  in a `Visuals2D` object.
 
         Only attributes not already in `self.visuals` and with `True` entries in the `Include1D` object are extracted
         for plotting.
 
         From a mass object the following 2D attributes can be extracted for plotting:
 
@@ -100,15 +99,15 @@
         - border: the border of this mask.
         - mass profile centres: the (y,x) centre of every `MassProfile` in the mass object.
         - critical curves: the critical curves of the mass object.
 
         Parameters
         ----------
         mass_obj
-            The mass object (e.g. a `MassProfile`, `Galaxy`, `Plane`) whose attributes are extracted for plotting.
+            The mass object (e.g. a `MassProfile`, `Galaxy`) whose attributes are extracted for plotting.
         grid
             The 2D grid of (y,x) coordinates used to plot the mass object's quantities in 2D.
 
         Returns
         -------
         vis.Visuals2D
             The collection of attributes that can be plotted by a `Plotter` object.
@@ -152,34 +151,32 @@
             + self.visuals.__class__(
                 mass_profile_centres=mass_profile_centres,
                 tangential_critical_curves=tangential_critical_curves,
                 radial_critical_curves=radial_critical_curves,
             )
         )
 
-    def via_light_mass_obj_from(
-        self, light_mass_obj: Union[Galaxy, Plane], grid
-    ) -> Visuals2D:
+    def via_light_mass_obj_from(self, light_mass_obj: Union[Galaxy], grid) -> Visuals2D:
         """
-        From an object that contains both light profiles and / or mass profiles (e.g. a `Galaxy`, `Plane`), get the
+        From an object that contains both light profiles and / or mass profiles (e.g. a `Galaxy`), get the
         attributes that can be plotted and returns them in a `Visuals2D` object.
 
         Only attributes with `True` entries in the `Include` object are extracted.
 
         From a light and lensing object the following attributes can be extracted for plotting:
 
         - origin: the (y,x) origin of the coordinate system used to plot the light object's quantities in 2D.
         - light profile centres: the (y,x) centre of every `LightProfile` in the object.
         - mass profile centres: the (y,x) centre of every `MassProfile` in the object.
         - critical curves: the critical curves of all mass profile combined.
 
         Parameters
         ----------
         light_mass_obj
-            The light and mass object (e.g. a `Galaxy`, `Plane`) whose attributes are extracted for plotting.
+            The light and mass object (e.g. a `Galaxy`) whose attributes are extracted for plotting.
         grid
             The 2D grid of (y,x) coordinates used to plot the light and mass object's quantities in 2D.
 
         Returns
         -------
         vis.Visuals2D
             A collection of attributes that can be plotted by a `Plotter` object.
@@ -192,110 +189,70 @@
 
         return (
             visuals_2d
             + visuals_with_grid
             + self.via_light_obj_from(light_obj=light_mass_obj, grid=grid)
         )
 
-    def via_plane_from(
-        self, plane: Plane, grid: aa.type.Grid2DLike, galaxy_index: int
+    def via_galaxies_from(
+        self, galaxies: List[Galaxy], grid: aa.type.Grid2DLike, galaxy_index: int
     ) -> Visuals2D:
         """
-        From a `Plane` get the attributes that can be plotted and returns them in a `Visuals2D` object.
+        From a list of galaxies get the attributes that can be plotted and returns them in a `Visuals2D` object.
 
         Only attributes with `True` entries in the `Include` object are extracted.
 
-        From a plane the following attributes can be extracted for plotting:
+        From a list of galaxie the following attributes can be extracted for plotting:
 
         - origin: the (y,x) origin of the coordinate system used to plot the light object's quantities in 2D.
         - border: the border of the mask of the grid used to plot the light object's quantities in 2D.
         - light profile centres: the (y,x) centre of every `LightProfile` in the object.
         - mass profile centres: the (y,x) centre of every `MassProfile` in the object.
-        - critical curves: the critical curves of all of the plane's mass profiles combined.
-        - caustics: the caustics of all of the plane's mass profiles combined.
+        - critical curves: the critical curves of all of the galaxy's mass profiles combined.
+        - caustics: the caustics of all of the galaxy's mass profiles combined.
 
-        When plotting a `Plane` it is common for plots to only display quantities corresponding to one galaxy at a time
-        (e.g. the image of each galaxy). Therefore, quantities are only extracted from one plane, specified by the
+        When plotting galaxies it is common for plots to only display quantities corresponding to one galaxy at a time
+        (e.g. the image of each galaxy). Therefore, quantities are only extracted from one galaxy, specified by the
         input `galaxy_index`.
 
         Parameters
         ----------
-        plane
-            The `Plane` object which has attributes extracted for plotting.
+        galaxies
+            The galaxies which have attributes extracted for plotting.
         grid
-            The 2D grid of (y,x) coordinates used to plot the plane's quantities in 2D.
+            The 2D grid of (y,x) coordinates used to plot the galaxies quantities in 2D.
         galaxy_index
-            The index of the plane in the plane which is used to extract quantities, as only one plane is plotted
+            The index of the galaxy in the galaxies which is used to extract quantities, as only one galaxy is plotted
             at a time.
 
         Returns
         -------
         vis.Visuals2D
             A collection of attributes that can be plotted by a `Plotter` object.
         """
         origin = self.get("origin", value=aa.Grid2DIrregular(values=[grid.origin]))
 
         light_profile_centres = self.get(
             "light_profile_centres",
-            plane.galaxies[galaxy_index].extract_attribute(
+            galaxies[galaxy_index].extract_attribute(
                 cls=LightProfile, attr_name="centre"
             ),
         )
 
         mass_profile_centres = self.get(
             "mass_profile_centres",
-            plane.galaxies[galaxy_index].extract_attribute(
+            galaxies[galaxy_index].extract_attribute(
                 cls=MassProfile, attr_name="centre"
             ),
         )
 
-        if galaxy_index == 0:
-            tangential_critical_curves = self.get(
-                "tangential_critical_curves",
-                plane.tangential_critical_curve_list_from(grid=grid),
-                "tangential_critical_curves",
-            )
-        else:
-            tangential_critical_curves = None
-
-        if galaxy_index == 0:
-            radial_critical_curves = self.get(
-                "radial_critical_curves",
-                plane.radial_critical_curve_list_from(grid=grid),
-                "radial_critical_curves",
-            )
-        else:
-            radial_critical_curves = None
-
-        if galaxy_index == 1:
-            tangential_caustics = self.get(
-                "tangential_caustics",
-                plane.tangential_caustic_list_from(grid=grid),
-                "tangential_caustics",
-            )
-        else:
-            tangential_caustics = None
-
-        if galaxy_index == 1:
-            radial_caustics = self.get(
-                "radial_caustics",
-                plane.radial_caustic_list_from(grid=grid),
-                "radial_caustics",
-            )
-        else:
-            radial_caustics = None
-
         return self.visuals + self.visuals.__class__(
             origin=origin,
             light_profile_centres=light_profile_centres,
             mass_profile_centres=mass_profile_centres,
-            tangential_critical_curves=tangential_critical_curves,
-            radial_critical_curves=radial_critical_curves,
-            tangential_caustics=tangential_caustics,
-            radial_caustics=radial_caustics,
         )
 
     def via_fit_imaging_from(self, fit: FitImaging) -> Visuals2D:
         """
         From a `FitImaging` get its attributes that can be plotted and return them in a `Visuals2D` object.
 
         Only attributes not already in `self.visuals` and with `True` entries in the `Include2D` object are extracted
@@ -319,11 +276,11 @@
         -------
         Visuals2D
             The collection of attributes that are plotted by a `Plotter` object.
         """
         visuals_2d_via_fit = super().via_fit_imaging_from(fit=fit)
 
         visuals_2d_via_light_mass_obj = self.via_light_mass_obj_from(
-            light_mass_obj=fit.plane, grid=fit.grid
+            light_mass_obj=fit.galaxies, grid=fit.grid
         )
 
         return visuals_2d_via_fit + visuals_2d_via_light_mass_obj
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/plot/include/one_d.py` & `autogalaxy-2024.5.16.0/autogalaxy/plot/include/one_d.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/plot/include/two_d.py` & `autogalaxy-2024.5.16.0/autogalaxy/plot/include/two_d.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/plot/mass_plotter.py` & `autogalaxy-2024.5.16.0/autogalaxy/plot/mass_plotter.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/plot/mat_plot/one_d.py` & `autogalaxy-2024.5.16.0/autogalaxy/plot/mat_plot/one_d.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/plot/mat_plot/two_d.py` & `autogalaxy-2024.5.16.0/autogalaxy/plot/mat_plot/two_d.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
         interpolated_reconstruction: Optional[aplt.InterpolatedReconstruction] = None,
         voronoi_drawer: Optional[aplt.VoronoiDrawer] = None,
         origin_scatter: Optional[aplt.OriginScatter] = None,
         mask_scatter: Optional[aplt.MaskScatter] = None,
         border_scatter: Optional[aplt.BorderScatter] = None,
         positions_scatter: Optional[aplt.PositionsScatter] = None,
         index_scatter: Optional[aplt.IndexScatter] = None,
+        index_plot: Optional[aplt.IndexPlot] = None,
         mesh_grid_scatter: Optional[aplt.MeshGridScatter] = None,
         light_profile_centres_scatter: Optional[w.LightProfileCentresScatter] = None,
         mass_profile_centres_scatter: Optional[w.MassProfileCentresScatter] = None,
         multiple_images_scatter: Optional[w.MultipleImagesScatter] = None,
         tangential_critical_curves_plot: Optional[
             w.TangentialCriticalCurvesPlot
         ] = None,
@@ -190,14 +191,15 @@
             output=output,
             origin_scatter=origin_scatter,
             mask_scatter=mask_scatter,
             border_scatter=border_scatter,
             grid_scatter=grid_scatter,
             positions_scatter=positions_scatter,
             index_scatter=index_scatter,
+            index_plot=index_plot,
             mesh_grid_scatter=mesh_grid_scatter,
             vector_yx_quiver=vector_yx_quiver,
             patch_overlay=patch_overlay,
             array_overlay=array_overlay,
             contour=contour,
             grid_plot=grid_plot,
             interpolated_reconstruction=interpolated_reconstruction,
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/plot/visuals/one_d.py` & `autogalaxy-2024.5.16.0/autogalaxy/plot/visuals/one_d.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/plot/visuals/two_d.py` & `autogalaxy-2024.5.16.0/autogalaxy/plot/visuals/two_d.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,17 +59,17 @@
         self.mass_profile_centres = mass_profile_centres
         self.multiple_images = multiple_images
         self.tangential_critical_curves = tangential_critical_curves
         self.radial_critical_curves = radial_critical_curves
         self.tangential_caustics = tangential_caustics
         self.radial_caustics = radial_caustics
 
-    def plot_via_plotter(self, plotter, grid_indexes=None, mapper=None):
+    def plot_via_plotter(self, plotter, grid_indexes=None, mapper=None, geometry=None):
         super().plot_via_plotter(
-            plotter=plotter, grid_indexes=grid_indexes, mapper=mapper
+            plotter=plotter, grid_indexes=grid_indexes, mapper=mapper, geometry=geometry
         )
 
         if self.light_profile_centres is not None:
             plotter.light_profile_centres_scatter.scatter_grid(
                 grid=self.light_profile_centres
             )
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/plot/wrap.py` & `autogalaxy-2024.5.16.0/autogalaxy/plot/wrap.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/geometry_profiles.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/geometry_profiles.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Optional, Tuple, Type
 
 import numpy as np
 
 import autoarray as aa
-from autoarray.structures.grids.transformed_2d import Grid2DTransformedNumpy
+
 from autogalaxy import convert
 
 
 class GeometryProfile:
     """
     An abstract geometry profile, which describes profiles with y and x centre Cartesian coordinates
 
@@ -34,21 +34,23 @@
 
     def has(self, cls: Type) -> bool:
         """
         Does this instance have an attribute which is of type cls?
         """
         return aa.util.misc.has(values=self.__dict__.values(), cls=cls)
 
-    def transformed_to_reference_frame_grid_from(self, grid):
+    def transformed_to_reference_frame_grid_from(self, grid, **kwargs):
         raise NotImplemented()
 
-    def transformed_from_reference_frame_grid_from(self, grid):
+    def transformed_from_reference_frame_grid_from(self, grid, **kwargs):
         raise NotImplemented()
 
-    def _radial_projected_shape_slim_from(self, grid: aa.type.Grid1D2DLike) -> int:
+    def _radial_projected_shape_slim_from(
+        self, grid: aa.type.Grid1D2DLike, **kwargs
+    ) -> int:
         """
         To make 1D plots (e.g. `image_1d_from()`) from an input 2D grid, one uses that 2D grid to radially project
         the coordinates across the profile's major-axis.
 
         This function computes the distance from the profile centre to the edge of this 2D grid.
 
         If a 1D grid is input it returns the shape of this grid, as the grid itself defines the radial coordinates.
@@ -76,45 +78,44 @@
     centre
         The (y,x) arc-second coordinates of the profile centre.
     """
 
     def __init__(self, centre: Tuple[float, float] = (0.0, 0.0)):
         super().__init__(centre=centre)
 
-    @aa.grid_dec.grid_2d_to_structure
-    @aa.grid_dec.transform
-    def radial_grid_from(self, grid: aa.type.Grid2DLike) -> np.ndarray:
+    @aa.grid_dec.to_array
+    def radial_grid_from(self, grid: aa.type.Grid2DLike, **kwargs) -> np.ndarray:
         """
         Convert a grid of (y, x) coordinates, to their radial distances from the profile
         centre (e.g. :math: r = x**2 + y**2).
 
         Parameters
         ----------
         grid
             The grid of (y, x) coordinates which are converted to radial distances.
         """
         return np.sqrt(np.add(np.square(grid[:, 0]), np.square(grid[:, 1])))
 
     def angle_to_profile_grid_from(
-        self, grid_angles: np.ndarray
+        self, grid_angles: np.ndarray, **kwargs
     ) -> Tuple[np.ndarray, np.ndarray]:
         """
         Convert a grid of angles, defined in degrees counter-clockwise from the positive x-axis, to a grid of
         angles between the input angles and the profile.
 
         Parameters
         ----------
         grid_angles
             The angle theta counter-clockwise from the positive x-axis to each coordinate in radians.
         """
         return np.cos(grid_angles), np.sin(grid_angles)
 
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.grid_dec.to_grid
     def _cartesian_grid_via_radial_from(
-        self, grid: aa.type.Grid2DLike, radius: np.ndarray
+        self, grid: aa.type.Grid2DLike, radius: np.ndarray, **kwargs
     ) -> aa.type.Grid2DLike:
         """
         Convert a grid of (y,x) coordinates with their specified radial distances (e.g. :math: r = x**2 + y**2) to
         their original (y,x) Cartesian coordinates.
 
         Parameters
         ----------
@@ -123,44 +124,42 @@
         radius
             The circular radius of each coordinate from the profile center.
         """
         grid_angles = np.arctan2(grid[:, 0], grid[:, 1])
         cos_theta, sin_theta = self.angle_to_profile_grid_from(grid_angles=grid_angles)
         return np.multiply(radius[:, None], np.vstack((sin_theta, cos_theta)).T)
 
-    @aa.grid_dec.grid_2d_to_structure
-    def transformed_to_reference_frame_grid_from(self, grid):
+    @aa.grid_dec.to_grid
+    def transformed_to_reference_frame_grid_from(self, grid, **kwargs):
         """
         Transform a grid of (y,x) coordinates to the reference frame of the profile.
 
         This performs a translation to the profile's `centre`.
 
         Parameters
         ----------
         grid
             The (y, x) coordinates in the original reference frame of the grid.
         """
-        transformed = np.subtract(grid, self.centre)
-        return Grid2DTransformedNumpy(values=transformed)
+        return np.subtract(grid, self.centre)
 
-    @aa.grid_dec.grid_2d_to_structure
-    def transformed_from_reference_frame_grid_from(self, grid):
+    @aa.grid_dec.to_grid
+    def transformed_from_reference_frame_grid_from(self, grid, **kwargs):
         """
         Transform a grid of (y,x) coordinates from the reference frame of the profile to the original observer
         reference frame.
 
         This performs a translation from the profile's `centre`.
 
         Parameters
         ----------
         grid
             The (y, x) coordinates in the reference frame of the profile.
         """
-        transformed = np.add(grid, self.centre)
-        return transformed.view(Grid2DTransformedNumpy)
+        return np.add(grid, self.centre)
 
 
 class EllProfile(SphProfile):
     def __init__(
         self,
         centre: Tuple[float, float] = (0.0, 0.0),
         ell_comps: Tuple[float, float] = (0.0, 0.0),
@@ -237,37 +236,37 @@
     def _cos_angle(self) -> float:
         return self._cos_and_sin_to_x_axis()[0]
 
     @property
     def _sin_angle(self) -> float:
         return self._cos_and_sin_to_x_axis()[1]
 
-    def _cos_and_sin_to_x_axis(self):
+    def _cos_and_sin_to_x_axis(self, **kwargs):
         """
         Determine the sin and cosine of the angle between the profile's ellipse and the positive x-axis,
         counter-clockwise.
         """
         angle_radians = np.radians(self.angle)
         return np.cos(angle_radians), np.sin(angle_radians)
 
-    def angle_to_profile_grid_from(self, grid_angles):
+    def angle_to_profile_grid_from(self, grid_angles, **kwargs):
         """
         The angle between each angle theta on the grid and the profile, in radians.
 
         Parameters
         ----------
         grid_angles
             The angle theta counter-clockwise from the positive x-axis to each coordinate in radians.
         """
         theta_coordinate_to_profile = np.add(grid_angles, -self.angle_radians)
         return np.cos(theta_coordinate_to_profile), np.sin(theta_coordinate_to_profile)
 
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.grid_dec.to_grid
     def rotated_grid_from_reference_frame_from(
-        self, grid, angle: Optional[float] = None
+        self, grid, angle: Optional[float] = None, **kwargs
     ):
         """
         Rotate a grid of (y,x) coordinates which have been transformed to the elliptical reference frame of a profile
         back to the original unrotated coordinate grid reference frame.
 
         Note that unlike the method `transformed_from_reference_frame_grid_from` the coordinates are not
         translated back to the profile's original centre.
@@ -288,98 +287,93 @@
         if angle is None:
             angle = self.angle
 
         return aa.util.geometry.transform_grid_2d_from_reference_frame(
             grid_2d=grid, centre=(0.0, 0.0), angle=angle
         )
 
-    @aa.grid_dec.grid_2d_to_structure
-    @aa.grid_dec.transform
+    @aa.grid_dec.to_array
     @aa.grid_dec.relocate_to_radial_minimum
-    def elliptical_radii_grid_from(self, grid: aa.type.Grid2DLike) -> np.ndarray:
+    def elliptical_radii_grid_from(
+        self, grid: aa.type.Grid2DLike, **kwargs
+    ) -> np.ndarray:
         """
         Convert a grid of (y,x) coordinates to their elliptical radii values: :math: (x^2 + (y^2/q))^0.5
 
-        If the coordinates have not been transformed to the profile's geometry (e.g. translated to the
-        profile `centre`), this is performed automatically.
-
         Parameters
         ----------
         grid
             The (y, x) coordinates in the reference frame of the elliptical profile.
         """
         return np.sqrt(
             np.add(
                 np.square(grid[:, 1]), np.square(np.divide(grid[:, 0], self.axis_ratio))
             )
         )
 
-    @aa.grid_dec.grid_2d_to_structure
-    @aa.grid_dec.transform
+    @aa.grid_dec.to_array
     @aa.grid_dec.relocate_to_radial_minimum
-    def eccentric_radii_grid_from(self, grid: aa.type.Grid2DLike) -> np.ndarray:
+    def eccentric_radii_grid_from(
+        self, grid: aa.type.Grid2DLike, **kwargs
+    ) -> np.ndarray:
         """
         Convert a grid of (y,x) coordinates to an eccentric radius: :math: axis_ratio^0.5 (x^2 + (y^2/q))^0.5
 
         This is used in certain light profiles define their half-light radii as a circular radius.
 
         If the coordinates have not been transformed to the profile's geometry (e.g. translated to the
         profile `centre`), this is performed automatically.
 
         Parameters
         ----------
         grid
             The (y, x) coordinates in the reference frame of the elliptical profile.
         """
-        return np.multiply(
-            np.sqrt(self.axis_ratio), self.elliptical_radii_grid_from(grid)
-        ).view(np.ndarray)
 
-    @aa.grid_dec.grid_2d_to_structure
+        grid_radii = self.elliptical_radii_grid_from(grid=grid, **kwargs)
+
+        return np.multiply(np.sqrt(self.axis_ratio), grid_radii).view(np.ndarray)
+
+    @aa.grid_dec.to_grid
     def transformed_to_reference_frame_grid_from(
-        self, grid: aa.type.Grid2DLike
-    ) -> Grid2DTransformedNumpy:
+        self, grid: aa.type.Grid2DLike, **kwargs
+    ) -> np.ndarray:
         """
         Transform a grid of (y,x) coordinates to the reference frame of the profile.
 
         This includes a translation to the profile's `centre` and a rotation using its `angle`.
 
         Parameters
         ----------
         grid
             The (y, x) coordinates in the original reference frame of the grid.
         """
         if self.__class__.__name__.endswith("Sph"):
-            return super().transformed_to_reference_frame_grid_from(
-                grid=Grid2DTransformedNumpy(values=grid)
-            )
-        transformed = aa.util.geometry.transform_grid_2d_to_reference_frame(
+            return super().transformed_to_reference_frame_grid_from(grid=grid)
+        return aa.util.geometry.transform_grid_2d_to_reference_frame(
             grid_2d=grid, centre=self.centre, angle=self.angle
         )
-        return Grid2DTransformedNumpy(values=transformed)
 
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.grid_dec.to_grid
     def transformed_from_reference_frame_grid_from(
-        self, grid: aa.type.Grid2DLike
+        self, grid: aa.type.Grid2DLike, **kwargs
     ) -> aa.type.Grid2DLike:
         """
         Transform a grid of (y,x) coordinates from the reference frame of the profile to the original observer
         reference frame.
 
         This includes a translation from the profile's `centre` and a rotation using its `angle`.
 
         Parameters
         ----------
         grid
             The (y, x) coordinates in the reference frame of the profile.
         """
         if self.__class__.__name__.startswith("Sph"):
-            return super().transformed_from_reference_frame_grid_from(
-                grid=Grid2DTransformedNumpy(values=grid)
-            )
+            return super().transformed_from_reference_frame_grid_from(grid=grid)
 
         return aa.util.geometry.transform_grid_2d_from_reference_frame(
             grid_2d=grid, centre=self.centre, angle=self.angle
         )
 
     def _eta_u(self, u, coordinates):
         return np.sqrt(
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/light/abstract.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/light/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,20 @@
         ell_comps
             The first and second ellipticity components of the elliptical coordinate system (see the module
             `autogalaxy -> convert.py` for the convention).
         """
         super().__init__(centre=centre, ell_comps=ell_comps)
         self.intensity = intensity
 
+    @property
+    def coefficient_tag(self) -> str:
+        return ""
+
     def image_2d_from(
-        self, grid: aa.type.Grid2DLike, operated_only: Optional[bool] = None
+        self, grid: aa.type.Grid2DLike, operated_only: Optional[bool] = None, **kwargs
     ) -> aa.Array2D:
         """
         Returns the light profile's 2D image from a 2D grid of Cartesian (y,x) coordinates, which may have been
         transformed using the light profile's geometry.
 
         If the coordinates have not been transformed to the profile's geometry (e.g. translated to the
         profile `centre`), this is performed automatically.
@@ -68,38 +72,40 @@
         Parameters
         ----------
         grid_radii
             The radial distances from the centre of the profile, for each coordinate on the grid.
         """
         raise NotImplementedError()
 
-    @aa.grid_dec.grid_1d_to_structure
-    def image_1d_from(self, grid: aa.type.Grid1D2DLike) -> aa.type.Grid1D2DLike:
+    @aa.grid_dec.project_grid
+    def image_1d_from(
+        self, grid: aa.type.Grid1D2DLike, **kwargs
+    ) -> aa.type.Grid1D2DLike:
         """
         Returns the light profile's 1D image from a grid of Cartesian coordinates, which may have been
         transformed using the light profile's geometry.
 
         If a 1D grid is input the image is evaluated every coordinate on the grid. If a 2D grid is input, this is
         converted to a 1D grid by aligning with the major-axis of the light profile's elliptical geometry.
 
         Internally, this function uses a 2D grid to compute the image, which is mapped to a 1D data structure on return
-        via the `grid_1d_to_structure` decorator. This avoids code repetition by ensuring that light profiles only use
+        via the `project_grid` decorator. This avoids code repetition by ensuring that light profiles only use
         their `image_2d_from()`  function to evaluate their image.
 
         Parameters
         ----------
         grid
             A 1D or 2D grid of coordinates which are used to evaluate the light profile in 1D.
 
         Returns
         -------
         image
             The 1D image of the light profile evaluated at every (x,) coordinate on the 1D transformed grid.
         """
-        return self.image_2d_from(grid=grid)
+        return self.image_2d_from(grid=grid, **kwargs)
 
     def luminosity_within_circle_from(self, radius: float) -> float:
         """
         Integrate the light profile to compute the total luminosity within a circle of specified radius. This is
         centred on the light profile's `centre`.
 
         The `intensity` of a light profile is in dimension units, which are given physical meaning when the light
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/light/basis.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/light/basis.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             ell_comps=light_profile_list[0].ell_comps,
         )
 
         self.light_profile_list = light_profile_list
         self.regularization = regularization
 
     def image_2d_from(
-        self, grid: aa.type.Grid2DLike, operated_only: Optional[bool] = None
+        self, grid: aa.type.Grid2DLike, operated_only: Optional[bool] = None, **kwargs
     ) -> aa.Array2D:
         return sum(self.image_2d_list_from(grid=grid, operated_only=operated_only))
 
     def image_2d_list_from(
         self, grid: aa.type.Grid2DLike, operated_only: Optional[bool] = None
     ) -> List[aa.Array2D]:
         return [
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/light/decorators.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/light/decorators.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/light/linear/abstract.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/light/linear/abstract.py`

 * *Files 4% similar despite different names*

```diff
@@ -129,19 +129,25 @@
         self.light_profile_list = light_profile_list
 
     @property
     def params(self):
         return len(self.light_profile_list)
 
     @property
+    def pixels_in_mask(self):
+        if isinstance(self.grid, aa.Grid2DOverSampled):
+            return self.grid.pixels_in_mask
+        return self.grid.mask.pixels_in_mask
+
+    @property
     def mapping_matrix(self) -> np.ndarray:
-        mapping_matrix = np.zeros(shape=(self.grid.mask.pixels_in_mask, self.params))
+        mapping_matrix = np.zeros(shape=(self.pixels_in_mask, self.params))
 
         for pixel, light_profile in enumerate(self.light_profile_list):
-            image_2d = light_profile.image_2d_from(grid=self.grid).binned.slim
+            image_2d = light_profile.image_2d_from(grid=self.grid).slim
 
             mapping_matrix[:, pixel] = image_2d
 
         return mapping_matrix
 
     @cached_property
     def operated_mapping_matrix_override(self) -> Optional[np.ndarray]:
@@ -162,17 +168,15 @@
         A blurred mapping matrix of dimensions (total_mask_pixels, 1) which overrides the mapping matrix calculations
         performed in the linear equation solvers.
         """
 
         if isinstance(self.light_profile_list[0], LightProfileOperated):
             return self.mapping_matrix
 
-        operated_mapping_matrix = np.zeros(
-            shape=(self.grid.mask.pixels_in_mask, self.params)
-        )
+        operated_mapping_matrix = np.zeros(shape=(self.pixels_in_mask, self.params))
 
         for pixel, light_profile in enumerate(self.light_profile_list):
             image_2d = light_profile.image_2d_from(grid=self.grid)
 
             blurring_image_2d = light_profile.image_2d_from(grid=self.blurring_grid)
 
             blurred_image_2d = self.convolver.convolve_image(
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/light/linear/dev_vaucouleurs.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/light/linear/dev_vaucouleurs.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/light/linear/exponential.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/light/linear/exponential.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/light/linear/exponential_core.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/light/linear/exponential_core.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/light/linear/gaussian.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/light/linear/gaussian.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/light/linear/moffat.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/light/linear/moffat.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/light/linear/sersic.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/light/linear/sersic.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/light/linear/sersic_core.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/light/linear/sersic_core.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/light/mock/mock_light_profile.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/light/mock/mock_light_profile.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,17 +23,17 @@
         self.image_2d = image_2d
         self.image_2d_value = image_2d_value
         self.image_2d_first_value = image_2d_first_value
 
         self.value = value
         self.value1 = value1
 
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.grid_dec.to_array
     @check_operated_only
-    def image_2d_from(self, grid, operated_only: Optional[bool] = None):
+    def image_2d_from(self, grid, operated_only: Optional[bool] = None, **kwargs):
         if self.image_2d is not None:
             return self.image_2d
 
         image_2d = np.ones(shape=(grid.shape[0]))
 
         if self.image_2d_first_value is not None:
             image_2d[0] = self.image_2d_first_value
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/light/shapelets/abstract.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/light/standard/shapelets/abstract.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from typing import Tuple
 
-from autogalaxy.profiles.light.linear.abstract import LightProfileLinear
+from autogalaxy.profiles.light.abstract import LightProfile
 
 
-class AbstractShapelet(LightProfileLinear):
+class AbstractShapelet(LightProfile):
     def __init__(
         self,
         centre: Tuple[float, float] = (0.0, 0.0),
         ell_comps: Tuple[float, float] = (0.0, 0.0),
+        intensity: float = 1.0,
         beta: float = 1.0,
     ):
         """
         Abstract Base class of a Shapelet.
 
         Shapelets are always defined and used as a linear light profile.
 
         Shapelets are defined according to:
 
           https://arxiv.org/abs/astro-ph/0105178
 
-        Shapelets are are described in the context of strong lens modeling in:
+        Shapelets are described in the context of strong lens modeling in:
 
           https://ui.adsabs.harvard.edu/abs/2016MNRAS.457.3066T/abstract
 
         Parameters
         ----------
         centre
             The (y,x) arc-second coordinates of the profile (shapelet) centre.
@@ -31,8 +32,8 @@
             The first and second ellipticity components of the elliptical coordinate system.
         beta
             The characteristic length scale of the shapelet basis function, defined in arc-seconds.
         """
 
         self.beta = beta
 
-        super().__init__(centre=centre, ell_comps=ell_comps, intensity=1.0)
+        super().__init__(centre=centre, ell_comps=ell_comps, intensity=intensity)
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/light/shapelets/cartesian.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/light/linear/shapelets/cartesian.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import numpy as np
 from scipy.special import hermite, factorial
 from typing import Optional, Tuple
 
 import autoarray as aa
 
+from autogalaxy.profiles.light import standard as lp
+
 from autogalaxy.profiles.light.decorators import (
     check_operated_only,
 )
-from autogalaxy.profiles.light.shapelets.abstract import AbstractShapelet
+from autogalaxy.profiles.light.linear.abstract import LightProfileLinear
 
 
-class ShapeletCartesianEll(AbstractShapelet):
+class ShapeletCartesian(lp.ShapeletCartesian, LightProfileLinear):
     def __init__(
         self,
         n_y: int,
         n_x: int,
         centre: Tuple[float, float] = (0.0, 0.0),
         ell_comps: Tuple[float, float] = (0.0, 0.0),
         beta: float = 1.0,
@@ -22,15 +24,15 @@
         """
         Shapelets where the basis function is defined according to a Cartesian (y,x) grid of coordinates.
 
         Shapelets are defined according to:
 
           https://arxiv.org/abs/astro-ph/0105178
 
-        Shapelets are are described in the context of strong lens modeling in:
+        Shapelets are described in the context of strong lens modeling in:
 
           https://ui.adsabs.harvard.edu/abs/2016MNRAS.457.3066T/abstract
 
         Parameters
         ----------
         n_y
             The order of the shapelets basis function in the y-direction.
@@ -40,25 +42,25 @@
             The (y,x) arc-second coordinates of the profile (shapelet) centre.
         ell_comps
             The first and second ellipticity components of the elliptical coordinate system.
         beta
             The characteristic length scale of the shapelet basis function, defined in arc-seconds.
         """
 
-        self.n_y = n_y
-        self.n_x = n_x
-
-        super().__init__(centre=centre, ell_comps=ell_comps, beta=beta)
+        super().__init__(
+            n_y=n_y, n_x=n_x, centre=centre, ell_comps=ell_comps, beta=beta
+        )
 
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.over_sample
+    @aa.grid_dec.to_array
     @check_operated_only
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
     def image_2d_from(
-        self, grid: aa.type.Grid2DLike, operated_only: Optional[bool] = None
+        self, grid: aa.type.Grid2DLike, operated_only: Optional[bool] = None, **kwargs
     ) -> np.ndarray:
         """
         Returns the Cartesian Shapelet light profile's 2D image from a 2D grid of Cartesian (y,x) coordinates.
 
         If the coordinates have not been transformed to the profile's geometry (e.g. translated to the
         profile `centre`), this is performed automatically.
 
@@ -93,31 +95,35 @@
                     * (np.pi)
                     * factorial(self.n_y)
                     * factorial(self.n_x)
                 )
             )
         )
 
+    @property
+    def lp_cls(self):
+        return lp.ShapeletCartesian
+
 
-class ShapeletCartesian(ShapeletCartesianEll):
+class ShapeletCartesianSph(ShapeletCartesian):
     def __init__(
         self,
         n_y: int,
         n_x: int,
         centre: Tuple[float, float] = (0.0, 0.0),
         beta: float = 1.0,
     ):
         """
         Shapelets where the basis function is defined according to a Cartesian (y,x) grid of coordinates.
 
         Shapelets are defined according to:
 
           https://arxiv.org/abs/astro-ph/0105178
 
-        Shapelets are are described in the context of strong lens modeling in:
+        Shapelets are described in the context of strong lens modeling in:
 
           https://ui.adsabs.harvard.edu/abs/2016MNRAS.457.3066T/abstract
 
         Parameters
         ----------
         n_y
             The order of the shapelets basis function in the y-direction.
@@ -128,7 +134,11 @@
         beta
             The characteristic length scale of the shapelet basis function, defined in arc-seconds.
         """
 
         super().__init__(
             n_y=n_y, n_x=n_x, centre=centre, ell_comps=(0.0, 0.0), beta=beta
         )
+
+    @property
+    def lp_cls(self):
+        return lp.ShapeletCartesian
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/light/shapelets/exponential.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/light/linear/shapelets/exponential.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import numpy as np
 from scipy.special import factorial, genlaguerre
 from typing import Optional, Tuple
 
 import autoarray as aa
 
+from autogalaxy.profiles.light import standard as lp
+
 from autogalaxy.profiles.light.decorators import (
     check_operated_only,
 )
-from autogalaxy.profiles.light.shapelets.abstract import AbstractShapelet
+from autogalaxy.profiles.light.linear.abstract import LightProfileLinear
 
 
-class ShapeletExponentialEll(AbstractShapelet):
+class ShapeletExponential(lp.ShapeletExponential, LightProfileLinear):
     def __init__(
         self,
         n: int,
         m: int,
         centre: Tuple[float, float] = (0.0, 0.0),
         ell_comps: Tuple[float, float] = (0.0, 0.0),
         beta: float = 1.0,
@@ -23,15 +25,15 @@
         Shapelets where the basis function is defined according to an Exponential using a polar (r,theta) grid of
         coordinates.
 
         Shapelets are defined according to:
 
           https://arxiv.org/abs/astro-ph/0105178
 
-        Shapelets are are described in the context of strong lens modeling in:
+        Shapelets are described in the context of strong lens modeling in:
 
           https://ui.adsabs.harvard.edu/abs/2016MNRAS.457.3066T/abstract
 
         Parameters
         ----------
         n
             The n order of the shapelets basis function.
@@ -41,25 +43,23 @@
             The (y,x) arc-second coordinates of the profile (shapelet) centre.
         ell_comps
             The first and second ellipticity components of the elliptical coordinate system.
         beta
             The characteristic length scale of the shapelet basis function, defined in arc-seconds.
         """
 
-        self.n = n
-        self.m = m
-
-        super().__init__(centre=centre, ell_comps=ell_comps, beta=beta)
+        super().__init__(n=n, m=m, centre=centre, ell_comps=ell_comps, beta=beta)
 
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.over_sample
+    @aa.grid_dec.to_array
     @check_operated_only
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
     def image_2d_from(
-        self, grid: aa.type.Grid2DLike, operated_only: Optional[bool] = None
+        self, grid: aa.type.Grid2DLike, operated_only: Optional[bool] = None, **kwargs
     ) -> np.ndarray:
         """
         Returns the Exponential Shapelet light profile's 2D image from a 2D grid of Exponential (y,x) coordinates.
 
         If the coordinates have not been transformed to the profile's geometry (e.g. translated to the
         profile `centre`), this is performed automatically.
 
@@ -97,31 +97,35 @@
             * np.exp(-radial / (2 * self.n + 1))
             * radial ** (np.abs(self.m))
             * shapelet
             * np.cos(self.m * theta)
             + -1.0j * np.sin(self.m * theta)
         )
 
+    @property
+    def lp_cls(self):
+        return lp.ShapeletExponential
 
-class ShapeletExponential(ShapeletExponentialEll):
+
+class ShapeletExponentialSph(ShapeletExponential):
     def __init__(
         self,
         n: int,
         m: int,
         centre: Tuple[float, float] = (0.0, 0.0),
         beta: float = 1.0,
     ):
         """
         Shapelets where the basis function is defined according to a Exponential (r,theta) grid of coordinates.
 
         Shapelets are defined according to:
 
           https://arxiv.org/abs/astro-ph/0105178
 
-        Shapelets are are described in the context of strong lens modeling in:
+        Shapelets are described in the context of strong lens modeling in:
 
           https://ui.adsabs.harvard.edu/abs/2016MNRAS.457.3066T/abstract
 
         Parameters
         ----------
         n_y
             The order of the shapelets basis function in the y-direction.
@@ -130,7 +134,11 @@
         centre
             The (y,x) arc-second coordinates of the profile (shapelet) centre.
         beta
             The characteristic length scale of the shapelet basis function, defined in arc-seconds.
         """
 
         super().__init__(n=n, m=m, centre=centre, ell_comps=(0.0, 0.0), beta=beta)
+
+    @property
+    def lp_cls(self):
+        return lp.ShapeletExponentialSph
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/light/shapelets/polar.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/light/standard/shapelets/polar.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,64 +1,76 @@
 import numpy as np
 from scipy.special import factorial, genlaguerre
 from typing import Optional, Tuple
 
 import autoarray as aa
 
+
 from autogalaxy.profiles.light.decorators import (
     check_operated_only,
 )
-from autogalaxy.profiles.light.shapelets.abstract import AbstractShapelet
+from autogalaxy.profiles.light.standard.shapelets.abstract import AbstractShapelet
 
 
-class ShapeletPolarEll(AbstractShapelet):
+class ShapeletPolar(AbstractShapelet):
     def __init__(
         self,
         n: int,
         m: int,
         centre: Tuple[float, float] = (0.0, 0.0),
         ell_comps: Tuple[float, float] = (0.0, 0.0),
+        intensity: float = 1.0,
         beta: float = 1.0,
     ):
         """
         Shapelets where the basis function is defined according to a Polar (r,theta) grid of coordinates.
 
         Shapelets are defined according to:
 
           https://arxiv.org/abs/astro-ph/0105178
 
-        Shapelets are are described in the context of strong lens modeling in:
+        Shapelets are described in the context of strong lens modeling in:
 
           https://ui.adsabs.harvard.edu/abs/2016MNRAS.457.3066T/abstract
 
         Parameters
         ----------
         n
             The n order of the shapelets basis function.
         m
             The m order of the shapelets basis function in the x-direction.
         centre
             The (y,x) arc-second coordinates of the profile (shapelet) centre.
         ell_comps
             The first and second ellipticity components of the elliptical coordinate system.
+        intensity
+            Overall intensity normalisation of the light profile (units are dimensionless and derived from the data
+            the light profile's image is compared too, which is expected to be electrons per second).
         beta
             The characteristic length scale of the shapelet basis function, defined in arc-seconds.
         """
 
         self.n = n
         self.m = m
 
-        super().__init__(centre=centre, ell_comps=ell_comps, beta=beta)
+        super().__init__(
+            centre=centre, ell_comps=ell_comps, beta=beta, intensity=intensity
+        )
+
+    @property
+    def coefficient_tag(self) -> str:
+        return f"n_{self.n}_m_{self.m}"
 
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.over_sample
+    @aa.grid_dec.to_array
     @check_operated_only
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
     def image_2d_from(
-        self, grid: aa.type.Grid2DLike, operated_only: Optional[bool] = None
+        self, grid: aa.type.Grid2DLike, operated_only: Optional[bool] = None, **kwargs
     ) -> np.ndarray:
         """
         Returns the Polar Shapelet light profile's 2D image from a 2D grid of Polar (y,x) coordinates.
 
         If the coordinates have not been transformed to the profile's geometry (e.g. translated to the
         profile `centre`), this is performed automatically.
 
@@ -69,66 +81,76 @@
 
         Returns
         -------
         image
             The image of the Polar Shapelet evaluated at every (y,x) coordinate on the transformed grid.
         """
 
-        radial = (grid[:, 0] ** 2 + grid[:, 1] ** 2) / self.beta**2.0
-        theta = np.arctan(grid[:, 1] / grid[:, 0])
-
         laguerre = genlaguerre(n=(self.n - np.abs(self.m)) / 2.0, alpha=np.abs(self.m))
 
-        shapelet = laguerre(radial)
-
         const = (
-            ((-1) ** ((self.n - np.abs(self.m)) / 2))
+            ((-1) ** ((self.n - np.abs(self.m)) // 2))
             * np.sqrt(
-                factorial((self.n - np.abs(self.m)) / 2)
-                / factorial((self.n + np.abs(self.m)) / 2)
+                factorial((self.n - np.abs(self.m)) // 2)
+                / factorial((self.n + np.abs(self.m)) // 2)
             )
             / self.beta
             / np.sqrt(np.pi)
         )
-        gauss = np.exp(-radial / 2.0)
 
-        return np.abs(
-            const
-            * radial ** (np.abs(self.m / 2.0))
-            * shapelet
-            * gauss
-            * np.exp(0.0 + 1j * -self.m * theta)
-        )
+        rsq = (grid[:, 0] ** 2 + grid[:, 1] ** 2) / self.beta**2
+        theta = np.arctan2(grid[:, 1], grid[:, 0])
+        radial = rsq ** (abs(self.m / 2.0)) * np.exp(-rsq / 2.0) * laguerre(rsq)
+
+        if self.m == 0:
+            azimuthal = 1
+        elif self.m > 0:
+            azimuthal = np.sin((-1) * self.m * theta)
+        else:
+            azimuthal = np.cos((-1) * self.m * theta)
 
+        return const * radial * azimuthal
 
-class ShapeletPolar(ShapeletPolarEll):
+
+class ShapeletPolarSph(ShapeletPolar):
     def __init__(
         self,
         n: int,
         m: int,
         centre: Tuple[float, float] = (0.0, 0.0),
+        intensity: float = 1.0,
         beta: float = 1.0,
     ):
         """
         Shapelets where the basis function is defined according to a Polar (r,theta) grid of coordinates.
 
         Shapelets are defined according to:
 
           https://arxiv.org/abs/astro-ph/0105178
 
-        Shapelets are are described in the context of strong lens modeling in:
+        Shapelets are described in the context of strong lens modeling in:
 
           https://ui.adsabs.harvard.edu/abs/2016MNRAS.457.3066T/abstract
 
         Parameters
         ----------
         n_y
             The order of the shapelets basis function in the y-direction.
         n_x
             The order of the shapelets basis function in the x-direction.
         centre
             The (y,x) arc-second coordinates of the profile (shapelet) centre.
+        intensity
+            Overall intensity normalisation of the light profile (units are dimensionless and derived from the data
+            the light profile's image is compared too, which is expected to be electrons per second).
         beta
             The characteristic length scale of the shapelet basis function, defined in arc-seconds.
         """
 
-        super().__init__(n=n, m=m, centre=centre, ell_comps=(0.0, 0.0), beta=beta)
+        super().__init__(
+            n=n,
+            m=m,
+            centre=centre,
+            ell_comps=(0.0, 0.0),
+            intensity=intensity,
+            beta=beta,
+        )
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/light/snr/abstract.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/light/snr/abstract.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         ----------
         signal_to_noise_ratio
             The signal-to-noises ratio that the simulated light profile will produce.
         """
         self.signal_to_noise_ratio = signal_to_noise_ratio
 
     def image_2d_from(
-        self, grid: aa.type.Grid2DLike, operated_only: Optional[bool] = None
+        self, grid: aa.type.Grid2DLike, operated_only: Optional[bool] = None, **kwargs
     ) -> aa.Array2D:
         """
         Abstract method for obtaining intensity at a grid of Cartesian (y,x) coordinates.
 
         Parameters
         ----------
         grid
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/light/snr/chameleon.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/light/snr/gaussian.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,83 +1,56 @@
 from typing import Tuple
 
 from autogalaxy.profiles.light.snr.abstract import LightProfileSNR
-
 from autogalaxy.profiles.light import standard as lp
 
 
-class Chameleon(lp.Chameleon, LightProfileSNR):
+class Gaussian(lp.Gaussian, LightProfileSNR):
     def __init__(
         self,
         signal_to_noise_ratio: float = 10.0,
         centre: Tuple[float, float] = (0.0, 0.0),
         ell_comps: Tuple[float, float] = (0.0, 0.0),
-        core_radius_0: float = 0.01,
-        core_radius_1: float = 0.05,
+        sigma: float = 1.0,
     ):
         """
-        The elliptical Chameleon light profile.
-
-        Profile form:
-            mass_to_light_ratio * intensity *\
-                (1.0 / Sqrt(x^2 + (y/q)^2 + rc^2) - 1.0 / Sqrt(x^2 + (y/q)^2 + (rc + dr)**2.0))
+        The elliptical Gaussian light profile.
 
         Parameters
         ----------
         centre
             The (y,x) arc-second coordinates of the profile centre.
         ell_comps
             The first and second ellipticity components of the elliptical coordinate system.
         intensity
             Overall intensity normalisation of the light profile (units are dimensionless and derived from the data
             the light profile's image is compared too, which is expected to be electrons per second).
-        core_radius_0 : the core size of the first elliptical cored Isothermal profile.
-        core_radius_1 : rc + dr is the core size of the second elliptical cored Isothermal profile.
-             We use dr here is to avoid negative values.
+        sigma
+            The sigma value of the Gaussian, corresponding to ~ 1 / sqrt(2 log(2)) the full width half maximum.
         """
 
-        super().__init__(
-            centre=centre,
-            ell_comps=ell_comps,
-            intensity=0.0,
-            core_radius_0=core_radius_0,
-            core_radius_1=core_radius_1,
-        )
+        super().__init__(centre=centre, ell_comps=ell_comps, intensity=0.0, sigma=sigma)
         LightProfileSNR.__init__(self, signal_to_noise_ratio=signal_to_noise_ratio)
 
 
-class ChameleonSph(lp.ChameleonSph, LightProfileSNR):
+class GaussianSph(lp.GaussianSph, LightProfileSNR):
     def __init__(
         self,
         signal_to_noise_ratio: float = 10.0,
         centre: Tuple[float, float] = (0.0, 0.0),
-        core_radius_0: float = 0.01,
-        core_radius_1: float = 0.05,
+        sigma: float = 1.0,
     ):
         """
-        The spherical Chameleon light profile.
-
-        Profile form:
-            mass_to_light_ratio * intensity *\
-                (1.0 / Sqrt(x^2 + (y/q)^2 + rc^2) - 1.0 / Sqrt(x^2 + (y/q)^2 + (rc + dr)**2.0))
+        The spherical Gaussian light profile.
 
         Parameters
         ----------
         centre
             The (y,x) arc-second coordinates of the profile centre.
-        ell_comps
-            The first and second ellipticity components of the elliptical coordinate system.
         intensity
             Overall intensity normalisation of the light profile (units are dimensionless and derived from the data
             the light profile's image is compared too, which is expected to be electrons per second).
-        core_radius_0 : the core size of the first elliptical cored Isothermal profile.
-        core_radius_1 : rc + dr is the core size of the second elliptical cored Isothermal profile.
-             We use dr here is to avoid negative values.
+        sigma
+            The sigma value of the Gaussian, corresponding to ~ 1 / sqrt(2 log(2)) the full width half maximum.
         """
-
-        super().__init__(
-            centre=centre,
-            intensity=0.0,
-            core_radius_0=core_radius_0,
-            core_radius_1=core_radius_1,
-        )
+        super().__init__(centre=centre, intensity=0.0, sigma=sigma)
         LightProfileSNR.__init__(self, signal_to_noise_ratio=signal_to_noise_ratio)
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/light/snr/dev_vaucouleurs.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/light/snr/dev_vaucouleurs.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/light/snr/eff.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/light/snr/eff.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/light/snr/exponential.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/light/snr/exponential.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/light/snr/gaussian.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/light/snr/sersic_core.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,60 @@
 from typing import Tuple
 
 from autogalaxy.profiles.light.snr.abstract import LightProfileSNR
 from autogalaxy.profiles.light import standard as lp
 
 
-class Gaussian(lp.Gaussian, LightProfileSNR):
+class SersicCore(lp.SersicCore, LightProfileSNR):
     def __init__(
         self,
         signal_to_noise_ratio: float = 10.0,
         centre: Tuple[float, float] = (0.0, 0.0),
         ell_comps: Tuple[float, float] = (0.0, 0.0),
-        sigma: float = 1.0,
+        effective_radius: float = 0.6,
+        sersic_index: float = 4.0,
+        radius_break: float = 0.01,
+        intensity: float = 0.05,
+        gamma: float = 0.25,
+        alpha: float = 3.0,
     ):
         """
-        The elliptical Gaussian light profile.
+        The elliptical cored-Sersic light profile.
+
+        Instead of an `intensity` a `signal_to_noise_ratio` is input which sets the signal to noise of the brightest
+        pixel of the profile's image when used to simulate imaging data.
 
         Parameters
         ----------
+        signal_to_noise_ratio
+            The signal to noise of the light profile when it is used to simulate strong lens imaging.
         centre
             The (y,x) arc-second coordinates of the profile centre.
         ell_comps
             The first and second ellipticity components of the elliptical coordinate system.
+        effective_radius
+            The circular radius containing half the light of this profile.
+        sersic_index
+            Controls the concentration of the profile (lower -> less concentrated, higher -> more concentrated).
+        radius_break
+            The break radius separating the inner power-law (with logarithmic slope gamma) and outer Sersic function.
         intensity
-            Overall intensity normalisation of the light profile (units are dimensionless and derived from the data
-            the light profile's image is compared too, which is expected to be electrons per second).
-        sigma
-            The sigma value of the Gaussian, corresponding to ~ 1 / sqrt(2 log(2)) the full width half maximum.
+            The intensity at the break radius.
+        gamma
+            The logarithmic power-law slope of the inner core profiles
+        alpha
+            Controls the sharpness of the transition between the inner core / outer Sersic profiles.
         """
+        super().__init__(
+            centre=centre,
+            ell_comps=ell_comps,
+            effective_radius=effective_radius,
+            sersic_index=sersic_index,
+            radius_break=radius_break,
+            intensity=0.0,
+            alpha=alpha,
+            gamma=gamma,
+        )
 
-        super().__init__(centre=centre, ell_comps=ell_comps, intensity=0.0, sigma=sigma)
-        LightProfileSNR.__init__(self, signal_to_noise_ratio=signal_to_noise_ratio)
-
-
-class GaussianSph(lp.GaussianSph, LightProfileSNR):
-    def __init__(
-        self,
-        signal_to_noise_ratio: float = 10.0,
-        centre: Tuple[float, float] = (0.0, 0.0),
-        sigma: float = 1.0,
-    ):
-        """
-        The spherical Gaussian light profile.
+        self.intensity = self.intensity
 
-        Parameters
-        ----------
-        centre
-            The (y,x) arc-second coordinates of the profile centre.
-        intensity
-            Overall intensity normalisation of the light profile (units are dimensionless and derived from the data
-            the light profile's image is compared too, which is expected to be electrons per second).
-        sigma
-            The sigma value of the Gaussian, corresponding to ~ 1 / sqrt(2 log(2)) the full width half maximum.
-        """
-        super().__init__(centre=centre, intensity=0.0, sigma=sigma)
         LightProfileSNR.__init__(self, signal_to_noise_ratio=signal_to_noise_ratio)
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/light/snr/sersic.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/light/snr/sersic.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/light/snr/sersic_core.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/light/standard/exponential_core.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,94 @@
 from typing import Tuple
 
-from autogalaxy.profiles.light.snr.abstract import LightProfileSNR
-from autogalaxy.profiles.light import standard as lp
+from autogalaxy.profiles.light.standard.sersic_core import SersicCore
 
 
-class SersicCore(lp.SersicCore, LightProfileSNR):
+class ExponentialCore(SersicCore):
     def __init__(
         self,
-        signal_to_noise_ratio: float = 10.0,
         centre: Tuple[float, float] = (0.0, 0.0),
         ell_comps: Tuple[float, float] = (0.0, 0.0),
         effective_radius: float = 0.6,
-        sersic_index: float = 4.0,
         radius_break: float = 0.01,
         intensity: float = 0.05,
         gamma: float = 0.25,
         alpha: float = 3.0,
     ):
         """
-        The elliptical cored-Sersic light profile.
-
-        Instead of an `intensity` a `signal_to_noise_ratio` is input which sets the signal to noise of the brightest
-        pixel of the profile's image when used to simulate imaging data.
+        The elliptical cored-Exponential light profile.
 
         Parameters
         ----------
-        signal_to_noise_ratio
-            The signal to noise of the light profile when it is used to simulate strong lens imaging.
         centre
             The (y,x) arc-second coordinates of the profile centre.
         ell_comps
             The first and second ellipticity components of the elliptical coordinate system.
         effective_radius
             The circular radius containing half the light of this profile.
         sersic_index
             Controls the concentration of the profile (lower -> less concentrated, higher -> more concentrated).
         radius_break
             The break radius separating the inner power-law (with logarithmic slope gamma) and outer Sersic function.
         intensity
             The intensity at the break radius.
         gamma
             The logarithmic power-law slope of the inner core profiles
-        alpha
+        alpha :
             Controls the sharpness of the transition between the inner core / outer Sersic profiles.
         """
+
         super().__init__(
             centre=centre,
             ell_comps=ell_comps,
+            intensity=intensity,
             effective_radius=effective_radius,
-            sersic_index=sersic_index,
+            sersic_index=1.0,
             radius_break=radius_break,
-            intensity=0.0,
-            alpha=alpha,
             gamma=gamma,
+            alpha=alpha,
         )
 
-        self.intensity = self.intensity
 
-        LightProfileSNR.__init__(self, signal_to_noise_ratio=signal_to_noise_ratio)
+class ExponentialCoreSph(ExponentialCore):
+    def __init__(
+        self,
+        centre: Tuple[float, float] = (0.0, 0.0),
+        effective_radius: float = 0.6,
+        radius_break: float = 0.01,
+        intensity: float = 0.05,
+        gamma: float = 0.25,
+        alpha: float = 3.0,
+    ):
+        """
+        The elliptical cored-Exponential light profile.
+
+        Parameters
+        ----------
+        centre
+            The (y,x) arc-second coordinates of the profile centre.
+        effective_radius
+            The circular radius containing half the light of this profile.
+        radius_break
+            The break radius separating the inner power-law (with logarithmic slope gamma) and outer Sersic function.
+        intensity
+            The intensity at the break radius.
+        gamma
+            The logarithmic power-law slope of the inner core profiles
+        alpha :
+            Controls the sharpness of the transition between the inner core / outer Sersic profiles.
+        """
+
+        super().__init__(
+            centre=centre,
+            ell_comps=(0.0, 0.0),
+            effective_radius=effective_radius,
+            radius_break=radius_break,
+            intensity=intensity,
+            gamma=gamma,
+            alpha=alpha,
+        )
+
+        self.radius_break = radius_break
+        self.intensity = intensity
+        self.alpha = alpha
+        self.gamma = gamma
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/light/standard/chameleon.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/light/standard/chameleon.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,20 +86,21 @@
                             (4.0 * self.core_radius_1**2.0) / axis_ratio_factor,
                         )
                     ),
                 ),
             ),
         )
 
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.over_sample
+    @aa.grid_dec.to_array
     @check_operated_only
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
     def image_2d_from(
-        self, grid: aa.type.Grid2DLike, operated_only: Optional[bool] = None
+        self, grid: aa.type.Grid2DLike, operated_only: Optional[bool] = None, **kwargs
     ) -> np.ndarray:
         """
         Returns the Chameleon light profile's 2D image from a 2D grid of Cartesian (y,x) coordinates.
 
         If the coordinates have not been transformed to the profile's geometry (e.g. translated to the
         profile `centre`), this is performed automatically.
 
@@ -109,15 +110,17 @@
             The 2D (y, x) coordinates in the original reference frame of the grid.
 
         Returns
         -------
         image
             The image of the Chameleon evaluated at every (y,x) coordinate on the transformed grid.
         """
-        return self.image_2d_via_radii_from(self.elliptical_radii_grid_from(grid))
+        return self.image_2d_via_radii_from(
+            self.elliptical_radii_grid_from(grid=grid, **kwargs)
+        )
 
 
 class ChameleonSph(Chameleon):
     def __init__(
         self,
         centre: Tuple[float, float] = (0.0, 0.0),
         intensity: float = 0.1,
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/light/standard/dev_vaucouleurs.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/light/standard/dev_vaucouleurs.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/light/standard/eff.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/light/standard/eff.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,20 +53,21 @@
             The radial distances from the centre of the profile, for each coordinate on the grid.
         """
         np.seterr(all="ignore")
         return self._intensity * (1 + (grid_radii / self.effective_radius) ** 2) ** (
             -self.eta
         )
 
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.over_sample
+    @aa.grid_dec.to_array
     @check_operated_only
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
     def image_2d_from(
-        self, grid: aa.type.Grid2DLike, operated_only: Optional[bool] = None
+        self, grid: aa.type.Grid2DLike, operated_only: Optional[bool] = None, **kwargs
     ) -> np.ndarray:
         """
         Returns the Eff light profile's 2D image from a 2D grid of Cartesian (y,x) coordinates.
 
         If the coordinates have not been transformed to the profile's geometry (e.g. translated to the
         profile `centre`), this is performed automatically.
 
@@ -76,15 +77,17 @@
             The 2D (y, x) coordinates in the original reference frame of the grid.
 
         Returns
         -------
         image
             The image of the Eff evaluated at every (y,x) coordinate on the transformed grid.
         """
-        return self.image_2d_via_radii_from(self.eccentric_radii_grid_from(grid))
+        return self.image_2d_via_radii_from(
+            self.eccentric_radii_grid_from(grid=grid, **kwargs)
+        )
 
     @property
     def half_light_radius(self) -> float:
         return self.effective_radius * np.sqrt(0.5 ** (1.0 / (1.0 - self.eta)) - 1.0)
 
 
 class ElsonFreeFallSph(ElsonFreeFall):
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/light/standard/exponential.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/light/standard/exponential.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/light/standard/gaussian.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/light/standard/gaussian.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,14 +37,20 @@
             the light profile's image is compared too, which is expected to be electrons per second).
         sigma
             The sigma value of the Gaussian, corresponding to ~ 1 / sqrt(2 log(2)) the full width half maximum.
         """
         super().__init__(centre=centre, ell_comps=ell_comps, intensity=intensity)
         self.sigma = sigma
 
+    @property
+    def coefficient_tag(self) -> str:
+        return (
+            f"sigma_{np.round(self.sigma, 2)}__ell_comps_{np.round(self.ell_comps, 2)}"
+        )
+
     def image_2d_via_radii_from(self, grid_radii: np.ndarray) -> np.ndarray:
         """
         Returns the 2D image of the Gaussian light profile from a grid of coordinates which are the radial distance of
         each coordinate from the its `centre`.
 
         Note: sigma is divided by sqrt(q) here.
 
@@ -59,20 +65,21 @@
                 -0.5
                 * np.square(
                     np.divide(grid_radii, self.sigma / np.sqrt(self.axis_ratio))
                 )
             ),
         )
 
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.over_sample
+    @aa.grid_dec.to_array
     @check_operated_only
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
     def image_2d_from(
-        self, grid: aa.type.Grid2DLike, operated_only: Optional[bool] = None
+        self, grid: aa.type.Grid2DLike, operated_only: Optional[bool] = None, **kwargs
     ) -> np.ndarray:
         """
         Returns the Gaussian light profile's 2D image from a 2D grid of Cartesian (y,x) coordinates.
 
         If the coordinates have not been transformed to the profile's geometry (e.g. translated to the
         profile `centre`), this is performed automatically.
 
@@ -83,15 +90,17 @@
 
         Returns
         -------
         image
             The image of the Gaussian evaluated at every (y,x) coordinate on the transformed grid.
         """
 
-        return self.image_2d_via_radii_from(self.eccentric_radii_grid_from(grid))
+        return self.image_2d_via_radii_from(
+            self.eccentric_radii_grid_from(grid=grid, **kwargs)
+        )
 
 
 class GaussianSph(Gaussian):
     def __init__(
         self,
         centre: Tuple[float, float] = (0.0, 0.0),
         intensity: float = 0.1,
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/light/standard/moffat.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/light/standard/moffat.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,20 +64,21 @@
                 + np.square(
                     np.divide(grid_radii, self.alpha / np.sqrt(self.axis_ratio))
                 ),
                 -self.beta,
             ),
         )
 
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.over_sample
+    @aa.grid_dec.to_array
     @check_operated_only
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
     def image_2d_from(
-        self, grid: aa.type.Grid2DLike, operated_only: Optional[bool] = None
+        self, grid: aa.type.Grid2DLike, operated_only: Optional[bool] = None, **kwargs
     ) -> np.ndarray:
         """
         Returns the Moffat light profile's 2D image from a 2D grid of Cartesian (y,x) coordinates.
 
         If the coordinates have not been transformed to the profile's geometry (e.g. translated to the
         profile `centre`), this is performed automatically.
 
@@ -88,15 +89,17 @@
 
         Returns
         -------
         image
             The image of the Moffat evaluated at every (y,x) coordinate on the transformed grid.
         """
 
-        return self.image_2d_via_radii_from(self.eccentric_radii_grid_from(grid))
+        return self.image_2d_via_radii_from(
+            self.eccentric_radii_grid_from(grid=grid, **kwargs)
+        )
 
 
 class MoffatSph(Moffat):
     def __init__(
         self,
         centre: Tuple[float, float] = (0.0, 0.0),
         intensity: float = 0.1,
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/light/standard/sersic.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/light/standard/sersic.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,15 @@
             centre=centre,
             ell_comps=ell_comps,
             intensity=intensity,
             effective_radius=effective_radius,
             sersic_index=sersic_index,
         )
 
-    def image_2d_via_radii_from(self, grid_radii: np.ndarray) -> np.ndarray:
+    def image_2d_via_radii_from(self, grid_radii: np.ndarray, **kwargs) -> np.ndarray:
         """
         Returns the 2D image of the Sersic light profile from a grid of coordinates which are the radial distances of
         each coordinate from the its `centre`.
 
         Parameters
         ----------
         grid_radii
@@ -140,20 +140,21 @@
                         ),
                         -1,
                     ),
                 )
             ),
         )
 
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.over_sample
+    @aa.grid_dec.to_array
     @check_operated_only
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
     def image_2d_from(
-        self, grid: aa.type.Grid2DLike, operated_only: Optional[bool] = None
+        self, grid: aa.type.Grid2DLike, operated_only: Optional[bool] = None, **kwargs
     ) -> aa.Array2D:
         """
         Returns the Sersic light profile's 2D image from a 2D grid of Cartesian (y,x) coordinates.
 
         If the coordinates have not been transformed to the profile's geometry (e.g. translated to the
         profile `centre`), this is performed automatically.
 
@@ -163,15 +164,18 @@
             The 2D (y, x) coordinates in the original reference frame of the grid.
 
         Returns
         -------
         image
             The image of the Sersic evaluated at every (y,x) coordinate on the transformed grid.
         """
-        return self.image_2d_via_radii_from(self.eccentric_radii_grid_from(grid))
+
+        grid_radii = self.eccentric_radii_grid_from(grid=grid, **kwargs)
+
+        return self.image_2d_via_radii_from(grid_radii=grid_radii, **kwargs)
 
 
 class SersicSph(Sersic):
     def __init__(
         self,
         centre: Tuple[float, float] = (0.0, 0.0),
         intensity: float = 0.1,
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/light/standard/sersic_core.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/light/standard/sersic_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
                     ((2.0 ** (1.0 / self.alpha)) * self.radius_break)
                     / self.effective_radius
                 )
                 ** (1.0 / self.sersic_index)
             )
         )
 
-    def image_2d_via_radii_from(self, grid_radii: np.ndarray) -> np.ndarray:
+    def image_2d_via_radii_from(self, grid_radii: np.ndarray, **kwargs) -> np.ndarray:
         """
         Returns the 2D image of the Sersic light profile from a grid of coordinates which are the radial distances of
         each coordinate from the its `centre`.
 
         Parameters
         ----------
         grid_radii
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/light_and_mass_profiles.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/light_and_mass_profiles.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/__init__.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/__init__.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/abstract/abstract.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/abstract/abstract.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,22 +45,22 @@
 
     def convergence_2d_from(self, grid):
         raise NotImplementedError
 
     def convergence_func(self, grid_radius: float) -> float:
         raise NotImplementedError
 
-    @aa.grid_dec.grid_1d_to_structure
+    @aa.grid_dec.project_grid
     def convergence_1d_from(self, grid: aa.type.Grid1D2DLike) -> aa.type.Grid1D2DLike:
         return self.convergence_2d_from(grid=grid)
 
     def potential_2d_from(self, grid):
         raise NotImplementedError
 
-    @aa.grid_dec.grid_1d_to_structure
+    @aa.grid_dec.project_grid
     def potential_1d_from(self, grid: aa.type.Grid1D2DLike) -> aa.type.Grid1D2DLike:
         return self.potential_2d_from(grid=grid)
 
     def potential_func(self, u, y, x):
         raise NotImplementedError
 
     def mass_integral(self, x):
@@ -82,15 +82,16 @@
         """
 
         return quad(self.mass_integral, a=0.0, b=radius)[0]
 
     def density_between_circular_annuli(
         self, inner_annuli_radius: float, outer_annuli_radius: float
     ):
-        """Calculate the mass between two circular annuli and compute the density by dividing by the annuli surface
+        """
+        Calculate the mass between two circular annuli and compute the density by dividing by the annuli surface
         area.
 
         The value returned by the mass integral is dimensionless, therefore the density between annuli is returned in \
         unit_label of inverse radius squared. A conversion factor can be specified to convert this to a physical value \
         (e.g. the critical surface mass density).
 
         Parameters
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/abstract/cse.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/abstract/cse.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,18 +110,22 @@
 
         results = lstsq(coefficient_matrix, y_samples.T)
 
         amplitude_list = results[0]
 
         return amplitude_list, core_radius_list
 
-    def convergence_2d_via_cse_from(self, grid_radii: np.ndarray) -> np.ndarray:
+    def convergence_2d_via_cse_from(
+        self, grid_radii: np.ndarray, **kwargs
+    ) -> np.ndarray:
         pass
 
-    def _convergence_2d_via_cse_from(self, grid_radii: np.ndarray) -> np.ndarray:
+    def _convergence_2d_via_cse_from(
+        self, grid_radii: np.ndarray, **kwargs
+    ) -> np.ndarray:
         """
         Calculate the projected 2D convergence from a grid of radial coordinates, by computing and summing the
         convergence of each individual cse used to decompose the mass profile.
 
         The cored steep elliptical (cse) decomposition of a given mass profile (e.g. `convergence_cse_1d_from`) is
         defined for every mass profile and defines how it is efficiently decomposed its cses.
 
@@ -139,30 +143,30 @@
             amplitude
             * self.convergence_cse_1d_from(
                 grid_radii=grid_radii, core_radius=core_radius
             )
             for amplitude, core_radius in zip(amplitude_list, core_radius_list)
         )
 
-    def _deflections_2d_via_cse_from(self, grid: np.ndarray) -> np.ndarray:
+    def _deflections_2d_via_cse_from(self, grid: np.ndarray, **kwargs) -> np.ndarray:
         """
         Calculate the projected 2D deflection angles from a grid of radial coordinates, by computing and summing the
         deflections of each individual cse used to decompose the mass profile.
 
         The cored steep elliptical (cse) decomposition of a given mass profile (e.g. `convergence_cse_1d_from`) is
         defined for every mass profile and defines how it is efficiently decomposed its cses.
 
         Parameters
         ----------
         grid_radii
             The grid of 1D radial arc-second coordinates the convergence is computed on.
         """
 
         amplitude_list, core_radius_list = self.decompose_convergence_via_cse(
-            grid_radii=self.radial_grid_from(grid=grid)
+            grid_radii=self.radial_grid_from(grid=grid, **kwargs)
         )
         q = self.axis_ratio
         q2 = q**2.0
         grid_y = grid[:, 0]
         grid_x = grid[:, 1]
         gridx2 = grid_x**2.0
         gridy2 = grid_y**2.0
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/abstract/mge.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/abstract/mge.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,16 +122,16 @@
 
         output_grid_final = np.zeros(grid.shape[0], dtype="complex128")
 
         q2 = axis_ratio**2.0
 
         scale_factor = axis_ratio / (sigmas[0] * np.sqrt(2.0 * (1.0 - q2)))
 
-        xs = (grid[:, 1] * scale_factor).copy()
-        ys = (grid[:, 0] * scale_factor).copy()
+        xs = np.array((grid[:, 1] * scale_factor).copy())
+        ys = np.array((grid[:, 0] * scale_factor).copy())
 
         ys_minus = ys < 0.0
         ys[ys_minus] *= -1
         z = xs + 1j * ys
         zq = axis_ratio * xs + 1j * ys / axis_ratio
 
         expv = -(xs**2.0) * (1.0 - q2) - ys**2.0 * (1.0 / q2 - 1.0)
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/dark/abstract.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/dark/abstract.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,61 +52,63 @@
         super().__init__(centre=centre, ell_comps=ell_comps)
         super(MassProfileMGE, self).__init__()
 
         self.kappa_s = kappa_s
         self.scale_radius = scale_radius
         self.inner_slope = inner_slope
 
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.over_sample
+    @aa.grid_dec.to_array
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
-    def convergence_2d_from(self, grid: aa.type.Grid2DLike):
+    def convergence_2d_from(self, grid: aa.type.Grid2DLike, **kwargs):
         """Calculate the projected convergence at a given set of arc-second gridded coordinates.
 
         Parameters
         ----------
         grid
             The grid of (y,x) arc-second coordinates the convergence is computed on.
 
         """
 
-        grid_eta = self.elliptical_radii_grid_from(grid=grid)
+        grid_eta = self.elliptical_radii_grid_from(grid=grid, **kwargs)
 
         return self.convergence_func(grid_radius=grid_eta)
 
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.over_sample
+    @aa.grid_dec.to_array
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
-    def convergence_2d_via_mge_from(self, grid: aa.type.Grid2DLike):
+    def convergence_2d_via_mge_from(self, grid: aa.type.Grid2DLike, **kwargs):
         """Calculate the projected convergence at a given set of arc-second gridded coordinates.
 
         Parameters
         ----------
         grid
             The grid of (y,x) arc-second coordinates the convergence is computed on.
 
         """
 
-        elliptical_radii = self.elliptical_radii_grid_from(grid)
+        elliptical_radii = self.elliptical_radii_grid_from(grid=grid, **kwargs)
 
         return self._convergence_2d_via_mge_from(grid_radii=elliptical_radii)
 
-    def tabulate_integral(self, grid, tabulate_bins):
+    def tabulate_integral(self, grid, tabulate_bins, **kwargs):
         """Tabulate an integral over the convergence of deflection potential of a mass profile. This is used in \
         the GeneralizedNFW profile classes to speed up the integration procedure.
 
         Parameters
         ----------
         grid
             The grid of (y,x) arc-second coordinates the potential / deflection_stacks are computed on.
         tabulate_bins
             The number of bins to tabulate the inner integral of this profile.
         """
         eta_min = 1.0e-4
-        eta_max = 1.05 * np.max(self.elliptical_radii_grid_from(grid))
+        eta_max = 1.05 * np.max(self.elliptical_radii_grid_from(grid=grid, **kwargs))
 
         minimum_log_eta = np.log10(eta_min)
         maximum_log_eta = np.log10(eta_max)
         bin_size = (maximum_log_eta - minimum_log_eta) / (tabulate_bins - 1)
 
         return eta_min, eta_max, minimum_log_eta, maximum_log_eta, bin_size
 
@@ -129,21 +131,21 @@
         amplitude_list, sigma_list = self._decompose_convergence_via_mge(
             func=gnfw_3d, radii_min=radii_min, radii_max=radii_max
         )
         amplitude_list *= np.sqrt(2.0 * np.pi) * sigma_list
         return amplitude_list, sigma_list
 
     def coord_func_f(self, grid_radius):
-        if isinstance(grid_radius, np.ndarray):
-            return self.coord_func_f_jit(
-                grid_radius=grid_radius,
-                f=np.ones(shape=grid_radius.shape[0], dtype="complex64"),
-            )
-        else:
-            return self.coord_func_f_float_jit(grid_radius=grid_radius)
+        if isinstance(grid_radius, float) or isinstance(grid_radius, complex):
+            grid_radius = np.array([grid_radius])
+
+        return self.coord_func_f_jit(
+            grid_radius=np.array(grid_radius),
+            f=np.ones(shape=grid_radius.shape[0], dtype="complex64"),
+        )
 
     @staticmethod
     @aa.util.numba.jit()
     def coord_func_f_jit(grid_radius, f):
         for index in range(f.shape[0]):
             if np.real(grid_radius[index]) > 1.0:
                 f[index] = (
@@ -152,63 +154,39 @@
             elif np.real(grid_radius[index]) < 1.0:
                 f[index] = (
                     1.0 / np.sqrt(1.0 - np.square(grid_radius[index]))
                 ) * np.arccosh(np.divide(1.0, grid_radius[index]))
 
         return f
 
-    @staticmethod
-    @aa.util.numba.jit()
-    def coord_func_f_float_jit(grid_radius):
-        if np.real(grid_radius) > 1.0:
-            return (1.0 / np.sqrt(np.square(grid_radius) - 1.0)) * np.arccos(
-                np.divide(1.0, grid_radius)
-            )
-        elif np.real(grid_radius) < 1.0:
-            return (1.0 / np.sqrt(1.0 - np.square(grid_radius))) * np.arccosh(
-                np.divide(1.0, grid_radius)
-            )
-        else:
-            return 1.0
-
     def coord_func_g(self, grid_radius):
+        if isinstance(grid_radius, float) or isinstance(grid_radius, complex):
+            grid_radius = np.array([grid_radius])
+
         f_r = self.coord_func_f(grid_radius=grid_radius)
 
-        if isinstance(grid_radius, np.ndarray):
-            return self.coord_func_g_jit(
-                grid_radius=grid_radius,
-                f_r=f_r,
-                g=np.zeros(shape=grid_radius.shape[0], dtype="complex64"),
-            )
-        else:
-            return self.coord_func_g_float_jit(grid_radius=grid_radius, f_r=f_r)
+        return self.coord_func_g_jit(
+            grid_radius=np.array(grid_radius),
+            f_r=f_r,
+            g=np.zeros(shape=grid_radius.shape[0], dtype="complex64"),
+        )
 
     @staticmethod
     @aa.util.numba.jit()
     def coord_func_g_jit(grid_radius, f_r, g):
         for index in range(f_r.shape[0]):
             if np.real(grid_radius[index]) > 1.0:
                 g[index] = (1.0 - f_r[index]) / (np.square(grid_radius[index]) - 1.0)
             elif np.real(grid_radius[index]) < 1.0:
                 g[index] = (f_r[index] - 1.0) / (1.0 - np.square(grid_radius[index]))
             else:
                 g[index] = 1.0 / 3.0
 
         return g
 
-    @staticmethod
-    @aa.util.numba.jit()
-    def coord_func_g_float_jit(grid_radius, f_r):
-        if np.real(grid_radius) > 1.0:
-            return (1.0 - f_r) / (np.square(grid_radius) - 1.0)
-        elif np.real(grid_radius) < 1.0:
-            return (f_r - 1.0) / (1.0 - np.square(grid_radius))
-        else:
-            return 1.0 / 3.0
-
     def coord_func_h(self, grid_radius):
         return np.log(grid_radius / 2.0) + self.coord_func_f(grid_radius=grid_radius)
 
     def rho_at_scale_radius_solar_mass_per_kpc3(
         self, redshift_object, redshift_source, cosmology: LensingCosmology = Planck15()
     ):
         """
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/dark/gnfw.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/dark/gnfw.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,30 +79,30 @@
 
     cf = cfunc(float64(intc, CPointer(float64)))
 
     return LowLevelCallable(cf(wrapped).ctypes)
 
 
 class gNFW(AbstractgNFW):
-    def deflections_yx_2d_from(self, grid: aa.type.Grid2DLike):
-        return self.deflections_2d_via_mge_from(grid=grid)
+    def deflections_yx_2d_from(self, grid: aa.type.Grid2DLike, **kwargs):
+        return self.deflections_2d_via_mge_from(grid=grid, **kwargs)
 
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.grid_dec.to_vector_yx
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
-    def deflections_2d_via_mge_from(self, grid: aa.type.Grid2DLike):
+    def deflections_2d_via_mge_from(self, grid: aa.type.Grid2DLike, **kwargs):
         return self._deflections_2d_via_mge_from(
             grid=grid, sigmas_factor=self.axis_ratio
         )
 
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.grid_dec.to_vector_yx
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
     def deflections_2d_via_integral_from(
-        self, grid: aa.type.Grid2DLike, tabulate_bins=1000
+        self, grid: aa.type.Grid2DLike, tabulate_bins=1000, **kwargs
     ):
         """
         Calculate the deflection angles at a given set of arc-second gridded coordinates.
 
         Parameters
         ----------
         grid
@@ -226,18 +226,19 @@
                     (1 + grid_radius[index]) ** (self.inner_slope - 3)
                     + ((3 - self.inner_slope) * integral_y_value)
                 )
             )
 
         return grid_radius
 
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.over_sample
+    @aa.grid_dec.to_array
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
-    def potential_2d_from(self, grid: aa.type.Grid2DLike, tabulate_bins=1000):
+    def potential_2d_from(self, grid: aa.type.Grid2DLike, tabulate_bins=1000, **kwargs):
         """
         Calculate the potential at a given set of arc-second gridded coordinates.
 
         Parameters
         ----------
         grid
             The grid of (y,x) arc-second coordinates the deflection angles are computed on.
@@ -358,37 +359,39 @@
             centre=centre,
             ell_comps=(0.0, 0.0),
             kappa_s=kappa_s,
             inner_slope=inner_slope,
             scale_radius=scale_radius,
         )
 
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.grid_dec.to_vector_yx
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
     def deflections_2d_via_integral_from(self, grid: aa.type.Grid2DLike, **kwargs):
         """
         Calculate the deflection angles at a given set of arc-second gridded coordinates.
 
         Parameters
         ----------
         grid
             The grid of (y,x) arc-second coordinates the deflection angles are computed on.
         """
 
-        eta = np.multiply(1.0 / self.scale_radius, self.radial_grid_from(grid))
+        eta = np.multiply(
+            1.0 / self.scale_radius, self.radial_grid_from(grid, **kwargs)
+        )
 
         deflection_grid = np.zeros(grid.shape[0])
 
         for i in range(grid.shape[0]):
             deflection_grid[i] = np.multiply(
                 4.0 * self.kappa_s * self.scale_radius, self.deflection_func_sph(eta[i])
             )
 
-        return self._cartesian_grid_via_radial_from(grid, deflection_grid)
+        return self._cartesian_grid_via_radial_from(grid=grid, radius=deflection_grid)
 
     @staticmethod
     def deflection_integrand(y, eta, inner_slope):
         return (y + eta) ** (inner_slope - 3) * ((1 - np.sqrt(1 - y**2)) / y)
 
     def deflection_func_sph(self, eta):
         integral_y_2 = quad(
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/dark/gnfw_mcr.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/dark/gnfw_mcr.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/dark/mcr_util.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/dark/mcr_util.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/dark/nfw.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/dark/nfw.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,21 +37,21 @@
             ell_comps=ell_comps,
             kappa_s=kappa_s,
             inner_slope=1.0,
             scale_radius=scale_radius,
         )
         super(MassProfileCSE, self).__init__()
 
-    def deflections_yx_2d_from(self, grid: aa.type.Grid2DLike):
-        return self.deflections_2d_via_cse_from(grid=grid)
+    def deflections_yx_2d_from(self, grid: aa.type.Grid2DLike, **kwargs):
+        return self.deflections_2d_via_cse_from(grid=grid, **kwargs)
 
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.grid_dec.to_vector_yx
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
-    def deflections_2d_via_integral_from(self, grid: aa.type.Grid2DLike):
+    def deflections_2d_via_integral_from(self, grid: aa.type.Grid2DLike, **kwargs):
         """
         Calculate the deflection angles at a given set of arc-second gridded coordinates.
 
         Parameters
         ----------
         grid
             The grid of (y,x) arc-second coordinates the deflection angles are computed on.
@@ -83,19 +83,19 @@
         deflection_y = calculate_deflection_component(1.0, 0)
         deflection_x = calculate_deflection_component(0.0, 1)
 
         return self.rotated_grid_from_reference_frame_from(
             np.multiply(1.0, np.vstack((deflection_y, deflection_x)).T)
         )
 
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.grid_dec.to_vector_yx
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
-    def deflections_2d_via_cse_from(self, grid: aa.type.Grid2DLike):
-        return self._deflections_2d_via_cse_from(grid=grid)
+    def deflections_2d_via_cse_from(self, grid: aa.type.Grid2DLike, **kwargs):
+        return self._deflections_2d_via_cse_from(grid=grid, **kwargs)
 
     @staticmethod
     def deflection_func(u, y, x, npow, axis_ratio, scale_radius):
         _eta_u = (1.0 / scale_radius) * np.sqrt(
             (u * ((x**2) + (y**2 / (1 - (1 - axis_ratio**2) * u))))
         )
 
@@ -113,44 +113,46 @@
         return (
             2.0
             * (1 - _eta_u_2)
             / (_eta_u**2 - 1)
             / ((1 - (1 - axis_ratio**2) * u) ** (npow + 0.5))
         )
 
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.over_sample
+    @aa.grid_dec.to_array
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
-    def convergence_2d_via_cse_from(self, grid: aa.type.Grid2DLike):
+    def convergence_2d_via_cse_from(self, grid: aa.type.Grid2DLike, **kwargs):
         """
         Calculate the projected 2D convergence from a grid of (y,x) arc second coordinates, by computing and summing
         the convergence of each individual cse used to decompose the mass profile.
 
         The cored steep elliptical (cse) decomposition of a the elliptical NFW mass
         profile (e.g. `decompose_convergence_via_cse`) is using equation (12) of
         Oguri 2021 (https://arxiv.org/abs/2106.11464).
 
         Parameters
         ----------
         grid
             The grid of (y,x) arc-second coordinates the convergence is computed on.
         """
 
-        elliptical_radii = self.elliptical_radii_grid_from(grid)
+        elliptical_radii = self.elliptical_radii_grid_from(grid=grid, **kwargs)
 
         return self._convergence_2d_via_cse_from(grid_radii=elliptical_radii)
 
     def convergence_func(self, grid_radius: float) -> float:
         grid_radius = (1.0 / self.scale_radius) * grid_radius + 0j
         return np.real(2.0 * self.kappa_s * self.coord_func_g(grid_radius=grid_radius))
 
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.over_sample
+    @aa.grid_dec.to_array
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
-    def potential_2d_from(self, grid: aa.type.Grid2DLike):
+    def potential_2d_from(self, grid: aa.type.Grid2DLike, **kwargs):
         """
         Calculate the potential at a given set of arc-second gridded coordinates.
 
         Parameters
         ----------
         grid
             The grid of (y,x) arc-second coordinates the deflection angles are computed on.
@@ -283,57 +285,62 @@
         super().__init__(
             centre=centre,
             ell_comps=(0.0, 0.0),
             kappa_s=kappa_s,
             scale_radius=scale_radius,
         )
 
-    def deflections_yx_2d_from(self, grid: aa.type.Grid2DLike):
-        return self.deflections_2d_via_analytic_from(grid=grid)
+    def deflections_yx_2d_from(self, grid: aa.type.Grid2DLike, **kwargs):
+        return self.deflections_2d_via_analytic_from(grid=grid, **kwargs)
 
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.grid_dec.to_vector_yx
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
-    def deflections_2d_via_analytic_from(self, grid: aa.type.Grid2DLike):
+    def deflections_2d_via_analytic_from(self, grid: aa.type.Grid2DLike, **kwargs):
         """
         Calculate the deflection angles at a given set of arc-second gridded coordinates.
 
         Parameters
         ----------
         grid
             The grid of (y,x) arc-second coordinates the deflection angles are computed on.
         """
 
-        eta = np.multiply(1.0 / self.scale_radius, self.radial_grid_from(grid=grid))
+        eta = np.multiply(
+            1.0 / self.scale_radius, self.radial_grid_from(grid=grid, **kwargs)
+        )
 
         deflection_grid = np.multiply(
             (4.0 * self.kappa_s * self.scale_radius / eta),
             self.deflection_func_sph(grid_radius=eta),
         )
 
-        return self._cartesian_grid_via_radial_from(grid, deflection_grid)
+        return self._cartesian_grid_via_radial_from(grid=grid, radius=deflection_grid)
 
     def deflection_func_sph(self, grid_radius):
         grid_radius = grid_radius + 0j
         return np.real(self.coord_func_h(grid_radius=grid_radius))
 
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.over_sample
+    @aa.grid_dec.to_array
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
-    def potential_2d_from(self, grid: aa.type.Grid2DLike):
+    def potential_2d_from(self, grid: aa.type.Grid2DLike, **kwargs):
         """
         Calculate the potential at a given set of arc-second gridded coordinates.
 
         Parameters
         ----------
         grid
             The grid of (y,x) arc-second coordinates the deflection angles are computed on.
 
         """
-        eta = (1.0 / self.scale_radius) * self.radial_grid_from(grid) + 0j
+        eta = (1.0 / self.scale_radius) * self.radial_grid_from(
+            grid=grid, **kwargs
+        ) + 0j
         return np.real(
             2.0 * self.scale_radius * self.kappa_s * self.potential_func_sph(eta)
         )
 
     @staticmethod
     def potential_func_sph(eta):
         return ((np.log(eta / 2.0)) ** 2) - (np.arctanh(np.sqrt(1 - eta**2))) ** 2
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/dark/nfw_mcr.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/dark/nfw_mcr.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/dark/nfw_mcr_scatter.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/dark/nfw_mcr_scatter.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/dark/nfw_truncated.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/dark/nfw_truncated.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,47 +23,48 @@
             inner_slope=1.0,
             scale_radius=scale_radius,
         )
 
         self.truncation_radius = truncation_radius
         self.tau = self.truncation_radius / self.scale_radius
 
-    @aa.grid_dec.grid_2d_to_vector_yx
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.grid_dec.to_vector_yx
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
     def deflections_yx_2d_from(self, grid: aa.type.Grid2DLike, **kwargs):
         """
         Calculate the deflection angles at a given set of arc-second gridded coordinates.
 
         Parameters
         ----------
         grid
             The grid of (y,x) arc-second coordinates the deflection angles are computed on.
         """
 
-        eta = np.multiply(1.0 / self.scale_radius, self.radial_grid_from(grid=grid))
+        eta = np.multiply(
+            1.0 / self.scale_radius, self.radial_grid_from(grid=grid, **kwargs)
+        )
 
         deflection_grid = np.multiply(
             (4.0 * self.kappa_s * self.scale_radius / eta),
             self.deflection_func_sph(grid_radius=eta),
         )
 
-        return self._cartesian_grid_via_radial_from(grid, deflection_grid)
+        return self._cartesian_grid_via_radial_from(grid=grid, radius=deflection_grid)
 
     def deflection_func_sph(self, grid_radius):
         grid_radius = grid_radius + 0j
         return np.real(self.coord_func_m(grid_radius=grid_radius))
 
     def convergence_func(self, grid_radius: float) -> float:
         grid_radius = ((1.0 / self.scale_radius) * grid_radius) + 0j
         return np.real(2.0 * self.kappa_s * self.coord_func_l(grid_radius=grid_radius))
 
-    @aa.grid_dec.grid_2d_to_structure
-    def potential_2d_from(self, grid: aa.type.Grid2DLike):
+    @aa.grid_dec.to_array
+    def potential_2d_from(self, grid: aa.type.Grid2DLike, **kwargs):
         return np.zeros(shape=grid.shape[0])
 
     def coord_func_k(self, grid_radius):
         return np.log(
             np.divide(
                 grid_radius,
                 np.sqrt(np.square(grid_radius) + np.square(self.tau)) + self.tau,
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/dark/nfw_truncated_mcr.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/dark/nfw_truncated_mcr.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/dark/nfw_truncated_mcr_scatter.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/dark/nfw_truncated_mcr_scatter.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/dark/nfw_virial_mass_conc.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/dark/nfw_virial_mass_conc.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/mock/mock_mass_profile.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/mock/mock_mass_profile.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/point/point.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/point/point.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,34 +20,33 @@
             The (y,x) arc-second coordinates of the profile centre.
         einstein_radius
             The arc-second Einstein radius of the point-mass.
         """
         super().__init__(centre=centre, ell_comps=(0.0, 0.0))
         self.einstein_radius = einstein_radius
 
-    def convergence_2d_from(self, grid: aa.type.Grid2DLike):
+    def convergence_2d_from(self, grid: aa.type.Grid2DLike, **kwargs):
         squared_distances = np.square(grid[:, 0] - self.centre[0]) + np.square(
             grid[:, 1] - self.centre[1]
         )
         central_pixel = np.argmin(squared_distances)
 
         convergence = np.zeros(shape=grid.shape[0])
         #    convergence[central_pixel] = np.pi * self.einstein_radius ** 2.0
         return convergence
 
-    @aa.grid_dec.grid_2d_to_structure
-    def potential_2d_from(self, grid: aa.type.Grid2DLike):
+    @aa.grid_dec.to_array
+    def potential_2d_from(self, grid: aa.type.Grid2DLike, **kwargs):
         return np.zeros(shape=grid.shape[0])
 
-    @aa.grid_dec.grid_2d_to_vector_yx
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.grid_dec.to_vector_yx
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
-    def deflections_yx_2d_from(self, grid: aa.type.Grid2DLike):
-        grid_radii = self.radial_grid_from(grid=grid)
+    def deflections_yx_2d_from(self, grid: aa.type.Grid2DLike, **kwargs):
+        grid_radii = self.radial_grid_from(grid=grid, **kwargs)
         return self._cartesian_grid_via_radial_from(
             grid=grid, radius=self.einstein_radius**2 / grid_radii
         )
 
     @property
     def is_point_mass(self):
         return True
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/point/smbh.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/point/smbh.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/point/smbh_binary.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/point/smbh_binary.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,52 +86,52 @@
     @property
     def angle_binary_radians(self) -> float:
         """
         The angle between the two SMBHs in radians.
         """
         return self.angle_binary * np.pi / 180.0
 
-    def convergence_2d_from(self, grid: aa.type.Grid2DLike):
+    def convergence_2d_from(self, grid: aa.type.Grid2DLike, **kwargs):
         """
         Returns the two dimensional projected convergence on a grid of (y,x) arc-second coordinates.
 
         The convergence is computed as the sum of the convergence of the two individual `SMBH` profiles in the binary.
 
         Parameters
         ----------
         grid
             The grid of (y,x) arc-second coordinates the convergence is computed on.
         """
         return self.smbh_0.convergence_2d_from(
             grid=grid
-        ) + self.smbh_1.convergence_2d_from(grid=grid)
+        ) + self.smbh_1.convergence_2d_from(grid=grid, **kwargs)
 
-    def potential_2d_from(self, grid: aa.type.Grid2DLike):
+    def potential_2d_from(self, grid: aa.type.Grid2DLike, **kwargs):
         """
         Returns the two dimensional projected potential on a grid of (y,x) arc-second coordinates.
 
         The potential is computed as the sum of the potential of the two individual `SMBH` profiles in the binary.
 
         Parameters
         ----------
         grid
             The grid of (y,x) arc-second coordinates the potential is computed on.
         """
-        return self.smbh_0.potential_2d_from(grid=grid) + self.smbh_1.potential_2d_from(
-            grid=grid
-        )
+        return self.smbh_0.potential_2d_from(
+            grid=grid, **kwargs
+        ) + self.smbh_1.potential_2d_from(grid=grid)
 
-    def deflections_yx_2d_from(self, grid: aa.type.Grid2DLike):
+    def deflections_yx_2d_from(self, grid: aa.type.Grid2DLike, **kwargs):
         """
         Returns the two dimensional deflection angles on a grid of (y,x) arc-second coordinates.
 
         The deflection angles are computed as the sum of the convergence of the two individual `SMBH` profiles in the
         binary.
 
         Parameters
         ----------
         grid
             The grid of (y,x) arc-second coordinates the deflection angles are computed on.
         """
         return self.smbh_0.deflections_yx_2d_from(
             grid=grid
-        ) + self.smbh_1.deflections_yx_2d_from(grid=grid)
+        ) + self.smbh_1.deflections_yx_2d_from(grid=grid, **kwargs)
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/sheets/external_shear.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/sheets/external_shear.py`

 * *Files 11% similar despite different names*

```diff
@@ -34,35 +34,34 @@
 
     def convergence_func(self, grid_radius: float) -> float:
         return 0.0
 
     def average_convergence_of_1_radius(self):
         return 0.0
 
-    @aa.grid_dec.grid_2d_to_structure
-    def convergence_2d_from(self, grid: aa.type.Grid2DLike):
+    @aa.grid_dec.to_array
+    def convergence_2d_from(self, grid: aa.type.Grid2DLike, **kwargs):
         return np.zeros(shape=grid.shape[0])
 
-    @aa.grid_dec.grid_2d_to_structure
-    def potential_2d_from(self, grid: aa.type.Grid2DLike):
+    @aa.grid_dec.to_array
+    def potential_2d_from(self, grid: aa.type.Grid2DLike, **kwargs):
         shear_angle = (
             self.angle - 90
         )  ##to be onsistent with autolens deflection angle calculation
         phig = np.deg2rad(shear_angle)
         shear_amp = self.magnitude
         phicoord = np.arctan2(grid[:, 0], grid[:, 1])
         rcoord = np.sqrt(grid[:, 0] ** 2.0 + grid[:, 1] ** 2.0)
 
         return -0.5 * shear_amp * rcoord**2 * np.cos(2 * (phicoord - phig))
 
-    @aa.grid_dec.grid_2d_to_vector_yx
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.grid_dec.to_vector_yx
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
-    def deflections_yx_2d_from(self, grid: aa.type.Grid2DLike):
+    def deflections_yx_2d_from(self, grid: aa.type.Grid2DLike, **kwargs):
         """
         Calculate the deflection angles at a given set of arc-second gridded coordinates.
 
         Parameters
         ----------
         grid
             The grid of (y,x) arc-second coordinates the deflection angles are computed on.
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/sheets/input_deflections.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/sheets/input_deflections.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,39 +64,38 @@
             self.normalization_scale = 1.0
             self.preload_blurring_deflections = self.deflections_yx_2d_from(
                 grid=preload_blurring_grid
             )
 
         self.normalization_scale = 1.0  # normalization_scale
 
-    @aa.grid_dec.grid_2d_to_structure
-    def convergence_2d_from(self, grid: aa.type.Grid2DLike):
-        return self.convergence_2d_via_jacobian_from(grid=grid)
+    @aa.grid_dec.to_array
+    def convergence_2d_from(self, grid: aa.type.Grid2DLike, **kwargs):
+        return self.convergence_2d_via_jacobian_from(grid=grid, **kwargs)
 
-    @aa.grid_dec.grid_2d_to_structure
-    def potential_2d_from(self, grid: aa.type.Grid2DLike):
+    @aa.grid_dec.to_array
+    def potential_2d_from(self, grid: aa.type.Grid2DLike, **kwargs):
         return np.zeros(shape=grid.shape[0])
 
-    @aa.grid_dec.grid_2d_to_vector_yx
-    @aa.grid_dec.grid_2d_to_structure
-    def deflections_yx_2d_from(self, grid: aa.type.Grid2DLike):
+    @aa.grid_dec.to_vector_yx
+    def deflections_yx_2d_from(self, grid: aa.type.Grid2DLike, **kwargs):
         if self.preload_grid is not None and self.preload_deflections is not None:
             try:
-                if grid.sub_shape_slim == self.preload_grid.sub_shape_slim:
+                if grid.shape_slim == self.preload_grid.shape_slim:
                     if np.allclose(grid, self.preload_grid, 1e-8):
                         return self.normalization_scale * self.preload_deflections
             except AttributeError:
                 pass
 
         if (
             self.preload_blurring_grid is not None
             and self.preload_blurring_deflections is not None
         ):
             try:
-                if grid.sub_shape_slim == self.preload_blurring_grid.sub_shape_slim:
+                if grid.shape_slim == self.preload_blurring_grid.shape_slim:
                     if np.allclose(grid, self.preload_blurring_grid, 1e-8):
                         return (
                             self.normalization_scale * self.preload_blurring_deflections
                         )
             except AttributeError:
                 pass
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/stellar/chameleon.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/stellar/chameleon.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,21 +44,21 @@
         super(Chameleon, self).__init__(centre=centre, ell_comps=ell_comps)
         super(MassProfile, self).__init__(centre=centre, ell_comps=ell_comps)
         self.mass_to_light_ratio = mass_to_light_ratio
         self.intensity = intensity
         self.core_radius_0 = core_radius_0
         self.core_radius_1 = core_radius_1
 
-    def deflections_yx_2d_from(self, grid: aa.type.Grid2DLike):
-        return self.deflections_2d_via_analytic_from(grid=grid)
+    def deflections_yx_2d_from(self, grid: aa.type.Grid2DLike, **kwargs):
+        return self.deflections_2d_via_analytic_from(grid=grid, **kwargs)
 
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.grid_dec.to_vector_yx
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
-    def deflections_2d_via_analytic_from(self, grid: aa.type.Grid2DLike):
+    def deflections_2d_via_analytic_from(self, grid: aa.type.Grid2DLike, **kwargs):
         """
         Calculate the deflection angles at a given set of arc-second gridded coordinates.
         Following Eq. (15) and (16), but the parameters are slightly different.
 
         Parameters
         ----------
         grid
@@ -120,31 +120,34 @@
         deflection_y = np.subtract(deflection_y0, deflection_y1)
         deflection_x = np.subtract(deflection_x0, deflection_x1)
 
         return self.rotated_grid_from_reference_frame_from(
             np.multiply(factor, np.vstack((deflection_y, deflection_x)).T)
         )
 
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.over_sample
+    @aa.grid_dec.to_array
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
-    def convergence_2d_from(self, grid: aa.type.Grid2DLike):
+    def convergence_2d_from(self, grid: aa.type.Grid2DLike, **kwargs):
         """Calculate the projected convergence at a given set of arc-second gridded coordinates.
         Parameters
         ----------
         grid
             The grid of (y,x) arc-second coordinates the convergence is computed on.
         """
-        return self.convergence_func(self.elliptical_radii_grid_from(grid))
+        return self.convergence_func(
+            self.elliptical_radii_grid_from(grid=grid, **kwargs)
+        )
 
     def convergence_func(self, grid_radius: float) -> float:
         return self.mass_to_light_ratio * self.image_2d_via_radii_from(grid_radius)
 
-    @aa.grid_dec.grid_2d_to_structure
-    def potential_2d_from(self, grid: aa.type.Grid2DLike):
+    @aa.grid_dec.to_array
+    def potential_2d_from(self, grid: aa.type.Grid2DLike, **kwargs):
         return np.zeros(shape=grid.shape[0])
 
     def image_2d_via_radii_from(self, grid_radii: np.ndarray):
         """Calculate the intensity of the Chamelon light profile on a grid of radial coordinates.
 
         Parameters
         ----------
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/stellar/dev_vaucouleurs.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/stellar/dev_vaucouleurs.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/stellar/exponential.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/stellar/exponential.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/stellar/gaussian.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/stellar/gaussian.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,30 +37,30 @@
 
         super(Gaussian, self).__init__(centre=centre, ell_comps=ell_comps)
         super(MassProfile, self).__init__(centre=centre, ell_comps=ell_comps)
         self.mass_to_light_ratio = mass_to_light_ratio
         self.intensity = intensity
         self.sigma = sigma
 
-    def deflections_yx_2d_from(self, grid: aa.type.Grid2DLike):
+    def deflections_yx_2d_from(self, grid: aa.type.Grid2DLike, **kwargs):
         """
         Calculate the deflection angles at a given set of arc-second gridded coordinates.
 
         Parameters
         ----------
         grid
             The grid of (y,x) arc-second coordinates the deflection angles are computed on.
 
         """
-        return self.deflections_2d_via_analytic_from(grid=grid)
+        return self.deflections_2d_via_analytic_from(grid=grid, **kwargs)
 
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.grid_dec.to_vector_yx
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
-    def deflections_2d_via_analytic_from(self, grid: aa.type.Grid2DLike):
+    def deflections_2d_via_analytic_from(self, grid: aa.type.Grid2DLike, **kwargs):
         """
         Calculate the deflection angles at a given set of arc-second gridded coordinates.
 
         Parameters
         ----------
         grid
             The grid of (y,x) arc-second coordinates the deflection angles are computed on.
@@ -77,18 +77,18 @@
 
         return self.rotated_grid_from_reference_frame_from(
             np.multiply(
                 1.0, np.vstack((-1.0 * np.imag(deflections), np.real(deflections))).T
             )
         )
 
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.grid_dec.to_vector_yx
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
-    def deflections_2d_via_integral_from(self, grid: aa.type.Grid2DLike):
+    def deflections_2d_via_integral_from(self, grid: aa.type.Grid2DLike, **kwargs):
         """
         Calculate the deflection angles at a given set of arc-second gridded coordinates.
 
         Parameters
         ----------
         grid
             The grid of (y,x) arc-second coordinates the deflection angles are computed on.
@@ -133,33 +133,36 @@
             (u * ((x**2) + (y**2 / (1 - (1 - axis_ratio**2) * u))))
         )
 
         return np.exp(-0.5 * np.square(np.divide(_eta_u, sigma))) / (
             (1 - (1 - axis_ratio**2) * u) ** (npow + 0.5)
         )
 
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.over_sample
+    @aa.grid_dec.to_array
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
-    def convergence_2d_from(self, grid: aa.type.Grid2DLike):
+    def convergence_2d_from(self, grid: aa.type.Grid2DLike, **kwargs):
         """Calculate the projected convergence at a given set of arc-second gridded coordinates.
 
         Parameters
         ----------
         grid
             The grid of (y,x) arc-second coordinates the convergence is computed on.
 
         """
-        return self.convergence_func(self.eccentric_radii_grid_from(grid))
+        return self.convergence_func(
+            self.eccentric_radii_grid_from(grid=grid, **kwargs)
+        )
 
     def convergence_func(self, grid_radius: float) -> float:
         return self.mass_to_light_ratio * self.image_2d_via_radii_from(grid_radius)
 
-    @aa.grid_dec.grid_2d_to_structure
-    def potential_2d_from(self, grid: aa.type.Grid2DLike):
+    @aa.grid_dec.to_array
+    def potential_2d_from(self, grid: aa.type.Grid2DLike, **kwargs):
         return np.zeros(shape=grid.shape[0])
 
     def image_2d_via_radii_from(self, grid_radii: np.ndarray):
         """Calculate the intensity of the Gaussian light profile on a grid of radial coordinates.
 
         Parameters
         ----------
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/stellar/sersic.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/stellar/sersic.py`

 * *Files 4% similar despite different names*

```diff
@@ -117,21 +117,21 @@
         super(MassProfileMGE, self).__init__()
         super(MassProfileCSE, self).__init__()
         self.mass_to_light_ratio = mass_to_light_ratio
         self.intensity = intensity
         self.effective_radius = effective_radius
         self.sersic_index = sersic_index
 
-    def deflections_yx_2d_from(self, grid: aa.type.Grid2DLike):
-        return self.deflections_2d_via_cse_from(grid=grid)
+    def deflections_yx_2d_from(self, grid: aa.type.Grid2DLike, **kwargs):
+        return self.deflections_2d_via_cse_from(grid=grid, **kwargs)
 
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.grid_dec.to_vector_yx
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
-    def deflections_2d_via_mge_from(self, grid: aa.type.Grid2DLike):
+    def deflections_2d_via_mge_from(self, grid: aa.type.Grid2DLike, **kwargs):
         """
         Calculate the projected 2D deflection angles from a grid of (y,x) arc second coordinates, by computing and
         summing the convergence of each individual cse used to decompose the mass profile.
 
         The cored steep elliptical (cse) decomposition of a the elliptical NFW mass
         profile (e.g. `decompose_convergence_via_cse`) is using equation (12) of
         Oguri 2021 (https://arxiv.org/abs/2106.11464).
@@ -141,92 +141,97 @@
         grid
             The grid of (y,x) arc-second coordinates the convergence is computed on.
         """
         return self._deflections_2d_via_mge_from(
             grid=grid, sigmas_factor=np.sqrt(self.axis_ratio)
         )
 
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.grid_dec.to_vector_yx
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
-    def deflections_2d_via_cse_from(self, grid: aa.type.Grid2DLike):
+    def deflections_2d_via_cse_from(self, grid: aa.type.Grid2DLike, **kwargs):
         """
         Calculate the projected 2D deflection angles from a grid of (y,x) arc second coordinates, by computing and
         summing the convergence of each individual cse used to decompose the mass profile.
 
         The cored steep elliptical (cse) decomposition of a the elliptical NFW mass
         profile (e.g. `decompose_convergence_via_cse`) is using equation (12) of
         Oguri 2021 (https://arxiv.org/abs/2106.11464).
 
         Parameters
         ----------
         grid
             The grid of (y,x) arc-second coordinates the convergence is computed on.
         """
-        return self._deflections_2d_via_cse_from(grid=grid)
+        return self._deflections_2d_via_cse_from(grid=grid, **kwargs)
 
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.over_sample
+    @aa.grid_dec.to_array
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
-    def convergence_2d_from(self, grid: aa.type.Grid2DLike):
+    def convergence_2d_from(self, grid: aa.type.Grid2DLike, **kwargs):
         """Calculate the projected convergence at a given set of arc-second gridded coordinates.
 
         Parameters
         ----------
         grid
             The grid of (y,x) arc-second coordinates the convergence is computed on.
 
         """
-        return self.convergence_func(self.eccentric_radii_grid_from(grid))
+        return self.convergence_func(
+            self.eccentric_radii_grid_from(grid=grid, **kwargs)
+        )
 
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.over_sample
+    @aa.grid_dec.to_array
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
-    def convergence_2d_via_mge_from(self, grid: aa.type.Grid2DLike):
+    def convergence_2d_via_mge_from(self, grid: aa.type.Grid2DLike, **kwargs):
         """
         Calculate the projected convergence at a given set of arc-second gridded coordinates.
 
         Parameters
         ----------
         grid
             The grid of (y,x) arc-second coordinates the convergence is computed on.
 
         """
 
-        eccentric_radii = self.eccentric_radii_grid_from(grid=grid)
+        eccentric_radii = self.eccentric_radii_grid_from(grid=grid, **kwargs)
 
         return self._convergence_2d_via_mge_from(grid_radii=eccentric_radii)
 
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.over_sample
+    @aa.grid_dec.to_array
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
-    def convergence_2d_via_cse_from(self, grid: aa.type.Grid2DLike):
+    def convergence_2d_via_cse_from(self, grid: aa.type.Grid2DLike, **kwargs):
         """
         Calculate the projected 2D convergence from a grid of (y,x) arc second coordinates, by computing and summing
         the convergence of each individual cse used to decompose the mass profile.
 
         The cored steep elliptical (cse) decomposition of a the elliptical NFW mass
         profile (e.g. `decompose_convergence_via_cse`) is using equation (12) of
         Oguri 2021 (https://arxiv.org/abs/2106.11464).
 
         Parameters
         ----------
         grid
             The grid of (y,x) arc-second coordinates the convergence is computed on.
         """
 
-        elliptical_radii = self.elliptical_radii_grid_from(grid=grid)
+        elliptical_radii = self.elliptical_radii_grid_from(grid=grid, **kwargs)
 
         return self._convergence_2d_via_cse_from(grid_radii=elliptical_radii)
 
     def convergence_func(self, grid_radius: float) -> float:
         return self.mass_to_light_ratio * self.image_2d_via_radii_from(grid_radius)
 
-    @aa.grid_dec.grid_2d_to_structure
-    def potential_2d_from(self, grid: aa.type.Grid2DLike):
+    @aa.grid_dec.to_array
+    def potential_2d_from(self, grid: aa.type.Grid2DLike, **kwargs):
         return np.zeros(shape=grid.shape[0])
 
     def image_2d_via_radii_from(self, radius: np.ndarray):
         """
         Returns the intensity of the profile at a given radius.
 
             Parameters
@@ -345,18 +350,18 @@
         The elliptical effective radius instead describes the major-axis radius of the ellipse containing \
         half the light, and may be more appropriate for highly flattened systems like disk galaxies.
         """
         return self.effective_radius / np.sqrt(self.axis_ratio)
 
 
 class Sersic(AbstractSersic, MassProfileMGE, MassProfileCSE):
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.grid_dec.to_vector_yx
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
-    def deflections_2d_via_integral_from(self, grid: aa.type.Grid2DLike):
+    def deflections_2d_via_integral_from(self, grid: aa.type.Grid2DLike, **kwargs):
         """
         Calculate the deflection angles at a given set of arc-second gridded coordinates.
 
         Parameters
         ----------
         grid
             The grid of (y,x) arc-second coordinates the deflection angles are computed on.
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/stellar/sersic_core.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/stellar/sersic_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,16 +55,16 @@
         )
 
         self.radius_break = radius_break
         self.intensity = intensity
         self.alpha = alpha
         self.gamma = gamma
 
-    def deflections_yx_2d_from(self, grid: aa.type.Grid2DLike):
-        return self.deflections_2d_via_mge_from(grid=grid)
+    def deflections_yx_2d_from(self, grid: aa.type.Grid2DLike, **kwargs):
+        return self.deflections_2d_via_mge_from(grid=grid, **kwargs)
 
     def image_2d_via_radii_from(self, grid_radii: np.ndarray):
         """
         Calculate the intensity of the cored-Sersic light profile on a grid of radial coordinates.
 
         Parameters
         ----------
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/stellar/sersic_radial_gradient.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/stellar/sersic_radial_gradient.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,18 +46,18 @@
             intensity=intensity,
             effective_radius=effective_radius,
             sersic_index=sersic_index,
             mass_to_light_ratio=mass_to_light_ratio,
         )
         self.mass_to_light_gradient = mass_to_light_gradient
 
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.grid_dec.to_vector_yx
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
-    def deflections_2d_via_integral_from(self, grid: aa.type.Grid2DLike):
+    def deflections_2d_via_integral_from(self, grid: aa.type.Grid2DLike, **kwargs):
         """
         Calculate the deflection angles at a given set of arc-second gridded coordinates.
 
         Parameters
         ----------
         grid
             The grid of (y,x) arc-second coordinates the deflection angles are computed on.
@@ -119,27 +119,30 @@
             * np.exp(
                 -sersic_constant
                 * (((_eta_u / effective_radius) ** (1.0 / sersic_index)) - 1)
             )
             / ((1 - (1 - axis_ratio**2) * u) ** (npow + 0.5))
         )
 
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.over_sample
+    @aa.grid_dec.to_array
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
-    def convergence_2d_from(self, grid: aa.type.Grid2DLike):
+    def convergence_2d_from(self, grid: aa.type.Grid2DLike, **kwargs):
         """Calculate the projected convergence at a given set of arc-second gridded coordinates.
 
         Parameters
         ----------
         grid
             The grid of (y,x) arc-second coordinates the convergence is computed on.
 
         """
-        return self.convergence_func(self.eccentric_radii_grid_from(grid))
+        return self.convergence_func(
+            self.eccentric_radii_grid_from(grid=grid, **kwargs)
+        )
 
     def convergence_func(self, grid_radius: float) -> float:
         return (
             self.mass_to_light_ratio
             * (
                 ((self.axis_ratio * grid_radius) / self.effective_radius)
                 ** -self.mass_to_light_gradient
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/total/isothermal.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/total/isothermal.py`

 * *Files 7% similar despite different names*

```diff
@@ -69,19 +69,18 @@
         )
 
     @property
     def axis_ratio(self):
         axis_ratio = super().axis_ratio
         return min(axis_ratio, 0.99999)
 
-    @aa.grid_dec.grid_2d_to_vector_yx
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.grid_dec.to_vector_yx
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
-    def deflections_yx_2d_from(self, grid: aa.type.Grid2DLike):
+    def deflections_yx_2d_from(self, grid: aa.type.Grid2DLike, **kwargs):
         """
         Calculate the deflection angles on a grid of (y,x) arc-second coordinates.
 
         For coordinates (0.0, 0.0) the analytic calculation of the deflection angle gives a NaN. Therefore,
         coordinates at (0.0, 0.0) are shifted slightly to (1.0e-8, 1.0e-8).
 
         Parameters
@@ -102,21 +101,22 @@
         deflection_y = np.arctanh(
             np.divide(np.multiply(np.sqrt(1 - self.axis_ratio**2), grid[:, 0]), psi)
         )
         deflection_x = np.arctan(
             np.divide(np.multiply(np.sqrt(1 - self.axis_ratio**2), grid[:, 1]), psi)
         )
         return self.rotated_grid_from_reference_frame_from(
-            grid=np.multiply(factor, np.vstack((deflection_y, deflection_x)).T)
+            grid=np.multiply(factor, np.vstack((deflection_y, deflection_x)).T),
+            **kwargs
         )
 
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.grid_dec.to_vector_yx
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
-    def shear_yx_2d_from(self, grid: aa.type.Grid2DLike):
+    def shear_yx_2d_from(self, grid: aa.type.Grid2DLike, **kwargs):
         """
         Calculate the (gamma_y, gamma_x) shear vector field on a grid of (y,x) arc-second coordinates.
 
         The result is returned as a `ShearYX2D` dats structure, which has shape [total_shear_vectors, 2], where
         entries for [:,0] are the gamma_2 values and entries for [:,1] are the gamma_1 values.
 
         Note therefore that this convention means the FIRST entries in the array are the gamma_2 values and the SECOND
@@ -125,15 +125,15 @@
         Parameters
         ----------
         grid
             The grid of (y,x) arc-second coordinates the deflection angles are computed on.
 
         """
 
-        convergence = self.convergence_2d_from(grid=grid)
+        convergence = self.convergence_2d_from(grid=grid, **kwargs)
 
         gamma_2 = (
             -2
             * convergence
             * np.divide(grid[:, 1] * grid[:, 0], grid[:, 1] ** 2 + grid[:, 0] ** 2)
         )
         gamma_1 = -convergence * np.divide(
@@ -166,39 +166,40 @@
             centre=centre, ell_comps=(0.0, 0.0), einstein_radius=einstein_radius
         )
 
     @property
     def axis_ratio(self):
         return 1.0
 
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.over_sample
+    @aa.grid_dec.to_array
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
-    def potential_2d_from(self, grid: aa.type.Grid2DLike):
+    def potential_2d_from(self, grid: aa.type.Grid2DLike, **kwargs):
         """
         Calculate the potential on a grid of (y,x) arc-second coordinates.
 
         Parameters
         ----------
         grid
             The grid of (y,x) arc-second coordinates the deflection angles are computed on.
         """
-        eta = self.elliptical_radii_grid_from(grid)
+        eta = self.elliptical_radii_grid_from(grid=grid, **kwargs)
         return 2.0 * self.einstein_radius_rescaled * eta
 
-    @aa.grid_dec.grid_2d_to_vector_yx
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.grid_dec.to_vector_yx
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
-    def deflections_yx_2d_from(self, grid: aa.type.Grid2DLike):
+    def deflections_yx_2d_from(self, grid: aa.type.Grid2DLike, **kwargs):
         """
         Calculate the deflection angles on a grid of (y,x) arc-second coordinates.
 
         Parameters
         ----------
         grid
             The grid of (y,x) arc-second coordinates the deflection angles are computed on.
         """
         return self._cartesian_grid_via_radial_from(
             grid=grid,
             radius=np.full(grid.shape[0], 2.0 * self.einstein_radius_rescaled),
+            **kwargs
         )
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/total/isothermal_core.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/total/isothermal_core.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/total/power_law.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/total/power_law.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,31 +34,30 @@
             centre=centre,
             ell_comps=ell_comps,
             einstein_radius=einstein_radius,
             slope=slope,
             core_radius=0.0,
         )
 
-    @aa.grid_dec.grid_2d_to_structure
-    def potential_2d_from(self, grid: aa.type.Grid2DLike):
-        alpha = self.deflections_yx_2d_from(grid)
+    @aa.grid_dec.to_array
+    def potential_2d_from(self, grid: aa.type.Grid2DLike, **kwargs):
+        alpha = self.deflections_yx_2d_from(aa.Grid2DIrregular(grid), **kwargs)
 
         alpha_x = alpha[:, 1]
         alpha_y = alpha[:, 0]
 
         x = grid[:, 1] - self.centre[1]
         y = grid[:, 0] - self.centre[0]
 
         return (x * alpha_x + y * alpha_y) / (3 - self.slope)
 
-    @aa.grid_dec.grid_2d_to_vector_yx
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.grid_dec.to_vector_yx
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
-    def deflections_yx_2d_from(self, grid: aa.type.Grid2DLike):
+    def deflections_yx_2d_from(self, grid: aa.type.Grid2DLike, **kwargs):
         """
         Calculate the deflection angles on a grid of (y,x) arc-second coordinates.
 
         For coordinates (0.0, 0.0) the analytic calculation of the deflection angle gives a NaN. Therefore,
         coordinates at (0.0, 0.0) are shifted slightly to (1.0e-8, 1.0e-8).
 
         This code is an adaption of Tessore & Metcalf 2015:
@@ -147,22 +146,21 @@
         super().__init__(
             centre=centre,
             ell_comps=(0.0, 0.0),
             einstein_radius=einstein_radius,
             slope=slope,
         )
 
-    @aa.grid_dec.grid_2d_to_vector_yx
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.grid_dec.to_vector_yx
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
-    def deflections_yx_2d_from(self, grid: aa.type.Grid2DLike):
-        eta = self.radial_grid_from(grid)
+    def deflections_yx_2d_from(self, grid: aa.type.Grid2DLike, **kwargs):
+        eta = self.radial_grid_from(grid=grid, **kwargs)
         deflection_r = (
             2.0
             * self.einstein_radius_rescaled
             * np.divide(
                 np.power(eta, (3.0 - self.slope)), np.multiply((3.0 - self.slope), eta)
             )
         )
 
-        return self._cartesian_grid_via_radial_from(grid, deflection_r)
+        return self._cartesian_grid_via_radial_from(grid=grid, radius=deflection_r)
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/total/power_law_broken.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/total/power_law_broken.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,18 +45,19 @@
             self.kB = (2 - self.inner_slope) / (
                 (2 * self.nu**2)
                 * (1 + self.dt * (self.nu ** (self.outer_slope - 2) - 1))
             )
         else:
             self.kB = (2 - self.inner_slope) / (2 * self.nu**2)
 
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.over_sample
+    @aa.grid_dec.to_array
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
-    def convergence_2d_from(self, grid: aa.type.Grid2DLike):
+    def convergence_2d_from(self, grid: aa.type.Grid2DLike, **kwargs):
         """
         Returns the dimensionless density kappa=Sigma/Sigma_c (eq. 1)
         """
 
         # Ell radius
         radius = np.hypot(grid[:, 1] * self.axis_ratio, grid[:, 0])
 
@@ -66,23 +67,22 @@
         # Outside break radius
         kappa_outer = self.kB * (self.break_radius / radius) ** self.outer_slope
 
         return kappa_inner * (radius <= self.break_radius) + kappa_outer * (
             radius > self.break_radius
         )
 
-    @aa.grid_dec.grid_2d_to_structure
-    def potential_2d_from(self, grid: aa.type.Grid2DLike):
+    @aa.grid_dec.to_array
+    def potential_2d_from(self, grid: aa.type.Grid2DLike, **kwargs):
         return np.zeros(shape=grid.shape[0])
 
-    @aa.grid_dec.grid_2d_to_vector_yx
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.grid_dec.to_vector_yx
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
-    def deflections_yx_2d_from(self, grid, max_terms=20):
+    def deflections_yx_2d_from(self, grid, max_terms=20, **kwargs):
         """
         Returns the complex deflection angle from eq. 18 and 19
         """
         # Rotate coordinates
         z = grid[:, 1] + 1j * grid[:, 0]
 
         # Ell radius
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/total/power_law_core.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/total/power_law_core.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,43 +45,45 @@
         Rescale the einstein radius by slope and axis_ratio, to reduce its degeneracy with other mass-profiles
         parameters.
         """
         return ((3 - self.slope) / (1 + self.axis_ratio)) * self.einstein_radius ** (
             self.slope - 1
         )
 
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.over_sample
+    @aa.grid_dec.to_array
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
-    def convergence_2d_from(self, grid: aa.type.Grid2DLike):
+    def convergence_2d_from(self, grid: aa.type.Grid2DLike, **kwargs):
         """
         Returns the two dimensional projected convergence on a grid of (y,x) arc-second coordinates.
 
         The `grid_2d_to_structure` decorator reshapes the ndarrays the convergence is outputted on. See
         *aa.grid_2d_to_structure* for a description of the output.
 
         Parameters
         ----------
         grid
             The grid of (y,x) arc-second coordinates the convergence is computed on.
         """
 
         covnergence_grid = np.zeros(grid.shape[0])
 
-        grid_eta = self.elliptical_radii_grid_from(grid)
+        grid_eta = self.elliptical_radii_grid_from(grid=grid, **kwargs)
 
         for i in range(grid.shape[0]):
             covnergence_grid[i] = self.convergence_func(grid_eta[i])
 
         return covnergence_grid
 
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.over_sample
+    @aa.grid_dec.to_array
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
-    def potential_2d_from(self, grid: aa.type.Grid2DLike):
+    def potential_2d_from(self, grid: aa.type.Grid2DLike, **kwargs):
         """
         Calculate the potential on a grid of (y,x) arc-second coordinates.
 
         Parameters
         ----------
         grid
             The grid of (y,x) arc-second coordinates the deflection angles are computed on.
@@ -101,19 +103,18 @@
                     self.slope,
                     self.core_radius,
                 ),
             )[0]
 
         return self.einstein_radius_rescaled * self.axis_ratio * potential_grid
 
-    @aa.grid_dec.grid_2d_to_vector_yx
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.grid_dec.to_vector_yx
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
-    def deflections_yx_2d_from(self, grid: aa.type.Grid2DLike):
+    def deflections_yx_2d_from(self, grid: aa.type.Grid2DLike, **kwargs):
         """
         Calculate the deflection angles on a grid of (y,x) arc-second coordinates.
 
         Parameters
         ----------
         grid
             The grid of (y,x) arc-second coordinates the deflection angles are computed on.
@@ -212,29 +213,28 @@
             centre=centre,
             ell_comps=(0.0, 0.0),
             einstein_radius=einstein_radius,
             slope=slope,
             core_radius=core_radius,
         )
 
-    @aa.grid_dec.grid_2d_to_vector_yx
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.grid_dec.to_vector_yx
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
-    def deflections_yx_2d_from(self, grid: aa.type.Grid2DLike):
+    def deflections_yx_2d_from(self, grid: aa.type.Grid2DLike, **kwargs):
         """
         Calculate the deflection angles on a grid of (y,x) arc-second coordinates.
 
         Parameters
         ----------
         grid
             The grid of (y,x) arc-second coordinates the deflection angles are computed on.
 
         """
-        eta = self.radial_grid_from(grid=grid)
+        eta = self.radial_grid_from(grid=grid, **kwargs)
         deflection = np.multiply(
             2.0 * self.einstein_radius_rescaled,
             np.divide(
                 np.add(
                     np.power(
                         np.add(self.core_radius**2, np.square(eta)),
                         (3.0 - self.slope) / 2.0,
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/mass/total/power_law_multipole.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/mass/total/power_law_multipole.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from astropy import units
 import numpy as np
 from typing import Tuple
 
 import autoarray as aa
 
+from autogalaxy import convert
+
 from autogalaxy.profiles.mass.abstract.abstract import MassProfile
 
 
 def radial_and_angle_grid_from(
     grid: aa.type.Grid2DLike, centre: Tuple[float, float] = (0.0, 0.0)
 ) -> Tuple[np.ndarray, np.ndarray]:
     """
@@ -32,74 +34,14 @@
     radial_grid = np.sqrt(x_shifted**2 + y_shifted**2)
 
     angle_grid = np.arctan2(y_shifted, x_shifted)
 
     return radial_grid, angle_grid
 
 
-def multipole_parameters_from(
-    multipole_comps: Tuple[float, float], m: int
-) -> Tuple[float, float]:
-    """
-    Converts the multipole component parameters to their normalizartion value `k_m` and angle `phi`,
-    which are given by:
-
-    .. math::
-        \phi^{\rm mass}_m = \arctan{\frac{\epsilon_{\rm 2}^{\rm mp}}{\epsilon_{\rm 2}^{\rm mp}}}, \, \,
-        k^{\rm mass}_m = \sqrt{{\epsilon_{\rm 1}^{\rm mp}}^2 + {\epsilon_{\rm 2}^{\rm mp}}^2} \, .
-
-    The conversion depends on the multipole order `m`, to ensure that all possible rotationally symmetric
-    multiple mass profiles are available in the conversion for multiple components spanning -inf to inf.
-
-    Parameters
-    ----------
-    multipole_comps
-        The first and second components of the multipole.
-
-    Returns
-    -------
-    The normalization and angle parameters of the multipole.
-    """
-    phi_m = (
-        np.arctan2(multipole_comps[0], multipole_comps[1]) * 180.0 / np.pi / float(m)
-    )
-    k_m = np.sqrt(multipole_comps[1] ** 2 + multipole_comps[0] ** 2)
-
-    return k_m, phi_m
-
-
-def multipole_comps_from(k_m: float, phi_m: float, m: int) -> Tuple[float, float]:
-    """
-    Converts the multipole normalizartion value `k_m` and angle `phi` to their multipole component parameters,
-    which are given by:
-
-    .. math::
-        \phi^{\rm mass}_m = \arctan{\frac{\epsilon_{\rm 2}^{\rm mp}}{\epsilon_{\rm 2}^{\rm mp}}}, \, \,
-        k^{\rm mass}_m = \sqrt{{\epsilon_{\rm 1}^{\rm mp}}^2 + {\epsilon_{\rm 2}^{\rm mp}}^2} \, .
-
-    The conversion depends on the multipole order `m`, to ensure that all possible rotationally symmetric
-    multiple mass profiles are available in the conversion for multiple components spanning -inf to inf.
-
-    Parameters
-    ----------
-    k_m
-        The magnitude of the multipole.
-    phi_m
-        The angle of the multipole.
-
-    Returns
-    -------
-    The multipole component parameters.
-    """
-    multipole_comp_0 = k_m * np.sin(phi_m * float(m) * units.deg.to(units.rad))
-    multipole_comp_1 = k_m * np.cos(phi_m * float(m) * units.deg.to(units.rad))
-
-    return (multipole_comp_0, multipole_comp_1)
-
-
 class PowerLawMultipole(MassProfile):
     def __init__(
         self,
         m=4,
         centre: Tuple[float, float] = (0.0, 0.0),
         einstein_radius: float = 1.0,
         slope: float = 2.0,
@@ -175,15 +117,15 @@
 
         self.m = int(m)
 
         self.einstein_radius = einstein_radius
         self.slope = slope
 
         self.multipole_comps = multipole_comps
-        self.k_m, self.angle_m = multipole_parameters_from(
+        self.k_m, self.angle_m = convert.multipole_k_m_and_phi_m_from(
             multipole_comps=multipole_comps, m=m
         )
         self.angle_m *= units.deg.to(units.rad)
 
     def jacobian(
         self, a_r: np.ndarray, a_angle: np.ndarray, polar_angle_grid: np.ndarray
     ) -> Tuple[np.ndarray, Tuple]:
@@ -200,19 +142,20 @@
             The polar angle coordinates of the input (y,x) Cartesian grid of coordinates.
         """
         return (
             a_r * np.sin(polar_angle_grid) + a_angle * np.cos(polar_angle_grid),
             a_r * np.cos(polar_angle_grid) - a_angle * np.sin(polar_angle_grid),
         )
 
-    @aa.grid_dec.grid_2d_to_vector_yx
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.grid_dec.to_vector_yx
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
-    def deflections_yx_2d_from(self, grid: aa.type.Grid1D2DLike) -> np.ndarray:
+    def deflections_yx_2d_from(
+        self, grid: aa.type.Grid1D2DLike, **kwargs
+    ) -> np.ndarray:
         """
         Calculate the deflection angles on a grid of (y,x) arc-second coordinates.
 
         For coordinates (0.0, 0.0) the analytic calculation of the deflection angle gives a NaN. Therefore,
         coordinates at (0.0, 0.0) are shifted slightly to (1.0e-8, 1.0e-8).
 
         Parameters
@@ -245,18 +188,19 @@
         )
 
         return np.stack(
             self.jacobian(a_r=a_r, a_angle=a_angle, polar_angle_grid=polar_angle_grid),
             axis=-1,
         )
 
-    @aa.grid_dec.grid_2d_to_structure
+    @aa.over_sample
+    @aa.grid_dec.to_array
     @aa.grid_dec.transform
     @aa.grid_dec.relocate_to_radial_minimum
-    def convergence_2d_from(self, grid: aa.type.Grid1D2DLike) -> np.ndarray:
+    def convergence_2d_from(self, grid: aa.type.Grid1D2DLike, **kwargs) -> np.ndarray:
         """
         Returns the two dimensional projected convergence on a grid of (y,x) arc-second coordinates.
 
         Parameters
         ----------
         grid
             The grid of (y,x) arc-second coordinates the convergence is computed on.
@@ -267,16 +211,16 @@
             1.0
             / 2.0
             * (self.einstein_radius / r) ** (self.slope - 1)
             * self.k_m
             * np.cos(self.m * (angle - self.angle_m))
         )
 
-    @aa.grid_dec.grid_2d_to_structure
-    def potential_2d_from(self, grid: aa.type.Grid2DLike) -> np.ndarray:
+    @aa.grid_dec.to_array
+    def potential_2d_from(self, grid: aa.type.Grid2DLike, **kwargs) -> np.ndarray:
         """
         Calculate the potential on a grid of (y,x) arc-second coordinates.
 
         Parameters
         ----------
         grid
             The grid of (y,x) arc-second coordinates the deflection angles are computed on.
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/plot/light_profile_plotters.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/plot/light_profile_plotters.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/plot/mass_profile_plotters.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/plot/mass_profile_plotters.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/profiles/scaling_relations.py` & `autogalaxy-2024.5.16.0/autogalaxy/profiles/scaling_relations.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/quantity/dataset_quantity.py` & `autogalaxy-2024.5.16.0/autogalaxy/quantity/dataset_quantity.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,176 +1,161 @@
 import logging
 import numpy as np
 from pathlib import Path
 from typing import List, Optional, Union
 
 import autoarray as aa
-from autoarray.dataset.abstract.settings import AbstractSettingsDataset
 from autoarray.dataset.abstract.dataset import AbstractDataset
 
 logger = logging.getLogger(__name__)
 
 
-class SettingsQuantity(AbstractSettingsDataset):
-    def __init__(
-        self,
-        grid_class=aa.Grid2D,
-        sub_size: int = 1,
-        fractional_accuracy: float = 0.9999,
-        relative_accuracy: Optional[float] = None,
-        sub_steps: List[int] = None,
-    ):
-        """
-        The lens dataset is the collection of data_type (image, noise-map, PSF), a mask, grid, convolver
-        and other utilities that are used for modeling and fitting an image of a strong lens.
-
-        Whilst the image, noise-map, etc. are loaded in 2D, the lens dataset creates reduced 1D arrays of each
-        for lens calculations.
-
-        Parameters
-        ----------
-        grid_class : ag.Grid2D
-            The type of grid used to create the image from the `Galaxy` and `Plane`. The options are `Grid2D`,
-            and `Grid2DIterate` (see the `Grid2D` documentation for a description of these options).
-        grid_pixelization_class : ag.Grid2D
-            The type of grid used to create the grid that maps the `LEq` source pixels to the data's image-pixels.
-            The options are `Grid2D` and `Grid2DIterate`.
-            (see the `Grid2D` documentation for a description of these options).
-        sub_size
-            If the grid and / or grid_pixelization use a `Grid2D`, this sets the sub-size used by the `Grid2D`.
-        fractional_accuracy
-            If the grid and / or grid_pixelization use a `Grid2DIterate`, this sets the fractional accuracy it
-            uses when evaluating functions, where the fraction accuracy is the ratio of the values computed using
-            two grids at a higher and lower sub-grid size.
-        relative_accuracy
-            If the grid and / or grid_pixelization use a `Grid2DIterate`, this sets the relative accuracy it
-            uses when evaluating functions, where the relative accuracy is the absolute difference of the values
-            computed using two grids at a higher and lower sub-grid size.
-        sub_steps : [int]
-            If the grid and / or grid_pixelization use a `Grid2DIterate`, this sets the steps the sub-size is increased by
-            to meet the fractional accuracy when evaluating functions.
-        psf_shape_2d
-            The shape of the PSF used for convolving model image generated using analytic light profiles. A smaller
-            shape will trim the PSF relative to the input image PSF, giving a faster analysis run-time.
-        """
-
-        super().__init__(
-            grid_class=grid_class,
-            sub_size=sub_size,
-            fractional_accuracy=fractional_accuracy,
-            relative_accuracy=relative_accuracy,
-            sub_steps=sub_steps,
-        )
-
-
 class DatasetQuantity(AbstractDataset):
     def __init__(
         self,
         data: Union[aa.Array2D, aa.VectorYX2D],
         noise_map: Union[aa.Array2D, aa.VectorYX2D],
-        settings: SettingsQuantity = SettingsQuantity(),
+        over_sampling: Optional[aa.OverSamplingIterate] = None,
     ):
         """
-        Represents a derived quantity of a light profile, mass profile, galaxy or plane as a dataset that can be fitted
-        with a model via a non-linear.
+        A quantity dataset, which represents a derived quantity of a light profile, mass profile, galaxy or galaxies
+        that can be fitted with a model via a non-linear.
 
         For example, the `DatasetQuantity` could represent the `convergence` of a mass profile, and this dataset could
-        then be fit with a `plane` via the `AnalysisQuantity` class. The benefit of doing this is that the components
+        then be fit with a galaxies via the `AnalysisQuantity` class. The benefit of doing this is that the components
         of different models can be fitted to one another and matched for example, the power-law model whose convergence
         best matches the convergence of a dark matter profile could be inferred).
 
+        The following quantities of the data are available and used for the following tasks:
+
+        - `data`: The quantity data, which shows the signal that is analysed and fitted with a model data of a model
+        object.
+
+        - `noise_map`: The RMS standard deviation error in every pixel, which is used to compute the chi-squared value
+        and likelihood of a fit.
+
+        Datasets also contains following properties:
+
+        - `grid`: A grids of (y,x) coordinates which align with the image pixels, whereby each coordinate corresponds to
+        the centre of an image pixel. This may be used in fits to calculate the model image of the imaging data.
+
+        - `grid_pixelization`: A grid of (y,x) coordinates which align with the pixels of a pixelization. This grid
+        is specifically used for pixelizations computed via the `invserion` module, which often use different
+        oversampling and sub-size values to the grid above.
+
+        The `over_sampling` and `over_sampling_pixelization` define how over sampling is performed for these grids.
+
+        This is used in the project PyAutoGalaxy to load imaging data of a galaxy and fit it with galaxy light profiles.
+        It is used in PyAutoLens to load imaging data of a strong lens and fit it with a lens model.
+
         Parameters
         ----------
         data
             The data of the quantity (e.g. 2D convergence, 2D potential, 2D deflections) that is fitted.
         noise_map
-            The 2D noise map of the quantity's data, which is often chosen in an arbitrary way.
-        settings
-            Controls settings of how the dataset is set up (e.g. the types of grids used to perform calculations).
+            The 2D noise map of the quantity's data.
+        noise_map
+            An array describing the RMS standard deviation error in each pixel used for computing quantities like the
+            chi-squared in a fit, which is often chosen in an arbitrary way for a quantity dataset given the quantities
+            are not observed using real astronomical instruments.
+        over_sampling
+            How over sampling is performed for the grid which performs calculations not associated with a pixelization.
+            In PyAutoGalaxy and PyAutoLens this is light profile calculations.
+        over_sampling_pixelization
+            How over sampling is performed for the grid which is associated with a pixelization, which is therefore
+            passed into the calculations performed in the `inversion` module.
         """
-
         if data.shape != noise_map.shape:
             if data.shape[0:-1] == noise_map.shape[0:]:
                 noise_map = aa.VectorYX2D.no_mask(
                     values=np.stack((noise_map, noise_map), axis=-1),
                     pixel_scales=data.pixel_scales,
                     shape_native=data.shape_native,
-                    sub_size=data.sub_size,
                     origin=data.origin,
                 )
 
         self.unmasked = None
 
-        super().__init__(data=data, noise_map=noise_map, settings=settings)
+        super().__init__(
+            data=data,
+            noise_map=noise_map,
+            over_sampling=over_sampling,
+        )
 
     @classmethod
     def via_signal_to_noise_map(
         cls,
         data: Union[aa.Array2D, aa.VectorYX2D],
         signal_to_noise_map: Union[aa.Array2D],
-        settings: SettingsQuantity = SettingsQuantity(),
+        over_sampling: Optional[aa.OverSamplingIterate] = None,
     ):
         """
-        Represents a derived quantity of a light profile, mass profile, galaxy or plane as a dataset that can be fitted
-        with a model via a non-linear (see `DatasetQuantity.__init__`).
+        Represents a derived quantity of a light profile, mass profile, galaxy or galaxies as a dataset that can be
+        fitted with a model via a non-linear (see `DatasetQuantity.__init__`).
 
         This classmethod takes as input a signal-to-noise map, as opposed to the noise map used in the `__init__`
         constructor. The noise-map is then derived from this signal-to-noise map, such that this is the signal to
         noise of the `DatasetQuantity` that is returned.
 
         Parameters
         ----------
         data
             The data of the quantity (e.g. 2D convergence, 2D potential, 2D deflections) that is fitted.
         signal_to_noise_map
             The 2D signal to noise map of the quantity's data.
-        settings
-            Controls settings of how the dataset is set up (e.g. the types of grids used to perform calculations).
         """
         try:
             noise_map = data / signal_to_noise_map
         except ValueError:
             noise_map = aa.VectorYX2D.zeros(
                 shape_native=data.shape_native, pixel_scales=data.pixel_scales
             )
             noise_map = noise_map.apply_mask(mask=data.mask)
 
             signal_to_noise_map[signal_to_noise_map < 1e-8] = 1e-8
 
             noise_map[:, 0] = np.abs(data.slim[:, 0]) / signal_to_noise_map
             noise_map[:, 1] = np.abs(data.slim[:, 1]) / signal_to_noise_map
 
-        return DatasetQuantity(data=data, noise_map=noise_map, settings=settings)
+        return DatasetQuantity(
+            data=data,
+            noise_map=noise_map,
+            over_sampling=over_sampling,
+        )
 
     @property
     def y(self) -> "DatasetQuantity":
         """
         If the `DatasetQuantity` contains a `VectorYX2D` as its data, this property returns a new `DatasetQuantity`
         with just the y-values of the vectors as the data, alongside the noise-map.
 
         This is primarily used for visualizing a fit to the `DatasetQuantity` containing vectors, as it allows one to
         reuse tools which visualize `Array2D` objects.
         """
         if isinstance(self.data, aa.VectorYX2D):
             return DatasetQuantity(
-                data=self.data.y, noise_map=self.noise_map.y, settings=self.settings
+                data=self.data.y,
+                noise_map=self.noise_map.y,
+                over_sampling=self.over_sampling,
             )
 
     @property
     def x(self) -> "DatasetQuantity":
         """
         If the `DatasetQuantity` contains a `VectorYX2D` as its data, this property returns a new `DatasetQuantity`
         with just the x-values of the vectors as the data, alongside the noise-map.
 
         This is primarily used for visualizing a fit to the `DatasetQuantity` containing vectors, as it allows one to
         reuse tools which visualize `Array2D` objects.
         """
         if isinstance(self.data, aa.VectorYX2D):
             return DatasetQuantity(
-                data=self.data.x, noise_map=self.noise_map.x, settings=self.settings
+                data=self.data.x,
+                noise_map=self.noise_map.x,
+                over_sampling=self.over_sampling,
             )
 
     def apply_mask(self, mask: aa.Mask2D) -> "DatasetQuantity":
         """
         Apply a mask to the quantity dataset, whereby the mask is applied to the data and noise-map one-by-one.
 
         The original unmasked qunatity dataset is stored as the `self.unmasked` attribute. This is used to ensure that
@@ -183,45 +168,31 @@
             The 2D mask that is applied to the image.
         """
         if self.data.mask.is_all_false:
             unmasked_dataset = self
         else:
             unmasked_dataset = self.unmasked
 
-        data = self.data.apply_mask(mask=mask.derive_mask.sub_1)
-        noise_map = self.noise_map.apply_mask(mask=mask.derive_mask.sub_1)
+        data = self.data.apply_mask(mask=mask)
+        noise_map = self.noise_map.apply_mask(mask=mask)
 
         dataset = DatasetQuantity(
-            data=data, noise_map=noise_map, settings=self.settings
+            data=data,
+            noise_map=noise_map,
+            over_sampling=self.over_sampling,
         )
 
         dataset.unmasked = unmasked_dataset
 
         logger.info(
             f"IMAGING - Data masked, contains a total of {mask.pixels_in_mask} image-pixels"
         )
 
         return dataset
 
-    def apply_settings(self, settings: SettingsQuantity) -> "DatasetQuantity":
-        """
-        Returns a new instance of the quantity dataset with the input `SettingsQuantity` applied to them.
-
-        This can be used to update settings like the types of grids associated with the dataset that are used
-        to perform calculations.
-
-        Parameters
-        ----------
-        settings
-            The settings for the quantity dataset which control things like the grids used for calculations.
-        """
-        return DatasetQuantity(
-            data=self.data, noise_map=self.noise_map, settings=settings
-        )
-
     @property
     def shape_native(self):
         return self.data.shape_native
 
     @property
     def pixel_scales(self):
         return self.data.pixel_scales
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/quantity/fit_quantity.py` & `autogalaxy-2024.5.16.0/autogalaxy/quantity/fit_quantity.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from typing import Optional, Union
+from typing import List, Optional, Union
 
 import autoarray as aa
 
 from autogalaxy.quantity.dataset_quantity import DatasetQuantity
 from autogalaxy.profiles.light.abstract import LightProfile
 from autogalaxy.profiles.mass.abstract.abstract import MassProfile
 from autogalaxy.galaxy.galaxy import Galaxy
-from autogalaxy.plane.plane import Plane
+from autogalaxy.galaxy.galaxies import Galaxies
 
 
 class FitQuantity(aa.FitImaging):
     def __init__(
         self,
         dataset: DatasetQuantity,
-        light_mass_obj: Union[LightProfile, MassProfile, Galaxy, Plane],
+        light_mass_obj: Union[LightProfile, MassProfile, Galaxy, Galaxies],
         func_str: str,
         model_data_manual: Optional[Union[aa.Array2D, aa.VectorYX2D]] = None,
     ):
         """
         Fits a `DatasetQuantity` object with model data.
 
         This is used to fit a quantity (e.g. a convergence, deflection angles), from an object like
-        a `LightProfile`, `MassProfile`, `Galaxy` or `Plane`, to the same quantity derived from another of that object.
+        a `LightProfile`, `MassProfile`, `Galaxy`, to the same quantity derived from another of that object.
 
         For example, we may have the 2D convergence of a power-law mass profile and wish to determine how closely the
         2D convergence of an nfw mass profile's matches it. The `FitQuantity` can fit the two, where a noise-map
         is associated with the quantity's dataset such that figure of merits like a chi-squared and log likelihood
         can be computed.
 
         This is ultimately used in the `AnalysisQuantity` class to perform model-fitting of quantities of different
@@ -33,18 +33,18 @@
 
         Parameters
         ----------
         dataset
             The quantity that is to be fitted, which has a noise-map associated it with for computing goodness-of-fit
             metrics.
         light_mass_obj
-            An object containing functions which computes a light and / or mass quantity (e.g. a plane of galaxies)
+            An object containing functions which computes a light and / or mass quantity (e.g. galaxies)
             whose model quantities are used to fit the quantity data.
         func_str
-            A string giving the name of the method of the input `Plane` used to compute the quantity that fits
+            A string giving the name of the method of the input galaxy used to compute the quantity that fits
             the dataset.
         model_data_manual
             Manually pass the model-data, omitting its calculation via the function defined by the `func_str`.
         """
 
         self.light_mass_obj = light_mass_obj
         self.func_str = func_str
@@ -52,15 +52,15 @@
 
         super().__init__(dataset=dataset, use_mask_in_fit=False)
 
     @property
     def model_data(self):
         if self.model_data_manual is None:
             func = getattr(self.light_mass_obj, self.func_str)
-            return func(grid=self.dataset.grid)
+            return func(grid=self.grid)
 
         return self.model_data_manual
 
     @property
     def y(self) -> "FitQuantity":
         """
         If the `FitQuantity` contains a `VectorYX2D` as its data, this property returns a new `FitQuantity`
@@ -93,25 +93,17 @@
                 dataset=self.dataset.x,
                 light_mass_obj=self.light_mass_obj,
                 func_str=self.func_str,
                 model_data_manual=self.model_data.x,
             )
 
     @property
-    def quantity_dataset(self):
-        return self.dataset
-
-    @property
     def mask(self):
         return self.dataset.mask
 
     @property
     def inversion(self):
         return None
 
     @property
-    def grid(self):
-        return self.quantity_dataset.grid
-
-    @property
-    def plane(self):
+    def galaxies(self):
         return self.light_mass_obj
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/quantity/model/analysis.py` & `autogalaxy-2024.5.16.0/autogalaxy/quantity/model/analysis.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-import os
-
 from autoconf.dictable import to_dict
 
 import autofit as af
 
-from autogalaxy.analysis.analysis import Analysis
+from autogalaxy.analysis.analysis.analysis import Analysis
 from autogalaxy.cosmology.lensing import LensingCosmology
 from autogalaxy.cosmology.wrap import Planck15
-from autogalaxy.quantity.model.visualizer import VisualizerQuantity
 from autogalaxy.quantity.dataset_quantity import DatasetQuantity
 from autogalaxy.quantity.model.result import ResultQuantity
+from autogalaxy.quantity.model.visualizer import VisualizerQuantity
 from autogalaxy.quantity.fit_quantity import FitQuantity
 
 from autogalaxy import exc
 
 
 class AnalysisQuantity(Analysis):
+    Result = ResultQuantity
+    Visualizer = VisualizerQuantity
+
     def __init__(
         self,
         dataset: DatasetQuantity,
         func_str: str,
         cosmology: LensingCosmology = Planck15(),
     ):
         """
@@ -31,27 +32,27 @@
         It handles many other tasks, such as visualization, outputting results to hard-disk and storing results in
         a format that can be loaded after the model-fit is complete.
 
         This class is used for model-fits which fit derived quantity of galaxies, for example their
         convergence, potential or deflection angles, to another model for that quantity. For example, one could find
         the `PowerLaw` mass profile model that best fits the deflection angles of an `NFW` mass profile.
 
-        The `func_str` input defines what quantity is fitted, it corresponds to the function of the model `Plane`
+        The `func_str` input defines what quantity is fitted, it corresponds to the function of the model galaxy
         objects that is called to create the model quantity. For example, if `func_str="convergence_2d_from"`, the
-        convergence is computed from each model `Plane`.
+        convergence is computed from each model galaxy.
 
         This class stores the settings used to perform the model-fit for certain components of the model (e.g. the
         Cosmology used for the analysis).
 
         Parameters
         ----------
         dataset
             The `DatasetQuantity` dataset that the model is fitted too.
         func_str
-            A string giving the name of the method of the input `Plane` used to compute the quantity that fits
+            A string giving the name of the method of the input galaxy used to compute the quantity that fits
             the dataset.
         cosmology
             The Cosmology assumed for this analysis.
         """
         super().__init__(cosmology=cosmology)
 
         self.dataset = dataset
@@ -107,97 +108,23 @@
         instance
             An instance of the model that is being fitted to the data by this analysis (whose parameters have been set
             via a non-linear search).
 
         Returns
         -------
         FitQuantity
-            The fit of the plane to the imaging dataset, which includes the log likelihood.
+            The fit of the galaxies to the imaging dataset, which includes the log likelihood.
         """
 
-        plane = self.plane_via_instance_from(instance=instance)
+        galaxies = self.galaxies_via_instance_from(instance=instance)
 
         return FitQuantity(
-            dataset=self.dataset, light_mass_obj=plane, func_str=self.func_str
+            dataset=self.dataset, light_mass_obj=galaxies, func_str=self.func_str
         )
 
-    def visualize(
-        self,
-        paths: af.DirectoryPaths,
-        instance: af.ModelInstance,
-        during_analysis: bool,
-    ):
-        """
-        Output images of the maximum log likelihood model inferred by the model-fit. This function is called throughout
-        the non-linear search at regular intervals, and therefore provides on-the-fly visualization of how well the
-        model-fit is going.
-
-        The visualization performed by this function includes:
-
-        - Images of the best-fit `Plane`, including the images of each of its galaxies.
-
-        - Images of the best-fit `FitQuantity`, including the model-image, residuals and chi-squared of its fit to
-        the imaging data.
-
-        The images output by this function are customized using the file `config/visualize/plots.ini`.
-
-        Parameters
-        ----------
-        paths
-            The PyAutoFit paths object which manages all paths, e.g. where the non-linear search outputs are stored,
-            visualization, and the pickled objects used by the aggregator output by this function.
-        instance
-            An instance of the model that is being fitted to the data by this analysis (whose parameters have been set
-            via a non-linear search).
-        during_analysis
-            If True the visualization is being performed midway through the non-linear search before it is finished,
-            which may change which images are output.
-        """
-
-        if os.environ.get("PYAUTOFIT_TEST_MODE") == "1":
-            return
-
-        fit = self.fit_quantity_for_instance(instance=instance)
-
-        visualizer = VisualizerQuantity(visualize_path=paths.image_path)
-        visualizer.visualize_fit_quantity(fit=fit)
-
-    def make_result(
-        self,
-        samples: af.SamplesPDF,
-    ) -> ResultQuantity:
-        """
-        After the non-linear search is complete create its `ResultQuantity`, which includes:
-
-        - The samples of the non-linear search (E.g. MCMC chains, nested sampling samples) which are used to compute
-        the maximum likelihood model, posteriors and other properties.
-
-        - The model used to fit the data, which uses the samples to create specific instances of the model (e.g.
-        an instance of the maximum log likelihood model).
-
-        - The non-linear search used to perform the model fit.
-
-        The `ResultQuantity` object contains a number of methods which use the above objects to create the max
-        log likelihood `Plane`, `FitQuantity`,etc.
-
-        Parameters
-        ----------
-        samples
-            A PyAutoFit object which contains the samples of the non-linear search, for example the chains of an MCMC
-            run of samples of the nested sampler.
-        search
-            The non-linear search used to perform this model-fit.
-
-        Returns
-        -------
-        ResultQuantity
-            The result of fitting the model to the imaging dataset, via a non-linear search.
-        """
-        return ResultQuantity(samples=samples, analysis=self)
-
     def save_attributes(self, paths: af.DirectoryPaths):
         """
         Before the non-linear search begins, this routine saves attributes of the `Analysis` object to the `pickles`
         folder such that they can be loaded after the analysis using PyAutoFit's database and aggregator tools.
 
         For this analysis, it uses the `AnalysisDataset` object's method to output the following:
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/quantity/model/visualizer.py` & `autogalaxy-2024.5.16.0/autogalaxy/quantity/model/plotter_interface.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from autogalaxy.quantity.fit_quantity import FitQuantity
 from autogalaxy.quantity.plot.fit_quantity_plotters import FitQuantityPlotter
-from autogalaxy.analysis.visualizer import Visualizer
-from autogalaxy.analysis.visualizer import plot_setting
+from autogalaxy.analysis.plotter_interface import PlotterInterface
+from autogalaxy.analysis.plotter_interface import plot_setting
 from autogalaxy.plot.visuals.two_d import Visuals2D
 
 
-class VisualizerQuantity(Visualizer):
-    def visualize_fit_quantity(
+class PlotterInterfaceQuantity(PlotterInterface):
+    def fit_quantity(
         self,
         fit: FitQuantity,
         visuals_2d: Visuals2D = Visuals2D(),
         fit_quanaity_plotter_cls=FitQuantityPlotter,
     ):
         """
         Visualizes a `FitQuantity` object, which fits a quantity of a light or mass profile (e.g. an image, potential)
         to the same quantity of another light or mass profile.
 
-        Images are output to the `image` folder of the `visualize_path` in a subfolder called `fit_quantity`. When
-        used with a non-linear search the `visualize_path` points to the search's results folder and this function
+        Images are output to the `image` folder of the `image_path` in a subfolder called `fit_quantity`. When
+        used with a non-linear search the `image_path` points to the search's results folder and this function
         visualizes the maximum log likelihood `FitQuantity` inferred by the search so far.
 
         Visualization includes individual images of attributes of the `FitQuantity` (e.g. the model data, residual map)
         and a subplot of all `FitQuantity`'s images on the same figure.
 
-        The images output by the `Visualizer` are customized using the file `config/visualize/plots.ini` under the
+        The images output by the `PlotterInterface` are customized using the file `config/visualize/plots.yaml` under the
         [fit_quantity] header.
 
         Parameters
         ----------
         fit
             The maximum log likelihood `FitQuantity` of the non-linear search which is used to plot the fit.
         visuals_2d
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/quantity/plot/fit_quantity_plotters.py` & `autogalaxy-2024.5.16.0/autogalaxy/quantity/plot/fit_quantity_plotters.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/util/__init__.py` & `autogalaxy-2024.5.16.0/autogalaxy/util/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,9 +17,8 @@
 from autoarray.inversion.inversion.interferometer import (
     inversion_interferometer_util as inversion_interferometer,
 )
 from autoarray.operators import transformer_util as transformer
 from autoarray.util import misc_util as misc
 
 from autogalaxy.util import error_util as error
-from autogalaxy.plane import plane_util as plane
 from autogalaxy.analysis import chaining_util as chaining
```

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/util/error_util.py` & `autogalaxy-2024.5.16.0/autogalaxy/util/error_util.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/util/mock/mock_cosmology.py` & `autogalaxy-2024.5.16.0/autogalaxy/util/mock/mock_cosmology.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/autogalaxy/util/shear_field.py` & `autogalaxy-2024.5.16.0/autogalaxy/util/shear_field.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2024.1.27.4/setup.py` & `autogalaxy-2024.5.16.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 this_dir = abspath(dirname(__file__))
 with open(join(this_dir, "README.rst"), encoding="utf-8") as file:
     long_description = file.read()
 
 with open(join(this_dir, "requirements.txt")) as f:
     requirements = f.read().split("\n")
 
-version = environ.get("VERSION", "1.0.dev0")
+version = environ.get("VERSION", "2024.5.16.0")
 requirements.extend(
     [f"autoconf=={version}", f"autoarray=={version}", f"autofit=={version}"]
 )
 
 
 def config_packages(directory):
     paths = [directory.replace("/", ".")]
```

