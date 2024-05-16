# Comparing `tmp/methodicconfigurator-0.6.0.tar.gz` & `tmp/methodicconfigurator-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "methodicconfigurator-0.6.0.tar", last modified: Thu May 16 10:33:01 2024, max compression
+gzip compressed data, was "methodicconfigurator-0.6.1.tar", last modified: Thu May 16 12:17:07 2024, max compression
```

## Comparing `methodicconfigurator-0.6.0.tar` & `methodicconfigurator-0.6.1.tar`

### file list

```diff
@@ -1,309 +1,309 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:33:01.317068 methodicconfigurator-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35823 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:33:01.257068 methodicconfigurator-0.6.0/MethodicConfigurator/
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/MethodicConfigurator/ArduPilot_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)    26216 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/MethodicConfigurator/ArduPilot_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/MethodicConfigurator/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    27852 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/MethodicConfigurator/annotate_params.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4993 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/MethodicConfigurator/ardupilot_methodic_configurator.py
--rw-r--r--   0 runner    (1001) docker     (127)    29041 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/MethodicConfigurator/backend_filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/MethodicConfigurator/backend_filesystem_configuration_steps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/MethodicConfigurator/backend_filesystem_vehicle_components.py
--rw-r--r--   0 runner    (1001) docker     (127)    31001 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/MethodicConfigurator/backend_flightcontroller.py
--rw-r--r--   0 runner    (1001) docker     (127)    26774 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/MethodicConfigurator/backend_mavftp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/MethodicConfigurator/battery_cell_voltages.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/MethodicConfigurator/common_arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     8259 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/MethodicConfigurator/extract_param_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)    13811 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/MethodicConfigurator/frontend_tkinter_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    18042 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/MethodicConfigurator/frontend_tkinter_component_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/MethodicConfigurator/frontend_tkinter_component_editor_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    14736 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/MethodicConfigurator/frontend_tkinter_connection_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)    20140 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/MethodicConfigurator/frontend_tkinter_directory_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)    37652 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/MethodicConfigurator/frontend_tkinter_parameter_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)    27018 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/MethodicConfigurator/frontend_tkinter_parameter_editor_table.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2468 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/MethodicConfigurator/get_release_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/MethodicConfigurator/param_ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)     9757 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/MethodicConfigurator/param_pid_adjustment_update.py
--rw-r--r--   0 runner    (1001) docker     (127)    22803 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/MethodicConfigurator/tempcal_imu.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/MethodicConfigurator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:33:01.317068 methodicconfigurator-0.6.0/MethodicConfigurator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-16 10:33:01.000000 methodicconfigurator-0.6.0/MethodicConfigurator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23766 2024-05-16 10:33:01.000000 methodicconfigurator-0.6.0/MethodicConfigurator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 10:33:01.000000 methodicconfigurator-0.6.0/MethodicConfigurator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-16 10:33:01.000000 methodicconfigurator-0.6.0/MethodicConfigurator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-16 10:33:01.000000 methodicconfigurator-0.6.0/MethodicConfigurator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-16 10:33:01.000000 methodicconfigurator-0.6.0/MethodicConfigurator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 10:32:53.000000 methodicconfigurator-0.6.0/MethodicConfigurator.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-16 10:33:01.317068 methodicconfigurator-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 10:33:01.317068 methodicconfigurator-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:33:01.253068 methodicconfigurator-0.6.0/vehicle_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:33:01.253068 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:33:01.273068 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/
--rw-r--r--   0 runner    (1001) docker     (127)    17325 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/00_default.param
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/02_imu_temperature_calibration_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/03_imu_temperature_calibration_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/04_board_orientation.param
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/05_remote_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/06_telemetry.param
--rw-r--r--   0 runner    (1001) docker     (127)    15167 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/07_esc.param
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/08_batt1.param
--rw-r--r--   0 runner    (1001) docker     (127)     7341 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/10_gnss.param
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/11_mp_setup_mandatory_hardware.param
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/12_general_configuration.param
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/13_logging.param
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/14_motor.param
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/15_pid_adjustment.param
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/16_remote_id.param
--rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/17_notch_filter_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/18_notch_filter_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/19_throttle_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/20_quick_tune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/21_quick_tune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/22_inflight_magnetometer_fit_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/22_inflight_magnetometer_fit_setup.pdef.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/23_inflight_magnetometer_fit_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/24_quick_tune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/25_quick_tune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/26_evaluate_the_aircraft_tune_ff_disable.param
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/27_evaluate_the_aircraft_tune_ff_enable.param
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/28_autotune_roll_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/29_autotune_roll_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/30_autotune_pitch_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/31_autotune_pitch_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/32_autotune_yaw_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/33_autotune_yaw_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/34_autotune_yawd_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/35_autotune_yawd_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/36_autotune_roll_pitch_retune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/37_autotune_roll_pitch_retune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/38_windspeed_estimation.param
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/39_barometer_compensation.param
--rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/40_system_id_roll.param
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/41_system_id_pitch.param
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/42_system_id_yaw.param
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/43_system_id_thrust.param
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/44_analytical_pid_optimization.param
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/45_everyday_use.param
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/46_position_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)    14385 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/47_precision_land.param
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/48_guided_operation.param
--rw-r--r--   0 runner    (1001) docker     (127)  1998191 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/apm.pdef.xml
--rw-r--r--   0 runner    (1001) docker     (127)    77536 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/tempcal_acc.png
--rw-r--r--   0 runner    (1001) docker     (127)    78746 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/tempcal_gyro.png
--rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/vehicle_components.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:33:01.253068 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:33:01.281068 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/
--rw-r--r--   0 runner    (1001) docker     (127)    21744 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/00_default.param
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/02_imu_temperature_calibration_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/03_imu_temperature_calibration_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/04_board_orientation.param
--rw-r--r--   0 runner    (1001) docker     (127)    20075 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/05_remote_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/06_telemetry.param
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/07_esc.param
--rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/08_batt1.param
--rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/09_batt2.param
--rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/10_gnss.param
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/11_mp_setup_mandatory_hardware.param
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/12_general_configuration.param
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/13_logging.param
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/14_motor.param
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/15_pid_adjustment.param
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/16_remote_id.param
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/17_notch_filter_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/18_notch_filter_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/19_throttle_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/20_quick_tune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/21_quick_tune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/22_inflight_magnetometer_fit_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/22_inflight_magnetometer_fit_setup.pdef.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/23_inflight_magnetometer_fit_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/24_quick_tune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/25_quick_tune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/26_evaluate_the_aircraft_tune_ff_disable.param
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/27_evaluate_the_aircraft_tune_ff_enable.param
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/28_autotune_roll_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/29_autotune_roll_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/30_autotune_pitch_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/31_autotune_pitch_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/32_autotune_yaw_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/33_autotune_yaw_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/34_autotune_yawd_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/35_autotune_yawd_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/36_autotune_roll_pitch_retune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/37_autotune_roll_pitch_retune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/38_windspeed_estimation.param
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/39_barometer_compensation.param
--rw-r--r--   0 runner    (1001) docker     (127)     6165 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/40_system_id_roll.param
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/41_system_id_pitch.param
--rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/42_system_id_yaw.param
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/43_system_id_thrust.param
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/44_analytical_pid_optimization.param
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/45_everyday_use.param
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/46_position_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)    13406 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/47_precision_land.param
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/48_guided_operation.param
--rw-r--r--   0 runner    (1001) docker     (127)  1476098 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/apm.pdef.xml
--rw-r--r--   0 runner    (1001) docker     (127)   126547 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/vehicle.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/vehicle_components.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:33:01.293068 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/
--rw-r--r--   0 runner    (1001) docker     (127)    21744 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/00_default.param
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/02_imu_temperature_calibration_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/03_imu_temperature_calibration_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/04_board_orientation.param
--rw-r--r--   0 runner    (1001) docker     (127)    20688 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/05_remote_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/06_telemetry.param
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/07_esc.param
--rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/08_batt1.param
--rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/09_batt2.param
--rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/10_gnss.param
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/11_mp_setup_mandatory_hardware.param
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/12_general_configuration.param
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/13_logging.param
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/14_motor.param
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/15_pid_adjustment.param
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/16_remote_id.param
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/17_notch_filter_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/18_notch_filter_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/19_throttle_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/20_quick_tune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/21_quick_tune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/22_inflight_magnetometer_fit_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/22_inflight_magnetometer_fit_setup.pdef.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/23_inflight_magnetometer_fit_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/24_quick_tune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/25_quick_tune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/26_evaluate_the_aircraft_tune_ff_disable.param
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/27_evaluate_the_aircraft_tune_ff_enable.param
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/28_autotune_roll_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/29_autotune_roll_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/30_autotune_pitch_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/31_autotune_pitch_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/32_autotune_yaw_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/33_autotune_yaw_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/34_autotune_yawd_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/35_autotune_yawd_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/36_autotune_roll_pitch_retune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/37_autotune_roll_pitch_retune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/38_windspeed_estimation.param
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/39_barometer_compensation.param
--rw-r--r--   0 runner    (1001) docker     (127)     6997 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/40_system_id_roll.param
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/41_system_id_pitch.param
--rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/42_system_id_yaw.param
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/43_system_id_thrust.param
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/44_analytical_pid_optimization.param
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/45_everyday_use.param
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/46_position_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)    13612 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/47_precision_land.param
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/48_guided_operation.param
--rw-r--r--   0 runner    (1001) docker     (127)  1599965 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/apm.pdef.xml
--rw-r--r--   0 runner    (1001) docker     (127)   126547 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/vehicle.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/vehicle_components.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:33:01.305068 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/
--rw-r--r--   0 runner    (1001) docker     (127)    21744 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/00_default.param
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/02_imu_temperature_calibration_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/03_imu_temperature_calibration_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/04_board_orientation.param
--rw-r--r--   0 runner    (1001) docker     (127)    21636 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/05_remote_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/06_telemetry.param
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/07_esc.param
--rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/08_batt1.param
--rw-r--r--   0 runner    (1001) docker     (127)     5885 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/09_batt2.param
--rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/10_gnss.param
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/11_mp_setup_mandatory_hardware.param
--rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/12_general_configuration.param
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/13_logging.param
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/14_motor.param
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/15_pid_adjustment.param
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/16_remote_id.param
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/17_notch_filter_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/18_notch_filter_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/19_throttle_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/20_quick_tune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/21_quick_tune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/22_inflight_magnetometer_fit_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/22_inflight_magnetometer_fit_setup.pdef.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/23_inflight_magnetometer_fit_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/24_quick_tune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/25_quick_tune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/26_evaluate_the_aircraft_tune_ff_disable.param
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/27_evaluate_the_aircraft_tune_ff_enable.param
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/28_autotune_roll_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/29_autotune_roll_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/30_autotune_pitch_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/31_autotune_pitch_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/32_autotune_yaw_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/33_autotune_yaw_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/34_autotune_yawd_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/35_autotune_yawd_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/36_autotune_roll_pitch_retune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/37_autotune_roll_pitch_retune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/38_windspeed_estimation.param
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/39_barometer_compensation.param
--rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/40_system_id_roll.param
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/41_system_id_pitch.param
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/42_system_id_yaw.param
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/43_system_id_thrust.param
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/44_analytical_pid_optimization.param
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/45_everyday_use.param
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/46_position_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)    14081 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/47_precision_land.param
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/48_guided_operation.param
--rw-r--r--   0 runner    (1001) docker     (127)  1966610 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/apm.pdef.xml
--rw-r--r--   0 runner    (1001) docker     (127)   126547 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/vehicle.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/vehicle_components.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:33:01.317068 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/
--rw-r--r--   0 runner    (1001) docker     (127)    21744 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/00_default.param
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/02_imu_temperature_calibration_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/03_imu_temperature_calibration_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/04_board_orientation.param
--rw-r--r--   0 runner    (1001) docker     (127)    22629 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/05_remote_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/06_telemetry.param
--rw-r--r--   0 runner    (1001) docker     (127)    15514 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/07_esc.param
--rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/08_batt1.param
--rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/09_batt2.param
--rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/10_gnss.param
--rw-r--r--   0 runner    (1001) docker     (127)    34447 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/11_mp_setup_mandatory_hardware.param
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/12_general_configuration.param
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/13_logging.param
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/14_motor.param
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/15_pid_adjustment.param
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/16_remote_id.param
--rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/17_notch_filter_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/18_notch_filter_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/19_throttle_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/20_quick_tune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/21_quick_tune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/22_inflight_magnetometer_fit_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/22_inflight_magnetometer_fit_setup.pdef.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/23_inflight_magnetometer_fit_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/24_quick_tune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/25_quick_tune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/26_evaluate_the_aircraft_tune_ff_disable.param
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/27_evaluate_the_aircraft_tune_ff_enable.param
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/28_autotune_roll_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/29_autotune_roll_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/30_autotune_pitch_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/31_autotune_pitch_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/32_autotune_yaw_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/33_autotune_yaw_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/34_autotune_yawd_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/35_autotune_yawd_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/36_autotune_roll_pitch_retune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/37_autotune_roll_pitch_retune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/38_windspeed_estimation.param
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/39_barometer_compensation.param
--rw-r--r--   0 runner    (1001) docker     (127)     6244 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/40_system_id_roll.param
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/41_system_id_pitch.param
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/42_system_id_yaw.param
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/43_system_id_thrust.param
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/44_analytical_pid_optimization.param
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/45_everyday_use.param
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/46_position_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)    14119 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/47_precision_land.param
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/48_guided_operation.param
--rw-r--r--   0 runner    (1001) docker     (127)  1982447 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/apm.pdef.xml
--rw-r--r--   0 runner    (1001) docker     (127)   126547 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/vehicle.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-05-16 10:32:34.000000 methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/vehicle_components.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:17:07.195321 methodicconfigurator-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35823 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:17:07.135321 methodicconfigurator-0.6.1/MethodicConfigurator/
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/ArduPilot_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26216 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/ArduPilot_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27852 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/annotate_params.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4993 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/ardupilot_methodic_configurator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29041 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/backend_filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/backend_filesystem_configuration_steps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/backend_filesystem_vehicle_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31001 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/backend_flightcontroller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26774 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/backend_mavftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/battery_cell_voltages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/common_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8259 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/extract_param_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13811 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/frontend_tkinter_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18042 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/frontend_tkinter_component_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/frontend_tkinter_component_editor_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14736 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/frontend_tkinter_connection_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20140 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/frontend_tkinter_directory_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37652 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/frontend_tkinter_parameter_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27039 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/frontend_tkinter_parameter_editor_table.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2468 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/get_release_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/param_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9757 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/param_pid_adjustment_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22803 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/tempcal_imu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:17:07.195321 methodicconfigurator-0.6.1/MethodicConfigurator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-16 12:17:07.000000 methodicconfigurator-0.6.1/MethodicConfigurator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23766 2024-05-16 12:17:07.000000 methodicconfigurator-0.6.1/MethodicConfigurator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 12:17:07.000000 methodicconfigurator-0.6.1/MethodicConfigurator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-16 12:17:07.000000 methodicconfigurator-0.6.1/MethodicConfigurator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-16 12:17:07.000000 methodicconfigurator-0.6.1/MethodicConfigurator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-16 12:17:07.000000 methodicconfigurator-0.6.1/MethodicConfigurator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 12:16:59.000000 methodicconfigurator-0.6.1/MethodicConfigurator.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-16 12:17:07.195321 methodicconfigurator-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 12:17:07.195321 methodicconfigurator-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:17:07.131321 methodicconfigurator-0.6.1/vehicle_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:17:07.131321 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:17:07.147321 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/
+-rw-r--r--   0 runner    (1001) docker     (127)    17325 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/00_default.param
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/02_imu_temperature_calibration_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/03_imu_temperature_calibration_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/04_board_orientation.param
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/05_remote_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/06_telemetry.param
+-rw-r--r--   0 runner    (1001) docker     (127)    15186 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/07_esc.param
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/08_batt1.param
+-rw-r--r--   0 runner    (1001) docker     (127)     7341 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/10_gnss.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/11_mp_setup_mandatory_hardware.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/12_general_configuration.param
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/13_logging.param
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/14_motor.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/15_pid_adjustment.param
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/16_remote_id.param
+-rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/17_notch_filter_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/18_notch_filter_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/19_throttle_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/20_quick_tune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/21_quick_tune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/22_inflight_magnetometer_fit_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/22_inflight_magnetometer_fit_setup.pdef.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/23_inflight_magnetometer_fit_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/24_quick_tune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/25_quick_tune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/26_evaluate_the_aircraft_tune_ff_disable.param
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/27_evaluate_the_aircraft_tune_ff_enable.param
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/28_autotune_roll_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/29_autotune_roll_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/30_autotune_pitch_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/31_autotune_pitch_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/32_autotune_yaw_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/33_autotune_yaw_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/34_autotune_yawd_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/35_autotune_yawd_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/36_autotune_roll_pitch_retune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/37_autotune_roll_pitch_retune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/38_windspeed_estimation.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/39_barometer_compensation.param
+-rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/40_system_id_roll.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/41_system_id_pitch.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/42_system_id_yaw.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/43_system_id_thrust.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/44_analytical_pid_optimization.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/45_everyday_use.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/46_position_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)    14385 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/47_precision_land.param
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/48_guided_operation.param
+-rw-r--r--   0 runner    (1001) docker     (127)  1998191 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/apm.pdef.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    77536 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/tempcal_acc.png
+-rw-r--r--   0 runner    (1001) docker     (127)    78746 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/tempcal_gyro.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/vehicle_components.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:17:07.131321 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:17:07.159321 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/
+-rw-r--r--   0 runner    (1001) docker     (127)    21744 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/00_default.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/02_imu_temperature_calibration_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/03_imu_temperature_calibration_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/04_board_orientation.param
+-rw-r--r--   0 runner    (1001) docker     (127)    20075 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/05_remote_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/06_telemetry.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/07_esc.param
+-rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/08_batt1.param
+-rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/09_batt2.param
+-rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/10_gnss.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/11_mp_setup_mandatory_hardware.param
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/12_general_configuration.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/13_logging.param
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/14_motor.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/15_pid_adjustment.param
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/16_remote_id.param
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/17_notch_filter_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/18_notch_filter_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/19_throttle_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/20_quick_tune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/21_quick_tune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/22_inflight_magnetometer_fit_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/22_inflight_magnetometer_fit_setup.pdef.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/23_inflight_magnetometer_fit_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/24_quick_tune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/25_quick_tune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/26_evaluate_the_aircraft_tune_ff_disable.param
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/27_evaluate_the_aircraft_tune_ff_enable.param
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/28_autotune_roll_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/29_autotune_roll_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/30_autotune_pitch_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/31_autotune_pitch_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/32_autotune_yaw_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/33_autotune_yaw_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/34_autotune_yawd_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/35_autotune_yawd_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/36_autotune_roll_pitch_retune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/37_autotune_roll_pitch_retune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/38_windspeed_estimation.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/39_barometer_compensation.param
+-rw-r--r--   0 runner    (1001) docker     (127)     6165 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/40_system_id_roll.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/41_system_id_pitch.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/42_system_id_yaw.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/43_system_id_thrust.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/44_analytical_pid_optimization.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/45_everyday_use.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/46_position_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)    13406 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/47_precision_land.param
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/48_guided_operation.param
+-rw-r--r--   0 runner    (1001) docker     (127)  1476098 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/apm.pdef.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   126547 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/vehicle.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/vehicle_components.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:17:07.171321 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/
+-rw-r--r--   0 runner    (1001) docker     (127)    21744 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/00_default.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/02_imu_temperature_calibration_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/03_imu_temperature_calibration_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/04_board_orientation.param
+-rw-r--r--   0 runner    (1001) docker     (127)    20688 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/05_remote_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/06_telemetry.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/07_esc.param
+-rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/08_batt1.param
+-rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/09_batt2.param
+-rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/10_gnss.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/11_mp_setup_mandatory_hardware.param
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/12_general_configuration.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/13_logging.param
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/14_motor.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/15_pid_adjustment.param
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/16_remote_id.param
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/17_notch_filter_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/18_notch_filter_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/19_throttle_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/20_quick_tune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/21_quick_tune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/22_inflight_magnetometer_fit_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/22_inflight_magnetometer_fit_setup.pdef.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/23_inflight_magnetometer_fit_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/24_quick_tune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/25_quick_tune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/26_evaluate_the_aircraft_tune_ff_disable.param
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/27_evaluate_the_aircraft_tune_ff_enable.param
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/28_autotune_roll_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/29_autotune_roll_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/30_autotune_pitch_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/31_autotune_pitch_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/32_autotune_yaw_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/33_autotune_yaw_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/34_autotune_yawd_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/35_autotune_yawd_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/36_autotune_roll_pitch_retune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/37_autotune_roll_pitch_retune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/38_windspeed_estimation.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/39_barometer_compensation.param
+-rw-r--r--   0 runner    (1001) docker     (127)     6997 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/40_system_id_roll.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/41_system_id_pitch.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/42_system_id_yaw.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/43_system_id_thrust.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/44_analytical_pid_optimization.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/45_everyday_use.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/46_position_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)    13612 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/47_precision_land.param
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/48_guided_operation.param
+-rw-r--r--   0 runner    (1001) docker     (127)  1599965 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/apm.pdef.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   126547 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/vehicle.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/vehicle_components.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:17:07.183321 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/
+-rw-r--r--   0 runner    (1001) docker     (127)    21744 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/00_default.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/02_imu_temperature_calibration_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/03_imu_temperature_calibration_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/04_board_orientation.param
+-rw-r--r--   0 runner    (1001) docker     (127)    21636 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/05_remote_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/06_telemetry.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/07_esc.param
+-rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/08_batt1.param
+-rw-r--r--   0 runner    (1001) docker     (127)     5885 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/09_batt2.param
+-rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/10_gnss.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/11_mp_setup_mandatory_hardware.param
+-rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/12_general_configuration.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/13_logging.param
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/14_motor.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/15_pid_adjustment.param
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/16_remote_id.param
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/17_notch_filter_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/18_notch_filter_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/19_throttle_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/20_quick_tune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/21_quick_tune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/22_inflight_magnetometer_fit_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/22_inflight_magnetometer_fit_setup.pdef.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/23_inflight_magnetometer_fit_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/24_quick_tune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/25_quick_tune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/26_evaluate_the_aircraft_tune_ff_disable.param
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/27_evaluate_the_aircraft_tune_ff_enable.param
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/28_autotune_roll_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/29_autotune_roll_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/30_autotune_pitch_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/31_autotune_pitch_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/32_autotune_yaw_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/33_autotune_yaw_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/34_autotune_yawd_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/35_autotune_yawd_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/36_autotune_roll_pitch_retune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/37_autotune_roll_pitch_retune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/38_windspeed_estimation.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/39_barometer_compensation.param
+-rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/40_system_id_roll.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/41_system_id_pitch.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/42_system_id_yaw.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/43_system_id_thrust.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/44_analytical_pid_optimization.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/45_everyday_use.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/46_position_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)    14081 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/47_precision_land.param
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/48_guided_operation.param
+-rw-r--r--   0 runner    (1001) docker     (127)  1966610 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/apm.pdef.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   126547 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/vehicle.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/vehicle_components.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:17:07.191321 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/
+-rw-r--r--   0 runner    (1001) docker     (127)    21744 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/00_default.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/02_imu_temperature_calibration_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/03_imu_temperature_calibration_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/04_board_orientation.param
+-rw-r--r--   0 runner    (1001) docker     (127)    22629 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/05_remote_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/06_telemetry.param
+-rw-r--r--   0 runner    (1001) docker     (127)    15514 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/07_esc.param
+-rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/08_batt1.param
+-rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/09_batt2.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/10_gnss.param
+-rw-r--r--   0 runner    (1001) docker     (127)    34447 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/11_mp_setup_mandatory_hardware.param
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/12_general_configuration.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/13_logging.param
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/14_motor.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/15_pid_adjustment.param
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/16_remote_id.param
+-rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/17_notch_filter_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/18_notch_filter_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/19_throttle_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/20_quick_tune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/21_quick_tune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/22_inflight_magnetometer_fit_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/22_inflight_magnetometer_fit_setup.pdef.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/23_inflight_magnetometer_fit_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/24_quick_tune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/25_quick_tune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/26_evaluate_the_aircraft_tune_ff_disable.param
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/27_evaluate_the_aircraft_tune_ff_enable.param
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/28_autotune_roll_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/29_autotune_roll_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/30_autotune_pitch_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/31_autotune_pitch_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/32_autotune_yaw_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/33_autotune_yaw_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/34_autotune_yawd_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/35_autotune_yawd_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/36_autotune_roll_pitch_retune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/37_autotune_roll_pitch_retune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/38_windspeed_estimation.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/39_barometer_compensation.param
+-rw-r--r--   0 runner    (1001) docker     (127)     6244 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/40_system_id_roll.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/41_system_id_pitch.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/42_system_id_yaw.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/43_system_id_thrust.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/44_analytical_pid_optimization.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/45_everyday_use.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/46_position_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)    14119 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/47_precision_land.param
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/48_guided_operation.param
+-rw-r--r--   0 runner    (1001) docker     (127)  1982447 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/apm.pdef.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   126547 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/vehicle.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/vehicle_components.json
```

### Comparing `methodicconfigurator-0.6.0/LICENSE.md` & `methodicconfigurator-0.6.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/MethodicConfigurator/ArduPilot_icon.png` & `methodicconfigurator-0.6.1/MethodicConfigurator/ArduPilot_icon.png`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/MethodicConfigurator/ArduPilot_logo.png` & `methodicconfigurator-0.6.1/MethodicConfigurator/ArduPilot_logo.png`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/MethodicConfigurator/annotate_params.py` & `methodicconfigurator-0.6.1/MethodicConfigurator/annotate_params.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/MethodicConfigurator/ardupilot_methodic_configurator.py` & `methodicconfigurator-0.6.1/MethodicConfigurator/ardupilot_methodic_configurator.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/MethodicConfigurator/backend_filesystem.py` & `methodicconfigurator-0.6.1/MethodicConfigurator/backend_filesystem.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/MethodicConfigurator/backend_filesystem_configuration_steps.py` & `methodicconfigurator-0.6.1/MethodicConfigurator/backend_filesystem_configuration_steps.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/MethodicConfigurator/backend_filesystem_vehicle_components.py` & `methodicconfigurator-0.6.1/MethodicConfigurator/backend_filesystem_vehicle_components.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/MethodicConfigurator/backend_flightcontroller.py` & `methodicconfigurator-0.6.1/MethodicConfigurator/backend_flightcontroller.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/MethodicConfigurator/backend_mavftp.py` & `methodicconfigurator-0.6.1/MethodicConfigurator/backend_mavftp.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/MethodicConfigurator/battery_cell_voltages.py` & `methodicconfigurator-0.6.1/MethodicConfigurator/battery_cell_voltages.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/MethodicConfigurator/common_arguments.py` & `methodicconfigurator-0.6.1/MethodicConfigurator/common_arguments.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/MethodicConfigurator/extract_param_defaults.py` & `methodicconfigurator-0.6.1/MethodicConfigurator/extract_param_defaults.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/MethodicConfigurator/frontend_tkinter_base.py` & `methodicconfigurator-0.6.1/MethodicConfigurator/frontend_tkinter_base.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/MethodicConfigurator/frontend_tkinter_component_editor.py` & `methodicconfigurator-0.6.1/MethodicConfigurator/frontend_tkinter_component_editor.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/MethodicConfigurator/frontend_tkinter_component_editor_base.py` & `methodicconfigurator-0.6.1/MethodicConfigurator/frontend_tkinter_component_editor_base.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/MethodicConfigurator/frontend_tkinter_connection_selection.py` & `methodicconfigurator-0.6.1/MethodicConfigurator/frontend_tkinter_connection_selection.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/MethodicConfigurator/frontend_tkinter_directory_selection.py` & `methodicconfigurator-0.6.1/MethodicConfigurator/frontend_tkinter_directory_selection.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/MethodicConfigurator/frontend_tkinter_parameter_editor.py` & `methodicconfigurator-0.6.1/MethodicConfigurator/frontend_tkinter_parameter_editor.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/MethodicConfigurator/frontend_tkinter_parameter_editor_table.py` & `methodicconfigurator-0.6.1/MethodicConfigurator/frontend_tkinter_parameter_editor_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,21 +136,21 @@
             for i, (param_name, param) in enumerate(params.items(), 1):
                 param_metadata = self.local_filesystem.doc_dict.get(param_name, None)
                 param_default = self.local_filesystem.param_default_dict.get(param_name, None)
                 doc_tooltip = param_metadata.get('doc_tooltip') if param_metadata else \
                     "No documentation available in apm.pdef.xml for this parameter"
 
                 column = []
