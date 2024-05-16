# Comparing `tmp/module_qc_nonelec_gui-0.0.4.tar.gz` & `tmp/module_qc_nonelec_gui-0.0.5.tar.gz`

## Comparing `module_qc_nonelec_gui-0.0.4.tar` & `module_qc_nonelec_gui-0.0.5.tar`

### file list

```diff
@@ -1,159 +1,159 @@
--rw-r--r--   0        0        0     3272 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/.gitlab-ci.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/.gitmodules
--rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/MANIFEST.in
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/tbump.toml
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/docs/Makefile
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/docs/conf.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/docs/index.rst
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/docs/make.bat
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/__init__.py
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/__main__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/_version.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/config_modifier.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/GUI/__init__.py
--rw-r--r--   0        0        0    10387 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/GUI/choosetest_win.py
--rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/GUI/componentinfo_win.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/GUI/connectdb_win.py
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/GUI/connectpd_win.py
--rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/GUI/continue_win.py
--rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/GUI/inputatlsn_win.py
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/GUI/selectmode_win.py
--rw-r--r--   0        0        0     2995 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/GUI/setup_win.py
--rw-r--r--   0        0        0    73479 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/GUI/icon/ATLAS-Logo-BW-CMYK-LGBT-simple-transparent.png
--rw-r--r--   0        0        0   523993 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/GUI/icon/ATLAS-Logo-Blue-RGB-H_0.jpg
--rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/GUI/icon/Logo-Outline-web-Blue100.png
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/GUI/registration_bare_module/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/GUI/registration_bare_module/__init__.py
--rw-r--r--   0        0        0     2825 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/GUI/registration_bare_module/bareinfo_win.py
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/GUI/registration_bare_module/bareregist_main.py
--rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/GUI/registration_bare_module/bareregist_win.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/GUI/registration_bare_module/connectpd_win.py
--rw-r--r--   0        0        0     7189 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/GUI/registration_bare_module/feinfo_win.py
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/GUI/registration_bare_module/initial_win.py
--rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/GUI/registration_bare_module/sensorinfo_win.py
--rw-r--r--   0        0        0    56779 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/GUI/registration_bare_module/img/assembledmodule.jpg
--rw-r--r--   0        0        0    33023 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/GUI/registration_bare_module/img/baremodule.jpg
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/cli/__init__.py
--rw-r--r--   0        0        0    39184 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/cli/main.py
--rw-r--r--   0        0        0     7820 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/configuration/config_default.json
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/configuration/config_quad.json
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/configuration/config_triplet_r.json
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/configuration/config_triplet_s.json
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/dbinterface/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/dbinterface/__init__.py
--rw-r--r--   0        0        0     6495 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/dbinterface/db_write.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/dbinterface/localdb_authenticator.py
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/dbinterface/localdb_retriever.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/dbinterface/localdb_uploader.py
--rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/dbinterface/upload_results_sample.py
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/dbinterface/bin/uploader_sample.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/dbinterface/data/sample_results.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/FLATNESS/__init__.py
--rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/FLATNESS/confirm.py
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/FLATNESS/main.py
--rw-r--r--   0        0        0     4682 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/FLATNESS/user_input.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/FLATNESS/example/example.json
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE/__init__.py
--rw-r--r--   0        0        0     4099 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE/confirm.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE/main.py
--rw-r--r--   0        0        0     5441 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE/user_input.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE/example/example.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE/example/jsonschema/tmp
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE/example/jsonschema/validation_schema.json
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE_BARE/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE_BARE/__init__.py
--rw-r--r--   0        0        0     4237 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE_BARE/confirm.py
--rw-r--r--   0        0        0     8703 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE_BARE/function.py
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE_BARE/main.py
--rw-r--r--   0        0        0     7231 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE_BARE/user_input.py
--rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE_BARE/example/example.dat
--rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE_BARE/example/example.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE_BARE/example/jsonschema/tmp
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE_BARE/example/jsonschema/validation_schema.json
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/MASS_MEASUREMENT/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/MASS_MEASUREMENT/__init__.py
--rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/MASS_MEASUREMENT/confirm.py
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/MASS_MEASUREMENT/main.py
--rw-r--r--   0        0        0     5144 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/MASS_MEASUREMENT/user_input.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/QUAD_MODULE_METROLOGY/__init__.py
--rw-r--r--   0        0        0     4449 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/QUAD_MODULE_METROLOGY/confirm.py
--rw-r--r--   0        0        0     7157 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/QUAD_MODULE_METROLOGY/initial_metrology.py
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/QUAD_MODULE_METROLOGY/main.py
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/QUAD_MODULE_METROLOGY/example/db.csv
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/QUAD_MODULE_METROLOGY/example/db.json
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/QUAD_MODULE_METROLOGY/example/db_new.csv
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/QUAD_MODULE_METROLOGY/example/db_new.json
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/QUAD_MODULE_METROLOGY/example/practice.txt
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/THERMAL_CYCLING/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/THERMAL_CYCLING/__init__.py
--rw-r--r--   0        0        0     5672 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/THERMAL_CYCLING/confirm.py
--rw-r--r--   0        0        0     7890 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/THERMAL_CYCLING/initial_Thermal.py
--rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/THERMAL_CYCLING/main.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/THERMAL_CYCLING/example/practice.txt
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/__init__.py
--rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/checklist.py
--rw-r--r--   0        0        0    35511 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/checklist_Module.py
--rw-r--r--   0        0        0    81372 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/checklist_PCB.py
--rw-r--r--   0        0        0     7445 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/confirm.py
--rw-r--r--   0        0        0    18290 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/inspection_win.py
--rw-r--r--   0        0        0    15434 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/main.py
--rw-r--r--   0        0        0    54946 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/shaping_win.py
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/splitimg_win.py
--rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/summary_win.py
--rw-r--r--   0        0        0     5332 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/vi_initial_win.py
--rw-r--r--   0        0        0     4262 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/VI_Config_Module.json
--rw-r--r--   0        0        0     8934 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/VI_Config_Module_MODULETOPCB.json
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_BARE_MODULE_BAREMODULERECEPTION.json
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_BARE_MODULE_default.json
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_MODULE_MODULE__ASSEMBLY.json
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_MODULE_MODULE__PARYLENE_COATING.json
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_MODULE_MODULE__PARYLENE_MASKING.json
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_MODULE_MODULE__PARYLENE_UNMASKING.json
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_MODULE_MODULE__THERMAL_CYCLES.json
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_MODULE_MODULE__WIREBONDING.json
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_MODULE_MODULE__WIREBOND_PROTECTION.json
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_MODULE_default.json
--rw-r--r--   0        0        0     9592 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_PCB.json
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_PCB_PCB_POPULATION.json
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_PCB_PCB_RECEPTION.json
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_PCB_default.json
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/reference_MODULE_MODULE__ASSEMBLY.json
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/reference_MODULE_MODULE__PARYLENE_COATING.json
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/reference_MODULE_MODULE__PARYLENE_MASKING.json
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/reference_MODULE_MODULE__PARYLENE_UNMASKING.json
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/reference_MODULE_MODULE__THERMAL_CYCLES.json
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/reference_MODULE_MODULE__WIREBONDING.json
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/reference_MODULE_MODULE__WIREBOND_PROTECTION.json
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/reference_PCB.json
--rw-r--r--   0        0        0     8066 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/functions/auto_trim.py
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/functions/cv2_func.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/WIREBOND_PULL_TEST/README.md
--rw-r--r--   0        0        0     3651 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/WIREBOND_PULL_TEST/confirm.py
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/WIREBOND_PULL_TEST/main.py
--rw-r--r--   0        0        0     8851 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/WIREBOND_PULL_TEST/user_input.py
--rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/glue_info_module_flex/Glue_info.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/glue_info_module_flex/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/glue_info_module_flex/__init__.py
--rw-r--r--   0        0        0     5610 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/glue_info_module_flex/confirm.py
--rw-r--r--   0        0        0     8228 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/glue_info_module_flex/initial_Glue_info.py
--rw-r--r--   0        0        0     7546 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/parylene_properties/Parylene_prop.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/parylene_properties/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/parylene_properties/__init__.py
--rw-r--r--   0        0        0     6090 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/parylene_properties/confirm.py
--rw-r--r--   0        0        0     9286 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/parylene_properties/initial_Parylene_prop.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/wirebonding_info/README.md
--rw-r--r--   0        0        0     5685 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/wirebonding_info/Wire_info.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/wirebonding_info/__init__.py
--rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/wirebonding_info/confirm.py
--rw-r--r--   0        0        0     9595 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/wirebonding_info/initial_Wire_info.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/wirebonding_info/example/practice.txt
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/tests/test_package.py
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/.gitignore
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/LICENSE
--rw-r--r--   0        0        0     5625 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/README.md
--rw-r--r--   0        0        0     6714 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     9356 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     3272 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/.gitlab-ci.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/.gitmodules
+-rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/MANIFEST.in
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/tbump.toml
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/docs/Makefile
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/docs/conf.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/docs/index.rst
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/docs/make.bat
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/__init__.py
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/__main__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/_version.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/config_modifier.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/GUI/__init__.py
+-rw-r--r--   0        0        0    10472 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/GUI/choosetest_win.py
+-rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/GUI/componentinfo_win.py
+-rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/GUI/connectdb_win.py
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/GUI/connectpd_win.py
+-rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/GUI/continue_win.py
+-rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/GUI/inputatlsn_win.py
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/GUI/selectmode_win.py
+-rw-r--r--   0        0        0     2995 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/GUI/setup_win.py
+-rw-r--r--   0        0        0    73479 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/GUI/icon/ATLAS-Logo-BW-CMYK-LGBT-simple-transparent.png
+-rw-r--r--   0        0        0   523993 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/GUI/icon/ATLAS-Logo-Blue-RGB-H_0.jpg
+-rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/GUI/icon/Logo-Outline-web-Blue100.png
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/GUI/registration_bare_module/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/GUI/registration_bare_module/__init__.py
+-rw-r--r--   0        0        0     2825 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/GUI/registration_bare_module/bareinfo_win.py
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/GUI/registration_bare_module/bareregist_main.py
+-rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/GUI/registration_bare_module/bareregist_win.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/GUI/registration_bare_module/connectpd_win.py
+-rw-r--r--   0        0        0     7189 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/GUI/registration_bare_module/feinfo_win.py
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/GUI/registration_bare_module/initial_win.py
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/GUI/registration_bare_module/sensorinfo_win.py
+-rw-r--r--   0        0        0    56779 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/GUI/registration_bare_module/img/assembledmodule.jpg
+-rw-r--r--   0        0        0    33023 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/GUI/registration_bare_module/img/baremodule.jpg
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/cli/__init__.py
+-rw-r--r--   0        0        0    41491 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/cli/main.py
+-rw-r--r--   0        0        0     7820 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/configuration/config_default.json
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/configuration/config_quad.json
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/configuration/config_triplet_r.json
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/configuration/config_triplet_s.json
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/dbinterface/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/dbinterface/__init__.py
+-rw-r--r--   0        0        0     6495 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/dbinterface/db_write.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/dbinterface/localdb_authenticator.py
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/dbinterface/localdb_retriever.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/dbinterface/localdb_uploader.py
+-rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/dbinterface/upload_results_sample.py
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/dbinterface/bin/uploader_sample.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/dbinterface/data/sample_results.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/FLATNESS/__init__.py
+-rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/FLATNESS/confirm.py
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/FLATNESS/main.py
+-rw-r--r--   0        0        0     4682 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/FLATNESS/user_input.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/FLATNESS/example/example.json
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE/__init__.py
+-rw-r--r--   0        0        0     4099 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE/confirm.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE/main.py
+-rw-r--r--   0        0        0     5441 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE/user_input.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE/example/example.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE/example/jsonschema/tmp
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE/example/jsonschema/validation_schema.json
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE_BARE/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE_BARE/__init__.py
+-rw-r--r--   0        0        0     4237 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE_BARE/confirm.py
+-rw-r--r--   0        0        0     8703 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE_BARE/function.py
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE_BARE/main.py
+-rw-r--r--   0        0        0     7231 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE_BARE/user_input.py
+-rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE_BARE/example/example.dat
+-rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE_BARE/example/example.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE_BARE/example/jsonschema/tmp
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE_BARE/example/jsonschema/validation_schema.json
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/MASS_MEASUREMENT/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/MASS_MEASUREMENT/__init__.py
+-rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/MASS_MEASUREMENT/confirm.py
+-rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/MASS_MEASUREMENT/main.py
+-rw-r--r--   0        0        0     5144 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/MASS_MEASUREMENT/user_input.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/QUAD_MODULE_METROLOGY/__init__.py
+-rw-r--r--   0        0        0     4449 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/QUAD_MODULE_METROLOGY/confirm.py
+-rw-r--r--   0        0        0     7157 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/QUAD_MODULE_METROLOGY/initial_metrology.py
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/QUAD_MODULE_METROLOGY/main.py
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/QUAD_MODULE_METROLOGY/example/db.csv
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/QUAD_MODULE_METROLOGY/example/db.json
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/QUAD_MODULE_METROLOGY/example/db_new.csv
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/QUAD_MODULE_METROLOGY/example/db_new.json
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/QUAD_MODULE_METROLOGY/example/practice.txt
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/THERMAL_CYCLING/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/THERMAL_CYCLING/__init__.py
+-rw-r--r--   0        0        0     5672 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/THERMAL_CYCLING/confirm.py
+-rw-r--r--   0        0        0     7890 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/THERMAL_CYCLING/initial_Thermal.py
+-rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/THERMAL_CYCLING/main.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/THERMAL_CYCLING/example/practice.txt
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/__init__.py
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/checklist.py
+-rw-r--r--   0        0        0    35511 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/checklist_Module.py
+-rw-r--r--   0        0        0    81372 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/checklist_PCB.py
+-rw-r--r--   0        0        0     7903 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/confirm.py
+-rw-r--r--   0        0        0    18842 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/inspection_win.py
+-rw-r--r--   0        0        0    15502 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/main.py
+-rw-r--r--   0        0        0    55997 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/shaping_win.py
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/splitimg_win.py
+-rw-r--r--   0        0        0     5303 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/summary_win.py
+-rw-r--r--   0        0        0     5402 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/vi_initial_win.py
+-rw-r--r--   0        0        0     4262 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/VI_Config_Module.json
+-rw-r--r--   0        0        0     8934 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/VI_Config_Module_MODULETOPCB.json
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_BARE_MODULE_BAREMODULERECEPTION.json
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_BARE_MODULE_default.json
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_MODULE_MODULE__ASSEMBLY.json
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_MODULE_MODULE__PARYLENE_COATING.json
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_MODULE_MODULE__PARYLENE_MASKING.json
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_MODULE_MODULE__PARYLENE_UNMASKING.json
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_MODULE_MODULE__THERMAL_CYCLES.json
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_MODULE_MODULE__WIREBONDING.json
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_MODULE_MODULE__WIREBOND_PROTECTION.json
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_MODULE_default.json
+-rw-r--r--   0        0        0     9592 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_PCB.json
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_PCB_PCB_POPULATION.json
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_PCB_PCB_RECEPTION.json
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_PCB_default.json
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/reference_MODULE_MODULE__ASSEMBLY.json
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/reference_MODULE_MODULE__PARYLENE_COATING.json
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/reference_MODULE_MODULE__PARYLENE_MASKING.json
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/reference_MODULE_MODULE__PARYLENE_UNMASKING.json
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/reference_MODULE_MODULE__THERMAL_CYCLES.json
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/reference_MODULE_MODULE__WIREBONDING.json
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/reference_MODULE_MODULE__WIREBOND_PROTECTION.json
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/reference_PCB.json
+-rw-r--r--   0        0        0     8066 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/functions/auto_trim.py
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/functions/cv2_func.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/WIREBOND_PULL_TEST/README.md
+-rw-r--r--   0        0        0     3651 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/WIREBOND_PULL_TEST/confirm.py
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/WIREBOND_PULL_TEST/main.py
+-rw-r--r--   0        0        0     8851 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/WIREBOND_PULL_TEST/user_input.py
+-rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/glue_info_module_flex/Glue_info.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/glue_info_module_flex/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/glue_info_module_flex/__init__.py
+-rw-r--r--   0        0        0     5610 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/glue_info_module_flex/confirm.py
+-rw-r--r--   0        0        0     8228 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/glue_info_module_flex/initial_Glue_info.py
+-rw-r--r--   0        0        0     7546 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/parylene_properties/Parylene_prop.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/parylene_properties/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/parylene_properties/__init__.py
+-rw-r--r--   0        0        0     6090 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/parylene_properties/confirm.py
+-rw-r--r--   0        0        0     9286 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/parylene_properties/initial_Parylene_prop.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/wirebonding_info/README.md
+-rw-r--r--   0        0        0     5685 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/wirebonding_info/Wire_info.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/wirebonding_info/__init__.py
+-rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/wirebonding_info/confirm.py
+-rw-r--r--   0        0        0     9595 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/wirebonding_info/initial_Wire_info.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/wirebonding_info/example/practice.txt
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/tests/test_package.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/LICENSE
+-rw-r--r--   0        0        0     5625 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/README.md
+-rw-r--r--   0        0        0     6714 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     9356 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.5/PKG-INFO
```

