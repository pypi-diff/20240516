# Comparing `tmp/cwltool-3.1.20240404144621.tar.gz` & `tmp/cwltool-3.1.20240508115724.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cwltool-3.1.20240404144621.tar", last modified: Wed Apr 10 13:22:11 2024, max compression
+gzip compressed data, was "cwltool-3.1.20240508115724.tar", last modified: Thu May 16 12:40:46 2024, max compression
```

## Comparing `cwltool-3.1.20240404144621.tar` & `cwltool-3.1.20240508115724.tar`

### file list

```diff
@@ -1,1068 +1,1068 @@
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.640125 cwltool-3.1.20240404144621/
--rw-r--r--   0 michael   (1000) michael   (1000)       40 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/.codecov.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      257 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/.coveragerc
--rw-r--r--   0 michael   (1000) michael   (1000)      290 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/.dockerignore
--rw-r--r--   0 michael   (1000) michael   (1000)      224 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/.flake8
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/.git-blame-ignore-revs
--rw-r--r--   0 michael   (1000) michael   (1000)       31 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/.gitattributes
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.524123 cwltool-3.1.20240404144621/.github/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.524123 cwltool-3.1.20240404144621/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 michael   (1000) michael   (1000)      143 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     1257 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 michael   (1000) michael   (1000)      643 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/.github/dependabot.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.528123 cwltool-3.1.20240404144621/.github/workflows/
--rw-r--r--   0 michael   (1000) michael   (1000)     9031 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/.github/workflows/ci-tests.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      699 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2030 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/.github/workflows/quay-publish.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      593 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/.gitignore
--rw-r--r--   0 michael   (1000) michael   (1000)      734 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/.mergify.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      512 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/.readthedocs.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      385 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/.snyk
--rw-r--r--   0 michael   (1000) michael   (1000)     5435 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/CODE_OF_CONDUCT.md
--rw-r--r--   0 michael   (1000) michael   (1000)     4343 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/CONTRIBUTING.md
--rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/LICENSE.txt
--rw-r--r--   0 michael   (1000) michael   (1000)     3181 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/MANIFEST.in
--rw-r--r--   0 michael   (1000) michael   (1000)     7313 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/Makefile
--rw-r--r--   0 michael   (1000) michael   (1000)    40543 2024-04-10 13:22:11.640125 cwltool-3.1.20240404144621/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)    38143 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/README.rst
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1084 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/build-cwltool-docker.sh
--rwxr-xr-x   0 michael   (1000) michael   (1000)     6535 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/conformance-test.sh
--rwxr-xr-x   0 michael   (1000) michael   (1000)      280 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwl-docker.sh
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.528123 cwltool-3.1.20240404144621/cwlref-runner/
--rw-r--r--   0 michael   (1000) michael   (1000)      223 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwlref-runner/README
--rw-r--r--   0 michael   (1000) michael   (1000)      771 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwlref-runner/setup.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.532123 cwltool-3.1.20240404144621/cwltool/
--rw-r--r--   0 michael   (1000) michael   (1000)      280 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)       81 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/__main__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      437 2024-04-10 13:22:11.000000 cwltool-3.1.20240404144621/cwltool/_version.py
--rw-r--r--   0 michael   (1000) michael   (1000)    30804 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/argparser.py
--rw-r--r--   0 michael   (1000) michael   (1000)    29616 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/builder.py
--rw-r--r--   0 michael   (1000) michael   (1000)    21296 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/checker.py
--rw-r--r--   0 michael   (1000) michael   (1000)    66095 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/command_line_tool.py
--rw-r--r--   0 michael   (1000) michael   (1000)     9184 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/context.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2341 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/cuda.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.536123 cwltool-3.1.20240404144621/cwltool/cwlprov/
--rw-r--r--   0 michael   (1000) michael   (1000)     5140 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/cwlprov/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1887 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/cwlprov/provenance_constants.py
--rw-r--r--   0 michael   (1000) michael   (1000)    32949 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/cwlprov/provenance_profile.py
--rw-r--r--   0 michael   (1000) michael   (1000)    23846 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/cwlprov/ro.py
--rw-r--r--   0 michael   (1000) michael   (1000)    10899 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/cwlprov/writablebagfile.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6398 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/cwlrdf.py
--rw-r--r--   0 michael   (1000) michael   (1000)     7318 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/cwlviewer.py
--rw-r--r--   0 michael   (1000) michael   (1000)    18656 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/docker.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4283 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/docker_id.py
--rw-r--r--   0 michael   (1000) michael   (1000)      927 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/env_to_stdout.py
--rw-r--r--   0 michael   (1000) michael   (1000)      346 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/errors.py
--rw-r--r--   0 michael   (1000) michael   (1000)    20003 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/executors.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4161 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/extensions-v1.1.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     8565 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/extensions-v1.2.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     7404 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/extensions.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2402 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/factory.py
--rw-r--r--   0 michael   (1000) michael   (1000)      704 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/flatten.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     4127 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/hello.simg
--rw-r--r--   0 michael   (1000) michael   (1000)    40577 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/job.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.536123 cwltool-3.1.20240404144621/cwltool/jshint/
--rwxr-xr-x   0 michael   (1000) michael   (1000)  1286196 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/jshint/jshint.js
--rw-r--r--   0 michael   (1000) michael   (1000)     1240 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/jshint/jshint_wrapper.js
--rw-r--r--   0 michael   (1000) michael   (1000)    24252 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/load_tool.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1612 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/loghandler.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    54334 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/main.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2613 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/mpi.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3221 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/mutation.py
--rw-r--r--   0 michael   (1000) michael   (1000)    11058 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/pack.py
--rw-r--r--   0 michael   (1000) michael   (1000)     8975 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/pathmapper.py
--rw-r--r--   0 michael   (1000) michael   (1000)    51808 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/process.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4655 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/procgenerator.py
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/py.typed
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.536123 cwltool-3.1.20240404144621/cwltool/rdfqueries/
--rw-r--r--   0 michael   (1000) michael   (1000)     2722 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/rdfqueries/get_inner_edges.sparql
--rw-r--r--   0 michael   (1000) michael   (1000)     2149 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/rdfqueries/get_input_edges.sparql
--rw-r--r--   0 michael   (1000) michael   (1000)     2134 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/rdfqueries/get_output_edges.sparql
--rw-r--r--   0 michael   (1000) michael   (1000)     2146 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/rdfqueries/get_root.sparql
--rw-r--r--   0 michael   (1000) michael   (1000)     3507 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/resolver.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3680 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/run_job.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.536123 cwltool-3.1.20240404144621/cwltool/schemas/
--rw-r--r--   0 michael   (1000) michael   (1000)     1141 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/CITATION
--rw-r--r--   0 michael   (1000) michael   (1000)     5435 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/CODE_OF_CONDUCT.md
--rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/LICENSE.txt
--rw-r--r--   0 michael   (1000) michael   (1000)    20024 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/README.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.536123 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/
--rw-r--r--   0 michael   (1000) michael   (1000)       53 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/CommandLineTool-standalone.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    35108 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/CommandLineTool.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      209 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/CommonWorkflowLanguage.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    33209 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/Process.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      856 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)       83 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/UserGuide.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    21941 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/Workflow.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    18072 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/concepts.md
--rw-r--r--   0 michael   (1000) michael   (1000)    42373 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/conformance_test_v1.0.yaml
--rw-r--r--   0 michael   (1000) michael   (1000)      985 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/contrib.md
--rw-r--r--   0 michael   (1000) michael   (1000)      884 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/intro.md
--rw-r--r--   0 michael   (1000) michael   (1000)     7889 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/invocation.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.540123 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/
--rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/LICENSE.txt
--rw-r--r--   0 michael   (1000) michael   (1000)     3781 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/README.rst
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.516123 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.540123 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/
--rw-r--r--   0 michael   (1000) michael   (1000)     1328 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/field_name.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/field_name_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      257 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/field_name_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/field_name_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     1692 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/ident_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      370 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/ident_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      235 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/ident_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      338 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/ident_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     4595 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/import_include.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1806 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/link_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      411 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/link_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      264 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/link_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      313 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/link_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      933 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      182 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       89 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    10104 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/metaschema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     3696 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/metaschema_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    10837 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/salad.md
--rw-r--r--   0 michael   (1000) michael   (1000)      765 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/typedsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      394 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/typedsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/typedsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      111 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/typedsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      787 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/vocab_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/vocab_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/vocab_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/vocab_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      193 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/userguide-intro.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.544123 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/
--rw-r--r--   0 michael   (1000) michael   (1000)     1141 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/CITATION
--rw-r--r--   0 michael   (1000) michael   (1000)     5435 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 michael   (1000) michael   (1000)      904 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/CONFORMANCE_TESTS.md
--rw-r--r--   0 michael   (1000) michael   (1000)       54 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/CommandLineTool-standalone.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    47777 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/CommandLineTool.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      228 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/CommonWorkflowLanguage.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/LICENSE.txt
--rw-r--r--   0 michael   (1000) michael   (1000)    36571 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/Process.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      416 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)    25923 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/Workflow.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    24688 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/concepts.md
--rw-r--r--   0 michael   (1000) michael   (1000)    93742 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/conformance_tests.yaml
--rw-r--r--   0 michael   (1000) michael   (1000)      769 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/contrib.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1349 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/cwl-runner.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     2402 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/index.md
--rw-r--r--   0 michael   (1000) michael   (1000)      891 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/intro.md
--rw-r--r--   0 michael   (1000) michael   (1000)     8140 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/invocation.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.548123 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/
--rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/LICENSE.txt
--rw-r--r--   0 michael   (1000) michael   (1000)     4197 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/README.rst
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.516123 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.552124 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/
--rw-r--r--   0 michael   (1000) michael   (1000)     1328 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/field_name.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/field_name_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      257 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/field_name_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/field_name_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     1692 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/ident_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      370 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/ident_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      235 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/ident_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      338 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/ident_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     4595 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/import_include.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1806 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/link_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      411 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/link_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      264 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/link_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      313 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/link_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      933 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      182 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       89 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    10277 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/metaschema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     3799 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/metaschema_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    10837 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/salad.md
--rw-r--r--   0 michael   (1000) michael   (1000)      765 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/typedsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      394 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/typedsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/typedsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      111 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/typedsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      787 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/vocab_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/vocab_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/vocab_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/vocab_res_src.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.544123 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/
--rw-r--r--   0 michael   (1000) michael   (1000)       53 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/CommandLineTool-standalone.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    47285 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/CommandLineTool.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      228 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/CommonWorkflowLanguage.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    36569 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/Process.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      423 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)    25411 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/Workflow.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    24564 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/concepts.md
--rw-r--r--   0 michael   (1000) michael   (1000)      769 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/contrib.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1356 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/cwl-runner.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      891 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/intro.md
--rw-r--r--   0 michael   (1000) michael   (1000)     8140 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/invocation.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.544123 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/
--rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/LICENSE.txt
--rw-r--r--   0 michael   (1000) michael   (1000)     4197 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/README.rst
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.516123 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.548123 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/
--rw-r--r--   0 michael   (1000) michael   (1000)     1328 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/field_name.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/field_name_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      257 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/field_name_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/field_name_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     1692 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/ident_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      370 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/ident_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      235 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/ident_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      338 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/ident_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     4595 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/import_include.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1806 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/link_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      411 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/link_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      264 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/link_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      313 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/link_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      933 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      182 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       89 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    10277 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/metaschema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     3799 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/metaschema_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    10837 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/salad.md
--rw-r--r--   0 michael   (1000) michael   (1000)      765 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/typedsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      394 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/typedsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/typedsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      111 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/typedsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      787 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/vocab_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/vocab_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/vocab_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/vocab_res_src.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.552124 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/
--rw-r--r--   0 michael   (1000) michael   (1000)     5435 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1004 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/CONFORMANCE_TESTS.md
--rw-r--r--   0 michael   (1000) michael   (1000)       54 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/CommandLineTool-standalone.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    51493 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/CommandLineTool.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      228 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/CommonWorkflowLanguage.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2348 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/Operation.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    40072 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/Process.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      290 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)    29004 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/Workflow.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    29634 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/concepts.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1746 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/contrib.md
--rw-r--r--   0 michael   (1000) michael   (1000)     2459 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/index.md
--rw-r--r--   0 michael   (1000) michael   (1000)      821 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/intro.md
--rw-r--r--   0 michael   (1000) michael   (1000)     8260 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/invocation.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.516123 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.516123 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.584124 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/
--rw-r--r--   0 michael   (1000) michael   (1000)     1328 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/field_name.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/field_name_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      257 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/field_name_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/field_name_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2439 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/ident_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      493 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/ident_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      447 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/ident_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      437 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/ident_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2915 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/import_include.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1806 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/link_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      411 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/link_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      264 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/link_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      313 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/link_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      933 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      182 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       89 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12584 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/metaschema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     3799 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/metaschema_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12990 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/salad.md
--rw-r--r--   0 michael   (1000) michael   (1000)      893 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/sfdsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      367 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/sfdsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      289 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/sfdsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      188 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/sfdsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      831 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/typedsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      394 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/typedsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/typedsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      111 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/typedsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      865 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/vocab_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/vocab_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/vocab_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/vocab_res_src.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.556124 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/
--rw-r--r--   0 michael   (1000) michael   (1000)       54 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/CommandLineTool-standalone.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    43403 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/CommandLineTool.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      228 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/CommonWorkflowLanguage.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    36600 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/Process.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      293 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)    26814 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/Workflow.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    25563 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/concepts.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1692 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/contrib.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1356 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/cwl-runner.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      960 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/intro.md
--rw-r--r--   0 michael   (1000) michael   (1000)     8260 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/invocation.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.556124 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/
--rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/LICENSE.txt
--rw-r--r--   0 michael   (1000) michael   (1000)     4197 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/README.rst
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.516123 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.560124 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/
--rw-r--r--   0 michael   (1000) michael   (1000)     1328 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/field_name.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/field_name_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      257 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/field_name_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/field_name_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2439 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/ident_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      493 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/ident_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      447 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/ident_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      437 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/ident_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2915 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/import_include.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1806 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/link_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      411 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/link_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      264 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/link_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      313 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/link_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      933 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/map_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      182 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/map_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/map_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       89 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/map_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12584 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/metaschema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     3799 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/metaschema_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12977 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/salad.md
--rw-r--r--   0 michael   (1000) michael   (1000)      882 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/sfdsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      367 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/sfdsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      289 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/sfdsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      188 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/sfdsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      831 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/typedsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      394 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/typedsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/typedsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      111 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/typedsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      865 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/vocab_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/vocab_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/vocab_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/vocab_res_src.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.560124 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/
--rw-r--r--   0 michael   (1000) michael   (1000)       54 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/CommandLineTool-standalone.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    45433 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/CommandLineTool.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      228 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/CommonWorkflowLanguage.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2348 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/Operation.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    38245 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/Process.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      293 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)    27116 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/Workflow.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    25563 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/concepts.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1688 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/contrib.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1356 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/cwl-runner.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      960 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/intro.md
--rw-r--r--   0 michael   (1000) michael   (1000)     8260 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/invocation.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.560124 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/
--rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/LICENSE.txt
--rw-r--r--   0 michael   (1000) michael   (1000)     4197 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/README.rst
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.516123 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.564124 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/
--rw-r--r--   0 michael   (1000) michael   (1000)     1328 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/field_name.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/field_name_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      257 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/field_name_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/field_name_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2439 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/ident_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      493 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/ident_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      447 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/ident_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      437 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/ident_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2915 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/import_include.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1806 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/link_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      411 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/link_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      264 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/link_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      313 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/link_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      933 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      182 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       89 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12584 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/metaschema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     3799 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/metaschema_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12990 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/salad.md
--rw-r--r--   0 michael   (1000) michael   (1000)      893 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/sfdsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      367 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/sfdsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      289 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/sfdsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      188 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/sfdsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      831 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/typedsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      394 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/typedsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/typedsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      111 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/typedsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      865 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/vocab_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/vocab_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/vocab_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/vocab_res_src.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.564124 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/
--rw-r--r--   0 michael   (1000) michael   (1000)       54 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/CommandLineTool-standalone.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    45578 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/CommandLineTool.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      228 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/CommonWorkflowLanguage.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2348 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/Operation.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    39141 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/Process.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)    27124 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/Workflow.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    25563 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/concepts.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1688 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/contrib.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1356 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/cwl-runner.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     2466 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/index.md
--rw-r--r--   0 michael   (1000) michael   (1000)      960 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/intro.md
--rw-r--r--   0 michael   (1000) michael   (1000)     8260 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/invocation.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.564124 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/
--rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/LICENSE.txt
--rw-r--r--   0 michael   (1000) michael   (1000)     4197 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/README.rst
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.516123 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.568124 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/
--rw-r--r--   0 michael   (1000) michael   (1000)     1328 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/field_name.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/field_name_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      257 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/field_name_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/field_name_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2439 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/ident_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      493 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/ident_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      447 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/ident_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      437 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/ident_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2915 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/import_include.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1806 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/link_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      411 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/link_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      264 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/link_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      313 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/link_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      933 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      182 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       89 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12584 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/metaschema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     3799 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/metaschema_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12990 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/salad.md
--rw-r--r--   0 michael   (1000) michael   (1000)      893 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/sfdsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      367 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/sfdsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      289 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/sfdsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      188 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/sfdsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      831 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/typedsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      394 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/typedsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/typedsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      111 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/typedsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      865 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/vocab_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/vocab_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/vocab_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/vocab_res_src.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.572124 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/
--rw-r--r--   0 michael   (1000) michael   (1000)     1141 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/CITATION
--rw-r--r--   0 michael   (1000) michael   (1000)     5435 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/CODE_OF_CONDUCT.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1004 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/CONFORMANCE_TESTS.md
--rw-r--r--   0 michael   (1000) michael   (1000)       54 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/CommandLineTool-standalone.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    51543 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/CommandLineTool.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      228 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/CommonWorkflowLanguage.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/LICENSE.txt
--rw-r--r--   0 michael   (1000) michael   (1000)     2348 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/Operation.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    40042 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/Process.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)    29054 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/Workflow.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    26611 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/concepts.md
--rw-r--r--   0 michael   (1000) michael   (1000)    95333 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/conformance_tests.yaml
--rw-r--r--   0 michael   (1000) michael   (1000)     1245 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/contrib.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1356 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/cwl-runner.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     2466 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/index.md
--rw-r--r--   0 michael   (1000) michael   (1000)      960 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/intro.md
--rw-r--r--   0 michael   (1000) michael   (1000)     8260 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/invocation.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.572124 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/
--rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/LICENSE.txt
--rw-r--r--   0 michael   (1000) michael   (1000)     4197 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/README.rst
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.516123 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.576124 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/
--rw-r--r--   0 michael   (1000) michael   (1000)     1328 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/field_name.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/field_name_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      257 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/field_name_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/field_name_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2439 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/ident_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      493 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/ident_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      447 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/ident_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      437 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/ident_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2915 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/import_include.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1806 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/link_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      411 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/link_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      264 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/link_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      313 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/link_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      933 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      182 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       89 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12584 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/metaschema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     3799 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/metaschema_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12990 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/salad.md
--rw-r--r--   0 michael   (1000) michael   (1000)      893 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/sfdsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      367 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/sfdsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      289 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/sfdsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      188 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/sfdsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      831 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/typedsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      394 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/typedsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/typedsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      111 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/typedsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      865 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/vocab_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/vocab_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/vocab_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/vocab_res_src.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.576124 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/
--rw-r--r--   0 michael   (1000) michael   (1000)     1141 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/CITATION
--rw-r--r--   0 michael   (1000) michael   (1000)     5435 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/CODE_OF_CONDUCT.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1004 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/CONFORMANCE_TESTS.md
--rw-r--r--   0 michael   (1000) michael   (1000)       54 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/CommandLineTool-standalone.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    51543 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/CommandLineTool.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      228 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/CommonWorkflowLanguage.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/LICENSE.txt
--rw-r--r--   0 michael   (1000) michael   (1000)     2348 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/Operation.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    40064 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/Process.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)    29054 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/Workflow.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    29634 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/concepts.md
--rw-r--r--   0 michael   (1000) michael   (1000)    96242 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/conformance_tests.yaml
--rw-r--r--   0 michael   (1000) michael   (1000)     1737 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/contrib.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1356 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/cwl-runner.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     2466 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/index.md
--rw-r--r--   0 michael   (1000) michael   (1000)      821 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/intro.md
--rw-r--r--   0 michael   (1000) michael   (1000)     8260 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/invocation.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.576124 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/
--rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/LICENSE.txt
--rw-r--r--   0 michael   (1000) michael   (1000)     4197 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/README.rst
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.516123 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.580124 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/
--rw-r--r--   0 michael   (1000) michael   (1000)     1328 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/field_name.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/field_name_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      257 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/field_name_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/field_name_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2439 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/ident_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      493 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/ident_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      447 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/ident_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      437 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/ident_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2915 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/import_include.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1806 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/link_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      411 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/link_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      264 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/link_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      313 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/link_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      933 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      182 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       89 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12584 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/metaschema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     3799 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/metaschema_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12990 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/salad.md
--rw-r--r--   0 michael   (1000) michael   (1000)      893 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/sfdsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      367 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/sfdsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      289 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/sfdsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      188 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/sfdsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      831 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/typedsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      394 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/typedsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/typedsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      111 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/typedsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      865 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/vocab_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/vocab_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/vocab_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/vocab_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2376 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/secrets.py
--rw-r--r--   0 michael   (1000) michael   (1000)    22137 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/singularity.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1094 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/singularity_utils.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6506 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/software_requirements.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1775 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/stdfsaccess.py
--rw-r--r--   0 michael   (1000) michael   (1000)     9751 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/subgraph.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3695 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/task_queue.py
--rw-r--r--   0 michael   (1000) michael   (1000)      614 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/udocker.py
--rw-r--r--   0 michael   (1000) michael   (1000)    11158 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/update.py
--rw-r--r--   0 michael   (1000) michael   (1000)    15913 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/utils.py
--rw-r--r--   0 michael   (1000) michael   (1000)     8506 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/validate_js.py
--rw-r--r--   0 michael   (1000) michael   (1000)    19161 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/workflow.py
--rw-r--r--   0 michael   (1000) michael   (1000)    41287 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/workflow_job.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)      613 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool-in-docker.sh
--rw-r--r--   0 michael   (1000) michael   (1000)     1366 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool.Dockerfile
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.640125 cwltool-3.1.20240404144621/cwltool.egg-info/
--rw-r--r--   0 michael   (1000) michael   (1000)    40543 2024-04-10 13:22:11.000000 cwltool-3.1.20240404144621/cwltool.egg-info/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)    41948 2024-04-10 13:22:11.000000 cwltool-3.1.20240404144621/cwltool.egg-info/SOURCES.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2024-04-10 13:22:11.000000 cwltool-3.1.20240404144621/cwltool.egg-info/dependency_links.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       45 2024-04-10 13:22:11.000000 cwltool-3.1.20240404144621/cwltool.egg-info/entry_points.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      412 2024-04-10 13:22:11.000000 cwltool-3.1.20240404144621/cwltool.egg-info/requires.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        8 2024-04-10 13:22:11.000000 cwltool-3.1.20240404144621/cwltool.egg-info/top_level.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2024-04-10 13:21:18.000000 cwltool-3.1.20240404144621/cwltool.egg-info/zip-safe
--rwxr-xr-x   0 michael   (1000) michael   (1000)      335 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.588124 cwltool-3.1.20240404144621/docs/
--rw-r--r--   0 michael   (1000) michael   (1000)    18134 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/docs/CWLProv.rst
--rw-r--r--   0 michael   (1000) michael   (1000)      634 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/docs/Makefile
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.588124 cwltool-3.1.20240404144621/docs/_static/
--rw-r--r--   0 michael   (1000) michael   (1000)    15086 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/docs/_static/favicon.ico
--rw-r--r--   0 michael   (1000) michael   (1000)      126 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/docs/cli.rst
--rw-r--r--   0 michael   (1000) michael   (1000)     3569 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/docs/conf.py
--rw-r--r--   0 michael   (1000) michael   (1000)      248 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/docs/index.rst
--rw-r--r--   0 michael   (1000) michael   (1000)     6674 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/docs/loop.rst
--rw-r--r--   0 michael   (1000) michael   (1000)      795 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/docs/make.bat
--rw-r--r--   0 michael   (1000) michael   (1000)     7683 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/docs/processgen.rst
--rw-r--r--   0 michael   (1000) michael   (1000)     2510 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/docs/pythonversions.rst
--rw-r--r--   0 michael   (1000) michael   (1000)      145 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/docs/requirements.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       42 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/lint-requirements.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      233 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-requirements.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.588124 cwltool-3.1.20240404144621/mypy-stubs/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.588124 cwltool-3.1.20240404144621/mypy-stubs/arcp/
--rw-r--r--   0 michael   (1000) michael   (1000)      118 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/arcp/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      788 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/arcp/parse.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1736 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/bagit.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.588124 cwltool-3.1.20240404144621/mypy-stubs/black/
--rw-r--r--   0 michael   (1000) michael   (1000)      469 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/black/__init__.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.588124 cwltool-3.1.20240404144621/mypy-stubs/coloredlogs/
--rw-r--r--   0 michael   (1000) michael   (1000)      196 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/coloredlogs/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     7565 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/mistune.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.588124 cwltool-3.1.20240404144621/mypy-stubs/prov/
--rw-r--r--   0 michael   (1000) michael   (1000)      170 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/prov/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     6855 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/prov/constants.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1721 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/prov/dot.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1498 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/prov/graph.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1060 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/prov/identifier.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)    15085 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/prov/model.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.588124 cwltool-3.1.20240404144621/mypy-stubs/prov/serializers/
--rw-r--r--   0 michael   (1000) michael   (1000)     1405 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/prov/serializers/provjson.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      255 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/prov/serializers/provn.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     3009 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/prov/serializers/provrdf.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      767 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/prov/serializers/provxml.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     5310 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/pydot.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.592124 cwltool-3.1.20240404144621/mypy-stubs/rdflib/
--rw-r--r--   0 michael   (1000) michael   (1000)     1292 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      674 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/collection.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     8337 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/graph.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.592124 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/
--rw-r--r--   0 michael   (1000) michael   (1000)     2010 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_CSVW.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      493 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_DC.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1034 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_DCAT.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2361 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_DCTERMS.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1109 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_DOAP.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1847 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_FOAF.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     4691 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_ODRL2.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1259 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_ORG.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2260 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_OWL.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      441 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_PROF.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     4520 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_PROV.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1105 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_QB.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      620 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_RDF.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      519 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_RDFS.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)    41401 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_SDO.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     4965 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_SH.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      943 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_SKOS.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1075 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_SOSA.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      680 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_SSN.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2462 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_TIME.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      927 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_VOID.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1742 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_XSD.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2282 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      131 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/parser.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      724 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/paths.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      325 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/plugin.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.592124 cwltool-3.1.20240404144621/mypy-stubs/rdflib/plugins/
--rw-r--r--   0 michael   (1000) michael   (1000)      118 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/plugins/__init__.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.592124 cwltool-3.1.20240404144621/mypy-stubs/rdflib/plugins/parsers/
--rw-r--r--   0 michael   (1000) michael   (1000)      126 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/plugins/parsers/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)       34 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/plugins/parsers/notation3.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1354 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/query.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1370 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/resource.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1337 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/term.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.592124 cwltool-3.1.20240404144621/mypy-stubs/ruamel/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/ruamel/__init__.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.592124 cwltool-3.1.20240404144621/mypy-stubs/shellescape/
--rw-r--r--   0 michael   (1000) michael   (1000)      147 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/shellescape/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      104 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/shellescape/main.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.520123 cwltool-3.1.20240404144621/mypy-stubs/spython/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.592124 cwltool-3.1.20240404144621/mypy-stubs/spython/main/
--rw-r--r--   0 michael   (1000) michael   (1000)      190 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/spython/main/__init__.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.592124 cwltool-3.1.20240404144621/mypy-stubs/spython/main/base/
--rw-r--r--   0 michael   (1000) michael   (1000)       84 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/spython/main/base/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      732 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/spython/main/build.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.592124 cwltool-3.1.20240404144621/mypy-stubs/spython/main/parse/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.596125 cwltool-3.1.20240404144621/mypy-stubs/spython/main/parse/parsers/
--rw-r--r--   0 michael   (1000) michael   (1000)      363 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/spython/main/parse/parsers/base.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      239 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/spython/main/parse/parsers/docker.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      496 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/spython/main/parse/recipe.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.596125 cwltool-3.1.20240404144621/mypy-stubs/spython/main/parse/writers/
--rw-r--r--   0 michael   (1000) michael   (1000)      236 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/spython/main/parse/writers/base.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      342 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/spython/main/parse/writers/singularity.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      258 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy.ini
--rw-r--r--   0 michael   (1000) michael   (1000)      535 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/pyproject.toml
--rwxr-xr-x   0 michael   (1000) michael   (1000)     3178 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/release-test.sh
--rw-r--r--   0 michael   (1000) michael   (1000)      382 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/requirements.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-04-10 13:22:11.640125 cwltool-3.1.20240404144621/setup.cfg
--rw-r--r--   0 michael   (1000) michael   (1000)     6934 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/setup.py
--rw-r--r--   0 michael   (1000) michael   (1000)      359 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/test-requirements.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.608125 cwltool-3.1.20240404144621/tests/
--rw-r--r--   0 michael   (1000) michael   (1000)      671 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/2.fasta
--rw-r--r--   0 michael   (1000) michael   (1000)      255 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/2.fastq
--rw-r--r--   0 michael   (1000) michael   (1000)       25 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      340 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/arg-empty-prefix-separate-false.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     3735 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/bundle-context.jsonld
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.608125 cwltool-3.1.20240404144621/tests/checker_wf/
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1358 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/checker_wf/broken-wf.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1350 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/checker_wf/broken-wf2.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      776 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/checker_wf/broken-wf3.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      255 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/checker_wf/broken-wf4.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      196 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/checker_wf/cat-a.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      188 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/checker_wf/cat.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      543 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/checker_wf/circ-dep-wf.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      534 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/checker_wf/circ-dep-wf2.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      215 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/checker_wf/echo.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1283 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/checker_wf/functional-wf.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      185 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/checker_wf/ls.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      359 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/checker_wf/optional_array_mismatch.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)        2 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/checker_wf/test.txt
--rwxr-xr-x   0 michael   (1000) michael   (1000)      257 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/checker_wf/wc.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.608125 cwltool-3.1.20240404144621/tests/cwl-conformance/
--rw-r--r--   0 michael   (1000) michael   (1000)     1064 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/cwl-conformance/cwltool-conftest.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)      205 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/debian_image_id.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      215 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/debian_image_id2.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      339 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/default_values_list.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      517 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/echo-badposition-expr.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      105 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/echo-job.yaml
--rw-r--r--   0 michael   (1000) michael   (1000)       14 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/echo-position-expr-job.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/echo-position-expr.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      313 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/echo-stderr.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      178 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/echo-stdout-log-dir.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      297 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/echo.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      167 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/echo_broken_outputs.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      280 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/env.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      285 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/env2.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      145 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/env3.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      360 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/env4.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      157 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/env_with_software_req.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.608125 cwltool-3.1.20240404144621/tests/input_deps/
--rw-r--r--   0 michael   (1000) michael   (1000)      202 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/input_deps/docker-array-secondaryfiles-job.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1081 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/input_deps/docker-array-secondaryfiles.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)    12010 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/input_deps/ref.fasta
--rw-r--r--   0 michael   (1000) michael   (1000)      193 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/input_deps/ref.fasta.fai
--rw-r--r--   0 michael   (1000) michael   (1000)    12010 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/input_deps/ref2.fasta
--rw-r--r--   0 michael   (1000) michael   (1000)      193 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/input_deps/ref2.fasta.fai
--rw-r--r--   0 michael   (1000) michael   (1000)      510 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/iwdr_bad_expr.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      506 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/iwdr_dir_literal_real_file.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       38 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/listing-job.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       38 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/listing2-job.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.612125 cwltool-3.1.20240404144621/tests/loop/
--rw-r--r--   0 michael   (1000) michael   (1000)      590 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/all-output-loop-no-iteration.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      591 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/all-output-loop.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1038 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/default-value-loop.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      558 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/invalid-loop-command-line-tool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      409 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/invalid-loop-expression-tool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      584 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/invalid-loop-hint.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      725 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/invalid-loop-scatter.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      733 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/invalid-loop-when.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      695 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/invalid-loop-workflow.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1518 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/invalid-multi-source-loop-no-requirement.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      669 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/invalid-no-loopWhen.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      700 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/invalid-non-boolean-loopWhen.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      674 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/invalid-value-from-loop-no-requirement.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1311 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/loop-inside-loop-all.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1246 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/loop-inside-loop.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       25 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/loop-inside-scatter-job.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     1076 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/loop-inside-scatter.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1556 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/multi-source-loop.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1052 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/scatter-inside-loop.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)        5 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/single-var-loop-job.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      590 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/single-var-loop-no-iteration.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      591 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/single-var-loop.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      637 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/two-vars-loop-2.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       11 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/two-vars-loop-job.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      691 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/two-vars-loop.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      711 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/value-from-loop.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      175 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/nested-array.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      371 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/non_portable.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      406 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/non_portable2.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.616125 cwltool-3.1.20240404144621/tests/override/
--rw-r--r--   0 michael   (1000) michael   (1000)      125 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/override/echo-job-ov.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      144 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/override/echo-job-ov2.yml
--rw-r--r--   0 michael   (1000) michael   (1000)        8 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/override/echo-job.yml
--rwxr-xr-x   0 michael   (1000) michael   (1000)      211 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/override/echo-wf.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      427 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/override/echo.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      206 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/override/env-tool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      133 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/override/env-tool_cwl-requirement_override.yaml
--rw-r--r--   0 michael   (1000) michael   (1000)      168 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/override/env-tool_cwl-requirement_override_default.yaml
--rw-r--r--   0 michael   (1000) michael   (1000)      187 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/override/env-tool_cwl-requirement_override_default_wrongver.yaml
--rw-r--r--   0 michael   (1000) michael   (1000)      213 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/override/env-tool_v1.1.0-dev1.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      206 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/override/env-tool_v1.1.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      116 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/override/ov.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      127 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/override/ov2.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      119 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/override/ov3.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      413 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/portable.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      530 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/random_lines.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      100 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/random_lines_job.json
--rwxr-xr-x   0 michael   (1000) michael   (1000)      533 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/random_lines_mapping.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.616125 cwltool-3.1.20240404144621/tests/reloc/
--rw-r--r--   0 michael   (1000) michael   (1000)      268 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/reloc/test.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1063 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/scatter_numbers.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      620 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/secondary-files-bad.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       45 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/secondary-files-job.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      336 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/secondary-files-required-container.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      336 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/secondary-files-required-missing-container.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      369 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/secondary-files-string-v1.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      609 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/secondary-files.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      432 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/seqtk_seq.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       69 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/seqtk_seq_job.json
--rwxr-xr-x   0 michael   (1000) michael   (1000)      513 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/seqtk_seq_with_docker.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      539 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/seqtk_seq_wrong_name.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      206 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/sing_pullfolder_test.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.620125 cwltool-3.1.20240404144621/tests/subgraph/
--rw-r--r--   0 michael   (1000) michael   (1000)      469 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/1432.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      946 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/count-lines1-wf.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     4722 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/count-lines17-wf.cwl.json
--rw-r--r--   0 michael   (1000) michael   (1000)       31 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/env-job.json
--rw-r--r--   0 michael   (1000) michael   (1000)      260 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/env-tool2.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      190 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/env-tool2_no_env.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/env-tool2_req.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      298 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/env-wf2.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      291 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/env-wf2_hint_collision.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      295 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/env-wf2_hint_req_collision.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      307 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/env-wf2_long.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      315 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/env-wf2_only_hint.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      302 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/env-wf2_req_collision.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     3679 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/env-wf2_subwf-packed.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      340 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/env-wf2_subwf.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/env-wf2_subwf_b.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1181 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/extract_count_output.json
--rw-r--r--   0 michael   (1000) michael   (1000)     2623 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/extract_file1.json
--rw-r--r--   0 michael   (1000) michael   (1000)      854 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/extract_file2.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1082 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/extract_file3.json
--rw-r--r--   0 michael   (1000) michael   (1000)      854 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/extract_output3.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1232 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/extract_output4.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1082 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/extract_output5.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1788 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/extract_step1.json
--rw-r--r--   0 michael   (1000) michael   (1000)      810 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/extract_step2.json
--rw-r--r--   0 michael   (1000) michael   (1000)      818 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/extract_step2_1432.json
--rw-r--r--   0 michael   (1000) michael   (1000)      854 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/extract_step3.json
--rw-r--r--   0 michael   (1000) michael   (1000)      861 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/extract_step4.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1082 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/extract_step5.json
--rwxr-xr-x   0 michael   (1000) michael   (1000)      279 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/parseInt-tool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1162 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/single_step1.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1189 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/single_step2.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1230 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/single_step3.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1245 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/single_step4.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1584 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/single_step5.json
--rw-r--r--   0 michael   (1000) michael   (1000)      538 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/steplevel-resreq.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      803 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/timelimit2-wf.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      301 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/wc-tool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     5329 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_anon_types.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)      558 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_bad_outputs_wf.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      377 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_check.py
--rw-r--r--   0 michael   (1000) michael   (1000)      563 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_conditionals.py
--rw-r--r--   0 michael   (1000) michael   (1000)      794 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_content_type.py
--rw-r--r--   0 michael   (1000) michael   (1000)      820 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_context.py
--rw-r--r--   0 michael   (1000) michael   (1000)     9278 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_cuda.py
--rw-r--r--   0 michael   (1000) michael   (1000)      369 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_cwl_version.py
--rw-r--r--   0 michael   (1000) michael   (1000)      562 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_default_path.py
--rw-r--r--   0 michael   (1000) michael   (1000)     5684 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_dependencies.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.520123 cwltool-3.1.20240404144621/tests/test_deps_env/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.520123 cwltool-3.1.20240404144621/tests/test_deps_env/modulefiles/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.620125 cwltool-3.1.20240404144621/tests/test_deps_env/modulefiles/random-lines/
--rw-r--r--   0 michael   (1000) michael   (1000)      523 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_deps_env/modulefiles/random-lines/1.0
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.520123 cwltool-3.1.20240404144621/tests/test_deps_env/random-lines/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.620125 cwltool-3.1.20240404144621/tests/test_deps_env/random-lines/1.0/
--rw-r--r--   0 michael   (1000) michael   (1000)      355 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_deps_env/random-lines/1.0/env.sh
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.620125 cwltool-3.1.20240404144621/tests/test_deps_env/random-lines/1.0/scripts/
--rwxr-xr-x   0 michael   (1000) michael   (1000)     2300 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_deps_env/random-lines/1.0/scripts/random-lines
--rw-r--r--   0 michael   (1000) michael   (1000)       55 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_deps_env_modules_resolvers_conf.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       60 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_deps_env_resolvers_conf.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      106 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_deps_env_resolvers_conf_rewrite.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      101 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_deps_mapping.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     8162 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_docker.py
--rw-r--r--   0 michael   (1000) michael   (1000)      414 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_docker_info.py
--rw-r--r--   0 michael   (1000) michael   (1000)      845 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_docker_paths_with_colons.py
--rw-r--r--   0 michael   (1000) michael   (1000)      513 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_empty_input.py
--rw-r--r--   0 michael   (1000) michael   (1000)     8326 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_environment.py
--rw-r--r--   0 michael   (1000) michael   (1000)    64197 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_examples.py
--rw-r--r--   0 michael   (1000) michael   (1000)     7610 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_ext.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2533 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_fetch.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2487 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_http_input.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4335 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_input_deps.py
--rw-r--r--   0 michael   (1000) michael   (1000)    10932 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_iwdr.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4466 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_js_sandbox.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6991 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_load_tool.py
--rw-r--r--   0 michael   (1000) michael   (1000)     9409 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_loop.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1302 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_main_parsed_args.py
--rw-r--r--   0 michael   (1000) michael   (1000)      831 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_make_template.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2761 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_misc_cli.py
--rw-r--r--   0 michael   (1000) michael   (1000)    11905 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_mpi.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3979 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_override.py
--rw-r--r--   0 michael   (1000) michael   (1000)     7708 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_pack.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1126 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_parallel.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6158 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_path_checks.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2682 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_pathmapper.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1382 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_procgenerator.py
--rw-r--r--   0 michael   (1000) michael   (1000)    28315 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_provenance.py
--rw-r--r--   0 michael   (1000) michael   (1000)      589 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_rdfprint.py
--rw-r--r--   0 michael   (1000) michael   (1000)      527 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_recursive_validation.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2010 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_relocate.py
--rw-r--r--   0 michael   (1000) michael   (1000)      319 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_schemadef.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3034 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_secrets.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4597 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_singularity.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4458 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_singularity_versions.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1870 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_stdout_stderr_log_dir.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2726 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_streaming.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2289 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_subclass_mypyc.py
--rw-r--r--   0 michael   (1000) michael   (1000)    11067 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_subgraph.py
--rw-r--r--   0 michael   (1000) michael   (1000)      936 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_target.py
--rw-r--r--   0 michael   (1000) michael   (1000)    11938 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_tmpdir.py
--rw-r--r--   0 michael   (1000) michael   (1000)     5693 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_toolargparse.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4342 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_trs.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3580 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_udocker.py
--rw-r--r--   0 michael   (1000) michael   (1000)      746 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_user_agent.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1882 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_validate.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2170 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_validate_js.py
--rw-r--r--   0 michael   (1000) michael   (1000)      867 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_windows_warning.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.520123 cwltool-3.1.20240404144621/tests/tmp1/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.520123 cwltool-3.1.20240404144621/tests/tmp1/tmp2/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.620125 cwltool-3.1.20240404144621/tests/tmp1/tmp2/tmp3/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/tmp1/tmp2/tmp3/.gitkeep
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.520123 cwltool-3.1.20240404144621/tests/tmp4/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.620125 cwltool-3.1.20240404144621/tests/tmp4/alpha/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/tmp4/alpha/baker
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/tmp4/alpha/charlie
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/tmp4/alpha/delta
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/tmp4/alpha/echo
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/tmp4/alpha/foxtrot
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.620125 cwltool-3.1.20240404144621/tests/trs/
--rw-r--r--   0 michael   (1000) michael   (1000)     1505 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/trs/Dockstore.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      821 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/trs/md5sum-tool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/trs/md5sum-workflow.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      674 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/utf_doc_example.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     5261 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/util.py
--rw-r--r--   0 michael   (1000) michael   (1000)      236 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wc-tool-bad-hints.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wc-tool-bad-reqs.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.640125 cwltool-3.1.20240404144621/tests/wf/
--rw-r--r--   0 michael   (1000) michael   (1000)      286 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/1496.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      468 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/1590.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      373 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/1st-workflow.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       51 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/1st-workflow_bad_inputs.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      181 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/811-12.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      178 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/811.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       26 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/811_inputs.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      212 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/816_tool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      155 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/816_wf.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      650 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/910.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      394 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/arguments.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      254 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/bad-stderr-expr.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      225 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/bad-stdin-expr.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      239 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/bad-stdout-expr.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      523 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/bad_formattest.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      533 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/bad_formattest2.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      222 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/bad_networkaccess.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/bad_timelimit.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      294 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/badout1.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      304 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/badout2.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      299 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/badout3.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      272 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/cache_test_workflow.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      289 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/cat-tool.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      130 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/cat.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      469 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/conditional_step_no_inputs.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      577 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/conflict.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      266 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/cores_float.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      388 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/count-lines1-wf.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      409 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/default-dir5.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/default-wf5.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      212 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/default_path.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      210 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/dir_deps.json
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1479 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/directory.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1420 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/double-nested.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      534 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/echo.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/empty.ttl
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/empty2.ttl
--rw-r--r--   0 michael   (1000) michael   (1000)      922 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/expect_iwd-passthrough1_packed.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     4397 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/expect_packed.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     4564 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/expect_revsort_datetime_packed.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     4574 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/expect_trick_packed.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1262 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/extract_region_specs.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      619 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/floats_small_and_large.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      120 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/formattest-job.json
--rwxr-xr-x   0 michael   (1000) michael   (1000)      412 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/formattest.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.640125 cwltool-3.1.20240404144621/tests/wf/generator/
--rw-r--r--   0 michael   (1000) michael   (1000)      710 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/generator/pytoolgen.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      275 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/generator/zing.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      672 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/hello-workflow-badhints.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      673 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/hello-workflow-badhints2.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      657 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/hello-workflow.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       35 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/hello.txt
--rwxr-xr-x   0 michael   (1000) michael   (1000)      168 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/hello_single_tool.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.640125 cwltool-3.1.20240404144621/tests/wf/indir/
--rw-r--r--   0 michael   (1000) michael   (1000)        7 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/indir/hello2.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      213 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/input_named_id.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       37 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/input_named_id.yaml
--rw-r--r--   0 michael   (1000) michael   (1000)      580 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/iwd-passthrough1.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      230 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/iwdr-empty.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      414 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/iwdr-entry.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1775 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/iwdr-passthrough-successive.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)     2268 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/iwdr_permutations.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      155 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/iwdr_permutations_inplace.yml
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1016 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/iwdr_permutations_nocontainer.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      284 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/js_output.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      364 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/js_output_workflow.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      291 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/listing_deep.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      276 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/listing_none.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      292 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/listing_shallow.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      158 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/listing_v1_0.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       35 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/literalfile-job.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      208 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/literalfile.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      111 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/malformed_outputs.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      145 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/missing-tool.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      548 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/missing_cwlVersion.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      249 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/mpi_env.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      645 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/mpi_expr.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       13 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/mpi_expr.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      401 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/mpi_line_count.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      471 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/mpi_simple.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      640 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/mpi_simple_wf.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      238 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/mut.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      299 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/mut2.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      281 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/mut3.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1107 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/nested.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      362 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/networkaccess-fail.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      425 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/networkaccess.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      233 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/no-parameters-echo.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      445 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/nvidia-smi-cc.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      434 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/nvidia-smi-container.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      382 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/nvidia-smi-max.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      408 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/nvidia-smi-range.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      429 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/nvidia-smi.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.640125 cwltool-3.1.20240404144621/tests/wf/operation/
--rw-r--r--   0 michael   (1000) michael   (1000)      442 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/operation/abstract-cosifer.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     5209 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/operation/expect_operation-single_packed.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      969 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/operation/operation-single.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      337 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/optional-numerical-output-0.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      174 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/optional_src_mandatory_sink.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      221 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/override-no-secrets.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     1921 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/packed-with-loadlisting.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1056 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/packed_no_main.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      786 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/paramref_arguments_roundtrip.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      877 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/paramref_arguments_self.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      279 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/parseInt-tool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      984 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/record_outputeval.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      377 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/resreq_expr_float_v1_0.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      377 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/resreq_expr_float_v1_2.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      181 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/revsort-job-shortcut.json
--rw-r--r--   0 michael   (1000) michael   (1000)      152 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/revsort-job.json
--rwxr-xr-x   0 michael   (1000) michael   (1000)     2331 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/revsort.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)     2447 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/revsort_datetime.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)     2317 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/revsort_step_bad_schema.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1367 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/revtool.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1471 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/revtool_bad_schema.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)       62 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/scatter-job2.json
--rwxr-xr-x   0 michael   (1000) michael   (1000)      927 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/scatter-wf4.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     2999 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/scatter-wf4.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1563 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/scatter2.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1805 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/scatter2_subwf.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      703 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/scatterfail.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)    94112 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/schemadef-bug-1473.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      412 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/schemadef-tool-12.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      412 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/schemadef-tool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      158 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/schemadef-type.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      163 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/sec-tool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      948 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/sec-wf-out.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      214 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/sec-wf.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      403 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/secret_job.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      380 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/secret_wf.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      363 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/separate_without_prefix.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      233 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/shm_size.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1101 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/sorttool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      391 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/storage_float.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      320 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/tar-param.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1124 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/three_step_color.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      222 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/timelimit-fail.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      277 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/timelimit.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      304 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/touch_tool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      278 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/trick_defaults.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      260 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/trick_defaults2.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)     2400 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/trick_revsort.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      318 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/updatedir.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      431 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/updatedir_inplace.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      488 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/updateval.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      102 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/updateval.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)      603 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/updateval_inplace.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      382 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/vf-concat.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       82 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/wc-job.json
--rwxr-xr-x   0 michael   (1000) michael   (1000)      301 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/wc-tool.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      639 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/wffail.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1111 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/whale.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      329 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/workreuse-fail.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      392 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/workreuse.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      565 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/wrong_cwlVersion.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      150 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/with_doc.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      107 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/without_doc.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     2094 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tox.ini
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.101051 cwltool-3.1.20240508115724/
+-rw-r--r--   0 michael   (1000) michael   (1000)       40 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/.codecov.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      257 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/.coveragerc
+-rw-r--r--   0 michael   (1000) michael   (1000)      290 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/.dockerignore
+-rw-r--r--   0 michael   (1000) michael   (1000)      224 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/.flake8
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/.git-blame-ignore-revs
+-rw-r--r--   0 michael   (1000) michael   (1000)       31 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/.gitattributes
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:45.961048 cwltool-3.1.20240508115724/.github/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:45.961048 cwltool-3.1.20240508115724/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 michael   (1000) michael   (1000)      143 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1257 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      643 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/.github/dependabot.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:45.961048 cwltool-3.1.20240508115724/.github/workflows/
+-rw-r--r--   0 michael   (1000) michael   (1000)     9059 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/.github/workflows/ci-tests.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      699 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2030 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/.github/workflows/quay-publish.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      593 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/.gitignore
+-rw-r--r--   0 michael   (1000) michael   (1000)      734 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/.mergify.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      512 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/.readthedocs.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      385 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/.snyk
+-rw-r--r--   0 michael   (1000) michael   (1000)     5435 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/CODE_OF_CONDUCT.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     4343 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/CONTRIBUTING.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/LICENSE.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)     3181 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/MANIFEST.in
+-rw-r--r--   0 michael   (1000) michael   (1000)     7313 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/Makefile
+-rw-r--r--   0 michael   (1000) michael   (1000)    40543 2024-05-16 12:40:46.097051 cwltool-3.1.20240508115724/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)    38143 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/README.rst
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1084 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/build-cwltool-docker.sh
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     6505 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/conformance-test.sh
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      280 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwl-docker.sh
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:45.961048 cwltool-3.1.20240508115724/cwlref-runner/
+-rw-r--r--   0 michael   (1000) michael   (1000)      223 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwlref-runner/README
+-rw-r--r--   0 michael   (1000) michael   (1000)      771 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwlref-runner/setup.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:45.965048 cwltool-3.1.20240508115724/cwltool/
+-rw-r--r--   0 michael   (1000) michael   (1000)      280 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)       81 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/__main__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      437 2024-05-16 12:40:45.000000 cwltool-3.1.20240508115724/cwltool/_version.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    30804 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/argparser.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    29614 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/builder.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    21296 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/checker.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    66093 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/command_line_tool.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     9184 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/context.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2341 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/cuda.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:45.969048 cwltool-3.1.20240508115724/cwltool/cwlprov/
+-rw-r--r--   0 michael   (1000) michael   (1000)     5140 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/cwlprov/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1887 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/cwlprov/provenance_constants.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    32949 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/cwlprov/provenance_profile.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    23846 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/cwlprov/ro.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    10899 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/cwlprov/writablebagfile.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6396 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/cwlrdf.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     7318 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/cwlviewer.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    18630 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/docker.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4283 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/docker_id.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      927 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/env_to_stdout.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      346 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/errors.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    20003 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/executors.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4161 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/extensions-v1.1.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     8565 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/extensions-v1.2.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     7404 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/extensions.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2402 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/factory.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      704 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/flatten.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     4127 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/hello.simg
+-rw-r--r--   0 michael   (1000) michael   (1000)    40577 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/job.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:45.969048 cwltool-3.1.20240508115724/cwltool/jshint/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)  1286196 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/jshint/jshint.js
+-rw-r--r--   0 michael   (1000) michael   (1000)     1240 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/jshint/jshint_wrapper.js
+-rw-r--r--   0 michael   (1000) michael   (1000)    24252 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/load_tool.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1612 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/loghandler.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    54334 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/main.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2613 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/mpi.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3221 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/mutation.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    11058 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/pack.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     8975 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/pathmapper.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    51808 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/process.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4655 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/procgenerator.py
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/py.typed
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:45.969048 cwltool-3.1.20240508115724/cwltool/rdfqueries/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2722 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/rdfqueries/get_inner_edges.sparql
+-rw-r--r--   0 michael   (1000) michael   (1000)     2149 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/rdfqueries/get_input_edges.sparql
+-rw-r--r--   0 michael   (1000) michael   (1000)     2134 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/rdfqueries/get_output_edges.sparql
+-rw-r--r--   0 michael   (1000) michael   (1000)     2146 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/rdfqueries/get_root.sparql
+-rw-r--r--   0 michael   (1000) michael   (1000)     3507 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/resolver.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3680 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/run_job.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:45.969048 cwltool-3.1.20240508115724/cwltool/schemas/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1141 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/CITATION
+-rw-r--r--   0 michael   (1000) michael   (1000)     5435 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/CODE_OF_CONDUCT.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/LICENSE.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)    20024 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/README.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:45.973049 cwltool-3.1.20240508115724/cwltool/schemas/v1.0/
+-rw-r--r--   0 michael   (1000) michael   (1000)       53 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.0/CommandLineTool-standalone.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    35108 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.0/CommandLineTool.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      209 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.0/CommonWorkflowLanguage.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    33209 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.0/Process.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      856 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.0/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)       83 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.0/UserGuide.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    21941 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.0/Workflow.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    18072 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.0/concepts.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    42373 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.0/conformance_test_v1.0.yaml
+-rw-r--r--   0 michael   (1000) michael   (1000)      985 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.0/contrib.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      884 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.0/intro.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     7889 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.0/invocation.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:45.973049 cwltool-3.1.20240508115724/cwltool/schemas/v1.0/salad/
+-rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.0/salad/LICENSE.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)     3781 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.0/salad/README.rst
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:45.953048 cwltool-3.1.20240508115724/cwltool/schemas/v1.0/salad/schema_salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:45.981049 cwltool-3.1.20240508115724/cwltool/schemas/v1.0/salad/schema_salad/metaschema/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1328 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.0/salad/schema_salad/metaschema/field_name.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.0/salad/schema_salad/metaschema/field_name_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      257 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.0/salad/schema_salad/metaschema/field_name_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.0/salad/schema_salad/metaschema/field_name_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1692 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.0/salad/schema_salad/metaschema/ident_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      370 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.0/salad/schema_salad/metaschema/ident_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      235 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.0/salad/schema_salad/metaschema/ident_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      338 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.0/salad/schema_salad/metaschema/ident_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     4595 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.0/salad/schema_salad/metaschema/import_include.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1806 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.0/salad/schema_salad/metaschema/link_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      411 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.0/salad/schema_salad/metaschema/link_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      264 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.0/salad/schema_salad/metaschema/link_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      313 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.0/salad/schema_salad/metaschema/link_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      933 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      182 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       89 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    10104 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.0/salad/schema_salad/metaschema/metaschema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     3696 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.0/salad/schema_salad/metaschema/metaschema_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    10837 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.0/salad/schema_salad/metaschema/salad.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      765 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.0/salad/schema_salad/metaschema/typedsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      394 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.0/salad/schema_salad/metaschema/typedsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.0/salad/schema_salad/metaschema/typedsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      111 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.0/salad/schema_salad/metaschema/typedsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      787 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.0/salad/schema_salad/metaschema/vocab_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.0/salad/schema_salad/metaschema/vocab_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.0/salad/schema_salad/metaschema/vocab_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.0/salad/schema_salad/metaschema/vocab_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      193 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.0/userguide-intro.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:45.985049 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1141 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/CITATION
+-rw-r--r--   0 michael   (1000) michael   (1000)     5435 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      904 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/CONFORMANCE_TESTS.md
+-rw-r--r--   0 michael   (1000) michael   (1000)       54 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/CommandLineTool-standalone.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    47777 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/CommandLineTool.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      228 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/CommonWorkflowLanguage.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/LICENSE.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)    36571 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/Process.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      416 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    25923 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/Workflow.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    24688 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/concepts.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    93742 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/conformance_tests.yaml
+-rw-r--r--   0 michael   (1000) michael   (1000)      769 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/contrib.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1349 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/cwl-runner.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     2402 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/index.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      891 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/intro.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     8140 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/invocation.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:45.993049 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/salad/
+-rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/salad/LICENSE.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)     4197 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/salad/README.rst
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:45.953048 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/salad/schema_salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:45.997049 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/salad/schema_salad/metaschema/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1328 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/salad/schema_salad/metaschema/field_name.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/salad/schema_salad/metaschema/field_name_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      257 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/salad/schema_salad/metaschema/field_name_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/salad/schema_salad/metaschema/field_name_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1692 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/salad/schema_salad/metaschema/ident_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      370 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/salad/schema_salad/metaschema/ident_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      235 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/salad/schema_salad/metaschema/ident_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      338 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/salad/schema_salad/metaschema/ident_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     4595 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/salad/schema_salad/metaschema/import_include.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1806 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/salad/schema_salad/metaschema/link_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      411 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/salad/schema_salad/metaschema/link_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      264 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/salad/schema_salad/metaschema/link_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      313 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/salad/schema_salad/metaschema/link_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      933 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      182 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       89 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    10277 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/salad/schema_salad/metaschema/metaschema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     3799 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/salad/schema_salad/metaschema/metaschema_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    10837 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/salad/schema_salad/metaschema/salad.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      765 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/salad/schema_salad/metaschema/typedsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      394 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/salad/schema_salad/metaschema/typedsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/salad/schema_salad/metaschema/typedsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      111 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/salad/schema_salad/metaschema/typedsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      787 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/salad/schema_salad/metaschema/vocab_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/salad/schema_salad/metaschema/vocab_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/salad/schema_salad/metaschema/vocab_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1/salad/schema_salad/metaschema/vocab_res_src.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:45.989049 cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/
+-rw-r--r--   0 michael   (1000) michael   (1000)       53 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/CommandLineTool-standalone.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    47285 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/CommandLineTool.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      228 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/CommonWorkflowLanguage.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    36569 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/Process.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      423 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    25411 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/Workflow.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    24564 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/concepts.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      769 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/contrib.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1356 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/cwl-runner.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      891 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/intro.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     8140 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/invocation.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:45.989049 cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/salad/
+-rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/salad/LICENSE.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)     4197 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/salad/README.rst
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:45.953048 cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:45.993049 cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1328 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/field_name.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/field_name_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      257 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/field_name_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/field_name_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1692 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/ident_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      370 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/ident_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      235 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/ident_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      338 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/ident_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     4595 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/import_include.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1806 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/link_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      411 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/link_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      264 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/link_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      313 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/link_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      933 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      182 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       89 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    10277 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/metaschema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     3799 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/metaschema_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    10837 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/salad.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      765 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/typedsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      394 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/typedsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/typedsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      111 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/typedsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      787 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/vocab_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/vocab_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/vocab_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/vocab_res_src.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.001049 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/
+-rw-r--r--   0 michael   (1000) michael   (1000)     5435 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1004 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/CONFORMANCE_TESTS.md
+-rw-r--r--   0 michael   (1000) michael   (1000)       54 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/CommandLineTool-standalone.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    51493 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/CommandLineTool.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      228 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/CommonWorkflowLanguage.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2348 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/Operation.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    40072 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/Process.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      290 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    29004 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/Workflow.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    29634 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/concepts.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1746 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/contrib.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     2459 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/index.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      821 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/intro.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     8260 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/invocation.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:45.953048 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:45.953048 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/salad/schema_salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.045050 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/salad/schema_salad/metaschema/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1328 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/salad/schema_salad/metaschema/field_name.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/salad/schema_salad/metaschema/field_name_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      257 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/salad/schema_salad/metaschema/field_name_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/salad/schema_salad/metaschema/field_name_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2439 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/salad/schema_salad/metaschema/ident_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/salad/schema_salad/metaschema/ident_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      447 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/salad/schema_salad/metaschema/ident_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      437 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/salad/schema_salad/metaschema/ident_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2915 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/salad/schema_salad/metaschema/import_include.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1806 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/salad/schema_salad/metaschema/link_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      411 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/salad/schema_salad/metaschema/link_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      264 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/salad/schema_salad/metaschema/link_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      313 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/salad/schema_salad/metaschema/link_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      933 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      182 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       89 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12584 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/salad/schema_salad/metaschema/metaschema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     3799 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/salad/schema_salad/metaschema/metaschema_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12990 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/salad/schema_salad/metaschema/salad.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      893 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/salad/schema_salad/metaschema/sfdsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      367 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/salad/schema_salad/metaschema/sfdsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      289 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/salad/schema_salad/metaschema/sfdsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      188 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/salad/schema_salad/metaschema/sfdsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      831 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/salad/schema_salad/metaschema/typedsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      394 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/salad/schema_salad/metaschema/typedsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/salad/schema_salad/metaschema/typedsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      111 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/salad/schema_salad/metaschema/typedsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      865 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/salad/schema_salad/metaschema/vocab_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/salad/schema_salad/metaschema/vocab_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/salad/schema_salad/metaschema/vocab_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2/salad/schema_salad/metaschema/vocab_res_src.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.005049 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/
+-rw-r--r--   0 michael   (1000) michael   (1000)       54 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/CommandLineTool-standalone.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    43403 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/CommandLineTool.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      228 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/CommonWorkflowLanguage.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    36600 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/Process.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      293 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    26814 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/Workflow.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    25563 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/concepts.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1692 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/contrib.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1356 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/cwl-runner.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      960 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/intro.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     8260 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/invocation.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.005049 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/
+-rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/LICENSE.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)     4197 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/README.rst
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:45.953048 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.009049 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1328 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/field_name.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/field_name_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      257 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/field_name_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/field_name_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2439 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/ident_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/ident_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      447 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/ident_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      437 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/ident_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2915 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/import_include.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1806 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/link_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      411 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/link_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      264 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/link_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      313 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/link_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      933 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/map_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      182 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/map_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/map_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       89 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/map_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12584 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/metaschema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     3799 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/metaschema_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12977 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/salad.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      882 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/sfdsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      367 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/sfdsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      289 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/sfdsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      188 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/sfdsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      831 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/typedsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      394 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/typedsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/typedsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      111 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/typedsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      865 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/vocab_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/vocab_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/vocab_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/vocab_res_src.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.013049 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/
+-rw-r--r--   0 michael   (1000) michael   (1000)       54 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/CommandLineTool-standalone.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    45433 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/CommandLineTool.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      228 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/CommonWorkflowLanguage.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2348 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/Operation.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    38245 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/Process.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      293 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    27116 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/Workflow.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    25563 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/concepts.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1688 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/contrib.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1356 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/cwl-runner.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      960 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/intro.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     8260 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/invocation.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.013049 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/
+-rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/LICENSE.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)     4197 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/README.rst
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:45.953048 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.017049 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1328 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/field_name.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/field_name_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      257 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/field_name_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/field_name_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2439 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/ident_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/ident_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      447 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/ident_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      437 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/ident_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2915 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/import_include.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1806 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/link_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      411 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/link_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      264 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/link_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      313 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/link_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      933 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      182 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       89 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12584 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/metaschema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     3799 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/metaschema_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12990 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/salad.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      893 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/sfdsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      367 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/sfdsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      289 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/sfdsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      188 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/sfdsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      831 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/typedsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      394 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/typedsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/typedsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      111 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/typedsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      865 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/vocab_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/vocab_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/vocab_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/vocab_res_src.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.021049 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/
+-rw-r--r--   0 michael   (1000) michael   (1000)       54 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/CommandLineTool-standalone.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    45578 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/CommandLineTool.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      228 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/CommonWorkflowLanguage.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2348 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/Operation.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    39141 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/Process.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    27124 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/Workflow.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    25563 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/concepts.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1688 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/contrib.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1356 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/cwl-runner.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     2466 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/index.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      960 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/intro.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     8260 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/invocation.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.021049 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/
+-rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/LICENSE.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)     4197 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/README.rst
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:45.953048 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.029049 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1328 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/field_name.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/field_name_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      257 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/field_name_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/field_name_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2439 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/ident_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/ident_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      447 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/ident_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      437 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/ident_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2915 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/import_include.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1806 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/link_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      411 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/link_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      264 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/link_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      313 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/link_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      933 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      182 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       89 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12584 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/metaschema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     3799 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/metaschema_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12990 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/salad.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      893 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/sfdsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      367 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/sfdsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      289 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/sfdsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      188 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/sfdsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      831 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/typedsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      394 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/typedsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/typedsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      111 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/typedsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      865 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/vocab_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/vocab_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/vocab_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/vocab_res_src.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.033050 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1141 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/CITATION
+-rw-r--r--   0 michael   (1000) michael   (1000)     5435 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1004 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/CONFORMANCE_TESTS.md
+-rw-r--r--   0 michael   (1000) michael   (1000)       54 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/CommandLineTool-standalone.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    51543 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/CommandLineTool.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      228 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/CommonWorkflowLanguage.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/LICENSE.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)     2348 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/Operation.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    40042 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/Process.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    29054 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/Workflow.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    26611 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/concepts.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    95333 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/conformance_tests.yaml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1245 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/contrib.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1356 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/cwl-runner.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     2466 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/index.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      960 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/intro.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     8260 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/invocation.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.033050 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/
+-rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/LICENSE.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)     4197 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/README.rst
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:45.953048 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.037050 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1328 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/field_name.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/field_name_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      257 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/field_name_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/field_name_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2439 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/ident_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/ident_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      447 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/ident_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      437 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/ident_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2915 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/import_include.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1806 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/link_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      411 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/link_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      264 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/link_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      313 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/link_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      933 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      182 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       89 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12584 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/metaschema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     3799 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/metaschema_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12990 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/salad.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      893 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/sfdsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      367 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/sfdsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      289 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/sfdsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      188 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/sfdsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      831 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/typedsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      394 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/typedsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/typedsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      111 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/typedsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      865 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/vocab_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/vocab_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/vocab_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/vocab_res_src.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.037050 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1141 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/CITATION
+-rw-r--r--   0 michael   (1000) michael   (1000)     5435 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1004 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/CONFORMANCE_TESTS.md
+-rw-r--r--   0 michael   (1000) michael   (1000)       54 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/CommandLineTool-standalone.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    51543 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/CommandLineTool.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      228 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/CommonWorkflowLanguage.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/LICENSE.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)     2348 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/Operation.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    40064 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/Process.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    29054 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/Workflow.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    29634 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/concepts.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    96242 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/conformance_tests.yaml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1737 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/contrib.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1356 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/cwl-runner.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     2466 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/index.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      821 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/intro.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     8260 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/invocation.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.037050 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/
+-rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/LICENSE.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)     4197 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/README.rst
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:45.953048 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.041050 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1328 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/field_name.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/field_name_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      257 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/field_name_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/field_name_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2439 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/ident_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/ident_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      447 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/ident_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      437 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/ident_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2915 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/import_include.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1806 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/link_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      411 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/link_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      264 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/link_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      313 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/link_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      933 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      182 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       89 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12584 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/metaschema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     3799 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/metaschema_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12990 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/salad.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      893 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/sfdsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      367 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/sfdsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      289 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/sfdsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      188 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/sfdsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      831 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/typedsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      394 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/typedsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/typedsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      111 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/typedsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      865 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/vocab_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/vocab_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/vocab_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/vocab_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2376 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/secrets.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    22137 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/singularity.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1094 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/singularity_utils.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6506 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/software_requirements.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1775 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/stdfsaccess.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     9751 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/subgraph.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3695 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/task_queue.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      614 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/udocker.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    11158 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/update.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    15911 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/utils.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     8506 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/validate_js.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    19161 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/workflow.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    41287 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool/workflow_job.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      613 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool-in-docker.sh
+-rw-r--r--   0 michael   (1000) michael   (1000)     1366 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool.Dockerfile
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.097051 cwltool-3.1.20240508115724/cwltool.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)    40543 2024-05-16 12:40:45.000000 cwltool-3.1.20240508115724/cwltool.egg-info/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)    41948 2024-05-16 12:40:45.000000 cwltool-3.1.20240508115724/cwltool.egg-info/SOURCES.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2024-05-16 12:40:45.000000 cwltool-3.1.20240508115724/cwltool.egg-info/dependency_links.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       45 2024-05-16 12:40:45.000000 cwltool-3.1.20240508115724/cwltool.egg-info/entry_points.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      412 2024-05-16 12:40:45.000000 cwltool-3.1.20240508115724/cwltool.egg-info/requires.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        8 2024-05-16 12:40:45.000000 cwltool-3.1.20240508115724/cwltool.egg-info/top_level.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2024-05-16 12:29:52.000000 cwltool-3.1.20240508115724/cwltool.egg-info/zip-safe
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      335 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/cwltool.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.045050 cwltool-3.1.20240508115724/docs/
+-rw-r--r--   0 michael   (1000) michael   (1000)    18134 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/docs/CWLProv.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)      634 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/docs/Makefile
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.045050 cwltool-3.1.20240508115724/docs/_static/
+-rw-r--r--   0 michael   (1000) michael   (1000)    15086 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/docs/_static/favicon.ico
+-rw-r--r--   0 michael   (1000) michael   (1000)      126 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/docs/cli.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)     3569 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/docs/conf.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      248 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/docs/index.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)     6674 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/docs/loop.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)      795 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/docs/make.bat
+-rw-r--r--   0 michael   (1000) michael   (1000)     7683 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/docs/processgen.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)     2510 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/docs/pythonversions.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)      145 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/docs/requirements.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       42 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/lint-requirements.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      234 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-requirements.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.049050 cwltool-3.1.20240508115724/mypy-stubs/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.049050 cwltool-3.1.20240508115724/mypy-stubs/arcp/
+-rw-r--r--   0 michael   (1000) michael   (1000)      118 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/arcp/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      788 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/arcp/parse.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1736 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/bagit.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.049050 cwltool-3.1.20240508115724/mypy-stubs/black/
+-rw-r--r--   0 michael   (1000) michael   (1000)      469 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/black/__init__.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.049050 cwltool-3.1.20240508115724/mypy-stubs/coloredlogs/
+-rw-r--r--   0 michael   (1000) michael   (1000)      196 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/coloredlogs/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     7565 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/mistune.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.049050 cwltool-3.1.20240508115724/mypy-stubs/prov/
+-rw-r--r--   0 michael   (1000) michael   (1000)      170 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/prov/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     6855 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/prov/constants.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1721 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/prov/dot.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1498 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/prov/graph.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1060 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/prov/identifier.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)    15085 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/prov/model.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.049050 cwltool-3.1.20240508115724/mypy-stubs/prov/serializers/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1405 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/prov/serializers/provjson.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      255 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/prov/serializers/provn.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     3009 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/prov/serializers/provrdf.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      767 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/prov/serializers/provxml.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     5310 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/pydot.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.049050 cwltool-3.1.20240508115724/mypy-stubs/rdflib/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1292 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/rdflib/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      674 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/rdflib/collection.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     8337 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/rdflib/graph.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.053050 cwltool-3.1.20240508115724/mypy-stubs/rdflib/namespace/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2010 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/rdflib/namespace/_CSVW.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/rdflib/namespace/_DC.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1034 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/rdflib/namespace/_DCAT.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2361 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/rdflib/namespace/_DCTERMS.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1109 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/rdflib/namespace/_DOAP.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1847 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/rdflib/namespace/_FOAF.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     4691 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/rdflib/namespace/_ODRL2.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1259 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/rdflib/namespace/_ORG.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2260 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/rdflib/namespace/_OWL.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      441 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/rdflib/namespace/_PROF.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     4520 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/rdflib/namespace/_PROV.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1105 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/rdflib/namespace/_QB.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      620 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/rdflib/namespace/_RDF.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      519 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/rdflib/namespace/_RDFS.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)    41401 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/rdflib/namespace/_SDO.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     4965 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/rdflib/namespace/_SH.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      943 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/rdflib/namespace/_SKOS.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1075 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/rdflib/namespace/_SOSA.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      680 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/rdflib/namespace/_SSN.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2462 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/rdflib/namespace/_TIME.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      927 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/rdflib/namespace/_VOID.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1742 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/rdflib/namespace/_XSD.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2282 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/rdflib/namespace/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      131 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/rdflib/parser.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      724 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/rdflib/paths.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      325 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/rdflib/plugin.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.053050 cwltool-3.1.20240508115724/mypy-stubs/rdflib/plugins/
+-rw-r--r--   0 michael   (1000) michael   (1000)      118 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/rdflib/plugins/__init__.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.053050 cwltool-3.1.20240508115724/mypy-stubs/rdflib/plugins/parsers/
+-rw-r--r--   0 michael   (1000) michael   (1000)      126 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/rdflib/plugins/parsers/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)       34 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/rdflib/plugins/parsers/notation3.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1354 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/rdflib/query.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1370 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/rdflib/resource.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1337 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/rdflib/term.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.053050 cwltool-3.1.20240508115724/mypy-stubs/ruamel/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/ruamel/__init__.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.053050 cwltool-3.1.20240508115724/mypy-stubs/shellescape/
+-rw-r--r--   0 michael   (1000) michael   (1000)      147 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/shellescape/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      104 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/shellescape/main.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:45.957048 cwltool-3.1.20240508115724/mypy-stubs/spython/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.053050 cwltool-3.1.20240508115724/mypy-stubs/spython/main/
+-rw-r--r--   0 michael   (1000) michael   (1000)      190 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/spython/main/__init__.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.053050 cwltool-3.1.20240508115724/mypy-stubs/spython/main/base/
+-rw-r--r--   0 michael   (1000) michael   (1000)       84 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/spython/main/base/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      732 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/spython/main/build.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.053050 cwltool-3.1.20240508115724/mypy-stubs/spython/main/parse/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.057050 cwltool-3.1.20240508115724/mypy-stubs/spython/main/parse/parsers/
+-rw-r--r--   0 michael   (1000) michael   (1000)      363 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/spython/main/parse/parsers/base.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      239 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/spython/main/parse/parsers/docker.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      496 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/spython/main/parse/recipe.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.057050 cwltool-3.1.20240508115724/mypy-stubs/spython/main/parse/writers/
+-rw-r--r--   0 michael   (1000) michael   (1000)      236 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/spython/main/parse/writers/base.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      342 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy-stubs/spython/main/parse/writers/singularity.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      258 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/mypy.ini
+-rw-r--r--   0 michael   (1000) michael   (1000)      536 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/pyproject.toml
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     3174 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/release-test.sh
+-rw-r--r--   0 michael   (1000) michael   (1000)      382 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/requirements.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-05-16 12:40:46.101051 cwltool-3.1.20240508115724/setup.cfg
+-rw-r--r--   0 michael   (1000) michael   (1000)     6934 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/setup.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      359 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/test-requirements.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.069050 cwltool-3.1.20240508115724/tests/
+-rw-r--r--   0 michael   (1000) michael   (1000)      671 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/2.fasta
+-rw-r--r--   0 michael   (1000) michael   (1000)      255 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/2.fastq
+-rw-r--r--   0 michael   (1000) michael   (1000)       25 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      340 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/arg-empty-prefix-separate-false.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     3735 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/bundle-context.jsonld
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.069050 cwltool-3.1.20240508115724/tests/checker_wf/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1358 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/checker_wf/broken-wf.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1350 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/checker_wf/broken-wf2.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      776 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/checker_wf/broken-wf3.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      255 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/checker_wf/broken-wf4.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      196 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/checker_wf/cat-a.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      188 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/checker_wf/cat.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      543 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/checker_wf/circ-dep-wf.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      534 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/checker_wf/circ-dep-wf2.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      215 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/checker_wf/echo.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1283 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/checker_wf/functional-wf.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      185 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/checker_wf/ls.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      359 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/checker_wf/optional_array_mismatch.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)        2 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/checker_wf/test.txt
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      257 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/checker_wf/wc.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.069050 cwltool-3.1.20240508115724/tests/cwl-conformance/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1064 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/cwl-conformance/cwltool-conftest.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      205 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/debian_image_id.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      215 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/debian_image_id2.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      339 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/default_values_list.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      517 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/echo-badposition-expr.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      105 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/echo-job.yaml
+-rw-r--r--   0 michael   (1000) michael   (1000)       14 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/echo-position-expr-job.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/echo-position-expr.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      313 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/echo-stderr.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      178 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/echo-stdout-log-dir.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      297 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/echo.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      167 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/echo_broken_outputs.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      280 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/env.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      285 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/env2.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      145 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/env3.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      360 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/env4.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      157 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/env_with_software_req.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.069050 cwltool-3.1.20240508115724/tests/input_deps/
+-rw-r--r--   0 michael   (1000) michael   (1000)      202 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/input_deps/docker-array-secondaryfiles-job.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1081 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/input_deps/docker-array-secondaryfiles.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)    12010 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/input_deps/ref.fasta
+-rw-r--r--   0 michael   (1000) michael   (1000)      193 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/input_deps/ref.fasta.fai
+-rw-r--r--   0 michael   (1000) michael   (1000)    12010 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/input_deps/ref2.fasta
+-rw-r--r--   0 michael   (1000) michael   (1000)      193 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/input_deps/ref2.fasta.fai
+-rw-r--r--   0 michael   (1000) michael   (1000)      510 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/iwdr_bad_expr.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      506 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/iwdr_dir_literal_real_file.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       38 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/listing-job.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       38 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/listing2-job.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.073050 cwltool-3.1.20240508115724/tests/loop/
+-rw-r--r--   0 michael   (1000) michael   (1000)      590 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/loop/all-output-loop-no-iteration.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      591 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/loop/all-output-loop.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1038 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/loop/default-value-loop.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      558 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/loop/invalid-loop-command-line-tool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      409 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/loop/invalid-loop-expression-tool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      584 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/loop/invalid-loop-hint.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      725 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/loop/invalid-loop-scatter.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      733 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/loop/invalid-loop-when.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      695 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/loop/invalid-loop-workflow.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1518 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/loop/invalid-multi-source-loop-no-requirement.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      669 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/loop/invalid-no-loopWhen.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      700 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/loop/invalid-non-boolean-loopWhen.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      674 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/loop/invalid-value-from-loop-no-requirement.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1311 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/loop/loop-inside-loop-all.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1246 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/loop/loop-inside-loop.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       25 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/loop/loop-inside-scatter-job.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1076 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/loop/loop-inside-scatter.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1556 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/loop/multi-source-loop.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1052 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/loop/scatter-inside-loop.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)        5 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/loop/single-var-loop-job.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      590 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/loop/single-var-loop-no-iteration.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      591 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/loop/single-var-loop.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      637 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/loop/two-vars-loop-2.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       11 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/loop/two-vars-loop-job.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      691 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/loop/two-vars-loop.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      711 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/loop/value-from-loop.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      175 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/nested-array.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      371 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/non_portable.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      406 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/non_portable2.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.073050 cwltool-3.1.20240508115724/tests/override/
+-rw-r--r--   0 michael   (1000) michael   (1000)      125 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/override/echo-job-ov.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      144 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/override/echo-job-ov2.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)        8 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/override/echo-job.yml
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      211 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/override/echo-wf.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      427 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/override/echo.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      206 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/override/env-tool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      133 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/override/env-tool_cwl-requirement_override.yaml
+-rw-r--r--   0 michael   (1000) michael   (1000)      168 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/override/env-tool_cwl-requirement_override_default.yaml
+-rw-r--r--   0 michael   (1000) michael   (1000)      187 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/override/env-tool_cwl-requirement_override_default_wrongver.yaml
+-rw-r--r--   0 michael   (1000) michael   (1000)      213 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/override/env-tool_v1.1.0-dev1.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      206 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/override/env-tool_v1.1.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      116 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/override/ov.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      127 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/override/ov2.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      119 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/override/ov3.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      413 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/portable.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      530 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/random_lines.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      100 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/random_lines_job.json
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      533 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/random_lines_mapping.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.073050 cwltool-3.1.20240508115724/tests/reloc/
+-rw-r--r--   0 michael   (1000) michael   (1000)      268 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/reloc/test.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1063 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/scatter_numbers.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      620 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/secondary-files-bad.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       45 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/secondary-files-job.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      336 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/secondary-files-required-container.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      336 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/secondary-files-required-missing-container.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      369 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/secondary-files-string-v1.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      609 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/secondary-files.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      432 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/seqtk_seq.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       69 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/seqtk_seq_job.json
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      513 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/seqtk_seq_with_docker.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      539 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/seqtk_seq_wrong_name.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      206 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/sing_pullfolder_test.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.077051 cwltool-3.1.20240508115724/tests/subgraph/
+-rw-r--r--   0 michael   (1000) michael   (1000)      469 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/subgraph/1432.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      946 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/subgraph/count-lines1-wf.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     4722 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/subgraph/count-lines17-wf.cwl.json
+-rw-r--r--   0 michael   (1000) michael   (1000)       31 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/subgraph/env-job.json
+-rw-r--r--   0 michael   (1000) michael   (1000)      260 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/subgraph/env-tool2.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      190 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/subgraph/env-tool2_no_env.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/subgraph/env-tool2_req.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      298 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/subgraph/env-wf2.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      291 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/subgraph/env-wf2_hint_collision.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      295 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/subgraph/env-wf2_hint_req_collision.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      307 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/subgraph/env-wf2_long.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      315 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/subgraph/env-wf2_only_hint.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      302 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/subgraph/env-wf2_req_collision.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     3679 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/subgraph/env-wf2_subwf-packed.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      340 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/subgraph/env-wf2_subwf.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/subgraph/env-wf2_subwf_b.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1181 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/subgraph/extract_count_output.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     2623 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/subgraph/extract_file1.json
+-rw-r--r--   0 michael   (1000) michael   (1000)      854 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/subgraph/extract_file2.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1082 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/subgraph/extract_file3.json
+-rw-r--r--   0 michael   (1000) michael   (1000)      854 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/subgraph/extract_output3.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1232 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/subgraph/extract_output4.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1082 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/subgraph/extract_output5.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1788 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/subgraph/extract_step1.json
+-rw-r--r--   0 michael   (1000) michael   (1000)      810 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/subgraph/extract_step2.json
+-rw-r--r--   0 michael   (1000) michael   (1000)      818 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/subgraph/extract_step2_1432.json
+-rw-r--r--   0 michael   (1000) michael   (1000)      854 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/subgraph/extract_step3.json
+-rw-r--r--   0 michael   (1000) michael   (1000)      861 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/subgraph/extract_step4.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1082 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/subgraph/extract_step5.json
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      279 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/subgraph/parseInt-tool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1162 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/subgraph/single_step1.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1189 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/subgraph/single_step2.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1230 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/subgraph/single_step3.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1245 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/subgraph/single_step4.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1584 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/subgraph/single_step5.json
+-rw-r--r--   0 michael   (1000) michael   (1000)      538 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/subgraph/steplevel-resreq.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      803 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/subgraph/timelimit2-wf.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      301 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/subgraph/wc-tool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     5329 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_anon_types.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      558 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_bad_outputs_wf.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      377 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_check.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      563 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_conditionals.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      794 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_content_type.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      820 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_context.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     9278 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_cuda.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      369 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_cwl_version.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      562 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_default_path.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     5684 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_dependencies.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:45.957048 cwltool-3.1.20240508115724/tests/test_deps_env/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:45.957048 cwltool-3.1.20240508115724/tests/test_deps_env/modulefiles/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.077051 cwltool-3.1.20240508115724/tests/test_deps_env/modulefiles/random-lines/
+-rw-r--r--   0 michael   (1000) michael   (1000)      523 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_deps_env/modulefiles/random-lines/1.0
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:45.957048 cwltool-3.1.20240508115724/tests/test_deps_env/random-lines/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.077051 cwltool-3.1.20240508115724/tests/test_deps_env/random-lines/1.0/
+-rw-r--r--   0 michael   (1000) michael   (1000)      355 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_deps_env/random-lines/1.0/env.sh
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.077051 cwltool-3.1.20240508115724/tests/test_deps_env/random-lines/1.0/scripts/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2300 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_deps_env/random-lines/1.0/scripts/random-lines
+-rw-r--r--   0 michael   (1000) michael   (1000)       55 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_deps_env_modules_resolvers_conf.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       60 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_deps_env_resolvers_conf.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      106 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_deps_env_resolvers_conf_rewrite.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      101 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_deps_mapping.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     8162 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_docker.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      414 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_docker_info.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      845 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_docker_paths_with_colons.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      513 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_empty_input.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     8326 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_environment.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    64197 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_examples.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     7610 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_ext.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2533 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_fetch.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2487 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_http_input.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4335 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_input_deps.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    10932 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_iwdr.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4466 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_js_sandbox.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6991 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_load_tool.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     9409 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_loop.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1302 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_main_parsed_args.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      831 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_make_template.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2761 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_misc_cli.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    11905 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_mpi.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3979 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_override.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     7708 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_pack.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1126 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_parallel.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6928 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_path_checks.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2682 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_pathmapper.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1382 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_procgenerator.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    28315 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_provenance.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      589 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_rdfprint.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      527 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_recursive_validation.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2010 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_relocate.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      319 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_schemadef.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3034 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_secrets.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4597 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_singularity.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4458 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_singularity_versions.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1870 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_stdout_stderr_log_dir.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2726 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_streaming.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2289 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_subclass_mypyc.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    11067 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_subgraph.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      936 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_target.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    13557 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_tmpdir.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     5693 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_toolargparse.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4342 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_trs.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3580 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_udocker.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      746 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_user_agent.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1882 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_validate.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2170 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_validate_js.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      867 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/test_windows_warning.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:45.957048 cwltool-3.1.20240508115724/tests/tmp1/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:45.957048 cwltool-3.1.20240508115724/tests/tmp1/tmp2/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.077051 cwltool-3.1.20240508115724/tests/tmp1/tmp2/tmp3/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/tmp1/tmp2/tmp3/.gitkeep
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:45.957048 cwltool-3.1.20240508115724/tests/tmp4/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.081050 cwltool-3.1.20240508115724/tests/tmp4/alpha/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/tmp4/alpha/baker
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/tmp4/alpha/charlie
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/tmp4/alpha/delta
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/tmp4/alpha/echo
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/tmp4/alpha/foxtrot
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.081050 cwltool-3.1.20240508115724/tests/trs/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1505 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/trs/Dockstore.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      821 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/trs/md5sum-tool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/trs/md5sum-workflow.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      674 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/utf_doc_example.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     5261 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/util.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      236 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wc-tool-bad-hints.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wc-tool-bad-reqs.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.097051 cwltool-3.1.20240508115724/tests/wf/
+-rw-r--r--   0 michael   (1000) michael   (1000)      286 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/1496.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      468 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/1590.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      373 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/1st-workflow.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       51 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/1st-workflow_bad_inputs.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      181 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/811-12.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      178 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/811.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       26 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/811_inputs.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      212 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/816_tool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      155 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/816_wf.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      650 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/910.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      394 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/arguments.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      254 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/bad-stderr-expr.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      225 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/bad-stdin-expr.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      239 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/bad-stdout-expr.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      523 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/bad_formattest.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      533 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/bad_formattest2.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      222 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/bad_networkaccess.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/bad_timelimit.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      294 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/badout1.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      304 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/badout2.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      299 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/badout3.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      272 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/cache_test_workflow.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      289 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/cat-tool.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      130 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/cat.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      469 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/conditional_step_no_inputs.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      577 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/conflict.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      266 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/cores_float.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      388 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/count-lines1-wf.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      409 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/default-dir5.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/default-wf5.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      212 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/default_path.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      210 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/dir_deps.json
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1479 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/directory.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1420 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/double-nested.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      534 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/echo.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/empty.ttl
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/empty2.ttl
+-rw-r--r--   0 michael   (1000) michael   (1000)      922 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/expect_iwd-passthrough1_packed.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     4397 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/expect_packed.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     4564 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/expect_revsort_datetime_packed.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     4574 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/expect_trick_packed.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1262 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/extract_region_specs.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      619 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/floats_small_and_large.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      120 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/formattest-job.json
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      412 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/formattest.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.097051 cwltool-3.1.20240508115724/tests/wf/generator/
+-rw-r--r--   0 michael   (1000) michael   (1000)      710 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/generator/pytoolgen.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      275 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/generator/zing.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      672 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/hello-workflow-badhints.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      673 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/hello-workflow-badhints2.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      657 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/hello-workflow.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       35 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/hello.txt
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      168 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/hello_single_tool.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.097051 cwltool-3.1.20240508115724/tests/wf/indir/
+-rw-r--r--   0 michael   (1000) michael   (1000)        7 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/indir/hello2.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      213 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/input_named_id.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       37 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/input_named_id.yaml
+-rw-r--r--   0 michael   (1000) michael   (1000)      580 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/iwd-passthrough1.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      230 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/iwdr-empty.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      414 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/iwdr-entry.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1775 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/iwdr-passthrough-successive.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2268 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/iwdr_permutations.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      155 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/iwdr_permutations_inplace.yml
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1016 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/iwdr_permutations_nocontainer.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      284 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/js_output.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      364 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/js_output_workflow.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      291 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/listing_deep.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      276 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/listing_none.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      292 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/listing_shallow.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      158 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/listing_v1_0.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       35 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/literalfile-job.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      208 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/literalfile.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      111 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/malformed_outputs.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      145 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/missing-tool.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      548 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/missing_cwlVersion.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      249 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/mpi_env.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      645 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/mpi_expr.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       13 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/mpi_expr.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      401 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/mpi_line_count.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      471 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/mpi_simple.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      640 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/mpi_simple_wf.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      238 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/mut.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      299 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/mut2.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      281 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/mut3.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1107 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/nested.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      362 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/networkaccess-fail.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      425 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/networkaccess.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      233 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/no-parameters-echo.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      445 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/nvidia-smi-cc.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      434 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/nvidia-smi-container.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      382 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/nvidia-smi-max.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      408 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/nvidia-smi-range.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      429 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/nvidia-smi.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-16 12:40:46.097051 cwltool-3.1.20240508115724/tests/wf/operation/
+-rw-r--r--   0 michael   (1000) michael   (1000)      442 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/operation/abstract-cosifer.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     5209 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/operation/expect_operation-single_packed.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      969 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/operation/operation-single.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      337 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/optional-numerical-output-0.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      174 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/optional_src_mandatory_sink.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      221 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/override-no-secrets.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1921 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/packed-with-loadlisting.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1056 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/packed_no_main.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      786 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/paramref_arguments_roundtrip.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      877 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/paramref_arguments_self.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      279 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/parseInt-tool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      984 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/record_outputeval.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      377 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/resreq_expr_float_v1_0.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      377 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/resreq_expr_float_v1_2.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      181 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/revsort-job-shortcut.json
+-rw-r--r--   0 michael   (1000) michael   (1000)      152 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/revsort-job.json
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2331 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/revsort.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2447 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/revsort_datetime.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2317 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/revsort_step_bad_schema.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1367 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/revtool.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1471 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/revtool_bad_schema.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)       62 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/scatter-job2.json
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      927 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/scatter-wf4.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     2999 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/scatter-wf4.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1563 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/scatter2.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1805 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/scatter2_subwf.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      703 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/scatterfail.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)    94112 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/schemadef-bug-1473.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      412 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/schemadef-tool-12.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      412 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/schemadef-tool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      158 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/schemadef-type.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      163 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/sec-tool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      948 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/sec-wf-out.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      214 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/sec-wf.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      403 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/secret_job.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      380 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/secret_wf.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      363 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/separate_without_prefix.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      233 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/shm_size.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1101 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/sorttool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      391 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/storage_float.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      320 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/tar-param.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1124 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/three_step_color.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      222 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/timelimit-fail.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      277 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/timelimit.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      304 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/touch_tool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      278 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/trick_defaults.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      260 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/trick_defaults2.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2400 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/trick_revsort.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      318 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/updatedir.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      431 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/updatedir_inplace.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      488 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/updateval.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      102 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/updateval.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      603 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/updateval_inplace.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      382 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/vf-concat.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       82 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/wc-job.json
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      301 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/wc-tool.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      639 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/wffail.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1111 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/whale.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      329 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/workreuse-fail.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      392 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/workreuse.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      565 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/wf/wrong_cwlVersion.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      150 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/with_doc.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      107 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tests/without_doc.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     2094 2024-05-16 12:29:27.000000 cwltool-3.1.20240508115724/tox.ini
```

### Comparing `cwltool-3.1.20240404144621/.github/ISSUE_TEMPLATE.md` & `cwltool-3.1.20240508115724/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/.github/dependabot.yml` & `cwltool-3.1.20240508115724/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/.github/workflows/ci-tests.yml` & `cwltool-3.1.20240508115724/.github/workflows/ci-tests.yml`

 * *Files 2% similar despite different names*

```diff
@@ -200,15 +200,15 @@
           python-version: 3.12
           cache: pip
 
       - name: "Test CWL ${{ matrix.cwl-version }} conformance"
         env:
           VERSION: ${{ matrix.cwl-version }}
           CONTAINER: ${{ matrix.container }}