-                column[0] = self.__create_delete_button(param_name)
-                column[1] = self.__create_parameter_name(param_name, param_metadata, doc_tooltip)
-                column[2] = self.__create_flightcontroller_value(fc_parameters, param_name, param_default, doc_tooltip)
-                column[3] = self.__create_new_value_entry(param_name, param, param_metadata, param_default, doc_tooltip)
-                column[4] = self.__create_unit_label(param_metadata)
-                column[5] = self.__create_upload_checkbutton(param_name)
-                column[6] = self.__create_change_reason_entry(param_name, param, column[3])
+                column.append(self.__create_delete_button(param_name))
+                column.append(self.__create_parameter_name(param_name, param_metadata, doc_tooltip))
+                column.append(self.__create_flightcontroller_value(fc_parameters, param_name, param_default, doc_tooltip))
+                column.append(self.__create_new_value_entry(param_name, param, param_metadata, param_default, doc_tooltip))
+                column.append(self.__create_unit_label(param_metadata))
+                column.append(self.__create_upload_checkbutton(param_name))
+                column.append(self.__create_change_reason_entry(param_name, param, column[3]))
 
                 column[0].grid(row=i, column=0, sticky="w", padx=0)
                 column[1].grid(row=i, column=1, sticky="w", padx=0)
                 column[2].grid(row=i, column=2, sticky="e", padx=0)
                 column[3].grid(row=i, column=3, sticky="e", padx=0)
                 column[4].grid(row=i, column=4, sticky="e", padx=0)
                 column[5].grid(row=i, column=5, sticky="e", padx=0)
