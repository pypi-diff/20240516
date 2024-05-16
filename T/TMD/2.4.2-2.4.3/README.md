# Comparing `tmp/TMD-2.4.2.tar.gz` & `tmp/tmd-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TMD-2.4.2.tar", last modified: Mon Feb 19 12:46:09 2024, max compression
+gzip compressed data, was "tmd-2.4.3.tar", last modified: Thu May 16 12:12:37 2024, max compression
```

## Comparing `TMD-2.4.2.tar` & `tmd-2.4.3.tar`

### file list

```diff
@@ -1,158 +1,158 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:46:09.955516 TMD-2.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-02-19 12:45:57.000000 TMD-2.4.2/.auto-changelog
--rw-r--r--   0 runner    (1001) docker     (127)    11016 2024-02-19 12:45:57.000000 TMD-2.4.2/.auto-changelog-template.hbs
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 12:45:57.000000 TMD-2.4.2/.codespellignorelines
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-19 12:45:57.000000 TMD-2.4.2/.codespellrc
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-02-19 12:45:57.000000 TMD-2.4.2/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-02-19 12:45:57.000000 TMD-2.4.2/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-19 12:45:57.000000 TMD-2.4.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:46:09.935516 TMD-2.4.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:46:09.935516 TMD-2.4.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-02-19 12:45:57.000000 TMD-2.4.2/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-19 12:45:57.000000 TMD-2.4.2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-02-19 12:45:57.000000 TMD-2.4.2/.github/ISSUE_TEMPLATE/feature_request.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-02-19 12:45:57.000000 TMD-2.4.2/.github/ISSUE_TEMPLATE/how_to_use.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-02-19 12:45:57.000000 TMD-2.4.2/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-02-19 12:45:57.000000 TMD-2.4.2/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:46:09.935516 TMD-2.4.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-02-19 12:45:57.000000 TMD-2.4.2/.github/workflows/commitlint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-02-19 12:45:57.000000 TMD-2.4.2/.github/workflows/publish-sdist.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-02-19 12:45:57.000000 TMD-2.4.2/.github/workflows/run-tox.yml
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-02-19 12:45:57.000000 TMD-2.4.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-02-19 12:45:57.000000 TMD-2.4.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-02-19 12:45:57.000000 TMD-2.4.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-02-19 12:45:57.000000 TMD-2.4.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-02-19 12:45:57.000000 TMD-2.4.2/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)    17858 2024-02-19 12:45:57.000000 TMD-2.4.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-02-19 12:45:57.000000 TMD-2.4.2/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-02-19 12:45:57.000000 TMD-2.4.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-02-19 12:45:57.000000 TMD-2.4.2/COPYRIGHT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-02-19 12:45:57.000000 TMD-2.4.2/LICENSE-BSD.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-02-19 12:45:57.000000 TMD-2.4.2/LICENSE-LGPL.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-19 12:45:57.000000 TMD-2.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-02-19 12:46:09.955516 TMD-2.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-02-19 12:45:57.000000 TMD-2.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:46:09.955516 TMD-2.4.2/TMD.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-02-19 12:46:09.000000 TMD-2.4.2/TMD.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-02-19 12:46:09.000000 TMD-2.4.2/TMD.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 12:46:09.000000 TMD-2.4.2/TMD.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-02-19 12:46:09.000000 TMD-2.4.2/TMD.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-19 12:46:09.000000 TMD-2.4.2/TMD.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-19 12:45:57.000000 TMD-2.4.2/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-02-19 12:45:57.000000 TMD-2.4.2/commitlint.config.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:46:09.935516 TMD-2.4.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-02-19 12:45:57.000000 TMD-2.4.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:46:09.939516 TMD-2.4.2/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-02-19 12:45:57.000000 TMD-2.4.2/docs/source/api_ref.rst
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-19 12:45:57.000000 TMD-2.4.2/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-02-19 12:45:57.000000 TMD-2.4.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-19 12:45:57.000000 TMD-2.4.2/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-19 12:45:57.000000 TMD-2.4.2/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:46:09.939516 TMD-2.4.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:46:09.939516 TMD-2.4.2/examples/Advanced/
--rw-r--r--   0 runner    (1001) docker     (127)    34098 2024-02-19 12:45:57.000000 TMD-2.4.2/examples/Advanced/advanced_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     6980 2024-02-19 12:45:57.000000 TMD-2.4.2/examples/Advanced/classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-02-19 12:45:57.000000 TMD-2.4.2/examples/Advanced/diversity_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-02-19 12:45:57.000000 TMD-2.4.2/examples/Advanced/matching.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-02-19 12:45:57.000000 TMD-2.4.2/examples/Advanced/polar_plot_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-02-19 12:45:57.000000 TMD-2.4.2/examples/Advanced/time_series_tmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    20425 2024-02-19 12:45:57.000000 TMD-2.4.2/examples/Advanced/variability.py
--rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-02-19 12:45:57.000000 TMD-2.4.2/examples/classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-02-19 12:45:57.000000 TMD-2.4.2/examples/distances_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-02-19 12:45:57.000000 TMD-2.4.2/examples/extract_ph.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-02-19 12:45:57.000000 TMD-2.4.2/examples/write_swc.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-02-19 12:45:57.000000 TMD-2.4.2/package.json
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-02-19 12:45:57.000000 TMD-2.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 12:46:09.955516 TMD-2.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-02-19 12:45:57.000000 TMD-2.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:46:09.943516 TMD-2.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:46:09.947517 TMD-2.4.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/data/basic.swc
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/data/basic_exotic_section_types.swc
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/data/basic_no_comments.swc
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/data/basic_no_sec_ids.swc
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/data/basic_options.swc
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/data/neuron.swc
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/data/neuron_ph_1.txt
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/data/neuron_ph_2.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/data/sample.swc
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/data/sample_disordered.swc
--rw-r--r--   0 runner    (1001) docker     (127)     4140 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/data/sample_disordered_v1.h5
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/data/sample_ph_0.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/data/sample_ph_1.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/data/sample_v0.h5
--rw-r--r--   0 runner    (1001) docker     (127)     4140 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/data/sample_v1.h5
--rw-r--r--   0 runner    (1001) docker     (127)     7264 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/data/sample_v2.h5
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/data/test_morph.swc
--rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/data/test_morph_v1.h5
--rw-r--r--   0 runner    (1001) docker     (127)     8552 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/data/test_morph_v2.h5
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:46:09.947517 TMD-2.4.2/tests/data/upper_case_names/
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/data/upper_case_names/Sample1.ASC
--rw-r--r--   0 runner    (1001) docker     (127)    12224 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/data/upper_case_names/Sample1.H5
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/data/upper_case_names/Sample1.SWC
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/data/upper_case_names/Sample2.AsC
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/data/upper_case_names/Sample2.SwC
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:46:09.947517 TMD-2.4.2/tests/data/valid/
--rw-r--r--   0 runner    (1001) docker     (127)    48864 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/data/valid/C010398B-P2.CNG.swc
--rwxr-xr-x   0 runner    (1001) docker     (127)    33168 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/data/valid/C010398B-P2.h5
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/data/valid/sample.swc
--rw-r--r--   0 runner    (1001) docker     (127)     4140 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/data/valid/sample_v1.h5
--rw-r--r--   0 runner    (1001) docker     (127)     7264 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/data/valid/sample_v2.h5
--rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/test_h5.py
--rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/test_neuron.py
--rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/test_neuron_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/test_neuron_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/test_population.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/test_soma.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/test_soma_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/test_swc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8090 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/test_topology_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/test_topology_distances.py
--rw-r--r--   0 runner    (1001) docker     (127)    11018 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/test_topology_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/test_topology_persistent_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/test_topology_vectorizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/test_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     8124 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/test_tree_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-02-19 12:45:57.000000 TMD-2.4.2/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:46:09.947517 TMD-2.4.2/tmd/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:46:09.947517 TMD-2.4.2/tmd/Neuron/
--rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-02-19 12:45:57.000000 TMD-2.4.2/tmd/Neuron/Neuron.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-02-19 12:45:57.000000 TMD-2.4.2/tmd/Neuron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-02-19 12:45:57.000000 TMD-2.4.2/tmd/Neuron/methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:46:09.947517 TMD-2.4.2/tmd/Population/
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-02-19 12:45:57.000000 TMD-2.4.2/tmd/Population/Population.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-02-19 12:45:57.000000 TMD-2.4.2/tmd/Population/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:46:09.951516 TMD-2.4.2/tmd/Soma/
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-02-19 12:45:57.000000 TMD-2.4.2/tmd/Soma/Soma.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-02-19 12:45:57.000000 TMD-2.4.2/tmd/Soma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-02-19 12:45:57.000000 TMD-2.4.2/tmd/Soma/methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:46:09.951516 TMD-2.4.2/tmd/Topology/
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-02-19 12:45:57.000000 TMD-2.4.2/tmd/Topology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11239 2024-02-19 12:45:57.000000 TMD-2.4.2/tmd/Topology/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-02-19 12:45:57.000000 TMD-2.4.2/tmd/Topology/distances.py
--rw-r--r--   0 runner    (1001) docker     (127)     6805 2024-02-19 12:45:57.000000 TMD-2.4.2/tmd/Topology/methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     6595 2024-02-19 12:45:57.000000 TMD-2.4.2/tmd/Topology/persistent_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-02-19 12:45:57.000000 TMD-2.4.2/tmd/Topology/statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-02-19 12:45:57.000000 TMD-2.4.2/tmd/Topology/transformations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-02-19 12:45:57.000000 TMD-2.4.2/tmd/Topology/vectorizations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:46:09.951516 TMD-2.4.2/tmd/Tree/
--rw-r--r--   0 runner    (1001) docker     (127)     6210 2024-02-19 12:45:57.000000 TMD-2.4.2/tmd/Tree/Tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-02-19 12:45:57.000000 TMD-2.4.2/tmd/Tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10254 2024-02-19 12:45:57.000000 TMD-2.4.2/tmd/Tree/methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-02-19 12:45:57.000000 TMD-2.4.2/tmd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:46:09.951516 TMD-2.4.2/tmd/io/
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-02-19 12:45:57.000000 TMD-2.4.2/tmd/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-02-19 12:45:57.000000 TMD-2.4.2/tmd/io/conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     6323 2024-02-19 12:45:57.000000 TMD-2.4.2/tmd/io/h5.py
--rw-r--r--   0 runner    (1001) docker     (127)     7515 2024-02-19 12:45:57.000000 TMD-2.4.2/tmd/io/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     4688 2024-02-19 12:45:57.000000 TMD-2.4.2/tmd/io/swc.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-02-19 12:45:57.000000 TMD-2.4.2/tmd/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:46:09.951516 TMD-2.4.2/tmd/view/
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-02-19 12:45:57.000000 TMD-2.4.2/tmd/view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22487 2024-02-19 12:45:57.000000 TMD-2.4.2/tmd/view/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    11723 2024-02-19 12:45:57.000000 TMD-2.4.2/tmd/view/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    40938 2024-02-19 12:45:57.000000 TMD-2.4.2/tmd/view/view.py
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-02-19 12:45:57.000000 TMD-2.4.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:12:37.738665 tmd-2.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-16 12:12:32.000000 tmd-2.4.3/.auto-changelog
+-rw-r--r--   0 runner    (1001) docker     (127)    11016 2024-05-16 12:12:32.000000 tmd-2.4.3/.auto-changelog-template.hbs
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:12:32.000000 tmd-2.4.3/.codespellignorelines
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-16 12:12:32.000000 tmd-2.4.3/.codespellrc
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-16 12:12:32.000000 tmd-2.4.3/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-16 12:12:32.000000 tmd-2.4.3/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-16 12:12:32.000000 tmd-2.4.3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:12:37.718666 tmd-2.4.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:12:37.718666 tmd-2.4.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-05-16 12:12:32.000000 tmd-2.4.3/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-16 12:12:32.000000 tmd-2.4.3/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-16 12:12:32.000000 tmd-2.4.3/.github/ISSUE_TEMPLATE/feature_request.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-05-16 12:12:32.000000 tmd-2.4.3/.github/ISSUE_TEMPLATE/how_to_use.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-16 12:12:32.000000 tmd-2.4.3/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-16 12:12:32.000000 tmd-2.4.3/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:12:37.718666 tmd-2.4.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-16 12:12:32.000000 tmd-2.4.3/.github/workflows/commitlint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-16 12:12:32.000000 tmd-2.4.3/.github/workflows/publish-sdist.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-05-16 12:12:32.000000 tmd-2.4.3/.github/workflows/run-tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-16 12:12:32.000000 tmd-2.4.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-16 12:12:32.000000 tmd-2.4.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-16 12:12:32.000000 tmd-2.4.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-16 12:12:32.000000 tmd-2.4.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-16 12:12:32.000000 tmd-2.4.3/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)    17858 2024-05-16 12:12:32.000000 tmd-2.4.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-05-16 12:12:32.000000 tmd-2.4.3/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-16 12:12:32.000000 tmd-2.4.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-16 12:12:32.000000 tmd-2.4.3/COPYRIGHT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-16 12:12:32.000000 tmd-2.4.3/LICENSE-BSD.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-16 12:12:32.000000 tmd-2.4.3/LICENSE-LGPL.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-16 12:12:32.000000 tmd-2.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-05-16 12:12:37.738665 tmd-2.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-05-16 12:12:32.000000 tmd-2.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:12:37.734665 tmd-2.4.3/TMD.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-05-16 12:12:37.000000 tmd-2.4.3/TMD.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-05-16 12:12:37.000000 tmd-2.4.3/TMD.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 12:12:37.000000 tmd-2.4.3/TMD.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-16 12:12:37.000000 tmd-2.4.3/TMD.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-16 12:12:37.000000 tmd-2.4.3/TMD.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-16 12:12:32.000000 tmd-2.4.3/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-16 12:12:32.000000 tmd-2.4.3/commitlint.config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:12:37.718666 tmd-2.4.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-16 12:12:32.000000 tmd-2.4.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:12:37.718666 tmd-2.4.3/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-16 12:12:32.000000 tmd-2.4.3/docs/source/api_ref.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-16 12:12:32.000000 tmd-2.4.3/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-05-16 12:12:32.000000 tmd-2.4.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-16 12:12:32.000000 tmd-2.4.3/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-16 12:12:32.000000 tmd-2.4.3/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:12:37.722666 tmd-2.4.3/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:12:37.722666 tmd-2.4.3/examples/Advanced/
+-rw-r--r--   0 runner    (1001) docker     (127)    34098 2024-05-16 12:12:32.000000 tmd-2.4.3/examples/Advanced/advanced_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6980 2024-05-16 12:12:32.000000 tmd-2.4.3/examples/Advanced/classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-05-16 12:12:32.000000 tmd-2.4.3/examples/Advanced/diversity_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-05-16 12:12:32.000000 tmd-2.4.3/examples/Advanced/matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-16 12:12:32.000000 tmd-2.4.3/examples/Advanced/polar_plot_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-05-16 12:12:32.000000 tmd-2.4.3/examples/Advanced/time_series_tmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20425 2024-05-16 12:12:32.000000 tmd-2.4.3/examples/Advanced/variability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-05-16 12:12:32.000000 tmd-2.4.3/examples/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-16 12:12:32.000000 tmd-2.4.3/examples/distances_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-16 12:12:32.000000 tmd-2.4.3/examples/extract_ph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-16 12:12:32.000000 tmd-2.4.3/examples/write_swc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-16 12:12:32.000000 tmd-2.4.3/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-16 12:12:32.000000 tmd-2.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 12:12:37.738665 tmd-2.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-16 12:12:32.000000 tmd-2.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:12:37.726666 tmd-2.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:12:37.726666 tmd-2.4.3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/data/basic.swc
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/data/basic_exotic_section_types.swc
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/data/basic_no_comments.swc
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/data/basic_no_sec_ids.swc
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/data/basic_options.swc
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/data/neuron.swc
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/data/neuron_ph_1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/data/neuron_ph_2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/data/sample.swc
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/data/sample_disordered.swc
+-rw-r--r--   0 runner    (1001) docker     (127)     4140 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/data/sample_disordered_v1.h5
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/data/sample_ph_0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/data/sample_ph_1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/data/sample_v0.h5
+-rw-r--r--   0 runner    (1001) docker     (127)     4140 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/data/sample_v1.h5
+-rw-r--r--   0 runner    (1001) docker     (127)     7264 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/data/sample_v2.h5
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/data/test_morph.swc
+-rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/data/test_morph_v1.h5
+-rw-r--r--   0 runner    (1001) docker     (127)     8552 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/data/test_morph_v2.h5
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:12:37.730666 tmd-2.4.3/tests/data/upper_case_names/
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/data/upper_case_names/Sample1.ASC
+-rw-r--r--   0 runner    (1001) docker     (127)    12224 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/data/upper_case_names/Sample1.H5
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/data/upper_case_names/Sample1.SWC
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/data/upper_case_names/Sample2.AsC
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/data/upper_case_names/Sample2.SwC
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:12:37.730666 tmd-2.4.3/tests/data/valid/
+-rw-r--r--   0 runner    (1001) docker     (127)    48864 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/data/valid/C010398B-P2.CNG.swc
+-rwxr-xr-x   0 runner    (1001) docker     (127)    33168 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/data/valid/C010398B-P2.h5
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/data/valid/sample.swc
+-rw-r--r--   0 runner    (1001) docker     (127)     4140 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/data/valid/sample_v1.h5
+-rw-r--r--   0 runner    (1001) docker     (127)     7264 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/data/valid/sample_v2.h5
+-rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/test_neuron.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/test_neuron_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/test_neuron_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/test_population.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/test_soma.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/test_soma_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/test_swc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8090 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/test_topology_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/test_topology_distances.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11018 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/test_topology_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/test_topology_persistent_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/test_topology_vectorizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/test_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8124 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/test_tree_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-16 12:12:32.000000 tmd-2.4.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:12:37.730666 tmd-2.4.3/tmd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:12:37.730666 tmd-2.4.3/tmd/Neuron/
+-rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-05-16 12:12:32.000000 tmd-2.4.3/tmd/Neuron/Neuron.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-16 12:12:32.000000 tmd-2.4.3/tmd/Neuron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-16 12:12:32.000000 tmd-2.4.3/tmd/Neuron/methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:12:37.730666 tmd-2.4.3/tmd/Population/
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-05-16 12:12:32.000000 tmd-2.4.3/tmd/Population/Population.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-16 12:12:32.000000 tmd-2.4.3/tmd/Population/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:12:37.730666 tmd-2.4.3/tmd/Soma/
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-16 12:12:32.000000 tmd-2.4.3/tmd/Soma/Soma.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-16 12:12:32.000000 tmd-2.4.3/tmd/Soma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-16 12:12:32.000000 tmd-2.4.3/tmd/Soma/methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:12:37.734665 tmd-2.4.3/tmd/Topology/
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-16 12:12:32.000000 tmd-2.4.3/tmd/Topology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-05-16 12:12:32.000000 tmd-2.4.3/tmd/Topology/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-16 12:12:32.000000 tmd-2.4.3/tmd/Topology/distances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-05-16 12:12:32.000000 tmd-2.4.3/tmd/Topology/methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6595 2024-05-16 12:12:32.000000 tmd-2.4.3/tmd/Topology/persistent_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-05-16 12:12:32.000000 tmd-2.4.3/tmd/Topology/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-16 12:12:32.000000 tmd-2.4.3/tmd/Topology/transformations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-16 12:12:32.000000 tmd-2.4.3/tmd/Topology/vectorizations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:12:37.734665 tmd-2.4.3/tmd/Tree/
+-rw-r--r--   0 runner    (1001) docker     (127)     6210 2024-05-16 12:12:32.000000 tmd-2.4.3/tmd/Tree/Tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-16 12:12:32.000000 tmd-2.4.3/tmd/Tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10254 2024-05-16 12:12:32.000000 tmd-2.4.3/tmd/Tree/methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-16 12:12:32.000000 tmd-2.4.3/tmd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:12:37.734665 tmd-2.4.3/tmd/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-16 12:12:32.000000 tmd-2.4.3/tmd/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-05-16 12:12:32.000000 tmd-2.4.3/tmd/io/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6323 2024-05-16 12:12:32.000000 tmd-2.4.3/tmd/io/h5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7515 2024-05-16 12:12:32.000000 tmd-2.4.3/tmd/io/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4688 2024-05-16 12:12:32.000000 tmd-2.4.3/tmd/io/swc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-16 12:12:32.000000 tmd-2.4.3/tmd/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:12:37.734665 tmd-2.4.3/tmd/view/
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-16 12:12:32.000000 tmd-2.4.3/tmd/view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22478 2024-05-16 12:12:32.000000 tmd-2.4.3/tmd/view/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11723 2024-05-16 12:12:32.000000 tmd-2.4.3/tmd/view/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40873 2024-05-16 12:12:32.000000 tmd-2.4.3/tmd/view/view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-05-16 12:12:32.000000 tmd-2.4.3/tox.ini
```

### Comparing `TMD-2.4.2/.auto-changelog` & `tmd-2.4.3/.auto-changelog`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/.auto-changelog-template.hbs` & `tmd-2.4.3/.auto-changelog-template.hbs`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/.copier-answers.yml` & `tmd-2.4.3/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/.github/ISSUE_TEMPLATE/bug_report.yaml` & `tmd-2.4.3/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/.github/ISSUE_TEMPLATE/feature_request.yaml` & `tmd-2.4.3/.github/ISSUE_TEMPLATE/feature_request.yaml`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/.github/ISSUE_TEMPLATE/how_to_use.yaml` & `tmd-2.4.3/.github/ISSUE_TEMPLATE/how_to_use.yaml`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/.github/dependabot.yml` & `tmd-2.4.3/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/.github/pull_request_template.md` & `tmd-2.4.3/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/.github/workflows/commitlint.yml` & `tmd-2.4.3/.github/workflows/commitlint.yml`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/.github/workflows/publish-sdist.yml` & `tmd-2.4.3/.github/workflows/publish-sdist.yml`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/.github/workflows/run-tox.yml` & `tmd-2.4.3/.github/workflows/run-tox.yml`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/.pre-commit-config.yaml` & `tmd-2.4.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/.pylintrc` & `tmd-2.4.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/CHANGELOG.md` & `tmd-2.4.3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/CITATION.cff` & `tmd-2.4.3/CITATION.cff`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/CONTRIBUTING.md` & `tmd-2.4.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/COPYRIGHT.txt` & `tmd-2.4.3/COPYRIGHT.txt`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/LICENSE-BSD.txt` & `tmd-2.4.3/LICENSE-BSD.txt`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/LICENSE-LGPL.txt` & `tmd-2.4.3/LICENSE-LGPL.txt`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/PKG-INFO` & `tmd-2.4.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TMD
-Version: 2.4.2
+Version: 2.4.3
 Summary: A python package for the topological analysis of neurons.
 Home-page: https://TMD.readthedocs.io
 Author: Blue Brain Project, EPFL
 License: GNU Lesser General Public License v3.0
 Project-URL: Tracker, https://github.com/BlueBrain/TMD/issues
 Project-URL: Source, https://github.com/BlueBrain/TMD
 Classifier: Development Status :: 4 - Beta
@@ -30,14 +30,15 @@
 Requires-Dist: cached-property>=1.5.1
 Requires-Dist: morphio<4,>=3.3.4
 Provides-Extra: docs
 Requires-Dist: m2r2; extra == "docs"
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-bluebrain-theme; extra == "docs"
 Requires-Dist: sphinx-click; extra == "docs"
+Requires-Dist: docutils<0.21; extra == "docs"
 Provides-Extra: test
 Requires-Dist: mock>=3; extra == "test"
 Requires-Dist: pytest>=6; extra == "test"
 Requires-Dist: pytest-cov>=3; extra == "test"
 Requires-Dist: pytest-html>=2; extra == "test"
 Provides-Extra: viewer
 Requires-Dist: matplotlib>=3.2.0; extra == "viewer"
```