### Comparing `module_qc_nonelec_gui-0.0.4/.gitlab-ci.yml` & `module_qc_nonelec_gui-0.0.5/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/.pre-commit-config.yaml` & `module_qc_nonelec_gui-0.0.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/tbump.toml` & `module_qc_nonelec_gui-0.0.5/tbump.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 00000000: 5b76 6572 7369 6f6e 5d0a 6375 7272 656e  [version].curren
-00000010: 7420 3d20 2230 2e30 2e34 220a 0a23 2045  t = "0.0.4"..# E
+00000010: 7420 3d20 2230 2e30 2e35 220a 0a23 2045  t = "0.0.5"..# E
 00000020: 7861 6d70 6c65 206f 6620 6120 7365 6d76  xample of a semv
 00000030: 6572 2072 6567 6578 702e 0a23 204d 616b  er regexp..# Mak
 00000040: 6520 7375 7265 2074 6869 7320 6d61 7463  e sure this matc
 00000050: 6865 7320 6375 7272 656e 745f 7665 7273  hes current_vers
 00000060: 696f 6e20 6265 666f 7265 0a23 2075 7369  ion before.# usi
 00000070: 6e67 2074 6275 6d70 0a72 6567 6578 203d  ng tbump.regex =
 00000080: 2027 2727 0a20 2028 3f50 3c6d 616a 6f72   '''.  (?P<major
@@ -15,15 +15,15 @@
 000000e0: 2029 3f0a 2020 2727 270a 0a5b 6769 745d   )?.  '''..[git]
 000000f0: 0a23 2054 6865 2063 7572 7265 6e74 2076  .# The current v
 00000100: 6572 7369 6f6e 2077 696c 6c20 6765 7420  ersion will get 
 00000110: 7570 6461 7465 6420 7768 656e 2074 6275  updated when tbu
 00000120: 6d70 2069 7320 7275 6e0a 6d65 7373 6167  mp is run.messag
 00000130: 655f 7465 6d70 6c61 7465 203d 2022 4275  e_template = "Bu
 00000140: 6d70 2076 6572 7369 6f6e 3a20 302e 302e  mp version: 0.0.
-00000150: 3420 e286 9220 7b6e 6577 5f76 6572 7369  4 ... {new_versi
+00000150: 3520 e286 9220 7b6e 6577 5f76 6572 7369  5 ... {new_versi
 00000160: 6f6e 7d22 0a74 6167 5f74 656d 706c 6174  on}".tag_templat
 00000170: 6520 3d20 2276 7b6e 6577 5f76 6572 7369  e = "v{new_versi
 00000180: 6f6e 7d22 0a0a 2320 466f 7220 6561 6368  on}"..# For each
 00000190: 2066 696c 6520 746f 2070 6174 6368 2c20   file to patch, 
 000001a0: 6164 6420 6120 5b5b 6669 6c65 5d5d 2063  add a [[file]] c
 000001b0: 6f6e 6669 670a 2320 7365 6374 696f 6e20  onfig.# section 
 000001c0: 636f 6e74 6169 6e69 6e67 2074 6865 2070  containing the p
```

### Comparing `module_qc_nonelec_gui-0.0.4/docs/Makefile` & `module_qc_nonelec_gui-0.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/docs/conf.py` & `module_qc_nonelec_gui-0.0.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/docs/make.bat` & `module_qc_nonelec_gui-0.0.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/__main__.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/__main__.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/config_modifier.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/config_modifier.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/GUI/choosetest_win.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/GUI/choosetest_win.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,17 @@
 
 
 class ChooseTestWindow(QWidget):
     def __init__(self, parent=None):
         super(QWidget, self).__init__()
         self.parent = parent
 
