# Comparing `tmp/spiakid_simulation-1.21.tar.gz` & `tmp/spiakid_simulation-1.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spiakid_simulation-1.21.tar", last modified: Tue May 14 08:51:26 2024, max compression
+gzip compressed data, was "spiakid_simulation-1.22.tar", last modified: Thu May 16 12:51:41 2024, max compression
```

## Comparing `spiakid_simulation-1.21.tar` & `spiakid_simulation-1.22.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-14 08:51:26.482870 spiakid_simulation-1.21/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    10177 2023-08-28 10:56:06.000000 spiakid_simulation-1.21/LICENSE
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      184 2024-02-15 13:53:03.000000 spiakid_simulation-1.21/MANIFEST.in
--rw-r--r--   0 sfaes     (4303) sfaes     (2722)     1265 2024-05-14 08:51:26.482870 spiakid_simulation-1.21/PKG-INFO
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     1406 2024-02-08 10:38:39.000000 spiakid_simulation-1.21/README.md
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      643 2024-02-26 13:13:11.000000 spiakid_simulation-1.21/README_for_pip.md
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      665 2024-05-14 08:39:56.000000 spiakid_simulation-1.21/pyproject.toml
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)       38 2024-05-14 08:51:26.482870 spiakid_simulation-1.21/setup.cfg
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-14 08:51:26.406870 spiakid_simulation-1.21/spiakid_simulation/
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-14 08:51:26.446870 spiakid_simulation-1.21/spiakid_simulation/Example/
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-14 08:51:26.446870 spiakid_simulation-1.21/spiakid_simulation/Example/Calib/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      125 2024-04-22 12:39:15.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Calib/Trans.csv
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     3627 2024-04-22 12:39:15.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Calib/Wv_IQ_calib.csv
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     3799 2024-04-23 11:59:54.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Calib/Wv_ph_calib.csv
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     4239 2024-03-11 12:55:11.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Sim_10obj.ipynb
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     4538 2024-03-11 12:55:31.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Sim_Gaussian.ipynb
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     4251 2024-05-14 08:30:04.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Sim_phase.ipynb
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     4910 2024-03-11 12:55:54.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Sim_psf.ipynb
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-14 08:51:26.478870 spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT3750G000M025K200A000.DAT
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT3750G100M025K200A000.DAT
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT4000G050M250K200A040.DAT
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT4125G300M175K200A040.DAT
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT4500G000P050K200A000.DAT
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT5000G150M175K200A040.DAT
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT5125G350M175K200A040.DAT
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT5250G450M300K200A040.DAT
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT5875G000M075K200A020.DAT
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT6625G350M025K200A000.DAT
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT6875G450M150K200A040.DAT
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT7000G450M200K200A040.DAT
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT7000G500M050K200A020.DAT
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT7250G500M225K200A040.DAT
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      665 2024-03-11 13:03:11.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Template_10obj.yaml
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      541 2024-03-11 12:10:32.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Template_Gaussian.yaml
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     1091 2024-05-14 08:30:45.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Template_phase.yaml
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      652 2024-03-11 12:00:07.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Template_psf.yaml
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    18211 2024-05-14 08:35:05.000000 spiakid_simulation-1.21/spiakid_simulation/PhotonSimulator.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      978 2024-02-26 13:07:20.000000 spiakid_simulation-1.21/spiakid_simulation/Simulation.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)        0 2023-10-12 08:37:50.000000 spiakid_simulation-1.21/spiakid_simulation/__init__.py
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-14 08:51:26.478870 spiakid_simulation-1.21/spiakid_simulation/electronics/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      523 2024-02-07 10:08:03.000000 spiakid_simulation-1.21/spiakid_simulation/electronics/Yaml_rw.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    12011 2023-11-06 16:00:40.000000 spiakid_simulation-1.21/spiakid_simulation/electronics/cmplxIQ_params.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      677 2023-11-07 14:19:59.000000 spiakid_simulation-1.21/spiakid_simulation/electronics/data_reading.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     7406 2024-04-22 13:16:25.000000 spiakid_simulation-1.21/spiakid_simulation/electronics/filter.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    53144 2023-11-06 15:58:05.000000 spiakid_simulation-1.21/spiakid_simulation/electronics/resonator.py
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-14 08:51:26.478870 spiakid_simulation-1.21/spiakid_simulation/functions/
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-14 08:51:26.478870 spiakid_simulation-1.21/spiakid_simulation/functions/IQ/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     5250 2024-05-14 08:38:06.000000 spiakid_simulation-1.21/spiakid_simulation/functions/IQ/IQ_sim.py
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-14 08:51:26.478870 spiakid_simulation-1.21/spiakid_simulation/functions/noise/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     5029 2024-04-22 13:11:36.000000 spiakid_simulation-1.21/spiakid_simulation/functions/noise/noise.py
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-14 08:51:26.478870 spiakid_simulation-1.21/spiakid_simulation/functions/output/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     2364 2024-04-23 09:17:38.000000 spiakid_simulation-1.21/spiakid_simulation/functions/output/HDF5_creation.py
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-14 08:51:26.478870 spiakid_simulation-1.21/spiakid_simulation/functions/phase/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     1507 2024-02-07 10:11:13.000000 spiakid_simulation-1.21/spiakid_simulation/functions/phase/calib_read.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     5319 2024-04-23 08:47:14.000000 spiakid_simulation-1.21/spiakid_simulation/functions/phase/phase_conversion.py
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-14 08:51:26.478870 spiakid_simulation-1.21/spiakid_simulation/functions/photon/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     3431 2024-02-29 09:30:06.000000 spiakid_simulation-1.21/spiakid_simulation/functions/photon/black_body.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      264 2023-11-02 10:55:48.000000 spiakid_simulation-1.21/spiakid_simulation/functions/photon/contamination.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     2512 2023-10-06 09:10:32.000000 spiakid_simulation-1.21/spiakid_simulation/functions/photon/photon_gen_image.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     4573 2024-05-14 08:35:26.000000 spiakid_simulation-1.21/spiakid_simulation/functions/photon/rot.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     6529 2024-05-14 08:23:43.000000 spiakid_simulation-1.21/spiakid_simulation/functions/photon/sim_image_photon.py
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-14 08:51:26.478870 spiakid_simulation-1.21/spiakid_simulation/functions/theory/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     6198 2023-08-28 15:04:02.000000 spiakid_simulation-1.21/spiakid_simulation/functions/theory/Calc.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    14485 2023-09-18 12:50:04.000000 spiakid_simulation-1.21/spiakid_simulation/functions/theory/MKID.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    10145 2023-08-28 10:56:06.000000 spiakid_simulation-1.21/spiakid_simulation/functions/theory/SC.py
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-14 08:51:26.482870 spiakid_simulation-1.21/spiakid_simulation/functions/timeline/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     3249 2024-05-14 07:22:08.000000 spiakid_simulation-1.21/spiakid_simulation/functions/timeline/timeline.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      579 2023-08-28 10:56:06.000000 spiakid_simulation-1.21/spiakid_simulation/functions/utils.py
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-14 08:51:26.482870 spiakid_simulation-1.21/spiakid_simulation/functions/yaml/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      522 2024-02-15 12:49:21.000000 spiakid_simulation-1.21/spiakid_simulation/functions/yaml/yaml_rw.py
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-14 08:51:26.482870 spiakid_simulation-1.21/spiakid_simulation/image_process/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     2759 2024-05-13 13:42:02.000000 spiakid_simulation-1.21/spiakid_simulation/image_process/PSF_interface.py
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-14 08:51:26.482870 spiakid_simulation-1.21/spiakid_simulation/image_process/atmosphere/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    16411 2023-12-14 15:07:47.000000 spiakid_simulation-1.21/spiakid_simulation/image_process/atmosphere/interface.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    17502 2024-03-08 16:54:53.000000 spiakid_simulation-1.21/spiakid_simulation/image_process/atmosphere/interface_mult.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     1732 2023-12-14 14:48:00.000000 spiakid_simulation-1.21/spiakid_simulation/image_process/atmosphere/test_displacement.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    14479 2024-05-13 13:40:17.000000 spiakid_simulation-1.21/spiakid_simulation/image_process/atmosphere/turbulence.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     3166 2024-05-14 08:14:01.000000 spiakid_simulation-1.21/spiakid_simulation/image_process/image_generation.py
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-14 08:51:26.482870 spiakid_simulation-1.21/spiakid_simulation.egg-info/
--rw-r--r--   0 sfaes     (4303) sfaes     (2722)     1265 2024-05-14 08:51:26.000000 spiakid_simulation-1.21/spiakid_simulation.egg-info/PKG-INFO
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     3108 2024-05-14 08:51:26.000000 spiakid_simulation-1.21/spiakid_simulation.egg-info/SOURCES.txt
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)        1 2024-05-14 08:51:26.000000 spiakid_simulation-1.21/spiakid_simulation.egg-info/dependency_links.txt
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)       69 2024-05-14 08:51:26.000000 spiakid_simulation-1.21/spiakid_simulation.egg-info/requires.txt
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)       19 2024-05-14 08:51:26.000000 spiakid_simulation-1.21/spiakid_simulation.egg-info/top_level.txt
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-14 08:51:26.482870 spiakid_simulation-1.21/test/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      157 2023-09-18 12:50:04.000000 spiakid_simulation-1.21/test/test_simu.py
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-16 12:51:41.064471 spiakid_simulation-1.22/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    10177 2023-08-28 10:56:06.000000 spiakid_simulation-1.22/LICENSE
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      184 2024-02-15 13:53:03.000000 spiakid_simulation-1.22/MANIFEST.in
+-rw-r--r--   0 sfaes     (4303) sfaes     (2722)     1265 2024-05-16 12:51:41.064471 spiakid_simulation-1.22/PKG-INFO
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     1406 2024-02-08 10:38:39.000000 spiakid_simulation-1.22/README.md
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      643 2024-02-26 13:13:11.000000 spiakid_simulation-1.22/README_for_pip.md
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      665 2024-05-16 12:50:02.000000 spiakid_simulation-1.22/pyproject.toml
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)       38 2024-05-16 12:51:41.064471 spiakid_simulation-1.22/setup.cfg
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-16 12:51:41.044471 spiakid_simulation-1.22/spiakid_simulation/
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-16 12:51:41.044471 spiakid_simulation-1.22/spiakid_simulation/Example/
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-16 12:51:41.044471 spiakid_simulation-1.22/spiakid_simulation/Example/Calib/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      125 2024-04-22 12:39:15.000000 spiakid_simulation-1.22/spiakid_simulation/Example/Calib/Trans.csv
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     3627 2024-04-22 12:39:15.000000 spiakid_simulation-1.22/spiakid_simulation/Example/Calib/Wv_IQ_calib.csv
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     3799 2024-04-23 11:59:54.000000 spiakid_simulation-1.22/spiakid_simulation/Example/Calib/Wv_ph_calib.csv
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     4239 2024-03-11 12:55:11.000000 spiakid_simulation-1.22/spiakid_simulation/Example/Sim_10obj.ipynb
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     4538 2024-03-11 12:55:31.000000 spiakid_simulation-1.22/spiakid_simulation/Example/Sim_Gaussian.ipynb
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     4251 2024-05-14 08:30:04.000000 spiakid_simulation-1.22/spiakid_simulation/Example/Sim_phase.ipynb
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     4910 2024-03-11 12:55:54.000000 spiakid_simulation-1.22/spiakid_simulation/Example/Sim_psf.ipynb
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-16 12:51:41.060471 spiakid_simulation-1.22/spiakid_simulation/Example/Spectrum/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.22/spiakid_simulation/Example/Spectrum/FT3750G000M025K200A000.DAT
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.22/spiakid_simulation/Example/Spectrum/FT3750G100M025K200A000.DAT
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.22/spiakid_simulation/Example/Spectrum/FT4000G050M250K200A040.DAT
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.22/spiakid_simulation/Example/Spectrum/FT4125G300M175K200A040.DAT
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.22/spiakid_simulation/Example/Spectrum/FT4500G000P050K200A000.DAT
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.22/spiakid_simulation/Example/Spectrum/FT5000G150M175K200A040.DAT
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.22/spiakid_simulation/Example/Spectrum/FT5125G350M175K200A040.DAT
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.22/spiakid_simulation/Example/Spectrum/FT5250G450M300K200A040.DAT
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.22/spiakid_simulation/Example/Spectrum/FT5875G000M075K200A020.DAT
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.22/spiakid_simulation/Example/Spectrum/FT6625G350M025K200A000.DAT
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.22/spiakid_simulation/Example/Spectrum/FT6875G450M150K200A040.DAT
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.22/spiakid_simulation/Example/Spectrum/FT7000G450M200K200A040.DAT
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.22/spiakid_simulation/Example/Spectrum/FT7000G500M050K200A020.DAT
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.22/spiakid_simulation/Example/Spectrum/FT7250G500M225K200A040.DAT
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      665 2024-03-11 13:03:11.000000 spiakid_simulation-1.22/spiakid_simulation/Example/Template_10obj.yaml
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      541 2024-03-11 12:10:32.000000 spiakid_simulation-1.22/spiakid_simulation/Example/Template_Gaussian.yaml
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     1091 2024-05-14 08:30:45.000000 spiakid_simulation-1.22/spiakid_simulation/Example/Template_phase.yaml
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      652 2024-03-11 12:00:07.000000 spiakid_simulation-1.22/spiakid_simulation/Example/Template_psf.yaml
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    18126 2024-05-16 12:16:28.000000 spiakid_simulation-1.22/spiakid_simulation/PhotonSimulator.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      978 2024-02-26 13:07:20.000000 spiakid_simulation-1.22/spiakid_simulation/Simulation.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)        0 2023-10-12 08:37:50.000000 spiakid_simulation-1.22/spiakid_simulation/__init__.py
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-16 12:51:41.060471 spiakid_simulation-1.22/spiakid_simulation/electronics/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      523 2024-02-07 10:08:03.000000 spiakid_simulation-1.22/spiakid_simulation/electronics/Yaml_rw.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    12011 2023-11-06 16:00:40.000000 spiakid_simulation-1.22/spiakid_simulation/electronics/cmplxIQ_params.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      677 2023-11-07 14:19:59.000000 spiakid_simulation-1.22/spiakid_simulation/electronics/data_reading.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     7406 2024-04-22 13:16:25.000000 spiakid_simulation-1.22/spiakid_simulation/electronics/filter.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    53144 2023-11-06 15:58:05.000000 spiakid_simulation-1.22/spiakid_simulation/electronics/resonator.py
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-16 12:51:41.060471 spiakid_simulation-1.22/spiakid_simulation/functions/
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-16 12:51:41.060471 spiakid_simulation-1.22/spiakid_simulation/functions/IQ/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     5250 2024-05-14 08:38:06.000000 spiakid_simulation-1.22/spiakid_simulation/functions/IQ/IQ_sim.py
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-16 12:51:41.060471 spiakid_simulation-1.22/spiakid_simulation/functions/noise/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     5029 2024-04-22 13:11:36.000000 spiakid_simulation-1.22/spiakid_simulation/functions/noise/noise.py
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-16 12:51:41.060471 spiakid_simulation-1.22/spiakid_simulation/functions/output/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     2364 2024-04-23 09:17:38.000000 spiakid_simulation-1.22/spiakid_simulation/functions/output/HDF5_creation.py
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-16 12:51:41.060471 spiakid_simulation-1.22/spiakid_simulation/functions/phase/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     1507 2024-02-07 10:11:13.000000 spiakid_simulation-1.22/spiakid_simulation/functions/phase/calib_read.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     5319 2024-04-23 08:47:14.000000 spiakid_simulation-1.22/spiakid_simulation/functions/phase/phase_conversion.py
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-16 12:51:41.064471 spiakid_simulation-1.22/spiakid_simulation/functions/photon/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     3431 2024-02-29 09:30:06.000000 spiakid_simulation-1.22/spiakid_simulation/functions/photon/black_body.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      264 2023-11-02 10:55:48.000000 spiakid_simulation-1.22/spiakid_simulation/functions/photon/contamination.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     2512 2023-10-06 09:10:32.000000 spiakid_simulation-1.22/spiakid_simulation/functions/photon/photon_gen_image.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     4578 2024-05-16 12:49:17.000000 spiakid_simulation-1.22/spiakid_simulation/functions/photon/rot.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     6572 2024-05-16 12:13:58.000000 spiakid_simulation-1.22/spiakid_simulation/functions/photon/sim_image_photon.py
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-16 12:51:41.064471 spiakid_simulation-1.22/spiakid_simulation/functions/theory/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     6198 2023-08-28 15:04:02.000000 spiakid_simulation-1.22/spiakid_simulation/functions/theory/Calc.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    14485 2023-09-18 12:50:04.000000 spiakid_simulation-1.22/spiakid_simulation/functions/theory/MKID.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    10145 2023-08-28 10:56:06.000000 spiakid_simulation-1.22/spiakid_simulation/functions/theory/SC.py
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-16 12:51:41.064471 spiakid_simulation-1.22/spiakid_simulation/functions/timeline/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     3312 2024-05-16 12:01:07.000000 spiakid_simulation-1.22/spiakid_simulation/functions/timeline/timeline.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      579 2023-08-28 10:56:06.000000 spiakid_simulation-1.22/spiakid_simulation/functions/utils.py
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-16 12:51:41.064471 spiakid_simulation-1.22/spiakid_simulation/functions/yaml/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      522 2024-02-15 12:49:21.000000 spiakid_simulation-1.22/spiakid_simulation/functions/yaml/yaml_rw.py
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-16 12:51:41.064471 spiakid_simulation-1.22/spiakid_simulation/image_process/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     2759 2024-05-13 13:42:02.000000 spiakid_simulation-1.22/spiakid_simulation/image_process/PSF_interface.py
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-16 12:51:41.064471 spiakid_simulation-1.22/spiakid_simulation/image_process/atmosphere/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    16411 2023-12-14 15:07:47.000000 spiakid_simulation-1.22/spiakid_simulation/image_process/atmosphere/interface.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    17502 2024-03-08 16:54:53.000000 spiakid_simulation-1.22/spiakid_simulation/image_process/atmosphere/interface_mult.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     1732 2023-12-14 14:48:00.000000 spiakid_simulation-1.22/spiakid_simulation/image_process/atmosphere/test_displacement.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    14479 2024-05-13 13:40:17.000000 spiakid_simulation-1.22/spiakid_simulation/image_process/atmosphere/turbulence.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     3166 2024-05-14 08:14:01.000000 spiakid_simulation-1.22/spiakid_simulation/image_process/image_generation.py
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-16 12:51:41.064471 spiakid_simulation-1.22/spiakid_simulation.egg-info/
+-rw-r--r--   0 sfaes     (4303) sfaes     (2722)     1265 2024-05-16 12:51:41.000000 spiakid_simulation-1.22/spiakid_simulation.egg-info/PKG-INFO
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     3108 2024-05-16 12:51:41.000000 spiakid_simulation-1.22/spiakid_simulation.egg-info/SOURCES.txt
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)        1 2024-05-16 12:51:41.000000 spiakid_simulation-1.22/spiakid_simulation.egg-info/dependency_links.txt
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)       69 2024-05-16 12:51:41.000000 spiakid_simulation-1.22/spiakid_simulation.egg-info/requires.txt
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)       19 2024-05-16 12:51:41.000000 spiakid_simulation-1.22/spiakid_simulation.egg-info/top_level.txt
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-16 12:51:41.064471 spiakid_simulation-1.22/test/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      157 2023-09-18 12:50:04.000000 spiakid_simulation-1.22/test/test_simu.py
```

### Comparing `spiakid_simulation-1.21/LICENSE` & `spiakid_simulation-1.22/LICENSE`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/PKG-INFO` & `spiakid_simulation-1.22/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spiakid-simulation
-Version: 1.21
+Version: 1.22
 Summary: Data simulation of SPIAKID project
 Author-email: Sebastien Faes <faesebastien@gmail.com>
 Project-URL: Homepage, https://spiakid.pages.obspm.fr/simulation/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: <=3.11
 Description-Content-Type: text/markdown
```