### Comparing `TMD-2.4.2/README.md` & `tmd-2.4.3/README.md`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/TMD.egg-info/PKG-INFO` & `tmd-2.4.3/TMD.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TMD
-Version: 2.4.2
+Version: 2.4.3
 Summary: A python package for the topological analysis of neurons.
 Home-page: https://TMD.readthedocs.io
 Author: Blue Brain Project, EPFL
 License: GNU Lesser General Public License v3.0
 Project-URL: Tracker, https://github.com/BlueBrain/TMD/issues
 Project-URL: Source, https://github.com/BlueBrain/TMD
 Classifier: Development Status :: 4 - Beta
@@ -30,14 +30,15 @@
 Requires-Dist: cached-property>=1.5.1
 Requires-Dist: morphio<4,>=3.3.4
 Provides-Extra: docs
 Requires-Dist: m2r2; extra == "docs"
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-bluebrain-theme; extra == "docs"
 Requires-Dist: sphinx-click; extra == "docs"
+Requires-Dist: docutils<0.21; extra == "docs"
 Provides-Extra: test
 Requires-Dist: mock>=3; extra == "test"
 Requires-Dist: pytest>=6; extra == "test"
 Requires-Dist: pytest-cov>=3; extra == "test"
 Requires-Dist: pytest-html>=2; extra == "test"
 Provides-Extra: viewer
 Requires-Dist: matplotlib>=3.2.0; extra == "viewer"
