# Comparing `tmp/DMT_extraction-1.0.0.tar.gz` & `tmp/DMT_extraction-1.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DMT_extraction-1.0.0.tar", last modified: Thu May 16 20:14:14 2024, max compression
+gzip compressed data, was "DMT_extraction-1.0.0rc2.tar", last modified: Thu May 16 20:00:54 2024, max compression
```

## Comparing `DMT_extraction-1.0.0.tar` & `DMT_extraction-1.0.0rc2.tar`

### file list

```diff
@@ -1,86 +1,87 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:14:14.840617 DMT_extraction-1.0.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:14:14.713617 DMT_extraction-1.0.0/DMT/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:14:14.739617 DMT_extraction-1.0.0/DMT/autodoc_template/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:14:14.740617 DMT_extraction-1.0.0/DMT/autodoc_template/base/
--rw-rw-rw-   0 root         (0) root         (0)     5557 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/autodoc_template/base/header.tex
--rw-rw-rw-   0 root         (0) root         (0)      948 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/autodoc_template/base/parameters.tex
--rw-rw-rw-   0 root         (0) root         (0)      527 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/autodoc_template/bib.bib
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:14:14.741617 DMT_extraction-1.0.0/DMT/autodoc_template/content/
--rw-rw-rw-   0 root         (0) root         (0)     1065 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/autodoc_template/content/conclusion.tex
--rw-rw-rw-   0 root         (0) root         (0)     1597 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/autodoc_template/content/deckblatt.tex
--rw-rw-rw-   0 root         (0) root         (0)     1082 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/autodoc_template/content/introduction.tex
--rw-rw-rw-   0 root         (0) root         (0)        6 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/autodoc_template/doc
--rw-rw-rw-   0 root         (0) root         (0)     1573 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/autodoc_template/documentation.tex
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:14:14.781617 DMT_extraction-1.0.0/DMT/extraction/
--rw-rw-rw-   0 root         (0) root         (0)     2970 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/extraction/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    28844 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/extraction/docu_xtraction.py
--rw-rw-rw-   0 root         (0) root         (0)     2270 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/extraction/extract_dimensions.py
--rw-rw-rw-   0 root         (0) root         (0)     2736 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/extraction/find_nearest.py
--rw-rw-rw-   0 root         (0) root         (0)    27127 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/extraction/generate_virtual_data.py
--rw-rw-rw-   0 root         (0) root         (0)     5004 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/extraction/get_poly_region.py
--rw-rw-rw-   0 root         (0) root         (0)     5641 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/extraction/ixbounds.py
--rw-rw-rw-   0 root         (0) root         (0)     4470 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/extraction/iynorm.py
--rw-rw-rw-   0 root         (0) root         (0)    10037 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/extraction/model.py
--rw-rw-rw-   0 root         (0) root         (0)     2320 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/extraction/model_diode.py
--rw-rw-rw-   0 root         (0) root         (0)    12037 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/extraction/mx_step.py
--rw-rw-rw-   0 root         (0) root         (0)    19114 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/extraction/mx_verify.py
--rw-rw-rw-   0 root         (0) root         (0)     7318 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/extraction/q_step.py
--rw-rw-rw-   0 root         (0) root         (0)      510 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/extraction/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     5766 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/extraction/x_diode.py
--rw-rw-rw-   0 root         (0) root         (0)     7032 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/extraction/x_res.py
--rw-rw-rw-   0 root         (0) root         (0)    94852 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/extraction/x_step.py
--rw-rw-rw-   0 root         (0) root         (0)    56480 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/extraction/x_verify.py
--rw-rw-rw-   0 root         (0) root         (0)    31586 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/extraction/x_verify_mmc.py
--rw-rw-rw-   0 root         (0) root         (0)    20238 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/extraction/x_verify_plots.py
--rw-rw-rw-   0 root         (0) root         (0)    49081 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/extraction/xq_poa.py
--rw-rw-rw-   0 root         (0) root         (0)    65732 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/extraction/xq_poa_bilinear_full.py
--rw-rw-rw-   0 root         (0) root         (0)    18999 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/extraction/xq_poa_bilinear_full_reg.py
--rw-rw-rw-   0 root         (0) root         (0)     9862 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/extraction/xq_poa_classic.py
--rw-rw-rw-   0 root         (0) root         (0)    10716 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/extraction/xq_poa_only_perimeter.py
--rw-rw-rw-   0 root         (0) root         (0)    24357 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/extraction/xq_poa_x.py
--rw-rw-rw-   0 root         (0) root         (0)     7997 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/extraction/xstep_parameter_table.py
--rw-rw-rw-   0 root         (0) root         (0)    20005 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/extraction/xtraction.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:14:14.828617 DMT_extraction-1.0.0/DMT/gui/
--rw-rw-rw-   0 root         (0) root         (0)     1130 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/gui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11858 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/gui/commands.py
--rw-rw-rw-   0 root         (0) root         (0)     1000 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/gui/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2322 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/gui/file_dialog.py
--rw-rw-rw-   0 root         (0) root         (0)    10948 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/gui/main_window.py
--rw-rw-rw-   0 root         (0) root         (0)    12256 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/gui/mcard_widget.py
--rw-rw-rw-   0 root         (0) root         (0)     4337 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/gui/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     5972 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/gui/x_step_gui.py
--rw-rw-rw-   0 root         (0) root         (0)    44380 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/gui/x_step_widget.py
--rw-rw-rw-   0 root         (0) root         (0)    18302 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/gui/xplot.py
--rw-rw-rw-   0 root         (0) root         (0)    12431 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/gui/xtraction_gui.py
--rw-rw-rw-   0 root         (0) root         (0)     8745 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/gui/xtraction_tree_view.py
--rw-rw-rw-   0 root         (0) root         (0)     8041 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/gui/xtraction_view.py
--rw-rw-rw-   0 root         (0) root         (0)     4927 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/gui/xtraction_view_ui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:14:14.838617 DMT_extraction-1.0.0/DMT/psp/
--rw-rw-rw-   0 root         (0) root         (0)     3049 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/psp/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14868 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/psp/mc_psp.py
--rw-rw-rw-   0 root         (0) root         (0)     6708 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/psp/psp_data_processor.py
--rw-rw-rw-   0 root         (0) root         (0)     5922 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/psp/psp_default_circuits.py
--rw-rw-rw-   0 root         (0) root         (0)     9921 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/psp/x_ccg.py
--rw-rw-rw-   0 root         (0) root         (0)    11157 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/psp/x_cgg.py
--rw-rw-rw-   0 root         (0) root         (0)     9588 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/psp/x_gds.py
--rw-rw-rw-   0 root         (0) root         (0)    10029 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/psp/x_gm.py
--rw-rw-rw-   0 root         (0) root         (0)     9278 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/psp/x_ib.py
--rw-rw-rw-   0 root         (0) root         (0)     9178 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/psp/x_ids_vd.py
--rw-rw-rw-   0 root         (0) root         (0)    12299 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/psp/x_ids_vg.py
--rw-rw-rw-   0 root         (0) root         (0)     9263 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/psp/x_ig.py
--rw-rw-rw-   0 root         (0) root         (0)    12067 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/psp/x_juncap_cap.py
--rw-rw-rw-   0 root         (0) root         (0)    12536 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/psp/x_juncap_current.py
--rw-rw-rw-   0 root         (0) root         (0)     9116 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/psp/x_y_rs.py
--rw-rw-rw-   0 root         (0) root         (0)     9097 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/DMT/psp/x_y_vt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:14:14.839617 DMT_extraction-1.0.0/DMT_extraction.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5155 2024-05-16 20:14:14.000000 DMT_extraction-1.0.0/DMT_extraction.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2033 2024-05-16 20:14:14.000000 DMT_extraction-1.0.0/DMT_extraction.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 20:14:14.000000 DMT_extraction-1.0.0/DMT_extraction.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      112 2024-05-16 20:14:14.000000 DMT_extraction-1.0.0/DMT_extraction.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2024-05-16 20:14:14.000000 DMT_extraction-1.0.0/DMT_extraction.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)    35190 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5155 2024-05-16 20:14:14.839617 DMT_extraction-1.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4335 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-16 20:13:03.000000 DMT_extraction-1.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-16 20:14:14.840617 DMT_extraction-1.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1259 2024-05-16 20:14:13.000000 DMT_extraction-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:00:54.456805 DMT_extraction-1.0.0rc2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:00:54.266806 DMT_extraction-1.0.0rc2/DMT/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:00:54.341805 DMT_extraction-1.0.0rc2/DMT/autodoc_template/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:00:54.343805 DMT_extraction-1.0.0rc2/DMT/autodoc_template/base/
+-rw-rw-rw-   0 root         (0) root         (0)     5557 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/autodoc_template/base/header.tex
+-rw-rw-rw-   0 root         (0) root         (0)      948 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/autodoc_template/base/parameters.tex
+-rw-rw-rw-   0 root         (0) root         (0)      527 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/autodoc_template/bib.bib
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:00:54.346805 DMT_extraction-1.0.0rc2/DMT/autodoc_template/content/
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/autodoc_template/content/conclusion.tex
+-rw-rw-rw-   0 root         (0) root         (0)     1597 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/autodoc_template/content/deckblatt.tex
+-rw-rw-rw-   0 root         (0) root         (0)     1082 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/autodoc_template/content/introduction.tex
+-rw-rw-rw-   0 root         (0) root         (0)        6 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/autodoc_template/doc
+-rw-rw-rw-   0 root         (0) root         (0)     1573 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/autodoc_template/documentation.tex
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:00:54.376805 DMT_extraction-1.0.0rc2/DMT/extraction/
+-rw-rw-rw-   0 root         (0) root         (0)     2970 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/extraction/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    28844 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/extraction/docu_xtraction.py
+-rw-rw-rw-   0 root         (0) root         (0)     2270 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/extraction/extract_dimensions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2736 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/extraction/find_nearest.py
+-rw-rw-rw-   0 root         (0) root         (0)    27127 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/extraction/generate_virtual_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     5004 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/extraction/get_poly_region.py
+-rw-rw-rw-   0 root         (0) root         (0)     5641 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/extraction/ixbounds.py
+-rw-rw-rw-   0 root         (0) root         (0)     4470 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/extraction/iynorm.py
+-rw-rw-rw-   0 root         (0) root         (0)    10037 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/extraction/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2320 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/extraction/model_diode.py
+-rw-rw-rw-   0 root         (0) root         (0)    12037 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/extraction/mx_step.py
+-rw-rw-rw-   0 root         (0) root         (0)    19114 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/extraction/mx_verify.py
+-rw-rw-rw-   0 root         (0) root         (0)     7318 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/extraction/q_step.py
+-rw-rw-rw-   0 root         (0) root         (0)      510 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/extraction/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     5766 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/extraction/x_diode.py
+-rw-rw-rw-   0 root         (0) root         (0)     7032 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/extraction/x_res.py
+-rw-rw-rw-   0 root         (0) root         (0)    94852 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/extraction/x_step.py
+-rw-rw-rw-   0 root         (0) root         (0)    56480 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/extraction/x_verify.py
+-rw-rw-rw-   0 root         (0) root         (0)    31586 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/extraction/x_verify_mmc.py
+-rw-rw-rw-   0 root         (0) root         (0)    20238 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/extraction/x_verify_plots.py
+-rw-rw-rw-   0 root         (0) root         (0)    49081 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/extraction/xq_poa.py
+-rw-rw-rw-   0 root         (0) root         (0)    65732 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/extraction/xq_poa_bilinear_full.py
+-rw-rw-rw-   0 root         (0) root         (0)    18999 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/extraction/xq_poa_bilinear_full_reg.py
+-rw-rw-rw-   0 root         (0) root         (0)     9862 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/extraction/xq_poa_classic.py
+-rw-rw-rw-   0 root         (0) root         (0)    10716 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/extraction/xq_poa_only_perimeter.py
+-rw-rw-rw-   0 root         (0) root         (0)    24357 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/extraction/xq_poa_x.py
+-rw-rw-rw-   0 root         (0) root         (0)     7997 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/extraction/xstep_parameter_table.py
+-rw-rw-rw-   0 root         (0) root         (0)    20005 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/extraction/xtraction.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:00:54.421805 DMT_extraction-1.0.0rc2/DMT/gui/
+-rw-rw-rw-   0 root         (0) root         (0)     1130 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/gui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11858 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/gui/commands.py
+-rw-rw-rw-   0 root         (0) root         (0)     1000 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/gui/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2322 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/gui/file_dialog.py
+-rw-rw-rw-   0 root         (0) root         (0)    10948 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/gui/main_window.py
+-rw-rw-rw-   0 root         (0) root         (0)    12256 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/gui/mcard_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)     4337 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/gui/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     5972 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/gui/x_step_gui.py
+-rw-rw-rw-   0 root         (0) root         (0)    44380 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/gui/x_step_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)    18302 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/gui/xplot.py
+-rw-rw-rw-   0 root         (0) root         (0)    12431 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/gui/xtraction_gui.py
+-rw-rw-rw-   0 root         (0) root         (0)     8745 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/gui/xtraction_tree_view.py
+-rw-rw-rw-   0 root         (0) root         (0)     8041 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/gui/xtraction_view.py
+-rw-rw-rw-   0 root         (0) root         (0)     4927 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/gui/xtraction_view_ui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:00:54.455805 DMT_extraction-1.0.0rc2/DMT/psp/
+-rw-rw-rw-   0 root         (0) root         (0)     3049 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/psp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14868 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/psp/mc_psp.py
+-rw-rw-rw-   0 root         (0) root         (0)     6708 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/psp/psp_data_processor.py
+-rw-rw-rw-   0 root         (0) root         (0)     5922 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/psp/psp_default_circuits.py
+-rw-rw-rw-   0 root         (0) root         (0)     9921 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/psp/x_ccg.py
+-rw-rw-rw-   0 root         (0) root         (0)    11157 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/psp/x_cgg.py
+-rw-rw-rw-   0 root         (0) root         (0)     9588 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/psp/x_gds.py
+-rw-rw-rw-   0 root         (0) root         (0)    10029 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/psp/x_gm.py
+-rw-rw-rw-   0 root         (0) root         (0)     9278 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/psp/x_ib.py
+-rw-rw-rw-   0 root         (0) root         (0)     9178 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/psp/x_ids_vd.py
+-rw-rw-rw-   0 root         (0) root         (0)    12299 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/psp/x_ids_vg.py
+-rw-rw-rw-   0 root         (0) root         (0)     9263 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/psp/x_ig.py
+-rw-rw-rw-   0 root         (0) root         (0)    12067 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/psp/x_juncap_cap.py
+-rw-rw-rw-   0 root         (0) root         (0)    12536 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/psp/x_juncap_current.py
+-rw-rw-rw-   0 root         (0) root         (0)     9116 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/psp/x_y_rs.py
+-rw-rw-rw-   0 root         (0) root         (0)     9097 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/DMT/psp/x_y_vt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:00:54.456805 DMT_extraction-1.0.0rc2/DMT_extraction.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      790 2024-05-16 20:00:54.000000 DMT_extraction-1.0.0rc2/DMT_extraction.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2074 2024-05-16 20:00:54.000000 DMT_extraction-1.0.0rc2/DMT_extraction.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 20:00:54.000000 DMT_extraction-1.0.0rc2/DMT_extraction.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2024-05-16 20:00:54.000000 DMT_extraction-1.0.0rc2/DMT_extraction.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      112 2024-05-16 20:00:54.000000 DMT_extraction-1.0.0rc2/DMT_extraction.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2024-05-16 20:00:54.000000 DMT_extraction-1.0.0rc2/DMT_extraction.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)    35190 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      790 2024-05-16 20:00:54.456805 DMT_extraction-1.0.0rc2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4335 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-16 19:59:40.000000 DMT_extraction-1.0.0rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-16 20:00:54.456805 DMT_extraction-1.0.0rc2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1295 2024-05-16 20:00:53.000000 DMT_extraction-1.0.0rc2/setup.py
```

### Comparing `DMT_extraction-1.0.0/DMT/autodoc_template/base/header.tex` & `DMT_extraction-1.0.0rc2/DMT/autodoc_template/base/header.tex`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/autodoc_template/base/parameters.tex` & `DMT_extraction-1.0.0rc2/DMT/autodoc_template/base/parameters.tex`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/autodoc_template/bib.bib` & `DMT_extraction-1.0.0rc2/DMT/autodoc_template/bib.bib`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/autodoc_template/content/conclusion.tex` & `DMT_extraction-1.0.0rc2/DMT/autodoc_template/content/conclusion.tex`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/autodoc_template/content/deckblatt.tex` & `DMT_extraction-1.0.0rc2/DMT/autodoc_template/content/deckblatt.tex`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/autodoc_template/content/introduction.tex` & `DMT_extraction-1.0.0rc2/DMT/autodoc_template/content/introduction.tex`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/autodoc_template/documentation.tex` & `DMT_extraction-1.0.0rc2/DMT/autodoc_template/documentation.tex`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/extraction/__init__.py` & `DMT_extraction-1.0.0rc2/DMT/extraction/__init__.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/extraction/docu_xtraction.py` & `DMT_extraction-1.0.0rc2/DMT/extraction/docu_xtraction.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/extraction/extract_dimensions.py` & `DMT_extraction-1.0.0rc2/DMT/extraction/extract_dimensions.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/extraction/find_nearest.py` & `DMT_extraction-1.0.0rc2/DMT/extraction/find_nearest.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/extraction/generate_virtual_data.py` & `DMT_extraction-1.0.0rc2/DMT/extraction/generate_virtual_data.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/extraction/get_poly_region.py` & `DMT_extraction-1.0.0rc2/DMT/extraction/get_poly_region.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/extraction/ixbounds.py` & `DMT_extraction-1.0.0rc2/DMT/extraction/ixbounds.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/extraction/iynorm.py` & `DMT_extraction-1.0.0rc2/DMT/extraction/iynorm.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/extraction/model.py` & `DMT_extraction-1.0.0rc2/DMT/extraction/model.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/extraction/model_diode.py` & `DMT_extraction-1.0.0rc2/DMT/extraction/model_diode.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/extraction/mx_step.py` & `DMT_extraction-1.0.0rc2/DMT/extraction/mx_step.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/extraction/mx_verify.py` & `DMT_extraction-1.0.0rc2/DMT/extraction/mx_verify.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/extraction/q_step.py` & `DMT_extraction-1.0.0rc2/DMT/extraction/q_step.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/extraction/x_diode.py` & `DMT_extraction-1.0.0rc2/DMT/extraction/x_diode.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/extraction/x_res.py` & `DMT_extraction-1.0.0rc2/DMT/extraction/x_res.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/extraction/x_step.py` & `DMT_extraction-1.0.0rc2/DMT/extraction/x_step.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/extraction/x_verify.py` & `DMT_extraction-1.0.0rc2/DMT/extraction/x_verify.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/extraction/x_verify_mmc.py` & `DMT_extraction-1.0.0rc2/DMT/extraction/x_verify_mmc.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/extraction/x_verify_plots.py` & `DMT_extraction-1.0.0rc2/DMT/extraction/x_verify_plots.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/extraction/xq_poa.py` & `DMT_extraction-1.0.0rc2/DMT/extraction/xq_poa.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/extraction/xq_poa_bilinear_full.py` & `DMT_extraction-1.0.0rc2/DMT/extraction/xq_poa_bilinear_full.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/extraction/xq_poa_bilinear_full_reg.py` & `DMT_extraction-1.0.0rc2/DMT/extraction/xq_poa_bilinear_full_reg.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/extraction/xq_poa_classic.py` & `DMT_extraction-1.0.0rc2/DMT/extraction/xq_poa_classic.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/extraction/xq_poa_only_perimeter.py` & `DMT_extraction-1.0.0rc2/DMT/extraction/xq_poa_only_perimeter.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/extraction/xq_poa_x.py` & `DMT_extraction-1.0.0rc2/DMT/extraction/xq_poa_x.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/extraction/xstep_parameter_table.py` & `DMT_extraction-1.0.0rc2/DMT/extraction/xstep_parameter_table.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/extraction/xtraction.py` & `DMT_extraction-1.0.0rc2/DMT/extraction/xtraction.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/gui/__init__.py` & `DMT_extraction-1.0.0rc2/DMT/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/gui/commands.py` & `DMT_extraction-1.0.0rc2/DMT/gui/commands.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/gui/config.py` & `DMT_extraction-1.0.0rc2/DMT/gui/config.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/gui/file_dialog.py` & `DMT_extraction-1.0.0rc2/DMT/gui/file_dialog.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/gui/main_window.py` & `DMT_extraction-1.0.0rc2/DMT/gui/main_window.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/gui/mcard_widget.py` & `DMT_extraction-1.0.0rc2/DMT/gui/mcard_widget.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/gui/utils.py` & `DMT_extraction-1.0.0rc2/DMT/gui/utils.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/gui/x_step_gui.py` & `DMT_extraction-1.0.0rc2/DMT/gui/x_step_gui.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/gui/x_step_widget.py` & `DMT_extraction-1.0.0rc2/DMT/gui/x_step_widget.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/gui/xplot.py` & `DMT_extraction-1.0.0rc2/DMT/gui/xplot.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/gui/xtraction_gui.py` & `DMT_extraction-1.0.0rc2/DMT/gui/xtraction_gui.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/gui/xtraction_tree_view.py` & `DMT_extraction-1.0.0rc2/DMT/gui/xtraction_tree_view.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/gui/xtraction_view.py` & `DMT_extraction-1.0.0rc2/DMT/gui/xtraction_view.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/gui/xtraction_view_ui.py` & `DMT_extraction-1.0.0rc2/DMT/gui/xtraction_view_ui.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/psp/__init__.py` & `DMT_extraction-1.0.0rc2/DMT/psp/__init__.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/psp/mc_psp.py` & `DMT_extraction-1.0.0rc2/DMT/psp/mc_psp.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/psp/psp_data_processor.py` & `DMT_extraction-1.0.0rc2/DMT/psp/psp_data_processor.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/psp/psp_default_circuits.py` & `DMT_extraction-1.0.0rc2/DMT/psp/psp_default_circuits.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/psp/x_ccg.py` & `DMT_extraction-1.0.0rc2/DMT/psp/x_ccg.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/psp/x_cgg.py` & `DMT_extraction-1.0.0rc2/DMT/psp/x_cgg.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/psp/x_gds.py` & `DMT_extraction-1.0.0rc2/DMT/psp/x_gds.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/psp/x_gm.py` & `DMT_extraction-1.0.0rc2/DMT/psp/x_gm.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/psp/x_ib.py` & `DMT_extraction-1.0.0rc2/DMT/psp/x_ib.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/psp/x_ids_vd.py` & `DMT_extraction-1.0.0rc2/DMT/psp/x_ids_vd.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/psp/x_ids_vg.py` & `DMT_extraction-1.0.0rc2/DMT/psp/x_ids_vg.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/psp/x_ig.py` & `DMT_extraction-1.0.0rc2/DMT/psp/x_ig.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/psp/x_juncap_cap.py` & `DMT_extraction-1.0.0rc2/DMT/psp/x_juncap_cap.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/psp/x_juncap_current.py` & `DMT_extraction-1.0.0rc2/DMT/psp/x_juncap_current.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/psp/x_y_rs.py` & `DMT_extraction-1.0.0rc2/DMT/psp/x_y_rs.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT/psp/x_y_vt.py` & `DMT_extraction-1.0.0rc2/DMT/psp/x_y_vt.py`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/DMT_extraction.egg-info/PKG-INFO` & `DMT_extraction-1.0.0rc2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: DMT-extraction
-Version: 1.0.0
-Summary: Device Modeling Toolkit extraction submodule
-Home-page: https://gitlab.com/dmt-development/dmt_extraction
-Author: SemiMod
-Author-email: mario.krattenmacher@semimod.de
-License: DMT License
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
-Description-Content-Type: text/markdown
-Provides-Extra: batch_mode
-Provides-Extra: pyside2
-Provides-Extra: pyside6
-License-File: LICENSE
-
 [![pyversion](https://img.shields.io/badge/python->3.6-blue?logo=python)](https://docs.python.org/3.8/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # DMT-extraction
 
 Device-Modeling Toolkit (DMT) is a Python framework used for compact model parameter extraction. 
 DMT-core is the main module that provides various routines useful for semiconductor device engineers that 
@@ -115,9 +93,7 @@
     - [2] N. Arora, "MOSFET Modeling for VLSI Simulation", World Scientific, 2007.
     - [3] J. Robinson, "A GENERAL FOUR-TERMINAL CHARGING-CURRENT MODEL FOR THE INSULATED-GATE FIELD-EFFECT TRANSISTOR - I", Solid State Electronics, vol. 23, pp. 405-410, 1980.
     - [4] H. Iwal et. al., "A Scaleable Technique for the Measurement of Intrinsic MOS Capacitance with Atto-Farad Resolution", IEEE Journal of Solid State Devices, 1985.
 
 # License
 
 This repository is licensed under the GPL, see the file LICENSE.
-
-
```

### Comparing `DMT_extraction-1.0.0/DMT_extraction.egg-info/SOURCES.txt` & `DMT_extraction-1.0.0rc2/DMT_extraction.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -67,9 +67,10 @@
 DMT/psp/x_juncap_cap.py
 DMT/psp/x_juncap_current.py
 DMT/psp/x_y_rs.py
 DMT/psp/x_y_vt.py
 DMT_extraction.egg-info/PKG-INFO
 DMT_extraction.egg-info/SOURCES.txt
 DMT_extraction.egg-info/dependency_links.txt
+DMT_extraction.egg-info/entry_points.txt
 DMT_extraction.egg-info/requires.txt
 DMT_extraction.egg-info/top_level.txt
```

### Comparing `DMT_extraction-1.0.0/LICENSE` & `DMT_extraction-1.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `DMT_extraction-1.0.0/setup.py` & `DMT_extraction-1.0.0rc2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import setuptools
 
-with open("README.md", "r") as fh:
-    long_description = fh.read()
+# import numpy
 
 setuptools.setup(
     name="DMT_extraction",
-    version="1.0.0",
+    version="1.0.0-rc.2",
     author="SemiMod",
     author_email="mario.krattenmacher@semimod.de",
     description="Device Modeling Toolkit extraction submodule",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
+    # long_description=long_description,
+    # long_description_content_type="text/markdown",
     url="https://gitlab.com/dmt-development/dmt_extraction",
     packages=setuptools.find_namespace_packages(include=["DMT.*"]),
     license="DMT License",
     classifiers=[
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
@@ -30,8 +29,9 @@
         "matplotlib",
     ],
     extras_require={
         "batch_mode": ["coloredlogs", "click"],
         "pyside2": ["PySide2"],
         "pyside6": ["PySide6"],
     },
+    entry_points={"console_scripts": ["dmt_batched = DMT.batchmode.cli:main"]},
 )
```