+        self.setMinimumWidth(400)
+        self.setMinimumHeight(500)
+
         label_choosetest = QLabel()
         label_choosetest.setText('<center><font size="6"> Select Test</font></center>')
 
         next_button = QPushButton("&Next")
         next_button.clicked.connect(self.next_page)
         back_button = QPushButton("&Back")
         back_button.clicked.connect(self.back_page)
@@ -136,19 +139,19 @@
 
         if self.parent.isPractice:
             form_text.setStyleSheet("color: rgb black; background-color:linen;")
             status = "Practice"
         else:
             try:
                 stage = self.parent.info_dict["currentStage"]
-                status = self.parent.qcStatus["QC_results"][stage]
+                status = self.parent.qcStatus["QC_results"][stage][test_to_check]
                 log.info("check_uploaded(): " + pprint.pformat(test_to_check))
                 log.info("check_uploaded(): " + pprint.pformat(status))
 
-                if status == "-1":
+                if status != "-1":
                     form_text.setStyleSheet("color: black; background-color:linen;")
                     status = "Already uploaded"
                 else:
                     form_text.setStyleSheet("color: red; background-color:linen;")
                     status = "N/A"
 
                 # self.make_subwin(label_text, upload_status)
```

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/GUI/componentinfo_win.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/GUI/componentinfo_win.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/GUI/connectdb_win.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/GUI/connectdb_win.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 
 
 class ConnectDBWindow(QWidget):
     def __init__(self, parent=None):
         super(QWidget, self).__init__()
         self.parent = parent
 
+        self.setMinimumWidth(340)
+        self.setMinimumHeight(200)
+
         layout = QVBoxLayout()
         hbox_bottom = QHBoxLayout()
         edit_form = QFormLayout()
         form_box = QHBoxLayout()
 
         label_text = QLabel()
         label_text.setText('<center><font size="7">Log in to Local DB</font></center>')
```

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/GUI/connectpd_win.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/GUI/connectpd_win.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/GUI/continue_win.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/GUI/continue_win.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,17 @@
 
 
 class ContinueWindow(QWidget):
     def __init__(self, parent=None):
         super(QWidget, self).__init__()
         self.parent = parent
 
+        self.setMinimumWidth(400)
+        self.setMinimumHeight(500)
+
         layout = QVBoxLayout()
         yn_box = QHBoxLayout()
         yn_hbox = QHBoxLayout()
         where_box = QHBoxLayout()
         where_vbox = QVBoxLayout()
         button_box = QHBoxLayout()
```

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/GUI/inputatlsn_win.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/GUI/inputatlsn_win.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 
 
 class InitialWindow(QWidget):
     def __init__(self, parent=None):
         super(QWidget, self).__init__()
         self.parent = parent
 
+        self.setMinimumWidth(340)
+        self.setMinimumHeight(200)
+
         layout = QVBoxLayout()
         form_layout = QFormLayout()
         button_box = QHBoxLayout()
 
         label_text = QLabel()
         label_text.setText(
             '<center><font size="6">Input ATLAS Serial Number</font></center>'
```

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/GUI/selectmode_win.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/GUI/selectmode_win.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/GUI/setup_win.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/GUI/setup_win.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/GUI/icon/ATLAS-Logo-BW-CMYK-LGBT-simple-transparent.png` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/GUI/icon/ATLAS-Logo-BW-CMYK-LGBT-simple-transparent.png`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/GUI/icon/ATLAS-Logo-Blue-RGB-H_0.jpg` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/GUI/icon/ATLAS-Logo-Blue-RGB-H_0.jpg`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/GUI/icon/Logo-Outline-web-Blue100.png` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/GUI/icon/Logo-Outline-web-Blue100.png`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/GUI/registration_bare_module/bareinfo_win.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/GUI/registration_bare_module/bareinfo_win.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/GUI/registration_bare_module/bareregist_main.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/GUI/registration_bare_module/bareregist_main.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/GUI/registration_bare_module/bareregist_win.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/GUI/registration_bare_module/bareregist_win.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/GUI/registration_bare_module/connectpd_win.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/GUI/registration_bare_module/connectpd_win.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/GUI/registration_bare_module/feinfo_win.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/GUI/registration_bare_module/feinfo_win.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/GUI/registration_bare_module/initial_win.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/GUI/registration_bare_module/initial_win.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/GUI/registration_bare_module/sensorinfo_win.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/GUI/registration_bare_module/sensorinfo_win.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/GUI/registration_bare_module/img/assembledmodule.jpg` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/GUI/registration_bare_module/img/assembledmodule.jpg`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/GUI/registration_bare_module/img/baremodule.jpg` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/GUI/registration_bare_module/img/baremodule.jpg`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/cli/main.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/cli/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from datetime import date, datetime, timezone
 from importlib import machinery
 from pathlib import Path
 
 import itkdb
 import requests
 from bson.objectid import ObjectId