```

### Comparing `TMD-2.4.2/TMD.egg-info/SOURCES.txt` & `tmd-2.4.3/TMD.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/commitlint.config.js` & `tmd-2.4.3/commitlint.config.js`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/docs/Makefile` & `tmd-2.4.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/docs/source/conf.py` & `tmd-2.4.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/examples/Advanced/advanced_plot.py` & `tmd-2.4.3/examples/Advanced/advanced_plot.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/examples/Advanced/classification.py` & `tmd-2.4.3/examples/Advanced/classification.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/examples/Advanced/diversity_index.py` & `tmd-2.4.3/examples/Advanced/diversity_index.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/examples/Advanced/matching.py` & `tmd-2.4.3/examples/Advanced/matching.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/examples/Advanced/polar_plot_generation.py` & `tmd-2.4.3/examples/Advanced/polar_plot_generation.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/examples/Advanced/time_series_tmd.py` & `tmd-2.4.3/examples/Advanced/time_series_tmd.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/examples/Advanced/variability.py` & `tmd-2.4.3/examples/Advanced/variability.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/examples/classifier.py` & `tmd-2.4.3/examples/classifier.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/examples/distances_example.py` & `tmd-2.4.3/examples/distances_example.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/examples/extract_ph.py` & `tmd-2.4.3/examples/extract_ph.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/package.json` & `tmd-2.4.3/package.json`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/pyproject.toml` & `tmd-2.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/setup.py` & `tmd-2.4.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 ]
 
 doc_reqs = [
     "m2r2",
     "sphinx",
     "sphinx-bluebrain-theme",
     "sphinx-click",
+    "docutils<0.21",
 ]
 
 test_reqs = [
     "mock>=3",
     "pytest>=6",
     "pytest-cov>=3",
     "pytest-html>=2",
```

### Comparing `TMD-2.4.2/tests/conftest.py` & `tmd-2.4.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tests/data/sample.swc` & `tmd-2.4.3/tests/data/sample.swc`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tests/data/sample_disordered.swc` & `tmd-2.4.3/tests/data/sample_disordered.swc`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tests/data/sample_disordered_v1.h5` & `tmd-2.4.3/tests/data/sample_disordered_v1.h5`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tests/data/sample_v0.h5` & `tmd-2.4.3/tests/data/sample_v0.h5`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tests/data/sample_v1.h5` & `tmd-2.4.3/tests/data/sample_v1.h5`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tests/data/sample_v2.h5` & `tmd-2.4.3/tests/data/sample_v2.h5`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tests/data/test_morph.swc` & `tmd-2.4.3/tests/data/test_morph.swc`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tests/data/test_morph_v1.h5` & `tmd-2.4.3/tests/data/test_morph_v1.h5`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tests/data/test_morph_v2.h5` & `tmd-2.4.3/tests/data/test_morph_v2.h5`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tests/data/upper_case_names/Sample1.ASC` & `tmd-2.4.3/tests/data/upper_case_names/Sample1.ASC`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tests/data/upper_case_names/Sample1.H5` & `tmd-2.4.3/tests/data/upper_case_names/Sample1.H5`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tests/data/upper_case_names/Sample1.SWC` & `tmd-2.4.3/tests/data/upper_case_names/Sample1.SWC`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tests/data/upper_case_names/Sample2.AsC` & `tmd-2.4.3/tests/data/upper_case_names/Sample2.AsC`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tests/data/upper_case_names/Sample2.SwC` & `tmd-2.4.3/tests/data/upper_case_names/Sample2.SwC`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tests/data/valid/C010398B-P2.CNG.swc` & `tmd-2.4.3/tests/data/valid/C010398B-P2.CNG.swc`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tests/data/valid/C010398B-P2.h5` & `tmd-2.4.3/tests/data/valid/C010398B-P2.h5`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tests/data/valid/sample.swc` & `tmd-2.4.3/tests/data/valid/sample.swc`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tests/data/valid/sample_v1.h5` & `tmd-2.4.3/tests/data/valid/sample_v1.h5`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tests/data/valid/sample_v2.h5` & `tmd-2.4.3/tests/data/valid/sample_v2.h5`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tests/test_h5.py` & `tmd-2.4.3/tests/test_h5.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tests/test_io.py` & `tmd-2.4.3/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tests/test_neuron.py` & `tmd-2.4.3/tests/test_neuron.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tests/test_neuron_conversion.py` & `tmd-2.4.3/tests/test_neuron_conversion.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tests/test_population.py` & `tmd-2.4.3/tests/test_population.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tests/test_soma.py` & `tmd-2.4.3/tests/test_soma.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tests/test_soma_methods.py` & `tmd-2.4.3/tests/test_soma_methods.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tests/test_swc.py` & `tmd-2.4.3/tests/test_swc.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tests/test_topology_analysis.py` & `tmd-2.4.3/tests/test_topology_analysis.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tests/test_topology_distances.py` & `tmd-2.4.3/tests/test_topology_distances.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tests/test_topology_methods.py` & `tmd-2.4.3/tests/test_topology_methods.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tests/test_topology_persistent_properties.py` & `tmd-2.4.3/tests/test_topology_persistent_properties.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tests/test_topology_vectorizations.py` & `tmd-2.4.3/tests/test_topology_vectorizations.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tests/test_tree.py` & `tmd-2.4.3/tests/test_tree.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tests/test_tree_methods.py` & `tmd-2.4.3/tests/test_tree_methods.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tmd/Neuron/Neuron.py` & `tmd-2.4.3/tmd/Neuron/Neuron.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tmd/Neuron/__init__.py` & `tmd-2.4.3/tmd/Neuron/__init__.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tmd/Neuron/methods.py` & `tmd-2.4.3/tmd/Neuron/methods.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tmd/Population/Population.py` & `tmd-2.4.3/tmd/Population/Population.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tmd/Population/__init__.py` & `tmd-2.4.3/tmd/Population/__init__.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tmd/Soma/Soma.py` & `tmd-2.4.3/tmd/Soma/Soma.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tmd/Soma/__init__.py` & `tmd-2.4.3/tmd/Soma/__init__.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tmd/Soma/methods.py` & `tmd-2.4.3/tmd/Soma/methods.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tmd/Topology/__init__.py` & `tmd-2.4.3/tmd/Topology/__init__.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tmd/Topology/analysis.py` & `tmd-2.4.3/tmd/Topology/analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -299,10 +299,10 @@
     else:
         p1_enh = p1
         p2_enh = p2
 
     D = cdist(p1_enh, p2_enh)
     m = munkres.Munkres()
     indices = m.compute(np.copy(D))
-    ssum = np.sum([D[i][j] for (i, j) in indices])
+    ssum = np.sum([D[i][j] for (i, j) in indices])  # pylint: disable=unsubscriptable-object
 
     return indices, ssum
```

### Comparing `TMD-2.4.2/tmd/Topology/distances.py` & `tmd-2.4.3/tmd/Topology/distances.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tmd/Topology/methods.py` & `tmd-2.4.3/tmd/Topology/methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,21 +165,19 @@
     neuron, feature="radial_distances", output_file=None, neurite_type="all", sort=False, **kwargs
 ):
     """Extracts persistent homology from tree."""
     ph = get_ph_neuron(neuron, feature=feature, neurite_type="all", **kwargs)
 
     if sort:
         sort_ph(ph)
