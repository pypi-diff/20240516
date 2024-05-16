# Comparing `tmp/straxen-2.2.2.tar.gz` & `tmp/straxen-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "straxen-2.2.2.tar", last modified: Tue Apr 30 23:26:07 2024, max compression
+gzip compressed data, was "straxen-2.2.3.tar", last modified: Thu May 16 14:26:53 2024, max compression
```

## Comparing `straxen-2.2.2.tar` & `straxen-2.2.3.tar`

### file list

```diff
@@ -1,253 +1,254 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.269488 straxen-2.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)    50745 2024-04-30 23:26:04.000000 straxen-2.2.2/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-30 23:26:04.000000 straxen-2.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-30 23:26:04.000000 straxen-2.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    53161 2024-04-30 23:26:07.269488 straxen-2.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-30 23:26:04.000000 straxen-2.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.237488 straxen-2.2.2/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)    37105 2024-04-30 23:26:04.000000 straxen-2.2.2/bin/ajax
--rwxr-xr-x   0 runner    (1001) docker     (127)    67403 2024-04-30 23:26:04.000000 straxen-2.2.2/bin/bootstrax
--rwxr-xr-x   0 runner    (1001) docker     (127)     8446 2024-04-30 23:26:04.000000 straxen-2.2.2/bin/fake_daq
--rwxr-xr-x   0 runner    (1001) docker     (127)     6236 2024-04-30 23:26:04.000000 straxen-2.2.2/bin/microstrax
--rwxr-xr-x   0 runner    (1001) docker     (127)     5099 2024-04-30 23:26:04.000000 straxen-2.2.2/bin/refresh_raw_records
--rwxr-xr-x   0 runner    (1001) docker     (127)    36681 2024-04-30 23:26:04.000000 straxen-2.2.2/bin/restrax
--rwxr-xr-x   0 runner    (1001) docker     (127)      754 2024-04-30 23:26:04.000000 straxen-2.2.2/bin/straxen-print_versions
--rwxr-xr-x   0 runner    (1001) docker     (127)    12167 2024-04-30 23:26:04.000000 straxen-2.2.2/bin/straxer
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.237488 straxen-2.2.2/extra_requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-30 23:26:04.000000 straxen-2.2.2/extra_requirements/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-30 23:26:04.000000 straxen-2.2.2/extra_requirements/requirements-tests.txt
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-30 23:26:04.000000 straxen-2.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-30 23:26:07.269488 straxen-2.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-30 23:26:04.000000 straxen-2.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.241488 straxen-2.2.2/straxen/
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.245488 straxen-2.2.2/straxen/analyses/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/analyses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34262 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/analyses/bokeh_waveform_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/analyses/daq_waveforms.py
--rw-r--r--   0 runner    (1001) docker     (127)    16212 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/analyses/event_display.py
--rw-r--r--   0 runner    (1001) docker     (127)    15551 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/analyses/holoviews_waveform_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/analyses/posrec_comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     9986 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/analyses/pulse_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     8581 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/analyses/quick_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5486 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/analyses/records_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     9178 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/analyses/waveform_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/bokeh_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    20895 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    13095 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/contexts.py
--rw-r--r--   0 runner    (1001) docker     (127)    18806 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/corrections_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/daq_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/entry_points.py
--rw-r--r--   0 runner    (1001) docker     (127)     8125 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/get_corrections.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.245488 straxen-2.2.2/straxen/holoviews/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/holoviews/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9759 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/holoviews/holoviews_inspector.py
--rw-r--r--   0 runner    (1001) docker     (127)    12135 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/holoviews/holoviews_peak_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5299 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/holoviews/holoviews_pmt_array.py
--rw-r--r--   0 runner    (1001) docker     (127)    15310 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/holoviews/holoviews_tpc_event_display.py
--rw-r--r--   0 runner    (1001) docker     (127)    18651 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/holoviews_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14994 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/itp_map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.245488 straxen-2.2.2/straxen/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/legacy/contexts_1t.py
--rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/legacy/hitfinder_thresholds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.245488 straxen-2.2.2/straxen/legacy/plugins_1t/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/legacy/plugins_1t/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/legacy/plugins_1t/event_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/legacy/plugins_1t/fake_daqreader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6275 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/legacy/plugins_1t/pax_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/legacy/plugins_1t/peak_positions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10409 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/legacy/plugins_1t/x1t_cuts.py
--rw-r--r--   0 runner    (1001) docker     (127)     7550 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/legacy/xenon1t_url_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6801 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/matplotlib_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/mini_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    17970 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/numbafied_scipy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.245488 straxen-2.2.2/straxen/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.245488 straxen-2.2.2/straxen/plugins/afterpulses/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/afterpulses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11531 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/afterpulses/afterpulse_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.245488 straxen-2.2.2/straxen/plugins/aqmon_hits/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/aqmon_hits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5234 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/aqmon_hits/aqmon_hits.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.253488 straxen-2.2.2/straxen/plugins/events/
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/_event_s1_positions_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/_event_s2_positions_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12324 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/corrected_areas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/distinct_channels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/energy_estimates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/event_ambience.py
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/event_area_per_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)    16510 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/event_basics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/event_basics_som.py
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/event_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/event_info_double.py
--rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/event_nearest_triggering.py
--rw-r--r--   0 runner    (1001) docker     (127)    26370 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/event_pattern_fit.py
--rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/event_positions.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/event_s1_positions_cnn.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/event_s2_positions_cnn.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/event_s2_positions_gcn.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/event_s2_positions_mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/event_se_sensity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/event_shadow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/event_top_bottom_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/event_w_bayes_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/event_waveform.py
--rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     8338 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/local_minimum_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/multi_scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/s2_recon_pos_diff.py
--rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/veto_proximity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.253488 straxen-2.2.2/straxen/plugins/events_mv/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events_mv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events_mv/events_mv.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events_mv/events_sync_mv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.253488 straxen-2.2.2/straxen/plugins/events_nv/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events_nv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7846 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events_nv/event_positions_nv.py
--rw-r--r--   0 runner    (1001) docker     (127)     8230 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events_nv/events_nv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events_nv/events_sync_nv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.253488 straxen-2.2.2/straxen/plugins/gps_syncing/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/gps_syncing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10950 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/gps_syncing/gps_syncing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.253488 straxen-2.2.2/straxen/plugins/hitlets_mv/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/hitlets_mv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/hitlets_mv/hitlets_mv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.253488 straxen-2.2.2/straxen/plugins/hitlets_nv/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/hitlets_nv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/hitlets_nv/hitlets_nv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.253488 straxen-2.2.2/straxen/plugins/individual_peak_monitor/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/individual_peak_monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/individual_peak_monitor/individual_peak_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.253488 straxen-2.2.2/straxen/plugins/led_cal/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/led_cal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8952 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/led_cal/led_calibration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.253488 straxen-2.2.2/straxen/plugins/merged_s2s/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/merged_s2s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9363 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/merged_s2s/merged_s2s.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.253488 straxen-2.2.2/straxen/plugins/merged_s2s_he/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/merged_s2s_he/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/merged_s2s_he/merged_s2s_he.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.253488 straxen-2.2.2/straxen/plugins/online_monitor_mv/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/online_monitor_mv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/online_monitor_mv/online_monitor_mv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.257488 straxen-2.2.2/straxen/plugins/online_monitor_nv/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/online_monitor_nv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/online_monitor_nv/online_monitor_nv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.257488 straxen-2.2.2/straxen/plugins/online_peak_monitor/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/online_peak_monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/online_peak_monitor/online_peak_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.257488 straxen-2.2.2/straxen/plugins/peaklets/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaklets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaklets/peaklet_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)    11704 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaklets/peaklet_classification_som.py
--rw-r--r--   0 runner    (1001) docker     (127)    25952 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaklets/peaklets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.257488 straxen-2.2.2/straxen/plugins/peaklets_he/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaklets_he/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaklets_he/peaklet_classification_he.py
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaklets_he/peaklets_he.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.261488 straxen-2.2.2/straxen/plugins/peaks/
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks/_peak_positions_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks/_peak_s1_positions_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7628 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks/peak_ambience.py
--rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks/peak_basics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks/peak_basics_som.py
--rw-r--r--   0 runner    (1001) docker     (127)     7898 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks/peak_classification_bayes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks/peak_corrections.py
--rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks/peak_nearest_triggering.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks/peak_per_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks/peak_positions.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks/peak_positions_cnn.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks/peak_positions_gcn.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks/peak_positions_mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks/peak_proximity.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks/peak_s1_positions_cnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks/peak_se_sensity.py
--rw-r--r--   0 runner    (1001) docker     (127)    10392 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks/peak_shadow.py
--rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks/peak_top_bottom_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks/peaks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks/peaks_som.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.261488 straxen-2.2.2/straxen/plugins/peaks_he/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks_he/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks_he/peak_basics_he.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks_he/peaks_he.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.261488 straxen-2.2.2/straxen/plugins/raw_records/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/raw_records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16574 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/raw_records/daqreader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.261488 straxen-2.2.2/straxen/plugins/raw_records_coin_nv/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/raw_records_coin_nv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19584 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/raw_records_coin_nv/nveto_recorder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.261488 straxen-2.2.2/straxen/plugins/records/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17520 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/records/records.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.261488 straxen-2.2.2/straxen/plugins/records_he/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/records_he/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/records_he/records_he.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.261488 straxen-2.2.2/straxen/plugins/records_mv/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/records_mv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/records_mv/records_mv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.261488 straxen-2.2.2/straxen/plugins/records_nv/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/records_nv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/records_nv/records_nv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.261488 straxen-2.2.2/straxen/plugins/ref_mon_nv/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/ref_mon_nv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/ref_mon_nv/ref_mon_nv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.261488 straxen-2.2.2/straxen/plugins/veto_intervals/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/veto_intervals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7166 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/veto_intervals/veto_intervals.py
--rw-r--r--   0 runner    (1001) docker     (127)    26574 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/scada.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.265488 straxen-2.2.2/straxen/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14552 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/storage/mongo_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/storage/online_monitor_frontend.py
--rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/storage/rucio_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     7920 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/storage/rucio_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)    13295 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/storage/rundb.py
--rw-r--r--   0 runner    (1001) docker     (127)     7494 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/units.py
--rw-r--r--   0 runner    (1001) docker     (127)    26074 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/url_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.241488 straxen-2.2.2/straxen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    53161 2024-04-30 23:26:07.000000 straxen-2.2.2/straxen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7528 2024-04-30 23:26:07.000000 straxen-2.2.2/straxen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 23:26:07.000000 straxen-2.2.2/straxen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 23:26:07.000000 straxen-2.2.2/straxen.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-30 23:26:07.000000 straxen-2.2.2/straxen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-30 23:26:07.000000 straxen-2.2.2/straxen.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.269488 straxen-2.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.269488 straxen-2.2.2/tests/storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9266 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/storage/test_database_frontends.py
--rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/storage/test_mongo_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/storage/test_mongo_interactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7445 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/storage/test_rucio_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/storage/test_rucio_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_1T_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)    10472 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_aqmon.py
--rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_channel_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_cmt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_contexts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_count_pulses.py
--rw-r--r--   0 runner    (1001) docker     (127)     6795 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_daq_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_holoviews_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_itp_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_led_calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)    14806 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_mini_analyses.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9247 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_nveto_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_nveto_recorder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_patternfit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_peaklet_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_peaks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_scada.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_testing_suite.py
--rw-r--r--   0 runner    (1001) docker     (127)    15988 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_url_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_veto_hitlets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:53.771144 straxen-2.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    51219 2024-05-16 14:26:46.000000 straxen-2.2.3/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-16 14:26:46.000000 straxen-2.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-16 14:26:46.000000 straxen-2.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    53635 2024-05-16 14:26:53.771144 straxen-2.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-16 14:26:46.000000 straxen-2.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:53.743144 straxen-2.2.3/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    37105 2024-05-16 14:26:46.000000 straxen-2.2.3/bin/ajax
+-rwxr-xr-x   0 runner    (1001) docker     (127)    67403 2024-05-16 14:26:46.000000 straxen-2.2.3/bin/bootstrax
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8446 2024-05-16 14:26:46.000000 straxen-2.2.3/bin/fake_daq
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6236 2024-05-16 14:26:46.000000 straxen-2.2.3/bin/microstrax
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5099 2024-05-16 14:26:46.000000 straxen-2.2.3/bin/refresh_raw_records
+-rwxr-xr-x   0 runner    (1001) docker     (127)    36681 2024-05-16 14:26:46.000000 straxen-2.2.3/bin/restrax
+-rwxr-xr-x   0 runner    (1001) docker     (127)      754 2024-05-16 14:26:46.000000 straxen-2.2.3/bin/straxen-print_versions
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12167 2024-05-16 14:26:46.000000 straxen-2.2.3/bin/straxer
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:53.743144 straxen-2.2.3/extra_requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-16 14:26:46.000000 straxen-2.2.3/extra_requirements/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-16 14:26:46.000000 straxen-2.2.3/extra_requirements/requirements-tests.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-16 14:26:46.000000 straxen-2.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-16 14:26:53.771144 straxen-2.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-16 14:26:46.000000 straxen-2.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:53.747144 straxen-2.2.3/straxen/
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:53.747144 straxen-2.2.3/straxen/analyses/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/analyses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34262 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/analyses/bokeh_waveform_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/analyses/daq_waveforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16212 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/analyses/event_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15551 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/analyses/holoviews_waveform_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/analyses/posrec_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9986 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/analyses/pulse_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8581 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/analyses/quick_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5486 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/analyses/records_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9178 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/analyses/waveform_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/bokeh_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20895 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13095 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/contexts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18806 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/corrections_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/daq_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/docs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8125 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/get_corrections.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:53.747144 straxen-2.2.3/straxen/holoviews/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/holoviews/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9759 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/holoviews/holoviews_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12135 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/holoviews/holoviews_peak_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5299 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/holoviews/holoviews_pmt_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15310 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/holoviews/holoviews_tpc_event_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18651 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/holoviews_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14994 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/itp_map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:53.747144 straxen-2.2.3/straxen/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/legacy/contexts_1t.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/legacy/hitfinder_thresholds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:53.751144 straxen-2.2.3/straxen/legacy/plugins_1t/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/legacy/plugins_1t/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/legacy/plugins_1t/event_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/legacy/plugins_1t/fake_daqreader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6275 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/legacy/plugins_1t/pax_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/legacy/plugins_1t/peak_positions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10409 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/legacy/plugins_1t/x1t_cuts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7550 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/legacy/xenon1t_url_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6801 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/matplotlib_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/mini_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17974 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/numbafied_scipy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:53.751144 straxen-2.2.3/straxen/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:53.751144 straxen-2.2.3/straxen/plugins/afterpulses/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/afterpulses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11531 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/afterpulses/afterpulse_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:53.751144 straxen-2.2.3/straxen/plugins/aqmon_hits/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/aqmon_hits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5234 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/aqmon_hits/aqmon_hits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:53.755144 straxen-2.2.3/straxen/plugins/events/
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/events/_event_s1_positions_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/events/_event_s2_positions_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12324 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/events/corrected_areas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/events/distinct_channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/events/energy_estimates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/events/event_ambience.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/events/event_area_per_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16485 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/events/event_basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/events/event_basics_som.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/events/event_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/events/event_info_double.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/events/event_nearest_triggering.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26370 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/events/event_pattern_fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/events/event_positions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/events/event_s1_positions_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/events/event_s2_positions_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/events/event_s2_positions_gcn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/events/event_s2_positions_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/events/event_se_sensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/events/event_shadow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/events/event_top_bottom_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/events/event_w_bayes_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/events/event_waveform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/events/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8338 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/events/local_minimum_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/events/multi_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/events/s2_recon_pos_diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/events/veto_proximity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:53.755144 straxen-2.2.3/straxen/plugins/events_mv/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/events_mv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/events_mv/events_mv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/events_mv/events_sync_mv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:53.755144 straxen-2.2.3/straxen/plugins/events_nv/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/events_nv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7846 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/events_nv/event_positions_nv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8230 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/events_nv/events_nv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/events_nv/events_sync_nv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:53.755144 straxen-2.2.3/straxen/plugins/gps_syncing/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/gps_syncing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10950 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/gps_syncing/gps_syncing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:53.755144 straxen-2.2.3/straxen/plugins/hitlets_mv/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/hitlets_mv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/hitlets_mv/hitlets_mv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:53.755144 straxen-2.2.3/straxen/plugins/hitlets_nv/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/hitlets_nv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/hitlets_nv/hitlets_nv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:53.759144 straxen-2.2.3/straxen/plugins/individual_peak_monitor/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/individual_peak_monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/individual_peak_monitor/individual_peak_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:53.759144 straxen-2.2.3/straxen/plugins/led_cal/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/led_cal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8952 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/led_cal/led_calibration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:53.759144 straxen-2.2.3/straxen/plugins/merged_s2s/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/merged_s2s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9363 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/merged_s2s/merged_s2s.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:53.759144 straxen-2.2.3/straxen/plugins/merged_s2s_he/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/merged_s2s_he/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/merged_s2s_he/merged_s2s_he.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:53.759144 straxen-2.2.3/straxen/plugins/online_monitor_mv/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/online_monitor_mv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/online_monitor_mv/online_monitor_mv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:53.759144 straxen-2.2.3/straxen/plugins/online_monitor_nv/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/online_monitor_nv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/online_monitor_nv/online_monitor_nv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:53.759144 straxen-2.2.3/straxen/plugins/online_peak_monitor/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/online_peak_monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/online_peak_monitor/online_peak_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:53.759144 straxen-2.2.3/straxen/plugins/peaklets/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/peaklets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/peaklets/peaklet_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11704 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/peaklets/peaklet_classification_som.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25952 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/peaklets/peaklets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:53.759144 straxen-2.2.3/straxen/plugins/peaklets_he/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/peaklets_he/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/peaklets_he/peaklet_classification_he.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/peaklets_he/peaklets_he.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:53.763144 straxen-2.2.3/straxen/plugins/peaks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/peaks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/peaks/_peak_positions_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/peaks/_peak_s1_positions_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7628 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/peaks/peak_ambience.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/peaks/peak_basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/peaks/peak_basics_som.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7898 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/peaks/peak_classification_bayes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/peaks/peak_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/peaks/peak_nearest_triggering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/peaks/peak_per_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/peaks/peak_positions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/peaks/peak_positions_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/peaks/peak_positions_gcn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/peaks/peak_positions_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/peaks/peak_proximity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/peaks/peak_s1_positions_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/peaks/peak_se_sensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10392 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/peaks/peak_shadow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/peaks/peak_top_bottom_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/peaks/peaks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/peaks/peaks_som.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:53.763144 straxen-2.2.3/straxen/plugins/peaks_he/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/peaks_he/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/peaks_he/peak_basics_he.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/peaks_he/peaks_he.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:53.763144 straxen-2.2.3/straxen/plugins/raw_records/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/raw_records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16574 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/raw_records/daqreader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:53.763144 straxen-2.2.3/straxen/plugins/raw_records_coin_nv/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/raw_records_coin_nv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19584 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/raw_records_coin_nv/nveto_recorder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:53.763144 straxen-2.2.3/straxen/plugins/records/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17520 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/records/records.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:53.763144 straxen-2.2.3/straxen/plugins/records_he/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/records_he/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/records_he/records_he.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:53.767144 straxen-2.2.3/straxen/plugins/records_mv/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/records_mv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/records_mv/records_mv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:53.767144 straxen-2.2.3/straxen/plugins/records_nv/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/records_nv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/records_nv/records_nv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:53.767144 straxen-2.2.3/straxen/plugins/ref_mon_nv/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/ref_mon_nv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/ref_mon_nv/ref_mon_nv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:53.767144 straxen-2.2.3/straxen/plugins/veto_intervals/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/veto_intervals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7166 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/plugins/veto_intervals/veto_intervals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26574 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/scada.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:53.767144 straxen-2.2.3/straxen/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14552 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/storage/mongo_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/storage/online_monitor_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/storage/rucio_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7920 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/storage/rucio_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13295 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/storage/rundb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7494 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26074 2024-05-16 14:26:46.000000 straxen-2.2.3/straxen/url_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:53.747144 straxen-2.2.3/straxen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    53635 2024-05-16 14:26:53.000000 straxen-2.2.3/straxen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7550 2024-05-16 14:26:53.000000 straxen-2.2.3/straxen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 14:26:53.000000 straxen-2.2.3/straxen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 14:26:53.000000 straxen-2.2.3/straxen.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-16 14:26:53.000000 straxen-2.2.3/straxen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-16 14:26:53.000000 straxen-2.2.3/straxen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:53.771144 straxen-2.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:46.000000 straxen-2.2.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:53.771144 straxen-2.2.3/tests/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 14:26:46.000000 straxen-2.2.3/tests/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9266 2024-05-16 14:26:46.000000 straxen-2.2.3/tests/storage/test_database_frontends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-05-16 14:26:46.000000 straxen-2.2.3/tests/storage/test_mongo_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-16 14:26:46.000000 straxen-2.2.3/tests/storage/test_mongo_interactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7445 2024-05-16 14:26:46.000000 straxen-2.2.3/tests/storage/test_rucio_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-16 14:26:46.000000 straxen-2.2.3/tests/storage/test_rucio_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-05-16 14:26:46.000000 straxen-2.2.3/tests/test_1T_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10472 2024-05-16 14:26:46.000000 straxen-2.2.3/tests/test_aqmon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-05-16 14:26:46.000000 straxen-2.2.3/tests/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-16 14:26:46.000000 straxen-2.2.3/tests/test_channel_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-05-16 14:26:46.000000 straxen-2.2.3/tests/test_cmt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-16 14:26:46.000000 straxen-2.2.3/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-05-16 14:26:46.000000 straxen-2.2.3/tests/test_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-16 14:26:46.000000 straxen-2.2.3/tests/test_count_pulses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6795 2024-05-16 14:26:46.000000 straxen-2.2.3/tests/test_daq_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-16 14:26:46.000000 straxen-2.2.3/tests/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-05-16 14:26:46.000000 straxen-2.2.3/tests/test_holoviews_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-05-16 14:26:46.000000 straxen-2.2.3/tests/test_itp_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-16 14:26:46.000000 straxen-2.2.3/tests/test_led_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14806 2024-05-16 14:26:46.000000 straxen-2.2.3/tests/test_mini_analyses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-16 14:26:46.000000 straxen-2.2.3/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9247 2024-05-16 14:26:46.000000 straxen-2.2.3/tests/test_nveto_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-05-16 14:26:46.000000 straxen-2.2.3/tests/test_nveto_recorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-16 14:26:46.000000 straxen-2.2.3/tests/test_patternfit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-05-16 14:26:46.000000 straxen-2.2.3/tests/test_peaklet_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-16 14:26:46.000000 straxen-2.2.3/tests/test_peaks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-05-16 14:26:46.000000 straxen-2.2.3/tests/test_scada.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-16 14:26:46.000000 straxen-2.2.3/tests/test_testing_suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15996 2024-05-16 14:26:46.000000 straxen-2.2.3/tests/test_url_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-16 14:26:46.000000 straxen-2.2.3/tests/test_veto_hitlets.py
```

### Comparing `straxen-2.2.2/HISTORY.md` & `straxen-2.2.3/HISTORY.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+2.2.3 / 2024-05-16
+-------------------
+* No need to set `loop_over` for `EventBasics` by @dachengx in https://github.com/XENONnT/straxen/pull/1377
+* Initialize plugins whose `depends_on` is property by @dachengx in https://github.com/XENONnT/straxen/pull/1379
+* Collect functions used for documentation building in `docs_utils.py` by @dachengx in https://github.com/XENONnT/straxen/pull/1380
+
+**Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.2.2...v2.2.3
+
+
 2.2.2 / 2024-04-30
 -------------------
 * Minor change of indents by @dachengx in https://github.com/XENONnT/straxen/pull/1341
 * Remove unused `__all__` by @dachengx in https://github.com/XENONnT/straxen/pull/1342
 * Bump graphviz from 0.20.1 to 0.20.2 in /extra_requirements by @dependabot in https://github.com/XENONnT/straxen/pull/1345
 * Specifically install `lxml_html_clean` by @dachengx in https://github.com/XENONnT/straxen/pull/1352
 * Improve InterpolateAndExtrapolate performance for array valued maps by @l-althueser in https://github.com/XENONnT/straxen/pull/1347
