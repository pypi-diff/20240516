# Comparing `tmp/qbraid-0.7.0.dev20240423224133.tar.gz` & `tmp/qbraid-0.7.0.dev20240516020308.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbraid-0.7.0.dev20240423224133.tar", last modified: Tue Apr 23 22:41:36 2024, max compression
+gzip compressed data, was "qbraid-0.7.0.dev20240516020308.tar", last modified: Thu May 16 02:03:11 2024, max compression
```

## Comparing `qbraid-0.7.0.dev20240423224133.tar` & `qbraid-0.7.0.dev20240516020308.tar`

### file list

```diff
@@ -1,178 +1,221 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.373251 qbraid-0.7.0.dev20240423224133/
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    55236 2024-04-23 22:41:36.373251 qbraid-0.7.0.dev20240423224133/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11630 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.341251 qbraid-0.7.0.dev20240423224133/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.341251 qbraid-0.7.0.dev20240423224133/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.341251 qbraid-0.7.0.dev20240423224133/docs/_static/cards/
--rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/_static/cards/jupyter.png
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/_static/cards/python.png
--rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/_static/cards/terminal.png
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/_static/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.345251 qbraid-0.7.0.dev20240423224133/docs/_static/pkg-logos/
--rw-r--r--   0 runner    (1001) docker     (127)    36600 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/_static/pkg-logos/braket.png
--rw-r--r--   0 runner    (1001) docker     (127)    53519 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/_static/pkg-logos/cirq.png
--rw-r--r--   0 runner    (1001) docker     (127)    26788 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/_static/pkg-logos/pennylane.png
--rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/_static/pkg-logos/pyquil.png
--rw-r--r--   0 runner    (1001) docker     (127)   125852 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/_static/pkg-logos/qasm.png
--rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/_static/pkg-logos/qir.png
--rw-r--r--   0 runner    (1001) docker     (127)    13073 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/_static/pkg-logos/qiskit.png
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/_static/pkg-logos/quantinuum.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.345251 qbraid-0.7.0.dev20240423224133/docs/_static/sdk-files/
--rw-r--r--   0 runner    (1001) docker     (127)    10475 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/_static/sdk-files/batch_counts.png
--rw-r--r--   0 runner    (1001) docker     (127)    35963 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/_static/sdk-files/conversion_graph.png
--rw-r--r--   0 runner    (1001) docker     (127)   447304 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/_static/sdk-files/get_devices.png
--rw-r--r--   0 runner    (1001) docker     (127)   180765 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/_static/sdk-files/hub_spokes.png
--rw-r--r--   0 runner    (1001) docker     (127)   707295 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/_static/sdk-files/lab_jobs.png
--rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/_static/sdk-files/plot_counts.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.349251 qbraid-0.7.0.dev20240423224133/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/api/qbraid.interface.rst
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/api/qbraid.programs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/api/qbraid.providers.rst
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/api/qbraid.rst
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/api/qbraid.transforms.rst
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/api/qbraid.transpiler.rst
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/api/qbraid.visualization.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.349251 qbraid-0.7.0.dev20240423224133/docs/sdk/
--rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/sdk/devices.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5366 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/sdk/jobs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6273 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/sdk/overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7767 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/sdk/programs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/sdk/providers.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/sdk/results.rst
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/sdk/transpiler.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.349251 qbraid-0.7.0.dev20240423224133/qbraid/
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/_about.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/_import.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-23 22:41:33.000000 qbraid-0.7.0.dev20240423224133/qbraid/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/get_devices.py
--rw-r--r--   0 runner    (1001) docker     (127)     6280 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/get_jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.353251 qbraid-0.7.0.dev20240423224133/qbraid/interface/
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/interface/circuit_equality.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.353251 qbraid-0.7.0.dev20240423224133/qbraid/interface/random/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/interface/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/interface/random/cirq_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/interface/random/qasm3_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/interface/random/qiskit_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/interface/random/random.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.353251 qbraid-0.7.0.dev20240423224133/qbraid/programs/
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/programs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/programs/_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/programs/abc_program.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/programs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/programs/inspector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.357251 qbraid-0.7.0.dev20240423224133/qbraid/programs/libs/
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/programs/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/programs/libs/braket.py
--rw-r--r--   0 runner    (1001) docker     (127)     8907 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/programs/libs/cirq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/programs/libs/pennylane.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/programs/libs/pyquil.py
--rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/programs/libs/pytket.py
--rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/programs/libs/qasm2.py
--rw-r--r--   0 runner    (1001) docker     (127)    15186 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/programs/libs/qasm3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/programs/libs/qiskit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/programs/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/programs/qasm_passes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/programs/qasm_qelib1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.357251 qbraid-0.7.0.dev20240423224133/qbraid/providers/
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/providers/_import.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.357251 qbraid-0.7.0.dev20240423224133/qbraid/providers/aws/
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/providers/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10773 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/providers/aws/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/providers/aws/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     6473 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/providers/aws/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/providers/aws/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/providers/aws/tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)    18460 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/providers/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/providers/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/providers/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.361251 qbraid-0.7.0.dev20240423224133/qbraid/providers/ibm/
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/providers/ibm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6166 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/providers/ibm/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/providers/ibm/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/providers/ibm/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/providers/ibm/result.py
--rw-r--r--   0 runner    (1001) docker     (127)    10095 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/providers/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     8511 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/providers/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/providers/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/providers/status_maps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.361251 qbraid-0.7.0.dev20240423224133/qbraid/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transforms/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.361251 qbraid-0.7.0.dev20240423224133/qbraid/transforms/pytket/
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transforms/pytket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transforms/pytket/ionq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.361251 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/annotations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.361251 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.361251 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/braket/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/braket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10636 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/braket/cirq_from_braket.py
--rw-r--r--   0 runner    (1001) docker     (127)    13215 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/braket/cirq_to_braket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/braket/conversions_cirq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/braket/conversions_qasm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/braket/custom_instr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.365251 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/cirq/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/cirq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23224 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/cirq/cirq_qasm_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/cirq/conversions_qasm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/cirq/custom_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.365251 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/openqasm3/
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/openqasm3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/openqasm3/conversions_qasm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.365251 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/pennylane/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/pennylane/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/pennylane/conversions_qasm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.365251 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/pyquil/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/pyquil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10806 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/pyquil/cirq_quil_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    21811 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/pyquil/cirq_quil_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/pyquil/conversions_cirq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.365251 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/pytket/
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/pytket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/pytket/conversions_braket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/pytket/conversions_qasm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.365251 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/qiskit/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/qiskit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/qiskit/conversions_braket.py
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/qiskit/conversions_qasm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7054 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7275 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.365251 qbraid-0.7.0.dev20240423224133/qbraid/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/visualization/draw_circuit.py
--rw-r--r--   0 runner    (1001) docker     (127)    13544 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/visualization/draw_qasm3.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/visualization/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/visualization/plot_conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10107 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/visualization/plot_counts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.365251 qbraid-0.7.0.dev20240423224133/qbraid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    55236 2024-04-23 22:41:36.000000 qbraid-0.7.0.dev20240423224133/qbraid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-04-23 22:41:36.000000 qbraid-0.7.0.dev20240423224133/qbraid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 22:41:36.000000 qbraid-0.7.0.dev20240423224133/qbraid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-23 22:41:36.000000 qbraid-0.7.0.dev20240423224133/qbraid.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-23 22:41:36.000000 qbraid-0.7.0.dev20240423224133/qbraid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-23 22:41:36.000000 qbraid-0.7.0.dev20240423224133/qbraid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 22:41:36.373251 qbraid-0.7.0.dev20240423224133/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.365251 qbraid-0.7.0.dev20240423224133/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/tools/set_provider_configs.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4480 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/tools/verify_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.527386 qbraid-0.7.0.dev20240516020308/
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15828 2024-05-16 02:03:11.527386 qbraid-0.7.0.dev20240516020308/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13159 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.495386 qbraid-0.7.0.dev20240516020308/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.495386 qbraid-0.7.0.dev20240516020308/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.495386 qbraid-0.7.0.dev20240516020308/docs/_static/cards/
+-rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/_static/cards/jupyter.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/_static/cards/python.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/_static/cards/terminal.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/_static/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.499386 qbraid-0.7.0.dev20240516020308/docs/_static/pkg-logos/
+-rw-r--r--   0 runner    (1001) docker     (127)    36600 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/_static/pkg-logos/braket.png
+-rw-r--r--   0 runner    (1001) docker     (127)    53519 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/_static/pkg-logos/cirq.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26788 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/_static/pkg-logos/pennylane.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/_static/pkg-logos/pyquil.png
+-rw-r--r--   0 runner    (1001) docker     (127)   125852 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/_static/pkg-logos/qasm.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/_static/pkg-logos/qir.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13073 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/_static/pkg-logos/qiskit.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/_static/pkg-logos/quantinuum.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.499386 qbraid-0.7.0.dev20240516020308/docs/_static/sdk-files/
+-rw-r--r--   0 runner    (1001) docker     (127)    10475 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/_static/sdk-files/batch_counts.png
+-rw-r--r--   0 runner    (1001) docker     (127)    35963 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/_static/sdk-files/conversion_graph.png
+-rw-r--r--   0 runner    (1001) docker     (127)   447304 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/_static/sdk-files/get_devices.png
+-rw-r--r--   0 runner    (1001) docker     (127)   180765 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/_static/sdk-files/hub_spokes.png
+-rw-r--r--   0 runner    (1001) docker     (127)   707295 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/_static/sdk-files/lab_jobs.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/_static/sdk-files/plot_counts.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.499386 qbraid-0.7.0.dev20240516020308/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/api/qbraid.interface.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/api/qbraid.programs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/api/qbraid.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/api/qbraid.runtime.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/api/qbraid.transforms.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/api/qbraid.transpiler.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/api/qbraid.visualization.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.503386 qbraid-0.7.0.dev20240516020308/docs/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/sdk/devices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5385 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/sdk/jobs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6277 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/sdk/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7767 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/sdk/programs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/sdk/providers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/sdk/results.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/sdk/transpiler.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.503386 qbraid-0.7.0.dev20240516020308/qbraid/
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/_about.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-16 02:03:08.000000 qbraid-0.7.0.dev20240516020308/qbraid/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.503386 qbraid-0.7.0.dev20240516020308/qbraid/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/interface/circuit_equality.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.507386 qbraid-0.7.0.dev20240516020308/qbraid/interface/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/interface/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/interface/random/cirq_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/interface/random/qasm3_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/interface/random/qiskit_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/interface/random/random.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.507386 qbraid-0.7.0.dev20240516020308/qbraid/programs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/programs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/programs/_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/programs/alias_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/programs/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.507386 qbraid-0.7.0.dev20240516020308/qbraid/programs/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/programs/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/programs/libs/braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9515 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/programs/libs/cirq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/programs/libs/pennylane.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/programs/libs/pyquil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/programs/libs/pytket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/programs/libs/qasm2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15083 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/programs/libs/qasm3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/programs/libs/qiskit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/programs/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6210 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/programs/program.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/programs/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/programs/spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.511386 qbraid-0.7.0.dev20240516020308/qbraid/runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/_display.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.511386 qbraid-0.7.0.dev20240516020308/qbraid/runtime/braket/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/braket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8698 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/braket/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/braket/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8902 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/braket/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/braket/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/braket/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8840 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.511386 qbraid-0.7.0.dev20240516020308/qbraid/runtime/ionq/
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/ionq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/ionq/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/ionq/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/ionq/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/ionq/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.511386 qbraid-0.7.0.dev20240516020308/qbraid/runtime/native/
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/native/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7722 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/native/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/native/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/native/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/native/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.511386 qbraid-0.7.0.dev20240516020308/qbraid/runtime/qiskit/
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/qiskit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/qiskit/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/qiskit/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4722 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/qiskit/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/qiskit/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/result.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.515386 qbraid-0.7.0.dev20240516020308/qbraid/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.515386 qbraid-0.7.0.dev20240516020308/qbraid/transforms/braket/
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transforms/braket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transforms/braket/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.515386 qbraid-0.7.0.dev20240516020308/qbraid/transforms/cirq/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transforms/cirq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transforms/cirq/passes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transforms/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.515386 qbraid-0.7.0.dev20240516020308/qbraid/transforms/pytket/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transforms/pytket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transforms/pytket/ionq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.515386 qbraid-0.7.0.dev20240516020308/qbraid/transforms/qasm2/
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transforms/qasm2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transforms/qasm2/passes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transforms/qasm2/qasm_qelib1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.515386 qbraid-0.7.0.dev20240516020308/qbraid/transforms/qasm3/
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transforms/qasm3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transforms/qasm3/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.515386 qbraid-0.7.0.dev20240516020308/qbraid/transforms/qiskit/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transforms/qiskit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transforms/qiskit/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.515386 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/annotations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.515386 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.519386 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/braket/
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/braket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/braket/braket_extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11942 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/braket/braket_to_cirq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/braket/braket_to_qasm3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.519386 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/cirq/
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/cirq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/cirq/braket_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/cirq/cirq_extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21821 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/cirq/cirq_quil_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13536 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/cirq/cirq_to_braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/cirq/cirq_to_pyquil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/cirq/cirq_to_qasm2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.519386 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/openqasm3/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/openqasm3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/openqasm3/openqasm3_to_qasm3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.519386 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/pennylane/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/pennylane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/pennylane/pennylane_to_qasm2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.519386 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/pyquil/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/pyquil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10800 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/pyquil/cirq_quil_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/pyquil/pyquil_to_cirq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.519386 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/pytket/
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/pytket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/pytket/pytket_extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/pytket/pytket_to_qasm2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.519386 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qasm2/
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qasm2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qasm2/cirq_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23075 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qasm2/cirq_qasm_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qasm2/qasm2_to_cirq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qasm2/qasm2_to_pytket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qasm2/qasm2_to_qasm3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qasm2/qasm2_to_qiskit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.523386 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qasm3/
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qasm3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qasm3/qasm3_extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qasm3/qasm3_to_braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qasm3/qasm3_to_openqasm3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qasm3/qasm3_to_qiskit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.523386 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qiskit/
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qiskit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qiskit/qiskit_extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qiskit/qiskit_to_qasm2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qiskit/qiskit_to_qasm3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7556 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/scheme.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.523386 qbraid-0.7.0.dev20240516020308/qbraid/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/visualization/draw_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13544 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/visualization/draw_qasm3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/visualization/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/visualization/plot_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10199 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/visualization/plot_counts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.523386 qbraid-0.7.0.dev20240516020308/qbraid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15828 2024-05-16 02:03:11.000000 qbraid-0.7.0.dev20240516020308/qbraid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6157 2024-05-16 02:03:11.000000 qbraid-0.7.0.dev20240516020308/qbraid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 02:03:11.000000 qbraid-0.7.0.dev20240516020308/qbraid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-16 02:03:11.000000 qbraid-0.7.0.dev20240516020308/qbraid.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-16 02:03:11.000000 qbraid-0.7.0.dev20240516020308/qbraid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-16 02:03:11.000000 qbraid-0.7.0.dev20240516020308/qbraid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 02:03:11.527386 qbraid-0.7.0.dev20240516020308/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.523386 qbraid-0.7.0.dev20240516020308/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/tools/set_provider_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/tox.ini
```

### Comparing `qbraid-0.7.0.dev20240423224133/CODE_OF_CONDUCT.md` & `qbraid-0.7.0.dev20240516020308/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240423224133/CONTRIBUTING.md` & `qbraid-0.7.0.dev20240516020308/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240423224133/LICENSE` & `qbraid-0.7.0.dev20240516020308/LICENSE`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240423224133/README.md` & `qbraid-0.7.0.dev20240516020308/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -20,29 +20,44 @@
     <img src="https://img.shields.io/github/license/qBraid/qbraid.svg" alt="License"/>
   </a>
   <a href="https://discord.gg/TPBU2sa8Et">
     <img src="https://img.shields.io/discord/771898982564626445.svg?color=pink" alt="Discord"/>
   </a>
 </p>
 
-The qBraid-SDK is a Python toolkit for cross-framework abstraction,
-transpilation, and execution of quantum programs.
+The qBraid-SDK is a platform-agnostic quantum runtime framework designed for both quantum software and hardware providers.
+
+This Python-based tool streamlines the full lifecycle management of quantum jobs&mdash;from defining program specifications to job submission, and through to the post-processing and visualization of results. Distinguishing itself through a streamlined and highly-configurable approach to cross-platform integration, the qBraid-SDK *does not assume a fixed target software framework*. Instead, it allows providers to dynamically register any desired run input program type as the target, depending on their specific needs. These program types are interconnected via a graph-based transpiler, where each program type is represented as a node and supported conversions as edges. The breadth, depth, and connectivity of this `ConversionGraph` can be customized by the provider.
+
+The framework also facilitates the insertion of additional program validations, circuit transformations, and transpiler/compiler steps into its modular pipeline through a comprehensive `TargetProfile`. This profile encapsulates both device properties (such as number of qubits, maximum shots, native gate set) and the software requirements (`ProgramSpec`) needed to submit a job, vastly reducing the overhead and redundancy typically associated with cross-platform integrations in quantum computing.
 
 [<img src="https://qbraid-static.s3.amazonaws.com/logos/Launch_on_qBraid_white.png" width="150">](https://account.qbraid.com?gitHubUrl=https://github.com/qBraid/qBraid.git)
 
-## Features
+## Key Features
+
+### 1. Quantum Program Integration
+
+Offers native support for 10 major quantum programming libraries including 20+ inter-library conversions with the ability to
+dynamically register new program types and conversions on the fly. This enables flexible program submissions to cater to the unique capabilities and constraints of your preferred framework, facilitated by a unique conversion map that automatically adapts quantum programs during runtime according to the given specifications.
+
+### 2. Modular Design
 
-- Unified quantum frontend interface. **Transpile** quantum circuits between
-  supported packages. Leverage the capabilities of multiple frontends through
-  **simple, consistent protocols**.
-- Build once, target many. **Create** quantum programs using your preferred
-  circuit-building package, and **execute** on any backend that interfaces with
-  a supported frontend.
-- Benchmark, compare, interpret results. Built-in **compatible** post-processing
-  enables comparing results between runs and **across backends**.
+- `qbraid.programs`: Extracts and manages metadata from supported quantum program types, with the flexibility to introduce new types.
+- `qbraid.transpiler`: Bridges different quantum programming IRs through native and customizable circuit conversions.
+- `qbraid.transforms`: Ensures quantum programs conform to hardware specifications through essential runtime transformations.
+- `qbraid.runtime`: Defines essential abstractions for providers, devices, jobs, and results, integrated through a coherent runtime profile.
+- `qbraid.visualization`: Provides tools for visualizing quantum circuits and experimental data, enhancing data interpretation.
+
+### 3. Extensibility and Customization
+
+The framework encourages community contributions and extensions, supporting an evolving ecosystem of program types and conversions, adaptable to specific provider needs. By providing a comprehensive runtime solution, the qBraid-SDK offers significant advantages to *both hardware and software providers*:
+
+- **Reduces Overhead**: Minimizes the effort required to develop client-side applications for securely submitting and managing quantum experiments remotely.
+- **Enhances Integration**: Facilitates seamless integration and interoperability of quantum software tools across all layers of the stack.
+- **Broad Compatibility**: Supports a diverse range of API complexities, catering to both established players like IBM and AWS as well as emerging providers.
 
 ## Installation & Setup
 
 <img align="right" width="300" alt="qbraid-sdk-env" src="https://github.com/qBraid/qBraid/assets/46977852/c82d61b4-2518-4c7e-8f48-05106afa708e">
 
 For the best experience, install the qBraid-SDK environment on
 [lab.qbraid.com](https://lab.qbraid.com). Login (or
@@ -63,21 +78,19 @@
 
 ```shell
 git clone https://github.com/qBraid/qBraid.git
 cd qBraid
 pip install .
 ```
 
-*Note*: The qBraid-SDK requires Python 3.9 or greater.
+> *Note:* The qBraid-SDK requires Python 3.9 or greater.
 
 If using locally, follow linked instructions to configure your
 [qBraid](#local-account-setup),
-[AWS](https://github.com/aws/amazon-braket-sdk-python#boto3-and-setting-up-aws-credentials),
-and [IBMQ](https://github.com/Qiskit/qiskit-ibm-provider#provider-setup)
-credentials.
+[AWS](https://github.com/aws/amazon-braket-sdk-python#boto3-and-setting-up-aws-credentials), [IBM](https://github.com/Qiskit/qiskit-ibm-runtime?tab=readme-ov-file#account-setup), and/or [IonQ](https://cloud.ionq.com/settings/keys) credentials.
 
 ### Check version
 
 You can view the version of the qBraid-SDK you have installed within Python using the following:
 
 ```python
 In [1]: import qbraid
@@ -98,33 +111,33 @@
 
 ## Quickstart
 
 ### Transpiler
 
 Construct a quantum program of any supported program type.
 
-Below, `SUPPORTED_QPROGRAMS` maps shorthand identifiers for supported quantum programs, each corresponding to a type in the typed `QPROGRAM` Union.
+Below, `QPROGRAM_REGISTRY` maps shorthand identifiers for supported quantum programs, each corresponding to a type in the typed `QPROGRAM` Union.
 For example, 'qiskit' maps to `qiskit.QuantumCircuit` in `QPROGRAM`. Notably, 'qasm2' and 'qasm3' both represent raw OpenQASM strings.
 This arrangement simplifies targeting and transpiling between different quantum programming frameworks.
 
 ```python
->>> from qbraid.programs import SUPPORTED_QPROGRAMS
->>> SUPPORTED_QPROGRAMS
+>>> from qbraid.programs import QPROGRAM_REGISTRY
+>>> QPROGRAM_REGISTRY
 {'cirq': 'cirq.circuits.circuit.Circuit',
  'qiskit': 'qiskit.circuit.quantumcircuit.QuantumCircuit',
  'pyquil': 'pyquil.quil.Program',
  'pytket': 'pytket._tket.circuit.Circuit',
  'braket': 'braket.circuits.circuit.Circuit',
  'openqasm3': 'openqasm3.ast.Program',
  'qasm2': 'str',
  'qasm3': 'str'}
 ```
 
-Pass any quantum program of type `qbraid.programs.QPROGRAM` to the `load_program()` and specify a target package
-from `SUPPORTED_QPROGRAMS` to "transpile" your circuit to a new program type:
+Pass any registered quantum program along with a target package from
+`QPROGRAM_REGISTRY` to "transpile" your circuit to a new program type:
 
 ```python
 >>> from qbraid.interface import random_circuit
 >>> from qbraid.transpiler import transpile
 >>> qiskit_circuit = random_circuit("qiskit")
 >>> cirq_circuit = transpile(qiskit_circuit, "cirq")
 >>> print(qiskit_circuit)
@@ -135,147 +148,104 @@
      └───┘    └────┘
 >>> print(cirq_circuit)
 0: ───@───Rx(0.966π)───
       │
 1: ───H───X^0.5────────
 ```
 
-The same functionality can be achieved using the underlying `transpile()` function directly:
-
-```python
->>> from qbraid.transpiler import transpile
->>> cirq_circuit = transpile(qiskit_circuit, "cirq")
-```
-
 Behind the scenes, the qBraid-SDK uses ``networkx`` to create a directional graph that maps all possible conversions between supported program types:
 
 ```python
 from qbraid.transpiler import ConversionGraph
 from qbraid.visualization import plot_conversion_graph
 
 graph = ConversionGraph()
 
 graph.plot()
 ```
 
