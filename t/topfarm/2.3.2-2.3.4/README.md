# Comparing `tmp/topfarm-2.3.2.tar.gz` & `tmp/topfarm-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "topfarm-2.3.2.tar", last modified: Mon Mar 27 12:55:44 2023, max compression
+gzip compressed data, was "topfarm-2.3.4.tar", last modified: Thu May 16 06:23:03 2024, max compression
```

## Comparing `topfarm-2.3.2.tar` & `topfarm-2.3.4.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:55:44.167452 topfarm-2.3.2/
--rw-rw-rw-   0 root         (0) root         (0)     1064 2023-03-15 10:02:58.000000 topfarm-2.3.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1005 2023-03-27 12:55:44.167452 topfarm-2.3.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      750 2023-03-15 10:02:58.000000 topfarm-2.3.2/README
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:55:44.147452 topfarm-2.3.2/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-15 10:02:58.000000 topfarm-2.3.2/examples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:55:44.151452 topfarm-2.3.2/examples/irp_wind/
--rw-rw-rw-   0 root         (0) root         (0)     1704 2023-03-15 10:02:58.000000 topfarm-2.3.2/examples/irp_wind/Hornsrev_aep.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-15 10:02:58.000000 topfarm-2.3.2/examples/irp_wind/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3106 2023-03-15 10:02:58.000000 topfarm-2.3.2/examples/irp_wind/optimization_3tb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:55:44.151452 topfarm-2.3.2/examples/scripts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-15 10:02:58.000000 topfarm-2.3.2/examples/scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4624 2023-03-15 10:02:58.000000 topfarm-2.3.2/examples/scripts/example_10_mongodb.py
--rw-rw-rw-   0 root         (0) root         (0)     1714 2023-03-15 10:02:58.000000 topfarm-2.3.2/examples/scripts/example_13_automatic_differentiation.py
--rw-rw-rw-   0 root         (0) root         (0)     3737 2023-03-15 10:02:58.000000 topfarm-2.3.2/examples/scripts/example_14_regular_grid_optimization.py
--rw-rw-rw-   0 root         (0) root         (0)     7862 2023-03-15 10:02:58.000000 topfarm-2.3.2/examples/scripts/example_15_sgd_driver.py
--rw-rw-rw-   0 root         (0) root         (0)     2741 2023-03-15 10:02:58.000000 topfarm-2.3.2/examples/scripts/example_16_smart_start_types.py
--rw-rw-rw-   0 root         (0) root         (0)     3955 2023-03-15 10:02:58.000000 topfarm-2.3.2/examples/scripts/example_1_constrained_layout_optimization.py
--rw-rw-rw-   0 root         (0) root         (0)     5732 2023-03-15 10:02:58.000000 topfarm-2.3.2/examples/scripts/example_2_wake_comparison.py
--rw-rw-rw-   0 root         (0) root         (0)     2382 2023-03-15 10:02:58.000000 topfarm-2.3.2/examples/scripts/example_3_turbine_type_optimization.py
--rw-rw-rw-   0 root         (0) root         (0)     2905 2023-03-15 10:02:58.000000 topfarm-2.3.2/examples/scripts/example_4_integrated_optimization_aep_and_irr.py
--rw-rw-rw-   0 root         (0) root         (0)     3318 2023-03-15 10:02:58.000000 topfarm-2.3.2/examples/scripts/example_5_integrated_opt_with_dtu_cost_model.py
--rw-rw-rw-   0 root         (0) root         (0)    11228 2023-03-15 10:02:58.000000 topfarm-2.3.2/examples/scripts/example_6_floris.py
--rw-rw-rw-   0 root         (0) root         (0)     2820 2023-03-15 10:02:58.000000 topfarm-2.3.2/examples/scripts/example_7_parallel_cost_comp_mpi.py
--rw-rw-rw-   0 root         (0) root         (0)     4204 2023-03-15 10:02:58.000000 topfarm-2.3.2/examples/scripts/example_9_irr_opt_on_weibull_site.py
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-03-27 12:55:44.167452 topfarm-2.3.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1673 2023-03-15 10:02:58.000000 topfarm-2.3.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:55:44.155452 topfarm-2.3.2/topfarm/
--rw-rw-rw-   0 root         (0) root         (0)      378 2023-03-27 12:55:43.000000 topfarm-2.3.2/topfarm/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    29029 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/_topfarm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:55:44.155452 topfarm-2.3.2/topfarm/constraint_components/
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/constraint_components/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      573 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/constraint_components/_constraint.py
--rw-rw-rw-   0 root         (0) root         (0)    50388 2023-03-17 08:19:32.000000 topfarm-2.3.2/topfarm/constraint_components/boundary.py
--rw-rw-rw-   0 root         (0) root         (0)    18987 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/constraint_components/boundary_component.py
--rw-rw-rw-   0 root         (0) root         (0)     2415 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/constraint_components/capacity.py
--rw-rw-rw-   0 root         (0) root         (0)     2811 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/constraint_components/constrained_generator.py
--rw-rw-rw-   0 root         (0) root         (0)     4017 2023-03-17 08:19:32.000000 topfarm-2.3.2/topfarm/constraint_components/constraint_aggregation.py
--rw-rw-rw-   0 root         (0) root         (0)    12685 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/constraint_components/load.py
--rw-rw-rw-   0 root         (0) root         (0)     2814 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/constraint_components/penalty_component.py
--rw-rw-rw-   0 root         (0) root         (0)      287 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/constraint_components/post_constraint.py
--rw-rw-rw-   0 root         (0) root         (0)    15096 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/constraint_components/spacing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:55:44.159452 topfarm-2.3.2/topfarm/cost_models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/cost_models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1204 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/cost_models/aggregated_cost.py
--rw-rw-rw-   0 root         (0) root         (0)    13251 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/cost_models/cost_model_wrappers.py
--rw-rw-rw-   0 root         (0) root         (0)     1994 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/cost_models/dummy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:55:44.159452 topfarm-2.3.2/topfarm/cost_models/economic_models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/cost_models/economic_models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21836 2023-03-24 11:54:07.000000 topfarm-2.3.2/topfarm/cost_models/economic_models/dtu_wind_cm_main.py
--rw-rw-rw-   0 root         (0) root         (0)    12298 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/cost_models/economic_models/turbine_cost.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:55:44.159452 topfarm-2.3.2/topfarm/cost_models/electrical/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/cost_models/electrical/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3512 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/cost_models/electrical/simple_msp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:55:44.159452 topfarm-2.3.2/topfarm/cost_models/fuga/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/cost_models/fuga/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1776 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/cost_models/fuga/py_fuga.py
--rw-rw-rw-   0 root         (0) root         (0)     6554 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/cost_models/py_wake_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:55:44.159452 topfarm-2.3.2/topfarm/cost_models/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/cost_models/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3728 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/cost_models/utils/spanning_tree.py
--rw-rw-rw-   0 root         (0) root         (0)     6317 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/deprectated_topfarm_problems.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:55:44.159452 topfarm-2.3.2/topfarm/drivers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/drivers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    28811 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/drivers/genetic_algorithm_driver.py
--rw-rw-rw-   0 root         (0) root         (0)    14453 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/drivers/random_search_driver.py
--rw-rw-rw-   0 root         (0) root         (0)     9561 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/drivers/stochastic_gradient_descent_driver.py
--rw-rw-rw-   0 root         (0) root         (0)    15379 2023-03-17 08:19:32.000000 topfarm-2.3.2/topfarm/easy_drivers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:55:44.159452 topfarm-2.3.2/topfarm/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/examples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:55:44.159452 topfarm-2.3.2/topfarm/examples/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/examples/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2057 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/examples/data/parque_ficticio_offshore.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:55:44.159452 topfarm-2.3.2/topfarm/examples/iea37/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/examples/iea37/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2674 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/examples/iea37/_iea37.py
--rw-rw-rw-   0 root         (0) root         (0)    32326 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/mongo_recorder.py
--rw-rw-rw-   0 root         (0) root         (0)     3201 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/parallel_runner.py
--rw-rw-rw-   0 root         (0) root         (0)    15346 2023-03-17 10:31:15.000000 topfarm-2.3.2/topfarm/plotting.py
--rw-rw-rw-   0 root         (0) root         (0)    10102 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/recorders.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:55:44.163452 topfarm-2.3.2/topfarm/tests/
--rw-rw-rw-   0 root         (0) root         (0)       93 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6112 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/tests/notebook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:55:44.163452 topfarm-2.3.2/topfarm/tests/test_constraint/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/tests/test_constraint/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2852 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/tests/test_constraint/test_BoundaryBaseComp.py
--rw-rw-rw-   0 root         (0) root         (0)     4218 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/tests/test_constraint/test_CircleBoundaryComp.py
--rw-rw-rw-   0 root         (0) root         (0)     3921 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/tests/test_constraint/test_ConvexBoundaryComp.py
--rw-rw-rw-   0 root         (0) root         (0)     4082 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/tests/test_constraint/test_PolygonBoundaryComp.py
--rw-rw-rw-   0 root         (0) root         (0)     7439 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/tests/test_constraint/test_boundary_polygon.py
--rw-rw-rw-   0 root         (0) root         (0)     1726 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/tests/test_constraint/test_capacityComp.py
--rw-rw-rw-   0 root         (0) root         (0)     4663 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/tests/test_constraint/test_constrained_generator.py
--rw-rw-rw-   0 root         (0) root         (0)     9763 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/tests/test_constraint/test_loads.py
--rw-rw-rw-   0 root         (0) root         (0)     8115 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/tests/test_constraint/test_spacingComp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:55:44.163452 topfarm-2.3.2/topfarm/tests/test_costmodel_utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/tests/test_costmodel_utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5974 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/tests/test_costmodel_utils/test_cost_model_wrappers.py
--rw-rw-rw-   0 root         (0) root         (0)     1416 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/tests/test_costmodel_utils/test_spanning_tree.py
--rw-rw-rw-   0 root         (0) root         (0)     2794 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/tests/test_examples.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:55:44.163452 topfarm-2.3.2/topfarm/tests/test_files/
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/tests/test_files/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:55:44.163452 topfarm-2.3.2/topfarm/tests/test_files/example_data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/tests/test_files/example_data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:55:44.163452 topfarm-2.3.2/topfarm/tests/test_files/example_data/floris/
--rw-rw-rw-   0 root         (0) root         (0)    26115 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/tests/test_files/example_data/floris/NREL5MW.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/tests/test_files/example_data/floris/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1443 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/tests/test_files/xy3tb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:55:44.163452 topfarm-2.3.2/topfarm/tests/test_fuga/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/tests/test_fuga/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8890 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/tests/test_fuga/test_pyfuga.py
--rw-rw-rw-   0 root         (0) root         (0)     1586 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/tests/test_main.py
--rw-rw-rw-   0 root         (0) root         (0)     1727 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/tests/test_notebooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:55:44.167452 topfarm-2.3.2/topfarm/tests/test_topfarm_problems/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/tests/test_topfarm_problems/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10857 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/tests/test_topfarm_problems/test_TopFarmProblem.py
--rw-rw-rw-   0 root         (0) root         (0)     5252 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/tests/test_topfarm_problems/test_TopFarmProblem_limits_and_constraints.py
--rw-rw-rw-   0 root         (0) root         (0)     2196 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/tests/test_topfarm_problems/test_nested_problems.py
--rw-rw-rw-   0 root         (0) root         (0)     1564 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/tests/test_topfarm_problems/test_optimization_problems.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:55:44.167452 topfarm-2.3.2/topfarm/tests/test_topfarm_utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/tests/test_topfarm_utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10588 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/tests/test_topfarm_utils/test_drivers.py
--rw-rw-rw-   0 root         (0) root         (0)     1224 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/tests/test_topfarm_utils/test_parellel_runner.py
--rw-rw-rw-   0 root         (0) root         (0)    10986 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/tests/test_topfarm_utils/test_recorders.py
--rw-rw-rw-   0 root         (0) root         (0)    12447 2023-03-15 20:00:54.000000 topfarm-2.3.2/topfarm/tests/test_topfarm_utils/test_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1025 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/tests/test_with_dummy.py
--rw-rw-rw-   0 root         (0) root         (0)    18417 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2282 2023-03-15 10:02:58.000000 topfarm-2.3.2/topfarm/workshop.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:55:44.155452 topfarm-2.3.2/topfarm.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1005 2023-03-27 12:55:43.000000 topfarm-2.3.2/topfarm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4467 2023-03-27 12:55:44.000000 topfarm-2.3.2/topfarm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-27 12:55:43.000000 topfarm-2.3.2/topfarm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      199 2023-03-27 12:55:43.000000 topfarm-2.3.2/topfarm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-03-27 12:55:43.000000 topfarm-2.3.2/topfarm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-27 12:55:43.000000 topfarm-2.3.2/topfarm.egg-info/zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:23:03.926867 topfarm-2.3.4/
+-rw-rw-rw-   0 root         (0) root         (0)     1064 2023-12-02 14:20:16.000000 topfarm-2.3.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1481 2024-05-16 06:23:03.926867 topfarm-2.3.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      750 2023-12-02 14:20:16.000000 topfarm-2.3.4/README
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:23:03.914867 topfarm-2.3.4/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 06:22:49.000000 topfarm-2.3.4/examples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:23:03.914867 topfarm-2.3.4/examples/irp_wind/
+-rw-rw-rw-   0 root         (0) root         (0)     1704 2023-12-02 14:20:16.000000 topfarm-2.3.4/examples/irp_wind/Hornsrev_aep.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 06:22:49.000000 topfarm-2.3.4/examples/irp_wind/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3106 2023-12-02 14:20:16.000000 topfarm-2.3.4/examples/irp_wind/optimization_3tb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:23:03.918867 topfarm-2.3.4/examples/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 06:22:49.000000 topfarm-2.3.4/examples/scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4624 2023-12-02 14:20:16.000000 topfarm-2.3.4/examples/scripts/example_10_mongodb.py
+-rw-rw-rw-   0 root         (0) root         (0)     1714 2023-12-02 14:20:16.000000 topfarm-2.3.4/examples/scripts/example_13_automatic_differentiation.py
+-rw-rw-rw-   0 root         (0) root         (0)     3772 2023-12-02 14:20:16.000000 topfarm-2.3.4/examples/scripts/example_14_regular_grid_optimization.py
+-rw-rw-rw-   0 root         (0) root         (0)     7995 2023-12-02 14:20:16.000000 topfarm-2.3.4/examples/scripts/example_15_sgd_driver.py
+-rw-rw-rw-   0 root         (0) root         (0)     2741 2023-12-02 14:20:16.000000 topfarm-2.3.4/examples/scripts/example_16_smart_start_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     3955 2023-12-02 14:20:16.000000 topfarm-2.3.4/examples/scripts/example_1_constrained_layout_optimization.py
+-rw-rw-rw-   0 root         (0) root         (0)     5732 2023-12-02 14:20:16.000000 topfarm-2.3.4/examples/scripts/example_2_wake_comparison.py
+-rw-rw-rw-   0 root         (0) root         (0)     2382 2023-12-02 14:20:16.000000 topfarm-2.3.4/examples/scripts/example_3_turbine_type_optimization.py
+-rw-rw-rw-   0 root         (0) root         (0)     2921 2023-12-02 14:20:16.000000 topfarm-2.3.4/examples/scripts/example_4_integrated_optimization_aep_and_irr.py
+-rw-rw-rw-   0 root         (0) root         (0)     3331 2023-12-02 14:20:16.000000 topfarm-2.3.4/examples/scripts/example_5_integrated_opt_with_dtu_cost_model.py
+-rw-rw-rw-   0 root         (0) root         (0)    11228 2023-12-02 14:20:16.000000 topfarm-2.3.4/examples/scripts/example_6_floris.py
+-rw-rw-rw-   0 root         (0) root         (0)     2820 2023-12-02 14:20:16.000000 topfarm-2.3.4/examples/scripts/example_7_parallel_cost_comp_mpi.py
+-rw-rw-rw-   0 root         (0) root         (0)     4204 2023-12-02 14:20:16.000000 topfarm-2.3.4/examples/scripts/example_9_irr_opt_on_weibull_site.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2024-05-16 06:23:03.926867 topfarm-2.3.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1733 2024-04-30 08:22:52.000000 topfarm-2.3.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:23:03.918867 topfarm-2.3.4/topfarm/
+-rw-rw-rw-   0 root         (0) root         (0)      378 2024-05-16 06:23:03.000000 topfarm-2.3.4/topfarm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    30668 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/_topfarm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:23:03.922867 topfarm-2.3.4/topfarm/constraint_components/
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/constraint_components/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      573 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/constraint_components/_constraint.py
+-rw-rw-rw-   0 root         (0) root         (0)    51064 2024-04-30 08:22:52.000000 topfarm-2.3.4/topfarm/constraint_components/boundary.py
+-rw-rw-rw-   0 root         (0) root         (0)    18987 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/constraint_components/boundary_component.py
+-rw-rw-rw-   0 root         (0) root         (0)     2388 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/constraint_components/capacity.py
+-rw-rw-rw-   0 root         (0) root         (0)     2812 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/constraint_components/constrained_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     4686 2023-12-11 11:41:32.000000 topfarm-2.3.4/topfarm/constraint_components/constraint_aggregation.py
+-rw-rw-rw-   0 root         (0) root         (0)    12685 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/constraint_components/load.py
+-rw-rw-rw-   0 root         (0) root         (0)     2968 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/constraint_components/penalty_component.py
+-rw-rw-rw-   0 root         (0) root         (0)    15029 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/constraint_components/spacing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:23:03.922867 topfarm-2.3.4/topfarm/cost_models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 06:22:49.000000 topfarm-2.3.4/topfarm/cost_models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13424 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/cost_models/cost_model_wrappers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1994 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/cost_models/dummy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:23:03.922867 topfarm-2.3.4/topfarm/cost_models/economic_models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 06:22:49.000000 topfarm-2.3.4/topfarm/cost_models/economic_models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21836 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/cost_models/economic_models/dtu_wind_cm_main.py
+-rw-rw-rw-   0 root         (0) root         (0)    12298 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/cost_models/economic_models/turbine_cost.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:23:03.922867 topfarm-2.3.4/topfarm/cost_models/electrical/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 06:22:49.000000 topfarm-2.3.4/topfarm/cost_models/electrical/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3512 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/cost_models/electrical/simple_msp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:23:03.922867 topfarm-2.3.4/topfarm/cost_models/fuga/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 06:22:49.000000 topfarm-2.3.4/topfarm/cost_models/fuga/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1776 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/cost_models/fuga/py_fuga.py
+-rw-rw-rw-   0 root         (0) root         (0)    10203 2023-12-11 10:49:48.000000 topfarm-2.3.4/topfarm/cost_models/py_wake_wrapper.py
+-rw-rw-rw-   0 root         (0) root         (0)     6671 2024-03-18 10:12:11.000000 topfarm-2.3.4/topfarm/cost_models/topfarm_components.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:23:03.922867 topfarm-2.3.4/topfarm/cost_models/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 06:22:49.000000 topfarm-2.3.4/topfarm/cost_models/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3728 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/cost_models/utils/spanning_tree.py
+-rw-rw-rw-   0 root         (0) root         (0)     6317 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/deprectated_topfarm_problems.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:23:03.922867 topfarm-2.3.4/topfarm/drivers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 06:22:49.000000 topfarm-2.3.4/topfarm/drivers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    28875 2024-05-02 09:10:15.000000 topfarm-2.3.4/topfarm/drivers/genetic_algorithm_driver.py
+-rw-rw-rw-   0 root         (0) root         (0)    14453 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/drivers/random_search_driver.py
+-rw-rw-rw-   0 root         (0) root         (0)     9561 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/drivers/stochastic_gradient_descent_driver.py
+-rw-rw-rw-   0 root         (0) root         (0)    15660 2024-05-02 08:23:44.000000 topfarm-2.3.4/topfarm/easy_drivers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:23:03.922867 topfarm-2.3.4/topfarm/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 06:22:49.000000 topfarm-2.3.4/topfarm/examples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:23:03.922867 topfarm-2.3.4/topfarm/examples/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 06:22:49.000000 topfarm-2.3.4/topfarm/examples/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2079 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/examples/data/parque_ficticio_offshore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:23:03.922867 topfarm-2.3.4/topfarm/examples/iea37/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/examples/iea37/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2759 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/examples/iea37/_iea37.py
+-rw-rw-rw-   0 root         (0) root         (0)    32395 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/mongo_recorder.py
+-rw-rw-rw-   0 root         (0) root         (0)     3201 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/parallel_runner.py
+-rw-rw-rw-   0 root         (0) root         (0)    14976 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/plotting.py
+-rw-rw-rw-   0 root         (0) root         (0)    10103 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/recorders.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:23:03.922867 topfarm-2.3.4/topfarm/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       93 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6112 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/tests/notebook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:23:03.926867 topfarm-2.3.4/topfarm/tests/test_constraint/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 06:22:49.000000 topfarm-2.3.4/topfarm/tests/test_constraint/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2852 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/tests/test_constraint/test_BoundaryBaseComp.py
+-rw-rw-rw-   0 root         (0) root         (0)     4174 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/tests/test_constraint/test_CircleBoundaryComp.py
+-rw-rw-rw-   0 root         (0) root         (0)     3921 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/tests/test_constraint/test_ConvexBoundaryComp.py
+-rw-rw-rw-   0 root         (0) root         (0)     4082 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/tests/test_constraint/test_PolygonBoundaryComp.py
+-rw-rw-rw-   0 root         (0) root         (0)     8492 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/tests/test_constraint/test_boundary_polygon.py
+-rw-rw-rw-   0 root         (0) root         (0)     1744 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/tests/test_constraint/test_capacityComp.py
+-rw-rw-rw-   0 root         (0) root         (0)     4663 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/tests/test_constraint/test_constrained_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     9763 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/tests/test_constraint/test_loads.py
+-rw-rw-rw-   0 root         (0) root         (0)     8128 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/tests/test_constraint/test_spacingComp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:23:03.926867 topfarm-2.3.4/topfarm/tests/test_costmodel_utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 06:22:49.000000 topfarm-2.3.4/topfarm/tests/test_costmodel_utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5974 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/tests/test_costmodel_utils/test_cost_model_wrappers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1896 2023-12-11 10:49:48.000000 topfarm-2.3.4/topfarm/tests/test_costmodel_utils/test_cost_pywake_wrappers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1416 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/tests/test_costmodel_utils/test_spanning_tree.py
+-rw-rw-rw-   0 root         (0) root         (0)     2794 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/tests/test_examples.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:23:03.926867 topfarm-2.3.4/topfarm/tests/test_files/
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/tests/test_files/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:23:03.926867 topfarm-2.3.4/topfarm/tests/test_files/example_data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 06:22:49.000000 topfarm-2.3.4/topfarm/tests/test_files/example_data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:23:03.926867 topfarm-2.3.4/topfarm/tests/test_files/example_data/floris/
+-rw-rw-rw-   0 root         (0) root         (0)    26115 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/tests/test_files/example_data/floris/NREL5MW.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 06:22:49.000000 topfarm-2.3.4/topfarm/tests/test_files/example_data/floris/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1443 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/tests/test_files/xy3tb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:23:03.926867 topfarm-2.3.4/topfarm/tests/test_fuga/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 06:22:49.000000 topfarm-2.3.4/topfarm/tests/test_fuga/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8890 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/tests/test_fuga/test_pyfuga.py
+-rw-rw-rw-   0 root         (0) root         (0)     1586 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/tests/test_main.py
+-rw-rw-rw-   0 root         (0) root         (0)     1727 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/tests/test_notebooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:23:03.926867 topfarm-2.3.4/topfarm/tests/test_topfarm_problems/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 06:22:49.000000 topfarm-2.3.4/topfarm/tests/test_topfarm_problems/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11032 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/tests/test_topfarm_problems/test_TopFarmProblem.py
+-rw-rw-rw-   0 root         (0) root         (0)     5252 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/tests/test_topfarm_problems/test_TopFarmProblem_limits_and_constraints.py
+-rw-rw-rw-   0 root         (0) root         (0)     2196 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/tests/test_topfarm_problems/test_nested_problems.py
+-rw-rw-rw-   0 root         (0) root         (0)     1564 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/tests/test_topfarm_problems/test_optimization_problems.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:23:03.926867 topfarm-2.3.4/topfarm/tests/test_topfarm_utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 06:22:49.000000 topfarm-2.3.4/topfarm/tests/test_topfarm_utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10594 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/tests/test_topfarm_utils/test_drivers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1224 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/tests/test_topfarm_utils/test_parellel_runner.py
+-rw-rw-rw-   0 root         (0) root         (0)    10986 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/tests/test_topfarm_utils/test_recorders.py
+-rw-rw-rw-   0 root         (0) root         (0)    12447 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/tests/test_topfarm_utils/test_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1025 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/tests/test_with_dummy.py
+-rw-rw-rw-   0 root         (0) root         (0)    18409 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2282 2023-12-02 14:20:16.000000 topfarm-2.3.4/topfarm/workshop.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:23:03.926867 topfarm-2.3.4/topfarm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1481 2024-05-16 06:23:03.000000 topfarm-2.3.4/topfarm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4485 2024-05-16 06:23:03.000000 topfarm-2.3.4/topfarm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 06:23:03.000000 topfarm-2.3.4/topfarm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      206 2024-05-16 06:23:03.000000 topfarm-2.3.4/topfarm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-16 06:23:03.000000 topfarm-2.3.4/topfarm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 06:23:03.000000 topfarm-2.3.4/topfarm.egg-info/zip-safe
```

### Comparing `topfarm-2.3.2/LICENSE` & `topfarm-2.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `topfarm-2.3.2/PKG-INFO` & `topfarm-2.3.4/README`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: topfarm
-Version: 2.3.2
-Summary: Topfarm - Wind farm optimization using OpenMDAO
-Home-page: https://gitlab.windenergy.dtu.dk/TOPFARM/topfarm2
-Author: DTU Wind Energy
-Author-email: mikf@dtu.dk
-License: MIT
-License-File: LICENSE
-
 |pipeline status| |coverage report|
 
 Welcome to TOPFARM
 ------------------
 
 This is the plant-level optimization tool that is being developed by DTU
 Wind Energy.