-    else:
-        p = ph
 
     if output_file is None:
         output_file = "PH_" + neuron.name + "_" + neurite_type + ".txt"
 
-    write_ph(p, output_file)
+    write_ph(ph, output_file)
 
 
 def get_lifetime(tree, feature="point_radial_distances"):
     """Returns the sequence of birth - death times for each section.
 
     This can be used as the first step for the approximation of P.H.
     of the radial distances of the neuronal branches.
```

### Comparing `TMD-2.4.2/tmd/Topology/persistent_properties.py` & `tmd-2.4.3/tmd/Topology/persistent_properties.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tmd/Topology/statistics.py` & `tmd-2.4.3/tmd/Topology/statistics.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tmd/Topology/transformations.py` & `tmd-2.4.3/tmd/Topology/transformations.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tmd/Topology/vectorizations.py` & `tmd-2.4.3/tmd/Topology/vectorizations.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tmd/Tree/Tree.py` & `tmd-2.4.3/tmd/Tree/Tree.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tmd/Tree/__init__.py` & `tmd-2.4.3/tmd/Tree/__init__.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tmd/Tree/methods.py` & `tmd-2.4.3/tmd/Tree/methods.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tmd/__init__.py` & `tmd-2.4.3/tmd/__init__.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tmd/io/__init__.py` & `tmd-2.4.3/tmd/io/__init__.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tmd/io/conversion.py` & `tmd-2.4.3/tmd/io/conversion.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tmd/io/h5.py` & `tmd-2.4.3/tmd/io/h5.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tmd/io/io.py` & `tmd-2.4.3/tmd/io/io.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tmd/io/swc.py` & `tmd-2.4.3/tmd/io/swc.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tmd/utils.py` & `tmd-2.4.3/tmd/utils.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tmd/view/__init__.py` & `tmd-2.4.3/tmd/view/__init__.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tmd/view/common.py` & `tmd-2.4.3/tmd/view/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 import os
 
 import matplotlib.pyplot as plt
 import numpy as np
 
-jet_map = plt.cm.get_cmap("jet")
-blues_map = plt.cm.get_cmap("Blues")
-reds_map = plt.cm.get_cmap("Reds")
+jet_map = plt.get_cmap("jet")
+blues_map = plt.get_cmap("Blues")
+reds_map = plt.get_cmap("Reds")
 
 
 def figure_naming(pretitle=None, posttitle=None, prefile=None, postfile=None):
     """Helping function to define the strings that handle pre-post conventions.
 
     These strings can be used for viewing - plotting title and saving options.
