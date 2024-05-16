# Comparing `tmp/stepup-1.2.0.tar.gz` & `tmp/stepup-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stepup-1.2.0.tar", last modified: Thu May  2 09:23:18 2024, max compression
+gzip compressed data, was "stepup-1.2.1.tar", last modified: Tue May  7 17:53:04 2024, max compression
```

## Comparing `stepup-1.2.0.tar` & `stepup-1.2.1.tar`

### file list

```diff
@@ -1,949 +1,948 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.310011 stepup-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-02 09:23:07.000000 stepup-1.2.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.158011 stepup-1.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.170011 stepup-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-02 09:23:07.000000 stepup-1.2.0/.github/workflows/mkdocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-02 09:23:07.000000 stepup-1.2.0/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-02 09:23:07.000000 stepup-1.2.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-02 09:23:07.000000 stepup-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-02 09:23:07.000000 stepup-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-02 09:23:07.000000 stepup-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-02 09:23:18.310011 stepup-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-02 09:23:07.000000 stepup-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.174011 stepup-1.2.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.174011 stepup-1.2.0/docs/advanced_topics/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.174011 stepup-1.2.0/docs/advanced_topics/amending_static_inputs/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/amending_static_inputs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/amending_static_inputs/config.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      149 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/amending_static_inputs/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      170 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/amending_static_inputs/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/amending_static_inputs/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/amending_static_inputs.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.174011 stepup-1.2.0/docs/advanced_topics/amending_steps/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/amending_steps/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)      146 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/amending_steps/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      262 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/amending_steps/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/amending_steps/stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      465 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/amending_steps/step.py
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/amending_steps.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.178011 stepup-1.2.0/docs/advanced_topics/blocked_steps/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/blocked_steps/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)      131 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/blocked_steps/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      161 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/blocked_steps/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/blocked_steps/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/blocked_steps.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.178011 stepup-1.2.0/docs/advanced_topics/cyclic_dependencies/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/cyclic_dependencies/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)      131 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/cyclic_dependencies/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      102 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/cyclic_dependencies/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/cyclic_dependencies/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/cyclic_dependencies.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.178011 stepup-1.2.0/docs/advanced_topics/environment_variables/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/environment_variables/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)      141 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/environment_variables/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)       91 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/environment_variables/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/environment_variables/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/environment_variables.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.178011 stepup-1.2.0/docs/advanced_topics/here_and_root/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/here_and_root/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)      242 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/here_and_root/main.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.178011 stepup-1.2.0/docs/advanced_topics/here_and_root/source/
--rwxr-xr-x   0 runner    (1001) docker     (127)      134 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/here_and_root/source/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.178011 stepup-1.2.0/docs/advanced_topics/here_and_root/source/sub/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/here_and_root/source/sub/example.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      164 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/here_and_root/source/sub/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/here_and_root/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/here_and_root.md
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/introduction.md
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/manual_cleaning.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.178011 stepup-1.2.0/docs/advanced_topics/optional_steps/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/optional_steps/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)      438 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/optional_steps/generate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      185 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/optional_steps/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/optional_steps/matplotlibrc
--rwxr-xr-x   0 runner    (1001) docker     (127)      170 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/optional_steps/plan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      503 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/optional_steps/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    62512 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/optional_steps/plot_logmap.png
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/optional_steps/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/optional_steps.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.182011 stepup-1.2.0/docs/advanced_topics/pools/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/pools/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)      131 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/pools/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      195 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/pools/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/pools/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/pools.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.182011 stepup-1.2.0/docs/advanced_topics/static_deferred_glob/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/static_deferred_glob/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/static_deferred_glob/bar.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/static_deferred_glob/foo.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/static_deferred_glob/graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/static_deferred_glob/graph_creator.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/static_deferred_glob/graph_supplier.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)      316 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/static_deferred_glob/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      178 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/static_deferred_glob/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/static_deferred_glob/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/static_deferred_glob.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.182011 stepup-1.2.0/docs/advanced_topics/static_named_glob/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/static_named_glob/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.182011 stepup-1.2.0/docs/advanced_topics/static_named_glob/ch1/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/static_named_glob/ch1/sec1_1_introduction.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/static_named_glob/ch1/sec1_2_objectives.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/static_named_glob/ch1/unused.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.182011 stepup-1.2.0/docs/advanced_topics/static_named_glob/ch2/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/static_named_glob/ch2/sec2_1_mathematical_requisites.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/static_named_glob/ch2/sec2_2_theory.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.182011 stepup-1.2.0/docs/advanced_topics/static_named_glob/ch3/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/static_named_glob/ch3/sec3_1_applications.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/static_named_glob/ch3/sec3_2_discussion.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.182011 stepup-1.2.0/docs/advanced_topics/static_named_glob/ch4/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/static_named_glob/ch4/sec4_1_summary.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      421 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/static_named_glob/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      647 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/static_named_glob/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/static_named_glob/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/static_named_glob.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.186011 stepup-1.2.0/docs/advanced_topics/variable_substitution/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/variable_substitution/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/variable_substitution/dst_foo.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      176 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/variable_substitution/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      186 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/variable_substitution/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/variable_substitution/src_foo.txt
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/variable_substitution/stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      177 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/variable_substitution/step.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/variable_substitution.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.186011 stepup-1.2.0/docs/advanced_topics/volatile_outputs/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/volatile_outputs/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)      132 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/volatile_outputs/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)       96 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/volatile_outputs/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/volatile_outputs/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/advanced_topics/volatile_outputs.md
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/clean_stdout.sed
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/development.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.186011 stepup-1.2.0/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/automatic_cleaning.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.186011 stepup-1.2.0/docs/getting_started/copy_mkdir/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/copy_mkdir/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)      132 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/copy_mkdir/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      157 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/copy_mkdir/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/copy_mkdir/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/copy_mkdir.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.190011 stepup-1.2.0/docs/getting_started/dependencies/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/dependencies/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/dependencies/graph_creator.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/dependencies/graph_supplier.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)      286 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/dependencies/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      233 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/dependencies/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/dependencies/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/dependencies.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.190011 stepup-1.2.0/docs/getting_started/distributed_plans/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/distributed_plans/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)      182 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/distributed_plans/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/distributed_plans/part1.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      137 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/distributed_plans/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/distributed_plans/stdout.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.190011 stepup-1.2.0/docs/getting_started/distributed_plans/sub/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/distributed_plans/sub/part2.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      140 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/distributed_plans/sub/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/distributed_plans.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.190011 stepup-1.2.0/docs/getting_started/first_step/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/first_step/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)      194 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/first_step/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)       81 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/first_step/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/first_step/stdout1.txt
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/first_step/stdout2.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/first_step.md
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/interactive_usage.md
--rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/introduction.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.190011 stepup-1.2.0/docs/getting_started/no_rules/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/no_rules/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/no_rules/lower1.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/no_rules/lower2.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      168 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/no_rules/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      229 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/no_rules/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/no_rules/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/no_rules.md
--rw-r--r--   0 runner    (1001) docker     (127)    16830 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/processes.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.194011 stepup-1.2.0/docs/getting_started/script_multiple/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/script_multiple/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    13493 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/script_multiple/ebbr.csv
--rw-r--r--   0 runner    (1001) docker     (127)    13550 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/script_multiple/ebos.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)      199 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/script_multiple/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/script_multiple/matplotlibrc
--rwxr-xr-x   0 runner    (1001) docker     (127)      142 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/script_multiple/plan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      962 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/script_multiple/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    60027 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/script_multiple/plot_ebbr.png
--rw-r--r--   0 runner    (1001) docker     (127)    69904 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/script_multiple/plot_ebos.png
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/script_multiple/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/script_multiple.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.194011 stepup-1.2.0/docs/getting_started/script_single/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/script_single/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/script_single/config.json
--rwxr-xr-x   0 runner    (1001) docker     (127)      508 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/script_single/generate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      170 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/script_single/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      125 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/script_single/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/script_single/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/script_single.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.194011 stepup-1.2.0/docs/getting_started/static_files/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/static_files/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/static_files/limerick.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      152 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/static_files/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      154 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/static_files/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/static_files/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/static_files.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.194011 stepup-1.2.0/docs/getting_started/static_glob/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/static_glob/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)      132 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/static_glob/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      168 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/static_glob/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.194011 stepup-1.2.0/docs/getting_started/static_glob/src/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/static_glob/src/bar.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/static_glob/src/foo.txt
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/static_glob/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/static_glob.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.198011 stepup-1.2.0/docs/getting_started/static_glob_conditional/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/static_glob_conditional/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.198011 stepup-1.2.0/docs/getting_started/static_glob_conditional/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/static_glob_conditional/dataset/bigfile.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      232 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/static_glob_conditional/expensive.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      244 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/static_glob_conditional/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      339 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/static_glob_conditional/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/static_glob_conditional/stdout1.txt
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/static_glob_conditional/stdout2.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/getting_started/static_glob_conditional.md
--rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/license.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     1846 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.198011 stepup-1.2.0/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/reference/interactive.md
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/reference/stepup.core.api.md
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/reference/stepup.core.interact.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      913 2024-05-02 09:23:07.000000 stepup-1.2.0/docs/run_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-02 09:23:07.000000 stepup-1.2.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-02 09:23:07.000000 stepup-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 09:23:18.310011 stepup-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.162011 stepup-1.2.0/stepup/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.202011 stepup-1.2.0/stepup/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-02 09:23:07.000000 stepup-1.2.0/stepup/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-02 09:23:18.000000 stepup-1.2.0/stepup/core/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    21298 2024-05-02 09:23:07.000000 stepup-1.2.0/stepup/core/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6986 2024-05-02 09:23:07.000000 stepup-1.2.0/stepup/core/assoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-02 09:23:07.000000 stepup-1.2.0/stepup/core/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)    19643 2024-05-02 09:23:07.000000 stepup-1.2.0/stepup/core/cascade.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-02 09:23:07.000000 stepup-1.2.0/stepup/core/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-02 09:23:07.000000 stepup-1.2.0/stepup/core/deferred_glob.py
--rw-r--r--   0 runner    (1001) docker     (127)    17076 2024-05-02 09:23:07.000000 stepup-1.2.0/stepup/core/director.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-02 09:23:07.000000 stepup-1.2.0/stepup/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7714 2024-05-02 09:23:07.000000 stepup-1.2.0/stepup/core/file.py
--rw-r--r--   0 runner    (1001) docker     (127)    12143 2024-05-02 09:23:07.000000 stepup-1.2.0/stepup/core/hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-05-02 09:23:07.000000 stepup-1.2.0/stepup/core/interact.py
--rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-05-02 09:23:07.000000 stepup-1.2.0/stepup/core/job.py
--rw-r--r--   0 runner    (1001) docker     (127)    21319 2024-05-02 09:23:07.000000 stepup-1.2.0/stepup/core/nglob.py
--rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-05-02 09:23:07.000000 stepup-1.2.0/stepup/core/pytest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-05-02 09:23:07.000000 stepup-1.2.0/stepup/core/reporter.py
--rw-r--r--   0 runner    (1001) docker     (127)    16273 2024-05-02 09:23:07.000000 stepup-1.2.0/stepup/core/rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    12497 2024-05-02 09:23:07.000000 stepup-1.2.0/stepup/core/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-05-02 09:23:07.000000 stepup-1.2.0/stepup/core/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    11749 2024-05-02 09:23:07.000000 stepup-1.2.0/stepup/core/script.py
--rw-r--r--   0 runner    (1001) docker     (127)    27113 2024-05-02 09:23:07.000000 stepup-1.2.0/stepup/core/step.py
--rw-r--r--   0 runner    (1001) docker     (127)     9068 2024-05-02 09:23:07.000000 stepup-1.2.0/stepup/core/tui.py
--rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-05-02 09:23:07.000000 stepup-1.2.0/stepup/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8362 2024-05-02 09:23:07.000000 stepup-1.2.0/stepup/core/watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    19950 2024-05-02 09:23:07.000000 stepup-1.2.0/stepup/core/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)    32915 2024-05-02 09:23:07.000000 stepup-1.2.0/stepup/core/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.306011 stepup-1.2.0/stepup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-02 09:23:18.000000 stepup-1.2.0/stepup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    33312 2024-05-02 09:23:18.000000 stepup-1.2.0/stepup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 09:23:18.000000 stepup-1.2.0/stepup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-02 09:23:18.000000 stepup-1.2.0/stepup.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-02 09:23:18.000000 stepup-1.2.0/stepup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 09:23:18.000000 stepup-1.2.0/stepup.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.206011 stepup-1.2.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.206011 stepup-1.2.0/tests/cases/
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.206011 stepup-1.2.0/tests/cases/amend/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend/expected_graph_03.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend/expected_graph_04.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend/expected_stdout_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend/expected_stdout_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend/expected_stdout_03.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend/inp1.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     2066 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      185 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend/plan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      249 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend/step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.210011 stepup-1.2.0/tests/cases/amend_delay/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend_delay/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend_delay/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend_delay/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend_delay/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend_delay/expected_graph_03.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend_delay/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1602 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend_delay/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      308 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend_delay/plan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      307 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend_delay/step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.210011 stepup-1.2.0/tests/cases/amend_env_vars/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend_env_vars/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend_env_vars/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend_env_vars/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend_env_vars/expected_stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend_env_vars/foo.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      692 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend_env_vars/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      100 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend_env_vars/plan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      475 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend_env_vars/step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.210011 stepup-1.2.0/tests/cases/amend_missing/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend_missing/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend_missing/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend_missing/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend_missing/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      562 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend_missing/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      189 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend_missing/plan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      203 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend_missing/step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.214011 stepup-1.2.0/tests/cases/amend_outdir_pending/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend_outdir_pending/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend_outdir_pending/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)       92 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend_outdir_pending/demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend_outdir_pending/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend_outdir_pending/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      534 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend_outdir_pending/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)       74 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend_outdir_pending/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.214011 stepup-1.2.0/tests/cases/amend_voldir_pending/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend_voldir_pending/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend_voldir_pending/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)       92 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend_voldir_pending/demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend_voldir_pending/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend_voldir_pending/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      534 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend_voldir_pending/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)       74 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/amend_voldir_pending/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.214011 stepup-1.2.0/tests/cases/deferred_glob1/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/deferred_glob1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/deferred_glob1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/deferred_glob1/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/deferred_glob1/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/deferred_glob1/expected_stdout_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/deferred_glob1/expected_stdout_02.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1213 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/deferred_glob1/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      153 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/deferred_glob1/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.214011 stepup-1.2.0/tests/cases/deferred_glob1/static/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/deferred_glob1/static/data1.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/deferred_glob1/static/data2.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.214011 stepup-1.2.0/tests/cases/deferred_glob1/static/sub/
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/deferred_glob1/static/sub/bar.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/deferred_glob1/static/sub/foo.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.218011 stepup-1.2.0/tests/cases/deferred_glob2/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/deferred_glob2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/deferred_glob2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/deferred_glob2/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/deferred_glob2/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/deferred_glob2/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      984 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/deferred_glob2/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      132 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/deferred_glob2/plan_01.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       87 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/deferred_glob2/plan_02.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.218011 stepup-1.2.0/tests/cases/deferred_glob2/static/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/deferred_glob2/static/data1.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/deferred_glob2/static/data2.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.218011 stepup-1.2.0/tests/cases/deferred_glob2/static/sub/
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/deferred_glob2/static/sub/bar.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/deferred_glob2/static/sub/foo.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.218011 stepup-1.2.0/tests/cases/deferred_subdir/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/deferred_subdir/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/deferred_subdir/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/deferred_subdir/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/deferred_subdir/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      599 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/deferred_subdir/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      107 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/deferred_subdir/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.218011 stepup-1.2.0/tests/cases/deferred_subdir/sub/
--rwxr-xr-x   0 runner    (1001) docker     (127)      119 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/deferred_subdir/sub/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/deferred_subdir/sub/unused.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/deferred_subdir/sub/used.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.222011 stepup-1.2.0/tests/cases/env_vars/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      242 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars/demovars.py
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars/expected_graph_03.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars/expected_graph_04.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars/expected_graph_05.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars/expected_stdout_a.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars/expected_stdout_b.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars/expected_stdout_c.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars/expected_stdout_d.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars/expected_variables_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars/expected_variables_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars/expected_variables_03.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars/expected_variables_04.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars/expected_variables_05.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     3193 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      183 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars/plan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      224 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars/printvars.py
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars/variables_01.json
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars/variables_02.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.226011 stepup-1.2.0/tests/cases/env_vars_amend/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars_amend/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars_amend/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      102 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars_amend/demovars.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars_amend/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars_amend/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars_amend/expected_stdout_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars_amend/expected_stdout_02.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1025 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars_amend/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      162 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars_amend/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.226011 stepup-1.2.0/tests/cases/env_vars_path/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars_path/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars_path/FOO.md
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars_path/FOO.txt
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars_path/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars_path/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars_path/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars_path/expected_stdout_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars_path/expected_stdout_02.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1255 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars_path/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      480 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars_path/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.226011 stepup-1.2.0/tests/cases/env_vars_subs/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars_subs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars_subs/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars_subs/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars_subs/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      616 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars_subs/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      159 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars_subs/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.226011 stepup-1.2.0/tests/cases/env_vars_subs/sub/
--rwxr-xr-x   0 runner    (1001) docker     (127)      133 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars_subs/sub/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.230011 stepup-1.2.0/tests/cases/env_vars_workdir/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars_workdir/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars_workdir/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars_workdir/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars_workdir/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      644 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars_workdir/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      355 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars_workdir/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.230011 stepup-1.2.0/tests/cases/env_vars_workdir/sub/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/env_vars_workdir/sub/input.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.230011 stepup-1.2.0/tests/cases/error_cyclic_late/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_cyclic_late/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_cyclic_late/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_cyclic_late/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_cyclic_late/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      591 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_cyclic_late/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      164 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_cyclic_late/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.230011 stepup-1.2.0/tests/cases/error_deferred_nonexisting/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_deferred_nonexisting/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_deferred_nonexisting/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_deferred_nonexisting/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      573 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_deferred_nonexisting/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      162 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_deferred_nonexisting/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.230011 stepup-1.2.0/tests/cases/error_env_var/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_env_var/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_env_var/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_env_var/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_env_var/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      534 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_env_var/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      124 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_env_var/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.234011 stepup-1.2.0/tests/cases/error_main_fails/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_main_fails/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_main_fails/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_main_fails/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_main_fails/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_main_fails/expected_stdout_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_main_fails/expected_stdout_02.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1044 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_main_fails/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      101 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_main_fails/plan_01.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       36 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_main_fails/plan_02.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.234011 stepup-1.2.0/tests/cases/error_not_executable/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_not_executable/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_not_executable/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_not_executable/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      385 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_not_executable/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_not_executable/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.234011 stepup-1.2.0/tests/cases/error_overlap_deferred/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_overlap_deferred/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_overlap_deferred/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_overlap_deferred/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_overlap_deferred/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      564 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_overlap_deferred/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      157 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_overlap_deferred/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.238011 stepup-1.2.0/tests/cases/error_static_dir/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_static_dir/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_static_dir/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_static_dir/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_static_dir/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      534 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_static_dir/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      114 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_static_dir/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.238011 stepup-1.2.0/tests/cases/error_static_dir/subdir/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_static_dir/subdir/.keep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.238011 stepup-1.2.0/tests/cases/error_step/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_step/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_step/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_step/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_step/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      534 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_step/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      107 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/error_step/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.238011 stepup-1.2.0/tests/cases/here/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/here/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/here/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/here/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/here/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      724 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/here/main.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.238011 stepup-1.2.0/tests/cases/here/source/
--rwxr-xr-x   0 runner    (1001) docker     (127)      198 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/here/source/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.238011 stepup-1.2.0/tests/cases/here/source/www/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/here/source/www/index.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      130 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/here/source/www/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.242011 stepup-1.2.0/tests/cases/makedirs/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/makedirs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/makedirs/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      456 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/makedirs/bunch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/makedirs/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/makedirs/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      610 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/makedirs/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      170 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/makedirs/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.242011 stepup-1.2.0/tests/cases/mkdir/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/mkdir/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/mkdir/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.242011 stepup-1.2.0/tests/cases/mkdir/exists/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/mkdir/exists/.keep
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/mkdir/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/mkdir/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      599 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/mkdir/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      237 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/mkdir/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.242011 stepup-1.2.0/tests/cases/mkdir_error/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/mkdir_error/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/mkdir_error/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/mkdir_error/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/mkdir_error/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      534 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/mkdir_error/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)       79 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/mkdir_error/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.246011 stepup-1.2.0/tests/cases/nodata/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/nodata/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/nodata/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/nodata/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/nodata/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/nodata/expected_graph_03.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/nodata/expected_stdout_a.txt
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/nodata/expected_stdout_b.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1495 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/nodata/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/nodata/original.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      259 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/nodata/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.246011 stepup-1.2.0/tests/cases/noplan/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/noplan/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/noplan/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/noplan/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      294 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/noplan/main.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.246011 stepup-1.2.0/tests/cases/nostatic/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/nostatic/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/nostatic/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/nostatic/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/nostatic/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1082 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/nostatic/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      181 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/nostatic/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.246011 stepup-1.2.0/tests/cases/not_cyclic/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/not_cyclic/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/not_cyclic/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/not_cyclic/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/not_cyclic/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/not_cyclic/expected_graph_03.txt
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/not_cyclic/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1386 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/not_cyclic/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      211 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/not_cyclic/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.250011 stepup-1.2.0/tests/cases/optional_convert/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/optional_convert/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/optional_convert/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/optional_convert/expected_graph_a.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/optional_convert/expected_graph_b.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/optional_convert/expected_graph_c.txt
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/optional_convert/expected_stdout_a.txt
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/optional_convert/expected_stdout_b.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1540 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/optional_convert/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      253 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/optional_convert/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/optional_convert/raw_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/optional_convert/raw_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/optional_convert/raw_03.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/optional_convert/raw_04.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.250011 stepup-1.2.0/tests/cases/output_not_created/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/output_not_created/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/output_not_created/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/output_not_created/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/output_not_created/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      627 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/output_not_created/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      169 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/output_not_created/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.250011 stepup-1.2.0/tests/cases/pending/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/pending/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/pending/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/pending/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/pending/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      534 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/pending/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      143 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/pending/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.254011 stepup-1.2.0/tests/cases/permissions_file_rerun/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/permissions_file_rerun/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/permissions_file_rerun/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/permissions_file_rerun/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/permissions_file_rerun/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/permissions_file_rerun/expected_stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/permissions_file_rerun/input.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1198 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/permissions_file_rerun/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      116 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/permissions_file_rerun/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.254011 stepup-1.2.0/tests/cases/permissions_plan_rerun/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/permissions_plan_rerun/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/permissions_plan_rerun/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/permissions_plan_rerun/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/permissions_plan_rerun/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/permissions_plan_rerun/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      984 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/permissions_plan_rerun/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      107 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/permissions_plan_rerun/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.254011 stepup-1.2.0/tests/cases/permissions_plan_rerun/sub/
--rwxr-xr-x   0 runner    (1001) docker     (127)       95 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/permissions_plan_rerun/sub/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.254011 stepup-1.2.0/tests/cases/permissions_plan_restart/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/permissions_plan_restart/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/permissions_plan_restart/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/permissions_plan_restart/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/permissions_plan_restart/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/permissions_plan_restart/expected_stdout_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/permissions_plan_restart/expected_stdout_02.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1140 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/permissions_plan_restart/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      107 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/permissions_plan_restart/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.254011 stepup-1.2.0/tests/cases/permissions_plan_restart/sub/
--rwxr-xr-x   0 runner    (1001) docker     (127)       95 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/permissions_plan_restart/sub/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.258011 stepup-1.2.0/tests/cases/permissions_step_rerun/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/permissions_step_rerun/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/permissions_step_rerun/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/permissions_step_rerun/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/permissions_step_rerun/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/permissions_step_rerun/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      962 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/permissions_step_rerun/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      115 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/permissions_step_rerun/plan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       95 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/permissions_step_rerun/step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.258011 stepup-1.2.0/tests/cases/permissions_step_restart/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/permissions_step_restart/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/permissions_step_restart/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/permissions_step_restart/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/permissions_step_restart/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/permissions_step_restart/expected_stdout_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/permissions_step_restart/expected_stdout_02.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1058 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/permissions_step_restart/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      115 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/permissions_step_restart/plan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       95 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/permissions_step_restart/step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.262011 stepup-1.2.0/tests/cases/pool/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/pool/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/pool/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/pool/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/pool/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      588 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/pool/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      316 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/pool/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/pool/r.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.262011 stepup-1.2.0/tests/cases/reqdir_missing/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/reqdir_missing/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/reqdir_missing/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/reqdir_missing/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/reqdir_missing/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      605 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/reqdir_missing/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      136 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/reqdir_missing/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.262011 stepup-1.2.0/tests/cases/restart_blocked/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_blocked/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_blocked/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_blocked/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_blocked/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_blocked/expected_stdout_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_blocked/expected_stdout_02.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      210 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_blocked/expensive.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_blocked/initial.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1052 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_blocked/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      261 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_blocked/plan_blocked.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      249 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_blocked/plan_unblocked.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.266011 stepup-1.2.0/tests/cases/restart_changes/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_changes/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_changes/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_changes/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_changes/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_changes/expected_stdout_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_changes/expected_stdout_02.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1394 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_changes/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      301 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_changes/plan_01.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      301 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_changes/plan_02.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_changes/source_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_changes/source_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_changes/source_both.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.266011 stepup-1.2.0/tests/cases/restart_deferred_glob/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_deferred_glob/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_deferred_glob/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_deferred_glob/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_deferred_glob/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_deferred_glob/expected_stdout_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_deferred_glob/expected_stdout_02.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      944 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_deferred_glob/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      142 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_deferred_glob/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.266011 stepup-1.2.0/tests/cases/restart_deferred_glob/static/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_deferred_glob/static/foo.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.266011 stepup-1.2.0/tests/cases/restart_nochanges/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_nochanges/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_nochanges/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_nochanges/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_nochanges/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_nochanges/expected_stdout_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_nochanges/expected_stdout_02.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1066 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_nochanges/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      296 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_nochanges/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.270011 stepup-1.2.0/tests/cases/restart_orphan/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_orphan/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_orphan/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_orphan/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_orphan/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_orphan/expected_stdout_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_orphan/expected_stdout_02.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      986 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_orphan/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      132 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_orphan/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.270011 stepup-1.2.0/tests/cases/restart_outdated_amend/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_outdated_amend/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_outdated_amend/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_outdated_amend/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_outdated_amend/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_outdated_amend/expected_stdout_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_outdated_amend/expected_stdout_02.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1139 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_outdated_amend/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      164 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_outdated_amend/plan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      271 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_outdated_amend/step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.274011 stepup-1.2.0/tests/cases/restart_output/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_output/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_output/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_output/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_output/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_output/expected_stdout_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_output/expected_stdout_02.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      964 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_output/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_output/original.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      120 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/restart_output/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.274011 stepup-1.2.0/tests/cases/script_cases/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/script_cases/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/script_cases/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/script_cases/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/script_cases/expected_stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/script_cases/helper.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      658 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/script_cases/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      115 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/script_cases/plan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      397 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/script_cases/work.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.274011 stepup-1.2.0/tests/cases/script_cases_settings/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/script_cases_settings/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/script_cases_settings/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/script_cases_settings/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/script_cases_settings/expected_stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/script_cases_settings/helper.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      658 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/script_cases_settings/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      130 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/script_cases_settings/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/script_cases_settings/settings.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      423 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/script_cases_settings/work.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.278011 stepup-1.2.0/tests/cases/script_single/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/script_single/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/script_single/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/script_single/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/script_single/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      639 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/script_single/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      193 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/script_single/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.278011 stepup-1.2.0/tests/cases/script_single/work/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/script_single/work/config.json
--rwxr-xr-x   0 runner    (1001) docker     (127)      554 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/script_single/work/generate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.278011 stepup-1.2.0/tests/cases/static/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      567 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static/original.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)       81 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.278011 stepup-1.2.0/tests/cases/static_abs/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_abs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_abs/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_abs/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_abs/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      567 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_abs/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_abs/original.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      103 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_abs/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.282011 stepup-1.2.0/tests/cases/static_dir/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_dir/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_dir/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_dir/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_dir/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      595 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_dir/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)       76 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_dir/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.282011 stepup-1.2.0/tests/cases/static_glob/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_glob/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_glob/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_glob/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_glob/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_glob/expected_graph_03.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_glob/expected_stdout_a.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_glob/expected_stdout_b.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1686 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_glob/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      137 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_glob/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.282011 stepup-1.2.0/tests/cases/static_nglob/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_nglob/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_nglob/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.282011 stepup-1.2.0/tests/cases/static_nglob/ch-1-intro/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_nglob/ch-1-intro/sec-1-1-blabla.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_nglob/ch-1-intro/sec-1-2-some-more.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.282011 stepup-1.2.0/tests/cases/static_nglob/ch-2-theory/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_nglob/ch-2-theory/sec-2-1-basics.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.286011 stepup-1.2.0/tests/cases/static_nglob/ch-3-conclusions/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_nglob/ch-3-conclusions/sec-3-1-summary.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_nglob/ch-3-conclusions/sec-3-2-outlook.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18883 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_nglob/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18883 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_nglob/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_nglob/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     2740 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_nglob/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      972 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_nglob/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_nglob/sec-2-2.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.286011 stepup-1.2.0/tests/cases/static_nglob_partial/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_nglob_partial/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_nglob_partial/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_nglob_partial/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_nglob_partial/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_nglob_partial/expected_graph_03.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_nglob_partial/expected_graph_04.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_nglob_partial/expected_stdout_a.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_nglob_partial/expected_stdout_b.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     2132 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_nglob_partial/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      297 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_nglob_partial/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.286011 stepup-1.2.0/tests/cases/static_nglob_subdir/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_nglob_subdir/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_nglob_subdir/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_nglob_subdir/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_nglob_subdir/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      742 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_nglob_subdir/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      107 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_nglob_subdir/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.286011 stepup-1.2.0/tests/cases/static_nglob_subdir/sub/
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_nglob_subdir/sub/inp1.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_nglob_subdir/sub/inp2.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      151 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/static_nglob_subdir/sub/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.290011 stepup-1.2.0/tests/cases/subdir/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/subdir/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/subdir/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/subdir/example.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/subdir/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/subdir/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      636 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/subdir/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      170 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/subdir/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.290011 stepup-1.2.0/tests/cases/subdir/sub/
--rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/subdir/sub/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.290011 stepup-1.2.0/tests/cases/watch_blocked/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_blocked/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_blocked/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_blocked/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_blocked/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_blocked/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      210 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_blocked/expensive.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_blocked/initial.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      961 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_blocked/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      261 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_blocked/plan_blocked.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      249 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_blocked/plan_unblocked.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.294011 stepup-1.2.0/tests/cases/watch_boot/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_boot/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_boot/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_boot/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_boot/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_boot/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      983 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_boot/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      178 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_boot/plan_01.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      182 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_boot/plan_02.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.294011 stepup-1.2.0/tests/cases/watch_chain/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_chain/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_chain/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_chain/config_01.json
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_chain/config_02.json
--rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_chain/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_chain/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_chain/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1069 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_chain/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      229 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_chain/plan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      545 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_chain/use_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.298011 stepup-1.2.0/tests/cases/watch_input/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_input/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_input/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_input/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_input/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_input/expected_graph_03.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_input/expected_stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_input/first.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      940 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_input/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      155 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_input/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_input/second.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.298011 stepup-1.2.0/tests/cases/watch_middle/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_middle/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_middle/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_middle/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_middle/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_middle/expected_graph_03.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_middle/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1158 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_middle/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_middle/original.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      235 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_middle/plan_01.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      247 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_middle/plan_02.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.302011 stepup-1.2.0/tests/cases/watch_mixed/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_mixed/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_mixed/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_mixed/backup.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_mixed/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_mixed/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_mixed/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      825 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_mixed/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      219 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_mixed/plan_full.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      125 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_mixed/plan_trimmed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.302011 stepup-1.2.0/tests/cases/watch_nochanges/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_nochanges/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_nochanges/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_nochanges/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_nochanges/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_nochanges/expected_stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_nochanges/input.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      876 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_nochanges/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      155 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_nochanges/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.302011 stepup-1.2.0/tests/cases/watch_outdated_amend1/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_outdated_amend1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_outdated_amend1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_outdated_amend1/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_outdated_amend1/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_outdated_amend1/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1071 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_outdated_amend1/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      164 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_outdated_amend1/plan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      271 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_outdated_amend1/step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.306011 stepup-1.2.0/tests/cases/watch_outdated_amend2/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_outdated_amend2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_outdated_amend2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_outdated_amend2/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_outdated_amend2/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_outdated_amend2/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1260 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_outdated_amend2/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      331 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_outdated_amend2/plan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      167 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_outdated_amend2/step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.306011 stepup-1.2.0/tests/cases/watch_output/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_output/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_output/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_output/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_output/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_output/expected_stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_output/input.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      920 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_output/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      116 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_output/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_output/second.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:23:18.306011 stepup-1.2.0/tests/cases/watch_wanted/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_wanted/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_wanted/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_wanted/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_wanted/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_wanted/expected_graph_03.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_wanted/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1538 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_wanted/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      328 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_wanted/plan_01.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      105 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/cases/watch_wanted/plan_02.py
--rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/core_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/echo_server_socket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/echo_server_stdio.py
--rw-r--r--   0 runner    (1001) docker     (127)     9480 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/test_assoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (127)    15868 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/test_cascade.py
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/test_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/test_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)    21262 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/test_nglob.py
--rw-r--r--   0 runner    (1001) docker     (127)     7996 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/test_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9091 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    65158 2024-05-02 09:23:07.000000 stepup-1.2.0/tests/test_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.341539 stepup-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-07 17:53:00.000000 stepup-1.2.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.185540 stepup-1.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.201540 stepup-1.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-07 17:53:00.000000 stepup-1.2.1/.github/workflows/mkdocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-07 17:53:00.000000 stepup-1.2.1/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-07 17:53:00.000000 stepup-1.2.1/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-07 17:53:00.000000 stepup-1.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-07 17:53:00.000000 stepup-1.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-07 17:53:00.000000 stepup-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-07 17:53:04.341539 stepup-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-07 17:53:00.000000 stepup-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.201540 stepup-1.2.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.205540 stepup-1.2.1/docs/advanced_topics/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.205540 stepup-1.2.1/docs/advanced_topics/amending_static_inputs/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/amending_static_inputs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/amending_static_inputs/config.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      149 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/amending_static_inputs/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      170 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/amending_static_inputs/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/amending_static_inputs/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/amending_static_inputs.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.205540 stepup-1.2.1/docs/advanced_topics/amending_steps/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/amending_steps/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      146 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/amending_steps/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      262 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/amending_steps/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/amending_steps/stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      465 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/amending_steps/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/amending_steps.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.205540 stepup-1.2.1/docs/advanced_topics/blocked_steps/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/blocked_steps/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      131 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/blocked_steps/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      161 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/blocked_steps/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/blocked_steps/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/blocked_steps.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.209540 stepup-1.2.1/docs/advanced_topics/cyclic_dependencies/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/cyclic_dependencies/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      131 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/cyclic_dependencies/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      102 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/cyclic_dependencies/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/cyclic_dependencies/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/cyclic_dependencies.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.209540 stepup-1.2.1/docs/advanced_topics/environment_variables/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/environment_variables/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      141 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/environment_variables/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       91 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/environment_variables/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/environment_variables/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/environment_variables.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.209540 stepup-1.2.1/docs/advanced_topics/here_and_root/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/here_and_root/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      242 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/here_and_root/main.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.209540 stepup-1.2.1/docs/advanced_topics/here_and_root/source/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      134 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/here_and_root/source/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.209540 stepup-1.2.1/docs/advanced_topics/here_and_root/source/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/here_and_root/source/sub/example.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      164 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/here_and_root/source/sub/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/here_and_root/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/here_and_root.md
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/introduction.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/manual_cleaning.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.209540 stepup-1.2.1/docs/advanced_topics/optional_steps/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/optional_steps/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      438 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/optional_steps/generate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      185 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/optional_steps/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/optional_steps/matplotlibrc
+-rwxr-xr-x   0 runner    (1001) docker     (127)      170 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/optional_steps/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      504 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/optional_steps/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62512 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/optional_steps/plot_logmap.png
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/optional_steps/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/optional_steps.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.209540 stepup-1.2.1/docs/advanced_topics/pools/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/pools/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      131 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/pools/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      195 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/pools/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/pools/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/pools.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.213540 stepup-1.2.1/docs/advanced_topics/static_deferred_glob/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/static_deferred_glob/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/static_deferred_glob/bar.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/static_deferred_glob/foo.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/static_deferred_glob/graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/static_deferred_glob/graph_creator.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/static_deferred_glob/graph_supplier.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      316 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/static_deferred_glob/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      178 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/static_deferred_glob/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/static_deferred_glob/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/static_deferred_glob.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.213540 stepup-1.2.1/docs/advanced_topics/static_named_glob/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/static_named_glob/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.213540 stepup-1.2.1/docs/advanced_topics/static_named_glob/ch1/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/static_named_glob/ch1/sec1_1_introduction.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/static_named_glob/ch1/sec1_2_objectives.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/static_named_glob/ch1/unused.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.213540 stepup-1.2.1/docs/advanced_topics/static_named_glob/ch2/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/static_named_glob/ch2/sec2_1_mathematical_requisites.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/static_named_glob/ch2/sec2_2_theory.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.213540 stepup-1.2.1/docs/advanced_topics/static_named_glob/ch3/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/static_named_glob/ch3/sec3_1_applications.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/static_named_glob/ch3/sec3_2_discussion.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.213540 stepup-1.2.1/docs/advanced_topics/static_named_glob/ch4/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/static_named_glob/ch4/sec4_1_summary.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      421 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/static_named_glob/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      647 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/static_named_glob/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/static_named_glob/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/static_named_glob.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.217540 stepup-1.2.1/docs/advanced_topics/variable_substitution/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/variable_substitution/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/variable_substitution/dst_foo.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      176 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/variable_substitution/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      186 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/variable_substitution/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/variable_substitution/src_foo.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/variable_substitution/stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      178 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/variable_substitution/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/variable_substitution.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.217540 stepup-1.2.1/docs/advanced_topics/volatile_outputs/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/volatile_outputs/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      132 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/volatile_outputs/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       96 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/volatile_outputs/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/volatile_outputs/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/advanced_topics/volatile_outputs.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/clean_stdout.sed
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/development.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.217540 stepup-1.2.1/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/automatic_cleaning.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.217540 stepup-1.2.1/docs/getting_started/copy_mkdir/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/copy_mkdir/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      132 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/copy_mkdir/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      157 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/copy_mkdir/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/copy_mkdir/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/copy_mkdir.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.221540 stepup-1.2.1/docs/getting_started/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/dependencies/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/dependencies/graph_creator.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/dependencies/graph_supplier.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      286 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/dependencies/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      233 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/dependencies/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/dependencies/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/dependencies.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.221540 stepup-1.2.1/docs/getting_started/distributed_plans/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/distributed_plans/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      182 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/distributed_plans/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/distributed_plans/part1.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      137 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/distributed_plans/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/distributed_plans/stdout.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.221540 stepup-1.2.1/docs/getting_started/distributed_plans/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/distributed_plans/sub/part2.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      140 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/distributed_plans/sub/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/distributed_plans.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.221540 stepup-1.2.1/docs/getting_started/first_step/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/first_step/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      194 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/first_step/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       81 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/first_step/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/first_step/stdout1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/first_step/stdout2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/first_step.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/interactive_usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/introduction.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.221540 stepup-1.2.1/docs/getting_started/no_rules/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/no_rules/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/no_rules/lower1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/no_rules/lower2.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      168 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/no_rules/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      229 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/no_rules/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/no_rules/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/no_rules.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16830 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/processes.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.225540 stepup-1.2.1/docs/getting_started/script_multiple/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/script_multiple/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    13493 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/script_multiple/ebbr.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    13550 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/script_multiple/ebos.csv
+-rwxr-xr-x   0 runner    (1001) docker     (127)      199 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/script_multiple/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/script_multiple/matplotlibrc
+-rwxr-xr-x   0 runner    (1001) docker     (127)      142 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/script_multiple/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      963 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/script_multiple/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60027 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/script_multiple/plot_ebbr.png
+-rw-r--r--   0 runner    (1001) docker     (127)    69904 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/script_multiple/plot_ebos.png
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/script_multiple/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/script_multiple.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.225540 stepup-1.2.1/docs/getting_started/script_single/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/script_single/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/script_single/config.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)      509 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/script_single/generate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      170 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/script_single/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      125 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/script_single/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/script_single/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/script_single.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.225540 stepup-1.2.1/docs/getting_started/static_files/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/static_files/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/static_files/limerick.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      152 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/static_files/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      154 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/static_files/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/static_files/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/static_files.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.229540 stepup-1.2.1/docs/getting_started/static_glob/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/static_glob/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      132 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/static_glob/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      168 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/static_glob/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.229540 stepup-1.2.1/docs/getting_started/static_glob/src/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/static_glob/src/bar.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/static_glob/src/foo.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/static_glob/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/static_glob.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.229540 stepup-1.2.1/docs/getting_started/static_glob_conditional/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/static_glob_conditional/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.229540 stepup-1.2.1/docs/getting_started/static_glob_conditional/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/static_glob_conditional/dataset/bigfile.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      232 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/static_glob_conditional/expensive.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      244 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/static_glob_conditional/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      339 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/static_glob_conditional/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/static_glob_conditional/stdout1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/static_glob_conditional/stdout2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/getting_started/static_glob_conditional.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/license.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1847 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.229540 stepup-1.2.1/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/reference/interactive.md
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/reference/stepup.core.api.md
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/reference/stepup.core.interact.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      927 2024-05-07 17:53:00.000000 stepup-1.2.1/docs/run_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-07 17:53:00.000000 stepup-1.2.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-05-07 17:53:00.000000 stepup-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 17:53:04.341539 stepup-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.189540 stepup-1.2.1/stepup/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.237540 stepup-1.2.1/stepup/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-07 17:53:00.000000 stepup-1.2.1/stepup/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21303 2024-05-07 17:53:00.000000 stepup-1.2.1/stepup/core/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-05-07 17:53:00.000000 stepup-1.2.1/stepup/core/assoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-05-07 17:53:00.000000 stepup-1.2.1/stepup/core/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19597 2024-05-07 17:53:00.000000 stepup-1.2.1/stepup/core/cascade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-07 17:53:00.000000 stepup-1.2.1/stepup/core/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-07 17:53:00.000000 stepup-1.2.1/stepup/core/deferred_glob.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17076 2024-05-07 17:53:00.000000 stepup-1.2.1/stepup/core/director.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-07 17:53:00.000000 stepup-1.2.1/stepup/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7725 2024-05-07 17:53:00.000000 stepup-1.2.1/stepup/core/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12144 2024-05-07 17:53:00.000000 stepup-1.2.1/stepup/core/hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-07 17:53:00.000000 stepup-1.2.1/stepup/core/interact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-05-07 17:53:00.000000 stepup-1.2.1/stepup/core/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21318 2024-05-07 17:53:00.000000 stepup-1.2.1/stepup/core/nglob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-05-07 17:53:00.000000 stepup-1.2.1/stepup/core/pytest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-05-07 17:53:00.000000 stepup-1.2.1/stepup/core/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16280 2024-05-07 17:53:00.000000 stepup-1.2.1/stepup/core/rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12450 2024-05-07 17:53:00.000000 stepup-1.2.1/stepup/core/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-05-07 17:53:00.000000 stepup-1.2.1/stepup/core/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11775 2024-05-07 17:53:00.000000 stepup-1.2.1/stepup/core/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27140 2024-05-07 17:53:00.000000 stepup-1.2.1/stepup/core/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9128 2024-05-07 17:53:00.000000 stepup-1.2.1/stepup/core/tui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7024 2024-05-07 17:53:00.000000 stepup-1.2.1/stepup/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8377 2024-05-07 17:53:00.000000 stepup-1.2.1/stepup/core/watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19965 2024-05-07 17:53:00.000000 stepup-1.2.1/stepup/core/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32855 2024-05-07 17:53:00.000000 stepup-1.2.1/stepup/core/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.341539 stepup-1.2.1/stepup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-07 17:53:04.000000 stepup-1.2.1/stepup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    33288 2024-05-07 17:53:04.000000 stepup-1.2.1/stepup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 17:53:04.000000 stepup-1.2.1/stepup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-07 17:53:04.000000 stepup-1.2.1/stepup.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-07 17:53:04.000000 stepup-1.2.1/stepup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 17:53:04.000000 stepup-1.2.1/stepup.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.237540 stepup-1.2.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.237540 stepup-1.2.1/tests/cases/
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.241540 stepup-1.2.1/tests/cases/amend/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend/expected_graph_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend/expected_graph_04.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend/expected_stdout_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend/expected_stdout_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend/inp1.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2066 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      185 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      250 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend/step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.241540 stepup-1.2.1/tests/cases/amend_delay/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend_delay/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend_delay/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend_delay/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend_delay/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend_delay/expected_graph_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend_delay/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1602 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend_delay/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      308 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend_delay/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      307 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend_delay/step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.245540 stepup-1.2.1/tests/cases/amend_env_vars/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend_env_vars/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend_env_vars/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend_env_vars/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend_env_vars/expected_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend_env_vars/foo.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      692 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend_env_vars/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      100 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend_env_vars/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      475 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend_env_vars/step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.245540 stepup-1.2.1/tests/cases/amend_missing/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend_missing/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend_missing/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend_missing/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend_missing/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      562 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend_missing/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      189 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend_missing/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      204 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend_missing/step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.245540 stepup-1.2.1/tests/cases/amend_outdir_pending/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend_outdir_pending/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend_outdir_pending/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)       92 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend_outdir_pending/demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend_outdir_pending/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend_outdir_pending/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      534 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend_outdir_pending/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       74 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend_outdir_pending/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.249540 stepup-1.2.1/tests/cases/amend_voldir_pending/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend_voldir_pending/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend_voldir_pending/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)       92 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend_voldir_pending/demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend_voldir_pending/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend_voldir_pending/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      534 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend_voldir_pending/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       74 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/amend_voldir_pending/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.249540 stepup-1.2.1/tests/cases/deferred_glob1/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/deferred_glob1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/deferred_glob1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/deferred_glob1/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/deferred_glob1/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/deferred_glob1/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/deferred_glob1/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1213 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/deferred_glob1/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      153 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/deferred_glob1/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.249540 stepup-1.2.1/tests/cases/deferred_glob1/static/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/deferred_glob1/static/data1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/deferred_glob1/static/data2.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.249540 stepup-1.2.1/tests/cases/deferred_glob1/static/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/deferred_glob1/static/sub/bar.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/deferred_glob1/static/sub/foo.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.249540 stepup-1.2.1/tests/cases/deferred_glob2/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/deferred_glob2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/deferred_glob2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/deferred_glob2/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/deferred_glob2/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/deferred_glob2/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      984 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/deferred_glob2/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      132 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/deferred_glob2/plan_01.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       87 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/deferred_glob2/plan_02.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.253540 stepup-1.2.1/tests/cases/deferred_glob2/static/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/deferred_glob2/static/data1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/deferred_glob2/static/data2.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.253540 stepup-1.2.1/tests/cases/deferred_glob2/static/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/deferred_glob2/static/sub/bar.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/deferred_glob2/static/sub/foo.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.253540 stepup-1.2.1/tests/cases/deferred_subdir/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/deferred_subdir/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/deferred_subdir/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/deferred_subdir/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/deferred_subdir/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      599 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/deferred_subdir/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      107 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/deferred_subdir/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.253540 stepup-1.2.1/tests/cases/deferred_subdir/sub/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      119 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/deferred_subdir/sub/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/deferred_subdir/sub/unused.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/deferred_subdir/sub/used.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.257540 stepup-1.2.1/tests/cases/env_vars/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      242 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars/demovars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars/expected_graph_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars/expected_graph_04.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars/expected_graph_05.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars/expected_stdout_a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars/expected_stdout_b.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars/expected_stdout_c.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars/expected_stdout_d.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars/expected_variables_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars/expected_variables_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars/expected_variables_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars/expected_variables_04.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars/expected_variables_05.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3193 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      183 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      223 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars/printvars.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars/variables_01.json
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars/variables_02.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.257540 stepup-1.2.1/tests/cases/env_vars_amend/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars_amend/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars_amend/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      102 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars_amend/demovars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars_amend/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars_amend/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars_amend/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars_amend/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1025 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars_amend/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      162 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars_amend/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.261540 stepup-1.2.1/tests/cases/env_vars_path/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars_path/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars_path/FOO.md
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars_path/FOO.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars_path/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars_path/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars_path/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars_path/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars_path/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1255 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars_path/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      480 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars_path/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.261540 stepup-1.2.1/tests/cases/env_vars_subs/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars_subs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars_subs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars_subs/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars_subs/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      616 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars_subs/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      159 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars_subs/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.261540 stepup-1.2.1/tests/cases/env_vars_subs/sub/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      133 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars_subs/sub/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.261540 stepup-1.2.1/tests/cases/env_vars_workdir/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars_workdir/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars_workdir/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars_workdir/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars_workdir/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      644 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars_workdir/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      355 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars_workdir/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.261540 stepup-1.2.1/tests/cases/env_vars_workdir/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/env_vars_workdir/sub/input.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.265540 stepup-1.2.1/tests/cases/error_cyclic_late/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_cyclic_late/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_cyclic_late/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_cyclic_late/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_cyclic_late/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      591 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_cyclic_late/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      164 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_cyclic_late/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.265540 stepup-1.2.1/tests/cases/error_deferred_nonexisting/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_deferred_nonexisting/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_deferred_nonexisting/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_deferred_nonexisting/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      573 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_deferred_nonexisting/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      162 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_deferred_nonexisting/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.265540 stepup-1.2.1/tests/cases/error_env_var/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_env_var/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_env_var/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_env_var/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_env_var/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      534 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_env_var/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      124 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_env_var/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.269540 stepup-1.2.1/tests/cases/error_main_fails/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_main_fails/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_main_fails/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_main_fails/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_main_fails/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_main_fails/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_main_fails/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1044 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_main_fails/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      101 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_main_fails/plan_01.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       46 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_main_fails/plan_02.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.269540 stepup-1.2.1/tests/cases/error_not_executable/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_not_executable/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_not_executable/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_not_executable/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      385 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_not_executable/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_not_executable/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.269540 stepup-1.2.1/tests/cases/error_overlap_deferred/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_overlap_deferred/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_overlap_deferred/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_overlap_deferred/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_overlap_deferred/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      564 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_overlap_deferred/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      157 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_overlap_deferred/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.269540 stepup-1.2.1/tests/cases/error_static_dir/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_static_dir/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_static_dir/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_static_dir/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_static_dir/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      534 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_static_dir/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      114 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_static_dir/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.269540 stepup-1.2.1/tests/cases/error_static_dir/subdir/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_static_dir/subdir/.keep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.273540 stepup-1.2.1/tests/cases/error_step/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_step/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_step/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_step/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_step/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      534 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_step/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      107 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/error_step/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.273540 stepup-1.2.1/tests/cases/here/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/here/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/here/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/here/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/here/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      724 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/here/main.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.273540 stepup-1.2.1/tests/cases/here/source/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      198 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/here/source/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.273540 stepup-1.2.1/tests/cases/here/source/www/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/here/source/www/index.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      130 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/here/source/www/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.273540 stepup-1.2.1/tests/cases/makedirs/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/makedirs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/makedirs/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      457 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/makedirs/bunch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/makedirs/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/makedirs/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      610 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/makedirs/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      170 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/makedirs/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.277540 stepup-1.2.1/tests/cases/mkdir/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/mkdir/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/mkdir/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.277540 stepup-1.2.1/tests/cases/mkdir/exists/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/mkdir/exists/.keep
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/mkdir/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/mkdir/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      599 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/mkdir/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      237 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/mkdir/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.277540 stepup-1.2.1/tests/cases/mkdir_error/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/mkdir_error/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/mkdir_error/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/mkdir_error/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/mkdir_error/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      534 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/mkdir_error/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       79 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/mkdir_error/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.277540 stepup-1.2.1/tests/cases/nodata/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/nodata/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/nodata/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/nodata/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/nodata/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/nodata/expected_graph_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/nodata/expected_stdout_a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/nodata/expected_stdout_b.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1495 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/nodata/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/nodata/original.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      259 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/nodata/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.281540 stepup-1.2.1/tests/cases/noplan/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/noplan/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/noplan/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/noplan/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      294 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/noplan/main.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.281540 stepup-1.2.1/tests/cases/nostatic/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/nostatic/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/nostatic/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/nostatic/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/nostatic/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1082 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/nostatic/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      181 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/nostatic/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.281540 stepup-1.2.1/tests/cases/not_cyclic/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/not_cyclic/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/not_cyclic/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/not_cyclic/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/not_cyclic/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/not_cyclic/expected_graph_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/not_cyclic/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1386 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/not_cyclic/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      211 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/not_cyclic/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.285539 stepup-1.2.1/tests/cases/optional_convert/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/optional_convert/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/optional_convert/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/optional_convert/expected_graph_a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/optional_convert/expected_graph_b.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/optional_convert/expected_graph_c.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/optional_convert/expected_stdout_a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/optional_convert/expected_stdout_b.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1540 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/optional_convert/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      253 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/optional_convert/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/optional_convert/raw_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/optional_convert/raw_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/optional_convert/raw_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/optional_convert/raw_04.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.285539 stepup-1.2.1/tests/cases/output_not_created/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/output_not_created/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/output_not_created/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/output_not_created/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/output_not_created/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      627 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/output_not_created/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      169 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/output_not_created/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.285539 stepup-1.2.1/tests/cases/pending/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/pending/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/pending/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/pending/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/pending/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      534 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/pending/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      143 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/pending/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.289539 stepup-1.2.1/tests/cases/permissions_file_rerun/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/permissions_file_rerun/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/permissions_file_rerun/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/permissions_file_rerun/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/permissions_file_rerun/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/permissions_file_rerun/expected_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/permissions_file_rerun/input.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1198 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/permissions_file_rerun/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      116 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/permissions_file_rerun/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.289539 stepup-1.2.1/tests/cases/permissions_plan_rerun/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/permissions_plan_rerun/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/permissions_plan_rerun/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/permissions_plan_rerun/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/permissions_plan_rerun/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/permissions_plan_rerun/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      984 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/permissions_plan_rerun/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      107 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/permissions_plan_rerun/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.289539 stepup-1.2.1/tests/cases/permissions_plan_rerun/sub/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       95 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/permissions_plan_rerun/sub/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.289539 stepup-1.2.1/tests/cases/permissions_plan_restart/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/permissions_plan_restart/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/permissions_plan_restart/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/permissions_plan_restart/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/permissions_plan_restart/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/permissions_plan_restart/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/permissions_plan_restart/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1140 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/permissions_plan_restart/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      107 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/permissions_plan_restart/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.289539 stepup-1.2.1/tests/cases/permissions_plan_restart/sub/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       95 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/permissions_plan_restart/sub/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.293540 stepup-1.2.1/tests/cases/permissions_step_rerun/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/permissions_step_rerun/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/permissions_step_rerun/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/permissions_step_rerun/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/permissions_step_rerun/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/permissions_step_rerun/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      962 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/permissions_step_rerun/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      115 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/permissions_step_rerun/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       95 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/permissions_step_rerun/step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.293540 stepup-1.2.1/tests/cases/permissions_step_restart/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/permissions_step_restart/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/permissions_step_restart/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/permissions_step_restart/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/permissions_step_restart/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/permissions_step_restart/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/permissions_step_restart/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1058 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/permissions_step_restart/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      115 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/permissions_step_restart/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       95 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/permissions_step_restart/step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.293540 stepup-1.2.1/tests/cases/pool/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/pool/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/pool/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/pool/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/pool/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      588 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/pool/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      316 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/pool/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/pool/r.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.297540 stepup-1.2.1/tests/cases/reqdir_missing/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/reqdir_missing/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/reqdir_missing/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/reqdir_missing/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/reqdir_missing/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      605 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/reqdir_missing/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      136 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/reqdir_missing/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.297540 stepup-1.2.1/tests/cases/restart_blocked/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_blocked/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_blocked/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_blocked/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_blocked/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_blocked/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_blocked/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      210 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_blocked/expensive.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_blocked/initial.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1052 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_blocked/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      261 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_blocked/plan_blocked.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      249 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_blocked/plan_unblocked.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.301540 stepup-1.2.1/tests/cases/restart_changes/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_changes/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_changes/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_changes/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_changes/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_changes/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_changes/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1394 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_changes/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      301 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_changes/plan_01.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      301 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_changes/plan_02.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_changes/source_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_changes/source_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_changes/source_both.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.301540 stepup-1.2.1/tests/cases/restart_deferred_glob/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_deferred_glob/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_deferred_glob/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_deferred_glob/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_deferred_glob/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_deferred_glob/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_deferred_glob/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      944 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_deferred_glob/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      142 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_deferred_glob/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.301540 stepup-1.2.1/tests/cases/restart_deferred_glob/static/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_deferred_glob/static/foo.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.301540 stepup-1.2.1/tests/cases/restart_nochanges/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_nochanges/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_nochanges/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_nochanges/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_nochanges/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_nochanges/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_nochanges/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1066 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_nochanges/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      296 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_nochanges/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.305539 stepup-1.2.1/tests/cases/restart_orphan/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_orphan/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_orphan/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_orphan/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_orphan/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_orphan/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_orphan/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      986 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_orphan/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      132 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_orphan/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.305539 stepup-1.2.1/tests/cases/restart_outdated_amend/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_outdated_amend/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_outdated_amend/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_outdated_amend/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_outdated_amend/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_outdated_amend/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_outdated_amend/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1139 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_outdated_amend/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      164 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_outdated_amend/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      271 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_outdated_amend/step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.309539 stepup-1.2.1/tests/cases/restart_output/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_output/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_output/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_output/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_output/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_output/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_output/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      964 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_output/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_output/original.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      120 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/restart_output/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.309539 stepup-1.2.1/tests/cases/script_cases/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/script_cases/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/script_cases/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/script_cases/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/script_cases/expected_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/script_cases/helper.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      658 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/script_cases/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      115 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/script_cases/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      396 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/script_cases/work.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.309539 stepup-1.2.1/tests/cases/script_cases_settings/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/script_cases_settings/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/script_cases_settings/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/script_cases_settings/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/script_cases_settings/expected_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/script_cases_settings/helper.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      658 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/script_cases_settings/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      130 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/script_cases_settings/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/script_cases_settings/settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      422 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/script_cases_settings/work.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.313540 stepup-1.2.1/tests/cases/script_single/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/script_single/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/script_single/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/script_single/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/script_single/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      639 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/script_single/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      193 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/script_single/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.313540 stepup-1.2.1/tests/cases/script_single/work/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/script_single/work/config.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)      554 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/script_single/work/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.313540 stepup-1.2.1/tests/cases/static/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      567 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static/original.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)       81 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.313540 stepup-1.2.1/tests/cases/static_abs/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_abs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_abs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_abs/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_abs/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      567 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_abs/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_abs/original.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      103 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_abs/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.313540 stepup-1.2.1/tests/cases/static_dir/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_dir/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_dir/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_dir/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_dir/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      595 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_dir/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       76 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_dir/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.317540 stepup-1.2.1/tests/cases/static_glob/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_glob/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_glob/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_glob/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_glob/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_glob/expected_graph_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_glob/expected_stdout_a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_glob/expected_stdout_b.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1686 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_glob/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      137 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_glob/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.317540 stepup-1.2.1/tests/cases/static_nglob/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_nglob/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_nglob/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.317540 stepup-1.2.1/tests/cases/static_nglob/ch-1-intro/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_nglob/ch-1-intro/sec-1-1-blabla.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_nglob/ch-1-intro/sec-1-2-some-more.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.317540 stepup-1.2.1/tests/cases/static_nglob/ch-2-theory/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_nglob/ch-2-theory/sec-2-1-basics.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.317540 stepup-1.2.1/tests/cases/static_nglob/ch-3-conclusions/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_nglob/ch-3-conclusions/sec-3-1-summary.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_nglob/ch-3-conclusions/sec-3-2-outlook.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18883 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_nglob/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18883 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_nglob/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_nglob/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2740 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_nglob/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      972 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_nglob/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_nglob/sec-2-2.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.321539 stepup-1.2.1/tests/cases/static_nglob_partial/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_nglob_partial/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_nglob_partial/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_nglob_partial/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_nglob_partial/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_nglob_partial/expected_graph_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_nglob_partial/expected_graph_04.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_nglob_partial/expected_stdout_a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_nglob_partial/expected_stdout_b.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2132 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_nglob_partial/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      297 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_nglob_partial/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.321539 stepup-1.2.1/tests/cases/static_nglob_subdir/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_nglob_subdir/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_nglob_subdir/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_nglob_subdir/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_nglob_subdir/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      742 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_nglob_subdir/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      107 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_nglob_subdir/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.321539 stepup-1.2.1/tests/cases/static_nglob_subdir/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_nglob_subdir/sub/inp1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_nglob_subdir/sub/inp2.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      151 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/static_nglob_subdir/sub/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.321539 stepup-1.2.1/tests/cases/subdir/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/subdir/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/subdir/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/subdir/example.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/subdir/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/subdir/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      636 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/subdir/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      170 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/subdir/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.321539 stepup-1.2.1/tests/cases/subdir/sub/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      450 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/subdir/sub/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.325539 stepup-1.2.1/tests/cases/watch_blocked/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_blocked/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_blocked/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_blocked/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_blocked/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_blocked/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      210 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_blocked/expensive.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_blocked/initial.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      961 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_blocked/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      261 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_blocked/plan_blocked.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      249 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_blocked/plan_unblocked.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.325539 stepup-1.2.1/tests/cases/watch_boot/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_boot/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_boot/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_boot/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_boot/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_boot/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      983 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_boot/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      178 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_boot/plan_01.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      182 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_boot/plan_02.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.325539 stepup-1.2.1/tests/cases/watch_chain/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_chain/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_chain/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_chain/config_01.json
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_chain/config_02.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_chain/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_chain/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_chain/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1069 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_chain/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      229 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_chain/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      546 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_chain/use_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.329539 stepup-1.2.1/tests/cases/watch_input/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_input/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_input/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_input/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_input/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_input/expected_graph_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_input/expected_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_input/first.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      940 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_input/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      155 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_input/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_input/second.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.329539 stepup-1.2.1/tests/cases/watch_middle/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_middle/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_middle/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_middle/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_middle/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_middle/expected_graph_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_middle/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1158 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_middle/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_middle/original.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      235 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_middle/plan_01.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      247 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_middle/plan_02.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.329539 stepup-1.2.1/tests/cases/watch_mixed/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_mixed/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_mixed/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_mixed/backup.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_mixed/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_mixed/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_mixed/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      825 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_mixed/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      219 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_mixed/plan_full.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      125 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_mixed/plan_trimmed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.333539 stepup-1.2.1/tests/cases/watch_nochanges/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_nochanges/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_nochanges/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_nochanges/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_nochanges/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_nochanges/expected_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_nochanges/input.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      876 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_nochanges/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      155 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_nochanges/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.333539 stepup-1.2.1/tests/cases/watch_outdated_amend1/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_outdated_amend1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_outdated_amend1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_outdated_amend1/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_outdated_amend1/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_outdated_amend1/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1071 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_outdated_amend1/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      164 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_outdated_amend1/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      271 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_outdated_amend1/step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.337540 stepup-1.2.1/tests/cases/watch_outdated_amend2/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_outdated_amend2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_outdated_amend2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_outdated_amend2/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_outdated_amend2/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_outdated_amend2/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1260 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_outdated_amend2/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      331 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_outdated_amend2/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      168 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_outdated_amend2/step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.337540 stepup-1.2.1/tests/cases/watch_output/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_output/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_output/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_output/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_output/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_output/expected_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_output/input.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      920 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_output/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      116 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_output/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_output/second.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:04.341539 stepup-1.2.1/tests/cases/watch_wanted/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_wanted/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_wanted/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_wanted/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_wanted/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_wanted/expected_graph_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_wanted/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1538 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_wanted/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      328 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_wanted/plan_01.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      105 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/cases/watch_wanted/plan_02.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/core_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/echo_server_socket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/echo_server_stdio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9479 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/test_assoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15868 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/test_cascade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/test_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/test_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21270 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/test_nglob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/test_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9064 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65157 2024-05-07 17:53:00.000000 stepup-1.2.1/tests/test_workflow.py
```

### Comparing `stepup-1.2.0/.github/workflows/release.yaml` & `stepup-1.2.1/.github/workflows/release.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -24,16 +24,15 @@
     - name: Store the distribution packages
       uses: actions/upload-artifact@v3
       with:
         name: python-package-distributions
         path: dist/
 
   publish-to-pypi:
-    name: >-
-      Publish Python distribution to PyPI
+    name: Publish Python distribution to PyPI
     if: startsWith(github.ref, 'refs/tags/')  # only publish to PyPI on tag pushes
     needs:
     - build
     runs-on: ubuntu-latest
     environment:
       name: pypi
       url: https://pypi.org/p/stepup
@@ -90,21 +89,22 @@
       run: >-
         gh release upload
         '${{ github.ref_name }}' dist/**
         --repo '${{ github.repository }}'
 
   publish-to-testpypi:
     name: Publish Python distribution to TestPyPI
+    if: ${{ github.ref == 'refs/heads/main' &&  github.repository_owner == 'reproducible-reporting'}}
     needs:
     - build
     runs-on: ubuntu-latest
 
     environment:
       name: testpypi
-      url: https://test.pypi.org/p/<package-name>
+      url: https://test.pypi.org/p/stepup
 
     permissions:
       id-token: write
 
     steps:
     - name: Download all the dists
       uses: actions/download-artifact@v3
```

### Comparing `stepup-1.2.0/.pre-commit-config.yaml` & `stepup-1.2.1/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.5.0
+  rev: v4.6.0
   hooks:
     - id: check-added-large-files
     - id: check-ast
     - id: check-case-conflict
     - id: check-executables-have-shebangs
     - id: check-json
     - id: check-merge-conflict
@@ -20,20 +20,17 @@
     - id: pretty-format-json
       args: ["--autofix", "--no-sort-keys"]
     - id: trailing-whitespace
 - repo: https://github.com/Lucas-C/pre-commit-hooks
   rev: v1.5.5
   hooks:
     - id: remove-crlf
-- repo: https://github.com/psf/black
-  rev: 24.3.0
-  hooks:
-    - id: black
 - repo: https://github.com/astral-sh/ruff-pre-commit
-  rev: 'v0.3.5'
+  rev: v0.4.3
   hooks:
+    - id: ruff-format
     - id: ruff
-      args: ["--fix"]
+      args: ["--fix", "--show-fixes"]
 - repo: https://github.com/python-jsonschema/check-jsonschema
-  rev: 0.28.1
+  rev: 0.28.2
   hooks:
     - id: check-github-workflows
```

### Comparing `stepup-1.2.0/LICENSE` & `stepup-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/PKG-INFO` & `stepup-1.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stepup
-Version: 1.2.0
+Version: 1.2.1
 Summary: StepUp Core provides the basic framework for the StepUp build tool
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
 Project-URL: Documentation, https://reproducible-reporting.github.io/stepup-core/
 Project-URL: Issues, https://github.com/reproducible-reporting/stepup-core/issues
 Project-URL: Source, https://github.com/reproducible-reporting/stepup-core/
 Project-URL: Changelog, https://reproducible-reporting.github.io/stepup-core/changelog/
 Classifier: Environment :: Console
@@ -31,14 +31,15 @@
 Requires-Dist: mkdocs-macros-plugin; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 Requires-Dist: numpy; extra == "dev"
 Requires-Dist: matplotlib; extra == "dev"
 
 [![release](https://github.com/reproducible-reporting/stepup-core/actions/workflows/release.yaml/badge.svg)](https://github.com/reproducible-reporting/stepup-core/actions/workflows/release.yaml)
 [![pytest](https://github.com/reproducible-reporting/stepup-core/actions/workflows/pytest.yaml/badge.svg)](https://github.com/reproducible-reporting/stepup-core/actions/workflows/pytest.yaml)
+[![mkdocs](https://github.com/reproducible-reporting/stepup-core/actions/workflows/mkdocs.yaml/badge.svg)](https://github.com/reproducible-reporting/stepup-core/actions/workflows/mkdocs.yaml)
 [![PyPI Version](https://img.shields.io/pypi/v/stepup)](https://pypi.org/project/stepup/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/stepup)
 ![GPL-3 License](https://img.shields.io/github/license/reproducible-reporting/stepup-core)
 
 # StepUp Core
 
 StepUp is a simple, powerful and universal build tool.
```

### Comparing `stepup-1.2.0/README.md` & `stepup-1.2.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 [![release](https://github.com/reproducible-reporting/stepup-core/actions/workflows/release.yaml/badge.svg)](https://github.com/reproducible-reporting/stepup-core/actions/workflows/release.yaml)
 [![pytest](https://github.com/reproducible-reporting/stepup-core/actions/workflows/pytest.yaml/badge.svg)](https://github.com/reproducible-reporting/stepup-core/actions/workflows/pytest.yaml)
+[![mkdocs](https://github.com/reproducible-reporting/stepup-core/actions/workflows/mkdocs.yaml/badge.svg)](https://github.com/reproducible-reporting/stepup-core/actions/workflows/mkdocs.yaml)
 [![PyPI Version](https://img.shields.io/pypi/v/stepup)](https://pypi.org/project/stepup/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/stepup)
 ![GPL-3 License](https://img.shields.io/github/license/reproducible-reporting/stepup-core)
 
 # StepUp Core
 
 StepUp is a simple, powerful and universal build tool.
```

### Comparing `stepup-1.2.0/docs/advanced_topics/amending_static_inputs/stdout.txt` & `stepup-1.2.1/docs/advanced_topics/amending_static_inputs/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/advanced_topics/amending_static_inputs.md` & `stepup-1.2.1/docs/advanced_topics/amending_static_inputs.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Amending Static Inputs
 
 Occasionally, it may be convenient to declare a static file and then use it as input in the same script.
-As of StepUp 1.1, this is allowed and no longer treated as a cyclic dependency.
+As of StepUp 1.2.0, this is allowed and no longer treated as a cyclic dependency.
 
 
 ## Example
 
 Create the following `plan.py`, which declares a static file, amends it as input, and then opens it to print it to the standard output.
 
 ```python
```

### Comparing `stepup-1.2.0/docs/advanced_topics/amending_steps/stdout.txt` & `stepup-1.2.1/docs/advanced_topics/amending_steps/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/advanced_topics/amending_steps.md` & `stepup-1.2.1/docs/advanced_topics/amending_steps.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/advanced_topics/blocked_steps/stdout.txt` & `stepup-1.2.1/docs/advanced_topics/blocked_steps/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/advanced_topics/blocked_steps.md` & `stepup-1.2.1/docs/advanced_topics/blocked_steps.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/advanced_topics/cyclic_dependencies/stdout.txt` & `stepup-1.2.1/docs/advanced_topics/cyclic_dependencies/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/advanced_topics/cyclic_dependencies.md` & `stepup-1.2.1/docs/advanced_topics/cyclic_dependencies.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/advanced_topics/environment_variables/stdout.txt` & `stepup-1.2.1/docs/advanced_topics/environment_variables/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/advanced_topics/environment_variables.md` & `stepup-1.2.1/docs/advanced_topics/environment_variables.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/advanced_topics/here_and_root/stdout.txt` & `stepup-1.2.1/docs/advanced_topics/here_and_root/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/advanced_topics/here_and_root.md` & `stepup-1.2.1/docs/advanced_topics/here_and_root.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/advanced_topics/manual_cleaning.md` & `stepup-1.2.1/docs/advanced_topics/manual_cleaning.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/advanced_topics/optional_steps/plot_logmap.png` & `stepup-1.2.1/docs/advanced_topics/optional_steps/plot_logmap.png`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/advanced_topics/optional_steps/stdout.txt` & `stepup-1.2.1/docs/advanced_topics/optional_steps/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/advanced_topics/optional_steps.md` & `stepup-1.2.1/docs/advanced_topics/optional_steps.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/advanced_topics/pools/stdout.txt` & `stepup-1.2.1/docs/advanced_topics/pools/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/advanced_topics/pools.md` & `stepup-1.2.1/docs/advanced_topics/pools.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/advanced_topics/static_deferred_glob/graph.txt` & `stepup-1.2.1/docs/advanced_topics/static_deferred_glob/graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/advanced_topics/static_deferred_glob/graph_creator.svg` & `stepup-1.2.1/docs/advanced_topics/static_deferred_glob/graph_creator.svg`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/advanced_topics/static_deferred_glob/graph_supplier.svg` & `stepup-1.2.1/docs/advanced_topics/static_deferred_glob/graph_supplier.svg`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/advanced_topics/static_deferred_glob/stdout.txt` & `stepup-1.2.1/docs/advanced_topics/static_deferred_glob/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/advanced_topics/static_deferred_glob.md` & `stepup-1.2.1/docs/advanced_topics/static_deferred_glob.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/advanced_topics/static_named_glob/plan.py` & `stepup-1.2.1/docs/advanced_topics/static_named_glob/plan.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python
-from stepup.core.api import glob, copy, mkdir, step
+from stepup.core.api import copy, glob, mkdir, step
 
 # Make all chapter directories static
 glob("ch*/")
 
 # Enforce consistent chapter numbers throughout the match,
 # ignoring inconsistent txt files.
 md_chapter = {}
