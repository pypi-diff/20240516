# Comparing `tmp/DMT_core-2.0.0.tar.gz` & `tmp/DMT_core-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DMT_core-2.0.0.tar", last modified: Tue Jul 18 12:49:35 2023, max compression
+gzip compressed data, was "DMT_core-2.1.0.tar", last modified: Thu May 16 19:05:10 2024, max compression
```

## Comparing `DMT_core-2.0.0.tar` & `DMT_core-2.1.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:49:35.381547 DMT_core-2.0.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:49:35.369547 DMT_core-2.0.0/DMT/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:49:35.370547 DMT_core-2.0.0/DMT/Hdev/
--rw-rw-rw-   0 root         (0) root         (0)      954 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/Hdev/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    42089 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/Hdev/dut_hdev.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:49:35.371547 DMT_core-2.0.0/DMT/config/
--rw-rw-rw-   0 root         (0) root         (0)     2932 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/config/DMT_config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     6905 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/config/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:49:35.377547 DMT_core-2.0.0/DMT/core/
--rw-rw-rw-   0 root         (0) root         (0)     4425 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8634 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/circuit.py
--rw-rw-rw-   0 root         (0) root         (0)     3205 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/constants.py
--rw-rw-rw-   0 root         (0) root         (0)    90055 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/data_frame.py
--rw-rw-rw-   0 root         (0) root         (0)    34879 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/data_processor.py
--rw-rw-rw-   0 root         (0) root         (0)    27057 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/data_reader.py
--rw-rw-rw-   0 root         (0) root         (0)     8779 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/database_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     9998 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/df_to_sweep.py
--rw-rw-rw-   0 root         (0) root         (0)      159 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/dmt_units.txt
--rw-rw-rw-   0 root         (0) root         (0)    42237 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/docu_dut_lib.py
--rw-rw-rw-   0 root         (0) root         (0)    10578 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/dut_circuit.py
--rw-rw-rw-   0 root         (0) root         (0)     4676 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/dut_dummy.py
--rw-rw-rw-   0 root         (0) root         (0)    71359 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/dut_lib.py
--rw-rw-rw-   0 root         (0) root         (0)    12163 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/dut_meas.py
--rw-rw-rw-   0 root         (0) root         (0)     8116 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/dut_tcad.py
--rw-rw-rw-   0 root         (0) root         (0)    13057 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/dut_type.py
--rw-rw-rw-   0 root         (0) root         (0)    41817 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/dut_view.py
--rw-rw-rw-   0 root         (0) root         (0)     2452 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/hasher.py
--rw-rw-rw-   0 root         (0) root         (0)    50056 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/mc_parameter.py
--rw-rw-rw-   0 root         (0) root         (0)     7171 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/mc_skywater.py
--rw-rw-rw-   0 root         (0) root         (0)    28046 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/mcard.py
--rw-rw-rw-   0 root         (0) root         (0)    38026 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/naming.py
--rw-rw-rw-   0 root         (0) root         (0)    82840 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/plot.py
--rw-rw-rw-   0 root         (0) root         (0)    22847 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/plot_2yaxis.py
--rw-rw-rw-   0 root         (0) root         (0)    11669 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/plot_smith.py
--rw-rw-rw-   0 root         (0) root         (0)    36689 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/sim_con.py
--rw-rw-rw-   0 root         (0) root         (0)     2859 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/singleton.py
--rw-rw-rw-   0 root         (0) root         (0)    31475 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/sweep.py
--rw-rw-rw-   0 root         (0) root         (0)    18223 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/sweep_def.py
--rw-rw-rw-   0 root         (0) root         (0)     8298 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/technology.py
--rw-rw-rw-   0 root         (0) root         (0)     2319 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    11995 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/va_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:49:35.377547 DMT_core-2.0.0/DMT/exceptions/
--rw-rw-rw-   0 root         (0) root         (0)     3007 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/exceptions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:49:35.378547 DMT_core-2.0.0/DMT/external/
--rw-rw-rw-   0 root         (0) root         (0)      883 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/external/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10703 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/external/latex.py
--rw-rw-rw-   0 root         (0) root         (0)     3201 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/external/os.py
--rw-rw-rw-   0 root         (0) root         (0)     5532 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/external/pylatex.py
--rwxrwxrwx   0 root         (0) root         (0)     5331 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/external/pypi.py
--rw-rw-rw-   0 root         (0) root         (0)     5111 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/external/verilogae.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:49:35.378547 DMT_core-2.0.0/DMT/libautodoc_template/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:49:35.378547 DMT_core-2.0.0/DMT/libautodoc_template/base/
--rw-rw-rw-   0 root         (0) root         (0)      848 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/libautodoc_template/base/acronyms.tex
--rw-rw-rw-   0 root         (0) root         (0)     4056 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/libautodoc_template/base/header.tex
--rw-rw-rw-   0 root         (0) root         (0)        6 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/libautodoc_template/bib.bib
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:49:35.379546 DMT_core-2.0.0/DMT/libautodoc_template/content/
--rw-rw-rw-   0 root         (0) root         (0)      789 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/libautodoc_template/content/conclusion.tex
--rw-rw-rw-   0 root         (0) root         (0)     1262 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/libautodoc_template/content/deckblatt.tex
--rw-rw-rw-   0 root         (0) root         (0)     1317 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/libautodoc_template/content/introduction.tex
--rw-rw-rw-   0 root         (0) root         (0)     1236 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/libautodoc_template/documentation.tex
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:49:35.379546 DMT_core-2.0.0/DMT/ngspice/
--rw-rw-rw-   0 root         (0) root         (0)      891 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/ngspice/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    46941 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/ngspice/dut_ngspice.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:49:35.379546 DMT_core-2.0.0/DMT/xyce/
--rw-rw-rw-   0 root         (0) root         (0)      980 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/xyce/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    38969 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/xyce/dut_xyce.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:49:35.380546 DMT_core-2.0.0/DMT_core.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5865 2023-07-18 12:49:35.000000 DMT_core-2.0.0/DMT_core.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1547 2023-07-18 12:49:35.000000 DMT_core-2.0.0/DMT_core.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 12:49:35.000000 DMT_core-2.0.0/DMT_core.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      478 2023-07-18 12:49:35.000000 DMT_core-2.0.0/DMT_core.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-07-18 12:49:35.000000 DMT_core-2.0.0/DMT_core.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)    35333 2023-07-18 12:49:29.000000 DMT_core-2.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5865 2023-07-18 12:49:35.380546 DMT_core-2.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4646 2023-07-18 12:49:29.000000 DMT_core-2.0.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-07-18 12:49:29.000000 DMT_core-2.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 12:49:35.381547 DMT_core-2.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2182 2023-07-18 12:49:34.000000 DMT_core-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:05:10.882325 DMT_core-2.1.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:05:10.869325 DMT_core-2.1.0/DMT/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:05:10.870325 DMT_core-2.1.0/DMT/Hdev/
+-rw-rw-rw-   0 root         (0) root         (0)      954 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/Hdev/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    42838 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/Hdev/dut_hdev.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:05:10.871325 DMT_core-2.1.0/DMT/config/
+-rw-rw-rw-   0 root         (0) root         (0)     2932 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/config/DMT_config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     6910 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/config/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:05:10.877325 DMT_core-2.1.0/DMT/core/
+-rw-rw-rw-   0 root         (0) root         (0)     4465 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9382 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/core/circuit.py
+-rw-rw-rw-   0 root         (0) root         (0)     3206 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/core/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    96942 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/core/data_frame.py
+-rw-rw-rw-   0 root         (0) root         (0)    35848 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/core/data_processor.py
+-rw-rw-rw-   0 root         (0) root         (0)    27069 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/core/data_reader.py
+-rw-rw-rw-   0 root         (0) root         (0)     8780 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/core/database_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     9999 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/core/df_to_sweep.py
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/core/dmt_units.txt
+-rw-rw-rw-   0 root         (0) root         (0)    48708 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/core/docu_dut_lib.py
+-rw-rw-rw-   0 root         (0) root         (0)    11194 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/core/dut_circuit.py
+-rw-rw-rw-   0 root         (0) root         (0)     4676 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/core/dut_dummy.py
+-rw-rw-rw-   0 root         (0) root         (0)    74714 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/core/dut_lib.py
+-rw-rw-rw-   0 root         (0) root         (0)    12170 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/core/dut_meas.py
+-rw-rw-rw-   0 root         (0) root         (0)     8169 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/core/dut_tcad.py
+-rw-rw-rw-   0 root         (0) root         (0)    14387 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/core/dut_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    43477 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/core/dut_view.py
+-rw-rw-rw-   0 root         (0) root         (0)     2460 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/core/hasher.py
+-rw-rw-rw-   0 root         (0) root         (0)    51866 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/core/mc_parameter.py
+-rw-rw-rw-   0 root         (0) root         (0)     7139 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/core/mc_skywater.py
+-rw-rw-rw-   0 root         (0) root         (0)    29088 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/core/mcard.py
+-rw-rw-rw-   0 root         (0) root         (0)    38500 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/core/naming.py
+-rw-rw-rw-   0 root         (0) root         (0)    82715 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/core/plot.py
+-rw-rw-rw-   0 root         (0) root         (0)    22950 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/core/plot_2yaxis.py
+-rw-rw-rw-   0 root         (0) root         (0)    11670 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/core/plot_smith.py
+-rw-rw-rw-   0 root         (0) root         (0)    37411 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/core/sim_con.py
+-rw-rw-rw-   0 root         (0) root         (0)     2860 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/core/singleton.py
+-rw-rw-rw-   0 root         (0) root         (0)    32538 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/core/sweep.py
+-rw-rw-rw-   0 root         (0) root         (0)    19071 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/core/sweep_def.py
+-rw-rw-rw-   0 root         (0) root         (0)     8641 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/core/technology.py
+-rw-rw-rw-   0 root         (0) root         (0)     2319 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/core/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    12287 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/core/va_file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:05:10.877325 DMT_core-2.1.0/DMT/exceptions/
+-rw-rw-rw-   0 root         (0) root         (0)     3007 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/exceptions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:05:10.878325 DMT_core-2.1.0/DMT/external/
+-rw-rw-rw-   0 root         (0) root         (0)      884 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/external/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10704 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/external/latex.py
+-rw-rw-rw-   0 root         (0) root         (0)     3201 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/external/os.py
+-rw-rw-rw-   0 root         (0) root         (0)     5599 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/external/pylatex.py
+-rwxrwxrwx   0 root         (0) root         (0)     6850 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/external/pypi.py
+-rw-rw-rw-   0 root         (0) root         (0)     5193 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/external/verilogae.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:05:10.879325 DMT_core-2.1.0/DMT/libautodoc_template/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:05:10.879325 DMT_core-2.1.0/DMT/libautodoc_template/base/
+-rw-rw-rw-   0 root         (0) root         (0)      848 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/libautodoc_template/base/acronyms.tex
+-rw-rw-rw-   0 root         (0) root         (0)     4056 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/libautodoc_template/base/header.tex
+-rw-rw-rw-   0 root         (0) root         (0)        6 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/libautodoc_template/bib.bib
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:05:10.880325 DMT_core-2.1.0/DMT/libautodoc_template/content/
+-rw-rw-rw-   0 root         (0) root         (0)      789 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/libautodoc_template/content/conclusion.tex
+-rw-rw-rw-   0 root         (0) root         (0)     1262 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/libautodoc_template/content/deckblatt.tex
+-rw-rw-rw-   0 root         (0) root         (0)     1317 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/libautodoc_template/content/introduction.tex
+-rw-rw-rw-   0 root         (0) root         (0)     1236 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/libautodoc_template/documentation.tex
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:05:10.880325 DMT_core-2.1.0/DMT/ngspice/
+-rw-rw-rw-   0 root         (0) root         (0)      891 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/ngspice/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    47883 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/ngspice/dut_ngspice.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:05:10.880325 DMT_core-2.1.0/DMT/xyce/
+-rw-rw-rw-   0 root         (0) root         (0)      980 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/xyce/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    40760 2024-05-16 19:05:06.000000 DMT_core-2.1.0/DMT/xyce/dut_xyce.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:05:10.881325 DMT_core-2.1.0/DMT_core.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6050 2024-05-16 19:05:10.000000 DMT_core-2.1.0/DMT_core.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1547 2024-05-16 19:05:10.000000 DMT_core-2.1.0/DMT_core.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 19:05:10.000000 DMT_core-2.1.0/DMT_core.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      487 2024-05-16 19:05:10.000000 DMT_core-2.1.0/DMT_core.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2024-05-16 19:05:10.000000 DMT_core-2.1.0/DMT_core.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)    35333 2024-05-16 19:05:06.000000 DMT_core-2.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6050 2024-05-16 19:05:10.881325 DMT_core-2.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4831 2024-05-16 19:05:06.000000 DMT_core-2.1.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       99 2024-05-16 19:05:06.000000 DMT_core-2.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-16 19:05:10.882325 DMT_core-2.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2202 2024-05-16 19:05:10.000000 DMT_core-2.1.0/setup.py
```

### Comparing `DMT_core-2.0.0/DMT/Hdev/__init__.py` & `DMT_core-2.1.0/DMT/Hdev/__init__.py`

 * *Files identical despite different names*

### Comparing `DMT_core-2.0.0/DMT/Hdev/dut_hdev.py` & `DMT_core-2.1.0/DMT/Hdev/dut_hdev.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """ Manges a device under test which can be simulated by Hdev using the TCAD Interface class.
 
 Author: Markus Müller
 """
+
 # DMT_core
 # Copyright (C) from 2022  SemiMod
 # Copyright (C) until 2021  Markus Müller, Mario Krattenmacher and Pascal Kuthe
 # <https://gitlab.com/dmt-development/dmt-core>
 #
 # This file is part of DMT_core.
 #
@@ -26,17 +27,16 @@
 import re
 import copy
 import os
 import numpy as np
 import pandas as pd
 import logging
 import h5py
-from typing import cast
 import shutil
-from typing import List, Dict
+from typing import cast, List, Dict, Type
 
 try:
     from semver.version import Version as VersionInfo
 except ImportError:
     from semver import VersionInfo
 
 from DMT.core import (
@@ -94,25 +94,26 @@
 
     Attributes
     ----------
     sim_name : str
         DEVICE simulation title. Sort of a DUT-Name.
 
     """
+
     inited = False
 
     def __init__(
         self,
         database_dir,
         dut_type,
         inp_structure,
         name="hdev_",
         simulator_command=None,
         inp_name="hdev_inp.din",
-        **kwargs
+        **kwargs,
     ):
         if simulator_command is None:
             simulator_command = COMMANDS["Hdev"]
 
         super().__init__(
             database_dir,
             name,
@@ -146,26 +147,26 @@
             }
         }
 
     @classmethod
     def from_json(
         cls,
         json_content: Dict,
-        classes_technology: List[type[Technology]],
+        classes_technology: List[Type[Technology]],
         subclass_kwargs: Dict = None,
     ) -> "DutHdev":
         """Static class method. Loads a DutHdev object from a json or pickle file with full path save_dir.
 
         Calls the from_json method of DutView with all dictionary inside the "parent" keyword. Afterwards the additional parameters are set correctly.
 
         Parameters
         ----------
         json_content  :  dict
             Readed dictionary from a saved json DutHdev.
-        classes_technology : List[type[Technology]]
+        classes_technology : List[Type[Technology]]
             All possible technologies this loaded DutHdev can have. One will be choosen according to the serialized technology loaded from the file.
         subclass_kwargs : Dict, optional
             Additional kwargs necessary to create the concrete subclassed DutView.
 
         Returns
         -------
         DutHdev
@@ -527,21 +528,22 @@
 
                     dfs_temp.append(df_dc)
                     dfs_temp.append(df_ac)
 
                     n = n + 1
 
                 # create new big dataframe with DC and AC data
-                df_iv = pd.concat(dfs_temp)
+                df_iv = pd.concat(dfs_temp, ignore_index=True)
 
             # convert columns to specifiers
             df_iv = df_iv.real2cmplx()
             for _col in df_iv.columns:
                 df_iv.rename(
-                    columns={_col: get_specifier_from_string(_col, nodes=self.nodes)}, inplace=True
+                    columns={_col: get_specifier_from_string(_col, nodes=self.nodes)},
+                    inplace=True,
                 )
 
             if not df_iv.columns.is_unique:
                 df_iv = df_iv.loc[:, ~df_iv.columns.duplicated()]
 
             try:
                 freqs = np.unique(df_iv[specifiers.FREQUENCY].to_numpy())
@@ -551,15 +553,16 @@
 
                 # ensure some columns
                 df_iv.ensure_specifier_column(specifiers.CAPACITANCE + "B" + "E", ports=["B", "C"])
                 df_iv.ensure_specifier_column(specifiers.CAPACITANCE + "B" + "C", ports=["B", "C"])
                 df_iv.ensure_specifier_column(specifiers.TRANSIT_FREQUENCY, ports=["B", "C"])
                 df_iv.ensure_specifier_column(specifiers.TRANSCONDUCTANCE, ports=["B", "C"])
                 df_iv.ensure_specifier_column(
-                    specifiers.SS_PARA_Y + "C" + "B" + sub_specifiers.REAL, ports=["B", "C"]
+                    specifiers.SS_PARA_Y + "C" + "B" + sub_specifiers.REAL,
+                    ports=["B", "C"],
                 )
             except KeyError:
                 pass
 
             if (
                 ac and len(dfs_inqu) > 0
             ):  # only one frequency simulated => post process (maybe also check for 1D)
@@ -584,15 +587,15 @@
                     qp = np.zeros(len(df_iv))
                     qn = np.zeros(len(df_iv))
                     for i_row, _row in enumerate(df_iv.iterrows()):
                         try:
                             key_inqu = next(
                                 _key
                                 for _key in self.data.keys()
-                                if "_inqu" in _key and "op" + str(i_row + 1) in _key
+                                if key in _key and "_inqu" in _key and "op" + str(i_row + 1) in _key
                             )
                         except:
                             continue
                         df_inqu = self.data[key_inqu]
                         qn[i_row] = np.trapz(df_inqu["N"], df_inqu["X"])
                         qp[i_row] = np.trapz(df_inqu["P"], df_inqu["X"])
 
@@ -605,36 +608,39 @@
                     tau_be = np.ones(len(df_iv))
                     tau_b = np.ones(len(df_iv))
                     tau_c = np.ones(len(df_iv))
                     tau_bc = np.ones(len(df_iv))
 
                     try:
                         for i_row, row in enumerate(df_iv.iterrows()):
-                            key_inqu = next(
-                                _key
-                                for _key in self.data.keys()
-                                if "_inqu" in _key and "op" + str(i_row + 1) in _key
-                            )
-                            key_ac_inqu = next(
-                                _key
-                                for _key in self.data.keys()
-                                if "acinqu" in _key
-                                and "op" + str(i_row + 1) in _key
-                                and "dVb" in _key
-                            )
+                            key_inqu = self.join_key(key, f"op{i_row+1}_inqu")
+                            # next(
+                            #     _key
+                            #     for _key in self.data.keys()
+                            #     if key in _key and "_inqu" in _key and "op" + str(i_row + 1) in _key
+                            # )
+                            key_ac_inqu = self.join_key(key, f"acinqu_op{i_row+1}_dVb")
+                            # key_ac_inqu = next(
+                            #     _key
+                            #     for _key in self.data.keys()
+                            #     if key in _key
+                            #     and "acinqu" in _key
+                            #     and "op" + str(i_row + 1) in _key
+                            #     and "dVb" in _key
+                            # )
 
                             # get the necessary data
                             df_ac_inqu_i = self.data[key_ac_inqu]
-                            dn_dic = df_ac_inqu_i["re_d_n_x"].to_numpy() / gm[i_row + 1]
+                            dn_dic = df_ac_inqu_i["re_d_n_x"].to_numpy() / gm[i_row]
                             try:
-                                dn2_dic = df_ac_inqu_i["re_d_n2_x"].to_numpy() / gm[i_row + 1]
+                                dn2_dic = df_ac_inqu_i["re_d_n2_x"].to_numpy() / gm[i_row]
                             except KeyError:
-                                dn2_dic = df_ac_inqu_i["re_d_n_x"].to_numpy() / gm[i_row + 1]
+                                dn2_dic = df_ac_inqu_i["re_d_n_x"].to_numpy() / gm[i_row]
 
-                            dp_dic = df_ac_inqu_i["re_d_p_x"].to_numpy() / gm[i_row + 1]
+                            dp_dic = df_ac_inqu_i["re_d_p_x"].to_numpy() / gm[i_row]
                             droh_dic = dp_dic - dn_dic
                             # transit time
                             changes = (
                                 np.where(np.sign(droh_dic[:-1]) != np.sign(droh_dic[1:]))[0] + 1
                             )
                             index_be = changes[np.argmin(np.abs(changes - junctions[0]))]
                             index_bc = changes[np.argmin(np.abs(changes - junctions[1]))]
@@ -695,18 +701,20 @@
 
                         df_iv["tau_e"] = tau_e
                         df_iv["tau_be"] = tau_be
                         df_iv["tau_b"] = tau_b
                         df_iv["tau_bc"] = tau_bc
                         df_iv["tau_c"] = tau_c
 
-                    except:
-                        pass
+                    except Exception as err:
+                        print(err)
+                        # pass
 
             key_iv = self.join_key(key, "iv")
+            df_iv.index = [a for a in range(df_iv.shape[0])]
             self.data[key_iv] = df_iv
 
             logging.info(
                 "Read the Hdev simulation output data of the sweep %s. \nThe simulation folder is %s",
                 sweep.name,
                 sim_folder,
             )
@@ -872,15 +880,19 @@
                     else:
                         raise NotImplementedError
                     dummy = 1
                     break
 
         elif sub_sweep.sweep_type.startswith("LIST"):
             bias_fun = "'TAB'"  # we convert to list, to support list=1 setting used by DMT in Hdev
-            bias_info = {"cont_name": cont_name, "bias_fun": bias_fun, "bias_val": sub_sweep.values}
+            bias_info = {
+                "cont_name": cont_name,
+                "bias_fun": bias_fun,
+                "bias_val": sub_sweep.values,
+            }
         else:
             raise NotImplementedError
 
         return bias_info  # type: ignore
 
     def get_mobility(self, semiconductor, valley, field, temperature, doping, grading):
         if not DutHdev.inited:
@@ -919,15 +931,25 @@
                         grading,
                     )
         else:
             mob = np.zeros_like(field)
             for i in range(len(field)):
                 if doping > 0:
                     mob[i] = hdev_py.get_mobility_py(
-                        semiconductor, valley, field[i], 1, 1, 1, temperature, 0, doping, 0, grading
+                        semiconductor,
+                        valley,
+                        field[i],
+                        1,
+                        1,
+                        1,
+                        temperature,
+                        0,
+                        doping,
+                        0,
+                        grading,
                     )
                     # def get_mobility_py(semi_name     ,valley,f       , ec_l, ec_r, dim, t, dens, don, acc,  grad):
                 else:
                     mob[i] = hdev_py.get_mobility_py(
                         semiconductor,
                         valley,
                         field[i],
@@ -1042,14 +1064,15 @@
     tn=True,
     no_inqu=False,
     lambda_e=None,
     xj_l=None,
     mu_min_a=None,
     mu_min_d=None,
     beta=None,
+    **kwargs,
 ):
     """Return a DutHdev for ITRS HBTS. Only for SiGe HBTs.
 
     Parameters
     ----------
     hbt_fun : callable
         Function that returns a Hdev HBT definition.
@@ -1120,8 +1143,9 @@
     inp = turn_off_recombination(inp)
 
     return DutHdev(
         None,
         DutType.npn,
         inp,
         reference_node="E",
+        **kwargs,
     )
```

### Comparing `DMT_core-2.0.0/DMT/config/DMT_config.yaml` & `DMT_core-2.1.0/DMT/config/DMT_config.yaml`

 * *Files identical despite different names*

### Comparing `DMT_core-2.0.0/DMT/config/__init__.py` & `DMT_core-2.1.0/DMT/config/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """ DMT config management
 
 Collects the config from 3 different locations:
 
 * Local script directory (DMT_config.yaml).
-* User's home directory (%LOCALAPPDATA%\DMT\DMT_config.yaml or $XDG_CONFIG_HOME/DMT/DMT_config.yaml with $XDG_CONFIG_HOME defaulting to ~/.config) and
+* User's home directory (%LOCALAPPDATA%\\DMT\\DMT_config.yaml or $XDG_CONFIG_HOME/DMT/DMT_config.yaml with $XDG_CONFIG_HOME defaulting to ~/.config) and
 * DMT package installation directory (DMT/config/DMT_config.yaml)
 
 They are all read and finally taken in the order given here. This means that anything given in the local directory overwrites all others.
 
 """
+
 # DMT_core
 # Copyright (C) from 2022  SemiMod
 # Copyright (C) until 2021  Markus Müller, Mario Krattenmacher and Pascal Kuthe
 # <https://gitlab.com/dmt-development/dmt-core>
 #
 # This file is part of DMT_core.
 #
@@ -68,15 +69,15 @@
 except FileNotFoundError:
     try:
         user_config_old = Path.home() / ".DMT" / "DMT_config.yaml"
         data_user = yaml.safe_load(user_config_old.read_text())
         warnings.warn(
             (
                 "The DMT user configuration file has been moved. The new paths are:\n"
-                + "Windows: %LOCALAPPDATA%\DMT\DMT_config.yaml\n"
+                + "Windows: %LOCALAPPDATA%\\DMT\\DMT_config.yaml\n"
                 + "Linux and MacOS: $XDG_CONFIG_HOME/DMT/DMT_config.yaml\n"
                 + "Defaulting to ~/.config/DMT/DMT_config.yaml"
             ),
             category=DeprecationWarning,
         )
     except FileNotFoundError:
         pass
```

### Comparing `DMT_core-2.0.0/DMT/core/__init__.py` & `DMT_core-2.1.0/DMT/core/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 from .plot import COMPARISON_3
 from .plot_smith import SmithPlot
 from .plot_2yaxis import Plot2YAxis
 
 # Data management and processing
 from .data_processor import is_iterable, flatten, strictly_increasing, DataProcessor
 
-from .data_frame import DataFrame
+from .data_frame import DataFrame, df_concat
 from .sweep_def import SweepDef
 from .sweep import Sweep, get_sweepdef
 from .database_manager import DatabaseManager
 from .data_reader import (
     read_data,
     save_elpa,
     read_ADS_bin,
@@ -121,26 +121,25 @@
 # docu
 from .docu_dut_lib import DocuDutLib
 
 # determine which modules are present
 core_exists = True  # always, without DMT is not possible
 try:
     pkgutil.find_loader("DMT.extraction")
-    # import DMT.extraction
-
     extraction_exists = True
 except ImportError:
     extraction_exists = False
-
-
-if core_exists and not extraction_exists:
-    mode = "free version"
-elif core_exists and extraction_exists:
-    mode = "all"
+try:
+    pkgutil.find_loader("DMT.hl2")
+    bjt_exists = True
+except ImportError:
+    bjt_exists = False
 
 print("-----------------------------------------------------------------------")
 print("DMT Copyright (C) 2022 SemiMod")
 print("This program comes with ABSOLUTELY NO WARRANTY.")
-print("DMT_core is free software, and you are welcome to redistribute it.")
+print("DMT.core is free software and licensed under GPLv3.")
 if extraction_exists:
-    print("DMT_other is free for non-commercial use, see LICENSE.md. ")
+    print("DMT.extraction is free software and licensed under GPLv3.")
+if bjt_exists:
+    print("other DMT modules are free for non-commercial use, see LICENSE.md. ")
 print("-----------------------------------------------------------------------")
```

### Comparing `DMT_core-2.0.0/DMT/core/circuit.py` & `DMT_core-2.1.0/DMT/core/circuit.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """ DMT description of a circuit.
 
 Must be used to describe a circuit and then passed to a circuit simulator dut.
 
 Later on this can be extended to allow (pseudo-)simulations directly inside DMT.
 
 """
+
 # DMT_core
 # Copyright (C) from 2022  SemiMod
 # Copyright (C) until 2021  Markus Müller, Mario Krattenmacher and Pascal Kuthe
 # <https://gitlab.com/dmt-development/dmt-core>
 #
 # This file is part of DMT_core.
 #
@@ -21,25 +22,27 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>
 from __future__ import annotations
-import warnings
-from typing import Callable, Iterable, Optional, Union, List, Tuple
-from DMT.core import MCard, McParameterCollection
+from pathlib import Path
+from typing import Iterable, Optional, Union, List, Tuple
+from DMT.core import MCard, McParameterCollection, VAFileMap
 
 
 RESISTANCE = "R"
 """ Indicates a resistance in a circuit. """
 CAPACITANCE = "C"
 """ Indicates a capacitance in a circuit. """
 INDUCTANCE = "L"
 """ Indicates a inductance in a circuit. """
+SUBCIRCUIT = "X"
+""" Indicates a subcircuit in a circuit. """
 CURRENT = "I_Source"
 """ Indicates a current source in a circuit. """
 VOLTAGE = "V_Source"
 """ Indicates a voltage source in a circuit. """
 SHORT = "Short"
 """ Indicates a voltage source in a circuit. """
 HICUML2_HBT = "BHT"
@@ -86,14 +89,15 @@
 
     possible_types = [
         VOLTAGE,
         CURRENT,
         RESISTANCE,
         CAPACITANCE,
         INDUCTANCE,
+        SUBCIRCUIT,
         SHORT,
         HICUML2_HBT,
         HICUML0_HBT,
         SGP_BJT,
         DIODE,
         "va_module",
         "pdk",
@@ -101,14 +105,16 @@
         '"hbt_n1m"',
         '"n1m"',
         '"n1s"',
         "n1s_sgp",
         "n1m_sgp",
         "hbt_n1s",
         "hbt_n1m",
+        "npn13G2",
+        '"npn13G2"',
         "n1m",
         "n1s",
         "hbt_n2s",
         '"hbt_n2s"',
         "hbt_n3s",
         '"npn_hicum"',
         '"npn_hs"',
@@ -178,22 +184,24 @@
         elif isinstance(parameters, list):
             for i_parameter, parameter in enumerate(parameters):
                 if isinstance(parameter, tuple):
                     for parameter_part in parameter:
                         if not isinstance(parameter_part, str):
                             raise TypeError(
                                 "The parameters have to be a list of tuple of strings! Given was a list of tuples with at least one element of "
-                                + type(parameter_part)
+                                + str(type(parameter_part))
                                 + " in the tuple "
                                 + str(i_parameter)
                             )
+                elif isinstance(parameter, str):
+                    pass
                 else:
                     raise TypeError(
-                        "The parameters have to be a list of tuple of strings! Given was a list with at least one element of "
-                        + type(parameter)
+                        "The parameters have to be a list of tuples of strings or strings! Given was a list with at least one element of "
+                        + str(type(parameter))
                         + " at position "
                         + str(i_parameter)
                     )
 
         elif isinstance(parameters, MCard) or isinstance(parameters, McParameterCollection):
             # Allow model cards!
             pass
@@ -226,18 +234,34 @@
 
     Raises
     ------
     TypeError
         If one element of the circuit to create is neither a :class:`~DMT.core.circuit.CircuitElement` nor a simple str.
     """
 
-    def __init__(self, circuit_elements: List[Union[str, CircuitElement]]):
+    def __init__(
+        self,
+        circuit_elements: List[Union[str, CircuitElement]],
+        lib_files: List[Union[str, Path]] = None,
+        va_root_files: List[Union[str, Path, VAFileMap]] = None,
+    ):
         for i_element, element in enumerate(circuit_elements):
             if not isinstance(element, (CircuitElement, str)):
                 raise TypeError(
                     "The netlist has to be a list of CircuitElement or str! At position "
                     + str(i_element)
                     + " is a entry of type "
                     + type(element)
                 )
 
         self.netlist = circuit_elements
+        if lib_files is None:
+            self.lib_files = []
+        else:
+            self.lib_files = lib_files
+
+        self.verilog_maps = []
+        if va_root_files is not None:
+            for va_file in va_root_files:
+                if not isinstance(va_file, VAFileMap):
+                    va_file = VAFileMap(va_file)
+                self.verilog_maps.append(va_file)
```

### Comparing `DMT_core-2.0.0/DMT/core/constants.py` & `DMT_core-2.1.0/DMT/core/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 Namings :
 
 *  M is a mathematical constant
 *  P is a physical constant. The constants have been taken from http://physics.nist.gov
 *  others: HICUM constants
 
 """
+
 # DMT_core
 # Copyright (C) from 2022  SemiMod
 # Copyright (C) until 2021  Markus Müller, Mario Krattenmacher and Pascal Kuthe
 # <https://gitlab.com/dmt-development/dmt-core>
 #
 # This file is part of DMT_core.
 #
```

### Comparing `DMT_core-2.0.0/DMT/core/data_frame.py` & `DMT_core-2.1.0/DMT/core/data_frame.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """ data_frame module
 
 Implements a extended pandas.DataFrame. It is based on the pandas.DataFrame and extended by many special methods that simplify working with electrical quantities.
 This includes easy management of small signal parameter and other quantities which can be calculated from them.
 
 """
+
 # DMT_core
 # Copyright (C) from 2022  SemiMod
 # Copyright (C) until 2021  Markus Müller, Mario Krattenmacher and Pascal Kuthe
 # <https://gitlab.com/dmt-development/dmt-core>
 #
 # This file is part of DMT_core.
 #
@@ -19,32 +20,32 @@
 # DMT_core is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>
-import numpy as np
 import re
 import logging
 import copy
+import numpy as np
+import pandas as pd
 from scipy.optimize import curve_fit
+from typing import Iterator, Tuple, Dict
 from DMT.exceptions import UnknownColumnError
+from DMT.core.data_processor import DataProcessor, flatten
 from DMT.core import (
     specifiers_ss_para,
     get_specifier_from_string,
     specifiers,
     SpecifierStr,
     sub_specifiers,
     get_nodes,
     get_sub_specifiers,
-    flatten,
-    DataProcessor,
 )
-import pandas as pd
 
 # pylint: disable = too-many-lines
 
 
 # helper functions for Y Parameter smoothing
 def fun_re(freq, a1, a2, a3):
     """Fit function for real Y Parameters normalized."""
@@ -384,15 +385,16 @@
         unknown_columns = []
         for col in self.columns:
             if col in fallback.keys():
                 # the complete column name is in the fallback. So use it!
                 if fallback[col] is None:
                     if warnings:
                         logging.warning(
-                            "The column %s is dropped as it is in the fallback dictionary!", col
+                            "The column %s is dropped as it is in the fallback dictionary!",
+                            col,
                         )
                     # drop it!
                 elif fallback[col]:
                     if warnings:
                         logging.warning(
                             "The column %s is kept as %s according to the fallback dictionary!",
                             col,
@@ -751,23 +753,31 @@
                     "The voltage '"
                     + str(col)
                     + "' and the needed potentials are missing in the given data frame and can not be calculated."
                 ) from err
         elif (specifier == specifiers.VOLTAGE) and (len(nodes) == 1):
             try:
                 self = self.create_potential(
-                    nodes, reference_node, voltage_sub_specifiers=sub_specifiers_in_col, debug=debug
+                    nodes,
+                    reference_node,
+                    voltage_sub_specifiers=sub_specifiers_in_col,
+                    debug=debug,
                 )
             except IOError as err:
                 raise KeyError(
                     "The potential '"
                     + str(col)
                     + "' and the needed voltages are missing in the given data frame and can not be calculated."
                 ) from err
 
+        elif (specifier == specifiers.CURRENT) and (len(nodes) == 2):
+            self[col] = (
+                self[SpecifierStr(specifier, nodes[0], sub_specifiers=sub_specifiers_to_ensure)]
+                - self[SpecifierStr(specifier, nodes[1], sub_specifiers=sub_specifiers_to_ensure)]
+            )
         elif specifier == specifiers.CURRENT_DENSITY:
             if area is None:
                 raise IOError(
                     "DMT -> DataFrame -> ensure_specifier_column: area not given, but tried to calcualte current DENSITY. Abort."
                 )
             self.loc[:, specifiers.CURRENT_DENSITY + nodes[0]] = (
                 self[specifiers.CURRENT + nodes[0]] / area
@@ -793,14 +803,22 @@
                     self = self.calc_cbe(port_1=ports[0], port_2=ports[1])
                 elif nodes[0] == "C" and nodes[1] == "E":  # CCE
                     self = self.calc_cce(port_1=ports[0], port_2=ports[1])
                 elif nodes[0] == "B" and nodes[1] == "C":  # CBC
                     self = self.calc_cbc(port_1=ports[0], port_2=ports[1])
                 elif nodes[0] == "G" and nodes[1] == "S":  # CGS
                     self = self.calc_cgs(port_1=ports[0], port_2=ports[1])
+                elif nodes[0] == "G" and nodes[1] == "D":  # CGD
+                    self = self.calc_cgd(port_1=ports[0], port_2=ports[1])
+                elif nodes[0] == "G" and nodes[1] == "G":  # CGG
+                    self = self.calc_cgg(port_1=ports[0], port_2=ports[1])
+                elif nodes[0] == "D" and nodes[1] == "B":  # CDB
+                    self = self.calc_cdb(port_1=ports[0], port_2=ports[1], port_3=ports[2])
+                elif nodes[0] == "S" and nodes[1] == "B":  # CSB
+                    self = self.calc_csb(port_1=ports[0], port_2=ports[1], port_3=ports[2])
                 else:
                     raise KeyError("The " + "".join(nodes) + " capacitance can not be calculated.")
             except IOError as err:
                 raise KeyError(
                     "The " + "".join(nodes) + " capacitance could not be calculated."
                 ) from err
 
@@ -861,22 +879,22 @@
                 self = self.calc_beta()
             except IOError as err:
                 raise KeyError(
                     "The dc current amplification beta is missing in the given data frame and can not be calculated."
                 ) from err
         elif specifier == specifiers.TRANSCONDUCTANCE:
             try:
-                self = self.calc_gm()
+                self = self.calc_gm(ports=ports)
             except IOError as err:
                 raise KeyError(
                     "The transconductance is missing in the given data frame and can not be calculated."
                 ) from err
         elif specifier == specifiers.OUTPUT_CONDUCTANCE:
             try:
-                self = self.calc_go()
+                self = self.calc_go(ports=ports)
             except IOError as err:
                 raise KeyError(
                     "The transconductance is missing in the given data frame and can not be calculated."
                 ) from err
         elif specifier in specifiers_ss_para:
             try:  # try tog et from S paras
                 self = self.convert_n_port_para(p_from="S", p_to=specifier, ports=ports)
@@ -1042,15 +1060,17 @@
         # init specifiers for the potentials
         potential = SpecifierStr(
             specifiers.VOLTAGE, nodes[0], sub_specifiers=voltage_sub_specifiers
         )
 
         try:
             reference_potential = SpecifierStr(
-                specifiers.VOLTAGE, reference_node, sub_specifiers=voltage_sub_specifiers
+                specifiers.VOLTAGE,
+                reference_node,
+                sub_specifiers=voltage_sub_specifiers,
             )
         except TypeError as err:
             raise IOError("DMT->data_frame: No or incompatible reference_node were given.") from err
 
         if reference_potential not in self.columns:  # pylint: disable=unsupported-membership-test
             potentials = self.get_all_potentials()
             # try create potential by faking different reference potential
@@ -1358,15 +1378,23 @@
             raise ValueError
 
         # set values and throw away unnecessary parameters
         self = self.set_ss_para("S", s_para_values, *ports)
         self = self.strip_ss_para()
         return self
 
-    def deembed(self, df_open, df_short, ports=None, ndevices=1, ndevices_open=1, ndevices_short=1):
+    def deembed(
+        self,
+        df_open,
+        df_short,
+        ports=None,
+        ndevices=1,
+        ndevices_open=1,
+        ndevices_short=1,
+    ):
         """Deembed the measured data in df from the measured data in df_open and df_short.
 
         This method deembeds the masured small signal parameters in df using the measured small signal parameters of one dummy open and one dummy short structure.
 
         Parameters
         ----------
         df_open     :  :class:`DMT.core.DataFrame`