### Comparing `spiakid_simulation-1.21/README.md` & `spiakid_simulation-1.22/README.md`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/README_for_pip.md` & `spiakid_simulation-1.22/README_for_pip.md`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/pyproject.toml` & `spiakid_simulation-1.22/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "spiakid-simulation"
-version = "1.21"
+version = "1.22"
 authors = [
     { name="Sebastien Faes", email="faesebastien@gmail.com"}
 ]
 description = "Data simulation of SPIAKID project"
 readme = "README_for_pip.md"
 requires-python = "<=3.11"
 classifiers = [
```

### Comparing `spiakid_simulation-1.21/spiakid_simulation/Example/Calib/Wv_IQ_calib.csv` & `spiakid_simulation-1.22/spiakid_simulation/Example/Calib/Wv_IQ_calib.csv`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation/Example/Calib/Wv_ph_calib.csv` & `spiakid_simulation-1.22/spiakid_simulation/Example/Calib/Wv_ph_calib.csv`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation/Example/Sim_10obj.ipynb` & `spiakid_simulation-1.22/spiakid_simulation/Example/Sim_10obj.ipynb`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation/Example/Sim_Gaussian.ipynb` & `spiakid_simulation-1.22/spiakid_simulation/Example/Sim_Gaussian.ipynb`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation/Example/Sim_phase.ipynb` & `spiakid_simulation-1.22/spiakid_simulation/Example/Sim_phase.ipynb`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation/Example/Sim_psf.ipynb` & `spiakid_simulation-1.22/spiakid_simulation/Example/Sim_psf.ipynb`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT3750G000M025K200A000.DAT` & `spiakid_simulation-1.22/spiakid_simulation/Example/Spectrum/FT3750G000M025K200A000.DAT`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT3750G100M025K200A000.DAT` & `spiakid_simulation-1.22/spiakid_simulation/Example/Spectrum/FT3750G100M025K200A000.DAT`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT4000G050M250K200A040.DAT` & `spiakid_simulation-1.22/spiakid_simulation/Example/Spectrum/FT4000G050M250K200A040.DAT`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT4125G300M175K200A040.DAT` & `spiakid_simulation-1.22/spiakid_simulation/Example/Spectrum/FT4125G300M175K200A040.DAT`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT4500G000P050K200A000.DAT` & `spiakid_simulation-1.22/spiakid_simulation/Example/Spectrum/FT4500G000P050K200A000.DAT`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT5000G150M175K200A040.DAT` & `spiakid_simulation-1.22/spiakid_simulation/Example/Spectrum/FT5000G150M175K200A040.DAT`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT5125G350M175K200A040.DAT` & `spiakid_simulation-1.22/spiakid_simulation/Example/Spectrum/FT5125G350M175K200A040.DAT`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT5250G450M300K200A040.DAT` & `spiakid_simulation-1.22/spiakid_simulation/Example/Spectrum/FT5250G450M300K200A040.DAT`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT5875G000M075K200A020.DAT` & `spiakid_simulation-1.22/spiakid_simulation/Example/Spectrum/FT5875G000M075K200A020.DAT`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT6625G350M025K200A000.DAT` & `spiakid_simulation-1.22/spiakid_simulation/Example/Spectrum/FT6625G350M025K200A000.DAT`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT6875G450M150K200A040.DAT` & `spiakid_simulation-1.22/spiakid_simulation/Example/Spectrum/FT6875G450M150K200A040.DAT`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT7000G450M200K200A040.DAT` & `spiakid_simulation-1.22/spiakid_simulation/Example/Spectrum/FT7000G450M200K200A040.DAT`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT7000G500M050K200A020.DAT` & `spiakid_simulation-1.22/spiakid_simulation/Example/Spectrum/FT7000G500M050K200A020.DAT`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT7250G500M225K200A040.DAT` & `spiakid_simulation-1.22/spiakid_simulation/Example/Spectrum/FT7250G500M225K200A040.DAT`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation/Example/Template_10obj.yaml` & `spiakid_simulation-1.22/spiakid_simulation/Example/Template_10obj.yaml`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation/Example/Template_Gaussian.yaml` & `spiakid_simulation-1.22/spiakid_simulation/Example/Template_Gaussian.yaml`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation/Example/Template_phase.yaml` & `spiakid_simulation-1.22/spiakid_simulation/Example/Template_phase.yaml`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation/Example/Template_psf.yaml` & `spiakid_simulation-1.22/spiakid_simulation/Example/Template_psf.yaml`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation/PhotonSimulator.py` & `spiakid_simulation-1.22/spiakid_simulation/PhotonSimulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
             sky = sim_config['sky']
             
             alt = self.type_variable(sky['guide']['alt'],'altitude',[float,int]) * np.pi / 180 
             az = self.type_variable(sky['guide']['az'],'azimuth',[float,int]) * np.pi / 180
 
             rotation = self.type_variable(sky['rotation'],'rotation',[bool])
 
-
+            point_nb = self.type_variable(self.config['2-Timeline']['point_nb'],'point_nb',[int])
                 
             #   Creation of stars with their spectrum
             self.star_pos,self.star_spec = IG.image_sim(Image_size=int(pix_nbr/pix_size), object_number=nb_object, distance=distance, Path_file=path,Wavelength=wavelength_array,spectrum = spectrum,save = False)
 
             rot = np.zeros(len(self.star_pos),dtype = object)
             alt_ev = np.zeros(len(self.star_pos),dtype = object)
             
@@ -103,15 +103,15 @@
                     ang = 0
 
                     
             try: trans_Path = self.type_variable(telescope['transmittance'],'transmittance',[str])
             except: trans_Path = False
 
             #   Creation of photons
-            self.photon_list = SI.photon(wavelength_array,self.star_spec,exposure_time,tel_diam,process_nb,trans_Path)   
+            self.photon_list = SI.photon(wavelength_array,self.star_spec,exposure_time,tel_diam,point_nb,process_nb,trans_Path)   
                 
                 #   Point Source Function
             try: sim_config['PSF']
             except:
                 # print('No PSF -> Point')
                 psf_grid = np.zeros(shape = (pix_nbr,pix_nbr,len(wavelength_array)))
                 psf_grid[int(pix_nbr/2),int(pix_nbr/2),:] = 1
@@ -152,25 +152,25 @@
                 Points = np.linspace(0,1,psf_pix_nbr)
                 psf = interpolate.RegularGridInterpolator((Points,Points,wavelength_array),self.psf_visu)
       
             # Computing position of photon on the PSF 
             max_psf = []
        
             max_point = np.linspace(0,len(wavelength_array)-1,len(wavelength_array))
-            for i in range(len(max_point)): max_psf.append(np.max(self.psf_visu[:,:,i])+0.01)
+            for i in range(len(max_point)): max_psf.append(np.max(self.psf_visu[:,:,i])+0.1*np.max(self.psf_visu[:,:,i]))
             # we add 0.01 to be sure to be above
            
             interp_point = np.linspace(wavelength_array[0],wavelength_array[-1],len(wavelength_array))
             max_func = interpolate.interp1d(interp_point, max_psf)
            
             self.photon_dict_on_PSF = SI.photon_pos_on_PSF(self.star_pos, self.photon_list, psf, np.shape(self.psf_visu)[0],max_func, process_nb)
             lam0 = (max(wavelength_array)+min(wavelength_array))/2
             psf2detect = psf_pix_nbr / psf_size
          
-            self.photon_dict = SI.photon_proj(self.photon_dict_on_PSF,self.star_pos,psf2detect,rot,alt_ev,pix_nbr,pix_size,lam0)
+            self.photon_dict = SI.photon_proj(self.photon_dict_on_PSF,self.star_pos,psf2detect,rot,alt_ev,pix_nbr,pix_size,lam0,point_nb)
         
             self.wavelength, self.time = SI.detector_scale(detector_dim=detector_dim, photon_dict=self.photon_dict)
 
             # self.calib_dict = SI.photon_calib(detector_dim, [star['wavelength_array']['min'],star['wavelength_array']['max']]) 
             
 
         
@@ -182,37 +182,37 @@
                 try: self.config['3-IQ']
                 # We don't want to simulate nor the phase neither IQ
                 except: pass
                 # We want to simulate IQ
                 else:
                     #   NOT UPDATED
                     # Creation of the Timeline
-                    point_nb = self.type_variable(self.config['2-Timeline']['point_nb'],'point_nb',[int])
+                   
                     # print('Timeline creation')
                     self.photon_timeline = Tl.sorting(exposure_time,self.wavelength,point_nb,self.time, process_nb) 
                     self.photon_timeline_calib = Tl.sorting_calib(detector_dim,point_nb,[star['wavelength_array']['min'],star['wavelength_array']['max']])
                     self.IQ_Compute(obj = '3-IQ')
 
             else:
 
                 # Creation of the Timeline
-                point_nb = self.type_variable(self.config['2-Timeline']['point_nb'],'point_nb',[int])
+
               
                 self.photon_timeline = Tl.sorting(exposure_time,self.wavelength,point_nb,self.time, process_nb) 
                 self.photon_timeline_calib = Tl.sorting_calib(detector_dim,point_nb,[star['wavelength_array']['min'],star['wavelength_array']['max']])
                 # print('Phase')
-                self.phase_compute(detector_dim=detector_dim,obj = '3-Phase',timeline=self.photon_timeline, nb_process=process_nb, Filter = False)
+                self.phase_compute(detector_dim=detector_dim,obj = '3-Phase',timeline=self.photon_timeline, point_nb=point_nb, nb_process=process_nb, Filter = False)
              
             try:self.config['4-Electronic']
             except:
                 pass
             else:
                 wavelength, photon_time = np.zeros(detector_dim,dtype = float), np.zeros(detector_dim, dtype = float)
                 photon_timeline = Tl.sorting(exposure_time,wavelength,point_nb,photon_time, process_nb)
-                self.phase_compute(detector_dim=detector_dim,obj = '3-Phase',timeline=photon_timeline, nb_process=process_nb,Filter = True)
+                self.phase_compute(detector_dim=detector_dim,obj = '3-Phase',timeline=photon_timeline,point_nb=point_nb, nb_process=process_nb,Filter = True)
 
             try: self.config['5-Output']['save']
             except: pass
             else:
                 if self.type_variable(self.config['5-Output']['save'],'save',[str]) == 'Simulation':
                     # print('Saving in HDF5 at: ' + str(path))
                     hdf.save_dict_to_hdf5(self.config, path,self,pix_nbr)
@@ -220,15 +220,15 @@
                 elif self.type_variable(self.config['5-Output']['save'],'save',[str]) == 'photon_list':
                     # print('Saving the photon list at:' +str(path))
                     hdf.save_photon_list(path,self.config, self.fil_phase,self.filtered_noise,alt_az_t,ra_dec_t,self.fil_phase_calib,ang)
 
 
 
 
-    def phase_compute(self, detector_dim, obj, timeline, nb_process, Filter = False):
+    def phase_compute(self, detector_dim, obj, timeline,point_nb, nb_process, Filter = False):
 
             # Reading convertion coeff
             try: self.config[obj]['Conv_wv'] and self.config[obj]['Conv_phase']
             except: 
                 try: self.config[obj]['Calib_File']
                 except: 
                     Cr.write_csv('Calib.csv',dim = detector_dim, sep = '/')
@@ -286,15 +286,15 @@
                     else:
                         pass
                     # Filter creation
 
                     nperseg = self.type_variable(self.config['4-Electronic']['nperseg'],'nperseg',[int])
                     template_time = self.type_variable(self.config['4-Electronic']['template_time'],'template_time',[float,int])
                     trigerinx = self.type_variable(self.config['4-Electronic']['trigerinx'],'trigerinx',[int])
-                    point_nb = self.type_variable(self.config['4-Electronic']['point_nb'],'point_nb',[int])
+                    
                   
                     self.psd = Fi.psd(self.noise,nperseg)
                   
                     self.template = Fi.template(self.noise, decay=decay, template_time=template_time, trigerinx=trigerinx,point_nb=point_nb)
                 
                     self.filter = Fi.filter_creation(Noise = self.noise, template=self.template, psd=self.psd, nb_process=nb_process)
```

### Comparing `spiakid_simulation-1.21/spiakid_simulation/Simulation.py` & `spiakid_simulation-1.22/spiakid_simulation/Simulation.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation/electronics/Yaml_rw.py` & `spiakid_simulation-1.22/spiakid_simulation/electronics/Yaml_rw.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation/electronics/cmplxIQ_params.py` & `spiakid_simulation-1.22/spiakid_simulation/electronics/cmplxIQ_params.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation/electronics/data_reading.py` & `spiakid_simulation-1.22/spiakid_simulation/electronics/data_reading.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation/electronics/filter.py` & `spiakid_simulation-1.22/spiakid_simulation/electronics/filter.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation/electronics/resonator.py` & `spiakid_simulation-1.22/spiakid_simulation/electronics/resonator.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation/functions/IQ/IQ_sim.py` & `spiakid_simulation-1.22/spiakid_simulation/functions/IQ/IQ_sim.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation/functions/noise/noise.py` & `spiakid_simulation-1.22/spiakid_simulation/functions/noise/noise.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation/functions/output/HDF5_creation.py` & `spiakid_simulation-1.22/spiakid_simulation/functions/output/HDF5_creation.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation/functions/phase/calib_read.py` & `spiakid_simulation-1.22/spiakid_simulation/functions/phase/calib_read.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation/functions/phase/phase_conversion.py` & `spiakid_simulation-1.22/spiakid_simulation/functions/phase/phase_conversion.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation/functions/photon/black_body.py` & `spiakid_simulation-1.22/spiakid_simulation/functions/photon/black_body.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation/functions/photon/photon_gen_image.py` & `spiakid_simulation-1.22/spiakid_simulation/functions/photon/photon_gen_image.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation/functions/photon/rot.py` & `spiakid_simulation-1.22/spiakid_simulation/functions/photon/rot.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,17 +39,17 @@
                   [-Y0*Z0/np.sqrt((X0**2+Y0**2)*(X0**2+Y0**2+Z0**2)), -X0/np.sqrt(X0**2+Y0**2), Y0/np.sqrt(X0**2+Y0**2+Z0**2)],
                   [np.sqrt(X0**2+Y0**2)/np.sqrt((X0**2+Y0**2+Z0**2)), 0, Z0/np.sqrt(X0**2+Y0**2+Z0**2)]])
   new_pos_x = np.zeros(len(t))
   new_pos_y = np.zeros(len(t))
   alt_ev = np.zeros(len(t))
   alt_az_guide = []
   for i in range (len(t)):
