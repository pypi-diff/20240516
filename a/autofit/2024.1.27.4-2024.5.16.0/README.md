# Comparing `tmp/autofit-2024.1.27.4.tar.gz` & `tmp/autofit-2024.5.16.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autofit-2024.1.27.4.tar", last modified: Sat Jan 27 19:56:38 2024, max compression
+gzip compressed data, was "autofit-2024.5.16.0.tar", last modified: Thu May 16 09:57:33 2024, max compression
```

## Comparing `autofit-2024.1.27.4.tar` & `autofit-2024.5.16.0.tar`

### file list

```diff
@@ -1,305 +1,428 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.105184 autofit-2024.1.27.4/
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/CITATIONS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8572 2024-01-27 19:56:38.105184 autofit-2024.1.27.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.065184 autofit-2024.1.27.4/autofit/
--rw-r--r--   0 runner    (1001) docker     (127)     5843 2024-01-27 19:56:31.000000 autofit-2024.1.27.4/autofit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.065184 autofit-2024.1.27.4/autofit/aggregator/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/aggregator/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11540 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/aggregator/aggregator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/aggregator/file_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/aggregator/predicate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11525 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/aggregator/search_output.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.069184 autofit-2024.1.27.4/autofit/config/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/config/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/config/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/config/general.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/config/logging.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.069184 autofit-2024.1.27.4/autofit/config/non_linear/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/config/non_linear/GridSearch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/config/non_linear/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/config/non_linear/mcmc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8648 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/config/non_linear/nest.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/config/non_linear/optimize.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/config/notation.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/config/output.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.069184 autofit-2024.1.27.4/autofit/config/priors/
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/config/priors/Exponential.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/config/priors/Gaussian.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/config/priors/GaussianKurtosis.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/config/priors/MultiLevelGaussians.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/config/priors/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/config/priors/model.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/config/priors/prior.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/config/priors/profiles.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/config/priors/template.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.069184 autofit-2024.1.27.4/autofit/config/visualize/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/config/visualize/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/config/visualize/general.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/config/visualize/plots_search.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.069184 autofit-2024.1.27.4/autofit/database/
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/database/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.073184 autofit-2024.1.27.4/autofit/database/aggregator/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/database/aggregator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15828 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/database/aggregator/aggregator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/database/aggregator/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/database/aggregator/scrape.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.073184 autofit-2024.1.27.4/autofit/database/migration/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/database/migration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6131 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/database/migration/migration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/database/migration/session_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/database/migration/steps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.073184 autofit-2024.1.27.4/autofit/database/model/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/database/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/database/model/array.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/database/model/compound.py
--rw-r--r--   0 runner    (1001) docker     (127)    12454 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/database/model/fit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/database/model/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/database/model/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/database/model/prior.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.073184 autofit-2024.1.27.4/autofit/database/query/
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/database/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/database/query/condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/database/query/junction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.073184 autofit-2024.1.27.4/autofit/database/query/query/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/database/query/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/database/query/query/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/database/query/query/attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/database/query/query/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     8878 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/database/query/query/named.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/database/sqlalchemy_.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.077184 autofit-2024.1.27.4/autofit/example/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7000 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/example/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     6021 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/example/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/example/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/exc.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.077184 autofit-2024.1.27.4/autofit/graphical/
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/graphical/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.077184 autofit-2024.1.27.4/autofit/graphical/declarative/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/graphical/declarative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8648 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/graphical/declarative/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/graphical/declarative/collection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.077184 autofit-2024.1.27.4/autofit/graphical/declarative/factor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/graphical/declarative/factor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/graphical/declarative/factor/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/graphical/declarative/factor/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/graphical/declarative/factor/hierarchical.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/graphical/declarative/factor/prior.py
--rw-r--r--   0 runner    (1001) docker     (127)     8192 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/graphical/declarative/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/graphical/declarative/result.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.077184 autofit-2024.1.27.4/autofit/graphical/expectation_propagation/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/graphical/expectation_propagation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17242 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/graphical/expectation_propagation/ep_mean_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/graphical/expectation_propagation/factor_optimiser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9719 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/graphical/expectation_propagation/history.py
--rw-r--r--   0 runner    (1001) docker     (127)    17494 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/graphical/expectation_propagation/optimiser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/graphical/expectation_propagation/stochastic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/graphical/expectation_propagation/visualise.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.081184 autofit-2024.1.27.4/autofit/graphical/factor_graphs/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/graphical/factor_graphs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14727 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/graphical/factor_graphs/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    16180 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/graphical/factor_graphs/factor.py
--rw-r--r--   0 runner    (1001) docker     (127)    16109 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/graphical/factor_graphs/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/graphical/factor_graphs/jacobians.py
--rw-r--r--   0 runner    (1001) docker     (127)     6392 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/graphical/factor_graphs/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.081184 autofit-2024.1.27.4/autofit/graphical/laplace/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/graphical/laplace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10747 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/graphical/laplace/line_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    12004 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/graphical/laplace/newton.py
--rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/graphical/laplace/optimiser.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18909 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/graphical/mean_field.py
--rw-r--r--   0 runner    (1001) docker     (127)    16822 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/graphical/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.081184 autofit-2024.1.27.4/autofit/interpolator/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/interpolator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/interpolator/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     8608 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/interpolator/covariance.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/interpolator/linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/interpolator/query.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/interpolator/spline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/jax_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.085184 autofit-2024.1.27.4/autofit/mapper/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/mapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/mapper/identifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.085184 autofit-2024.1.27.4/autofit/mapper/mock/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/mapper/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/mapper/mock/mock_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    15378 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/mapper/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/mapper/model_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9859 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/mapper/model_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    23069 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/mapper/operator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.085184 autofit-2024.1.27.4/autofit/mapper/prior/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/mapper/prior/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8818 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/mapper/prior/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.085184 autofit-2024.1.27.4/autofit/mapper/prior/arithmetic/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/mapper/prior/arithmetic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/mapper/prior/arithmetic/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/mapper/prior/arithmetic/assertion.py
--rw-r--r--   0 runner    (1001) docker     (127)     8550 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/mapper/prior/arithmetic/compound.py
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/mapper/prior/deferred.py
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/mapper/prior/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/mapper/prior/log_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/mapper/prior/log_uniform.py
--rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/mapper/prior/tuple_prior.py
--rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/mapper/prior/uniform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/mapper/prior/width_modifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.089184 autofit-2024.1.27.4/autofit/mapper/prior_model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/mapper/prior_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    65184 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/mapper/prior_model/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/mapper/prior_model/annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/mapper/prior_model/attribute_pair.py
--rw-r--r--   0 runner    (1001) docker     (127)     9515 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/mapper/prior_model/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    17025 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/mapper/prior_model/prior_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/mapper/prior_model/recursion.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/mapper/prior_model/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    17043 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/mapper/variable.py
--rw-r--r--   0 runner    (1001) docker     (127)    19865 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/mapper/variable_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.089184 autofit-2024.1.27.4/autofit/messages/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14433 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/messages/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/messages/beta.py
--rw-r--r--   0 runner    (1001) docker     (127)     9477 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/messages/composed_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/messages/fixed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/messages/gamma.py
--rw-r--r--   0 runner    (1001) docker     (127)     7813 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/messages/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     8868 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/messages/normal.py
--rw-r--r--   0 runner    (1001) docker     (127)    11019 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/messages/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/messages/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.089184 autofit-2024.1.27.4/autofit/non_linear/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.093184 autofit-2024.1.27.4/autofit/non_linear/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/analysis/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    12753 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/analysis/combined.py
--rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/analysis/free_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/analysis/indexed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/analysis/model_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/analysis/multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/fitness.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.093184 autofit-2024.1.27.4/autofit/non_linear/grid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/grid/grid_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.093184 autofit-2024.1.27.4/autofit/non_linear/grid/grid_search/
--rw-r--r--   0 runner    (1001) docker     (127)    12415 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/grid/grid_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/grid/grid_search/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     8999 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/grid/grid_search/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/grid/grid_search/result_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.093184 autofit-2024.1.27.4/autofit/non_linear/grid/sensitivity/
--rw-r--r--   0 runner    (1001) docker     (127)    11590 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/grid/sensitivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/grid/sensitivity/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/grid/sensitivity/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/grid/simple_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)    11159 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/initializer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.093184 autofit-2024.1.27.4/autofit/non_linear/mock/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/mock/mock_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/mock/mock_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/mock/mock_samples.py
--rw-r--r--   0 runner    (1001) docker     (127)     5544 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/mock/mock_search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.093184 autofit-2024.1.27.4/autofit/non_linear/parallel/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/parallel/process.py
--rw-r--r--   0 runner    (1001) docker     (127)    14203 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/parallel/sneaky.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.097184 autofit-2024.1.27.4/autofit/non_linear/paths/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/paths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13143 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/paths/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     8086 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/paths/database.py
--rw-r--r--   0 runner    (1001) docker     (127)    13431 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/paths/directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/paths/null.py
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/paths/sub_directory_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)    10769 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/result.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.097184 autofit-2024.1.27.4/autofit/non_linear/samples/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/samples/efficient.py
--rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/samples/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     7626 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/samples/mcmc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6083 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/samples/nest.py
--rw-r--r--   0 runner    (1001) docker     (127)    18284 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/samples/pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     8410 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/samples/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)    20292 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/samples/samples.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/samples/stored.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/samples/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.097184 autofit-2024.1.27.4/autofit/non_linear/search/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41549 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/search/abstract_search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.097184 autofit-2024.1.27.4/autofit/non_linear/search/mcmc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/search/mcmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/search/mcmc/abstract_mcmc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5401 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/search/mcmc/auto_correlations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.097184 autofit-2024.1.27.4/autofit/non_linear/search/mcmc/emcee/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/search/mcmc/emcee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/search/mcmc/emcee/plotter.py
--rw-r--r--   0 runner    (1001) docker     (127)    12990 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/search/mcmc/emcee/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.101184 autofit-2024.1.27.4/autofit/non_linear/search/mcmc/zeus/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/search/mcmc/zeus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/search/mcmc/zeus/plotter.py
--rw-r--r--   0 runner    (1001) docker     (127)    13926 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/search/mcmc/zeus/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.101184 autofit-2024.1.27.4/autofit/non_linear/search/nest/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/search/nest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/search/nest/abstract_nest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.101184 autofit-2024.1.27.4/autofit/non_linear/search/nest/dynesty/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/search/nest/dynesty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/search/nest/dynesty/plotter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.101184 autofit-2024.1.27.4/autofit/non_linear/search/nest/dynesty/search/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/search/nest/dynesty/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17954 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/search/nest/dynesty/search/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/search/nest/dynesty/search/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/search/nest/dynesty/search/static.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.101184 autofit-2024.1.27.4/autofit/non_linear/search/nest/nautilus/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/search/nest/nautilus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/search/nest/nautilus/plotter.py
--rw-r--r--   0 runner    (1001) docker     (127)    18913 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/search/nest/nautilus/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.101184 autofit-2024.1.27.4/autofit/non_linear/search/nest/ultranest/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/search/nest/ultranest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/search/nest/ultranest/plotter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11825 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/search/nest/ultranest/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.101184 autofit-2024.1.27.4/autofit/non_linear/search/optimize/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/search/optimize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/search/optimize/abstract_optimize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.101184 autofit-2024.1.27.4/autofit/non_linear/search/optimize/drawer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/search/optimize/drawer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/search/optimize/drawer/plotter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7003 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/search/optimize/drawer/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.101184 autofit-2024.1.27.4/autofit/non_linear/search/optimize/lbfgs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/search/optimize/lbfgs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8740 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/search/optimize/lbfgs/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.105184 autofit-2024.1.27.4/autofit/non_linear/search/optimize/pyswarms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/search/optimize/pyswarms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/search/optimize/pyswarms/plotter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.105184 autofit-2024.1.27.4/autofit/non_linear/search/optimize/pyswarms/search/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/search/optimize/pyswarms/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12391 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/search/optimize/pyswarms/search/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/search/optimize/pyswarms/search/globe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/search/optimize/pyswarms/search/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/non_linear/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.105184 autofit-2024.1.27.4/autofit/plot/
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/plot/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/plot/samples_plotters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.105184 autofit-2024.1.27.4/autofit/text/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7089 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/text/formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/text/samples_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     4688 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/text/text_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.105184 autofit-2024.1.27.4/autofit/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/tools/add_notebook_quotes.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/tools/namer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/autofit/tools/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.105184 autofit-2024.1.27.4/autofit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9349 2024-01-27 19:56:38.000000 autofit-2024.1.27.4/autofit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:38.105184 autofit-2024.1.27.4/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:31.000000 autofit-2024.1.27.4/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      454 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/scripts/add_notebook_quotes.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      268 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/scripts/aggregate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      833 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/scripts/update_identifiers.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-01-27 19:56:38.109184 autofit-2024.1.27.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-01-27 19:56:30.000000 autofit-2024.1.27.4/setup.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.619212 autofit-2024.5.16.0/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:32.681794 autofit-2024.5.16.0/.github/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:32.746325 autofit-2024.5.16.0/.github/workflows/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2889 2024-04-24 06:43:36.000000 autofit-2024.5.16.0/.github/workflows/main.yml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      809 2023-09-14 15:31:52.000000 autofit-2024.5.16.0/CITATIONS.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18817 2023-09-14 15:31:52.000000 autofit-2024.5.16.0/CODE_OF_CONDUCT.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2454 2023-09-14 15:31:52.000000 autofit-2024.5.16.0/CONTRIBUTING.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1091 2023-09-14 15:31:52.000000 autofit-2024.5.16.0/LICENSE
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      379 2023-09-14 15:31:52.000000 autofit-2024.5.16.0/MANIFEST.in
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7992 2024-05-16 09:57:33.619212 autofit-2024.5.16.0/PKG-INFO
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7196 2023-09-14 15:31:52.000000 autofit-2024.5.16.0/README.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:32.760331 autofit-2024.5.16.0/autofit/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5767 2024-05-16 09:55:27.000000 autofit-2024.5.16.0/autofit/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:32.773567 autofit-2024.5.16.0/autofit/aggregator/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      106 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/aggregator/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11540 2024-04-24 06:43:36.000000 autofit-2024.5.16.0/autofit/aggregator/aggregator.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7478 2024-04-24 06:43:36.000000 autofit-2024.5.16.0/autofit/aggregator/base.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2922 2024-04-24 06:43:36.000000 autofit-2024.5.16.0/autofit/aggregator/file_output.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9866 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/aggregator/predicate.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12917 2024-04-24 06:43:36.000000 autofit-2024.5.16.0/autofit/aggregator/search_output.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       27 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/conf.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:32.789187 autofit-2024.5.16.0/autofit/config/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       11 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/config/.gitignore
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      668 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/config/README.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3558 2024-04-24 06:43:36.000000 autofit-2024.5.16.0/autofit/config/general.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      306 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/config/logging.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:32.801169 autofit-2024.5.16.0/autofit/config/non_linear/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      315 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/config/non_linear/GridSearch.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      439 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/config/non_linear/README.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4999 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/config/non_linear/mcmc.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8733 2024-04-24 06:43:36.000000 autofit-2024.5.16.0/autofit/config/non_linear/nest.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6591 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/config/non_linear/optimize.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1224 2024-04-24 06:43:36.000000 autofit-2024.5.16.0/autofit/config/notation.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5473 2024-04-24 06:43:36.000000 autofit-2024.5.16.0/autofit/config/output.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:32.824160 autofit-2024.5.16.0/autofit/config/priors/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      511 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/config/priors/Exponential.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      627 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/config/priors/Gaussian.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      796 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/config/priors/GaussianKurtosis.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      180 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/config/priors/MultiLevelGaussians.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1706 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/config/priors/README.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1168 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/config/priors/model.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      123 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/config/priors/prior.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1168 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/config/priors/profiles.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1187 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/config/priors/template.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:32.835160 autofit-2024.5.16.0/autofit/config/visualize/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      301 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/config/visualize/README.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      179 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/config/visualize/general.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      329 2024-04-24 06:43:36.000000 autofit-2024.5.16.0/autofit/config/visualize/plots_search.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      640 2024-04-24 06:43:36.000000 autofit-2024.5.16.0/autofit/config/visualize/plots_settings.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:32.839159 autofit-2024.5.16.0/autofit/database/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2351 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/database/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:32.848160 autofit-2024.5.16.0/autofit/database/aggregator/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       87 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/database/aggregator/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    16043 2024-04-24 06:43:36.000000 autofit-2024.5.16.0/autofit/database/aggregator/aggregator.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1913 2024-04-24 06:43:36.000000 autofit-2024.5.16.0/autofit/database/aggregator/info.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5619 2024-04-24 06:43:36.000000 autofit-2024.5.16.0/autofit/database/aggregator/scrape.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:32.856159 autofit-2024.5.16.0/autofit/database/migration/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       82 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/database/migration/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6131 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/database/migration/migration.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2485 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/database/migration/session_wrapper.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1190 2024-04-24 06:43:36.000000 autofit-2024.5.16.0/autofit/database/migration/steps.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:32.877159 autofit-2024.5.16.0/autofit/database/model/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      152 2024-04-24 06:43:36.000000 autofit-2024.5.16.0/autofit/database/model/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2460 2024-04-24 06:43:36.000000 autofit-2024.5.16.0/autofit/database/model/array.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      800 2024-04-24 06:43:36.000000 autofit-2024.5.16.0/autofit/database/model/common.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      871 2024-04-24 06:43:36.000000 autofit-2024.5.16.0/autofit/database/model/compound.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12834 2024-04-24 06:43:36.000000 autofit-2024.5.16.0/autofit/database/model/fit.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      846 2024-04-24 06:43:36.000000 autofit-2024.5.16.0/autofit/database/model/function.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2694 2024-04-24 06:43:36.000000 autofit-2024.5.16.0/autofit/database/model/instance.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6237 2024-04-24 06:43:36.000000 autofit-2024.5.16.0/autofit/database/model/model.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2699 2024-04-24 06:43:36.000000 autofit-2024.5.16.0/autofit/database/model/prior.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:32.884160 autofit-2024.5.16.0/autofit/database/query/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      468 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/database/query/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6449 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/database/query/condition.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4888 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/database/query/junction.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:32.896161 autofit-2024.5.16.0/autofit/database/query/query/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      129 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/database/query/query/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1643 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/database/query/query/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3012 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/database/query/query/attribute.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1199 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/database/query/query/info.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8878 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/database/query/query/named.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1086 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/database/sqlalchemy_.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:32.909160 autofit-2024.5.16.0/autofit/example/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      126 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/example/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9659 2024-04-24 06:43:36.000000 autofit-2024.5.16.0/autofit/example/analysis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6115 2024-04-24 06:43:36.000000 autofit-2024.5.16.0/autofit/example/model.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      533 2024-04-24 06:43:36.000000 autofit-2024.5.16.0/autofit/example/result.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1753 2024-04-24 06:43:36.000000 autofit-2024.5.16.0/autofit/example/util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8804 2024-04-24 06:43:36.000000 autofit-2024.5.16.0/autofit/example/visualize.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1647 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/exc.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      845 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/fixtures.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:32.916160 autofit-2024.5.16.0/autofit/graphical/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      813 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/graphical/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:32.928161 autofit-2024.5.16.0/autofit/graphical/declarative/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        1 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/graphical/declarative/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8668 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/graphical/declarative/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3186 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/graphical/declarative/collection.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:32.940160 autofit-2024.5.16.0/autofit/graphical/declarative/factor/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/graphical/declarative/factor/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2554 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/graphical/declarative/factor/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4100 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/graphical/declarative/factor/analysis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6630 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/graphical/declarative/factor/hierarchical.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1920 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/graphical/declarative/factor/prior.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8192 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/graphical/declarative/graph.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4721 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/graphical/declarative/result.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:32.956160 autofit-2024.5.16.0/autofit/graphical/expectation_propagation/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      213 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/graphical/expectation_propagation/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    17242 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/graphical/expectation_propagation/ep_mean_field.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2068 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/graphical/expectation_propagation/factor_optimiser.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9719 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/graphical/expectation_propagation/history.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    17494 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/graphical/expectation_propagation/optimiser.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4417 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/graphical/expectation_propagation/stochastic.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1745 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/graphical/expectation_propagation/visualise.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:32.970231 autofit-2024.5.16.0/autofit/graphical/factor_graphs/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      274 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/graphical/factor_graphs/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14727 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/graphical/factor_graphs/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    16180 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/graphical/factor_graphs/factor.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    16109 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/graphical/factor_graphs/graph.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4671 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/graphical/factor_graphs/jacobians.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6392 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/graphical/factor_graphs/transform.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:32.978230 autofit-2024.5.16.0/autofit/graphical/laplace/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      155 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/graphical/laplace/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10747 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/graphical/laplace/line_search.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12004 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/graphical/laplace/newton.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6087 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/graphical/laplace/optimiser.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18909 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/graphical/mean_field.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    16822 2024-03-26 18:27:39.000000 autofit-2024.5.16.0/autofit/graphical/utils.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:32.991232 autofit-2024.5.16.0/autofit/interpolator/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      145 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/interpolator/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4023 2023-12-11 20:56:25.000000 autofit-2024.5.16.0/autofit/interpolator/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8608 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/interpolator/covariance.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      362 2023-12-11 20:56:31.000000 autofit-2024.5.16.0/autofit/interpolator/linear.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1911 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/interpolator/query.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      357 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/interpolator/spline.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1144 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/jax_wrapper.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.007888 autofit-2024.5.16.0/autofit/mapper/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      124 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/mapper/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4880 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/mapper/identifier.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.013286 autofit-2024.5.16.0/autofit/mapper/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/mapper/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4507 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/mapper/mock/mock_model.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    15451 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/mapper/model.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2656 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/mapper/model_mapper.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10150 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/mapper/model_object.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    23069 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/mapper/operator.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.037157 autofit-2024.5.16.0/autofit/mapper/prior/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      154 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/mapper/prior/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8970 2024-05-03 12:26:40.000000 autofit-2024.5.16.0/autofit/mapper/prior/abstract.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.047210 autofit-2024.5.16.0/autofit/mapper/prior/arithmetic/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       40 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/mapper/prior/arithmetic/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6412 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/mapper/prior/arithmetic/arithmetic.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3706 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/mapper/prior/arithmetic/assertion.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11808 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/mapper/prior/arithmetic/compound.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2066 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/mapper/prior/deferred.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3499 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/mapper/prior/gaussian.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3570 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/mapper/prior/log_gaussian.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4375 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/mapper/prior/log_uniform.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4311 2023-12-01 11:23:42.000000 autofit-2024.5.16.0/autofit/mapper/prior/tuple_prior.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3522 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/mapper/prior/uniform.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2654 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/mapper/prior/width_modifier.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.070217 autofit-2024.5.16.0/autofit/mapper/prior_model/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/mapper/prior_model/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    62550 2024-04-24 06:48:06.000000 autofit-2024.5.16.0/autofit/mapper/prior_model/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      666 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/mapper/prior_model/annotation.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1431 2024-03-04 17:35:28.000000 autofit-2024.5.16.0/autofit/mapper/prior_model/attribute_pair.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9712 2024-04-24 06:49:49.000000 autofit-2024.5.16.0/autofit/mapper/prior_model/collection.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    17310 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/mapper/prior_model/prior_model.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2787 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/mapper/prior_model/recursion.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2752 2024-04-29 14:02:12.000000 autofit-2024.5.16.0/autofit/mapper/prior_model/representative.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      196 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/mapper/prior_model/util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    17043 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/mapper/variable.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    19865 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/mapper/variable_operator.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.093212 autofit-2024.5.16.0/autofit/messages/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      340 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/messages/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14433 2023-09-14 15:32:09.000000 autofit-2024.5.16.0/autofit/messages/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4679 2023-09-14 15:32:09.000000 autofit-2024.5.16.0/autofit/messages/beta.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10699 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/messages/composed_transform.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2568 2023-09-14 15:32:09.000000 autofit-2024.5.16.0/autofit/messages/fixed.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3231 2023-09-14 15:32:09.000000 autofit-2024.5.16.0/autofit/messages/gamma.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7813 2023-09-14 15:32:09.000000 autofit-2024.5.16.0/autofit/messages/interface.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9106 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/messages/normal.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11657 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/messages/transform.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1251 2023-09-14 15:32:09.000000 autofit-2024.5.16.0/autofit/messages/utils.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1852 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/mock.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.105210 autofit-2024.5.16.0/autofit/non_linear/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-09-14 15:32:09.000000 autofit-2024.5.16.0/autofit/non_linear/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.124211 autofit-2024.5.16.0/autofit/non_linear/analysis/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      120 2024-03-26 18:25:34.000000 autofit-2024.5.16.0/autofit/non_linear/analysis/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9037 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/analysis/analysis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13628 2024-05-03 12:49:14.000000 autofit-2024.5.16.0/autofit/non_linear/analysis/combined.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3827 2024-05-06 11:31:22.000000 autofit-2024.5.16.0/autofit/non_linear/analysis/free_parameter.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5022 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/analysis/indexed.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2319 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/analysis/model_analysis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5262 2023-12-01 11:23:42.000000 autofit-2024.5.16.0/autofit/non_linear/analysis/multiprocessing.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2768 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/analysis/visualize.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9151 2024-04-29 18:07:15.000000 autofit-2024.5.16.0/autofit/non_linear/fitness.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.130210 autofit-2024.5.16.0/autofit/non_linear/grid/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-09-14 15:32:09.000000 autofit-2024.5.16.0/autofit/non_linear/grid/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2371 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/grid/grid_list.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.141212 autofit-2024.5.16.0/autofit/non_linear/grid/grid_search/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12500 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/grid/grid_search/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1825 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/grid/grid_search/job.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8999 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/grid/grid_search/result.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2797 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/grid/grid_search/result_builder.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.149211 autofit-2024.5.16.0/autofit/non_linear/grid/sensitivity/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11586 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/grid/sensitivity/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4403 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/grid/sensitivity/job.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3397 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/grid/sensitivity/result.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1697 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/grid/simple_grid.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12536 2024-04-29 14:02:12.000000 autofit-2024.5.16.0/autofit/non_linear/initializer.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.163211 autofit-2024.5.16.0/autofit/non_linear/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/non_linear/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      761 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/non_linear/mock/mock_analysis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1915 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/mock/mock_result.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2098 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/mock/mock_samples.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2146 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/mock/mock_samples_summary.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5445 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/mock/mock_search.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.168210 autofit-2024.5.16.0/autofit/non_linear/parallel/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      201 2023-12-01 11:23:42.000000 autofit-2024.5.16.0/autofit/non_linear/parallel/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5220 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/non_linear/parallel/process.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13394 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/parallel/sneaky.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.184247 autofit-2024.5.16.0/autofit/non_linear/paths/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       74 2023-09-14 15:32:09.000000 autofit-2024.5.16.0/autofit/non_linear/paths/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14463 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/paths/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8412 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/paths/database.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    16934 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/paths/directory.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2343 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/paths/null.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3644 2023-09-14 15:32:09.000000 autofit-2024.5.16.0/autofit/non_linear/paths/sub_directory_paths.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.199223 autofit-2024.5.16.0/autofit/non_linear/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      118 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      212 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/plot/mcmc_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3785 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/plot/nest_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      236 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/plot/optimize_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4443 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/plot/output.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3386 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/plot/samples_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    15831 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/result.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.227229 autofit-2024.5.16.0/autofit/non_linear/samples/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      201 2023-09-14 15:32:09.000000 autofit-2024.5.16.0/autofit/non_linear/samples/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2454 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/samples/efficient.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6877 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/samples/interface.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7404 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/samples/mcmc.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5272 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/samples/nest.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    17252 2024-05-15 17:08:37.000000 autofit-2024.5.16.0/autofit/non_linear/samples/pdf.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8443 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/samples/sample.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14675 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/samples/samples.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      940 2023-09-14 15:32:09.000000 autofit-2024.5.16.0/autofit/non_linear/samples/stored.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2909 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/samples/summary.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      818 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/samples/util.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.231212 autofit-2024.5.16.0/autofit/non_linear/search/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-09-14 15:32:09.000000 autofit-2024.5.16.0/autofit/non_linear/search/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    42755 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/search/abstract_search.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.239274 autofit-2024.5.16.0/autofit/non_linear/search/mcmc/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-09-14 15:32:09.000000 autofit-2024.5.16.0/autofit/non_linear/search/mcmc/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2281 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/search/mcmc/abstract_mcmc.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5401 2023-09-14 15:32:09.000000 autofit-2024.5.16.0/autofit/non_linear/search/mcmc/auto_correlations.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.246210 autofit-2024.5.16.0/autofit/non_linear/search/mcmc/emcee/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-09-14 15:32:09.000000 autofit-2024.5.16.0/autofit/non_linear/search/mcmc/emcee/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13679 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/search/mcmc/emcee/search.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.252245 autofit-2024.5.16.0/autofit/non_linear/search/mcmc/zeus/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-09-14 15:32:09.000000 autofit-2024.5.16.0/autofit/non_linear/search/mcmc/zeus/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13967 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/search/mcmc/zeus/search.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.257225 autofit-2024.5.16.0/autofit/non_linear/search/nest/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-09-14 15:32:09.000000 autofit-2024.5.16.0/autofit/non_linear/search/nest/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3287 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/search/nest/abstract_nest.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.261213 autofit-2024.5.16.0/autofit/non_linear/search/nest/dynesty/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-09-14 15:32:09.000000 autofit-2024.5.16.0/autofit/non_linear/search/nest/dynesty/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.272210 autofit-2024.5.16.0/autofit/non_linear/search/nest/dynesty/search/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-09-14 15:32:09.000000 autofit-2024.5.16.0/autofit/non_linear/search/nest/dynesty/search/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    17679 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/search/nest/dynesty/search/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4952 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/search/nest/dynesty/search/dynamic.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6084 2024-04-29 14:02:12.000000 autofit-2024.5.16.0/autofit/non_linear/search/nest/dynesty/search/static.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.278210 autofit-2024.5.16.0/autofit/non_linear/search/nest/nautilus/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-09-14 15:32:09.000000 autofit-2024.5.16.0/autofit/non_linear/search/nest/nautilus/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    20149 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/search/nest/nautilus/search.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.284247 autofit-2024.5.16.0/autofit/non_linear/search/nest/ultranest/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-09-14 15:32:09.000000 autofit-2024.5.16.0/autofit/non_linear/search/nest/ultranest/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12499 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/search/nest/ultranest/search.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.290216 autofit-2024.5.16.0/autofit/non_linear/search/optimize/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-09-14 15:32:09.000000 autofit-2024.5.16.0/autofit/non_linear/search/optimize/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      900 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/search/optimize/abstract_optimize.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.296213 autofit-2024.5.16.0/autofit/non_linear/search/optimize/drawer/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-09-14 15:32:09.000000 autofit-2024.5.16.0/autofit/non_linear/search/optimize/drawer/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6509 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/search/optimize/drawer/search.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.304215 autofit-2024.5.16.0/autofit/non_linear/search/optimize/lbfgs/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-09-14 15:32:09.000000 autofit-2024.5.16.0/autofit/non_linear/search/optimize/lbfgs/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8366 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/search/optimize/lbfgs/search.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.309246 autofit-2024.5.16.0/autofit/non_linear/search/optimize/pyswarms/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-09-14 15:32:09.000000 autofit-2024.5.16.0/autofit/non_linear/search/optimize/pyswarms/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.323218 autofit-2024.5.16.0/autofit/non_linear/search/optimize/pyswarms/search/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-09-14 15:32:09.000000 autofit-2024.5.16.0/autofit/non_linear/search/optimize/pyswarms/search/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11789 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/search/optimize/pyswarms/search/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3081 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/search/optimize/pyswarms/search/globe.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3171 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/non_linear/search/optimize/pyswarms/search/local.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2479 2023-09-14 15:32:09.000000 autofit-2024.5.16.0/autofit/non_linear/settings.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2242 2023-12-01 11:23:42.000000 autofit-2024.5.16.0/autofit/non_linear/timer.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.326246 autofit-2024.5.16.0/autofit/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      315 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/plot/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.334211 autofit-2024.5.16.0/autofit/text/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       50 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/text/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7145 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/text/formatter.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3126 2024-04-29 14:02:12.000000 autofit-2024.5.16.0/autofit/text/samples_text.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4966 2024-04-29 14:02:12.000000 autofit-2024.5.16.0/autofit/text/text_util.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.346212 autofit-2024.5.16.0/autofit/tools/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/tools/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      766 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/tools/add_notebook_quotes.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      438 2023-09-14 15:32:08.000000 autofit-2024.5.16.0/autofit/tools/namer.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3546 2023-12-01 11:23:42.000000 autofit-2024.5.16.0/autofit/tools/util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6048 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/autofit/visualise.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.618214 autofit-2024.5.16.0/autofit.egg-info/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12476 2024-05-16 09:57:32.000000 autofit-2024.5.16.0/autofit.egg-info/SOURCES.txt
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       13 2023-12-01 11:23:42.000000 autofit-2024.5.16.0/build_requirements.txt
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.357243 autofit-2024.5.16.0/docs/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      654 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/Makefile
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.362214 autofit-2024.5.16.0/docs/_templates/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      832 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/_templates/custom-class-template.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1293 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/_templates/custom_module_template.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.381211 autofit-2024.5.16.0/docs/api/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      967 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/api/analysis.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      944 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/api/database.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1281 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/api/model.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      805 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/docs/api/plot.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1201 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/api/priors.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1145 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/api/samples.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2643 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/api/searches.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      649 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/api/source.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3755 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/conf.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.403211 autofit-2024.5.16.0/docs/cookbooks/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    28895 2024-04-29 14:02:12.000000 autofit-2024.5.16.0/docs/cookbooks/analysis.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10108 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/cookbooks/configs.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    22643 2024-04-29 14:02:12.000000 autofit-2024.5.16.0/docs/cookbooks/database.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    31092 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/cookbooks/model.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    19721 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/cookbooks/multi_level_model.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    29156 2024-04-29 14:02:12.000000 autofit-2024.5.16.0/docs/cookbooks/multiple_datasets.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    33083 2024-05-15 19:25:30.000000 autofit-2024.5.16.0/docs/cookbooks/result.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18251 2024-04-29 14:02:12.000000 autofit-2024.5.16.0/docs/cookbooks/search.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.417210 autofit-2024.5.16.0/docs/features/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8207 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/features/graphical.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.475225 autofit-2024.5.16.0/docs/features/images/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    53610 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/features/images/gaussian_x1_1__low_snr.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    38449 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/features/images/gaussian_x1_2__low_snr.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    37485 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/features/images/gaussian_x1_3__low_snr.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    33505 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/features/images/gaussian_x1_with_feature.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    44404 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/features/images/gaussian_x1_with_feature_fit_feature.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    43221 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/features/images/gaussian_x1_with_feature_fit_no_feature.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    46794 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/features/images/gaussian_x2_fit.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    25965 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/features/images/gaussian_x2_left.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    38024 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/features/images/gaussian_x2_left_fit.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    47517 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/features/images/gaussian_x2_right_fit.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    33623 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/features/images/gaussian_x2_split.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    23811 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/features/images/sensitivity_data_high.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    28902 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/features/images/sensitivity_data_high_fit.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    34204 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/features/images/sensitivity_data_low.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    40377 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/features/images/sensitivity_data_low_fit.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8058 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/docs/features/interpolate.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9083 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/features/search_chaining.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5844 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/features/search_grid_search.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11839 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/docs/features/sensitivity_mapping.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.490210 autofit-2024.5.16.0/docs/general/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1013 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/general/citations.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1014 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/docs/general/configs.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      279 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/general/credits.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1178 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/general/roadmap.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      494 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/general/software.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2300 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/general/workspace.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.500211 autofit-2024.5.16.0/docs/howtofit/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1769 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/howtofit/chapter_1_introduction.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1614 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/howtofit/chapter_database.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2198 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/howtofit/chapter_graphical_models.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5493 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/howtofit/howtofit.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.529214 autofit-2024.5.16.0/docs/images/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    69268 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/images/cornerplot.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    29052 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/images/data.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    26243 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/images/data_2.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    21103 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/images/model_gaussian.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13777 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/images/multi_data_0.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13792 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/images/multi_data_1.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14163 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/images/multi_data_2.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    35860 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/images/multi_model_data_0.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    35729 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/images/multi_model_data_1.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    36074 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/images/multi_model_data_2.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    43169 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/images/toy_model_fit.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    37612 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/images/toy_model_fit_2.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7466 2024-04-29 14:02:12.000000 autofit-2024.5.16.0/docs/index.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.542211 autofit-2024.5.16.0/docs/installation/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1409 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/installation/conda.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1549 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/docs/installation/overview.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1156 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/installation/pip.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1439 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/installation/source.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1446 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/installation/troubleshooting.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      795 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/make.bat
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.553231 autofit-2024.5.16.0/docs/overview/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14279 2024-04-29 14:02:12.000000 autofit-2024.5.16.0/docs/overview/backup.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.570233 autofit-2024.5.16.0/docs/overview/image/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)  1010915 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/overview/image/cluster_example.jpg
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)  2030601 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/overview/image/lens_model.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)  3051390 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/overview/image/lens_model_cluster.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    31017 2024-04-29 14:02:12.000000 autofit-2024.5.16.0/docs/overview/scientific_workflow.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5704 2024-04-29 14:02:12.000000 autofit-2024.5.16.0/docs/overview/statistical_methods.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    20966 2024-04-29 14:02:12.000000 autofit-2024.5.16.0/docs/overview/the_basics.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      438 2024-04-29 14:02:12.000000 autofit-2024.5.16.0/docs/requirements.txt
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.580217 autofit-2024.5.16.0/docs/science_examples/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13088 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/docs/science_examples/astronomy.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      139 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/eden.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.597230 autofit-2024.5.16.0/files/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1339 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/files/citation.tex
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13632 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/files/citations.bib
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1171 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/files/citations.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       31 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/files/eden.ini
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    27322 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/files/gaussian_example.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      544 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/files/release.sh
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1226 2023-11-17 08:59:27.000000 autofit-2024.5.16.0/files/to_do_list
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    43169 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/files/toy_model_fit.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      113 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/optional_requirements.txt
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.605211 autofit-2024.5.16.0/paper/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      180 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/paper/README.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12475 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/paper/paper.bib
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      813 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/paper/paper.json
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11887 2024-04-24 06:43:37.000000 autofit-2024.5.16.0/paper/paper.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      175 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/readthedocs.yml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      354 2024-04-29 14:02:12.000000 autofit-2024.5.16.0/requirements.txt
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:33.616213 autofit-2024.5.16.0/scripts/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/scripts/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      454 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/scripts/add_notebook_quotes.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      268 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/scripts/aggregate.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       39 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/scripts/example_map.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      833 2023-09-14 15:31:53.000000 autofit-2024.5.16.0/scripts/update_identifiers.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       63 2024-05-16 09:57:33.621211 autofit-2024.5.16.0/setup.cfg
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1918 2024-05-16 09:56:09.000000 autofit-2024.5.16.0/setup.py
```

### Comparing `autofit-2024.1.27.4/CITATIONS.rst` & `autofit-2024.5.16.0/CITATIONS.rst`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/LICENSE` & `autofit-2024.5.16.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/PKG-INFO` & `autofit-2024.5.16.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autofit
-Version: 2024.1.27.4
+Version: 2024.5.16.0
 Summary: Classy Probabilistic Programming
 Home-page: https://github.com/rhayes777/PyAutoFit
 Author: James Nightingale and Richard Hayes
 Author-email: richard@rghsoftware.co.uk
 License: MIT License
 Keywords: cli
 Classifier: Intended Audience :: Science/Research
@@ -15,32 +15,14 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: corner==2.2.1
-Requires-Dist: decorator>=4.2.1
-Requires-Dist: dill>=0.3.1.1
-Requires-Dist: dynesty==2.1.2
-Requires-Dist: typing-inspect>=0.4.0
-Requires-Dist: emcee>=3.1.3
-Requires-Dist: matplotlib
-Requires-Dist: numpydoc>=1.0.0
-Requires-Dist: pyprojroot==0.2.0
-Requires-Dist: pyswarms==1.3.0
-Requires-Dist: h5py>=2.10.0
-Requires-Dist: SQLAlchemy==1.3.20
-Requires-Dist: scipy<=1.11.3
-Requires-Dist: astunparse==1.6.3
-Requires-Dist: threadpoolctl<=3.2.0,>=3.1.0
-Requires-Dist: timeout-decorator==0.5.0
-Requires-Dist: xxhash<=3.4.1
-Requires-Dist: autoconf==2024.1.27.4
 
 PyAutoFit: Classy Probabilistic Programming
 ===========================================
 
 .. |binder| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/Jammy2211/autofit_workspace/HEAD
```

### Comparing `autofit-2024.1.27.4/README.rst` & `autofit-2024.5.16.0/README.rst`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/__init__.py` & `autofit-2024.5.16.0/autofit/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,21 +4,23 @@
 from dill import register
 
 from autoconf.dictable import register_parser
 from .non_linear.grid.grid_search import GridSearch as SearchGridSearch
 from . import conf
 from . import exc
 from . import mock as m
+from .aggregator.base import AggBase
 from .database.aggregator.aggregator import GridSearchAggregator
 from .graphical.expectation_propagation.history import EPHistory
 from .graphical.declarative.factor.analysis import AnalysisFactor
 from .graphical.declarative.collection import FactorGraphModel
 from .graphical.declarative.factor.hierarchical import HierarchicalFactor
 from .graphical.laplace import LaplaceOptimiser
 from .non_linear.grid.grid_list import GridList
+from .non_linear.samples.summary import SamplesSummary
 from .non_linear.samples import SamplesMCMC
 from .non_linear.samples import SamplesNest
 from .non_linear.samples import Samples
 from .non_linear.samples import SamplesPDF
 from .non_linear.samples import Sample
 from .non_linear.samples import load_from_table
 from .non_linear.samples import SamplesStored
@@ -49,23 +51,19 @@
 from .mapper.prior import LogGaussianPrior
 from .mapper.prior import LogUniformPrior
 from .mapper.prior.abstract import Prior
 from .mapper.prior.tuple_prior import TuplePrior
 from .mapper.prior import UniformPrior
 from .mapper.prior_model.abstract import AbstractPriorModel
 from .mapper.prior_model.annotation import AnnotationPriorModel
-from .mapper.prior_model.attribute_pair import AttributeNameValue
-from .mapper.prior_model.attribute_pair import InstanceNameValue
-from .mapper.prior_model.attribute_pair import PriorNameValue
-from .mapper.prior_model.attribute_pair import cast_collection
 from .mapper.prior_model.collection import Collection
 from .mapper.prior_model.prior_model import Model
 from .mapper.prior_model.prior_model import Model
-from .mapper.prior_model.util import PriorModelNameValue
 from .non_linear.search.abstract_search import NonLinearSearch
+from .non_linear.analysis.visualize import Visualizer
 from .non_linear.analysis.analysis import Analysis
 from .non_linear.analysis.combined import CombinedAnalysis
 from .non_linear.grid.grid_search import GridSearchResult
 from .non_linear.grid.sensitivity import Sensitivity
 from .non_linear.initializer import InitializerBall
 from .non_linear.initializer import InitializerPrior
 from .non_linear.initializer import SpecificRangeInitializer
@@ -76,23 +74,25 @@
 from .non_linear.search.nest.dynesty.search.dynamic import DynestyDynamic
 from .non_linear.search.nest.dynesty.search.static import DynestyStatic
 from .non_linear.search.nest.ultranest.search import UltraNest
 from .non_linear.search.optimize.drawer.search import Drawer
 from .non_linear.search.optimize.lbfgs.search import LBFGS
 from .non_linear.search.optimize.pyswarms.search.globe import PySwarmsGlobal
 from .non_linear.search.optimize.pyswarms.search.local import PySwarmsLocal
+from .non_linear.paths.abstract import AbstractPaths
 from .non_linear.paths import DirectoryPaths
 from .non_linear.paths import DatabasePaths
 from .non_linear.result import Result
 from .non_linear.result import ResultsCollection
 from .non_linear.settings import SettingsSearch
 from .non_linear.samples.pdf import marginalize
 from .example.model import Gaussian, Exponential
 from .text import formatter
 from .text import samples_text
+from .visualise import VisualiseGraph
 from .interpolator import (
     LinearInterpolator,
     SplineInterpolator,
     CovarianceInterpolator,
     LinearRelationship,
 )
 from .tools import util
@@ -128,8 +128,8 @@
 @register(abc.ABCMeta)
 def save_abc(pickler, obj):
     pickle._Pickler.save_type(pickler, obj)
 
 
 conf.instance.register(__file__)
 
-__version__ = "2024.1.27.4"
+__version__ = "2024.5.16.0"
```

### Comparing `autofit-2024.1.27.4/autofit/aggregator/aggregator.py` & `autofit-2024.5.16.0/autofit/aggregator/aggregator.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/aggregator/file_output.py` & `autofit-2024.5.16.0/autofit/aggregator/file_output.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,20 @@
             separated by '.' and without a suffix. e.g. output/directory/info.json -> directory.info
         path
             The path to the output file
         """
         self.name = name
         self.path = path
 
+    def __str__(self):
+        return f"{self.name} ({self.path})"
+
+    def __repr__(self):
+        return f"<{self.__class__.__name__} {self}>"
+
     @property
     @abstractmethod
     def value(self):
         pass
 
 
 class ArrayOutput(FileOutput):
```

### Comparing `autofit-2024.1.27.4/autofit/aggregator/predicate.py` & `autofit-2024.5.16.0/autofit/aggregator/predicate.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/aggregator/search_output.py` & `autofit-2024.5.16.0/autofit/aggregator/search_output.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 import csv
 import json
 import logging
 import pickle
 from os import path
 from pathlib import Path
-from typing import Generator, Tuple, Optional, List, cast
+from typing import Generator, Tuple, Optional, List, cast, Type
 
 import dill
 
 from autoconf import cached_property
+from autoconf.class_path import get_class
+from autofit.non_linear.samples import Samples
+
 from autofit.non_linear.samples.pdf import SamplesPDF
 from autofit.aggregator.file_output import (
     JSONOutput,
     FileOutput,
 )
 from autofit.mapper.identifier import Identifier
 from autofit.non_linear.samples.sample import samples_from_iterator
 from autoconf.dictable import from_dict
+from autofit.non_linear.samples.summary import SamplesSummary
+from autofit.non_linear.samples.util import simple_model_for_kwargs
 
 # noinspection PyProtectedMember
 original_create_file_handle = dill._dill._create_filehandle
 
 
 def _create_file_handle(*args, **kwargs):
     """
@@ -170,14 +175,15 @@
         directory
             The directory of the search
         """
         super().__init__(directory, reference)
         self.__search = None
         self.__model = None
         self._samples = None
+        self._latent_samples = None
 
         self.directory = directory
 
         self.file_path = directory / "metadata"
 
         try:
             with open(self.file_path) as f:
@@ -186,14 +192,25 @@
                     line.split("=") for line in self.text.split("\n") if "=" in line
                 ]
                 self.__dict__.update({pair[0]: pair[1] for pair in pairs})
         except FileNotFoundError:
             pass
 
     @property
+    def samples_summary(self) -> SamplesSummary:
+        """
+        The summary of the samples, which includes the maximum log likelihood sample and the log evidence.
+
+        This is loaded from a JSON file.
+        """
+        summary = self.value("samples_summary")
+        summary.model = self.model
+        return summary
+
+    @property
     def instance(self):
         """
         The instance of the maximum log likelihood sample i.e. the instance
         with the greatest likelihood.
 
         None if samples cannot be loaded.
         """
@@ -223,31 +240,58 @@
     @property
     def samples(self) -> SamplesPDF:
         """
         The samples of the search, parsed from a CSV containing individual samples
         and a JSON containing metadata.
         """
         if not self._samples:
-            try:
-                info_json = JSONOutput(
-                    "info", self.files_path / "samples_info.json"
-                ).dict
-
-                with open(self.files_path / "samples.csv") as f:
-                    sample_list = samples_from_iterator(csv.reader(f))
-
-                self._samples = SamplesPDF.from_list_info_and_model(
-                    sample_list=sample_list,
-                    samples_info=info_json,
-                    model=self.model,
-                )
-            except FileNotFoundError:
-                raise AttributeError("No samples found")
+            self._samples = self._load_samples(
+                model=self.model,
+            )
         return self._samples
 
+    @property
+    def latent_samples(self):
+        """
+        The latent variables of the search, parsed from a CSV file.
+        """
+        if not self._latent_samples:
+            self._latent_samples = self._load_samples("latent")
+        return self._latent_samples
+
+    def _load_samples(self, name=None, model=None):
+        if name:
+            directory = self.files_path / name
+        else:
+            directory = self.files_path
+        try:
+            info_json = JSONOutput("info", directory / "samples_info.json").dict
+
+            with open(directory / "samples.csv") as f:
+                sample_list = samples_from_iterator(csv.reader(f))
+
+            if model is None:
+                try:
+                    model = simple_model_for_kwargs(sample_list[0].kwargs)
+                except IndexError:
+                    model = None
+
+            cls = cast(
+                Type[Samples],
+                get_class(info_json["class_path"]),
+            )
+
+            return cls.from_list_info_and_model(
+                sample_list=sample_list,
+                samples_info=info_json,
+                model=model,
+            )
+        except FileNotFoundError:
+            raise AttributeError(f"No {name} found")
+
     def names_and_paths(
         self,
         suffix: str,
     ) -> Generator[Tuple[str, Path], None, None]:
         """
         Get the names and paths of files with a given suffix.
```

### Comparing `autofit-2024.1.27.4/autofit/config/README.rst` & `autofit-2024.5.16.0/autofit/config/README.rst`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/config/general.yaml` & `autofit-2024.5.16.0/autofit/config/general.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -6,30 +6,28 @@
 inversion:
   check_reconstruction: true        # If True, the inversion's reconstruction is checked to ensure the solution of a meshs's mapper is not an invalid solution where the values are all the same.
   reconstruction_vmax_factor: 0.5   # Plots of an Inversion's reconstruction use the reconstructed data's bright value multiplied by this factor.  
 model:
   ignore_prior_limits: false        # If ``True`` the limits applied to priors will be ignored, where limits set upper / lower limits. This stops PriorLimitException's from being raised.
 output:
   force_pickle_overwrite: false     # If True pickle files output by a search (e.g. samples.pickle) are recreated when a new model-fit is performed.
-  force_visualize_overwrite: false # If True, visualization images output by a search (e.g. subplots of the fit) are recreated when a new model-fit is performed.
+  force_visualize_overwrite: false  # If True, visualization images output by a search (e.g. subplots of the fit) are recreated when a new model-fit is performed.
   info_whitespace_length: 80        # Length of whitespace between the parameter names and values in the model.info / result.info
   log_level: INFO                   # The level of information output by logging.
   log_to_file: false                # If True, outputs the non-linear search log to a file (and not printed to screen).
   log_file: output.log              # The name of the file the logged output is written to (in the non-linear search output folder)
   model_results_decimal_places: 3   # Number of decimal places estimated parameter values / errors are output in model.results.
   remove_files: false               # If True, all output files of a non-linear search (e.g. samples, visualization, etc.) are deleted once the model-fit has completed, such that only the .zip file remains.
+  search_internal : false    # If True, the search internal folder which contains a saved state of the non-linear search is delete, saving on hard-disk space.
   samples_to_csv: true              # If True, non-linear search samples are written to a .csv file.
   unconverged_sample_size : 100     # If outputting results of an unconverged search, the number of samples used to estimate the median PDF values and errors.
 parallel:
   warn_environment_variables: true  # If True, a warning is displayed when the search's number of CPU > 1 and enviromment variables related to threading are also > 1.
-prior_passer:
-  sigma: 3.0                        # For non-linear search chaining and model prior passing, the sigma value of the inferred model parameter used as the sigma of the passed Gaussian prior.
-  use_errors: true                  # If True, the errors of the previous model's results are used when passing priors.
-  use_widths: true                  # If True the width of the model parameters defined in the priors config file are used.
 profiling:
   parallel_profile: false           # If True, the parallelization of the fit is profiled outputting a cPython graph.
   should_profile: false             # If True, the ``profile_log_likelihood_function()`` function of an analysis class is called throughout a model-fit, profiling run times.
   repeats: 1                        # The number of repeat function calls used to measure run-times when profiling.
 test:
+  check_likelihood_function: true   # if True, when a search is resumed the likelihood of a previous sample is recalculated to ensure it is consistent with the previous run.
   exception_override: false
   lh_timeout_seconds:               # If a float is input, the log_likelihood_function call is timed out after this many seconds, to diagnose infinite loops. Default is None, meaning no timeout.
   parallel_profile: false
```

### Comparing `autofit-2024.1.27.4/autofit/config/non_linear/mcmc.yaml` & `autofit-2024.5.16.0/autofit/config/non_linear/mcmc.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/config/non_linear/nest.yaml` & `autofit-2024.5.16.0/autofit/config/non_linear/nest.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Configuration files that customize the default behaviour of non-linear searches.
 
-# **PyAutoFit** supports the following nested sampling algorithms:
-
 # - Dynesty: https://github.com/joshspeagle/dynesty / https://dynesty.readthedocs.io/en/latest/index.html
+# - Nautilus https://https://github.com/johannesulf/nautilus / https://nautilus-sampler.readthedocs.io/en/stable/index.html
 # - UltraNest: https://github.com/JohannesBuchner/UltraNest / https://johannesbuchner.github.io/UltraNest/readme.html
 
 # Settings in the [search] and [run] entries are specific to each nested algorithm and should be determined by
 # consulting that MCMC method's own readthedocs.
 
 DynestyStatic:
   search:
@@ -23,15 +22,14 @@
     update_interval: null
     walks: 5
   run:
     dlogz: null
     logl_max: .inf
     maxcall: null
     maxiter: null
-    n_effective: null
   initialize:                       # The method used to generate where walkers are initialized in parameter space {prior}.
     method: prior                   # priors: samples are initialized by randomly drawing from each parameter's prior.
   parallel:
     number_of_cores: 1              # The number of cores the search is parallelized over by default, using Python multiprocessing.
     force_x1_cpu: false             # Force Dynesty to not use Python multiprocessing Pool, which can fix issues on certain operating systems.
   printing:
     silence: false                  # If True, the default print output of the non-linear search is silenced and not printed by the Python interpreter.
@@ -54,16 +52,14 @@
   run:
     dlogz_init: 0.01
     logl_max_init: .inf
     maxcall: null
     maxcall_init: null
     maxiter: null
     maxiter_init: null
-    n_effective: .inf
-    n_effective_init: .inf
     nlive_init: 500
   initialize:                       # The method used to generate where walkers are initialized in parameter space {prior}.
     method: prior                   # priors: samples are initialized by randomly drawing from each parameter's prior.
   parallel:
     number_of_cores: 1              # The number of cores the search is parallelized over by default, using Python multiprocessing.
     force_x1_cpu: false             # Force Dynesty to not use Python multiprocessing Pool, which can fix issues on certain operating systems.
   printing:
@@ -81,16 +77,17 @@
     n_networks: 4                   # Number of networks used in the estimator.
     n_batch: 100                    # Number of likelihood evaluations that are performed at each step. If likelihood evaluations are parallelized, should be multiple of the number of parallel processes.
     n_like_new_bound:               # The maximum number of likelihood calls before a new bounds is created. If None, use 10 times n_live.
     vectorized: false               # If True, the likelihood function can receive multiple input sets at once.
     seed:                           # Seed for random number generation used for reproducible results accross different runs.
   run:
     f_live: 0.01                    # Maximum fraction of the evidence contained in the live set before building the initial shells terminates.
-    n_shell:                        # Minimum number of points in each shell. The algorithm will sample from the shells until this is reached. Default is the batch size of the sampler which is 100 unless otherwise specified.
+    n_shell: 1                      # Minimum number of points in each shell. The algorithm will sample from the shells until this is reached. Default is 1.
     n_eff: 500                      # Minimum effective sample size. The algorithm will sample from the shells until this is reached. Default is 10000.
+    n_like_max: .inf                # Maximum number of likelihood evaluations. Regardless of progress, the sampler will stop if this value is reached. Default is infinity.
     discard_exploration: false      # Whether to discard points drawn in the exploration phase. This is required for a fully unbiased posterior and evidence estimate.
     verbose: true                   # Whether to print information about the run.
   initialize:                       # The method used to generate where walkers are initialized in parameter space {prior}.
     method: prior                   # priors: samples are initialized by randomly drawing from each parameter's prior.
   parallel:
     number_of_cores: 1              # The number of cores the search is parallelized over by default, using Python multiprocessing.
     force_x1_cpu: false             # Force Dynesty to not use Python multiprocessing Pool, which can fix issues on certain operating systems.
@@ -139,11 +136,10 @@
     stepsampler_cls: null
   initialize:                       # The method used to generate where walkers are initialized in parameter space {prior}.
     method: prior                   # priors: samples are initialized by randomly drawing from each parameter's prior.
   parallel:
     number_of_cores: 1              # The number of cores the search is parallelized over by default, using Python multiprocessing.
   printing:
     silence: false                  # If True, the default print output of the non-linear search is silenced and not printed by the Python interpreter.
-
   updates:
     iterations_per_update: 500      # The number of iterations of the non-linear search performed between every 'update', where an update performs tasks like outputting model.results.
     remove_state_files_at_end: true # Whether to remove the savestate of the seach (e.g. the Emcee hdf5 file) at the end to save hard-disk space (results are still stored as PyAutoFit pickles and loadable).
```

### Comparing `autofit-2024.1.27.4/autofit/config/non_linear/optimize.yaml` & `autofit-2024.5.16.0/autofit/config/non_linear/optimize.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/config/notation.yaml` & `autofit-2024.5.16.0/autofit/config/notation.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# The notation configs define the labels of every model parameter and its derived quantities, which are used when
+# The notation configs define the labels of every model parameter which are used when
 # visualizing results (for example labeling the axis of the PDF triangle plots output by a non-linear search).
 
 
 # label: The label given to the each parameter, for plots like PDF corner plots.
 
 # For example, if `centre=x`, the plot axis will be labeled 'x'.
```

### Comparing `autofit-2024.1.27.4/autofit/config/priors/Gaussian.yaml` & `autofit-2024.5.16.0/autofit/config/priors/Gaussian.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/config/priors/GaussianKurtosis.yaml` & `autofit-2024.5.16.0/autofit/config/priors/GaussianKurtosis.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/config/priors/README.rst` & `autofit-2024.5.16.0/autofit/config/priors/README.rst`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/config/priors/model.yaml` & `autofit-2024.5.16.0/autofit/config/priors/model.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/config/priors/profiles.yaml` & `autofit-2024.5.16.0/autofit/config/priors/profiles.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/config/priors/template.yaml` & `autofit-2024.5.16.0/autofit/config/priors/template.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/database/__init__.py` & `autofit-2024.5.16.0/autofit/database/__init__.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/database/aggregator/aggregator.py` & `autofit-2024.5.16.0/autofit/database/aggregator/aggregator.py`

 * *Files 2% similar despite different names*

```diff
@@ -387,14 +387,15 @@
         return fits
 
     def add_directory(
         self,
         directory: str,
         auto_commit=True,
         reference: Optional[dict] = None,
+        completed_only: bool = False,
     ):
         """
         Recursively search a directory for autofit results
         and add them to this database.
 
         Any pickles found in the pickles file are implicitly added
         to the fit object.
@@ -411,16 +412,23 @@
             to the database
         directory
             A directory containing autofit results embedded in a
             file structure
         reference
             A dictionary mapping the names of objects in the model
             to their class path.
+        completed_only
+            If true only searches that have completed are added
         """
-        scraper = Scraper(directory, self.session, reference=reference)
+        scraper = Scraper(
+            directory,
+            self.session,
+            reference=reference,
+            completed_only=completed_only,
+        )
         scraper.scrape()
 
         if auto_commit:
             self.session.commit()
             Info(self.session).write()
 
     @classmethod
```

### Comparing `autofit-2024.1.27.4/autofit/database/aggregator/info.py` & `autofit-2024.5.16.0/autofit/database/aggregator/info.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/database/aggregator/scrape.py` & `autofit-2024.5.16.0/autofit/database/aggregator/scrape.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,37 +11,41 @@
 
 class Scraper:
     def __init__(
         self,
         directory: Union[Path, str],
         session: sa.orm.Session,
         reference: Optional[dict] = None,
+        completed_only: bool = True,
     ):
         """
         Facilitates scraping of data output into a directory
         into the database.
 
         Parameters
         ----------
         directory
             A directory in which data has been stored
         session
             A database session
         reference
             A dictionary mapping search names to model paths
+        completed_only
+            If True, only completed fits will be scraped
         """
         self.directory = directory
         self.session = session
         self.reference = reference
 
         from autofit.aggregator.aggregator import Aggregator as ClassicAggregator
 
         self.aggregator = ClassicAggregator.from_directory(
             self.directory,
             reference=self.reference,
+            completed_only=completed_only,
         )
 
     def scrape(self):
         """
         Recursively scrape fits from the directory and
         add them to the session
         """
@@ -82,20 +86,20 @@
                     instance=item.instance,
                     is_complete=item.is_complete,
                     info=item.info,
                     max_log_likelihood=item.max_log_likelihood,
                     parent_id=item.parent_identifier,
                 )
 
-            _add_files(fit, item)
+            _add_files_fit(fit, item)
             for i, child_analysis in enumerate(item.child_analyses):
                 child_fit = m.Fit(
                     id=f"{item.id}_{i}",
                 )
-                _add_files(child_fit, child_analysis)
+                _add_files_fit(child_fit, child_analysis)
                 fit.children.append(child_fit)
 
             yield fit
 
     def _grid_searches(self):
         """
         Retrieve grid searches recursively from an output directory by
@@ -139,35 +143,45 @@
         ------
         NoResultFound
             If no fit is found with the identifier
         """
         return self.session.query(m.Fit).filter(m.Fit.id == item.id).one()
 
 
+def _add_files_fit(fit: m.Fit, item: SearchOutput):
+    try:
+        fit.samples = item.samples
+    except AttributeError:
+        logger.warning(f"Failed to load samples for {fit.id}")
+    try:
+        fit.latent_samples = item.latent_samples
+    except AttributeError:
+        logger.warning(f"Failed to load latent variables for {fit.id}")
+
+    _add_files(fit, item)
+
+
 def _add_files(fit: m.Fit, item: SearchOutput):
     """
     Load files from the path and add them to the database.
 
     Parameters
     ----------
     fit
         A fit to which the pickles belong
     """
-    try:
-        fit.samples = item.samples
-    except AttributeError:
-        logger.warning(f"Failed to load samples for {fit.id}")
-
     for json_output in item.jsons:
         fit.set_json(json_output.name, json_output.dict)
 
     for pickle_output in item.pickles:
         fit.set_pickle(pickle_output.name, pickle_output.value)
 
     for array_output in item.arrays:
+        if array_output.name in ("samples", "latent_samples"):
+            continue
         try:
             fit.set_array(array_output.name, array_output.value)
         except ValueError:
             logger.debug(f"Failed to load array {array_output.name} for {fit.id}")
 
     for hdu_output in item.hdus:
         fit.set_hdu(hdu_output.name, hdu_output.value)
```

### Comparing `autofit-2024.1.27.4/autofit/database/migration/migration.py` & `autofit-2024.5.16.0/autofit/database/migration/migration.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/database/migration/session_wrapper.py` & `autofit-2024.5.16.0/autofit/database/migration/session_wrapper.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/database/migration/steps.py` & `autofit-2024.5.16.0/autofit/database/migration/steps.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,10 +13,16 @@
     ),
     Step(
         "CREATE TABLE array (id INTEGER NOT NULL, name VARCHAR, bytes BLOB, _dtype VARCHAR, _shape VARCHAR, array_type VARCHAR, fit_id VARCHAR, PRIMARY KEY (id), FOREIGN KEY (fit_id) REFERENCES fit (id));"
     ),
     Step(
         "CREATE TABLE hdu (id INTEGER NOT NULL, array_type VARCHAR, _header VARCHAR, PRIMARY KEY (id), FOREIGN KEY (id) REFERENCES array (id));"
     ),
+    Step(
+        "ALTER TABLE object ADD COLUMN latent_variables_for_id INTEGER;",
+    ),
+    Step(
+        "ALTER TABLE object RENAME COLUMN latent_variables_for_id TO latent_samples_for_id;",
+    ),
 ]
 
 migrator = Migrator(*steps)
```

### Comparing `autofit-2024.1.27.4/autofit/database/model/array.py` & `autofit-2024.5.16.0/autofit/database/model/array.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
     id = sa.Column(
         sa.Integer,
         sa.ForeignKey("object.id"),
         primary_key=True,
+        index=True,
     )
 
     __mapper_args__ = {"polymorphic_identity": "array"}
 
     bytes = sa.Column(sa.LargeBinary)
     _dtype = sa.Column(sa.String)
     _shape = sa.Column(sa.String)
@@ -66,15 +67,20 @@
 class HDU(Array):
     """
     A serialised astropy.io.fits.PrimaryHDU
     """
 
     __tablename__ = "hdu"
 
-    id = sa.Column(sa.Integer, sa.ForeignKey("array.id"), primary_key=True)
+    id = sa.Column(
+        sa.Integer,
+        sa.ForeignKey("array.id"),
+        primary_key=True,
+        index=True,
+    )
 
     _header = sa.Column(sa.String)
 
     __mapper_args__ = {
         "polymorphic_identity": "hdu",
     }
```

### Comparing `autofit-2024.1.27.4/autofit/database/model/compound.py` & `autofit-2024.5.16.0/autofit/database/model/compound.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 class Compound(Object):
     __tablename__ = "compound"
 
     id = sa.Column(
         sa.Integer,
         sa.ForeignKey("object.id"),
         primary_key=True,
+        index=True,
     )
     compound_type = sa.Column(sa.String)
 
     @property
     def left(self):
         return self.children[0]
```

### Comparing `autofit-2024.1.27.4/autofit/database/model/fit.py` & `autofit-2024.5.16.0/autofit/database/model/fit.py`

 * *Files 2% similar despite different names*

```diff
@@ -252,27 +252,39 @@
     unique_tag = sa.Column(sa.String)
     name = sa.Column(sa.String)
     path_prefix = sa.Column(sa.String)
 
     _samples = sa.orm.relationship(
         Object, uselist=False, foreign_keys=[Object.samples_for_id]
     )
+    _latent_samples = sa.orm.relationship(
+        Object, uselist=False, foreign_keys=[Object.latent_samples_for_id]
+    )
 
     @property
     @try_none
     def samples(self) -> Samples:
         return self._samples().samples
 
     @samples.setter
     def samples(self, samples):
         self._samples = Object.from_object(
             EfficientSamples(samples),
         )
 
     @property
+    @try_none
+    def latent_samples(self) -> dict:
+        return self._latent_samples()
+
+    @latent_samples.setter
+    def latent_samples(self, latent_samples):
+        self._latent_samples = Object.from_object(latent_samples.minimise())
+
+    @property
     def info(self):
         return {info.key: info.value for info in self._info}
 
     @info.setter
     def info(self, info):
         if info is not None:
             self._info = [Info(key=key, value=value) for key, value in info.items()]
```

### Comparing `autofit-2024.1.27.4/autofit/database/model/instance.py` & `autofit-2024.5.16.0/autofit/database/model/instance.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,142 +3,104 @@
 
 
 class NoneInstance(Object):
     __tablename__ = "none"
 
     id = sa.Column(
         sa.Integer,
-        sa.ForeignKey(
-            "object.id"
-        ),
+        sa.ForeignKey("object.id"),
         primary_key=True,
+        index=True,
     )
 
-    __mapper_args__ = {
-        'polymorphic_identity': 'none'
-    }
+    __mapper_args__ = {"polymorphic_identity": "none"}
 
     def __call__(self):
         return None
 
 
 class Collection(Object):
     """
     A tuple or list
     """
 
     __tablename__ = "collection"
 
     id = sa.Column(
         sa.Integer,
-        sa.ForeignKey(
-            "object.id"
-        ),
-        primary_key=True
+        sa.ForeignKey("object.id"),
+        primary_key=True,
+        index=True,
     )
 
-    __mapper_args__ = {
-        'polymorphic_identity': 'collection'
-    }
+    __mapper_args__ = {"polymorphic_identity": "collection"}
 
     @classmethod
-    def _from_object(
-            cls,
-            source
-    ):
+    def _from_object(cls, source):
         instance = cls()
         instance.cls = type(source)
-        instance._add_children([
-            (str(i), item)
-            for i, item in enumerate(
-                source
-            )
-        ])
+        instance._add_children([(str(i), item) for i, item in enumerate(source)])
         return instance
 
     def __call__(self):
-        return self.cls([
-            child()
-            for child
-            in sorted(
-                self.children,
-                key=lambda child: int(child.name)
-            )
-        ])
+        return self.cls(
+            [
+                child()
+                for child in sorted(self.children, key=lambda child: int(child.name))
+            ]
+        )
 
 
 class Instance(Object):
     """
     An instance, such as a class instance
     """
 
     __tablename__ = "instance"
 
     id = sa.Column(
         sa.Integer,
-        sa.ForeignKey(
-            "object.id"
-        ),
+        sa.ForeignKey("object.id"),
         primary_key=True,
+        index=True,
     )
 
-    __mapper_args__ = {
-        'polymorphic_identity': 'instance'
-    }
+    __mapper_args__ = {"polymorphic_identity": "instance"}
 
     @classmethod
-    def _from_object(
-            cls,
-            source
-    ):
+    def _from_object(cls, source):
         instance = cls()
         instance.cls = type(source)
-        if hasattr(
-                source,
-                "__getstate__"
-        ):
-            instance._add_children(
-                source.__getstate__().items()
-            )
-        elif hasattr(
-                source,
-                "__dict__"
-        ):
-            instance._add_children(
-                source.__dict__.items()
-            )
+        if hasattr(source, "__getstate__"):
+            instance._add_children(source.__getstate__().items())
+        elif hasattr(source, "__dict__"):
+            instance._add_children(source.__dict__.items())
         return instance
 
 
 class Value(Object):
     """
     A float
     """
 
     __tablename__ = "value"
 
-    __mapper_args__ = {
-        'polymorphic_identity': 'value'
-    }
+    __mapper_args__ = {"polymorphic_identity": "value"}
 
     id = sa.Column(
         sa.Integer,
-        sa.ForeignKey(
-            "object.id"
-        ),
+        sa.ForeignKey("object.id"),
         primary_key=True,
+        index=True,
     )
 
     value = sa.Column(sa.Float)
 
     @classmethod
-    def _from_object(
-            cls,
-            source
-    ):
+    def _from_object(cls, source):
         instance = cls()
         instance.value = source
         return instance
 
     def __call__(self):
         return self.value
 
@@ -146,32 +108,26 @@
 class StringValue(Object):
     """
     A string
     """
 
     __tablename__ = "string_value"
 
-    __mapper_args__ = {
-        'polymorphic_identity': 'string_value'
-    }
+    __mapper_args__ = {"polymorphic_identity": "string_value"}
 
     id = sa.Column(
         sa.Integer,
-        sa.ForeignKey(
-            "object.id"
-        ),
+        sa.ForeignKey("object.id"),
         primary_key=True,
+        index=True,
     )
 
     value = sa.Column(sa.String)
 
     @classmethod
-    def _from_object(
-            cls,
-            source
-    ):
+    def _from_object(cls, source):
         instance = cls()
         instance.value = source
         return instance
 
     def __call__(self):
         return self.value
```

### Comparing `autofit-2024.1.27.4/autofit/database/model/model.py` & `autofit-2024.5.16.0/autofit/database/model/model.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,40 +2,50 @@
 import inspect
 from typing import List, Tuple, Any, Iterable, Union, ItemsView, Type
 
 import numpy as np
 
 from autoconf.class_path import get_class, get_class_path
 from ..sqlalchemy_ import sa, declarative
-from autofit.mapper.prior.arithmetic.assertion import ComparisonAssertion
-from autofit.mapper.prior.arithmetic.assertion import CompoundAssertion
 
 Base = declarative.declarative_base()
 
 _schema_version = 1
 
 
 class Object(Base):
     __tablename__ = "object"
 
     type = sa.Column(sa.String)
 
     id = sa.Column(
         sa.Integer,
         primary_key=True,
+        index=True,
     )
 
-    parent_id = sa.Column(sa.Integer, sa.ForeignKey("object.id"))
+    parent_id = sa.Column(
+        sa.Integer,
+        sa.ForeignKey("object.id"),
+        index=True,
+    )
     parent = sa.orm.relationship("Object", uselist=False, remote_side=[id])
 
     samples_for_id = sa.Column(sa.String, sa.ForeignKey("fit.id"))
     samples_for = sa.orm.relationship(
         "Fit", uselist=False, foreign_keys=[samples_for_id]
     )
 
+    latent_samples_for_id = sa.Column(sa.String, sa.ForeignKey("fit.id"))
+    latent_samples_for = sa.orm.relationship(
+        "Fit",
+        uselist=False,
+        foreign_keys=[latent_samples_for_id],
+    )
+
     children: List["Object"] = sa.orm.relationship(
         "Object",
         uselist=True,
     )
 
     def __len__(self):
         return len(self.children)
@@ -88,14 +98,15 @@
         ):
             from .instance import NoneInstance
 
             instance = NoneInstance()
         elif isinstance(source, np.ndarray):
             from .array import Array
 
+            # noinspection PyArgumentList
             instance = Array(array=source)
         elif isinstance(source, Model):
             from .prior import Model
 
             instance = Model._from_object(source)
         elif isinstance(source, Prior):
             from .prior import Prior
@@ -105,27 +116,35 @@
             from .instance import Value
 
             instance = Value._from_object(source)
         elif isinstance(source, (tuple, list)):
             from .instance import Collection
 
             instance = Collection._from_object(source)
-        elif isinstance(source, (Collection, dict)):
+        elif isinstance(source, dict):
+            from .common import Dict
+
+            instance = Dict._from_object(source)
+        elif isinstance(source, Collection):
             from .prior import Collection
 
             instance = Collection._from_object(source)
         elif isinstance(source, str):
             from .instance import StringValue
 
             instance = StringValue._from_object(source)
 
         elif isinstance(source, Compound):
             from .compound import Compound
 
             instance = Compound._from_object(source)
+        elif inspect.isfunction(source):
+            from .function import Function
+
+            instance = Function._from_object(source)
         else:
             from .instance import Instance
 
             instance = Instance._from_object(source)
         instance.name = name
         return instance
 
@@ -151,40 +170,20 @@
 
         If the instance implements __setstate__ then this is
         called with a dictionary of instantiated children.
         """
         instance = self._make_instance()
         child_instances = {child.name: child() for child in self.children}
 
-        assertions = [
-            child
-            for child in child_instances.values()
-            if isinstance(
-                child,
-                (
-                    ComparisonAssertion,
-                    CompoundAssertion,
-                ),
-            )
-        ]
-
-        child_instances = {
-            name: child
-            for name, child in child_instances.items()
-            if child not in assertions
-        }
-
         if hasattr(instance, "__setstate__"):
             instance.__setstate__(child_instances)
         else:
             for name, child in child_instances.items():
                 setattr(instance, name, child)
 
-        instance._assertions = assertions
-
         from autofit import ModelObject
 
         if isinstance(instance, ModelObject) and (
             not hasattr(instance, "id") or instance.id is None
         ):
             instance.id = instance.next_id()
```

### Comparing `autofit-2024.1.27.4/autofit/database/model/prior.py` & `autofit-2024.5.16.0/autofit/database/model/prior.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,35 +5,47 @@
 from autofit.mapper.prior import abstract
 from autofit.mapper.prior_model import prior_model
 from autofit.mapper.prior_model import collection
 
 from .model import Object
 
 
+def extra_children(source):
+    return [
+        (f"_assertions", source.assertions),
+    ]
+
+
 class Collection(Object):
     """
     A collection
     """
 
     __tablename__ = "collection_prior_model"
 
     id = sa.Column(
         sa.Integer,
         sa.ForeignKey("object.id"),
         primary_key=True,
+        index=True,
     )
 
     __mapper_args__ = {"polymorphic_identity": "collection_prior_model"}
 
     @classmethod
     def _from_object(cls, source: Union[collection.Collection, list, dict]):
         instance = cls()
-        if not isinstance(source, collection.Collection):
+        if isinstance(source, collection.Collection):
+            extra_children_ = extra_children(source)
+            instance._add_children(extra_children_)
+        else:
             source = collection.Collection(source)
+
         instance._add_children(source.items())
+
         instance.cls = collection.Collection
         return instance
 
 
 class Model(Object):
     """
     A prior model
@@ -41,52 +53,49 @@
 
     __tablename__ = "prior_model"
 
     id = sa.Column(
         sa.Integer,
         sa.ForeignKey("object.id"),
         primary_key=True,
+        index=True,
     )
 
     __mapper_args__ = {"polymorphic_identity": "prior_model"}
 
     @classmethod
     def _from_object(
         cls,
         model: prior_model.Model,
     ):
         instance = cls()
         instance.cls = model.cls
-        instance._add_children(
-            model.items()
-            + [
-                (f"assertion_{i}", assertion)
-                for i, assertion in enumerate(model.assertions)
-            ]
-        )
+        instance._add_children(model.items() + extra_children(model))
         return instance
 
     def _make_instance(self):
         instance = object.__new__(prior_model.Model)
         instance.cls = self.cls
         instance._assertions = []
+
         return instance
 
 
 class Prior(Object):
     """
     A prior
     """
 
     __tablename__ = "prior"
 
     id = sa.Column(
         sa.Integer,
         sa.ForeignKey("object.id"),
         primary_key=True,
+        index=True,
     )
 
     __mapper_args__ = {"polymorphic_identity": "prior"}
 
     @classmethod
     def _from_object(cls, model: abstract.Prior):
         instance = cls()
```

### Comparing `autofit-2024.1.27.4/autofit/database/query/condition.py` & `autofit-2024.5.16.0/autofit/database/query/condition.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/database/query/junction.py` & `autofit-2024.5.16.0/autofit/database/query/junction.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/database/query/query/abstract.py` & `autofit-2024.5.16.0/autofit/database/query/query/abstract.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/database/query/query/attribute.py` & `autofit-2024.5.16.0/autofit/database/query/query/attribute.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/database/query/query/info.py` & `autofit-2024.5.16.0/autofit/database/query/query/info.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/database/query/query/named.py` & `autofit-2024.5.16.0/autofit/database/query/query/named.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/database/sqlalchemy_.py` & `autofit-2024.5.16.0/autofit/database/sqlalchemy_.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/example/model.py` & `autofit-2024.5.16.0/autofit/example/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,18 @@
         sigma
             The sigma value controlling the size of the Gaussian.
         """
         self.centre = centre
         self.normalization = normalization
         self.sigma = sigma
 
+    @property
+    def fwhm(self):
+        return 2 * np.sqrt(2 * np.log(2)) * self.sigma
+
     def _tree_flatten(self):
         return (self.centre, self.normalization, self.sigma), None
 
     @classmethod
     def _tree_unflatten(cls, aux_data, children):
         return Gaussian(*children)
```

### Comparing `autofit-2024.1.27.4/autofit/example/util.py` & `autofit-2024.5.16.0/autofit/example/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,8 +45,9 @@
     plt.ylabel(ylabel)
     if output_filename is None:
         plt.show()
     else:
         if not path.exists(output_path):
             os.makedirs(output_path)
         plt.savefig(output_path / f"{output_filename}.png")
-    plt.clf()
+    plt.clf()
+    plt.close()
```

### Comparing `autofit-2024.1.27.4/autofit/exc.py` & `autofit-2024.5.16.0/autofit/exc.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/fixtures.py` & `autofit-2024.5.16.0/autofit/fixtures.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/graphical/__init__.py` & `autofit-2024.5.16.0/autofit/graphical/__init__.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/graphical/declarative/abstract.py` & `autofit-2024.5.16.0/autofit/graphical/declarative/abstract.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,14 +147,15 @@
             kwargs["variable_labels"] = variable_labels
         if "factor_labels" not in kwargs:
             kwargs["factor_labels"] = factor_labels
         graph.draw_graph(
             **kwargs
         )
         plt.show()
+        plt.close()
 
     @property
     def plates(self):
         return self._plates
 
     def mean_field_approximation(self) -> EPMeanField:
         """
```

### Comparing `autofit-2024.1.27.4/autofit/graphical/declarative/collection.py` & `autofit-2024.5.16.0/autofit/graphical/declarative/collection.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/graphical/declarative/factor/abstract.py` & `autofit-2024.5.16.0/autofit/graphical/declarative/factor/abstract.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/graphical/declarative/factor/analysis.py` & `autofit-2024.5.16.0/autofit/graphical/declarative/factor/analysis.py`

 * *Files 6% similar despite different names*

```diff
@@ -89,15 +89,18 @@
     def __getstate__(self):
         return self.__dict__
 
     def __setstate__(self, state):
         self.__dict__.update(state)
 
     def __getattr__(self, item):
-        return getattr(self.prior_model, item)
+        try:
+            return super().__getattr__(item)
+        except AttributeError:
+            return getattr(self.prior_model, item)
 
     def name_for_variable(self, variable):
         path = ".".join(self.prior_model.path_for_prior(variable))
         return f"{self.name}.{path}"
 
     def visualize(
         self, paths: AbstractPaths, instance: ModelInstance, during_analysis: bool
```

### Comparing `autofit-2024.1.27.4/autofit/graphical/declarative/factor/hierarchical.py` & `autofit-2024.5.16.0/autofit/graphical/declarative/factor/hierarchical.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/graphical/declarative/factor/prior.py` & `autofit-2024.5.16.0/autofit/graphical/declarative/factor/prior.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/graphical/declarative/graph.py` & `autofit-2024.5.16.0/autofit/graphical/declarative/graph.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/graphical/declarative/result.py` & `autofit-2024.5.16.0/autofit/graphical/declarative/result.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,72 +7,63 @@
 from autofit.mapper.prior_model.abstract import AbstractPriorModel
 from autofit.mapper.prior_model.collection import Collection
 from autofit.non_linear.result import Result, AbstractResult
 from autofit.non_linear.samples.samples import Samples
 
 
 class HierarchicalResult(AbstractResult):
-    def __init__(
-            self,
-            results: List[AbstractResult]
-    ):
+    def __init__(self, results: List[AbstractResult]):
         """
         One true factor is created per each variable drawn from the declarative
         hierarchical factor. One result for each of those factors is in this
         collection.
 
         Parameters
         ----------
         results
             Results from hierarchical factor optimisations
         """
-        super().__init__()
+        super().__init__(samples_summary=None, paths=None)
         self.results = results
 
     @property
     def samples(self) -> Samples:
         """
         All samples from all underlying optimisations are summed together.
         """
-        return sum(
-            result.samples
-            for result
-            in self.results
-        )
+        return sum(result.samples for result in self.results)
 
     @property
     def model(self) -> AbstractPriorModel:
         """
         Priors with the same path in the model are combined by taking the
         product of their underlying messages. i.e. the product of the
         posteriors.
 
         The distribution model is returned.
         """
         return AbstractPriorModel.product(
-            result.model
-            for result
-            in self.results
+            result.model for result in self.results
         ).distribution_model
 
     @property
     def instance(self):
         """
         Return the instance (e.g. prior) describing the distribution
         from which samples are drawn.
         """
-        return super().instance.distribution_model
+        return self.samples.instance.distribution_model
 
 
 class EPResult:
     def __init__(
-            self,
-            ep_history: EPHistory,
-            declarative_factor,
-            updated_ep_mean_field: EPMeanField,
+        self,
+        ep_history: EPHistory,
+        declarative_factor,
+        updated_ep_mean_field: EPMeanField,
     ):
         """
         The result of an EP Optimisation including its history, a declarative
         representation of the optimised graph and the resultant EPMeanField
         which comprises factors and resultant approximations of variables.
 
         Parameters
@@ -91,32 +82,26 @@
     @property
     def model(self) -> Collection:
         """
         A collection populated with messages representing the posteriors of
         the EP Optimisation. Each item in the collection represents a single
         factor in the optimisation.
         """
-        collection = Collection({
-            factor.name: factor.prior_model
-            for factor
-            in self.declarative_factor.model_factors
-        })
+        collection = Collection(
+            {
+                factor.name: factor.prior_model
+                for factor in self.declarative_factor.model_factors
+            }
+        )
         arguments = {
-            prior: prior.with_message(
-                self.updated_ep_mean_field.mean_field[
-                    prior
-                ]
-            )
-            for prior
-            in collection.priors
+            prior: prior.with_message(self.updated_ep_mean_field.mean_field[prior])
+            for prior in collection.priors
         }
 
-        return collection.gaussian_prior_model_for_arguments(
-            arguments
-        )
+        return collection.gaussian_prior_model_for_arguments(arguments)
 
     @property
     def latest_results(self) -> List[Result]:
         """
         A list of results for all analysis and hierarchical factors.
         """
         return [
@@ -127,18 +112,15 @@
     @property
     def instance(self):
         """
         The median instance taken from the updated model
         """
         return self.model.instance_from_prior_medians()
 
-    def latest_for(
-            self,
-            factor: Union[Factor, HierarchicalFactor]
-    ) -> AbstractResult:
+    def latest_for(self, factor: Union[Factor, HierarchicalFactor]) -> AbstractResult:
         """
         Return the latest result for a factor.
 
         If the factor is hierarchical return the latest result for
         the first true factor (i.e. for one of the drawn variable)
 
         Parameters
@@ -149,12 +131,11 @@
         Returns
         -------
         The latest result for that factor
         """
         if isinstance(factor, HierarchicalFactor):
             results = [
                 self.ep_history[child_factor].latest_result
-                for child_factor
-                in factor.factors
+                for child_factor in factor.factors
             ]
             return HierarchicalResult(results)
         return self.ep_history[factor].latest_result
```

### Comparing `autofit-2024.1.27.4/autofit/graphical/expectation_propagation/ep_mean_field.py` & `autofit-2024.5.16.0/autofit/graphical/expectation_propagation/ep_mean_field.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/graphical/expectation_propagation/factor_optimiser.py` & `autofit-2024.5.16.0/autofit/graphical/expectation_propagation/factor_optimiser.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/graphical/expectation_propagation/history.py` & `autofit-2024.5.16.0/autofit/graphical/expectation_propagation/history.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/graphical/expectation_propagation/optimiser.py` & `autofit-2024.5.16.0/autofit/graphical/expectation_propagation/optimiser.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/graphical/expectation_propagation/stochastic.py` & `autofit-2024.5.16.0/autofit/graphical/expectation_propagation/stochastic.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/graphical/expectation_propagation/visualise.py` & `autofit-2024.5.16.0/autofit/graphical/expectation_propagation/visualise.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 import os
 from pathlib import Path
+import warnings
 
 import matplotlib.pyplot as plt
 
 from autofit.graphical.expectation_propagation.history import EPHistory
 
 logger = logging.getLogger(__name__)
 
@@ -42,8 +43,11 @@
         #         factor_history.evidences, label=f"{factor.name} evidence"
         #     )
         #     kl_plot.plot(
         #         factor_history.kl_divergences, label=f"{factor.name} divergence"
         #     )
         evidence_plot.legend()
         kl_plot.legend()
-        plt.savefig(str(self.output_path / "graph.png"))
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+            plt.savefig(str(self.output_path / "graph.png"))
+        plt.close()
```

### Comparing `autofit-2024.1.27.4/autofit/graphical/factor_graphs/abstract.py` & `autofit-2024.5.16.0/autofit/graphical/factor_graphs/abstract.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/graphical/factor_graphs/factor.py` & `autofit-2024.5.16.0/autofit/graphical/factor_graphs/factor.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/graphical/factor_graphs/graph.py` & `autofit-2024.5.16.0/autofit/graphical/factor_graphs/graph.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/graphical/factor_graphs/jacobians.py` & `autofit-2024.5.16.0/autofit/graphical/factor_graphs/jacobians.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/graphical/factor_graphs/transform.py` & `autofit-2024.5.16.0/autofit/graphical/factor_graphs/transform.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/graphical/laplace/line_search.py` & `autofit-2024.5.16.0/autofit/graphical/laplace/line_search.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/graphical/laplace/newton.py` & `autofit-2024.5.16.0/autofit/graphical/laplace/newton.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/graphical/laplace/optimiser.py` & `autofit-2024.5.16.0/autofit/graphical/laplace/optimiser.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/graphical/mean_field.py` & `autofit-2024.5.16.0/autofit/graphical/mean_field.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/graphical/utils.py` & `autofit-2024.5.16.0/autofit/graphical/utils.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/interpolator/abstract.py` & `autofit-2024.5.16.0/autofit/interpolator/abstract.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/interpolator/covariance.py` & `autofit-2024.5.16.0/autofit/interpolator/covariance.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/interpolator/query.py` & `autofit-2024.5.16.0/autofit/interpolator/query.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/jax_wrapper.py` & `autofit-2024.5.16.0/autofit/jax_wrapper.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/mapper/identifier.py` & `autofit-2024.5.16.0/autofit/mapper/identifier.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/mapper/mock/mock_model.py` & `autofit-2024.5.16.0/autofit/mapper/mock/mock_model.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/mapper/model.py` & `autofit-2024.5.16.0/autofit/mapper/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,15 +186,15 @@
                 instance = getattr(instance, name)
         return instance
 
     @frozen_cache
     def path_instance_tuples_for_class(
         self,
         cls: Union[Tuple, Type],
-        ignore_class: bool = None,
+        ignore_class: Optional[type] = None,
         ignore_children: bool = True,
     ):
         """
         Tuples containing the path tuple and instance for every instance of the class
         in the model tree.
 
         Parameters
@@ -282,15 +282,18 @@
             )
             if issubclass(model.cls, cls)
             and (include_zero_dimension or model.prior_count > 0)
         ]
 
     @frozen_cache
     def attribute_tuples_with_type(
-        self, class_type, ignore_class=None, ignore_children=True
+        self,
+        class_type,
+        ignore_class=None,
+        ignore_children=True,
     ) -> List[tuple]:
         """
         Tuples describing the name and instance for attributes in the model
         with a given type, recursively.
 
         Parameters
         ----------
@@ -304,15 +307,17 @@
         Returns
         -------
         Tuples containing the name and instance of each attribute with the type
         """
         return [
             (path[-1] if len(path) > 0 else "", value)
             for path, value in self.path_instance_tuples_for_class(
-                class_type, ignore_class=ignore_class, ignore_children=ignore_children
+                class_type,
+                ignore_class=ignore_class,
+                ignore_children=ignore_children,
             )
         ]
 
 
 @DynamicRecursionCache()
 def path_instances_of_class(
     obj,
```

### Comparing `autofit-2024.1.27.4/autofit/mapper/model_mapper.py` & `autofit-2024.5.16.0/autofit/mapper/model_mapper.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/mapper/model_object.py` & `autofit-2024.5.16.0/autofit/mapper/model_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,14 +148,15 @@
         An instance
         """
         from autofit.mapper.prior_model.collection import Collection
         from autofit.mapper.prior_model.prior_model import Model
         from autofit.mapper.prior.abstract import Prior
         from autofit.mapper.prior.tuple_prior import TuplePrior
         from autofit.mapper.prior.arithmetic.compound import Compound
+        from autofit.mapper.prior.arithmetic.compound import ModifiedPrior
 
         if isinstance(d, list):
             return [
                 from_dict(
                     value,
                     reference=dereference(reference, str(index)),
                     loaded_ids=loaded_ids,
@@ -191,14 +192,20 @@
             instance = TuplePrior()
         elif type_ == "compound":
             return Compound.from_dict(
                 d,
                 reference=dereference(reference, "assertion"),
                 loaded_ids=loaded_ids,
             )
+        elif type_ == "modified":
+            return ModifiedPrior.from_dict(
+                d,
+                reference=dereference(reference, "prior"),
+                loaded_ids=loaded_ids,
+            )
         elif type_ == "dict":
             return {
                 key: from_dict(
                     value,
                     reference=dereference(reference, key),
                     loaded_ids=loaded_ids,
                 )
```

### Comparing `autofit-2024.1.27.4/autofit/mapper/operator.py` & `autofit-2024.5.16.0/autofit/mapper/operator.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/mapper/prior/abstract.py` & `autofit-2024.5.16.0/autofit/mapper/prior/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import random
 from abc import ABC, abstractmethod
 from copy import copy
 from typing import Union, Tuple, Optional, Dict
 
 from autoconf import conf
-from autofit import exc
+from autofit import exc, jax_wrapper
 from autofit.mapper.prior.arithmetic import ArithmeticMixin
 from autofit.mapper.prior.deferred import DeferredArgument
 from autofit.mapper.variable import Variable
 
 epsilon = 1e-14
 
 
@@ -111,14 +111,18 @@
     def factor(self):
         """
         A callable PDF used as a factor in factor graphs
         """
         return self.message.factor
 
     def assert_within_limits(self, value):
+
+        if jax_wrapper.use_jax:
+            return
+
         if not (self.lower_limit <= value <= self.upper_limit):
             raise exc.PriorLimitException(
                 "The physical value {} for a prior "
                 "was not within its limits {}, {}".format(
                     value, self.lower_limit, self.upper_limit
                 )
             )
@@ -164,15 +168,20 @@
         A physical value, mapped from the unit value accoridng to the prior.
         """
         result = self.message.value_for(unit)
         if not ignore_prior_limits:
             self.assert_within_limits(result)
         return result
 
-    def instance_for_arguments(self, arguments):
+    def instance_for_arguments(
+        self,
+        arguments,
+        ignore_assertions=False,
+    ):
+        _ = ignore_assertions
         return arguments[self]
 
     def project(self, samples, weights):
         result = copy(self)
         result.message = self.message.project(
             samples=samples,
             log_weight_list=weights,
```

### Comparing `autofit-2024.1.27.4/autofit/mapper/prior/arithmetic/arithmetic.py` & `autofit-2024.5.16.0/autofit/mapper/prior/arithmetic/arithmetic.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/mapper/prior/arithmetic/assertion.py` & `autofit-2024.5.16.0/autofit/mapper/prior/arithmetic/assertion.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,65 +20,87 @@
         return CompoundAssertion(self, self._left >= other)
 
     def __le__(self, other):
         return CompoundAssertion(self, self._right <= other)
 
 
 class GreaterThanLessThanAssertion(ComparisonAssertion):
-    def _instance_for_arguments(self, arguments):
+    def _instance_for_arguments(self, arguments, ignore_assertions=False):
         """
         Assert that the value in the dictionary associated with the lower
         prior is lower than the value associated with the greater prior.
 
         Parameters
         ----------
         arguments
             A dictionary mapping priors to physical values.
 
         Raises
         ------
         FitException
             If the assertion is not met
         """
-        lower = self.left_for_arguments(arguments)
-        greater = self.right_for_arguments(arguments)
+        lower = self.left_for_arguments(
+            arguments,
+            ignore_assertions=ignore_assertions,
+        )
+        greater = self.right_for_arguments(
+            arguments,
+            ignore_assertions=ignore_assertions,
+        )
         return lower < greater
 
 
 class GreaterThanLessThanEqualAssertion(ComparisonAssertion):
-    def _instance_for_arguments(self, arguments):
+    def _instance_for_arguments(
+        self,
+        arguments,
+        ignore_assertions=False,
+    ):
         """
         Assert that the value in the dictionary associated with the lower
         prior is lower than the value associated with the greater prior.
 
         Parameters
         ----------
         arguments
             A dictionary mapping priors to physical values.
 
         Raises
         ------
         FitException
             If the assertion is not met
         """
-        return self.left_for_arguments(arguments) <= self.right_for_arguments(arguments)
+        return self.left_for_arguments(
+            arguments,
+            ignore_assertions=ignore_assertions,
+        ) <= self.right_for_arguments(
+            arguments,
+            ignore_assertions=ignore_assertions,
+        )
 
 
 class CompoundAssertion(AbstractPriorModel, Compound):
     def __init__(self, assertion_1, assertion_2, name=""):
         super().__init__()
         self.assertion_1 = assertion_1
         self.assertion_2 = assertion_2
         self._name = name
 
-    def _instance_for_arguments(self, arguments):
+    def _instance_for_arguments(
+        self,
+        arguments,
+        ignore_assertions=False,
+    ):
         return self.assertion_1.instance_for_arguments(
             arguments,
+            ignore_assertions,
         ) and self.assertion_2.instance_for_arguments(
             arguments,
+            ignore_assertions,
         )
 
     def dict(self) -> dict:
         return {
             "type": "compound",
             "compound_type": self.__class__.__name__,
             "assertion_1": self.assertion_1.dict(),
```

### Comparing `autofit-2024.1.27.4/autofit/mapper/prior/arithmetic/compound.py` & `autofit-2024.5.16.0/autofit/mapper/prior/arithmetic/compound.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import logging
 from abc import ABC
 from copy import copy
 from typing import Optional, Dict
 
 import numpy as np
 
+from autofit.mapper.model_object import dereference
 from autofit.mapper.prior.arithmetic import ArithmeticMixin
 from autofit.mapper.prior_model.abstract import AbstractPriorModel
 
 logger = logging.getLogger(__name__)
 
 
 def retrieve_name(var):
@@ -137,125 +138,232 @@
             pass
         try:
             new.right = new.right.gaussian_prior_model_for_arguments(arguments)
         except AttributeError:
             pass
         return new
 
-    def left_for_arguments(self, arguments: dict):
+    def left_for_arguments(
+        self,
+        arguments: dict,
+        ignore_assertions=False,
+    ):
         """
         Instantiate the left object.
 
         Parameters
         ----------
         arguments
             A dictionary mapping priors to values
+        ignore_assertions
+            If True, ignore assertions
 
         Returns
         -------
         A value for the left object
         """
         try:
             return self._left.instance_for_arguments(
                 arguments,
+                ignore_assertions=ignore_assertions,
             )
         except AttributeError:
             return self._left
 
-    def right_for_arguments(self, arguments: dict):
+    def right_for_arguments(
+        self,
+        arguments: dict,
+        ignore_assertions=False,
+    ):
         """
         Instantiate the right object.
 
         Parameters
         ----------
         arguments
             A dictionary mapping priors to values
+        ignore_assertions
+            If True, ignore assertions
 
         Returns
         -------
         A value for the right object
         """
         try:
             return self._right.instance_for_arguments(
                 arguments,
+                ignore_assertions=ignore_assertions,
             )
         except AttributeError:
             return self._right
 
+    def __add__(self, other):
+        return ArithmeticMixin.__add__(self, other)
+
 
 class SumPrior(CompoundPrior):
     """
     The sum of two objects, computed after realisation.
     """
 
-    def _instance_for_arguments(self, arguments):
-        return self.left_for_arguments(arguments) + self.right_for_arguments(arguments)
+    def _instance_for_arguments(
+        self,
+        arguments,
+        ignore_assertions=False,
+    ):
+        return self.left_for_arguments(
+            arguments,
+            ignore_assertions=ignore_assertions,
+        ) + self.right_for_arguments(
+            arguments,
+            ignore_assertions=ignore_assertions,
+        )
 
     def __str__(self):
         return f"{self._left} + {self._right}"
 
 
 class MultiplePrior(CompoundPrior):
     """
     The multiple of two objects, computed after realisation.
     """
 
     def __str__(self):
         return f"{self._left} * {self._right}"
 
-    def _instance_for_arguments(self, arguments):
-        return self.left_for_arguments(arguments) * self.right_for_arguments(arguments)
+    def _instance_for_arguments(
+        self,
+        arguments,
+        ignore_assertions=False,
+    ):
+        return self.left_for_arguments(
+            arguments,
+            ignore_assertions=ignore_assertions,
+        ) * self.right_for_arguments(
+            arguments,
+            ignore_assertions=ignore_assertions,
+        )
 
 
 class DivisionPrior(CompoundPrior):
     """
     One object divided by another, computed after realisation
     """
 
-    def _instance_for_arguments(self, arguments):
-        return self.left_for_arguments(arguments) / self.right_for_arguments(arguments)
+    def _instance_for_arguments(
+        self,
+        arguments,
+        ignore_assertions=False,
+    ):
+        return self.left_for_arguments(
+            arguments,
+            ignore_assertions=ignore_assertions,
+        ) / self.right_for_arguments(
+            arguments,
+            ignore_assertions=ignore_assertions,
+        )
 
 
 class FloorDivPrior(CompoundPrior):
     """
     One object divided by another and floored, computed after realisation.
     """
 
-    def _instance_for_arguments(self, arguments):
-        return self.left_for_arguments(arguments) // self.right_for_arguments(arguments)
+    def _instance_for_arguments(
+        self,
+        arguments,
+        ignore_assertions=False,
+    ):
+        return self.left_for_arguments(
+            arguments,
+            ignore_assertions=ignore_assertions,
+        ) // self.right_for_arguments(
+            arguments,
+            ignore_assertions=ignore_assertions,
+        )
 
 
 class ModPrior(CompoundPrior):
     """
     The modulus of a pair of objects, computed after realisation.
     """
 
-    def _instance_for_arguments(self, arguments):
-        return self.left_for_arguments(arguments) % self.right_for_arguments(arguments)
+    def _instance_for_arguments(
+        self,
+        arguments,
+        ignore_assertions=False,
+    ):
+        return self.left_for_arguments(
+            arguments,
+            ignore_assertions=ignore_assertions,
+        ) % self.right_for_arguments(
+            arguments,
+            ignore_assertions=ignore_assertions,
+        )
 
 
 class PowerPrior(CompoundPrior):
     """
     One object to the power of another, computed after realisation.
     """
 
-    def _instance_for_arguments(self, arguments):
-        return self.left_for_arguments(arguments) ** self.right_for_arguments(arguments)
+    def _instance_for_arguments(
+        self,
+        arguments,
+        ignore_assertions=False,
+    ):
+        return self.left_for_arguments(
+            arguments,
+            ignore_assertions=ignore_assertions,
+        ) ** self.right_for_arguments(
+            arguments,
+            ignore_assertions=ignore_assertions,
+        )
 
 
-class ModifiedPrior(AbstractPriorModel, ABC, ArithmeticMixin):
-    def __init__(self, prior):
+class ModifiedPrior(AbstractPriorModel, ABC, ArithmeticMixin, Compound):
+    def __init__(self, prior, name=None):
         super().__init__()
-        self._prior_name = retrieve_name(prior)
+        self._prior_name = name or retrieve_name(prior)
 
         if self._prior_name == "prior":
             self._prior_name = "prior_"
 
         self.prior = prior
 
+    def dict(self):
+        return {
+            "type": "modified",
+            "modified_type": self.__class__.__name__,
+            "name": self._prior_name,
+            "prior": self.prior.dict()
+            if isinstance(self.prior, AbstractPriorModel)
+            else self.prior,
+        }
+
+    @classmethod
+    def from_dict(
+        cls,
+        d,
+        reference: Optional[Dict[str, str]] = None,
+        loaded_ids: Optional[dict] = None,
+    ):
+        modified_type = d.pop("modified_type")
+        for subclass in cls.descendants():
+            if subclass.__name__ == modified_type:
+                return subclass(
+                    AbstractPriorModel.from_dict(
+                        d["prior"],
+                        reference=dereference(reference, "prior"),
+                        loaded_ids=loaded_ids,
+                    ),
+                    name=d["name"],
+                )
+        raise ValueError(f"Modified type {modified_type} not recognised")
+
     def __add__(self, other):
         return ArithmeticMixin.__add__(self, other)
 
     @property
     def cls(self):
         return self.prior.cls
 
@@ -277,50 +385,70 @@
 
 
 class NegativePrior(ModifiedPrior):
     """
     The negation of an object, computed after realisation.
     """
 
-    def _instance_for_arguments(self, arguments):
+    def _instance_for_arguments(
+        self,
+        arguments,
+        ignore_assertions=False,
+    ):
         return -self.prior.instance_for_arguments(
             arguments,
+            ignore_assertions=ignore_assertions,
         )
 
 
 class AbsolutePrior(ModifiedPrior):
     """
     The absolute value of an object, computed after realisation.
     """
 
-    def _instance_for_arguments(self, arguments):
+    def _instance_for_arguments(
+        self,
+        arguments,
+        ignore_assertions=False,
+    ):
         return abs(
             self.prior.instance_for_arguments(
                 arguments,
+                ignore_assertions=ignore_assertions,
             )
         )
 
 
 class Log(ModifiedPrior):
     """
     The natural logarithm of an object, computed after realisation.
     """
 
-    def _instance_for_arguments(self, arguments):
+    def _instance_for_arguments(
+        self,
+        arguments,
+        ignore_assertions=False,
+    ):
         return np.log(
             self.prior.instance_for_arguments(
                 arguments,
+                ignore_assertions=ignore_assertions,
             )
         )
 
 
 class Log10(ModifiedPrior):
     """
     The base10 logarithm of an object, computed after realisation.
     """
 
-    def _instance_for_arguments(self, arguments):
+    def _instance_for_arguments(
+        self,
+        arguments,
+        ignore_assertions=False,
+    ):
         return np.log10(
             self.prior.instance_for_arguments(
                 arguments,
+                ignore_assertions=ignore_assertions,
             )
         )
```

### Comparing `autofit-2024.1.27.4/autofit/mapper/prior/deferred.py` & `autofit-2024.5.16.0/autofit/mapper/prior/deferred.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/mapper/prior/gaussian.py` & `autofit-2024.5.16.0/autofit/mapper/prior/gaussian.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/mapper/prior/log_gaussian.py` & `autofit-2024.5.16.0/autofit/mapper/prior/uniform.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,103 +1,113 @@
+from autofit.jax_wrapper import register_pytree_node_class
 from typing import Optional
 
-from autofit.messages.normal import NormalMessage
+from autofit.messages.normal import UniformNormalMessage
 from .abstract import Prior
+from .abstract import epsilon
 from ...messages.composed_transform import TransformedMessage
-from ...messages.transform import log_transform
+from ...messages.transform import LinearShiftTransform
 
 
-class LogGaussianPrior(Prior):
-    __identifier_fields__ = ("lower_limit", "upper_limit", "mean", "sigma")
-    __database_args__ = ("mean", "sigma", "lower_limit", "upper_limit", "id_")
+@register_pytree_node_class
+class UniformPrior(Prior):
+    __identifier_fields__ = ("lower_limit", "upper_limit")
 
     def __init__(
         self,
-        mean: float,
-        sigma: float,
         lower_limit: float = 0.0,
-        upper_limit: float = float("inf"),
+        upper_limit: float = 1.0,
         id_: Optional[int] = None,
     ):
         """
-        A prior with a log base 10 uniform distribution, defined between a lower limit and upper limit.
+        A prior with a uniform distribution, defined between a lower limit and upper limit.
 
         The conversion of an input unit value, ``u``, to a physical value, ``p``, via the prior is as follows:
 
         .. math::
 
-            p = \mu + (\sigma * sqrt(2) * erfcinv(2.0 * (1.0 - u))
-
-        For example for ``prior = LogGaussianPrior(mean=1.0, sigma=2.0)``, an
+        For example for ``prior = UniformPrior(lower_limit=0.0, upper_limit=2.0)``, an
         input ``prior.value_for(unit=0.5)`` is equal to 1.0.
 
         [Rich describe how this is done via message]
 
         Parameters
         ----------
-        mean
-            The mean of the Gaussian distribution defining the prior.
-        sigma
-            The sigma value of the Gaussian distribution defining the prior.
         lower_limit
-            A lower limit of the Gaussian distribution; physical values below this value are rejected.
+            The lower limit of the uniform distribution defining the prior.
         upper_limit
-            A upper limit of the Gaussian distribution; physical values below this value are rejected.
+            The upper limit of the uniform distribution defining the prior.
 
         Examples
         --------
 
-        prior = af.LogGaussianPrior(mean=1.0, sigma=2.0, lower_limit=0.0, upper_limit=2.0)
+        prior = af.UniformPrior(lower_limit=0.0, upper_limit=2.0)
 
-        physical_value = prior.value_for(unit=0.5)
+        physical_value = prior.value_for(unit=0.2)
         """
+
         lower_limit = float(lower_limit)
         upper_limit = float(upper_limit)
 
-        self.mean = mean
-        self.sigma = sigma
-
         message = TransformedMessage(
-            NormalMessage(mean, sigma),
-            log_transform,
+            UniformNormalMessage,
+            LinearShiftTransform(shift=lower_limit, scale=upper_limit - lower_limit),
+            lower_limit=lower_limit,
+            upper_limit=upper_limit,
         )
-
         super().__init__(
-            message=message,
+            message,
             lower_limit=lower_limit,
             upper_limit=upper_limit,
             id_=id_,
         )
 
-    def _new_for_base_message(self, message):
-        """
-        Create a new instance of this wrapper but change the parameters used
-        to instantiate the underlying message. This is useful for retaining
-        the same transform stack after recreating the underlying message during
-        projection.
-        """
-        return LogGaussianPrior(
-            *message.parameters,
-            lower_limit=self.lower_limit,
-            upper_limit=self.upper_limit,
-            id_=self.instance().id,
-        )
+    def tree_flatten(self):
+        return (self.lower_limit, self.upper_limit), (self.id,)
+
+    def logpdf(self, x):
+        # TODO: handle x as a numpy array
+        if x == self.lower_limit:
+            x += epsilon
+        elif x == self.upper_limit:
+            x -= epsilon
+        return self.message.logpdf(x)
+
+    @property
+    def parameter_string(self) -> str:
+        return f"lower_limit = {self.lower_limit}, upper_limit = {self.upper_limit}"
 
     def value_for(self, unit: float, ignore_prior_limits: bool = False) -> float:
         """
-        Return a physical value for a value between 0 and 1 with the transformation
-        described by this prior.
+        Returns a physical value from an input unit value according to the limits of the uniform prior.
 
         Parameters
         ----------
         unit
             A unit value between 0 and 1.
 
         Returns
         -------
-        A physical value, mapped from the unit value accoridng to the prior.
+        value
+            The unit value mapped to a physical value according to the prior.
+
+        Examples
+        --------
+
+        prior = af.UniformPrior(lower_limit=0.0, upper_limit=2.0)
+
+        physical_value = prior.value_for(unit=0.2)
         """
-        return super().value_for(unit, ignore_prior_limits=ignore_prior_limits)
+        return float(round(
+            super().value_for(unit, ignore_prior_limits=ignore_prior_limits), 14
+        ))
 
-    @property
-    def parameter_string(self) -> str:
-        return f"mean = {self.mean}, sigma = {self.sigma}"
+    def log_prior_from_value(self, value):
+        """
+        Returns the log prior of a physical value, so the log likelihood of a model evaluation can be converted to a
+        posterior as log_prior + log_likelihood.
+
+        This is used by certain non-linear searches (e.g. Emcee) in the log likelihood function evaluation.
+
+        For a UniformPrior this is always zero, provided the value is between the lower and upper limit.
+        """
+        return 0.0
```

### Comparing `autofit-2024.1.27.4/autofit/mapper/prior/log_uniform.py` & `autofit-2024.5.16.0/autofit/mapper/prior/log_uniform.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,16 +94,15 @@
         return cls(
             lower_limit=max(0.000001, lower_limit),
             upper_limit=upper_limit,
         )
 
     __identifier_fields__ = ("lower_limit", "upper_limit")
 
-    @staticmethod
-    def log_prior_from_value(value) -> float:
+    def log_prior_from_value(self, value) -> float:
         """
         Returns the log prior of a physical value, so the log likelihood of a model evaluation can be converted to a
         posterior as log_prior + log_likelihood.
 
         This is used by certain non-linear searches (e.g. Emcee) in the log likelihood function evaluation.
 
         Parameters
```

### Comparing `autofit-2024.1.27.4/autofit/mapper/prior/tuple_prior.py` & `autofit-2024.5.16.0/autofit/mapper/prior/tuple_prior.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/mapper/prior/uniform.py` & `autofit-2024.5.16.0/autofit/mapper/prior/log_gaussian.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,115 +1,114 @@
-from autofit.jax_wrapper import register_pytree_node_class
 from typing import Optional
 
-from autofit.messages.normal import UniformNormalMessage
+import numpy as np
+
+from autofit.messages.normal import NormalMessage
 from .abstract import Prior
-from .abstract import epsilon
 from ...messages.composed_transform import TransformedMessage
-from ...messages.transform import LinearShiftTransform
+from ...messages.transform import log_transform
 
 
-@register_pytree_node_class
-class UniformPrior(Prior):
-    __identifier_fields__ = ("lower_limit", "upper_limit")
+class LogGaussianPrior(Prior):
+    __identifier_fields__ = ("lower_limit", "upper_limit", "mean", "sigma")
+    __database_args__ = ("mean", "sigma", "lower_limit", "upper_limit", "id_")
 
     def __init__(
         self,
+        mean: float,
+        sigma: float,
         lower_limit: float = 0.0,
-        upper_limit: float = 1.0,
+        upper_limit: float = float("inf"),
         id_: Optional[int] = None,
     ):
         """
-        A prior with a uniform distribution, defined between a lower limit and upper limit.
+        A prior for a variable whose logarithm is gaussian distributed. Work in natural log.
 
         The conversion of an input unit value, ``u``, to a physical value, ``p``, via the prior is as follows:
 
         .. math::
 
-        For example for ``prior = UniformPrior(lower_limit=0.0, upper_limit=2.0)``, an
+            p = \mu + (\sigma * sqrt(2) * erfcinv(2.0 * (1.0 - u))
+
+        For example for ``prior = LogGaussianPrior(mean=1.0, sigma=2.0)``, an
         input ``prior.value_for(unit=0.5)`` is equal to 1.0.
 
         [Rich describe how this is done via message]
 
         Parameters
         ----------
+        mean
+            The *natural log* of the distribution's mean.
+        sigma
+            The spread of this distribution in *natural log* space, e.g. sigma=1.0 means P(ln x) has a
+            standard deviation of 1.
         lower_limit
-            The lower limit of the uniform distribution defining the prior.
+            A lower limit in *real space* (not log); physical values below this are rejected.
         upper_limit
-            The upper limit of the uniform distribution defining the prior.
+            A upper limit in *real space* (not log); physical values above this are rejected.
 
         Examples
         --------
 
-        prior = af.UniformPrior(lower_limit=0.0, upper_limit=2.0)
+        prior = af.LogGaussianPrior(mean=1.0, sigma=2.0, lower_limit=0.0, upper_limit=2.0)
 
-        physical_value = prior.value_for(unit=0.2)
+        physical_value = prior.value_for(unit=0.5)
         """
-
         lower_limit = float(lower_limit)
         upper_limit = float(upper_limit)
 
+        self.mean = mean
+        self.sigma = sigma
+
         message = TransformedMessage(
-            UniformNormalMessage,
-            LinearShiftTransform(shift=lower_limit, scale=upper_limit - lower_limit),
-            lower_limit=lower_limit,
-            upper_limit=upper_limit,
+            NormalMessage(mean, sigma),
+            log_transform,
         )
+
         super().__init__(
-            message,
+            message=message,
             lower_limit=lower_limit,
             upper_limit=upper_limit,
             id_=id_,
         )
 
-    def tree_flatten(self):
-        return (self.lower_limit, self.upper_limit), (self.id,)
-
-    def logpdf(self, x):
-        # TODO: handle x as a numpy array
-        if x == self.lower_limit:
-            x += epsilon
-        elif x == self.upper_limit:
-            x -= epsilon
-        return self.message.logpdf(x)
-
-    @property
-    def parameter_string(self) -> str:
-        return f"lower_limit = {self.lower_limit}, upper_limit = {self.upper_limit}"
+    def _new_for_base_message(self, message):
+        """
+        Create a new instance of this wrapper but change the parameters used
+        to instantiate the underlying message. This is useful for retaining
+        the same transform stack after recreating the underlying message during
+        projection.
+        """
+        return LogGaussianPrior(
+            *message.parameters,
+            lower_limit=self.lower_limit,
+            upper_limit=self.upper_limit,
+            id_=self.instance().id,
+        )
 
     def value_for(self, unit: float, ignore_prior_limits: bool = False) -> float:
         """
-        Returns a physical value from an input unit value according to the limits of the uniform prior.
+        Return a physical value for a value between 0 and 1 with the transformation
+        described by this prior.
 
         Parameters
         ----------
         unit
             A unit value between 0 and 1.
 
         Returns
         -------
-        value
-            The unit value mapped to a physical value according to the prior.
-
-        Examples
-        --------
-
-        prior = af.UniformPrior(lower_limit=0.0, upper_limit=2.0)
-
-        physical_value = prior.value_for(unit=0.2)
+        A physical value, mapped from the unit value accoridng to the prior.
         """
-        return round(
-            super().value_for(unit, ignore_prior_limits=ignore_prior_limits), 14
-        )
+        return super().value_for(unit, ignore_prior_limits=ignore_prior_limits)
 
-    # noinspection PyUnusedLocal
-    @staticmethod
-    def log_prior_from_value(value):
-        """
-        Returns the log prior of a physical value, so the log likelihood of a model evaluation can be converted to a
-        posterior as log_prior + log_likelihood.
+    @property
+    def parameter_string(self) -> str:
+        return f"mean = {self.mean}, sigma = {self.sigma}"
 
-        This is used by certain non-linear searches (e.g. Emcee) in the log likelihood function evaluation.
+    def log_prior_from_value(self, value):
+        if value <= 0:
+            return float("-inf")
 
-        For a UniformPrior this is always zero, provided the value is between the lower and upper limit.
-        """
-        return 0.0
+        return self.message.base_message.log_prior_from_value(np.log(value)) - np.log(
+            value
+        )
```

### Comparing `autofit-2024.1.27.4/autofit/mapper/prior/width_modifier.py` & `autofit-2024.5.16.0/autofit/mapper/prior/width_modifier.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/mapper/prior_model/abstract.py` & `autofit-2024.5.16.0/autofit/mapper/prior_model/abstract.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,1886 +1,1878 @@
-import copy
-import inspect
-import json
-import logging
-import random
-import types
-from collections import defaultdict
-from typing import Tuple, Optional, Dict, List, Iterable, Generator, Union, Type
-
-import numpy as np
-
-from autoconf import conf
-from autoconf.exc import ConfigException
-from autofit import exc
-from autofit.mapper import model
-from autofit.mapper.model import AbstractModel, frozen_cache
-from autofit.mapper.prior import GaussianPrior
-from autofit.mapper.prior import UniformPrior
-from autofit.mapper.prior.abstract import Prior
-from autofit.mapper.prior.deferred import DeferredArgument
-from autofit.mapper.prior.tuple_prior import TuplePrior
-from autofit.mapper.prior.width_modifier import WidthModifier
-from autofit.mapper.prior_model.attribute_pair import DeferredNameValue
-from autofit.mapper.prior_model.attribute_pair import (
-    cast_collection,
-    PriorNameValue,
-    InstanceNameValue,
-)
-from autofit.mapper.prior_model.recursion import DynamicRecursionCache
-from autofit.mapper.prior_model.util import PriorModelNameValue
-from autofit.text import formatter as frm
-from autofit.text.formatter import TextFormatter
-from autofit.tools.util import info_whitespace
-from autofit.tools.util import split_paths
-
-logger = logging.getLogger(__name__)
-
-
-class Limits:
-    @staticmethod
-    def for_class_and_attributes_name(cls, attribute_name):
-        limit_dict = conf.instance.prior_config.for_class_and_suffix_path(
-            cls, [attribute_name, "gaussian_limits"]
-        )
-        return limit_dict["lower"], limit_dict["upper"]
-
-
-class TuplePathModifier:
-    def __init__(self, model_: "AbstractPriorModel"):
-        """
-        Modifies paths to priors contained in tuples.
-
-        When a tuple is found in a signature a PriorTuple is created.
-
-        The true path to a variable in the tuple is
-        ("some", "preamble", "tuple_name", "tuple_name_0")
-
-        Where 0 is the index of the tuple member. "tuple_name" must be
-        removed from this path for some uses.
-
-        When called, instances of this class remove the name of the tuple
-        i.e:
-        -> ("some", "preamble", "tuple_name_0")
-
-        Parameters
-        ----------
-        model_
-        """
-        tuple_priors = model_.path_instance_tuples_for_class(TuplePrior)
-        try:
-            self.tuple_paths, _ = zip(*tuple_priors)
-        except ValueError:
-            self.tuple_paths = None
-
-    def __call__(self, path):
-        if self.tuple_paths is not None:
-            if path[:-1] in self.tuple_paths:
-                return path[:-2] + (path[-1],)
-        return path
-
-
-Path = Tuple[str, ...]
-
-
-class MeanField:
-    def __init__(self, prior_model: "AbstractPriorModel"):
-        """
-        Implements same interface as graphical code
-
-        Parameters
-        ----------
-        prior_model
-        """
-        self.prior_model = prior_model
-
-    def __getitem__(self, item):
-        """
-        Retrieve a prior by a prior with the same id
-        """
-        for prior in self.prior_model.priors:
-            if prior == item:
-                return prior
-        raise KeyError(f"Could not find {item} in model")
-
-
-def paths_to_tree(paths: List[Tuple[str, ...]], tree: Optional[dict] = None) -> dict:
-    """
-    Recursively convert a list of paths to a tree structure where common paths
-    are matched.
-
-    Parameters
-    ----------
-    paths
-        A list of paths to attributes in the model.
-    tree
-        A tree already embedded in a parent tree.
-
-    Returns
-    -------
-    A tree with depth max(map(len, paths))
-
-    Examples
-    --------
-    paths_to_tree([
-        ("one", "two", "three"),
-        ("one", "two", "four"),
-    ])
-
-    gives
-
-    {
-        "one": {
-            "two": {
-                "three": {},
-                "four": {}
-            }
-        }
-    }
-    """
-    tree = tree or dict()
-    for path in paths:
-        if len(path) == 0:
-            return tree
-        first, *rest = path
-        if first not in tree:
-            child = dict()
-            tree[first] = child
-        tree[first] = paths_to_tree([rest], tree=tree[first])
-    return tree
-
-
-class AbstractPriorModel(AbstractModel):
-    """
-    Abstract model that maps a set of priors to a particular class. Must be
-    overridden by any prior model so that the model mapper recognises its prior \
-    model attributes.
-    @DynamicAttrs
-    """
-
-    def __init__(self, label=None):
-        super().__init__(label=label)
-        self._assertions = list()
-
-    @property
-    def assertions(self):
-        return self._assertions
-
-    @assertions.setter
-    def assertions(self, assertions):
-        self._assertions = assertions
-
-    def check_assertions(self, arguments: Dict[Prior, float]):
-        """
-        Check that all assertions are satisfied by the given arguments.
-
-        Parameters
-        ----------
-        arguments
-            A dictionary mapping priors to values
-
-        Raises
-        ------
-        FitException
-            If any assertion is not satisfied
-        """
-        failed_assertions = [
-            assertion
-            for assertion in self._assertions
-            if assertion is False
-            or assertion is not True
-            and not assertion.instance_for_arguments(
-                arguments,
-            )
-        ]
-        number_of_failed_assertions = len(failed_assertions)
-        if number_of_failed_assertions > 0:
-            name_string = "\n".join(
-                [
-                    assertion.name
-                    for assertion in failed_assertions
-                    if hasattr(assertion, "name") and assertion.name is not None
-                ]
-            )
-            raise exc.FitException(
-                f"{number_of_failed_assertions} assertions failed!\n{name_string}"
-            )
-
-    def cast(
-        self,
-        value_dict: Dict["AbstractModel", dict],
-        new_class: type,
-    ) -> "AbstractPriorModel":
-        """
-        Cast models to a new type. Allows selected models in within this
-        model to be given a new type and new arguments.
-
-        Parameters
-        ----------
-        value_dict
-            A dictionary mapping models to dictionaries of argument overrides
-        new_class
-            A new class to which specified models should be converted
-
-        Returns
-        -------
-        A model where specified child models have been updated to a new class
-        and new arguments
-        """
-        from .prior_model import Model
-
-        updated = self
-
-        for path, prior_model in self.path_instance_tuples_for_class(Model):
-            try:
-                model_value_dict = value_dict[prior_model]
-                argument_dict = {
-                    **dict(prior_model.direct_prior_tuples),
-                    **dict(prior_model.direct_tuples_with_type(float)),
-                    **model_value_dict,
-                }
-                updated = updated.replacing_for_path(
-                    path, Model(new_class, **argument_dict)
-                )
-
-            except KeyError:
-                pass
-
-        return updated
-
-    def without_attributes(self) -> "AbstractModel":
-        """
-        Returns a copy of this object with all priors, prior models and
-        constants removed.
-        """
-        without_attributes = copy.copy(self)
-        for key in self.__dict__:
-            if not (key.startswith("_") or key in ("cls", "id")):
-                delattr(without_attributes, key)
-        return without_attributes
-
-    def _with_paths(self, tree: dict) -> "AbstractModel":
-        """
-        Recursively generate a copy of this model retaining only objects
-        specified by the tree.
-
-        Parameters
-        ----------
-        tree
-            A tree formed of dictionaries describing which components of the
-            model should be retained.
-
-        Returns
-        -------
-        A copy of this model with a subset of attributes
-        """
-        if len(tree) == 0:
-            return self
-
-        with_paths = self.without_attributes()
-        for name, subtree in tree.items():
-            # noinspection PyProtectedMember
-            new_value = getattr(self, name)
-            if isinstance(
-                new_value,
-                (
-                    AbstractPriorModel,
-                    TuplePrior,
-                ),
-            ):
-                new_value = new_value._with_paths(subtree)
-            setattr(with_paths, name, new_value)
-        return with_paths
-
-    @split_paths
-    def with_paths(self, paths: List[Tuple[str, ...]]) -> "AbstractModel":
-        """
-        Recursively generate a copy of this model retaining only objects
-        specified by the list of paths.
-
-        Parameters
-        ----------
-        paths
-            A list of tuples of strings each of which points to a retained attribute.
-            All children of a given path are retained.
-
-        Returns
-        -------
-        A copy of this model with a subset of attributes
-        """
-        return self._with_paths(paths_to_tree(paths))
-
-    def _without_paths(self, tree: dict) -> "AbstractModel":
-        """
-        Recursively generate a copy of this model removing objects
-        specified by the tree.
-
-        Parameters
-        ----------
-        tree
-            A tree formed of dictionaries describing which components of the
-            model should be removed.
-
-        Returns
-        -------
-        A copy of this model with a subset of attributes
-        """
-        without_paths = copy.deepcopy(self)
-        for name, subtree in tree.items():
-            # noinspection PyProtectedMember
-            if len(subtree) == 0:
-                delattr(without_paths, name)
-            else:
-                new_value = getattr(without_paths, name)
-                if isinstance(
-                    new_value,
-                    (
-                        AbstractPriorModel,
-                        TuplePrior,
-                    ),
-                ):
-                    new_value = new_value._without_paths(subtree)
-                setattr(without_paths, name, new_value)
-        return without_paths
-
-    @split_paths
-    def without_paths(self, paths: List[Tuple[str, ...]]) -> "AbstractModel":
-        """
-        Recursively generate a copy of this model retaining only objects
-        not specified by the list of paths.
-
-        Parameters
-        ----------
-        paths
-            A list of tuples of strings each of which points to removed attribute.
-            All children of a given path are removed.
-
-        Returns
-        -------
-        A copy of this model with a subset of attributes
-        """
-        return self._without_paths(paths_to_tree(paths))
-
-    def index(self, path: Tuple[str, ...]) -> int:
-        """
-        Retrieve the index of a given path in the model
-        """
-        return self.paths.index(path)
-
-    @property
-    def mean_field(self) -> MeanField:
-        """
-        Implements the same interface as the graphical code
-        """
-        return MeanField(self)
-
-    @classmethod
-    def from_json(cls, file: str):
-        """
-        Loads the model from a .json file, which was written using the model's dictionary (`dict`) attribute as
-        follows:
-
-        import json
-
-        with open(filename, "w+") as f:
-            json.dump(model.dict, f, indent=4)
-
-        Parameters
-        ----------
-        file
-            The path and name of the .json file the model is loaded from.
-
-        Returns
-        -------
-        object
-            The model, which may be a `Collection` of `Model` objects or a single `Model`.
-        """
-
-        with open(file) as json_file:
-            model_dict = json.load(json_file)
-
-        return cls.from_dict(d=model_dict)
-
-    def add_assertion(self, assertion, name=""):
-        """
-        Assert that some relationship holds between physical values associated with
-        priors at the point an instance is created. If this fails a FitException is
-        raised causing the model to be re-sampled.
-        Parameters
-        ----------
-        assertion
-            An assertion that one prior must be greater than another.
-        name
-            A name describing the assertion that is logged when it is violated.
-        """
-        if assertion is True:
-            return
-        try:
-            assertion.name = name
-        except AttributeError:
-            pass
-        self._assertions.append(assertion)
-
-    @property
-    def name(self):
-        return self.__class__.__name__
-
-    # noinspection PyUnusedLocal
-    @staticmethod
-    def from_object(t, *args, **kwargs):
-        if inspect.isclass(t):
-            from .prior_model import Model
-
-            obj = object.__new__(Model)
-            obj.__init__(t, **kwargs)
-        elif isinstance(t, list) or isinstance(t, dict):
-            from autofit.mapper.prior_model import collection
-
-            obj = object.__new__(collection.Collection)
-            obj.__init__(t)
-        else:
-            obj = t
-        return obj
-
-    def take_attributes(self, source: object):
-        """
-        Take all attributes with a matching path from the source prior model.
-
-        For example, if this prior model has a prior "one" and a matching prior
-        is found associated with the source model then that attribute is attached
-        to this model.
-
-        If no matching attribute is found nothing happens.
-
-        Parameters
-        ----------
-        source
-            An instance or prior model from a previous search from which attributes
-            are passed to this model.
-        """
-
-        def assert_no_assertions(obj):
-            if len(getattr(obj, "_assertions", [])) > 0:
-                raise AssertionError(
-                    "take_attributes cannot be called once assertions have been added to the target"
-                )
-
-        assert_no_assertions(self)
-
-        for path, _ in sum(
-            map(self.path_instance_tuples_for_class, (Prior, float, TuplePrior)), []
-        ):
-            try:
-                item = copy.copy(source)
-                if isinstance(item, dict):
-                    from autofit.mapper.prior_model.collection import Collection
-
-                    item = Collection(item)
-                for attribute in path:
-                    if isinstance(attribute, int):
-                        item = item[attribute]
-                    else:
-                        item = copy.copy(getattr(item, attribute))
-
-                target = self
-                for attribute in path[:-1]:
-                    if isinstance(attribute, int):
-                        target = target[attribute]
-                    else:
-                        target = getattr(target, attribute)
-                    assert_no_assertions(target)
-
-                attribute = path[-1]
-                if isinstance(attribute, int):
-                    target[attribute] = item
-                else:
-                    setattr(target, path[-1], item)
-            except AttributeError:
-                pass
-
-    def instance_from_unit_vector(self, unit_vector, ignore_prior_limits=False):
-        """
-        Returns a ModelInstance, which has an attribute and class instance corresponding
-        to every `Model` attributed to this instance.
-        This method takes as input a unit vector of parameter values, converting each to
-        physical values via their priors.
-        Parameters
-        ----------
-        ignore_prior_limits
-            If true then no exception is thrown if priors fall outside defined limits
-        unit_vector: [float]
-            A unit hypercube vector that is mapped to an instance of physical values via the priors.
-        Returns
-        -------
-        model_instance : autofit.mapper.model.ModelInstance
-            An object containing reconstructed model_mapper instances
-        Raises
-        ------
-        exc.FitException
-            If any assertion attached to this object returns False.
-        """
-        exception_tuples = self.attribute_tuples_with_type(ConfigException)
-        if len(exception_tuples) > 0:
-            for name, exception in exception_tuples:
-                logger.exception(f"Could not load {name} because:\n\n{exception}")
-            names = [name for name, _ in exception_tuples]
-            raise ConfigException(
-                f"No configuration was found for some attributes ({', '.join(names)})"
-            )
-
-        if self.prior_count != len(unit_vector):
-            raise AssertionError(
-                f"prior_count ({self.prior_count}) != len(unit_vector) {len(unit_vector)}"
-            )
-
-        arguments = dict(
-            map(
-                lambda prior_tuple, unit: (
-                    prior_tuple.prior,
-                    prior_tuple.prior.value_for(
-                        unit,
-                        ignore_prior_limits=ignore_prior_limits,
-                    ),
-                ),
-                self.prior_tuples_ordered_by_id,
-                unit_vector,
-            )
-        )
-
-        return self.instance_for_arguments(
-            arguments,
-            ignore_assertions=ignore_prior_limits,
-        )
-
-    @property
-    @cast_collection(PriorNameValue)
-    @frozen_cache
-    def unique_prior_tuples(self):
-        """
-        Returns
-        -------
-        prior_tuple_dict: [(Prior, PriorTuple)]
-            The set of all priors associated with this mapper
-        """
-        return list(
-            {
-                prior_tuple[1]: prior_tuple
-                for prior_tuple in self.attribute_tuples_with_type(Prior)
-            }.values()
-        )
-
-    @property
-    @cast_collection(PriorNameValue)
-    @frozen_cache
-    def prior_tuples_ordered_by_id(self):
-        """
-        Returns
-        -------
-        priors: [Prior]
-            An ordered list of unique priors associated with this mapper
-        """
-        return sorted(
-            list(self.unique_prior_tuples), key=lambda prior_tuple: prior_tuple.prior.id
-        )
-
-    @property
-    def priors_ordered_by_id(self):
-        return [prior for _, prior in self.prior_tuples_ordered_by_id]
-
-    def vector_from_unit_vector(self, unit_vector, ignore_prior_limits=False):
-        """
-        Parameters
-        ----------
-        unit_vector: [float]
-            A unit hypercube vector
-        ignore_prior_limits
-            Set to True to prevent an exception being raised if
-            the physical value of a prior is outside the allowable
-            limits
-
-        Returns
-        -------
-        values: [float]
-            A vector with values output by priors
-        """
-        return list(
-            map(
-                lambda prior_tuple, unit: prior_tuple.prior.value_for(
-                    unit, ignore_prior_limits=ignore_prior_limits
-                ),
-                self.prior_tuples_ordered_by_id,
-                unit_vector,
-            )
-        )
-
-    def random_unit_vector_within_limits(
-        self, lower_limit: float = 0.0, upper_limit: float = 1.0
-    ) -> List[float]:
-        """
-        Generate a random vector of unit values by drawing uniform random values between 0 and 1.
-
-        Returns
-        -------
-        unit_values
-            A list of unit values constructed by taking random values from each prior.
-        """
-        return [
-            random.uniform(
-                max(lower_limit, prior.lower_unit_limit),
-                min(upper_limit, prior.upper_unit_limit),
-            )
-            for prior in self.priors_ordered_by_id
-        ]
-
-    def random_vector_from_priors_within_limits(
-        self, lower_limit: float = 0.0, upper_limit: float = 1.0
-    ) -> List[float]:
-        """
-        Returns a random vector of physical values by drawing uniform random values between lower and upper limits
-        defined as unit values, using the model priors to map them from unit values to physical values.
-
-        This function guesses infinite unit vectors, until one is randomly sampled whose physical parameters are within
-        the model's phyiscal limits.
-
-        This is used for MCMC initialization, whereby the starting points of a walker(s) are confined to a restricted
-        range of prior space. In particular, it is used for generate the "ball" initialization of Emcee.
-
-        Parameters
-        ----------
-        lower_limit
-            The lower limit as a unit value within which unit values (which are converted to physical values via the
-            priors) are generated.
-        upper_limit
-            The upper limit as a unit value within which unit values (which are converted to physical values via the
-            priors) are generated.
-
-        Returns
-        -------
-        physical_values
-            A list of physical values constructed by taking the mean possible value from
-            each prior.
-        """
-        vector = []
-
-        for prior in self.priors_ordered_by_id:
-            vector.append(
-                prior.random(
-                    lower_limit=lower_limit,
-                    upper_limit=upper_limit,
-                )
-            )
-
-        return vector
-
-    def random_instance_from_priors_within_limits(
-        self, lower_limit: float = 0.0, upper_limit: float = 1.0
-    ):
-        """
-        Returns a random instance of physical values by drawing uniform random values between lower and upper limits
-        defined as unit values, using the model priors to map them from unit values to physical values.
-
-        This function guesses infinite unit vectors, until one is randomly sampled whose physical parameters are within
-        the model's phyiscal limits. The final unit vector is then mapped to an instance.
-
-        Parameters
-        ----------
-        lower_limit
-            The lower limit as a unit value within which unit values (which are converted to physical values via the
-            priors) are generated.
-        upper_limit
-            The upper limit as a unit value within which unit values (which are converted to physical values via the
-            priors) are generated.
-
-        Returns
-        -------
-        physical_values
-            A list of physical values constructed by taking the mean possible value from
-            each prior.
-        """
-
-        vector = self.random_vector_from_priors_within_limits(
-            lower_limit=lower_limit, upper_limit=upper_limit
-        )
-
-        return self.instance_from_vector(vector=vector)
-
-    @property
-    def random_vector_from_priors(self):
-        """Generate a random vector of physical values by drawing uniform random values between 0 and 1 and using
-        the model priors to map them from unit values to physical values.
-        Returns
-        -------
-        physical_values: [float]
-            A list of physical values constructed by taking random values from each prior.
-        """
-        return self.random_vector_from_priors_within_limits(
-            lower_limit=0.0, upper_limit=1.0
-        )
-
-    @property
-    def physical_values_from_prior_medians(self):
-        """
-        Returns
-        -------
-        physical_values: [float]
-            A list of physical values constructed by taking the mean possible value from
-            each prior.
-        """
-        return self.vector_from_unit_vector([0.5] * len(self.unique_prior_tuples))
-
-    def instance_from_vector(self, vector, ignore_prior_limits=False):
-        """
-        Returns a ModelInstance, which has an attribute and class instance corresponding
-        to every `Model` attributed to this instance.
-        This method takes as input a physical vector of parameter values, thus omitting
-        the use of priors.
-        Parameters
-        ----------
-        vector: [float]
-            A vector of physical parameter values that is mapped to an instance.
-        ignore_prior_limits
-            If True don't check that physical values are within expected limits.
-
-        Returns
-        -------
-        model_instance : autofit.mapper.model.ModelInstance
-            An object containing reconstructed model_mapper instances
-        """
-        if len(vector) != self.prior_count:
-            raise AssertionError(
-                f"Vector length {len(vector)} != prior count {self.prior_count}"
-            )
-        arguments = dict(
-            map(
-                lambda prior_tuple, physical_unit: (prior_tuple.prior, physical_unit),
-                self.prior_tuples_ordered_by_id,
-                vector,
-            )
-        )
-
-        if not ignore_prior_limits:
-            for prior, value in arguments.items():
-                prior.assert_within_limits(value)
-
-        return self.instance_for_arguments(
-            arguments,
-            ignore_assertions=ignore_prior_limits,
-        )
-
-    def has(self, cls: Union[Type, Tuple[Type, ...]]) -> bool:
-        """
-        Parameters
-        ----------
-        cls
-            The type to check for
-
-        Returns
-        -------
-        True iff this model contains an instance or model with the given
-        type recursively. Includes models which have zero priors.
-        """
-        return self.has_instance(cls) or self.has_model(
-            cls, include_zero_dimension=True
-        )
-
-    def has_instance(self, cls) -> bool:
-        """
-        True iff this model contains an instance of type
-        cls, recursively.
-        """
-        return len(self.attribute_tuples_with_type(cls)) > 0
-
-    def has_model(self, cls, include_zero_dimension=False) -> bool:
-        """
-        True iff this model contains a Model of type
-        cls, recursively.
-        """
-        return (
-            len(
-                self.model_tuples_with_type(
-                    cls,
-                    include_zero_dimension=include_zero_dimension,
-                )
-            )
-            > 0
-        )
-
-    def is_only_model(self, cls) -> bool:
-        """
-        True iff this model contains at least one Model
-        of type cls and contains no PriorModels that are not
-        of type cls, recursively.
-        """
-        from .prior_model import Model
-
-        cls_models = self.model_tuples_with_type(cls)
-        other_models = [
-            value
-            for _, value in self.attribute_tuples_with_type(Model)
-            if value.prior_count > 0
-        ]
-        return len(cls_models) > 0 and len(cls_models) == len(other_models)
-
-    def replacing(self, arguments):
-        return self.mapper_from_partial_prior_arguments(arguments)
-
-    @classmethod
-    def product(cls, models: Iterable["AbstractPriorModel"]) -> "AbstractPriorModel":
-        """
-        Combine multiple models with the same structure by replacing priors with
-        priors that contain a message which is the product of the messages of the
-        priors with the same path in each model.
-
-        Parameters
-        ----------
-        models
-            A list of models to be combined
-
-        Returns
-        -------
-        A model where each prior has a message which is the product of the messages
-        associated with that prior across the models.
-        """
-        first, *rest = models
-
-        arguments = dict()
-
-        for path, prior in first.path_priors_tuples:
-            for other in rest:
-                prior = prior.with_message(
-                    prior.message * other.object_for_path(path).message
-                )
-            arguments[prior] = prior
-        return first.mapper_from_prior_arguments(arguments)
-
-    def mapper_from_partial_prior_arguments(self, arguments):
-        """
-        Returns a new model mapper from a dictionary mapping existing priors to
-        new priors, keeping existing priors where no mapping is provided.
-        Parameters
-        ----------
-        arguments: {Prior: Prior}
-            A dictionary mapping priors to priors
-        Returns
-        -------
-        model_mapper: ModelMapper
-            A new model mapper with updated priors.
-        """
-        original_prior_dict = {prior: prior for prior in self.priors}
-        return self.mapper_from_prior_arguments({**original_prior_dict, **arguments})
-
-    def mapper_from_prior_arguments(self, arguments):
-        """
-        Returns a new model mapper from a dictionary mapping existing priors to
-        new priors.
-        Parameters
-        ----------
-        arguments: {Prior: Prior}
-            A dictionary mapping priors to priors
-        Returns
-        -------
-        model_mapper: ModelMapper
-            A new model mapper with updated priors.
-        """
-        logger.debug(f"Creating a new mapper from arguments")
-
-        return self.gaussian_prior_model_for_arguments(arguments)
-
-    def gaussian_prior_model_for_arguments(self, arguments):
-        raise NotImplementedError()
-
-    def mapper_from_gaussian_tuples(
-        self, tuples, a=None, r=None, use_errors=True, use_widths=True, no_limits=False
-    ):
-        """
-        The widths of the new priors are taken from the
-        width_config. The new gaussian priors must be provided in the same order as
-        the priors associated with model.
-        If a is not None then all priors are created with an absolute width of a.
-        If r is not None then all priors are created with a relative width of r.
-        Parameters
-        ----------
-        no_limits
-            If `True` generated priors have infinite limits
-        r
-            The relative width to be assigned to gaussian priors
-        a
-            print(tuples[i][1], width)
-            The absolute width to be assigned to gaussian priors
-        use_errors
-            If True, the passed errors of the model components estimated in a previous `NonLinearSearch` (computed
-            at the prior_passer.sigma value) are used to set the pass Gaussian Prior sigma value (if both width and
-            passed errors are used, the maximum of these two values are used).
-        use_widths
-            If True, the minimum prior widths specified in the prior configs of the model components are used to
-            set the passed Gaussian Prior sigma value (if both widths and passed errors are used, the maximum of
-            these two values are used).
-        tuples
-            A list of tuples each containing the mean and width of a prior
-        Returns
-        -------
-        mapper: ModelMapper
-            A new model mapper with all priors replaced by gaussian priors.
-        """
-
-        prior_tuples = self.prior_tuples_ordered_by_id
-        prior_class_dict = self.prior_class_dict
-        arguments = {}
-
-        for i, prior_tuple in enumerate(prior_tuples):
-            prior = prior_tuple.prior
-            cls = prior_class_dict[prior]
-            mean, sigma = tuples[i]
-
-            name = prior_tuple.name
-            # Use the name of the collection for configuration when a prior's name
-            # is just a number (i.e. its position in a collection)
-            if name.isdigit():
-                name = self.path_for_prior(prior_tuple.prior)[-2]
-
-            width_modifier = (
-                prior.width_modifier
-                or WidthModifier.for_class_and_attribute_name(cls, name)
-            )
-
-            if a is not None and r is not None:
-                raise exc.PriorException(
-                    "Width of new priors cannot be both relative and absolute."
-                )
-            if a is not None:
-                width = a
-            elif r is not None:
-                width = r * mean
-            else:
-                width = width_modifier(mean)
-
-            if no_limits:
-                limits = (float("-inf"), float("inf"))
-            else:
-                try:
-                    limits = Limits.for_class_and_attributes_name(cls, name)
-                except ConfigException:
-                    limits = prior.limits
-
-            if use_errors and not use_widths:
-                sigma = tuples[i][1]
-            elif not use_errors and use_widths:
-                sigma = width
-            elif use_errors and use_widths:
-                sigma = max(tuples[i][1], width)
-            else:
-                raise exc.PriorException(
-                    "use_passed_errors and use_widths are both False, meaning there is no "
-                    "way to pass priors to set up the new model's Gaussian Priors."
-                )
-
-            new_prior = GaussianPrior(mean, sigma, *limits)
-            new_prior.id = prior.id
-            new_prior.width_modifier = prior.width_modifier
-            arguments[prior] = new_prior
-
-        return self.mapper_from_prior_arguments(arguments)
-
-    def with_limits(self, limits: List[Tuple[float, float]]) -> "AbstractPriorModel":
-        """
-        Create a new instance of this model where each prior is updated to
-        lie between new limits.
-
-        Parameters
-        ----------
-        limits
-            A list of pairs of lower and upper limits, one for each prior.
-
-        Returns
-        -------
-        A new model with updated limits
-        """
-        return self.mapper_from_prior_arguments(
-            {
-                prior: prior.with_limits(*prior_limits)
-                for prior, prior_limits in zip(self.priors_ordered_by_id, limits)
-            }
-        )
-
-    def mapper_from_uniform_floats(self, floats, b):
-        """
-        The widths of the new priors are the `floats` value minus and plus the input bound `b`.
-
-        Parameters
-        ----------
-        floats
-            A list of floats each containing the centre of the new uniform priors.
-        b
-            The bound value which is subtracted from each float to calculate the `lower_limit` and `upper_limit`
-            of each uniform prior.
-
-        Returns
-        -------
-        mapper: ModelMapper
-            A new model mapper with all priors replaced by uniform priors.
-        """
-
-        prior_tuples = self.prior_tuples_ordered_by_id
-        arguments = {}
-
-        for i, prior_tuple in enumerate(prior_tuples):
-            prior = prior_tuple.prior
-
-            new_prior = UniformPrior(
-                lower_limit=floats[i] - b, upper_limit=floats[i] + b
-            )
-            new_prior.id = prior.id
-            arguments[prior] = new_prior
-
-        return self.mapper_from_prior_arguments(arguments)
-
-    def instance_from_prior_medians(self, ignore_prior_limits=False):
-        """
-        Returns a list of physical values from the median values of the priors.
-        Returns
-        -------
-        physical_values : [float]
-            A list of physical values
-        """
-        return self.instance_from_unit_vector(
-            unit_vector=[0.5] * self.prior_count,
-            ignore_prior_limits=ignore_prior_limits,
-        )
-
-    def log_prior_list_from_vector(
-        self,
-        vector: [float],
-    ):
-        """
-        Compute the log priors of every parameter in a vector, using the Prior of every parameter.
-        The log prior values are used by Emcee to map the log likelihood to the poserior of the model.
-        Parameters
-        ----------
-        vector : [float]
-            A vector of physical parameter values.
-        Returns
-        -------
-        log_prior_list : []
-            An list of the log prior value of every parameter.
-        """
-        return list(
-            map(
-                lambda prior_tuple, value: prior_tuple.prior.log_prior_from_value(
-                    value=value
-                ),
-                self.prior_tuples_ordered_by_id,
-                vector,
-            )
-        )
-
-    def random_instance(self, ignore_prior_limits=False):
-        """
-        Returns a random instance of the model.
-        """
-        logger.debug(f"Creating a random instance")
-        if ignore_prior_limits:
-            return self.instance_from_unit_vector(
-                unit_vector=[random.random() for _ in range(self.prior_count)],
-                ignore_prior_limits=ignore_prior_limits,
-            )
-        return self.instance_for_arguments(
-            {prior: prior.random() for prior in self.priors}
-        )
-
-    @staticmethod
-    @DynamicRecursionCache()
-    def from_instance(
-        instance,
-        model_classes: Union[type, Iterable[type]] = tuple(),
-        exclude_classes: Union[type, Iterable[type]] = tuple(),
-    ):
-        """
-        Recursively create a prior object model from an object model.
-
-        Parameters
-        ----------
-        model_classes
-            A tuple of classes that should be converted to a prior model
-        exclude_classes
-            A tuple of classes that should not be converted to a prior model
-        instance
-            A dictionary, list, class instance or model instance
-        Returns
-        -------
-        abstract_prior_model
-            A concrete child of an abstract prior model
-        """
-        from autofit.mapper.prior_model import collection
-
-        if isinstance(instance, exclude_classes):
-            return instance
-        if isinstance(instance, (Prior, AbstractPriorModel)):
-            return instance
-        elif isinstance(instance, list):
-            result = collection.Collection(
-                [
-                    AbstractPriorModel.from_instance(
-                        item,
-                        model_classes=model_classes,
-                        exclude_classes=exclude_classes,
-                    )
-                    for item in instance
-                ]
-            )
-        elif isinstance(instance, model.ModelInstance):
-            from autofit.mapper import model_mapper
-
-            result = model_mapper.ModelMapper()
-            for key, value in instance.dict.items():
-                setattr(
-                    result,
-                    key,
-                    AbstractPriorModel.from_instance(
-                        value,
-                        model_classes=model_classes,
-                        exclude_classes=exclude_classes,
-                    ),
-                )
-        elif isinstance(instance, dict):
-            result = collection.Collection(
-                {
-                    key: AbstractPriorModel.from_instance(
-                        value,
-                        model_classes=model_classes,
-                        exclude_classes=exclude_classes,
-                    )
-                    for key, value in instance.items()
-                }
-            )
-        elif isinstance(instance, (np.ndarray, types.FunctionType)):
-            return instance
-        else:
-            from .prior_model import Model
-
-            try:
-                result = Model(
-                    instance.__class__,
-                    **{
-                        key: AbstractPriorModel.from_instance(
-                            value,
-                            model_classes=model_classes,
-                            exclude_classes=exclude_classes,
-                        )
-                        for key, value in instance.__dict__.items()
-                        if key != "cls"
-                    },
-                )
-            except AttributeError:
-                return instance
-        if isinstance(instance, model_classes):
-            return result.as_model()
-        return result
-
-    def items(self):
-        return (
-            self.direct_prior_tuples
-            + self.direct_instance_tuples
-            + self.direct_prior_model_tuples
-            + self.direct_tuple_priors
-        )
-
-    @property
-    @cast_collection(PriorNameValue)
-    def direct_prior_tuples(self):
-        return self.direct_tuples_with_type(Prior)
-
-    @property
-    @cast_collection(InstanceNameValue)
-    def direct_instance_tuples(self):
-        return self.direct_tuples_with_type(float)
-
-    @property
-    @cast_collection(PriorModelNameValue)
-    def prior_model_tuples(self):
-        return self.direct_tuples_with_type(AbstractPriorModel)
-
-    @property
-    @cast_collection(PriorModelNameValue)
-    def direct_prior_model_tuples(self):
-        return self.direct_tuples_with_type(AbstractPriorModel)
-
-    @property
-    @cast_collection(PriorModelNameValue)
-    def direct_tuple_priors(self):
-        return self.direct_tuples_with_type(TuplePrior)
-
-    @property
-    @cast_collection(PriorNameValue)
-    def tuple_prior_tuples(self):
-        """
-        Returns
-        -------
-        tuple_prior_tuples: [(String, TuplePrior)]
-        """
-        return self.direct_tuples_with_type(TuplePrior)
-
-    @property
-    @cast_collection(PriorNameValue)
-    def direct_prior_tuples(self):
-        """
-        Returns
-        -------
-        direct_priors: [(String, Prior)]
-        """
-        return self.direct_tuples_with_type(Prior)
-
-    @property
-    @cast_collection(DeferredNameValue)
-    def direct_deferred_tuples(self):
-        return self.direct_tuples_with_type(DeferredArgument)
-
-    @property
-    @cast_collection(PriorNameValue)
-    def prior_tuples(self):
-        """
-        Returns
-        -------
-        priors: [(String, Prior))]
-        """
-        # noinspection PyUnresolvedReferences
-        return self.attribute_tuples_with_type(Prior, ignore_children=True)
-
-    def __eq__(self, other):
-        return (
-            isinstance(other, AbstractPriorModel)
-            and self.direct_prior_model_tuples == other.direct_prior_model_tuples
-        )
-
-    @property
-    @cast_collection(InstanceNameValue)
-    def instance_tuples(self):
-        """
-        Returns
-        -------
-        instances: [(String, instance)]
-        """
-        return self.attribute_tuples_with_type(float, ignore_class=Prior)
-
-    @property
-    def prior_class_dict(self):
-        from autofit.mapper.prior_model.annotation import AnnotationPriorModel
-
-        d = {prior[1]: self.cls for prior in self.prior_tuples}
-        for prior_model in self.prior_model_tuples:
-            if not isinstance(prior_model[1], AnnotationPriorModel):
-                d.update(prior_model[1].prior_class_dict)
-        return d
-
-    def _instance_for_arguments(
-        self,
-        arguments: Dict[Prior, float],
-    ):
-        raise NotImplementedError()
-
-    def instance_for_arguments(
-        self,
-        arguments: Dict[Prior, float],
-        ignore_assertions: bool = False,
-    ):
-        """
-        Returns an instance of the model for a set of arguments
-
-        Parameters
-        ----------
-        arguments
-            Dictionary mapping priors to attribute analysis_path and value pairs
-        ignore_assertions
-            If True, assertions will not be checked
-
-        Returns
-        -------
-            An instance of the class
-        """
-        if not (
-            conf.instance["general"]["test"]["exception_override"] or ignore_assertions
-        ):
-            self.check_assertions(arguments)
-
-        logger.debug(f"Creating an instance for arguments")
-        return self._instance_for_arguments(
-            arguments,
-        )
-
-    def path_for_name(self, name: str) -> Tuple[str, ...]:
-        """
-        Find the path to a prior in the model that matches
-        a given name.
-
-        For example, name_of_model_name_of_prior could match
-        (name_of_model, name_of_prior). Unfortunately it is
-        possible for ambiguity to occur. For example, another
-        valid path could be (name, of_model, name_of_prior)
-        in which case there is no way to determine which path
-        actually matches the name.
-
-        Parameters
-        ----------
-        name
-            A name for a prior where names of models and the
-            name of the prior have been joined by underscores.
-
-        Returns
-        -------
-        A path to that model
-
-        Raises
-        ------
-        AssertionError
-            Iff no matching path is found
-        """
-
-        def _explode_path(path_):
-            return tuple(string for part in path_ for string in part.split("_"))
-
-        exploded = tuple(name.split("_"))
-        for path, _ in self.path_priors_tuples:
-            exploded_path = _explode_path(path)
-            if exploded_path == exploded:
-                return path
-
-        for path, prior_tuple in self.path_instance_tuples_for_class(TuplePrior):
-            for name, prior in prior_tuple.prior_tuples:
-                total_path = path[:-1] + (name,)
-                exploded_path = _explode_path(total_path)
-                if exploded_path == exploded:
-                    return path + (name,)
-        raise AssertionError(f"No path was found matching {name}")
-
-    def instance_from_prior_name_arguments(
-        self, prior_name_arguments: Dict[str, float]
-    ):
-        """
-        Instantiate the model from the names of priors and
-        corresponding values.
-
-        Parameters
-        ----------
-        prior_name_arguments
-            The names of priors where names of models and the
-            name of the prior have been joined by underscores,
-            mapped to corresponding values.
-
-        Returns
-        -------
-        An instance of the model
-        """
-        return self.instance_from_path_arguments(
-            {
-                self.path_for_name(name): value
-                for name, value in prior_name_arguments.items()
-            }
-        )
-
-    def instance_from_path_arguments(self, path_arguments: Dict[Tuple[str], float]):
-        """
-        Create an instance from a dictionary mapping paths to tuples
-        to corresponding values.
-
-        Parameters
-        ----------
-        path_arguments
-            A dictionary mapping paths to priors to corresponding values.
-            Note that, for linked priors, each path only needs to be
-            specified once. If multiple paths for the same prior are
-            specified then the value for the last path will be used.
-
-        Returns
-        -------
-        An instance of the model
-        """
-        arguments = {
-            self.object_for_path(path): value for path, value in path_arguments.items()
-        }
-        return self._instance_for_arguments(arguments)
-
-    @property
-    def prior_count(self) -> int:
-        """
-        How many unique priors does this model contain?
-        """
-        return len(self.unique_prior_tuples)
-
-    @property
-    def total_free_parameters(self) -> int:
-        """
-        Returns the prior count, but with a name that is more easy to interpret for users.
-        """
-        return self.prior_count
-
-    @property
-    def priors(self):
-        return [prior_tuple.prior for prior_tuple in self.prior_tuples]
-
-    @property
-    def _prior_id_map(self):
-        return {prior.id: prior for prior in self.priors}
-
-    def prior_with_id(self, prior_id):
-        return self._prior_id_map[prior_id]
-
-    def name_for_prior(self, prior):
-        for prior_model_name, prior_model in self.direct_prior_model_tuples:
-            prior_name = prior_model.name_for_prior(prior)
-            if prior_name is not None:
-                return "{}_{}".format(prior_model_name, prior_name)
-        prior_tuples = self.prior_tuples
-        for name, p in prior_tuples:
-            if p == prior:
-                return name
-
-    def __hash__(self):
-        return self.id
-
-    def __add__(self, other):
-        if isinstance(other, Prior):
-            return other + self
-
-        result = copy.deepcopy(self)
-
-        for key, value in other.__dict__.items():
-            if not hasattr(result, key) or isinstance(value, Prior):
-                setattr(result, key, value)
-                continue
-            result_value = getattr(result, key)
-            if isinstance(value, AbstractPriorModel):
-                if isinstance(result_value, AbstractPriorModel):
-                    setattr(result, key, result_value + value)
-                else:
-                    setattr(result, key, value)
-
-        return result
-
-    def copy_with_fixed_priors(self, instance, excluded_classes=tuple()):
-        """
-        Recursively overwrite priors in the mapper with instance values from the
-        instance except where the containing class is the descendant of a listed class.
-        Parameters
-        ----------
-        excluded_classes
-            Classes that should be left model
-        instance
-            The best fit from the previous search
-        """
-        mapper = copy.deepcopy(self)
-        transfer_classes(instance, mapper, excluded_classes)
-        return mapper
-
-    @property
-    def path_priors_tuples(self) -> List[Tuple[Path, Prior]]:
-        path_priors_tuples = self.path_instance_tuples_for_class(Prior)
-        return sorted(path_priors_tuples, key=lambda item: item[1].id)
-
-    @property
-    def paths(self) -> List[Path]:
-        """
-        A list of paths to all the priors in the model, ordered by their
-        ids
-        """
-        return [path for path, _ in self.path_priors_tuples]
-
-    @property
-    def composition(self):
-        return [".".join(path) for path in self.paths]
-
-    def sort_priors_alphabetically(self, priors: Iterable[Prior]) -> List[Prior]:
-        """
-        Sort priors by their paths according to this model.
-
-        Parameters
-        ----------
-        priors
-            A set of priors
-
-        Returns
-        -------
-        Those priors sorted alphabetically by path.
-        """
-        return sorted(priors, key=lambda prior: self.path_for_prior(prior))
-
-    def path_for_prior(self, prior: Prior) -> Optional[Path]:
-        """
-        Find a path that points at the given tuple.
-        Returns the first path or None if no path is found.
-        Parameters
-        ----------
-        prior
-            A prior representing what's known about some dimension of the model.
-        Returns
-        -------
-        A path, a series of attributes that point to one location of the prior.
-        """
-        for path in self.all_paths_for_prior(prior):
-            return path
-        return None
-
-    def all_paths_for_prior(self, prior: Prior) -> Generator[Path, None, None]:
-        """
-        Find all paths that points at the given tuple.
-
-        Parameters
-        ----------
-        prior
-            A prior representing what's known about some dimension of the model.
-        Yields
-        -------
-        Paths, each a series of attributes that point to one location of the prior.
-        """
-        for path, path_prior in reversed(self.path_priors_tuples):
-            if path_prior == prior:
-                yield path
-
-    @property
-    def path_float_tuples(self):
-        return self.path_instance_tuples_for_class(float, ignore_class=Prior)
-
-    @property
-    def unique_prior_paths(self):
-        return [item[0] for item in self.unique_path_prior_tuples]
-
-    @property
-    def unique_path_prior_tuples(self):
-        unique = {item[1]: item for item in self.path_priors_tuples}.values()
-        return sorted(unique, key=lambda item: item[1].id)
-
-    @property
-    def prior_prior_model_dict(self):
-        """
-        Returns
-        -------
-        prior_prior_model_dict: {Prior: Model}
-            A dictionary mapping priors to associated prior models. Each prior will only
-            have one prior model; if a prior is shared by two prior models then one of
-            those prior models will be in this dictionary.
-        """
-        return {
-            prior: prior_model[1]
-            for prior_model in self.prior_model_tuples + [("model", self)]
-            for _, prior in prior_model[1].prior_tuples
-        }
-
-    def log_prior_list_from(self, parameter_lists: List[List]) -> List:
-        return [
-            sum(self.log_prior_list_from_vector(vector=vector))
-            for vector in parameter_lists
-        ]
-
-    @property
-    def info(self) -> str:
-        """
-        Use the priors that make up the model_mapper to generate information on each
-        parameter of the overall model.
-        This information is extracted from each priors *model_info* property.
-        """
-
-        formatter = TextFormatter(line_length=info_whitespace())
-
-        for t in self.path_instance_tuples_for_class(
-            (Prior, float, int, tuple, ConfigException), ignore_children=True
-        ):
-            name = t[0][-1]
-            if name in ("id", "item_number"):
-                continue
-
-            if isinstance(t[1], ConfigException):
-                t = (t[0], "Prior Missing: Enter Manually or Add to Config")
-
-            formatter.add(*t)
-
-        return "\n\n".join(
-            [
-                f"Total Free Parameters = {self.prior_count}",
-                f"{self.parameterization}",
-                formatter.text,
-            ]
-        )
-
-    @property
-    def order_no(self) -> str:
-        """
-        A string that can be used to order models by their
-        parametrisation.
-
-        Priors and constants are ordered by their paths and then
-        joined into a string which means that models with higher
-        associated values are consistently ordered later in a
-        collection.
-        """
-        values = [
-            str(float(value))
-            for _, value in sorted(
-                self.path_instance_tuples_for_class((Prior, float)), key=lambda t: t[0]
-            )
-        ]
-        return ":".join(values)
-
-    @property
-    def parameterization(self) -> str:
-        """
-        Describes the path to each of the PriorModels, its class
-        and its number of free parameters
-        """
-        from .prior_model import Model
-
-        formatter = TextFormatter(line_length=info_whitespace())
-
-        for t in self.path_instance_tuples_for_class(
-            (
-                Prior,
-                float,
-                tuple,
-            ),
-            ignore_children=True,
-        ):
-            for i in range(len(t[0])):
-                path = t[0][:i]
-                obj = self.object_for_path(path)
-                if isinstance(obj, TuplePrior):
-                    continue
-                if isinstance(obj, AbstractPriorModel):
-                    n = obj.prior_count
-                else:
-                    n = 0
-                if isinstance(obj, Model):
-                    name = obj.cls.__name__
-                else:
-                    name = type(obj).__name__
-
-                formatter.add(("model",) + path, f"{name} (N={n})")
-
-        return formatter.text
-
-    @property
-    def all_paths(self) -> List[Tuple[Path]]:
-        """
-        All possible paths to all priors grouped such that all
-        paths to the same prior are collected together in a tuple.
-        """
-        if self.prior_count == 0:
-            return []
-        paths, _ = zip(*self.all_paths_prior_tuples)
-        return paths
-
-    @property
-    def all_paths_prior_tuples(self) -> List[Tuple[Tuple[Path], Prior]]:
-        """
-        Maps a tuple containing all paths to a given prior to that prior.
-        """
-        prior_paths_dict = defaultdict(tuple)
-        for path, prior in self.path_priors_tuples:
-            prior_paths_dict[prior] += (path,)
-        return sorted(
-            [(paths, prior) for prior, paths in prior_paths_dict.items()],
-            key=lambda item: item[1].id,
-        )
-
-    @property
-    def all_names(self) -> List[Tuple[str]]:
-        """
-        All possible names for all priors grouped such that all
-        names for a given prior are collected together in a tuple.
-        """
-        if self.prior_count == 0:
-            return []
-        names, _ = zip(*self.all_name_prior_tuples)
-        return names
-
-    @property
-    def all_name_prior_tuples(self) -> List[Tuple[Tuple[str], Prior]]:
-        """
-        Maps a tuple containing all names for a given prior to that prior.
-        """
-        path_modifier = TuplePathModifier(self)
-        return [
-            (tuple(".".join(path_modifier(path)) for path in paths), prior)
-            for paths, prior in self.all_paths_prior_tuples
-        ]
-
-    @property
-    def model_component_and_parameter_names(self) -> List[str]:
-        """The param_names vector is a list each parameter's analysis_path, and is used
-        for *corner.py* visualization.
-        The parameter names are determined from the class instance names of the
-        model_mapper. Latex tags are properties of each model class."""
-        prior_paths = self.unique_prior_paths
-
-        tuple_filter = TuplePathModifier(self)
-
-        prior_paths = list(map(tuple_filter, prior_paths))
-
-        return [".".join(path) for path in prior_paths]
-
-    @property
-    def joined_paths(self) -> List[str]:
-        prior_paths = self.unique_prior_paths
-
-        return [".".join(path) for path in prior_paths]
-
-    @property
-    def parameter_names(self) -> List[str]:
-        """
-        The param_names vector is a list each parameter's analysis_path, and is used
-        for *corner.py* visualization.
-
-        The parameter names are determined from the class instance names of the
-        model_mapper. Latex tags are properties of each model class.
-        """
-        return [parameter_name[-1] for parameter_name in self.unique_prior_paths]
-
-    @property
-    def parameter_labels(self) -> List[str]:
-        """
-        Returns a list of the label of every parameter in a model.
-
-        This is used for displaying model results as text and for visualization with *corner.py*.
-
-        The parameter labels are defined for every parameter of every model component in the config files label.ini and
-        label_format.ini.
-        """
-
-        parameter_labels = []
-
-        for parameter_name in self.parameter_names:
-            parameter_label = frm.convert_name_to_label(
-                parameter_name=parameter_name, name_to_label=True
-            )
-            parameter_labels.append(parameter_label)
-
-        return parameter_labels
-
-    @property
-    def superscripts(self) -> List[str]:
-        """
-        Returns a list of the model component superscripts for every parameter in a model.
-
-
-        The class superscript labels are defined as the name of every model component in the `ModelMapper`. For
-        the example of a 1D Gaussian, if the model component name is `gaussian` three superscripts
-        with this string (corresponding to the parameters `centre`, `normalization` and `sigma`) will
-        be returned.
-
-        For a `Collection`, the name of the inner model components are used.
-
-        These superscripts may be overwritten by those returned from the `superscripts_config_overwrite` property,
-        which optionally loads the superscripts from a `.json` config file. This allows high levels of customization
-        in what superscripts are used.
-
-        This is used for displaying model results as text and for visualization.
-        """
-
-        prior_paths = self.unique_prior_paths
-
-        tuple_filter = TuplePathModifier(self)
-
-        prior_paths = map(tuple_filter, prior_paths)
-
-        superscripts = [path[-2] if len(path) > 1 else None for path in prior_paths]
-
-        return [
-            superscript if not superscript_overwrite else superscript_overwrite
-            for superscript, superscript_overwrite in zip(
-                superscripts, self.superscripts_overwrite_via_config
-            )
-        ]
-
-    @property
-    def superscripts_overwrite_via_config(self) -> List[str]:
-        """
-        Returns a list of the model component superscripts for every parameter in a model, which can be used to
-        overwrite the default superscripts used in the function above.
-
-        The class superscript labels are defined for a model component in the config file `notation/label.ini`. By
-        default, the model component names are used as superscripts (which are loaded via the method `superscripts`).
-        These are overwritten by the superscripts loaded via a  config in this function. If no value is present in the
-        config the model component names are used.
-
-        For the example of a 1D Gaussian, when instatiated as a model component it is typically given the
-        name `gaussian`. Thus, the string `gaussian` will be used as the supersript of every one its parameter labels
-        (`centre`, `normalization` and `sigma`). However, if the config file `label.ini` reads `Gaussian=g`, every
-        superscript for these parameters will instead be given the superscript `g`.
-
-        This is used for displaying model results as text and for visualization with.
-        """
-
-        superscripts = []
-
-        for prior_name, prior in self.prior_tuples_ordered_by_id:
-            cls = self.prior_class_dict[prior]
-            try:
-                superscript = conf.instance["notation"]["label"]["superscript"][
-                    cls.__name__
-                ]
-
-            except KeyError:
-                superscript = ""
-
-            superscripts.append(superscript)
-
-        return superscripts
-
-    @property
-    def parameter_labels_with_superscripts(self) -> List[str]:
-        """
-        Returns a list of the latex parameter label and superscript of every parameter in a model.
-
-        The parameter labels are defined for every parameter of every model component in the config file `label.ini`.
-        This file can also be used to overwrite superscripts, that are assigned based on the model component name.
-
-        This is used for displaying model results as text and for visualization, for example labelling parameters on a
-        cornerplot.
-        """
-
-        return [
-            f"{label}^{{\\rm {superscript}}}" if superscript else f"{label}"
-            for label, superscript in zip(self.parameter_labels, self.superscripts)
-        ]
-
-    @property
-    def parameter_labels_with_superscripts_latex(self) -> List[str]:
-        """
-        Returns a list of the latex parameter label and superscript of every parameter in a model.
-
-        The parameter labels are defined for every parameter of every model component in the config file `label.ini`.
-        This file can also be used to overwrite superscripts, that are assigned based on the model component name.
-
-        This is used for displaying model results as text and for visualization, for example labelling parameters on a
-        cornerplot.
-        """
-
-        return [f"${label}$" for label in self.parameter_labels_with_superscripts]
-
-
-def transfer_classes(instance, mapper, model_classes=None):
-    """
-    Recursively overwrite priors in the mapper with instance values from the
-    instance except where the containing class is the descendant of a listed class.
-    Parameters
-    ----------
-    model_classes
-        Classes whose descendants should not be overwritten
-    instance
-        The best fit from the previous search
-    mapper
-        The prior model from the previous search
-    """
-    from autofit.mapper.prior_model.annotation import AnnotationPriorModel
-
-    model_classes = model_classes or []
-    for key, instance_value in instance.__dict__.items():
-        try:
-            mapper_value = getattr(mapper, key)
-            if isinstance(mapper_value, Prior) or isinstance(
-                mapper_value, AnnotationPriorModel
-            ):
-                setattr(mapper, key, instance_value)
-                continue
-            if not any(isinstance(instance_value, cls) for cls in model_classes):
-                try:
-                    transfer_classes(instance_value, mapper_value, model_classes)
-                except AttributeError:
-                    setattr(mapper, key, instance_value)
-        except AttributeError:
-            pass
+import copy
+import inspect
+import json
+import logging
+import random
+import types
+from collections import defaultdict
+from typing import Tuple, Optional, Dict, List, Iterable, Generator, Union, Type
+
+import numpy as np
+
+from autoconf import conf
+from autoconf.exc import ConfigException
+from autofit import exc
+from autofit.mapper import model
+from autofit.mapper.model import AbstractModel, frozen_cache
+from autofit.mapper.prior import GaussianPrior
+from autofit.mapper.prior import UniformPrior
+from autofit.mapper.prior.abstract import Prior
+from autofit.mapper.prior.deferred import DeferredArgument
+from autofit.mapper.prior.tuple_prior import TuplePrior
+from autofit.mapper.prior.width_modifier import WidthModifier
+from autofit.mapper.prior_model.attribute_pair import DeferredNameValue
+from autofit.mapper.prior_model.attribute_pair import (
+    cast_collection,
+    PriorNameValue,
+    InstanceNameValue,
+)
+from autofit.mapper.prior_model.recursion import DynamicRecursionCache
+from autofit.mapper.prior_model.representative import find_groups
+from autofit.mapper.prior_model.util import PriorModelNameValue
+from autofit.text import formatter as frm
+from autofit.text.formatter import TextFormatter
+from autofit.tools.util import info_whitespace
+from autofit.tools.util import split_paths
+
+logger = logging.getLogger(__name__)
+
+
+class Limits:
+    @staticmethod
+    def for_class_and_attributes_name(cls, attribute_name):
+        limit_dict = conf.instance.prior_config.for_class_and_suffix_path(
+            cls, [attribute_name, "gaussian_limits"]
+        )
+        return limit_dict["lower"], limit_dict["upper"]
+
+
+class TuplePathModifier:
+    def __init__(self, model_: "AbstractPriorModel"):
+        """
+        Modifies paths to priors contained in tuples.
+
+        When a tuple is found in a signature a PriorTuple is created.
+
+        The true path to a variable in the tuple is
+        ("some", "preamble", "tuple_name", "tuple_name_0")
+
+        Where 0 is the index of the tuple member. "tuple_name" must be
+        removed from this path for some uses.
+
+        When called, instances of this class remove the name of the tuple
+        i.e:
+        -> ("some", "preamble", "tuple_name_0")
+
+        Parameters
+        ----------
+        model_
+        """
+        tuple_priors = model_.path_instance_tuples_for_class(TuplePrior)
+        try:
+            self.tuple_paths, _ = zip(*tuple_priors)
+        except ValueError:
+            self.tuple_paths = None
+
+    def __call__(self, path):
+        if self.tuple_paths is not None:
+            if path[:-1] in self.tuple_paths:
+                return path[:-2] + (path[-1],)
+        return path
+
+
+Path = Tuple[str, ...]
+
+
+class MeanField:
+    def __init__(self, prior_model: "AbstractPriorModel"):
+        """
+        Implements same interface as graphical code
+
+        Parameters
+        ----------
+        prior_model
+        """
+        self.prior_model = prior_model
+
+    def __getitem__(self, item):
+        """
+        Retrieve a prior by a prior with the same id
+        """
+        for prior in self.prior_model.priors:
+            if prior == item:
+                return prior
+        raise KeyError(f"Could not find {item} in model")
+
+
+def paths_to_tree(paths: List[Tuple[str, ...]], tree: Optional[dict] = None) -> dict:
+    """
+    Recursively convert a list of paths to a tree structure where common paths
+    are matched.
+
+    Parameters
+    ----------
+    paths
+        A list of paths to attributes in the model.
+    tree
+        A tree already embedded in a parent tree.
+
+    Returns
+    -------
+    A tree with depth max(map(len, paths))
+
+    Examples
+    --------
+    paths_to_tree([
+        ("one", "two", "three"),
+        ("one", "two", "four"),
+    ])
+
+    gives
+
+    {
+        "one": {
+            "two": {
+                "three": {},
+                "four": {}
+            }
+        }
+    }
+    """
+    tree = tree or dict()
+    for path in paths:
+        if len(path) == 0:
+            return tree
+        first, *rest = path
+        if first not in tree:
+            child = dict()
+            tree[first] = child
+        tree[first] = paths_to_tree([rest], tree=tree[first])
+    return tree
+
+
+class AbstractPriorModel(AbstractModel):
+    """
+    Abstract model that maps a set of priors to a particular class. Must be
+    overridden by any prior model so that the model mapper recognises its prior \
+    model attributes.
+    @DynamicAttrs
+    """
+
+    def __init__(self, label=None):
+        super().__init__(label=label)
+        self._assertions = list()
+
+    @property
+    def assertions(self):
+        return self._assertions
+
+    @assertions.setter
+    def assertions(self, assertions):
+        self._assertions = assertions
+
+    def check_assertions(self, arguments: Dict[Prior, float]):
+        """
+        Check that all assertions are satisfied by the given arguments.
+
+        Parameters
+        ----------
+        arguments
+            A dictionary mapping priors to values
+
+        Raises
+        ------
+        FitException
+            If any assertion is not satisfied
+        """
+        failed_assertions = [
+            assertion
+            for assertion in self._assertions
+            if assertion is False
+            or assertion is not True
+            and not assertion.instance_for_arguments(
+                arguments,
+            )
+        ]
+        number_of_failed_assertions = len(failed_assertions)
+        if number_of_failed_assertions > 0:
+            name_string = "\n".join(
+                [
+                    assertion.name
+                    for assertion in failed_assertions
+                    if hasattr(assertion, "name") and assertion.name is not None
+                ]
+            )
+            raise exc.FitException(
+                f"{number_of_failed_assertions} assertions failed!\n{name_string}"
+            )
+
+    def cast(
+        self,
+        value_dict: Dict["AbstractModel", dict],
+        new_class: type,
+    ) -> "AbstractPriorModel":
+        """
+        Cast models to a new type. Allows selected models in within this
+        model to be given a new type and new arguments.
+
+        Parameters
+        ----------
+        value_dict
+            A dictionary mapping models to dictionaries of argument overrides
+        new_class
+            A new class to which specified models should be converted
+
+        Returns
+        -------
+        A model where specified child models have been updated to a new class
+        and new arguments
+        """
+        from .prior_model import Model
+
+        updated = self
+
+        for path, prior_model in self.path_instance_tuples_for_class(Model):
+            try:
+                model_value_dict = value_dict[prior_model]
+                argument_dict = {
+                    **dict(prior_model.direct_prior_tuples),
+                    **dict(prior_model.direct_tuples_with_type(float)),
+                    **model_value_dict,
+                }
+                updated = updated.replacing_for_path(
+                    path, Model(new_class, **argument_dict)
+                )
+
+            except KeyError:
+                pass
+
+        return updated
+
+    def without_attributes(self) -> "AbstractModel":
+        """
+        Returns a copy of this object with all priors, prior models and
+        constants removed.
+        """
+        without_attributes = copy.copy(self)
+        for key in self.__dict__:
+            if not (key.startswith("_") or key in ("cls", "id")):
+                delattr(without_attributes, key)
+        return without_attributes
+
+    def _with_paths(self, tree: dict) -> "AbstractModel":
+        """
+        Recursively generate a copy of this model retaining only objects
+        specified by the tree.
+
+        Parameters
+        ----------
+        tree
+            A tree formed of dictionaries describing which components of the
+            model should be retained.
+
+        Returns
+        -------
+        A copy of this model with a subset of attributes
+        """
+        if len(tree) == 0:
+            return self
+
+        with_paths = self.without_attributes()
+        for name, subtree in tree.items():
+            # noinspection PyProtectedMember
+            new_value = getattr(self, name)
+            if isinstance(
+                new_value,
+                (
+                    AbstractPriorModel,
+                    TuplePrior,
+                ),
+            ):
+                new_value = new_value._with_paths(subtree)
+            setattr(with_paths, name, new_value)
+        return with_paths
+
+    @split_paths
+    def with_paths(self, paths: List[Tuple[str, ...]]) -> "AbstractModel":
+        """
+        Recursively generate a copy of this model retaining only objects
+        specified by the list of paths.
+
+        Parameters
+        ----------
+        paths
+            A list of tuples of strings each of which points to a retained attribute.
+            All children of a given path are retained.
+
+        Returns
+        -------
+        A copy of this model with a subset of attributes
+        """
+        return self._with_paths(paths_to_tree(paths))
+
+    def _without_paths(self, tree: dict) -> "AbstractModel":
+        """
+        Recursively generate a copy of this model removing objects
+        specified by the tree.
+
+        Parameters
+        ----------
+        tree
+            A tree formed of dictionaries describing which components of the
+            model should be removed.
+
+        Returns
+        -------
+        A copy of this model with a subset of attributes
+        """
+        without_paths = copy.deepcopy(self)
+        for name, subtree in tree.items():
+            # noinspection PyProtectedMember
+            if len(subtree) == 0:
+                delattr(without_paths, name)
+            else:
+                new_value = getattr(without_paths, name)
+                if isinstance(
+                    new_value,
+                    (
+                        AbstractPriorModel,
+                        TuplePrior,
+                    ),
+                ):
+                    new_value = new_value._without_paths(subtree)
+                setattr(without_paths, name, new_value)
+        return without_paths
+
+    @split_paths
+    def without_paths(self, paths: List[Tuple[str, ...]]) -> "AbstractModel":
+        """
+        Recursively generate a copy of this model retaining only objects
+        not specified by the list of paths.
+
+        Parameters
+        ----------
+        paths
+            A list of tuples of strings each of which points to removed attribute.
+            All children of a given path are removed.
+
+        Returns
+        -------
+        A copy of this model with a subset of attributes
+        """
+        return self._without_paths(paths_to_tree(paths))
+
+    def index(self, path: Tuple[str, ...]) -> int:
+        """
+        Retrieve the index of a given path in the model
+        """
+        return self.paths.index(path)
+
+    @property
+    def mean_field(self) -> MeanField:
+        """
+        Implements the same interface as the graphical code
+        """
+        return MeanField(self)
+
+    @classmethod
+    def from_json(cls, file: str):
+        """
+        Loads the model from a .json file, which was written using the model's dictionary (`dict`) attribute as
+        follows:
+
+        import json
+
+        with open(filename, "w+") as f:
+            json.dump(model.dict, f, indent=4)
+
+        Parameters
+        ----------
+        file
+            The path and name of the .json file the model is loaded from.
+
+        Returns
+        -------
+        object
+            The model, which may be a `Collection` of `Model` objects or a single `Model`.
+        """
+
+        with open(file) as json_file:
+            model_dict = json.load(json_file)
+
+        return cls.from_dict(d=model_dict)
+
+    def add_assertion(self, assertion, name=""):
+        """
+        Assert that some relationship holds between physical values associated with
+        priors at the point an instance is created. If this fails a FitException is
+        raised causing the model to be re-sampled.
+        Parameters
+        ----------
+        assertion
+            An assertion that one prior must be greater than another.
+        name
+            A name describing the assertion that is logged when it is violated.
+        """
+        if assertion is True:
+            return
+        try:
+            assertion.name = name
+        except AttributeError:
+            pass
+        self._assertions.append(assertion)
+
+    @property
+    def name(self):
+        return self.__class__.__name__
+
+    # noinspection PyUnusedLocal
+    @staticmethod
+    def from_object(t, *args, **kwargs):
+        if inspect.isclass(t):
+            from .prior_model import Model
+
+            obj = object.__new__(Model)
+            obj.__init__(t, **kwargs)
+        elif isinstance(t, list) or isinstance(t, dict):
+            from autofit.mapper.prior_model import collection
+
+            obj = object.__new__(collection.Collection)
+            obj.__init__(t)
+        else:
+            obj = t
+        return obj
+
+    def take_attributes(self, source: object):
+        """
+        Take all attributes with a matching path from the source prior model.
+
+        For example, if this prior model has a prior "one" and a matching prior
+        is found associated with the source model then that attribute is attached
+        to this model.
+
+        If no matching attribute is found nothing happens.
+
+        Parameters
+        ----------
+        source
+            An instance or prior model from a previous search from which attributes
+            are passed to this model.
+        """
+
+        def assert_no_assertions(obj):
+            if len(getattr(obj, "_assertions", [])) > 0:
+                raise AssertionError(
+                    "take_attributes cannot be called once assertions have been added to the target"
+                )
+
+        assert_no_assertions(self)
+
+        for path, _ in sum(
+            map(self.path_instance_tuples_for_class, (Prior, float, TuplePrior)), []
+        ):
+            try:
+                item = copy.copy(source)
+                if isinstance(item, dict):
+                    from autofit.mapper.prior_model.collection import Collection
+
+                    item = Collection(item)
+                for attribute in path:
+                    if isinstance(attribute, int):
+                        item = item[attribute]
+                    else:
+                        item = copy.copy(getattr(item, attribute))
+
+                target = self
+                for attribute in path[:-1]:
+                    if isinstance(attribute, int):
+                        target = target[attribute]
+                    else:
+                        target = getattr(target, attribute)
+                    assert_no_assertions(target)
+
+                attribute = path[-1]
+                if isinstance(attribute, int):
+                    target[attribute] = item
+                else:
+                    setattr(target, path[-1], item)
+            except AttributeError:
+                pass
+
+    def instance_from_unit_vector(self, unit_vector, ignore_prior_limits=False):
+        """
+        Returns a ModelInstance, which has an attribute and class instance corresponding
+        to every `Model` attributed to this instance.
+        This method takes as input a unit vector of parameter values, converting each to
+        physical values via their priors.
+        Parameters
+        ----------
+        ignore_prior_limits
+            If true then no exception is thrown if priors fall outside defined limits
+        unit_vector: [float]
+            A unit hypercube vector that is mapped to an instance of physical values via the priors.
+        Returns
+        -------
+        model_instance : autofit.mapper.model.ModelInstance
+            An object containing reconstructed model_mapper instances
+        Raises
+        ------
+        exc.FitException
+            If any assertion attached to this object returns False.
+        """
+        exception_tuples = self.attribute_tuples_with_type(ConfigException)
+        if len(exception_tuples) > 0:
+            for name, exception in exception_tuples:
+                logger.exception(f"Could not load {name} because:\n\n{exception}")
+            names = [name for name, _ in exception_tuples]
+            raise ConfigException(
+                f"No configuration was found for some attributes ({', '.join(names)})"
+            )
+
+        if self.prior_count != len(unit_vector):
+            raise AssertionError(
+                f"prior_count ({self.prior_count}) != len(unit_vector) {len(unit_vector)}"
+            )
+
+        arguments = dict(
+            map(
+                lambda prior_tuple, unit: (
+                    prior_tuple.prior,
+                    prior_tuple.prior.value_for(
+                        unit,
+                        ignore_prior_limits=ignore_prior_limits,
+                    ),
+                ),
+                self.prior_tuples_ordered_by_id,
+                unit_vector,
+            )
+        )
+
+        return self.instance_for_arguments(
+            arguments,
+            ignore_assertions=ignore_prior_limits,
+        )
+
+    @property
+    @cast_collection(PriorNameValue)
+    @frozen_cache
+    def unique_prior_tuples(self):
+        """
+        Returns
+        -------
+        prior_tuple_dict: [(Prior, PriorTuple)]
+            The set of all priors associated with this mapper
+        """
+        return list(
+            {
+                prior_tuple[1]: prior_tuple
+                for prior_tuple in self.attribute_tuples_with_type(Prior)
+            }.values()
+        )
+
+    @property
+    @cast_collection(PriorNameValue)
+    @frozen_cache
+    def prior_tuples_ordered_by_id(self):
+        """
+        Returns
+        -------
+        priors: [Prior]
+            An ordered list of unique priors associated with this mapper
+        """
+        return sorted(
+            list(self.unique_prior_tuples), key=lambda prior_tuple: prior_tuple.prior.id
+        )
+
+    @property
+    def priors_ordered_by_id(self):
+        return [prior for _, prior in self.prior_tuples_ordered_by_id]
+
+    def vector_from_unit_vector(self, unit_vector, ignore_prior_limits=False):
+        """
+        Parameters
+        ----------
+        unit_vector: [float]
+            A unit hypercube vector
+        ignore_prior_limits
+            Set to True to prevent an exception being raised if
+            the physical value of a prior is outside the allowable
+            limits
+
+        Returns
+        -------
+        values: [float]
+            A vector with values output by priors
+        """
+        return list(
+            map(
+                lambda prior_tuple, unit: prior_tuple.prior.value_for(
+                    unit, ignore_prior_limits=ignore_prior_limits
+                ),
+                self.prior_tuples_ordered_by_id,
+                unit_vector,
+            )
+        )
+
+    def random_unit_vector_within_limits(
+        self, lower_limit: float = 0.0, upper_limit: float = 1.0
+    ) -> List[float]:
+        """
+        Generate a random vector of unit values by drawing uniform random values between 0 and 1.
+
+        Returns
+        -------
+        unit_values
+            A list of unit values constructed by taking random values from each prior.
+        """
+        return [
+            random.uniform(
+                max(lower_limit, prior.lower_unit_limit),
+                min(upper_limit, prior.upper_unit_limit),
+            )
+            for prior in self.priors_ordered_by_id
+        ]
+
+    def random_vector_from_priors_within_limits(
+        self, lower_limit: float = 0.0, upper_limit: float = 1.0
+    ) -> List[float]:
+        """
+        Returns a random vector of physical values by drawing uniform random values between lower and upper limits
+        defined as unit values, using the model priors to map them from unit values to physical values.
+
+        This function guesses infinite unit vectors, until one is randomly sampled whose physical parameters are within
+        the model's phyiscal limits.
+
+        This is used for MCMC initialization, whereby the starting points of a walker(s) are confined to a restricted
+        range of prior space. In particular, it is used for generate the "ball" initialization of Emcee.
+
+        Parameters
+        ----------
+        lower_limit
+            The lower limit as a unit value within which unit values (which are converted to physical values via the
+            priors) are generated.
+        upper_limit
+            The upper limit as a unit value within which unit values (which are converted to physical values via the
+            priors) are generated.
+
+        Returns
+        -------
+        physical_values
+            A list of physical values constructed by taking the mean possible value from
+            each prior.
+        """
+        vector = []
+
+        for prior in self.priors_ordered_by_id:
+            vector.append(
+                prior.random(
+                    lower_limit=lower_limit,
+                    upper_limit=upper_limit,
+                )
+            )
+
+        return vector
+
+    def random_instance_from_priors_within_limits(
+        self, lower_limit: float = 0.0, upper_limit: float = 1.0
+    ):
+        """
+        Returns a random instance of physical values by drawing uniform random values between lower and upper limits
+        defined as unit values, using the model priors to map them from unit values to physical values.
+
+        This function guesses infinite unit vectors, until one is randomly sampled whose physical parameters are within
+        the model's phyiscal limits. The final unit vector is then mapped to an instance.
+
+        Parameters
+        ----------
+        lower_limit
+            The lower limit as a unit value within which unit values (which are converted to physical values via the
+            priors) are generated.
+        upper_limit
+            The upper limit as a unit value within which unit values (which are converted to physical values via the
+            priors) are generated.
+
+        Returns
+        -------
+        physical_values
+            A list of physical values constructed by taking the mean possible value from
+            each prior.
+        """
+
+        vector = self.random_vector_from_priors_within_limits(
+            lower_limit=lower_limit, upper_limit=upper_limit
+        )
+
+        return self.instance_from_vector(vector=vector)
+
+    @property
+    def random_vector_from_priors(self):
+        """Generate a random vector of physical values by drawing uniform random values between 0 and 1 and using
+        the model priors to map them from unit values to physical values.
+        Returns
+        -------
+        physical_values: [float]
+            A list of physical values constructed by taking random values from each prior.
+        """
+        return self.random_vector_from_priors_within_limits(
+            lower_limit=0.0, upper_limit=1.0
+        )
+
+    @property
+    def physical_values_from_prior_medians(self):
+        """
+        Returns
+        -------
+        physical_values: [float]
+            A list of physical values constructed by taking the mean possible value from
+            each prior.
+        """
+        return self.vector_from_unit_vector([0.5] * len(self.unique_prior_tuples))
+
+    def instance_from_vector(self, vector, ignore_prior_limits=False):
+        """
+        Returns a ModelInstance, which has an attribute and class instance corresponding
+        to every `Model` attributed to this instance.
+        This method takes as input a physical vector of parameter values, thus omitting
+        the use of priors.
+        Parameters
+        ----------
+        vector: [float]
+            A vector of physical parameter values that is mapped to an instance.
+        ignore_prior_limits
+            If True don't check that physical values are within expected limits.
+
+        Returns
+        -------
+        model_instance : autofit.mapper.model.ModelInstance
+            An object containing reconstructed model_mapper instances
+        """
+        if len(vector) != self.prior_count:
+            raise AssertionError(
+                f"Vector length {len(vector)} != prior count {self.prior_count}"
+            )
+        arguments = dict(
+            map(
+                lambda prior_tuple, physical_unit: (prior_tuple.prior, physical_unit),
+                self.prior_tuples_ordered_by_id,
+                vector,
+            )
+        )
+
+        if not ignore_prior_limits:
+            for prior, value in arguments.items():
+                prior.assert_within_limits(value)
+
+        return self.instance_for_arguments(
+            arguments,
+            ignore_assertions=ignore_prior_limits,
+        )
+
+    def has(self, cls: Union[Type, Tuple[Type, ...]]) -> bool:
+        """
+        Parameters
+        ----------
+        cls
+            The type to check for
+
+        Returns
+        -------
+        True iff this model contains an instance or model with the given
+        type recursively. Includes models which have zero priors.
+        """
+        return self.has_instance(cls) or self.has_model(
+            cls, include_zero_dimension=True
+        )
+
+    def has_instance(self, cls) -> bool:
+        """
+        True iff this model contains an instance of type
+        cls, recursively.
+        """
+        return len(self.attribute_tuples_with_type(cls)) > 0
+
+    def has_model(self, cls, include_zero_dimension=False) -> bool:
+        """
+        True iff this model contains a Model of type
+        cls, recursively.
+        """
+        return (
+            len(
+                self.model_tuples_with_type(
+                    cls,
+                    include_zero_dimension=include_zero_dimension,
+                )
+            )
+            > 0
+        )
+
+    def is_only_model(self, cls) -> bool:
+        """
+        True iff this model contains at least one Model
+        of type cls and contains no PriorModels that are not
+        of type cls, recursively.
+        """
+        from .prior_model import Model
+
+        cls_models = self.model_tuples_with_type(cls)
+        other_models = [
+            value
+            for _, value in self.attribute_tuples_with_type(Model)
+            if value.prior_count > 0
+        ]
+        return len(cls_models) > 0 and len(cls_models) == len(other_models)
+
+    def replacing(self, arguments):
+        return self.mapper_from_partial_prior_arguments(arguments)
+
+    @classmethod
+    def product(cls, models: Iterable["AbstractPriorModel"]) -> "AbstractPriorModel":
+        """
+        Combine multiple models with the same structure by replacing priors with
+        priors that contain a message which is the product of the messages of the
+        priors with the same path in each model.
+
+        Parameters
+        ----------
+        models
+            A list of models to be combined
+
+        Returns
+        -------
+        A model where each prior has a message which is the product of the messages
+        associated with that prior across the models.
+        """
+        first, *rest = models
+
+        arguments = dict()
+
+        for path, prior in first.path_priors_tuples:
+            for other in rest:
+                prior = prior.with_message(
+                    prior.message * other.object_for_path(path).message
+                )
+            arguments[prior] = prior
+        return first.mapper_from_prior_arguments(arguments)
+
+    def mapper_from_partial_prior_arguments(self, arguments):
+        """
+        Returns a new model mapper from a dictionary mapping existing priors to
+        new priors, keeping existing priors where no mapping is provided.
+        Parameters
+        ----------
+        arguments: {Prior: Prior}
+            A dictionary mapping priors to priors
+        Returns
+        -------
+        model_mapper: ModelMapper
+            A new model mapper with updated priors.
+        """
+        original_prior_dict = {prior: prior for prior in self.priors}
+        return self.mapper_from_prior_arguments({**original_prior_dict, **arguments})
+
+    def mapper_from_prior_arguments(self, arguments):
+        """
+        Returns a new model mapper from a dictionary mapping existing priors to
+        new priors.
+        Parameters
+        ----------
+        arguments: {Prior: Prior}
+            A dictionary mapping priors to priors
+        Returns
+        -------
+        model_mapper: ModelMapper
+            A new model mapper with updated priors.
+        """
+        logger.debug(f"Creating a new mapper from arguments")
+
+        return self.gaussian_prior_model_for_arguments(arguments)
+
+    def gaussian_prior_model_for_arguments(self, arguments):
+        raise NotImplementedError()
+
+    def mapper_from_prior_means(self, means, a=None, r=None, no_limits=False):
+        """
+        The widths of the new priors are taken from the
+        width_config. The new gaussian priors must be provided in the same order as
+        the priors associated with model.
+        If a is not None then all priors are created with an absolute width of a.
+        If r is not None then all priors are created with a relative width of r.
+        Parameters
+        ----------
+        means
+            The median PDF value of every Gaussian, which centres each `GaussianPrior`.
+        no_limits
+            If `True` generated priors have infinite limits
+        r
+            The relative width to be assigned to gaussian priors
+        a
+            print(tuples[i][1], width)
+            The absolute width to be assigned to gaussian priors
+        tuples
+            A list of tuples each containing the mean and width of a prior
+        Returns
+        -------
+        mapper: ModelMapper
+            A new model mapper with all priors replaced by gaussian priors.
+        """
+
+        prior_tuples = self.prior_tuples_ordered_by_id
+        prior_class_dict = self.prior_class_dict
+        arguments = {}
+
+        for prior_tuple, mean in zip(prior_tuples, means):
+            prior = prior_tuple.prior
+            cls = prior_class_dict[prior]
+
+            name = prior_tuple.name
+            # Use the name of the collection for configuration when a prior's name
+            # is just a number (i.e. its position in a collection)
+            if name.isdigit():
+                name = self.path_for_prior(prior_tuple.prior)[-2]
+
+            width_modifier = (
+                prior.width_modifier
+                or WidthModifier.for_class_and_attribute_name(cls, name)
+            )
+
+            if a is not None and r is not None:
+                raise exc.PriorException(
+                    "Width of new priors cannot be both relative and absolute."
+                )
+            if a is not None:
+                width = a
+            elif r is not None:
+                width = r * mean
+            else:
+                width = width_modifier(mean)
+
+            if no_limits:
+                limits = (float("-inf"), float("inf"))
+            else:
+                try:
+                    limits = Limits.for_class_and_attributes_name(cls, name)
+                except ConfigException:
+                    limits = prior.limits
+
+            sigma = width
+
+            new_prior = GaussianPrior(mean, sigma, *limits)
+            new_prior.id = prior.id
+            new_prior.width_modifier = prior.width_modifier
+            arguments[prior] = new_prior
+
+        return self.mapper_from_prior_arguments(arguments)
+
+    def with_limits(self, limits: List[Tuple[float, float]]) -> "AbstractPriorModel":
+        """
+        Create a new instance of this model where each prior is updated to
+        lie between new limits.
+
+        Parameters
+        ----------
+        limits
+            A list of pairs of lower and upper limits, one for each prior.
+
+        Returns
+        -------
+        A new model with updated limits
+        """
+        return self.mapper_from_prior_arguments(
+            {
+                prior: prior.with_limits(*prior_limits)
+                for prior, prior_limits in zip(self.priors_ordered_by_id, limits)
+            }
+        )
+
+    def mapper_from_uniform_floats(self, floats, b):
+        """
+        The widths of the new priors are the `floats` value minus and plus the input bound `b`.
+
+        Parameters
+        ----------
+        floats
+            A list of floats each containing the centre of the new uniform priors.
+        b
+            The bound value which is subtracted from each float to calculate the `lower_limit` and `upper_limit`
+            of each uniform prior.
+
+        Returns
+        -------
+        mapper: ModelMapper
+            A new model mapper with all priors replaced by uniform priors.
+        """
+
+        prior_tuples = self.prior_tuples_ordered_by_id
+        arguments = {}
+
+        for i, prior_tuple in enumerate(prior_tuples):
+            prior = prior_tuple.prior
+
+            new_prior = UniformPrior(
+                lower_limit=floats[i] - b, upper_limit=floats[i] + b
+            )
+            new_prior.id = prior.id
+            arguments[prior] = new_prior
+
+        return self.mapper_from_prior_arguments(arguments)
+
+    def instance_from_prior_medians(self, ignore_prior_limits=False):
+        """
+        Returns a list of physical values from the median values of the priors.
+        Returns
+        -------
+        physical_values : [float]
+            A list of physical values
+        """
+        return self.instance_from_unit_vector(
+            unit_vector=[0.5] * self.prior_count,
+            ignore_prior_limits=ignore_prior_limits,
+        )
+
+    def log_prior_list_from_vector(
+        self,
+        vector: [float],
+    ):
+        """
+        Compute the log priors of every parameter in a vector, using the Prior of every parameter.
+        The log prior values are used by Emcee to map the log likelihood to the poserior of the model.
+        Parameters
+        ----------
+        vector : [float]
+            A vector of physical parameter values.
+        Returns
+        -------
+        log_prior_list : []
+            An list of the log prior value of every parameter.
+        """
+        return list(
+            map(
+                lambda prior_tuple, value: prior_tuple.prior.log_prior_from_value(
+                    value=value
+                ),
+                self.prior_tuples_ordered_by_id,
+                vector,
+            )
+        )
+
+    def random_instance(self, ignore_prior_limits=False):
+        """
+        Returns a random instance of the model.
+        """
+        logger.debug(f"Creating a random instance")
+        if ignore_prior_limits:
+            return self.instance_from_unit_vector(
+                unit_vector=[random.random() for _ in range(self.prior_count)],
+                ignore_prior_limits=ignore_prior_limits,
+            )
+        return self.instance_for_arguments(
+            {prior: prior.random() for prior in self.priors}
+        )
+
+    @staticmethod
+    @DynamicRecursionCache()
+    def from_instance(
+        instance,
+        model_classes: Union[type, Iterable[type]] = tuple(),
+        exclude_classes: Union[type, Iterable[type]] = tuple(),
+    ):
+        """
+        Recursively create a prior object model from an object model.
+
+        Parameters
+        ----------
+        model_classes
+            A tuple of classes that should be converted to a prior model
+        exclude_classes
+            A tuple of classes that should not be converted to a prior model
+        instance
+            A dictionary, list, class instance or model instance
+        Returns
+        -------
+        abstract_prior_model
+            A concrete child of an abstract prior model
+        """
+        from autofit.mapper.prior_model import collection
+
+        if isinstance(instance, exclude_classes):
+            return instance
+        if isinstance(instance, (Prior, AbstractPriorModel)):
+            return instance
+        elif isinstance(instance, list):
+            result = collection.Collection(
+                [
+                    AbstractPriorModel.from_instance(
+                        item,
+                        model_classes=model_classes,
+                        exclude_classes=exclude_classes,
+                    )
+                    for item in instance
+                ]
+            )
+        elif isinstance(instance, model.ModelInstance):
+            from autofit.mapper import model_mapper
+
+            result = model_mapper.ModelMapper()
+            for key, value in instance.dict.items():
+                setattr(
+                    result,
+                    key,
+                    AbstractPriorModel.from_instance(
+                        value,
+                        model_classes=model_classes,
+                        exclude_classes=exclude_classes,
+                    ),
+                )
+        elif isinstance(instance, dict):
+            result = collection.Collection(
+                {
+                    key: AbstractPriorModel.from_instance(
+                        value,
+                        model_classes=model_classes,
+                        exclude_classes=exclude_classes,
+                    )
+                    for key, value in instance.items()
+                }
+            )
+        elif isinstance(instance, (np.ndarray, types.FunctionType)):
+            return instance
+        else:
+            from .prior_model import Model
+
+            try:
+                result = Model(
+                    instance.__class__,
+                    **{
+                        key: AbstractPriorModel.from_instance(
+                            value,
+                            model_classes=model_classes,
+                            exclude_classes=exclude_classes,
+                        )
+                        for key, value in instance.__dict__.items()
+                        if key != "cls"
+                    },
+                )
+            except AttributeError:
+                return instance
+        if isinstance(instance, model_classes):
+            return result.as_model()
+        return result
+
+    def items(self):
+        return [
+            (key, value)
+            for key, value in self.__dict__.items()
+            if not key.startswith("_") and key not in ("cls", "id")
+        ]
+
+    @property
+    @cast_collection(PriorNameValue)
+    def direct_prior_tuples(self):
+        return self.direct_tuples_with_type(Prior)
+
+    @property
+    @cast_collection(InstanceNameValue)
+    def direct_instance_tuples(self):
+        return self.direct_tuples_with_type(float)
+
+    @property
+    @cast_collection(PriorModelNameValue)
+    def prior_model_tuples(self):
+        return self.direct_tuples_with_type(AbstractPriorModel)
+
+    @property
+    @cast_collection(PriorModelNameValue)
+    def direct_prior_model_tuples(self):
+        return self.direct_tuples_with_type(AbstractPriorModel)
+
+    @property
+    @cast_collection(PriorModelNameValue)
+    def direct_tuple_priors(self):
+        return self.direct_tuples_with_type(TuplePrior)
+
+    @property
+    @cast_collection(PriorNameValue)
+    def tuple_prior_tuples(self):
+        """
+        Returns
+        -------
+        tuple_prior_tuples: [(String, TuplePrior)]
+        """
+        return self.direct_tuples_with_type(TuplePrior)
+
+    @property
+    @cast_collection(PriorNameValue)
+    def direct_prior_tuples(self):
+        """
+        Returns
+        -------
+        direct_priors: [(String, Prior)]
+        """
+        return self.direct_tuples_with_type(Prior)
+
+    @property
+    @cast_collection(DeferredNameValue)
+    def direct_deferred_tuples(self):
+        return self.direct_tuples_with_type(DeferredArgument)
+
+    @property
+    @cast_collection(PriorNameValue)
+    def prior_tuples(self):
+        """
+        Returns
+        -------
+        priors: [(String, Prior))]
+        """
+        # noinspection PyUnresolvedReferences
+        return self.attribute_tuples_with_type(Prior, ignore_children=True)
+
+    def __eq__(self, other):
+        return (
+            isinstance(other, AbstractPriorModel)
+            and self.direct_prior_model_tuples == other.direct_prior_model_tuples
+        )
+
+    @property
+    @cast_collection(InstanceNameValue)
+    def instance_tuples(self):
+        """
+        Returns
+        -------
+        instances: [(String, instance)]
+        """
+        return self.attribute_tuples_with_type(float, ignore_class=Prior)
+
+    @property
+    def prior_class_dict(self):
+        from autofit.mapper.prior_model.annotation import AnnotationPriorModel
+
+        d = {prior[1]: self.cls for prior in self.prior_tuples}
+        for prior_model in self.prior_model_tuples:
+            if not isinstance(prior_model[1], AnnotationPriorModel):
+                d.update(prior_model[1].prior_class_dict)
+        return d
+
+    def _instance_for_arguments(
+        self,
+        arguments: Dict[Prior, float],
+        ignore_assertions: bool = False,
+    ):
+        raise NotImplementedError()
+
+    def instance_for_arguments(
+        self,
+        arguments: Dict[Prior, float],
+        ignore_assertions: bool = False,
+    ):
+        """
+        Returns an instance of the model for a set of arguments
+
+        Parameters
+        ----------
+        arguments
+            Dictionary mapping priors to attribute analysis_path and value pairs
+        ignore_assertions
+            If True, assertions will not be checked
+
+        Returns
+        -------
+            An instance of the class
+        """
+        if not (
+            conf.instance["general"]["test"]["exception_override"] or ignore_assertions
+        ):
+            self.check_assertions(arguments)
+
+        logger.debug(f"Creating an instance for arguments")
+        return self._instance_for_arguments(
+            arguments,
+            ignore_assertions=ignore_assertions,
+        )
+
+    def path_for_name(self, name: str) -> Tuple[str, ...]:
+        """
+        Find the path to a prior in the model that matches
+        a given name.
+
+        For example, name_of_model_name_of_prior could match
+        (name_of_model, name_of_prior). Unfortunately it is
+        possible for ambiguity to occur. For example, another
+        valid path could be (name, of_model, name_of_prior)
+        in which case there is no way to determine which path
+        actually matches the name.
+
+        Parameters
+        ----------
+        name
+            A name for a prior where names of models and the
+            name of the prior have been joined by underscores.
+
+        Returns
+        -------
+        A path to that model
+
+        Raises
+        ------
+        AssertionError
+            Iff no matching path is found
+        """
+
+        def _explode_path(path_):
+            return tuple(string for part in path_ for string in part.split("_"))
+
+        exploded = tuple(name.split("_"))
+        for path, _ in self.path_priors_tuples:
+            exploded_path = _explode_path(path)
+            if exploded_path == exploded:
+                return path
+
+        for path, prior_tuple in self.path_instance_tuples_for_class(TuplePrior):
+            for name, prior in prior_tuple.prior_tuples:
+                total_path = path[:-1] + (name,)
+                exploded_path = _explode_path(total_path)
+                if exploded_path == exploded:
+                    return path + (name,)
+        raise AssertionError(f"No path was found matching {name}")
+
+    def instance_from_prior_name_arguments(
+        self, prior_name_arguments: Dict[str, float]
+    ):
+        """
+        Instantiate the model from the names of priors and
+        corresponding values.
+
+        Parameters
+        ----------
+        prior_name_arguments
+            The names of priors where names of models and the
+            name of the prior have been joined by underscores,
+            mapped to corresponding values.
+
+        Returns
+        -------
+        An instance of the model
+        """
+        return self.instance_from_path_arguments(
+            {
+                self.path_for_name(name): value
+                for name, value in prior_name_arguments.items()
+            }
+        )
+
+    def instance_from_path_arguments(self, path_arguments: Dict[Tuple[str], float]):
+        """
+        Create an instance from a dictionary mapping paths to tuples
+        to corresponding values.
+
+        Parameters
+        ----------
+        path_arguments
+            A dictionary mapping paths to priors to corresponding values.
+            Note that, for linked priors, each path only needs to be
+            specified once. If multiple paths for the same prior are
+            specified then the value for the last path will be used.
+
+        Returns
+        -------
+        An instance of the model
+        """
+        arguments = {
+            self.object_for_path(path): value for path, value in path_arguments.items()
+        }
+        return self._instance_for_arguments(arguments)
+
+    @property
+    def prior_count(self) -> int:
+        """
+        How many unique priors does this model contain?
+        """
+        return len(self.unique_prior_tuples)
+
+    @property
+    def total_free_parameters(self) -> int:
+        """
+        Returns the prior count, but with a name that is more easy to interpret for users.
+        """
+        return self.prior_count
+
+    @property
+    def priors(self):
+        return [prior_tuple.prior for prior_tuple in self.prior_tuples]
+
+    @property
+    def _prior_id_map(self):
+        return {prior.id: prior for prior in self.priors}
+
+    def prior_with_id(self, prior_id):
+        return self._prior_id_map[prior_id]
+
+    def name_for_prior(self, prior):
+        for prior_model_name, prior_model in self.direct_prior_model_tuples:
+            prior_name = prior_model.name_for_prior(prior)
+            if prior_name is not None:
+                return "{}_{}".format(prior_model_name, prior_name)
+        prior_tuples = self.prior_tuples
+        for name, p in prior_tuples:
+            if p == prior:
+                return name
+
+    def __hash__(self):
+        return self.id
+
+    def __add__(self, other):
+        if isinstance(other, Prior):
+            return other + self
+
+        result = copy.deepcopy(self)
+
+        for key, value in other.__dict__.items():
+            if not hasattr(result, key) or isinstance(value, Prior):
+                setattr(result, key, value)
+                continue
+            result_value = getattr(result, key)
+            if isinstance(value, AbstractPriorModel):
+                if isinstance(result_value, AbstractPriorModel):
+                    setattr(result, key, result_value + value)
+                else:
+                    setattr(result, key, value)
+
+        return result
+
+    def copy_with_fixed_priors(self, instance, excluded_classes=tuple()):
+        """
+        Recursively overwrite priors in the mapper with instance values from the
+        instance except where the containing class is the descendant of a listed class.
+        Parameters
+        ----------
+        excluded_classes
+            Classes that should be left model
+        instance
+            The best fit from the previous search
+        """
+        mapper = copy.deepcopy(self)
+        transfer_classes(instance, mapper, excluded_classes)
+        return mapper
+
+    @property
+    def path_priors_tuples(self) -> List[Tuple[Path, Prior]]:
+        path_priors_tuples = self.path_instance_tuples_for_class(Prior)
+        return sorted(path_priors_tuples, key=lambda item: item[1].id)
+
+    @property
+    def paths(self) -> List[Path]:
+        """
+        A list of paths to all the priors in the model, ordered by their
+        ids
+        """
+        return [path for path, _ in self.path_priors_tuples]
+
+    @property
+    def composition(self):
+        return [".".join(path) for path in self.paths]
+
+    def sort_priors_alphabetically(self, priors: Iterable[Prior]) -> List[Prior]:
+        """
+        Sort priors by their paths according to this model.
+
+        Parameters
+        ----------
+        priors
+            A set of priors
+
+        Returns
+        -------
+        Those priors sorted alphabetically by path.
+        """
+        return sorted(priors, key=lambda prior: self.path_for_prior(prior))
+
+    def path_for_prior(self, prior: Prior) -> Optional[Path]:
+        """
+        Find a path that points at the given tuple.
+        Returns the first path or None if no path is found.
+        Parameters
+        ----------
+        prior
+            A prior representing what's known about some dimension of the model.
+        Returns
+        -------
+        A path, a series of attributes that point to one location of the prior.
+        """
+        for path in self.all_paths_for_prior(prior):
+            return path
+        return None
+
+    def all_paths_for_prior(self, prior: Prior) -> Generator[Path, None, None]:
+        """
+        Find all paths that points at the given tuple.
+
+        Parameters
+        ----------
+        prior
+            A prior representing what's known about some dimension of the model.
+        Yields
+        -------
+        Paths, each a series of attributes that point to one location of the prior.
+        """
+        for path, path_prior in reversed(self.path_priors_tuples):
+            if path_prior == prior:
+                yield path
+
+    @property
+    def path_float_tuples(self):
+        return self.path_instance_tuples_for_class(float, ignore_class=Prior)
+
+    @property
+    def unique_prior_paths(self):
+        return [item[0] for item in self.unique_path_prior_tuples]
+
+    @property
+    def unique_path_prior_tuples(self):
+        unique = {item[1]: item for item in self.path_priors_tuples}.values()
+        return sorted(unique, key=lambda item: item[1].id)
+
+    @property
+    def prior_prior_model_dict(self):
+        """
+        Returns
+        -------
+        prior_prior_model_dict: {Prior: Model}
+            A dictionary mapping priors to associated prior models. Each prior will only
+            have one prior model; if a prior is shared by two prior models then one of
+            those prior models will be in this dictionary.
+        """
+        return {
+            prior: prior_model[1]
+            for prior_model in self.prior_model_tuples + [("model", self)]
+            for _, prior in prior_model[1].prior_tuples
+        }
+
+    def log_prior_list_from(self, parameter_lists: List[List]) -> List:
+        return [
+            sum(self.log_prior_list_from_vector(vector=vector))
+            for vector in parameter_lists
+        ]
+
+    @property
+    def info(self) -> str:
+        """
+        Use the priors that make up the model_mapper to generate information on each
+        parameter of the overall model.
+        This information is extracted from each priors *model_info* property.
+        """
+
+        formatter = TextFormatter(line_length=info_whitespace())
+
+        for t in find_groups(
+            [
+                t
+                for t in self.path_instance_tuples_for_class(
+                    (Prior, float, int, tuple, ConfigException), ignore_children=True
+                )
+                if t[0][-1] not in ("id", "item_number")
+            ],
+            limit=1,
+        ):
+            if isinstance(t[1], ConfigException):
+                t = (t[0], "Prior Missing: Enter Manually or Add to Config")
+
+            formatter.add(*t)
+
+        return "\n\n".join(
+            [
+                f"Total Free Parameters = {self.prior_count}",
+                f"{self.parameterization}",
+                formatter.text,
+            ]
+        )
+
+    @property
+    def order_no(self) -> str:
+        """
+        A string that can be used to order models by their
+        parametrisation.
+
+        Priors and constants are ordered by their paths and then
+        joined into a string which means that models with higher
+        associated values are consistently ordered later in a
+        collection.
+        """
+        values = [
+            str(float(value))
+            for _, value in sorted(
+                self.path_instance_tuples_for_class((Prior, float)), key=lambda t: t[0]
+            )
+        ]
+        return ":".join(values)
+
+    @property
+    def parameterization(self) -> str:
+        """
+        Describes the path to each of the PriorModels, its class
+        and its number of free parameters
+        """
+        from .prior_model import Model
+
+        formatter = TextFormatter(line_length=info_whitespace())
+
+        paths = []
+
+        for t in self.path_instance_tuples_for_class(
+            (
+                Prior,
+                float,
+                tuple,
+            ),
+            ignore_children=True,
+        ):
+            for i in range(len(t[0])):
+                path = t[0][:i]
+                obj = self.object_for_path(path)
+                if isinstance(obj, TuplePrior):
+                    continue
+                if isinstance(obj, AbstractPriorModel):
+                    n = obj.prior_count
+                else:
+                    n = 0
+                if isinstance(obj, Model):
+                    name = obj.cls.__name__
+                else:
+                    name = type(obj).__name__
+
+                paths.append((("model",) + path, f"{name} (N={n})"))
+
+        for group in find_groups(paths, limit=0):
+            formatter.add(*group)
+
+        return formatter.text
+
+    @property
+    def all_paths(self) -> List[Tuple[Path]]:
+        """
+        All possible paths to all priors grouped such that all
+        paths to the same prior are collected together in a tuple.
+        """
+        if self.prior_count == 0:
+            return []
+        paths, _ = zip(*self.all_paths_prior_tuples)
+        return paths
+
+    @property
+    def all_paths_prior_tuples(self) -> List[Tuple[Tuple[Path], Prior]]:
+        """
+        Maps a tuple containing all paths to a given prior to that prior.
+        """
+        prior_paths_dict = defaultdict(tuple)
+        for path, prior in self.path_priors_tuples:
+            prior_paths_dict[prior] += (path,)
+        return sorted(
+            [(paths, prior) for prior, paths in prior_paths_dict.items()],
+            key=lambda item: item[1].id,
+        )
+
+    @property
+    def all_names(self) -> List[Tuple[str]]:
+        """
+        All possible names for all priors grouped such that all
+        names for a given prior are collected together in a tuple.
+        """
+        if self.prior_count == 0:
+            return []
+        names, _ = zip(*self.all_name_prior_tuples)
+        return names
+
+    @property
+    def all_name_prior_tuples(self) -> List[Tuple[Tuple[str], Prior]]:
+        """
+        Maps a tuple containing all names for a given prior to that prior.
+        """
+        path_modifier = TuplePathModifier(self)
+        return [
+            (tuple(".".join(path_modifier(path)) for path in paths), prior)
+            for paths, prior in self.all_paths_prior_tuples
+        ]
+
+    @property
+    def model_component_and_parameter_names(self) -> List[str]:
+        """
+        Lists each parameter's name and path, and is used for labeling visualization with parameter labels.
+
+        The parameter names are determined from the class instance names of the model_mapper. Latex tags are properties
+        of each model class.
+        """
+        prior_paths = self.unique_prior_paths
+
+        tuple_filter = TuplePathModifier(self)
+
+        prior_paths = list(map(tuple_filter, prior_paths))
+
+        return [".".join(path) for path in prior_paths]
+
+    @property
+    def joined_paths(self) -> List[str]:
+        prior_paths = self.unique_prior_paths
+
+        return [".".join(path) for path in prior_paths]
+
+    @property
+    def parameter_names(self) -> List[str]:
+        """
+        Returns a list of labels containing the name of every parameter in a model.
+
+        This is used for displaying model results as text and for visualization.
+
+        The parameter labels are defined for every parameter of every model component in the config files label.ini and
+        label_format.ini.
+        """
+        return [parameter_name[-1] for parameter_name in self.unique_prior_paths]
+
+    @property
+    def parameter_labels(self) -> List[str]:
+        """
+        Returns a list of labels containing latex labels of every parameter in a model.
+
+        This is used for displaying model results as text and for visualization.
+
+        The parameter labels are defined for every parameter of every model component in the config files label.ini and
+        label_format.ini.
+        """
+
+        parameter_labels = []
+
+        for parameter_name in self.parameter_names:
+            parameter_label = frm.convert_name_to_label(
+                parameter_name=parameter_name, name_to_label=True
+            )
+            parameter_labels.append(parameter_label)
+
+        return parameter_labels
+
+    @property
+    def superscripts(self) -> List[str]:
+        """
+        Returns a list of the model component superscripts for every parameter in a model.
+
+
+        The class superscript labels are defined as the name of every model component in the `ModelMapper`. For
+        the example of a 1D Gaussian, if the model component name is `gaussian` three superscripts
+        with this string (corresponding to the parameters `centre`, `normalization` and `sigma`) will
+        be returned.
+
+        For a `Collection`, the name of the inner model components are used.
+
+        These superscripts may be overwritten by those returned from the `superscripts_config_overwrite` property,
+        which optionally loads the superscripts from a `.json` config file. This allows high levels of customization
+        in what superscripts are used.
+
+        This is used for displaying model results as text and for visualization.
+        """
+
+        prior_paths = self.unique_prior_paths
+
+        tuple_filter = TuplePathModifier(self)
+
+        prior_paths = map(tuple_filter, prior_paths)
+
+        superscripts = [path[-2] if len(path) > 1 else None for path in prior_paths]
+
+        return [
+            superscript if not superscript_overwrite else superscript_overwrite
+            for superscript, superscript_overwrite in zip(
+                superscripts, self.superscripts_overwrite_via_config
+            )
+        ]
+
+    @property
+    def superscripts_overwrite_via_config(self) -> List[str]:
+        """
+        Returns a list of the model component superscripts for every parameter in a model, which can be used to
+        overwrite the default superscripts used in the function above.
+
+        The class superscript labels are defined for a model component in the config file `notation/label.ini`. By
+        default, the model component names are used as superscripts (which are loaded via the method `superscripts`).
+        These are overwritten by the superscripts loaded via a  config in this function. If no value is present in the
+        config the model component names are used.
+
+        For the example of a 1D Gaussian, when instatiated as a model component it is typically given the
+        name `gaussian`. Thus, the string `gaussian` will be used as the supersript of every one its parameter labels
+        (`centre`, `normalization` and `sigma`). However, if the config file `label.ini` reads `Gaussian=g`, every
+        superscript for these parameters will instead be given the superscript `g`.
+
+        This is used for displaying model results as text and for visualization with.
+        """
+
+        superscripts = []
+
+        for prior_name, prior in self.prior_tuples_ordered_by_id:
+            cls = self.prior_class_dict[prior]
+            try:
+                superscript = conf.instance["notation"]["label"]["superscript"][
+                    cls.__name__
+                ]
+
+            except KeyError:
+                superscript = ""
+
+            superscripts.append(superscript)
+
+        return superscripts
+
+    @property
+    def parameter_labels_with_superscripts(self) -> List[str]:
+        """
+        Returns a list of the latex parameter label and superscript of every parameter in a model.
+
+        The parameter labels are defined for every parameter of every model component in the config file `label.ini`.
+        This file can also be used to overwrite superscripts, that are assigned based on the model component name.
+
+        This is used for displaying model results as text and for visualization, for example labelling parameters.
+        """
+
+        return [
+            f"{label}^{{\\rm {superscript}}}" if superscript else f"{label}"
+            for label, superscript in zip(self.parameter_labels, self.superscripts)
+        ]
+
+    @property
+    def parameter_labels_with_superscripts_latex(self) -> List[str]:
+        """
+        Returns a list of the latex parameter label and superscript of every parameter in a model.
+
+        The parameter labels are defined for every parameter of every model component in the config file `label.ini`.
+        This file can also be used to overwrite superscripts, that are assigned based on the model component name.
+
+        This is used for displaying model results as text and for visualization, for example labelling parameters.
+        """
+
+        return [f"${label}$" for label in self.parameter_labels_with_superscripts]
+
+
+def transfer_classes(instance, mapper, model_classes=None):
+    """
+    Recursively overwrite priors in the mapper with instance values from the
+    instance except where the containing class is the descendant of a listed class.
+    Parameters
+    ----------
+    model_classes
+        Classes whose descendants should not be overwritten
+    instance
+        The best fit from the previous search
+    mapper
+        The prior model from the previous search
+    """
+    from autofit.mapper.prior_model.annotation import AnnotationPriorModel
+
+    model_classes = model_classes or []
+    for key, instance_value in instance.__dict__.items():
+        try:
+            mapper_value = getattr(mapper, key)
+            if isinstance(mapper_value, Prior) or isinstance(
+                mapper_value, AnnotationPriorModel
+            ):
+                setattr(mapper, key, instance_value)
+                continue
+            if not any(isinstance(instance_value, cls) for cls in model_classes):
+                try:
+                    transfer_classes(instance_value, mapper_value, model_classes)
+                except AttributeError:
+                    setattr(mapper, key, instance_value)
+        except AttributeError:
+            pass
```

### Comparing `autofit-2024.1.27.4/autofit/mapper/prior_model/annotation.py` & `autofit-2024.5.16.0/autofit/mapper/prior_model/annotation.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/mapper/prior_model/attribute_pair.py` & `autofit-2024.5.16.0/autofit/mapper/prior_model/attribute_pair.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/mapper/prior_model/collection.py` & `autofit-2024.5.16.0/autofit/mapper/prior_model/collection.py`

 * *Files 14% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             setattr(instance, key, value)
         return instance
 
     def __contains__(self, item):
         return item in self._dict or item in self._dict.values()
 
     def __getitem__(self, item):
-        if item in self._dict:
+        if isinstance(item, str):
             return self._dict[item]
         return self.values[item]
 
     def __len__(self):
         return len(self.values)
 
     def __str__(self):
@@ -84,15 +84,19 @@
                 key: value.as_model()
                 if isinstance(value, AbstractPriorModel)
                 else value
                 for key, value in self.dict().items()
             }
         )
 
-    def __init__(self, *arguments, **kwargs):
+    def __init__(
+        self,
+        *arguments,
+        **kwargs,
+    ):
         """
         The object multiple Python classes are input into to create model-components, which has free parameters that
         are fitted by a non-linear search.
 
         Multiple Python classes can be input into a `Collection` in order to compose high dimensional models made of
         multiple model-components.
 
@@ -225,15 +229,19 @@
             if isinstance(value, AbstractPriorModel):
                 collection[key] = value.gaussian_prior_model_for_arguments(arguments)
             if isinstance(value, Prior):
                 collection[key] = arguments[value]
 
         return collection
 
-    def _instance_for_arguments(self, arguments):
+    def _instance_for_arguments(
+        self,
+        arguments,
+        ignore_assertions=False,
+    ):
         """
         Parameters
         ----------
         arguments: {Prior: float}
             A dictionary of arguments
 
         Returns
@@ -242,15 +250,18 @@
             A list of instances constructed from the list of prior models.
         """
         result = ModelInstance()
         for key, value in self.__dict__.items():
             if key.startswith("_"):
                 continue
             if isinstance(value, AbstractPriorModel):
-                value = value.instance_for_arguments(arguments)
+                value = value.instance_for_arguments(
+                    arguments,
+                    ignore_assertions=ignore_assertions,
+                )
             elif isinstance(value, Prior):
                 value = arguments[value]
             setattr(result, key, value)
         return result
 
     def gaussian_prior_model_for_arguments(self, arguments):
         """
```

### Comparing `autofit-2024.1.27.4/autofit/mapper/prior_model/prior_model.py` & `autofit-2024.5.16.0/autofit/mapper/prior_model/prior_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,19 @@
         if self.cls != other.cls:
             raise TypeError(
                 f"Cannot add PriorModels with different classes "
                 f"({self.cls.__name__} and {other.cls.__name__})"
             )
         return super().__add__(other)
 
-    def __init__(self, cls, **kwargs):
+    def __init__(
+        self,
+        cls,
+        **kwargs,
+    ):
         """
         The object a Python class is input into to create a model-component, which has free parameters that are fitted
         by a non-linear search.
 
         The ``Model`` object is flexible, and can create models from many input Python data structures
         (e.g. a list of classes, dictionary of classes, hierarchy of classes).
 
@@ -93,15 +97,17 @@
             ):
                 self.centre = centre
                 self.normalization = normalization
                 self.sigma = sigma
 
         model = af.Model(Gaussian)
         """
-        super().__init__(label=namer(cls.__name__) if inspect.isclass(cls) else None)
+        super().__init__(
+            label=namer(cls.__name__) if inspect.isclass(cls) else None,
+        )
         if cls is self:
             return
 
         if not (inspect.isclass(cls) or inspect.isfunction(cls)):
             raise AssertionError(f"{cls} is not a class or function")
 
         self.cls = cls
@@ -380,15 +386,19 @@
         self.__getattribute__(item)
 
     @property
     def is_deferred_arguments(self):
         return len(self.direct_deferred_tuples) > 0
 
     # noinspection PyUnresolvedReferences
-    def _instance_for_arguments(self, arguments: {ModelObject: object}):
+    def _instance_for_arguments(
+        self,
+        arguments: {ModelObject: object},
+        ignore_assertions=False,
+    ):
         """
         Returns an instance of the associated class for a set of arguments
 
         Parameters
         ----------
         arguments: {Prior: float}
             Dictionary mapping_matrix priors to attribute analysis_path and value pairs
@@ -410,14 +420,15 @@
             )
         for prior_model_tuple in self.direct_prior_model_tuples:
             prior_model = prior_model_tuple.prior_model
             model_arguments[
                 prior_model_tuple.name
             ] = prior_model.instance_for_arguments(
                 arguments,
+                ignore_assertions=ignore_assertions,
             )
 
         prior_arguments = dict()
 
         for name, prior in self.direct_prior_tuples:
             try:
                 prior_arguments[name] = arguments[prior]
@@ -444,15 +455,18 @@
             if (
                 not hasattr(result, key)
                 and not isinstance(value, Prior)
                 and not key == "cls"
                 and not key.startswith("_")
             ):
                 if isinstance(value, Model):
-                    value = value.instance_for_arguments(arguments)
+                    value = value.instance_for_arguments(
+                        arguments,
+                        ignore_assertions=ignore_assertions,
+                    )
                 elif isinstance(value, Prior):
                     value = arguments[value]
                 try:
                     setattr(result, key, value)
                 except AttributeError:
                     pass
```

### Comparing `autofit-2024.1.27.4/autofit/mapper/prior_model/recursion.py` & `autofit-2024.5.16.0/autofit/mapper/prior_model/recursion.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/mapper/variable.py` & `autofit-2024.5.16.0/autofit/mapper/variable.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/mapper/variable_operator.py` & `autofit-2024.5.16.0/autofit/mapper/variable_operator.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/messages/abstract.py` & `autofit-2024.5.16.0/autofit/messages/abstract.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/messages/beta.py` & `autofit-2024.5.16.0/autofit/messages/beta.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/messages/composed_transform.py` & `autofit-2024.5.16.0/autofit/messages/composed_transform.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import functools
-from typing import Tuple, Optional, Union
-
 import numpy as np
+import warnings
+from typing import Tuple, Optional, Union
 
-from autofit.messages.abstract import MessageInterface
+from autofit.messages.abstract import MessageInterface, AbstractMessage
 from autofit.messages.transform import AbstractDensityTransform
 
 
 def arithmetic(func):
     """
     When arithmetic is performed between a two transformed messages the
     operation is performed between the base messages and the result it
@@ -90,14 +90,21 @@
         self.transforms = transforms
         self.base_message = base_message
         self.id = id_
 
         self.lower_limit = lower_limit
         self.upper_limit = upper_limit
 
+        x0, x1 = zip(*base_message._support)
+        z0 = self._inverse_transform(np.array(x0))
+        z1 = self._inverse_transform(np.array(x1))
+        self._support = tuple(zip(z0, z1))
+
+    log_normalisation = AbstractMessage.log_normalisation
+
     def from_natural_parameters(self, new_params, **kwargs):
         return self.with_base(
             self.base_message.from_natural_parameters(new_params, **kwargs,)
         )
 
     @property
     def broadcast(self):
@@ -189,18 +196,35 @@
 
         Inverts transform (above)
         """
         for _transform in self.transforms:
             x = _transform.inv_transform(x)
         return x
 
-    def transform_det(self, x):
-        for _transform in self.transforms:
-            x = _transform.log_det(x)
-        return x
+    def _transform_det(self, x):
+
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+
+            logd = 0
+            for _transform in reversed(self.transforms):
+                x, _logd = _transform.transform_det(x)
+                logd += _logd
+            return x, logd
+    
+    def _transform_det_jac(self, x):
+        logd = 0
+        logd_jacs = []
+        for _transform in reversed(self.transforms):
+            x, _logd, _logd_grad, _jac = _transform.transform_det_jac(x)
+            logd += _logd
+            logd_jacs.append((_logd_grad, _jac))
+
+        return x, logd, logd_jacs
+
 
     def invert_natural_parameters(
         self, natural_parameters: np.ndarray,
     ) -> Tuple[np.ndarray, ...]:
         return self.base_message.invert_natural_parameters(natural_parameters)
 
     @transform
@@ -242,22 +266,17 @@
             variance = jacobian.invquad(variance)
 
         return variance
 
     @inverse_transform
     def _sample(self, n_samples) -> np.ndarray:
         return self.base_message._sample(n_samples)
-
-    def _factor(self, _, x: Union[np.ndarray, float],) -> np.ndarray:
-        log_det = self.transform_det(x)
-        x = self._transform(x)
-        eta = self.base_message._broadcast_natural_parameters(x)
-        t = self.base_message.to_canonical_form(x)
-        log_base = self.calc_log_base_measure(x) + log_det
-        return self.base_message.natural_logpdf(eta, t, log_base, self.log_partition)
+    
+    def exp_factor(self, x):
+        return np.exp(np.nan_to_num(self.factor(x), nan=-np.inf))
 
     def factor(self, x: Union[float, np.ndarray]) -> Union[np.ndarray, float]:
         """
         Call the factor. The closer to the mean a given value is the higher
         the probability returned.
 
         Parameters
@@ -265,15 +284,40 @@
         x
             A value in the space of the transformed message.
 
         Returns
         -------
         The probability this value is correct
         """
-        return self._factor(self, x)
+        x, logd = self._transform_det(x)
+        return self.base_message.logpdf(x) + logd
+    
+    def factor_gradient(self, x: Union[float, np.ndarray]) -> Tuple[Union[np.ndarray, float],Union[np.ndarray, float]]:
+        """
+        Call the factor. The closer to the mean a given value is the higher
+        the probability returned.
+
+        Parameters
+        ----------
+        x
+            A value in the space of the transformed message.
+
+        Returns
+        -------
+        The probability this value is correct
+        """
+        x, logd, logd_grad, jacs = self._transform_det_jac(x)
+        logp, grad = self.base_message.logpdf_gradient(x)
+        for jac in reversed(jacs):
+            grad = grad * jac 
+        return logp + logd, grad + logd_grad
+    
+
+
+    
 
     @property
     def multivariate(self):
         return self.base_message.multivariate
 
     def logpdf_gradient(self, x: np.ndarray) -> Tuple[np.ndarray, np.ndarray]:
         jacobians = []
```

### Comparing `autofit-2024.1.27.4/autofit/messages/fixed.py` & `autofit-2024.5.16.0/autofit/messages/fixed.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/messages/gamma.py` & `autofit-2024.5.16.0/autofit/messages/gamma.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/messages/interface.py` & `autofit-2024.5.16.0/autofit/messages/interface.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/messages/normal.py` & `autofit-2024.5.16.0/autofit/messages/normal.py`

 * *Files 4% similar despite different names*

```diff
@@ -174,15 +174,19 @@
         Examples
         --------
 
         prior = af.GaussianPrior(mean=1.0, sigma=2.0, lower_limit=0.0, upper_limit=2.0)
 
         physical_value = prior.value_for(unit=0.5)
         """
-        inv = erfinv(1 - 2.0 * (1.0 - unit))
+        try:
+            inv = erfinv(1 - 2.0 * (1.0 - unit))
+        except TypeError:
+            from scipy.special import erfinv as scipy_erfinv
+            inv = scipy_erfinv(1 - 2.0 * (1.0 - unit))
         return self.mean + (self.sigma * np.sqrt(2) * inv)
 
     def log_prior_from_value(self, value):
         """
         Returns the log prior of a physical value, so the log likelihood of a model evaluation can be converted to a
         posterior as log_prior + log_likelihood.
         This is used by certain non-linear searches (e.g. Emcee) in the log likelihood function evaluation.
@@ -291,12 +295,13 @@
 
 
 UniformNormalMessage = TransformedMessage(NormalMessage(0, 1), phi_transform)
 
 Log10UniformNormalMessage = TransformedMessage(UniformNormalMessage, log_10_transform)
 
 LogNormalMessage = TransformedMessage(NormalMessage(0, 1), log_transform)
+Log10NormalMessage = TransformedMessage(NormalMessage(0, 1), log_10_transform)
 
 # Support is the simplex
 MultiLogitNormalMessage = TransformedMessage(
     NormalMessage(0, 1), multinomial_logit_transform
 )
```

### Comparing `autofit-2024.1.27.4/autofit/messages/transform.py` & `autofit-2024.5.16.0/autofit/messages/transform.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import warnings
 from abc import ABC, abstractmethod
 from functools import wraps
 from typing import Tuple
 
 import numpy as np
 from scipy.special import ndtr, ndtri as ndtri_
 from scipy.stats._continuous_distns import _norm_pdf
@@ -34,19 +35,19 @@
 
 
 class AbstractDensityTransform(ABC):
     """
     This class allows the transformation of a probability density function, p(x)
     whilst preserving the measure of the distribution, i.e.
 
-    \int p(x) dx = 1
+    int p(x) dx = 1
 
     p'(f) = p(f(x)) * |df/dx|
 
-    \inf p'(f) df = 1
+    inf p'(f) df = 1
 
     Methods
     -------
     transform
         calculates f(x)
 
     inv_transform
@@ -169,15 +170,17 @@
 class LinearShiftTransform(LinearTransform):
     def __init__(self, shift: float = 0, scale: float = 1):
         self.shift = float(shift)
         self.scale = float(scale)
         super().__init__(DiagonalMatrix(np.reciprocal(self.scale)))
 
     def inv_transform(self, x: np.ndarray) -> np.ndarray:
-        return x * self.scale + self.shift
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+            return x * self.scale + self.shift
 
     def transform(self, x: np.ndarray) -> np.ndarray:
         return (x - self.shift) / self.scale
 
     def log_det(self, x: np.ndarray) -> np.ndarray:
         return -np.log(self.scale) * np.ones_like(x)
 
@@ -188,25 +191,36 @@
         self.inv_func = inv_func
         self.grad = grad
         self.hess = hess
         self.args = args
         self.func_grad_hess = func_grad_hess
 
     def transform(self, x):
-        return self.func(x, *self.args)
+
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+
+            return self.func(x, *self.args)
 
     def inv_transform(self, x):
-        return self.inv_func(x, *self.args)
+
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+
+            return self.inv_func(x, *self.args)
 
     def jacobian(self, x):
         return DiagonalMatrix(self.grad(x, *self.args))
 
     def log_det(self, x: np.ndarray) -> np.ndarray:
-        gs = self.grad(x, *self.args)
-        return np.log(gs)
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+
+            gs = self.grad(x, *self.args)
+            return np.log(gs)
 
     def log_det_grad(self, x: np.ndarray) -> Tuple[np.ndarray, np.ndarray]:
         if self.func_grad_hess:
             x0, gs, hs = self.func_grad_hess(x, *self.args)
         else:
             gs = self.grad(x, *self.args)
             hs = self.hess(x, *self.args)
@@ -239,17 +253,24 @@
 
 log_transform = FunctionTransform(np.log, np.exp, np.reciprocal, func_grad_hess=log3)
 
 
 def _log_10_inv(x):
     return 10**x
 
+LOG10 = np.log(10)
+def _log10_recip(x):
+    return np.reciprocal(x) / LOG10
+
+def log10_3(x):
+    ix = _log10_recip(x)
+    return np.log10(x), ix, -ix/x
 
 # TODO: what should func_grad_hess look like? np.log10, ... ?
-log_10_transform = FunctionTransform(np.log10, _log_10_inv, np.reciprocal)
+log_10_transform = FunctionTransform(np.log10, _log_10_inv, _log10_recip, func_grad_hess=log10_3)
 
 
 def sigmoid(x, scale=1, shift=0):
     return scale / (1 + np.exp(-x)) + shift
 
 
 def logit(x, scale=1, shift=0):
@@ -338,15 +359,17 @@
         p = np.asanyarray(p)
         lnp1 = np.log(1 - np.sum(p, axis=self.axis, keepdims=True))
         lnp = np.log(p)
         return lnp - lnp1
 
     def inv_transform(self, x):
         expx = np.exp(x)
-        return expx / (expx.sum(axis=self.axis, keepdims=True) + 1)
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+            return expx / (expx.sum(axis=self.axis, keepdims=True) + 1)
 
     def jacobian(self, p):
         p = np.asanyarray(p)
         pn1 = 1 - np.sum(p, axis=-1, keepdims=True)
         # ln1p = np.log(pn1)
         # lnp = np.log(p)
         return ShermanMorrison(
```

### Comparing `autofit-2024.1.27.4/autofit/messages/utils.py` & `autofit-2024.5.16.0/autofit/messages/utils.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/mock.py` & `autofit-2024.5.16.0/autofit/mock.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from autofit.non_linear.mock.mock_analysis import MockAnalysis
 from autofit.non_linear.mock.mock_result import MockResult
 from autofit.non_linear.mock.mock_result import MockResultGrid
 from autofit.non_linear.mock.mock_search import MockSearch
 from autofit.non_linear.mock.mock_search import MockOptimizer
+from autofit.non_linear.mock.mock_samples_summary import MockSamplesSummary
 from autofit.non_linear.mock.mock_samples import MockSamples
 from autofit.non_linear.mock.mock_samples import MockSamplesNest
 
 from autofit.mapper.mock.mock_model import MockChildTuple
 from autofit.mapper.mock.mock_model import MockClassInf
 from autofit.mapper.mock.mock_model import MockClassRelativeWidth
 from autofit.mapper.mock.mock_model import MockChildTuplex3
```

### Comparing `autofit-2024.1.27.4/autofit/non_linear/analysis/combined.py` & `autofit-2024.5.16.0/autofit/non_linear/analysis/combined.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,44 @@
 import logging
-from typing import Union, List
+from typing import Union, List, Optional
 
 from autoconf import conf
 from autofit.mapper.prior.abstract import Prior
 from autofit.mapper.prior.tuple_prior import TuplePrior
 from autofit.mapper.prior_model.abstract import AbstractPriorModel
 from autofit.non_linear.analysis.multiprocessing import AnalysisPool
 from autofit.non_linear.paths.abstract import AbstractPaths
 from autofit.non_linear.result import Result
 from .analysis import Analysis
+from autofit.non_linear.samples.summary import SamplesSummary
+from autofit.non_linear.samples import SamplesPDF
 
 logger = logging.getLogger(__name__)
 
 
 class CombinedResult:
-    def __init__(self, results: List[Result]):
+    def __init__(
+        self,
+        results: List[Result],
+        samples: Optional[SamplesPDF] = None,
+        samples_summary: Optional[SamplesSummary] = None,
+    ):
         """
         A `Result` object that is composed of multiple `Result` objects. This is used to combine the results of
         multiple `Analysis` objects into a single `Result` object, for example when performing a model-fitting
         analysis where there are multiple datasets.
 
         Parameters
         ----------
         results
             The list of `Result` objects that are combined into this `CombinedResult` object.
         """
         self.child_results = results
+        self.samples = samples
+        self.samples_summary = samples_summary
 
     def __getattr__(self, item: str):
         """
         Get an attribute of the first `Result` object in the list of `Result` objects.
         """
         if item in ("__getstate__", "__setstate__"):
             raise AttributeError(item)
@@ -191,14 +200,20 @@
 
     def save_results(self, paths: AbstractPaths, result: Result):
         def func(child_paths, analysis, result_):
             analysis.save_results(paths=child_paths, result=result_)
 
         self._for_each_analysis(func, paths, result)
 
+    def save_results_combined(self, paths: AbstractPaths, result: Result):
+        self.analyses[0].save_results_combined(
+            paths=paths,
+            result=result,
+        )
+
     def visualize_before_fit(self, paths: AbstractPaths, model: AbstractPriorModel):
         """
         Visualise the model before fitting.
 
         Visualisation output is distinguished by using an integer suffix
         for each analysis path.
 
@@ -217,15 +232,15 @@
 
         def func(child_paths, analysis):
             analysis.visualize_before_fit(child_paths, model)
 
         self._for_each_analysis(func, paths)
 
     def visualize_before_fit_combined(
-        self, analyses, paths: AbstractPaths, model: AbstractPriorModel
+        self, paths: AbstractPaths, model: AbstractPriorModel
     ):
         """
         Visualise images and quantities which are shared across all analyses.
 
         For example, each Analysis may have a different dataset, where the data in each dataset is intended to all
         be plotted on the same matplotlib subplot. This function can be overwritten to allow the visualization of such
         a plot.
@@ -234,15 +249,16 @@
         `analyses` property to access the other analyses and perform visualization.
 
         Parameters
         ----------
         paths
             An object describing the paths for saving data (e.g. hard-disk directories or entries in sqlite database).
         """
-        self.analyses[0].visualize_before_fit_combined(
+
+        self.analyses[0].Visualizer.visualize_before_fit_combined(
             analyses=self.analyses,
             paths=paths,
             model=model,
         )
 
     def visualize(self, paths: AbstractPaths, instance, during_analysis):
         """
@@ -272,15 +288,14 @@
         def func(child_paths, analysis):
             analysis.visualize(child_paths, instance, during_analysis)
 
         self._for_each_analysis(func, paths)
 
     def visualize_combined(
         self,
-        analyses: List["Analysis"],
         instance,
         paths: AbstractPaths,
         during_analysis,
     ):
         """
         Visualise the instance using images and quantities which are shared across all analyses.
 
@@ -296,15 +311,15 @@
         paths
             An object describing the paths for saving data (e.g. hard-disk directories or entries in sqlite database).
         instance
             The maximum likelihood instance of the model so far in the non-linear search.
         during_analysis
             Is this visualisation during analysis?
         """
-        self.analyses[0].visualize_combined(
+        self.analyses[0].Visualizer.visualize_combined(
             analyses=self.analyses,
             paths=paths,
             instance=instance,
             during_analysis=during_analysis,
         )
 
     def profile_log_likelihood_function(
@@ -329,18 +344,29 @@
             analysis.profile_log_likelihood_function(
                 child_paths,
                 instance,
             )
 
         self._for_each_analysis(func, paths)
 
-    def make_result(self, samples):
+    def make_result(
+        self,
+        samples_summary: SamplesSummary,
+        paths: AbstractPaths,
+        samples: Optional[SamplesPDF] = None,
+        search_internal: Optional[object] = None,
+        analysis: Optional[object] = None,
+    ):
         child_results = [
             analysis.make_result(
-                samples,
+                samples_summary=samples_summary,
+                paths=paths,
+                samples=samples,
+                search_internal=search_internal,
+                analysis=analysis
             )
             for analysis in self.analyses
         ]
         return CombinedResult(child_results)
 
     def __len__(self):
         return len(self.analyses)
```

### Comparing `autofit-2024.1.27.4/autofit/non_linear/analysis/free_parameter.py` & `autofit-2024.5.16.0/autofit/non_linear/analysis/free_parameter.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/non_linear/analysis/multiprocessing.py` & `autofit-2024.5.16.0/autofit/non_linear/analysis/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/non_linear/fitness.py` & `autofit-2024.5.16.0/autofit/non_linear/fitness.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,93 +1,108 @@
 import numpy as np
+import os
+from typing import Optional
 
 from autoconf import conf
 
 from autofit import exc
 
+from autofit.mapper.prior_model.abstract import AbstractPriorModel
+from autofit.non_linear.paths.abstract import AbstractPaths
+from autofit.non_linear.analysis import Analysis
+
 from timeout_decorator import timeout
 
 from autofit import jax_wrapper
 
 
 def get_timeout_seconds():
+
     try:
         return conf.instance["general"]["test"]["lh_timeout_seconds"]
     except KeyError:
         pass
 
 
 timeout_seconds = get_timeout_seconds()
 
 
 class Fitness:
     def __init__(
         self,
-        model,
-        analysis,
+        model : AbstractPriorModel,
+        analysis : Analysis,
+        paths : Optional[AbstractPaths] = None,
         fom_is_log_likelihood: bool = True,
         resample_figure_of_merit: float = -np.inf,
         convert_to_chi_squared: bool = False,
     ):
         """
-        Interfaces with any non-linear in order to fit a model to the data and return a log likelihood via
-        an `Analysis` class.
+        Interfaces with any non-linear search to fit the model to the data and return a log likelihood via
+        the analysis.
 
-        The interface of a non-linear search and a fitness function can be summarized as follows:
+        The interface of a non-linear search and fitness function is summarized as follows:
 
-        1) The non-linear search chooses a new set of parameters for the model, which are passed to the fitness
+        1) The non-linear search samples a new set of model parameters, which are passed to the fitness
         function's `__call__` method.
 
-        2) The parameter values (typically a list) are mapped to an instance of the model (via its priors if
-        appropriate for the non-linear search).
+        2) The list of parameter values are mapped to an instance of the model.
 
         3) The instance is passed to the analysis class's log likelihood function, which fits the model to the
         data and returns the log likelihood.
 
         4) A final figure-of-merit is computed and returned to the non-linear search, which is either the log
-        likelihood or log posterior depending on the type of non-linear search.
+        likelihood or log posterior (e.g. adding the log prior to the log likelihood).
+
+        Certain searches (commonly nested samplers) require the parameters to be mapped from unit values to physical
+        values, which is performed internally by the fitness object in step 2.
 
-        It is common for nested sampling algorithms to require that the figure of merit returned is a log likelihood
-        as priors are often built into the mapping of values from a unit hyper-cube. Optimizers and MCMC methods
-        typically require that the figure of merit returned is a log posterior, with the prior terms added via this
-        fitness function. This is not a strict rule, but is a good default.
-
-        Some methods also require a chi-squared value to be computed (which is minimized), which is the log likelihood
-        multiplied by -2.0. The `Fitness` class can also compute this value, if the `convert_to_chi_squared` bool is
-        `True`.
+        Certain searches require the returned figure of merit to be a log posterior (often MCMC methods) whereas
+        others require it to be a log likelihood (often nested samples which account for priors internally) in step 4.
+        Which values is returned by the `fom_is_log_likelihood` bool.
 
-        If a model-fit raises an exception of returns a `np.nan` a `resample_figure_of_merit` value is returned. The
-        appropriate value depends on the non-linear search, but is typically either `None`, `-np.inf` or `1.0e99`.
+        Some searches require a chi-squared value (which they minimized), given by the log likelihood multiplied
+        by -2.0. This is returned by the fitness if the `convert_to_chi_squared` bool is `True`.
+
+        If a model-fit raises an exception or returns a `np.nan`, a `resample_figure_of_merit` value is returned
+        instead. The appropriate value depends on the search, but is typically either `None`, `-np.inf` or `1.0e99`.
         All values indicate to the non-linear search that the model-fit should be resampled or ignored.
 
         Parameters
         ----------
         analysis
             An object that encapsulates the data and a log likelihood function which fits the model to the data
             via the non-linear search.
         model
             The model that is fitted to the data, which is used by the non-linear search to create instances of
             the model that are fitted to the data via the log likelihood function.
+        paths
+            The paths of the search, which if the search is being resumed from an old run is used to check that
+            the likelihood function has not changed from the previous run.
         fom_is_log_likelihood
             If `True`, the figure of merit returned by the fitness function is the log likelihood. If `False`, the
             figure of merit is the log posterior.
         resample_figure_of_merit
             The figure of merit returned if the model-fit raises an exception or returns a `np.nan`.
         convert_to_chi_squared
             If `True`, the figure of merit returned is the log likelihood multiplied by -2.0, such that it is a
             chi-squared value that is minimized.
         """
 
         self.analysis = analysis
         self.model = model
+        self.paths = paths
         self.fom_is_log_likelihood = fom_is_log_likelihood
         self.resample_figure_of_merit = resample_figure_of_merit
         self.convert_to_chi_squared = convert_to_chi_squared
         self._log_likelihood_function = None
 
+        if self.paths is not None:
+            self.check_log_likelihood(fitness=self)
+
     def __getstate__(self):
         state = self.__dict__.copy()
         del state["_log_likelihood_function"]
         return state
 
     def __setstate__(self, state):
         self.__dict__.update(state)
@@ -139,7 +154,64 @@
             log_prior_list = self.model.log_prior_list_from_vector(vector=parameters)
             figure_of_merit = log_likelihood + sum(log_prior_list)
 
         if self.convert_to_chi_squared:
             figure_of_merit *= -2.0
 
         return figure_of_merit
+
+    def check_log_likelihood(self, fitness):
+        """
+        Changes to the PyAutoGalaxy source code may inadvertantly change the numerics of how a log likelihood is
+        computed. Equally, one may set off a model-fit that resumes from previous results, but change the settings of
+        the pixelization or inversion in a way that changes the log likelihood function.
+
+        This function performs an optional sanity check, which raises an exception if the log likelihood calculation
+        changes, to ensure a model-fit is not resumed with a different likelihood calculation to the previous run.
+
+        If the model-fit has not been performed before (e.g. it is not a resume) this function outputs
+        the `figure_of_merit` (e.g. the log likelihood) of the maximum log likelihood model at the end of the model-fit.
+
+        If the model-fit is a resume, it loads this `figure_of_merit` and compares it against a new value computed for
+        the resumed run (again using the maximum log likelihood model inferred). If the two likelihoods do not agree
+        and therefore the log likelihood function has changed, an exception is raised and the code execution terminated.
+
+        Parameters
+        ----------
+        paths
+            certain searches the non-linear search outputs are stored,
+            visualization, and pickled objects used by the database and aggregator.
+        result
+            The result containing the maximum log likelihood fit of the model.
+        """
+
+        if os.environ.get("PYAUTOFIT_TEST_MODE") == "1":
+            return
+
+        if not conf.instance["general"]["test"]["check_likelihood_function"]:
+            return
+
+        try:
+            samples_summary = self.paths.load_samples_summary()
+        except FileNotFoundError:
+            return
+
+        max_log_likelihood_sample = samples_summary.max_log_likelihood_sample
+        log_likelihood_old = samples_summary.max_log_likelihood_sample.log_likelihood
+
+        parameters = max_log_likelihood_sample.parameter_lists_for_model(model=self.model)
+
+        log_likelihood_new = fitness(parameters=parameters)
+
+        if not np.isclose(log_likelihood_old, log_likelihood_new):
+            raise exc.SearchException(
+                f"""
+                Figure of merit sanity check failed. 
+
+                This means that the existing results of a model fit used a different
+                likelihood function compared to the one implemented now.
+                Old Figure of Merit = {log_likelihood_old}
+                New Figure of Merit = {log_likelihood_new}
+                """
+            )
+
+
```

### Comparing `autofit-2024.1.27.4/autofit/non_linear/grid/grid_list.py` & `autofit-2024.5.16.0/autofit/non_linear/grid/grid_list.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/non_linear/grid/grid_search/__init__.py` & `autofit-2024.5.16.0/autofit/non_linear/grid/grid_search/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,15 +213,21 @@
             The result of the grid search
         """
         self.logger.info("...in parallel")
 
         grid_priors = model.sort_priors_alphabetically(set(grid_priors))
         lists = self.make_lists(grid_priors)
 
-        builder = ResultBuilder(lists=lists, grid_priors=grid_priors)
+        jobs = self.make_jobs(model, analysis, grid_priors, info)
+
+        builder = ResultBuilder(
+            lists=lists,
+            grid_priors=grid_priors,
+            paths=[j.search_instance.paths for j in jobs],
+        )
 
         self.save_metadata()
 
         def save_results():
             self.paths.save_json("result", to_dict(builder()))
 
         def write_results():
@@ -248,17 +254,15 @@
                 rows,
                 self.paths.output_path / "results.csv",
             )
 
         results_list = []
 
         for i, job_result in enumerate(
-            process_class.run_jobs(
-                self.make_jobs(model, analysis, grid_priors, info), self.number_of_cores
-            )
+            process_class.run_jobs(jobs, self.number_of_cores)
         ):
             builder.add(job_result)
             results_list.append(job_result.result_list_row)
             write_results()
             if i % self._result_output_interval == 0:
                 save_results()
```

### Comparing `autofit-2024.1.27.4/autofit/non_linear/grid/grid_search/job.py` & `autofit-2024.5.16.0/autofit/non_linear/grid/grid_search/job.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,11 +62,11 @@
             *[
                 prior.lower_limit
                 for prior in self.model.sort_priors_alphabetically(
                     self.arguments.values()
                 )
             ],
             result.log_likelihood,
-            result.samples.log_evidence,
+            result.samples_summary.log_evidence,
         ]
 
         return JobResult(result, result_list_row, self.number)
```

### Comparing `autofit-2024.1.27.4/autofit/non_linear/grid/grid_search/result.py` & `autofit-2024.5.16.0/autofit/non_linear/grid/grid_search/result.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/non_linear/grid/sensitivity/__init__.py` & `autofit-2024.5.16.0/autofit/non_linear/grid/sensitivity/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,17 +139,17 @@
                             *values,
                             result_.log_evidence_increase,
                             result_.log_likelihood_increase,
                         ]
                     )
 
         result = SensitivityResult(
-            samples=[result.result.samples.summary() for result in results],
+            samples=[result.result.samples_summary for result in results],
             perturb_samples=[
-                result.perturb_result.samples.summary() for result in results
+                result.perturb_result.samples_summary for result in results
             ],
             shape=self.shape,
         )
 
         self.paths.save_json("result", to_dict(result))
 
         return result
```

### Comparing `autofit-2024.1.27.4/autofit/non_linear/grid/sensitivity/job.py` & `autofit-2024.5.16.0/autofit/non_linear/grid/sensitivity/job.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/non_linear/grid/sensitivity/result.py` & `autofit-2024.5.16.0/autofit/non_linear/grid/sensitivity/result.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/non_linear/grid/simple_grid.py` & `autofit-2024.5.16.0/autofit/non_linear/grid/simple_grid.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,11 +50,10 @@
                 best_likelihood = likelihood
                 best_instance = instance
 
         return Result(
             samples=MockSamples(
                 max_log_likelihood_instance=best_instance,
                 log_likelihood_list=likelihoods,
-                gaussian_tuples=None
             ),
             model=model
         )
```

### Comparing `autofit-2024.1.27.4/autofit/non_linear/initializer.py` & `autofit-2024.5.16.0/autofit/non_linear/initializer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,56 @@
 import configparser
 import logging
 import os
 import random
 from abc import ABC, abstractmethod
-from typing import Dict, Tuple, List
+from typing import Dict, Tuple, List, Optional
 
 import numpy as np
 
 from autofit import exc
+from autofit.non_linear.paths.abstract import AbstractPaths
 from autofit.mapper.prior.abstract import Prior
 from autofit.mapper.prior_model.abstract import AbstractPriorModel
+from autofit.non_linear.parallel import SneakyPool
 
 logger = logging.getLogger(__name__)
 
 
 class AbstractInitializer(ABC):
     """
     Family of classes used to provide initial points for non-linear search
     """
 
     @abstractmethod
     def _generate_unit_parameter_list(self, model):
         pass
 
+    @staticmethod
+    def figure_of_metric(args) -> Optional[float]:
+        fitness, parameter_list = args
+        try:
+            figure_of_merit = fitness(parameters=parameter_list)
+
+            if np.isnan(figure_of_merit) or figure_of_merit < -1e98:
+                return None
+
+            return figure_of_merit
+        except exc.FitException:
+            return None
+
     def samples_from_model(
         self,
         total_points: int,
         model: AbstractPriorModel,
         fitness,
+        paths: AbstractPaths,
         use_prior_medians: bool = False,
         test_mode_samples: bool = True,
+        n_cores: int = 1,
     ):
         """
         Generate the initial points of the non-linear search, by randomly drawing unit values from a uniform
         distribution between the ball_lower_limit and ball_upper_limit values.
 
         Parameters
         ----------
@@ -44,46 +61,55 @@
             of free dimensions of the model.
         """
 
         if os.environ.get("PYAUTOFIT_TEST_MODE") == "1" and test_mode_samples:
             return self.samples_in_test_mode(total_points=total_points, model=model)
 
         logger.info(
-            "Generating initial samples of model, which are subject to prior limits and other constraints."
+            f"Generating initial samples of model, which are subject to prior limits and other constraints. "
+            f"Using {n_cores} cores."
         )
 
         unit_parameter_lists = []
         parameter_lists = []
         figures_of_merit_list = []
 
-        point_index = 0
-
-        while point_index < total_points:
-            if not use_prior_medians:
-                unit_parameter_list = self._generate_unit_parameter_list(model)
-            else:
-                unit_parameter_list = [0.5] * model.prior_count
-
-            parameter_list = model.vector_from_unit_vector(
-                unit_vector=unit_parameter_list
-            )
+        sneaky_pool = SneakyPool(n_cores, fitness, paths)
 
-            try:
-                figure_of_merit = fitness(parameters=parameter_list)
+        while len(figures_of_merit_list) < total_points:
+            remaining_points = total_points - len(figures_of_merit_list)
+            batch_size = min(remaining_points, n_cores)
+            parameter_lists_ = []
+            unit_parameter_lists_ = []
+
+            for _ in range(batch_size):
+                if not use_prior_medians:
+                    unit_parameter_list = self._generate_unit_parameter_list(model)
+                else:
+                    unit_parameter_list = [0.5] * model.prior_count
 
-                if np.isnan(figure_of_merit) or figure_of_merit < -1e98:
-                    raise exc.FitException
+                parameter_list = model.vector_from_unit_vector(
+                    unit_vector=unit_parameter_list
+                )
 
-                unit_parameter_lists.append(unit_parameter_list)
-                parameter_lists.append(parameter_list)
-                figures_of_merit_list.append(figure_of_merit)
-                point_index += 1
-            except exc.FitException:
-                pass
+                parameter_lists_.append(parameter_list)
+                unit_parameter_lists_.append(unit_parameter_list)
 
+            for figure_of_merit, unit_parameter_list, parameter_list in zip(
+                sneaky_pool.map(
+                    self.figure_of_metric,
+                    [(fitness, parameter_list) for parameter_list in parameter_lists_],
+                ),
+                unit_parameter_lists_,
+                parameter_lists_,
+            ):
+                if figure_of_merit is not None:
+                    unit_parameter_lists.append(unit_parameter_list)
+                    parameter_lists.append(parameter_list)
+                    figures_of_merit_list.append(figure_of_merit)
 
         if total_points > 1 and np.allclose(
             a=figures_of_merit_list[0], b=figures_of_merit_list[1:]
         ):
             raise exc.InitializerException(
                 """
                 The initial samples all have the same figure of merit (e.g. log likelihood values).
@@ -170,14 +196,16 @@
         upper_limit
             A default, unit upper limit used when a prior is not specified
         """
         self.parameter_dict = parameter_dict
         self.lower_limit = lower_limit
         self.upper_limit = upper_limit
 
+        self._generated_warnings = set()
+
     def _generate_unit_parameter_list(self, model: AbstractPriorModel) -> List[float]:
         """
         Generate a unit vector for the model. The default limits are used for any
         priors which the model has but are not found in the parameter dict.
 
         Parameters
         ----------
@@ -191,18 +219,22 @@
 
         unit_parameter_list = []
         for prior in model.priors_ordered_by_id:
             try:
                 lower, upper = map(prior.unit_value_for, self.parameter_dict[prior])
                 value = random.uniform(lower, upper)
             except KeyError:
-                logger.warning(
-                    f"Range for {'.'.join(model.path_for_prior(prior))} not set in the SpecificRangeInitializer. "
-                    f"Using defaults."
-                )
+                key = ".".join(model.path_for_prior(prior))
+                if key not in self._generated_warnings:
+                    logger.warning(
+                        f"Range for {key} not set in the SpecificRangeInitializer. "
+                        f"Using defaults."
+                    )
+                    self._generated_warnings.add(key)
+
                 lower = self.lower_limit
                 upper = self.upper_limit
 
                 value = prior.unit_value_for(prior.random(lower, upper))
 
             unit_parameter_list.append(value)
```

### Comparing `autofit-2024.1.27.4/autofit/non_linear/mock/mock_analysis.py` & `autofit-2024.5.16.0/autofit/non_linear/mock/mock_analysis.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/non_linear/mock/mock_result.py` & `autofit-2024.5.16.0/autofit/non_linear/mock/mock_result.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,68 @@
 from autofit.mapper.model import ModelInstance
 from autofit.mapper.model_mapper import ModelMapper
 from autofit.non_linear.result import Result
 
+from autofit.non_linear.mock.mock_samples_summary import MockSamplesSummary
 from autofit.non_linear.mock.mock_samples import MockSamples
 
 
 class MockResult(Result):
     def __init__(
         self,
+        samples_summary: MockSamplesSummary = None,
+        paths=None,
         samples=None,
         instance=None,
         analysis=None,
         search=None,
         model=None,
     ):
-        super().__init__(samples)
+        super().__init__(
+            samples_summary=samples_summary
+            or MockSamplesSummary(
+                model=model or ModelMapper(),
+            ),
+            paths=paths,
+            samples=samples,
+            search_internal=None,
+        )
 
         self._instance = instance or ModelInstance()
         self._samples = samples or MockSamples(
-            max_log_likelihood_instance=self.instance, model=model or ModelMapper()
+            model=model
+            or ModelMapper()
         )
 
-        self.gaussian_tuples = None
+        self.prior_means = None
         self.analysis = analysis
         self.search = search
         self.model = model
 
-    def model_absolute(self, absolute):
-        return self.model
-
-    def model_relative(self, relative):
-        return self.model
+    def model_absolute(self, a):
+        try:
+            return self.samples_summary.model_absolute(a)
+        except AttributeError:
+            return self.model
+
+    def model_relative(self, r):
+        try:
+            return self.samples_summary.model_relative(r)
+        except AttributeError:
+            return self.model
 
     @property
     def last(self):
         return self
 
 
 class MockResultGrid(Result):
     def __init__(self, log_likelihood):
         # noinspection PyTypeChecker
-        super().__init__(None)
+        super().__init__(None, None)
         self._log_likelihood = log_likelihood
         self.model = log_likelihood
 
     @property
     def log_likelihood(self):
         return self._log_likelihood
```

### Comparing `autofit-2024.1.27.4/autofit/non_linear/mock/mock_search.py` & `autofit-2024.5.16.0/autofit/non_linear/mock/mock_search.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,169 +1,173 @@
-import math
-from typing import Optional, Tuple
-
-from autoconf import conf
-from autofit import exc
-from autofit.mapper.model_mapper import ModelMapper
-from autofit.graphical import FactorApproximation
-from autofit.graphical.utils import Status
-from autofit.non_linear.search.abstract_search import NonLinearSearch
-from autofit.non_linear.mock.mock_result import MockResult
-from autofit.non_linear.mock.mock_samples import MockSamples
-from autofit.non_linear.samples import Sample
-
-
-def samples_with_log_likelihood_list(log_likelihood_list, kwargs):
-    if isinstance(log_likelihood_list, float):
-        log_likelihood_list = [log_likelihood_list]
-    return [
-        Sample(
-            log_likelihood=log_likelihood,
-            log_prior=0,
-            weight=0,
-            kwargs=kwargs,
-        )
-        for log_likelihood in log_likelihood_list
-    ]
-
-
-def _make_samples(model):
-    return {path: prior.value_for(0.5) for path, prior in model.path_priors_tuples}
-
-
-class MockSearch(NonLinearSearch):
-    def __init__(
-        self,
-        name="",
-        samples=None,
-        result=None,
-        unique_tag: Optional[str] = None,
-        fit_fast=True,
-        sample_multiplier=1,
-        save_for_aggregator=False,
-        return_sensitivity_results=False,
-        **kwargs
-    ):
-        super().__init__(name=name, unique_tag=unique_tag, **kwargs)
-
-        self.samples = samples or MockSamples(ModelMapper())
-
-        self.result = MockResult(samples=samples) if result is None else result
-
-        self.fit_fast = fit_fast
-        self.sample_multiplier = sample_multiplier
-
-        self.save_for_aggregator = save_for_aggregator
-        self.return_sensitivity_results = return_sensitivity_results
-
-    def check_model(self, model):
-        pass
-
-    @property
-    def config_type(self):
-        return conf.instance["non_linear"]["mock"]
-
-    @property
-    def config_dict_search(self):
-        return {}
-
-    def _fit_fast(self, model, analysis):
-        class Fitness:
-            def __init__(self, instance_from_vector, result):
-                self.result = result
-                self.instance_from_vector = instance_from_vector
-
-            def __call__(self, vector):
-                instance = self.instance_from_vector(vector)
-
-                log_likelihood = analysis.log_likelihood_function(instance)
-
-                if self.result.instance is None:
-                    self.result.instance = instance
-
-                # Return Chi squared
-                return -2 * log_likelihood
-
-        self.paths.samples_to_csv(self.samples)
-
-        if self.save_for_aggregator:
-            analysis.save_attributes(paths=self.paths)
-
-        fitness = Fitness(model.instance_from_vector, result=self.result)
-        fitness([prior.mean for prior in model.priors_ordered_by_id])
-
-        return fitness.result
-
-    def _fit(self, model, analysis):
-        if self.fit_fast:
-            result = self._fit_fast(model=model, analysis=analysis)
-            return result
-
-        if model.prior_count == 0:
-            raise AssertionError("There are no priors associated with the model!")
-        if model.prior_count != len(model.unique_prior_paths):
-            raise AssertionError(
-                "Prior count doesn't match number of unique prior paths"
-            )
-        index = 0
-        unit_vector = model.prior_count * [0.5]
-        while True:
-            try:
-                instance = model.instance_from_unit_vector(unit_vector)
-                fit = analysis.log_likelihood_function(instance)
-                break
-            except exc.FitException as e:
-                unit_vector[index] += 0.1
-                if unit_vector[index] >= 1:
-                    raise e
-                index = (index + 1) % model.prior_count
-        samples = MockSamples(
-            sample_list=samples_with_log_likelihood_list(
-                self.sample_multiplier * fit, _make_samples(model)
-            ),
-            model=model,
-            gaussian_tuples=[
-                (prior.mean, prior.width if math.isfinite(prior.width) else 1.0)
-                for prior in sorted(model.priors, key=lambda prior: prior.id)
-            ],
-        )
-
-        self.paths.samples_to_csv(self.samples)
-
-        return analysis.make_result(
-            samples=samples,
-        )
-
-    def perform_update(self, model, analysis, during_analysis, search_internal=None):
-        if self.samples is not None and not self.return_sensitivity_results:
-            self.paths.samples_to_csv(self.samples)
-            return self.samples
-
-        return MockSamples(
-            sample_list=samples_with_log_likelihood_list(
-                [1.0, 2.0], _make_samples(model)
-            ),
-            gaussian_tuples=[
-                (prior.mean, prior.width if math.isfinite(prior.width) else 1.0)
-                for prior in sorted(model.priors, key=lambda prior: prior.id)
-            ],
-            model=model,
-        )
-
-    def samples_from(self, model):
-        return self.samples
-
-
-class MockOptimizer(MockSearch):
-    def __init__(self, **kwargs):
-        super().__init__(fit_fast=False, **kwargs)
-
-    @property
-    def samples_cls(self):
-        return MockOptimizer
-
-    def project(
-        self, factor_approx: FactorApproximation, status: Status = Status()
-    ) -> Tuple[FactorApproximation, Status]:
-        pass
-
-    init_args = list()
+from typing import Optional, Tuple
+
+from autoconf import conf
+from autofit import exc
+from autofit.graphical import FactorApproximation
+from autofit.graphical.utils import Status
+from autofit.non_linear.mock.mock_samples import MockSamples
+from autofit.non_linear.search.abstract_search import NonLinearSearch
+from autofit.non_linear.mock.mock_result import MockResult
+from autofit.non_linear.mock.mock_samples_summary import MockSamplesSummary
+from autofit.non_linear.samples import Sample
+
+
+def samples_with_log_likelihood_list(log_likelihood_list, kwargs):
+    if isinstance(log_likelihood_list, float):
+        log_likelihood_list = [log_likelihood_list]
+    return [
+        Sample(
+            log_likelihood=log_likelihood,
+            log_prior=0.0,
+            weight=1.0,
+            kwargs=kwargs,
+        )
+        for log_likelihood in log_likelihood_list
+    ]
+
+
+def _make_samples(model):
+    return {path: prior.value_for(0.5) for path, prior in model.path_priors_tuples}
+
+
+class MockSearch(NonLinearSearch):
+    def __init__(
+        self,
+        name="",
+        samples_summary=None,
+        samples=None,
+        result=None,
+        unique_tag: Optional[str] = None,
+        fit_fast=True,
+        sample_multiplier=1,
+        save_for_aggregator=False,
+        return_sensitivity_results=False,
+        **kwargs
+    ):
+        super().__init__(name=name, unique_tag=unique_tag, **kwargs)
+
+        if samples_summary is None:
+            samples_summary = MockSamplesSummary.default()
+
+        self.samples_summary = samples_summary
+        self.samples = samples
+
+        self.result = (
+            MockResult(
+                samples_summary=samples_summary,
+                model=samples_summary.model,
+            )
+            if result is None
+            else result
+        )
+
+        self.fit_fast = fit_fast
+        self.sample_multiplier = sample_multiplier
+
+        self.save_for_aggregator = save_for_aggregator
+        self.return_sensitivity_results = return_sensitivity_results
+
+    def check_model(self, model):
+        pass
+
+    @property
+    def config_type(self):
+        return conf.instance["non_linear"]["mock"]
+
+    @property
+    def config_dict_search(self):
+        return {}
+
+    def _fit_fast(self, model, analysis):
+        class Fitness:
+            def __init__(self, instance_from_vector, result):
+                self.result = result
+                self.instance_from_vector = instance_from_vector
+
+            def __call__(self, vector):
+                instance = self.instance_from_vector(vector)
+
+                log_likelihood = analysis.log_likelihood_function(instance)
+
+                if self.result.instance is None:
+                    self.result.samples_summary._instance = instance
+
+                # Return Chi squared
+                return -2 * log_likelihood
+
+        self.paths.save_samples_summary(self.samples_summary)
+        self.paths.save_samples(samples=self.samples)
+
+        if self.save_for_aggregator:
+            analysis.save_attributes(paths=self.paths)
+
+        fitness = Fitness(model.instance_from_vector, result=self.result)
+        fitness([prior.mean for prior in model.priors_ordered_by_id])
+
+        return fitness.result
+
+    def _fit(self, model, analysis):
+        if self.fit_fast:
+            return self._fit_fast(model=model, analysis=analysis)
+
+        if model.prior_count == 0:
+            raise AssertionError("There are no priors associated with the model!")
+        if model.prior_count != len(model.unique_prior_paths):
+            raise AssertionError(
+                "Prior count doesn't match number of unique prior paths"
+            )
+        index = 0
+        unit_vector = model.prior_count * [0.5]
+        while True:
+            try:
+                instance = model.instance_from_unit_vector(unit_vector)
+                fit = analysis.log_likelihood_function(instance)
+                break
+            except exc.FitException as e:
+                unit_vector[index] += 0.1
+                if unit_vector[index] >= 1:
+                    raise e
+                index = (index + 1) % model.prior_count
+
+        samples_summary = MockSamplesSummary(
+            model=model,
+            prior_means=[
+                prior.mean for prior in sorted(model.priors, key=lambda prior: prior.id)
+            ],
+        )
+
+        self.paths.save_samples_summary(self.samples_summary)
+
+        return analysis.make_result(
+            samples_summary=samples_summary,
+            paths=self.paths,
+        )
+
+    def perform_update(self, model, analysis, during_analysis, search_internal=None):
+        if self.samples_summary is not None and not self.return_sensitivity_results:
+            self.paths.save_samples_summary(self.samples_summary)
+
+        return MockSamples(
+            sample_list=samples_with_log_likelihood_list(
+                [1.0, 2.0], _make_samples(model)
+            ),
+            prior_means=[
+                prior.mean for prior in sorted(model.priors, key=lambda prior: prior.id)
+            ],
+            model=model,
+        )
+
+
+class MockOptimizer(MockSearch):
+    def __init__(self, **kwargs):
+        super().__init__(fit_fast=False, **kwargs)
+
+    @property
+    def samples_cls(self):
+        return MockOptimizer
+
+    def project(
+        self, factor_approx: FactorApproximation, status: Status = Status()
+    ) -> Tuple[FactorApproximation, Status]:
+        pass
+
+    init_args = list()
```

### Comparing `autofit-2024.1.27.4/autofit/non_linear/parallel/process.py` & `autofit-2024.5.16.0/autofit/non_linear/parallel/process.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/non_linear/parallel/sneaky.py` & `autofit-2024.5.16.0/autofit/non_linear/parallel/sneaky.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,18 @@
 from typing import Iterable, Optional, Callable
 
 from autoconf import conf
 
 from autofit.non_linear.paths.abstract import AbstractPaths
 from .process import AbstractJob, Process, StopCommand
 
-logger = logging.getLogger(
-    __name__
-)
+logger = logging.getLogger(__name__)
 
 
-def _is_likelihood_function(
-        function
-) -> bool:
+def _is_likelihood_function(function) -> bool:
     """
     Is the function a callable used to evaluate likelihood?
 
     Naturally in Autofit this would be a child of the Fitness class.
     In Dynesty the likelihood function is wrapped in _function_wrapper
     and called 'loglikelihood'
 
@@ -33,28 +29,23 @@
     Returns
     -------
     Is the object a log likelihood function?
     """
     from autofit.non_linear.fitness import Fitness
     from dynesty.dynesty import _function_wrapper
     from emcee.ensemble import _FunctionWrapper
-    return any([
-        isinstance(
-            function,
-            Fitness
-        ),
-        isinstance(
-            function,
-            _function_wrapper
-        ) and function.name == 'loglikelihood',
-        isinstance(
-            function,
-            _FunctionWrapper
-        )
-    ])
+
+    return any(
+        [
+            isinstance(function, Fitness),
+            isinstance(function, _function_wrapper)
+            and function.name == "loglikelihood",
+            isinstance(function, _FunctionWrapper),
+        ]
+    )
 
 
 class SneakyJob(AbstractJob):
     def __init__(self, function, *args):
         """
         A job performed on a process.
 
@@ -79,17 +70,15 @@
         else:
             self.function = function
 
         self.args = list()
         self.fitness_index = None
 
         for i, arg in enumerate(args):
-            if _is_likelihood_function(
-                    arg
-            ):
+            if _is_likelihood_function(arg):
                 if self.fitness_index is not None:
                     raise AssertionError(
                         f"Two arguments of type NonLinear.Fitness passed to {function.__name__}"
                     )
                 self.fitness_index = i
             else:
                 self.args.append(arg)
@@ -119,37 +108,33 @@
             to avoid copying data for every single function call
 
         Returns
         -------
         The log likelihood
         """
         if self.function is None:
-            return likelihood_function(
-                self.args
-            )
+            return likelihood_function(self.args)
         if self.is_not_fitness:
             return self.function(self.args)
         args = (
-                self.args[:self.fitness_index]
-                + [likelihood_function]
-                + self.args[self.fitness_index:]
-        )
-        return self.function(
-            args
+            self.args[: self.fitness_index]
+            + [likelihood_function]
+            + self.args[self.fitness_index :]
         )
+        return self.function(args)
 
 
 class SneakyProcess(Process):
     def __init__(
-            self,
-            name: str,
-            paths: AbstractPaths,
-            initializer=None,
-            initargs=None,
-            job_args=tuple()
+        self,
+        name: str,
+        paths: AbstractPaths,
+        initializer=None,
+        initargs=None,
+        job_args=tuple(),
     ):
         """
         Each SneakyProcess creates its own queue to avoid locking during
         highly parallel optimisations.
         """
 
         super().__init__(
@@ -175,57 +160,49 @@
             pr.enable()
 
         self._init()
         self.logger.debug("starting")
         while True:
             job = self.job_queue.get()
             if job is StopCommand:
-                self.logger.debug(
-                    "StopCommand found"
-                )
+                self.logger.debug("StopCommand found")
                 break
             try:
-                self.queue.put(
-                    job.perform(
-                        *self.job_args
-                    )
-                )
+                self.queue.put(job.perform(*self.job_args))
             except Exception as e:
                 self.logger.exception(e)
                 self.queue.put(e)
         self.logger.debug("terminating process {}".format(self.name))
         self.job_queue.close()
 
         if conf.instance["general"]["test"]["parallel_profile"]:
-
             try:
                 os.makedirs(self.paths.profile_path)
             except FileExistsError:
                 pass
 
             sneaky_path = self.paths.profile_path / f"sneaky_{self.pid}.prof"
 
             pr.dump_stats(sneaky_path)
             pr.disable()
 
     def open_profiler(self):
-
         if conf.instance["general"]["test"]["parallel_profile"]:
             pr = cProfile.Profile()
             pr.enable()
 
 
 class SneakyPool:
     def __init__(
-            self,
-            processes: int,
-            fitness,
-            paths: AbstractPaths,
-            initializer=None,
-            initargs=None
+        self,
+        processes: int,
+        fitness,
+        paths: AbstractPaths,
+        initializer=None,
+        initargs=None,
     ):
         """
         Implements the same interface as multiprocessing's pool,
         but associates the fitness object with each process to
         prevent data being copies to each process for every function
         call.
 
@@ -235,24 +212,22 @@
             The number of cores to be used simultaneously.
         fitness
             A class comprising data and a model which can be used
             to evaluate the likelihood of a live point
         initializer
         initargs
         """
-        logger.debug(
-            f"Creating SneakyPool with {processes} processes"
-        )
+        logger.info(f"Creating pool with {processes} processes")
         self._processes = [
             SneakyProcess(
                 str(number),
                 paths=paths,
                 initializer=initializer,
                 initargs=initargs,
-                job_args=(fitness,)
+                job_args=(fitness,),
             )
             for number in range(processes)
         ]
         for process in self.processes:
             process.start()
 
     @property
@@ -274,100 +249,79 @@
 
         Yields
         ------
         Results from the function evaluation
         """
         jobs = [
             SneakyJob(
-                function,
-                *(
-                    (args,) if not isinstance(
-                        args,
-                        Iterable
-                    ) else tuple(args)
-                )
-            ) for args in args_list
+                function, *((args,) if not isinstance(args, Iterable) else tuple(args))
+            )
+            for args in args_list
         ]
 
-        logger.debug(
-            f"Running {len(jobs)} jobs across {self.processes} processes"
-        )
+        logger.info(f"Running {len(jobs)} jobs across {self.processes} processes")
 
         for i, job in enumerate(jobs):
-            process = self.processes[
-                i % len(self.processes)
-                ]
-            process.job_queue.put(
-                job
-            )
+            process = self.processes[i % len(self.processes)]
+            process.job_queue.put(job)
 
         target = len(jobs)
         count = 0
 
         exception = None
 
         while count < target:
             for process in self.processes:
                 if not process.queue.empty():
                     item = process.queue.get()
                     count += 1
-                    if isinstance(
-                            item,
-                            Exception
-                    ):
+                    if isinstance(item, Exception):
                         exception = item
                     else:
                         yield item
 
-        logger.debug(
-            "All jobs complete"
-        )
+        logger.debug("All jobs complete")
 
         if exception is not None:
             raise exception
 
     def __del__(self):
         """
         Called when the map goes out of scope.
 
         Tell each process to terminate with a StopCommand and then join
         each process with a timeout of one second.
         """
-        logger.debug(
-            "Deconstructing SneakyMap"
-        )
+        logger.debug("Deconstructing SneakyMap")
 
-        logger.debug(
-            "Terminating processes..."
-        )
+        logger.debug("Terminating processes...")
         for process in self.processes:
             process.job_queue.put(StopCommand)
 
-        logger.debug(
-            "Joining processes..."
-        )
+        logger.debug("Joining processes...")
         for process in self.processes:
             try:
                 process.join(0.5)
             except Exception as e:
                 logger.exception(e)
 
+
 class FunctionCache:
     """
     Singleton class to cache the functions and optional arguments between calls
     """
 
 
 def initializer(
-        fitness ,
-        prior_transform,
-        fitness_args,
-        fitness_kwargs,
-        prior_transform_args,
-        prior_transform_kwargs
+    fitness,
+    prior_transform,
+    fitness_args,
+    fitness_kwargs,
+    prior_transform_args,
+    prior_transform_kwargs,
 ):
     """
     Initialized function used to initialize the
     singleton object inside each worker of the pool
     """
     FunctionCache.fitness = fitness
     FunctionCache.prior_transform = prior_transform
@@ -377,98 +331,96 @@
     FunctionCache.prior_transform_kwargs = prior_transform_kwargs
 
 
 def fitness_cache(x):
     """
     Likelihood function call
     """
-    return FunctionCache.fitness(x, *FunctionCache.fitness_args,
-                                 **FunctionCache.fitness_kwargs)
+    return FunctionCache.fitness(
+        x, *FunctionCache.fitness_args, **FunctionCache.fitness_kwargs
+    )
 
 
 def prior_transform_cache(x):
     """
     Prior transform call
     """
 
-    return FunctionCache.prior_transform(x, *FunctionCache.prior_transform_args,
-                                         **FunctionCache.prior_transform_kwargs)
-
+    return FunctionCache.prior_transform(
+        x, *FunctionCache.prior_transform_args, **FunctionCache.prior_transform_kwargs
+    )
 
 
 class SneakierPool:
     def __init__(
-            self,
-            processes: int,
-            fitness: Callable,
-            prior_transform: Optional[Callable] = None,
-            fitness_args: Optional[Iterable] = None,
-            fitness_kwargs: Optional[dict] = None,
-            prior_transform_args: Optional[Iterable] = None,
-            prior_transform_kwargs: Optional[dict] = None,
+        self,
+        processes: int,
+        fitness: Callable,
+        prior_transform: Optional[Callable] = None,
+        fitness_args: Optional[Iterable] = None,
+        fitness_kwargs: Optional[dict] = None,
+        prior_transform_args: Optional[Iterable] = None,
+        prior_transform_kwargs: Optional[dict] = None,
     ):
-
         self.fitness_init = fitness
         self.prior_transform_init = prior_transform
         self.fitness = fitness_cache
         self.prior_transform = prior_transform_cache
         self.fitness_args = fitness_args or ()
         self.fitness_kwargs = fitness_kwargs or {}
         self.prior_transform_args = prior_transform_args or ()
         self.prior_transform_kwargs = prior_transform_kwargs or {}
         self.processes = processes
         self.pool = None
         try:
             from mpi4py import MPI
+
             self.comm = MPI.COMM_WORLD
             self._processes = self.comm.size
         except ModuleNotFoundError:
             self._processes = 1
 
         init_args = (
-            self.fitness_init, self.prior_transform_init,
-            self.fitness_args, self.fitness_kwargs,
-            self.prior_transform_args, self.prior_transform_kwargs
+            self.fitness_init,
+            self.prior_transform_init,
+            self.fitness_args,
+            self.fitness_kwargs,
+            self.prior_transform_args,
+            self.prior_transform_kwargs,
         )
         initializer(*init_args)
 
     def check_if_mpi(self):
-
         return self._processes > 1
 
     def is_master(self):
-
         is_mpi = self.check_if_mpi()
         if is_mpi:
             return_value = self.comm.rank == 0
         else:
             return_value = True
-        
+
         return return_value
 
     def wait(self):
-
         is_mpi = self.check_if_mpi()
         if is_mpi:
             self.pool.wait()
         else:
             pass
-            warnings.warn(
-                "Cannot wait for pool to finish if not using MPI"
-            )
+            warnings.warn("Cannot wait for pool to finish if not using MPI")
 
     def __enter__(self):
         """
         Activate the mp / mpi pool
         """
 
         use_mpi = self.check_if_mpi()
 
         if use_mpi:
-
             from schwimmbad import MPIPool
 
             if self.is_master():
                 logger.info("... using Schwimmbad MPIPool")
             self.pool = MPIPool(use_dill=True)
 
         else:
@@ -476,47 +428,48 @@
                 logger.info("... using multiprocessing")
             self.pool = mp.Pool(
                 processes=self.processes,
             )
 
         return self
 
-    def map(
-            self, function: Callable,
-            iterable: Iterable
-    ):
+    def map(self, function: Callable, iterable: Iterable):
         """
         Map a function over an iterable using the map method
         of the initialized pool.
 
         Parameters
         ----------
         function
             A function to map
         iterable
             An iterable to map over
 
         """
         return self.pool.map(function, iterable)
-    
+
     def __exit__(self, exc_type, exc_val, exc_tb):
         try:
             self.pool.terminate()
         except:  # noqa
             pass
         try:
-            del (FunctionCache.fitness, FunctionCache.prior_transform,
-                 FunctionCache.fitness_args, FunctionCache.fitness_kwargs,
-                 FunctionCache.prior_transform_args, FunctionCache.prior_transform_kwargs)
+            del (
+                FunctionCache.fitness,
+                FunctionCache.prior_transform,
+                FunctionCache.fitness_args,
+                FunctionCache.fitness_kwargs,
+                FunctionCache.prior_transform_args,
+                FunctionCache.prior_transform_kwargs,
+            )
         except:  # noqa
             pass
-    
+
     @property
     def size(self):
-
         return self.njobs
-    
+
     def close(self):
         self.pool.close()
-    
+
     def join(self):
-        self.pool.join()
+        self.pool.join()
```

### Comparing `autofit-2024.1.27.4/autofit/non_linear/paths/abstract.py` & `autofit-2024.5.16.0/autofit/non_linear/paths/abstract.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-import dill
-import json
 import logging
 import os
 import re
 import shutil
 import zipfile
 from abc import ABC, abstractmethod
 from configparser import NoSectionError
 from os import path
 from pathlib import Path
-from typing import Dict, Optional
+from typing import Optional
 
 import numpy as np
 
 from autoconf import conf
 from autofit.mapper.identifier import Identifier, IdentifierField
+from autofit.non_linear.samples.summary import SamplesSummary
+
 from autofit.text import text_util
 from autofit.tools.util import open_, zip_directory
 
 logger = logging.getLogger(__name__)
 
 pattern = re.compile(r"(?<!^)(?=[A-Z])")
 
 
 class AbstractPaths(ABC):
     def __init__(
         self,
         name: Optional[str] = None,
-        path_prefix: Optional[str] = None,
+        path_prefix: Optional[os.PathLike] = None,
         is_identifier_in_paths=True,
         parent: Optional["AbstractPaths"] = None,
         unique_tag: Optional[str] = None,
         identifier: str = None,
     ):
         """
         Manages the path structure for `NonLinearSearch` output, for analyses both not using and using the search
@@ -67,29 +67,35 @@
 
         self.name = name or ""
         self.path_prefix = path_prefix or ""
 
         self.unique_tag = unique_tag
 
         self._non_linear_name = None
-        self.__identifier = identifier or None
+        self.__custom_identifier = identifier
+        self.__identifier = None
 
         self.is_identifier_in_paths = is_identifier_in_paths
 
         self._parent = None
         self.parent = parent
 
         try:
             self.remove_files = conf.instance["general"]["output"]["remove_files"]
 
             if conf.instance["general"]["hpc"]["hpc_mode"]:
                 self.remove_files = True
         except NoSectionError as e:
             logger.exception(e)
 
+    @property
+    @abstractmethod
+    def samples(self):
+        pass
+
     def save_parent_identifier(self):
         pass
 
     def save_unique_tag(self, is_grid_search=False):
         pass
 
     def __str__(self):
@@ -157,14 +163,16 @@
                 self._non_linear_name = pattern.sub(
                     "_", type(self.search).__name__
                 ).lower()
         return self._non_linear_name
 
     @property
     def _identifier(self):
+        if self.__custom_identifier is not None:
+            return self.__custom_identifier
         if self.__identifier is None:
             if None in (self.model, self.search):
                 logger.debug(
                     "Generating identifier without both model and search having been set."
                 )
 
             identifier_list = [self.search, self.model]
@@ -235,15 +243,18 @@
 
     @property
     def _files_path(self) -> Path:
         """
         This is private for a reason, use the save_json etc. methods to save and load json
         """
         files_path = self.output_path / "files"
-        os.makedirs(files_path, exist_ok=True)
+        try:
+            os.makedirs(files_path, exist_ok=True)
+        except FileExistsError:
+            pass
         return files_path
 
     def zip_remove(self):
         """
         Copy files from the sym linked search folder then remove the sym linked folder.
         """
 
@@ -319,22 +330,28 @@
         Copy files from the ``.zip`` file to the samples folder.
         """
 
         if path.exists(self._zip_path):
             shutil.rmtree(self.output_path, ignore_errors=True)
 
             try:
-                with zipfile.ZipFile(self._zip_path, "r") as f:
-                    f.extractall(self.output_path)
+                try:
+                    with zipfile.ZipFile(self._zip_path, "r") as f:
+                        f.extractall(self.output_path)
+                except FileExistsError:
+                    pass
             except zipfile.BadZipFile as e:
                 raise zipfile.BadZipFile(
                     f"Unable to restore the zip file at the path {self._zip_path}"
                 ) from e
 
-            os.remove(self._zip_path)
+            try:
+                os.remove(self._zip_path)
+            except FileNotFoundError:
+                pass
 
     def __eq__(self, other):
         return isinstance(other, AbstractPaths) and all(
             [
                 self.path_prefix == other.path_prefix,
                 self.name == other.name,
                 self.non_linear_name == other.non_linear_name,
@@ -387,14 +404,17 @@
 
     def save_search_internal(self, obj):
         raise NotImplementedError
 
     def load_search_internal(self):
         raise NotImplementedError
 
+    def remove_search_internal(self):
+        raise NotImplementedError
+
     @property
     @abstractmethod
     def is_complete(self) -> bool:
         pass
 
     @abstractmethod
     def completed(self):
@@ -412,43 +432,70 @@
 
     @abstractmethod
     def save_samples(self, samples):
         """
         Save samples to the database
         """
 
-    def samples_to_csv(self, samples):
+    def save_samples_summary(self, samples_summary: SamplesSummary):
+        """
+        Save samples summary to the database.
+        """
+
+    def load_samples_summary(self) -> SamplesSummary:
         """
-        Save the final-result samples associated with the phase as a pickle
+        Load samples summary from the database.
+        """
+
+    @abstractmethod
+    def save_latent_samples(self, latent_samples):
+        """
+        Save latent variables. These are values computed from an instance and output
+        during analysis.
         """
 
     @abstractmethod
     def load_samples_info(self):
         pass
 
-    def save_summary(self, samples, log_likelihood_function_time):
+    def save_summary(
+        self,
+        samples,
+        latent_samples,
+        log_likelihood_function_time,
+    ):
         result_info = text_util.result_info_from(
             samples=samples,
         )
-
         filename = self.output_path / "model.results"
-
         with open_(filename, "w") as f:
             f.write(result_info)
 
+        if latent_samples:
+            result_info = text_util.result_info_from(
+                samples=latent_samples,
+            )
+            filename = self.output_path / "latent.results"
+            with open_(filename, "w") as f:
+                f.write(result_info)
+
         text_util.search_summary_to_file(
             samples=samples,
             log_likelihood_function_time=log_likelihood_function_time,
             filename=self.output_path / "search.summary",
         )
 
     @property
     def _samples_file(self) -> Path:
         return self._files_path / "samples.csv"
 
     @property
+    def _latent_variables_file(self) -> Path:
+        return self._files_path / "latent.csv"
+
+    @property
     def _covariance_file(self) -> Path:
         return self._files_path / "covariance.csv"
 
     @property
     def _info_file(self) -> Path:
         return self._files_path / "samples_info.json"
```

### Comparing `autofit-2024.1.27.4/autofit/non_linear/paths/database.py` & `autofit-2024.5.16.0/autofit/non_linear/paths/database.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import shutil
-from typing import Dict, Optional, Union
+from typing import Optional, Union
 
 from autoconf.output import conditional_output
 from autofit.database.sqlalchemy_ import sa
 from .abstract import AbstractPaths
 import numpy as np
 
 from autofit.database.model import Fit
@@ -29,14 +29,16 @@
             parent=parent,
         )
         self.session = session
         self._fit = None
         self.save_all_samples = save_all_samples
         self.unique_tag = unique_tag
 
+    __nullify_fields__ = ("session",)
+
     parent: "DatabasePaths"
 
     @AbstractPaths.parent.setter
     def parent(self, parent: "DatabasePaths"):
         """
         The search performed before this search. For example, a search
         that is then compared to searches during a grid search.
@@ -143,14 +145,18 @@
 
         Returns
         -------
         The loaded dictionary
         """
         return self.fit.get_json(name)
 
+    @property
+    def samples(self):
+        return self.fit.samples
+
     @conditional_output
     def save_array(self, name, array: np.ndarray):
         """
         Save an array as a json file in the database
 
         Parameters
         ----------
@@ -220,14 +226,17 @@
 
     def save_search_internal(self, obj):
         pass
 
     def load_search_internal(self):
         pass
 
+    def remove_search_internal(self):
+        pass
+
     @property
     def fit(self) -> Fit:
         if self._fit is None:
             try:
                 self._fit = (
                     self.session.query(Fit).filter(Fit.id == self.identifier).one()
                 )
@@ -248,30 +257,37 @@
     @property
     def is_complete(self) -> bool:
         return self.fit.is_complete
 
     def completed(self):
         self.fit.is_complete = True
 
-    def save_summary(self, samples, log_likelihood_function_time):
+    def save_summary(
+        self,
+        samples,
+        latent_samples,
+        log_likelihood_function_time,
+    ):
         self.fit.instance = samples.max_log_likelihood()
         self.fit.max_log_likelihood = samples.max_log_likelihood_sample.log_likelihood
 
     def save_samples(self, samples):
         if not self.save_all_samples:
             samples = samples.minimise()
 
         self.fit.samples = samples
         self.fit.set_json("samples_info", samples.samples_info)
 
-    def samples_to_csv(self, samples):
-        """
-        Save the final-result samples associated with the phase as a pickle
-        """
-        pass
+    def save_latent_samples(self, latent_samples):
+        if not self.save_all_samples:
+            latent_samples = latent_samples.minimise()
+        self.fit.latent_samples = latent_samples
+
+    def load_latent_samples(self):
+        return self.fit.latent_samples
 
     def _load_samples(self):
         samples = self.fit.samples
         samples.model = self.model
         return samples
 
     def load_samples(self):
```

### Comparing `autofit-2024.1.27.4/autofit/non_linear/paths/directory.py` & `autofit-2024.5.16.0/autofit/non_linear/paths/directory.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,44 @@
+import shutil
+
 import dill
 import json
 import os
 from os import path
 from pathlib import Path
-from typing import Optional, Union
+from typing import Optional, Union, cast, Type
 import logging
 
 from autoconf import conf
-from autoconf.dictable import to_dict
-from autoconf.output import conditional_output
+from autoconf.class_path import get_class
+from autoconf.dictable import to_dict, from_dict
+from autoconf.output import conditional_output, should_output
 from autofit.text import formatter
 from autofit.tools.util import open_
+from autofit.non_linear.samples.samples import Samples
 
 from .abstract import AbstractPaths
+
 from ..samples import load_from_table
 from autofit.non_linear.samples.pdf import SamplesPDF
+from autofit.non_linear.samples.summary import SamplesSummary
 import numpy as np
 
+from ...visualise import VisualiseGraph
+
 logger = logging.getLogger(__name__)
 
 
 class DirectoryPaths(AbstractPaths):
     def _path_for_pickle(self, name: str, prefix: str = "") -> Path:
         return self._files_path / prefix / f"{name}.pickle"
 
     def _path_for_json(self, name, prefix: str = "") -> Path:
+        if isinstance(name, Path):
+            return name
         return self._files_path / prefix / f"{name}.json"
 
     def _path_for_csv(self, name) -> Path:
         return self._files_path / f"{name}.csv"
 
     def _path_for_fits(self, name, prefix: str = "") -> Path:
         os.makedirs(self._files_path / prefix, exist_ok=True)
@@ -193,57 +203,155 @@
         The results in this representation are required to use a search's in-built tools for visualization,
         analysing samples and other tasks.
 
         Returns
         -------
         The results of the non-linear search in its internal representation.
         """
+
+        # This is a nasty hack to load emcee backends. It will be removed once the source code is more stable.
+
+        import emcee
+
+        backend_filename = self.search_internal_path / "search_internal.hdf"
+        if os.path.isfile(backend_filename):
+            return emcee.backends.HDFBackend(filename=str(backend_filename))
+
         filename = self.search_internal_path / "search_internal.dill"
 
         with open_(filename, "rb") as f:
             return dill.load(f)
 
+    def remove_search_internal(self):
+        """
+        Remove the internal representation of a non-linear search.
+
+        This deletes the entire `search_internal` folder, including a .pickle / .dill file containing the interal
+        results and files with the timer values.
+
+        This folder can often have a large filesize, thus deleting it can reduce hard-disk use of the model-fit.
+        """
+        shutil.rmtree(self.search_internal_path)
+
     def completed(self):
         """
         Mark the search as complete by saving a file
         """
         open_(self._has_completed_path, "w+").close()
 
     def load_samples(self):
         return load_from_table(filename=self._samples_file)
 
+    @property
+    def samples(self):
+        """
+        Load the samples associated with the search from the output directory.
+        """
+        sample_list = self.load_samples()
+        samples_info = self.load_samples_info()
+
+        cls = cast(Type[Samples], get_class(samples_info["class_path"]))
+
+        return cls.from_list_info_and_model(
+            sample_list=sample_list,
+            samples_info=samples_info,
+            model=self.model,
+        )
+
+    def save_latent_samples(
+        self,
+        latent_samples,
+    ):
+        """
+        Write out the latent variables of the model to a file.
+
+        Parameters
+        ----------
+        latent_samples
+            Samples describing the latent variables of the model
+        """
+        self._save_samples(latent_samples, name="latent")
+
     def save_samples(self, samples):
-        pass
+        """
+        Save the final-result samples associated with the phase as a pickle
+        """
+        self._save_samples(samples)
 
-    def samples_to_csv(self, samples):
+    def _save_samples(self, samples, name=None):
         """
         Save the final-result samples associated with the phase as a pickle
         """
-        if conf.instance["general"]["output"]["samples_to_csv"]:
-            samples.write_table(filename=self._samples_file)
-            self.save_json("samples_info", samples.samples_info)
+
+        if name is not None:
+            directory = self._files_path / name
+        else:
+            directory = self._files_path
+            name = "samples"
+        if conf.instance["general"]["output"]["samples_to_csv"] and should_output(name):
+            self.save_json(directory / "samples_info.json", samples.samples_info)
+
             if isinstance(samples, SamplesPDF):
                 try:
-                    samples.save_covariance_matrix(self._covariance_file)
-                except ValueError as e:
+                    samples.save_covariance_matrix(directory / "covariance.csv")
+                except (ValueError, ZeroDivisionError) as e:
                     logger.warning(
                         f"Could not save covariance matrix because of the following error:\n{e}"
                     )
 
+            samples.write_table(filename=directory / "samples.csv")
+
+    def save_samples_summary(self, samples_summary: SamplesSummary):
+        model = samples_summary.model
+
+        filter_args = tuple(
+            name
+            for name in (
+                "errors_at_sigma_1",
+                "errors_at_sigma_3",
+                "values_at_sigma_1",
+                "values_at_sigma_3",
+                "max_log_likelihood_sample",
+                "median_pdf_sample",
+            )
+            if not should_output(name)
+        )
+
+        samples_summary.model = None
+        self.save_json(
+            "samples_summary",
+            to_dict(
+                samples_summary,
+                filter_args=filter_args,
+            ),
+        )
+        samples_summary.model = model
+
+    def load_samples_summary(self) -> SamplesSummary:
+        samples_summary = from_dict(self.load_json(name="samples_summary"))
+        samples_summary.model = self.model
+
+        return samples_summary
+
+    def load_latent_samples(self):
+        return load_from_table(filename=self._files_path / "latent/samples.csv")
+
     def load_samples_info(self):
         with open_(self._info_file) as infile:
             return json.load(infile)
 
     def save_all(self, search_config_dict=None, info=None):
         info = info or {}
 
         self.save_identifier()
         self.save_parent_identifier()
         self._save_model_info(model=self.model)
-        self._save_parameter_names_file(model=self.model)
+        VisualiseGraph(
+            model=self.model,
+        ).save(str(self.output_path / "model_graph.html"))
         if info:
             self.save_json("info", info)
         self.save_json("search", to_dict(self.search))
         self.save_json("model", to_dict(self.model))
         self._save_metadata(search_name=type(self.search).__name__.lower())
 
     @AbstractPaths.parent.setter
```

### Comparing `autofit-2024.1.27.4/autofit/non_linear/paths/null.py` & `autofit-2024.5.16.0/autofit/non_linear/paths/null.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,21 @@
 
 
 class NullPaths(AbstractPaths):
     """
     Null version of paths object for avoiding writing of files to disk
     """
 
+    @property
+    def samples(self):
+        return None
+
+    def save_latent_samples(self, latent_samples):
+        pass
+
     def save_json(self, name, object_dict: dict, prefix: str = ""):
         pass
 
     def load_json(self, name, prefix: str = "") -> dict:
         pass
 
     def save_array(self, name, array):
@@ -28,15 +35,15 @@
         pass
 
     def __init__(self):
         super().__init__()
         self.objects = dict()
         self._samples_path = tempfile.mkdtemp()
 
-    def save_summary(self, samples, log_likelihood_function_time):
+    def save_summary(self, samples, latent_samples, log_likelihood_function_time):
         pass
 
     @property
     def samples_path(self) -> str:
         return self._samples_path
 
     @AbstractPaths.parent.setter
@@ -80,14 +87,17 @@
 
     def save_search_internal(self, obj):
         pass
 
     def load_search_internal(self):
         pass
 
+    def remove_search_internal(self):
+        pass
+
     @property
     def search_internal_path(self):
         pass
 
     def load_samples(self):
         pass
```

### Comparing `autofit-2024.1.27.4/autofit/non_linear/paths/sub_directory_paths.py` & `autofit-2024.5.16.0/autofit/non_linear/paths/sub_directory_paths.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/non_linear/result.py` & `autofit-2024.5.16.0/autofit/non_linear/result.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,22 @@
+from __future__ import annotations
 import logging
 from abc import ABC, abstractmethod
 import numpy as np
+from typing import TYPE_CHECKING, Optional
+import warnings
 
-from autoconf import conf
+if TYPE_CHECKING:
+    from autofit.non_linear.analysis.analysis import Analysis
 
 from autofit import exc
 from autofit.mapper.prior_model.abstract import AbstractPriorModel
+from autofit.non_linear.paths.abstract import AbstractPaths
 from autofit.non_linear.samples import Samples
+from autofit.non_linear.samples.summary import SamplesSummary
 from autofit.text import text_util
 
 
 class Placeholder:
     def __getattr__(self, item):
         """
         Placeholders return None to represent the missing result's value
@@ -38,17 +44,36 @@
         return -np.inf
 
     def summary(self):
         return self
 
 
 class AbstractResult(ABC):
+    """
+    @DynamicAttrs
+    """
+
+    def __init__(self, samples_summary, paths):
+        """
+        Abstract result of a non-linear search.
+
+        Parameters
+        ----------
+        samples_summary
+            A summary of the most important samples of the non-linear search (e.g. maximum log likelihood, median PDF).
+        paths
+            The paths to the results of the search.
+        """
+
+        self._samples_summary = samples_summary
+        self.paths = paths
+
     @property
-    def sigma(self):
-        return self.samples.sigma
+    def samples_summary(self):
+        return self._samples_summary
 
     @property
     @abstractmethod
     def samples(self):
         pass
 
     @property
@@ -80,20 +105,20 @@
         """
         if isinstance(other, Placeholder):
             return False
         return self.log_likelihood < other.log_likelihood
 
     @property
     def log_likelihood(self):
-        return max(self.samples.log_likelihood_list)
+        return self.samples_summary.max_log_likelihood_sample.log_likelihood
 
     @property
     def instance(self):
         try:
-            return self.samples.instance
+            return self.samples_summary.instance
         except AttributeError as e:
             logging.warning(e)
             return None
 
     @property
     def max_log_likelihood_instance(self):
         return self.instance
@@ -114,15 +139,15 @@
             The absolute width of gaussian priors
 
         Returns
         -------
         A model mapper created by taking results from this search and creating priors with the defined absolute
         width.
         """
-        return self.samples.model_absolute(a)
+        return self.samples_summary.model_absolute(a)
 
     def model_relative(self, r: float) -> AbstractPriorModel:
         """
         Returns a model where every free parameter is a `GaussianPrior` with `mean` the previous result's
         inferred maximum log likelihood parameter values and `sigma` a relative value from the result `r`.
 
         For example, a previous result may infer a parameter to have a maximum log likelihood value of 2 and
@@ -137,15 +162,15 @@
             The relative width of gaussian priors
 
         Returns
         -------
         A model mapper created by taking results from this search and creating priors with the defined relative
         width.
         """
-        return self.samples.model_relative(r)
+        return self.samples_summary.model_relative(r)
 
     def model_bounded(self, b: float) -> AbstractPriorModel:
         """
         Returns a model where every free parameter is a `UniformPrior` with `lower_limit` and `upper_limit the previous
         result's inferred maximum log likelihood parameter values minus and plus the bound `b`.
 
         For example, a previous result may infer a parameter to have a maximum log likelihood value of 2.
@@ -159,51 +184,139 @@
             The size of the bounds of the uniform prior
 
         Returns
         -------
         A model mapper created by taking results from this search and creating priors with the defined bounded
         uniform priors.
         """
-        return self.samples.model_bounded(b)
+        return self.samples_summary.model_bounded(b)
+
 
 class Result(AbstractResult):
-    def __init__(self, samples: Samples):
-        """
-        The result of a non-linear search, which includes:
+    def __init__(
+        self,
+        samples_summary: SamplesSummary,
+        paths: Optional[AbstractPaths] = None,
+        samples: Optional[Samples] = None,
+        search_internal: Optional[object] = None,
+        analysis: Optional[Analysis] = None,
+    ):
+        """
+        The result of a non-linear search.
+
+        The default behaviour is for all key results to be in the `samples_summary` attribute, which is a concise
+        summary of the results of the non-linear search. The reasons for this to be the main attribute are:
+
+        - It is concise and therefore has minimal I/O overhead, which is important because when runs are resumed
+        the results are loaded often, which can become very slow for large results via a `samples.csv`.
+
+        - The `output.yaml` config files can be used to disable the output of the `samples.csv` file
+        and `search_internal.dill` files. This means in order for results to be loaded in a way that allows a run to
+        resume, the `samples_summary` must contain all results necessary to resume the run.
+
+        For this reason, the `samples` and `search_internal` attributes are optional. On the first run of a model-fit,
+        they will always contain values as they are passed in via memory from the results of the search. However, if
+        a run is resumed they are no longer available in memory, and they will only be available if their corresponding
+        `samples.csv` and `search_internal.dill` files are output on disk and available to load.
+
+        This object includes:
+
+        - The `samples_summary` attribute, which is a summary of the results of the non-linear search.
+
+        - The `paths` attribute, which contains the path structure to the results of the search on the hard-disk and
+        is used to load the samples and search internal attributes if they are required and not available in memory.
 
         - The samples of the non-linear search (E.g. MCMC chains, nested sampling samples) which are used to compute
         the maximum likelihood model, posteriors and other properties.
 
-        - The model used to fit the data, which uses the samples to create specific instances of the model (e.g.
-        an instance of the maximum log likelihood model).
-
-        - The non-linear search used to perform the model fit.
+        - The non-linear search used to perform the model fit in its internal format (e.g. the Dynesty sampler used
+        by dynesty itself as opposed to PyAutoFit abstract classes).
 
         Parameters
         ----------
+        samples_summary
+            A summary of the most important samples of the non-linear search (e.g. maximum log likelihood, median PDF).
+        paths
+            The paths to the results of the search, used to load the samples and search internal attributes if they are
+            required and not available in memory.
         samples
-            The samples of the non-linear search
+            The samples of the non-linear search, for example the MCMC chains.
+        search_internal
+            The non-linear search used to perform the model fit in its internal format.
+        analysis
+            The `Analysis` object that was used to perform the model-fit from which this result is inferred.
         """
+        super().__init__(samples_summary=samples_summary, paths=paths)
+
         self._samples = samples
+        self._search_internal = search_internal
+
+        self.analysis = analysis
 
         self.__model = None
 
         self.child_results = None
 
     def dict(self) -> dict:
         """
         Human-readable dictionary representation of the results
         """
         return {
-            "max_log_likelihood": self.samples.max_log_likelihood_sample.model_dict(),
+            "max_log_likelihood": self.samples_summary.max_log_likelihood_sample.model_dict(),
+            "median pdf": self.samples_summary.median_pdf_sample.model_dict(),
         }
 
     @property
-    def samples(self):
-        return self._samples
+    def samples(self) -> Optional[Samples]:
+        """
+        Returns the samples of the non-linear search, for example the MCMC chains or nested sampling samples.
+
+        When a model-fit is run the first time, the samples are passed into the result via memory and therefore
+        always available.
+
+        However, if a model-fit is resumed the samples are not available in memory and they only way to load them is
+        via the `samples.csv` file output on the hard-disk. This property handles the loading of the samples from
+        the `samples.csv` file if they are not available in memory.
+
+        Returns
+        -------
+        The samples of the non-linear search.
+        """
+
+        if self._samples is not None:
+            return self._samples
+
+        try:
+            return self.paths.samples
+        except FileNotFoundError:
+            return None
+
+    @property
+    def search_internal(self):
+        """
+        Returns the non-linear search used to perform the model fit in its internal sampler format.
+
+        When a model-fit is run the first time, the search internal is passed into the result via memory and therefore
+        always available.
+
+        However, if a model-fit is resumed the search internal is not available in memory and they only way to load
+        it is via the `search_internal.dill` file output on the hard-disk. This property handles the loading of
+        the search internal from the `search_internal.dill` file if it is not available in memory.
+
+        Returns
+        -------
+        The non-linear search used to perform the model fit in its internal sampler format.
+        """
+        if self._search_internal is not None:
+            return self._search_internal
+
+        try:
+            return self.paths.load_search_internal()
+        except FileNotFoundError:
+            pass
 
     @property
     def projected_model(self) -> AbstractPriorModel:
         """
         Create a new model with the same structure as the previous model,
         replacing each prior with a new prior created by calculating sufficient
         statistics from samples and corresponding weights for that prior.
@@ -216,22 +329,19 @@
             )
             for path, prior in self.samples.model.path_priors_tuples
         }
         return self.samples.model.mapper_from_prior_arguments(arguments)
 
     @property
     def model(self):
-        use_errors = conf.instance["general"]["prior_passer"]["use_errors"]
-        use_widths = conf.instance["general"]["prior_passer"]["use_widths"]
-
         if self.__model is None:
-            tuples = self.samples.gaussian_priors_at_sigma(sigma=self.sigma)
-            self.__model = self.samples.model.mapper_from_gaussian_tuples(
-                tuples, use_errors=use_errors, use_widths=use_widths
+            self.__model = self.samples_summary.model.mapper_from_prior_means(
+                means=self.samples_summary.prior_means
             )
+
         return self.__model
 
     @model.setter
     def model(self, model):
         self.__model = model
 
     def __str__(self):
```

### Comparing `autofit-2024.1.27.4/autofit/non_linear/samples/efficient.py` & `autofit-2024.5.16.0/autofit/non_linear/samples/efficient.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,14 @@
-from typing import List
+from typing import List, cast, Type
 
 import numpy as np
+
+from autoconf.class_path import get_class
 from .sample import Sample
+from .samples import Samples
 from .pdf import SamplesPDF
 
 
 class EfficientSamples:
     def __init__(self, samples: SamplesPDF):
         """
         A representation of samples where values are stored in numpy arrays. This is more
@@ -14,36 +17,38 @@
         Parameters
         ----------
         samples
             A representation of samples where values are in instances of the Sample class.
         """
         self.model = samples.model
         self.samples_info = samples.samples_info
-        self.search_internal = samples.search_internal
 
         sample_list = samples.sample_list
-        self._keys = list(sample_list[0].kwargs.keys())
+        try:
+            self._keys = list(sample_list[0].kwargs.keys())
+        except IndexError:
+            self._keys = []
         self._values = np.asarray(
             [[sample.kwargs[key] for key in self._keys] for sample in sample_list]
         )
         self._log_likelihoods = np.asarray(
             [sample.log_likelihood for sample in sample_list]
         )
         self._log_priors = np.asarray([sample.log_prior for sample in sample_list])
         self._weights = np.asarray([sample.weight for sample in sample_list])
 
     @property
-    def samples(self) -> SamplesPDF:
+    def samples(self) -> Samples:
         """
         Convert the efficient samples back to a SamplesPDF instance.
         """
-        return SamplesPDF(
+        cls = cast(Type[Samples], get_class(self.samples_info["class_path"]))
+        return cls(
             model=self.model,
             samples_info=self.samples_info,
-            search_internal=self.search_internal,
             sample_list=self.sample_list,
         )
 
     @property
     def sample_list(self) -> List[Sample]:
         """
         Convert the efficient samples back to a list of Sample instances.
```

### Comparing `autofit-2024.1.27.4/autofit/non_linear/samples/interface.py` & `autofit-2024.5.16.0/autofit/non_linear/samples/interface.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,38 @@
 from abc import ABC, abstractmethod
 from functools import wraps
 from typing import Union, List, Tuple
 
-from autofit import conf
 from autofit.mapper.model import ModelInstance
 from autofit.mapper.prior_model.abstract import AbstractPriorModel
 from autofit.mapper.prior_model.abstract import Path
 
 
 def to_instance(func):
+    """
+    Decorator for methods that return a vector of parameters, which can be converted to a model instance.
+
+    Parameters
+    ----------
+    func
+        A method that returns a vector of parameters
+
+    Returns
+    -------
+    A wrapper that converts the vector to a model instance
+    """
+
     @wraps(func)
     def wrapper(
-        obj, as_instance: bool = True, *args, **kwargs
+        self, *args, as_instance: bool = True, **kwargs
     ) -> Union[List, ModelInstance]:
-        vector = func(obj, as_instance, *args, **kwargs)
+        vector = func(self, *args, **kwargs)
 
         if as_instance:
-            return obj.model.instance_from_vector(
-                vector=vector, ignore_prior_limits=True
-            )
+            return self._instance_from_vector(vector)
 
         return vector
 
     return wrapper
 
 
 class SamplesInterface(ABC):
@@ -109,17 +119,15 @@
             The absolute width of gaussian priors
 
         Returns
         -------
         A model mapper created by taking results from this search and creating priors with the defined absolute
         width.
         """
-        return self.model.mapper_from_gaussian_tuples(
-            self.gaussian_priors_at_sigma(sigma=self.sigma), a=a
-        )
+        return self.model.mapper_from_prior_means(means=self.prior_means, a=a)
 
     def model_relative(self, r: float) -> AbstractPriorModel:
         """
         Returns a model where every free parameter is a `GaussianPrior` with `mean` the previous result's
         inferred maximum log likelihood parameter values and `sigma` a relative value from the result `r`.
 
         For example, a previous result may infer a parameter to have a maximum log likelihood value of 2 and
@@ -134,17 +142,15 @@
             The relative width of gaussian priors
 
         Returns
         -------
         A model mapper created by taking results from this search and creating priors with the defined relative
         width.
         """
-        return self.model.mapper_from_gaussian_tuples(
-            self.gaussian_priors_at_sigma(sigma=self.sigma), r=r
-        )
+        return self.model.mapper_from_prior_means(means=self.prior_means, r=r)
 
     def model_bounded(self, b: float) -> AbstractPriorModel:
         """
         Returns a model where every free parameter is a `UniformPrior` with `lower_limit` and `upper_limit the previous
         result's inferred maximum log likelihood parameter values minus and plus the bound `b`.
 
         For example, a previous result may infer a parameter to have a maximum log likelihood value of 2.
@@ -162,32 +168,31 @@
         A model mapper created by taking results from this search and creating priors with the defined bounded
         uniform priors.
         """
         return self.model.mapper_from_uniform_floats(
             floats=self.max_log_likelihood(as_instance=False), b=b
         )
 
-    @property
-    def sigma(self):
-        return conf.instance["general"]["prior_passer"]["sigma"]
+    def _instance_from_vector(self, vector: List[float]) -> ModelInstance:
+        return self.model.instance_from_vector(vector=vector, ignore_prior_limits=True)
 
-    def gaussian_priors_at_sigma(self, sigma: float) -> [List]:
+    @property
+    def prior_means(self) -> [List]:
         """
-        Returns `GaussianPrior`'s of every parameter in a fit for use with non-linear search chaining.
-
-        `GaussianPrior`s of every parameter used to link its inferred values and errors to priors used to sample the
+        The mean of every parameter used to link its inferred values and errors to priors used to sample the
         same (or similar) parameters in a subsequent search, where:
 
-        - The mean is given by maximum log likelihood model values.
-        - Their errors are omitted, as this information is not available from an search. When these priors are
-          used to link to another search, it will thus automatically use the prior config values.
-
-        Parameters
-        ----------
-        sigma
-            The sigma limit within which the PDF is used to estimate errors (e.g. sigma = 1.0 uses 0.6826 of the PDF).
+        - The mean is given by their most-probable values median PDF values if using a sampler that provides this
+          information(using median_pdf(as_instance=False)).
+        - The man is given by the maximum log likelihood values otherwise (e.g. for a maximum likelihood estimator).
         """
-        return list(
-            map(
-                lambda vector: (vector, 0.0), self.max_log_likelihood(as_instance=False)
-            )
-        )
+
+        try:
+            return self.median_pdf(as_instance=False)
+        except (AttributeError, IndexError):
+            return self.max_log_likelihood(as_instance=False)
+
+    def path_map_for_model(self, model):
+        return {
+            tuple(self.model.all_paths_for_prior(prior)): path
+            for path, prior in model.path_priors_tuples
+        }
```

### Comparing `autofit-2024.1.27.4/autofit/non_linear/samples/mcmc.py` & `autofit-2024.5.16.0/autofit/non_linear/samples/mcmc.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,76 +5,60 @@
 
 from autofit.mapper.prior_model.abstract import AbstractPriorModel
 from autofit.non_linear.search.mcmc.auto_correlations import AutoCorrelations
 from autofit.non_linear.search.mcmc.auto_correlations import AutoCorrelationsSettings
 from autofit.non_linear.samples.pdf import SamplesPDF
 from autofit.non_linear.samples.samples import Sample
 
-from autofit.non_linear.samples.samples import to_instance, to_instance_sigma
+from autofit.non_linear.samples.samples import to_instance
 
 from autofit import exc
 
-class SamplesMCMC(SamplesPDF):
 
+class SamplesMCMC(SamplesPDF):
     def __init__(
-            self,
-            model: AbstractPriorModel,
-            sample_list: List[Sample],
-            samples_info : Optional[Dict] = None,
-            search_internal: Optional = None,
-            auto_correlation_settings: Optional[AutoCorrelationsSettings] = None,
-            auto_correlations : Optional[AutoCorrelations] = None
+        self,
+        model: AbstractPriorModel,
+        sample_list: List[Sample],
+        samples_info: Optional[Dict] = None,
+        auto_correlation_settings: Optional[AutoCorrelationsSettings] = None,
+        auto_correlations: Optional[AutoCorrelations] = None,
     ):
         """
-        The `Samples` classes in **PyAutoFit** provide an interface between the search_internal of
-        a `NonLinearSearch` (e.g. as files on your hard-disk) and Python.
+        Contains the samples of the non-linear search, including parameter values, log likelihoods,
+        weights and other quantites.
 
         For example, the output class can be used to load an instance of the best-fit model, get an instance of any
         individual sample by the `NonLinearSearch` and return information on the likelihoods, errors, etc.
 
-        This class stores the samples of a MCMC model-fit (e.g. `emcee`, `zeus`). To use a library's in-built
-        visualization tools search_internal are optionally stored in their native internal format using
-        the `search_internal` attribute.
-
         Attributes
         ----------
-        search_internal
-            The MCMC results in their native internal format from which the samples are computed.
         model
             Maps input vectors of unit parameter values to physical values and model instances via priors.
         auto_correlation_settings
             Customizes and performs auto correlation calculations performed during and after the search.
         time
             The time taken to perform the model-fit, which is passed around `Samples` objects for outputting
             information on the overall fit.
-        search_internal
-            The MCMC library's results in their native internal format for interfacing its visualization library.
         """
 
         self.auto_correlations = auto_correlations
         self.auto_correlation_settings = auto_correlation_settings
 
         super().__init__(
             model=model,
             sample_list=sample_list,
             samples_info=samples_info,
-            search_internal=search_internal
         )
 
-    def __add__(
-            self,
-            other: "SamplesMCMC"
-    ) -> "SamplesMCMC":
+    def __add__(self, other: "SamplesMCMC") -> "SamplesMCMC":
         """
         Samples can be added together, which combines their `sample_list` meaning that inferred parameters are
         computed via their joint PDF.
 
-        For Zeus samples there are no tools for combining results in their native format, therefore these
-        `search_internal` are set to None and support for visualization is disabled.
-
         Parameters
         ----------
         other
             Another Samples class
 
         Returns
         -------
@@ -82,34 +66,59 @@
         """
 
         self._check_addition(other=other)
 
         warnings.warn(
             f"Addition of {self.__class__.__name__} cannot retain results in native format. "
             "Visualization of summed samples diabled.",
-            exc.SamplesWarning
+            exc.SamplesWarning,
         )
 
         return self.__class__(
             model=self.model,
             sample_list=self.sample_list + other.sample_list,
             samples_info=self.samples_info,
             auto_correlation_settings=self.auto_correlation_settings,
-            search_internal=None
+        )
+
+    @classmethod
+    def from_list_info_and_model(
+        cls,
+        sample_list,
+        samples_info,
+        model: AbstractPriorModel,
+    ):
+        try:
+            auto_correlation_settings = AutoCorrelationsSettings(
+                check_for_convergence=True,
+                check_size=samples_info["check_size"],
+                required_length=samples_info["required_length"],
+                change_threshold=samples_info["change_threshold"],
+            )
+        except (KeyError, NameError):
+            auto_correlation_settings = None
+
+        return cls(
+            model=model,
+            sample_list=sample_list,
+            samples_info=samples_info,
+            auto_correlation_settings=auto_correlation_settings,
         )
 
     @property
     def pdf_converged(self):
         """
-        To analyse and visualize samples using corner.py, the analysis must be sufficiently converged to produce
-        smooth enough PDF for analysis. This property checks whether the non-linear search's samples are sufficiently
-        converged for corner.py use.
+        To analyse and visualize samples, the analysis must be sufficiently converged to produce smooth enough PDF
+        for analysis.
+
+        This property checks whether the non-linear search's samples are sufficiently converged for analysis and
+        visualization.
 
-        Emcee samples can be analysed by corner.py irrespective of how long the sampler has run, albeit low run times
-        will likely produce inaccurate results.
+        Emcee samples can be analysed irrespective of how long the sampler has run, albeit low run times will likely
+        produce inaccurate results.
         """
         try:
             if len(self.parameter_lists) == 0:
                 return False
             return True
         except ValueError:
             return False
@@ -137,16 +146,16 @@
             return [
                 float(np.percentile(self.parameters_extract[i, :], [50]))
                 for i in range(self.model.prior_count)
             ]
 
         return self.max_log_likelihood(as_instance=False)
 
-    @to_instance_sigma
-    def values_at_sigma(self, sigma: float, as_instance: bool = True) -> [float]:
+    @to_instance
+    def values_at_sigma(self, sigma: float) -> [float]:
         """
         The value of every parameter marginalized in 1D at an input sigma value of its probability density function
         (PDF), returned as two lists of values corresponding to the lower and upper values parameter values.
 
         For example, if sigma is 1.0, the marginalized values of every parameter at 31.7% and 68.2% percentiles of each
         PDF is returned.
 
@@ -171,18 +180,18 @@
                 tuple(
                     np.percentile(samples[i, :], [100.0 * (1.0 - limit), 100.0 * limit])
                 )
                 for i in range(self.model.prior_count)
             ]
 
         parameters_min = list(
-            np.min(self.parameter_lists[-self.unconverged_sample_size:], axis=0)
+            np.min(self.parameter_lists[-self.unconverged_sample_size :], axis=0)
         )
         parameters_max = list(
-            np.max(self.parameter_lists[-self.unconverged_sample_size:], axis=0)
+            np.max(self.parameter_lists[-self.unconverged_sample_size :], axis=0)
         )
 
         return [
             (parameters_min[index], parameters_max[index])
             for index in range(len(parameters_min))
         ]
 
@@ -192,8 +201,8 @@
 
     @property
     def total_walkers(self) -> int:
         return self.samples_info["total_walkers"]
 
     @property
     def log_evidence(self):
-        return None
+        return None
```

### Comparing `autofit-2024.1.27.4/autofit/non_linear/samples/nest.py` & `autofit-2024.5.16.0/autofit/non_linear/samples/nest.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,67 +5,53 @@
 from autofit.mapper.prior_model.abstract import AbstractPriorModel
 from autofit.non_linear.samples.pdf import SamplesPDF
 from autofit.non_linear.samples.samples import Sample
 from autofit.non_linear.samples.stored import SamplesStored
 
 from autofit import exc
 
-class SamplesNest(SamplesPDF):
 
+class SamplesNest(SamplesPDF):
     def __init__(
-            self,
-            model: AbstractPriorModel,
-            sample_list: List[Sample],
-            samples_info : Optional[Dict] = None,
-            search_internal: Optional = None,
+        self,
+        model: AbstractPriorModel,
+        sample_list: List[Sample],
+        samples_info: Optional[Dict] = None,
     ):
         """
-        The `Samples` classes in **PyAutoFit** provide an interface between the search_internal of
-        a `NonLinearSearch` (e.g. as files on your hard-disk) and Python.
+        Contains the samples of the non-linear search, including parameter values, log likelihoods,
+        weights and other quantites.
 
         For example, the output class can be used to load an instance of the best-fit model, get an instance of any
         individual sample by the `NonLinearSearch` and return information on the likelihoods, errors, etc.
 
-        This class stores the samples of nested sampler model-fit (e.g. `dynesty`, `UltraNest`). To use a library's
-        in-built visualization tools results are optionally stored in their native internal format using the
-        `search_internal` attribute.
-
         Parameters
         ----------
         model
             Maps input vectors of unit parameter values to physical values and model instances via priors.
         sample_list
             The list of `Samples` which contains the paramoeters, likelihood, weights, etc. of every sample taken
             by the non-linear search.
         number_live_points
             The number of live points used by the nested sampler.
         samples_info
             Contains information on the samples (e.g. total iterations, time to run the search, etc.).
-        search_internal
-            The nested sampler's results in their native internal format for interfacing its visualization library.
         """
 
         super().__init__(
             model=model,
             sample_list=sample_list,
             samples_info=samples_info,
-            search_internal=search_internal
         )
 
-    def __add__(
-            self,
-            other: "SamplesNest"
-    ) -> "SamplesNest":
+    def __add__(self, other: "SamplesNest") -> "SamplesNest":
         """
         Samples can be added together, which combines their `sample_list` meaning that inferred parameters are
         computed via their joint PDF.
 
-        For UltraNest samples there are no tools for combining results in their native format, therefore these
-        `search_internal` are set to None and support for visualization is disabled.
-
         Parameters
         ----------
         other
             Another Samples class
 
         Returns
         -------
@@ -73,22 +59,21 @@
         """
 
         self._check_addition(other=other)
 
         warnings.warn(
             f"Addition of {self.__class__.__name__} cannot retain results in native format. "
             "Visualization of summed samples diabled.",
-            exc.SamplesWarning
+            exc.SamplesWarning,
         )
 
         return self.__class__(
             model=self.model,
             sample_list=self.sample_list + other.sample_list,
             samples_info=self.samples_info,
-            search_internal=None
         )
 
     @property
     def number_live_points(self):
         return self.samples_info["number_live_points"]
 
     @property
@@ -100,27 +85,25 @@
         return self.samples_info["total_samples"]
 
     @property
     def total_accepted_samples(self) -> int:
         """
         The total number of accepted samples performed by the nested sampler.
         """
-        return len(self.log_likelihood_list)
+        return self.samples_info["total_accepted_samples"]
 
     @property
     def acceptance_ratio(self) -> float:
         """
         The ratio of accepted samples to total samples.
         """
         return self.total_accepted_samples / self.total_samples
 
     def samples_within_parameter_range(
-            self,
-            parameter_index: int,
-            parameter_range: [float, float]
+        self, parameter_index: int, parameter_range: [float, float]
     ) -> "SamplesStored":
         """
         Returns a new set of Samples where all points without parameter values inside a specified range removed.
 
         For example, if our `Samples` object was for a model with 4 parameters are consistent of the following 3 sets
         of parameters:
 
@@ -143,31 +126,30 @@
 
         parameter_list = []
         log_likelihood_list = []
         log_prior_list = []
         weight_list = []
 
         for sample in self.sample_list:
-
             parameters = sample.parameter_lists_for_model(model=self.model)
 
             if (parameters[parameter_index] > parameter_range[0]) and (
-                    parameters[parameter_index] < parameter_range[1]):
-
+                parameters[parameter_index] < parameter_range[1]
+            ):
                 parameter_list.append(parameters)
                 log_likelihood_list.append(sample.log_likelihood)
                 log_prior_list.append(sample.log_prior)
                 weight_list.append(sample.weight)
 
         sample_list = Sample.from_lists(
             model=self.model,
             parameter_lists=parameter_list,
             log_likelihood_list=log_likelihood_list,
             log_prior_list=log_prior_list,
-            weight_list=weight_list
+            weight_list=weight_list,
         )
 
         return SamplesStored(
             model=self.model,
             sample_list=sample_list,
             samples_info=self.samples_info,
         )
```

### Comparing `autofit-2024.1.27.4/autofit/non_linear/samples/pdf.py` & `autofit-2024.5.16.0/autofit/non_linear/samples/pdf.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,82 +1,79 @@
 import logging
 import math
+import pathlib
+import warnings
 from typing import Dict, List, Optional, Tuple, Union
 
 import numpy as np
 
 from autoconf import conf
+from autoconf.output import should_output
 from autofit.mapper.model import ModelInstance
-from autofit.mapper.prior_model.abstract import AbstractPriorModel, Path
+from autofit.mapper.prior_model.abstract import AbstractPriorModel
 from autofit.non_linear.samples.sample import Sample, load_from_table
-from autofit.non_linear.samples.samples import (
-    to_instance,
-    to_instance_sigma,
-    to_instance_input,
-)
+from autofit.non_linear.samples.samples import to_instance
 from .samples import Samples
 from .summary import SamplesSummary
 
 
 class SamplesPDF(Samples):
     def __init__(
         self,
         model: AbstractPriorModel,
         sample_list: List[Sample],
         samples_info: Optional[Dict] = None,
-        search_internal: Optional = None,
     ):
         """
-        The `Samples` classes in **PyAutoFit** provide an interface between the search_internal of
-        a `NonLinearSearch` (e.g. as files on your hard-disk) and Python.
+        Contains the samples of the non-linear search, including parameter values, log likelihoods,
+        weights and other quantites.
 
         For example, the output class can be used to load an instance of the best-fit model, get an instance of any
         individual sample by the `NonLinearSearch` and return information on the likelihoods, errors, etc.
 
         This class stores samples of searches which provide the probability distribution function (PDF) of the
         model fit (e.g. nested samplers, MCMC).
 
-        To use a library's in-built visualization tools results are optionally stored in their native internal format
-        using the `search_internal` attribute.
-
         Parameters
         ----------
         model
             Maps input vectors of unit parameter values to physical values and model instances via priors.
         sample_list
             The list of `Samples` which contains the paramoeters, likelihood, weights, etc. of every sample taken
             by the non-linear search.
         samples_info
             Contains information on the samples (e.g. total iterations, time to run the search, etc.).
-        search_internal
-            The nested sampler's results in their native internal format for interfacing its visualization library.
         """
 
         super().__init__(
-            model=model,
-            sample_list=sample_list,
-            samples_info=samples_info,
-            search_internal=search_internal,
+            model=model, sample_list=sample_list, samples_info=samples_info
         )
 
     def summary(self):
-        try:
-            covariance_matrix = self.covariance_matrix
-        except Exception as e:
-            logging.warning(f"Could not create covariance matrix: {e}")
-            covariance_matrix = None
+        median_pdf_sample = Sample.from_lists(
+            model=self.model,
+            parameter_lists=[self.median_pdf(as_instance=False)],
+            log_likelihood_list=[self.max_log_likelihood_sample.log_likelihood],
+            log_prior_list=[self.max_log_likelihood_sample.log_prior],
+            weight_list=[self.max_log_likelihood_sample.weight],
+        )[0]
+
         return SamplesSummary(
-            max_log_likelihood_sample=self.max_log_likelihood_sample,
             model=self.model,
-            covariance_matrix=covariance_matrix,
+            max_log_likelihood_sample=self.max_log_likelihood_sample,
+            median_pdf_sample=median_pdf_sample,
             log_evidence=self.log_evidence,
+            errors_at_sigma_1=self.errors_at_sigma(sigma=1.0, as_instance=False),
+            errors_at_sigma_3=self.errors_at_sigma(sigma=3.0, as_instance=False),
+            values_at_sigma_1=self.values_at_sigma(sigma=1.0, as_instance=False),
+            values_at_sigma_3=self.values_at_sigma(sigma=3.0, as_instance=False),
         )
 
     @classmethod
-    def from_table(cls, filename: str, model, number_live_points=None):
+    def from_table(cls, filename: str, model):
         """
         Write a table of parameters, posteriors, priors and likelihoods
 
         Parameters
         ----------
         filename
             Where the table is to be written
@@ -86,16 +83,15 @@
         sample_list = load_from_table(filename=filename)
 
         return SamplesStored(model=model, sample_list=sample_list)
 
     @property
     def unconverged_sample_size(self):
         """
-        If a set of samples are unconverged, alternative methods to compute their means, errors, etc are used as
-        an alternative to corner.py.
+        If a set of samples are unconverged, alternative methods to compute their means, errors, etc are used.
 
         These use a subset of samples spanning the range from the most recent sample to the valaue of the
         unconverted_sample_size. However, if there are fewer samples than this size, we change the size to be the
         the size of the total number of samples.
         """
 
         unconverged_sample_size = conf.instance["general"]["output"][
@@ -120,42 +116,40 @@
         can be performed numerically.
         """
         if np.max(self.weight_list) > 0.99:
             return False
         return True
 
     @to_instance
-    def median_pdf(self, as_instance: bool = True) -> List[float]:
+    def median_pdf(self) -> List[float]:
         """
         The median of the probability density function (PDF) of every parameter marginalized in 1D, returned
         as a model instance or list of values.
         """
         if self.pdf_converged:
             return [
                 quantile(x=params, q=0.5, weights=self.weight_list)[0]
                 for params in self.parameters_extract
             ]
         return self.max_log_likelihood(as_instance=False)
 
-    @to_instance_sigma
-    def values_at_sigma(
-        self, sigma: float, as_instance: bool = True
-    ) -> [Tuple, ModelInstance]:
+    @to_instance
+    def values_at_sigma(self, sigma: float) -> [Tuple, ModelInstance]:
         """
         The value of every parameter marginalized in 1D at an input sigma value of its probability density function
         (PDF), returned as two lists of values corresponding to the lower and upper values parameter values.
 
         For example, if sigma is 1.0, the marginalized values of every parameter at 31.7% and 68.2% percentiles of each
         PDF is returned.
 
         This does not account for covariance between parameters. For example, if two parameters (x, y) are degenerate
         whereby x decreases as y gets larger to give the same PDF, this function will still return both at their
         upper values. Thus, caution is advised when using the function to reperform a model-fits.
 
-        For Dynesty, this is estimated using corner.py if the samples have converged, by sampling the density
+        This is estimated using the `quantile` function if the samples have converged, by sampling the density
         function at an input PDF %. If not converged, a crude estimate using the range of values of the current
         physical live points is used.
 
         Parameters
         ----------
         sigma
             The sigma within which the PDF is used to estimate errors (e.g. sigma = 1.0 uses 0.6826 of the PDF).
@@ -172,29 +166,27 @@
                 quantile(x=params, q=1 - low_limit, weights=self.weight_list)[0]
                 for params in self.parameters_extract
             ]
 
             return [(lower, upper) for lower, upper in zip(lower_errors, upper_errors)]
 
         parameters_min = list(
-            np.min(self.parameter_lists[-self.unconverged_sample_size :], axis=0)
+            np.min(self.parameter_lists[-int(self.unconverged_sample_size) :], axis=0)
         )
         parameters_max = list(
-            np.max(self.parameter_lists[-self.unconverged_sample_size :], axis=0)
+            np.max(self.parameter_lists[-int(self.unconverged_sample_size) :], axis=0)
         )
 
         return [
             (parameters_min[index], parameters_max[index])
             for index in range(len(parameters_min))
         ]
 
-    @to_instance_sigma
-    def values_at_upper_sigma(
-        self, sigma: float, as_instance: bool = True
-    ) -> Union[List, ModelInstance]:
+    @to_instance
+    def values_at_upper_sigma(self, sigma: float) -> Union[List, ModelInstance]:
         """
         The upper value of every parameter marginalized in 1D at an input sigma value of its probability density
         function (PDF), returned as a list.
 
         See values_at_sigma for a full description of how the parameters at sigma are computed.
 
         Parameters
@@ -202,18 +194,16 @@
         sigma
             The sigma within which the PDF is used to estimate errors (e.g. sigma = 1.0 uses 0.6826 of the PDF).
         """
         return list(
             map(lambda param: param[1], self.values_at_sigma(sigma, as_instance=False))
         )
 
-    @to_instance_sigma
-    def values_at_lower_sigma(
-        self, sigma: float, as_instance: bool = True
-    ) -> Union[List, ModelInstance]:
+    @to_instance
+    def values_at_lower_sigma(self, sigma: float) -> Union[List, ModelInstance]:
         """
         The lower value of every parameter marginalized in 1D at an input sigma value of its probability density
         function (PDF), returned as a list.
 
         See values_at_sigma for a full description of how the parameters at sigma are computed.
 
         Parameters
@@ -221,15 +211,15 @@
         sigma
             The sigma limit within which the PDF is used to estimate errors (e.g. sigma = 1.0 uses 0.6826 of the PDF).
         """
         return list(
             map(lambda param: param[0], self.values_at_sigma(sigma, as_instance=False))
         )
 
-    @to_instance_sigma
+    @to_instance
     def errors_at_sigma(
         self, sigma: float, as_instance: bool = True
     ) -> [Tuple, ModelInstance]:
         """
         The lower and upper error of every parameter marginalized in 1D at an input sigma value of its probability
         density function (PDF), returned as a list.
 
@@ -243,15 +233,15 @@
         error_vector_lower = self.errors_at_lower_sigma(sigma=sigma, as_instance=False)
         error_vector_upper = self.errors_at_upper_sigma(sigma=sigma, as_instance=False)
         return [
             (lower, upper)
             for lower, upper in zip(error_vector_lower, error_vector_upper)
         ]
 
-    @to_instance_sigma
+    @to_instance
     def errors_at_upper_sigma(
         self, sigma: float, as_instance: bool = True
     ) -> Union[List, ModelInstance]:
         """
         The upper error of every parameter marginalized in 1D at an input sigma value of its probability density
         function (PDF), returned as a list.
 
@@ -267,18 +257,16 @@
             map(
                 lambda upper, median_pdf: upper - median_pdf,
                 uppers,
                 self.median_pdf(as_instance=False),
             )
         )
 
-    @to_instance_sigma
-    def errors_at_lower_sigma(
-        self, sigma: float, as_instance: bool = True
-    ) -> Union[List, ModelInstance]:
+    @to_instance
+    def errors_at_lower_sigma(self, sigma: float) -> Union[List, ModelInstance]:
         """
         The lower error of every parameter marginalized in 1D at an input sigma value of its probability density
         function (PDF), returned as a list.
 
         See values_at_sigma for a full description of how the parameters at sigma are computed.
 
         Parameters
@@ -291,18 +279,16 @@
             map(
                 lambda lower, median_pdf: median_pdf - lower,
                 lowers,
                 self.median_pdf(as_instance=False),
             )
         )
 
-    @to_instance_sigma
-    def error_magnitudes_at_sigma(
-        self, sigma: float, as_instance: bool = True
-    ) -> Union[List, ModelInstance]:
+    @to_instance
+    def error_magnitudes_at_sigma(self, sigma: float) -> Union[List, ModelInstance]:
         """
         The magnitude of every error after marginalization in 1D at an input sigma value of the probability density
         function (PDF), returned as two lists of values corresponding to the lower and upper errors.
 
         For example, if sigma is 1.0, the difference in the inferred values marginalized at 31.7% and 68.2% percentiles
         of each PDF is returned.
 
@@ -311,66 +297,33 @@
         sigma
             The sigma within which the PDF is used to estimate errors (e.g. sigma = 1.0 uses 0.6826 of the PDF).
         """
         uppers = self.values_at_upper_sigma(sigma=sigma, as_instance=False)
         lowers = self.values_at_lower_sigma(sigma=sigma, as_instance=False)
         return list(map(lambda upper, lower: upper - lower, uppers, lowers))
 
-    def gaussian_priors_at_sigma(self, sigma: float) -> [List]:
-        """
-        `GaussianPrior`s of every parameter used to link its inferred values and errors to priors used to sample the
-        same (or similar) parameters in a subsequent search, where:
-
-        - The mean is given by their most-probable values (using median_pdf(as_instance=False)).
-        - Their errors are computed at an input sigma value (using errors_at_sigma).
-
-        Parameters
-        ----------
-        sigma
-            The sigma within which the PDF is used to estimate errors (e.g. sigma = 1.0 uses 0.6826 of the PDF).
-        """
-
-        means = self.median_pdf(as_instance=False)
-
-        uppers = self.values_at_upper_sigma(sigma=sigma, as_instance=False)
-        lowers = self.values_at_lower_sigma(sigma=sigma, as_instance=False)
-
-        # noinspection PyArgumentList
-        sigmas = list(
-            map(
-                lambda mean, upper, lower: max([upper - mean, mean - lower]),
-                means,
-                uppers,
-                lowers,
-            )
-        )
-
-        return list(map(lambda mean, sigma: (mean, sigma), means, sigmas))
-
     @to_instance
-    def draw_randomly_via_pdf(
-        self, as_instance: bool = True
-    ) -> Union[List, ModelInstance]:
+    def draw_randomly_via_pdf(self) -> Union[List, ModelInstance]:
         """
         The parameter vector of an individual sample of the non-linear search drawn randomly from the PDF, returned as
         a 1D list.
 
         The draw is weighted by the sample weights to ensure that the sample is drawn from the PDF (which is important
         for non-linear searches like nested sampling).
         """
 
         sample_index = np.random.choice(
             a=range(len(self.sample_list)), p=self.weight_list
         )
 
         return self.parameter_lists[sample_index][:]
 
-    @to_instance_input
+    @to_instance
     def offset_values_via_input_values(
-        self, input_vector: List, as_instance: bool = True
+        self, input_vector: List
     ) -> Union[List, ModelInstance]:
         """
         The values of an input_vector offset by the median_pdf(as_instance=False) (the PDF medians).
 
         If the 'true' values of a model are known and input as the input_vector, this function returns the results
         of the `NonLinearSearch` as values offset from the 'true' model. For example, a value 0.0 means the non-linear
         search estimated the model parameter value correctly.
@@ -395,33 +348,44 @@
         Compute the covariance matrix of the non-linear search samples, using the method `np.cov()` which is described
         at the following link:
 
         https://numpy.org/doc/stable/reference/generated/numpy.cov.html
 
         Follow that link for a description of what the covariance matrix is.
 
+        This function may be called during a non-linear search, before the samples contain high likelihood regions
+        that enable a robust covariance matrix to be computed. To reduce command line noise, the warning associated
+        with this behaviour is suppressed.
+
         Returns
         -------
         ndarray
             A covariance matrix of shape [total_parameters, total_parameters] for the model parameters of the
             non-linear search.
         """
         if len(self.parameter_lists) == 1:
             return np.eye(1)
-        return np.cov(m=self.parameter_lists, rowvar=False, aweights=self.weight_list)
 
-    def save_covariance_matrix(self, filename: Union[Path, str]):
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+            return np.cov(
+                m=self.parameter_lists, rowvar=False, aweights=self.weight_list
+            )
+
+    def save_covariance_matrix(self, filename: Union[pathlib.Path, str]):
         """
         Save the covariance matrix as a CSV file.
 
         Parameters
         ----------
         filename
             The filename the covariance matrix is saved to.
         """
+        if not should_output("covariance"):
+            return
         # noinspection PyTypeChecker
         np.savetxt(filename, self.covariance_matrix, delimiter=",")
 
     @property
     def log_evidence(self):
         return None
```

### Comparing `autofit-2024.1.27.4/autofit/non_linear/samples/sample.py` & `autofit-2024.5.16.0/autofit/non_linear/samples/sample.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,19 @@
 from autoconf.class_path import get_class_path
 from autofit.mapper.prior_model.abstract import AbstractPriorModel
 from autofit.tools.util import split_paths
 
 
 class Sample:
     def __init__(
-        self, log_likelihood: float, log_prior: float, weight: float, kwargs=None
+        self,
+        log_likelihood: float,
+        log_prior: float,
+        weight: float,
+        kwargs=None,
     ):
         """
         One sample taken during a search
 
         Parameters
         ----------
         log_likelihood
```

### Comparing `autofit-2024.1.27.4/autofit/non_linear/samples/samples.py` & `autofit-2024.5.16.0/autofit/non_linear/samples/samples.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,311 +1,110 @@
 from abc import ABC
-import csv
-from functools import wraps
+
 import json
-import warnings
 from copy import copy
+import logging
+import os
 from typing import Dict, List, Optional, Tuple, Union
 
 import numpy as np
+from pathlib import Path
 
+from autoconf import conf
+from autoconf.class_path import get_class_path
 from autofit import exc
-from autofit.non_linear.search.mcmc.auto_correlations import AutoCorrelationsSettings
 from autofit.mapper.model import ModelInstance
 from autofit.mapper.prior_model.abstract import AbstractPriorModel
 from autofit.non_linear.samples.sample import Sample
 
 from .summary import SamplesSummary
 from .interface import SamplesInterface, to_instance
 from ...text.formatter import write_table
 
-
-### TODO: Rich how do I reduce this to one wrapper sensible?
-
-
-def to_instance_sigma(func):
-    """
-
-    Parameters
-    ----------
-    func
-
-    Returns
-    -------
-        A function that returns a 2D image.
-    """
-
-    @wraps(func)
-    def wrapper(
-        obj, sigma, as_instance: bool = True, *args, **kwargs
-    ) -> Union[List, ModelInstance]:
-        """
-        This decorator checks if a light profile is a `LightProfileOperated` class and therefore already has had operations like a
-        PSF convolution performed.
-
-        This is compared to the `only_operated` input to determine if the image of that light profile is returned, or
-        an array of zeros.
-
-        Parameters
-        ----------
-        obj
-            A light profile with an `image_2d_from` function whose class is inspected to determine if the image is
-            operated on.
-        grid
-            A grid_like object of (y,x) coordinates on which the function values are evaluated.
-        operated_only
-            By default this is None and the image is returned irrespecive of light profile class (E.g. it does not matter
-            if it is already operated or not). If this input is included as a bool, the light profile image is only
-            returned if they are or are not already operated.
-
-        Returns
-        -------
-            The 2D image, which is customized depending on whether it has been operated on.
-        """
-
-        vector = func(obj, sigma, as_instance, *args, **kwargs)
-
-        if as_instance:
-            return obj.model.instance_from_vector(
-                vector=vector, ignore_prior_limits=True
-            )
-
-        return vector
-
-    return wrapper
-
-
-def to_instance_samples(func):
-    """
-
-    Parameters
-    ----------
-    func
-
-    Returns
-    -------
-        A function that returns a 2D image.
-    """
-
-    @wraps(func)
-    def wrapper(
-        obj, sample_index, as_instance: bool = True, *args, **kwargs
-    ) -> Union[List, ModelInstance]:
-        """
-        This decorator checks if a light profile is a `LightProfileOperated` class and therefore already has had operations like a
-        PSF convolution performed.
-
-        This is compared to the `only_operated` input to determine if the image of that light profile is returned, or
-        an array of zeros.
-
-        Parameters
-        ----------
-        obj
-            A light profile with an `image_2d_from` function whose class is inspected to determine if the image is
-            operated on.
-        grid
-            A grid_like object of (y,x) coordinates on which the function values are evaluated.
-        operated_only
-            By default this is None and the image is returned irrespecive of light profile class (E.g. it does not matter
-            if it is already operated or not). If this input is included as a bool, the light profile image is only
-            returned if they are or are not already operated.
-
-        Returns
-        -------
-            The 2D image, which is customized depending on whether it has been operated on.
-        """
-
-        vector = func(obj, sample_index, as_instance, *args, **kwargs)
-
-        if as_instance:
-            return obj.model.instance_from_vector(
-                vector=vector, ignore_prior_limits=True
-            )
-
-        return vector
-
-    return wrapper
-
-
-def to_instance_input(func):
-    """
-
-    Parameters
-    ----------
-    func
-
-    Returns
-    -------
-        A function that returns a 2D image.
-    """
-
-    @wraps(func)
-    def wrapper(
-        obj, input_vector, as_instance: bool = True, *args, **kwargs
-    ) -> Union[List, ModelInstance]:
-        """
-        This decorator checks if a light profile is a `LightProfileOperated` class and therefore already has had operations like a
-        PSF convolution performed.
-
-        This is compared to the `only_operated` input to determine if the image of that light profile is returned, or
-        an array of zeros.
-
-        Parameters
-        ----------
-        obj
-            A light profile with an `image_2d_from` function whose class is inspected to determine if the image is
-            operated on.
-        grid
-            A grid_like object of (y,x) coordinates on which the function values are evaluated.
-        operated_only
-            By default this is None and the image is returned irrespecive of light profile class (E.g. it does not matter
-            if it is already operated or not). If this input is included as a bool, the light profile image is only
-            returned if they are or are not already operated.
-
-        Returns
-        -------
-            The 2D image, which is customized depending on whether it has been operated on.
-        """
-
-        vector = func(obj, input_vector, as_instance, *args, **kwargs)
-
-        if as_instance:
-            return obj.model.instance_from_vector(
-                vector=vector, ignore_prior_limits=True
-            )
-
-        return vector
-
-    return wrapper
+logger = logging.getLogger(__name__)
 
 
 class Samples(SamplesInterface, ABC):
     def __init__(
         self,
         model: AbstractPriorModel,
         sample_list: List[Sample],
         samples_info: Optional[Dict] = None,
-        search_internal: Optional = None,
     ):
         """
-        The `Samples` classes in **PyAutoFit** provide an interface between the search_internal of
-        a `NonLinearSearch` (e.g. as files on your hard-disk) and Python.
+        Contains the samples of the non-linear search, including parameter values, log likelihoods,
+        weights and other quantites.
 
         For example, the output class can be used to load an instance of the best-fit model, get an instance of any
         individual sample by the `NonLinearSearch` and return information on the likelihoods, errors, etc.
 
         This class stores samples of searches which provide maximum likelihood estimates of the  model-fit (e.g.
         PySwarms, LBFGS).
 
-        To use a library's in-built visualization tools results are optionally stored in their native internal format
-        using the `search_internal` attribute.
-
         Parameters
         ----------
         model
             Maps input vectors of unit parameter values to physical values and model instances via priors.
         sample_list
             The list of `Samples` which contains the paramoeters, likelihood, weights, etc. of every sample taken
             by the non-linear search.
         samples_info
             Contains information on the samples (e.g. total iterations, time to run the search, etc.).
-        search_internal
-            The nested sampler's results in their native internal format for interfacing its visualization library.
         """
 
         super().__init__(model=model)
 
         self.sample_list = sample_list
-        self.samples_info = samples_info
-        self.search_internal = search_internal
-
-    @property
-    def log_evidence(self):
-        return None
-
-    @classmethod
-    def from_csv(cls, paths, model: AbstractPriorModel):
-        """
-        Returns a `Samples` object from the output paths of a non-linear search.
-
-        This function loads the sample values (e.g. parameters, log likelihoods) from a .csv file, which is a
-        standardized output for all **PyAutoFit** non-linear searches.
+        self.samples_info = {
+            **(samples_info or {}),
+            "class_path": get_class_path(self.__class__),
+        }
 
-        The samples object requires additional information on the non-linear search (e.g. the number of live points),
-        which is loaded from the `samples_info.json` file.
+    def __str__(self):
+        return f"{self.__class__.__name__}({len(self.sample_list)})"
 
-        This function also looks for the internal results of the non-linear search and includes them in the samples if
-        they exists, which allows for the search's internal visualization and analysis tools to be used.
+    def __repr__(self):
+        return str(self)
 
-        Parameters
-        ----------
-        paths
-            An object describing the paths for saving data (e.g. hard-disk directories or entries in sqlite database).
-        model
-            An object that represents possible instances of some model with a given dimensionality which is the number
-            of free dimensions of the model.
-
-        Returns
-        -------
-        The samples which have been loaded from hard-disk via .csv.
+    @property
+    def instances(self):
         """
+        One model instance for each sample
+        """
+        return [
+            self.model.instance_from_vector(
+                sample.parameter_lists_for_paths(
+                    self.paths if sample.is_path_kwargs else self.names
+                ),
+                ignore_prior_limits=True,
+            )
+            for sample in self.sample_list
+        ]
 
-        sample_list = paths.load_samples()
-        samples_info = paths.load_samples_info()
-
-        try:
-            search_internal = paths.load_search_internal()
-        except FileNotFoundError:
-            search_internal = None
-
-        return cls.from_list_info_and_model(
-            sample_list=sample_list,
-            samples_info=samples_info,
-            model=model,
-            search_internal=search_internal,
-        )
+    @property
+    def log_evidence(self):
+        return None
 
     @classmethod
     def from_list_info_and_model(
         cls,
         sample_list,
         samples_info,
         model: AbstractPriorModel,
-        search_internal=None,
     ):
-        try:
-            auto_correlation_settings = AutoCorrelationsSettings(
-                check_for_convergence=True,
-                check_size=samples_info["check_size"],
-                required_length=samples_info["required_length"],
-                change_threshold=samples_info["change_threshold"],
-            )
-        except (KeyError, NameError):
-            auto_correlation_settings = None
-
-        try:
-            return cls(
-                model=model,
-                sample_list=sample_list,
-                samples_info=samples_info,
-                search_internal=search_internal,
-                auto_correlation_settings=auto_correlation_settings,
-            )
-        except TypeError:
-            return cls(
-                model=model,
-                sample_list=sample_list,
-                samples_info=samples_info,
-                search_internal=search_internal,
-            )
+        return cls(
+            model=model,
+            sample_list=sample_list,
+            samples_info=samples_info,
+        )
 
     def summary(self):
         return SamplesSummary(
-            max_log_likelihood_sample=self.max_log_likelihood_sample,
             model=self.model,
+            max_log_likelihood_sample=self.max_log_likelihood_sample,
         )
 
     def __add__(self, other: "Samples") -> "Samples":
         """
         Samples can be added together, which combines their `sample_list` meaning that inferred parameters are
         computed via their joint PDF.
 
@@ -317,21 +116,14 @@
         Returns
         -------
         A class that combined the samples of the two Samples objects.
         """
 
         self._check_addition(other=other)
 
-        if self.search_internal is not None:
-            warnings.warn(
-                f"Addition of {self.__class__.__name__} cannot retain results in native format. "
-                "Visualization of summed samples diabled.",
-                exc.SamplesWarning,
-            )
-
         return self.__class__(
             model=self.model,
             sample_list=self.sample_list + other.sample_list,
         )
 
     def __radd__(self, other):
         """
@@ -476,15 +268,15 @@
             yield row + [
                 log_likelihood_list[index],
                 log_prior_list[index],
                 log_posterior_list[index],
                 weight_list[index],
             ]
 
-    def write_table(self, filename: str):
+    def write_table(self, filename: Union[str, Path]):
         """
         Write a table of parameters, posteriors, priors and likelihoods.
 
         Parameters
         ----------
         filename
             Where the table is to be written
@@ -509,16 +301,23 @@
             if (
                 most_likely_sample is None
                 or sample.log_likelihood > most_likely_sample.log_likelihood
             ):
                 most_likely_sample = sample
         return most_likely_sample
 
+    @property
+    def max_log_likelihood_index(self) -> int:
+        """
+        The index of the sample with the highest log likelihood.
+        """
+        return int(np.argmax(self.log_likelihood_list))
+
     @to_instance
-    def max_log_likelihood(self, as_instance: bool = True) -> List[float]:
+    def max_log_likelihood(self) -> List[float]:
         """
         The parameters of the maximum log likelihood sample of the `NonLinearSearch` returned as a model instance or
         list of values.
         """
 
         sample = self.max_log_likelihood_sample
 
@@ -534,34 +333,79 @@
     def max_log_posterior_index(self) -> int:
         """
         The index of the sample with the highest log posterior.
         """
         return int(np.argmax(self.log_posterior_list))
 
     @to_instance
-    def max_log_posterior(self, as_instance: bool = True) -> ModelInstance:
+    def max_log_posterior(self) -> ModelInstance:
         """
         The parameters of the maximum log posterior sample of the `NonLinearSearch` returned as a model instance.
         """
         return self.parameter_lists[self.max_log_posterior_index]
 
-    @to_instance_samples
-    def from_sample_index(
-        self, sample_index: int, as_instance: bool = True
-    ) -> ModelInstance:
+    @to_instance
+    def from_sample_index(self, sample_index: int) -> ModelInstance:
         """
         The parameters of an individual sample of the non-linear search, returned as a model instance.
 
         Parameters
         ----------
         sample_index
             The sample index of the weighted sample to return.
         """
         return self.parameter_lists[sample_index]
 
+    def samples_above_weight_threshold_from(
+        self, weight_threshold: Optional[float] = None, log_message: bool = False
+    ) -> "Samples":
+        """
+        Returns a new `Samples` object containing only the samples with a weight above the input threshold.
+
+        This function can be used after a non-linear search is complete, to reduce the samples to only the high weight
+        values. The benefit of this is that the corresponding `samples.csv` file will be reduced in hard-disk size.
+
+        For large libraries of results can significantly reduce the overall hard-disk space used and speed up the
+        time taken to load the samples from a .csv file and perform analysis on them.
+
+        For a sufficiently low threshold, this has a neglible impact on the numerical accuracy of the results, and
+        even higher values can be used for aggresive use cases where hard-disk space is at a premium.
+
+        Parameters
+        ----------
+        weight_threshold
+            The threshold of weight at which a sample is included in the new `Samples` object.
+        """
+
+        if weight_threshold is None:
+            weight_threshold = conf.instance["output"]["samples_weight_threshold"]
+
+        if os.environ.get("PYAUTOFIT_TEST_MODE") == "1":
+            weight_threshold = None
+
+        if weight_threshold is None:
+            return self
+
+        sample_list = []
+
+        for sample in self.sample_list:
+            if sample.weight > weight_threshold:
+                sample_list.append(sample)
+
+        if log_message:
+            logger.info(
+                f"Samples with weight less than {weight_threshold} removed from samples.csv."
+            )
+
+        return self.__class__(
+            model=self.model,
+            sample_list=sample_list,
+            samples_info=self.samples_info,
+        )
+
     def minimise(self) -> "Samples":
         """
         A copy of this object with only important samples retained
         """
         samples = copy(self)
         samples.model = None
         samples.sample_list = list(
@@ -619,18 +463,15 @@
         ]
         return with_paths
 
     def subsamples(self, model):
         if self.model is None:
             return None
 
-        path_map = {
-            tuple(self.model.all_paths_for_prior(prior)): path
-            for path, prior in model.path_priors_tuples
-        }
+        path_map = self.path_map_for_model(model)
         copied = copy(self)
         copied._paths = None
         copied._names = None
         copied.model = model
 
         copied.sample_list = [sample.subsample(path_map) for sample in self.sample_list]
         return copied
```

### Comparing `autofit-2024.1.27.4/autofit/non_linear/samples/stored.py` & `autofit-2024.5.16.0/autofit/non_linear/samples/stored.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/non_linear/search/abstract_search.py` & `autofit-2024.5.16.0/autofit/non_linear/search/abstract_search.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,27 @@
+from __future__ import annotations
 import copy
 import logging
 import multiprocessing as mp
 import os
 import time
 import warnings
 from abc import ABC, abstractmethod
 from collections import Counter
 from functools import wraps
 from pathlib import Path
-from typing import Optional, Union, Tuple, List, Dict
+from typing import TYPE_CHECKING, Optional, Union, Tuple, List, Dict
+
+if TYPE_CHECKING:
+    from autofit.non_linear.result import Result
 
 from autoconf import conf, cached_property
-from autoconf.dictable import to_dict
+
+from autoconf.output import should_output
+
 from autofit import exc, jax_wrapper
 from autofit.database.sqlalchemy_ import sa
 from autofit.graphical import (
     MeanField,
     AnalysisFactor,
     _HierarchicalFactor,
     FactorApproximation,
@@ -27,15 +33,15 @@
 from autofit.non_linear.fitness import Fitness
 from autofit.non_linear.parallel import SneakyPool, SneakierPool
 from autofit.non_linear.paths.abstract import AbstractPaths
 from autofit.non_linear.paths.database import DatabasePaths
 from autofit.non_linear.paths.directory import DirectoryPaths
 from autofit.non_linear.paths.sub_directory_paths import SubDirectoryPaths
 from autofit.non_linear.samples.samples import Samples
-from autofit.non_linear.result import Result
+from autofit.non_linear.samples.summary import SamplesSummary
 from autofit.non_linear.timer import Timer
 from autofit.non_linear.analysis import Analysis
 from autofit.non_linear.analysis.combined import CombinedResult
 from autofit.non_linear.analysis.indexed import IndexCollectionAnalysis
 from autofit.non_linear.paths.null import NullPaths
 from autofit.graphical.declarative.abstract import PriorFactor
 from autofit.graphical.expectation_propagation import AbstractFactorOptimiser
@@ -67,14 +73,53 @@
         if self.number_of_cores == 1:
             return None
         return func(self, *args, **kwargs)
 
     return wrapper
 
 
+def configure_handler(func):
+    """
+    Add a file handler for logging during the course of the search.
+
+    Optionally outputs 'search.log' to the search's output directory. Can be
+    turned on or off in the output.yaml file.
+
+    Parameters
+    ----------
+    func
+        Some function for which logging should be output to file
+
+    Returns
+    -------
+    A decorated version of the function
+    """
+    root_logger = logging.getLogger()
+
+    def decorated(self, *args, **kwargs):
+        if not should_output("search_log"):
+            return func(self, *args, **kwargs)
+        try:
+            os.makedirs(
+                self.paths.output_path,
+                exist_ok=True,
+            )
+            handler = logging.FileHandler(self.paths.output_path / "search.log")
+            root_logger.addHandler(handler)
+        except AttributeError:
+            return func(self, *args, **kwargs)
+
+        try:
+            return func(self, *args, **kwargs)
+        finally:
+            root_logger.removeHandler(handler)
+
+    return decorated
+
+
 class NonLinearSearch(AbstractFactorOptimiser, ABC):
     def __init__(
         self,
         name: Optional[str] = None,
         path_prefix: Optional[str] = None,
         unique_tag: Optional[str] = None,
         initializer: Initializer = None,
@@ -152,19 +197,14 @@
             )
         else:
             self.paths = NullPaths()
 
         self.force_pickle_overwrite = conf.instance["general"]["output"][
             "force_pickle_overwrite"
         ]
-        self.skip_save_samples = kwargs.get("skip_save_samples")
-        if self.skip_save_samples is None:
-            self.skip_save_samples = conf.instance["general"]["output"].get(
-                "skip_save_samples"
-            )
 
         self.force_visualize_overwrite = conf.instance["general"]["output"][
             "force_visualize_overwrite"
         ]
 
         if initializer is None:
             self.logger.debug("Creating initializer ")
@@ -218,51 +258,52 @@
                 "OPENBLAS_NUM_THREADS",
                 "MKL_NUM_THREADS",
                 "OMP_NUM_THREADS",
                 "VECLIB_MAXIMUM_THREADS",
                 "NUMEXPR_NUM_THREADS",
             )
         ):
-            warnings.warn(
-                exc.SearchWarning(
-                    """
-                    The non-linear search is using multiprocessing (number_of_cores>1). 
-
-                    However, the following environment variables have not been set to 1:
-
-                    OPENBLAS_NUM_THREADS
-                    MKL_NUM_THREADS
-                    OMP_NUM_THREADS
-                    VECLIB_MAXIMUM_THREADS
-                    NUMEXPR_NUM_THREADS
-
-                    This can lead to performance issues, because both the non-linear search and libraries that may be
-                    used in your `log_likelihood_function` evaluation (e.g. NumPy, SciPy, scikit-learn) may attempt to
-                    parallelize over all cores available.
-
-                    This will lead to slow-down, due to overallocation of tasks over the CPUs.
-
-                    To mitigate this, set the environment variables to 1 via the following command on your
-                    bash terminal / command line:
-
-                    export OPENBLAS_NUM_THREADS=1
-                    export MKL_NUM_THREADS=1
-                    export OMP_NUM_THREADS=1
-                    export VECLIB_MAXIMUM_THREADS=1
-                    export NUMEXPR_NUM_THREADS=1
-
-                    This means only the non-linear search is parallelized over multiple cores.
-
-                    If you "know what you are doing" and do not want these environment variables to be set to one, you 
-                    can disable this warning by changing the following entry in the config files:
-
-                    `config -> general.yaml -> parallel: -> warn_environment_variable=False`
-                    """
+            if conf.instance["general"]["parallel"]["warn_environment_variables"]:
+                warnings.warn(
+                    exc.SearchWarning(
+                        """
+                        The non-linear search is using multiprocessing (number_of_cores>1). 
+    
+                        However, the following environment variables have not been set to 1:
+    
+                        OPENBLAS_NUM_THREADS
+                        MKL_NUM_THREADS
+                        OMP_NUM_THREADS
+                        VECLIB_MAXIMUM_THREADS
+                        NUMEXPR_NUM_THREADS
+    
+                        This can lead to performance issues, because both the non-linear search and libraries that may be
+                        used in your `log_likelihood_function` evaluation (e.g. NumPy, SciPy, scikit-learn) may attempt to
+                        parallelize over all cores available.
+    
+                        This will lead to slow-down, due to overallocation of tasks over the CPUs.
+    
+                        To mitigate this, set the environment variables to 1 via the following command on your
+                        bash terminal / command line:
+    
+                        export OPENBLAS_NUM_THREADS=1
+                        export MKL_NUM_THREADS=1
+                        export OMP_NUM_THREADS=1
+                        export VECLIB_MAXIMUM_THREADS=1
+                        export NUMEXPR_NUM_THREADS=1
+    
+                        This means only the non-linear search is parallelized over multiple cores.
+    
+                        If you "know what you are doing" and do not want these environment variables to be set to one, you 
+                        can disable this warning by changing the following entry in the config files:
+    
+                        `config -> general.yaml -> parallel: -> warn_environment_variables=False`
+                        """
+                    )
                 )
-            )
 
         self.optimisation_counter = Counter()
 
     __identifier_fields__ = tuple()
 
     def optimise(
         self,
@@ -481,15 +522,15 @@
 
     def fit(
         self,
         model: AbstractPriorModel,
         analysis: Analysis,
         info: Optional[Dict] = None,
         bypass_nuclear_if_on: bool = False,
-    ) -> Union["Result", List["Result"]]:
+    ) -> Union[Result, List[Result]]:
         """
         Fit a model, M with some function f that takes instances of the
         class represented by model M and gives a score for their fitness.
 
         A model which represents possible instances with some dimensionality is fit.
 
         The analysis provides two functions. One visualises an instance of a model and the
@@ -518,35 +559,18 @@
         produced by this fit.
 
         Raises
         ------
         AssertionError
             If the model has 0 dimensions.
         """
-
-        if os.environ.get("PYAUTOFIT_TEST_MODE") == "1":
-            from autofit.non_linear.search.nest.nautilus.search import Nautilus
-
-            if isinstance(self, Nautilus):
-                from autofit.non_linear.search.nest.dynesty.search.static import (
-                    DynestyStatic,
-                )
-
-                from pathlib import Path
-
-                search = DynestyStatic(
-                    paths=self.paths,
-                    unique_tag=self.unique_tag,
-                    number_of_cores=self.number_of_cores,
-                )
-
-                return search.fit(model=model, analysis=analysis, info=info)
-
         self.check_model(model=model)
 
+        logger.info(f"Starting non-linear search with {self.number_of_cores} cores.")
+
         model = analysis.modify_model(model)
         self.paths.model = model
         self.paths.unique_tag = self.unique_tag
 
         if self.is_master:
             self.paths.restore()
 
@@ -575,14 +599,15 @@
         if self.is_master:
             analysis = analysis.modify_after_fit(
                 paths=self.paths, model=model, result=result
             )
 
             self.post_fit_output(
                 bypass_nuclear_if_on=bypass_nuclear_if_on,
+                search_internal=result.search_internal,
             )
 
         return result
 
     def pre_fit_output(
         self, analysis: Analysis, model: AbstractPriorModel, info: Optional[Dict] = None
     ):
@@ -630,27 +655,27 @@
 
         if analysis.should_visualize(paths=self.paths):
             analysis.visualize_before_fit(
                 paths=self.paths,
                 model=model,
             )
             analysis.visualize_before_fit_combined(
-                analyses=None,
                 paths=self.paths,
                 model=model,
             )
 
-            timeout_seconds = get_timeout_seconds()
+        timeout_seconds = get_timeout_seconds()
 
-            if timeout_seconds is not None:
-                logger.info(
-                    f"\n\n ***Log Likelihood Function timeout is "
-                    f"turned on and set to {timeout_seconds} seconds.***\n"
-                )
+        if timeout_seconds is not None:
+            logger.info(
+                f"\n\n ***Log Likelihood Function timeout is "
+                f"turned on and set to {timeout_seconds} seconds.***\n"
+            )
 
+    @configure_handler
     def start_resume_fit(self, analysis: Analysis, model: AbstractPriorModel) -> Result:
         """
         Start a non-linear search from scratch, or resumes one which was previously terminated mid-way through.
 
         If the search is resumed, the model-fit will begin by loading the samples from the previous search and
         from where it left off.
 
@@ -688,34 +713,43 @@
             model=model,
             analysis=analysis,
             search_internal=search_internal,
             during_analysis=False,
         )
 
         result = analysis.make_result(
+            samples_summary=samples.summary(),
+            paths=self.paths,
             samples=samples,
+            search_internal=search_internal,
         )
 
         if self.is_master:
             analysis.save_results(paths=self.paths, result=result)
+            analysis.save_results_combined(paths=self.paths, result=result)
 
         model.unfreeze()
 
         self.paths.completed()
 
         return result
 
     def result_via_completed_fit(
-        self, analysis: Analysis, model: AbstractPriorModel, search_internal=None
+        self,
+        analysis: Analysis,
+        model: AbstractPriorModel,
     ) -> Result:
         """
         Returns the result of the non-linear search of a completed model-fit.
 
-        The result contains the non-linear search samples, which are loaded from the searches internal results,
-        or the `samples.csv` file if the internal results are not available.
+        The result contains the non-linear search samples summary, which contains the maximum log likelihood instance
+        that is used for visualization and prior passing via the search chaining API.
+
+        This funciton may also load the full samples of the completed fit, for example if visualization of the
+        seatch chains (e.g. a corner plot) is performed. This task is optional and be slow due to loading times.
 
         Optional tasks can be performed to update the results of the model-fit on hard-disk depending on the following
         entries of the `general.yaml` config file's `output` section:
 
         ` `force_visualize_overwrite=True`: the visualization of the model-fit is performed again (e.g. to
         add new visualizations or replot figures with a different source code).
 
@@ -726,51 +760,56 @@
         ----------
         analysis
             An object that encapsulates the data and a log likelihood function which fits the model to the data
             via the non-linear search.
         model
             The model that is fitted to the data, which is used by the non-linear search to create instances of
             the model that are fitted to the data via the log likelihood function.
+
         Returns
         -------
         The result of the non-linear search, which includes the best-fit model instance and best-fit log likelihood
         and errors on the model parameters.
         """
 
         model.freeze()
-        samples = self.samples_from(model=model)
+        samples_summary = self.paths.load_samples_summary()
+        try:
+            samples = self.paths.samples
+        except FileNotFoundError:
+            samples = None
 
         result = analysis.make_result(
+            samples_summary=samples_summary,
             samples=samples,
+            paths=self.paths,
         )
 
         if self.is_master:
             self.logger.info(f"Fit Already Completed: skipping non-linear search.")
 
             if self.force_visualize_overwrite:
                 self.perform_visualization(
                     model=model,
                     analysis=analysis,
-                    search_internal=search_internal,
+                    samples_summary=samples_summary,
                     during_analysis=False,
                 )
 
             if self.force_pickle_overwrite:
                 self.logger.info("Forcing pickle overwrite")
 
-                if not self.skip_save_samples:
-                    self.paths.save_json("samples_summary", to_dict(samples.summary()))
-
                 analysis.save_results(paths=self.paths, result=result)
+                analysis.save_results_combined(paths=self.paths, result=result)
 
         model.unfreeze()
 
         return result
 
-    def post_fit_output(self, bypass_nuclear_if_on: bool):
+    def post_fit_output(self, search_internal, bypass_nuclear_if_on: bool):
         """
         Cleans up the output folderds after a completed non-linear search.
 
         The main task this performs is removing the folder containing the results of a non-linear search such that only
         its corresponding `.zip` file is left. This is use for supercomputers, where users often have a file limit on
         the number of files they can store in their home directory, so storing them all in just a .zip file is
         advantageous.
@@ -778,30 +817,36 @@
         This only occurs if `remove_files=False` in the `general.yaml` config file's `output` section.
 
         Parameters
         ----------
         bypass_nuclear_if_on
             Whether to use nuclear mode to delete a lot of files (see nuclear mode description).
         """
+        if not conf.instance["output"]["search_internal"]:
+            self.logger.info("Removing search internal folder.")
+            self.paths.remove_search_internal()
+        else:
+            self.output_search_internal(search_internal=search_internal)
+
         self.logger.info("Removing all files except for .zip file")
         self.paths.zip_remove()
 
         if not bypass_nuclear_if_on:
             self.paths.zip_remove_nuclear()
 
     @abstractmethod
     def _fit(self, model: AbstractPriorModel, analysis: Analysis):
         pass
 
     def check_model(self, model: AbstractPriorModel):
         if model is not None and model.prior_count == 0:
             raise AssertionError("Model has no priors! Cannot fit a 0 dimension model.")
 
-    def config_dict_with_test_mode_settings_from(self, config_dict: Dict) -> Dict:
-        return config_dict
+    def config_dict_test_mode_from(self, config_dict: Dict) -> Dict:
+        raise NotImplementedError
 
     @property
     def _class_config(self) -> Dict:
         return self.config_type[self.__class__.__name__]
 
     @cached_property
     def config_dict_search(self) -> Dict:
@@ -824,17 +869,15 @@
                 config_dict[key] = self.kwargs[key]
             except KeyError:
                 pass
 
         if os.environ.get("PYAUTOFIT_TEST_MODE") == "1":
             logger.warning(f"TEST MODE ON: SEARCH WILL SKIP SAMPLING\n\n")
 
-            config_dict = self.config_dict_with_test_mode_settings_from(
-                config_dict=config_dict
-            )
+            config_dict = self.config_dict_test_mode_from(config_dict=config_dict)
 
         return config_dict
 
     @property
     def config_dict_settings(self) -> Dict:
         return self._class_config["settings"]
 
@@ -854,29 +897,34 @@
         Returns
         -------
         attribute
             An attribute for the key with the specified type.
         """
         return self._class_config[section][attribute_name]
 
+    def output_search_internal(self, search_internal):
+        self.paths.save_search_internal(
+            obj=search_internal,
+        )
+
     def perform_update(
         self,
         model: AbstractPriorModel,
         analysis: Analysis,
         during_analysis: bool,
         search_internal=None,
     ) -> Samples:
         """
         Perform an update of the non-linear search's model-fitting results.
 
         This occurs every `iterations_per_update` of the non-linear search and once it is complete.
 
         The update performs the following tasks (if the settings indicate they should be performed):
 
-        1) Visualize the search results (e.g. a cornerplot).
+        1) Visualize the search results.
         2) Visualize the maximum log likelihood model using model-specific visualization implented via the `Analysis`
            object.
         3) Perform profiling of the analysis object `log_likelihood_function` and ouptut run-time information.
         4) Output the `search.summary` file which contains information on model-fitting so far.
         5) Output the `model.results` file which contains a concise text summary of the model results so far.
 
         Parameters
@@ -890,44 +938,57 @@
             If the update is during a non-linear search, in which case tasks are only performed after a certain number
             of updates and only a subset of visualization may be performed.
         """
 
         self.iterations += self.iterations_per_update
         if during_analysis:
             self.logger.info(
-                f"Fit Still Running: Updating results after {self.iterations} iterations (see "
-                f"output folder for latest visualization, samples, etc.)"
+                f"""Fit Running: Updating results after {self.iterations} iterations (see output folder)."""
             )
         else:
             self.logger.info(
-                f"Fit Complete: Updating final results (see "
-                f"output folder for final visualization, samples, etc.)"
+                "Fit Complete: Updating final results (see output folder)."
             )
 
         if not isinstance(self.paths, DatabasePaths) and not isinstance(
             self.paths, NullPaths
         ):
             self.timer.update()
 
         samples = self.samples_from(model=model, search_internal=search_internal)
+        samples_summary = samples.summary()
 
         try:
-            instance = samples.max_log_likelihood()
+            instance = samples_summary.instance
         except exc.FitException:
             return samples
 
         if self.is_master:
-            self.paths.samples_to_csv(samples=samples)
+            self.paths.save_samples_summary(samples_summary=samples_summary)
+
+            samples_save = samples
+            samples_save = samples_save.samples_above_weight_threshold_from(
+                log_message=not during_analysis
+            )
+            self.paths.save_samples(samples=samples_save)
 
-            if not self.skip_save_samples:
-                self.paths.save_json("samples_summary", to_dict(samples.summary()))
+            latent_samples = None
+
+            if (during_analysis and conf.instance["output"]["latent_during_fit"]) or (
+                not during_analysis and conf.instance["output"]["latent_after_fit"]
+            ):
+                latent_samples = analysis.compute_latent_samples(samples_save)
+
+                if latent_samples:
+                    self.paths.save_latent_samples(latent_samples)
 
             self.perform_visualization(
                 model=model,
                 analysis=analysis,
+                samples_summary=samples_summary,
                 during_analysis=during_analysis,
                 search_internal=search_internal,
             )
 
             if self.should_profile:
                 self.logger.debug("Profiling Maximum Likelihood Model")
                 analysis.profile_log_likelihood_function(
@@ -944,89 +1005,84 @@
 
                 start = time.time()
                 log_likelihood_function(instance=instance)
                 log_likelihood_function_time = time.time() - start
 
                 self.paths.save_summary(
                     samples=samples,
+                    latent_samples=latent_samples,
                     log_likelihood_function_time=log_likelihood_function_time,
                 )
             except exc.FitException:
                 pass
 
             if not during_analysis and self.remove_state_files_at_end:
                 self.logger.debug("Removing state files")
-                try:
-                    self.remove_state_files()
-                except FileNotFoundError:
-                    pass
 
         return samples
 
     def perform_visualization(
         self,
         model: AbstractPriorModel,
         analysis: AbstractPriorModel,
+        samples_summary: SamplesSummary,
         during_analysis: bool,
         search_internal=None,
     ):
         """
         Perform visualization of the non-linear search's model-fitting results.
 
         This occurs every `iterations_per_update` of the non-linear search, when the search is complete and can
         also be forced to occur even though a search is completed on a rerun, to update the visualization
         with different `matplotlib` settings.
 
         The update performs the following tasks (if the settings indicate they should be performed):
 
-        1) Visualize the search results (e.g. a cornerplot).
-        2) Visualize the maximum log likelihood model using model-specific visualization implented via the `Analysis`
+        1) Visualize the maximum log likelihood model using model-specific visualization implented via the `Analysis`
            object.
+        2) Visualize the search results.
 
         Parameters
         ----------
         model
             The model which generates instances for different points in parameter space.
         analysis
             Contains the data and the log likelihood function which fits an instance of the model to the data, returning
             the log likelihood the `NonLinearSearch` maximizes.
         during_analysis
             If the update is during a non-linear search, in which case tasks are only performed after a certain number
             of updates and only a subset of visualization may be performed.
         """
-        samples = self.samples_from(model=model, search_internal=search_internal)
-
-        try:
-            instance = samples.max_log_likelihood()
-        except exc.FitException:
-            return samples
-
-        if analysis.should_visualize(paths=self.paths, during_analysis=during_analysis):
-            if not isinstance(self.paths, NullPaths):
-                self.plot_results(samples=samples)
 
         self.logger.debug("Visualizing")
+
         if analysis.should_visualize(paths=self.paths, during_analysis=during_analysis):
             analysis.visualize(
-                paths=self.paths, instance=instance, during_analysis=during_analysis
+                paths=self.paths,
+                instance=samples_summary.instance,
+                during_analysis=during_analysis,
             )
             analysis.visualize_combined(
-                analyses=None,
                 paths=self.paths,
-                instance=instance,
+                instance=samples_summary.instance,
                 during_analysis=during_analysis,
             )
 
+        if analysis.should_visualize(paths=self.paths, during_analysis=during_analysis):
+            if not isinstance(self.paths, NullPaths):
+                samples = self.samples_from(
+                    model=model, search_internal=search_internal
+                )
+
+                self.plot_results(samples=samples)
+
     @property
     def samples_cls(self):
         raise NotImplementedError()
 
-    def remove_state_files(self):
-        pass
-
     def samples_from(self, model: AbstractPriorModel, search_internal=None) -> Samples:
         """
         Loads the samples of a non-linear search from its output files.
 
         The samples can be loaded from one of two files, which are attempted to be loading in the following order:
 
         1) Load via the internal results of the non-linear search, which are specified to that search's outputs
@@ -1041,42 +1097,21 @@
             The model which generates instances for different points in parameter space.
         """
         try:
             return self.samples_via_internal_from(
                 model=model, search_internal=search_internal
             )
         except (FileNotFoundError, NotImplementedError, AttributeError):
-            return self.samples_via_csv_from(model=model)
+            return self.paths.samples
 
     def samples_via_internal_from(
         self, model: AbstractPriorModel, search_internal=None
     ):
         raise NotImplementedError
 
-    def samples_via_csv_from(self, model: AbstractPriorModel) -> Samples:
-        """
-        Returns a `Samples` object from the `samples.csv` and `samples_info.json` files.
-
-        The samples contain all information on the parameter space sampling (e.g. the parameters,
-        log likelihoods, etc.).
-
-        The samples in csv format are already converted to the autofit format, where samples are lists of values
-        (e.g. `parameter_lists`, `log_likelihood_list`).
-
-        Parameters
-        ----------
-        model
-            Maps input vectors of unit parameter values to physical values and model instances via priors.
-        """
-
-        return self.samples_cls.from_csv(
-            paths=self.paths,
-            model=model,
-        )
-
     @check_cores
     def make_pool(self):
         """Make the pool instance used to parallelize a `NonLinearSearch` alongside a set of unique ids for every
         process in the pool. If the specified number of cores is 1, a pool instance is not made and None is returned.
 
         The pool cannot be set as an attribute of the class itself because this prevents pickling, thus it is generated
         via this function before calling the non-linear search.
@@ -1129,8 +1164,8 @@
 
         return pool
 
     def __eq__(self, other):
         return isinstance(other, NonLinearSearch) and self.__dict__ == other.__dict__
 
     def plot_results(self, samples):
-        pass
+        raise NotImplementedError
```

### Comparing `autofit-2024.1.27.4/autofit/non_linear/search/mcmc/abstract_mcmc.py` & `autofit-2024.5.16.0/autofit/non_linear/search/mcmc/abstract_mcmc.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 from autoconf import conf
 from autofit.database.sqlalchemy_ import sa
 from autofit.non_linear.search.abstract_search import NonLinearSearch
 from autofit.non_linear.initializer import Initializer
 from autofit.non_linear.samples import SamplesMCMC
 from autofit.non_linear.search.mcmc.auto_correlations import AutoCorrelationsSettings
-
+from autofit.non_linear.plot.mcmc_plotters import MCMCPlotter
+from autofit.non_linear.plot.output import Output
 
 class AbstractMCMC(NonLinearSearch):
 
     def __init__(
             self,
             name: Optional[str] = None,
             path_prefix: Optional[str] = None,
@@ -41,8 +42,28 @@
 
     @property
     def config_type(self):
         return conf.instance["non_linear"]["mcmc"]
 
     @property
     def samples_cls(self):
-        return SamplesMCMC
+        return SamplesMCMC
+
+    @property
+    def plotter_cls(self):
+        return MCMCPlotter
+
+    def plot_results(self, samples):
+
+        if not samples.pdf_converged:
+            return
+
+        def should_plot(name):
+            return conf.instance["visualize"]["plots_search"]["mcmc"][name]
+
+        plotter = self.plotter_cls(
+            samples=samples,
+            output=Output(path=self.paths.image_path / "search", format="png"),
+        )
+
+        if should_plot("corner_cornerpy"):
+            plotter.corner_cornerpy()
```

### Comparing `autofit-2024.1.27.4/autofit/non_linear/search/mcmc/auto_correlations.py` & `autofit-2024.5.16.0/autofit/non_linear/search/mcmc/auto_correlations.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/non_linear/search/mcmc/emcee/search.py` & `autofit-2024.5.16.0/autofit/non_linear/search/mcmc/emcee/search.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 import os
-from typing import Optional
+from typing import Dict, Optional
 
 import emcee
 import numpy as np
 
-from autoconf import conf
 from autofit.database.sqlalchemy_ import sa
 from autofit.mapper.model_mapper import ModelMapper
 from autofit.mapper.prior_model.abstract import AbstractPriorModel
 from autofit.non_linear.fitness import Fitness
 from autofit.non_linear.initializer import Initializer
 from autofit.non_linear.search.mcmc.abstract_mcmc import AbstractMCMC
 from autofit.non_linear.search.mcmc.auto_correlations import AutoCorrelationsSettings
 from autofit.non_linear.search.mcmc.auto_correlations import AutoCorrelations
 from autofit.non_linear.samples.sample import Sample
 from autofit.non_linear.samples.mcmc import SamplesMCMC
-from autofit.plot import EmceePlotter
-from autofit.plot.output import Output
 
 
 class Emcee(AbstractMCMC):
     __identifier_fields__ = ("nwalkers",)
 
     def __init__(
         self,
@@ -102,16 +99,17 @@
         -------
         A result object comprising the Samples object that inclues the maximum log likelihood instance and full
         chains used by the fit.
         """
         fitness = Fitness(
             model=model,
             analysis=analysis,
+            paths=self.paths,
             fom_is_log_likelihood=False,
-            resample_figure_of_merit=-np.inf
+            resample_figure_of_merit=-np.inf,
         )
 
         pool = self.make_sneaky_pool(fitness)
 
         try:
             backend = emcee.backends.HDFBackend(filename=self.backend_filename)
         except TypeError:
@@ -145,14 +143,16 @@
                 unit_parameter_lists,
                 parameter_lists,
                 log_posterior_list,
             ) = self.initializer.samples_from_model(
                 total_points=search_internal.nwalkers,
                 model=model,
                 fitness=fitness,
+                paths=self.paths,
+                n_cores=self.number_of_cores,
             )
 
             state = np.zeros(shape=(search_internal.nwalkers, model.prior_count))
 
             self.logger.info(
                 "Starting new Emcee non-linear search (no previous samples found)."
             )
@@ -182,41 +182,57 @@
 
             total_iterations += iterations
             iterations_remaining = self.config_dict_run["nsteps"] - total_iterations
 
             samples = self.samples_from(model=model, search_internal=search_internal)
 
             if self.auto_correlation_settings.check_for_convergence:
-                if search_internal.iteration > self.auto_correlation_settings.check_size:
+                if (
+                    search_internal.iteration
+                    > self.auto_correlation_settings.check_size
+                ):
                     if samples.converged:
                         iterations_remaining = 0
 
             if iterations_remaining > 0:
-
                 self.perform_update(
                     model=model,
                     analysis=analysis,
                     search_internal=search_internal,
-                    during_analysis=True
+                    during_analysis=True,
                 )
+
         return search_internal
 
-    def samples_info_from(self, search_internal=None):
+    def output_search_internal(self, search_internal):
+        """
+        Output the sampler results to hard-disk in their internal format.
+
+        Emcee uses a backend to store and load results, therefore the outputting of the search internal to a
+        dill file is disabled.
+
+        Parameters
+        ----------
+        sampler
+            The nautilus sampler object containing the results of the model-fit.
+        """
+        pass
 
+    def samples_info_from(self, search_internal=None):
         search_internal = search_internal or self.backend
 
         auto_correlations = self.auto_correlations_from(search_internal=search_internal)
 
         return {
             "check_size": auto_correlations.check_size,
             "required_length": auto_correlations.required_length,
             "change_threshold": auto_correlations.change_threshold,
             "total_walkers": len(search_internal.get_chain()[0, :, 0]),
             "total_steps": len(search_internal.get_log_prob()),
-            "time": self.timer.time if self.timer else None
+            "time": self.timer.time if self.timer else None,
         }
 
     def samples_via_internal_from(self, model, search_internal=None):
         """
         Returns a `Samples` object from the emcee internal results.
 
         The samples contain all information on the parameter space sampling (e.g. the parameters,
@@ -230,22 +246,22 @@
         model
             Maps input vectors of unit parameter values to physical values and model instances via priors.
         """
 
         search_internal = search_internal or self.backend
 
         if os.environ.get("PYAUTOFIT_TEST_MODE") == "1":
-
             samples_after_burn_in = search_internal.get_chain(
-            discard=5, thin=5, flat=True
-        )
+                discard=5, thin=5, flat=True
+            )
 
         else:
-
-            auto_correlations = self.auto_correlations_from(search_internal=search_internal)
+            auto_correlations = self.auto_correlations_from(
+                search_internal=search_internal
+            )
 
             discard = int(3.0 * np.max(auto_correlations.times))
             thin = int(np.max(auto_correlations.times) / 2.0)
             samples_after_burn_in = search_internal.get_chain(
                 discard=discard, thin=thin, flat=True
             )
 
@@ -274,21 +290,21 @@
             weight_list=weight_list,
         )
 
         return SamplesMCMC(
             model=model,
             sample_list=sample_list,
             samples_info=self.samples_info_from(search_internal=search_internal),
-            search_internal=search_internal,
             auto_correlation_settings=self.auto_correlation_settings,
-            auto_correlations=self.auto_correlations_from(search_internal=search_internal),
+            auto_correlations=self.auto_correlations_from(
+                search_internal=search_internal
+            ),
         )
 
     def auto_correlations_from(self, search_internal=None):
-
         search_internal = search_internal or self.backend
 
         times = search_internal.get_autocorr_time(tol=0)
 
         previous_auto_correlation_times = emcee.autocorr.integrated_time(
             x=search_internal.get_chain()[
                 : -self.auto_correlation_settings.check_size, :, :
@@ -300,15 +316,32 @@
             check_size=self.auto_correlation_settings.check_size,
             required_length=self.auto_correlation_settings.required_length,
             change_threshold=self.auto_correlation_settings.change_threshold,
             times=times,
             previous_times=previous_auto_correlation_times,
         )
 
-    def config_dict_with_test_mode_settings_from(self, config_dict):
+    def config_dict_test_mode_from(self, config_dict: Dict) -> Dict:
+        """
+        Returns a configuration dictionary for test mode meaning that the sampler terminates as quickly as possible.
+
+        Entries which set the total number of samples of the sampler (e.g. maximum calls, maximum likelihood
+        evaluations) are reduced to low values meaning it terminates nearly immediately.
+
+        Parameters
+        ----------
+        config_dict
+            The original configuration dictionary for this sampler which includes entries controlling how fast the
+            sampler terminates.
+
+        Returns
+        -------
+        A configuration dictionary where settings which control the sampler's number of samples are reduced so it
+        terminates as quickly as possible.
+        """
         return {
             **config_dict,
             "nwalkers": 20,
             "nsteps": 10,
         }
 
     @property
@@ -325,28 +358,7 @@
 
         if os.path.isfile(self.backend_filename):
             return emcee.backends.HDFBackend(filename=str(self.backend_filename))
         else:
             raise FileNotFoundError(
                 f"The file search_internal.hdf does not exist at the path {self.paths.search_internal_path}"
             )
-
-    def plot_results(self, samples):
-        def should_plot(name):
-            return conf.instance["visualize"]["plots_search"]["emcee"][name]
-
-        plotter = EmceePlotter(
-            samples=samples,
-            output=Output(path=self.paths.image_path / "search", format="png"),
-        )
-
-        if should_plot("corner"):
-            plotter.corner()
-
-        if should_plot("trajectories"):
-            plotter.trajectories()
-
-        if should_plot("likelihood_series"):
-            plotter.likelihood_series()
-
-        if should_plot("time_series"):
-            plotter.time_series()
```

### Comparing `autofit-2024.1.27.4/autofit/non_linear/search/mcmc/zeus/search.py` & `autofit-2024.5.16.0/autofit/non_linear/search/mcmc/zeus/search.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,46 +1,44 @@
-from typing import Optional
+from typing import Dict, Optional
 
 import numpy as np
 
-from autoconf import conf
 from autofit.database.sqlalchemy_ import sa
 from autofit.mapper.model_mapper import ModelMapper
 from autofit.mapper.prior_model.abstract import AbstractPriorModel
 from autofit.non_linear.fitness import Fitness
 from autofit.non_linear.initializer import Initializer
 from autofit.non_linear.search.mcmc.abstract_mcmc import AbstractMCMC
 from autofit.non_linear.search.mcmc.auto_correlations import AutoCorrelationsSettings
 from autofit.non_linear.search.mcmc.auto_correlations import AutoCorrelations
-from autofit.non_linear.search.mcmc.zeus.plotter import ZeusPlotter
 from autofit.non_linear.samples.sample import Sample
 from autofit.non_linear.samples.mcmc import SamplesMCMC
-from autofit.plot.output import Output
+
 
 class Zeus(AbstractMCMC):
     __identifier_fields__ = (
         "nwalkers",
         "tune",
         "tolerance",
         "patience",
         "mu",
         "light_mode",
     )
 
     def __init__(
-            self,
-            name: Optional[str] = None,
-            path_prefix: Optional[str] = None,
-            unique_tag: Optional[str] = None,
-            initializer: Optional[Initializer] = None,
-            auto_correlation_settings=AutoCorrelationsSettings(),
-            iterations_per_update: int = None,
-            number_of_cores: int = None,
-            session: Optional[sa.orm.Session] = None,
-            **kwargs
+        self,
+        name: Optional[str] = None,
+        path_prefix: Optional[str] = None,
+        unique_tag: Optional[str] = None,
+        initializer: Optional[Initializer] = None,
+        auto_correlation_settings=AutoCorrelationsSettings(),
+        iterations_per_update: int = None,
+        number_of_cores: int = None,
+        session: Optional[sa.orm.Session] = None,
+        **kwargs
     ):
         """
         An Zeus non-linear search.
 
         For a full description of Zeus, checkout its Github and readthedocs webpages:
 
         https://github.com/minaskar/zeus
@@ -123,20 +121,20 @@
             )
 
         pool = self.make_pool()
 
         fitness = Fitness(
             model=model,
             analysis=analysis,
+            paths=self.paths,
             fom_is_log_likelihood=False,
-            resample_figure_of_merit=-np.inf
+            resample_figure_of_merit=-np.inf,
         )
 
         try:
-
             search_internal = self.paths.load_search_internal()
 
             state = search_internal.get_last_sample()
             log_posterior_list = search_internal.get_last_log_prob()
 
             samples = self.samples_from(model=model, search_internal=search_internal)
 
@@ -148,15 +146,14 @@
                 iterations_remaining = self.config_dict_run["nsteps"] - total_iterations
 
                 self.logger.info(
                     "Resuming Zeus non-linear search (previous samples found)."
                 )
 
         except (FileNotFoundError, AttributeError):
-
             search_internal = zeus.EnsembleSampler(
                 nwalkers=self.config_dict_search["nwalkers"],
                 ndim=model.prior_count,
                 logprob_fn=fitness.__call__,
                 pool=pool,
             )
 
@@ -166,15 +163,17 @@
                 unit_parameter_lists,
                 parameter_lists,
                 log_posterior_list,
             ) = self.initializer.samples_from_model(
                 total_points=search_internal.nwalkers,
                 model=model,
                 fitness=fitness,
-                test_mode_samples=False
+                test_mode_samples=False,
+                paths=self.paths,
+                n_cores=self.number_of_cores,
             )
 
             state = np.zeros(shape=(search_internal.nwalkers, model.prior_count))
 
             self.logger.info(
                 "Starting new Zeus non-linear search (no previous samples found)."
             )
@@ -182,25 +181,24 @@
             for index, parameters in enumerate(parameter_lists):
                 state[index, :] = np.asarray(parameters)
 
             total_iterations = 0
             iterations_remaining = self.config_dict_run["nsteps"]
 
         while iterations_remaining > 0:
-
             if self.iterations_per_update > iterations_remaining:
                 iterations = iterations_remaining
             else:
                 iterations = self.iterations_per_update
 
             for sample in search_internal.sample(
-                    start=state,
-                    log_prob0=log_posterior_list,
-                    iterations=iterations,
-                    progress=True,
+                start=state,
+                log_prob0=log_posterior_list,
+                iterations=iterations,
+                progress=True,
             ):
                 pass
 
             search_internal.ncall_total += search_internal.ncall
 
             self.paths.save_search_internal(
                 obj=search_internal,
@@ -211,46 +209,47 @@
 
             total_iterations += iterations
             iterations_remaining = self.config_dict_run["nsteps"] - total_iterations
 
             samples = self.samples_from(model=model, search_internal=search_internal)
 
             if self.auto_correlation_settings.check_for_convergence:
-                if search_internal.iteration > self.auto_correlation_settings.check_size:
+                if (
+                    search_internal.iteration
+                    > self.auto_correlation_settings.check_size
+                ):
                     if samples.converged:
                         iterations_remaining = 0
 
-            auto_correlation_time = zeus.AutoCorrTime(samples=search_internal.get_chain())
+            auto_correlation_time = zeus.AutoCorrTime(
+                samples=search_internal.get_chain()
+            )
 
             discard = int(3.0 * np.max(auto_correlation_time))
             thin = int(np.max(auto_correlation_time) / 2.0)
             chain = search_internal.get_chain(discard=discard, thin=thin, flat=True)
 
             if "maxcall" in self.kwargs:
                 if search_internal.ncall_total > self.kwargs["maxcall"]:
                     iterations_remaining = 0
 
             if iterations_remaining > 0:
-
                 self.perform_update(
                     model=model,
                     analysis=analysis,
                     search_internal=search_internal,
-                    during_analysis=True
+                    during_analysis=True,
                 )
 
         return search_internal
 
-    def samples_info_from(self, search_internal = None):
-
+    def samples_info_from(self, search_internal=None):
         search_internal = search_internal or self.paths.load_search_internal()
 
-        auto_correlations = self.auto_correlations_from(
-            search_internal=search_internal
-        )
+        auto_correlations = self.auto_correlations_from(search_internal=search_internal)
 
         return {
             "check_size": auto_correlations.check_size,
             "required_length": auto_correlations.required_length,
             "change_threshold": auto_correlations.change_threshold,
             "total_walkers": len(search_internal.get_chain()[0, :, 0]),
             "total_steps": int(search_internal.ncall_total),
@@ -271,99 +270,89 @@
         ----------
         model
             Maps input vectors of unit parameter values to physical values and model instances via priors.
         """
 
         search_internal = search_internal or self.paths.load_search_internal()
 
-        auto_correlations = self.auto_correlations_from(
-            search_internal=search_internal
-        )
+        auto_correlations = self.auto_correlations_from(search_internal=search_internal)
 
         discard = int(3.0 * np.max(auto_correlations.times))
         thin = int(np.max(auto_correlations.times) / 2.0)
-        samples_after_burn_in =  search_internal.get_chain(discard=discard, thin=thin, flat=True)
+        samples_after_burn_in = search_internal.get_chain(
+            discard=discard, thin=thin, flat=True
+        )
 
         parameter_lists = samples_after_burn_in.tolist()
         log_posterior_list = search_internal.get_log_prob(flat=True).tolist()
         log_prior_list = model.log_prior_list_from(parameter_lists=parameter_lists)
 
         log_likelihood_list = [
             log_posterior - log_prior
-            for log_posterior, log_prior
-            in zip(log_posterior_list, log_prior_list)
+            for log_posterior, log_prior in zip(log_posterior_list, log_prior_list)
         ]
 
         weight_list = len(log_likelihood_list) * [1.0]
 
         sample_list = Sample.from_lists(
             model=model,
             parameter_lists=parameter_lists,
             log_likelihood_list=log_likelihood_list,
             log_prior_list=log_prior_list,
-            weight_list=weight_list
+            weight_list=weight_list,
         )
 
         return SamplesMCMC(
             model=model,
             sample_list=sample_list,
             samples_info=self.samples_info_from(search_internal=search_internal),
-            search_internal=search_internal,
             auto_correlation_settings=self.auto_correlation_settings,
             auto_correlations=auto_correlations,
         )
 
     def auto_correlations_from(self, search_internal=None):
-
         import zeus
 
         search_internal = search_internal or self.paths.load_search_internal()
 
         times = zeus.AutoCorrTime(samples=search_internal.get_chain())
         try:
             previous_auto_correlation_times = zeus.AutoCorrTime(
-                samples=search_internal.get_chain()[: - self.auto_correlation_settings.check_size, :, :],
+                samples=search_internal.get_chain()[
+                    : -self.auto_correlation_settings.check_size, :, :
+                ],
             )
         except IndexError:
-            self.logger.debug(
-                "Unable to compute previous auto correlation times."
-            )
+            self.logger.debug("Unable to compute previous auto correlation times.")
             previous_auto_correlation_times = None
 
         return AutoCorrelations(
             check_size=self.auto_correlation_settings.check_size,
             required_length=self.auto_correlation_settings.required_length,
             change_threshold=self.auto_correlation_settings.change_threshold,
             times=times,
             previous_times=previous_auto_correlation_times,
         )
 
-    def config_dict_with_test_mode_settings_from(self, config_dict):
+    def config_dict_test_mode_from(self, config_dict: Dict) -> Dict:
+        """
+        Returns a configuration dictionary for test mode meaning that the sampler terminates as quickly as possible.
 
+        Entries which set the total number of samples of the sampler (e.g. maximum calls, maximum likelihood
+        evaluations) are reduced to low values meaning it terminates nearly immediately.
+
+        Parameters
+        ----------
+        config_dict
+            The original configuration dictionary for this sampler which includes entries controlling how fast the
+            sampler terminates.
+
+        Returns
+        -------
+        A configuration dictionary where settings which control the sampler's number of samples are reduced so it
+        terminates as quickly as possible.
+        """
         return {
             **config_dict,
             "nwalkers": 20,
             "nsteps": 10,
         }
-
-    def plot_results(self, samples):
-        def should_plot(name):
-            return conf.instance["visualize"]["plots_search"]["zeus"][name]
-
-        plotter = ZeusPlotter(
-            samples=samples,
-            output=Output(
-                path=self.paths.image_path / "search", format="png"
-            ),
-        )
-
-        if should_plot("corner"):
-            plotter.corner()
-
-        if should_plot("trajectories"):
-            plotter.trajectories()
-
-        if should_plot("likelihood_series"):
-            plotter.likelihood_series()
-
-        if should_plot("time_series"):
-            plotter.time_series()
```

### Comparing `autofit-2024.1.27.4/autofit/non_linear/search/nest/abstract_nest.py` & `autofit-2024.5.16.0/autofit/non_linear/search/nest/abstract_nest.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from abc import ABC
 from typing import Optional
+import warnings
 
 from autoconf import conf
 from autofit.database.sqlalchemy_ import sa
 from autofit.non_linear.search.abstract_search import NonLinearSearch
 from autofit.non_linear.initializer import (
     InitializerPrior,
     AbstractInitializer,
     SpecificRangeInitializer,
 )
 from autofit.non_linear.samples import SamplesNest
+from autofit.non_linear.plot.nest_plotters import NestPlotter
+from autofit.non_linear.plot.output import Output
 
 
 class AbstractNest(NonLinearSearch, ABC):
     def __init__(
         self,
         name: Optional[str] = None,
         path_prefix: Optional[str] = None,
@@ -60,7 +63,25 @@
     @property
     def config_type(self):
         return conf.instance["non_linear"]["nest"]
 
     @property
     def samples_cls(self):
         return SamplesNest
+
+    @property
+    def plotter_cls(self):
+        return NestPlotter
+
+    def plot_results(self, samples):
+
+        def should_plot(name):
+            return conf.instance["visualize"]["plots_search"]["nest"][name]
+
+        plotter = self.plotter_cls(
+            samples=samples,
+            output=Output(path=self.paths.image_path / "search", format="png"),
+        )
+        if should_plot("corner_anesthetic"):
+            with warnings.catch_warnings():
+                warnings.simplefilter("ignore")
+                plotter.corner_anesthetic()
```

### Comparing `autofit-2024.1.27.4/autofit/non_linear/search/nest/dynesty/search/abstract.py` & `autofit-2024.5.16.0/autofit/non_linear/search/nest/dynesty/search/abstract.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import os
 from abc import ABC
-from typing import Optional, Tuple, Union
+from typing import Dict, Optional, Tuple, Union
 
 import numpy as np
 from dynesty import NestedSampler, DynamicNestedSampler
+import warnings
 
 from autoconf import conf
 from autofit import exc
 from autofit.database.sqlalchemy_ import sa
 from autofit import jax_wrapper
 from autofit.non_linear.fitness import Fitness
 from autofit.mapper.prior_model.abstract import AbstractPriorModel
 from autofit.non_linear.paths.null import NullPaths
 from autofit.non_linear.search.nest.abstract_nest import AbstractNest
 from autofit.non_linear.samples.sample import Sample
 from autofit.non_linear.samples.nest import SamplesNest
-from autofit.plot.output import Output
 
 
 def prior_transform(cube, model):
     phys_cube = model.vector_from_unit_vector(
         unit_vector=cube, ignore_prior_limits=True
     )
 
@@ -116,14 +116,15 @@
         """
 
         from dynesty.pool import Pool
 
         fitness = Fitness(
             model=model,
             analysis=analysis,
+            paths=self.paths,
             fom_is_log_likelihood=True,
             resample_figure_of_merit=-1.0e99,
         )
 
         if not isinstance(self.paths, NullPaths):
             checkpoint_exists = os.path.exists(self.checkpoint_file)
         else:
@@ -196,26 +197,28 @@
                 self.perform_update(
                     model=model,
                     analysis=analysis,
                     search_internal=search_internal,
                     during_analysis=True,
                 )
 
-        self.paths.save_search_internal(
-            obj=search_internal.results,
-        )
+        try:
+            os.remove(self.checkpoint_file)
+        except TypeError:
+            pass
 
         return search_internal
 
     def samples_info_from(self, search_internal=None):
         search_internal = search_internal or self.search_internal
 
         return {
             "log_evidence": np.max(search_internal.results.logz),
             "total_samples": int(np.sum(search_internal.results.ncall)),
+            "total_accepted_samples": len(search_internal.results.logl),
             "time": self.timer.time if self.timer else None,
             "number_live_points": self.number_live_points,
         }
 
     def samples_via_internal_from(self, model, search_internal=None):
         """
         Returns a `Samples` object from the dynesty internal results.
@@ -233,37 +236,33 @@
         """
         search_internal = search_internal or self.search_internal
 
         parameter_lists = search_internal.results.samples.tolist()
         log_prior_list = model.log_prior_list_from(parameter_lists=parameter_lists)
         log_likelihood_list = list(search_internal.results.logl)
 
-        try:
-            weight_list = list(
-                np.exp(
-                    np.asarray(search_internal.results.logwt)
-                    - search_internal.results.logz[-1]
-                )
+        weight_list = list(
+            np.exp(
+                np.asarray(search_internal.results.logwt)
+                - search_internal.results.logz[-1]
             )
-        except:
-            weight_list = search_internal.results["weights"]
+        )
 
         sample_list = Sample.from_lists(
             model=model,
             parameter_lists=parameter_lists,
             log_likelihood_list=log_likelihood_list,
             log_prior_list=log_prior_list,
             weight_list=weight_list,
         )
 
         return SamplesNest(
             model=model,
             sample_list=sample_list,
             samples_info=self.samples_info_from(search_internal=search_internal),
-            search_internal=search_internal,
         )
 
     @property
     def search_internal(self):
         raise NotImplementedError
 
     def iterations_from(
@@ -336,20 +335,23 @@
         config_dict_run = {
             key: value
             for key, value in self.config_dict_run.items()
             if key != "maxcall"
         }
 
         if iterations > 0:
-            search_internal.run_nested(
-                maxcall=iterations,
-                print_progress=not self.silence,
-                checkpoint_file=self.checkpoint_file,
-                **config_dict_run,
-            )
+            with warnings.catch_warnings():
+                warnings.simplefilter("ignore")
+
+                search_internal.run_nested(
+                    maxcall=iterations,
+                    print_progress=not self.silence,
+                    checkpoint_file=self.checkpoint_file,
+                    **config_dict_run,
+                )
 
         iterations_after_run = np.sum(search_internal.results.ncall)
 
         if isinstance(self.paths, NullPaths):
             return True
 
         return (
@@ -393,15 +395,32 @@
         If autofit is not outputting results to hard-disk (e.g. paths is `NullPaths`), this function is bypassed.
         """
         try:
             return str(self.paths.search_internal_path / "savestate.save")
         except TypeError:
             pass
 
-    def config_dict_with_test_mode_settings_from(self, config_dict):
+    def config_dict_test_mode_from(self, config_dict: Dict) -> Dict:
+        """
+        Returns a configuration dictionary for test mode meaning that the sampler terminates as quickly as possible.
+
+        Entries which set the total number of samples of the sampler (e.g. maximum calls, maximum likelihood
+        evaluations) are reduced to low values meaning it terminates nearly immediately.
+
+        Parameters
+        ----------
+        config_dict
+            The original configuration dictionary for this sampler which includes entries controlling how fast the
+            sampler terminates.
+
+        Returns
+        -------
+        A configuration dictionary where settings which control the sampler's number of samples are reduced so it
+        terminates as quickly as possible.
+        """
         return {
             **config_dict,
             "maxiter": 1,
             "maxcall": 1,
         }
 
     def live_points_init_from(self, model, fitness):
@@ -425,14 +444,16 @@
             unit_parameters,
             parameters,
             log_likelihood_list,
         ) = self.initializer.samples_from_model(
             total_points=self.number_live_points,
             model=model,
             fitness=fitness,
+            paths=self.paths,
+            n_cores=self.number_of_cores,
         )
 
         init_unit_parameters = np.zeros(
             shape=(self.number_live_points, model.prior_count)
         )
         init_parameters = np.zeros(shape=(self.number_live_points, model.prior_count))
         init_log_likelihood_list = np.zeros(shape=(self.number_live_points))
@@ -474,46 +495,10 @@
                 multiprocessing pool, whereas the run is now trying to use a multiprocessing pool.
 
                 This could indiciate the number of cores have change values or Python multiprocessing
                 has been disabled and then enabled.
                 """
             )
 
-    def remove_state_files(self):
-        try:
-            os.remove(self.checkpoint_file)
-        except TypeError:
-            pass
-
     @property
     def number_live_points(self):
         raise NotImplementedError()
-
-    def plot_results(self, samples):
-        from autofit.non_linear.search.nest.dynesty.plotter import DynestyPlotter
-
-        if not samples.pdf_converged:
-            return
-
-        def should_plot(name):
-            return conf.instance["visualize"]["plots_search"]["dynesty"][name]
-
-        plotter = DynestyPlotter(
-            samples=samples,
-            output=Output(path=self.paths.image_path / "search", format="png"),
-        )
-
-        if should_plot("cornerplot"):
-            plotter.cornerplot()
-
-        if should_plot("traceplot"):
-            plotter.traceplot()
-
-        # There is currently a bug internal in dynesty where the matplotlib figure produced after these plots
-        # is not closed, and has weird extra stuff on. I have commented these out for now, in the hope that dynesty
-        # fix this bug in the future.
-
-        # if should_plot("runplot"):
-        #     plotter.runplot()
-
-        # if should_plot("cornerpoints"):
-        #     plotter.cornerpoints()
```

### Comparing `autofit-2024.1.27.4/autofit/non_linear/search/nest/dynesty/search/dynamic.py` & `autofit-2024.5.16.0/autofit/non_linear/search/nest/dynesty/search/dynamic.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/non_linear/search/nest/dynesty/search/static.py` & `autofit-2024.5.16.0/autofit/non_linear/search/nest/dynesty/search/static.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     def __init__(self, function):
         self.function = function
 
     @cached_property
     def grad(self):
         import jax
         from jax import grad
-
         print("Compiling gradient")
         return jax.jit(grad(self.function))
 
     def __getstate__(self):
         return {"function": self.function}
 
     def __setstate__(self, state):
@@ -131,14 +130,15 @@
             An instance of the fitness class used to evaluate the likelihood of each model.
         pool
             A dynesty Pool object which performs likelihood evaluations over multiple CPUs.
         queue_size
             The number of CPU's over which multiprocessing is performed, determining how many samples are stored
             in the dynesty queue for samples.
         """
+
         if self.use_gradient:
             gradient = GradWrapper(fitness)
         else:
             gradient = None
 
         if checkpoint_exists:
             search_internal = StaticSampler.restore(
```

### Comparing `autofit-2024.1.27.4/autofit/non_linear/search/nest/nautilus/search.py` & `autofit-2024.5.16.0/autofit/non_linear/search/nest/nautilus/search.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import numpy as np
 import logging
 import os
 import sys
-from typing import Optional
+from typing import Dict, Optional, Tuple
 
 from autofit import jax_wrapper
 from autofit.database.sqlalchemy_ import sa
 
 from autoconf import conf
 from autofit.mapper.prior_model.abstract import AbstractPriorModel
 from autofit.non_linear.fitness import Fitness
 from autofit.non_linear.paths.null import NullPaths
 from autofit.non_linear.search.nest import abstract_nest
 from autofit.non_linear.samples.sample import Sample
 from autofit.non_linear.samples.nest import SamplesNest
-from autofit.plot.output import Output
 
 logger = logging.getLogger(__name__)
 
 
 def prior_transform(cube, model):
     return model.vector_from_unit_vector(unit_vector=cube, ignore_prior_limits=True)
 
@@ -111,14 +110,15 @@
         A result object comprising the Samples object that includes the maximum log likelihood instance and full
         set of accepted ssamples of the fit.
         """
 
         fitness = Fitness(
             model=model,
             analysis=analysis,
+            paths=self.paths,
             fom_is_log_likelihood=True,
             resample_figure_of_merit=-1.0e99,
         )
 
         if not isinstance(self.paths, NullPaths):
             checkpoint_exists = os.path.exists(self.checkpoint_file)
         else:
@@ -139,33 +139,32 @@
             or self.kwargs.get("force_x1_cpu")
             or jax_wrapper.use_jax
         ):
             search_internal = self.fit_x1_cpu(
                 fitness=fitness,
                 model=model,
                 analysis=analysis,
-                checkpoint_exists=checkpoint_exists,
             )
         else:
             if not self.using_mpi:
                 search_internal = self.fit_multiprocessing(
                     fitness=fitness,
                     model=model,
                     analysis=analysis,
-                    checkpoint_exists=checkpoint_exists,
                 )
             else:
                 search_internal = self.fit_mpi(
                     fitness=fitness,
                     model=model,
                     analysis=analysis,
                     checkpoint_exists=checkpoint_exists,
                 )
 
         if self.checkpoint_file is not None:
+
             os.remove(self.checkpoint_file)
 
         return search_internal
 
     @property
     def sampler_cls(self):
         try:
@@ -190,15 +189,15 @@
         If autofit is not outputting results to hard-disk (e.g. paths is `NullPaths`), this function is bypassed.
         """
         try:
             return self.paths.search_internal_path / "checkpoint.hdf5"
         except TypeError:
             pass
 
-    def fit_x1_cpu(self, fitness, model, analysis, checkpoint_exists: bool):
+    def fit_x1_cpu(self, fitness, model, analysis):
         """
         Perform the non-linear search, using one CPU core.
 
         This is used if the likelihood function calls external libraries that cannot be parallelized or use
         threading in a way that conflicts with the parallelization of the non-linear search.
 
         Parameters
@@ -207,16 +206,14 @@
             The function which takes a model instance and returns its log likelihood via the Analysis class
         model
             The model which maps parameters chosen via the non-linear search (e.g. via the priors or sampling) to
             instances of the model, which are passed to the fitness function.
         analysis
             Contains the data and the log likelihood function which fits an instance of the model to the data, returning
             the log likelihood the search maximizes.
-        checkpoint_exists
-            Does the checkpoint file corresponding do a previous run of this search exist?
         """
 
         self.logger.info(
             """
             Running search where parallelization is disabled.
             """
         )
@@ -227,33 +224,17 @@
             n_dim=model.prior_count,
             prior_kwargs={"model": model},
             filepath=self.checkpoint_file,
             pool=None,
             **self.config_dict_search,
         )
 
-        if checkpoint_exists:
-            self.output_sampler_results(search_internal=search_internal)
-
-            self.perform_update(
-                model=model,
-                analysis=analysis,
-                during_analysis=True,
-                search_internal=search_internal,
-            )
-
-        search_internal.run(
-            **self.config_dict_run,
-        )
-
-        self.output_sampler_results(search_internal=search_internal)
-
-        return search_internal
+        return self.call_search(search_internal=search_internal, model=model, analysis=analysis)
 
-    def fit_multiprocessing(self, fitness, model, analysis, checkpoint_exists: bool):
+    def fit_multiprocessing(self, fitness, model, analysis):
         """
         Perform the non-linear search, using multiple CPU cores parallelized via Python's multiprocessing module.
 
         This uses PyAutoFit's sneaky pool class, which allows us to use the multiprocessing module in a way that plays
         nicely with the non-linear search (e.g. exception handling, keyboard interupts, etc.).
 
         Multiprocessing parallelization can only parallelize across multiple cores on a single device, it cannot be
@@ -265,43 +246,87 @@
             The function which takes a model instance and returns its log likelihood via the Analysis class
         model
             The model which maps parameters chosen via the non-linear search (e.g. via the priors or sampling) to
             instances of the model, which are passed to the fitness function.
         analysis
             Contains the data and the log likelihood function which fits an instance of the model to the data, returning
             the log likelihood the search maximizes.
-        checkpoint_exists
-            Does the checkpoint file corresponding do a previous run of this search exist?
         """
 
         search_internal = self.sampler_cls(
             prior=prior_transform,
             likelihood=fitness.__call__,
             n_dim=model.prior_count,
             prior_kwargs={"model": model},
             filepath=self.checkpoint_file,
             pool=self.number_of_cores,
             **self.config_dict_search,
         )
 
-        if checkpoint_exists:
-            self.output_sampler_results(search_internal=search_internal)
+        return self.call_search(search_internal=search_internal, model=model, analysis=analysis)
 
-            self.perform_update(
-                model=model,
-                analysis=analysis,
-                during_analysis=True,
-                search_internal=search_internal,
+    def call_search(self, search_internal, model, analysis):
+        """
+        The x1 CPU and multiprocessing searches both call this function to perform the non-linear search.
+
+        This function calls the search a reduced number of times, corresponding to the `iterations_per_update` of the
+        search. This allows the search to output results on-the-fly, for example writing to the hard-disk the latest
+        model and samples.
+
+        It tracks how often to do this update alongside the maximum number of iterations the search will perform.
+        This ensures that on-the-fly output is performed at regular intervals and that the search does not perform more
+        iterations than the `n_like_max` input variable.
+
+        Parameters
+        ----------
+        search_internal
+            The single CPU or multiprocessing search which is run and performs nested sampling.
+        model
+            The model which maps parameters chosen via the non-linear search (e.g. via the priors or sampling) to
+            instances of the model, which are passed to the fitness function.
+        analysis
+            Contains the data and the log likelihood function which fits an instance of the model to the data, returning
+            the log likelihood the search maximizes.
+        """
+
+        finished = False
+
+        while not finished:
+
+            iterations, total_iterations = self.iterations_from(
+                search_internal=search_internal
             )
 
-        search_internal.run(
-            **self.config_dict_run,
-        )
+            config_dict_run = {
+                key: value
+                for key, value in self.config_dict_run.items()
+                if key != "n_like_max"
+            }
+
+            search_internal.run(
+                **config_dict_run,
+                n_like_max=iterations,
+            )
+
+            iterations_after_run = self.iterations_from(search_internal=search_internal)[1]
+
+            if (
+                    total_iterations == iterations_after_run
+                    or iterations_after_run == self.config_dict_run["n_like_max"]
+            ):
+                finished = True
+
+            if not finished:
 
-        self.output_sampler_results(search_internal=search_internal)
+                self.perform_update(
+                    model=model,
+                    analysis=analysis,
+                    during_analysis=True,
+                    search_internal=search_internal
+                )
 
         return search_internal
 
     def fit_mpi(self, fitness, model, analysis, checkpoint_exists: bool):
         """
         Perform the non-linear search, using MPI to distribute the model-fit across multiple computing nodes.
 
@@ -340,80 +365,103 @@
                 filepath=self.checkpoint_file,
                 pool=pool,
                 **self.config_dict_search,
             )
 
             if checkpoint_exists:
                 if self.is_master:
-                    self.output_sampler_results(search_internal=search_internal)
 
                     self.perform_update(
                         model=model,
                         analysis=analysis,
                         during_analysis=True,
                         search_internal=search_internal,
                     )
 
             search_internal.run(
                 **self.config_dict_run,
             )
 
-            self.output_sampler_results(search_internal=search_internal)
-
         return search_internal
 
-    def output_sampler_results(self, search_internal):
+    def iterations_from(
+        self, search_internal
+    ) -> Tuple[int, int]:
         """
-        Output the sampler results to hard-disk in a generalized PyAutoFit format.
+        Returns the next number of iterations that a dynesty call will use and the total number of iterations
+        that have been performed so far.
+
+        This is used so that the `iterations_per_update` input leads to on-the-fly output of dynesty results.
 
-        The results in this format are loaded by other functions in order to create a `Samples` object, perform updates
-        which visualize the results and write the results to the hard-disk as an output of the model-fit.
+        It also ensures dynesty does not perform more samples than the `n_like_max` input variable.
+
+        Parameters
+        ----------
+        search_internal
+            The Dynesty sampler (static or dynamic) which is run and performs nested sampling.
+
+        Returns
+        -------
+        The next number of iterations that a dynesty run sampling will perform and the total number of iterations
+        it has performed so far.
+        """
+
+        if isinstance(self.paths, NullPaths):
+            n_like_max = self.config_dict_run.get("n_like_max")
+
+            if n_like_max is not None:
+                return n_like_max, n_like_max
+            return int(1e99), int(1e99)
+
+        try:
+            total_iterations = len(search_internal.posterior()[1])
+        except ValueError:
+            total_iterations = 0
+
+        iterations = total_iterations + self.iterations_per_update
+
+        if self.config_dict_run["n_like_max"] is not None:
+            if iterations > self.config_dict_run["n_like_max"]:
+                iterations = self.config_dict_run["n_like_max"]
+
+        return iterations, total_iterations
+
+    def output_search_internal(self, search_internal):
+        """
+        Output the sampler results to hard-disk in their internal format.
+
+        The multiprocessing `Pool` object cannot be pickled and thus the sampler cannot be saved to hard-disk. This
+        function therefore extracts the necessary information from the sampler and saves it to hard-disk.
 
         Parameters
         ----------
         sampler
             The nautilus sampler object containing the results of the model-fit.
         """
 
-        parameters, log_weights, log_likelihoods = search_internal.posterior()
+        pool_l = search_internal.pool_l
+        pool_s = search_internal.pool_s
 
-        parameter_lists = parameters.tolist()
-        log_likelihood_list = log_likelihoods.tolist()
-        weight_list = np.exp(log_weights).tolist()
-
-        search_internal = {
-            "parameter_lists": parameter_lists,
-            "log_likelihood_list": log_likelihood_list,
-            "weight_list": weight_list,
-            "log_evidence": search_internal.evidence(),
-            "total_samples": int(search_internal.n_like),
-            "time": self.timer.time if self.timer else None,
-            "number_live_points": int(search_internal.n_live),
-        }
+        search_internal.pool_l = None
+        search_internal.pool_s = None
 
         self.paths.save_search_internal(
             obj=search_internal,
         )
 
-    def samples_info_from(self, search_internal=None):
-        search_internal_dict = search_internal or self.paths.load_search_internal()
-
-        if search_internal is not None:
-            return {
-                "log_evidence": search_internal.evidence(),
-                "total_samples": int(search_internal.n_like),
-                "time": self.timer.time if self.timer else None,
-                "number_live_points": int(search_internal.n_live),
-            }
+        search_internal.pool_l = pool_l
+        search_internal.pool_s = pool_s
 
+    def samples_info_from(self, search_internal=None):
         return {
-            "log_evidence": search_internal_dict["log_evidence"],
-            "total_samples": search_internal_dict["total_samples"],
+            "log_evidence": search_internal.evidence(),
+            "total_samples": int(search_internal.n_like),
+            "total_accepted_samples": int(search_internal.n_like),
             "time": self.timer.time if self.timer else None,
-            "number_live_points": search_internal_dict["number_live_points"],
+            "number_live_points": int(search_internal.n_live),
         }
 
     def samples_via_internal_from(
         self, model: AbstractPriorModel, search_internal=None
     ):
         """
         Returns a `Samples` object from the ultranest internal results.
@@ -426,27 +474,22 @@
 
         Parameters
         ----------
         model
             Maps input vectors of unit parameter values to physical values and model instances via priors.
         """
 
-        if search_internal is not None:
-            parameters, log_weights, log_likelihoods = search_internal.posterior()
+        if search_internal is None:
+            search_internal = self.paths.load_search_internal()
 
-            parameter_lists = parameters.tolist()
-            log_likelihood_list = log_likelihoods.tolist()
-            weight_list = np.exp(log_weights).tolist()
-
-        else:
-            search_internal_dict = self.paths.load_search_internal()
+        parameters, log_weights, log_likelihoods = search_internal.posterior()
 
-            parameter_lists = search_internal_dict["parameter_lists"]
-            log_likelihood_list = search_internal_dict["log_likelihood_list"]
-            weight_list = search_internal_dict["weight_list"]
+        parameter_lists = parameters.tolist()
+        log_likelihood_list = log_likelihoods.tolist()
+        weight_list = np.exp(log_weights).tolist()
 
         log_prior_list = [
             sum(model.log_prior_list_from_vector(vector=vector))
             for vector in parameter_lists
         ]
 
         sample_list = Sample.from_lists(
@@ -457,49 +500,35 @@
             weight_list=weight_list,
         )
 
         return SamplesNest(
             model=model,
             sample_list=sample_list,
             samples_info=self.samples_info_from(search_internal=search_internal),
-            search_internal=None,
         )
 
     @property
     def config_dict(self):
         return conf.instance["non_linear"]["nest"][self.__class__.__name__]
 
-    def config_dict_with_test_mode_settings_from(self, config_dict):
-        return {
-            **config_dict,
-            "max_iters": 1,
-            "max_ncalls": 1,
-        }
-
-    def plot_results(self, samples):
-        from autofit.non_linear.search.nest.nautilus.plotter import NautilusPlotter
-
-        if not samples.pdf_converged:
-            return
+    def config_dict_test_mode_from(self, config_dict : Dict) -> Dict:
+        """
+        Returns a configuration dictionary for test mode meaning that the sampler terminates as quickly as possible.
 
-        def should_plot(name):
-            return conf.instance["visualize"]["plots_search"]["nautilus"][name]
+        Entries which set the total number of samples of the sampler (e.g. maximum calls, maximum likelihood
+        evaluations) are reduced to low values meaning it terminates nearly immediately.
 
-        plotter = NautilusPlotter(
-            samples=samples,
-            output=Output(path=self.paths.image_path / "search", format="png"),
-        )
+        Parameters
+        ----------
+        config_dict
+            The original configuration dictionary for this sampler which includes entries controlling how fast the
+            sampler terminates.
 
-        if should_plot("cornerplot"):
-            plotter.cornerplot(
-                panelsize=3.5,
-                yticksize=16,
-                xticksize=16,
-                bins=20,
-                plot_datapoints=False,
-                plot_density=False,
-                fill_contours=True,
-                levels=(0.68, 0.95),
-                labelpad=0.02,
-                range=np.ones(samples.model.total_free_parameters) * 0.999,
-                label_kwargs={"fontsize": 24},
-            )
+        Returns
+        -------
+        A configuration dictionary where settings which control the sampler's number of samples are reduced so it
+        terminates as quickly as possible.
+        """
+        return {
+            **config_dict,
+            "n_like_max": 1,
+        }
```

### Comparing `autofit-2024.1.27.4/autofit/non_linear/search/nest/ultranest/plotter.py` & `autofit-2024.5.16.0/autofit/non_linear/plot/samples_plotters.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,97 +1,127 @@
+import matplotlib.pyplot as plt
+import numpy as np
 from functools import wraps
-from autofit.plot import SamplesPlotter
+import logging
+import os
 
-from autofit.plot.samples_plotters import skip_plot_in_test_mode
+from autoconf import conf
 
-def log_value_error(func):
+from autofit.non_linear.plot.output import Output
 
-    @wraps(func)
-    def wrapper(self, *args, **kwargs):
-        """
-        Prevent an exception terminating the run if visualization fails due to convergence not yet being reached.
+logger = logging.getLogger(__name__)
 
-        Searches attempt to perform visualization every `iterations_per_update`, however these visualization calls
-        may occur before the search has converged on enough of parameter to successfully perform visualization.
+def skip_plot_in_test_mode(func):
+    """
+    Skips visualization plots of non-linear searches if test mode is on.
 
-        This can lead the search to raise an exception which terminates the Python script, when we instead
-        want the code to continue running, to continue the search and perform visualization on a subsequent iteration
-        once convergence has been achieved.
+    Parameters
+    ----------
+    func
+        A function which plots a result of a non-linear search.
 
-        This wrapper catches these exceptions, logs them so the user can see visualization failed and then
-        continues the code without raising an exception in a way that terminates the script.
+    Returns
+    -------
+        A function that plots a visual, or None if test mode is on.
+    """
 
-        This wrapper is specific to UltraNest, which raises a `KeyError` when visualization is performed before
-        convergence has been achieved.
+    @wraps(func)
+    def wrapper(
+        *args,
+        **kwargs
+    ):
+        """
+        Skips visualization plots of non-linear searches if test mode is on.
 
         Parameters
         ----------
-        self
-            An instance of a `SearchPlotter` class.
-        args
-            The arguments used to perform a visualization of the search.
-        kwargs
-            The keyword arguments used to perform a visualization of the search.
-        """
-        try:
-            return func(self, *args, **kwargs)
-        except (KeyError, AssertionError):
-            self.log_plot_exception(func.__name__)
+        obj
+            An plotter object which performs visualization of a non-linear search.
 
-    return wrapper
+        Returns
+        -------
+            A function that plots a visual, or None if test mode is on.
+        """
 
-class UltraNestPlotter(SamplesPlotter):
+        if os.environ.get("PYAUTOFIT_TEST_MODE") == "1":
+            return
 
-    @skip_plot_in_test_mode
-    @log_value_error
-    def cornerplot(self, **kwargs):
-        """
-        Plots the in-built ``ultranest`` plot ``cornerplot``.
+        return func(*args, **kwargs)
 
-        This figure plots a corner plot of the 1-D and 2-D marginalized posteriors.
-        """
+    return wrapper
 
-        from ultranest import plot
 
-        plot.cornerplot(
-            results=self.samples.search_internal,
-            **kwargs
-        )
 
-        self.output.to_figure(structure=None, auto_filename="cornerplot")
-        self.close()
+class SamplesPlotter:
+    def __init__(
+            self, 
+            samples,
+            output : Output = Output()
+    ):
+
+        self.samples = samples
+        self.output = output
+
+    @property
+    def model(self):
+        return self.samples.model
+
+    @property
+    def log_posterior_list(self):
+        return self.samples.log_posterior_list
+
+    def close(self):
+        if plt.fignum_exists(num=1):
+            plt.close()
+
+    def log_plot_exception(self, plot_name : str):
+        """
+        Plotting the results of a ``dynesty`` model-fit before they have converged on an
+        accurate estimate of the posterior can lead the ``dynesty`` plotting routines
+        to raise a ``ValueError``.
 
-    @skip_plot_in_test_mode
-    @log_value_error
-    def runplot(self, **kwargs):
-        """
-        Plots the in-built ``ultranest`` plot ``runplot``.
+        This exception is caught in each of the plotting methods below, and this
+        function is used to log the behaviour.
 
-        This figure plots live points, ln(likelihood), ln(weight), and ln(evidence) vs. ln(prior volume).
+        Parameters
+        ----------
+        plot_name
+            The name of the ``dynesty`` plot which raised a ``ValueError``
         """
-        from ultranest import plot
 
-        plot.runplot(
-            results=self.samples.search_internal,
-            **kwargs
+        logger.info(
+            f"""{self.__class__.__name__} unable to produce {plot_name} visual: posterior estimate therefore
+            not yet sufficient for this model-fit is not yet robust enough to do this. 
+            Visuals should be produced in later update, once posterior estimate is updated.
+            """
         )
 
-        self.output.to_figure(structure=None, auto_filename="runplot")
-        self.close()
-
-    @skip_plot_in_test_mode
-    @log_value_error
-    def traceplot(self, **kwargs):
+    def corner_cornerpy(self, **kwargs):
         """
-        Plots the in-built ``ultranest`` plot ``traceplot``.
+        Plots a corner plot via the visualization library `corner.py`.
 
-        This figure plots traces and marginalized posteriors for each parameter.
+        This plots a corner plot including the 1-D and 2-D marginalized posteriors.
         """
-        from ultranest import plot
 
-        plot.traceplot(
-            results=self.samples.search_internal,
-            **kwargs
+        if os.environ.get("PYAUTOFIT_TEST_MODE") == "1":
+            return
+
+        import matplotlib.pylab as pylab
+
+        config_dict = conf.instance["visualize"]["plots_settings"]["corner_cornerpy"]
+
+        params = {'font.size' : int(config_dict["fontsize"])}
+        pylab.rcParams.update(params)
+
+        import corner
+
+        corner.corner(
+            data=np.asarray(self.samples.parameter_lists),
+            weight_list=self.samples.weight_list,
+            labels=self.model.parameter_labels_with_superscripts_latex,
         )
 
-        self.output.to_figure(structure=None, auto_filename="traceplot")
-        self.close()
+        self.output.to_figure(auto_filename="corner")
+        self.close()
+
+
+
```

### Comparing `autofit-2024.1.27.4/autofit/non_linear/search/nest/ultranest/search.py` & `autofit-2024.5.16.0/autofit/non_linear/search/nest/ultranest/search.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 import os
-from typing import Optional
+from typing import Dict, Optional
 
 from autofit.database.sqlalchemy_ import sa
 
-from autoconf import conf
 from autofit.mapper.prior_model.abstract import AbstractPriorModel
 from autofit.non_linear.search.nest import abstract_nest
 from autofit.non_linear.fitness import Fitness
 from autofit.non_linear.samples.sample import Sample
 from autofit.non_linear.samples.nest import SamplesNest
-from autofit.plot import UltraNestPlotter
-from autofit.plot.output import Output
 
 class UltraNest(abstract_nest.AbstractNest):
     __identifier_fields__ = (
         "draw_multiple",
         "ndraw_min",
         "ndraw_max",
         "min_num_live_points",
@@ -116,14 +113,15 @@
                 "Install it via the command `pip install ultranest==3.6.2`.\n\n"
                 "----------------------"
             )
 
         fitness = Fitness(
             model=model,
             analysis=analysis,
+            paths=self.paths,
             fom_is_log_likelihood=True,
             resample_figure_of_merit=-1.0e99
         )
 
         def prior_transform(cube):
             return model.vector_from_unit_vector(
                 unit_vector=cube,
@@ -206,21 +204,38 @@
                     analysis=analysis,
                     during_analysis=True,
                     search_internal=search_internal
                 )
 
         return search_internal
 
+    def output_search_internal(self, search_internal):
+        """
+        Output the sampler results to hard-disk in their internal format.
+
+        UltraNest uses a backend to store and load results, therefore the outputting of the search internal to a
+        dill file is disabled.
+
+        However, a dictionary of the search results is output to dill above.
+
+        Parameters
+        ----------
+        sampler
+            The nautilus sampler object containing the results of the model-fit.
+        """
+        pass
+
     def samples_info_from(self, search_internal=None):
 
         search_internal = search_internal or self.paths.load_search_internal()
 
         return {
             "log_evidence": search_internal["logz"],
             "total_samples": search_internal["ncall"],
+            "total_accepted_samples": len(search_internal["weighted_samples"]["logl"]),
             "time": self.timer.time if self.timer else None,
             "number_live_points": self.config_dict_run["min_num_live_points"]
         }
 
     def samples_via_internal_from(self, model: AbstractPriorModel, search_internal=None):
         """
         Returns a `Samples` object from the ultranest internal results.
@@ -254,19 +269,34 @@
             weight_list=weight_list
         )
 
         return SamplesNest(
             model=model,
             sample_list=sample_list,
             samples_info=self.samples_info_from(search_internal=search_internal),
-            search_internal=search_internal,
         )
 
-    def config_dict_with_test_mode_settings_from(self, config_dict):
+    def config_dict_test_mode_from(self, config_dict: Dict) -> Dict:
+        """
+        Returns a configuration dictionary for test mode meaning that the sampler terminates as quickly as possible.
+
+        Entries which set the total number of samples of the sampler (e.g. maximum calls, maximum likelihood
+        evaluations) are reduced to low values meaning it terminates nearly immediately.
+
+        Parameters
+        ----------
+        config_dict
+            The original configuration dictionary for this sampler which includes entries controlling how fast the
+            sampler terminates.
 
+        Returns
+        -------
+        A configuration dictionary where settings which control the sampler's number of samples are reduced so it
+        terminates as quickly as possible.
+        """
         return {
             **config_dict,
             "max_iters": 1,
             "max_ncalls": 1,
         }
 
     @property
@@ -301,30 +331,8 @@
             config_dict_stepsampler.pop("scale")
             return stepsampler.AHARMSampler(**config_dict_stepsampler)
         elif stepsampler_cls == "CubeMHSampler":
             return stepsampler.CubeMHSampler(**config_dict_stepsampler)
         elif stepsampler_cls == "CubeSliceSampler":
             return stepsampler.CubeSliceSampler(**config_dict_stepsampler)
         elif stepsampler_cls == "RegionSliceSampler":
-            return stepsampler.RegionSliceSampler(**config_dict_stepsampler)
-
-    def plot_results(self, samples):
-
-        if not samples.pdf_converged:
-            return
-
-        def should_plot(name):
-            return conf.instance["visualize"]["plots_search"]["ultranest"][name]
-
-        plotter = UltraNestPlotter(
-            samples=samples,
-            output=Output(self.paths.image_path / "search", format="png")
-        )
-
-        if should_plot("cornerplot"):
-            plotter.cornerplot()
-
-        if should_plot("runplot"):
-            plotter.runplot()
-
-        if should_plot("traceplot"):
-            plotter.traceplot()
+            return stepsampler.RegionSliceSampler(**config_dict_stepsampler)
```

### Comparing `autofit-2024.1.27.4/autofit/non_linear/search/optimize/drawer/search.py` & `autofit-2024.5.16.0/autofit/non_linear/search/optimize/drawer/search.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 import numpy as np
 from typing import Optional
 
 from autofit.database.sqlalchemy_ import sa
 
-from autoconf import conf
 from autofit.mapper.prior_model.abstract import AbstractPriorModel
 from autofit.non_linear.fitness import Fitness
 from autofit.non_linear.search.optimize.abstract_optimize import AbstractOptimizer
 from autofit.non_linear.initializer import AbstractInitializer
-from autofit.non_linear.search.optimize.drawer.plotter import DrawerPlotter
 from autofit.non_linear.samples import Samples, Sample
-from autofit.plot.output import Output
 
 
 class Drawer(AbstractOptimizer):
     __identifier_fields__ = ("total_draws",)
 
     def __init__(
         self,
@@ -99,17 +96,18 @@
         A result object comprising the Samples object that inclues the maximum log likelihood instance and full
         chains used by the fit.
         """
 
         fitness = Fitness(
             model=model,
             analysis=analysis,
+            paths=self.paths,
             fom_is_log_likelihood=False,
             resample_figure_of_merit=-np.inf,
-            convert_to_chi_squared=False
+            convert_to_chi_squared=False,
         )
 
         total_draws = self.config_dict_search["total_draws"]
 
         self.logger.info(
             f"Performing DrawerSearch for a total of {total_draws} points."
         )
@@ -118,44 +116,42 @@
             unit_parameter_lists,
             parameter_lists,
             log_posterior_list,
         ) = self.initializer.samples_from_model(
             total_points=self.config_dict_search["total_draws"],
             model=model,
             fitness=fitness,
+            paths=self.paths,
+            n_cores=self.number_of_cores,
         )
 
         search_internal = {
-            "parameter_lists" : parameter_lists,
-            "log_posterior_list" : log_posterior_list,
-            "time": self.timer.time
+            "parameter_lists": parameter_lists,
+            "log_posterior_list": log_posterior_list,
+            "time": self.timer.time,
         }
 
         self.paths.save_search_internal(
             obj=search_internal,
         )
 
         self.logger.info("Drawer complete")
 
     def samples_from(self, model, search_internal):
-
         search_internal_dict = self.paths.load_search_internal()
 
         parameter_lists = search_internal_dict["parameter_lists"]
         log_posterior_list = search_internal_dict["log_posterior_list"]
 
         log_prior_list = [
             sum(model.log_prior_list_from_vector(vector=vector))
             for vector in parameter_lists
         ]
         log_likelihood_list = [
-            lp - prior
-            for lp, prior in zip(
-                log_posterior_list, log_prior_list
-            )
+            lp - prior for lp, prior in zip(log_posterior_list, log_prior_list)
         ]
 
         weight_list = len(log_likelihood_list) * [1.0]
 
         sample_list = Sample.from_lists(
             model=model,
             parameter_lists=parameter_lists,
@@ -165,22 +161,7 @@
         )
 
         return Samples(
             model=model,
             sample_list=sample_list,
             samples_info=search_internal_dict,
         )
-
-    def plot_results(
-        self,
-        samples,
-        during_analysis : bool = False,
-    ):
-        def should_plot(name):
-            return conf.instance["visualize"]["plots_search"]["drawer"][name]
-
-        plotter = DrawerPlotter(
-            samples=samples,
-            output=Output(
-                path=self.paths.image_path / "search", format="png"
-            ),
-        )
```

### Comparing `autofit-2024.1.27.4/autofit/non_linear/search/optimize/lbfgs/search.py` & `autofit-2024.5.16.0/autofit/non_linear/search/optimize/lbfgs/search.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 import copy
 from scipy import optimize
 import numpy as np
 
 
 class LBFGS(AbstractOptimizer):
-
     __identifier_fields__ = ()
 
     def __init__(
         self,
         name: Optional[str] = None,
         path_prefix: Optional[str] = None,
         unique_tag: Optional[str] = None,
@@ -67,15 +66,14 @@
             **kwargs
         )
 
         self.logger.debug("Creating LBFGS Search")
 
     @cached_property
     def config_dict_options(self):
-
         config_dict = copy.deepcopy(self._class_config["options"])
 
         for key, value in config_dict.items():
             try:
                 config_dict[key] = self.kwargs[key]
             except KeyError:
                 pass
@@ -103,101 +101,99 @@
         -------
         A result object comprising the Samples object that inclues the maximum log likelihood instance and full
         chains used by the fit.
         """
         fitness = Fitness(
             model=model,
             analysis=analysis,
+            paths=self.paths,
             fom_is_log_likelihood=False,
             resample_figure_of_merit=-np.inf,
-            convert_to_chi_squared=True
+            convert_to_chi_squared=True,
         )
 
         try:
-
             search_internal_dict = self.paths.load_search_internal()
 
             x0 = search_internal_dict["x0"]
             total_iterations = search_internal_dict["total_iterations"]
 
             self.logger.info(
                 "Resuming LBFGS non-linear search (previous samples found)."
             )
 
         except (FileNotFoundError, TypeError):
-
             (
                 unit_parameter_lists,
                 parameter_lists,
                 log_posterior_list,
             ) = self.initializer.samples_from_model(
-                total_points=1, model=model, fitness=fitness,
+                total_points=1,
+                model=model,
+                fitness=fitness,
+                paths=self.paths,
+                n_cores=self.number_of_cores,
             )
 
             x0 = np.asarray(parameter_lists[0])
 
             total_iterations = 0
 
             self.logger.info(
                 "Starting new LBFGS non-linear search (no previous samples found)."
             )
 
         maxiter = self.config_dict_options.get("maxiter", 1e8)
 
         while total_iterations < maxiter:
-
             iterations_remaining = maxiter - total_iterations
 
             iterations = min(self.iterations_per_update, iterations_remaining)
 
             if iterations > 0:
-
                 config_dict_options = self.config_dict_options
                 config_dict_options["maxiter"] = iterations
 
                 search_internal = optimize.minimize(
                     fun=fitness.__call__,
                     x0=x0,
                     method="L-BFGS-B",
                     options=config_dict_options,
                     **self.config_dict_search
                 )
 
-
                 total_iterations += search_internal.nit
 
-                search_internal_dict = {
-                    "total_iterations": total_iterations,
-                    "log_posterior_list": -0.5 * fitness(parameters=search_internal.x),
-                    "x0": search_internal.x,
-                }
-
-                search_internal.log_posterior_list = search_internal_dict["log_posterior_list"]
+                search_internal.log_posterior_list = -0.5 * fitness(
+                    parameters=search_internal.x
+                )
 
                 self.paths.save_search_internal(
-                    obj=search_internal_dict,
+                    obj=search_internal,
                 )
 
                 x0 = search_internal.x
 
                 if search_internal.nit < iterations:
                     return search_internal
 
                 self.perform_update(
                     model=model,
                     analysis=analysis,
                     during_analysis=True,
-                    search_internal=search_internal
+                    search_internal=search_internal,
                 )
 
         self.logger.info("L-BFGS sampling complete.")
 
         return search_internal
 
-    def samples_via_internal_from(self, model: AbstractPriorModel, search_internal=None):
+    def samples_via_internal_from(
+        self, model: AbstractPriorModel, search_internal=None
+    ):
         """
         Returns a `Samples` object from the LBFGS internal results.
 
         The samples contain all information on the parameter space sampling (e.g. the parameters,
         log likelihoods, etc.).
 
         The internal search results are converted from the native format used by the search to lists of values
@@ -205,50 +201,40 @@
 
         Parameters
         ----------
         model
             Maps input vectors of unit parameter values to physical values and model instances via priors.
         """
 
-        if search_internal is not None:
-
-            x0 = search_internal.x
-            total_iterations = search_internal.nit
-            log_posterior_list = np.array([search_internal.log_posterior_list])
-
-        else:
-
-            search_internal_dict = self.paths.load_search_internal()
+        if search_internal is None:
+            search_internal = self.paths.load_search_internal()
 
-            x0 = search_internal_dict["x0"]
-            total_iterations = search_internal_dict["total_iterations"]
-            log_posterior_list = np.array([search_internal_dict["log_posterior_list"]])
+        x0 = search_internal.x
+        total_iterations = search_internal.nit
+        log_posterior_list = np.array([search_internal.log_posterior_list])
 
         parameter_lists = [list(x0)]
         log_prior_list = model.log_prior_list_from(parameter_lists=parameter_lists)
 
         log_likelihood_list = [
-            lp - prior
-            for lp, prior
-            in zip(log_posterior_list, log_prior_list)
+            lp - prior for lp, prior in zip(log_posterior_list, log_prior_list)
         ]
         weight_list = len(log_likelihood_list) * [1.0]
 
         sample_list = Sample.from_lists(
             model=model,
             parameter_lists=parameter_lists,
             log_likelihood_list=log_likelihood_list,
             log_prior_list=log_prior_list,
-            weight_list=weight_list
+            weight_list=weight_list,
         )
 
         samples_info = {
             "total_iterations": total_iterations,
             "time": self.timer.time if self.timer else None,
         }
 
         return Samples(
             model=model,
             sample_list=sample_list,
             samples_info=samples_info,
-            search_internal=x0,
-        )
+        )
```

### Comparing `autofit-2024.1.27.4/autofit/non_linear/search/optimize/pyswarms/search/abstract.py` & `autofit-2024.5.16.0/autofit/non_linear/search/optimize/pyswarms/search/abstract.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,22 @@
-from os import path
-from typing import Optional
+from typing import Dict, Optional
 
 import numpy as np
 
-from autoconf import conf
 from autofit import exc
 from autofit.database.sqlalchemy_ import sa
 from autofit.mapper.prior_model.abstract import AbstractPriorModel
 from autofit.non_linear.fitness import Fitness
 from autofit.non_linear.initializer import AbstractInitializer
 from autofit.non_linear.search.optimize.abstract_optimize import AbstractOptimizer
 from autofit.non_linear.samples.sample import Sample
 from autofit.non_linear.samples.samples import Samples
-from autofit.plot import PySwarmsPlotter
-from autofit.plot.output import Output
 
 
 class FitnessPySwarms(Fitness):
-
     def __call__(self, parameters, *kwargs):
         """
         Interfaces with any non-linear in order to fit a model to the data and return a log likelihood via
         an `Analysis` class.
 
         The interface is described in full in the `__init__` docstring.
 
@@ -46,44 +41,46 @@
 
         if isinstance(parameters[0], float):
             parameters = [parameters]
 
         figure_of_merit_list = []
 
         for params_of_particle in parameters:
-
             try:
                 instance = self.model.instance_from_vector(vector=params_of_particle)
-                log_likelihood = self.analysis.log_likelihood_function(instance=instance)
-                log_prior = self.model.log_prior_list_from_vector(vector=params_of_particle)
+                log_likelihood = self.analysis.log_likelihood_function(
+                    instance=instance
+                )
+                log_prior = self.model.log_prior_list_from_vector(
+                    vector=params_of_particle
+                )
                 log_posterior = log_likelihood + sum(log_prior)
                 figure_of_merit = -2.0 * log_posterior
             except exc.FitException:
                 figure_of_merit = np.nan
 
             if np.isnan(figure_of_merit):
                 figure_of_merit = -2.0 * self.resample_figure_of_merit
 
             figure_of_merit_list.append(figure_of_merit)
 
         return np.asarray(figure_of_merit_list)
 
 
-
 class AbstractPySwarms(AbstractOptimizer):
     def __init__(
-            self,
-            name: Optional[str] = None,
-            path_prefix: Optional[str] = None,
-            unique_tag: Optional[str] = None,
-            initializer: Optional[AbstractInitializer] = None,
-            iterations_per_update: int = None,
-            number_of_cores: int = None,
-            session: Optional[sa.orm.Session] = None,
-            **kwargs
+        self,
+        name: Optional[str] = None,
+        path_prefix: Optional[str] = None,
+        unique_tag: Optional[str] = None,
+        initializer: Optional[AbstractInitializer] = None,
+        iterations_per_update: int = None,
+        number_of_cores: int = None,
+        session: Optional[sa.orm.Session] = None,
+        **kwargs
     ):
         """
         A PySwarms Particle Swarm Optimizer global non-linear search.
 
         For a full description of PySwarms, checkout its Github and readthedocs webpages:
 
         https://github.com/ljvmiranda921/pyswarms
@@ -145,101 +142,92 @@
         """
 
         fitness = FitnessPySwarms(
             model=model,
             analysis=analysis,
             fom_is_log_likelihood=False,
             resample_figure_of_merit=-np.inf,
-            convert_to_chi_squared=True
+            convert_to_chi_squared=True,
         )
 
         try:
+            search_internal = self.paths.load_search_internal()
 
-            search_internal_dict = self.paths.load_search_internal()
-
-            search_internal = search_internal_dict["pos_history"]
-
-            init_pos = search_internal[-1]
-            total_iterations = search_internal_dict["total_iterations"]
+            init_pos = search_internal.pos_history[-1]
+            total_iterations = len(search_internal.cost_history)
 
             self.logger.info(
                 "Resuming PySwarms non-linear search (previous samples found)."
             )
 
-        except (FileNotFoundError, TypeError):
-
-            unit_parameter_lists, parameter_lists, log_posterior_list = self.initializer.samples_from_model(
+        except (FileNotFoundError, TypeError, AttributeError):
+            (
+                unit_parameter_lists,
+                parameter_lists,
+                log_posterior_list,
+            ) = self.initializer.samples_from_model(
                 total_points=self.config_dict_search["n_particles"],
                 model=model,
                 fitness=fitness,
+                paths=self.paths,
+                n_cores=self.number_of_cores,
             )
 
-            init_pos = np.zeros(shape=(self.config_dict_search["n_particles"], model.prior_count))
+            init_pos = np.zeros(
+                shape=(self.config_dict_search["n_particles"], model.prior_count)
+            )
 
             for index, parameters in enumerate(parameter_lists):
-
                 init_pos[index, :] = np.asarray(parameters)
 
             total_iterations = 0
 
             self.logger.info(
                 "Starting new PySwarms non-linear search (no previous samples found)."
             )
 
         ## TODO : Use actual limits
 
         vector_lower = model.vector_from_unit_vector(
-            unit_vector=[1e-6] * model.prior_count,
-            ignore_prior_limits=True
+            unit_vector=[1e-6] * model.prior_count, ignore_prior_limits=True
         )
         vector_upper = model.vector_from_unit_vector(
-            unit_vector=[0.9999999] * model.prior_count,
-            ignore_prior_limits=True
+            unit_vector=[0.9999999] * model.prior_count, ignore_prior_limits=True
         )
 
         lower_bounds = [lower for lower in vector_lower]
         upper_bounds = [upper for upper in vector_upper]
 
         bounds = (np.asarray(lower_bounds), np.asarray(upper_bounds))
 
         while total_iterations < self.config_dict_run["iters"]:
-
             search_internal = self.search_internal_from(
-                model=model,
-                fitness=fitness,
-                bounds=bounds,
-                init_pos=init_pos
+                model=model, fitness=fitness, bounds=bounds, init_pos=init_pos
             )
 
             iterations_remaining = self.config_dict_run["iters"] - total_iterations
 
             iterations = min(self.iterations_per_update, iterations_remaining)
 
             if iterations > 0:
-
-                search_internal.optimize(objective_func=fitness.__call__, iters=iterations)
+                search_internal.optimize(
+                    objective_func=fitness.__call__, iters=iterations
+                )
 
                 total_iterations += iterations
 
-                search_internal_dict = {
-                    "pos_history" : search_internal.pos_history,
-                    "total_iterations": total_iterations,
-                    "log_posterior_list": [-0.5 * cost for cost in search_internal.cost_history],
-                    "time": self.timer.time if self.timer else None,
-                }
-
                 self.paths.save_search_internal(
-                    obj=search_internal_dict,
+                    obj=search_internal,
                 )
 
                 self.perform_update(
                     model=model,
                     analysis=analysis,
                     during_analysis=True,
-                    search_internal=search_internal
+                    search_internal=search_internal,
                 )
 
                 init_pos = search_internal.pos_history[-1]
 
         return search_internal
 
     def samples_via_internal_from(self, model, search_internal=None):
@@ -254,85 +242,70 @@
 
         Parameters
         ----------
         model
             Maps input vectors of unit parameter values to physical values and model instances via priors.
         """
 
-        if search_internal is not None:
-
-            search_internal_dict = {
-                "total_iterations": None,
-                "log_posterior_list": [-0.5 * cost for cost in search_internal.cost_history],
-                "time": self.timer.time if self.timer else None,
-            }
-            pos_history = search_internal.pos_history
-
-
+        if search_internal is None:
+            search_internal = self.paths.load_search_internal()
 
-        else:
-
-            search_internal_dict = self.paths.load_search_internal()
-            pos_history = search_internal_dict["pos_history"]
-
-            search_internal_dict = {
-                "total_iterations": search_internal_dict["total_iterations"],
-                "log_posterior_list": search_internal_dict["log_posterior_list"],
-                "time": search_internal_dict["time"]
-            }
+        search_internal_dict = {
+            "total_iterations": None,
+            "log_posterior_list": [
+                -0.5 * cost for cost in search_internal.cost_history
+            ],
+            "time": self.timer.time if self.timer else None,
+        }
+        pos_history = search_internal.pos_history
 
         parameter_lists = [
             param.tolist() for parameters in pos_history for param in parameters
         ]
         parameter_lists_2 = [parameters.tolist()[0] for parameters in pos_history]
 
         log_posterior_list = search_internal_dict["log_posterior_list"]
         log_prior_list = model.log_prior_list_from(parameter_lists=parameter_lists)
-        log_likelihood_list = [lp - prior for lp, prior in zip(log_posterior_list, log_prior_list)]
+        log_likelihood_list = [
+            lp - prior for lp, prior in zip(log_posterior_list, log_prior_list)
+        ]
         weight_list = len(log_likelihood_list) * [1.0]
 
         sample_list = Sample.from_lists(
             model=model,
             parameter_lists=parameter_lists_2,
             log_likelihood_list=log_likelihood_list,
             log_prior_list=log_prior_list,
-            weight_list=weight_list
+            weight_list=weight_list,
         )
 
         return Samples(
             model=model,
             sample_list=sample_list,
             samples_info=search_internal_dict,
-            search_internal=pos_history
         )
 
-    def config_dict_with_test_mode_settings_from(self, config_dict):
+    def config_dict_test_mode_from(self, config_dict: Dict) -> Dict:
+        """
+        Returns a configuration dictionary for test mode meaning that the sampler terminates as quickly as possible.
+
+        Entries which set the total number of samples of the sampler (e.g. maximum calls, maximum likelihood
+        evaluations) are reduced to low values meaning it terminates nearly immediately.
 
+        Parameters
+        ----------
+        config_dict
+            The original configuration dictionary for this sampler which includes entries controlling how fast the
+            sampler terminates.
+
+        Returns
+        -------
+        A configuration dictionary where settings which control the sampler's number of samples are reduced so it
+        terminates as quickly as possible.
+        """
         return {
             **config_dict,
             "iters": 1,
         }
 
     def search_internal_from(self, model, fitness, bounds, init_pos):
         raise NotImplementedError()
-
-    def plot_results(self, samples):
-
-        def should_plot(name):
-            return conf.instance["visualize"]["plots_search"]["pyswarms"][name]
-
-        plotter = PySwarmsPlotter(
-            samples=samples,
-            output=Output(path=self.paths.image_path / "search", format="png")
-        )
-
-        if should_plot("contour"):
-            plotter.contour()
-
-        if should_plot("cost_history"):
-            plotter.cost_history()
-
-        if should_plot("trajectories"):
-            plotter.trajectories()
-
-        if should_plot("time_series"):
-            plotter.time_series()
```

### Comparing `autofit-2024.1.27.4/autofit/non_linear/search/optimize/pyswarms/search/globe.py` & `autofit-2024.5.16.0/autofit/non_linear/search/optimize/pyswarms/search/globe.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/non_linear/search/optimize/pyswarms/search/local.py` & `autofit-2024.5.16.0/autofit/non_linear/search/optimize/pyswarms/search/local.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/non_linear/settings.py` & `autofit-2024.5.16.0/autofit/non_linear/settings.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/non_linear/timer.py` & `autofit-2024.5.16.0/autofit/non_linear/timer.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/plot/output.py` & `autofit-2024.5.16.0/autofit/non_linear/plot/output.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import matplotlib
 from pathlib import Path
+from os import path
 from typing import List, Optional, Union
 
 from autoconf import conf
 
 
 def set_backend():
     backend = conf.get_matplotlib_backend()
@@ -75,50 +76,67 @@
     def format_list(self):
         if not isinstance(self.format, list):
             return [self.format]
         return self.format
 
     def to_figure(
         self,
-        structure,
         auto_filename: Optional[str] = None,
     ):
         """
         Output the figure, by either displaying it on the user's screen or to the hard-disk as a .png or .fits file.
 
         Parameters
         ----------
         structure
             The 2D array of image to be output, required for outputting the image as a fits file.
         """
 
         filename = auto_filename if self.filename is None else self.filename
 
         for format in self.format_list:
+            if os.environ.get("PYAUTOARRAY_OUTPUT_MODE") == "1":
+                return self.to_figure_output_mode(filename=filename)
             if not self.bypass:
                 if format == "show":
                     plt.show()
                 elif format == "png":
                     plt.savefig(self.path / f"{filename}.png")
                 elif format == "pdf":
                     plt.savefig(self.path / f"{filename}.pdf")
-                elif format == "fits":
-                    if structure is not None:
-                        structure.output_to_fits(
-                            file_path=self.path / f"{filename}.fits",
-                            overwrite=True,
-                        )
 
     def subplot_to_figure(self, auto_filename=None):
         """
         Output a subplot figure, either as an image on the screen or to the hard-disk as a png or fits file.
         """
 
         filename = auto_filename if self.filename is None else self.filename
 
         for format in self.format_list:
+            if os.environ.get("PYAUTOARRAY_OUTPUT_MODE") == "1":
+                return self.to_figure_output_mode(filename=filename)
             if format == "show":
                 plt.show()
             elif format == "png":
                 plt.savefig(self.path / f"{filename}.png")
             elif format == "pdf":
                 plt.savefig(self.path / f"{filename}.pdf")
+
+
+    def to_figure_output_mode(self, filename: str):
+        global COUNT
+
+        try:
+            COUNT += 1
+        except NameError:
+            COUNT = 0
+
+        import sys
+
+        script_name = path.split(sys.argv[0])[-1].replace(".py", "")
+
+        output_path = path.join(os.getcwd(), "output_mode", script_name)
+        os.makedirs(output_path, exist_ok=True)
+
+        plt.savefig(
+            path.join(output_path, f"{COUNT}_{filename}.png"),
+        )
```

### Comparing `autofit-2024.1.27.4/autofit/text/formatter.py` & `autofit-2024.5.16.0/autofit/text/formatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,34 @@
 
     def __len__(self):
         return len(self._dict)
 
     def items(self):
         return self._dict.items()
 
+    def list(self, indent=4, line_length=90):
+        lines = []
+        for key, value in self.items():
+            indent_string = indent * " "
+            if value.value is not None:
+                value_string = str(value.value)
+                space_string = max((line_length - len(str(key))), 1) * " "
+                lines.append(f"{key}{space_string}{value_string}")
+
+            if len(value) > 0:
+                sub_lines = value.list(
+                    indent=indent,
+                    line_length=line_length - indent,
+                )
+                if value.value is None:
+                    lines.append(key)
+                for line in sub_lines:
+                    lines.append(f"{indent_string}{line}")
+        return lines
+
 
 class TextFormatter:
     def __init__(self, line_length=90, indent=4):
         self.dict = FormatNode()
         self.line_length = line_length
         self.indent = indent
 
@@ -38,40 +58,24 @@
             node.value = value
         else:
             self.add_to_dict(path[1:], value, node)
 
     def add(self, path: Tuple[str, ...], value):
         self.add_to_dict(path, value, self.dict)
 
-    def dict_to_list(self, info_dict, line_length):
-        lines = []
-        for key, value in info_dict.items():
-            indent_string = self.indent * " "
-            if value.value is not None:
-                value_string = str(value.value)
-                space_string = max((line_length - len(str(key))), 1) * " "
-                lines.append(f"{key}{space_string}{value_string}")
-
-            if len(value) > 0:
-                sub_lines = self.dict_to_list(
-                    value, line_length=line_length - self.indent
-                )
-                if value.value is None:
-                    lines.append(key)
-                for line in sub_lines:
-                    lines.append(f"{indent_string}{line}")
-        return lines
-
     @property
-    def list(self):
-        return self.dict_to_list(self.dict, line_length=self.line_length)
+    def text(self):
+        return "\n".join(map(str, self.list))
 
     @property
-    def text(self):
-        return "\n".join(self.list)
+    def list(self):
+        return self.dict.list(
+            indent=self.indent,
+            line_length=self.line_length,
+        )
 
 
 def format_string_for_parameter_name(parameter_name: str) -> str:
     """
     Get the format for the label. Attempts to extract the key string associated with
     the dimension. Seems dodgy.
```

### Comparing `autofit-2024.1.27.4/autofit/text/samples_text.py` & `autofit-2024.5.16.0/autofit/text/samples_text.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import logging
 
+from autofit.mapper.prior_model.representative import find_groups
 from autofit.text import formatter as frm
 
 logger = logging.getLogger(__name__)
 
-def values_from_samples(samples, median_pdf_model):
 
+def values_from_samples(samples, median_pdf_model):
     if median_pdf_model:
         return samples.median_pdf(as_instance=False)
     return samples.max_log_likelihood(as_instance=False)
 
 
 def summary(
     samples, sigma=3.0, median_pdf_model=True, indent=1, line_length=None
@@ -18,74 +19,81 @@
     Create a string summarizing the results of the `NonLinearSearch` at an input sigma value.
 
     This function is used for creating the model.results files of a non-linear search.
 
     Parameters
     ----------
     sigma
-        The sigma within which the PDF is used to estimate errors (e.g. sigma = 1.0 uses 0.6826 of the PDF)."""
+        The sigma within which the PDF is used to estimate errors (e.g. sigma = 1.0 uses 0.6826 of the PDF).
+    """
 
     values = values_from_samples(samples=samples, median_pdf_model=median_pdf_model)
     values_at_sigma = samples.values_at_sigma(sigma=sigma, as_instance=False)
 
     parameter_names = samples.model.parameter_names
 
     if line_length is None:
         line_length = len(max(parameter_names, key=len)) + 8
 
     sigma_formatter = frm.TextFormatter(indent=indent, line_length=line_length)
 
-    for i, prior_path in enumerate(samples.model.unique_prior_paths):
+    prior_result_map = {}
 
-        value_result = frm.value_result_string_from(
+    for i, (_, prior) in enumerate(samples.model.unique_path_prior_tuples):
+        prior_result_map[prior] = frm.value_result_string_from(
             parameter_name=parameter_names[i],
             value=values[i],
             values_at_sigma=values_at_sigma[i],
         )
 
-        sigma_formatter.add(prior_path, value_result)
+    paths = []
+    for path, prior in samples.model.path_priors_tuples:
+        paths.append((path, prior_result_map[prior]))
+
+    for path, value in find_groups(paths):
+        sigma_formatter.add(path, value)
 
     return f"\n\nSummary ({sigma} sigma limits):\n\n{sigma_formatter.text}"
 
 
 def latex(
-        samples,
-        median_pdf_model=True,
-        sigma=3.0,
-        name_to_label=True,
-        include_name=True,
-        include_quickmath=False,
-        prefix="",
-        suffix=""
+    samples,
+    median_pdf_model=True,
+    sigma=3.0,
+    name_to_label=True,
+    include_name=True,
+    include_quickmath=False,
+    prefix="",
+    suffix="",
 ) -> str:
     """
     Create a string summarizing the results of the `NonLinearSearch` at an input sigma value.
 
     This function is used for creating the model.results files of a non-linear search.
 
     Parameters
     ----------
     sigma
-        The sigma within which the PDF is used to estimate errors (e.g. sigma = 1.0 uses 0.6826 of the PDF)."""
+        The sigma within which the PDF is used to estimate errors (e.g. sigma = 1.0 uses 0.6826 of the PDF).
+    """
 
     values = values_from_samples(samples=samples, median_pdf_model=median_pdf_model)
     errors_at_sigma = samples.errors_at_sigma(sigma=sigma, as_instance=False)
 
     table = []
 
     for i in range(samples.model.prior_count):
-
         label_value = frm.parameter_result_latex_from(
             parameter_name=samples.model.parameter_names[i],
             value=values[i],
             errors=errors_at_sigma[i],
             superscript=samples.model.superscripts[i],
             name_to_label=name_to_label,
             include_name=include_name,
-            include_quickmath=include_quickmath
+            include_quickmath=include_quickmath,
         )
 
         table.append(f"{label_value}")
 
     table = "".join(table)[:-3]
 
     return f"{prefix}{table}{suffix}"
```

### Comparing `autofit-2024.1.27.4/autofit/text/text_util.py` & `autofit-2024.5.16.0/autofit/text/text_util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import datetime as dt
 
 from autoconf import conf
+from autofit.mapper.prior_model.representative import find_groups
 from autofit.text import formatter as frm, samples_text
 from autofit.tools.util import info_whitespace
 
 
 def padding(item, target=6):
     string = str(item)
     difference = target - len(string)
@@ -51,19 +52,26 @@
 
     results += ["Maximum Log Likelihood Model:\n\n"]
 
     formatter = frm.TextFormatter(line_length=info_whitespace())
 
     max_log_likelihood_sample = samples.max_log_likelihood(as_instance=False)
 
-    for prior_path, value in zip(
-        samples.model.unique_prior_paths,
+    paths = []
+
+    model = samples.model
+    for (_, prior), value in zip(
+        model.unique_path_prior_tuples,
         max_log_likelihood_sample,
     ):
-        formatter.add(prior_path, format_str().format(value))
+        for path in model.all_paths_for_prior(prior):
+            paths.append((path, value))
+
+    for path, value in find_groups(paths):
+        formatter.add(path, format_str().format(value))
     results += [formatter.text + "\n"]
 
     if hasattr(samples, "pdf_converged"):
         if samples.pdf_converged:
             results += samples_text.summary(
                 samples=samples, sigma=3.0, indent=4, line_length=info_whitespace()
             )
@@ -81,16 +89,16 @@
                 samples=samples, sigma=1.0, indent=4, line_length=info_whitespace()
             )
 
         results += ["\n\ninstances\n"]
 
     formatter = frm.TextFormatter(line_length=info_whitespace())
 
-    for t in samples.model.path_float_tuples:
-        formatter.add(*t)
+    for path, value in find_groups(samples.model.path_float_tuples):
+        formatter.add(path, value)
 
     results += ["\n" + formatter.text]
 
     return "".join(results)
 
 
 def search_summary_from_samples(samples) -> [str]:
@@ -108,18 +116,18 @@
 
 def search_summary_to_file(samples, log_likelihood_function_time, filename):
     summary = search_summary_from_samples(samples=samples)
     summary.append(
         f"Log Likelihood Function Evaluation Time (seconds) = {log_likelihood_function_time}\n"
     )
 
-    expected_time = dt.timedelta(seconds=float(samples.total_samples * log_likelihood_function_time))
-    summary.append(
-        f"Expected Time To Run (seconds) = {expected_time}\n"
+    expected_time = dt.timedelta(
+        seconds=float(samples.total_samples * log_likelihood_function_time)
     )
+    summary.append(f"Expected Time To Run (seconds) = {expected_time}\n")
 
     try:
         speed_up_factor = float(expected_time.total_seconds()) / float(samples.time)
         summary.append(
             f"Speed Up Factor (e.g. due to parallelization) = {speed_up_factor}"
         )
     except TypeError:
```

### Comparing `autofit-2024.1.27.4/autofit/tools/add_notebook_quotes.py` & `autofit-2024.5.16.0/autofit/tools/add_notebook_quotes.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/autofit/tools/util.py` & `autofit-2024.5.16.0/autofit/tools/util.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/scripts/update_identifiers.py` & `autofit-2024.5.16.0/scripts/update_identifiers.py`

 * *Files identical despite different names*

### Comparing `autofit-2024.1.27.4/setup.py` & `autofit-2024.5.16.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 this_dir = abspath(dirname(__file__))
 with open(join(this_dir, "README.rst"), encoding="utf-8") as file:
     long_description = file.read()
 
 with open(join(this_dir, "requirements.txt")) as f:
     requirements = f.read().split("\n")
 
-version = environ.get("VERSION", "1.0.dev0")
+version = environ.get("VERSION", "2024.5.16.0")
 requirements.extend([
     f'autoconf=={version}'
 ])
 
 
 def config_packages(directory):
     paths = [directory.replace("/", ".")]
```

