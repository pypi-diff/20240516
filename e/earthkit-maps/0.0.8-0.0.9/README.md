# Comparing `tmp/earthkit-maps-0.0.8.tar.gz` & `tmp/earthkit-maps-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "earthkit-maps-0.0.8.tar", last modified: Fri Sep  8 17:06:47 2023, max compression
+gzip compressed data, was "earthkit-maps-0.0.9.tar", last modified: Wed Nov  1 10:24:19 2023, max compression
```

## Comparing `earthkit-maps-0.0.8.tar` & `earthkit-maps-0.0.9.tar`

### file list

```diff
@@ -1,131 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:06:47.242819 earthkit-maps-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      611 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/.cruft.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:06:47.210819 earthkit-maps-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:06:47.218819 earthkit-maps-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     5846 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6961 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      146 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/.pre-commit-config-weekly.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      260 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11382 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/MANIFST.in
--rw-r--r--   0 runner    (1001) docker     (127)      808 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2023-09-08 17:06:47.242819 earthkit-maps-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:06:47.218819 earthkit-maps-0.0.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:06:47.218819 earthkit-maps-0.0.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    53944 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/docs/_static/earthkit-maps.png
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:06:47.222819 earthkit-maps-0.0.8/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)   412484 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/docs/examples/efi.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   274665 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/docs/examples/era5-el-nino.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   568129 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/docs/examples/fieldlist-input.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)  1348948 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/docs/examples/projected-coordinates.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   761592 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/docs/examples/scatter.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   546003 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/docs/examples/t850-z500.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      469 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:06:47.210819 earthkit-maps-0.0.8/earthkit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:06:47.226819 earthkit-maps-0.0.8/earthkit/maps/
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:06:47.226819 earthkit-maps-0.0.8/earthkit/maps/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:06:47.226819 earthkit-maps-0.0.8/earthkit/maps/data/colors/
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/data/colors/earthkit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/data/domains.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:06:47.226819 earthkit-maps-0.0.8/earthkit/maps/data/identities/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/data/identities/2m-temperature.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      143 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/data/identities/geopotential.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      155 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/data/identities/mean-sea-level-pressure.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/data/identities/river-discharge.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       91 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/data/identities/soil-loss.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:06:47.226819 earthkit-maps-0.0.8/earthkit/maps/data/logos/
--rw-r--r--   0 runner    (1001) docker     (127)    10365 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/data/logos/ecmwf.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:06:47.226819 earthkit-maps-0.0.8/earthkit/maps/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/data/schemas/default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/data/schemas/ecmwf.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:06:47.214819 earthkit-maps-0.0.8/earthkit/maps/data/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:06:47.214819 earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:06:47.230819 earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/Lato/
--rw-r--r--   0 runner    (1001) docker     (127)    69500 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/Lato/Lato-Black.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    72000 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/Lato/Lato-BlackItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    73332 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/Lato/Lato-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    77732 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/Lato/Lato-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    75792 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/Lato/Lato-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    77208 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/Lato/Lato-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    49080 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/Lato/Lato-LightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    75152 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/Lato/Lato-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    69976 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/Lato/Lato-Thin.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    48864 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/Lato/Lato-ThinItalic.ttf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:06:47.234819 earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/OpenSans/
--rw-r--r--   0 runner    (1001) docker     (127)     4482 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/OpenSans/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (127)   129784 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/OpenSans/OpenSans-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   135108 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/OpenSans/OpenSans-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   130180 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/OpenSans/OpenSans-ExtraBold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   135688 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/OpenSans/OpenSans-ExtraBoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   135380 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/OpenSans/OpenSans-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   129756 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/OpenSans/OpenSans-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   135668 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/OpenSans/OpenSans-LightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   129948 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/OpenSans/OpenSans-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   135556 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/OpenSans/OpenSans-MediumItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   129796 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/OpenSans/OpenSans-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   129716 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/OpenSans/OpenSans-SemiBold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   135512 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/OpenSans/OpenSans-SemiBoldItalic.ttf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:06:47.214819 earthkit-maps-0.0.8/earthkit/maps/data/static/images/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:06:47.234819 earthkit-maps-0.0.8/earthkit/maps/data/static/images/logos/
--rw-r--r--   0 runner    (1001) docker     (127)    10365 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/data/static/images/logos/ecmwf.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:06:47.214819 earthkit-maps-0.0.8/earthkit/maps/data/styles/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:06:47.238819 earthkit-maps-0.0.8/earthkit/maps/data/styles/default/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/data/styles/default/2m-temperature.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      212 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/data/styles/default/geopotential.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      164 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/data/styles/default/mean-sea-level-pressure.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      168 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/data/styles/default/river-discharge.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      113 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/data/styles/default/soil-loss.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:06:47.238819 earthkit-maps-0.0.8/earthkit/maps/data/styles/ecmwf/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/data/styles/ecmwf/2m-temperature.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/data/styles/ecmwf/geopotential.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/data.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:06:47.238819 earthkit-maps-0.0.8/earthkit/maps/domains/
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/domains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4162 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/domains/bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     4835 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/domains/crs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7965 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/domains/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/domains/natural_earth.py
--rw-r--r--   0 runner    (1001) docker     (127)     7820 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/domains/optimal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:06:47.238819 earthkit-maps-0.0.8/earthkit/maps/formats/
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/formats/units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:06:47.238819 earthkit-maps-0.0.8/earthkit/maps/layers/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3580 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/layers/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6422 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/layers/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    16975 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/layers/subplots.py
--rw-r--r--   0 runner    (1001) docker     (127)    14101 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/layers/superplots.py
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/layouts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/legends.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/logos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/quickplot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4695 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/shapes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:06:47.242819 earthkit-maps-0.0.8/earthkit/maps/styles/
--rw-r--r--   0 runner    (1001) docker     (127)    19560 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/styles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/styles/auto.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:06:47.242819 earthkit-maps-0.0.8/earthkit/maps/styles/ecmwf/
--rw-r--r--   0 runner    (1001) docker     (127)      888 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/styles/ecmwf/geopotential.py
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/styles/ecmwf/temperature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/styles/geopotential.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/styles/pressure.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/styles/river_discharge.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/styles/soil.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/styles/temperature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/earthkit/maps/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-09-08 17:06:47.000000 earthkit-maps-0.0.8/earthkit/maps/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:06:47.242819 earthkit-maps-0.0.8/earthkit_maps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2023-09-08 17:06:47.000000 earthkit-maps-0.0.8/earthkit_maps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3862 2023-09-08 17:06:47.000000 earthkit-maps-0.0.8/earthkit_maps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-08 17:06:47.000000 earthkit-maps-0.0.8/earthkit_maps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2023-09-08 17:06:47.000000 earthkit-maps-0.0.8/earthkit_maps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-09-08 17:06:47.000000 earthkit-maps-0.0.8/earthkit_maps.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      329 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      364 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2023-09-08 17:06:47.242819 earthkit-maps-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:06:47.242819 earthkit-maps-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2023-09-08 17:06:29.000000 earthkit-maps-0.0.8/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 10:24:19.521172 earthkit-maps-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/.cruft.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 10:24:19.493172 earthkit-maps-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 10:24:19.505172 earthkit-maps-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     5846 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     8827 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11382 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/MANIFST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2023-11-01 10:24:19.521172 earthkit-maps-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 10:24:19.505172 earthkit-maps-0.0.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 10:24:19.505172 earthkit-maps-0.0.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    53944 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/docs/_static/earthkit-maps.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 10:24:19.509172 earthkit-maps-0.0.9/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)   412484 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/docs/examples/efi.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   274665 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/docs/examples/era5-el-nino.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   568129 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/docs/examples/fieldlist-input.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  1348948 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/docs/examples/projected-coordinates.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   761592 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/docs/examples/scatter.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   546003 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/docs/examples/t850-z500.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 10:24:19.509172 earthkit-maps-0.0.9/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   230901 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/docs/images/quickplot-era5-t2m-20220901.png
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 10:24:19.497172 earthkit-maps-0.0.9/earthkit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 10:24:19.513172 earthkit-maps-0.0.9/earthkit/maps/
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 10:24:19.513172 earthkit-maps-0.0.9/earthkit/maps/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 10:24:19.513172 earthkit-maps-0.0.9/earthkit/maps/data/colors/
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/data/colors/earthkit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/data/domains.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 10:24:19.513172 earthkit-maps-0.0.9/earthkit/maps/data/identities/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/data/identities/2m-temperature.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/data/identities/geopotential.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/data/identities/mean-sea-level-pressure.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/data/identities/river-discharge.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/data/identities/soil-loss.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 10:24:19.513172 earthkit-maps-0.0.9/earthkit/maps/data/logos/
+-rw-r--r--   0 runner    (1001) docker     (127)    10365 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/data/logos/ecmwf.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 10:24:19.513172 earthkit-maps-0.0.9/earthkit/maps/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/data/schemas/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/data/schemas/ecmwf.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 10:24:19.501172 earthkit-maps-0.0.9/earthkit/maps/data/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 10:24:19.501172 earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 10:24:19.513172 earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/Lato/
+-rw-r--r--   0 runner    (1001) docker     (127)    69500 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/Lato/Lato-Black.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    72000 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/Lato/Lato-BlackItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    73332 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/Lato/Lato-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    77732 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/Lato/Lato-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    75792 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/Lato/Lato-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    77208 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/Lato/Lato-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    49080 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/Lato/Lato-LightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    75152 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/Lato/Lato-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    69976 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/Lato/Lato-Thin.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    48864 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/Lato/Lato-ThinItalic.ttf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 10:24:19.517172 earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/OpenSans/
+-rw-r--r--   0 runner    (1001) docker     (127)     4482 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/OpenSans/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   129784 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/OpenSans/OpenSans-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   135108 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/OpenSans/OpenSans-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   130180 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/OpenSans/OpenSans-ExtraBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   135688 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/OpenSans/OpenSans-ExtraBoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   135380 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/OpenSans/OpenSans-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   129756 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/OpenSans/OpenSans-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   135668 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/OpenSans/OpenSans-LightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   129948 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/OpenSans/OpenSans-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   135556 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/OpenSans/OpenSans-MediumItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   129796 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/OpenSans/OpenSans-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   129716 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/OpenSans/OpenSans-SemiBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   135512 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/OpenSans/OpenSans-SemiBoldItalic.ttf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 10:24:19.501172 earthkit-maps-0.0.9/earthkit/maps/data/static/images/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 10:24:19.517172 earthkit-maps-0.0.9/earthkit/maps/data/static/images/logos/
+-rw-r--r--   0 runner    (1001) docker     (127)    10365 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/data/static/images/logos/ecmwf.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 10:24:19.501172 earthkit-maps-0.0.9/earthkit/maps/data/styles/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 10:24:19.517172 earthkit-maps-0.0.9/earthkit/maps/data/styles/default/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/data/styles/default/2m-temperature.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/data/styles/default/geopotential.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/data/styles/default/mean-sea-level-pressure.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/data/styles/default/river-discharge.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/data/styles/default/soil-loss.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 10:24:19.517172 earthkit-maps-0.0.9/earthkit/maps/data/styles/ecmwf/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/data/styles/ecmwf/2m-temperature.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/data/styles/ecmwf/geopotential.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 10:24:19.521172 earthkit-maps-0.0.9/earthkit/maps/domains/
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/domains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4162 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/domains/bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4835 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/domains/crs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7967 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/domains/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/domains/natural_earth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7820 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/domains/optimal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 10:24:19.521172 earthkit-maps-0.0.9/earthkit/maps/formats/
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/formats/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 10:24:19.521172 earthkit-maps-0.0.9/earthkit/maps/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3580 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/layers/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6422 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/layers/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18203 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/layers/subplots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14147 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/layers/superplots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/layouts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/legends.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/logos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/quickplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4695 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/shapes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 10:24:19.521172 earthkit-maps-0.0.9/earthkit/maps/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)    20017 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/styles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/styles/anomalies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/styles/auto.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 10:24:19.521172 earthkit-maps-0.0.9/earthkit/maps/styles/ecmwf/
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/styles/ecmwf/geopotential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/styles/ecmwf/temperature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/styles/geopotential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/styles/pressure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/styles/river_discharge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/styles/soil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/styles/temperature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/earthkit/maps/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2023-11-01 10:24:19.000000 earthkit-maps-0.0.9/earthkit/maps/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 10:24:19.521172 earthkit-maps-0.0.9/earthkit_maps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2023-11-01 10:24:19.000000 earthkit-maps-0.0.9/earthkit_maps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2023-11-01 10:24:19.000000 earthkit-maps-0.0.9/earthkit_maps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-01 10:24:19.000000 earthkit-maps-0.0.9/earthkit_maps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2023-11-01 10:24:19.000000 earthkit-maps-0.0.9/earthkit_maps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-11-01 10:24:19.000000 earthkit-maps-0.0.9/earthkit_maps.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2023-11-01 10:24:19.521172 earthkit-maps-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 10:24:19.521172 earthkit-maps-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2023-11-01 10:24:02.000000 earthkit-maps-0.0.9/tests/test_version.py
```

### Comparing `earthkit-maps-0.0.8/.cruft.json` & `earthkit-maps-0.0.9/.cruft.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.89375%*

 * *Differences: {"'commit'": "'baa719b04376f091dee7b3f221d3b62eb29d2f95'",*

 * * "'context'": "{'cookiecutter': {'integration_tests': False}}"}*