```

### Comparing `methodicconfigurator-0.6.0/MethodicConfigurator/get_release_stats.py` & `methodicconfigurator-0.6.1/MethodicConfigurator/get_release_stats.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/MethodicConfigurator/param_ftp.py` & `methodicconfigurator-0.6.1/MethodicConfigurator/param_ftp.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/MethodicConfigurator/param_pid_adjustment_update.py` & `methodicconfigurator-0.6.1/MethodicConfigurator/param_pid_adjustment_update.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/MethodicConfigurator/tempcal_imu.py` & `methodicconfigurator-0.6.1/MethodicConfigurator/tempcal_imu.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/MethodicConfigurator.egg-info/PKG-INFO` & `methodicconfigurator-0.6.1/MethodicConfigurator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MethodicConfigurator
-Version: 0.6.0
+Version: 0.6.1
 Summary: A clear configuration sequence for ArduPilot vehicles
 Home-page: https://github.com/ArduPilot/MethodicConfigurator
 Author: Amilcar do Carmo Lucas
 Author-email: amilcar.lucas@iav.de
 License: GPLv3
 Keywords: ArduPilot,Configuration,SCM,Methodic,ArduCopter,ArduPlane,ArduRover,ArduSub
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `methodicconfigurator-0.6.0/MethodicConfigurator.egg-info/SOURCES.txt` & `methodicconfigurator-0.6.1/MethodicConfigurator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/PKG-INFO` & `methodicconfigurator-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MethodicConfigurator
-Version: 0.6.0
+Version: 0.6.1
 Summary: A clear configuration sequence for ArduPilot vehicles
 Home-page: https://github.com/ArduPilot/MethodicConfigurator
 Author: Amilcar do Carmo Lucas
 Author-email: amilcar.lucas@iav.de
 License: GPLv3
 Keywords: ArduPilot,Configuration,SCM,Methodic,ArduCopter,ArduPlane,ArduRover,ArduSub
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `methodicconfigurator-0.6.0/README.md` & `methodicconfigurator-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/setup.py` & `methodicconfigurator-0.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/00_default.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/00_default.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/02_imu_temperature_calibration_setup.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/02_imu_temperature_calibration_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/03_imu_temperature_calibration_results.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/03_imu_temperature_calibration_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/04_board_orientation.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/04_board_orientation.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/06_telemetry.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/06_telemetry.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/07_esc.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/07_esc.param`

 * *Files 1% similar despite different names*

```diff
@@ -310,7 +310,9 @@
 MOT_PWM_MAX,1950
 
 MOT_PWM_MIN,1050
 
 MOT_SPOOL_TIME,3
 
 TKOFF_SLEW_TIME,4
