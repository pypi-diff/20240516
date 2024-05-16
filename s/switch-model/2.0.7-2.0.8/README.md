# Comparing `tmp/switch_model-2.0.7.tar.gz` & `tmp/switch_model-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "switch_model-2.0.7.tar", last modified: Wed Nov  2 00:33:46 2022, max compression
+gzip compressed data, was "switch_model-2.0.8.tar", last modified: Thu Apr 25 22:11:43 2024, max compression
```

## Comparing `switch_model-2.0.7.tar` & `switch_model-2.0.8.tar`

### file list

```diff
@@ -1,1033 +1,1092 @@
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.860471 switch_model-2.0.7/
--rw-r--r--   0 matthias   (501) wheel        (0)      789 2022-11-02 00:23:51.000000 switch_model-2.0.7/AUTHORS
--rw-r--r--   0 matthias   (501) wheel        (0)     4174 2022-11-02 00:23:51.000000 switch_model-2.0.7/DEV_INSTALL.txt
--rw-r--r--   0 matthias   (501) wheel        (0)    11529 2022-11-02 00:23:51.000000 switch_model-2.0.7/LICENSE
--rw-r--r--   0 matthias   (501) wheel        (0)      735 2022-11-02 00:23:51.000000 switch_model-2.0.7/LICENSE.BOILERPLATE
--rw-r--r--   0 matthias   (501) wheel        (0)      216 2022-11-02 00:23:51.000000 switch_model-2.0.7/MANIFEST.in
--rw-r--r--   0 matthias   (501) wheel        (0)     5512 2022-11-02 00:33:46.860306 switch_model-2.0.7/PKG-INFO
--rw-r--r--   0 matthias   (501) wheel        (0)     4167 2022-11-02 00:23:51.000000 switch_model-2.0.7/README
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.623207 switch_model-2.0.7/examples/
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.630166 switch_model-2.0.7/examples/3zone_toy/
--rw-r--r--   0 matthias   (501) wheel        (0)      309 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy/README.md
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.634262 switch_model-2.0.7/examples/3zone_toy/inputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy/inputs/financials.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      487 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy/inputs/fuel_cost.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      514 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy/inputs/fuel_supply_curves.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      179 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy/inputs/fuels.csv
--rw-r--r--   0 matthias   (501) wheel        (0)     2704 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy/inputs/gen_build_costs.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      233 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy/inputs/gen_build_predetermined.csv
--rw-r--r--   0 matthias   (501) wheel        (0)     3812 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy/inputs/gen_info.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      161 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy/inputs/load_zones.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      303 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy/inputs/loads.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      470 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy/inputs/modules.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       54 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy/inputs/non_fuel_energy_sources.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       72 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy/inputs/periods.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      112 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy/inputs/regional_fuel_markets.csv
--rw-r--r--   0 matthias   (501) wheel        (0)        6 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy/inputs/switch_inputs_version.txt
--rw-r--r--   0 matthias   (501) wheel        (0)      218 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy/inputs/timepoints.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      158 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy/inputs/timeseries.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       87 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy/inputs/trans_params.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      148 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy/inputs/transmission_lines.csv
--rw-r--r--   0 matthias   (501) wheel        (0)     2365 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy/inputs/variable_capacity_factors.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       77 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy/inputs/zone_balancing_areas.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      138 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy/inputs/zone_coincident_peak_demand.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      299 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy/inputs/zone_fuel_cost_diff.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      160 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy/inputs/zone_to_regional_fuel_market.csv
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.634422 switch_model-2.0.7/examples/3zone_toy/outputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       19 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy/outputs/total_cost.txt
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.635949 switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/
--rw-r--r--   0 matthias   (501) wheel        (0)     7183 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/PySPInputGenerator.py
--rw-r--r--   0 matthias   (501) wheel        (0)    11070 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/README.md
--rw-r--r--   0 matthias   (501) wheel        (0)     3627 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/ReferenceModel.py
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.640239 switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/inputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/inputs/financials.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      566 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/inputs/fuel_cost.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      191 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/inputs/fuels.csv
--rw-r--r--   0 matthias   (501) wheel        (0)     2704 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/inputs/gen_build_costs.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      233 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/inputs/gen_build_predetermined.csv
--rw-r--r--   0 matthias   (501) wheel        (0)     3689 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/inputs/gen_info.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      124 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/inputs/load_zones.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      303 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/inputs/loads.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      469 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/inputs/modules.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       54 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/inputs/non_fuel_energy_sources.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       72 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/inputs/periods.csv
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.642381 switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/inputs/pysp_inputs/
--rw-r--r--   0 matthias   (501) wheel        (0)      429 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/inputs/pysp_inputs/HighFuelCosts.dat
--rw-r--r--   0 matthias   (501) wheel        (0)      432 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/inputs/pysp_inputs/LowFuelCosts.dat
--rw-r--r--   0 matthias   (501) wheel        (0)        0 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/inputs/pysp_inputs/MediumFuelCosts.dat
--rw-r--r--   0 matthias   (501) wheel        (0)    25575 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/inputs/pysp_inputs/RootNode.dat
--rw-r--r--   0 matthias   (501) wheel        (0)     1039 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/inputs/pysp_inputs/ScenarioStructure.dat
--rw-r--r--   0 matthias   (501) wheel        (0)        6 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/inputs/switch_inputs_version.txt
--rw-r--r--   0 matthias   (501) wheel        (0)      218 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/inputs/timepoints.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      158 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/inputs/timeseries.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      148 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/inputs/transmission_lines.csv
--rw-r--r--   0 matthias   (501) wheel        (0)     2365 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/inputs/variable_capacity_factors.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       77 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/inputs/zone_balancing_areas.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      138 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/inputs/zone_coincident_peak_demand.csv
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.643165 switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/outputs-runef/
--rw-r--r--   0 matthias   (501) wheel        (0)    69326 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/outputs-runef/ef.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      528 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/outputs-runef/ef_StageCostDetail.csv
--rw-r--r--   0 matthias   (501) wheel        (0)    22488 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/outputs-runef/runef-stdoutput.txt
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.644250 switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/outputs-runph-rhosetter/
--rw-r--r--   0 matthias   (501) wheel        (0)    70071 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/outputs-runph-rhosetter/ph.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      529 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/outputs-runph-rhosetter/ph_StageCostDetail.csv
--rw-r--r--   0 matthias   (501) wheel        (0)    62632 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/outputs-runph-rhosetter/runph-rhosetter-stdoutput.txt
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.646316 switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/outputs-runph-rhosetter-FS-only/
--rw-r--r--   0 matthias   (501) wheel        (0)    70071 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/outputs-runph-rhosetter-FS-only/ph.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      529 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/outputs-runph-rhosetter-FS-only/ph_StageCostDetail.csv
--rw-r--r--   0 matthias   (501) wheel        (0)    62644 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/outputs-runph-rhosetter-FS-only/runph-rhosetter-FS-only-stdoutput.txt
--rw-r--r--   0 matthias   (501) wheel        (0)     1426 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/pha_bounds_cfg.py
--rw-r--r--   0 matthias   (501) wheel        (0)     3211 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/rhosetter.py
--rw-r--r--   0 matthias   (501) wheel        (0)     1639 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/rhosetter_FS_only.py
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.646892 switch_model-2.0.7/examples/carbon_cap/
--rw-r--r--   0 matthias   (501) wheel        (0)      236 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/carbon_cap/README.md
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.650762 switch_model-2.0.7/examples/carbon_cap/inputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       84 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/carbon_cap/inputs/carbon_policies.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/carbon_cap/inputs/financials.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      487 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/carbon_cap/inputs/fuel_cost.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      514 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/carbon_cap/inputs/fuel_supply_curves.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      191 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/carbon_cap/inputs/fuels.csv
--rw-r--r--   0 matthias   (501) wheel        (0)     2704 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/carbon_cap/inputs/gen_build_costs.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      233 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/carbon_cap/inputs/gen_build_predetermined.csv
--rw-r--r--   0 matthias   (501) wheel        (0)     3818 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/carbon_cap/inputs/gen_info.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      124 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/carbon_cap/inputs/load_zones.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      303 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/carbon_cap/inputs/loads.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      508 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/carbon_cap/inputs/modules.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       54 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/carbon_cap/inputs/non_fuel_energy_sources.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       72 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/carbon_cap/inputs/periods.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      112 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/carbon_cap/inputs/regional_fuel_markets.csv
--rw-r--r--   0 matthias   (501) wheel        (0)        6 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/carbon_cap/inputs/switch_inputs_version.txt
--rw-r--r--   0 matthias   (501) wheel        (0)      218 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/carbon_cap/inputs/timepoints.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      158 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/carbon_cap/inputs/timeseries.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      148 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/carbon_cap/inputs/transmission_lines.csv
--rw-r--r--   0 matthias   (501) wheel        (0)     2365 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/carbon_cap/inputs/variable_capacity_factors.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       77 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/carbon_cap/inputs/zone_balancing_areas.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      138 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/carbon_cap/inputs/zone_coincident_peak_demand.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      299 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/carbon_cap/inputs/zone_fuel_cost_diff.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      160 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/carbon_cap/inputs/zone_to_regional_fuel_market.csv
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.651361 switch_model-2.0.7/examples/carbon_cap/outputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       19 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/carbon_cap/outputs/total_cost.txt
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.651748 switch_model-2.0.7/examples/ccs/
--rw-r--r--   0 matthias   (501) wheel        (0)      129 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/ccs/README.md
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.654796 switch_model-2.0.7/examples/ccs/inputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/ccs/inputs/financials.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       56 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/ccs/inputs/fuel_cost.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/ccs/inputs/fuels.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      262 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/ccs/inputs/gen_build_costs.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      111 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/ccs/inputs/gen_build_predetermined.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      596 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/ccs/inputs/gen_info.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       60 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/ccs/inputs/load_zones.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       59 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/ccs/inputs/loads.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      347 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/ccs/inputs/modules.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       31 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/ccs/inputs/non_fuel_energy_sources.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       57 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/ccs/inputs/periods.csv
--rw-r--r--   0 matthias   (501) wheel        (0)        6 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/ccs/inputs/switch_inputs_version.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       78 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/ccs/inputs/timepoints.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       95 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/ccs/inputs/timeseries.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       96 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/ccs/inputs/variable_capacity_factors.csv
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.654949 switch_model-2.0.7/examples/ccs/outputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       19 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/ccs/outputs/total_cost.txt
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.655083 switch_model-2.0.7/examples/copperplate0/
--rw-r--r--   0 matthias   (501) wheel        (0)      262 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/copperplate0/README.md
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.660202 switch_model-2.0.7/examples/copperplate0/inputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/copperplate0/inputs/financials.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       56 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/copperplate0/inputs/fuel_cost.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/copperplate0/inputs/fuels.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      262 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/copperplate0/inputs/gen_build_costs.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      111 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/copperplate0/inputs/gen_build_predetermined.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      532 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/copperplate0/inputs/gen_info.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       16 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/copperplate0/inputs/load_zones.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       59 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/copperplate0/inputs/loads.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      347 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/copperplate0/inputs/modules.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       31 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/copperplate0/inputs/non_fuel_energy_sources.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       57 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/copperplate0/inputs/periods.csv
--rw-r--r--   0 matthias   (501) wheel        (0)        6 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/copperplate0/inputs/switch_inputs_version.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       78 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/copperplate0/inputs/timepoints.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       95 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/copperplate0/inputs/timeseries.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       96 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/copperplate0/inputs/variable_capacity_factors.csv
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.660319 switch_model-2.0.7/examples/copperplate0/outputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       18 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/copperplate0/outputs/total_cost.txt
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.660453 switch_model-2.0.7/examples/copperplate1/
--rw-r--r--   0 matthias   (501) wheel        (0)      336 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/copperplate1/README.md
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.667750 switch_model-2.0.7/examples/copperplate1/inputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/copperplate1/inputs/financials.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      187 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/copperplate1/inputs/fuel_supply_curves.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       91 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/copperplate1/inputs/fuels.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      466 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/copperplate1/inputs/gen_build_costs.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      119 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/copperplate1/inputs/gen_build_predetermined.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      974 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/copperplate1/inputs/gen_info.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       73 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/copperplate1/inputs/load_zones.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       59 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/copperplate1/inputs/loads.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      383 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/copperplate1/inputs/modules.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       31 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/copperplate1/inputs/non_fuel_energy_sources.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       57 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/copperplate1/inputs/periods.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/copperplate1/inputs/regional_fuel_markets.csv
--rw-r--r--   0 matthias   (501) wheel        (0)        6 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/copperplate1/inputs/switch_inputs_version.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       78 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/copperplate1/inputs/timepoints.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       95 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/copperplate1/inputs/timeseries.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      231 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/copperplate1/inputs/variable_capacity_factors.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       60 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/copperplate1/inputs/zone_to_regional_fuel_market.csv
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.667977 switch_model-2.0.7/examples/copperplate1/outputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       18 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/copperplate1/outputs/total_cost.txt
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.669971 switch_model-2.0.7/examples/custom_extension/
--rw-r--r--   0 matthias   (501) wheel        (0)      235 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/custom_extension/README
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.670431 switch_model-2.0.7/examples/custom_extension/__pycache__/
--rw-r--r--   0 matthias   (501) wheel        (0)     1276 2022-11-02 00:28:58.000000 switch_model-2.0.7/examples/custom_extension/__pycache__/sunk_costs.cpython-310.pyc
--rw-r--r--   0 matthias   (501) wheel        (0)     1258 2022-11-02 00:24:42.000000 switch_model-2.0.7/examples/custom_extension/__pycache__/sunk_costs.cpython-37.pyc
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.673896 switch_model-2.0.7/examples/custom_extension/inputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/custom_extension/inputs/financials.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       56 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/custom_extension/inputs/fuel_cost.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/custom_extension/inputs/fuels.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      262 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/custom_extension/inputs/gen_build_costs.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      111 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/custom_extension/inputs/gen_build_predetermined.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      532 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/custom_extension/inputs/gen_info.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       60 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/custom_extension/inputs/load_zones.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       59 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/custom_extension/inputs/loads.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      358 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/custom_extension/inputs/modules.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       31 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/custom_extension/inputs/non_fuel_energy_sources.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       57 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/custom_extension/inputs/periods.csv
--rw-r--r--   0 matthias   (501) wheel        (0)        6 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/custom_extension/inputs/switch_inputs_version.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       78 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/custom_extension/inputs/timepoints.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       95 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/custom_extension/inputs/timeseries.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       96 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/custom_extension/inputs/variable_capacity_factors.csv
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.675665 switch_model-2.0.7/examples/custom_extension/outputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       18 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/custom_extension/outputs/total_cost.txt
--rw-r--r--   0 matthias   (501) wheel        (0)     1060 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/custom_extension/sunk_costs.py
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.675895 switch_model-2.0.7/examples/diagnose_infeasibility/
--rw-r--r--   0 matthias   (501) wheel        (0)     1385 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/diagnose_infeasibility/README.md
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.680654 switch_model-2.0.7/examples/diagnose_infeasibility/inputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/diagnose_infeasibility/inputs/financials.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       56 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/diagnose_infeasibility/inputs/fuel_cost.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/diagnose_infeasibility/inputs/fuels.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      128 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/diagnose_infeasibility/inputs/gen_build_costs.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      533 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/diagnose_infeasibility/inputs/gen_info.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       60 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/diagnose_infeasibility/inputs/load_zones.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       59 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/diagnose_infeasibility/inputs/loads.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      428 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/diagnose_infeasibility/inputs/modules.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       31 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/diagnose_infeasibility/inputs/non_fuel_energy_sources.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       57 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/diagnose_infeasibility/inputs/periods.csv
--rw-r--r--   0 matthias   (501) wheel        (0)        6 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/diagnose_infeasibility/inputs/switch_inputs_version.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       78 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/diagnose_infeasibility/inputs/timepoints.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       95 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/diagnose_infeasibility/inputs/timeseries.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       96 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/diagnose_infeasibility/inputs/variable_capacity_factors.csv
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.681329 switch_model-2.0.7/examples/diagnose_infeasibility/outputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       18 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/diagnose_infeasibility/outputs/total_cost.txt
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.681813 switch_model-2.0.7/examples/discrete_and_min_build/
--rw-r--r--   0 matthias   (501) wheel        (0)      443 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/discrete_and_min_build/README.md
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.686816 switch_model-2.0.7/examples/discrete_and_min_build/inputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/discrete_and_min_build/inputs/financials.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       79 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/discrete_and_min_build/inputs/fuel_supply_curves.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/discrete_and_min_build/inputs/fuels.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      262 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/discrete_and_min_build/inputs/gen_build_costs.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      111 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/discrete_and_min_build/inputs/gen_build_predetermined.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      553 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/discrete_and_min_build/inputs/gen_info.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       73 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/discrete_and_min_build/inputs/load_zones.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       59 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/discrete_and_min_build/inputs/loads.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      431 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/discrete_and_min_build/inputs/modules.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       31 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/discrete_and_min_build/inputs/non_fuel_energy_sources.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       57 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/discrete_and_min_build/inputs/periods.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       44 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/discrete_and_min_build/inputs/regional_fuel_markets.csv
--rw-r--r--   0 matthias   (501) wheel        (0)        6 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/discrete_and_min_build/inputs/switch_inputs_version.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       78 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/discrete_and_min_build/inputs/timepoints.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       95 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/discrete_and_min_build/inputs/timeseries.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       96 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/discrete_and_min_build/inputs/variable_capacity_factors.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       68 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/discrete_and_min_build/inputs/zone_coincident_peak_demand.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       44 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/discrete_and_min_build/inputs/zone_to_regional_fuel_market.csv
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.687354 switch_model-2.0.7/examples/discrete_and_min_build/outputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       19 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/discrete_and_min_build/outputs/total_cost.txt
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.687545 switch_model-2.0.7/examples/discrete_build/
--rw-r--r--   0 matthias   (501) wheel        (0)      317 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/discrete_build/README.md
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.690452 switch_model-2.0.7/examples/discrete_build/inputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/discrete_build/inputs/financials.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       79 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/discrete_build/inputs/fuel_supply_curves.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/discrete_build/inputs/fuels.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      262 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/discrete_build/inputs/gen_build_costs.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      111 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/discrete_build/inputs/gen_build_predetermined.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      553 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/discrete_build/inputs/gen_info.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       73 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/discrete_build/inputs/load_zones.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       59 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/discrete_build/inputs/loads.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      431 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/discrete_build/inputs/modules.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       31 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/discrete_build/inputs/non_fuel_energy_sources.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       57 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/discrete_build/inputs/periods.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       44 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/discrete_build/inputs/regional_fuel_markets.csv
--rw-r--r--   0 matthias   (501) wheel        (0)        6 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/discrete_build/inputs/switch_inputs_version.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       78 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/discrete_build/inputs/timepoints.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       95 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/discrete_build/inputs/timeseries.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       96 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/discrete_build/inputs/variable_capacity_factors.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       68 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/discrete_build/inputs/zone_coincident_peak_demand.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       44 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/discrete_build/inputs/zone_to_regional_fuel_market.csv
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.690869 switch_model-2.0.7/examples/discrete_build/outputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       18 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/discrete_build/outputs/total_cost.txt
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.691027 switch_model-2.0.7/examples/dr_simple/
--rw-r--r--   0 matthias   (501) wheel        (0)      378 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/dr_simple/README.md
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.695121 switch_model-2.0.7/examples/dr_simple/inputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       86 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/dr_simple/inputs/dr_data.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/dr_simple/inputs/financials.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      187 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/dr_simple/inputs/fuel_supply_curves.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       91 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/dr_simple/inputs/fuels.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      466 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/dr_simple/inputs/gen_build_costs.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      128 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/dr_simple/inputs/gen_build_predetermined.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      974 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/dr_simple/inputs/gen_info.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       73 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/dr_simple/inputs/load_zones.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       59 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/dr_simple/inputs/loads.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      563 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/dr_simple/inputs/modules.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       31 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/dr_simple/inputs/non_fuel_energy_sources.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       57 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/dr_simple/inputs/periods.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/dr_simple/inputs/regional_fuel_markets.csv
--rw-r--r--   0 matthias   (501) wheel        (0)        6 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/dr_simple/inputs/switch_inputs_version.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       78 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/dr_simple/inputs/timepoints.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       95 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/dr_simple/inputs/timeseries.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      231 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/dr_simple/inputs/variable_capacity_factors.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       60 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/dr_simple/inputs/zone_to_regional_fuel_market.csv
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.695296 switch_model-2.0.7/examples/dr_simple/outputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       18 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/dr_simple/outputs/total_cost.txt
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.695427 switch_model-2.0.7/examples/hydro_simple/
--rw-r--r--   0 matthias   (501) wheel        (0)      547 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/hydro_simple/README.md
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.698225 switch_model-2.0.7/examples/hydro_simple/inputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/hydro_simple/inputs/financials.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       56 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/hydro_simple/inputs/fuel_cost.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/hydro_simple/inputs/fuels.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      343 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/hydro_simple/inputs/gen_build_costs.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      161 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/hydro_simple/inputs/gen_build_predetermined.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      671 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/hydro_simple/inputs/gen_info.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      114 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/hydro_simple/inputs/hydro_timeseries.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       60 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/hydro_simple/inputs/load_zones.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       84 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/hydro_simple/inputs/loads.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      395 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/hydro_simple/inputs/modules.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       37 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/hydro_simple/inputs/non_fuel_energy_sources.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       57 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/hydro_simple/inputs/periods.csv
--rw-r--r--   0 matthias   (501) wheel        (0)        6 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/hydro_simple/inputs/switch_inputs_version.txt
--rw-r--r--   0 matthias   (501) wheel        (0)      134 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/hydro_simple/inputs/timepoints.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      123 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/hydro_simple/inputs/timeseries.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      204 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/hydro_simple/inputs/variable_capacity_factors.csv
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.698343 switch_model-2.0.7/examples/hydro_simple/outputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       19 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/hydro_simple/outputs/total_cost.txt
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.698458 switch_model-2.0.7/examples/hydro_system/
--rw-r--r--   0 matthias   (501) wheel        (0)     1531 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/hydro_system/README.md
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.701721 switch_model-2.0.7/examples/hydro_system/inputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/hydro_system/inputs/financials.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       57 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/hydro_system/inputs/fuel_cost.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       57 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/hydro_system/inputs/fuels.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      196 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/hydro_system/inputs/gen_build_costs.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      180 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/hydro_system/inputs/gen_build_predetermined.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      667 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/hydro_system/inputs/gen_info.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      186 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/hydro_system/inputs/hydro_generation_projects.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       61 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/hydro_system/inputs/load_zones.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      643 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/hydro_system/inputs/loads.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      395 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/hydro_system/inputs/modules.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       26 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/hydro_system/inputs/non_fuel_energy_sources.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       57 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/hydro_system/inputs/periods.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      124 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/hydro_system/inputs/reservoirs.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       21 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/hydro_system/inputs/spillage_penalty.csv
--rw-r--r--   0 matthias   (501) wheel        (0)        6 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/hydro_system/inputs/switch_inputs_version.txt
--rw-r--r--   0 matthias   (501) wheel        (0)     1609 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/hydro_system/inputs/timepoints.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      143 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/hydro_system/inputs/timeseries.csv
--rw-r--r--   0 matthias   (501) wheel        (0)     1244 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/hydro_system/inputs/variable_capacity_factors.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      183 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/hydro_system/inputs/water_connections.csv
--rw-r--r--   0 matthias   (501) wheel        (0)     1290 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/hydro_system/inputs/water_node_tp_flows.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      147 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/hydro_system/inputs/water_nodes.csv
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.701848 switch_model-2.0.7/examples/hydro_system/outputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       18 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/hydro_system/outputs/total_cost.txt
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.701970 switch_model-2.0.7/examples/new_builds_only/
--rw-r--r--   0 matthias   (501) wheel        (0)      257 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/new_builds_only/README.md
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.706435 switch_model-2.0.7/examples/new_builds_only/inputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/new_builds_only/inputs/financials.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       56 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/new_builds_only/inputs/fuel_cost.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/new_builds_only/inputs/fuels.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      156 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/new_builds_only/inputs/gen_build_costs.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      532 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/new_builds_only/inputs/gen_info.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       60 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/new_builds_only/inputs/load_zones.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       59 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/new_builds_only/inputs/loads.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      347 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/new_builds_only/inputs/modules.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       31 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/new_builds_only/inputs/non_fuel_energy_sources.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       57 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/new_builds_only/inputs/periods.csv
--rw-r--r--   0 matthias   (501) wheel        (0)        6 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/new_builds_only/inputs/switch_inputs_version.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       78 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/new_builds_only/inputs/timepoints.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       95 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/new_builds_only/inputs/timeseries.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       96 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/new_builds_only/inputs/variable_capacity_factors.csv
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.706562 switch_model-2.0.7/examples/new_builds_only/outputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       19 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/new_builds_only/outputs/total_cost.txt
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.706692 switch_model-2.0.7/examples/planning_reserves/
--rw-r--r--   0 matthias   (501) wheel        (0)      307 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/planning_reserves/README.md
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.714302 switch_model-2.0.7/examples/planning_reserves/inputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/planning_reserves/inputs/financials.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      487 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/planning_reserves/inputs/fuel_cost.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      514 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/planning_reserves/inputs/fuel_supply_curves.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      191 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/planning_reserves/inputs/fuels.csv
--rw-r--r--   0 matthias   (501) wheel        (0)     2552 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/planning_reserves/inputs/gen_build_costs.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      233 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/planning_reserves/inputs/gen_build_predetermined.csv
--rw-r--r--   0 matthias   (501) wheel        (0)     4024 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/planning_reserves/inputs/gen_info.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      124 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/planning_reserves/inputs/load_zones.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      303 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/planning_reserves/inputs/loads.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      511 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/planning_reserves/inputs/modules.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       54 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/planning_reserves/inputs/non_fuel_energy_sources.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       72 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/planning_reserves/inputs/periods.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      160 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/planning_reserves/inputs/planning_reserve_requirement_zones.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      160 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/planning_reserves/inputs/planning_reserve_requirements.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      112 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/planning_reserves/inputs/regional_fuel_markets.csv
--rw-r--r--   0 matthias   (501) wheel        (0)     2741 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/planning_reserves/inputs/reserve_capacity_value.csv
--rw-r--r--   0 matthias   (501) wheel        (0)        6 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/planning_reserves/inputs/switch_inputs_version.txt
--rw-r--r--   0 matthias   (501) wheel        (0)      218 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/planning_reserves/inputs/timepoints.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      158 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/planning_reserves/inputs/timeseries.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      148 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/planning_reserves/inputs/transmission_lines.csv
--rw-r--r--   0 matthias   (501) wheel        (0)     2365 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/planning_reserves/inputs/variable_capacity_factors.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       77 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/planning_reserves/inputs/zone_balancing_areas.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      138 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/planning_reserves/inputs/zone_coincident_peak_demand.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      299 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/planning_reserves/inputs/zone_fuel_cost_diff.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      160 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/planning_reserves/inputs/zone_to_regional_fuel_market.csv
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.714676 switch_model-2.0.7/examples/planning_reserves/outputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       19 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/planning_reserves/outputs/total_cost.txt
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.714857 switch_model-2.0.7/examples/production_cost_models/
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.715198 switch_model-2.0.7/examples/production_cost_models/1plant/
--rw-r--r--   0 matthias   (501) wheel        (0)      211 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/1plant/README.md
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.717481 switch_model-2.0.7/examples/production_cost_models/1plant/inputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/1plant/inputs/financials.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       56 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/1plant/inputs/fuel_cost.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/1plant/inputs/fuels.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       90 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/1plant/inputs/gen_build_costs.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       69 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/1plant/inputs/gen_build_predetermined.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      338 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/1plant/inputs/gen_info.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       72 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/1plant/inputs/load_zones.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       45 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/1plant/inputs/loads.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      382 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/1plant/inputs/modules.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       57 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/1plant/inputs/periods.csv
--rw-r--r--   0 matthias   (501) wheel        (0)        6 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/1plant/inputs/switch_inputs_version.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       56 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/1plant/inputs/timepoints.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       96 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/1plant/inputs/timeseries.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       68 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/1plant/inputs/zone_coincident_peak_demand.csv
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.717617 switch_model-2.0.7/examples/production_cost_models/1plant/outputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       19 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/1plant/outputs/total_cost.txt
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.717746 switch_model-2.0.7/examples/production_cost_models/3plants/
--rw-r--r--   0 matthias   (501) wheel        (0)      211 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/3plants/README.md
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.720256 switch_model-2.0.7/examples/production_cost_models/3plants/inputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/3plants/inputs/financials.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       56 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/3plants/inputs/fuel_cost.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/3plants/inputs/fuels.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      174 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/3plants/inputs/gen_build_costs.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      119 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/3plants/inputs/gen_build_predetermined.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      532 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/3plants/inputs/gen_info.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       72 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/3plants/inputs/load_zones.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       45 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/3plants/inputs/loads.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      382 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/3plants/inputs/modules.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       25 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/3plants/inputs/non_fuel_energy_sources.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       57 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/3plants/inputs/periods.csv
--rw-r--r--   0 matthias   (501) wheel        (0)        6 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/3plants/inputs/switch_inputs_version.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       56 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/3plants/inputs/timepoints.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       96 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/3plants/inputs/timeseries.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       68 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/3plants/inputs/zone_coincident_peak_demand.csv
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.720412 switch_model-2.0.7/examples/production_cost_models/3plants/outputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       18 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/3plants/outputs/total_cost.txt
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.720553 switch_model-2.0.7/examples/production_cost_models/4plants/
--rw-r--r--   0 matthias   (501) wheel        (0)      243 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/4plants/README.md
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.723506 switch_model-2.0.7/examples/production_cost_models/4plants/inputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/4plants/inputs/financials.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       56 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/4plants/inputs/fuel_cost.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/4plants/inputs/fuels.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      210 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/4plants/inputs/gen_build_costs.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      161 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/4plants/inputs/gen_build_predetermined.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      611 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/4plants/inputs/gen_info.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       72 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/4plants/inputs/load_zones.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       76 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/4plants/inputs/loads.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      382 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/4plants/inputs/modules.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       31 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/4plants/inputs/non_fuel_energy_sources.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       57 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/4plants/inputs/periods.csv
--rw-r--r--   0 matthias   (501) wheel        (0)        6 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/4plants/inputs/switch_inputs_version.txt
--rw-r--r--   0 matthias   (501) wheel        (0)      122 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/4plants/inputs/timepoints.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       95 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/4plants/inputs/timeseries.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      138 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/4plants/inputs/variable_capacity_factors.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       68 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/4plants/inputs/zone_coincident_peak_demand.csv
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.723704 switch_model-2.0.7/examples/production_cost_models/4plants/outputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       19 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/4plants/outputs/total_cost.txt
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.723925 switch_model-2.0.7/examples/production_cost_models/4plants_with_unserved_load/
--rw-r--r--   0 matthias   (501) wheel        (0)      395 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/4plants_with_unserved_load/README.md
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.730831 switch_model-2.0.7/examples/production_cost_models/4plants_with_unserved_load/inputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/4plants_with_unserved_load/inputs/financials.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       56 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/4plants_with_unserved_load/inputs/fuel_cost.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/4plants_with_unserved_load/inputs/fuels.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      210 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/4plants_with_unserved_load/inputs/gen_build_costs.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      161 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/4plants_with_unserved_load/inputs/gen_build_predetermined.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      611 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/4plants_with_unserved_load/inputs/gen_info.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       72 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/4plants_with_unserved_load/inputs/load_zones.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       76 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/4plants_with_unserved_load/inputs/loads.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       25 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/4plants_with_unserved_load/inputs/lost_load_cost.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      419 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/4plants_with_unserved_load/inputs/modules.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       31 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/4plants_with_unserved_load/inputs/non_fuel_energy_sources.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       57 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/4plants_with_unserved_load/inputs/periods.csv
--rw-r--r--   0 matthias   (501) wheel        (0)        6 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/4plants_with_unserved_load/inputs/switch_inputs_version.txt
--rw-r--r--   0 matthias   (501) wheel        (0)      122 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/4plants_with_unserved_load/inputs/timepoints.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       95 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/4plants_with_unserved_load/inputs/timeseries.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      138 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/4plants_with_unserved_load/inputs/variable_capacity_factors.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       68 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/4plants_with_unserved_load/inputs/zone_coincident_peak_demand.csv
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.730967 switch_model-2.0.7/examples/production_cost_models/4plants_with_unserved_load/outputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       17 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/4plants_with_unserved_load/outputs/total_cost.txt
--rw-r--r--   0 matthias   (501) wheel        (0)      393 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/README
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.731093 switch_model-2.0.7/examples/production_cost_models/discrete_unit_commit/
--rw-r--r--   0 matthias   (501) wheel        (0)      243 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/discrete_unit_commit/README.md
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.737357 switch_model-2.0.7/examples/production_cost_models/discrete_unit_commit/inputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/discrete_unit_commit/inputs/financials.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       56 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/discrete_unit_commit/inputs/fuel_cost.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/discrete_unit_commit/inputs/fuels.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      210 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/discrete_unit_commit/inputs/gen_build_costs.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      161 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/discrete_unit_commit/inputs/gen_build_predetermined.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      733 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/discrete_unit_commit/inputs/gen_info.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       72 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/discrete_unit_commit/inputs/load_zones.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       76 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/discrete_unit_commit/inputs/loads.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      477 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/discrete_unit_commit/inputs/modules.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       31 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/discrete_unit_commit/inputs/non_fuel_energy_sources.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       57 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/discrete_unit_commit/inputs/periods.csv
--rw-r--r--   0 matthias   (501) wheel        (0)        6 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/discrete_unit_commit/inputs/switch_inputs_version.txt
--rw-r--r--   0 matthias   (501) wheel        (0)      122 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/discrete_unit_commit/inputs/timepoints.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       95 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/discrete_unit_commit/inputs/timeseries.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      138 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/discrete_unit_commit/inputs/variable_capacity_factors.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       68 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/discrete_unit_commit/inputs/zone_coincident_peak_demand.csv
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.737480 switch_model-2.0.7/examples/production_cost_models/discrete_unit_commit/outputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       18 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/discrete_unit_commit/outputs/total_cost.txt
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.738014 switch_model-2.0.7/examples/production_cost_models/spinning_reserves/
--rw-r--r--   0 matthias   (501) wheel        (0)      118 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/spinning_reserves/README.md
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.748801 switch_model-2.0.7/examples/production_cost_models/spinning_reserves/inputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/spinning_reserves/inputs/financials.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       56 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/spinning_reserves/inputs/fuel_cost.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/spinning_reserves/inputs/fuels.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      210 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/spinning_reserves/inputs/gen_build_costs.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      151 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/spinning_reserves/inputs/gen_build_predetermined.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      206 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/spinning_reserves/inputs/gen_inc_heat_rates.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      801 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/spinning_reserves/inputs/gen_info.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       72 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/spinning_reserves/inputs/load_zones.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       76 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/spinning_reserves/inputs/loads.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      569 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/spinning_reserves/inputs/modules.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       31 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/spinning_reserves/inputs/non_fuel_energy_sources.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       57 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/spinning_reserves/inputs/periods.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       28 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/spinning_reserves/inputs/spinning_reserve_params.csv
--rw-r--r--   0 matthias   (501) wheel        (0)        6 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/spinning_reserves/inputs/switch_inputs_version.txt
--rw-r--r--   0 matthias   (501) wheel        (0)      122 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/spinning_reserves/inputs/timepoints.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       95 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/spinning_reserves/inputs/timeseries.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      138 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/spinning_reserves/inputs/variable_capacity_factors.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       68 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/spinning_reserves/inputs/zone_coincident_peak_demand.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       51 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/spinning_reserves/options.txt
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.749485 switch_model-2.0.7/examples/production_cost_models/spinning_reserves/outputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       18 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/spinning_reserves/outputs/total_cost.txt
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.750000 switch_model-2.0.7/examples/production_cost_models/spinning_reserves_advanced/
--rw-r--r--   0 matthias   (501) wheel        (0)      118 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/spinning_reserves_advanced/README.md
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.754957 switch_model-2.0.7/examples/production_cost_models/spinning_reserves_advanced/inputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/spinning_reserves_advanced/inputs/financials.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       56 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/spinning_reserves_advanced/inputs/fuel_cost.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/spinning_reserves_advanced/inputs/fuels.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      210 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/spinning_reserves_advanced/inputs/gen_build_costs.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      151 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/spinning_reserves_advanced/inputs/gen_build_predetermined.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      206 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/spinning_reserves_advanced/inputs/gen_inc_heat_rates.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      801 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/spinning_reserves_advanced/inputs/gen_info.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       76 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/spinning_reserves_advanced/inputs/generation_projects_reserve_capability.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       72 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/spinning_reserves_advanced/inputs/load_zones.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       76 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/spinning_reserves_advanced/inputs/loads.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      578 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/spinning_reserves_advanced/inputs/modules.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       31 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/spinning_reserves_advanced/inputs/non_fuel_energy_sources.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       57 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/spinning_reserves_advanced/inputs/periods.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       28 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/spinning_reserves_advanced/inputs/spinning_reserve_params.csv
--rw-r--r--   0 matthias   (501) wheel        (0)        6 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/spinning_reserves_advanced/inputs/switch_inputs_version.txt
--rw-r--r--   0 matthias   (501) wheel        (0)      122 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/spinning_reserves_advanced/inputs/timepoints.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       95 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/spinning_reserves_advanced/inputs/timeseries.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      138 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/spinning_reserves_advanced/inputs/variable_capacity_factors.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       68 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/spinning_reserves_advanced/inputs/zone_coincident_peak_demand.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       51 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/spinning_reserves_advanced/options.txt
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.755113 switch_model-2.0.7/examples/production_cost_models/spinning_reserves_advanced/outputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       18 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/spinning_reserves_advanced/outputs/total_cost.txt
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.755238 switch_model-2.0.7/examples/production_cost_models/unit_commit/
--rw-r--r--   0 matthias   (501) wheel        (0)     1229 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/unit_commit/README.md
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.761695 switch_model-2.0.7/examples/production_cost_models/unit_commit/inputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/unit_commit/inputs/financials.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       56 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/unit_commit/inputs/fuel_cost.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/unit_commit/inputs/fuels.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      210 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/unit_commit/inputs/gen_build_costs.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      161 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/unit_commit/inputs/gen_build_predetermined.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      206 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/unit_commit/inputs/gen_inc_heat_rates.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      201 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/unit_commit/inputs/gen_inc_heat_rates_30p_commit.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      215 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/unit_commit/inputs/gen_inc_heat_rates_test_high_end_avoidance.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      761 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/unit_commit/inputs/gen_info.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       72 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/unit_commit/inputs/load_zones.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       76 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/unit_commit/inputs/loads.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      432 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/unit_commit/inputs/modules.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       31 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/unit_commit/inputs/non_fuel_energy_sources.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       57 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/unit_commit/inputs/periods.csv
--rw-r--r--   0 matthias   (501) wheel        (0)        6 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/unit_commit/inputs/switch_inputs_version.txt
--rw-r--r--   0 matthias   (501) wheel        (0)      122 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/unit_commit/inputs/timepoints.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       95 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/unit_commit/inputs/timeseries.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      138 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/unit_commit/inputs/variable_capacity_factors.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       68 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/unit_commit/inputs/zone_coincident_peak_demand.csv
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.762614 switch_model-2.0.7/examples/production_cost_models/unit_commit/outputs/
--rw-r--r--   0 matthias   (501) wheel        (0)      216 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/unit_commit/outputs/dispatch.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       18 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/production_cost_models/unit_commit/outputs/total_cost.txt
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.762751 switch_model-2.0.7/examples/rps_simple/
--rw-r--r--   0 matthias   (501) wheel        (0)      598 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/rps_simple/README.md
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.768818 switch_model-2.0.7/examples/rps_simple/inputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/rps_simple/inputs/financials.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      487 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/rps_simple/inputs/fuel_cost.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      514 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/rps_simple/inputs/fuel_supply_curves.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      218 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/rps_simple/inputs/fuels.csv
--rw-r--r--   0 matthias   (501) wheel        (0)     2704 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/rps_simple/inputs/gen_build_costs.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      233 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/rps_simple/inputs/gen_build_predetermined.csv
--rw-r--r--   0 matthias   (501) wheel        (0)     3824 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/rps_simple/inputs/gen_info.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      124 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/rps_simple/inputs/load_zones.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      303 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/rps_simple/inputs/loads.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      503 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/rps_simple/inputs/modules.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       54 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/rps_simple/inputs/non_fuel_energy_sources.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       72 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/rps_simple/inputs/periods.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      112 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/rps_simple/inputs/regional_fuel_markets.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       37 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/rps_simple/inputs/rps_targets.csv
--rw-r--r--   0 matthias   (501) wheel        (0)        6 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/rps_simple/inputs/switch_inputs_version.txt
--rw-r--r--   0 matthias   (501) wheel        (0)      218 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/rps_simple/inputs/timepoints.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      158 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/rps_simple/inputs/timeseries.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      148 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/rps_simple/inputs/transmission_lines.csv
--rw-r--r--   0 matthias   (501) wheel        (0)     2365 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/rps_simple/inputs/variable_capacity_factors.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       77 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/rps_simple/inputs/zone_balancing_areas.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      138 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/rps_simple/inputs/zone_coincident_peak_demand.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      299 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/rps_simple/inputs/zone_fuel_cost_diff.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      160 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/rps_simple/inputs/zone_to_regional_fuel_market.csv
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.768938 switch_model-2.0.7/examples/rps_simple/outputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       19 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/rps_simple/outputs/total_cost.txt
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.769059 switch_model-2.0.7/examples/storage/
--rw-r--r--   0 matthias   (501) wheel        (0)      137 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/storage/README.md
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.773804 switch_model-2.0.7/examples/storage/inputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/storage/inputs/financials.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       56 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/storage/inputs/fuel_cost.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/storage/inputs/fuels.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      328 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/storage/inputs/gen_build_costs.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      158 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/storage/inputs/gen_build_predetermined.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      576 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/storage/inputs/gen_info.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       60 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/storage/inputs/load_zones.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       59 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/storage/inputs/loads.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      390 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/storage/inputs/modules.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       43 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/storage/inputs/non_fuel_energy_sources.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       57 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/storage/inputs/periods.csv
--rw-r--r--   0 matthias   (501) wheel        (0)        6 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/storage/inputs/switch_inputs_version.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       78 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/storage/inputs/timepoints.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       95 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/storage/inputs/timeseries.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       96 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/storage/inputs/variable_capacity_factors.csv
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.779122 switch_model-2.0.7/examples/storage/outputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       19 2022-11-02 00:23:51.000000 switch_model-2.0.7/examples/storage/outputs/total_cost.txt
--rw-r--r--   0 matthias   (501) wheel        (0)     3513 2022-11-02 00:23:51.000000 switch_model-2.0.7/how_to_collaborate.txt
--rwxr-xr-x   0 matthias   (501) wheel        (0)     2218 2022-11-02 00:23:51.000000 switch_model-2.0.7/run_tests.py
--rw-r--r--   0 matthias   (501) wheel        (0)       38 2022-11-02 00:33:46.860512 switch_model-2.0.7/setup.cfg
--rw-r--r--   0 matthias   (501) wheel        (0)     4808 2022-11-02 00:23:51.000000 switch_model-2.0.7/setup.py
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.797872 switch_model-2.0.7/switch_model/
--rw-r--r--   0 matthias   (501) wheel        (0)     1021 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/__init__.py
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.805572 switch_model-2.0.7/switch_model/balancing/
--rw-r--r--   0 matthias   (501) wheel        (0)        0 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/balancing/__init__.py
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.805803 switch_model-2.0.7/switch_model/balancing/demand_response/
--rw-r--r--   0 matthias   (501) wheel        (0)        0 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/balancing/demand_response/__init__.py
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.806298 switch_model-2.0.7/switch_model/balancing/demand_response/iterative/
--rw-r--r--   0 matthias   (501) wheel        (0)    61086 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/balancing/demand_response/iterative/__init__.py
--rw-r--r--   0 matthias   (501) wheel        (0)     3375 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/balancing/demand_response/iterative/constant_elasticity_demand_system.py
--rw-r--r--   0 matthias   (501) wheel        (0)     6468 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/balancing/demand_response/iterative/r_demand_system.py
--rw-r--r--   0 matthias   (501) wheel        (0)     3379 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/balancing/demand_response/simple.py
--rwxr-xr-x   0 matthias   (501) wheel        (0)    10218 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/balancing/diagnose_infeasibility.py
--rw-r--r--   0 matthias   (501) wheel        (0)     8389 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/balancing/load_zones.py
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.806865 switch_model-2.0.7/switch_model/balancing/operating_reserves/
--rw-r--r--   0 matthias   (501) wheel        (0)        0 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/balancing/operating_reserves/__init__.py
--rw-r--r--   0 matthias   (501) wheel        (0)     2268 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/balancing/operating_reserves/areas.py
--rw-r--r--   0 matthias   (501) wheel        (0)    26259 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/balancing/operating_reserves/spinning_reserves.py
--rw-r--r--   0 matthias   (501) wheel        (0)    30430 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/balancing/operating_reserves/spinning_reserves_advanced.py
--rw-r--r--   0 matthias   (501) wheel        (0)    13586 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/balancing/planning_reserves.py
--rw-r--r--   0 matthias   (501) wheel        (0)     2283 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/balancing/unserved_load.py
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.807213 switch_model-2.0.7/switch_model/energy_sources/
--rw-r--r--   0 matthias   (501) wheel        (0)        0 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/energy_sources/__init__.py
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.808090 switch_model-2.0.7/switch_model/energy_sources/fuel_costs/
--rw-r--r--   0 matthias   (501) wheel        (0)        0 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/energy_sources/fuel_costs/__init__.py
--rw-r--r--   0 matthias   (501) wheel        (0)    24354 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/energy_sources/fuel_costs/markets.py
--rw-r--r--   0 matthias   (501) wheel        (0)     8284 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/energy_sources/fuel_costs/markets_expansion.py
--rw-r--r--   0 matthias   (501) wheel        (0)     3589 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/energy_sources/fuel_costs/simple.py
--rw-r--r--   0 matthias   (501) wheel        (0)     4063 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/energy_sources/fuel_costs/simple_per_timepoint.py
--rw-r--r--   0 matthias   (501) wheel        (0)     7046 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/energy_sources/properties.py
--rw-r--r--   0 matthias   (501) wheel        (0)    16938 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/financials.py
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.808243 switch_model-2.0.7/switch_model/generators/
--rw-r--r--   0 matthias   (501) wheel        (0)        0 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/generators/__init__.py
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.809270 switch_model-2.0.7/switch_model/generators/core/
--rw-r--r--   0 matthias   (501) wheel        (0)      377 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/generators/core/__init__.py
--rw-r--r--   0 matthias   (501) wheel        (0)    30411 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/generators/core/build.py
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.809765 switch_model-2.0.7/switch_model/generators/core/commit/
--rw-r--r--   0 matthias   (501) wheel        (0)      464 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/generators/core/commit/__init__.py
--rw-r--r--   0 matthias   (501) wheel        (0)     2743 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/generators/core/commit/discrete.py
--rw-r--r--   0 matthias   (501) wheel        (0)    16618 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/generators/core/commit/fuel_use.py
--rw-r--r--   0 matthias   (501) wheel        (0)    19914 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/generators/core/commit/operate.py
--rw-r--r--   0 matthias   (501) wheel        (0)    24296 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/generators/core/dispatch.py
--rw-r--r--   0 matthias   (501) wheel        (0)     1702 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/generators/core/gen_discrete_build.py
--rw-r--r--   0 matthias   (501) wheel        (0)     5444 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/generators/core/no_commit.py
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.810247 switch_model-2.0.7/switch_model/generators/extensions/
--rw-r--r--   0 matthias   (501) wheel        (0)        0 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/generators/extensions/__init__.py
--rw-r--r--   0 matthias   (501) wheel        (0)     8082 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/generators/extensions/hydro_simple.py
--rw-r--r--   0 matthias   (501) wheel        (0)    22766 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/generators/extensions/hydro_system.py
--rw-r--r--   0 matthias   (501) wheel        (0)    14496 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/generators/extensions/storage.py
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.816734 switch_model-2.0.7/switch_model/hawaii/
--rw-r--r--   0 matthias   (501) wheel        (0)        0 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/hawaii/__init__.py
--rw-r--r--   0 matthias   (501) wheel        (0)     6046 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/hawaii/batteries.py
--rw-r--r--   0 matthias   (501) wheel        (0)     6719 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/hawaii/batteries_fixed_calendar_life.py
--rw-r--r--   0 matthias   (501) wheel        (0)    38086 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/hawaii/demand_response_no_reserves.py
--rw-r--r--   0 matthias   (501) wheel        (0)     3321 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/hawaii/demand_response_simple.py
--rw-r--r--   0 matthias   (501) wheel        (0)      875 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/hawaii/emission_rules.py
--rw-r--r--   0 matthias   (501) wheel        (0)    10340 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/hawaii/ev.py
--rw-r--r--   0 matthias   (501) wheel        (0)    11116 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/hawaii/ev_advanced.py
--rw-r--r--   0 matthias   (501) wheel        (0)     3706 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/hawaii/fed_subsidies.py
--rw-r--r--   0 matthias   (501) wheel        (0)     5500 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/hawaii/fuel_markets_expansion.py
--rw-r--r--   0 matthias   (501) wheel        (0)    37100 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/hawaii/heco_outlook_2019.py
--rw-r--r--   0 matthias   (501) wheel        (0)    48333 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/hawaii/heco_outlook_2020_06.py
--rw-r--r--   0 matthias   (501) wheel        (0)    47629 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/hawaii/heco_outlook_2020_08.py
--rw-r--r--   0 matthias   (501) wheel        (0)    37342 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/hawaii/heco_plan_2020_06.py
--rw-r--r--   0 matthias   (501) wheel        (0)    36778 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/hawaii/heco_plan_2020_08.py
--rw-r--r--   0 matthias   (501) wheel        (0)     3658 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/hawaii/hi_spinning_reserves.py
--rw-r--r--   0 matthias   (501) wheel        (0)    17417 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/hawaii/hydrogen.py
--rw-r--r--   0 matthias   (501) wheel        (0)     1229 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/hawaii/lake_wilson.py
--rw-r--r--   0 matthias   (501) wheel        (0)    13491 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/hawaii/lng_conversion.py
--rw-r--r--   0 matthias   (501) wheel        (0)      560 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/hawaii/no_central_pv.py
--rw-r--r--   0 matthias   (501) wheel        (0)      391 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/hawaii/no_onshore_wind.py
--rw-r--r--   0 matthias   (501) wheel        (0)      753 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/hawaii/no_renewables.py
--rw-r--r--   0 matthias   (501) wheel        (0)      600 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/hawaii/no_wind.py
--rw-r--r--   0 matthias   (501) wheel        (0)     8195 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/hawaii/oahu_plants.py
--rw-r--r--   0 matthias   (501) wheel        (0)    14284 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/hawaii/psip_2016_04.py
--rw-r--r--   0 matthias   (501) wheel        (0)    28641 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/hawaii/psip_2016_12.py
--rw-r--r--   0 matthias   (501) wheel        (0)     7297 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/hawaii/pumped_hydro.py
--rw-r--r--   0 matthias   (501) wheel        (0)     7807 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/hawaii/register_hi_storage_reserves.py
--rw-r--r--   0 matthias   (501) wheel        (0)    13305 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/hawaii/reserves.py
--rw-r--r--   0 matthias   (501) wheel        (0)    38383 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/hawaii/rps.py
--rw-r--r--   0 matthias   (501) wheel        (0)    31350 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/hawaii/save_results.py
--rw-r--r--   0 matthias   (501) wheel        (0)    59373 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/hawaii/scenario_data.py
--rw-r--r--   0 matthias   (501) wheel        (0)     7349 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/hawaii/scenarios.py
--rw-r--r--   0 matthias   (501) wheel        (0)    12397 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/hawaii/smooth_dispatch.py
--rw-r--r--   0 matthias   (501) wheel        (0)     8836 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/hawaii/smooth_dispatch_quadratic.py
--rw-r--r--   0 matthias   (501) wheel        (0)     2413 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/hawaii/switch_patch.py
--rw-r--r--   0 matthias   (501) wheel        (0)     2644 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/hawaii/unserved_load.py
--rw-r--r--   0 matthias   (501) wheel        (0)     3036 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/hawaii/util.py
--rw-r--r--   0 matthias   (501) wheel        (0)     1936 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/main.py
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.817179 switch_model-2.0.7/switch_model/policies/
--rw-r--r--   0 matthias   (501) wheel        (0)        0 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/policies/__init__.py
--rw-r--r--   0 matthias   (501) wheel        (0)     5314 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/policies/carbon_policies.py
--rw-r--r--   0 matthias   (501) wheel        (0)     6182 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/policies/rps_simple.py
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.817815 switch_model-2.0.7/switch_model/reporting/
--rw-r--r--   0 matthias   (501) wheel        (0)    10323 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/reporting/__init__.py
--rw-r--r--   0 matthias   (501) wheel        (0)    30291 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/reporting/basic_exports.py
--rw-r--r--   0 matthias   (501) wheel        (0)     1675 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/reporting/dump.py
--rw-r--r--   0 matthias   (501) wheel        (0)     1195 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/reporting/example_export.py
--rwxr-xr-x   0 matthias   (501) wheel        (0)    53689 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/solve.py
--rwxr-xr-x   0 matthias   (501) wheel        (0)    17718 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/solve_scenarios.py
--rw-r--r--   0 matthias   (501) wheel        (0)      366 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/test.py
--rw-r--r--   0 matthias   (501) wheel        (0)    18977 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/timescales.py
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.818365 switch_model-2.0.7/switch_model/transmission/
--rw-r--r--   0 matthias   (501) wheel        (0)        0 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/transmission/__init__.py
--rw-r--r--   0 matthias   (501) wheel        (0)      438 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/transmission/copperplate.py
--rw-r--r--   0 matthias   (501) wheel        (0)    12576 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/transmission/local_td.py
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.818753 switch_model-2.0.7/switch_model/transmission/transport/
--rw-r--r--   0 matthias   (501) wheel        (0)      405 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/transmission/transport/__init__.py
--rw-r--r--   0 matthias   (501) wheel        (0)    15859 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/transmission/transport/build.py
--rw-r--r--   0 matthias   (501) wheel        (0)     3463 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/transmission/transport/dispatch.py
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.820396 switch_model-2.0.7/switch_model/upgrade/
--rw-r--r--   0 matthias   (501) wheel        (0)      956 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/upgrade/__init__.py
--rw-r--r--   0 matthias   (501) wheel        (0)     8087 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/upgrade/manager.py
--rw-r--r--   0 matthias   (501) wheel        (0)      569 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/upgrade/re_upgrade.py
--rw-r--r--   0 matthias   (501) wheel        (0)    20441 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/upgrade/upgrade_2_0_0b1.py
--rw-r--r--   0 matthias   (501) wheel        (0)     2085 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/upgrade/upgrade_2_0_0b2.py
--rw-r--r--   0 matthias   (501) wheel        (0)     2444 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/upgrade/upgrade_2_0_0b4.py
--rw-r--r--   0 matthias   (501) wheel        (0)     6121 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/upgrade/upgrade_2_0_1.py
--rw-r--r--   0 matthias   (501) wheel        (0)     4767 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/upgrade/upgrade_2_0_4.py
--rw-r--r--   0 matthias   (501) wheel        (0)     6304 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/upgrade/upgrade_2_0_5.py
--rw-r--r--   0 matthias   (501) wheel        (0)     5947 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/upgrade/upgrade_2_0_6.py
--rw-r--r--   0 matthias   (501) wheel        (0)     6943 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/upgrade/upgrade_2_0_7.py
--rw-r--r--   0 matthias   (501) wheel        (0)    44669 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/utilities.py
--rw-r--r--   0 matthias   (501) wheel        (0)      349 2022-11-02 00:23:51.000000 switch_model-2.0.7/switch_model/version.py
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.804854 switch_model-2.0.7/switch_model.egg-info/
--rw-r--r--   0 matthias   (501) wheel        (0)     5512 2022-11-02 00:33:46.000000 switch_model-2.0.7/switch_model.egg-info/PKG-INFO
--rw-r--r--   0 matthias   (501) wheel        (0)    49340 2022-11-02 00:33:46.000000 switch_model-2.0.7/switch_model.egg-info/SOURCES.txt
--rw-r--r--   0 matthias   (501) wheel        (0)        1 2022-11-02 00:33:46.000000 switch_model-2.0.7/switch_model.egg-info/dependency_links.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       50 2022-11-02 00:33:46.000000 switch_model-2.0.7/switch_model.egg-info/entry_points.txt
--rw-r--r--   0 matthias   (501) wheel        (0)      191 2022-11-02 00:33:46.000000 switch_model-2.0.7/switch_model.egg-info/requires.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       13 2022-11-02 00:33:46.000000 switch_model-2.0.7/switch_model.egg-info/top_level.txt
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.820912 switch_model-2.0.7/tests/
--rw-r--r--   0 matthias   (501) wheel        (0)      136 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/__init__.py
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.823816 switch_model-2.0.7/tests/__pycache__/
--rw-r--r--   0 matthias   (501) wheel        (0)      136 2022-11-02 00:28:55.000000 switch_model-2.0.7/tests/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 matthias   (501) wheel        (0)      130 2022-11-02 00:24:39.000000 switch_model-2.0.7/tests/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 matthias   (501) wheel        (0)     3020 2022-11-02 00:28:55.000000 switch_model-2.0.7/tests/__pycache__/examples_test.cpython-310.pyc
--rw-r--r--   0 matthias   (501) wheel        (0)     2907 2022-11-02 00:24:39.000000 switch_model-2.0.7/tests/__pycache__/examples_test.cpython-37.pyc
--rw-r--r--   0 matthias   (501) wheel        (0)     3328 2022-11-02 00:28:55.000000 switch_model-2.0.7/tests/__pycache__/upgrade_test.cpython-310.pyc
--rw-r--r--   0 matthias   (501) wheel        (0)     3248 2022-11-02 00:24:39.000000 switch_model-2.0.7/tests/__pycache__/upgrade_test.cpython-37.pyc
--rw-r--r--   0 matthias   (501) wheel        (0)     3957 2022-11-02 00:28:55.000000 switch_model-2.0.7/tests/__pycache__/utilities_test.cpython-310.pyc
--rw-r--r--   0 matthias   (501) wheel        (0)     3835 2022-11-02 00:24:39.000000 switch_model-2.0.7/tests/__pycache__/utilities_test.cpython-37.pyc
--rw-r--r--   0 matthias   (501) wheel        (0)     3429 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/examples_test.py
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.824031 switch_model-2.0.7/tests/upgrade_dat/
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.625031 switch_model-2.0.7/tests/upgrade_dat/3zone_toy/
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.827369 switch_model-2.0.7/tests/upgrade_dat/3zone_toy/inputs/
--rw-r--r--   0 matthias   (501) wheel        (0)      240 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy/inputs/balancing_areas.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       91 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy/inputs/financials.dat
--rw-r--r--   0 matthias   (501) wheel        (0)      487 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy/inputs/fuel_cost.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      492 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy/inputs/fuel_supply_curves.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      168 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy/inputs/fuels.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      713 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy/inputs/gen_new_build_costs.tab
--rw-r--r--   0 matthias   (501) wheel        (0)     1266 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy/inputs/generator_info.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      152 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy/inputs/load_zones.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      277 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy/inputs/loads.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       76 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy/inputs/lz_balancing_areas.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      297 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy/inputs/lz_fuel_cost_diff.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      115 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy/inputs/lz_peak_loads.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      159 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy/inputs/lz_to_regional_fuel_market.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       67 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy/inputs/modules.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       53 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy/inputs/non_fuel_energy_sources.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       72 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy/inputs/periods.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      358 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy/inputs/proj_build_costs.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      215 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy/inputs/proj_existing_builds.tab
--rw-r--r--   0 matthias   (501) wheel        (0)     1765 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy/inputs/project_info.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      111 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy/inputs/regional_fuel_markets.tab
--rw-r--r--   0 matthias   (501) wheel        (0)        8 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy/inputs/switch_inputs_version.txt
--rw-r--r--   0 matthias   (501) wheel        (0)      217 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy/inputs/timepoints.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      157 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy/inputs/timeseries.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      147 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy/inputs/transmission_lines.tab
--rw-r--r--   0 matthias   (501) wheel        (0)     2402 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy/inputs/variable_capacity_factors.tab
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.827499 switch_model-2.0.7/tests/upgrade_dat/3zone_toy/outputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       14 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy/outputs/total_cost.txt
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.625218 switch_model-2.0.7/tests/upgrade_dat/3zone_toy_2_0_6/
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.830933 switch_model-2.0.7/tests/upgrade_dat/3zone_toy_2_0_6/inputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy_2_0_6/inputs/financials.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      487 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy_2_0_6/inputs/fuel_cost.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      514 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy_2_0_6/inputs/fuel_supply_curves.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      179 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy_2_0_6/inputs/fuels.csv
--rw-r--r--   0 matthias   (501) wheel        (0)     2704 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy_2_0_6/inputs/gen_build_costs.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      231 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy_2_0_6/inputs/gen_build_predetermined.csv
--rw-r--r--   0 matthias   (501) wheel        (0)     3812 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy_2_0_6/inputs/generation_projects_info.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      124 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy_2_0_6/inputs/load_zones.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      303 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy_2_0_6/inputs/loads.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      470 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy_2_0_6/inputs/modules.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       54 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy_2_0_6/inputs/non_fuel_energy_sources.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       72 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy_2_0_6/inputs/periods.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      112 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy_2_0_6/inputs/regional_fuel_markets.csv
--rw-r--r--   0 matthias   (501) wheel        (0)        6 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy_2_0_6/inputs/switch_inputs_version.txt
--rw-r--r--   0 matthias   (501) wheel        (0)      218 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy_2_0_6/inputs/timepoints.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      158 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy_2_0_6/inputs/timeseries.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      116 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy_2_0_6/inputs/trans_params.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      148 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy_2_0_6/inputs/transmission_lines.csv
--rw-r--r--   0 matthias   (501) wheel        (0)     2365 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy_2_0_6/inputs/variable_capacity_factors.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       77 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy_2_0_6/inputs/zone_balancing_areas.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      138 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy_2_0_6/inputs/zone_coincident_peak_demand.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      299 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy_2_0_6/inputs/zone_fuel_cost_diff.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      160 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy_2_0_6/inputs/zone_to_regional_fuel_market.csv
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.831067 switch_model-2.0.7/tests/upgrade_dat/3zone_toy_2_0_6/outputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       19 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/3zone_toy_2_0_6/outputs/total_cost.txt
--rw-r--r--   0 matthias   (501) wheel        (0)      678 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/README.txt
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.625393 switch_model-2.0.7/tests/upgrade_dat/copperplate0/
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.833462 switch_model-2.0.7/tests/upgrade_dat/copperplate0/inputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       91 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/copperplate0/inputs/financials.dat
--rw-r--r--   0 matthias   (501) wheel        (0)       55 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/copperplate0/inputs/fuel_cost.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/copperplate0/inputs/fuels.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      151 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/copperplate0/inputs/gen_new_build_costs.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      391 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/copperplate0/inputs/generator_info.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       59 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/copperplate0/inputs/load_zones.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       55 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/copperplate0/inputs/loads.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       28 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/copperplate0/inputs/modules.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       31 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/copperplate0/inputs/non_fuel_energy_sources.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       57 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/copperplate0/inputs/periods.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      143 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/copperplate0/inputs/proj_build_costs.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       94 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/copperplate0/inputs/proj_existing_builds.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      247 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/copperplate0/inputs/project_info.tab
--rw-r--r--   0 matthias   (501) wheel        (0)        8 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/copperplate0/inputs/switch_inputs_version.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       78 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/copperplate0/inputs/timepoints.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       95 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/copperplate0/inputs/timeseries.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       84 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/copperplate0/inputs/variable_capacity_factors.tab
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.833595 switch_model-2.0.7/tests/upgrade_dat/copperplate0/outputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       14 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/copperplate0/outputs/total_cost.txt
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.625578 switch_model-2.0.7/tests/upgrade_dat/copperplate1/
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.836099 switch_model-2.0.7/tests/upgrade_dat/copperplate1/inputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       91 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/copperplate1/inputs/financials.dat
--rw-r--r--   0 matthias   (501) wheel        (0)      181 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/copperplate1/inputs/fuel_supply_curves.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       88 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/copperplate1/inputs/fuels.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      275 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/copperplate1/inputs/gen_new_build_costs.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      599 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/copperplate1/inputs/generator_info.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       73 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/copperplate1/inputs/load_zones.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       55 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/copperplate1/inputs/loads.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       59 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/copperplate1/inputs/lz_to_regional_fuel_market.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       40 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/copperplate1/inputs/modules.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       31 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/copperplate1/inputs/non_fuel_energy_sources.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       57 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/copperplate1/inputs/periods.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      162 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/copperplate1/inputs/proj_build_costs.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      101 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/copperplate1/inputs/proj_existing_builds.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      433 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/copperplate1/inputs/project_info.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       62 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/copperplate1/inputs/regional_fuel_markets.tab
--rw-r--r--   0 matthias   (501) wheel        (0)        8 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/copperplate1/inputs/switch_inputs_version.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       78 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/copperplate1/inputs/timepoints.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       95 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/copperplate1/inputs/timeseries.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      217 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/copperplate1/inputs/variable_capacity_factors.tab
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.836230 switch_model-2.0.7/tests/upgrade_dat/copperplate1/outputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       14 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/copperplate1/outputs/total_cost.txt
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.836354 switch_model-2.0.7/tests/upgrade_dat/custom_extension/
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.840908 switch_model-2.0.7/tests/upgrade_dat/custom_extension/inputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       91 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/custom_extension/inputs/financials.dat
--rw-r--r--   0 matthias   (501) wheel        (0)       55 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/custom_extension/inputs/fuel_cost.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/custom_extension/inputs/fuels.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      151 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/custom_extension/inputs/gen_new_build_costs.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      391 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/custom_extension/inputs/generator_info.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       59 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/custom_extension/inputs/load_zones.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       55 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/custom_extension/inputs/loads.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       50 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/custom_extension/inputs/modules.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       31 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/custom_extension/inputs/non_fuel_energy_sources.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       57 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/custom_extension/inputs/periods.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      143 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/custom_extension/inputs/proj_build_costs.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       94 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/custom_extension/inputs/proj_existing_builds.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      215 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/custom_extension/inputs/project_info.tab
--rw-r--r--   0 matthias   (501) wheel        (0)        8 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/custom_extension/inputs/switch_inputs_version.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       78 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/custom_extension/inputs/timepoints.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       95 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/custom_extension/inputs/timeseries.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       84 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/custom_extension/inputs/variable_capacity_factors.tab
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.841067 switch_model-2.0.7/tests/upgrade_dat/custom_extension/outputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       14 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/custom_extension/outputs/total_cost.txt
--rw-r--r--   0 matthias   (501) wheel        (0)     1073 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/custom_extension/sunk_costs.py
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.625939 switch_model-2.0.7/tests/upgrade_dat/hydro_simple/
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.843499 switch_model-2.0.7/tests/upgrade_dat/hydro_simple/inputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       91 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/hydro_simple/inputs/financials.dat
--rw-r--r--   0 matthias   (501) wheel        (0)       55 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/hydro_simple/inputs/fuel_cost.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/hydro_simple/inputs/fuels.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      151 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/hydro_simple/inputs/gen_new_build_costs.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      480 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/hydro_simple/inputs/generator_info.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      110 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/hydro_simple/inputs/hydro_timeseries.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       59 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/hydro_simple/inputs/load_zones.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       76 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/hydro_simple/inputs/loads.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       52 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/hydro_simple/inputs/modules.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       37 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/hydro_simple/inputs/non_fuel_energy_sources.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       57 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/hydro_simple/inputs/periods.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      213 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/hydro_simple/inputs/proj_build_costs.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      133 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/hydro_simple/inputs/proj_existing_builds.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      308 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/hydro_simple/inputs/project_info.tab
--rw-r--r--   0 matthias   (501) wheel        (0)        8 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/hydro_simple/inputs/switch_inputs_version.txt
--rw-r--r--   0 matthias   (501) wheel        (0)      133 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/hydro_simple/inputs/timepoints.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      123 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/hydro_simple/inputs/timeseries.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      186 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/hydro_simple/inputs/variable_capacity_factors.tab
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.843616 switch_model-2.0.7/tests/upgrade_dat/hydro_simple/outputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       14 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/hydro_simple/outputs/total_cost.txt
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.626129 switch_model-2.0.7/tests/upgrade_dat/hydro_system/
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.847220 switch_model-2.0.7/tests/upgrade_dat/hydro_system/inputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       91 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/hydro_system/inputs/financials.dat
--rw-r--r--   0 matthias   (501) wheel        (0)       57 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/hydro_system/inputs/fuel_cost.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       57 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/hydro_system/inputs/fuels.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       69 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/hydro_system/inputs/gen_new_build_costs.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      396 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/hydro_system/inputs/generator_info.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      164 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/hydro_system/inputs/hydro_projects.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       61 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/hydro_system/inputs/load_zones.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      642 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/hydro_system/inputs/loads.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       52 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/hydro_system/inputs/modules.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       26 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/hydro_system/inputs/non_fuel_energy_sources.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       57 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/hydro_system/inputs/periods.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      187 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/hydro_system/inputs/proj_build_costs.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      163 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/hydro_system/inputs/proj_existing_builds.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      330 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/hydro_system/inputs/project_info.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      149 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/hydro_system/inputs/reservoirs.tab
--rw-r--r--   0 matthias   (501) wheel        (0)        8 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/hydro_system/inputs/switch_inputs_version.txt
--rw-r--r--   0 matthias   (501) wheel        (0)     1609 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/hydro_system/inputs/timepoints.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      143 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/hydro_system/inputs/timeseries.tab
--rw-r--r--   0 matthias   (501) wheel        (0)     1183 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/hydro_system/inputs/variable_capacity_factors.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      183 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/hydro_system/inputs/water_connections.tab
--rw-r--r--   0 matthias   (501) wheel        (0)     1291 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/hydro_system/inputs/water_node_tp_flows.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      137 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/hydro_system/inputs/water_nodes.tab
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.847358 switch_model-2.0.7/tests/upgrade_dat/hydro_system/outputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       14 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/hydro_system/outputs/total_cost.txt
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.626960 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.626579 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/4plants/
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.849471 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/4plants/inputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       91 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/4plants/inputs/financials.dat
--rw-r--r--   0 matthias   (501) wheel        (0)       55 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/4plants/inputs/fuel_cost.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/4plants/inputs/fuels.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      446 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/4plants/inputs/generator_info.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       72 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/4plants/inputs/load_zones.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       74 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/4plants/inputs/loads.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       46 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/4plants/inputs/lz_peak_loads.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       37 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/4plants/inputs/modules.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       30 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/4plants/inputs/non_fuel_energy_sources.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       57 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/4plants/inputs/periods.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      200 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/4plants/inputs/proj_build_costs.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      127 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/4plants/inputs/proj_existing_builds.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      248 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/4plants/inputs/project_info.tab
--rw-r--r--   0 matthias   (501) wheel        (0)        8 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/4plants/inputs/switch_inputs_version.txt
--rw-r--r--   0 matthias   (501) wheel        (0)      122 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/4plants/inputs/timepoints.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       95 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/4plants/inputs/timeseries.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      126 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/4plants/inputs/variable_capacity_factors.tab
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.849614 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/4plants/outputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       14 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/4plants/outputs/total_cost.txt
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.626880 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/discrete_unit_commit/
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.852507 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/discrete_unit_commit/inputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       91 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/discrete_unit_commit/inputs/financials.dat
--rw-r--r--   0 matthias   (501) wheel        (0)       55 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/discrete_unit_commit/inputs/fuel_cost.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/discrete_unit_commit/inputs/fuels.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      552 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/discrete_unit_commit/inputs/generator_info.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       72 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/discrete_unit_commit/inputs/load_zones.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       74 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/discrete_unit_commit/inputs/loads.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       46 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/discrete_unit_commit/inputs/lz_peak_loads.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       66 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/discrete_unit_commit/inputs/modules.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       30 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/discrete_unit_commit/inputs/non_fuel_energy_sources.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       57 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/discrete_unit_commit/inputs/periods.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      200 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/discrete_unit_commit/inputs/proj_build_costs.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      127 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/discrete_unit_commit/inputs/proj_existing_builds.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      248 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/discrete_unit_commit/inputs/project_info.tab
--rw-r--r--   0 matthias   (501) wheel        (0)        8 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/discrete_unit_commit/inputs/switch_inputs_version.txt
--rw-r--r--   0 matthias   (501) wheel        (0)      122 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/discrete_unit_commit/inputs/timepoints.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       95 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/discrete_unit_commit/inputs/timeseries.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      126 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/discrete_unit_commit/inputs/variable_capacity_factors.tab
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.852653 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/discrete_unit_commit/outputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       14 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/discrete_unit_commit/outputs/total_cost.txt
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.627081 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/unit_commit/
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.855776 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/unit_commit/inputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       91 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/unit_commit/inputs/financials.dat
--rw-r--r--   0 matthias   (501) wheel        (0)       55 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/unit_commit/inputs/fuel_cost.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/unit_commit/inputs/fuels.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      197 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/unit_commit/inputs/gen_inc_heat_rates.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      197 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/unit_commit/inputs/gen_inc_heat_rates_30p_commit.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      205 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/unit_commit/inputs/gen_inc_heat_rates_test_high_end_avoidance.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      553 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/unit_commit/inputs/generator_info.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       72 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/unit_commit/inputs/load_zones.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       74 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/unit_commit/inputs/loads.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       46 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/unit_commit/inputs/lz_peak_loads.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       38 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/unit_commit/inputs/modules.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       30 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/unit_commit/inputs/non_fuel_energy_sources.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       57 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/unit_commit/inputs/periods.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      200 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/unit_commit/inputs/proj_build_costs.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      127 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/unit_commit/inputs/proj_existing_builds.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      248 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/unit_commit/inputs/project_info.tab
--rw-r--r--   0 matthias   (501) wheel        (0)        8 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/unit_commit/inputs/switch_inputs_version.txt
--rw-r--r--   0 matthias   (501) wheel        (0)      122 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/unit_commit/inputs/timepoints.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       95 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/unit_commit/inputs/timeseries.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      126 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/unit_commit/inputs/variable_capacity_factors.tab
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.855897 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/unit_commit/outputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       14 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/production_cost_models/unit_commit/outputs/total_cost.txt
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.627272 switch_model-2.0.7/tests/upgrade_dat/storage/
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.858203 switch_model-2.0.7/tests/upgrade_dat/storage/inputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       91 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/storage/inputs/financials.dat
--rw-r--r--   0 matthias   (501) wheel        (0)       55 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/storage/inputs/fuel_cost.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/storage/inputs/fuels.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      225 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/storage/inputs/gen_new_build_costs.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      484 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/storage/inputs/generator_info.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       59 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/storage/inputs/load_zones.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       55 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/storage/inputs/loads.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       47 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/storage/inputs/modules.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       42 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/storage/inputs/non_fuel_energy_sources.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       57 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/storage/inputs/periods.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      115 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/storage/inputs/proj_build_costs.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       79 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/storage/inputs/proj_existing_builds.tab
--rw-r--r--   0 matthias   (501) wheel        (0)      254 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/storage/inputs/project_info.tab
--rw-r--r--   0 matthias   (501) wheel        (0)        8 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/storage/inputs/switch_inputs_version.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       78 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/storage/inputs/timepoints.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       95 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/storage/inputs/timeseries.tab
--rw-r--r--   0 matthias   (501) wheel        (0)       84 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/storage/inputs/variable_capacity_factors.tab
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.858322 switch_model-2.0.7/tests/upgrade_dat/storage/outputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       13 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/storage/outputs/total_cost.txt
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.627484 switch_model-2.0.7/tests/upgrade_dat/storage_206/
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.859987 switch_model-2.0.7/tests/upgrade_dat/storage_206/inputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/storage_206/inputs/financials.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       56 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/storage_206/inputs/fuel_cost.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       63 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/storage_206/inputs/fuels.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      328 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/storage_206/inputs/gen_build_costs.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      153 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/storage_206/inputs/gen_build_predetermined.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      576 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/storage_206/inputs/generation_projects_info.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       60 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/storage_206/inputs/load_zones.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       59 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/storage_206/inputs/loads.csv
--rw-r--r--   0 matthias   (501) wheel        (0)      390 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/storage_206/inputs/modules.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       43 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/storage_206/inputs/non_fuel_energy_sources.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       57 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/storage_206/inputs/periods.csv
--rw-r--r--   0 matthias   (501) wheel        (0)        6 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/storage_206/inputs/switch_inputs_version.txt
--rw-r--r--   0 matthias   (501) wheel        (0)       78 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/storage_206/inputs/timepoints.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       95 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/storage_206/inputs/timeseries.csv
--rw-r--r--   0 matthias   (501) wheel        (0)       96 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/storage_206/inputs/variable_capacity_factors.csv
-drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2022-11-02 00:33:46.860096 switch_model-2.0.7/tests/upgrade_dat/storage_206/outputs/
--rw-r--r--   0 matthias   (501) wheel        (0)       19 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_dat/storage_206/outputs/total_cost.txt
--rw-r--r--   0 matthias   (501) wheel        (0)     3951 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/upgrade_test.py
--rw-r--r--   0 matthias   (501) wheel        (0)     4600 2022-11-02 00:23:51.000000 switch_model-2.0.7/tests/utilities_test.py
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.556986 switch_model-2.0.8/
+-rw-r--r--   0 matthias   (501) wheel        (0)      789 2024-04-23 07:17:04.000000 switch_model-2.0.8/AUTHORS
+-rw-r--r--   0 matthias   (501) wheel        (0)     4174 2024-04-23 07:17:04.000000 switch_model-2.0.8/DEV_INSTALL.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)    11529 2024-04-23 07:17:04.000000 switch_model-2.0.8/LICENSE
+-rw-r--r--   0 matthias   (501) wheel        (0)      735 2024-04-23 07:17:04.000000 switch_model-2.0.8/LICENSE.BOILERPLATE
+-rw-r--r--   0 matthias   (501) wheel        (0)      216 2024-04-23 07:17:04.000000 switch_model-2.0.8/MANIFEST.in
+-rw-r--r--   0 matthias   (501) wheel        (0)     5972 2024-04-25 22:11:43.556730 switch_model-2.0.8/PKG-INFO
+-rw-r--r--   0 matthias   (501) wheel        (0)     4167 2024-04-23 07:17:04.000000 switch_model-2.0.8/README
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.367181 switch_model-2.0.8/examples/
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.373000 switch_model-2.0.8/examples/3zone_toy/
+-rw-r--r--   0 matthias   (501) wheel        (0)      309 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy/README.md
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.376941 switch_model-2.0.8/examples/3zone_toy/inputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy/inputs/financials.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      487 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy/inputs/fuel_cost.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      514 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy/inputs/fuel_supply_curves.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      179 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy/inputs/fuels.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)     2704 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy/inputs/gen_build_costs.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      233 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy/inputs/gen_build_predetermined.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)     3812 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy/inputs/gen_info.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      161 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy/inputs/load_zones.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      303 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy/inputs/loads.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      470 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy/inputs/modules.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       54 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy/inputs/non_fuel_energy_sources.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       72 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy/inputs/periods.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      112 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy/inputs/regional_fuel_markets.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)        6 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy/inputs/switch_inputs_version.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)      218 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy/inputs/timepoints.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      158 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy/inputs/timeseries.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       87 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy/inputs/trans_params.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      148 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy/inputs/transmission_lines.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)     2365 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy/inputs/variable_capacity_factors.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       77 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy/inputs/zone_balancing_areas.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      138 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy/inputs/zone_coincident_peak_demand.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      299 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy/inputs/zone_fuel_cost_diff.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      160 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy/inputs/zone_to_regional_fuel_market.csv
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.377133 switch_model-2.0.8/examples/3zone_toy/outputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       17 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy/outputs/total_cost.txt
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.378139 switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/
+-rw-r--r--   0 matthias   (501) wheel        (0)     7183 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/PySPInputGenerator.py
+-rw-r--r--   0 matthias   (501) wheel        (0)    11070 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/README.md
+-rw-r--r--   0 matthias   (501) wheel        (0)     3627 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/ReferenceModel.py
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.381210 switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/inputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/inputs/financials.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      566 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/inputs/fuel_cost.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      191 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/inputs/fuels.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)     2704 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/inputs/gen_build_costs.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      233 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/inputs/gen_build_predetermined.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)     3689 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/inputs/gen_info.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      124 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/inputs/load_zones.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      303 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/inputs/loads.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      469 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/inputs/modules.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       54 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/inputs/non_fuel_energy_sources.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       72 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/inputs/periods.csv
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.382043 switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/inputs/pysp_inputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)      429 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/inputs/pysp_inputs/HighFuelCosts.dat
+-rw-r--r--   0 matthias   (501) wheel        (0)      432 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/inputs/pysp_inputs/LowFuelCosts.dat
+-rw-r--r--   0 matthias   (501) wheel        (0)        0 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/inputs/pysp_inputs/MediumFuelCosts.dat
+-rw-r--r--   0 matthias   (501) wheel        (0)    25575 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/inputs/pysp_inputs/RootNode.dat
+-rw-r--r--   0 matthias   (501) wheel        (0)     1039 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/inputs/pysp_inputs/ScenarioStructure.dat
+-rw-r--r--   0 matthias   (501) wheel        (0)        6 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/inputs/switch_inputs_version.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)      218 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/inputs/timepoints.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      158 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/inputs/timeseries.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      148 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/inputs/transmission_lines.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)     2365 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/inputs/variable_capacity_factors.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       77 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/inputs/zone_balancing_areas.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      138 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/inputs/zone_coincident_peak_demand.csv
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.382705 switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/outputs-runef/
+-rw-r--r--   0 matthias   (501) wheel        (0)    69326 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/outputs-runef/ef.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      528 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/outputs-runef/ef_StageCostDetail.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)    22488 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/outputs-runef/runef-stdoutput.txt
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.383430 switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/outputs-runph-rhosetter/
+-rw-r--r--   0 matthias   (501) wheel        (0)    70071 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/outputs-runph-rhosetter/ph.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      529 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/outputs-runph-rhosetter/ph_StageCostDetail.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)    62632 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/outputs-runph-rhosetter/runph-rhosetter-stdoutput.txt
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.384153 switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/outputs-runph-rhosetter-FS-only/
+-rw-r--r--   0 matthias   (501) wheel        (0)    70071 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/outputs-runph-rhosetter-FS-only/ph.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      529 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/outputs-runph-rhosetter-FS-only/ph_StageCostDetail.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)    62644 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/outputs-runph-rhosetter-FS-only/runph-rhosetter-FS-only-stdoutput.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)     1426 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/pha_bounds_cfg.py
+-rw-r--r--   0 matthias   (501) wheel        (0)     3211 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/rhosetter.py
+-rw-r--r--   0 matthias   (501) wheel        (0)     1639 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/rhosetter_FS_only.py
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.384395 switch_model-2.0.8/examples/carbon_cap/
+-rw-r--r--   0 matthias   (501) wheel        (0)      236 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/carbon_cap/README.md
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.388324 switch_model-2.0.8/examples/carbon_cap/inputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       84 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/carbon_cap/inputs/carbon_policies.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/carbon_cap/inputs/financials.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      487 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/carbon_cap/inputs/fuel_cost.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      514 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/carbon_cap/inputs/fuel_supply_curves.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      191 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/carbon_cap/inputs/fuels.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)     2704 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/carbon_cap/inputs/gen_build_costs.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      233 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/carbon_cap/inputs/gen_build_predetermined.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)     3818 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/carbon_cap/inputs/gen_info.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      124 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/carbon_cap/inputs/load_zones.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      303 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/carbon_cap/inputs/loads.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      508 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/carbon_cap/inputs/modules.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       54 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/carbon_cap/inputs/non_fuel_energy_sources.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       72 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/carbon_cap/inputs/periods.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      112 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/carbon_cap/inputs/regional_fuel_markets.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)        6 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/carbon_cap/inputs/switch_inputs_version.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)      218 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/carbon_cap/inputs/timepoints.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      158 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/carbon_cap/inputs/timeseries.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      148 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/carbon_cap/inputs/transmission_lines.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)     2365 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/carbon_cap/inputs/variable_capacity_factors.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       77 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/carbon_cap/inputs/zone_balancing_areas.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      138 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/carbon_cap/inputs/zone_coincident_peak_demand.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      299 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/carbon_cap/inputs/zone_fuel_cost_diff.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      160 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/carbon_cap/inputs/zone_to_regional_fuel_market.csv
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.388494 switch_model-2.0.8/examples/carbon_cap/outputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       19 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/carbon_cap/outputs/total_cost.txt
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.388657 switch_model-2.0.8/examples/ccs/
+-rw-r--r--   0 matthias   (501) wheel        (0)      129 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/ccs/README.md
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.391156 switch_model-2.0.8/examples/ccs/inputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/ccs/inputs/financials.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       56 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/ccs/inputs/fuel_cost.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/ccs/inputs/fuels.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      262 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/ccs/inputs/gen_build_costs.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      111 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/ccs/inputs/gen_build_predetermined.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      596 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/ccs/inputs/gen_info.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       60 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/ccs/inputs/load_zones.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       59 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/ccs/inputs/loads.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      347 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/ccs/inputs/modules.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       31 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/ccs/inputs/non_fuel_energy_sources.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       57 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/ccs/inputs/periods.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)        6 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/ccs/inputs/switch_inputs_version.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       78 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/ccs/inputs/timepoints.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       95 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/ccs/inputs/timeseries.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       96 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/ccs/inputs/variable_capacity_factors.csv
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.391315 switch_model-2.0.8/examples/ccs/outputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       19 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/ccs/outputs/total_cost.txt
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.391468 switch_model-2.0.8/examples/copperplate0/
+-rw-r--r--   0 matthias   (501) wheel        (0)      262 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/copperplate0/README.md
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.394742 switch_model-2.0.8/examples/copperplate0/inputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/copperplate0/inputs/financials.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       56 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/copperplate0/inputs/fuel_cost.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/copperplate0/inputs/fuels.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      262 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/copperplate0/inputs/gen_build_costs.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      111 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/copperplate0/inputs/gen_build_predetermined.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      532 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/copperplate0/inputs/gen_info.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       16 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/copperplate0/inputs/load_zones.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       59 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/copperplate0/inputs/loads.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      347 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/copperplate0/inputs/modules.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       31 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/copperplate0/inputs/non_fuel_energy_sources.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       57 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/copperplate0/inputs/periods.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)        6 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/copperplate0/inputs/switch_inputs_version.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       78 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/copperplate0/inputs/timepoints.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       95 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/copperplate0/inputs/timeseries.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       96 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/copperplate0/inputs/variable_capacity_factors.csv
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.394900 switch_model-2.0.8/examples/copperplate0/outputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       18 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/copperplate0/outputs/total_cost.txt
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.395075 switch_model-2.0.8/examples/copperplate1/
+-rw-r--r--   0 matthias   (501) wheel        (0)      336 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/copperplate1/README.md
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.399008 switch_model-2.0.8/examples/copperplate1/inputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/copperplate1/inputs/financials.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      187 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/copperplate1/inputs/fuel_supply_curves.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       91 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/copperplate1/inputs/fuels.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      466 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/copperplate1/inputs/gen_build_costs.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      119 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/copperplate1/inputs/gen_build_predetermined.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      974 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/copperplate1/inputs/gen_info.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       73 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/copperplate1/inputs/load_zones.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       59 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/copperplate1/inputs/loads.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      383 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/copperplate1/inputs/modules.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       31 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/copperplate1/inputs/non_fuel_energy_sources.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       57 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/copperplate1/inputs/periods.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/copperplate1/inputs/regional_fuel_markets.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)        6 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/copperplate1/inputs/switch_inputs_version.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       78 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/copperplate1/inputs/timepoints.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       95 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/copperplate1/inputs/timeseries.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      231 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/copperplate1/inputs/variable_capacity_factors.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       60 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/copperplate1/inputs/zone_to_regional_fuel_market.csv
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.399201 switch_model-2.0.8/examples/copperplate1/outputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       18 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/copperplate1/outputs/total_cost.txt
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.399555 switch_model-2.0.8/examples/custom_extension/
+-rw-r--r--   0 matthias   (501) wheel        (0)      235 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/custom_extension/README
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.399731 switch_model-2.0.8/examples/custom_extension/__pycache__/
+-rw-r--r--   0 matthias   (501) wheel        (0)     1417 2024-04-25 22:00:59.000000 switch_model-2.0.8/examples/custom_extension/__pycache__/sunk_costs.cpython-312.pyc
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.402858 switch_model-2.0.8/examples/custom_extension/inputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/custom_extension/inputs/financials.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       56 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/custom_extension/inputs/fuel_cost.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/custom_extension/inputs/fuels.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      262 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/custom_extension/inputs/gen_build_costs.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      111 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/custom_extension/inputs/gen_build_predetermined.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      532 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/custom_extension/inputs/gen_info.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       60 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/custom_extension/inputs/load_zones.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       59 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/custom_extension/inputs/loads.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      358 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/custom_extension/inputs/modules.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       31 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/custom_extension/inputs/non_fuel_energy_sources.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       57 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/custom_extension/inputs/periods.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)        6 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/custom_extension/inputs/switch_inputs_version.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       78 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/custom_extension/inputs/timepoints.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       95 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/custom_extension/inputs/timeseries.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       96 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/custom_extension/inputs/variable_capacity_factors.csv
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.403005 switch_model-2.0.8/examples/custom_extension/outputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       19 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/custom_extension/outputs/total_cost.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)     1060 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/custom_extension/sunk_costs.py
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.403149 switch_model-2.0.8/examples/diagnose_infeasibility/
+-rw-r--r--   0 matthias   (501) wheel        (0)     1385 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/diagnose_infeasibility/README.md
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.405449 switch_model-2.0.8/examples/diagnose_infeasibility/inputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/diagnose_infeasibility/inputs/financials.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       56 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/diagnose_infeasibility/inputs/fuel_cost.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/diagnose_infeasibility/inputs/fuels.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      128 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/diagnose_infeasibility/inputs/gen_build_costs.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      533 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/diagnose_infeasibility/inputs/gen_info.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       60 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/diagnose_infeasibility/inputs/load_zones.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       59 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/diagnose_infeasibility/inputs/loads.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      428 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/diagnose_infeasibility/inputs/modules.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       31 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/diagnose_infeasibility/inputs/non_fuel_energy_sources.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       57 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/diagnose_infeasibility/inputs/periods.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)        6 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/diagnose_infeasibility/inputs/switch_inputs_version.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       78 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/diagnose_infeasibility/inputs/timepoints.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       95 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/diagnose_infeasibility/inputs/timeseries.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       96 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/diagnose_infeasibility/inputs/variable_capacity_factors.csv
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.405646 switch_model-2.0.8/examples/diagnose_infeasibility/outputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       18 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/diagnose_infeasibility/outputs/total_cost.txt
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.405828 switch_model-2.0.8/examples/discrete_and_min_build/
+-rw-r--r--   0 matthias   (501) wheel        (0)      443 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/discrete_and_min_build/README.md
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.409198 switch_model-2.0.8/examples/discrete_and_min_build/inputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/discrete_and_min_build/inputs/financials.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       79 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/discrete_and_min_build/inputs/fuel_supply_curves.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/discrete_and_min_build/inputs/fuels.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      262 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/discrete_and_min_build/inputs/gen_build_costs.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      111 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/discrete_and_min_build/inputs/gen_build_predetermined.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      553 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/discrete_and_min_build/inputs/gen_info.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       73 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/discrete_and_min_build/inputs/load_zones.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       59 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/discrete_and_min_build/inputs/loads.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      431 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/discrete_and_min_build/inputs/modules.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       31 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/discrete_and_min_build/inputs/non_fuel_energy_sources.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       57 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/discrete_and_min_build/inputs/periods.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       44 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/discrete_and_min_build/inputs/regional_fuel_markets.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)        6 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/discrete_and_min_build/inputs/switch_inputs_version.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       78 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/discrete_and_min_build/inputs/timepoints.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       95 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/discrete_and_min_build/inputs/timeseries.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       96 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/discrete_and_min_build/inputs/variable_capacity_factors.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       68 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/discrete_and_min_build/inputs/zone_coincident_peak_demand.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       44 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/discrete_and_min_build/inputs/zone_to_regional_fuel_market.csv
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.409359 switch_model-2.0.8/examples/discrete_and_min_build/outputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       18 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/discrete_and_min_build/outputs/total_cost.txt
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.409525 switch_model-2.0.8/examples/discrete_build/
+-rw-r--r--   0 matthias   (501) wheel        (0)      317 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/discrete_build/README.md
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.412477 switch_model-2.0.8/examples/discrete_build/inputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/discrete_build/inputs/financials.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       79 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/discrete_build/inputs/fuel_supply_curves.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/discrete_build/inputs/fuels.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      262 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/discrete_build/inputs/gen_build_costs.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      111 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/discrete_build/inputs/gen_build_predetermined.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      553 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/discrete_build/inputs/gen_info.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       73 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/discrete_build/inputs/load_zones.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       59 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/discrete_build/inputs/loads.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      431 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/discrete_build/inputs/modules.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       31 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/discrete_build/inputs/non_fuel_energy_sources.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       57 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/discrete_build/inputs/periods.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       44 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/discrete_build/inputs/regional_fuel_markets.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)        6 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/discrete_build/inputs/switch_inputs_version.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       78 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/discrete_build/inputs/timepoints.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       95 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/discrete_build/inputs/timeseries.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       96 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/discrete_build/inputs/variable_capacity_factors.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       68 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/discrete_build/inputs/zone_coincident_peak_demand.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       44 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/discrete_build/inputs/zone_to_regional_fuel_market.csv
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.412610 switch_model-2.0.8/examples/discrete_build/outputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       18 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/discrete_build/outputs/total_cost.txt
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.412804 switch_model-2.0.8/examples/dr_simple/
+-rw-r--r--   0 matthias   (501) wheel        (0)      378 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/dr_simple/README.md
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.415759 switch_model-2.0.8/examples/dr_simple/inputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       86 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/dr_simple/inputs/dr_data.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/dr_simple/inputs/financials.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      187 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/dr_simple/inputs/fuel_supply_curves.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       91 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/dr_simple/inputs/fuels.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      466 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/dr_simple/inputs/gen_build_costs.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      128 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/dr_simple/inputs/gen_build_predetermined.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      974 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/dr_simple/inputs/gen_info.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       73 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/dr_simple/inputs/load_zones.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       59 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/dr_simple/inputs/loads.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      563 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/dr_simple/inputs/modules.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       31 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/dr_simple/inputs/non_fuel_energy_sources.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       57 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/dr_simple/inputs/periods.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/dr_simple/inputs/regional_fuel_markets.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)        6 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/dr_simple/inputs/switch_inputs_version.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)      104 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/dr_simple/inputs/timepoints.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       95 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/dr_simple/inputs/timeseries.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      231 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/dr_simple/inputs/variable_capacity_factors.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       60 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/dr_simple/inputs/zone_to_regional_fuel_market.csv
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.416041 switch_model-2.0.8/examples/dr_simple/outputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       18 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/dr_simple/outputs/total_cost.txt
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.416266 switch_model-2.0.8/examples/hydro_simple/
+-rw-r--r--   0 matthias   (501) wheel        (0)      547 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydro_simple/README.md
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.418986 switch_model-2.0.8/examples/hydro_simple/inputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydro_simple/inputs/financials.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       56 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydro_simple/inputs/fuel_cost.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydro_simple/inputs/fuels.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      343 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydro_simple/inputs/gen_build_costs.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      161 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydro_simple/inputs/gen_build_predetermined.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      671 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydro_simple/inputs/gen_info.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      114 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydro_simple/inputs/hydro_timeseries.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       60 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydro_simple/inputs/load_zones.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       84 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydro_simple/inputs/loads.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      395 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydro_simple/inputs/modules.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       37 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydro_simple/inputs/non_fuel_energy_sources.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       57 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydro_simple/inputs/periods.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)        6 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydro_simple/inputs/switch_inputs_version.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)      134 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydro_simple/inputs/timepoints.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      123 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydro_simple/inputs/timeseries.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      204 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydro_simple/inputs/variable_capacity_factors.csv
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.419144 switch_model-2.0.8/examples/hydro_simple/outputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       18 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydro_simple/outputs/total_cost.txt
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.419309 switch_model-2.0.8/examples/hydro_system/
+-rw-r--r--   0 matthias   (501) wheel        (0)     1531 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydro_system/README.md
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.423074 switch_model-2.0.8/examples/hydro_system/inputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydro_system/inputs/financials.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       57 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydro_system/inputs/fuel_cost.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       57 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydro_system/inputs/fuels.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      196 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydro_system/inputs/gen_build_costs.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      180 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydro_system/inputs/gen_build_predetermined.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      667 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydro_system/inputs/gen_info.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      181 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydro_system/inputs/hydro_generation_projects.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       61 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydro_system/inputs/load_zones.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      643 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydro_system/inputs/loads.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      395 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydro_system/inputs/modules.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       26 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydro_system/inputs/non_fuel_energy_sources.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       57 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydro_system/inputs/periods.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      124 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydro_system/inputs/reservoirs.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       21 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydro_system/inputs/spillage_penalty.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)        6 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydro_system/inputs/switch_inputs_version.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)     1609 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydro_system/inputs/timepoints.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      143 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydro_system/inputs/timeseries.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)     1244 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydro_system/inputs/variable_capacity_factors.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      158 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydro_system/inputs/water_connections.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)     1290 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydro_system/inputs/water_node_tp_flows.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      147 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydro_system/inputs/water_nodes.csv
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.423228 switch_model-2.0.8/examples/hydro_system/outputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       18 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydro_system/outputs/total_cost.txt
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.423379 switch_model-2.0.8/examples/hydrogen/
+-rw-r--r--   0 matthias   (501) wheel        (0)      943 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydrogen/README.md
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.427849 switch_model-2.0.8/examples/hydrogen/inputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       80 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydrogen/inputs/carbon_policies.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydrogen/inputs/financials.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      635 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydrogen/inputs/fuel_cost.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      480 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydrogen/inputs/fuel_supply_curves.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      208 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydrogen/inputs/fuels.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)     2464 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydrogen/inputs/gen_build_costs.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      233 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydrogen/inputs/gen_build_predetermined.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)     3725 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydrogen/inputs/gen_info.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      132 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydrogen/inputs/gen_multiple_fuels.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      606 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydrogen/inputs/hydrogen.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      124 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydrogen/inputs/load_zones.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      303 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydrogen/inputs/loads.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      556 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydrogen/inputs/modules.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       54 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydrogen/inputs/non_fuel_energy_sources.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       72 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydrogen/inputs/periods.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      112 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydrogen/inputs/regional_fuel_markets.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)        6 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydrogen/inputs/switch_inputs_version.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)      289 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydrogen/inputs/timepoints.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      158 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydrogen/inputs/timeseries.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      148 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydrogen/inputs/transmission_lines.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)     2389 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydrogen/inputs/variable_capacity_factors.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       77 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydrogen/inputs/zone_balancing_areas.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      138 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydrogen/inputs/zone_coincident_peak_demand.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      299 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydrogen/inputs/zone_fuel_cost_diff.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      160 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydrogen/inputs/zone_to_regional_fuel_market.csv
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.428009 switch_model-2.0.8/examples/hydrogen/outputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       18 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/hydrogen/outputs/total_cost.txt
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.428177 switch_model-2.0.8/examples/new_builds_only/
+-rw-r--r--   0 matthias   (501) wheel        (0)      257 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/new_builds_only/README.md
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.430349 switch_model-2.0.8/examples/new_builds_only/inputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/new_builds_only/inputs/financials.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       56 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/new_builds_only/inputs/fuel_cost.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/new_builds_only/inputs/fuels.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      156 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/new_builds_only/inputs/gen_build_costs.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      532 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/new_builds_only/inputs/gen_info.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       60 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/new_builds_only/inputs/load_zones.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       59 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/new_builds_only/inputs/loads.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      347 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/new_builds_only/inputs/modules.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       31 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/new_builds_only/inputs/non_fuel_energy_sources.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       57 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/new_builds_only/inputs/periods.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)        6 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/new_builds_only/inputs/switch_inputs_version.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       78 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/new_builds_only/inputs/timepoints.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       95 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/new_builds_only/inputs/timeseries.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       96 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/new_builds_only/inputs/variable_capacity_factors.csv
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.430532 switch_model-2.0.8/examples/new_builds_only/outputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       19 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/new_builds_only/outputs/total_cost.txt
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.430733 switch_model-2.0.8/examples/planning_reserves/
+-rw-r--r--   0 matthias   (501) wheel        (0)      307 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/planning_reserves/README.md
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.435552 switch_model-2.0.8/examples/planning_reserves/inputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/planning_reserves/inputs/financials.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      487 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/planning_reserves/inputs/fuel_cost.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      514 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/planning_reserves/inputs/fuel_supply_curves.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      191 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/planning_reserves/inputs/fuels.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)     2552 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/planning_reserves/inputs/gen_build_costs.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      233 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/planning_reserves/inputs/gen_build_predetermined.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)     4024 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/planning_reserves/inputs/gen_info.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      124 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/planning_reserves/inputs/load_zones.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      303 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/planning_reserves/inputs/loads.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      511 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/planning_reserves/inputs/modules.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       54 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/planning_reserves/inputs/non_fuel_energy_sources.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       72 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/planning_reserves/inputs/periods.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      160 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/planning_reserves/inputs/planning_reserve_requirement_zones.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      160 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/planning_reserves/inputs/planning_reserve_requirements.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      112 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/planning_reserves/inputs/regional_fuel_markets.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)     2741 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/planning_reserves/inputs/reserve_capacity_value.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)        6 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/planning_reserves/inputs/switch_inputs_version.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)      218 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/planning_reserves/inputs/timepoints.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      158 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/planning_reserves/inputs/timeseries.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      148 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/planning_reserves/inputs/transmission_lines.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)     2365 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/planning_reserves/inputs/variable_capacity_factors.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       77 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/planning_reserves/inputs/zone_balancing_areas.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      138 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/planning_reserves/inputs/zone_coincident_peak_demand.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      299 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/planning_reserves/inputs/zone_fuel_cost_diff.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      160 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/planning_reserves/inputs/zone_to_regional_fuel_market.csv
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.435740 switch_model-2.0.8/examples/planning_reserves/outputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       19 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/planning_reserves/outputs/total_cost.txt
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.435953 switch_model-2.0.8/examples/production_cost_models/
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.436131 switch_model-2.0.8/examples/production_cost_models/1plant/
+-rw-r--r--   0 matthias   (501) wheel        (0)      211 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/1plant/README.md
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.439164 switch_model-2.0.8/examples/production_cost_models/1plant/inputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/1plant/inputs/financials.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       56 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/1plant/inputs/fuel_cost.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/1plant/inputs/fuels.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       90 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/1plant/inputs/gen_build_costs.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       69 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/1plant/inputs/gen_build_predetermined.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      338 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/1plant/inputs/gen_info.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       72 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/1plant/inputs/load_zones.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       45 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/1plant/inputs/loads.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      382 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/1plant/inputs/modules.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       57 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/1plant/inputs/periods.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)        6 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/1plant/inputs/switch_inputs_version.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       56 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/1plant/inputs/timepoints.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       96 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/1plant/inputs/timeseries.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       68 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/1plant/inputs/zone_coincident_peak_demand.csv
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.439346 switch_model-2.0.8/examples/production_cost_models/1plant/outputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       19 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/1plant/outputs/total_cost.txt
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.439641 switch_model-2.0.8/examples/production_cost_models/3plants/
+-rw-r--r--   0 matthias   (501) wheel        (0)      211 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/3plants/README.md
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.443518 switch_model-2.0.8/examples/production_cost_models/3plants/inputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/3plants/inputs/financials.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       56 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/3plants/inputs/fuel_cost.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/3plants/inputs/fuels.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      174 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/3plants/inputs/gen_build_costs.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      119 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/3plants/inputs/gen_build_predetermined.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      532 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/3plants/inputs/gen_info.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       72 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/3plants/inputs/load_zones.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       45 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/3plants/inputs/loads.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      382 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/3plants/inputs/modules.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       25 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/3plants/inputs/non_fuel_energy_sources.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       57 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/3plants/inputs/periods.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)        6 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/3plants/inputs/switch_inputs_version.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       56 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/3plants/inputs/timepoints.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       96 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/3plants/inputs/timeseries.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       68 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/3plants/inputs/zone_coincident_peak_demand.csv
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.443705 switch_model-2.0.8/examples/production_cost_models/3plants/outputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       18 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/3plants/outputs/total_cost.txt
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.443891 switch_model-2.0.8/examples/production_cost_models/4plants/
+-rw-r--r--   0 matthias   (501) wheel        (0)      243 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/4plants/README.md
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.446970 switch_model-2.0.8/examples/production_cost_models/4plants/inputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/4plants/inputs/financials.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       56 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/4plants/inputs/fuel_cost.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/4plants/inputs/fuels.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      210 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/4plants/inputs/gen_build_costs.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      161 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/4plants/inputs/gen_build_predetermined.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      611 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/4plants/inputs/gen_info.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       72 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/4plants/inputs/load_zones.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       76 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/4plants/inputs/loads.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      382 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/4plants/inputs/modules.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       31 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/4plants/inputs/non_fuel_energy_sources.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       57 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/4plants/inputs/periods.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)        6 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/4plants/inputs/switch_inputs_version.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)      122 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/4plants/inputs/timepoints.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       95 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/4plants/inputs/timeseries.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      138 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/4plants/inputs/variable_capacity_factors.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       68 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/4plants/inputs/zone_coincident_peak_demand.csv
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.447302 switch_model-2.0.8/examples/production_cost_models/4plants/outputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       18 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/4plants/outputs/total_cost.txt
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.447507 switch_model-2.0.8/examples/production_cost_models/4plants_with_unserved_load/
+-rw-r--r--   0 matthias   (501) wheel        (0)      395 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/4plants_with_unserved_load/README.md
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.451312 switch_model-2.0.8/examples/production_cost_models/4plants_with_unserved_load/inputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/4plants_with_unserved_load/inputs/financials.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       56 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/4plants_with_unserved_load/inputs/fuel_cost.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/4plants_with_unserved_load/inputs/fuels.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      210 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/4plants_with_unserved_load/inputs/gen_build_costs.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      161 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/4plants_with_unserved_load/inputs/gen_build_predetermined.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      611 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/4plants_with_unserved_load/inputs/gen_info.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       72 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/4plants_with_unserved_load/inputs/load_zones.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       76 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/4plants_with_unserved_load/inputs/loads.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       25 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/4plants_with_unserved_load/inputs/lost_load_cost.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      419 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/4plants_with_unserved_load/inputs/modules.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       31 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/4plants_with_unserved_load/inputs/non_fuel_energy_sources.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       57 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/4plants_with_unserved_load/inputs/periods.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)        6 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/4plants_with_unserved_load/inputs/switch_inputs_version.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)      122 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/4plants_with_unserved_load/inputs/timepoints.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       95 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/4plants_with_unserved_load/inputs/timeseries.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      138 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/4plants_with_unserved_load/inputs/variable_capacity_factors.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       68 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/4plants_with_unserved_load/inputs/zone_coincident_peak_demand.csv
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.451773 switch_model-2.0.8/examples/production_cost_models/4plants_with_unserved_load/outputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       17 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/4plants_with_unserved_load/outputs/total_cost.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)      393 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/README
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.452048 switch_model-2.0.8/examples/production_cost_models/discrete_unit_commit/
+-rw-r--r--   0 matthias   (501) wheel        (0)      243 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/discrete_unit_commit/README.md
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.455420 switch_model-2.0.8/examples/production_cost_models/discrete_unit_commit/inputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/discrete_unit_commit/inputs/financials.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       56 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/discrete_unit_commit/inputs/fuel_cost.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/discrete_unit_commit/inputs/fuels.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      210 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/discrete_unit_commit/inputs/gen_build_costs.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      161 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/discrete_unit_commit/inputs/gen_build_predetermined.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      733 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/discrete_unit_commit/inputs/gen_info.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       72 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/discrete_unit_commit/inputs/load_zones.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       76 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/discrete_unit_commit/inputs/loads.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      477 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/discrete_unit_commit/inputs/modules.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       31 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/discrete_unit_commit/inputs/non_fuel_energy_sources.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       57 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/discrete_unit_commit/inputs/periods.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)        6 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/discrete_unit_commit/inputs/switch_inputs_version.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)      122 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/discrete_unit_commit/inputs/timepoints.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       95 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/discrete_unit_commit/inputs/timeseries.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      138 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/discrete_unit_commit/inputs/variable_capacity_factors.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       68 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/discrete_unit_commit/inputs/zone_coincident_peak_demand.csv
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.455622 switch_model-2.0.8/examples/production_cost_models/discrete_unit_commit/outputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       18 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/discrete_unit_commit/outputs/total_cost.txt
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.456323 switch_model-2.0.8/examples/production_cost_models/spinning_reserves/
+-rw-r--r--   0 matthias   (501) wheel        (0)      118 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/spinning_reserves/README.md
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.460653 switch_model-2.0.8/examples/production_cost_models/spinning_reserves/inputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/spinning_reserves/inputs/financials.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       56 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/spinning_reserves/inputs/fuel_cost.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/spinning_reserves/inputs/fuels.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      210 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/spinning_reserves/inputs/gen_build_costs.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      151 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/spinning_reserves/inputs/gen_build_predetermined.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      206 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/spinning_reserves/inputs/gen_inc_heat_rates.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      801 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/spinning_reserves/inputs/gen_info.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       72 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/spinning_reserves/inputs/load_zones.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       76 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/spinning_reserves/inputs/loads.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      569 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/spinning_reserves/inputs/modules.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       31 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/spinning_reserves/inputs/non_fuel_energy_sources.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       57 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/spinning_reserves/inputs/periods.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       28 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/spinning_reserves/inputs/spinning_reserve_params.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)        6 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/spinning_reserves/inputs/switch_inputs_version.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)      122 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/spinning_reserves/inputs/timepoints.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       95 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/spinning_reserves/inputs/timeseries.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      138 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/spinning_reserves/inputs/variable_capacity_factors.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       68 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/spinning_reserves/inputs/zone_coincident_peak_demand.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       51 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/spinning_reserves/options.txt
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.460911 switch_model-2.0.8/examples/production_cost_models/spinning_reserves/outputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       18 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/spinning_reserves/outputs/total_cost.txt
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.461276 switch_model-2.0.8/examples/production_cost_models/spinning_reserves_advanced/
+-rw-r--r--   0 matthias   (501) wheel        (0)      118 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/spinning_reserves_advanced/README.md
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.467628 switch_model-2.0.8/examples/production_cost_models/spinning_reserves_advanced/inputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/spinning_reserves_advanced/inputs/financials.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       56 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/spinning_reserves_advanced/inputs/fuel_cost.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/spinning_reserves_advanced/inputs/fuels.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      210 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/spinning_reserves_advanced/inputs/gen_build_costs.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      151 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/spinning_reserves_advanced/inputs/gen_build_predetermined.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      206 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/spinning_reserves_advanced/inputs/gen_inc_heat_rates.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      801 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/spinning_reserves_advanced/inputs/gen_info.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       76 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/spinning_reserves_advanced/inputs/generation_projects_reserve_capability.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       72 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/spinning_reserves_advanced/inputs/load_zones.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       76 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/spinning_reserves_advanced/inputs/loads.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      578 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/spinning_reserves_advanced/inputs/modules.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       31 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/spinning_reserves_advanced/inputs/non_fuel_energy_sources.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       57 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/spinning_reserves_advanced/inputs/periods.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       28 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/spinning_reserves_advanced/inputs/spinning_reserve_params.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)        6 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/spinning_reserves_advanced/inputs/switch_inputs_version.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)      122 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/spinning_reserves_advanced/inputs/timepoints.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       95 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/spinning_reserves_advanced/inputs/timeseries.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      138 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/spinning_reserves_advanced/inputs/variable_capacity_factors.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       68 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/spinning_reserves_advanced/inputs/zone_coincident_peak_demand.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       51 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/spinning_reserves_advanced/options.txt
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.468013 switch_model-2.0.8/examples/production_cost_models/spinning_reserves_advanced/outputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       18 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/spinning_reserves_advanced/outputs/total_cost.txt
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.468249 switch_model-2.0.8/examples/production_cost_models/unit_commit/
+-rw-r--r--   0 matthias   (501) wheel        (0)     1229 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/unit_commit/README.md
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.475072 switch_model-2.0.8/examples/production_cost_models/unit_commit/inputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/unit_commit/inputs/financials.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       56 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/unit_commit/inputs/fuel_cost.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/unit_commit/inputs/fuels.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      210 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/unit_commit/inputs/gen_build_costs.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      161 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/unit_commit/inputs/gen_build_predetermined.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      206 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/unit_commit/inputs/gen_inc_heat_rates.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      201 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/unit_commit/inputs/gen_inc_heat_rates_30p_commit.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      215 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/unit_commit/inputs/gen_inc_heat_rates_test_high_end_avoidance.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      761 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/unit_commit/inputs/gen_info.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       72 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/unit_commit/inputs/load_zones.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       76 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/unit_commit/inputs/loads.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      432 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/unit_commit/inputs/modules.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       31 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/unit_commit/inputs/non_fuel_energy_sources.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       57 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/unit_commit/inputs/periods.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)        6 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/unit_commit/inputs/switch_inputs_version.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)      122 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/unit_commit/inputs/timepoints.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       95 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/unit_commit/inputs/timeseries.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      138 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/unit_commit/inputs/variable_capacity_factors.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       68 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/unit_commit/inputs/zone_coincident_peak_demand.csv
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.475790 switch_model-2.0.8/examples/production_cost_models/unit_commit/outputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)      216 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/unit_commit/outputs/dispatch.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       18 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/production_cost_models/unit_commit/outputs/total_cost.txt
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.366935 switch_model-2.0.8/examples/retrofits/
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.481317 switch_model-2.0.8/examples/retrofits/inputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       82 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/retrofits/inputs/carbon_policies.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/retrofits/inputs/financials.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      487 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/retrofits/inputs/fuel_cost.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      480 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/retrofits/inputs/fuel_supply_curves.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      179 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/retrofits/inputs/fuels.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)     2762 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/retrofits/inputs/gen_build_costs.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      252 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/retrofits/inputs/gen_build_predetermined.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)     3909 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/retrofits/inputs/gen_info.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      153 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/retrofits/inputs/gen_retrofits.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      161 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/retrofits/inputs/load_zones.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      303 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/retrofits/inputs/loads.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      602 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/retrofits/inputs/modules.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       54 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/retrofits/inputs/non_fuel_energy_sources.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       72 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/retrofits/inputs/periods.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      112 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/retrofits/inputs/regional_fuel_markets.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)        6 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/retrofits/inputs/switch_inputs_version.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)      218 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/retrofits/inputs/timepoints.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      158 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/retrofits/inputs/timeseries.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       87 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/retrofits/inputs/trans_params.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      148 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/retrofits/inputs/transmission_lines.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)     2365 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/retrofits/inputs/variable_capacity_factors.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       77 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/retrofits/inputs/zone_balancing_areas.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      138 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/retrofits/inputs/zone_coincident_peak_demand.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      299 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/retrofits/inputs/zone_fuel_cost_diff.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      160 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/retrofits/inputs/zone_to_regional_fuel_market.csv
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.481480 switch_model-2.0.8/examples/retrofits/outputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       19 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/retrofits/outputs/total_cost.txt
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.481685 switch_model-2.0.8/examples/rps_simple/
+-rw-r--r--   0 matthias   (501) wheel        (0)      598 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/rps_simple/README.md
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.486107 switch_model-2.0.8/examples/rps_simple/inputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/rps_simple/inputs/financials.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      487 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/rps_simple/inputs/fuel_cost.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      514 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/rps_simple/inputs/fuel_supply_curves.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      218 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/rps_simple/inputs/fuels.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)     2704 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/rps_simple/inputs/gen_build_costs.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      233 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/rps_simple/inputs/gen_build_predetermined.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)     3824 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/rps_simple/inputs/gen_info.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      124 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/rps_simple/inputs/load_zones.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      303 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/rps_simple/inputs/loads.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      503 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/rps_simple/inputs/modules.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       54 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/rps_simple/inputs/non_fuel_energy_sources.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       72 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/rps_simple/inputs/periods.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      112 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/rps_simple/inputs/regional_fuel_markets.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       37 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/rps_simple/inputs/rps_targets.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)        6 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/rps_simple/inputs/switch_inputs_version.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)      218 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/rps_simple/inputs/timepoints.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      158 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/rps_simple/inputs/timeseries.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      148 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/rps_simple/inputs/transmission_lines.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)     2365 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/rps_simple/inputs/variable_capacity_factors.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       77 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/rps_simple/inputs/zone_balancing_areas.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      138 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/rps_simple/inputs/zone_coincident_peak_demand.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      299 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/rps_simple/inputs/zone_fuel_cost_diff.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      160 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/rps_simple/inputs/zone_to_regional_fuel_market.csv
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.486268 switch_model-2.0.8/examples/rps_simple/outputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       19 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/rps_simple/outputs/total_cost.txt
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.486422 switch_model-2.0.8/examples/storage/
+-rw-r--r--   0 matthias   (501) wheel        (0)      137 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/storage/README.md
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.489261 switch_model-2.0.8/examples/storage/inputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/storage/inputs/financials.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       56 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/storage/inputs/fuel_cost.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/storage/inputs/fuels.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      378 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/storage/inputs/gen_build_costs.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      158 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/storage/inputs/gen_build_predetermined.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      576 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/storage/inputs/gen_info.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       60 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/storage/inputs/load_zones.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       59 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/storage/inputs/loads.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      390 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/storage/inputs/modules.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       43 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/storage/inputs/non_fuel_energy_sources.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       57 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/storage/inputs/periods.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)        6 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/storage/inputs/switch_inputs_version.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       78 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/storage/inputs/timepoints.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       95 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/storage/inputs/timeseries.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       96 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/storage/inputs/variable_capacity_factors.csv
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.489522 switch_model-2.0.8/examples/storage/outputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       18 2024-04-23 07:17:04.000000 switch_model-2.0.8/examples/storage/outputs/total_cost.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)     3513 2024-04-23 07:17:04.000000 switch_model-2.0.8/how_to_collaborate.txt
+-rwxr-xr-x   0 matthias   (501) wheel        (0)     2218 2024-04-23 07:17:04.000000 switch_model-2.0.8/run_tests.py
+-rw-r--r--   0 matthias   (501) wheel        (0)       38 2024-04-25 22:11:43.557037 switch_model-2.0.8/setup.cfg
+-rw-r--r--   0 matthias   (501) wheel        (0)     4667 2024-04-23 07:17:04.000000 switch_model-2.0.8/setup.py
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.492443 switch_model-2.0.8/switch_model/
+-rw-r--r--   0 matthias   (501) wheel        (0)     1021 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/__init__.py
+-rw-r--r--   0 matthias   (501) wheel        (0)    12096 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/api.py
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.494205 switch_model-2.0.8/switch_model/balancing/
+-rw-r--r--   0 matthias   (501) wheel        (0)        0 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/balancing/__init__.py
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.494497 switch_model-2.0.8/switch_model/balancing/demand_response/
+-rw-r--r--   0 matthias   (501) wheel        (0)        0 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/balancing/demand_response/__init__.py
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.495212 switch_model-2.0.8/switch_model/balancing/demand_response/iterative/
+-rw-r--r--   0 matthias   (501) wheel        (0)    61868 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/balancing/demand_response/iterative/__init__.py
+-rw-r--r--   0 matthias   (501) wheel        (0)     3386 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/balancing/demand_response/iterative/constant_elasticity_demand_system.py
+-rw-r--r--   0 matthias   (501) wheel        (0)     6468 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/balancing/demand_response/iterative/r_demand_system.py
+-rw-r--r--   0 matthias   (501) wheel        (0)     3636 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/balancing/demand_response/simple.py
+-rwxr-xr-x   0 matthias   (501) wheel        (0)    10633 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/balancing/diagnose_infeasibility.py
+-rw-r--r--   0 matthias   (501) wheel        (0)     8389 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/balancing/load_zones.py
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.495971 switch_model-2.0.8/switch_model/balancing/operating_reserves/
+-rw-r--r--   0 matthias   (501) wheel        (0)        0 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/balancing/operating_reserves/__init__.py
+-rw-r--r--   0 matthias   (501) wheel        (0)     2268 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/balancing/operating_reserves/areas.py
+-rw-r--r--   0 matthias   (501) wheel        (0)    26259 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/balancing/operating_reserves/spinning_reserves.py
+-rw-r--r--   0 matthias   (501) wheel        (0)    30430 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/balancing/operating_reserves/spinning_reserves_advanced.py
+-rw-r--r--   0 matthias   (501) wheel        (0)    13586 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/balancing/planning_reserves.py
+-rw-r--r--   0 matthias   (501) wheel        (0)     2283 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/balancing/unserved_load.py
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.496520 switch_model-2.0.8/switch_model/energy_sources/
+-rw-r--r--   0 matthias   (501) wheel        (0)        0 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/energy_sources/__init__.py
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.497579 switch_model-2.0.8/switch_model/energy_sources/fuel_costs/
+-rw-r--r--   0 matthias   (501) wheel        (0)        0 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/energy_sources/fuel_costs/__init__.py
+-rw-r--r--   0 matthias   (501) wheel        (0)    23882 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/energy_sources/fuel_costs/markets.py
+-rw-r--r--   0 matthias   (501) wheel        (0)     8284 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/energy_sources/fuel_costs/markets_expansion.py
+-rw-r--r--   0 matthias   (501) wheel        (0)     3589 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/energy_sources/fuel_costs/simple.py
+-rw-r--r--   0 matthias   (501) wheel        (0)     4063 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/energy_sources/fuel_costs/simple_per_timepoint.py
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.497894 switch_model-2.0.8/switch_model/energy_sources/hydrogen/
+-rw-r--r--   0 matthias   (501) wheel        (0)        0 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/energy_sources/hydrogen/__init__.py
+-rw-r--r--   0 matthias   (501) wheel        (0)    14391 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/energy_sources/hydrogen/production.py
+-rw-r--r--   0 matthias   (501) wheel        (0)     7046 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/energy_sources/properties.py
+-rw-r--r--   0 matthias   (501) wheel        (0)    18330 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/financials.py
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.498103 switch_model-2.0.8/switch_model/generators/
+-rw-r--r--   0 matthias   (501) wheel        (0)        0 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/generators/__init__.py
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.499083 switch_model-2.0.8/switch_model/generators/core/
+-rw-r--r--   0 matthias   (501) wheel        (0)      377 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/generators/core/__init__.py
+-rw-r--r--   0 matthias   (501) wheel        (0)    36953 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/generators/core/build.py
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.499943 switch_model-2.0.8/switch_model/generators/core/commit/
+-rw-r--r--   0 matthias   (501) wheel        (0)      464 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/generators/core/commit/__init__.py
+-rw-r--r--   0 matthias   (501) wheel        (0)     2743 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/generators/core/commit/discrete.py
+-rw-r--r--   0 matthias   (501) wheel        (0)    16616 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/generators/core/commit/fuel_use.py
+-rw-r--r--   0 matthias   (501) wheel        (0)    19914 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/generators/core/commit/operate.py
+-rw-r--r--   0 matthias   (501) wheel        (0)    24449 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/generators/core/dispatch.py
+-rw-r--r--   0 matthias   (501) wheel        (0)     2367 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/generators/core/gen_discrete_build.py
+-rw-r--r--   0 matthias   (501) wheel        (0)     5444 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/generators/core/no_commit.py
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.500930 switch_model-2.0.8/switch_model/generators/extensions/
+-rw-r--r--   0 matthias   (501) wheel        (0)        0 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/generators/extensions/__init__.py
+-rw-r--r--   0 matthias   (501) wheel        (0)     8082 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/generators/extensions/hydro_simple.py
+-rw-r--r--   0 matthias   (501) wheel        (0)    22789 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/generators/extensions/hydro_system.py
+-rw-r--r--   0 matthias   (501) wheel        (0)    16338 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/generators/extensions/retrofit.py
+-rw-r--r--   0 matthias   (501) wheel        (0)    17156 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/generators/extensions/storage.py
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.508147 switch_model-2.0.8/switch_model/hawaii/
+-rw-r--r--   0 matthias   (501) wheel        (0)        0 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/hawaii/__init__.py
+-rw-r--r--   0 matthias   (501) wheel        (0)     6046 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/hawaii/batteries.py
+-rw-r--r--   0 matthias   (501) wheel        (0)     6719 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/hawaii/batteries_fixed_calendar_life.py
+-rw-r--r--   0 matthias   (501) wheel        (0)    38086 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/hawaii/demand_response_no_reserves.py
+-rw-r--r--   0 matthias   (501) wheel        (0)     3321 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/hawaii/demand_response_simple.py
+-rw-r--r--   0 matthias   (501) wheel        (0)      875 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/hawaii/emission_rules.py
+-rw-r--r--   0 matthias   (501) wheel        (0)    10340 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/hawaii/ev.py
+-rw-r--r--   0 matthias   (501) wheel        (0)    11116 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/hawaii/ev_advanced.py
+-rw-r--r--   0 matthias   (501) wheel        (0)     3706 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/hawaii/fed_subsidies.py
+-rw-r--r--   0 matthias   (501) wheel        (0)     5500 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/hawaii/fuel_markets_expansion.py
+-rw-r--r--   0 matthias   (501) wheel        (0)    37100 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/hawaii/heco_outlook_2019.py
+-rw-r--r--   0 matthias   (501) wheel        (0)    48333 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/hawaii/heco_outlook_2020_06.py
+-rw-r--r--   0 matthias   (501) wheel        (0)    47629 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/hawaii/heco_outlook_2020_08.py
+-rw-r--r--   0 matthias   (501) wheel        (0)    37342 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/hawaii/heco_plan_2020_06.py
+-rw-r--r--   0 matthias   (501) wheel        (0)    36778 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/hawaii/heco_plan_2020_08.py
+-rw-r--r--   0 matthias   (501) wheel        (0)     3658 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/hawaii/hi_spinning_reserves.py
+-rw-r--r--   0 matthias   (501) wheel        (0)    17507 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/hawaii/hydrogen.py
+-rw-r--r--   0 matthias   (501) wheel        (0)     1229 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/hawaii/lake_wilson.py
+-rw-r--r--   0 matthias   (501) wheel        (0)    13491 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/hawaii/lng_conversion.py
+-rw-r--r--   0 matthias   (501) wheel        (0)      560 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/hawaii/no_central_pv.py
+-rw-r--r--   0 matthias   (501) wheel        (0)      391 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/hawaii/no_onshore_wind.py
+-rw-r--r--   0 matthias   (501) wheel        (0)      753 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/hawaii/no_renewables.py
+-rw-r--r--   0 matthias   (501) wheel        (0)      600 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/hawaii/no_wind.py
+-rw-r--r--   0 matthias   (501) wheel        (0)     8195 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/hawaii/oahu_plants.py
+-rw-r--r--   0 matthias   (501) wheel        (0)    14284 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/hawaii/psip_2016_04.py
+-rw-r--r--   0 matthias   (501) wheel        (0)    28641 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/hawaii/psip_2016_12.py
+-rw-r--r--   0 matthias   (501) wheel        (0)     7297 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/hawaii/pumped_hydro.py
+-rw-r--r--   0 matthias   (501) wheel        (0)     7807 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/hawaii/register_hi_storage_reserves.py
+-rw-r--r--   0 matthias   (501) wheel        (0)    13305 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/hawaii/reserves.py
+-rw-r--r--   0 matthias   (501) wheel        (0)    38383 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/hawaii/rps.py
+-rw-r--r--   0 matthias   (501) wheel        (0)    32507 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/hawaii/save_results.py
+-rw-r--r--   0 matthias   (501) wheel        (0)    59375 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/hawaii/scenario_data.py
+-rw-r--r--   0 matthias   (501) wheel        (0)     7349 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/hawaii/scenarios.py
+-rw-r--r--   0 matthias   (501) wheel        (0)    12397 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/hawaii/smooth_dispatch.py
+-rw-r--r--   0 matthias   (501) wheel        (0)     8836 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/hawaii/smooth_dispatch_quadratic.py
+-rw-r--r--   0 matthias   (501) wheel        (0)     2413 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/hawaii/switch_patch.py
+-rw-r--r--   0 matthias   (501) wheel        (0)     2644 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/hawaii/unserved_load.py
+-rw-r--r--   0 matthias   (501) wheel        (0)     3036 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/hawaii/util.py
+-rw-r--r--   0 matthias   (501) wheel        (0)     2014 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/main.py
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.508618 switch_model-2.0.8/switch_model/policies/
+-rw-r--r--   0 matthias   (501) wheel        (0)        0 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/policies/__init__.py
+-rw-r--r--   0 matthias   (501) wheel        (0)     5804 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/policies/carbon_policies.py
+-rw-r--r--   0 matthias   (501) wheel        (0)     6182 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/policies/rps_simple.py
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.509436 switch_model-2.0.8/switch_model/reporting/
+-rw-r--r--   0 matthias   (501) wheel        (0)    10426 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/reporting/__init__.py
+-rw-r--r--   0 matthias   (501) wheel        (0)    30291 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/reporting/basic_exports.py
+-rw-r--r--   0 matthias   (501) wheel        (0)     1675 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/reporting/dump.py
+-rw-r--r--   0 matthias   (501) wheel        (0)     1195 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/reporting/example_export.py
+-rwxr-xr-x   0 matthias   (501) wheel        (0)    54257 2024-04-25 22:00:04.000000 switch_model-2.0.8/switch_model/solve.py
+-rwxr-xr-x   0 matthias   (501) wheel        (0)    17718 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/solve_scenarios.py
+-rw-r--r--   0 matthias   (501) wheel        (0)      366 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/test.py
+-rw-r--r--   0 matthias   (501) wheel        (0)    22424 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/timescales.py
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.509851 switch_model-2.0.8/switch_model/transmission/
+-rw-r--r--   0 matthias   (501) wheel        (0)        0 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/transmission/__init__.py
+-rw-r--r--   0 matthias   (501) wheel        (0)      438 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/transmission/copperplate.py
+-rw-r--r--   0 matthias   (501) wheel        (0)    12576 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/transmission/local_td.py
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.510319 switch_model-2.0.8/switch_model/transmission/transport/
+-rw-r--r--   0 matthias   (501) wheel        (0)      405 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/transmission/transport/__init__.py
+-rw-r--r--   0 matthias   (501) wheel        (0)    15859 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/transmission/transport/build.py
+-rw-r--r--   0 matthias   (501) wheel        (0)     3463 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/transmission/transport/dispatch.py
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.512126 switch_model-2.0.8/switch_model/upgrade/
+-rw-r--r--   0 matthias   (501) wheel        (0)      956 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/upgrade/__init__.py
+-rw-r--r--   0 matthias   (501) wheel        (0)     8087 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/upgrade/manager.py
+-rw-r--r--   0 matthias   (501) wheel        (0)      569 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/upgrade/re_upgrade.py
+-rw-r--r--   0 matthias   (501) wheel        (0)    20437 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/upgrade/upgrade_2_0_0b1.py
+-rw-r--r--   0 matthias   (501) wheel        (0)     2085 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/upgrade/upgrade_2_0_0b2.py
+-rw-r--r--   0 matthias   (501) wheel        (0)     2444 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/upgrade/upgrade_2_0_0b4.py
+-rw-r--r--   0 matthias   (501) wheel        (0)     6121 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/upgrade/upgrade_2_0_1.py
+-rw-r--r--   0 matthias   (501) wheel        (0)     4767 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/upgrade/upgrade_2_0_4.py
+-rw-r--r--   0 matthias   (501) wheel        (0)     6304 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/upgrade/upgrade_2_0_5.py
+-rw-r--r--   0 matthias   (501) wheel        (0)     4126 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/upgrade/upgrade_2_0_6.py
+-rw-r--r--   0 matthias   (501) wheel        (0)     8768 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/upgrade/upgrade_2_0_7.py
+-rw-r--r--   0 matthias   (501) wheel        (0)    45191 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/utilities.py
+-rw-r--r--   0 matthias   (501) wheel        (0)      349 2024-04-23 07:17:04.000000 switch_model-2.0.8/switch_model/version.py
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.493379 switch_model-2.0.8/switch_model.egg-info/
+-rw-r--r--   0 matthias   (501) wheel        (0)     5972 2024-04-25 22:11:43.000000 switch_model-2.0.8/switch_model.egg-info/PKG-INFO
+-rw-r--r--   0 matthias   (501) wheel        (0)    51655 2024-04-25 22:11:43.000000 switch_model-2.0.8/switch_model.egg-info/SOURCES.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)        1 2024-04-25 22:11:43.000000 switch_model-2.0.8/switch_model.egg-info/dependency_links.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       50 2024-04-25 22:11:43.000000 switch_model-2.0.8/switch_model.egg-info/entry_points.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)      160 2024-04-25 22:11:43.000000 switch_model-2.0.8/switch_model.egg-info/requires.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       13 2024-04-25 22:11:43.000000 switch_model-2.0.8/switch_model.egg-info/top_level.txt
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.512804 switch_model-2.0.8/tests/
+-rw-r--r--   0 matthias   (501) wheel        (0)      136 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/__init__.py
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.515129 switch_model-2.0.8/tests/__pycache__/
+-rw-r--r--   0 matthias   (501) wheel        (0)      140 2024-04-25 22:00:21.000000 switch_model-2.0.8/tests/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0 matthias   (501) wheel        (0)     5290 2024-04-25 22:00:21.000000 switch_model-2.0.8/tests/__pycache__/examples_test.cpython-312.pyc
+-rw-r--r--   0 matthias   (501) wheel        (0)     5699 2024-04-25 22:00:21.000000 switch_model-2.0.8/tests/__pycache__/upgrade_test.cpython-312.pyc
+-rw-r--r--   0 matthias   (501) wheel        (0)     6667 2024-04-25 22:00:21.000000 switch_model-2.0.8/tests/__pycache__/utilities_test.cpython-312.pyc
+-rw-r--r--   0 matthias   (501) wheel        (0)     3429 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/examples_test.py
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.515323 switch_model-2.0.8/tests/upgrade_dat/
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.368832 switch_model-2.0.8/tests/upgrade_dat/3zone_toy/
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.519878 switch_model-2.0.8/tests/upgrade_dat/3zone_toy/inputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)      240 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy/inputs/balancing_areas.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       91 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy/inputs/financials.dat
+-rw-r--r--   0 matthias   (501) wheel        (0)      487 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy/inputs/fuel_cost.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      492 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy/inputs/fuel_supply_curves.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      168 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy/inputs/fuels.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      713 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy/inputs/gen_new_build_costs.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)     1266 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy/inputs/generator_info.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      152 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy/inputs/load_zones.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      277 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy/inputs/loads.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       76 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy/inputs/lz_balancing_areas.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      297 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy/inputs/lz_fuel_cost_diff.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      115 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy/inputs/lz_peak_loads.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      159 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy/inputs/lz_to_regional_fuel_market.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       67 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy/inputs/modules.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       53 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy/inputs/non_fuel_energy_sources.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       72 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy/inputs/periods.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      358 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy/inputs/proj_build_costs.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      215 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy/inputs/proj_existing_builds.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)     1765 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy/inputs/project_info.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      111 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy/inputs/regional_fuel_markets.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)        8 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy/inputs/switch_inputs_version.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)      217 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy/inputs/timepoints.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      157 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy/inputs/timeseries.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      147 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy/inputs/transmission_lines.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)     2402 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy/inputs/variable_capacity_factors.tab
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.520030 switch_model-2.0.8/tests/upgrade_dat/3zone_toy/outputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       14 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy/outputs/total_cost.txt
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.369001 switch_model-2.0.8/tests/upgrade_dat/3zone_toy_2_0_6/
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.523677 switch_model-2.0.8/tests/upgrade_dat/3zone_toy_2_0_6/inputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy_2_0_6/inputs/financials.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      487 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy_2_0_6/inputs/fuel_cost.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      514 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy_2_0_6/inputs/fuel_supply_curves.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      179 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy_2_0_6/inputs/fuels.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)     2704 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy_2_0_6/inputs/gen_build_costs.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      231 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy_2_0_6/inputs/gen_build_predetermined.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)     3812 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy_2_0_6/inputs/generation_projects_info.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      124 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy_2_0_6/inputs/load_zones.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      303 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy_2_0_6/inputs/loads.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      470 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy_2_0_6/inputs/modules.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       54 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy_2_0_6/inputs/non_fuel_energy_sources.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       72 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy_2_0_6/inputs/periods.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      112 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy_2_0_6/inputs/regional_fuel_markets.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)        6 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy_2_0_6/inputs/switch_inputs_version.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)      218 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy_2_0_6/inputs/timepoints.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      158 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy_2_0_6/inputs/timeseries.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      116 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy_2_0_6/inputs/trans_params.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      148 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy_2_0_6/inputs/transmission_lines.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)     2365 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy_2_0_6/inputs/variable_capacity_factors.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       77 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy_2_0_6/inputs/zone_balancing_areas.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      138 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy_2_0_6/inputs/zone_coincident_peak_demand.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      299 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy_2_0_6/inputs/zone_fuel_cost_diff.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      160 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy_2_0_6/inputs/zone_to_regional_fuel_market.csv
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.523851 switch_model-2.0.8/tests/upgrade_dat/3zone_toy_2_0_6/outputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       19 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/3zone_toy_2_0_6/outputs/total_cost.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)      678 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/README.txt
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.369171 switch_model-2.0.8/tests/upgrade_dat/copperplate0/
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.527077 switch_model-2.0.8/tests/upgrade_dat/copperplate0/inputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       91 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/copperplate0/inputs/financials.dat
+-rw-r--r--   0 matthias   (501) wheel        (0)       55 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/copperplate0/inputs/fuel_cost.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/copperplate0/inputs/fuels.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      151 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/copperplate0/inputs/gen_new_build_costs.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      391 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/copperplate0/inputs/generator_info.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       59 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/copperplate0/inputs/load_zones.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       55 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/copperplate0/inputs/loads.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       28 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/copperplate0/inputs/modules.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       31 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/copperplate0/inputs/non_fuel_energy_sources.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       57 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/copperplate0/inputs/periods.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      143 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/copperplate0/inputs/proj_build_costs.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       94 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/copperplate0/inputs/proj_existing_builds.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      247 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/copperplate0/inputs/project_info.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)        8 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/copperplate0/inputs/switch_inputs_version.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       78 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/copperplate0/inputs/timepoints.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       95 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/copperplate0/inputs/timeseries.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       84 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/copperplate0/inputs/variable_capacity_factors.tab
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.527227 switch_model-2.0.8/tests/upgrade_dat/copperplate0/outputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       14 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/copperplate0/outputs/total_cost.txt
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.369339 switch_model-2.0.8/tests/upgrade_dat/copperplate1/
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.529978 switch_model-2.0.8/tests/upgrade_dat/copperplate1/inputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       91 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/copperplate1/inputs/financials.dat
+-rw-r--r--   0 matthias   (501) wheel        (0)      181 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/copperplate1/inputs/fuel_supply_curves.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       88 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/copperplate1/inputs/fuels.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      275 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/copperplate1/inputs/gen_new_build_costs.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      599 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/copperplate1/inputs/generator_info.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       73 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/copperplate1/inputs/load_zones.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       55 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/copperplate1/inputs/loads.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       59 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/copperplate1/inputs/lz_to_regional_fuel_market.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       40 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/copperplate1/inputs/modules.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       31 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/copperplate1/inputs/non_fuel_energy_sources.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       57 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/copperplate1/inputs/periods.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      162 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/copperplate1/inputs/proj_build_costs.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      101 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/copperplate1/inputs/proj_existing_builds.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      433 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/copperplate1/inputs/project_info.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       62 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/copperplate1/inputs/regional_fuel_markets.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)        8 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/copperplate1/inputs/switch_inputs_version.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       78 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/copperplate1/inputs/timepoints.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       95 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/copperplate1/inputs/timeseries.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      217 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/copperplate1/inputs/variable_capacity_factors.tab
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.530131 switch_model-2.0.8/tests/upgrade_dat/copperplate1/outputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       14 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/copperplate1/outputs/total_cost.txt
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.530271 switch_model-2.0.8/tests/upgrade_dat/custom_extension/
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.533188 switch_model-2.0.8/tests/upgrade_dat/custom_extension/inputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       91 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/custom_extension/inputs/financials.dat
+-rw-r--r--   0 matthias   (501) wheel        (0)       55 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/custom_extension/inputs/fuel_cost.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/custom_extension/inputs/fuels.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      151 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/custom_extension/inputs/gen_new_build_costs.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      391 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/custom_extension/inputs/generator_info.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       59 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/custom_extension/inputs/load_zones.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       55 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/custom_extension/inputs/loads.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       50 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/custom_extension/inputs/modules.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       31 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/custom_extension/inputs/non_fuel_energy_sources.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       57 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/custom_extension/inputs/periods.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      143 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/custom_extension/inputs/proj_build_costs.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       94 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/custom_extension/inputs/proj_existing_builds.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      215 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/custom_extension/inputs/project_info.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)        8 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/custom_extension/inputs/switch_inputs_version.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       78 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/custom_extension/inputs/timepoints.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       95 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/custom_extension/inputs/timeseries.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       84 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/custom_extension/inputs/variable_capacity_factors.tab
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.533399 switch_model-2.0.8/tests/upgrade_dat/custom_extension/outputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       14 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/custom_extension/outputs/total_cost.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)     1073 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/custom_extension/sunk_costs.py
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.369686 switch_model-2.0.8/tests/upgrade_dat/hydro_simple/
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.536443 switch_model-2.0.8/tests/upgrade_dat/hydro_simple/inputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       91 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/hydro_simple/inputs/financials.dat
+-rw-r--r--   0 matthias   (501) wheel        (0)       55 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/hydro_simple/inputs/fuel_cost.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/hydro_simple/inputs/fuels.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      151 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/hydro_simple/inputs/gen_new_build_costs.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      480 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/hydro_simple/inputs/generator_info.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      110 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/hydro_simple/inputs/hydro_timeseries.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       59 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/hydro_simple/inputs/load_zones.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       76 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/hydro_simple/inputs/loads.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       52 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/hydro_simple/inputs/modules.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       37 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/hydro_simple/inputs/non_fuel_energy_sources.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       57 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/hydro_simple/inputs/periods.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      213 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/hydro_simple/inputs/proj_build_costs.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      133 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/hydro_simple/inputs/proj_existing_builds.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      308 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/hydro_simple/inputs/project_info.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)        8 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/hydro_simple/inputs/switch_inputs_version.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)      133 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/hydro_simple/inputs/timepoints.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      123 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/hydro_simple/inputs/timeseries.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      186 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/hydro_simple/inputs/variable_capacity_factors.tab
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.536598 switch_model-2.0.8/tests/upgrade_dat/hydro_simple/outputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       14 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/hydro_simple/outputs/total_cost.txt
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.369855 switch_model-2.0.8/tests/upgrade_dat/hydro_system/
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.540620 switch_model-2.0.8/tests/upgrade_dat/hydro_system/inputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       91 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/hydro_system/inputs/financials.dat
+-rw-r--r--   0 matthias   (501) wheel        (0)       57 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/hydro_system/inputs/fuel_cost.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       57 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/hydro_system/inputs/fuels.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       69 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/hydro_system/inputs/gen_new_build_costs.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      396 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/hydro_system/inputs/generator_info.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      164 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/hydro_system/inputs/hydro_projects.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       61 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/hydro_system/inputs/load_zones.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      642 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/hydro_system/inputs/loads.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       52 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/hydro_system/inputs/modules.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       26 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/hydro_system/inputs/non_fuel_energy_sources.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       57 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/hydro_system/inputs/periods.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      187 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/hydro_system/inputs/proj_build_costs.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      163 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/hydro_system/inputs/proj_existing_builds.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      330 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/hydro_system/inputs/project_info.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      149 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/hydro_system/inputs/reservoirs.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)        8 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/hydro_system/inputs/switch_inputs_version.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)     1609 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/hydro_system/inputs/timepoints.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      143 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/hydro_system/inputs/timeseries.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)     1183 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/hydro_system/inputs/variable_capacity_factors.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      183 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/hydro_system/inputs/water_connections.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)     1291 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/hydro_system/inputs/water_node_tp_flows.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      137 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/hydro_system/inputs/water_nodes.tab
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.540834 switch_model-2.0.8/tests/upgrade_dat/hydro_system/outputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       14 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/hydro_system/outputs/total_cost.txt
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.370317 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.370083 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/4plants/
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.544319 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/4plants/inputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       91 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/4plants/inputs/financials.dat
+-rw-r--r--   0 matthias   (501) wheel        (0)       55 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/4plants/inputs/fuel_cost.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/4plants/inputs/fuels.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      446 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/4plants/inputs/generator_info.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       72 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/4plants/inputs/load_zones.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       74 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/4plants/inputs/loads.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       46 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/4plants/inputs/lz_peak_loads.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       37 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/4plants/inputs/modules.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       30 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/4plants/inputs/non_fuel_energy_sources.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       57 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/4plants/inputs/periods.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      200 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/4plants/inputs/proj_build_costs.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      127 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/4plants/inputs/proj_existing_builds.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      248 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/4plants/inputs/project_info.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)        8 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/4plants/inputs/switch_inputs_version.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)      122 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/4plants/inputs/timepoints.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       95 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/4plants/inputs/timeseries.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      126 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/4plants/inputs/variable_capacity_factors.tab
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.544469 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/4plants/outputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       14 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/4plants/outputs/total_cost.txt
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.370254 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/discrete_unit_commit/
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.547252 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/discrete_unit_commit/inputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       91 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/discrete_unit_commit/inputs/financials.dat
+-rw-r--r--   0 matthias   (501) wheel        (0)       55 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/discrete_unit_commit/inputs/fuel_cost.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/discrete_unit_commit/inputs/fuels.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      552 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/discrete_unit_commit/inputs/generator_info.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       72 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/discrete_unit_commit/inputs/load_zones.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       74 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/discrete_unit_commit/inputs/loads.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       46 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/discrete_unit_commit/inputs/lz_peak_loads.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       66 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/discrete_unit_commit/inputs/modules.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       30 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/discrete_unit_commit/inputs/non_fuel_energy_sources.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       57 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/discrete_unit_commit/inputs/periods.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      200 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/discrete_unit_commit/inputs/proj_build_costs.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      127 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/discrete_unit_commit/inputs/proj_existing_builds.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      248 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/discrete_unit_commit/inputs/project_info.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)        8 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/discrete_unit_commit/inputs/switch_inputs_version.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)      122 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/discrete_unit_commit/inputs/timepoints.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       95 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/discrete_unit_commit/inputs/timeseries.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      126 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/discrete_unit_commit/inputs/variable_capacity_factors.tab
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.547442 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/discrete_unit_commit/outputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       14 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/discrete_unit_commit/outputs/total_cost.txt
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.370427 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/unit_commit/
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.550547 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/unit_commit/inputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       91 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/unit_commit/inputs/financials.dat
+-rw-r--r--   0 matthias   (501) wheel        (0)       55 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/unit_commit/inputs/fuel_cost.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/unit_commit/inputs/fuels.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      197 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/unit_commit/inputs/gen_inc_heat_rates.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      197 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/unit_commit/inputs/gen_inc_heat_rates_30p_commit.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      205 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/unit_commit/inputs/gen_inc_heat_rates_test_high_end_avoidance.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      553 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/unit_commit/inputs/generator_info.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       72 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/unit_commit/inputs/load_zones.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       74 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/unit_commit/inputs/loads.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       46 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/unit_commit/inputs/lz_peak_loads.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       38 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/unit_commit/inputs/modules.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       30 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/unit_commit/inputs/non_fuel_energy_sources.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       57 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/unit_commit/inputs/periods.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      200 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/unit_commit/inputs/proj_build_costs.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      127 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/unit_commit/inputs/proj_existing_builds.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      248 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/unit_commit/inputs/project_info.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)        8 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/unit_commit/inputs/switch_inputs_version.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)      122 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/unit_commit/inputs/timepoints.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       95 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/unit_commit/inputs/timeseries.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      126 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/unit_commit/inputs/variable_capacity_factors.tab
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.550738 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/unit_commit/outputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       14 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/production_cost_models/unit_commit/outputs/total_cost.txt
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.370586 switch_model-2.0.8/tests/upgrade_dat/storage/
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.553447 switch_model-2.0.8/tests/upgrade_dat/storage/inputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       91 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/storage/inputs/financials.dat
+-rw-r--r--   0 matthias   (501) wheel        (0)       55 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/storage/inputs/fuel_cost.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/storage/inputs/fuels.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      225 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/storage/inputs/gen_new_build_costs.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      484 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/storage/inputs/generator_info.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       59 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/storage/inputs/load_zones.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       55 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/storage/inputs/loads.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       47 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/storage/inputs/modules.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       42 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/storage/inputs/non_fuel_energy_sources.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       57 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/storage/inputs/periods.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      115 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/storage/inputs/proj_build_costs.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       79 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/storage/inputs/proj_existing_builds.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)      254 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/storage/inputs/project_info.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)        8 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/storage/inputs/switch_inputs_version.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       78 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/storage/inputs/timepoints.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       95 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/storage/inputs/timeseries.tab
+-rw-r--r--   0 matthias   (501) wheel        (0)       84 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/storage/inputs/variable_capacity_factors.tab
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.553623 switch_model-2.0.8/tests/upgrade_dat/storage/outputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       13 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/storage/outputs/total_cost.txt
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.370753 switch_model-2.0.8/tests/upgrade_dat/storage_206/
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.555768 switch_model-2.0.8/tests/upgrade_dat/storage_206/inputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/storage_206/inputs/financials.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       56 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/storage_206/inputs/fuel_cost.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       63 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/storage_206/inputs/fuels.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      328 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/storage_206/inputs/gen_build_costs.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      153 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/storage_206/inputs/gen_build_predetermined.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      576 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/storage_206/inputs/generation_projects_info.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       60 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/storage_206/inputs/load_zones.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       59 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/storage_206/inputs/loads.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)      390 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/storage_206/inputs/modules.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       43 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/storage_206/inputs/non_fuel_energy_sources.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       57 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/storage_206/inputs/periods.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)        6 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/storage_206/inputs/switch_inputs_version.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)       78 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/storage_206/inputs/timepoints.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       95 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/storage_206/inputs/timeseries.csv
+-rw-r--r--   0 matthias   (501) wheel        (0)       96 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/storage_206/inputs/variable_capacity_factors.csv
+drwxr-xr-x   0 matthias   (501) wheel        (0)        0 2024-04-25 22:11:43.555920 switch_model-2.0.8/tests/upgrade_dat/storage_206/outputs/
+-rw-r--r--   0 matthias   (501) wheel        (0)       19 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_dat/storage_206/outputs/total_cost.txt
+-rw-r--r--   0 matthias   (501) wheel        (0)     3951 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/upgrade_test.py
+-rw-r--r--   0 matthias   (501) wheel        (0)     4600 2024-04-23 07:17:04.000000 switch_model-2.0.8/tests/utilities_test.py
```

### Comparing `switch_model-2.0.7/AUTHORS` & `switch_model-2.0.8/AUTHORS`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/DEV_INSTALL.txt` & `switch_model-2.0.8/DEV_INSTALL.txt`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/LICENSE` & `switch_model-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/LICENSE.BOILERPLATE` & `switch_model-2.0.8/LICENSE.BOILERPLATE`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/PKG-INFO` & `switch_model-2.0.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: switch_model
-Version: 2.0.7
+Version: 2.0.8
 Summary: Switch Power System Planning Model
 Home-page: http://switch-model.org
 Maintainer: Switch Authors
 Maintainer-email: authors@switch-model.org
 License: Apache License 2.0
 Keywords: renewable,power,energy,electricity,production cost,capacity expansion,planning,optimization
 Platform: any
@@ -19,23 +19,35 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7.0, <3.11.0a0
+Requires-Python: >=3.7.2, <3.13.0a0
 Description-Content-Type: text/markdown
-Provides-Extra: advanced
-Provides-Extra: dev
-Provides-Extra: plotting
-Provides-Extra: database_access
 License-File: LICENSE
 License-File: LICENSE.BOILERPLATE
 License-File: AUTHORS
+Requires-Dist: Pyomo<=6.7.1,>=6.0.0
+Requires-Dist: pint
+Requires-Dist: testfixtures
+Requires-Dist: pandas
+Provides-Extra: advanced
+Requires-Dist: numpy; extra == "advanced"
+Requires-Dist: scipy; extra == "advanced"
+Requires-Dist: rpy2; extra == "advanced"
+Requires-Dist: sympy; extra == "advanced"
+Provides-Extra: dev
+Requires-Dist: ipdb; extra == "dev"
+Provides-Extra: plotting
+Requires-Dist: plotnine; extra == "plotting"
+Requires-Dist: matplotlib; extra == "plotting"
+Provides-Extra: database-access
+Requires-Dist: psycopg2-binary; extra == "database-access"
 
 This contains version 2 of the Switch electricity planning model.
 This optimization model is modular and can be used with varying levels
 of complexity. Look in the examples directory for demonstrations of
 using Switch for investment planning or production cost simulation. The
 examples enable varying levels of model complexity by choosing which
 modules to include.
```

### Comparing `switch_model-2.0.7/README` & `switch_model-2.0.8/README`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/3zone_toy/inputs/fuel_supply_curves.csv` & `switch_model-2.0.8/examples/3zone_toy/inputs/fuel_supply_curves.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/3zone_toy/inputs/gen_build_costs.csv` & `switch_model-2.0.8/examples/3zone_toy/inputs/gen_build_costs.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/3zone_toy/inputs/gen_info.csv` & `switch_model-2.0.8/examples/3zone_toy/inputs/gen_info.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/3zone_toy/inputs/variable_capacity_factors.csv` & `switch_model-2.0.8/examples/3zone_toy/inputs/variable_capacity_factors.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/PySPInputGenerator.py` & `switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/PySPInputGenerator.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/README.md` & `switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/README.md`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/ReferenceModel.py` & `switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/ReferenceModel.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/inputs/fuel_cost.csv` & `switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/inputs/fuel_cost.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/inputs/gen_build_costs.csv` & `switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/inputs/gen_build_costs.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/inputs/gen_info.csv` & `switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/inputs/gen_info.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/inputs/pysp_inputs/RootNode.dat` & `switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/inputs/pysp_inputs/RootNode.dat`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/inputs/pysp_inputs/ScenarioStructure.dat` & `switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/inputs/pysp_inputs/ScenarioStructure.dat`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/inputs/variable_capacity_factors.csv` & `switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/inputs/variable_capacity_factors.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/outputs-runef/ef.csv` & `switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/outputs-runef/ef.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/outputs-runef/ef_StageCostDetail.csv` & `switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/outputs-runef/ef_StageCostDetail.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/outputs-runef/runef-stdoutput.txt` & `switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/outputs-runef/runef-stdoutput.txt`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/outputs-runph-rhosetter/ph.csv` & `switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/outputs-runph-rhosetter/ph.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/outputs-runph-rhosetter/ph_StageCostDetail.csv` & `switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/outputs-runph-rhosetter/ph_StageCostDetail.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/outputs-runph-rhosetter/runph-rhosetter-stdoutput.txt` & `switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/outputs-runph-rhosetter/runph-rhosetter-stdoutput.txt`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/outputs-runph-rhosetter-FS-only/ph.csv` & `switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/outputs-runph-rhosetter-FS-only/ph.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/outputs-runph-rhosetter-FS-only/ph_StageCostDetail.csv` & `switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/outputs-runph-rhosetter-FS-only/ph_StageCostDetail.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/outputs-runph-rhosetter-FS-only/runph-rhosetter-FS-only-stdoutput.txt` & `switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/outputs-runph-rhosetter-FS-only/runph-rhosetter-FS-only-stdoutput.txt`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/pha_bounds_cfg.py` & `switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/pha_bounds_cfg.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/rhosetter.py` & `switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/rhosetter.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/3zone_toy_stochastic_PySP/rhosetter_FS_only.py` & `switch_model-2.0.8/examples/3zone_toy_stochastic_PySP/rhosetter_FS_only.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/carbon_cap/inputs/fuel_supply_curves.csv` & `switch_model-2.0.8/examples/carbon_cap/inputs/fuel_supply_curves.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/carbon_cap/inputs/gen_build_costs.csv` & `switch_model-2.0.8/examples/carbon_cap/inputs/gen_build_costs.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/carbon_cap/inputs/gen_info.csv` & `switch_model-2.0.8/examples/carbon_cap/inputs/gen_info.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/carbon_cap/inputs/variable_capacity_factors.csv` & `switch_model-2.0.8/examples/carbon_cap/inputs/variable_capacity_factors.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/ccs/inputs/gen_info.csv` & `switch_model-2.0.8/examples/ccs/inputs/gen_info.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/copperplate0/inputs/gen_info.csv` & `switch_model-2.0.8/examples/copperplate0/inputs/gen_info.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/copperplate1/inputs/gen_info.csv` & `switch_model-2.0.8/examples/copperplate1/inputs/gen_info.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/custom_extension/__pycache__/sunk_costs.cpython-310.pyc` & `switch_model-2.0.8/examples/custom_extension/__pycache__/sunk_costs.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Nov  2 00:23:51 2022 UTC, .py size: 1060 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 21% similar despite different names*

```diff
@@ -1,80 +1,89 @@
-00000000: 6f0d 0d0a 0000 0000 97b8 6163 2404 0000  o.........ac$...
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 1800 0000 6400  .....@...s....d.
-00000030: 5a00 6401 6402 6c01 5400 6403 6404 8400  Z.d.d.l.T.d.d...
-00000040: 5a02 6405 5300 2906 61ac 0200 000a 0a41  Z.d.S.).a......A
-00000050: 6464 2063 7573 746f 6d20 636f 6d70 6f6e  dd custom compon
-00000060: 656e 7473 2074 6f20 7468 6520 5377 6974  ents to the Swit
-00000070: 6368 206d 6f64 656c 2074 6f20 6465 7363  ch model to desc
-00000080: 7269 6265 2066 6978 6564 2073 7973 7465  ribe fixed syste
-00000090: 6d0a 636f 7374 7320 7468 6174 2061 7265  m.costs that are
-000000a0: 206e 6565 6465 6420 746f 2061 6363 7572   needed to accur
-000000b0: 6174 656c 7920 6361 6c63 756c 6174 6520  ately calculate 
-000000c0: 656c 6563 7472 6963 6974 7920 636f 7374  electricity cost
-000000d0: 732e 2054 6869 730a 6d69 6d69 6373 2074  s. This.mimics t
-000000e0: 6865 2063 6f6e 7665 6e74 696f 6e20 6f66  he convention of
-000000f0: 2073 7769 7463 6820 6d6f 6475 6c65 7320   switch modules 
-00000100: 7468 6174 2063 616e 2069 6e63 6c75 6465  that can include
-00000110: 2074 6865 2066 6f6c 6c6f 7769 6e67 0a66   the following.f
-00000120: 756e 6374 696f 6e73 3a0a 0a64 6566 696e  unctions:..defin
-00000130: 655f 636f 6d70 6f6e 656e 7473 286d 6f64  e_components(mod
-00000140: 656c 290a 6465 6669 6e65 5f64 796e 616d  el).define_dynam
-00000150: 6963 5f63 6f6d 706f 6e65 6e74 7328 6d6f  ic_components(mo
-00000160: 6465 6c29 0a6c 6f61 645f 696e 7075 7473  del).load_inputs
-00000170: 286d 6f64 656c 2c20 6461 7461 5f70 6f72  (model, data_por
-00000180: 7461 6c2c 2069 6e70 7574 735f 6469 7229  tal, inputs_dir)
-00000190: 0a70 7265 5f73 6f6c 7665 2869 6e73 7461  .pre_solve(insta
-000001a0: 6e63 652c 206f 7574 6469 7229 0a70 6f73  nce, outdir).pos
-000001b0: 745f 736f 6c76 6528 696e 7374 616e 6365  t_solve(instance
-000001c0: 2c20 6f75 7464 6972 290a 0a49 6e20 7468  , outdir)..In th
-000001d0: 6973 2065 7861 6d70 6c65 2c20 4920 6861  is example, I ha
-000001e0: 7665 206f 6e6c 7920 696d 706c 656d 656e  ve only implemen
-000001f0: 7465 6420 6465 6669 6e65 5f63 6f6d 706f  ted define_compo
-00000200: 6e65 6e74 7328 2920 7768 6963 6820 6164  nents() which ad
-00000210: 6473 0a61 2061 646d 696e 6973 7472 6174  ds.a administrat
-00000220: 696f 6e5f 6665 6573 2070 6172 616d 6574  ion_fees paramet
-00000230: 6572 2074 6f20 7468 6520 6d6f 6465 6c20  er to the model 
-00000240: 7468 6174 2073 7065 6369 6669 6573 2061  that specifies a
-00000250: 2066 6978 6564 0a61 6e6e 7561 6c20 636f   fixed.annual co
-00000260: 7374 206f 6620 3120 6d69 6c6c 696f 6e20  st of 1 million 
-00000270: 646f 6c6c 6172 7320 616e 6420 7265 6769  dollars and regi
-00000280: 7374 6572 7320 7468 6973 2063 6f73 7420  sters this cost 
-00000290: 7769 7468 2074 6865 0a6f 626a 6563 7469  with the.objecti
-000002a0: 7665 2066 756e 6374 696f 6e2e 0a0a 5377  ve function...Sw
-000002b0: 6974 6368 2069 7320 6c69 6365 6e73 6564  itch is licensed
-000002c0: 2075 6e64 6572 2041 7061 6368 6520 4c69   under Apache Li
-000002d0: 6365 6e73 6520 322e 3020 4d6f 7265 2069  cense 2.0 More i
-000002e0: 6e66 6f20 6174 2073 7769 7463 682d 0a6d  nfo at switch-.m
-000002f0: 6f64 656c 2e6f 7267 0ae9 0000 0000 2901  odel.org......).
-00000300: da01 2a63 0100 0000 0000 0000 0000 0000  ..*c............
-00000310: 0100 0000 0500 0000 4300 0000 7326 0000  ........C...s&..
-00000320: 0074 007c 006a 0164 0164 0284 0074 0264  .t.|.j.d.d...t.d
-00000330: 038d 037c 005f 037c 006a 04a0 0564 04a1  ...|._.|.j...d..
-00000340: 0101 0064 0053 0029 054e 6302 0000 0000  ...d.S.).Nc.....
-00000350: 0000 0000 0000 0002 0000 0001 0000 0053  ...............S
-00000360: 0000 0073 0400 0000 6401 5300 2902 4e69  ...s....d.S.).Ni
-00000370: 4042 0f00 a900 2902 da01 6dda 0170 7203  @B....)...m..pr.
-00000380: 0000 0072 0300 0000 fa41 2f70 7269 7661  ...r.....A/priva
-00000390: 7465 2f74 6d70 2f74 7769 6e65 2f73 7769  te/tmp/twine/swi
-000003a0: 7463 682f 6578 616d 706c 6573 2f63 7573  tch/examples/cus
-000003b0: 746f 6d5f 6578 7465 6e73 696f 6e2f 7375  tom_extension/su
-000003c0: 6e6b 5f63 6f73 7473 2e70 79da 083c 6c61  nk_costs.py..<la
-000003d0: 6d62 6461 3e1f 0000 0073 0200 0000 0400  mbda>....s......
-000003e0: 7a23 6465 6669 6e65 5f63 6f6d 706f 6e65  z#define_compone
-000003f0: 6e74 732e 3c6c 6f63 616c 733e 2e3c 6c61  nts.<locals>.<la
-00000400: 6d62 6461 3e29 02da 0a69 6e69 7469 616c  mbda>)...initial
-00000410: 697a 65da 0677 6974 6869 6eda 1361 646d  ize..within..adm
-00000420: 696e 6973 7472 6174 696f 6e5f 6665 6573  inistration_fees
-00000430: 2906 da05 5061 7261 6dda 0750 4552 494f  )...Param..PERIO
-00000440: 4453 da03 416e 7972 0a00 0000 da1a 436f  DS..Anyr......Co
-00000450: 7374 5f43 6f6d 706f 6e65 6e74 735f 5065  st_Components_Pe
-00000460: 725f 5065 7269 6f64 da06 6170 7065 6e64  r_Period..append
-00000470: 2901 da03 6d6f 6472 0300 0000 7203 0000  )...modr....r...
-00000480: 0072 0600 0000 da11 6465 6669 6e65 5f63  .r......define_c
-00000490: 6f6d 706f 6e65 6e74 731d 0000 0073 0800  omponents....s..
-000004a0: 0000 0201 0c01 08ff 1003 7211 0000 004e  ..........r....N
-000004b0: 2903 da07 5f5f 646f 635f 5fda 0d70 796f  )...__doc__..pyo
-000004c0: 6d6f 2e65 6e76 6972 6f6e 7211 0000 0072  mo.environr....r
-000004d0: 0300 0000 7203 0000 0072 0300 0000 7206  ....r....r....r.
-000004e0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-000004f0: 0073 0600 0000 0403 0816 0c03            .s..........
+00000000: cb0d 0d0a 0000 0000 7060 2766 2404 0000  ........p`'f$...
+00000010: e300 0000 0000 0000 0000 0000 0002 0000  ................
+00000020: 0000 0000 00f3 1800 0000 9700 6400 5a00  ............d.Z.
+00000030: 6401 6402 6c01 ad02 0100 6403 8400 5a02  d.d.l.....d...Z.
+00000040: 7904 2905 61ac 0200 000a 0a41 6464 2063  y.).a......Add c
+00000050: 7573 746f 6d20 636f 6d70 6f6e 656e 7473  ustom components
+00000060: 2074 6f20 7468 6520 5377 6974 6368 206d   to the Switch m
+00000070: 6f64 656c 2074 6f20 6465 7363 7269 6265  odel to describe
+00000080: 2066 6978 6564 2073 7973 7465 6d0a 636f   fixed system.co
+00000090: 7374 7320 7468 6174 2061 7265 206e 6565  sts that are nee
+000000a0: 6465 6420 746f 2061 6363 7572 6174 656c  ded to accuratel
+000000b0: 7920 6361 6c63 756c 6174 6520 656c 6563  y calculate elec
+000000c0: 7472 6963 6974 7920 636f 7374 732e 2054  tricity costs. T
+000000d0: 6869 730a 6d69 6d69 6373 2074 6865 2063  his.mimics the c
+000000e0: 6f6e 7665 6e74 696f 6e20 6f66 2073 7769  onvention of swi
+000000f0: 7463 6820 6d6f 6475 6c65 7320 7468 6174  tch modules that
+00000100: 2063 616e 2069 6e63 6c75 6465 2074 6865   can include the
+00000110: 2066 6f6c 6c6f 7769 6e67 0a66 756e 6374   following.funct
+00000120: 696f 6e73 3a0a 0a64 6566 696e 655f 636f  ions:..define_co
+00000130: 6d70 6f6e 656e 7473 286d 6f64 656c 290a  mponents(model).
+00000140: 6465 6669 6e65 5f64 796e 616d 6963 5f63  define_dynamic_c
+00000150: 6f6d 706f 6e65 6e74 7328 6d6f 6465 6c29  omponents(model)
+00000160: 0a6c 6f61 645f 696e 7075 7473 286d 6f64  .load_inputs(mod
+00000170: 656c 2c20 6461 7461 5f70 6f72 7461 6c2c  el, data_portal,
+00000180: 2069 6e70 7574 735f 6469 7229 0a70 7265   inputs_dir).pre
+00000190: 5f73 6f6c 7665 2869 6e73 7461 6e63 652c  _solve(instance,
+000001a0: 206f 7574 6469 7229 0a70 6f73 745f 736f   outdir).post_so
+000001b0: 6c76 6528 696e 7374 616e 6365 2c20 6f75  lve(instance, ou
+000001c0: 7464 6972 290a 0a49 6e20 7468 6973 2065  tdir)..In this e
+000001d0: 7861 6d70 6c65 2c20 4920 6861 7665 206f  xample, I have o
+000001e0: 6e6c 7920 696d 706c 656d 656e 7465 6420  nly implemented 
+000001f0: 6465 6669 6e65 5f63 6f6d 706f 6e65 6e74  define_component
+00000200: 7328 2920 7768 6963 6820 6164 6473 0a61  s() which adds.a
+00000210: 2061 646d 696e 6973 7472 6174 696f 6e5f   administration_
+00000220: 6665 6573 2070 6172 616d 6574 6572 2074  fees parameter t
+00000230: 6f20 7468 6520 6d6f 6465 6c20 7468 6174  o the model that
+00000240: 2073 7065 6369 6669 6573 2061 2066 6978   specifies a fix
+00000250: 6564 0a61 6e6e 7561 6c20 636f 7374 206f  ed.annual cost o
+00000260: 6620 3120 6d69 6c6c 696f 6e20 646f 6c6c  f 1 million doll
+00000270: 6172 7320 616e 6420 7265 6769 7374 6572  ars and register
+00000280: 7320 7468 6973 2063 6f73 7420 7769 7468  s this cost with
+00000290: 2074 6865 0a6f 626a 6563 7469 7665 2066   the.objective f
+000002a0: 756e 6374 696f 6e2e 0a0a 5377 6974 6368  unction...Switch
+000002b0: 2069 7320 6c69 6365 6e73 6564 2075 6e64   is licensed und
+000002c0: 6572 2041 7061 6368 6520 4c69 6365 6e73  er Apache Licens
+000002d0: 6520 322e 3020 4d6f 7265 2069 6e66 6f20  e 2.0 More info 
+000002e0: 6174 2073 7769 7463 682d 0a6d 6f64 656c  at switch-.model
+000002f0: 2e6f 7267 0ae9 0000 0000 2901 da01 2a63  .org......)...*c
+00000300: 0100 0000 0000 0000 0000 0000 0500 0000  ................
+00000310: 0300 0000 f37e 0000 0097 0074 0100 0000  .....~.....t....
+00000320: 0000 0000 007c 006a 0200 0000 0000 0000  .....|.j........
+00000330: 0000 0000 0000 0000 0000 0064 0184 0074  ...........d...t
+00000340: 0400 0000 0000 0000 00ac 02ab 0300 0000  ................
+00000350: 0000 007c 005f 0300 0000 0000 0000 007c  ...|._.........|
+00000360: 006a 0800 0000 0000 0000 0000 0000 0000  .j..............
+00000370: 0000 0000 006a 0b00 0000 0000 0000 0000  .....j..........
+00000380: 0000 0000 0000 0000 0064 03ab 0100 0000  .........d......
+00000390: 0000 0001 0079 0029 044e 6302 0000 0000  .....y.).Nc.....
+000003a0: 0000 0000 0000 0000 0000 0013 0000 00f3  ................
+000003b0: 0400 0000 9700 7901 2902 4e69 4042 0f00  ......y.).Ni@B..
+000003c0: a900 2902 da01 6dda 0170 7302 0000 0020  ..)...m..ps.... 
+000003d0: 20fa 412f 7072 6976 6174 652f 746d 702f   .A/private/tmp/
+000003e0: 7477 696e 652f 7377 6974 6368 2f65 7861  twine/switch/exa
+000003f0: 6d70 6c65 732f 6375 7374 6f6d 5f65 7874  mples/custom_ext
+00000400: 656e 7369 6f6e 2f73 756e 6b5f 636f 7374  ension/sunk_cost
+00000410: 732e 7079 fa08 3c6c 616d 6264 613e 7a23  s.py..<lambda>z#
+00000420: 6465 6669 6e65 5f63 6f6d 706f 6e65 6e74  define_component
+00000430: 732e 3c6c 6f63 616c 733e 2e3c 6c61 6d62  s.<locals>.<lamb
+00000440: 6461 3e1f 0000 0073 0200 0000 8100 f300  da>....s........
+00000450: 0000 0029 02da 0a69 6e69 7469 616c 697a  ...)...initializ
+00000460: 65da 0677 6974 6869 6eda 1361 646d 696e  e..within..admin
+00000470: 6973 7472 6174 696f 6e5f 6665 6573 2906  istration_fees).
+00000480: da05 5061 7261 6dda 0750 4552 494f 4453  ..Param..PERIODS
+00000490: da03 416e 7972 0e00 0000 da1a 436f 7374  ..Anyr......Cost
+000004a0: 5f43 6f6d 706f 6e65 6e74 735f 5065 725f  _Components_Per_
+000004b0: 5065 7269 6f64 da06 6170 7065 6e64 2901  Period..append).
+000004c0: da03 6d6f 6473 0100 0000 2072 0900 0000  ..mods.... r....
+000004d0: da11 6465 6669 6e65 5f63 6f6d 706f 6e65  ..define_compone
+000004e0: 6e74 7372 1500 0000 1d00 0000 7332 0000  ntsr........s2..
+000004f0: 0080 00dc 1e23 d808 0b8f 0b89 0bd1 2034  .....#........ 4
+00000500: bc53 f403 021f 0680 43d4 041b f006 0005  .S......C.......
+00000510: 08d7 0422 d104 22d7 0429 d104 29d0 2a3f  ...".."..)..).*?
+00000520: d504 4072 0b00 0000 4e29 03da 075f 5f64  ..@r....N)...__d
+00000530: 6f63 5f5f da0d 7079 6f6d 6f2e 656e 7669  oc__..pyomo.envi
+00000540: 726f 6e72 1500 0000 7206 0000 0072 0b00  ronr....r....r..
+00000550: 0000 7209 0000 00fa 083c 6d6f 6475 6c65  ..r......<module
+00000560: 3e72 1800 0000 0100 0000 7315 0000 00f0  >r........s.....
+00000570: 0301 0101 f108 1401 04f4 2c00 011c f306  ..........,.....
+00000580: 0401 4101 720b 0000 00                   ..A.r....
```

### Comparing `switch_model-2.0.7/examples/custom_extension/inputs/gen_info.csv` & `switch_model-2.0.8/examples/custom_extension/inputs/gen_info.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/custom_extension/sunk_costs.py` & `switch_model-2.0.8/examples/custom_extension/sunk_costs.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/diagnose_infeasibility/README.md` & `switch_model-2.0.8/examples/diagnose_infeasibility/README.md`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/diagnose_infeasibility/inputs/gen_info.csv` & `switch_model-2.0.8/examples/diagnose_infeasibility/inputs/gen_info.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/discrete_and_min_build/inputs/gen_info.csv` & `switch_model-2.0.8/examples/discrete_and_min_build/inputs/gen_info.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/discrete_build/inputs/gen_info.csv` & `switch_model-2.0.8/examples/discrete_build/inputs/gen_info.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/dr_simple/inputs/gen_info.csv` & `switch_model-2.0.8/examples/dr_simple/inputs/gen_info.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/dr_simple/inputs/modules.txt` & `switch_model-2.0.8/examples/dr_simple/inputs/modules.txt`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/hydro_simple/README.md` & `switch_model-2.0.8/examples/hydro_simple/README.md`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/hydro_simple/inputs/gen_info.csv` & `switch_model-2.0.8/examples/hydro_simple/inputs/gen_info.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/hydro_system/README.md` & `switch_model-2.0.8/examples/hydro_system/README.md`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/hydro_system/inputs/gen_info.csv` & `switch_model-2.0.8/examples/hydro_system/inputs/gen_info.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/hydro_system/inputs/loads.csv` & `switch_model-2.0.8/examples/hydro_system/inputs/loads.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/hydro_system/inputs/timepoints.csv` & `switch_model-2.0.8/examples/hydro_system/inputs/timepoints.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/hydro_system/inputs/variable_capacity_factors.csv` & `switch_model-2.0.8/examples/hydro_system/inputs/variable_capacity_factors.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/hydro_system/inputs/water_node_tp_flows.csv` & `switch_model-2.0.8/examples/hydro_system/inputs/water_node_tp_flows.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/new_builds_only/inputs/gen_info.csv` & `switch_model-2.0.8/examples/new_builds_only/inputs/gen_info.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/planning_reserves/inputs/fuel_supply_curves.csv` & `switch_model-2.0.8/examples/planning_reserves/inputs/fuel_supply_curves.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/planning_reserves/inputs/gen_build_costs.csv` & `switch_model-2.0.8/examples/planning_reserves/inputs/gen_build_costs.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/planning_reserves/inputs/gen_info.csv` & `switch_model-2.0.8/examples/planning_reserves/inputs/gen_info.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/planning_reserves/inputs/reserve_capacity_value.csv` & `switch_model-2.0.8/examples/planning_reserves/inputs/reserve_capacity_value.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/planning_reserves/inputs/variable_capacity_factors.csv` & `switch_model-2.0.8/examples/planning_reserves/inputs/variable_capacity_factors.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/production_cost_models/3plants/inputs/gen_info.csv` & `switch_model-2.0.8/examples/production_cost_models/3plants/inputs/gen_info.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/production_cost_models/4plants/inputs/gen_info.csv` & `switch_model-2.0.8/examples/production_cost_models/4plants/inputs/gen_info.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/production_cost_models/4plants_with_unserved_load/inputs/gen_info.csv` & `switch_model-2.0.8/examples/production_cost_models/4plants_with_unserved_load/inputs/gen_info.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/production_cost_models/discrete_unit_commit/inputs/gen_info.csv` & `switch_model-2.0.8/examples/production_cost_models/discrete_unit_commit/inputs/gen_info.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/production_cost_models/spinning_reserves/inputs/gen_info.csv` & `switch_model-2.0.8/examples/production_cost_models/spinning_reserves/inputs/gen_info.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/production_cost_models/spinning_reserves/inputs/modules.txt` & `switch_model-2.0.8/examples/production_cost_models/spinning_reserves/inputs/modules.txt`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/production_cost_models/spinning_reserves_advanced/inputs/gen_info.csv` & `switch_model-2.0.8/examples/production_cost_models/spinning_reserves_advanced/inputs/gen_info.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/production_cost_models/spinning_reserves_advanced/inputs/modules.txt` & `switch_model-2.0.8/examples/production_cost_models/spinning_reserves_advanced/inputs/modules.txt`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/production_cost_models/unit_commit/README.md` & `switch_model-2.0.8/examples/production_cost_models/unit_commit/README.md`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/production_cost_models/unit_commit/inputs/gen_info.csv` & `switch_model-2.0.8/examples/production_cost_models/unit_commit/inputs/gen_info.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/rps_simple/README.md` & `switch_model-2.0.8/examples/rps_simple/README.md`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/rps_simple/inputs/fuel_supply_curves.csv` & `switch_model-2.0.8/examples/rps_simple/inputs/fuel_supply_curves.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/rps_simple/inputs/gen_build_costs.csv` & `switch_model-2.0.8/examples/rps_simple/inputs/gen_build_costs.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/rps_simple/inputs/gen_info.csv` & `switch_model-2.0.8/examples/rps_simple/inputs/gen_info.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/rps_simple/inputs/variable_capacity_factors.csv` & `switch_model-2.0.8/examples/retrofits/inputs/variable_capacity_factors.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/examples/storage/inputs/gen_info.csv` & `switch_model-2.0.8/examples/storage/inputs/gen_info.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/how_to_collaborate.txt` & `switch_model-2.0.8/how_to_collaborate.txt`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/run_tests.py` & `switch_model-2.0.8/run_tests.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/setup.py` & `switch_model-2.0.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -63,39 +63,36 @@
         "energy",
         "electricity",
         "production cost",
         "capacity expansion",
         "planning",
         "optimization",
     ],
-    # Pyomo <=6.4.2 crashes on Python 3.11, so we rule that out until they
-    # resolve it
-    python_requires=">=3.7.0, <3.11.0a0",
+    # We pin the upper limit for Pyomo and Python because there have been cases
+    # where Pyomo introduced non-backward compatible changes or started crashing
+    # with a new version of Python (e.g., Pyomo <=6.4.2 crashed on Python 3.11).
+    # There's still some chance users will end up with an incompatible mix with
+    # these or with other packages (e.g., newer versions of testfixtures don't
+    # work on older versions of Python without adding mock, and testfixtures
+    # 6.3.0 fails on Python >= 3.10), but we don't have an easy way to identify
+    # compatible mixes and we don't want to be overly restrictive.
+    # Note: testfixtures requires a separate mock installation if running with
+    # Python 3.7.0 or 3.7.1, so we require a higher version to avoid this. (Newer
+    # versions of Pyomo need 3.8+ anyway.)
+    python_requires=">=3.7.2, <3.13.0a0",
     install_requires=[
-        # Most of our code is compatible with Pyomo 5.5.1+, but Pyomo <=5.6.8
-        # has a bug that makes it fail to report when values are out of domain
-        # for a parameter. So we must require a later version than 5.6.8, which
-        # was the highest version we previously supported, so all users will
-        # need to upgrade their Pyomo version.
-        # In principle, we could accept Pyomo 5.6.9 with pyutilib 5.8.0 (works
-        # OK in testing), but we block that because Pyomo 5.6.9 says it's
-        # willing to work with pyutilib 6.0.0, but isn't actually compatible.
-        # We have to allow pyutilib 6.0.0 for the later versions of Pyomo and
-        # setuptools doesn't give us a way to say Pyomo 5.6.9 should only be
-        # installed with pyutilib 5.8.0, so we just block Pyomo 5.6.9.
-        "Pyomo >=5.7.0, <=6.4.2",
-        # Pyomo 5.7 specifies that it needs pyutilib >=6.0.0. We've seen cases
-        # cases where Pyomo released a later pyutilib that broke an earlier
-        # Pyomo (e.g., Pyomo 5.6.x with Pyutilib 6.0.0), so we had to
-        # retroactively pin the pyutilib version. Pyomo 6.0 phased out the
-        # pyutilib dependency, but we still pin at 6.0.0, just in case the user
-        # installs Pyomo 5.7 and Pyutilib releases an incompatible update.
-        "pyutilib ==6.0.0",
-        # pint is needed by Pyomo when running our tests, but isn't installed by
-        # Pyomo.
+        # In principle, we could accept Pyomo 5.6.9, but it tends to install
+        # a non-compatible version of pyutilib (needs 5.8.0 but accepts 6.0.0
+        # and then breaks). On the other hand, Pyomo 5.7 requires pyutilib 6.0.0
+        # and Pyomo 6.0 doesn't require pyutilib at all. So we now use Pyomo 6.0+
+        # and skip pyutilib.
+        "Pyomo >=6.0.0, <=6.7.1",
+        # pint is needed by Pyomo 6.4.1, 6.7.1 and probably others (but not
+        # 6.0.0) when running our tests. But it isn't listed as a Pyomo
+        # dependency, so we add it explicitly. (Still true as of Pyomo 6.7.1).
         "pint",
         # used for standard tests
         "testfixtures",
         # used for input upgrades and some reporting
         "pandas",
     ],
     extras_require={
@@ -104,18 +101,18 @@
             "numpy",
             "scipy",
             "rpy2",
             "sympy",
         ],
         "dev": ["ipdb"],
         "plotting": [
-            # plotnine before <= 0.9.0 is not compatible with matplotlib >= 3.6
-            # later versions of plotnine may be, but for now we require that
-            # matplotlib be below 3.6.0 to ensure compatibility.
-            # See https://stackoverflow.com/a/73797154/
-            "plotnine<=0.9.0",
-            "matplotlib<3.6.0a0",
+            # We have previously had to work around incompatibilities between
+            # different versions of plotnine and matplotlib
+            # (https://stackoverflow.com/a/73797154/) but they seem to be
+            # resolved now.
+            "plotnine",
+            "matplotlib",
         ],
         "database_access": ["psycopg2-binary"],
     },
     entry_points={"console_scripts": ["switch = switch_model.main:main"]},
 )
```

### Comparing `switch_model-2.0.7/switch_model/__init__.py` & `switch_model-2.0.8/switch_model/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/balancing/demand_response/iterative/__init__.py` & `switch_model-2.0.8/switch_model/balancing/demand_response/iterative/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 model at a time. An alternative approach would be to receive a calibration_data
 object back from demand_module.calibrate(), then add that to the model and pass
 it back to the bid function when needed.
 
 note: we also take advantage of this assumption and store a reference to the
 current demand_module in this module (rather than storing it in the model itself)
 """
+
 from __future__ import print_function
 from __future__ import division
 
 # TODO: create a new module to handle total-cost pricing.
 # That should apply a simple tax to every retail kWh sold (zone_demand_mw or FlexibleDemand)
 # (this is a fixed adder to the cost in $/kWh, not a multiplier times the marginal cost)
 # that module can be used as-is to find the effect of any particular adder
@@ -62,15 +63,14 @@
         help="Type(s) of reserves to provide from demand response (e.g., 'contingency' or 'regulation'). "
         "Specify 'none' to disable. Default is 'spinning' if an operating reserve module is used, "
         "otherwise it is 'none'.",
     )
 
 
 def define_components(m):
-
     # load scipy.optimize; this is done here to avoid loading it during unit tests
     try:
         global scipy
         import scipy.optimize
     except ImportError:
         print("=" * 80)
         print(
@@ -189,17 +189,19 @@
     #         print "constructing DR_Convex_Bid_Weight constraint"
     #         return (sum(m.DRBidWeight[b, z, ts] for b in m.DR_BID_LIST) == 1)
     #
     # choose a convex combination of bids for each zone and timeseries
     m.DR_Convex_Bid_Weight = Constraint(
         m.LOAD_ZONES,
         m.TIMESERIES,
-        rule=lambda m, z, ts: Constraint.Skip
-        if len(m.DR_BID_LIST) == 0
-        else (sum(m.DRBidWeight[b, z, ts] for b in m.DR_BID_LIST) == 1),
+        rule=lambda m, z, ts: (
+            Constraint.Skip
+            if len(m.DR_BID_LIST) == 0
+            else (sum(m.DRBidWeight[b, z, ts] for b in m.DR_BID_LIST) == 1)
+        ),
     )
 
     # Since we don't have differentiated prices for each zone, we have to use the same
     # weights for all zones. (Otherwise the model will try to micromanage load in each
     # zone, but that won't be reflected in the prices we report.)
     # Note: LOAD_ZONES is not an ordered set, so we have to use a trick to get a single
     # arbitrary one to refer to (list(m.LOAD_ZONES)[0] would also work).
@@ -275,26 +277,29 @@
     # m.Zone_Power_Withdrawals.append('FlexibleDemand')
     idx = m.Zone_Power_Withdrawals.index("zone_demand_mw")
     m.Zone_Power_Withdrawals[idx] = "FlexibleDemand"
 
     # private benefit of the electricity consumption
     # (i.e., willingness to pay for the current electricity supply)
     # reported as negative cost, i.e., positive benefit
-    # also divide by number of timepoints in the timeseries
-    # to convert from a cost per timeseries to a cost per timepoint.
+    # also divide by duration of the timeseries
+    # to convert from a cost per timeseries to a cost per hour,
+    # which can be reported per timepoint.
+    # TODO: this assumes wtp per timeseries accounts for duration of timepoints
+    # but the weighting in the convergence test may not, and the bidding module
+    # may not (e.g., it may just take a sum across timepoints, which would have
+    # units of $/MWh * ts_num_tps, not $/timeseries)
     m.DR_Welfare_Cost = Expression(
         m.TIMEPOINTS,
-        rule=lambda m, tp: (-1.0)
-        * sum(
-            m.DRBidWeight[b, z, m.tp_ts[tp]] * m.dr_bid_benefit[b, z, m.tp_ts[tp]]
+        rule=lambda m, tp: sum(
+            -m.DRBidWeight[b, z, m.tp_ts[tp]] * m.dr_bid_benefit[b, z, m.tp_ts[tp]]
             for b in m.DR_BID_LIST
             for z in m.LOAD_ZONES
         )
-        * m.tp_duration_hrs[tp]
-        / m.ts_num_tps[m.tp_ts[tp]],
+        / m.ts_duration_hrs[m.tp_ts[tp]],
     )
 
     # add the private benefit to the model's objective function
     m.Cost_Components_Per_TP.append("DR_Welfare_Cost")
 
     # variable to store the baseline data
     m.base_data = None
@@ -465,14 +470,20 @@
                 for tp in m.TPS_IN_TS[ts]
             )
         )
         best_bid_benefit = value(
             sum(
                 (
                     -sum(m.dr_bid_benefit[b, z, ts] for z in m.LOAD_ZONES)
+                    # TODO: clarify whether bids should return total benefit
+                    # per timeseries, which must consider duration of timepoints
+                    # or just benefit per hour * number of timepoints (weird, but
+                    # probably what they do), since the bidding module probably
+                    # just looks at $/MWh marginal costs and treats them as
+                    # $/MW/timepoint
                     * m.tp_duration_hrs[tp]
                     / m.ts_num_tps[ts]
                 )
                 * m.bring_timepoint_costs_to_base_year[tp]
                 for ts in m.TIMESERIES
                 for tp in m.TPS_IN_TS[ts]
             )
@@ -869,15 +880,15 @@
     for z in m.LOAD_ZONES:
         for ts in m.TIMESERIES:
             demand, wtp = demand_module.bid(m, z, ts, prices[z, ts])
             # import pdb; pdb.set_trace()
             if m.options.dr_flat_pricing:
                 # assume demand side will not provide reserves, even if they offered some
                 # (at zero price)
-                for (k, v) in demand.items():
+                for k, v in demand.items():
                     if k != "energy":
                         for i in range(len(v)):
                             v[i] = 0.0
             bids.append((z, ts, prices[z, ts], demand, wtp))
 
     return bids
 
@@ -955,15 +966,16 @@
         for ts in m.TS_IN_PERIOD[p]
     }
     return final_prices
 
 
 def revenue_imbalance(flat_price, m, load_zone, period, dynamic_prices):
     """find demand and revenue that would occur in this load_zone and period with flat prices, and
-    compare to the cost of meeting that demand by purchasing power at the current dynamic prices"""
+    compare to the cost of meeting that demand by purchasing power at the current dynamic prices
+    """
     flat_price_revenue = 0.0
     dynamic_price_revenue = 0.0
     for ts in m.TS_IN_PERIOD[period]:
         prices = {
             prod: [flat_price if prod == "energy" else 0.0] * len(m.TPS_IN_TS[ts])
             for prod in m.DR_PRODUCTS
         }
@@ -1005,15 +1017,15 @@
         b = 1
     else:
         b = max(m.DR_BID_LIST) + 1
 
     m.DR_BID_LIST.add(b)
 
     # add the bids for each load zone and timepoint to the dr_bid list
-    for (z, ts, prices, demand, wtp) in bids:
+    for z, ts, prices, demand, wtp in bids:
         # record the private benefit
         m.dr_bid_benefit[b, z, ts] = wtp
         # record the level of demand for each timepoint
         for prod in m.DR_PRODUCTS:
             for i, tp in enumerate(m.TPS_IN_TS[ts]):
                 m.dr_bid[b, z, tp, prod] = demand[prod][i]
                 m.dr_price[b, z, tp, prod] = prices[prod][i]
@@ -1342,17 +1354,19 @@
         + tuple(getattr(m, component)[z, t] for component in m.Zone_Power_Withdrawals)
         + tuple(m.dr_price[last_bid, z, t, prod] for prod in m.DR_PRODUCTS)
         + tuple(m.dr_bid[last_bid, z, t, prod] for prod in m.DR_PRODUCTS)
         + tuple(electricity_marginal_cost(m, z, t, prod) for prod in m.DR_PRODUCTS)
         + tuple(final_prices[z, t, prod] for prod in m.DR_PRODUCTS)
         + tuple(final_quantities[z, t, prod] for prod in m.DR_PRODUCTS)
         + (
-            "peak"
-            if m.ts_scale_to_year[m.tp_ts[t]] < 0.5 * avg_ts_scale
-            else "typical",
+            (
+                "peak"
+                if m.ts_scale_to_year[m.tp_ts[t]] < 0.5 * avg_ts_scale
+                else "typical"
+            ),
             m.base_data_dict[z, t][0],
             m.base_data_dict[z, t][1],
         ),
     )
 
     # import pprint
     # b=[(g, pe, value(m.BuildGen[g, pe]), m.gen_tech[g], m.gen_overnight_cost[g, pe]) for (g, pe) in m.BuildGen if value(m.BuildGen[g, pe]) > 0]
```

### Comparing `switch_model-2.0.7/switch_model/balancing/demand_response/iterative/constant_elasticity_demand_system.py` & `switch_model-2.0.8/switch_model/balancing/demand_response/iterative/constant_elasticity_demand_system.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import division
 
 
-def calibrate(base_data, dr_elasticity_scenario=3):
+def calibrate(m, base_data, dr_elasticity_scenario=3):
     """Accept a list of tuples showing [base hourly loads], and [base hourly prices] for each
     location (load_zone) and date (time_series). Store these for later reference by bid().
     """
     # import numpy; we delay till here to avoid interfering with unit tests
     global np
     import numpy as np
 
@@ -19,22 +19,23 @@
     base_price_dict = {
         (z, ts): np.array(base_prices, float)
         for (z, ts, base_loads, base_prices) in base_data
     }
     elasticity_scenario = dr_elasticity_scenario
 
 
-def bid(load_zone, time_series, prices):
+def bid(m, load_zone, time_series, prices):
     """Accept a vector of current prices, for a particular location (load_zone) and day (time_series).
     Return a tuple showing hourly load levels and willingness to pay for those loads (relative to the
     loads achieved at the base_price).
 
     This version assumes that part of the load is price elastic with constant elasticity of 0.1 and no
     substitution between hours (this part is called "elastic load" below), and the rest of the load is inelastic
-    in total volume, but schedules itself to the cheapest hours (this part is called "shiftable load")."""
+    in total volume, but schedules itself to the cheapest hours (this part is called "shiftable load").
+    """
 
     elasticity = 0.1
     shiftable_share = 0.1 * elasticity_scenario  # 1-3
 
     # convert prices to a numpy vector, and make non-zero
     # to avoid errors when raising to a negative power
     p = np.maximum(1.0, np.array(prices, float))
```

### Comparing `switch_model-2.0.7/switch_model/balancing/demand_response/iterative/r_demand_system.py` & `switch_model-2.0.8/switch_model/balancing/demand_response/iterative/r_demand_system.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/balancing/demand_response/simple.py` & `switch_model-2.0.8/switch_model/balancing/demand_response/simple.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 # Copyright (c) 2015-2022 The Switch Authors. All rights reserved.
 # Licensed under the Apache License, Version 2, which is in the LICENSE file.
 
 """
 Defines a simple Demand Response Shift Service for the Switch model.
 Load in a certain load zone may be shifted between timepoints belonging to the
-same timeseries at no cost, which allows assessing the potential value of
+same date at no cost, which allows assessing the potential value of
 demand shifting. This does not include a Shed Service (curtailment of load),
 nor a Shimmy Service (fast dispatch for load following or regulation).
 
 """
 
 import os
 from pyomo.environ import *
 
 dependencies = "switch_model.timescales", "switch_model.balancing.load_zones"
 optional_dependencies = "switch_model.transmission.local_td"
 
 
 def define_components(mod):
-
     """
     Adds components to a Pyomo abstract model object to describe a demand
     response shift service.
 
     dr_shift_down_limit[(z,t in ZONE_TIMEPOINTS)] is a parameter
     that describes the maximum reduction in demand for load-shifting demand
     response (in MW) that is allowed in a load zone at a specific timepoint.
@@ -39,17 +38,21 @@
     and dr_shift_up_limit.
 
     If the local_td module is included, ShiftDemand[z,t] will be registered
     with local_td's distributed node for energy balancing purposes. If
     local_td is not included, it will be registered with load zone's central
     node and will not reflect efficiency losses in the distribution network.
 
-    DR_Shift_Net_Zero[z,ts in TIMESERIES] is a constraint that forces all the
-    changes in the demand to balance out over the course of each timeseries.
+    DR_Shift_Net_Zero[z, d in DATES] is a constraint that forces all the
+    changes in the demand to balance out over the course of each date.
 
+    When using multi-day timeseries (e.g., weeks or years), you should provide
+    tp_date values in timepoints.csv to identify which timepoints fall on the
+    same date. Otherwise, load will be shifted freely to any other part of the
+    same timeseries (possibly months away).
     """
 
     mod.dr_shift_down_limit = Param(
         mod.LOAD_ZONES,
         mod.TIMEPOINTS,
         default=0.0,
         within=NonNegativeReals,
@@ -66,16 +69,16 @@
             (-1.0) * m.dr_shift_down_limit[z, t],
             m.dr_shift_up_limit[z, t],
         ),
     )
 
     mod.DR_Shift_Net_Zero = Constraint(
         mod.LOAD_ZONES,
-        mod.TIMESERIES,
-        rule=lambda m, z, ts: sum(m.ShiftDemand[z, t] for t in m.TPS_IN_TS[ts]) == 0.0,
+        mod.DATES,
+        rule=lambda m, z, d: sum(m.ShiftDemand[z, t] for t in m.TPS_IN_DATE[d]) == 0.0,
     )
 
     try:
         mod.Distributed_Power_Withdrawals.append("ShiftDemand")
     except AttributeError:
         mod.Zone_Power_Withdrawals.append("ShiftDemand")
```

### Comparing `switch_model-2.0.7/switch_model/balancing/diagnose_infeasibility.py` & `switch_model-2.0.8/switch_model/balancing/diagnose_infeasibility.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """
 Relax constraints to help diagnose data problems in infeasible models
 
 This module adds relaxation terms to all constraints in the model, which makes
 every model feasible. It then minimizes the simple sum of the relaxation
 variables (i.e., total violation of all constraints) instead of the normal cost
-function. Then it report which constraints were violated and by how much. 
+function. Then it report which constraints were violated and by how much.
 
 Users can experiment by specifying `--no-relax` for some constraints, to find
 out which constraints cannot be met on their own or cannot be met in combination
 with other constraints (e.g., if specifying `--no-relax Constraint1` causes
 `Constraint2` to be violated instead, then we know these are related. Then if
 the model becomes infeasible when specifying `--no-relax Constraint1
 Constraint2`, we know that Constraint1 and Constraint2 cannot be satisfied at
 the same time. Users should then look for inconsistencies in the data used for
 these two constraints.
 """
+
 from switch_model.utilities import make_iterable
 import pyomo.environ as pyo
 
 relax_var_prefix = "Relax"
 relax_var_dir = {1: "up", -1: "down"}
 
 # TODO: look for a way to do all this from the pre_solve() step and in a more
@@ -94,40 +95,45 @@
         constraint_name = constraint.name
         for key, c in constraint.items():
             for direction in [-1, 1]:
                 # get the matching relaxation variable
                 relax_var = getattr(m, relax_var_name(constraint, direction))
                 val = relax_var[key].value
                 if val is not None and val >= 1e-9:
-                    # We could use name = c.name here, but for it is slow to
+                    # We could use name = c.name here, but it is slow to
                     # access constraints later in the model (see
                     # https://github.com/Pyomo/pyomo/issues/2560). Using repr()
-                    # also gives a more copy-pastable representation of the
-                    # constraint, which can be useful for debugging.
+                    # or str() on a list also gives a more copy-pastable
+                    # representation of the constraint, which can be useful for
+                    # debugging.
                     name = constraint_name
                     if key is not None:
-                        name += repr(list(key))
+                        name += repr(list(make_iterable(key)))
                     unsatisfied_constraints.append([name, direction * val])
 
     # We report results using logger.info, so users must set log-level to
     # info to see them. This is because these are diagnostic messages, not
     # errors, and because it prevents chatter from the test suite.
     if unsatisfied_constraints:
         for name, val in unsatisfied_constraints:
-            m.logger.info(
-                "WARNING: Constraint {} violated by {:.4g} units.".format(name, val)
-            )
+            m.logger.info("")
+            m.logger.info(f"WARNING: Constraint {name} violated by {val:.4g} units.")
     else:
         m.logger.info(
-            "\nCongratulations, the model is feasible. Please solve again "
-            "without using the {} module to obtain the optimal solution.\n".format(
-                __name__
-            )
+            "\nCongratulations, the model is feasible. To obtain the optimal\n"
+            f"solution, please solve again without using the {__name__} module."
         )
 
+    m.logger.info(
+        f"\nNOTE: Module {__name__} was used for this run.\n"
+        "This seeks only to minimize violations of constraints, and does not minimize\n"
+        "costs. All results from this run (other than constraint violations) should be\n"
+        "ignored.\n"
+    )
+
 
 def relax_var_name(constraint, direction):
     return "_".join(
         [
             relax_var_prefix,
             constraint.name,
             relax_var_dir[direction],
@@ -138,14 +144,17 @@
 def relax_constraint(c):
     def new_rule(m, *idx):
         # note: we use getattr(m, c.name) instead of just c, because
         # c is an object in the AbstractModel and this rule will be called on
         # a concrete instance.
         expr = getattr(m, c.name).original_rule(m, *idx)
         if expr is not pyo.Constraint.Skip and expr is not pyo.Constraint.Infeasible:
+            if isinstance(expr, tuple):
+                # constraint of type (lb, expr, up)
+                expr = expr[1]
             # pyomo provides a .args argument but it is not editable.
             # some versions provide ._args and some provide ._args_, so we use
             # what is available
             a = "_args" if hasattr(expr, "_args") else "_args_"
             args = list(getattr(expr, a))  # make mutable
             # add up and down relaxation vars to an arbitrary point in the
             # inequality (usually works out as high side)
```

### Comparing `switch_model-2.0.7/switch_model/balancing/load_zones.py` & `switch_model-2.0.8/switch_model/balancing/load_zones.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/balancing/operating_reserves/areas.py` & `switch_model-2.0.8/switch_model/balancing/operating_reserves/areas.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/balancing/operating_reserves/spinning_reserves.py` & `switch_model-2.0.8/switch_model/balancing/operating_reserves/spinning_reserves.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/balancing/operating_reserves/spinning_reserves_advanced.py` & `switch_model-2.0.8/switch_model/balancing/operating_reserves/spinning_reserves_advanced.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/balancing/planning_reserves.py` & `switch_model-2.0.8/switch_model/balancing/planning_reserves.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/balancing/unserved_load.py` & `switch_model-2.0.8/switch_model/balancing/unserved_load.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/energy_sources/fuel_costs/markets.py` & `switch_model-2.0.8/switch_model/energy_sources/fuel_costs/markets.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,15 +220,15 @@
     )
     mod.ZONE_FUELS = Set(
         dimen=2, initialize=lambda m: [(z, m.rfm_fuel[rfm]) for (z, rfm) in m.ZONE_RFMS]
     )
 
     def zone_fuel_rfm_init(m, load_zone, fuel):
         # find first (only) matching rfm
-        for (z, rfm) in m.ZONE_RFMS:
+        for z, rfm in m.ZONE_RFMS:
             if z == load_zone and fuel == m.rfm_fuel[rfm]:
                 return rfm
 
     mod.zone_fuel_rfm = Param(
         mod.ZONE_FUELS, within=mod.REGIONAL_FUEL_MARKETS, initialize=zone_fuel_rfm_init
     )
     mod.min_data_check("REGIONAL_FUEL_MARKETS", "rfm_fuel", "zone_fuel_rfm")
@@ -478,68 +478,53 @@
         _load_simple_cost_data(mod, switch_data, path)
 
 
 def _load_simple_cost_data(mod, switch_data, path):
     with open(path, "r") as simple_cost_file:
         simple_cost_dat = list(csv.DictReader(simple_cost_file, delimiter=","))
         # Scan once for error checking
+        fname = os.path.basename(path)
         for row in simple_cost_dat:
             z = row["load_zone"]
             f = row["fuel"]
             p = int(row["period"])
             f_cost = float(row["fuel_cost"])
             # Basic data validity checks
             if z not in switch_data.data(name="LOAD_ZONES"):
                 raise ValueError(
-                    "Load zone "
-                    + z
-                    + " in zone_simple_fuel_cost.csv is not "
-                    + "a known load zone from load_zones.csv."
+                    f"Load zone {z} in {fname} is not "
+                    f"a known load zone from load_zones.csv."
                 )
             if f not in switch_data.data(name="FUELS"):
                 raise ValueError(
-                    "Fuel "
-                    + f
-                    + " in zone_simple_fuel_cost.csv is not "
-                    + "a known fuel from fuels.csv."
+                    f"Fuel {f} in {fname} is not a known fuel from fuels.csv."
                 )
             if p not in switch_data.data(name="PERIODS"):
                 raise ValueError(
-                    "Period "
-                    + p
-                    + " in zone_simple_fuel_cost.csv is not "
-                    + "a known investment period."
+                    f"Period {p} in {fname} is not a known investment period."
                 )
             # Make sure they aren't overriding a supply curve or
             # regional fuel market defined in previous files.
-            for (z, rfm) in switch_data.data(name="ZONE_RFMS"):
+            for z, rfm in switch_data.data(name="ZONE_RFMS"):
                 if z == z and switch_data.data(name="rfm_fuel")[rfm] == f:
                     raise ValueError(
-                        "The supply for fuel '"
-                        + f
-                        + "' for load_zone '"
-                        + z
-                        + "' was already registered with the regional fuel "
-                        + "market '"
-                        + rfm
-                        + "', so you cannot "
-                        + "specify a simple fuel cost for it in "
-                        + "zone_simple_fuel_cost.csv. You either need to delete "
-                        + "that entry from zone_to_regional_fuel_market.csv, or "
-                        + "remove those entries in zone_simple_fuel_cost.csv."
+                        f"The supply for fuel '{f}' for load_zone '{z}' was "
+                        f"already registered with the regional fuel market "
+                        f"'{rfm}', so you cannot specify a simple fuel cost for "
+                        f"it in {fname}. You either need to delete that entry "
+                        f"from zone_to_regional_fuel_market.csv, or remove those "
+                        f"entries in {fname}."
                     )
             # Make a new single-load zone regional fuel market.
             rfm = z + "_" + f
             if rfm in switch_data.data(name="REGIONAL_FUEL_MARKETS"):
                 raise ValueError(
-                    "Trying to construct a simple Regional Fuel Market "
-                    + "called "
-                    + rfm
-                    + " from data in zone_simple_fuel_cost.csv"
-                    + ", but an RFM of that name already exists. Bailing out!"
+                    f"Trying to construct a simple Regional Fuel Market called "
+                    f"{rfm} from data in {fname}, but an RFM of that name already "
+                    f"exists. Bailing out!"
                 )
         # Scan again and actually import the data
         for row in simple_cost_dat:
             z = row["load_zone"]
             f = row["fuel"]
             p = int(row["period"])
             f_cost = float(row["fuel_cost"])
```

### Comparing `switch_model-2.0.7/switch_model/energy_sources/fuel_costs/markets_expansion.py` & `switch_model-2.0.8/switch_model/energy_sources/fuel_costs/markets_expansion.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/energy_sources/fuel_costs/simple.py` & `switch_model-2.0.8/switch_model/energy_sources/fuel_costs/simple.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/energy_sources/fuel_costs/simple_per_timepoint.py` & `switch_model-2.0.8/switch_model/energy_sources/fuel_costs/simple_per_timepoint.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/energy_sources/properties.py` & `switch_model-2.0.8/switch_model/energy_sources/properties.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/financials.py` & `switch_model-2.0.8/switch_model/financials.py`

 * *Files 6% similar despite different names*

```diff
@@ -223,54 +223,59 @@
 
     mod.base_financial_year = Param(within=NonNegativeReals)
     mod.interest_rate = Param(within=NonNegativeReals)
     mod.discount_rate = Param(
         within=NonNegativeReals, default=lambda m: value(m.interest_rate)
     )
     mod.min_data_check("base_financial_year", "interest_rate")
+    mod.bring_future_costs_to_base_year = Param(
+        mod.PERIODS,
+        within=NonNegativeReals,
+        initialize=lambda m, p: future_to_present_value(
+            m.discount_rate, m.period_start[p] - m.base_financial_year
+        ),
+    )
     mod.bring_annual_costs_to_base_year = Param(
         mod.PERIODS,
         within=NonNegativeReals,
         initialize=lambda m, p: (
             uniform_series_to_present_value(m.discount_rate, m.period_length_years[p])
-            * future_to_present_value(
-                m.discount_rate, m.period_start[p] - m.base_financial_year
-            )
+            * m.bring_future_costs_to_base_year[p]
         ),
     )
     mod.bring_timepoint_costs_to_base_year = Param(
         mod.TIMEPOINTS,
         within=NonNegativeReals,
         initialize=lambda m, t: (
             m.bring_annual_costs_to_base_year[m.tp_period[t]] * m.tp_weight_in_year[t]
         ),
     )
 
 
 def define_dynamic_components(mod):
     """
 
-    Adds components to a Pyomo abstract model object to summarize net
-    present value of all system costs. Other modules will register cost
-    components into dynamic lists that are used here to calculate total
-    system costs. This function is called after define_components() so
-    that other modules have a chance to add entries to the dynamic
-    lists.
-
-    Unless otherwise stated, all terms describing power are in units of
-    MW and all terms describing energy are in units of MWh. Future costs
-    (both hourly and annual) are in real dollars relative to the
-    base_year and are converted to net present value in the base year
-    within this module.
+    Adds components to a Pyomo abstract model object to summarize net present
+    value of all system costs. Other modules will register cost components into
+    dynamic lists that are used here to calculate total system costs. This
+    function is called after define_components() so that other modules have a
+    chance to add entries to the dynamic lists.
+
+    Unless otherwise stated, all terms describing power are in units of MW and
+    all terms describing energy are in units of MWh. Future costs (both hourly
+    and annual) are in real dollars relative to the base_year and are converted
+    to net present value in the base year within this module.
 
-    SystemCostPerPeriod[p in PERIODS] is an expression that sums
-    total system costs in each period based on the two lists
+    SystemCostPerPeriod[p in PERIODS] is an expression that sums total system
+    costs in each period on a discounted basis, based on the two lists
     Cost_Components_Per_TP and Cost_Components_Per_Period. Components in the
-    first list are indexed by timepoint and components in the second are
-    indexed by period.
+    first list are indexed by timepoint and components in the second are indexed
+    by period. Components in the _Per_TP list should have costs given in $/hour
+    (not $/timepoint) and components in the _Per_Period list should have costs
+    given in $/year (not $/period).
 
     Minimize_System_Cost is the objective function that seeks to minimize
     TotalSystemCost.
 
     """
 
     def calc_tp_costs_in_period(m, t):
@@ -291,17 +296,16 @@
     def calc_sys_costs_per_period(m, p):
         return (
             # All annual payments in the period
             (
                 calc_annual_costs_in_period(m, p)
                 + sum(calc_tp_costs_in_period(m, t) for t in m.TPS_IN_PERIOD[p])
             )
-            *
             # Conversion from annual costs to base year
-            m.bring_annual_costs_to_base_year[p]
+            * m.bring_annual_costs_to_base_year[p]
         )
 
     mod.SystemCostPerPeriod = Expression(mod.PERIODS, rule=calc_sys_costs_per_period)
     # starting with Pyomo 4.2, it is impossible to call Objective.reconstruct()
     # or calculate terms like Objective / <some other model component>,
     # so it's best to define a separate expression and use that for these purposes.
     mod.SystemCost = Expression(
@@ -324,47 +328,64 @@
         param=(mod.base_financial_year, mod.interest_rate, mod.discount_rate),
     )
 
 
 def post_solve(instance, outdir):
     m = instance
     # Overall electricity costs, if appropriate (some models may be gas-only)
+
+    # Note: through (and including) v. 2.0.7, SystemCostPerPeriod_Real was
+    # a (mislabeled) annual cost but SystemDemand_MWh was a total for the period
+    # so EnergyCostReal_per_MWh was low by the number of years in the period.
+
+    # Starting with 2.0.8, we report both costs and quantities per year to avoid
+    # this problem.
+
     if hasattr(m, "zone_total_demand_in_period_mwh"):
         normalized_dat = [
             {
                 "PERIOD": p,
-                "SystemCostPerPeriod_NPV": value(m.SystemCostPerPeriod[p]),
-                "SystemCostPerPeriod_Real": value(
-                    m.SystemCostPerPeriod[p] / m.bring_annual_costs_to_base_year[p]
-                ),
-                "EnergyCostReal_per_MWh": value(
+                "SystemCostPerYear_Real": value(
+                    # dividing SystemCostPerPeriod[p] by m.bring_annual_costs_to_base_year[p]
+                    # undoes the conversion from real $/year to NPV $/period, so
+                    # this expression is a cost per year in period p
                     m.SystemCostPerPeriod[p]
                     / m.bring_annual_costs_to_base_year[p]
-                    / sum(m.zone_total_demand_in_period_mwh[z, p] for z in m.LOAD_ZONES)
                 ),
-                "SystemDemand_MWh": value(
+                "SystemDemandPerYear_MWh": value(
+                    # zone_total_demand_in_period_mwh is a total value for the period,
+                    # so must be divided by the length of the period to get MWh/year
                     sum(m.zone_total_demand_in_period_mwh[z, p] for z in m.LOAD_ZONES)
+                    / m.period_length_years[p]
                 ),
             }
             for p in m.PERIODS
         ]
-        df = pd.DataFrame(normalized_dat)
-        df.set_index(["PERIOD"], inplace=True)
+        df = pd.DataFrame(normalized_dat).set_index("PERIOD")
+        df["EnergyCostReal_per_MWh"] = (
+            df["SystemCostPerYear_Real"] / df["SystemDemandPerYear_MWh"]
+        )
         if instance.options.sorted_output:
             df.sort_index(inplace=True)
         df.to_csv(os.path.join(outdir, "electricity_cost.csv"))
 
     # Itemized annual costs
+    # Note: through v. 2.0.7, AnnualCost_NPV was actually a period cost
+    # TODO: decide whether to report these costs as total NPV values for each period
+    # for model review and diagnosis (should add up to objective function) or
+    # as annual costs for analysis and reporting. Maybe they should be in two
+    # separate files? Or at least rename the NPV terms to say they are per period
+    # and the real terms to say they are per year, real.
     annualized_costs = [
         {
             "PERIOD": p,
             "Component": annual_cost,
             "Component_type": "annual",
             "AnnualCost_NPV": value(
-                getattr(m, annual_cost)[p] * m.bring_annual_costs_to_base_year[p]
+                getattr(m, annual_cost)[p] * m.bring_future_costs_to_base_year[p]
             ),
             "AnnualCost_Real": value(getattr(m, annual_cost)[p]),
         }
         for p in m.PERIODS
         for annual_cost in m.Cost_Components_Per_Period
     ] + [
         {
@@ -372,15 +393,15 @@
             "Component": tp_cost,
             "Component_type": "timepoint",
             "AnnualCost_NPV": value(
                 sum(
                     getattr(m, tp_cost)[t] * m.tp_weight_in_year[t]
                     for t in m.TPS_IN_PERIOD[p]
                 )
-                * m.bring_annual_costs_to_base_year[p]
+                * m.bring_future_costs_to_base_year[p]
             ),
             "AnnualCost_Real": value(
                 sum(
                     getattr(m, tp_cost)[t] * m.tp_weight_in_year[t]
                     for t in m.TPS_IN_PERIOD[p]
                 )
             ),
```

### Comparing `switch_model-2.0.7/switch_model/generators/core/build.py` & `switch_model-2.0.8/switch_model/generators/core/build.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-# Copyright (c) 2015-2022 The Switch Authors. All rights reserved.
+# Copyright (c) 2015-2024 The Switch Authors. All rights reserved.
 # Licensed under the Apache License, Version 2.0, which is in the LICENSE file.
 """
-Defines generation projects build-outs.
-
+Defines generation project construction and suspension/retirement plan.
 """
 
 import os
 from pyomo.environ import *
 from switch_model.financials import capital_recovery_factor as crf
 from switch_model.reporting import write_table
 from switch_model.utilities import unique_list
@@ -15,186 +14,227 @@
     "switch_model.timescales",
     "switch_model.balancing.load_zones",
     "switch_model.financials",
     "switch_model.energy_sources.properties.properties",
 )
 
 
+def define_arguments(argparser):
+    argparser.add_argument(
+        "--retire",
+        dest="retire_time",
+        default="late",
+        choices=["early", "mid", "late"],
+        help=(
+            "Retire generation projects at the start of the period when they "
+            "reach end-of-life ('early') (i.e., only run if they survive to the "
+            "end of the period), or retire them if they survive past the middle "
+            "of the period ('mid'), or extend operation to the end of the period "
+            "when they reach end-of-life ('late'). Late is the default."
+        ),
+    )
+
+
 def define_components(mod):
     """
 
-    Adds components to a Pyomo abstract model object to describe
-    generation and storage projects. Unless otherwise stated, all power
-    capacity is specified in units of MW and all sets and parameters
-    are mandatory.
-
-    GENERATION_PROJECTS is the set of generation and storage projects that
-    have been built or could potentially be built. A project is a combination
-    of generation technology, load zone and location. A particular build-out
-    of a project should also include the year in which construction was
-    complete and additional capacity came online. Members of this set are
-    abbreviated as gen in parameter names and g in indexes. Use of p instead
-    of g is discouraged because p is reserved for period.
+    Adds components to a Pyomo abstract model object to describe generation and
+    storage projects. Unless otherwise stated, all power capacity is specified
+    in units of MW and all sets and parameters are mandatory.
+
+    GENERATION_PROJECTS is the set of generation and storage projects that have
+    been built or could potentially be built. A project is a combination of
+    generation technology, load zone and location. A particular build-out of a
+    project should also include the year in which construction was complete and
+    additional capacity came online. Members of this set are abbreviated as gen
+    in parameter names and g in indexes. Use of p instead of g is discouraged
+    because p is reserved for period.
 
     gen_dbid[g] is an external database id for each generation project. This is
     an optional parameter than defaults to the project index.
 
-    gen_tech[g] describes what kind of technology a generation project is
-    using.
+    gen_tech[g] describes what kind of technology a generation project is using.
 
     gen_load_zone[g] is the load zone this generation project is built in.
 
-    VARIABLE_GENS is a subset of GENERATION_PROJECTS that only includes
-    variable generators such as wind or solar that have exogenous
-    constraints on their energy production.
-
-    BASELOAD_GENS is a subset of GENERATION_PROJECTS that only includes
-    baseload generators such as coal or geothermal.
-
-    GENS_IN_ZONE[z in LOAD_ZONES] is an indexed set that lists all
-    generation projects within each load zone.
-
-    CAPACITY_LIMITED_GENS is the subset of GENERATION_PROJECTS that are
-    capacity limited. Most of these will be generator types that are resource
-    limited like wind, solar or geothermal, but this can be specified for any
-    generation project. Some existing or proposed generation projects may have
-    upper bounds on increasing capacity or replacing capacity as it is retired
-    based on permits or local air quality regulations.
+    VARIABLE_GENS is a subset of GENERATION_PROJECTS that only includes variable
+    generators such as wind or solar that have exogenous constraints on their
+    energy production.
+
+    BASELOAD_GENS is a subset of GENERATION_PROJECTS that only includes baseload
+    generators such as coal or geothermal.
+
+    GENS_IN_ZONE[z in LOAD_ZONES] is an indexed set that lists all generation
+    projects within each load zone.
+
+    CAPACITY_LIMITED_GENS is the subset of GENERATION_PROJECTS that are capacity
+    limited. Most of these will be generator types that are resource limited
+    like wind, solar or geothermal, but this can be specified for any generation
+    project. Some existing or proposed generation projects may have upper bounds
+    on increasing capacity or replacing capacity as it is retired based on
+    permits or local air quality regulations.
 
     gen_capacity_limit_mw[g] is defined for generation technologies that are
     resource limited and do not compete for land area. This describes the
     maximum possible capacity of a generation project in units of megawatts.
 
-    -- CONSTRUCTION --
+    -- CONSTRUCTION / SUSPENSION / RETIREMENT --
 
-    GEN_BLD_YRS is a two-dimensional set of generation projects and the
-    years in which construction or expansion occured or can occur. You
-    can think of a project as a physical site that can be built out over
-    time. BuildYear is the year in which construction is completed and
-    new capacity comes online, not the year when constrution begins.
-    BuildYear will be in the past for existing projects and will be the
-    first year of an investment period for new projects. Investment
-    decisions are made for each project/invest period combination. This
-    set is derived from other parameters for all new construction. This
-    set also includes entries for existing projects that have already
-    been built and planned projects whose capacity buildouts have already been
-    decided; information for legacy projects come from other files
-    and their build years will usually not correspond to the set of
-    investment periods. There are two recommended options for
-    abbreviating this set for denoting indexes: typically this should be
-    written out as (g, build_year) for clarity, but when brevity is
-    more important (g, b) is acceptable.
-
-    NEW_GEN_BLD_YRS is a subset of GEN_BLD_YRS that only
-    includes projects that have not yet been constructed. This is
-    derived by joining the set of GENERATION_PROJECTS with the set of
-    NEW_GENERATION_BUILDYEARS using generation technology.
-
-    PREDETERMINED_GEN_BLD_YRS is a subset of GEN_BLD_YRS that
-    only includes existing or planned projects that are not subject to
-    optimization.
-
-    build_gen_predetermined[(g, build_year) in PREDETERMINED_GEN_BLD_YRS] is
-    a parameter that describes how much capacity was built in the past
-    for existing projects, or is planned to be built for future projects.
-
-    BuildGen[g, build_year] is a decision variable that describes
-    how much capacity of a project to install in a given period. This also
-    stores the amount of capacity that was installed in existing projects
-    that are still online.
-
-    GenCapacity[g, period] is an expression that returns the total
-    capacity online in a given period. This is the sum of installed capacity
-    minus all retirements.
+    GEN_BLD_YRS is a two-dimensional set of generation projects and the years in
+    which construction or expansion occured or can occur. You can think of a
+    project as a physical site that can be built out over time. BuildYear is the
+    year in which construction is completed and new capacity comes online, not
+    the year when constrution begins. BuildYear will be in the past for existing
+    projects and will be the first year of an investment period for new
+    projects. Investment decisions are made for each project/invest period
+    combination. This set is derived from other parameters for all new
+    construction. This set also includes entries for existing projects that have
+    already been built and planned projects whose capacity buildouts have
+    already been decided; information for legacy projects come from other files
+    and their build years will usually not correspond to the set of investment
+    periods. There are two recommended options for abbreviating this set for
+    denoting indexes: typically this should be written out as (g, build_year)
+    for clarity, but when brevity is more important (g, b) is acceptable.
+
+    NEW_GEN_BLD_YRS is a subset of GEN_BLD_YRS that only includes projects that
+    have not yet been constructed. This is derived by joining the set of
+    GENERATION_PROJECTS with the set of NEW_GENERATION_BUILDYEARS using
+    generation technology.
+
+    PREDETERMINED_GEN_BLD_YRS is a subset of GEN_BLD_YRS that only includes
+    existing or planned projects that are not subject to optimization.
+
+    GEN_BLD_SUSPEND_YRS is the set of all valid generation projects, build years
+    and suspension years, i.e., generator vintages that are active in a given
+    study period, which could therefore be suspended or retired in that period
+
+    NEW_GEN_WITH_MIN_BUILD_YEARS is the subset of NEW_GEN_BLD_YRS for which
+    minimum capacity build-out constraints will be enforced.
+
+    build_gen_predetermined[(g, build_year) in PREDETERMINED_GEN_BLD_YRS] is a
+    parameter that describes how much capacity was built in the past for
+    existing projects, or is planned to be built for future projects.
+
+    gen_can_suspend[g] is a parameter that indicates whether generator `g` can
+    be suspended for one or more periods; if this flag is set to 1 or True, the
+    generator can be suspended and then be unsuspended in later periods.
+
+    gen_can_retire_early[g] is a parameter that indicates whether generator `g`
+    can be retired, which is implemented by being suspended for all the
+    remaining periods of its normal life. If this flag is set to 1 or True, the
+    generator can be suspended in any period, but not resume in later periods.
+    If both gen_can_suspend and gen_can_retire_early are set True,
+    gen_can_suspend takes precedence and temporary suspension is allowed.
+
+    BuildGen[g, build_year] is a decision variable that describes how much
+    capacity of a project to install in a given period. This also stores the
+    amount of capacity that was installed in existing projects that are still
+    online.
+
+    SuspendGen[g, bld_yr, sus_yr] shows how much capacity of project `g` that
+    was built in year `bld_yr` will be suspended in year `sus_yr`, where
+    `sus_yr` is before automatic end of life at `bld_yr + gen_max_age`. For
+    suspended generators, fixed O&M costs go to zero, but capital recovery
+    continues as usual.
+
+    GenCapacity[g, period] is an expression that returns the total capacity
+    online in a given period. This is the sum of installed capacity minus all
+    suspensions and end-of-life retirements.
 
-    Max_Build_Potential[g] is a constraint defined for each project
-    that enforces maximum capacity limits for resource-limited projects.
+    Max_Build_Potential[g] is a constraint defined for each project that
+    enforces maximum capacity limits for resource-limited projects.
 
         GenCapacity <= gen_capacity_limit_mw
 
-    NEW_GEN_WITH_MIN_BUILD_YEARS is the subset of NEW_GEN_BLD_YRS for
-    which minimum capacity build-out constraints will be enforced.
-
-    BuildMinGenCap[g, build_year] is a binary variable that indicates
-    whether a project will build capacity in a period or not. If the model is
-    committing to building capacity, then the minimum must be enforced.
-
-    Enforce_Min_Build_Lower[g, build_year]  and
-    Enforce_Min_Build_Upper[g, build_year] are a pair of constraints that
-    force project build-outs to meet the minimum build requirements for
-    generation technologies that have those requirements. They force BuildGen
-    to be 0 when BuildMinGenCap is 0, and to be greater than
-    gen_min_build_capacity when BuildMinGenCap is 1. In the latter case,
-    the upper constraint should be non-binding; the upper limit is set to 10
-    times the peak non-conincident demand of the entire system.
+    BuildMinGenCap[g, build_year] is a binary variable that indicates whether a
+    project will build capacity in a period or not. If the model is committing
+    to building capacity, then the minimum must be enforced.
+
+    Enforce_Min_Build_Lower[g, build_year]  and Enforce_Min_Build_Upper[g,
+    build_year] are a pair of constraints that force project build-outs to meet
+    the minimum build requirements for generation technologies that have those
+    requirements. They force BuildGen to be 0 when BuildMinGenCap is 0, and to
+    be greater than gen_min_build_capacity when BuildMinGenCap is 1. In the
+    latter case, the upper constraint should be non-binding; the upper limit is
+    set to 10 times the peak non-conincident demand of the entire system.
+
+    Only_Suspend_Built_Capacity[g, build_year, suspend_year] is a constraint
+    that prevents suspending more capacity than has been built
+
+    Only_Suspend_Suspendable_Gens[g, build_year, suspend_year] is a constraint
+    that prevents suspension of generators unless gen_can_suspend or
+    gen_can_retire_early are set.
+
+    Suspend_Retired_gens[g, build_year, suspend_year] is a constraint that
+    requires generators to remain suspended in later periods if they were
+    suspended in an earlier period and gen_can_retire_early is set to True or 1
+    and gen_can_suspend is not set to True or 1.
 
     --- OPERATIONS ---
 
-    PERIODS_FOR_GEN_BLD_YR[g, build_year] is an indexed
-    set that describes which periods a given project build will be
-    operational.
-
-    BLD_YRS_FOR_GEN_PERIOD[g, period] is a complementary
-    indexed set that identify which build years will still be online
-    for the given project in the given period. For some project-period
-    combinations, this will be an empty set.
-
-    PERIODS_FOR_GEN[g] is the set of all periods when generation project
-    g could potentially be operated.
-
-    GEN_PERIODS describes periods in which generation projects
-    could be operational. Unlike the related sets above, it is not
-    indexed. Instead it is specified as a set of (g, period)
-    combinations useful for indexing other model components.
+    PERIODS_FOR_GEN_BLD_YR[g, build_year] is an indexed set that describes which
+    periods a given project build will be operational.
+
+    BLD_YRS_FOR_GEN_PERIOD[g, period] is a complementary indexed set that
+    identify which build years will still be online for the given project in the
+    given period. For some project-period combinations, this will be an empty
+    set.
+
+    PERIODS_FOR_GEN[g] is the set of all periods when generation project g could
+    potentially be operated.
+
+    GEN_PERIODS describes periods in which generation projects could be
+    operational. Unlike the related sets above, it is not indexed. Instead it is
+    specified as a set of (g, period) combinations useful for indexing other
+    model components.
 
 
     --- COSTS ---
 
-    gen_connect_cost_per_mw[g] is the cost of grid upgrades to support a
-    new project, in dollars per peak MW. These costs include new
-    transmission lines to a substation, substation upgrades and any
-    other grid upgrades that are needed to deliver power from the
-    interconnect point to the load center or from the load center to the
-    broader transmission network.
-
-    The following cost components are defined for each project and build
-    year. These parameters will always be available, but will typically
-    be populated by the generic costs specified in generator costs
-    inputs file and the load zone cost adjustment multipliers from
-    load_zones inputs file.
-
-    gen_overnight_cost[g, build_year] is the overnight capital cost per
-    MW of capacity for building a project in the given period. By
-    "installed in the given period", I mean that it comes online at the
-    beginning of the given period and construction starts before that.
-
-    gen_fixed_om[g, build_year] is the annual fixed Operations and
-    Maintenance costs (O&M) per MW of capacity for given project that
-    was installed in the given period.
+    gen_connect_cost_per_mw[g] is the cost of grid upgrades to support a new
+    project, in dollars per peak MW. These costs include new transmission lines
+    to a substation, substation upgrades and any other grid upgrades that are
+    needed to deliver power from the interconnect point to the load center or
+    from the load center to the broader transmission network.
+
+    The following cost components are defined for each project and build year.
+    These parameters will always be available, but will typically be populated
+    by the generic costs specified in generator costs inputs file and the load
+    zone cost adjustment multipliers from load_zones inputs file.
+
+    gen_overnight_cost[g, build_year] is the overnight capital cost per MW of
+    capacity for building a project in the given period. By "installed in the
+    given period", I mean that it comes online at the beginning of the given
+    period and construction starts before that.
+
+    gen_fixed_om[g, build_year] is the annual fixed Operations and Maintenance
+    costs (O&M) per MW of capacity for given project that was installed in the
+    given period.
 
     -- Derived cost parameters --
 
-    gen_capital_cost_annual[g, build_year] is the annualized loan
-    payments for a project's capital and connection costs in units of
-    $/MW per year. This is specified in non-discounted real dollars in a
-    future period, not real dollars in net present value.
-
-    Proj_Fixed_Costs_Annual[g, period] is the total annual fixed
-    costs (capital as well as fixed operations & maintenance) incurred
-    by a project in a period. This reflects all of the builds are
-    operational in the given period. This is an expression that reflect
-    decision variables.
-
-    ProjFixedCosts[period] is the sum of
-    Proj_Fixed_Costs_Annual[g, period] for all projects that could be
-    online in the target period. This aggregation is performed for the
-    benefit of the objective function.
-
-    TODO:
-    - Allow early capacity retirements with savings on fixed O&M
+    gen_capital_cost_annual[g, build_year] is the annualized loan payments for a
+    project's capital and connection costs in units of $/MW per year. This is
+    specified in non-discounted real dollars in a future period, not real
+    dollars in net present value.
+
+    GenCapitalCosts[g, period] is the total annual capital recovery required for
+    a project in a period. This includes all of the builds that have not yet
+    reached their maximum age. Capital costs continue to be recovered even if a
+    generator is suspended or retired (and they are not brought forward to the
+    retirement year).
+
+    GenFixedOMCosts[g, period] is the total annual fixed operations &
+    maintenance cost incurred by a project in a period. This reflects all of the
+    builds that are operational (haven't reached end of life or been suspended)
+    in the given period.
+
+    TotalGenFixedCosts[period] is the sum of GenCapitalCosts[g, period] and
+    GenFixedOMCosts[g, period] for all projects that could be online in the
+    target period.
 
     """
     mod.GENERATION_PROJECTS = Set(dimen=1)
     mod.gen_dbid = Param(mod.GENERATION_PROJECTS, default=lambda m, g: g, within=Any)
     mod.gen_tech = Param(mod.GENERATION_PROJECTS, within=Any)
     mod.GENERATION_TECHNOLOGIES = Set(
         dimen=1,
@@ -215,14 +255,18 @@
     )
     mod.gen_scheduled_outage_rate = Param(
         mod.GENERATION_PROJECTS, within=PercentFraction, default=0
     )
     mod.gen_forced_outage_rate = Param(
         mod.GENERATION_PROJECTS, within=PercentFraction, default=0
     )
+    mod.gen_can_suspend = Param(mod.GENERATION_PROJECTS, within=Boolean, default=False)
+    mod.gen_can_retire_early = Param(
+        mod.GENERATION_PROJECTS, within=Boolean, default=False
+    )
     mod.min_data_check(
         "GENERATION_PROJECTS",
         "gen_tech",
         "gen_energy_source",
         "gen_load_zone",
         "gen_max_age",
         "gen_is_variable",
@@ -381,37 +425,54 @@
     mod.build_gen_predetermined = Param(
         mod.PREDETERMINED_GEN_BLD_YRS, within=NonNegativeReals
     )
     mod.min_data_check("build_gen_predetermined")
 
     def gen_build_can_operate_in_period(m, g, build_year, period):
         if build_year in m.PERIODS:
+            # always build at start of period
             online = m.period_start[build_year]
         else:
             online = build_year
         retirement = online + m.gen_max_age[g]
-        return online <= m.period_start[period] < retirement
-        # This is probably more correct, but is a different behavior
-        # mid_period = m.period_start[period] + 0.5 * m.period_length_years[period]
-        # return online <= m.period_start[period] and mid_period <= retirement
+        if build_year == period:
+            # always allow operation during the period it is built, even
+            # if asset life isn't enough to cover the period
+            can_run = True
+        elif m.options.retire_time == "late":
+            # default:
+            # operate if it survives across the start of the period
+            # (but not if it retires exactly at the start, i.e., in the
+            # prior period)
+            can_run = online <= m.period_start[period] < retirement
+        elif m.options.retire_time == "mid":
+            mid_period = m.period_start[period] + 0.5 * m.period_length_years[period]
+            can_run = online <= mid_period <= retirement
+        else:
+            # user-chose retire-at-start-of-period option
+            # operate if it survives across the end of the period
+            # (but not if it's built right at the end, i.e., in the
+            # next period)
+            can_run = online < m.period_end[period] <= retirement
+        return can_run
 
     # The set of periods when a project built in a certain year will be online
     mod.PERIODS_FOR_GEN_BLD_YR = Set(
         mod.GEN_BLD_YRS,
         dimen=1,
         within=mod.PERIODS,
         ordered=True,
         initialize=lambda m, g, bld_yr: [
             period
             for period in m.PERIODS
             if gen_build_can_operate_in_period(m, g, bld_yr, period)
         ],
     )
     # The set of build years that could be online in the given period
-    # for the given project.
+    # for the given project (possibly empty).
     mod.BLD_YRS_FOR_GEN_PERIOD = Set(
         mod.GENERATION_PROJECTS,
         mod.PERIODS,
         dimen=1,
         initialize=lambda m, g, period: unique_list(
             bld_yr
             for (gen, bld_yr) in m.GEN_BLD_YRS
@@ -437,14 +498,15 @@
             # This does not replace Max_Build_Potential because
             # Max_Build_Potential applies across all build years.
             return (0, model.gen_capacity_limit_mw[g])
         else:
             return (0, None)
 
     mod.BuildGen = Var(mod.GEN_BLD_YRS, within=NonNegativeReals, bounds=bounds_BuildGen)
+
     # Some projects are retired before the first study period, so they
     # don't appear in the objective function or any constraints.
     # In this case, pyomo may leave the variable value undefined even
     # after a solve, instead of assigning a value within the allowed
     # range. This causes errors in the Progressive Hedging code, which
     # expects every variable to have a value after the solve. So as a
     # starting point we assign an appropriate value to all the existing
@@ -468,19 +530,78 @@
     mod.GEN_PERIODS = Set(
         dimen=2,
         initialize=lambda m: [
             (g, p) for g in m.GENERATION_PROJECTS for p in m.PERIODS_FOR_GEN[g]
         ],
     )
 
+    # set of years when a generator vintage (generator/build-year combination)
+    # can have operation suspended and avoid fixed O&M charges.
+    mod.GEN_BLD_SUSPEND_YRS = Set(
+        dimen=3,
+        within=mod.GEN_BLD_YRS * mod.PERIODS,
+        initialize=lambda m: [
+            (g, bld_yr, sus_yr)
+            for g, bld_yr in m.GEN_BLD_YRS
+            for sus_yr in m.PERIODS_FOR_GEN_BLD_YR[g, bld_yr]
+        ],
+    )
+
+    # SuspendGen[g, bld_yr, sus_yr] shows how much capacity of project `g`
+    # that was built in year `bld_yr` will be suspended in year `sus_yr`, where
+    # `sus_yr` is before automatic end of life at `bld_yr + gen_max_age`
+    mod.SuspendGen = Var(mod.GEN_BLD_SUSPEND_YRS, within=NonNegativeReals)
+
+    # Don't suspend more capacity than has been built
+    mod.Only_Suspend_Built_Capacity = Constraint(
+        mod.GEN_BLD_SUSPEND_YRS,
+        rule=lambda m, g, bld_yr, sus_yr: m.SuspendGen[g, bld_yr, sus_yr]
+        <= m.BuildGen[g, bld_yr],
+    )
+
+    # only suspend if allowed
+    mod.Only_Suspend_Suspendable_Gens = Constraint(
+        mod.GEN_BLD_SUSPEND_YRS,
+        rule=lambda m, g, bld_yr, sus_yr: (
+            Constraint.Skip
+            if m.gen_can_suspend[g] or m.gen_can_retire_early[g]
+            else (m.SuspendGen[g, bld_yr, sus_yr] == 0)
+        ),
+    )
+
+    # Force permanent retirement (suspension must continue through all later
+    # years), if early retirement is allowed but suspension is not
+    def rule(m, g, bld_yr, sus_yr):
+        if m.gen_can_retire_early[g] and not m.gen_can_suspend[g]:
+            # gen can retire, but not suspend
+            try:
+                # it's tricky to anticipate which combinations of g, bld_yr, and
+                # sus_yr could have been suspended in the prior period (e.g., a
+                # plant scheduled for construction in 2025 would be active in a
+                # 2021-2030 period when using early retirement, but not when
+                # using late retirement). So we just give it a try and catch
+                # errors if the previous period doesn't exist or wasn't a
+                # suspendable year.
+                return (
+                    m.SuspendGen[g, bld_yr, sus_yr]
+                    >= m.SuspendGen[g, bld_yr, m.PERIODS.prev(sus_yr)]
+                )
+            except (KeyError, IndexError):
+                # couldn't suspend in previous period (if it existed)
+                pass
+        return Constraint.Skip
+
+    mod.Suspend_Retired_Gens = Constraint(mod.GEN_BLD_SUSPEND_YRS, rule=rule)
+
     mod.GenCapacity = Expression(
         mod.GENERATION_PROJECTS,
         mod.PERIODS,
         rule=lambda m, g, period: sum(
-            m.BuildGen[g, bld_yr] for bld_yr in m.BLD_YRS_FOR_GEN_PERIOD[g, period]
+            m.BuildGen[g, bld_yr] - m.SuspendGen[g, bld_yr, period]
+            for bld_yr in m.BLD_YRS_FOR_GEN_PERIOD[g, period]
         ),
     )
 
     mod.Max_Build_Potential = Constraint(
         mod.CAPACITY_LIMITED_GENS,
         mod.PERIODS,
         rule=lambda m, g, p: (m.gen_capacity_limit_mw[g] >= m.GenCapacity[g, p]),
@@ -516,22 +637,22 @@
         rule=lambda m, g, p: (
             m.BuildGen[g, p]
             <= m.BuildMinGenCap[g, p] * mod._gen_max_cap_for_binary_constraints
         ),
     )
 
     # Costs
-    mod.gen_variable_om = Param(mod.GENERATION_PROJECTS, within=NonNegativeReals)
+    mod.gen_variable_om = Param(mod.GENERATION_PROJECTS, within=Reals)
     mod.gen_connect_cost_per_mw = Param(
         mod.GENERATION_PROJECTS, within=NonNegativeReals
     )
     mod.min_data_check("gen_variable_om", "gen_connect_cost_per_mw")
 
     mod.gen_overnight_cost = Param(mod.GEN_BLD_YRS, within=NonNegativeReals)
-    mod.gen_fixed_om = Param(mod.GEN_BLD_YRS, within=NonNegativeReals)
+    mod.gen_fixed_om = Param(mod.GEN_BLD_YRS, within=Reals)
     mod.min_data_check("gen_overnight_cost", "gen_fixed_om")
 
     # Derived annual costs
     mod.gen_capital_cost_annual = Param(
         mod.GEN_BLD_YRS,
         within=NonNegativeReals,
         initialize=lambda m, g, bld_yr: (
@@ -548,15 +669,16 @@
             for bld_yr in m.BLD_YRS_FOR_GEN_PERIOD[g, p]
         ),
     )
     mod.GenFixedOMCosts = Expression(
         mod.GENERATION_PROJECTS,
         mod.PERIODS,
         rule=lambda m, g, p: sum(
-            m.BuildGen[g, bld_yr] * m.gen_fixed_om[g, bld_yr]
+            (m.BuildGen[g, bld_yr] - m.SuspendGen[g, bld_yr, p])
+            * m.gen_fixed_om[g, bld_yr]
             for bld_yr in m.BLD_YRS_FOR_GEN_PERIOD[g, p]
         ),
     )
     # Summarize costs for the objective function. Units should be total
     # annual future costs in $base_year real dollars. The objective
     # function will convert these to base_year Net Present Value in
     # $base_year real dollars.
@@ -636,14 +758,16 @@
             mod.gen_ccs_capture_efficiency,
             mod.gen_full_load_heat_rate,
             mod.gen_variable_om,
             mod.gen_min_build_capacity,
             mod.gen_connect_cost_per_mw,
             mod.gen_is_cogen,
             mod.gen_is_distributed,
+            mod.gen_can_suspend,
+            mod.gen_can_retire_early,
         ),
     )
     # Construct sets of capacity-limited, ccs-capable and unit-size-specified
     # projects. These sets include projects for which these parameters have
     # a value
     if "gen_capacity_limit_mw" in switch_data.data():
         switch_data.data()["CAPACITY_LIMITED_GENS"] = {
@@ -696,30 +820,32 @@
         ),
         values=lambda m, g, p: (
             g,
             p,
             m.gen_tech[g],
             m.gen_load_zone[g],
             m.gen_energy_source[g],
-            m.BuildGen[g, p] if (g, p) in m.BuildGen else 0.0,
+            m.BuildGen[g, p] if (g, p) in m.BuildGen else ".",
             (
                 m.BuildStorageEnergy[g, p]
                 if hasattr(m, "BuildStorageEnergy") and (g, p) in m.BuildStorageEnergy
-                else 0.0
+                else "."
             ),
             (
                 (m.gen_overnight_cost[g, p] + m.gen_connect_cost_per_mw[g])
                 * m.BuildGen[g, p]
+                + (
+                    m.BuildStorageEnergy[g, p]
+                    * m.gen_storage_energy_overnight_cost[g, p]
+                    if hasattr(m, "BuildStorageEnergy")
+                    and (g, p) in m.BuildStorageEnergy
+                    else 0.0
+                )
                 if (g, p) in m.BuildGen
-                else 0.0
-            )
-            + (
-                (m.BuildStorageEnergy[g, p] * m.gen_storage_energy_overnight_cost[g, p])
-                if hasattr(m, "BuildStorageEnergy") and (g, p) in m.BuildStorageEnergy
-                else 0.0
+                else "."
             ),
         ),
     )
 
     # report total generator and storage capacity in place for each generator in
     # each period. Also show capital and fixed O&M recovery per year in that
     # period (these are the costs Switch seeks to minimize)
@@ -731,30 +857,34 @@
         headings=(
             "GENERATION_PROJECT",
             "PERIOD",
             "gen_tech",
             "gen_load_zone",
             "gen_energy_source",
             "GenCapacity",
+            "SuspendGen_total",
             "GenStorageCapacity",
             "GenCapitalRecovery",
             "GenFixedOMCosts",
         ),
         values=lambda m, g, p: (
             g,
             p,
             m.gen_tech[g],
             m.gen_load_zone[g],
             m.gen_energy_source[g],
             m.GenCapacity[g, p],
+            sum(
+                m.SuspendGen[g, bld_yr, p] for bld_yr in m.BLD_YRS_FOR_GEN_PERIOD[g, p]
+            ),
             (
                 m.StorageEnergyCapacity[g, p]
                 if hasattr(m, "StorageEnergyCapacity")
                 and (g, p) in m.StorageEnergyCapacity
-                else 0.0
+                else "."
             ),
             m.GenCapitalCosts[g, p]
             + (
                 m.StorageEnergyCapitalCost[g, p]
                 if hasattr(m, "StorageEnergyCapitalCost")
                 and (g, p) in m.StorageEnergyCapitalCost
                 else 0.0
```

### Comparing `switch_model-2.0.7/switch_model/generators/core/commit/discrete.py` & `switch_model-2.0.8/switch_model/generators/core/commit/discrete.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/generators/core/commit/fuel_use.py` & `switch_model-2.0.8/switch_model/generators/core/commit/fuel_use.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,15 +205,15 @@
                 switch_data.data()["gen_min_load_fraction"] = {}
             dp_dict = switch_data.data(name="gen_min_load_fraction")
             if g in dp_dict:
                 min_load_dat = dp_dict[g]
                 if not approx_equal(min_load[g], min_load_dat):
                     raise ValueError(
                         (
-                            "gen_min_load_fraction is inconsistant with "
+                            "gen_min_load_fraction is inconsistent with "
                             + "incremental heat rate data for project "
                             + "{}."
                         ).format(g)
                     )
             else:
                 dp_dict[g] = min_load[g]
         # Same thing, but for full load heat rate.
@@ -222,15 +222,15 @@
                 switch_data.data()["gen_full_load_heat_rate"] = {}
             dp_dict = switch_data.data(name="gen_full_load_heat_rate")
             if g in dp_dict:
                 full_hr_dat = dp_dict[g]
                 if abs((full_hr[g] - full_hr_dat) / full_hr_dat) > 0.01:
                     raise ValueError(
                         (
-                            "gen_full_load_heat_rate is inconsistant with "
+                            "gen_full_load_heat_rate is inconsistent with "
                             + "incremental heat rate data for project "
                             + "{}."
                         ).format(g)
                     )
             else:
                 dp_dict[g] = full_hr[g]
         # Copy parsed data into the data portal.
@@ -322,15 +322,15 @@
         ihr_dat[u].sort()
         # Assume that the maximum power output is the rated capacity.
         (junk, capacity, junk) = ihr_dat[u][len(ihr_dat[u]) - 1]
         # Retrieve the first incremental heat rate for error checking.
         (min_power, junk, ihr_prev) = ihr_dat[u][0]
         min_cap_factor[u] = min_power / capacity
         # Process each line segment.
-        for (p_start, p_end, ihr) in ihr_dat[u]:
+        for p_start, p_end, ihr in ihr_dat[u]:
             # Error check: This incremental heat rate cannot be less than
             # the previous one.
             if ihr_prev > ihr:
                 raise ValueError(
                     (
                         "Error processing incremental heat rates for "
                         + "{} in file {}. The incremental heat rate "
```

### Comparing `switch_model-2.0.7/switch_model/generators/core/commit/operate.py` & `switch_model-2.0.8/switch_model/generators/core/commit/operate.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/generators/core/dispatch.py` & `switch_model-2.0.8/switch_model/generators/core/dispatch.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,15 +153,15 @@
     implemented in separate modules.
 
     """
 
     def period_active_gen_rule(m, period):
         if not hasattr(m, "period_active_gen_dict"):
             m.period_active_gen_dict = dict()
-            for (_g, _period) in m.GEN_PERIODS:
+            for _g, _period in m.GEN_PERIODS:
                 m.period_active_gen_dict.setdefault(_period, []).append(_g)
         result = m.period_active_gen_dict.pop(period)
         if len(m.period_active_gen_dict) == 0:
             delattr(m, "period_active_gen_dict")
         return result
 
     mod.GENS_IN_PERIOD = Set(
@@ -262,15 +262,15 @@
     )
     try:
         mod.Distributed_Power_Injections.append("ZoneTotalDistributedDispatch")
     except AttributeError:
         mod.Zone_Power_Injections.append("ZoneTotalDistributedDispatch")
 
     def init_gen_availability(m, g):
-        if m.gen_is_baseload[g]:
+        if g in m.BASELOAD_GENS:
             return (1 - m.gen_forced_outage_rate[g]) * (
                 1 - m.gen_scheduled_outage_rate[g]
             )
         else:
             return 1 - m.gen_forced_outage_rate[g]
 
     mod.gen_availability = Param(
@@ -298,29 +298,30 @@
         # Tell user if the input files specify timeseries for renewable plant
         # capacity factors that extend beyond the lifetime of the plant.
         def rule(m):
             extra_indexes = m.VARIABLE_GEN_TPS_RAW - m.VARIABLE_GEN_TPS
             if extra_indexes:
                 num_impacted_generators = len(set(g for g, t in extra_indexes))
                 extraneous = {g: [] for (g, t) in extra_indexes}
-                for (g, t) in extra_indexes:
+                for g, t in extra_indexes:
                     extraneous[g].append(t)
                 pprint = "\n".join(
                     "* {}: {} to {}".format(g, min(tps), max(tps))
                     for g, tps in extraneous.items()
                 )
                 # basic message for everyone at info level
                 msg = unwrap(
                     """
-                    {} generation project[s] have data in
+                    {} generation project{} data in
                     variable_capacity_factors.csv for timepoints when they are
                     not operable, either before construction is possible or
                     after retirement.
                 """.format(
-                        num_impacted_generators
+                        num_impacted_generators,
+                        " has" if num_impacted_generators == 1 else "s have",
                     )
                 )
                 if m.logger.isEnabledFor(logging.DEBUG):
                     # more detailed message
                     msg += unwrap(
                         """
                          You can avoid this message by only placing data in
@@ -453,22 +454,25 @@
                 instance.DispatchGen[g, t] * instance.tp_weight_in_year[t] / 1000
             ),
             "VariableCost_per_yr": value(
                 instance.DispatchGen[g, t]
                 * instance.gen_variable_om[g]
                 * instance.tp_weight_in_year[t]
             ),
-            "DispatchEmissions_tCO2_per_typical_yr": value(
-                sum(
-                    instance.DispatchEmissions[g, t, f] * instance.tp_weight_in_year[t]
-                    for f in instance.FUELS_FOR_GEN[g]
+            "DispatchEmissions_tCO2_per_typical_yr": (
+                value(
+                    sum(
+                        instance.DispatchEmissions[g, t, f]
+                        * instance.tp_weight_in_year[t]
+                        for f in instance.FUELS_FOR_GEN[g]
+                    )
                 )
-            )
-            if instance.gen_uses_fuel[g]
-            else 0,
+                if instance.gen_uses_fuel[g]
+                else 0
+            ),
             "GenCapacity_MW": value(instance.GenCapacity[g, p]),
             "GenCapitalCosts": value(instance.GenCapitalCosts[g, p]),
             "GenFixedOMCosts": value(instance.GenFixedOMCosts[g, p]),
         }
         try:
             try:
                 record["ChargeStorage_MW"] = -1.0 * value(instance.ChargeStorage[g, t])
```

### Comparing `switch_model-2.0.7/switch_model/generators/core/gen_discrete_build.py` & `switch_model-2.0.8/switch_model/generators/core/gen_discrete_build.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,7 +45,23 @@
     mod.BuildUnits = Var(mod.DISCRETE_GEN_BLD_YRS, within=NonNegativeIntegers)
     mod.Build_Units_Consistency = Constraint(
         mod.DISCRETE_GEN_BLD_YRS,
         rule=lambda m, g, bld_yr: (
             m.BuildGen[g, bld_yr] == m.BuildUnits[g, bld_yr] * m.gen_unit_size[g]
         ),
     )
+    if hasattr(mod, "EarlyRetireGen"):
+        mod.DISCRETE_GEN_BLD_RETIRE_YRS = Set(
+            dimen=3,
+            initialize=mod.GEN_BLD_RETIRE_YRS,
+            filter=lambda m, g, bld_yr, ret_yr: g in m.DISCRETELY_SIZED_GENS,
+        )
+        mod.EarlyRetireUnits = Var(
+            mod.DISCRETE_GEN_BLD_RETIRE_YRS, within=NonNegativeIntegers
+        )
+        mod.Early_Retire_Units_Consistency = Constraint(
+            mod.DISCRETE_GEN_BLD_RETIRE_YRS,
+            rule=lambda m, g, bld_yr, ret_yr: (
+                m.EarlyRetireGen[g, bld_yr, ret_yr]
+                == m.EarlyRetireUnits[g, bld_yr, ret_yr] * m.gen_unit_size[g]
+            ),
+        )
```

### Comparing `switch_model-2.0.7/switch_model/generators/core/no_commit.py` & `switch_model-2.0.8/switch_model/generators/core/no_commit.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/generators/extensions/hydro_simple.py` & `switch_model-2.0.8/switch_model/generators/extensions/hydro_simple.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/generators/extensions/hydro_system.py` & `switch_model-2.0.8/switch_model/generators/extensions/hydro_system.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,225 +41,211 @@
     "switch_model.generators.core.dispatch",
 )
 
 
 def define_components(mod):
     """
 
-    WATER_NODES is the set of nodes of the water system that do not have
-    storage capacity. These usually represent confluence and/or divergence
-    of different water flows. Members of this set can be abbreviated as
-    wn or wnode.
-
-    WNODE_TPS is a set showing all the combinations of
-    water nodes and timepoints, in which the conservation of mass law
-    must be enforced. For now it is initialized as the cross product of
-    the WATER_NODES and TIMEPOINTS sets, but it should be flexibilized
-    to allow for addition and removal of water nodes in intermediate
-    timepoints of the simulation horizon.
-
-    wnode_constant_inflow[wn] is the value of constant inflow of
-    water at each node of the hydraulic system throughout the whole
-    simulation. Inflow refers to an external source of water that comes
-    into the system at the water node, such as rainfall. Water flows
-    that originate from an upstream model component, such as another water
-    node or a reservoir, are decided by the model and so must not be
-    specified here. This parameter is specified in cubic meters per second
-    (cumec) and defaults to 0.
-
-    wnode_constant_consumption[wn] is the value of constant
-    consumption of water at each node of the hydraulic system throughout
-    the whole simulation. Consumption refers to any activity that takes
-    water out of the modeled hydraulic system, such as crop irrigation,
-    human and animal consumption, minimum ecological flow for a sink
-    node, etc. This parameter is specified in cubic meters per second
-    (cumec) and defaults to 0.
-
-    wnode_tp_inflow[wn, t] and wnode_tp_consumption[wn, t]
-    are the values of water inflow and consumption at each node of the
-    hydraulic system specified at each timepoint. These are optional
-    parameters that default to wnode_constant_inflow and
-    wnode_constant_consumption. Depending on data availability,
-    these parameters may be used to represent different phenomena. In
-    example, the Chilean datasets specify water inflows due to rainfall
-    and melting snows at different nodes in a weekly basis. So, all
-    simulated timepoints that belong to the same week will have the same
-    wnode_tp_inflow parameter specified for each water node.
-
-    wn_is_sink[WATER_NODES] is a binary flag indicating whether a water
-    node is a sink. These nodes need not obey the law of conservation of
-    mass, so that water flows that go into them may be greater than the
-    ones that flow out. The main use case for these is to be the end of a
-    water basin (such as the ocean or a lake).
+    WATER_NODES is the set of nodes of the water system that do not have storage
+    capacity. These usually represent confluence and/or divergence of different
+    water flows. Members of this set can be abbreviated as wn or wnode.
+
+    WNODE_TPS is a set showing all the combinations of water nodes and
+    timepoints, in which the conservation of mass law must be enforced. For now
+    it is initialized as the cross product of the WATER_NODES and TIMEPOINTS
+    sets, but it should be flexibilized to allow for addition and removal of
+    water nodes in intermediate timepoints of the simulation horizon.
+
+    wnode_constant_inflow[wn] is the value of constant inflow of water at each
+    node of the hydraulic system throughout the whole simulation. Inflow refers
+    to an external source of water that comes into the system at the water node,
+    such as rainfall. Water flows that originate from an upstream model
+    component, such as another water node or a reservoir, are decided by the
+    model and so must not be specified here. This parameter is specified in
+    cubic meters per second (cumec) and defaults to 0.
+
+    wnode_constant_consumption[wn] is the value of constant consumption of water
+    at each node of the hydraulic system throughout the whole simulation.
+    Consumption refers to any activity that takes water out of the modeled
+    hydraulic system, such as crop irrigation, human and animal consumption,
+    minimum ecological flow for a sink node, etc. This parameter is specified in
+    cubic meters per second (cumec) and defaults to 0.
+
+    wnode_tp_inflow[wn, t] and wnode_tp_consumption[wn, t] are the values of
+    water inflow and consumption at each node of the hydraulic system specified
+    at each timepoint. These are optional parameters that default to
+    wnode_constant_inflow and wnode_constant_consumption. Depending on data
+    availability, these parameters may be used to represent different phenomena.
+    In example, the Chilean datasets specify water inflows due to rainfall and
+    melting snows at different nodes in a weekly basis. So, all simulated
+    timepoints that belong to the same week will have the same wnode_tp_inflow
+    parameter specified for each water node.
+
+    wn_is_sink[WATER_NODES] is a binary flag indicating whether a water node is
+    a sink. These nodes need not obey the law of conservation of mass, so that
+    water flows that go into them may be greater than the ones that flow out.
+    The main use case for these is to be the end of a water basin (such as the
+    ocean or a lake).
 
     node_spillage_cost is the parameter that sets the cost in $/(cubic meters)
     of spilling water out of the water network. This is equivalent to relaxing
     the conservation of mass law when balancing flows in each node and
     timepoint, so cost is set to a high default value. This parameter lets the
-    model spill water freely in sink nodes, but relaxes the equality
-    constraint for mass balance. This aids the solver in obtaining optimal
-    solutions significantly faster and with small water spillages.
-
-    SpillWaterAtNode[WNODE_TPS] are  the decisions of
-    water spillage out of the water network at each node and timepoint
-    in  cubic meters per second.
-
-
-    RESERVOIRS is a subset of water nodes that are reservoirs. These
-    require additional characterization. Members of this set may be
-    abbreviated as r or res.
-
-    res_min_vol[r] is a parameter that specifies the minimum storage
-    capacity of the reservoir in millions of cubic meters. Usually
-    this will be a positive value, since reservoirs cannot be
-    completely emptied because of physical limitations, but it is
-    allowed to be 0 in case relative volumes want to be used.
-
-    res_max_vol[r] is a parameter that specifies the maximum storage
-    capacity of the reservoir in millions of cubic meters. If at any
-
-    timepoint the volume of water in the reservoir reaches this limit,
-    spillage may occur to mantain the mass balance. This parameter is
-    determined by the physical characteristics of the reservoir.
-
-    RESERVOIR_TPS is a set showing all the combinations of
-    reservoirs and timepoints, in which the conservation of mass law
-    must be enforced. For now it is initialized as the cross product of
-    the RESERVOIRS and TIMEPOINTS sets, but it should be flexibilized
-    to allow for addition and removal of reservoirs in intermediate
-    timepoints of the simulation horizon.
-
-    res_min_vol_tp[r, t] and res_max_vol_tp[r, t] are the
-    values of allowable minimum and maximum water volume at each
-    reservoir specified at each timepoint. These may be used to represent
-    seasonal restrictions in water levels at any reservoir. In example,
-    minimum volumes of water must be kept during summer at some reservoirs
-    to allow for leisure and tourism activities, such as water sports.
-    These parameters are optional and must be specified in cubic meters
-    and default to reservoir_min_vol and reservoir_max_vol.
-
-    initial_res_vol[r] is a parameter that states the starting volume
-    of stored water in each reservoir in millions of cubic meters. The
-    same value will be used as a starting point in each period of the
-    simulation, independent of which was the final level at the last
-    timepoint of the previous period. This methodology has been used
-    in several expansion planning papers  that include reservoir hydro
-    power plants, because it allows decoupling the operational
+    model spill water freely in sink nodes, but relaxes the equality constraint
+    for mass balance. This aids the solver in obtaining optimal solutions
+    significantly faster and with small water spillages.
+
+    SpillWaterAtNode[WNODE_TPS] are  the decisions of water spillage out of the
+    water network at each node and timepoint in  cubic meters per second.
+
+
+    RESERVOIRS is a subset of water nodes that are reservoirs. These require
+    additional characterization. Members of this set may be abbreviated as r or
+    res.
+
+    res_min_vol[r] is a parameter that specifies the minimum storage capacity of
+    the reservoir in millions of cubic meters. Usually this will be a positive
+    value, since reservoirs cannot be completely emptied because of physical
+    limitations, but it is allowed to be 0 in case relative volumes want to be
+    used.
+
+    res_max_vol[r] is a parameter that specifies the maximum storage capacity of
+    the reservoir in millions of cubic meters. If at any timepoint the volume of
+    water in the reservoir reaches this limit, spillage may occur to mantain the
+    mass balance. This parameter is determined by the physical characteristics
+    of the reservoir.
+
+    RESERVOIR_TPS is a set showing all the combinations of reservoirs and
+    timepoints, in which the conservation of mass law must be enforced. For now
+    it is initialized as the cross product of the RESERVOIRS and TIMEPOINTS
+    sets, but it should be flexibilized to allow for addition and removal of
+    reservoirs in intermediate timepoints of the simulation horizon.
+
+    res_min_vol_tp[r, t] and res_max_vol_tp[r, t] are the values of allowable
+    minimum and maximum water volume at each reservoir specified at each
+    timepoint. These may be used to represent seasonal restrictions in water
+    levels at any reservoir. In example, minimum volumes of water must be kept
+    during summer at some reservoirs to allow for leisure and tourism
+    activities, such as water sports. These parameters are optional and must be
+    specified in cubic meters and default to reservoir_min_vol and
+    reservoir_max_vol.
+
+    initial_res_vol[r] is a parameter that states the starting volume of stored
+    water in each reservoir in millions of cubic meters. The same value will be
+    used as a starting point in each period of the simulation, independent of
+    which was the final level at the last timepoint of the previous period. This
+    methodology has been used in several expansion planning papers  that include
+    reservoir hydro power plants, because it allows decoupling the operational
     subproblems of each period and thus speeding up the optimization
     considerably.
 
-    final_res_vol[r] is a parameter that states the final volume of
-    stored water in each reservoir in millions of cubic meters. This
-    level is enforced as a minimum for the final volume. Usually, this
-    parameter is specified to be the same as  the initial volume, so
-    that the reservoir may only arbitrage with the water inflows that
-    come into it during the period.
-
-    ReservoirVol[r, t] is a variable that tracks the volume of water
-    at each reservoir in the beginging of each timepoint, specified in
-    cubic meters. This variable is determined by the volume in the
-    previous timepoint, the inflows and the outflows.
-
-    ReservoirFinalVol[r, p] is the amount of water in the reservoir after
-    the last timepoint of each period.
-
-    WATER_CONNECTIONS is the set of flows that begin and end in different
-    water bodies, such as reservoirs and nodes. The model decides how much
-    water is "dispatched" through each connection at each timepoint. Water
-    may only flow in one direction, so "to" and "from" parameters must be
-    inputted. Members of this set may be abbreviated by wc or wcon.
-
-    WCON_TPS is the set of the cross product between
-    TIMEPOINTS and WATER_CONNECTIONS. In the future, this should be
-    flexibilized to allow for new water connections to be created within
-    the simulation horizon (as with WNODE_TPS and
-    RESERVOIR_TPS).
-
-    water_node_from[wc] is a parameter that specifies the water body from
-    which the connection extracts water.
-
-    water_node_to[wc] is a parameter that specifies the water body to which
-    the connection injects water.
-
-    wc_capacity[wc] is a parameter that specifies the limit, in cubic
-    meters per second, of the water flow through the connection. This
-    datum is difficult to find, but could be relevant in some cases where
-    rivers or streams have a defined capacity and greater flows could
-    cause them to collapse and/or flood the surrounding area. Defaults
-    to 9999 cumec.
+    final_res_vol[r] is a parameter that states the final volume of stored water
+    in each reservoir in millions of cubic meters. This level is enforced as a
+    minimum for the final volume. Usually, this parameter is specified to be the
+    same as  the initial volume, so that the reservoir may only arbitrage with
+    the water inflows that come into it during the period.
+
+    ReservoirVol[r, t] is a variable that tracks the volume of water at each
+    reservoir in the beginging of each timepoint, specified in millions of cubic
+    meters. This variable is determined by the volume in the previous timepoint,
+    the inflows and the outflows.
+
+    ReservoirFinalVol[r, p] is the amount of water in the reservoir after the
+    last timepoint of each period.
+
+    WATER_CONNECTIONS is the set of flows that begin and end in different water
+    bodies, such as reservoirs and nodes. The model decides how much water is
+    "dispatched" through each connection at each timepoint. Water may only flow
+    in one direction, so "to" and "from" parameters must be inputted. Members of
+    this set may be abbreviated by wc or wcon.
+
+    WCON_TPS is the set of the cross product between TIMEPOINTS and
+    WATER_CONNECTIONS. In the future, this should be flexibilized to allow for
+    new water connections to be created within the simulation horizon (as with
+    WNODE_TPS and RESERVOIR_TPS).
+
+    water_node_from[wc] is a parameter that specifies the water body from which
+    the connection extracts water.
+
+    water_node_to[wc] is a parameter that specifies the water body to which the
+    connection injects water.
+
+    wc_capacity[wc] is a parameter that specifies the limit, in cubic meters per
+    second, of the water flow through the connection. This datum is difficult to
+    find, but could be relevant in some cases where rivers or streams have a
+    defined capacity and greater flows could cause them to collapse and/or flood
+    the surrounding area. Defaults to infinity.
 
     min_eco_flow[wc, t] is a parameter that indicates the minimum ecological
     water flow that must be dispatched through each water connection at each
-    timepoint, specified in cubic meters per second. The parameter is
-    indexed by timepoint to allow for representation of seasonal or hourly
-    ecological or social constraints. This is an optional parameter that
-    defaults to 0.
-
-    DispatchWater[wc, t] is a variable that represents how much water is
-    flowing through each water connection at each timepoint. The lower bound is
-    m.min_eco_flow[wc, t] and the upper bound is m.wc_capacity[wc].
-
-    Enforce_Wnode_Balance[(wn, t) for (wn, t) in WNODE_TPS]
-    is a constraint that enforces conservation of mass at water nodes. This
-    accounts for any spills at sink nodes, or any change in reservoir volume
-    between one timepoint and the next. This also links the reservoir volumes
-    between timepoints, and enforces the final reservoir volume constraint.
-
-    HYDRO_GENS is a subset of GENERATION_PROJECTS which are to be linked with the
-    hydraulic system. Both reservoir generators as well as hydroelectric
-    projects in series must be specified as HYDRO_GENS and will be
-    treated the same. Members of this set may be abbreviated as hproj.
-
-    HYDRO_GEN_TPS is a subset of GEN_TPS only with
-    projects that belong to the HYDRO_GENS set. This set is used to
-    index the electricity generation decisions.
+    timepoint, specified in cubic meters per second. The parameter is indexed by
+    timepoint to allow for representation of seasonal or hourly ecological or
+    social constraints. This is an optional parameter that defaults to 0.
+
+    DispatchWater[wc, t] is a variable that represents how much water is flowing
+    through each water connection at each timepoint, in cubic meters per second.
+    The lower bound is m.min_eco_flow[wc, t] and the upper bound is
+    m.wc_capacity[wc].
+
+    Enforce_Wnode_Balance[(wn, t) for (wn, t) in WNODE_TPS] is a constraint that
+    enforces conservation of mass at water nodes. This accounts for any spills
+    at sink nodes, or any change in reservoir volume between one timepoint and
+    the next. This also links the reservoir volumes between timepoints, and
+    enforces the final reservoir volume constraint.
+
+    HYDRO_GENS is a subset of GENERATION_PROJECTS which are to be linked with
+    the hydraulic system. Both reservoir generators as well as hydroelectric
+    projects in series must be specified as HYDRO_GENS and will be treated the
+    same. Members of this set may be abbreviated as hproj.
+
+    HYDRO_GEN_TPS is a subset of GEN_TPS only with projects that belong to the
+    HYDRO_GENS set. This set is used to index the electricity generation
+    decisions.
 
     hydro_efficiency[hproj] is a parameter that specifies the hydraulic
-    efficiency of a project, in units of MW/(cubic meters per second).
-    The amount of power generated by a hydroelectric generator with a
-    certain flow depends on the water head. This creates a non linear
-    relationship between the generated power per water flow and the volume
-    of stored water. In this module the efficiency is assumed to be a
-    constant for each project, to keep the problem linear.
-
-    hydraulic_location[hproj] is a parameter that specifies the water
-    connection in which each hydro project is located. Multiple projects
-    may be located at the same connection, which allows modeling of
-    cascading generation.
-
-    TurbinateFlow[hg, t] is a variable that represents the water flow,
-    in cubic meters per second, that is passed through the turbines of each
-    project at each timepoint. This is the flow that is used to generate
-    electricity.
-
-    SpillFlow[hg, t] is a variable that represents the water flow,
-    in cubic meters per second, that is spilled by each project at each
-    timepoint. All spilled water is considered to be returned to the same
-    water connection from which it was originally extracted.
+    efficiency of a project, in units of MW/(cubic meters per second). The
+    amount of power generated by a hydroelectric generator with a certain flow
+    depends on the water head. This creates a non linear relationship between
+    the generated power per water flow and the volume of stored water. In this
+    module the efficiency is assumed to be a constant for each project, to keep
+    the problem linear.
+
+    hydraulic_location[hproj] is a parameter that specifies the water connection
+    in which each hydro project is located. Multiple projects may be located at
+    the same connection, which allows modeling of cascading generation.
+
+    TurbinateFlow[hg, t] is a variable that represents the water flow, in cubic
+    meters per second, that is passed through the turbines of each project at
+    each timepoint. This is the flow that is used to generate electricity.
+
+    SpillFlow[hg, t] is a variable that represents the water flow, in cubic
+    meters per second, that is spilled by each project at each timepoint. All
+    spilled water is considered to be returned to the same water connection from
+    which it was originally extracted.
 
     Enforce_Hydro_Generation[hg, t] is the constraint that forces power
-    generation at each hydro project to be equal to the flow of water that
-    goes through its turbines, times its hydro efficiency. This relation
-    is observed at each timepoint.
+    generation at each hydro project to be equal to the flow of water that goes
+    through its turbines, times its hydro efficiency. This relation is observed
+    at each timepoint.
 
     Enforce_Hydro_Extraction[hg, t] is the constraint that mantains the
-    conservation of mass at each project's water extraction point, so that
-    the sum of the flows that go through its turbines and the one that is
-    spilled are equal to the water that is flowing at each timepoint through
-    the water connection where it is located.
+    conservation of mass at each project's water extraction point, so that the
+    sum of the flows that go through its turbines and the one that is spilled
+    are equal to the water that is flowing at each timepoint through the water
+    connection where it is located.
 
     -----
     TODO:
     -Implement pumped storage
 
-    -Allow setting the water spillage cost as a parameter. The default
-    of 10000 US$/cumecshould prevent significant water spillage in
-    non-sink nodes in mostcases. Nonetheless, some users could want to
-    lower the penalties forsome nodes in order to get faster solution
-    times, and other could want to raise them to avoid spilling completely.
+    -Allow setting the water spillage cost as a parameter. The default of 10000
+    US$/cumec should prevent significant water spillage in non-sink nodes in
+    most cases. Nonetheless, some users could want to lower the penalties for
+    some nodes in order to get faster solution times, and others could want to
+    raise them to avoid spilling completely.
 
     """
     #################
     # Nodes of the water network
     mod.WATER_NODES = Set(dimen=1)
     mod.WNODE_TPS = Set(dimen=2, initialize=lambda m: m.WATER_NODES * m.TIMEPOINTS)
     mod.wnode_constant_inflow = Param(
@@ -409,19 +395,21 @@
             for wn in m.WATER_NODES
             if not m.wn_is_sink[wn]
         ),
     )
     mod.Cost_Components_Per_TP.append("NodeSpillageCosts")
 
     ################
-    # Hydro projects
+    # Hydro projects and available timepoints
     mod.HYDRO_GENS = Set(dimen=1, within=mod.GENERATION_PROJECTS)
     mod.HYDRO_GEN_TPS = Set(
-        dimen=2, initialize=mod.GEN_TPS, filter=lambda m, g, t: g in m.HYDRO_GENS
+        dimen=2,
+        initialize=lambda m: ((g, tp) for g in m.HYDRO_GENS for tp in m.TPS_FOR_GEN[g]),
     )
+
     mod.hydro_efficiency = Param(mod.HYDRO_GENS, within=NonNegativeReals)
     mod.hydraulic_location = Param(mod.HYDRO_GENS, within=mod.WATER_CONNECTIONS)
     mod.TurbinateFlow = Var(mod.HYDRO_GEN_TPS, within=NonNegativeReals)
     mod.SpillFlow = Var(mod.HYDRO_GEN_TPS, within=NonNegativeReals)
     mod.Enforce_Hydro_Generation = Constraint(
         mod.HYDRO_GEN_TPS,
         rule=lambda m, g, t: (
@@ -466,15 +454,15 @@
             mod.wnode_constant_inflow,
             mod.wnode_constant_consumption,
         ),
     )
     switch_data.load_aug(
         optional=True,
         filename=os.path.join(inputs_dir, "water_node_tp_flows.csv"),
-        optional_params=["mod.wnode_tp_inflow", "mod.wnode_tp_consumption"],
+        optional_params=["wnode_tp_inflow", "wnode_tp_consumption"],
         param=(mod.wnode_tp_inflow, mod.wnode_tp_consumption),
     )
     switch_data.load_aug(
         filename=os.path.join(inputs_dir, "reservoirs.csv"),
         index=mod.RESERVOIRS,
         param=(
             mod.res_min_vol,
@@ -487,15 +475,15 @@
         raise NotImplementedError(
             "Code needs to be added to hydro_system module to enforce "
             "reservoir volume limits per timepoint."
         )
     switch_data.load_aug(
         filename=os.path.join(inputs_dir, "reservoir_tp_data.csv"),
         optional=True,
-        optional_params=["mod.res_max_vol_tp", "mod.res_min_vol_tp"],
+        optional_params=["res_max_vol_tp", "res_min_vol_tp"],
         param=(mod.res_max_vol_tp, mod.res_min_vol_tp),
     )
     switch_data.load_aug(
         filename=os.path.join(inputs_dir, "water_connections.csv"),
         index=mod.WATER_CONNECTIONS,
         param=(mod.water_node_from, mod.water_node_to, mod.wc_capacity),
     )
```

### Comparing `switch_model-2.0.7/switch_model/generators/extensions/storage.py` & `switch_model-2.0.8/switch_model/generators/extensions/storage.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,94 +22,103 @@
 
 
 def define_components(mod):
     """
 
     STORAGE_GENS is the subset of projects that can provide energy storage.
 
-    STORAGE_GEN_BLD_YRS is the subset of GEN_BLD_YRS, restricted
-    to storage projects.
+    STORAGE_GEN_BLD_YRS is the subset of GEN_BLD_YRS, restricted to storage
+    projects.
 
-    gen_storage_efficiency[STORAGE_GENS] describes the round trip
-    efficiency of a storage technology. A storage technology that is 75
-    percent efficient would have a storage_efficiency of .75. If 1 MWh
-    was stored in such a storage project, 750 kWh would be available for
-    extraction later. Internal leakage or energy dissipation of storage
-    technologies is assumed to be neglible, which is consistent with
-    short-duration storage technologies currently on the market which
-    tend to consume stored power within 1 day. If a given storage
-    technology has significant internal discharge when it stores power
-    for extended time perios, then those behaviors will need to be
-    modeled in more detail.
-
-    gen_store_to_release_ratio[STORAGE_GENS] describes the maximum rate
-    that energy can be stored, expressed as a ratio of discharge power
-    capacity. This is an optional parameter and will default to 1. If a
-    storage project has 1 MW of dischage capacity and a gen_store_to_release_ratio
-    of 1.2, then it can consume up to 1.2 MW of power while charging.
-
-    gen_storage_energy_to_power_ratio[STORAGE_GENS], if specified, restricts
-    the storage capacity (in MWh) to be a fixed multiple of the output
-    power (in MW), i.e., specifies a particular number of hours of
-    storage capacity. Omit this column or specify "." to allow Switch
-    to choose the energy/power ratio. (Note: gen_storage_energy_overnight_cost
-    or gen_overnight_cost should often be set to 0 when using this.)
-
-    gen_storage_max_cycles_per_year[STORAGE_GENS], if specified, restricts
-    the number of charge/discharge cycles each storage project can perform
-    per year; one cycle is defined as discharging an amount of energy
-    equal to the storage capacity of the project.
-
-    gen_storage_energy_overnight_cost[(g, bld_yr) in
-    STORAGE_GEN_BLD_YRS] is the overnight capital cost per MWh of
-    energy capacity for building the given storage technology installed in the
-    given investment period. This is only defined for storage technologies.
-    Note that this describes the energy component and the overnight_cost
-    describes the power component.
-
-    build_gen_energy_predetermined[(g, bld_yr) in
-    PREDETERMINED_GEN_BLD_YRS] is the amount of storage that has either been
-    installed previously, or is slated for installation and is not a free
-    decision variable. This is analogous to build_gen_predetermined, but in
-    units of energy of storage capacity (MWh) rather than power (MW).
-
-    BuildStorageEnergy[(g, bld_yr) in STORAGE_GEN_BLD_YRS]
-    is a decision of how much energy capacity to build onto a storage
-    project. This is analogous to BuildGen, but for energy rather than power.
-
-    StorageEnergyInstallCosts[PERIODS] is an expression of the
-    annual costs incurred by the BuildStorageEnergy decision.
-
-    StorageEnergyCapacity[g, period] is an expression describing the
-    cumulative available energy capacity of BuildStorageEnergy. This is
-    analogous to GenCapacity.
+    gen_storage_efficiency[STORAGE_GENS] describes the round trip efficiency of
+    a storage technology. A storage technology that is 75 percent efficient
+    would have a storage_efficiency of .75. If 1 MWh was stored in such a
+    storage project, 750 kWh would be available for extraction later. Internal
+    leakage or energy dissipation of storage technologies is assumed to be
+    neglible, which is consistent with short-duration storage technologies
+    currently on the market which tend to consume stored power within 1 day. If
+    a given storage technology has significant internal discharge when it stores
+    power for extended time perios, then those behaviors will need to be modeled
+    in more detail.
+
+    gen_store_to_release_ratio[STORAGE_GENS] describes the maximum rate that
+    energy can be stored, expressed as a ratio of discharge power capacity. This
+    is an optional parameter and will default to 1. If a storage project has 1
+    MW of dischage capacity and a gen_store_to_release_ratio of 1.2, then it can
+    consume up to 1.2 MW of power while charging.
+
+    gen_storage_energy_to_power_ratio[STORAGE_GENS], if specified, restricts the
+    storage capacity (in MWh) to be a fixed multiple of the output power (in
+    MW), i.e., specifies a particular number of hours of storage capacity. Omit
+    this column or specify "." to allow Switch to choose the energy/power ratio.
+    (Note: gen_storage_energy_overnight_cost or gen_overnight_cost should often
+    be set to 0 when using this.)
+
+    gen_storage_max_cycles_per_year[STORAGE_GENS], if specified, restricts the
+    number of charge/discharge cycles each storage project can perform per year;
+    one cycle is defined as discharging an amount of energy equal to the storage
+    capacity of the project.
+
+    gen_storage_energy_overnight_cost[(g, bld_yr) in STORAGE_GEN_BLD_YRS] is the
+    overnight capital cost per MWh of energy capacity for building the given
+    storage technology installed in the given investment period. This is only
+    defined for storage technologies. Note that this describes the energy
+    component and the overnight_cost describes the power component.
+
+    gen_storage_energy_fixed_om[(g, bld_yr) in STORAGE_GEN_BLD_YRS] is the
+    annual fixed operations & maintenance cost per MWh of energy capacity
+    installed. This is charged every year over the life of the storage project,
+    whether it is operated or not. It should be in units of real dollars per
+    year per MWh of capacity. This should only be defined for storage
+    technologies; it will be ignored for non-storage generators. Note that this
+    shows the cost per unit of energy capacity (i.e., batteries) and
+    gen_fixed_om shows the cost per unit of power capacity (i.e. inverters).
+    Note: there is no gen_storage_energy_variable_om parameter; variable O&M for
+    the storage component should be included in variable O&M for the power
+    component (gen_fixed_om).
+
+    build_gen_energy_predetermined[(g, bld_yr) in PREDETERMINED_GEN_BLD_YRS] is
+    the amount of storage that has either been installed previously, or is
+    slated for installation and is not a free decision variable. This is
+    analogous to build_gen_predetermined, but in units of energy of storage
+    capacity (MWh) rather than power (MW).
+
+    BuildStorageEnergy[(g, bld_yr) in STORAGE_GEN_BLD_YRS] is a decision of how
+    much energy capacity to build onto a storage project. This is analogous to
+    BuildGen, but for energy rather than power.
+
+    StorageEnergyInstallCosts[PERIODS] is an expression of the annual costs
+    incurred by the BuildStorageEnergy decision.
+
+    StorageEnergyCapacity[g, period] is an expression describing the cumulative
+    available energy capacity of BuildStorageEnergy. This is analogous to
+    GenCapacity.
 
-    STORAGE_GEN_TPS is the subset of GEN_TPS,
-    restricted to storage projects.
+    STORAGE_GEN_TPS is the subset of GEN_TPS, restricted to storage projects.
 
-    ChargeStorage[(g, t) in STORAGE_GEN_TPS] is a dispatch
-    decision of how much to charge a storage project in each timepoint.
+    ChargeStorage[(g, t) in STORAGE_GEN_TPS] is a dispatch decision of how much
+    to charge a storage project in each timepoint.
 
     StorageNetCharge[LOAD_ZONE, TIMEPOINT] is an expression describing the
     aggregate impact of ChargeStorage in each load zone and timepoint.
 
-    Charge_Storage_Upper_Limit[(g, t) in STORAGE_GEN_TPS]
-    constrains ChargeStorage to available power capacity (accounting for
+    Charge_Storage_Upper_Limit[(g, t) in STORAGE_GEN_TPS] constrains
+    ChargeStorage to available power capacity (accounting for
     gen_store_to_release_ratio)
 
-    StateOfCharge[(g, t) in STORAGE_GEN_TPS] is a variable
-    for tracking state of charge. This value stores the state of charge at
-    the end of each timepoint for each storage project.
-
-    Track_State_Of_Charge[(g, t) in STORAGE_GEN_TPS] constrains
-    StateOfCharge based on the StateOfCharge in the previous timepoint,
-    ChargeStorage and DispatchGen.
+    StateOfCharge[(g, t) in STORAGE_GEN_TPS] is a variable for tracking state of
+    charge. This value stores the state of charge at the end of each timepoint
+    for each storage project.
+
+    Track_State_Of_Charge[(g, t) in STORAGE_GEN_TPS] constrains StateOfCharge
+    based on the StateOfCharge in the previous timepoint, ChargeStorage and
+    DispatchGen.
 
-    State_Of_Charge_Upper_Limit[(g, t) in STORAGE_GEN_TPS]
-    constrains StateOfCharge based on installed energy capacity.
+    State_Of_Charge_Upper_Limit[(g, t) in STORAGE_GEN_TPS] constrains
+    StateOfCharge based on installed energy capacity.
 
     """
 
     mod.STORAGE_GENS = Set(within=mod.GENERATION_PROJECTS, dimen=1)
     mod.STORAGE_GEN_PERIODS = Set(
         dimen=2,
         within=mod.GEN_PERIODS,
@@ -139,14 +148,18 @@
         mod.STORAGE_GEN_BLD_YRS, within=NonNegativeReals
     )
     mod.min_data_check("gen_storage_energy_overnight_cost")
     mod.build_gen_energy_predetermined = Param(
         mod.PREDETERMINED_GEN_BLD_YRS, within=NonNegativeReals
     )
 
+    mod.gen_storage_energy_fixed_om = Param(
+        mod.STORAGE_GEN_BLD_YRS, within=NonNegativeReals, default=0.0
+    )
+
     def bounds_BuildStorageEnergy(m, g, bld_yr):
         if (g, bld_yr) in m.build_gen_energy_predetermined:
             return (
                 m.build_gen_energy_predetermined[g, bld_yr],
                 m.build_gen_energy_predetermined[g, bld_yr],
             )
         else:
@@ -154,41 +167,45 @@
 
     mod.BuildStorageEnergy = Var(
         mod.STORAGE_GEN_BLD_YRS,
         within=NonNegativeReals,
         bounds=bounds_BuildStorageEnergy,
     )
 
-    # Summarize capital costs of energy storage for the objective function
-    # Note: A bug in to 2.0.0b3 - 2.0.5, assigned costs that were several times
-    # too high
+    # Summarize capital and O&M costs of energy storage for the objective
+    # function
     mod.StorageEnergyCapitalCost = Expression(
         mod.STORAGE_GENS,
         mod.PERIODS,
         rule=lambda m, g, p: sum(
             m.BuildStorageEnergy[g, bld_yr]
             * m.gen_storage_energy_overnight_cost[g, bld_yr]
             * crf(m.interest_rate, m.gen_max_age[g])
+            # apply to all vintages (bld_yr) of storage that are active in the
+            # current period (p)
+            for bld_yr in m.BLD_YRS_FOR_GEN_PERIOD[g, p]
+        ),
+    )
+    mod.StorageEnergyFixedOMCost = Expression(
+        mod.STORAGE_GENS,
+        mod.PERIODS,
+        rule=lambda m, g, p: sum(
+            m.BuildStorageEnergy[g, bld_yr] * m.gen_storage_energy_fixed_om[g, bld_yr]
             for bld_yr in m.BLD_YRS_FOR_GEN_PERIOD[g, p]
         ),
     )
     mod.StorageEnergyFixedCost = Expression(
         mod.PERIODS,
-        rule=lambda m, p: sum(m.StorageEnergyCapitalCost[g, p] for g in m.STORAGE_GENS),
+        rule=lambda m, p: sum(
+            m.StorageEnergyCapitalCost[g, p] + m.StorageEnergyFixedOMCost[g, p]
+            for g in m.STORAGE_GENS
+        ),
     )
     mod.Cost_Components_Per_Period.append("StorageEnergyFixedCost")
 
-    # 2.0.0b3 code:
-    # mod.StorageEnergyInstallCosts = Expression(
-    # mod.PERIODS,
-    # rule=lambda m, p: sum(m.BuildStorageEnergy[g, bld_yr] *
-    #            m.gen_storage_energy_overnight_cost[g, bld_yr] *
-    #            crf(m.interest_rate, m.gen_max_age[g])
-    #            for (g, bld_yr) in m.STORAGE_GEN_BLD_YRS))
-
     mod.StorageEnergyCapacity = Expression(
         mod.STORAGE_GENS,
         mod.PERIODS,
         rule=lambda m, g, period: sum(
             m.BuildStorageEnergy[g, bld_yr]
             for bld_yr in m.BLD_YRS_FOR_GEN_PERIOD[g, period]
         ),
@@ -221,19 +238,22 @@
     # Register net charging with zonal energy balance. Discharging is already
     # covered by DispatchGen.
     mod.Zone_Power_Withdrawals.append("StorageNetCharge")
 
     # use fixed energy/power ratio (# hours of capacity) when specified
     mod.Enforce_Fixed_Energy_Storage_Ratio = Constraint(
         mod.STORAGE_GEN_BLD_YRS,
-        rule=lambda m, g, y: Constraint.Skip
-        if m.gen_storage_energy_to_power_ratio[g] == float("inf")  # no value specified
-        else (
-            m.BuildStorageEnergy[g, y]
-            == m.gen_storage_energy_to_power_ratio[g] * m.BuildGen[g, y]
+        rule=lambda m, g, y: (
+            Constraint.Skip
+            if m.gen_storage_energy_to_power_ratio[g]
+            == float("inf")  # no value specified
+            else (
+                m.BuildStorageEnergy[g, y]
+                == m.gen_storage_energy_to_power_ratio[g] * m.BuildGen[g, y]
+            )
         ),
     )
 
     def Charge_Storage_Upper_Limit_rule(m, g, t):
         return (
             m.ChargeStorage[g, t]
             <= m.DispatchUpperLimit[g, t] * m.gen_store_to_release_ratio[g]
@@ -268,41 +288,74 @@
     )
 
     # batteries can only complete the specified number of cycles per year, averaged over each period
     mod.Battery_Cycle_Limit = Constraint(
         mod.STORAGE_GEN_PERIODS,
         rule=lambda m, g, p:
         # solvers sometimes perform badly with infinite constraint
-        Constraint.Skip
-        if m.gen_storage_max_cycles_per_year[g] == float("inf")
-        else (
-            sum(
-                m.DispatchGen[g, tp] * m.tp_duration_hrs[tp]
-                for tp in m.TPS_IN_PERIOD[p]
+        (
+            Constraint.Skip
+            if m.gen_storage_max_cycles_per_year[g] == float("inf")
+            else (
+                sum(
+                    m.DispatchGen[g, tp] * m.tp_duration_hrs[tp]
+                    for tp in m.TPS_IN_PERIOD[p]
+                )
+                <= m.gen_storage_max_cycles_per_year[g]
+                * m.StorageEnergyCapacity[g, p]
+                * m.period_length_years[p]
             )
-            <= m.gen_storage_max_cycles_per_year[g]
-            * m.StorageEnergyCapacity[g, p]
-            * m.period_length_years[p]
         ),
     )
 
+    # Some projects are retired before the first study period, so they don't
+    # appear in the objective function or any constraints. In this case, pyomo
+    # may leave the variable value undefined even after a solve instead of
+    # assigning a value within the allowed range. This causes errors in the
+    # Progressive Hedging code, which expects every variable to have a value
+    # after the solve. So as a starting point we assign an appropriate value to
+    # all the existing projects here.
+    def BuildStorageEnergy_assign_default_value(m, g, bld_yr):
+        if (g, bld_yr) in m.build_gen_energy_predetermined:
+            m.BuildStorageEnergy[g, bld_yr] = m.build_gen_energy_predetermined[
+                g, bld_yr
+            ]
+        elif g in m.STORAGE_GENS and m.gen_storage_energy_to_power_ratio[g] == float(
+            "inf"
+        ):
+            raise ValueError(
+                f"For storage generator g='{g}', gen_build_predetermined[g, {bld_yr}] "
+                f"has been specified, but not "
+                f"gen_build_energy_predetermined[g, {bld_yr}] or "
+                f"gen_storage_energy_to_power_ratio[g]."
+            )
+
+    mod.BuildStorageEnergy_assign_default_value = BuildAction(
+        mod.PREDETERMINED_GEN_BLD_YRS, rule=BuildStorageEnergy_assign_default_value
+    )
+
+    # TODO: expand m.PREDETERMINED_GEN_BLD_YRS to include generators with energy
+    # specified but not power, and in these cases, raise an error if
+    # energy_to_power_ratio is not specified.
+
 
 def load_inputs(mod, switch_data, inputs_dir):
     """
 
     Import storage parameters. Optional columns are noted with a *.
 
     gen_info.csv
         GENERATION_PROJECT, ...
         gen_storage_efficiency, gen_store_to_release_ratio*,
         gen_storage_energy_to_power_ratio*, gen_storage_max_cycles_per_year*
 
     gen_build_costs.csv
         GENERATION_PROJECT, build_year, ...
         gen_storage_energy_overnight_cost
+        gen_storage_energy_fixed_om*
 
     gen_build_predetermined.csv
         GENERATION_PROJECT, build_year, ...,
         build_gen_energy_predetermined*
 
     """
 
@@ -329,15 +382,15 @@
     # Base the set of storage projects on storage efficiency being specified.
     # TODO: define this in a more normal way
     switch_data.data()["STORAGE_GENS"] = {
         None: list(switch_data.data(name="gen_storage_efficiency").keys())
     }
     switch_data.load_aug(
         filename=os.path.join(inputs_dir, "gen_build_costs.csv"),
-        param=(mod.gen_storage_energy_overnight_cost),
+        param=(mod.gen_storage_energy_overnight_cost, mod.gen_storage_energy_fixed_om),
     )
     switch_data.load_aug(
         optional=True,
         filename=os.path.join(inputs_dir, "gen_build_predetermined.csv"),
         param=(mod.build_gen_energy_predetermined,),
     )
```

### Comparing `switch_model-2.0.7/switch_model/hawaii/batteries.py` & `switch_model-2.0.8/switch_model/hawaii/batteries.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/hawaii/batteries_fixed_calendar_life.py` & `switch_model-2.0.8/switch_model/hawaii/batteries_fixed_calendar_life.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/hawaii/demand_response_no_reserves.py` & `switch_model-2.0.8/switch_model/hawaii/demand_response_no_reserves.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/hawaii/demand_response_simple.py` & `switch_model-2.0.8/switch_model/hawaii/demand_response_simple.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/hawaii/emission_rules.py` & `switch_model-2.0.8/switch_model/hawaii/emission_rules.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/hawaii/ev.py` & `switch_model-2.0.8/switch_model/hawaii/ev.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/hawaii/ev_advanced.py` & `switch_model-2.0.8/switch_model/hawaii/ev_advanced.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/hawaii/fed_subsidies.py` & `switch_model-2.0.8/switch_model/hawaii/fed_subsidies.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/hawaii/fuel_markets_expansion.py` & `switch_model-2.0.8/switch_model/hawaii/fuel_markets_expansion.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/hawaii/heco_outlook_2019.py` & `switch_model-2.0.8/switch_model/hawaii/heco_outlook_2019.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/hawaii/heco_outlook_2020_06.py` & `switch_model-2.0.8/switch_model/hawaii/heco_outlook_2020_06.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/hawaii/heco_outlook_2020_08.py` & `switch_model-2.0.8/switch_model/hawaii/heco_outlook_2020_08.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/hawaii/heco_plan_2020_06.py` & `switch_model-2.0.8/switch_model/hawaii/heco_plan_2020_06.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/hawaii/heco_plan_2020_08.py` & `switch_model-2.0.8/switch_model/hawaii/heco_plan_2020_08.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/hawaii/hi_spinning_reserves.py` & `switch_model-2.0.8/switch_model/hawaii/hi_spinning_reserves.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/hawaii/hydrogen.py` & `switch_model-2.0.8/switch_model/hawaii/hydrogen.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 
 def define_components(m):
     if not m.options.no_hydrogen:
         define_hydrogen_components(m)
 
 
 def define_hydrogen_components(m):
-
     # electrolyzer details
     m.hydrogen_electrolyzer_capital_cost_per_mw = Param(within=NonNegativeReals)
     m.hydrogen_electrolyzer_fixed_cost_per_mw_year = Param(
         within=NonNegativeReals, default=0.0
     )
     # assumed to include any refurbishment needed
     m.hydrogen_electrolyzer_variable_cost_per_kg = Param(
@@ -236,14 +235,16 @@
     m.Hydrogen_FC_Reserve_Electrolyzer_Limit = Constraint(
         m.LOAD_ZONES,
         m.TIMEPOINTS,
         rule=lambda m, z, t: m.HydrogenFuelCellMaxReservePower[z, t]
         <= 2.0 * m.ElectrolyzerCapacityMW[z, m.tp_period[t]],
     )
 
+    # TODO: add fuel cells to planning reserves by adding them to m.CAPACITY_FOR_RESERVES
+
     # how much extra power could hydrogen equipment produce or absorb on short notice (for reserves)
     m.HydrogenSlackUp = Expression(
         m.LOAD_ZONES,
         m.TIMEPOINTS,
         rule=lambda m, z, t: m.RunElectrolyzerMW[z, t]
         + m.LiquifyHydrogenMW[z, t]
         + m.HydrogenFuelCellMaxReservePower[z, t]
```

### Comparing `switch_model-2.0.7/switch_model/hawaii/lake_wilson.py` & `switch_model-2.0.8/switch_model/hawaii/lake_wilson.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/hawaii/lng_conversion.py` & `switch_model-2.0.8/switch_model/hawaii/lng_conversion.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/hawaii/no_central_pv.py` & `switch_model-2.0.8/switch_model/hawaii/no_central_pv.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/hawaii/no_renewables.py` & `switch_model-2.0.8/switch_model/hawaii/no_renewables.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/hawaii/no_wind.py` & `switch_model-2.0.8/switch_model/hawaii/no_wind.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/hawaii/oahu_plants.py` & `switch_model-2.0.8/switch_model/hawaii/oahu_plants.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/hawaii/psip_2016_04.py` & `switch_model-2.0.8/switch_model/hawaii/psip_2016_04.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/hawaii/psip_2016_12.py` & `switch_model-2.0.8/switch_model/hawaii/psip_2016_12.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/hawaii/pumped_hydro.py` & `switch_model-2.0.8/switch_model/hawaii/pumped_hydro.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/hawaii/register_hi_storage_reserves.py` & `switch_model-2.0.8/switch_model/hawaii/register_hi_storage_reserves.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/hawaii/reserves.py` & `switch_model-2.0.8/switch_model/hawaii/reserves.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/hawaii/rps.py` & `switch_model-2.0.8/switch_model/hawaii/rps.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/hawaii/save_results.py` & `switch_model-2.0.8/switch_model/hawaii/save_results.py`

 * *Files 4% similar despite different names*

```diff
@@ -226,64 +226,93 @@
         s
         for s in m.Zone_Power_Injections
         if s not in {"ZoneTotalCentralDispatch", "ZoneTotalDistributedDispatch"}
     )
     avg_ts_scale = float(sum(m.ts_scale_to_year[ts] for ts in m.TIMESERIES)) / len(
         m.TIMESERIES
     )
+    # do some lookups in advance to avoid re-filtering every timepoint
+    gens_by_fuel_and_zone = {
+        (f, z): [g for g in m.GENS_BY_FUEL[f] if m.gen_load_zone[g] == z]
+        for f in m.FUELS
+        for z in m.LOAD_ZONES
+    }
+    gens_by_non_fuel_energy_source_and_zone = {
+        (s, z): [
+            g for g in m.GENS_BY_NON_FUEL_ENERGY_SOURCE[s] if m.gen_load_zone[g] == z
+        ]
+        for z in m.LOAD_ZONES
+        for s in m.NON_FUEL_ENERGY_SOURCES
+    }
+    gens_by_non_fuel_tech_and_zone = {
+        (tech, z): [g for g in m.GENS_BY_TECHNOLOGY[tech] if m.gen_load_zone[g] == z]
+        for tech in non_fuel_techs
+        for z in m.LOAD_ZONES
+    }
+
     util.write_table(
         m,
         m.LOAD_ZONES,
         m.TIMEPOINTS,
         output_file=os.path.join(outputs_dir, "energy_sources{t}.csv".format(t=tag)),
         headings=("load_zone", "period", "timepoint_label")
         + tuple(m.FUELS)
         + tuple(m.NON_FUEL_ENERGY_SOURCES)
         + non_fuel_techs
         + tuple("curtail_" + s for s in m.NON_FUEL_ENERGY_SOURCES)
         + tuple(m.Zone_Power_Injections)
         + tuple(m.Zone_Power_Withdrawals)
+        + (
+            tuple(m.Distributed_Power_Withdrawals)
+            if hasattr(m, "Distributed_Power_Withdrawals")
+            else tuple()
+        )
         + ("spinning_reserve_provision", "spinning_reserve_requirement")
         + ("marginal_cost", "peak_day"),
         values=lambda m, z, t: (z, m.tp_period[t], m.tp_timestamp[t])
         + tuple(
             sum(
-                DispatchGenByFuel(m, p, t, f)
-                for p in m.GENS_BY_FUEL[f]
-                if (p, t) in m.GEN_TPS and m.gen_load_zone[p] == z
+                DispatchGenByFuel(m, g, t, f)
+                for g in gens_by_fuel_and_zone[f, z]
+                if (g, t) in m.GEN_TPS
             )
             for f in m.FUELS
         )
         + tuple(
             sum(
-                util.get(m.DispatchGen, (p, t), 0.0)
-                for p in m.GENS_BY_NON_FUEL_ENERGY_SOURCE[s]
-                if m.gen_load_zone[p] == z
+                util.get(m.DispatchGen, (g, t), 0.0)
+                for g in gens_by_non_fuel_energy_source_and_zone[s, z]
             )
             for s in m.NON_FUEL_ENERGY_SOURCES
         )
         + tuple(
             sum(
                 util.get(m.DispatchGen, (g, t), 0.0)
-                for g in m.GENS_BY_TECHNOLOGY[tech]
-                if m.gen_load_zone[g] == z
+                for g in gens_by_non_fuel_tech_and_zone[tech, z]
             )
             for tech in non_fuel_techs
         )
         + tuple(
             sum(
-                util.get(m.DispatchUpperLimit, (p, t), 0.0)
-                - util.get(m.DispatchGen, (p, t), 0.0)
-                for p in m.GENS_BY_NON_FUEL_ENERGY_SOURCE[s]
-                if m.gen_load_zone[p] == z
+                util.get(m.DispatchUpperLimit, (g, t), 0.0)
+                - util.get(m.DispatchGen, (g, t), 0.0)
+                for g in gens_by_non_fuel_energy_source_and_zone[s, z]
             )
             for s in m.NON_FUEL_ENERGY_SOURCES
         )
         + tuple(getattr(m, component)[z, t] for component in m.Zone_Power_Injections)
         + tuple(getattr(m, component)[z, t] for component in m.Zone_Power_Withdrawals)
+        + (
+            tuple(
+                getattr(m, component)[z, t]
+                for component in m.Distributed_Power_Withdrawals
+            )
+            if hasattr(m, "Distributed_Power_Withdrawals")
+            else tuple()
+        )
         + (  # save spinning reserve requirements and provisions; note: this assumes one zone per balancing area
             (
                 spinning_reserve_provisions[m.zone_balancing_area[z], t],
                 spinning_reserve_requirements[m.zone_balancing_area[z], t],
             )
             if hasattr(m, "Spinning_Reserve_Up_Requirements")
             else (0.0, 0.0)
@@ -420,15 +449,15 @@
             )
         )
     )
     active_periods_for_gen = defaultdict(set)
     used_cap = getattr(
         m, "CommitGen", m.DispatchGen
     )  # use CommitGen if available, otherwise DispatchGen
-    for (g, tp) in m.GEN_TPS:
+    for g, tp in m.GEN_TPS:
         if value(used_cap[g, tp]) > 0.001:
             active_periods_for_gen[g].add(m.tp_period[tp])
     # add the periods between the first and last active period if capacity was available then
     operate_gen_in_period = set()
     for g, active_periods in active_periods_for_gen.items():
         start = min(active_periods)
         end = max(active_periods)
@@ -482,14 +511,20 @@
         output_file=os.path.join(
             outputs_dir, "capacity_by_technology_vertical{t}.csv".format(t=tag)
         ),
         headings=("load_zone", "technology", "period", "capacity"),
         values=lambda m, z, t, pe: (z, t, pe, tech_cap[z, t, pe]),
     )
 
+    built_gens_for_tech_and_zone = {
+        (t, z): [] for z in m.LOAD_ZONES for t in built_tech
+    }
+    for g in built_gens:
+        built_gens_for_tech_and_zone[m.gen_tech[g], m.gen_load_zone[g]].append(g)
+
     util.write_table(
         m,
         m.LOAD_ZONES,
         m.PERIODS,
         output_file=os.path.join(
             outputs_dir, "capacity_used_by_technology{t}.csv".format(t=tag)
         ),
@@ -497,16 +532,15 @@
         values=lambda m, z, pe: (
             z,
             pe,
         )
         + tuple(
             sum(
                 (m.GenCapacity[g, pe] if ((g, pe) in operate_gen_in_period) else 0.0)
-                for g in built_gens
-                if m.gen_tech[g] == t and m.gen_load_zone[g] == z
+                for g in built_gens_for_tech_and_zone[t, z]
             )
             for t in built_tech
         )
         + (
             m.Pumped_Hydro_Capacity_MW[z, pe]
             if hasattr(m, "Pumped_Hydro_Capacity_MW")
             else 0,
@@ -581,21 +615,21 @@
             outputs_dir, "production_by_technology{t}.csv".format(t=tag)
         ),
         headings=("load_zone", "period") + built_tech + ad_hoc_sources,
         values=lambda m, z, pe: (
             z,
             pe,
         )
-        + tuple(
+        + tuple(  # total output for each gen tech in this zone/period
             sum(
-                m.DispatchGen[g, tp] * m.tp_weight_in_year[tp] * 0.001  # MWh -> GWh
-                for g in built_gens
-                if m.gen_tech[g] == t and m.gen_load_zone[g] == z
+                m.DispatchGen[g, tp] * m.tp_weight_in_year[tp]
+                for g in built_gens_for_tech_and_zone[t, z]
                 for tp in m.TPS_FOR_GEN_IN_PERIOD[g, pe]
             )
+            * 0.001  # MWh -> GWh
             for t in built_tech
         )
         + tuple(  # ad hoc techs: hydrogen, pumped storage, etc.
             sum(
                 comp[z, tp] * m.tp_weight_in_year[tp] * 0.001
                 for tp in m.TPS_IN_PERIOD[pe]
             )
```

### Comparing `switch_model-2.0.7/switch_model/hawaii/scenario_data.py` & `switch_model-2.0.8/switch_model/hawaii/scenario_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1365,15 +1365,15 @@
                 ############################################################################################
                 Error while connecting to database '{db}' on postgres server '{server}' as user '{user}'.
                 Please ensure that the following environment variables are set:
                 PGUSER = your postgres username
                 PGHOST = hostname or IP address of postgres server
                 PGDATABASE = name of switch database on this server.
                 There should also be a line like "*:*:*:<user>:<password>" in ~/.pgpass (which should be chmod 0600)
-                or in %APPDATA%\postgresql\pgpass.conf (Windows).
+                or in %APPDATA%\\postgresql\\pgpass.conf (Windows).
                 See http://www.postgresql.org/docs/9.1/static/libpq-pgpass.html for more details.
                 ############################################################################################
                 """.format(
                         server=pghost, db=pgdatabase, user=pguser
                     )
                 )
             )
```

### Comparing `switch_model-2.0.7/switch_model/hawaii/scenarios.py` & `switch_model-2.0.8/switch_model/hawaii/scenarios.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/hawaii/smooth_dispatch.py` & `switch_model-2.0.8/switch_model/hawaii/smooth_dispatch.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/hawaii/smooth_dispatch_quadratic.py` & `switch_model-2.0.8/switch_model/hawaii/smooth_dispatch_quadratic.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/hawaii/switch_patch.py` & `switch_model-2.0.8/switch_model/hawaii/switch_patch.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/hawaii/unserved_load.py` & `switch_model-2.0.8/switch_model/hawaii/unserved_load.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/hawaii/util.py` & `switch_model-2.0.8/switch_model/hawaii/util.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/main.py` & `switch_model-2.0.8/switch_model/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import sys, os
 import switch_model
 
 # print "running {} as {}.".format(__file__, __name__)
 
 
 def main():
-    cmds = ["solve", "solve-scenarios", "test", "upgrade", "--version"]
+    cmds = ["solve", "solve-scenarios", "test", "upgrade", "info", "--version"]
     if len(sys.argv) >= 2 and sys.argv[1] in cmds:
         # If users run a script from the command line, the location of the script
         # gets added to the start of sys.path; if they call a module from the
         # command line then an empty entry gets added to the start of the path,
         # indicating the current working directory. This module is often called
         # from a command-line script, but we want the current working
         # directory in the path because users may try to load local modules via
@@ -29,14 +29,16 @@
         if cmd == "--version":
             print("Switch model version " + switch_model.__version__)
             return 0
         if cmd == "solve":
             from .solve import main
         elif cmd == "solve-scenarios":
             from .solve_scenarios import main
+        elif cmd == "info":
+            from .api import info as main
         elif cmd == "test":
             from .test import main
         elif cmd == "upgrade":
             from switch_model.upgrade import main
         main()
     else:
         print(
```

### Comparing `switch_model-2.0.7/switch_model/policies/carbon_policies.py` & `switch_model-2.0.8/switch_model/policies/carbon_policies.py`

 * *Files 15% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         default=0.0,
         doc="The cost adder applied to emissions, in future dollars per metric tonne of CO2.",
     )
     model.EmissionsCosts = Expression(
         model.PERIODS,
         rule=lambda model, period: model.AnnualEmissions[period]
         * model.carbon_cost_dollar_per_tco2[period],
-        doc=("Enforces the carbon cap for generation-related emissions."),
+        doc=("Calculates the carbon cost for generation-related emissions."),
     )
     model.Cost_Components_Per_Period.append("EmissionsCosts")
 
 
 def load_inputs(model, switch_data, inputs_dir):
     """
     Typically, people will specify either carbon caps or carbon costs, but not
@@ -106,16 +106,23 @@
         # integer values, which is often a reasonable approach and should give
         # meaningful duals for the carbon cost, which occurs on a much higher
         # level).
         if (
             period in model.Enforce_Carbon_Cap
             and model.Enforce_Carbon_Cap[period] in model.dual
         ):
+            # Note: until 2023, this reported the dual directly, which was
+            # always negative because this is a <= constraint in a minimization
+            # problem (see paragraph below equ 12 in
+            # https://web.mit.edu/15.053/www/AMP-Chapter-04.pdf). Beginning in
+            # 2023, we report the absolute value, since users are generally just
+            # interested in the magnitude of the shadow price, not the direction
+            # of the constraint.
             row.append(
-                model.dual[model.Enforce_Carbon_Cap[period]]
+                abs(model.dual[model.Enforce_Carbon_Cap[period]])
                 / model.bring_annual_costs_to_base_year[period]
             )
         else:
             row.append(".")
         row.append(model.carbon_cost_dollar_per_tco2[period])
         row.append(
             model.carbon_cost_dollar_per_tco2[period] * model.AnnualEmissions[period]
```

### Comparing `switch_model-2.0.7/switch_model/policies/rps_simple.py` & `switch_model-2.0.8/switch_model/policies/rps_simple.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/reporting/__init__.py` & `switch_model-2.0.8/switch_model/reporting/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,14 +247,15 @@
         fh.write("{}\n".format(value(instance.SystemCost)))
 
 
 def save_cost_components(m, outdir):
     """
     Save values for all individual components of total system cost on NPV basis.
     """
+    # TODO: should this use bring_future_costs_to_base_year instead of bring_annual_costs_to_base_year
     cost_dict = dict()
     for annual_cost in m.Cost_Components_Per_Period:
         cost = getattr(m, annual_cost)
         # note: storing value() instead of the expression may save
         # some memory while this function runs
         cost_dict[annual_cost] = value(
             sum(cost[p] * m.bring_annual_costs_to_base_year[p] for p in m.PERIODS)
```

### Comparing `switch_model-2.0.7/switch_model/reporting/basic_exports.py` & `switch_model-2.0.8/switch_model/reporting/basic_exports.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/reporting/dump.py` & `switch_model-2.0.8/switch_model/reporting/dump.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/reporting/example_export.py` & `switch_model-2.0.8/switch_model/reporting/example_export.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/solve.py` & `switch_model-2.0.8/switch_model/solve.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 #!/usr/bin/env python
 # Copyright (c) 2015-2022 The Switch Authors. All rights reserved.
 # Licensed under the Apache License, Version 2.0, which is in the LICENSE file.
 from __future__ import print_function
 
 import logging
-import sys, os, time, shlex, re, inspect, textwrap, types, threading, json, traceback
+import sys
+import os
+import time
+import shlex
+import ast
+import re
+import inspect
+import textwrap
+import types
+import threading
+import json
+import traceback
+import argparse
+import pickle
 
 try:
     import IPython
 
     has_ipython = True
 except ImportError:
     has_ipython = False
 
-try:
-    # Python 2
-    import cPickle as pickle
-except ImportError:
-    import pickle
-
-try:
-    # Python 2
-    input = raw_input
-except NameError:
-    pass
-
 from pyomo.environ import *
 from pyomo.opt import SolverFactory, SolverStatus, TerminationCondition
 import pyomo.version
 
 import switch_model
 from switch_model.utilities import (
     create_model,
@@ -41,15 +42,14 @@
     unwrap,
     rewrap,
 )
 from switch_model.upgrade import do_inputs_need_upgrade, upgrade_inputs
 
 
 def main(args=None, return_model=False, return_instance=False):
-
     timer = StepTimer()
     if args is None:
         # combine default arguments read from options.txt file with
         # additional arguments specified on the command line
         args = get_option_file_args(extra_args=sys.argv[1:])
 
     # Get options needed before any modules are loaded
@@ -163,18 +163,14 @@
                 )
                 return -1
 
         # build a module list based on configuration options, and add
         # the current module (to register define_arguments callback)
         modules = get_module_list(args)
 
-        # Patch pyomo if needed, to allow reconstruction of expressions.
-        # This must be done before the model is constructed.
-        patch_pyomo()
-
         # Define the model
         model = create_model(modules, args=args, logger=logger)
         # Add any suffixes specified on the command line (usually only iis)
         add_extra_suffixes(model)
 
         logger.info("Model defined in {:.2f} s.".format(timer.step_time()))
 
@@ -193,14 +189,16 @@
                 raise IOError(
                     "Prior solution {} does not exist.".format(prior_solution_file)
                 )
 
         # create an instance (also reports time spent reading data and loading into model)
         logger.info("\nLoading inputs...")
         instance = model.load_inputs()
+        # steps above reported their own timing; now reset timer for next step
+        timer.step_time()
 
         #### Below here, we refer to instance instead of model ####
 
         logger.info("Executing pre-solve functions...")
         instance.pre_solve()
         logger.info(f"Completed pre-solve processing in {timer.step_time():.2f} s.")
 
@@ -251,17 +249,27 @@
                         "modules": modules,
                         "iterate_modules": instance.iterate_modules,
                     },
                     f,
                     indent=4,
                 )
 
-            if not instance.options.no_save_solution:
+            if instance.options.no_save_solution:
+                logger.warning(
+                    "\nThe --no-save-solution option is deprecated because it "
+                    "is now the default setting. This flag will raise an error "
+                    "in future versions of Switch. Please use the "
+                    "--save-solution-file option if you want to save a "
+                    "results.pickle file."
+                )
+                # no action needed, because this just requests the new default behavior
+
+            if instance.options.save_solution_file:
                 logger.info(f"\nSaving solution file...")
-                save_results(instance, instance.options.outputs_dir)
+                save_solution_file(instance, instance.options.outputs_dir)
                 logger.info(f"Saved solution file in {timer.step_time():.2f} s.")
 
         # report results
         # (repeated if model is reloaded, to automatically run any new export code)
         if not instance.options.no_post_solve:
             logger.info("\nExecuting post-solve functions...")
             instance.post_solve()
@@ -286,14 +294,20 @@
                 "Abstract model is in 'model' variable;",
                 "Solved instance is in 'instance' and 'm' variables.",
                 "Type ctrl-d or exit() to exit shell.",
                 "=" * 60,
                 "",
             ]
         )
+
+        # turn off exception interception while interacting, because that
+        # causes Python to bomb out on any error
+        switch_excepthook = sys.excepthook
+        sys.excepthook = old_excepthook
+
         # IPython support is disabled until they fix
         # https://github.com/ipython/ipython/issues/12199
         if has_ipython and False:
             banner += "\nUse tab to auto-complete"
             IPython.embed(
                 banner1=banner,
                 exit_msg="Leaving interactive interpreter, returning to program.",
@@ -303,14 +317,17 @@
             import code
 
             code.interact(
                 banner=banner,
                 local=dict(list(globals().items()) + list(locals().items())),
             )
 
+        # restore excepthook
+        sys.excepthook = switch_excepthook
+
     # return solved model for users who want to do other things with it
     return instance
 
 
 # should we show a full traceback when there is an error?
 full_traceback = False
 
@@ -366,90 +383,14 @@
 def reload_prior_solution_from_pickle(instance, pickle_file):
     with open(pickle_file, "rb") as fh:
         results = pickle.load(fh)
     instance.solutions.load_from(results)
     return instance
 
 
-patched_pyomo = False
-
-
-def patch_pyomo():
-    # patch Pyomo if needed
-    global patched_pyomo
-    if patched_pyomo:
-        return
-    patched_pyomo = True
-
-    # Pyomo 5.1.1 (and maybe others) is very slow to load prior solutions
-    # because it does a full-component search for each component name as it
-    # assigns the data. This ends up taking longer than solving the model. So we
-    # micro- patch pyomo.core.base.PyomoModel.ModelSolutions.add_solution to use
-    # Pyomo's built-in caching system for component names.
-    # TODO: create a pull request for Pyomo to do this
-    # NOTE: space inside the long quotes is significant; must match the Pyomo code
-    old_code = """
-                    for obj in instance.component_data_objects(Var):
-                        cache[obj.name] = obj
-                    for obj in instance.component_data_objects(Objective, active=True):
-                        cache[obj.name] = obj
-                    for obj in instance.component_data_objects(Constraint, active=True):
-                        cache[obj.name] = obj"""
-    new_code = """
-                    # use buffer to avoid full search of component for data object
-                    # which introduces a delay that is quadratic in model size
-                    buf=dict()
-                    for obj in instance.component_data_objects(Var):
-                        cache[obj.getname(fully_qualified=True, name_buffer=buf)] = obj
-                    for obj in instance.component_data_objects(Objective, active=True):
-                        cache[obj.getname(fully_qualified=True, name_buffer=buf)] = obj
-                    for obj in instance.component_data_objects(Constraint, active=True):
-                        cache[obj.getname(fully_qualified=True, name_buffer=buf)] = obj"""
-
-    from pyomo.core.base.PyomoModel import ModelSolutions
-
-    add_solution_code = inspect.getsource(ModelSolutions.add_solution)
-    if old_code in add_solution_code:
-        # create and inject a new version of the method
-        add_solution_code = add_solution_code.replace(old_code, new_code)
-        replace_method(ModelSolutions, "add_solution", add_solution_code)
-    elif pyomo.version.version_info[:2] >= (5, 0):
-        # We don't allow later versions of Pyomo than we've tested with, so
-        # this should only show up during testing when preparing to release a
-        # new version.
-        print(
-            "NOTE: The patch to pyomo.core.base.PyomoModel.ModelSolutions.add_solution "
-            "has been deactivated because the Pyomo source code has changed. "
-            f"Check whether this patch is still needed and edit {__file__} "
-            "accordingly."
-        )
-
-
-def replace_method(class_ref, method_name, new_source_code):
-    """
-    Replace specified class method with a compiled version of new_source_code.
-    """
-    orig_method = getattr(class_ref, method_name)
-    # compile code into a function
-    workspace = dict()
-    exec(textwrap.dedent(new_source_code), workspace)
-    new_method = workspace[method_name]
-    # create a new function with the same body, but using the old method's namespace
-    new_func = types.FunctionType(
-        new_method.__code__,
-        orig_method.__globals__,
-        orig_method.__name__,
-        orig_method.__defaults__,
-        orig_method.__closure__,
-    )
-    # note: this normal function will be automatically converted to an unbound
-    # method when it is assigned as an attribute of a class
-    setattr(class_ref, method_name, new_func)
-
-
 def reload_prior_solution_from_csvs(instance):
     """
     Assign values to all model variables from <variable>.csv files saved after
     previous solution. (Not currently used.)
     """
     import csv
 
@@ -678,15 +619,15 @@
         help="Method for Pyomo to use to communicate with solver",
     )
     # note: pyomo has a --solver-options option but it is not clear
     # whether that does the same thing as --solver-options-string so we don't reuse the same name.
     argparser.add_argument(
         "--solver-options-string",
         dest="solver_options_string",
-        default=None,
+        default="",
         help="""
             A quoted string of options to pass to the model solver. Each option
             must be of the form option=value. (e.g., --solver-options-string
             "mipgap=0.001 primalopt='' advance=2 threads=1")
         """,
     )
     argparser.add_argument(
@@ -778,28 +719,47 @@
         action="store_true",
         help="""
             Don't run post-solve code on the completed model (i.e., reporting
             functions).
         """,
     )
     argparser.add_argument(
+        "--no-load-solution",
+        default=False,
+        action="store_true",
+        help="""
+            Attempt to solve model but do not load the results from the solver.
+            This can be useful for reporting additional information on models
+            that fail to solve.
+        """,
+    )
+    argparser.add_argument(
         "--reload-prior-solution",
         default=False,
         action="store_true",
         help="""
             Load a previously saved solution; useful for re-running
             post-solve code or interactively exploring the model (with
             --interact).
         """,
     )
     argparser.add_argument(
         "--no-save-solution",
         default=False,
         action="store_true",
-        help="Don't save solution after model is solved.",
+        help=argparse.SUPPRESS,  # deprecated
+    )
+    argparser.add_argument(
+        "--save-solution-file",
+        default=False,
+        action="store_true",
+        help="""
+            Save solution file (results.pickle) after model is solved, to enable
+            reloading via `--reload-prior-solution`.
+        """,
     )
     argparser.add_argument(
         "--interact",
         default=False,
         action="store_true",
         help="""
             Enter interactive shell after solving the instance to enable
@@ -1056,91 +1016,121 @@
 def solve(model):
     if not hasattr(model, "solver"):
         # Create a solver object the first time in. We don't do this until a solve is
         # requested, because sometimes a different solve function may be used,
         # with its own solver object (e.g., with runph or a parallel solver server).
         # In those cases, we don't want to go through the expense of creating an
         # unused solver object, or get errors if the solver options are invalid.
-        model.solver = SolverFactory(
-            model.options.solver, solver_io=model.options.solver_io
-        )
-
-        # patch for Pyomo < 4.2
-        # note: Pyomo added an options_string argument to solver.solve() in Pyomo 4.2 rev 10587.
-        # (See https://software.sandia.gov/trac/pyomo/browser/pyomo/trunk/pyomo/opt/base/solvers.py?rev=10587 )
-        # This is misreported in the documentation as options=, but options= actually accepts a dictionary.
-        if model.options.solver_options_string and not hasattr(
-            model.solver, "_options_string_to_dict"
-        ):
-            for k, v in _options_string_to_dict(
-                model.options.solver_options_string
-            ).items():
-                model.solver.options[k] = v
+        # Only specify keyword args if values are provided; `None` can cause errors
+        solver_args = {}
+        if model.options.solver_io is not None:
+            solver_args["solver_io"] = model.options.solver_io
+        model.solver = SolverFactory(model.options.solver, **solver_args)
 
         model.solver_manager = SolverManagerFactory(model.options.solver_manager)
 
     # get solver arguments
     solver_args = dict(
-        options_string=model.options.solver_options_string,
+        # note: prior to switch 2.0.8, we passed solver_options_string as
+        # a solver_options argument, but the appsi_ solvers don't accept that,
+        # so now we pass an options dict for all solvers instead
+        options=options_string_to_dict(model.options.solver_options_string),
         keepfiles=model.options.keepfiles,
         tee=model.options.tee,
         symbolic_solver_labels=model.options.symbolic_solver_labels,
     )
     # drop all the unspecified options
-    solver_args = {k: v for (k, v) in solver_args.items() if v is not None}
+    solver_args = {k: v for (k, v) in solver_args.items() if v}
 
-    # Automatically send all defined suffixes to the solver
-    solver_args["suffixes"] = [c.name for c in model.component_objects(ctype=Suffix)]
+    if model.options.no_load_solution:
+        solver_args["load_solutions"] = False
 
-    # note: the next few lines are faster than the line above, but seem risky:
-    # i = m._ctypes.get(Suffix, [None])[0]
-    # solver_args["suffixes"] = []
-    # while i is not None:
-    #     c, i = m._decl_order[i]
-    #     solver_args[suffixes].append(c.name)
-
-    # patch for Pyomo < 4.2
-    if not hasattr(model.solver, "_options_string_to_dict"):
-        solver_args.pop("options_string", "")
+    # Automatically send any defined suffixes to the solver
+    # This is mostly obsolete: appsi_* solvers won't accept any suffixes but
+    # automatically adapt to duals, slack and rc; cplex and gurobi accept
+    # suffixes but will also produce duals automatically if the model has
+    # a duals component. But we send these anyway in case that treatment doesn't
+    # extend to more specialized suffixes like iis.
+    suffixes = [c.name for c in model.component_objects(ctype=Suffix)]
+    if suffixes and not model.options.solver.startswith("appsi_"):
+        # don't assign at all if no suffixes are defined, since appsi_highs
+        # (and maybe others, but also maybe only old versions) want None
+        # instead of an empty list, but cplex and gurobi crash with None
+        solver_args["suffixes"] = suffixes
 
     # patch Pyomo to retrieve MIP duals from cplex if needed
     if model.options.retrieve_cplex_mip_duals:
         retrieve_cplex_mip_duals(model)
 
     # solve the model
     timer = StepTimer()
     model.logger.info("\nSolving model...")
 
     if model.options.tempdir is not None:
-        # from https://software.sandia.gov/downloads/pub/pyomo/PyomoOnlineDocs.html#_changing_the_temporary_directory
-        from pyutilib.services import TempfileManager
+        from pyomo.common.tempfiles import TempfileManager
 
         TempfileManager.tempdir = model.options.tempdir
 
     if model.options.tee:
         # bar above solver output
         model.logger.info("-" * 33 + " solver output " + "-" * 32)
 
     try:
         results = model.solver_manager.solve(model, opt=model.solver, **solver_args)
-    except ValueError as err:
-        # show the solver status for obscure errors if possible
-        model.logger.error("\n" + "=" * 80 + "\nError during solve:\n")
-        try:
-            model.logger.error(err.__traceback__.tb_frame.f_locals["results"])
-        except:
-            pass
+    except Exception as err:
+        # report miscellaneous errors
+        # TODO: convert appsi's recommendations into Switch recommendations,
+        # i.e., create a --no-load-results option and tell the user to set that,
+        # then report the actual status (without results loaded, which will get
+        # us down to the invalid-solution step later...)
+        err_str = str(err)
+
+        # convert some errors to more useful form
+        if "Solver <class" in err_str and "is not available" in err_str:
+            raise RuntimeError(
+                f"Solver {model.options.solver} could not be found. "
+                "This is usually due to missing either the solver binary "
+                "software or the python bindings for it."
+            )
+        elif err_str.startswith(
+            "A feasible solution was not found, so no solution can be loaded."
+        ):
+            new_err = (
+                "A feasible solution was not found, so no solution could be loaded. "
+                "You may be able to obtain additional details by re-running Switch "
+                "with the `--no-load-solution` flag. "
+            )
+            if model.options.tee:
+                new_err += (
+                    "There may also be additional details in the solver log above."
+                )
+            else:
+                new_err += "The solver may also report additional details if you specify `--stream-solver`."
+            raise RuntimeError(new_err)
+
+        # Report and re-raise error as is
+        model.logger.error(
+            "\n" + "=" * 80 + "\nAn error occurred while solving the model:\n"
+        )
+        model.logger.error(err_str + "\n")
+        if model.options.tee:
+            model.logger.error("Check the solver log above for more details.")
+        else:
+            model.logger.error(
+                "Specify `--stream-solver` and then check the solver log for "
+                "more details."
+            )
         raise
 
     if model.options.tee:
         # bar below solver output
         model.logger.info("-" * 28 + " end of solver output " + "-" * 28 + "\n")
 
     model.logger.info(
-        f"Solved model. Total time spent in solver: {timer.step_time():0.2f} s."
+        f"Solver finished. Total time spent in solver: {timer.step_time():0.2f} s."
     )
 
     # Treat infeasibility as an error, rather than trying to load and save the results
     # (note: in this case, results.solver.status may be SolverStatus.warning instead of
     # SolverStatus.error)
     infeasibility_message = (
         "You can identify infeasible constraints by adding "
@@ -1149,76 +1139,110 @@
         "\n\nAlternatively, if the solver can generate an irreducibly "
         "inconsistent set (IIS), more information may be available by setting "
         "the appropriate flags in the --solver-options-string and then calling "
         'this script with "--suffixes iis".\n'
     )
 
     if results.solver.termination_condition == TerminationCondition.infeasible:
+        model.logger.info("")
         if hasattr(model, "iis"):
             model.logger.error(
-                "Model was infeasible; irreducibly inconsistent set (IIS) returned by solver:"
+                rewrap(
+                    "Model was infeasible; irreducibly inconsistent set (IIS) "
+                    "returned by solver:"
+                )
             )
             model.logger.error("\n".join(sorted(c.name for c in model.iis)))
         else:
-            model.logger.error("Model was infeasible. " + infeasibility_message)
+            model.logger.error(rewrap("Model was infeasible. " + infeasibility_message))
 
         # This infeasibility logging module could be nice, but it doesn't work
         # for my solvers and produces extraneous messages.
         # import pyomo.util.infeasible
         # pyomo.util.infeasible.log_infeasible_constraints(model)
         raise RuntimeError("Infeasible model")
 
-    # Raise an error if the solver failed to produce a solution
-    # Note that checking for results.solver.status in {SolverStatus.ok,
-    # SolverStatus.warning} is not enough because with a warning there will
-    # sometimes be a solution and sometimes not.
+    # There is no clear way to determine whether there is a solution, even if
+    # results.solver.status is not SolverStatus.ok. If results.solver.status ==
+    # SolverStatus.warning (maybe others too), there will sometimes be a
+    # solution and sometimes not (e.g., some solvers give a warning if iteration
+    # limit runs out but still return a valid model). For glpk, infeasible
+    # models produce SolverStatus.ok but termination condition "other" and a
+    # seemingly OK result object, but variable values of None in the model.
+    # Options we've considered:
+    # - (len(model.solutions.solutions) == 0 or
+    #   len(model.solutions[-1]._entry["variable"]) == 0)
+    #   - our standard test through Switch 2.0.7
+    #   - appsi solvers fail this test even when they have a solution
+    # - (results.problem.lower_bound == float("-inf") and
+    #   results.problem.upper_bound == float("inf"))
+    #   - always fails for ampl solvers
+    # - does the solve call raise an error?
+    #   - appsi raises error whenever there's no solution
+    #   - cplexamp raises error when there's no solution (e.g., iteration count
+    #     too low to get a candidate)
+    #   - cplexamp doesn't raise an error if model is proved infeasible
+    #   - glpk does not raise an error even if there's no solution
+    # - len(model.solutions.symbol_map) == 0
+    #   - ampl solver fails this even when it's successful
 
+    # Starting with 2.0.8, we just duck-type it: if the active objective is
+    # accessible valid, it must be OK, otherwise not.
     try:
-        # pyomo 5.2, maybe earlier or later
-        no_solution = len(model.solutions.solutions) == 0
-        solution_status = "unavailable"
-    except AttributeError:
-        # other pyomo version (4.4 or 5.6.8?)
-        # Note: the results object originally contains values for model components
-        # in results.solution.variable, etc., but pyomo.solvers.solve erases it via
-        # result.solution.clear() after calling model.solutions.load_from() with it.
-        # load_from() loads values into the model.solutions._entry, so we check there.
-        # (See pyomo.PyomoModel.ModelSolutions.add_solution() for the code that
-        # actually creates _entry).
-        # Another option might be to check that model.solutions[-1].status (previously
-        # result.solution.status, but also cleared) is in
-        # pyomo.opt.SolutionStatus.['optimal', 'bestSoFar', 'feasible', 'globallyOptimal', 'locallyOptimal'],
-        # but this seems pretty foolproof (if undocumented).
-        no_solution = len(model.solutions[-1]._entry["variable"]) == 0
-        solution_status = model.solutions[-1].status
-
-    if no_solution:
+        for o in model.component_objects(Objective):
+            if o.active:
+                # this mentions the first component that can't be evaluated,
+                # but this is a rare error and there's not much harm in that
+                o()
+    except ValueError:
         # no solution returned
-        model.logger.error("Solver terminated without a solution.")
-        model.logger.error("  Solver Status: ", results.solver.status)
-        model.logger.error("  Solution Status: ", solution_status)
+        model.logger.error("\n" + "=" * 80)
+        model.logger.error("\nSolver terminated without a solution:")
+        model.logger.error(f"  Solver Status: {results.solver.status}")
         model.logger.error(
-            "  Termination Condition: ", results.solver.termination_condition
+            f"  Termination Condition: {results.solver.termination_condition}"
         )
         if (
             model.options.solver == "glpk"
             and results.solver.termination_condition == TerminationCondition.other
         ):
             model.logger.error(
-                "Hint: glpk has been known to classify infeasible problems as 'other'."
+                rewrap(
+                    "Hint: glpk sometimes reports infeasible problems as "
+                    "'Termination condition: other'."
+                )
+            )
+        if model.options.no_load_solution:
+            model.logger.error(
+                "This may be resolved by removing the --no-load-solution flag."
+            )
+
+        if model.options.tee:
+            model.logger.error("Check the solver log above for more details.")
+        else:
+            model.logger.error(
+                "Specify `--stream-solver` and then check the solver log for "
+                "more details."
             )
+
             model.logger.error(infeasibility_message)
-        raise RuntimeError("Solver failed to find an optimal solution.")
+        model.logger.error("")  # add extra line to set info apart
+        raise RuntimeError("Solver failed to produce a solution.")
 
     # Report any warnings; these are written to stderr so users can find them in
     # error logs (e.g. on HPC systems). These can occur, e.g., if solver reaches
     # time limit or iteration limit but still returns a valid solution
-    if results.solver.status == SolverStatus.warning:
+    if results.solver.status != SolverStatus.ok:
+        stat = (
+            "warning"
+            if results.solver.status == SolverStatus.warning
+            else "unexpected status"
+        )
         model.logger.warning(
-            "Solver terminated with warning.\n"
+            f"Solver terminated with {stat}.\n"
             f"  Solver Status: {results.solver.status}\n"
             f"  Solution Status: {model.solutions[-1].status}\n"
             f"  Termination Condition: {results.solver.termination_condition}"
         )
 
     ### process and return solution ###
 
@@ -1278,15 +1302,15 @@
         if (
             hasattr(command, "script")
             and "optimize\n" in command.script
             and not "change problem fix\n" in command.script
         ):
             command.script = command.script.replace(
                 "optimize\n",
-                "optimize\nchange problem fix\noptimize\n"
+                "optimize\nchange problem fix\noptimize\n",
                 # see http://www-01.ibm.com/support/docview.wss?uid=swg21399941
                 # and http://www-01.ibm.com/support/docview.wss?uid=swg21400009
             )
             logger.info("changed CPLEX solve script to the following:")
             logger.info(command.script)
         else:
             logger.warning(
@@ -1296,42 +1320,15 @@
         return command
 
     new_create_command_line.is_patched = True
     if not getattr(CPLEXSHELL.create_command_line, "is_patched", False):
         CPLEXSHELL.create_command_line = new_create_command_line
 
 
-# taken from https://software.sandia.gov/trac/pyomo/browser/pyomo/trunk/pyomo/opt/base/solvers.py?rev=10784
-# This can be removed when all users are on Pyomo 4.2
-import pyutilib
-
-
-def _options_string_to_dict(istr):
-    ans = {}
-    istr = istr.strip()
-    if not istr:
-        return ans
-    if istr[0] == "'" or istr[0] == '"':
-        istr = eval(istr)
-    tokens = pyutilib.misc.quote_split("[ ]+", istr)
-    for token in tokens:
-        index = token.find("=")
-        if index == -1:
-            raise ValueError(
-                "Solver options must have the form option=value: '{}'".format(istr)
-            )
-        try:
-            val = eval(token[(index + 1) :])
-        except:
-            val = token[(index + 1) :]
-        ans[token[:index]] = val
-    return ans
-
-
-def save_results(instance, outdir):
+def save_solution_file(instance, outdir):
     """
     Save model solution for later reuse.
 
     Note that this pickles a solver results object because the instance itself
     cannot be pickled -- see
     https://stackoverflow.com/questions/39941520/pyomo-ipopt-does-not-return-solution
     """
@@ -1401,11 +1398,32 @@
                 print(
                     "\nA model can be found in '{}.model()' {}".format(name, location)
                 )
                 return
     print("\nNo Pyomo model was found in the current stack trace.")
 
 
+def options_string_to_dict(opt_str):
+    opt_dict = {}
+    tokens = shlex.split(opt_str)
+    for token in tokens:
+        try:
+            key, val = token.split("=", 1)
+        except ValueError:
+            # couldn't split at an equal sign
+            raise ValueError(
+                "Solver options must have the form option=value: '{}'".format(opt_str)
+            )
+        # convert to standard types if possible, otherwise leave as is (usually
+        # an unquoted string)
+        try:
+            val = ast.literal_eval(val)
+        except ValueError:
+            pass
+        opt_dict[key] = val
+    return opt_dict
+
+
 ###############
 
 if __name__ == "__main__":
     main()
```

### Comparing `switch_model-2.0.7/switch_model/solve_scenarios.py` & `switch_model-2.0.8/switch_model/solve_scenarios.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/timescales.py` & `switch_model-2.0.8/switch_model/timescales.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
 
 import os
 from pyomo.environ import *
 from . import utilities
+from .utilities import unique_list
 
 hours_per_year = 8766
 
 
 def define_components(mod):
     """
     Augments a Pyomo abstract model object with sets and parameters that
@@ -120,14 +121,28 @@
     average number of hours in a year rounded to the nearest integer
     (8766) by the number of years per period. I implemented this rule
     because these are used as weights for variable costs of dispatch and
     operations, and I think it is important for those costs to reflect
     those expected costs over an entire period or else the levelized
     costs of power that is being optimized will not make sense.
 
+    Date-related fields, used to identify individual dates when running multi-
+    day timeseries. These are used by modules that require balancing within the
+    day, such as demand response or hydrogen production. The tp_date column in
+    timepoints.csv should be filled in when using these modules.
+
+    tp_date[tp]: date ID for timepoint tp, read from timepoints.csv. If not
+    provided, we use the timeseries that holds this timepoint (tp_ts[tp]).
+
+    DATES: set of all dates used in this model, based on tp_date. Will be
+    equivalent to TIMESERIES if tp_date is not provided.
+
+    TPS_IN_DATE[d in DATES]: indexed set of all TIMEPOINTS that fall in DATE
+    d, derived from tp_date. Will be equivalent to TPS_IN_TS[ts in
+    TIMESERIES] if tp_date is not provided.
 
     EXAMPLES
 
     These hypothetical examples illustrate differential weighting of
     timepoints and timeseries. Each timepoint adds additional
     computational complexity, and you may wish to reduce the time
     resolution in low-stress periods and increase the time resolution in
@@ -391,14 +406,73 @@
                 )
             )
             return 0
         return 1
 
     mod.validate_time_weights = BuildCheck(mod.PERIODS, rule=validate_time_weights_rule)
 
+    #############
+    # date-related code
+
+    # Use a custom timepoint -> date mapping if tp_dates.csv is provided.
+    # Otherwise just use the timeseries as the date ID (more common). Custom
+    # dates can be useful when running a single timeseries for the whole year,
+    # but you still need to identify dates within the year for the flexible load
+    # calculations.
+    mod.tp_date = Param(mod.TIMEPOINTS, default=lambda m, tp: m.tp_ts[tp], within=Any)
+    mod.DATES = Set(
+        initialize=lambda m: unique_list(m.tp_date[tp] for tp in m.TIMEPOINTS)
+    )
+
+    # Efficiently construct the set of timepoints within each date
+    def TPS_IN_DATE_init(m, d):
+        try:
+            dd = m.TPS_IN_DATE_dict
+        except AttributeError:
+            # haven't constructed the date dictionary yet (first call to this
+            # function); build it now
+            dd = m.TPS_IN_DATE_dict = dict()
+            for tp in m.TIMEPOINTS:
+                # create an empty list for the date holding this timepoint (if
+                # needed), then append this timepoint
+                dd.setdefault(m.tp_date[tp], []).append(tp)
+        return dd.pop(d)  # use pop to free memory as we go
+
+    mod.TPS_IN_DATE = Set(mod.DATES, initialize=TPS_IN_DATE_init)
+
+    # Efficiently construct the set of dates within each timeseries
+    # If any date spans multiple timeseries, it will be an error
+    def DATES_IN_TS_init(m, ts):
+        try:
+            dd = m.DATES_IN_TS_dict
+        except AttributeError:
+            # haven't constructed the date dictionary yet (first call to this
+            # function); build it now
+            dd = m.DATES_IN_TS_dict = dict()
+            date_ts = dict()  # cache of already known ts for each date
+            for tp in m.TIMEPOINTS:
+                d = m.tp_date[tp]
+                _ts = m.tp_ts[tp]
+                if _ts != date_ts.setdefault(d, _ts):
+                    # was previously assigned to a different date
+                    raise ValueError(
+                        "Timepoints from different timeseries have been "
+                        f"assigned to the same date {d} in tp_dates.csv. "
+                        "This is not allowed."
+                    )
+                # create a new list for the timeseries holding this
+                # timepoint (if needed), then add this date
+                dd.setdefault(_ts, []).append(d)
+        # return all unique dates for this timeseries
+        return unique_list(dd.pop(ts))
+
+    mod.DATES_IN_TS = Set(mod.TIMESERIES, initialize=DATES_IN_TS_init)
+    # End date code
+    ##########
+
     def validate_period_lengths_rule(m, p):
         tol = 0.01
         if p != m.PERIODS.last():
             p_end = m.period_start[p] + m.period_length_years[p]
             p_next = m.period_start[m.PERIODS.next(p)]
             if abs(p_next - p_end) > tol:
                 print(
@@ -432,15 +506,15 @@
     The order of rows in timepoints.csv indicates the order of the
     timepoints per Pyomo and AMPL convention. To maintain your sanity,
     we highly recommend that you sort your input file chronologically by
     timestamp. Note: timestamp is solely used as a label and be in any
     format.
 
     timepoints.csv
-        timepoint_id, timestamp, timeseries
+        timepoint_id, timestamp, timeseries, tp_date*
 
     """
     # Include select in each load() function so that it will check out column
     # names, be indifferent to column order, and throw an error message if
     # some columns are not found.
     switch_data.load_aug(
         filename=os.path.join(inputs_dir, "periods.csv"),
@@ -455,11 +529,11 @@
             mod.ts_duration_of_tp,
             mod.ts_num_tps,
             mod.ts_scale_to_period,
         ),
     )
     switch_data.load_aug(
         filename=os.path.join(inputs_dir, "timepoints.csv"),
-        select=("timepoint_id", "timestamp", "timeseries"),
+        select=("timepoint_id", "timestamp", "timeseries", "tp_date"),
         index=mod.TIMEPOINTS,
-        param=(mod.tp_timestamp, mod.tp_ts),
+        param=(mod.tp_timestamp, mod.tp_ts, mod.tp_date),
     )
```

### Comparing `switch_model-2.0.7/switch_model/transmission/local_td.py` & `switch_model-2.0.8/switch_model/transmission/local_td.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/transmission/transport/build.py` & `switch_model-2.0.8/switch_model/transmission/transport/build.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/transmission/transport/dispatch.py` & `switch_model-2.0.8/switch_model/transmission/transport/dispatch.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/upgrade/__init__.py` & `switch_model-2.0.8/switch_model/upgrade/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/upgrade/manager.py` & `switch_model-2.0.8/switch_model/upgrade/manager.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/upgrade/re_upgrade.py` & `switch_model-2.0.8/switch_model/upgrade/re_upgrade.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/upgrade/upgrade_2_0_0b1.py` & `switch_model-2.0.8/switch_model/upgrade/upgrade_2_0_0b1.py`

 * *Files 0% similar despite different names*

```diff
@@ -279,15 +279,15 @@
         for col in col_list:
             default_col = col + ".default"
             if default_col not in df:
                 continue
             if col not in df:
                 df.rename(columns={default_col: col}, inplace=True)
             else:
-                df[col].fillna(df[default_col], inplace=True)
+                df[col] = df[col].fillna(df[default_col])
                 del df[default_col]
 
     columns_with_defaults = [
         "proj_scheduled_outage_rate",
         "proj_forced_outage_rate",
         "proj_variable_om",
         "proj_full_load_heat_rate",
```

### Comparing `switch_model-2.0.7/switch_model/upgrade/upgrade_2_0_0b2.py` & `switch_model-2.0.8/switch_model/upgrade/upgrade_2_0_0b2.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/upgrade/upgrade_2_0_0b4.py` & `switch_model-2.0.8/switch_model/upgrade/upgrade_2_0_0b4.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/upgrade/upgrade_2_0_1.py` & `switch_model-2.0.8/switch_model/upgrade/upgrade_2_0_1.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/upgrade/upgrade_2_0_4.py` & `switch_model-2.0.8/switch_model/upgrade/upgrade_2_0_4.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/upgrade/upgrade_2_0_5.py` & `switch_model-2.0.8/switch_model/upgrade/upgrade_2_0_5.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/switch_model/upgrade/upgrade_2_0_6.py` & `switch_model-2.0.8/switch_model/upgrade/upgrade_2_0_7.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 # Copyright (c) 2015-2022 The Switch Authors. All rights reserved.
 # Licensed under the Apache License, Version 2.0, which is in the LICENSE file.
 import os, shutil, argparse, glob
 import pandas as pd
 import switch_model.upgrade
 from pyomo.environ import DataPortal
 
-upgrades_from = "2.0.5"
-upgrades_to = "2.0.6"
+upgrades_from = "2.0.6"
+upgrades_to = "2.0.7"
 
 replace_modules = {
     # modules to be replaced in the module list
     # old_module: [new_module1, new_module2, ...],
-    "switch_model.hawaii.psip_2016_12": ["switch_model.hawaii.heco_outlook_2020_06"],
-    "switch_model.hawaii.kalaeloa": ["switch_model.hawaii.oahu_plants"],
 }
 
 module_messages = {
     # description of significant changes to particular modules other than
     # moving/renaming
     # old_module: message
-    "switch_model.generators.core.build": "Beginning with Switch 2.0.6, gen_multiple_fuels.dat should "
+    "switch_model.generators.core.build":
+    "Beginning with Switch 2.0.7, gen_multiple_fuels.dat should "
     "be replaced with gen_multiple_fuels.csv. The .csv file should have "
     "two columns: GENERATION_PROJECT and fuel. It should have one row for "
     "each allowed fuel for each multi-fuel generator."
 }
 
 
 def upgrade_input_dir(inputs_dir):
@@ -32,38 +31,118 @@
     """
     # Write a new version text file. We do this early so that if the update
     # fails and then the user tries again it won't try to upgrade a second time,
     # overwriting their backup.
     switch_model.upgrade._write_input_version(inputs_dir, upgrades_to)
 
     # rename modules and report changes
-    update_modules(inputs_dir)
+    # update_modules(inputs_dir)
 
     # convert the multi-fuels file to csv format (this is the last .dat input)
     convert_gen_multiple_fuels_to_csv(inputs_dir)
 
-    # rename_file('fuel_cost.csv', 'fuel_cost_per_period.csv')
-    # rename_column('fuel_cost_per_period.csv', 'fuel_cost', 'period_fuel_cost')
+    rename_file(inputs_dir, "generation_projects_info.csv", "gen_info.csv", False)
 
+    rename_column(
+        inputs_dir,
+        "gen_build_predetermined.csv",
+        "gen_predetermined_cap",
+        "build_gen_predetermined",
+    )
+
+    rename_column(
+        inputs_dir,
+        "gen_build_predetermined.csv",
+        "gen_predetermined_storage_energy_mwh",  # briefly used pre-release
+        "build_gen_energy_predetermined",
+    )
+
+    move_column(
+        inputs_dir,
+        old_file_name="trans_params.csv",
+        old_col_name="distribution_loss_rate",
+        new_file_name="load_zones.csv",
+        new_col_name="local_td_loss_rate",
+        join_cols=tuple(),
+        optional_col=True,
+    )
 
-def rename_file(old_name, new_name, optional_file=True):
+
+def rename_file(inputs_dir, old_name, new_name, optional_file=True):
     old_path = os.path.join(inputs_dir, old_name)
     new_path = os.path.join(inputs_dir, new_name)
     if optional_file and not os.path.isfile(old_path):
-        return
-    shutil.move(old_path, new_path)
+        pass
+    elif os.path.isfile(new_path) and not os.path.isfile(old_path):
+        switch_model.upgrade.print_verbose(
+            f"Input file {old_name} was already renamed to {new_name}."
+        )
+    else:
+        shutil.move(old_path, new_path)
+        switch_model.upgrade.print_verbose(
+            f"Input file {old_name} has been renamed to {new_name}."
+        )
 
 
-def rename_column(file_name, old_col_name, new_col_name, optional_file=True):
+def rename_column(
+    inputs_dir, file_name, old_col_name, new_col_name, optional_file=True
+):
     path = os.path.join(inputs_dir, file_name)
     if optional_file and not os.path.isfile(path):
         return
     df = pd.read_csv(path, na_values=["."], sep=",")  # for 2.0.5+
-    df.rename(columns={old_col_name: new_col_name}, inplace=True)
-    df.to_csv(path, sep=",", na_rep=".", index=False)
+    if old_col_name in df.columns:
+        df.rename(columns={old_col_name: new_col_name}, inplace=True)
+        df.to_csv(path, sep=",", na_rep=".", index=False)
+        switch_model.upgrade.print_verbose(
+            f"Column {old_col_name} has been renamed to {new_col_name} in {file_name}."
+        )
+    elif new_col_name in df.columns:
+        switch_model.upgrade.print_verbose(
+            f"Column {old_col_name} was already renamed to {new_col_name} in {file_name}."
+        )
+
+
+def move_column(
+    inputs_dir,
+    old_file_name,
+    old_col_name,
+    new_file_name,
+    new_col_name,
+    join_cols,
+    optional_col=True,
+):
+    old_path = os.path.join(inputs_dir, old_file_name)
+    new_path = os.path.join(inputs_dir, new_file_name)
+    if optional_col and not os.path.isfile(old_path):
+        return
+    # add dummy key to allow cross-joins
+    fixed_join_cols = list(join_cols) + ["dummy_join_key"]
+    old_df = pd.read_csv(old_path, na_values=["."], sep=",").assign(dummy_join_key=0)
+    # TODO: create new_path if it doesn't exist
+    new_df = pd.read_csv(new_path, na_values=["."], sep=",").assign(dummy_join_key=0)
+    if old_col_name in old_df.columns:
+        new_col = old_df.loc[:, fixed_join_cols + [old_col_name]].merge(
+            new_df.loc[:, fixed_join_cols], on=fixed_join_cols
+        )
+        new_df[new_col_name] = new_col[old_col_name]
+        new_df.drop("dummy_join_key", axis=1, inplace=True)
+        new_df.to_csv(new_path, sep=",", na_rep=".", index=False)
+        old_df.drop([old_col_name, "dummy_join_key"], axis=1, inplace=True)
+        old_df.to_csv(old_path, sep=",", na_rep=".", index=False)
+        switch_model.upgrade.print_verbose(
+            f"Column {old_file_name} > {old_col_name} has been moved to {new_file_name} > {new_col_name}."
+        )
+    elif new_col_name in new_df.columns:
+        switch_model.upgrade.print_verbose(
+            f"Column {old_file_name} > {old_col_name} was already moved to {new_file_name} > {new_col_name}."
+        )
+    elif not optional_col:
+        # column wasn't found and isn't optional
+        raise ValueError(f"Mandatory column {old_col_name} not found in {old_path}.")
 
 
 def item_list(items):
     """Generate normal-text version of list of items, with commas and "and" as needed."""
     return " and ".join(", ".join(items).rsplit(", ", 1))
```

### Comparing `switch_model-2.0.7/switch_model/utilities.py` & `switch_model-2.0.8/switch_model/utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,20 +207,25 @@
             self.__n_components_constructed = 1
 
         try:
             next_report = self.__next_report_components_construction
         except:
             next_report = 0
 
-        fraction_constructed = self.__n_components_constructed / len(self._decl_order)
+        # note: we previously used self._decl_order (collection of all
+        # components in model), but that may have dummy entries, especially when
+        # using the diagnose_infeasibility module, so we switched to self._decl,
+        # which shows the indexes in _decl_order for all the actual components
+        # in the model.
+        fraction_constructed = self.__n_components_constructed / len(self._decl)
 
         if fraction_constructed >= next_report:
             self.logger.info(
                 f"Constructed "
-                f"{self.__n_components_constructed} of {len(self._decl_order)} "
+                f"{self.__n_components_constructed} of {len(self._decl)} "
                 f"components ({fraction_constructed:.0%})"
             )
             self.__next_report_components_construction = next_report + 0.1
 
     def load_inputs(self, inputs_dir=None, attach_data_portal=True):
         """
         Load input data using the appropriate modules and return a model
@@ -328,15 +333,15 @@
     Create a list with the unique elements from seq, preserving original order.
 
     This is often useful instead of `set()` when creating Pyomo Sets from unique
     members of a collection, since Pyomo >= 5.7 always creates ordered sets and
     deprecates use of Python's unordered sets for initialization.
     """
     # from https://stackoverflow.com/a/17016257/
-    # Note that this solution depends on Python's order-preserving dicts after
+    # Note that this solution depends on Python's order-preserving dicts
     # in version 3.7+, which is fine since Switch requires Python >= 3.7.
     return list(dict.fromkeys(seq))
 
 
 def make_iterable(item):
     """Return an iterable for the one or more items passed."""
     if isinstance(item, string_types):
@@ -383,18 +388,16 @@
     Save input data to a .dat file for use with PySP or other command line
     tools that have not been fully integrated with DataPortal.
     SYNOPSIS:
         save_inputs_as_dat(model, instance, save_path)
     """
     # helper function to convert values to strings,
     # putting quotes around values that start as strings
-    quote_str = (
-        lambda v: '"{}"'.format(v)
-        if isinstance(v, string_types)
-        else "{}".format(str(v))
+    quote_str = lambda v: (
+        '"{}"'.format(v) if isinstance(v, string_types) else "{}".format(str(v))
     )
     # helper function to create delimited lists from single items or iterables of any data type
     from switch_model.reporting import make_iterable
 
     join_space = lambda items: " ".join(
         map(str, make_iterable(items))
     )  # space-separated list
@@ -707,15 +710,15 @@
             kwargs["param"] = list(kwargs["param"])
         # Singleton -> list
         elif not isinstance(kwargs["param"], list):
             kwargs["param"] = [kwargs["param"]]
         params = kwargs["param"]
     # optional_params may include Param objects instead of names. In
     # those cases, convert objects to names.
-    for (i, p) in enumerate(optional_params):
+    for i, p in enumerate(optional_params):
         if not isinstance(p, string_types):
             optional_params[i] = p.name
     # Expand the list of optional parameters to include any parameter that has
     # default() defined or that comes from an optional table. We also allow an
     # explicit list of optional parameters to support parameters like
     # gen_unit_size, which doesn't have a default value because it is undefined
     # for generators for which it does not apply.
@@ -765,25 +768,25 @@
         kwargs["select"] = headers[0:num_indexes] + [p.name for p in params]
     # Check to see if expected column names are in the file. If a column
     # name is missing and its parameter is optional, then drop it from
     # the select & param lists.
     if isinstance(kwargs["select"], tuple):
         kwargs["select"] = list(kwargs["select"])
     del_items = []
-    for (i, col) in enumerate(kwargs["select"]):
+    for i, col in enumerate(kwargs["select"]):
         p_i = i - num_indexes
         if col not in headers:
             if len(params) > p_i >= 0 and params[p_i].name in optional_params:
                 del_items.append((i, p_i))
             else:
                 raise InputError(f"Required column {col} not found in file {path}.")
     # When deleting entries from select & param lists, go from last
     # to first so that the indexes won't get messed up as we go.
     del_items.sort(reverse=True)
-    for (i, p_i) in del_items:
+    for i, p_i in del_items:
         del kwargs["select"][i]
         del kwargs["param"][p_i]
 
     # keep a record of which table each param was read from, for reporting
     # by min_data_check later
     for col, param in zip(kwargs["select"][num_indexes:], params):
         try:
@@ -791,14 +794,17 @@
         except AttributeError:
             map = switch_data._model.param_column_map = dict()
         map[param.name] = (kwargs["filename"], col)
 
     if optional and file_has_no_data_rows:
         # Skip the file.  Note that we are only doing this after having
         # validated the file's column headings.
+        # TODO: allow skipping even if the table is not optional, to deal with
+        # .csv files with empty index sets. This may be equivalent to
+        # https://github.com/Pyomo/pyomo/issues/1083#issuecomment-723528448
         return
     # All done with cleaning optional bits. Pass the updated arguments
     # into the DataPortal.load() function.
     try:
         switch_data.load(**kwargs)
     except Exception as e:
         # Pyomo error messages can be very cryptic, so we at least make sure to
@@ -900,14 +906,15 @@
 # --scenario x --solver-options-string="a=b c=d"
 test_parser = argparse.ArgumentParser()
 test_parser.add_argument("--arg1", nargs="+", default=[])
 bad_equal_parser = (
     len(test_parser.parse_known_args(["--arg1", "a", "--arg2=a=1 b=2"])[1]) == 0
 )
 
+
 # TODO: merge the _ArgumentParserAllowAbbrev code into this class
 class _ArgumentParser(_ArgumentParserAllowAbbrev):
     """
     Custom version of ArgumentParser:
     - warns about a bug in standard Python ArgumentParser for --arg="some words"
     - allows use of 'extend', 'include' and 'exclude' actions to accumulate lists
       with multiple calls
```

### Comparing `switch_model-2.0.7/switch_model.egg-info/PKG-INFO` & `switch_model-2.0.8/switch_model.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: switch-model
-Version: 2.0.7
+Version: 2.0.8
 Summary: Switch Power System Planning Model
 Home-page: http://switch-model.org
 Maintainer: Switch Authors
 Maintainer-email: authors@switch-model.org
 License: Apache License 2.0
 Keywords: renewable,power,energy,electricity,production cost,capacity expansion,planning,optimization
 Platform: any
@@ -19,23 +19,35 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7.0, <3.11.0a0
+Requires-Python: >=3.7.2, <3.13.0a0
 Description-Content-Type: text/markdown
-Provides-Extra: advanced
-Provides-Extra: dev
-Provides-Extra: plotting
-Provides-Extra: database_access
 License-File: LICENSE
 License-File: LICENSE.BOILERPLATE
 License-File: AUTHORS
+Requires-Dist: Pyomo<=6.7.1,>=6.0.0
+Requires-Dist: pint
+Requires-Dist: testfixtures
+Requires-Dist: pandas
+Provides-Extra: advanced
+Requires-Dist: numpy; extra == "advanced"
+Requires-Dist: scipy; extra == "advanced"
+Requires-Dist: rpy2; extra == "advanced"
+Requires-Dist: sympy; extra == "advanced"
+Provides-Extra: dev
+Requires-Dist: ipdb; extra == "dev"
+Provides-Extra: plotting
+Requires-Dist: plotnine; extra == "plotting"
+Requires-Dist: matplotlib; extra == "plotting"
+Provides-Extra: database-access
+Requires-Dist: psycopg2-binary; extra == "database-access"
 
 This contains version 2 of the Switch electricity planning model.
 This optimization model is modular and can be used with varying levels
 of complexity. Look in the examples directory for demonstrations of
 using Switch for investment planning or production cost simulation. The
 examples enable varying levels of model complexity by choosing which
 modules to include.
```

### Comparing `switch_model-2.0.7/switch_model.egg-info/SOURCES.txt` & `switch_model-2.0.8/switch_model.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -146,16 +146,15 @@
 examples/copperplate1/inputs/timepoints.csv
 examples/copperplate1/inputs/timeseries.csv
 examples/copperplate1/inputs/variable_capacity_factors.csv
 examples/copperplate1/inputs/zone_to_regional_fuel_market.csv
 examples/copperplate1/outputs/total_cost.txt
 examples/custom_extension/README
 examples/custom_extension/sunk_costs.py
-examples/custom_extension/__pycache__/sunk_costs.cpython-310.pyc
-examples/custom_extension/__pycache__/sunk_costs.cpython-37.pyc
+examples/custom_extension/__pycache__/sunk_costs.cpython-312.pyc
 examples/custom_extension/inputs/financials.csv
 examples/custom_extension/inputs/fuel_cost.csv
 examples/custom_extension/inputs/fuels.csv
 examples/custom_extension/inputs/gen_build_costs.csv
 examples/custom_extension/inputs/gen_build_predetermined.csv
 examples/custom_extension/inputs/gen_info.csv
 examples/custom_extension/inputs/load_zones.csv
@@ -281,14 +280,41 @@
 examples/hydro_system/inputs/timepoints.csv
 examples/hydro_system/inputs/timeseries.csv
 examples/hydro_system/inputs/variable_capacity_factors.csv
 examples/hydro_system/inputs/water_connections.csv
 examples/hydro_system/inputs/water_node_tp_flows.csv
 examples/hydro_system/inputs/water_nodes.csv
 examples/hydro_system/outputs/total_cost.txt
+examples/hydrogen/README.md
+examples/hydrogen/inputs/carbon_policies.csv
+examples/hydrogen/inputs/financials.csv
+examples/hydrogen/inputs/fuel_cost.csv
+examples/hydrogen/inputs/fuel_supply_curves.csv
+examples/hydrogen/inputs/fuels.csv
+examples/hydrogen/inputs/gen_build_costs.csv
+examples/hydrogen/inputs/gen_build_predetermined.csv
+examples/hydrogen/inputs/gen_info.csv
+examples/hydrogen/inputs/gen_multiple_fuels.csv
+examples/hydrogen/inputs/hydrogen.csv
+examples/hydrogen/inputs/load_zones.csv
+examples/hydrogen/inputs/loads.csv
+examples/hydrogen/inputs/modules.txt
+examples/hydrogen/inputs/non_fuel_energy_sources.csv
+examples/hydrogen/inputs/periods.csv
+examples/hydrogen/inputs/regional_fuel_markets.csv
+examples/hydrogen/inputs/switch_inputs_version.txt
+examples/hydrogen/inputs/timepoints.csv
+examples/hydrogen/inputs/timeseries.csv
+examples/hydrogen/inputs/transmission_lines.csv
+examples/hydrogen/inputs/variable_capacity_factors.csv
+examples/hydrogen/inputs/zone_balancing_areas.csv
+examples/hydrogen/inputs/zone_coincident_peak_demand.csv
+examples/hydrogen/inputs/zone_fuel_cost_diff.csv
+examples/hydrogen/inputs/zone_to_regional_fuel_market.csv
+examples/hydrogen/outputs/total_cost.txt
 examples/new_builds_only/README.md
 examples/new_builds_only/inputs/financials.csv
 examples/new_builds_only/inputs/fuel_cost.csv
 examples/new_builds_only/inputs/fuels.csv
 examples/new_builds_only/inputs/gen_build_costs.csv
 examples/new_builds_only/inputs/gen_info.csv
 examples/new_builds_only/inputs/load_zones.csv
@@ -478,14 +504,40 @@
 examples/production_cost_models/unit_commit/inputs/switch_inputs_version.txt
 examples/production_cost_models/unit_commit/inputs/timepoints.csv
 examples/production_cost_models/unit_commit/inputs/timeseries.csv
 examples/production_cost_models/unit_commit/inputs/variable_capacity_factors.csv
 examples/production_cost_models/unit_commit/inputs/zone_coincident_peak_demand.csv
 examples/production_cost_models/unit_commit/outputs/dispatch.txt
 examples/production_cost_models/unit_commit/outputs/total_cost.txt
+examples/retrofits/inputs/carbon_policies.csv
+examples/retrofits/inputs/financials.csv
+examples/retrofits/inputs/fuel_cost.csv
+examples/retrofits/inputs/fuel_supply_curves.csv
+examples/retrofits/inputs/fuels.csv
+examples/retrofits/inputs/gen_build_costs.csv
+examples/retrofits/inputs/gen_build_predetermined.csv
+examples/retrofits/inputs/gen_info.csv
+examples/retrofits/inputs/gen_retrofits.csv
+examples/retrofits/inputs/load_zones.csv
+examples/retrofits/inputs/loads.csv
+examples/retrofits/inputs/modules.txt
+examples/retrofits/inputs/non_fuel_energy_sources.csv
+examples/retrofits/inputs/periods.csv
+examples/retrofits/inputs/regional_fuel_markets.csv
+examples/retrofits/inputs/switch_inputs_version.txt
+examples/retrofits/inputs/timepoints.csv
+examples/retrofits/inputs/timeseries.csv
+examples/retrofits/inputs/trans_params.csv
+examples/retrofits/inputs/transmission_lines.csv
+examples/retrofits/inputs/variable_capacity_factors.csv
+examples/retrofits/inputs/zone_balancing_areas.csv
+examples/retrofits/inputs/zone_coincident_peak_demand.csv
+examples/retrofits/inputs/zone_fuel_cost_diff.csv
+examples/retrofits/inputs/zone_to_regional_fuel_market.csv
+examples/retrofits/outputs/total_cost.txt
 examples/rps_simple/README.md
 examples/rps_simple/inputs/financials.csv
 examples/rps_simple/inputs/fuel_cost.csv
 examples/rps_simple/inputs/fuel_supply_curves.csv
 examples/rps_simple/inputs/fuels.csv
 examples/rps_simple/inputs/gen_build_costs.csv
 examples/rps_simple/inputs/gen_build_predetermined.csv
@@ -521,14 +573,15 @@
 examples/storage/inputs/periods.csv
 examples/storage/inputs/switch_inputs_version.txt
 examples/storage/inputs/timepoints.csv
 examples/storage/inputs/timeseries.csv
 examples/storage/inputs/variable_capacity_factors.csv
 examples/storage/outputs/total_cost.txt
 switch_model/__init__.py
+switch_model/api.py
 switch_model/financials.py
 switch_model/main.py
 switch_model/solve.py
 switch_model/solve_scenarios.py
 switch_model/test.py
 switch_model/timescales.py
 switch_model/utilities.py
@@ -556,27 +609,30 @@
 switch_model/energy_sources/__init__.py
 switch_model/energy_sources/properties.py
 switch_model/energy_sources/fuel_costs/__init__.py
 switch_model/energy_sources/fuel_costs/markets.py
 switch_model/energy_sources/fuel_costs/markets_expansion.py
 switch_model/energy_sources/fuel_costs/simple.py
 switch_model/energy_sources/fuel_costs/simple_per_timepoint.py
+switch_model/energy_sources/hydrogen/__init__.py
+switch_model/energy_sources/hydrogen/production.py
 switch_model/generators/__init__.py
 switch_model/generators/core/__init__.py
 switch_model/generators/core/build.py
 switch_model/generators/core/dispatch.py
 switch_model/generators/core/gen_discrete_build.py
 switch_model/generators/core/no_commit.py
 switch_model/generators/core/commit/__init__.py
 switch_model/generators/core/commit/discrete.py
 switch_model/generators/core/commit/fuel_use.py
 switch_model/generators/core/commit/operate.py
 switch_model/generators/extensions/__init__.py
 switch_model/generators/extensions/hydro_simple.py
 switch_model/generators/extensions/hydro_system.py
+switch_model/generators/extensions/retrofit.py
 switch_model/generators/extensions/storage.py
 switch_model/hawaii/__init__.py
 switch_model/hawaii/batteries.py
 switch_model/hawaii/batteries_fixed_calendar_life.py
 switch_model/hawaii/demand_response_no_reserves.py
 switch_model/hawaii/demand_response_simple.py
 switch_model/hawaii/emission_rules.py
@@ -636,22 +692,18 @@
 switch_model/upgrade/upgrade_2_0_5.py
 switch_model/upgrade/upgrade_2_0_6.py
 switch_model/upgrade/upgrade_2_0_7.py
 tests/__init__.py
 tests/examples_test.py
 tests/upgrade_test.py
 tests/utilities_test.py
-tests/__pycache__/__init__.cpython-310.pyc
-tests/__pycache__/__init__.cpython-37.pyc
-tests/__pycache__/examples_test.cpython-310.pyc
-tests/__pycache__/examples_test.cpython-37.pyc
-tests/__pycache__/upgrade_test.cpython-310.pyc
-tests/__pycache__/upgrade_test.cpython-37.pyc
-tests/__pycache__/utilities_test.cpython-310.pyc
-tests/__pycache__/utilities_test.cpython-37.pyc
+tests/__pycache__/__init__.cpython-312.pyc
+tests/__pycache__/examples_test.cpython-312.pyc
+tests/__pycache__/upgrade_test.cpython-312.pyc
+tests/__pycache__/utilities_test.cpython-312.pyc
 tests/upgrade_dat/README.txt
 tests/upgrade_dat/3zone_toy/inputs/balancing_areas.tab
 tests/upgrade_dat/3zone_toy/inputs/financials.dat
 tests/upgrade_dat/3zone_toy/inputs/fuel_cost.tab
 tests/upgrade_dat/3zone_toy/inputs/fuel_supply_curves.tab
 tests/upgrade_dat/3zone_toy/inputs/fuels.tab
 tests/upgrade_dat/3zone_toy/inputs/gen_new_build_costs.tab
```

### Comparing `switch_model-2.0.7/tests/examples_test.py` & `switch_model-2.0.8/tests/examples_test.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/tests/upgrade_dat/3zone_toy/inputs/gen_new_build_costs.tab` & `switch_model-2.0.8/tests/upgrade_dat/3zone_toy/inputs/gen_new_build_costs.tab`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/tests/upgrade_dat/3zone_toy/inputs/generator_info.tab` & `switch_model-2.0.8/tests/upgrade_dat/3zone_toy/inputs/generator_info.tab`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/tests/upgrade_dat/3zone_toy/inputs/project_info.tab` & `switch_model-2.0.8/tests/upgrade_dat/3zone_toy/inputs/project_info.tab`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/tests/upgrade_dat/3zone_toy/inputs/variable_capacity_factors.tab` & `switch_model-2.0.8/tests/upgrade_dat/3zone_toy/inputs/variable_capacity_factors.tab`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/tests/upgrade_dat/3zone_toy_2_0_6/inputs/fuel_supply_curves.csv` & `switch_model-2.0.8/tests/upgrade_dat/3zone_toy_2_0_6/inputs/fuel_supply_curves.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/tests/upgrade_dat/3zone_toy_2_0_6/inputs/gen_build_costs.csv` & `switch_model-2.0.8/tests/upgrade_dat/3zone_toy_2_0_6/inputs/gen_build_costs.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/tests/upgrade_dat/3zone_toy_2_0_6/inputs/generation_projects_info.csv` & `switch_model-2.0.8/tests/upgrade_dat/3zone_toy_2_0_6/inputs/generation_projects_info.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/tests/upgrade_dat/3zone_toy_2_0_6/inputs/variable_capacity_factors.csv` & `switch_model-2.0.8/examples/rps_simple/inputs/variable_capacity_factors.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/tests/upgrade_dat/README.txt` & `switch_model-2.0.8/tests/upgrade_dat/README.txt`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/tests/upgrade_dat/copperplate1/inputs/generator_info.tab` & `switch_model-2.0.8/tests/upgrade_dat/copperplate1/inputs/generator_info.tab`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/tests/upgrade_dat/custom_extension/sunk_costs.py` & `switch_model-2.0.8/tests/upgrade_dat/custom_extension/sunk_costs.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/tests/upgrade_dat/hydro_system/inputs/loads.tab` & `switch_model-2.0.8/tests/upgrade_dat/hydro_system/inputs/loads.tab`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/tests/upgrade_dat/hydro_system/inputs/timepoints.tab` & `switch_model-2.0.8/tests/upgrade_dat/hydro_system/inputs/timepoints.tab`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/tests/upgrade_dat/hydro_system/inputs/variable_capacity_factors.tab` & `switch_model-2.0.8/tests/upgrade_dat/hydro_system/inputs/variable_capacity_factors.tab`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/tests/upgrade_dat/hydro_system/inputs/water_node_tp_flows.tab` & `switch_model-2.0.8/tests/upgrade_dat/hydro_system/inputs/water_node_tp_flows.tab`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/tests/upgrade_dat/production_cost_models/discrete_unit_commit/inputs/generator_info.tab` & `switch_model-2.0.8/tests/upgrade_dat/production_cost_models/discrete_unit_commit/inputs/generator_info.tab`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/tests/upgrade_dat/production_cost_models/unit_commit/inputs/generator_info.tab` & `switch_model-2.0.8/tests/upgrade_dat/production_cost_models/unit_commit/inputs/generator_info.tab`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/tests/upgrade_dat/storage_206/inputs/generation_projects_info.csv` & `switch_model-2.0.8/tests/upgrade_dat/storage_206/inputs/generation_projects_info.csv`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/tests/upgrade_test.py` & `switch_model-2.0.8/tests/upgrade_test.py`

 * *Files identical despite different names*

### Comparing `switch_model-2.0.7/tests/utilities_test.py` & `switch_model-2.0.8/tests/utilities_test.py`

 * *Files identical despite different names*