-    normalisation = 2 * size
+    normalisation = 10 * size
     coo = [coo_star[1]/normalisation,coo_star[2]/normalisation]
-
+    
     z = np.sqrt(1-coo[0]**2 - coo[1]**2)
 
     coo.append(z)
     # print('coo_star: ',coo_star)
     r1_prime = np.array(coo) - np.array([0,0,1])
     # print('r1_prime:' ,r1_prime)
     r1   = R_inv@r1_prime
```

### Comparing `spiakid_simulation-1.21/spiakid_simulation/functions/photon/sim_image_photon.py` & `spiakid_simulation-1.22/spiakid_simulation/functions/photon/sim_image_photon.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,22 +12,22 @@
     spectre = spectre * wavelength * 10**-3 / (6.26*10**-34 *3*10**8) * np.pi * (diam/2)**2  * time
     nbr = spectre.max() * (wavelength[-1]-wavelength[0]) * 10**-6 
 
     return(int(nbr),spectre)
 
 
 
-def photon(wavelength,spectre,time,diam,nb_process,transmission=False):
+def photon(wavelength,spectre,time,diam,point_nb,transmission=False):
     ph = {}
 
     for st in range(len(spectre)): 
 
         ph_nbr,sp = photon_nbr(wavelength,spectre[st][:],time,diam,transmission)
         lbd = rand.uniform(low = wavelength[0],high = wavelength[-1],size = ph_nbr)
