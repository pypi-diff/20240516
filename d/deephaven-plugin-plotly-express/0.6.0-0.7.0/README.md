# Comparing `tmp/deephaven-plugin-plotly-express-0.6.0.tar.gz` & `tmp/deephaven-plugin-plotly-express-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deephaven-plugin-plotly-express-0.6.0.tar", last modified: Tue Mar 19 17:47:17 2024, max compression
+gzip compressed data, was "deephaven-plugin-plotly-express-0.7.0.tar", last modified: Wed Apr  3 22:02:56 2024, max compression
```

## Comparing `deephaven-plugin-plotly-express-0.6.0.tar` & `deephaven-plugin-plotly-express-0.7.0.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:47:17.746317 deephaven-plugin-plotly-express-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-03-19 17:47:17.746317 deephaven-plugin-plotly-express-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-03-19 17:47:17.746317 deephaven-plugin-plotly-express-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:47:17.718317 deephaven-plugin-plotly-express-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:47:17.718317 deephaven-plugin-plotly-express-0.6.0/src/deephaven/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:47:17.718317 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:47:17.718317 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:47:17.722317 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/
--rw-r--r--   0 runner    (1001) docker     (127)     9793 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:47:17.726317 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/
--rw-r--r--   0 runner    (1001) docker     (127)      278 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/DashboardPlugin.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      269 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/DashboardPlugin.d.ts.map
--rw-r--r--   0 runner    (1001) docker     (127)     1546 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/DashboardPlugin.js
--rw-r--r--   0 runner    (1001) docker     (127)     1411 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/DashboardPlugin.js.map
--rw-r--r--   0 runner    (1001) docker     (127)      333 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChart.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      346 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChart.d.ts.map
--rw-r--r--   0 runner    (1001) docker     (127)     1403 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChart.js
--rw-r--r--   0 runner    (1001) docker     (127)     1242 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChart.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     2690 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChartModel.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     2067 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChartModel.d.ts.map
--rw-r--r--   0 runner    (1001) docker     (127)    11457 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChartModel.js
--rw-r--r--   0 runner    (1001) docker     (127)     9508 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChartModel.js.map
--rw-r--r--   0 runner    (1001) docker     (127)      333 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChartPanel.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      324 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChartPanel.d.ts.map
--rw-r--r--   0 runner    (1001) docker     (127)     1708 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChartPanel.js
--rw-r--r--   0 runner    (1001) docker     (127)     1175 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChartPanel.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     1595 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChartUtils.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1167 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChartUtils.d.ts.map
--rw-r--r--   0 runner    (1001) docker     (127)     2668 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChartUtils.js
--rw-r--r--   0 runner    (1001) docker     (127)     1924 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChartUtils.js.map
--rw-r--r--   0 runner    (1001) docker     (127)      258 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/PlotlyExpressPlugin.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      302 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/PlotlyExpressPlugin.d.ts.map
--rw-r--r--   0 runner    (1001) docker     (127)      585 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/PlotlyExpressPlugin.js
--rw-r--r--   0 runner    (1001) docker     (127)      515 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/PlotlyExpressPlugin.js.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:47:17.734317 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/bundle/
--rw-r--r--   0 runner    (1001) docker     (127)  6658826 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/bundle/index.js
--rw-r--r--   0 runner    (1001) docker     (127)    69117 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/bundle/style.css
--rw-r--r--   0 runner    (1001) docker     (127)      265 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      239 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/index.d.ts.map
--rw-r--r--   0 runner    (1001) docker     (127)      341 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      250 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/index.js.map
--rw-r--r--   0 runner    (1001) docker     (127)      282 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/useHandleSceneTicks.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      278 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/useHandleSceneTicks.d.ts.map
--rw-r--r--   0 runner    (1001) docker     (127)     1647 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/useHandleSceneTicks.js
--rw-r--r--   0 runner    (1001) docker     (127)     1311 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/useHandleSceneTicks.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     2035 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/package.json
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_register.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:47:17.738317 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/communication/
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/communication/DeephavenFigureConnection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6178 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/communication/DeephavenFigureListener.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/communication/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:47:17.738317 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/data/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10305 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/data/data_generators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:47:17.738317 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/data_mapping/
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/data_mapping/DataMapping.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/data_mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6518 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/data_mapping/data_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/data_mapping/data_mapping_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/data_mapping/json_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:47:17.738317 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/deephaven_figure/
--rw-r--r--   0 runner    (1001) docker     (127)    21272 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/deephaven_figure/DeephavenFigure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/deephaven_figure/RevisionManager.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/deephaven_figure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/deephaven_figure/custom_draw.py
--rw-r--r--   0 runner    (1001) docker     (127)    34201 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/deephaven_figure/generate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:47:17.738317 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/exporter/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/exporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/exporter/export.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:47:17.742318 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/plots/
--rw-r--r--   0 runner    (1001) docker     (127)    25488 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/plots/PartitionManager.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19439 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/plots/_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)    17133 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/plots/_private_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10652 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/plots/area.py
--rw-r--r--   0 runner    (1001) docker     (127)    24048 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/plots/bar.py
--rw-r--r--   0 runner    (1001) docker     (127)    24302 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/plots/distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     7661 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/plots/financial.py
--rw-r--r--   0 runner    (1001) docker     (127)    20359 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/plots/hierarchial.py
--rw-r--r--   0 runner    (1001) docker     (127)    40152 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/plots/line.py
--rw-r--r--   0 runner    (1001) docker     (127)    38474 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/plots/maps.py
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/plots/pie.py
--rw-r--r--   0 runner    (1001) docker     (127)    37924 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/plots/scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10777 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/plots/subplots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:47:17.742318 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/preprocess/
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/preprocess/AttachedPreprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/preprocess/FreqPreprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8788 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/preprocess/HistPreprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/preprocess/Preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/preprocess/StyleManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/preprocess/TimePreprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/preprocess/UnivariatePreprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/preprocess/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:47:17.746317 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/shared/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/shared/_update_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/shared/distribution_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-03-19 17:45:54.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/shared/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:47:17.746317 deephaven-plugin-plotly-express-0.6.0/src/deephaven_plugin_plotly_express.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-03-19 17:47:17.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven_plugin_plotly_express.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-03-19 17:47:17.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven_plugin_plotly_express.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 17:47:17.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven_plugin_plotly_express.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-19 17:47:17.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven_plugin_plotly_express.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-19 17:47:17.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven_plugin_plotly_express.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-19 17:47:17.000000 deephaven-plugin-plotly-express-0.6.0/src/deephaven_plugin_plotly_express.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:02:56.604569 deephaven-plugin-plotly-express-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-03 22:02:56.604569 deephaven-plugin-plotly-express-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-03 22:02:56.604569 deephaven-plugin-plotly-express-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:02:56.576569 deephaven-plugin-plotly-express-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:02:56.572569 deephaven-plugin-plotly-express-0.7.0/src/deephaven/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:02:56.572569 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:02:56.576569 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:02:56.576569 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/
+-rw-r--r--   0 runner    (1001) docker     (127)     9793 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:02:56.584569 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/DashboardPlugin.d.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      269 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/DashboardPlugin.d.ts.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/DashboardPlugin.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/DashboardPlugin.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      333 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChart.d.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      346 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChart.d.ts.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChart.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChart.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChartModel.d.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChartModel.d.ts.map
+-rw-r--r--   0 runner    (1001) docker     (127)    11457 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChartModel.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9508 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChartModel.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      333 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChartPanel.d.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      324 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChartPanel.d.ts.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChartPanel.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChartPanel.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChartUtils.d.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChartUtils.d.ts.map
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChartUtils.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChartUtils.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      258 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/PlotlyExpressPlugin.d.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      302 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/PlotlyExpressPlugin.d.ts.map
+-rw-r--r--   0 runner    (1001) docker     (127)      585 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/PlotlyExpressPlugin.js
+-rw-r--r--   0 runner    (1001) docker     (127)      515 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/PlotlyExpressPlugin.js.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:02:56.592569 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/bundle/
+-rw-r--r--   0 runner    (1001) docker     (127)  6658954 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/bundle/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)    69117 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/bundle/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)      265 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      239 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/index.d.ts.map
+-rw-r--r--   0 runner    (1001) docker     (127)      341 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      250 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/index.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      282 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/useHandleSceneTicks.d.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      278 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/useHandleSceneTicks.d.ts.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/useHandleSceneTicks.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/useHandleSceneTicks.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 1985-10-26 08:15:00.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_register.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:02:56.592569 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/communication/
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/communication/DeephavenFigureConnection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6178 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/communication/DeephavenFigureListener.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/communication/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:02:56.592569 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10305 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/data/data_generators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:02:56.596569 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/data_mapping/
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/data_mapping/DataMapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/data_mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6518 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/data_mapping/data_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/data_mapping/data_mapping_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/data_mapping/json_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:02:56.596569 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/deephaven_figure/
+-rw-r--r--   0 runner    (1001) docker     (127)    21616 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/deephaven_figure/DeephavenFigure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/deephaven_figure/RevisionManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/deephaven_figure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/deephaven_figure/custom_draw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34201 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/deephaven_figure/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:02:56.596569 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/exporter/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/exporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/exporter/export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:02:56.600569 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/plots/
+-rw-r--r--   0 runner    (1001) docker     (127)    25605 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/plots/PartitionManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19439 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/plots/_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17133 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/plots/_private_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10652 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/plots/area.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24048 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/plots/bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24302 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/plots/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7661 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/plots/financial.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20359 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/plots/hierarchial.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40152 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/plots/line.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38474 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/plots/maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/plots/pie.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37924 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/plots/scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10777 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/plots/subplots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:02:56.600569 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/preprocess/AttachedPreprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/preprocess/FreqPreprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8788 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/preprocess/HistPreprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/preprocess/Preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/preprocess/StyleManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/preprocess/TimePreprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/preprocess/UnivariatePreprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/preprocess/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:02:56.600569 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/shared/_update_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/shared/distribution_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-03 22:01:27.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/shared/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:02:56.604569 deephaven-plugin-plotly-express-0.7.0/src/deephaven_plugin_plotly_express.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-03 22:02:56.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven_plugin_plotly_express.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-04-03 22:02:56.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven_plugin_plotly_express.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 22:02:56.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven_plugin_plotly_express.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 22:02:56.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven_plugin_plotly_express.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-03 22:02:56.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven_plugin_plotly_express.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 22:02:56.000000 deephaven-plugin-plotly-express-0.7.0/src/deephaven_plugin_plotly_express.egg-info/top_level.txt
```

### Comparing `deephaven-plugin-plotly-express-0.6.0/LICENSE` & `deephaven-plugin-plotly-express-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/PKG-INFO` & `deephaven-plugin-plotly-express-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deephaven-plugin-plotly-express
-Version: 0.6.0
+Version: 0.7.0
 Summary: Deephaven Chart Plugin
 Home-page: https://github.com/deephaven/deephaven-plugins
 Author: Devin Smith, Vlad Babich, Joe Numainville
 Author-email: josephnumainville@deephaven.io
 Project-URL: Source Code, https://github.com/deephaven/deephaven-plugins
 Project-URL: Bug Tracker, https://github.com/deephaven/deephaven-plugins/issues
 Keywords: deephaven,plugin,graph