+
+MOT_HOVER_LEARN,2
```

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/10_gnss.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/10_gnss.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/11_mp_setup_mandatory_hardware.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/11_mp_setup_mandatory_hardware.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/12_general_configuration.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/12_general_configuration.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/15_pid_adjustment.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/15_pid_adjustment.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/17_notch_filter_setup.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/17_notch_filter_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/18_notch_filter_results.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/18_notch_filter_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/22_inflight_magnetometer_fit_setup.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/22_inflight_magnetometer_fit_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/22_inflight_magnetometer_fit_setup.pdef.xml` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/22_inflight_magnetometer_fit_setup.pdef.xml`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/23_inflight_magnetometer_fit_results.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/23_inflight_magnetometer_fit_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/29_autotune_roll_results.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/29_autotune_roll_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/31_autotune_pitch_results.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/31_autotune_pitch_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/32_autotune_yaw_setup.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/32_autotune_yaw_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/33_autotune_yaw_results.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/33_autotune_yaw_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/35_autotune_yawd_results.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/35_autotune_yawd_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/37_autotune_roll_pitch_retune_results.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/37_autotune_roll_pitch_retune_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/38_windspeed_estimation.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/38_windspeed_estimation.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/39_barometer_compensation.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/39_barometer_compensation.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/40_system_id_roll.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/40_system_id_roll.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/41_system_id_pitch.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/41_system_id_pitch.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/42_system_id_yaw.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/42_system_id_yaw.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/43_system_id_thrust.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/43_system_id_thrust.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/44_analytical_pid_optimization.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/44_analytical_pid_optimization.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/45_everyday_use.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/45_everyday_use.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/46_position_controller.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/46_position_controller.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/47_precision_land.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/47_precision_land.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/48_guided_operation.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/48_guided_operation.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/apm.pdef.xml` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/apm.pdef.xml`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/tempcal_acc.png` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/tempcal_acc.png`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/tempcal_gyro.png` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/tempcal_gyro.png`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/X11_plus/vehicle_components.json` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/vehicle_components.json`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/00_default.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/00_default.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/02_imu_temperature_calibration_setup.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/02_imu_temperature_calibration_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/03_imu_temperature_calibration_results.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/03_imu_temperature_calibration_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/04_board_orientation.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/04_board_orientation.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/05_remote_controller.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/05_remote_controller.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/06_telemetry.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/06_telemetry.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/07_esc.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/07_esc.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/08_batt1.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/08_batt1.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/09_batt2.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/09_batt2.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/10_gnss.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/10_gnss.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/11_mp_setup_mandatory_hardware.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/11_mp_setup_mandatory_hardware.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/12_general_configuration.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/12_general_configuration.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/13_logging.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/13_logging.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/15_pid_adjustment.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/15_pid_adjustment.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/17_notch_filter_setup.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/17_notch_filter_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/22_inflight_magnetometer_fit_setup.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/22_inflight_magnetometer_fit_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/22_inflight_magnetometer_fit_setup.pdef.xml` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/22_inflight_magnetometer_fit_setup.pdef.xml`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/23_inflight_magnetometer_fit_results.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/23_inflight_magnetometer_fit_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/25_quick_tune_results.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/25_quick_tune_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/29_autotune_roll_results.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/29_autotune_roll_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/31_autotune_pitch_results.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/31_autotune_pitch_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/32_autotune_yaw_setup.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/32_autotune_yaw_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/33_autotune_yaw_results.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/33_autotune_yaw_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/34_autotune_yawd_setup.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/34_autotune_yawd_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/35_autotune_yawd_results.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/35_autotune_yawd_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/37_autotune_roll_pitch_retune_results.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/37_autotune_roll_pitch_retune_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/38_windspeed_estimation.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/38_windspeed_estimation.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/39_barometer_compensation.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/39_barometer_compensation.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/40_system_id_roll.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/40_system_id_roll.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/41_system_id_pitch.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/41_system_id_pitch.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/42_system_id_yaw.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/42_system_id_yaw.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/43_system_id_thrust.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/43_system_id_thrust.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/44_analytical_pid_optimization.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/44_analytical_pid_optimization.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/45_everyday_use.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/45_everyday_use.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/46_position_controller.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/46_position_controller.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/47_precision_land.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/47_precision_land.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/48_guided_operation.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/48_guided_operation.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/apm.pdef.xml` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/apm.pdef.xml`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/vehicle.jpg` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/vehicle.jpg`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/vehicle_components.json` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/vehicle_components.json`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/00_default.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/00_default.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/02_imu_temperature_calibration_setup.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/02_imu_temperature_calibration_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/03_imu_temperature_calibration_results.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/03_imu_temperature_calibration_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/04_board_orientation.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/04_board_orientation.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/05_remote_controller.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/05_remote_controller.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/06_telemetry.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/06_telemetry.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/07_esc.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/07_esc.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/08_batt1.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/08_batt1.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/09_batt2.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/09_batt2.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/10_gnss.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/10_gnss.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/11_mp_setup_mandatory_hardware.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/11_mp_setup_mandatory_hardware.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/12_general_configuration.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/12_general_configuration.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/13_logging.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/13_logging.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/15_pid_adjustment.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/15_pid_adjustment.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/17_notch_filter_setup.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/17_notch_filter_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/21_quick_tune_results.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/21_quick_tune_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/22_inflight_magnetometer_fit_setup.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/22_inflight_magnetometer_fit_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/22_inflight_magnetometer_fit_setup.pdef.xml` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/22_inflight_magnetometer_fit_setup.pdef.xml`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/23_inflight_magnetometer_fit_results.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/23_inflight_magnetometer_fit_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/24_quick_tune_setup.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/24_quick_tune_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/25_quick_tune_results.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/25_quick_tune_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/29_autotune_roll_results.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/29_autotune_roll_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/31_autotune_pitch_results.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/31_autotune_pitch_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/32_autotune_yaw_setup.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/32_autotune_yaw_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/33_autotune_yaw_results.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/33_autotune_yaw_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/34_autotune_yawd_setup.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/34_autotune_yawd_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/35_autotune_yawd_results.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/35_autotune_yawd_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/37_autotune_roll_pitch_retune_results.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/37_autotune_roll_pitch_retune_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/38_windspeed_estimation.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/38_windspeed_estimation.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/39_barometer_compensation.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/39_barometer_compensation.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/40_system_id_roll.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/40_system_id_roll.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/41_system_id_pitch.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/41_system_id_pitch.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/42_system_id_yaw.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/42_system_id_yaw.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/43_system_id_thrust.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/43_system_id_thrust.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/44_analytical_pid_optimization.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/44_analytical_pid_optimization.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/45_everyday_use.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/45_everyday_use.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/46_position_controller.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/46_position_controller.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/47_precision_land.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/47_precision_land.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/48_guided_operation.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/48_guided_operation.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/apm.pdef.xml` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/apm.pdef.xml`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/vehicle.jpg` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/vehicle.jpg`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/vehicle_components.json` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/vehicle_components.json`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/00_default.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/00_default.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/02_imu_temperature_calibration_setup.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/02_imu_temperature_calibration_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/03_imu_temperature_calibration_results.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/03_imu_temperature_calibration_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/04_board_orientation.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/04_board_orientation.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/05_remote_controller.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/05_remote_controller.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/06_telemetry.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/06_telemetry.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/07_esc.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/07_esc.param`

 * *Files 2% similar despite different names*