```

### Comparing `stepup-1.2.0/docs/advanced_topics/static_named_glob/stdout.txt` & `stepup-1.2.1/docs/advanced_topics/static_named_glob/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/advanced_topics/static_named_glob.md` & `stepup-1.2.1/docs/advanced_topics/static_named_glob.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/advanced_topics/variable_substitution.md` & `stepup-1.2.1/docs/advanced_topics/variable_substitution.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/advanced_topics/volatile_outputs.md` & `stepup-1.2.1/docs/advanced_topics/volatile_outputs.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/changelog.md` & `stepup-1.2.1/docs/changelog.md`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,21 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [1.2.1] - 2024-05-07
+
+### Fixed
+
+- Fixed packaging mistake that confused PyCharm and Pytest.
+
+
 ## [1.2.0] - 2024-05-02
 
 ### Added
 
 - Export of graphs to [Graphviz](https://graphviz.org/) DOT files.
 - The `cleanup` script for manually cleaning up outputs.
```

### Comparing `stepup-1.2.0/docs/development.md` & `stepup-1.2.1/docs/development.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,12 @@
 # Developer Notes
 
 If you would like to contribute, please read [CONTRIBUTING.md](https://github.com/reproducible-reporting/.github/blob/main/CONTRIBUTING.md).
 
 
-## How to Make Releases
-
-- Mark the release in `docs/changelog.md`.
-- Make a new commit and tag it with `vX.Y.Z`.
-- Trigger the PyPI GitHub Action: `git push origin main --tags`.
-
-
 ## Development Install and Unit Tests
 
 ```bash
 git clone git@github.com:reproducible-reporting/stepup-core.git
 cd stepup-core
 pre-commit install
 python -m venv venv
@@ -35,19 +28,29 @@
 mkdocs serve --watch stepup/core/
 ```
 
 (Keep this running.)
 Then open the live preview in your browser at [http://127.0.0.1:8000/](http://127.0.0.1:8000/)
 and edit Markdown files in your IDE.
 
+Please, use [Semantic Line Breaks](https://sembr.org/)
+because it results in cleaner file diffs when editing documentation.
+
 
 ## Tutorial Example Outputs
 
 If you wish to regenerate the output of the examples, run `stepup` in the `docs` directory:
 
 ```bash
 cd docs
 stepup -n
 ```
 
 Note that some scripts use [Graphviz](https://graphviz.org/) to generate diagrams,
 so you must have it installed on your system.
+
+
+## How to Make a Release
+
+- Mark the release in `docs/changelog.md`.
+- Make a new commit and tag it with `vX.Y.Z`.
+- Trigger the PyPI GitHub Action: `git push origin main --tags`.
```

### Comparing `stepup-1.2.0/docs/getting_started/automatic_cleaning.md` & `stepup-1.2.1/docs/getting_started/automatic_cleaning.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/getting_started/copy_mkdir/stdout.txt` & `stepup-1.2.1/docs/getting_started/copy_mkdir/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/getting_started/copy_mkdir.md` & `stepup-1.2.1/docs/getting_started/copy_mkdir.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/getting_started/dependencies/graph_creator.svg` & `stepup-1.2.1/docs/getting_started/dependencies/graph_creator.svg`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/getting_started/dependencies/graph_supplier.svg` & `stepup-1.2.1/docs/getting_started/dependencies/graph_supplier.svg`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/getting_started/dependencies/stdout.txt` & `stepup-1.2.1/docs/getting_started/dependencies/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/getting_started/dependencies.md` & `stepup-1.2.1/docs/getting_started/dependencies.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/getting_started/distributed_plans/stdout.txt` & `stepup-1.2.1/docs/getting_started/distributed_plans/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/getting_started/distributed_plans.md` & `stepup-1.2.1/docs/getting_started/distributed_plans.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/getting_started/first_step/stdout1.txt` & `stepup-1.2.1/docs/getting_started/first_step/stdout1.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/getting_started/first_step.md` & `stepup-1.2.1/docs/getting_started/first_step.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/getting_started/interactive_usage.md` & `stepup-1.2.1/docs/getting_started/interactive_usage.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/getting_started/introduction.md` & `stepup-1.2.1/docs/getting_started/introduction.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/getting_started/no_rules/stdout.txt` & `stepup-1.2.1/docs/getting_started/no_rules/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/getting_started/no_rules.md` & `stepup-1.2.1/docs/getting_started/no_rules.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/getting_started/processes.svg` & `stepup-1.2.1/docs/getting_started/processes.svg`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/getting_started/script_multiple/ebbr.csv` & `stepup-1.2.1/docs/getting_started/script_multiple/ebbr.csv`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/getting_started/script_multiple/ebos.csv` & `stepup-1.2.1/docs/getting_started/script_multiple/ebos.csv`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/getting_started/script_multiple/plot.py` & `stepup-1.2.1/docs/getting_started/script_multiple/plot.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
-import numpy as np
 import matplotlib
 import matplotlib.pyplot as plt
+import numpy as np
 from matplotlib.dates import DateFormatter
+
 from stepup.core.script import driver
 
 
 def cases():
     yield "ebbr"
     yield "ebos"
```

### Comparing `stepup-1.2.0/docs/getting_started/script_multiple/plot_ebbr.png` & `stepup-1.2.1/docs/getting_started/script_multiple/plot_ebbr.png`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/getting_started/script_multiple/plot_ebos.png` & `stepup-1.2.1/docs/getting_started/script_multiple/plot_ebos.png`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/getting_started/script_multiple/stdout.txt` & `stepup-1.2.1/docs/getting_started/script_multiple/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/getting_started/script_multiple.md` & `stepup-1.2.1/docs/getting_started/script_multiple.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/getting_started/script_single.md` & `stepup-1.2.1/docs/getting_started/script_single.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/getting_started/static_files.md` & `stepup-1.2.1/docs/getting_started/static_files.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/getting_started/static_glob/stdout.txt` & `stepup-1.2.1/docs/getting_started/static_glob/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/getting_started/static_glob.md` & `stepup-1.2.1/docs/getting_started/static_glob.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/getting_started/static_glob_conditional/stdout1.txt` & `stepup-1.2.1/docs/getting_started/static_glob_conditional/stdout1.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/getting_started/static_glob_conditional.md` & `stepup-1.2.1/docs/getting_started/static_glob_conditional.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/index.md` & `stepup-1.2.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/installation.md` & `stepup-1.2.1/docs/installation.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/license.md` & `stepup-1.2.1/docs/license.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/plan.py` & `stepup-1.2.1/docs/plan.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python
 """StepUp plan to generate all the outputs of the examples."""
 
-from stepup.core.api import glob, static, step, amend
 from path import Path
 
+from stepup.core.api import amend, glob, static, step
+
 
 def scan_main(path_main: str) -> tuple[list[Path], Path, list[Path]]:
     """Get list of static inputs, StepUp root and some outputs of the example.
 
     This information is embedded in the comments of `main.sh` and the commands
 
     ```
```

### Comparing `stepup-1.2.0/docs/reference/interactive.md` & `stepup-1.2.1/docs/reference/interactive.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/reference/stepup.core.api.md` & `stepup-1.2.1/docs/reference/stepup.core.api.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/docs/run_example.py` & `stepup-1.2.1/docs/run_example.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 #!/usr/bin/env python
 """Run one example and amend (volatile) outputs."""
 
-import sys
 import subprocess
+import sys
 
 from path import Path
+
 from stepup.core.api import amend
 from stepup.core.file import FileState
 from stepup.core.workflow import Workflow
 
 
 def main():
     path_main, root = sys.argv[1:]
 
     workdir, name_main = Path(path_main).splitpath()
-    subprocess.run(f"./{name_main}", cwd=workdir)
+    subprocess.run(f"./{name_main}", cwd=workdir, check=False)
 
     root = Path(root)
     path_stepup = root / ".stepup/"
     path_workflow = path_stepup / "workflow.mpk.xz"
     workflow = Workflow.from_file(path_workflow)
     out = [path_stepup]
     vol = [path_workflow]
```

### Comparing `stepup-1.2.0/mkdocs.yml` & `stepup-1.2.1/mkdocs.yml`

 * *Files 3% similar despite different names*

```diff
@@ -98,7 +98,9 @@
   - pymdownx.highlight:
       anchor_linenums: true
       line_spans: __span
       pygments_lang_class: true
   - pymdownx.inlinehilite
   - pymdownx.snippets
   - pymdownx.superfences
+  - toc:
+      permalink: true
```

### Comparing `stepup-1.2.0/pyproject.toml` & `stepup-1.2.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -59,18 +59,18 @@
 line-length = 100
 target-version = ['py311']
 
 [tool.ruff]
 line-length = 100
 target-version = "py311"
 
-[too.ruff.lint]
-select = ["E", "F", "UP", "B", "I", "PGH", "PL", "RUF", "C"]
+[tool.ruff.lint]
+select = ["E", "F", "UP", "B", "SIM", "I", "PGH", "PL", "RUF", "C"]
 ignore = ["PLR0911", "PLR0912", "PLR0913", "PLR0915", "PLR2004", "PLW2901", "C901"]
 
 [tool.setuptools]
-packages = ["stepup.core"]
+packages = ["stepup"]
 
 [tool.setuptools_scm]
 write_to = "stepup/core/_version.py"
 version_scheme = "post-release"
 local_scheme = "no-local-version"
```

### Comparing `stepup-1.2.0/stepup/core/__init__.py` & `stepup-1.2.1/stepup/core/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """StepUp Core package."""
 
-
 __all__ = ("__version__", "__version_tuple__")
 
 
 try:
     from ._version import __version__, __version_tuple__
 except ImportError:
     __version__ = "0.0.0a-dev"
```

### Comparing `stepup-1.2.0/stepup/core/api.py` & `stepup-1.2.1/stepup/core/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,30 +22,29 @@
 To keep things simple, it is assumed that one Python process only communicates with one director.
 
 This module should not be imported by other stepup.core modules, except for stepup.interact.
 """
 
 import contextlib
 import os
+from collections.abc import Callable, Collection, Iterable, Iterator
 from time import sleep
-from typing import Collection, Iterable, Iterator, Callable
 
 from path import Path
 
 from .nglob import NGlobMulti
+from .rpc import DummySyncRPCClient, SocketSyncRPCClient
 from .utils import (
-    myrelpath,
     CaseSensitiveTemplate,
-    mynormpath,
-    make_path_out,
     check_inp_path,
     lookupdict,
+    make_path_out,
+    mynormpath,
+    myrelpath,
 )
-from .rpc import SocketSyncRPCClient, DummySyncRPCClient
-
 
 __all__ = (
     # Basic API
     "static",
     "glob",
     "step",
     "pool",
@@ -594,15 +593,15 @@
 def _get_rpc_client():
     """Try setting up a Synchronous RPC client or fall back to the dummy client if that fails."""
     STEPUP_DIRECTOR_SOCKET = os.getenv("STEPUP_DIRECTOR_SOCKET")
     if STEPUP_DIRECTOR_SOCKET is None:
         STEPUP_ROOT = Path(os.getenv("STEPUP_ROOT", "./"))
         path_tmpsock = STEPUP_ROOT / ".stepup/tmpsock.txt"
         time = 0.0
-        for itry in range(5):
+        for _ in range(5):
             if time > 0:
                 print(f"WARNING: waiting {time} seconds for {path_tmpsock}")
                 sleep(time)
                 time *= 2
             else:
                 time = 0.1
             if path_tmpsock.is_file():
```

### Comparing `stepup-1.2.0/stepup/core/assoc.py` & `stepup-1.2.1/stepup/core/assoc.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """Bidirectional non-exclusive map."""
 
 import enum
-from typing import TypeVar, Generic, Iterator
+from collections.abc import Iterator
+from typing import Generic, TypeVar
 
 import attrs
 
-
 __all__ = ("Assoc", "AssocView", "one_to_one", "one_to_many", "many_to_one", "many_to_many")
 
 
 # Taken from attrs._make
 class _Nothing(enum.Enum):
     NOTHING = enum.auto()
```

### Comparing `stepup-1.2.0/stepup/core/asyncio.py` & `stepup-1.2.1/stepup/core/asyncio.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 # --
 """Asyncio utilities used in StepUp."""
 
 import asyncio
 import os
 import sys
 
-
 __all__ = (
     "wait_for_events",
     "stoppable_iterator",
     "stdio",
     "pipe",
 )
 
@@ -146,16 +145,16 @@
         The StreamReader taking data out of the pipe.
     writer
         The StreamWriter putting data into the pipe.
     """
     if loop is None:
         loop = asyncio.get_event_loop()
     fd_in, fd_out = os.pipe()
-    pipe_in = open(fd_in)
-    pipe_out = open(fd_out)
+    pipe_in = open(fd_in)  # noqa: SIM115
+    pipe_out = open(fd_out)  # noqa: SIM115
     reader = asyncio.StreamReader(limit=limit, loop=loop)
     await loop.connect_read_pipe(lambda: asyncio.StreamReaderProtocol(reader, loop=loop), pipe_in)
     writer_transport, writer_protocol = await loop.connect_write_pipe(
         lambda: asyncio.streams.FlowControlMixin(loop=loop), pipe_out
     )
     writer = asyncio.streams.StreamWriter(writer_transport, writer_protocol, None, loop)
     return reader, writer
```

### Comparing `stepup-1.2.0/stepup/core/cascade.py` & `stepup-1.2.1/stepup/core/cascade.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,21 +24,22 @@
 All other nodes and their logic are implemented in `stepup.core.workflow`.
 
 The separation between `Cascade` and `Workflow` allows for testing a well-defined subset,
 before building more complexity on top of it.
 """
 
 import lzma
-from typing import Any, Self, Iterator
+from collections.abc import Iterator
+from typing import Any, Self
 
 import attrs
 import msgpack
 
-from .assoc import Assoc, one_to_many, many_to_many, AssocView
-from .exceptions import GraphError, CyclicError
+from .assoc import Assoc, AssocView, many_to_many, one_to_many
+from .exceptions import CyclicError, GraphError
 from .utils import classproperty, lookupdict
 
 __all__ = ("Node", "Root", "Vacuum", "Cascade", "get_kind")
 
 
 @attrs.define
 class Node:
@@ -237,15 +238,15 @@
         return cascade
 
     def unstructure(self):
         lookup = lookupdict()
         state = {"nodes": [], "products": [], "consumers": []}
         for key in self.nodes:
             lookup[key] = len(lookup)
-        for inode, (key, node) in enumerate(self.nodes.items()):
+        for node in self.nodes.values():
             node_data = {"c": node.kind}
             node_data.update(node.unstructure(self, lookup))
             state["nodes"].append(node_data)
         for key_src, key_dst in self.products.pairs():
             state["products"].append([lookup[key_src], lookup[key_dst]])
         state["products"].sort()
         for key_src, key_dst in self.consumers.pairs():
@@ -278,15 +279,15 @@
             creator_key = self.get_creator(key)
             assert creator_key is not None
             if creator_key == "vacuum:":
                 lines.append(f"({key})")
             else:
                 lines.append(key)
             for name, value in node.format_properties(self):
-                lines.append(f"{name:>20s} = {str(value)}")
+                lines.append(f"{name:>20s} = {value!s}")
             pairs = []
             if not (creator_key == "vacuum:" or key == "root:"):
                 pairs.append(("created by", creator_key))
             for other_key in self.get_suppliers(key, include_orphans=True):
                 pairs.append(("consumes", other_key))
             for other_key in self.get_products(key, include_orphans=True):
                 if other_key != "root:":
@@ -362,18 +363,15 @@
             for other in self.consumers.get(key, ())
             if (include_orphans or not self.is_orphan(other))
             and (kind is None or kind == get_kind(other))
         )
 
     def get_nodes(self, kind: str | None = None, include_orphans: bool = False):
         assert kind is None or kind in self.node_classes
-        if kind is None:
-            keys = self.nodes
-        else:
-            keys = self.kinds.get(kind, ())
+        keys = self.nodes if kind is None else self.kinds.get(kind, ())
         keys = sorted(key for key in keys if (include_orphans or not self.is_orphan(key)))
         return [self.nodes[key] for key in keys]
 
     #
     # Graph modifications
     #
 
@@ -385,15 +383,15 @@
         This method only consider supplier-consumer edges.
         """
         if src_key != "root:":
             if src_key == dst_key:
                 yield (src_key,)
             for supplier_key in self.suppliers.get(src_key, ()):
                 for cycle in self._iter_cycles(supplier_key, dst_key):
-                    yield (src_key,) + cycle
+                    yield (src_key, *cycle)
 
     def report_cyclic(self, src_key: str, dst_key: str):
         """Raise an informative exception when the new edge would make the directed graph cyclic.
 
         Notes
         -----
         - This method is rather slow and only called when there is a known problem.
@@ -403,21 +401,21 @@
         lines = []
         for cycle in self._iter_cycles(src_key, dst_key):
             lines.append("cycle:")
             for key in cycle:
                 lines.append(f"  {key}")
             lines.append("")
         if len(lines) > 0:
-            lines = [
+            lines[:0] = [
                 "New relation introduces cyclic dependency",
                 "",
                 f"src = {src_key}",
                 f"dst = {dst_key}",
                 "",
-            ] + lines
+            ]
             raise CyclicError("\n".join(lines))
 
     def walk_suppliers(self, key: str, visited: set[str]):
         """Efficiently collect all suppliers of `key` and add them to `visited`."""
         if key in ["root:", "vacuum:"]:
             return
         visited.add(key)
```

### Comparing `stepup-1.2.0/stepup/core/cleanup.py` & `stepup-1.2.1/stepup/core/cleanup.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/stepup/core/deferred_glob.py` & `stepup-1.2.1/stepup/core/deferred_glob.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,27 +15,28 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """Deferred patterns for static files."""
 
-from typing import Any, Self, Iterator, TYPE_CHECKING
+from collections.abc import Iterator
+from typing import TYPE_CHECKING, Any, Self
 
 import attrs
 
 from .cascade import Node
 from .nglob import NGlobMulti
 from .utils import classproperty
 
 if TYPE_CHECKING:
     from .workflow import Workflow
 
 
-__all__ = "DeferredGlob"
+__all__ = ("DeferredGlob",)
 
 
 @attrs.define
 class DeferredGlob(Node):
     """A pattern to make files static when they are used as input."""
 
     _ngm: NGlobMulti = attrs.field()
```

### Comparing `stepup-1.2.0/stepup/core/director.py` & `stepup-1.2.1/stepup/core/director.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,37 +15,37 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """The director process manages the workflow and sends jobs to the worker processes."""
 
+import argparse
 import asyncio
 import contextlib
 import os
-import argparse
 import shutil
 import sys
 import traceback
 from decimal import Decimal
 
 import attrs
 from path import Path
 
 from stepup.core.file import FileState
 from stepup.core.nglob import NGlobMulti
-from .rpc import serve_socket_rpc, allow_rpc
-from .workflow import Workflow
+
 from .exceptions import GraphError
 from .reporter import ReporterClient
+from .rpc import allow_rpc, serve_socket_rpc
 from .runner import Runner
 from .scheduler import Scheduler
 from .utils import check_plan, mynormpath, remove_path
 from .watcher import Watcher
-
+from .workflow import Workflow
 
 __all__ = ("interpret_num_workers", "serve")
 
 
 def main():
     asyncio.run(async_main())
```

### Comparing `stepup-1.2.0/stepup/core/exceptions.py` & `stepup-1.2.1/stepup/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/stepup/core/file.py` & `stepup-1.2.1/stepup/core/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,21 +16,22 @@
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """A `File` is StepUp's node for an input or output file of a step."""
 
 import enum
-from typing import Any, Self, Iterator, TYPE_CHECKING
+from collections.abc import Iterator
+from typing import TYPE_CHECKING, Any, Self
 
 import attrs
 from path import Path
 
-from .hash import FileHash
 from .cascade import Node
+from .hash import FileHash
 from .utils import format_digest
 
 if TYPE_CHECKING:
     from .workflow import Workflow
 
 
 __all__ = ("FileState", "File")
@@ -125,17 +126,16 @@
 
     def cleanup(self, workflow: "Workflow"):
         if self._path.endswith("/"):
             workflow.dir_queue.put_nowait((True, self._path))
         state = self.get_state(workflow)
         if state == FileState.VOLATILE:
             workflow.to_be_deleted.append((self._path, None))
-        elif state in (FileState.PENDING, FileState.BUILT):
-            if self.hash.digest != b"u":
-                workflow.to_be_deleted.append((self._path, self.hash))
+        elif state in (FileState.PENDING, FileState.BUILT) and self.hash.digest != b"u":
+            workflow.to_be_deleted.append((self._path, self.hash))
         workflow.file_states.discard(self.key, insist=True)
 
     #
     # File state
     #
 
     def get_state(self, workflow: "Workflow") -> FileState:
```

### Comparing `stepup-1.2.0/stepup/core/hash.py` & `stepup-1.2.1/stepup/core/hash.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 import os
 import stat
 from typing import Self
 
 import attrs
 from path import Path
 
-
 __all__ = (
     "HashWords",
     "compute_file_digest",
     "FileHash",
     "StepHash",
     "ExtendedStepHash",
     "compare_step_hashes",
@@ -249,17 +248,16 @@
         return StepHash(*args[:2])
 
 
 def compare_step_hashes(old_hash: StepHash, new_hash: StepHash) -> tuple[str, str]:
     chl = []
     sml = []
     _compare_step_digests(chl, sml, old_hash, new_hash)
-    if isinstance(old_hash, ExtendedStepHash):
-        if isinstance(new_hash, ExtendedStepHash):
-            _compare_extended_hashes(chl, sml, old_hash, new_hash)
+    if isinstance(old_hash, ExtendedStepHash) and isinstance(new_hash, ExtendedStepHash):
+        _compare_extended_hashes(chl, sml, old_hash, new_hash)
     changed = "\n".join(f"{descr:20s} {content}" for descr, content in chl)
     same = "\n".join(f"{descr:20s} {content}" for descr, content in sml)
     return changed, same
 
 
 def _compare_step_digests(
     chl: list[tuple[str, str]], sml: list[tuple[str, str]], old_hash: StepHash, new_hash: StepHash
@@ -325,19 +323,18 @@
                 changed, line = _report_hash_diff(label, path, old_hashes[path], new_hashes[path])
                 if changed:
                     chl.append(line)
                 else:
                     sml.append(line)
             else:
                 chl.append((f"Deleted {label} hash", path))
+        elif path in new_hashes:
+            chl.append((f"Added {label} hash", path))
         else:
-            if path in new_hashes:
-                chl.append((f"Added {label} hash", path))
-            else:
-                assert False
+            raise AssertionError("This should never happen.")
 
 
 def _report_hash_diff(
     label: str, path: str, old_hash: FileHash, new_hash: FileHash
 ) -> tuple[bool, tuple[str, str]]:
     changes = []
 
@@ -376,17 +373,16 @@
                 new_var = _fmt_env_value(new_env[name])
                 if old_env[name] == new_env[name]:
                     sml.append(("Same env var", f"{name} {old_var}"))
                 else:
                     chl.append(("Modified env var", f"{name} {old_var} ➜ {new_var}"))
             else:
                 chl.append(("Deleted env var", f"{name} {old_var}"))
+        elif name in new_env:
+            new_var = _fmt_env_value(new_env[name])
+            chl.append(("Added env var", f"{name} {new_var}"))
         else:
-            if name in new_env:
-                new_var = _fmt_env_value(new_env[name])
-                chl.append(("Added env var", f"{name} {new_var}"))
-            else:
-                assert False
+            raise AssertionError("This should never happen.")
 
 
 def _fmt_env_value(value: str | None) -> str:
     return "(unset)" if value is None else f"='{value}'"
```

### Comparing `stepup-1.2.0/stepup/core/interact.py` & `stepup-1.2.1/stepup/core/interact.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 python -c 'from stepup.core.interact import run; run()'
 ```
 
 This command must be executed in the top-level directory
 where a `stepup` command is running in interactive mode.
 """
 
-
 from .api import RPC_CLIENT, translate
 
 __all__ = ("run", "cleanup", "graph", "watch_update", "watch_delete", "wait", "join")
 
 
 def run():
     """Exit the watch phase and start running steps whose inputs have changed."""
```

### Comparing `stepup-1.2.0/stepup/core/job.py` & `stepup-1.2.1/stepup/core/job.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -15,21 +15,21 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """Definition of jobs to be executed by a worker."""
 
-
 from typing import TYPE_CHECKING
+
 import attrs
 
 if TYPE_CHECKING:
-    from .worker import WorkerClient
     from .scheduler import Scheduler
+    from .worker import WorkerClient
     from .workflow import Workflow
 
 
 __all__ = ("Job", "ValidateAmendedJob", "TryReplayJob", "RunJob")
 
 
 @attrs.define
```

### Comparing `stepup-1.2.0/stepup/core/nglob.py` & `stepup-1.2.1/stepup/core/nglob.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,20 +78,20 @@
 - Conventional glob wildcards are also allowed and are called "anonymous wildcards"
   to clarify the distinction from named wildcards.
 """
 
 import copy
 import glob
 import re
-from typing import Iterator, Iterable, Self, Collection, Any
+from collections.abc import Collection, Iterable, Iterator
+from typing import Any, Self
 
 import attrs
 from path import Path
 
-
 RE_NAMED_WILD = re.compile(r"(\[.*?]|\$\{\*[a-zA-Z0-9_]*?}|[*]{1,2}|[?])")
 
 
 __all__ = (
     "NGlobMatch",
     "NGlobSingle",
     "NGlobMulti",
@@ -108,16 +108,16 @@
 
     def __getitem__(self, idx) -> Path | list[Path]:
         return self._files[idx]
 
     def __getattr__(self, name) -> str:
         try:
             return self._mapping[name]
-        except KeyError:
-            raise AttributeError(f"'NGlobMatch' object has not attribute '{name}'")
+        except KeyError as exc:
+            raise AttributeError(f"'NGlobMatch' object has not attribute '{name}'") from exc
 
     @property
     def mapping(self) -> dict[str, str]:
         return self._mapping
 
     @property
     def files(self) -> list[Path]:
@@ -297,15 +297,15 @@
         ]
         # A little hacky way to make the result more compact.
         for ngs_data in data[0]:
             del ngs_data["s"]
         return data
 
     @classmethod
-    def from_patterns(cls, patterns: Iterable[str], subs: dict[str, str] = None) -> Self:
+    def from_patterns(cls, patterns: Iterable[str], subs: dict[str, str] | None = None) -> Self:
         if isinstance(patterns, str):
             raise TypeError("The patterns argument cannot be a string")
         if not all(isinstance(pattern, str) for pattern in patterns):
             raise TypeError(f"The patterns must be a list of strings, got {patterns}")
         if subs is None:
             subs = {}
         else:
@@ -343,35 +343,35 @@
         start = full_paths if isinstance(full_paths, int) else len(full_paths)
         if start == len(self._nglob_singles):
             yield tuple(criteria[name] for name in self._used_names), full_paths
         else:
             ngs = self._nglob_singles[start]
             for new_values, paths in ngs.results.items():
                 next_criteria = criteria.copy()
-                for name, new_value in zip(ngs.used_names, new_values):
+                for name, new_value in zip(ngs.used_names, new_values, strict=False):
                     value = next_criteria.get(name)
                     if value is None:
                         next_criteria[name] = new_value
                     elif value != new_value:
                         next_criteria = None
                         break
                 if next_criteria is not None:
                     next_full_paths = (
                         start + 1 if isinstance(full_paths, int) else [*full_paths, paths]
                     )
                     yield from self._iter_consistent(next_criteria, next_full_paths)
 
     def _extend_consistent(self, i: int, values: tuple[str, ...]):
-        criteria = dict(zip(self._nglob_singles[i].used_names, values))
+        criteria = dict(zip(self._nglob_singles[i].used_names, values, strict=False))
         new_items = list(self._iter_consistent(criteria, []))
         for full_values, full_paths in new_items:
             self._results[full_values] = full_paths
 
     def _reduce_consistent(self, i: int, values: tuple[str, ...]):
-        criteria = dict(zip(self._nglob_singles[i].used_names, values))
+        criteria = dict(zip(self._nglob_singles[i].used_names, values, strict=False))
         old_items = list(self._iter_consistent(criteria, 0))
         for full_values, _ in old_items:
             del self._results[full_values]
 
     def extend(self, paths: Iterable[str]):
         """Find matches from a list of paths. Return new full matches (and track partial matches)"""
         if isinstance(paths, str):
@@ -402,18 +402,18 @@
         return self._results == other._results
 
     # Convenience methods
 
     def matches(self) -> Iterator[NGlobMatch]:
         """Iterate over combinations of files that consistently match of all patterns."""
         for values, path_sets in sorted(self._results.items()):
-            mapping = dict(zip(self._used_names, values))
+            mapping = dict(zip(self._used_names, values, strict=False))
             files = [
                 (sorted(paths) if has_anonymous_wildcards(ngs.pattern) else next(iter(paths)))
-                for ngs, paths in zip(self._nglob_singles, path_sets)
+                for ngs, paths in zip(self._nglob_singles, path_sets, strict=False)
             ]
             yield NGlobMatch(mapping, files)
 
     def files(self) -> tuple[Path, ...]:
         """Return a tuple of sorted files that match the individual patterns.
 
         No constraints between multiple patterns are imposed and files may belong to partial
@@ -438,18 +438,15 @@
     def may_match(self, path):
         """Return True if the path matches one of the NGlobSingle instances.
 
         This means that it may be path contributing to a consistent match of NGlobMulti.
         When added, it will show up in the result of the `files` method and it may affect the
         outcome of the `matches` method.
         """
-        for ngs in self._nglob_singles:
-            if ngs.regex.fullmatch(path):
-                return True
-        return False
+        return any(ngs.regex.fullmatch(path) for ngs in self._nglob_singles)
 
     def may_change(self, deleted: set[str], added: set[str]) -> bool:
         """Determine whether the results may change (later) after deleting or adding files.
 
         Parameters
         ----------
         deleted
@@ -532,18 +529,15 @@
             if part == "?":
                 regex = r"[^/]"
             elif part == "*":
                 regex = r"[^/]*"
             elif part == "**":
                 regex = r".*"
             elif part.startswith("[") and part.endswith("]"):
-                if part[1] == "!":
-                    regex = rf"[^{part[2:-1]}]"
-                else:
-                    regex = rf"[{part[1:-1]}]"
+                regex = rf"[^{part[2:-1]}]" if part[1] == "!" else rf"[{part[1:-1]}]"
             elif part.startswith("${*") and part.endswith("}"):
                 if not allow_names:
                     raise ValueError(f"Named wildcards not allowed in {pattern}")
                 name = part[3:-1]
                 if name in encountered:
                     regex = rf"(?P={name})"
                 else:
```

### Comparing `stepup-1.2.0/stepup/core/pytest.py` & `stepup-1.2.1/stepup/core/pytest.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,24 +15,22 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """Utilities for testing with pytest."""
 
-
 import asyncio
 import os
 import re
 import shutil
 import subprocess
 
 from path import Path
 
-
 __all__ = ("remove_hashes", "run_example")
 
 
 def remove_hashes(graph: dict) -> dict:
     """Remove hashes from a JSON representation of the workflow."""
     for node in graph["nodes"]:
         node.pop("h", None)
```

### Comparing `stepup-1.2.0/stepup/core/reporter.py` & `stepup-1.2.1/stepup/core/reporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,28 +15,28 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """Terminal output of StepUp's runner progress and observed file changes."""
 
-
 import asyncio
 import contextlib
 from collections import Counter
 from time import perf_counter
 from typing import Self
 
 import attrs
 from rich.console import Console
-from rich.theme import Theme
-from rich.progress import Progress as ProgressBar, TaskID, BarColumn, MofNCompleteColumn, TextColumn
 from rich.markup import escape as escape_markup
+from rich.progress import BarColumn, MofNCompleteColumn, TaskID, TextColumn
+from rich.progress import Progress as ProgressBar
+from rich.theme import Theme
 
-from .rpc import BaseAsyncRPCClient, DummyAsyncRPCClient, AsyncRPCClient, allow_rpc
+from .rpc import AsyncRPCClient, BaseAsyncRPCClient, DummyAsyncRPCClient, allow_rpc
 from .step import StepState
 
 __all__ = ("ReporterClient", "ReporterHandler")
 
 
 @attrs.define
 class ReporterClient:
```

### Comparing `stepup-1.2.0/stepup/core/rpc.py` & `stepup-1.2.1/stepup/core/rpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,30 +18,29 @@
 #
 # --
 """Lightweight and versatile RPC implementation using asyncio stream reader and writer.
 
 This module also includes a synchronous RPC client to support simple client APIs.
 """
 
-
-import inspect
-import traceback
 import asyncio
-import subprocess
+import inspect
 import pickle
 import socket
+import subprocess
+import traceback
+from collections.abc import Awaitable, Callable, Collection
 from functools import partial
-from typing import Any, Callable, Collection, Awaitable
+from typing import Any
 
 import attrs
 
-from .asyncio import stoppable_iterator, stdio
+from .asyncio import stdio, stoppable_iterator
 from .exceptions import RPCError
 
-
 __all__ = (
     "fmt_rpc_call",
     "allow_rpc",
     "serve_rpc",
     "serve_socket_rpc",
     "serve_stdio_rpc",
     "BaseAsyncRPCClient",
@@ -56,17 +55,15 @@
 #
 # Utilities
 #
 
 
 def fmt_rpc_call(name: str, args: Collection, kwargs: dict) -> str:
     """String format an RPC call with arguments."""
-    all_args = [repr(arg) for arg in args] + [
-        f"{name}={repr(value)}" for name, value in kwargs.items()
-    ]
+    all_args = [repr(arg) for arg in args] + [f"{name}={value!r}" for name, value in kwargs.items()]
     return f"{name}({', '.join(all_args)})"
 
 
 def _handle_error(body: str, name: str, args, kwargs):
     fmt_call = fmt_rpc_call(name, args, kwargs)
     raise RPCError(f"An exception was raised in the server during the call {fmt_call}: \n\n{body}")
```

### Comparing `stepup-1.2.0/stepup/core/runner.py` & `stepup-1.2.1/stepup/core/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,34 +15,32 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """The `Runner` delegates the execution of jobs by the workers."""
 
-
 import asyncio
 import logging
 from functools import partial
 
 import attrs
 from path import Path
 
 from .asyncio import wait_for_events
 from .hash import FileHash
 from .job import Job
 from .reporter import ReporterClient
 from .scheduler import Scheduler
-from .step import StepState, Mandatory
+from .step import Mandatory, StepState
 from .utils import remove_path
 from .watcher import Watcher
 from .worker import WorkerClient
 from .workflow import Workflow
 
-
 __all__ = ("Runner",)
 
 
 @attrs.define
 class Runner:
     # The watcher instance, used to start the watcher when the runner becomes idle.
     watcher: Watcher = attrs.field()
@@ -223,17 +221,18 @@
             waits.append(worker.close())
         await asyncio.gather(*waits)
 
 
 async def remove_files(to_be_deleted: list[tuple[str, FileHash | None]], reporter: ReporterClient):
     to_be_deleted.sort(reverse=True)
     for path, file_hash in to_be_deleted:
-        if path.endswith("/") or file_hash is None or file_hash.update(path) is False:
-            if remove_path(Path(path)):
-                await reporter("CLEAN", path)
+        if (
+            path.endswith("/") or file_hash is None or file_hash.update(path) is False
+        ) and remove_path(Path(path)):
+            await reporter("CLEAN", path)
     to_be_deleted.clear()
 
 
 async def report_completion(workflow: Workflow, scheduler: Scheduler, reporter: ReporterClient):
     """Report parts of the workflow that could not be executed."""
     success = True
     step_keys_failed = workflow.step_states.inverse.get(StepState.FAILED, ())
@@ -297,18 +296,15 @@
                 lines.append(f"{prefix}     VOLATILE  {path}")
                 prefix = "       "
 
             pending_pages.append(("PENDING Step", "\n".join(lines)))
 
         if num_pending > 0:
             success = False
-            if num_pending == 1:
-                lead = "1 step remains"
-            else:
-                lead = f"{num_pending} steps remain"
+            lead = "1 step remains" if num_pending == 1 else f"{num_pending} steps remain"
             if len(block_lines) > 0:
                 block_page = ("Blocked steps", "\n".join(block_lines))
                 await reporter("WARNING", f"{lead} pending due to blocked steps", [block_page])
             else:
                 await reporter(
                     "WARNING", f"{lead} pending due to incomplete requirements", pending_pages
                 )
```

### Comparing `stepup-1.2.0/stepup/core/scheduler.py` & `stepup-1.2.1/stepup/core/scheduler.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 import asyncio
 import itertools
 
 import attrs
 
 from .job import Job
 
-
 __all__ = ("Pool", "Scheduler")
 
 
 @attrs.define
 class Pool:
     """A single pool of which the scheduler can contain several"""
```

### Comparing `stepup-1.2.0/stepup/core/script.py` & `stepup-1.2.1/stepup/core/script.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,21 +19,21 @@
 # --
 """Support for scripts that combine planning and execution."""
 
 import argparse
 import inspect
 import os
 import sys
-from typing import Any, Iterator
+from collections.abc import Iterator
+from typing import Any
 
 import attrs
 from parse import parse
 from path import Path
 
-
 __all__ = ("driver",)
 
 
 def driver(obj=None) -> int:
     """Driver function to be called from a script as `driver()` or `driver(obj)`.
 
     Parameters
```

### Comparing `stepup-1.2.0/stepup/core/step.py` & `stepup-1.2.1/stepup/core/step.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,22 +16,23 @@
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """A `Step` is a shell command that can be executed and that has inputs and outputs."""
 
 import enum
-from typing import Any, Self, Iterator, TYPE_CHECKING, Collection
+from collections.abc import Collection, Iterator
+from typing import TYPE_CHECKING, Any, Self
 
 import attrs
 
 from .cascade import Node
 from .file import FileState
-from .hash import StepHash, ExtendedStepHash
-from .job import TryReplayJob, RunJob, ValidateAmendedJob
+from .hash import ExtendedStepHash, StepHash
+from .job import RunJob, TryReplayJob, ValidateAmendedJob
 from .nglob import NGlobMulti
 from .utils import format_digest
 
 if TYPE_CHECKING:
     from .workflow import Workflow
```

### Comparing `stepup-1.2.0/stepup/core/tui.py` & `stepup-1.2.1/stepup/core/tui.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,32 +15,30 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """StepUp terminal user interface."""
 
-
 import argparse
 import asyncio
 import os
 import subprocess
 import sys
 import tempfile
 import termios
 from decimal import Decimal
 
 import attrs
 from path import Path
 
 from .asyncio import stoppable_iterator
 from .director import interpret_num_workers
-from .rpc import serve_socket_rpc, AsyncRPCClient
-from .reporter import ReporterHandler, ReporterClient
-
+from .reporter import ReporterClient, ReporterHandler
+from .rpc import AsyncRPCClient, serve_socket_rpc
 
 __all__ = ()
 
 
 def main():
     asyncio.run(async_main())
 
@@ -75,57 +73,56 @@
         task_reporter = asyncio.create_task(
             serve_socket_rpc(reporter_handler, reporter_socket_path, stop_event),
             name="reporter-rpc",
         )
         tasks = [task_reporter]
 
         # Launch director as background process
-        log_file = open(".stepup/logs/director", "w")
         argv = [
             "-m",
             "stepup.core.director",
             args.plan_py,
             director_socket_path,
             f"--num-workers={num_workers}",
             f"--reporter={reporter_socket_path}",
         ]
         if args.show_perf > 1:
             argv.append("--show-perf")
         if args.explain_rerun:
             argv.append("--explain-rerun")
         try:
-            process_director = await asyncio.create_subprocess_exec(
-                sys.executable,
-                *argv,
-                stdin=subprocess.DEVNULL,
-                stdout=log_file,
-                stderr=subprocess.STDOUT,
-            )
-            # Instantiate keyboard interaction or work non-interactively
-            if args.interactive:
-                if sys.stdin.isatty():
+            with open(".stepup/logs/director", "w") as log_file:
+                process_director = await asyncio.create_subprocess_exec(
+                    sys.executable,
+                    *argv,
+                    stdin=subprocess.DEVNULL,
+                    stdout=log_file,
+                    stderr=subprocess.STDOUT,
+                )
+                # Instantiate keyboard interaction or work non-interactively
+                if args.interactive:
+                    if sys.stdin.isatty():
+                        await wait_for_path(director_socket_path, stop_event)
+                        task_keyboard = asyncio.create_task(
+                            keyboard(director_socket_path, reporter_socket_path, stop_event),
+                            name="keyboard",
+                        )
+                        tasks.append(task_keyboard)
+                else:
                     await wait_for_path(director_socket_path, stop_event)
-                    task_keyboard = asyncio.create_task(
-                        keyboard(director_socket_path, reporter_socket_path, stop_event),
-                        name="keyboard",
-                    )
-                    tasks.append(task_keyboard)
-            else:
-                await wait_for_path(director_socket_path, stop_event)
-                async with await AsyncRPCClient.socket(director_socket_path) as client:
-                    await client.call.join()
-            await process_director.wait()
+                    async with await AsyncRPCClient.socket(director_socket_path) as client:
+                        await client.call.join()
+                await process_director.wait()
             stop_event.set()
         finally:
             try:
                 await asyncio.gather(*tasks)
             except ConnectionRefusedError:
                 reporter_handler.report("ERROR", "Could not connect to director", [])
             finally:
-                log_file.close()
                 path_tmpsock.remove_p()
 
 
 async def wait_for_path(path: Path, stop_event: asyncio.Event):
     while not path.exists():
         if stop_event.is_set():
             return
```

### Comparing `stepup-1.2.0/stepup/core/utils.py` & `stepup-1.2.1/stepup/core/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,21 +17,20 @@
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """Small utilities used throughout."""
 
 import importlib.util
 import os
-import string
 import re
+import string
 from types import ModuleType
 
 from path import Path
 
-
 __all__ = (
     # Path manipulation
     "mynormpath",
     "myrelpath",
     "myabsolute",
     "myparent",
     "make_path_out",
@@ -124,18 +123,15 @@
         A properly formatted output path.
     """
     path_in = Path(path_in)
     if out is None or out.endswith(os.sep):
         path_out = path_in
         if ext is not None:
             path_out = Path(path_out.stem + ext)
-        if out is None:
-            path_out = path_in.parent / path_out
-        else:
-            path_out = Path(out) / path_out.basename()
+        path_out = path_in.parent / path_out if out is None else Path(out) / path_out.basename()
     else:
         path_out = Path(out)
     if path_out == path_in:
         raise ValueError(f"The output path cannot equal the input path: {path_out}")
     if not (ext is None or path_out.suffix == ext):
         raise ValueError(f"The output path does not have extension '{ext}': {path_out}.")
     return path_out
@@ -155,32 +151,31 @@
         try:
             path.remove()
             return True
         except FileNotFoundError:
             return False
         except OSError:
             return False
-    return False
 
 
 #
 # Miscellaneous
 #
 
 
-# Taken from https://stackoverflow.com/a/39542816/494584
+# Adapted from https://stackoverflow.com/a/39542816/494584
 class classproperty(property):
     def __get__(self, obj, objtype=None):
-        return super(classproperty, self).__get__(objtype)
+        return super().__get__(objtype)
 
     def __set__(self, obj, value):
-        super(classproperty, self).__set__(type(obj), value)
+        super().__set__(type(obj), value)
 
     def __delete__(self, obj):
-        super(classproperty, self).__delete__(type(obj))
+        super().__delete__(type(obj))
 
 
 class lookupdict(dict):
     """Dictionary assigning enumerated values to keys."""
 
     def __missing__(self, key):
         if not isinstance(key, str):
```

### Comparing `stepup-1.2.0/stepup/core/watcher.py` & `stepup-1.2.1/stepup/core/watcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,18 +26,17 @@
 from path import Path
 from watchdog.events import FileSystemEvent, FileSystemEventHandler, FileSystemMovedEvent
 from watchdog.observers import Observer
 
 from .asyncio import stoppable_iterator
 from .file import FileState
 from .reporter import ReporterClient
-from .utils import myrelpath, myabsolute
+from .utils import myabsolute, myrelpath
 from .workflow import Workflow
 
-
 __all__ = ("Watcher",)
 
 
 class Change(enum.Enum):
     UPDATED = 41
     DELETED = 42
 
@@ -158,15 +157,15 @@
         """Record a single event taken from the change_queue."""
         if change == Change.DELETED and path not in self.deleted:
             if self.workflow.is_relevant(path):
                 await self.reporter("DELETED", path)
                 self.deleted.add(path)
                 self.updated.discard(path)
                 self.files_changed.set()
-        elif change == Change.UPDATED and path not in self.updated:
+        elif change == Change.UPDATED and path not in self.updated:  # noqa: SIM102
             if self.workflow.is_relevant(path):
                 await self.reporter("UPDATED", path)
                 self.deleted.discard(path)
                 self.updated.add(path)
                 self.files_changed.set()
```

### Comparing `stepup-1.2.0/stepup/core/worker.py` & `stepup-1.2.1/stepup/core/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,34 +15,33 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """Worker process."""
 
-
 import argparse
 import asyncio
 import os
 import resource
 import sys
 from time import perf_counter
 
 import attrs
 from path import Path
 
 from stepup.core.utils import check_inp_path
+
 from .exceptions import RPCError
-from .hash import FileHash, compare_step_hashes, StepHash, create_step_hash
+from .file import FileState
+from .hash import FileHash, StepHash, compare_step_hashes, create_step_hash
 from .reporter import ReporterClient
-from .rpc import serve_stdio_rpc, AsyncRPCClient, allow_rpc
+from .rpc import AsyncRPCClient, allow_rpc, serve_stdio_rpc
+from .step import Step, StepState
 from .workflow import Workflow
-from .step import StepState, Step
-from .file import FileState
-
 
 __all__ = ("WorkerClient", "WorkerStep", "WorkerHandler")
 
 
 #
 # In the main director process
 #
@@ -75,15 +74,15 @@
     client: AsyncRPCClient | None = attrs.field(init=False, default=None)
 
     #
     # Setup and teardown
     #
 
     async def boot(self):
-        log_file = open(f".stepup/logs/worker{self.idx}", "w")
+        log_file = open(f".stepup/logs/worker{self.idx}", "w")  # noqa: SIM115
         args = [
             "-m",
             "stepup.core.worker",
             self.director_socket_path,
         ]
         if self.show_perf:
             args.append("--show-perf")
```

### Comparing `stepup-1.2.0/stepup/core/workflow.py` & `stepup-1.2.1/stepup/core/workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,28 +19,29 @@
 # --
 """The `Workflow` is a `Cascade` subclass with more concrete node implementations."""
 
 import asyncio
 import json
 import os
 import textwrap
-from typing import cast, Collection, Self
 from collections import Counter
+from collections.abc import Collection
+from typing import Self, cast
 
 import attrs
 
 from .assoc import Assoc, many_to_one
 from .cascade import Cascade, Node, get_kind
+from .deferred_glob import DeferredGlob
 from .exceptions import GraphError
 from .file import File, FileState
-from .hash import FileHash, ExtendedStepHash
+from .hash import ExtendedStepHash, FileHash
 from .nglob import NGlobMulti
-from .deferred_glob import DeferredGlob
-from .step import Step, StepState, Mandatory
-from .utils import myparent, lookupdict
+from .step import Mandatory, Step, StepState
+from .utils import lookupdict, myparent
 
 __all__ = ("Workflow",)
 
 
 @attrs.define
 class Workflow(Cascade):
     # Steps ready for scheduling and execution.
@@ -82,17 +83,16 @@
         return workflow
 
     def check_consistency(self):
         super().check_consistency()
         # Check whether the initial graph satisfies all constraints.
         for node_key in self.nodes:
             creator_key = self.get_creator(node_key)
-            if get_kind(creator_key) == "step":
-                if node_key == creator_key:
-                    raise ValueError("A step cannot be its own creator")
+            if get_kind(creator_key) == "step" and node_key == creator_key:
+                raise ValueError("A step cannot be its own creator")
             if get_kind(node_key) == "file":
                 parent_key = self.get_parent_key(node_key[5:], allow_orphan=True)
                 if not (parent_key is None or parent_key in self.suppliers.get(node_key, ())):
                     raise ValueError(f"File is not consumer of its parent: {node_key}")
 
     @staticmethod
     def default_node_classes() -> dict[str, type[Node]]:
@@ -435,22 +435,20 @@
             # because adding these may require adding their parent paths.
             if not creator_key.startswith("dg:"):
                 try:
                     parent_key = self.get_parent_key(path)
                     if not (
                         parent_key is None or self.file_states.get(parent_key) == FileState.STATIC
                     ):
-                        raise GraphError(
-                            f"Static path does not have static parent path node: {path}"
-                        )
-                except ValueError:
+                        raise GraphError(f"Static path has no static parent path node: {path}")
+                except ValueError as exc:
                     parent_path = myparent(path)
                     if parent_path not in paths:
-                        raise GraphError(f"Static path does not have a parent path node: {path}")
-            #
+                        raise GraphError(f"Static path has no parent path node: {path}") from exc
+
             file_key = f"file:{path}"
             if file_key in self.nodes:
                 if file_key in self.nodes and not self.is_orphan(file_key):
                     raise GraphError(f"Static path already exists: {path}")
                 self.check_cyclic(creator_key, file_key)
         # Make the actual changes
         self.graph_changed = True
```

### Comparing `stepup-1.2.0/stepup.egg-info/PKG-INFO` & `stepup-1.2.1/stepup.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stepup
-Version: 1.2.0
+Version: 1.2.1
 Summary: StepUp Core provides the basic framework for the StepUp build tool
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
 Project-URL: Documentation, https://reproducible-reporting.github.io/stepup-core/
 Project-URL: Issues, https://github.com/reproducible-reporting/stepup-core/issues
 Project-URL: Source, https://github.com/reproducible-reporting/stepup-core/
 Project-URL: Changelog, https://reproducible-reporting.github.io/stepup-core/changelog/
 Classifier: Environment :: Console
@@ -31,14 +31,15 @@
 Requires-Dist: mkdocs-macros-plugin; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 Requires-Dist: numpy; extra == "dev"
 Requires-Dist: matplotlib; extra == "dev"
 
 [![release](https://github.com/reproducible-reporting/stepup-core/actions/workflows/release.yaml/badge.svg)](https://github.com/reproducible-reporting/stepup-core/actions/workflows/release.yaml)
 [![pytest](https://github.com/reproducible-reporting/stepup-core/actions/workflows/pytest.yaml/badge.svg)](https://github.com/reproducible-reporting/stepup-core/actions/workflows/pytest.yaml)
+[![mkdocs](https://github.com/reproducible-reporting/stepup-core/actions/workflows/mkdocs.yaml/badge.svg)](https://github.com/reproducible-reporting/stepup-core/actions/workflows/mkdocs.yaml)
 [![PyPI Version](https://img.shields.io/pypi/v/stepup)](https://pypi.org/project/stepup/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/stepup)
 ![GPL-3 License](https://img.shields.io/github/license/reproducible-reporting/stepup-core)
 
 # StepUp Core
 
 StepUp is a simple, powerful and universal build tool.
```

### Comparing `stepup-1.2.0/stepup.egg-info/SOURCES.txt` & `stepup-1.2.1/stepup.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,14 @@
 stepup.egg-info/PKG-INFO
 stepup.egg-info/SOURCES.txt
 stepup.egg-info/dependency_links.txt
 stepup.egg-info/entry_points.txt
 stepup.egg-info/requires.txt
 stepup.egg-info/top_level.txt
 stepup/core/__init__.py
-stepup/core/_version.py
 stepup/core/api.py
 stepup/core/assoc.py
 stepup/core/asyncio.py
 stepup/core/cascade.py
 stepup/core/cleanup.py
 stepup/core/deferred_glob.py
 stepup/core/director.py
```

### Comparing `stepup-1.2.0/tests/cases/README.md` & `stepup-1.2.1/tests/cases/README.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/amend/expected_graph_01.txt` & `stepup-1.2.1/tests/cases/amend/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/amend/expected_graph_02.txt` & `stepup-1.2.1/tests/cases/amend/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/amend/expected_graph_03.txt` & `stepup-1.2.1/tests/cases/amend/expected_graph_03.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/amend/expected_graph_04.txt` & `stepup-1.2.1/tests/cases/amend/expected_graph_04.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/amend/expected_stdout_01.txt` & `stepup-1.2.1/tests/cases/amend/expected_stdout_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/amend/expected_stdout_02.txt` & `stepup-1.2.1/tests/cases/amend/expected_stdout_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/amend/expected_stdout_03.txt` & `stepup-1.2.1/tests/cases/amend/expected_stdout_03.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/amend/main.sh` & `stepup-1.2.1/tests/cases/amend/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/amend_delay/expected_graph_01.txt` & `stepup-1.2.1/tests/cases/amend_delay/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/amend_delay/expected_graph_02.txt` & `stepup-1.2.1/tests/cases/amend_delay/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/amend_delay/expected_graph_03.txt` & `stepup-1.2.1/tests/cases/amend_delay/expected_graph_03.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/amend_delay/expected_stdout.txt` & `stepup-1.2.1/tests/cases/amend_delay/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/amend_delay/main.sh` & `stepup-1.2.1/tests/cases/amend_delay/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/amend_env_vars/expected_graph.txt` & `stepup-1.2.1/tests/cases/amend_env_vars/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/amend_env_vars/main.sh` & `stepup-1.2.1/tests/cases/amend_env_vars/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/amend_missing/expected_graph.txt` & `stepup-1.2.1/tests/cases/amend_missing/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/amend_missing/expected_stdout.txt` & `stepup-1.2.1/tests/cases/amend_missing/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/amend_missing/main.sh` & `stepup-1.2.1/tests/cases/amend_missing/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/amend_outdir_pending/expected_graph.txt` & `stepup-1.2.1/tests/cases/amend_outdir_pending/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/amend_outdir_pending/expected_stdout.txt` & `stepup-1.2.1/tests/cases/amend_outdir_pending/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/amend_outdir_pending/main.sh` & `stepup-1.2.1/tests/cases/amend_outdir_pending/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/amend_voldir_pending/expected_graph.txt` & `stepup-1.2.1/tests/cases/amend_voldir_pending/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/amend_voldir_pending/expected_stdout.txt` & `stepup-1.2.1/tests/cases/amend_voldir_pending/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/amend_voldir_pending/main.sh` & `stepup-1.2.1/tests/cases/amend_voldir_pending/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/deferred_glob1/expected_graph_01.txt` & `stepup-1.2.1/tests/cases/deferred_glob1/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/deferred_glob1/expected_graph_02.txt` & `stepup-1.2.1/tests/cases/deferred_glob1/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/deferred_glob1/main.sh` & `stepup-1.2.1/tests/cases/deferred_glob1/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/deferred_glob2/expected_graph_01.txt` & `stepup-1.2.1/tests/cases/deferred_glob2/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/deferred_glob2/expected_graph_02.txt` & `stepup-1.2.1/tests/cases/deferred_glob2/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/deferred_glob2/expected_stdout.txt` & `stepup-1.2.1/tests/cases/deferred_glob2/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/deferred_glob2/main.sh` & `stepup-1.2.1/tests/cases/deferred_glob2/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/deferred_subdir/expected_graph.txt` & `stepup-1.2.1/tests/cases/deferred_subdir/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/deferred_subdir/main.sh` & `stepup-1.2.1/tests/cases/deferred_subdir/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/env_vars/expected_graph_01.txt` & `stepup-1.2.1/tests/cases/env_vars/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/env_vars/expected_graph_02.txt` & `stepup-1.2.1/tests/cases/env_vars/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/env_vars/expected_graph_03.txt` & `stepup-1.2.1/tests/cases/env_vars/expected_graph_03.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/env_vars/expected_graph_04.txt` & `stepup-1.2.1/tests/cases/env_vars/expected_graph_04.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/env_vars/expected_graph_05.txt` & `stepup-1.2.1/tests/cases/env_vars/expected_graph_05.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/env_vars/expected_stdout_a.txt` & `stepup-1.2.1/tests/cases/env_vars/expected_stdout_a.txt`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Same step hash       extended, digest 58d07c3f, inp_digset 58d07c3f
 Same inp hash        ./
 Same inp hash        demovars.py
 Same inp hash        variables.json
 ────────────────────────────────────────────────────────────────────────────────
       SKIP │ ./printvars.py
 ───────────────────────────── No changes observed ──────────────────────────────
-Same step hash       extended, digest d52c2733, inp_digset 2a71c927
+Same step hash       extended, digest 0acb0b1e, inp_digset 9419840d
 Same inp hash        ./
 Same inp hash        printvars.py
 Same env var         ENV_VAR_TEST_STEPUP_AWDFTD ='AAAA'
 Same env var         ENV_VAR_TEST_STEPUP_DFTHYH ='BBBB'
 Same out hash        current_variables.txt
 ────────────────────────────────────────────────────────────────────────────────
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
```

### Comparing `stepup-1.2.0/tests/cases/env_vars/expected_stdout_b.txt` & `stepup-1.2.1/tests/cases/env_vars/expected_stdout_d.txt`

 * *Files 4% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 Same step hash       extended, digest 58d07c3f, inp_digset 58d07c3f
 Same inp hash        ./
 Same inp hash        demovars.py
 Same inp hash        variables.json
 ────────────────────────────────────────────────────────────────────────────────
     NOSKIP │ ./printvars.py
 ──────────────────────────── Changes causing rerun ─────────────────────────────
-Modified step hash   extended, digest d52c2733 ➜ 170341b4, inp_digset 2a71c927 ➜ b6f74e79
-Modified env var     ENV_VAR_TEST_STEPUP_DFTHYH ='BBBB' ➜ ='CCCC'
+Modified step hash   extended, digest 564da52a ➜ e4352467, inp_digset 7ec4d750 ➜ 4927786d
+Modified env var     ENV_VAR_TEST_STEPUP_AWDFTD (unset) ➜ ='DDDD'
 ────────────────────────────── Remained the same ───────────────────────────────
 Same inp hash        ./
 Same inp hash        printvars.py
-Same env var         ENV_VAR_TEST_STEPUP_AWDFTD ='AAAA'
+Same env var         ENV_VAR_TEST_STEPUP_DFTHYH ='CCCC'
 Same out hash        current_variables.txt
 ────────────────────────────────────────────────────────────────────────────────
      START │ ./printvars.py
    SUCCESS │ ./printvars.py
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
   DIRECTOR │ Stopping workers.
```

### Comparing `stepup-1.2.0/tests/cases/env_vars/expected_stdout_c.txt` & `stepup-1.2.1/tests/cases/env_vars/expected_stdout_c.txt`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 Same step hash       extended, digest 58d07c3f, inp_digset 58d07c3f
 Same inp hash        ./
 Same inp hash        demovars.py
 Same inp hash        variables.json
 ────────────────────────────────────────────────────────────────────────────────
     NOSKIP │ ./printvars.py
 ──────────────────────────── Changes causing rerun ─────────────────────────────
-Modified step hash   extended, digest 4b6ff17e ➜ ec75d2f2, inp_digset b6f74e79 ➜ b3c18f7e
+Modified step hash   extended, digest 430ca894 ➜ 45ddbcc4, inp_digset a84a12a5 ➜ 7ec4d750
 Modified env var     ENV_VAR_TEST_STEPUP_AWDFTD ='AAAA' ➜ (unset)
 ────────────────────────────── Remained the same ───────────────────────────────
 Same inp hash        ./
 Same inp hash        printvars.py
 Same env var         ENV_VAR_TEST_STEPUP_DFTHYH ='CCCC'
 Same out hash        current_variables.txt
 ────────────────────────────────────────────────────────────────────────────────
```

### Comparing `stepup-1.2.0/tests/cases/env_vars/expected_stdout_d.txt` & `stepup-1.2.1/tests/cases/env_vars/expected_stdout_b.txt`

 * *Files 3% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 Same step hash       extended, digest 58d07c3f, inp_digset 58d07c3f
 Same inp hash        ./
 Same inp hash        demovars.py
 Same inp hash        variables.json
 ────────────────────────────────────────────────────────────────────────────────
     NOSKIP │ ./printvars.py
 ──────────────────────────── Changes causing rerun ─────────────────────────────
-Modified step hash   extended, digest 759b9c26 ➜ cb1aa93f, inp_digset b3c18f7e ➜ a11013a2
-Modified env var     ENV_VAR_TEST_STEPUP_AWDFTD (unset) ➜ ='DDDD'
+Modified step hash   extended, digest 0acb0b1e ➜ 4d2473bd, inp_digset 9419840d ➜ a84a12a5
+Modified env var     ENV_VAR_TEST_STEPUP_DFTHYH ='BBBB' ➜ ='CCCC'
 ────────────────────────────── Remained the same ───────────────────────────────
 Same inp hash        ./
 Same inp hash        printvars.py
-Same env var         ENV_VAR_TEST_STEPUP_DFTHYH ='CCCC'
+Same env var         ENV_VAR_TEST_STEPUP_AWDFTD ='AAAA'
 Same out hash        current_variables.txt
 ────────────────────────────────────────────────────────────────────────────────
      START │ ./printvars.py
    SUCCESS │ ./printvars.py
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
   DIRECTOR │ Stopping workers.
```

### Comparing `stepup-1.2.0/tests/cases/env_vars/main.sh` & `stepup-1.2.1/tests/cases/env_vars/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/env_vars_amend/expected_graph_01.txt` & `stepup-1.2.1/tests/cases/env_vars_amend/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/env_vars_amend/expected_graph_02.txt` & `stepup-1.2.1/tests/cases/env_vars_amend/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/env_vars_amend/expected_stdout_02.txt` & `stepup-1.2.1/tests/cases/env_vars_amend/expected_stdout_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/env_vars_amend/main.sh` & `stepup-1.2.1/tests/cases/env_vars_amend/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/env_vars_path/expected_graph_01.txt` & `stepup-1.2.1/tests/cases/env_vars_path/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/env_vars_path/expected_graph_02.txt` & `stepup-1.2.1/tests/cases/env_vars_path/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/env_vars_path/expected_stdout_01.txt` & `stepup-1.2.1/tests/cases/env_vars_path/expected_stdout_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/env_vars_path/expected_stdout_02.txt` & `stepup-1.2.1/tests/cases/env_vars_path/expected_stdout_02.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
   WORKFLOW │ Loaded from .stepup/workflow.mpk.xz
   DIRECTOR │ Launched worker 0
      PHASE │ run
     NOSKIP │ ./plan.py
 ──────────────────────────── Changes causing rerun ─────────────────────────────
-Modified step hash   extended, digest 20bbb647 ➜ c4b2f903, inp_digset 20bbb647 ➜ c4b2f903
+Modified step hash   extended, digest f9085952 ➜ f2fab713, inp_digset f9085952 ➜ f2fab713
 Modified env var     ENV_VAR_TEST_STEPUP_PREFIX ='README' ➜ ='FOO'
 ────────────────────────────── Remained the same ───────────────────────────────
 Same inp hash        ./
 Same inp hash        plan.py
 ────────────────────────────────────────────────────────────────────────────────
      START │ ./plan.py
    SUCCESS │ ./plan.py
```

### Comparing `stepup-1.2.0/tests/cases/env_vars_path/main.sh` & `stepup-1.2.1/tests/cases/env_vars_path/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/env_vars_subs/expected_graph.txt` & `stepup-1.2.1/tests/cases/env_vars_subs/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/env_vars_subs/expected_stdout.txt` & `stepup-1.2.1/tests/cases/env_vars_subs/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/env_vars_subs/main.sh` & `stepup-1.2.1/tests/cases/env_vars_subs/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/env_vars_workdir/expected_graph.txt` & `stepup-1.2.1/tests/cases/env_vars_workdir/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/env_vars_workdir/main.sh` & `stepup-1.2.1/tests/cases/env_vars_workdir/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/error_cyclic_late/expected_graph.txt` & `stepup-1.2.1/tests/cases/error_cyclic_late/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/error_cyclic_late/expected_stdout.txt` & `stepup-1.2.1/tests/cases/error_cyclic_late/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/error_cyclic_late/main.sh` & `stepup-1.2.1/tests/cases/error_cyclic_late/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/error_deferred_nonexisting/expected_stdout.txt` & `stepup-1.2.1/tests/cases/error_deferred_nonexisting/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/error_deferred_nonexisting/main.sh` & `stepup-1.2.1/tests/cases/error_deferred_nonexisting/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/error_env_var/expected_graph.txt` & `stepup-1.2.1/tests/cases/error_env_var/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/error_env_var/expected_stdout.txt` & `stepup-1.2.1/tests/cases/error_env_var/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/error_env_var/main.sh` & `stepup-1.2.1/tests/cases/error_env_var/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/error_main_fails/expected_graph_01.txt` & `stepup-1.2.1/tests/cases/error_main_fails/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/error_main_fails/expected_graph_02.txt` & `stepup-1.2.1/tests/cases/error_main_fails/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/error_main_fails/expected_stdout_02.txt` & `stepup-1.2.1/tests/cases/error_main_fails/expected_stdout_02.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
   WORKFLOW │ Loaded from .stepup/workflow.mpk.xz
   DIRECTOR │ Launched worker 0
      PHASE │ run
     NOSKIP │ ./plan.py
 ──────────────────────────── Changes causing rerun ─────────────────────────────
-Modified step hash   extended, digest 53ca023c ➜ cc5deac6, inp_digset 53ca023c ➜ cc5deac6
-Modified inp hash    plan.py (digest 98e52b4a ➜ 66b966f4, size 101 ➜ 36)
+Modified step hash   extended, digest 53ca023c ➜ 59506490, inp_digset 53ca023c ➜ 59506490
+Modified inp hash    plan.py (digest 98e52b4a ➜ 6057f437, size 101 ➜ 46)
 ────────────────────────────── Remained the same ───────────────────────────────
 Same inp hash        ./
 ────────────────────────────────────────────────────────────────────────────────
      START │ ./plan.py
       FAIL │ ./plan.py
 ────────────────────────────────── Step info ───────────────────────────────────
 Command               ./plan.py
```

### Comparing `stepup-1.2.0/tests/cases/error_main_fails/main.sh` & `stepup-1.2.1/tests/cases/error_main_fails/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/error_not_executable/expected_stdout.txt` & `stepup-1.2.1/tests/cases/error_not_executable/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/error_overlap_deferred/expected_stdout.txt` & `stepup-1.2.1/tests/cases/error_overlap_deferred/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/error_overlap_deferred/main.sh` & `stepup-1.2.1/tests/cases/error_overlap_deferred/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/error_static_dir/expected_graph.txt` & `stepup-1.2.1/tests/cases/error_static_dir/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/error_static_dir/expected_stdout.txt` & `stepup-1.2.1/tests/cases/error_static_dir/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/error_static_dir/main.sh` & `stepup-1.2.1/tests/cases/error_static_dir/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/error_step/expected_graph.txt` & `stepup-1.2.1/tests/cases/error_step/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/error_step/expected_stdout.txt` & `stepup-1.2.1/tests/cases/error_step/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/error_step/main.sh` & `stepup-1.2.1/tests/cases/error_step/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/here/expected_graph.txt` & `stepup-1.2.1/tests/cases/here/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/here/expected_stdout.txt` & `stepup-1.2.1/tests/cases/here/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/here/main.sh` & `stepup-1.2.1/tests/cases/here/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/makedirs/expected_graph.txt` & `stepup-1.2.1/tests/cases/makedirs/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/makedirs/main.sh` & `stepup-1.2.1/tests/cases/makedirs/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/mkdir/expected_graph.txt` & `stepup-1.2.1/tests/cases/mkdir/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/mkdir/main.sh` & `stepup-1.2.1/tests/cases/mkdir/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/mkdir_error/expected_graph.txt` & `stepup-1.2.1/tests/cases/mkdir_error/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/mkdir_error/expected_stdout.txt` & `stepup-1.2.1/tests/cases/mkdir_error/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/mkdir_error/main.sh` & `stepup-1.2.1/tests/cases/mkdir_error/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/nodata/expected_graph_01.txt` & `stepup-1.2.1/tests/cases/nodata/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/nodata/expected_graph_02.txt` & `stepup-1.2.1/tests/cases/nodata/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/nodata/expected_graph_03.txt` & `stepup-1.2.1/tests/cases/nodata/expected_graph_03.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/nodata/expected_stdout_a.txt` & `stepup-1.2.1/tests/cases/nodata/expected_stdout_a.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/nodata/expected_stdout_b.txt` & `stepup-1.2.1/tests/cases/nodata/expected_stdout_b.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/nodata/main.sh` & `stepup-1.2.1/tests/cases/nodata/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/noplan/expected_stdout.txt` & `stepup-1.2.1/tests/cases/noplan/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/nostatic/expected_graph.txt` & `stepup-1.2.1/tests/cases/nostatic/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/nostatic/expected_stdout.txt` & `stepup-1.2.1/tests/cases/nostatic/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/nostatic/main.sh` & `stepup-1.2.1/tests/cases/nostatic/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/not_cyclic/expected_graph_01.txt` & `stepup-1.2.1/tests/cases/not_cyclic/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/not_cyclic/expected_graph_02.txt` & `stepup-1.2.1/tests/cases/not_cyclic/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/not_cyclic/expected_graph_03.txt` & `stepup-1.2.1/tests/cases/not_cyclic/expected_graph_03.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/not_cyclic/expected_stdout.txt` & `stepup-1.2.1/tests/cases/not_cyclic/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/not_cyclic/main.sh` & `stepup-1.2.1/tests/cases/not_cyclic/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/optional_convert/expected_graph_a.txt` & `stepup-1.2.1/tests/cases/optional_convert/expected_graph_a.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/optional_convert/expected_graph_b.txt` & `stepup-1.2.1/tests/cases/optional_convert/expected_graph_b.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/optional_convert/expected_graph_c.txt` & `stepup-1.2.1/tests/cases/optional_convert/expected_graph_c.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/optional_convert/expected_stdout_a.txt` & `stepup-1.2.1/tests/cases/optional_convert/expected_stdout_a.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/optional_convert/main.sh` & `stepup-1.2.1/tests/cases/optional_convert/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/output_not_created/expected_graph.txt` & `stepup-1.2.1/tests/cases/output_not_created/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/output_not_created/expected_stdout.txt` & `stepup-1.2.1/tests/cases/output_not_created/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/output_not_created/main.sh` & `stepup-1.2.1/tests/cases/output_not_created/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/pending/expected_graph.txt` & `stepup-1.2.1/tests/cases/pending/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/pending/expected_stdout.txt` & `stepup-1.2.1/tests/cases/pending/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/pending/main.sh` & `stepup-1.2.1/tests/cases/pending/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/permissions_file_rerun/expected_graph_01.txt` & `stepup-1.2.1/tests/cases/permissions_file_rerun/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/permissions_file_rerun/expected_graph_02.txt` & `stepup-1.2.1/tests/cases/permissions_file_rerun/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/permissions_file_rerun/expected_stdout.txt` & `stepup-1.2.1/tests/cases/permissions_file_rerun/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/permissions_file_rerun/main.sh` & `stepup-1.2.1/tests/cases/permissions_file_rerun/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/permissions_plan_rerun/expected_graph_01.txt` & `stepup-1.2.1/tests/cases/permissions_plan_rerun/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/permissions_plan_rerun/expected_graph_02.txt` & `stepup-1.2.1/tests/cases/permissions_plan_rerun/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/permissions_plan_rerun/expected_stdout.txt` & `stepup-1.2.1/tests/cases/permissions_plan_rerun/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/permissions_plan_rerun/main.sh` & `stepup-1.2.1/tests/cases/permissions_plan_rerun/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/permissions_plan_restart/expected_graph_01.txt` & `stepup-1.2.1/tests/cases/permissions_plan_restart/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/permissions_plan_restart/expected_graph_02.txt` & `stepup-1.2.1/tests/cases/permissions_plan_restart/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/permissions_plan_restart/expected_stdout_01.txt` & `stepup-1.2.1/tests/cases/permissions_plan_restart/expected_stdout_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/permissions_plan_restart/expected_stdout_02.txt` & `stepup-1.2.1/tests/cases/permissions_plan_restart/expected_stdout_02.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
   WORKFLOW │ Loaded from .stepup/workflow.mpk.xz
   DIRECTOR │ Launched worker 0
      PHASE │ run
       SKIP │ ./plan.py
 ───────────────────────────── No changes observed ──────────────────────────────
-Same step hash       extended, digest 97a2efee, inp_digset 97a2efee
+Same step hash       extended, digest 73bc1a4e, inp_digset 73bc1a4e
 Same inp hash        ./
 Same inp hash        plan.py
 ────────────────────────────────────────────────────────────────────────────────
      START │ ./plan.py  # wd=sub/
    SUCCESS │ ./plan.py  # wd=sub/
      START │ touch done.txt  # wd=sub/
    SUCCESS │ touch done.txt  # wd=sub/
```

### Comparing `stepup-1.2.0/tests/cases/permissions_plan_restart/main.sh` & `stepup-1.2.1/tests/cases/permissions_plan_restart/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/permissions_step_rerun/expected_graph_01.txt` & `stepup-1.2.1/tests/cases/permissions_step_rerun/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/permissions_step_rerun/expected_graph_02.txt` & `stepup-1.2.1/tests/cases/permissions_step_rerun/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/permissions_step_rerun/expected_stdout.txt` & `stepup-1.2.1/tests/cases/permissions_step_rerun/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/permissions_step_rerun/main.sh` & `stepup-1.2.1/tests/cases/permissions_step_rerun/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/permissions_step_restart/expected_graph_01.txt` & `stepup-1.2.1/tests/cases/permissions_step_restart/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/permissions_step_restart/expected_graph_02.txt` & `stepup-1.2.1/tests/cases/permissions_step_restart/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/permissions_step_restart/expected_stdout_01.txt` & `stepup-1.2.1/tests/cases/permissions_step_restart/expected_stdout_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/permissions_step_restart/expected_stdout_02.txt` & `stepup-1.2.1/tests/cases/permissions_step_restart/expected_stdout_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/permissions_step_restart/main.sh` & `stepup-1.2.1/tests/cases/permissions_step_restart/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/pool/expected_graph.txt` & `stepup-1.2.1/tests/cases/pool/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/pool/expected_stdout.txt` & `stepup-1.2.1/tests/cases/pool/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/pool/main.sh` & `stepup-1.2.1/tests/cases/pool/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/reqdir_missing/expected_graph.txt` & `stepup-1.2.1/tests/cases/reqdir_missing/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/reqdir_missing/expected_stdout.txt` & `stepup-1.2.1/tests/cases/reqdir_missing/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/reqdir_missing/main.sh` & `stepup-1.2.1/tests/cases/reqdir_missing/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/restart_blocked/expected_graph_01.txt` & `stepup-1.2.1/tests/cases/restart_blocked/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/restart_blocked/expected_graph_02.txt` & `stepup-1.2.1/tests/cases/restart_blocked/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/restart_blocked/expected_stdout_01.txt` & `stepup-1.2.1/tests/cases/restart_blocked/expected_stdout_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/restart_blocked/expected_stdout_02.txt` & `stepup-1.2.1/tests/cases/restart_blocked/expected_stdout_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/restart_blocked/main.sh` & `stepup-1.2.1/tests/cases/restart_blocked/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/restart_changes/expected_graph_01.txt` & `stepup-1.2.1/tests/cases/restart_changes/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/restart_changes/expected_graph_02.txt` & `stepup-1.2.1/tests/cases/restart_changes/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/restart_changes/expected_stdout_02.txt` & `stepup-1.2.1/tests/cases/restart_changes/expected_stdout_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/restart_changes/main.sh` & `stepup-1.2.1/tests/cases/restart_changes/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/restart_deferred_glob/expected_graph_01.txt` & `stepup-1.2.1/tests/cases/restart_deferred_glob/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/restart_deferred_glob/expected_graph_02.txt` & `stepup-1.2.1/tests/cases/restart_deferred_glob/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/restart_deferred_glob/expected_stdout_01.txt` & `stepup-1.2.1/tests/cases/restart_deferred_glob/expected_stdout_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/restart_deferred_glob/expected_stdout_02.txt` & `stepup-1.2.1/tests/cases/restart_deferred_glob/expected_stdout_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/restart_deferred_glob/main.sh` & `stepup-1.2.1/tests/cases/restart_deferred_glob/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/restart_nochanges/expected_graph_01.txt` & `stepup-1.2.1/tests/cases/restart_nochanges/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/restart_nochanges/expected_graph_02.txt` & `stepup-1.2.1/tests/cases/restart_nochanges/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/restart_nochanges/expected_stdout_01.txt` & `stepup-1.2.1/tests/cases/restart_nochanges/expected_stdout_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/restart_nochanges/expected_stdout_02.txt` & `stepup-1.2.1/tests/cases/restart_nochanges/expected_stdout_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/restart_nochanges/main.sh` & `stepup-1.2.1/tests/cases/restart_nochanges/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/restart_orphan/expected_graph_01.txt` & `stepup-1.2.1/tests/cases/restart_orphan/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/restart_orphan/expected_graph_02.txt` & `stepup-1.2.1/tests/cases/restart_orphan/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/restart_orphan/expected_stdout_02.txt` & `stepup-1.2.1/tests/cases/restart_orphan/expected_stdout_02.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
   WORKFLOW │ Loaded from .stepup/workflow.mpk.xz
   DIRECTOR │ Launched worker 0
      PHASE │ run
       SKIP │ ./plan.py
 ───────────────────────────── No changes observed ──────────────────────────────
-Same step hash       extended, digest 45f26b3e, inp_digset 45f26b3e
+Same step hash       extended, digest f26ce644, inp_digset f26ce644
 Same inp hash        ./
 Same inp hash        plan.py
 ────────────────────────────────────────────────────────────────────────────────
       SKIP │ echo test > foo.txt
 ───────────────────────────── No changes observed ──────────────────────────────
 Same step hash       extended, digest 53875d0a, inp_digset 91626af7
 Same inp hash        ./
```

### Comparing `stepup-1.2.0/tests/cases/restart_orphan/main.sh` & `stepup-1.2.1/tests/cases/restart_orphan/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/restart_outdated_amend/expected_graph_01.txt` & `stepup-1.2.1/tests/cases/restart_outdated_amend/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/restart_outdated_amend/expected_graph_02.txt` & `stepup-1.2.1/tests/cases/restart_outdated_amend/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/restart_outdated_amend/expected_stdout_02.txt` & `stepup-1.2.1/tests/cases/restart_outdated_amend/expected_stdout_02.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
   WORKFLOW │ Loaded from .stepup/workflow.mpk.xz
   DIRECTOR │ Launched worker 0
      PHASE │ run
       SKIP │ ./plan.py
 ───────────────────────────── No changes observed ──────────────────────────────
-Same step hash       extended, digest 03904dae, inp_digset 03904dae
+Same step hash       extended, digest edb0b44b, inp_digset edb0b44b
 Same inp hash        ./
 Same inp hash        plan.py
 ────────────────────────────────────────────────────────────────────────────────
  DROPAMEND │ ./step.py
 ────────────────────── Outdated amended step information ───────────────────────
 Modified step hash   extended, digest 764de23c ➜ ccae7573, inp_digset d7b8a410 ➜ 7eb5fb40
 Modified inp hash    subs.txt (digest 30d31453 ➜ c273a7ee)
```

### Comparing `stepup-1.2.0/tests/cases/restart_outdated_amend/main.sh` & `stepup-1.2.1/tests/cases/restart_outdated_amend/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/restart_output/expected_graph_01.txt` & `stepup-1.2.1/tests/cases/restart_output/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/restart_output/expected_graph_02.txt` & `stepup-1.2.1/tests/cases/restart_output/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/restart_output/expected_stdout_02.txt` & `stepup-1.2.1/tests/cases/restart_output/expected_stdout_02.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
   WORKFLOW │ Loaded from .stepup/workflow.mpk.xz
   DIRECTOR │ Launched worker 0
      PHASE │ run
       SKIP │ ./plan.py
 ───────────────────────────── No changes observed ──────────────────────────────
-Same step hash       extended, digest 8d0cad40, inp_digset 8d0cad40
+Same step hash       extended, digest c961e387, inp_digset c961e387
 Same inp hash        ./
 Same inp hash        plan.py
 ────────────────────────────────────────────────────────────────────────────────
     NOSKIP │ cp -aT original.txt copy.txt
 ───────────────────────────── Missing output files ─────────────────────────────
 copy.txt
 ────────────────────────────── Remained the same ───────────────────────────────
```

### Comparing `stepup-1.2.0/tests/cases/restart_output/main.sh` & `stepup-1.2.1/tests/cases/restart_output/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/script_cases/expected_graph.txt` & `stepup-1.2.1/tests/cases/script_cases/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/script_cases/main.sh` & `stepup-1.2.1/tests/cases/script_cases/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/script_cases_settings/README.md` & `stepup-1.2.1/tests/cases/script_cases_settings/README.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/script_cases_settings/expected_graph.txt` & `stepup-1.2.1/tests/cases/script_cases_settings/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/script_cases_settings/main.sh` & `stepup-1.2.1/tests/cases/script_cases_settings/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/script_single/expected_graph.txt` & `stepup-1.2.1/tests/cases/script_single/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/script_single/expected_stdout.txt` & `stepup-1.2.1/tests/cases/script_single/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/script_single/main.sh` & `stepup-1.2.1/tests/cases/script_single/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/script_single/work/generate.py` & `stepup-1.2.1/tests/cases/script_single/work/generate.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/static/expected_graph.txt` & `stepup-1.2.1/tests/cases/static/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/static/main.sh` & `stepup-1.2.1/tests/cases/static/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/static_abs/expected_graph.txt` & `stepup-1.2.1/tests/cases/static_abs/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/static_abs/main.sh` & `stepup-1.2.1/tests/cases/static_abs/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/static_dir/expected_graph.txt` & `stepup-1.2.1/tests/cases/static_dir/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/static_dir/main.sh` & `stepup-1.2.1/tests/cases/static_dir/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/static_glob/expected_graph_01.txt` & `stepup-1.2.1/tests/cases/static_glob/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/static_glob/expected_graph_02.txt` & `stepup-1.2.1/tests/cases/static_glob/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/static_glob/expected_graph_03.txt` & `stepup-1.2.1/tests/cases/static_glob/expected_graph_03.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/static_glob/expected_stdout_a.txt` & `stepup-1.2.1/tests/cases/static_glob/expected_stdout_a.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/static_glob/expected_stdout_b.txt` & `stepup-1.2.1/tests/cases/static_glob/expected_stdout_b.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/static_glob/main.sh` & `stepup-1.2.1/tests/cases/static_glob/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/static_nglob/expected_graph_01.txt` & `stepup-1.2.1/tests/cases/static_nglob/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/static_nglob/expected_graph_02.txt` & `stepup-1.2.1/tests/cases/static_nglob/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/static_nglob/expected_stdout.txt` & `stepup-1.2.1/tests/cases/static_nglob/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/static_nglob/main.sh` & `stepup-1.2.1/tests/cases/static_nglob/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/static_nglob/plan.py` & `stepup-1.2.1/tests/cases/static_nglob/plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python
-from stepup.core.api import glob, copy, step
+from stepup.core.api import copy, glob, step
 
 # This double loop mimics the conversion and concatenation of sections and chapters
 paths_ch = []
 for m_ch in glob("ch-${*ch}-${*name}/", ch="[0-9]", _required=True):
     print(f"Planning ch {m_ch.ch} {m_ch.name}")
     paths_sec = []
     ngm_sec = glob(
```

### Comparing `stepup-1.2.0/tests/cases/static_nglob_partial/expected_graph_01.txt` & `stepup-1.2.1/tests/cases/static_nglob_partial/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/static_nglob_partial/expected_graph_02.txt` & `stepup-1.2.1/tests/cases/static_nglob_partial/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/static_nglob_partial/expected_graph_03.txt` & `stepup-1.2.1/tests/cases/static_nglob_partial/expected_graph_03.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/static_nglob_partial/expected_graph_04.txt` & `stepup-1.2.1/tests/cases/static_nglob_partial/expected_graph_04.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/static_nglob_partial/expected_stdout_a.txt` & `stepup-1.2.1/tests/cases/static_nglob_partial/expected_stdout_a.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/static_nglob_partial/expected_stdout_b.txt` & `stepup-1.2.1/tests/cases/static_nglob_partial/expected_stdout_b.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/static_nglob_partial/main.sh` & `stepup-1.2.1/tests/cases/static_nglob_partial/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/static_nglob_subdir/expected_graph.txt` & `stepup-1.2.1/tests/cases/static_nglob_subdir/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/static_nglob_subdir/main.sh` & `stepup-1.2.1/tests/cases/static_nglob_subdir/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/subdir/expected_graph.txt` & `stepup-1.2.1/tests/cases/subdir/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/subdir/expected_stdout.txt` & `stepup-1.2.1/tests/cases/subdir/expected_stdout.txt`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
    SUCCESS │ ./plan.py  # wd=sub/
      START │ tr '[:lower:]' '[:upper:]' < example.txt > upper.txt  # wd=sub/
    SUCCESS │ tr '[:lower:]' '[:upper:]' < example.txt > upper.txt  # wd=sub/
      START │ cat ../plan.py  # wd=sub/
    SUCCESS │ cat ../plan.py  # wd=sub/
 ─────────────────────────────── Standard output ────────────────────────────────
 #!/usr/bin/env python
-from stepup.core.api import static, plan, copy
+from stepup.core.api import copy, plan, static
 
 static("example.txt")
 static("sub/")
 static("sub/plan.py")
 copy("example.txt", "sub/")
 plan("sub/")
 ────────────────────────────────────────────────────────────────────────────────
```

### Comparing `stepup-1.2.0/tests/cases/subdir/main.sh` & `stepup-1.2.1/tests/cases/subdir/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/watch_blocked/expected_graph_01.txt` & `stepup-1.2.1/tests/cases/watch_blocked/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/watch_blocked/expected_graph_02.txt` & `stepup-1.2.1/tests/cases/watch_blocked/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/watch_blocked/expected_stdout.txt` & `stepup-1.2.1/tests/cases/watch_blocked/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/watch_blocked/main.sh` & `stepup-1.2.1/tests/cases/watch_blocked/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/watch_boot/expected_graph_01.txt` & `stepup-1.2.1/tests/cases/watch_boot/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/watch_boot/expected_graph_02.txt` & `stepup-1.2.1/tests/cases/watch_boot/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/watch_boot/expected_stdout.txt` & `stepup-1.2.1/tests/cases/watch_boot/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/watch_boot/main.sh` & `stepup-1.2.1/tests/cases/watch_boot/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/watch_chain/README.md` & `stepup-1.2.1/tests/cases/watch_chain/README.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/watch_chain/expected_graph_01.txt` & `stepup-1.2.1/tests/cases/watch_chain/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/watch_chain/expected_graph_02.txt` & `stepup-1.2.1/tests/cases/watch_chain/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/watch_chain/expected_stdout.txt` & `stepup-1.2.1/tests/cases/watch_chain/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/watch_chain/main.sh` & `stepup-1.2.1/tests/cases/watch_chain/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/watch_chain/use_config.py` & `stepup-1.2.1/tests/cases/watch_chain/use_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python
 import json
+
 from stepup.core.api import step
 
 # Load configuration
 with open("config.json") as fh:
     config = json.load(fh)
 
 # Write some output file
```

### Comparing `stepup-1.2.0/tests/cases/watch_input/expected_graph_01.txt` & `stepup-1.2.1/tests/cases/watch_input/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/watch_input/expected_graph_02.txt` & `stepup-1.2.1/tests/cases/watch_input/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/watch_input/expected_graph_03.txt` & `stepup-1.2.1/tests/cases/watch_input/expected_graph_03.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/watch_input/expected_stdout.txt` & `stepup-1.2.1/tests/cases/watch_input/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/watch_input/main.sh` & `stepup-1.2.1/tests/cases/watch_input/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/watch_middle/expected_graph_01.txt` & `stepup-1.2.1/tests/cases/watch_middle/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/watch_middle/expected_graph_02.txt` & `stepup-1.2.1/tests/cases/watch_middle/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/watch_middle/expected_graph_03.txt` & `stepup-1.2.1/tests/cases/watch_middle/expected_graph_03.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/watch_middle/expected_stdout.txt` & `stepup-1.2.1/tests/cases/watch_middle/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/watch_middle/main.sh` & `stepup-1.2.1/tests/cases/watch_middle/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/watch_mixed/expected_graph_01.txt` & `stepup-1.2.1/tests/cases/watch_mixed/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/watch_mixed/expected_graph_02.txt` & `stepup-1.2.1/tests/cases/watch_mixed/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/watch_mixed/expected_stdout.txt` & `stepup-1.2.1/tests/cases/watch_mixed/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/watch_mixed/main.sh` & `stepup-1.2.1/tests/cases/watch_mixed/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/watch_nochanges/expected_graph_01.txt` & `stepup-1.2.1/tests/cases/watch_nochanges/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/watch_nochanges/expected_graph_02.txt` & `stepup-1.2.1/tests/cases/watch_nochanges/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/watch_nochanges/main.sh` & `stepup-1.2.1/tests/cases/watch_nochanges/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/watch_outdated_amend1/expected_graph_01.txt` & `stepup-1.2.1/tests/cases/watch_outdated_amend1/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/watch_outdated_amend1/expected_graph_02.txt` & `stepup-1.2.1/tests/cases/watch_outdated_amend1/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/watch_outdated_amend1/expected_stdout.txt` & `stepup-1.2.1/tests/cases/watch_outdated_amend1/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/watch_outdated_amend1/main.sh` & `stepup-1.2.1/tests/cases/watch_outdated_amend1/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/watch_outdated_amend2/expected_graph_01.txt` & `stepup-1.2.1/tests/cases/watch_outdated_amend2/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/watch_outdated_amend2/expected_graph_02.txt` & `stepup-1.2.1/tests/cases/watch_outdated_amend2/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/watch_outdated_amend2/expected_stdout.txt` & `stepup-1.2.1/tests/cases/watch_outdated_amend2/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/watch_outdated_amend2/main.sh` & `stepup-1.2.1/tests/cases/watch_outdated_amend2/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/watch_output/expected_graph_01.txt` & `stepup-1.2.1/tests/cases/watch_output/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/watch_output/expected_graph_02.txt` & `stepup-1.2.1/tests/cases/watch_output/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/watch_output/expected_stdout.txt` & `stepup-1.2.1/tests/cases/watch_output/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/watch_output/main.sh` & `stepup-1.2.1/tests/cases/watch_output/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/watch_wanted/expected_graph_01.txt` & `stepup-1.2.1/tests/cases/watch_wanted/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/watch_wanted/expected_graph_02.txt` & `stepup-1.2.1/tests/cases/watch_wanted/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/watch_wanted/expected_graph_03.txt` & `stepup-1.2.1/tests/cases/watch_wanted/expected_graph_03.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/watch_wanted/expected_stdout.txt` & `stepup-1.2.1/tests/cases/watch_wanted/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/cases/watch_wanted/main.sh` & `stepup-1.2.1/tests/cases/watch_wanted/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/conftest.py` & `stepup-1.2.1/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,27 +15,26 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """Fixtures for testing StepUp."""
 
-
 import asyncio
 import contextlib
 import os
 import stat
 from collections.abc import Iterator
 
-import pytest_asyncio
 import pytest
+import pytest_asyncio
 from path import Path
 
-from stepup.core.reporter import ReporterClient
 from stepup.core.director import serve
+from stepup.core.reporter import ReporterClient
 from stepup.core.rpc import AsyncRPCClient
 
 pytest.register_assert_rewrite("stepup.core.pytest")
 
 BOOT_UNTIL_DONE = """\
 #!/usr/bin/env python
 from path import Path
```

### Comparing `stepup-1.2.0/tests/core_common.py` & `stepup-1.2.1/tests/core_common.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/echo_server_socket.py` & `stepup-1.2.1/tests/echo_server_socket.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -18,18 +18,18 @@
 #
 # --
 """A single echo RPC server over stdio pipes, used by test_rpc.py"""
 
 import asyncio
 import sys
 
-from stepup.core.rpc import serve_socket_rpc
-
 from core_common import EchoHandler
 
+from stepup.core.rpc import serve_socket_rpc
+
 
 async def main():
     handler = EchoHandler("socket")
     await serve_socket_rpc(handler, sys.argv[1], handler.stop_event)
 
 
 if __name__ == "__main__":
```

### Comparing `stepup-1.2.0/tests/echo_server_stdio.py` & `stepup-1.2.1/tests/echo_server_stdio.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,18 +16,19 @@
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """A single echo RPC server over stdio pipes, used by test_rpc.py"""
 
 import asyncio
-from stepup.core.rpc import serve_stdio_rpc
 
 from core_common import EchoHandler
 
+from stepup.core.rpc import serve_stdio_rpc
+
 
 async def main():
     handler = EchoHandler("stdio")
     await serve_stdio_rpc(handler)
 
 
 if __name__ == "__main__":
```

### Comparing `stepup-1.2.0/tests/test_assoc.py` & `stepup-1.2.1/tests/test_assoc.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 # --
 """Unit tests for stepup.core.assoc."""
 
 import pytest
 
 from stepup.core.assoc import Assoc
 
-
 MAX_CASES = [(None, None), (1, 2), (2, 1), (2, None), (None, 2), (1, None), (None, 1)]
 MAX_CASES_SRC_MULTI = [case for case in MAX_CASES if case[1] != 1]
 MAX_CASES_DST_MULTI = [case for case in MAX_CASES if case[0] != 1]
 MAX_CASES_MULTI = [case for case in MAX_CASES if case[0] != 1 and case[1] != 1]
 
 
 @pytest.mark.parametrize("dst_max, src_max", MAX_CASES)
```

### Comparing `stepup-1.2.0/tests/test_basics.py` & `stepup-1.2.1/tests/test_basics.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 """Test a few StepUp basic scenarios."""
 
 import re
 
 import pytest
 from path import Path
 
-from stepup.core.rpc import AsyncRPCClient
 from stepup.core.exceptions import RPCError
+from stepup.core.rpc import AsyncRPCClient
 
 
 @pytest.mark.asyncio
 async def test_unknown_instruction(client: AsyncRPCClient):
     with open("DONE.txt", "w") as fh:
         fh.write("done")
     with pytest.raises(RPCError):
```

### Comparing `stepup-1.2.0/tests/test_cascade.py` & `stepup-1.2.1/tests/test_cascade.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.0/tests/test_cases.py` & `stepup-1.2.1/tests/test_cases.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 import os
 
 import pytest
 from path import Path
 
 from stepup.core.pytest import run_example
 
-
 OVERWRITE_EXPECTED = "STEPUP_OVERWRITE_EXPECTED" in os.environ
 
 
 @pytest.mark.parametrize(
     "name",
     [
         "amend",
```

### Comparing `stepup-1.2.0/tests/test_hash.py` & `stepup-1.2.1/tests/test_hash.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """Unit tests for stepup.core.hash"""
 
 import msgpack
-
 import pytest
 
 from stepup.core.hash import FileHash
 
 
 def test_new():
     file_hash = FileHash.unknown()
```

### Comparing `stepup-1.2.0/tests/test_nglob.py` & `stepup-1.2.1/tests/test_nglob.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,33 +15,32 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """Unit tests for stepup.core.nglob2"""
 
-
 import contextlib
 import re
-import msgpack
-from typing import Collection
+from collections.abc import Collection
 
+import msgpack
 import pytest
 from path import Path
 
 from stepup.core.nglob import (
     RE_NAMED_WILD,
-    NGlobSingle,
+    NGlobMatch,
     NGlobMulti,
-    has_wildcards,
-    has_anonymous_wildcards,
-    iter_wildcard_names,
+    NGlobSingle,
     convert_nglob_to_glob,
     convert_nglob_to_regex,
-    NGlobMatch,
+    has_anonymous_wildcards,
+    has_wildcards,
+    iter_wildcard_names,
 )
 from stepup.core.utils import lookupdict
 
 
 @pytest.mark.parametrize(
     "pattern", ["bar_${*foo}", "foo*", "*", "?", "**", "ls/ff**f/", "num[0-9]"]
 )
```

### Comparing `stepup-1.2.0/tests/test_rpc.py` & `stepup-1.2.1/tests/test_rpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,21 +20,20 @@
 """Unit tests for stepup.core.rpc"""
 
 import asyncio
 import sys
 
 import pytest
 import pytest_asyncio
+from core_common import EchoHandler
 from path import Path
 
 from stepup.core.asyncio import pipe
 from stepup.core.exceptions import RPCError
-from stepup.core.rpc import serve_rpc, fmt_rpc_call, AsyncRPCClient, SocketSyncRPCClient
-
-from core_common import EchoHandler
+from stepup.core.rpc import AsyncRPCClient, SocketSyncRPCClient, fmt_rpc_call, serve_rpc
 
 
 @pytest_asyncio.fixture()
 async def pc():
     async with asyncio.timeout(5):
         handler = EchoHandler("pipe")
         sr, cw = await pipe()
```

### Comparing `stepup-1.2.0/tests/test_scheduler.py` & `stepup-1.2.1/tests/test_scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,20 +14,21 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """Unit tests for stepup.core.scheduler."""
+
 import asyncio
 
 import pytest
 
+from stepup.core.job import RunJob, TryReplayJob
 from stepup.core.scheduler import Pool, Scheduler
-from stepup.core.job import TryReplayJob, RunJob
 
 
 def test_pool_basics():
     pool = Pool(2)
     assert pool.used == 0
     assert pool.size == 2
     assert pool.available
@@ -50,18 +51,15 @@
     assert pool.size == 2
     assert pool.available
     with pytest.raises(ValueError):
         pool.release()
 
 
 def queue_job(scheduler: Scheduler, step_key: str, pool: str | None, try_replay: bool):
-    if try_replay:
-        job = TryReplayJob(step_key, pool)
-    else:
-        job = RunJob(step_key, pool)
+    job = TryReplayJob(step_key, pool) if try_replay else RunJob(step_key, pool)
     scheduler.inqueue.put_nowait(job)
     scheduler.changed.set()
 
 
 def test_scheduler_basics_without_pools():
     scheduler = Scheduler(asyncio.Queue(), asyncio.Event())
     assert scheduler.num_workers == 1
```

### Comparing `stepup-1.2.0/tests/test_utils.py` & `stepup-1.2.1/tests/test_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,25 +15,24 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """Tests for stepup.core.utils."""
 
-
 import pytest
 from path import Path
 
 from stepup.core.utils import (
-    myrelpath,
+    load_module_file,
+    make_path_out,
+    myabsolute,
     mynormpath,
     myparent,
-    myabsolute,
-    make_path_out,
-    load_module_file,
+    myrelpath,
 )
 
 
 @pytest.mark.parametrize(
     "inp, out",
     [
         ("./foo", "foo"),
```

### Comparing `stepup-1.2.0/tests/test_workflow.py` & `stepup-1.2.1/tests/test_workflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,27 +20,26 @@
 """Unit tests for stepup.core.workflow."""
 
 from collections import Counter
 from typing import cast
 
 import pytest
 from path import Path
+from test_cascade import check_cascade_unstructure
 
 from stepup.core.deferred_glob import DeferredGlob
 from stepup.core.exceptions import GraphError
 from stepup.core.file import File, FileState
 from stepup.core.hash import FileHash, StepHash
-from stepup.core.job import TryReplayJob, RunJob, ValidateAmendedJob
+from stepup.core.job import RunJob, TryReplayJob, ValidateAmendedJob
 from stepup.core.nglob import NGlobMulti
 from stepup.core.pytest import remove_hashes
-from stepup.core.step import Step, StepState, StepRecording, Mandatory
+from stepup.core.step import Mandatory, Step, StepRecording, StepState
 from stepup.core.workflow import Workflow
 
-from test_cascade import check_cascade_unstructure
-
 
 def check_workflow_unstructure(workflow: Workflow) -> Workflow:
     workflow = cast(Workflow, check_cascade_unstructure(workflow))
     for step in workflow.get_steps():
         if step.get_state(workflow) == StepState.SUCCEEDED:
             assert step._hash is not None
             assert step._recording is not None
```