```

### Comparing `TMD-2.4.2/tmd/view/plot.py` & `tmd-2.4.3/tmd/view/plot.py`

 * *Files identical despite different names*

### Comparing `TMD-2.4.2/tmd/view/view.py` & `tmd-2.4.3/tmd/view/view.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,16 +72,15 @@
         horz1 = seg[0][horz] + x_add
         horz2 = seg[1][horz] + x_add
         vert1 = seg[0][vert] + y_add
         vert2 = seg[1][vert] + y_add
 
         return ((horz1, vert1), (horz2, vert2))
 
-    if len(tr.get_segments()) < N:
-        N = len(tr.get_segments())
+    N = min(N, len(tr.get_segments()))
 
     segs = [_seg_2d(seg, hadd, vadd) for seg in tr.get_segments()[:N]]
 
     linewidth = _get_default("linewidth", **kwargs)
 
     # Definition of the linewidth according to diameter, if diameter is True.
 
@@ -690,16 +689,15 @@
         vert1 = seg[0][vert]
         vert2 = seg[1][vert]
         depth1 = seg[0][depth]
         depth2 = seg[1][depth]
 
         return ((horz1, vert1, depth1), (horz2, vert2, depth2))
 
-    if len(tr.get_segments()) < N:
-        N = len(tr.get_segments())
+    N = min(N, len(tr.get_segments()))
 
     segs = [_seg_3d(seg) for seg in tr.get_segments()[:N]]
 
     linewidth = _get_default("linewidth", **kwargs)
 
     # Definition of the linewidth according to diameter, if diameter is True.
 
@@ -1117,15 +1115,15 @@
     tr,
     ph_graph,
     colors=None,
     new_fig=True,
     subplot=111,
     new_axes=True,
     plane="xy",
-    cmap=plt.cm.jet,
+    cmap=plt.jet,
     **kwargs,
 ):
     """Generate a 2d pic of the tree, each branch has a unique color.
 
     Args:
         tr (Tree):
             A Tree object.
```

### Comparing `TMD-2.4.2/tox.ini` & `tmd-2.4.3/tox.ini`

 * *Files identical despite different names*