```

### Comparing `topfarm-2.3.2/examples/irp_wind/Hornsrev_aep.py` & `topfarm-2.3.4/examples/irp_wind/Hornsrev_aep.py`

 * *Files identical despite different names*

### Comparing `topfarm-2.3.2/examples/irp_wind/optimization_3tb.py` & `topfarm-2.3.4/examples/irp_wind/optimization_3tb.py`

 * *Files identical despite different names*

### Comparing `topfarm-2.3.2/examples/scripts/example_10_mongodb.py` & `topfarm-2.3.4/examples/scripts/example_10_mongodb.py`

 * *Files identical despite different names*

### Comparing `topfarm-2.3.2/examples/scripts/example_13_automatic_differentiation.py` & `topfarm-2.3.4/examples/scripts/example_13_automatic_differentiation.py`

 * *Files identical despite different names*

### Comparing `topfarm-2.3.2/examples/scripts/example_14_regular_grid_optimization.py` & `topfarm-2.3.4/examples/scripts/example_14_regular_grid_optimization.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,18 @@
 from topfarm.easy_drivers import EasyScipyOptimizeDriver
 from topfarm.cost_models.cost_model_wrappers import CostModelComponent
 from topfarm.constraint_components.boundary import XYBoundaryConstraint
 from topfarm.constraint_components.spacing import SpacingConstraint
 from topfarm.utils import regular_generic_layout, regular_generic_layout_gradients
 
 
-def main():
-    if __name__ == '__main__':
+# def main():
+#     if __name__ == '__main__':
+if 1:
+    if 1:
         site = Hornsrev1Site()
         wt = V80()
         D = wt.diameter()
         windFarmModel = BastankhahGaussian(site, wt)
         n_wt = 16
         stagger = 1 * D
 
@@ -33,15 +35,15 @@
                                                        ('sy', 0),
                                                        ('rotation', 0)],
                                       n_wt=n_wt,
                                       cost_function=reg_func,
                                       cost_gradient_function = reg_grad,
                                       output_keys= [('x', np.zeros(n_wt)), ('y', np.zeros(n_wt))],
                                       objective=False,
-                                      use_penalty=False,
+                                      use_constraint_violation=False,
                                       )
 
         # AEP function 
         def aep_fun(x, y):
             aep = windFarmModel(x, y).aep().sum()
             return aep
 
@@ -75,8 +77,8 @@
                                  plot_comp=XYPlotComp(),
                                  expected_cost=ec,
                                  )
 
         # problem.evaluate()
         cost, state, recorder = problem.optimize()
 
-main()
+# main()
```

### Comparing `topfarm-2.3.2/examples/scripts/example_15_sgd_driver.py` & `topfarm-2.3.4/examples/scripts/example_15_sgd_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,25 @@
 from py_wake.examples.data.iea37._iea37 import IEA37_WindTurbines
 from py_wake.deficit_models.gaussian import BastankhahGaussian
 from py_wake.examples.data.lillgrund import LillgrundSite
 from py_wake.utils.gradients import autograd
 from py_wake.examples.data.hornsrev1 import Hornsrev1Site, HornsrevV80
 from topfarm.cost_models.cost_model_wrappers import CostModelComponent
 from topfarm.easy_drivers import EasySGDDriver, EasyScipyOptimizeDriver
-from topfarm.plotting import AggregatedConstraintsPlotComponent, XYPlotComp
+from topfarm.plotting import XYPlotComp #AggregatedConstraintsPlotComponent, 
 from topfarm.constraint_components.spacing import SpacingConstraint
 from topfarm import TopFarmProblem
 from topfarm.constraint_components.boundary import XYBoundaryConstraint
 from topfarm.recorders import TopFarmListRecorder
 
 
-def main():
-    if __name__ == '__main__':
+# def main():
+#     if __name__ == '__main__':
+if 1:
+    if 1:
         plt.close('all')
 
         site = LillgrundSite()
         site.interp_method = 'linear'
         windTurbines = HornsrevV80() 
         wake_model = BastankhahGaussian(site, windTurbines) 
 
@@ -112,30 +114,32 @@
         component_args = {'input_keys': [('wtSeparationSquared', np.zeros(int(n_wt * (n_wt - 1) / 2))),
                                          ('boundaryDistances', np.zeros((n_wt, 4)))],
                           'n_wt': n_wt,
                           'cost_function': constr_aggr_func,
                           'cost_gradient_function': constr_aggr_grad,
                           'objective': False,
                           'output_keys': [(name, 0)],
-                          'use_penalty': False}
+                          'use_constraint_violation': False
+                          }
         constraint_args = {'name': name, 'lower': 0}
         from topfarm.constraint_components.constraint_aggregation import ConstraintAggregation
 
         driver_names = ['SLSQP', 'SGD']
         drivers = [EasyScipyOptimizeDriver(maxiter=200, tol=1e-3), EasySGDDriver(maxiter=400, learning_rate=windTurbines.diameter() / 5, max_time=30 * 60, speedupSGD=True, sgd_thresh=0.5)]
         driver_no = 1
         constraints = [[SpacingConstraint(2 * windTurbines.diameter()), constraint_comp], ConstraintAggregation([SpacingConstraint(2 * windTurbines.diameter()), constraint_comp],
                                                   component_args=component_args, constraint_args=constraint_args)]
         ecs = [1e2, 1]
         tf = TopFarmProblem(
                 design_vars={'x':(x,0,xu), 'y':(y,0,yu)}, # setting up our two turbines as design variables
                 cost_comp=cost_comps[driver_no], # using dummy cost model
                 constraints=constraints[driver_no], # constraint set up for the boundary type provided)
                 driver=drivers[driver_no],
-                plot_comp=[XYPlotComp(), AggregatedConstraintsPlotComponent()][driver_no],
+                # plot_comp=[XYPlotComp(), AggregatedConstraintsPlotComponent()][driver_no],
+                plot_comp=[XYPlotComp(), XYPlotComp()][driver_no],
                 expected_cost=ecs[driver_no],
                 )
         #tf.driver.learning_rate = windTurbines.diameter() / 5
         if 1:
             cost, state, recorder = tf.optimize()
             recorder.save(f'{driver_names[driver_no]}')
 
@@ -154,8 +158,8 @@
                     #     aep = 
                 plt.plot(rec['timestamp']-rec['timestamp'][0], aep, label=driver_names[i])
             plt.legend()
             plt.savefig('conv')
             plt.clf()
             # plt.plot()
 
-main()
+# main()
```

### Comparing `topfarm-2.3.2/examples/scripts/example_16_smart_start_types.py` & `topfarm-2.3.4/examples/scripts/example_16_smart_start_types.py`

 * *Files identical despite different names*

### Comparing `topfarm-2.3.2/examples/scripts/example_1_constrained_layout_optimization.py` & `topfarm-2.3.4/examples/scripts/example_1_constrained_layout_optimization.py`

 * *Files identical despite different names*

### Comparing `topfarm-2.3.2/examples/scripts/example_2_wake_comparison.py` & `topfarm-2.3.4/examples/scripts/example_2_wake_comparison.py`

 * *Files identical despite different names*

### Comparing `topfarm-2.3.2/examples/scripts/example_3_turbine_type_optimization.py` & `topfarm-2.3.4/examples/scripts/example_3_turbine_type_optimization.py`

 * *Files identical despite different names*

### Comparing `topfarm-2.3.2/examples/scripts/example_4_integrated_optimization_aep_and_irr.py` & `topfarm-2.3.4/examples/scripts/example_4_integrated_optimization_aep_and_irr.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,15 +54,15 @@
             output_unit="%",
             objective=True,
             maximize=True)
         group = TopFarmGroup([aep_comp, irr_comp])
         problem = TopFarmProblem(
             design_vars=dict(zip('xy', site.initial_position.T)),
             cost_comp=group,
-            driver=EasyRandomSearchDriver(randomize_func=RandomizeTurbinePosition_Circle(), max_iter=5),
+            driver=EasyRandomSearchDriver(randomize_func=RandomizeTurbinePosition_Circle(600), max_iter=5, max_time=10),
             constraints=[SpacingConstraint(200),
                          CircleBoundaryConstraint([0, 0], 1300.1)],
             plot_comp=plot_comp)
         cost, state, recorder = problem.optimize()
         #        problem.evaluate()
         n2(problem, outfile='example_4_integrated_optimization_aep_and_irr_n2.html', show_browser=False)