```

### Comparing `deephaven-plugin-plotly-express-0.6.0/README.md` & `deephaven-plugin-plotly-express-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/setup.cfg` & `deephaven-plugin-plotly-express-0.7.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = deephaven-plugin-plotly-express
 description = Deephaven Chart Plugin
 long_description = file: README.md
 long_description_content_type = text/markdown
-version = 0.6.0
+version = 0.7.0
 url = https://github.com/deephaven/deephaven-plugins
 project_urls = 
 	Source Code = https://github.com/deephaven/deephaven-plugins
 	Bug Tracker = https://github.com/deephaven/deephaven-plugins/issues
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: Apache Software License
```

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/__init__.py` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import json
 from typing import Any
 
 from deephaven.plugin.object_type import BidirectionalObjectType, MessageStream
+from plotly.graph_objs import Figure
 
 from .communication.DeephavenFigureConnection import DeephavenFigureConnection
 from .deephaven_figure import DeephavenFigure
 
 from .plots import (
     area,
     bar,
@@ -62,23 +63,24 @@
         Returns:
             The name of the plugin
         """
         return NAME
 
     def is_type(self, obj: Any) -> bool:
         """
-        Check if an object is a DeephavenFigure
+        Check if an object is a DeephavenFigure or Plotly Figure
+        Plotly figures are wrapped in DeephavenFigure when sent to the client
 
         Args:
           obj: The object to check
 
         Returns:
             True if the object is of the correct type, False otherwise
         """
-        return isinstance(obj, DeephavenFigure)
+        return isinstance(obj, DeephavenFigure) or isinstance(obj, Figure)
 
     def create_client_connection(
         self, obj: DeephavenFigure, connection: MessageStream
     ) -> MessageStream:
         """
         Create a client connection for the DeephavenFigure.
         This sends an initial figure to the client.
@@ -86,14 +88,18 @@
         Args:
           obj: The object to create the connection for
           connection: The connection to use
 
         Returns:
             The client connection
         """
+        if isinstance(obj, Figure):
+            # this is a plotly figure, it will never be updated, so wrap once and send
+            obj = DeephavenFigure(obj, is_plotly_fig=True)
+
         figure_connection = DeephavenFigureConnection(obj, connection)
         initial_message = json.dumps(
             {
                 "type": "RETRIEVE",
             }
         ).encode()
         payload, references = figure_connection.on_data(initial_message, [])
```

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/LICENSE` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/LICENSE`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/DashboardPlugin.js` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/DashboardPlugin.js`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/DashboardPlugin.js.map` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/DashboardPlugin.js.map`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChart.js` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChart.js`

 * *Files 17% similar despite different names*

#### js-beautify {}

```diff
@@ -20,34 +20,34 @@
 export function PlotlyExpressChart(props) {
     const dh = useApi();
     const {
         fetch
     } = props;
     const containerRef = useRef(null);
     const [model, setModel] = useState();
+    const [widgetRevision, setWidgetRevision] = useState(0); // Used to force a clean chart state on widget change
     useEffect(() => {
         let cancelled = false;
         async function init() {
             const widgetData = await fetch();
             if (!cancelled) {
                 setModel(new PlotlyExpressChartModel(dh, widgetData, fetch));
+                setWidgetRevision(r => r + 1);
             }
         }
         init();
         return () => {
             cancelled = true;
         };
     }, [dh, fetch]);
     useHandleSceneTicks(model, containerRef.current);
     return model ? (_jsx(Chart
         // eslint-disable-next-line react/jsx-props-no-spreading, @typescript-eslint/ban-ts-comment
         // @ts-ignore
         , {
-            // eslint-disable-next-line react/jsx-props-no-spreading, @typescript-eslint/ban-ts-comment
-            // @ts-ignore
             containerRef: containerRef,
             model: model,
             Plotly: Plotly
-        })) : null;
+        }, widgetRevision)) : null;
 }
 export default PlotlyExpressChart;
 //# sourceMappingURL=PlotlyExpressChart.js.map
```

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChart.js.map` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChart.js.map`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'mappings'": "';AAAA,OAAc,EAAE,SAAS,EAAE,MAAM,EAAE,QAAQ,EAAE,MAAM,OAAO,CAAC;AAC3D,OAAO,MAAM,MAAM,oBAAoB,CAAC;AACxC,OAAO,EAAE,KAAK,EAAE,MAAM,kBAAkB,CAAC;AAGzC,OAAO,EAAE,MAAM,EAAE,MAAM,4BAA4B,CAAC;AACpD,OAAO,uBAAuB,MAAM,8BAA8B,CAAC;AACnE,OAAO,EAAE,mBAAmB,EAAE,MAAM,0BAA0B,CAAC;AAE/D,MAAM,UAAU,kBAAkB,CAChC,KAAmC;IAEnC,MAAM,EAAE,GAAG,MAAM,EAAE,CAAC;IACpB,MAAM,EAAE,KAAK,EAAE,GAAG,KAAK,CAAC;IACxB,MAAM,YAAY,GAAG,MAAM,CAAiB,IAAI,CAAC,CAAC;IAClD,MAAM,CAAC,KAAK,EAAE,QAAQ,CAAC,GAAG,QAAQ,EAA2B,CAAC;IAC9D,MAAM,CAAC,cAA […]*

```diff
@@ -1,10 +1,10 @@
 {
     "file": "PlotlyExpressChart.js",
-    "mappings": ";AAAA,OAAc,EAAE,SAAS,EAAE,MAAM,EAAE,QAAQ,EAAE,MAAM,OAAO,CAAC;AAC3D,OAAO,MAAM,MAAM,oBAAoB,CAAC;AACxC,OAAO,EAAE,KAAK,EAAE,MAAM,kBAAkB,CAAC;AAGzC,OAAO,EAAE,MAAM,EAAE,MAAM,4BAA4B,CAAC;AACpD,OAAO,uBAAuB,MAAM,8BAA8B,CAAC;AACnE,OAAO,EAAE,mBAAmB,EAAE,MAAM,0BAA0B,CAAC;AAE/D,MAAM,UAAU,kBAAkB,CAChC,KAAmC;IAEnC,MAAM,EAAE,GAAG,MAAM,EAAE,CAAC;IACpB,MAAM,EAAE,KAAK,EAAE,GAAG,KAAK,CAAC;IACxB,MAAM,YAAY,GAAG,MAAM,CAAiB,IAAI,CAAC,CAAC;IAClD,MAAM,CAAC,KAAK,EAAE,QAAQ,CAAC,GAAG,QAAQ,EAA2B,CAAC;IAE9D,SAAS,CAAC,GAAG,EAAE;QACb,IAAI,SAAS,GAAG,KAAK,CAAC;QACtB,KAAK,UAAU,IAAI;YACjB,MAAM,UAAU,GAAG,MAAM,KAAK,EAAE,CAAC;YACjC,IAAI,CAAC,SAAS,EAAE;gBACd,QAAQ,CAAC,IAAI,uBAAuB,CAAC,EAAE,EAAE,UAAU,EAAE,KAAK,CAAC,CAAC,CAAC;aAC9D;QACH,CAAC;QAED,IAAI,EAAE,CAAC;QAEP,OAAO,GAAG,EAAE;YACV,SAAS,GAAG,IAAI,CAAC;QACnB,CAAC,CAAC;IACJ,CAAC,EAAE,CAAC,EAAE,EAAE,KAAK,CAAC,CAAC,CAAC;IAEhB,mBAAmB,CAAC,KAAK,EAAE,YAAY,CAAC,OAAO,CAAC,CAAC;IAEjD,OAAO,KAAK,CAAC,CAAC,CAAC,CACb,KAAC,KAAK;IACJ,2FAA2F;IAC3F,aAAa;;QADb,2FAA2F;QAC3F,aAAa;QACb,YAAY,EAAE,YAAY,EAC1B,KAAK,EAAE,KAAK,EACZ,MAAM,EAAE,MAAM,GACd,CACH,CAAC,CAAC,CAAC,IAAI,CAAC;AACX,CAAC;AAED,eAAe,kBAAkB,CAAC",
+    "mappings": ";AAAA,OAAc,EAAE,SAAS,EAAE,MAAM,EAAE,QAAQ,EAAE,MAAM,OAAO,CAAC;AAC3D,OAAO,MAAM,MAAM,oBAAoB,CAAC;AACxC,OAAO,EAAE,KAAK,EAAE,MAAM,kBAAkB,CAAC;AAGzC,OAAO,EAAE,MAAM,EAAE,MAAM,4BAA4B,CAAC;AACpD,OAAO,uBAAuB,MAAM,8BAA8B,CAAC;AACnE,OAAO,EAAE,mBAAmB,EAAE,MAAM,0BAA0B,CAAC;AAE/D,MAAM,UAAU,kBAAkB,CAChC,KAAmC;IAEnC,MAAM,EAAE,GAAG,MAAM,EAAE,CAAC;IACpB,MAAM,EAAE,KAAK,EAAE,GAAG,KAAK,CAAC;IACxB,MAAM,YAAY,GAAG,MAAM,CAAiB,IAAI,CAAC,CAAC;IAClD,MAAM,CAAC,KAAK,EAAE,QAAQ,CAAC,GAAG,QAAQ,EAA2B,CAAC;IAC9D,MAAM,CAAC,cAAc,EAAE,iBAAiB,CAAC,GAAG,QAAQ,CAAC,CAAC,CAAC,CAAC,CAAC,qDAAqD;IAE9G,SAAS,CAAC,GAAG,EAAE;QACb,IAAI,SAAS,GAAG,KAAK,CAAC;QACtB,KAAK,UAAU,IAAI;YACjB,MAAM,UAAU,GAAG,MAAM,KAAK,EAAE,CAAC;YACjC,IAAI,CAAC,SAAS,EAAE;gBACd,QAAQ,CAAC,IAAI,uBAAuB,CAAC,EAAE,EAAE,UAAU,EAAE,KAAK,CAAC,CAAC,CAAC;gBAC7D,iBAAiB,CAAC,CAAC,CAAC,EAAE,CAAC,CAAC,GAAG,CAAC,CAAC,CAAC;aAC/B;QACH,CAAC;QAED,IAAI,EAAE,CAAC;QAEP,OAAO,GAAG,EAAE;YACV,SAAS,GAAG,IAAI,CAAC;QACnB,CAAC,CAAC;IACJ,CAAC,EAAE,CAAC,EAAE,EAAE,KAAK,CAAC,CAAC,CAAC;IAEhB,mBAAmB,CAAC,KAAK,EAAE,YAAY,CAAC,OAAO,CAAC,CAAC;IAEjD,OAAO,KAAK,CAAC,CAAC,CAAC,CACb,KAAC,KAAK;IACJ,2FAA2F;IAC3F,aAAa;QAEb,YAAY,EAAE,YAAY,EAC1B,KAAK,EAAE,KAAK,EACZ,MAAM,EAAE,MAAM,IAHT,cAAc,CAInB,CACH,CAAC,CAAC,CAAC,IAAI,CAAC;AACX,CAAC;AAED,eAAe,kBAAkB,CAAC",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "../src/PlotlyExpressChart.tsx"
     ],
     "version": 3
 }
```

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChartModel.d.ts` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChartModel.d.ts`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChartModel.d.ts.map` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChartModel.d.ts.map`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChartModel.js` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChartModel.js`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChartModel.js.map` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChartModel.js.map`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChartPanel.js` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChartPanel.js`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChartPanel.js.map` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChartPanel.js.map`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChartUtils.d.ts` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChartUtils.d.ts`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChartUtils.d.ts.map` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChartUtils.d.ts.map`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChartUtils.js` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChartUtils.js`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChartUtils.js.map` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/PlotlyExpressChartUtils.js.map`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/PlotlyExpressPlugin.js` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/PlotlyExpressPlugin.js`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/PlotlyExpressPlugin.js.map` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/PlotlyExpressPlugin.js.map`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/bundle/index.js` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/bundle/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -155754,34 +155754,37 @@
 function PlotlyExpressChart(props) {
     const dh = jsapiBootstrap.useApi();
     const {
         fetch
     } = props;
     const containerRef = React.useRef(null);
     const [model, setModel] = React.useState();
+    const [widgetRevision, setWidgetRevision] = React.useState(0);
     React.useEffect(() => {
         let cancelled = false;
         async function init2() {
             const widgetData = await fetch();
             if (!cancelled) {
                 setModel(new PlotlyExpressChartModel(dh, widgetData, fetch));
+                setWidgetRevision((r2) => r2 + 1);
             }
         }
         init2();
         return () => {
             cancelled = true;
         };
     }, [dh, fetch]);
     useHandleSceneTicks(model, containerRef.current);
     return model ? /* @__PURE__ */ jsxRuntimeExports.jsx(
         chart.Chart, {
             containerRef,
             model,
             Plotly
-        }
+        },
+        widgetRevision
     ) : null;
 }
 var toStr$9 = Object.prototype.toString;
 var isArguments$3 = function isArguments(value) {
     var str = toStr$9.call(value);
     var isArgs2 = str === "[object Arguments]";
     if (!isArgs2) {
```

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/bundle/style.css` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/bundle/style.css`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/useHandleSceneTicks.js` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/useHandleSceneTicks.js`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/dist/useHandleSceneTicks.js.map` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/dist/useHandleSceneTicks.js.map`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js/package.json` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9722222222222222%*

 * *Differences: {"'version'": "'0.7.0'"}*

```diff
@@ -68,9 +68,9 @@
     },
     "scripts": {
         "build": "tsc && vite build",
         "start": "vite build --watch",
         "update-dh-packages": "node ../../../../tools/update-dh-packages.mjs"
     },
     "type": "module",
-    "version": "0.6.0"
+    "version": "0.7.0"
 }
```

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/_js_plugin.py` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/_js_plugin.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/communication/DeephavenFigureConnection.py` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/communication/DeephavenFigureConnection.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/communication/DeephavenFigureListener.py` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/communication/DeephavenFigureListener.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/data/data_generators.py` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/data/data_generators.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/data_mapping/DataMapping.py` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/data_mapping/DataMapping.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/data_mapping/data_mapping.py` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/data_mapping/data_mapping.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/data_mapping/data_mapping_constants.py` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/data_mapping/data_mapping_constants.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/data_mapping/json_conversion.py` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/data_mapping/json_conversion.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/deephaven_figure/DeephavenFigure.py` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/deephaven_figure/DeephavenFigure.py`

 * *Files 1% similar despite different names*

```diff
@@ -390,27 +390,29 @@
         fig: Figure | None = None,
         call_args: dict[str, Any] | None = None,
         data_mappings: list[DataMapping] | None = None,
         has_template: bool = False,
         has_color: bool = False,
         trace_generator: Generator[dict[str, Any], None, None] | None = None,
         has_subplots: bool = False,
+        is_plotly_fig: bool = False,
     ):
         """
         Create a new DeephavenFigure
 
         Args:
             fig: The plotly figure
             call_args: Call args, used to determine if the figure
                 has a template or color
             data_mappings: The data mappings
             has_template: If this figure has a template
             has_color: If this figure has color
             trace_generator: The trace generator
             has_subplots: If this figure has subplots
+            is_plotly_fig: If this is a plotly figure
         """
         # keep track of function that called this, and it's args
         self._head_node = DeephavenHeadNode()
 
         # note: these variables might not be up-to-date with the latest
         # figure if the figure is updated
         self._plotly_fig = fig
@@ -424,14 +426,16 @@
 
         self._call_args = call_args
 
         self._data_mappings = data_mappings if data_mappings else []
 
         self._has_subplots = has_subplots
 
+        self._is_plotly_fig = is_plotly_fig
+
         self._liveness_scope = LivenessScope()
 
     def copy_mappings(self: DeephavenFigure, offset: int = 0) -> list[DataMapping]:
         """Copy all DataMappings within this figure, adding a specific offset
 
         Args:
           offset: The offset to offset the copy by
@@ -580,14 +584,18 @@
     def get_figure(self) -> DeephavenFigure | None:
         """
         Get the true DeephavenFigure for this figure.
 
         Returns:
             The figure
         """
+        if self._is_plotly_fig:
+            # a plotly figure was passed directly
+            # just return this figure since it will never be updated
+            return self
         return self._head_node.get_figure()
 
     def get_plotly_fig(self) -> Figure | None:
         """
         Get the plotly figure for this figure
 
         Returns:
@@ -672,14 +680,15 @@
             self._plotly_fig,
             self._call_args,
             self._data_mappings,
             self._has_template,
             self._has_color,
             self._trace_generator,
             self._has_subplots,
+            self._is_plotly_fig,
         )
         new_figure._head_node = self._head_node.copy_graph()
         return new_figure
 
     def recreate_figure(self) -> None:
         """
         Recreate the figure. This is called to ensure the figure is up-to-date
```

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/deephaven_figure/RevisionManager.py` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/deephaven_figure/RevisionManager.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/deephaven_figure/custom_draw.py` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/deephaven_figure/custom_draw.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/deephaven_figure/generate.py` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/deephaven_figure/generate.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/exporter/export.py` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/exporter/export.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/plots/PartitionManager.py` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/plots/PartitionManager.py`

 * *Files 1% similar despite different names*

```diff
@@ -599,15 +599,17 @@
 
         Returns:
             The default figure
         """
         # this is very hacky but it's needed to prevent errors when
         # there are no partitions until a better solution can be done
         # also need the px template to be set
-        default_fig = px.scatter(x=[0], y=[0])
+        # the title can also be set here as it will never change
+        title = self.args.get("title")
+        default_fig = px.scatter(x=[0], y=[0], title=title)
         default_fig.update_traces(x=[], y=[])
         return DeephavenFigure(default_fig)
 
     def create_figure(self) -> DeephavenFigure:
         """
         Create a figure. This handles layering different partitions as necessary as well
         as any special preprocessing or postprocessing needed for different types of plots
```

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/plots/__init__.py` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/plots/_layer.py` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/plots/_layer.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/plots/_private_utils.py` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/plots/_private_utils.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/plots/area.py` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/plots/area.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/plots/bar.py` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/plots/bar.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/plots/distribution.py` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/plots/distribution.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/plots/financial.py` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/plots/financial.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/plots/hierarchial.py` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/plots/hierarchial.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/plots/line.py` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/plots/line.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/plots/maps.py` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/plots/maps.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/plots/pie.py` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/plots/pie.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/plots/scatter.py` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/plots/scatter.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/plots/subplots.py` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/plots/subplots.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/preprocess/AttachedPreprocessor.py` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/preprocess/AttachedPreprocessor.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/preprocess/FreqPreprocessor.py` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/preprocess/FreqPreprocessor.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/preprocess/HistPreprocessor.py` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/preprocess/HistPreprocessor.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/preprocess/Preprocessor.py` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/preprocess/Preprocessor.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/preprocess/StyleManager.py` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/preprocess/StyleManager.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/preprocess/TimePreprocessor.py` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/preprocess/TimePreprocessor.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/preprocess/UnivariatePreprocessor.py` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/preprocess/UnivariatePreprocessor.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/preprocess/preprocess.py` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/preprocess/preprocess.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/shared/_update_wrapper.py` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/shared/_update_wrapper.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/shared/distribution_args.py` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/shared/distribution_args.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven/plot/express/shared/shared.py` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven/plot/express/shared/shared.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven_plugin_plotly_express.egg-info/PKG-INFO` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven_plugin_plotly_express.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deephaven-plugin-plotly-express
-Version: 0.6.0
+Version: 0.7.0
 Summary: Deephaven Chart Plugin
 Home-page: https://github.com/deephaven/deephaven-plugins
 Author: Devin Smith, Vlad Babich, Joe Numainville
 Author-email: josephnumainville@deephaven.io
 Project-URL: Source Code, https://github.com/deephaven/deephaven-plugins
 Project-URL: Bug Tracker, https://github.com/deephaven/deephaven-plugins/issues
 Keywords: deephaven,plugin,graph
```

### Comparing `deephaven-plugin-plotly-express-0.6.0/src/deephaven_plugin_plotly_express.egg-info/SOURCES.txt` & `deephaven-plugin-plotly-express-0.7.0/src/deephaven_plugin_plotly_express.egg-info/SOURCES.txt`

 * *Files identical despite different names*