```diff
@@ -1,15 +1,16 @@
 {
     "checkout": null,
-    "commit": "c7cd369f71b4cfc647fc7c1972cc3c45860256d5",
+    "commit": "baa719b04376f091dee7b3f221d3b62eb29d2f95",
     "context": {
         "cookiecutter": {
             "_template": "https://github.com/ecmwf-projects/cookiecutter-conda-package",
             "copyright_holder": "European Centre for Medium Range Weather Forecasts",
             "copyright_year": "2023",
+            "integration_tests": false,
             "mypy_strict": "False",
             "project_name": "earthkit-maps",
             "project_short_description": "Geospatial visualisation tools and templates",
             "project_slug": "earthkit-maps"
         }
     },
     "directory": null,
```

### Comparing `earthkit-maps-0.0.8/.github/workflows/ci.yml` & `earthkit-maps-0.0.9/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/.gitignore` & `earthkit-maps-0.0.9/.gitignore`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,69 @@
 # setuptools-scm
 version.py
 
 # Sphinx automatic generation of API
 docs/_api/
 
-# Created by https://www.toptal.com/developers/gitignore/api/python,jupyternotebooks,vim,visualstudiocode,pycharm
-# Edit at https://www.toptal.com/developers/gitignore?templates=python,jupyternotebooks,vim,visualstudiocode,pycharm
+# Combined environments
+ci/combined-environment-*.yml
+
+# Created by https://www.toptal.com/developers/gitignore/api/python,jupyternotebooks,vim,visualstudiocode,pycharm,emacs,linux,macos,windows
+# Edit at https://www.toptal.com/developers/gitignore?templates=python,jupyternotebooks,vim,visualstudiocode,pycharm,emacs,linux,macos,windows
+
+### Emacs ###
+# -*- mode: gitignore; -*-
+*~
+\#*\#
+/.emacs.desktop
+/.emacs.desktop.lock
+*.elc
+auto-save-list
+tramp
+.\#*
+
+# Org-mode
+.org-id-locations
+*_archive
+
+# flymake-mode
+*_flymake.*
+
+# eshell files
+/eshell/history
+/eshell/lastdir
+
+# elpa packages
+/elpa/
+
+# reftex files
+*.rel
+
+# AUCTeX auto folder
+/auto/
+
+# cask packages
+.cask/
+dist/
+
+# Flycheck
+flycheck_*.el
+
+# server auth directory
+/server/
+
+# projectiles files
+.projectile
+
+# directory configuration
+.dir-locals.el
+
+# network security
+/network-security.data
+
 
 ### JupyterNotebooks ###
 # gitignore template for Jupyter Notebooks
 # website: http://jupyter.org/
 
 .ipynb_checkpoints
 */.ipynb_checkpoints/*
@@ -17,14 +71,60 @@
 # IPython
 profile_default/
 ipython_config.py
 
 # Remove previous ipynb_checkpoints
 #   git rm -r .ipynb_checkpoints/
 
+### Linux ###
+
+# temporary files which can be created if a process still has a handle open of a deleted file
+.fuse_hidden*
+
+# KDE directory preferences
+.directory
+
+# Linux trash folder which might appear on any partition or disk
+.Trash-*
+
+# .nfs files are created when an open file is removed but is still being accessed
+.nfs*
+
+### macOS ###
+# General
+.DS_Store
+.AppleDouble
+.LSOverride
+
+# Icon must end with two \r
+Icon
+
+# Thumbnails
+._*
+
+# Files that might appear in the root of a volume
+.DocumentRevisions-V100
+.fseventsd
+.Spotlight-V100
+.TemporaryItems
+.Trashes
+.VolumeIcon.icns
+.com.apple.timemachine.donotpresent
+
+# Directories potentially created on remote AFP share
+.AppleDB
+.AppleDesktop
+Network Trash Folder
+Temporary Items
+.apdisk
+
+### macOS Patch ###
+# iCloud generated files
+*.icloud
+
 ### PyCharm ###
 # Covers JetBrains IDEs: IntelliJ, RubyMine, PhpStorm, AppCode, PyCharm, CLion, Android Studio, WebStorm and Rider
 # Reference: https://intellij-support.jetbrains.com/hc/en-us/articles/206544839
 
 # User-specific stuff
 .idea/**/workspace.xml
 .idea/**/tasks.xml