-<img align="middle" width="full" alt="conversion_graph" src="https://qbraid-static.s3.amazonaws.com/conversion_graph.png">
+<img align="middle" width="full" alt="conversion_graph" src="https://qbraid-static.s3.amazonaws.com/conversion_graph_extras.png">
 
 You can use the native conversions supported by qBraid, or define your own custom nodes and/or edges. For [example](https://github.com/qBraid/qbraid-qir?tab=readme-ov-file#add-qir-node-to-qbraid-conversion-graph):
 
 ```python
 from qbraid_qir.qasm3 import qasm3_to_qir
 from qbraid.transpiler import Conversion
 
-conversion = Conversion("qasm3", "qir", qasm3_to_qir)
+conversion = Conversion("qasm3", "pyqir", qasm3_to_qir)
 
 graph.add_conversion(conversion)
 
 graph.plot()
 ```
 
-### Devices & Jobs
-
-Search for quantum backend(s) on which to execute your program.
-
-```python
->>> from qbraid import get_devices
->>> get_devices()
-Device status updated 0 minutes ago
-
-Device ID                           Status
----------                           ------
-aws_oqc_lucy                        ONLINE
-aws_ionq_aria2                      OFFLINE
-aws_rigetti_aspen_m3                ONLINE
-ibm_q_brisbane                      ONLINE
-...
-
-```
+### QbraidProvider
 
-You can get a Python list of device objects using:
+Run experiements using on-demand simulators provided by qBraid using the `qbraid.runtime.native.QbraidProvider`. You can get a Python list of device objects using:
 
 ```python
-from qbraid.providers import QbraidProvider
+from qbraid.runtime.native import QbraidProvider
 
 provider = QbraidProvider()
 qdevices = provider.get_devices()
 ```
 
 Or, instantiate a known device by ID via the `QbraidProvider.get_device()` method,
 and submit quantum jobs from any supported program type:
 
 ```python
->>> from qbraid import get_jobs
->>> from qbraid.providers import QbraidProvider
->>> provider = QbraidProvider()
->>> aws_device = provider.get_device("aws_oqc_lucy")
->>> ibm_device = provider.get_device("ibm_q_brisbane")
->>> aws_job = aws_device.run(qiskit_circuit, shots=1000)
->>> ibm_job = ibm_device.run(cirq_circuit, shots=1000)
->>> get_jobs()
-Displaying 2 most recent jobs:
-
-Job ID                                              Submitted                  Status
-------                                              ---------                  ------
-aws_oqc_lucy-exampleuser-qjob-zzzzzzz...            2023-05-21T21:13:47.220Z   QUEUED
-ibm_q_brisbane-exampleuser-qjob-xxxxxxx...          2023-05-21T21:13:48.220Z   RUNNING
-...
-```
-
-Compare results in a consistent, unified format:
+device = provider.get_device("qbraid_qir_simulator")
+jobs = device.run([qiskit_circuit, braket_circuit, cirq_circuit, qasm3_str], shots=1000)
+results = [job.result() for job in jobs]
 
-```python
->>> aws_result = aws_job.result()
->>> ibm_result = ibm_job.result()
->>> aws_result.measurement_counts()
-{'00': 483, '01': 14, '10': 486, '11': 17}
->>> ibm_result.measurement_counts()
-{'00': 496, '01': 12, '10': 479, '11': 13}
+print(results[0].measurement_counts())
+# {'00': 483, '01': 14, '10': 486, '11': 17}
 ```
 
 ## Local account setup
+
 <img align="right" width="300" alt="api_key" src="https://qbraid-static.s3.amazonaws.com/manage-account.png">
 
 To use the qBraid-SDK locally (outside of qBraid Lab), you must add your account
 credentials:
 
 1. Create a qBraid account or log in to your existing account by visiting
    [account.qbraid.com](https://account.qbraid.com/)
 2. Copy your API Key token from the left side of
     your [account page](https://account.qbraid.com/):
 
-3. Save your API key from step 2 by calling
-   `QbraidSession.save_config()`:
+### Save account to disk
+
+Once you have your API key from step 2 by, you can save it locally in a configuration file `~/.qbraid/qbraidrc`,
+where `~` corresponds to your home (`$HOME`) directory:
+
+| :warning: Account credentials are saved in plain text, so only do so if you are using a trusted device. |
+|:---------------------------|
 
 ```python
-from qbraid_core import QbraidSession
+from qbraid.runtime.native import QbraidProvider
 
-session = QbraidSession(api_key='API_KEY')
-session.save_config()
+provider = QbraidProvider(api_key='API_KEY')
+provider.save_config()
 ```
 
-The command above stores your credentials locally in a configuration file `~/.qbraid/qbraidrc`,
-where `~` corresponds to your home (`$HOME`) directory. Once saved, you can then connect to the
-qBraid API and leverage functions such as `get_devices()` and `get_jobs()`.
+Once the account is saved on disk, you can instantiate the provider without any arguments:
 
-### Load Account from Environment Variables
-
-Alternatively, the qBraid-SDK can discover credentials from environment
-variables:
+```python
+from qbraid.runtime.native import QbraidProvider
 
-```shell
-export QBRAID_API_KEY='QBRAID_API_KEY'
+provider = QbraidProvider()
 ```
 
-Then instantiate the session without any arguments
+### Load account from environment variables
 
-```python
-from qbraid_core import QbraidSession
+Alternatively, the qBraid-SDK can discover credentials from environment variables:
 
-session = QbraidSession()
+```shell
+export QBRAID_API_KEY='QBRAID_API_KEY'
 ```
 
 ## Launch on qBraid
 
 The "Launch on qBraid" button (below) can be added to any public GitHub
 repository. Clicking on it automaically opens qBraid Lab, and performs a
 `git clone` of the project repo into your account's home directory. Copy the
```

#### html2text {}

```diff
@@ -1,131 +1,155 @@
 [qbraid-sdk-header]
 _[_C_I_]_[_c_o_d_e_c_o_v_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]_[_L_i_c_e_n_s_e_]_[_D_i_s_c_o_r_d_]
-The qBraid-SDK is a Python toolkit for cross-framework abstraction,
-transpilation, and execution of quantum programs. [[https://qbraid-
+The qBraid-SDK is a platform-agnostic quantum runtime framework designed for
+both quantum software and hardware providers. This Python-based tool
+streamlines the full lifecycle management of quantum jobs—from defining program
+specifications to job submission, and through to the post-processing and
+visualization of results. Distinguishing itself through a streamlined and
+highly-configurable approach to cross-platform integration, the qBraid-SDK
+*does not assume a fixed target software framework*. Instead, it allows
+providers to dynamically register any desired run input program type as the
+target, depending on their specific needs. These program types are
+interconnected via a graph-based transpiler, where each program type is
+represented as a node and supported conversions as edges. The breadth, depth,
+and connectivity of this `ConversionGraph` can be customized by the provider.
+The framework also facilitates the insertion of additional program validations,
+circuit transformations, and transpiler/compiler steps into its modular
+pipeline through a comprehensive `TargetProfile`. This profile encapsulates
+both device properties (such as number of qubits, maximum shots, native gate
+set) and the software requirements (`ProgramSpec`) needed to submit a job,
+vastly reducing the overhead and redundancy typically associated with cross-
+platform integrations in quantum computing. [[https://qbraid-
 static.s3.amazonaws.com/logos/Launch_on_qBraid_white.png]](https://
-account.qbraid.com?gitHubUrl=https://github.com/qBraid/qBraid.git) ## Features
-- Unified quantum frontend interface. **Transpile** quantum circuits between
-supported packages. Leverage the capabilities of multiple frontends through
-**simple, consistent protocols**. - Build once, target many. **Create** quantum
-programs using your preferred circuit-building package, and **execute** on any
-backend that interfaces with a supported frontend. - Benchmark, compare,
-interpret results. Built-in **compatible** post-processing enables comparing
-results between runs and **across backends**. ## Installation & Setup [qbraid-
-sdk-env]For the best experience, install the qBraid-SDK environment on
-[lab.qbraid.com](https://lab.qbraid.com). Login (or [create an account](https:/
-/account.qbraid.com)) and follow the steps to [install an environment](https://
-docs.qbraid.com/projects/lab/en/latest/lab/environments.html#install-
-environment). Using the SDK on [qBraid Lab](https://docs.qbraid.com/projects/
-lab/en/latest/lab/overview.html) means direct, pre-configured access to QPUs
-from IonQ, Oxford Quantum Circuits, QuEra, and Rigetti, as well as on-demand
-simulators from AWS, all with no additional access keys or API tokens required.
-See [qBraid Quantum Jobs](https://docs.qbraid.com/projects/lab/en/latest/lab/
-quantum_jobs.html) for more. ### Local install The qBraid-SDK, and all of its
-dependencies, can also be installed using pip: ```shell pip install qbraid ```
-You can also [install from source](CONTRIBUTING.md#installing-from-source) by
-cloning this repository and running a pip install command in the root directory
-of the repository: ```shell git clone https://github.com/qBraid/qBraid.git cd
-qBraid pip install . ``` *Note*: The qBraid-SDK requires Python 3.9 or greater.
-If using locally, follow linked instructions to configure your [qBraid](#local-
-account-setup), [AWS](https://github.com/aws/amazon-braket-sdk-python#boto3-
-and-setting-up-aws-credentials), and [IBMQ](https://github.com/Qiskit/qiskit-
-ibm-provider#provider-setup) credentials. ### Check version You can view the
-version of the qBraid-SDK you have installed within Python using the following:
-```python In [1]: import qbraid In [2]: qbraid.__version__ ``` ## Documentation
-& Tutorials qBraid documentation is available at [docs.qbraid.com](https://
-docs.qbraid.com/en/stable/). See also: - [API Reference](https://
-docs.qbraid.com/en/stable/api/qbraid.html) - [User Guide](https://
-docs.qbraid.com/en/stable/sdk/overview.html) - [Example Notebooks](https://
-github.com/qBraid/qbraid-lab-demo) ## Quickstart ### Transpiler Construct a
-quantum program of any supported program type. Below, `SUPPORTED_QPROGRAMS`
-maps shorthand identifiers for supported quantum programs, each corresponding
-to a type in the typed `QPROGRAM` Union. For example, 'qiskit' maps to
-`qiskit.QuantumCircuit` in `QPROGRAM`. Notably, 'qasm2' and 'qasm3' both
-represent raw OpenQASM strings. This arrangement simplifies targeting and
-transpiling between different quantum programming frameworks. ```python >>>
-from qbraid.programs import SUPPORTED_QPROGRAMS >>> SUPPORTED_QPROGRAMS
-{'cirq': 'cirq.circuits.circuit.Circuit', 'qiskit':
+account.qbraid.com?gitHubUrl=https://github.com/qBraid/qBraid.git) ## Key
+Features ### 1. Quantum Program Integration Offers native support for 10 major
+quantum programming libraries including 20+ inter-library conversions with the
+ability to dynamically register new program types and conversions on the fly.
+This enables flexible program submissions to cater to the unique capabilities
+and constraints of your preferred framework, facilitated by a unique conversion
+map that automatically adapts quantum programs during runtime according to the
+given specifications. ### 2. Modular Design - `qbraid.programs`: Extracts and
+manages metadata from supported quantum program types, with the flexibility to
+introduce new types. - `qbraid.transpiler`: Bridges different quantum
+programming IRs through native and customizable circuit conversions. -
+`qbraid.transforms`: Ensures quantum programs conform to hardware
+specifications through essential runtime transformations. - `qbraid.runtime`:
+Defines essential abstractions for providers, devices, jobs, and results,
+integrated through a coherent runtime profile. - `qbraid.visualization`:
+Provides tools for visualizing quantum circuits and experimental data,
+enhancing data interpretation. ### 3. Extensibility and Customization The
+framework encourages community contributions and extensions, supporting an
+evolving ecosystem of program types and conversions, adaptable to specific
+provider needs. By providing a comprehensive runtime solution, the qBraid-SDK
+offers significant advantages to *both hardware and software providers*: -
+**Reduces Overhead**: Minimizes the effort required to develop client-side
+applications for securely submitting and managing quantum experiments remotely.
+- **Enhances Integration**: Facilitates seamless integration and
+interoperability of quantum software tools across all layers of the stack. -
+**Broad Compatibility**: Supports a diverse range of API complexities, catering
+to both established players like IBM and AWS as well as emerging providers. ##
+Installation & Setup [qbraid-sdk-env]For the best experience, install the
+qBraid-SDK environment on [lab.qbraid.com](https://lab.qbraid.com). Login (or
+[create an account](https://account.qbraid.com)) and follow the steps to
+[install an environment](https://docs.qbraid.com/projects/lab/en/latest/lab/
+environments.html#install-environment). Using the SDK on [qBraid Lab](https://
+docs.qbraid.com/projects/lab/en/latest/lab/overview.html) means direct, pre-
+configured access to QPUs from IonQ, Oxford Quantum Circuits, QuEra, and
+Rigetti, as well as on-demand simulators from AWS, all with no additional
+access keys or API tokens required. See [qBraid Quantum Jobs](https://
+docs.qbraid.com/projects/lab/en/latest/lab/quantum_jobs.html) for more. ###
+Local install The qBraid-SDK, and all of its dependencies, can also be
+installed using pip: ```shell pip install qbraid ``` You can also [install from
+source](CONTRIBUTING.md#installing-from-source) by cloning this repository and
+running a pip install command in the root directory of the repository: ```shell
+git clone https://github.com/qBraid/qBraid.git cd qBraid pip install . ``` >
+*Note:* The qBraid-SDK requires Python 3.9 or greater. If using locally, follow
+linked instructions to configure your [qBraid](#local-account-setup), [AWS]
+(https://github.com/aws/amazon-braket-sdk-python#boto3-and-setting-up-aws-
+credentials), [IBM](https://github.com/Qiskit/qiskit-ibm-runtime?tab=readme-ov-
+file#account-setup), and/or [IonQ](https://cloud.ionq.com/settings/keys)
+credentials. ### Check version You can view the version of the qBraid-SDK you
+have installed within Python using the following: ```python In [1]: import
+qbraid In [2]: qbraid.__version__ ``` ## Documentation & Tutorials qBraid
+documentation is available at [docs.qbraid.com](https://docs.qbraid.com/en/
+stable/). See also: - [API Reference](https://docs.qbraid.com/en/stable/api/
+qbraid.html) - [User Guide](https://docs.qbraid.com/en/stable/sdk/
+overview.html) - [Example Notebooks](https://github.com/qBraid/qbraid-lab-demo)
+## Quickstart ### Transpiler Construct a quantum program of any supported
+program type. Below, `QPROGRAM_REGISTRY` maps shorthand identifiers for
+supported quantum programs, each corresponding to a type in the typed
+`QPROGRAM` Union. For example, 'qiskit' maps to `qiskit.QuantumCircuit` in
+`QPROGRAM`. Notably, 'qasm2' and 'qasm3' both represent raw OpenQASM strings.
+This arrangement simplifies targeting and transpiling between different quantum
+programming frameworks. ```python >>> from qbraid.programs import
+QPROGRAM_REGISTRY >>> QPROGRAM_REGISTRY {'cirq':
+'cirq.circuits.circuit.Circuit', 'qiskit':
 'qiskit.circuit.quantumcircuit.QuantumCircuit', 'pyquil':
 'pyquil.quil.Program', 'pytket': 'pytket._tket.circuit.Circuit', 'braket':
 'braket.circuits.circuit.Circuit', 'openqasm3': 'openqasm3.ast.Program',
-'qasm2': 'str', 'qasm3': 'str'} ``` Pass any quantum program of type
-`qbraid.programs.QPROGRAM` to the `load_program()` and specify a target package
-from `SUPPORTED_QPROGRAMS` to "transpile" your circuit to a new program type:
-```python >>> from qbraid.interface import random_circuit >>> from
-qbraid.transpiler import transpile >>> qiskit_circuit = random_circuit
+'qasm2': 'str', 'qasm3': 'str'} ``` Pass any registered quantum program along
+with a target package from `QPROGRAM_REGISTRY` to "transpile" your circuit to a
+new program type: ```python >>> from qbraid.interface import random_circuit >>>
+from qbraid.transpiler import transpile >>> qiskit_circuit = random_circuit
 ("qiskit") >>> cirq_circuit = transpile(qiskit_circuit, "cirq") >>> print
 (qiskit_circuit) ââââââââââââââ q_0:
 âââ âââ¤ Rx(3.0353) â
 âââ´âââââââ¬âââââ¬ââââ q_1: â¤ H
 ââââââ¤ âX âââââ âââââ ââââââ >>>
 print(cirq_circuit) 0: âââ@âââRx(0.966Ï)âââ â 1:
-âââHâââX^0.5ââââââââ ``` The same functionality can
-be achieved using the underlying `transpile()` function directly: ```python >>>
-from qbraid.transpiler import transpile >>> cirq_circuit = transpile
-(qiskit_circuit, "cirq") ``` Behind the scenes, the qBraid-SDK uses
-``networkx`` to create a directional graph that maps all possible conversions
-between supported program types: ```python from qbraid.transpiler import
-ConversionGraph from qbraid.visualization import plot_conversion_graph graph =
-ConversionGraph() graph.plot() ``` [conversion_graph]You can use the native
-conversions supported by qBraid, or define your own custom nodes and/or edges.
-For [example](https://github.com/qBraid/qbraid-qir?tab=readme-ov-file#add-qir-
-node-to-qbraid-conversion-graph): ```python from qbraid_qir.qasm3 import
-qasm3_to_qir from qbraid.transpiler import Conversion conversion = Conversion
-("qasm3", "qir", qasm3_to_qir) graph.add_conversion(conversion) graph.plot()
-``` ### Devices & Jobs Search for quantum backend(s) on which to execute your
-program. ```python >>> from qbraid import get_devices >>> get_devices() Device
-status updated 0 minutes ago Device ID Status --------- ------ aws_oqc_lucy
-ONLINE aws_ionq_aria2 OFFLINE aws_rigetti_aspen_m3 ONLINE ibm_q_brisbane ONLINE
-... ``` You can get a Python list of device objects using: ```python from
-qbraid.providers import QbraidProvider provider = QbraidProvider() qdevices =
-provider.get_devices() ``` Or, instantiate a known device by ID via the
-`QbraidProvider.get_device()` method, and submit quantum jobs from any
-supported program type: ```python >>> from qbraid import get_jobs >>> from
-qbraid.providers import QbraidProvider >>> provider = QbraidProvider() >>>
-aws_device = provider.get_device("aws_oqc_lucy") >>> ibm_device =
-provider.get_device("ibm_q_brisbane") >>> aws_job = aws_device.run
-(qiskit_circuit, shots=1000) >>> ibm_job = ibm_device.run(cirq_circuit,
-shots=1000) >>> get_jobs() Displaying 2 most recent jobs: Job ID Submitted
-Status ------ --------- ------ aws_oqc_lucy-exampleuser-qjob-zzzzzzz... 2023-
-05-21T21:13:47.220Z QUEUED ibm_q_brisbane-exampleuser-qjob-xxxxxxx... 2023-05-
-21T21:13:48.220Z RUNNING ... ``` Compare results in a consistent, unified
-format: ```python >>> aws_result = aws_job.result() >>> ibm_result =
-ibm_job.result() >>> aws_result.measurement_counts() {'00': 483, '01': 14,
-'10': 486, '11': 17} >>> ibm_result.measurement_counts() {'00': 496, '01': 12,
-'10': 479, '11': 13} ``` ## Local account setup [api_key]To use the qBraid-SDK
+âââHâââX^0.5ââââââââ ``` Behind the scenes, the
+qBraid-SDK uses ``networkx`` to create a directional graph that maps all
+possible conversions between supported program types: ```python from
+qbraid.transpiler import ConversionGraph from qbraid.visualization import
+plot_conversion_graph graph = ConversionGraph() graph.plot() ```
+[conversion_graph]You can use the native conversions supported by qBraid, or
+define your own custom nodes and/or edges. For [example](https://github.com/
+qBraid/qbraid-qir?tab=readme-ov-file#add-qir-node-to-qbraid-conversion-graph):
+```python from qbraid_qir.qasm3 import qasm3_to_qir from qbraid.transpiler
+import Conversion conversion = Conversion("qasm3", "pyqir", qasm3_to_qir)
+graph.add_conversion(conversion) graph.plot() ``` ### QbraidProvider Run
+experiements using on-demand simulators provided by qBraid using the
+`qbraid.runtime.native.QbraidProvider`. You can get a Python list of device
+objects using: ```python from qbraid.runtime.native import QbraidProvider
+provider = QbraidProvider() qdevices = provider.get_devices() ``` Or,
+instantiate a known device by ID via the `QbraidProvider.get_device()` method,
+and submit quantum jobs from any supported program type: ```python device =
+provider.get_device("qbraid_qir_simulator") jobs = device.run([qiskit_circuit,
+braket_circuit, cirq_circuit, qasm3_str], shots=1000) results = [job.result()
+for job in jobs] print(results[0].measurement_counts()) # {'00': 483, '01': 14,
+'10': 486, '11': 17} ``` ## Local account setup [api_key]To use the qBraid-SDK
 locally (outside of qBraid Lab), you must add your account credentials: 1.
 Create a qBraid account or log in to your existing account by visiting
 [account.qbraid.com](https://account.qbraid.com/) 2. Copy your API Key token
-from the left side of your [account page](https://account.qbraid.com/): 3. Save
-your API key from step 2 by calling `QbraidSession.save_config()`: ```python
-from qbraid_core import QbraidSession session = QbraidSession
-(api_key='API_KEY') session.save_config() ``` The command above stores your
-credentials locally in a configuration file `~/.qbraid/qbraidrc`, where `~`
-corresponds to your home (`$HOME`) directory. Once saved, you can then connect
-to the qBraid API and leverage functions such as `get_devices()` and `get_jobs
-()`. ### Load Account from Environment Variables Alternatively, the qBraid-SDK
-can discover credentials from environment variables: ```shell export
-QBRAID_API_KEY='QBRAID_API_KEY' ``` Then instantiate the session without any
-arguments ```python from qbraid_core import QbraidSession session =
-QbraidSession() ``` ## Launch on qBraid The "Launch on qBraid" button (below)
-can be added to any public GitHub repository. Clicking on it automaically opens
-qBraid Lab, and performs a `git clone` of the project repo into your account's
-home directory. Copy the code below, and replace `YOUR-USERNAME` and `YOUR-
-REPOSITORY` with your GitHub info. [[https://qbraid-static.s3.amazonaws.com/
-logos/Launch_on_qBraid_white.png]](https://account.qbraid.com?gitHubUrl=https:/
-/github.com/qBraid/qBraid.git) Use the badge in your project's `README.md`:
-```markdown [[https://qbraid-static.s3.amazonaws.com/logos/
-Launch_on_qBraid_white.png]](https://account.qbraid.com?gitHubUrl=https://
-github.com/YOUR-USERNAME/YOUR-REPOSITORY.git) ``` Use the badge in your
-project's `README.rst`: ```rst .. image:: https://qbraid-
-static.s3.amazonaws.com/logos/Launch_on_qBraid_white.png :target: https://
+from the left side of your [account page](https://account.qbraid.com/): ###
+Save account to disk Once you have your API key from step 2 by, you can save it
+locally in a configuration file `~/.qbraid/qbraidrc`, where `~` corresponds to
+your home (`$HOME`) directory: | :warning: Account credentials are saved in
+plain text, so only do so if you are using a trusted device. | |:--------------
+-------------| ```python from qbraid.runtime.native import QbraidProvider
+provider = QbraidProvider(api_key='API_KEY') provider.save_config() ``` Once
+the account is saved on disk, you can instantiate the provider without any
+arguments: ```python from qbraid.runtime.native import QbraidProvider provider
+= QbraidProvider() ``` ### Load account from environment variables
+Alternatively, the qBraid-SDK can discover credentials from environment
+variables: ```shell export QBRAID_API_KEY='QBRAID_API_KEY' ``` ## Launch on
+qBraid The "Launch on qBraid" button (below) can be added to any public GitHub
+repository. Clicking on it automaically opens qBraid Lab, and performs a `git
+clone` of the project repo into your account's home directory. Copy the code
+below, and replace `YOUR-USERNAME` and `YOUR-REPOSITORY` with your GitHub info.
+[[https://qbraid-static.s3.amazonaws.com/logos/Launch_on_qBraid_white.png]]
+(https://account.qbraid.com?gitHubUrl=https://github.com/qBraid/qBraid.git) Use
+the badge in your project's `README.md`: ```markdown [[https://qbraid-
+static.s3.amazonaws.com/logos/Launch_on_qBraid_white.png]](https://
 account.qbraid.com?gitHubUrl=https://github.com/YOUR-USERNAME/YOUR-
-REPOSITORY.git :width: 150px ``` ## Contributing - Interested in contributing
-code, or making a PR? See [CONTRIBUTING.md](CONTRIBUTING.md) - For feature
-requests and bug reports: [Submit an issue](https://github.com/qBraid/qBraid/
-issues) - For discussions, and specific questions about the qBraid-SDK [join
-our discord community](https://discord.gg/TPBU2sa8Et) - For questions that are
-more suited for a forum, post to [Quantum Computing Stack Exchange](https://
-quantumcomputing.stackexchange.com/) with the [`qbraid`](https://
+REPOSITORY.git) ``` Use the badge in your project's `README.rst`: ```rst ..
+image:: https://qbraid-static.s3.amazonaws.com/logos/Launch_on_qBraid_white.png
+:target: https://account.qbraid.com?gitHubUrl=https://github.com/YOUR-USERNAME/
+YOUR-REPOSITORY.git :width: 150px ``` ## Contributing - Interested in
+contributing code, or making a PR? See [CONTRIBUTING.md](CONTRIBUTING.md) - For
+feature requests and bug reports: [Submit an issue](https://github.com/qBraid/
+qBraid/issues) - For discussions, and specific questions about the qBraid-SDK
+[join our discord community](https://discord.gg/TPBU2sa8Et) - For questions
+that are more suited for a forum, post to [Quantum Computing Stack Exchange]
+(https://quantumcomputing.stackexchange.com/) with the [`qbraid`](https://
 quantumcomputing.stackexchange.com/questions/tagged/qbraid) tag. ## License
 [GNU General Public License v3.0](LICENSE)
```

### Comparing `qbraid-0.7.0.dev20240423224133/docs/_static/cards/jupyter.png` & `qbraid-0.7.0.dev20240516020308/docs/_static/cards/jupyter.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240423224133/docs/_static/cards/python.png` & `qbraid-0.7.0.dev20240516020308/docs/_static/cards/python.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240423224133/docs/_static/cards/terminal.png` & `qbraid-0.7.0.dev20240516020308/docs/_static/cards/terminal.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240423224133/docs/_static/favicon.ico` & `qbraid-0.7.0.dev20240516020308/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240423224133/docs/_static/logo.png` & `qbraid-0.7.0.dev20240516020308/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240423224133/docs/_static/pkg-logos/braket.png` & `qbraid-0.7.0.dev20240516020308/docs/_static/pkg-logos/braket.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240423224133/docs/_static/pkg-logos/cirq.png` & `qbraid-0.7.0.dev20240516020308/docs/_static/pkg-logos/cirq.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240423224133/docs/_static/pkg-logos/pennylane.png` & `qbraid-0.7.0.dev20240516020308/docs/_static/pkg-logos/pennylane.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240423224133/docs/_static/pkg-logos/pyquil.png` & `qbraid-0.7.0.dev20240516020308/docs/_static/pkg-logos/pyquil.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240423224133/docs/_static/pkg-logos/qasm.png` & `qbraid-0.7.0.dev20240516020308/docs/_static/pkg-logos/qasm.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240423224133/docs/_static/pkg-logos/qir.png` & `qbraid-0.7.0.dev20240516020308/docs/_static/pkg-logos/qir.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240423224133/docs/_static/pkg-logos/qiskit.png` & `qbraid-0.7.0.dev20240516020308/docs/_static/pkg-logos/qiskit.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240423224133/docs/_static/pkg-logos/quantinuum.png` & `qbraid-0.7.0.dev20240516020308/docs/_static/pkg-logos/quantinuum.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240423224133/docs/_static/sdk-files/batch_counts.png` & `qbraid-0.7.0.dev20240516020308/docs/_static/sdk-files/batch_counts.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240423224133/docs/_static/sdk-files/conversion_graph.png` & `qbraid-0.7.0.dev20240516020308/docs/_static/sdk-files/conversion_graph.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240423224133/docs/_static/sdk-files/get_devices.png` & `qbraid-0.7.0.dev20240516020308/docs/_static/sdk-files/get_devices.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240423224133/docs/_static/sdk-files/hub_spokes.png` & `qbraid-0.7.0.dev20240516020308/docs/_static/sdk-files/hub_spokes.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240423224133/docs/_static/sdk-files/lab_jobs.png` & `qbraid-0.7.0.dev20240516020308/docs/_static/sdk-files/lab_jobs.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240423224133/docs/_static/sdk-files/plot_counts.png` & `qbraid-0.7.0.dev20240516020308/docs/_static/sdk-files/plot_counts.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240423224133/docs/conf.py` & `qbraid-0.7.0.dev20240516020308/docs/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,27 +6,20 @@
 
 # -- Path setup --------------------------------------------------------------
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
-import os
-import sys
-
 import qbraid
 
 # Set an environment variable to detect whether we are building the docs
 # so that we know to use raw imports instead of lazy loading.
 # os.environ['SPHINX_BUILD'] = '1'
 
-
-sys.path.insert(0, os.path.abspath(".."))
-sys.path.insert(0, os.path.abspath("../../qbraid"))
-
 # -- Project information -----------------------------------------------------
 
 project = "qBraid"
 copyright = "2024, qBraid Development Team"
 author = "qBraid Development Team"
 
 # The full version, including alpha/beta/rc tags
@@ -42,20 +35,21 @@
     "sphinx.ext.autodoc",
     "sphinx_autodoc_typehints",
     "sphinx.ext.autosummary",
     "sphinx.ext.todo",
     "sphinx.ext.mathjax",
     "sphinx.ext.coverage",
     "sphinx.ext.viewcode",
+    "sphinx_copybutton",
 ]
 
 # set_type_checking_flag = True
 autodoc_member_order = "bysource"
 autoclass_content = "both"
-autodoc_mock_imports = ["cirq", "braket", "qiskit", "pennylane", "pyquil", "pytket", "openqasm3", "numpy", "matplotlib", "matplotlib.pyplot"]
+autodoc_mock_imports = ["cirq", "braket", "qiskit", "pennylane", "pyquil", "pytket", "openqasm3", "numpy", "matplotlib", "matplotlib.pyplot", "stim", "qbraid_core"]
 napoleon_numpy_docstring = False
 todo_include_todos = True
 mathjax_path = "https://cdn.jsdelivr.net/npm/mathjax@2/MathJax.js?config=TeX-AMS-MML_HTMLorMML"
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
```

### Comparing `qbraid-0.7.0.dev20240423224133/docs/index.rst` & `qbraid-0.7.0.dev20240516020308/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
    :hidden:
 
    api/qbraid
    api/qbraid.programs
    api/qbraid.interface
    api/qbraid.transpiler
    api/qbraid.transforms
-   api/qbraid.providers
+   api/qbraid.runtime
    api/qbraid.visualization
 
 
 .. Indices and Tables
 .. ------------------
 
 .. * :ref:`genindex`
```

#### html2text {}

```diff
@@ -7,10 +7,10 @@
 _[_t_e_r_m_i_n_a_l_]
 _**_**_**_**_ _SS_DD_KK_ _**_**_**_**
 _[_t_e_r_m_i_n_a_l_]
 | .. toctree:: :maxdepth: 1 :caption: SDK User Guide :hidden: sdk/overview sdk/
 programs sdk/transpiler sdk/providers sdk/devices sdk/jobs sdk/results ..
 toctree:: :maxdepth: 1 :caption: SDK API Reference :hidden: api/qbraid api/
 qbraid.programs api/qbraid.interface api/qbraid.transpiler api/
-qbraid.transforms api/qbraid.providers api/qbraid.visualization .. Indices and
+qbraid.transforms api/qbraid.runtime api/qbraid.visualization .. Indices and
 Tables .. ------------------ .. * :ref:`genindex` .. * :ref:`modindex` .. * :
 ref:`search`
```

### Comparing `qbraid-0.7.0.dev20240423224133/docs/sdk/devices.rst` & `qbraid-0.7.0.dev20240516020308/docs/sdk/devices.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 Devices
 =========
 
 In this module, you will learn how to use the qBraid SDK to interface with
 quantum backends. We will demonstrate how to construct queries and search
 for available devices using the ``qbraid.get_devices`` function, and
-overview how to execute circuits using the ``qbraid.providers`` module.
+overview how to execute circuits using the ``qbraid.runtime`` module.
 
 Unified Device Search
 ----------------------
 
 The ``get_devices`` function provides a unified quantum device search. It returns a complete list
 of all quantum backends available through Qiskit, Cirq, and Amazon Braket, along with the "status" of
 each device, i.e. ``ONLINE`` or ``OFFLINE``.
@@ -103,20 +103,20 @@
 
 .. _Query Selectors: https://docs.mongodb.com/manual/reference/operator/query/#query-selectors
 
 
 Device Wrapper
 ----------------
 
-Given a ``qbraid_id`` retrieved from ``get_devices``, a ``qbraid.providers.QuantumDevice``
+Given a ``qbraid_id`` retrieved from ``get_devices``, a ``qbraid.runtime.QuantumDevice``
 object can be created as follows:
 
 .. code-block:: python
 
-    from qbraid.providers import QbraidProvider
+    from qbraid.runtime import QbraidProvider
 
     provider = QbraidProvider()
     qbraid_id = 'aws_oqc_lucy'  # as an example
 
     qdevice = provider.get_device(qbraid_id)
 
 
@@ -185,15 +185,15 @@
 
 In this section, we'll piece together a workflow example, starting by using the
 ``ibm_least_busy_qpu`` function to get the ``qbraid_id`` of the IBMQ QPU with the
 least number of queued quantum jobs.
 
 .. code-block:: python
 
-    >>> from qbraid.providers.ibm import ibm_least_busy_qpu
+    >>> from qbraid.runtime.qiskit import ibm_least_busy_qpu
     >>> qbraid_id = ibm_least_busy_qpu()
     >>> qdevice = provider.get_device(qbraid_id)
     >>> qdevice.name
     'Nairobi'
     >>> qdevice.status()
     <DeviceStatus.ONLINE: 0>
```

### Comparing `qbraid-0.7.0.dev20240423224133/docs/sdk/jobs.rst` & `qbraid-0.7.0.dev20240516020308/docs/sdk/jobs.rst`

 * *Files 4% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 
 The `device module <./devices.html>`_ illustrated how qBraid device wrappers can
 be used execute circuits on quantum backends. Using the OQC Lucy QPU as our example
 target backend, the procedure was as follows:
 
 .. code-block:: python
 
-    >>> from qbraid.providers import QbraidProvider
-    >>> qbraid_id = 'aws_oqc_lucy'
-    >>> provider = QbraidProvider()
-    >>> qdevice = provider.get_device(qbraid_id)
+    >>> from qbraid.runtime.braket import BraketProvider
+    >>> arn = 'arn:aws:braket:eu-west-2::device/qpu/oqc/Lucy'
+    >>> provider = BraketProvider()
+    >>> qdevice = provider.get_device(arn)
     >>> qjob = qdevice.run(circuit)
     >>> type(qjob)
-    qbraid.providers.aws.job.BraketQuantumTaskWrapper
+    qbraid.runtime.braket.job.BraketQuantumTask
 
 Invoking the ``run`` method of a qBraid ``QuantumDevice`` returns a qBraid
 ``QuantumJob``. Through a unified set of methods and attributes, this class
 provides access to data about the quantum jobs executed across any qBraid supported
 backend. You can also directly access the wrapped "job-like" object using the
 ``_job`` attribute.
 
@@ -85,34 +85,34 @@
 
     >>> from qbraid import get_jobs
     >>> get_jobs(filters={"qbraidDeviceId": "aws_oqc_lucy"})
     Displaying 10 most recent jobs matching query:
 
     Job ID                                                  Submitted                 Status
     ------                                                  ---------                 ------
-    aws_oqc_lucy-exampleuser-qjob-xxxxxxxxxxxxxxxxxxxx      2023-05-21T21:13:48.220Z  RUNNING
-    aws_oqc_lucy-exampleuser-qjob-yyyyyyyyyyyyyyyyyyyy      2023-04-15T11:09:56.783Z  COMPLETED
+    aws_oqc_lucy-exampleuser-qjob-xxxxxxxxxxxxxxxxxxxx      2024-05-21T21:13:48.220Z  RUNNING
+    aws_oqc_lucy-exampleuser-qjob-yyyyyyyyyyyyyyyyyyyy      2024-04-15T11:09:56.783Z  COMPLETED
     ...
 
 
 This job ID can be used to reinstantiate a qBraid ``QuantumJob`` object at any
 time, and even in a seperate program, with no loss of information.
 
 .. code-block:: python
 
-    >>> from qbraid.providers import QuantumJob
+    >>> from qbraid.runtime import QuantumJob
     >>> saved_job_id = 'aws_oqc_lucy-exampleuser-qjob-xxxxxxxxxxxxxxxxxxxx'
     >>> qjob = QuantumJob.retrieve(saved_job_id)
 
 
 You can also load a previously submitted jobs directly through the corresponding provider class:
 
 .. code-block:: python
 
-    >>> from qbraid.providers.aws import BraketQuantumTask
+    >>> from qbraid.runtime.braket import BraketQuantumTask
     >>> qjob = BraketQuantumTask(saved_job_id)
 
 
 Jobs submitted through the SDK are organized in the qBraid Lab Quantum Jobs Sidebar:
 
 .. image:: ../_static/sdk-files/lab_jobs.png
     :width: 90%
```

### Comparing `qbraid-0.7.0.dev20240423224133/docs/sdk/overview.rst` & `qbraid-0.7.0.dev20240516020308/docs/sdk/overview.rst`

 * *Files 2% similar despite different names*

```diff
@@ -56,17 +56,17 @@
 Usage
 ------
 
 Construct a quantum program of any supported program type:
 
 .. code-block:: python
    
-   >>> from qbraid.programs import QPROGRAM_LIBS
+   >>> from qbraid.programs import QPROGRAM_ALIASES
    >>> from qbraid.interface import random_circuit
-   >>> QPROGRAM_LIBS
+   >>> QPROGRAM_ALIASES
    ['cirq', 'qiskit', 'pyquil', 'pytket', 'braket', 'openqasm3', 'qasm2', 'qasm3']
    >>> circuit = random_circuit("qiskit", num_qubits=1, measure=True)
 
 Search for quantum backend(s) on which to execute your program:
 
 .. code-block:: python
 
@@ -84,15 +84,15 @@
    >>> ibm_least_busy_qpu()
    ibm_q_oslo
 
 Select a device using the ``QbraidProvider`` and send your quantum jobs:
 
 .. code-block:: python
 
-   >>> from qbraid.providers import QbraidProvider
+   >>> from qbraid.runtime import QbraidProvider
    >>> provider = QbraidProvider()
    >>> jobs  = []
    >>> qbraid_ids = ['aws_oqc_lucy', 'ibm_q_oslo']
    >>> for device in qbraid_ids:
    ... qdevice = provider.get_device(device)
    ... qjob = qdevice.run(circuit, shots=1000)
    ... jobs.append(qjob)
@@ -103,16 +103,16 @@
 
    >>> from qbraid import get_jobs
    >>> get_jobs(filters={"numResults": 2})
    Displaying 2 most recent jobs matching query:
 
    Job ID                                              Submitted                  Status
    ------                                              ---------                  ------
-   aws_oqc_lucy-exampleuser-qjob-zzzzzzz...            2023-05-21T21:13:47.220Z   QUEUED
-   ibm_q_oslo-exampleuser-qjob-xxxxxxx...              2023-05-21T21:13:48.220Z   RUNNING
+   aws_oqc_lucy-exampleuser-qjob-zzzzzzz...            2024-05-21T21:13:47.220Z   QUEUED
+   ibm_q_oslo-exampleuser-qjob-xxxxxxx...              2024-05-21T21:13:48.220Z   RUNNING
 
 Compare the results:
 
 .. code-block:: python
 
    >>> print("{:<20} {:<20}".format('Device','Counts'))
    ... for i, job in enumerate(jobs):
```

### Comparing `qbraid-0.7.0.dev20240423224133/docs/sdk/programs.rst` & `qbraid-0.7.0.dev20240516020308/docs/sdk/programs.rst`

 * *Files 6% similar despite different names*

```diff
@@ -87,36 +87,36 @@
     >>> type(qprogram.program)
     qiskit.circuit.quantumcircuit.QuantumCircuit
 
 
 Transpiler
 -----------
 
-Now, we can use the ``qbraid.programs.QuantumProgram.transpile`` method to convert to wrapped circuit into
-any other supported program type. Simply pass in the name of the target package from one of ``qbraid.programs.QPROGRAM_LIBS``.
+Now, we can use the ``qbraid.transpiler.transpile`` function to convert to a quantum program into
+any other supported program type. Simply pass in the name of the target package from one of ``qbraid.programs.QPROGRAM_ALIASES``.
 For example, use input "braket" to return a ``braket.circuits.Circuit``:
 
 .. code-block:: python
 
-    >>> braket_circuit = qprogram.transpile("braket")
+    >>> braket_circuit = transpile(qiskit_circuit, "braket")
     >>> print(braket_circuit)
     T  : |0|1|
             
     q0 : -H-C-
             |   
     q1 : ---X-
 
     T  : |0|1|
 
 
-This time, using the same origin circuit wrapper, we'll input ``"pyquil"`` to return a ``pyquil.quil.Program``:
+This time, using the same origin circuit, we'll input ``"pyquil"`` to return a ``pyquil.quil.Program``:
 
 .. code-block:: python
 
-    >>> pyquil_program = qprogram.transpile("pyquil")
+    >>> pyquil_program = transpile(qiskit_circuit, "pyquil")
     >>> print(pyquil_program)
     H 0
     CNOT 0 1
 
 
 Unitary calculations
 ----------------------
```

### Comparing `qbraid-0.7.0.dev20240423224133/docs/sdk/results.rst` & `qbraid-0.7.0.dev20240516020308/docs/sdk/results.rst`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 This time, we'll run our quantum program on the IBMQ Nairobi QPU. After the
 job has completed, we'll gather the result, print the measurement counts,
 and plot a histogram of the probabilities.
 
 .. code-block:: python
 
-    from qbraid.providers import QbraidProvider
+    from qbraid.runtime import QbraidProvider
     from qbraid.visualization import plot_histogram
 
     shots = 2**10
     
     provider = QbraidProvider()
     qdevice = provider.get_device('ibm_q_nairobi')
     qjob = ibmq_device.run(circuit, shots=shots)
@@ -48,15 +48,15 @@
 The results layer follows the same wrapper abstraction as the circuit, device
 and job layers. You can access the underlying "result-like" object using
 the ``_result`` attribute:
 
 .. code-block:: python
 
     >>> type(qresult_ibmq)
-    qbraid.providers.ibm.result.QiskitResult
+    qbraid.runtime.qiskit.result.QiskitResult
     >>> type(qresult_ibmq._result)
     qiskit.result.result.Result
 
 
 Now, let's run a batch job using two copies of the one-qubit qiskit circuit
 on a density-matrix simulator provided AWS:
```

### Comparing `qbraid-0.7.0.dev20240423224133/docs/sdk/transpiler.rst` & `qbraid-0.7.0.dev20240516020308/docs/sdk/transpiler.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240423224133/pyproject.toml` & `qbraid-0.7.0.dev20240516020308/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,81 +1,68 @@
 [build-system]
 requires = ["setuptools>=61", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qbraid"
 dynamic = ["version"]
-description = "A Python toolkit for cross-framework abstraction of quantum programs."
+description = "Platform-agnostic quantum runtime framework."
 readme = "README.md"
-authors = [{ name = "qBraid Development Team", email = "contact@qbraid.com" }]
-license = { file = "LICENSE" }
-keywords = ["qbraid", "quantum", "openqasm"]
+authors = [{name = "qBraid Development Team"}, {email = "contact@qbraid.com"}]
+license = {text = "GNU General Public License v3.0"}
+keywords = ["qbraid", "quantum", "openqasm", "runtime"]
 classifiers = [
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Natural Language :: English",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Physics"
 ]
 dependencies = [
     "networkx>=2.5,<4.0",
     "numpy>=1.17,<1.27",
     "openqasm3[parser]>=0.4.0,<0.6.0",
     "ply>=3.6",
-    "qbraid-core>=0.1.3,<0.2.0"
 ]
-requires-python = ">= 3.9"
+requires-python = ">=3.9,<3.13"
 
 [project.urls]
 Homepage = "https://www.qbraid.com/"
 Documentation = "https://docs.qbraid.com/en/stable/"
 "Source Code" = "https://github.com/qBraid/qBraid"
 "Bug Tracker" = "https://github.com/qBraid/qBraid/issues"
 Discord = "https://discord.gg/TPBU2sa8Et"
 "Launch on Lab" = "https://account.qbraid.com/?gitHubUrl=https://github.com/qBraid/qBraid.git"
 
 [project.optional-dependencies]
-braket = ["amazon-braket-sdk>=1.42.1,<1.79.0"]
-cirq = ["cirq-core>=1.3.0,<1.4.0"]
-pennylane = ["pennylane>=0.33.1,<0.36.0"]
-pytket = ["pytket>=1.16.0,<1.28.0"]
-pyquil = ["pyquil>=3.5.4,<4.4.0"]
-qir = ["qbraid-qir>=0.1.1,<0.2.0"]
-qiskit = ["qiskit>=0.44.0,<1.1.0", "qiskit-ibm-provider>=0.5.3,<0.11.0", "qiskit-ibm-runtime>=0.18.0,<0.21.0", "qiskit[visualization]"]
-ionq = ["cirq-core>=1.3.0,<1.4.0", "cirq-ionq>=1.3.0,<1.4.0", "pytket-braket>=0.30.0,<0.36.0"]
+braket = ["amazon-braket-sdk>=1.42.1,<1.80.0", "pytket-braket>=0.30.0,<0.37.0"]
+qiskit = ["qiskit>=0.44.0,<1.1.0", "qiskit-ibm-runtime>=0.18.0,<0.21.0"]
+runtime = ["qbraid-qir>=0.2.0", "qbraid-core>=0.1.6"]
 visualization = ["ipython", "matplotlib", "pylatexenc"]
 test = ["pytest", "pytest-cov"]
-lint = ["black", "isort", "pylint"]
-docs = ["sphinx>=7.2.6,<7.4.0", "sphinx-autodoc-typehints>=1.24,<2.2", "sphinx-rtd-theme>=1.3,<2.1", "docutils<0.22"]
+lint = ["black", "isort", "pylint", "qbraid-cli"]
+docs = ["sphinx>=7.2.6,<7.4.0", "sphinx-autodoc-typehints>=1.24,<2.2", "sphinx-rtd-theme>=1.3,<2.1", "docutils<0.22", "sphinx-copybutton"]
 
 [project.entry-points."qbraid.programs"]
 braket = "qbraid.programs.libs.braket:BraketCircuit"
 cirq = "qbraid.programs.libs.cirq:CirqCircuit"
 pennylane = "qbraid.programs.libs.pennylane:PennylaneTape"
 pyquil = "qbraid.programs.libs.pyquil:PyQuilProgram"
 qiskit = "qbraid.programs.libs.qiskit:QiskitCircuit"
 pytket = "qbraid.programs.libs.pytket:PytketCircuit"
 qasm2 = "qbraid.programs.libs.qasm2:OpenQasm2Program"
 qasm3 = "qbraid.programs.libs.qasm3:OpenQasm3Program"
 
-[project.entry-points."qbraid.providers"]
-"aws.device" = "qbraid.providers.aws:BraketDevice"
-"aws.job" = "qbraid.providers.aws:BraketQuantumTask"
-"aws.provider" = "qbraid.providers.aws:BraketProvider"
-"ibm.device" = "qbraid.providers.ibm:QiskitBackend"
-"ibm.job" = "qbraid.providers.ibm:QiskitJob"
-"ibm.provider" = "qbraid.providers.ibm:QiskitProvider"
-
 [tool.setuptools.dynamic]
 version = {attr = "qbraid._version.__version__"}
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 log_cli = false
 log_cli_level = "CRITICAL"
@@ -94,15 +81,14 @@
     "ignore::RuntimeWarning:numpy.linalg.linalg",
 ]
 
 [tool.coverage.run]
 parallel = true
 source = ["qbraid"]
 omit = [
-  "**/qbraid/transpiler/conversions/cirq/cirq_gates.py",
   "**/qbraid/visualization/plot_conversions.py",
   "**/qbraid/visualization/draw_circuit.py.py",
   "**/qbraid/_compat.py",
 ]
 
 [tool.coverage.paths]
 source = ["qbraid", ".tox/*/lib/python*/site-packages/qbraid"]
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/__init__.py` & `qbraid-0.7.0.dev20240516020308/qbraid/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
@@ -15,63 +15,53 @@
 
 Functions
 ----------
 
 .. autosummary::
    :toctree: ../stubs/
 
-   about
-   get_devices
-   get_jobs
-
-
-Classes
---------
-
-.. autosummary::
-   :toctree: ../stubs/
-
-   LazyLoader
-
+    about
+    configure_logging
+    filterwarnings
+    check_warn_version_update
 
 Exceptions
 -----------
 
 .. autosummary::
    :toctree: ../stubs/
 
    QbraidError
 
 """
 import sys
 
 from ._about import about
+from ._compat import check_warn_version_update, configure_logging, filterwarnings
 from ._import import LazyLoader
 from ._version import __version__
 from .exceptions import QbraidError
-from .get_devices import get_devices
-from .get_jobs import get_jobs
 
 if "sphinx" in sys.modules:
-    from . import interface, programs, providers, transforms, transpiler, visualization
+    from . import interface, programs, runtime, transforms, transpiler, visualization
 else:
     transforms = LazyLoader("transforms", globals(), "qbraid.transforms")
     interface = LazyLoader("interface", globals(), "qbraid.interface")
     programs = LazyLoader("programs", globals(), "qbraid.programs")
-    providers = LazyLoader("providers", globals(), "qbraid.providers")
+    runtime = LazyLoader("runtime", globals(), "qbraid.runtime")
     transpiler = LazyLoader("transpiler", globals(), "qbraid.transpiler")
     visualization = LazyLoader("visualization", globals(), "qbraid.visualization")
 
 
 __all__ = [
     "about",
-    "transforms",
-    "get_devices",
-    "get_jobs",
+    "configure_logging",
+    "check_warn_version_update",
+    "filterwarnings",
     "interface",
-    "LazyLoader",
     "programs",
-    "providers",
+    "runtime",
     "QbraidError",
+    "transforms",
     "transpiler",
     "visualization",
 ]
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/_about.py` & `qbraid-0.7.0.dev20240516020308/qbraid/_about.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,64 +6,66 @@
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """Information about qBraid and dependencies."""
 
+from ._compat import check_warn_version_update
+
 
 def about() -> None:
     """Displays information about qBraid, core/optional packages, and Python
     version/platform information.
     """
     # pylint: disable=import-outside-toplevel
     import platform
 
     from networkx import __version__ as networkx_version
     from numpy import __version__ as numpy_version
     from openqasm3 import __version__ as openqasm3_version
     from ply import __version__ as ply_version
-    from qbraid_core import __version__ as qbraid_core_version
 
     from ._version import __version__ as qbraid_version
 
     # Core dependencies
     core_dependencies = {
-        "qbraid_core": qbraid_core_version,
         "networkx": networkx_version,
         "openqasm3": openqasm3_version,
         "numpy": numpy_version,
         "ply": ply_version,
     }
 
     # Optional dependencies
     optional_packages = {
-        "pyquil": "pyquil",
-        "qiskit": "qiskit",
+        "qbraid_core": "qbraid_core",
+        "qbraid_qir": "qbraid_qir",
         "braket": "braket._sdk",
-        "pennylane": "pennylane",
         "cirq": "cirq",
+        "pyquil": "pyquil",
+        "pennylane": "pennylane",
         "pytket": "pytket",
-        "qiskit_ibm_provider": "qiskit_ibm_provider",
+        "qiskit": "qiskit",
         "qiskit_ibm_runtime": "qiskit_ibm_runtime",
-        "qbraid_qir": "qbraid_qir",
     }
 
+    check_warn_version = False
     optional_dependencies = {}
     for package_name, import_path in optional_packages.items():
         try:
             package = __import__(import_path, fromlist=[""])
             optional_dependencies[package_name] = package.__version__
+            check_warn_version = check_warn_version or package_name == "qbraid_core"
         except ImportError:
             continue
 
     about_str = (
-        "\nqBraid: A Python toolkit for cross-framework abstraction of quantum programs\n"
-        "==============================================================================\n"
-        f"Authored by: qBraid Development Team (https://github.com/qBraid/qBraid)\n\n"
+        "\nqBraid-SDK: A platform-agnostic quantum runtime framework\n"
+        "======================================================================\n"
+        f"(C) 2024 qBraid Development Team (https://github.com/qBraid/qBraid)\n\n"
         f"qbraid:\t{qbraid_version}\n\n"
         "Core Dependencies\n"
         "-----------------\n"
         + "\n".join([f"{k}: {v}" for k, v in core_dependencies.items()])
         + "\n\n"
         "Optional Dependencies\n"
         "---------------------\n"
@@ -75,7 +77,10 @@
         about_str += "None"
 
     about_str += (
         f"\n\nPython: {platform.python_version()}\n"
         f"Platform: {platform.system()} ({platform.machine()})"
     )
     print(about_str)
+
+    if check_warn_version:
+        check_warn_version_update()
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/_compat.py` & `qbraid-0.7.0.dev20240516020308/qbraid/_compat.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
@@ -12,15 +12,17 @@
 Module for emitting and configuring warnings and logging at top level.
 
 """
 import logging
 import os
 import warnings
 
-from qbraid_core._compat import check_version
+from ._import import LazyLoader
+
+qbraid_core = LazyLoader("qbraid_core", globals(), "qbraid_core")
 
 
 def configure_logging():
     """Configure logging to show warnings and errors."""
     level = os.getenv("LOG_LEVEL", "INFO").upper()  # Default to INFO if not set
     logging.basicConfig(
         level=getattr(logging, level, logging.INFO),
@@ -32,12 +34,17 @@
     """Filter out warnings that are not relevant to the user."""
     warnings.filterwarnings("ignore", category=SyntaxWarning)
     warnings.filterwarnings(
         "ignore", category=UserWarning, message="Setuptools is replacing distutils"
     )
     warnings.filterwarnings("ignore", category=DeprecationWarning)
     warnings.filterwarnings("ignore", category=RuntimeWarning, module="numpy")
+    warnings.filterwarnings(
+        "ignore",
+        message="networkx backend defined more than once: nx-loopback",
+        category=RuntimeWarning,
+    )
 
 
 def check_warn_version_update():
-    """Emit a warning if updated package version exists."""
-    check_version("qbraid")
+    """Emit a warning if updated qBraid-SDK package version exists."""
+    qbraid_core._compat.check_version("qbraid")
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/_import.py` & `qbraid-0.7.0.dev20240516020308/qbraid/_import.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/exceptions.py` & `qbraid-0.7.0.dev20240516020308/qbraid/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/interface/__init__.py` & `qbraid-0.7.0.dev20240516020308/qbraid/interface/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/interface/circuit_equality.py` & `qbraid-0.7.0.dev20240516020308/qbraid/interface/circuit_equality.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
 Module for calculating unitary of quantum circuit/program
 
 """
-from typing import TYPE_CHECKING, Tuple
+from typing import TYPE_CHECKING
 
 import numpy as np
 
 from qbraid.programs import load_program
 
 if TYPE_CHECKING:
     import qbraid
 
 
-def match_global_phase(a: np.ndarray, b: np.ndarray) -> Tuple[np.ndarray, np.ndarray]:
+def match_global_phase(a: np.ndarray, b: np.ndarray) -> tuple[np.ndarray, np.ndarray]:
     """
     Matches the global phase of two numpy arrays.
 
     This function aligns the global phases of two matrices by applying a phase shift based
     on the position of the largest entry in one matrix. It computes and adjusts for the
     phase difference at this position, resulting in two phase-aligned matrices. The output,
     (a', b'), indicates that a' == b' is equivalent to a == b * exp(i * t) for some phase t.
 
     Args:
         a (np.ndarray): The first input matrix.
         b (np.ndarray): The second input matrix.
 
     Returns:
-        Tuple[np.ndarray, np.ndarray]: A tuple of the two matrices `(a', b')`, adjusted for
+        tuple[np.ndarray, np.ndarray]: A tuple of the two matrices `(a', b')`, adjusted for
                                        global phase. If shapes of `a` and `b` do not match or
                                        either is empty, returns copies of the original matrices.
     """
     if a.shape != b.shape or a.size == 0:
         return np.copy(a), np.copy(b)
 
     k = max(np.ndindex(*a.shape), key=lambda t: abs(b[t]))
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/interface/random/__init__.py` & `qbraid-0.7.0.dev20240516020308/qbraid/interface/random/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/interface/random/cirq_random.py` & `qbraid-0.7.0.dev20240516020308/qbraid/interface/random/cirq_random.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/interface/random/qasm3_random.py` & `qbraid-0.7.0.dev20240516020308/qbraid/interface/random/qasm3_random.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/interface/random/qiskit_random.py` & `qbraid-0.7.0.dev20240516020308/qbraid/interface/random/qiskit_random.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/interface/random/random.py` & `qbraid-0.7.0.dev20240516020308/qbraid/interface/random/random.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
 Module for generate random quantum circuits used for testing
 
 """
-from typing import TYPE_CHECKING, Any, Callable, Dict, Optional, Tuple
+from typing import TYPE_CHECKING, Any, Callable, Optional
 
 import numpy as np
 
-from qbraid.programs._import import QPROGRAM, QPROGRAM_LIBS
 from qbraid.programs.exceptions import PackageValueError
+from qbraid.programs.registry import QPROGRAM, QPROGRAM_ALIASES
 from qbraid.transpiler.converter import transpile
 
-QROGRAM_TEST_TYPE = Tuple[Dict[str, Callable[[Any], QPROGRAM]], np.ndarray]
+QROGRAM_TEST_TYPE = tuple[dict[str, Callable[[Any], QPROGRAM]], np.ndarray]
 
 if TYPE_CHECKING:
     import qbraid.programs
 
 
 def random_circuit(
     package: str, num_qubits: Optional[int] = None, depth: Optional[int] = None, **kwargs
@@ -41,15 +41,15 @@
         PackageValueError: if ``package`` is not supported
         QbraidError: when invalid random circuit options given
 
     Returns:
         :data:`~qbraid.programs.QPROGRAM`: randomly generated quantum circuit/program
 
     """
-    if package not in QPROGRAM_LIBS:
+    if package not in QPROGRAM_ALIASES:
         raise PackageValueError(package)
 
     num_qubits = np.random.randint(1, 4) if num_qubits is None else num_qubits
     depth = np.random.randint(1, 4) if depth is None else depth
 
     # pylint: disable=import-outside-toplevel
     if package == "qasm3":
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/programs/exceptions.py` & `qbraid-0.7.0.dev20240516020308/qbraid/runtime/exceptions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,31 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
-Module defining exceptions for errors raised by qBraid.
+Module defining exceptions for errors raised while processing a device.
 
 """
-
 from qbraid.exceptions import QbraidError
 
-from ._import import QPROGRAM_LIBS
-
 
-class PackageValueError(QbraidError):
-    """Class for errors raised due to unsupported quantum frontend package"""
+class ProgramValidationError(QbraidError):
+    """Base class for errors raised while validating a quantum program."""
 
-    def __init__(self, package):
-        msg = (
-            f"Quantum frontend module '{package}' is not supported.\n"
-            f"Frontends supported by qBraid are: {QPROGRAM_LIBS}"
-        )
-        super().__init__(msg)
 
+class QbraidRuntimeError(QbraidError):
+    """Base class for errors raised while submitting a quantum job."""
 
-class ProgramTypeError(QbraidError):
-    """Class for errors raised when processing unsupported quantum programs"""
 
-    def __init__(self, program):
-        msg = f"Quantum program of type '{type(program)}' is not supported."
-        super().__init__(msg)
+class ResourceNotFoundError(QbraidError):
+    """Exception raised when the desired resource could not be found."""
 
 
-class QasmError(QbraidError):
-    """For errors raised while processing OpenQASM programs."""
+class JobStateError(QbraidError):
+    """Class for errors raised due to the state of a quantum job"""
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/programs/inspector.py` & `qbraid-0.7.0.dev20240516020308/qbraid/programs/exceptions.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,85 +1,57 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
-Module for performing QASM program checks before conversion
+Module defining exceptions for errors raised by qBraid.
 
 """
-from typing import TYPE_CHECKING, Optional
+from typing import Any, Optional
 
-from openqasm3.parser import QASM3ParsingError, parse
+from qbraid.exceptions import QbraidError
 
-from ._import import QPROGRAM_LIBS
-from .exceptions import PackageValueError, ProgramTypeError, QasmError
+from .registry import QPROGRAM_ALIASES
 
-if TYPE_CHECKING:
-    import qbraid.programs
 
+class PackageValueError(QbraidError):
+    """Class for errors raised due to unsupported quantum frontend package"""
 
-def get_qasm_version(qasm_str: str) -> str:
-    """Gets OpenQASM program version, either qasm2 or qasm3.
+    def __init__(self, package: str):
+        msg = (
+            f"Quantum frontend module '{package}' is not supported.\n"
+            f"Frontends supported by qBraid are: {QPROGRAM_ALIASES}"
+        )
+        super().__init__(msg)
 
-    Args:
-        qasm_str: An OpenQASM program string
 
-    Returns:
-        QASM version from list :obj:`~qbraid.programs.QPROGRAM_LIBS`
+class ProgramTypeError(QbraidError):
+    """Exception raised for errors encountered with unsupported quantum programs.
 
-    Raises:
-        :class:`~qbraid.programs.QasmError`: If string does not represent a valid OpenQASAM program.
-
-    """
-    qasm_str = qasm_str.replace("opaque", "// opaque")
-
-    try:
-        program = parse(qasm_str)
-        verion = int(float(program.version))
-        return f"qasm{verion}"
-    except QASM3ParsingError as err:
-        raise QasmError("Failed to parse OpenQASM program.") from err
-
-
-def get_program_type(
-    program: "qbraid.programs.QPROGRAM", require_supported: bool = True
-) -> Optional[str]:
+    Attributes:
+        program (Optional[Any]): The program that caused the error, default is None.
+        message (Optional[str]): Explanation of the error. If None, a default error message
+                                 is generated based on the provided program.
     """
-    Get the type of a quantum program.
 
-    Args:
-        program (qbraid.programs.QPROGRAM): The quantum program to get the type of.
-        require_supported (bool): If True, raise an error if the program type is not supported.
-
-    Returns:
-        str: The type of the quantum program, or None if the type cannot be determined and
-             require_supported is False.
-    """
-    if isinstance(program, str):
-        try:
-            package = get_qasm_version(program)
-        except QasmError as err:
-            if require_supported:
-                raise ProgramTypeError(
-                    "Input of type string must represent a valid OpenQASM program."
-                ) from err
-            package = None
-
-    else:
-        try:
-            program_module = program.__module__
-            package = program_module.split(".")[0].lower()
-        except AttributeError as err:
-            if require_supported:
-                raise ProgramTypeError(program) from err
-            package = None
+    def __init__(self, program: Optional[Any] = None, message: Optional[str] = None):
+        self.program = program
+        self.message = message
+        super().__init__(self.generate_message())
+
+    def generate_message(self) -> str:
+        """Generate an error message based on the input."""
+        if self.message is not None:
+            return self.message
+        if self.program is not None:
+            return f"Quantum program of type '{type(self.program)}' is not supported."
+        return "Unsupported quantum program type."
 
-    if package not in QPROGRAM_LIBS and require_supported:
-        raise PackageValueError(package)
 
-    return package
+class QasmError(QbraidError):
+    """For errors raised while processing OpenQASM programs."""
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/programs/libs/__init__.py` & `qbraid-0.7.0.dev20240516020308/qbraid/programs/libs/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,20 +29,20 @@
    qasm3
    qiskit
 
 """
 import importlib
 
 _qbraid = importlib.import_module("qbraid.programs._import")
-_PROGRAM_LIBS = getattr(_qbraid, "QPROGRAM_LIBS", [])
+NATIVE_REGISTRY = getattr(_qbraid, "NATIVE_REGISTRY", {})
 
 submodules = []
 base_path = "qbraid.programs.libs."
 
-for lib in _PROGRAM_LIBS:
+for lib in NATIVE_REGISTRY:
     try:
         imported_lib = importlib.import_module(base_path + lib)
         submodules.append(lib)
         globals()[lib] = imported_lib
 
     except ImportError:
         pass
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/programs/libs/braket.py` & `qbraid-0.7.0.dev20240516020308/qbraid/programs/libs/braket.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,45 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
 Module defining BraketCircuit Class
 
 """
-from typing import TYPE_CHECKING, List
+from typing import TYPE_CHECKING
 
 from braket.circuits import Circuit, Instruction, Qubit
 
-from qbraid.programs.abc_program import QuantumProgram
+from qbraid.programs.exceptions import ProgramTypeError
+from qbraid.programs.program import QbraidProgram
 
 if TYPE_CHECKING:
     import braket.circuits
     import numpy as np
 
 
-class BraketCircuit(QuantumProgram):
+class BraketCircuit(QbraidProgram):
     """Wrapper class for ``braket.circuits.Circuit`` objects."""
 
     def __init__(self, program: "braket.circuits.Circuit"):
         super().__init__(program)
+        if not isinstance(program, Circuit):
+            raise ProgramTypeError(
+                message=f"Expected 'braket.circuits.Circuit' object, got '{type(program)}'."
+            )
 
     @property
-    def program(self) -> Circuit:
-        return self._program
-
-    @program.setter
-    def program(self, value: Circuit) -> None:
-        if not isinstance(value, Circuit):
-            raise ValueError("Program must be an instance of braket.circuits.Circuit")
-        self._program = value
-
-    @property
-    def qubits(self) -> List[Qubit]:
+    def qubits(self) -> list[Qubit]:
         """Return the qubits acted upon by the operations in this circuit"""
         return list(self.program.qubits)
 
     @property
     def num_qubits(self) -> int:
         """Return the number of qubits in the circuit."""
         return self.program.qubit_count
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/programs/libs/cirq.py` & `qbraid-0.7.0.dev20240516020308/qbraid/programs/libs/cirq.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,48 +1,41 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
 Module defining CirqCircuit Class
 
 """
 
-from typing import List
-
 import cirq
 import numpy as np
 
-from qbraid.programs.abc_program import QuantumProgram
+from qbraid.programs.exceptions import ProgramTypeError
+from qbraid.programs.program import QbraidProgram
 
 
-class CirqCircuit(QuantumProgram):
+class CirqCircuit(QbraidProgram):
     """Wrapper class for ``cirq.Circuit`` objects."""
 
     def __init__(self, program: "cirq.Circuit"):
         super().__init__(program)
+        if not isinstance(program, cirq.Circuit):
+            raise ProgramTypeError(
+                message=f"Expected 'cirq.Circuit' object, got '{type(program)}'."
+            )
 
     @property
-    def program(self) -> cirq.Circuit:
-        return self._program
-
-    @program.setter
-    def program(self, value: cirq.Circuit) -> None:
-        if not isinstance(value, cirq.Circuit):
-            raise ValueError("Program must be an instance of cirq.Circuit")
-        self._program = value
-
-    @property
-    def qubits(self) -> List[cirq.Qid]:
+    def qubits(self) -> list[cirq.Qid]:
         """Return the qubits acted upon by the operations in this circuit"""
         return list(self.program.all_qubits())
 
     @property
     def num_clbits(self) -> int:
         """Return the number of classical bits in the circuit."""
         return 0
@@ -118,15 +111,15 @@
         else:
             raise ValueError(
                 "Expected qubit of type 'GridQubit' 'LineQubit' or 'NamedQubit'"
                 f"but instead got {type(qubit)}"
             )
 
     @staticmethod
-    def _make_qubits(qubits: List[cirq.Qid], targets: List[int]) -> List[cirq.Qid]:
+    def _make_qubits(qubits: list[cirq.Qid], targets: list[int]) -> list[cirq.Qid]:
         if len(set(type(qubit) for qubit in qubits)) > 1:
             # If mixed types, default to LineQubits
             qubit_type = cirq.LineQubit
         else:
             qubit_type = type(qubits[0])
 
         if qubit_type == cirq.LineQubit:
@@ -219,7 +212,26 @@
         """Rerverse qubit ordering of circuit."""
         qubits = self.qubits
         qubits.sort()
         qubits_rev = qubits.copy()
         qubits_rev.reverse()
         qubit_map = dict(zip(qubits, qubits_rev))
         self._program = self.program.transform_qubits(lambda q: qubit_map[q])
+
+    @staticmethod
+    def remove_measurements(circuit: cirq.Circuit) -> cirq.Circuit:
+        """Remove all measurement gates from the given Cirq circuit.
+
+        Args:
+            circuit (cirq.Circuit): The input circuit from which to remove measurement gates.
+
+        Returns:
+            cirq.Circuit: A new circuit with all measurement gates removed.
+        """
+        new_circuit = cirq.Circuit()
+        for mom in circuit:
+            filtered_operations = [
+                op for op in mom.operations if not isinstance(op.gate, cirq.MeasurementGate)
+            ]
+            if filtered_operations:
+                new_circuit.append(cirq.Moment(filtered_operations))
+        return new_circuit
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/programs/libs/pennylane.py` & `qbraid-0.7.0.dev20240516020308/qbraid/programs/libs/pennylane.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,45 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
 Module defining PennylaneTape Class
 
 """
-from typing import TYPE_CHECKING, List
+from typing import TYPE_CHECKING
 
 import pennylane as qml
 from pennylane.tape import QuantumTape
 
-from qbraid.programs.abc_program import QuantumProgram
+from qbraid.programs.exceptions import ProgramTypeError
+from qbraid.programs.program import QbraidProgram
 
 if TYPE_CHECKING:
     import numpy as np
 
 
-class PennylaneTape(QuantumProgram):
+class PennylaneTape(QbraidProgram):
     """Wrapper class for Pennylane Quantum Tape programs."""
 
     def __init__(self, program: QuantumTape):
         super().__init__(program)
+        if not isinstance(program, QuantumTape):
+            raise ProgramTypeError(
+                message=f"Expected 'pennylane.tape.QuantumTape' object, got '{type(program)}'."
+            )
 
     @property
-    def program(self) -> QuantumTape:
-        return self._program
-
-    @program.setter
-    def program(self, value: QuantumTape) -> None:
-        if not isinstance(value, QuantumTape):
-            raise ValueError("Program must be an instance of qml.tape.QuantumTape")
-        self._program = value
-
-    @property
-    def qubits(self) -> List[int]:
+    def qubits(self) -> list[int]:
         """Returns the wires of the quantum tape as a list of ints"""
         return self.program.wires.tolist()
 
     @property
     def num_clbits(self) -> int:
         """Return the number of classical bits in the tape."""
         return 0
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/programs/libs/pyquil.py` & `qbraid-0.7.0.dev20240516020308/qbraid/programs/libs/pyquil.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,60 +1,48 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
 Module defining PyQuilProgram Class
 
 """
 
-from typing import List
-
 import numpy as np
 import pyquil
 from pyquil import Program
 from pyquil.quilbase import Declare, Measurement
 from pyquil.simulation.tools import program_unitary
 
-from qbraid.programs.abc_program import QuantumProgram
+from qbraid.programs.exceptions import ProgramTypeError
+from qbraid.programs.program import QbraidProgram
 
 
-class PyQuilProgram(QuantumProgram):
+class PyQuilProgram(QbraidProgram):
     """Wrapper class for ``pyQuil.Program`` objects."""
 
     def __init__(self, program: "pyquil.Program"):
         super().__init__(program)
+        if not isinstance(program, Program):
+            raise ProgramTypeError(
+                message=f"Expected 'pyquil.Program' object, got '{type(program)}'."
+            )
 
     @property
-    def program(self) -> pyquil.Program:
-        return self._program
-
-    @program.setter
-    def program(self, value: pyquil.Program) -> None:
-        if not isinstance(value, pyquil.Program):
-            raise ValueError("Program must be an instance of pyquil.Program")
-        self._program = value
-
-    @property
-    def qubits(self) -> List[int]:
+    def qubits(self) -> list[int]:
         """Return the qubits acted upon by the operations in this circuit"""
         return list(self.program.get_qubits())
 
     @property
-    def num_qubits(self) -> int:
-        """Return the number of qubits in the circuit."""
-        return len(self.qubits)
-
-    @property
     def num_clbits(self) -> int:
         """Return the number of classical bits in the circuit."""
         return 0
 
     @property
     def depth(self) -> int:
         """Return the circuit depth (i.e., length of critical path)."""
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/programs/libs/pytket.py` & `qbraid-0.7.0.dev20240516020308/qbraid/programs/libs/pytket.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,47 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
 Module defining PytketCircuit Class
 
 """
 
-from typing import TYPE_CHECKING, List, Optional, Union
+from typing import TYPE_CHECKING, Optional, Union
 
 import numpy as np
-from pytket.circuit import Circuit, Command, OpType
+from pytket.circuit import Circuit, Command, OpType  # pylint: disable=no-name-in-module
 from pytket.unit_id import Qubit
 
-from qbraid.programs.abc_program import QuantumProgram
+from qbraid.programs.exceptions import ProgramTypeError
+from qbraid.programs.program import QbraidProgram
 
 if TYPE_CHECKING:
     import pytket
 
 
-class PytketCircuit(QuantumProgram):
+class PytketCircuit(QbraidProgram):
     """Wrapper class for ``pytket.circuit.Circuit`` objects."""
 
     def __init__(self, program: "pytket.Circuit"):
         super().__init__(program)
+        if not isinstance(program, Circuit):
+            raise ProgramTypeError(
+                message=f"Expected 'pytket.Circuit' object, got '{type(program)}'."
+            )
 
     @property
-    def program(self) -> Circuit:
-        return self._program
-
-    @program.setter
-    def program(self, value: Circuit) -> None:
-        if not isinstance(value, Circuit):
-            raise ValueError("Program must be an instance of pytket.circuit.Circuit")
-        self._program = value
-
-    @property
-    def qubits(self) -> List[Qubit]:
+    def qubits(self) -> list[Qubit]:
         """Return the qubits acted upon by the operations in this circuit"""
         return self.program.qubits
 
     @property
     def num_qubits(self) -> int:
         """Return the number of qubits in the circuit."""
         return self.program.n_qubits
@@ -114,15 +109,15 @@
                 np.array(gate_op.params) / np.pi if gate_op.params else gate_op.params,
                 circuit_qubits,
             )
         self._program = new_c
 
     @staticmethod
     def gate_to_matrix(
-        gates: Optional[Union[List[Circuit], Command]], flat: bool = False
+        gates: Optional[Union[list[Circuit], Command]], flat: bool = False
     ) -> np.ndarray:
         """Return the unitary of the Command"""
         gates = gates if (list == type(gates)) else [gates]
         a = list(map(max, [gate.qubits for gate in gates]))
         circuit = Circuit(max(a).index[0] + 1)
         for gate in gates:
             gate_op = gate.op
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/programs/libs/qasm2.py` & `qbraid-0.7.0.dev20240516020308/qbraid/programs/libs/qasm2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,40 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
 Module defining OpenQasm2Program Class
 
 """
 import re
-from typing import TYPE_CHECKING, List
+from typing import TYPE_CHECKING
 
-from qbraid.programs.abc_program import QuantumProgram
+from qbraid.programs.exceptions import ProgramTypeError
+from qbraid.programs.program import QbraidProgram
 
 if TYPE_CHECKING:
     import numpy as np
 
 
-class OpenQasm2Program(QuantumProgram):
+class OpenQasm2Program(QbraidProgram):
     """Wrapper class for OpenQASM 2 strings."""
 
     def __init__(self, program: str):
         super().__init__(program)
+        if not isinstance(program, str):
+            raise ProgramTypeError(message=f"Expected 'str' object, got '{type(program)}'.")
 
-    @property
-    def program(self) -> str:
-        return self._program
-
-    @program.setter
-    def program(self, value: str) -> None:
-        if not isinstance(value, str):
-            raise ValueError("Program must be an instance of str")
-        self._program = value
-
-    def _get_bits(self, bit_type: str) -> List[str]:
+    def _get_bits(self, bit_type: str) -> list[str]:
         """Return the number of qubits or classical bits in the circuit.
 
         Args:
             bit_type: either "q" or "c" for qubits or classical bits, respectively.
 
         """
         matches = re.findall(rf"{bit_type}reg (\w+)\[(\d+)\];", self.program)
@@ -51,15 +44,15 @@
             var_name = match[0]
             n = int(match[1])
             result.extend([f"{var_name}[{i}]" for i in range(n)])
 
         return result
 
     @property
-    def qubits(self) -> List[str]:
+    def qubits(self) -> list[str]:
         """Use regex to extract all qreg definitions from the string"""
         return self._get_bits("q")
 
     @property
     def num_clbits(self) -> int:
         """Return the number of classical bits in the circuit."""
         return self._get_bits("c")
@@ -148,15 +141,15 @@
                     track_measured[creg] = matches, max_depth + 1
 
         return self._get_max_count(depth_counts)
 
     def _unitary(self) -> "np.ndarray":
         """Return the unitary of the QASM"""
         # pylint: disable=import-outside-toplevel
-        from qbraid.transpiler.conversions.cirq.conversions_qasm import qasm2_to_cirq
+        from qbraid.transpiler.conversions.qasm2 import qasm2_to_cirq
 
         return qasm2_to_cirq(self.program).unitary()
 
     def remove_idle_qubits(self) -> None:
         """Checks whether the circuit uses contiguous qubits/indices,
         and if not, reduces dimension accordingly."""
         raise NotImplementedError
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/programs/libs/qasm3.py` & `qbraid-0.7.0.dev20240516020308/qbraid/programs/libs/qasm3.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
@@ -10,48 +10,41 @@
 
 """
 Module defining OpenQasm3Program Class
 
 """
 
 import re
-from typing import List, Optional, Tuple
+from typing import Optional
 
 import numpy as np
 from openqasm3.ast import BitType, ClassicalDeclaration, QubitDeclaration
 from openqasm3.parser import parse
 
-from qbraid.programs.abc_program import QuantumProgram
+from qbraid.programs.exceptions import ProgramTypeError
+from qbraid.programs.program import QbraidProgram
 
 
-class OpenQasm3Program(QuantumProgram):
+class OpenQasm3Program(QbraidProgram):
     """Wrapper class for OpenQASM 3 strings."""
 
     def __init__(self, program: str):
         super().__init__(program)
+        if not isinstance(program, str):
+            raise ProgramTypeError(message=f"Expected 'str' object, got '{type(program)}'.")
         self._parse_qasm()
 
-    @property
-    def program(self) -> str:
-        return self._program
-
-    @program.setter
-    def program(self, value: str) -> None:
-        if not isinstance(value, str):
-            raise ValueError("Program must be an instance of str")
-        self._program = value
-
     def _parse_qasm(self) -> str:
         """Process the program string."""
         program = parse(self._program)
 
         num_qubits = 0
         num_clbits = 0
-        qubits: List[Tuple[str, Optional[int]]] = []
-        clbits: List[Tuple[str, Optional[int]]] = []
+        qubits: list[tuple[str, Optional[int]]] = []
+        clbits: list[tuple[str, Optional[int]]] = []
 
         for statement in program.statements:
             if isinstance(statement, QubitDeclaration):
                 name = statement.qubit.name
                 size = None if statement.size is None else statement.size.value
                 qubits.append((name, size))
                 num_qubits += 1 if size is None else size
@@ -65,20 +58,20 @@
 
         self._num_qubits = num_qubits
         self._num_clbits = num_clbits
         self._qubits = qubits
         self._clbits = clbits
 
     @property
-    def qubits(self) -> List[Tuple[str, int]]:
+    def qubits(self) -> list[tuple[str, int]]:
         """Return the qubits acted upon by the operations in this circuit"""
         return self._qubits
 
     @property
-    def clbits(self) -> List[Tuple[str, int]]:
+    def clbits(self) -> list[tuple[str, int]]:
         """Return the qubits acted upon by the operations in this circuit"""
         return self._clbits
 
     @property
     def num_qubits(self) -> int:
         """Return the number of qubits in the circuit."""
         return self._num_qubits
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/programs/libs/qiskit.py` & `qbraid-0.7.0.dev20240516020308/qbraid/programs/libs/qiskit.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
@@ -10,45 +10,40 @@
 
 """
 Module defining QiskitCircuit Class
 
 """
 
 from collections import OrderedDict
-from typing import TYPE_CHECKING, List
+from typing import TYPE_CHECKING
 
 import qiskit
 from qiskit.circuit import Qubit
 from qiskit.converters import circuit_to_dag, dag_to_circuit
 from qiskit.quantum_info import Operator
 
-from qbraid.programs.abc_program import QuantumProgram
+from qbraid.programs.exceptions import ProgramTypeError
+from qbraid.programs.program import QbraidProgram
 
 if TYPE_CHECKING:
     import numpy as np
 
 
-class QiskitCircuit(QuantumProgram):
+class QiskitCircuit(QbraidProgram):
     """Wrapper class for ``qiskit.QuantumCircuit`` objects"""
 
     def __init__(self, program: "qiskit.QuantumCircuit"):
         super().__init__(program)
+        if not isinstance(program, qiskit.QuantumCircuit):
+            raise ProgramTypeError(
+                message=f"Expected 'qiskit.QuantumCircuit' object, got '{type(program)}'."
+            )
 
     @property
-    def program(self) -> qiskit.QuantumCircuit:
-        return self._program
-
-    @program.setter
-    def program(self, value: qiskit.QuantumCircuit) -> None:
-        if not isinstance(value, qiskit.QuantumCircuit):
-            raise ValueError("Program must be an instance of qiskit.QuantumCircuit")
-        self._program = value
-
-    @property
-    def qubits(self) -> List[Qubit]:
+    def qubits(self) -> list[Qubit]:
         """Return the qubits acted upon by the operations in this circuit"""
         return self.program.qubits
 
     @property
     def num_qubits(self) -> int:
         """Return the number of qubits in the circuit."""
         return self.program.num_qubits
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/programs/loader.py` & `qbraid-0.7.0.dev20240516020308/qbraid/programs/loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from typing import TYPE_CHECKING
 
 import openqasm3
 
 from qbraid._import import _load_entrypoint
 from qbraid.exceptions import QbraidError
 
-from .inspector import get_program_type
+from .alias_manager import get_program_type_alias
 
 if TYPE_CHECKING:
     import qbraid.programs
 
 
 def load_program(program: "qbraid.programs.QPROGRAM") -> "qbraid.programs.QuantumProgram":
     """Apply qbraid quantum program wrapper to a supported quantum program.
@@ -44,22 +44,17 @@
         :class:`~qbraid.QbraidError`: If the input circuit is not a supported quantum program.
 
     """
     if isinstance(program, openqasm3.ast.Program):
         program = openqasm3.dumps(program)
 
     try:
-        package = get_program_type(program)
+        package = get_program_type_alias(program)
     except QbraidError as err:
-        raise QbraidError(
-            f"Error applying circuit wrapper to quantum program \
-            of type {type(program)}"
-        ) from err
+        raise QbraidError(f"Error loading quantum program of type {type(program)}") from err
 
     try:
         load_program_class = _load_entrypoint("programs", package)
     except Exception as err:
-        raise QbraidError(
-            f"Error applying circuit wrapper to quantum program of type {type(program)}"
-        ) from err
+        raise QbraidError(f"Error loading quantum program of type {type(program)}") from err
 
     return load_program_class(program)
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/programs/qasm_passes.py` & `qbraid-0.7.0.dev20240516020308/qbraid/transforms/qasm2/passes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,26 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
 Module for preprocessing qasm string to before it is passed to parser.
 
 """
-import math
 import re
 
 from .qasm_qelib1 import decompose_qasm_qelib1
 
 
-def convert_qasm_pi_to_decimal(qasm_str: str) -> str:
-    """Convert all instances of 'pi' in the QASM string to their decimal value."""
-
-    pattern = r"(\d*\.?\d*\s*[*/+-]\s*)?pi(\s*[*/+-]\s*\d*\.?\d*)?"
-
-    def replace_with_decimal(match):
-        expr = match.group()
-        try:
-            value = eval(expr.replace("pi", str(math.pi)))  # pylint: disable=eval-used
-        except SyntaxError:
-            return expr
-        return str(value)
-
-    return re.sub(pattern, replace_with_decimal, qasm_str)
-
-
 def remove_qasm_barriers(qasm_str: str) -> str:
     """Returns a copy of the input QASM with all barriers removed.
 
     Args:
         qasm_str: QASM to remove barriers from.
     """
     quoted_re = r"(?:\"[^\"]*?\")"
@@ -75,14 +58,16 @@
 def unfold_qasm_gate_defs(qasm_string):
     """Recursively expands gate definitions in the input OpenQASM string."""
     # Define regular expression patterns
     gate_definition_pattern = re.compile(
         r"gate ([a-zA-Z0-9_]+)(\((.*?)\))? ((q[0-9]+,)*q[0-9]+) {(.*?)}"
     )
 
+    gate_body = ""
+    params_list = []
     gate_usage_match = None
 
     # Find gate definition and extract its components
     gate_definition_match = gate_definition_pattern.search(qasm_string)
     if gate_definition_match:
         gate_name, _, params, qubits, _, gate_body = gate_definition_match.groups()
         params_list = [param.strip() for param in params.split(",")] if params is not None else []
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/programs/qasm_qelib1.py` & `qbraid-0.7.0.dev20240516020308/qbraid/transforms/qasm2/qasm_qelib1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
@@ -11,15 +11,15 @@
 """
 Module that implements qelib1.inc qasm gate definitions as python functions
 
 """
 import re
 from typing import Optional
 
-from .exceptions import QasmError
+from qbraid.transforms.exceptions import DecompositionError
 
 
 def _get_param(instr: str) -> Optional[str]:
     try:
         return instr[instr.index("(") + 1 : instr.index(")")]
     except ValueError:
         return None
@@ -45,15 +45,15 @@
         instr = _remove_spaces_in_parentheses(instr)
         cu_gate, qs = instr.split(" ")
         a, b = qs.strip(";").split(",")
         params_lst = _get_param(cu_gate).split(",")
         params = [float(x) for x in params_lst]
         theta, phi, lam, gamma = params
     except (AttributeError, ValueError) as err:
-        raise QasmError from err
+        raise DecompositionError from err
     instr_out = "\n// cu gate\n"
     instr_out += f"p({gamma}) {a};\n"
     instr_out += f"p({(lam+phi)/2}) {a};\n"
     instr_out += f"p({(lam-phi)/2}) {b};\n"
     instr_out += f"cx {a},{b};\n"
     instr_out += f"u({-1*theta/2},0,{-1*(phi+lam)/2}) {b};\n"
     instr_out += f"cx {a},{b};\n"
@@ -65,15 +65,15 @@
     """two-qubit XX rotation"""
     try:
         instr = instr.replace(", ", ",")
         rxx_gate, qs = instr.split(" ")
         a, b = qs.strip(";").split(",")
         theta = _get_param(rxx_gate)
     except (AttributeError, ValueError) as err:
-        raise QasmError from err
+        raise DecompositionError from err
     instr_out = "\n// rxx gate\n"
     instr_out += f"h {a};\n"
     instr_out += f"h {b};\n"
     instr_out += f"cx {a},{b};\n"
     instr_out += f"rz({theta}) {b};\n"
     instr_out += f"cx {a},{b};\n"
     instr_out += f"h {b};\n"
@@ -83,15 +83,15 @@
 
 def _decompose_rccx_instr(instr: str) -> str:
     """relative-phase CCX"""
     try:
         _, qs = instr.split(" ")
         a, b, c = qs.strip(";").split(",")
     except (AttributeError, ValueError) as err:
-        raise QasmError from err
+        raise DecompositionError from err
     instr_out = "\n// rccx gate\n"
     instr_out += f"u2(0,pi) {c};\n"
     instr_out += f"u1(pi/4) {c};\n"
     instr_out += f"cx {b},{c};\n"
     instr_out += f"u1(-pi/4) {c};\n"
     instr_out += f"cx {a},{c};\n"
     instr_out += f"u1(pi/4) {c};\n"
@@ -103,15 +103,15 @@
 
 def _decompose_rc3x_instr(instr: str) -> str:
     """relative-phase 3-controlled X gate"""
     try:
         _, qs = instr.split(" ")
         a, b, c, d = qs.strip(";").split(",")
     except (AttributeError, ValueError) as err:
-        raise QasmError from err
+        raise DecompositionError from err
     instr_out = "\n// rc3x gate\n"
     instr_out += f"u2(0,pi) {d};\n"
     instr_out += f"u1(pi/4) {d};\n"
     instr_out += f"cx {c},{d};\n"
     instr_out += f"u1(-pi/4) {d};\n"
     instr_out += f"u2(0,pi) {d};\n"
     instr_out += f"cx {a},{d};\n"
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/providers/aws/__init__.py` & `qbraid-0.7.0.dev20240516020308/qbraid/runtime/braket/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
@@ -10,15 +10,15 @@
 
 # pylint: skip-file
 
 """
 Mdule submiting and managing quantm tasks through AWS
 and Amazon Braket supported devices.
 
-.. currentmodule:: qbraid.providers.aws
+.. currentmodule:: qbraid.runtime.braket
 
 Classes
 ---------
 
 .. autosummary::
    :toctree: ../stubs/
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/providers/aws/device.py` & `qbraid-0.7.0.dev20240516020308/qbraid/runtime/braket/device.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,98 +1,91 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
 Module defining BraketDeviceWrapper Class
 
 """
-import json
 from datetime import datetime, timedelta
-from typing import TYPE_CHECKING, Any, Dict, List, Tuple
+from typing import TYPE_CHECKING, Optional, Union
 
+import braket.circuits
+from braket.aws import AwsDevice
 from braket.device_schema import ExecutionDay
 
-from qbraid.programs._import import QPROGRAM_LIBS
-from qbraid.programs.libs.braket import BraketCircuit
-from qbraid.providers.device import QuantumDevice
-from qbraid.providers.enums import DeviceStatus, DeviceType
-from qbraid.transpiler import CircuitConversionError, ConversionPathNotFoundError, transpile
+from qbraid.runtime.device import QuantumDevice
+from qbraid.runtime.enums import DeviceStatus
+from qbraid.transforms.braket import transform
 
 from .job import BraketQuantumTask
 
 if TYPE_CHECKING:
     import braket.aws
-    import braket.circuits
 
-    import qbraid.providers.aws
+    import qbraid.runtime
+    import qbraid.runtime.braket
     import qbraid.transpiler
 
 
 def _future_utc_datetime(hours: int, minutes: int, seconds: int) -> str:
     """Return a UTC datetime that is hours, minutes, and seconds from now
     as an ISO string without fractional seconds."""
     current_utc = datetime.utcnow()
     future_time = current_utc + timedelta(hours=hours, minutes=minutes, seconds=seconds)
     return future_time.strftime("%Y-%m-%dT%H:%M:%SZ")
 
 
 class BraketDevice(QuantumDevice):
     """Wrapper class for Amazon Braket ``Device`` objects."""
 
-    def __init__(self, aws_device: "braket.aws.AwsDevice"):
+    def __init__(
+        self,
+        profile: "qbraid.runtime.TargetProfile",
+        session: "Optional[braket.aws.AwsSession]" = None,
+    ):
         """Create a BraketDevice."""
-
-        super().__init__(aws_device)
-        self._vendor = "AWS"
-        self._run_package = "braket"
-
-    def _populate_metadata(self, device: "braket.aws.AwsDevice") -> None:
-        """Populate device metadata using BraketSchemaBase"""
-        # pylint: disable=attribute-defined-outside-init
-        metadata = device.aws_session.get_device(device.arn)
-        capabilities = json.loads(metadata.get("deviceCapabilities"))
-
-        self._vendor_id = metadata.get("deviceArn")
-        self._name = metadata.get("deviceName")
-        self._provider = metadata.get("providerName")
-        self._device_type = DeviceType(metadata.get("deviceType"))
-
-        try:
-            self._num_qubits = capabilities["paradigm"]["qubitCount"]
-        except KeyError:
-            self._num_qubits = None
-
-    def status(self) -> "qbraid.providers.DeviceStatus":
-        """Return the status of this Device.
-
-        Returns:
-            The status of this Device
-        """
-        if self._device.is_available:
-            return DeviceStatus.ONLINE
+        super().__init__(profile=profile)
+        self._device = AwsDevice(arn=self.id, aws_session=session)
+        self._provider_name = self.profile.get("provider_name")
+
+    @property
+    def name(self) -> str:
+        """Return the name of this Device."""
+        return self._device.name
+
+    def __str__(self):
+        """Official string representation of QuantumDevice object."""
+        return f"{self.__class__.__name__}('{self._provider_name} {self.name}')"
+
+    def status(self) -> "qbraid.runtime.DeviceStatus":
+        """Return the status of this Device."""
+        if self._device.status == "ONLINE":
+            if self._device.is_available:
+                return DeviceStatus.ONLINE
+            return DeviceStatus.UNAVAILABLE
 
         if self._device.status == "RETIRED":
             return DeviceStatus.RETIRED
 
         return DeviceStatus.OFFLINE
 
-    def availability_window(self) -> Tuple[bool, str, str]:
+    def availability_window(self) -> tuple[bool, str, str]:
         """Provides device availability status. Indicates current availability,
         time remaining (hours, minutes, seconds) until next availability or
         unavailability, and future UTC datetime of next change in availability status.
 
         Returns:
-            Tuple[bool, str, str]: Current device availability, hr/min/sec until availability
+            tuple[bool, str, str]: Current device availability, hr/min/sec until availability
                                    switch, future UTC datetime of availability switch
         """
 
         is_available_result = False
         available_time = None
 
         device = self._device
@@ -148,14 +141,15 @@
             )
 
             if execution_window.executionDay in ordered_days:
                 day = (ordered_days.index(execution_window.executionDay) - weekday) % 6
 
             start_time = execution_window.windowStartHour
             end_time = current_time_utc
+            day_factor = 0
 
             if day == 0:
                 day_factor = day
             elif start_time.hour < end_time.hour:
                 day_factor = day - 1
             elif start_time.hour == end_time.hour:
                 if start_time.minute < end_time.minute:
@@ -198,79 +192,38 @@
             if isinstance(num_queued, str) and num_queued.startswith(">"):
                 num_queued = num_queued[1:]
             total_queued += int(num_queued)
         return total_queued
 
     def transform(self, run_input: "braket.circuits.Circuit") -> "braket.circuits.Circuit":
         """Transpile a circuit for the device."""
-        if self._device_type.name == "SIMULATOR":
-            program = BraketCircuit(run_input)
-            program.remove_idle_qubits()
-            run_input = program.program
-
-        if self.provider.lower() == "ionq" and "pytket" in QPROGRAM_LIBS:
-
-            # pylint: disable=import-outside-toplevel
-            from qbraid.transforms.pytket.ionq import pytket_ionq_transform
-
-            try:
-                tk_circuit = transpile(run_input, "pytket", max_path_depth=1)
-                tk_transformed = pytket_ionq_transform(tk_circuit)
-                run_input = transpile(tk_transformed, "braket", max_path_depth=1)
-            except (ConversionPathNotFoundError, CircuitConversionError):
-                pass
-
-        return run_input
+        return transform(run_input, device=self)
 
-    def _run(self, run_input: "braket.circuits.Circuit", *args, **kwargs) -> Dict[str, Any]:
+    def submit(
+        self,
+        run_input: Union[braket.circuits.Circuit, list[braket.circuits.Circuit]],
+        *args,
+        **kwargs,
+    ) -> Union[BraketQuantumTask, list[BraketQuantumTask]]:
         """Run a quantum task specification on this quantum device. Task must represent a
         quantum circuit, annealing problems not supported.
 
         Args:
             run_input: Specification of a task to run on device.
 
         Keyword Args:
             shots (int): The number of times to run the task on the device.
 
         Returns:
             The job like object for the run.
 
         """
-        aws_quantum_task = self._device.run(run_input, *args, **kwargs)
-        metadata = aws_quantum_task.metadata()
-        return {
-            "vendor_job_id": metadata["quantumTaskArn"],
-            "tags": metadata.get("tags", {}),
-            "shots": metadata.get("shots", 0),
-            "vendor_job_obj": aws_quantum_task,
-            "qbraid_job_obj": BraketQuantumTask,
-        }
-
-    def _run_batch(self, run_input, *args, **kwargs) -> List[Dict[str, Any]]:
-        """Run batch of quantum tasks on this quantum device.
-
-        Args:
-            run_input: A circuit object list to run on the wrapped device.
-
-        Keyword Args:
-            auto_compile (bool): Whether to compile the circuits for the device before running.
-            shots (int): The number of times to run the task on the device. Default is 1024.
-
-        Returns:
-            List of BraketQuantumTask objects for the run.
-
-        """
-        device = self._device
-        aws_quantum_task_batch = device.run_batch(run_input, *args, **kwargs)
-        aws_quantum_tasks = aws_quantum_task_batch.tasks
-        aws_quantum_task_data = []
-        for _, aws_quantum_task in enumerate(aws_quantum_tasks):
-            metadata = aws_quantum_task.metadata()
-            job_data = {
-                "vendor_job_id": metadata["quantumTaskArn"],
-                "tags": metadata.get("tags", {}),
-                "shots": metadata.get("shots", 0),
-                "vendor_job_obj": aws_quantum_task,
-                "qbraid_job_obj": BraketQuantumTask,
-            }
-            aws_quantum_task_data.append(job_data)
-        return aws_quantum_task_data
+        is_single_input = not isinstance(run_input, list)
+        run_input = [run_input] if is_single_input else run_input
+        aws_quantum_task_batch = self._device.run_batch(run_input, *args, **kwargs)
+        tasks = [
+            BraketQuantumTask(task.metadata()["quantumTaskArn"], task=task, device=self._device)
+            for task in aws_quantum_task_batch.tasks
+        ]
+        if is_single_input:
+            return tasks[0]
+        return tasks
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/providers/aws/job.py` & `qbraid-0.7.0.dev20240516020308/qbraid/runtime/braket/job.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
@@ -13,73 +13,84 @@
 
 """
 import logging
 from typing import Optional
 
 from braket.aws import AwsQuantumTask
 
-from qbraid.providers.enums import JOB_FINAL
-from qbraid.providers.exceptions import JobStateError
-from qbraid.providers.job import QuantumJob
+from qbraid.runtime.enums import JobStatus
+from qbraid.runtime.exceptions import JobStateError
+from qbraid.runtime.job import QuantumJob
 
 from .result import BraketGateModelResult
 from .tracker import get_quantum_task_cost
 
 logger = logging.getLogger(__name__)
 
+AWS_TASK_STATUS_MAP = {
+    "CREATED": JobStatus.INITIALIZING,
+    "QUEUED": JobStatus.QUEUED,
+    "RUNNING": JobStatus.RUNNING,
+    "CANCELLING": JobStatus.CANCELLING,
+    "CANCELLED": JobStatus.CANCELLED,
+    "COMPLETED": JobStatus.COMPLETED,
+    "FAILED": JobStatus.FAILED,
+}
+
 
 class AmazonBraketVersionError(Exception):
     """Exception raised for Amazon Braket SDK errors due to versioning."""
 
 
 class BraketQuantumTask(QuantumJob):
     """Wrapper class for Amazon Braket ``QuantumTask`` objects."""
 
-    def __init__(self, job_id: str, **kwargs):
+    def __init__(self, task_id: str, task: Optional[AwsQuantumTask] = None, **kwargs):
         """Create a BraketQuantumTask."""
 
-        super().__init__(job_id, **kwargs)
-
-    def _get_job(self):
-        """Return the job like object that is being wrapped."""
-        return AwsQuantumTask(self.vendor_job_id)
+        super().__init__(task_id, **kwargs)
+        self._task = task or AwsQuantumTask(task_id)
 
-    def _get_status(self):
+    def status(self):
         """Returns status from Braket QuantumTask object metadata."""
-        return self._job.state()
+        state = self._task.state()
+        status = AWS_TASK_STATUS_MAP.get(state, JobStatus.UNKNOWN)
+        self._cache_metadata["status"] = status
+        return status
 
     def queue_position(self) -> Optional[int]:
         """Returns queue position from Braket QuantumTask.
         '>2000' returns as 2000 for typing consistency."""
         try:
-            position = self._job.queue_position().queue_position
+            position = self._task.queue_position().queue_position
             if isinstance(position, str):
                 if position.startswith(">"):
                     position = position[1:]
                 return int(position)
             return position
         except AttributeError as err:
             raise AmazonBraketVersionError(
                 "Queue visibility is only available for amazon-braket-sdk>=1.56.0"
             ) from err
 
     def result(self) -> BraketGateModelResult:
         """Return the results of the job."""
-        if self.status() not in JOB_FINAL:
+        if not self.is_terminal_state():
             logger.info("Result will be available when job has reached final state.")
-        return BraketGateModelResult(self._job.result())
+        return BraketGateModelResult(self._task.result())
 
     def cancel(self) -> None:
         """Cancel the quantum task."""
-        task = self._job
-        status = self.status()
-        if status in JOB_FINAL:
-            raise JobStateError(f"Cannot cancel quantum job in the {status} state.")
+        task = self._task
+
+        if self.is_terminal_state():
+            raise JobStateError("Cannot cancel quantum job in terminal state.")
+
         try:
             task.cancel()
         except RuntimeError:
             task._aws_session.cancel_quantum_task(task.arn)
 
     def get_cost(self) -> float:
         """Return the cost of the job."""
-        decimal_cost = get_quantum_task_cost(self.vendor_job_id)
+        decimal_cost = get_quantum_task_cost(self._task.arn)
         return float(decimal_cost)
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/providers/aws/provider.py` & `qbraid-0.7.0.dev20240516020308/qbraid/runtime/braket/provider.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,63 +1,84 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
 Module for configuring provider credentials and authentication.
 
 """
 
+import json
 import os
-from typing import TYPE_CHECKING, List, Optional
+from typing import TYPE_CHECKING, Optional
 
 import boto3
+import braket.circuits
 from boto3.session import Session
 from braket.aws import AwsDevice, AwsSession
 from qbraid_core.services.quantum import quantum_lib_proxy_state
+from qbraid_core.services.quantum.proxy_braket import aws_configure
 
 from qbraid.exceptions import QbraidError
-from qbraid.providers.provider import QuantumProvider
+from qbraid.programs import ProgramSpec
+from qbraid.runtime import DeviceType, QuantumProvider, TargetProfile
+
+from .device import BraketDevice
 
 if TYPE_CHECKING:
     import braket.aws
 
+    import qbraid.runtime.braket
+
 
 class BraketProvider(QuantumProvider):
     """
     This class is responsible for managing the interactions and
     authentications with the AWS services.
 
     Attributes:
         aws_access_key_id (str): AWS access key ID for authenticating with AWS services.
         aws_secret_access_key (str): AWS secret access key for authenticating with AWS services.
     """
 
     REGIONS = ("us-east-1", "us-west-1", "us-west-2", "eu-west-2")
 
-    def __init__(self, aws_access_key_id=None, aws_secret_access_key=None):
+    def __init__(
+        self, aws_access_key_id: Optional[str] = None, aws_secret_access_key: Optional[str] = None
+    ):
         """
         Initializes the QbraidProvider object with optional AWS credentials.
 
         Args:
             aws_access_key_id (str, optional): AWS access key ID. Defaults to None.
             aws_secret_access_key (str, optional): AWS secret access token. Defaults to None.
         """
         self.aws_access_key_id = aws_access_key_id or os.getenv("AWS_ACCESS_KEY_ID")
         self.aws_secret_access_key = aws_secret_access_key or os.getenv("AWS_SECRET_ACCESS_KEY")
 
-    def save_config(self):
+    def save_config(
+        self,
+        aws_access_key_id: Optional[str] = None,
+        aws_secret_access_key: Optional[str] = None,
+        **kwargs,
+    ):
         """Save the current configuration."""
-        raise NotImplementedError
+        aws_access_key_id = aws_access_key_id or self.aws_access_key_id
+        aws_secret_access_key = aws_secret_access_key or self.aws_secret_access_key
+        aws_configure(
+            aws_access_key_id=aws_access_key_id,
+            aws_secret_access_key=aws_secret_access_key,
+            **kwargs,
+        )
 
     @staticmethod
     def _get_default_region() -> str:
         """Returns the default AWS region."""
         try:
             session = Session()
             return session.region_name
@@ -69,73 +90,103 @@
         """Return name of the default bucket to use in the AWS Session"""
         try:
             aws_session = AwsSession()
             return aws_session.default_bucket()
         except Exception:  # pylint: disable=broad-exception-caught
             return "amazon-braket-qbraid-provider"
 
-    def _get_region_name(self, device_arn: str) -> str:
-        """Returns the AWS region name."""
-        maybe_region = device_arn.split(":")[3]
-        if maybe_region in self.REGIONS:
-            return maybe_region
-
-        provider = device_arn.split("/")[-2]
-        if provider in ["ionq", "quera", "xanadu"]:
-            return "us-east-1"
-        if provider == "oqc":
-            return "eu-west-2"
-        if provider == "rigetti":
-            return "us-west-1"
-
-        return self._get_default_region()
-
     def _get_aws_session(self, region_name: Optional[str] = None) -> "braket.aws.AwsSession":
         """Returns the AwsSession provider."""
         region_name = region_name or self._get_default_region()
         default_bucket = self._get_s3_default_bucket()
 
         boto_session = Session(
             region_name=region_name,
             aws_access_key_id=self.aws_access_key_id,
             aws_secret_access_key=self.aws_secret_access_key,
         )
         return AwsSession(boto_session=boto_session, default_bucket=default_bucket)
 
+    def _build_runtime_profile(
+        self, device: "braket.aws.AwsDevice", program_spec: Optional[ProgramSpec] = None
+    ) -> TargetProfile:
+        """Returns the runtime profile for the device."""
+        metadata = device.aws_session.get_device(device.arn)
+        provider_name = metadata.get("providerName")
+        capabilities = json.loads(metadata.get("deviceCapabilities"))
+        action = capabilities.get("action", {})
+        supported = action.get("braket.ir.openqasm.program") is not None
+        if not supported:
+            raise QbraidError(
+                f"TargetProfile cannot be created for device '{device.arn}' as it does not "
+                f"support 'braket.ir.openqasm.program' program types. Please verify device "
+                f"capabilities or select a different, compatible device."
+            )
+        device_type = DeviceType(metadata.get("deviceType"))
+        num_qubits = capabilities.get("paradigm", {}).get("qubitCount")
+        program_spec = program_spec or ProgramSpec(braket.circuits.Circuit)
+        return TargetProfile(
+            device_type=device_type,
+            num_qubits=num_qubits,
+            program_spec=program_spec,
+            provider_name=provider_name,
+            device_id=device.arn,
+        )
+
     def get_devices(
-        self, aws_session=None, statuses=None, **kwargs
-    ) -> List["braket.aws.AwsDevice"]:
+        self,
+        aws_session: "Optional[braket.aws.AwsSession]" = None,
+        statuses: Optional[list[str]] = None,
+        **kwargs,
+    ) -> list["qbraid.runtime.braket.BraketDevice"]:
         """Return a list of backends matching the specified filtering."""
         aws_session = self._get_aws_session() if aws_session is None else aws_session
         statuses = ["ONLINE", "OFFLINE"] if statuses is None else statuses
+        aws_devices = AwsDevice.get_devices(aws_session=aws_session, statuses=statuses, **kwargs)
+        qasm_spec = ProgramSpec(braket.circuits.Circuit)
+        return [
+            BraketDevice(
+                profile=self._build_runtime_profile(device, program_spec=qasm_spec),
+                session=device.aws_session,
+            )
+            for device in aws_devices
+            if device._provider_name in ["Rigetti", "IonQ", "Oxford", "Amazon Braket"]
+        ]
 
-        return AwsDevice.get_devices(aws_session=aws_session, statuses=statuses, **kwargs)
-
-    def get_device(self, device_id: str) -> "braket.aws.AwsDevice":
+    def get_device(self, device_id: str) -> "qbraid.runtime.braket.BraketDevice":
         """Returns the AWS device."""
-        region_name = self._get_region_name(device_id)  # deviceArn
+        try:
+            region_name = device_id.split(":")[3]
+        except IndexError as err:
+            raise ValueError(
+                f"Device ARN is not a valid format: {device_id}. For valid Braket ARNs, "
+                "see 'https://docs.aws.amazon.com/braket/latest/developerguide/braket-devices.html'"
+            ) from err
         aws_session = self._get_aws_session(region_name=region_name)
-        return AwsDevice(arn=device_id, aws_session=aws_session)
+        device = AwsDevice(arn=device_id, aws_session=aws_session)
+        program_spec = ProgramSpec(braket.circuits.Circuit)
+        profile = self._build_runtime_profile(device, program_spec=program_spec)
+        return BraketDevice(profile=profile, session=device.aws_session)
 
     def get_tasks_by_tag(
-        self, key: str, values: Optional[List[str]] = None, region_names: Optional[List[str]] = None
-    ) -> List[str]:
+        self, key: str, values: Optional[list[str]] = None, region_names: Optional[list[str]] = None
+    ) -> list[str]:
         """
         Retrieves a list of quantum task ARNs that match the specified tag keys or key/value pairs.
 
         Args:
             key (str): The tag key to match.
-            values (Optional[List[str]]): A list of tag values to match against the provided
+            values (Optional[list[str]]): A list of tag values to match against the provided
                                           key. If None, tasks with the specified key,
                                           regardless of its value, are matched.
-            region_names (Optional[List[str]]): A list of region names to search. If None, all
+            region_names (Optional[list[str]]): A list of region names to search. If None, all
                                                 regions in `self.REGIONS` are searched.
 
         Returns:
-            List[str]: A list of ARNs for quantum tasks that match the given tag criteria.
+            list[str]: A list of ARNs for quantum tasks that match the given tag criteria.
 
         Raises:
             QbraidError: If the function is called within a qBraid quantum job environment
                          where AWS S3 requests are not supported.
         """
         try:
             jobs_state = quantum_lib_proxy_state("braket")
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/providers/aws/result.py` & `qbraid-0.7.0.dev20240516020308/qbraid/runtime/braket/result.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
@@ -10,15 +10,15 @@
 
 """
 Module defining BraketGateModelResult Class
 
 """
 import numpy as np
 
-from qbraid.providers.result import QuantumJobResult
+from qbraid.runtime.result import QuantumJobResult
 
 
 class BraketGateModelResult(QuantumJobResult):
     """Wrapper class for Amazon Braket result objects."""
 
     def measurements(self):
         """2d array - row is shot and column is qubit. Default is None. Only available when
@@ -26,15 +26,15 @@
         `GateModelQuantumTaskResult.measured_qubits`.
 
         TODO: Make doc-string consistent with parent.
 
         """
         return np.flip(self._result.measurements, 1)
 
-    def raw_counts(self):
+    def raw_counts(self, **kwargs):
         """Returns the histogram data of the run"""
         braket_counts = dict(self._result.measurement_counts)
         qbraid_counts = {}
         for key in braket_counts:
             str_key = "".join(reversed([str(i) for i in key]))
             qbraid_counts[str_key] = braket_counts[key]
         return qbraid_counts
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/providers/aws/tracker.py` & `qbraid-0.7.0.dev20240516020308/qbraid/runtime/braket/tracker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
 Module for interfacing with the Amazon Braket cost tracker
 
 """
 from decimal import Decimal
-from typing import Any, Dict, Optional
+from typing import Any, Optional
 
 from boto3.session import Session
 from braket.aws import AwsDevice, AwsQuantumTask, AwsSession
 from braket.tracking.tracker import Tracker, _get_qpu_task_cost, _get_simulator_task_cost
 from braket.tracking.tracking_context import register_tracker
 from braket.tracking.tracking_events import _TaskCompletionEvent, _TaskCreationEvent
 
 
-def _generate_creation_event(boto_data: Dict[str, Any]) -> _TaskCreationEvent:
+def _generate_creation_event(boto_data: dict[str, Any]) -> _TaskCreationEvent:
     """Generate a task creation event."""
     job_token = boto_data.pop("jobToken", None)
     return _TaskCreationEvent(
         arn=boto_data["quantumTaskArn"],
         shots=boto_data["shots"],
         is_job_task=(job_token is not None),
         device=boto_data["deviceArn"],
     )
 
 
 def _generate_completion_event(
-    boto_data: Dict[str, Any], aws_session: Optional[AwsSession] = None
+    boto_data: dict[str, Any], aws_session: Optional[AwsSession] = None
 ) -> _TaskCompletionEvent:
     """Generate a task completion event."""
     task_arn = boto_data["quantumTaskArn"]
     result = AwsQuantumTask(task_arn, aws_session=aws_session).result()
     execution_duration = None
     try:
         execution_duration = result.additional_metadata.simulatorMetadata.executionDuration
@@ -50,16 +50,16 @@
         "status": boto_data["status"],
         "execution_duration": execution_duration,
     }
     return _TaskCompletionEvent(**completion_data)
 
 
 def _get_tracker_task_details(
-    boto_data: Dict[str, Any], aws_session: Optional[AwsSession] = None
-) -> Dict[str, Any]:
+    boto_data: dict[str, Any], aws_session: Optional[AwsSession] = None
+) -> dict[str, Any]:
     """Get the quantum task details populated by the Amazon Braket cost tracker."""
     tracker = Tracker()
     register_tracker(tracker)
     creation_event = _generate_creation_event(boto_data)
     completion_event = _generate_completion_event(boto_data, aws_session=aws_session)
     tracker.receive_event(creation_event)
     tracker.receive_event(completion_event)
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/providers/enums.py` & `qbraid-0.7.0.dev20240516020308/qbraid/runtime/enums.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,75 +1,77 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
-Module defining all :mod:`~qbraid.providers` enumerated types.
+Module defining all :mod:`~qbraid.runtime` enumerated types.
 
 """
 from enum import Enum
 
 
 class DeviceType(str, Enum):
-    """Class for possible device types.
+    """
+    Enumeration for different types of quantum computing devices.
 
     Attributes:
-        SIMULATOR (str): the device is a simulator
-        QPU (str): the device is a QPU
-        FAKE (str): is a fake device used for testing
-
+        QPU (str): A Quantum Processing Unit (QPU) hardware device located remotely.
+        SIMULATOR (str): A simulator that runs on remote servers.
+        LOCAL_SIMULATOR (str): A simulator that runs locally on the user's machine.
     """
 
-    SIMULATOR = "SIMULATOR"
     QPU = "QPU"
-    FAKE = "FAKE"
+    SIMULATOR = "SIMULATOR"
+    LOCAL_SIMULATOR = "LOCAL_SIMULATOR"
 
 
-class DeviceStatus(int, Enum):
-    """Class for the status of devices.
+class DeviceStatus(str, Enum):
+    """Enumeration for representing various operational statuses of devices.
 
     Attributes:
-        ONLINE (int): the device is online
-        OFFLINE (int): the device is offline
-
+        ONLINE (str): Device is online and accepting jobs.
+        UNAVAILABLE (str): Device is online but not accepting jobs.
+        OFFLINE (str): Device is offline.
+        RETIRED (str): Device has been retired and is no longer operational.
     """
 
-    ONLINE = 0
-    OFFLINE = 1
-    RETIRED = 2
+    ONLINE = "online"
+    UNAVAILABLE = "unavailable"
+    OFFLINE = "offline"
+    RETIRED = "retired"
 
 
 class JobStatus(str, Enum):
     """Class for the status of processes (i.e. jobs / quantum tasks) resulting from any
-    :meth:`~qbraid.providers.QuantumDevice.run` method.
+    :meth:`~qbraid.runtime.QuantumDevice.run` method.
 
     Attributes:
         INITIALIZING (str): job is being initialized
         QUEUED (str): job is queued
         VALIDATING (str): job is being validated
         RUNNING (str): job is actively running
         CANCELLING (str): job is being cancelled
         CANCELLED (str): job has been cancelled
         COMPLETED (str): job has successfully run
         FAILED (str): job failed / incurred error
-        UNKNOWN (str): vendor-supplied job status not recognized
+        UNKNOWN (str): job status is unknown/undetermined
 
     """
 
     INITIALIZING = "job is being initialized"
     QUEUED = "job is queued"
     VALIDATING = "job is being validated"
     RUNNING = "job is actively running"
     CANCELLING = "job is being cancelled"
     CANCELLED = "job has been cancelled"
     COMPLETED = "job has successfully run"
     FAILED = "job failed / incurred error"
-    UNKNOWN = "vendor-supplied job status not recognized"
+    UNKNOWN = "job status is unknown/undetermined"
 
 
-JOB_FINAL = (JobStatus.COMPLETED, JobStatus.CANCELLED, JobStatus.FAILED)
+JOB_STATUS_FINAL = (JobStatus.COMPLETED, JobStatus.CANCELLED, JobStatus.FAILED)
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/providers/exceptions.py` & `qbraid-0.7.0.dev20240516020308/qbraid/transforms/exceptions.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,28 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
-Module defining exceptions for errors raised while processing a device.
+Module defining exceptions for errors raised by qBraid transforms.
 
 """
-from qbraid.exceptions import QbraidError
-
-
-class ProgramValidationError(QbraidError):
-    """Base class for errors raised while validating a quantum program."""
 
-
-class QbraidRuntimeError(QbraidError):
-    """Base class for errors raised while submitting a quantum job."""
+from qbraid.exceptions import QbraidError
 
 
-class ResourceNotFoundError(QbraidError):
-    """Exception raised when the desired resource could not be found."""
+class TransformError(QbraidError):
+    """Base class for errors raised during qBraid transform processes."""
 
 
-class JobError(QbraidError):
-    """Base class for errors raised by Jobs."""
+class CompilationError(TransformError):
+    """Base class for errors raised during circuit compilation processes."""
 
 
-class JobStateError(JobError):
-    """Class for errors raised due to the state of a quantum job"""
+class DecompositionError(TransformError):
+    """For errors raised during circuit decomposition processes."""
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/providers/ibm/__init__.py` & `qbraid-0.7.0.dev20240516020308/qbraid/runtime/qiskit/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,33 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 # pylint: skip-file
 
 """
 Mdule submiting and managing jobs through IBM and IBM backends.
 
-.. currentmodule:: qbraid.providers.ibm
+.. currentmodule:: qbraid.runtime.qiskit
 
 Classes
 --------
 
 .. autosummary::
    :toctree: ../stubs/
 
    QiskitBackend
    QiskitJob
-   QiskitRemoteService
-   QiskitProvider
-   QiskitRuntime
+   QiskitRuntimeProvider
    QiskitResult
 
 """
 from .device import QiskitBackend
 from .job import QiskitJob
-from .provider import QiskitProvider, QiskitRemoteService, QiskitRuntime
+from .provider import QiskitRuntimeProvider
 from .result import QiskitResult
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/providers/ibm/job.py` & `qbraid-0.7.0.dev20240516020308/qbraid/runtime/qiskit/job.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,66 +1,80 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
 Module defining QiskitJob Class
 
 """
 import logging
+from typing import TYPE_CHECKING, Optional
 
-from qiskit_ibm_provider import IBMBackend
-from qiskit_ibm_provider.job.exceptions import IBMJobInvalidStateError
+from qiskit_ibm_runtime.exceptions import RuntimeInvalidStateError
 
-from qbraid.providers.enums import JOB_FINAL
-from qbraid.providers.exceptions import JobError, JobStateError
-from qbraid.providers.job import QuantumJob
+from qbraid.runtime.enums import JobStatus
+from qbraid.runtime.exceptions import JobStateError, QbraidRuntimeError
+from qbraid.runtime.job import QuantumJob
 
 from .result import QiskitResult
 
+if TYPE_CHECKING:
+    import qiskit_ibm_runtime
+
 logger = logging.getLogger(__name__)
 
+IBM_JOB_STATUS_MAP = {
+    "INITIALIZING": JobStatus.INITIALIZING,
+    "QUEUED": JobStatus.QUEUED,
+    "VALIDATING": JobStatus.VALIDATING,
+    "RUNNING": JobStatus.RUNNING,
+    "CANCELLED": JobStatus.CANCELLED,
+    "DONE": JobStatus.COMPLETED,
+    "ERROR": JobStatus.FAILED,
+}
+
 
 class QiskitJob(QuantumJob):
     """Wrapper class for IBM Qiskit ``Job`` objects."""
 
-    def __init__(self, job_id: str, **kwargs):
+    def __init__(
+        self, job_id: str, job: "Optional[qiskit_ibm_runtime.RuntimeJob]" = None, **kwargs
+    ):
         """Create a ``QiskitJob`` object."""
         super().__init__(job_id, **kwargs)
+        self._job = job or self._get_job()
 
     def _get_job(self):
         """Return the job like object that is being wrapped."""
-        if not isinstance(self.device._device, IBMBackend):
-            raise JobError(
-                "Cannot retrieve job submitted to unrecognized backend. Expected device of type "
-                f"qiskit_ibm_provider.IBMBackend, but instead got {type(self.device._device)}."
-            )
-        job_id = self.vendor_job_id
-        backend = self.device._device
-        provider = backend.provider
-        return provider.backend.retrieve_job(job_id)
+        try:
+            service = self.device._service
+            return service.job(self.id)
+        except Exception as err:  # pylint: disable=broad-exception-caught
+            raise QbraidRuntimeError(f"Error retrieving job {self.id}") from err
 
-    def _get_status(self):
+    def status(self):
         """Returns status from Qiskit Job object."""
-        return str(self._job.status())
+        job_status = self._job.status().name
+        status = IBM_JOB_STATUS_MAP.get(job_status, JobStatus.UNKNOWN)
+        self._cache_metadata["status"] = status
+        return status
 
     def result(self):
         """Return the results of the job."""
-        if self.status() not in JOB_FINAL:
+        if self.is_terminal_state():
             logger.info("Result will be available when job has reached final state.")
         return QiskitResult(self._job.result())
 
     def cancel(self):
         """Attempt to cancel the job."""
-        status = self.status()
-        if status in JOB_FINAL:
-            raise JobStateError(f"Cannot cancel quantum job in the {status} state.")
+        if self.is_terminal_state():
+            raise JobStateError("Cannot cancel quantum job in non-terminal state.")
         try:
             return self._job.cancel()
-        except IBMJobInvalidStateError as err:
+        except RuntimeInvalidStateError as err:
             raise JobStateError from err
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/providers/ibm/provider.py` & `qbraid-0.7.0.dev20240516020308/qbraid/runtime/qiskit/provider.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,121 +1,135 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
-Module for configuring provider credentials and authentication.
+Module for configuring IBM provider credentials and authentication.
 
 """
 
 import os
-import re
-from abc import abstractmethod
-from typing import TYPE_CHECKING, List, Union
+from typing import TYPE_CHECKING, Optional
 
-from qbraid.providers.provider import QuantumProvider
+import qiskit
+from qiskit_ibm_runtime import QiskitRuntimeService
+from qiskit_ibm_runtime.accounts import ChannelType
+
+from qbraid.programs import ProgramSpec
+from qbraid.runtime.enums import DeviceType
+from qbraid.runtime.profile import TargetProfile
+from qbraid.runtime.provider import QuantumProvider
+
+from .device import QiskitBackend
 
 if TYPE_CHECKING:
-    import qiskit_ibm_provider
     import qiskit_ibm_runtime
 
+    import qbraid.runtime.qiskit
+
 
-class QiskitRemoteService(QuantumProvider):
+class QiskitRuntimeProvider(QuantumProvider):
     """
     This class is responsible for managing the interactions and
     authentications with the IBM Quantum services.
 
     Attributes:
-        qiskit_ibm_token (str): IBM Quantum token for authenticating with IBM Quantum services.
+        token (str): IBM Cloud API key or IBM Quantum API token.
+        runtime_service (qiskit_ibm_runtime.QiskitRuntimeService): IBM Quantum runtime service.
     """
 
-    def __init__(self, qiskit_ibm_token=None, **kwargs):
+    def __init__(
+        self, token: Optional[str] = None, channel: Optional[ChannelType] = None, **kwargs
+    ):
         """
         Initializes the QbraidProvider object with optional AWS and IBM Quantum credentials.
 
         Args:
-            qiskit_ibm_token (str, optional): IBM Quantum token. Defaults to None.
+            token (str, optional): IBM Quantum token. Defaults to None.
         """
-        self.qiskit_ibm_token = qiskit_ibm_token or os.getenv("QISKIT_IBM_TOKEN")
-        self._provider = self._get_ibm_provider(**kwargs)
+        self.token = token or os.getenv("QISKIT_IBM_TOKEN")
+        self.channel = channel or os.getenv("QISKIT_IBM_CHANNEL", "ibm_quantum")
+        self._runtime_service = QiskitRuntimeService(
+            token=self.token, channel=self.channel, **kwargs
+        )
+
+    @property
+    def runtime_service(self) -> "qiskit_ibm_runtime.QiskitRuntimeService":
+        """Returns the IBM Quantum runtime service."""
+        return self._runtime_service
 
-    @abstractmethod
-    def _get_ibm_provider(self, **kwargs):
-        """Returns the IBM Quantum provider."""
+    def save_config(
+        self,
+        token: Optional[str] = None,
+        channel: Optional[str] = None,
+        overwrite: bool = True,
+        **kwargs,
+    ) -> None:
+        """Saves IBM runtime service account to disk for future use."""
+        token = token or self.token
+        channel = channel or self.channel
+        QiskitRuntimeService.save_account(
+            token=token, channel=channel, overwrite=overwrite, **kwargs
+        )
+
+    def _build_runtime_profile(
+        self, backend: "qiskit_ibm_runtime.IBMBackend", program_spec: Optional[ProgramSpec] = None
+    ) -> TargetProfile:
+        """Builds a runtime profile from a backend."""
+        program_spec = program_spec or ProgramSpec(qiskit.QuantumCircuit)
+        config = backend.configuration()
+
+        if config.local:
+            device_type = DeviceType.LOCAL_SIMULATOR
+        elif config.simulator:
+            device_type = DeviceType.SIMULATOR
+        else:
+            device_type = DeviceType.QPU
+
+        return TargetProfile(
+            device_id=backend.name,
+            device_type=device_type,
+            num_qubits=config.n_qubits,
+            program_spec=program_spec,
+            instance=backend._instance,
+            max_shots=config.max_shots,
+        )
 
     def get_devices(
         self, operational=True, **kwargs
-    ) -> List[Union["qiskit_ibm_provider.IBMBackend", "qiskit_ibm_runtime.IBMBackend"]]:
+    ) -> list["qbraid.runtime.qiskit.QiskitBackend"]:
         """Returns the IBM Quantum provider backends."""
-        return self._provider.backends(operational=operational, **kwargs)
+        backends = self.runtime_service.backends(operational=operational, **kwargs)
+        program_spec = ProgramSpec(qiskit.QuantumCircuit)
+        return [
+            QiskitBackend(
+                profile=self._build_runtime_profile(backend, program_spec=program_spec),
+                service=self.runtime_service,
+            )
+            for backend in backends
+        ]
 
     def get_device(
-        self, device_id: str
-    ) -> Union["qiskit_ibm_provider.IBMBackend", "qiskit_ibm_runtime.IBMBackend"]:
+        self, device_id: str, instance: Optional[str] = None
+    ) -> "qbraid.runtime.qiskit.QiskitBackend":
         """Returns the IBM Quantum provider backends."""
-        provider = self._get_ibm_provider()
-        return provider.get_backend(device_id)
-
-    @staticmethod
-    def ibm_to_qbraid_id(name: str) -> str:
-        """Converts IBM device name to qBraid device ID"""
-        if name.startswith("ibm") or name.startswith("ibmq_"):
-            return re.sub(r"^(ibm)(q)?_(.*)", r"\1_q_\3", name)
-        return "ibm_q_" + name
-
-    @abstractmethod
-    def native_least_busy(
-        self,
-    ) -> Union["qiskit_ibm_provider.IBMBackend", "qiskit_ibm_runtime.IBMBackend"]:
-        """Return the Backend object of the least busy qpu."""
-
-    def ibm_least_busy_qpu(self) -> str:
-        """Return the qBraid ID of the least busy IBMQ QPU."""
-        backend = self.native_least_busy()
-        ibm_id = backend.name  # QPU name of form `ibm_*` or `ibmq_*`
-        _, name = ibm_id.split("_")
-        return f"ibm_q_{name}"
-
-
-class QiskitProvider(QiskitRemoteService):
-    """Wrapper for qiskit_ibm_provider.IBMProvider class"""
-
-    def save_config(self):
-        """Save the current configuration."""
-        provider = self._get_ibm_provider()
-        provider.save_account(token=self.qiskit_ibm_token, overwrite=True)
-
-    def _get_ibm_provider(self, **kwargs) -> "qiskit_ibm_provider.IBMProvider":
-        """Returns the IBM Quantum provider."""
-        from qiskit_ibm_provider import IBMProvider  # pylint: disable=import-outside-toplevel
-
-        return IBMProvider(token=self.qiskit_ibm_token, **kwargs)
-
-    def native_least_busy(self) -> "qiskit_ibm_provider.IBMBackend":
-        """Return the qBraid ID of the least busy IBMQ QPU."""
-        from qiskit_ibm_provider import least_busy  # pylint: disable=import-outside-toplevel
-
-        backends = self.get_devices(simulator=False, operational=True)
-        return least_busy(backends)
-
-
-class QiskitRuntime(QiskitRemoteService):
-    """Wrapper for qiskit_ibm_runtime.QiskitRuntimeService class."""
-
-    def _get_ibm_provider(
-        self, channel: str = "ibm_quantum", **kwargs
-    ) -> "qiskit_ibm_runtime.QiskitRuntimeService":
-        """Returns the IBM Qiskt Runtime service."""
-        # pylint: disable-next=import-outside-toplevel
-        from qiskit_ibm_runtime import QiskitRuntimeService
-
-        return QiskitRuntimeService(token=self.qiskit_ibm_token, channel=channel, **kwargs)
-
-    def native_least_busy(self) -> "qiskit_ibm_runtime.IBMBackend":
-        """Return the qBraid ID of the least busy IBMQ QPU."""
-        return self._provider.least_busy(simulator=False, operational=True)
+        backend = self.runtime_service.backend(device_id, instance=instance)
+        return QiskitBackend(
+            profile=self._build_runtime_profile(backend), service=self.runtime_service
+        )
+
+    def least_busy(
+        self, simulator=False, operational=True, **kwargs
+    ) -> "qbraid.runtime.qiskit.QiskitBackend":
+        """Return the least busy IBMQ QPU."""
+        backend = self.runtime_service.least_busy(
+            simulator=simulator, operational=operational, **kwargs
+        )
+        return QiskitBackend(
+            profile=self._build_runtime_profile(backend), service=self.runtime_service
+        )
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/providers/ibm/result.py` & `qbraid-0.7.0.dev20240516020308/qbraid/runtime/qiskit/result.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
@@ -10,15 +10,15 @@
 
 """
 Module defining QiskitResult Class
 
 """
 import numpy as np
 
-from qbraid.providers.result import QuantumJobResult
+from qbraid.runtime.result import QuantumJobResult
 
 
 class QiskitResult(QuantumJobResult):
     """Qiskit ``Result`` wrapper class."""
 
     def _format_measurements(self, memory_list):
         """Format the measurements into int for the given memory list"""
@@ -35,10 +35,10 @@
         qbraid_meas = [self._format_measurements(qiskit_meas[i]) for i in range(num_circuits)]
 
         if num_circuits == 1:
             qbraid_meas = qbraid_meas[0]
 
         return np.array(qbraid_meas)
 
-    def raw_counts(self):
+    def raw_counts(self, **kwargs):
         """Returns the histogram data of the run"""
         return self._result.get_counts()
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/providers/result.py` & `qbraid-0.7.0.dev20240516020308/qbraid/runtime/result.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,44 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
 Module defining abstract QuantumJobResult Class
 
 """
 from abc import ABC, abstractmethod
+from typing import Any, Optional
+
+import numpy as np
 
 
 class QuantumJobResult(ABC):
     """Abstract interface for result-like classes.
 
     Args:
         _result: A result-like object
 
     """
 
-    def __init__(self, _result):
-        self._result = _result
+    def __init__(self, result: Optional[Any] = None):
+        self._result = result
 
     @abstractmethod
-    def measurements(self):
+    def measurements(self) -> np.ndarray:
         """Return measurements as list"""
 
     @abstractmethod
-    def raw_counts(self):
+    def raw_counts(self, **kwargs):
         """Returns raw histogram data of the run"""
 
     @staticmethod
     def format_counts(counts: dict, include_zero_values: bool = False) -> dict:
         """Formats, sorts, and adds missing bit indices to counts dictionary
         Can pass in a 'include_zero_values' parameter to decide whether to include the states
         with zero counts.
@@ -59,16 +62,16 @@
         final_counts = {key: counts.get(key, 0) for key in sorted(all_keys)}
 
         if not include_zero_values:
             final_counts = {key: value for key, value in final_counts.items() if value != 0}
 
         return final_counts
 
-    def measurement_counts(self, include_zero_values: bool = False) -> dict:
+    def measurement_counts(self, include_zero_values: bool = False, **kwargs) -> dict:
         """Returns the sorted histogram data of the run"""
-        raw_counts = self.raw_counts()
+        raw_counts = self.raw_counts(**kwargs)
         if isinstance(raw_counts, dict):
             return self.format_counts(raw_counts, include_zero_values=include_zero_values)
         return [
             self.format_counts(counts, include_zero_values=include_zero_values)
             for counts in raw_counts
         ]
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/transforms/__init__.py` & `qbraid-0.7.0.dev20240516020308/qbraid/visualization/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,18 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
-
 """
-Module for runtime quantum program transformations.
-
-.. currentmodule:: qbraid.transforms
-
-Exceptions
------------
+Module for exceptions raised by visualization tools.
 
-.. autosummary::
-   :toctree: ../stubs/
+"""
+from qbraid.exceptions import QbraidError
 
-   CompilationError
 
-"""
-from .exceptions import CompilationError
+class VisualizationError(QbraidError):
+    """Class for errors raised when using visualization features."""
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/transforms/pytket/__init__.py` & `qbraid-0.7.0.dev20240516020308/qbraid/transforms/pytket/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
@@ -15,11 +15,11 @@
 
 Functions
 ----------
 
 .. autosummary::
    :toctree: ../stubs/
 
-   pytket_ionq_transform
+   harmony_transform
 
 """
-from .ionq import pytket_ionq_transform
+from .ionq import harmony_transform
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/transforms/pytket/ionq.py` & `qbraid-0.7.0.dev20240516020308/qbraid/transforms/pytket/ionq.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
 Module for converting generic quantum circuits to basis gate set compatible with IonQ devices.
 
 """
+
+# pylint: disable=no-name-in-module,no-member
+
 from typing import TYPE_CHECKING
 
 import pytket
 
 try:
     # pytket >= 1.22
     from pytket.circuit_library import TK1_to_RzRx  # type: ignore
@@ -82,17 +85,17 @@
 ionq_rebase_pass = RebaseCustom(
     ionq_gates,
     pytket.Circuit(),  # cx_replacement (irrelevant)
     TK1_to_RzRx,
 )  # tk1_replacement
 
 
-def pytket_ionq_transform(circuit: "pytket.circuit.Circuit") -> "pytket.circuit.Circuit":
+def harmony_transform(circuit: "pytket.circuit.Circuit") -> "pytket.circuit.Circuit":
     """
-    Compiles a Braket circuit to a Braket circuit that can run on IonQ Harmony.
+    Compiles a pytket circuit to gate set supported by IonQ Harmony.
 
     Args:
         circuit (pytket.circuit.Circuit): The input PyTKET circuit to be transformed.
 
     Returns:
         pytket.circuit.Circuit: The transformed PyTKET circuit that can run on IonQ Harmony.
 
@@ -109,15 +112,13 @@
                 ECR
                 GPi
                 GPi2
                 MS
                 PSwap
                 Unitary
 
-        - Otherwise, the circuit is transpiled using ``pytket-braket``'s ``braket_to_tk``.
-
     """
     cu = CompilationUnit(circuit, preds)
     ionq_rebase_pass.apply(cu)
     if not cu.check_all_predicates():
         raise CompilationError("Circuit cannot be compiled to IonQ Harmony.")
     return cu.circuit
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/__init__.py` & `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
@@ -16,16 +16,17 @@
 
 Classes
 --------
 
 .. autosummary::
    :toctree: ../stubs/
 
-   ConversionGraph
    Conversion
+   ConversionGraph
+   ConversionScheme
 
 Functions
 -----------
 
 .. autosummary::
    :toctree: ../stubs/
 
@@ -44,7 +45,8 @@
 
 """
 from .annotations import requires_extras
 from .converter import transpile
 from .edge import Conversion
 from .exceptions import CircuitConversionError, ConversionPathNotFoundError, NodeNotFoundError
 from .graph import ConversionGraph
+from .scheme import ConversionScheme
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/annotations.py` & `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/annotations.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/__init__.py` & `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
@@ -19,41 +19,42 @@
 
 .. autosummary::
    :toctree: ../stubs/
 
    braket
    cirq
    openqasm3
+   qasm2
+   qasm3
    pennylane
    pyquil
    pytket
    qiskit
 
 """
 import importlib
 import inspect
 
-# Dynamically import QPROGRAM_LIBS when needed
+# Dynamically import QPROGRAM_ALIASES when needed
 _qbraid = importlib.import_module("qbraid.programs._import")
-_PROGRAM_LIBS = getattr(_qbraid, "_PROGRAM_LIBS", [])
-QPROGRAM_LIBS = getattr(_qbraid, "QPROGRAM_LIBS", [])
-
-qprogram_libs_set = set(QPROGRAM_LIBS)
+_registry = importlib.import_module("qbraid.programs.registry")
+NATIVE_REGISTRY = getattr(_qbraid, "NATIVE_REGISTRY", {})
+QPROGRAM_REGISTRY = getattr(_registry, "QPROGRAM_REGISTRY", {})
 
 # Cache for storing previously seen valid combinations, including reversed pairs
 valid_combinations_cache = set()
 
 # List to store the names of the imported functions
 conversion_functions = []
 
 # Base path for the sub-modules
 base_path = "qbraid.transpiler.conversions."
 
 # Iterate over the installed libraries
-for lib in _PROGRAM_LIBS:
+for lib in NATIVE_REGISTRY:
     try:
         # Dynamically import the sub-module
         sub_module = importlib.import_module(base_path + lib)
 
         # Extract function names from the sub-module
         function_names = [
             name
@@ -71,15 +72,15 @@
             # Check if either pair or its reverse has been seen as valid before
             if pair in valid_combinations_cache or reverse_pair in valid_combinations_cache:
                 globals()[name] = getattr(sub_module, name)
                 conversion_functions.append(name)
                 continue
 
             # Check if both p1 and p2 are in the set
-            if p1 in qprogram_libs_set and p2 in qprogram_libs_set:
+            if p1 in NATIVE_REGISTRY and p2 in QPROGRAM_REGISTRY:
                 globals()[name] = getattr(sub_module, name)
                 conversion_functions.append(name)
                 # Add both the pair and its reverse to the cache
                 valid_combinations_cache.add(pair)
                 valid_combinations_cache.add(reverse_pair)
 
     except ModuleNotFoundError:
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/braket/__init__.py` & `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/pytket/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,27 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
-Amazon Braket conversions
+PyTKET conversions
 
-.. currentmodule:: qbraid.transpiler.conversions.braket
+.. currentmodule:: qbraid.transpiler.conversions.pytket
 
 Functions
 ----------
 
 .. autosummary::
    :toctree: ../stubs/
 
-   braket_to_cirq
-   cirq_to_braket
-   braket_to_qasm3
-   qasm3_to_braket
+   pytket_to_braket
+   pytket_to_qasm2
 
 """
-from .conversions_cirq import braket_to_cirq, cirq_to_braket
-from .conversions_qasm import braket_to_qasm3, qasm3_to_braket
+from .pytket_extras import pytket_to_braket
+from .pytket_to_qasm2 import pytket_to_qasm2
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/braket/cirq_from_braket.py` & `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/braket/braket_to_cirq.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 # Copyright (C) Unitary Fund
 #
 # This file is part of the qBraid-SDK.
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
@@ -10,57 +10,92 @@
 # This file includes code adapted from Mitiq (https://github.com/unitaryfund/mitiq)
 # with modifications by qBraid. The original copyright notice is included above.
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 # qbraid: skip-header
 
 """
-Module for converting Cirq circuits to Braket circuits
+Module for converting Braket circuits to Cirq circuits
 
 """
-from typing import Dict, List
+from typing import TYPE_CHECKING
 
 import numpy as np
 from braket.circuits import Circuit as BKCircuit
 from braket.circuits import Instruction as BKInstruction
 from braket.circuits import gates as braket_gates
 from braket.circuits import noises as braket_noise_gate
-from cirq import Circuit, LineQubit
-from cirq import ops as cirq_ops
-from cirq import protocols
+
+try:
+    import cirq
+except ImportError:
+    cirq = None
 
 try:
     import cirq_ionq.ionq_native_gates as cirq_ionq_ops
 except ImportError:
     cirq_ionq_ops = None
 
-from qbraid.transpiler.conversions.cirq.custom_ops import matrix_gate as matrix_to_cirq_gate
+from qbraid._import import LazyLoader
 from qbraid.transpiler.exceptions import CircuitConversionError
 
-from .custom_instr import gate_to_matrix as braket_gate_to_matrix
+cirq_passes = LazyLoader("cirq_passes", globals(), "qbraid.transforms.cirq.passes")
+
+if TYPE_CHECKING:
+    import cirq.circuits as cirq_circuits
+    import cirq.devices as cirq_devices
+    import cirq.ops as cirq_ops
+
+
+def _give_cirq_gate_name(gate: "cirq_ops.Gate", name: str, n_qubits: int) -> "cirq_ops.Gate":
+    def _circuit_diagram_info_(args):  # pylint: disable=unused-argument
+        return name, *(name,) * (n_qubits - 1)
+
+    gate._circuit_diagram_info_ = _circuit_diagram_info_
 
 
-def _braket_to_cirq(circuit: BKCircuit) -> Circuit:
+def matrix_to_cirq_gate(matrix: np.ndarray) -> "cirq_ops.MatrixGate":
+    """Return cirq matrix gate given unitary"""
+    n_qubits = int(np.log2(len(matrix)))
+    unitary_gate = cirq.MatrixGate(matrix)
+    _give_cirq_gate_name(unitary_gate, "U", n_qubits)
+    return unitary_gate
+
+
+def braket_gate_to_matrix(gate: braket_gates.Unitary) -> np.ndarray:
+    """Return the matrix representation of a Braket gate."""
+    matrix = gate.to_matrix()
+    unitary_gate = braket_gates.Unitary(matrix)
+    nqubits = int(np.log2(len(matrix)))
+    qubits = list(range(nqubits)) if nqubits > 1 else 0
+    bk_circuit = BKCircuit([BKInstruction(unitary_gate, qubits)])
+    return bk_circuit.to_unitary()
+
+
+def braket_to_cirq(circuit: BKCircuit) -> "cirq_circuits.Circuit":
     """Returns a Cirq circuit equivalent to the input Braket circuit.
 
     Note: The returned Cirq circuit acts on cirq.LineQubit's with indices equal
     to the qubit indices of the Braket circuit.
 
     Args:
         circuit: Braket circuit to convert to a Cirq circuit.
     """
     bk_qubits = [int(q) for q in circuit.qubits]
-    cirq_qubits = [LineQubit(x) for x in bk_qubits]
+    cirq_qubits = [cirq.LineQubit(x) for x in bk_qubits]
     qubit_mapping = {q: cirq_qubits[i] for i, q in enumerate(bk_qubits)}
-    return Circuit(_from_braket_instruction(instr, qubit_mapping) for instr in circuit.instructions)
+    circuit = cirq.Circuit(
+        _from_braket_instruction(instr, qubit_mapping) for instr in circuit.instructions
+    )
+    return cirq_passes.align_final_measurements(circuit)
 
 
 def _from_braket_instruction(
-    instr: BKInstruction, qubit_mapping: Dict[int, LineQubit]
-) -> List[cirq_ops.Operation]:
+    instr: BKInstruction, qubit_mapping: "dict[int, cirq_devices.LineQubit]"
+) -> "list[cirq_ops.Operation]":
     """Converts the braket instruction to an equivalent Cirq operation or list
     of Cirq operations.
 
     Args:
         instr: Braket instruction to convert.
         qubit_mapping: Braket qubit indicies mapped to indexed Cirq LineQubits
 
@@ -68,197 +103,201 @@
         ValueError: If the instruction cannot be converted to Cirq.
         CircuitConversionError: If error raise during conversion.
     """
     nqubits = len(instr.target)
     BK_qubits = [int(q) for q in instr.target]
     qubits = [qubit_mapping[x] for x in BK_qubits]
 
+    if str(instr.operator) == "Measure":
+        return [cirq.ops.MeasurementGate(num_qubits=nqubits).on(*qubits)]
+
     try:
         if nqubits == 1:
             return _from_one_qubit_braket_instruction(instr, qubits)
 
         if nqubits == 2:
             return _from_two_qubit_braket_instruction(instr, qubits)
 
         if nqubits == 3:
             if isinstance(instr.operator, braket_gates.CCNot):
-                return [cirq_ops.TOFFOLI.on(*qubits)]
+                return [cirq.ops.TOFFOLI.on(*qubits)]
             if isinstance(instr.operator, braket_gates.CSwap):
-                return [cirq_ops.FREDKIN.on(*qubits)]
+                return [cirq.ops.FREDKIN.on(*qubits)]
             try:
                 matrix = braket_gate_to_matrix(instr.operator)
-                return [cirq_ops.MatrixGate(matrix).on(*qubits)]
+                return [cirq.ops.MatrixGate(matrix).on(*qubits)]
             except (ValueError, TypeError) as err:
                 raise CircuitConversionError(
                     f"Unable to convert the instruction {instr} to Cirq."
                 ) from err
 
         # Unknown instructions.
         raise CircuitConversionError(
             f"Unable to convert to Cirq due to unrecognized \
             instruction: {instr}."
         )
+
     except Exception as err:
         raise CircuitConversionError(
             f"qBraid transpiler doesn't support operator {instr.operator}"
         ) from err
 
 
 def _from_one_qubit_braket_instruction(
-    instr: BKInstruction, qubits: List[LineQubit]
-) -> List[cirq_ops.Operation]:
+    instr: BKInstruction, qubits: "list[cirq_devices.LineQubit]"
+) -> "list[cirq_ops.Operation]":
     """Converts the one-qubit Braket instruction to Cirq operation(s).
 
     Args:
         instr: One-qubit Braket instruction to convert.
         qubits: Cirq LineQubit list indexed according to Braket instruction
 
     Raises:
         ValueError: If the instruction cannot be converted to Cirq.
     """
     gate = instr.operator
 
     # One-qubit non-parameterized gates.
     if isinstance(gate, braket_gates.I):
-        return [cirq_ops.I.on(*qubits)]
+        return [cirq.ops.I.on(*qubits)]
     if isinstance(gate, braket_gates.X):
-        return [cirq_ops.X.on(*qubits)]
+        return [cirq.ops.X.on(*qubits)]
     if isinstance(gate, braket_gates.Y):
-        return [cirq_ops.Y.on(*qubits)]
+        return [cirq.ops.Y.on(*qubits)]
     if isinstance(gate, braket_gates.Z):
-        return [cirq_ops.Z.on(*qubits)]
+        return [cirq.ops.Z.on(*qubits)]
     if isinstance(gate, braket_gates.H):
-        return [cirq_ops.H.on(*qubits)]
+        return [cirq.ops.H.on(*qubits)]
     if isinstance(gate, braket_gates.S):
-        return [cirq_ops.S.on(*qubits)]
+        return [cirq.ops.S.on(*qubits)]
     if isinstance(gate, braket_gates.Si):
-        return [protocols.inverse(cirq_ops.S.on(*qubits))]
+        return [cirq.protocols.inverse(cirq.ops.S.on(*qubits))]
     if isinstance(gate, braket_gates.T):
-        return [cirq_ops.T.on(*qubits)]
+        return [cirq.ops.T.on(*qubits)]
     if isinstance(gate, braket_gates.Ti):
-        return [protocols.inverse(cirq_ops.T.on(*qubits))]
+        return [cirq.protocols.inverse(cirq.ops.T.on(*qubits))]
     if isinstance(gate, braket_gates.V):
-        return [cirq_ops.X.on(*qubits) ** 0.5]
+        return [cirq.ops.X.on(*qubits) ** 0.5]
     if isinstance(gate, braket_gates.Vi):
-        return [cirq_ops.X.on(*qubits) ** -0.5]
+        return [cirq.ops.X.on(*qubits) ** -0.5]
 
     # One-qubit parameterized gates.
     if isinstance(gate, braket_gates.Rx):
-        return [cirq_ops.rx(gate.angle).on(*qubits)]
+        return [cirq.ops.rx(gate.angle).on(*qubits)]
     if isinstance(gate, braket_gates.Ry):
-        return [cirq_ops.ry(gate.angle).on(*qubits)]
+        return [cirq.ops.ry(gate.angle).on(*qubits)]
     if isinstance(gate, braket_gates.Rz):
-        return [cirq_ops.rz(gate.angle).on(*qubits)]
+        return [cirq.ops.rz(gate.angle).on(*qubits)]
     if isinstance(gate, braket_gates.PhaseShift):
-        return [cirq_ops.Z.on(*qubits) ** (gate.angle / np.pi)]
+        return [cirq.ops.Z.on(*qubits) ** (gate.angle / np.pi)]
 
     # One-qubit parameterized IonQ gates
     if cirq_ionq_ops and isinstance(gate, (braket_gates.GPi, braket_gates.GPi2)):
         phi = gate.angle / (2 * np.pi)
         gate_class = (
             cirq_ionq_ops.GPIGate if isinstance(gate, braket_gates.GPi) else cirq_ionq_ops.GPI2Gate
         )
         return [gate_class(phi=phi).on(*qubits)]
 
     # One-qubit Noise gates.
     if isinstance(gate, braket_noise_gate.BitFlip):
-        return [cirq_ops.BitFlipChannel(gate.probability).on(*qubits)]
+        return [cirq.ops.BitFlipChannel(gate.probability).on(*qubits)]
     if isinstance(gate, braket_noise_gate.PhaseFlip):
-        return [cirq_ops.PhaseFlipChannel(gate.probability).on(*qubits)]
+        return [cirq.ops.PhaseFlipChannel(gate.probability).on(*qubits)]
     if isinstance(gate, braket_noise_gate.Depolarizing):
-        return [cirq_ops.DepolarizingChannel(gate.probability).on(*qubits)]
+        return [cirq.ops.DepolarizingChannel(gate.probability).on(*qubits)]
     if isinstance(gate, braket_noise_gate.AmplitudeDamping):
-        return [cirq_ops.AmplitudeDampingChannel(gate.gamma).on(*qubits)]
+        return [cirq.ops.AmplitudeDampingChannel(gate.gamma).on(*qubits)]
     if isinstance(gate, braket_noise_gate.GeneralizedAmplitudeDamping):
         return [
-            cirq_ops.GeneralizedAmplitudeDampingChannel(gate.probability, gate.gamma).on(*qubits)
+            cirq.ops.GeneralizedAmplitudeDampingChannel(gate.probability, gate.gamma).on(*qubits)
         ]
     if isinstance(gate, braket_noise_gate.PhaseDamping):
-        return [cirq_ops.PhaseDampingChannel(gate.gamma).on(*qubits)]
+        return [cirq.ops.PhaseDampingChannel(gate.gamma).on(*qubits)]
 
     try:
         matrix = braket_gate_to_matrix(gate)
-        return [cirq_ops.MatrixGate(matrix).on(*qubits)]
+        return [cirq.ops.MatrixGate(matrix).on(*qubits)]
     except (ValueError, TypeError) as err:
         raise ValueError(f"Unable to convert the instruction {instr} to Cirq.") from err
 
 
 def _from_two_qubit_braket_instruction(
-    instr: BKInstruction, qubits: List[LineQubit]
-) -> List[cirq_ops.Operation]:
+    instr: BKInstruction, qubits: "list[cirq_devices.LineQubit]"
+) -> "list[cirq_ops.Operation]":
     """Converts the two-qubit braket instruction to Cirq.
 
     Args:
         instr: Two-qubit Braket instruction to convert.
         qubits: Cirq LineQubit list indexed according to Braket instruction
 
     Raises:
         ValueError: If the instruction cannot be converted to Cirq.
     """
     gate = instr.operator
 
     # Two-qubit non-parameterized gates.
     if isinstance(gate, braket_gates.CNot):
-        return [cirq_ops.CNOT.on(*qubits)]
+        return [cirq.ops.CNOT.on(*qubits)]
 
     if isinstance(gate, braket_gates.Swap):
-        return [cirq_ops.SWAP.on(*qubits)]
+        return [cirq.ops.SWAP.on(*qubits)]
     if isinstance(gate, braket_gates.ISwap):
-        return [cirq_ops.ISWAP.on(*qubits)]
+        return [cirq.ops.ISWAP.on(*qubits)]
     if isinstance(gate, braket_gates.CZ):
-        return [cirq_ops.CZ.on(*qubits)]
+        return [cirq.ops.CZ.on(*qubits)]
     if isinstance(gate, braket_gates.CY):
         return [
-            protocols.inverse(cirq_ops.S.on(qubits[1])),
-            cirq_ops.CNOT.on(*qubits),
-            cirq_ops.S.on(qubits[1]),
+            cirq.protocols.inverse(cirq.ops.S.on(qubits[1])),
+            cirq.ops.CNOT.on(*qubits),
+            cirq.ops.S.on(qubits[1]),
         ]
 
     # Two-qubit parameterized gates.
     if isinstance(gate, braket_gates.CPhaseShift):
-        return [cirq_ops.CZ.on(*qubits) ** (gate.angle / np.pi)]
+        return [cirq.ops.CZ.on(*qubits) ** (gate.angle / np.pi)]
     if isinstance(gate, braket_gates.CPhaseShift00):
         return [
-            cirq_ops.XX(*qubits),
-            cirq_ops.CZ.on(*qubits) ** (gate.angle / np.pi),
-            cirq_ops.XX(*qubits),
+            cirq.ops.XX(*qubits),
+            cirq.ops.CZ.on(*qubits) ** (gate.angle / np.pi),
+            cirq.ops.XX(*qubits),
         ]
     if isinstance(gate, braket_gates.CPhaseShift01):
         return [
-            cirq_ops.X(qubits[0]),
-            cirq_ops.CZ.on(*qubits) ** (gate.angle / np.pi),
-            cirq_ops.X(qubits[0]),
+            cirq.ops.X(qubits[0]),
+            cirq.ops.CZ.on(*qubits) ** (gate.angle / np.pi),
+            cirq.ops.X(qubits[0]),
         ]
     if isinstance(gate, braket_gates.CPhaseShift10):
         return [
-            cirq_ops.X(qubits[1]),
-            cirq_ops.CZ.on(*qubits) ** (gate.angle / np.pi),
-            cirq_ops.X(qubits[1]),
+            cirq.ops.X(qubits[1]),
+            cirq.ops.CZ.on(*qubits) ** (gate.angle / np.pi),
+            cirq.ops.X(qubits[1]),
         ]
     if isinstance(gate, braket_gates.PSwap):
         return [
-            cirq_ops.SWAP.on(*qubits),
-            cirq_ops.CNOT.on(*qubits),
-            cirq_ops.Z.on(qubits[1]) ** (gate.angle / np.pi),
-            cirq_ops.CNOT.on(*qubits),
+            cirq.ops.SWAP.on(*qubits),
+            cirq.ops.CNOT.on(*qubits),
+            cirq.ops.Z.on(qubits[1]) ** (gate.angle / np.pi),
+            cirq.ops.CNOT.on(*qubits),
         ]
     if isinstance(gate, braket_gates.XX):
-        return [cirq_ops.XXPowGate(exponent=gate.angle / np.pi, global_shift=-0.5).on(*qubits)]
+        return [cirq.ops.XXPowGate(exponent=gate.angle / np.pi, global_shift=-0.5).on(*qubits)]
     if isinstance(gate, braket_gates.YY):
-        return [cirq_ops.YYPowGate(exponent=gate.angle / np.pi, global_shift=-0.5).on(*qubits)]
+        return [cirq.ops.YYPowGate(exponent=gate.angle / np.pi, global_shift=-0.5).on(*qubits)]
     if isinstance(gate, braket_gates.ZZ):
-        return [cirq_ops.ZZPowGate(exponent=gate.angle / np.pi, global_shift=-0.5).on(*qubits)]
+        return [cirq.ops.ZZPowGate(exponent=gate.angle / np.pi, global_shift=-0.5).on(*qubits)]
     if isinstance(gate, braket_gates.XY):
-        return [cirq_ops.ISwapPowGate(exponent=gate.angle / np.pi).on(*qubits)]
+        return [cirq.ops.ISwapPowGate(exponent=gate.angle / np.pi).on(*qubits)]
 
     # Two-qubit noise gates.
     if isinstance(gate, braket_noise_gate.Kraus):
-        return [cirq_ops.KrausChannel(gate._matrices).on(*qubits)]
+        return [cirq.ops.KrausChannel(gate._matrices).on(*qubits)]
     if isinstance(gate, braket_noise_gate.TwoQubitDepolarizing):
-        return [cirq_ops.DepolarizingChannel(gate.probability, n_qubits=2).on(*qubits)]
+        return [cirq.ops.DepolarizingChannel(gate.probability, n_qubits=2).on(*qubits)]
 
     # Two-qubit two-parameters IonQ gates.
     if cirq_ionq_ops and isinstance(gate, braket_gates.MS):
         return [
             cirq_ionq_ops.MSGate(
                 phi0=gate.angle_1 / (2 * np.pi),
                 phi1=gate.angle_2 / (2 * np.pi),
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/braket/cirq_to_braket.py` & `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/cirq/cirq_to_braket.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 # Copyright (C) Unitary Fund
 #
 # This file is part of the qBraid-SDK.
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
@@ -14,38 +14,52 @@
 # qbraid: skip-header
 
 """
 Module for converting Braket circuits to Cirq circuits
 
 """
 from copy import deepcopy
-from typing import Dict, List, Optional, Union
+from typing import TYPE_CHECKING, Optional, Union
 
 import numpy as np
-from braket.circuits import Circuit as BKCircuit
-from braket.circuits import Instruction as BKInstruction
-from braket.circuits import gates as braket_gates
-from braket.circuits import noises as braket_noise_gate
+
+try:
+    from braket.circuits import Circuit as BKCircuit
+    from braket.circuits import Instruction as BKInstruction
+    from braket.circuits import gates as braket_gates
+    from braket.circuits import noises as braket_noise_gate
+except ImportError:
+    BKCircuit = None
+    BKInstruction = None
+    braket_gates = None
+    braket_noise_gate = None
+
 from cirq import Circuit
 from cirq import ops as cirq_ops
 from cirq import protocols
 from cirq.linalg.decompositions import kak_decomposition
 
 try:
     import cirq_ionq.ionq_native_gates as cirq_ionq_ops
 except ImportError:
     cirq_ionq_ops = None
 
 import qbraid.programs.libs.cirq
 from qbraid.transpiler.exceptions import CircuitConversionError
 
-from .custom_instr import C as BKControl
+try:
+    from .braket_custom import C as BKControl
+except ImportError:
+    BKControl = None
+
+if TYPE_CHECKING:
+    import braket.circuits
 
 
-def _cirq_to_braket(circuit: Circuit) -> BKCircuit:
+def cirq_to_braket(circuit: Circuit) -> "braket.circuits.Circuit":
     """Returns a Braket circuit equivalent to the input Cirq circuit.
 
     Args:
         circuit: Cirq circuit to convert to a Braket circuit.
 
     Returns:
         Braket circuit equivalent to the input Cirq circuit.
@@ -59,16 +73,16 @@
     return BKCircuit(
         _to_braket_instruction(operation, qubit_mapping) for operation in circuit.all_operations()
     )
 
 
 def _to_braket_instruction(
     operation: cirq_ops.Operation,
-    qubit_mapping: Dict[int, int],
-) -> List[BKInstruction]:
+    qubit_mapping: dict[int, int],
+) -> "list[braket.circuits.Instruction]":
     """Converts Cirq operation to equivalent Braket instruction(s).
 
     Args:
         operation: Cirq operation to convert.
         qubit_mapping: Mappings of input / output qubit indicies
 
     Raises:
@@ -120,15 +134,15 @@
     raise CircuitConversionError(f"Unable to convert {operation} to Braket")
 
 
 def _to_one_qubit_braket_instruction(
     operation: Union[np.ndarray, cirq_ops.Gate, cirq_ops.Operation],
     target: int,
     gate_name: Optional[str] = None,
-) -> List[BKInstruction]:
+) -> "list[braket.circuits.Instruction]":
     """Converts one-qubit Cirq operation or NumPy array to equivalent Braket instruction(s)
 
     Args:
         operation: One-qubit Cirq operation or numpy unitary to translate.
         target: Qubit index for the operation to act on. Must be specified and if only
             if `operation` is given as a numpy array.
         gate_name: Optional unitary gate display name for `operation` of type `np.ndarray`
@@ -235,16 +249,16 @@
         raise ValueError(f"Unable to convert {operation} to braket")
 
     return convert_one_qubit_gate(gate, target)
 
 
 def _to_two_qubit_braket_instruction(
     operation: Union[cirq_ops.Gate, cirq_ops.Operation],
-    qubits: List[int],
-) -> List[BKInstruction]:
+    qubits: list[int],
+) -> "list[braket.circuits.Instruction]":
     """Converts two-qubit Cirq operation to equivalent Braket instruction(s)
 
     Args:
         operation: Two-qubit Cirq operation to translate.
         qubits: Length 2 list of qubit indicies
 
     Raises:
@@ -290,15 +304,15 @@
     # Fallback: arbitrary two-qubit unitary (KAK) decomposition
     unitary = protocols.unitary(operation)
     return _kak_decomposition_to_braket_instruction(unitary, q1, q2)
 
 
 def _kak_decomposition_to_braket_instruction(
     matrix: np.ndarray, q1: int, q2: int
-) -> List[BKInstruction]:
+) -> "list[braket.circuits.Instruction]":
     """Converts 4x4 Numpy array to equivalent Braket instruction(s) via kak decomposition
 
     Args:
         matrix: Unitary 4x4 numpy array representing 2-qubit gate.
         q1: Index of first qubit to act on
         q2: Index of second qubit to act on
     """
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/braket/conversions_cirq.py` & `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/pytket/pytket_extras.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,46 +5,35 @@
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
-Module for converting Braket circuits to/from Cirq
+Module containing PyTKET conversion extras.
 
 """
 
 from typing import TYPE_CHECKING
 
-if TYPE_CHECKING:
-    import braket.circuits
-    import cirq
-
-
-def braket_to_cirq(circuit: "braket.circuits.Circuit") -> "cirq.Circuit":
-    """Returns a Cirq circuit equivalent to the input Braket circuit.
-
-    Note: The returned Cirq circuit acts on cirq.LineQubit's with indices equal
-    to the qubit indices of the Braket circuit.
+from qbraid._import import LazyLoader
+from qbraid.transpiler.annotations import requires_extras
 
-    Args:
-        circuit: Braket circuit to convert to a Cirq circuit.
-    """
-    # pylint: disable-next=import-outside-toplevel
-    from .cirq_from_braket import _braket_to_cirq
+pytket_braket = LazyLoader("pytket_braket", globals(), "pytket.extensions.braket")
 
-    return _braket_to_cirq(circuit)
+if TYPE_CHECKING:
+    import braket.circuits
+    import pytket.circuit
 
 
-def cirq_to_braket(circuit: "cirq.Circuit") -> "braket.circuits.Circuit":
-    """Returns a Braket circuit equivalent to the input Cirq circuit.
+@requires_extras("pytket.extensions.braket")
+def pytket_to_braket(circuit: "pytket.circuit.Circuit") -> "braket.circuits.Circuit":
+    """Returns an Amazon Braket circuit equivalent to the input pytket circuit.
 
     Args:
-        circuit: Cirq circuit to convert to a Braket circuit.
+        circuit (pytket.circuit.Circuit): PyTKET circuit to convert to Braket circuit.
 
     Returns:
-        Braket circuit equivalent to the input Cirq circuit.
+        braket.circuits.Circuit: Braket circuit equivalent to input pytket circuit.
     """
-    # pylint: disable-next=import-outside-toplevel
-    from .cirq_to_braket import _cirq_to_braket
-
-    return _cirq_to_braket(circuit)
+    braket_circuit, _, _ = pytket_braket.braket_convert.tk_to_braket(circuit)
+    return braket_circuit
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/braket/conversions_qasm.py` & `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qasm3/qasm3_to_braket.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,79 +1,47 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
 Module for converting Braket circuits to/from OpenQASM 3
 
 """
-from braket.circuits import Circuit
-from braket.circuits.serialization import IRType
-from braket.ir.openqasm import Program as OpenQasmProgram
+from typing import TYPE_CHECKING
 
-from qbraid.programs import QasmError, convert_qasm_pi_to_decimal
+from qbraid._import import LazyLoader
+from qbraid.programs import QasmError
+from qbraid.transforms.qasm3.compat import transform_notation_to_external
 
-QASMType = str
+braket_circuits = LazyLoader("braket_circuits", globals(), "braket.circuits")
+braket_openqasm = LazyLoader("braket_openqasm", globals(), "braket.ir.openqasm")
 
+if TYPE_CHECKING:
+    import braket.circuits
 
-def qasm3_to_braket(qasm3_str: QASMType) -> Circuit:
+
+def qasm3_to_braket(qasm3_str: str) -> "braket.circuits.Circuit":
     """Converts an OpenQASM 3.0 string to a ``braket.circuits.Circuit``.
 
     Args:
         qasm3_str: OpenQASM 3 string
 
     Returns:
         The Amazon Braket circuit equivalent to the input OpenQASM 3.0 string
 
     Raises:
         CircuitConversionError: If qasm to braket conversion fails
 
     """
-    replacements = {
-        "cx ": "cnot ",
-        "sdg ": "si ",
-        "tdg ": "ti ",
-        "sx ": "v ",
-        "sxdg ": "vi ",
-        "p(": "phaseshift(",
-        "cp(": "cphaseshift(",
-    }
-
-    def replace_commands(qasm, replacements):
-        for old, new in replacements.items():
-            qasm = qasm.replace(old, new)
-        return qasm
-
-    qasm3_str = qasm3_str.replace('include "stdgates.inc";', "")
-    qasm3_str = replace_commands(qasm3_str, replacements)
-    qasm3_str = convert_qasm_pi_to_decimal(qasm3_str)
+    qasm3_str = transform_notation_to_external(qasm3_str)
 
     try:
-        program = OpenQasmProgram(source=qasm3_str)
-        return Circuit.from_ir(source=program.source, inputs=program.inputs)
+        program = braket_openqasm.Program(source=qasm3_str)
+        return braket_circuits.Circuit.from_ir(source=program.source, inputs=program.inputs)
     except Exception as err:
         raise QasmError("Error converting qasm3 string to braket circuit") from err
-
-
-def braket_to_qasm3(circuit: Circuit) -> QASMType:
-    """Converts a ``braket.circuits.Circuit`` to an OpenQASM 3.0 string.
-
-    Args:
-        circuit: Amazon Braket quantum circuit
-
-    Returns:
-        The OpenQASM 3.0 string equivalent to the circuit
-
-    Raises:
-        CircuitConversionError: If braket to qasm conversion fails
-
-    """
-    try:
-        return circuit.to_ir(IRType.OPENQASM).source
-    except Exception as err:
-        raise QasmError("Error converting braket circuit to qasm3 string") from err
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/braket/custom_instr.py` & `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/cirq/braket_custom.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,62 +1,30 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
-Module for Braket custom gates
+Module for defining custom Amazon Braket control gate
 
 """
 import itertools
-from typing import Any, List
+from typing import Any
 
 import braket.ir.jaqcd as ir
 import numpy as np
-from braket.circuits import Circuit, Gate, Instruction, QubitSet, circuit
+from braket.circuits import Gate, Instruction, QubitSet, circuit
 from braket.circuits.gates import Unitary, format_complex
 from braket.circuits.serialization import OpenQASMSerializationProperties
 
-from qbraid.transpiler.exceptions import CircuitConversionError
-
-# pylint: disable=missing-function-docstring
-
-
-def gate_to_matrix(gate: Unitary) -> np.ndarray:
-    matrix = gate.to_matrix()
-    unitary_gate = Unitary(matrix)
-    nqubits = int(np.log2(len(matrix)))
-    qubits = list(range(nqubits)) if nqubits > 1 else 0
-    bk_circuit = Circuit([Instruction(unitary_gate, qubits)])
-    return bk_circuit.to_unitary()
-
-
-def unitary_instruction(instr: Instruction) -> Instruction:
-    """Converts a Braket instruction to a unitary gate instruction.
-
-    Args:
-        instr: Braket instruction to convert.
-
-    Raises:
-        CircuitConversionError: If the instruction cannot be converted
-    """
-    gate = instr.operator
-
-    try:
-        matrix = gate_to_matrix(gate)
-        gate_name = "U" if gate.name is None else gate.name
-        return Instruction(Unitary(matrix, display_name=gate_name), instr.target)
-    except (ValueError, TypeError) as err:
-        raise CircuitConversionError(f"Unable to convert the instruction {instr}.") from err
-
 
 class C(Gate):
     """Controlled gate
     Args:
         sub_gate (Gate): Quantum Gate.
         targets (QubitSet): Target qubits.
     """
@@ -88,15 +56,16 @@
 
         Returns:
             np.ndarray: A matrix representation of the quantum operator
         """
         sub_matrix = self.sub_gate.to_matrix()
         return self._extend_matrix(sub_matrix)
 
-    def adjoint(self) -> List[Gate]:
+    def adjoint(self) -> list[Gate]:
+        """Returns the adjoint of the gate."""
         return [Unitary(self.to_matrix().conj().T, display_name=f"({self.ascii_symbols})^†")]
 
     def _to_jaqcd(self, target: QubitSet) -> Any:
         return ir.Unitary.construct(
             targets=list(target),
             matrix=Unitary._transform_matrix_to_ir(self.to_matrix()),
         )
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/cirq/__init__.py` & `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/pyquil/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,25 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
-Cirq conversions
+PyQuil conversions
 
-.. currentmodule:: qbraid.transpiler.conversions.cirq
-
-Classes
-----------
-
-.. autosummary::
-   :toctree: ../stubs/
-
-   QasmParser
+.. currentmodule:: qbraid.transpiler.conversions.pyquil
 
 Functions
 ----------
 
 .. autosummary::
    :toctree: ../stubs/
 
-   qasm2_to_cirq
-   cirq_to_qasm2
+   pyquil_to_cirq
 
 """
-from .cirq_qasm_parser import QasmParser
-from .conversions_qasm import cirq_to_qasm2, qasm2_to_cirq
+from .pyquil_to_cirq import pyquil_to_cirq
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/cirq/cirq_qasm_parser.py` & `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qasm2/cirq_qasm_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 # Copyright (C) The Cirq Developers
 #
 # This file is part of the qBraid-SDK.
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. This specific file, adapted from Cirq, is dual-licensed under both the
 # Apache License, Version 2.0, and the GPL v3. You may not use this file except in
@@ -22,26 +22,26 @@
 
 """
 Module defining qBraid Cirq QASM parser.
 
 """
 import functools
 import operator
-from typing import Any, Callable, cast, Dict, Iterable, List, Optional, Union, TYPE_CHECKING
+from typing import Any, Callable, cast, Iterable, Optional, Union, TYPE_CHECKING
 
 import numpy as np
 # import sympy
 from ply import yacc
 
 from cirq import ops, Circuit, NamedQubit, CX
 from cirq.circuits.qasm_output import QasmUGate
 from cirq.contrib.qasm_import._lexer import QasmLexer
 from cirq.contrib.qasm_import.exception import QasmException
 
-import qbraid.transpiler.conversions.cirq.custom_ops as qbraid_cirq_gates
+from .cirq_custom import U2Gate, U3Gate, rzz
 
 # Redefined lexer tokens (4/7/21) to surpress warning:
 # Token ['IF', 'NE'] defined, but not used
 QasmLexer.tokens = [
     "FORMAT_SPEC",
     "NUMBER",
     "NATURAL_NUMBER",
@@ -82,15 +82,15 @@
     and parameters of the call and to generate a list of corresponding
     cirq.GateOperation's in the 'on' method.
     """
 
     def __init__(
         self,
         qasm_gate: str,
-        cirq_gate: Union[ops.Gate, Callable[[List[float]], ops.Gate]],
+        cirq_gate: Union[ops.Gate, Callable[[list[float]], ops.Gate]],
         num_params: int,
         num_args: int,
     ):
         """Initializes a Qasm gate statement.
         Args:
             qasm_gate: The symbol of the QASM gate.
             cirq_gate: The gate class on the cirq side.
@@ -101,31 +101,31 @@
         self.cirq_gate = cirq_gate
         self.num_params = num_params
 
         # at least one quantum argument is mandatory for gates to act on
         assert num_args >= 1
         self.num_args = num_args
 
-    def _validate_args(self, args: List[List[ops.Qid]], lineno: int):
+    def _validate_args(self, args: list[list[ops.Qid]], lineno: int):
         if len(args) != self.num_args:
             raise QasmException(
                 "{} only takes {} arg(s) (qubits and/or registers), "
                 "got: {}, at line {}".format(self.qasm_gate, self.num_args, len(args), lineno)
             )
 
-    def _validate_params(self, params: List[float], lineno: int):
+    def _validate_params(self, params: list[float], lineno: int):
         if len(params) != self.num_params:
             raise QasmException(
                 "{} takes {} parameter(s), got: {}, at line {}".format(
                     self.qasm_gate, self.num_params, len(params), lineno
                 )
             )
 
     def on(
-        self, params: List[float], args: List[List[ops.Qid]], lineno: int
+        self, params: list[float], args: list[list[ops.Qid]], lineno: int
     ) -> Iterable[ops.Operation]:
         self._validate_args(args, lineno)
         self._validate_params(params, lineno)
 
         reg_sizes = np.unique([len(reg) for reg in args])
         if len(reg_sizes) > 2 or (len(reg_sizes) > 1 and reg_sizes[0] != 1):
             raise QasmException(
@@ -142,15 +142,15 @@
         # Based on the OpenQASM spec (https://arxiv.org/abs/1707.03429),
         # single qubit arguments can be mixed with qubit registers.
         # Given quantum registers of length reg_size and single qubits are both
         # used as arguments, we generate reg_size GateOperations via iterating
         # through each qubit of the registers 0 to n-1 and use the same one
         # qubit from the "single-qubit registers" for each operation.
         op_qubits = functools.reduce(
-            cast(Callable[[List['cirq.Qid'], List['cirq.Qid']], List['cirq.Qid']], np.broadcast),
+            cast(Callable[[list['cirq.Qid'], list['cirq.Qid']], list['cirq.Qid']], np.broadcast),
             args,
         )
         for qubits in op_qubits:
             if isinstance(qubits, ops.Qid):
                 yield final_gate.on(qubits)
             elif len(np.unique(qubits)) < len(qubits):
                 raise QasmException(f"Overlapping qubits in arguments at line {lineno}")
@@ -165,21 +165,21 @@
         qasm = "OPENQASM 2.0; qreg q1[2]; CX q1[0], q1[1];"
         parsedQasm = QasmParser().parse(qasm)
     """
 
     def __init__(self):
         self.parser = yacc.yacc(module=self, debug=False, write_tables=False)
         self.circuit = Circuit()
-        self.qregs: Dict[str, int] = {}
-        self.cregs: Dict[str, int] = {}
+        self.qregs: dict[str, int] = {}
+        self.cregs: dict[str, int] = {}
         self.qelibinc = False
         self.lexer = QasmLexer()
         self.supported_format = False
         self.parsedQasm: Optional[Qasm] = None
-        self.qubits: Dict[str, ops.Qid] = {}
+        self.qubits: dict[str, ops.Qid] = {}
         self.functions = {
             'sin': np.sin,
             'cos': np.cos,
             'tan': np.tan,
             'exp': np.exp,
             'ln': np.log,
             'sqrt': np.sqrt,
@@ -192,15 +192,15 @@
             '+': operator.add,
             '-': operator.sub,
             '*': operator.mul,
             '/': operator.truediv,
             '^': operator.pow,
         }
 
-    basic_gates: Dict[str, QasmGateStatement] = {
+    basic_gates: dict[str, QasmGateStatement] = {
         'CX': QasmGateStatement(qasm_gate='CX', cirq_gate=CX, num_params=0, num_args=2),
         'U': QasmGateStatement(
             qasm_gate='U',
             num_params=3,
             num_args=1,
             # QasmUGate expects half turns
             cirq_gate=(lambda params: QasmUGate(*[p / np.pi for p in params])),
@@ -233,27 +233,27 @@
             qasm_gate='u1',
             cirq_gate=(lambda params: ops.ZPowGate(exponent=params[0] / np.pi)),
             num_params=1,
             num_args=1,
         ),
         'u2': QasmGateStatement(
             qasm_gate='u2',
-            cirq_gate=(lambda params: qbraid_cirq_gates.U2Gate(*params)),
+            cirq_gate=(lambda params: U2Gate(*params)),
             num_params=2,
             num_args=1,
         ),
         'u3': QasmGateStatement(
             qasm_gate='u3',
-            cirq_gate=(lambda params: qbraid_cirq_gates.U3Gate(*params)),
+            cirq_gate=(lambda params: U3Gate(*params)),
             num_params=3,
             num_args=1,
         ),
         'u': QasmGateStatement(
             qasm_gate='u',
-            cirq_gate=(lambda params: qbraid_cirq_gates.U3Gate(*params)),
+            cirq_gate=(lambda params: U3Gate(*params)),
             num_params=3,
             num_args=1,
         ),
         'r': QasmGateStatement(
             qasm_gate='r',
             num_params=2,
             num_args=1,
@@ -314,21 +314,21 @@
             qasm_gate='cu1',
             cirq_gate=(lambda params: ops.ControlledGate(ops.ZPowGate(exponent=params[0] / np.pi))),
             num_params=1,
             num_args=2,
         ),
         'cu3': QasmGateStatement(
             qasm_gate='cu3',
-            cirq_gate=(lambda params: ops.ControlledGate(qbraid_cirq_gates.U3Gate(*params))),
+            cirq_gate=(lambda params: ops.ControlledGate(U3Gate(*params))),
             num_params=3,
             num_args=2,
         ),
         'cu': QasmGateStatement(
             qasm_gate='cu',
-            cirq_gate=(lambda params: ops.ControlledGate(qbraid_cirq_gates.U3Gate(*params))),
+            cirq_gate=(lambda params: ops.ControlledGate(U3Gate(*params))),
             num_params=3,
             num_args=2,
         ),
         'p': QasmGateStatement(
             qasm_gate='p', cirq_gate=(lambda params: ops.ZPowGate(exponent=params[0] / np.pi)), num_params=1, num_args=1,
         ),
         'cp': QasmGateStatement(
@@ -338,15 +338,15 @@
             num_args=2,
         ),
         'iswap': QasmGateStatement(
             qasm_gate='iswap', cirq_gate=ops.ISWAP, num_params=0, num_args=2
         ),
         'rzz': QasmGateStatement(
             qasm_gate='rzz',
-            cirq_gate=(lambda params: qbraid_cirq_gates.rzz(params[0])),
+            cirq_gate=(lambda params: rzz(params[0])),
             num_params=1,
             num_args=2,
         ),
     }
 
     all_gates = {**basic_gates, **qelib_gates}
 
@@ -432,15 +432,15 @@
         self._resolve_gate_operation(p[2], gate=p[1], p=p, params=[])
 
     def p_gate_op_with_params(self, p):
         """gate_op :  ID '(' params ')' qargs"""
         self._resolve_gate_operation(args=p[5], gate=p[1], p=p, params=p[3])
 
     def _resolve_gate_operation(
-        self, args: List[List[ops.Qid]], gate: str, p: Any, params: List[float]
+        self, args: list[list[ops.Qid]], gate: str, p: Any, params: list[float]
     ):
         gate_set = self.basic_gates if not self.qelibinc else self.all_gates
         if gate not in gate_set.keys():
             msg = 'Unknown gate "{}" at line {}{}'.format(
                 gate,
                 p.lineno(1),
                 ", did you forget to include qelib1.inc?" if not self.qelibinc else "",
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/cirq/conversions_qasm.py` & `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/cirq/cirq_to_qasm2.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
@@ -12,22 +12,17 @@
 Module for conversions between Cirq Circuits and QASM strings
 
 """
 from typing import Optional
 
 import cirq
 from cirq import ops
-from cirq.contrib.qasm_import.exception import QasmException as CirqQasmException
 
 from qbraid._version import __version__ as qbraid_version
-from qbraid.programs.exceptions import QasmError as QbraidQasmError
-from qbraid.programs.qasm_passes import flatten_qasm_program
-
-from .cirq_qasm_parser import QasmParser
-from .custom_ops import _map_zpow_and_unroll
+from qbraid.transforms.cirq import map_zpow_and_unroll
 
 QASMType = str
 
 
 def _to_qasm_output(
     circuit: cirq.Circuit,
     header: Optional[str] = None,
@@ -65,25 +60,9 @@
 
     Args:
         circuit: Cirq circuit to convert to a QASM string.
 
     Returns:
         QASMType: QASM string equivalent to the input Cirq circuit.
     """
-    circuit = _map_zpow_and_unroll(circuit)
+    circuit = map_zpow_and_unroll(circuit)
     return str(_to_qasm_output(circuit, header, precision, qubit_order))
-
-
-def qasm2_to_cirq(qasm: QASMType) -> cirq.Circuit:
-    """Returns a Cirq circuit equivalent to the input QASM string.
-
-    Args:
-        qasm: QASM string to convert to a Cirq circuit.
-
-    Returns:
-        Cirq circuit representation equivalent to the input QASM string.
-    """
-    try:
-        qasm = flatten_qasm_program(qasm)
-        return QasmParser().parse(qasm).circuit
-    except CirqQasmException as err:
-        raise QbraidQasmError from err
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/cirq/custom_ops.py` & `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qasm2/cirq_custom.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
@@ -12,29 +12,19 @@
 
 """
 Module for Cirq custom gates to aid the transpiler and qasm parser
 
 """
 
 import fractions
-from typing import Optional, Tuple
 
-import cirq
 import numpy as np
-from cirq import (
-    OP_TREE,
-    Circuit,
-    CircuitDiagramInfo,
-    Gate,
-    IdentityGate,
-    MatrixGate,
-    Operation,
-    TwoQubitDiagonalGate,
-    value,
-)
+from cirq import CircuitDiagramInfo, Gate, IdentityGate, TwoQubitDiagonalGate
+
+# pylint: disable=abstract-method
 
 
 class U2Gate(Gate):
     """A single qubit gate for rotations about the
     X+Z axis of the Bloch sphere.
     """
 
@@ -148,66 +138,14 @@
         rounded_theta = np.array(theta_radians)
         if args.precision is not None:
             rounded_theta = rounded_theta.round(args.precision)
         gate_str = f"RZZ({rounded_theta})"
         return CircuitDiagramInfo((gate_str, gate_str))
 
 
-@value.value_equality
-class ZPowGate(cirq.ZPowGate):
-    """A single qubit gate for rotations around the
-    Z axis of the Bloch sphere.
-    """
-
-    def _qasm_(self, args: "cirq.QasmArgs", qubits: Tuple["cirq.Qid", ...]) -> Optional[str]:
-        args.validate_version("2.0")
-        if self._global_shift == 0:
-            if self._exponent == 0.25:
-                return args.format("t {0};\n", qubits[0])
-            if self._exponent == -0.25:
-                return args.format("tdg {0};\n", qubits[0])
-            if self._exponent == 0.5:
-                return args.format("s {0};\n", qubits[0])
-            if self._exponent == -0.5:
-                return args.format("sdg {0};\n", qubits[0])
-            if self._exponent == 1:
-                return args.format("z {0};\n", qubits[0])
-            return args.format("p({0:half_turns}) {1};\n", self._exponent, qubits[0])
-        return args.format("rz({0:half_turns}) {1};\n", self._exponent, qubits[0])
-
-
-def _give_cirq_gate_name(gate: Gate, name: str, n_qubits: int) -> Gate:
-    def _circuit_diagram_info_(args):
-        return name, *(name,) * (n_qubits - 1)
-
-    gate._circuit_diagram_info_ = _circuit_diagram_info_
-
-
-def matrix_gate(matrix: np.ndarray) -> MatrixGate:
-    """Return cirq matrix gate given unitary"""
-    n_qubits = int(np.log2(len(matrix)))
-    unitary_gate = MatrixGate(matrix)
-    _give_cirq_gate_name(unitary_gate, "U", n_qubits)
-    return unitary_gate
-
-
 def rzz(theta):
     """Returns custom cirq RZZ gate given rotation angle"""
     if theta == 0:
         return IdentityGate(2)
     if theta == 2 * np.pi:
         return TwoQubitDiagonalGate([np.pi] * 4)
     return RZZGate(theta)
-
-
-def _map_zpow_and_unroll(circuit: Circuit) -> Circuit:
-    """Map ZPowGate to RZ and unroll circuit"""
-
-    def _map_zpow(op: Operation, _: int) -> OP_TREE:
-        if isinstance(op.gate, cirq.ZPowGate):
-            yield ZPowGate(exponent=op.gate.exponent, global_shift=op.gate.global_shift)(
-                op.qubits[0]
-            )
-        else:
-            yield op
-
-    return cirq.map_operations_and_unroll(circuit, _map_zpow)
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/openqasm3/__init__.py` & `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qasm3/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,31 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
-OpenQASM conversions
+OpenQASM 3 conversions
 
-.. currentmodule:: qbraid.transpiler.conversions.openqasm3
+.. currentmodule:: qbraid.transpiler.conversions.qasm3
 
 Functions
 ----------
 
 .. autosummary::
    :toctree: ../stubs/
 
-   qasm2_to_qasm3
-   openqasm3_to_qasm3
+   qasm3_to_braket
    qasm3_to_openqasm3
+   qasm3_to_qiskit
+   qasm3_to_pyqir
 
 """
-from .conversions_qasm import openqasm3_to_qasm3, qasm2_to_qasm3, qasm3_to_openqasm3
+from .qasm3_extras import qasm3_to_pyqir
+from .qasm3_to_braket import qasm3_to_braket
+from .qasm3_to_openqasm3 import qasm3_to_openqasm3
+from .qasm3_to_qiskit import qasm3_to_qiskit
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/pennylane/__init__.py` & `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/pennylane/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
@@ -18,8 +18,8 @@
 
 .. autosummary::
    :toctree: ../stubs/
 
    pennylane_to_qasm2
 
 """
-from .conversions_qasm import pennylane_to_qasm2
+from .pennylane_to_qasm2 import pennylane_to_qasm2
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/pennylane/conversions_qasm.py` & `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/pennylane/pennylane_to_qasm2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/pyquil/__init__.py` & `qbraid-0.7.0.dev20240516020308/qbraid/transforms/cirq/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
-PyQuil conversions
+Module containing functions for transforming cirq programs.
 
-.. currentmodule:: qbraid.transpiler.conversions.pyquil
+.. currentmodule:: qbraid.transforms.cirq
 
 Functions
 ----------
 
 .. autosummary::
    :toctree: ../stubs/
 
-   pyquil_to_cirq
-   cirq_to_pyquil
+   decompose
+   map_zpow_and_unroll
 
 """
-
-from .conversions_cirq import cirq_to_pyquil, pyquil_to_cirq
+from .passes import decompose, map_zpow_and_unroll
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/pyquil/cirq_quil_input.py` & `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/pyquil/cirq_quil_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 # Copyright (C) 2020 The Cirq Developers
 #
 # This file is part of the qBraid-SDK.
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. This specific file, adapted from Cirq, is dual-licensed under both the
 # Apache License, Version 2.0, and the GPL v3. You may not use this file except in
@@ -17,15 +17,15 @@
 # qbraid: skip-header
 
 """
 Module for conversions from Quil to Cirq.
 
 """
 
-from typing import Callable, Dict, Union, cast
+from typing import Callable, Union, cast
 
 import numpy as np
 from cirq import Circuit, LineQubit
 from cirq.ops import (
     CCNOT,
     CNOT,
     CSWAP,
@@ -185,15 +185,15 @@
 
 RESET_ERROR = """
 Please remove RESETs from your Quil program.
 RESET directives have special meaning on QCS, to enable active reset.
 """
 
 # Parameterized gates map to functions that produce Gate constructors.
-SUPPORTED_GATES: Dict[str, Union[Gate, Callable[..., Gate]]] = {
+SUPPORTED_GATES: dict[str, Union[Gate, Callable[..., Gate]]] = {
     "CCNOT": CCNOT,
     "CNOT": CNOT,
     "CSWAP": CSWAP,
     "CPHASE": cphase,
     "CPHASE00": cphase00,
     "CPHASE01": cphase01,
     "CPHASE10": cphase10,
@@ -212,15 +212,15 @@
     "X": X,
     "Y": Y,
     "Z": Z,
     "XY": xy,
 }
 
 
-def parse_defgates(quil_str: str) -> Dict[str, np.ndarray]:
+def parse_defgates(quil_str: str) -> dict[str, np.ndarray]:
     """
     Parses non-parameterized DEFGATE definitions from a Quil program string.
 
     This function scans through the given Quil program string and extracts
     the definitions of custom gates defined using the DEFGATE directive.
     It only supports non-parameterized gate definitions. If a parameterized
     gate definition is encountered, the function raises a ValueError.
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/pyquil/cirq_quil_output.py` & `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/cirq/cirq_quil_output.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 # Copyright (C) 2022 The Cirq Developers
 #
 # This file is part of the qBraid-SDK.
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. This specific file, adapted from Cirq, is dual-licensed under both the
 # Apache License, Version 2.0, and the GPL v3. You may not use this file except in
@@ -19,15 +19,15 @@
 """
 Module defining qBraid Cirq QuilOutput.
 
 """
 
 import string
 from fractions import Fraction
-from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union, cast
+from typing import Any, Callable, Optional, Union, cast
 
 import cirq
 import numpy as np
 from cirq import ops, protocols, value
 
 
 def exponent_to_pi_string(exp: float) -> str:
@@ -58,15 +58,15 @@
     return f"{cnum.real}+{cnum.imag}i"
 
 
 class QuilFormatter(string.Formatter):
     """A unique formatter to correctly output values to QUIL."""
 
     def __init__(
-        self, qubit_id_map: Dict["cirq.Qid", str], measurement_id_map: Dict[str, str]
+        self, qubit_id_map: dict["cirq.Qid", str], measurement_id_map: dict[str, str]
     ) -> None:
         """Inits QuilFormatter.
 
         Args:
             qubit_id_map: A dictionary {qubit, quil_output_string} for
             the proper QUIL output for each qubit.
             measurement_id_map: A dictionary {measurement_key,
@@ -83,14 +83,15 @@
             value = self.qubit_id_map[value]
         if isinstance(value, str) and spec == "meas":
             value = self.measurement_id_map[value]
             spec = ""
         return super().format_field(value, spec)
 
 
+# pylint: disable=abstract-method
 @value.value_equality(approximate=True)
 class QuilOneQubitGate(ops.Gate):
     """A QUIL gate representing any single qubit unitary with a DEFGATE and
     2x2 matrix in QUIL.
     """
 
     def __init__(self, matrix: np.ndarray) -> None:
@@ -387,15 +388,15 @@
 
 class QuilOutput:
     """An object for passing operations and qubits then outputting them to
     QUIL format. The string representation returns the QUIL output for the
     circuit.
     """
 
-    def __init__(self, operations: "cirq.OP_TREE", qubits: Tuple["cirq.Qid", ...]) -> None:
+    def __init__(self, operations: "cirq.OP_TREE", qubits: tuple["cirq.Qid", ...]) -> None:
         """Inits QuilOutput.
 
         Args:
             operations: A list or tuple of `cirq.OP_TREE` arguments.
             qubits: The qubits used in the operations.
         """
         self.qubits = qubits
@@ -405,20 +406,20 @@
         )
         self.qubit_id_map = self._generate_qubit_ids()
         self.measurement_id_map = self._generate_measurement_ids()
         self.formatter = QuilFormatter(
             qubit_id_map=self.qubit_id_map, measurement_id_map=self.measurement_id_map
         )
 
-    def _generate_qubit_ids(self) -> Dict["cirq.Qid", str]:
+    def _generate_qubit_ids(self) -> dict["cirq.Qid", str]:
         return {qubit: str(i) for i, qubit in enumerate(self.qubits)}
 
-    def _generate_measurement_ids(self) -> Dict[str, str]:
+    def _generate_measurement_ids(self) -> dict[str, str]:
         index = 0
-        measurement_id_map: Dict[str, str] = {}
+        measurement_id_map: dict[str, str] = {}
         for op in self.operations:
             if isinstance(op.gate, ops.MeasurementGate):
                 key = protocols.measurement_key_name(op)
                 if key in measurement_id_map:
                     continue
                 measurement_id_map[key] = f"m{index}"
                 index += 1
@@ -446,15 +447,15 @@
         if not quil_str:
             raise ValueError("Can't convert Operation to string")
         return quil_str
 
     def _write_quil(self, output_func: Callable[[str], None]) -> None:
         output_func("# Created using qBraid.\n\n")
         if len(self.measurements) > 0:
-            measurements_declared: Set[str] = set()
+            measurements_declared: set[str] = set()
             for m in self.measurements:
                 key = protocols.measurement_key_name(m)
                 if key in measurements_declared:
                     continue
                 measurements_declared.add(key)
                 output_func(f"DECLARE {self.measurement_id_map[key]} BIT[{len(m.qubits)}]\n")
             output_func("\n")
@@ -537,17 +538,17 @@
             the `qubit_id_map` and `measurement_id_map`.
     """
 
     def __init__(
         self,
         *,
         operations: cirq.OP_TREE,
-        qubits: Tuple[cirq.Qid, ...],
-        decompose_operation: Optional[Callable[[cirq.Operation], List[cirq.Operation]]] = None,
-        qubit_id_map: Optional[Dict[cirq.Qid, str]] = None,
+        qubits: tuple[cirq.Qid, ...],
+        decompose_operation: Optional[Callable[[cirq.Operation], list[cirq.Operation]]] = None,
+        qubit_id_map: Optional[dict[cirq.Qid, str]] = None,
     ):
         """Initializes an instance of `RigettiQCSQuilOutput`.
 
         Args:
             operations: A list or tuple of `cirq.OP_TREE` arguments.
             qubits: The qubits used in the operations.
             decompose_operation: Optional; A callable that decomposes a circuit operation
@@ -577,15 +578,15 @@
         """
         if self._decompose_operation is None:
             super()._write_quil(output_func)
         else:
             output_func("# Created using qBraid.\n\n")
 
             if len(self.measurements) > 0:
-                measurements_declared: Set[str] = set()
+                measurements_declared: set[str] = set()
                 for m in self.measurements:
                     key = cirq.measurement_key_name(m)
                     if key in measurements_declared:
                         continue
                     measurements_declared.add(key)
                     output_func(f"DECLARE {self.measurement_id_map[key]} BIT[{len(m.qubits)}]\n")
                 output_func("\n")
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/pyquil/conversions_cirq.py` & `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/cirq/cirq_to_pyquil.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,80 +1,61 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
-Module containing functions to convert between Cirq's circuit
-representation and pyQuil's circuit representation (Quil programs).
+Module containing function to convert from Cirq's circuit
+representation to pyQuil's circuit representation (Quil programs).
 
 """
 from typing import TYPE_CHECKING
 
-from pyquil import Program
+from cirq import LineQubit, QubitOrder
 
+from qbraid._import import LazyLoader
 from qbraid.transpiler.exceptions import CircuitConversionError
 
+try:
+    from .cirq_quil_output import QuilOutput
+except ImportError:
+    QuilOutput = None
+
+pyquil = LazyLoader("pyquil", globals(), "pyquil")
+
 if TYPE_CHECKING:
     import cirq.circuits
-    import pyquil.quil
+    import pyquil as pyquil_
 
 
-def cirq_to_pyquil(circuit: "cirq.circuits.Circuit") -> "pyquil.quil.Program":
+def cirq_to_pyquil(circuit: "cirq.circuits.Circuit") -> "pyquil_.Program":
     """Returns a pyQuil Program equivalent to the input Cirq circuit.
 
     Args:
         circuit: Cirq circuit to convert to a pyQuil Program.
 
     Returns:
         pyquil.Program object equivalent to the input Cirq circuit.
     """
-    # pylint: disable=import-outside-toplevel
-    from cirq import LineQubit, QubitOrder
-
-    from .cirq_quil_output import QuilOutput
-
-    # pylint: enable=import-outside-toplevel
-
     input_qubits = circuit.all_qubits()
     max_qubit = max(input_qubits)
     # if we are using LineQubits, keep the qubit labeling the same
     if isinstance(max_qubit, LineQubit):
         qubit_range = max_qubit.x + 1
         qubit_order = LineQubit.range(qubit_range)
     # otherwise, use the default ordering (starting from zero)
     else:
         qubit_order = QubitOrder.DEFAULT
     qubits = QubitOrder.as_qubit_order(qubit_order).order_for(input_qubits)
     operations = circuit.all_operations()
     try:
         quil_str = str(QuilOutput(operations, qubits))
-        return Program(quil_str)
+        return pyquil.Program(quil_str)
     except ValueError as err:
         raise CircuitConversionError(
             f"Cirq qasm converter doesn't yet support {err.args[0][32:]}."
         ) from err
-
-
-def pyquil_to_cirq(program: "pyquil.quil.Program") -> "cirq.circuits.Circuit":
-    """Returns a Cirq circuit equivalent to the input pyQuil Program.
-
-    Args:
-        program: PyQuil Program to convert to a Cirq circuit.
-
-    Returns:
-        Cirq circuit representation equivalent to the input pyQuil Program.
-    """
-    # pylint: disable-next=import-outside-toplevel
-    from .cirq_quil_input import circuit_from_quil
-
-    try:
-        return circuit_from_quil(program.out())
-    except Exception as err:
-        raise CircuitConversionError(
-            "qBraid transpiler doesn't yet support pyQuil noise gates."
-        ) from err
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/pytket/conversions_qasm.py` & `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/pytket/pytket_to_qasm2.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
@@ -10,32 +10,20 @@
 
 """
 Module containing functions to convert between OpenQASM 2 and PyTKET.
 
 """
 from typing import TYPE_CHECKING
 
-from pytket.qasm import circuit_from_qasm_str, circuit_to_qasm_str
+from pytket.qasm import circuit_to_qasm_str
 
 if TYPE_CHECKING:
     import pytket.circuit
 
 
-def qasm2_to_pytket(qasm: str) -> "pytket.circuit.Circuit":
-    """Returns a pytket circuit equivalent to the input OpenQASM 2 string.
-
-    Args:
-        qasm (str): OpenQASM 2 string to convert to a pytket circuit.
-
-    Returns:
-        pytket.circuit.Circuit: PyTKET circuit object equivalent to input OpenQASM 2 string.
-    """
-    return circuit_from_qasm_str(qasm)
-
-
 def pytket_to_qasm2(circuit: "pytket.circuit.Circuit") -> str:
     """Returns an OpenQASM 2 string equivalent to the input pytket circuit.
 
     Args:
         circuit (pytket.circuit.Circuit): PyTKET circuit to convert to OpenQASM 2 string.
 
     Returns:
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/qiskit/__init__.py` & `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qiskit/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
@@ -15,14 +15,16 @@
 
 Functions
 ----------
 
 .. autosummary::
    :toctree: ../stubs/
 
-   qasm3_to_qiskit
-   qiskit_to_qasm3
-   qasm2_to_qiskit
    qiskit_to_qasm2
+   qiskit_to_qasm3
+   qiskit_to_braket
+   qiskit_to_pyqir
 
 """
-from .conversions_qasm import qasm2_to_qiskit, qasm3_to_qiskit, qiskit_to_qasm2, qiskit_to_qasm3
+from .qiskit_extras import qiskit_to_braket, qiskit_to_pyqir
+from .qiskit_to_qasm2 import qiskit_to_qasm2
+from .qiskit_to_qasm3 import qiskit_to_qasm3
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/qiskit/conversions_braket.py` & `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/braket/braket_extras.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,57 +5,49 @@
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
-Module defining Qiskit to Amazon Braket conversion(s)
+Module defining Amazon Braket conversion extras.
 
 """
 
 from typing import TYPE_CHECKING
 
+from qbraid._import import LazyLoader
 from qbraid.transpiler.annotations import requires_extras
 
+qiskit_braket_provider = LazyLoader("qiskit_braket_provider", globals(), "qiskit_braket_provider")
+pytket_braket = LazyLoader("pytket_braket", globals(), "pytket.extensions.braket")
+
 if TYPE_CHECKING:
     import braket.circuits
+    import pytket.circuit
     import qiskit.circuit
 
 
 @requires_extras("qiskit_braket_provider")
-def qiskit_to_braket(
-    circuit: "qiskit.circuit.QuantumCircuit", **kwargs
-) -> "braket.circuits.Circuit":
-    """Return a Braket quantum circuit from a Qiskit quantum circuit.
+def braket_to_qiskit(circuit: "braket.circuits.Circuit") -> "qiskit.circuit.QuantumCircuit":
+    """Return a Qiskit quantum circuit from a Braket quantum circuit.
 
     Args:
-        circuit (QuantumCircuit): Qiskit quantum circuit
-        basis_gates (Optional[Iterable[str]]): The gateset to transpile to.
-            If `None`, the transpiler will use all gates defined in the Braket SDK.
-            Default: `None`.
-        verbatim (bool): Whether to translate the circuit without any modification, in other
-            words without transpiling it. Default: False.
+        circuit (Circuit): Braket quantum circuit
 
     Returns:
-        Circuit: Braket circuit
+        QuantumCircuit: Qiskit quantum circuit
     """
-    # pylint: disable-next=import-outside-toplevel
-    from qiskit_braket_provider.providers.adapter import to_braket  # type: ignore
-
-    return to_braket(circuit, **kwargs)
+    return qiskit_braket_provider.providers.adapter.to_qiskit(circuit)
 
 
-@requires_extras("qiskit_braket_provider")
-def braket_to_qiskit(circuit: "braket.circuits.Circuit") -> "qiskit.circuit.QuantumCircuit":
-    """Return a Qiskit quantum circuit from a Braket quantum circuit.
+@requires_extras("pytket.extensions.braket")
+def braket_to_pytket(circuit: "braket.circuits.Circuit") -> "pytket.circuit.Circuit":
+    """Returns a pytket circuit equivalent to the input Amazon Braket circuit.
 
     Args:
-        circuit (Circuit): Braket quantum circuit
+        circuit (braket.circuits.Circuit): Braket circuit to convert to a pytket circuit.
 
     Returns:
-        QuantumCircuit: Qiskit quantum circuit
+        pytket.circuit.Circuit: PyTKET circuit object equivalent to input Braket circuit.
     """
-    # pylint: disable-next=import-outside-toplevel
-    from qiskit_braket_provider.providers.adapter import to_qiskit  # type: ignore
-
-    return to_qiskit(circuit)
+    return pytket_braket.braket_convert.braket_to_tk(circuit)
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/converter.py` & `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/converter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
@@ -11,58 +11,41 @@
 """
 Module for transpiling quantum programs between different quantum programming languages
 
 """
 import logging
 import warnings
 from copy import deepcopy
-from typing import TYPE_CHECKING, Callable, List, Optional
+from typing import TYPE_CHECKING, Callable, Optional
 
-from qbraid.programs import QPROGRAM_LIBS, get_program_type
+from qbraid.programs import QPROGRAM_ALIASES, ProgramTypeError, get_program_type_alias
 
 from .exceptions import CircuitConversionError, ConversionPathNotFoundError, NodeNotFoundError
 from .graph import ConversionGraph
 
 if TYPE_CHECKING:
-    import cirq
-
     import qbraid.programs
 
 
 logger = logging.getLogger(__name__)
 
 
 def _warn_if_unsupported(program_type, program_direction):
-    if program_type not in QPROGRAM_LIBS:
+    if program_type not in QPROGRAM_ALIASES:
         warnings.warn(
             f"Converting {program_direction} unsupported program type '{program_type}'.",
             UserWarning,
         )
 
 
-def _flatten_cirq(circuit: "cirq.Circuit") -> "cirq.Circuit":
-    """
-    Flatten a Cirq circuit.
-
-    Args:
-        circuit (cirq.Circuit): The Cirq circuit to flatten.
-
-    Returns:
-        cirq.Circuit: The flattened Cirq circuit.
-    """
-    # TODO: potentially replace with native cirq.decompose
-    # https://quantumai.google/reference/python/cirq/decompose
-
-    # pylint: disable=import-outside-toplevel
-    from cirq.contrib.qasm_import import circuit_from_qasm
-
-    return circuit_from_qasm(circuit.to_qasm())
+def _format_exception(err: Exception) -> str:
+    return f"{type(err).__name__}: {str(err)}\n"
 
 
-def _get_path_from_bound_methods(bound_methods: List[Callable]) -> str:
+def _get_path_from_bound_methods(bound_methods: list[Callable]) -> str:
     """
     Constructs a path string from a list of bound methods of Conversion instances.
 
     This function takes a list of bound methods (specifically 'convert' methods bound to
     Conversion instances) and constructs a path string representing the sequence of
     conversions. Each conversion is defined by the 'source' and 'target' properties of the
     Conversion instance to which each method is bound.
@@ -97,14 +80,15 @@
 
 def transpile(
     program: "qbraid.programs.QPROGRAM",
     target: str,
     conversion_graph: Optional[ConversionGraph] = None,
     max_path_attempts: int = 3,
     max_path_depth: Optional[int] = None,
+    **kwargs,
 ) -> "qbraid.programs.QPROGRAM":
     """
     Transpile a quantum program to a target language using a conversion graph.
     This function attempts to find a conversion path from the program's current
     format to the target format. It can limit the search to a certain number of
     attempts and path depths.
 
@@ -126,24 +110,24 @@
 
     Raises:
         NodeNotFoundError: If the target or source package is not in the ConversionGraph.
         ConversionPathNotFoundError: If no path is available to conversion between the
             source and target packages.
         CircuitConversionError: If the conversion fails through all attempted paths.
     """
-    graph = conversion_graph or ConversionGraph()
+    graph = conversion_graph or ConversionGraph(**kwargs)
     graph_type = "Default" if conversion_graph is None else "Provided"
 
     if not graph.has_node(target):
         raise NodeNotFoundError(graph_type, target, graph.nodes)
 
-    source = get_program_type(program, require_supported=conversion_graph is None)
+    source = get_program_type_alias(program)
 
     if not graph.has_node(source):
-        raise NodeNotFoundError(graph_type, target, graph.nodes)
+        raise NodeNotFoundError(graph_type, source, graph.nodes)
 
     if not graph.has_path(source, target):
         raise ConversionPathNotFoundError(source, target)
 
     if source == target:
         return program
 
@@ -153,32 +137,54 @@
     paths = graph.find_top_shortest_conversion_paths(source, target, top_n=max_path_attempts)
 
     if max_path_depth is not None:
         paths = [path for path in paths if len(path) <= max_path_depth]
         if len(paths) == 0:
             raise ConversionPathNotFoundError(source, target, max_path_depth)
 
+    error_messages = []
+
     for path in paths:
+        path_details = _get_path_from_bound_methods(path)
         temp_program = deepcopy(program)
         try:
             for convert_func in path:
                 try:
                     temp_program = convert_func(temp_program)
-                except Exception:  # pylint: disable=broad-exception-caught
-                    if get_program_type(temp_program) == "cirq":
-                        temp_program = _flatten_cirq(temp_program)
+                except Exception as err:  # pylint: disable=broad-exception-caught
+                    try:
+                        alias = get_program_type_alias(temp_program)
+                    except ProgramTypeError:
+                        alias = None
+
+                    if alias == "cirq":
+                        # pylint: disable=import-outside-toplevel
+                        from qbraid.transforms.cirq import decompose
+
+                        temp_program = decompose(temp_program)
                         temp_program = convert_func(temp_program)  # Retry conversion
                     else:
+                        error_detail = (
+                            f"Conversion {path_details} failed due to "
+                            f"exception raised while converting from '{alias}'."
+                        )
+                        error_messages.append(error_detail)
+                        error_messages.append(_format_exception(err))
                         raise
-            logger.info(
-                "\nSuccessfully transpiled using conversions: %s",
-                _get_path_from_bound_methods(path),
-            )
+
+            logger.info("\nSuccessfully transpiled using conversions: %s", path_details)
             return temp_program
-        except Exception:  # pylint: disable=broad-exception-caught
-            logger.info(
-                "\nFailed to transpile using conversions: %s",
-                _get_path_from_bound_methods(path),
-            )
+        except Exception as err:  # pylint: disable=broad-exception-caught
+            logger.info("\nFailed to transpile using conversions: %s", path_details)
+            formatted_error = _format_exception(err)
+            if len(error_messages) == 0 or error_messages[-1] != formatted_error:
+                error_messages.append(formatted_error)
             continue
 
-    raise CircuitConversionError(f"Failed to convert program from '{source}' to '{target}'.")
+    raise CircuitConversionError(
+        f"Failed to convert '{source}' to '{target}'"
+        + (
+            " due to the following error(s):\n\n" + "\n".join(error_messages)
+            if error_messages
+            else "."
+        )
+    )
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/edge.py` & `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/edge.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
@@ -12,15 +12,15 @@
 Module for defining custom conversions
 
 """
 import importlib
 import inspect
 from typing import TYPE_CHECKING, Any, Callable, Union
 
-from qbraid.programs import SUPPORTED_QPROGRAMS, get_program_type
+from qbraid.programs import QPROGRAM_REGISTRY, get_program_type_alias
 
 if TYPE_CHECKING:
     import qbraid
 
 
 class Conversion:
     """
@@ -36,20 +36,16 @@
             target (str): The target package to which conversion is done.
             conversion_func (Callable): The function that performs the actual conversion.
         """
         self._source = source
         self._target = target
         self._conversion_func = conversion_func
         self._extras = getattr(conversion_func, "requires_extras", [])
-
-        module = inspect.getmodule(conversion_func)
-        self._native = (
-            module is not None and module.__name__.startswith("qbraid") and len(self._extras) == 0
-        )
-        self._supported = self._check_supported()
+        self._native = self._is_module_native(conversion_func)
+        self._supported = self._is_conversion_supported()
 
     @property
     def source(self) -> str:
         """
         The source package of the conversion.
 
         Returns:
@@ -83,15 +79,33 @@
         True if all packages required to perform the conversion are installed. False otherwise.
 
         Returns:
             bool: Whether the conversion function supported in the current runtime environment.
         """
         return self._supported
 
-    def _check_supported(self) -> bool:
+    def _is_module_native(self, func: Callable) -> bool:
+        """
+        Determine if the function's module is 'qbraid' and requires no extras.
+
+        Args:
+            func (Callable): The function to check the module of.
+
+        Returns:
+            bool: True if the module is 'qbraid' and requires no extras, False otherwise.
+        """
+        module = inspect.getmodule(func)
+        is_native = (
+            module is not None
+            and module.__name__.split(".")[0] == "qbraid"
+            and len(self._extras) == 0
+        )
+        return is_native
+
+    def _is_conversion_supported(self) -> bool:
         """
         Determine if the required packages for the conversion are installed.
 
         Returns:
             bool: True if supported, otherwise False.
         """
         if self._native:
@@ -115,19 +129,19 @@
         Returns:
             Union[qbraid.programs.QPROGRAM, Any]: The converted quantum program,
                                          typically of a supported program type.
 
         Raises:
             ValueError: If the provided program's type does not match the source package type.
         """
-        package = get_program_type(program)
+        package = get_program_type_alias(program)
         if package != self._source:
             raise ValueError(
-                f"Expected program of type {SUPPORTED_QPROGRAMS[self._source]}, "
-                f"but got program of type {SUPPORTED_QPROGRAMS[package]}."
+                f"Expected program of type {QPROGRAM_REGISTRY[self._source]}, "
+                f"but got program of type {QPROGRAM_REGISTRY[package]}."
             )
         return self._conversion_func(program)
 
     def __repr__(self) -> str:
         """
         Represent the Conversion instance as a string indicating
         source and target packages.
@@ -150,8 +164,10 @@
         if not isinstance(other, Conversion):
             return False
 
         return (
             self._source == other._source
             and self._target == other._target
             and self._native == other._native
+            and self._supported == other._supported
+            and self._extras == other._extras
         )
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/exceptions.py` & `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
 Module defining exceptions for errors raised during conversions
 
 """
-from typing import List, Optional
+from typing import Optional
 
 from qbraid.exceptions import QbraidError
 
 
 class CircuitConversionError(QbraidError):
     """Base class for errors raised while converting a circuit."""
 
 
 class NodeNotFoundError(ValueError, QbraidError):
     """Class for errors raised when a node is not present in a ConversionGraph."""
 
-    def __init__(self, graph_type: str, package: str, nodes: List[str]):
+    def __init__(self, graph_type: str, package: str, nodes: list[str]):
         message = (
             f"{graph_type} conversion graph does not contain node '{package}'. "
             f"Supported nodes are: {nodes}"
         )
         super().__init__(message)
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/graph.py` & `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
@@ -10,15 +10,15 @@
 
 """
 Module providing tools to map, analyze, and visualize conversion paths between different
 quantum programs available through the qbraid.transpiler using directed graphs.
 
 """
 from importlib import import_module
-from typing import List, Optional
+from typing import Optional
 
 import networkx as nx
 
 from .conversions import conversion_functions
 from .edge import Conversion
 from .exceptions import ConversionPathNotFoundError
 
@@ -26,62 +26,62 @@
 class ConversionGraph(nx.DiGraph):
     """
     Class for coordinating conversions between different quantum software programs
 
     """
 
     def __init__(
-        self, conversions: Optional[List[Conversion]] = None, requires_extras: bool = False
+        self, conversions: Optional[list[Conversion]] = None, require_native: bool = False
     ):
         """
         Initialize a ConversionGraph instance.
 
         Args:
-            conversions (optional, List[Conversion]): List of conversion edges. If None, default
-                                                          conversion edges are created.
-            requires_extras (bool): If True, include unsupported "requires_extras" conversion
-                                    functions. Defaults to False.
+            conversions (optional, list[Conversion]): List of conversion edges. If None,
+                                                      default conversion edges are used.
+            require_native (bool): If True, only include "native" conversion functions.
+                                   Defaults to False.
         """
         super().__init__()
-        self.requires_extras = requires_extras
+        self.require_native = require_native
         self._conversions = conversions or self.load_default_conversions()
         self.create_conversion_graph()
 
     @staticmethod
-    def load_default_conversions() -> List[Conversion]:
+    def load_default_conversions() -> list[Conversion]:
         """
         Create a list of default conversion nodes using predefined conversion functions.
 
         Returns:
-            List[Conversion]: List of default conversion edges.
+            list[Conversion]: List of default conversion edges.
         """
         transpiler = import_module("qbraid.transpiler.conversions")
         return [
             Conversion(*conversion.split("_to_"), getattr(transpiler, conversion))
             for conversion in conversion_functions
         ]
 
     def create_conversion_graph(self) -> None:
         """
         Create a directed graph from a list of conversion functions.
 
         Returns:
             None
         """
-        for edge in self._conversions:
-            if not self.requires_extras and not edge.supported:
-                continue
+        for edge in (
+            e for e in self._conversions if e.supported and (not self.require_native or e.native)
+        ):
             self.add_edge(edge.source, edge.target, native=edge.native, func=edge.convert)
 
-    def conversions(self) -> List[Conversion]:
+    def conversions(self) -> list[Conversion]:
         """
         Get the list of conversion edges.
 
         Returns:
-            List[Conversion]: The conversion edges of the graph.
+            list[Conversion]: The conversion edges of the graph.
         """
         return self._conversions
 
     def add_conversion(self, edge: Conversion, overwrite: bool = False) -> None:
         """
         Add a new conversion function as an edge in the graph.
 
@@ -118,15 +118,15 @@
 
         self._conversions = [
             conv
             for conv in self._conversions.copy()
             if not (conv.source == source and conv.target == target)
         ]
 
-    def find_shortest_conversion_path(self, source: str, target: str) -> List[str]:
+    def find_shortest_conversion_path(self, source: str, target: str) -> list[str]:
         """
         Find the shortest conversion path between two nodes in a graph.
 
         Args:
             source (str): The starting node for the path.
             target (str): The target node for the path.
 
@@ -140,15 +140,15 @@
             path = nx.shortest_path(self, source, target)
             return [self[path[i]][path[i + 1]]["func"] for i in range(len(path) - 1)]
         except nx.NetworkXNoPath as err:
             raise ConversionPathNotFoundError(source, target) from err
 
     def find_top_shortest_conversion_paths(
         self, source: str, target: str, top_n: int = 3
-    ) -> List[List[str]]:
+    ) -> list[list[str]]:
         """
         Find the top shortest conversion paths between two nodes in a graph.
 
         Args:
             source (str): The starting node for the path.
             target (str): The target node for the path.
             top_n (int): Number of top shortest paths to find.
@@ -178,15 +178,15 @@
             target (str): The target language.
 
         Returns:
             bool: True if the conversion is supported, False otherwise.
         """
         return nx.has_path(self, source, target)
 
-    def reset(self, conversions: Optional[List[Conversion]] = None) -> None:
+    def reset(self, conversions: Optional[list[Conversion]] = None) -> None:
         """
         Reset the graph to its default state.
 
         Returns:
             None
         """
         self.clear()
@@ -199,11 +199,11 @@
 
         Args:
             **kwargs: Keyword arguments for the plot function.
 
         Returns:
             None
         """
-        # pylint: disable=import-outside-toplevel
+        # pylint: disable-next=import-outside-toplevel
         from qbraid.visualization.plot_conversions import plot_conversion_graph
 
         plot_conversion_graph(self, **kwargs)
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/visualization/__init__.py` & `qbraid-0.7.0.dev20240516020308/qbraid/visualization/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/visualization/draw_circuit.py` & `qbraid-0.7.0.dev20240516020308/qbraid/visualization/draw_circuit.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
@@ -10,15 +10,15 @@
 
 """
 Module for drawing quantum circuit diagrams
 
 """
 from typing import TYPE_CHECKING, Optional
 
-from qbraid.programs import QPROGRAM_LIBS, ProgramTypeError, get_program_type
+from qbraid.programs import QPROGRAM_ALIASES, ProgramTypeError, get_program_type_alias
 from qbraid.transpiler.converter import transpile
 
 from .draw_qasm3 import qasm3_drawer
 from .exceptions import VisualizationError
 
 if TYPE_CHECKING:
     import qbraid.programs
@@ -34,17 +34,17 @@
 
     Args:
         :data:`~.qbraid.programs.QPROGRAM`: Supported quantum program
 
     Raises:
         ProgramTypeError: If quantum program is not of a supported type
     """
-    package = get_program_type(program)
+    package = get_program_type_alias(program)
 
-    if as_package and as_package != package and as_package in QPROGRAM_LIBS:
+    if as_package and as_package != package and as_package in QPROGRAM_ALIASES:
         program = transpile(program, as_package)
         package = as_package
 
     # pylint: disable=import-outside-toplevel
 
     if package == "qiskit":
         from qiskit.visualization import circuit_drawer as qiskit_drawer
@@ -103,17 +103,17 @@
         )
 
     if package == "qasm3":
         return qasm3_drawer(program)
 
     if package == "qasm2":
         # coverage: ignore
-        if "cirq" in QPROGRAM_LIBS:
+        if "cirq" in QPROGRAM_ALIASES:
             program = transpile(program, "cirq")
-        elif "qiskit" in QPROGRAM_LIBS:
+        elif "qiskit" in QPROGRAM_ALIASES:
             program = transpile(program, "qiskit")
         else:
             program = transpile(program, "qasm3")
 
         return circuit_drawer(program, output=output, **kwargs)
 
     if package == "pennylane":
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/visualization/draw_qasm3.py` & `qbraid-0.7.0.dev20240516020308/qbraid/visualization/draw_qasm3.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/visualization/plot_conversions.py` & `qbraid-0.7.0.dev20240516020308/qbraid/visualization/plot_conversions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,43 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 """
 Module for plotting qBraid transpiler quantum program conversion graphs.
 
 """
-from typing import TYPE_CHECKING, Dict, Optional
+from typing import TYPE_CHECKING, Optional
 
-import matplotlib.pyplot as plt
 import networkx as nx
 
-from qbraid.programs._import import QPROGRAM_LIBS
+from qbraid._import import LazyLoader
+from qbraid.programs.registry import is_registered_alias_native
 
 if TYPE_CHECKING:
     import qbraid.transpiler
 
+plt = LazyLoader("plt", globals(), "matplotlib.pyplot")
+
 
 def plot_conversion_graph(  # pylint: disable=too-many-arguments
     graph: "qbraid.transpiler.ConversionGraph",
     title: Optional[str] = "qBraid Quantum Program Conversion Graph",
     legend: bool = False,
     seed: Optional[int] = None,
     node_size: int = 1200,
     min_target_margin: int = 18,
     show: bool = True,
     save_path: Optional[str] = None,
-    colors: Optional[Dict[str, str]] = None,
+    colors: Optional[dict[str, str]] = None,
 ) -> None:
     """
     Plot the conversion graph using matplotlib. The graph is displayed using node
     and edge color conventions, with options for a title, legend, and figure saving.
 
     Args:
         graph (qbraid.interface.ConversionGraph): The directed conversion graph to be plotted.
@@ -45,15 +47,15 @@
         seed (Optional[int]): Seed for the node layout algorithm. Useful for consistent positioning.
                               Defaults to None.
         node_size (int): Size of the nodes. Defaults to 1200.
         min_target_margin (int): Minimum target margin for edges. Defaults to 18.
         show (bool): If True, display the figure. Defaults to True.
         save_path (Optional[str]): Path to save the figure. If None, the figure is not saved.
                                    Defaults to None.
-        colors (Optional[Dict[str, str]]): Dictionary for node and edge colors. Expected keys are
+        colors (Optional[dict[str, str]]): Dictionary for node and edge colors. Expected keys are
             'qbraid_node', 'external_node', 'qbraid_edge', 'external_edge'. Defaults to None.
 
     Returns:
         None
     """
     # Set default colors if not provided
     if colors is None:
@@ -63,15 +65,15 @@
             "qbraid_edge": "gray",
             "external_edge": "blue",
             "extras_edge": "red",
         }
 
     # Extract colors and apply them in the drawing
     ncolors = [
-        colors["qbraid_node"] if node in QPROGRAM_LIBS else colors["external_node"]
+        colors["qbraid_node"] if is_registered_alias_native(node) else colors["external_node"]
         for node in graph.nodes()
     ]
 
     # Create a dictionary for quick lookup of conversions by their source and target
     conversion_dict = {
         (conversion.source, conversion.target): conversion for conversion in graph.conversions()
     }
@@ -80,15 +82,15 @@
         for edge in graph.edges()
         if (edge[0], edge[1]) in conversion_dict
     ]
     ecolors = [
         (
             colors["qbraid_edge"]
             if graph[edge.source][edge.target]["native"]
-            else colors["external_edge"] if edge.supported else colors["extras_edge"]
+            else colors["extras_edge"] if len(edge._extras) > 0 else colors["external_edge"]
         )
         for edge in conversions_ordered
     ]
 
     pos = nx.spring_layout(graph, seed=seed)  # good seeds: 123, 134
     nx.draw_networkx_nodes(graph, pos, node_color=ncolors, node_size=node_size)
     nx.draw_networkx_edges(graph, pos, edge_color=ecolors, min_target_margin=min_target_margin)
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid/visualization/plot_counts.py` & `qbraid-0.7.0.dev20240516020308/qbraid/visualization/plot_counts.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
 Module for plotting historgram of measurement counts against quantum states.
 
 """
 
-from typing import Callable, Dict, List, Optional, Union
+from typing import Callable, Optional, Union
 
-import matplotlib.pyplot as plt
-from matplotlib import colormaps
+from qbraid._import import LazyLoader
+
+plt = LazyLoader("plt", globals(), "matplotlib.pyplot")
+matplotlib = LazyLoader("matplotlib", globals(), "matplotlib")
 
 # pylint: disable=too-many-arguments,unnecessary-lambda
 
 
 def _counts_to_decimal(counts: dict) -> dict:
     """
     Converts a dictionary of counts to decimal form.
@@ -52,17 +54,17 @@
 
     decimal_dict = {key: value / total_count for key, value in counts.items()}
 
     return decimal_dict
 
 
 def _plot_data(
-    counts: Union[List[Dict], dict],
-    legend: Optional[Union[List[str], str]] = None,
-    colors: Optional[Union[List[str], str]] = None,
+    counts: Union[list[dict], dict],
+    legend: Optional[Union[list[str], str]] = None,
+    colors: Optional[Union[list[str], str]] = None,
     title: Optional[str] = None,
     x_label: Optional[str] = None,
     y_label: Optional[str] = None,
     show_plot: Optional[bool] = True,
     save_path: Optional[str] = None,
     transform_fn: Optional[Callable[[dict], dict]] = None,
     label_format_fn: Optional[Callable[[float], str]] = lambda x: str(x),
@@ -81,15 +83,15 @@
 
     num_dicts = len(counts)
     bar_width = 0.8 / num_dicts
 
     x_positions = range(len(all_states))
 
     if colors is None:
-        cmap = colormaps.get_cmap("tab10")
+        cmap = matplotlib.colormaps.get_cmap("tab10")
         colors = [cmap(i / 10) for i in range(num_dicts)]
 
     if len(colors) != len(counts):
         raise ValueError("Number of colors must match number of datasets")
 
     if isinstance(legend, list) and len(legend) != len(counts):
         raise ValueError("Number of legend labels must match number of datasets")
@@ -147,34 +149,34 @@
         plt.savefig(save_path)
 
     if show_plot:
         plt.show()
 
 
 def plot_distribution(
-    counts: Union[List[Dict], Dict],
-    legend: Optional[Union[List[str], str]] = None,
-    colors: Optional[Union[List[str], str]] = None,
+    counts: Union[list[dict], dict],
+    legend: Optional[Union[list[str], str]] = None,
+    colors: Optional[Union[list[str], str]] = None,
     title: Optional[str] = None,
     x_label: Optional[str] = None,
     y_label: Optional[str] = None,
     show_plot: Optional[bool] = True,
     save_path: Optional[str] = None,
 ):
     """
     Plots a histogram probability distribution of quantum states.
 
     Args:
-        counts (Union[List[Dict], Dict]): Dictionary or a list of dictionaries containing the
+        counts (Union[list[Dict], Dict]): Dictionary or a list of dictionaries containing the
                                           quantum states as keys and their respective counts as
                                           values.
-        legend (Optional[Union[List[str], str]]): List of strings or a single string representing
+        legend (Optional[Union[list[str], str]]): List of strings or a single string representing
                                                   the labels of the datasets. Defaults to None,
                                                   where it generates default labels.
-        colors (Optional[Union[List[str], str]]): List of strings or a single string representing
+        colors (Optional[Union[list[str], str]]): List of strings or a single string representing
                                                   the colors for each dataset. Defaults to None,
                                                   where it generates a color sequence.
         title (Optional[str]): String representing the title of the plot. Defaults to None.
         x_label (Optional[str]): String representing the label for the x-axis. Defaults to None.
         y_label (Optional[str]): String representing the label for the y-axis. Defaults to None.
         show_plot (Optional[bool]): Boolean representing whether to show the plot. Defaults to True.
         save_path (Optional[str]): String representing the path to save the plot. Defaults to None.
@@ -214,34 +216,34 @@
         save_path,
         transform_fn=_counts_to_decimal,
         label_format_fn=lambda x: "{:.3f}".format(x),  # pylint: disable=consider-using-f-string
     )
 
 
 def plot_histogram(
-    counts: Union[List[Dict], Dict],
-    legend: Optional[Union[List[str], str]] = None,
-    colors: Optional[Union[List[str], str]] = None,
+    counts: Union[list[dict], dict],
+    legend: Optional[Union[list[str], str]] = None,
+    colors: Optional[Union[list[str], str]] = None,
     title: Optional[str] = None,
     x_label: Optional[str] = None,
     y_label: Optional[str] = None,
     show_plot: Optional[bool] = True,
     save_path: Optional[str] = None,
 ):
     """
     Plots a histogram of measurement counts against quantum states.
 
     Args:
-        counts (Union[List[Dict], Dict]): Dictionary or a list of dictionaries containing the
+        counts (Union[list[Dict], Dict]): Dictionary or a list of dictionaries containing the
                                           quantum states as keys and their respective counts as
                                           values.
-        legend (Optional[Union[List[str], str]]): List of strings or a single string representing
+        legend (Optional[Union[list[str], str]]): List of strings or a single string representing
                                                   the labels of the datasets. Defaults to None,
                                                   where it generates default labels.
-        colors (Optional[Union[List[str], str]]): List of strings or a single string representing
+        colors (Optional[Union[list[str], str]]): List of strings or a single string representing
                                                   the colors for each dataset. Defaults to None,
                                                   where it generates a color sequence.
         title (Optional[str]): String representing the title of the plot. Defaults to None.
         x_label (Optional[str]): String representing the label for the x-axis. Defaults to None.
         y_label (Optional[str]): String representing the label for the y-axis. Defaults to None.
         show_plot (Optional[bool]): Boolean representing whether to show the plot. Defaults to True.
         save_path (Optional[str]): String representing the path to save the plot. Defaults to None.
```

### Comparing `qbraid-0.7.0.dev20240423224133/qbraid.egg-info/SOURCES.txt` & `qbraid-0.7.0.dev20240516020308/qbraid.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 CODE_OF_CONDUCT.md
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
+SECURITY.md
 pyproject.toml
 requirements-dev.txt
 requirements.txt
 tox.ini
 docs/conf.py
 docs/index.rst
 docs/_static/favicon.ico
@@ -26,16 +27,16 @@
 docs/_static/sdk-files/conversion_graph.png
 docs/_static/sdk-files/get_devices.png
 docs/_static/sdk-files/hub_spokes.png
 docs/_static/sdk-files/lab_jobs.png
 docs/_static/sdk-files/plot_counts.png
 docs/api/qbraid.interface.rst
 docs/api/qbraid.programs.rst
-docs/api/qbraid.providers.rst
 docs/api/qbraid.rst
+docs/api/qbraid.runtime.rst
 docs/api/qbraid.transforms.rst
 docs/api/qbraid.transpiler.rst
 docs/api/qbraid.visualization.rst
 docs/sdk/devices.rst
 docs/sdk/jobs.rst
 docs/sdk/overview.rst
 docs/sdk/programs.rst
@@ -45,16 +46,15 @@
 qbraid/__init__.py
 qbraid/_about.py
 qbraid/_compat.py
 qbraid/_display.py
 qbraid/_import.py
 qbraid/_version.py
 qbraid/exceptions.py
-qbraid/get_devices.py
-qbraid/get_jobs.py
+qbraid/py.typed
 qbraid.egg-info/PKG-INFO
 qbraid.egg-info/SOURCES.txt
 qbraid.egg-info/dependency_links.txt
 qbraid.egg-info/entry_points.txt
 qbraid.egg-info/requires.txt
 qbraid.egg-info/top_level.txt
 qbraid/interface/__init__.py
@@ -62,85 +62,119 @@
 qbraid/interface/random/__init__.py
 qbraid/interface/random/cirq_random.py
 qbraid/interface/random/qasm3_random.py
 qbraid/interface/random/qiskit_random.py
 qbraid/interface/random/random.py
 qbraid/programs/__init__.py
 qbraid/programs/_import.py
-qbraid/programs/abc_program.py
+qbraid/programs/alias_manager.py
 qbraid/programs/exceptions.py
-qbraid/programs/inspector.py
 qbraid/programs/loader.py
-qbraid/programs/qasm_passes.py
-qbraid/programs/qasm_qelib1.py
+qbraid/programs/program.py
+qbraid/programs/registry.py
+qbraid/programs/spec.py
 qbraid/programs/libs/__init__.py
 qbraid/programs/libs/braket.py
 qbraid/programs/libs/cirq.py
 qbraid/programs/libs/pennylane.py
 qbraid/programs/libs/pyquil.py
 qbraid/programs/libs/pytket.py
 qbraid/programs/libs/qasm2.py
 qbraid/programs/libs/qasm3.py
 qbraid/programs/libs/qiskit.py
-qbraid/providers/__init__.py
-qbraid/providers/_import.py
-qbraid/providers/device.py
-qbraid/providers/enums.py
-qbraid/providers/exceptions.py
-qbraid/providers/job.py
-qbraid/providers/provider.py
-qbraid/providers/result.py
-qbraid/providers/status_maps.py
-qbraid/providers/aws/__init__.py
-qbraid/providers/aws/device.py
-qbraid/providers/aws/job.py
-qbraid/providers/aws/provider.py
-qbraid/providers/aws/result.py
-qbraid/providers/aws/tracker.py
-qbraid/providers/ibm/__init__.py
-qbraid/providers/ibm/device.py
-qbraid/providers/ibm/job.py
-qbraid/providers/ibm/provider.py
-qbraid/providers/ibm/result.py
+qbraid/runtime/__init__.py
+qbraid/runtime/_display.py
+qbraid/runtime/device.py
+qbraid/runtime/enums.py
+qbraid/runtime/exceptions.py
+qbraid/runtime/job.py
+qbraid/runtime/profile.py
+qbraid/runtime/provider.py
+qbraid/runtime/result.py
+qbraid/runtime/braket/__init__.py
+qbraid/runtime/braket/device.py
+qbraid/runtime/braket/job.py
+qbraid/runtime/braket/provider.py
+qbraid/runtime/braket/result.py
+qbraid/runtime/braket/tracker.py
+qbraid/runtime/ionq/__init__.py
+qbraid/runtime/ionq/device.py
+qbraid/runtime/ionq/job.py
+qbraid/runtime/ionq/provider.py
+qbraid/runtime/ionq/result.py
+qbraid/runtime/native/__init__.py
+qbraid/runtime/native/device.py
+qbraid/runtime/native/job.py
+qbraid/runtime/native/provider.py
+qbraid/runtime/native/result.py
+qbraid/runtime/qiskit/__init__.py
+qbraid/runtime/qiskit/device.py
+qbraid/runtime/qiskit/job.py
+qbraid/runtime/qiskit/provider.py
+qbraid/runtime/qiskit/result.py
 qbraid/transforms/__init__.py
 qbraid/transforms/exceptions.py
+qbraid/transforms/braket/__init__.py
+qbraid/transforms/braket/transform.py
+qbraid/transforms/cirq/__init__.py
+qbraid/transforms/cirq/passes.py
 qbraid/transforms/pytket/__init__.py
 qbraid/transforms/pytket/ionq.py
+qbraid/transforms/qasm2/__init__.py
+qbraid/transforms/qasm2/passes.py
+qbraid/transforms/qasm2/qasm_qelib1.py
+qbraid/transforms/qasm3/__init__.py
+qbraid/transforms/qasm3/compat.py
+qbraid/transforms/qiskit/__init__.py
+qbraid/transforms/qiskit/transform.py
 qbraid/transpiler/__init__.py
 qbraid/transpiler/annotations.py
 qbraid/transpiler/converter.py
 qbraid/transpiler/edge.py
 qbraid/transpiler/exceptions.py
 qbraid/transpiler/graph.py
+qbraid/transpiler/scheme.py
 qbraid/transpiler/conversions/__init__.py
 qbraid/transpiler/conversions/braket/__init__.py
-qbraid/transpiler/conversions/braket/cirq_from_braket.py
-qbraid/transpiler/conversions/braket/cirq_to_braket.py
-qbraid/transpiler/conversions/braket/conversions_cirq.py
-qbraid/transpiler/conversions/braket/conversions_qasm.py
-qbraid/transpiler/conversions/braket/custom_instr.py
+qbraid/transpiler/conversions/braket/braket_extras.py
+qbraid/transpiler/conversions/braket/braket_to_cirq.py
+qbraid/transpiler/conversions/braket/braket_to_qasm3.py
 qbraid/transpiler/conversions/cirq/__init__.py
-qbraid/transpiler/conversions/cirq/cirq_qasm_parser.py
-qbraid/transpiler/conversions/cirq/conversions_qasm.py
-qbraid/transpiler/conversions/cirq/custom_ops.py
+qbraid/transpiler/conversions/cirq/braket_custom.py
+qbraid/transpiler/conversions/cirq/cirq_extras.py
+qbraid/transpiler/conversions/cirq/cirq_quil_output.py
+qbraid/transpiler/conversions/cirq/cirq_to_braket.py
+qbraid/transpiler/conversions/cirq/cirq_to_pyquil.py
+qbraid/transpiler/conversions/cirq/cirq_to_qasm2.py
 qbraid/transpiler/conversions/openqasm3/__init__.py
-qbraid/transpiler/conversions/openqasm3/conversions_qasm.py
+qbraid/transpiler/conversions/openqasm3/openqasm3_to_qasm3.py
 qbraid/transpiler/conversions/pennylane/__init__.py
-qbraid/transpiler/conversions/pennylane/conversions_qasm.py
+qbraid/transpiler/conversions/pennylane/pennylane_to_qasm2.py
 qbraid/transpiler/conversions/pyquil/__init__.py
 qbraid/transpiler/conversions/pyquil/cirq_quil_input.py
-qbraid/transpiler/conversions/pyquil/cirq_quil_output.py
-qbraid/transpiler/conversions/pyquil/conversions_cirq.py
+qbraid/transpiler/conversions/pyquil/pyquil_to_cirq.py
 qbraid/transpiler/conversions/pytket/__init__.py
-qbraid/transpiler/conversions/pytket/conversions_braket.py
-qbraid/transpiler/conversions/pytket/conversions_qasm.py
+qbraid/transpiler/conversions/pytket/pytket_extras.py
+qbraid/transpiler/conversions/pytket/pytket_to_qasm2.py
+qbraid/transpiler/conversions/qasm2/__init__.py
+qbraid/transpiler/conversions/qasm2/cirq_custom.py
+qbraid/transpiler/conversions/qasm2/cirq_qasm_parser.py
+qbraid/transpiler/conversions/qasm2/qasm2_to_cirq.py
+qbraid/transpiler/conversions/qasm2/qasm2_to_pytket.py
+qbraid/transpiler/conversions/qasm2/qasm2_to_qasm3.py
+qbraid/transpiler/conversions/qasm2/qasm2_to_qiskit.py
+qbraid/transpiler/conversions/qasm3/__init__.py
+qbraid/transpiler/conversions/qasm3/qasm3_extras.py
+qbraid/transpiler/conversions/qasm3/qasm3_to_braket.py
+qbraid/transpiler/conversions/qasm3/qasm3_to_openqasm3.py
+qbraid/transpiler/conversions/qasm3/qasm3_to_qiskit.py
 qbraid/transpiler/conversions/qiskit/__init__.py
-qbraid/transpiler/conversions/qiskit/conversions_braket.py
-qbraid/transpiler/conversions/qiskit/conversions_qasm.py
+qbraid/transpiler/conversions/qiskit/qiskit_extras.py
+qbraid/transpiler/conversions/qiskit/qiskit_to_qasm2.py
+qbraid/transpiler/conversions/qiskit/qiskit_to_qasm3.py
 qbraid/visualization/__init__.py
 qbraid/visualization/draw_circuit.py
 qbraid/visualization/draw_qasm3.py
 qbraid/visualization/exceptions.py
 qbraid/visualization/plot_conversions.py
 qbraid/visualization/plot_counts.py
-tools/set_provider_configs.py
-tools/verify_headers.py
+tools/set_provider_configs.py
```

### Comparing `qbraid-0.7.0.dev20240423224133/tools/set_provider_configs.py` & `qbraid-0.7.0.dev20240516020308/tools/set_provider_configs.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 qBraid
+# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
@@ -11,37 +11,48 @@
 """
 Set config inside testing virtual environments with default values
 hard-coded and secret values read from environment variables.
 
 Note: this script is intended for CI/CD purposes only.
 
 """
+import logging
 import os
 from typing import Optional
 
 from qbraid_core import QbraidSession
 from qbraid_core.services.quantum.proxy_braket import aws_configure
-from qiskit_ibm_provider import IBMProvider
 
 # Skip tests if IBM/AWS account auth/creds not configured
 skip_remote_tests: bool = os.getenv("QBRAID_RUN_REMOTE_TESTS", "False").lower() != "true"
 REASON = "QBRAID_RUN_REMOTE_TESTS not set (requires configuration of qBraid storage)"
 
+logger = logging.getLogger(__name__)
+
 
 def qbraid_configure(api_key: Optional[str] = None) -> None:
     """Initializes qBraid configuration and credentials files."""
     api_key = api_key or os.getenv("QBRAID_API_KEY", "MYAPIKEY")
     session = QbraidSession(api_key=api_key)
     session.save_config()
 
 
-def ibm_configure(token: Optional[str] = None, overwrite: bool = True, **kwargs) -> None:
+def ibm_configure(
+    token: Optional[str] = None, channel: Optional[str] = None, overwrite: bool = True, **kwargs
+) -> None:
     """Initializes IBM Quantum configuration and credentials files."""
-    token = token or os.getenv("QISKIT_IBM_TOKEN", "MYTOKEN")
-    IBMProvider.save_account(token=token, overwrite=overwrite, **kwargs)
+    # pylint: disable-next=import-outside-toplevel
+    from qiskit_ibm_runtime import QiskitRuntimeService
+
+    token = token or os.getenv("QISKIT_IBM_TOKEN", "MY_IBM_QUANTUM_TOKEN")
+    channel = channel or os.getenv("QISKIT_IBM_CHANNEL", "ibm_quantum")
+    QiskitRuntimeService.save_account(token=token, channel=channel, overwrite=overwrite, **kwargs)
 
 
 if __name__ == "__main__":
     if not skip_remote_tests:
         qbraid_configure()
         aws_configure()
-        ibm_configure()
+        try:
+            ibm_configure()
+        except ImportError:
+            logger.error("qiskit-ibm-runtime not installed, skipping IBM Quantum configuration")
```

### Comparing `qbraid-0.7.0.dev20240423224133/tox.ini` & `qbraid-0.7.0.dev20240516020308/tox.ini`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 [tox]
-requires =
-    tox>=4.2
+minversion = 4.2.0
 env_list =
     unit-tests
     docs
     linters
     format-check
 skip_missing_interpreter = true
 
@@ -23,24 +22,24 @@
 
 [testenv:unit-tests]
 description = Run pytests and generate coverage report.
 commands =
     python3 tools/set_provider_configs.py
     coverage run -m pytest -x tests/programs \
                               tests/transpiler \
-                              tests/providers \
                               tests/transforms \
+                              tests/runtime \
                               tests/visualization \
                               tests/top_level \
                            -W ignore::DeprecationWarning \
                            -W ignore::PendingDeprecationWarning \
                            -W ignore::urllib3.exceptions.InsecureRequestWarning \
                            -W ignore::RuntimeWarning
     coverage combine
-    coverage report --omit=qbraid/transpiler/conversions/cirq/custom_ops.py,qbraid/visualization/draw_circuit.py,qbraid/visualization/plot_conversions.py,qbraid/_compat.py
+    coverage report --omit=qbraid/visualization/draw_circuit.py,qbraid/visualization/plot_conversions.py,qbraid/_compat.py
     coverage html
     coverage xml
 
 [testenv:docs]
 description = Use sphinx to build the HTML docs.
 extras =
     docs
@@ -67,34 +66,37 @@
 deps = black
 commands = 
     black qbraid tools tests --exclude /(tests/transpiler/cirq/test_qasm_parser.py)/ {posargs}
 
 [testenv:headers]
 envdir = .tox/linters
 skip_install = true
-deps =
+deps = qbraid-cli
 commands = 
-    python tools/verify_headers.py qbraid tests tools {posargs}
+    qbraid admin headers tests tools qbraid --type=gpl {posargs}
 
 [testenv:linters]
+allowlist_externals = qbraid
 envdir = .tox/linters
 skip_install = true
 deps =
     {[testenv:isort]deps}
     {[testenv:black]deps}
 commands =
     {[testenv:isort]commands}
     {[testenv:black]commands}
     {[testenv:headers]commands} {posargs:--fix}
 
 [testenv:format-check]
+allowlist_externals = qbraid
 envdir = .tox/linters
 skip_install = true
 deps =
     {[testenv:pylint]deps}
     {[testenv:isort]deps}
     {[testenv:black]deps}
+    {[testenv:headers]deps}
 commands =
     {[testenv:pylint]commands}
     {[testenv:isort]commands} {posargs:--check-only}
     {[testenv:black]commands} {posargs:--check}
     {[testenv:headers]commands}
```

