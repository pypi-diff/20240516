# Comparing `tmp/gfatpy-0.8.0.tar.gz` & `tmp/gfatpy-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gfatpy-0.8.0.tar", max compression
+gzip compressed data, was "gfatpy-0.9.0.tar", max compression
```

## Comparing `gfatpy-0.8.0.tar` & `gfatpy-0.9.0.tar`

### file list

```diff
@@ -1,117 +1,117 @@
--rw-r--r--   0        0        0     1470 2023-01-19 15:14:33.615682 gfatpy-0.8.0/LICENSE
--rw-r--r--   0        0        0     2288 2023-07-25 03:08:40.486165 gfatpy-0.8.0/gfatpy/__init__.py
--rw-r--r--   0        0        0     1077 2023-01-19 15:14:33.615682 gfatpy-0.8.0/gfatpy/aeronet/__init__.py
--rw-r--r--   0        0        0      710 2023-01-19 15:14:33.615682 gfatpy-0.8.0/gfatpy/aeronet/aeronet4lidar.py
--rw-r--r--   0        0        0     1053 2023-01-19 15:14:33.615682 gfatpy-0.8.0/gfatpy/aeronet/info.yml
--rw-r--r--   0        0        0    18417 2023-07-25 03:08:40.486165 gfatpy-0.8.0/gfatpy/aeronet/plot.py
--rw-r--r--   0        0        0     4040 2023-07-25 03:08:40.486165 gfatpy-0.8.0/gfatpy/aeronet/reader.py
--rw-r--r--   0        0        0     8855 2023-07-25 03:08:40.486165 gfatpy-0.8.0/gfatpy/aeronet/typing.py
--rw-r--r--   0        0        0    16725 2023-07-25 03:08:40.486165 gfatpy-0.8.0/gfatpy/aeronet/utils.py
--rw-r--r--   0        0        0    28725 2023-01-19 15:14:33.615682 gfatpy-0.8.0/gfatpy/assets/LOGO_GFAT_150pp.png
--rw-r--r--   0        0        0        0 2023-01-19 15:14:33.615682 gfatpy-0.8.0/gfatpy/atmo/__init__.py
--rw-r--r--   0        0        0    21888 2023-07-25 03:08:40.486165 gfatpy-0.8.0/gfatpy/atmo/atmo.py
--rw-r--r--   0        0        0     7262 2023-07-25 03:08:40.486165 gfatpy-0.8.0/gfatpy/atmo/ecmwf.py
--rw-r--r--   0        0        0    74896 2023-01-19 15:14:33.615682 gfatpy-0.8.0/gfatpy/atmo/solar.py
--rw-r--r--   0        0        0     4471 2023-07-25 03:08:40.486165 gfatpy-0.8.0/gfatpy/cli/lidar/main.py
--rw-r--r--   0        0        0     1183 2023-01-19 15:14:33.615682 gfatpy-0.8.0/gfatpy/cli/lidar/plot/main.py
--rw-r--r--   0        0        0      896 2023-01-19 15:14:33.615682 gfatpy-0.8.0/gfatpy/cli/main.py
--rw-r--r--   0        0        0      270 2023-01-19 15:14:33.615682 gfatpy-0.8.0/gfatpy/cloudnet/__init__.py
--rw-r--r--   0        0        0     8870 2023-07-25 03:08:40.486165 gfatpy-0.8.0/gfatpy/cloudnet/cloud_model.py
--rw-r--r--   0        0        0       49 2023-01-19 15:14:33.615682 gfatpy-0.8.0/gfatpy/cloudnet/info.yml
--rw-r--r--   0        0        0     4600 2023-01-19 15:14:33.615682 gfatpy-0.8.0/gfatpy/cloudnet/plot_deprecated.py
--rw-r--r--   0        0        0     5423 2023-01-19 15:14:33.615682 gfatpy-0.8.0/gfatpy/cloudnet/reader.py
--rw-r--r--   0        0        0    18077 2023-07-25 03:08:40.486165 gfatpy-0.8.0/gfatpy/cloudnet/utils.py
--rw-r--r--   0        0        0      237 2023-07-25 03:08:40.486165 gfatpy-0.8.0/gfatpy/config.py
--rw-r--r--   0        0        0      342 2023-07-25 03:08:40.486165 gfatpy-0.8.0/gfatpy/lidar/__init__.py
--rw-r--r--   0        0        0      174 2023-01-19 15:14:33.615682 gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/.hg_archival.txt
--rw-r--r--   0        0        0      121 2023-01-19 15:14:33.615682 gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/.hgignore
--rw-r--r--   0        0        0      570 2023-01-19 15:14:33.615682 gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/.hgtags
--rw-r--r--   0        0        0  2508885 2023-01-19 15:14:33.625682 gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/About the effects of polarising optics_4b_1L_corr.pdf
--rw-r--r--   0        0        0     2541 2023-01-19 15:14:33.625682 gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/CHANGELOG.md
--rw-r--r--   0        0        0   179791 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/GHK_0.9.8h_Py3.7.py
--rw-r--r--   0        0        0   793573 2023-01-19 15:14:33.625682 gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/Improvements_of_the_GHK_script_200529.pdf
--rw-r--r--   0        0        0    13468 2023-01-19 15:14:33.625682 gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/LICENSE.md
--rw-r--r--   0        0        0     1628 2023-01-19 15:14:33.625682 gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/README.md
--rw-r--r--   0        0        0      108 2023-01-19 15:14:33.625682 gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/requirements.txt
--rw-r--r--   0        0        0        0 2023-01-19 15:14:33.625682 gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/system_settings/__init__.py
--rw-r--r--   0        0        0     7453 2023-04-18 20:55:26.084565 gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/system_settings/mulhacen_polarizer_template.py
--rw-r--r--   0        0        0     7455 2023-04-18 20:55:26.084565 gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/system_settings/mulhacen_rotator_casoG_template.py
--rw-r--r--   0        0        0     7390 2023-04-18 20:55:26.084565 gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/system_settings/mulhacen_run.py
--rw-r--r--   0        0        0    11034 2023-04-18 20:55:26.084565 gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_0.9.8e4-PollyXT_Lacros.py
--rw-r--r--   0        0        0    10931 2023-04-18 20:55:26.084565 gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_0.9.8h-PollyXT_Cyprus_532_210429_vf_4.py
--rw-r--r--   0        0        0    11059 2023-01-19 15:14:33.625682 gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_mhc_pol_532x_20130101.py
--rw-r--r--   0        0        0    11059 2023-01-19 15:14:33.625682 gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_mhc_rot_532x_20130101.py
--rw-r--r--   0        0        0    11059 2023-01-19 15:14:33.625682 gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_mhc_rot_532x_20220614.py
--rw-r--r--   0        0        0     2533 2023-07-25 03:08:40.486165 gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK.py
--rw-r--r--   0        0        0    14442 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/depolarization/calibration.py
--rw-r--r--   0        0        0     1463 2023-04-01 21:13:27.762405 gfatpy-0.8.0/gfatpy/lidar/depolarization/depolarization_calibration_alh.py
--rw-r--r--   0        0        0     9744 2023-04-01 21:13:27.762405 gfatpy-0.8.0/gfatpy/lidar/depolarization/depolarization_calibration_mhc.py
--rw-r--r--   0        0        0      913 2023-04-01 21:13:27.762405 gfatpy-0.8.0/gfatpy/lidar/depolarization/depolarization_calibration_vlt.py
--rw-r--r--   0        0        0     1506 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/depolarization/io.py
--rw-r--r--   0        0        0     6044 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/depolarization/plot.py
--rw-r--r--   0        0        0    11856 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/depolarization/retrieval.py
--rw-r--r--   0        0        0     1429 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/depolarization/utils.py
--rw-r--r--   0        0        0     9911 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/file_manager.py
--rw-r--r--   0        0        0     5121 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/info.yml
--rw-r--r--   0        0        0     4072 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/nc_convert/configs/ALHAMBRA.toml
--rw-r--r--   0        0        0      920 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/nc_convert/configs/MULHACEN.toml
--rw-r--r--   0        0        0    12676 2023-07-31 14:23:15.575739 gfatpy-0.8.0/gfatpy/lidar/nc_convert/converter.py
--rw-r--r--   0        0        0      244 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/nc_convert/types.py
--rw-r--r--   0        0        0     2042 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/plot/info.yml
--rw-r--r--   0        0        0      168 2023-01-19 15:14:33.625682 gfatpy-0.8.0/gfatpy/lidar/plot/profile.py
--rw-r--r--   0        0        0     3442 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/plot/quicklook.py
--rw-r--r--   0        0        0     2299 2023-01-19 15:14:33.625682 gfatpy-0.8.0/gfatpy/lidar/preprocessing/__init__.py
--rw-r--r--   0        0        0     1931 2023-01-19 15:14:33.625682 gfatpy-0.8.0/gfatpy/lidar/preprocessing/gluing_de_la_rosa.py
--rw-r--r--   0        0        0     3364 2023-01-19 15:14:33.625682 gfatpy-0.8.0/gfatpy/lidar/preprocessing/gluing_de_la_rosa_slope.py
--rw-r--r--   0        0        0     2639 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/preprocessing/gluing_proportional.py
--rw-r--r--   0        0        0       26 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/preprocessing/lidar_dead_time.py
--rw-r--r--   0        0        0     2958 2023-01-19 15:14:33.625682 gfatpy-0.8.0/gfatpy/lidar/preprocessing/lidar_gluing_bravo_aranda.py
--rw-r--r--   0        0        0    21478 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/preprocessing/lidar_gluing_damico.py
--rw-r--r--   0        0        0     3626 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/preprocessing/lidar_linear_response_region.py
--rw-r--r--   0        0        0    17135 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/preprocessing/lidar_preprocessing.py
--rw-r--r--   0        0        0    14976 2023-01-19 15:14:33.625682 gfatpy-0.8.0/gfatpy/lidar/preprocessing/lidar_preprocessing_tools.py
--rw-r--r--   0        0        0    38037 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/preprocessing/study_dead_time.py
--rw-r--r--   0        0        0     1064 2023-01-19 15:14:33.625682 gfatpy-0.8.0/gfatpy/lidar/quality_assurance/common.py
--rw-r--r--   0        0        0        0 2023-01-19 15:14:33.625682 gfatpy-0.8.0/gfatpy/lidar/quality_assurance/dark_measurement.py
--rw-r--r--   0        0        0     5097 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/quality_assurance/io.py
--rw-r--r--   0        0        0     8242 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/quality_assurance/overlap.py
--rw-r--r--   0        0        0    10544 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/quality_assurance/plot.py
--rw-r--r--   0        0        0    10162 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/quality_assurance/rayleigh_fit.py
--rw-r--r--   0        0        0     8044 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/quality_assurance/telecover.py
--rw-r--r--   0        0        0    10850 2023-01-19 15:14:33.635682 gfatpy-0.8.0/gfatpy/lidar/reader.py
--rw-r--r--   0        0        0        0 2023-01-19 15:14:33.635682 gfatpy-0.8.0/gfatpy/lidar/retrieval/__init__.py
--rw-r--r--   0        0        0     3563 2023-01-19 15:14:33.635682 gfatpy-0.8.0/gfatpy/lidar/retrieval/helper.py
--rw-r--r--   0        0        0     6175 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/retrieval/klett.py
--rw-r--r--   0        0        0     5145 2023-01-19 15:14:33.635682 gfatpy-0.8.0/gfatpy/lidar/retrieval/lidar_layer_detection.py
--rw-r--r--   0        0        0        0 2023-01-19 15:14:33.635682 gfatpy-0.8.0/gfatpy/lidar/retrieval/number_concentration.py
--rw-r--r--   0        0        0     7009 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/retrieval/raman.py
--rw-r--r--   0        0        0     8196 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/retrieval/synthetic/generator.py
--rw-r--r--   0        0        0      563 2023-07-31 14:12:26.725658 gfatpy-0.8.0/gfatpy/lidar/scc/systems/alhambra/alhambra.py
--rw-r--r--   0        0        0      634 2023-07-31 14:12:26.725658 gfatpy-0.8.0/gfatpy/lidar/scc/systems/alhambra/alhambra_729.py
--rw-r--r--   0        0        0    10769 2023-07-31 14:12:26.725658 gfatpy-0.8.0/gfatpy/lidar/scc/systems/alhambra/alhambra_all.py
--rw-r--r--   0        0        0     2151 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/types.py
--rw-r--r--   0        0        0     6247 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/utils.py
--rw-r--r--   0        0        0      244 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/radar/__init__.py
--rw-r--r--   0        0        0      101 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/radar/info.yml
--rw-r--r--   0        0        0        0 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/radar/plot/info.yml
--rw-r--r--   0        0        0     2225 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/radar/reader.py
--rw-r--r--   0        0        0    61357 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/radar/scattering_databases/0.C_24.1GHz.csv
--rw-r--r--   0        0        0    61200 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/radar/scattering_databases/0.C_35.5GHz.csv
--rw-r--r--   0        0        0    60964 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/radar/scattering_databases/0.C_94.0GHz.csv
--rw-r--r--   0        0        0    61372 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/radar/scattering_databases/10C_24.1GHz.csv
--rw-r--r--   0        0        0    61213 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/radar/scattering_databases/10C_35.5GHz.csv
--rw-r--r--   0        0        0    60965 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/radar/scattering_databases/10C_94.0GHz.csv
--rw-r--r--   0        0        0    60528 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/radar/scattering_databases/20C_24.1GHz.csv
--rw-r--r--   0        0        0    61215 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/radar/scattering_databases/20C_35.5GHz.csv
--rw-r--r--   0        0        0    60984 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/radar/scattering_databases/20C_94.0GHz.csv
--rw-r--r--   0        0        0     1305 2023-07-25 03:08:40.506165 gfatpy-0.8.0/gfatpy/radar/types.py
--rw-r--r--   0        0        0     5853 2023-07-25 03:08:40.506165 gfatpy-0.8.0/gfatpy/radar/utils.py
--rw-r--r--   0        0        0       34 2023-01-19 15:14:33.635682 gfatpy-0.8.0/gfatpy/utils/__init__.py
--rw-r--r--   0        0        0     9655 2023-07-25 03:08:40.506165 gfatpy-0.8.0/gfatpy/utils/calibration.py
--rw-r--r--   0        0        0     3510 2023-07-31 14:23:02.085738 gfatpy-0.8.0/gfatpy/utils/io.py
--rw-r--r--   0        0        0     2870 2023-07-25 03:08:40.506165 gfatpy-0.8.0/gfatpy/utils/optimized.py
--rw-r--r--   0        0        0     6664 2023-01-19 15:14:33.635682 gfatpy-0.8.0/gfatpy/utils/plot.py
--rw-r--r--   0        0        0    13283 2023-07-25 03:08:40.506165 gfatpy-0.8.0/gfatpy/utils/utils.py
--rw-r--r--   0        0        0     1510 2023-07-31 14:23:26.055740 gfatpy-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     1892 1970-01-01 00:00:00.000000 gfatpy-0.8.0/setup.py
--rw-r--r--   0        0        0     1517 1970-01-01 00:00:00.000000 gfatpy-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1470 2023-01-19 15:14:33.615682 gfatpy-0.9.0/LICENSE
+-rw-r--r--   0        0        0     2288 2023-07-25 03:08:40.486165 gfatpy-0.9.0/gfatpy/__init__.py
+-rw-r--r--   0        0        0     1077 2023-01-19 15:14:33.615682 gfatpy-0.9.0/gfatpy/aeronet/__init__.py
+-rw-r--r--   0        0        0      710 2023-01-19 15:14:33.615682 gfatpy-0.9.0/gfatpy/aeronet/aeronet4lidar.py
+-rw-r--r--   0        0        0     1053 2023-01-19 15:14:33.615682 gfatpy-0.9.0/gfatpy/aeronet/info.yml
+-rw-r--r--   0        0        0    18417 2023-07-25 03:08:40.486165 gfatpy-0.9.0/gfatpy/aeronet/plot.py
+-rw-r--r--   0        0        0     4040 2023-07-25 03:08:40.486165 gfatpy-0.9.0/gfatpy/aeronet/reader.py
+-rw-r--r--   0        0        0     8855 2023-07-25 03:08:40.486165 gfatpy-0.9.0/gfatpy/aeronet/typing.py
+-rw-r--r--   0        0        0    16725 2023-07-25 03:08:40.486165 gfatpy-0.9.0/gfatpy/aeronet/utils.py
+-rw-r--r--   0        0        0    28725 2023-01-19 15:14:33.615682 gfatpy-0.9.0/gfatpy/assets/LOGO_GFAT_150pp.png
+-rw-r--r--   0        0        0        0 2023-01-19 15:14:33.615682 gfatpy-0.9.0/gfatpy/atmo/__init__.py
+-rw-r--r--   0        0        0    21888 2023-07-25 03:08:40.486165 gfatpy-0.9.0/gfatpy/atmo/atmo.py
+-rw-r--r--   0        0        0     7262 2023-07-25 03:08:40.486165 gfatpy-0.9.0/gfatpy/atmo/ecmwf.py
+-rw-r--r--   0        0        0    74896 2023-01-19 15:14:33.615682 gfatpy-0.9.0/gfatpy/atmo/solar.py
+-rw-r--r--   0        0        0     4471 2023-07-25 03:08:40.486165 gfatpy-0.9.0/gfatpy/cli/lidar/main.py
+-rw-r--r--   0        0        0     1183 2023-01-19 15:14:33.615682 gfatpy-0.9.0/gfatpy/cli/lidar/plot/main.py
+-rw-r--r--   0        0        0      896 2023-01-19 15:14:33.615682 gfatpy-0.9.0/gfatpy/cli/main.py
+-rw-r--r--   0        0        0      270 2023-01-19 15:14:33.615682 gfatpy-0.9.0/gfatpy/cloudnet/__init__.py
+-rw-r--r--   0        0        0     8870 2023-07-25 03:08:40.486165 gfatpy-0.9.0/gfatpy/cloudnet/cloud_model.py
+-rw-r--r--   0        0        0       49 2023-01-19 15:14:33.615682 gfatpy-0.9.0/gfatpy/cloudnet/info.yml
+-rw-r--r--   0        0        0     4600 2023-01-19 15:14:33.615682 gfatpy-0.9.0/gfatpy/cloudnet/plot_deprecated.py
+-rw-r--r--   0        0        0     5423 2023-01-19 15:14:33.615682 gfatpy-0.9.0/gfatpy/cloudnet/reader.py
+-rw-r--r--   0        0        0    18077 2023-07-25 03:08:40.486165 gfatpy-0.9.0/gfatpy/cloudnet/utils.py
+-rw-r--r--   0        0        0      237 2023-07-25 03:08:40.486165 gfatpy-0.9.0/gfatpy/config.py
+-rw-r--r--   0        0        0      342 2023-07-25 03:08:40.486165 gfatpy-0.9.0/gfatpy/lidar/__init__.py
+-rw-r--r--   0        0        0      174 2023-01-19 15:14:33.615682 gfatpy-0.9.0/gfatpy/lidar/depolarization/GHK/.hg_archival.txt
+-rw-r--r--   0        0        0      121 2023-01-19 15:14:33.615682 gfatpy-0.9.0/gfatpy/lidar/depolarization/GHK/.hgignore
+-rw-r--r--   0        0        0      570 2023-01-19 15:14:33.615682 gfatpy-0.9.0/gfatpy/lidar/depolarization/GHK/.hgtags
+-rw-r--r--   0        0        0  2508885 2023-01-19 15:14:33.625682 gfatpy-0.9.0/gfatpy/lidar/depolarization/GHK/About the effects of polarising optics_4b_1L_corr.pdf
+-rw-r--r--   0        0        0     2541 2023-01-19 15:14:33.625682 gfatpy-0.9.0/gfatpy/lidar/depolarization/GHK/CHANGELOG.md
+-rw-r--r--   0        0        0   179791 2023-07-25 03:08:40.496165 gfatpy-0.9.0/gfatpy/lidar/depolarization/GHK/GHK_0.9.8h_Py3.7.py
+-rw-r--r--   0        0        0   793573 2023-01-19 15:14:33.625682 gfatpy-0.9.0/gfatpy/lidar/depolarization/GHK/Improvements_of_the_GHK_script_200529.pdf
+-rw-r--r--   0        0        0    13468 2023-01-19 15:14:33.625682 gfatpy-0.9.0/gfatpy/lidar/depolarization/GHK/LICENSE.md
+-rw-r--r--   0        0        0     1628 2023-01-19 15:14:33.625682 gfatpy-0.9.0/gfatpy/lidar/depolarization/GHK/README.md
+-rw-r--r--   0        0        0      108 2023-01-19 15:14:33.625682 gfatpy-0.9.0/gfatpy/lidar/depolarization/GHK/requirements.txt
+-rw-r--r--   0        0        0        0 2023-01-19 15:14:33.625682 gfatpy-0.9.0/gfatpy/lidar/depolarization/GHK/system_settings/__init__.py
+-rw-r--r--   0        0        0     7453 2023-04-18 20:55:26.084565 gfatpy-0.9.0/gfatpy/lidar/depolarization/GHK/system_settings/mulhacen_polarizer_template.py
+-rw-r--r--   0        0        0     7455 2023-04-18 20:55:26.084565 gfatpy-0.9.0/gfatpy/lidar/depolarization/GHK/system_settings/mulhacen_rotator_casoG_template.py
+-rw-r--r--   0        0        0     7390 2023-04-18 20:55:26.084565 gfatpy-0.9.0/gfatpy/lidar/depolarization/GHK/system_settings/mulhacen_run.py
+-rw-r--r--   0        0        0    11034 2023-04-18 20:55:26.084565 gfatpy-0.9.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_0.9.8e4-PollyXT_Lacros.py
+-rw-r--r--   0        0        0    10931 2023-04-18 20:55:26.084565 gfatpy-0.9.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_0.9.8h-PollyXT_Cyprus_532_210429_vf_4.py
+-rw-r--r--   0        0        0    11059 2023-01-19 15:14:33.625682 gfatpy-0.9.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_mhc_pol_532x_20130101.py
+-rw-r--r--   0        0        0    11059 2023-01-19 15:14:33.625682 gfatpy-0.9.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_mhc_rot_532x_20130101.py
+-rw-r--r--   0        0        0    11059 2023-01-19 15:14:33.625682 gfatpy-0.9.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_mhc_rot_532x_20220614.py
+-rw-r--r--   0        0        0     2533 2023-07-25 03:08:40.486165 gfatpy-0.9.0/gfatpy/lidar/depolarization/GHK.py
+-rw-r--r--   0        0        0    14442 2023-07-25 03:08:40.496165 gfatpy-0.9.0/gfatpy/lidar/depolarization/calibration.py
+-rw-r--r--   0        0        0     1463 2023-04-01 21:13:27.762405 gfatpy-0.9.0/gfatpy/lidar/depolarization/depolarization_calibration_alh.py
+-rw-r--r--   0        0        0     9744 2023-04-01 21:13:27.762405 gfatpy-0.9.0/gfatpy/lidar/depolarization/depolarization_calibration_mhc.py
+-rw-r--r--   0        0        0      913 2023-04-01 21:13:27.762405 gfatpy-0.9.0/gfatpy/lidar/depolarization/depolarization_calibration_vlt.py
+-rw-r--r--   0        0        0     1506 2023-07-25 03:08:40.496165 gfatpy-0.9.0/gfatpy/lidar/depolarization/io.py
+-rw-r--r--   0        0        0     6044 2023-07-25 03:08:40.496165 gfatpy-0.9.0/gfatpy/lidar/depolarization/plot.py
+-rw-r--r--   0        0        0    11856 2023-07-25 03:08:40.496165 gfatpy-0.9.0/gfatpy/lidar/depolarization/retrieval.py
+-rw-r--r--   0        0        0     1429 2023-07-25 03:08:40.496165 gfatpy-0.9.0/gfatpy/lidar/depolarization/utils.py
+-rw-r--r--   0        0        0     9911 2023-07-25 03:08:40.496165 gfatpy-0.9.0/gfatpy/lidar/file_manager.py
+-rw-r--r--   0        0        0     5121 2023-07-25 03:08:40.496165 gfatpy-0.9.0/gfatpy/lidar/info.yml
+-rw-r--r--   0        0        0     4072 2023-07-25 03:08:40.496165 gfatpy-0.9.0/gfatpy/lidar/nc_convert/configs/ALHAMBRA.toml
+-rw-r--r--   0        0        0      920 2023-07-25 03:08:40.496165 gfatpy-0.9.0/gfatpy/lidar/nc_convert/configs/MULHACEN.toml
+-rw-r--r--   0        0        0    12690 2023-07-31 22:27:47.376514 gfatpy-0.9.0/gfatpy/lidar/nc_convert/converter.py
+-rw-r--r--   0        0        0      244 2023-07-25 03:08:40.496165 gfatpy-0.9.0/gfatpy/lidar/nc_convert/types.py
+-rw-r--r--   0        0        0     2042 2023-07-25 03:08:40.496165 gfatpy-0.9.0/gfatpy/lidar/plot/info.yml
+-rw-r--r--   0        0        0      168 2023-01-19 15:14:33.625682 gfatpy-0.9.0/gfatpy/lidar/plot/profile.py
+-rw-r--r--   0        0        0     3442 2023-07-25 03:08:40.496165 gfatpy-0.9.0/gfatpy/lidar/plot/quicklook.py
+-rw-r--r--   0        0        0     2299 2023-01-19 15:14:33.625682 gfatpy-0.9.0/gfatpy/lidar/preprocessing/__init__.py
+-rw-r--r--   0        0        0     1931 2023-01-19 15:14:33.625682 gfatpy-0.9.0/gfatpy/lidar/preprocessing/gluing_de_la_rosa.py
+-rw-r--r--   0        0        0     3364 2023-01-19 15:14:33.625682 gfatpy-0.9.0/gfatpy/lidar/preprocessing/gluing_de_la_rosa_slope.py
+-rw-r--r--   0        0        0     2639 2023-07-25 03:08:40.496165 gfatpy-0.9.0/gfatpy/lidar/preprocessing/gluing_proportional.py
+-rw-r--r--   0        0        0       26 2023-07-25 03:08:40.496165 gfatpy-0.9.0/gfatpy/lidar/preprocessing/lidar_dead_time.py
+-rw-r--r--   0        0        0     2958 2023-01-19 15:14:33.625682 gfatpy-0.9.0/gfatpy/lidar/preprocessing/lidar_gluing_bravo_aranda.py
+-rw-r--r--   0        0        0    21478 2023-07-25 03:08:40.496165 gfatpy-0.9.0/gfatpy/lidar/preprocessing/lidar_gluing_damico.py
+-rw-r--r--   0        0        0     3626 2023-07-25 03:08:40.496165 gfatpy-0.9.0/gfatpy/lidar/preprocessing/lidar_linear_response_region.py
+-rw-r--r--   0        0        0    17135 2023-07-25 03:08:40.496165 gfatpy-0.9.0/gfatpy/lidar/preprocessing/lidar_preprocessing.py
+-rw-r--r--   0        0        0    14976 2023-01-19 15:14:33.625682 gfatpy-0.9.0/gfatpy/lidar/preprocessing/lidar_preprocessing_tools.py
+-rw-r--r--   0        0        0    38037 2023-07-25 03:08:40.496165 gfatpy-0.9.0/gfatpy/lidar/preprocessing/study_dead_time.py
+-rw-r--r--   0        0        0     1064 2023-01-19 15:14:33.625682 gfatpy-0.9.0/gfatpy/lidar/quality_assurance/common.py
+-rw-r--r--   0        0        0        0 2023-01-19 15:14:33.625682 gfatpy-0.9.0/gfatpy/lidar/quality_assurance/dark_measurement.py
+-rw-r--r--   0        0        0     5097 2023-07-25 03:08:40.496165 gfatpy-0.9.0/gfatpy/lidar/quality_assurance/io.py
+-rw-r--r--   0        0        0     8242 2023-07-25 03:08:40.496165 gfatpy-0.9.0/gfatpy/lidar/quality_assurance/overlap.py
+-rw-r--r--   0        0        0    10544 2023-07-25 03:08:40.496165 gfatpy-0.9.0/gfatpy/lidar/quality_assurance/plot.py
+-rw-r--r--   0        0        0    10162 2023-07-25 03:08:40.496165 gfatpy-0.9.0/gfatpy/lidar/quality_assurance/rayleigh_fit.py
+-rw-r--r--   0        0        0     8044 2023-07-25 03:08:40.496165 gfatpy-0.9.0/gfatpy/lidar/quality_assurance/telecover.py
+-rw-r--r--   0        0        0    10850 2023-01-19 15:14:33.635682 gfatpy-0.9.0/gfatpy/lidar/reader.py
+-rw-r--r--   0        0        0        0 2023-01-19 15:14:33.635682 gfatpy-0.9.0/gfatpy/lidar/retrieval/__init__.py
+-rw-r--r--   0        0        0     3563 2023-01-19 15:14:33.635682 gfatpy-0.9.0/gfatpy/lidar/retrieval/helper.py
+-rw-r--r--   0        0        0     6175 2023-07-25 03:08:40.496165 gfatpy-0.9.0/gfatpy/lidar/retrieval/klett.py
+-rw-r--r--   0        0        0     5145 2023-01-19 15:14:33.635682 gfatpy-0.9.0/gfatpy/lidar/retrieval/lidar_layer_detection.py
+-rw-r--r--   0        0        0        0 2023-01-19 15:14:33.635682 gfatpy-0.9.0/gfatpy/lidar/retrieval/number_concentration.py
+-rw-r--r--   0        0        0     7009 2023-07-25 03:08:40.496165 gfatpy-0.9.0/gfatpy/lidar/retrieval/raman.py
+-rw-r--r--   0        0        0     8196 2023-07-25 03:08:40.496165 gfatpy-0.9.0/gfatpy/lidar/retrieval/synthetic/generator.py
+-rw-r--r--   0        0        0      563 2023-07-31 14:12:26.725658 gfatpy-0.9.0/gfatpy/lidar/scc/systems/alhambra/alhambra.py
+-rw-r--r--   0        0        0      634 2023-07-31 14:12:26.725658 gfatpy-0.9.0/gfatpy/lidar/scc/systems/alhambra/alhambra_729.py
+-rw-r--r--   0        0        0    10769 2023-07-31 14:12:26.725658 gfatpy-0.9.0/gfatpy/lidar/scc/systems/alhambra/alhambra_all.py
+-rw-r--r--   0        0        0     2151 2023-07-25 03:08:40.496165 gfatpy-0.9.0/gfatpy/lidar/types.py
+-rw-r--r--   0        0        0     6247 2023-07-25 03:08:40.496165 gfatpy-0.9.0/gfatpy/lidar/utils.py
+-rw-r--r--   0        0        0      244 2023-07-25 03:08:40.496165 gfatpy-0.9.0/gfatpy/radar/__init__.py
+-rw-r--r--   0        0        0      101 2023-07-25 03:08:40.496165 gfatpy-0.9.0/gfatpy/radar/info.yml
+-rw-r--r--   0        0        0        0 2023-07-25 03:08:40.496165 gfatpy-0.9.0/gfatpy/radar/plot/info.yml
+-rw-r--r--   0        0        0     2225 2023-07-25 03:08:40.496165 gfatpy-0.9.0/gfatpy/radar/reader.py
+-rw-r--r--   0        0        0    61357 2023-07-25 03:08:40.496165 gfatpy-0.9.0/gfatpy/radar/scattering_databases/0.C_24.1GHz.csv
+-rw-r--r--   0        0        0    61200 2023-07-25 03:08:40.496165 gfatpy-0.9.0/gfatpy/radar/scattering_databases/0.C_35.5GHz.csv
+-rw-r--r--   0        0        0    60964 2023-07-25 03:08:40.496165 gfatpy-0.9.0/gfatpy/radar/scattering_databases/0.C_94.0GHz.csv
+-rw-r--r--   0        0        0    61372 2023-07-25 03:08:40.496165 gfatpy-0.9.0/gfatpy/radar/scattering_databases/10C_24.1GHz.csv
+-rw-r--r--   0        0        0    61213 2023-07-25 03:08:40.496165 gfatpy-0.9.0/gfatpy/radar/scattering_databases/10C_35.5GHz.csv
+-rw-r--r--   0        0        0    60965 2023-07-25 03:08:40.496165 gfatpy-0.9.0/gfatpy/radar/scattering_databases/10C_94.0GHz.csv
+-rw-r--r--   0        0        0    60528 2023-07-25 03:08:40.496165 gfatpy-0.9.0/gfatpy/radar/scattering_databases/20C_24.1GHz.csv
+-rw-r--r--   0        0        0    61215 2023-07-25 03:08:40.496165 gfatpy-0.9.0/gfatpy/radar/scattering_databases/20C_35.5GHz.csv
+-rw-r--r--   0        0        0    60984 2023-07-25 03:08:40.496165 gfatpy-0.9.0/gfatpy/radar/scattering_databases/20C_94.0GHz.csv
+-rw-r--r--   0        0        0     1305 2023-07-25 03:08:40.506165 gfatpy-0.9.0/gfatpy/radar/types.py
+-rw-r--r--   0        0        0     5853 2023-07-25 03:08:40.506165 gfatpy-0.9.0/gfatpy/radar/utils.py
+-rw-r--r--   0        0        0       34 2023-01-19 15:14:33.635682 gfatpy-0.9.0/gfatpy/utils/__init__.py
+-rw-r--r--   0        0        0     9655 2023-07-25 03:08:40.506165 gfatpy-0.9.0/gfatpy/utils/calibration.py
+-rw-r--r--   0        0        0     3510 2023-07-31 14:23:02.085738 gfatpy-0.9.0/gfatpy/utils/io.py
+-rw-r--r--   0        0        0     2870 2023-07-25 03:08:40.506165 gfatpy-0.9.0/gfatpy/utils/optimized.py
+-rw-r--r--   0        0        0     6664 2023-01-19 15:14:33.635682 gfatpy-0.9.0/gfatpy/utils/plot.py
+-rw-r--r--   0        0        0    13283 2023-07-25 03:08:40.506165 gfatpy-0.9.0/gfatpy/utils/utils.py
+-rw-r--r--   0        0        0     1510 2023-07-31 22:28:01.086512 gfatpy-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1892 1970-01-01 00:00:00.000000 gfatpy-0.9.0/setup.py
+-rw-r--r--   0        0        0     1517 1970-01-01 00:00:00.000000 gfatpy-0.9.0/PKG-INFO
```

### Comparing `gfatpy-0.8.0/LICENSE` & `gfatpy-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/__init__.py` & `gfatpy-0.9.0/gfatpy/__init__.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/aeronet/__init__.py` & `gfatpy-0.9.0/gfatpy/aeronet/__init__.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/aeronet/aeronet4lidar.py` & `gfatpy-0.9.0/gfatpy/aeronet/aeronet4lidar.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/aeronet/info.yml` & `gfatpy-0.9.0/gfatpy/aeronet/info.yml`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/aeronet/plot.py` & `gfatpy-0.9.0/gfatpy/aeronet/plot.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/aeronet/reader.py` & `gfatpy-0.9.0/gfatpy/aeronet/reader.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/aeronet/typing.py` & `gfatpy-0.9.0/gfatpy/aeronet/typing.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/aeronet/utils.py` & `gfatpy-0.9.0/gfatpy/aeronet/utils.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/assets/LOGO_GFAT_150pp.png` & `gfatpy-0.9.0/gfatpy/assets/LOGO_GFAT_150pp.png`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/atmo/atmo.py` & `gfatpy-0.9.0/gfatpy/atmo/atmo.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/atmo/ecmwf.py` & `gfatpy-0.9.0/gfatpy/atmo/ecmwf.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/atmo/solar.py` & `gfatpy-0.9.0/gfatpy/atmo/solar.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/cli/lidar/main.py` & `gfatpy-0.9.0/gfatpy/cli/lidar/main.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/cli/lidar/plot/main.py` & `gfatpy-0.9.0/gfatpy/cli/lidar/plot/main.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/cli/main.py` & `gfatpy-0.9.0/gfatpy/cli/main.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/cloudnet/cloud_model.py` & `gfatpy-0.9.0/gfatpy/cloudnet/cloud_model.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/cloudnet/plot_deprecated.py` & `gfatpy-0.9.0/gfatpy/cloudnet/plot_deprecated.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/cloudnet/reader.py` & `gfatpy-0.9.0/gfatpy/cloudnet/reader.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/cloudnet/utils.py` & `gfatpy-0.9.0/gfatpy/cloudnet/utils.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/.hgtags` & `gfatpy-0.9.0/gfatpy/lidar/depolarization/GHK/.hgtags`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/About the effects of polarising optics_4b_1L_corr.pdf` & `gfatpy-0.9.0/gfatpy/lidar/depolarization/GHK/About the effects of polarising optics_4b_1L_corr.pdf`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/CHANGELOG.md` & `gfatpy-0.9.0/gfatpy/lidar/depolarization/GHK/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/GHK_0.9.8h_Py3.7.py` & `gfatpy-0.9.0/gfatpy/lidar/depolarization/GHK/GHK_0.9.8h_Py3.7.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/Improvements_of_the_GHK_script_200529.pdf` & `gfatpy-0.9.0/gfatpy/lidar/depolarization/GHK/Improvements_of_the_GHK_script_200529.pdf`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/LICENSE.md` & `gfatpy-0.9.0/gfatpy/lidar/depolarization/GHK/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/README.md` & `gfatpy-0.9.0/gfatpy/lidar/depolarization/GHK/README.md`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/system_settings/mulhacen_polarizer_template.py` & `gfatpy-0.9.0/gfatpy/lidar/depolarization/GHK/system_settings/mulhacen_polarizer_template.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/system_settings/mulhacen_rotator_casoG_template.py` & `gfatpy-0.9.0/gfatpy/lidar/depolarization/GHK/system_settings/mulhacen_rotator_casoG_template.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/system_settings/mulhacen_run.py` & `gfatpy-0.9.0/gfatpy/lidar/depolarization/GHK/system_settings/mulhacen_run.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_0.9.8e4-PollyXT_Lacros.py` & `gfatpy-0.9.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_0.9.8e4-PollyXT_Lacros.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_0.9.8h-PollyXT_Cyprus_532_210429_vf_4.py` & `gfatpy-0.9.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_0.9.8h-PollyXT_Cyprus_532_210429_vf_4.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_mhc_pol_532x_20130101.py` & `gfatpy-0.9.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_mhc_pol_532x_20130101.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_mhc_rot_532x_20130101.py` & `gfatpy-0.9.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_mhc_rot_532x_20130101.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_mhc_rot_532x_20220614.py` & `gfatpy-0.9.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_mhc_rot_532x_20220614.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK.py` & `gfatpy-0.9.0/gfatpy/lidar/depolarization/GHK.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/depolarization/calibration.py` & `gfatpy-0.9.0/gfatpy/lidar/depolarization/calibration.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/depolarization/depolarization_calibration_alh.py` & `gfatpy-0.9.0/gfatpy/lidar/depolarization/depolarization_calibration_alh.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/depolarization/depolarization_calibration_mhc.py` & `gfatpy-0.9.0/gfatpy/lidar/depolarization/depolarization_calibration_mhc.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/depolarization/depolarization_calibration_vlt.py` & `gfatpy-0.9.0/gfatpy/lidar/depolarization/depolarization_calibration_vlt.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/depolarization/io.py` & `gfatpy-0.9.0/gfatpy/lidar/depolarization/io.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/depolarization/plot.py` & `gfatpy-0.9.0/gfatpy/lidar/depolarization/plot.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/depolarization/retrieval.py` & `gfatpy-0.9.0/gfatpy/lidar/depolarization/retrieval.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/depolarization/utils.py` & `gfatpy-0.9.0/gfatpy/lidar/depolarization/utils.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/file_manager.py` & `gfatpy-0.9.0/gfatpy/lidar/file_manager.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/info.yml` & `gfatpy-0.9.0/gfatpy/lidar/info.yml`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/nc_convert/configs/ALHAMBRA.toml` & `gfatpy-0.9.0/gfatpy/lidar/nc_convert/configs/ALHAMBRA.toml`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/nc_convert/configs/MULHACEN.toml` & `gfatpy-0.9.0/gfatpy/lidar/nc_convert/configs/MULHACEN.toml`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/nc_convert/converter.py` & `gfatpy-0.9.0/gfatpy/lidar/nc_convert/converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,15 +241,15 @@
         config_path = Path(opt_config)
         if not config_path.exists():
             try_last_chance = True
     elif opt_config is None:
         try_last_chance = True
 
     if try_last_chance:
-        config_path = Path(CONFIGS_DIR / f"{lidar_name}.toml")
+        config_path = Path(CONFIGS_DIR / f"{lidar_name.value.upper()}.toml")
     else:
         raise FileNotFoundError(f"No configution file found in {opt_config}")
 
     if not config_path.exists():
         raise FileNotFoundError(f"No configution file found in {opt_config}")
 
     return get_config(config_path)
```

