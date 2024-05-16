# Comparing `tmp/stips-2.2.0.tar.gz` & `tmp/stips-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stips-2.2.0.tar", last modified: Fri May 10 13:25:57 2024, max compression
+gzip compressed data, was "stips-2.2.1.tar", last modified: Thu May 16 01:01:54 2024, max compression
```

## Comparing `stips-2.2.0.tar` & `stips-2.2.1.tar`

### file list

```diff
@@ -1,107 +1,108 @@
-drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.297964 stips-2.2.0/
-drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.222033 stips-2.2.0/.github/
-drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.235329 stips-2.2.0/.github/workflows/
--rw-r--r--   0 jotor     (2330)     1031     1780 2024-05-10 13:21:12.000000 stips-2.2.0/.github/workflows/ci_workflows.yml
--rw-r--r--   0 jotor     (2330)     1031     3045 2024-05-10 13:21:12.000000 stips-2.2.0/.gitignore
--rw-r--r--   0 jotor     (2330)     1031     1018 2024-05-10 13:21:12.000000 stips-2.2.0/.readthedocs.yaml
--rw-r--r--   0 jotor     (2330)     1031      282 2024-05-10 13:21:12.000000 stips-2.2.0/.rtd-environment.yml
--rw-r--r--   0 jotor     (2330)     1031     3279 2024-05-10 13:21:12.000000 stips-2.2.0/CHANGES.rst
--rw-r--r--   0 jotor     (2330)     1031      266 2024-05-10 13:21:12.000000 stips-2.2.0/CITATION
--rw-r--r--   0 jotor     (2330)     1031     3207 2024-05-10 13:21:12.000000 stips-2.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 jotor     (2330)     1031      721 2024-05-10 13:21:12.000000 stips-2.2.0/CONTRIBUTING.md
--rw-r--r--   0 jotor     (2330)     1031      673 2024-05-10 13:21:12.000000 stips-2.2.0/Dockerfile
--rw-r--r--   0 jotor     (2330)     1031      376 2024-05-10 13:21:12.000000 stips-2.2.0/MANIFEST.in
--rw-r--r--   0 jotor     (2330)     1031      753 2024-05-10 13:25:57.297515 stips-2.2.0/PKG-INFO
--rw-r--r--   0 jotor     (2330)     1031     2346 2024-05-10 13:21:12.000000 stips-2.2.0/README.md
-drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.243025 stips-2.2.0/docs/
--rw-r--r--   0 jotor     (2330)     1031     4810 2024-05-10 13:21:12.000000 stips-2.2.0/docs/Makefile
--rw-r--r--   0 jotor     (2330)     1031     9600 2024-05-10 13:21:12.000000 stips-2.2.0/docs/basic_tutorial.rst
--rw-r--r--   0 jotor     (2330)     1031     2865 2024-05-10 13:21:12.000000 stips-2.2.0/docs/bugs.rst
--rw-r--r--   0 jotor     (2330)     1031     7430 2024-05-10 13:21:12.000000 stips-2.2.0/docs/conf.py
--rw-r--r--   0 jotor     (2330)     1031     3654 2024-05-10 13:21:12.000000 stips-2.2.0/docs/examples.rst
-drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.243599 stips-2.2.0/docs/exts/
--rw-r--r--   0 jotor     (2330)     1031     3319 2024-05-10 13:21:12.000000 stips-2.2.0/docs/exts/numfig.py
--rw-r--r--   0 jotor     (2330)     1031      164 2024-05-10 13:21:12.000000 stips-2.2.0/docs/help.rst
--rw-r--r--   0 jotor     (2330)     1031     2144 2024-05-10 13:21:12.000000 stips-2.2.0/docs/index.rst
--rw-r--r--   0 jotor     (2330)     1031     5528 2024-05-10 13:21:12.000000 stips-2.2.0/docs/installation.rst
--rw-r--r--   0 jotor     (2330)     1031     4513 2024-05-10 13:21:12.000000 stips-2.2.0/docs/make.bat
--rw-r--r--   0 jotor     (2330)     1031      273 2024-05-10 13:21:12.000000 stips-2.2.0/docs/requirements.txt
-drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.245670 stips-2.2.0/docs/roman_figures/
--rw-r--r--   0 jotor     (2330)     1031   415382 2024-05-10 13:21:12.000000 stips-2.2.0/docs/roman_figures/stips_basic_tutorial.png
--rw-r--r--   0 jotor     (2330)     1031   404340 2024-05-10 13:21:12.000000 stips-2.2.0/docs/roman_figures/stips_demo.png
--rw-r--r--   0 jotor     (2330)     1031      141 2024-05-10 13:21:12.000000 stips-2.2.0/docs/rtd-pip-requirements
-drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.248488 stips-2.2.0/docs/using_stips/
--rw-r--r--   0 jotor     (2330)     1031     8768 2024-05-10 13:21:12.000000 stips-2.2.0/docs/using_stips/catalogue_formats.rst
--rw-r--r--   0 jotor     (2330)     1031     7358 2024-05-10 13:21:12.000000 stips-2.2.0/docs/using_stips/config_file.rst
--rw-r--r--   0 jotor     (2330)     1031     1120 2024-05-10 13:21:12.000000 stips-2.2.0/docs/using_stips/psf_grid.rst
--rw-r--r--   0 jotor     (2330)     1031      203 2024-05-10 13:21:12.000000 stips-2.2.0/docs/using_stips.rst
--rw-r--r--   0 jotor     (2330)     1031     1682 2024-05-10 13:21:12.000000 stips-2.2.0/environment.yml
--rw-r--r--   0 jotor     (2330)     1031     2230 2024-05-10 13:21:12.000000 stips-2.2.0/environment_dev.yml
-drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.250372 stips-2.2.0/licenses/
--rw-r--r--   0 jotor     (2330)     1031     1539 2024-05-10 13:21:12.000000 stips-2.2.0/licenses/LICENSE.rst
--rw-r--r--   0 jotor     (2330)     1031      372 2024-05-10 13:21:12.000000 stips-2.2.0/licenses/README.rst
--rw-r--r--   0 jotor     (2330)     1031     1659 2024-05-10 13:21:12.000000 stips-2.2.0/licenses/TEMPLATE_LICENCE.rst
-drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.251976 stips-2.2.0/notebooks/
--rw-r--r--   0 jotor     (2330)     1031    23150 2024-05-10 13:21:12.000000 stips-2.2.0/notebooks/STIPS Advanced I – Further Observations, Noise and Distortion.ipynb
--rw-r--r--   0 jotor     (2330)     1031    12688 2024-05-10 13:21:12.000000 stips-2.2.0/notebooks/STIPS Advanced II - PSFs.ipynb
--rw-r--r--   0 jotor     (2330)     1031    13384 2024-05-10 13:21:12.000000 stips-2.2.0/notebooks/STIPS Basic Tutorial.ipynb
-drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.252689 stips-2.2.0/notebooks/notebooks_data/
--rw-r--r--   0 jotor     (2330)     1031  2263680 2024-05-10 13:21:12.000000 stips-2.2.0/notebooks/notebooks_data/psf_WFI_2.0.0_F129_sca01.fits
-drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.257837 stips-2.2.0/ref_data/
--rw-r--r--   0 jotor     (2330)     1031      696 2024-05-10 13:21:12.000000 stips-2.2.0/ref_data/retrieve_stips_data.py
--rw-r--r--   0 jotor     (2330)     1031     1740 2024-05-10 13:25:57.300022 stips-2.2.0/setup.cfg
--rwxr-xr-x   0 jotor     (2330)     1031      126 2024-05-10 13:21:12.000000 stips-2.2.0/setup.py
-drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.259206 stips-2.2.0/stips/
--rwxr-xr-x   0 jotor     (2330)     1031      802 2024-05-10 13:21:12.000000 stips-2.2.0/stips/__init__.py
-drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.265113 stips-2.2.0/stips/astro_image/
--rwxr-xr-x   0 jotor     (2330)     1031       83 2024-05-10 13:21:12.000000 stips-2.2.0/stips/astro_image/__init__.py
--rwxr-xr-x   0 jotor     (2330)     1031    61362 2024-05-10 13:21:12.000000 stips-2.2.0/stips/astro_image/astro_image.py
-drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.268325 stips-2.2.0/stips/astro_image/tests/
--rwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:21:12.000000 stips-2.2.0/stips/astro_image/tests/__init__.py
--rwxr-xr-x   0 jotor     (2330)     1031     4206 2024-05-10 13:21:12.000000 stips-2.2.0/stips/astro_image/tests/test_AstroImage.py
--rwxr-xr-x   0 jotor     (2330)     1031      468 2024-05-10 13:21:12.000000 stips-2.2.0/stips/astro_image/tests/test_header.py
--rwxr-xr-x   0 jotor     (2330)     1031     3821 2024-05-10 13:21:12.000000 stips-2.2.0/stips/astro_image/tests/test_wcs.py
--rwxr-xr-x   0 jotor     (2330)     1031      344 2024-05-10 13:21:12.000000 stips-2.2.0/stips/conftest.py
-drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.277840 stips-2.2.0/stips/data/
--rwxr-xr-x   0 jotor     (2330)     1031    15321 2024-05-10 13:21:12.000000 stips-2.2.0/stips/data/CreateIsochroneGrid.py
--rwxr-xr-x   0 jotor     (2330)     1031     6532 2024-05-10 13:21:12.000000 stips-2.2.0/stips/data/CreatePhoenixGrid.py
--rwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:21:12.000000 stips-2.2.0/stips/data/__init__.py
--rwxr-xr-x   0 jotor     (2330)     1031  2263680 2024-05-10 13:21:12.000000 stips-2.2.0/stips/data/psf_WFI_2.0.0_F129_sca01.fits
--rwxr-xr-x   0 jotor     (2330)     1031     2420 2024-05-10 13:21:12.000000 stips-2.2.0/stips/data/stips_config.yaml
-drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.279590 stips-2.2.0/stips/errors/
--rwxr-xr-x   0 jotor     (2330)     1031      116 2024-05-10 13:21:12.000000 stips-2.2.0/stips/errors/__init__.py
--rwxr-xr-x   0 jotor     (2330)     1031     3932 2024-05-10 13:21:12.000000 stips-2.2.0/stips/errors/make_cosmic_ray.py
-drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.282919 stips-2.2.0/stips/instruments/
--rwxr-xr-x   0 jotor     (2330)     1031      102 2024-05-10 13:21:12.000000 stips-2.2.0/stips/instruments/__init__.py
--rwxr-xr-x   0 jotor     (2330)     1031    51688 2024-05-10 13:21:12.000000 stips-2.2.0/stips/instruments/instrument.py
--rwxr-xr-x   0 jotor     (2330)     1031     1476 2024-05-10 13:21:12.000000 stips-2.2.0/stips/instruments/roman_instrument.py
--rwxr-xr-x   0 jotor     (2330)     1031    11345 2024-05-10 13:21:12.000000 stips-2.2.0/stips/instruments/wfi.py
-drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.284494 stips-2.2.0/stips/observation_module/
--rwxr-xr-x   0 jotor     (2330)     1031       99 2024-05-10 13:21:12.000000 stips-2.2.0/stips/observation_module/__init__.py
--rwxr-xr-x   0 jotor     (2330)     1031    13571 2024-05-10 13:21:12.000000 stips-2.2.0/stips/observation_module/observation_module.py
-drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.286580 stips-2.2.0/stips/scene_module/
--rwxr-xr-x   0 jotor     (2330)     1031       98 2024-05-10 13:21:12.000000 stips-2.2.0/stips/scene_module/__init__.py
--rwxr-xr-x   0 jotor     (2330)     1031     6710 2024-05-10 13:21:12.000000 stips-2.2.0/stips/scene_module/convert_units.py
--rwxr-xr-x   0 jotor     (2330)     1031    23804 2024-05-10 13:21:12.000000 stips-2.2.0/stips/scene_module/scene_module.py
-drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.288805 stips-2.2.0/stips/stellar_module/
--rwxr-xr-x   0 jotor     (2330)     1031       91 2024-05-10 13:21:12.000000 stips-2.2.0/stips/stellar_module/__init__.py
--rwxr-xr-x   0 jotor     (2330)     1031    14428 2024-05-10 13:21:12.000000 stips-2.2.0/stips/stellar_module/star_generator.py
-drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.289833 stips-2.2.0/stips/tests/
--rwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:21:12.000000 stips-2.2.0/stips/tests/__init__.py
-drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.293512 stips-2.2.0/stips/utilities/
--rwxr-xr-x   0 jotor     (2330)     1031     8114 2024-05-10 13:21:12.000000 stips-2.2.0/stips/utilities/DataTable.py
--rwxr-xr-x   0 jotor     (2330)     1031      385 2024-05-10 13:21:12.000000 stips-2.2.0/stips/utilities/__init__.py
--rw-r--r--   0 jotor     (2330)     1031    12110 2024-05-10 13:21:12.000000 stips-2.2.0/stips/utilities/makePSF.py
--rwxr-xr-x   0 jotor     (2330)     1031     3612 2024-05-10 13:21:12.000000 stips-2.2.0/stips/utilities/testing.py
-drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.295012 stips-2.2.0/stips/utilities/tests/
--rwxr-xr-x   0 jotor     (2330)     1031     2091 2024-05-10 13:21:12.000000 stips-2.2.0/stips/utilities/tests/test_config.py
--rwxr-xr-x   0 jotor     (2330)     1031    12282 2024-05-10 13:21:12.000000 stips-2.2.0/stips/utilities/tests/test_makePSF.py
--rwxr-xr-x   0 jotor     (2330)     1031    25231 2024-05-10 13:21:12.000000 stips-2.2.0/stips/utilities/utilities.py
-drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.296478 stips-2.2.0/stips.egg-info/
--rw-r--r--   0 jotor     (2330)     1031      753 2024-05-10 13:25:57.000000 stips-2.2.0/stips.egg-info/PKG-INFO
--rw-r--r--   0 jotor     (2330)     1031     2232 2024-05-10 13:25:57.000000 stips-2.2.0/stips.egg-info/SOURCES.txt
--rw-r--r--   0 jotor     (2330)     1031        1 2024-05-10 13:25:57.000000 stips-2.2.0/stips.egg-info/dependency_links.txt
--rw-r--r--   0 jotor     (2330)     1031        1 2024-05-10 13:25:57.000000 stips-2.2.0/stips.egg-info/not-zip-safe
--rw-r--r--   0 jotor     (2330)     1031      136 2024-05-10 13:25:57.000000 stips-2.2.0/stips.egg-info/requires.txt
--rw-r--r--   0 jotor     (2330)     1031        6 2024-05-10 13:25:57.000000 stips-2.2.0/stips.egg-info/top_level.txt
--rw-r--r--   0 jotor     (2330)     1031      310 2024-05-10 13:21:12.000000 stips-2.2.0/tox.ini
+drwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)        0 2024-05-16 01:01:54.038188 stips-2.2.1/
+drwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)        0 2024-05-16 01:01:53.967915 stips-2.2.1/.github/
+drwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)        0 2024-05-16 01:01:53.982373 stips-2.2.1/.github/workflows/
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)     1780 2024-05-16 01:00:58.000000 stips-2.2.1/.github/workflows/ci_workflows.yml
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)     3045 2024-05-16 01:00:58.000000 stips-2.2.1/.gitignore
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)     1018 2024-05-16 01:00:58.000000 stips-2.2.1/.readthedocs.yaml
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)      282 2024-05-16 01:00:58.000000 stips-2.2.1/.rtd-environment.yml
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)     3501 2024-05-16 01:00:58.000000 stips-2.2.1/CHANGES.rst
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)      266 2024-05-16 01:00:58.000000 stips-2.2.1/CITATION
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)     3207 2024-05-16 01:00:58.000000 stips-2.2.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)      721 2024-05-16 01:00:58.000000 stips-2.2.1/CONTRIBUTING.md
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)      673 2024-05-16 01:00:58.000000 stips-2.2.1/Dockerfile
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)      376 2024-05-16 01:00:58.000000 stips-2.2.1/MANIFEST.in
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)      753 2024-05-16 01:01:54.037923 stips-2.2.1/PKG-INFO
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)     2422 2024-05-16 01:00:58.000000 stips-2.2.1/README.md
+drwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)        0 2024-05-16 01:01:53.989323 stips-2.2.1/docs/
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)     4810 2024-05-16 01:00:58.000000 stips-2.2.1/docs/Makefile
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)     9600 2024-05-16 01:00:58.000000 stips-2.2.1/docs/basic_tutorial.rst
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)     2865 2024-05-16 01:00:58.000000 stips-2.2.1/docs/bugs.rst
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)     7428 2024-05-16 01:00:58.000000 stips-2.2.1/docs/conf.py
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)     3654 2024-05-16 01:00:58.000000 stips-2.2.1/docs/examples.rst
+drwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)        0 2024-05-16 01:01:53.989876 stips-2.2.1/docs/exts/
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)     3319 2024-05-16 01:00:58.000000 stips-2.2.1/docs/exts/numfig.py
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)      164 2024-05-16 01:00:58.000000 stips-2.2.1/docs/help.rst
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)     2154 2024-05-16 01:00:58.000000 stips-2.2.1/docs/index.rst
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)     5528 2024-05-16 01:00:58.000000 stips-2.2.1/docs/installation.rst
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)     4513 2024-05-16 01:00:58.000000 stips-2.2.1/docs/make.bat
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)     6413 2024-05-16 01:00:58.000000 stips-2.2.1/docs/release.rst
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)      273 2024-05-16 01:00:58.000000 stips-2.2.1/docs/requirements.txt
+drwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)        0 2024-05-16 01:01:53.993333 stips-2.2.1/docs/roman_figures/
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)   415382 2024-05-16 01:00:58.000000 stips-2.2.1/docs/roman_figures/stips_basic_tutorial.png
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)   404340 2024-05-16 01:00:58.000000 stips-2.2.1/docs/roman_figures/stips_demo.png
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)      141 2024-05-16 01:00:58.000000 stips-2.2.1/docs/rtd-pip-requirements
+drwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)        0 2024-05-16 01:01:53.997122 stips-2.2.1/docs/using_stips/
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)     8768 2024-05-16 01:00:58.000000 stips-2.2.1/docs/using_stips/catalogue_formats.rst
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)     7358 2024-05-16 01:00:58.000000 stips-2.2.1/docs/using_stips/config_file.rst
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)     1120 2024-05-16 01:00:58.000000 stips-2.2.1/docs/using_stips/psf_grid.rst
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)      203 2024-05-16 01:00:58.000000 stips-2.2.1/docs/using_stips.rst
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)     1682 2024-05-16 01:00:58.000000 stips-2.2.1/environment.yml
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)     2230 2024-05-16 01:00:58.000000 stips-2.2.1/environment_dev.yml
+drwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)        0 2024-05-16 01:01:53.998898 stips-2.2.1/licenses/
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)     1539 2024-05-16 01:00:58.000000 stips-2.2.1/licenses/LICENSE.rst
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)      372 2024-05-16 01:00:58.000000 stips-2.2.1/licenses/README.rst
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)     1659 2024-05-16 01:00:58.000000 stips-2.2.1/licenses/TEMPLATE_LICENCE.rst
+drwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)        0 2024-05-16 01:01:54.000643 stips-2.2.1/notebooks/
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)    23150 2024-05-16 01:00:58.000000 stips-2.2.1/notebooks/STIPS Advanced I – Further Observations, Noise and Distortion.ipynb
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)    12688 2024-05-16 01:00:58.000000 stips-2.2.1/notebooks/STIPS Advanced II - PSFs.ipynb
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)    13384 2024-05-16 01:00:58.000000 stips-2.2.1/notebooks/STIPS Basic Tutorial.ipynb
+drwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)        0 2024-05-16 01:01:54.001269 stips-2.2.1/notebooks/notebooks_data/
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)  2263680 2024-05-16 01:00:58.000000 stips-2.2.1/notebooks/notebooks_data/psf_WFI_2.0.0_F129_sca01.fits
+drwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)        0 2024-05-16 01:01:54.007857 stips-2.2.1/ref_data/
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)      696 2024-05-16 01:00:58.000000 stips-2.2.1/ref_data/retrieve_stips_data.py
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)     1740 2024-05-16 01:01:54.039524 stips-2.2.1/setup.cfg
+-rwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)      126 2024-05-16 01:00:58.000000 stips-2.2.1/setup.py
+drwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)        0 2024-05-16 01:01:54.009260 stips-2.2.1/stips/
+-rwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)      802 2024-05-16 01:00:58.000000 stips-2.2.1/stips/__init__.py
+drwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)        0 2024-05-16 01:01:54.013997 stips-2.2.1/stips/astro_image/
+-rwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)       83 2024-05-16 01:00:58.000000 stips-2.2.1/stips/astro_image/__init__.py
+-rwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)    61361 2024-05-16 01:00:58.000000 stips-2.2.1/stips/astro_image/astro_image.py
+drwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)        0 2024-05-16 01:01:54.016487 stips-2.2.1/stips/astro_image/tests/
+-rwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)        0 2024-05-16 01:00:58.000000 stips-2.2.1/stips/astro_image/tests/__init__.py
+-rwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)     4206 2024-05-16 01:00:58.000000 stips-2.2.1/stips/astro_image/tests/test_AstroImage.py
+-rwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)      468 2024-05-16 01:00:58.000000 stips-2.2.1/stips/astro_image/tests/test_header.py
+-rwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)     3821 2024-05-16 01:00:58.000000 stips-2.2.1/stips/astro_image/tests/test_wcs.py
+-rwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)      344 2024-05-16 01:00:58.000000 stips-2.2.1/stips/conftest.py
+drwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)        0 2024-05-16 01:01:54.023469 stips-2.2.1/stips/data/
+-rwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)    15321 2024-05-16 01:00:58.000000 stips-2.2.1/stips/data/CreateIsochroneGrid.py
+-rwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)     6532 2024-05-16 01:00:58.000000 stips-2.2.1/stips/data/CreatePhoenixGrid.py
+-rwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)        0 2024-05-16 01:00:58.000000 stips-2.2.1/stips/data/__init__.py
+-rwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)  2263680 2024-05-16 01:00:58.000000 stips-2.2.1/stips/data/psf_WFI_2.0.0_F129_sca01.fits
+-rwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)     2420 2024-05-16 01:00:58.000000 stips-2.2.1/stips/data/stips_config.yaml
+drwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)        0 2024-05-16 01:01:54.024557 stips-2.2.1/stips/errors/
+-rwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)      116 2024-05-16 01:00:58.000000 stips-2.2.1/stips/errors/__init__.py
+-rwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)     3932 2024-05-16 01:00:58.000000 stips-2.2.1/stips/errors/make_cosmic_ray.py
+drwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)        0 2024-05-16 01:01:54.026738 stips-2.2.1/stips/instruments/
+-rwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)      102 2024-05-16 01:00:58.000000 stips-2.2.1/stips/instruments/__init__.py
+-rwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)    51688 2024-05-16 01:00:58.000000 stips-2.2.1/stips/instruments/instrument.py
+-rwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)     1476 2024-05-16 01:00:58.000000 stips-2.2.1/stips/instruments/roman_instrument.py
+-rwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)    11345 2024-05-16 01:00:58.000000 stips-2.2.1/stips/instruments/wfi.py
+drwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)        0 2024-05-16 01:01:54.027813 stips-2.2.1/stips/observation_module/
+-rwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)       99 2024-05-16 01:00:58.000000 stips-2.2.1/stips/observation_module/__init__.py
+-rwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)    13571 2024-05-16 01:00:58.000000 stips-2.2.1/stips/observation_module/observation_module.py
+drwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)        0 2024-05-16 01:01:54.029523 stips-2.2.1/stips/scene_module/
+-rwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)       98 2024-05-16 01:00:58.000000 stips-2.2.1/stips/scene_module/__init__.py
+-rwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)     6710 2024-05-16 01:00:58.000000 stips-2.2.1/stips/scene_module/convert_units.py
+-rwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)    23804 2024-05-16 01:00:58.000000 stips-2.2.1/stips/scene_module/scene_module.py
+drwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)        0 2024-05-16 01:01:54.030727 stips-2.2.1/stips/stellar_module/
+-rwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)       91 2024-05-16 01:00:58.000000 stips-2.2.1/stips/stellar_module/__init__.py
+-rwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)    14428 2024-05-16 01:00:58.000000 stips-2.2.1/stips/stellar_module/star_generator.py
+drwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)        0 2024-05-16 01:01:54.031350 stips-2.2.1/stips/tests/
+-rwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)        0 2024-05-16 01:00:58.000000 stips-2.2.1/stips/tests/__init__.py
+drwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)        0 2024-05-16 01:01:54.034582 stips-2.2.1/stips/utilities/
+-rwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)     8114 2024-05-16 01:00:58.000000 stips-2.2.1/stips/utilities/DataTable.py
+-rwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)      385 2024-05-16 01:00:58.000000 stips-2.2.1/stips/utilities/__init__.py
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)    12110 2024-05-16 01:00:58.000000 stips-2.2.1/stips/utilities/makePSF.py
+-rwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)     3612 2024-05-16 01:00:58.000000 stips-2.2.1/stips/utilities/testing.py
+drwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)        0 2024-05-16 01:01:54.036092 stips-2.2.1/stips/utilities/tests/
+-rwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)     2091 2024-05-16 01:00:58.000000 stips-2.2.1/stips/utilities/tests/test_config.py
+-rwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)    12282 2024-05-16 01:00:58.000000 stips-2.2.1/stips/utilities/tests/test_makePSF.py
+-rwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)    25231 2024-05-16 01:00:58.000000 stips-2.2.1/stips/utilities/utilities.py
+drwxr-xr-x   0 jotor     (2330) STSCI\science  (1031)        0 2024-05-16 01:01:54.036994 stips-2.2.1/stips.egg-info/
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)      753 2024-05-16 01:01:53.000000 stips-2.2.1/stips.egg-info/PKG-INFO
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)     2249 2024-05-16 01:01:53.000000 stips-2.2.1/stips.egg-info/SOURCES.txt
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)        1 2024-05-16 01:01:53.000000 stips-2.2.1/stips.egg-info/dependency_links.txt
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)        1 2024-05-16 01:01:53.000000 stips-2.2.1/stips.egg-info/not-zip-safe
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)      136 2024-05-16 01:01:53.000000 stips-2.2.1/stips.egg-info/requires.txt
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)        6 2024-05-16 01:01:53.000000 stips-2.2.1/stips.egg-info/top_level.txt
+-rw-r--r--   0 jotor     (2330) STSCI\science  (1031)      310 2024-05-16 01:00:58.000000 stips-2.2.1/tox.ini
```

### Comparing `stips-2.2.0/.github/workflows/ci_workflows.yml` & `stips-2.2.1/.github/workflows/ci_workflows.yml`

 * *Files identical despite different names*

### Comparing `stips-2.2.0/.gitignore` & `stips-2.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `stips-2.2.0/.readthedocs.yaml` & `stips-2.2.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `stips-2.2.0/CHANGES.rst` & `stips-2.2.1/CHANGES.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 #############
 Release Notes
 #############
 
 Version History and Change Log
 ------------------------------
 