-          GIT_TARGET: ${{ matrix.cwl-version == 'v1.2' && '1.2.1_proposed' || 'main' }}
+          GIT_TARGET: main
           CWLTOOL_OPTIONS: ${{ matrix.cwl-version == 'v1.2' && '--relax-path-checks' || '' }} ${{ matrix.extras }}
         run: ./conformance-test.sh
       - name: Archive test results
         uses: actions/upload-artifact@v4
         with:
           name: cwl-${{ matrix.cwl-version }}-${{ matrix.container }}${{ matrix.extras }}-conformance-results
           path: |
@@ -262,15 +262,15 @@
       - name: record cwltool version
         run: pip install -U setuptools wheel && pip install setuptools_scm[toml] && python setup.py --version
       - name: build & test cwltool_module container
         run: ./build-cwltool-docker.sh
 
   macos:
     name: Test on macos-latest
-    runs-on: macos-latest
+    runs-on: macos-13  # not latest, that is now an Apple Silicon M1, for which seqtk is not yet built on bioconda
     env:
       TOXENV: py312-unit
     steps:
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0
       - name: Set up Python
```

### Comparing `cwltool-3.1.20240404144621/.github/workflows/codeql-analysis.yml` & `cwltool-3.1.20240508115724/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/.github/workflows/quay-publish.yml` & `cwltool-3.1.20240508115724/.github/workflows/quay-publish.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/.gitignore` & `cwltool-3.1.20240508115724/.gitignore`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/.mergify.yml` & `cwltool-3.1.20240508115724/.mergify.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/.readthedocs.yml` & `cwltool-3.1.20240508115724/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/CODE_OF_CONDUCT.md` & `cwltool-3.1.20240508115724/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/CONTRIBUTING.md` & `cwltool-3.1.20240508115724/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/LICENSE.txt` & `cwltool-3.1.20240508115724/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/MANIFEST.in` & `cwltool-3.1.20240508115724/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/Makefile` & `cwltool-3.1.20240508115724/Makefile`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/PKG-INFO` & `cwltool-3.1.20240508115724/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwltool
-Version: 3.1.20240404144621
+Version: 3.1.20240508115724
 Summary: Common workflow language reference implementation
 Home-page: https://github.com/common-workflow-language/cwltool
 Download-URL: https://github.com/common-workflow-language/cwltool
 Author: Common workflow language working group
 Author-email: common-workflow-language@googlegroups.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `cwltool-3.1.20240404144621/README.rst` & `cwltool-3.1.20240508115724/README.rst`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/build-cwltool-docker.sh` & `cwltool-3.1.20240508115724/build-cwltool-docker.sh`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/conformance-test.sh` & `cwltool-3.1.20240508115724/conformance-test.sh`

 * *Files 1% similar despite different names*