```

### Comparing `topfarm-2.3.2/examples/scripts/example_5_integrated_opt_with_dtu_cost_model.py` & `topfarm-2.3.4/examples/scripts/example_5_integrated_opt_with_dtu_cost_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
             output_unit="%",
             objective=True,
             maximize=True)
         group = TopFarmGroup([aep_comp, irr_comp])
         problem = TopFarmProblem(
             design_vars=dict(zip('xy', site.initial_position.T)),
             cost_comp=group,
-            driver=EasyRandomSearchDriver(randomize_func=RandomizeTurbinePosition_Circle(), max_iter=5),
+            driver=EasyRandomSearchDriver(randomize_func=RandomizeTurbinePosition_Circle(), max_iter=5, max_time=10),
             constraints=[SpacingConstraint(200),
                          CircleBoundaryConstraint([0, 0], 1300.1)],
             plot_comp=plot_comp)
         cost, state, recorder = problem.optimize()
         #        problem.evaluate()
 #        n2(problem, outfile='example_4_integrated_optimization_aep_and_irr_n2.html', show_browser=False)
```

### Comparing `topfarm-2.3.2/examples/scripts/example_6_floris.py` & `topfarm-2.3.4/examples/scripts/example_6_floris.py`

 * *Files identical despite different names*

### Comparing `topfarm-2.3.2/examples/scripts/example_7_parallel_cost_comp_mpi.py` & `topfarm-2.3.4/examples/scripts/example_7_parallel_cost_comp_mpi.py`

 * *Files identical despite different names*

### Comparing `topfarm-2.3.2/examples/scripts/example_9_irr_opt_on_weibull_site.py` & `topfarm-2.3.4/examples/scripts/example_9_irr_opt_on_weibull_site.py`

 * *Files identical despite different names*

### Comparing `topfarm-2.3.2/setup.py` & `topfarm-2.3.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 # -*- coding: utf-8 -*-
 """
 Setup file for Topfarm2
 """
 
 
 import os
-from git_utils import write_vers
 from setuptools import setup, find_packages
 
 repo = os.path.dirname(__file__)