### Comparing `gfatpy-0.8.0/gfatpy/lidar/plot/info.yml` & `gfatpy-0.9.0/gfatpy/lidar/plot/info.yml`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/plot/quicklook.py` & `gfatpy-0.9.0/gfatpy/lidar/plot/quicklook.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/preprocessing/__init__.py` & `gfatpy-0.9.0/gfatpy/lidar/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/preprocessing/gluing_de_la_rosa.py` & `gfatpy-0.9.0/gfatpy/lidar/preprocessing/gluing_de_la_rosa.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/preprocessing/gluing_de_la_rosa_slope.py` & `gfatpy-0.9.0/gfatpy/lidar/preprocessing/gluing_de_la_rosa_slope.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/preprocessing/gluing_proportional.py` & `gfatpy-0.9.0/gfatpy/lidar/preprocessing/gluing_proportional.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/preprocessing/lidar_gluing_bravo_aranda.py` & `gfatpy-0.9.0/gfatpy/lidar/preprocessing/lidar_gluing_bravo_aranda.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/preprocessing/lidar_gluing_damico.py` & `gfatpy-0.9.0/gfatpy/lidar/preprocessing/lidar_gluing_damico.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/preprocessing/lidar_linear_response_region.py` & `gfatpy-0.9.0/gfatpy/lidar/preprocessing/lidar_linear_response_region.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/preprocessing/lidar_preprocessing.py` & `gfatpy-0.9.0/gfatpy/lidar/preprocessing/lidar_preprocessing.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/preprocessing/lidar_preprocessing_tools.py` & `gfatpy-0.9.0/gfatpy/lidar/preprocessing/lidar_preprocessing_tools.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/preprocessing/study_dead_time.py` & `gfatpy-0.9.0/gfatpy/lidar/preprocessing/study_dead_time.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/quality_assurance/common.py` & `gfatpy-0.9.0/gfatpy/lidar/quality_assurance/common.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/quality_assurance/io.py` & `gfatpy-0.9.0/gfatpy/lidar/quality_assurance/io.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/quality_assurance/overlap.py` & `gfatpy-0.9.0/gfatpy/lidar/quality_assurance/overlap.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/quality_assurance/plot.py` & `gfatpy-0.9.0/gfatpy/lidar/quality_assurance/plot.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/quality_assurance/rayleigh_fit.py` & `gfatpy-0.9.0/gfatpy/lidar/quality_assurance/rayleigh_fit.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/quality_assurance/telecover.py` & `gfatpy-0.9.0/gfatpy/lidar/quality_assurance/telecover.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/reader.py` & `gfatpy-0.9.0/gfatpy/lidar/reader.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/retrieval/helper.py` & `gfatpy-0.9.0/gfatpy/lidar/retrieval/helper.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/retrieval/klett.py` & `gfatpy-0.9.0/gfatpy/lidar/retrieval/klett.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/retrieval/lidar_layer_detection.py` & `gfatpy-0.9.0/gfatpy/lidar/retrieval/lidar_layer_detection.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/retrieval/raman.py` & `gfatpy-0.9.0/gfatpy/lidar/retrieval/raman.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/retrieval/synthetic/generator.py` & `gfatpy-0.9.0/gfatpy/lidar/retrieval/synthetic/generator.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/scc/systems/alhambra/alhambra.py` & `gfatpy-0.9.0/gfatpy/lidar/scc/systems/alhambra/alhambra.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/scc/systems/alhambra/alhambra_729.py` & `gfatpy-0.9.0/gfatpy/lidar/scc/systems/alhambra/alhambra_729.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/scc/systems/alhambra/alhambra_all.py` & `gfatpy-0.9.0/gfatpy/lidar/scc/systems/alhambra/alhambra_all.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/types.py` & `gfatpy-0.9.0/gfatpy/lidar/types.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/lidar/utils.py` & `gfatpy-0.9.0/gfatpy/lidar/utils.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/radar/reader.py` & `gfatpy-0.9.0/gfatpy/radar/reader.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/radar/scattering_databases/0.C_24.1GHz.csv` & `gfatpy-0.9.0/gfatpy/radar/scattering_databases/0.C_24.1GHz.csv`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/radar/scattering_databases/0.C_35.5GHz.csv` & `gfatpy-0.9.0/gfatpy/radar/scattering_databases/0.C_35.5GHz.csv`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/radar/scattering_databases/0.C_94.0GHz.csv` & `gfatpy-0.9.0/gfatpy/radar/scattering_databases/0.C_94.0GHz.csv`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/radar/scattering_databases/10C_24.1GHz.csv` & `gfatpy-0.9.0/gfatpy/radar/scattering_databases/10C_24.1GHz.csv`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/radar/scattering_databases/10C_35.5GHz.csv` & `gfatpy-0.9.0/gfatpy/radar/scattering_databases/10C_35.5GHz.csv`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/radar/scattering_databases/10C_94.0GHz.csv` & `gfatpy-0.9.0/gfatpy/radar/scattering_databases/10C_94.0GHz.csv`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/radar/scattering_databases/20C_24.1GHz.csv` & `gfatpy-0.9.0/gfatpy/radar/scattering_databases/20C_24.1GHz.csv`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/radar/scattering_databases/20C_35.5GHz.csv` & `gfatpy-0.9.0/gfatpy/radar/scattering_databases/20C_35.5GHz.csv`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/radar/scattering_databases/20C_94.0GHz.csv` & `gfatpy-0.9.0/gfatpy/radar/scattering_databases/20C_94.0GHz.csv`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/radar/types.py` & `gfatpy-0.9.0/gfatpy/radar/types.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/radar/utils.py` & `gfatpy-0.9.0/gfatpy/radar/utils.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/utils/calibration.py` & `gfatpy-0.9.0/gfatpy/utils/calibration.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/utils/io.py` & `gfatpy-0.9.0/gfatpy/utils/io.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/utils/optimized.py` & `gfatpy-0.9.0/gfatpy/utils/optimized.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/utils/plot.py` & `gfatpy-0.9.0/gfatpy/utils/plot.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/gfatpy/utils/utils.py` & `gfatpy-0.9.0/gfatpy/utils/utils.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.8.0/pyproject.toml` & `gfatpy-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gfatpy"
-version = "0.8.0"
+version = "0.9.0"
 description = "A python package for GFAT utilities"
 # Can be extended to multiple authors
 authors = [
     "Juan Diego De la Rosa <jdidelarc@gmail.com>"
 ]
 classifiers = [
     "Intended Audience :: Science/Research",
```

### Comparing `gfatpy-0.8.0/setup.py` & `gfatpy-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 {'docs': ['pdoc>=12.0.2,<13.0.0']}
 
 entry_points = \
 {'console_scripts': ['gfatpy = gfatpy.cli.main:app']}
 
 setup_kwargs = {
     'name': 'gfatpy',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'A python package for GFAT utilities',
     'long_description': 'None',
     'author': 'Juan Diego De la Rosa',
     'author_email': 'jdidelarc@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `gfatpy-0.8.0/PKG-INFO` & `gfatpy-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gfatpy
-Version: 0.8.0
+Version: 0.9.0
 Summary: A python package for GFAT utilities
 Author: Juan Diego De la Rosa
 Author-email: jdidelarc@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