@@ -1426,77 +1454,103 @@
             self = self.deembed_short(df_short_deem, ports, times=times)
         except ValueError:
             raise ValueError
         # pr.disable()
         # pr.print_stats(sort='cumtime')
         return self
 
-    def determine_mres(self, forced_current=False):
+    def determine_mres(self, forced_current=False, ac_ports=None, reference_node="E") -> Dict:
         """Determine the external restistances caused by the metallization.
 
         Parameters
         ----------
         forced_current : bool, optional
 
 
         Returns
         -------
         dict
             A dict of resistances Rb,m, Rc,m, and Re,m.
 
         """
+        if ac_ports is None:
+            ac_ports = ["B", "C"]
+
+        sp_in0 = specifiers.CURRENT + ac_ports[0]
+        sp_vn0 = specifiers.VOLTAGE + ac_ports[0]
+        sp_in1 = specifiers.CURRENT + ac_ports[1]
+        sp_vn1 = specifiers.VOLTAGE + ac_ports[1]
+        sp_inr = specifiers.CURRENT + reference_node
+        sp_vnr = specifiers.VOLTAGE + reference_node
 
         if forced_current:
             try:
-                df_RC = self.loc[np.isclose(self[specifiers.CURRENT + "B"], 0.0, atol=1e-6)]
-                df_RB = self.loc[np.isclose(self[specifiers.CURRENT + "C"], 0.0, atol=1e-6)]
+                df_RC = self.loc[np.isclose(self[sp_in0], 0.0, atol=1e-6)]
+                df_RB = self.loc[np.isclose(self[sp_in1], 0.0, atol=1e-6)]
             except KeyError:
                 raise IOError
 
             mres = {}
 
-            re2 = np.polyfit(df_RB["I_B"], df_RB["V_C"], 1)[0]
-            re1 = np.polyfit(df_RC["I_C"], df_RC["V_B"], 1)[0]
+            re2 = np.polyfit(df_RB[sp_in0], df_RB[sp_vn1], 1)[0]
+            re1 = np.polyfit(df_RC[sp_in1], df_RC[sp_vn0], 1)[0]
 
             re = (re1 + re2) / 2
             de = np.abs(re1 - re2)
 
             print(
                 f"rem disagreement is {de} Ohm. Using average {re} Ohm with uncertantiy {de / (200 * re)}%"
             )
 
-            rc = np.polyfit(df_RC["I_C"], df_RC["V_C"], 1)[0] - re
-            rb = np.polyfit(df_RB["I_B"], df_RB["V_B"], 1)[0] - re
+            rc = np.polyfit(df_RC[sp_in1], df_RC[sp_vn1], 1)[0] - re
+            rb = np.polyfit(df_RB[sp_in0], df_RB[sp_vn0], 1)[0] - re
 
-            return {"R_CM": rc, "R_BM": rb, "R_EM": re}
+            return {f"R_{ac_ports[0]}M": rb, f"R_{ac_ports[1]}M": rc, f"R_{reference_node}M": re}
         else:
             try:
                 df_RCE_RBE = self.loc[
                     np.isclose(
-                        self[specifiers.VOLTAGE + "C"], self[specifiers.VOLTAGE + "E"], atol=1e-4
+                        self[sp_vn1],
+                        self[sp_vnr],
+                        atol=1e-4,
                     )
                 ]
                 df_RBC = self.loc[
                     np.isclose(
-                        self[specifiers.VOLTAGE + "B"], self[specifiers.VOLTAGE + "E"], atol=1e-4
+                        self[sp_vn0],
+                        self[sp_vnr],
+                        atol=1e-4,
                     )
                 ]
             except KeyError:
                 raise IOError
 
             mres = {}
 
-            mres = DataFrame.processor.calc_RBC_RBE(mres, df_RCE_RBE)
-            mres = DataFrame.processor.calc_RCE(mres, df_RBC)
+            mres = DataFrame.processor.calc_RBC_RBE(
+                mres, df_RCE_RBE, ac_ports=ac_ports, reference_node=reference_node
+            )
+            mres = DataFrame.processor.calc_RCE(
+                mres, df_RBC, ac_ports=ac_ports, reference_node=reference_node
+            )
 
-            mres = DataFrame.processor.convert_mres(mres)
+            mres = DataFrame.processor.convert_mres(
+                mres, ac_ports=ac_ports, reference_node=reference_node
+            )
 
             return mres
 
-    def deembed_DC(self, mres=None, df_short_dc=None, forced_current=False):
+    def deembed_DC(
+        self,
+        mres: Dict = None,
+        df_short_dc=None,
+        forced_current=False,
+        ac_ports=None,
+        reference_node="E",
+    ):
         """Deembed the measured DC data in df from external metallization resistances.
 
         Determine the metallization resistances and substract their impact from the measured voltages.
 
         Parameters
         ----------
         mres : dict
@@ -1507,17 +1561,21 @@
         -------
         :class:`DMT.core.DataFrame`
             DataFrame containing the de-embedded DC-voltages.
 
         """
 
         if mres is None:
-            mres = df_short_dc.determine_mres(forced_current=forced_current)
+            mres = df_short_dc.determine_mres(
+                forced_current=forced_current, ac_ports=ac_ports, reference_node=reference_node
+            )
 
-        return DataFrame.processor.deembed_mres(self, mres)
+        return DataFrame.processor.deembed_mres(
+            self, mres, ac_ports=ac_ports, reference_node=reference_node
+        )
 
     def check_ss_cols(self, para):
         """Check the existence of the small signal parameters para cols.
 
         Parameters
         ----------
         para : string
@@ -1922,14 +1980,91 @@
             raise NotImplementedError(
                 "DMT -> DataFrame -> calc_cgs: transistor configuration not implemented."
             )
 
         pd.options.mode.chained_assignment = "warn"
         return self
 
+    def calc_cgg(self, port_1="G", port_2="D"):
+        """Calculates the total gate capacitance CGG assuming PI equivalent circuit and common source configuration.
+
+        Returns
+        -------
+        :class:`DMT.core.DataFrame`
+            Dataframe that contains CBE.
+        """
+        # get values
+        s_para_values = self.get_ss_para("Y", port_1, port_2)
+
+        sp_cgg = specifiers.CAPACITANCE + ["G", "G"]
+
+        # put values in col of self
+        pd.options.mode.chained_assignment = (
+            None  # default='warn' , Markus: This should not warn here.
+        )
+        if port_1 == "G" and port_2 == "D":
+            self[sp_cgg] = self.processor.calc_cap_total_port_1(self["FREQ"], s_para_values, "Y")
+        else:
+            raise NotImplementedError(
+                "DMT -> DataFrame -> calc_cgg: transistor configuration not implemented."
+            )
+
+        pd.options.mode.chained_assignment = "warn"
+        return self
+
+    def calc_cdb(self, port_1="G", port_2="D", port_3="B"):
+        """Calculates the drain-bulk capacitance CDB assuming PI equivalent circuit and common source configuration.
+
+        Returns
+        -------
+        :class:`DMT.core.DataFrame`
+            Dataframe that contains CDB.
+        """
+        # get values
+
+        sp_cdb = specifiers.CAPACITANCE + ["D", "B"]
+
+        # put values in col of self
+        pd.options.mode.chained_assignment = None
+        if port_1 == "G" and port_2 == "D" and port_3 == "B":
+            s_para_values = self.get_ss_para("Y", port_2, port_3)
+            self[sp_cdb] = self.processor.calc_cap_series_thru(self["FREQ"], s_para_values, "Y")
+        else:
+            raise NotImplementedError(
+                "DMT -> DataFrame -> calc_cgs: transistor configuration not implemented."
+            )
+
+        pd.options.mode.chained_assignment = "warn"
+        return self
+
+    def calc_csb(self, port_1="G", port_2="D", port_3="B"):
+        """Calculates the source-bulk capacitance CDB assuming PI equivalent circuit and common source configuration.
+
+        Returns
+        -------
+        :class:`DMT.core.DataFrame`
+            Dataframe that contains CDB.
+        """
+        # get values
+
+        sp_csb = specifiers.CAPACITANCE + ["S", "B"]
+
+        # put values in col of self
+        pd.options.mode.chained_assignment = None
+        if port_1 == "G" and port_2 == "D" and port_3 == "B":
+            s_para_values = self.get_ss_para("Y", port_2, port_3)
+            self[sp_csb] = self.processor.calc_cap_shunt_port_2(self["FREQ"], s_para_values, "Y")
+        else:
+            raise NotImplementedError(
+                "DMT -> DataFrame -> calc_cgs: transistor configuration not implemented."
+            )
+
+        pd.options.mode.chained_assignment = "warn"
+        return self
+
     def calc_cbe(self, port_1="B", port_2="C"):
         """Calculates the base-emitter junction capacitance CBE assuming PI equivalent circuit and common emitter configuration.
 
         Returns
         -------
         :class:`DMT.core.DataFrame`
             Dataframe that contains CBE.
@@ -1988,14 +2123,36 @@
             raise NotImplementedError(
                 "DMT -> DataFrame -> calc_cce: transistor configuration not implemented."
             )
 
         pd.options.mode.chained_assignment = "warn"
         return self
 
+    def calc_cgd(self, port_1="G", port_2="D"):
+        """Calculates the gate-drain capacitance CGD.
+
+        Returns
+        -------
+        :class:`DMT.core.DataFrame`
+            Dataframe that contains CGD.
+        """
+        # get values
+        s_para_values = self.get_ss_para("Y", port_1, port_2)
+
+        sp_cgd = specifiers.CAPACITANCE + ["G", "D"]
+
+        # put values in col of self
+        if port_1 == "G" and port_2 == "D":
+            self[sp_cgd] = self.processor.calc_cap_series_thru(self["FREQ"], s_para_values, "Y")
+        else:
+            raise NotImplementedError(
+                "DMT -> DataFrame -> calc_cbe: transistor configuration not implemented."
+            )
+        return self
+
     def calc_cbc(self, port_1="B", port_2="C"):
         """Calculates the base-collector junction capacitance CBC.
 
         Returns
         -------
         :class:`DMT.core.DataFrame`
             Dataframe that contains CBE.
@@ -2036,61 +2193,82 @@
         col_ic = specifiers.CURRENT + "C"
         col_ib = specifiers.CURRENT + "B"
         self[specifiers.DC_CURRENT_AMPLIFICATION] = self.processor.calc_beta(
             self[col_ic], self[col_ib]
         )
         return self
 
-    def calc_gm(self):
+    def calc_gm(self, ports=["B", "C", "E"]):
         """Calculates the DC transconductance of a BJT.
 
+        Parameters
+        ----------
+        ports : [str], None
+            If None, BJT contact ports are assumed. Else it is assumed that ports[2] is the
+            grounded contact, ports[0] is the input port (gate/base) and ports[1] is the output port.
+
         Returns
         -------
         :class:`DMT.core.DataFrame`
             Dataframe that contains the TRANSCONDUCTANCE
         """
-        col_ic = specifiers.CURRENT + "C"
-        col_vc_forced = specifiers.VOLTAGE + "C" + sub_specifiers.FORCED
-        col_vb_forced = specifiers.VOLTAGE + "B" + sub_specifiers.FORCED
-        col_vbe = specifiers.VOLTAGE + ["B", "E"]
+        if ports is None:
+            ports = ["B", "C", "E"]
+        elif len(ports) == 2 and ports[0] == "B" and ports[1] == "C":
+            ports = ["B", "C", "E"]
+
+        col_i = specifiers.CURRENT + ports[1]
+        col_vc_forced = specifiers.VOLTAGE + ports[1] + sub_specifiers.FORCED
+        col_vb_forced = specifiers.VOLTAGE + ports[0] + sub_specifiers.FORCED
+        col_vbe = specifiers.VOLTAGE + [ports[0], ports[2]]
 
         # get voltages
         self.ensure_specifier_column(col_vbe)
-        self.ensure_specifier_column(col_ic)
+        self.ensure_specifier_column(col_i)
 
         # if possible also pass vbc forced
         try:
             self.ensure_specifier_column(col_vc_forced)
             self.ensure_specifier_column(col_vb_forced)
             try:
                 self.loc[:, specifiers.TRANSCONDUCTANCE] = self.processor.calc_gm(
-                    self[col_ic].to_numpy(),
+                    self[col_i].to_numpy(),
                     self[col_vbe].to_numpy(),
                     vc_forced=self[col_vc_forced].to_numpy(),
                     vb_forced=self[col_vb_forced].to_numpy(),
                 )
             except ValueError:
                 pass
         except KeyError:
             self.loc[:, specifiers.TRANSCONDUCTANCE] = self.processor.calc_gm(
-                self[col_ic].to_numpy(), self[col_vbe].to_numpy()
+                self[col_i].to_numpy(), self[col_vbe].to_numpy()
             )
 
         return self
 
-    def calc_go(self):
-        """Calculates the DC output condutance of a BJT.
+    def calc_go(self, ports=["B", "C", "E"]):
+        """Calculates the DC output condutance of a BJT or generic transistor in common emitter/source configuration.
+
+        Parameters
+        ----------
+        ports : [str], None
+            If None, BJT contact ports are assumed. Else it is assumed that ports[2] is the
+            grounded contact, ports[0] is the input port (gate/base) and ports[1] is the output port.
 
         Returns
         -------
         :class:`DMT.core.DataFrame`
             Dataframe that contains the TRANSCONDUCTANCE
         """
-        col_ic = specifiers.CURRENT + "C"
-        col_vce_forced = specifiers.VOLTAGE + "C" + "E" + sub_specifiers.FORCED
+        if ports == None:  # assume HBT
+            col_ic = specifiers.CURRENT + "C"
+            col_vce_forced = specifiers.VOLTAGE + ["C", "E"] + sub_specifiers.FORCED
+        else:
+            col_ic = specifiers.CURRENT + ports[1]
+            col_vce_forced = specifiers.VOLTAGE + [ports[1], ports[2]] + sub_specifiers.FORCED
 
         # get voltages
         self.ensure_specifier_column(col_vce_forced)
         self.ensure_specifier_column(col_ic)
 
         self.loc[:, specifiers.OUTPUT_CONDUCTANCE] = self.processor.calc_go(
             self[col_ic].to_numpy(), self[col_vce_forced].to_numpy()
@@ -2188,15 +2366,17 @@
                 y_para_re = specifiers_ss_para.SS_PARA_Y + [port1, port2] + sub_specifiers.REAL
                 y_para_im = specifiers_ss_para.SS_PARA_Y + [port1, port2] + sub_specifiers.IMAG
                 df_new[y_para] = df_new[y_para_re] + 1j * df_new[y_para_im]
                 df_new.drop(columns=[y_para_im, y_para_re])
 
         return df_new
 
-    def iter_unique_col(self, column, decimals=5):
+    def iter_unique_col(
+        self, column: SpecifierStr, decimals: int = 5
+    ) -> Iterator[Tuple[int, complex, "DataFrame"]]:
         """Allows iteration over the unique values and their slices of a column
 
         Parameters
         ----------
         column : :class:`DMT.core.SpecifierStr` or str
             Column name to iterate over
         decimals : int, optional
@@ -2231,16 +2411,22 @@
             val_unique = np.unique(self[column])
             atol = None
         else:
             val_unique = np.unique(np.round(self[column], decimals=decimals))
             atol = 5 * np.float_power(10, -(decimals + 1))
 
         while index < len(val_unique):
-            val = val_unique[index]
+            val: complex = val_unique[index]
 
             if atol is None:
                 dataframe = self[self[column] == val]
             else:
                 dataframe = self[np.isclose(self[column], val, atol=atol)]
 
             yield index, val, dataframe
             index += 1
+
+
+def df_concat(*frames):
+    frame = pd.concat(frames, axis=0, ignore_index=True)
+    frame.__class__ == DataFrame
+    return frame
```

### Comparing `DMT_core-2.0.0/DMT/core/data_processor.py` & `DMT_core-2.1.0/DMT/core/data_processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """ data processor module
 
 """
+
 # DMT_core
 # Copyright (C) from 2022  SemiMod
 # Copyright (C) until 2021  Markus Müller, Mario Krattenmacher and Pascal Kuthe
 # <https://gitlab.com/dmt-development/dmt-core>
 #
 # This file is part of DMT_core.
 #
@@ -18,15 +19,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>
 import numpy as np
 from skrf import network as rf_network
-from DMT.core import specifiers, set_col_name, sub_specifiers
+from DMT.core.naming import specifiers, sub_specifiers
 
 
 def is_iterable(arg):
     """Returns True if the object is iterable
 
     Source: https://stackoverflow.com/a/36407550/13212532
 
@@ -407,149 +408,142 @@
             s_para_values, "S", "Y"
         )  # (n_freq, n_port, n_port)
         # normalize Y para
         y_para_values = y_para_values / ndevices
 
         return self.convert_n_port_para(y_para_values, "Y", "S")
 
-    def calc_RBC_RBE(self, mres, df_RM):
+    def calc_RBC_RBE(self, mres, df_RM, ac_ports=None, reference_node="E"):
         """Calculate the metallization resistances R_CE and R_BE.
 
         Parameters
         ----------
         df_RM   : df
             Containing all values for the incoming df, where V_CE=0V.
 
         Returns
         -------
         mres    : [list]
             List containing the calculated resistance values
         """
+        if ac_ports is None:
+            ac_ports = ["B", "C"]
+
+        sp_in0 = specifiers.CURRENT + ac_ports[0]
+        sp_vn0 = specifiers.VOLTAGE + ac_ports[0]
+        sp_in1 = specifiers.CURRENT + ac_ports[1]
 
         df_RM_clean = df_RM.dropna(axis=0, how="any")
 
-        R_BCM = np.polyfit(np.negative(df_RM_clean["I_C"]), df_RM_clean["V_B"], 1)
+        r_BCM = np.polyfit(np.negative(df_RM_clean[sp_in1]), df_RM_clean[sp_vn0], 1)
 
-        ic_2 = df_RM_clean["I_B"] + df_RM_clean["I_C"]
-        R_BEM = np.polyfit(ic_2, df_RM_clean["V_B"], 1)
+        ic_2 = df_RM_clean[sp_in0] + df_RM_clean[sp_in1]
+        r_BEM = np.polyfit(ic_2, df_RM_clean[sp_vn0], 1)
 
-        mres["R_BCM"] = R_BCM[0]
-        mres["R_BEM"] = R_BEM[0]
+        mres[f"R_{ac_ports[0]}{ac_ports[1]}M"] = r_BCM[0]
+        mres[f"R_{ac_ports[0]}{reference_node}M"] = r_BEM[0]
         return mres
 
-    def calc_RCE(self, mres, df_RM):
+    def calc_RCE(self, mres, df_RM, ac_ports=None, reference_node="E"):
         """Calculate the metallization resistances R_BC.
 
         Parameters
         ----------
         df_RM   : df
             Containing all values for the incoming df, where V_BE=0V.
 
         Returns
         -------
         mres    : {dict}
             List containing the calculated resistance values
         """
+        if ac_ports is None:
+            ac_ports = ["B", "C"]
+        sp_in0 = specifiers.CURRENT + ac_ports[0]
+        sp_in1 = specifiers.CURRENT + ac_ports[1]
+        sp_vn1 = specifiers.VOLTAGE + ac_ports[1]
+
         df_RM_clean = df_RM.dropna(axis=0, how="any")
 
-        R_CEM = np.polyfit((df_RM_clean["I_B"] + df_RM_clean["I_C"]), df_RM_clean["V_C"], 1)
+        R_CEM = np.polyfit((df_RM_clean[sp_in0] + df_RM_clean[sp_in1]), df_RM_clean[sp_vn1], 1)
 
-        mres["R_CEM"] = R_CEM[0]
+        mres[f"R_{ac_ports[1]}{reference_node}M"] = R_CEM[0]
 
         return mres
 
-    def convert_mres(self, mres):
+    def convert_mres(self, mres, ac_ports=None, reference_node="E"):
         """Converts the calculated resistance network from delta- to wye-form.
 
         Parameters
         ----------
         mres    : {dict}
             List containing the calculated delta-form resistances
         Returns
         -------
         mres    : {dict}
             Same list with appended wye-form parameters.
         """
-        R_sum = mres["R_BCM"] + mres["R_CEM"] + mres["R_BEM"]
-
-        R_BM = (mres["R_BEM"] * mres["R_BCM"]) / R_sum
-        R_CM = (mres["R_BCM"] * mres["R_CEM"]) / R_sum
-        R_EM = (mres["R_BEM"] * mres["R_CEM"]) / R_sum
-
-        mres["R_BM"] = R_BM
-        mres["R_CM"] = R_CM
-        mres["R_EM"] = R_EM
+        k_rbcm = f"R_{ac_ports[0]}{ac_ports[1]}M"
+        k_rbem = f"R_{ac_ports[0]}{reference_node}M"
+        k_rcem = f"R_{ac_ports[1]}{reference_node}M"
+        k_rbm = f"R_{ac_ports[0]}M"
+        k_rcm = f"R_{ac_ports[1]}M"
+        k_rem = f"R_{reference_node}M"
+
+        r_sum = mres[k_rbcm] + mres[k_rcem] + mres[k_rbem]
+
+        r_BM = (mres[k_rbem] * mres[k_rbcm]) / r_sum
+        r_CM = (mres[k_rbcm] * mres[k_rcem]) / r_sum
+        r_EM = (mres[k_rbem] * mres[k_rcem]) / r_sum
+
+        mres[k_rbm] = r_BM
+        mres[k_rcm] = r_CM
+        mres[k_rem] = r_EM
 
         return mres
 
-    def deembed_mres(self, df, mres):
+    def deembed_mres(self, df, mres, ac_ports=None, reference_node="E"):
         """Substract external voltage drop over metal resistances from measured voltages.
 
         Parameters
         ----------
         df      : DMT.dataframe
             df contains DC measurements that are to be deembedded.
         mres    : {'R_BM':float64, 'R_CM':float64, 'R_EM'_float64}
             List of calculated resistances R_CM, R_BM, and R_EM.
         """
-        col_vb, col_ib, col_vc, col_ic, col_ve = None, None, None, None, None
-        try:
-            col_vb = df.get_col_name(specifiers.VOLTAGE, "B")
-            col_vb_force = set_col_name(
-                specifiers.VOLTAGE, "B", sub_specifiers=sub_specifiers.FORCED
-            )
-            df[col_vb_force] = df[col_vb].to_numpy()
-        except KeyError:
-            pass
-        try:
-            col_vc = df.get_col_name(specifiers.VOLTAGE, "C")
-            col_vc_force = set_col_name(
-                specifiers.VOLTAGE, "C", sub_specifiers=sub_specifiers.FORCED
-            )
-            df[col_vc_force] = df[col_vc].to_numpy()
-        except KeyError:
-            pass
-        try:
-            col_ve = df.get_col_name(specifiers.VOLTAGE, "E")
-            col_ve_force = set_col_name(
-                specifiers.VOLTAGE, "E", sub_specifiers=sub_specifiers.FORCED
-            )
-            df[col_ve_force] = df[col_ve].to_numpy()
-        except KeyError:
-            pass
+        if ac_ports is None:
+            ac_ports = ["B", "C"]
+
+        for node in ac_ports:
+            try:
+                sp_vn = df.get_col_name(specifiers.VOLTAGE, node)
+                sp_vn_force = specifiers.VOLTAGE + node + sub_specifiers.FORCED
+                df[sp_vn_force] = df[sp_vn].to_numpy()
+                sp_in = df.get_col_name(specifiers.CURRENT, node)
+                i_n = df[sp_in].to_numpy()
+                df[sp_vn] = df[sp_vn_force] - i_n * mres[f"R_{node}M"]
+            except KeyError:
+                pass
+
+        sp_vn_force = specifiers.VOLTAGE + reference_node + sub_specifiers.FORCED
         try:
-            col_ic = df.get_col_name(specifiers.CURRENT, "C")
+            sp_vn = df.get_col_name(specifiers.VOLTAGE, reference_node)
+            df[sp_vn_force] = df[sp_vn].to_numpy()
         except KeyError:
             pass
+
         try:
-            col_ib = df.get_col_name(specifiers.CURRENT, "B")
+            sp_in0 = specifiers.VOLTAGE + ac_ports[0]
+            sp_in1 = specifiers.VOLTAGE + ac_ports[1]
+            i_n = df[sp_in0].to_numpy() + df[sp_in1].to_numpy()
+            df[sp_vn] = df[sp_vn_force] + i_n * mres[f"R_{reference_node}M"]
         except KeyError:
             pass
 
-        if col_vb and col_ib:
-            vb = df[col_vb].to_numpy()
-            ib = df[col_ib].to_numpy()
-            # vb_dif      = [i * mres["R_BM"] for i in ib]
-            vb_dif = ib * mres["R_BM"]
-            df[col_vb] = vb - vb_dif
-
-        if col_vc and col_ic:
-            vc = df[col_vc].to_numpy()
-            ic = df[col_ic].to_numpy()
-            vc_dif = ic * mres["R_CM"]
-            df[col_vc] = vc - vc_dif
-
-        if col_ve and col_ib and col_ic:
-            ve = df[col_ve].to_numpy()
-            # ie = [sum(i) for i in zip(ic, ib)]
-            ie = ib + ic
-            # ve_dif      = [i * mres["R_EM"] for i in ie]
-            ve_dif = ie * mres["R_EM"]
-            df[col_ve] = ve + ve_dif
-
         return df
 
     def deembed_short(self, s_para_values, s_para_short_values, times=1):
         """Deembed the measured S parameters in s_para_values from the measured S parameters in s_para_short_values.
 
         Parameters
         ----------
@@ -750,15 +744,15 @@
 
     def calc_mag(self, freq, para_values, p_type):
         """Calculates the maximum available gain MAG.
 
         Parameters
         ----------
         freq         :  np.ndarray()
-            Frequencys that correspond to para_values.
+            Frequencies that correspond to para_values.
         para_values  :  np.ndarray()
             Small signal parameters of type p_type with shape [n_freq, n_port, n_port]
         p_type       :  string
             Type of the small signal parameters in para_values.
 
         Returns
         -------
@@ -778,15 +772,15 @@
 
     def calc_k(self, freq, para_values, p_type):
         """Calculates the k-factor.
 
         Parameters
         ----------
         freq         :  np.ndarray()
-            Frequencys that correspond to para_values.
+            Frequencies that correspond to para_values.
         para_values  :  np.ndarray()
             Small signal parameters of type p_type with shape [n_freq, n_port, n_port]
         p_type       :  string
             Type of the small signal parameters in para_values.
 
         Returns
         -------
@@ -832,15 +826,15 @@
 
     def calc_cap_shunt_port_1(self, freq, para_values, p_type):
         """Calculates the shunt capacitance at port 1 assuming a Pi equivalent circuit capacitance cbe from the small signal parameters para_values.
 
         Parameters
         ----------
         freq         :  np.ndarray()
-            Frequencys that correspond to para_values.
+            Frequencies that correspond to para_values.
         para_values  :  np.ndarray()
             Small signal parameters of type p_type with shape [n_freq, n_port, n_port]
         p_type       :  string
             Type of the small signal parameters in para_values.
 
         Returns
         -------
@@ -850,14 +844,38 @@
         y_para_values = self.convert_n_port_para(para_values, p_type, "Y")
 
         # calculate cbe from y para
         cbe = np.imag(y_para_values[:, 0, 0] + y_para_values[:, 0, 1]) / (2.0 * np.pi * freq)
 
         return cbe
 
+    def calc_cap_total_port_1(self, freq, para_values, p_type):
+        """Calculates the total capacitance at port 1 assuming a Pi equivalent circuit capacitance cgg from the small signal parameters para_values.
+
+        Parameters
+        ----------
+        freq         :  np.ndarray()
+            Frequenciess that correspond to para_values.
+        para_values  :  np.ndarray()
+            Small signal parameters of type p_type with shape [n_freq, n_port, n_port]
+        p_type       :  string
+            Type of the small signal parameters in para_values.
+
+        Returns
+        -------
+        cgg           :  np.ndarray()
+            Total capacitance at port 1.
+        """
+        y_para_values = self.convert_n_port_para(para_values, p_type, "Y")
+
+        # calculate cbe from y para
+        cgg = np.imag(y_para_values[:, 0, 0]) / (2.0 * np.pi * freq)
+
+        return cgg
+
     def calc_cap_series_thru(self, freq, para_values, p_type):
         """Calculates the the series-thru junction capacitance cbc from the small signal parameters para_values.
 
         Parameters
         ----------
         freq         :  np.ndarray()
             Frequencys that correspond to para_values.
```

### Comparing `DMT_core-2.0.0/DMT/core/data_reader.py` & `DMT_core-2.1.0/DMT/core/data_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 save_hdf(df, save_dir, filename)
     Save the dataframe df into save_dir as filename.h5 .
 
 save_elpa(fname, ELPA, cols, firstline)
     Save data as a elpa file.
 
 """
+
 # DMT_core
 # Copyright (C) from 2022  SemiMod
 # Copyright (C) until 2021  Markus Müller, Mario Krattenmacher and Pascal Kuthe
 # <https://gitlab.com/dmt-development/dmt-core>
 #
 # This file is part of DMT_core.
 #
@@ -60,15 +61,15 @@
 import pandas as pd
 import warnings
 import numpy as np
 import re
 import _pickle as pickle
 import struct
 from pathlib import Path
-from DMT.core import DataFrame
+from DMT.core.data_frame import DataFrame
 
 
 def read_data(filename, key=None, **kwargs):
     """General data reading routine.
 
     Used to read in data of an arbitrary file format. Correct reading routine is selected based on file extension.
```

### Comparing `DMT_core-2.0.0/DMT/core/database_manager.py` & `DMT_core-2.1.0/DMT/core/database_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 Features:
 
 * Can read all relevant file formats produced by simulators used at CEDIC.
 * Uses pandas to manage the data internally.
 * Allows to "search" and "filter" existing data.
 
 """
+
 # DMT_core
 # Copyright (C) from 2022  SemiMod
 # Copyright (C) until 2021  Markus Müller, Mario Krattenmacher and Pascal Kuthe
 # <https://gitlab.com/dmt-development/dmt-core>
 #
 # This file is part of DMT_core.
 #
```

### Comparing `DMT_core-2.0.0/DMT/core/df_to_sweep.py` & `DMT_core-2.1.0/DMT/core/df_to_sweep.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """ Converter routine to create a sweep definition from a given DataFrame
 """
+
 # DMT_core
 # Copyright (C) from 2022  SemiMod
 # Copyright (C) until 2021  Markus Müller, Mario Krattenmacher and Pascal Kuthe
 # <https://gitlab.com/dmt-development/dmt-core>
 #
 # This file is part of DMT_core.
 #
```

### Comparing `DMT_core-2.0.0/DMT/core/docu_dut_lib.py` & `DMT_core-2.1.0/DMT/core/docu_dut_lib.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """ Automatic documentation for DutLib
 """
+
 # Copyright (C) from 2022  SemiMod
 # <https://gitlab.com/dmt-development/dmt-core>
 #
 # This file is part of DMT.
 #
 # DMT is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
@@ -15,266 +16,297 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>
 import copy
 import datetime
+import numpy as np
 from pathlib import Path
 from typing import Dict, List, Mapping, Sequence, Optional, Union
-import numpy as np
+from joblib import Parallel, delayed
 from scipy import interpolate
 from DMT.config import COMMAND_TEX, DATA_CONFIG
-from DMT.core import DutType, DutLib, specifiers, sub_specifiers, specifiers_ss_para
+from DMT.core import (
+    DutType,
+    DutLib,
+    specifiers,
+    sub_specifiers,
+    MCard,
+    DutCircuit,
+    DutMeas,
+    Sweep,
+    SimCon,
+)
 from DMT.core.plot import MIX, PLOT_STYLES, natural_scales, Plot
 from DMT.external.os import recursive_copy, rmtree
 
 try:
-    from pylatex import Section, Subsection, SmallText, Tabular, NoEscape, Center, Figure
+    from pylatex import (
+        Section,
+        Subsection,
+        Subsubsection,
+        SmallText,
+        Tabular,
+        NoEscape,
+        Center,
+        Figure,
+    )
     from pylatex.base_classes import Arguments
     from DMT.external.pylatex import SubFile, Tex, CommandInput, CommandLabel
 except ImportError:
     pass
 
 # defaults for autodoc feature plots
 PLOT_DEFAULTS = {
     DutType.npn: {
         "gummel_vbc": {
             "x_log": False,
             "y_log": True,
-            "at": specifiers.VOLTAGE + "B" + "C" + sub_specifiers.FORCED,
-            "quantity_x": specifiers.VOLTAGE + "B" + "E",
+            "at": specifiers.VOLTAGE + ["B", "C"] + sub_specifiers.FORCED,
+            "quantity_x": specifiers.VOLTAGE + ["B", "E"],
             "quantity_y": specifiers.CURRENT_DENSITY + "C",
             "legend_location": "upper left",
             "y_limits": (None, None),
             "x_limits": (None, None),
-            "tex": r"Gummel @ $V_{\mathrm{BC}}$.",
+            "caption": r"Gummel @ $V_{\mathrm{BC}}$.",
         },
         "gummel_vbc_mark_ft": {
             "x_log": False,
             "y_log": True,
-            "at": specifiers.VOLTAGE + "B" + "C" + sub_specifiers.FORCED,
-            "quantity_x": specifiers.VOLTAGE + "B" + "E",
+            "at": specifiers.VOLTAGE + ["B", "C"] + sub_specifiers.FORCED,
+            "quantity_x": specifiers.VOLTAGE + ["B", "E"],
             "quantity_y": specifiers.CURRENT_DENSITY + "C",
             "legend_location": "upper left",
             "y_limits": (None, None),
             "x_limits": (None, None),
-            "tex": r"Gummel @ $V_{\mathrm{BC}}$.",
+            "caption": r"Gummel @ $V_{\mathrm{BC}}$.",
         },
         "output_vbe": {
             "x_log": False,
             "y_log": False,
             "at": specifiers.VOLTAGE + "B" + "E" + sub_specifiers.FORCED,
             "quantity_x": specifiers.VOLTAGE + "C" + "E",
             "quantity_y": specifiers.CURRENT_DENSITY + "C",
             "legend_location": "upper left",
             "y_limits": (None, None),
             "x_limits": (None, None),
-            "tex": r"Output @ $V_{\mathrm{BE}}$.",
+            "caption": r"Output @ $V_{\mathrm{BE}}$.",
         },
         "output_ib": {
             "x_log": False,
             "y_log": False,
             "at": specifiers.CURRENT_DENSITY + "B",
             "quantity_x": specifiers.VOLTAGE + "C" + "E",
             "quantity_y": specifiers.CURRENT_DENSITY + "C",
             "legend_location": "upper left",
             "y_limits": (None, None),
             "x_limits": (None, None),
-            "tex": r"Output @ $I_{\mathrm{B}}$.",
+            "caption": r"Output @ $I_{\mathrm{B}}$.",
         },
         "ft_jc_vbc": {
             "x_log": True,
             "y_log": False,
-            "at": specifiers.VOLTAGE + "B" + "C" + sub_specifiers.FORCED,
+            "at": specifiers.VOLTAGE + ["B", "C"] + sub_specifiers.FORCED,
             "quantity_x": specifiers.CURRENT_DENSITY + "C",
             "quantity_y": specifiers.TRANSIT_FREQUENCY,
             "legend_location": "upper left",
             "y_limits": (0, None),
             "x_limits": (None, None),
-            "tex": r"$f_{\mathrm{T}} \left( J_{\mathrm{C}} \right) $ @ $V_{\mathrm{BC}}$.",
+            "caption": r"$f_{\mathrm{T}} \left( J_{\mathrm{C}} \right) $ @ $V_{\mathrm{BC}}$.",
         },
         "fmax_jc_vbc": {
             "x_log": True,
             "y_log": False,
             "at": specifiers.VOLTAGE + "B" + "C" + sub_specifiers.FORCED,
             "quantity_x": specifiers.CURRENT_DENSITY + "C",
             "quantity_y": specifiers.MAXIMUM_OSCILLATION_FREQUENCY,
             "legend_location": "upper left",
             "y_limits": (0, None),
             "x_limits": (None, None),
-            "tex": r"$f_{\mathrm{max}} \left( J_{\mathrm{C}} \right) $ @ $V_{\mathrm{BC}}$.",
+            "caption": r"$f_{\mathrm{max}} \left( J_{\mathrm{C}} \right) $ @ $V_{\mathrm{BC}}$.",
         },
         "ft_jc_vce": {
             "x_log": True,
             "y_log": False,
             "at": specifiers.VOLTAGE + "C" + "E" + sub_specifiers.FORCED,
             "quantity_x": specifiers.CURRENT_DENSITY + "C",
             "quantity_y": specifiers.TRANSIT_FREQUENCY,
             "legend_location": "upper left",
             "y_limits": (0, None),
             "x_limits": (None, None),
-            "tex": r"$F_{\mathrm{T}} \left( J_{\mathrm{C}} \right) $ @ $V_{\mathrm{CE}}$.",
+            "caption": r"$F_{\mathrm{T}} \left( J_{\mathrm{C}} \right) $ @ $V_{\mathrm{CE}}$.",
         },
         "fmax_jc_vce": {
             "x_log": True,
             "y_log": False,
             "at": specifiers.VOLTAGE + "C" + "E" + sub_specifiers.FORCED,
             "quantity_x": specifiers.CURRENT_DENSITY + "C",
             "quantity_y": specifiers.MAXIMUM_OSCILLATION_FREQUENCY,
             "legend_location": "upper left",
             "y_limits": (0, None),
             "x_limits": (None, None),
-            "tex": r"$f_{\mathrm{max}} \left( J_{\mathrm{C}} \right) $ @ $V_{\mathrm{CE}}$.",
+            "caption": r"$f_{\mathrm{max}} \left( J_{\mathrm{C}} \right) $ @ $V_{\mathrm{CE}}$.",
         },
         "beta_jc_vbc": {
             "x_log": True,
             "y_log": False,
             "at": specifiers.VOLTAGE + "B" + "C" + sub_specifiers.FORCED,
             "quantity_x": specifiers.CURRENT_DENSITY + "C",
             "quantity_y": specifiers.DC_CURRENT_AMPLIFICATION,
             "legend_location": "upper left",
             "y_limits": (None, None),
             "x_limits": (None, None),
-            "tex": r"$\beta_{\mathrm{DC}} \left( J_{\mathrm{C}} \right)$ @ $V_{\mathrm{BC}}$.",
+            "caption": r"$\beta_{\mathrm{DC}} \left( J_{\mathrm{C}} \right)$ @ $V_{\mathrm{BC}}$.",
         },
         "rey21_f_vbe_vbc": {
             "x_log": True,
             "y_log": False,
             "at": [
                 specifiers.VOLTAGE + "B" + "E" + sub_specifiers.FORCED,
                 specifiers.VOLTAGE + "B" + "C" + sub_specifiers.FORCED,
             ],
             "quantity_x": specifiers.FREQUENCY,
             "quantity_y": specifiers.SS_PARA_Y + "C" + "B" + sub_specifiers.REAL,
             "legend_location": "upper left",
             "y_limits": (None, None),
             "x_limits": (None, None),
-            "tex": r"$\Re \left\{ Y_{21} \right\} \left( f \right)$ @ $V_{\mathrm{BC}} @ V_{\mathrm{BE}}$.",
+            "caption": r"$\Re \left\{ Y_{21} \right\} \left( f \right)$ @ $V_{\mathrm{BC}} @ V_{\mathrm{BE}}$.",
         },
         "imy11_f_vbe_vbc": {
             "x_log": True,
             "y_log": True,
             "at": [
                 specifiers.VOLTAGE + "B" + "E" + sub_specifiers.FORCED,
                 specifiers.VOLTAGE + "B" + "C" + sub_specifiers.FORCED,
             ],
             "quantity_x": specifiers.FREQUENCY,
             "quantity_y": specifiers.SS_PARA_Y + "B" + "B" + sub_specifiers.IMAG,
             "legend_location": "upper left",
             "y_limits": (None, None),
             "x_limits": (None, None),
-            "tex": r"$\Im \left\{ Y_{11} \right\} \left( f \right)$ @ $V_{\mathrm{BC}} @ V_{\mathrm{BE}}$.",
+            "caption": r"$\Im \left\{ Y_{11} \right\} \left( f \right)$ @ $V_{\mathrm{BC}} @ V_{\mathrm{BE}}$.",
         },
         "y21_jc_vbc": {
             "x_log": True,
             "y_log": True,
             "at": [
                 specifiers.FREQUENCY,
                 specifiers.VOLTAGE + "B" + "C" + sub_specifiers.FORCED,
             ],
             "quantity_x": specifiers.CURRENT_DENSITY + "C",
             "quantity_y": specifiers.SS_PARA_Y + "C" + "B" + sub_specifiers.REAL,
             "legend_location": "upper left",
             "y_limits": (None, None),
             "x_limits": (None, None),
-            "tex": r"$\Re \left\{ Y_{21} \right\} \left( J_{\mathrm{C}} \right)$ @ $V_{\mathrm{BC}}$.",
+            "caption": r"$\Re \left\{ Y_{21} \right\} \left( J_{\mathrm{C}} \right)$ @ $V_{\mathrm{BC}}$.",
         },
         "y21_jc_vbc_mark_ft": {
             "x_log": True,
             "y_log": True,
             "at": [
                 specifiers.FREQUENCY,
                 specifiers.VOLTAGE + "B" + "C" + sub_specifiers.FORCED,
             ],
             "quantity_x": specifiers.CURRENT_DENSITY + "C",
             "quantity_y": specifiers.SS_PARA_Y + "C" + "B" + sub_specifiers.REAL,
             "legend_location": "upper left",
             "y_limits": (None, None),
             "x_limits": (None, None),
-            "tex": r"$\Re \left\{ Y_{21} \right\} \left( J_{\mathrm{C}} \right)$ @ $V_{\mathrm{BC}}$.",
+            "caption": r"$\Re \left\{ Y_{21} \right\} \left( J_{\mathrm{C}} \right)$ @ $V_{\mathrm{BC}}$.",
         },
         "y21_jc_vbc_mark_ft": {
             "x_log": True,
             "y_log": True,
             "at": [
                 specifiers.FREQUENCY,
                 specifiers.VOLTAGE + "B" + "C" + sub_specifiers.FORCED,
             ],
             "quantity_x": specifiers.CURRENT_DENSITY + "C",
             "quantity_y": specifiers.SS_PARA_Y + "C" + "B" + sub_specifiers.REAL,
             "legend_location": "upper left",
             "y_limits": (None, None),
             "x_limits": (None, None),
-            "tex": r"$\Re \left\{ Y_{21} \right\} \left( J_{\mathrm{C}} \right)$ @ $V_{\mathrm{BC}}$.",
+            "caption": r"$\Re \left\{ Y_{21} \right\} \left( J_{\mathrm{C}} \right)$ @ $V_{\mathrm{BC}}$.",
         },
         "tj_jc_at_vbc": {
             "x_log": True,
             "y_log": False,
             "at": specifiers.VOLTAGE + "B" + "C" + sub_specifiers.FORCED,
             "quantity_x": specifiers.CURRENT_DENSITY + "C",
             "quantity_y": specifiers.TEMPERATURE,
             "legend_location": "upper left",
             "y_limits": (None, None),
             "x_limits": (None, None),
-            "tex": r"$T_{\mathrm{j}} \left( J_{\mathrm{C}} \right)$ @ $V_{\mathrm{BC}}$.",
+            "caption": r"$T_{\mathrm{j}} \left( J_{\mathrm{C}} \right)$ @ $V_{\mathrm{BC}}$.",
             "rth": 3e3,
         },
     },
     DutType.n_mos: {
         "id(vg)": {
             "x_log": False,
             "y_log": False,
             "at": [specifiers.VOLTAGE + ["D"], specifiers.VOLTAGE + ["B"]],
             "quantity_x": specifiers.VOLTAGE + ["G"],
             "quantity_y": specifiers.CURRENT + ["D"],
             "legend_location": "upper left",
             "y_limits": (None, None),
             "x_limits": (None, None),
-            "tex": r"$I_{\mathrm{D}}(V_{\mathrm{G}})@V_{\mathrm{D}}$.",
+            "caption": r"$I_{\mathrm{D}}(V_{\mathrm{G}})@V_{\mathrm{D}}$.",
         },
         "id(vd)": {
             "x_log": False,
             "y_log": False,
             "at": [specifiers.VOLTAGE + ["G"], specifiers.VOLTAGE + ["B"]],
             "quantity_x": specifiers.VOLTAGE + ["D"],
             "quantity_y": specifiers.CURRENT + ["D"],
             "legend_location": "upper left",
             "y_limits": (None, None),
             "x_limits": (None, None),
-            "tex": r"$I_{\mathrm{D}}(V_{\mathrm{D}})@V_{\mathrm{G}}$.",
+            "caption": r"$I_{\mathrm{D}}(V_{\mathrm{D}})@V_{\mathrm{G}}$.",
         },
     },
     DutType.p_mos: {
         "id(vg)": {
             "x_log": False,
             "y_log": False,
             "at": [specifiers.VOLTAGE + ["D"], specifiers.VOLTAGE + ["B"]],
             "quantity_x": specifiers.VOLTAGE + ["G"],
             "quantity_y": specifiers.CURRENT + ["D"],
             "legend_location": "upper left",
             "y_limits": (None, None),
             "x_limits": (None, None),
-            "tex": r"$I_{\mathrm{D}}(V_{\mathrm{G}})@V_{\mathrm{D}}$.",
+            "caption": r"$I_{\mathrm{D}}(V_{\mathrm{G}})@V_{\mathrm{D}}$.",
         },
         "id(vd)": {
             "x_log": False,
             "y_log": False,
             "at": [specifiers.VOLTAGE + ["G"], specifiers.VOLTAGE + ["B"]],
             "quantity_x": specifiers.VOLTAGE + ["D"],
             "quantity_y": specifiers.CURRENT + ["D"],
             "legend_location": "upper left",
             "y_limits": (None, None),
             "x_limits": (None, None),
-            "tex": r"$I_{\mathrm{D}}(V_{\mathrm{D}})@V_{\mathrm{G}}$.",
+            "caption": r"$I_{\mathrm{D}}(V_{\mathrm{D}})@V_{\mathrm{G}}$.",
         },
     },
 }
 
 
+def obtain(plot_spec, key, dut_type, plot_type, value_default=None):
+    if key in plot_spec:
+        return plot_spec[key]
+
+    if dut_type in PLOT_DEFAULTS:
+        if plot_type in PLOT_DEFAULTS[dut_type]:
+            return PLOT_DEFAULTS[dut_type][plot_type].get(key, value_default)
+
+    return value_default
+
+
 class DocuDutLib(object):
     """Documentation of an DutLib
 
     Parameters
     ----------
     dut_lib : :class:`~DMT.core.DutLib`
         Library to document
@@ -289,15 +321,21 @@
                 'width'         :0.22e-6,
             },]
     date : convertable to str
         Date of the documentation report.
     """
 
     def __init__(
-        self, dut_lib: DutLib, devices: Optional[Sequence[Mapping[str, object]]] = None, date=None
+        self,
+        dut_lib: DutLib,
+        devices: Optional[Sequence[Mapping[str, object]]] = None,
+        date: Optional[str] = None,
+        modelcard_dict: Optional[Dict[DutType, MCard]] = None,
+        DutCircuitClass: Optional[DutCircuit] = None,
+        dut_class_kwargs: Optional[Dict] = None,
     ):
         self.dut_lib = dut_lib
 
         if devices is None:
             self.duts = self.dut_lib.duts
         else:
             self.duts = []  # array of DMT Duts
@@ -315,14 +353,18 @@
                             try:
                                 if not np.isclose(dut_property, val):
                                     ok = False
                             except (
                                 ValueError
                             ):  # tetrodes will not work like this (tuple dut_property)
                                 pass
+                        else:
+                            dut_property = getattr(dut, device_spec)
+                            if val != dut_property:
+                                ok = False
 
                     if ok:
                         print("Found device " + dut.name + ".")
                         self.duts.append(dut)
 
         if not self.duts:
             raise IOError("Found 0 devices.")
@@ -330,15 +372,40 @@
         print("Search finished...\nFound " + str(len(self.duts)) + " devices for plotting.")
 
         if date is None:
             self.date = datetime.datetime.today().strftime("%Y-%m-%d")
         else:
             self.date = date
 
-        self.plts = []
+        self.plts: List[Plot] = []
+
+        self.modelcard_dict = modelcard_dict
+        self.DutCircuitClass = DutCircuitClass
+        if dut_class_kwargs is None:
+            self.dut_class_kwargs = {}
+        else:
+            self.dut_class_kwargs = dut_class_kwargs
+
+    def get_dut_sim(self, dut_meas: DutMeas) -> DutCircuit:
+        """Retrieve a circuit dut view which should be compared to the given dut_meas"""
+        if self.DutCircuitClass is not None:
+            return self.DutCircuitClass(
+                database_dir=None,
+                dut_type=dut_meas.dut_type,
+                input_circuit=self.modelcard_dict[dut_meas.dut_type],
+                technology=dut_meas.technology,  # needed for scaling!
+                width=dut_meas.width,
+                length=dut_meas.length,
+                contact_config=dut_meas.contact_config,
+                nfinger=dut_meas.nfinger,
+                reference_node=dut_meas.reference_node,
+                **self.dut_class_kwargs,
+            )
+        else:
+            return None
 
     def generate_docu(
         self,
         target_base_path: Union[str, Path],
         plot_specs: List[Dict],
         save_tikz_settings: Optional[Dict] = None,
         show: bool = False,
@@ -354,28 +421,30 @@
         save_tikz_settings : Dict
             Plot specs passed to :meth:`~DMT.core.docu_dut_lib.DocuDutLib.generate_all_plots`
         show : bool, optional
             If True, the plots are displayed before the documentation folder is created, by default False
         """
         self.create_all_plots(plot_specs)
 
-        # TODO
-        # technology
-        # mcard
-        # ADD data from mcard simulation
-
-        if show:
-            if len(self.plts) > 1:
-                for plt in self.plts[:-1]:
-                    plt.plot_pyqtgraph(show=False)
-
-            self.plts[-1].plot_pyqtgraph(show=True)
+        if show and self.plts:
+            for plt in self.plts:
+                plt.plot_pyqtgraph(show=False)
+
+            self.plts[0].show_pyqtgraph()
+
+            for plt in self.plts:
+                plt.mw_pg = None
+                plt.pw_pg = None
+                # remove the plot from the object to allow Parallel prcessing
+                # pickle is used to transfer between processes
 
         self.generate_all_plots(target_base_path, save_tikz_settings)
 
+        # sleep(30)
+
         self.create_documentation(target_base_path)
 
     def create_all_plots(
         self,
         plot_specs: List[Dict],
     ):
         """This method generates plots for selected devices in the DutLib in a highly configurable way.
@@ -392,195 +461,238 @@
                     'exact_match' : False,       #Bool, if True, use only keys that match "key" exactly
                     'FREQ'        : 10e9,        #optional, float: If given, use only data at FREQ
                     'xmin'        : 10e-2,       #optional, float: Minimum Value on x-axis to be displayed
                     'xmax'        : 1e2,         #optional, float: Maximum Value on x-axis to be displayed
                     'ymax'        : 300,         #optional, float: Maximum Value on y-axis to be displayed
                     'ymin'        : 0,           #optional, float: Minimum Value on y-axis to be displayed
                     'no_at'       : True,        #optional, Bool: if True, do not display the "at" quantities in the legend.
+                    'simulate'    : True,        #optional, Bool: if True, a matching simulation is added to the plot, if not given, default is True
                 },
 
         """
         plot_spec_defaults = {
             "style": MIX,
             "legend": True,
             "dut_type": DutType.npn,
             "no_at": False,  # no at_specifier= in legend
         }
+        sim_con = SimCon()
 
         # set defaults
         for plot_spec in plot_specs:
             for key in plot_spec_defaults:
                 if key not in plot_spec.keys():
                     plot_spec[key] = plot_spec_defaults[key]
 
         # check plot_spec
         for plot_spec in plot_specs:
             try:
                 plot_type = plot_spec["type"]
             except KeyError as err:
                 raise IOError("type not specified for plot specification.") from err
 
-            valid_plots = PLOT_DEFAULTS[plot_spec["dut_type"]].keys()
-            if not plot_type in valid_plots:
-                raise IOError(
-                    "Plot type "
-                    + plot_type
-                    + " not valid. Valid: "
-                    + " ".join(str(PLOT_DEFAULTS.keys()))
-                    + " ."
-                )
+            # valid_plots = PLOT_DEFAULTS[plot_spec["dut_type"]].keys()
+            # if not plot_type in valid_plots:
+            #     raise IOError(
+            #         f"Plot type {plot_type} not valid. Valid: "
+            #         + " ".join(str(PLOT_DEFAULTS.keys()))
+            #         + " ."
+            #     )
 
             if not plot_spec["style"] in PLOT_STYLES:
                 raise IOError("Plot style not valid. Valid: " + " ".join(PLOT_STYLES))
 
             if not "key" in plot_spec.keys():
-                raise IOError("Database key not specified for plot of type " + plot_type + " .")
+                raise IOError(f"Database key not specified for plot of type {plot_type}.")
 
             # matching key?
             if "exact_match" not in plot_spec.keys():
                 plot_spec["exact_match"] = False
 
         # ensure that plot with type gummel_vbc_mark_ft comes first
         for i, plot_spec in enumerate(plot_specs):
             if plot_spec["type"] == "gummel_vbc_mark_ft":
                 if i == 0:
                     pass
                 else:
-                    plot_specs[0], plot_specs[i] = plot_specs[i], plot_specs[0]  # swap elements
+                    plot_specs[0], plot_specs[i] = (
+                        plot_specs[i],
+                        plot_specs[0],
+                    )  # swap elements
 
                 break
 
         print("Generating plots...")
         # for every plot try to generate appropriate plots
         self.plts = []
         for plot_spec in plot_specs:
             plot_type = plot_spec["type"]
-            print("Generating plots of type " + plot_type + " .")
+            print(f"Generating plots of type {plot_type}.")
 
             style = plot_spec["style"]
-            print("Chosen plot style: " + style)
+            print(f"Chosen plot style: {style}")
 
             for dut in self.duts:
-                # load default settings of plot
-                try:
-                    x_log = PLOT_DEFAULTS[dut.dut_type][plot_type]["x_log"]
-                    y_log = PLOT_DEFAULTS[dut.dut_type][plot_type]["y_log"]
-                    quantity_x = PLOT_DEFAULTS[dut.dut_type][plot_type]["quantity_x"]
-                    quantity_y = PLOT_DEFAULTS[dut.dut_type][plot_type]["quantity_y"]
-                    legend_location = PLOT_DEFAULTS[dut.dut_type][plot_type]["legend_location"]
-                    at_specifier = PLOT_DEFAULTS[dut.dut_type][plot_type]["at"]
-                except KeyError:
-                    continue  # no plot_type in plot_defaults for this plot_spec
+                if "dut_filter" in plot_spec:
+                    if not plot_spec["dut_filter"](dut):
+                        continue
+                elif "dut_type" in plot_spec:
+                    if not dut.dut_type.is_subtype(plot_spec["dut_type"]):
+                        continue
 
-                # overwrite defaults with plot_spec
-                try:
-                    legend_location = plot_spec["legend_location"]
-                except KeyError:
-                    pass
+                if obtain(plot_spec, "simulate", dut.dut_type, plot_type, True):
+                    dut_sim = self.get_dut_sim(dut)
+                else:
+                    dut_sim = None
+
+                quantity_x = obtain(plot_spec, "quantity_x", dut.dut_type, plot_type)
+                x_log = obtain(plot_spec, "x_log", dut.dut_type, plot_type, value_default=False)
+
+                x_scale = obtain(plot_spec, "x_scale", dut.dut_type, plot_type, value_default=None)
 
-                if not isinstance(at_specifier, list):
+                quantity_y = obtain(plot_spec, "quantity_y", dut.dut_type, plot_type)
+                quantities_y = None
+                if quantity_y is None:
+                    quantities_y = plot_spec["quantities_y"]
+                    quantity_y = quantities_y[0]
+                y_log = obtain(plot_spec, "y_log", dut.dut_type, plot_type, value_default=False)
+                y_scale = obtain(plot_spec, "y_scale", dut.dut_type, plot_type, value_default=None)
+
+                # load settings from plot_spec with additions from defaults
+                legend_location = obtain(plot_spec, "legend_location", dut.dut_type, plot_type)
+                at_specifier = obtain(plot_spec, "at", dut.dut_type, plot_type)
+
+                if at_specifier is None:
+                    at_specifier = []
+                elif not isinstance(at_specifier, list):
                     at_specifier = [at_specifier]
 
+                if "xmin" in plot_spec.keys() or "xmax" in plot_spec.keys():
+                    x_limits = (plot_spec.get("xmin", None), plot_spec.get("xmax", None))
+                else:
+                    try:
+                        x_limits = PLOT_DEFAULTS[dut.dut_type][plot_type]["x_limits"]
+                    except KeyError:
+                        x_limits = (None, None)
+
+                if "ymin" in plot_spec.keys() or "ymax" in plot_spec.keys():
+                    y_limits = (plot_spec.get("ymin", None), plot_spec.get("ymax", None))
+                else:
+                    try:
+                        y_limits = PLOT_DEFAULTS[dut.dut_type][plot_type]["y_limits"]
+                    except KeyError:
+                        y_limits = (None, None)
+
+                caption = obtain(plot_spec, "caption", dut.dut_type, plot_type)
+
                 quantities_to_ensure = [quantity_x, quantity_y] + at_specifier
+                if quantities_y is not None:
+                    quantities_to_ensure += quantities_y
+
                 if "mark_ft" in plot_type:
                     quantities_to_ensure.append(specifiers.TRANSIT_FREQUENCY)
-                    peaks = {"vbe": [], "jc": [], "vbc": []}  # store peak ft values for later
+                    peaks = {
+                        "vbe": [],
+                        "jc": [],
+                        "vbc": [],
+                    }  # store peak ft values for later
 
                 at_scale = []
                 for at_ in at_specifier:
                     try:
                         at_scale_ = natural_scales[at_.specifier]
                     except AttributeError:
                         at_scale_ = natural_scales[at_]
 
-                    if at_ == specifiers.CURRENT + "B" or at_ == specifiers.CURRENT_DENSITY + "B":
-                        at_scale_ = at_scale_ * 1e3
+                    # if at_ == specifiers.CURRENT + "B" or at_ == specifiers.CURRENT_DENSITY + "B":
+                    #     at_scale_ = at_scale_ * 1e3
 
                     at_scale.append(at_scale_)
 
-                print("Generating plot of type " + plot_type + " for dut " + dut.name + " ...")
-                name = [
-                    "dut_",
-                    dut.name,
-                    "_",
-                    plot_type,
-                ]
+                print(f"Generating plot of type {plot_type} for dut {dut.name} ...")
+                name = [dut.name, plot_type]
                 if specifiers.TEMPERATURE in plot_spec.keys():
                     name.append("atT" + str(plot_spec[specifiers.TEMPERATURE]) + "K")
                 if specifiers.FREQUENCY in plot_spec.keys():
                     name.append("atf" + str(plot_spec[specifiers.FREQUENCY] * 1e-9) + "GHz")
-
                 for at_ in at_specifier:
                     name.append("at" + at_)
 
-                name = "_".join(name)
+                name = "_".join(name).replace(".", "p")
 
                 # calc drawn emitter windows area
-                AE0_drawn = dut.width * dut.length * dut.contact_config.count("E")
+                try:
+                    AE0_drawn = (
+                        dut.width * dut.length * dut.contact_config.count("E") * dut.ndevices
+                    )
+                except (TypeError, AttributeError):
+                    AE0_drawn = 1
 
                 # find temperatures
                 temps = []
                 for key in dut.data.keys():
-                    temps.append(dut.get_key_temperature(key))
+                    temp = dut.get_key_temperature(key)
+                    if specifiers.TEMPERATURE in plot_spec and np.isclose(
+                        temp, plot_spec[specifiers.TEMPERATURE]
+                    ):
+                        temps.append(dut.get_key_temperature(key))
+                    elif specifiers.TEMPERATURE not in plot_spec:
+                        temps.append(dut.get_key_temperature(key))
+
                 temps = list(set(temps))
 
                 for temp in temps:
-                    y_scale = 1
-                    x_label = None  # autolabel
-                    y_label = None
-                    if (
-                        quantity_y.specifier in specifiers.SS_PARA_Y
-                    ):  # special cases that I do not want in DMT
-                        y_scale = 1e3 / (1e6 * 1e6)  # mS/um^2
-                        y_label = r"$\Re{ \left\{ Y_{21} \right\} } / \si{\milli\siemens\per\square\micro\meter } $"
-
                     plt = Plot(
                         name,
                         style=style,
                         num=name,
                         x_specifier=quantity_x,
                         y_specifier=quantity_y,
                         x_log=x_log,
                         y_log=y_log,
+                        x_scale=x_scale,
                         y_scale=y_scale,
-                        x_label=x_label,
-                        y_label=y_label,
                         legend_location=legend_location,
                     )
-                    plt.dut_name = (
-                        dut.name
-                        + f"w{dut.width*1e6:.2f}um_l{dut.length*1e6:.2f}um_{len(self.plts)}"
-                    )
+
+                    plt.dut_name = (dut.name + f"{len(self.plts)}").replace(".", "p")
                     plt.plot_type = plot_type
                     plt.dut = dut
                     plt.temp = temp
                     plt.plot_spec = plot_spec
+                    plt.caption = caption
 
-                    n = 0
                     for key in dut.data.keys():
                         # selected only keys at temp
                         if not dut.get_key_temperature(key) == temp:
                             continue
 
-                        if specifiers.TEMPERATURE in plot_spec.keys():
-                            if temp != plot_spec[specifiers.TEMPERATURE]:
-                                continue  # key not suitable
-
                         match = False
                         if plot_spec["exact_match"]:
-                            match = plot_spec["key"] == dut.split_key(key)[-1]
+                            if isinstance(plot_spec["key"], str):
+                                match = plot_spec["key"] == dut.split_key(key)[-1]
+                            else:
+                                match = dut.split_key(key)[-1] in plot_spec["key"]
                         else:
-                            match = plot_spec["key"] in key
+                            if isinstance(plot_spec["key"], str):
+                                match = plot_spec["key"] in key
+                            else:
+                                match = any(
+                                    plot_spec_key in key for plot_spec_key in plot_spec["key"]
+                                )
 
                         if match:
                             df = dut.data[key]
                             if specifiers.FREQUENCY in plot_spec.keys():
                                 try:
                                     df = df[
-                                        df[specifiers.FREQUENCY] == plot_spec[specifiers.FREQUENCY]
+                                        np.isclose(
+                                            df[specifiers.FREQUENCY],
+                                            plot_spec[specifiers.FREQUENCY],
+                                        )
                                     ]
                                 except KeyError:
                                     pass
 
                             for quantity in quantities_to_ensure:
                                 try:
                                     df.ensure_specifier_column(
@@ -612,20 +724,14 @@
                                         if a > 0.0:
                                             F_th = dut.length / np.log(a)
                                         rth = SRTHRM * F_th
 
                                         df.loc[:, quantity] = temp + pdiss * rth
                                         dut.rth = rth
 
-                                try:
-                                    if quantity.specifier in specifiers_ss_para.SS_PARA_Y:
-                                        df.loc[:, quantity] = df[quantity] / AE0_drawn
-                                except:
-                                    pass
-
                             at_vals = []
                             for i, at_ in enumerate(at_specifier):
                                 at_val = df[at_].to_numpy()
                                 if at_.specifier == specifiers.VOLTAGE:
                                     at_val = np.round(at_val, decimals=3)
                                     at_val = np.unique(at_val)
                                 elif at_.specifier == specifiers.CURRENT:
@@ -638,121 +744,132 @@
                                 if "at_vals" in plot_spec:
                                     at_val = plot_spec["at_vals"][i]
                                     if not isinstance(at_val, list):
                                         at_val = [at_val]
 
                                 at_vals.append(at_val)
 
-                            units = []
-                            for i, at_ in enumerate(at_specifier):
-                                units.append(at_.get_tex_unit(scale=at_scale[i]))
+                            # units = []
+                            # for i, at_ in enumerate(at_specifier):
+                            #     units.append(at_.get_tex_unit(scale=at_scale[i]))
 
                             f = []
-                            if len(at_specifier) == 1:
+                            if len(at_specifier) == 0:
+                                f = [None]
+                            elif len(at_specifier) == 1:
                                 for point in at_vals[0]:
                                     f.append((point,))
                             elif len(at_specifier) == 2:
                                 f = [(x, y) for x in at_vals[0] for y in at_vals[1]]
                             else:
                                 raise IOError("at with more than two specifiers not implemented.")
 
                             for point in f:
                                 df_filter = True
-                                at_str = r"$"
-                                for i, (speci, u, scale_) in enumerate(
-                                    zip(at_specifier, units, at_scale)
-                                ):
-                                    df_filter = np.logical_and(
-                                        df_filter, np.isclose(df[speci], point[i], rtol=1e-3)
-                                    )
-                                    if at_str != r"$":
-                                        at_str += r",\,"
-                                    if plot_spec["no_at"]:
-                                        at_str += r"{0:1.2f}".format(point[i] * scale_) + u
-                                    else:
-                                        at_str += (
-                                            speci.to_tex()
-                                            + r" = {0:1.2f}".format(point[i] * scale_)
-                                            + u
+                                at_str = ""
+                                if point is None:
+                                    df_tmp = df
+                                else:
+                                    for i, at_speci in enumerate(at_specifier):
+                                        df_filter = np.logical_and(
+                                            df_filter,
+                                            np.isclose(df[at_speci], point[i], rtol=1e-3),
+                                        )
+
+                                        if at_str:
+                                            at_str += r",\,"
+
+                                        curr_str = at_speci.to_legend_with_value(
+                                            point[i], decimals=2
                                         )
 
-                                at_str += r"$"
-                                df_tmp = df[df_filter]
+                                        if plot_spec["no_at"]:
+                                            # only the number
+                                            at_str += "$" + curr_str.split("=")[1]
+                                        else:
+                                            at_str += curr_str
+
+                                    df_tmp = df[df_filter]
+
                                 x = df_tmp[quantity_x].to_numpy()
                                 y = df_tmp[quantity_y].to_numpy()
 
                                 # device if legend is wanted...default yes
-                                kwargs = {}
-                                if plot_spec["legend"]:
-                                    kwargs["label"] = at_str
-
-                                plt.add_data_set(
-                                    x,
-                                    y,
-                                    **kwargs,
-                                )
+                                if "legend" in plot_spec and not plot_spec["legend"]:
+                                    label = None
+                                else:
+                                    label = at_str
+
+                                if quantities_y is None:
+                                    plt.add_data_set(x, y, label=label)
+                                else:
+                                    for quant in quantities_y:
+                                        plt.add_data_set(
+                                            x, df_tmp[quant], label=f"${quant.to_tex():s}$"
+                                        )
 
                                 # add dots at peak ft
                                 if "mark_ft" in plot_type:
                                     ft = df_tmp[specifiers.TRANSIT_FREQUENCY].to_numpy() * 1e-9
                                     interp_fun_ft = interpolate.interp1d(x, ft)
                                     interp_fun_ic = interpolate.interp1d(x, y)
 
                                     index_peak_ft = np.argmax(ft)
                                     try:
                                         vbe_new = np.linspace(
-                                            x[index_peak_ft - 10], x[index_peak_ft + 10], 201
+                                            x[index_peak_ft - 10],
+                                            x[index_peak_ft + 10],
+                                            201,
                                         )  # may error
                                     except IndexError:
                                         vbe_new = np.linspace(
                                             x[index_peak_ft - 10], x[-1], 201
                                         )  # may error
 
                                     index_peak_ft = np.argmax(interp_fun_ft(vbe_new))
 
                                     vbe_peak = vbe_new[index_peak_ft]
                                     jc_peak = interp_fun_ic(vbe_new[index_peak_ft])
-                                    vbc_peak = point
 
                                     plt.add_data_set(
                                         np.tile(np.array(vbe_peak), 5),
                                         np.tile(np.array(jc_peak), 5),
                                         style=" ök",  # black dots
                                     )
                                     peaks["vbe"].append(np.tile(vbe_peak, 10))
                                     peaks["jc"].append(np.tile(jc_peak, 10))
                                     peaks["vbc"].append(np.tile(point[0], 10))
 
-                                n = n + 1
-
-                            if "ymin" in plot_spec.keys() or "ymax" in plot_spec.keys():
-                                if not "ymin" in plot_spec.keys():
-                                    plot_spec["ymin"] = None
-                                if not "ymax" in plot_spec.keys():
-                                    plot_spec["ymax"] = None
-                                plt.y_limits = (plot_spec["ymin"], plot_spec["ymax"])
-
-                            else:
-                                try:
-                                    plt.y_limits = PLOT_DEFAULTS[plot_type]["y_limits"]
-                                except KeyError:
-                                    pass
-
-                            if "xmin" in plot_spec.keys() or "xmax" in plot_spec.keys():
-                                if not "xmin" in plot_spec.keys():
-                                    plot_spec["xmin"] = None
-                                if not "xmax" in plot_spec.keys():
-                                    plot_spec["xmax"] = None
-                                plt.x_limits = (plot_spec["xmin"], plot_spec["xmax"])
+                                if dut_sim is not None:
+                                    # get a sweep
+                                    sweep = Sweep.get_sweep_from_dataframe(
+                                        data=df_tmp,
+                                        temperature=temp,
+                                        outputdef=[quantity_x, quantity_y],
+                                        # othervar={},
+                                    )
+                                    # simulate
+                                    sim_con.append_simulation(dut=dut_sim, sweep=sweep)
+                                    sim_con.run_and_read()
+                                    # add to plot
+                                    df_sim = dut_sim.get_data(sweep=sweep)
+                                    df_sim.ensure_specifier_column(
+                                        quantity_x, area=AE0_drawn, ports=dut.ac_ports
+                                    )
+                                    df_sim.ensure_specifier_column(
+                                        quantity_y, area=AE0_drawn, ports=dut.ac_ports
+                                    )
+                                    plt.add_data_set(
+                                        df_sim[quantity_x].to_numpy(),
+                                        df_sim[quantity_y].to_numpy(),
+                                        label=label + " sim",
+                                    )
 
-                            else:
-                                try:
-                                    plt.x_limits = PLOT_DEFAULTS[plot_type]["x_limits"]
-                                except KeyError:
-                                    pass
+                            plt.x_limits = x_limits
+                            plt.y_limits = y_limits
 
                     # plots that required to mark peak of ft are accounted for here.
                     if plot_type == "gummel_vbc_mark_ft":
                         dut.peaks = peaks
                     elif plot_type == "output_ib":  # add ft peaks if they exist
                         try:
                             peaks = dut.peaks
@@ -767,30 +884,26 @@
                                 jc[inds],
                                 style="-ök",  # black dots
                             )
                         except AttributeError:
                             pass
 
                     print(
-                        "...finished plot of type "
-                        + plot_type
-                        + " for dut "
-                        + dut.name
-                        + " , found "
-                        + str(n)
-                        + " lines."
+                        f"...finished plot of type {plot_type} for dut {dut.name}, found {len(dut.data)} lines."
                     )
 
-                    if n == 0:
-                        print("Found no lines for plot " + plot_type + " .")
-                    else:
+                    if plt.data:
                         self.plts.append(plt)
+                    else:
+                        print("Found no lines for plot " + plot_type + ". Plot is not added!")
 
     def generate_all_plots(
-        self, target_base_path: Union[str, Path], save_tikz_settings: Optional[Dict] = None
+        self,
+        target_base_path: Union[str, Path],
+        save_tikz_settings: Optional[Dict] = None,
     ):
         """Generates the plot tex and pdf files.
 
         If a plot with the same name already exists, it is deleted before the new is created.
 
         Parameters
         ----------
