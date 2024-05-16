# Comparing `tmp/smac-2.0.2.tar.gz` & `tmp/smac-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smac-2.0.2.tar", last modified: Tue Aug  1 13:20:09 2023, max compression
+gzip compressed data, was "smac-2.1.0.tar", last modified: Thu May 16 14:07:34 2024, max compression
```

## Comparing `smac-2.0.2.tar` & `smac-2.1.0.tar`

### file list

```diff
@@ -1,147 +1,147 @@
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-08-01 13:20:09.885776 smac-2.0.2/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3377 2023-03-03 09:52:31.000000 smac-2.0.2/LICENSE.txt
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      127 2023-07-31 15:47:05.000000 smac-2.0.2/MANIFEST.in
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     7245 2023-08-01 13:20:09.885776 smac-2.0.2/PKG-INFO
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     6116 2023-07-31 15:47:05.000000 smac-2.0.2/README.md
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2887 2023-07-31 15:47:05.000000 smac-2.0.2/pyproject.toml
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)       38 2023-08-01 13:20:09.885776 smac-2.0.2/setup.cfg
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2051 2023-08-01 13:05:49.000000 smac-2.0.2/setup.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-08-01 13:20:09.881776 smac-2.0.2/smac/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1555 2023-08-01 13:05:49.000000 smac-2.0.2/smac/__init__.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-08-01 13:20:09.881776 smac-2.0.2/smac/acquisition/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)        0 2023-07-31 15:47:05.000000 smac-2.0.2/smac/acquisition/__init__.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-08-01 13:20:09.881776 smac-2.0.2/smac/acquisition/function/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      717 2023-07-31 15:47:05.000000 smac-2.0.2/smac/acquisition/function/__init__.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3552 2023-07-31 15:47:05.000000 smac-2.0.2/smac/acquisition/function/abstract_acquisition_function.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3086 2023-07-31 15:47:05.000000 smac-2.0.2/smac/acquisition/function/confidence_bound.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     9061 2023-07-31 15:47:05.000000 smac-2.0.2/smac/acquisition/function/expected_improvement.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     4002 2023-07-31 15:47:05.000000 smac-2.0.2/smac/acquisition/function/integrated_acquisition_function.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     9380 2023-07-31 15:47:05.000000 smac-2.0.2/smac/acquisition/function/prior_acqusition_function.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2692 2023-07-31 15:47:05.000000 smac-2.0.2/smac/acquisition/function/probability_improvement.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1930 2023-07-31 15:47:05.000000 smac-2.0.2/smac/acquisition/function/thompson.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-08-01 13:20:09.881776 smac-2.0.2/smac/acquisition/maximizer/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      649 2023-07-31 15:47:05.000000 smac-2.0.2/smac/acquisition/maximizer/__init__.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     6213 2023-07-31 15:47:05.000000 smac-2.0.2/smac/acquisition/maximizer/abstract_acqusition_maximizer.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2344 2023-07-31 15:47:05.000000 smac-2.0.2/smac/acquisition/maximizer/differential_evolution.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     4165 2023-07-31 15:47:05.000000 smac-2.0.2/smac/acquisition/maximizer/helpers.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    10116 2023-07-31 15:47:05.000000 smac-2.0.2/smac/acquisition/maximizer/local_and_random_search.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    19915 2023-07-31 15:47:05.000000 smac-2.0.2/smac/acquisition/maximizer/local_search.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1828 2023-07-31 15:47:05.000000 smac-2.0.2/smac/acquisition/maximizer/random_search.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-08-01 13:20:09.881776 smac-2.0.2/smac/callback/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      160 2023-07-31 15:47:05.000000 smac-2.0.2/smac/callback/__init__.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2519 2023-07-31 15:47:05.000000 smac-2.0.2/smac/callback/callback.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1013 2023-07-31 15:47:05.000000 smac-2.0.2/smac/callback/metadata_callback.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      270 2023-07-31 15:47:05.000000 smac-2.0.2/smac/constants.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-08-01 13:20:09.881776 smac-2.0.2/smac/facade/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      674 2023-07-31 15:47:05.000000 smac-2.0.2/smac/facade/__init__.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    21480 2023-08-01 13:05:49.000000 smac-2.0.2/smac/facade/abstract_facade.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     6199 2023-07-31 15:47:05.000000 smac-2.0.2/smac/facade/algorithm_configuration_facade.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    11605 2023-07-31 15:47:05.000000 smac-2.0.2/smac/facade/blackbox_facade.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2394 2023-07-31 15:47:05.000000 smac-2.0.2/smac/facade/hyperband_facade.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     7578 2023-07-31 15:47:05.000000 smac-2.0.2/smac/facade/hyperparameter_optimization_facade.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     4387 2023-07-31 15:47:05.000000 smac-2.0.2/smac/facade/multi_fidelity_facade.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     5976 2023-07-31 15:47:05.000000 smac-2.0.2/smac/facade/random_facade.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-08-01 13:20:09.881776 smac-2.0.2/smac/initial_design/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      621 2023-07-31 15:47:05.000000 smac-2.0.2/smac/initial_design/__init__.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     8211 2023-07-31 15:47:05.000000 smac-2.0.2/smac/initial_design/abstract_initial_design.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      552 2023-07-31 15:47:05.000000 smac-2.0.2/smac/initial_design/default_design.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2202 2023-07-31 15:47:05.000000 smac-2.0.2/smac/initial_design/factorial_design.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1084 2023-07-31 15:47:05.000000 smac-2.0.2/smac/initial_design/latin_hypercube_design.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      656 2023-07-31 15:47:05.000000 smac-2.0.2/smac/initial_design/random_design.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1671 2023-07-31 15:47:05.000000 smac-2.0.2/smac/initial_design/sobol_design.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-08-01 13:20:09.881776 smac-2.0.2/smac/intensifier/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      341 2023-07-31 15:47:05.000000 smac-2.0.2/smac/intensifier/__init__.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    33241 2023-07-31 15:47:05.000000 smac-2.0.2/smac/intensifier/abstract_intensifier.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2159 2023-07-31 15:47:05.000000 smac-2.0.2/smac/intensifier/hyperband.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    17357 2023-07-31 15:47:05.000000 smac-2.0.2/smac/intensifier/intensifier.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    24527 2023-08-01 13:05:49.000000 smac-2.0.2/smac/intensifier/successive_halving.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      553 2023-07-31 15:47:05.000000 smac-2.0.2/smac/logging.yml
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-08-01 13:20:09.881776 smac-2.0.2/smac/main/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)        0 2023-07-31 15:47:05.000000 smac-2.0.2/smac/main/__init__.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    14855 2023-08-01 13:05:49.000000 smac-2.0.2/smac/main/config_selector.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    24653 2023-08-01 13:05:49.000000 smac-2.0.2/smac/main/smbo.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-08-01 13:20:09.881776 smac-2.0.2/smac/model/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      247 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/__init__.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    11457 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/abstract_model.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-08-01 13:20:09.885776 smac-2.0.2/smac/model/gaussian_process/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      350 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/gaussian_process/__init__.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     6523 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/gaussian_process/abstract_gaussian_process.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    10482 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/gaussian_process/gaussian_process.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    35950 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/gaussian_process/gpytorch_gaussian_process.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-08-01 13:20:09.885776 smac-2.0.2/smac/model/gaussian_process/kernels/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      607 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/gaussian_process/kernels/__init__.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    23169 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/gaussian_process/kernels/_boing.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    17056 2023-08-01 13:05:49.000000 smac-2.0.2/smac/model/gaussian_process/kernels/base_kernels.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3648 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/gaussian_process/kernels/hamming_kernel.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     4121 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/gaussian_process/kernels/matern_kernel.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2738 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/gaussian_process/kernels/rbf_kernel.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1881 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/gaussian_process/kernels/white_kernel.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    16808 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/gaussian_process/mcmc_gaussian_process.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-08-01 13:20:09.885776 smac-2.0.2/smac/model/gaussian_process/priors/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      435 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/gaussian_process/priors/__init__.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     4306 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/gaussian_process/priors/abstract_prior.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2013 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/gaussian_process/priors/gamma_prior.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2402 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/gaussian_process/priors/horseshoe_prior.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1900 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/gaussian_process/priors/log_normal_prior.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     5338 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/gaussian_process/priors/tophat_prior.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3002 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/multi_objective_model.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-08-01 13:20:09.885776 smac-2.0.2/smac/model/random_forest/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      208 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/random_forest/__init__.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1741 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/random_forest/abstract_random_forest.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    10805 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/random_forest/random_forest.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1206 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/random_model.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-08-01 13:20:09.885776 smac-2.0.2/smac/multi_objective/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      333 2023-07-31 15:47:05.000000 smac-2.0.2/smac/multi_objective/__init__.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1038 2023-07-31 15:47:05.000000 smac-2.0.2/smac/multi_objective/abstract_multi_objective_algorithm.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1399 2023-07-31 15:47:05.000000 smac-2.0.2/smac/multi_objective/aggregation_strategy.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1902 2023-07-31 15:47:05.000000 smac-2.0.2/smac/multi_objective/parego.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)        0 2023-03-03 09:52:31.000000 smac-2.0.2/smac/py.typed
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-08-01 13:20:09.885776 smac-2.0.2/smac/random_design/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      585 2023-07-31 15:47:05.000000 smac-2.0.2/smac/random_design/__init__.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1362 2023-07-31 15:47:05.000000 smac-2.0.2/smac/random_design/abstract_random_design.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2691 2023-07-31 15:47:05.000000 smac-2.0.2/smac/random_design/annealing_design.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3489 2023-07-31 15:47:05.000000 smac-2.0.2/smac/random_design/modulus_design.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2439 2023-07-31 15:47:05.000000 smac-2.0.2/smac/random_design/probability_design.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-08-01 13:20:09.885776 smac-2.0.2/smac/runhistory/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      393 2023-07-31 15:47:05.000000 smac-2.0.2/smac/runhistory/__init__.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     4337 2023-07-31 15:47:05.000000 smac-2.0.2/smac/runhistory/dataclasses.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-08-01 13:20:09.885776 smac-2.0.2/smac/runhistory/encoder/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1076 2023-07-31 15:47:05.000000 smac-2.0.2/smac/runhistory/encoder/__init__.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    10551 2023-07-31 15:47:05.000000 smac-2.0.2/smac/runhistory/encoder/abstract_encoder.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2443 2023-07-31 15:47:05.000000 smac-2.0.2/smac/runhistory/encoder/boing_encoder.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2878 2023-07-31 15:47:05.000000 smac-2.0.2/smac/runhistory/encoder/eips_encoder.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2540 2023-07-31 15:47:05.000000 smac-2.0.2/smac/runhistory/encoder/encoder.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1372 2023-07-31 15:47:05.000000 smac-2.0.2/smac/runhistory/encoder/inverse_scaled_encoder.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      867 2023-07-31 15:47:05.000000 smac-2.0.2/smac/runhistory/encoder/log_encoder.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1180 2023-07-31 15:47:05.000000 smac-2.0.2/smac/runhistory/encoder/log_scaled_encoder.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      978 2023-07-31 15:47:05.000000 smac-2.0.2/smac/runhistory/encoder/scaled_encoder.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1354 2023-07-31 15:47:05.000000 smac-2.0.2/smac/runhistory/encoder/sqrt_scaled_encoder.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      356 2023-07-31 15:47:05.000000 smac-2.0.2/smac/runhistory/enumerations.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)       48 2023-07-31 15:47:05.000000 smac-2.0.2/smac/runhistory/errors.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    41527 2023-08-01 13:05:49.000000 smac-2.0.2/smac/runhistory/runhistory.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-08-01 13:20:09.885776 smac-2.0.2/smac/runner/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      472 2023-07-31 15:47:05.000000 smac-2.0.2/smac/runner/__init__.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     9402 2023-07-31 15:47:05.000000 smac-2.0.2/smac/runner/abstract_runner.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1787 2023-07-31 15:47:05.000000 smac-2.0.2/smac/runner/abstract_serial_runner.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     9153 2023-07-31 15:47:05.000000 smac-2.0.2/smac/runner/dask_runner.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      419 2023-07-31 15:47:05.000000 smac-2.0.2/smac/runner/exceptions.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     9356 2023-08-01 13:05:49.000000 smac-2.0.2/smac/runner/target_function_runner.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     7486 2023-07-31 15:47:05.000000 smac-2.0.2/smac/runner/target_function_script_runner.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    10868 2023-07-31 15:47:05.000000 smac-2.0.2/smac/scenario.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-08-01 13:20:09.885776 smac-2.0.2/smac/utils/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)        0 2023-03-03 09:52:31.000000 smac-2.0.2/smac/utils/__init__.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     9299 2023-08-01 13:05:49.000000 smac-2.0.2/smac/utils/configspace.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2276 2023-07-31 15:47:05.000000 smac-2.0.2/smac/utils/data_structures.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1252 2023-07-31 15:47:05.000000 smac-2.0.2/smac/utils/logging.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1167 2023-08-01 13:05:49.000000 smac-2.0.2/smac/utils/multi_objective.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     6018 2023-07-31 15:47:05.000000 smac-2.0.2/smac/utils/pareto_front.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-08-01 13:20:09.885776 smac-2.0.2/smac/utils/subspaces/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    29592 2023-07-31 15:47:05.000000 smac-2.0.2/smac/utils/subspaces/__init__.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     8717 2023-07-31 15:47:05.000000 smac-2.0.2/smac/utils/subspaces/boing_subspace.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    13823 2023-07-31 15:47:05.000000 smac-2.0.2/smac/utils/subspaces/turbo_subspace.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-08-01 13:20:09.881776 smac-2.0.2/smac.egg-info/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     7245 2023-08-01 13:20:09.000000 smac-2.0.2/smac.egg-info/PKG-INFO
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     4513 2023-08-01 13:20:09.000000 smac-2.0.2/smac.egg-info/SOURCES.txt
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)        1 2023-08-01 13:20:09.000000 smac-2.0.2/smac.egg-info/dependency_links.txt
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      324 2023-08-01 13:20:09.000000 smac-2.0.2/smac.egg-info/requires.txt
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)       11 2023-08-01 13:20:09.000000 smac-2.0.2/smac.egg-info/top_level.txt
+drwxr-xr-x   0 helenagraf   (501) staff       (20)        0 2024-05-16 14:07:34.030475 smac-2.1.0/
+-rw-r--r--   0 helenagraf   (501) staff       (20)     3377 2022-12-08 10:26:18.000000 smac-2.1.0/LICENSE.txt
+-rw-r--r--   0 helenagraf   (501) staff       (20)      127 2023-04-12 06:47:10.000000 smac-2.1.0/MANIFEST.in
+-rw-r--r--   0 helenagraf   (501) staff       (20)     7245 2024-05-16 14:07:34.030236 smac-2.1.0/PKG-INFO
+-rw-r--r--   0 helenagraf   (501) staff       (20)     6116 2024-05-07 12:14:09.000000 smac-2.1.0/README.md
+-rw-r--r--   0 helenagraf   (501) staff       (20)     3093 2024-05-16 14:00:56.000000 smac-2.1.0/pyproject.toml
+-rw-r--r--   0 helenagraf   (501) staff       (20)       38 2024-05-16 14:07:34.030537 smac-2.1.0/setup.cfg
+-rw-r--r--   0 helenagraf   (501) staff       (20)     2069 2024-05-16 14:00:56.000000 smac-2.1.0/setup.py
+drwxr-xr-x   0 helenagraf   (501) staff       (20)        0 2024-05-16 14:07:33.998462 smac-2.1.0/smac/
+-rw-r--r--   0 helenagraf   (501) staff       (20)     1555 2024-05-16 14:00:56.000000 smac-2.1.0/smac/__init__.py
+drwxr-xr-x   0 helenagraf   (501) staff       (20)        0 2024-05-16 14:07:33.999910 smac-2.1.0/smac/acquisition/
+-rw-r--r--   0 helenagraf   (501) staff       (20)        0 2023-04-12 06:47:10.000000 smac-2.1.0/smac/acquisition/__init__.py
+drwxr-xr-x   0 helenagraf   (501) staff       (20)        0 2024-05-16 14:07:34.001749 smac-2.1.0/smac/acquisition/function/
+-rw-r--r--   0 helenagraf   (501) staff       (20)      717 2024-05-07 12:14:09.000000 smac-2.1.0/smac/acquisition/function/__init__.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     3552 2024-05-07 12:14:09.000000 smac-2.1.0/smac/acquisition/function/abstract_acquisition_function.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     3086 2024-05-07 12:14:09.000000 smac-2.1.0/smac/acquisition/function/confidence_bound.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     9061 2023-04-12 06:47:10.000000 smac-2.1.0/smac/acquisition/function/expected_improvement.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     4002 2023-04-12 06:47:10.000000 smac-2.1.0/smac/acquisition/function/integrated_acquisition_function.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     9380 2023-04-12 06:47:10.000000 smac-2.1.0/smac/acquisition/function/prior_acqusition_function.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     2692 2023-04-12 06:47:10.000000 smac-2.1.0/smac/acquisition/function/probability_improvement.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     1930 2023-04-12 06:47:10.000000 smac-2.1.0/smac/acquisition/function/thompson.py
+drwxr-xr-x   0 helenagraf   (501) staff       (20)        0 2024-05-16 14:07:34.003611 smac-2.1.0/smac/acquisition/maximizer/
+-rw-r--r--   0 helenagraf   (501) staff       (20)      573 2024-05-16 14:00:56.000000 smac-2.1.0/smac/acquisition/maximizer/__init__.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     6250 2024-05-16 14:00:56.000000 smac-2.1.0/smac/acquisition/maximizer/abstract_acqusition_maximizer.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     2414 2024-05-16 14:00:56.000000 smac-2.1.0/smac/acquisition/maximizer/differential_evolution.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     2911 2024-05-16 14:00:56.000000 smac-2.1.0/smac/acquisition/maximizer/helpers.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     8128 2024-05-16 14:00:56.000000 smac-2.1.0/smac/acquisition/maximizer/local_and_random_search.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)    20001 2024-05-16 14:00:56.000000 smac-2.1.0/smac/acquisition/maximizer/local_search.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     1828 2024-05-14 14:32:47.000000 smac-2.1.0/smac/acquisition/maximizer/random_search.py
+drwxr-xr-x   0 helenagraf   (501) staff       (20)        0 2024-05-16 14:07:34.004409 smac-2.1.0/smac/callback/
+-rw-r--r--   0 helenagraf   (501) staff       (20)      160 2024-05-07 12:14:09.000000 smac-2.1.0/smac/callback/__init__.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     2519 2024-05-07 12:14:09.000000 smac-2.1.0/smac/callback/callback.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     1013 2024-05-07 12:14:09.000000 smac-2.1.0/smac/callback/metadata_callback.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)      270 2023-04-12 06:47:10.000000 smac-2.1.0/smac/constants.py
+drwxr-xr-x   0 helenagraf   (501) staff       (20)        0 2024-05-16 14:07:34.006215 smac-2.1.0/smac/facade/
+-rw-r--r--   0 helenagraf   (501) staff       (20)      674 2023-04-12 06:47:10.000000 smac-2.1.0/smac/facade/__init__.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)    21558 2024-05-16 14:00:56.000000 smac-2.1.0/smac/facade/abstract_facade.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     6276 2024-05-16 14:00:56.000000 smac-2.1.0/smac/facade/algorithm_configuration_facade.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)    12115 2024-05-16 14:00:56.000000 smac-2.1.0/smac/facade/blackbox_facade.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     2394 2024-05-07 12:14:09.000000 smac-2.1.0/smac/facade/hyperband_facade.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     7607 2024-05-16 14:00:56.000000 smac-2.1.0/smac/facade/hyperparameter_optimization_facade.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     4465 2024-05-16 14:00:56.000000 smac-2.1.0/smac/facade/multi_fidelity_facade.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     6053 2024-05-16 14:00:56.000000 smac-2.1.0/smac/facade/random_facade.py
+drwxr-xr-x   0 helenagraf   (501) staff       (20)        0 2024-05-16 14:07:34.007857 smac-2.1.0/smac/initial_design/
+-rw-r--r--   0 helenagraf   (501) staff       (20)      621 2023-04-12 06:47:10.000000 smac-2.1.0/smac/initial_design/__init__.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     8211 2024-05-07 12:14:09.000000 smac-2.1.0/smac/initial_design/abstract_initial_design.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)      552 2023-04-12 07:02:28.000000 smac-2.1.0/smac/initial_design/default_design.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     2202 2023-04-12 07:02:28.000000 smac-2.1.0/smac/initial_design/factorial_design.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     1084 2023-04-12 07:02:28.000000 smac-2.1.0/smac/initial_design/latin_hypercube_design.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)      656 2023-04-12 07:02:28.000000 smac-2.1.0/smac/initial_design/random_design.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     1671 2023-04-12 07:02:28.000000 smac-2.1.0/smac/initial_design/sobol_design.py
+drwxr-xr-x   0 helenagraf   (501) staff       (20)        0 2024-05-16 14:07:34.009427 smac-2.1.0/smac/intensifier/
+-rw-r--r--   0 helenagraf   (501) staff       (20)      341 2023-04-12 06:47:10.000000 smac-2.1.0/smac/intensifier/__init__.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)    33506 2024-05-16 14:00:56.000000 smac-2.1.0/smac/intensifier/abstract_intensifier.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     2159 2024-05-07 12:14:09.000000 smac-2.1.0/smac/intensifier/hyperband.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)    17357 2024-05-07 12:14:09.000000 smac-2.1.0/smac/intensifier/intensifier.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)    24527 2024-05-07 12:14:09.000000 smac-2.1.0/smac/intensifier/successive_halving.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)      553 2023-04-12 06:47:10.000000 smac-2.1.0/smac/logging.yml
+drwxr-xr-x   0 helenagraf   (501) staff       (20)        0 2024-05-16 14:07:34.010291 smac-2.1.0/smac/main/
+-rw-r--r--   0 helenagraf   (501) staff       (20)        0 2023-04-12 06:47:10.000000 smac-2.1.0/smac/main/__init__.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)    14848 2024-05-16 14:00:56.000000 smac-2.1.0/smac/main/config_selector.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)    24653 2024-05-07 12:14:09.000000 smac-2.1.0/smac/main/smbo.py
+drwxr-xr-x   0 helenagraf   (501) staff       (20)        0 2024-05-16 14:07:34.011655 smac-2.1.0/smac/model/
+-rw-r--r--   0 helenagraf   (501) staff       (20)      247 2023-04-12 06:47:10.000000 smac-2.1.0/smac/model/__init__.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)    11457 2024-05-07 12:14:09.000000 smac-2.1.0/smac/model/abstract_model.py
+drwxr-xr-x   0 helenagraf   (501) staff       (20)        0 2024-05-16 14:07:34.013193 smac-2.1.0/smac/model/gaussian_process/
+-rw-r--r--   0 helenagraf   (501) staff       (20)      350 2023-04-12 06:47:10.000000 smac-2.1.0/smac/model/gaussian_process/__init__.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     6523 2023-04-12 06:47:10.000000 smac-2.1.0/smac/model/gaussian_process/abstract_gaussian_process.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)    10482 2023-04-12 06:47:10.000000 smac-2.1.0/smac/model/gaussian_process/gaussian_process.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)    35950 2023-04-12 06:47:10.000000 smac-2.1.0/smac/model/gaussian_process/gpytorch_gaussian_process.py
+drwxr-xr-x   0 helenagraf   (501) staff       (20)        0 2024-05-16 14:07:34.015243 smac-2.1.0/smac/model/gaussian_process/kernels/
+-rw-r--r--   0 helenagraf   (501) staff       (20)      607 2023-04-12 06:47:10.000000 smac-2.1.0/smac/model/gaussian_process/kernels/__init__.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)    23169 2023-04-12 06:47:10.000000 smac-2.1.0/smac/model/gaussian_process/kernels/_boing.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)    17056 2024-05-07 12:14:09.000000 smac-2.1.0/smac/model/gaussian_process/kernels/base_kernels.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     3648 2023-04-12 06:47:10.000000 smac-2.1.0/smac/model/gaussian_process/kernels/hamming_kernel.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     4121 2023-04-12 06:47:10.000000 smac-2.1.0/smac/model/gaussian_process/kernels/matern_kernel.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     2738 2023-04-12 06:47:10.000000 smac-2.1.0/smac/model/gaussian_process/kernels/rbf_kernel.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     1881 2023-04-12 06:47:10.000000 smac-2.1.0/smac/model/gaussian_process/kernels/white_kernel.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)    16808 2023-04-12 06:47:10.000000 smac-2.1.0/smac/model/gaussian_process/mcmc_gaussian_process.py
+drwxr-xr-x   0 helenagraf   (501) staff       (20)        0 2024-05-16 14:07:34.016502 smac-2.1.0/smac/model/gaussian_process/priors/
+-rw-r--r--   0 helenagraf   (501) staff       (20)      435 2023-04-12 06:47:10.000000 smac-2.1.0/smac/model/gaussian_process/priors/__init__.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     4306 2023-04-12 06:47:10.000000 smac-2.1.0/smac/model/gaussian_process/priors/abstract_prior.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     2013 2023-04-12 06:47:10.000000 smac-2.1.0/smac/model/gaussian_process/priors/gamma_prior.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     2402 2023-04-12 06:47:10.000000 smac-2.1.0/smac/model/gaussian_process/priors/horseshoe_prior.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     1900 2023-04-12 06:47:10.000000 smac-2.1.0/smac/model/gaussian_process/priors/log_normal_prior.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     5338 2023-04-12 06:47:10.000000 smac-2.1.0/smac/model/gaussian_process/priors/tophat_prior.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     3002 2023-04-12 06:47:10.000000 smac-2.1.0/smac/model/multi_objective_model.py
+drwxr-xr-x   0 helenagraf   (501) staff       (20)        0 2024-05-16 14:07:34.017223 smac-2.1.0/smac/model/random_forest/
+-rw-r--r--   0 helenagraf   (501) staff       (20)      208 2023-04-12 06:47:10.000000 smac-2.1.0/smac/model/random_forest/__init__.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     1948 2024-05-16 14:00:56.000000 smac-2.1.0/smac/model/random_forest/abstract_random_forest.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)    10870 2024-05-16 14:00:56.000000 smac-2.1.0/smac/model/random_forest/random_forest.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     1206 2023-04-12 06:47:10.000000 smac-2.1.0/smac/model/random_model.py
+drwxr-xr-x   0 helenagraf   (501) staff       (20)        0 2024-05-16 14:07:34.018520 smac-2.1.0/smac/multi_objective/
+-rw-r--r--   0 helenagraf   (501) staff       (20)      333 2023-04-12 06:47:10.000000 smac-2.1.0/smac/multi_objective/__init__.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     1038 2023-04-12 06:47:10.000000 smac-2.1.0/smac/multi_objective/abstract_multi_objective_algorithm.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     1399 2023-04-12 06:47:10.000000 smac-2.1.0/smac/multi_objective/aggregation_strategy.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     1902 2023-04-12 06:47:10.000000 smac-2.1.0/smac/multi_objective/parego.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)        0 2022-12-08 10:26:18.000000 smac-2.1.0/smac/py.typed
+drwxr-xr-x   0 helenagraf   (501) staff       (20)        0 2024-05-16 14:07:34.020089 smac-2.1.0/smac/random_design/
+-rw-r--r--   0 helenagraf   (501) staff       (20)      585 2023-04-12 06:47:10.000000 smac-2.1.0/smac/random_design/__init__.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     1362 2023-04-12 06:47:10.000000 smac-2.1.0/smac/random_design/abstract_random_design.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     2691 2023-04-12 06:47:10.000000 smac-2.1.0/smac/random_design/annealing_design.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     3489 2023-04-12 06:47:10.000000 smac-2.1.0/smac/random_design/modulus_design.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     2439 2023-04-12 06:47:10.000000 smac-2.1.0/smac/random_design/probability_design.py
+drwxr-xr-x   0 helenagraf   (501) staff       (20)        0 2024-05-16 14:07:34.021453 smac-2.1.0/smac/runhistory/
+-rw-r--r--   0 helenagraf   (501) staff       (20)      393 2023-04-12 06:47:10.000000 smac-2.1.0/smac/runhistory/__init__.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     4337 2023-04-12 06:47:10.000000 smac-2.1.0/smac/runhistory/dataclasses.py
+drwxr-xr-x   0 helenagraf   (501) staff       (20)        0 2024-05-16 14:07:34.025338 smac-2.1.0/smac/runhistory/encoder/
+-rw-r--r--   0 helenagraf   (501) staff       (20)     1076 2023-04-12 06:47:10.000000 smac-2.1.0/smac/runhistory/encoder/__init__.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)    10589 2024-05-16 14:00:56.000000 smac-2.1.0/smac/runhistory/encoder/abstract_encoder.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     2443 2023-04-12 06:47:10.000000 smac-2.1.0/smac/runhistory/encoder/boing_encoder.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     2878 2024-05-07 12:14:09.000000 smac-2.1.0/smac/runhistory/encoder/eips_encoder.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     2540 2024-05-07 12:14:09.000000 smac-2.1.0/smac/runhistory/encoder/encoder.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     1372 2023-04-12 06:47:10.000000 smac-2.1.0/smac/runhistory/encoder/inverse_scaled_encoder.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)      867 2024-05-07 12:14:09.000000 smac-2.1.0/smac/runhistory/encoder/log_encoder.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     1180 2024-05-07 12:14:09.000000 smac-2.1.0/smac/runhistory/encoder/log_scaled_encoder.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)      978 2024-05-07 12:14:09.000000 smac-2.1.0/smac/runhistory/encoder/scaled_encoder.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     1354 2024-05-07 12:14:09.000000 smac-2.1.0/smac/runhistory/encoder/sqrt_scaled_encoder.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)      356 2023-04-12 06:47:10.000000 smac-2.1.0/smac/runhistory/enumerations.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)       48 2023-04-12 06:47:10.000000 smac-2.1.0/smac/runhistory/errors.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)    41598 2024-05-16 14:00:56.000000 smac-2.1.0/smac/runhistory/runhistory.py
+drwxr-xr-x   0 helenagraf   (501) staff       (20)        0 2024-05-16 14:07:34.027055 smac-2.1.0/smac/runner/
+-rw-r--r--   0 helenagraf   (501) staff       (20)      472 2023-04-12 06:47:10.000000 smac-2.1.0/smac/runner/__init__.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     9479 2024-05-16 14:00:56.000000 smac-2.1.0/smac/runner/abstract_runner.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     1787 2023-04-12 06:47:10.000000 smac-2.1.0/smac/runner/abstract_serial_runner.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     9158 2024-05-16 14:00:56.000000 smac-2.1.0/smac/runner/dask_runner.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)      419 2023-04-12 06:47:10.000000 smac-2.1.0/smac/runner/exceptions.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     9433 2024-05-16 14:00:56.000000 smac-2.1.0/smac/runner/target_function_runner.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     7563 2024-05-16 14:00:56.000000 smac-2.1.0/smac/runner/target_function_script_runner.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)    10868 2024-05-07 12:14:09.000000 smac-2.1.0/smac/scenario.py
+drwxr-xr-x   0 helenagraf   (501) staff       (20)        0 2024-05-16 14:07:34.028855 smac-2.1.0/smac/utils/
+-rw-r--r--   0 helenagraf   (501) staff       (20)        0 2022-12-08 10:26:18.000000 smac-2.1.0/smac/utils/__init__.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     9299 2024-05-07 12:14:09.000000 smac-2.1.0/smac/utils/configspace.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     2276 2023-04-12 06:47:10.000000 smac-2.1.0/smac/utils/data_structures.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     1252 2023-06-01 12:26:48.000000 smac-2.1.0/smac/utils/logging.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     1167 2024-05-07 12:14:09.000000 smac-2.1.0/smac/utils/multi_objective.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     6018 2023-04-12 06:47:10.000000 smac-2.1.0/smac/utils/pareto_front.py
+drwxr-xr-x   0 helenagraf   (501) staff       (20)        0 2024-05-16 14:07:34.029758 smac-2.1.0/smac/utils/subspaces/
+-rw-r--r--   0 helenagraf   (501) staff       (20)    29592 2023-04-12 06:47:10.000000 smac-2.1.0/smac/utils/subspaces/__init__.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)     8717 2023-04-12 06:47:10.000000 smac-2.1.0/smac/utils/subspaces/boing_subspace.py
+-rw-r--r--   0 helenagraf   (501) staff       (20)    13823 2023-04-12 06:47:10.000000 smac-2.1.0/smac/utils/subspaces/turbo_subspace.py
+drwxr-xr-x   0 helenagraf   (501) staff       (20)        0 2024-05-16 14:07:33.999744 smac-2.1.0/smac.egg-info/
+-rw-r--r--   0 helenagraf   (501) staff       (20)     7245 2024-05-16 14:07:33.000000 smac-2.1.0/smac.egg-info/PKG-INFO
+-rw-r--r--   0 helenagraf   (501) staff       (20)     4513 2024-05-16 14:07:33.000000 smac-2.1.0/smac.egg-info/SOURCES.txt
+-rw-r--r--   0 helenagraf   (501) staff       (20)        1 2024-05-16 14:07:33.000000 smac-2.1.0/smac.egg-info/dependency_links.txt
+-rw-r--r--   0 helenagraf   (501) staff       (20)      331 2024-05-16 14:07:33.000000 smac-2.1.0/smac.egg-info/requires.txt
+-rw-r--r--   0 helenagraf   (501) staff       (20)       11 2024-05-16 14:07:33.000000 smac-2.1.0/smac.egg-info/top_level.txt
```

### Comparing `smac-2.0.2/LICENSE.txt` & `smac-2.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/PKG-INFO` & `smac-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smac
-Version: 2.0.2
+Version: 2.1.0
 Summary: SMAC3, a Python implementation of 'Sequential Model-based Algorithm Configuration'.
 Home-page: https://www.automl.org/
 Author: 	Marius Lindauer, Katharina Eggensperger, Matthias Feurer, André Biedenkapp, Difan Deng,
 	Carolin Benjamins, Tim Ruhkopf, René Sass and Frank Hutter
 Author-email: fh@cs.uni-freiburg.de
 License: BSD 3-Clause License
 Project-URL: Documentation, https://https://github.com/automl.github.io/SMAC3/main