```diff
@@ -23,7 +23,9 @@
 SERVO3_MAX,2000  # Use the full available 1000-2000 DShot range
 SERVO3_MIN,1000  # Use the full available 1000-2000 DShot range
 SERVO3_TRIM,1000  # Use the full available 1000-2000 DShot range
 SERVO4_MAX,2000  # Use the full available 1000-2000 DShot range
 SERVO4_MIN,1000  # Use the full available 1000-2000 DShot range
 SERVO4_TRIM,1000  # Use the full available 1000-2000 DShot range
 TKOFF_RPM_MIN,1400  # Our motors should idle at around 1400 RPM, see https://ardupilot.org/copter/docs/tkoff-rpm-min.html
+
+MOT_HOVER_LEARN,2
```

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/08_batt1.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/08_batt1.param`

 * *Files 0% similar despite different names*

```diff
@@ -44,27 +44,27 @@
 # 1: Land
 # 2: RTL
 # 3: SmartRTL or RTL
 # 4: SmartRTL or Land
 # 5: Terminate
 # 6: Auto DO_LAND_START or RTL
 # Default: 0
-BATT_FS_CRT_ACT,1  # flying indoors, just land ASAP, no need to hit the celing while doing RTL
+BATT_FS_CRT_ACT,1  # flying indoors, just land ASAP, no need to hit the celling while doing RTL
 
 # Low battery failsafe action
 # What action the vehicle should perform if it hits a low battery failsafe
 # 0: None
 # 1: Land
 # 2: RTL
 # 3: SmartRTL or RTL
 # 4: SmartRTL or Land
 # 5: Terminate
 # 6: Auto DO_LAND_START or RTL
 # Default: 0