@@ -143,15 +243,14 @@
 # C extensions
 *.so
 
 # Distribution / packaging
 .Python
 build/
 develop-eggs/
-dist/
 downloads/
 eggs/
 .eggs/
 lib/
 lib64/
 parts/
 sdist/
@@ -289,14 +388,24 @@
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 
+### Python Patch ###
+# Poetry local configuration file - https://python-poetry.org/docs/configuration/#local-configuration
+poetry.toml
+
+# ruff
+.ruff_cache/
+
+# LSP config files
+pyrightconfig.json
+
 ### Vim ###
 # Swap
 [._]*.s[a-v][a-z]
 !*.svg  # comment out if you don't need vector files
 [._]*.sw[a-p]
 [._]s[a-rt-v][a-z]
 [._]ss[a-gi-z]
@@ -304,22 +413,23 @@
 
 # Session
 Session.vim
 Sessionx.vim
 
 # Temporary
 .netrwhist
-*~
 # Auto-generated tag files
 tags
 # Persistent undo
 [._]*.un~
 
 ### VisualStudioCode ###
 .vscode/
+.DS_Store
+docs/.DS_Store
 # .vscode/*
 # !.vscode/settings.json
 # !.vscode/tasks.json
 # !.vscode/launch.json
 # !.vscode/extensions.json
 # !.vscode/*.code-snippets
 