```

### Comparing `smac-2.0.2/README.md` & `smac-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/pyproject.toml` & `smac-2.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -61,14 +61,19 @@
     "D400", # First line should end with a period
     "D401", # First line should be in imperative mood
     "D404", # First word of docstring should not be this
     "D413", # Missing blank line after last section
     "D415", # First line should end with a period, question mark, or exclamation point
 ]
 
+[tool.pylint."messages control"]
+# FIXME: This is to do a staged introduction of pylint checks for just a single class of problems initially (#1067).
+disable = ["all"]
+enable = ["dangerous-default-value"]
+
 [tool.mypy]
 python_version = "3.9"
 show_error_codes = true
 warn_unused_configs = true         # warn about unused [tool.mypy] lines
 follow_imports = "normal"          # Type check top level api code we use from imports
 ignore_missing_imports = true      # prefer explicit ignores
 disallow_untyped_defs = true       # All functions must have types
```

### Comparing `smac-2.0.2/setup.py` & `smac-2.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,14 +34,15 @@
         # Others
         "mypy",
         "isort",
         "black",
         "pydocstyle",
         "flake8",
         "pre-commit",
+        "pylint",
     ],
 }
 
 setuptools.setup(
     name=package_name,
     author=author,
     author_email=author_email,
```

### Comparing `smac-2.0.2/smac/__init__.py` & `smac-2.1.0/smac/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "Documentation": "https://https://github.com/automl.github.io/SMAC3/main",
     "Source Code": "https://github.com/https://github.com/automl/smac",
 }
 copyright = f"""
     Copyright {datetime.date.today().strftime('%Y')}, Marius Lindauer, Katharina Eggensperger,
     Matthias Feurer, André Biedenkapp, Difan Deng, Carolin Benjamins, Tim Ruhkopf, René Sass
     and Frank Hutter"""