-version = write_vers(vers_file='topfarm/__init__.py', repo=repo, skip_chars=1)
+try:
+    from git_utils import write_vers
+    version = write_vers(vers_file='topfarm/__init__.py', repo=repo, skip_chars=1)
+except Exception:
+    version = '999'
+
 
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(name='topfarm',
@@ -25,20 +29,20 @@
       author_email='mikf@dtu.dk',
       license='MIT',
       packages=find_packages(),
       install_requires=[
               'matplotlib',  # for plotting
               'numpy',  # for numerical calculations
               'numpy-financial',  # for irr calculations
-              'openmdao>=3.16',  # for optimization
+              'openmdao>=3.16, <=3.26',  # for optimization
               'pytest',  # for testing
               'pycodestyle',  # for testing
               'pytest-cov',  # for calculating coverage
               'py_wake>=2',  # for calculating AEP
-              'pyDOE2',  # for GA driver
+              'pyDOE3',  # for GA driver
               'pymongo[srv]',  # for mongo_recorder
               'scipy',  # constraints
               'sphinx',  # generating documentation
               'sphinx_rtd_theme',  # docs theme
               'scikit-learn',  # load surrogate
               'mock',  # replace variables during tests
               'tensorflow',  # loads examples with surrogates
```

### Comparing `topfarm-2.3.2/topfarm/_topfarm.py` & `topfarm-2.3.4/topfarm/_topfarm.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,32 +18,33 @@
 ```from openmdao.utils import mpi
 mpi.MPI = None```
 """
 import time
 import numpy as np
 import warnings
 import copy
+import inspect
 from openmdao.api import Problem, IndepVarComp, Group, ParallelGroup,\
     ExplicitComponent, ListGenerator, DOEDriver, SimpleGADriver, OpenMDAOWarning
 from openmdao.drivers.doe_generators import DOEGenerator
 from openmdao.utils import mpi
 from openmdao.core.constants import _SetupStatus
 import topfarm
 from topfarm.recorders import NestedTopFarmListRecorder,\
     TopFarmListRecorder, split_record_id
 from topfarm.mongo_recorder import MongoRecorder
 from topfarm.plotting import NoPlot
-from topfarm.easy_drivers import EasyScipyOptimizeDriver, EasySimpleGADriver, EasyDriverBase
+from topfarm.easy_drivers import EasyScipyOptimizeDriver, EasySimpleGADriver, EasyDriverBase, EasySGDDriver
 from topfarm.utils import smart_start
 from topfarm.constraint_components.spacing import SpacingComp, SpacingTypeComp
 from topfarm.constraint_components.boundary import BoundaryBaseComp
-from topfarm.constraint_components.penalty_component import PenaltyComponent, PostPenaltyComponent
-from topfarm.cost_models.aggregated_cost import AggregatedCost
+# from topfarm.constraint_components.penalty_component import ConstraintViolationComponent, PenaltyComponent #, PostPenaltyComponent
+from topfarm.cost_models.topfarm_components import ObjectiveComponent, DummyObjectiveComponent, ConstraintViolationComponent
 from topfarm.cost_models.cost_model_wrappers import CostModelComponent
-from topfarm.constraint_components.post_constraint import PostConstraint
+# from topfarm.constraint_components.post_constraint import PostConstraint
 from topfarm.constraint_components import Constraint
 
 
 class TopFarmBaseGroup(Group):
     def __init__(self, comps=[], output_key=None, output_unit=''):
         super().__init__()
         self.comps = []
@@ -75,17 +76,17 @@
         self.add_subsystem('objective', self.obj_comp, promotes=['*'])
 
 
 class TopFarmProblem(Problem):
 
     def __init__(self, design_vars, cost_comp=None, driver=EasyScipyOptimizeDriver(),
                  constraints=[], plot_comp=NoPlot(), record_id=None,
-                 expected_cost=1, ext_vars={}, post_constraints=[], approx_totals=False,
+                 expected_cost=1, ext_vars={}, approx_totals=False,
                  recorder=None, additional_recorders=None,
-                 n_wt=0, grid_layout_comp=None):
+                 n_wt=0, grid_layout_comp=None, penalty_comp=None, reports=None, **kwargs):
         """Initialize TopFarmProblem
 
         Parameters
         ----------
         design_vars : dict or list of key-initial_value-tuples
             Design variables for the problem.\n
             Ex: {'x': [1,2,3], 'y':([3,2,1],0,1), 'z':([4,5,6],[4,5,4], [6,7,6])}\n
@@ -105,16 +106,21 @@
             Pure python cost functions can be wrapped using ``CostModelComponent``
             class in ``topfarm.cost_models.cost_model_wrappers``.\n
             ExplicitComponent are wrapped into a TopFarmGroup.\n
             For nested problems, the cost comp_comp is typically a TopFarmProblem
         driver : openmdao Driver, optinal
             Driver used to solve the optimization driver. For an example, see the
             ``EasyScipyOptimizeDriver`` class in ``topfarm.easy_drivers``.
-        constraints : list of Constraint-objects
-            E.g. XYBoundaryConstraint, SpacingConstraint
+        constraints : list of Constraint-objects or tuples
+            Constraint-objects are e.g. XYBoundaryConstraint, SpacingConstraint
+            Tuples have the form (variable to constrain, {dict with options passed to the the OpenMDAO method add_constraint})
+        penalty_comp : ExplicitComponent, optional
+            Component that converts constraints into penalty both for drivers that do and do not support constraints.
+            Constraints are automatically converted to penalty for drivers that do not support constraints and the default magnitude of the
+            penalty that is added to the objective is the sum of the constraint violations + 10**10.
         plot_comp : ExplicitComponent, optional
             OpenMDAO ExplicitComponent used to plot the state (during
             optimization).
             For no plotting, pass in the ``topfarm.plotting.NoPlot`` class.
         record_id : string "<record_id>:<case>", optional
             Identifier for the optimization. Allows a user to restart an
             optimization where it left off.\n
@@ -128,17 +134,14 @@
             Used to scale the cost, default is 1. This has influence on some drivers, e.g.
             SLSQP where it affects the step size\n
             If None, the value is found by evaluating the cost function
         ext_vars : dict or list of key-initial_value tuple
             Used for nested problems to propagate variables from parent problem\n
             Ex. {'type': [1,2,3]}\n
             Ex. [('type', [1,2,3])]\n
-        post_constraints : list of Constraint-objects that needs the cost component to be
-            evaluated, unlike (pre-)constraints which are evaluated before the cost component.
-            E.g. LoadConstraint
         approx_totals : bool or dict
             If True, approximates the total derivative of the cost_comp group,
             skipping the partial ones. If it is a dictionary, it's elements
             are passed to the approx_totals function of an OpenMDAO Group.
         recorder : Main recorder
         additional_recorders: list(Recorder) or None
             A list of additional recorders to be added to the problem
@@ -160,16 +163,29 @@
             comm = None
         else:
             from openmdao.utils.mpi import FakeComm
             comm = FakeComm()
 
         self.main_recorder = recorder
         self._additional_recorders = additional_recorders
+        if not isinstance(constraints, list):
+            constraints = [constraints]
+        if 'post_constraints' in kwargs:
+            warnings.warn("""post_constraints keyword is deprecated. Both Constraint objects and
+                          constraint tuples of type (keyword, {constraint options}) can be included in the constriants list.""",
+                          DeprecationWarning, stacklevel=2)
 
-        Problem.__init__(self, comm=comm)
+            post_constraints = kwargs['post_constraints']
+        else:
+            post_constraints = [constraint for constraint in constraints if isinstance(constraint, dict) or isinstance(constraint, tuple)]
+            constraints = [constraint for constraint in constraints if isinstance(constraint, Constraint)]
+        if 'reports' not in inspect.getfullargspec(Problem.__init__).args:
+            Problem.__init__(self, comm=comm)
+        else:
+            Problem.__init__(self, comm=comm, reports=reports)
         if cost_comp:
             if isinstance(cost_comp, TopFarmProblem):
                 cost_comp = cost_comp.as_component()
             elif isinstance(cost_comp, ExplicitComponent) and (len(post_constraints) > 0):
                 cost_comp = TopFarmGroup([cost_comp])
             cost_comp.parent = self
         self.cost_comp = cost_comp
@@ -186,16 +202,14 @@
 
         self.plot_comp = plot_comp
 
         self.record_id = record_id
         self.load_recorder()
         if not isinstance(approx_totals, dict) and approx_totals:
             approx_totals = {'method': 'fd'}
-        if not isinstance(constraints, list):
-            constraints = [constraints]
         if not isinstance(design_vars, dict):
             design_vars = dict(design_vars)
         self.design_vars = design_vars
         self.indeps = self.model.add_subsystem('indeps', IndepVarComp(), promotes=['*'])
         for k, v in design_vars.items():
             if isinstance(v, tuple):
                 if (not isinstance(v[-1], str)) or (not v[-1]):
@@ -220,78 +234,75 @@
         for k, v in ext_vars.items():
             self.indeps.add_output(k, v)
         self.ext_vars = ext_vars
 
         if grid_layout_comp:
             self.model.add_subsystem('grid_layout_comp', grid_layout_comp, promotes=['*'])
 
-        if cost_comp and isinstance(cost_comp, PostConstraint):
-            post_constraints = post_constraints + [cost_comp]
+        if cost_comp and hasattr(cost_comp, 'post_constraint'):
+            post_constraints = post_constraints + [cost_comp.post_constraint]
 
-        constraints_as_penalty = ((not self.driver.supports['inequality_constraints'] or
-                                   isinstance(self.driver, SimpleGADriver) or
-                                   isinstance(self.driver, EasySimpleGADriver)) and
-                                  len(constraints) + len(post_constraints) > 0)
+        constraints_as_penalty = ((((not self.driver.supports['inequality_constraints'] or
+                                     isinstance(self.driver, SimpleGADriver) or
+                                     isinstance(self.driver, EasySimpleGADriver)) and
+                                    len(constraints) + len(post_constraints) > 0) or
+                                   (penalty_comp is not None)) and not
+                                  isinstance(self.driver, EasySGDDriver))
 
         if len(constraints) > 0:
-            self.model.add_subsystem('pre_constraints', ParallelGroup(), promotes=['*'])
+            self.model.add_subsystem('constraint_group', ParallelGroup(), promotes=['*'])
             for constr in constraints:
                 if constraints_as_penalty:
                     constr.setup_as_penalty(self)
                 else:
                     constr.setup_as_constraint(self)
-            penalty_comp = PenaltyComponent(constraints, constraints_as_penalty)
-            self.model.add_subsystem('penalty_comp', penalty_comp, promotes=['*'])
+            constraint_violation_comp = ConstraintViolationComponent(constraints)
+            self.model.add_subsystem('constraint_violation_comp', constraint_violation_comp, promotes=['*'])
         else:
+            constraint_violation_comp = None
             if isinstance(self.cost_comp, (CostModelComponent, TopFarmGroup)):
-                self.indeps.add_output('penalty', val=0.0)
+                self.indeps.add_output('constraint_violation', val=0.0)
 
         self.model.constraint_components = [constr.constraintComponent for constr in constraints]
 
         for k, v in design_vars.items():
             if isinstance(driver, EasyDriverBase):
                 kwargs = driver.get_desvar_kwargs(self.model, k, v)
             else:
                 kwargs = EasyDriverBase.get_desvar_kwargs(None, self.model, k, v)
             self.model.add_design_var(k, **kwargs)
 
         if cost_comp:
             self.model.add_subsystem('cost_comp', cost_comp, promotes=['*'])
 
         if len(post_constraints) > 0:
-            if constraints_as_penalty:
-                penalty_comp = PostPenaltyComponent(post_constraints, constraints_as_penalty)
-                self.model.add_subsystem('post_penalty_comp', penalty_comp, promotes=['*'])
-            else:
+            if not constraints_as_penalty:
                 for constr in post_constraints:
                     if isinstance(constr, Constraint):
-                        if 'post_constraints' not in self.model._subsystems_allprocs and 'post_constraints' not in self.model._static_subsystems_allprocs:
-                            self.model.add_subsystem('post_constraints', ParallelGroup(), promotes=['*'])
-                        constr.setup_as_constraint(self, group='post_constraints')
+                        if 'constraints_group2' not in self.model._subsystems_allprocs:  # and 'post_constraints' not in self.model._static_subsystems_allprocs:
+                            self.model.add_subsystem('constraints_group2', ParallelGroup(), promotes=['*'])
+                        constr.setup_as_constraint(self, group='constraints_group2')
 
                     elif isinstance(constr[-1], dict):
                         self.model.add_constraint(str(constr[0]), **constr[-1])
-                    elif len(constr) == 2:  # assuming only name and upper value is specified and value is per turbine
-                        if len(constr[1]) == 1:
-                            self.model.add_constraint(constr[0], upper=np.full(self.n_wt, constr[1]))
-                        else:
-                            self.model.add_constraint(constr[0], upper=constr[1])
-                    elif len(constr) == 3:  # four arguments are: key, lower, upper ,shape
-                        lower = None if constr[1] is None else constr[1]
-                        upper = None if constr[2] is None else constr[2]
-                        self.model.add_constraint(
-                            constr[0], lower=lower, upper=upper)
-                    elif len(constr) == 4:  # four arguments are: key, lower, upper ,shape
-                        lower = None if constr[1] is None else np.full(constr[3], constr[1])
-                        upper = None if constr[2] is None else np.full(constr[3], constr[2])
-                        self.model.add_constraint(
-                            constr[0], lower=lower, upper=upper)
-
-        aggr_comp = AggregatedCost(constraints_as_penalty, constraints, post_constraints)
-        self.model.add_subsystem('aggr_comp', aggr_comp, promotes=['*'])
+                    else:
+                        warnings.warn("""constraint tuples should be of type (keyword, {constraint options}).""",
+                                      DeprecationWarning, stacklevel=2)
+        if constraints_as_penalty:
+            if penalty_comp is None:
+                if constraint_violation_comp:
+                    constraints_for_aggregation = post_constraints + [constraint_violation_comp]
+                else:
+                    constraints_for_aggregation = post_constraints
+                objective_comp = ObjectiveComponent(constraints_for_aggregation)
+            else:
+                objective_comp = penalty_comp
+        else:
+            objective_comp = DummyObjectiveComponent()
+        self.model.add_subsystem('objective_comp', objective_comp, promotes=['*'])
         if cost_comp:
             if expected_cost is None:
                 expected_cost = self.evaluate()[0]
                 if self._metadata:
                     self._metadata['setup_status'] = 0
             if isinstance(driver, EasyDriverBase) and driver.supports_expected_cost is False:
                 expected_cost = 1
@@ -301,26 +312,37 @@
             if 'assembled_jac_type' in self.model.cost_comp.options:
                 self.model.cost_comp.options['assembled_jac_type'] = 'dense'
                 self.model.cost_comp.linear_solver.assemble_jac = True
 
         else:
             self.indeps.add_output('cost')
 
-        self.model.add_objective('aggr_cost', scaler=1 / abs(expected_cost))
+        self.model.add_objective('final_cost', scaler=1 / abs(expected_cost))
 
         if plot_comp and not isinstance(plot_comp, NoPlot):
             self.model.add_subsystem('plot_comp', plot_comp, promotes=['*'])
             plot_comp.problem = self
             plot_comp.n_wt = self.n_wt
 
         self.setup()
 
+    # This is needed to avoid an error from interaction between creation of coloring reports and parametrizised pytests in openmdao 3.23-3.26
+    def _update_reports(self, driver):
+        try:
+            from openmdao.utils.reports_system import activate_reports, clear_reports
+            if self._driver is not None:
+                clear_reports(self._driver)
+            driver._set_problem(self)
+            activate_reports(self._reports, driver)
+        except ModuleNotFoundError:
+            pass
+
     @property
     def cost(self):
-        return self['aggr_cost'][0]
+        return self['final_cost'][0]
 
     def __getitem__(self, name):
         return Problem.__getitem__(self, name).copy()
 
     @property
     def state(self):
         """Return current state"""
@@ -423,15 +445,15 @@
 
     def evaluate_gradients(self, disp=False):
         """Evaluate the gradients."""
         self.setup()
         t = time.time()
         rec = TopFarmListRecorder()
         self.driver.add_recorder(rec)
-        res = self.compute_totals(['aggr_cost'], wrt=[topfarm.x_key, topfarm.y_key], return_format='dict')
+        res = self.compute_totals(['final_cost'], wrt=[topfarm.x_key, topfarm.y_key], return_format='dict')
         self.driver._rec_mgr._recorders.remove(rec)
         if disp:
             print("Gradients evaluated in\t%.3fs" % (time.time() - t))
         return res
 
     def optimize(self, state={}, disp=False, recorder_as_list=False):
         """Run the optimization problem
@@ -478,15 +500,15 @@
         self.run_driver()
         self.cleanup()
         if disp:
             print("Optimized in\t%.3fs" % (time.time() - t))
         if self.driver._rec_mgr._recorders != []:  # in openmdao<2.4 cleanup does not delete recorders
             self.driver._rec_mgr._recorders.remove(self.recorder)
         if isinstance(self.driver, DOEDriver) or isinstance(self.driver, SimpleGADriver):
-            costs = self.recorder['aggr_cost']
+            costs = self.recorder['final_cost']
             best_case_index = int(np.argmin(costs))
             best_state = {k: self.recorder[k][best_case_index] for k in self.design_vars}
             self.evaluate(best_state)
         if recorder_as_list:
             return self.cost, copy.deepcopy(self.state), self.recorder.recorder2list()
         else:
             return self.cost, copy.deepcopy(self.state), self.recorder
@@ -500,17 +522,21 @@
         else:
             comp_name_lst = [self.cost_comp.pathname]
         print("checking %s" % ", ".join(comp_name_lst))
         res = self.check_partials(includes=comp_name_lst, compact_print=True)
         for comp in comp_name_lst:
             var_pair = [(x, dx) for x, dx in res[comp].keys()
                         if (x not in ['cost_comp_eval'] and
-                            not x.startswith('penalty') and
-                            not dx.startswith('penalty'))]
-            worst = var_pair[np.argmax([res[comp][k]['rel error'].forward for k in var_pair])]
+                            # not x.startswith('penalty') and
+                            # not dx.startswith('penalty'))]
+                            not (x.startswith('constraint_violation') and
+                                 comp != 'constraint_violation_comp')
+                            )
+                        ]
+            worst = var_pair[np.argmax(np.nan_to_num([res[comp][k]['rel error'].forward for k in var_pair]))]
             err = res[comp][worst]['rel error'].forward
             if err > tol:
                 raise Warning("Mismatch between finite difference derivative of '%s' wrt. '%s' and derivative computed in '%s' is: %f" %
                               (worst[0], worst[1], comp, err))
 
     def as_component(self):
         return ProblemComponent(self)
@@ -570,15 +596,15 @@
 
     def __init__(self, problem, additional_inputs=[]):
         ExplicitComponent.__init__(self)
         self.problem = problem
         self.additional_inputs = additional_inputs
 
     def setup(self):
-        missing_in_problem_exceptions = ['penalty']
+        missing_in_problem_exceptions = ['constraint_violation']
         parent_temp = {}
         parent_temp.update(self.parent.indeps._static_var_rel2meta)
         parent_temp.update(self.parent.indeps._var_rel2meta)
         problem_temp = {}
         problem_temp.update(self.problem.indeps._static_var_rel2meta)
         problem_temp.update(self.problem.indeps._var_rel2meta)
         missing_in_problem = (set(parent_temp) -
```

### Comparing `topfarm-2.3.2/topfarm/constraint_components/_constraint.py` & `topfarm-2.3.4/topfarm/constraint_components/_constraint.py`

 * *Files identical despite different names*

### Comparing `topfarm-2.3.2/topfarm/constraint_components/boundary.py` & `topfarm-2.3.4/topfarm/constraint_components/boundary.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from scipy.spatial import ConvexHull
 from topfarm.constraint_components import Constraint, ConstraintComponent
 from topfarm.utils import smooth_max, smooth_max_gradient
 import topfarm
 from shapely.geometry import Polygon, MultiPolygon, LineString
 from shapely.ops import unary_union
 import warnings
+from tqdm import tqdm
 
 
 class XYBoundaryConstraint(Constraint):
     def __init__(self, boundary, boundary_type='convex_hull', units=None, relaxation=False, **kwargs):
         """Initialize XYBoundaryConstraint
 
         Parameters
@@ -37,15 +38,15 @@
             self.zones = boundary
             assert 'turbines' in list(kwargs)
             self.turbines = kwargs['turbines']
             self.boundary = np.asarray(self.zones[0].boundary)
         else:
             self.boundary = np.asarray(boundary)
         self.boundary_type = boundary_type
-        self.const_id = 'xyboundary_comp_{}_{}'.format(boundary_type, int(self.boundary.sum()))
+        self.const_id = 'xyboundary_comp_{}'.format(boundary_type)
         self.units = units
         self.relaxation = relaxation
 
     def get_comp(self, n_wt):
         if not hasattr(self, 'boundary_comp'):
             if self.boundary_type == 'polygon':
                 self.boundary_comp = PolygonBoundaryComp(
@@ -73,28 +74,32 @@
             if k in design_vars:
                 if len(design_vars[k]) == 4:
                     design_vars[k] = (design_vars[k][0], np.maximum(design_vars[k][1], l),
                                       np.minimum(design_vars[k][2], u), design_vars[k][-1])
                 else:
                     design_vars[k] = (design_vars[k][0], l, u, design_vars[k][-1])
 
-    def _setup(self, problem, group='pre_constraints'):
+    def _setup(self, problem, group='constraint_group'):
         n_wt = problem.n_wt
         self.boundary_comp = self.get_comp(n_wt)
         self.boundary_comp.problem = problem
         self.set_design_var_limits(problem.design_vars)
         # problem.xy_boundary = np.r_[self.boundary_comp.xy_boundary, self.boundary_comp.xy_boundary[:1]]
         problem.indeps.add_output('xy_boundary', self.boundary_comp.xy_boundary)
         getattr(problem.model, group).add_subsystem('xy_bound_comp', self.boundary_comp, promotes=['*'])
 
-    def setup_as_constraint(self, problem, group='pre_constraints'):
+    def setup_as_constraint(self, problem, group='constraint_group'):
         self._setup(problem, group=group)
-        problem.model.add_constraint('boundaryDistances', lower=self.boundary_comp.zeros)
+        if problem.n_wt == 1:
+            lower = 0
+        else:
+            lower = self.boundary_comp.zeros
+        problem.model.add_constraint('boundaryDistances', lower=lower)
 
-    def setup_as_penalty(self, problem, group='pre_constraints'):
+    def setup_as_penalty(self, problem, group='constraint_group'):
         self._setup(problem, group=group)
 
 
 class CircleBoundaryConstraint(XYBoundaryConstraint):
     def __init__(self, center, radius):
         """Initialize CircleBoundaryConstraint
 
@@ -144,15 +149,15 @@
                        desc='x coordinates of turbines in global ref. frame', units=self.units)
         self.add_input(topfarm.y_key, np.zeros(self.n_wt),
                        desc='y coordinates of turbines in global ref. frame', units=self.units)
         if self.relaxation:
             self.add_input('time', 0)
         if hasattr(self, 'types'):
             self.add_input('type', np.zeros(self.n_wt))
-        self.add_output('penalty_' + self.const_id, val=0.0)
+        # self.add_output('constraint_violation_' + self.const_id, val=0.0)
         # Explicitly size output array
         # (vector with positive elements if turbines outside of hull)
         self.add_output('boundaryDistances', self.zeros,
                         desc="signed perpendicular distances from each turbine to each face CCW; + is inside")
         self.declare_partials('boundaryDistances', [topfarm.x_key, topfarm.y_key])
         if self.relaxation:
             self.declare_partials('boundaryDistances', 'time')
@@ -160,15 +165,15 @@
         # self.declare_partials('boundaryDistances', ['boundaryVertices', 'boundaryNormals'], method='fd')
 
     def compute(self, inputs, outputs):
         # calculate distances from each point to each face
         args = {x: inputs[x] for x in [topfarm.x_key, topfarm.y_key, topfarm.type_key] if x in inputs}
         boundaryDistances = self.distances(**args)
         outputs['boundaryDistances'] = boundaryDistances
-        outputs['penalty_' + self.const_id] = np.sum(np.minimum(boundaryDistances, 0) ** 2)
+        # outputs['constraint_violation_' + self.const_id] = np.sum(np.minimum(boundaryDistances, 0) ** 2)
 
     def compute_partials(self, inputs, partials):
         # return Jacobian dict
         if not self.relaxation:
             dx, dy = self.gradients(**{xy: inputs[k] for xy, k in zip('xy', [topfarm.x_key, topfarm.y_key])})
         else:
             dx, dy, dt = self.gradients(**{xy: inputs[k] for xy, k in zip('xy', [topfarm.x_key, topfarm.y_key])})
@@ -466,15 +471,17 @@
         ddist_dxy[:, use_A] = sign_use_A * (AP[:, use_A] / vec_len(AP[:, use_A]))
         ddist_dxy[:, use_B] = sign_use_B * (BP[:, use_B] / vec_len(BP[:, use_B]))
         ddist_dX, ddist_dY = ddist_dxy
 
         return distance, ddist_dX, ddist_dY
 
     def calc_distance_and_gradients(self, x, y):
-        if np.all(np.array([x, y]) == self._cache_input):
+        if not np.shape([x, y]) == np.shape(self._cache_input):
+            pass
+        elif np.all(np.array([x, y]) == self._cache_input):
             return self._cache_output
         distance, ddist_dX, ddist_dY = self._calc_distance_and_gradients(x, y)
         closest_edge_index = np.argmin(np.abs(distance), 1)
         self._cache_input = np.array([x, y])
         self._cache_output = [np.choose(closest_edge_index, v.T) for v in [distance, ddist_dX, ddist_dY]]
         return self._cache_output
 
@@ -570,26 +577,29 @@
 
         '''
         self.zones = zones
         self.bounds_poly, xy_boundaries = self.get_xy_boundaries()
         PolygonBoundaryComp.__init__(self, n_wt, xy_boundary=xy_boundaries[0], const_id=const_id, units=units, relaxation=relaxation)
         # self.bounds_poly = [Polygon(x) for x in xy_boundaries]
         self.incl_excls = [x.incl for x in zones]
-        self._setup_boundaries()
+        self._setup_boundaries(self.bounds_poly, self.incl_excls)
         self.relaxation = relaxation
         self.method = method
         if simplify_geometry:
             self.simplify(simplify_geometry)
 
     def simplify(self, simplify_geometry):
+        bounds = [bi[0] for bi in self.boundaries]
+        self.incl_excls = [bi[1] for bi in self.boundaries]
+        polygons = [Polygon(b) for b in bounds]
         if isinstance(simplify_geometry, dict):
-            self.bounds_poly = [rp.simplify(**simplify_geometry) for rp in self.bounds_poly]
+            self.bounds_poly = [rp.simplify(**simplify_geometry) for rp in polygons]
         else:
-            self.bounds_poly = [rp.simplify(simplify_geometry) for rp in self.bounds_poly]
-        self._setup_boundaries()
+            self.bounds_poly = [rp.simplify(simplify_geometry) for rp in polygons]
+        self._setup_boundaries(self.bounds_poly, self.incl_excls)
 
     # def line_to_xy_boundary(self, line, buffer):
     #     return np.asarray(Polygon(LineString(line).buffer(buffer, join_style=2).exterior).exterior.coords)
 
     def get_xy_boundaries(self):
         polygons = []
         bounds = []
@@ -602,16 +612,16 @@
                 poly = Polygon(LineString(z.boundary).buffer(buffer, join_style=2).exterior)
             elif z.geometry_type == 'polygon':
                 poly = Polygon(z.boundary).buffer(buffer, join_style=2)
             polygons.append(poly)
             bounds.append(np.asarray(poly.exterior.coords))
         return polygons, bounds
 
-    def _setup_boundaries(self):
-        self.res_poly = self._calc_resulting_polygons(self.bounds_poly)
+    def _setup_boundaries(self, bounds_poly, incl_excl):
+        self.res_poly = self._calc_resulting_polygons(bounds_poly, incl_excl)
         self.boundaries = self._poly_to_bound(self.res_poly)
 
         boundary_properties_list_all = list(zip(*[self.get_boundary_properties(bound, incl_excl)[1:]
                                                   for bound, incl_excl in self.boundaries]))
 
         self.boundary_properties_list_all = [np.concatenate(v, -1)
                                              for v in boundary_properties_list_all]
@@ -622,35 +632,35 @@
             x, y = bound.exterior.xy
             boundaries.append((np.asarray([x, y]).T[:-1, :], 1))
             for interior in bound.interiors:
                 x, y = interior.xy
                 boundaries.append((np.asarray([x, y]).T[:-1, :], 0))
         return boundaries
 
-    def _calc_resulting_polygons(self, boundary_polygons):
+    def _calc_resulting_polygons(self, boundary_polygons, incl_excls):
         '''
         Parameters
         ----------
         boundary_polygons : list
             list of shapely polygons as specifed or inferred from user input
         Returns
         -------
         list of merged shapely polygons. Resolves issues arrising if any are overlapping, touching or contained in each other
         '''
         domain = []
-        for i in range(len(boundary_polygons)):
+        for i in tqdm(range(len(boundary_polygons))):
             b = boundary_polygons[i]
             if len(domain) == 0:
-                if self.incl_excls[i]:
+                if incl_excls[i]:
                     domain.append(b)
                 else:
                     warnings.warn("First boundary should be an inclusion zone or it will be ignored")
                     pass
             else:
-                if self.incl_excls[i]:
+                if incl_excls[i]:
                     temp = []
                     for j, d in enumerate(domain):
                         if d.intersects(b):
                             b = unary_union([d, b])
                         else:
                             if d.contains(b):
                                 warnings.warn("Boundary is fully contained preceding polygon and will be ignored")
@@ -707,15 +717,17 @@
             Array of point-edge distances. index 'i' is points and index 'j' is total number of edges.
         sign_i : 1d array
             Array of signs of the governing distance.
         dDdk_jk : 2d array
             Jacobian of the distance matrix D_ij with respect to x and y.
 
         '''
-        if np.all(np.array([x, y]) == self._cache_input) & (not self.relaxation):
+        if not np.shape([x, y]) == np.shape(self._cache_input):
+            pass
+        elif np.all(np.array([x, y]) == self._cache_input) & (not self.relaxation):
             return self._cache_output
 
         Dist_ij, ddist_dX, ddist_dY = self._calc_distance_and_gradients(x, y, self.boundary_properties_list_all)
 
         dDdk_ijk = np.moveaxis([ddist_dX, ddist_dY], 0, -1)
         sign_i = self.sign(Dist_ij)
         self._cache_input = np.array([x, y])
@@ -774,15 +786,15 @@
         for i, p in enumerate(poly):
             if booleans[i] == 0:
                 pb = p.buffer(-self.calc_relaxation(iteration_no), join_style=2)
                 relaxed_poly.append(pb)
             else:
                 pb = p.buffer(self.calc_relaxation(iteration_no), join_style=2)
                 relaxed_poly.append(pb)
-        merged_poly = self._calc_resulting_polygons(relaxed_poly)
+        merged_poly = self._calc_resulting_polygons(relaxed_poly, booleans)
         return self._poly_to_bound(merged_poly)
 
 
 class TurbineSpecificBoundaryComp(MultiPolygonBoundaryComp):
     def __init__(self, n_wt, wind_turbines, zones, const_id=None,
                  units=None, relaxation=False, method='nearest', simplify_geometry=False):
         # self.dependencies = [d or {'type': None, 'multiplier': None, 'ref': None} for d in dependencies]
@@ -858,15 +870,15 @@
     #             ts_polygon_boundary = bound.buffer(dep['multiplier']*h-ref, join_style=2)
     #         else:
     #             ts_polygon_boundary = bound
     #         temp.append(ts_polygon_boundary)
     #     return temp
 
     def merge_boundaries(self):
-        return [self._calc_resulting_polygons(bounds) for bounds in self.ts_polygon_boundaries]
+        return [self._calc_resulting_polygons(bounds, self.incl_excls) for bounds in self.ts_polygon_boundaries]
 
     def get_ts_boundary_properties(self,):
         return [[self.get_boundary_properties(bound) for bound, _ in bounds] for bounds in self.ts_merged_xy_boundaries]
 
     def get_ts_item_indices(self):
         temp = []
         for bounds in self.ts_merged_xy_boundaries:
@@ -875,18 +887,21 @@
             start_at = np.cumsum(n_edges) - n_edges
             end_at = start_at + n_edges
             item_indices = [n_edges_tot, start_at, end_at]
             temp.append(item_indices)
         return temp
 
     def calc_distance_and_gradients(self, x, y, types=None):
-        if not isinstance(self._cache_input, type(None)):
-            if np.all(np.array([x, y]) == self._cache_input[0]) & (not self.relaxation) & np.all(np.asarray([types]) == self._cache_input[1]):
-                return self._cache_output
-        if isinstance(types, type(None)):
+        if self._cache_input is None:
+            pass
+        elif not np.shape([x, y]) == np.shape(self._cache_input[0]) or not np.shape(types) == np.shape(self._cache_input[1]):
+            pass
+        elif np.all(np.array([x, y]) == self._cache_input[0]) & (not self.relaxation) & np.all(np.asarray([types]) == self._cache_input[1]):
+            return self._cache_output
+        if types is None:
             types = np.zeros(self.n_wt)
         Dist_i = np.zeros(self.n_wt)
         sign_i = np.zeros(self.n_wt)
         dDdx_i = np.zeros(self.n_wt)
         dDdy_i = np.zeros(self.n_wt)
         for t in set(types):
             t = int(t)
```

### Comparing `topfarm-2.3.2/topfarm/constraint_components/boundary_component.py` & `topfarm-2.3.4/topfarm/constraint_components/boundary_component.py`

 * *Files identical despite different names*

### Comparing `topfarm-2.3.2/topfarm/constraint_components/capacity.py` & `topfarm-2.3.4/topfarm/constraint_components/capacity.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,16 +21,16 @@
     @property
     def constraintComponent(self):
         return self.capacity_comp
 
     def _setup(self, problem):
         self.n_wt = problem.n_wt
         self.capacity_comp = CapacityComp(self.n_wt, self.max_capacity, self.rated_power_array, self.const_id)
-        problem.model.pre_constraints.add_subsystem(self.const_id, self.capacity_comp, promotes=[
-            topfarm.type_key, 'penalty_' + self.const_id, 'totalcapacity'])
+        problem.model.constraint_group.add_subsystem(self.const_id, self.capacity_comp, promotes=[
+            '*'])
 
     def setup_as_constraint(self, problem):
         self._setup(problem)
         problem.model.add_constraint('totalcapacity', upper=self.max_capacity)
 
     def setup_as_penalty(self, problem):
         self._setup(problem)
@@ -46,19 +46,19 @@
         self.n_wt = n_wt
         self.max_capacity = max_capacity
         self.rated_power_array = np.array(rated_power_array)
         self.const_id = const_id
 
     def setup(self):
         self.add_input(topfarm.type_key, np.zeros(self.n_wt, dtype=int))
-        self.add_output('penalty_' + self.const_id, val=0.0)
+        # self.add_output('constraint_violation_' + self.const_id, val=0.0)
         self.add_output('totalcapacity', val=0.0,
                         desc='wind farm installed capacity')
         # Partial declaration is not needed for type or penalty in this case.
         # Because it is only used for integer optimization.
 
     def compute(self, inputs, outputs):
         outputs['totalcapacity'] = np.sum(self.rated_power_array[inputs[topfarm.type_key].astype(int)])
-        outputs['penalty_' + self.const_id] = np.maximum(0, outputs['totalcapacity'][0] - self.max_capacity)
+        # outputs['constraint_violation_' + self.const_id] = np.maximum(0, outputs['totalcapacity'][0] - self.max_capacity)
 
     def satisfy(self):
         pass
```

### Comparing `topfarm-2.3.2/topfarm/constraint_components/constrained_generator.py` & `topfarm-2.3.4/topfarm/constraint_components/constrained_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     def __init__(self, generator):
         DOEGenerator.__init__(self)
         if isinstance(generator, list):
             generator = ListGenerator(generator)
         self.generator = generator
 
     def __call__(self, design_vars, model=None):
-        constr = model._get_subsystem('pre_constraints')
+        constr = model._get_subsystem('constraint_group')
         xy_boundary_comp = constr._get_subsystem('xy_bound_comp')
         spacing_comp = constr._get_subsystem('spacing_comp')
         for xyz_tuple_lst in self.generator(design_vars, model=model):
             x, y = ([np.array(t[1]) for t in xyz_tuple_lst] + [0])[:2]
             if spacing_comp:
                 dist = spacing_comp._compute(x, y)
                 if np.any(dist < spacing_comp.min_spacing**2):
```

### Comparing `topfarm-2.3.2/topfarm/constraint_components/constraint_aggregation.py` & `topfarm-2.3.4/topfarm/constraint_components/constraint_aggregation.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 Created on Thu Oct  6 13:55:21 2022
 
 @author: mikf
 """
 import numpy as np
 from topfarm.constraint_components import Constraint, ConstraintComponent
 from topfarm.cost_models.cost_model_wrappers import CostModelComponent
+from topfarm.constraint_components.spacing import SpacingConstraint
+from topfarm.constraint_components.boundary import XYBoundaryConstraint
 
 
 class ConstraintAggregation(Constraint):
     def __init__(self, constraints, **kwargs):
         self.constraints = constraints
         self.const_id = 'constraint_aggregation_comp'
         self.kwargs = kwargs
@@ -18,35 +20,40 @@
         self.output_keys = list([(i, i[0])[isinstance(i, tuple)] for i in kwargs['component_args']['output_keys']])
 
     @property
     def constraintComponent(self):
         return self.constraint_aggregation_comp
 
     def _setup(self, problem):
-        self.constraint_aggregation_comp = ConstraintAggregationComp(**self.kwargs['component_args'])
+        self.constraint_aggregation_comp = ConstraintAggregationComp(self.constraints, **self.kwargs['component_args'])
         for constraint in self.constraints:
             constraint._setup(problem)
         problem.model.add_subsystem(self.const_id, self.constraint_aggregation_comp,
                                     promotes=['*'])
 
     def setup_as_constraint(self, problem):
         self._setup(problem)
         problem.model.add_constraint(**self.kwargs['constraint_args'])
 
     def setup_as_penalty(self, problem):
         self._setup(problem)
 
 
 class ConstraintAggregationComp(CostModelComponent, ConstraintComponent):
-    def __init__(self, **kwargs):
+    def __init__(self, constraints, **kwargs):
+        self.constraints = constraints
         CostModelComponent.__init__(self, **kwargs)
 
     def satisfy(self, state):
         pass
 
+    def plot(self, ax):
+        for constraint in self.constraints:
+            constraint.constraintComponent.plot(ax)
+
 
 class DistanceConstraintAggregation(ConstraintAggregation):
     """Aggregating the spacing and boundary distances constraints into a penalty function"""
 
     def __init__(self, constraints, n_wt, min_spacing_m, windTurbines, name='sgd_constraint', **kwargs):
         """Initializing spacing constraint aggregation class
 
@@ -73,18 +80,28 @@
             separation_constraint = wtSeparationSquared - (2 * windTurbines.diameter()) ** 2
             J_separation = np.zeros_like(wtSeparationSquared)
             J_separation[np.where(separation_constraint < 0)] = -1
             J_distance = np.zeros_like(boundaryDistances)
             J_distance[np.where(boundaryDistances < 0)] = 2 * boundaryDistances[np.where(boundaryDistances < 0)]
             return [[J_separation], [J_distance]]
 
-        kwargs['component_args'] = {'input_keys': [('wtSeparationSquared', np.zeros(int(n_wt * (n_wt - 1) / 2))),
-                                                   ('boundaryDistances', np.zeros((n_wt, 4)))],
+        input_keys = []
+        for cons in constraints:
+            if isinstance(cons, XYBoundaryConstraint):
+                comp = cons.get_comp(n_wt)
+                zeros = comp.zeros
+                input_keys.append(('boundaryDistances', zeros))
+            elif isinstance(cons, SpacingConstraint):
+                zeros = np.zeros(int(n_wt * (n_wt - 1) / 2))
+                input_keys.append(('wtSeparationSquared', zeros))
+
+        kwargs['component_args'] = {'input_keys': input_keys,
                                     'n_wt': n_wt,
                                     'cost_function': constr_aggr_func,
                                     'cost_gradient_function': constr_aggr_grad,
                                     'objective': False,
                                     'output_keys': [(name, 0)],
-                                    'use_penalty': False}
+                                    'use_constraint_violation': False
+                                    }
         kwargs['constraint_args'] = {'name': name, 'lower': 0}
 
         ConstraintAggregation.__init__(self, constraints, **kwargs)
```

### Comparing `topfarm-2.3.2/topfarm/constraint_components/load.py` & `topfarm-2.3.4/topfarm/constraint_components/load.py`

 * *Files identical despite different names*

### Comparing `topfarm-2.3.2/topfarm/constraint_components/spacing.py` & `topfarm-2.3.4/topfarm/constraint_components/spacing.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,16 @@
         return self.spacing_comp
 
     def _setup(self, problem):
         self.n_wt = problem.n_wt
         self.spacing_comp = SpacingComp(self.n_wt, self.min_spacing, self.const_id, self.units,
                                         aggregation_function=self.aggregation_function,
                                         full_aggregation=self.full_aggregation)
-        problem.model.pre_constraints.add_subsystem(self.const_id, self.spacing_comp,
-                                                    promotes=[topfarm.x_key, topfarm.y_key, 'penalty_' + self.const_id, 'wtSeparationSquared'])
+        problem.model.constraint_group.add_subsystem(self.const_id, self.spacing_comp,
+                                                     promotes=[topfarm.x_key, topfarm.y_key, 'wtSeparationSquared'])
 
     def setup_as_constraint(self, problem):
         self._setup(problem)
         problem.model.add_constraint('wtSeparationSquared', lower=self.min_spacing**2)
 
     def setup_as_penalty(self, problem):
         self._setup(problem)
@@ -67,15 +67,15 @@
 
     def setup(self):
         # Explicitly size input arrays
         self.add_input(topfarm.x_key, val=np.zeros(self.n_wt),
                        desc='x coordinates of turbines in wind dir. ref. frame', units=self.units)
         self.add_input(topfarm.y_key, val=np.zeros(self.n_wt),
                        desc='y coordinates of turbines in wind dir. ref. frame', units=self.units)
-        self.add_output('penalty_' + self.const_id, val=0.0)
+        # self.add_output('constraint_violation_' + self.const_id, val=0.0)
         # Explicitly size output array
         self.add_output(self.constraint_key, val=np.zeros(self.veclen),
                         desc='spacing of all turbines in the wind farm')
 
         col_pairs = np.array([(i, j) for i in range(self.n_wt - 1) for j in range(i + 1, self.n_wt)])
         if self.aggregation_function:
             self.declare_partials(self.constraint_key, [topfarm.x_key, topfarm.y_key])
@@ -102,15 +102,15 @@
                 outputs[self.constraint_key] = self.aggregation_function(separation_squared)
             else:
                 outputs[self.constraint_key] = self.aggregation_function(
                     separation_squared[self.partial_indices], 0)
                 # print(outputs[self.constraint_key])
         else:
             outputs[self.constraint_key] = separation_squared
-        outputs['penalty_' + self.const_id] = -np.minimum(separation_squared - self.min_spacing**2, 0).sum()
+        # outputs['constraint_violation_' + self.const_id] = -np.minimum(separation_squared - self.min_spacing**2, 0).sum()
 
     def _compute(self, x, y):
         n_wt = self.n_wt
 
         # compute distance matrixes
         dX, dY = [np.subtract(*np.meshgrid(xy, xy, indexing='ij')).T
                   for xy in [x, y]]
@@ -187,15 +187,15 @@
     def plot(self, ax=None):
         from matplotlib.pyplot import Circle
         import matplotlib.pyplot as plt
         ax = ax or plt.gca()
 
         def get_xy(xy):
             if not hasattr(self, xy):
-                setattr(self, xy, dict(self.list_inputs(out_stream=None))[f'pre_constraints.{self.name}.{xy}']['value'])
+                setattr(self, xy, dict(self.list_inputs(out_stream=None))[f'constraint_group.{self.name}.{xy}']['value'])
             xy = getattr(self, xy)
             return xy if not isinstance(xy, tuple) else xy[0]
 
         for x, y in zip(get_xy('x'), get_xy('y')):
             circle = Circle((x, y), self.min_spacing / 2, color='k', ls='--', fill=False)
             ax.add_artist(circle)
 
@@ -236,17 +236,16 @@
         self.min_spacing = np.asarray(min_spacing)
 
     def _setup(self, problem):
         self.n_wt = problem.n_wt
         self.spacing_comp = SpacingTypeComp(self.n_wt, self.min_spacing, self.const_id, self.units,
                                             aggregation_function=self.aggregation_function,
                                             full_aggregation=self.full_aggregation)
-        problem.model.pre_constraints.add_subsystem(self.const_id, self.spacing_comp,
-                                                    promotes=[topfarm.x_key, topfarm.y_key, topfarm.type_key,
-                                                              'penalty_' + self.const_id, 'wtRelativeSeparationSquared'])
+        problem.model.constraint_group.add_subsystem(self.const_id, self.spacing_comp,
+                                                     promotes=[topfarm.x_key, topfarm.y_key, topfarm.type_key, 'wtRelativeSeparationSquared'])
 
     def setup_as_constraint(self, problem):
         self._setup(problem)
         problem.model.add_constraint('wtRelativeSeparationSquared', lower=0)
 
 
 class SpacingTypeComp(SpacingComp):
@@ -276,15 +275,15 @@
                 outputs[self.constraint_key] = self.aggregation_function(relative_separation_squared)
             else:
                 outputs[self.constraint_key] = self.aggregation_function(
                     relative_separation_squared[self.partial_indices], 0)
                 # print(outputs[self.constraint_key])
         else:
             outputs[self.constraint_key] = relative_separation_squared
-        outputs['penalty_' + self.const_id] = -np.minimum(relative_separation_squared, 0).sum()
+        # outputs['constraint_violation_' + self.const_id] = -np.minimum(relative_separation_squared, 0).sum()
 
     def get_min_eff_spacing(self, t):
         return (self.min_spacing[np.atleast_1d(t).astype(int)][:, na] + self.min_spacing[np.atleast_1d(t).astype(int)][na, :]) / 2
 
     def _compute(self, x, y, t):
         n_wt = self.n_wt
         # compute distance matrixes
@@ -297,15 +296,15 @@
     def plot(self, ax=None):
         from matplotlib.pyplot import Circle
         import matplotlib.pyplot as plt
         ax = ax or plt.gca()
 
         def get_xy(xy):
             if not hasattr(self, xy):
-                setattr(self, xy, dict(self.list_inputs(out_stream=None))[f'pre_constraints.{self.name}.{xy}']['value'])
+                setattr(self, xy, dict(self.list_inputs(out_stream=None))[f'constraint_group.{self.name}.{xy}']['value'])
             xy = getattr(self, xy)
             return xy if not isinstance(xy, tuple) else xy[0]
 
         for x, y, t in zip(get_xy('x'), get_xy('y'), get_xy('type')):
             circle = Circle((x, y), self.get_min_eff_spacing(t).ravel() / 2, color='k', ls='--', fill=False)
             ax.add_artist(circle)
```

### Comparing `topfarm-2.3.2/topfarm/cost_models/cost_model_wrappers.py` & `topfarm-2.3.4/topfarm/cost_models/cost_model_wrappers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from openmdao.core.explicitcomponent import ExplicitComponent
 import numpy as np
 import time
 from _collections import defaultdict
-from topfarm.constraint_components.post_constraint import PostConstraint
+# from topfarm.constraint_components.post_constraint import PostConstraint
 import warnings
 
 
 class CostModelComponent(ExplicitComponent):
     """Wrapper for pure-Python cost functions"""
 
     def __init__(self, input_keys, n_wt, cost_function, cost_gradient_function=None,
                  output_keys=["Cost"], output_unit="", additional_input=[], additional_output=[], max_eval=None,
-                 objective=True, maximize=False, output_vals=[0.0], input_units=[], step={}, use_penalty=True, **kwargs):
+                 objective=True, maximize=False, output_vals=[0.0], input_units=[], step={}, use_constraint_violation=True, **kwargs):
         """Initialize wrapper for pure-Python cost function
 
         Parameters
         ----------
         input_keys : list of str
             Inputs to the cost function
         n_wt : int
@@ -100,24 +100,24 @@
         self.input_units = (input_units + [None] * n_input)[:n_input]
 
         self.n_func_eval = 0
         self.func_time_sum = 0
         self.n_grad_eval = 0
         self.grad_time_sum = 0
         self.step = step
-        self.use_penalty = use_penalty
+        self.use_constraint_violation = use_constraint_violation
 
     def setup(self):
         for i, u in zip(self.input_keys + self.additional_input, self.input_units):
             if isinstance(i, tuple) and len(i) == 2:
                 self.add_input(i[0], val=i[1], units=u)
             else:
                 self.add_input(i, val=np.zeros(self.n_wt), units=u)
-        if self.use_penalty:
-            self.add_input('penalty', val=0.0)
+        if self.use_constraint_violation:
+            self.add_input('constraint_violation', val=0.0)
         if self.objective:
             self.add_output('cost', val=0.0)
             self.add_output('cost_comp_eval', val=0.0)
         for o, v in zip(self.output_keys, self.output_vals):
             if isinstance(o, tuple) and len(o) == 2:
                 self.add_output(o[0], val=o[1])
             else:
@@ -152,16 +152,16 @@
             counter += self.n_grad_eval * max(ratio, 1)
         else:
             counter += self.n_grad_eval
         return int(counter)
 
     def compute(self, inputs, outputs):
         """Compute cost model"""
-        if self.use_penalty:
-            if inputs['penalty'] > 0:
+        if self.use_constraint_violation:
+            if (inputs['constraint_violation'] > 1e5) and (self.n_func_eval > 0):
                 return
         if self.counter >= self.max_eval:
             return
         t = time.time()
         if self.additional_output:
             c, additional_output = self.cost_function(**{x: inputs[x] for x in self.all_input_keys})
             for k, v in additional_output.items():
@@ -237,15 +237,15 @@
                                     cost_gradient_function=cost_gradient_function,
                                     output_key=output_key, output_unit=output_unit,
                                     additional_input=additional_input,
                                     additional_output=additional_output,
                                     max_eval=max_eval, maximize=True, **kwargs)
 
 
-class AEPMaxLoadCostModelComponent(CostModelComponent, PostConstraint):
+class AEPMaxLoadCostModelComponent(CostModelComponent):
     """Wrapper for pure-Python cost functions"""
     def __init__(self, input_keys, n_wt, aep_load_function, max_loads,
                  aep_load_gradient=None, output_keys=["AEP", 'loads'], step={},
                  maximize=True, **kwargs):
         """Initialize Sub class of the CostModelComponent for AEP maximization and load constraints
 
         Parameters
@@ -281,13 +281,14 @@
             gradient_function = None
 
         # additional_output = kwargs.get('additional_output', []) + [('loads', max_loads)]
         CostModelComponent.__init__(self, input_keys, n_wt, cost_function=cost_function,
                                     cost_gradient_function=gradient_function,
                                     output_keys=output_keys, step=step, maximize=maximize,
                                     **kwargs)
-        PostConstraint.__init__(self, 'loads', upper=max_loads)
+        self.post_constraint = ('loads', {'upper': max_loads})
+        # PostConstraint.__init__(self, 'loads', upper=max_loads)
 
     # def setup(self):
     #     AEPCostModelComponent.setup(self)
     #     input_keys = list([(i, i[0])[isinstance(i, tuple)] for i in self.input_keys])
         # self.declare_partials('loads', input_keys, method='fd')
```

### Comparing `topfarm-2.3.2/topfarm/cost_models/dummy.py` & `topfarm-2.3.4/topfarm/cost_models/dummy.py`

 * *Files identical despite different names*

### Comparing `topfarm-2.3.2/topfarm/cost_models/economic_models/dtu_wind_cm_main.py` & `topfarm-2.3.4/topfarm/cost_models/economic_models/dtu_wind_cm_main.py`

 * *Files identical despite different names*

### Comparing `topfarm-2.3.2/topfarm/cost_models/economic_models/turbine_cost.py` & `topfarm-2.3.4/topfarm/cost_models/economic_models/turbine_cost.py`

 * *Files identical despite different names*

### Comparing `topfarm-2.3.2/topfarm/cost_models/electrical/simple_msp.py` & `topfarm-2.3.4/topfarm/cost_models/electrical/simple_msp.py`

 * *Files identical despite different names*

### Comparing `topfarm-2.3.2/topfarm/cost_models/fuga/py_fuga.py` & `topfarm-2.3.4/topfarm/cost_models/fuga/py_fuga.py`

 * *Files identical despite different names*

### Comparing `topfarm-2.3.2/topfarm/cost_models/py_wake_wrapper.py` & `topfarm-2.3.4/topfarm/cost_models/py_wake_wrapper.py`

 * *Files 26% similar despite different names*

```diff
@@ -129,14 +129,84 @@
                 sim_res = self.windFarmModel(wt_x, wt_y, type=t, wd=wd, ws=ws, n_cpu=self.n_cpu)
                 H = np.full(X.shape, self.windFarmModel.windTurbines.hub_height())
                 next_type = type_[min(len(type_) - 1, len(wt_x) + 1)]
             return sim_res.aep_map(Points(X, Y, H), type=next_type, n_cpu=self.n_cpu).values
         return aep4smart_start
 
 
+class PyWakeAEPCostModelComponentAdditionalTurbines(PyWakeAEPCostModelComponent):
+    '''PyWake AEP component that allows for including additional turbine positions that are not
+    considered design variables but still considered for wake effect. Note that this functionality
+    can be limited by your wind farm models ability to predict long distance wakes.'''
+    def __init__(self, windFarmModel, n_wt, add_wt_x, add_wt_y, add_wt_type=0, add_wt_h=None, wd=None, ws=None, max_eval=None, grad_method=autograd, n_cpu=1, **kwargs):
+        self.x2, self.y2 = add_wt_x, add_wt_y
+        self.windFarmModel = windFarmModel
+        self.n_cpu = n_cpu
+
+        def aep(**kwargs):
+            x = np.concatenate([kwargs[topfarm.x_key], self.x2])
+            y = np.concatenate([kwargs[topfarm.y_key], self.y2])
+            if add_wt_h is not None:
+                h_primary = np.full_like(kwargs[topfarm.x_key], kwargs.get(topfarm.z_key, None))
+                h_secondary = np.full_like(add_wt_x)
+                h = np.concatenate((h_primary, h_secondary))
+            else:
+                h = None
+            type_primary = np.ones_like(kwargs[topfarm.x_key]) * kwargs.get(topfarm.type_key, 0)
+            type_secondary = np.ones_like(add_wt_x) * add_wt_type
+            type = np.concatenate([type_primary, type_secondary])
+            try:
+                return self.windFarmModel(x=x,
+                                          y=y,
+                                          h=h,
+                                          type=type,
+                                          wd=wd, ws=ws,
+                                          n_cpu=n_cpu).aep().sum(['wd', 'ws']).values[:n_wt].sum()
+            except ValueError as e:
+                if 'are at the same position' in str(e):
+                    return 0
+
+        if grad_method:
+            if hasattr(self.windFarmModel, 'dAEPdxy'):
+                # for backward compatibility
+                dAEPdxy = self.windFarmModel.dAEPdxy(grad_method)
+            else:
+                def dAEPdxy(**kwargs):
+                    return self.windFarmModel.aep_gradients(
+                        gradient_method=grad_method, wrt_arg=['x', 'y'], n_cpu=n_cpu, **kwargs)
+
+            def daep(**kwargs):
+                x = np.concatenate([kwargs[topfarm.x_key], self.x2])
+                y = np.concatenate([kwargs[topfarm.y_key], self.y2])
+                if add_wt_h is not None:
+                    h_primary = np.full_like(kwargs[topfarm.x_key], kwargs.get(topfarm.z_key, None))
+                    h_secondary = np.full_like(add_wt_x)
+                    h = np.concatenate((h_primary, h_secondary))
+                else:
+                    h = None
+                type_primary = np.ones_like(kwargs[topfarm.x_key]) * kwargs.get(topfarm.type_key, 0)
+                type_secondary = np.ones_like(add_wt_x) * add_wt_type
+                type = np.concatenate([type_primary, type_secondary])
+                grad = dAEPdxy(x=x,
+                               y=y,
+                               h=h,
+                               type=type,
+                               wd=wd, ws=ws)[:, :n_wt]
+                return grad
+        else:
+            daep = None
+        AEPCostModelComponent.__init__(self,
+                                       input_keys=[topfarm.x_key, topfarm.y_key],
+                                       n_wt=n_wt,
+                                       cost_function=aep,
+                                       cost_gradient_function=daep,
+                                       output_unit='GWh',
+                                       max_eval=max_eval, **kwargs)
+
+
 def main():
     if __name__ == '__main__':
         n_wt = 16
         site = IEA37Site(n_wt)
         windTurbines = IEA37_WindTurbines()
         windFarmModel = IEA37SimpleBastankhahGaussian(site, windTurbines)
         tf = TopFarmProblem(
```

### Comparing `topfarm-2.3.2/topfarm/cost_models/utils/spanning_tree.py` & `topfarm-2.3.4/topfarm/cost_models/utils/spanning_tree.py`

 * *Files identical despite different names*

### Comparing `topfarm-2.3.2/topfarm/deprectated_topfarm_problems.py` & `topfarm-2.3.4/topfarm/deprectated_topfarm_problems.py`

 * *Files identical despite different names*

### Comparing `topfarm-2.3.2/topfarm/drivers/genetic_algorithm_driver.py` & `topfarm-2.3.4/topfarm/drivers/genetic_algorithm_driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,18 @@
 import os
 import copy
 
 from six import iteritems, itervalues, next
 from six.moves import range, zip
 
 import numpy as np
-from pyDOE2 import lhs
+try:
+    from pyDOE2 import lhs
+except ModuleNotFoundError:
+    from pyDOE3 import lhs
 
 import openmdao
 from openmdao.core.driver import Driver, RecordingDebugging
 from openmdao.utils.concurrent import concurrent_eval
 from openmdao.utils.mpi import MPI
 from openmdao.core.analysis_error import AnalysisError
```

### Comparing `topfarm-2.3.2/topfarm/drivers/random_search_driver.py` & `topfarm-2.3.4/topfarm/drivers/random_search_driver.py`

 * *Files identical despite different names*

### Comparing `topfarm-2.3.2/topfarm/drivers/stochastic_gradient_descent_driver.py` & `topfarm-2.3.4/topfarm/drivers/stochastic_gradient_descent_driver.py`

 * *Files identical despite different names*

### Comparing `topfarm-2.3.2/topfarm/easy_drivers.py` & `topfarm-2.3.4/topfarm/easy_drivers.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
             for lst in [scipy_optimizer._optimizers, scipy_optimizer._gradient_optimizers, scipy_optimizer._bounds_optimizers,
                         scipy_optimizer._all_optimizers, scipy_optimizer._constraint_optimizers, scipy_optimizer._constraint_grad_optimizers]:
                 lst.add(minimize_sgd_wrapper)
             optimizer = minimize_sgd_wrapper
 
         self.options.update({'optimizer': optimizer, 'maxiter': self.max_iter or maxiter, 'tol': tol, 'disp': disp})
         if kwargs:
-            self.options.update(kwargs)
+            self.opt_settings.update(kwargs)
 
     def get_desvar_kwargs(self, model, desvar_name, desvar_values):
         kwargs = super().get_desvar_kwargs(model, desvar_name, desvar_values)
         if self.options['optimizer'] == 'SLSQP':
             if tuple([int(v) for v in scipy.__version__.split(".")]) < (1, 5, 0):
                 # Upper and lower disturbs SLSQP when running with constraints. Add limits as constraints
                 model.add_constraint(desvar_name, kwargs.get('lower', None), kwargs.get('upper', None))
@@ -191,21 +191,26 @@
                                       'start_with_resto': 'yes',
                                       'expect_infeasible_problem': 'yes'})
 
     from pyoptsparse.pyIPOPT.pyIPOPT import pyipoptcore
     if pyipoptcore is None:
         setattr(sys.modules[__name__], 'EasyPyOptSparseIPOPT', PyOptSparseMissingDriver)
 
+    # Test if the SNOPT optimizer is available in the installation. This gives an exception even if pyOptSparseDriver is successfully instantiated with 'SNOPT'
+    _tmp = __import__('pyoptsparse', globals(), locals(), ['SNOPT'], 0)
+    getattr(_tmp, 'SNOPT')()
+
     class EasyPyOptSparseSNOPT(pyOptSparseDriver, EasyDriverBase):
         def __init__(self, major_iteration_limit=200, major_feasibility_tolerance=1e-6, major_optimality_tolerance=1e-6,
                      difference_interval=1e-6, function_precision=1e-8,
                      Print_file='SNOPT_print.out', Summary_file='SNOPT_summary.out', print_results=False):
             """For information about the arguments see
             https://web.stanford.edu/group/SOL/software/snoptHelp/whgdata/whlstt9.htm#9
             """
+
             pyOptSparseDriver.__init__(self)
             self.options.update({'optimizer': 'SNOPT', 'print_results': print_results})
             self.opt_settings.update({
                 'Major feasibility tolerance': major_feasibility_tolerance,
                 'Major optimality tolerance': major_optimality_tolerance,
                 'Difference interval': difference_interval,
                 'Hessian full memory': None,
@@ -221,15 +226,15 @@
                 ref0 = np.min(desvar_values[1])
                 ref1 = np.max(desvar_values[2])
                 l, u = desvar_values[1], desvar_values[2]
                 kwargs = {'ref0': ref0, 'ref': ref1, 'lower': l, 'upper': u}
             return kwargs
 
 
-except ModuleNotFoundError:
+except (ModuleNotFoundError, Exception):
     for n in ['EasyPyOptSparseSLSQP', 'EasyPyOptSparseIPOPT', 'EasyPyOptSparseSNOPT']:
         setattr(sys.modules[__name__], n, PyOptSparseMissingDriver)
 
 
 class EasySimpleGADriver(SimpleGADriver, EasyDriverBase):
     def __init__(self, max_gen=100, pop_size=25, Pm=None, Pc=.5, elitism=True,
                  bits={}, debug_print=[], run_parallel=False, random_state=None):
```

### Comparing `topfarm-2.3.2/topfarm/examples/data/parque_ficticio_offshore.py` & `topfarm-2.3.4/topfarm/examples/data/parque_ficticio_offshore.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,9 +43,13 @@
         ds['x'] = x
         ds['y'] = y
         XRSite.__init__(self, ds)
         self.boundary = boundary
         self.initial_position = np.array([wt_x, wt_y]).T
 
 
-if __name__ == '__main__':
-    site = ParqueFicticioOffshore()
+def main():
+    if __name__ == '__main__':
+        ParqueFicticioOffshore()
+
+
+main()
```

### Comparing `topfarm-2.3.2/topfarm/examples/iea37/_iea37.py` & `topfarm-2.3.4/topfarm/examples/iea37/_iea37.py`

 * *Files 17% similar despite different names*

```diff
@@ -49,23 +49,27 @@
     wd = npa(range(16)) * 22.5  # only 16 bins
     site = IEA37Site(n_wt)
     wind_turbines = IEA37_WindTurbines()
     wake_model = IEA37SimpleBastankhahGaussian(site, wind_turbines)
     return PyWakeAEPCostModelComponent(wake_model, n_wt, wd=wd)
 
 
-if __name__ == '__main__':
-    from topfarm import TopFarmProblem
-    from topfarm import EasyRandomSearchDriver
-    from topfarm.drivers.random_search_driver import RandomizeTurbinePosition_Circle
-    from topfarm.plotting import XYPlotComp
-    n_wt = 16
-    x, y = get_iea37_initial(n_wt).T * 0.99999  # make sure the turbines numerically are inside the boundary for random search driver
-    constr = get_iea37_constraints(n_wt)
-    cost = get_iea37_cost(n_wt)
-    driver = EasyRandomSearchDriver(RandomizeTurbinePosition_Circle(max_step=300), max_iter=10, max_time=10)
-    problem = TopFarmProblem({'x': x, 'y': y},
-                             cost_comp=cost,
-                             constraints=constr,
-                             driver=driver,
-                             plot_comp=XYPlotComp())
-    problem.evaluate()
+def main():
+    if __name__ == '__main__':
+        from topfarm import TopFarmProblem
+        from topfarm import EasyRandomSearchDriver
+        from topfarm.drivers.random_search_driver import RandomizeTurbinePosition_Circle
+        from topfarm.plotting import XYPlotComp
+        n_wt = 16
+        x, y = get_iea37_initial(n_wt).T * 0.99999  # make sure the turbines numerically are inside the boundary for random search driver
+        constr = get_iea37_constraints(n_wt)
+        cost = get_iea37_cost(n_wt)
+        driver = EasyRandomSearchDriver(RandomizeTurbinePosition_Circle(max_step=300), max_iter=10, max_time=10)
+        problem = TopFarmProblem({'x': x, 'y': y},
+                                 cost_comp=cost,
+                                 constraints=constr,
+                                 driver=driver,
+                                 plot_comp=XYPlotComp())
+        problem.evaluate()
+
+
+main()
```

### Comparing `topfarm-2.3.2/topfarm/mongo_recorder.py` & `topfarm-2.3.4/topfarm/mongo_recorder.py`

 * *Files 0% similar despite different names*

```diff
@@ -340,41 +340,42 @@
 
         driver = None
 
         # grab the system and driver
         if isinstance(recording_requester, Driver):
             system = recording_requester._problem().model
             driver = recording_requester
-        elif isinstance(recording_requester, System):
-            system = recording_requester
-            driver = None
-        elif isinstance(recording_requester, Problem):
-            system = recording_requester.model
-            driver = recording_requester.driver
-        elif isinstance(recording_requester, Solver):
-            system = recording_requester._system()
-            driver = None
+        # elif isinstance(recording_requester, System):
+        #     system = recording_requester
+        #     driver = None
+        # elif isinstance(recording_requester, Problem):
+        #     system = recording_requester.model
+        #     driver = recording_requester.driver
+        # elif isinstance(recording_requester, Solver):
+        #     system = recording_requester._system()
+        #     driver = None
         else:
             raise ValueError('Driver encountered a recording_requester it cannot handle'
                              ': {0}'.format(recording_requester))
 
         states = system._list_states_allprocs()
 
         if self.connection:
 
             if driver is None:
-                desvars = system.get_design_vars(True, get_sizes=False, use_prom_ivc=False)
-                responses = system.get_responses(True, get_sizes=False)
-                constraints = OrderedDict()
-                objectives = OrderedDict()
-                for name, data in responses.items():
-                    if data['type'] == 'con':
-                        constraints[name] = data
-                    else:
-                        objectives[name] = data
+                pass
+                # desvars = system.get_design_vars(True, get_sizes=False, use_prom_ivc=False)
+                # responses = system.get_responses(True, get_sizes=False)
+                # constraints = OrderedDict()
+                # objectives = OrderedDict()
+                # for name, data in responses.items():
+                #     if data['type'] == 'con':
+                #         constraints[name] = data
+                #     else:
+                #         objectives[name] = data
             else:
                 desvars = driver._designvars.copy()
                 responses = driver._responses.copy()
                 constraints = driver._cons.copy()
                 objectives = driver._objs.copy()
 
             inputs = list(system.abs_name_iter('input', local=False, discrete=True))
@@ -485,20 +486,20 @@
         self._counter += 1
 
         self._iteration_coordinate = \
             recording_requester._recording_iter.get_formatted_iteration_coordinate()
 
         if isinstance(recording_requester, Driver):
             self.record_iteration_driver(recording_requester, data, metadata)
-        elif isinstance(recording_requester, System):
-            self.record_iteration_system(recording_requester, data, metadata)
-        elif isinstance(recording_requester, Solver):
-            self.record_iteration_solver(recording_requester, data, metadata)
-        elif isinstance(recording_requester, Problem):
-            self.record_iteration_problem(recording_requester, data, metadata)
+        # elif isinstance(recording_requester, System):
+        #     self.record_iteration_system(recording_requester, data, metadata)
+        # elif isinstance(recording_requester, Solver):
+        #     self.record_iteration_solver(recording_requester, data, metadata)
+        # elif isinstance(recording_requester, Problem):
+        #     self.record_iteration_problem(recording_requester, data, metadata)
         else:
             raise ValueError("Recorders must be attached to Drivers, Systems, or Solvers.")
 
     def record_iteration_driver(self, driver, data, metadata):
         """
         Record data and metadata from a Driver.
```

### Comparing `topfarm-2.3.2/topfarm/parallel_runner.py` & `topfarm-2.3.4/topfarm/parallel_runner.py`

 * *Files identical despite different names*

### Comparing `topfarm-2.3.2/topfarm/plotting.py` & `topfarm-2.3.4/topfarm/plotting.py`

 * *Files 8% similar despite different names*

```diff
@@ -284,109 +284,100 @@
 
     def plot_current_position(self, x, y):
         for m, c, x_, y_ in zip(self.markers[self.types], self.colors[self.types], x, y):
             # self.ax.plot(x_, y_, 'o', color=c, ms=5)
             self.ax.plot(x_, y_, m + 'k', markeredgecolor=c, markeredgewidth=1, ms=20)
 
 
-class TurbineCablePlotComponent(XYPlotComp):
-    """Plotting component for electrical colletion system"""
-    colors = ['b', 'r', 'm', 'c', 'g', 'y', 'orange', 'indigo', 'grey'] * 100
-
-    def __init__(self, ecsga, **kwargs):
-        """Initialize component for plotting turbine types
-
-        Parameters
-        ----------
-        turbine_type_names : list of str
-            Names of turbine types for legend
-        **kwargs : keyword arguments, optional
-            Keyword arguments that can be passed into XYPlotComp
-        """
-        self.ecsga = ecsga
-        XYPlotComp.__init__(self, **kwargs)
-
-    def setup(self):
-        XYPlotComp.setup(self)
-        self.add_input('tree', np.zeros((self.n_wt, 5)))
-
-    def compute(self, inputs, outputs):
-        self.tree = np.asarray(inputs['tree'])
-        XYPlotComp.compute(self, inputs, outputs)
-
-    def init_plot(self, limits):
-        XYPlotComp.init_plot(self, limits)
-        for n, cable_type in enumerate(self.ecsga.Cable.ID):
-            index = self.tree[:, 3] == n
-            if index.any():
-                self.ax.plot([], [], self.colors[n], label='Cable: {} mm2'.format(self.ecsga.Cable.CrossSection[n]))
-        self.ax.legend()
-
-    def plot_current_position(self, x, y):
-        CoordX = self.ecsga.CoordX
-        CoordY = self.ecsga.CoordY
-        CoordX[1:] = x
-        CoordY[1:] = y
-        self.ax.plot(CoordX[0], CoordY[0], 'ro', markersize=10, label='OSS')
-#        if (self.tree[0].shape)[1] == 2: # If no feasible solution was found
-#            n1xs = CoordX[(self.tree[0].T[0:1]-1).astype(int)].ravel().T
-#            n2xs = CoordX[(self.tree[0].T[1:2]-1).astype(int)].ravel().T
-#            n1ys = CoordY[(self.tree[0].T[0:1]-1).astype(int)].ravel().T
-#            n2ys = CoordY[(self.tree[0].T[1:2]-1).astype(int)].ravel().T
-#            xs = np.vstack([n1xs,n2xs])
-#            ys = np.vstack([n1ys,n2ys])
-#            plt.plot(xs,ys,'{}'.format(self.colors[0]))
-#        else:
-        for n, cable_type in enumerate(self.ecsga.Cable.ID):
-            index = self.tree[:, 3].astype(int) == n
-            if index.any():
-                xs = CoordX[(self.tree[index].T[:2] - 1).astype(int)]
-                ys = CoordY[(self.tree[index].T[:2] - 1).astype(int)]
-                self.ax.plot(xs, ys, self.colors[n])
-
-
-class AggregatedConstraintsPlotComponent(XYPlotComp):
-
-    colors = np.array(['b', 'r', 'm', 'c', 'g', 'y', 'orange', 'indigo', 'grey'] * 10)
-    markers = np.array(list("123v^<>.o48spP*hH+xXDd|_"))
-
-    def show(self):
-        pass
-
-    def plot_constraints(self):
-        if len(self.problem.model.aggr_comp.constraints) != 0:
-            for constr in self.problem.model.aggr_comp.constraints[0].constraints:
-                constr.constraintComponent.plot(self.ax)
-        else:
-            for constr in self.problem.model.constraint_components:
-                constr.plot(self.ax)
-
-    def plot_history(self, x, y):
-        rec = self.problem.recorder
-        if rec.num_cases > 0:
-            def get(xy, xy_key, pw):
-                rec_xy = pw[xy_key][-self.memory:]
-                if len(rec_xy.shape) == 1:
-                    rec_xy = rec_xy[:, np.newaxis]
-                return np.r_[rec_xy, [xy]]
-            pw = self.problem.get_vars_from_recorder()
-            x = get(x, topfarm.x_key, pw)
-            y = get(y, topfarm.y_key, pw)
-            for c, x_, y_ in zip(self.colors, x.T, y.T):
-                self.ax.plot(x_, y_, '--', color=c)
-
-    def plot_initial2current(self, x0, y0, x, y):
-        rec = self.problem.recorder
-        if rec.num_cases > 0:
-            pw = self.problem.get_vars_from_recorder()
-            x0 = np.atleast_1d(pw['x0'])
-            y0 = np.atleast_1d(pw['y0'])
-            for c, x0_, y0_, x_, y_ in zip(self.colors, x0, y0, x, y):
-                self.ax.plot(x0_, y0_, '>', markerfacecolor=c, markeredgecolor='k')
-                self.ax.plot((x0_, x_), (y0_, y_), '-', color=c)
-            self.ax.plot([], [], '>k', markerfacecolor="#00000000", markeredgecolor='k', label='Initial position')
-
-    def plot_current_position(self, x, y):
-        for c, x_, y_ in zip(self.colors, x, y):
-            self.ax.plot(x_, y_, 'o', color=c, ms=5)
-            self.ax.plot(x_, y_, 'xk', ms=4)
-        self.ax.plot([], [], 'xk', label='Current position')
+# class TurbineCablePlotComponent(XYPlotComp):
+#     """Plotting component for electrical colletion system"""
+#     colors = ['b', 'r', 'm', 'c', 'g', 'y', 'orange', 'indigo', 'grey'] * 100
+
+#     def __init__(self, ecsga, **kwargs):
+#         """Initialize component for plotting turbine types
+
+#         Parameters
+#         ----------
+#         turbine_type_names : list of str
+#             Names of turbine types for legend
+#         **kwargs : keyword arguments, optional
+#             Keyword arguments that can be passed into XYPlotComp
+#         """
+#         self.ecsga = ecsga
+#         XYPlotComp.__init__(self, **kwargs)
+
+#     def setup(self):
+#         XYPlotComp.setup(self)
+#         self.add_input('tree', np.zeros((self.n_wt, 5)))
+
+#     def compute(self, inputs, outputs):
+#         self.tree = np.asarray(inputs['tree'])
+#         XYPlotComp.compute(self, inputs, outputs)
+
+#     def init_plot(self, limits):
+#         XYPlotComp.init_plot(self, limits)
+#         for n, cable_type in enumerate(self.ecsga.Cable.ID):
+#             index = self.tree[:, 3] == n
+#             if index.any():
+#                 self.ax.plot([], [], self.colors[n], label='Cable: {} mm2'.format(self.ecsga.Cable.CrossSection[n]))
+#         self.ax.legend()
+
+#     def plot_current_position(self, x, y):
+#         CoordX = self.ecsga.CoordX
+#         CoordY = self.ecsga.CoordY
+#         CoordX[1:] = x
+#         CoordY[1:] = y
+#         self.ax.plot(CoordX[0], CoordY[0], 'ro', markersize=10, label='OSS')
+#         for n, cable_type in enumerate(self.ecsga.Cable.ID):
+#             index = self.tree[:, 3].astype(int) == n
+#             if index.any():
+#                 xs = CoordX[(self.tree[index].T[:2] - 1).astype(int)]
+#                 ys = CoordY[(self.tree[index].T[:2] - 1).astype(int)]
+#                 self.ax.plot(xs, ys, self.colors[n])
+
+
+# class AggregatedConstraintsPlotComponent(XYPlotComp):
+
+#     colors = np.array(['b', 'r', 'm', 'c', 'g', 'y', 'orange', 'indigo', 'grey'] * 10)
+#     markers = np.array(list("123v^<>.o48spP*hH+xXDd|_"))
+
+#     def show(self):
+#         pass
+
+#     def plot_constraints(self):
+#         # if len(self.problem.model.aggr_comp.constraints) != 0:
+#         #     for constr in self.problem.model.aggr_comp.constraints[0].constraints:
+#         #         constr.constraintComponent.plot(self.ax)
+#         # else:
+#         for constr in self.problem.model.constraint_components:
+#             constr.plot(self.ax)
+
+#     def plot_history(self, x, y):
+#         rec = self.problem.recorder
+#         if rec.num_cases > 0:
+#             def get(xy, xy_key, pw):
+#                 rec_xy = pw[xy_key][-self.memory:]
+#                 if len(rec_xy.shape) == 1:
+#                     rec_xy = rec_xy[:, np.newaxis]
+#                 return np.r_[rec_xy, [xy]]
+#             pw = self.problem.get_vars_from_recorder()
+#             x = get(x, topfarm.x_key, pw)
+#             y = get(y, topfarm.y_key, pw)
+#             for c, x_, y_ in zip(self.colors, x.T, y.T):
+#                 self.ax.plot(x_, y_, '--', color=c)
+
+#     def plot_initial2current(self, x0, y0, x, y):
+#         rec = self.problem.recorder
+#         if rec.num_cases > 0:
+#             pw = self.problem.get_vars_from_recorder()
+#             x0 = np.atleast_1d(pw['x0'])
+#             y0 = np.atleast_1d(pw['y0'])
+#             for c, x0_, y0_, x_, y_ in zip(self.colors, x0, y0, x, y):
+#                 self.ax.plot(x0_, y0_, '>', markerfacecolor=c, markeredgecolor='k')
+#                 self.ax.plot((x0_, x_), (y0_, y_), '-', color=c)
+#             self.ax.plot([], [], '>k', markerfacecolor="#00000000", markeredgecolor='k', label='Initial position')
+
+#     def plot_current_position(self, x, y):
+#         for c, x_, y_ in zip(self.colors, x, y):
+#             self.ax.plot(x_, y_, 'o', color=c, ms=5)
+#             self.ax.plot(x_, y_, 'xk', ms=4)
+#         self.ax.plot([], [], 'xk', label='Current position')
```

### Comparing `topfarm-2.3.2/topfarm/recorders.py` & `topfarm-2.3.4/topfarm/recorders.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,15 +204,15 @@
         if load_case == 'none' or load_case == '0':
             return self
 
         self.list_load(filename)
         if load_case == 'latest':
             load_case = None
         elif load_case == 'best':
-            load_case = np.argmin(self.get('aggr_cost')) + 1
+            load_case = np.argmin(self.get('final_cost')) + 1
         else:
             load_case = int(load_case)
         self.driver_iteration_dict = {k: v[:load_case] for k, v in self.driver_iteration_dict.items()}
         self.iteration_coordinate_lst = self.iteration_coordinate_lst[:load_case]
 
         self.filename, self.load_case = filename, load_case
         return self
```

### Comparing `topfarm-2.3.2/topfarm/tests/notebook.py` & `topfarm-2.3.4/topfarm/tests/notebook.py`

 * *Files identical despite different names*

### Comparing `topfarm-2.3.2/topfarm/tests/test_constraint/test_BoundaryBaseComp.py` & `topfarm-2.3.4/topfarm/tests/test_constraint/test_BoundaryBaseComp.py`

 * *Files identical despite different names*

### Comparing `topfarm-2.3.2/topfarm/tests/test_constraint/test_CircleBoundaryComp.py` & `topfarm-2.3.4/topfarm/tests/test_constraint/test_CircleBoundaryComp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import os
+import numpy as np
 
 from openmdao.drivers.genetic_algorithm_driver import SimpleGADriver
 import pytest
 
-import numpy as np
 from topfarm._topfarm import TopFarmProblem
-from topfarm.constraint_components.boundary import ConvexBoundaryComp,\
-    CircleBoundaryConstraint, CircleBoundaryComp
-from topfarm.cost_models.dummy import DummyCost, DummyCostPlotComp
+from topfarm.constraint_components.boundary import CircleBoundaryConstraint, CircleBoundaryComp
+from topfarm.cost_models.dummy import DummyCost
 from topfarm.plotting import NoPlot, PlotComp
 from topfarm.tests import npt
 
 
 def testCircle():
     b = CircleBoundaryComp(3, [1, 2], 3)
     np.testing.assert_array_almost_equal(((b.xy_boundary - [1, 2])**2).sum(1), 3**2)
```

### Comparing `topfarm-2.3.2/topfarm/tests/test_constraint/test_ConvexBoundaryComp.py` & `topfarm-2.3.4/topfarm/tests/test_constraint/test_ConvexBoundaryComp.py`

 * *Files identical despite different names*

### Comparing `topfarm-2.3.2/topfarm/tests/test_constraint/test_PolygonBoundaryComp.py` & `topfarm-2.3.4/topfarm/tests/test_constraint/test_PolygonBoundaryComp.py`

 * *Files identical despite different names*

### Comparing `topfarm-2.3.2/topfarm/tests/test_constraint/test_boundary_polygon.py` & `topfarm-2.3.4/topfarm/tests/test_constraint/test_boundary_polygon.py`

 * *Files 17% similar despite different names*

```diff
@@ -113,15 +113,15 @@
                         plot_comp=plot_comp, driver=EasyScipyOptimizeDriver(tol=1e-8, disp=False))
     tf.evaluate()
     cost, state, recorder = tf.optimize()
     np.testing.assert_array_almost_equal(tf.turbine_positions[:, :2], optimal, 4)
     relaxation = tf.model.constraint_components[0].calc_relaxation() \
         + tf.model.constraint_components[0].relaxation[0]
     assert tf.cost_comp.n_grad_eval <= 10
-    assert tf.model.pre_constraints.xy_bound_comp == tf.model.constraint_components[0]
+    assert tf.model.constraint_group.xy_bound_comp == tf.model.constraint_components[0]
     # distances in the 2 lower corners should be the same
     assert tf.model.constraint_components[0].distances(np.array([0]), np.array([0])) \
         == tf.model.constraint_components[0].distances(np.array([5]), np.array([0]))
     # gradients with respect of iteration number should be the same at every point
     assert tf.model.constraint_components[0].gradients(np.array([3]), np.array([5]))[2][0] \
         == tf.model.constraint_components[0].gradients(np.array([1.5]), np.array([8]))[2][1]
 
@@ -144,7 +144,31 @@
                                                     [-0.3, -0.3],
                                                     [-0.3, 2.3],
                                                     [2.3, 2.3]]))
     np.testing.assert_allclose(bp2[0][0], np.array([[1.45, 1.2],
                                                     [0.8, 1.2],
                                                     [0.8, 0.8],
                                                     [1.45, 0.8]]))