-BATT_FS_LOW_ACT,1  # flying indoors, just land ASAP, no need to hit the celing while doing RTL
+BATT_FS_LOW_ACT,1  # flying indoors, just land ASAP, no need to hit the celling while doing RTL
 
 # Failsafe voltage source
 # Voltage type used for detection of low voltage event
 # 0: Raw Voltage
 # 1: Sag Compensated Voltage
 # Default: 0
 BATT_FS_VOLTSRC,1
```

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/09_batt2.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/09_batt2.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/10_gnss.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/10_gnss.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/11_mp_setup_mandatory_hardware.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/11_mp_setup_mandatory_hardware.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/12_general_configuration.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/12_general_configuration.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/13_logging.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/13_logging.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/15_pid_adjustment.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/15_pid_adjustment.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/17_notch_filter_setup.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/17_notch_filter_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/21_quick_tune_results.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/21_quick_tune_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/22_inflight_magnetometer_fit_setup.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/22_inflight_magnetometer_fit_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/22_inflight_magnetometer_fit_setup.pdef.xml` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/22_inflight_magnetometer_fit_setup.pdef.xml`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/23_inflight_magnetometer_fit_results.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/23_inflight_magnetometer_fit_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/24_quick_tune_setup.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/24_quick_tune_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/25_quick_tune_results.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/25_quick_tune_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/29_autotune_roll_results.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/29_autotune_roll_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/31_autotune_pitch_results.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/31_autotune_pitch_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/32_autotune_yaw_setup.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/32_autotune_yaw_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/33_autotune_yaw_results.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/33_autotune_yaw_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/34_autotune_yawd_setup.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/34_autotune_yawd_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/35_autotune_yawd_results.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/35_autotune_yawd_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/37_autotune_roll_pitch_retune_results.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/37_autotune_roll_pitch_retune_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/38_windspeed_estimation.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/38_windspeed_estimation.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/39_barometer_compensation.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/39_barometer_compensation.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/40_system_id_roll.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/40_system_id_roll.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/41_system_id_pitch.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/41_system_id_pitch.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/42_system_id_yaw.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/42_system_id_yaw.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/43_system_id_thrust.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/43_system_id_thrust.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/44_analytical_pid_optimization.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/44_analytical_pid_optimization.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/45_everyday_use.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/45_everyday_use.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/46_position_controller.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/46_position_controller.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/47_precision_land.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/47_precision_land.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/48_guided_operation.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/48_guided_operation.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/apm.pdef.xml` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/apm.pdef.xml`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/vehicle.jpg` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/vehicle.jpg`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/vehicle_components.json` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/vehicle_components.json`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/00_default.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/00_default.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/02_imu_temperature_calibration_setup.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/02_imu_temperature_calibration_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/03_imu_temperature_calibration_results.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/03_imu_temperature_calibration_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/04_board_orientation.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/04_board_orientation.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/05_remote_controller.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/05_remote_controller.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/06_telemetry.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/06_telemetry.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/07_esc.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/07_esc.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/08_batt1.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/08_batt1.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/09_batt2.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/09_batt2.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/10_gnss.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/10_gnss.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/11_mp_setup_mandatory_hardware.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/11_mp_setup_mandatory_hardware.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/12_general_configuration.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/12_general_configuration.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/13_logging.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/13_logging.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/15_pid_adjustment.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/15_pid_adjustment.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/16_remote_id.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/16_remote_id.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/17_notch_filter_setup.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/17_notch_filter_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/18_notch_filter_results.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/18_notch_filter_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/19_throttle_controller.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/19_throttle_controller.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/22_inflight_magnetometer_fit_setup.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/22_inflight_magnetometer_fit_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/22_inflight_magnetometer_fit_setup.pdef.xml` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/22_inflight_magnetometer_fit_setup.pdef.xml`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/23_inflight_magnetometer_fit_results.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/23_inflight_magnetometer_fit_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/29_autotune_roll_results.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/29_autotune_roll_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/31_autotune_pitch_results.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/31_autotune_pitch_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/32_autotune_yaw_setup.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/32_autotune_yaw_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/33_autotune_yaw_results.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/33_autotune_yaw_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/35_autotune_yawd_results.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/35_autotune_yawd_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/37_autotune_roll_pitch_retune_results.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/37_autotune_roll_pitch_retune_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/38_windspeed_estimation.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/38_windspeed_estimation.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/39_barometer_compensation.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/39_barometer_compensation.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/40_system_id_roll.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/40_system_id_roll.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/41_system_id_pitch.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/41_system_id_pitch.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/42_system_id_yaw.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/42_system_id_yaw.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/43_system_id_thrust.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/43_system_id_thrust.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/44_analytical_pid_optimization.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/44_analytical_pid_optimization.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/45_everyday_use.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/45_everyday_use.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/46_position_controller.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/46_position_controller.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/47_precision_land.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/47_precision_land.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/48_guided_operation.param` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/48_guided_operation.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/apm.pdef.xml` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/apm.pdef.xml`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/vehicle.jpg` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/vehicle.jpg`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.0/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/vehicle_components.json` & `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/vehicle_components.json`

 * *Files identical despite different names*