```diff
@@ -9,23 +9,23 @@
     fi
   fi
   # shellcheck source=/dev/null
   source "$1"/bin/activate
 }
 
 # Set these variables when running the script, e.g.:
-# VERSION=v1.2 GIT_TARGET=1.2.1_proposed CONTAINER=podman ./conformance_test.sh
+# VERSION=v1.2 GIT_TARGET=main CONTAINER=podman ./conformance_test.sh
 
 # Version of the standard to test against
 # Current options: v1.0, v1.1, v1.2
 VERSION=${VERSION:-"v1.2"}
 
 # Which commit of the standard's repo to use
-# Defaults to the last commit of the 1.2.1_proposed branch
-GIT_TARGET=${GIT_TARGET:-"1.2.1_proposed"}
+# Defaults to the last commit of the main branch
+GIT_TARGET=${GIT_TARGET:-"main"}
 
 # Which container runtime to use
 # Valid options: docker, singularity
 CONTAINER=${CONTAINER:-docker}
 
 # Comma-separated list of test names that should be excluded from execution
 # Defaults to "docker_entrypoint, inplace_update_on_file_content"
```

### Comparing `cwltool-3.1.20240404144621/cwlref-runner/setup.py` & `cwltool-3.1.20240508115724/cwlref-runner/setup.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/argparser.py` & `cwltool-3.1.20240508115724/cwltool/argparser.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/builder.py` & `cwltool-3.1.20240508115724/cwltool/builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     """
     Read a file as a string, respecting the :py:data:`~cwltool.utils.CONTENT_LIMIT`.
 
     :param f: file handle
     :returns: the file contents
     :raises WorkflowException: if the file is too large
     """
-    return content_limit_respected_read_bytes(f).decode("utf-8")
+    return str(content_limit_respected_read_bytes(f), "utf-8")
 
 
 def substitute(value: str, replace: str) -> str:
     """Perform CWL SecondaryFilesDSL style substitution."""
     if replace.startswith("^"):
         try:
             return substitute(value[0 : value.rindex(".")], replace[1:])
```

### Comparing `cwltool-3.1.20240404144621/cwltool/checker.py` & `cwltool-3.1.20240508115724/cwltool/checker.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/command_line_tool.py` & `cwltool-3.1.20240508115724/cwltool/command_line_tool.py`

 * *Files 0% similar despite different names*

```diff
@@ -1365,16 +1365,16 @@
                     if files["class"] == "Directory":
                         ll = binding.get("loadListing") or builder.loadListing
                         if ll and ll != "no_listing":
                             get_listing(fs_access, files, (ll == "deep_listing"))
                     else:
                         if binding.get("loadContents"):
                             with fs_access.open(cast(str, rfile["location"]), "rb") as f:
-                                files["contents"] = content_limit_respected_read_bytes(f).decode(
-                                    "utf-8"
+                                files["contents"] = str(
+                                    content_limit_respected_read_bytes(f), "utf-8"
                                 )
                         if compute_checksum:
                             with fs_access.open(cast(str, rfile["location"]), "rb") as f:
                                 checksum = hashlib.sha1()  # nosec
                                 contents = f.read(1024 * 1024)
                                 while contents != b"":
                                     checksum.update(contents)
```

### Comparing `cwltool-3.1.20240404144621/cwltool/context.py` & `cwltool-3.1.20240508115724/cwltool/context.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/cuda.py` & `cwltool-3.1.20240508115724/cwltool/cuda.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/cwlprov/__init__.py` & `cwltool-3.1.20240508115724/cwltool/cwlprov/__init__.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/cwlprov/provenance_constants.py` & `cwltool-3.1.20240508115724/cwltool/cwlprov/provenance_constants.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/cwlprov/provenance_profile.py` & `cwltool-3.1.20240508115724/cwltool/cwlprov/provenance_profile.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/cwlprov/ro.py` & `cwltool-3.1.20240508115724/cwltool/cwlprov/ro.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/cwlprov/writablebagfile.py` & `cwltool-3.1.20240508115724/cwltool/cwlprov/writablebagfile.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/cwlrdf.py` & `cwltool-3.1.20240508115724/cwltool/cwlrdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 
 def printrdf(wflow: Process, ctx: ContextType, style: str) -> str:
     """Serialize the CWL document into a string, ready for printing."""
     rdf = gather(wflow, ctx).serialize(format=style, encoding="utf-8")
     if not rdf:
         return ""
-    return rdf.decode("utf-8")
+    return str(rdf, "utf-8")
 
 
 def lastpart(uri: Any) -> str:
     uri2 = str(uri)
     if "/" in uri2:
         return uri2[uri2.rindex("/") + 1 :]
     return uri2
```

### Comparing `cwltool-3.1.20240404144621/cwltool/cwlviewer.py` & `cwltool-3.1.20240508115724/cwltool/cwlviewer.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/docker.py` & `cwltool-3.1.20240508115724/cwltool/docker.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,44 +112,46 @@
         with _IMAGES_LOCK:
             if docker_requirement["dockerImageId"] in _IMAGES:
                 return True
 
         if (docker_image_id := docker_requirement.get("dockerImageId")) is not None:
             try:
                 manifest = json.loads(
-                    subprocess.check_output(
-                        [self.docker_exec, "inspect", docker_image_id]
-                    ).decode(  # nosec
-                        "utf-8"
+                    str(
+                        subprocess.check_output(
+                            [self.docker_exec, "inspect", docker_image_id]
+                        ),  # nosec
+                        "utf-8",
                     )
                 )
                 found = manifest is not None
             except (OSError, subprocess.CalledProcessError, UnicodeError):
                 pass
 
+        cmd: List[str] = []
+        if "dockerFile" in docker_requirement:
+            dockerfile_dir = create_tmp_dir(tmp_outdir_prefix)
+            with open(os.path.join(dockerfile_dir, "Dockerfile"), "w") as dfile:
+                dfile.write(docker_requirement["dockerFile"])
+            cmd = [
+                self.docker_exec,
+                "build",
+                "--tag=%s" % str(docker_requirement["dockerImageId"]),
+                dockerfile_dir,
+            ]
+            _logger.info(str(cmd))
+            subprocess.check_call(cmd, stdout=sys.stderr)  # nosec
+            found = True
+
         if (force_pull or not found) and pull_image:
-            cmd: List[str] = []
             if "dockerPull" in docker_requirement:
                 cmd = [self.docker_exec, "pull", str(docker_requirement["dockerPull"])]
                 _logger.info(str(cmd))
                 subprocess.check_call(cmd, stdout=sys.stderr)  # nosec
                 found = True
-            elif "dockerFile" in docker_requirement:
-                dockerfile_dir = create_tmp_dir(tmp_outdir_prefix)
-                with open(os.path.join(dockerfile_dir, "Dockerfile"), "w") as dfile:
-                    dfile.write(docker_requirement["dockerFile"])
-                cmd = [
-                    self.docker_exec,
-                    "build",
-                    "--tag=%s" % str(docker_requirement["dockerImageId"]),
-                    dockerfile_dir,
-                ]
-                _logger.info(str(cmd))
-                subprocess.check_call(cmd, stdout=sys.stderr)  # nosec
-                found = True
             elif "dockerLoad" in docker_requirement:
                 cmd = [self.docker_exec, "load"]
                 _logger.info(str(cmd))
                 if os.path.exists(docker_requirement["dockerLoad"]):
                     _logger.info(
                         "Loading docker image from %s",
                         docker_requirement["dockerLoad"],
```

### Comparing `cwltool-3.1.20240404144621/cwltool/docker_id.py` & `cwltool-3.1.20240508115724/cwltool/docker_id.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/env_to_stdout.py` & `cwltool-3.1.20240508115724/cwltool/env_to_stdout.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/executors.py` & `cwltool-3.1.20240508115724/cwltool/executors.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/extensions-v1.1.yml` & `cwltool-3.1.20240508115724/cwltool/extensions-v1.1.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/extensions-v1.2.yml` & `cwltool-3.1.20240508115724/cwltool/extensions-v1.2.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/extensions.yml` & `cwltool-3.1.20240508115724/cwltool/extensions.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/factory.py` & `cwltool-3.1.20240508115724/cwltool/factory.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/flatten.py` & `cwltool-3.1.20240508115724/cwltool/flatten.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/hello.simg` & `cwltool-3.1.20240508115724/cwltool/hello.simg`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/job.py` & `cwltool-3.1.20240508115724/cwltool/job.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/jshint/jshint.js` & `cwltool-3.1.20240508115724/cwltool/jshint/jshint.js`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/jshint/jshint_wrapper.js` & `cwltool-3.1.20240508115724/cwltool/jshint/jshint_wrapper.js`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/load_tool.py` & `cwltool-3.1.20240508115724/cwltool/load_tool.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/loghandler.py` & `cwltool-3.1.20240508115724/cwltool/loghandler.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/main.py` & `cwltool-3.1.20240508115724/cwltool/main.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/mpi.py` & `cwltool-3.1.20240508115724/cwltool/mpi.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/mutation.py` & `cwltool-3.1.20240508115724/cwltool/mutation.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/pack.py` & `cwltool-3.1.20240508115724/cwltool/pack.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/pathmapper.py` & `cwltool-3.1.20240508115724/cwltool/pathmapper.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/process.py` & `cwltool-3.1.20240508115724/cwltool/process.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/procgenerator.py` & `cwltool-3.1.20240508115724/cwltool/procgenerator.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/rdfqueries/get_inner_edges.sparql` & `cwltool-3.1.20240508115724/cwltool/rdfqueries/get_inner_edges.sparql`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/rdfqueries/get_input_edges.sparql` & `cwltool-3.1.20240508115724/cwltool/rdfqueries/get_input_edges.sparql`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/rdfqueries/get_output_edges.sparql` & `cwltool-3.1.20240508115724/cwltool/rdfqueries/get_output_edges.sparql`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/rdfqueries/get_root.sparql` & `cwltool-3.1.20240508115724/cwltool/rdfqueries/get_root.sparql`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/resolver.py` & `cwltool-3.1.20240508115724/cwltool/resolver.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/run_job.py` & `cwltool-3.1.20240508115724/cwltool/run_job.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/CITATION` & `cwltool-3.1.20240508115724/cwltool/schemas/CITATION`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/CODE_OF_CONDUCT.md` & `cwltool-3.1.20240508115724/cwltool/schemas/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/LICENSE.txt` & `cwltool-3.1.20240508115724/cwltool/schemas/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/README.md` & `cwltool-3.1.20240508115724/cwltool/schemas/README.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.0/CommandLineTool.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.0/CommandLineTool.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.0/Process.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.0/Process.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.0/README.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.0/README.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.0/Workflow.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.0/Workflow.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.0/concepts.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.0/concepts.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.0/conformance_test_v1.0.yaml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.0/conformance_test_v1.0.yaml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.0/contrib.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.0/contrib.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.0/intro.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.0/intro.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.0/invocation.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.0/invocation.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/LICENSE.txt` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.0/salad/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/README.rst` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.0/salad/README.rst`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/field_name.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.0/salad/schema_salad/metaschema/field_name.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/ident_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.0/salad/schema_salad/metaschema/ident_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/import_include.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.0/salad/schema_salad/metaschema/import_include.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/link_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.0/salad/schema_salad/metaschema/link_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res_schema.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res_schema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/metaschema.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.0/salad/schema_salad/metaschema/metaschema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/metaschema_base.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.0/salad/schema_salad/metaschema/metaschema_base.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/salad.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.0/salad/schema_salad/metaschema/salad.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/typedsl_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.0/salad/schema_salad/metaschema/typedsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/vocab_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.0/salad/schema_salad/metaschema/vocab_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/CITATION` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1/CITATION`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/CODE_OF_CONDUCT.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/CONFORMANCE_TESTS.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1/CONFORMANCE_TESTS.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/CommandLineTool.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1/CommandLineTool.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/LICENSE.txt` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/Process.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1/Process.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/Workflow.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1/Workflow.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/concepts.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1/concepts.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/conformance_tests.yaml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1/conformance_tests.yaml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/contrib.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1/contrib.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/cwl-runner.cwl` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1/cwl-runner.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/index.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1/index.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/intro.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1/intro.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/invocation.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1/invocation.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/LICENSE.txt` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1/salad/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/README.rst` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1/salad/README.rst`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/field_name.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1/salad/schema_salad/metaschema/field_name.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/ident_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1/salad/schema_salad/metaschema/ident_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/import_include.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1/salad/schema_salad/metaschema/import_include.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/link_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1/salad/schema_salad/metaschema/link_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res_schema.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res_schema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/metaschema.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1/salad/schema_salad/metaschema/metaschema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/metaschema_base.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1/salad/schema_salad/metaschema/metaschema_base.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/salad.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1/salad/schema_salad/metaschema/salad.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/typedsl_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1/salad/schema_salad/metaschema/typedsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/vocab_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1/salad/schema_salad/metaschema/vocab_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/CommandLineTool.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/CommandLineTool.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/Process.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/Process.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/Workflow.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/Workflow.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/concepts.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/concepts.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/contrib.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/contrib.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/cwl-runner.cwl` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/cwl-runner.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/intro.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/intro.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/invocation.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/invocation.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/LICENSE.txt` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/salad/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/README.rst` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/salad/README.rst`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/field_name.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/field_name.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/ident_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/ident_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/import_include.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/import_include.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/link_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/link_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res_schema.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res_schema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/metaschema.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/metaschema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/metaschema_base.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/metaschema_base.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/salad.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/salad.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/typedsl_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/typedsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/vocab_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/vocab_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2/CODE_OF_CONDUCT.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2/CONFORMANCE_TESTS.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2/CONFORMANCE_TESTS.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2/CommandLineTool.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2/CommandLineTool.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2/Operation.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2/Operation.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2/Process.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2/Process.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2/Workflow.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2/Workflow.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2/concepts.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2/concepts.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2/contrib.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2/contrib.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2/index.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2/index.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2/intro.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2/intro.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2/invocation.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2/invocation.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/field_name.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2/salad/schema_salad/metaschema/field_name.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/ident_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2/salad/schema_salad/metaschema/ident_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/import_include.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2/salad/schema_salad/metaschema/import_include.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/link_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2/salad/schema_salad/metaschema/link_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res_schema.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res_schema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/metaschema.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2/salad/schema_salad/metaschema/metaschema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/metaschema_base.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2/salad/schema_salad/metaschema/metaschema_base.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/salad.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2/salad/schema_salad/metaschema/salad.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/sfdsl_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2/salad/schema_salad/metaschema/sfdsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/typedsl_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2/salad/schema_salad/metaschema/typedsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/vocab_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2/salad/schema_salad/metaschema/vocab_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/CommandLineTool.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/CommandLineTool.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/Process.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/Process.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/Workflow.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/Workflow.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/concepts.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/concepts.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/contrib.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/contrib.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/cwl-runner.cwl` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/cwl-runner.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/intro.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/intro.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/invocation.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/invocation.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/LICENSE.txt` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/README.rst` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/README.rst`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/field_name.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/field_name.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/ident_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/ident_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/import_include.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/import_include.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/link_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/link_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/map_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/map_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/map_res_schema.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/map_res_schema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/metaschema.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/metaschema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/metaschema_base.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/metaschema_base.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/salad.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/salad.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/sfdsl_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/sfdsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/typedsl_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/typedsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/vocab_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/vocab_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/CommandLineTool.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/CommandLineTool.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/Operation.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/Operation.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/Process.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/Process.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/Workflow.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/Workflow.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/concepts.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/concepts.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/contrib.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/contrib.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/cwl-runner.cwl` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/cwl-runner.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/intro.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/intro.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/invocation.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/invocation.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/LICENSE.txt` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/README.rst` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/README.rst`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/field_name.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/field_name.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/ident_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/ident_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/import_include.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/import_include.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/link_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/link_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res_schema.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res_schema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/metaschema.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/metaschema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/metaschema_base.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/metaschema_base.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/salad.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/salad.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/sfdsl_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/sfdsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/typedsl_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/typedsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/vocab_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/vocab_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/CommandLineTool.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/CommandLineTool.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/Operation.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/Operation.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/Process.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/Process.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/Workflow.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/Workflow.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/concepts.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/concepts.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/contrib.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/contrib.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/cwl-runner.cwl` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/cwl-runner.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/index.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/index.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/intro.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/intro.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/invocation.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/invocation.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/LICENSE.txt` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/README.rst` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/README.rst`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/field_name.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/field_name.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/ident_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/ident_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/import_include.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/import_include.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/link_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/link_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res_schema.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res_schema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/metaschema.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/metaschema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/metaschema_base.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/metaschema_base.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/salad.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/salad.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/sfdsl_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/sfdsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/typedsl_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/typedsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/vocab_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/vocab_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/CITATION` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/CITATION`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/CODE_OF_CONDUCT.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/CONFORMANCE_TESTS.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/CONFORMANCE_TESTS.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/CommandLineTool.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/CommandLineTool.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/LICENSE.txt` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/Operation.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/Operation.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/Process.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/Process.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/Workflow.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/Workflow.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/concepts.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/concepts.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/conformance_tests.yaml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/conformance_tests.yaml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/contrib.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/contrib.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/cwl-runner.cwl` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/cwl-runner.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/index.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/index.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/intro.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/intro.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/invocation.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/invocation.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/LICENSE.txt` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/README.rst` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/README.rst`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/field_name.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/field_name.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/ident_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/ident_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/import_include.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/import_include.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/link_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/link_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res_schema.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res_schema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/metaschema.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/metaschema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/metaschema_base.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/metaschema_base.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/salad.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/salad.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/sfdsl_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/sfdsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/typedsl_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/typedsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/vocab_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/vocab_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/CITATION` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/CITATION`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/CODE_OF_CONDUCT.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/CONFORMANCE_TESTS.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/CONFORMANCE_TESTS.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/CommandLineTool.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/CommandLineTool.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/LICENSE.txt` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/Operation.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/Operation.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/Process.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/Process.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/Workflow.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/Workflow.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/concepts.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/concepts.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/conformance_tests.yaml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/conformance_tests.yaml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/contrib.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/contrib.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/cwl-runner.cwl` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/cwl-runner.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/index.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/index.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/intro.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/intro.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/invocation.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/invocation.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/LICENSE.txt` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/README.rst` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/README.rst`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/field_name.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/field_name.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/ident_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/ident_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/import_include.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/import_include.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/link_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/link_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res_schema.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res_schema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/metaschema.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/metaschema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/metaschema_base.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/metaschema_base.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/salad.md` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/salad.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/sfdsl_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/sfdsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/typedsl_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/typedsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/vocab_res.yml` & `cwltool-3.1.20240508115724/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/vocab_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/secrets.py` & `cwltool-3.1.20240508115724/cwltool/secrets.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/singularity.py` & `cwltool-3.1.20240508115724/cwltool/singularity.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/singularity_utils.py` & `cwltool-3.1.20240508115724/cwltool/singularity_utils.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/software_requirements.py` & `cwltool-3.1.20240508115724/cwltool/software_requirements.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/stdfsaccess.py` & `cwltool-3.1.20240508115724/cwltool/stdfsaccess.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/subgraph.py` & `cwltool-3.1.20240508115724/cwltool/subgraph.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/task_queue.py` & `cwltool-3.1.20240508115724/cwltool/task_queue.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/udocker.py` & `cwltool-3.1.20240508115724/cwltool/udocker.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/update.py` & `cwltool-3.1.20240508115724/cwltool/update.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/utils.py` & `cwltool-3.1.20240508115724/cwltool/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,15 +196,15 @@
     if isinstance(inp, MutableSequence):
         for idx, value in enumerate(inp):
             inp[idx] = bytes2str_in_dicts(value)
             return inp
 
     # if value is bytes, return decoded string,
     elif isinstance(inp, bytes):
-        return inp.decode("utf-8")
+        return str(inp, "utf-8")
 
     # simply return elements itself
     return inp
 
 
 def visit_class(rec: Any, cls: Iterable[Any], op: Callable[..., Any]) -> None:
     """Apply a function to with "class" in cls."""
```

### Comparing `cwltool-3.1.20240404144621/cwltool/validate_js.py` & `cwltool-3.1.20240508115724/cwltool/validate_js.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/workflow.py` & `cwltool-3.1.20240508115724/cwltool/workflow.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool/workflow_job.py` & `cwltool-3.1.20240508115724/cwltool/workflow_job.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool-in-docker.sh` & `cwltool-3.1.20240508115724/cwltool-in-docker.sh`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool.Dockerfile` & `cwltool-3.1.20240508115724/cwltool.Dockerfile`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/cwltool.egg-info/PKG-INFO` & `cwltool-3.1.20240508115724/cwltool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwltool
-Version: 3.1.20240404144621
+Version: 3.1.20240508115724
 Summary: Common workflow language reference implementation
 Home-page: https://github.com/common-workflow-language/cwltool
 Download-URL: https://github.com/common-workflow-language/cwltool
 Author: Common workflow language working group
 Author-email: common-workflow-language@googlegroups.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `cwltool-3.1.20240404144621/cwltool.egg-info/SOURCES.txt` & `cwltool-3.1.20240508115724/cwltool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/docs/CWLProv.rst` & `cwltool-3.1.20240508115724/docs/CWLProv.rst`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/docs/Makefile` & `cwltool-3.1.20240508115724/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/docs/_static/favicon.ico` & `cwltool-3.1.20240508115724/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/docs/conf.py` & `cwltool-3.1.20240508115724/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/docs/loop.rst` & `cwltool-3.1.20240508115724/docs/loop.rst`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/docs/make.bat` & `cwltool-3.1.20240508115724/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/docs/processgen.rst` & `cwltool-3.1.20240508115724/docs/processgen.rst`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/docs/pythonversions.rst` & `cwltool-3.1.20240508115724/docs/pythonversions.rst`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/mypy-stubs/arcp/parse.pyi` & `cwltool-3.1.20240508115724/mypy-stubs/arcp/parse.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/mypy-stubs/bagit.pyi` & `cwltool-3.1.20240508115724/mypy-stubs/bagit.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/mypy-stubs/mistune.pyi` & `cwltool-3.1.20240508115724/mypy-stubs/mistune.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/mypy-stubs/prov/constants.py` & `cwltool-3.1.20240508115724/mypy-stubs/prov/constants.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/mypy-stubs/prov/dot.pyi` & `cwltool-3.1.20240508115724/mypy-stubs/prov/dot.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/mypy-stubs/prov/graph.pyi` & `cwltool-3.1.20240508115724/mypy-stubs/prov/graph.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/mypy-stubs/prov/identifier.pyi` & `cwltool-3.1.20240508115724/mypy-stubs/prov/identifier.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/mypy-stubs/prov/model.pyi` & `cwltool-3.1.20240508115724/mypy-stubs/prov/model.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/mypy-stubs/prov/serializers/provjson.pyi` & `cwltool-3.1.20240508115724/mypy-stubs/prov/serializers/provjson.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/mypy-stubs/prov/serializers/provrdf.pyi` & `cwltool-3.1.20240508115724/mypy-stubs/prov/serializers/provrdf.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/mypy-stubs/prov/serializers/provxml.pyi` & `cwltool-3.1.20240508115724/mypy-stubs/prov/serializers/provxml.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/mypy-stubs/pydot.pyi` & `cwltool-3.1.20240508115724/mypy-stubs/pydot.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/mypy-stubs/rdflib/__init__.pyi` & `cwltool-3.1.20240508115724/mypy-stubs/rdflib/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/mypy-stubs/rdflib/collection.pyi` & `cwltool-3.1.20240508115724/mypy-stubs/rdflib/collection.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/mypy-stubs/rdflib/graph.pyi` & `cwltool-3.1.20240508115724/mypy-stubs/rdflib/graph.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_CSVW.pyi` & `cwltool-3.1.20240508115724/mypy-stubs/rdflib/namespace/_CSVW.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_DCAT.pyi` & `cwltool-3.1.20240508115724/mypy-stubs/rdflib/namespace/_DCAT.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_DCTERMS.pyi` & `cwltool-3.1.20240508115724/mypy-stubs/rdflib/namespace/_DCTERMS.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_DOAP.pyi` & `cwltool-3.1.20240508115724/mypy-stubs/rdflib/namespace/_DOAP.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_FOAF.pyi` & `cwltool-3.1.20240508115724/mypy-stubs/rdflib/namespace/_FOAF.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_ODRL2.pyi` & `cwltool-3.1.20240508115724/mypy-stubs/rdflib/namespace/_ODRL2.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_ORG.pyi` & `cwltool-3.1.20240508115724/mypy-stubs/rdflib/namespace/_ORG.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_OWL.pyi` & `cwltool-3.1.20240508115724/mypy-stubs/rdflib/namespace/_OWL.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_PROV.pyi` & `cwltool-3.1.20240508115724/mypy-stubs/rdflib/namespace/_PROV.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_QB.pyi` & `cwltool-3.1.20240508115724/mypy-stubs/rdflib/namespace/_QB.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_RDF.pyi` & `cwltool-3.1.20240508115724/mypy-stubs/rdflib/namespace/_RDF.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_RDFS.pyi` & `cwltool-3.1.20240508115724/mypy-stubs/rdflib/namespace/_RDFS.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_SDO.pyi` & `cwltool-3.1.20240508115724/mypy-stubs/rdflib/namespace/_SDO.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_SH.pyi` & `cwltool-3.1.20240508115724/mypy-stubs/rdflib/namespace/_SH.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_SKOS.pyi` & `cwltool-3.1.20240508115724/mypy-stubs/rdflib/namespace/_SKOS.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_SOSA.pyi` & `cwltool-3.1.20240508115724/mypy-stubs/rdflib/namespace/_SOSA.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_SSN.pyi` & `cwltool-3.1.20240508115724/mypy-stubs/rdflib/namespace/_SSN.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_TIME.pyi` & `cwltool-3.1.20240508115724/mypy-stubs/rdflib/namespace/_TIME.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_VOID.pyi` & `cwltool-3.1.20240508115724/mypy-stubs/rdflib/namespace/_VOID.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_XSD.pyi` & `cwltool-3.1.20240508115724/mypy-stubs/rdflib/namespace/_XSD.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/__init__.pyi` & `cwltool-3.1.20240508115724/mypy-stubs/rdflib/namespace/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/mypy-stubs/rdflib/paths.pyi` & `cwltool-3.1.20240508115724/mypy-stubs/rdflib/paths.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/mypy-stubs/rdflib/query.pyi` & `cwltool-3.1.20240508115724/mypy-stubs/rdflib/query.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/mypy-stubs/rdflib/resource.pyi` & `cwltool-3.1.20240508115724/mypy-stubs/rdflib/resource.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/mypy-stubs/rdflib/term.pyi` & `cwltool-3.1.20240508115724/mypy-stubs/rdflib/term.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/mypy-stubs/spython/main/build.pyi` & `cwltool-3.1.20240508115724/mypy-stubs/spython/main/build.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/pyproject.toml` & `cwltool-3.1.20240508115724/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [build-system]
 requires = [
     "setuptools>=45",
     "setuptools_scm[toml]>=8.0.4,<9",
-    "mypy==1.9.0",  # also update mypy-requirements.txt
+    "mypy==1.10.0",  # also update mypy-requirements.txt
     "types-requests",
     "types-psutil",
     "importlib_resources>=1.4;python_version<'3.9'",
     "ruamel.yaml>=0.16.0,<0.18",
     "schema-salad>=8.4.20230426093816,<9",
     "cwl-utils>=0.32",
     "toml",
```

### Comparing `cwltool-3.1.20240404144621/release-test.sh` & `cwltool-3.1.20240508115724/release-test.sh`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         && pip install setuptools==${setuptoolsver} wheel
 # The following can fail if you haven't pushed your commits to ${repo}
 pip install -e "git+${repo}@${HEAD}#egg=${package}${extras}"
 pushd src/${package}
 pip install -rtest-requirements.txt build
 make dist
 #make test
-cp dist/${package}*tar.gz ../../../testenv3/
+cp dist/${module}*tar.gz ../../../testenv3/
 pip uninstall -y ${package} || true; pip uninstall -y ${package} || true; make install
 popd # ../.. no subdir named ${proj} here, safe for py.testing the installed module
 # shellcheck disable=SC2086
 #run_tests
 popd
 
 # Is the source distribution in testenv2 complete enough to build another
@@ -83,21 +83,21 @@
 
 pushd testenv3/
 # shellcheck source=/dev/null
 source bin/activate
 rm -f lib/python-wheels/setuptools* \
 	&& pip install --force-reinstall -U pip==${pipver} \
         && pip install setuptools==${setuptoolsver} wheel
-package_tar=$(find . -name "${package}*tar.gz")
+package_tar=$(find . -name "${module}*tar.gz")
 pip install "-r${DIR}/test-requirements.txt" udocker build
 pip install "${package_tar}${extras}"
 udocker install
 mkdir out
-tar --extract --directory=out -z -f ${package}*.tar.gz
-pushd out/${package}*
+tar --extract --directory=out -z -f ${module}*.tar.gz
+pushd out/${module}*
 make dist
 make test
 pip install "-r${DIR}/mypy-requirements.txt"
 make mypyc
 pip uninstall -y ${package} || true; pip uninstall -y ${package} || true; make install
 mkdir ../not-${module}
 pushd ../not-${module}
```

### Comparing `cwltool-3.1.20240404144621/setup.py` & `cwltool-3.1.20240508115724/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
     },
     python_requires=">=3.8, <4",
     use_scm_version=True,
     setup_requires=PYTEST_RUNNER + ["setuptools_scm>=8.0.4,<9"],
     test_suite="tests",
     tests_require=[
         "bagit >= 1.6.4, < 1.9",
-        "pytest >= 6.2, < 8.2",
+        "pytest >= 6.2, < 8.3",
         "mock >= 2.0.0",
         "pytest-mock >= 1.10.0",
         "pytest-httpserver",
         "arcp >= 0.2.0",
     ],
     entry_points={"console_scripts": ["cwltool=cwltool.main:run"]},
     zip_safe=True,
```

### Comparing `cwltool-3.1.20240404144621/tests/2.fasta` & `cwltool-3.1.20240508115724/tests/2.fasta`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/bundle-context.jsonld` & `cwltool-3.1.20240508115724/tests/bundle-context.jsonld`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/checker_wf/broken-wf.cwl` & `cwltool-3.1.20240508115724/tests/checker_wf/broken-wf.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/checker_wf/broken-wf2.cwl` & `cwltool-3.1.20240508115724/tests/checker_wf/broken-wf2.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/checker_wf/broken-wf3.cwl` & `cwltool-3.1.20240508115724/tests/checker_wf/broken-wf3.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/checker_wf/circ-dep-wf.cwl` & `cwltool-3.1.20240508115724/tests/checker_wf/circ-dep-wf.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/checker_wf/circ-dep-wf2.cwl` & `cwltool-3.1.20240508115724/tests/checker_wf/circ-dep-wf2.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/checker_wf/functional-wf.cwl` & `cwltool-3.1.20240508115724/tests/checker_wf/functional-wf.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/cwl-conformance/cwltool-conftest.py` & `cwltool-3.1.20240508115724/tests/cwl-conformance/cwltool-conftest.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/echo-badposition-expr.cwl` & `cwltool-3.1.20240508115724/tests/echo-badposition-expr.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/echo-position-expr.cwl` & `cwltool-3.1.20240508115724/tests/echo-position-expr.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/input_deps/docker-array-secondaryfiles.cwl` & `cwltool-3.1.20240508115724/tests/input_deps/docker-array-secondaryfiles.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/input_deps/ref.fasta` & `cwltool-3.1.20240508115724/tests/input_deps/ref.fasta`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/input_deps/ref2.fasta` & `cwltool-3.1.20240508115724/tests/input_deps/ref2.fasta`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/loop/all-output-loop-no-iteration.cwl` & `cwltool-3.1.20240508115724/tests/loop/all-output-loop-no-iteration.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/loop/all-output-loop.cwl` & `cwltool-3.1.20240508115724/tests/loop/all-output-loop.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/loop/default-value-loop.cwl` & `cwltool-3.1.20240508115724/tests/loop/default-value-loop.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/loop/invalid-loop-command-line-tool.cwl` & `cwltool-3.1.20240508115724/tests/loop/invalid-loop-command-line-tool.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/loop/invalid-loop-hint.cwl` & `cwltool-3.1.20240508115724/tests/loop/invalid-loop-hint.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/loop/invalid-loop-scatter.cwl` & `cwltool-3.1.20240508115724/tests/loop/invalid-loop-scatter.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/loop/invalid-loop-when.cwl` & `cwltool-3.1.20240508115724/tests/loop/invalid-loop-when.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/loop/invalid-loop-workflow.cwl` & `cwltool-3.1.20240508115724/tests/loop/invalid-loop-workflow.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/loop/invalid-multi-source-loop-no-requirement.cwl` & `cwltool-3.1.20240508115724/tests/loop/invalid-multi-source-loop-no-requirement.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/loop/invalid-no-loopWhen.cwl` & `cwltool-3.1.20240508115724/tests/loop/invalid-no-loopWhen.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/loop/invalid-non-boolean-loopWhen.cwl` & `cwltool-3.1.20240508115724/tests/loop/invalid-non-boolean-loopWhen.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/loop/invalid-value-from-loop-no-requirement.cwl` & `cwltool-3.1.20240508115724/tests/loop/invalid-value-from-loop-no-requirement.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/loop/loop-inside-loop-all.cwl` & `cwltool-3.1.20240508115724/tests/loop/loop-inside-loop-all.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/loop/loop-inside-loop.cwl` & `cwltool-3.1.20240508115724/tests/loop/loop-inside-loop.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/loop/loop-inside-scatter.cwl` & `cwltool-3.1.20240508115724/tests/loop/loop-inside-scatter.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/loop/multi-source-loop.cwl` & `cwltool-3.1.20240508115724/tests/loop/multi-source-loop.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/loop/scatter-inside-loop.cwl` & `cwltool-3.1.20240508115724/tests/loop/scatter-inside-loop.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/loop/single-var-loop-no-iteration.cwl` & `cwltool-3.1.20240508115724/tests/loop/single-var-loop-no-iteration.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/loop/single-var-loop.cwl` & `cwltool-3.1.20240508115724/tests/loop/single-var-loop.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/loop/two-vars-loop-2.cwl` & `cwltool-3.1.20240508115724/tests/loop/two-vars-loop-2.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/loop/two-vars-loop.cwl` & `cwltool-3.1.20240508115724/tests/loop/two-vars-loop.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/loop/value-from-loop.cwl` & `cwltool-3.1.20240508115724/tests/loop/value-from-loop.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/random_lines.cwl` & `cwltool-3.1.20240508115724/tests/random_lines.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/random_lines_mapping.cwl` & `cwltool-3.1.20240508115724/tests/random_lines_mapping.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/scatter_numbers.cwl` & `cwltool-3.1.20240508115724/tests/scatter_numbers.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/secondary-files-bad.cwl` & `cwltool-3.1.20240508115724/tests/secondary-files-bad.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/secondary-files.cwl` & `cwltool-3.1.20240508115724/tests/secondary-files.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/seqtk_seq_with_docker.cwl` & `cwltool-3.1.20240508115724/tests/seqtk_seq_with_docker.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/seqtk_seq_wrong_name.cwl` & `cwltool-3.1.20240508115724/tests/seqtk_seq_wrong_name.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/subgraph/count-lines1-wf.cwl` & `cwltool-3.1.20240508115724/tests/subgraph/count-lines1-wf.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/subgraph/count-lines17-wf.cwl.json` & `cwltool-3.1.20240508115724/tests/subgraph/count-lines17-wf.cwl.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/subgraph/env-wf2_subwf-packed.cwl` & `cwltool-3.1.20240508115724/tests/subgraph/env-wf2_subwf-packed.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/subgraph/extract_count_output.json` & `cwltool-3.1.20240508115724/tests/subgraph/extract_count_output.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/subgraph/extract_file1.json` & `cwltool-3.1.20240508115724/tests/subgraph/extract_file1.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/subgraph/extract_file2.json` & `cwltool-3.1.20240508115724/tests/subgraph/extract_file2.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/subgraph/extract_file3.json` & `cwltool-3.1.20240508115724/tests/subgraph/extract_file3.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/subgraph/extract_output3.json` & `cwltool-3.1.20240508115724/tests/subgraph/extract_output3.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/subgraph/extract_output4.json` & `cwltool-3.1.20240508115724/tests/subgraph/extract_output4.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/subgraph/extract_output5.json` & `cwltool-3.1.20240508115724/tests/subgraph/extract_output5.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/subgraph/extract_step1.json` & `cwltool-3.1.20240508115724/tests/subgraph/extract_step1.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/subgraph/extract_step2.json` & `cwltool-3.1.20240508115724/tests/subgraph/extract_step2.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/subgraph/extract_step2_1432.json` & `cwltool-3.1.20240508115724/tests/subgraph/extract_step2_1432.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/subgraph/extract_step3.json` & `cwltool-3.1.20240508115724/tests/subgraph/extract_step3.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/subgraph/extract_step4.json` & `cwltool-3.1.20240508115724/tests/subgraph/extract_step4.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/subgraph/extract_step5.json` & `cwltool-3.1.20240508115724/tests/subgraph/extract_step5.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/subgraph/single_step1.json` & `cwltool-3.1.20240508115724/tests/subgraph/single_step1.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/subgraph/single_step2.json` & `cwltool-3.1.20240508115724/tests/subgraph/single_step2.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/subgraph/single_step3.json` & `cwltool-3.1.20240508115724/tests/subgraph/single_step3.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/subgraph/single_step4.json` & `cwltool-3.1.20240508115724/tests/subgraph/single_step4.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/subgraph/single_step5.json` & `cwltool-3.1.20240508115724/tests/subgraph/single_step5.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/subgraph/steplevel-resreq.cwl` & `cwltool-3.1.20240508115724/tests/subgraph/steplevel-resreq.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/subgraph/timelimit2-wf.cwl` & `cwltool-3.1.20240508115724/tests/subgraph/timelimit2-wf.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_anon_types.py` & `cwltool-3.1.20240508115724/tests/test_anon_types.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_bad_outputs_wf.cwl` & `cwltool-3.1.20240508115724/tests/test_bad_outputs_wf.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_conditionals.py` & `cwltool-3.1.20240508115724/tests/test_conditionals.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_content_type.py` & `cwltool-3.1.20240508115724/tests/test_content_type.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_context.py` & `cwltool-3.1.20240508115724/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_cuda.py` & `cwltool-3.1.20240508115724/tests/test_cuda.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_default_path.py` & `cwltool-3.1.20240508115724/tests/test_default_path.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_dependencies.py` & `cwltool-3.1.20240508115724/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_deps_env/modulefiles/random-lines/1.0` & `cwltool-3.1.20240508115724/tests/test_deps_env/modulefiles/random-lines/1.0`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_deps_env/random-lines/1.0/scripts/random-lines` & `cwltool-3.1.20240508115724/tests/test_deps_env/random-lines/1.0/scripts/random-lines`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_docker.py` & `cwltool-3.1.20240508115724/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_docker_paths_with_colons.py` & `cwltool-3.1.20240508115724/tests/test_docker_paths_with_colons.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_empty_input.py` & `cwltool-3.1.20240508115724/tests/test_empty_input.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_environment.py` & `cwltool-3.1.20240508115724/tests/test_environment.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_examples.py` & `cwltool-3.1.20240508115724/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_ext.py` & `cwltool-3.1.20240508115724/tests/test_ext.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_fetch.py` & `cwltool-3.1.20240508115724/tests/test_fetch.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_http_input.py` & `cwltool-3.1.20240508115724/tests/test_http_input.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_input_deps.py` & `cwltool-3.1.20240508115724/tests/test_input_deps.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_iwdr.py` & `cwltool-3.1.20240508115724/tests/test_iwdr.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_js_sandbox.py` & `cwltool-3.1.20240508115724/tests/test_js_sandbox.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_load_tool.py` & `cwltool-3.1.20240508115724/tests/test_load_tool.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_loop.py` & `cwltool-3.1.20240508115724/tests/test_loop.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_main_parsed_args.py` & `cwltool-3.1.20240508115724/tests/test_main_parsed_args.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_make_template.py` & `cwltool-3.1.20240508115724/tests/test_make_template.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_misc_cli.py` & `cwltool-3.1.20240508115724/tests/test_misc_cli.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_mpi.py` & `cwltool-3.1.20240508115724/tests/test_mpi.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_override.py` & `cwltool-3.1.20240508115724/tests/test_override.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_pack.py` & `cwltool-3.1.20240508115724/tests/test_pack.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_parallel.py` & `cwltool-3.1.20240508115724/tests/test_parallel.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_path_checks.py` & `cwltool-3.1.20240508115724/tests/test_path_checks.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 from schema_salad.sourceline import cmap
 
 from cwltool.command_line_tool import CommandLineTool
 from cwltool.context import LoadingContext, RuntimeContext
 from cwltool.main import main
 from cwltool.stdfsaccess import StdFsAccess
 from cwltool.update import INTERNAL_VERSION
-from cwltool.utils import CWLObjectType
+from cwltool.utils import CWLObjectType, CONTENT_LIMIT, bytes2str_in_dicts
+from cwltool.builder import content_limit_respected_read
+from cwltool.errors import WorkflowException
 
 from .util import needs_docker
 
 script = """
 #!/usr/bin/env cwl-runner
 cwlVersion: v1.0
 class: CommandLineTool