+
+
+def testChangingNumberOfTurbines():
+    zones = [InclusionZone([(0, 0), (5, 0), (5, 2), (3, 2), (3, 1), (2, 1), (2, 2), (0, 2), (0, 0)]),
+             InclusionZone([(3.5, 0.5), (4.5, 0.5), (4.5, 1.5), (3.5, 1.5)]),
+             ExclusionZone([(0.5, 0.5), (1.75, 0.5), (1.75, 1.5), (0.5, 1.5)]),
+             ExclusionZone([(0.75, 0.75), (1.25, 0.75), (1.25, 1.25), (0.75, 1.25)]),
+             ]
+
+    MPBC = MultiPolygonBoundaryComp(1, zones)
+
+    xs, ys = np.linspace(0, 5, 5), np.linspace(0, 2, 5)
+    XS, YS = np.meshgrid(xs, ys)
+    X, Y = XS.ravel(), YS.ravel()
+    _, _, sign = MPBC.calc_distance_and_gradients(X, Y)
+    sign_ref = np.array([0, 0, 0, 0, 0, 0, 0, 1, 1, 0, 0, -1, 0, 1, 0, 0, 0, -1, 1, 0, 0, 0, -1, 0, 0])
+    np.testing.assert_allclose(sign, sign_ref)
+
+    xs2, ys2 = np.linspace(0, 5, 2), np.linspace(0, 2, 1)
+    XS2, YS2 = np.meshgrid(xs2, ys2)
+    X2, Y2 = XS2.ravel(), YS2.ravel()
+    _, _, sign2 = MPBC.calc_distance_and_gradients(X2, Y2)
+    sign_ref2 = np.array([0, 0])
+    np.testing.assert_allclose(sign2, sign_ref2)
```

### Comparing `topfarm-2.3.2/topfarm/tests/test_constraint/test_capacityComp.py` & `topfarm-2.3.4/topfarm/tests/test_constraint/test_capacityComp.py`

 * *Files 22% similar despite different names*

```diff
@@ -28,14 +28,14 @@
                         constraints=[CapacityConstraint(max_capacity=50, rated_power_array=rated_power_array_kW)],
                         driver=EasySimpleGADriver()
                         )
 
     tf.evaluate()
     # case above the maximum allowed installed capacity, yes penalty
     assert tf["totalcapacity"] == 82.5