@@ -813,61 +926,66 @@
         """
         if isinstance(target_base_path, Path):
             base_path = target_base_path
         else:
             base_path = Path(target_base_path)
 
         save_tikz_settings_defaults = {
-            "width": "3in",
-            "height": "5in",
+            "width": "3.5in",
+            "height": "4in",
             "standalone": True,
             "svg": False,
             "build": True,
             "mark_repeat": 20,
-            "clean": False,  # Remove all files except *.pdf files in plots
+            "clean": True,  # Remove all files except *.pdf files in plots
         }
 
         if save_tikz_settings is None:
             save_tikz_settings = save_tikz_settings_defaults
         else:
             for key in save_tikz_settings_defaults:
                 if not key in save_tikz_settings.keys():
                     save_tikz_settings[key] = save_tikz_settings[key]
 
-        for plt in self.plts:
-            plot_path = (
-                base_path / "figs" / plt.dut_name / ("T" + str(plt.temp) + "K") / plt.plot_type
-            )
-
-            if plt.plot_type == "tj_jc_at_vbc":
-                plot_path = (
-                    base_path
-                    / "figs"
-                    / plt.dut_name
-                    / ("T" + str(plt.temp) + "K")
-                    / (plt.plot_type + "rth_" + "{0:1.1f}".format(plt.dut.rth * 1e-3) + "kWperK")
-                )
-
-            if plot_path.exists():
-                rmtree(plot_path)
-
-            plot_path.mkdir(parents=True, exist_ok=True)
-
-            # special output from plot_spec
-            save_tikz_settings_tmp = copy.deepcopy(save_tikz_settings)
-            for special in ["width", "height"]:
-                try:
-                    save_tikz_settings_tmp[special] = plt.plot_spec[special]
-                except KeyError:
-                    continue
+        paths = Parallel(n_jobs=20, verbose=10)(
+            _build_plot(plt, base_path, save_tikz_settings) for plt in self.plts
+        )
+        for i_plt, plt in enumerate(self.plts):
+            plt.path = paths[i_plt]
+        # for plt in self.plts:
+        #     plot_path = (
+        #         base_path / "figs" / plt.dut_name / ("T" + str(plt.temp) + "K") / plt.plot_type
+        #     )
+
+        #     if plt.plot_type == "tj_jc_at_vbc":
+        #         plot_path = (
+        #             base_path
+        #             / "figs"
+        #             / plt.dut_name
+        #             / ("T" + str(plt.temp) + "K")
+        #             / (plt.plot_type + "rth_" + "{0:1.1f}".format(plt.dut.rth * 1e-3) + "kWperK")
+        #         )
+
+        #     if plot_path.exists():
+        #         rmtree(plot_path)
+
+        #     plot_path.mkdir(parents=True, exist_ok=True)
+
+        #     # special output from plot_spec
+        #     save_tikz_settings_tmp = copy.deepcopy(save_tikz_settings)
+        #     for special in ["width", "height"]:
+        #         try:
+        #             save_tikz_settings_tmp[special] = plt.plot_spec[special]
+        #         except KeyError:
+        #             continue
 
-            plt.legend_location = "upper right outer"
-            filename = plt.save_tikz(plot_path, **save_tikz_settings_tmp)
+        #     plt.legend_location = "upper right outer"
+        #     filename = plt.save_tikz(plot_path, **save_tikz_settings_tmp)
 
-            plt.path = plot_path / filename.replace("tex", "pdf")
+        #     plt.path = plot_path / filename.replace("tex", "pdf")
 
     def create_documentation(self, target_base_path: Union[str, Path]):
         """Generates the other tex files from the template.
 
         The template path from the config is used. The key is::
 
             directories:
@@ -923,48 +1041,88 @@
         # subfile that contains overview of library
         lib_tex = SubFile(master="../documentation.tex")
         lib_tex.append(self.dut_lib.toTex())
 
         # subfile that contains all plots
         plots_tex = SubFile(master="../documentation.tex")
         doc = Tex()
-        for dut in self.duts:
-            with doc.create(Section(dut.name)):
-                plts_for_this_dut = []
-                for plt in self.plts:
-                    if plt.dut == dut:
-                        plts_for_this_dut.append(plt)
-
-                temps = []
-                for plt in plts_for_this_dut:
-                    temps.append(plt.temp)
+        dut_types = set([dut.dut_type for dut in self.duts])
+        duts_sorted = sorted(self.duts, key=lambda dut_a: (dut_a.dut_type, dut_a.name))
+        for dut_type in dut_types:
+            duts_filtered = [dut for dut in duts_sorted if dut.dut_type == dut_type]
+            with doc.create(Section(dut_type.string)):
+                for dut in duts_filtered:
+                    plts_for_this_dut = []
+                    for plt in self.plts:
+                        if plt.dut == dut:
+                            plts_for_this_dut.append(plt)
 
-                temps = list(set(temps))
+                    if not plts_for_this_dut:
+                        continue
 
-                for temp in temps:
-                    with doc.create(Subsection("T=" + str(temp) + "K")):
+                    with doc.create(Subsection(dut.name)):
+                        temps = []
                         for plt in plts_for_this_dut:
-                            if plt.temp == temp:
-                                # check if plot exists:
-                                # Why? The plots are added as images not as tikz plots Oo
-                                if plt.path.is_file():
-                                    doc.append(NoEscape(r"\FloatBarrier "))
-                                    with doc.create(Figure(position="ht!")) as _plot:
-                                        _plot.append(
-                                            NoEscape(r"\setlength\figurewidth{\textwidth}")
-                                        )
-                                        # _plot.append(CommandInput(arguments=Arguments(plt.path)))
-                                        _plot.add_image('"' + str(plt.path) + '"')
-                                        _plot.add_caption(
-                                            NoEscape(
-                                                PLOT_DEFAULTS[dut.dut_type][plt.plot_type]["tex"]
-                                            )
-                                        )
-                                        # _plot.append(CommandLabel(arguments=Argument(plt.dut_name + plt.)))
+                            temps.append(plt.temp)
+
+                        temps = list(set(temps))
 
-                                    doc.append(NoEscape(r"\FloatBarrier "))
+                        for temp in temps:
+                            with doc.create(Subsubsection("T=" + str(temp) + "K", label=False)):
+                                for plt in plts_for_this_dut:
+                                    if plt.temp == temp:
+                                        # check if plot exists:
+                                        # Why? The plots are added as images not as tikz plots Oo
+                                        if plt.path.is_file():
+                                            doc.append(NoEscape(r"\FloatBarrier "))
+                                            with doc.create(Figure(position="ht!")) as _plot:
+                                                _plot.append(
+                                                    NoEscape(r"\setlength\figurewidth{\textwidth}")
+                                                )
+                                                # _plot.append(CommandInput(arguments=Arguments(plt.path)))
+                                                _plot.add_image(
+                                                    '"'
+                                                    + str(plt.path.relative_to(destination))
+                                                    + '"'
+                                                )
+                                                _plot.add_caption(NoEscape(plt.caption))
+                                                # _plot.append(CommandLabel(arguments=Argument(plt.dut_name + plt.)))
+
+                                            doc.append(NoEscape(r"\FloatBarrier "))
 
         # put into subfile
         plots_tex.append(doc)
 
         lib_tex.generate_tex(str(destination / "content" / "lib_overview"))
         plots_tex.generate_tex(str(destination / "content" / "lib_plots"))
+
+
+@delayed
+def _build_plot(plt, base_path, save_tikz_settings):
+    plot_path = base_path / "figs" / plt.dut_name / ("T" + str(plt.temp) + "K") / plt.plot_type
+
+    if plt.plot_type == "tj_jc_at_vbc":
+        plot_path = (
+            base_path
+            / "figs"
+            / plt.dut_name
+            / ("T" + str(plt.temp) + "K")
+            / (plt.plot_type + "rth_" + "{0:1.1f}".format(plt.dut.rth * 1e-3) + "kWperK")
+        )
+
+    if plot_path.exists():
+        rmtree(plot_path)
+
+    plot_path.mkdir(parents=True, exist_ok=True)
+
+    # special output from plot_spec
+    save_tikz_settings_tmp = copy.deepcopy(save_tikz_settings)
+    for special in ["width", "height"]:
+        try:
+            save_tikz_settings_tmp[special] = plt.plot_spec[special]
+        except KeyError:
+            continue
+
+    plt.legend_location = "upper right outer"
+    filename = plt.save_tikz(plot_path, **save_tikz_settings_tmp)
+
+    return plot_path / filename.replace("tex", "pdf")
```

### Comparing `DMT_core-2.0.0/DMT/core/dut_circuit.py` & `DMT_core-2.1.0/DMT/core/dut_circuit.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 * String with path to a netlist of a circuit
 * String with the netlist of a circuit
 * List with paths to netlists or strings with netlists, these will be combined into the netlist to simulate.
 
 
 Author: Mario Krattenmacher | Mario.Krattenmacher@semimod.de
 """
+
 # DMT_core
 # Copyright (C) from 2022  SemiMod
 # Copyright (C) until 2021  Markus Müller, Mario Krattenmacher and Pascal Kuthe
 # <https://gitlab.com/dmt-development/dmt-core>
 #
 # This file is part of DMT_core.
 #
@@ -29,16 +30,22 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>
 import copy
 from collections import OrderedDict
-from typing import List, Dict
-from DMT.core import create_md5_hash, DutView, McParameterCollection, DutType, Technology
+from typing import List, Dict, Type, Union
+from DMT.core import (
+    create_md5_hash,
+    DutView,
+    McParameterCollection,
+    DutType,
+    Technology,
+)
 from DMT.core.mcard import MCard
 
 try:
     from semver.version import Version as VersionInfo
 except ImportError:
     from semver import VersionInfo
 
@@ -74,15 +81,15 @@
     """
 
     def __init__(
         self,
         database_dir: str,
         name: str,
         dut_type: DutType,
-        inp_circuit,
+        input_circuit,
         simulator_options: dict = None,
         get_circuit_arguments: dict = None,
         **kwargs
     ):
         self._inp_header = ""
 
         super().__init__(database_dir, name, dut_type, **kwargs)
@@ -96,15 +103,29 @@
             self.get_circuit_arguments = OrderedDict()
         else:
             self.get_circuit_arguments = OrderedDict(sorted(get_circuit_arguments.items()))
 
         # save for later use
         self._inp_circuit = None
         self._modelcard = None
-        self.inp_header = inp_circuit
+
+        if (
+            isinstance(input_circuit, MCard)
+            and self.technology
+            and hasattr(self.technology, "scale_modelcard")
+        ):
+            input_circuit = self.technology.scale_modelcard(
+                mcard=input_circuit,
+                lE0=self.length,
+                bE0=self.width,
+                nfinger=self.nfinger,
+                config=self.contact_config,
+            )
+
+        self.inp_header = input_circuit
 
     @property
     def inp_header(self):
         """Getter method for the input header of the simulation input file"""
         return self._inp_header
 
     @inp_header.setter
@@ -168,41 +189,41 @@
             "modelcard": modelcard,
         }
 
     @classmethod
     def from_json(
         cls,
         json_content: Dict,
-        classes_technology: List[type[Technology]],
+        classes_technology: List[Type[Technology]],
         subclass_kwargs: Dict = None,
     ) -> "DutCircuit":
         """Static class method. Loads a DutCircuit object from a pickle file with full path save_dir.
 
         Calls the from_json method of DutView with all dictionary inside the "parent" keyword. Afterwards the additional parameters are set correctly.
 
         Parameters
         ----------
         json_content  :  dict
             Readed dictionary from a saved json DutCircuit.
-        classes_technology : List[type[Technology]]
+        classes_technology : List[Type[Technology]]
             All possible technologies this loaded DutCircuit can have. One will be choosen according to the serialized technology loaded from the file.
         subclass_kwargs : Dict, optional
             Additional kwargs necessary to create the concrete subclassed DutView.
 
         Returns
         -------
         DutTcad
             Loaded object.
         """
         if json_content["__DutCircuit__"] != SEMVER_DUTCIRCUIT_CURRENT:
             raise NotImplementedError("DMT.DutCircuit: Unknown version of DutCircuit to load!")
 
         if subclass_kwargs is None:
             subclass_kwargs = {}
-        subclass_kwargs["inp_circuit"] = json_content["inp_header"]
+        subclass_kwargs["input_circuit"] = json_content["inp_header"]
 
         dut_view = super().from_json(
             json_content["parent"], classes_technology, subclass_kwargs=subclass_kwargs
         )
 
         dut_view._modelcard = json_content["modelcard"]
         dut_view.simulator_options = json_content["simulator_options"]
@@ -225,36 +246,39 @@
         """
         if isinstance(modelcard, MCard) or isinstance(modelcard, McParameterCollection):
             self._modelcard = modelcard
             self.inp_header = modelcard
         else:
             raise OSError("The modelcard has to be a instance of MCard or its children!")
 
-    def get_hash(self):
+    def get_hash(self) -> Union[bool, str]:
         """Returns a md5 hash generated from self.inp_header, if it is not set, this will return False!
 
         Is overwritten here, to include the imported and appended files!
 
         Returns
         -------
         str or False
 
         Notes
         -----
         Also account for dut.name?
         """
-        if self.inp_header is None:
+        if (
+            not self.inp_header
+        ):  # if the input header is empty, no circuit was given. So this device is an empty hull currently -> No hash
             return False
 
         if self._list_va_file_contents:
             list_va = [
                 vafile.get_tree_hash() for vafile in self._list_va_file_contents
             ]  # directly use the hash here - hash of hash should be ok :)
         else:
             list_va = []
+
         return create_md5_hash(self.inp_header, *self.list_copy, *list_va)
 
     def create_inp_header(self, inp_circuit):
         """Creates the inp_header from the given circuit.
 
         Parameters
         ----------
```

### Comparing `DMT_core-2.0.0/DMT/core/dut_dummy.py` & `DMT_core-2.1.0/DMT/core/dut_dummy.py`

 * *Files identical despite different names*

### Comparing `DMT_core-2.0.0/DMT/core/dut_lib.py` & `DMT_core-2.1.0/DMT/core/dut_lib.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,16 +23,17 @@
 import copy
 import re
 import filecmp
 import numpy as np
 import json
 from pathlib import Path
 from joblib import Parallel, delayed
-from typing import List
-from DMT.core import DutType, DutTypeFlag, print_progress_bar, DutView, Technology
+from typing import List, Type, Union
+from DMT.core import DutType, DutTypeFlag, print_progress_bar, DutView, Technology, df_concat
+from DMT.core.dut_view import DutView
 from DMT.exceptions import NoOpenDeembeddingDut, NoShortDeembeddingDut
 
 try:
     from semver.version import Version as VersionInfo
 except ImportError:
     from semver import VersionInfo
 
@@ -201,15 +202,15 @@
         Deembeds measured AC data with the corresponding O&S data.
     deembed_DC()
         Deembeds measured AC data with the corresponding O&S data.
     """
 
     def __init__(
         self,
-        deem_types=None,
+        deem_types: List[DutType] = None,
         AC_filter_names=None,
         DC_filter_names=None,
         is_deembedded_DC=False,
         is_deembedded_AC=False,
         save_dir=None,
         force=False,
         n_jobs=4,
@@ -220,55 +221,55 @@
             self.deem_types = deem_types
 
         self.AC_filter_names = AC_filter_names
         self.DC_filter_names = DC_filter_names
         self.is_deembedded_AC = is_deembedded_AC
         self.is_deembedded_DC = is_deembedded_DC
 
-        self.deem_open = (
-            DutTypeFlag.flag_open
-        )  # deem_open_bjt # look only for the flag not for the device!
-        self.deem_short = DutTypeFlag.flag_short  # deem_short_bjt
+        self.deem_open = DutTypeFlag.flag_open  # look only for the flag not for the device!
+        self.deem_short = DutTypeFlag.flag_short
 
-        self.duts = []  # The devices that shall be managed by this dut
-        self._dut_ref = None  # The reference device of this technology
+        self.duts: List[DutView] = []  # The devices that shall be managed by this dut
+        self._dut_ref: DutView = None  # The reference device of this technology
         self.dut_ref_dut_dir = None
-        self._dut_intrinsic = None  # The intrinsic dut of the reference dut (without rbi)
+        self._dut_intrinsic: DutView = None  # The intrinsic dut of the reference dut (without rbi)
         self.dut_intrinsic_dut_dir = None  # The intrinsic dut of the reference dut (without rbi)
-        self._dut_internal = None  # The internal dut of the reference dut (with rbi)
+        self._dut_internal: DutView = None  # The internal dut of the reference dut (with rbi)
         self.dut_internal_dut_dir = None  # The intrinsic dut of the reference dut (without rbi)
         self._save_dir = None  # Here the DutLib will try to save itself
         if save_dir is not None:
             if force:
                 try:
                     shutil.rmtree(save_dir)
                 except FileNotFoundError:
                     pass
 
             self.save_dir = save_dir  # Here the DutLib will try to save itself
 
-        self.ignore_duts = []  # list of names which are not returned while iteration
+        self.ignore_duts: List[str] = []  # list of names which are not returned while iteration
 
         self.n_jobs = n_jobs  # number of parallel jobs while directory import
 
         # additional information to help assess the data later
         self.wafer = None
         self.date_tapeout = None
         self.date_received = None
 
+        self.plots = []  # list of plots for the documentation.
+
     @property
     def dut_ref(self):
         """Returns always just self._dut_ref"""
         if self._dut_ref is None:
             raise IOError("Dut_ref doesn't exist!")
 
         return self._dut_ref
 
     @dut_ref.setter
-    def dut_ref(self, dut):
+    def dut_ref(self, dut: DutView):
         """Ensure that dut_ref is in duts"""
         if not id(dut) in [id(dut_) for dut_ in self.duts]:
             self.duts.append(dut)
 
         self._dut_ref = dut
 
     @property
@@ -276,15 +277,15 @@
         """Returns always just self._dut_internal"""
         if self._dut_internal is None:
             raise IOError("Dut_internal doesn't exist!")
 
         return self._dut_internal
 
     @dut_internal.setter
-    def dut_internal(self, dut):
+    def dut_internal(self, dut: DutView):
         """Ensure that dut_internal is in duts"""
         if not id(dut) in [id(dut_) for dut_ in self.duts]:
             self.duts.append(dut)
 
         self._dut_internal = dut
 
     @property
@@ -292,15 +293,15 @@
         """Returns always just self._dut_intrinsic"""
         if self._dut_intrinsic is None:
             raise IOError("Dut_intrinsic doesn't exist!")
 
         return self._dut_intrinsic
 
     @dut_intrinsic.setter
-    def dut_intrinsic(self, dut):
+    def dut_intrinsic(self, dut: DutView):
         """Ensure that dut_intrinsic is in duts"""
         if not id(dut) in [id(dut_) for dut_ in self.duts]:
             self.duts.append(dut)
 
         self._dut_intrinsic = dut
 
     @property
@@ -432,36 +433,36 @@
         print("DutLib imported " + str(len(duts)) + " DUTs.")
 
         if not self.is_deembedded_AC and not self.is_deembedded_DC:
             self.add_duts(duts)
 
         return duts
 
-    def add_duts(self, duts):
+    def add_duts(self, duts: Union[List[DutView], DutView]):
         """Add duts to the DutLib duts array.
 
         Parameters
         ----------
         duts : [DutView] or DutView
             The dut or duts that shall be added.
         """
         if self.is_deembedded_AC or self.is_deembedded_DC:
             raise IOError("DutLib: I am already deembedded and don" "t want to add Duts.")
 
         try:
             for dut in duts:
                 if dut.name in [dut_a.name for dut_a in self.duts]:
                     raise IOError(
-                        "DutLib: A DuT of this name already exists. Dut names must be unique!"
+                        f"DutLib: A DuT with the name {dut.name} already exists. Dut names must be unique!"
                     )
                 self.duts.append(dut)
         except TypeError:
             if duts.name in [dut_a.name for dut_a in self.duts]:
                 raise IOError(
-                    "DutLib: A DuT of this name already exists. Dut names must be unique!"
+                    f"DutLib: A DuT with the name {dut.name} already exists. Dut names must be unique!"
                 )
             self.duts.append(duts)
 
     def save(self):
         """Save the DutLib to save_dir.
 
         The DutLib will be saved as a json file and in the folder "duts" there will be the DutViews.
@@ -548,27 +549,27 @@
 
         file_path = self.save_dir / "dut_lib.json"
         file_path.write_text(json.dumps(dict_content, indent=4), encoding="utf8")
 
     @staticmethod
     def load(
         lib_directory,
-        classes_technology: List[type[Technology]] = None,
-        classes_dut_view: List[type["DutView"]] = None,
+        classes_technology: List[Type[Technology]] = None,
+        classes_dut_view: List[Type["DutView"]] = None,
     ) -> "DutLib":
         """Static class method. Loads a DutLib object from a pickle or json file with full path lib_directory.
 
         Parameters
         ----------
         lib_directory  :  str or os.Pathlike
             Path to the direcotry that contains a pickled DutLib object that shall be loaded.
-        classes_technology : List[type[Technology]]
-            All possible technologies this loaded DutView can have. One will be choosen according to the serialized technology loaded from the file.
-        classes_dut_view : List[type[DutView]]
-            All possible DutViews this loaded DutView can be. One will be choosen according to the serialized dutview class name loaded from the file.
+        classes_technology : List[Type[Technology]]
+            All possible technologies this loaded DutView can have. One will be chosen according to the serialized technology loaded from the file.
+        classes_dut_view : List[Type[DutView]]
+            All possible DutViews this loaded DutView can be. One will be chosen according to the serialized DutView class name loaded from the file.
 
 
 
         Returns
         -------
         DutLib
             Loaded object from the json or pickle file.
@@ -577,14 +578,18 @@
         lib_directory = Path(lib_directory).resolve()
         if (lib_directory / "dut_lib.json").exists():
             with (lib_directory / "dut_lib.json").open("r", encoding="utf8") as file_json:
                 json_content = json.load(file_json)
             if not json_content["__DutLib__"] == SEMVER_DUTLIB_CURRENT:
                 raise IOError("DMT.DutLib: Tried to load a DutLib with unkown version.")
 
+            for key, value in json_content.items():
+                if value == "None":
+                    json_content[key] = None
+
             deem_types = [
                 DutType.deserialize(deem_type) for deem_type in json_content["deem_types"]
             ]
             dut_lib = DutLib(
                 deem_types=deem_types,
                 AC_filter_names=json_content["AC_filter_names"],
                 DC_filter_names=json_content["DC_filter_names"],
@@ -612,34 +617,36 @@
         else:
             raise IOError(
                 "DMT.DutLib: Loading failed since no DutLib file was found (supported are json and pickle)."
             )
 
         save_dir_old = ""
         # need to cast paths? This is needed when the machine is changed -> new absolute paths...
-        if (
-            lib_directory != dut_lib.save_dir
-        ):  # dut_lib.save_dir is the old absolute path of the lib
+        if dut_lib.save_dir is None:
+            # write to internal value to avoid consistency check
+            dut_lib._save_dir = lib_directory  # pylint: disable=protected-access
+        elif lib_directory != dut_lib.save_dir:
+            # dut_lib.save_dir is the old absolute path of the lib
             save_dir_old = str(dut_lib.save_dir)
             # write to internal value to avoid consistency check
             dut_lib._save_dir = lib_directory  # pylint: disable=protected-access
 
         # load all duts
         ignore_duts = copy.deepcopy(dut_lib.ignore_duts)
         dut_lib.ignore_duts = []  # load all duts, even the one who were ignored
-        # for dir_name, dir_list, file_list in os.walk(dut_lib.save_dir / "duts"):  # find the duts
-        #     for file_dut in file_list:
-        #         if file_dut.endswith(".json") or file_dut.endswith(".p"):
-        #             dut_lib.duts.append(DutView.load_dut(os.path.join(dir_name, file_dut)))
+
+        loaded_paths = []
         for file_dut in (dut_lib.save_dir / "duts").glob("**/*.json"):
             dut_lib.duts.append(
                 DutView.load_dut(file_dut, classes_technology, classes_dut_view=classes_dut_view)
             )
+            loaded_paths.append(file_dut.parent)
         for file_dut in (dut_lib.save_dir / "duts").glob("**/*.p"):
-            dut_lib.duts.append(DutView.load_dut(file_dut))
+            if not file_dut.parent in loaded_paths:
+                dut_lib.duts.append(DutView.load_dut(file_dut))
 
         # correct dut paths:
         if dut_lib.dut_ref_dut_dir is not None:
             dut_lib.dut_ref_dut_dir = Path(dut_lib.dut_ref_dut_dir)
             if not dut_lib.dut_ref_dut_dir.exists():
                 dut_lib.dut_ref_dut_dir = Path(
                     str(dut_lib.dut_ref_dut_dir).replace(save_dir_old, str(lib_directory))
@@ -740,19 +747,27 @@
         # in the simplest case we only have one deemb device. Then use it.
         if len(open_list) == 1 and len(short_list) == 1:
             print("\n")
             print("DMT will now try to deembed all devices in DutLib object:")
             for i_dev, dev in enumerate(dev_list):
                 self.deembed_dut_AC(dev, open_list[0], short_list[0])
                 print_progress_bar(
-                    i_dev, len(dev_list), prefix="Deembedding AC:", suffix=dev.name, length=50
+                    i_dev,
+                    len(dev_list),
+                    prefix="Deembedding AC:",
+                    suffix=dev.name,
+                    length=50,
                 )
 
             print_progress_bar(
-                len(dev_list), len(dev_list), prefix="Deembedding AC:", suffix=dev.name, length=50
+                len(dev_list),
+                len(dev_list),
+                prefix="Deembedding AC:",
+                suffix=dev.name,
+                length=50,
             )
             self.is_deembedded_AC = True
             return
 
         # more than one deemb device, then we need filters.
         if not width_filter and not length_filter and not name_filter and user_fun is None:
             raise IOError(
@@ -820,20 +835,28 @@
                     + "Available opens: "
                     + "".join([dut.name + " " for dut in open_list])
                 )
             elif len(suitable_shorts) == 0:
                 raise NoShortDeembeddingDut("For " + dev.name + " no Short was found.")
             else:
                 print_progress_bar(
-                    i_dev, len(dev_list), prefix="Deembedding AC:", suffix=dev.name, length=50
+                    i_dev,
+                    len(dev_list),
+                    prefix="Deembedding AC:",
+                    suffix=dev.name,
+                    length=50,
                 )
                 self.deembed_dut_AC(dev, suitable_opens[0], suitable_shorts[0])
 
             print_progress_bar(
-                len(dev_list), len(dev_list), prefix="Deembedding AC:", suffix=dev.name, length=50
+                len(dev_list),
+                len(dev_list),
+                prefix="Deembedding AC:",
+                suffix=dev.name,
+                length=50,
             )
 
             # Deembed DC data if required
         self.is_deembedded_AC = True
 
     def deembed_DC(
         self,
@@ -921,29 +944,39 @@
                         short_i,
                         function_dut=function_dut,
                         function_df=function_df,
                         t_ref=t_ref,
                         forced_current=forced_current,
                     )
                 print_progress_bar(
-                    i_dev, len(dev_list), prefix="Deembedding DC:", suffix=dev.name, length=50
+                    i_dev,
+                    len(dev_list),
+                    prefix="Deembedding DC:",
+                    suffix=dev.name,
+                    length=50,
                 )
 
             print_progress_bar(
-                len(dev_list), len(dev_list), prefix="Deembedding DC:", suffix="finish", length=50
+                len(dev_list),
+                len(dev_list),
+                prefix="Deembedding DC:",
+                suffix="finish",
+                length=50,
             )
             self.is_deembedded_DC = True
             return mres
 
         # more than one deemb device, then we need filters.
         if not width_filter and not length_filter and not name_filter:
             raise IOError(
                 "DMT -> DutLib: You did not select any filter flags that would allow deembedding!"
             )
 
+        mres = {}
+
         # Iterating through the dev_list, which contains all devices that require deembedding.
         for i_dev, dev in enumerate(dev_list):
             print("\n")
             print("DMT will now try to DC deembed all devices in DutLib object:")
             suitable_shorts = []
             for deem_dut in short_list:
                 if name_filter:
@@ -978,27 +1011,37 @@
 
                 raise IOError(message)
 
             elif len(suitable_shorts) == 0:
                 raise NoShortDeembeddingDut("For " + dev.name + " no short was found.")
             else:
                 print_progress_bar(
-                    i_dev, len(dev_list), prefix="Deembedding DC:", suffix=dev.name, length=50
+                    i_dev,
+                    len(dev_list),
+                    prefix="Deembedding DC:",
+                    suffix=dev.name,
+                    length=50,
                 )
-                mres = self.deembed_dut_DC(
-                    dev,
-                    suitable_shorts[0],
-                    function_dut=function_dut,
-                    function_df=function_df,
-                    t_ref=t_ref,
-                    forced_current=forced_current,
+                mres.update(
+                    self.deembed_dut_DC(
+                        dev,
+                        suitable_shorts[0],
+                        function_dut=function_dut,
+                        function_df=function_df,
+                        t_ref=t_ref,
+                        forced_current=forced_current,
+                    )
                 )
 
         print_progress_bar(
-            len(dev_list), len(dev_list), prefix="Deembedding DC:", suffix=dev.name, length=50
+            len(dev_list),
+            len(dev_list),
+            prefix="Deembedding DC:",
+            suffix=dev.name,
+            length=50,
         )
 
         self.is_deembedded_DC = True
 
         return mres
 
     def deembed_dut_AC(self, dut, dut_open, dut_short):
@@ -1162,29 +1205,40 @@
         if not self.is_deembedded_AC and not self.is_deembedded_DC:
             self.add_duts(duts)
 
         return duts
 
     # Makes it possible to iterate over DutLib objects
     def __iter__(self):
-        return iter([dut for dut in self.duts if dut.name not in self.ignore_duts])
+        return iter(
+            sorted(
+                [dut for dut in self.duts if dut.name not in self.ignore_duts],
+                key=lambda dut: dut.name,
+            )
+        )
 
     def __getitem__(self, key):
         return self.duts[key]
 
     def normalize(self, dut_type):
         for dut in self.duts:
             if dut.dut_type == dut_type:
                 if dut.ndevices > 1:
                     for key in dut.data.keys():
                         df = dut.data[key]
                         dut.data[key] = df.parallel_norm(dut.ndevices, *dut.ac_ports)
 
     def deembed_dut_DC(
-        self, dut, dut_short, function_dut=None, function_df=None, t_ref=300, forced_current=False
+        self,
+        dut,
+        dut_short,
+        function_dut=None,
+        function_df=None,
+        t_ref=300,
+        forced_current=False,
     ):
         """Deembeds all DC_measurements in GSG-Pads.
 
         Parameters
         ----------
         dut         : [dut]
             Current DuT which is to be deembedded.
@@ -1207,81 +1261,108 @@
                 "DMT->DutLib->deembed_DC: Either function_dut or function_df can be given, but not both!"
             )
 
         # print how exactly deembedding is performed for possible future debugging purposes
         # ISSUE: No for-loop "(meas_filter, deem_filter) in self.DC_filter_names:" performed here.
         # all measurements stored under keys are DC deembedded here!
         if function_dut is not None:
-            mres_tref = function_dut(dut_short)
+            mres = function_dut(dut_short)
             print("\n")
             print(dut.name)
             print("\n")
             for key in dut.data.keys():
                 print(key)
                 dut.data[key] = dut.data[key].deembed_DC(
-                    mres=mres_tref, forced_current=forced_current
+                    mres=mres,
+                    forced_current=forced_current,
+                    ac_ports=dut.ac_ports,
+                    reference_node=dut.reference_node,
                 )
         else:
-            mres_tref = None
+            mres = {}
 
             for meas_filter, deem_filter in self.DC_filter_names:
                 # get the short keys
                 short_keys = []
                 for short_key in dut_short.data.keys():
                     if re.search(deem_filter, short_key, re.IGNORECASE):
                         short_keys.append(short_key)
 
                 if len(short_keys) == 1:
                     # if only one short key has been found we just take it for everything
                     df_short = dut_short.data[short_keys[0]]
 
                     if function_df is None:
-                        mres_tref = df_short.determine_mres(forced_current=forced_current)
+                        mres = df_short.determine_mres(
+                            forced_current=forced_current,
+                            ac_ports=dut_short.ac_ports,
+                            reference_node=dut_short.reference_node,
+                        )
                     else:
-                        mres_tref = function_df(dut_short)
+                        mres = function_df(dut_short)
 
                 for key in dut.data.keys():
                     # check if df needs to be DC deembedded
                     if re.search(meas_filter, key, re.IGNORECASE):
                         if len(short_keys) == 1:
                             mres = mres_tref
-                        else:  # NOT TESTED!!!!
-                            # bad news...try to find matching temperatures. #TODO: Does not work if no keys are found
+                        else:
+                            # try to find matching temperatures.
                             key_temperature = dut.get_key_temperature(key)
+                            short_keys_matching = []
                             for short_key in short_keys:
                                 if np.isclose(
-                                    key_temperature, dut_short.get_key_temperature(short_key)
+                                    key_temperature,
+                                    dut_short.get_key_temperature(short_key),
                                 ):
-                                    break
-                            df_short = dut_short.data[short_key]
+                                    short_keys_matching.append(short_key)
+
+                            df_shorts = []
+                            for short_key in short_keys_matching:
+                                df_shorts.append(dut_short.data[short_key])
+                            if df_shorts:
+                                df_short = df_concat(*df_shorts)
+                            else:
+                                raise IOError(
+                                    f"Did not find suitable short keys for {dut.name} at {key_temperature}K. \n The available short keys were: "
+                                    + ",".join(short_keys)
+                                )
 
                             if function_df is None:
                                 try:
-                                    mres = df_short.determine_mres(forced_current=forced_current)
+                                    mres[f"{dut_short.name}@{key_temperature:.0f}K"] = (
+                                        df_short.determine_mres(
+                                            forced_current=forced_current,
+                                            ac_ports=dut_short.ac_ports,
+                                            reference_node=dut_short.reference_node,
+                                        )
+                                    )
                                 except IOError as err:
                                     raise IOError(
                                         "Column missing in df of dut "
                                         + dut_short.name
                                         + " of df with key "
                                         + short_key
-                                        + ". Available keys: "
-                                        + str(df_short.data.keys())
+                                        + ". Available columns: "
+                                        + str(df_short.columns())
                                         + "."
                                     ) from err
                             else:
-                                mres = function_df(dut_short)
-
-                            if np.isclose(key_temperature, t_ref):
-                                mres_tref = mres
+                                mres["f{dut_short.name}@{key_temperature:.0f}K"] = function_df(
+                                    dut_short
+                                )
 
                         dut.data[key] = dut.data[key].deembed_DC(
-                            mres=mres, forced_current=forced_current
+                            mres=mres,
+                            forced_current=forced_current,
+                            ac_ports=dut.ac_ports,
+                            reference_node=dut.reference_node,
                         )
 
-        return mres_tref
+        return mres
 
     def toTex(self):
         """This function generates a TeX representation of a DutLib.
 
         This function generates a section with the title "Measured Devices"
         For each DutType a table is generated that summarizes the available device dimensions for this DutType.
         """
@@ -1347,14 +1428,25 @@
                                         for dut in self
                                         if dut.dut_type == dut_type
                                         and dut.contact_config == config
                                         and dut.flavor == flavor
                                     ]
                                 )
                             )
+                            if dut_type.is_subtype(DutTypeFlag.flag_tlm):
+                                for dut in duts:
+                                    dut_name = dut.name.replace("_", "\_")
+                                    doc.append(
+                                        NoEscape(
+                                            f"One TLM-Structure with the name {dut_name} with the width \\SI{{{dut.width*1e6}}}{{\\micro\\metre}} and the lengths \\SI{{{dut.length[0]*1e6}}}{{\\micro\\metre}} and \\SI{{{dut.length[1]*1e6}}}{{\\micro\\metre}}."
+                                        )
+                                    )
+                                doc.append("\r")
+                                continue
+
                             lE0s = list(set([dut.length for dut in duts]))
                             bE0s = list(set([dut.width for dut in duts]))
                             lE0s.sort()
                             bE0s.sort()
                             header = "|" + " c | " * (
                                 len(lE0s) + 1
                             )  # one col for each length and one for bE0 indices