-version = "2.0.2"
+version = "2.1.0"
 
 
 try:
     from smac.callback.callback import Callback
     from smac.facade import (
         AlgorithmConfigurationFacade,
         BlackBoxFacade,
```

### Comparing `smac-2.0.2/smac/acquisition/function/__init__.py` & `smac-2.1.0/smac/acquisition/function/__init__.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/acquisition/function/abstract_acquisition_function.py` & `smac-2.1.0/smac/acquisition/function/abstract_acquisition_function.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/acquisition/function/confidence_bound.py` & `smac-2.1.0/smac/acquisition/function/confidence_bound.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/acquisition/function/expected_improvement.py` & `smac-2.1.0/smac/acquisition/function/expected_improvement.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/acquisition/function/integrated_acquisition_function.py` & `smac-2.1.0/smac/acquisition/function/integrated_acquisition_function.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/acquisition/function/prior_acqusition_function.py` & `smac-2.1.0/smac/acquisition/function/prior_acqusition_function.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/acquisition/function/probability_improvement.py` & `smac-2.1.0/smac/acquisition/function/probability_improvement.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/acquisition/function/thompson.py` & `smac-2.1.0/smac/acquisition/function/thompson.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/acquisition/maximizer/abstract_acqusition_maximizer.py` & `smac-2.1.0/smac/acquisition/maximizer/abstract_acqusition_maximizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,20 +23,17 @@
     """Abstract class for the acquisition maximization.
 
     In order to use this class it has to be subclassed and the
     method `_maximize` must be implemented.
 
     Parameters
     ----------
-    configspace : ConfigurationSpace
-    acquisition_function : AbstractAcquisitionFunction
-    challengers : int, defaults to 5000
-        Number of configurations to sample from the configuration space to get
-        the acquisition function value for, thus challenging the current
-        incumbent and becoming a candidate for the next function evaluation.
+    configspace : ConfigurationSpace acquisition_function : AbstractAcquisitionFunction
+    challengers : int, defaults to 5000 Number of configurations sampled during the optimization process,
+    details depend on the used maximizer. Also, the number of configurations that is returned by calling `maximize`.
     seed : int, defaults to 0
     """
 
     def __init__(
         self,
         configspace: ConfigurationSpace,
         acquisition_function: AbstractAcquisitionFunction | None = None,
@@ -81,16 +78,16 @@
         """Maximize acquisition function using `_maximize`, implemented by a subclass.
 
         Parameters
         ----------
         previous_configs: list[Configuration]
             Previous evaluated configurations.
         n_points: int, defaults to None
-            Number of points to be sampled. If `n_points` is not specified,
-            `self._challengers` is used.
+            Number of points to be sampled & number of configurations to be returned. If `n_points` is not specified,
+            `self._challengers` is used. Semantics depend on concrete implementation.
         random_design: AbstractRandomDesign, defaults to None
             Part of the returned ChallengerList such that we can interleave random configurations
             by a scheme defined by the random design. The method `random_design.next_iteration()`
             is called at the end of this function.
 
         Returns
         -------
```

### Comparing `smac-2.0.2/smac/acquisition/maximizer/differential_evolution.py` & `smac-2.1.0/smac/acquisition/maximizer/differential_evolution.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     """
 
     def _maximize(
         self,
         previous_configs: list[Configuration],
         n_points: int,
     ) -> list[tuple[float, Configuration]]:
+        # n_points is not used here, but is required by the interface
 
         configs: list[tuple[float, Configuration]] = []
 
         def func(x: np.ndarray) -> np.ndarray:
             assert self._acquisition_function is not None
             return -self._acquisition_function([Configuration(self._configspace, vector=x)])
```

### Comparing `smac-2.0.2/smac/acquisition/maximizer/helpers.py` & `smac-2.1.0/smac/acquisition/maximizer/helpers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 from __future__ import annotations
 
 from typing import Callable, Iterator
 
 from ConfigSpace import Configuration, ConfigurationSpace
 
+from smac.random_design import ProbabilityRandomDesign
 from smac.random_design.abstract_random_design import AbstractRandomDesign
-from smac.random_design.modulus_design import ModulusRandomDesign
 
 
 class ChallengerList(Iterator):
     """Helper class to interleave random configurations in a list of challengers.
 
     Provides an iterator which returns a random configuration in each second
     iteration. Reduces time necessary to generate a list of new challengers
     as one does not need to sample several hundreds of random configurations
     in each iteration which are never looked at.
 
     Parameters
     ----------
     configspace : ConfigurationSpace
     challenger_callback : Callable
-        Callback function which returns a list of challengers (without interleaved random configurations, must a be a
+        Callback function which returns a list of challengers (without interleaved random configurations), must a be a
         python closure.
     random_design : AbstractRandomDesign | None, defaults to ModulusRandomDesign(modulus=2.0)
         Which random design should be used.
     """
 
     def __init__(
         self,
         configspace: ConfigurationSpace,
         challenger_callback: Callable,
-        random_design: AbstractRandomDesign | None = ModulusRandomDesign(modulus=2.0),
+        random_design: AbstractRandomDesign | None = ProbabilityRandomDesign(seed=0, probability=0.08447232371720552),
     ):
         self._challengers_callback = challenger_callback
         self._challengers: list[Configuration] | None = None
         self._configspace = configspace
         self._index = 0
         self._iteration = 1  # 1-based to prevent from starting with a random configuration
         self._random_design = random_design
@@ -68,48 +68,7 @@
             return config
 
     def __len__(self) -> int:
         if self._challengers is None:
             self._challengers = self._challengers_callback()
 
         return len(self._challengers) - self._index
-
-
-'''
-class FixedSet(AbstractAcquisitionMaximizer):
-    def __init__(
-        self,
-        configurations: list[Configuration],
-        acquisition_function: AbstractAcquisitionFunction,
-        configspace: ConfigurationSpace,
-        challengers: int = 5000,
-        seed: int = 0,
-    ):
-        """Maximize the acquisition function over a finite list of configurations.
-
-        Parameters
-        ----------
-        configurations : list[~smac._configspace.Configuration]
-            Candidate configurations
-        acquisition_function : ~smac.acquisition.AbstractAcquisitionFunction
-
-        configspace : ~smac._configspace.ConfigurationSpace
-
-        rng : np.random.RandomState or int, optional
-        """
-        super().__init__(
-            acquisition_function=acquisition_function, configspace=configspace, challengers=challengers, seed=seed
-        )
-        self.configurations = configurations
-
-    def _maximize(
-        self,
-        runhistory: RunHistory,
-        stats: Stats,
-        n_points: int,
-    ) -> list[tuple[float, Configuration]]:
-        configurations = copy.deepcopy(self.configurations)
-        for config in configurations:
-            config.origin = "Fixed Set"
-
-        return self._sort_by_acquisition_value(configurations)
-'''
```

### Comparing `smac-2.0.2/smac/acquisition/maximizer/local_search.py` & `smac-2.1.0/smac/acquisition/maximizer/local_search.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,17 +86,17 @@
 
     def _maximize(
         self,
         previous_configs: list[Configuration],
         n_points: int,
         additional_start_points: list[tuple[float, Configuration]] | None = None,
     ) -> list[tuple[float, Configuration]]:
-        """Start a local search from the given startpoints. Iteratively collect neighbours
+        """Start a local search from the given start points. Iteratively collect neighbours
         using Configspace.utils.get_one_exchange_neighbourhood and evaluate them.
-        If the new config is better than the current best, the local search is coninued from the
+        If the new config is better than the current best, the local search is continued from the
         new config.
 
         Quit if either the max number of steps is reached or
         no neighbor with a higher improvement was found or the number of local steps self._n_steps_plateau_walk
         for each of the starting point is depleted.
 
 
@@ -145,24 +145,30 @@
             Additional starting points.
 
         Returns
         -------
         list[Configuration]
             A list of initial points/configurations.
         """
-        if len(previous_configs) == 0:
-            init_points = self._configspace.sample_configuration(size=n_points)
-        else:
+        sampled_points = []
+        init_points = []
+        n_init_points = n_points
+        if len(previous_configs) < n_points:
+            sampled_points = self._configspace.sample_configuration(size=n_points - len(previous_configs))
+            n_init_points = len(previous_configs)
+            if not isinstance(sampled_points, list):
+                sampled_points = [sampled_points]
+        if len(previous_configs) > 0:
             init_points = self._get_init_points_from_previous_configs(
                 previous_configs,
-                n_points,
+                n_init_points,
                 additional_start_points,
             )
 
-        return init_points
+        return sampled_points + init_points
 
     def _get_init_points_from_previous_configs(
         self,
         previous_configs: list[Configuration],
         n_points: int,
         additional_start_points: list[tuple[float, Configuration]] | None,
     ) -> list[Configuration]:
@@ -183,29 +189,25 @@
         are dropped.
 
         Parameters
         ----------
         previous_configs: list[Configuration]
             Previous configuration (e.g., from the runhistory).
         n_points: int
-            Number of initial points to be generated.
+            Number of initial points to be generated; selected from previous configs (+ random configs if necessary).
         additional_start_points: list[tuple[float, Configuration]] | None
             Additional starting points.
 
         Returns
         -------
         init_points: list[Configuration]
             A list of initial points.
         """
         assert self._acquisition_function is not None
 
-        # configurations with the highest previous EI
-        configs_previous_runs_sorted = self._sort_by_acquisition_value(previous_configs)
-        configs_previous_runs_sorted = [conf[1] for conf in configs_previous_runs_sorted[:n_points]]
-
         # configurations with the lowest predictive cost, check for None to make unit tests work
         if self._acquisition_function.model is not None:
             conf_array = convert_configurations_to_array(previous_configs)
             costs = self._acquisition_function.model.predict_marginalized(conf_array)[0]
             assert len(conf_array) == len(costs), (conf_array.shape, costs.shape)
 
             # In case of the predictive model returning the prediction for more than one objective per configuration
@@ -224,22 +226,21 @@
             # Cannot use zip here because the indices array cannot index the
             # rand_configs list, because the second is a pure python list
             previous_configs_sorted_by_cost = [previous_configs[ind] for ind in indices][:n_points]
         else:
             previous_configs_sorted_by_cost = []
 
         if additional_start_points is not None:
-            additional_start_points = [asp[1] for asp in additional_start_points[:n_points]]
+            additional_start_points = [asp[1] for asp in additional_start_points]
         else:
             additional_start_points = []
 
         init_points = []
         init_points_as_set: set[Configuration] = set()
         for cand in itertools.chain(
-            configs_previous_runs_sorted,
             previous_configs_sorted_by_cost,
             additional_start_points,
         ):
             if cand not in init_points_as_set:
                 init_points.append(cand)
                 init_points_as_set.add(cand)
```

### Comparing `smac-2.0.2/smac/acquisition/maximizer/random_search.py` & `smac-2.1.0/smac/acquisition/maximizer/random_search.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/callback/callback.py` & `smac-2.1.0/smac/callback/callback.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/callback/metadata_callback.py` & `smac-2.1.0/smac/callback/metadata_callback.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/facade/__init__.py` & `smac-2.1.0/smac/facade/__init__.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/facade/abstract_facade.py` & `smac-2.1.0/smac/facade/abstract_facade.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,20 +113,23 @@
         initial_design: AbstractInitialDesign | None = None,
         random_design: AbstractRandomDesign | None = None,
         intensifier: AbstractIntensifier | None = None,
         multi_objective_algorithm: AbstractMultiObjectiveAlgorithm | None = None,
         runhistory_encoder: AbstractRunHistoryEncoder | None = None,
         config_selector: ConfigSelector | None = None,
         logging_level: int | Path | Literal[False] | None = None,
-        callbacks: list[Callback] = [],
+        callbacks: list[Callback] = None,
         overwrite: bool = False,
         dask_client: Client | None = None,
     ):
         setup_logging(logging_level)
 
+        if callbacks is None:
+            callbacks = []
+
         if model is None:
             model = self.get_model(scenario)
 
         if acquisition_function is None:
             acquisition_function = self.get_acquisition_function(scenario)
 
         if acquisition_maximizer is None:
@@ -186,15 +189,15 @@
                 scenario=scenario,
                 target_function=target_function,
                 required_arguments=self._get_signature_arguments(),
             )
 
         # In case of multiple jobs, we need to wrap the runner again using DaskParallelRunner
         if (n_workers := scenario.n_workers) > 1 or dask_client is not None:
-            if dask_client is not None:
+            if dask_client is not None and n_workers > 1:
                 logger.warning(
                     "Provided `dask_client`. Ignore `scenario.n_workers`, directly set `n_workers` in `dask_client`."
                 )
             else:
                 available_workers = joblib.cpu_count()
                 if n_workers > available_workers:
                     logger.info(f"Workers are reduced to {n_workers}.")
```

### Comparing `smac-2.0.2/smac/facade/algorithm_configuration_facade.py` & `smac-2.1.0/smac/facade/algorithm_configuration_facade.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,23 +121,25 @@
             max_incumbents=max_incumbents,
         )
 
     @staticmethod
     def get_initial_design(  # type: ignore
         scenario: Scenario,
         *,
-        additional_configs: list[Configuration] = [],
+        additional_configs: list[Configuration] = None,
     ) -> DefaultInitialDesign:
         """Returns an initial design, which returns the default configuration.
 
         Parameters
         ----------
         additional_configs: list[Configuration], defaults to []
             Adds additional configurations to the initial design.
         """
+        if additional_configs is None:
+            additional_configs = []
         return DefaultInitialDesign(
             scenario=scenario,
             additional_configs=additional_configs,
         )
 
     @staticmethod
     def get_random_design(  # type: ignore
```

### Comparing `smac-2.0.2/smac/facade/blackbox_facade.py` & `smac-2.1.0/smac/facade/blackbox_facade.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from smac.acquisition.function.expected_improvement import EI
 from smac.acquisition.maximizer.local_and_random_search import (
     LocalAndSortedRandomSearch,
 )
 from smac.facade.abstract_facade import AbstractFacade
 from smac.initial_design.sobol_design import SobolInitialDesign
 from smac.intensifier.intensifier import Intensifier
+from smac.main.config_selector import ConfigSelector
 from smac.model.gaussian_process.abstract_gaussian_process import (
     AbstractGaussianProcess,
 )
 from smac.model.gaussian_process.gaussian_process import GaussianProcess
 from smac.model.gaussian_process.kernels import (
     ConstantKernel,
     HammingKernel,
@@ -236,15 +237,15 @@
     @staticmethod
     def get_initial_design(  # type: ignore
         scenario: Scenario,
         *,
         n_configs: int | None = None,
         n_configs_per_hyperparamter: int = 8,
         max_ratio: float = 0.25,
-        additional_configs: list[Configuration] = [],
+        additional_configs: list[Configuration] = None,
     ) -> SobolInitialDesign:
         """Returns a Sobol design instance.
 
         Parameters
         ----------
         scenario : Scenario
         n_configs : int | None, defaults to None
@@ -255,14 +256,16 @@
             samples.
         max_ratio: float, defaults to 0.25
             Use at most ``scenario.n_trials`` * ``max_ratio`` number of configurations in the initial design.
             Additional configurations are not affected by this parameter.
         additional_configs: list[Configuration], defaults to []
             Adds additional configurations to the initial design.
         """
+        if additional_configs is None:
+            additional_configs = []
         return SobolInitialDesign(
             scenario=scenario,
             n_configs=n_configs,
             n_configs_per_hyperparameter=n_configs_per_hyperparamter,
             max_ratio=max_ratio,
             additional_configs=additional_configs,
             seed=scenario.seed,
@@ -305,7 +308,19 @@
 
     @staticmethod
     def get_runhistory_encoder(
         scenario: Scenario,
     ) -> RunHistoryEncoder:
         """Returns the default runhistory encoder."""
         return RunHistoryEncoder(scenario)
+
+    @staticmethod
+    def get_config_selector(
+        scenario: Scenario,
+        *,
+        retrain_after: int = 1,
+        retries: int = 16,
+    ) -> ConfigSelector:
+        """Returns the default configuration selector."""
+        return super(BlackBoxFacade, BlackBoxFacade).get_config_selector(
+            scenario, retrain_after=retrain_after, retries=retries
+        )
```

### Comparing `smac-2.0.2/smac/facade/hyperband_facade.py` & `smac-2.1.0/smac/facade/hyperband_facade.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/facade/hyperparameter_optimization_facade.py` & `smac-2.1.0/smac/facade/hyperparameter_optimization_facade.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,15 +134,15 @@
     @staticmethod
     def get_initial_design(  # type: ignore
         scenario: Scenario,
         *,
         n_configs: int | None = None,
         n_configs_per_hyperparamter: int = 10,
         max_ratio: float = 0.25,
-        additional_configs: list[Configuration] = [],
+        additional_configs: list[Configuration] | None = None,
     ) -> SobolInitialDesign:
         """Returns a Sobol design instance.
 
         Parameters
         ----------
         scenario : Scenario
         n_configs : int | None, defaults to None
@@ -174,15 +174,15 @@
         """Returns ``ProbabilityRandomDesign`` for interleaving configurations.
 
         Parameters
         ----------
         probability : float, defaults to 0.2
             Probability that a configuration will be drawn at random.
         """
-        return ProbabilityRandomDesign(probability=probability)
+        return ProbabilityRandomDesign(probability=probability, seed=scenario.seed)
 
     @staticmethod
     def get_multi_objective_algorithm(  # type: ignore
         scenario: Scenario,
         *,
         objective_weights: list[float] | None = None,
     ) -> MeanAggregationStrategy:
```

### Comparing `smac-2.0.2/smac/facade/multi_fidelity_facade.py` & `smac-2.1.0/smac/facade/multi_fidelity_facade.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,33 +63,35 @@
     @staticmethod
     def get_initial_design(  # type: ignore
         scenario: Scenario,
         *,
         n_configs: int | None = None,
         n_configs_per_hyperparamter: int = 10,
         max_ratio: float = 0.25,
-        additional_configs: list[Configuration] = [],
+        additional_configs: list[Configuration] = None,
     ) -> RandomInitialDesign:
         """Returns a random initial design.
 
         Parameters
         ----------
         scenario : Scenario
         n_configs : int | None, defaults to None
             Number of initial configurations (disables the arguments ``n_configs_per_hyperparameter``).
         n_configs_per_hyperparameter: int, defaults to 10
             Number of initial configurations per hyperparameter. For example, if my configuration space covers five
             hyperparameters and ``n_configs_per_hyperparameter`` is set to 10, then 50 initial configurations will be
             samples.
-        max_ratio: float, defaults to 0.1
+        max_ratio: float, defaults to 0.25
             Use at most ``scenario.n_trials`` * ``max_ratio`` number of configurations in the initial design.
             Additional configurations are not affected by this parameter.
         additional_configs: list[Configuration], defaults to []
             Adds additional configurations to the initial design.
         """
+        if additional_configs is None:
+            additional_configs = []
         return RandomInitialDesign(
             scenario=scenario,
             n_configs=n_configs,
             n_configs_per_hyperparameter=n_configs_per_hyperparamter,
             max_ratio=max_ratio,
             additional_configs=additional_configs,
         )
```

### Comparing `smac-2.0.2/smac/facade/random_facade.py` & `smac-2.1.0/smac/facade/random_facade.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,23 +88,25 @@
             max_incumbents=max_incumbents,
         )
 
     @staticmethod
     def get_initial_design(
         scenario: Scenario,
         *,
-        additional_configs: list[Configuration] = [],
+        additional_configs: list[Configuration] = None,
     ) -> DefaultInitialDesign:
         """Returns an initial design, which returns the default configuration.
 
         Parameters
         ----------
         additional_configs: list[Configuration], defaults to []
             Adds additional configurations to the initial design.
         """
+        if additional_configs is None:
+            additional_configs = []
         return DefaultInitialDesign(
             scenario=scenario,
             additional_configs=additional_configs,
         )
 
     @staticmethod
     def get_random_design(scenario: Scenario) -> AbstractRandomDesign:
```

### Comparing `smac-2.0.2/smac/initial_design/__init__.py` & `smac-2.1.0/smac/initial_design/__init__.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/initial_design/abstract_initial_design.py` & `smac-2.1.0/smac/initial_design/abstract_initial_design.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/initial_design/default_design.py` & `smac-2.1.0/smac/initial_design/default_design.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/initial_design/factorial_design.py` & `smac-2.1.0/smac/initial_design/factorial_design.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/initial_design/latin_hypercube_design.py` & `smac-2.1.0/smac/initial_design/latin_hypercube_design.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/initial_design/random_design.py` & `smac-2.1.0/smac/initial_design/random_design.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/initial_design/sobol_design.py` & `smac-2.1.0/smac/initial_design/sobol_design.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/intensifier/abstract_intensifier.py` & `smac-2.1.0/smac/intensifier/abstract_intensifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -567,16 +567,20 @@
 
         # We compare the incumbents now and only return the ones on the pareto front
         new_incumbents = calculate_pareto_front(rh, incumbents, all_incumbent_isb_keys)
         new_incumbent_ids = [rh.get_config_id(c) for c in new_incumbents]
 
         if len(previous_incumbents) == len(new_incumbents):
             if previous_incumbents == new_incumbents:
-                # No changes in the incumbents
-                self._remove_rejected_config(config_id)
+                # No changes in the incumbents, we need this clause because we can't use set difference then
+                if config_id in new_incumbent_ids:
+                    self._remove_rejected_config(config_id)
+                else:
+                    # config worse than incumbents and thus rejected
+                    self._add_rejected_config(config_id)
                 return
             else:
                 # In this case, we have to determine which config replaced which incumbent and reject it
                 removed_incumbent_id = list(set(previous_incumbent_ids) - set(new_incumbent_ids))[0]
                 removed_incumbent_hash = get_config_hash(rh.get_config(removed_incumbent_id))
                 self._add_rejected_config(removed_incumbent_id)
```

### Comparing `smac-2.0.2/smac/intensifier/hyperband.py` & `smac-2.1.0/smac/intensifier/hyperband.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/intensifier/intensifier.py` & `smac-2.1.0/smac/intensifier/intensifier.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/intensifier/successive_halving.py` & `smac-2.1.0/smac/intensifier/successive_halving.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/logging.yml` & `smac-2.1.0/smac/logging.yml`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/main/config_selector.py` & `smac-2.1.0/smac/main/config_selector.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,23 +87,23 @@
         initial_design: AbstractInitialDesign,
         runhistory: RunHistory,
         runhistory_encoder: AbstractRunHistoryEncoder,
         model: AbstractModel,
         acquisition_maximizer: AbstractAcquisitionMaximizer,
         acquisition_function: AbstractAcquisitionFunction,
         random_design: AbstractRandomDesign,
-        callbacks: list[Callback] = [],
+        callbacks: list[Callback] = None,
     ) -> None:
         self._runhistory = runhistory
         self._runhistory_encoder = runhistory_encoder
         self._model = model
         self._acquisition_maximizer = acquisition_maximizer
         self._acquisition_function = acquisition_function
         self._random_design = random_design
-        self._callbacks = callbacks
+        self._callbacks = callbacks if callbacks is not None else []
 
         self._initial_design_configs = initial_design.select_configurations()
         if len(self._initial_design_configs) == 0:
             raise RuntimeError("SMAC needs initial configurations to work.")
 
     @property
     def meta(self) -> dict[str, Any]:
@@ -209,15 +209,14 @@
             # We want to cache how many entries we used because if we have the same number of entries
             # we don't need to train the next time
             self._previous_entries = Y.shape[0]
 
             # Now we maximize the acquisition function
             challengers = self._acquisition_maximizer.maximize(
                 previous_configs,
-                n_points=self._retrain_after,
                 random_design=self._random_design,
             )
 
             counter = 0
             failed_counter = 0
             for config in challengers:
                 if config not in self._processed_configs:
@@ -278,15 +277,15 @@
         # Get #points per budget and if there are enough samples, then build a model
         for b in available_budgets:
             X, Y = self._runhistory_encoder.transform(budget_subset=[b])
 
             if X.shape[0] >= self._min_trials:
                 self._considered_budgets = [b]
 
-                # TODO: Add running configs
+                # Possible add running configs?
                 configs_array = self._runhistory_encoder.get_configurations(budget_subset=self._considered_budgets)
 
                 return X, Y, configs_array
 
         return (
             np.empty(shape=[0, 0]),
             np.empty(
```

### Comparing `smac-2.0.2/smac/main/smbo.py` & `smac-2.1.0/smac/main/smbo.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/model/abstract_model.py` & `smac-2.1.0/smac/model/abstract_model.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/model/gaussian_process/abstract_gaussian_process.py` & `smac-2.1.0/smac/model/gaussian_process/abstract_gaussian_process.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/model/gaussian_process/gaussian_process.py` & `smac-2.1.0/smac/model/gaussian_process/gaussian_process.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/model/gaussian_process/gpytorch_gaussian_process.py` & `smac-2.1.0/smac/model/gaussian_process/gpytorch_gaussian_process.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/model/gaussian_process/kernels/__init__.py` & `smac-2.1.0/smac/model/gaussian_process/kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/model/gaussian_process/kernels/_boing.py` & `smac-2.1.0/smac/model/gaussian_process/kernels/_boing.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/model/gaussian_process/kernels/base_kernels.py` & `smac-2.1.0/smac/model/gaussian_process/kernels/base_kernels.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/model/gaussian_process/kernels/hamming_kernel.py` & `smac-2.1.0/smac/model/gaussian_process/kernels/hamming_kernel.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/model/gaussian_process/kernels/matern_kernel.py` & `smac-2.1.0/smac/model/gaussian_process/kernels/matern_kernel.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/model/gaussian_process/kernels/rbf_kernel.py` & `smac-2.1.0/smac/model/gaussian_process/kernels/rbf_kernel.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/model/gaussian_process/kernels/white_kernel.py` & `smac-2.1.0/smac/model/gaussian_process/kernels/white_kernel.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/model/gaussian_process/mcmc_gaussian_process.py` & `smac-2.1.0/smac/model/gaussian_process/mcmc_gaussian_process.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/model/gaussian_process/priors/abstract_prior.py` & `smac-2.1.0/smac/model/gaussian_process/priors/abstract_prior.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/model/gaussian_process/priors/gamma_prior.py` & `smac-2.1.0/smac/model/gaussian_process/priors/gamma_prior.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/model/gaussian_process/priors/horseshoe_prior.py` & `smac-2.1.0/smac/model/gaussian_process/priors/horseshoe_prior.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/model/gaussian_process/priors/log_normal_prior.py` & `smac-2.1.0/smac/model/gaussian_process/priors/log_normal_prior.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/model/gaussian_process/priors/tophat_prior.py` & `smac-2.1.0/smac/model/gaussian_process/priors/tophat_prior.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/model/multi_objective_model.py` & `smac-2.1.0/smac/model/multi_objective_model.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/model/random_forest/random_forest.py` & `smac-2.1.0/smac/model/random_forest/random_forest.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,17 @@
         self._rf_opts.tree_opts.min_samples_in_leaf = min_samples_leaf
         self._rf_opts.tree_opts.max_depth = max_depth
         self._rf_opts.tree_opts.epsilon_purity = eps_purity
         self._rf_opts.tree_opts.max_num_nodes = max_nodes
         self._rf_opts.compute_law_of_total_variance = False
         self._rf: BinaryForest | None = None
         self._log_y = log_y
-        self._rng = regression.default_random_engine(seed)
+
+        # Case to `int` incase we get an `np.integer` type
+        self._rng = regression.default_random_engine(int(seed))
 
         self._n_trees = n_trees
         self._n_points_per_tree = n_points_per_tree
         self._ratio_features = ratio_features
         self._min_samples_split = min_samples_split
         self._min_samples_leaf = min_samples_leaf
         self._max_depth = max_depth
```

### Comparing `smac-2.0.2/smac/model/random_model.py` & `smac-2.1.0/smac/model/random_model.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/multi_objective/abstract_multi_objective_algorithm.py` & `smac-2.1.0/smac/multi_objective/abstract_multi_objective_algorithm.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/multi_objective/aggregation_strategy.py` & `smac-2.1.0/smac/multi_objective/aggregation_strategy.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/multi_objective/parego.py` & `smac-2.1.0/smac/multi_objective/parego.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/random_design/__init__.py` & `smac-2.1.0/smac/random_design/__init__.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/random_design/abstract_random_design.py` & `smac-2.1.0/smac/random_design/abstract_random_design.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/random_design/annealing_design.py` & `smac-2.1.0/smac/random_design/annealing_design.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/random_design/modulus_design.py` & `smac-2.1.0/smac/random_design/modulus_design.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/random_design/probability_design.py` & `smac-2.1.0/smac/random_design/probability_design.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/runhistory/dataclasses.py` & `smac-2.1.0/smac/runhistory/dataclasses.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/runhistory/encoder/__init__.py` & `smac-2.1.0/smac/runhistory/encoder/__init__.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/runhistory/encoder/abstract_encoder.py` & `smac-2.1.0/smac/runhistory/encoder/abstract_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,35 +38,35 @@
     TypeError
         If no success states are given.
     """
 
     def __init__(
         self,
         scenario: Scenario,
-        considered_states: list[StatusType] = [
-            StatusType.SUCCESS,
-            StatusType.CRASHED,
-            StatusType.MEMORYOUT,
-        ],
-        lower_budget_states: list[StatusType] = [],
+        considered_states: list[StatusType] = None,
+        lower_budget_states: list[StatusType] = None,
         scale_percentage: int = 5,
         seed: int | None = None,
     ) -> None:
         if considered_states is None:
-            raise TypeError("No success states are given.")
+            considered_states = [
+                StatusType.SUCCESS,
+                StatusType.CRASHED,
+                StatusType.MEMORYOUT,
+            ]
 
         if seed is None:
             seed = scenario.seed
 
         self._seed = seed
         self._rng = np.random.RandomState(seed)
         self._scale_percentage = scale_percentage
         self._n_objectives = scenario.count_objectives()
         self._algorithm_walltime_limit = scenario.trial_walltime_limit
-        self._lower_budget_states = lower_budget_states
+        self._lower_budget_states = lower_budget_states if lower_budget_states is not None else []
         self._considered_states = considered_states
 
         self._instances = scenario.instances
         self._instance_features = scenario.instance_features
         self._n_features = scenario.count_instance_features()
         self._n_params = len(scenario.configspace.get_hyperparameters())
```

### Comparing `smac-2.0.2/smac/runhistory/encoder/boing_encoder.py` & `smac-2.1.0/smac/runhistory/encoder/boing_encoder.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/runhistory/encoder/eips_encoder.py` & `smac-2.1.0/smac/runhistory/encoder/eips_encoder.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/runhistory/encoder/encoder.py` & `smac-2.1.0/smac/runhistory/encoder/encoder.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/runhistory/encoder/inverse_scaled_encoder.py` & `smac-2.1.0/smac/runhistory/encoder/inverse_scaled_encoder.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/runhistory/encoder/log_encoder.py` & `smac-2.1.0/smac/runhistory/encoder/log_encoder.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/runhistory/encoder/log_scaled_encoder.py` & `smac-2.1.0/smac/runhistory/encoder/log_scaled_encoder.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/runhistory/encoder/scaled_encoder.py` & `smac-2.1.0/smac/runhistory/encoder/scaled_encoder.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/runhistory/encoder/sqrt_scaled_encoder.py` & `smac-2.1.0/smac/runhistory/encoder/sqrt_scaled_encoder.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/runhistory/runhistory.py` & `smac-2.1.0/smac/runhistory/runhistory.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,15 +174,15 @@
         time: float = 0.0,
         status: StatusType = StatusType.SUCCESS,
         instance: str | None = None,
         seed: int | None = None,
         budget: float | None = None,
         starttime: float = 0.0,
         endtime: float = 0.0,
-        additional_info: dict[str, Any] = {},
+        additional_info: dict[str, Any] = None,
         force_update: bool = False,
     ) -> None:
         """Adds a new trial to the RunHistory.
 
         Parameters
         ----------
         config : Configuration
@@ -201,14 +201,16 @@
         force_update : bool, defaults to false
             Overwrites a previous trial if the trial already exists.
         """
         if config is None:
             raise TypeError("Configuration must not be None.")
         elif not isinstance(config, Configuration):
             raise TypeError("Configuration is not of type Configuration, but %s." % type(config))
+        if additional_info is None:
+            additional_info = {}
 
         # Squeeze is important to reduce arrays with one element
         # to scalars.
         cost_array = np.asarray(cost).squeeze()
         n_objectives = np.size(cost_array)
 
         # Get the config id
```

### Comparing `smac-2.0.2/smac/runner/abstract_runner.py` & `smac-2.1.0/smac/runner/abstract_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,16 +46,18 @@
     required_arguments : list[str]
         A list of required arguments, which are passed to the target function.
     """
 
     def __init__(
         self,
         scenario: Scenario,
-        required_arguments: list[str] = [],
+        required_arguments: list[str] = None,
     ):
+        if required_arguments is None:
+            required_arguments = []
         self._scenario = scenario
         self._required_arguments = required_arguments
 
         # The results are a FIFO structure, implemented via a list
         # (because the Queue lock is not pickable). Finished runs are
         # put in this list and collected via _process_pending_runs
         self._results_queue: list[tuple[TrialInfo, TrialValue]] = []
```

### Comparing `smac-2.0.2/smac/runner/abstract_serial_runner.py` & `smac-2.1.0/smac/runner/abstract_serial_runner.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/runner/dask_runner.py` & `smac-2.1.0/smac/runner/dask_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
                 n_workers=self._scenario.n_workers,
                 processes=True,
                 threads_per_worker=1,
                 local_directory=str(self._scenario.output_directory),
             )
 
             if self._scenario.output_directory is not None:
-                self._scheduler_file = self._scenario.output_directory / ".dask_scheduler_file"
+                self._scheduler_file = Path(self._scenario.output_directory, ".dask_scheduler_file")
                 self._client.write_scheduler_file(scheduler_file=str(self._scheduler_file))
         else:
             # We just use their set up
             self._client = dask_client
             self._close_client_at_del = False
 
     def submit_trial(self, trial_info: TrialInfo, **dask_data_to_scatter: dict[str, Any]) -> None:
```

### Comparing `smac-2.0.2/smac/runner/target_function_runner.py` & `smac-2.1.0/smac/runner/target_function_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,16 +41,18 @@
         A list of required arguments, which are passed to the target function.
     """
 
     def __init__(
         self,
         scenario: Scenario,
         target_function: Callable,
-        required_arguments: list[str] = [],
+        required_arguments: list[str] = None,
     ):
+        if required_arguments is None:
+            required_arguments = []
         super().__init__(scenario=scenario, required_arguments=required_arguments)
         self._target_function = target_function
 
         # Check if target function is callable
         if not callable(self._target_function):
             raise TypeError(
                 "Argument `target_function` must be a callable but is type" f"`{type(self._target_function)}`."
```

### Comparing `smac-2.0.2/smac/runner/target_function_script_runner.py` & `smac-2.1.0/smac/runner/target_function_script_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,16 +47,18 @@
         A list of required arguments, which are passed to the target function.
     """
 
     def __init__(
         self,
         target_function: str,
         scenario: Scenario,
-        required_arguments: list[str] = [],
+        required_arguments: list[str] = None,
     ):
+        if required_arguments is None:
+            required_arguments = []
         super().__init__(scenario=scenario, required_arguments=required_arguments)
         self._target_function = target_function
 
         # Check if target function is callable
         if not isinstance(self._target_function, str):
             raise TypeError(
                 "Argument `target_function` must be a string but is type" f"`{type(self._target_function)}`."
```

### Comparing `smac-2.0.2/smac/scenario.py` & `smac-2.1.0/smac/scenario.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/utils/configspace.py` & `smac-2.1.0/smac/utils/configspace.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/utils/data_structures.py` & `smac-2.1.0/smac/utils/data_structures.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/utils/logging.py` & `smac-2.1.0/smac/utils/logging.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/utils/multi_objective.py` & `smac-2.1.0/smac/utils/multi_objective.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/utils/pareto_front.py` & `smac-2.1.0/smac/utils/pareto_front.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/utils/subspaces/__init__.py` & `smac-2.1.0/smac/utils/subspaces/__init__.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/utils/subspaces/boing_subspace.py` & `smac-2.1.0/smac/utils/subspaces/boing_subspace.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac/utils/subspaces/turbo_subspace.py` & `smac-2.1.0/smac/utils/subspaces/turbo_subspace.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.2/smac.egg-info/PKG-INFO` & `smac-2.1.0/smac.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smac
-Version: 2.0.2
+Version: 2.1.0
 Summary: SMAC3, a Python implementation of 'Sequential Model-based Algorithm Configuration'.
 Home-page: https://www.automl.org/
 Author: 	Marius Lindauer, Katharina Eggensperger, Matthias Feurer, André Biedenkapp, Difan Deng,
 	Carolin Benjamins, Tim Ruhkopf, René Sass and Frank Hutter
 Author-email: fh@cs.uni-freiburg.de
 License: BSD 3-Clause License
 Project-URL: Documentation, https://https://github.com/automl.github.io/SMAC3/main
```

### Comparing `smac-2.0.2/smac.egg-info/SOURCES.txt` & `smac-2.1.0/smac.egg-info/SOURCES.txt`

 * *Files identical despite different names*