-    assert tf['penalty_comp.penalty_capacity_comp_50'] == 32.5
+    assert tf['constraint_violation_comp.constraint_violation'] == 32.5
 
     # set all turbines type 0, still 15 turbines and re-run the problem
     tf.evaluate({'type': inputtypes * 0})
     # case below the maximum allowed installed capacity, no penalty
     assert tf["totalcapacity"] == 15
-    assert tf['penalty_comp.penalty_capacity_comp_50'][0] == 0.0
+    assert tf['constraint_violation_comp.constraint_violation'][0] == 0.0
```

### Comparing `topfarm-2.3.2/topfarm/tests/test_constraint/test_constrained_generator.py` & `topfarm-2.3.4/topfarm/tests/test_constraint/test_constrained_generator.py`

 * *Files identical despite different names*

### Comparing `topfarm-2.3.2/topfarm/tests/test_constraint/test_loads.py` & `topfarm-2.3.4/topfarm/tests/test_constraint/test_loads.py`

 * *Files identical despite different names*

### Comparing `topfarm-2.3.2/topfarm/tests/test_constraint/test_spacingComp.py` & `topfarm-2.3.4/topfarm/tests/test_constraint/test_spacingComp.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,15 +188,15 @@
     check = tf.check_partials(compact_print=True,
                               includes='sc*',
                               method='fd',
                               step=1e-6,
                               form='central')
 
     fil = {'sc': {key: val for key, val in check['sc'].items()
-                  if 'penalty' not in key[0]}}
+                  if 'constraint_violation' not in key[0]}}
 
     atol = 1.e-6
     rtol = 1.e-6
     try:
         assert_check_partials(fil, atol, rtol)
     except ValueError as err:
         print(str(err))