@@ -330,14 +440,34 @@
 *.vsix
 
 ### VisualStudioCode Patch ###
 # Ignore all local history of files
 .history
 .ionide
 
-# Support for Project snippet scope
-.vscode/*.code-snippets
+### Windows ###
+# Windows thumbnail cache files
+Thumbs.db
+Thumbs.db:encryptable
+ehthumbs.db
+ehthumbs_vista.db
+
+# Dump file
+*.stackdump
+
+# Folder config file
+[Dd]esktop.ini
+
+# Recycle Bin used on file shares
+$RECYCLE.BIN/
+
+# Windows Installer files
+*.cab
+*.msi
+*.msix
+*.msm
+*.msp
 
-# Ignore code-workspaces
-*.code-workspace
+# Windows shortcuts
+*.lnk
 
-# End of https://www.toptal.com/developers/gitignore/api/python,jupyternotebooks,vim,visualstudiocode,pycharm
+# End of https://www.toptal.com/developers/gitignore/api/python,jupyternotebooks,vim,visualstudiocode,pycharm,emacs,linux,macos,windows
```

### Comparing `earthkit-maps-0.0.8/.pre-commit-config.yaml` & `earthkit-maps-0.0.9/.pre-commit-config.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.4.0
+  rev: v4.5.0
   hooks:
   - id: trailing-whitespace
   - id: end-of-file-fixer
   - id: check-json
   - id: check-yaml
   - id: check-toml
   # - id: check-added-large-files
@@ -19,30 +19,23 @@
   hooks:
   - id: black
 - repo: https://github.com/keewis/blackdoc
   rev: v0.3.8
   hooks:
   - id: blackdoc
     additional_dependencies: [black==22.3.0]
-- repo: https://github.com/PyCQA/flake8
-  rev: 6.0.0
+- repo: https://github.com/astral-sh/ruff-pre-commit
+  rev: v0.1.3
   hooks:
-  - id: flake8
+  - id: ruff
+    args: [--fix, --show-fixes]
 - repo: https://github.com/executablebooks/mdformat
-  rev: 0.7.16
+  rev: 0.7.17
   hooks:
   - id: mdformat
-    exclude: cruft-update-template.md
 - repo: https://github.com/macisamuele/language-formatters-pre-commit-hooks
-  rev: v2.5.0
+  rev: v2.11.0
   hooks:
   - id: pretty-format-yaml
     args: [--autofix, --preserve-quotes]
   - id: pretty-format-toml
     args: [--autofix]
-    additional_dependencies: [toml-sort<0.22.0]
-- repo: https://github.com/PyCQA/pydocstyle.git
-  rev: 6.1.1
-  hooks:
-  - id: pydocstyle
-    additional_dependencies: [toml]
-    exclude: tests|docs
```

### Comparing `earthkit-maps-0.0.8/LICENSE` & `earthkit-maps-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/Makefile` & `earthkit-maps-0.0.9/Makefile`

 * *Files 12% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 docker-build:
 	docker build -t $(PROJECT) .
 
 docker-run:
 	docker run --rm -ti -v $(PWD):/srv $(PROJECT)
 
 template-update:
-	pre-commit run --all-files cruft -c .pre-commit-config-weekly.yaml
+	pre-commit run --all-files cruft -c .pre-commit-config-cruft.yaml
 
 docs-build:
 	cd docs && rm -fr _api && make clean && make html
 
 #integration-tests:
 #    python -m pytest -vv --cov=. --cov-report=$(COV_REPORT) tests/integration*.py
 #    python -m pytest -vv --doctest-glob='*.md'
```

### Comparing `earthkit-maps-0.0.8/PKG-INFO` & `earthkit-maps-0.0.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthkit-maps
-Version: 0.0.8
+Version: 0.0.9
 Summary: Geospatial visualisation tools and templates
 License: Apache License 2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -30,17 +30,15 @@
 # earthkit.maps
 
 ![earthkit-maps](docs/_static/earthkit-maps.png)
 
 Geospatial visualisation tools and templates
 
 **DISCLAIMER**
-This project is **BETA** and will be **Experimental** for the foreseeable future.
-Interfaces and functionality are likely to change, and the project itself may be scrapped.
-**DO NOT** use this software in any project/software that is operational.
+This project is in the **BETA** stage of development. Please be aware that interfaces and functionality may change as the project develops. If this software is to be used in operational systems you are **strongly advised to use a released tag in your system configuration**, and you should be willing to accept incoming changes and bug fixes that require adaptations on your part. ECMWF **does use** this software in operations and abides by the same caveats.
 
 ## Quick Start
 
 ```python
 >>> import earthkit.maps
 
 ```
```

### Comparing `earthkit-maps-0.0.8/README.md` & `earthkit-maps-0.0.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # earthkit.maps
 
 ![earthkit-maps](docs/_static/earthkit-maps.png)
 
 Geospatial visualisation tools and templates
 
 **DISCLAIMER**
-This project is **BETA** and will be **Experimental** for the foreseeable future.
-Interfaces and functionality are likely to change, and the project itself may be scrapped.
-**DO NOT** use this software in any project/software that is operational.
+This project is in the **BETA** stage of development. Please be aware that interfaces and functionality may change as the project develops. If this software is to be used in operational systems you are **strongly advised to use a released tag in your system configuration**, and you should be willing to accept incoming changes and bug fixes that require adaptations on your part. ECMWF **does use** this software in operations and abides by the same caveats.
 
 ## Quick Start
 
 ```python
 >>> import earthkit.maps
 
 ```
```

### Comparing `earthkit-maps-0.0.8/docs/_static/earthkit-maps.png` & `earthkit-maps-0.0.9/docs/_static/earthkit-maps.png`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/docs/conf.py` & `earthkit-maps-0.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/docs/examples/efi.ipynb` & `earthkit-maps-0.0.9/docs/examples/efi.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/docs/examples/era5-el-nino.ipynb` & `earthkit-maps-0.0.9/docs/examples/era5-el-nino.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/docs/examples/fieldlist-input.ipynb` & `earthkit-maps-0.0.9/docs/examples/fieldlist-input.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/docs/examples/projected-coordinates.ipynb` & `earthkit-maps-0.0.9/docs/examples/projected-coordinates.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/docs/examples/scatter.ipynb` & `earthkit-maps-0.0.9/docs/examples/scatter.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/docs/examples/t850-z500.ipynb` & `earthkit-maps-0.0.9/docs/examples/t850-z500.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/__init__.py` & `earthkit-maps-0.0.9/earthkit/maps/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/data/colors/earthkit.yaml` & `earthkit-maps-0.0.9/earthkit/maps/data/colors/earthkit.yaml`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/data/domains.yaml` & `earthkit-maps-0.0.9/earthkit/maps/data/domains.yaml`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/data/logos/ecmwf.png` & `earthkit-maps-0.0.9/earthkit/maps/data/logos/ecmwf.png`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/data/schemas/default.yaml` & `earthkit-maps-0.0.9/earthkit/maps/data/schemas/default.yaml`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/Lato/Lato-Black.ttf` & `earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/Lato/Lato-Black.ttf`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/Lato/Lato-BlackItalic.ttf` & `earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/Lato/Lato-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/Lato/Lato-Bold.ttf` & `earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/Lato/Lato-Bold.ttf`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/Lato/Lato-BoldItalic.ttf` & `earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/Lato/Lato-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/Lato/Lato-Italic.ttf` & `earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/Lato/Lato-Italic.ttf`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/Lato/Lato-Light.ttf` & `earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/Lato/Lato-Light.ttf`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/Lato/Lato-LightItalic.ttf` & `earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/Lato/Lato-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/Lato/Lato-Regular.ttf` & `earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/Lato/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/Lato/Lato-Thin.ttf` & `earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/Lato/Lato-Thin.ttf`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/Lato/Lato-ThinItalic.ttf` & `earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/Lato/Lato-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/OpenSans/OFL.txt` & `earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/OpenSans/OFL.txt`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/OpenSans/OpenSans-Bold.ttf` & `earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/OpenSans/OpenSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/OpenSans/OpenSans-BoldItalic.ttf` & `earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/OpenSans/OpenSans-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/OpenSans/OpenSans-ExtraBold.ttf` & `earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/OpenSans/OpenSans-ExtraBold.ttf`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/OpenSans/OpenSans-ExtraBoldItalic.ttf` & `earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/OpenSans/OpenSans-ExtraBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/OpenSans/OpenSans-Italic.ttf` & `earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/OpenSans/OpenSans-Italic.ttf`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/OpenSans/OpenSans-Light.ttf` & `earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/OpenSans/OpenSans-Light.ttf`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/OpenSans/OpenSans-LightItalic.ttf` & `earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/OpenSans/OpenSans-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/OpenSans/OpenSans-Medium.ttf` & `earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/OpenSans/OpenSans-Medium.ttf`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/OpenSans/OpenSans-MediumItalic.ttf` & `earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/OpenSans/OpenSans-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/OpenSans/OpenSans-Regular.ttf` & `earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/OpenSans/OpenSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/OpenSans/OpenSans-SemiBold.ttf` & `earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/OpenSans/OpenSans-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/data/static/fonts/OpenSans/OpenSans-SemiBoldItalic.ttf` & `earthkit-maps-0.0.9/earthkit/maps/data/static/fonts/OpenSans/OpenSans-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/data/static/images/logos/ecmwf.png` & `earthkit-maps-0.0.9/earthkit/maps/data/static/images/logos/ecmwf.png`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/data.py` & `earthkit-maps-0.0.9/earthkit/maps/data.py`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/definitions.py` & `earthkit-maps-0.0.9/earthkit/maps/definitions.py`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/domains/__init__.py` & `earthkit-maps-0.0.9/earthkit/maps/domains/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/domains/bounds.py` & `earthkit-maps-0.0.9/earthkit/maps/domains/bounds.py`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/domains/crs.py` & `earthkit-maps-0.0.9/earthkit/maps/domains/crs.py`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/domains/domain.py` & `earthkit-maps-0.0.9/earthkit/maps/domains/domain.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,17 +120,17 @@
         can_bbox = True
         if any(isinstance(self.crs, crs) for crs in NO_BBOX):
             can_bbox = False
         return can_bbox
 
     @property
     def title(self):
-        if self.domain_name in DOMAIN_LOOKUP["the_countries"]:
-            return f"the {self.domain_name}"
-        elif self.domain_name is None:
+        # if self.domain_name in DOMAIN_LOOKUP["the_countries"]:
+        #     return f"the {self.domain_name}"
+        if self.domain_name is None:
             if self.bounds is None:
                 string = "custom domain"
             else:
                 ordinal_values = []
                 for lon in self.latlon_bounds[:2]:
                     direction = ""
                     if lon != 0:
```

### Comparing `earthkit-maps-0.0.8/earthkit/maps/domains/natural_earth.py` & `earthkit-maps-0.0.9/earthkit/maps/domains/natural_earth.py`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/domains/optimal.py` & `earthkit-maps-0.0.9/earthkit/maps/domains/optimal.py`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/formats/units.py` & `earthkit-maps-0.0.9/earthkit/maps/formats/units.py`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/layers/__init__.py` & `earthkit-maps-0.0.9/earthkit/maps/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/layers/layers.py` & `earthkit-maps-0.0.9/earthkit/maps/layers/layers.py`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/layers/metadata.py` & `earthkit-maps-0.0.9/earthkit/maps/layers/metadata.py`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/layers/subplots.py` & `earthkit-maps-0.0.9/earthkit/maps/layers/subplots.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+
 import cartopy.crs as ccrs
 import cartopy.feature as cfeature
 import cartopy.io.shapereader as shpreader
 import earthkit.data
 import geopandas as gpd
 import matplotlib.pyplot as plt
 import numpy as np
@@ -111,23 +112,32 @@
             # - TEMPORARY: in the future all "fields" will be "fieldlists" -
             if isinstance(data, earthkit.data.core.Base) and hasattr(data, "__len__"):
                 try:
                     data = data[0]
                 except (ValueError, TypeError, AttributeError):
                     pass
             # --------------------------------------------------------------
+
+            is_reduced_gg = False
             if x is not None and y is not None:
                 if transform is None:
                     raise ValueError(
                         "you must pass a 'transform' when plotting manually "
                         "with x and y coordinates"
                     )
                 values = data
             else:
-                x, y, values = extract_scalar(data, self.domain)
+                if data.metadata("gridType", default=None) == "reduced_gg":
+                    is_reduced_gg = True
+                    x, y, values = extract_reduced_gg(data, self.domain)
+                    kwargs.pop("transform_first", None)
+                    transform = self.domain.crs
+
+                else:
+                    x, y, values = extract_scalar(data, self.domain)
                 if transform is None:
                     try:
                         transform = data.projection().to_cartopy_crs()
                     except AttributeError:
                         transform = ccrs.PlateCarree()
 
             source_units = data.metadata("units", default=None)
@@ -138,20 +148,36 @@
                 style_units = None
                 if not schema.force_style_units:
                     style_units = kwargs.pop("units", None) or source_units
                 style = suggest_style(data, units=style_units)
 
             values = style.convert_units(values, source_units, short_name=short_name)
 
-            if "transform_first" not in kwargs:
+            if "transform_first" not in kwargs and not is_reduced_gg:
                 kwargs["transform_first"] = self._can_transform_first(method)
 
-            mappable = method(
-                self, x, y, values, style=style, transform=transform, **kwargs
-            )
+            if is_reduced_gg:
+                mappable = self._tricontourf(
+                    x,
+                    y,
+                    values,
+                    style=style,
+                    transform=transform,
+                    **kwargs,
+                )
+            else:
+                mappable = method(
+                    self,
+                    x,
+                    y,
+                    values,
+                    style=style,
+                    transform=transform,
+                    **kwargs,
+                )
 
             layer = Layer(data, mappable, self, style=style)
             self.layers.append(layer)
 
             return layer
 
         return wrapper
@@ -232,14 +258,20 @@
         except NotImplementedError:
             return style.contourf(self.ax, *args, **kwargs)
 
     @gridded_scalar
     def contourf(self, *args, style=None, **kwargs):
         return style.contourf(self.ax, *args, **kwargs)
 
+    def _tricontourf(self, *args, style=None, **kwargs):
+
+        kwargs.pop("transform", None)
+
+        return style.tricontourf(self.ax, *args, **kwargs)
+
     @polygonal
     def polygons(self, *args, style=None, **kwargs):
         return style.polygons(self.ax, *args, **kwargs)
 
     @gridded_scalar
     def contour(self, *args, style=None, **kwargs):
         return style.contour(self.ax, *args, **kwargs)
@@ -480,7 +512,22 @@
     return x, y, values
 
 
 def extract_vector(data, domain):
     x, y, u_values = extract_scalar(data[0], domain)
     _, _, v_values = extract_scalar(data[1], domain)
     return x, y, (u_values, v_values)
+
+
+def extract_reduced_gg(data, domain):
+    values = data.values
+    points = data.to_points()
+
+    xy = domain.crs.transform_points(
+        ccrs.PlateCarree(),
+        points["x"],
+        points["y"],
+    )
+    x = xy[:, 0]
+    y = xy[:, 1]
+
+    return x, y, values
```

### Comparing `earthkit-maps-0.0.8/earthkit/maps/layers/superplots.py` & `earthkit-maps-0.0.9/earthkit/maps/layers/superplots.py`

 * *Files 1% similar despite different names*

```diff
@@ -418,14 +418,14 @@
         """Display the chart."""
         if len(self) == 0:
             self._rows, self._cols = (1, 1)
             self.add_subplot()
         self._release_queue()
         plt.show(*args, **kwargs)
 
-    def save(self, *args, **kwargs):
+    def save(self, *args, bbox_inches="tight", **kwargs):
         """Save the chart."""
         if len(self) == 0:
             self._rows, self._cols = (1, 1)
             self.add_subplot()
         self._release_queue()
-        return plt.savefig(*args, **kwargs)
+        return plt.savefig(*args, bbox_inches=bbox_inches, **kwargs)
```

### Comparing `earthkit-maps-0.0.8/earthkit/maps/layouts.py` & `earthkit-maps-0.0.9/earthkit/maps/layouts.py`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/legends.py` & `earthkit-maps-0.0.9/earthkit/maps/legends.py`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/logos.py` & `earthkit-maps-0.0.9/earthkit/maps/logos.py`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/quickplot.py` & `earthkit-maps-0.0.9/earthkit/maps/quickplot.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,8 +40,8 @@
 
     for item, unit in zip(data, units):
         chart.plot(item, units=unit)
 
     for method, method_kwargs in blueprint.items():
         getattr(chart, method)(**method_kwargs)
 
-    chart.show()
+    return chart
```

### Comparing `earthkit-maps-0.0.8/earthkit/maps/schemas.py` & `earthkit-maps-0.0.9/earthkit/maps/schemas.py`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/shapes.py` & `earthkit-maps-0.0.9/earthkit/maps/shapes.py`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/styles/__init__.py` & `earthkit-maps-0.0.9/earthkit/maps/styles/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,21 +28,26 @@
 from earthkit.maps.schemas import schema
 
 logger = logging.getLogger(__name__)
 
 DEFAULT_LEGEND_LABEL = "{variable_name} ({units})"
 
 
-def auto_range(data, n_levels=8):
+def auto_range(data, divergence_point=None, n_levels=8):
 
     if isinstance(data, earthkit.data.core.Base):
         data = data.to_numpy()
     min_value = np.nanmin(data)
     max_value = np.nanmax(data)
 
+    if divergence_point == 0:
+        abs_max = max(abs(min_value), abs(max_value))
+        min_value = -abs_max
+        max_value = abs_max
+
     data_range = max_value - min_value
 
     initial_bin = data_range / n_levels
 
     magnitude = 10 ** (math.floor(math.log(initial_bin, 10)))
     bin_width = initial_bin - (initial_bin % -magnitude)
 
@@ -109,14 +114,15 @@
 
 
 class Style:
     def __init__(
         self,
         colors="auto",
         levels=None,
+        divergence_point=None,
         level_step=None,
         level_multiple=None,
         units=None,
         units_override=None,
         normalize=True,
         legend_type="colorbar",
         categories=None,
@@ -130,14 +136,15 @@
             self._colors = schema.cmap
         else:
             self._colors = colors
 
         self._levels = levels
         self._level_step = level_step
         self._level_multiple = level_multiple
+        self._divergence_point = divergence_point
 
         self.legend_type = legend_type
 
         self._units = units
         self._units_override = units_override
         self.normalize = normalize
         self.kwargs = kwargs
@@ -177,15 +184,15 @@
             return values
 
         return Unit(source_units).convert(values, self._units)
 
     def levels(self, data):
         if self._levels is None:
             if self._level_step is None:
-                return auto_range(data)
+                return auto_range(data, self._divergence_point)
             else:
                 return step_range(data, self._level_step, self._level_multiple)
         return self._levels
 
     def get_levels(self, layer):
         return layer.mappable.norm.boundaries
 
@@ -231,14 +238,18 @@
     def plot(self, *args, **kwargs):
         raise NotImplementedError("Generic styles cannot be used with 'plot'")
 
     def contourf(self, ax, x, y, values, *args, **kwargs):
         kwargs = {**self.to_contourf_kwargs(values), **kwargs}
         return ax.contourf(x, y, values, *args, **kwargs)
 
+    def tricontourf(self, ax, x, y, values, *args, **kwargs):
+        kwargs = {**self.to_contourf_kwargs(values), **kwargs}
+        return ax.tricontourf(x, y, values, *args, **kwargs)
+
     def contour(self, ax, x, y, values, *args, **kwargs):
         kwargs = {**self.to_contour_kwargs(values), **kwargs}
         return ax.contour(x, y, values, *args, **kwargs)
 
     def pcolormesh(self, ax, x, y, values, *args, **kwargs):
         kwargs.pop("transform_first", None)
         kwargs = {**self.to_pcolormesh_kwargs(values), **kwargs}
```

### Comparing `earthkit-maps-0.0.8/earthkit/maps/styles/auto.py` & `earthkit-maps-0.0.9/earthkit/maps/styles/auto.py`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/styles/ecmwf/geopotential.py` & `earthkit-maps-0.0.9/earthkit/maps/styles/ecmwf/geopotential.py`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/styles/ecmwf/temperature.py` & `earthkit-maps-0.0.9/earthkit/maps/styles/ecmwf/temperature.py`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/styles/geopotential.py` & `earthkit-maps-0.0.9/earthkit/maps/styles/geopotential.py`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/styles/pressure.py` & `earthkit-maps-0.0.9/earthkit/maps/styles/pressure.py`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/styles/river_discharge.py` & `earthkit-maps-0.0.9/earthkit/maps/styles/river_discharge.py`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/styles/soil.py` & `earthkit-maps-0.0.9/earthkit/maps/styles/soil.py`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/styles/temperature.py` & `earthkit-maps-0.0.9/earthkit/maps/styles/temperature.py`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit/maps/utils.py` & `earthkit-maps-0.0.9/earthkit/maps/utils.py`

 * *Files identical despite different names*

### Comparing `earthkit-maps-0.0.8/earthkit_maps.egg-info/PKG-INFO` & `earthkit-maps-0.0.9/earthkit_maps.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthkit-maps
-Version: 0.0.8
+Version: 0.0.9
 Summary: Geospatial visualisation tools and templates
 License: Apache License 2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -30,17 +30,15 @@
 # earthkit.maps
 
 ![earthkit-maps](docs/_static/earthkit-maps.png)
 
 Geospatial visualisation tools and templates
 
 **DISCLAIMER**
-This project is **BETA** and will be **Experimental** for the foreseeable future.
-Interfaces and functionality are likely to change, and the project itself may be scrapped.
-**DO NOT** use this software in any project/software that is operational.
+This project is in the **BETA** stage of development. Please be aware that interfaces and functionality may change as the project develops. If this software is to be used in operational systems you are **strongly advised to use a released tag in your system configuration**, and you should be willing to accept incoming changes and bug fixes that require adaptations on your part. ECMWF **does use** this software in operations and abides by the same caveats.
 
 ## Quick Start
 
 ```python
 >>> import earthkit.maps
 
 ```
```

### Comparing `earthkit-maps-0.0.8/earthkit_maps.egg-info/SOURCES.txt` & `earthkit-maps-0.0.9/earthkit_maps.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 .cruft.json
 .gitignore
-.pre-commit-config-weekly.yaml
 .pre-commit-config.yaml
 Dockerfile
 LICENSE
 MANIFST.in
 Makefile
 README.md
 environment.yml
@@ -16,14 +15,15 @@
 docs/_static/earthkit-maps.png
 docs/examples/efi.ipynb
 docs/examples/era5-el-nino.ipynb
 docs/examples/fieldlist-input.ipynb
 docs/examples/projected-coordinates.ipynb
 docs/examples/scatter.ipynb
 docs/examples/t850-z500.ipynb
+docs/images/quickplot-era5-t2m-20220901.png
 earthkit/maps/__init__.py
 earthkit/maps/data.py
 earthkit/maps/definitions.py
 earthkit/maps/layouts.py
 earthkit/maps/legends.py
 earthkit/maps/logos.py
 earthkit/maps/quickplot.py
@@ -81,14 +81,15 @@
 earthkit/maps/formats/units.py
 earthkit/maps/layers/__init__.py
 earthkit/maps/layers/layers.py
 earthkit/maps/layers/metadata.py
 earthkit/maps/layers/subplots.py
 earthkit/maps/layers/superplots.py
 earthkit/maps/styles/__init__.py
+earthkit/maps/styles/anomalies.py
 earthkit/maps/styles/auto.py
 earthkit/maps/styles/geopotential.py
 earthkit/maps/styles/pressure.py
 earthkit/maps/styles/river_discharge.py
 earthkit/maps/styles/soil.py
 earthkit/maps/styles/temperature.py
 earthkit/maps/styles/ecmwf/geopotential.py
```

### Comparing `earthkit-maps-0.0.8/setup.cfg` & `earthkit-maps-0.0.9/setup.cfg`

 * *Files identical despite different names*