+Version 2.2.1
+=============
+- Fixed a bug on the version of STIPS in __init__.py
+- Updated WebbPSF version to be >= 1.1.1 instead of == 1.1.1
+- Updated synphot>=1.1.1 and stsynphot>=1.1.0 from forced to specific version.
+
 Version 2.2.0
 =============
 - Added a functionality to allow for faster simulations of extended sources.
 - Fixed a bug related to the simulation of extended sources.
 - Fixed a bug related to the WCS.
 - Updated pandeia to version 3.1 and its corresponding reference files.
 - Changed the minimum required Python version to 3.10
```

### Comparing `stips-2.2.0/CODE_OF_CONDUCT.md` & `stips-2.2.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `stips-2.2.0/CONTRIBUTING.md` & `stips-2.2.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `stips-2.2.0/Dockerfile` & `stips-2.2.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `stips-2.2.0/PKG-INFO` & `stips-2.2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: stips
-Version: 2.2.0
+Version: 2.2.1
 Summary: STIPS is the Space Telescope Imaging Product Simulator.
 Home-page: https://github.com/spacetelescope/STScI-STIPS
 Author: Space Telescope Science Institute
 Author-email: york@stsci.edu
 License: BSD 3-Clause
 Requires-Dist: astropy
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: photutils
-Requires-Dist: synphot==1.1.1
-Requires-Dist: stsynphot==1.1.0
-Requires-Dist: webbpsf==1.1.1
+Requires-Dist: synphot>=1.1.1
+Requires-Dist: stsynphot>=1.1.0
+Requires-Dist: webbpsf>=1.1.1
 Requires-Dist: pandeia.engine==3.1
 Requires-Dist: montage-wrapper
 Requires-Dist: pyyaml
 Requires-Dist: soc_roman_tools
 
 STIPS is the Space Telescope Imaging Product Simulator. It is designed to create simulations of full-detector post-pipeline astronomical scenes for the Nancy Grace Roman Space Telescope.
```