-        t=rand.uniform(low=0,high = time,size = ph_nbr)
+        t=rand.uniform(low=0,high = time*point_nb,size = ph_nbr)
         intens=rand.uniform(low = 0,high = sp.max(),size = ph_nbr)
         sp_func = interpolate.interp1d(wavelength,sp)
         pop_list = []
         dic_list = []
         for i in range(ph_nbr):
             if intens[i] > sp_func(lbd[i]):
                 pop_list.append(i)
@@ -99,23 +99,23 @@
         pool.close()
         pool.join()
         dict_photon[st] = ph_list
      
     return(dict_photon)
 
 
-def photon_proj(Photon_dict, star_pos, psf_to_detect,rot_func, alt_ev, size, FOV,lam0):
+def photon_proj(Photon_dict, star_pos, psf_to_detect,rot_func, alt_ev, size, FOV,lam0,point_nb):
     dict_photon = []
     pix_length = FOV/size
 
     for st in range(len(star_pos)):
         for ph in range(len(Photon_dict[st])):
             # Adding the star position taking account of rotation + ratio psf size to dectector size
-            x_ph, y_ph = Photon_dict[st][ph][0] / psf_to_detect + rot_func[st][0](Photon_dict[st][ph][3]), Photon_dict[st][ph][1] / psf_to_detect + rot_func[st][1](Photon_dict[st][ph][3])
-            alt = alt_ev[st](Photon_dict[st][ph][3])  # photon altitude at t
+            x_ph, y_ph = Photon_dict[st][ph][0] / psf_to_detect + rot_func[st][0](Photon_dict[st][ph][3]/point_nb), Photon_dict[st][ph][1] / psf_to_detect + rot_func[st][1](Photon_dict[st][ph][3]/point_nb)
+            alt = alt_ev[st](Photon_dict[st][ph][3]/point_nb)  # photon altitude at t
    
             DR = dispersion(np.pi/2 - alt, lam0, Photon_dict[st][ph][2])
 
             y_ph = y_ph + DR * pix_length
             dict_photon.append([x_ph,y_ph,Photon_dict[st][ph][2],Photon_dict[st][ph][3]])
     return(dict_photon)