```

### Comparing `topfarm-2.3.2/topfarm/tests/test_costmodel_utils/test_cost_model_wrappers.py` & `topfarm-2.3.4/topfarm/tests/test_costmodel_utils/test_cost_model_wrappers.py`

 * *Files identical despite different names*

### Comparing `topfarm-2.3.2/topfarm/tests/test_costmodel_utils/test_spanning_tree.py` & `topfarm-2.3.4/topfarm/tests/test_costmodel_utils/test_spanning_tree.py`

 * *Files identical despite different names*

### Comparing `topfarm-2.3.2/topfarm/tests/test_examples.py` & `topfarm-2.3.4/topfarm/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `topfarm-2.3.2/topfarm/tests/test_files/example_data/floris/NREL5MW.py` & `topfarm-2.3.4/topfarm/tests/test_files/example_data/floris/NREL5MW.py`

 * *Files identical despite different names*

### Comparing `topfarm-2.3.2/topfarm/tests/test_files/xy3tb.py` & `topfarm-2.3.4/topfarm/tests/test_files/xy3tb.py`

 * *Files identical despite different names*

### Comparing `topfarm-2.3.2/topfarm/tests/test_fuga/test_pyfuga.py` & `topfarm-2.3.4/topfarm/tests/test_fuga/test_pyfuga.py`

 * *Files identical despite different names*