@@ -210,7 +212,30 @@
     assert result["class"] == "File"
     assert result["basename"] == special
     assert result["nameroot"] == special
     assert (
         result["location"]
         == "keep:ae755cd1b3cff63152ff4200f4dea7e9+52/%3A%3F%23%5B%5D%40%21%24%26%27%28%29%2A%2B%2C%3B%3D"
     )
+
+
+def test_content_limit_respected_read() -> None:
+    b1 = b"abcd" * 100
+    b1io = BytesIO(b1)
+
+    assert len(b1) < CONTENT_LIMIT
+    assert content_limit_respected_read(b1io) == str("abcd" * 100)
+
+    b2 = b"abcd" * 20000
+    b2io = BytesIO(b2)
+
+    assert len(b2) > CONTENT_LIMIT
+    with pytest.raises(WorkflowException):
+        content_limit_respected_read(b2io)
+
+
+def test_bytes2str_in_dicts() -> None:
+    assert bytes2str_in_dicts({"foo": b"bar"}) == {"foo": "bar"}
+
+    assert bytes2str_in_dicts({"foo": [b"bar"]}) == {"foo": ["bar"]}
+
+    assert bytes2str_in_dicts({"foo": {"foo2": b"bar"}}) == {"foo": {"foo2": "bar"}}
```

### Comparing `cwltool-3.1.20240404144621/tests/test_pathmapper.py` & `cwltool-3.1.20240508115724/tests/test_pathmapper.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_procgenerator.py` & `cwltool-3.1.20240508115724/tests/test_procgenerator.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_provenance.py` & `cwltool-3.1.20240508115724/tests/test_provenance.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_rdfprint.py` & `cwltool-3.1.20240508115724/tests/test_rdfprint.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_recursive_validation.py` & `cwltool-3.1.20240508115724/tests/test_recursive_validation.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_relocate.py` & `cwltool-3.1.20240508115724/tests/test_relocate.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_secrets.py` & `cwltool-3.1.20240508115724/tests/test_secrets.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_singularity.py` & `cwltool-3.1.20240508115724/tests/test_singularity.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_singularity_versions.py` & `cwltool-3.1.20240508115724/tests/test_singularity_versions.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_stdout_stderr_log_dir.py` & `cwltool-3.1.20240508115724/tests/test_stdout_stderr_log_dir.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_streaming.py` & `cwltool-3.1.20240508115724/tests/test_streaming.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_subclass_mypyc.py` & `cwltool-3.1.20240508115724/tests/test_subclass_mypyc.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_subgraph.py` & `cwltool-3.1.20240508115724/tests/test_subgraph.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_target.py` & `cwltool-3.1.20240508115724/tests/test_target.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_tmpdir.py` & `cwltool-3.1.20240508115724/tests/test_tmpdir.py`

 * *Files 9% similar despite different names*

```diff
@@ -164,14 +164,72 @@
     children = sorted(tmp_outdir_prefix.parent.glob("*"))
     assert len(children) == 1
     subdir = tmp_path / children[0]
     assert len(sorted(subdir.glob("*"))) == 1
     assert (subdir / "Dockerfile").exists()
 
 