### Comparing `stips-2.2.0/README.md` & `stips-2.2.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 # STScI-STIPS
 
-[![Build Status](https://travis-ci.com/spacetelescope/STScI-STIPS.svg?branch=master)](https://travis-ci.com/spacetelescope/STScI-STIPS)
+[![Build Status](https://github.com/spacetelescope/STScI-STIPS/actions/workflows/ci_workflows.yml/badge.svg?branch=main)](https://github.com/spacetelescope/STScI-STIPS/actions/workflows/ci_workflows.yml?query=branch:main)
 [![STScI](https://img.shields.io/badge/powered%20by-STScI-blue.svg?colorA=707170&colorB=3e8ddd&style=flat)](http://www.stsci.edu)
 
 For documentation and installation instructions please visit https://stips.readthedocs.io
 
 ## Table of Contents
 
 * [Overview](#overview)
 * [Why use STIPS?](#why-use-stips)
 
 ## Overview
 
-STIPS is the Space Telescope Imaging Product Simulator. It is designed to create 
-simulations of full-detector post-pipeline astronomical scenes for the Nancy Grace Roman 
-Space Telescope's Wide-Field Instrument (WFI). STIPS has the ability to add 
+STIPS is the Space Telescope Imaging Product Simulator. It is designed to create
+simulations of full-detector post-pipeline astronomical scenes for the Nancy Grace Roman
+Space Telescope's Wide-Field Instrument (WFI). STIPS has the ability to add
 instrumental distortion (if available) as well as calibration residuals from flatfields,
 dark currents, and cosmic rays. It automatically includes Poisson noise and readout noise.
 It does not include instrument saturation effects.
 
 ## Why use STIPS?
 
-STIPS is intended to produce quick simulations of Level 2 (L2) images, and is provided for 
+STIPS is intended to produce quick simulations of Level 2 (L2) images, and is provided for
 cases where [Pandeia](https://pypi.org/project/pandeia.engine) does not
 provide a large enough simulation area (e.g., full-detector or multiple-detector
 observations). STIPS obtains its Roman instrument and filter values from
 Pandeia, so it should produce output within 10% of output produced by Pandeia.
 
-STIPS does not start with Level 1 (L1) images and propagate instrumental calibrations 
+STIPS does not start with Level 1 (L1) images and propagate instrumental calibrations
 through the simulations. While it does have the ability to add error residuals (representing
-the remaining uncertainty after pipeline calibration), these residuals are not validated 
-against actual pipeline calibrations of L1 images. STIPS is not the ideal choice if 
-extremely good instrumental accuracy is needed. Pandeia is the preferred tool for 
+the remaining uncertainty after pipeline calibration), these residuals are not validated
+against actual pipeline calibrations of L1 images. STIPS is not the ideal choice if
+extremely good instrumental accuracy is needed. Pandeia is the preferred tool for
 high-accuracy observations.
 
 Developed by Brian York ([@york-stsci](https://github.com/york-stsci)),
-Robel Geda ([@robelgeda](https://github.com/robelgeda)), and 
+Robel Geda ([@robelgeda](https://github.com/robelgeda)), and
 O. Justin Otor ([@ojustino](https://github.com/ojustino)).
-Python ePSF code developed by 
+Python ePSF code developed by
 Sebastian Gomez ([@gmzsebastian](https://github.com/gmzsebastian)) based on Fortran code
 developed by Andrea Bellini ([@AndreaBellini](https://github.com/AndreaBellini)).
 
 ![Alt text](docs/roman_figures/stips_demo.png?raw=true "Roman WFI Image of a Star Cluster and Background Galaxies")
```

### Comparing `stips-2.2.0/docs/Makefile` & `stips-2.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `stips-2.2.0/docs/basic_tutorial.rst` & `stips-2.2.1/docs/basic_tutorial.rst`

 * *Files identical despite different names*

### Comparing `stips-2.2.0/docs/bugs.rst` & `stips-2.2.1/docs/bugs.rst`

 * *Files identical despite different names*

### Comparing `stips-2.2.0/docs/conf.py` & `stips-2.2.1/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,14 +176,14 @@
 if eval(setup_cfg.get('edit_on_github')):
 
     versionmod = __import__(setup_cfg['name'] + '.version')
     edit_on_github_project = setup_cfg['github_project']
     if versionmod.version.release:
         edit_on_github_branch = "v" + versionmod.version.version
     else:
-        edit_on_github_branch = "master"
+        edit_on_github_branch = "main"
 
     edit_on_github_source_root = ""
     edit_on_github_doc_root = "docs"
 
 # -- Resolving issue number to links in changelog -----------------------------
 github_issues_url = 'https://github.com/{0}/issues/'.format(setup_cfg['github_project'])
```

### Comparing `stips-2.2.0/docs/examples.rst` & `stips-2.2.1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `stips-2.2.0/docs/exts/numfig.py` & `stips-2.2.1/docs/exts/numfig.py`

 * *Files identical despite different names*

### Comparing `stips-2.2.0/docs/index.rst` & `stips-2.2.1/docs/index.rst`

 * *Files 0% similar despite different names*

```diff
@@ -47,8 +47,9 @@
   :maxdepth: 2
 
   installation
   using_stips
   basic_tutorial
   examples
   bugs
+  release
   help
```

### Comparing `stips-2.2.0/docs/installation.rst` & `stips-2.2.1/docs/installation.rst`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 in this section along with instructions.
 
 STIPS Requirements
 ##################
 
 * ``pandeia>=3.1``: Exposure time calculator.
 
-* ``webbpsf==1.1.1``: Nancy Grace Roman PSF calculator. STIPS also requires that ``poppy``, a
+* ``webbpsf>=1.1.1``: Nancy Grace Roman PSF calculator. STIPS also requires that ``poppy``, a
   support package used by WebbPSF, have version ``>=1.0.3``.
 
 * ``astropy``: STIPS uses Astropy in order to:
 
     * Read and write FITS files.
 
     * Read and write ASCII tables (specifically in the IPAC format).
```

### Comparing `stips-2.2.0/docs/make.bat` & `stips-2.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `stips-2.2.0/docs/roman_figures/stips_basic_tutorial.png` & `stips-2.2.1/docs/roman_figures/stips_basic_tutorial.png`

 * *Files identical despite different names*

### Comparing `stips-2.2.0/docs/roman_figures/stips_demo.png` & `stips-2.2.1/docs/roman_figures/stips_demo.png`

 * *Files identical despite different names*

### Comparing `stips-2.2.0/docs/using_stips/catalogue_formats.rst` & `stips-2.2.1/docs/using_stips/catalogue_formats.rst`

 * *Files identical despite different names*

### Comparing `stips-2.2.0/docs/using_stips/config_file.rst` & `stips-2.2.1/docs/using_stips/config_file.rst`

 * *Files identical despite different names*

### Comparing `stips-2.2.0/docs/using_stips/psf_grid.rst` & `stips-2.2.1/docs/using_stips/psf_grid.rst`

 * *Files identical despite different names*

### Comparing `stips-2.2.0/environment.yml` & `stips-2.2.1/environment.yml`

 * *Files 6% similar despite different names*

```diff
@@ -31,18 +31,18 @@
   - esutil # installed from conda because you need the pre-compiled binaries.
 
   - pip:
     # Special Modules. These are temporary entries and require documentation.
     - poppy==1.0.3
 
     # Core Modules
-    - webbpsf==1.1.1
+    - webbpsf>=1.1.1
     - pandeia.engine==3.1
-    - synphot==1.1.1
-    - stsynphot==1.1.0
+    - synphot>=1.1.1
+    - stsynphot>=1.1.0
     - soc_roman_tools
 
     # Major modules
     - astropy
     - photutils
     - ConfigParser
     - numpy
```

### Comparing `stips-2.2.0/environment_dev.yml` & `stips-2.2.1/environment_dev.yml`

 * *Files 5% similar despite different names*

```diff
@@ -40,18 +40,18 @@
     # poppy 1.0.3 fixes a bug with the way poppy was calling factorial with non-integer
     # values. Currently this is the only way to ensure that webbpsf picks up the correct
     # poppy version. This peg should be removed as soon as webbpsf has updated to only
     # use poppy versions that include this fix.
     - poppy==1.0.3
 
     # Core Modules
-    - webbpsf==1.1.1
+    - webbpsf>=1.1.1
     - pandeia.engine==3.1
-    - synphot==1.1.1
-    - stsynphot==1.1.0
+    - synphot>=1.1.1
+    - stsynphot>=1.1.0
     - soc_roman_tools
 
     # Major modules
     - astropy
     - photutils
     - ConfigParser
     - numpy
```

### Comparing `stips-2.2.0/licenses/LICENSE.rst` & `stips-2.2.1/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `stips-2.2.0/licenses/TEMPLATE_LICENCE.rst` & `stips-2.2.1/licenses/TEMPLATE_LICENCE.rst`

 * *Files identical despite different names*

### Comparing `stips-2.2.0/notebooks/STIPS Advanced I – Further Observations, Noise and Distortion.ipynb` & `stips-2.2.1/notebooks/STIPS Advanced I – Further Observations, Noise and Distortion.ipynb`

 * *Files identical despite different names*

### Comparing `stips-2.2.0/notebooks/STIPS Advanced II - PSFs.ipynb` & `stips-2.2.1/notebooks/STIPS Advanced II - PSFs.ipynb`

 * *Files identical despite different names*

### Comparing `stips-2.2.0/notebooks/STIPS Basic Tutorial.ipynb` & `stips-2.2.1/notebooks/STIPS Basic Tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `stips-2.2.0/notebooks/notebooks_data/psf_WFI_2.0.0_F129_sca01.fits` & `stips-2.2.1/notebooks/notebooks_data/psf_WFI_2.0.0_F129_sca01.fits`

 * *Files identical despite different names*

### Comparing `stips-2.2.0/ref_data/retrieve_stips_data.py` & `stips-2.2.1/ref_data/retrieve_stips_data.py`

 * *Files identical despite different names*

### Comparing `stips-2.2.0/setup.cfg` & `stips-2.2.1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = stips
-version = 2.2.0
+version = 2.2.1
 author = Space Telescope Science Institute
 author_email = york@stsci.edu
 description = STIPS is the Space Telescope Imaging Product Simulator.
 long_description = STIPS is the Space Telescope Imaging Product Simulator. It is designed to create simulations of full-detector post-pipeline astronomical scenes for the Nancy Grace Roman Space Telescope.
 license = BSD 3-Clause
 url = https://github.com/spacetelescope/STScI-STIPS
 edit_on_github = False
@@ -16,17 +16,17 @@
 setup_requires = 
 	numpy
 install_requires = 
 	astropy
 	numpy
 	scipy
 	photutils
-	synphot==1.1.1
-	stsynphot==1.1.0
-	webbpsf==1.1.1
+	synphot>=1.1.1
+	stsynphot>=1.1.0
+	webbpsf>=1.1.1
 	pandeia.engine==3.1
 	montage-wrapper
 	pyyaml
 	soc_roman_tools
 zip_safe = False
 use_2to3 = False
 include_package_data = True
```

### Comparing `stips-2.2.0/stips/__init__.py` & `stips-2.2.1/stips/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import absolute_import
 
 import os
 
 __all__ = ['observation_module', 'scene_module']
 
-__version__ = "2.1.0"
+__version__ = "2.2.1"
 version = __version__
 
 from .utilities import SetupDataPaths
 
 SetupDataPaths()
 
 # Local Definitions
```

### Comparing `stips-2.2.0/stips/astro_image/astro_image.py` & `stips-2.2.1/stips/astro_image/astro_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,15 +369,15 @@
         self._log("info", "Created Extension HDU from AstroImage {}".format(self.name))
         return hdu
 
     @property
     def psf_constructor(self):
         import webbpsf
         if not hasattr(webbpsf, self.telescope.lower()) and self.telescope.lower() == 'roman':
-            return getattr(getattr(webbpsf, 'wfirst'), self.instrument)()
+            return getattr(getattr(webbpsf, 'roman'), self.instrument)()
         if hasattr(webbpsf, self.instrument):
             return getattr(webbpsf, self.instrument)()
         return getattr(getattr(webbpsf, self.telescope), self.instrument)()
 
     def toFits(self, outFile):
         """Create a FITS file from the current state of the AstroImage data."""
         self._log("info", "Writing AstroImage {} to FITS".format(self.name))
```

### Comparing `stips-2.2.0/stips/astro_image/tests/test_AstroImage.py` & `stips-2.2.1/stips/astro_image/tests/test_AstroImage.py`

 * *Files identical despite different names*

### Comparing `stips-2.2.0/stips/astro_image/tests/test_wcs.py` & `stips-2.2.1/stips/astro_image/tests/test_wcs.py`

 * *Files identical despite different names*

### Comparing `stips-2.2.0/stips/data/CreateIsochroneGrid.py` & `stips-2.2.1/stips/data/CreateIsochroneGrid.py`

 * *Files identical despite different names*

### Comparing `stips-2.2.0/stips/data/CreatePhoenixGrid.py` & `stips-2.2.1/stips/data/CreatePhoenixGrid.py`

 * *Files identical despite different names*

### Comparing `stips-2.2.0/stips/data/psf_WFI_2.0.0_F129_sca01.fits` & `stips-2.2.1/stips/data/psf_WFI_2.0.0_F129_sca01.fits`

 * *Files identical despite different names*

### Comparing `stips-2.2.0/stips/data/stips_config.yaml` & `stips-2.2.1/stips/data/stips_config.yaml`

 * *Files identical despite different names*

### Comparing `stips-2.2.0/stips/errors/make_cosmic_ray.py` & `stips-2.2.1/stips/errors/make_cosmic_ray.py`

 * *Files identical despite different names*

### Comparing `stips-2.2.0/stips/instruments/instrument.py` & `stips-2.2.1/stips/instruments/instrument.py`

 * *Files identical despite different names*

### Comparing `stips-2.2.0/stips/instruments/roman_instrument.py` & `stips-2.2.1/stips/instruments/roman_instrument.py`

 * *Files identical despite different names*

### Comparing `stips-2.2.0/stips/instruments/wfi.py` & `stips-2.2.1/stips/instruments/wfi.py`

 * *Files identical despite different names*

### Comparing `stips-2.2.0/stips/observation_module/observation_module.py` & `stips-2.2.1/stips/observation_module/observation_module.py`

 * *Files identical despite different names*

### Comparing `stips-2.2.0/stips/scene_module/convert_units.py` & `stips-2.2.1/stips/scene_module/convert_units.py`

 * *Files identical despite different names*

### Comparing `stips-2.2.0/stips/scene_module/scene_module.py` & `stips-2.2.1/stips/scene_module/scene_module.py`

 * *Files identical despite different names*

### Comparing `stips-2.2.0/stips/stellar_module/star_generator.py` & `stips-2.2.1/stips/stellar_module/star_generator.py`

 * *Files identical despite different names*

### Comparing `stips-2.2.0/stips/utilities/DataTable.py` & `stips-2.2.1/stips/utilities/DataTable.py`

 * *Files identical despite different names*

### Comparing `stips-2.2.0/stips/utilities/makePSF.py` & `stips-2.2.1/stips/utilities/makePSF.py`

 * *Files identical despite different names*

### Comparing `stips-2.2.0/stips/utilities/testing.py` & `stips-2.2.1/stips/utilities/testing.py`

 * *Files identical despite different names*

### Comparing `stips-2.2.0/stips/utilities/tests/test_config.py` & `stips-2.2.1/stips/utilities/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `stips-2.2.0/stips/utilities/tests/test_makePSF.py` & `stips-2.2.1/stips/utilities/tests/test_makePSF.py`

 * *Files identical despite different names*

### Comparing `stips-2.2.0/stips/utilities/utilities.py` & `stips-2.2.1/stips/utilities/utilities.py`

 * *Files identical despite different names*

### Comparing `stips-2.2.0/stips.egg-info/PKG-INFO` & `stips-2.2.1/stips.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: stips
-Version: 2.2.0
+Version: 2.2.1
 Summary: STIPS is the Space Telescope Imaging Product Simulator.
 Home-page: https://github.com/spacetelescope/STScI-STIPS
 Author: Space Telescope Science Institute
 Author-email: york@stsci.edu
 License: BSD 3-Clause
 Requires-Dist: astropy
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: photutils
-Requires-Dist: synphot==1.1.1
-Requires-Dist: stsynphot==1.1.0
-Requires-Dist: webbpsf==1.1.1
+Requires-Dist: synphot>=1.1.1
+Requires-Dist: stsynphot>=1.1.0
+Requires-Dist: webbpsf>=1.1.1
 Requires-Dist: pandeia.engine==3.1
 Requires-Dist: montage-wrapper
 Requires-Dist: pyyaml
 Requires-Dist: soc_roman_tools
 
 STIPS is the Space Telescope Imaging Product Simulator. It is designed to create simulations of full-detector post-pipeline astronomical scenes for the Nancy Grace Roman Space Telescope.
```

### Comparing `stips-2.2.0/stips.egg-info/SOURCES.txt` & `stips-2.2.1/stips.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 docs/bugs.rst
 docs/conf.py
 docs/examples.rst
 docs/help.rst
 docs/index.rst
 docs/installation.rst
 docs/make.bat
+docs/release.rst
 docs/requirements.txt
 docs/rtd-pip-requirements
 docs/using_stips.rst
 docs/exts/numfig.py
 docs/roman_figures/stips_basic_tutorial.png
 docs/roman_figures/stips_demo.png
 docs/using_stips/catalogue_formats.rst
```