### Comparing `topfarm-2.3.2/topfarm/tests/test_main.py` & `topfarm-2.3.4/topfarm/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `topfarm-2.3.2/topfarm/tests/test_notebooks.py` & `topfarm-2.3.4/topfarm/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `topfarm-2.3.2/topfarm/tests/test_topfarm_problems/test_TopFarmProblem.py` & `topfarm-2.3.4/topfarm/tests/test_topfarm_problems/test_TopFarmProblem.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,15 +171,15 @@
     tf = turbineXYZOptimizationProblem_generator(None, cost_comp)
     with pytest.raises(Warning, match="Mismatch between finite difference derivative of 'cost' wrt. 'y' and derivative computed in 'cost_comp' is"):
         tf.check_gradients()
 
 
 def testTopFarmProblem_evaluate_gradients(turbineXYZOptimizationProblem_generator):
     tf = turbineXYZOptimizationProblem_generator(gradients)
-    np.testing.assert_array_equal(tf.evaluate_gradients(disp=True)['aggr_cost']['x'], [[-6., -14., -8., -6.]])
+    np.testing.assert_array_equal(tf.evaluate_gradients(disp=True)['final_cost']['x'], [[-6., -14., -8., -6.]])
 
 
 def testTopFarmProblem_as_component(turbineTypeOptimizationProblem):
     tf = turbineTypeOptimizationProblem
     c = tf.as_component()
     npt.assert_equal(c.__class__, ProblemComponent)
     assert c.problem == tf
@@ -294,7 +294,12 @@
     tf = xy3tb.get_tf(approx_totals=True)
     np.testing.assert_array_equal(tf.turbine_positions, xy3tb.initial)
 
 
 def testTopFarmProblem_expected_cost():
     tf = xy3tb.get_tf(expected_cost=None)
     np.testing.assert_array_equal(tf.turbine_positions, xy3tb.initial)
+
+
+def testTopFarmProblem_update_reports(turbineTypeOptimizationProblem):
+    tf = turbineTypeOptimizationProblem
+    tf._update_reports(DOEDriver(FullFactorialGenerator(3)))
```

### Comparing `topfarm-2.3.2/topfarm/tests/test_topfarm_problems/test_TopFarmProblem_limits_and_constraints.py` & `topfarm-2.3.4/topfarm/tests/test_topfarm_problems/test_TopFarmProblem_limits_and_constraints.py`

 * *Files identical despite different names*

### Comparing `topfarm-2.3.2/topfarm/tests/test_topfarm_problems/test_nested_problems.py` & `topfarm-2.3.4/topfarm/tests/test_topfarm_problems/test_nested_problems.py`

 * *Files identical despite different names*

### Comparing `topfarm-2.3.2/topfarm/tests/test_topfarm_problems/test_optimization_problems.py` & `topfarm-2.3.4/topfarm/tests/test_topfarm_problems/test_optimization_problems.py`

 * *Files identical despite different names*

### Comparing `topfarm-2.3.2/topfarm/tests/test_topfarm_utils/test_drivers.py` & `topfarm-2.3.4/topfarm/tests/test_topfarm_utils/test_drivers.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 
     tb_pos = tf.turbine_positions[:, :2]
 
     assert sum((tb_pos[2] - tb_pos[0])**2) > 2**2 - tol  # check min spacing
     assert tb_pos[1][0] < 6 + tol  # check within border
     tf.plot_comp.show()
     if isinstance(driver, EasySimpleGADriver):
-        assert cost == recorder['cost'].min()
+        assert cost == recorder['final_cost'].min()
     else:
         np.testing.assert_array_almost_equal(tb_pos, optimal[:, :2], -int(np.log10(tol)))
 
 
 @pytest.mark.parametrize('driver,tol,N', [
     (EasyScipyOptimizeDriver(disp=False), 1e-4, 30),
     (EasyPyOptSparseSNOPT(), 1e-4, 39),
```

### Comparing `topfarm-2.3.2/topfarm/tests/test_topfarm_utils/test_parellel_runner.py` & `topfarm-2.3.4/topfarm/tests/test_topfarm_utils/test_parellel_runner.py`

 * *Files identical despite different names*

### Comparing `topfarm-2.3.2/topfarm/tests/test_topfarm_utils/test_recorders.py` & `topfarm-2.3.4/topfarm/tests/test_topfarm_utils/test_recorders.py`

 * *Files identical despite different names*

### Comparing `topfarm-2.3.2/topfarm/tests/test_topfarm_utils/test_utils.py` & `topfarm-2.3.4/topfarm/tests/test_topfarm_utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `topfarm-2.3.2/topfarm/tests/test_with_dummy.py` & `topfarm-2.3.4/topfarm/tests/test_with_dummy.py`

 * *Files identical despite different names*

### Comparing `topfarm-2.3.2/topfarm/utils.py` & `topfarm-2.3.4/topfarm/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,31 +120,31 @@
 
         x0 = arr[0][next_ind]
         y0 = arr[1][next_ind]
         xs.append(x0)
         ys.append(y0)
 
         if plot:
-            if types:
-                for typ in types:
-                    plt.figure()
-                    c = plt.scatter(arr[0, :, typ], arr[1, :, typ], c=arr[2, :, typ])
-                    plt.colorbar(c)
-                    plt.plot(xs, ys, '2k', ms=10)
-                    plt.plot(xs[-1], ys[-1], '2r', ms=10)
-                    plt.axis('equal')
-                    plt.show()
-            else:
-                plt.figure()
-                c = plt.scatter(arr[0], arr[1], c=z)
-                plt.colorbar(c)
-                plt.plot(xs, ys, '2k', ms=10)
-                plt.plot(xs[-1], ys[-1], '2r', ms=10)
-                plt.axis('equal')
-                plt.show()
+            # if types:
+            #     for typ in types:
+            #         plt.figure()
+            #         c = plt.scatter(arr[0, :, typ], arr[1, :, typ], c=arr[2, :, typ])
+            #         plt.colorbar(c)
+            #         plt.plot(xs, ys, '2k', ms=10)
+            #         plt.plot(xs[-1], ys[-1], '2r', ms=10)
+            #         plt.axis('equal')
+            #         plt.show()
+            # else:
+            plt.figure()
+            c = plt.scatter(arr[0], arr[1], c=z)
+            plt.colorbar(c)
+            plt.plot(xs, ys, '2k', ms=10)
+            plt.plot(xs[-1], ys[-1], '2r', ms=10)
+            plt.axis('equal')
+            plt.show()
 
         # Remove all point within min_space from the newly added wt
         if types:
             eff_min_space = (min_space + min_space[t]) / 2
             mask = np.logical_and(mask, ((arr[0, :, 0] - x0) ** 2 + (arr[1, :, 0] - y0) ** 2)[:, na] >= eff_min_space[na, :] ** 2)
             idx = mask.sum((1)) > 0
             arr = arr[:, idx, :]
```

### Comparing `topfarm-2.3.2/topfarm/workshop.py` & `topfarm-2.3.4/topfarm/workshop.py`

 * *Files identical despite different names*

### Comparing `topfarm-2.3.2/topfarm.egg-info/SOURCES.txt` & `topfarm-2.3.4/topfarm.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -41,21 +41,20 @@
 topfarm/constraint_components/boundary.py
 topfarm/constraint_components/boundary_component.py
 topfarm/constraint_components/capacity.py
 topfarm/constraint_components/constrained_generator.py
 topfarm/constraint_components/constraint_aggregation.py
 topfarm/constraint_components/load.py
 topfarm/constraint_components/penalty_component.py
-topfarm/constraint_components/post_constraint.py
 topfarm/constraint_components/spacing.py
 topfarm/cost_models/__init__.py
-topfarm/cost_models/aggregated_cost.py
 topfarm/cost_models/cost_model_wrappers.py
 topfarm/cost_models/dummy.py
 topfarm/cost_models/py_wake_wrapper.py
+topfarm/cost_models/topfarm_components.py
 topfarm/cost_models/economic_models/__init__.py
 topfarm/cost_models/economic_models/dtu_wind_cm_main.py
 topfarm/cost_models/economic_models/turbine_cost.py
 topfarm/cost_models/electrical/__init__.py
 topfarm/cost_models/electrical/simple_msp.py
 topfarm/cost_models/fuga/__init__.py
 topfarm/cost_models/fuga/py_fuga.py
@@ -84,14 +83,15 @@
 topfarm/tests/test_constraint/test_boundary_polygon.py
 topfarm/tests/test_constraint/test_capacityComp.py
 topfarm/tests/test_constraint/test_constrained_generator.py
 topfarm/tests/test_constraint/test_loads.py
 topfarm/tests/test_constraint/test_spacingComp.py
 topfarm/tests/test_costmodel_utils/__init__.py
 topfarm/tests/test_costmodel_utils/test_cost_model_wrappers.py
+topfarm/tests/test_costmodel_utils/test_cost_pywake_wrappers.py
 topfarm/tests/test_costmodel_utils/test_spanning_tree.py
 topfarm/tests/test_files/__init__.py
 topfarm/tests/test_files/xy3tb.py
 topfarm/tests/test_files/example_data/__init__.py
 topfarm/tests/test_files/example_data/floris/NREL5MW.py
 topfarm/tests/test_files/example_data/floris/__init__.py
 topfarm/tests/test_fuga/__init__.py
```