```

### Comparing `DMT_core-2.0.0/DMT/core/dut_meas.py` & `DMT_core-2.1.0/DMT/core/dut_meas.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """ Manage measurement data in DMT in as a measurement dut. Additionally has attributes which define the size and die of the dut.
 
 """
+
 # DMT_core
 # Copyright (C) from 2022  SemiMod
 # Copyright (C) until 2021  Markus Müller, Mario Krattenmacher and Pascal Kuthe
 # <https://gitlab.com/dmt-development/dmt-core>
 #
 # This file is part of DMT_core.
 #
@@ -19,15 +20,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>
 
 import logging
 import re
-from typing import List, Dict
+from typing import List, Dict, Type
 from DMT.core import Technology
 from DMT.core.dut_view import DutView
 
 
 try:
     from semver.version import Version as VersionInfo
 except ImportError:
@@ -134,24 +135,24 @@
                 "die": self.die,
                 "ndevices": self.ndevices,
                 "deemb_name": self.deemb_name,
             }
         }
 
     @classmethod
-    def from_json(cls, json_content: Dict, classes_technology: List[type[Technology]]) -> "DutMeas":
+    def from_json(cls, json_content: Dict, classes_technology: List[Type[Technology]]) -> "DutMeas":
         """Static class method. Loads a DutMeas object from a pickle file with full path save_dir.
 
         Calls the from_json method of DutView with all dictionary inside the "parent" keyword. Afterwards the additional parameters are set correctly.
 
         Parameters
         ----------
         json_content  :  dict
             Readed dictionary from a saved json DutMeas.
-        classes_technology : List[type[Technology]]
+        classes_technology : List[Type[Technology]]
             All possible technologies this loaded DutMeas can have. One will be choosen according to the serialized technology loaded from the file.
 
         Returns
         -------
         DutMeas
             Loaded object.
         """
```

### Comparing `DMT_core-2.0.0/DMT/core/dut_tcad.py` & `DMT_core-2.1.0/DMT/core/dut_tcad.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """ Provdes a class for TCAD DuTs
 
 Provides a interface superclass. Here all methods which must be implemented by all TCAD interfaces are collected.
 
 Author: Mario Krattenmacher | Mario.Krattenmacher@semimod.de
 """
+
 # DMT_core
 # Copyright (C) from 2022  SemiMod
 # Copyright (C) until 2021  Markus Müller, Mario Krattenmacher and Pascal Kuthe
 # <https://gitlab.com/dmt-development/dmt-core>
 #
 # This file is part of DMT_core.
 #
@@ -21,15 +22,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>
 import copy
 import logging
-from typing import List, Dict
+from typing import List, Dict, Type
 from DMT.core import create_md5_hash, DutView, Technology
 
 try:
     from semver.version import Version as VersionInfo
 except ImportError:
     from semver import VersionInfo
 
@@ -120,15 +121,17 @@
                 # could not open input file. Assume it is the already read string
                 self._inp_header = value
         else:
             self._inp_structure = copy.deepcopy(value)
             self._inp_header = self.create_inp_header(value)
 
         logging.info(
-            "Successfully created input header of dut %s%s!", self.name, str(self.get_hash())
+            "Successfully created input header of dut %s%s!",
+            self.name,
+            str(self.get_hash()),
         )
         logging.debug("Content:\n%s", self._inp_header)
 
     def info_json(self, **_kwargs) -> Dict:
         """Returns a dict with serializeable content for the json file to create.
 
         The topmost dict MUST have only one key: The string casted class name.
@@ -149,26 +152,26 @@
             "inp_header": self.inp_header,
         }
 
     @classmethod
     def from_json(
         cls,
         json_content: Dict,
-        classes_technology: List[type[Technology]],
+        classes_technology: List[Type[Technology]],
         subclass_kwargs: Dict = None,
     ) -> "DutTcad":
         """Static class method. Loads a DutTcad object from a pickle file with full path save_dir.
 
         Calls the from_json method of DutView with all dictionary inside the "parent" keyword. Afterwards the additional parameters are set correctly.
 
         Parameters
         ----------
         json_content  :  dict
             Readed dictionary from a saved json DutTcad.
-        classes_technology : List[type[Technology]]
+        classes_technology : List[Type[Technology]]
             All possible technologies this loaded DutTcad can have. One will be choosen according to the serialized technology loaded from the file.
         subclass_kwargs : Dict, optional
             Additional kwargs necessary to create the concrete subclassed DutView.
 
         Returns
         -------
         DutTcad
@@ -178,29 +181,31 @@
             raise NotImplementedError("DMT.DutTcad: Unknown version of DutTcad to load!")
 
         if subclass_kwargs is None:
             subclass_kwargs = {}
         subclass_kwargs["inp_structure"] = json_content["inp_header"]
 
         dut_view = super().from_json(
-            json_content["parent"], classes_technology, subclass_kwargs=subclass_kwargs
+            json_content["parent"],
+            classes_technology,
+            subclass_kwargs=subclass_kwargs,
         )
 
         return dut_view
 
     def get_hash(self):
         """Returns a md5 hash generated from self.inp_header, if it is not set, this will return False!
 
         In case a InpStructure is set, this always recreates the inp_header :/.
 
         Returns
         -------
         str or False
         """
-        if self.inp_header is None:
+        if not self.inp_header:
             return False
 
         # i have to ensure always correct hash for a dut... sorry
         if self._inp_structure is not None:
             self._inp_header = self.create_inp_header(self._inp_structure)
 
         return create_md5_hash(self._inp_header + self.sim_command)
```

### Comparing `DMT_core-2.0.0/DMT/core/dut_type.py` & `DMT_core-2.1.0/DMT/core/dut_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """ Used to flag the dut type for each dut view
 
 """
+
 # DMT_core
 # Copyright (C) from 2022  SemiMod
 # Copyright (C) until 2021  Markus Müller, Mario Krattenmacher and Pascal Kuthe
 # <https://gitlab.com/dmt-development/dmt-core>
 #
 # This file is part of DMT_core.
 #
@@ -122,28 +123,45 @@
 
         Ignores the flag_subtype!
 
         Parameters
         ----------
         other : int, DutTypeInt
         """
-        try:
-            val = int(self & other)
-        except AttributeError:
-            val = self.value & other
-
         # remove subtype flag..
-        val_subtype_flags = ~(
-            DutTypeFlag._flag_subtype_1
-            | DutTypeFlag._flag_subtype_2
-            | DutTypeFlag._flag_subtype_3
-            | DutTypeFlag._flag_subtype_4
-        )
+        # val_subtype_flags = (
+        #     DutTypeFlag._flag_subtype_1
+        #     | DutTypeFlag._flag_subtype_2
+        #     | DutTypeFlag._flag_subtype_3
+        #     | DutTypeFlag._flag_subtype_4
+        # )
+        if DutTypeFlag._flag_subtype_1 & self:
+            self_wo_subtype = self - DutTypeFlag._flag_subtype_1
+        elif DutTypeFlag._flag_subtype_2 & self:
+            self_wo_subtype = self - DutTypeFlag._flag_subtype_2
+        elif DutTypeFlag._flag_subtype_3 & self:
+            self_wo_subtype = self - DutTypeFlag._flag_subtype_3
+        elif DutTypeFlag._flag_subtype_4 & self:
+            self_wo_subtype = self - DutTypeFlag._flag_subtype_4
+        else:
+            self_wo_subtype = self
+
+        if DutTypeFlag._flag_subtype_1 & other:
+            other_wo_subtype = other - DutTypeFlag._flag_subtype_1
+        elif DutTypeFlag._flag_subtype_2 & other:
+            other_wo_subtype = other - DutTypeFlag._flag_subtype_2
+        elif DutTypeFlag._flag_subtype_3 & other:
+            other_wo_subtype = other - DutTypeFlag._flag_subtype_3
+        elif DutTypeFlag._flag_subtype_4 & other:
+            other_wo_subtype = other - DutTypeFlag._flag_subtype_4
+        else:
+            other_wo_subtype = other
 
-        return bool(val_subtype_flags.value & val)
+        res = self_wo_subtype & other_wo_subtype
+        return res == other
 
     def __lt__(self, other):
         try:
             return DutTypeInt(self.value < other.value, string=self.get_string(), nodes=self.nodes)
         except AttributeError:
             return DutTypeInt(self.value < other, string=self.get_string(), nodes=self.nodes)
 
@@ -219,18 +237,18 @@
     flag_cap = auto()
     flag_res = auto()
     flag_tetrode = auto()
     flag_tlm = auto()
     flag_deem = auto()
     flag_vdp = auto()
 
-    flag_npn = auto()
-    flag_pnp = auto()
-    flag_n_mos = auto()
-    flag_p_mos = auto()
+    # flag_npn = auto()
+    # flag_pnp = auto()
+    # flag_n_mos = auto()
+    # flag_p_mos = auto()
 
     flag_open = auto()
     flag_short = auto()
 
     def get_nodes(self):
         """
         Return the nodes that are typically found in this DutType. For convenience.
@@ -290,18 +308,24 @@
     )  # because of node names :(
     deem_mos = DutTypeInt(
         deemb_struct | DutTypeFlag.flag_mos_deemb,
         nodes=["G", "D", "S", "B"],
         string="mos_deemb",
     )  # because of node names :(
 
-    npn = DutTypeInt(bjt | DutTypeFlag.flag_npn, string="npn")  # nodes are inherited from bjt
-    pnp = DutTypeInt(bjt | DutTypeFlag.flag_pnp, string="pnp")
-    n_mos = DutTypeInt(mos | DutTypeFlag.flag_n_mos, string="nmos")
-    p_mos = DutTypeInt(mos | DutTypeFlag.flag_p_mos, string="pmos")
+    # npn = DutTypeInt(bjt | DutTypeFlag.flag_npn, string="npn")  # nodes are inherited from bjt
+    npn = DutTypeInt(
+        bjt | DutTypeFlag._flag_subtype_1, string="npn"
+    )  # nodes are inherited from bjt
+    # pnp = DutTypeInt(bjt | DutTypeFlag.flag_pnp, string="pnp")
+    pnp = DutTypeInt(bjt | DutTypeFlag._flag_subtype_2, string="pnp")
+    # n_mos = DutTypeInt(mos | DutTypeFlag.flag_n_mos, string="nmos")
+    n_mos = DutTypeInt(mos | DutTypeFlag._flag_subtype_1, string="nmos")
+    # p_mos = DutTypeInt(mos | DutTypeFlag.flag_p_mos, string="pmos")
+    p_mos = DutTypeInt(mos | DutTypeFlag._flag_subtype_2, string="pmos")
 
     diode = DutTypeInt(device | DutTypeFlag.flag_diode, nodes=["C", "A"], string="diode")
     pn_diode = DutTypeInt(diode | DutTypeFlag._flag_subtype_1, string="pn-diode")
     pin_diode = DutTypeInt(diode | DutTypeFlag._flag_subtype_2, string="pin-diode")
     cap = DutTypeInt(device | DutTypeFlag.flag_cap, nodes=["C", "A"], string="capacitance")
     res = DutTypeInt(device | DutTypeFlag.flag_res, nodes=["C", "A"], string="resistor")
 
@@ -363,15 +387,17 @@
             if dut_type is None:
                 warnings.warn(
                     "DMT.DutType: Did not find the loaded duttype with the string '"
                     + dict_loaded["string"]
                     + "' in the current DMT version."
                 )
                 dut_type = DutTypeInt(
-                    dict_loaded["value"], string=dict_loaded["string"], nodes=dict_loaded["nodes"]
+                    dict_loaded["value"],
+                    string=dict_loaded["string"],
+                    nodes=dict_loaded["nodes"],
                 )
             else:
                 dut_type.nodes = dict_loaded["nodes"]
         else:
             raise IOError(
                 "DMT.DutType: I dont know how to deserealize the DutType: " + dict_loaded["DutType"]
             )
```

### Comparing `DMT_core-2.0.0/DMT/core/dut_view.py` & `DMT_core-2.1.0/DMT/core/dut_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,41 +13,40 @@
 # DMT_core is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>
+from __future__ import annotations
 import os
 import re
 import shutil
 import _pickle as cpickle  # type: ignore
 import json
 import copy
 import logging
 from pathlib import Path
 import pandas as pd
-from typing import List, Dict
+from typing import List, Dict, Type, Union
 
 try:
     from semver.version import Version as VersionInfo
 except ImportError:
     from semver import VersionInfo
 
-from DMT.core import (
-    DatabaseManager,
-    read_data,
-    DataFrame,
-    VAFileMap,
-    DutTypeFlag,
-    DutTypeInt,
-    DutType,
-    Technology,
-)
+from DMT.core.data_frame import DataFrame
+from DMT.core.database_manager import DatabaseManager
+from DMT.core.data_reader import read_data
+from DMT.core.dut_type import DutTypeFlag, DutTypeInt, DutType
+from DMT.core.va_file import VAFileMap
+from DMT.core.sweep import Sweep
+import DMT.core.technology as dmt_tech
 from DMT.config import DATA_CONFIG
+from DMT.exceptions import UnknownColumnError
 
 SEMVER_DUTVIEW_CURRENT = VersionInfo(major=1, minor=0)
 
 
 class DutView(object):
     """DutView is the parent class of all DUTs in DMT.
 
@@ -165,15 +164,15 @@
         separate_databases=False,
         list_copy=None,
         t_max=None,
         sim_dir=DATA_CONFIG["directories"]["simulation"],
         simulate_on_server=None,
         simulator_command="",
         simulator_arguments=None,
-        technology=None,
+        technology: "dmt_tech.Technology" = None,
         width=None,
         length=None,
         nfinger=None,
         contact_config=None,
         flavor=None,
         ac_ports=None,
         nodes=None,
@@ -201,15 +200,15 @@
             if not isinstance(list_copy, list):
                 self.list_copy = [list_copy]
             else:
                 self.list_copy = list_copy
         self._list_va_file_contents: list[VAFileMap] = []
 
         # if the dut already exists and no force -> error!
-        if self.save_dir:
+        if self.save_dir.exists():
             if force:
                 # delete the saved database
                 self.del_db()
                 self.del_dut()
             elif loading:
                 pass
             else:
@@ -247,14 +246,16 @@
         self.va_code_filter = va_code_filter
 
         if simulator_arguments is None:
             self.sim_args = []
         else:
             self.sim_args = simulator_arguments
 
+        if not isinstance(sim_dir, Path):
+            sim_dir = Path(sim_dir)
         self.sim_dir = sim_dir
 
         self.technology = technology
         self.contact_config = contact_config
         self.flavor = flavor
         self.width = width
         self.length = length
@@ -274,15 +275,15 @@
             self.simulate_on_server = simulate_on_server
         self.zip_result = True
 
         # in these attributes, store the name of another dut that has been used for deembedding...for documentation this is nice
         self.open_deembedded_with = "-"
         self.short_deembedded_with = "-"
 
-    def prepare_simulation(self, sweep):
+    def prepare_simulation(self, sweep: Sweep):
         """Creates a simulation folder, appends the sweep to the structure definition and creates a input file in the simulation folder.
 
         Parameters
         ----------
         sweep : Sweep
         """
         logging.info(
@@ -356,15 +357,15 @@
         """Option to write a data table for a simulation. As the file type may depend on the simulator this is not implemented here!"""
         raise NotImplementedError("Has to be overwritten in the subclass.")
 
     def make_pbs(self, sweep):
         """Create a PBS script for the PBS job system. (See: https://albertsk.files.wordpress.com/2011/12/pbs.pdf)"""
         raise NotImplementedError("Not Implemented for this Dut Class!")
 
-    def make_input(self, sweep):
+    def make_input(self, sweep: Sweep):
         """Joins simulation header with a given Sweep object and returns it.
 
         Parameters
         ----------
         sweep : :class:`DMT.core.sweep.Sweep`
             Sweep specification according to the Sweep class.
         """
@@ -397,15 +398,15 @@
         IOError
             If the given sweep can not be read.
         """
         raise NotImplementedError(
             "DutView does not implement the concrete import_output_data method!"
         )
 
-    def validate_simulation_successful(self, sweep):
+    def validate_simulation_successful(self, sweep: Sweep):
         """Checks if the simulation of the given sweep was successful.
 
         Parameters
         ----------
         sweep  :  :class:`DMT.core.sweep.Sweep`
             Sweep that has been simulated.
 
@@ -419,15 +420,15 @@
             If the sim log file does not exist.
         """
         raise NotImplementedError(
             "DutView does not implement the concrete import_output_data method!"
         )
 
     @property
-    def save_dir(self):
+    def save_dir(self) -> Path:
         if self.get_hash():
             return self.database_dir / (self.name + "_hash_" + str(self.get_hash()))
         else:
             return self.database_dir / self.name
 
     @property
     def database_dir(self):
@@ -437,15 +438,15 @@
     def database_dir(self, new_dir):
         """Make sure data is loaded before changing save location of this DutView."""
         if not self._data:
             self.load_db()
 
         self._database_dir = Path(new_dir)
 
-    def get_db_dir(self, name="db"):
+    def get_db_dir(self, name="db") -> Path:
         """Returns the name for a db, either use 'db' for regular behavior or use 'sweep.get_hash()' for a db per sweep."""
         return self.save_dir / (name + ".h5")
 
     @property
     def dut_dir(self):
         return self.save_dir / "dut.json"
 
@@ -458,15 +459,15 @@
 
         """
         if not self._data:  # empty dict evaluates to false
             self.load_db()
 
         return self._data
 
-    def get_sim_folder(self, sweep):
+    def get_sim_folder(self, sweep: Sweep) -> Path:
         """Returns the simulation folder of the given sweep
 
         Parameters
         ----------
         sweep  :  Sweep
             Sweep object that corresponds to the folder.
 
@@ -477,15 +478,15 @@
         """
         return (
             self.sim_dir
             / (self.name + str(self.get_hash()))
             / (sweep.name + "_" + sweep.get_hash())
         )
 
-    def delete_sim_results(self, sweep, ignore_errors=False):
+    def delete_sim_results(self, sweep: Sweep, ignore_errors=False):
         """Deletes the simulation results of the given sweep.
 
         Parameters
         ----------
         sweep  :  Sweep
             Sweep object that corresponds to the folder.
         ignore_errors : {False, True}, optional
@@ -505,15 +506,19 @@
         self.save_dir.mkdir(parents=True, exist_ok=True)
         self._database_dir = self._database_dir.resolve()  # convert to absolute path
 
         self.save_db()
 
         self.dut_dir.write_text(json.dumps(self.info_json(**kwargs), indent=4), encoding="utf8")
 
-    def info_json(self, **_kwargs):
+        if self.dut_dir.with_suffix(".p").exists():
+            # it there is still a "old" pickle file in the directory -> remove it
+            self.dut_dir.with_suffix(".p").unlink()
+
+    def info_json(self, **_kwargs) -> Dict:
         """Returns a dict with serializeable content for the json file to create.
 
         Add the info about the concrete subclass to create here! See :py:method::`DMT.core.dut_meas.DutMeas.info_json()` for an example implementation.
 
         Returns
         -------
         dict
@@ -574,26 +579,26 @@
         """Return state values to be pickled. Implemented according `to <https://www.ibm.com/developerworks/library/l-pypers/index.html>`_ ."""
         self.__dict__ = state  # pylint: disable=attribute-defined-outside-init
         self.__dict__["_data"] = {}
 
     @staticmethod
     def load_dut(
         file_dut,
-        classes_technology: List[type[Technology]] = None,
-        classes_dut_view: List[type["DutView"]] = None,
+        classes_technology: List[Type["dmt_tech.Technology"]] = None,
+        classes_dut_view: List[Type["DutView"]] = None,
     ) -> "DutView":
         """Static class method. Loads a DutView object from a pickle file with full path save_dir.
 
         Parameters
         ----------
         file_dut  :  str or os.Pathlike
             Path to the json or pickle DutView file that shall be loaded.
-        classes_technology : List[type[Technology]]
+        classes_technology : List[Type[Technology]]
             All possible technologies this loaded DutView can have. One will be choosen according to the serialized technology loaded from the file.
-        classes_dut_view : List[type[DutView]]
+        classes_dut_view : List[Type[DutView]]
             All possible DutViews this loaded DutView can be. One will be choosen according to the serialized dutview class name loaded from the file.
 
         Returns
         -------
         DutView
             Loaded object.
         """
@@ -609,17 +614,22 @@
                 classes_dut_view += _DEFAULT_DUT_VIEWS
 
             with file_dut.open("r", encoding="utf8") as file_json:
                 json_content = json.load(file_json)
 
             # the key on the first dictionary is the class
             clsstr_dut_view = list(json_content.keys())[0]
-            cls_dut_view = next(
-                cls_dv for cls_dv in classes_dut_view if str(cls_dv) == clsstr_dut_view
-            )
+            try:
+                cls_dut_view = next(
+                    cls_dv for cls_dv in classes_dut_view if str(cls_dv) == clsstr_dut_view
+                )
+            except StopIteration as err:
+                raise IOError(
+                    f"DMT.DutLib: Encountered unknown DutView class while loading the library: {clsstr_dut_view}"
+                ) from err
 
             dut = cls_dut_view.from_json(json_content[clsstr_dut_view], classes_technology)
 
         elif file_dut.suffix == ".p":
             with file_dut.open(mode="rb") as handle:
                 dut = cpickle.load(handle)
         else:
@@ -638,24 +648,24 @@
 
         return dut
 
     @classmethod
     def from_json(
         cls,
         json_content: Dict,
-        classes_technology: List[type[Technology]],
+        classes_technology: List[Type["dmt_tech.Technology"]],
         subclass_kwargs: Dict = None,
     ) -> "DutView":
         """Static class method. Loads a DutView object from a pickle file with full path save_dir.
 
         Parameters
         ----------
         json_content  :  dict
             Readed dictionary from a saved json DutView.
-        classes_technology : List[type[Technology]]
+        classes_technology : List[Type[Technology]]
             All possible technologies this loaded DutView can have. One will be choosen according to the serialized technology loaded from the file.
         subclass_args: List = None,
             Positional arguments needed
         subclass_kwargs: Dict = None,
 
         Returns
         -------
@@ -665,19 +675,24 @@
         if json_content["__DutView__"] != SEMVER_DUTVIEW_CURRENT:
             raise NotImplementedError("DMT.DutView: Unknown version of DutView to load!")
 
         serialized_technology = json_content["technology"]
         if serialized_technology is None:
             tech = None
         else:
-            cls_technology = next(
-                cls_tech
-                for cls_tech in classes_technology
-                if str(cls_tech) == serialized_technology["class"]
-            )
+            try:
+                cls_technology = next(
+                    cls_tech
+                    for cls_tech in classes_technology
+                    if str(cls_tech.__name__) in serialized_technology["class"]
+                )
+            except StopIteration as err:
+                raise IOError(
+                    "DMT.DutLib: Encountered unknown Technology class while loading the library."
+                ) from err
             args = serialized_technology.get("args", [])
             kwargs = serialized_technology.get("kwargs", {})
             if serialized_technology.get("constructor", None) is None:
                 tech = cls_technology(*args, **kwargs)
             else:
                 tech = getattr(cls_technology, serialized_technology["constructor"])(
                     *args, **kwargs
@@ -718,27 +733,35 @@
             VAFileMap.import_dict(va_file) for va_file in json_content["list_va_file_contents"]
         ]
         dut_view.zip_result = json_content["zip_result"]
         dut_view.open_deembedded_with = json_content["open_deembedded_with"]
         dut_view.short_deembedded_with = json_content["short_deembedded_with"]
         return dut_view
 
-    def add_data(self, data, key=None, force=True, **kwargs):
+    def add_data(
+        self,
+        data: Union[DataFrame, Sweep, str, os.Pathlike],
+        key: Union[str, None] = None,
+        force: bool = True,
+        **kwargs,
+    ):
         """Add a measurement or simulation data to the DutView's data.
 
         Parameters
         ----------
         data   :   DataFrame, sweep or str
             If DataFrame: Directly added to the data using the given key.
             If str: Full path to the file that shall be added to the database
             if sweep: Simulated sweep to import.
         key    :   string, optional
             Key that shall be used in the database to save the data.
         force  :  bool, optional
             Default=True. If = True, the data is added even if it already exists.
+        kwargs : keyword arguments, optional
+            Passed on to read_data in case of str as a data argment.
         """
         if key is None:
             try:
                 key = self.get_sweep_key(data)
             except AttributeError:
                 pass
 
@@ -752,43 +775,44 @@
             else:
                 logging.info(
                     "DMT -> DutView -> add_data(): Skipped a dataframe with key %s since it was already existent in dut.data.",
                     key,
                 )
                 return
 
-        try:
+        if isinstance(data, DataFrame) or isinstance(data, pd.DataFrame):
+            # it is a regular dataframe
+            # prevents pandas bug with non-unique columns:
+            if not data.columns.is_unique:
+                data = data.loc[:, ~data.columns.duplicated()]
+            self.data[key] = data
+        elif isinstance(data, Sweep):
+            # simulation valid?
+            self.validate_simulation_successful(data)
+            # try special import
+            self.import_output_data(data)
+        else:
             self.data[key] = read_data(data, **kwargs)
-        except (OSError, IOError, TypeError) as _error:
-            # could not read file using the general read data!
-            if isinstance(data, DataFrame) or isinstance(data, pd.DataFrame):
-                # it is a regular dataframe
-                # prevents pandas bug with non-unique columns:
-                if not data.columns.is_unique:
-                    data = data.loc[:, ~data.columns.duplicated()]
-                self.data[key] = data
-            else:
-                # simulation valid?
-                self.validate_simulation_successful(data)
-                # try special import
-                self.import_output_data(data)
 
-        logging.info("DMT -> DutView -> add_data(): Added a dataframe with key %s to the dut.", key)
+        logging.info(
+            "DMT -> DutView -> add_data(): Added a dataframe with key %s to the dut.",
+            key,
+        )
 
-    def remove_data(self, key):
+    def remove_data(self, key: str):
         """Remove a measurement or simulation dataframe from the DutView's data.
 
         Parameters
         ----------
         key    :   string
             Key that shall be removed from the database.
         """
         del self.data[key]
 
-    def get_data(self, key="iv", sweep=None):
+    def get_data(self, key: str = "iv", sweep: Sweep = None) -> DataFrame:
         """Return data stored in the DutView's data.
 
         One needs to specify either:
 
         - key      : The data stored under the path key in the dut's database is returned.
         - sweep    : Get the data from this sweep. If none, key must be a valid key for the database.
         - sweep+key: Return the data stored as self.get_sweep_key(sweep)+'/'+key from the dut's database.
@@ -862,14 +886,23 @@
                 df = df.clean_data(
                     self.nodes,
                     self.reference_node,
                     fallback=fallback,
                     ac_ports=self.ac_ports,
                     **kwargs,
                 )
+            except UnknownColumnError as err:
+                raise UnknownColumnError(
+                    "The DutView is "
+                    + self.name
+                    + " of DutType "
+                    + self.dut_type.get_string()
+                    + " with the ac_ports "
+                    + str(self.ac_ports)
+                ) from err
 
             self.data[key] = df
 
     def save_db(self, sweep_keys=None):
         """Write a database for this dut. If it already exists it is overwritten. Does NOT save all keys starting with '_'
 
         Parameters
@@ -952,15 +985,15 @@
             try:
                 self._data = self.manager.load_db(self.get_db_dir())
             except FileNotFoundError:
                 return False
 
         return True
 
-    def check_existence_sweep(self, sweep):
+    def check_existence_sweep(self, sweep: Sweep):
         """Return true, if the combination dut+sweep has already been simulated.
 
         If self.data is None, the database is loaded first.
 
         Parameters
         ----------
         sweep  : :class:`DMT.core.sweep.Sweep`
@@ -1007,15 +1040,15 @@
         -------
         list[str]
             key splitted at '/'
 
         """
         return key.split("/")
 
-    def get_sweep_key(self, sweep):
+    def get_sweep_key(self, sweep: Sweep):
         """Key for the dict in dut.data.
 
         Parameters
         ----------
         sweep : :class:`~DMT.core.sweep.Sweep` or str
             Either the key for the given sweep or if it is a string, directly the string
```

### Comparing `DMT_core-2.0.0/DMT/core/hasher.py` & `DMT_core-2.1.0/DMT/core/hasher.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 * The simulation directory in used the :ref:`config`
 * The dut subfolder named `<dut_name><dut_hash>`. The dut name is a attribute of :ref:`DutView<dut_view>`. The hash calculation depends on the subclass, but most times this is simply the MD5-Hash of all input files, for example the netlist file and the Verilog-AMS code.
 * The sweep subfolder named `<sweep_name><sweep_hash>`. The sweep name is a attribute of :ref:`Sweep<sweep>`. The hash is calculated from text converted sweep definition.
 
 Author: Mario Krattenmacher | Mario.Krattenmacher@semimod.de
 """
+
 # DMT_core
 # Copyright (C) from 2022  SemiMod
 # Copyright (C) until 2021  Markus Müller, Mario Krattenmacher and Pascal Kuthe
 # <https://gitlab.com/dmt-development/dmt-core>
 #
 # This file is part of DMT_core.
 #
@@ -29,15 +30,15 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>
 import hashlib
 import os
 from typing import Union
 
 
-def create_md5_hash(*contents: Union[str, os.PathLike]):
+def create_md5_hash(*contents: Union[str, os.PathLike]) -> str:
     """Construct the hash MD5 string with all parameters
 
     Parameters
     ----------
     contents : str
         Either a path to a file to read or some object which can be converted to a string using str()
```

### Comparing `DMT_core-2.0.0/DMT/core/mc_parameter.py` & `DMT_core-2.1.0/DMT/core/mc_parameter.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 Additionally parameters can be compared, they are considered equal, if they have the
 same name and value. Also collections can be compared, they are equal, if they have
 the same parameters and all parameters are equal.
 
 Finally the classes here also add some pretty printing and loading and saving using pickle.
 """
+
 # DMT_core
 # Copyright (C) from 2022  SemiMod
 # Copyright (C) until 2021  Markus Müller, Mario Krattenmacher and Pascal Kuthe
 # <https://gitlab.com/dmt-development/dmt-core>
 #
 # This file is part of DMT_core.
 #
@@ -44,19 +45,23 @@
     from semver import VersionInfo
 
 
 from pathlib import Path
 
 import _pickle as cpickle  # type: ignore
 import numpy as np
-from typing import Dict, OrderedDict, Type, Union, List, Optional
+from typing import Dict, OrderedDict, Type, Union, List, Optional, TYPE_CHECKING
 from pint.formatting import siunitx_format_unit
 from pint.errors import UndefinedUnitError
 
 from DMT.core import unit_registry
+
+if TYPE_CHECKING:
+    from DMT.core.circuit import Circuit
+
 from DMT.exceptions import (
     ValueExcludedError,
     ValueTooLargeError,
     ValueTooSmallError,
     BoundsError,
     ParaExistsError,
 )
@@ -65,15 +70,15 @@
     # try to import only, so it is a soft dependency...
     from pylatex import LongTable, MultiColumn, Section, NoEscape
     from DMT.external.pylatex import Tex  # pylint: disable=ungrouped-imports
 except ImportError:
     pass
 
 SEMVER_MCPARAMETER_CURRENT = VersionInfo(major=1, minor=0)
-SEMVER_MCPARAMETER_Collection_CURRENT = VersionInfo(major=1, minor=0)
+SEMVER_MCPARAMETER_Collection_CURRENT = VersionInfo(major=1, minor=0, patch=1)
 
 
 class McParameter(object):
     """Objects of this class represent a model card parameter. If you want to store many of them, see McParameterCollection class.
 
     Attributes
     ----------
@@ -502,21 +507,25 @@
         -------
         value  :  int or float
             Checked value
         """
         # type check, either int or float is allowed
         if self.val_type == int:
             if int(value) != value:
-                raise TypeError(f"The parameter {self:s} is of type Integer!")
+                raise TypeError(
+                    f"The parameter {self:s} is of type Integer! Given was {value} of type {type(value)}."
+                )
 
             value = int(value)
         elif not isinstance(
             value, (int, float)
         ):  # for floats also integer are allowed. This catches everything else like strings or lists etc.
-            raise TypeError(f"The parameter {self:s} is of type Float!")
+            raise TypeError(
+                f"The parameter {self:s} is of type Float! Given was {value} of type {type(value)}."
+            )
 
         # range check
         value_too_large = False
         value_too_small = False
 
         if self.inc_min and value < self.min:
             value_too_small = True
@@ -597,14 +606,25 @@
     def __eq__(self, other: McParameter) -> bool:
         """Comparing parameters, equal if name and value is equal."""
         if isinstance(other, McParameter):
             return (self.name == other.name) and (self.value == other.value)
 
         return NotImplemented
 
+    def __add__(self, other):
+        """Allows creation of a Collection by adding two parameters"""
+        if isinstance(other, McParameter):
+            mc_return = McParameterCollection()
+            mc_return.add(self)
+            mc_return.add(other)
+
+            return mc_return
+        else:
+            return NotImplemented
+
 
 class McParameterCollection(object):
     """
     This parameter collection has properties which as a single parameter. This way a group of parameters and a single parameter can be treated equally.
 
     Attributes
     ----------
@@ -636,15 +656,19 @@
             try:
                 __McParameterCollection__ = VersionInfo.parse(__McParameterCollection__)  # type: ignore
             except TypeError:
                 __McParameterCollection__ = VersionInfo.parse(
                     f"{__McParameterCollection__:1.1f}.0"
                 )  # if it is a number only MAJOR.MINOR is used
 
-        if __McParameterCollection__ != SEMVER_MCPARAMETER_Collection_CURRENT:
+        if __McParameterCollection__ == VersionInfo(major=1, minor=0):
+            # trun around possible groups..
+            if possible_groups is not None:
+                possible_groups = dict([(key, item) for item, key in possible_groups.items()])
+        elif __McParameterCollection__ != SEMVER_MCPARAMETER_Collection_CURRENT:
             raise NotImplementedError(
                 "DMT->McParameterCollection: Unknown version of collection to create!"
             )
 
         self._paras: list[McParameter] = list()
         self._values: OrderedDict[str, Union[float, int]] = OrderedDict()
 
@@ -814,15 +838,16 @@
                     collection.set(McParameter.load_json(**dict_content), update=False)
 
         collection.update_values()
 
         return collection
 
     def get(
-        self, parameters: Union[str, McParameter, list[str], tuple[str], McParameterCollection]
+        self,
+        parameters: Union[str, McParameter, list[str], tuple[str], McParameterCollection],
     ) -> Union[McParameter, McParameterCollection]:
         """Returns a McParameterCollection with copies of all given parameter names.
 
         Parameters
         ----------
         parameters  : str, iterable(str) or McParameterCollection
 
@@ -1235,15 +1260,16 @@
             ) as data_table:  # pylatex does not count s S columns from siunitx
                 data_table.add_hline()
                 data_table.add_row(["parameter", NoEscape("{value}")])
                 data_table.add_hline()
                 data_table.end_table_header()
                 data_table.add_hline()
                 data_table.add_row(
-                    (MultiColumn(2, align="r", data="continued on next Page"),), strict=False
+                    (MultiColumn(2, align="r", data="continued on next Page"),),
+                    strict=False,
                 )
                 data_table.add_hline()
                 data_table.end_table_footer()
                 data_table.add_hline()
                 data_table.add_row((MultiColumn(2, align="r", data="Finish"),), strict=False)
                 data_table.add_hline()
                 data_table.end_table_last_footer()
@@ -1252,37 +1278,39 @@
                 for para in sorted(clean_mcard, key=lambda x: (x.group, x.name)):
                     if group != para.group:
                         if group is not None:
                             data_table.add_hline()  # horizontal line after each group and then the next group name
 
                         group = para.group
                         try:
-                            group_desc = next(
-                                description
-                                for description, group_a in self.possible_groups.items()
-                                if group_a == group
-                            )
+                            # group_desc = next(
+                            #     description
+                            #     for description, group_a in self.possible_groups.items()
+                            #     if group_a == group
+                            # )
+                            group_desc = self.possible_groups[group]
                             data_table.add_row(
-                                (MultiColumn(2, align="l", data=group_desc),), strict=False
+                                (MultiColumn(2, align="l", data=group_desc),),
+                                strict=False,
                             )
-                        except StopIteration:
+                        except KeyError:
                             pass
 
                     if para.unit.dimensionless:
                         data_table.add_row(
                             [
                                 NoEscape(f"{para:<12s}"),
                                 NoEscape(f"{para:g}"),
                             ],
                             strict=False,
                         )
                     else:
                         data_table.add_row(
                             [
-                                NoEscape(f"{para:<12s}/\si{{{para:u}}}"),
+                                NoEscape(f"{para:<12s}/\\si{{{para:u}}}"),
                                 NoEscape(f"{para:g}"),
                             ],
                             strict=False,
                         )
 
         return doc
 
@@ -1351,15 +1379,15 @@
             mc_return = copy.deepcopy(self)
             mc_return.add(other, index=0)  # insert at start
 
             return mc_return
         else:
             return NotImplemented
 
-    def eq_paras(self, other):
+    def eq_paras(self, other, to_terminal=False):
         """Compares the parameters in two McParameterCollections or subclasses"""
         str_diff_vars = ""
         for para in self.paras:
             try:
                 if para.value != other.get(para.name).value:
                     str_diff_vars += f"{para:<12s}: {para:10.4e} || {other.get(para):10.4e}\n"
             except KeyError:
@@ -1367,19 +1395,37 @@
 
         # find parameters in other which are not in self!
         for para in other:
             if para.name not in self.name:
                 str_diff_vars += f"The first modelcard does not have a {para:s} parameter!\n"
 
         if str_diff_vars:
+            if to_terminal:
+                print(str_diff_vars)
+            str_diff_vars = (
+                "Comparision between 2 modelcards resultet in False. The difference is:\n"
+                + str_diff_vars
+            )
             logging.info(str_diff_vars)
             return False
 
         return True
 
     def __eq__(self, other):
         """Allows comparing 2 model cards using mc1 == mc2"""
         if isinstance(other, McParameterCollection):
             # can only compare to other collections
             return self.eq_paras(other)
 
         return NotImplemented
+
+    def get_circuit(self, use_build_in=False, topology=None, **kwargs) -> Circuit:
+        """Here the modelcard defines it's default simulation circuit.
+
+        Parameters
+        ----------
+        use_build_in : {False, True}, optional
+            Creates a circtui the modelcard using the build-in model
+        topology : optional
+            If a model has multiple standard circuits, use the topology to differentiate between them..
+        """
+        raise NotImplementedError("The superclass McParameterCollection has no circuit :(.")
```

### Comparing `DMT_core-2.0.0/DMT/core/mc_skywater.py` & `DMT_core-2.1.0/DMT/core/mc_skywater.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """ Skywater modelcard
 
 Author: Mario Krattenmacher | Mario.Krattenmacher@semimod.de
 """
+
 # DMT
 # Copyright (C) from 2022  SemiMod
 # <https://gitlab.com/dmt-development/dmt-device>
 #
 # This file is part of DMT_core.
 #
 # DMT_other is free software for non-commercial use only. DMT_other is licensed
@@ -31,15 +32,15 @@
 SEMVER_MCSKYWATER_CURRENT = VersionInfo(major=1, minor=0)
 
 
 class McSkywater(MCard):
     """All model parameters of Skywater130 pdk models
 
     Parameters
-    -----------
+    ----------
     load_model_from_path : str, optional
         Initialise the modelcard with the parameter from the given file path.
     version : float, optional
         Version of the model card. Default is 1.0
     pdk_path : str
         Path to the Skywater pdk: ".../sky130.lib.spice"
     pdk_corner : str
@@ -56,17 +57,15 @@
         default_subckt_name="X1",
         default_module_name="sky130_fd_pr__nfet",
         possible_groups=None,
         vae_module=None,
         **kwargs,
     ):
         if possible_groups is None:
-            possible_groups = {
-                "Geometrie": "geo",
-            }
+            possible_groups = {"geo": "Geometrie"}
 
         super().__init__(
             nodes_list,
             default_subckt_name,
             default_module_name,
             version=version,
             possible_groups=possible_groups,
@@ -117,15 +116,15 @@
 
         return info_dict
 
     def get_circuit(self, use_build_in=False, topology=None, **kwargs) -> Circuit:
         """Here the modelcard defines it's default simulation circuit.
 
         Parameters
-        -----------
+        ----------
         use_build_in : {False, True}, optional
             Creates a circuit for the modelcard using the build-in model
         topology : optional
             If a model has multiple standard circuits, use the topology to differentiate between them..
         """
         if use_build_in:
             mcard = self.get_build_in()
```

### Comparing `DMT_core-2.0.0/DMT/core/mcard.py` & `DMT_core-2.1.0/DMT/core/mcard.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """ Base class to handle verilog-a modelcards.
 
 Author: Mario Krattenmacher | Mario.Krattenmacher@semimod.de
 Author: Markus Müller       | Markus.Mueller3@tu-dresden.de
 """
+
 # DMT_core
 # Copyright (C) from 2022  SemiMod
 # Copyright (C) until 2021  Markus Müller, Mario Krattenmacher and Pascal Kuthe
 # <https://gitlab.com/dmt-development/dmt-core>
 #
 # This file is part of DMT_core.
 #
@@ -29,25 +30,28 @@
 import pickle
 import logging
 import scipy.io as sciio
 import ast
 import operator
 import warnings
 from pathlib import Path
-from typing import Union, Optional
+from typing import Union, Optional, TYPE_CHECKING
 from types import ModuleType
 
 try:
     from semver.version import Version as VersionInfo
 except ImportError:
     from semver import VersionInfo
 
 import verilogae
 
 from DMT.core import unit_registry, VAFileMap
+
+if TYPE_CHECKING:
+    from DMT.core.circuit import Circuit
 from DMT.core.mc_parameter import McParameterCollection, McParameter
 
 
 unit_converter = {
     "s": unit_registry.second,
     "sec": unit_registry.second,
     "A": unit_registry.ampere,
@@ -261,15 +265,17 @@
         -------
         VAFileMap
 
         """
         return self._va_codes
 
     def set_va_codes(
-        self, path_to_main_code: Union[os.PathLike, str], version: Union[str, float] = None
+        self,
+        path_to_main_code: Union[os.PathLike, str],
+        version: Union[str, float] = None,
     ):
         """Sets self._va_codes by extracting all included files from the main file down the include tree.
 
         Parameters
         ----------
         path_to_main_code : Union[os.PathLike, str]
             Relative or Absolute path to the main Verilog-AMS file
@@ -315,31 +321,34 @@
         Parameters
         ----------
         remove_old_parameters : bool, optional
             Deletes parameters which are not part of the VA-Code, by default False
         """
         vae_module = self.get_verilogae_model()
         paras_new = []
+        # missing_groups = []
         # Updated parameter properties
         for para_name, para_properties in vae_module.modelcard.items():
             para_name = para_name.lower()
             try:
                 # para = next(para for para in self._paras if para.name == para_name)
                 para = self.get(para_name)
                 self.remove(para_name)
                 ty = type(para_properties.default)
                 para.val_type = ty  # type: ignore
 
                 if para.min > para_properties.min:
                     para.min = para_properties.min
-                    para.inc_min = para_properties.min_inclusive  # type: ignore
+
+                para.inc_min = para_properties.min_inclusive  # type: ignore
 
                 if para.max < para_properties.max:
                     para.max = para_properties.max
-                    para.inc_max = para_properties.max_inclusive  # type: ignore
+
+                para.inc_max = para_properties.max_inclusive  # type: ignore
 
                 para.unit = unit_converter[para_properties.unit]  # type: ignore
                 para.description = para_properties.description  # type: ignore
                 para.group = para_properties.group  # type: ignore
             except KeyError:
                 para = McParameter(
                     para_name,
@@ -350,16 +359,32 @@
                     inc_min=para_properties.min_inclusive,
                     inc_max=para_properties.max_inclusive,
                     exclude=None,  # ? really needed
                     group=para_properties.group,
                     unit=unit_converter[para_properties.unit],
                     description=para_properties.description,
                 )
+
+            # if para.group not in self.possible_groups:
+            #     warnings.warn(
+            #         f"DMT->MCard: The parameter group {para.group} is not part of this modelcards possible groups.\nThis parameter group was given in the parameter {para.name}",
+            #         category=RuntimeWarning,
+            #     )
+            #     missing_groups.append(para.group)
+            #     self.possible_groups[para.group] = ""
             paras_new.append(para)
 
+        # if missing_groups:
+        #     missing_groups_dict_str = '":,\n"'.join(missing_groups)
+        #     warnings.warn(
+        #         f'DMT->MCard: Full list of missing groups to copy into a dict:\n"{missing_groups_dict_str}":,\n'
+        #         category=RuntimeWarning,
+        #         stacklevel=
+        #     )
+
         if remove_old_parameters:
             self._paras = []  # remove the old parameters fast...
 
         for para in paras_new:
             self.add(para, update=False)
 
         self.update_values()
@@ -423,15 +448,15 @@
         -------
         MCard
             Loaded modelcard
         """
 
         return super().load_json(file_path, directory_va_file=directory_va_file, ignore_checksum=ignore_checksum)  # type: ignore
 
-    def get_circuit(self, use_build_in=False, topology=None, **kwargs):
+    def get_circuit(self, use_build_in=False, topology=None, **kwargs) -> Circuit:
         """Here the modelcard defines it's default simulation circuit.
 
         Parameters
         ----------
         use_build_in : {False, True}, optional
             Creates a circtui the modelcard using the build-in model
         topology : optional
@@ -441,15 +466,20 @@
         raise NotImplementedError("The default modelcard has no circuit :(.")
 
     def get_build_in(self):
         """Return the parameters embedded in a build-in model (no Va code and correct module name etc)"""
         raise NotImplementedError("The submodels have to implement the build-in parameters")
 
     def print_to_file(
-        self, path_to_file, file_mode="w", subckt_name=None, module_name=None, line_break="\n"
+        self,
+        path_to_file,
+        file_mode="w",
+        subckt_name=None,
+        module_name=None,
+        line_break="\n",
     ):
         """Generates a spectre .lib file which can be included into an netlist.
 
         Existence of lib file is not checked before writing!
         Name of File: path_to_file + ".lib"
 
         Parameters
@@ -522,15 +552,18 @@
             path_to_file = Path(path_to_file)
 
         modcard = None
 
         # Loading protocol depends on file ending
         file_ending = path_to_file.suffix
         if file_ending == ".mcp" or file_ending == ".mcard":
-            logging.info("Loading model parameters from pickled model card: %s", str(path_to_file))
+            logging.info(
+                "Loading model parameters from pickled model card: %s",
+                str(path_to_file),
+            )
 
             with path_to_file.open("rb") as myfile:
                 modcard = pickle.load(myfile)
 
         elif file_ending == ".mat":
             logging.info("Loading model parameters from mat-File: %s", str(path_to_file))
 
@@ -549,15 +582,18 @@
             # split it
             re_object = re.findall(r"[a-zA-Z0-9]+\s*=\s*\S+", str_modelcard)
 
             for param_value in re_object:
                 param_value = param_value.split("=")
                 modcard.append((param_value[0].strip(), float(param_value[1].strip())))
         elif file_ending == ".lib" or file_ending == "":
-            logging.info("Loading model parameters from a TRADICA lib-File: %s", str(path_to_file))
+            logging.info(
+                "Loading model parameters from a TRADICA lib-File: %s",
+                str(path_to_file),
+            )
 
             modcard = []
             str_lib = path_to_file.read_text()
 
             # get the model part
             search_parameters = re.search(
                 r"(model|subckt)(.*)(ends|)", str_lib, flags=re.DOTALL | re.IGNORECASE
```

### Comparing `DMT_core-2.0.0/DMT/core/naming.py` & `DMT_core-2.1.0/DMT/core/naming.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 r""" Global namings for DMT
 
 Internally all variables and column names which contain a quantity of a specifier must have the same given names, e.g. all voltages will be called: 'V\_'
 """
+
 # DMT_core
 # Copyright (C) from 2022  SemiMod
 # Copyright (C) until 2021  Markus Müller, Mario Krattenmacher and Pascal Kuthe
 # <https://gitlab.com/dmt-development/dmt-core>
 #
 # This file is part of DMT_core.
 #
@@ -55,14 +56,15 @@
     "F": {
         1: r"\volt\per\meter",
         1e-5: r"\kilo\volt\per\centi\meter",
     },  # field
 }
 UNIT_PREFIX_DENOMINATOR = {
     1e-6: r"\centi",
+    1: "",
 }
 
 
 class SpecifierStr(str):
     """Acts like a string, but at the same time has the attribute "nodes"
 
     https://stackoverflow.com/a/2673863
@@ -91,14 +93,15 @@
     def __new__(
         cls,
         specifier: Union[str, SpecifierStr],
         *nodes: str,
         sub_specifiers: Union[
             FrozenSet[Union[str, SpecifierStr]],
             Set[Union[str, SpecifierStr]],
+            List[Union[str, SpecifierStr]],
             str,
             SpecifierStr,
             None,
         ] = None,
     ):
         if not nodes and sub_specifiers is None:
             try:
@@ -274,15 +277,16 @@
             unit = siunitx_format_unit(
                 unit._units, unit_registry
             )  # new version has other interface
         # for non-mixed quantities like voltages and current
         if self.specifier in UNIT_PREFIX_MIX:  # mixed unit
             unit_with_prefix = UNIT_PREFIX_MIX[self.specifier][np.round(scale, decimals=10)]
 
-            return f"${self.to_tex(**kwargs):s}=\\SI{{{value * scale:.{decimals}f}}}{{{unit_with_prefix:s}{unit:s}}}$"
+            # return f"${self.to_tex(**kwargs):s}=\\SI{{{value * scale:.{decimals}f}}}{{{unit_with_prefix:s}{unit:s}}}$"
+            return f"${self.to_tex(**kwargs):s}=\\SI{{{value * scale:.{decimals}f}}}{{{unit_with_prefix:s}}}$"
 
         else:
             unit_prefix = UNIT_PREFIX[scale]
 
             return f"${self.to_tex(**kwargs):s}=\\SI{{{value * scale:.{decimals}f}}}{{{unit_prefix:s}{unit:s}}}$"
 
     def to_raw_string(self) -> str:
@@ -320,15 +324,16 @@
             except IndexError:
                 sub_specifiers = None
             return SpecifierStr(spec, *nodes, sub_specifiers=sub_specifiers)
         else:  # it was just a regular str
             return string
 
     def __add__(
-        self: SpecifierStr, other: Union[SpecifierStr, str, list[Union[str, SpecifierStr]]]
+        self: SpecifierStr,
+        other: Union[SpecifierStr, str, list[Union[str, SpecifierStr]]],
     ) -> SpecifierStr:
         """Method stub"""
         raise NotImplementedError
 
     def __radd__(self, other):
         # if isinstance(other, SpecifierStr): # not needed since __add__ is taking care of this!
         if isinstance(other, str):  # reflected str + SpecifierStr
@@ -492,14 +497,16 @@
     WIDTH = SpecifierStr("", sub_specifiers="WIDTH")
     CORNER = SpecifierStr("", sub_specifiers="CORNER")
     FORCED = SpecifierStr("", sub_specifiers="FORCED")
     AC_BASE = SpecifierStr("", sub_specifiers="AC_BASE")
     AC_COLLECTOR = SpecifierStr("", sub_specifiers="AC_COLLECTOR")
     AC_GATE = SpecifierStr("", sub_specifiers="AC_GATE")
     AC_DRAIN = SpecifierStr("", sub_specifiers="AC_DRAIN")
+    AC_1 = SpecifierStr("", sub_specifiers="AC_1")
+    AC_2 = SpecifierStr("", sub_specifiers="AC_2")
     AC = SpecifierStr("", sub_specifiers="AC")
     REAL = SpecifierStr("", sub_specifiers="REAL")
     IMAG = SpecifierStr("", sub_specifiers="IMAG")
     MAG = SpecifierStr("", sub_specifiers="MAG")
     PHASE = SpecifierStr("", sub_specifiers="PHASE")
     DELTA = SpecifierStr("", sub_specifiers="DELTA")
     NOISE = SpecifierStr("", sub_specifiers="NOISE")
@@ -558,14 +565,15 @@
     QUASI_FERMI_POTENTIAL = SpecifierStr("PHI")
     ELECTRICAL_POTENTIAL = SpecifierStr("PSI")
     MOBILITY = SpecifierStr("MU")
     X = SpecifierStr("x")
     Y = SpecifierStr("y")
     Z = SpecifierStr("z")
     ENERGY = SpecifierStr("E")
+    NOISE = SpecifierStr("N")
 
     # only derived quantities here
     DC_CURRENT_AMPLIFICATION = SpecifierStr("BETA")
     TRANSCONDUCTANCE = SpecifierStr("GM")
     OUTPUT_CONDUCTANCE = SpecifierStr("GO")
     TRANSIT_FREQUENCY = SpecifierStr("F_T")
     MAXIMUM_OSCILLATION_FREQUENCY = SpecifierStr("F_MAX")
@@ -644,15 +652,17 @@
             return self
 
         if other[0] == "_" or other[0] == "|":
             other = other[1:]
 
         if other in SUB_SPECIFIERS_STR:
             return SpecifierStr(
-                self.specifier, *self.nodes, sub_specifiers=self.sub_specifiers | {other}
+                self.specifier,
+                *self.nodes,
+                sub_specifiers=self.sub_specifiers | {other},
             )
         else:
             return SpecifierStr(
                 self.specifier, *self.nodes, other, sub_specifiers=self.sub_specifiers
             )  # @Mario we should discuss this
 
     elif isinstance(other, (list, set, frozenset)):
@@ -691,14 +701,15 @@
     specifiers.MAXIMUM_OSCILLATION_FREQUENCY: unit_registry.hertz,
     specifiers.TRANSIT_TIME: unit_registry.second,
     specifiers.TRANSCONDUCTANCE: unit_registry.siemens,
     specifiers.ENERGY: unit_registry.volt,
     specifiers.FIELD: unit_registry.volt / unit_registry.meter,
     specifiers.DC_CURRENT_AMPLIFICATION: unit_registry.dimensionless,
     specifiers.MAXIMUM_STABLE_GAIN: unit_registry.dimensionless,
+    specifiers.OUTPUT_CONDUCTANCE: unit_registry.siemens,
     specifiers.NET_DOPING: 1 / unit_registry.meter / unit_registry.meter / unit_registry.meter,
     specifiers.ACCEPTORS: 1 / unit_registry.meter / unit_registry.meter / unit_registry.meter,
     specifiers.DONNORS: 1 / unit_registry.meter / unit_registry.meter / unit_registry.meter,
     specifiers.ELECTRONS: 1 / unit_registry.meter / unit_registry.meter / unit_registry.meter,
     specifiers.HOLES: 1 / unit_registry.meter / unit_registry.meter / unit_registry.meter,
 }  # type: dict[SpecifierStr, Unit]
 
@@ -1038,23 +1049,25 @@
     specifiers.VOLTAGE: 1,
     specifiers.MAXIMUM_STABLE_GAIN: 1,
     specifiers.CURRENT: 1e3,  # mA
     specifiers.CURRENT_DENSITY: 1e3 / (1e6 * 1e6),  # mA/um^2
     specifiers.MAXIMUM_OSCILLATION_FREQUENCY: 1e-9,
     specifiers.TRANSCONDUCTANCE: 1,
     specifiers.OUTPUT_CONDUCTANCE: 1,
-    specifiers.TRANSIT_FREQUENCY: 1e-9,
+    specifiers.TRANSIT_FREQUENCY: 1e-9,  # GHz
+    specifiers.TRANSIT_TIME: 1e12,  # ps
     specifiers.CAPACITANCE: 1e15,
     specifiers.CHARGE: 1e15,
     specifiers.CHARGE_DENSITY: 1e15 / (1e6 * 1e6),  # fF/um^2
     specifiers.SS_PARA_Y: 1e3,
     specifiers.DC_CURRENT_AMPLIFICATION: 1,
     specifiers.FREQUENCY: 1e-9,  # GHz
     specifiers.TEMPERATURE: 1,
     specifiers.X: 1e9,
     specifiers.POWER: 1e3,  # mW
     specifiers.RESISTANCE: 1,  # Ohm
     specifiers.CONDUCTANCE: 1,  # Siemens
     specifiers.ENERGY: 1,  # eV
     specifiers.UNILATERAL_GAIN: 1,
     specifiers.NET_DOPING: 1e-6,  # 1/cm^3
+    specifiers.NOISE: 1,
 }
```

### Comparing `DMT_core-2.0.0/DMT/core/plot.py` & `DMT_core-2.1.0/DMT/core/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """ Wrapper for nice plots with tikz, pyqtgraph and matplotlib.
 
 Author:
     Mario Krattenmacher | Mario.Krattenmacher@semimod.de
     Markus Mueller | Markus.Mueller3@tu-dresden.de
 """
+
 # DMT_core
 # Copyright (C) from 2022  SemiMod
 # Copyright (C) until 2021  Markus Müller, Mario Krattenmacher and Pascal Kuthe
 # <https://gitlab.com/dmt-development/dmt-core>
 #
 # This file is part of DMT_core.
 #
@@ -28,15 +29,22 @@
 import re
 from typing import Union
 import numpy as np
 from pathlib import Path
 from cycler import cycler
 from colormath.color_objects import sRGBColor
 from DMT.core import natural_scales, sub_specifiers
-from DMT.external import tex_to_text, build_tex, build_svg, clean_tex_files, build_png, slugify
+from DMT.external import (
+    tex_to_text,
+    build_tex,
+    build_svg,
+    clean_tex_files,
+    build_png,
+    slugify,
+)
 
 # if "PYQTGRAPH_QT_LIB" not in os.environ:
 #     # user did not choose Backend. Try to force PySide6 (best tested)
 #     try:
 #         import PySide6
 #     except ImportError:
 #         try:
@@ -50,15 +58,15 @@
 
     if hasattr(pyqtgraph, "QtWidgets"):
         pyqt_widgets = pyqtgraph.QtWidgets
     else:
         pyqt_widgets = pyqtgraph.Qt.QtGui
 
 except ImportError:
-    print(f"DMT->Plot: Failed to import plotting module pyqtgraph.")
+    print("DMT->Plot: Failed to import plotting module pyqtgraph.")
 
 try:
     import matplotlib
     import matplotlib.pyplot as plt
     import matplotlib._pylab_helpers
     import matplotlib.ticker as ticker
 
@@ -69,16 +77,16 @@
         "\\usepackage{amsmath}\n",
         "\\usepackage{mathtools}\n",
         "\\usepackage{amssymb}\n",
         "\\usepackage{siunitx}\n",
         "\\sisetup{range-units=repeat, list-units=repeat, binary-units, exponent-product = \\cdot, print-unity-mantissa=false}\n",
         "\\DeclareSIUnit\\sq{\\ensuremath{\\Box}}\n",
         "\\DeclareSIUnit\\degC{\\degreeCelsius}\n",
-        "\\DeclareUnicodeCharacter{221E}{$\infty$}\n",
-        "\\DeclareUnicodeCharacter{03A9}{$\Omega$}\n",
+        "\\DeclareUnicodeCharacter{221E}{$\\infty$}\n",
+        "\\DeclareUnicodeCharacter{03A9}{$\\Omega$}\n",
     ]
     packages_to_add = []
     str_user_packages = "".join(matplotlib.rcParams["text.latex.preamble"])
     for package in packages:
         if package not in str_user_packages:
             packages_to_add.append(package)
 
@@ -129,30 +137,32 @@
 XTRACTION_INTERPOLATED = "xtraction_interpolated"
 PLOT_STYLES.append(XTRACTION_INTERPOLATED)
 XTRACTION_INTERPOLATED_COLOR = "xtraction_interpolated_color"
 PLOT_STYLES.append(XTRACTION_INTERPOLATED_COLOR)
 MIX = "mix"
 PLOT_STYLES.append(MIX)
 
-CYCLER_MARKERS = cycler(marker=[char for char in "x+v^*<>.so"])
-CYCLER_LINESTYLES = cycler(linestyle=["-", "--", "-.", ":"])
-CYCLER_COLORS = cycler(
-    color=[
-        "#006400",  # darkgreen
-        "#00008b",  # darkblue
-        "#b03060",  # maroon3
-        "#ff0000",  # red
-        "#9467bd",  # yellow -> replaced by violett/brown combo
-        "#deb887",  # curlywood
-        "#00ff00",  # lime
-        "#00ffff",  # aqua
-        "#ff00ff",  # fuchsia
-        "#6495ed",  # cornflower
-    ]
-)
+MARKERS = [char for char in "x+v^*<>.so"]
+LINESTYLES = ["-", "--", "-.", ":"]
+COLORS = [
+    "#006400",  # darkgreen
+    "#00008b",  # darkblue
+    "#b03060",  # maroon3
+    "#ff0000",  # red
+    "#9467bd",  # yellow -> replaced by violett/brown combo
+    "#deb887",  # curlywood
+    "#00ff00",  # lime
+    "#00ffff",  # aqua
+    "#ff00ff",  # fuchsia
+    "#6495ed",  # cornflower
+]
+
+CYCLER_MARKERS = cycler(marker=MARKERS)
+CYCLER_LINESTYLES = cycler(linestyle=LINESTYLES)
+CYCLER_COLORS = cycler(color=COLORS)
 
 
 ### Translation dictionaries from matplotlib to tikz
 _DICT_MARKERS_MPL_TO_PGF = {
     ".": r"mark=*, mark options={solid, fill}, ",
     # ',',# do not know how to translate them ...
     "o": r"mark=o, mark options={solid, fill}, ",
@@ -179,15 +189,15 @@
     None: r" ",
 }
 _DICT_LINES_MPL_TO_PGF = {
     " ": "only marks, ",
     "--": "dashed, ",
     "-.": "dashdotted, ",
     "-": "solid, ",
-    ".": "dotted, ",
+    # ".": "dotted, ", # is used as a MARKER!
     ":": "dotted, ",  # or densely dotted ??
 }
 _DICT_COLORS_MPL = {
     "b": "blue",
     "g": "green",
     "r": "red",
     "c": "cyan",
@@ -231,14 +241,15 @@
         x_scale=None,
         y_scale=None,
         x_log=False,
         y_log=False,
         legend_location="upper right",
         num=None,
         divide_by_unit=False,
+        caption=None,
     ):
         """
         Parameters
         ----------
         plot_name : str
             Name of the plot object, also used for captions and saving the object.
         style : str, optional
@@ -357,14 +368,16 @@
             self.x_axis_scale = "linear"
 
         if y_log:
             self.y_axis_scale = "log"
         else:
             self.y_axis_scale = "linear"
 
+        self.caption = caption
+
     def set_x_label(self, x_label=None, x_specifier=None, x_scale=None):
         """Set the x label. Either using directly a string or a specifier.
 
         Parameters
         ----------
         x_label : str
         x_specifier : SpecifierStr
@@ -442,40 +455,17 @@
         Parameters
         ----------
         style : str
             Style for plotting of the lines. Possible are:
             'color', 'bw', 'markers_color', 'markers', 'markers_lines',
             'xtraction', 'xtraction_color', 'xtraction_interpolated', 'xtraction_interpolated_color',
         """
-        markers = [char for char in "x+v^*<>.so"]
-        linestyles = ["-", "--", "-.", ":"]
-        # MM: replaced grey1 (#7f7f7f) with black(#) and grey2 with dark blue #1012d5. Does this cause problems?
-        # MK: introduced completely new palette from https://mokole.com/palette.html (settings: 10 colors, 1% min, 80% max, 15000 loops, score 65.49)
-        colors = [
-            # "#1f77b4",
-            # "#ff7f0e",
-            # "#2ca02c",
-            # "#d62728",
-            # "#9467bd",
-            # "#e377c2",
-            # "#8c564b",
-            # "#0e1111",
-            # "#1012d5",
-            # "#17becf",
-            "#006400",  # darkgreen
-            "#00008b",  # darkblue
-            "#b03060",  # maroon3
-            "#ff0000",  # red
-            "#9467bd",  # yellow -> replaced by violett/brown combo
-            "#deb887",  # curlywood
-            "#00ff00",  # lime
-            "#00ffff",  # aqua
-            "#ff00ff",  # fuchsia
-            "#6495ed",  # cornflower
-        ]
+        markers = MARKERS
+        linestyles = LINESTYLES
+        colors = COLORS
 
         if style == BLACK_WHITE:
             self._cycler = (
                 cycler("color", ["black"]) * cycler("linestyle", "-") * cycler("marker", markers)
             )
 
         elif style == BLACK_SOLID:
@@ -648,23 +638,25 @@
         elif style == COMPARISON_4:
             # find the limiting style component in terms of numbers
             n_styles = np.argmin([int(len(markers) / 2), len(colors)])
             n_styles = [int(len(markers) / 2), len(colors)][n_styles]
 
             xtraction_markers = []
             for i, marker in enumerate(markers[:n_styles]):
-                xtraction_markers.append(None)
                 xtraction_markers.append(marker)
                 xtraction_markers.append(None)
-                xtraction_markers.append(markers[i + 1])
+                xtraction_markers.append(None)
+                xtraction_markers.append(None)
+
+                # xtraction_markers.append(markers[i + 1])
 
             xtraction_lstyle = []
             for marker in markers[:n_styles]:
-                xtraction_lstyle.append("-")
                 xtraction_lstyle.append("")
+                xtraction_lstyle.append("-")
                 xtraction_lstyle.append("--")
                 xtraction_lstyle.append("-.")
 
             colors2 = []
             for color in colors[:n_styles]:
                 colors2.append(color)
                 colors2.append(color)
@@ -902,27 +894,33 @@
                         + self.name
                         + " for line with label "
                         + str(label)
                     ) from err
             else:
                 try:
                     (line,) = self.ax.plot(
-                        x * self.x_scale, y * self.y_scale, label=label, **dict_line["kwargs"]
+                        x * self.x_scale,
+                        y * self.y_scale,
+                        label=label,
+                        **dict_line["kwargs"],
                     )
                 except ValueError as err:
                     raise ValueError(
                         "Too many values to unpack in plot "
                         + self.name
                         + " for line with label "
                         + str(label)
                     ) from err
             # self.lines.append(line)
 
         # labels and legend
-        if self.legend_location in ["upper right outer", "right mid"]:  # not supported here
+        if self.legend_location in [
+            "upper right outer",
+            "right mid",
+        ]:  # not supported here
             self.ax.legend(loc="upper right", frameon=self.legend_frame)
         else:
             self.ax.legend(loc=self.legend_location, frameon=self.legend_frame)
 
         if use_tex:
             self.ax.set_xlabel(self.x_label)
             self.ax.set_ylabel(self.y_label)
@@ -1026,17 +1024,30 @@
         y_label = tex_to_text(y_label)
 
         # labels and legend
         self.pw_pg.setLabel("bottom", x_label)
         self.pw_pg.setLabel("left", y_label)
         legend = self.pw_pg.addLegend()  # loc=self.legend_location, frameon=self.legend_frame)
         legend_pos = {  # not sure if correct
-            "upper right": {"itemPos": (1, 0), "parentPos": (1, 0), "offset": (-10, 10)},
+            "upper right": {
+                "itemPos": (1, 0),
+                "parentPos": (1, 0),
+                "offset": (-10, 10),
+            },
+            "upper right outer": {
+                "itemPos": (1, 0),
+                "parentPos": (1, 0),
+                "offset": (-10, 10),
+            },
             "upper left": {"itemPos": (0, 0), "parentPos": (0, 0), "offset": (10, 10)},
-            "lower right": {"itemPos": (1, 1), "parentPos": (1, 1), "offset": (-10, -10)},
+            "lower right": {
+                "itemPos": (1, 1),
+                "parentPos": (1, 1),
+                "offset": (-10, -10),
+            },
             "lower left": {"itemPos": (0, 1), "parentPos": (0, 1), "offset": (10, -10)},
             None: {"itemPos": (0, 0), "parentPos": (0, 0), "offset": (10, 10)},
         }
         legend.anchor(**legend_pos[self.legend_location])
 
         # actual plotting of the data
         for i_line, dict_line in enumerate(self.data):
@@ -1095,69 +1106,60 @@
                 x_min = np.nanmin(
                     [
                         np.nanmin(dict_line["x"])
                         for dict_line in self.data
                         if not len(dict_line["x"]) == 0
                     ]
                 )
-                x_min = 0.95 * x_min if x_min > 0 else 1.05 * x_min
-                x_min_set = x_min * self.x_scale
+                x_min = 0.95 * x_min * self.x_scale if x_min > 0 else 1.05 * x_min * self.x_scale
             else:
                 x_min = 0
-                x_min_set = x_min
         else:
             x_min = self.x_limits[0]
-            x_min_set = x_min
             padding = 0.0
 
         if self.x_limits[1] is None:
             if self.data:  # fails for empty plots
                 x_max = np.nanmax(
                     [
                         np.nanmax(dict_line["x"])
                         for dict_line in self.data
                         if not len(dict_line["x"]) == 0
                     ]
                 )
-                x_max = 1.05 * x_max if x_max > 0 else 0.95 * x_max
+                x_max = 1.05 * x_max * self.x_scale if x_max > 0 else 0.95 * x_max * self.x_scale
                 # x_max = np.ceil(1.1*x_max) if x_max > 0 else np.ceil(0.9*x_max)
-                x_max_set = x_max * self.x_scale
             else:
-                x_max = 1
-                x_max_set = x_max
+                x_max = self.x_scale * 10
         else:
             x_max = self.x_limits[1]
-            x_max_set = x_max
             padding = 0.0
 
-        if self.x_axis_scale == "log":
-            # also doing this in case of log for the data itself
-            x_min_set = np.log10(np.abs(x_min_set + np.finfo(float).tiny))
-            x_max_set = np.log10(np.abs(x_max_set + np.finfo(float).tiny))
-
         try:
-            self.pw_pg.setXRange(np.real(x_min_set), np.real(x_max_set), padding=padding)  # type: ignore
+            if self.x_axis_scale == "log":
+                # also doing this in case of log for the data itself
+                self.pw_pg.setXRange(np.real(np.log10(np.abs(x_min + np.finfo(float).tiny))), np.real(np.log10(np.abs(x_max + np.finfo(float).tiny))), padding=padding)  # type: ignore
+            else:
+                self.pw_pg.setXRange(np.real(x_min), np.real(x_max), padding=padding)  # type: ignore
         except Exception:
             print("Error setting the XRange of PyQtGraph plot with name " + self.name + ".")
 
         padding = None
         if self.y_limits[0] is None:
             if self.data:  # fails for empty plots
                 try:
                     y_min = np.inf
                     for dict_line in self.data:
                         y_filter = np.logical_and(
-                            dict_line["x"] > x_min,
-                            dict_line["x"] < x_max,
+                            dict_line["x"] > x_min / self.x_scale,
+                            dict_line["x"] < x_max / self.x_scale,
                         )
                         y_min_local = np.min(dict_line["y"][y_filter])
                         y_min = np.min([y_min, y_min_local])
-                    # y_min = (
-                    #     np.min([np.min(dict_line["y"]) for dict_line in self.data])
-                    # )
+
                     y_min = (
                         0.95 * y_min * self.y_scale if y_min > 0 else 1.05 * y_min * self.y_scale
                     )
                 except ValueError:
                     y_min = 0.0
                 # y_min = np.floor(0.9*y_min) if y_min > 0 else np.floor(1.1*y_min)
             else:
@@ -1168,29 +1170,29 @@
 
         if self.y_limits[1] is None:
             if self.data:  # fails for empty plots
                 try:
                     y_max = -np.inf
                     for dict_line in self.data:
                         y_filter = np.logical_and(
-                            dict_line["x"] > x_min,
-                            dict_line["x"] < x_max,
+                            dict_line["x"] > x_min / self.x_scale,
+                            dict_line["x"] < x_max / self.x_scale,
                         )
                         y_max_local = np.max(dict_line["y"][y_filter])
                         y_max = np.max([y_max, y_max_local])
                     # y_max = (
                     #     np.max([np.max(dict_line["y"]) for dict_line in self.data])
                     # )
                     y_max = (
                         1.05 * y_max * self.y_scale if y_max > 0 else 0.95 * y_max * self.y_scale
                     )
                 except ValueError:
-                    y_max = 1.0
+                    y_max = self.y_scale * 10
             else:
-                y_max = 1.0
+                y_max = self.y_scale * 10
         else:
             y_max = self.y_limits[1]
             padding = 0.0
 
         if self.y_axis_scale == "log":
             # also doing this in case of log for the data itself
             y_min = np.log10(np.abs(y_min + np.finfo(float).tiny))
@@ -1205,26 +1207,32 @@
 
         if self.mw_pg is not None:
             self.mw_pg.show()
 
         ## Start Qt event loop unless running in interactive mode or using pyside.
         if show:
             if sys.flags.interactive != 1 or not hasattr(pyqtgraph.Qt.QtCore, "PYQT_VERSION"):
-                pyqt_widgets.QApplication.exec()  # type: ignore
+                try:
+                    pyqt_widgets.QApplication.exec()  # type: ignore
+                except:
+                    pyqt_widgets.QApplication.exec_()  # type: ignore
 
         if only_widget:
             return self.pw_pg
         elif qt_layout is not None:
             return qt_layout
 
     def show_pyqtgraph(self):
         """Reshows the PyQtGraph main window and startes the Qt event loop"""
         if self.mw_pg is not None:
             self.mw_pg.show()
-            pyqt_widgets.QApplication.exec()  # type: ignore
+            try:
+                pyqt_widgets.QApplication.exec()  # type: ignore
+            except:
+                pyqt_widgets.QApplication.exec_()  # type: ignore
 
     def _convert_mpl_to_pyqt(self, mpl_style):
         """Returns a corresponding PyQtGraph style for a given matplotlib style.
 
         This can be very complicated as PyQtGraph directly uses a QtPen/QtBrush...
 
         Parameters
@@ -1410,22 +1418,21 @@
         clean=False,
         fontsize="normalsize",
         line_width="very thick",
         svg=False,
         png=False,
         extension=None,
         nth=1,
-        mark_delta=1,
-        skip_every=lambda x: x,
         n_ticks_x=None,
         n_ticks_y=None,
         show_legend=True,
         legend_location=None,
         legend_to_name=None,
         legend_columns=4,
+        mark_phase=False,
         **kwargs,
     ):
         """Save plot in directory and return name of the tikz file.
 
         The name of the tikz file will be the figure attribute self.num, if not given.
 
         Parameters
@@ -1506,24 +1513,24 @@
         if standalone:
             str_tikz_picture = (
                 "\\begin{tikzpicture}[font=\\"
                 + fontsize
                 + "]\n"
                 + "\\pgfplotsset{every axis/.append style={"
                 + line_width
-                + "},compat=1.5},\n"
+                + "},compat=1.18},\n"
             )
         else:  # if this figure is used in other tex documents, the axis are trimed so that figures with different y-labels and ticks get displayed nicely
             str_tikz_picture = (
                 "\\begin{tikzpicture}[font=\\"
                 + fontsize
-                + ",trim axis left, trim axis right,tight background]\n"
+                + ", trim axis left, trim axis right, tight background]\n"
                 + "\\pgfplotsset{every axis/.append style={"
                 + line_width
-                + "},compat=1.5},\n"
+                + "},compat=1.18}\n"
             )
         str_height = "" if height is None else "height=" + height + ",\n"
         if width is None:
             str_width = ""
         elif width == "\\textwidth":
             str_width = "width=0.951*\\figurewidth,\n"
         else:
@@ -1560,32 +1567,55 @@
 
             x_axis = self.ax.get_xaxis()
             x_min, x_max = self.ax.get_xlim()
             str_limits += f"xmin={x_min:g},\n"
             str_limits += f"xmax={x_max:g},\n"
 
             if x_axis._scale.name == "linear":
-                x_min_restrict = x_min / 5 if x_min > 0 else x_min * 5
-                x_max_restrict = x_max / 5 if x_max < 0 else x_max * 5
+                if x_min == 0:
+                    x_min_restrict = -1e-20
+                elif x_min > 0:
+                    x_min_restrict = x_min / 5
+                else:
+                    x_min_restrict = x_min * 5
+
+                if x_max == 0:
+                    x_max_restrict = 1e-20
+                elif x_max < 0:
+                    x_max_restrict = x_max / 5
+                else:
+                    x_max_restrict = x_max * 5
+
                 str_limits += comment_restrict + "restrict x to domain={0:g}:{1:g},\n".format(
                     x_min_restrict, x_max_restrict
                 )
             else:
                 str_limits += comment_restrict + "restrict x to domain={0:g}:{1:g},\n".format(
                     np.log10(x_min - 1), np.log10(x_max + 1)
                 )
             str_limits += "log basis x=10,\n"
 
             y_axis = self.ax.get_yaxis()
             y_min, y_max = self.ax.get_ylim()
             str_limits += "ymin={0:g},\n".format(y_min)
             str_limits += "ymax={0:g},\n".format(y_max)
             if y_axis._scale.name == "linear":
-                y_min_restrict = y_min / 5 if y_min > 0 else y_min * 5
-                y_max_restrict = y_max / 5 if y_max < 0 else y_max * 5
+                if y_min == 0:
+                    y_min_restrict = -1e-20
+                elif y_min > 0:
+                    y_min_restrict = y_min / 5
+                else:
+                    y_min_restrict = y_min * 5
+
+                if y_max == 0:
+                    y_max_restrict = 1e-20
+                elif y_max < 0:
+                    y_max_restrict = y_max / 5
+                else:
+                    y_max_restrict = y_max * 5
                 str_limits += comment_restrict + "restrict y to domain={0:g}:{1:g},\n".format(
                     y_min_restrict, y_max_restrict
                 )
             else:
                 str_limits += comment_restrict + "restrict y to domain={0:g}:{1:g},\n".format(
                     np.log10(y_min - 1), np.log10(y_max + 1)
                 )
@@ -1690,96 +1720,95 @@
             )
             str_limits += (
                 "% xmax=0,\n" if self.x_limits[1] is None else f"xmax={self.x_limits[1]:g},\n"
             )
             if self.x_limits[0] is None or self.x_limits[1] is None:
                 str_limits += "% restrict x to domain=0:1,\n"
             else:
-                if self.x_axis_scale == "linear":
-                    x_min_restrict = (
-                        self.x_limits[0] / 5 if self.x_limits[0] > 0 else self.x_limits[0] * 5
-                    )
-                    x_max_restrict = (
-                        self.x_limits[1] / 5 if self.x_limits[1] < 0 else self.x_limits[1] * 5
-                    )
+                if self.x_limits[0] == 0:
+                    x_min_restrict = -1e-20
+                elif self.x_limits[0] > 0:
+                    x_min_restrict = self.x_limits[0] / 5
                 else:
-                    x_min_restrict = (
-                        np.log10(self.x_limits[0] / 5)
-                        if self.x_limits[0] > 0
-                        else np.log10(self.x_limits[0] * 5)
-                    )
-                    x_max_restrict = (
-                        np.log10(self.x_limits[1] / 5)
-                        if self.x_limits[1] < 0
-                        else np.log10(self.x_limits[1] * 5)
-                    )
-                str_limits += comment_restrict + "restrict x to domain={0:g}:{1:g},\n".format(
-                    x_min_restrict, x_max_restrict
-                )
+                    x_min_restrict = self.x_limits[0] * 5
+
+                if self.x_limits[1] == 0:
+                    x_max_restrict = 1e-20
+                elif self.x_limits[1] > 0:
+                    x_max_restrict = self.x_limits[1] * 5
+                else:
+                    x_max_restrict = self.x_limits[1] / 5
+
+                if self.x_axis_scale == "log":
+                    x_min_restrict = np.log10(x_min_restrict)
+                    x_max_restrict = np.log10(x_max_restrict)
+
+                str_limits += f"{comment_restrict}restrict x to domain={x_min_restrict:g}:{x_max_restrict:g},\n"
 
             str_limits += "log basis x=10,\n"
             str_limits += (
                 "% ymin=0,\n" if self.y_limits[0] is None else f"ymin={self.y_limits[0]:g},\n"
             )
             str_limits += (
                 "% ymax=0,\n" if self.y_limits[1] is None else f"ymax={self.y_limits[1]:g},\n"
             )
             if self.y_limits[0] is None or self.y_limits[1] is None:
                 str_limits += "% restrict y to domain=0:1,\n"
             else:
-                if self.y_axis_scale == "linear":
-                    y_min_restrict = (
-                        self.y_limits[0] / 5 if self.y_limits[0] > 0 else self.y_limits[0] * 5
-                    )
-                    y_max_restrict = (
-                        self.y_limits[1] / 5 if self.y_limits[1] < 0 else self.y_limits[1] * 5
-                    )
+                if self.y_limits[0] == 0:
+                    y_min_restrict = -1e-20
+                elif self.y_limits[0] > 0:
+                    y_min_restrict = self.y_limits[0] / 5
                 else:
-                    y_min_restrict = (
-                        np.log10(self.y_limits[0] / 5)
-                        if self.y_limits[0] > 0
-                        else np.log10(self.y_limits[0] * 5)
-                    )
-                    y_max_restrict = (
-                        np.log10(self.y_limits[1] / 5)
-                        if self.y_limits[1] < 0
-                        else np.log10(self.y_limits[1] * 5)
-                    )
-                str_limits += comment_restrict + "restrict y to domain={0:g}:{1:g},\n".format(
-                    y_min_restrict, y_max_restrict
-                )
+                    y_min_restrict = self.y_limits[0] * 5
+
+                if self.y_limits[1] == 0:
+                    y_max_restrict = 1e-20
+                elif self.y_limits[1] > 0:
+                    y_max_restrict = self.y_limits[1] * 5
+                else:
+                    y_max_restrict = self.y_limits[1] / 5
+
+                if self.y_axis_scale == "log":
+                    y_min_restrict = np.log10(y_min_restrict)
+                    y_max_restrict = np.log10(y_max_restrict)
+
+                str_limits += f"{comment_restrict}restrict y to domain={y_min_restrict:g}:{y_max_restrict:g},\n"
+
             str_limits += "log basis y=10,\n"
             print("using pgf")
 
         if legend_to_name is None:
             legend_to_name = ""
         else:
             legend_to_name = "legend to name={},\n".format(legend_to_name)
 
         str_shift_labels = ""
         if fontsize == "normalsize":
-            str_shift_labels = "xlabel shift = -5 pt,\n ylabel shift = -5 pt,\n"
+            str_shift_labels = "xlabel shift=-5pt,\n ylabel shift=-5pt,\n"
 
         ### header
         str_axis = (
-            "\n\\begin{axis}[scale only axis,ytick pos=left,\n"
+            "\n\\begin{axis}[\n"
+            + "scale only axis,\n"
             # + fontsize+",\n"
             + str_width
             + str_height
             + "xlabel={"
             + self.x_label
             + "},\n"
             + "ylabel={"
             + self.y_label
             + "},\n"
             + str_x_log
             + str_y_log
             + str_limits
             + str_x_ticks
             + str_y_ticks
+            + "ytick pos=left,\n"
             + str_shift_labels
             + "xmajorgrids,\n"
             + "enlargelimits=false,\n"
             + "scaled ticks=true,\n"
             + "ymajorgrids,\n"
             + "x tick style={color=black},\n"
             + "y tick style={color=black},\n"
@@ -1797,25 +1826,29 @@
             + legend_to_name
             + "]\n"
         )
 
         ### Lines
         str_lines = ""
         colors = []
-        # try:
-        #     mark_delta = int(mark_repeat/len(self.data[::nth]))
-        # except ZeroDivisionError:
-        #     mark_delta = 1
-        #     print("DMT->plot->{:s}: Plot has no data, generating axis anyways.".format(self.name))
+        bool_mark_phase = mark_phase
+        mark_phase = 0
 
         for nr_line, dict_line in enumerate(self.data[::nth]):
             if len(dict_line["x"]) == 0:
                 continue
+            if bool_mark_phase and mark_repeat != 1:
+                mark_phase = nr_line
+
             str_addplot, colors = self._tikz_addplot(
-                dict_line, nr_line, colors=colors, mark_delta=mark_delta, show_label=show_legend
+                dict_line,
+                nr_line,
+                colors=colors,
+                mark_phase=mark_phase,
+                show_label=show_legend,
             )
             if str_addplot is not None:
                 str_lines += str_addplot
 
         ### footer
         str_footer = "\\end{axis}\n\n\\end{tikzpicture}\n"
 
@@ -1886,20 +1919,22 @@
                 ending_to_keep = ".png"
             else:
                 build_tex(path_file, wait=clean, extension=ext_file)
                 ending_to_keep = ".pdf"
 
             if clean:
                 clean_tex_files(
-                    directory, file_name.replace(ext_file, ""), keep=(ending_to_keep, ".tex")
+                    directory,
+                    file_name.replace(ext_file, ""),
+                    keep=(ending_to_keep, ".tex"),
                 )
 
         return file_name
 
-    def _tikz_addplot(self, dict_line, nr_line, colors=None, mark_delta=None, show_label=True):
+    def _tikz_addplot(self, dict_line, nr_line, colors=None, mark_phase=None, show_label=True):
         """Transforms a line into a pgfplots addplot command.
 
         Parameters
         ----------
         dict_line : (x_data, y_data, label, style)
             See the description in Plot.add_data .
         nr_line : int
@@ -1924,17 +1959,15 @@
 
         if style is None:
             opts_style, colors = self._get_pgfplotset_for_line_nr(nr_line, colors)
         else:
             opts_style, colors = self._convert_mpl_to_pfg(style, colors)
 
         if "mark phase" not in opts_style:
-            # Markus: what was this?
-            # mark_phase = int(nr_line)*mark_delta if (mark_delta is not None) else int(1)
-            opts_style += "mark phase={:d}, ".format(mark_delta)
+            opts_style += "mark phase={:d}, ".format(mark_phase)
 
         if line_width is not None:
             opts_style += "line width={0:f}pt, ".format(line_width)
 
         if mark_size is not None:
             opts_style += "mark size={0:f}pt, ".format(mark_size)
 
@@ -2098,17 +2131,17 @@
         Additional arguments that are passed to the save_tikz routine.
     """
     if len(plts) == 0:
         return
 
     if show:
         for plt in plts[:-1]:
-            plt.plot_py(show=False)
+            plt.plot_pyqtgraph(show=False)
 
-        plts[-1].plot_py(show=True)
+        plts[-1].plot_pyqtgraph(show=True)
     else:
         for plt in plts:
             plt.save_tikz(
                 location,
                 plt.name + "_standalone",
                 clean=True,
                 build=True,
```

### Comparing `DMT_core-2.0.0/DMT/core/plot_2yaxis.py` & `DMT_core-2.1.0/DMT/core/plot_2yaxis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """ Wrapper for plots with 2 y axis. Shows only "left plot" in pyqtgraph and merged in tikz
 
 Author:
     Mario Krattenmacher | Mario.Krattenmacher@semimod.de
     Markus Mueller | Markus.Mueller3@tu-dresden.de
 """
+
 # DMT_core
 # Copyright (C) from 2022  SemiMod
 # Copyright (C) until 2021  Markus Müller, Mario Krattenmacher and Pascal Kuthe
 # <https://gitlab.com/dmt-development/dmt-core>
 #
 # This file is part of DMT_core.
 #
@@ -80,14 +81,18 @@
         self.fig = None
         self.ax_left = None
         self.ax_right = None
 
         # self.lines_left = []
         # self.lines_right = []
 
+    @property
+    def caption(self):
+        return self.plot_left.caption + self.plot_right.caption
+
     def plot_py(
         self,
         show=True,
         font_size=None,
         allowGrid=False,
         tight_layout=True,
         figure_size=None,
```

### Comparing `DMT_core-2.0.0/DMT/core/plot_smith.py` & `DMT_core-2.1.0/DMT/core/plot_smith.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """ Wrapper for nice plots with tikz, pyqtgraph and matplotlib.
 
 Author:
     Mario Krattenmacher | Mario.Krattenmacher@semimod.de
     Markus Mueller | Markus.Mueller3@tu-dresden.de
 """
+
 # DMT_core
 # Copyright (C) from 2022  SemiMod
 # Copyright (C) until 2021  Markus Müller, Mario Krattenmacher and Pascal Kuthe
 # <https://gitlab.com/dmt-development/dmt-core>
 #
 # This file is part of DMT_core.
 #
```

### Comparing `DMT_core-2.0.0/DMT/core/sim_con.py` & `DMT_core-2.1.0/DMT/core/sim_con.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 * Manages all simulations in a unified way, independent of the actual simulation backend.
 * Supports to run simulations on multiple cores in parallel
 * Supports to run simulations on a remote server (including file up- and download)
 
 Author: Mario Krattenmacher | mario.krattenmacher@semimod.de
 Author: Markus Müller | markus.mueller@semimod.de
 """
+
 # DMT_core
 # Copyright (C) from 2022  SemiMod
 # Copyright (C) until 2021  Markus Müller, Mario Krattenmacher and Pascal Kuthe
 # <https://gitlab.com/dmt-development/dmt-core>
 #
 # This file is part of DMT_core.
 #
@@ -30,20 +31,24 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>
 import copy
 import logging
 import time
 import subprocess
 import itertools
+import warnings
 from joblib import Parallel, delayed
 from reprint import output
 from pathlib import Path, PurePosixPath, PureWindowsPath
+from typing import List, Optional, Union
 import multiprocessing
 
 from DMT.core import Singleton, print_progress_bar
+from DMT.core.dut_view import DutView
+from DMT.core.sweep import Sweep
 from DMT.config import DATA_CONFIG
 from DMT.exceptions import SimulationUnsuccessful, SimulationFail
 
 # import them always -> can become very annoying otherways (if default is False but one dut is remote)
 from tempfile import NamedTemporaryFile
 from zipfile import ZipFile
 
@@ -97,15 +102,17 @@
         self.ssh_client = None
         self.scp_client = None
 
     def clear_sim_list(self):
         """Remove everything from the sim_list"""
         self.sim_list = []
 
-    def append_simulation(self, dut=None, sweep=None):
+    def append_simulation(
+        self, dut: Union[List[DutView], DutView] = None, sweep: Union[List[Sweep], Sweep] = None
+    ):
         """Adds DutViews together with Sweeps to the list of simulations sim_list.
 
         This methods adds each dut with a copy of each sweep to the simulation list.
 
         Parameters
         ----------
         dut : :class:`~DMT.core.dut_view.DutView` or [:class:`~DMT.core.dut_view.DutView`]
@@ -134,17 +141,17 @@
         remove_simulations : bool, optional
             If True, the simulation results will be deleted after read in, by default False. Activate to save disk space.
         parallel_read : bool, optional
             If True, the simulation results are read in using joblib parallel, by default False. Is False because some simulators have issues with this...
 
         Returns
         -------
-        boolean
+        all_sims_success : boolean
             True, if no simulation failed. This means it is also true if no simulation was run at all.
-        boolean
+        run_sims : boolean
             True, if any simulation was started. False if all simulations were read from hard disk.
         """
         # reduce number of jobs if we only read a very low number of simulations
         n_jobs = self.n_core if len(self.sim_list) > self.n_core else len(self.sim_list)
         if n_jobs == 0:  # sim list is empty
             return True, False  # all sims were successfull, but no simulations were run
         elif not parallel_read:
@@ -457,15 +464,15 @@
 
     def run_simulations(self, sim_list):
         """Runs all given simulations in parallel.
 
         Parameters
         ----------
         sim_list :  [{}]
-            List of dictionaries, each dictionary has a 'dut': :class:`~DMT.core.DutView` and 'sweep': :class:`~DMT.core.Sweep` key value pair.
+            List of dictionaries, each dictionary has a 'dut': :class:`~:class:`~DMT.core.dut_view.DutView`` and 'sweep': :class:`~:class:`~DMT.core.sweep.Sweep`` key value pair.
 
         Returns
         -------
         success  :  list[process]
             List of finished processes
         """
         if len(sim_list) == 0:
@@ -644,14 +651,22 @@
                     if (p["dt"] > p["dut"].t_max) and (
                         p["dt"] > self.t_max
                     ):  # both t_max have to be smaller than the simulation time
                         if not p["backend_remote"]:
                             p["process"].kill()
                         # TODO: kill with pbs
                         p["success"] = False
+                        warnings.warn(
+                            "DMT->SimCon: Simulation of "
+                            + p["dut"].name
+                            + " with sweep "
+                            + p["sweep"].name
+                            + " was killed because its maximum runtime reached "
+                            + str(p["dt"])
+                        )
                         process_finished.append(p)
 
                 # remove finished processes from running processes
                 for p in process_finished:
                     if p in process_running:
                         process_running.remove(p)
 
@@ -786,16 +801,16 @@
 
 
 def _check_simulation_needed(i_sim, n_tot, dut=None, sweep=None, sweep_exists=None):
     """Function to check if the simulation is needed or already present in the database
 
     Parameter
     -----------
-    dut : DMT.core.DutView
-    sweep : DMT.core.Sweep
+    dut : :class:`~DMT.core.dut_view.DutView`
+    sweep : :class:`~DMT.core.sweep.Sweep`
 
     Returns
     -------
     {key: DMT.core.Dataframe}
         In case the data is read from database or previous simulation.
     None
         In case the simulation must be done.
@@ -833,16 +848,16 @@
 
 def _read_process_results(success, dut, sweep):
     """Read the process results
 
     Parameter
     -----------
     success : bool
-    dut : DMT.core.DutView
-    sweep : DMT.core.Sweep
+    dut : :class:`~DMT.core.dut_view.DutView`
+    sweep : :class:`~DMT.core.sweep.Sweep`
 
     Returns
     -------
     {'success': success, 'dut_hash':dut.get_hash(), 'data':dut.data}
     """
     dut_name = dut.name + str(dut.get_hash())
     sim_name = sweep.name + "_" + sweep.get_hash()
```

### Comparing `DMT_core-2.0.0/DMT/core/singleton.py` & `DMT_core-2.1.0/DMT/core/singleton.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """ singleton
 
 Provides a meta class to ensure single instantiation.
 
 """
+
 # DMT_core
 # Copyright (C) from 2022  SemiMod
 # Copyright (C) until 2021  Markus Müller, Mario Krattenmacher and Pascal Kuthe
 # <https://gitlab.com/dmt-development/dmt-core>
 #
 # This file is part of DMT_core.
 #
```

### Comparing `DMT_core-2.0.0/DMT/core/sweep.py` & `DMT_core-2.1.0/DMT/core/sweep.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 Sweeps are the basic element that can be fed into simulators or be retrieved from simulations or measurements.
 Features:
 
 * Clear syntax and definition to create a well described simulation independent of the simulator interface.
 
 """
+
 # DMT_core
 # Copyright (C) from 2022  SemiMod
 # Copyright (C) until 2021  Markus Müller, Mario Krattenmacher and Pascal Kuthe
 # <https://gitlab.com/dmt-development/dmt-core>
 #
 # This file is part of DMT_core.
 #
@@ -27,46 +28,45 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>
 from __future__ import annotations
 import logging
 import copy
 from typing import Dict, List, Mapping, Type, Optional, Union, Set
 import numpy as np
 from itertools import product
-from DMT.core import create_md5_hash, specifiers, sub_specifiers, SpecifierStr, DataFrame, SweepDef
-from DMT.core.sweep_def import (
-    SweepDefLinear,
-    SweepDefList,
-    SweepDefLog,
-    SweepDefSync,
-    SweepDefConst,
-)
+from DMT.core.data_frame import DataFrame
+from DMT.core.naming import specifiers, sub_specifiers, SpecifierStr
+from DMT.core.hasher import create_md5_hash
+from DMT.core.sweep_def import SweepDef, SweepDefList, SweepDefConst
 
 _SPEC_VOLTAGE = specifiers.VOLTAGE
 _SPEC_CURRENT = specifiers.CURRENT
 _SPEC_TEMPERATURE = specifiers.TEMPERATURE
 _SPEC_FREQUENCY = specifiers.FREQUENCY
 _SSPEC_FORCED = sub_specifiers.FORCED
 
 
 def get_sweepdef(
     data: DataFrame,
     inner_sweep_voltage: Optional[SpecifierStr] = None,
     outer_sweep_voltage: Optional[SpecifierStr] = None,
+    col_third: Optional[SpecifierStr] = None,
     decimals_potentials: int = 3,
 ) -> List[Dict]:
     """Given a dataframe, one inner sweep_voltage and one outer sweep voltage, this method tries to create a SweepDefinition that can be used to re-simulate the data.
 
     Parameters
     ----------
     data : DataFrame
         Frame to extract the sweepdefs from
     inner_sweep_voltage : SpecifierStr | None, optional
-        A specifier that determiens the inner sweep voltage, by default None
+        A specifier that determins the inner sweep voltage, by default None
+    outer_sweep_voltage : SpecifierStr | None, optional
+        A specifier that determins the inner outer voltage, by default None
     outer_sweep_voltage : SpecifierStr | None, optional
-        A specifier that determiens the inner outer voltage, by default None
+        A voltage at a third possible contact, that is not swept but may differ from zero.
     decimals_potentials : int, optional
         Round the potentials to x number of decimals, by default 3
 
     Returns
     -------
     sweepdef : [{}]
         A sweep definition that can be used to init a SweepDef.
@@ -282,26 +282,48 @@
                 data[inner_potential_name].to_numpy() - data[reference_potential].to_numpy()
             )
             inner_potentials = np.unique(inner_potentials)
 
             # the circuit only allows to sweep VB VC VE, which are forced due to the circuit topology
             sweepdef = [
                 SweepDefConst(
-                    _SPEC_VOLTAGE + reference_potential.nodes[0], sweep_order=0, value_def=0
+                    _SPEC_VOLTAGE + reference_potential.nodes[0],
+                    sweep_order=0,
+                    value_def=0,
                 ),
                 SweepDefConst(outer_sweep_voltage, sweep_order=1, value_def=outer_potentials),
                 SweepDefList(
                     _SPEC_VOLTAGE + inner_potential_name.nodes[0],
                     sweep_order=2,
                     value_def=inner_potentials,
                 ),
             ]
         else:
             raise NotImplementedError()
 
+    # check if there is a third voltage (which must be constant), for example for BULK or SUBSTRATE nodes
+    try:
+        cols = list(data.columns)
+        potential_one_third = _SPEC_VOLTAGE + col_third.nodes[0] + col_third.sub_specifiers
+        potential_two_third = _SPEC_VOLTAGE + col_third.nodes[1] + col_third.sub_specifiers
+        v_third = data[potential_one_third].to_numpy() - data[potential_two_third].to_numpy()
+
+        # get the outermost sweeporder
+        sweep_order_third_voltage = max([swd.sweep_order for swd in sweepdef]) + 1
+        sweepdef.append(
+            SweepDefConst(
+                _SPEC_VOLTAGE + col_third.nodes[0],
+                sweep_order=sweep_order_third_voltage,
+                value_def=[v_third[0]],
+            )
+        )
+
+    except:
+        pass
+
     return sweepdef
 
 
 class Sweep(object):
     r"""Creates a sweep.
 
     The following parameters need to be specified in the sweepdef or othervar parameter for every DUT, else an error is raised:
@@ -678,15 +700,17 @@
         """Returns a hash for this sweep.
 
         Returns
         -------
         str
             MD5 hash that corresponds to this sweep.
         """
-        sweep_string = " ".join([str(self.sweepdef), str(self.outputdef), str(self.othervar)])
+        sweep_string = " ".join(
+            [self.name, str(self.sweepdef), str(self.outputdef), str(self.othervar)]
+        )
         return create_md5_hash(sweep_string)
 
     def set_values(self):
         """Set the values of sweep according to the DMT definition."""
         for subsweep in self.sweepdef:
             subsweep.set_values()
```

### Comparing `DMT_core-2.0.0/DMT/core/sweep_def.py` & `DMT_core-2.1.0/DMT/core/sweep_def.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 Sweeps are the basic element that can be fed into simulators or be retrieved from simulations or measurements.
 Features:
 
 * Clear syntax and definition to create a well described simulation independent of the simulator interface.
 
 """
+
 # DMT_core
 # Copyright (C) from 2022  SemiMod
 # Copyright (C) until 2021  Markus Müller, Mario Krattenmacher and Pascal Kuthe
 # <https://gitlab.com/dmt-development/dmt-core>
 #
 # This file is part of DMT_core.
 #
@@ -22,22 +23,18 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>
 from __future__ import annotations
-from typing import Dict, List, Mapping, Type, Optional, Union, Tuple
+from typing import List, Optional, Union, Tuple
 import numpy as np
-from DMT.core import (
-    specifiers,
-    get_specifier_from_string,
-    flatten,
-    SpecifierStr,
-)
+from DMT.core.naming import specifiers, SpecifierStr, get_specifier_from_string
+from DMT.core.data_processor import flatten
 
 
 class SweepDef(object):
     """One sweep definition
 
     Subclass this to introduce own sweep types. The methods which need to be overwritten are:
 
@@ -293,17 +290,35 @@
         elif self.sweep_type == "SYNC":
             if self.master is None:  # master has not been replaced jet..
                 return
 
             try:
                 self.values = self.master.values + self.offset
             except TypeError:
+                if isinstance(self.offset_var, SpecifierStr) and len(self.offset_var.nodes) == 2:
+                    # this is most likely a voltage synced V_BC sweep (or sth like that)
+                    if (self.offset_var.nodes[0] == self.master_var.nodes[0]) and (
+                        self.offset_var.nodes[1] == self.var_name.nodes[0]
+                    ):
+                        # V_BC
+                        op = np.subtract
+                    elif (self.offset_var.nodes[1] == self.master_var.nodes[0]) and (
+                        self.offset_var.nodes[0] == self.var_name.nodes[0]
+                    ):
+                        # V_CB
+                        op = np.add
+                    else:
+                        # no cluse
+                        op = np.add
+                else:
+                    op = np.add
+
                 self.values = np.zeros((self.offset.values.size, self.master.values.size))
                 for i_col in range(self.values.shape[0]):
-                    self.values[i_col, :] = self.master.values + self.offset.values[i_col]
+                    self.values[i_col, :] = op(self.master.values, self.offset.values[i_col])
                 self.values = np.concatenate(self.values)
 
         elif self.sweep_type == "SINUS":
             # 3 periods with 40 points per period
             self.values = np.array(
                 list(flatten(np.linspace(0, 3 / freq, 121) for freq in self.value_def))
             )
```

### Comparing `DMT_core-2.0.0/DMT/core/technology.py` & `DMT_core-2.1.0/DMT/core/technology.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """ Technology class to describe all technology dependencies. Main use is scaling.
 
 If a technology can use TRADICA, the class :class:`DMT.TRADICA.TechTradica` is recommended!
 
 """
+
 # DMT_core
 # Copyright (C) from 2022  SemiMod
 # Copyright (C) until 2021  Markus Müller, Mario Krattenmacher and Pascal Kuthe
 # <https://gitlab.com/dmt-development/dmt-core>
 #
 # This file is part of DMT_core.
 #
@@ -20,14 +21,16 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>
 import abc
 from DMT.core.dut_type import DutType
+import DMT.core.mcard as dmt_mcard
+import DMT.core.dut_view as dmt_dv
 
 try:
     from pylatex import Section
     from DMT.external.pylatex import Tex
 except ImportError:
     pass
 
@@ -42,32 +45,33 @@
 
     Attributes
     ----------
     name : str
         Name of the technology
 
     """
+
     name = ""
 
     def __init__(self, name):
         self.name = name
 
     @abc.abstractmethod
     def print_tex(self, dut_ref, mcard):
         """Prints a technology description, mainly used for autodocumentation reasons.
 
         Parameters
         ----------
-        dut_ref : :class:`~DMT.core.DutView`
+        dut_ref : :class:`~:class:`~DMT.core.dut_view.DutView``
             Can be used to obtain tech quanties... (or to generate a TRADICA input file :) )
         mcard : :class:`~DMT.core.McParameterCollection`
             A Modelcard that contains all parameters that are required for scaling, as well as the parameters that shall be scaled.
         """
         doc = Tex()
-        with doc.create(Section("Technology :" + self.name)):
+        with doc.create(Section("Technology: " + self.name)):
             doc.append("Technology description missing")
         return doc
 
     @abc.abstractmethod
     def get_bib_entries(self):
         """bibliograpy entries of a technology"""
         return ""
@@ -183,25 +187,35 @@
             Number of emitter fingers.
         config : str
             A unique identifier for the configuration.
         """
         raise NotImplementedError
 
     def scale_modelcard(
-        self, mcard, lE0, bE0, nfinger, config, lE_drawn_ref=None, bE_drawn_ref=None
-    ):
+        self,
+        mcard: "dmt_mcard.MCard",
+        lE0: float,
+        bE0: float,
+        nfinger: int,
+        config: str,
+        dut: "dmt_dv.DutView" = None,
+        lE_drawn_ref: float = None,
+        bE_drawn_ref: float = None,
+    ) -> "dmt_mcard.MCard":
         """This method scales a already finished modelcard (no sheet resistances).
 
         Parameters
         ----------
         mcard : :class:`~DMT.core.McParameterCollection`
             A Modelcard or McParameterCompositon that contains all parameters that are required for scaling, as well as the parameters that shall be scaled.
         lE0   : float64
             The length of the desired emitter window to be modeled by mcard.
         bE0   : float64
             The width of the desired emitter window to be modeled by mcard.
         nfinger : integer
             Number of emitter fingers.
         config : str
             A unique identifier for the configuration.
+        dut : :class:`~DMT.core.DutView`
+            DutView to scale for.
         """
         raise NotImplementedError
```

### Comparing `DMT_core-2.0.0/DMT/core/utils.py` & `DMT_core-2.1.0/DMT/core/utils.py`

 * *Files identical despite different names*

### Comparing `DMT_core-2.0.0/DMT/core/va_file.py` & `DMT_core-2.1.0/DMT/core/va_file.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """ VA Code structure. As Includes traverse like a tree, it is implemented as a dictionary Oo.
 """
+
 # DMT_core
 # Copyright (C) from 2022  SemiMod
 # Copyright (C) until 2021  Markus Müller, Mario Krattenmacher and Pascal Kuthe
 # <https://gitlab.com/dmt-development/dmt-core>
 #
 # This file is part of DMT_core.
 #
@@ -173,20 +174,29 @@
     @property
     def root_vfs(self) -> str:
         """Returns the root path inside the vfs
 
         Returns
         -------
         str
-            [description]
+            Path to the root file
         """
         return "/" + self.root
 
     @property
     def vfs(self) -> dict[str, str]:
+        """Virtual file system of this VAFileMap
+
+        The vfs is saved in a dictionary with {<path>: <file content>}
+
+        Returns
+        -------
+        dict[str, str]
+            The key is the path and the values are the file contents
+        """
         vfs = dict()
         for name, code in self.files.items():
             vfs["/" + name] = str(code)
         return vfs
 
     def rename_root(self, name_new: str):
         """Rename the root file
@@ -230,15 +240,15 @@
             self.files[self.root] = VACode(code=path_to_main_code.read_text())  # be safe
         except FileNotFoundError as e:
             va_files = path_to_own_folder.glob("*.va")
             va_files = [str(va_file) for va_file in va_files]
             va_files = "\n" + "\n".join(va_files)
             raise FileNotFoundError(
                 e.strerror, e.filename, " . Verilog-A files in this folder:" + va_files
-            )
+            ) from e
 
         for file, code in verilogae.export_vfs(str(path_to_main_code)).items():  # type: ignore
             self.files[file[1:]] = VACode(code=code)
 
     def get_tree_hash(self) -> str:
         """Create a hash for all the codes from this node and all its children. Should be unique for each model...
 
@@ -299,17 +309,19 @@
                 files[name] = VACode(code=code)
             else:
                 files[name] = VACode(code_compressed=code, ignore_checksum=ignore_checksum)
 
         return VAFileMap(name=root, files=files)
 
     def write_files(
-        self, path_to_target: Union[str, Path], filter: Optional[Callable[[str], str]] = None
+        self,
+        path_to_target: Union[str, Path],
+        filter: Optional[Callable[[str], str]] = None,
     ):
-        """Writes the all Verilog-A files from this mapping into the given target path. The file structure is written as read from the "original"
+        r"""Writes the all Verilog-A files from this mapping into the given target path. The file structure is written as read from the "original"
 
         Parameters
         ----------
         path_to_target : Union[str, Path]
             Path to target directory
         filter : callable, optional
             Called with each code file as an argument. Can be used to filter out "non-compiling" additional code parts.
```

### Comparing `DMT_core-2.0.0/DMT/exceptions/__init__.py` & `DMT_core-2.1.0/DMT/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `DMT_core-2.0.0/DMT/external/__init__.py` & `DMT_core-2.1.0/DMT/external/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """ DMT's external tools.
 
 These are routines and classes which manage the interfaces to other Python packages. For example PyLaTeX.
 """
+
 from .os import cd, recursive_copy, slugify, rmtree
 
 ## build tex
 from .latex import (
     build_tex,
     build_svg,
     clean_tex_files,
```

### Comparing `DMT_core-2.0.0/DMT/external/latex.py` & `DMT_core-2.1.0/DMT/external/latex.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """ DMT supplied build latex command
 """
+
 # DMT_core
 # Copyright (C) from 2022  SemiMod
 # Copyright (C) until 2021  Markus Müller, Mario Krattenmacher and Pascal Kuthe
 # <https://gitlab.com/dmt-development/dmt-core>
 #
 # This file is part of DMT_core.
 #
```

### Comparing `DMT_core-2.0.0/DMT/external/os.py` & `DMT_core-2.1.0/DMT/external/os.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """ OS interaction of DMT
 """
+
 # DMT_core
 # Copyright (C) from 2022  SemiMod
 # Copyright (C) until 2021  Markus Müller, Mario Krattenmacher and Pascal Kuthe
 # <https://gitlab.com/dmt-development/dmt-core>
 #
 # This file is part of DMT_core.
 #
@@ -72,15 +73,15 @@
             if not item_dst.exists() or force:
                 shutil.copy(item_src, dst)
 
         elif item_src.is_dir():
             item_dst.mkdir(exist_ok=True)
             recursive_copy(item_src, item_dst)
         else:
-            raise ValueError("DMT->recursive_copy: I do not know this filettype.")
+            raise ValueError("DMT->recursive_copy: I do not know this filetype.")
 
 
 def rmtree(root):
     """rmtree method for Path objects
 
     Parameters
     ----------