+from PyQt5 import QtCore
 from PyQt5.QtGui import qt_set_sequence_auto_mnemonic
 from PyQt5.QtWidgets import (
     QApplication,
     QDesktopWidget,
     QFormLayout,
     QHBoxLayout,
     QLabel,
@@ -129,14 +130,17 @@
         self.confirm_wid = None
         self.json_wid = None
         self.continue_wid = None
 
         self.init_ui()
 
     def init_ui(self):
+        # self.setWindowFlags(QtCore.Qt.Window | QtCore.Qt.CustomizeWindowHint | QtCore.Qt.WindowStaysOnTopHint)
+        self.setWindowFlags(QtCore.Qt.WindowStaysOnTopHint)
+
         # configuration1
         try:
             log.info("loading custom json file...")
             with Path(
                 self.module_qc_nonelec_gui_dir + "/configuration/custom.json"
             ).open(encoding="utf-8") as f:
                 self.custom_conf = json.load(f)
@@ -162,15 +166,19 @@
         self.config = self.default_conf
 
         if self.isSameComponent:
             self.fill_info()
 
         else:
             self.connectdb_wid = connectdb_win.ConnectDBWindow(self)
-            self.update_widget(self.connectdb_wid)
+            self.update_widget(
+                self.connectdb_wid,
+                self.connectdb_wid.sizeHint().width(),
+                self.connectdb_wid.sizeHint().height(),
+            )
             # wid = selectmode_win.SelectmodeWindow(self)
             # self.update_widget(wid)
             # log.info(
             #    "\n---------------------------------------------------------------"
             # )
 
     def set_windowsize(self, x, y):
@@ -236,22 +244,30 @@
         if mode == 0:
             self.login_localdb()
         elif mode == 1:
             self.update_widget(connectpd_win.ConnectPDWindow(self))
 
     def login_localdb(self):
         self.connectdb_wid = connectdb_win.ConnectDBWindow(self)
-        self.update_widget(self.connectdb_wid)
+        self.update_widget(
+            self.connectdb_wid,
+            self.connectdb_wid.sizeHint().width(),
+            self.connectdb_wid.sizeHint().height(),
+        )
 
     def start_QCupload(self):
         if self.isPractice and self.token == 0:
             self.practice_pd()
         else:
             self.inputatlsn_wid = inputatlsn_win.InitialWindow(self)
-            self.update_widget(self.inputatlsn_wid)
+            self.update_widget(
+                self.inputatlsn_wid,
+                self.inputatlsn_wid.sizeHint().width(),
+                self.inputatlsn_wid.sizeHint().height(),
+            )
 
     def start_bareregist_main(self):
         self.baremodeule_win = bareregist_main.MainWindow(self)
         self.call_another_window(self.baremodeule_win)
 
     def receive_atlsn(self, sn):
         self.atlsn = sn
@@ -439,15 +455,19 @@
         self.fill_practice_testtype_dict()
         if self.isPractice and self.token == 0:
             self.institute_dict = {"practice": "Practice"}
         self.see_info()
 
     def see_info(self):
         self.componentinfo_wid = componentinfo_win.ComponentInfoWindow(self)
-        self.update_widget(self.componentinfo_wid)
+        self.update_widget(
+            self.componentinfo_wid,
+            self.componentinfo_wid.sizeHint().width(),
+            self.componentinfo_wid.sizeHint().height(),
+        )
 
     def back_from_componentinfo(self):
         self.isSameComponent = False
         if self.isPractice and self.token == 0:
             self.call_selectmode()
         else:
             self.start_QCupload()
@@ -455,15 +475,19 @@
     def typebranch(self):
         if self.isPractice:
             if (
                 self.info_dict["componentType"] in self.supportedComponentTypes
                 or self.info_dict["componentType"] == "practice"
             ):
                 self.connectdb_wid = connectdb_win.ConnectDBWindow(self)
-                self.update_widget(self.connectdb_wid)
+                self.update_widget(
+                    self.connectdb_wid,
+                    self.connectdb_wid.sizeHint().width(),
+                    self.connectdb_wid.sizeHint().height(),
+                )
             else:
                 QMessageBox.critical(
                     None,
                     "Warning",
                     " ComponentType:"
                     + self.info_dict["componentType"]
                     + " is not supported now. ",
@@ -474,15 +498,19 @@
                 self.info_dict["componentType"] in self.supportedComponentTypes
                 or self.info_dict["componentType"] == "practice"
             ):
                 if self.isSameUser:
                     self.choose_test()
                 else:
                     self.connectdb_wid = connectdb_win.ConnectDBWindow(self)
-                    self.update_widget(self.connectdb_wid)
+                    self.update_widget(
+                        self.connectdb_wid,
+                        self.connectdb_wid.sizeHint().width(),
+                        self.connectdb_wid.sizeHint().height(),
+                    )
             else:
                 QMessageBox.critical(
                     None,
                     "Warning",
                     " ComponentType:"
                     + self.info_dict["componentType"]
                     + " is not supported now. ",
@@ -519,15 +547,19 @@
                 None,
                 "Warning",
                 "Failed in LocalDB User Authentication",
                 QMessageBox.Ok,
             )
 
             self.connectdb_wid = connectdb_win.ConnectDBWindow(self)
-            self.update_widget(self.connectdb_wid)
+            self.update_widget(
+                self.connectdb_wid,
+                self.connectdb_wid.sizeHint().width(),
+                self.connectdb_wid.sizeHint().height(),
+            )
 
     def choose_test(self):
         self.info_dict["user"] = self.db_user
 
         if (
             self.info_dict["componentType"] in self.supportedComponentTypes
             or self.info_dict["componentType"] == "practice"
@@ -557,49 +589,66 @@
                 self.localDB_dict["component"] = self.module_id
                 self.localDB_dict["currentStage"] = self.info_dict["currentStage"]
                 self.localDB_dict["user"] = self.user_info["name"]
                 self.fill_testtype_dict()
 
                 try:
                     self.choosetest_wid = choosetest_win.ChooseTestWindow(self)
-                    self.update_widget(self.choosetest_wid)
+                    self.update_widget(
+                        self.choosetest_wid,
+                        self.choosetest_wid.sizeHint().width(),
+                        self.choosetest_wid.sizeHint().height(),
+                    )
+
                 except Exception as e:
                     QMessageBox.warning(
                         None,
                         "Warning",
                         str(e),
                     )
                     self.inputatlsn_wid = inputatlsn_win.InitialWindow(self)
-                    self.update_widget(self.inputatlsn_wid)
+                    self.update_widget(
+                        self.inputatlsn_wid,
+                        self.inputatlsn_wid.sizeHint().width(),
+                        self.inputatlsn_wid.sizeHint().height(),
+                    )
             except Exception:
                 log.exception(traceback.format_exc())
                 msgBox = QMessageBox.warning(
                     None,
                     "Warning",
                     "Authentication failed or LocalDB not ready. Do you want to continue as practice mode?",
                     QMessageBox.Yes | QMessageBox.No,
                 )
                 if msgBox == QMessageBox.Yes:
                     self.isPractice = True
                     self.practice_choosetest()
                 elif msgBox == QMessageBox.No:
                     self.isPractice = False
                     self.connectdb_wid = connectdb_win.ConnectDBWindow(self)
-                    self.update_widget(self.connectdb_wid)
+                    self.update_widget(
+                        self.connectdb_wid,
+                        self.connectdb_wid.sizeHint().width(),
+                        self.connectdb_wid.sizeHint().height(),
+                    )
 
     def practice_choosetest(self):
         self.info_dict["user"] = "practice"
         self.localDB_dict["component"] = "practice"
         self.localDB_dict["currentStage"] = "practice"
         self.localDB_dict["user"] = "practice"
         self.localDB_dict["address"] = "practice"
         self.localDB_dict["stage"] = "practice"
 
         self.choosetest_wid = choosetest_win.ChooseTestWindow(self)
-        self.update_widget(self.choosetest_wid)
+        self.update_widget(
+            self.choosetest_wid,
+            self.choosetest_wid.sizeHint().width(),
+            self.choosetest_wid.sizeHint().height(),
+        )
 
     def back_from_test(self):
         if (
             self.info_dict["componentType"] in self.supportedComponentTypes
             or self.info_dict["componentType"] == "practice"
         ):
             self.moduleQC_choose_test()
@@ -744,15 +793,19 @@
             log.info(f"test_confirm = {test_confirm}")
 
             self.confirm_module = machinery.SourceFileLoader(
                 "confirm", test_confirm
             ).load_module()
             self.confirm_wid = self.confirm_module.ConfirmWindow(self)
 
-            self.update_widget(self.confirm_wid)
+            self.update_widget(
+                self.confirm_wid,
+                self.confirm_wid.sizeHint().width(),
+                self.confirm_wid.sizeHint().height(),
+            )
 
         #        except(FileNotFoundError,self.confirm_module.NotSupportedError):
         except Exception:
             log.exception(traceback.format_exc())
             try:
                 test_confirm = Path(self.module_qc_nonelec_gui_dir).joinpath(
                     "GUI", "lib", "ConfirmWindow", "default_layout;py"
@@ -765,15 +818,19 @@
                 log.exception(traceback.format_exc())
                 QMessageBox.warning(
                     None,
                     "Warning",
                     'Module: "default_layout.py" is not found',
                     QMessageBox.Ok,
                 )
-        self.update_widget(self.confirm_wid)
+        self.update_widget(
+            self.confirm_wid,
+            self.confirm_wid.sizeHint().width(),
+            self.confirm_wid.sizeHint().height(),
+        )
 
     def confirm_init_common(self, sub, width=None, height=None):
         titlebox = QVBoxLayout()
         layout = QVBoxLayout()
         button_box = QHBoxLayout()
 
         label_title = QLabel()
@@ -812,15 +869,15 @@
         inner.setWidget(result_wid)
 
         layout.addLayout(titlebox)
         layout.addWidget(inner)
         layout.addLayout(button_box)
         sub.setLayout(layout)
 
-        self.update_widget(sub)
+        self.update_widget(sub, sub.sizeHint().width(), sub.sizeHint().height())
 
     def confirm_layout_common(self, sub):
         Form_layout = QFormLayout()
         sub.add_info(Form_layout, "Serial Number :", self.info_dict["component"])
         sub.add_info(Form_layout, "Component Type :", self.info_dict["componentType"])
         sub.add_info(
             Form_layout,
@@ -988,15 +1045,19 @@
                 self.isPractice = False
                 self.continue_from()
         elif button_alt == QMessageBox.No:
             self.finish_GUI()
 
     def continue_from(self):
         self.continue_wid = continue_win.ContinueWindow(self)
-        self.update_widget(self.continue_wid)
+        self.update_widget(
+            self.continue_wid,
+            self.continue_wid.sizeHint().width(),
+            self.continue_wid.sizeHint().height(),
+        )
 
     def restart(self, is_sameuser, is_sameconmponent):
         self.info_dict.clear()
         self.localDB_dict.clear()
         self.testRun.clear()
 
         self.isSummarize = False
```

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/configuration/config_default.json` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/configuration/config_default.json`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/configuration/config_triplet_r.json` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/configuration/config_triplet_r.json`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/configuration/config_triplet_s.json` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/configuration/config_triplet_s.json`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/dbinterface/db_write.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/dbinterface/db_write.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/dbinterface/localdb_authenticator.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/dbinterface/localdb_authenticator.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/dbinterface/localdb_retriever.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/dbinterface/localdb_retriever.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/dbinterface/localdb_uploader.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/dbinterface/localdb_uploader.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/dbinterface/upload_results_sample.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/dbinterface/upload_results_sample.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/dbinterface/bin/uploader_sample.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/dbinterface/bin/uploader_sample.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/FLATNESS/confirm.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/FLATNESS/confirm.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/FLATNESS/main.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/FLATNESS/main.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/FLATNESS/user_input.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/FLATNESS/user_input.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/FLATNESS/example/example.json` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/FLATNESS/example/example.json`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE/confirm.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE/confirm.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE/main.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE/main.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE/user_input.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE/user_input.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE/example/jsonschema/validation_schema.json` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE/example/jsonschema/validation_schema.json`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE_BARE/confirm.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE_BARE/confirm.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE_BARE/function.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE_BARE/function.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE_BARE/main.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE_BARE/main.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE_BARE/user_input.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE_BARE/user_input.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE_BARE/example/example.dat` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE_BARE/example/example.dat`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE_BARE/example/example.json` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE_BARE/example/example.json`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE_BARE/example/jsonschema/validation_schema.json` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE_BARE/example/jsonschema/validation_schema.json`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/MASS_MEASUREMENT/confirm.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/MASS_MEASUREMENT/confirm.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/MASS_MEASUREMENT/main.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/MASS_MEASUREMENT/main.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/MASS_MEASUREMENT/user_input.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/MASS_MEASUREMENT/user_input.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/QUAD_MODULE_METROLOGY/confirm.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/QUAD_MODULE_METROLOGY/confirm.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/QUAD_MODULE_METROLOGY/initial_metrology.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/QUAD_MODULE_METROLOGY/initial_metrology.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/QUAD_MODULE_METROLOGY/main.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/QUAD_MODULE_METROLOGY/main.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/QUAD_MODULE_METROLOGY/example/db.csv` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/QUAD_MODULE_METROLOGY/example/db.csv`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/QUAD_MODULE_METROLOGY/example/db.json` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/QUAD_MODULE_METROLOGY/example/db.json`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/QUAD_MODULE_METROLOGY/example/db_new.csv` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/QUAD_MODULE_METROLOGY/example/db_new.csv`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/QUAD_MODULE_METROLOGY/example/db_new.json` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/QUAD_MODULE_METROLOGY/example/db_new.json`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/THERMAL_CYCLING/confirm.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/THERMAL_CYCLING/confirm.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/THERMAL_CYCLING/initial_Thermal.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/THERMAL_CYCLING/initial_Thermal.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/THERMAL_CYCLING/main.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/THERMAL_CYCLING/main.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/README.md` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/README.md`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/checklist.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/checklist.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/checklist_Module.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/checklist_Module.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/checklist_PCB.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/checklist_PCB.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/confirm.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/confirm.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,47 +23,57 @@
     pass
 
 
 class ConfirmWindow(QWidget):
     def __init__(self, parent=None):
         super(QWidget, self).__init__(parent)
         self.parent = parent
-        self.resize(400, 600)
+
+        self.setMinimumWidth(900)
+        self.setMinimumHeight(400)
 
         layout = QVBoxLayout()
 
         label_text = QLabel()
         label_text.setText('<center><font size="6"> Submission Preview</font></center>')
-        layout.addWidget(label_text)
-
-        grid_layout = self.make_infotable()
-        hbox = QHBoxLayout()
-        hbox.addLayout(grid_layout)
-
-        layout.addLayout(hbox)
-        layout.addStretch()
 
+        # layout buttons
+        buttons_widget = QWidget()
         layout_buttons = QHBoxLayout()
         button_back = QPushButton("Back")
         button_back.clicked.connect(self.parent.back_to_test)
-
         button_check = QPushButton("Check JSON")
         button_check.clicked.connect(self.parent.confirm_json)
-
         button_write = QPushButton("Register to LocalDB")
         button_write.clicked.connect(self.parent.upload_to_db)
 
         layout_buttons.addWidget(button_back)
-        layout.addStretch()
         layout_buttons.addWidget(button_check)
-        layout.addStretch()
         layout_buttons.addWidget(button_write)
 
-        layout.addLayout(layout_buttons)
+        buttons_widget.setLayout(layout_buttons)
 
+        # layout infotable in a scrollarea
+        grid_layout = self.make_infotable()
+        layout_infotable = QHBoxLayout()
+        layout_infotable.addLayout(grid_layout)
+
+        infotable_widgets = QWidget()
+        infotable_widgets.setLayout(layout_infotable)
+
+        scroll = QScrollArea()
+        scroll.setWidgetResizable(True)
+        scroll.setVerticalScrollBarPolicy(Qt.ScrollBarAlwaysOn)
+        scroll.setWidget(infotable_widgets)
+
+        # layout final
+        layout = QVBoxLayout()
+        layout.addWidget(label_text)
+        layout.addWidget(scroll)
+        layout.addWidget(buttons_widget)
         layout.setSpacing(5)
         layout.setContentsMargins(20, 20, 20, 20)
 
         self.setLayout(layout)
 
     def get_maximum(self, contents_dict):
         N_char = []
```

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/inspection_win.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/inspection_win.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,15 +77,17 @@
 
         label_comment = QLabel(self)
         label_comment.setText("Describe observation and details of defects:")
 
         self.edit_comment = QPlainTextEdit(self)
         self.edit_comment.setFixedHeight(100)
         with contextlib.suppress(Exception):
-            self.edit_comment.setText(self.parent.comment_dic[str(self.parent.n_page)])
+            self.edit_comment.setPlainText(
+                self.parent.comment_dic[str(self.parent.n_page)]
+            )
 
         ## prepare buttons
         label_brightness = QLabel(self)
         label_brightness.setText("Brightness: ")
 
         label_contrast = QLabel(self)
         label_contrast.setText("Contrast: ")
@@ -296,15 +298,16 @@
         ## prepare target images
         self.path_target = self.split_img(self.img_bgr, self.parent.n_page)
 
         self.brightness = float(self.input_brightness.text())
         self.contrast = float(self.input_contrast.text())
 
         log.info(
-            f"retouch(): retouching the target image with brightness = {self.brightness}, contrast = {self.contrast}"
+            f"retouch(): retouching the target image with brightness = {self.brightness}, "
+            + f"contrast = {self.contrast}"
         )
 
         self.view = self.setImg(
             self.path_target,
             0,
             self.contrast,
             self.brightness,
@@ -333,23 +336,34 @@
             self.setImg(
                 self.parent.path_gm + f"/tile{self.parent.n_page}_wireline.jpg", 1
             )
         except Exception:
             self.setImg(self.path_gm, 1)
 
     def checkout(self):
-        self.anomaly_update()
-        self.parent.comment_dic[
-            str(self.parent.n_page)
-        ] = self.edit_comment.toPlainText()
+        if self.parent.page_checked[self.parent.n_page] is False:
+            self.anomaly_update()
+            self.parent.comment_dic[
+                str(self.parent.n_page)
+            ] = self.edit_comment.toPlainText()
+
+            self.parent.page_checked[self.parent.n_page] = True
+            log.debug(f" Just checked out: tileID {self.parent.n_page} ")
+            log.debug(f" Tiles checked: {self.nb_checked()} ")
+
+        else:
+            self.parent.page_checked[self.parent.n_page] = False
+            log.debug(f" Just checked in: tileID {self.parent.n_page} ")
+            log.debug(f" Tiles checked: {self.nb_checked()} ")
 
-        self.parent.page_checked[self.parent.n_page] = True
+    def nb_checked(self):
+        return reduce(lambda a, b: int(a) + int(b), self.parent.page_checked)
 
     def check_status(self):
-        n_checked = reduce(lambda a, b: int(a) + int(b), self.parent.page_checked)
+        n_checked = self.nb_checked()
 
         total = len(self.parent.page_checked)
 
         log.info(f"checked tiles: {n_checked} / {total}")
 
         return n_checked == total
```

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/main.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,15 +116,17 @@
                                     + self.config["checklist"][side][flag]
                                 )
 
         if self.config.get("backside") is True:
             QMessageBox.warning(
                 self,
                 "Warning",
-                "Back-side inspection is required in this stage: please make sure that the photograph is already recorded at this point, otherwise you will be required to re-do the front-side inspection again!",
+                "Back-side inspection is required in this stage: "
+                + "please make sure that the photograph is already recorded at this point, "
+                + "otherwise you will be required to re-do the front-side inspection again!",
             )
 
         log.info(pprint.pformat(self.config))
 
         self.origImgPath = {"front": "", "back": ""}
         self.mode = "front"
 
@@ -163,15 +165,18 @@
         except Exception:
             log.exception("missing the golden image file")
 
             while True:
                 msgBox = QMessageBox(self)
                 msgBox.setTextFormat(Qt.RichText)
                 msgBox.setText(
-                    'Golden module image bank needs to be deployed.<br /><br />[Step-1] Download the following zip file: <br /><a href="https://cernbox.cern.ch/s/PAMujVUmRUni0um">https://cernbox.cern.ch/s/PAMujVUmRUni0um</a><br /><br />[Step-2] Indicate the path of the zip file to this GUI.'
+                    "Golden module image bank needs to be deployed.<br /><br />"
+                    + "[Step-1] Download the following zip file: "
+                    + '<br /><a href="https://cernbox.cern.ch/s/PAMujVUmRUni0um">https://cernbox.cern.ch/s/PAMujVUmRUni0um</a><br /><br />'
+                    + "[Step-2] Indicate the path of the zip file to this GUI."
                 )
                 msgBox.setStandardButtons(QMessageBox.Ok)
                 msgBtn = msgBox.button(QMessageBox.Ok)
                 msgBtn.setText("Yes, downloaded the zip file")
                 msgBox.exec()
 
                 dlg = QFileDialog(self)
@@ -195,17 +200,15 @@
                 shell=True,
                 check=False,
             )
 
             shutil.rmtree(str(Path(self.path_gm).parent))
 
             subprocess.run(
-                "mv -f /var/tmp/golden_module {}; rm -rf /var/tmp/golden_module*".format(
-                    str(Path(self.path_gm).parent.parent)
-                ),
+                f"mv -f /var/tmp/golden_module {Path(self.path_gm).parent.parent!s}; rm -rf /var/tmp/golden_module*",
                 shell=True,
                 check=False,
             )
 
             with Path(self.path_gm + "/main_img.jpg").open(encoding="utf-8") as f:
                 pass
```

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/shaping_win.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/shaping_win.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,34 +4,38 @@
 import math
 import statistics
 import time
 
 import cv2
 import numpy as np
 from PyQt5 import QtCore
-from PyQt5.QtGui import QBrush, QDoubleValidator, QImage, QPen, QPixmap
+from PyQt5.QtGui import QBrush, QImage, QPen, QPixmap
 from PyQt5.QtWidgets import (
+    QDoubleSpinBox,
     QGraphicsPixmapItem,
     QGraphicsScene,
     QGraphicsView,
     QGridLayout,
     QHBoxLayout,
     QLabel,
     QLineEdit,
     QMessageBox,
     QPushButton,
+    QSpinBox,
     QWidget,
 )
 
 from module_qc_nonelec_gui.qc_tests.VISUAL_INSPECTION.functions.cv2_func import (
     img_cvt_rgb,
 )
 
 log = logging.getLogger(__name__)
 
+preview_size = 600
+
 
 class GraphicsScene(QGraphicsScene):
     def __init__(self, trimmer=None):
         QGraphicsScene.__init__(self, None)
         self.setSceneRect(0, 0, 0, 0)
         self.trimmer = trimmer
         self.turn = 0
@@ -110,45 +114,45 @@
         self.scene = GraphicsScene(self)
         self.srect = self.view.rect()
         self.view.setScene(self.scene)
 
         # load module picture
         img_org = cv2.imread(self.parent.origImgPath[self.parent.mode])
         h, w, d = img_org.shape
-        scale = min(600.0 / float(h), 600.0 / float(w))
+        scale = min(preview_size / float(h), preview_size / float(w))
 
         resize_img = cv2.resize(
             img_org, dsize=None, fx=scale, fy=scale, interpolation=cv2.INTER_LANCZOS4
         )
 
         img_rgb, h_rgb, w_rgb, d_rgb = img_cvt_rgb(resize_img)
         bytesPerLine = d_rgb * w_rgb
 
         self.image = QImage(
             img_rgb.data, w_rgb, h_rgb, bytesPerLine, QImage.Format_RGB888
         )
         self.item = QGraphicsPixmapItem(QPixmap.fromImage(self.image))
         self.scene.addItem(self.item)
         self.view.setScene(self.scene)
-        self.view.setFixedWidth(650)
-        self.view.setFixedHeight(650)
+        self.view.setFixedWidth(preview_size + 50)
+        self.view.setFixedHeight(preview_size + 50)
 
         self.layout.addWidget(self.view, self.nLayoutRows, 0, 1, 2)
         self.nLayoutRows = self.nLayoutRows + 1
 
         self.buttons = QHBoxLayout()
 
     def setupCustom(self, custom_params):
         pass
 
     def setupCommon2(self):
         button_back = QPushButton("Back")
         button_back.clicked.connect(self.parent.load_img)
 
-        button_rotate = QPushButton("Rotate")
+        button_rotate = QPushButton("Rotate (+90°)")
         button_rotate.clicked.connect(self.rotate)
 
         button_crop = QPushButton("Preview")
         button_crop.clicked.connect(self.trim)
 
         button_ok = QPushButton("Next")
         button_ok.clicked.connect(self.go_next)
@@ -159,37 +163,38 @@
         self.buttons.addWidget(button_ok)
 
         self.layout.addLayout(self.buttons, self.nLayoutRows, 0)
         self.nLayoutRows = self.nLayoutRows + 1
         self.setLayout(self.layout)
 
     def rotate(self):
-        self.parent.rotate_img()
+        self.parent.rotate_img()  # ROTATE_90_CLOCKWISE
         self.trim()
 
     def trim(self):
         try:
             self.trim_image(self.getParameters())
 
         except Exception as e:
             log.exception(e)
 
             QMessageBox.warning(
                 self,
                 "Warning",
-                "Failed in cropping!\n\nManually click the center of the GA1 Pickup Point, and then click the center of the GA3 Pickup Point to determine the frame",
+                "Failed in cropping!\n\nManually click the center of the GA1 Pickup Point, "
+                + "and then click the center of the GA3 Pickup Point to determine the frame",
             )
 
         preview = cv2.imread(self.tmp_preview_path)
 
         self.cropped = cv2.imread(self.tmp_cropped_path)
 
         h, w, d = preview.shape
 
-        scale = min(600.0 / float(h), 600.0 / float(w))
+        scale = min(preview_size / float(h), preview_size / float(w))
 
         resize_img = cv2.resize(
             preview, dsize=None, fx=scale, fy=scale, interpolation=cv2.INTER_LANCZOS4
         )
 
         img_rgb, h_rgb, w_rgb, d_rgb = img_cvt_rgb(resize_img)
         bytesPerLine = d_rgb * w_rgb
@@ -239,38 +244,47 @@
 
         label_blur = QLabel(self)
         label_blur.setText("Blur: [3, 10]")
 
         label_tweak = QLabel(self)
         label_tweak.setText("Tweak: [20, 50]")
 
-        self.input_rot = QLineEdit(self)
-        self.input_rot.setFixedWidth(40)
-        self.input_rot.setValidator(QDoubleValidator(-3.0, 3.0, 2))
-        self.input_rot.setText(str(0.00))
-
-        self.input_brightness = QLineEdit(self)
-        self.input_brightness.setFixedWidth(40)
-        self.input_brightness.setValidator(QDoubleValidator(-100, 100, 0))
-        self.input_brightness.setText(str(custom_params.get("Brightness", -20)))
-
-        self.input_contrast = QLineEdit(self)
-        self.input_contrast.setFixedWidth(40)
-        self.input_contrast.setValidator(QDoubleValidator(0.0, 2.0, 1))
-        self.input_contrast.setText(str(custom_params.get("Contrast", 1.3)))
-
-        self.input_blur = QLineEdit(self)
+        self.input_rot = QDoubleSpinBox()
+        self.input_rot.setMinimum(-3)
+        self.input_rot.setMaximum(3)
+        self.input_rot.setSingleStep(0.1)
+        self.input_rot.setFixedWidth(50)
+
+        self.input_brightness = QSpinBox()
+        self.input_brightness.setMinimum(-100)
+        self.input_brightness.setMaximum(100)
+        self.input_brightness.setSingleStep(10)
+        self.input_brightness.setFixedWidth(50)
+        self.input_brightness.setValue(custom_params.get("Brightness", -20))
+
+        self.input_contrast = QDoubleSpinBox()
+        self.input_contrast.setMinimum(0.0)
+        self.input_contrast.setMaximum(2.0)
+        self.input_contrast.setSingleStep(0.1)
+        self.input_contrast.setFixedWidth(50)
+        self.input_contrast.setValue(custom_params.get("Contrast", 1.3))
+
+        self.input_blur = QSpinBox()
+        self.input_blur.setMinimum(3)
+        self.input_blur.setMaximum(10)
+        self.input_blur.setSingleStep(1)
         self.input_blur.setFixedWidth(40)
-        self.input_blur.setValidator(QDoubleValidator(1, 5, 0))
-        self.input_blur.setText(str(custom_params.get("InitialBlur", 5)))
+        self.input_blur.setValue(custom_params.get("InitialBlur", 5))
 
-        self.input_tweak = QLineEdit(self)
+        self.input_tweak = QSpinBox()
+        self.input_tweak.setMinimum(20)
+        self.input_tweak.setMaximum(50)
+        self.input_tweak.setSingleStep(5)
         self.input_tweak.setFixedWidth(40)
-        self.input_tweak.setValidator(QDoubleValidator(20, 50, 0))
-        self.input_tweak.setText(str(custom_params.get("InitialParam2", 35)))
+        self.input_tweak.setValue(custom_params.get("InitialParam2", 35))
 
         self.handles.addWidget(label_rot)
         self.handles.addWidget(self.input_rot)
         self.handles.addWidget(label_brightness)
         self.handles.addWidget(self.input_brightness)
         self.handles.addWidget(label_contrast)
         self.handles.addWidget(self.input_contrast)
@@ -286,22 +300,26 @@
         self.nLayoutRows = self.nLayoutRows + 1
 
         self.layout.addLayout(self.handles2, self.nLayoutRows, 0)
         self.nLayoutRows = self.nLayoutRows + 1
 
     def getParameters(self):
         # get the original image
-        rot_angle = float(self.input_rot.text())
-        init_blur = int(self.input_blur.text())
-        contrast = float(self.input_contrast.text())
-        brightness = float(self.input_brightness.text())
-        init_param2 = int(self.input_tweak.text())
+        rot_angle = float(round(self.input_rot.value(), 1))
+        init_blur = int(self.input_blur.value())
+        contrast = float(round(self.input_contrast.value(), 1))
+        brightness = float(self.input_brightness.value())
+        init_param2 = int(self.input_tweak.value())
 
         log.info(
-            f"cropping with rot_angle {rot_angle}, init_blur {init_blur}, contrast {contrast}, brightness {brightness}, init_param2 {init_param2}"
+            f"cropping with rot_angle {rot_angle}, "
+            + f"init_blur {init_blur}, "
+            + f"contrast {contrast}, "
+            + f"brightness {brightness}, "
+            + f"init_param2 {init_param2}"
         )
 
         return {
             "rot_angle": rot_angle,
             "init_blur": init_blur,
             "contrast": contrast,
             "brightness": brightness,
@@ -316,15 +334,15 @@
         init_param2 = params["init_param2"]
 
         image_1 = self.parent.img_bgr.copy()
 
         image_center = tuple(np.array(image_1.shape[1::-1]) / 2)
         rot_mat = cv2.getRotationMatrix2D(image_center, rot_angle, 1.0)
         image_2 = cv2.warpAffine(
-            image_1, rot_mat, image_1.shape[1::-1], flags=cv2.INTER_LINEAR
+            image_1, rot_mat, image_1.shape[1::-1], flags=cv2.INTER_LANCZOS4
         )
 
         image_3 = cv2.convertScaleAbs(image_2, alpha=contrast, beta=brightness)
 
         height_org, width_org, channel = image_3.shape
 
         resize_scale = (
@@ -414,15 +432,16 @@
 
         cropped = image_2[y_edge1:y_edge2, x_edge1:x_edge2].copy()
 
         cv2.imwrite(self.tmp_cropped_path, cropped)
 
         marker_width = int(0.005 * width)
 
-        color = (0, 255, 128)
+        color = (0, 255, 128)  # Green
+        color2 = (255, 0, 128)  # Purple
 
         # Draw the center reticle
         gray_bgr = cv2.cvtColor(gray, cv2.COLOR_GRAY2RGB)
 
         cv2.line(
             gray_bgr,
             (center_x - 20, center_y),
@@ -434,74 +453,76 @@
             gray_bgr,
             (center_x, center_y - 20),
             (center_x, center_y + 20),
             color,
             marker_width,
         )
 
+        # Draw the outer corners
         cv2.line(
             gray_bgr,
             (x_edge1_0, y_edge1_0),
             (x_edge1_0 + 50, y_edge1_0),
-            color,
+            color2,
             marker_width,
         )
         cv2.line(
             gray_bgr,
             (x_edge1_0, y_edge1_0),
             (x_edge1_0, y_edge1_0 + 50),
-            color,
+            color2,
             marker_width,
         )
 
         cv2.line(
             gray_bgr,
             (x_edge2_0, y_edge1_0),
             (x_edge2_0 - 50, y_edge1_0),
-            color,
+            color2,
             marker_width,
         )
         cv2.line(
             gray_bgr,
             (x_edge2_0, y_edge1_0),
             (x_edge2_0, y_edge1_0 + 50),
-            color,
+            color2,
             marker_width,
         )
 
         cv2.line(
             gray_bgr,
             (x_edge1_0, y_edge2_0),
             (x_edge1_0 + 50, y_edge2_0),
-            color,
+            color2,
             marker_width,
         )
         cv2.line(
             gray_bgr,
             (x_edge1_0, y_edge2_0),
             (x_edge1_0, y_edge2_0 - 50),
-            color,
+            color2,
             marker_width,
         )
 
         cv2.line(
             gray_bgr,
             (x_edge2_0, y_edge2_0),
             (x_edge2_0 - 50, y_edge2_0),
-            color,
+            color2,
             marker_width,
         )
         cv2.line(
             gray_bgr,
             (x_edge2_0, y_edge2_0),
             (x_edge2_0, y_edge2_0 - 50),
-            color,
+            color2,
             marker_width,
         )
 
+        # Draw pickup point circles
         for p in pickup_points:
             cv2.circle(
                 gray_bgr,
                 (int(p[0]), int(p[1])),
                 int(p[2]),
                 color,
                 int(marker_width * 0.5),
@@ -521,15 +542,15 @@
         # init_param2 = params["init_param2"]
 
         image_1 = self.parent.img_bgr.copy()
 
         image_center = tuple(np.array(image_1.shape[1::-1]) / 2)
         rot_mat = cv2.getRotationMatrix2D(image_center, 0.0, 1.0)
         image_2 = cv2.warpAffine(
-            image_1, rot_mat, image_1.shape[1::-1], flags=cv2.INTER_LINEAR
+            image_1, rot_mat, image_1.shape[1::-1], flags=cv2.INTER_LANCZOS4
         )
 
         image_3 = cv2.convertScaleAbs(image_2, alpha=contrast, beta=brightness)
 
         height_org, width_org, channel = image_3.shape
 
         resize_scale = (
@@ -603,15 +624,16 @@
 
         cropped = image_2[y_edge1:y_edge2, x_edge1:x_edge2].copy()
 
         cv2.imwrite(self.tmp_cropped_path, cropped)
 
         marker_width = int(0.005 * width)
 
-        color = (0, 255, 128)
+        color = (0, 255, 128)  # Green
+        color2 = (255, 0, 128)  # Purple
 
         # Draw the center reticle
         gray_bgr = cv2.cvtColor(gray, cv2.COLOR_GRAY2RGB)
 
         cv2.line(
             gray_bgr,
             (center_x - 20, center_y),
@@ -623,74 +645,76 @@
             gray_bgr,
             (center_x, center_y - 20),
             (center_x, center_y + 20),
             color,
             marker_width,
         )
 
+        # Draw corner lines
         cv2.line(
             gray_bgr,
             (x_edge1_0, y_edge1_0),
             (x_edge1_0 + 50, y_edge1_0),
-            color,
+            color2,
             marker_width,
         )
         cv2.line(
             gray_bgr,
             (x_edge1_0, y_edge1_0),
             (x_edge1_0, y_edge1_0 + 50),
-            color,
+            color2,
             marker_width,
         )
 
         cv2.line(
             gray_bgr,
             (x_edge2_0, y_edge1_0),
             (x_edge2_0 - 50, y_edge1_0),
-            color,
+            color2,
             marker_width,
         )
         cv2.line(
             gray_bgr,
             (x_edge2_0, y_edge1_0),
             (x_edge2_0, y_edge1_0 + 50),
-            color,
+            color2,
             marker_width,
         )
 
         cv2.line(
             gray_bgr,
             (x_edge1_0, y_edge2_0),
             (x_edge1_0 + 50, y_edge2_0),
-            color,
+            color2,
             marker_width,
         )
         cv2.line(
             gray_bgr,
             (x_edge1_0, y_edge2_0),
             (x_edge1_0, y_edge2_0 - 50),
-            color,
+            color2,
             marker_width,
         )
 
         cv2.line(
             gray_bgr,
             (x_edge2_0, y_edge2_0),
             (x_edge2_0 - 50, y_edge2_0),
-            color,
+            color2,
             marker_width,
         )
         cv2.line(
             gray_bgr,
             (x_edge2_0, y_edge2_0),
             (x_edge2_0, y_edge2_0 - 50),
-            color,
+            color2,
             marker_width,
         )
 
+        # Draw the clicked points
         cv2.circle(
             gray_bgr,
             (
                 int(manual_points.get("GA1").get("x")) * 2,
                 int(manual_points.get("GA1").get("y")) * 2,
             ),
             10,
@@ -807,15 +831,14 @@
                     isHorizontal = ang < 2 * deg
                     isVertical = ang > 88 * deg
 
                     if not (isHorizontal or isVertical):
                         # log.info( f'{length:.2f} px, {ang/deg:6.3f} deg ==> skipped' )
                         continue
 
-                    # log.info( f'    {"Horizontal" if isHorizontal else "Vertical":12s}: {length:.2f} px, {ang/deg:6.3f} deg' )
                     cv2.line(
                         image_4,
                         (int(ci[0]), int(ci[1])),
                         (int(cj[0]), int(cj[1])),
                         (0, 0, 0),
                         1,
                     )
@@ -901,43 +924,54 @@
 
         label_cannyThr1 = QLabel(self)
         label_cannyThr1.setText("Thr1: [0, 255]")
 
         label_cannyThr2 = QLabel(self)
         label_cannyThr2.setText("Thr2: [0, 255]")
 
-        self.input_rot = QLineEdit(self)
-        self.input_rot.setFixedWidth(40)
-        self.input_rot.setValidator(QDoubleValidator(-3.0, 3.0, 2))
-        self.input_rot.setText(str(0.00))
-
-        self.input_brightness = QLineEdit(self)
-        self.input_brightness.setFixedWidth(40)
-        self.input_brightness.setValidator(QDoubleValidator(-100, 100, 0))
-        self.input_brightness.setText(str(custom_params.get("Brightness", 50)))
-
-        self.input_contrast = QLineEdit(self)
-        self.input_contrast.setFixedWidth(40)
-        self.input_contrast.setValidator(QDoubleValidator(0.0, 4.0, 1))
-        self.input_contrast.setText(str(custom_params.get("Contrast", 3.0)))
-
-        self.input_blur = QLineEdit(self)
+        self.input_rot = QDoubleSpinBox()
+        self.input_rot.setMinimum(-3)
+        self.input_rot.setMaximum(3)
+        self.input_rot.setSingleStep(0.1)
+        self.input_rot.setFixedWidth(50)
+
+        self.input_brightness = QSpinBox()
+        self.input_brightness.setMinimum(-100)
+        self.input_brightness.setMaximum(100)
+        self.input_brightness.setSingleStep(10)
+        self.input_brightness.setFixedWidth(50)
+        self.input_brightness.setValue(custom_params.get("Brightness", 50))
+
+        self.input_contrast = QDoubleSpinBox()
+        self.input_contrast.setMinimum(0.0)
+        self.input_contrast.setMaximum(4.0)
+        self.input_contrast.setSingleStep(0.1)
+        self.input_contrast.setFixedWidth(50)
+        self.input_contrast.setValue(custom_params.get("Contrast", 3))
+
+        self.input_blur = QSpinBox()
+        self.input_blur.setMinimum(1)
+        self.input_blur.setMaximum(5)
+        self.input_blur.setSingleStep(1)
         self.input_blur.setFixedWidth(40)
-        self.input_blur.setValidator(QDoubleValidator(1, 5, 0))
-        self.input_blur.setText(str(5))
+        self.input_blur.setValue(custom_params.get("InitialBlur", 5))
 
-        self.input_cannyThr1 = QLineEdit(self)
+        self.input_cannyThr1 = QSpinBox()
+        self.input_cannyThr1.setMinimum(0)
+        self.input_cannyThr1.setMaximum(255)
+        self.input_cannyThr1.setSingleStep(5)
         self.input_cannyThr1.setFixedWidth(40)
-        self.input_cannyThr1.setValidator(QDoubleValidator(0, 255, 0))
-        self.input_cannyThr1.setText(str(custom_params.get("CannyThr1", 100)))
+        self.input_cannyThr1.setValue(custom_params.get("CannyThr1", 100))
 
-        self.input_cannyThr2 = QLineEdit(self)
+        self.input_cannyThr2 = QSpinBox()
+        self.input_cannyThr2.setMinimum(0)
+        self.input_cannyThr2.setMaximum(255)
+        self.input_cannyThr2.setSingleStep(5)
         self.input_cannyThr2.setFixedWidth(40)
-        self.input_cannyThr2.setValidator(QDoubleValidator(0, 255, 0))
-        self.input_cannyThr2.setText(str(custom_params.get("CannyThr2", 20)))
+        self.input_cannyThr2.setValue(custom_params.get("CannyThr2", 20))
 
         self.handles.addWidget(label_rot)
         self.handles.addWidget(self.input_rot)
         self.handles.addWidget(label_brightness)
         self.handles.addWidget(self.input_brightness)
         self.handles.addWidget(label_contrast)
         self.handles.addWidget(self.input_contrast)
@@ -949,39 +983,44 @@
         self.handles2.addWidget(label_cannyThr2)
         self.handles2.addWidget(self.input_cannyThr2)
 
         self.layout.addLayout(self.handles, self.nLayoutRows, 0)
         self.nLayoutRows = self.nLayoutRows + 1
 
         msg = QLineEdit(self)
-        msg.setFixedWidth(700)
+        msg.setFixedWidth(preview_size + 50)
         msg.setReadOnly(True)
         msg.setText(
-            "If auto-detection fails, you can manually specify the cropping region by clicking two diagonal corners of the FEs"
+            "If auto-detection fails, you can manually specify "
+            + "the cropping region by clicking two diagonal corners of the FEs"
         )
         self.layout.addWidget(msg, self.nLayoutRows, 0)
         self.nLayoutRows = self.nLayoutRows + 1
 
         self.layout.addLayout(self.handles2, self.nLayoutRows, 0)
         self.nLayoutRows = self.nLayoutRows + 1
 
         self.handles.addStretch()
         self.handles2.addStretch()
 
     def getParameters(self):
         # get the original image
-        rot_angle = float(self.input_rot.text())
-        init_blur = int(self.input_blur.text())
-        contrast = float(self.input_contrast.text())
-        brightness = float(self.input_brightness.text())
-        cannyThr1 = int(self.input_cannyThr1.text())
-        cannyThr2 = int(self.input_cannyThr2.text())
+        rot_angle = float(round(self.input_rot.value(), 1))
+        init_blur = int(self.input_blur.value())
+        contrast = float(round(self.input_contrast.value(), 1))
+        brightness = float(round(self.input_brightness.value(), 1))
+        cannyThr1 = int(self.input_cannyThr1.value())
+        cannyThr2 = int(self.input_cannyThr2.value())
 
         log.info(
-            f"cropping with rot_angle {rot_angle}, init_blur {init_blur}, contrast {contrast}, brightness {brightness}, cannyThr [{cannyThr1}, {cannyThr2}]"
+            f"cropping with rot_angle {rot_angle}, "
+            + f"init_blur {init_blur}, "
+            + f"contrast {contrast}, "
+            + f"brightness {brightness}, "
+            + f"cannyThr [{cannyThr1}, {cannyThr2}]"
         )
 
         return {
             "rot_angle": rot_angle,
             "init_blur": init_blur,
             "contrast": contrast,
             "brightness": brightness,
@@ -995,15 +1034,15 @@
         brightness = params["brightness"]
 
         image_1 = self.parent.img_bgr.copy()
 
         image_center = tuple(np.array(image_1.shape[1::-1]) / 2)
         rot_mat = cv2.getRotationMatrix2D(image_center, rot_angle, 1.0)
         image_2 = cv2.warpAffine(
-            image_1, rot_mat, image_1.shape[1::-1], flags=cv2.INTER_LINEAR
+            image_1, rot_mat, image_1.shape[1::-1], flags=cv2.INTER_LANCZOS4
         )
 
         image_3 = cv2.convertScaleAbs(image_2, alpha=contrast, beta=brightness)
 
         height_org, width_org, channel = image_3.shape
         log.info(f"original image: width {width_org}, height {height_org}")
 
@@ -1118,15 +1157,15 @@
         # init_param2 = params["init_param2"]
 
         image_1 = self.parent.img_bgr.copy()
 
         image_center = tuple(np.array(image_1.shape[1::-1]) / 2)
         rot_mat = cv2.getRotationMatrix2D(image_center, 0.0, 1.0)
         image_2 = cv2.warpAffine(
-            image_1, rot_mat, image_1.shape[1::-1], flags=cv2.INTER_LINEAR
+            image_1, rot_mat, image_1.shape[1::-1], flags=cv2.INTER_LANCZOS4
         )
 
         # image_3 = cv2.convertScaleAbs(image_2, alpha=contrast, beta=brightness)
         image_3 = cv2.convertScaleAbs(image_2, alpha=contrast, beta=0)
 
         height_org, width_org, channel = image_3.shape
 
@@ -1175,15 +1214,16 @@
                 ),
             ]
         )
 
         pitch = gauge_std / 41.236  # pixels / mm
 
         log.info(
-            f"gauge_std = {gauge_std:.3f} px: 1mm = {pitch:.3f} px, center = ( {center_x:6.3f}, {center_y:6.3f} )"
+            f"gauge_std = {gauge_std:.3f} px: 1mm = {pitch:.3f} px, "
+            + f"center = ( {center_x:6.3f}, {center_y:6.3f} )"
         )
 
         x_edge1_0 = max(int(center_x - self.cropRange * pitch), 0)
         y_edge1_0 = max(int(center_y - self.cropRange * pitch), 0)
         x_edge2_0 = min(int(center_x + self.cropRange * pitch), width - 1)
         y_edge2_0 = min(int(center_y + self.cropRange * pitch), height - 1)
 
@@ -1485,15 +1525,15 @@
         init_param2 = params["init_param2"]
 
         image_1 = self.parent.img_bgr.copy()
 
         image_center = tuple(np.array(image_1.shape[1::-1]) / 2)
         rot_mat = cv2.getRotationMatrix2D(image_center, rot_angle, 1.0)
         image_2 = cv2.warpAffine(
-            image_1, rot_mat, image_1.shape[1::-1], flags=cv2.INTER_LINEAR
+            image_1, rot_mat, image_1.shape[1::-1], flags=cv2.INTER_LANCZOS4
         )
 
         image_3 = cv2.convertScaleAbs(image_2, alpha=contrast, beta=brightness)
 
         height_org, width_org, channel = image_3.shape
 
         resize_scale = (
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/splitimg_win.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/splitimg_win.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,17 @@
 class SplitImageWindow(QWidget):
     def __init__(self, parent=None):
         super(QWidget, self).__init__(parent)
         self.parent = parent
 
         layout = QGridLayout()
 
+        self.setMinimumWidth(650)
+        self.setMinimumHeight(700)
+
         self.view = QGraphicsView()
         self.scene = QGraphicsScene()
         self.srect = self.view.rect()
         self.view.setScene(self.scene)
 
         self.parent.update_img(self.parent.img_bgr)
         self.img_bgr_line, h, w, _d = read_img(
@@ -67,17 +70,14 @@
             fx=scale,
             fy=scale,
             interpolation=cv2.INTER_LANCZOS4,
         )
         img_rgb, h_rgb, w_rgb, d_rgb = img_cvt_rgb(resize_img)
         bytesPerLine = d_rgb * w_rgb
 
-        # # for test
-        # self.parent.update_img(img_bgr_line)
-
         self.image = QImage(
             img_rgb.data, w_rgb, h_rgb, bytesPerLine, QImage.Format_RGB888
         )
         self.item = QGraphicsPixmapItem(QPixmap.fromImage(self.image))
         self.scene.addItem(self.item)
         self.view.setScene(self.scene)
         self.view.setFixedWidth(600)
```

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/summary_win.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/summary_win.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from PyQt5.QtWidgets import (
     QGridLayout,
     QHBoxLayout,
     QLabel,
     QLineEdit,
     QPlainTextEdit,
     QPushButton,
+    QScrollArea,
     QVBoxLayout,
     QWidget,
 )
 
 # from PyQt5.QtWidgets import QLabel, QPushButton, QVBoxLayout, QWidget
 # from PyQt5.QtGUI import *
 #
@@ -21,42 +22,53 @@
 log = logging.getLogger(__name__)
 
 
 class SummaryWindow(QWidget):
     def __init__(self, parent=None):
         super(QWidget, self).__init__(parent)
         self.parent = parent
-        self.resize(400, 600)
 
-        layout = QVBoxLayout()
+        self.setMinimumWidth(900)
+        self.setMinimumHeight(400)
 
+        # layout common
         label_text = QLabel()
         label_text.setText('<center><font size="6"> Inspection Summary</font></center>')
-        layout.addWidget(label_text)
-
-        grid_layout = self.make_infotable()
-        hbox = QHBoxLayout()
-        hbox.addLayout(grid_layout)
-
-        layout.addLayout(hbox)
-        layout.addStretch()
 
+        # layout buttons
+        buttons_widget = QWidget()
         layout_buttons = QHBoxLayout()
         button_back = QPushButton("Back")
         button_back.clicked.connect(self.parent.inspection)
-
         button_write = QPushButton("Checkout Inspection")
         button_write.clicked.connect(self.write_data)
 
         layout_buttons.addWidget(button_back)
-        layout.addStretch()
         layout_buttons.addWidget(button_write)
 
-        layout.addLayout(layout_buttons)
+        buttons_widget.setLayout(layout_buttons)
 
+        # layout infotable in a scrollarea
+        grid_layout = self.make_infotable()
+        layout_infotable = QHBoxLayout()
+        layout_infotable.addLayout(grid_layout)
+
+        infotable_widgets = QWidget()
+        infotable_widgets.setLayout(layout_infotable)
+
+        scroll = QScrollArea()
+        scroll.setWidgetResizable(True)
+        scroll.setVerticalScrollBarPolicy(Qt.ScrollBarAlwaysOn)
+        scroll.setWidget(infotable_widgets)
+
+        # layout final
+        layout = QVBoxLayout()
+        layout.addWidget(label_text)
+        layout.addWidget(scroll)
+        layout.addWidget(buttons_widget)
         layout.setSpacing(5)
         layout.setContentsMargins(20, 20, 20, 20)
 
         self.setLayout(layout)
 
     def get_maximum(self, contents_dict):
         N_char = []
```

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/vi_initial_win.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/vi_initial_win.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 
 
 class InitialWindow(QWidget):
     def __init__(self, parent=None):
         super(QWidget, self).__init__(parent)
         self.parent = parent
 
+        self.setMinimumWidth(400)
+        self.setMinimumHeight(250)
+
         # Check if doing VI for PCB
         is_PCB = "PCB" in self.parent.type_name
         # Add instrument to the parent
         self.parent.instrument = ""
 
         # layout
         layout = QGridLayout()
```

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/VI_Config_Module.json` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/VI_Config_Module.json`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/VI_Config_Module_MODULETOPCB.json` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/VI_Config_Module_MODULETOPCB.json`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_BARE_MODULE_BAREMODULERECEPTION.json` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_BARE_MODULE_BAREMODULERECEPTION.json`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_BARE_MODULE_default.json` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_BARE_MODULE_default.json`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_MODULE_MODULE__ASSEMBLY.json` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_MODULE_MODULE__ASSEMBLY.json`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_MODULE_MODULE__PARYLENE_UNMASKING.json` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_MODULE_MODULE__PARYLENE_UNMASKING.json`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_MODULE_default.json` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_MODULE_default.json`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_PCB.json` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_PCB.json`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_PCB_PCB_POPULATION.json` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_PCB_PCB_POPULATION.json`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_PCB_PCB_RECEPTION.json` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_PCB_PCB_RECEPTION.json`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_PCB_default.json` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_PCB_default.json`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/functions/auto_trim.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/functions/auto_trim.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/functions/cv2_func.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/functions/cv2_func.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/WIREBOND_PULL_TEST/confirm.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/WIREBOND_PULL_TEST/confirm.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/WIREBOND_PULL_TEST/main.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/WIREBOND_PULL_TEST/main.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/WIREBOND_PULL_TEST/user_input.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/WIREBOND_PULL_TEST/user_input.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/glue_info_module_flex/Glue_info.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/glue_info_module_flex/Glue_info.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/glue_info_module_flex/confirm.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/glue_info_module_flex/confirm.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/glue_info_module_flex/initial_Glue_info.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/glue_info_module_flex/initial_Glue_info.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/parylene_properties/Parylene_prop.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/parylene_properties/Parylene_prop.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/parylene_properties/confirm.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/parylene_properties/confirm.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/parylene_properties/initial_Parylene_prop.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/parylene_properties/initial_Parylene_prop.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/wirebonding_info/Wire_info.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/wirebonding_info/Wire_info.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/wirebonding_info/confirm.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/wirebonding_info/confirm.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/src/module_qc_nonelec_gui/qc_tests/wirebonding_info/initial_Wire_info.py` & `module_qc_nonelec_gui-0.0.5/src/module_qc_nonelec_gui/qc_tests/wirebonding_info/initial_Wire_info.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/.gitignore` & `module_qc_nonelec_gui-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/LICENSE` & `module_qc_nonelec_gui-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/README.md` & `module_qc_nonelec_gui-0.0.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# module-qc-nonelec-gui 0.0.4
+# module-qc-nonelec-gui 0.0.5
 
 ## What is this
 
 This package is previously known to as "QC Helper" and it provides a GUI
 application for submitting non-electrical QC tests of ITkPix modules.
 
 It requires `python3.7` and relevant python modules. The GUI uses `PyQT5`
```

### Comparing `module_qc_nonelec_gui-0.0.4/pyproject.toml` & `module_qc_nonelec_gui-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.4/PKG-INFO` & `module_qc_nonelec_gui-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: module-qc-nonelec-gui
-Version: 0.0.4
+Version: 0.0.5
 Summary: GUI to upload Pixel Quality Control tests to ITk Production Database
 Project-URL: Documentation, https://module-qc-nonelec-gui.readthedocs.io/
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-nonelec-gui
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-nonelec-gui/-/issues
 Project-URL: Source, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-nonelec-gui
 Author-email: Hideyuki Oide <Hideyuki.Oide@cern.ch>, Minoru Hirose <Minoru.Hirose@cern.ch>, Giordon Stark <gstark@cern.ch>, Daiki Sameshima <sameshima@hepmail.phys.se.tmu.ac.jp>, Erika Oshima <ooshima@hepmail.phys.se.tmu.ac.jp>, Yuji Onishi <onishi@cern.ch>
 Maintainer-email: Giordon Stark <gstark@cern.ch>, Hideyuki Oide <Hideyuki.Oide@cern.ch>, ATLAS ITk Pixels <atlas-itk-pixel-modules@cern.ch>
@@ -60,15 +60,15 @@
 Requires-Dist: pyqt5; platform_system == 'Darwin'
 Requires-Dist: pyqt5; platform_system == 'Linux'
 Requires-Dist: requests
 Requires-Dist: typer
 Requires-Dist: typing-extensions>=3.7; python_version < '3.8'
 Description-Content-Type: text/markdown
 
-# module-qc-nonelec-gui 0.0.4
+# module-qc-nonelec-gui 0.0.5
 
 ## What is this
 
 This package is previously known to as "QC Helper" and it provides a GUI
 application for submitting non-electrical QC tests of ITkPix modules.
 
 It requires `python3.7` and relevant python modules. The GUI uses `PyQT5`
```