```

### Comparing `straxen-2.2.2/LICENSE` & `straxen-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/PKG-INFO` & `straxen-2.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: straxen
-Version: 2.2.2
+Version: 2.2.3
 Summary: Streaming analysis for XENON
 Home-page: https://github.com/XENONnT/straxen
 Author: Straxen contributors, the XENON collaboration
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
@@ -37,14 +37,23 @@
 
 
 ## Further status
 [![Python Versions](https://img.shields.io/pypi/pyversions/straxen.svg)](https://pypi.python.org/pypi/straxen)
 [![PyPI downloads](https://img.shields.io/pypi/dm/straxen.svg)](https://pypistats.org/packages/straxen)
 
 
+2.2.3 / 2024-05-16
+-------------------
+* No need to set `loop_over` for `EventBasics` by @dachengx in https://github.com/XENONnT/straxen/pull/1377
+* Initialize plugins whose `depends_on` is property by @dachengx in https://github.com/XENONnT/straxen/pull/1379
+* Collect functions used for documentation building in `docs_utils.py` by @dachengx in https://github.com/XENONnT/straxen/pull/1380
+
+**Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.2.2...v2.2.3
+
+
 2.2.2 / 2024-04-30
 -------------------
 * Minor change of indents by @dachengx in https://github.com/XENONnT/straxen/pull/1341
 * Remove unused `__all__` by @dachengx in https://github.com/XENONnT/straxen/pull/1342
 * Bump graphviz from 0.20.1 to 0.20.2 in /extra_requirements by @dependabot in https://github.com/XENONnT/straxen/pull/1345
 * Specifically install `lxml_html_clean` by @dachengx in https://github.com/XENONnT/straxen/pull/1352
 * Improve InterpolateAndExtrapolate performance for array valued maps by @l-althueser in https://github.com/XENONnT/straxen/pull/1347
```

### Comparing `straxen-2.2.2/README.md` & `straxen-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/bin/ajax` & `straxen-2.2.3/bin/ajax`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/bin/bootstrax` & `straxen-2.2.3/bin/bootstrax`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/bin/fake_daq` & `straxen-2.2.3/bin/fake_daq`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/bin/microstrax` & `straxen-2.2.3/bin/microstrax`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/bin/refresh_raw_records` & `straxen-2.2.3/bin/refresh_raw_records`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/bin/restrax` & `straxen-2.2.3/bin/restrax`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/bin/straxen-print_versions` & `straxen-2.2.3/bin/straxen-print_versions`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/bin/straxer` & `straxen-2.2.3/bin/straxer`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/setup.py` & `straxen-2.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     readme = file.read()
 
 with open("HISTORY.md") as file:
     history = file.read()
 
 setuptools.setup(
     name="straxen",
-    version="2.2.2",
+    version="2.2.3",
     description="Streaming analysis for XENON",
     author="Straxen contributors, the XENON collaboration",
     url="https://github.com/XENONnT/straxen",
     long_description=readme + "\n\n" + history,
     long_description_content_type="text/markdown",
     setup_requires=["pytest-runner"],
     install_requires=requires,
```

### Comparing `straxen-2.2.2/straxen/__init__.py` & `straxen-2.2.3/straxen/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # mypy: disable-error-code="no-redef"
-__version__ = "2.2.2"
+__version__ = "2.2.3"
 
 from utilix import uconfig
 from .common import *
 
 # contexts.py below
 from .corrections_services import *
 from .get_corrections import *
@@ -31,14 +31,17 @@
 # Do not make all contexts directly available under straxen.
 # Otherwise, we have straxen.demo() etc.
 from . import contexts
 
 from . import test_utils
 from .test_utils import *
 
+from . import docs_utils
+from .docs_utils import *
+
 from . import daq_core
 
 try:
     from . import holoviews_utils
     from .holoviews_utils import *
 except ModuleNotFoundError:
     pass
```

### Comparing `straxen-2.2.2/straxen/analyses/bokeh_waveform_plot.py` & `straxen-2.2.3/straxen/analyses/bokeh_waveform_plot.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/analyses/daq_waveforms.py` & `straxen-2.2.3/straxen/analyses/daq_waveforms.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/analyses/event_display.py` & `straxen-2.2.3/straxen/analyses/event_display.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/analyses/holoviews_waveform_display.py` & `straxen-2.2.3/straxen/analyses/holoviews_waveform_display.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/analyses/posrec_comparison.py` & `straxen-2.2.3/straxen/analyses/posrec_comparison.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/analyses/pulse_plots.py` & `straxen-2.2.3/straxen/analyses/pulse_plots.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/analyses/quick_checks.py` & `straxen-2.2.3/straxen/analyses/quick_checks.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/analyses/records_matrix.py` & `straxen-2.2.3/straxen/analyses/records_matrix.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/analyses/waveform_plot.py` & `straxen-2.2.3/straxen/analyses/waveform_plot.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/bokeh_utils.py` & `straxen-2.2.3/straxen/bokeh_utils.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/common.py` & `straxen-2.2.3/straxen/common.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/contexts.py` & `straxen-2.2.3/straxen/contexts.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/corrections_services.py` & `straxen-2.2.3/straxen/corrections_services.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/daq_core.py` & `straxen-2.2.3/straxen/daq_core.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/entry_points.py` & `straxen-2.2.3/straxen/entry_points.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/get_corrections.py` & `straxen-2.2.3/straxen/get_corrections.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/holoviews/holoviews_inspector.py` & `straxen-2.2.3/straxen/holoviews/holoviews_inspector.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/holoviews/holoviews_peak_data.py` & `straxen-2.2.3/straxen/holoviews/holoviews_peak_data.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/holoviews/holoviews_pmt_array.py` & `straxen-2.2.3/straxen/holoviews/holoviews_pmt_array.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/holoviews/holoviews_tpc_event_display.py` & `straxen-2.2.3/straxen/holoviews/holoviews_tpc_event_display.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/holoviews_utils.py` & `straxen-2.2.3/straxen/holoviews_utils.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/itp_map.py` & `straxen-2.2.3/straxen/itp_map.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/legacy/contexts_1t.py` & `straxen-2.2.3/straxen/legacy/contexts_1t.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/legacy/hitfinder_thresholds.py` & `straxen-2.2.3/straxen/legacy/hitfinder_thresholds.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/legacy/plugins_1t/pax_interface.py` & `straxen-2.2.3/straxen/legacy/plugins_1t/pax_interface.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/legacy/plugins_1t/peak_positions.py` & `straxen-2.2.3/straxen/legacy/plugins_1t/peak_positions.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/legacy/plugins_1t/x1t_cuts.py` & `straxen-2.2.3/straxen/legacy/plugins_1t/x1t_cuts.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/legacy/xenon1t_url_configs.py` & `straxen-2.2.3/straxen/legacy/xenon1t_url_configs.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/matplotlib_utils.py` & `straxen-2.2.3/straxen/matplotlib_utils.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/mini_analysis.py` & `straxen-2.2.3/straxen/mini_analysis.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/misc.py` & `straxen-2.2.3/straxen/misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -505,15 +505,15 @@
     if not_stored is None:
         not_stored = set()
     # the set of plugins which are not stored
     if st.is_stored(run_id, target):
         # if the plugin is stored, fill in green
         fillcolor = "green"
     else:
-        save_when = deepcopy(st._plugin_class_registry[target].save_when)
+        save_when = deepcopy(st._plugin_class_registry[target]().save_when)
         if isinstance(save_when, immutabledict):
             save_when = save_when[target]
         # if it is not stored, fill in the color according to save_when
         fillcolor = save_when_colors[save_when]
 
     if graph is None:
         graph = graphviz.Digraph(name=f"{to_dir}/{run_id}-{target}", strict=True)
@@ -527,15 +527,15 @@
         target,
         label=f"{target}\n{p.__class__.__name__}" if include_class else None,
         style="filled",
         fillcolor=fillcolor,
     )
     if (not st.is_stored(run_id, target)) and (target not in not_stored):
         not_stored.add(target)
-        depends_on = deepcopy(st._plugin_class_registry[target].depends_on)
+        depends_on = deepcopy(st._plugin_class_registry[target]().depends_on)
         depends_on = strax.to_str_tuple(depends_on)
         for dep in depends_on:
             # only add the node to the graph but not save the plot
             not_stored.update(
                 st.storage_graph(
                     run_id,
                     dep,
```

### Comparing `straxen-2.2.2/straxen/numbafied_scipy.py` & `straxen-2.2.3/straxen/numbafied_scipy.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/__init__.py` & `straxen-2.2.3/straxen/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/afterpulses/afterpulse_processing.py` & `straxen-2.2.3/straxen/plugins/afterpulses/afterpulse_processing.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/aqmon_hits/aqmon_hits.py` & `straxen-2.2.3/straxen/plugins/aqmon_hits/aqmon_hits.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/defaults.py` & `straxen-2.2.3/straxen/plugins/defaults.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/events/__init__.py` & `straxen-2.2.3/straxen/plugins/events/__init__.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/events/_event_s1_positions_base.py` & `straxen-2.2.3/straxen/plugins/events/_event_s1_positions_base.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/events/_event_s2_positions_base.py` & `straxen-2.2.3/straxen/plugins/events/_event_s2_positions_base.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/events/corrected_areas.py` & `straxen-2.2.3/straxen/plugins/events/corrected_areas.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/events/distinct_channels.py` & `straxen-2.2.3/straxen/plugins/events/distinct_channels.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/events/energy_estimates.py` & `straxen-2.2.3/straxen/plugins/events/energy_estimates.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/events/event_ambience.py` & `straxen-2.2.3/straxen/plugins/events/event_ambience.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/events/event_area_per_channel.py` & `straxen-2.2.3/straxen/plugins/events/event_area_per_channel.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/events/event_basics.py` & `straxen-2.2.3/straxen/plugins/events/event_basics.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     """
 
     __version__ = "1.3.3"
 
     depends_on = ("events", "peak_basics", "peak_positions", "peak_proximity")
     provides = "event_basics"
     data_kind = "events"
-    loop_over = "events"
 
     electron_drift_velocity = straxen.URLConfig(
         default="cmt://electron_drift_velocity?version=ONLINE&run_id=plugin.run_id",
         cache=True,
         help="Vertical electron drift velocity in cm/ns (1e4 m/ms)",
     )
```

### Comparing `straxen-2.2.2/straxen/plugins/events/event_basics_som.py` & `straxen-2.2.3/straxen/plugins/events/event_basics_som.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/events/event_info.py` & `straxen-2.2.3/straxen/plugins/events/event_info.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/events/event_info_double.py` & `straxen-2.2.3/straxen/plugins/events/event_info_double.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/events/event_nearest_triggering.py` & `straxen-2.2.3/straxen/plugins/events/event_nearest_triggering.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/events/event_pattern_fit.py` & `straxen-2.2.3/straxen/plugins/events/event_pattern_fit.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/events/event_positions.py` & `straxen-2.2.3/straxen/plugins/events/event_positions.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/events/event_s1_positions_cnn.py` & `straxen-2.2.3/straxen/plugins/events/event_s1_positions_cnn.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/events/event_s2_positions_cnn.py` & `straxen-2.2.3/straxen/plugins/events/event_s2_positions_cnn.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/events/event_s2_positions_gcn.py` & `straxen-2.2.3/straxen/plugins/events/event_s2_positions_gcn.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/events/event_s2_positions_mlp.py` & `straxen-2.2.3/straxen/plugins/events/event_s2_positions_mlp.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/events/event_se_sensity.py` & `straxen-2.2.3/straxen/plugins/events/event_se_sensity.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/events/event_shadow.py` & `straxen-2.2.3/straxen/plugins/events/event_shadow.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/events/event_top_bottom_params.py` & `straxen-2.2.3/straxen/plugins/events/event_top_bottom_params.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/events/event_w_bayes_class.py` & `straxen-2.2.3/straxen/plugins/events/event_w_bayes_class.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/events/event_waveform.py` & `straxen-2.2.3/straxen/plugins/events/event_waveform.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/events/events.py` & `straxen-2.2.3/straxen/plugins/events/events.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/events/local_minimum_info.py` & `straxen-2.2.3/straxen/plugins/events/local_minimum_info.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/events/multi_scatter.py` & `straxen-2.2.3/straxen/plugins/events/multi_scatter.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/events/s2_recon_pos_diff.py` & `straxen-2.2.3/straxen/plugins/events/s2_recon_pos_diff.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/events/veto_proximity.py` & `straxen-2.2.3/straxen/plugins/events/veto_proximity.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/events_mv/events_mv.py` & `straxen-2.2.3/straxen/plugins/events_mv/events_mv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/events_mv/events_sync_mv.py` & `straxen-2.2.3/straxen/plugins/events_mv/events_sync_mv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/events_nv/event_positions_nv.py` & `straxen-2.2.3/straxen/plugins/events_nv/event_positions_nv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/events_nv/events_nv.py` & `straxen-2.2.3/straxen/plugins/events_nv/events_nv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/events_nv/events_sync_nv.py` & `straxen-2.2.3/straxen/plugins/events_nv/events_sync_nv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/gps_syncing/gps_syncing.py` & `straxen-2.2.3/straxen/plugins/gps_syncing/gps_syncing.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/hitlets_mv/hitlets_mv.py` & `straxen-2.2.3/straxen/plugins/hitlets_mv/hitlets_mv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/hitlets_nv/hitlets_nv.py` & `straxen-2.2.3/straxen/plugins/hitlets_nv/hitlets_nv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/individual_peak_monitor/individual_peak_monitor.py` & `straxen-2.2.3/straxen/plugins/individual_peak_monitor/individual_peak_monitor.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/led_cal/led_calibration.py` & `straxen-2.2.3/straxen/plugins/led_cal/led_calibration.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/merged_s2s/merged_s2s.py` & `straxen-2.2.3/straxen/plugins/merged_s2s/merged_s2s.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/merged_s2s_he/merged_s2s_he.py` & `straxen-2.2.3/straxen/plugins/merged_s2s_he/merged_s2s_he.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/online_monitor_mv/online_monitor_mv.py` & `straxen-2.2.3/straxen/plugins/online_monitor_mv/online_monitor_mv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/online_monitor_nv/online_monitor_nv.py` & `straxen-2.2.3/straxen/plugins/online_monitor_nv/online_monitor_nv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/online_peak_monitor/online_peak_monitor.py` & `straxen-2.2.3/straxen/plugins/online_peak_monitor/online_peak_monitor.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/peaklets/peaklet_classification.py` & `straxen-2.2.3/straxen/plugins/peaklets/peaklet_classification.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/peaklets/peaklet_classification_som.py` & `straxen-2.2.3/straxen/plugins/peaklets/peaklet_classification_som.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/peaklets/peaklets.py` & `straxen-2.2.3/straxen/plugins/peaklets/peaklets.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/peaklets_he/peaklet_classification_he.py` & `straxen-2.2.3/straxen/plugins/peaklets_he/peaklet_classification_he.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/peaklets_he/peaklets_he.py` & `straxen-2.2.3/straxen/plugins/peaklets_he/peaklets_he.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/peaks/__init__.py` & `straxen-2.2.3/straxen/plugins/peaks/__init__.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/peaks/_peak_positions_base.py` & `straxen-2.2.3/straxen/plugins/peaks/_peak_positions_base.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/peaks/_peak_s1_positions_base.py` & `straxen-2.2.3/straxen/plugins/peaks/_peak_s1_positions_base.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/peaks/peak_ambience.py` & `straxen-2.2.3/straxen/plugins/peaks/peak_ambience.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/peaks/peak_basics.py` & `straxen-2.2.3/straxen/plugins/peaks/peak_basics.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/peaks/peak_basics_som.py` & `straxen-2.2.3/straxen/plugins/peaks/peak_basics_som.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/peaks/peak_classification_bayes.py` & `straxen-2.2.3/straxen/plugins/peaks/peak_classification_bayes.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/peaks/peak_corrections.py` & `straxen-2.2.3/straxen/plugins/peaks/peak_corrections.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/peaks/peak_nearest_triggering.py` & `straxen-2.2.3/straxen/plugins/peaks/peak_nearest_triggering.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/peaks/peak_per_event.py` & `straxen-2.2.3/straxen/plugins/peaks/peak_per_event.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/peaks/peak_positions.py` & `straxen-2.2.3/straxen/plugins/peaks/peak_positions.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/peaks/peak_positions_cnn.py` & `straxen-2.2.3/straxen/plugins/peaks/peak_positions_cnn.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/peaks/peak_positions_gcn.py` & `straxen-2.2.3/straxen/plugins/peaks/peak_positions_gcn.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/peaks/peak_positions_mlp.py` & `straxen-2.2.3/straxen/plugins/peaks/peak_positions_mlp.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/peaks/peak_proximity.py` & `straxen-2.2.3/straxen/plugins/peaks/peak_proximity.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/peaks/peak_s1_positions_cnn.py` & `straxen-2.2.3/straxen/plugins/peaks/peak_s1_positions_cnn.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/peaks/peak_se_sensity.py` & `straxen-2.2.3/straxen/plugins/peaks/peak_se_sensity.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/peaks/peak_shadow.py` & `straxen-2.2.3/straxen/plugins/peaks/peak_shadow.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/peaks/peak_top_bottom_params.py` & `straxen-2.2.3/straxen/plugins/peaks/peak_top_bottom_params.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/peaks/peaks.py` & `straxen-2.2.3/straxen/plugins/peaks/peaks.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/peaks/peaks_som.py` & `straxen-2.2.3/straxen/plugins/peaks/peaks_som.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/peaks_he/peaks_he.py` & `straxen-2.2.3/straxen/plugins/peaks_he/peaks_he.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/raw_records/daqreader.py` & `straxen-2.2.3/straxen/plugins/raw_records/daqreader.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/raw_records_coin_nv/nveto_recorder.py` & `straxen-2.2.3/straxen/plugins/raw_records_coin_nv/nveto_recorder.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/records/records.py` & `straxen-2.2.3/straxen/plugins/records/records.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/records_he/records_he.py` & `straxen-2.2.3/straxen/plugins/records_he/records_he.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/records_mv/records_mv.py` & `straxen-2.2.3/straxen/plugins/records_mv/records_mv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/records_nv/records_nv.py` & `straxen-2.2.3/straxen/plugins/records_nv/records_nv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/ref_mon_nv/ref_mon_nv.py` & `straxen-2.2.3/straxen/plugins/ref_mon_nv/ref_mon_nv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/plugins/veto_intervals/veto_intervals.py` & `straxen-2.2.3/straxen/plugins/veto_intervals/veto_intervals.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/scada.py` & `straxen-2.2.3/straxen/scada.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/storage/mongo_storage.py` & `straxen-2.2.3/straxen/storage/mongo_storage.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/storage/online_monitor_frontend.py` & `straxen-2.2.3/straxen/storage/online_monitor_frontend.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/storage/rucio_local.py` & `straxen-2.2.3/straxen/storage/rucio_local.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/storage/rucio_remote.py` & `straxen-2.2.3/straxen/storage/rucio_remote.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/storage/rundb.py` & `straxen-2.2.3/straxen/storage/rundb.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/test_utils.py` & `straxen-2.2.3/straxen/test_utils.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/units.py` & `straxen-2.2.3/straxen/units.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen/url_config.py` & `straxen-2.2.3/straxen/url_config.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/straxen.egg-info/PKG-INFO` & `straxen-2.2.3/straxen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: straxen
-Version: 2.2.2
+Version: 2.2.3
 Summary: Streaming analysis for XENON
 Home-page: https://github.com/XENONnT/straxen
 Author: Straxen contributors, the XENON collaboration
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
@@ -37,14 +37,23 @@
 
 
 ## Further status
 [![Python Versions](https://img.shields.io/pypi/pyversions/straxen.svg)](https://pypi.python.org/pypi/straxen)
 [![PyPI downloads](https://img.shields.io/pypi/dm/straxen.svg)](https://pypistats.org/packages/straxen)
 
 
+2.2.3 / 2024-05-16
+-------------------
+* No need to set `loop_over` for `EventBasics` by @dachengx in https://github.com/XENONnT/straxen/pull/1377
+* Initialize plugins whose `depends_on` is property by @dachengx in https://github.com/XENONnT/straxen/pull/1379
+* Collect functions used for documentation building in `docs_utils.py` by @dachengx in https://github.com/XENONnT/straxen/pull/1380
+
+**Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.2.2...v2.2.3
+
+
 2.2.2 / 2024-04-30
 -------------------
 * Minor change of indents by @dachengx in https://github.com/XENONnT/straxen/pull/1341
 * Remove unused `__all__` by @dachengx in https://github.com/XENONnT/straxen/pull/1342
 * Bump graphviz from 0.20.1 to 0.20.2 in /extra_requirements by @dependabot in https://github.com/XENONnT/straxen/pull/1345
 * Specifically install `lxml_html_clean` by @dachengx in https://github.com/XENONnT/straxen/pull/1352
 * Improve InterpolateAndExtrapolate performance for array valued maps by @l-althueser in https://github.com/XENONnT/straxen/pull/1347
```

### Comparing `straxen-2.2.2/straxen.egg-info/SOURCES.txt` & `straxen-2.2.3/straxen.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 extra_requirements/requirements-tests.txt
 straxen/__init__.py
 straxen/bokeh_utils.py
 straxen/common.py
 straxen/contexts.py
 straxen/corrections_services.py
 straxen/daq_core.py
+straxen/docs_utils.py
 straxen/entry_points.py
 straxen/get_corrections.py
 straxen/holoviews_utils.py
 straxen/itp_map.py
 straxen/matplotlib_utils.py
 straxen/mini_analysis.py
 straxen/misc.py
```

### Comparing `straxen-2.2.2/tests/storage/test_database_frontends.py` & `straxen-2.2.3/tests/storage/test_database_frontends.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/tests/storage/test_mongo_downloader.py` & `straxen-2.2.3/tests/storage/test_mongo_downloader.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/tests/storage/test_mongo_interactions.py` & `straxen-2.2.3/tests/storage/test_mongo_interactions.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/tests/storage/test_rucio_local.py` & `straxen-2.2.3/tests/storage/test_rucio_local.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/tests/storage/test_rucio_remote.py` & `straxen-2.2.3/tests/storage/test_rucio_remote.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/tests/test_1T_plugins.py` & `straxen-2.2.3/tests/test_1T_plugins.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/tests/test_aqmon.py` & `straxen-2.2.3/tests/test_aqmon.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/tests/test_basics.py` & `straxen-2.2.3/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/tests/test_channel_split.py` & `straxen-2.2.3/tests/test_channel_split.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/tests/test_cmt.py` & `straxen-2.2.3/tests/test_cmt.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/tests/test_common.py` & `straxen-2.2.3/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/tests/test_contexts.py` & `straxen-2.2.3/tests/test_contexts.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/tests/test_count_pulses.py` & `straxen-2.2.3/tests/test_count_pulses.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/tests/test_daq_reader.py` & `straxen-2.2.3/tests/test_daq_reader.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/tests/test_holoviews_utils.py` & `straxen-2.2.3/tests/test_holoviews_utils.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/tests/test_itp_map.py` & `straxen-2.2.3/tests/test_itp_map.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/tests/test_led_calibration.py` & `straxen-2.2.3/tests/test_led_calibration.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/tests/test_mini_analyses.py` & `straxen-2.2.3/tests/test_mini_analyses.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/tests/test_misc.py` & `straxen-2.2.3/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/tests/test_nveto_events.py` & `straxen-2.2.3/tests/test_nveto_events.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/tests/test_nveto_recorder.py` & `straxen-2.2.3/tests/test_nveto_recorder.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/tests/test_patternfit.py` & `straxen-2.2.3/tests/test_patternfit.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/tests/test_peaklet_processing.py` & `straxen-2.2.3/tests/test_peaklet_processing.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/tests/test_peaks.py` & `straxen-2.2.3/tests/test_peaks.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/tests/test_scada.py` & `straxen-2.2.3/tests/test_scada.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.2/tests/test_url_config.py` & `straxen-2.2.3/tests/test_url_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -371,16 +371,16 @@
         st1 = self.st.new_context(
             config={"test_config": "fake://electron_lifetimes?run_id=25000&version=v5&attr=value"}
         )
         st2 = self.st.new_context(
             config={"test_config": "fake://electron_lifetimes?attr=value&run_id=25000&version=v5"}
         )
         self.assertEqual(
-            st1.key_for(25000, "corrected_areas").lineage_hash,
-            st2.key_for(25000, "corrected_areas").lineage_hash,
+            st1.key_for("025000", "corrected_areas").lineage_hash,
+            st2.key_for("025000", "corrected_areas").lineage_hash,
         )
 
     def test_global_version_not_changed(self):
         """
         - if no global version is matched, the url version should not be changed
         - if config is not matched, the url version should not be changed
         """
@@ -409,15 +409,15 @@
 
         self.st.set_config({"test_config": "run_doc://fake_key?run_id=plugin.run_id&default=42"})
         p = self.st.get_single_plugin(nt_test_run_id, "test_data")
         self.assertEqual(p.test_config, 42)
 
         with self.assertRaises(ValueError):
             self.st.set_config({"test_config": "run_doc://mode?run_id=plugin.run_id"})
-            p = self.st.get_single_plugin(999999999, "test_data")
+            p = self.st.get_single_plugin("999999999", "test_data")
             return p.test_config
 
     def test_pad_array(self):
         """Test that pad_array works as expected."""
 
         self.st.set_config(
             {"test_config": "pad-array://json://[1,2,3]?pad_left=2&pad_right=3&pad_value=0"}
```

### Comparing `straxen-2.2.2/tests/test_veto_hitlets.py` & `straxen-2.2.3/tests/test_veto_hitlets.py`

 * *Files identical despite different names*