+@needs_docker
+def test_dockerfile_build(monkeypatch: pytest.MonkeyPatch, tmp_path: Path) -> None:
+    """Test that DockerCommandLineJob.get_image builds a Dockerfile."""
+    (tmp_path / "out").mkdir()
+    tmp_outdir_prefix = tmp_path / "out" / "1"
+    (tmp_path / "3").mkdir()
+    tmpdir_prefix = str(tmp_path / "3" / "ttmp")
+    runtime_context = RuntimeContext(
+        {"tmpdir_prefix": tmpdir_prefix, "user_space_docker_cmd": None}
+    )
+    builder = Builder(
+        {},
+        [],
+        [],
+        {},
+        schema.Names(),
+        [],
+        [],
+        {},
+        None,
+        None,
+        StdFsAccess,
+        StdFsAccess(""),
+        None,
+        0.1,
+        False,
+        False,
+        False,
+        "no_listing",
+        runtime_context.get_outdir(),
+        runtime_context.get_tmpdir(),
+        runtime_context.get_stagedir(),
+        INTERNAL_VERSION,
+        "docker",
+    )
+
+    docker_image_id = sys._getframe().f_code.co_name
+
+    assert DockerCommandLineJob(
+        builder, {}, CommandLineTool.make_path_mapper, [], [], ""
+    ).get_image(
+        {
+            "class": "DockerRequirement",
+            "dockerFile": "FROM debian:stable-slim",
+            "dockerImageId": docker_image_id,
+        },
+        pull_image=False,
+        force_pull=False,
+        tmp_outdir_prefix=str(tmp_outdir_prefix),
+    )
+    output = subprocess.check_output(
+        ["docker", "images", "--quiet", docker_image_id], stderr=subprocess.STDOUT, text=True
+    )
+
+    # If the output is empty, the image doesn't exist
+    assert output.strip(), f"Docker image {docker_image_id} does not exist"
+
+
 @needs_singularity
 def test_dockerfile_singularity_build(monkeypatch: pytest.MonkeyPatch, tmp_path: Path) -> None:
     """Test that SingularityCommandLineJob.get_image builds a Dockerfile with Singularity."""
     tmppath = Path(os.environ.get("APPTAINER_TMPDIR", tmp_path))
     # some HPC not allowed to execute on /tmp so allow user to define temp path with APPTAINER_TMPDIR
     # FATAL:   Unable to create build: 'noexec' mount option set on /tmp, temporary root filesystem
     monkeypatch.setattr(target=subprocess, name="check_call", value=lambda *args, **kwargs: True)
