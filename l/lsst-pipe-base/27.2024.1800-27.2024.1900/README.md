# Comparing `tmp/lsst_pipe_base-27.2024.1800.tar.gz` & `tmp/lsst_pipe_base-27.2024.1900.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst_pipe_base-27.2024.1800.tar", last modified: Thu May  2 10:03:20 2024, max compression
+gzip compressed data, was "lsst_pipe_base-27.2024.1900.tar", last modified: Thu May  9 09:48:08 2024, max compression
```

## Comparing `lsst_pipe_base-27.2024.1800.tar` & `lsst_pipe_base-27.2024.1900.tar`

### file list

```diff
@@ -1,147 +1,147 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:03:20.076642 lsst_pipe_base-27.2024.1800/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-02 10:03:20.076642 lsst_pipe_base-27.2024.1800/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/bsd_license.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:03:20.052641 lsst_pipe_base-27.2024.1800/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:03:20.056642 lsst_pipe_base-27.2024.1800/doc/lsst.pipe.base/
--rw-r--r--   0 runner    (1001) docker     (127)    20761 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/doc/lsst.pipe.base/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)    25134 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/doc/lsst.pipe.base/creating-a-pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (127)    50486 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/doc/lsst.pipe.base/creating-a-pipelinetask.rst
--rw-r--r--   0 runner    (1001) docker     (127)    15015 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/doc/lsst.pipe.base/creating-a-task.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/doc/lsst.pipe.base/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/doc/lsst.pipe.base/task-framework-overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/doc/lsst.pipe.base/task-retargeting-howto.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11157 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/doc/lsst.pipe.base/testing-a-pipeline-task.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/doc/lsst.pipe.base/testing-pipelines-with-mocks.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7191 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/doc/lsst.pipe.base/working-with-pipeline-graphs.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/gpl-v3.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:03:20.052641 lsst_pipe_base-27.2024.1800/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:03:20.056642 lsst_pipe_base-27.2024.1800/python/lsst/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:03:20.056642 lsst_pipe_base-27.2024.1800/python/lsst/pipe/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:03:20.060642 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6366 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/_datasetQueryConstraints.py
--rw-r--r--   0 runner    (1001) docker     (127)    11352 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/_dataset_handle.py
--rw-r--r--   0 runner    (1001) docker     (127)    30075 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/_instrument.py
--rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/_observation_dimension_packer.py
--rw-r--r--   0 runner    (1001) docker     (127)    17530 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/_quantumContext.py
--rw-r--r--   0 runner    (1001) docker     (127)     8947 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    24451 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/_task_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    27546 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/all_dimensions_quantum_graph_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/automatic_connection_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7214 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/caching_limited_butler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:03:20.064642 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:03:20.064642 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/cli/cmd/
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/cli/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/cli/cmd/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:03:20.064642 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/cli/opt/
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/cli/opt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/cli/opt/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/cli/opt/options.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/cli/resources.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11983 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14661 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/configOverrides.py
--rw-r--r--   0 runner    (1001) docker     (127)    19386 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/connectionTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)    52230 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)    21283 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/executionButlerBuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)    16969 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/execution_reports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:03:20.064642 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/formatters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/formatters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/formatters/pexConfig.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:03:20.064642 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/graph/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/graph/_implDetails.py
--rw-r--r--   0 runner    (1001) docker     (127)    11857 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/graph/_loadHelpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    27987 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/graph/_versionDeserializers.py
--rw-r--r--   0 runner    (1001) docker     (127)    56203 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/graph/graphSummary.py
--rw-r--r--   0 runner    (1001) docker     (127)     7195 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/graph/quantumNode.py
--rw-r--r--   0 runner    (1001) docker     (127)     8036 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/graphBuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/pipeTools.py
--rw-r--r--   0 runner    (1001) docker     (127)    63422 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    43674 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/pipelineIR.py
--rw-r--r--   0 runner    (1001) docker     (127)     8381 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/pipelineTask.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:03:20.068642 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/pipeline_graph/
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/pipeline_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20859 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/pipeline_graph/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10392 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/pipeline_graph/_dataset_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    32831 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/pipeline_graph/_edges.py
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/pipeline_graph/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9194 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/pipeline_graph/_mapping_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/pipeline_graph/_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    75567 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/pipeline_graph/_pipeline_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/pipeline_graph/_task_subsets.py
--rw-r--r--   0 runner    (1001) docker     (127)    39356 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/pipeline_graph/_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)    29594 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/pipeline_graph/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:03:20.068642 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/pipeline_graph/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/pipeline_graph/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/pipeline_graph/visualization/_formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)    17157 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/pipeline_graph/visualization/_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)    15036 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/pipeline_graph/visualization/_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/pipeline_graph/visualization/_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    16537 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/pipeline_graph/visualization/_printer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8992 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/pipeline_graph/visualization/_show.py
--rw-r--r--   0 runner    (1001) docker     (127)    28590 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/prerequisite_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    54285 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/quantum_graph_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    18544 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/quantum_graph_skeleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:03:20.068642 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/script/
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/script/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/script/register_instrument.py
--rw-r--r--   0 runner    (1001) docker     (127)     6433 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/script/transfer_from_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/struct.py
--rw-r--r--   0 runner    (1001) docker     (127)    15145 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/taskFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)    18456 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/testUtils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:03:20.068642 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:03:20.068642 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/tests/mocks/_data_id_match.py
--rw-r--r--   0 runner    (1001) docker     (127)    27231 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/tests/mocks/_pipeline_task.py
--rw-r--r--   0 runner    (1001) docker     (127)    22758 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/tests/mocks/_storage_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     4710 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/tests/no_dimensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7011 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/tests/pipelineStepTester.py
--rw-r--r--   0 runner    (1001) docker     (127)    20810 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/tests/simpleQGraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-02 10:03:19.000000 lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:03:20.076642 lsst_pipe_base-27.2024.1800/python/lsst_pipe_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-02 10:03:20.000000 lsst_pipe_base-27.2024.1800/python/lsst_pipe_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-05-02 10:03:20.000000 lsst_pipe_base-27.2024.1800/python/lsst_pipe_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 10:03:20.000000 lsst_pipe_base-27.2024.1800/python/lsst_pipe_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-02 10:03:20.000000 lsst_pipe_base-27.2024.1800/python/lsst_pipe_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-02 10:03:20.000000 lsst_pipe_base-27.2024.1800/python/lsst_pipe_base.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 10:03:19.000000 lsst_pipe_base-27.2024.1800/python/lsst_pipe_base.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-02 10:03:20.076642 lsst_pipe_base-27.2024.1800/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:03:20.076642 lsst_pipe_base-27.2024.1800/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/tests/test_caching_limited_butler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/tests/test_cliCmdRegisterInstrument.py
--rw-r--r--   0 runner    (1001) docker     (127)    12290 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/tests/test_configOverrides.py
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/tests/test_config_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10061 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/tests/test_connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     6144 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/tests/test_dataid_match.py
--rw-r--r--   0 runner    (1001) docker     (127)     8118 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/tests/test_dataset_handle.py
--rw-r--r--   0 runner    (1001) docker     (127)    15553 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/tests/test_dynamic_connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/tests/test_executionButler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/tests/test_execution_reports.py
--rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/tests/test_graphBuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)    16055 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/tests/test_instrument.py
--rw-r--r--   0 runner    (1001) docker     (127)     7310 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    26529 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/tests/test_pipelineIR.py
--rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/tests/test_pipelineLoadSubset.py
--rw-r--r--   0 runner    (1001) docker     (127)    15977 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/tests/test_pipelineTask.py
--rw-r--r--   0 runner    (1001) docker     (127)    67752 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/tests/test_pipeline_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    26949 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/tests/test_quantumGraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/tests/test_struct.py
--rw-r--r--   0 runner    (1001) docker     (127)    13796 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/tests/test_task.py
--rw-r--r--   0 runner    (1001) docker     (127)    10424 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/tests/test_taskmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    24994 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/tests/test_testUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-02 10:03:13.000000 lsst_pipe_base-27.2024.1800/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:48:08.937228 lsst_pipe_base-27.2024.1900/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-09 09:48:08.937228 lsst_pipe_base-27.2024.1900/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/bsd_license.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:48:08.913228 lsst_pipe_base-27.2024.1900/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:48:08.917228 lsst_pipe_base-27.2024.1900/doc/lsst.pipe.base/
+-rw-r--r--   0 runner    (1001) docker     (127)    20761 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/doc/lsst.pipe.base/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    25134 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/doc/lsst.pipe.base/creating-a-pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    50486 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/doc/lsst.pipe.base/creating-a-pipelinetask.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15015 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/doc/lsst.pipe.base/creating-a-task.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/doc/lsst.pipe.base/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/doc/lsst.pipe.base/task-framework-overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/doc/lsst.pipe.base/task-retargeting-howto.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11157 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/doc/lsst.pipe.base/testing-a-pipeline-task.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/doc/lsst.pipe.base/testing-pipelines-with-mocks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7191 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/doc/lsst.pipe.base/working-with-pipeline-graphs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/gpl-v3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:48:08.917228 lsst_pipe_base-27.2024.1900/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:48:08.917228 lsst_pipe_base-27.2024.1900/python/lsst/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:48:08.917228 lsst_pipe_base-27.2024.1900/python/lsst/pipe/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:48:08.925228 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6366 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/_datasetQueryConstraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11352 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/_dataset_handle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30075 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/_instrument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/_observation_dimension_packer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17530 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/_quantumContext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8947 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24451 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/_task_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27546 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/all_dimensions_quantum_graph_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/automatic_connection_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7214 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/caching_limited_butler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:48:08.925228 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:48:08.925228 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/cli/cmd/
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/cli/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/cli/cmd/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:48:08.925228 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/cli/opt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/cli/opt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/cli/opt/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/cli/opt/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/cli/resources.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11983 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14661 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/configOverrides.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19386 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/connectionTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52230 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21283 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/executionButlerBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16969 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/execution_reports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:48:08.925228 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/formatters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/formatters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/formatters/pexConfig.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:48:08.925228 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/graph/_implDetails.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11857 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/graph/_loadHelpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27987 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/graph/_versionDeserializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56203 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/graph/graphSummary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7195 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/graph/quantumNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8036 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/graphBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/pipeTools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63422 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43674 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/pipelineIR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8381 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/pipelineTask.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:48:08.929228 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/pipeline_graph/
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/pipeline_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20859 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/pipeline_graph/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10392 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/pipeline_graph/_dataset_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32831 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/pipeline_graph/_edges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/pipeline_graph/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9194 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/pipeline_graph/_mapping_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/pipeline_graph/_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75567 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/pipeline_graph/_pipeline_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/pipeline_graph/_task_subsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39356 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/pipeline_graph/_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29594 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/pipeline_graph/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:48:08.929228 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/pipeline_graph/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/pipeline_graph/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/pipeline_graph/visualization/_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17157 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/pipeline_graph/visualization/_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15036 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/pipeline_graph/visualization/_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/pipeline_graph/visualization/_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16537 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/pipeline_graph/visualization/_printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8992 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/pipeline_graph/visualization/_show.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28590 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/prerequisite_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    54285 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/quantum_graph_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18544 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/quantum_graph_skeleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:48:08.929228 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/script/
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/script/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/script/register_instrument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6433 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/script/transfer_from_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15145 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/taskFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18456 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/testUtils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:48:08.929228 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:48:08.933228 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/tests/mocks/_data_id_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27231 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/tests/mocks/_pipeline_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22758 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/tests/mocks/_storage_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4710 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/tests/no_dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7011 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/tests/pipelineStepTester.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20810 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/tests/simpleQGraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-09 09:48:08.000000 lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:48:08.937228 lsst_pipe_base-27.2024.1900/python/lsst_pipe_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-09 09:48:08.000000 lsst_pipe_base-27.2024.1900/python/lsst_pipe_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-05-09 09:48:08.000000 lsst_pipe_base-27.2024.1900/python/lsst_pipe_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 09:48:08.000000 lsst_pipe_base-27.2024.1900/python/lsst_pipe_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-09 09:48:08.000000 lsst_pipe_base-27.2024.1900/python/lsst_pipe_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-09 09:48:08.000000 lsst_pipe_base-27.2024.1900/python/lsst_pipe_base.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 09:48:08.000000 lsst_pipe_base-27.2024.1900/python/lsst_pipe_base.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-09 09:48:08.937228 lsst_pipe_base-27.2024.1900/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:48:08.937228 lsst_pipe_base-27.2024.1900/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/tests/test_caching_limited_butler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/tests/test_cliCmdRegisterInstrument.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12290 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/tests/test_configOverrides.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/tests/test_config_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10061 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/tests/test_connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6144 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/tests/test_dataid_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8118 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/tests/test_dataset_handle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15553 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/tests/test_dynamic_connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/tests/test_executionButler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/tests/test_execution_reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/tests/test_graphBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16055 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/tests/test_instrument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7310 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26529 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/tests/test_pipelineIR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/tests/test_pipelineLoadSubset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15977 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/tests/test_pipelineTask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67752 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/tests/test_pipeline_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26949 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/tests/test_quantumGraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/tests/test_struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13796 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/tests/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10424 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/tests/test_taskmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24994 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/tests/test_testUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-09 09:48:02.000000 lsst_pipe_base-27.2024.1900/tests/test_utils.py
```

### Comparing `lsst_pipe_base-27.2024.1800/PKG-INFO` & `lsst_pipe_base-27.2024.1900/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-pipe-base
-Version: 27.2024.1800
+Version: 27.2024.1900
 Summary: Pipeline infrastructure for the Rubin Science Pipelines.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/pipe_base
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst_pipe_base-27.2024.1800/README.md` & `lsst_pipe_base-27.2024.1900/README.md`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/bsd_license.txt` & `lsst_pipe_base-27.2024.1900/bsd_license.txt`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/doc/lsst.pipe.base/CHANGES.rst` & `lsst_pipe_base-27.2024.1900/doc/lsst.pipe.base/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/doc/lsst.pipe.base/creating-a-pipeline.rst` & `lsst_pipe_base-27.2024.1900/doc/lsst.pipe.base/creating-a-pipeline.rst`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/doc/lsst.pipe.base/creating-a-pipelinetask.rst` & `lsst_pipe_base-27.2024.1900/doc/lsst.pipe.base/creating-a-pipelinetask.rst`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/doc/lsst.pipe.base/creating-a-task.rst` & `lsst_pipe_base-27.2024.1900/doc/lsst.pipe.base/creating-a-task.rst`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/doc/lsst.pipe.base/index.rst` & `lsst_pipe_base-27.2024.1900/doc/lsst.pipe.base/index.rst`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/doc/lsst.pipe.base/task-framework-overview.rst` & `lsst_pipe_base-27.2024.1900/doc/lsst.pipe.base/task-framework-overview.rst`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/doc/lsst.pipe.base/task-retargeting-howto.rst` & `lsst_pipe_base-27.2024.1900/doc/lsst.pipe.base/task-retargeting-howto.rst`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/doc/lsst.pipe.base/testing-a-pipeline-task.rst` & `lsst_pipe_base-27.2024.1900/doc/lsst.pipe.base/testing-a-pipeline-task.rst`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/doc/lsst.pipe.base/testing-pipelines-with-mocks.rst` & `lsst_pipe_base-27.2024.1900/doc/lsst.pipe.base/testing-pipelines-with-mocks.rst`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/doc/lsst.pipe.base/working-with-pipeline-graphs.rst` & `lsst_pipe_base-27.2024.1900/doc/lsst.pipe.base/working-with-pipeline-graphs.rst`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/gpl-v3.0.txt` & `lsst_pipe_base-27.2024.1900/gpl-v3.0.txt`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/pyproject.toml` & `lsst_pipe_base-27.2024.1900/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/__init__.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/_datasetQueryConstraints.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/_datasetQueryConstraints.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/_dataset_handle.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/_dataset_handle.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/_instrument.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/_instrument.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/_observation_dimension_packer.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/_observation_dimension_packer.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/_quantumContext.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/_quantumContext.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/_status.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/_status.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/_task_metadata.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/_task_metadata.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/all_dimensions_quantum_graph_builder.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/all_dimensions_quantum_graph_builder.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/automatic_connection_constants.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/automatic_connection_constants.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/caching_limited_butler.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/caching_limited_butler.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/cli/cmd/__init__.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/cli/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/cli/cmd/commands.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/cli/cmd/commands.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/cli/opt/__init__.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/cli/opt/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/cli/opt/arguments.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/cli/opt/arguments.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/cli/opt/options.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/cli/opt/options.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/config.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/config.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/configOverrides.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/configOverrides.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/connectionTypes.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/connectionTypes.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/connections.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/connections.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/executionButlerBuilder.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/executionButlerBuilder.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/execution_reports.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/execution_reports.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/formatters/pexConfig.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/formatters/pexConfig.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/graph/_implDetails.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/graph/_implDetails.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/graph/_loadHelpers.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/graph/_loadHelpers.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/graph/_versionDeserializers.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/graph/_versionDeserializers.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/graph/graph.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/graph/graph.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/graph/graphSummary.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/graph/graphSummary.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/graph/quantumNode.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/graph/quantumNode.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/graphBuilder.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/graphBuilder.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/pipeTools.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/pipeTools.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/pipeline.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/pipeline.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/pipelineIR.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/pipelineIR.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/pipelineTask.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/pipelineTask.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/pipeline_graph/__init__.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/pipeline_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/pipeline_graph/__main__.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/pipeline_graph/__main__.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/pipeline_graph/_dataset_types.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/pipeline_graph/_dataset_types.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/pipeline_graph/_edges.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/pipeline_graph/_edges.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/pipeline_graph/_exceptions.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/pipeline_graph/_exceptions.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/pipeline_graph/_mapping_views.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/pipeline_graph/_mapping_views.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/pipeline_graph/_nodes.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/pipeline_graph/_nodes.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/pipeline_graph/_pipeline_graph.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/pipeline_graph/_pipeline_graph.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/pipeline_graph/_task_subsets.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/pipeline_graph/_task_subsets.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/pipeline_graph/_tasks.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/pipeline_graph/_tasks.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/pipeline_graph/io.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/pipeline_graph/io.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/pipeline_graph/visualization/__init__.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/pipeline_graph/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/pipeline_graph/visualization/_formatting.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/pipeline_graph/visualization/_formatting.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/pipeline_graph/visualization/_layout.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/pipeline_graph/visualization/_layout.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/pipeline_graph/visualization/_merge.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/pipeline_graph/visualization/_merge.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/pipeline_graph/visualization/_options.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/pipeline_graph/visualization/_options.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/pipeline_graph/visualization/_printer.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/pipeline_graph/visualization/_printer.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/pipeline_graph/visualization/_show.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/pipeline_graph/visualization/_show.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/prerequisite_helpers.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/prerequisite_helpers.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/quantum_graph_builder.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/quantum_graph_builder.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/quantum_graph_skeleton.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/quantum_graph_skeleton.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/script/__init__.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/script/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/script/register_instrument.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/script/register_instrument.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/script/transfer_from_graph.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/script/transfer_from_graph.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/struct.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/struct.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/task.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/task.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/taskFactory.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/taskFactory.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/testUtils.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/testUtils.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/tests/mocks/__init__.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/tests/mocks/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/tests/mocks/_data_id_match.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/tests/mocks/_data_id_match.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/tests/mocks/_pipeline_task.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/tests/mocks/_pipeline_task.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/tests/mocks/_storage_class.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/tests/mocks/_storage_class.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/tests/no_dimensions.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/tests/no_dimensions.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/tests/pipelineStepTester.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/tests/pipelineStepTester.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/tests/simpleQGraph.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/tests/simpleQGraph.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/tests/util.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/tests/util.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst/pipe/base/utils.py` & `lsst_pipe_base-27.2024.1900/python/lsst/pipe/base/utils.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst_pipe_base.egg-info/PKG-INFO` & `lsst_pipe_base-27.2024.1900/python/lsst_pipe_base.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-pipe-base
-Version: 27.2024.1800
+Version: 27.2024.1900
 Summary: Pipeline infrastructure for the Rubin Science Pipelines.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/pipe_base
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst_pipe_base-27.2024.1800/python/lsst_pipe_base.egg-info/SOURCES.txt` & `lsst_pipe_base-27.2024.1900/python/lsst_pipe_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/tests/test_caching_limited_butler.py` & `lsst_pipe_base-27.2024.1900/tests/test_caching_limited_butler.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/tests/test_cliCmdRegisterInstrument.py` & `lsst_pipe_base-27.2024.1900/tests/test_cliCmdRegisterInstrument.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/tests/test_configOverrides.py` & `lsst_pipe_base-27.2024.1900/tests/test_configOverrides.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/tests/test_config_formatter.py` & `lsst_pipe_base-27.2024.1900/tests/test_config_formatter.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/tests/test_connections.py` & `lsst_pipe_base-27.2024.1900/tests/test_connections.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/tests/test_dataid_match.py` & `lsst_pipe_base-27.2024.1900/tests/test_dataid_match.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/tests/test_dataset_handle.py` & `lsst_pipe_base-27.2024.1900/tests/test_dataset_handle.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/tests/test_dynamic_connections.py` & `lsst_pipe_base-27.2024.1900/tests/test_dynamic_connections.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/tests/test_executionButler.py` & `lsst_pipe_base-27.2024.1900/tests/test_executionButler.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/tests/test_execution_reports.py` & `lsst_pipe_base-27.2024.1900/tests/test_execution_reports.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/tests/test_graphBuilder.py` & `lsst_pipe_base-27.2024.1900/tests/test_graphBuilder.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/tests/test_instrument.py` & `lsst_pipe_base-27.2024.1900/tests/test_instrument.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/tests/test_pipeline.py` & `lsst_pipe_base-27.2024.1900/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/tests/test_pipelineIR.py` & `lsst_pipe_base-27.2024.1900/tests/test_pipelineIR.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/tests/test_pipelineLoadSubset.py` & `lsst_pipe_base-27.2024.1900/tests/test_pipelineLoadSubset.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/tests/test_pipelineTask.py` & `lsst_pipe_base-27.2024.1900/tests/test_pipelineTask.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/tests/test_pipeline_graph.py` & `lsst_pipe_base-27.2024.1900/tests/test_pipeline_graph.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/tests/test_quantumGraph.py` & `lsst_pipe_base-27.2024.1900/tests/test_quantumGraph.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/tests/test_struct.py` & `lsst_pipe_base-27.2024.1900/tests/test_struct.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/tests/test_task.py` & `lsst_pipe_base-27.2024.1900/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/tests/test_taskmetadata.py` & `lsst_pipe_base-27.2024.1900/tests/test_taskmetadata.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/tests/test_testUtils.py` & `lsst_pipe_base-27.2024.1900/tests/test_testUtils.py`

 * *Files identical despite different names*

### Comparing `lsst_pipe_base-27.2024.1800/tests/test_utils.py` & `lsst_pipe_base-27.2024.1900/tests/test_utils.py`

 * *Files identical despite different names*