```

### Comparing `DMT_core-2.0.0/DMT/external/pylatex.py` & `DMT_core-2.1.0/DMT/external/pylatex.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """ DMT specific PyLaTeX classes and routines used for automatic documentations
 
 """
+
 # DMT_core
 # Copyright (C) from 2022  SemiMod
 # Copyright (C) until 2021  Markus Müller, Mario Krattenmacher and Pascal Kuthe
 # <https://gitlab.com/dmt-development/dmt-core>
 #
 # This file is part of DMT_core.
 #
@@ -58,14 +59,16 @@
         if self.language == "TRADICA":
             str_language = (
                 "backgroundcolor=\\color{lightgray!40},\n"
                 + "breaklines=true, breakatwhitespace=true,\n"
                 + "emph={[1]NAME, TRACE, OPTI, PHYS, TECH, DEVICE, OUTPUT, PGEN, RUN, END}, emphstyle={[1]\\bfseries},\n"
                 + "emph={[2]UNIT_INP, PERMITT, BGP NARR, SAT_VELO, HOLE_MOBI, ELEC_MOBI, INFO_PROCESS, GEOM_DATA, ELEC_PAR, HICUM_PAR, MODEL_DEF, MISC_VAR, TRAN_CONF}, emphstyle={[2]\\color{Blue}},\n"
             )
+        elif self.language is None:
+            str_language = ""
         else:
             str_language = "language=" + self.language + ",\n"
 
         str_caption = "caption={:s},\n".format(self.caption) if self.caption is not None else ""
         str_label = "label={:s},\n".format(self.label) if self.label is not None else ""
         if self.file_path is None:
             return (
```

### Comparing `DMT_core-2.0.0/DMT/external/verilogae.py` & `DMT_core-2.1.0/DMT/external/verilogae.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """ Helpers to integrate VerilogAE into DMT
 """
+
 # DMT_core
 # Copyright (C) from 2022  SemiMod
 # Copyright (C) until 2021  Markus Müller, Mario Krattenmacher and Pascal Kuthe
 # <https://gitlab.com/dmt-development/dmt-core>
 #
 # This file is part of DMT_core.
 #
@@ -74,14 +75,15 @@
         else:
             try:
                 func_params += dependence.parameters
             except AttributeError:
                 func_params += get_param_list(dependence, all_parameters=all_parameters)
 
     # unique it!
+    func_params = [para.lower() for para in func_params]  # make sure lower case
     func_params = list(OrderedDict.fromkeys(func_params))
 
     if all_parameters:
         func_params = list(OrderedDict.fromkeys(func_params))
         return func_params
 
     # delete the parameters which are independent and without the opti_params
```

### Comparing `DMT_core-2.0.0/DMT/libautodoc_template/base/acronyms.tex` & `DMT_core-2.1.0/DMT/libautodoc_template/base/acronyms.tex`

 * *Files identical despite different names*

### Comparing `DMT_core-2.0.0/DMT/libautodoc_template/base/header.tex` & `DMT_core-2.1.0/DMT/libautodoc_template/base/header.tex`

 * *Files identical despite different names*

### Comparing `DMT_core-2.0.0/DMT/libautodoc_template/content/conclusion.tex` & `DMT_core-2.1.0/DMT/libautodoc_template/content/conclusion.tex`

 * *Files identical despite different names*

### Comparing `DMT_core-2.0.0/DMT/libautodoc_template/content/deckblatt.tex` & `DMT_core-2.1.0/DMT/libautodoc_template/content/deckblatt.tex`

 * *Files identical despite different names*

### Comparing `DMT_core-2.0.0/DMT/libautodoc_template/content/introduction.tex` & `DMT_core-2.1.0/DMT/libautodoc_template/content/introduction.tex`

 * *Files identical despite different names*

### Comparing `DMT_core-2.0.0/DMT/libautodoc_template/documentation.tex` & `DMT_core-2.1.0/DMT/libautodoc_template/documentation.tex`

 * *Files identical despite different names*

### Comparing `DMT_core-2.0.0/DMT/ngspice/__init__.py` & `DMT_core-2.1.0/DMT/ngspice/__init__.py`

 * *Files identical despite different names*

### Comparing `DMT_core-2.0.0/DMT/ngspice/dut_ngspice.py` & `DMT_core-2.1.0/DMT/ngspice/dut_ngspice.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 * :py:attr:`.list_append` : Absolute path to a load file. The file will be loaded using the absolute path at the begin of the netlist.
 * :py:attr:`.list_import` : Absolute or relative path files will be copied into the simulation folder and also loaded at the begin of the netlist.
 
 This can be used for Verilog files. The correct load of ADS is determined by file ending.
 
 """
+
 # DMT_core
 # Copyright (C) from 2022  SemiMod
 # Copyright (C) until 2021  Markus Müller, Mario Krattenmacher and Pascal Kuthe
 # <https://gitlab.com/dmt-development/dmt-core>
 #
 # This file is part of DMT_core.
 #
@@ -39,15 +40,15 @@
 import logging
 import copy
 import re
 import numpy as np
 import pandas as pd
 import subprocess
 from pathlib import Path
-from typing import List, Dict
+from typing import List, Dict, Type
 
 try:
     from semver.version import Version as VersionInfo
 except ImportError:
     from semver import VersionInfo
 
 from DMT.config import COMMANDS
@@ -59,15 +60,23 @@
     DataFrame,
     specifiers,
     sub_specifiers,
     McParameterCollection,
     SweepDef,
     Technology,
 )
-from DMT.core.circuit import SGP_BJT, VOLTAGE, CURRENT, HICUML2_HBT, SHORT, DIODE
+from DMT.core.circuit import (
+    SGP_BJT,
+    VOLTAGE,
+    CURRENT,
+    HICUML2_HBT,
+    SHORT,
+    DIODE,
+    SUBCIRCUIT,
+)
 
 from DMT.exceptions import SimulationUnsuccessful
 
 SEMVER_DUTNGSPICE_CURRENT = VersionInfo(major=1, minor=0)
 
 
 class DutNgspice(DutCircuit):
@@ -82,29 +91,32 @@
     dut_type   : :class:`~DMT.core.dut_type.DutType`
         Type of the DUT.
     nodes     : string
         Strings with comma separated node names of DUT. If nodes is None, nodes will be requested from Dut_type class.
     input_circuit : str, list[str] or :class:`~DMT.classes.circuit.Circuit`
     copy_va_files : {False, True}
         If True, all given VA-files are copied to the simulation directory and compiled there. If False, the VA-Files have to be given as a global path.
+    va_maps : [DMT.core.VAFileMap]
+        Verilog-A file mapping that contains any additional Verilog-A files needed for this DutCircuit.
     """
 
     def __init__(
         self,
         database_dir,
         dut_type,
-        inp_circuit,
+        input_circuit,
         name="ngspice_",
         simulator_options=None,
         simulator_command=None,
         simulator_arguments=None,
         initial_conditions={},
         command_openvaf=COMMANDS["OPENVAF"],
         copy_va_files=False,
         inp_name="ngspice_circuit.ckt",
+        va_maps=[],
         **kwargs,
     ):
         if simulator_command is None:
             simulator_command = COMMANDS["NGSPICE"]
 
         if simulator_arguments is None:
             simulator_arguments = ["-r raw.raw", "-b "]
@@ -117,20 +129,21 @@
 
         simulator_options = default_options
 
         self.initial_conditions = initial_conditions
         self.devices_op_vars = []
         self._osdi_imports = []
         self.command_openvaf = command_openvaf
+        self.va_maps = va_maps
 
         super().__init__(
             database_dir,
             name,
             dut_type,
-            inp_circuit,
+            input_circuit,
             simulator_command=simulator_command,
             simulator_options=simulator_options,
             simulator_arguments=simulator_arguments,
             inp_name=inp_name,
             copy_va_files=copy_va_files,
             **kwargs,
         )
@@ -153,35 +166,35 @@
 
         return {
             str(DutNgspice): {
                 "__DutNgspice__": str(SEMVER_DUTNGSPICE_CURRENT),
                 "parent": super(DutNgspice, self).info_json(**_kwargs),
                 "initial_conditions": self.initial_conditions,
                 "devices_op_vars": self.devices_op_vars,
-                "_osdi_imports": self._osdi_imports,
+                "_osdi_imports": [str(osdi) for osdi in self._osdi_imports],
                 "command_openvaf": self.command_openvaf,
             }
         }
 
     @classmethod
     def from_json(
         cls,
         json_content: Dict,
-        classes_technology: List[type[Technology]],
+        classes_technology: List[Type[Technology]],
         subclass_kwargs: Dict = None,
     ) -> "DutNgspice":
         """Static class method. Loads a DutNgspice object from a json or pickle file with full path save_dir.
 
         Calls the from_json method of DutView with all dictionary inside the "parent" keyword. Afterwards the additional parameters are set correctly.
 
         Parameters
         ----------
         json_content  :  dict
             Readed dictionary from a saved json DutNgspice.
-        classes_technology : List[type[Technology]]
+        classes_technology : List[Type[Technology]]
             All possible technologies this loaded DutNgspice can have. One will be choosen according to the serialized technology loaded from the file.
         subclass_kwargs : Dict, optional
             Additional kwargs necessary to create the concrete subclassed DutView.
 
         Returns
         -------
         DutNgspice
@@ -191,15 +204,15 @@
             raise NotImplementedError("DMT.DutNgspice: Unknown version of DutNgspice to load!")
 
         dut_view = super().from_json(
             json_content["parent"], classes_technology, subclass_kwargs=subclass_kwargs
         )
         dut_view.initial_conditions = json_content["initial_conditions"]
         dut_view.devices_op_vars = json_content["devices_op_vars"]
-        dut_view._osdi_imports = json_content["_osdi_imports"]
+        dut_view._osdi_imports = [Path(osdi) for osdi in json_content["_osdi_imports"]]
         dut_view.command_openvaf = json_content["command_openvaf"]
 
         return dut_view
 
     def create_inp_header(self, inp_circuit: Union[MCard, McParameterCollection, Circuit]):
         """Creates the input header of the given circuit description and returns it.
 
@@ -224,17 +237,19 @@
                 and self.get_circuit_arguments["use_build_in"]
             ):
                 use_osdi = False
             # in case a standard circuit is used, this is the real input circuit
         elif isinstance(inp_circuit, Circuit):
             self._modelcard = None
             self._inp_circuit = copy.deepcopy(inp_circuit)
+
+            self.list_copy += inp_circuit.lib_files
         else:
             raise OSError(
-                "For ADS circuits netlist generation is only possible from object of class DMT.classes.Circuit"
+                "For ngspice circuits netlist generation is only possible from object of class DMT.core.MCard or DMT.core.Circuit"
             )
 
         self.devices_op_vars = []
         str_netlist = "DMT generated netlist\n"
         str_netlist += ".Options " + self._convert_dict_to_inp_line(self.simulator_options) + "\n"
 
         if use_osdi:
@@ -243,14 +258,17 @@
             for element in self._inp_circuit.netlist:
                 try:
                     list_va_files.append(element.parameters.va_codes)
                 except AttributeError:
                     # element does not have a va_file.
                     pass
 
+            list_va_files += self._inp_circuit.verilog_maps
+            list_va_files += self.va_maps
+
             # pre_osdi strings
             self._osdi_imports = []
             for vafile in list_va_files:
                 if vafile is None:
                     continue
 
                 self._list_va_file_contents.append(vafile)
@@ -357,30 +375,34 @@
 
         for osdi in self._osdi_imports:
             try:
                 if osdi.suffix != ".osdi":
                     # compile needed ? Could be compiled by a "parallel" simulation
                     if not osdi.with_suffix(".osdi").is_file():
                         process = subprocess.run(
-                            [self.command_openvaf, osdi.name], shell=False, cwd=osdi.parent
+                            [self.command_openvaf, osdi.name],
+                            shell=False,
+                            cwd=osdi.parent,
                         )
                         if process.returncode != 0:
                             raise OSError(
                                 "DMT.DutNgspice: Run of OpenVAF failed!",
                                 f"The file to compile was {osdi}",
                             )
                     osdi = osdi.with_suffix(".osdi")
 
                 # import from common "VA_codes" folder
                 str_netlist += f"pre_osdi {osdi}\n"
             except AttributeError:
                 # import from relative location
                 # compile always needed
                 process = subprocess.run(
-                    [self.command_openvaf, osdi], shell=False, cwd=self.get_sim_folder(sweep)
+                    [self.command_openvaf, osdi],
+                    shell=False,
+                    cwd=self.get_sim_folder(sweep),
                 )
                 if process.returncode != 0:
                     raise OSError(
                         "DMT.DutNgspice: Run of OpenVAF failed!",
                         f"The file to compile was {osdi} in {self.get_sim_folder(sweep)}",
                     )
 
@@ -466,20 +488,25 @@
             str_netlist = str_netlist.replace(source_old, sources_new)
         except StopIteration:
             swd_tran = False
 
         # create vectors for each voltage
         one_ele_array = False
         for voltage_source in voltage_sources:
-            vals = df[voltage_source.name].to_numpy()
-            if (
-                len(vals) == 1
-            ):  # Ngspice does not support 1 element arrays ... so we just extend it.
+            try:
+                vals = df[voltage_source.name].to_numpy()
+            except KeyError:  # assume that a voltage not specified in the sweep is grounded
+                vals = np.zeros_like(0, shape=len(df))
+            if len(vals) == 1:
+                # spice does not support 1 element arrays ... so we just extend it.
                 vals = np.append(vals, vals)
                 one_ele_array = True
+            elif len(vals) > 1000:
+                raise IOError("ngspice only allows vectors up to 1000 length.")
+
             str_vec = (
                 "compose V_"
                 + voltage_source.name
                 + "_vec values "
                 + "".join(["(" + str(val) + ") " for val in vals])
             )
             str_netlist += str_vec + "\n"
@@ -596,20 +623,14 @@
         ----------
         sweep  :  :class:`DMT.core.sweep.Sweep`
             Sweep that has been simulated for the desired output files.
         """
         # get sweep folder
         sim_folder = self.get_sim_folder(sweep)
 
-        # find .ngspice file
-        for my_file in os.listdir(sim_folder):
-            filename = os.fsdecode(my_file)
-            if filename.endswith(".ngspice"):
-                break
-
         # find .ngspice files (these are DC and AC)
         files_dc_ac = [sim_file for sim_file in sim_folder.glob("*.ngspice")]
         # are there transient simulations?
         files_tran = sorted(sim_file for sim_file in sim_folder.glob("*.ngspice_tr"))
 
         key = self.join_key(self.get_sweep_key(sweep), "iv")
         dfs_dc_ac = [
@@ -641,15 +662,17 @@
             sim_folder,
         )
 
         sim_log = os.path.join(sim_folder, "sim.log")
         with open(sim_log) as my_log:
             log_content = my_log.read()
         search_obj_time = re.search(
-            r"User time(.+?)Total stopwatch time", log_content, flags=re.IGNORECASE | re.DOTALL
+            r"User time(.+?)Total stopwatch time",
+            log_content,
+            flags=re.IGNORECASE | re.DOTALL,
         )
         if search_obj_time:
             logging.info("Simulation times: %s.", search_obj_time.group(1))
 
     def validate_simulation_successful(self, sweep):
         """Checks if the simulation of the given sweep was successful.
 
@@ -672,30 +695,35 @@
 
         # find log file
         sim_log = os.path.join(sim_folder, "sim.log")
 
         with open(sim_log) as my_log:
             log_content = my_log.read()
 
-        if "error" in log_content:
+        if re.search("error", log_content, re.IGNORECASE):
             print("DMT - NGSPICE: Simulation failed! An error was found in the simulation log!")
             logging.debug("Log content:\n%s", log_content)
             raise SimulationUnsuccessful(
                 "NGSPICE Simulation of the sweep "
                 + sweep.name
                 + " with the hash "
                 + sweep.get_hash()
                 + " failed! An error was found!"
             )
 
-        # need to find something similar for ngspice
-        # if not seach_obj_end:
-        #     print("DMT - DutAds: Simulation failed! The simulation log file is not complete!")
-        #     logging.debug("Log content:\n%s", log_content)
-        #     raise SimulationUnsuccessful('ADS Simulation of the sweep ' + sweep.name + ' with the hash ' + sweep.get_hash() + ' failed! The simulation log file is not complete!')
+        if not re.search("Total elapsed time", log_content, re.IGNORECASE):
+            print("DMT - NGSPICE: Simulation not finished!")
+            logging.debug("Log content:\n%s", log_content)
+            raise SimulationUnsuccessful(
+                "NGSPICE Simulation of the sweep "
+                + sweep.name
+                + " with the hash "
+                + sweep.get_hash()
+                + " did not finish!"
+            )
 
         # find .ngspice file
         for my_file in os.listdir(sim_folder):
             filename = os.fsdecode(my_file)
             if filename.endswith(".ngspice"):
                 break
 
@@ -709,15 +737,15 @@
                 + sweep.name
                 + " with the hash "
                 + sweep.get_hash()
                 + " failed! The simulation result raw file was not found!"
             )
 
     def _convert_dict_to_inp_line(self, dict_key_para):
-        """Converts dictionary into a line for a ADS input file.
+        """Converts dictionary into a line for a ngspice input file.
 
         Transforms a dictionary with
 
         | dict[key1] = value1
         | dict[key2] = value2
 
         into a line with "key1=value1 key2=value2 ". Correctly converts strings, iteratables, bools and numbers.
@@ -773,14 +801,15 @@
         # only those that differ between DMT definiton and NGspice definition are listed here
         element_types = {
             VOLTAGE: "V",
             CURRENT: "I",
             HICUML2_HBT: "Q",
             SGP_BJT: "Q",
             "bjtn": "Q",
+            SUBCIRCUIT: "X",
         }
         if circuit_element.element_type in element_types.keys():
             element_type = element_types[circuit_element.element_type]
         elif circuit_element.element_type == SHORT:
             element_type = "V"
             circuit_element.name = "V_" + circuit_element.name.replace("I", "V")
             circuit_element.parameters = [("dc", str(0)), ("ac", str(0))]
@@ -881,33 +910,38 @@
                 self.devices_op_vars += [
                     f"@{element_type}_{circuit_element.name}[{op_var:s}]"
                     for op_var in mcard.op_vars
                 ]
 
             else:
                 str_temp = []
-                for para, value in circuit_element.parameters:
-                    if para in ["C", "R", "L"]:  # rename according to ngspice manual
-                        str_temp.append(value)
-                    elif para in ["Vdc", "Vac", "Idc", "Iac"] and not isinstance(
-                        value, float
+                for para in circuit_element.parameters:
+                    if isinstance(para, str):
+                        str_temp.append(para)
+                    elif para[0] in ["C", "R", "L"]:
+                        # rename according to ngspice manual
+                        str_temp.append(para[1])
+                    elif para[0] in ["Vdc", "Vac", "Idc", "Iac"] and not isinstance(
+                        para[1], float
                     ):  # just leave voltages from lines, as ngpsice directly changes the sources and not the parameters
                         pass
                     else:
-                        str_temp.append(para + "=" + value)
+                        str_temp.append(para[0] + "=" + para[1])
 
                 str_temp = " ".join(str_temp)
 
                 # find sim paras
                 sim_paras = ""
-                for para, value in circuit_element.parameters:
+                for para in circuit_element.parameters:
+                    if isinstance(para, str):
+                        pass
                     try:
-                        float(value)
+                        float(para[1])
                     except ValueError:
-                        sim_paras = sim_paras + value + "=0 "
+                        sim_paras = sim_paras + para[1] + "=0 "
 
                 if sim_paras != "":
                     sim_paras = "\n.param " + sim_paras
 
                 str_temp = str_temp + "".join(sim_paras)
 
             # catch ngspice keywords
@@ -1177,17 +1211,17 @@
         if "#BRANCH" in col_raw:  # current that we should save
             col_raw = col_raw.replace("#BRANCH", "")
             node = next(node for node in nodes if node in col_raw)
             new_df[specifiers.CURRENT + node] = -df[col]  # we want the other current direction
         elif col_raw[0:2] == "N_":  # found a node, will take the voltage
             node = col_raw[2:]
             if "_FORCED" in node:
-                new_df[
-                    specifiers.VOLTAGE + node.replace("_FORCED", "") + sub_specifiers.FORCED
-                ] = df[col]
+                new_df[specifiers.VOLTAGE + node.replace("_FORCED", "") + sub_specifiers.FORCED] = (
+                    df[col]
+                )
             else:
                 new_df[specifiers.VOLTAGE + node] = df[col]
         elif col_raw == "FREQUENCY":
             new_df[specifiers.FREQUENCY] = np.real(df["frequency"].to_numpy())
         elif col_raw == "TIME":
             new_df[specifiers.TIME] = np.real(df["time"].to_numpy())
```

### Comparing `DMT_core-2.0.0/DMT/xyce/__init__.py` & `DMT_core-2.1.0/DMT/xyce/__init__.py`

 * *Files identical despite different names*

### Comparing `DMT_core-2.0.0/DMT/xyce/dut_xyce.py` & `DMT_core-2.1.0/DMT/xyce/dut_xyce.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """ The interface to the Xyce circuit simulator from Sandia
 """
+
 # DMT_core
 # Copyright (C) from 2022  SemiMod
 # Copyright (C) until 2021  Markus Müller, Mario Krattenmacher and Pascal Kuthe
 # <https://gitlab.com/dmt-development/dmt-core>
 #
 # This file is part of DMT_core.
 #
@@ -24,15 +25,15 @@
 import re
 import subprocess
 import warnings
 import numpy as np
 import pandas as pd
 import time
 from pathlib import Path
-from typing import List, Dict
+from typing import List, Dict, Type
 
 try:
     from semver.version import Version as VersionInfo
 except ImportError:
     from semver import VersionInfo
 
 from DMT.config import DATA_CONFIG
@@ -58,28 +59,29 @@
     INDUCTANCE,
     CAPACITANCE,
     VOLTAGE,
     CURRENT,
     SHORT,
     HICUML2_HBT,
     SGP_BJT,
+    SUBCIRCUIT,
 )
 from DMT.exceptions import SimulationUnsuccessful, SimulationFail
 
 SEMVER_DUTXYCE_CURRENT = VersionInfo(major=1, minor=0)
 
 
 class DutXyce(DutCircuit):
     """Class to interface the Xyce circuit simulator"""
 
     def __init__(
         self,
         database_dir,
         dut_type,
-        inp_circuit,
+        input_circuit,
         name="xyce_",
         simulator_command=None,
         simulator_arguments=None,
         simulator_options=None,
         build_xyce_plugin_command="buildxyceplugin",
         inp_name="xyce_circuit.cir",
         **kwargs,
@@ -98,15 +100,15 @@
         self.build_xyce_plugin_command = build_xyce_plugin_command
         self._va_plugins_to_compile = []
 
         super().__init__(
             database_dir,
             name,
             dut_type,
-            inp_circuit,
+            input_circuit,
             simulator_command=simulator_command,
             simulator_options=simulator_options,
             simulator_arguments=simulator_arguments,
             inp_name=inp_name,
             **kwargs,
         )
 
@@ -145,26 +147,26 @@
             }
         }
 
     @classmethod
     def from_json(
         cls,
         json_content: Dict,
-        classes_technology: List[type[Technology]],
+        classes_technology: List[Type[Technology]],
         subclass_kwargs: Dict = None,
     ) -> "DutXyce":
         """Static class method. Loads a DutXyce object from a json or pickle file with full path save_dir.
 
         Calls the from_json method of DutView with all dictionary inside the "parent" keyword. Afterwards the additional parameters are set correctly.
 
         Parameters
         ----------
         json_content  :  dict
             Readed dictionary from a saved json DutNgspice.
-        classes_technology : List[type[Technology]]
+        classes_technology : List[Type[Technology]]
             All possible technologies this loaded DutNgspice can have. One will be choosen according to the serialized technology loaded from the file.
         subclass_kwargs : Dict, optional
             Additional kwargs necessary to create the concrete subclassed DutView.
 
         Returns
         -------
         DutXyce
@@ -212,37 +214,40 @@
                 "use_build_in" in self.get_circuit_arguments
                 and self.get_circuit_arguments["use_build_in"]
             ):
                 va_from_model_build_in = True
         elif isinstance(inp_circuit, Circuit):
             self._modelcard = None
             self._inp_circuit = copy.deepcopy(inp_circuit)
+            self.list_copy += inp_circuit.lib_files
         else:
             raise OSError(
-                "For Xyce circuits netlist generation is only possible from object of class DMT.classes.Circuit. Passed "
+                "For Xyce circuits netlist generation is only possible from object of class DMT.core.MCard or DMT.core.Circuit. Passed "
                 + str(inp_circuit)
                 + "."
             )
 
         str_netlist = (
             "DMT Xyce simulation\n"
             # "simulator1Options options "
             # + self._convert_dict_to_inp_line(self.simulator_options)
-            # + "\n\n"
+            + "\n\n"
         )
 
         # is a modelcard inside the netlist?
         list_va_files = list()
         for element in self._inp_circuit.netlist:
             try:
                 list_va_files.append(element.parameters.va_codes)
             except AttributeError:
                 # element does not have a va_file.
                 pass
 
+        list_va_files += self._inp_circuit.verilog_maps
+
         if not va_from_model_build_in:
             # load va file plugins and mark missing ones -> they are compiled later:
             va_plugins = []
             self._va_plugins_to_compile = []  # reset the plugins
             for vafile in list_va_files:
                 if vafile is None:
                     continue
@@ -271,19 +276,19 @@
                     self.sim_args.append(",".join(str(va_path) for va_path in va_plugins))
 
         str_netlist += "\n* Netlist\n"
 
         # add elements:
         for index, element in enumerate(self._inp_circuit.netlist):
             if isinstance(element, str):
-                if not "include" in element:
-                    str_netlist += ".PARAM " + element + "\n"
-                else:
-                    raise NotImplementedError("Need a test case for this ?!?")
+                if element.startswith(".include") or element.startswith(".lib"):
                     str_netlist += element + "\n"
+                else:
+                    # raise NotImplementedError("Need a test case for this ?!?")
+                    str_netlist += ".PARAM " + element + "\n"
 
             else:
                 str_netlist = str_netlist + self._convert_CircuitElement_netlist(element, index)
 
         logging.info("Successfully created input header of dut %s!", self.name)
         logging.debug("Content:\n%s", str_netlist)
 
@@ -304,14 +309,15 @@
         str
             Netlist line
         """
         converter = {
             RESISTANCE: "R",
             CAPACITANCE: "C",
             INDUCTANCE: "I",
+            SUBCIRCUIT: "X",
         }
 
         if circuit_element.element_type == SHORT:
             return (
                 "R"
                 + circuit_element.name
                 + " "
@@ -419,24 +425,28 @@
                         str_netlist += " {0:s} = {0:d}".format(para)
                     else:
                         str_netlist += " {0:s} = {0:10.10e}".format(para)
 
             return str_netlist + " )\n"
         else:
             try:
-                # resistors, capacitors and inductors
+                # resistors, capacitors, inductors and other "standard" elements
                 str_netlist = (
                     converter[circuit_element.element_type]
                     + circuit_element.name
                     + " "
                     + " ".join(circuit_element.contact_nodes)
                     + " "
                 )
-                for para, value in circuit_element.parameters:
-                    str_netlist += para.upper() + "=" + value + " "
+                # for para, value in circuit_element.parameters:
+                for para in circuit_element.parameters:
+                    if isinstance(para, str):
+                        str_netlist += para + " "  # flavors and stuff
+                    else:
+                        str_netlist += para[0].upper() + "=" + para[1] + " "
 
                 return str_netlist + " \n"
 
             except KeyError:
                 # special devices like the transistor
                 model_name = circuit_element.parameters.default_subckt_name + "_{:d}".format(index)
                 str_netlist = (
@@ -480,15 +490,18 @@
         # first make copy of sweep, ensuring that the actual sweep object is not changed
         tmp_sweep = copy.deepcopy(sweep)
         # sweepdefs = copy.deepcopy(tmp_sweep.sweepdef)
 
         # compile plugins if needed and also add to arguments
         if self._va_plugins_to_compile:
             print_progress_bar(
-                0, len(self._va_plugins_to_compile), prefix="Compiling Xyce plugins", length=50
+                0,
+                len(self._va_plugins_to_compile),
+                prefix="Compiling Xyce plugins",
+                length=50,
             )
             processes = []
             for path_plugin, vafile in self._va_plugins_to_compile:
                 # write to location
                 vafile.rename_root(path_plugin.with_suffix(".va").name)
                 # does it exist now ? (can happen if two different duts are used...)
                 if path_plugin.is_file():
@@ -511,15 +524,15 @@
                         stderr=subprocess.STDOUT,
                         stdout=log_file,
                     )
                 )
 
             time_start = time.time()
             time_out = True
-            while time.time() - time_start < 60:
+            while time.time() - time_start < 120:
                 finished = 0
                 for i_p, process in enumerate(processes[:]):
                     returncode = process.poll()
                     if returncode is None:
                         time.sleep(0.1)
                     else:
                         if (
@@ -592,15 +605,20 @@
         tmp_sweep.outputdef = []
 
         # ac forward and backward ?
         str_ac_switch = ""
         if swd_ac is not None:
             if "ac_switch" in str_netlist:
                 tmp_sweep.sweepdef.append(
-                    SweepDef(SpecifierStr("ac_switch"), "LIST", sweep_order=1000, value_def=[0, 1])
+                    SweepDef(
+                        SpecifierStr("ac_switch"),
+                        "LIST",
+                        sweep_order=1000,
+                        value_def=[0, 1],
+                    )
                 )  # just use a very high sweep order to make sure it is the last one...
                 str_ac_switch = " ac_switch"
 
         # remove columns which are not in the netlist
         tmp_sweep = tmp_sweep.set_values()
         df_def = tmp_sweep.create_df()
         for col in copy.deepcopy(df_def.columns):
@@ -655,14 +673,52 @@
         str_netlist += "\n.END\n"
 
         logging.info("Added bias sweep to input header.")
         logging.debug("\n%s", str_netlist)
 
         return str_netlist
 
+    def _convert_dict_to_inp_line(self, dict_key_para):
+        """Converts dictionary into a line for a ngspice input file.
+
+        Transforms a dictionary with
+
+        | dict[key1] = value1
+        | dict[key2] = value2
+
+        into a line with "key1=value1 key2=value2 ". Correctly converts strings, iteratables, bools and numbers.
+
+        Parameters
+        ----------
+        dict_key_para : dict
+
+        Returns
+        -------
+        str
+            Line to add into input file
+        """
+        str_return = ""
+
+        for key, param in dict_key_para.items():
+            if isinstance(param, str):
+                str_add = key + "=" + param + " "
+            elif isinstance(param, (list, tuple)):
+                str_add = key + "=" + " ".join([str(nr) for nr in param]) + " "
+            elif isinstance(param, bool):
+                str_add = "yes" if param else "no"
+                str_add = key + "=" + str_add
+            elif param is None:
+                str_add = key + " "
+            else:
+                str_add = key + "=" + str(param) + " "
+
+            str_return = str_return + str_add
+
+        return str_return
+
     def validate_simulation_successful(self, sweep):
         """Checks if the simulation of the given sweep was successful.
 
         Parameters
         ----------
         sweep  :  :class:`DMT.core.sweep.Sweep`
             Sweep that has been simulated.
@@ -747,15 +803,16 @@
             if search_obj_time:
                 logging.info("Simulation time: %s.", search_obj_time.group(1))
 
             if delete_sim_results:
                 self.delete_sim_results(sweep)
         else:
             logging.info(
-                "Read the Xyce simulation output data of the from the file %s.", filepaths[0]
+                "Read the Xyce simulation output data of the from the file %s.",
+                filepaths[0],
             )
 
     def _import_xyce_results(self, *filepaths):
         """Reads the filepaths (must be CSVs), converts them and joins them together to one DMT.DataFrame
 
         Parameters
         ----------
```

### Comparing `DMT_core-2.0.0/DMT_core.egg-info/PKG-INFO` & `DMT_core-2.1.0/DMT_core.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DMT-core
-Version: 2.0.0
+Version: 2.1.0
 Summary: Device Modeling Toolkit Core
 Home-page: https://gitlab.com/dmt-development/dmt
 Author: M.Mueller, M.Krattenmacher
 Author-email: markus.mueller@semimod.de, mario.krattenmacher@semimod.de
 License: GNU GPLv3+
 Project-URL: Bug Tracker, https://gitlab.com/dmt-development/dmt
 Project-URL: Documentation, https://dmt-development.gitlab.io/dmt-core/
@@ -41,14 +41,18 @@
 
 [![logo](https://gitlab.com/uploads/-/system/project/avatar/33580822/DMT_Logo_wText.png)](https://gitlab.com/uploads/-/system/project/avatar/33580822/DMT_Logo_wText.png)
 
 DeviceModelingToolkit (DMT) is a Python tool targeted at helping modeling engineers extract model parameters, run circuit and TCAD simulations and automate their infrastructure.
 
 See the [DMT-website](https://dmt-development.gitlab.io/dmt-core/index.html) for further information.
 
+This project is funded by [NLnet](https://nlnet.nl/project/DMT-Core/) under the [NGI Zero Entrust fund](https://nlnet.nl/entrust/).
+
+<img src="pictures/banner_nlnet.svg" width="325"/>
+
 ## Usage
 
 ### Installation to virtual environment
 
 After installing python 3.8 or later, create a virtual environment and install the release version using
 
 ```bash
```

### Comparing `DMT_core-2.0.0/DMT_core.egg-info/SOURCES.txt` & `DMT_core-2.1.0/DMT_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DMT_core-2.0.0/LICENSE` & `DMT_core-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `DMT_core-2.0.0/PKG-INFO` & `DMT_core-2.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DMT_core
-Version: 2.0.0
+Version: 2.1.0
 Summary: Device Modeling Toolkit Core
 Home-page: https://gitlab.com/dmt-development/dmt
 Author: M.Mueller, M.Krattenmacher
 Author-email: markus.mueller@semimod.de, mario.krattenmacher@semimod.de
 License: GNU GPLv3+
 Project-URL: Bug Tracker, https://gitlab.com/dmt-development/dmt
 Project-URL: Documentation, https://dmt-development.gitlab.io/dmt-core/
@@ -41,14 +41,18 @@
 
 [![logo](https://gitlab.com/uploads/-/system/project/avatar/33580822/DMT_Logo_wText.png)](https://gitlab.com/uploads/-/system/project/avatar/33580822/DMT_Logo_wText.png)
 
 DeviceModelingToolkit (DMT) is a Python tool targeted at helping modeling engineers extract model parameters, run circuit and TCAD simulations and automate their infrastructure.
 
 See the [DMT-website](https://dmt-development.gitlab.io/dmt-core/index.html) for further information.
 
+This project is funded by [NLnet](https://nlnet.nl/project/DMT-Core/) under the [NGI Zero Entrust fund](https://nlnet.nl/entrust/).
+
+<img src="pictures/banner_nlnet.svg" width="325"/>
+
 ## Usage
 
 ### Installation to virtual environment
 
 After installing python 3.8 or later, create a virtual environment and install the release version using
 
 ```bash
```

### Comparing `DMT_core-2.0.0/README.md` & `DMT_core-2.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 
 [![logo](https://gitlab.com/uploads/-/system/project/avatar/33580822/DMT_Logo_wText.png)](https://gitlab.com/uploads/-/system/project/avatar/33580822/DMT_Logo_wText.png)
 
 DeviceModelingToolkit (DMT) is a Python tool targeted at helping modeling engineers extract model parameters, run circuit and TCAD simulations and automate their infrastructure.
 
 See the [DMT-website](https://dmt-development.gitlab.io/dmt-core/index.html) for further information.
 
+This project is funded by [NLnet](https://nlnet.nl/project/DMT-Core/) under the [NGI Zero Entrust fund](https://nlnet.nl/entrust/).
+
+<img src="pictures/banner_nlnet.svg" width="325"/>
+
 ## Usage
 
 ### Installation to virtual environment
 
 After installing python 3.8 or later, create a virtual environment and install the release version using
 
 ```bash
```

### Comparing `DMT_core-2.0.0/setup.py` & `DMT_core-2.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "remote": ["paramiko", "scp"],
 }
 EXTRAS_REQUIRE["full"] = list(set(chain(*EXTRAS_REQUIRE.values())))
 EXTRAS_REQUIRE["full"].remove("PyQt5")  # not always needed
 
 setuptools.setup(
     name="DMT_core",
-    version="2.0.0",
+    version="2.1.0",
     author="M.Mueller, M.Krattenmacher",
     author_email="markus.mueller@semimod.de, mario.krattenmacher@semimod.de",
     description="Device Modeling Toolkit Core",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/dmt-development/dmt",
     project_urls={
@@ -59,10 +59,11 @@
         "pyyaml",
         "more_itertools",
         "semver",
         "verilogae>=0.9b4",
         "h5py",
         "cycler",
         "colormath",
+        "requests",
     ],
     extras_require=EXTRAS_REQUIRE,
 )
```