```

### Comparing `cwltool-3.1.20240404144621/tests/test_toolargparse.py` & `cwltool-3.1.20240508115724/tests/test_toolargparse.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_trs.py` & `cwltool-3.1.20240508115724/tests/test_trs.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_udocker.py` & `cwltool-3.1.20240508115724/tests/test_udocker.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_user_agent.py` & `cwltool-3.1.20240508115724/tests/test_user_agent.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_validate.py` & `cwltool-3.1.20240508115724/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_validate_js.py` & `cwltool-3.1.20240508115724/tests/test_validate_js.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/test_windows_warning.py` & `cwltool-3.1.20240508115724/tests/test_windows_warning.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/trs/Dockstore.cwl` & `cwltool-3.1.20240508115724/tests/trs/Dockstore.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/trs/md5sum-tool.cwl` & `cwltool-3.1.20240508115724/tests/trs/md5sum-tool.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/utf_doc_example.cwl` & `cwltool-3.1.20240508115724/tests/utf_doc_example.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/util.py` & `cwltool-3.1.20240508115724/tests/util.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/910.cwl` & `cwltool-3.1.20240508115724/tests/wf/910.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/bad_formattest.cwl` & `cwltool-3.1.20240508115724/tests/wf/bad_formattest.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/bad_formattest2.cwl` & `cwltool-3.1.20240508115724/tests/wf/bad_formattest2.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/conflict.cwl` & `cwltool-3.1.20240508115724/tests/wf/conflict.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/directory.cwl` & `cwltool-3.1.20240508115724/tests/wf/directory.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/double-nested.cwl` & `cwltool-3.1.20240508115724/tests/wf/double-nested.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/echo.cwl` & `cwltool-3.1.20240508115724/tests/wf/echo.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/expect_iwd-passthrough1_packed.cwl` & `cwltool-3.1.20240508115724/tests/wf/expect_iwd-passthrough1_packed.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/expect_packed.cwl` & `cwltool-3.1.20240508115724/tests/wf/expect_packed.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/expect_revsort_datetime_packed.cwl` & `cwltool-3.1.20240508115724/tests/wf/expect_revsort_datetime_packed.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/expect_trick_packed.cwl` & `cwltool-3.1.20240508115724/tests/wf/expect_trick_packed.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/extract_region_specs.cwl` & `cwltool-3.1.20240508115724/tests/wf/extract_region_specs.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/floats_small_and_large.cwl` & `cwltool-3.1.20240508115724/tests/wf/floats_small_and_large.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/generator/pytoolgen.cwl` & `cwltool-3.1.20240508115724/tests/wf/generator/pytoolgen.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/hello-workflow-badhints.cwl` & `cwltool-3.1.20240508115724/tests/wf/hello-workflow-badhints.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/hello-workflow-badhints2.cwl` & `cwltool-3.1.20240508115724/tests/wf/hello-workflow-badhints2.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/hello-workflow.cwl` & `cwltool-3.1.20240508115724/tests/wf/hello-workflow.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/iwd-passthrough1.cwl` & `cwltool-3.1.20240508115724/tests/wf/iwd-passthrough1.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/iwdr-passthrough-successive.cwl` & `cwltool-3.1.20240508115724/tests/wf/iwdr-passthrough-successive.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/iwdr_permutations.cwl` & `cwltool-3.1.20240508115724/tests/wf/iwdr_permutations.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/iwdr_permutations_nocontainer.cwl` & `cwltool-3.1.20240508115724/tests/wf/iwdr_permutations_nocontainer.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/missing_cwlVersion.cwl` & `cwltool-3.1.20240508115724/tests/wf/missing_cwlVersion.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/mpi_expr.cwl` & `cwltool-3.1.20240508115724/tests/wf/mpi_expr.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/mpi_simple_wf.cwl` & `cwltool-3.1.20240508115724/tests/wf/mpi_simple_wf.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/nested.cwl` & `cwltool-3.1.20240508115724/tests/wf/nested.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/operation/expect_operation-single_packed.cwl` & `cwltool-3.1.20240508115724/tests/wf/operation/expect_operation-single_packed.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/operation/operation-single.cwl` & `cwltool-3.1.20240508115724/tests/wf/operation/operation-single.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/packed-with-loadlisting.cwl` & `cwltool-3.1.20240508115724/tests/wf/packed-with-loadlisting.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/packed_no_main.cwl` & `cwltool-3.1.20240508115724/tests/wf/packed_no_main.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/paramref_arguments_roundtrip.cwl` & `cwltool-3.1.20240508115724/tests/wf/paramref_arguments_roundtrip.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/paramref_arguments_self.cwl` & `cwltool-3.1.20240508115724/tests/wf/paramref_arguments_self.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/record_outputeval.cwl` & `cwltool-3.1.20240508115724/tests/wf/record_outputeval.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/revsort.cwl` & `cwltool-3.1.20240508115724/tests/wf/revsort.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/revsort_datetime.cwl` & `cwltool-3.1.20240508115724/tests/wf/revsort_datetime.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/revsort_step_bad_schema.cwl` & `cwltool-3.1.20240508115724/tests/wf/revsort_step_bad_schema.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/revtool.cwl` & `cwltool-3.1.20240508115724/tests/wf/revtool.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/revtool_bad_schema.cwl` & `cwltool-3.1.20240508115724/tests/wf/revtool_bad_schema.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/scatter-wf4.cwl` & `cwltool-3.1.20240508115724/tests/wf/scatter-wf4.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/scatter-wf4.json` & `cwltool-3.1.20240508115724/tests/wf/scatter-wf4.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/scatter2.cwl` & `cwltool-3.1.20240508115724/tests/wf/scatter2.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/scatter2_subwf.cwl` & `cwltool-3.1.20240508115724/tests/wf/scatter2_subwf.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/scatterfail.cwl` & `cwltool-3.1.20240508115724/tests/wf/scatterfail.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/schemadef-bug-1473.cwl` & `cwltool-3.1.20240508115724/tests/wf/schemadef-bug-1473.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/sec-wf-out.cwl` & `cwltool-3.1.20240508115724/tests/wf/sec-wf-out.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/sorttool.cwl` & `cwltool-3.1.20240508115724/tests/wf/sorttool.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/three_step_color.cwl` & `cwltool-3.1.20240508115724/tests/wf/three_step_color.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/trick_revsort.cwl` & `cwltool-3.1.20240508115724/tests/wf/trick_revsort.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/updateval_inplace.cwl` & `cwltool-3.1.20240508115724/tests/wf/updateval_inplace.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/wffail.cwl` & `cwltool-3.1.20240508115724/tests/wf/wffail.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/whale.txt` & `cwltool-3.1.20240508115724/tests/wf/whale.txt`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tests/wf/wrong_cwlVersion.cwl` & `cwltool-3.1.20240508115724/tests/wf/wrong_cwlVersion.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240404144621/tox.ini` & `cwltool-3.1.20240508115724/tox.ini`

 * *Files identical despite different names*