```

### Comparing `spiakid_simulation-1.21/spiakid_simulation/functions/theory/Calc.py` & `spiakid_simulation-1.22/spiakid_simulation/functions/theory/Calc.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation/functions/theory/MKID.py` & `spiakid_simulation-1.22/spiakid_simulation/functions/theory/MKID.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation/functions/theory/SC.py` & `spiakid_simulation-1.22/spiakid_simulation/functions/theory/SC.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation/functions/timeline/timeline.py` & `spiakid_simulation-1.22/spiakid_simulation/functions/timeline/timeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,34 +23,36 @@
         signal: array
             Arrival time and wavelength of photons randomly spread
         
         """
         point_nb = int(point_nb)
        
         if type(data) == list:
-            sig = list(np.zeros([2,point_nb-len(data)]))
+            t = np.linspace(0,time,point_nb)
+            wv = np.zeros_like(t)
+            sig  = [t,wv]
+            sig[1][time_data] = data
         
-            photon_time = time_data
-            sig[0] = np.linspace(0,time,point_nb-len(data))
-            sig[0] = list(sig[0]) + list(photon_time)
-            sig[1] = list(sig[1]) + list(data)
-            signal_int = []
-            for p in range(len(sig[0])):
-                signal_int.append((sig[0][p],sig[1][p]))
-            Sorted_signal = sorted(signal_int,key=lambda x:x[0])
-            for p in range(len(sig[0])):
-                sig[0][p] = Sorted_signal[p][0]
-                sig[1][p] = Sorted_signal[p][1]
+            # sig[0] = np.linspace(0,time,point_nb-len(data))
+            # sig[0] = list(sig[0]) + list(photon_time)
+            # sig[1] = list(sig[1]) + list(data)
+            # signal_int = []
+            # for p in range(len(sig[0])):
+            #     signal_int.append((sig[0][p],sig[1][p]))
+            # Sorted_signal = sorted(signal_int,key=lambda x:x[0])
+            # for p in range(len(sig[0])):
+            #     sig[0][p] = Sorted_signal[p][0]
+            #     sig[1][p] = Sorted_signal[p][1]
         
         
         else:
              sig = list(np.zeros([2,point_nb]))
              sig[0] = np.linspace(0,time,point_nb)
-        signal[i,j] = np.array(sig)
-        return(i,j,signal[i,j])
+        # signal[i,j] = np.array(sig)
+        return(i,j,sig)
         
 
 
 def sorting(time,data,point_nb, time_data, process_nb):
     r""" Sort value according to the time on each pixel
 
         Parameters:
```

### Comparing `spiakid_simulation-1.21/spiakid_simulation/functions/utils.py` & `spiakid_simulation-1.22/spiakid_simulation/functions/utils.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation/functions/yaml/yaml_rw.py` & `spiakid_simulation-1.22/spiakid_simulation/functions/yaml/yaml_rw.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation/image_process/PSF_interface.py` & `spiakid_simulation-1.22/spiakid_simulation/image_process/PSF_interface.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation/image_process/atmosphere/interface.py` & `spiakid_simulation-1.22/spiakid_simulation/image_process/atmosphere/interface.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation/image_process/atmosphere/interface_mult.py` & `spiakid_simulation-1.22/spiakid_simulation/image_process/atmosphere/interface_mult.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation/image_process/atmosphere/test_displacement.py` & `spiakid_simulation-1.22/spiakid_simulation/image_process/atmosphere/test_displacement.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation/image_process/atmosphere/turbulence.py` & `spiakid_simulation-1.22/spiakid_simulation/image_process/atmosphere/turbulence.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation/image_process/image_generation.py` & `spiakid_simulation-1.22/spiakid_simulation/image_process/image_generation.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.21/spiakid_simulation.egg-info/PKG-INFO` & `spiakid_simulation-1.22/spiakid_simulation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spiakid-simulation
-Version: 1.21
+Version: 1.22
 Summary: Data simulation of SPIAKID project
 Author-email: Sebastien Faes <faesebastien@gmail.com>
 Project-URL: Homepage, https://spiakid.pages.obspm.fr/simulation/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: <=3.11
 Description-Content-Type: text/markdown
```

### Comparing `spiakid_simulation-1.21/spiakid_simulation.egg-info/SOURCES.txt` & `spiakid_simulation-1.22/spiakid_simulation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

